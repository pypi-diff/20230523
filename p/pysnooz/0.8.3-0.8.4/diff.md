# Comparing `tmp/pysnooz-0.8.3.tar.gz` & `tmp/pysnooz-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysnooz-0.8.3.tar", max compression
+gzip compressed data, was "pysnooz-0.8.4.tar", max compression
```

## Comparing `pysnooz-0.8.3.tar` & `pysnooz-0.8.4.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     1075 2022-10-27 02:42:35.403226 pysnooz-0.8.3/LICENSE
--rw-r--r--   0        0        0     3048 2022-10-27 02:42:35.403226 pysnooz-0.8.3/README.md
--rw-r--r--   0        0        0     2233 2022-10-27 02:42:36.331270 pysnooz-0.8.3/pyproject.toml
--rw-r--r--   0        0        0       22 2022-10-27 02:42:36.279267 pysnooz-0.8.3/src/pysnooz/__init__.py
--rw-r--r--   0        0        0     2143 2022-10-27 02:42:35.407227 pysnooz-0.8.3/src/pysnooz/advertisement.py
--rw-r--r--   0        0        0     5155 2022-10-27 02:42:35.407227 pysnooz-0.8.3/src/pysnooz/api.py
--rw-r--r--   0        0        0    13797 2022-10-27 02:42:35.407227 pysnooz-0.8.3/src/pysnooz/commands.py
--rw-r--r--   0        0        0      310 2022-10-27 02:42:35.407227 pysnooz-0.8.3/src/pysnooz/const.py
--rw-r--r--   0        0        0    17686 2022-10-27 02:42:35.407227 pysnooz-0.8.3/src/pysnooz/device.py
--rw-r--r--   0        0        0        0 2022-10-27 02:42:35.407227 pysnooz-0.8.3/src/pysnooz/py.typed
--rw-r--r--   0        0        0     6420 2022-10-27 02:42:35.407227 pysnooz-0.8.3/src/pysnooz/testing.py
--rw-r--r--   0        0        0     3110 2022-10-27 02:42:35.407227 pysnooz-0.8.3/src/pysnooz/transition.py
--rw-r--r--   0        0        0     4008 1970-01-01 00:00:00.000000 pysnooz-0.8.3/setup.py
--rw-r--r--   0        0        0     4317 1970-01-01 00:00:00.000000 pysnooz-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-05-23 17:05:02.937055 pysnooz-0.8.4/LICENSE
+-rw-r--r--   0        0        0     3048 2023-05-23 17:05:02.937055 pysnooz-0.8.4/README.md
+-rw-r--r--   0        0        0     2234 2023-05-23 17:05:03.721089 pysnooz-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-23 17:05:03.681088 pysnooz-0.8.4/src/pysnooz/__init__.py
+-rw-r--r--   0        0        0     2143 2023-05-23 17:05:02.937055 pysnooz-0.8.4/src/pysnooz/advertisement.py
+-rw-r--r--   0        0        0     5155 2023-05-23 17:05:02.937055 pysnooz-0.8.4/src/pysnooz/api.py
+-rw-r--r--   0        0        0    13797 2023-05-23 17:05:02.941055 pysnooz-0.8.4/src/pysnooz/commands.py
+-rw-r--r--   0        0        0      310 2023-05-23 17:05:02.941055 pysnooz-0.8.4/src/pysnooz/const.py
+-rw-r--r--   0        0        0    17684 2023-05-23 17:05:02.941055 pysnooz-0.8.4/src/pysnooz/device.py
+-rw-r--r--   0        0        0        0 2023-05-23 17:05:02.941055 pysnooz-0.8.4/src/pysnooz/py.typed
+-rw-r--r--   0        0        0     6420 2023-05-23 17:05:02.941055 pysnooz-0.8.4/src/pysnooz/testing.py
+-rw-r--r--   0        0        0     3110 2023-05-23 17:05:02.941055 pysnooz-0.8.4/src/pysnooz/transition.py
+-rw-r--r--   0        0        0     4268 1970-01-01 00:00:00.000000 pysnooz-0.8.4/PKG-INFO
```

### Comparing `pysnooz-0.8.3/LICENSE` & `pysnooz-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pysnooz-0.8.3/README.md` & `pysnooz-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `pysnooz-0.8.3/pyproject.toml` & `pysnooz-0.8.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysnooz"
-version = "0.8.3"
+version = "0.8.4"
 description = "Control SNOOZ white noise machines."
 authors = ["Austin Brunkhorst <pysnooz@alb.dev>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/AustinBrunkhorst/pysnooz"
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -16,25 +16,25 @@
 packages = [{ include = "pysnooz", from = "src" }]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/AustinBrunkhorst/pysnooz/issues"
 "Changelog" = "https://github.com/AustinBrunkhorst/pysnooz/blob/main/CHANGELOG.md"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
 home-assistant-bluetooth = ">=1.3.0"
 bluetooth-sensor-state-data = ">=1.5.0"
-bleak-retry-connector = ">=2.1.3"
-bleak = ">=0.18.1"
+bleak-retry-connector = ">=3.0.2"
+bleak = ">=0.20.2"
 Events = "^0.4"
 transitions = "^0.8.11"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0"
-pytest-cov = "^3.0"
+pytest-cov = "^4.0"
 pytest-asyncio = "^0.19.0"
 freezegun = "^1.2.2"
 pytest-mock = "^3.8.2"
 pandas = "^1.4.3"
 autopep8 = "^1.7.0"
 flake8 = "^5.0.4"
```

