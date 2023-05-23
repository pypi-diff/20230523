# Comparing `tmp/nexus_databoard-0.0.1.tar.gz` & `tmp/nexus_databoard-0.0.2.tar.gz`

## Comparing `nexus_databoard-0.0.1.tar` & `nexus_databoard-0.0.2.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 nexus_databoard-0.0.1/.env.sample
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 nexus_databoard-0.0.1/Dockerfile
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 nexus_databoard-0.0.1/Makefile
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 nexus_databoard-0.0.1/docker-compose.yml
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 nexus_databoard-0.0.1/requirements.txt
--rwxr-xr-x   0        0        0       44 2020-02-02 00:00:00.000000 nexus_databoard-0.0.1/run
--rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 nexus_databoard-0.0.1/.github/workflows/release.yml
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 nexus_databoard-0.0.1/src/nexus_databoard/Home.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 nexus_databoard-0.0.1/src/nexus_databoard/.streamlit/config.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nexus_databoard-0.0.1/src/nexus_databoard/common/__init__.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 nexus_databoard-0.0.1/src/nexus_databoard/common/config.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 nexus_databoard-0.0.1/src/nexus_databoard/common/email.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 nexus_databoard-0.0.1/src/nexus_databoard/common/page_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nexus_databoard-0.0.1/src/nexus_databoard/components/__init__.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 nexus_databoard-0.0.1/src/nexus_databoard/components/download.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 nexus_databoard-0.0.1/src/nexus_databoard/components/table.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nexus_databoard-0.0.1/src/nexus_databoard/data/__init__.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 nexus_databoard-0.0.1/src/nexus_databoard/data/db.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 nexus_databoard-0.0.1/src/nexus_databoard/data/google_sheets.py
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 nexus_databoard-0.0.1/src/nexus_databoard/pages/01_Example-1.py
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 nexus_databoard-0.0.1/src/nexus_databoard/pages/02_Example-2.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 nexus_databoard-0.0.1/src/nexus_databoard/pages/03_Example-3.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 nexus_databoard-0.0.1/src/nexus_databoard/pages/04_Example-4.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 nexus_databoard-0.0.1/src/nexus_databoard/pages/05_Example-5.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nexus_databoard-0.0.1/src/nexus_databoard/pages/__init__.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 nexus_databoard-0.0.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 nexus_databoard-0.0.1/LICENSE
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 nexus_databoard-0.0.1/README.md
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 nexus_databoard-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 nexus_databoard-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 nexus_databoard-0.0.2/.env.sample
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 nexus_databoard-0.0.2/Dockerfile
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 nexus_databoard-0.0.2/Makefile
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 nexus_databoard-0.0.2/docker-compose.yml
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 nexus_databoard-0.0.2/requirements.txt
+-rwxr-xr-x   0        0        0       44 2020-02-02 00:00:00.000000 nexus_databoard-0.0.2/run
+-rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 nexus_databoard-0.0.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 nexus_databoard-0.0.2/src/nexus_databoard/Home.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nexus_databoard-0.0.2/src/nexus_databoard/__init__.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 nexus_databoard-0.0.2/src/nexus_databoard/.streamlit/config.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nexus_databoard-0.0.2/src/nexus_databoard/common/__init__.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 nexus_databoard-0.0.2/src/nexus_databoard/common/config.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 nexus_databoard-0.0.2/src/nexus_databoard/common/email.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 nexus_databoard-0.0.2/src/nexus_databoard/common/page_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nexus_databoard-0.0.2/src/nexus_databoard/components/__init__.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 nexus_databoard-0.0.2/src/nexus_databoard/components/download.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 nexus_databoard-0.0.2/src/nexus_databoard/components/table.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nexus_databoard-0.0.2/src/nexus_databoard/data/__init__.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 nexus_databoard-0.0.2/src/nexus_databoard/data/db.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 nexus_databoard-0.0.2/src/nexus_databoard/data/google_sheets.py
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 nexus_databoard-0.0.2/src/nexus_databoard/pages/01_Example-1.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 nexus_databoard-0.0.2/src/nexus_databoard/pages/02_Example-2.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 nexus_databoard-0.0.2/src/nexus_databoard/pages/03_Example-3.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 nexus_databoard-0.0.2/src/nexus_databoard/pages/04_Example-4.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 nexus_databoard-0.0.2/src/nexus_databoard/pages/05_Example-5.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nexus_databoard-0.0.2/src/nexus_databoard/pages/__init__.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 nexus_databoard-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 nexus_databoard-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 nexus_databoard-0.0.2/README.md
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 nexus_databoard-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 nexus_databoard-0.0.2/PKG-INFO
```

### Comparing `nexus_databoard-0.0.1/requirements.txt` & `nexus_databoard-0.0.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `nexus_databoard-0.0.1/.github/workflows/release.yml` & `nexus_databoard-0.0.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `nexus_databoard-0.0.1/src/nexus_databoard/.streamlit/config.toml` & `nexus_databoard-0.0.2/src/nexus_databoard/.streamlit/config.toml`

 * *Files identical despite different names*

### Comparing `nexus_databoard-0.0.1/src/nexus_databoard/common/config.py` & `nexus_databoard-0.0.2/src/nexus_databoard/common/config.py`

 * *Files identical despite different names*

### Comparing `nexus_databoard-0.0.1/src/nexus_databoard/common/email.py` & `nexus_databoard-0.0.2/src/nexus_databoard/common/email.py`

 * *Files identical despite different names*

### Comparing `nexus_databoard-0.0.1/src/nexus_databoard/data/db.py` & `nexus_databoard-0.0.2/src/nexus_databoard/data/db.py`

 * *Files identical despite different names*

### Comparing `nexus_databoard-0.0.1/src/nexus_databoard/pages/01_Example-1.py` & `nexus_databoard-0.0.2/src/nexus_databoard/pages/01_Example-1.py`

 * *Files identical despite different names*

### Comparing `nexus_databoard-0.0.1/src/nexus_databoard/pages/02_Example-2.py` & `nexus_databoard-0.0.2/src/nexus_databoard/pages/02_Example-2.py`

 * *Files identical despite different names*

### Comparing `nexus_databoard-0.0.1/src/nexus_databoard/pages/03_Example-3.py` & `nexus_databoard-0.0.2/src/nexus_databoard/pages/03_Example-3.py`

 * *Files identical despite different names*

### Comparing `nexus_databoard-0.0.1/src/nexus_databoard/pages/04_Example-4.py` & `nexus_databoard-0.0.2/src/nexus_databoard/pages/04_Example-4.py`

 * *Files identical despite different names*

### Comparing `nexus_databoard-0.0.1/src/nexus_databoard/pages/05_Example-5.py` & `nexus_databoard-0.0.2/src/nexus_databoard/pages/05_Example-5.py`

 * *Files identical despite different names*

### Comparing `nexus_databoard-0.0.1/LICENSE` & `nexus_databoard-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nexus_databoard-0.0.1/README.md` & `nexus_databoard-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nexus_databoard-0.0.1/pyproject.toml` & `nexus_databoard-0.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "nexus_databoard"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Jeremy Branham", email="jeremy@savantly.net" },
 ]
 description = "An oppinionated data science project template for the Nexus platform. An abstraction over Streamlit."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `nexus_databoard-0.0.1/PKG-INFO` & `nexus_databoard-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus_databoard
-Version: 0.0.1
+Version: 0.0.2
 Summary: An oppinionated data science project template for the Nexus platform. An abstraction over Streamlit.
 Project-URL: Homepage, https://github.com/savantly-net/nexus-databoard
 Project-URL: Bug Tracker, https://github.com/savantly-net/nexus-databoard/issues
 Author-email: Jeremy Branham <jeremy@savantly.net>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

