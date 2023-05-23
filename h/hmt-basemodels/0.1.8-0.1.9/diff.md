# Comparing `tmp/hmt-basemodels-0.1.8.tar.gz` & `tmp/hmt-basemodels-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hmt-basemodels-0.1.8.tar", last modified: Tue Jun 29 16:02:05 2021, max compression
+gzip compressed data, was "dist/hmt-basemodels-0.1.9.tar", last modified: Wed Jun 30 20:27:14 2021, max compression
```

## Comparing `hmt-basemodels-0.1.8.tar` & `hmt-basemodels-0.1.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-29 16:02:05.000000 hmt-basemodels-0.1.8/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-29 16:02:05.000000 hmt-basemodels-0.1.8/basemodels/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1717 2021-06-29 16:00:29.000000 hmt-basemodels-0.1.8/basemodels/via.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-29 16:02:05.000000 hmt-basemodels-0.1.8/basemodels/pydantic/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1664 2021-06-29 16:00:29.000000 hmt-basemodels-0.1.8/basemodels/pydantic/via.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-29 16:02:05.000000 hmt-basemodels-0.1.8/basemodels/pydantic/manifest/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-29 16:02:05.000000 hmt-basemodels-0.1.8/basemodels/pydantic/manifest/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1715 2021-06-29 16:00:29.000000 hmt-basemodels-0.1.8/basemodels/pydantic/manifest/data/taskdata.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      427 2021-06-29 16:00:29.000000 hmt-basemodels-0.1.8/basemodels/pydantic/manifest/data/preprocess.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       98 2021-06-29 16:00:29.000000 hmt-basemodels-0.1.8/basemodels/pydantic/manifest/data/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2425 2021-06-29 16:00:29.000000 hmt-basemodels-0.1.8/basemodels/pydantic/manifest/data/groundtruth.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2591 2021-06-29 16:00:29.000000 hmt-basemodels-0.1.8/basemodels/pydantic/manifest/restricted_audience.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14546 2021-06-29 16:00:29.000000 hmt-basemodels-0.1.8/basemodels/pydantic/manifest/manifest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      105 2021-06-29 16:00:29.000000 hmt-basemodels-0.1.8/basemodels/pydantic/manifest/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      275 2021-06-29 16:00:29.000000 hmt-basemodels-0.1.8/basemodels/pydantic/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-29 16:02:05.000000 hmt-basemodels-0.1.8/basemodels/manifest/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-29 16:02:05.000000 hmt-basemodels-0.1.8/basemodels/manifest/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1324 2021-06-29 16:00:29.000000 hmt-basemodels-0.1.8/basemodels/manifest/data/taskdata.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      461 2021-06-29 16:00:29.000000 hmt-basemodels-0.1.8/basemodels/manifest/data/preprocess.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       98 2021-06-29 16:00:29.000000 hmt-basemodels-0.1.8/basemodels/manifest/data/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2439 2021-06-29 16:00:29.000000 hmt-basemodels-0.1.8/basemodels/manifest/data/groundtruth.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3327 2021-06-29 16:00:29.000000 hmt-basemodels-0.1.8/basemodels/manifest/restricted_audience.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11986 2021-06-29 16:00:29.000000 hmt-basemodels-0.1.8/basemodels/manifest/manifest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       24 2021-06-29 16:00:29.000000 hmt-basemodels-0.1.8/basemodels/manifest/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      217 2021-06-29 16:00:29.000000 hmt-basemodels-0.1.8/basemodels/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       18 2021-06-29 16:00:29.000000 hmt-basemodels-0.1.8/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      421 2021-06-29 16:02:05.000000 hmt-basemodels-0.1.8/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2580 2021-06-29 16:00:29.000000 hmt-basemodels-0.1.8/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-29 16:02:05.000000 hmt-basemodels-0.1.8/hmt_basemodels.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      421 2021-06-29 16:02:04.000000 hmt-basemodels-0.1.8/hmt_basemodels.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-06-29 16:02:04.000000 hmt-basemodels-0.1.8/hmt_basemodels.egg-info/zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-06-29 16:02:04.000000 hmt-basemodels-0.1.8/hmt_basemodels.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       11 2021-06-29 16:02:04.000000 hmt-basemodels-0.1.8/hmt_basemodels.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      958 2021-06-29 16:02:04.000000 hmt-basemodels-0.1.8/hmt_basemodels.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       73 2021-06-29 16:02:04.000000 hmt-basemodels-0.1.8/hmt_basemodels.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-06-29 16:02:05.000000 hmt-basemodels-0.1.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1071 2021-06-29 16:00:29.000000 hmt-basemodels-0.1.8/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      490 2021-06-29 16:00:29.000000 hmt-basemodels-0.1.8/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)      626 2021-06-29 16:00:29.000000 hmt-basemodels-0.1.8/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-30 20:27:14.000000 hmt-basemodels-0.1.9/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-30 20:27:14.000000 hmt-basemodels-0.1.9/basemodels/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1717 2021-06-30 20:25:37.000000 hmt-basemodels-0.1.9/basemodels/via.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-30 20:27:14.000000 hmt-basemodels-0.1.9/basemodels/pydantic/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1664 2021-06-30 20:25:37.000000 hmt-basemodels-0.1.9/basemodels/pydantic/via.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-30 20:27:14.000000 hmt-basemodels-0.1.9/basemodels/pydantic/manifest/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-30 20:27:14.000000 hmt-basemodels-0.1.9/basemodels/pydantic/manifest/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1715 2021-06-30 20:25:37.000000 hmt-basemodels-0.1.9/basemodels/pydantic/manifest/data/taskdata.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      427 2021-06-30 20:25:37.000000 hmt-basemodels-0.1.9/basemodels/pydantic/manifest/data/preprocess.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       98 2021-06-30 20:25:37.000000 hmt-basemodels-0.1.9/basemodels/pydantic/manifest/data/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2425 2021-06-30 20:25:37.000000 hmt-basemodels-0.1.9/basemodels/pydantic/manifest/data/groundtruth.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2591 2021-06-30 20:25:37.000000 hmt-basemodels-0.1.9/basemodels/pydantic/manifest/restricted_audience.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14620 2021-06-30 20:25:37.000000 hmt-basemodels-0.1.9/basemodels/pydantic/manifest/manifest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      105 2021-06-30 20:25:37.000000 hmt-basemodels-0.1.9/basemodels/pydantic/manifest/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      275 2021-06-30 20:25:37.000000 hmt-basemodels-0.1.9/basemodels/pydantic/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-30 20:27:14.000000 hmt-basemodels-0.1.9/basemodels/manifest/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-30 20:27:14.000000 hmt-basemodels-0.1.9/basemodels/manifest/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1324 2021-06-30 20:25:37.000000 hmt-basemodels-0.1.9/basemodels/manifest/data/taskdata.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      461 2021-06-30 20:25:37.000000 hmt-basemodels-0.1.9/basemodels/manifest/data/preprocess.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       98 2021-06-30 20:25:37.000000 hmt-basemodels-0.1.9/basemodels/manifest/data/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2439 2021-06-30 20:25:37.000000 hmt-basemodels-0.1.9/basemodels/manifest/data/groundtruth.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3327 2021-06-30 20:25:37.000000 hmt-basemodels-0.1.9/basemodels/manifest/restricted_audience.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12087 2021-06-30 20:25:37.000000 hmt-basemodels-0.1.9/basemodels/manifest/manifest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       24 2021-06-30 20:25:37.000000 hmt-basemodels-0.1.9/basemodels/manifest/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      217 2021-06-30 20:25:37.000000 hmt-basemodels-0.1.9/basemodels/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       18 2021-06-30 20:25:37.000000 hmt-basemodels-0.1.9/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)      421 2021-06-30 20:27:14.000000 hmt-basemodels-0.1.9/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2580 2021-06-30 20:25:37.000000 hmt-basemodels-0.1.9/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-30 20:27:14.000000 hmt-basemodels-0.1.9/hmt_basemodels.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      421 2021-06-30 20:27:14.000000 hmt-basemodels-0.1.9/hmt_basemodels.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-06-30 20:27:14.000000 hmt-basemodels-0.1.9/hmt_basemodels.egg-info/zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-06-30 20:27:14.000000 hmt-basemodels-0.1.9/hmt_basemodels.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       11 2021-06-30 20:27:14.000000 hmt-basemodels-0.1.9/hmt_basemodels.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      958 2021-06-30 20:27:14.000000 hmt-basemodels-0.1.9/hmt_basemodels.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       73 2021-06-30 20:27:14.000000 hmt-basemodels-0.1.9/hmt_basemodels.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-06-30 20:27:14.000000 hmt-basemodels-0.1.9/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1071 2021-06-30 20:25:37.000000 hmt-basemodels-0.1.9/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      490 2021-06-30 20:25:37.000000 hmt-basemodels-0.1.9/pyproject.toml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      626 2021-06-30 20:25:37.000000 hmt-basemodels-0.1.9/setup.py
```

### Comparing `hmt-basemodels-0.1.8/basemodels/via.py` & `hmt-basemodels-0.1.9/basemodels/via.py`

 * *Files identical despite different names*

### Comparing `hmt-basemodels-0.1.8/basemodels/pydantic/via.py` & `hmt-basemodels-0.1.9/basemodels/pydantic/via.py`

 * *Files identical despite different names*

### Comparing `hmt-basemodels-0.1.8/basemodels/pydantic/manifest/data/taskdata.py` & `hmt-basemodels-0.1.9/basemodels/pydantic/manifest/data/taskdata.py`

 * *Files identical despite different names*

### Comparing `hmt-basemodels-0.1.8/basemodels/pydantic/manifest/data/groundtruth.py` & `hmt-basemodels-0.1.9/basemodels/pydantic/manifest/data/groundtruth.py`

 * *Files identical despite different names*

### Comparing `hmt-basemodels-0.1.8/basemodels/pydantic/manifest/restricted_audience.py` & `hmt-basemodels-0.1.9/basemodels/pydantic/manifest/restricted_audience.py`

 * *Files identical despite different names*

### Comparing `hmt-basemodels-0.1.8/basemodels/pydantic/manifest/manifest.py` & `hmt-basemodels-0.1.9/basemodels/pydantic/manifest/manifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,14 +257,17 @@
 
     # Configuration id
     confcalc_configuration_id: Optional[str]
     restricted_audience: Optional[RestrictedAudience] = {}
 
     webhook: Optional[Webhook]
 
