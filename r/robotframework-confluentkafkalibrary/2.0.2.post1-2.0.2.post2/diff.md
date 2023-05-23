# Comparing `tmp/robotframework-confluentkafkalibrary-2.0.2.post1.tar.gz` & `tmp/robotframework-confluentkafkalibrary-2.0.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-confluentkafkalibrary-2.0.2.post1.tar", last modified: Mon Apr 24 19:04:41 2023, max compression
+gzip compressed data, was "robotframework-confluentkafkalibrary-2.0.2.post2.tar", last modified: Tue May 23 21:30:58 2023, max compression
```

## Comparing `robotframework-confluentkafkalibrary-2.0.2.post1.tar` & `robotframework-confluentkafkalibrary-2.0.2.post2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:04:41.340535 robotframework-confluentkafkalibrary-2.0.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-04-24 19:04:30.000000 robotframework-confluentkafkalibrary-2.0.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-24 19:04:41.336535 robotframework-confluentkafkalibrary-2.0.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-04-24 19:04:30.000000 robotframework-confluentkafkalibrary-2.0.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 19:04:41.340535 robotframework-confluentkafkalibrary-2.0.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-24 19:04:30.000000 robotframework-confluentkafkalibrary-2.0.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:04:41.336535 robotframework-confluentkafkalibrary-2.0.2.post1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:04:41.336535 robotframework-confluentkafkalibrary-2.0.2.post1/src/ConfluentKafkaLibrary/
--rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-04-24 19:04:30.000000 robotframework-confluentkafkalibrary-2.0.2.post1/src/ConfluentKafkaLibrary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-04-24 19:04:30.000000 robotframework-confluentkafkalibrary-2.0.2.post1/src/ConfluentKafkaLibrary/admin_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15924 2023-04-24 19:04:30.000000 robotframework-confluentkafkalibrary-2.0.2.post1/src/ConfluentKafkaLibrary/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-24 19:04:30.000000 robotframework-confluentkafkalibrary-2.0.2.post1/src/ConfluentKafkaLibrary/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-24 19:04:30.000000 robotframework-confluentkafkalibrary-2.0.2.post1/src/ConfluentKafkaLibrary/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-24 19:04:30.000000 robotframework-confluentkafkalibrary-2.0.2.post1/src/ConfluentKafkaLibrary/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:04:41.336535 robotframework-confluentkafkalibrary-2.0.2.post1/src/robotframework_confluentkafkalibrary.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-24 19:04:41.000000 robotframework-confluentkafkalibrary-2.0.2.post1/src/robotframework_confluentkafkalibrary.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-24 19:04:41.000000 robotframework-confluentkafkalibrary-2.0.2.post1/src/robotframework_confluentkafkalibrary.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 19:04:41.000000 robotframework-confluentkafkalibrary-2.0.2.post1/src/robotframework_confluentkafkalibrary.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-24 19:04:41.000000 robotframework-confluentkafkalibrary-2.0.2.post1/src/robotframework_confluentkafkalibrary.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-24 19:04:41.000000 robotframework-confluentkafkalibrary-2.0.2.post1/src/robotframework_confluentkafkalibrary.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:30:58.821857 robotframework-confluentkafkalibrary-2.0.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-05-23 21:30:50.000000 robotframework-confluentkafkalibrary-2.0.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-23 21:30:58.821857 robotframework-confluentkafkalibrary-2.0.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-05-23 21:30:50.000000 robotframework-confluentkafkalibrary-2.0.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 21:30:58.821857 robotframework-confluentkafkalibrary-2.0.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-23 21:30:50.000000 robotframework-confluentkafkalibrary-2.0.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:30:58.817857 robotframework-confluentkafkalibrary-2.0.2.post2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:30:58.821857 robotframework-confluentkafkalibrary-2.0.2.post2/src/ConfluentKafkaLibrary/
+-rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-05-23 21:30:50.000000 robotframework-confluentkafkalibrary-2.0.2.post2/src/ConfluentKafkaLibrary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-05-23 21:30:50.000000 robotframework-confluentkafkalibrary-2.0.2.post2/src/ConfluentKafkaLibrary/admin_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15924 2023-05-23 21:30:50.000000 robotframework-confluentkafkalibrary-2.0.2.post2/src/ConfluentKafkaLibrary/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-05-23 21:30:50.000000 robotframework-confluentkafkalibrary-2.0.2.post2/src/ConfluentKafkaLibrary/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-23 21:30:50.000000 robotframework-confluentkafkalibrary-2.0.2.post2/src/ConfluentKafkaLibrary/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-23 21:30:50.000000 robotframework-confluentkafkalibrary-2.0.2.post2/src/ConfluentKafkaLibrary/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:30:58.821857 robotframework-confluentkafkalibrary-2.0.2.post2/src/robotframework_confluentkafkalibrary.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-23 21:30:58.000000 robotframework-confluentkafkalibrary-2.0.2.post2/src/robotframework_confluentkafkalibrary.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-23 21:30:58.000000 robotframework-confluentkafkalibrary-2.0.2.post2/src/robotframework_confluentkafkalibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 21:30:58.000000 robotframework-confluentkafkalibrary-2.0.2.post2/src/robotframework_confluentkafkalibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-23 21:30:58.000000 robotframework-confluentkafkalibrary-2.0.2.post2/src/robotframework_confluentkafkalibrary.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-23 21:30:58.000000 robotframework-confluentkafkalibrary-2.0.2.post2/src/robotframework_confluentkafkalibrary.egg-info/top_level.txt
```

### Comparing `robotframework-confluentkafkalibrary-2.0.2.post1/LICENSE` & `robotframework-confluentkafkalibrary-2.0.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-confluentkafkalibrary-2.0.2.post1/PKG-INFO` & `robotframework-confluentkafkalibrary-2.0.2.post2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-confluentkafkalibrary
-Version: 2.0.2.post1
+Version: 2.0.2.post2
 Summary: Confluent Kafka library for Robot Framework
 Home-page: https://github.com/robooo/robotframework-ConfluentKafkaLibrary
 Author: Robert Karasek
 Author-email: <robo.karasek@gmail.com>
 License: Apache License 2.0
 Keywords: robotframework confluent kafka
 Platform: any
