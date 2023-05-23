# Comparing `tmp/apf_base-2.3.0.tar.gz` & `tmp/apf_base-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/APF/APF/dist/.tmp-zti0cb8a/apf_base-2.3.0.tar", last modified: Mon May 22 14:46:07 2023, max compression
+gzip compressed data, was "/home/runner/work/APF/APF/dist/.tmp-1sy2liwr/apf_base-2.4.0.tar", last modified: Tue May 23 16:40:48 2023, max compression
```

## Comparing `apf_base-2.3.0.tar` & `apf_base-2.4.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:46:07.000000 apf_base-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-22 14:45:31.000000 apf_base-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-22 14:46:07.000000 apf_base-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-22 14:45:31.000000 apf_base-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:46:07.000000 apf_base-2.3.0/apf/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:46:07.000000 apf_base-2.3.0/apf/consumers/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-22 14:45:31.000000 apf_base-2.3.0/apf/consumers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-22 14:45:31.000000 apf_base-2.3.0/apf/consumers/avro_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-22 14:45:31.000000 apf_base-2.3.0/apf/consumers/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-22 14:45:31.000000 apf_base-2.3.0/apf/consumers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-22 14:45:31.000000 apf_base-2.3.0/apf/consumers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-05-22 14:45:31.000000 apf_base-2.3.0/apf/consumers/kafka.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:46:07.000000 apf_base-2.3.0/apf/core/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-22 14:45:31.000000 apf_base-2.3.0/apf/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:46:07.000000 apf_base-2.3.0/apf/core/management/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-22 14:45:31.000000 apf_base-2.3.0/apf/core/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-22 14:45:31.000000 apf_base-2.3.0/apf/core/management/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-22 14:45:31.000000 apf_base-2.3.0/apf/core/secret_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    15312 2023-05-22 14:45:31.000000 apf_base-2.3.0/apf/core/step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:46:07.000000 apf_base-2.3.0/apf/core/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:46:07.000000 apf_base-2.3.0/apf/core/templates/step/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-22 14:45:31.000000 apf_base-2.3.0/apf/core/templates/step/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:46:07.000000 apf_base-2.3.0/apf/core/templates/step/package/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-22 14:45:31.000000 apf_base-2.3.0/apf/core/templates/step/package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-22 14:45:31.000000 apf_base-2.3.0/apf/core/templates/step/package/step.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-22 14:45:31.000000 apf_base-2.3.0/apf/core/templates/step/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:46:07.000000 apf_base-2.3.0/apf/core/templates/step/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-22 14:45:31.000000 apf_base-2.3.0/apf/core/templates/step/scripts/run_step.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-22 14:45:31.000000 apf_base-2.3.0/apf/core/templates/step/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 14:45:31.000000 apf_base-2.3.0/apf/core/templates/step/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-22 14:45:31.000000 apf_base-2.3.0/apf/core/topic_management.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:46:07.000000 apf_base-2.3.0/apf/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-22 14:45:31.000000 apf_base-2.3.0/apf/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-22 14:45:31.000000 apf_base-2.3.0/apf/metrics/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-22 14:45:31.000000 apf_base-2.3.0/apf/metrics/kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-22 14:45:31.000000 apf_base-2.3.0/apf/metrics/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:46:07.000000 apf_base-2.3.0/apf/metrics/prometheus/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-22 14:45:31.000000 apf_base-2.3.0/apf/metrics/prometheus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-22 14:45:31.000000 apf_base-2.3.0/apf/metrics/prometheus/prometheus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:46:07.000000 apf_base-2.3.0/apf/producers/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-22 14:45:31.000000 apf_base-2.3.0/apf/producers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-22 14:45:31.000000 apf_base-2.3.0/apf/producers/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-22 14:45:31.000000 apf_base-2.3.0/apf/producers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-22 14:45:31.000000 apf_base-2.3.0/apf/producers/json_prod.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-22 14:45:31.000000 apf_base-2.3.0/apf/producers/kafka.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:46:07.000000 apf_base-2.3.0/apf_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-22 14:46:07.000000 apf_base-2.3.0/apf_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-22 14:46:07.000000 apf_base-2.3.0/apf_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 14:46:07.000000 apf_base-2.3.0/apf_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-22 14:46:07.000000 apf_base-2.3.0/apf_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-22 14:46:07.000000 apf_base-2.3.0/apf_base.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:46:07.000000 apf_base-2.3.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-22 14:45:31.000000 apf_base-2.3.0/scripts/apf
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 14:46:07.000000 apf_base-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-22 14:45:31.000000 apf_base-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:40:48.000000 apf_base-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-23 16:40:22.000000 apf_base-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-23 16:40:48.000000 apf_base-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-23 16:40:22.000000 apf_base-2.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:40:48.000000 apf_base-2.4.0/apf/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:40:48.000000 apf_base-2.4.0/apf/consumers/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/consumers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/consumers/avro_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/consumers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/consumers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/consumers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/consumers/kafka.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:40:48.000000 apf_base-2.4.0/apf/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:40:48.000000 apf_base-2.4.0/apf/core/management/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/core/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/core/management/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/core/secret_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15241 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/core/step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:40:48.000000 apf_base-2.4.0/apf/core/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:40:48.000000 apf_base-2.4.0/apf/core/templates/step/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/core/templates/step/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:40:48.000000 apf_base-2.4.0/apf/core/templates/step/package/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/core/templates/step/package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/core/templates/step/package/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/core/templates/step/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:40:48.000000 apf_base-2.4.0/apf/core/templates/step/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/core/templates/step/scripts/run_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/core/templates/step/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/core/templates/step/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/core/topic_management.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:40:48.000000 apf_base-2.4.0/apf/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/metrics/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/metrics/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/metrics/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:40:48.000000 apf_base-2.4.0/apf/metrics/prometheus/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/metrics/prometheus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/metrics/prometheus/prometheus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:40:48.000000 apf_base-2.4.0/apf/producers/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/producers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/producers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/producers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/producers/json_prod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-23 16:40:22.000000 apf_base-2.4.0/apf/producers/kafka.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:40:48.000000 apf_base-2.4.0/apf_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-23 16:40:48.000000 apf_base-2.4.0/apf_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-23 16:40:48.000000 apf_base-2.4.0/apf_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 16:40:48.000000 apf_base-2.4.0/apf_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-23 16:40:48.000000 apf_base-2.4.0/apf_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-23 16:40:48.000000 apf_base-2.4.0/apf_base.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:40:48.000000 apf_base-2.4.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-23 16:40:22.000000 apf_base-2.4.0/scripts/apf
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 16:40:48.000000 apf_base-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-23 16:40:22.000000 apf_base-2.4.0/setup.py
```

### Comparing `apf_base-2.3.0/LICENSE` & `apf_base-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `apf_base-2.3.0/PKG-INFO` & `apf_base-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apf_base
-Version: 2.3.0
+Version: 2.4.0
 Summary: ALeRCE Alert Processing Framework.
 Author: ALeRCE Team
 Author-email: contact@alerce.online
 Project-URL: Github, https://github.com/alercebroker/APF
 Project-URL: Documentation, https://apf.readthedocs.io/en/latest/index.html
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `apf_base-2.3.0/README.md` & `apf_base-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `apf_base-2.3.0/apf/consumers/avro_file.py` & `apf_base-2.4.0/apf/consumers/avro_file.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.3.0/apf/consumers/csv.py` & `apf_base-2.4.0/apf/consumers/csv.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.3.0/apf/consumers/generic.py` & `apf_base-2.4.0/apf/consumers/generic.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 class GenericConsumer(ABC):
     """Generic Consumer for Alert Processing Framework.
 
     Parameters are passed through *config* as a :py:class:`dict` of params.
     """
 
     def __init__(self, config=None):
-        self.logger = logging.getLogger(self.__class__.__name__)
+        self.logger = logging.getLogger(f"alerce.{self.__class__.__name__}")
         self.logger.info(f"Creating {self.__class__.__name__}")
         self.config = config
 
     @abstractmethod
     def consume(self) -> Generator[Union[list, dict], None, None]:
         """Get a message from a data source
```

