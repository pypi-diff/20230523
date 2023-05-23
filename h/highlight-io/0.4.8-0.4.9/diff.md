# Comparing `tmp/highlight_io-0.4.8.tar.gz` & `tmp/highlight_io-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "highlight_io-0.4.8.tar", max compression
+gzip compressed data, was "highlight_io-0.4.9.tar", max compression
```

## Comparing `highlight_io-0.4.8.tar` & `highlight_io-0.4.9.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      350 2023-05-16 18:48:46.021901 highlight_io-0.4.8/README.md
--rw-r--r--   0        0        0       64 2023-05-16 18:48:46.021901 highlight_io-0.4.8/highlight_io/__init__.py
--rw-r--r--   0        0        0      155 2023-05-16 18:48:46.021901 highlight_io-0.4.8/highlight_io/integrations/__init__.py
--rw-r--r--   0        0        0      717 2023-05-16 18:48:46.021901 highlight_io-0.4.8/highlight_io/integrations/aws.py
--rw-r--r--   0        0        0      740 2023-05-16 18:48:46.021901 highlight_io-0.4.8/highlight_io/integrations/azure.py
--rw-r--r--   0        0        0     1631 2023-05-16 18:48:46.021901 highlight_io-0.4.8/highlight_io/integrations/django.py
--rw-r--r--   0        0        0      722 2023-05-16 18:48:46.021901 highlight_io-0.4.8/highlight_io/integrations/fastapi.py
--rw-r--r--   0        0        0     1519 2023-05-16 18:48:46.021901 highlight_io-0.4.8/highlight_io/integrations/flask.py
--rw-r--r--   0        0        0      747 2023-05-16 18:48:46.021901 highlight_io-0.4.8/highlight_io/integrations/gcp.py
--rw-r--r--   0        0        0     1072 2023-05-16 18:48:46.021901 highlight_io-0.4.8/highlight_io/integrations/serverless.py
--rw-r--r--   0        0        0     6801 2023-05-16 18:48:46.021901 highlight_io-0.4.8/highlight_io/sdk.py
--rw-r--r--   0        0        0     1698 2023-05-16 18:48:46.021901 highlight_io-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 highlight_io-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0      350 2023-03-06 07:22:47.581214 highlight_io-0.4.9/README.md
+-rw-r--r--   0        0        0       64 2023-03-06 07:22:47.585934 highlight_io-0.4.9/highlight_io/__init__.py
+-rw-r--r--   0        0        0      155 2023-03-06 07:22:47.586006 highlight_io-0.4.9/highlight_io/integrations/__init__.py
+-rw-r--r--   0        0        0      717 2023-04-11 23:45:03.063104 highlight_io-0.4.9/highlight_io/integrations/aws.py
+-rw-r--r--   0        0        0      740 2023-04-11 23:45:03.063208 highlight_io-0.4.9/highlight_io/integrations/azure.py
+-rw-r--r--   0        0        0     1631 2023-03-06 07:22:47.586615 highlight_io-0.4.9/highlight_io/integrations/django.py
+-rw-r--r--   0        0        0      722 2023-03-06 07:22:47.586847 highlight_io-0.4.9/highlight_io/integrations/fastapi.py
+-rw-r--r--   0        0        0     1519 2023-03-06 07:22:47.586917 highlight_io-0.4.9/highlight_io/integrations/flask.py
+-rw-r--r--   0        0        0      747 2023-04-11 23:45:03.063318 highlight_io-0.4.9/highlight_io/integrations/gcp.py
+-rw-r--r--   0        0        0     1072 2023-04-11 23:45:03.063459 highlight_io-0.4.9/highlight_io/integrations/serverless.py
+-rw-r--r--   0        0        0     6801 2023-04-19 17:13:56.388150 highlight_io-0.4.9/highlight_io/sdk.py
+-rw-r--r--   0        0        0     1698 2023-05-23 20:14:18.490479 highlight_io-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     1595 1970-01-01 00:00:00.000000 highlight_io-0.4.9/setup.py
+-rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 highlight_io-0.4.9/PKG-INFO
```

### Comparing `highlight_io-0.4.8/highlight_io/integrations/aws.py` & `highlight_io-0.4.9/highlight_io/integrations/aws.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.4.8/highlight_io/integrations/azure.py` & `highlight_io-0.4.9/highlight_io/integrations/azure.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.4.8/highlight_io/integrations/django.py` & `highlight_io-0.4.9/highlight_io/integrations/django.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.4.8/highlight_io/integrations/fastapi.py` & `highlight_io-0.4.9/highlight_io/integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.4.8/highlight_io/integrations/flask.py` & `highlight_io-0.4.9/highlight_io/integrations/flask.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.4.8/highlight_io/integrations/gcp.py` & `highlight_io-0.4.9/highlight_io/integrations/gcp.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.4.8/highlight_io/integrations/serverless.py` & `highlight_io-0.4.9/highlight_io/integrations/serverless.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.4.8/highlight_io/sdk.py` & `highlight_io-0.4.9/highlight_io/sdk.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.4.8/pyproject.toml` & `highlight_io-0.4.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "highlight-io"
-version = "0.4.8"
+version = "0.4.9"
 description = "Session replay and error monitoring: stop guessing why bugs happen!"
 license = "Apache-2.0"
 authors = [
     "Vadim Korolik <vadim@highlight.io>",
     "Jay Khatri <jay@highlight.io>",
 ]
 readme = "README.md"
