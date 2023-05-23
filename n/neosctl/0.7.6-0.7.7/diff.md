# Comparing `tmp/neosctl-0.7.6.tar.gz` & `tmp/neosctl-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neosctl-0.7.6.tar", max compression
+gzip compressed data, was "neosctl-0.7.7.tar", max compression
```

## Comparing `neosctl-0.7.6.tar` & `neosctl-0.7.7.tar`

### file list

```diff
@@ -1,21 +1,29 @@
--rw-r--r--   0        0        0     2655 2023-04-20 08:51:11.098121 neosctl-0.7.6/README.md
--rw-r--r--   0        0        0       22 2023-04-20 08:51:11.098121 neosctl-0.7.6/neosctl/__init__.py
--rw-r--r--   0        0        0     4478 2023-04-20 08:51:11.098121 neosctl-0.7.6/neosctl/auth.py
--rw-r--r--   0        0        0     4613 2023-04-20 08:51:11.098121 neosctl-0.7.6/neosctl/cli.py
--rw-r--r--   0        0        0      224 2023-04-20 08:51:11.098121 neosctl-0.7.6/neosctl/constant.py
--rw-r--r--   0        0        0      723 2023-04-20 08:51:11.098121 neosctl-0.7.6/neosctl/consume.py
--rw-r--r--   0        0        0     3730 2023-04-20 08:51:11.098121 neosctl-0.7.6/neosctl/iam.py
--rw-r--r--   0        0        0     4989 2023-04-20 08:51:11.099121 neosctl-0.7.6/neosctl/kafka.py
--rw-r--r--   0        0        0     2809 2023-04-20 08:51:11.099121 neosctl-0.7.6/neosctl/link.py
--rw-r--r--   0        0        0    15038 2023-04-20 08:51:11.099121 neosctl-0.7.6/neosctl/metadata.py
--rw-r--r--   0        0        0     8557 2023-04-20 08:51:11.099121 neosctl-0.7.6/neosctl/product.py
--rw-r--r--   0        0        0     4420 2023-04-20 08:51:11.099121 neosctl-0.7.6/neosctl/profile.py
--rw-r--r--   0        0        0     3062 2023-04-20 08:51:11.099121 neosctl-0.7.6/neosctl/registry.py
--rw-r--r--   0        0        0     7596 2023-04-20 08:51:11.099121 neosctl-0.7.6/neosctl/schema.py
--rw-r--r--   0        0        0     5884 2023-04-20 08:51:11.099121 neosctl-0.7.6/neosctl/secret.py
--rw-r--r--   0        0        0    12329 2023-04-20 08:51:11.099121 neosctl-0.7.6/neosctl/source.py
--rw-r--r--   0        0        0    13142 2023-04-20 08:51:11.099121 neosctl-0.7.6/neosctl/spark.py
--rw-r--r--   0        0        0    12105 2023-04-20 08:51:11.099121 neosctl-0.7.6/neosctl/storage.py
--rw-r--r--   0        0        0     8339 2023-04-20 08:51:11.100121 neosctl-0.7.6/neosctl/util.py
--rw-r--r--   0        0        0     2712 2023-04-20 08:51:11.100121 neosctl-0.7.6/pyproject.toml
--rw-r--r--   0        0        0     3552 1970-01-01 00:00:00.000000 neosctl-0.7.6/PKG-INFO
+-rw-r--r--   0        0        0     2655 2023-05-23 14:44:03.004880 neosctl-0.7.7/README.md
+-rw-r--r--   0        0        0       22 2023-05-23 14:44:03.004880 neosctl-0.7.7/neosctl/__init__.py
+-rw-r--r--   0        0        0     4476 2023-05-23 14:44:03.004880 neosctl-0.7.7/neosctl/auth.py
+-rw-r--r--   0        0        0     4677 2023-05-23 14:44:03.004880 neosctl-0.7.7/neosctl/cli.py
+-rw-r--r--   0        0        0      224 2023-05-23 14:44:03.004880 neosctl-0.7.7/neosctl/constant.py
+-rw-r--r--   0        0        0     4420 2023-05-23 14:44:03.004880 neosctl-0.7.7/neosctl/profile.py
+-rw-r--r--   0        0        0     2432 2023-05-23 14:44:03.004880 neosctl-0.7.7/neosctl/schema.py
+-rw-r--r--   0        0        0      138 2023-05-23 14:44:03.005880 neosctl-0.7.7/neosctl/services/__init__.py
+-rw-r--r--   0        0        0      249 2023-05-23 14:44:03.005880 neosctl-0.7.7/neosctl/services/gateway/__init__.py
+-rw-r--r--   0        0        0      723 2023-05-23 14:44:03.005880 neosctl-0.7.7/neosctl/services/gateway/consume.py
+-rw-r--r--   0        0        0     4989 2023-05-23 14:44:03.005880 neosctl-0.7.7/neosctl/services/gateway/kafka.py
+-rw-r--r--   0        0        0     2809 2023-05-23 14:44:03.005880 neosctl-0.7.7/neosctl/services/gateway/link.py
+-rw-r--r--   0        0        0    15074 2023-05-23 14:44:03.005880 neosctl-0.7.7/neosctl/services/gateway/metadata.py
+-rw-r--r--   0        0        0     8593 2023-05-23 14:44:03.005880 neosctl-0.7.7/neosctl/services/gateway/product.py
+-rw-r--r--   0        0        0     3985 2023-05-23 14:44:03.005880 neosctl-0.7.7/neosctl/services/gateway/schema.py
+-rw-r--r--   0        0        0     5884 2023-05-23 14:44:03.005880 neosctl-0.7.7/neosctl/services/gateway/secret.py
+-rw-r--r--   0        0        0    12365 2023-05-23 14:44:03.005880 neosctl-0.7.7/neosctl/services/gateway/source.py
+-rw-r--r--   0        0        0    13015 2023-05-23 14:44:03.005880 neosctl-0.7.7/neosctl/services/gateway/spark.py
+-rw-r--r--   0        0        0       55 2023-05-23 14:44:03.005880 neosctl-0.7.7/neosctl/services/iam/__init__.py
+-rw-r--r--   0        0        0     3762 2023-05-23 14:44:03.006880 neosctl-0.7.7/neosctl/services/iam/iam.py
+-rw-r--r--   0        0        0      664 2023-05-23 14:44:03.006880 neosctl-0.7.7/neosctl/services/iam/schema.py
+-rw-r--r--   0        0        0       65 2023-05-23 14:44:03.006880 neosctl-0.7.7/neosctl/services/registry/__init__.py
+-rw-r--r--   0        0        0     3080 2023-05-23 14:44:03.006880 neosctl-0.7.7/neosctl/services/registry/registry.py
+-rw-r--r--   0        0        0      141 2023-05-23 14:44:03.006880 neosctl-0.7.7/neosctl/services/registry/schema.py
+-rw-r--r--   0        0        0       63 2023-05-23 14:44:03.006880 neosctl-0.7.7/neosctl/services/storage/__init__.py
+-rw-r--r--   0        0        0     8408 2023-05-23 14:44:03.006880 neosctl-0.7.7/neosctl/services/storage/storage.py
+-rw-r--r--   0        0        0     8127 2023-05-23 14:44:03.006880 neosctl-0.7.7/neosctl/util.py
+-rw-r--r--   0        0        0     3013 2023-05-23 14:44:03.006880 neosctl-0.7.7/pyproject.toml
+-rw-r--r--   0        0        0     3584 1970-01-01 00:00:00.000000 neosctl-0.7.7/PKG-INFO
```

### Comparing `neosctl-0.7.6/README.md` & `neosctl-0.7.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Core CLI v0.7.6
+# Core CLI v0.7.7
 
 ## Prerequisites
 
 The following packages are used across python repositories. A global install of them all is _highly_ recommended.
 
 - [Poetry](https://python-poetry.org/docs/#installation)
 - [Invoke](https://www.pyinvoke.org/installing.html)
```

### Comparing `neosctl-0.7.6/neosctl/auth.py` & `neosctl-0.7.7/neosctl/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 
 def _auth_url(iam_api_url: str) -> str:
     return "{}".format(iam_api_url.rstrip("/"))
 
 
 def _check_refresh_token_exists(ctx: click.Context) -> bool:
-    if ctx.obj.profile.refresh_token == "":  # nosec: B105
+    if not ctx.obj.profile.refresh_token:  # nosec: B105
         raise exit_with_output(
             msg=f"You need to login. Run neosctl -p {ctx.obj.profile_name} auth login",
             exit_code=1,
         )
 
     return True
```

### Comparing `neosctl-0.7.6/neosctl/cli.py` & `neosctl-0.7.7/neosctl/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,27 +4,17 @@
 
 import typer
 
 import neosctl
 from neosctl import (
     auth,
     constant,
-    consume,
-    iam,
-    kafka,
-    link,
-    metadata,
-    product,
     profile,
-    registry,
     schema,
-    secret,
-    source,
-    spark,
-    storage,
+    services,
     util,
 )
 from neosctl.util import get_user_profile, read_config_dotfile
 
 
 def _generate_common_schema(
     gateway_api_url: str,
@@ -128,18 +118,23 @@
     user_profile = get_user_profile(ctx.obj.config, ctx.obj.profile_name)
     ctx.obj.profile = user_profile
 
 
 app = typer.Typer(name="neosctl", callback=_callback)
 app.add_typer(profile.app, name="profile", help="Manage profiles.")
 app.add_typer(auth.app, name="auth", callback=_common, help="Manage authentication status.")
-app.add_typer(consume.app, name="consume", callback=_common, help="Consume published data products.")
-app.add_typer(iam.app, name="iam", callback=_common, help="Manage access policies.")
-app.add_typer(storage.app, name="storage", callback=_common, help="Interact with Storage (as a service).")
-app.add_typer(metadata.app, name="metadata", callback=_common, help="Manage and browse metadata.")
-app.add_typer(product.app, name="product", callback=_common, help="Manage data products.")
-app.add_typer(source.app, name="source", help="Manage sources.")
-app.add_typer(registry.app, name="registry", callback=_common, help="Manage cores and search data products.")
-app.add_typer(spark.app, name="spark", callback=_common, help="Manage data product spark jobs.")
-app.add_typer(secret.app, name="secret", callback=_common, help="Manage secrets.")
-app.add_typer(kafka.app, name="kafka", callback=_common, help="Manage data product kafka streaming.")
-app.add_typer(link.app, name="link", callback=_common, help="Manage links.")
+app.add_typer(
+    services.gateway.consume.app,
+    name="consume",
+    callback=_common,
+    help="Consume published data products.",
+)
+app.add_typer(services.iam.app, name="iam", callback=_common, help="Manage access policies.")
+app.add_typer(services.storage.app, name="storage", callback=_common, help="Interact with Storage (as a service).")
+app.add_typer(services.gateway.metadata.app, name="metadata", callback=_common, help="Manage and browse metadata.")
+app.add_typer(services.gateway.product.app, name="product", callback=_common, help="Manage data products.")
+app.add_typer(services.gateway.source.app, name="source", help="Manage sources.")
+app.add_typer(services.registry.app, name="registry", callback=_common, help="Manage cores and search data products.")
+app.add_typer(services.gateway.spark.app, name="spark", callback=_common, help="Manage data product spark jobs.")
+app.add_typer(services.gateway.secret.app, name="secret", callback=_common, help="Manage secrets.")
+app.add_typer(services.gateway.kafka.app, name="kafka", callback=_common, help="Manage data product kafka streaming.")
+app.add_typer(services.gateway.link.app, name="link", callback=_common, help="Manage links.")
```

### Comparing `neosctl-0.7.6/neosctl/consume.py` & `neosctl-0.7.7/neosctl/services/gateway/consume.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.7.6/neosctl/iam.py` & `neosctl-0.7.7/neosctl/services/iam/iam.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import typing
 
 import httpx
 import typer
 
-from neosctl import schema, util
+from neosctl import util
 from neosctl.auth import ensure_login
+from neosctl.services.iam import schema
 from neosctl.util import process_response
 
 app = typer.Typer()
 
 
 def _iam_url(iam_api_url: str, postfix: str = "") -> str:
     return "{}/{}".format(iam_api_url.rstrip("/"), postfix)
```

### Comparing `neosctl-0.7.6/neosctl/kafka.py` & `neosctl-0.7.7/neosctl/services/gateway/kafka.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.7.6/neosctl/link.py` & `neosctl-0.7.7/neosctl/services/gateway/link.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.7.6/neosctl/metadata.py` & `neosctl-0.7.7/neosctl/services/gateway/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import httpx
 import typer
 
-from neosctl import schema, util
+from neosctl import util
 from neosctl.auth import ensure_login
+from neosctl.services.gateway import schema
 from neosctl.util import process_response
 
 app = typer.Typer()
 
 product_app = typer.Typer()
 tag_app = typer.Typer()
 pipeline_app = typer.Typer()
```

### Comparing `neosctl-0.7.6/neosctl/product.py` & `neosctl-0.7.7/neosctl/services/gateway/product.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 if sys.platform != "win32":
     import jq
 else:
     jq = None
 
 import typer
 
-from neosctl import schema, util
+from neosctl import util
 from neosctl.auth import ensure_login
+from neosctl.services.gateway import schema
 from neosctl.util import process_response
 
 app = typer.Typer()
 
 
 def _product_url(ctx: typer.Context) -> str:
     return "{}/product".format(ctx.obj.get_gateway_api_url().rstrip("/"))
```

### Comparing `neosctl-0.7.6/neosctl/profile.py` & `neosctl-0.7.7/neosctl/profile.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.7.6/neosctl/registry.py` & `neosctl-0.7.7/neosctl/services/registry/registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import httpx
 import typer
 
 from neosctl import util
 from neosctl.auth import ensure_login
-from neosctl.schema import RegisterCore, RemoveCore
+from neosctl.services.registry.schema import RegisterCore, RemoveCore
 from neosctl.util import process_response
 
 app = typer.Typer()
 
 
 def _core_url(registry_api_url: str) -> str:
     return "{}/core".format(registry_api_url.rstrip("/"))
```

### Comparing `neosctl-0.7.6/neosctl/secret.py` & `neosctl-0.7.7/neosctl/services/gateway/secret.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.7.6/neosctl/source.py` & `neosctl-0.7.7/neosctl/services/gateway/source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import json
 from typing import Optional
 
 import httpx
 import typer
 
-from neosctl import schema, util
+from neosctl import util
 from neosctl.auth import ensure_login
+from neosctl.services.gateway import schema
 from neosctl.util import process_response
 
 app = typer.Typer()
 
 
 def _source_url(ctx: typer.Context) -> str:
     return "{}/source".format(ctx.obj.gateway_api_url.rstrip("/"))
```

### Comparing `neosctl-0.7.6/neosctl/spark.py` & `neosctl-0.7.7/neosctl/services/gateway/spark.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,14 @@
 app = typer.Typer()
 
 
 def _spark_url(name: str, gateway_api_url: str) -> str:
     return "{}/spark/{}".format(gateway_api_url.rstrip("/"), name)
 
 
-def _secret_url(name: str, gateway_api_url: str) -> str:
-    return "{}/secret/{}".format(gateway_api_url.rstrip("/"), name)
-
-
 @app.command()
 def add_job(
     ctx: typer.Context,
     product_identifier: str = typer.Argument(
         ...,
         help="Data Product identifier",
         callback=util.sanitize,
```

### Comparing `neosctl-0.7.6/neosctl/util.py` & `neosctl-0.7.7/neosctl/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,20 +201,14 @@
                 exit_code=1,
             )
             return []  # never reached as raise exit_with_output, but it makes type checker happy
 
     return data
 
 
-def load_fields_file(fp: pathlib.Path, content_type: str = "schema") -> typing.List:
-    """Load contents of json file containing list of objects."""
-    r = load_json_file(fp, content_type)
-    return list(r)
-
-
 def load_object_file(fp: pathlib.Path, content_type: str) -> typing.Dict:
     """Load contents of json file containing an object."""
     r = load_json_file(fp, content_type)
     return dict(r)
 
 
 def _request(ctx: click.Context, method: str, url: str, **kwargs: ...) -> httpx.Response:
```

### Comparing `neosctl-0.7.6/pyproject.toml` & `neosctl-0.7.7/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [tool.poetry]
 name = "neosctl"
-version = "0.7.6"
+version = "0.7.7"
 description = "Nortal Core CLI"
 authors = []
 license = "closed"
 repository="https://github.com/NEOS-Critical/neos-platform-cli"
 homepage="https://github.com/NEOS-Critical/neos-platform-cli"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 httpx = "^0.23.0"
 typer = "^0.6.1"
 Pygments = "^2.13.0"
-pydantic = "^1.9.2"
-typing_extensions = { version = "^4.4.0", python = "<3.10" }
+typing_extensions = { version = "<4.6.0", python = "<3.10" }
 jq = { version = "^1.4.0", markers = "sys_platform != 'win32'" }
+minio = "^7.1.14"
+pydantic = "^1.10.7"
 
 [tool.poetry.dev-dependencies]
 
 # Tests
 freezegun = "^1.2.1"
 pretend = "^1.0.9"
 pytest = "~7.1.2"
@@ -94,14 +95,23 @@
 "neosctl/*"= [
     "D100", # Ignore module level docstrings, this project is never consumed
     "D104",  # Ignore public __init__ missing docstring.
 ]
 "neosctl/schema.py" = [
     "D101",  # ignore docstrings on pydantic models
 ]
+"neosctl/services/gateway/schema.py" = [
+    "D101",  # ignore docstrings on pydantic models
+]
+"neosctl/services/iam/schema.py" = [
+    "D101",  # ignore docstrings on pydantic models
+]
+"neosctl/services/registry/schema.py" = [
+    "D101",  # ignore docstrings on pydantic models
+]
 "tasks.py" = ["ANN", "INP001", "E501"]
 "tests/*" = [
     "ANN",  # skip annotation in tests
     "D",  # skip docstrings in tests
 ]
 
 [tool.ruff.flake8-quotes]
```

### Comparing `neosctl-0.7.6/PKG-INFO` & `neosctl-0.7.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: neosctl
-Version: 0.7.6
+Version: 0.7.7
 Summary: Nortal Core CLI
 Home-page: https://github.com/NEOS-Critical/neos-platform-cli
 License: closed
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pygments (>=2.13.0,<3.0.0)
 Requires-Dist: httpx (>=0.23.0,<0.24.0)
 Requires-Dist: jq (>=1.4.0,<2.0.0) ; sys_platform != "win32"
-Requires-Dist: pydantic (>=1.9.2,<2.0.0)
+Requires-Dist: minio (>=7.1.14,<8.0.0)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: typer (>=0.6.1,<0.7.0)
-Requires-Dist: typing_extensions (>=4.4.0,<5.0.0) ; python_version < "3.10"
+Requires-Dist: typing_extensions (<4.6.0) ; python_version < "3.10"
 Project-URL: Repository, https://github.com/NEOS-Critical/neos-platform-cli
 Description-Content-Type: text/markdown
 
-# Core CLI v0.7.6
+# Core CLI v0.7.7
 
 ## Prerequisites
 
 The following packages are used across python repositories. A global install of them all is _highly_ recommended.
 
 - [Poetry](https://python-poetry.org/docs/#installation)
 - [Invoke](https://www.pyinvoke.org/installing.html)
```

