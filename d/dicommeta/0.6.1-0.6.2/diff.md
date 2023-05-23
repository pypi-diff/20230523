# Comparing `tmp/dicommeta-0.6.1.tar.gz` & `tmp/dicommeta-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicommeta-0.6.1.tar", max compression
+gzip compressed data, was "dicommeta-0.6.2.tar", max compression
```

## Comparing `dicommeta-0.6.1.tar` & `dicommeta-0.6.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11356 2023-05-09 13:28:51.971341 dicommeta-0.6.1/LICENSE
--rw-r--r--   0        0        0     1901 2023-05-22 22:09:41.951820 dicommeta-0.6.1/README.md
--rw-r--r--   0        0        0      514 2023-05-23 00:18:16.933621 dicommeta-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     3292 2023-05-23 00:17:55.940412 dicommeta-0.6.1/src/dicommeta/Struct.py
--rw-r--r--   0        0        0     2109 2023-05-22 22:29:37.095454 dicommeta-0.6.1/src/dicommeta/Utils.py
--rw-r--r--   0        0        0        0 2023-05-22 22:10:29.709188 dicommeta-0.6.1/src/dicommeta/__init__.py
--rw-r--r--   0        0        0     2361 1970-01-01 00:00:00.000000 dicommeta-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-05-09 13:28:51.971341 dicommeta-0.6.2/LICENSE
+-rw-r--r--   0        0        0     1901 2023-05-22 22:09:41.951820 dicommeta-0.6.2/README.md
+-rw-r--r--   0        0        0      514 2023-05-23 00:27:12.673534 dicommeta-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     3292 2023-05-23 00:27:02.098545 dicommeta-0.6.2/src/dicommeta/Struct.py
+-rw-r--r--   0        0        0     2109 2023-05-22 22:29:37.095454 dicommeta-0.6.2/src/dicommeta/Utils.py
+-rw-r--r--   0        0        0        0 2023-05-22 22:10:29.709188 dicommeta-0.6.2/src/dicommeta/__init__.py
+-rw-r--r--   0        0        0     2361 1970-01-01 00:00:00.000000 dicommeta-0.6.2/PKG-INFO
```

### Comparing `dicommeta-0.6.1/LICENSE` & `dicommeta-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dicommeta-0.6.1/README.md` & `dicommeta-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `dicommeta-0.6.1/pyproject.toml` & `dicommeta-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dicommeta"
-version = "0.6.1"
+version = "0.6.2"
 description = "Dicom Metadata structures"
 authors = ["Kevin Long <longke@pennmedicine.upenn.edu>"]
 readme = "README.md"
 packages = [
     { include = "dicommeta", from = "src" },
 ]
```

### Comparing `dicommeta-0.6.1/src/dicommeta/Struct.py` & `dicommeta-0.6.2/src/dicommeta/Struct.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,33 @@
 
 
 @define(kw_only=True, slots=True, order=True, frozen=True)
 class Instance:
     SOPinstanceUID: str = field(factory=str)
 
 
+@define(kw_only=True, slots=True, order=True, frozen=True)
+class Series:
+    seriesUID: str = field(factory=str)
+    instance_dict: Dict[str, Instance] = field(factory=dict)
+
+    def add_instance(self, instance: Instance):
+        if instance.SOPinstanceUID not in self.instance_dict.keys():
+            self.instance_dict[instance.SOPinstanceUID] = instance
+
+    def get_instance(self, instance_uid: Instance) -> Instance:
+        return self.instance_dict[instance_uid]
+
+    def get_dict(self):
+        return asdict(self)
+
+    def get_iter(self) -> Iterable:
+        return iter(asdict(self))
+
+
 @define(kw_only=True, slots=True, order=True, frozen=False)
 class Study(dict):
     StudyUID: str = field(factory=str, validator=validator_pass)
     StudyInstanceUID: str = field(factory=str)
     SpecificCharacterSet: str = field(factory=str, validator=validator_pass)
     StudyDate: Optional[str] = field(default=None, validator=validator_parsable_date)
     StudyTime: Optional[str] = field(default=None, validator=validator_parsable_time)
@@ -54,26 +73,7 @@
             return asdict(self.series_dict[seriesUID])
 
     def get_dict(self):
         return asdict(self)
 
     def get_iter(self) -> Iterable:
         return iter(asdict(self))
-
-
-@define(kw_only=True, slots=True, order=True, frozen=True)
-class Series:
-    seriesUID: str = field(factory=str)
-    instance_dict: Dict[str, Instance] = field(factory=dict)
-
-    def add_instance(self, instance: Instance):
-        if instance.SOPinstanceUID not in self.instance_dict.keys():
-            self.instance_dict[instance.SOPinstanceUID] = instance
-
-    def get_instance(self, instance_uid: Instance) -> Instance:
-        return self.instance_dict[instance_uid]
-
-    def get_dict(self):
-        return asdict(self)
-
-    def get_iter(self) -> Iterable:
-        return iter(asdict(self))
```

### Comparing `dicommeta-0.6.1/src/dicommeta/Utils.py` & `dicommeta-0.6.2/src/dicommeta/Utils.py`

 * *Files identical despite different names*

### Comparing `dicommeta-0.6.1/PKG-INFO` & `dicommeta-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicommeta
-Version: 0.6.1
+Version: 0.6.2
 Summary: Dicom Metadata structures
 Author: Kevin Long
 Author-email: longke@pennmedicine.upenn.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

