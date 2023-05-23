# Comparing `tmp/mela-1.1.0a7.tar.gz` & `tmp/mela-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mela-1.1.0a7.tar", last modified: Thu Nov 17 05:58:19 2022, max compression
+gzip compressed data, was "mela-1.1.1.tar", last modified: Tue May 23 10:39:21 2023, max compression
```

## Comparing `mela-1.1.0a7.tar` & `mela-1.1.1.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 05:58:19.000000 mela-1.1.0a7/
--rw-r--r--   0 runner    (1001) docker     (121)      492 2022-11-17 05:58:19.000000 mela-1.1.0a7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 05:58:19.000000 mela-1.1.0a7/mela/
--rw-r--r--   0 runner    (1001) docker     (121)     1309 2022-11-17 05:58:11.000000 mela-1.1.0a7/mela/abc.py
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-11-17 05:58:11.000000 mela-1.1.0a7/mela/log.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 05:58:19.000000 mela-1.1.0a7/mela/scheme/
--rw-r--r--   0 runner    (1001) docker     (121)     2031 2022-11-17 05:58:11.000000 mela-1.1.0a7/mela/scheme/requirement.py
--rw-r--r--   0 runner    (1001) docker     (121)     3921 2022-11-17 05:58:11.000000 mela-1.1.0a7/mela/scheme/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 05:58:19.000000 mela-1.1.0a7/mela/components/
--rw-r--r--   0 runner    (1001) docker     (121)     5614 2022-11-17 05:58:11.000000 mela-1.1.0a7/mela/components/rpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2798 2022-11-17 05:58:11.000000 mela-1.1.0a7/mela/components/service.py
--rw-r--r--   0 runner    (1001) docker     (121)     2175 2022-11-17 05:58:11.000000 mela-1.1.0a7/mela/components/publisher.py
--rw-r--r--   0 runner    (1001) docker     (121)     3475 2022-11-17 05:58:11.000000 mela-1.1.0a7/mela/components/consumer.py
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-11-17 05:58:11.000000 mela-1.1.0a7/mela/components/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1353 2022-11-17 05:58:11.000000 mela-1.1.0a7/mela/components/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      271 2022-11-17 05:58:11.000000 mela-1.1.0a7/mela/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-11-17 05:58:11.000000 mela-1.1.0a7/mela/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     9856 2022-11-17 05:58:11.000000 mela-1.1.0a7/mela/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 05:58:19.000000 mela-1.1.0a7/mela/settings/
--rw-r--r--   0 runner    (1001) docker     (121)    15433 2022-11-17 05:58:11.000000 mela-1.1.0a7/mela/settings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 05:58:19.000000 mela-1.1.0a7/mela/factories/
--rw-r--r--   0 runner    (1001) docker     (121)     1850 2022-11-17 05:58:11.000000 mela-1.1.0a7/mela/factories/rpc.py
--rw-r--r--   0 runner    (1001) docker     (121)      700 2022-11-17 05:58:11.000000 mela-1.1.0a7/mela/factories/service.py
--rw-r--r--   0 runner    (1001) docker     (121)     1452 2022-11-17 05:58:11.000000 mela-1.1.0a7/mela/factories/publisher.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 05:58:19.000000 mela-1.1.0a7/mela/factories/core/
--rw-r--r--   0 runner    (1001) docker     (121)      568 2022-11-17 05:58:11.000000 mela-1.1.0a7/mela/factories/core/queue.py
--rw-r--r--   0 runner    (1001) docker     (121)      297 2022-11-17 05:58:11.000000 mela-1.1.0a7/mela/factories/core/exchange.py
--rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-11-17 05:58:11.000000 mela-1.1.0a7/mela/factories/core/connection.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 05:58:11.000000 mela-1.1.0a7/mela/factories/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2019 2022-11-17 05:58:11.000000 mela-1.1.0a7/mela/factories/consumer.py
--rw-r--r--   0 runner    (1001) docker     (121)      489 2022-11-17 05:58:11.000000 mela-1.1.0a7/mela/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2705 2022-11-17 05:58:11.000000 mela-1.1.0a7/mela/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-11-17 05:58:11.000000 mela-1.1.0a7/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1036 2022-11-17 05:58:11.000000 mela-1.1.0a7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 05:58:19.000000 mela-1.1.0a7/mela.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-11-17 05:58:19.000000 mela-1.1.0a7/mela.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-11-17 05:58:19.000000 mela-1.1.0a7/mela.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-17 05:58:19.000000 mela-1.1.0a7/mela.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      768 2022-11-17 05:58:19.000000 mela-1.1.0a7/mela.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2266 2022-11-17 05:58:19.000000 mela-1.1.0a7/mela.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2266 2022-11-17 05:58:19.000000 mela-1.1.0a7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:39:21.383256 mela-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-23 10:39:08.000000 mela-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-05-23 10:39:21.383256 mela-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-23 10:39:08.000000 mela-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:39:21.379256 mela-1.1.1/mela/
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-23 10:39:08.000000 mela-1.1.1/mela/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-23 10:39:08.000000 mela-1.1.1/mela/abc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:39:21.383256 mela-1.1.1/mela/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-23 10:39:08.000000 mela-1.1.1/mela/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-23 10:39:08.000000 mela-1.1.1/mela/components/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-05-23 10:39:08.000000 mela-1.1.1/mela/components/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-23 10:39:08.000000 mela-1.1.1/mela/components/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-23 10:39:08.000000 mela-1.1.1/mela/components/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-23 10:39:08.000000 mela-1.1.1/mela/components/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-23 10:39:08.000000 mela-1.1.1/mela/components/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-23 10:39:08.000000 mela-1.1.1/mela/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:39:21.383256 mela-1.1.1/mela/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-23 10:39:08.000000 mela-1.1.1/mela/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-23 10:39:08.000000 mela-1.1.1/mela/factories/consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:39:21.383256 mela-1.1.1/mela/factories/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:39:08.000000 mela-1.1.1/mela/factories/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-23 10:39:08.000000 mela-1.1.1/mela/factories/core/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-23 10:39:08.000000 mela-1.1.1/mela/factories/core/exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-23 10:39:08.000000 mela-1.1.1/mela/factories/core/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-23 10:39:08.000000 mela-1.1.1/mela/factories/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-23 10:39:08.000000 mela-1.1.1/mela/factories/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-23 10:39:08.000000 mela-1.1.1/mela/factories/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-23 10:39:08.000000 mela-1.1.1/mela/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-05-23 10:39:08.000000 mela-1.1.1/mela/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:39:21.383256 mela-1.1.1/mela/scheme/
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-05-23 10:39:08.000000 mela-1.1.1/mela/scheme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-23 10:39:08.000000 mela-1.1.1/mela/scheme/requirement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:39:21.383256 mela-1.1.1/mela/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)    15433 2023-05-23 10:39:08.000000 mela-1.1.1/mela/settings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:39:21.379256 mela-1.1.1/mela.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-05-23 10:39:21.000000 mela-1.1.1/mela.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-23 10:39:21.000000 mela-1.1.1/mela.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 10:39:21.000000 mela-1.1.1/mela.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-23 10:39:21.000000 mela-1.1.1/mela.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-23 10:39:21.000000 mela-1.1.1/mela.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-23 10:39:21.383256 mela-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-23 10:39:08.000000 mela-1.1.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mela-1.1.0a7/mela/abc.py` & `mela-1.1.1/mela/abc.py`

 * *Files identical despite different names*

### Comparing `mela-1.1.0a7/mela/scheme/requirement.py` & `mela-1.1.1/mela/scheme/requirement.py`

 * *Files identical despite different names*

### Comparing `mela-1.1.0a7/mela/scheme/__init__.py` & `mela-1.1.1/mela/scheme/__init__.py`

 * *Files identical despite different names*

### Comparing `mela-1.1.0a7/mela/components/rpc.py` & `mela-1.1.1/mela/components/rpc.py`

 * *Files identical despite different names*

### Comparing `mela-1.1.0a7/mela/components/service.py` & `mela-1.1.1/mela/components/service.py`

 * *Files identical despite different names*

### Comparing `mela-1.1.0a7/mela/components/publisher.py` & `mela-1.1.1/mela/components/publisher.py`

 * *Files identical despite different names*

### Comparing `mela-1.1.0a7/mela/components/consumer.py` & `mela-1.1.1/mela/components/consumer.py`

 * *Files identical despite different names*

### Comparing `mela-1.1.0a7/mela/components/base.py` & `mela-1.1.1/mela/components/base.py`

 * *Files identical despite different names*

### Comparing `mela-1.1.0a7/mela/processor.py` & `mela-1.1.1/mela/processor.py`

 * *Files identical despite different names*

### Comparing `mela-1.1.0a7/mela/settings/__init__.py` & `mela-1.1.1/mela/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `mela-1.1.0a7/mela/factories/rpc.py` & `mela-1.1.1/mela/factories/rpc.py`

 * *Files identical despite different names*

