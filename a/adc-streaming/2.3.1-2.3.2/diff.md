# Comparing `tmp/adc-streaming-2.3.1.tar.gz` & `tmp/adc-streaming-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/adc-streaming-2.3.1.tar", last modified: Mon Dec 19 17:58:55 2022, max compression
+gzip compressed data, was "dist/adc-streaming-2.3.2.tar", last modified: Tue May 23 18:27:58 2023, max compression
```

## Comparing `adc-streaming-2.3.1.tar` & `adc-streaming-2.3.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 christopher   (501) staff       (20)        0 2022-12-19 17:58:55.000000 adc-streaming-2.3.1/
-drwxr-xr-x   0 christopher   (501) staff       (20)        0 2022-12-19 17:58:55.000000 adc-streaming-2.3.1/.github/
-drwxr-xr-x   0 christopher   (501) staff       (20)        0 2022-12-19 17:58:55.000000 adc-streaming-2.3.1/.github/workflows/
--rw-r--r--   0 christopher   (501) staff       (20)      646 2022-12-19 17:55:28.000000 adc-streaming-2.3.1/.github/workflows/build.yml
--rw-r--r--   0 christopher   (501) staff       (20)     1215 2022-07-11 17:41:06.000000 adc-streaming-2.3.1/.gitignore
--rw-r--r--   0 christopher   (501) staff       (20)     1519 2022-07-11 17:41:06.000000 adc-streaming-2.3.1/LICENSE
--rw-r--r--   0 christopher   (501) staff       (20)     2046 2022-08-22 16:10:51.000000 adc-streaming-2.3.1/Makefile
--rw-r--r--   0 christopher   (501) staff       (20)     1913 2022-12-19 17:58:55.000000 adc-streaming-2.3.1/PKG-INFO
--rw-r--r--   0 christopher   (501) staff       (20)     1334 2022-07-11 17:41:06.000000 adc-streaming-2.3.1/README.md
-drwxr-xr-x   0 christopher   (501) staff       (20)        0 2022-12-19 17:58:55.000000 adc-streaming-2.3.1/adc/
--rw-r--r--   0 christopher   (501) staff       (20)      332 2022-07-11 17:41:06.000000 adc-streaming-2.3.1/adc/__init__.py
--rw-r--r--   0 christopher   (501) staff       (20)     2447 2022-07-11 17:41:06.000000 adc-streaming-2.3.1/adc/auth.py
--rw-r--r--   0 christopher   (501) staff       (20)    13120 2022-10-11 19:25:10.000000 adc-streaming-2.3.1/adc/consumer.py
--rw-r--r--   0 christopher   (501) staff       (20)     1880 2022-07-11 17:41:06.000000 adc-streaming-2.3.1/adc/errors.py
--rw-r--r--   0 christopher   (501) staff       (20)     2541 2022-07-11 17:41:06.000000 adc-streaming-2.3.1/adc/io.py
--rw-r--r--   0 christopher   (501) staff       (20)      933 2022-07-11 17:41:06.000000 adc-streaming-2.3.1/adc/kafka.py
--rw-r--r--   0 christopher   (501) staff       (20)     1038 2022-07-11 17:41:06.000000 adc-streaming-2.3.1/adc/oidc.py
--rw-r--r--   0 christopher   (501) staff       (20)     5629 2022-12-19 17:55:28.000000 adc-streaming-2.3.1/adc/producer.py
-drwxr-xr-x   0 christopher   (501) staff       (20)        0 2022-12-19 17:58:55.000000 adc-streaming-2.3.1/adc_streaming.egg-info/
--rw-r--r--   0 christopher   (501) staff       (20)     1913 2022-12-19 17:58:55.000000 adc-streaming-2.3.1/adc_streaming.egg-info/PKG-INFO
--rw-r--r--   0 christopher   (501) staff       (20)      699 2022-12-19 17:58:55.000000 adc-streaming-2.3.1/adc_streaming.egg-info/SOURCES.txt
--rw-r--r--   0 christopher   (501) staff       (20)        1 2022-12-19 17:58:55.000000 adc-streaming-2.3.1/adc_streaming.egg-info/dependency_links.txt
--rw-r--r--   0 christopher   (501) staff       (20)        1 2022-08-17 19:11:07.000000 adc-streaming-2.3.1/adc_streaming.egg-info/not-zip-safe
--rw-r--r--   0 christopher   (501) staff       (20)      270 2022-12-19 17:58:55.000000 adc-streaming-2.3.1/adc_streaming.egg-info/requires.txt
--rw-r--r--   0 christopher   (501) staff       (20)        4 2022-12-19 17:58:55.000000 adc-streaming-2.3.1/adc_streaming.egg-info/top_level.txt
-drwxr-xr-x   0 christopher   (501) staff       (20)        0 2022-12-19 17:58:55.000000 adc-streaming-2.3.1/doc/
--rw-r--r--   0 christopher   (501) staff       (20)      611 2022-07-11 17:41:06.000000 adc-streaming-2.3.1/doc/Makefile
-drwxr-xr-x   0 christopher   (501) staff       (20)        0 2022-12-19 17:58:55.000000 adc-streaming-2.3.1/doc/_static/
-drwxr-xr-x   0 christopher   (501) staff       (20)        0 2022-12-19 17:58:55.000000 adc-streaming-2.3.1/doc/_static/css/
--rw-r--r--   0 christopher   (501) staff       (20)      490 2022-07-11 17:41:06.000000 adc-streaming-2.3.1/doc/_static/css/my_theme.css
-drwxr-xr-x   0 christopher   (501) staff       (20)        0 2022-12-19 17:58:55.000000 adc-streaming-2.3.1/doc/_templates/
--rw-r--r--   0 christopher   (501) staff       (20)       64 2022-07-11 17:41:06.000000 adc-streaming-2.3.1/doc/_templates/layout.html
-drwxr-xr-x   0 christopher   (501) staff       (20)        0 2022-12-19 17:58:55.000000 adc-streaming-2.3.1/doc/api/
--rw-r--r--   0 christopher   (501) staff       (20)      102 2022-07-11 17:41:06.000000 adc-streaming-2.3.1/doc/api/api.rst
--rw-r--r--   0 christopher   (501) staff       (20)       97 2022-07-11 17:41:06.000000 adc-streaming-2.3.1/doc/api/streaming.rst
--rw-r--r--   0 christopher   (501) staff       (20)     5585 2022-07-11 17:41:06.000000 adc-streaming-2.3.1/doc/conf.py
--rw-r--r--   0 christopher   (501) staff       (20)      318 2022-07-11 17:41:06.000000 adc-streaming-2.3.1/doc/index.rst
-drwxr-xr-x   0 christopher   (501) staff       (20)        0 2022-12-19 17:58:55.000000 adc-streaming-2.3.1/doc/user/
--rw-r--r--   0 christopher   (501) staff       (20)      455 2022-07-11 17:41:06.000000 adc-streaming-2.3.1/doc/user/installation.rst
--rw-r--r--   0 christopher   (501) staff       (20)      484 2022-07-11 17:41:06.000000 adc-streaming-2.3.1/doc/user/quickstart.rst
--rw-r--r--   0 christopher   (501) staff       (20)      137 2022-09-26 14:21:11.000000 adc-streaming-2.3.1/pyproject.toml
-drwxr-xr-x   0 christopher   (501) staff       (20)        0 2022-12-19 17:58:55.000000 adc-streaming-2.3.1/recipe/
--rw-r--r--   0 christopher   (501) staff       (20)      653 2022-09-26 14:19:03.000000 adc-streaming-2.3.1/recipe/meta.yaml
--rw-r--r--   0 christopher   (501) staff       (20)      248 2022-12-19 17:58:55.000000 adc-streaming-2.3.1/setup.cfg
--rw-r--r--   0 christopher   (501) staff       (20)     1433 2022-10-11 19:25:10.000000 adc-streaming-2.3.1/setup.py
-drwxr-xr-x   0 christopher   (501) staff       (20)        0 2022-12-19 17:58:55.000000 adc-streaming-2.3.1/tests/
--rw-r--r--   0 christopher   (501) staff       (20)     1070 2022-07-11 17:41:06.000000 adc-streaming-2.3.1/tests/test_auth.py
--rw-r--r--   0 christopher   (501) staff       (20)     2633 2022-07-11 17:41:06.000000 adc-streaming-2.3.1/tests/test_kafka.py
--rw-r--r--   0 christopher   (501) staff       (20)    14385 2022-09-26 14:21:11.000000 adc-streaming-2.3.1/tests/test_kafka_integration.py
+drwxr-xr-x   0 christopher   (501) staff       (20)        0 2023-05-23 18:27:58.000000 adc-streaming-2.3.2/
+drwxr-xr-x   0 christopher   (501) staff       (20)        0 2023-05-23 18:27:58.000000 adc-streaming-2.3.2/.github/
+drwxr-xr-x   0 christopher   (501) staff       (20)        0 2023-05-23 18:27:58.000000 adc-streaming-2.3.2/.github/workflows/
+-rw-r--r--   0 christopher   (501) staff       (20)      646 2022-12-19 17:55:28.000000 adc-streaming-2.3.2/.github/workflows/build.yml
+-rw-r--r--   0 christopher   (501) staff       (20)     1215 2022-07-11 17:41:06.000000 adc-streaming-2.3.2/.gitignore
+-rw-r--r--   0 christopher   (501) staff       (20)     1519 2022-07-11 17:41:06.000000 adc-streaming-2.3.2/LICENSE
+-rw-r--r--   0 christopher   (501) staff       (20)     2046 2022-08-22 16:10:51.000000 adc-streaming-2.3.2/Makefile
+-rw-r--r--   0 christopher   (501) staff       (20)     1913 2023-05-23 18:27:58.000000 adc-streaming-2.3.2/PKG-INFO
+-rw-r--r--   0 christopher   (501) staff       (20)     1334 2022-07-11 17:41:06.000000 adc-streaming-2.3.2/README.md
+drwxr-xr-x   0 christopher   (501) staff       (20)        0 2023-05-23 18:27:58.000000 adc-streaming-2.3.2/adc/
+-rw-r--r--   0 christopher   (501) staff       (20)      332 2022-07-11 17:41:06.000000 adc-streaming-2.3.2/adc/__init__.py
+-rw-r--r--   0 christopher   (501) staff       (20)     2447 2022-07-11 17:41:06.000000 adc-streaming-2.3.2/adc/auth.py
+-rw-r--r--   0 christopher   (501) staff       (20)    13148 2023-05-23 17:36:24.000000 adc-streaming-2.3.2/adc/consumer.py
+-rw-r--r--   0 christopher   (501) staff       (20)     1880 2022-07-11 17:41:06.000000 adc-streaming-2.3.2/adc/errors.py
+-rw-r--r--   0 christopher   (501) staff       (20)     2541 2022-07-11 17:41:06.000000 adc-streaming-2.3.2/adc/io.py
+-rw-r--r--   0 christopher   (501) staff       (20)      933 2022-07-11 17:41:06.000000 adc-streaming-2.3.2/adc/kafka.py
+-rw-r--r--   0 christopher   (501) staff       (20)     1076 2023-05-23 17:36:24.000000 adc-streaming-2.3.2/adc/oidc.py
+-rw-r--r--   0 christopher   (501) staff       (20)     5657 2023-05-23 17:36:24.000000 adc-streaming-2.3.2/adc/producer.py
+drwxr-xr-x   0 christopher   (501) staff       (20)        0 2023-05-23 18:27:58.000000 adc-streaming-2.3.2/adc_streaming.egg-info/
+-rw-r--r--   0 christopher   (501) staff       (20)     1913 2023-05-23 18:27:58.000000 adc-streaming-2.3.2/adc_streaming.egg-info/PKG-INFO
+-rw-r--r--   0 christopher   (501) staff       (20)      699 2023-05-23 18:27:58.000000 adc-streaming-2.3.2/adc_streaming.egg-info/SOURCES.txt
+-rw-r--r--   0 christopher   (501) staff       (20)        1 2023-05-23 18:27:58.000000 adc-streaming-2.3.2/adc_streaming.egg-info/dependency_links.txt
+-rw-r--r--   0 christopher   (501) staff       (20)        1 2022-08-17 19:11:07.000000 adc-streaming-2.3.2/adc_streaming.egg-info/not-zip-safe
+-rw-r--r--   0 christopher   (501) staff       (20)      293 2023-05-23 18:27:58.000000 adc-streaming-2.3.2/adc_streaming.egg-info/requires.txt
+-rw-r--r--   0 christopher   (501) staff       (20)        4 2023-05-23 18:27:58.000000 adc-streaming-2.3.2/adc_streaming.egg-info/top_level.txt
+drwxr-xr-x   0 christopher   (501) staff       (20)        0 2023-05-23 18:27:58.000000 adc-streaming-2.3.2/doc/
+-rw-r--r--   0 christopher   (501) staff       (20)      611 2022-07-11 17:41:06.000000 adc-streaming-2.3.2/doc/Makefile
+drwxr-xr-x   0 christopher   (501) staff       (20)        0 2023-05-23 18:27:58.000000 adc-streaming-2.3.2/doc/_static/
+drwxr-xr-x   0 christopher   (501) staff       (20)        0 2023-05-23 18:27:58.000000 adc-streaming-2.3.2/doc/_static/css/
+-rw-r--r--   0 christopher   (501) staff       (20)      490 2022-07-11 17:41:06.000000 adc-streaming-2.3.2/doc/_static/css/my_theme.css
+drwxr-xr-x   0 christopher   (501) staff       (20)        0 2023-05-23 18:27:58.000000 adc-streaming-2.3.2/doc/_templates/
+-rw-r--r--   0 christopher   (501) staff       (20)       64 2022-07-11 17:41:06.000000 adc-streaming-2.3.2/doc/_templates/layout.html
+drwxr-xr-x   0 christopher   (501) staff       (20)        0 2023-05-23 18:27:58.000000 adc-streaming-2.3.2/doc/api/
+-rw-r--r--   0 christopher   (501) staff       (20)      102 2022-07-11 17:41:06.000000 adc-streaming-2.3.2/doc/api/api.rst
+-rw-r--r--   0 christopher   (501) staff       (20)       97 2022-07-11 17:41:06.000000 adc-streaming-2.3.2/doc/api/streaming.rst
+-rw-r--r--   0 christopher   (501) staff       (20)     5585 2022-07-11 17:41:06.000000 adc-streaming-2.3.2/doc/conf.py
+-rw-r--r--   0 christopher   (501) staff       (20)      318 2022-07-11 17:41:06.000000 adc-streaming-2.3.2/doc/index.rst
+drwxr-xr-x   0 christopher   (501) staff       (20)        0 2023-05-23 18:27:58.000000 adc-streaming-2.3.2/doc/user/
+-rw-r--r--   0 christopher   (501) staff       (20)      455 2022-07-11 17:41:06.000000 adc-streaming-2.3.2/doc/user/installation.rst
+-rw-r--r--   0 christopher   (501) staff       (20)      484 2022-07-11 17:41:06.000000 adc-streaming-2.3.2/doc/user/quickstart.rst
+-rw-r--r--   0 christopher   (501) staff       (20)      137 2022-09-26 14:21:11.000000 adc-streaming-2.3.2/pyproject.toml
+drwxr-xr-x   0 christopher   (501) staff       (20)        0 2023-05-23 18:27:58.000000 adc-streaming-2.3.2/recipe/
+-rw-r--r--   0 christopher   (501) staff       (20)      653 2022-09-26 14:19:03.000000 adc-streaming-2.3.2/recipe/meta.yaml
+-rw-r--r--   0 christopher   (501) staff       (20)      248 2023-05-23 18:27:58.000000 adc-streaming-2.3.2/setup.cfg
+-rw-r--r--   0 christopher   (501) staff       (20)     1462 2023-05-23 17:36:24.000000 adc-streaming-2.3.2/setup.py
+drwxr-xr-x   0 christopher   (501) staff       (20)        0 2023-05-23 18:27:58.000000 adc-streaming-2.3.2/tests/
+-rw-r--r--   0 christopher   (501) staff       (20)     1070 2022-07-11 17:41:06.000000 adc-streaming-2.3.2/tests/test_auth.py
+-rw-r--r--   0 christopher   (501) staff       (20)     2633 2022-07-11 17:41:06.000000 adc-streaming-2.3.2/tests/test_kafka.py
+-rw-r--r--   0 christopher   (501) staff       (20)    14385 2022-09-26 14:21:11.000000 adc-streaming-2.3.2/tests/test_kafka_integration.py
```

### Comparing `adc-streaming-2.3.1/.github/workflows/build.yml` & `adc-streaming-2.3.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adc-streaming-2.3.1/.gitignore` & `adc-streaming-2.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `adc-streaming-2.3.1/LICENSE` & `adc-streaming-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adc-streaming-2.3.1/Makefile` & `adc-streaming-2.3.2/Makefile`

 * *Files identical despite different names*

