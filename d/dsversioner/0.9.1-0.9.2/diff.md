# Comparing `tmp/dsversioner-0.9.1.tar.gz` & `tmp/dsversioner-0.9.2.tar.gz`

## Comparing `dsversioner-0.9.1.tar` & `dsversioner-0.9.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 dsversioner-0.9.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 dsversioner-0.9.1/SECURITY.md
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 dsversioner-0.9.1/docs/developer.md
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 dsversioner-0.9.1/docs/index.md
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 dsversioner-0.9.1/src/dsversioner/Dataset.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 dsversioner-0.9.1/src/dsversioner/DatasetMetadata.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 dsversioner-0.9.1/src/dsversioner/DatasetRecordData.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 dsversioner-0.9.1/src/dsversioner/DatasetVersion.py
--rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 dsversioner-0.9.1/src/dsversioner/Exceptions.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 dsversioner-0.9.1/src/dsversioner/FileSystemStorage.py
--rw-r--r--   0        0        0     6554 2020-02-02 00:00:00.000000 dsversioner-0.9.1/src/dsversioner/ObjectDataset.py
--rw-r--r--   0        0        0    20123 2020-02-02 00:00:00.000000 dsversioner-0.9.1/src/dsversioner/ObjectDatasetFileSystemStorage.py
--rw-r--r--   0        0        0     5516 2020-02-02 00:00:00.000000 dsversioner-0.9.1/src/dsversioner/ObjectDatasetMetadata.py
--rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 dsversioner-0.9.1/src/dsversioner/ObjectDatasetRecordData.py
--rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 dsversioner-0.9.1/src/dsversioner/ObjectDatasetStorage.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 dsversioner-0.9.1/src/dsversioner/ObjectDatasetVersion.py
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 dsversioner-0.9.1/src/dsversioner/Serializable.py
--rw-r--r--   0        0        0     5564 2020-02-02 00:00:00.000000 dsversioner-0.9.1/src/dsversioner/Storage.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 dsversioner-0.9.1/src/dsversioner/__init__.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 dsversioner-0.9.1/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 dsversioner-0.9.1/LICENSE
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 dsversioner-0.9.1/README.md
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 dsversioner-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 dsversioner-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 dsversioner-0.9.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 dsversioner-0.9.2/SECURITY.md
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 dsversioner-0.9.2/docs/developer.md
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 dsversioner-0.9.2/docs/index.md
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 dsversioner-0.9.2/src/dsversioner/Dataset.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 dsversioner-0.9.2/src/dsversioner/DatasetMetadata.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 dsversioner-0.9.2/src/dsversioner/DatasetRecordData.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 dsversioner-0.9.2/src/dsversioner/DatasetVersion.py
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 dsversioner-0.9.2/src/dsversioner/Exceptions.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 dsversioner-0.9.2/src/dsversioner/FileSystemStorage.py
+-rw-r--r--   0        0        0     6554 2020-02-02 00:00:00.000000 dsversioner-0.9.2/src/dsversioner/ObjectDataset.py
+-rw-r--r--   0        0        0    20123 2020-02-02 00:00:00.000000 dsversioner-0.9.2/src/dsversioner/ObjectDatasetFileSystemStorage.py
+-rw-r--r--   0        0        0     5516 2020-02-02 00:00:00.000000 dsversioner-0.9.2/src/dsversioner/ObjectDatasetMetadata.py
+-rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 dsversioner-0.9.2/src/dsversioner/ObjectDatasetRecordData.py
+-rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 dsversioner-0.9.2/src/dsversioner/ObjectDatasetStorage.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 dsversioner-0.9.2/src/dsversioner/ObjectDatasetVersion.py
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 dsversioner-0.9.2/src/dsversioner/Serializable.py
+-rw-r--r--   0        0        0     5564 2020-02-02 00:00:00.000000 dsversioner-0.9.2/src/dsversioner/Storage.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 dsversioner-0.9.2/src/dsversioner/__init__.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 dsversioner-0.9.2/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 dsversioner-0.9.2/LICENSE
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 dsversioner-0.9.2/README.md
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 dsversioner-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 dsversioner-0.9.2/PKG-INFO
```

### Comparing `dsversioner-0.9.1/SECURITY.md` & `dsversioner-0.9.2/SECURITY.md`

 * *Files identical despite different names*

### Comparing `dsversioner-0.9.1/docs/developer.md` & `dsversioner-0.9.2/docs/developer.md`

 * *Files identical despite different names*

### Comparing `dsversioner-0.9.1/src/dsversioner/Dataset.py` & `dsversioner-0.9.2/src/dsversioner/Dataset.py`

 * *Files identical despite different names*

### Comparing `dsversioner-0.9.1/src/dsversioner/DatasetMetadata.py` & `dsversioner-0.9.2/src/dsversioner/DatasetMetadata.py`

 * *Files identical despite different names*

### Comparing `dsversioner-0.9.1/src/dsversioner/DatasetVersion.py` & `dsversioner-0.9.2/src/dsversioner/DatasetVersion.py`

 * *Files identical despite different names*

### Comparing `dsversioner-0.9.1/src/dsversioner/Exceptions.py` & `dsversioner-0.9.2/src/dsversioner/Exceptions.py`

 * *Files identical despite different names*

### Comparing `dsversioner-0.9.1/src/dsversioner/ObjectDataset.py` & `dsversioner-0.9.2/src/dsversioner/ObjectDataset.py`

 * *Files identical despite different names*

### Comparing `dsversioner-0.9.1/src/dsversioner/ObjectDatasetFileSystemStorage.py` & `dsversioner-0.9.2/src/dsversioner/ObjectDatasetFileSystemStorage.py`

 * *Files identical despite different names*

### Comparing `dsversioner-0.9.1/src/dsversioner/ObjectDatasetMetadata.py` & `dsversioner-0.9.2/src/dsversioner/ObjectDatasetMetadata.py`

 * *Files identical despite different names*

### Comparing `dsversioner-0.9.1/src/dsversioner/ObjectDatasetRecordData.py` & `dsversioner-0.9.2/src/dsversioner/ObjectDatasetRecordData.py`

 * *Files identical despite different names*

### Comparing `dsversioner-0.9.1/src/dsversioner/ObjectDatasetStorage.py` & `dsversioner-0.9.2/src/dsversioner/ObjectDatasetStorage.py`

 * *Files identical despite different names*

### Comparing `dsversioner-0.9.1/src/dsversioner/ObjectDatasetVersion.py` & `dsversioner-0.9.2/src/dsversioner/ObjectDatasetVersion.py`

 * *Files identical despite different names*

### Comparing `dsversioner-0.9.1/src/dsversioner/Serializable.py` & `dsversioner-0.9.2/src/dsversioner/Serializable.py`

 * *Files identical despite different names*

### Comparing `dsversioner-0.9.1/src/dsversioner/Storage.py` & `dsversioner-0.9.2/src/dsversioner/Storage.py`

 * *Files identical despite different names*

### Comparing `dsversioner-0.9.1/src/dsversioner/__init__.py` & `dsversioner-0.9.2/src/dsversioner/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 This module...
 """
 
-from .Exceptions import *
-from .ObjectDataset import ObjectDataset
-from .ObjectDatasetFileSystemStorage import FileSystemObjectDatasetVersionStorage, \
+from dsversioner.Exceptions import *
+from dsversioner.ObjectDataset import ObjectDataset
+from dsversioner.ObjectDatasetFileSystemStorage import FileSystemObjectDatasetVersionStorage, \
     FileSystemObjectDatasetMetadataStorage, FileSystemObjectDatasetRecordStorage, FileSystemObjectDatasetObjectStorage
-from .ObjectDatasetMetadata import ObjectDatasetMetadata
-from .ObjectDatasetRecordData import PandasObjectDatasetRecordData
-from .ObjectDatasetVersion import ObjectDatasetVersion
-from .Storage import RecordStorageFormats
+from dsversioner.ObjectDatasetMetadata import ObjectDatasetMetadata
+from dsversioner.ObjectDatasetRecordData import PandasObjectDatasetRecordData
+from dsversioner.ObjectDatasetVersion import ObjectDatasetVersion
+from dsversioner.Storage import RecordStorageFormats
```

### Comparing `dsversioner-0.9.1/LICENSE` & `dsversioner-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dsversioner-0.9.1/pyproject.toml` & `dsversioner-0.9.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dsversioner"
-version = "0.9.1"
+version = "0.9.2"
 authors = [
   { name="Maxim Dernovoi", email="author@example.com" },
 ]
 description = "Flexible and extensible dataset versioning."
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
@@ -29,8 +29,11 @@
     "/src/dsversioner",
     "CONTRIBUTING.md",
     "LICENSE",
     "pyproject.toml",
     "README.md",
     "SECURITY.md"
 ]
+exclue = [
+    ".gitignore"
+]
```

### Comparing `dsversioner-0.9.1/PKG-INFO` & `dsversioner-0.9.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsversioner
-Version: 0.9.1
+Version: 0.9.2
 Summary: Flexible and extensible dataset versioning.
 Author-email: Maxim Dernovoi <author@example.com>
 License: MIT License
         
         Copyright (c) 2023 Maxim Dernovoi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