```

### Comparing `robotframework-confluentkafkalibrary-2.0.2.post1/README.md` & `robotframework-confluentkafkalibrary-2.0.2.post2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,48 @@
 # Robot Framework - ConfluentKafkaLibrary
 
-ConfluentKafkaLibrary library is wrapper for [confluent-kafka-python](https://github.com/confluentinc/confluent-kafka-python).
+ConfluentKafkaLibrary library is a wrapper for the [confluent-kafka-python](https://github.com/confluentinc/confluent-kafka-python).
 
-ConfluentKafkaLibrary works with latest confluent-kafka-python, tags are 1:1 (ConfluentKafkaLibrary 1.3.0 == confluent-kafka-python 1.3.0 ). Bugfixes and updates are set after the '-' e.g. `1.3.0-1`.
+ConfluentKafkaLibrary is compatible with the latest version of confluent-kafka-python, where the library versions have a 1:1 correspondence (e.g., ConfluentKafkaLibrary 1.3.0 corresponds to confluent-kafka-python 1.3.0). Bug fixes and updates are denoted by a trailing hyphen, such as `1.3.0-1`.
 
 ## Documentation
 
-Keyword documentation is available [here](https://robooo.github.io/robotframework-ConfluentKafkaLibrary/)
+The keyword documentation for ConfluentKafkaLibrary can be found [here](https://robooo.github.io/robotframework-ConfluentKafkaLibrary/)
 
-How to generate documentation:
+To generate the documentation, use the following command:
 
 ```
 python -m robot.libdoc -f html src/ConfluentKafkaLibrary docs/index.html
 ```
 
 ## Installation
 
+To install the library, run the following command:
+
 ```
 pip install robotframework-confluentkafkalibrary
 ```
 
 ## Usage
 
-In most cases [confluent-kafka-python documentation](https://docs.confluent.io/platform/current/clients/confluent-kafka-python/html/index.html) is your friend. Every keyword should match the same API as python functions, if you are not sure which are pre-configured please check our [robotframework-ConfluentKafkaLibrary documentation](https://robooo.github.io/robotframework-ConfluentKafkaLibrary/). Up to date documentation of configuration properties and its values is maintained [here](https://github.com/edenhill/librdkafka/blob/master/CONFIGURATION.md) by kafka team.
+In most cases, you can refer to the [confluent-kafka-python documentation](https://docs.confluent.io/platform/current/clients/confluent-kafka-python/html/index.html) for guidance. Every keyword in ConfluentKafkaLibrary is designed to match the corresponding Python functions. If you are unsure about the pre-configured keywords, please visit the  [robotframework-ConfluentKafkaLibrary documentation](https://robooo.github.io/robotframework-ConfluentKafkaLibrary/). The Kafka team maintains the up-to-date documentation for configuration properties and their values [here](https://github.com/edenhill/librdkafka/blob/master/CONFIGURATION.md).
 
-* Find basic usage examples at [./examples/test.robot](./examples/test.robot)
-* More complex examples (handle byte data from topic, use more consumers, run avro consumer threaded) are at [documentation](https://robooo.github.io/robotframework-ConfluentKafkaLibrary/#Examples) too.
+* You can find basic usage examples in the [./examples/test.robot](./examples/test.robot)
+* For more complex examples, such as handling byte data from a topic, using multiple consumers, or running threaded avro consumers, please refer to the [documentation](https://robooo.github.io/robotframework-ConfluentKafkaLibrary/#Examples).
 
 ## Testing
 
-* This library is tested by black-box tests written in RobotFramework and tests could be found at
-  * [examples/ directory](./examples).
-* Kafka platform used for testing is dockerized enterprise kafka with schema registry support and rest proxy, deployed & tested on each PR and merge to master.
-  * [docker-compose.yml](./examples/docker-compose.yml)
-* Output of latest run can be found at https://robooo.github.io/robotframework-ConfluentKafkaLibrary/log.html
-* Tests are divided to:
-  * test.robot - Basic tests to verify functionality of Consumer / Producer.
+* The library is tested using black-box tests written in Robot Framework.
+  * You can find the test files in the [examples/ directory](./examples) directory.
+* For testing, a dockerized enterprise Kafka platform with schema registry support and REST proxy is used. The platform is deployed and tested for each pull request and merge to the master branch.
+  * See [docker-compose.yml](./examples/docker-compose.yml) file with the necessary configuration.
+* Tests are divided into the following files:
+  * test.robot - Basic tests to verify functionality of the Consumer and Producer.
   * test_adminclient.robot - Verifications of admin client functionality.
   * test_avro.robot - Verifications of avro and serializers functionality.
-* Not executable example of oauth usage can be found [here](https://github.com/robooo/robotframework-ConfluentKafkaLibrary/blob/1.9.0/examples/test_oauth.robot#L14)
+* Not executable example of oauth usage can be found [here](https://github.com/robooo/robotframework-ConfluentKafkaLibrary/blob/master/examples/test_oauth.robot#L14)
   * Update of deployment https://github.com/robooo/robotframework-ConfluentKafkaLibrary/issues/21 is required.
-* Core of the testing logic is to produce data to kafka, connect one consumer in thread and work with the results in specific test cases.
+* The core testing logic involves producing data to Kafka, connecting one consumer in a thread, and working with the results in specific test cases.
+
+## Known Limitations:
+* Unable to install robotframework-confluentkafkalibrary on Amazon EC2 graviton instance type
+  * see the [steps to resolve](https://github.com/robooo/robotframework-ConfluentKafkaLibrary/issues/33#issuecomment-1464644752)
```

### Comparing `robotframework-confluentkafkalibrary-2.0.2.post1/setup.py` & `robotframework-confluentkafkalibrary-2.0.2.post2/setup.py`

 * *Files identical despite different names*

### Comparing `robotframework-confluentkafkalibrary-2.0.2.post1/src/ConfluentKafkaLibrary/__init__.py` & `robotframework-confluentkafkalibrary-2.0.2.post2/src/ConfluentKafkaLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-confluentkafkalibrary-2.0.2.post1/src/ConfluentKafkaLibrary/admin_client.py` & `robotframework-confluentkafkalibrary-2.0.2.post2/src/ConfluentKafkaLibrary/admin_client.py`

 * *Files identical despite different names*

### Comparing `robotframework-confluentkafkalibrary-2.0.2.post1/src/ConfluentKafkaLibrary/consumer.py` & `robotframework-confluentkafkalibrary-2.0.2.post2/src/ConfluentKafkaLibrary/consumer.py`

 * *Files identical despite different names*

### Comparing `robotframework-confluentkafkalibrary-2.0.2.post1/src/ConfluentKafkaLibrary/producer.py` & `robotframework-confluentkafkalibrary-2.0.2.post2/src/ConfluentKafkaLibrary/producer.py`

 * *Files 5% similar despite different names*

```diff
@@ -85,28 +85,31 @@
 
     def produce(
         self,
         group_id,
         topic,
         value=None,
         key=None,
+        headers=None,
         **kwargs
     ):
         """Produce message to topic asynchronously to Kafka by encoding with specified or default avro schema.\n
         https://docs.confluent.io/current/clients/confluent-kafka-python/#confluent_kafka.Producer.produce
 
         - ``topic`` (str) : name of the topic where to produce message.
         - ``value`` (str|bytes): Message payload.
         - ``key`` (str|bytes): Message key. Default: `None`.
+        - ``headers`` (dict[str, bytes]): Message headers. Default: `None`.
         - ``partition`` (int): Partition to produce to, else uses the configured built-in partitioner.
         """
         self.producers[group_id].produce(
             topic=topic,
             value=value,
             key=key,
+            headers=headers,
             **kwargs
         )
 
     def flush(self, group_id, timeout=0.1):
         """Wait for all messages in the Producer queue to be delivered. Returns the number of messages still in queue.
         This is a convenience method that calls poll() until len() is zero or the optional timeout elapses.
         - `timeout` (real) : Optional timeout. Default: `0.1`.
```

### Comparing `robotframework-confluentkafkalibrary-2.0.2.post1/src/ConfluentKafkaLibrary/serialization.py` & `robotframework-confluentkafkalibrary-2.0.2.post2/src/ConfluentKafkaLibrary/serialization.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,20 @@
     def get_integer_serializer(self):
         return IntegerSerializer()
 
     def get_json_serializer(self, schema_str, schema_registry_client, to_dict=None, conf=None):
         return JSONSerializer(schema_str, schema_registry_client, to_dict, conf)
 
     def get_protobuf_serializer(self, msg_type, schema_registry_client, conf=None):
+        base_conf = {'use.deprecated.format': False}
+        if conf is None:
+            conf = base_conf.copy()
+        else:
+            conf.update(base_conf)
+
         return ProtobufSerializer(msg_type, schema_registry_client, conf)
 
     def get_string_serializer(self, codec='utf_8'):
         return StringSerializer(codec)
 
 
 class Deserializer():
@@ -36,11 +42,11 @@
     def get_integer_deserializer(self):
         return IntegerDeserializer()
 
     def get_json_deserializer(self, schema_str, from_dict=None):
         return JSONDeserializer(schema_str, from_dict)
 
     def get_protobuf_deserializer(self, message_type):
-        return ProtobufDeserializer(message_type)
+        return ProtobufDeserializer(message_type, {'use.deprecated.format': False})
 
     def get_string_deserializer(self, codec='utf_8'):
         return StringDeserializer(codec)
```

### Comparing `robotframework-confluentkafkalibrary-2.0.2.post1/src/robotframework_confluentkafkalibrary.egg-info/PKG-INFO` & `robotframework-confluentkafkalibrary-2.0.2.post2/src/robotframework_confluentkafkalibrary.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-confluentkafkalibrary
-Version: 2.0.2.post1
+Version: 2.0.2.post2
 Summary: Confluent Kafka library for Robot Framework
 Home-page: https://github.com/robooo/robotframework-ConfluentKafkaLibrary
 Author: Robert Karasek
 Author-email: <robo.karasek@gmail.com>
 License: Apache License 2.0
 Keywords: robotframework confluent kafka
 Platform: any
```

### Comparing `robotframework-confluentkafkalibrary-2.0.2.post1/src/robotframework_confluentkafkalibrary.egg-info/SOURCES.txt` & `robotframework-confluentkafkalibrary-2.0.2.post2/src/robotframework_confluentkafkalibrary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

