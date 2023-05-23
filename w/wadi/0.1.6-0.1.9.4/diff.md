# Comparing `tmp/wadi-0.1.6.tar.gz` & `tmp/wadi-0.1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wadi-0.1.6.tar", last modified: Tue May 23 07:38:18 2023, max compression
+gzip compressed data, was "wadi-0.1.9.4.tar", last modified: Tue May 23 09:59:23 2023, max compression
```

## Comparing `wadi-0.1.6.tar` & `wadi-0.1.9.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:38:18.447099 wadi-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-23 07:38:00.000000 wadi-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-23 07:38:00.000000 wadi-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-23 07:38:18.447099 wadi-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-23 07:38:00.000000 wadi-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 07:38:18.447099 wadi-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-23 07:38:00.000000 wadi-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:38:18.443099 wadi-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-23 07:38:00.000000 wadi-0.1.6/tests/test_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:38:18.443099 wadi-0.1.6/wadi/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-23 07:38:00.000000 wadi-0.1.6/wadi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-05-23 07:38:00.000000 wadi-0.1.6/wadi/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-05-23 07:38:00.000000 wadi-0.1.6/wadi/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7617 2023-05-23 07:38:00.000000 wadi-0.1.6/wadi/dataobject.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-23 07:38:00.000000 wadi-0.1.6/wadi/documentation_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13556 2023-05-23 07:38:00.000000 wadi-0.1.6/wadi/filereader.py
--rw-r--r--   0 runner    (1001) docker     (123)    17687 2023-05-23 07:38:00.000000 wadi-0.1.6/wadi/harmonizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9667 2023-05-23 07:38:00.000000 wadi-0.1.6/wadi/infotable.py
--rw-r--r--   0 runner    (1001) docker     (123)    29684 2023-05-23 07:38:00.000000 wadi-0.1.6/wadi/mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:38:18.447099 wadi-0.1.6/wadi/mapping_data/
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-05-23 07:38:00.000000 wadi-0.1.6/wadi/mapping_data/atoms.csv
--rw-r--r--   0 runner    (1001) docker     (123)   838881 2023-05-23 07:38:00.000000 wadi-0.1.6/wadi/mapping_data/default_feature_map.json
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-23 07:38:00.000000 wadi-0.1.6/wadi/mapping_data/ions.csv
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-23 07:38:00.000000 wadi-0.1.6/wadi/mapping_data/other_than_concentrations.csv
--rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-05-23 07:38:00.000000 wadi-0.1.6/wadi/unitconverter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9323 2023-05-23 07:38:00.000000 wadi-0.1.6/wadi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:38:18.443099 wadi-0.1.6/wadi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-23 07:38:18.000000 wadi-0.1.6/wadi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-23 07:38:18.000000 wadi-0.1.6/wadi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 07:38:18.000000 wadi-0.1.6/wadi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-23 07:38:18.000000 wadi-0.1.6/wadi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-23 07:38:18.000000 wadi-0.1.6/wadi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:59:23.399899 wadi-0.1.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-23 09:59:09.000000 wadi-0.1.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-23 09:59:09.000000 wadi-0.1.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-23 09:59:23.399899 wadi-0.1.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-23 09:59:09.000000 wadi-0.1.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 09:59:23.399899 wadi-0.1.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-23 09:59:09.000000 wadi-0.1.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:59:23.391899 wadi-0.1.9.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-23 09:59:09.000000 wadi-0.1.9.4/tests/test_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:59:23.395899 wadi-0.1.9.4/wadi/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-23 09:59:09.000000 wadi-0.1.9.4/wadi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-05-23 09:59:09.000000 wadi-0.1.9.4/wadi/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-05-23 09:59:09.000000 wadi-0.1.9.4/wadi/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7617 2023-05-23 09:59:09.000000 wadi-0.1.9.4/wadi/dataobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-23 09:59:09.000000 wadi-0.1.9.4/wadi/documentation_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13556 2023-05-23 09:59:09.000000 wadi-0.1.9.4/wadi/filereader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17687 2023-05-23 09:59:09.000000 wadi-0.1.9.4/wadi/harmonizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9667 2023-05-23 09:59:09.000000 wadi-0.1.9.4/wadi/infotable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29684 2023-05-23 09:59:09.000000 wadi-0.1.9.4/wadi/mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:59:23.399899 wadi-0.1.9.4/wadi/mapping_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-05-23 09:59:09.000000 wadi-0.1.9.4/wadi/mapping_data/atoms.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   838881 2023-05-23 09:59:09.000000 wadi-0.1.9.4/wadi/mapping_data/default_feature_map.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-23 09:59:09.000000 wadi-0.1.9.4/wadi/mapping_data/ions.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-23 09:59:09.000000 wadi-0.1.9.4/wadi/mapping_data/other_than_concentrations.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-05-23 09:59:09.000000 wadi-0.1.9.4/wadi/unitconverter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9323 2023-05-23 09:59:09.000000 wadi-0.1.9.4/wadi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:59:23.395899 wadi-0.1.9.4/wadi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-23 09:59:23.000000 wadi-0.1.9.4/wadi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-23 09:59:23.000000 wadi-0.1.9.4/wadi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 09:59:23.000000 wadi-0.1.9.4/wadi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-23 09:59:23.000000 wadi-0.1.9.4/wadi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-23 09:59:23.000000 wadi-0.1.9.4/wadi.egg-info/top_level.txt
```

### Comparing `wadi-0.1.6/LICENSE` & `wadi-0.1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wadi-0.1.6/PKG-INFO` & `wadi-0.1.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wadi
-Version: 0.1.6
+Version: 0.1.9.4
 Summary: Generic importer for water quality data of the (Dutch) water laboratory
 Home-page: https://github.com/KWR-Water/wadi
 Author: KWR Water Research Institute
 Author-email: martin.korevaar@kwrwater.nl, martin.van.der.schans@kwrwater.nl
 License: MIT
 Project-URL: Source, https://github.com/KWR-Water/wadi
 Project-URL: Documentation, http://wadi.readthedocs.io/en/latest/