### Comparing `mela-1.1.0a7/mela/factories/service.py` & `mela-1.1.1/mela/factories/service.py`

 * *Files identical despite different names*

### Comparing `mela-1.1.0a7/mela/factories/publisher.py` & `mela-1.1.1/mela/factories/publisher.py`

 * *Files identical despite different names*

### Comparing `mela-1.1.0a7/mela/factories/core/queue.py` & `mela-1.1.1/mela/factories/core/queue.py`

 * *Files identical despite different names*

### Comparing `mela-1.1.0a7/mela/factories/core/connection.py` & `mela-1.1.1/mela/factories/core/connection.py`

 * *Files identical despite different names*

### Comparing `mela-1.1.0a7/mela/factories/consumer.py` & `mela-1.1.1/mela/factories/consumer.py`

 * *Files identical despite different names*

### Comparing `mela-1.1.0a7/mela/__init__.py` & `mela-1.1.1/mela/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 import asyncio
 from typing import Optional
 
+from aio_pika import IncomingMessage
+from aio_pika import Message
+
 from .components.base import Component
 from .components.base import ConsumingComponent
 from .factories.core.connection import close_all_connections
 from .factories.publisher import publisher
 from .factories.rpc import client as rpc_client
 from .scheme import MelaScheme
 from .settings import Settings
 
 