### Comparing `adc-streaming-2.3.1/PKG-INFO` & `adc-streaming-2.3.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adc-streaming
-Version: 2.3.1
+Version: 2.3.2
 Summary: Astronomy Data Commons streaming client libraries
 Home-page: https://github.com/astronomy-commons/adc-streaming
 Author: Astronomy Data Commons Team
 Author-email: swnelson@uw.edu
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `adc-streaming-2.3.1/README.md` & `adc-streaming-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `adc-streaming-2.3.1/adc/auth.py` & `adc-streaming-2.3.2/adc/auth.py`

 * *Files identical despite different names*

### Comparing `adc-streaming-2.3.1/adc/consumer.py` & `adc-streaming-2.3.2/adc/consumer.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     _consumer: confluent_kafka.Consumer
     logger: logging.Logger
 
     def __init__(self, conf: 'ConsumerConfig') -> None:
         self.logger = logging.getLogger("adc-streaming.consumer")
         self.conf = conf
         self._consumer = confluent_kafka.Consumer(conf._to_confluent_kafka())
-        # Workaround for https://github.com/edenhill/librdkafka/issues/3871.
+        # Workaround for https://github.com/confluentinc/librdkafka/issues/3753#issuecomment-1058272987.
         # FIXME: Remove once fixed upstream, or on removal of oauth_cb.
         self._consumer.poll(0)
         self._stop_event = threading.Event()
 
     def subscribe(self,
                   topics: Union[str, Iterable],
                   timeout: timedelta = timedelta(seconds=10)):
