# Comparing `tmp/pyworxcloud-3.1.8.tar.gz` & `tmp/pyworxcloud-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyworxcloud-3.1.8.tar", max compression
+gzip compressed data, was "pyworxcloud-3.1.9.tar", max compression
```

## Comparing `pyworxcloud-3.1.8.tar` & `pyworxcloud-3.1.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    35149 2023-05-22 06:38:43.036491 pyworxcloud-3.1.8/LICENSE
--rw-r--r--   0        0        0      929 2023-05-22 06:38:43.036491 pyworxcloud-3.1.8/README.md
--rw-r--r--   0        0        0      609 2023-05-22 06:38:59.128650 pyworxcloud-3.1.8/pyproject.toml
--rw-r--r--   0        0        0    29688 2023-05-22 06:38:43.036491 pyworxcloud-3.1.8/pyworxcloud/__init__.py
--rw-r--r--   0        0        0     4804 2023-05-22 06:38:43.036491 pyworxcloud-3.1.8/pyworxcloud/api.py
--rw-r--r--   0        0        0     1134 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/clouds.py
--rw-r--r--   0        0        0      927 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/const.py
--rw-r--r--   0        0        0      204 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/day_map.py
--rw-r--r--   0        0        0     3647 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/events.py
--rw-r--r--   0        0        0     2115 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/exceptions.py
--rw-r--r--   0        0        0      204 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/helpers/__init__.py
--rw-r--r--   0        0        0      637 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/helpers/logger.py
--rw-r--r--   0        0        0     2794 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/helpers/time_format.py
--rw-r--r--   0        0        0      838 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/__init__.py
--rw-r--r--   0        0        0     3338 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/battery.py
--rw-r--r--   0        0        0     2091 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/blades.py
--rw-r--r--   0        0        0     1924 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/capability.py
--rw-r--r--   0        0        0     3623 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/devices.py
--rw-r--r--   0        0        0      617 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/firmware.py
--rw-r--r--   0        0        0      281 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/landroid_class.py
--rw-r--r--   0        0        0      306 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/lawn.py
--rw-r--r--   0        0        0      427 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/location.py
--rw-r--r--   0        0        0     8300 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/mqtt.py
--rw-r--r--   0        0        0      411 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/orientation.py
--rw-r--r--   0        0        0     1348 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/product.py
--rw-r--r--   0        0        0     1109 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/rainsensor.py
--rw-r--r--   0        0        0     3188 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/requests.py
--rw-r--r--   0        0        0     6191 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/schedules.py
--rw-r--r--   0        0        0     2050 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/state.py
--rw-r--r--   0        0        0      657 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/statistics.py
--rw-r--r--   0        0        0      726 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/warranty.py
--rw-r--r--   0        0        0     2116 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/zone.py
--rw-r--r--   0        0        0     1747 1970-01-01 00:00:00.000000 pyworxcloud-3.1.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-23 13:12:41.405572 pyworxcloud-3.1.9/LICENSE
+-rw-r--r--   0        0        0      929 2023-05-23 13:12:41.405572 pyworxcloud-3.1.9/README.md
+-rw-r--r--   0        0        0      608 2023-05-23 13:12:56.109457 pyworxcloud-3.1.9/pyproject.toml
+-rw-r--r--   0        0        0    29688 2023-05-23 13:12:41.409572 pyworxcloud-3.1.9/pyworxcloud/__init__.py
+-rw-r--r--   0        0        0     4804 2023-05-23 13:12:41.409572 pyworxcloud-3.1.9/pyworxcloud/api.py
+-rw-r--r--   0        0        0     1128 2023-05-23 13:12:41.409572 pyworxcloud-3.1.9/pyworxcloud/clouds.py
+-rw-r--r--   0        0        0      927 2023-05-23 13:12:41.409572 pyworxcloud-3.1.9/pyworxcloud/const.py
+-rw-r--r--   0        0        0      204 2023-05-23 13:12:41.413572 pyworxcloud-3.1.9/pyworxcloud/day_map.py
+-rw-r--r--   0        0        0     3647 2023-05-23 13:12:41.413572 pyworxcloud-3.1.9/pyworxcloud/events.py
+-rw-r--r--   0        0        0     2115 2023-05-23 13:12:41.413572 pyworxcloud-3.1.9/pyworxcloud/exceptions.py
+-rw-r--r--   0        0        0      204 2023-05-23 13:12:41.413572 pyworxcloud-3.1.9/pyworxcloud/helpers/__init__.py
+-rw-r--r--   0        0        0      637 2023-05-23 13:12:41.413572 pyworxcloud-3.1.9/pyworxcloud/helpers/logger.py
+-rw-r--r--   0        0        0     2794 2023-05-23 13:12:41.413572 pyworxcloud-3.1.9/pyworxcloud/helpers/time_format.py
+-rw-r--r--   0        0        0      838 2023-05-23 13:12:41.413572 pyworxcloud-3.1.9/pyworxcloud/utils/__init__.py
+-rw-r--r--   0        0        0     3338 2023-05-23 13:12:41.413572 pyworxcloud-3.1.9/pyworxcloud/utils/battery.py
+-rw-r--r--   0        0        0     2091 2023-05-23 13:12:41.413572 pyworxcloud-3.1.9/pyworxcloud/utils/blades.py
+-rw-r--r--   0        0        0     1924 2023-05-23 13:12:41.413572 pyworxcloud-3.1.9/pyworxcloud/utils/capability.py
+-rw-r--r--   0        0        0     3623 2023-05-23 13:12:41.413572 pyworxcloud-3.1.9/pyworxcloud/utils/devices.py
+-rw-r--r--   0        0        0      617 2023-05-23 13:12:41.413572 pyworxcloud-3.1.9/pyworxcloud/utils/firmware.py
+-rw-r--r--   0        0        0      281 2023-05-23 13:12:41.413572 pyworxcloud-3.1.9/pyworxcloud/utils/landroid_class.py
+-rw-r--r--   0        0        0      306 2023-05-23 13:12:41.413572 pyworxcloud-3.1.9/pyworxcloud/utils/lawn.py
+-rw-r--r--   0        0        0      427 2023-05-23 13:12:41.413572 pyworxcloud-3.1.9/pyworxcloud/utils/location.py
+-rw-r--r--   0        0        0     8300 2023-05-23 13:12:41.413572 pyworxcloud-3.1.9/pyworxcloud/utils/mqtt.py
+-rw-r--r--   0        0        0      411 2023-05-23 13:12:41.413572 pyworxcloud-3.1.9/pyworxcloud/utils/orientation.py
+-rw-r--r--   0        0        0     1348 2023-05-23 13:12:41.413572 pyworxcloud-3.1.9/pyworxcloud/utils/product.py
+-rw-r--r--   0        0        0     1109 2023-05-23 13:12:41.413572 pyworxcloud-3.1.9/pyworxcloud/utils/rainsensor.py
+-rw-r--r--   0        0        0     3188 2023-05-23 13:12:41.413572 pyworxcloud-3.1.9/pyworxcloud/utils/requests.py
+-rw-r--r--   0        0        0     6191 2023-05-23 13:12:41.413572 pyworxcloud-3.1.9/pyworxcloud/utils/schedules.py
+-rw-r--r--   0        0        0     2050 2023-05-23 13:12:41.413572 pyworxcloud-3.1.9/pyworxcloud/utils/state.py
+-rw-r--r--   0        0        0      657 2023-05-23 13:12:41.413572 pyworxcloud-3.1.9/pyworxcloud/utils/statistics.py
+-rw-r--r--   0        0        0      726 2023-05-23 13:12:41.413572 pyworxcloud-3.1.9/pyworxcloud/utils/warranty.py
+-rw-r--r--   0        0        0     2116 2023-05-23 13:12:41.417572 pyworxcloud-3.1.9/pyworxcloud/utils/zone.py
+-rw-r--r--   0        0        0     1740 1970-01-01 00:00:00.000000 pyworxcloud-3.1.9/PKG-INFO
```

### Comparing `pyworxcloud-3.1.8/LICENSE` & `pyworxcloud-3.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.8/README.md` & `pyworxcloud-3.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.8/pyproject.toml` & `pyworxcloud-3.1.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pyworxcloud"
-version = "v3.1.8"
+version = "v3.1.9"
 description = "Landroid cloud (Positec) API library"
 authors = ["Malene Trab <malene@trab.dk>"]
 documentation = "https://github.com/mtrab/pyworxcloud"
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 
@@ -17,9 +17,9 @@
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/mtrab/pyworxcloud/issues"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 urllib3 = "^1.26.10"
-requests = "^2.26.0"
+requests = "2.31.0"
 paho-mqtt = "^1.6.1"
