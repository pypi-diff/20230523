# Comparing `tmp/dicommeta-0.6.4.tar.gz` & `tmp/dicommeta-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicommeta-0.6.4.tar", max compression
+gzip compressed data, was "dicommeta-0.6.5.tar", max compression
```

## Comparing `dicommeta-0.6.4.tar` & `dicommeta-0.6.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11356 2023-05-09 13:28:51.971341 dicommeta-0.6.4/LICENSE
--rw-r--r--   0        0        0     1901 2023-05-22 22:09:41.951820 dicommeta-0.6.4/README.md
--rw-r--r--   0        0        0      514 2023-05-23 11:59:55.189249 dicommeta-0.6.4/pyproject.toml
--rw-r--r--   0        0        0     3673 2023-05-23 11:56:02.053987 dicommeta-0.6.4/src/dicommeta/Struct.py
--rw-r--r--   0        0        0     2342 2023-05-23 11:49:03.746665 dicommeta-0.6.4/src/dicommeta/Utils.py
--rw-r--r--   0        0        0        0 2023-05-22 22:10:29.709188 dicommeta-0.6.4/src/dicommeta/__init__.py
--rw-r--r--   0        0        0     2361 1970-01-01 00:00:00.000000 dicommeta-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-05-09 13:28:51.971341 dicommeta-0.6.5/LICENSE
+-rw-r--r--   0        0        0     2666 2023-05-23 15:47:43.845985 dicommeta-0.6.5/README.md
+-rw-r--r--   0        0        0      514 2023-05-23 15:58:27.858380 dicommeta-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0     3673 2023-05-23 11:56:02.053987 dicommeta-0.6.5/src/dicommeta/Struct.py
+-rw-r--r--   0        0        0     2342 2023-05-23 11:49:03.746665 dicommeta-0.6.5/src/dicommeta/Utils.py
+-rw-r--r--   0        0        0        0 2023-05-22 22:10:29.709188 dicommeta-0.6.5/src/dicommeta/__init__.py
+-rw-r--r--   0        0        0     3126 1970-01-01 00:00:00.000000 dicommeta-0.6.5/PKG-INFO
```

### Comparing `dicommeta-0.6.4/LICENSE` & `dicommeta-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dicommeta-0.6.4/README.md` & `dicommeta-0.6.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -10,30 +10,30 @@
 pip install dicommeta
 ```
 
 ## Usage
 
 ```python
 from pprint import pprint
-from src.dicommeta import (Series, Study)
-from dicommeta import Instance
+
 from dicommeta.Utils import Mode
+from dicommeta.Struct import Study, Series, Instance
 
 new_dicom_study = Study(
-    StudyInstanceUID='1.3.6.1.4.1.14519.5.2.1.4334.1501.757929841898426427124434115918',
-    SpecificCharacterSet='ISO_IR 100',
-    StudyDate="20190701",
-    StudyTime='023750',
-    AccessionNumber='sdfk324234',
-    ReferringPhysicianName='Dr Strange',
-    PatientName='John Doe',
-    PatientID='A123',
-    StudyUID='study001',
-    PatientBirthDate='2000-01-01',
-    mode=Mode.CT)
+                        StudyInstanceUID='1.3.6.1.4.1.14519.5.2.1.4334.1501.757929841898426427124434115918',
+                        SpecificCharacterSet='ISO_IR 100',
+                        StudyDate="20190701",
+                        StudyTime='023750',
+                        AccessionNumber='sdfk324234',
+                        ReferringPhysicianName='Dr Strange',
+                        PatientName='John Doe',
+                        PatientID='A123',
+                        StudyUID='study001',
+                        PatientBirthDate='20000101',
+                        mode=Mode.CT)
 
 new_series01 = Series(seriesUID='series001')
 new_series01.add_instance(Instance(SOPinstanceUID='Instance001'))
 new_series01.add_instance(Instance(SOPinstanceUID='Instance002'))
 new_series01.add_instance(Instance(SOPinstanceUID='Instance002'))
 new_dicom_study.add_series(new_series01)
 new_series11 = Series(seriesUID='series001')
@@ -46,14 +46,35 @@
 new_series02.add_instance(Instance(SOPinstanceUID='Instance002'))
 new_series02.add_instance(Instance(SOPinstanceUID='Instance003'))
 new_dicom_study.add_series(new_series02)
 
 pprint(new_dicom_study.get_dict())
 pprint(new_dicom_study.get_series(seriesUID='series002'))
 