```

### Comparing `adc-streaming-2.3.1/adc/errors.py` & `adc-streaming-2.3.2/adc/errors.py`

 * *Files identical despite different names*

### Comparing `adc-streaming-2.3.1/adc/io.py` & `adc-streaming-2.3.2/adc/io.py`

 * *Files identical despite different names*

### Comparing `adc-streaming-2.3.1/adc/kafka.py` & `adc-streaming-2.3.2/adc/kafka.py`

 * *Files identical despite different names*

### Comparing `adc-streaming-2.3.1/adc/oidc.py` & `adc-streaming-2.3.2/adc/oidc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 def set_oauth_cb(config):
     """Implement client support for KIP-768 OpenID Connect.
 
     Apache Kafka 3.1.0 supports authentication using OpenID Client Credentials.
-    Native support for Python is coming in the next release of librdkafka
-    (version 1.9.0). Meanwhile, this is a pure Python implementation of the
-    refresh token callback.
+    Native support for Python is still incomplete due to this issue:
+    https://github.com/confluentinc/librdkafka/issues/3751
+
+    Meanwhile, this is a pure Python implementation of the refresh token
+    callback.
     """
     if config.pop('sasl.oauthbearer.method', None) != 'oidc':
         return
 
     client_id = config.pop('sasl.oauthbearer.client.id')
     client_secret = config.pop('sasl.oauthbearer.client.secret')
     scope = config.pop('sasl.oauthbearer.scope', None)