+    rejected_uri: Optional[AnyHttpUrl]
+    rejected_count: Optional[int]
+
     ##### Validators
 
     @validator("requester_min_repeats")
     def validate_min_repeats(cls, v, values):
         """ min repeats are required to be at least 4 if ilmc """
         if values["request_type"] == "image_label_multiple_choice":
             return max(v, 4)
```

### Comparing `hmt-basemodels-0.1.8/basemodels/manifest/data/taskdata.py` & `hmt-basemodels-0.1.9/basemodels/manifest/data/taskdata.py`

 * *Files identical despite different names*

### Comparing `hmt-basemodels-0.1.8/basemodels/manifest/data/groundtruth.py` & `hmt-basemodels-0.1.9/basemodels/manifest/data/groundtruth.py`

 * *Files identical despite different names*

### Comparing `hmt-basemodels-0.1.8/basemodels/manifest/restricted_audience.py` & `hmt-basemodels-0.1.9/basemodels/manifest/restricted_audience.py`

 * *Files identical despite different names*

### Comparing `hmt-basemodels-0.1.8/basemodels/manifest/manifest.py` & `hmt-basemodels-0.1.9/basemodels/manifest/manifest.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,14 +145,15 @@
 
     request_config = ModelType(RequestConfig, required=False)
 
     # Groundtruth data is stored as a URL or optionally as an inlined json-serialized stringtype
     groundtruth_uri = URLType(required=False)
     groundtruth = StringType(required=False)
 