```

### Comparing `pyworxcloud-3.1.8/pyworxcloud/__init__.py` & `pyworxcloud-3.1.9/pyworxcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.8/pyworxcloud/api.py` & `pyworxcloud-3.1.9/pyworxcloud/api.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.8/pyworxcloud/clouds.py` & `pyworxcloud-3.1.9/pyworxcloud/clouds.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,23 +17,23 @@
     """
 
     class WORX(str):
         """Settings for Worx devices."""
 
         BRAND_PREFIX: str = "WX"
         ENDPOINT: str = "api.worxlandroid.com"
-        AUTH_ENDPOINT: str = "id.eu.worx.com"
+        AUTH_ENDPOINT: str = "id.worx.com"
         AUTH_CLIENT_ID: str = "150da4d2-bb44-433b-9429-3773adc70a2a"
 
     class KRESS(str):
         """Settings for Kress devices."""
 
         BRAND_PREFIX: str = "KR"
         ENDPOINT: str = "api.kress-robotik.com"
-        AUTH_ENDPOINT: str = "id.eu.kress.com"
+        AUTH_ENDPOINT: str = "id.kress.com"
         AUTH_CLIENT_ID: str = "931d4bc4-3192-405a-be78-98e43486dc59"
 
     class LANDXCAPE(str):
         """Settings for Landxcape devices."""
 
         BRAND_PREFIX: str = "LX"
         ENDPOINT: str = "api.landxcape-services.com"
```

### Comparing `pyworxcloud-3.1.8/pyworxcloud/const.py` & `pyworxcloud-3.1.9/pyworxcloud/const.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.8/pyworxcloud/events.py` & `pyworxcloud-3.1.9/pyworxcloud/events.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.8/pyworxcloud/exceptions.py` & `pyworxcloud-3.1.9/pyworxcloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.8/pyworxcloud/helpers/logger.py` & `pyworxcloud-3.1.9/pyworxcloud/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.8/pyworxcloud/helpers/time_format.py` & `pyworxcloud-3.1.9/pyworxcloud/helpers/time_format.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.8/pyworxcloud/utils/__init__.py` & `pyworxcloud-3.1.9/pyworxcloud/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.8/pyworxcloud/utils/battery.py` & `pyworxcloud-3.1.9/pyworxcloud/utils/battery.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.8/pyworxcloud/utils/blades.py` & `pyworxcloud-3.1.9/pyworxcloud/utils/blades.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.8/pyworxcloud/utils/capability.py` & `pyworxcloud-3.1.9/pyworxcloud/utils/capability.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.8/pyworxcloud/utils/devices.py` & `pyworxcloud-3.1.9/pyworxcloud/utils/devices.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.8/pyworxcloud/utils/firmware.py` & `pyworxcloud-3.1.9/pyworxcloud/utils/firmware.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.8/pyworxcloud/utils/mqtt.py` & `pyworxcloud-3.1.9/pyworxcloud/utils/mqtt.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.8/pyworxcloud/utils/product.py` & `pyworxcloud-3.1.9/pyworxcloud/utils/product.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.8/pyworxcloud/utils/rainsensor.py` & `pyworxcloud-3.1.9/pyworxcloud/utils/rainsensor.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.8/pyworxcloud/utils/requests.py` & `pyworxcloud-3.1.9/pyworxcloud/utils/requests.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.8/pyworxcloud/utils/schedules.py` & `pyworxcloud-3.1.9/pyworxcloud/utils/schedules.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.8/pyworxcloud/utils/state.py` & `pyworxcloud-3.1.9/pyworxcloud/utils/state.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.8/pyworxcloud/utils/statistics.py` & `pyworxcloud-3.1.9/pyworxcloud/utils/statistics.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.8/pyworxcloud/utils/warranty.py` & `pyworxcloud-3.1.9/pyworxcloud/utils/warranty.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.8/pyworxcloud/utils/zone.py` & `pyworxcloud-3.1.9/pyworxcloud/utils/zone.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.8/PKG-INFO` & `pyworxcloud-3.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyworxcloud
-Version: 3.1.8
+Version: 3.1.9
 Summary: Landroid cloud (Positec) API library
 License: MIT
 Author: Malene Trab
 Author-email: malene@trab.dk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: paho-mqtt (>=1.6.1,<2.0.0)
-Requires-Dist: requests (>=2.26.0,<3.0.0)
+Requires-Dist: requests (==2.31.0)
 Requires-Dist: urllib3 (>=1.26.10,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/mtrab/pyworxcloud/issues
 Project-URL: Documentation, https://github.com/mtrab/pyworxcloud
 Description-Content-Type: text/markdown
 
 <a href="https://www.buymeacoffee.com/mtrab" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" ></a>
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: pyworxcloud Version: 3.1.8 Summary: Landroid cloud
+Metadata-Version: 2.1 Name: pyworxcloud Version: 3.1.9 Summary: Landroid cloud
 (Positec) API library License: MIT Author: Malene Trab Author-email:
 malene@trab.dk Requires-Python: >=3.9,<4.0 Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Software Development :: Libraries :: Python Modules Requires-Dist:
-paho-mqtt (>=1.6.1,<2.0.0) Requires-Dist: requests (>=2.26.0,<3.0.0) Requires-
-Dist: urllib3 (>=1.26.10,<2.0.0) Project-URL: Bug Tracker, https://github.com/
-mtrab/pyworxcloud/issues Project-URL: Documentation, https://github.com/mtrab/
+paho-mqtt (>=1.6.1,<2.0.0) Requires-Dist: requests (==2.31.0) Requires-Dist:
+urllib3 (>=1.26.10,<2.0.0) Project-URL: Bug Tracker, https://github.com/mtrab/
+pyworxcloud/issues Project-URL: Documentation, https://github.com/mtrab/
 pyworxcloud Description-Content-Type: text/markdown [Buy_Me_A_Coffee] #
 pyWorxCloud This is a PyPI module for communicating with Worx Cloud mowers,
 primarily developed for use with [Home Assistant](https://home-assistant.io),
 but I try to keep it as widely usable as possible.
 
 The module are compatible with cloud enabled devices from [these vendors]
 (https://github.com/MTrab/pyworxcloud/wiki#current-supported-brands--vendors)
```

