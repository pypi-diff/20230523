# Comparing `tmp/asgi_matomo-0.3.1.tar.gz` & `tmp/asgi_matomo-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgi_matomo-0.3.1.tar", max compression
+gzip compressed data, was "asgi_matomo-0.3.2.tar", max compression
```

## Comparing `asgi_matomo-0.3.1.tar` & `asgi_matomo-0.3.2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-05-23 07:51:11.967823 asgi_matomo-0.3.1/LICENSE
--rw-r--r--   0        0        0     4381 2023-05-23 07:51:11.967823 asgi_matomo-0.3.1/README.md
--rw-r--r--   0        0        0       84 2023-05-23 07:51:11.967823 asgi_matomo-0.3.1/asgi_matomo/__init__.py
--rw-r--r--   0        0        0     9799 2023-05-23 07:51:11.971823 asgi_matomo-0.3.1/asgi_matomo/middleware.py
--rw-r--r--   0        0        0      879 2023-05-23 07:51:11.971823 asgi_matomo-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     5234 1970-01-01 00:00:00.000000 asgi_matomo-0.3.1/setup.py
--rw-r--r--   0        0        0     5114 1970-01-01 00:00:00.000000 asgi_matomo-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-23 11:34:01.134242 asgi_matomo-0.3.2/LICENSE
+-rw-r--r--   0        0        0     5278 2023-05-23 11:34:01.134242 asgi_matomo-0.3.2/README.md
+-rw-r--r--   0        0        0      186 2023-05-23 11:34:01.134242 asgi_matomo-0.3.2/asgi_matomo/__init__.py
+-rw-r--r--   0        0        0     9799 2023-05-23 11:34:01.134242 asgi_matomo-0.3.2/asgi_matomo/middleware.py
+-rw-r--r--   0        0        0     1024 2023-05-23 11:34:01.134242 asgi_matomo-0.3.2/asgi_matomo/trackers.py
+-rw-r--r--   0        0        0      879 2023-05-23 11:34:01.134242 asgi_matomo-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     6163 1970-01-01 00:00:00.000000 asgi_matomo-0.3.2/setup.py
+-rw-r--r--   0        0        0     6011 1970-01-01 00:00:00.000000 asgi_matomo-0.3.2/PKG-INFO
```

### Comparing `asgi_matomo-0.3.1/LICENSE` & `asgi_matomo-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `asgi_matomo-0.3.1/README.md` & `asgi_matomo-0.3.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # asgi-matomo
 [![Packaging status](https://img.shields.io/pypi/v/asgi-matomo?color=%2334D058&label=pypi%20package)](https://pypi.org/project/asgi-matomo)
 [![CI](https://github.com/spraakbanken/asgi-matomo/workflows/CI/badge.svg)](https://github.com/spraakbanken/asgi-matomo/actions?query=workflow%3ACI)
-[![Coverage](https://github.com/spraakbanken/asgi-matomo/workflows/Coverage/badge.svg)](https://github.com/spraakbanken/asgi-matomo/actions?query=workflow%3ACoverage)
 [![codecov](https://codecov.io/gh/spraakbanken/asgi-matomo/branch/main/graph/badge.svg?token=MRJZVCJQF5)](https://codecov.io/gh/spraakbanken/asgi-matomo)
 
 Tracking requests with Matomo from ASGI apps.
 
 `MatomoMiddleware` adds tracking of all requests to Matomo to ASGI applications (Starlette, FastAPI, Quart, etc.). The intended usage is for api tracking (backends).
 
 **Note** If you serve HTML (directly or by templates), it is suggested to track those parts through Matomo's javascript tracking.
@@ -22,14 +21,15 @@
 - `url`
 - `ua`: user_agent
 - `gt_ms`: mesaured as the time before and after this middleware call next in the asgi stack.
 - `send_image=0` for performance issues
 - `cvar` with at least `http_status_code` and `http_method` set.
 - `lang` if `accept-lang` is set
 - `cip` client ip, **requires** `access_token` to be given.
+- `action_name` that defaults to path, but can be specified.
 
 You can also pass variable to track by adding an `asgi_matomo`  dict in the `state` dict of the ASGI `scope`:
 ```python
 scope = {
   "state": {
     "asgi_matomo": {
       "e_a": "Playing",
@@ -40,14 +40,43 @@
     }
   }
 }
 ```
 
 The keys of the `asgi_matomo` dict is expected to be valid parameter for the [Matomo HTTP Tracking API](https://developer.matomo.org/api-reference/tracking-api). `cvar` is serialized with the standard `json` lib.
 
+You can also track time spent on different tasks with `trackers.PerfMsTracker`.
+```python
+import asyncio
+from starlette.applications import Starlette
+from starlette.responses import JSONResponse
+from starlette.routing import Route
+from starlette.middleware import Middleware
+
+from asgi_matomo import MatomoMiddleware
+from asgi_matomo.trackers import PerfMsTracker
+
+async def homepage(request):
+    async with PerfMsTracker(scope=request.scope, key="pf_srv"):
+        # fetch/compute data
+        await asyncio.sleep(1)
+        data = {"data": "a"*4000}
+    return JSONResponse(data)
+
+app = Starlette(
+  routes=[Route("/", homepage)],
+  middleware=[
+    Middleware(
+      MatomoMiddleware,
+      matomo_url="YOUR MATOMO TRACKING URL",
+      idsite=12345, # your service tracking id
+  )],
+)
+```
+
 ## Examples
 
 ### Starlette
 
 ```python
 from starlette.applications import Starlette
 from starlette.responses import JSONResponse
