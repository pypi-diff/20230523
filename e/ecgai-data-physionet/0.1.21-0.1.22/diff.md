# Comparing `tmp/ecgai_data_physionet-0.1.21.tar.gz` & `tmp/ecgai_data_physionet-0.1.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecgai_data_physionet-0.1.21.tar", max compression
+gzip compressed data, was "ecgai_data_physionet-0.1.22.tar", max compression
```

## Comparing `ecgai_data_physionet-0.1.21.tar` & `ecgai_data_physionet-0.1.22.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1105 2023-05-23 12:56:48.380802 ecgai_data_physionet-0.1.21/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-23 12:56:48.380802 ecgai_data_physionet-0.1.21/src/ecgai_data_physionet/__init__.py
--rw-r--r--   0        0        0  6602796 2023-05-23 12:56:48.412801 ecgai_data_physionet-0.1.21/src/ecgai_data_physionet/data/ptbxl_database.csv
--rw-r--r--   0        0        0     9794 2023-05-23 12:56:48.412801 ecgai_data_physionet-0.1.21/src/ecgai_data_physionet/data/scp_statements.csv
--rw-r--r--   0        0        0     1656 2023-05-23 12:56:48.412801 ecgai_data_physionet-0.1.21/src/ecgai_data_physionet/exceptions.py
--rw-r--r--   0        0        0     4193 2023-05-23 12:56:48.412801 ecgai_data_physionet-0.1.21/src/ecgai_data_physionet/file_loader.py
--rw-r--r--   0        0        0      418 2023-05-23 12:56:48.412801 ecgai_data_physionet-0.1.21/src/ecgai_data_physionet/models/diagnostic_code.py
--rw-r--r--   0        0        0     1427 2023-05-23 12:56:48.412801 ecgai_data_physionet-0.1.21/src/ecgai_data_physionet/models/ecg.py
--rw-r--r--   0        0        0      551 2023-05-23 12:56:48.412801 ecgai_data_physionet-0.1.21/src/ecgai_data_physionet/models/ecg_lead.py
--rw-r--r--   0        0        0      499 2023-05-23 12:56:48.412801 ecgai_data_physionet-0.1.21/src/ecgai_data_physionet/models/model_base.py
--rw-r--r--   0        0        0     3407 2023-05-23 12:56:48.412801 ecgai_data_physionet-0.1.21/src/ecgai_data_physionet/physionet.py
--rw-r--r--   0        0        0    10543 2023-05-23 12:56:48.412801 ecgai_data_physionet-0.1.21/src/ecgai_data_physionet/ptbxl.py
--rw-r--r--   0        0        0      550 1970-01-01 00:00:00.000000 ecgai_data_physionet-0.1.21/PKG-INFO
+-rw-r--r--   0        0        0     1104 2023-05-23 19:24:33.918318 ecgai_data_physionet-0.1.22/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-23 19:24:33.918318 ecgai_data_physionet-0.1.22/src/ecgai_data_physionet/__init__.py
+-rw-r--r--   0        0        0  6602796 2023-05-23 19:24:33.946319 ecgai_data_physionet-0.1.22/src/ecgai_data_physionet/data/ptbxl_database.csv
+-rw-r--r--   0        0        0     9794 2023-05-23 19:24:33.946319 ecgai_data_physionet-0.1.22/src/ecgai_data_physionet/data/scp_statements.csv
+-rw-r--r--   0        0        0     1656 2023-05-23 19:24:33.946319 ecgai_data_physionet-0.1.22/src/ecgai_data_physionet/exceptions.py
+-rw-r--r--   0        0        0     4193 2023-05-23 19:24:33.946319 ecgai_data_physionet-0.1.22/src/ecgai_data_physionet/file_loader.py
+-rw-r--r--   0        0        0      418 2023-05-23 19:24:33.946319 ecgai_data_physionet-0.1.22/src/ecgai_data_physionet/models/diagnostic_code.py
+-rw-r--r--   0        0        0     1427 2023-05-23 19:24:33.946319 ecgai_data_physionet-0.1.22/src/ecgai_data_physionet/models/ecg.py
+-rw-r--r--   0        0        0      551 2023-05-23 19:24:33.946319 ecgai_data_physionet-0.1.22/src/ecgai_data_physionet/models/ecg_lead.py
+-rw-r--r--   0        0        0      499 2023-05-23 19:24:33.946319 ecgai_data_physionet-0.1.22/src/ecgai_data_physionet/models/model_base.py
+-rw-r--r--   0        0        0     3407 2023-05-23 19:24:33.946319 ecgai_data_physionet-0.1.22/src/ecgai_data_physionet/physionet.py
+-rw-r--r--   0        0        0    10543 2023-05-23 19:24:33.946319 ecgai_data_physionet-0.1.22/src/ecgai_data_physionet/ptbxl.py
+-rw-r--r--   0        0        0      599 1970-01-01 00:00:00.000000 ecgai_data_physionet-0.1.22/PKG-INFO
```

### Comparing `ecgai_data_physionet-0.1.21/pyproject.toml` & `ecgai_data_physionet-0.1.22/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "ecgai-data-physionet"
-version = "0.1.21"
+version = "0.1.22"
 description = ""
 authors = ["RobC <rob.clapham@gmail.com>"]
 
 [tool.poetry.dependencies]
 #TODO change poetry version to <4.0, currently required by scipy