### Comparing `pysnooz-0.8.3/src/pysnooz/advertisement.py` & `pysnooz-0.8.4/src/pysnooz/advertisement.py`

 * *Files identical despite different names*

### Comparing `pysnooz-0.8.3/src/pysnooz/api.py` & `pysnooz-0.8.4/src/pysnooz/api.py`

 * *Files identical despite different names*

### Comparing `pysnooz-0.8.3/src/pysnooz/commands.py` & `pysnooz-0.8.4/src/pysnooz/commands.py`

 * *Files identical despite different names*

### Comparing `pysnooz-0.8.3/src/pysnooz/device.py` & `pysnooz-0.8.4/src/pysnooz/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,15 @@
                 reason=DisconnectionReason.DEVICE
             )
             api.events.on_state_change += lambda state: self._on_receive_device_state(
                 state
             )
             self._before_device_connected()
             self._api = api
-        except (DEVICE_UNAVAILABLE_EXCEPTIONS) as ex:
+        except DEVICE_UNAVAILABLE_EXCEPTIONS as ex:
             raise SnoozDeviceUnavailableError() from ex
 
         # ensure each call with side effects checks the connection status
         # to prevent a cancellation race condition
 
         if self.connection_status == SnoozConnectionStatus.CONNECTING:
             await api.async_authenticate_connection(bytes.fromhex(self._token))
```

### Comparing `pysnooz-0.8.3/src/pysnooz/testing.py` & `pysnooz-0.8.4/src/pysnooz/testing.py`

 * *Files identical despite different names*

### Comparing `pysnooz-0.8.3/src/pysnooz/transition.py` & `pysnooz-0.8.4/src/pysnooz/transition.py`

 * *Files identical despite different names*

### Comparing `pysnooz-0.8.3/PKG-INFO` & `pysnooz-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: pysnooz
-Version: 0.8.3
+Version: 0.8.4
 Summary: Control SNOOZ white noise machines.
 Home-page: https://github.com/AustinBrunkhorst/pysnooz
 License: MIT
 Author: Austin Brunkhorst
 Author-email: pysnooz@alb.dev
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: Events (>=0.4,<0.5)
-Requires-Dist: bleak (>=0.18.1)
-Requires-Dist: bleak-retry-connector (>=2.1.3)
+Requires-Dist: bleak (>=0.20.2)
+Requires-Dist: bleak-retry-connector (>=3.0.2)
 Requires-Dist: bluetooth-sensor-state-data (>=1.5.0)
 Requires-Dist: home-assistant-bluetooth (>=1.3.0)
 Requires-Dist: transitions (>=0.8.11,<0.9.0)
 Project-URL: Bug Tracker, https://github.com/AustinBrunkhorst/pysnooz/issues
 Project-URL: Changelog, https://github.com/AustinBrunkhorst/pysnooz/blob/main/CHANGELOG.md
 Project-URL: Repository, https://github.com/AustinBrunkhorst/pysnooz
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: pysnooz Version: 0.8.3 Summary: Control SNOOZ white
+Metadata-Version: 2.1 Name: pysnooz Version: 0.8.4 Summary: Control SNOOZ white
 noise machines. Home-page: https://github.com/AustinBrunkhorst/pysnooz License:
 MIT Author: Austin Brunkhorst Author-email: pysnooz@alb.dev Requires-Python:
->=3.9,<4.0 Classifier: Development Status :: 4 - Beta Classifier: Intended
+>=3.10,<4.0 Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Topic :: Software Development :: Libraries Requires-Dist: Events (>=0.4,<0.5)
-Requires-Dist: bleak (>=0.18.1) Requires-Dist: bleak-retry-connector (>=2.1.3)
-Requires-Dist: bluetooth-sensor-state-data (>=1.5.0) Requires-Dist: home-
-assistant-bluetooth (>=1.3.0) Requires-Dist: transitions (>=0.8.11,<0.9.0)
-Project-URL: Bug Tracker, https://github.com/AustinBrunkhorst/pysnooz/issues
-Project-URL: Changelog, https://github.com/AustinBrunkhorst/pysnooz/blob/main/
-CHANGELOG.md Project-URL: Repository, https://github.com/AustinBrunkhorst/
-pysnooz Description-Content-Type: text/markdown # PySnooz
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Topic :: Software Development :: Libraries Requires-
+Dist: Events (>=0.4,<0.5) Requires-Dist: bleak (>=0.20.2) Requires-Dist: bleak-
+retry-connector (>=3.0.2) Requires-Dist: bluetooth-sensor-state-data (>=1.5.0)
+Requires-Dist: home-assistant-bluetooth (>=1.3.0) Requires-Dist: transitions
+(>=0.8.11,<0.9.0) Project-URL: Bug Tracker, https://github.com/
+AustinBrunkhorst/pysnooz/issues Project-URL: Changelog, https://github.com/
+AustinBrunkhorst/pysnooz/blob/main/CHANGELOG.md Project-URL: Repository, https:
+//github.com/AustinBrunkhorst/pysnooz Description-Content-Type: text/markdown #
+PySnooz
            [Python Language + Bleak API + SNOOZ White Noise Machine]
 [CI_Status] [Test_coverage_percentage] [PyPI_Version]
 Control SNOOZ white noise machines with Bluetooth. ## Installation Install this
 via pip (or your favourite package manager): `pip install pysnooz` ## Usage
 ```python import asyncio from datetime import timedelta from
 bleak.backends.client import BLEDevice from pysnooz.device import SnoozDevice
 from pysnooz.commands import SnoozCommandResultStatus, turn_on, turn_off,
```