+__all__ = ['IncomingMessage', 'Message', 'Mela']
+
+
 class Mela(MelaScheme):
 
     def __init__(
             self,
             name: str,
             settings_: Optional[Settings] = None,
             loop: Optional[asyncio.AbstractEventLoop] = None,
```

### Comparing `mela-1.1.0a7/setup.py` & `mela-1.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,10 +24,10 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Development Status :: 4 - Beta",
         "Framework :: AsyncIO",
         "Topic :: Software Development :: Libraries :: Application Frameworks",
         ""
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.11',
     install_requires=install_requires
 )
```

### Comparing `mela-1.1.0a7/mela.egg-info/SOURCES.txt` & `mela-1.1.1/mela.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 mela/__init__.py
 mela/abc.py
 mela/exceptions.py
 mela/log.py
```

### Comparing `mela-1.1.0a7/mela.egg-info/PKG-INFO` & `mela-1.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,86 +1,112 @@
 Metadata-Version: 2.1
 Name: mela
-Version: 1.1.0a7
+Version: 1.1.1
 Summary: Let's make microservice development fun again!
 Home-page: https://github.com/alem-research/mela
 Author: Daniyar Supiyev
 Author-email: undead.thunderbird@gmail.com
-License: UNKNOWN
-Description: # Alem Mela
-        
-        ## Overview
-        
-        Asynchronous framework that makes it really simple to build RabbitMQ services.
-        
-        ## Installation
-        
-        `pip install mela`
-        
-        ## Usage
-        
-        Basic usage does look like this:
-        
-        `app.py`:
-        ```
-        from mela import Mela
-        
-        app = Mela(__name__)
-        app.read_config_yaml('application.yml')
-        
-        
-        @app.service("printer")
-        def printer(body, message):
-            # Just print message body and push 
-            # unchanged message to output queue.
-            print(body)
-            return body
-        
-        
-        if __name__ == '__main__':
-            app.run()
-        
-        ```
-        
-        `application.yml`:
-        ```
-        connections:
-          default:
-            host: localhost
-            port: 5672
-            username: user
-            password: bitnami
-        
-        services:
-          printer:
-            consumer:
-              exchange: general-sentiment-x
-              routing_key: general-sentiment-q
-              queue: general-sentiment-q
-            publisher:
-              exchange: general-sentiment-x
-              routing_key: general-sentiment-q
-        ```
-        
-        
-        For more use cases and examples please 
-        check `/examples` directory.
-        
-        ## Authors
-        
-        Developed in Alem Research.
-        
-        Core maintainer: Daniyar Supiyev (undead.thunderbird@gmail.com).
-        
-        Sponsor: Sergazy Narynov.
-        
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: 
-Requires-Python: >=3.6
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Alem Mela
+
+## Overview
+
+Asynchronous framework that makes it really simple to build RabbitMQ services.
+
+## Installation
+
+`pip install mela`
+
+## Usage
+
+Basic usage does look like this:
+
+`app.py`:
+```
+from pydantic import BaseModel
+from datetime import datetime
+
+from mela import Mela
+
+app = Mela(__name__)
+
+
+class Document(BaseModel):
+    text: str
+    url: str
+    date: datetime
+
+
+@app.service('printer')
+def printer(body: Document) -> Document:
+    print(body)
+    return body
+
+
+if __name__ == '__main__':
+    app.run()
+```
+
+`application.yml`:
+```
+connections:
+  default:
+    host: localhost
+    port: 5672
+    username: user
+    password: bitnami
+
+services:
+  printer:
+    consumer:
+      exchange: general-sentiment-x
+      routing_key: general-sentiment-q
+      queue: general-sentiment-q
+    publisher:
+      exchange: general-sentiment-x
+      routing_key: general-sentiment-q
+```
+
+
+For more use cases check `/examples` directory.
+
+## Contribute
+
+Clone this repo, create virtualenv using `make setup` command.
+
+NOTE: If you use PyCharm - don't let it create its own virtualenv.
+
+Run tests using `make test`
+
+Run linter using `make lint`
+
+Run mypy using `make type`
+
+Feel free to create issues.
+
+Feel free to contribute.
+
+Feel free to add yourself to `Authors` block in this document.
+
+You also can join [our Telegram chat](https://t.me/MelaFramework).
+
+Despite major version, there is a lot of work undone.
+You can check TODO section in changelog to find an interesting task 
+for you or check issues section of this repository.
+
+## Contributors
+
+Developed in Alem Research.
+
+Core maintainer: Daniyar Supiyev (undead.thunderbird@gmail.com).
+
+Sponsor: Sergazy Narynov.
```

### Comparing `mela-1.1.0a7/PKG-INFO` & `mela-1.1.1/mela.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,86 +1,112 @@
 Metadata-Version: 2.1
 Name: mela
-Version: 1.1.0a7
+Version: 1.1.1
 Summary: Let's make microservice development fun again!
 Home-page: https://github.com/alem-research/mela
 Author: Daniyar Supiyev
 Author-email: undead.thunderbird@gmail.com
-License: UNKNOWN
-Description: # Alem Mela
-        
-        ## Overview
-        
-        Asynchronous framework that makes it really simple to build RabbitMQ services.
-        
-        ## Installation
-        
-        `pip install mela`
-        
-        ## Usage
-        
-        Basic usage does look like this:
-        
-        `app.py`:
-        ```
-        from mela import Mela
-        
-        app = Mela(__name__)
-        app.read_config_yaml('application.yml')
-        
-        
-        @app.service("printer")
-        def printer(body, message):
-            # Just print message body and push 
-            # unchanged message to output queue.
-            print(body)
-            return body
-        
-        
-        if __name__ == '__main__':
-            app.run()
-        
-        ```
-        
-        `application.yml`:
-        ```
-        connections:
-          default:
-            host: localhost
-            port: 5672
-            username: user
-            password: bitnami
-        
-        services:
-          printer:
-            consumer:
-              exchange: general-sentiment-x
-              routing_key: general-sentiment-q
-              queue: general-sentiment-q
-            publisher:
-              exchange: general-sentiment-x
-              routing_key: general-sentiment-q
-        ```
-        
-        
-        For more use cases and examples please 
-        check `/examples` directory.
-        
-        ## Authors
-        
-        Developed in Alem Research.
-        
-        Core maintainer: Daniyar Supiyev (undead.thunderbird@gmail.com).
-        
-        Sponsor: Sergazy Narynov.
-        
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: 
-Requires-Python: >=3.6
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Alem Mela
+
+## Overview
+
+Asynchronous framework that makes it really simple to build RabbitMQ services.
+
+## Installation
+
+`pip install mela`
+
+## Usage
+
+Basic usage does look like this:
+
+`app.py`:
+```
+from pydantic import BaseModel
+from datetime import datetime
+
+from mela import Mela
+
+app = Mela(__name__)
+
+
+class Document(BaseModel):
+    text: str
+    url: str
+    date: datetime
+
+
+@app.service('printer')
+def printer(body: Document) -> Document:
+    print(body)
+    return body
+
+
+if __name__ == '__main__':
+    app.run()
+```
+
+`application.yml`:
+```
+connections:
+  default:
+    host: localhost
+    port: 5672
+    username: user
+    password: bitnami
+
+services:
+  printer:
+    consumer:
+      exchange: general-sentiment-x
+      routing_key: general-sentiment-q
+      queue: general-sentiment-q
+    publisher:
+      exchange: general-sentiment-x
+      routing_key: general-sentiment-q
+```
+
+
+For more use cases check `/examples` directory.
+
+## Contribute
+
+Clone this repo, create virtualenv using `make setup` command.
+
+NOTE: If you use PyCharm - don't let it create its own virtualenv.
+
+Run tests using `make test`
+
+Run linter using `make lint`
+
+Run mypy using `make type`
+
+Feel free to create issues.
+
+Feel free to contribute.
+
+Feel free to add yourself to `Authors` block in this document.
+
+You also can join [our Telegram chat](https://t.me/MelaFramework).
+
+Despite major version, there is a lot of work undone.
+You can check TODO section in changelog to find an interesting task 
+for you or check issues section of this repository.
+
+## Contributors
+
+Developed in Alem Research.
+
+Core maintainer: Daniyar Supiyev (undead.thunderbird@gmail.com).
+
+Sponsor: Sergazy Narynov.
```