-python = "^3.10,<3.12"
+python = "^3.9,<3.12"
 numpy = "^1.23.2"
 aenum = "^3.1.11"
 pydantic = "^1.10.1"
 wfdb = "^4.0.0"
 pytest-asyncio = "^0.19.0"
 seqlog = "^0.3.20"
```

### Comparing `ecgai_data_physionet-0.1.21/src/ecgai_data_physionet/data/ptbxl_database.csv` & `ecgai_data_physionet-0.1.22/src/ecgai_data_physionet/data/ptbxl_database.csv`

 * *Files identical despite different names*

### Comparing `ecgai_data_physionet-0.1.21/src/ecgai_data_physionet/data/scp_statements.csv` & `ecgai_data_physionet-0.1.22/src/ecgai_data_physionet/data/scp_statements.csv`

 * *Files identical despite different names*

### Comparing `ecgai_data_physionet-0.1.21/src/ecgai_data_physionet/exceptions.py` & `ecgai_data_physionet-0.1.22/src/ecgai_data_physionet/exceptions.py`

 * *Files identical despite different names*

### Comparing `ecgai_data_physionet-0.1.21/src/ecgai_data_physionet/file_loader.py` & `ecgai_data_physionet-0.1.22/src/ecgai_data_physionet/file_loader.py`

 * *Files identical despite different names*

### Comparing `ecgai_data_physionet-0.1.21/src/ecgai_data_physionet/models/ecg.py` & `ecgai_data_physionet-0.1.22/src/ecgai_data_physionet/models/ecg.py`

 * *Files identical despite different names*

### Comparing `ecgai_data_physionet-0.1.21/src/ecgai_data_physionet/models/ecg_lead.py` & `ecgai_data_physionet-0.1.22/src/ecgai_data_physionet/models/ecg_lead.py`

 * *Files identical despite different names*

### Comparing `ecgai_data_physionet-0.1.21/src/ecgai_data_physionet/physionet.py` & `ecgai_data_physionet-0.1.22/src/ecgai_data_physionet/physionet.py`

 * *Files identical despite different names*

### Comparing `ecgai_data_physionet-0.1.21/src/ecgai_data_physionet/ptbxl.py` & `ecgai_data_physionet-0.1.22/src/ecgai_data_physionet/ptbxl.py`

 * *Files identical despite different names*

### Comparing `ecgai_data_physionet-0.1.21/PKG-INFO` & `ecgai_data_physionet-0.1.22/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: ecgai-data-physionet
-Version: 0.1.21
+Version: 0.1.22
 Summary: 
 Author: RobC
 Author-email: rob.clapham@gmail.com
-Requires-Python: >=3.10,<3.12
+Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aenum (>=3.1.11,<4.0.0)
 Requires-Dist: numpy (>=1.23.2,<2.0.0)
 Requires-Dist: pydantic (>=1.10.1,<2.0.0)
 Requires-Dist: pytest-asyncio (>=0.19.0,<0.20.0)
 Requires-Dist: seqlog (>=0.3.20,<0.4.0)
```