@@ -126,19 +155,22 @@
 - Currently only some parts [Matomo Tracking HTTP API](https://developer.matomo.org/api-reference/tracking-api) is supported.
 
 ## Ideas for further work:
 - [x] _filtering tracked of urls_
 - [x] _custom extraction of tracked data_
 
 
-This project keeps a [changelog](./CHANGELOG.md).
+This project keeps a [changelog](https://github.com/spraakbanken/asgi-matomo/CHANGELOG.md).
 
 # Releas Notes
 
 ## Latest Changes
 
+## [0.3.2] - 2023-05-23
+
+* feat: add PerfMsTracker. PR [#10](https://github.com/spraakbanken/asgi-matomo/pull/10) by [@kod-kristoff](https://github.com/kod-kristoff).
 
 ## [0.3.0] - 2023-05-22
 ### Added
 
 - Allow setting route-details
```

### Comparing `asgi_matomo-0.3.1/asgi_matomo/middleware.py` & `asgi_matomo-0.3.2/asgi_matomo/middleware.py`

 * *Files identical despite different names*

### Comparing `asgi_matomo-0.3.1/pyproject.toml` & `asgi_matomo-0.3.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asgi-matomo"
-version = "0.3.1"
+version = "0.3.2"
 description = "Middleware for tracking ASGI reqeusts with Matomo"
 authors = ["Kristoffer Andersson <kristoffer.andersson@gu.se>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://spraakbanken.gu.se"
 repository = "https://github.com/spraakbanken/asgi-matomo"
 packages = [{include = "asgi_matomo"}]
@@ -16,15 +16,15 @@
 python = "^3.10"
 asgiref = "^3.6.0"
 httpx = "^0.24.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 black = "^23.3.0"
-starlette = "^0.26.1"
+starlette = "^0.27.0"
 pytest-asyncio = "^0.21.0"
 asgi-lifespan = "^2.1.0"
 mypy = "^1.2.0"
 pytest-cov = "^4.0.0"
 bump2version = "^1.0.1"
 
 [tool.poetry.group.ci.dependencies]
```

### Comparing `asgi_matomo-0.3.1/setup.py` & `asgi_matomo-0.3.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['asgiref>=3.6.0,<4.0.0', 'httpx>=0.24.0,<0.25.0']
 
 setup_kwargs = {
     'name': 'asgi-matomo',
-    'version': '0.3.1',
+    'version': '0.3.2',
     'description': 'Middleware for tracking ASGI reqeusts with Matomo',
-    'long_description': '# asgi-matomo\n[![Packaging status](https://img.shields.io/pypi/v/asgi-matomo?color=%2334D058&label=pypi%20package)](https://pypi.org/project/asgi-matomo)\n[![CI](https://github.com/spraakbanken/asgi-matomo/workflows/CI/badge.svg)](https://github.com/spraakbanken/asgi-matomo/actions?query=workflow%3ACI)\n[![Coverage](https://github.com/spraakbanken/asgi-matomo/workflows/Coverage/badge.svg)](https://github.com/spraakbanken/asgi-matomo/actions?query=workflow%3ACoverage)\n[![codecov](https://codecov.io/gh/spraakbanken/asgi-matomo/branch/main/graph/badge.svg?token=MRJZVCJQF5)](https://codecov.io/gh/spraakbanken/asgi-matomo)\n\nTracking requests with Matomo from ASGI apps.\n\n`MatomoMiddleware` adds tracking of all requests to Matomo to ASGI applications (Starlette, FastAPI, Quart, etc.). The intended usage is for api tracking (backends).\n\n**Note** If you serve HTML (directly or by templates), it is suggested to track those parts through Matomo\'s javascript tracking.\n\n**Installation**\n\n```bash\npip install asgi-matomo\n```\n\n## What is tracked\n\nCurrently this middleware tracks:\n- `url`\n- `ua`: user_agent\n- `gt_ms`: mesaured as the time before and after this middleware call next in the asgi stack.\n- `send_image=0` for performance issues\n- `cvar` with at least `http_status_code` and `http_method` set.\n- `lang` if `accept-lang` is set\n- `cip` client ip, **requires** `access_token` to be given.\n\nYou can also pass variable to track by adding an `asgi_matomo`  dict in the `state` dict of the ASGI `scope`:\n```python\nscope = {\n  "state": {\n    "asgi_matomo": {\n      "e_a": "Playing",\n      "cvar": {\n        "your": "custom",\n        "data": "here",\n      }\n    }\n  }\n}\n```\n\nThe keys of the `asgi_matomo` dict is expected to be valid parameter for the [Matomo HTTP Tracking API](https://developer.matomo.org/api-reference/tracking-api). `cvar` is serialized with the standard `json` lib.\n\n## Examples\n\n### Starlette\n\n```python\nfrom starlette.applications import Starlette\nfrom starlette.responses import JSONResponse\nfrom starlette.routing import Route\nfrom starlette.middleware import Middleware\n\nfrom asgi_matomo import MatomoMiddleware\n\nasync def homepage(request):\n    return JSONResponse({"data": "a" * 4000})\n\napp = Starlette(\n  routes=[Route("/", homepage)],\n  middleware=[\n    Middleware(\n      MatomoMiddleware,\n      matomo_url="YOUR MATOMO TRACKING URL",\n      idsite=12345, # your service tracking id\n  )],\n)\n```\n\n### FastAPI\n\n```python\nfrom fastapi import FastAPI\nfrom asgi_matomo import MatomoMiddleware\n\napp = FastAPI()\napp.add_middleware(\n  BrotliMiddleware,\n  matomo_url="YOUR MATOMO TRACKING URL",\n  idsite=12345, # your service tracking id\n)\n\n@app.get("/")\ndef home() -> dict:\n    return {"data": "a" * 4000}\n```\n\n## API Reference\n\n**Overview**\n\n```python\napp.add_middleware(\n  MatomoMiddleware,\n  matomo_url="YOUR MATOMO TRACKING URL",\n  idsite=12345, # your service tracking id\n  access_token="SECRETTOKEN",\n  assume_https=True,\n  exclude_paths=["/health"],\n  exclude_patterns=[".*/old.*"],\n  route_details={\n    "route": {\n      "action_name": "Name",\n    }\n  }\n)\n```\n\n**Parameters**:\n\n- **(Required)** `matomo_url`: The URL to make your tracking calls to.\n- **(Required)** `idsite`: The tracking id for your service.\n- _(Optional)_ `access_token`: Access token for Matomo. If this is set `cip` is also tracked. Required for tracking some data.\n- _(Optional)_ `assume_https`: If `True`, set tracked url scheme to `https`, useful when running behind a proxy. Defaults to `True`.\n- _(Optional)_ `exclude_paths`: A list of paths to exclude, only excludes path that is equal to a path in this list. These are tried before `exclude_patterns`. Defaults to `None`.\n- _(Optional)_ `exclude_patterns`: A list of regex patterns that are compiled, and then exclude a path from tracking if any pattern match. Defaults to `None`.\nThese are tried after `exclude_paths`.\n- _(Optional)_ `route_details`: A dict with custom route-specific tracking data. Defaults to `None`.\n\n\n**Notes**:\n\n- Currently only some parts [Matomo Tracking HTTP API](https://developer.matomo.org/api-reference/tracking-api) is supported.\n\n## Ideas for further work:\n- [x] _filtering tracked of urls_\n- [x] _custom extraction of tracked data_\n\n\nThis project keeps a [changelog](./CHANGELOG.md).\n\n# Releas Notes\n\n## Latest Changes\n\n\n## [0.3.0] - 2023-05-22\n### Added\n\n- Allow setting route-details\n\n',
+    'long_description': '# asgi-matomo\n[![Packaging status](https://img.shields.io/pypi/v/asgi-matomo?color=%2334D058&label=pypi%20package)](https://pypi.org/project/asgi-matomo)\n[![CI](https://github.com/spraakbanken/asgi-matomo/workflows/CI/badge.svg)](https://github.com/spraakbanken/asgi-matomo/actions?query=workflow%3ACI)\n[![codecov](https://codecov.io/gh/spraakbanken/asgi-matomo/branch/main/graph/badge.svg?token=MRJZVCJQF5)](https://codecov.io/gh/spraakbanken/asgi-matomo)\n\nTracking requests with Matomo from ASGI apps.\n\n`MatomoMiddleware` adds tracking of all requests to Matomo to ASGI applications (Starlette, FastAPI, Quart, etc.). The intended usage is for api tracking (backends).\n\n**Note** If you serve HTML (directly or by templates), it is suggested to track those parts through Matomo\'s javascript tracking.\n\n**Installation**\n\n```bash\npip install asgi-matomo\n```\n\n## What is tracked\n\nCurrently this middleware tracks:\n- `url`\n- `ua`: user_agent\n- `gt_ms`: mesaured as the time before and after this middleware call next in the asgi stack.\n- `send_image=0` for performance issues\n- `cvar` with at least `http_status_code` and `http_method` set.\n- `lang` if `accept-lang` is set\n- `cip` client ip, **requires** `access_token` to be given.\n- `action_name` that defaults to path, but can be specified.\n\nYou can also pass variable to track by adding an `asgi_matomo`  dict in the `state` dict of the ASGI `scope`:\n```python\nscope = {\n  "state": {\n    "asgi_matomo": {\n      "e_a": "Playing",\n      "cvar": {\n        "your": "custom",\n        "data": "here",\n      }\n    }\n  }\n}\n```\n\nThe keys of the `asgi_matomo` dict is expected to be valid parameter for the [Matomo HTTP Tracking API](https://developer.matomo.org/api-reference/tracking-api). `cvar` is serialized with the standard `json` lib.\n\nYou can also track time spent on different tasks with `trackers.PerfMsTracker`.\n```python\nimport asyncio\nfrom starlette.applications import Starlette\nfrom starlette.responses import JSONResponse\nfrom starlette.routing import Route\nfrom starlette.middleware import Middleware\n\nfrom asgi_matomo import MatomoMiddleware\nfrom asgi_matomo.trackers import PerfMsTracker\n\nasync def homepage(request):\n    async with PerfMsTracker(scope=request.scope, key="pf_srv"):\n        # fetch/compute data\n        await asyncio.sleep(1)\n        data = {"data": "a"*4000}\n    return JSONResponse(data)\n\napp = Starlette(\n  routes=[Route("/", homepage)],\n  middleware=[\n    Middleware(\n      MatomoMiddleware,\n      matomo_url="YOUR MATOMO TRACKING URL",\n      idsite=12345, # your service tracking id\n  )],\n)\n```\n\n## Examples\n\n### Starlette\n\n```python\nfrom starlette.applications import Starlette\nfrom starlette.responses import JSONResponse\nfrom starlette.routing import Route\nfrom starlette.middleware import Middleware\n\nfrom asgi_matomo import MatomoMiddleware\n\nasync def homepage(request):\n    return JSONResponse({"data": "a" * 4000})\n\napp = Starlette(\n  routes=[Route("/", homepage)],\n  middleware=[\n    Middleware(\n      MatomoMiddleware,\n      matomo_url="YOUR MATOMO TRACKING URL",\n      idsite=12345, # your service tracking id\n  )],\n)\n```\n\n### FastAPI\n\n```python\nfrom fastapi import FastAPI\nfrom asgi_matomo import MatomoMiddleware\n\napp = FastAPI()\napp.add_middleware(\n  BrotliMiddleware,\n  matomo_url="YOUR MATOMO TRACKING URL",\n  idsite=12345, # your service tracking id\n)\n\n@app.get("/")\ndef home() -> dict:\n    return {"data": "a" * 4000}\n```\n\n## API Reference\n\n**Overview**\n\n```python\napp.add_middleware(\n  MatomoMiddleware,\n  matomo_url="YOUR MATOMO TRACKING URL",\n  idsite=12345, # your service tracking id\n  access_token="SECRETTOKEN",\n  assume_https=True,\n  exclude_paths=["/health"],\n  exclude_patterns=[".*/old.*"],\n  route_details={\n    "route": {\n      "action_name": "Name",\n    }\n  }\n)\n```\n\n**Parameters**:\n\n- **(Required)** `matomo_url`: The URL to make your tracking calls to.\n- **(Required)** `idsite`: The tracking id for your service.\n- _(Optional)_ `access_token`: Access token for Matomo. If this is set `cip` is also tracked. Required for tracking some data.\n- _(Optional)_ `assume_https`: If `True`, set tracked url scheme to `https`, useful when running behind a proxy. Defaults to `True`.\n- _(Optional)_ `exclude_paths`: A list of paths to exclude, only excludes path that is equal to a path in this list. These are tried before `exclude_patterns`. Defaults to `None`.\n- _(Optional)_ `exclude_patterns`: A list of regex patterns that are compiled, and then exclude a path from tracking if any pattern match. Defaults to `None`.\nThese are tried after `exclude_paths`.\n- _(Optional)_ `route_details`: A dict with custom route-specific tracking data. Defaults to `None`.\n\n\n**Notes**:\n\n- Currently only some parts [Matomo Tracking HTTP API](https://developer.matomo.org/api-reference/tracking-api) is supported.\n\n## Ideas for further work:\n- [x] _filtering tracked of urls_\n- [x] _custom extraction of tracked data_\n\n\nThis project keeps a [changelog](https://github.com/spraakbanken/asgi-matomo/CHANGELOG.md).\n\n# Releas Notes\n\n## Latest Changes\n\n## [0.3.2] - 2023-05-23\n\n* feat: add PerfMsTracker. PR [#10](https://github.com/spraakbanken/asgi-matomo/pull/10) by [@kod-kristoff](https://github.com/kod-kristoff).\n\n## [0.3.0] - 2023-05-22\n### Added\n\n- Allow setting route-details\n\n',
     'author': 'Kristoffer Andersson',
     'author_email': 'kristoffer.andersson@gu.se',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://spraakbanken.gu.se',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `asgi_matomo-0.3.1/PKG-INFO` & `asgi_matomo-0.3.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asgi-matomo
-Version: 0.3.1
+Version: 0.3.2
 Summary: Middleware for tracking ASGI reqeusts with Matomo
 Home-page: https://spraakbanken.gu.se
 License: MIT
 Author: Kristoffer Andersson
 Author-email: kristoffer.andersson@gu.se
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,14 @@
 Project-URL: Bug Tracker, https://github.com/spraakbanken/asgi-matomo/issues
 Project-URL: Repository, https://github.com/spraakbanken/asgi-matomo
 Description-Content-Type: text/markdown
 
 # asgi-matomo
 [![Packaging status](https://img.shields.io/pypi/v/asgi-matomo?color=%2334D058&label=pypi%20package)](https://pypi.org/project/asgi-matomo)
 [![CI](https://github.com/spraakbanken/asgi-matomo/workflows/CI/badge.svg)](https://github.com/spraakbanken/asgi-matomo/actions?query=workflow%3ACI)
-[![Coverage](https://github.com/spraakbanken/asgi-matomo/workflows/Coverage/badge.svg)](https://github.com/spraakbanken/asgi-matomo/actions?query=workflow%3ACoverage)
 [![codecov](https://codecov.io/gh/spraakbanken/asgi-matomo/branch/main/graph/badge.svg?token=MRJZVCJQF5)](https://codecov.io/gh/spraakbanken/asgi-matomo)
 
 Tracking requests with Matomo from ASGI apps.
 
 `MatomoMiddleware` adds tracking of all requests to Matomo to ASGI applications (Starlette, FastAPI, Quart, etc.). The intended usage is for api tracking (backends).
 
 **Note** If you serve HTML (directly or by templates), it is suggested to track those parts through Matomo's javascript tracking.
@@ -41,14 +40,15 @@
 - `url`
 - `ua`: user_agent
 - `gt_ms`: mesaured as the time before and after this middleware call next in the asgi stack.
 - `send_image=0` for performance issues
 - `cvar` with at least `http_status_code` and `http_method` set.
 - `lang` if `accept-lang` is set
 - `cip` client ip, **requires** `access_token` to be given.
+- `action_name` that defaults to path, but can be specified.
 
 You can also pass variable to track by adding an `asgi_matomo`  dict in the `state` dict of the ASGI `scope`:
 ```python
 scope = {
   "state": {
     "asgi_matomo": {
       "e_a": "Playing",
@@ -59,14 +59,43 @@
     }
   }
 }
 ```
 
 The keys of the `asgi_matomo` dict is expected to be valid parameter for the [Matomo HTTP Tracking API](https://developer.matomo.org/api-reference/tracking-api). `cvar` is serialized with the standard `json` lib.
 
+You can also track time spent on different tasks with `trackers.PerfMsTracker`.
+```python
+import asyncio
+from starlette.applications import Starlette
+from starlette.responses import JSONResponse
+from starlette.routing import Route
+from starlette.middleware import Middleware
+
+from asgi_matomo import MatomoMiddleware
+from asgi_matomo.trackers import PerfMsTracker
+
+async def homepage(request):
+    async with PerfMsTracker(scope=request.scope, key="pf_srv"):
+        # fetch/compute data
+        await asyncio.sleep(1)
+        data = {"data": "a"*4000}
+    return JSONResponse(data)
+
+app = Starlette(
+  routes=[Route("/", homepage)],
+  middleware=[
+    Middleware(
+      MatomoMiddleware,
+      matomo_url="YOUR MATOMO TRACKING URL",
+      idsite=12345, # your service tracking id
+  )],
+)
+```
+
 ## Examples
 
 ### Starlette
 
 ```python
 from starlette.applications import Starlette
 from starlette.responses import JSONResponse
@@ -145,20 +174,23 @@
 - Currently only some parts [Matomo Tracking HTTP API](https://developer.matomo.org/api-reference/tracking-api) is supported.
 
 ## Ideas for further work:
 - [x] _filtering tracked of urls_
 - [x] _custom extraction of tracked data_
 
 
-This project keeps a [changelog](./CHANGELOG.md).
+This project keeps a [changelog](https://github.com/spraakbanken/asgi-matomo/CHANGELOG.md).
 
 # Releas Notes
 
 ## Latest Changes
 
+## [0.3.2] - 2023-05-23
+
+* feat: add PerfMsTracker. PR [#10](https://github.com/spraakbanken/asgi-matomo/pull/10) by [@kod-kristoff](https://github.com/kod-kristoff).
 
 ## [0.3.0] - 2023-05-22
 ### Added
 
 - Allow setting route-details
```