+
     def validate_groundtruth(self, data, value):
         if data.get('groundtruth_uri') and data.get('groundtruth'):
             raise ValidationError("Specify only groundtruth_uri or groundtruth, not both.")
         return value
 
     # Configuration id -- XXX LEGACY
     confcalc_configuration_id = StringType(required=False)
@@ -233,14 +234,17 @@
     # If taskdata is separately stored
     taskdata_uri = URLType()
 
     # Groundtruth data is stored as a URL or optionally as an inlined json-serialized stringtype
     groundtruth_uri = URLType(required=False)
     groundtruth = StringType(required=False)
 
+    rejected_uri = URLType(required=False)
+    rejected_count = IntType(default=0, required=False)
+
     def validate_groundtruth(self, data, value):
         if data.get('groundtruth_uri') and data.get('groundtruth'):
             raise ValidationError("Specify only groundtruth_uri or groundtruth, not both.")
         return value
 
     # internal config options for param tests etc.
     internal_config = ModelType(InternalConfig, required=False)
```

### Comparing `hmt-basemodels-0.1.8/README.md` & `hmt-basemodels-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `hmt-basemodels-0.1.8/hmt_basemodels.egg-info/SOURCES.txt` & `hmt-basemodels-0.1.9/hmt_basemodels.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hmt-basemodels-0.1.8/LICENSE` & `hmt-basemodels-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hmt-basemodels-0.1.8/setup.py` & `hmt-basemodels-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="hmt-basemodels",
-    version="0.1.8",
+    version="0.1.9",
     author="HUMAN Protocol",
     description="Common data models shared by various components of the Human Protocol stack",
     url="https://github.com/hCaptcha/hmt-basemodels",
     include_package_data=True,
     zip_safe=True,
     classifiers=[
         "Intended Audience :: Developers", "Operating System :: OS Independent",
```