```

### Comparing `adc-streaming-2.3.1/adc/producer.py` & `adc-streaming-2.3.2/adc/producer.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     logger: logging.Logger
 
     def __init__(self, conf: 'ProducerConfig') -> None:
         self.logger = logging.getLogger("adc-streaming.producer")
         self.conf = conf
         self.logger.debug(f"connecting to producer with config {conf._to_confluent_kafka()}")
         self._producer = confluent_kafka.Producer(conf._to_confluent_kafka())
-        # Workaround for https://github.com/edenhill/librdkafka/issues/3871.
+        # Workaround for https://github.com/confluentinc/librdkafka/issues/3753#issuecomment-1058272987.
         # FIXME: Remove once fixed upstream, or on removal of oauth_cb.
         self._producer.poll(0)
 
     def write(self,
               msg: Union[bytes, 'Serializable'],
               headers: Optional[Union[dict, list]] = None,
               delivery_callback: Optional[DeliveryCallback] = log_delivery_errors) -> None:
```

### Comparing `adc-streaming-2.3.1/adc_streaming.egg-info/PKG-INFO` & `adc-streaming-2.3.2/adc_streaming.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adc-streaming
-Version: 2.3.1
+Version: 2.3.2
 Summary: Astronomy Data Commons streaming client libraries
 Home-page: https://github.com/astronomy-commons/adc-streaming
 Author: Astronomy Data Commons Team
 Author-email: swnelson@uw.edu
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `adc-streaming-2.3.1/adc_streaming.egg-info/SOURCES.txt` & `adc-streaming-2.3.2/adc_streaming.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adc-streaming-2.3.1/doc/Makefile` & `adc-streaming-2.3.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `adc-streaming-2.3.1/doc/conf.py` & `adc-streaming-2.3.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `adc-streaming-2.3.1/recipe/meta.yaml` & `adc-streaming-2.3.2/recipe/meta.yaml`

 * *Files identical despite different names*

### Comparing `adc-streaming-2.3.1/setup.py` & `adc-streaming-2.3.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 
 # requirements
 install_requires = [
     "authlib",  # FIXME: drop after next release of confluent-kafka with OIDC support
-    "confluent-kafka",
+    "confluent-kafka >= 1.6.1, != 2.1.0, != 2.1.1",
     "dataclasses ; python_version < '3.7'",
     "importlib-metadata ; python_version < '3.8'",
     "requests",  # FIXME: drop after next release of confluent-kafka with OIDC support
     "tqdm",
     "certifi>=2020.04.05.1",
     "typing-extensions ; python_version < '3.8'",
 ]
```

### Comparing `adc-streaming-2.3.1/tests/test_auth.py` & `adc-streaming-2.3.2/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `adc-streaming-2.3.1/tests/test_kafka.py` & `adc-streaming-2.3.2/tests/test_kafka.py`

 * *Files identical despite different names*

### Comparing `adc-streaming-2.3.1/tests/test_kafka_integration.py` & `adc-streaming-2.3.2/tests/test_kafka_integration.py`

 * *Files identical despite different names*