```

### Comparing `wadi-0.1.6/README.md` & `wadi-0.1.9.4/README.md`

 * *Files identical despite different names*

### Comparing `wadi-0.1.6/setup.py` & `wadi-0.1.9.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def read(fname):
     with open(os.path.join(os.path.dirname(__file__), fname)) as f:
         return f.read()
 
 setup(
     name='wadi',
-    version='v0.1.6',
+    version='v0.1.9.4',
     packages=find_packages(exclude=['tests*']),
     data_files=glob.glob('mapping_data/**'),
     license='MIT',
     description='Generic importer for water quality data of the (Dutch) water laboratory',
     long_description=read('README.md'),
     long_description_content_type="text/markdown",
     classifiers=[
```

### Comparing `wadi-0.1.6/wadi/api_utils.py` & `wadi-0.1.9.4/wadi/api_utils.py`

 * *Files identical despite different names*

### Comparing `wadi-0.1.6/wadi/base.py` & `wadi-0.1.9.4/wadi/base.py`

 * *Files identical despite different names*

### Comparing `wadi-0.1.6/wadi/dataobject.py` & `wadi-0.1.9.4/wadi/dataobject.py`

 * *Files identical despite different names*

### Comparing `wadi-0.1.6/wadi/documentation_helpers.py` & `wadi-0.1.9.4/wadi/documentation_helpers.py`

 * *Files identical despite different names*

### Comparing `wadi-0.1.6/wadi/filereader.py` & `wadi-0.1.9.4/wadi/filereader.py`

 * *Files identical despite different names*

### Comparing `wadi-0.1.6/wadi/harmonizer.py` & `wadi-0.1.9.4/wadi/harmonizer.py`

 * *Files identical despite different names*

### Comparing `wadi-0.1.6/wadi/infotable.py` & `wadi-0.1.9.4/wadi/infotable.py`

 * *Files identical despite different names*

### Comparing `wadi-0.1.6/wadi/mapper.py` & `wadi-0.1.9.4/wadi/mapper.py`

 * *Files identical despite different names*

### Comparing `wadi-0.1.6/wadi/mapping_data/atoms.csv` & `wadi-0.1.9.4/wadi/mapping_data/atoms.csv`

 * *Files identical despite different names*

### Comparing `wadi-0.1.6/wadi/mapping_data/default_feature_map.json` & `wadi-0.1.9.4/wadi/mapping_data/default_feature_map.json`

 * *Files identical despite different names*

### Comparing `wadi-0.1.6/wadi/mapping_data/ions.csv` & `wadi-0.1.9.4/wadi/mapping_data/ions.csv`

 * *Files identical despite different names*

### Comparing `wadi-0.1.6/wadi/unitconverter.py` & `wadi-0.1.9.4/wadi/unitconverter.py`

 * *Files identical despite different names*

### Comparing `wadi-0.1.6/wadi/utils.py` & `wadi-0.1.9.4/wadi/utils.py`

 * *Files identical despite different names*

### Comparing `wadi-0.1.6/wadi.egg-info/PKG-INFO` & `wadi-0.1.9.4/wadi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wadi
-Version: 0.1.6
+Version: 0.1.9.4
 Summary: Generic importer for water quality data of the (Dutch) water laboratory
 Home-page: https://github.com/KWR-Water/wadi
 Author: KWR Water Research Institute
 Author-email: martin.korevaar@kwrwater.nl, martin.van.der.schans@kwrwater.nl
 License: MIT
 Project-URL: Source, https://github.com/KWR-Water/wadi
 Project-URL: Documentation, http://wadi.readthedocs.io/en/latest/
```

### Comparing `wadi-0.1.6/wadi.egg-info/SOURCES.txt` & `wadi-0.1.9.4/wadi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

