# Comparing `tmp/bosch_alarm_mode2-0.3.1.tar.gz` & `tmp/bosch_alarm_mode2-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bosch_alarm_mode2-0.3.1.tar", max compression
+gzip compressed data, was "bosch_alarm_mode2-0.3.2.tar", max compression
```

## Comparing `bosch_alarm_mode2-0.3.1.tar` & `bosch_alarm_mode2-0.3.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       48 2023-05-21 02:31:10.469944 bosch_alarm_mode2-0.3.1/bosch_alarm_mode2/__init__.py
--rw-r--r--   0        0        0     2330 2023-05-21 03:21:31.913252 bosch_alarm_mode2-0.3.1/bosch_alarm_mode2/connection.py
--rw-r--r--   0        0        0     4220 2023-05-22 09:16:58.475238 bosch_alarm_mode2-0.3.1/bosch_alarm_mode2/const.py
--rw-r--r--   0        0        0    17857 2023-05-22 22:46:13.719931 bosch_alarm_mode2-0.3.1/bosch_alarm_mode2/panel.py
--rw-r--r--   0        0        0      262 2023-05-22 22:46:55.989931 bosch_alarm_mode2-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      355 1970-01-01 00:00:00.000000 bosch_alarm_mode2-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0       48 2023-05-21 02:31:10.469944 bosch_alarm_mode2-0.3.2/bosch_alarm_mode2/__init__.py
+-rw-r--r--   0        0        0     2330 2023-05-21 03:21:31.913252 bosch_alarm_mode2-0.3.2/bosch_alarm_mode2/connection.py
+-rw-r--r--   0        0        0     4220 2023-05-22 09:16:58.475238 bosch_alarm_mode2-0.3.2/bosch_alarm_mode2/const.py
+-rw-r--r--   0        0        0    17857 2023-05-22 22:49:25.036597 bosch_alarm_mode2-0.3.2/bosch_alarm_mode2/panel.py
+-rw-r--r--   0        0        0      262 2023-05-23 07:21:43.112117 bosch_alarm_mode2-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      355 1970-01-01 00:00:00.000000 bosch_alarm_mode2-0.3.2/PKG-INFO
```

### Comparing `bosch_alarm_mode2-0.3.1/bosch_alarm_mode2/connection.py` & `bosch_alarm_mode2-0.3.2/bosch_alarm_mode2/connection.py`

 * *Files identical despite different names*

### Comparing `bosch_alarm_mode2-0.3.1/bosch_alarm_mode2/const.py` & `bosch_alarm_mode2-0.3.2/bosch_alarm_mode2/const.py`

 * *Files identical despite different names*

### Comparing `bosch_alarm_mode2-0.3.1/bosch_alarm_mode2/panel.py` & `bosch_alarm_mode2-0.3.2/bosch_alarm_mode2/panel.py`

 * *Files identical despite different names*