+new_study01 = Study(StudyUID='study002', StudyDate=['20200101'])
+new_series03 = Series(seriesUID='series003')
+new_series03.add_instance(Instance(SOPinstanceUID='Instance01'))
+new_study01.add_series(new_series03)
+
+study_list = [new_dicom_study, new_study01]
+
+for study in study_list:
+    for instance in study.series_dict:
+        pprint(study.get_series(instance))
+        print("")
+
+print(new_dicom_study.get_series_ids())
+
+print(new_dicom_study.study_datetime)
+print(new_dicom_study.patient_age)
+
+print(new_study01.study_datetime)
+print(new_study01.patient_age)
+
+
 ```
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
```

### Comparing `dicommeta-0.6.4/pyproject.toml` & `dicommeta-0.6.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dicommeta"
-version = "0.6.4"
+version = "0.6.5"
 description = "Dicom Metadata structures"
 authors = ["Kevin Long <longke@pennmedicine.upenn.edu>"]
 readme = "README.md"
 packages = [
     { include = "dicommeta", from = "src" },
 ]
```

### Comparing `dicommeta-0.6.4/src/dicommeta/Struct.py` & `dicommeta-0.6.5/src/dicommeta/Struct.py`

 * *Files identical despite different names*

### Comparing `dicommeta-0.6.4/src/dicommeta/Utils.py` & `dicommeta-0.6.5/src/dicommeta/Utils.py`

 * *Files identical despite different names*

### Comparing `dicommeta-0.6.4/PKG-INFO` & `dicommeta-0.6.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicommeta
-Version: 0.6.4
+Version: 0.6.5
 Summary: Dicom Metadata structures
 Author: Kevin Long
 Author-email: longke@pennmedicine.upenn.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -24,30 +24,30 @@
 pip install dicommeta
 ```
 
 ## Usage
 
 ```python
 from pprint import pprint
-from src.dicommeta import (Series, Study)
-from dicommeta import Instance
+
 from dicommeta.Utils import Mode
+from dicommeta.Struct import Study, Series, Instance
 
 new_dicom_study = Study(
-    StudyInstanceUID='1.3.6.1.4.1.14519.5.2.1.4334.1501.757929841898426427124434115918',
-    SpecificCharacterSet='ISO_IR 100',
-    StudyDate="20190701",
-    StudyTime='023750',
-    AccessionNumber='sdfk324234',
-    ReferringPhysicianName='Dr Strange',
-    PatientName='John Doe',
-    PatientID='A123',
-    StudyUID='study001',
-    PatientBirthDate='2000-01-01',
-    mode=Mode.CT)
+                        StudyInstanceUID='1.3.6.1.4.1.14519.5.2.1.4334.1501.757929841898426427124434115918',
+                        SpecificCharacterSet='ISO_IR 100',
+                        StudyDate="20190701",
+                        StudyTime='023750',
+                        AccessionNumber='sdfk324234',
+                        ReferringPhysicianName='Dr Strange',
+                        PatientName='John Doe',
+                        PatientID='A123',
+                        StudyUID='study001',
+                        PatientBirthDate='20000101',
+                        mode=Mode.CT)
 
 new_series01 = Series(seriesUID='series001')
 new_series01.add_instance(Instance(SOPinstanceUID='Instance001'))
 new_series01.add_instance(Instance(SOPinstanceUID='Instance002'))
 new_series01.add_instance(Instance(SOPinstanceUID='Instance002'))
 new_dicom_study.add_series(new_series01)
 new_series11 = Series(seriesUID='series001')
@@ -60,14 +60,35 @@
 new_series02.add_instance(Instance(SOPinstanceUID='Instance002'))
 new_series02.add_instance(Instance(SOPinstanceUID='Instance003'))
 new_dicom_study.add_series(new_series02)
 
 pprint(new_dicom_study.get_dict())
 pprint(new_dicom_study.get_series(seriesUID='series002'))
 
+new_study01 = Study(StudyUID='study002', StudyDate=['20200101'])
+new_series03 = Series(seriesUID='series003')
+new_series03.add_instance(Instance(SOPinstanceUID='Instance01'))
+new_study01.add_series(new_series03)
+
+study_list = [new_dicom_study, new_study01]
+
+for study in study_list:
+    for instance in study.series_dict:
+        pprint(study.get_series(instance))
+        print("")
+
+print(new_dicom_study.get_series_ids())
+
+print(new_dicom_study.study_datetime)
+print(new_dicom_study.patient_age)
+
+print(new_study01.study_datetime)
+print(new_study01.patient_age)
+
+
 ```
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
```