@@ -27,21 +27,21 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 blinker = { version = "^1.5", optional = true }
 django = { version = "^4.1.7", optional = true }
 flask = { version = "^2.2.2", optional = true }
 fastapi = { version = "^0.92.0", optional = true }
 uvicorn = {version = "^0.20.0", extras = ["standard"], optional = true }
-opentelemetry-api = "^1.15.0"
-opentelemetry-distro = { extras = ["otlp"], version = "^0.37b0" }
-opentelemetry-exporter-otlp-proto-http = "^1.16.0"
-opentelemetry-instrumentation = "^0.37b0"
-opentelemetry-instrumentation-logging = "^0.37b0"
-opentelemetry-proto = "^1.16.0"
-opentelemetry-sdk = "^1.15.0"
+opentelemetry-api = "^1.18.0"
+opentelemetry-distro = { extras = ["otlp"], version = "^0.39b0" }
+opentelemetry-exporter-otlp-proto-http = "^1.18.0"
+opentelemetry-instrumentation = "^0.39b0"
+opentelemetry-instrumentation-logging = "^0.39b0"
+opentelemetry-proto = "^1.18.0"
+opentelemetry-sdk = "^1.18.0"
 
 [tool.poetry.group.dev.dependencies]
 azure-functions = "^1.13.2"
 black = "^23"
 functions-framework = "^3.3.0"
 pytest = "^7.2.1"
 pytest-mock = "^3.10.0"
```

### Comparing `highlight_io-0.4.8/PKG-INFO` & `highlight_io-0.4.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: highlight-io
-Version: 0.4.8
+Version: 0.4.9
 Summary: Session replay and error monitoring: stop guessing why bugs happen!
 Home-page: https://www.highlight.io
 License: Apache-2.0
 Keywords: web,framework
 Author: Vadim Korolik
 Author-email: vadim@highlight.io
 Requires-Python: >=3.8,<4.0
@@ -22,21 +22,21 @@
 Provides-Extra: django
 Provides-Extra: fastapi
 Provides-Extra: flask
 Requires-Dist: blinker (>=1.5,<2.0) ; extra == "flask"
 Requires-Dist: django (>=4.1.7,<5.0.0) ; extra == "django"
 Requires-Dist: fastapi (>=0.92.0,<0.93.0) ; extra == "fastapi"
 Requires-Dist: flask (>=2.2.2,<3.0.0) ; extra == "flask"
-Requires-Dist: opentelemetry-api (>=1.15.0,<2.0.0)
-Requires-Dist: opentelemetry-distro[otlp] (>=0.37b0,<0.38)
-Requires-Dist: opentelemetry-exporter-otlp-proto-http (>=1.16.0,<2.0.0)
-Requires-Dist: opentelemetry-instrumentation (>=0.37b0,<0.38)
-Requires-Dist: opentelemetry-instrumentation-logging (>=0.37b0,<0.38)
-Requires-Dist: opentelemetry-proto (>=1.16.0,<2.0.0)
-Requires-Dist: opentelemetry-sdk (>=1.15.0,<2.0.0)
+Requires-Dist: opentelemetry-api (>=1.18.0,<2.0.0)
+Requires-Dist: opentelemetry-distro[otlp] (>=0.39b0,<0.40)
+Requires-Dist: opentelemetry-exporter-otlp-proto-http (>=1.18.0,<2.0.0)
+Requires-Dist: opentelemetry-instrumentation (>=0.39b0,<0.40)
+Requires-Dist: opentelemetry-instrumentation-logging (>=0.39b0,<0.40)
+Requires-Dist: opentelemetry-proto (>=1.18.0,<2.0.0)
+Requires-Dist: opentelemetry-sdk (>=1.18.0,<2.0.0)
 Requires-Dist: uvicorn[standard] (>=0.20.0,<0.21.0) ; extra == "fastapi"
 Project-URL: Documentation, https://www.highlight.io/docs
 Project-URL: Repository, https://github.com/highlight/highlight
 Description-Content-Type: text/markdown
 
 # highlight-io Python SDK
```