### Comparing `apf_base-2.3.0/apf/consumers/json.py` & `apf_base-2.4.0/apf/consumers/json.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.3.0/apf/consumers/kafka.py` & `apf_base-2.4.0/apf/consumers/kafka.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.3.0/apf/core/__init__.py` & `apf_base-2.4.0/apf/core/__init__.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.3.0/apf/core/management/helpers.py` & `apf_base-2.4.0/apf/core/management/helpers.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.3.0/apf/core/secret_manager.py` & `apf_base-2.4.0/apf/core/secret_manager.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.3.0/apf/core/step.py` & `apf_base-2.4.0/apf/core/step.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,18 +48,17 @@
 
     def __init__(
         self,
         consumer: Type[GenericConsumer] = DefaultConsumer,
         producer: Type[GenericProducer] = DefaultProducer,
         metrics_sender: Type[GenericMetricsProducer] = DefaultMetricsProducer,
         config: dict = {},
-        level: int = logging.INFO,
         prometheus_metrics: PrometheusMetrics = DefaultPrometheusMetrics(),
     ):
-        self._set_logger(level)
+        self._set_logger()
         self.config = config
         self.consumer = self._get_consumer(consumer)(self.consumer_config)
         self.producer = self._get_producer(producer)(self.producer_config)
         self.metrics_sender = self._get_metrics_sender(metrics_sender)(
             self.metrics_producer_params
         )
         self.metrics = {}
@@ -83,17 +82,16 @@
 
     @property
     def metrics_producer_params(self) -> dict:
         if self.metrics_config:
             return self.metrics_config["PARAMS"]
         return {}
 
