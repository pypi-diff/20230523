# Comparing `tmp/amqp-rpc-server-1.2.3.tar.gz` & `tmp/amqp-rpc-server-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amqp-rpc-server-1.2.3.tar", last modified: Fri May 27 15:08:06 2022, max compression
+gzip compressed data, was "amqp-rpc-server-1.2.4.tar", last modified: Tue May 23 21:18:29 2023, max compression
```

## Comparing `amqp-rpc-server-1.2.3.tar` & `amqp-rpc-server-1.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 15:08:06.279820 amqp-rpc-server-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1524 2022-05-27 15:07:51.000000 amqp-rpc-server-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1569 2022-05-27 15:08:06.279820 amqp-rpc-server-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1035 2022-05-27 15:07:51.000000 amqp-rpc-server-1.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-05-27 15:07:51.000000 amqp-rpc-server-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      649 2022-05-27 15:08:06.279820 amqp-rpc-server-1.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 15:08:06.275820 amqp-rpc-server-1.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 15:08:06.279820 amqp-rpc-server-1.2.3/src/amqp_rpc_server/
--rw-r--r--   0 runner    (1001) docker     (121)     8927 2022-05-27 15:07:51.000000 amqp-rpc-server-1.2.3/src/amqp_rpc_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20878 2022-05-27 15:07:51.000000 amqp-rpc-server-1.2.3/src/amqp_rpc_server/basic_consumer.py
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-05-27 15:07:51.000000 amqp-rpc-server-1.2.3/src/amqp_rpc_server/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 15:08:06.279820 amqp-rpc-server-1.2.3/src/amqp_rpc_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1569 2022-05-27 15:08:05.000000 amqp-rpc-server-1.2.3/src/amqp_rpc_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      360 2022-05-27 15:08:06.000000 amqp-rpc-server-1.2.3/src/amqp_rpc_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-27 15:08:05.000000 amqp-rpc-server-1.2.3/src/amqp_rpc_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-05-27 15:08:06.000000 amqp-rpc-server-1.2.3/src/amqp_rpc_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-05-27 15:08:06.000000 amqp-rpc-server-1.2.3/src/amqp_rpc_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:18:29.186752 amqp-rpc-server-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-23 21:18:18.000000 amqp-rpc-server-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-23 21:18:29.186752 amqp-rpc-server-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-23 21:18:18.000000 amqp-rpc-server-1.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-23 21:18:18.000000 amqp-rpc-server-1.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-23 21:18:29.186752 amqp-rpc-server-1.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:18:29.182752 amqp-rpc-server-1.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:18:29.182752 amqp-rpc-server-1.2.4/src/amqp_rpc_server/
+-rw-r--r--   0 runner    (1001) docker     (123)     8927 2023-05-23 21:18:18.000000 amqp-rpc-server-1.2.4/src/amqp_rpc_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20786 2023-05-23 21:18:18.000000 amqp-rpc-server-1.2.4/src/amqp_rpc_server/basic_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-23 21:18:18.000000 amqp-rpc-server-1.2.4/src/amqp_rpc_server/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:18:29.186752 amqp-rpc-server-1.2.4/src/amqp_rpc_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-23 21:18:29.000000 amqp-rpc-server-1.2.4/src/amqp_rpc_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-23 21:18:29.000000 amqp-rpc-server-1.2.4/src/amqp_rpc_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 21:18:29.000000 amqp-rpc-server-1.2.4/src/amqp_rpc_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 21:18:29.000000 amqp-rpc-server-1.2.4/src/amqp_rpc_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-23 21:18:29.000000 amqp-rpc-server-1.2.4/src/amqp_rpc_server.egg-info/top_level.txt
```

### Comparing `amqp-rpc-server-1.2.3/LICENSE` & `amqp-rpc-server-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `amqp-rpc-server-1.2.3/PKG-INFO` & `amqp-rpc-server-1.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amqp-rpc-server
-Version: 1.2.3
+Version: 1.2.4
 Summary: A RPC server based on AMQPv0-9-1-enabled message broker
 Home-page: https://github.com/j-suchard/amqp-rpc-client
 Author: Jan Eike Suchard
 Author-email: jan-eike.suchard@magenta.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `amqp-rpc-server-1.2.3/README.md` & `amqp-rpc-server-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `amqp-rpc-server-1.2.3/setup.cfg` & `amqp-rpc-server-1.2.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = amqp-rpc-server
-version = 1.2.3
+version = 1.2.4
 author = Jan Eike Suchard
 author_email = jan-eike.suchard@magenta.de
 description = A RPC server based on AMQPv0-9-1-enabled message broker
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/j-suchard/amqp-rpc-client
 classifiers =
```

### Comparing `amqp-rpc-server-1.2.3/src/amqp_rpc_server/__init__.py` & `amqp-rpc-server-1.2.4/src/amqp_rpc_server/__init__.py`

 * *Files identical despite different names*

### Comparing `amqp-rpc-server-1.2.3/src/amqp_rpc_server/basic_consumer.py` & `amqp-rpc-server-1.2.4/src/amqp_rpc_server/basic_consumer.py`

 * *Files 1% similar despite different names*

```diff
@@ -424,24 +424,23 @@
                 )
             )
             return
 
         # Now run the executor and get its results and catch all errors happening which are not
         # explicitly caught during the execution
         try:
-            results = self._executor(message_body)
-            # Since the message has been processed it now will be acknowledged
+            # Since the message is valid it now will be acknowledged
             channel.basic_ack(delivery_properties.delivery_tag)
+            results = self._executor(message_body)
         except Exception as error:  # pylint: disable=broad-except
             # Since an error occurred we now put the information from the error into the response
             exception_data = {
                 "error": str(error)
             }
             results = json.dumps(exception_data, ensure_ascii=False).encode('utf-8')
-            channel.basic_reject(delivery_properties.delivery_tag, requeue=False)
         # Send the response to the message broker
         channel.basic_publish(
             exchange='',
             routing_key=message_properties.reply_to,
             body=results,
             properties=pika.BasicProperties(
                 correlation_id=message_properties.correlation_id,
```

### Comparing `amqp-rpc-server-1.2.3/src/amqp_rpc_server.egg-info/PKG-INFO` & `amqp-rpc-server-1.2.4/src/amqp_rpc_server.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amqp-rpc-server
-Version: 1.2.3
+Version: 1.2.4
 Summary: A RPC server based on AMQPv0-9-1-enabled message broker
 Home-page: https://github.com/j-suchard/amqp-rpc-client
 Author: Jan Eike Suchard
 Author-email: jan-eike.suchard@magenta.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Software Development :: Libraries
```