-    def _set_logger(self, level):
-        self.logger = logging.getLogger(self.__class__.__name__)
-        self.logger.setLevel(level)
+    def _set_logger(self):
+        self.logger = logging.getLogger(f"alerce.{self.__class__.__name__}")
         self.logger.info(f"Creating {self.__class__.__name__}")
 
     def _get_consumer(self, default: Type[GenericConsumer]) -> Type[GenericConsumer]:
         if self.consumer_config:
             Consumer = default
             if "CLASS" in self.consumer_config:
                 Consumer = get_class(self.consumer_config["CLASS"])
```

### Comparing `apf_base-2.3.0/apf/core/templates/step/package/step.py` & `apf_base-2.4.0/apf/core/templates/step/package/step.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.3.0/apf/core/topic_management.py` & `apf_base-2.4.0/apf/core/topic_management.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.3.0/apf/metrics/generic.py` & `apf_base-2.4.0/apf/metrics/generic.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         if isinstance(obj, (datetime.date, datetime.datetime)):
             return obj.isoformat()
 
 
 class GenericMetricsProducer(abc.ABC):
     def __init__(self, config):
         self.config = config
-        self.logger = logging.getLogger(self.__class__.__name__)
+        self.logger = logging.getLogger(f"alerce.{self.__class__.__name__}")
         self.logger.info(f"Creating {self.__class__.__name__}")
 
     @abc.abstractmethod
     def send_metrics(self, metrics):
         """Write metrics into a data store or other metrics system.
 
         Parameters
```

### Comparing `apf_base-2.3.0/apf/metrics/kafka.py` & `apf_base-2.4.0/apf/metrics/kafka.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.3.0/apf/metrics/log.py` & `apf_base-2.4.0/apf/metrics/log.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.3.0/apf/metrics/prometheus/prometheus.py` & `apf_base-2.4.0/apf/metrics/prometheus/prometheus.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.3.0/apf/producers/csv.py` & `apf_base-2.4.0/apf/producers/csv.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.3.0/apf/producers/generic.py` & `apf_base-2.4.0/apf/producers/generic.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 from typing import Union
 
 
 class GenericProducer(ABC):
     """Generic Producer for Alert Processing Framework."""
 
     def __init__(self, config=None):
-        self.logger = logging.getLogger(self.__class__.__name__)
+        self.logger = logging.getLogger(f"alerce.{self.__class__.__name__}")
         self.logger.info(f"Creating {self.__class__.__name__}")
         self.config = config
         self._key_field = None
 
     @property
     def key_field(self):
         return self._key_field
 
     def set_key_field(self, key):
+        """Set key used when indexing produced messages."""
         self._key_field = key
 
     @abstractmethod
     def produce(self, message=None, **kwargs):
         """Send a message after processing.
 
         Parameters
```

### Comparing `apf_base-2.3.0/apf/producers/json_prod.py` & `apf_base-2.4.0/apf/producers/json_prod.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from pandas import DataFrame, read_json, concat
 import pathlib
 
 
 class JSONProducer(GenericProducer):
     """JSON Producer
 
-    Parameters
-    ----------
-    FILE_PATH: :py:class:`str`
-        Output JSON File Directory.
-
     This producer creates multiple output files (json)
     according to the buffer size, where each file contains
     `buffer_size` elements.
 
     Every file is created in the `FILE_PATH` directory
     and each output file is named producer_output{i} where `i` is
     a counter for the times the buffer has completed.
+
+    Parameters
+    ----------
+    FILE_PATH: :py:class:`str`
+        Output JSON File Directory.
     """
 
     def __init__(self, config):
         super().__init__(config=config)
         self.buffer = DataFrame()
         self.buffer_size = config.get("buffer_size", 1)
         self.file_counter = 0
```

### Comparing `apf_base-2.3.0/apf/producers/kafka.py` & `apf_base-2.4.0/apf/producers/kafka.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.3.0/apf_base.egg-info/PKG-INFO` & `apf_base-2.4.0/apf_base.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apf-base
-Version: 2.3.0
+Version: 2.4.0
 Summary: ALeRCE Alert Processing Framework.
 Author: ALeRCE Team
 Author-email: contact@alerce.online
 Project-URL: Github, https://github.com/alercebroker/APF
 Project-URL: Documentation, https://apf.readthedocs.io/en/latest/index.html
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `apf_base-2.3.0/apf_base.egg-info/SOURCES.txt` & `apf_base-2.4.0/apf_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apf_base-2.3.0/setup.py` & `apf_base-2.4.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="apf_base",
-    version="2.3.0",
+    version="2.4.0",
     description="ALeRCE Alert Processing Framework.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ALeRCE Team",
     author_email="contact@alerce.online",
     packages=find_namespace_packages(include=["apf.*"]),
     scripts=["scripts/apf"],
```

