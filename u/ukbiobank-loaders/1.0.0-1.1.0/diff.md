# Comparing `tmp/ukbiobank_loaders-1.0.0.tar.gz` & `tmp/ukbiobank_loaders-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ukbiobank_loaders-1.0.0.tar", last modified: Thu Mar 30 10:11:54 2023, max compression
+gzip compressed data, was "ukbiobank_loaders-1.1.0.tar", last modified: Tue May 23 09:50:36 2023, max compression
```

## Comparing `ukbiobank_loaders-1.0.0.tar` & `ukbiobank_loaders-1.1.0.tar`

### file list

```diff
@@ -1,28 +1,59 @@
-drwxr-xr-x   0 bibianaangonese   (503) staff       (20)        0 2023-03-30 10:11:54.309329 ukbiobank_loaders-1.0.0/
--rw-r--r--   0 bibianaangonese   (503) staff       (20)     1069 2023-03-29 10:28:10.000000 ukbiobank_loaders-1.0.0/LICENSE
--rw-r--r--   0 bibianaangonese   (503) staff       (20)     7497 2023-03-30 10:11:54.309087 ukbiobank_loaders-1.0.0/PKG-INFO
--rw-r--r--   0 bibianaangonese   (503) staff       (20)     6669 2023-03-30 10:11:25.000000 ukbiobank_loaders-1.0.0/README.md
--rw-r--r--   0 bibianaangonese   (503) staff       (20)       38 2023-03-30 10:11:54.309387 ukbiobank_loaders-1.0.0/setup.cfg
--rw-r--r--   0 bibianaangonese   (503) staff       (20)     1921 2023-03-29 12:29:19.000000 ukbiobank_loaders-1.0.0/setup.py
-drwxr-xr-x   0 bibianaangonese   (503) staff       (20)        0 2023-03-30 10:11:54.304823 ukbiobank_loaders-1.0.0/ukbb_loaders/
--rw-r--r--   0 bibianaangonese   (503) staff       (20)       22 2023-03-29 13:07:15.000000 ukbiobank_loaders-1.0.0/ukbb_loaders/__init__.py
-drwxr-xr-x   0 bibianaangonese   (503) staff       (20)        0 2023-03-30 10:11:54.305144 ukbiobank_loaders-1.0.0/ukbb_loaders/loaders/
--rw-r--r--   0 bibianaangonese   (503) staff       (20)        0 2023-03-29 12:13:48.000000 ukbiobank_loaders-1.0.0/ukbb_loaders/loaders/__init__.py
--rw-r--r--   0 bibianaangonese   (503) staff       (20)     8587 2023-03-29 12:13:48.000000 ukbiobank_loaders-1.0.0/ukbb_loaders/loaders/load.py
-drwxr-xr-x   0 bibianaangonese   (503) staff       (20)        0 2023-03-30 10:11:54.305794 ukbiobank_loaders-1.0.0/ukbb_parser/
--rw-r--r--   0 bibianaangonese   (503) staff       (20)        0 2023-03-29 12:13:48.000000 ukbiobank_loaders-1.0.0/ukbb_parser/__init__.py
--rw-r--r--   0 bibianaangonese   (503) staff       (20)     1914 2023-03-29 12:13:48.000000 ukbiobank_loaders-1.0.0/ukbb_parser/update_data.py
-drwxr-xr-x   0 bibianaangonese   (503) staff       (20)        0 2023-03-30 10:11:54.307263 ukbiobank_loaders-1.0.0/ukbb_parser/updater/
--rw-r--r--   0 bibianaangonese   (503) staff       (20)        0 2023-03-29 12:13:48.000000 ukbiobank_loaders-1.0.0/ukbb_parser/updater/__init__.py
--rw-r--r--   0 bibianaangonese   (503) staff       (20)     1902 2023-03-29 12:13:48.000000 ukbiobank_loaders-1.0.0/ukbb_parser/updater/derive_death.py
--rw-r--r--   0 bibianaangonese   (503) staff       (20)     1761 2023-03-29 12:13:48.000000 ukbiobank_loaders-1.0.0/ukbb_parser/updater/derive_gp.py
--rw-r--r--   0 bibianaangonese   (503) staff       (20)     2940 2023-03-29 12:13:48.000000 ukbiobank_loaders-1.0.0/ukbb_parser/updater/derive_hospital.py
--rw-r--r--   0 bibianaangonese   (503) staff       (20)     7592 2023-03-29 12:13:48.000000 ukbiobank_loaders-1.0.0/ukbb_parser/updater/standardise_raw.py
--rw-r--r--   0 bibianaangonese   (503) staff       (20)      744 2023-03-29 12:13:48.000000 ukbiobank_loaders-1.0.0/ukbb_parser/updater/utils.py
-drwxr-xr-x   0 bibianaangonese   (503) staff       (20)        0 2023-03-30 10:11:54.308758 ukbiobank_loaders-1.0.0/ukbiobank_loaders.egg-info/
--rw-r--r--   0 bibianaangonese   (503) staff       (20)     7497 2023-03-30 10:11:54.000000 ukbiobank_loaders-1.0.0/ukbiobank_loaders.egg-info/PKG-INFO
--rw-r--r--   0 bibianaangonese   (503) staff       (20)      616 2023-03-30 10:11:54.000000 ukbiobank_loaders-1.0.0/ukbiobank_loaders.egg-info/SOURCES.txt
--rw-r--r--   0 bibianaangonese   (503) staff       (20)        1 2023-03-30 10:11:54.000000 ukbiobank_loaders-1.0.0/ukbiobank_loaders.egg-info/dependency_links.txt
--rw-r--r--   0 bibianaangonese   (503) staff       (20)        1 2023-03-29 12:14:22.000000 ukbiobank_loaders-1.0.0/ukbiobank_loaders.egg-info/not-zip-safe
--rw-r--r--   0 bibianaangonese   (503) staff       (20)       68 2023-03-30 10:11:54.000000 ukbiobank_loaders-1.0.0/ukbiobank_loaders.egg-info/requires.txt
--rw-r--r--   0 bibianaangonese   (503) staff       (20)       25 2023-03-30 10:11:54.000000 ukbiobank_loaders-1.0.0/ukbiobank_loaders.egg-info/top_level.txt
+drwxr-xr-x   0 bibianaangonese   (503) staff       (20)        0 2023-05-23 09:50:36.619934 ukbiobank_loaders-1.1.0/
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)     1069 2023-03-29 10:28:10.000000 ukbiobank_loaders-1.1.0/LICENSE
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)     8642 2023-05-23 09:50:36.619608 ukbiobank_loaders-1.1.0/PKG-INFO
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)     7814 2023-05-23 09:48:48.000000 ukbiobank_loaders-1.1.0/README.md
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)       38 2023-05-23 09:50:36.619997 ukbiobank_loaders-1.1.0/setup.cfg
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)     1921 2023-03-29 12:29:19.000000 ukbiobank_loaders-1.1.0/setup.py
+drwxr-xr-x   0 bibianaangonese   (503) staff       (20)        0 2023-05-23 09:50:36.589426 ukbiobank_loaders-1.1.0/ukbb_loaders/
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)       22 2023-05-23 09:49:30.000000 ukbiobank_loaders-1.1.0/ukbb_loaders/__init__.py
+drwxr-xr-x   0 bibianaangonese   (503) staff       (20)        0 2023-05-23 09:50:36.589578 ukbiobank_loaders-1.1.0/ukbb_loaders/files/
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)        0 2023-05-23 09:48:48.000000 ukbiobank_loaders-1.1.0/ukbb_loaders/files/__init__.py
+drwxr-xr-x   0 bibianaangonese   (503) staff       (20)        0 2023-05-23 09:50:36.608515 ukbiobank_loaders-1.1.0/ukbb_loaders/files/lookups/
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)        0 2023-05-23 09:48:48.000000 ukbiobank_loaders-1.1.0/ukbb_loaders/files/lookups/__init__.py
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)   638385 2023-05-23 09:48:48.000000 ukbiobank_loaders-1.1.0/ukbb_loaders/files/lookups/ehr_diagnosis_icd10.parquet
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)   461386 2023-05-23 09:48:48.000000 ukbiobank_loaders-1.1.0/ukbb_loaders/files/lookups/ehr_diagnosis_icd9.parquet
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)    50221 2023-05-23 09:48:48.000000 ukbiobank_loaders-1.1.0/ukbb_loaders/files/lookups/ehr_diagnosis_phecodes.parquet
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)  2134186 2023-05-23 09:48:48.000000 ukbiobank_loaders-1.1.0/ukbb_loaders/files/lookups/ehr_diagnosis_read2.parquet
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)  7081013 2023-05-23 09:48:49.000000 ukbiobank_loaders-1.1.0/ukbb_loaders/files/lookups/ehr_diagnosis_read3.parquet
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)    59659 2023-05-23 09:48:49.000000 ukbiobank_loaders-1.1.0/ukbb_loaders/files/lookups/ehr_procedures_opcs3.parquet
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)   368931 2023-05-23 09:48:49.000000 ukbiobank_loaders-1.1.0/ukbb_loaders/files/lookups/ehr_procedures_opcs4.parquet
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)     3651 2023-05-23 09:48:49.000000 ukbiobank_loaders-1.1.0/ukbb_loaders/files/lookups/parent_lookup.parquet
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)   835534 2023-05-23 09:48:49.000000 ukbiobank_loaders-1.1.0/ukbb_loaders/files/lookups/ukbiobank_assessment_centre_fields.parquet
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)    20577 2023-05-23 09:48:49.000000 ukbiobank_loaders-1.1.0/ukbb_loaders/files/lookups/ukbiobank_diagnosis_self_reported_20002.parquet
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)     4730 2023-05-23 09:48:49.000000 ukbiobank_loaders-1.1.0/ukbb_loaders/files/lookups/ukbiobank_ethnicity.parquet
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)   159088 2023-05-23 09:48:49.000000 ukbiobank_loaders-1.1.0/ukbb_loaders/files/lookups/ukbiobank_medications_self_reported_20003.parquet
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)    77597 2023-05-23 09:48:49.000000 ukbiobank_loaders-1.1.0/ukbb_loaders/files/lookups/ukbiobank_metabolomics_fields.parquet
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)    14110 2023-05-23 09:48:49.000000 ukbiobank_loaders-1.1.0/ukbb_loaders/files/lookups/ukbiobank_procedures_self_reported_20004.parquet
+drwxr-xr-x   0 bibianaangonese   (503) staff       (20)        0 2023-05-23 09:50:36.614864 ukbiobank_loaders-1.1.0/ukbb_loaders/files/mappers/
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)        0 2023-05-23 09:48:49.000000 ukbiobank_loaders-1.1.0/ukbb_loaders/files/mappers/__init__.py
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)     5183 2023-05-23 09:48:49.000000 ukbiobank_loaders-1.1.0/ukbb_loaders/files/mappers/ac_to_opcs4.parquet
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)   201207 2023-05-23 09:48:49.000000 ukbiobank_loaders-1.1.0/ukbb_loaders/files/mappers/atc_child_to_parent.parquet
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)   189259 2023-05-23 09:48:49.000000 ukbiobank_loaders-1.1.0/ukbb_loaders/files/mappers/icd10_to_mondo.parquet
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)   369473 2023-05-23 09:48:49.000000 ukbiobank_loaders-1.1.0/ukbb_loaders/files/mappers/icd10_to_phecodes.parquet
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)   268607 2023-05-23 09:48:49.000000 ukbiobank_loaders-1.1.0/ukbb_loaders/files/mappers/medications_to_atc.parquet
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)    37050 2023-05-23 09:48:49.000000 ukbiobank_loaders-1.1.0/ukbb_loaders/files/mappers/mondo_to_icd10.parquet
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)     3412 2023-05-23 09:48:49.000000 ukbiobank_loaders-1.1.0/ukbb_loaders/files/mappers/opcs3_to_opcs4.parquet
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)   203782 2023-05-23 09:48:49.000000 ukbiobank_loaders-1.1.0/ukbb_loaders/files/mappers/readcode_to_icd10.parquet
+drwxr-xr-x   0 bibianaangonese   (503) staff       (20)        0 2023-05-23 09:50:36.615571 ukbiobank_loaders-1.1.0/ukbb_loaders/loaders/
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)        0 2023-03-29 12:13:48.000000 ukbiobank_loaders-1.1.0/ukbb_loaders/loaders/__init__.py
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)     8725 2023-05-23 09:48:49.000000 ukbiobank_loaders-1.1.0/ukbb_loaders/loaders/load.py
+drwxr-xr-x   0 bibianaangonese   (503) staff       (20)        0 2023-05-23 09:50:36.615963 ukbiobank_loaders-1.1.0/ukbb_loaders/utilities/
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)        0 2023-05-23 09:48:49.000000 ukbiobank_loaders-1.1.0/ukbb_loaders/utilities/__init__.py
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)     1068 2023-05-23 09:48:49.000000 ukbiobank_loaders-1.1.0/ukbb_loaders/utilities/util.py
+drwxr-xr-x   0 bibianaangonese   (503) staff       (20)        0 2023-05-23 09:50:36.616340 ukbiobank_loaders-1.1.0/ukbb_parser/
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)        0 2023-03-29 12:13:48.000000 ukbiobank_loaders-1.1.0/ukbb_parser/__init__.py
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)     1914 2023-03-29 12:13:48.000000 ukbiobank_loaders-1.1.0/ukbb_parser/update_data.py
+drwxr-xr-x   0 bibianaangonese   (503) staff       (20)        0 2023-05-23 09:50:36.618067 ukbiobank_loaders-1.1.0/ukbb_parser/updater/
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)        0 2023-03-29 12:13:48.000000 ukbiobank_loaders-1.1.0/ukbb_parser/updater/__init__.py
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)     1902 2023-03-29 12:13:48.000000 ukbiobank_loaders-1.1.0/ukbb_parser/updater/derive_death.py
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)     1761 2023-03-29 12:13:48.000000 ukbiobank_loaders-1.1.0/ukbb_parser/updater/derive_gp.py
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)     2940 2023-03-29 12:13:48.000000 ukbiobank_loaders-1.1.0/ukbb_parser/updater/derive_hospital.py
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)     7592 2023-03-29 12:13:48.000000 ukbiobank_loaders-1.1.0/ukbb_parser/updater/standardise_raw.py
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)      744 2023-03-29 12:13:48.000000 ukbiobank_loaders-1.1.0/ukbb_parser/updater/utils.py
+drwxr-xr-x   0 bibianaangonese   (503) staff       (20)        0 2023-05-23 09:50:36.619336 ukbiobank_loaders-1.1.0/ukbiobank_loaders.egg-info/
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)     8642 2023-05-23 09:50:36.000000 ukbiobank_loaders-1.1.0/ukbiobank_loaders.egg-info/PKG-INFO
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)     2059 2023-05-23 09:50:36.000000 ukbiobank_loaders-1.1.0/ukbiobank_loaders.egg-info/SOURCES.txt
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)        1 2023-05-23 09:50:36.000000 ukbiobank_loaders-1.1.0/ukbiobank_loaders.egg-info/dependency_links.txt
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)        1 2023-03-29 12:14:22.000000 ukbiobank_loaders-1.1.0/ukbiobank_loaders.egg-info/not-zip-safe
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)       68 2023-05-23 09:50:36.000000 ukbiobank_loaders-1.1.0/ukbiobank_loaders.egg-info/requires.txt
+-rw-r--r--   0 bibianaangonese   (503) staff       (20)       25 2023-05-23 09:50:36.000000 ukbiobank_loaders-1.1.0/ukbiobank_loaders.egg-info/top_level.txt
```

### Comparing `ukbiobank_loaders-1.0.0/LICENSE` & `ukbiobank_loaders-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ukbiobank_loaders-1.0.0/PKG-INFO` & `ukbiobank_loaders-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: ukbiobank_loaders
-Version: 1.0.0
-Summary: Utility package for handling UK Biobank data
-Home-page: https://github.com/BenevolentAI/ukbiobank-loaders
-Author: BenevolentAI
-Author-email: ukbiobank.loaders@benevolent.ai
-License: MIT
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Software Development
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ukbiobank-loaders
 
 This repository provides an easy way to load UK Biobank data. It is composed of a pre-processing script, which converts the UK Biobank data into parquets that are easier to read,
 and a library that provides different methods to access the data.
 
 ## Installation
 To install this package, simply run
@@ -81,31 +59,88 @@
 73            NaT  icd10    N181      1
 48     1997-06-20  icd10    N181      1
 48     1945-03-05  icd10    N181      1
 48     1956-02-25  icd10    N181      1
 48     1981-04-08  icd10    N181      1
 ```
 
-### Documentation for ukbb\_loaders.loaders.load
+### Documentation for ukbb\_loaders.loaders
+
+### Table of Contents
+
+* [ukbb\_loaders.utilities.util](#ukbb_loaders.utilities.util)
+  * [load\_lookup](#ukbb_loaders.utilities.util.load_lookup)
+  * [load\_mapper](#ukbb_loaders.utilities.util.load_mapper)
+* [ukbb\_loaders.loaders.load](#ukbb_loaders.loaders.load)
+  * [DataLoader](#ukbb_loaders.loaders.load.DataLoader)
+    * [\_\_init\_\_](#ukbb_loaders.loaders.load.DataLoader.__init__)
+    * [get\_hospital\_data](#ukbb_loaders.loaders.load.DataLoader.get_hospital_data)
+    * [get\_death\_data](#ukbb_loaders.loaders.load.DataLoader.get_death_data)
+    * [get\_gp\_clinical\_data](#ukbb_loaders.loaders.load.DataLoader.get_gp_clinical_data)
+    * [get\_gp\_medication\_data](#ukbb_loaders.loaders.load.DataLoader.get_gp_medication_data)
+
+<a id="ukbb_loaders"></a>
+
+### ukbb\_loaders.utilities.util
+
+<a id="ukbb_loaders.utilities.util.load_lookup"></a>
+
+#### load\_lookup
+
+```python
+def load_lookup(lookup_name: str) -> pd.DataFrame
+```
+
+Loads lookup table.
+
+**Arguments**:
+
+- `lookup_name` _str_ - The name of the lookup table to be loaded.
+  
+
+**Returns**:
 
-#### Table of Contents
+- `(pd.DataFrame)` - The lookup table of interest.
+  
 
-* [DataLoader](#ukbb_loaders.loaders.load.DataLoader)
-  * [\_\_init\_\_](#ukbb_loaders.loaders.load.DataLoader.__init__)
-  * [get\_hospital\_data](#ukbb_loaders.loaders.load.DataLoader.get_hospital_data)
-  * [get\_death\_data](#ukbb_loaders.loaders.load.DataLoader.get_death_data)
-  * [get\_gp\_clinical\_data](#ukbb_loaders.loaders.load.DataLoader.get_gp_clinical_data)
-  * [get\_gp\_medication\_data](#ukbb_loaders.loaders.load.DataLoader.get_gp_medication_data)
+**Example**:
+  Load lookup of ICD10 diagnosis codes:
+  >>> load_lookup("ehr_diagnosis_icd10")
+  
 
+<a id="ukbb_loaders.utilities.util.load_mapper"></a>
+
+#### load\_mapper
+
+```python
+def load_mapper(mapper_name: str) -> pd.DataFrame
+```
+Loads ontology mapper.
+
+**Arguments**:
+
+- `mapper_name` _str_ - The name of the mapper to be loaded.
+
+**Returns**:
+
+- `(pd.DataFrame)` - The mapper of interest.
+  
+
+**Example**:
+  Load mapping from ICD10 codes to Phecodes:
+  >>> load_mapper("icd10_to_phecodes")
+  
+
+### ukbb\_loaders.loaders.load
 
 Loaders for versioned UKBB data.
 
 <a id="ukbb_loaders.loaders.load.DataLoader"></a>
 
-#### DataLoader Objects
+### DataLoader Objects
 
 ```python
 class DataLoader()
 ```
 
 <a id="ukbb_loaders.loaders.load.DataLoader.__init__"></a>
 
@@ -115,48 +150,51 @@
 def __init__(data_dir: str)
 ```
 
 Class for loading UKBB data.
 
 **Arguments**:
 
-- `data_dir` _str_ - The path to the directory containing the processed data. Note that on Windows the path must
-  have forward slashes, e.g.  "C:/Users/john/Documents/data_dir"
+- `data_dir` _str_ - The path to the directory containing the processed data.
+  Note that on Windows the path must have forward-slashes,
+  e.g.  "C:/Users/john/Documents/data_dir"
 
 <a id="ukbb_loaders.loaders.load.DataLoader.get_hospital_data"></a>
 
 #### get\_hospital\_data
 
 ```python
 def get_hospital_data(source: Union[str, List[str]],
                       level=None,
                       patient_list: np.ndarray = None) -> pd.DataFrame
 ```
 
+Method that fetches hospital data for the UKBB population.
+
 **Arguments**:
 
 - `source` _str or list_ - The coding/representation/source we would like to fetch.
   It needs to be one or more of:
-  - `icd10` - for fetching all icd10 related diagnoses.
-  - `icd9` - for fetching all icd9 related diagnoses.
-  - `opcs3` - for fetching all opcs4 related operational codes.
-  - `opcs4` - for fetching all opcs4 related operational codes.
+- `icd10` - for fetching all icd10 related diagnoses.
+- `icd9` - for fetching all icd9 related diagnoses.
+- `opcs3` - for fetching all opcs4 related operational codes.
+- `opcs4` - for fetching all opcs4 related operational codes.
 - `level` _list or string_ - The level/significance of diagnoses we would like to fetch.
   It needs to be one or both of:
-  - `primary` - for fetching only the primary code related to one diagnosis.
-  - `secondary` - for fetching all the secondary (complementary) codes for one
-    diagnosis.
-  - `external` - For fetching diagnosis codes from external sources.
-    Defaults to all of them.
+- `primary` - for fetching only the primary code related to one diagnosis.
+- `secondary` - for fetching all the secondary (complementary) codes for one
+  diagnosis.
+- `external` - For fetching diagnosis codes from external sources.
+  Defaults to all of them.
 - `patient_list` _np.ndarray_ - The patients to fetch characteristics for. If this is empty,
   all UKBB patients will be used.
 
 **Returns**:
 
-- `df` _pandas dataframe_ - A long canonical dataframe with patients as the index and the
+- `df` _pd.DataFrame_ - A long canonical dataframe with patients as the index and the
   following columns:
   - date_of_visit: pandas datetime for each hospital visit
   - feature: the different codes used (e.g. the different icd10 codes)
   - source: this is relevant to the source the feature is referring to (e.g. icd10)
   - value: the occurrence value for each row combination (initially 1.)
 
 <a id="ukbb_loaders.loaders.load.DataLoader.get_death_data"></a>
@@ -175,50 +213,51 @@
 - `level` _list or string_ - The level/significance of deaths we would like to fetch.
   It needs to be one or both of: primary (main reason of death), secondary. Defaults to both.
 - `patient_list` _np.ndarray_ - The patients to fetch characteristics for.
   If this is empty, all UKBB patients will be used.
 
 **Returns**:
 
-- `df` _pandas dataframe_ : A long canonical dataframe with patients as the index and all
+- `df` _pd.DataFrame_ - A long canonical dataframe with patients as the index and all
   recorded death information including death date in the right format.
 
 <a id="ukbb_loaders.loaders.load.DataLoader.get_gp_clinical_data"></a>
 
 #### get\_gp\_clinical\_data
 
 ```python
 def get_gp_clinical_data(source=None, patient_list: np.ndarray = None)
 ```
 
-Method that fetches gp diagnosis information for the UKBB population.
+Method that fetches GP diagnosis information for the UKBB population.
 
 **Arguments**:
 
 - `source` _str or list_ - Whether to load read_2, read_3 or both. Defaults to both.
 - `patient_list` _np.ndarray_ - The patients to fetch characteristics for.
   If this is empty, all UKBB patients will be used.
 
 **Returns**:
 
-- `df` _pandas dataframe_: A long canonical dataframe with patients as the index and all
+- `df` _pd.DataFrame_ - A long canonical dataframe with patients as the index and all
   recorded gp information including date in the right format.
 
 <a id="ukbb_loaders.loaders.load.DataLoader.get_gp_medication_data"></a>
 
 #### get\_gp\_medication\_data
 
 ```python
 def get_gp_medication_data(patient_list: np.ndarray = None) -> pd.DataFrame
 ```
 
+Method that fetches GP medication data for the UKBB population.
+
 **Arguments**:
 
 - `patient_list` _np.ndarray_ - The patients to fetch medication data for.
   If this is empty, all UKBB patients will be used.
 
 **Returns**:
-- `df` _pandas dataframe_ : A canonical long dataframe with patients as the index and
+
+- `df` _pd.DataFrame_ - A canonical long dataframe with patients as the index and
   features as columns.
 
-## Acknowledgments
-This package is developed using the UK Biobank Resource under Application Number 43138.
```

### Comparing `ukbiobank_loaders-1.0.0/README.md` & `ukbiobank_loaders-1.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: ukbiobank_loaders
+Version: 1.1.0
+Summary: Utility package for handling UK Biobank data
+Home-page: https://github.com/BenevolentAI/ukbiobank-loaders
+Author: BenevolentAI
+Author-email: ukbiobank.loaders@benevolent.ai
+License: MIT
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Requires-Python: >3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # ukbiobank-loaders
 
 This repository provides an easy way to load UK Biobank data. It is composed of a pre-processing script, which converts the UK Biobank data into parquets that are easier to read,
 and a library that provides different methods to access the data.
 
 ## Installation
 To install this package, simply run
@@ -59,31 +81,88 @@
 73            NaT  icd10    N181      1
 48     1997-06-20  icd10    N181      1
 48     1945-03-05  icd10    N181      1
 48     1956-02-25  icd10    N181      1
 48     1981-04-08  icd10    N181      1
 ```
 
-### Documentation for ukbb\_loaders.loaders.load
+### Documentation for ukbb\_loaders.loaders
+
+### Table of Contents
+
+* [ukbb\_loaders.utilities.util](#ukbb_loaders.utilities.util)
+  * [load\_lookup](#ukbb_loaders.utilities.util.load_lookup)
+  * [load\_mapper](#ukbb_loaders.utilities.util.load_mapper)
+* [ukbb\_loaders.loaders.load](#ukbb_loaders.loaders.load)
+  * [DataLoader](#ukbb_loaders.loaders.load.DataLoader)
+    * [\_\_init\_\_](#ukbb_loaders.loaders.load.DataLoader.__init__)
+    * [get\_hospital\_data](#ukbb_loaders.loaders.load.DataLoader.get_hospital_data)
+    * [get\_death\_data](#ukbb_loaders.loaders.load.DataLoader.get_death_data)
+    * [get\_gp\_clinical\_data](#ukbb_loaders.loaders.load.DataLoader.get_gp_clinical_data)
+    * [get\_gp\_medication\_data](#ukbb_loaders.loaders.load.DataLoader.get_gp_medication_data)
+
+<a id="ukbb_loaders"></a>
+
+### ukbb\_loaders.utilities.util
+
+<a id="ukbb_loaders.utilities.util.load_lookup"></a>
+
+#### load\_lookup
+
+```python
+def load_lookup(lookup_name: str) -> pd.DataFrame
+```
+
+Loads lookup table.
+
+**Arguments**:
+
+- `lookup_name` _str_ - The name of the lookup table to be loaded.
+  
+
+**Returns**:
 
-#### Table of Contents
+- `(pd.DataFrame)` - The lookup table of interest.
+  
 
-* [DataLoader](#ukbb_loaders.loaders.load.DataLoader)
-  * [\_\_init\_\_](#ukbb_loaders.loaders.load.DataLoader.__init__)
-  * [get\_hospital\_data](#ukbb_loaders.loaders.load.DataLoader.get_hospital_data)
-  * [get\_death\_data](#ukbb_loaders.loaders.load.DataLoader.get_death_data)
-  * [get\_gp\_clinical\_data](#ukbb_loaders.loaders.load.DataLoader.get_gp_clinical_data)
-  * [get\_gp\_medication\_data](#ukbb_loaders.loaders.load.DataLoader.get_gp_medication_data)
+**Example**:
+  Load lookup of ICD10 diagnosis codes:
+  >>> load_lookup("ehr_diagnosis_icd10")
+  
 
+<a id="ukbb_loaders.utilities.util.load_mapper"></a>
+
+#### load\_mapper
+
+```python
+def load_mapper(mapper_name: str) -> pd.DataFrame
+```
+Loads ontology mapper.
+
+**Arguments**:
+
+- `mapper_name` _str_ - The name of the mapper to be loaded.
+
+**Returns**:
+
+- `(pd.DataFrame)` - The mapper of interest.
+  
+
+**Example**:
+  Load mapping from ICD10 codes to Phecodes:
+  >>> load_mapper("icd10_to_phecodes")
+  
+
+### ukbb\_loaders.loaders.load
 
 Loaders for versioned UKBB data.
 
 <a id="ukbb_loaders.loaders.load.DataLoader"></a>
 
-#### DataLoader Objects
+### DataLoader Objects
 
 ```python
 class DataLoader()
 ```
 
 <a id="ukbb_loaders.loaders.load.DataLoader.__init__"></a>
 
@@ -93,48 +172,51 @@
 def __init__(data_dir: str)
 ```
 
 Class for loading UKBB data.
 
 **Arguments**:
 
-- `data_dir` _str_ - The path to the directory containing the processed data. Note that on Windows the path must
-  have forward slashes, e.g.  "C:/Users/john/Documents/data_dir"
+- `data_dir` _str_ - The path to the directory containing the processed data.
+  Note that on Windows the path must have forward-slashes,
+  e.g.  "C:/Users/john/Documents/data_dir"
 
 <a id="ukbb_loaders.loaders.load.DataLoader.get_hospital_data"></a>
 
 #### get\_hospital\_data
 
 ```python
 def get_hospital_data(source: Union[str, List[str]],
                       level=None,
                       patient_list: np.ndarray = None) -> pd.DataFrame
 ```
 
+Method that fetches hospital data for the UKBB population.
+
 **Arguments**:
 
 - `source` _str or list_ - The coding/representation/source we would like to fetch.
   It needs to be one or more of:
-  - `icd10` - for fetching all icd10 related diagnoses.
-  - `icd9` - for fetching all icd9 related diagnoses.
-  - `opcs3` - for fetching all opcs4 related operational codes.
-  - `opcs4` - for fetching all opcs4 related operational codes.
+- `icd10` - for fetching all icd10 related diagnoses.
+- `icd9` - for fetching all icd9 related diagnoses.
+- `opcs3` - for fetching all opcs4 related operational codes.
+- `opcs4` - for fetching all opcs4 related operational codes.
 - `level` _list or string_ - The level/significance of diagnoses we would like to fetch.
   It needs to be one or both of:
-  - `primary` - for fetching only the primary code related to one diagnosis.
-  - `secondary` - for fetching all the secondary (complementary) codes for one
-    diagnosis.
-  - `external` - For fetching diagnosis codes from external sources.
-    Defaults to all of them.
+- `primary` - for fetching only the primary code related to one diagnosis.
+- `secondary` - for fetching all the secondary (complementary) codes for one
+  diagnosis.
+- `external` - For fetching diagnosis codes from external sources.
+  Defaults to all of them.
 - `patient_list` _np.ndarray_ - The patients to fetch characteristics for. If this is empty,
   all UKBB patients will be used.
 
 **Returns**:
 
-- `df` _pandas dataframe_ - A long canonical dataframe with patients as the index and the
+- `df` _pd.DataFrame_ - A long canonical dataframe with patients as the index and the
   following columns:
   - date_of_visit: pandas datetime for each hospital visit
   - feature: the different codes used (e.g. the different icd10 codes)
   - source: this is relevant to the source the feature is referring to (e.g. icd10)
   - value: the occurrence value for each row combination (initially 1.)
 
 <a id="ukbb_loaders.loaders.load.DataLoader.get_death_data"></a>
@@ -153,50 +235,51 @@
 - `level` _list or string_ - The level/significance of deaths we would like to fetch.
   It needs to be one or both of: primary (main reason of death), secondary. Defaults to both.
 - `patient_list` _np.ndarray_ - The patients to fetch characteristics for.
   If this is empty, all UKBB patients will be used.
 
 **Returns**:
 
-- `df` _pandas dataframe_ : A long canonical dataframe with patients as the index and all
+- `df` _pd.DataFrame_ - A long canonical dataframe with patients as the index and all
   recorded death information including death date in the right format.
 
 <a id="ukbb_loaders.loaders.load.DataLoader.get_gp_clinical_data"></a>
 
 #### get\_gp\_clinical\_data
 
 ```python
 def get_gp_clinical_data(source=None, patient_list: np.ndarray = None)
 ```
 
-Method that fetches gp diagnosis information for the UKBB population.
+Method that fetches GP diagnosis information for the UKBB population.
 
 **Arguments**:
 
 - `source` _str or list_ - Whether to load read_2, read_3 or both. Defaults to both.
 - `patient_list` _np.ndarray_ - The patients to fetch characteristics for.
   If this is empty, all UKBB patients will be used.
 
 **Returns**:
 
-- `df` _pandas dataframe_: A long canonical dataframe with patients as the index and all
+- `df` _pd.DataFrame_ - A long canonical dataframe with patients as the index and all
   recorded gp information including date in the right format.
 
 <a id="ukbb_loaders.loaders.load.DataLoader.get_gp_medication_data"></a>
 
 #### get\_gp\_medication\_data
 
 ```python
 def get_gp_medication_data(patient_list: np.ndarray = None) -> pd.DataFrame
 ```
 
+Method that fetches GP medication data for the UKBB population.
+
 **Arguments**:
 
 - `patient_list` _np.ndarray_ - The patients to fetch medication data for.
   If this is empty, all UKBB patients will be used.
 
 **Returns**:
-- `df` _pandas dataframe_ : A canonical long dataframe with patients as the index and
+
+- `df` _pd.DataFrame_ - A canonical long dataframe with patients as the index and
   features as columns.
 
-## Acknowledgments
-This package is developed using the UK Biobank Resource under Application Number 43138.
```

### Comparing `ukbiobank_loaders-1.0.0/setup.py` & `ukbiobank_loaders-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `ukbiobank_loaders-1.0.0/ukbb_loaders/loaders/load.py` & `ukbiobank_loaders-1.1.0/ukbb_loaders/loaders/load.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,16 +18,17 @@
     def __init__(
             self,
             data_dir: str,
     ):
         """
         Class for loading UKBB data.
         Args:
-            data_dir (str): The path to the directory containing the processed data. Note that on Windows the path must
-            have forward-slashes, e.g.  "C:/Users/john/Documents/data_dir"
+            data_dir (str): The path to the directory containing the processed data.
+            Note that on Windows the path must have forward-slashes,
+            e.g.  "C:/Users/john/Documents/data_dir"
         """
         self.data_path = self._check_if_exists(data_dir=data_dir)
         self.hospital_map = {
             "icd9": "ehr_diagnosis_icd9.parquet",
             "icd10": "ehr_diagnosis_icd10.parquet",
             "opcs3": "ehr_procedures_opcs3.parquet",
             "opcs4": "ehr_procedures_opcs4.parquet",
@@ -58,14 +59,16 @@
     def get_hospital_data(
             self,
             source: Union[str, List[str]],
             level=None,
             patient_list: np.ndarray = None,
     ) -> pd.DataFrame:
         """
+        Method that fetches hospital data for the UKBB population.
+
         Args:
             source (str or list): The coding/representation/source we would like to fetch.
                 It needs to be one or more of:
                     icd10: for fetching all icd10 related diagnoses.
                     icd9: for fetching all icd9 related diagnoses.
                     opcs3: for fetching all opcs4 related operational codes.
                     opcs4: for fetching all opcs4 related operational codes.
@@ -75,15 +78,15 @@
                     secondary: for fetching all the secondary (complementary) codes for one
                         diagnosis.
                     external: For fetching diagnosis codes from external sources.
                 Defaults to all of them.
             patient_list (np.ndarray): The patients to fetch characteristics for. If this is empty,
                 all UKBB patients will be used.
         Returns:
-            df (pandas dataframe): A long canonical dataframe with patients as the index and the
+            df (pd.DataFrame): A long canonical dataframe with patients as the index and the
             following columns:
                 - date_of_visit: pandas datetime for each hospital visit
                 - feature: the different codes used (e.g. the different icd10 codes)
                 - source: this is relevant to the source the feature is referring to (e.g. icd10)
                 - value: the occurrence value for each row combination (initially 1.)
         """
         # Check if source and level got one of the accepted values
@@ -119,15 +122,15 @@
 
         Args:
             level (list or string): The level/significance of deaths we would like to fetch.
                 It needs to be one or both of: primary (main reason of death), secondary. Defaults to both.
             patient_list (np.ndarray): The patients to fetch characteristics for.
                 If this is empty, all UKBB patients will be used.
         Returns:
-            df (pandas dataframe): A long canonical dataframe with patients as the index and all
+            df (pd.DataFrame): A long canonical dataframe with patients as the index and all
                 recorded death information including death date in the right format.
         """
         if level is None:
             level = ["primary", "secondary"]
         _check_arg(given=level, accepted=["primary", "secondary"], arg_type="level")
         levels = _to_list_type(level)
 
@@ -144,21 +147,22 @@
         return df.rename({"date": "date_of_death"}, axis=1)
 
     def get_gp_clinical_data(
             self, source=None,
             patient_list: np.ndarray = None
     ):
         """
-        Method that fetches gp diagnosis information for the UKBB population.
+        Method that fetches GP diagnosis information for the UKBB population.
+
         Args:
             source (str or list): Whether to load read_2, read_3 or both. Defaults to both.
             patient_list (np.ndarray): The patients to fetch characteristics for.
                 If this is empty, all UKBB patients will be used.
         Returns:
-            df (pandas dataframe): A long canonical dataframe with patients as the index and all
+            df (pd.DataFrame): A long canonical dataframe with patients as the index and all
                 recorded gp information including date in the right format.
         """
         # Check if source got one of the accepted values
         if source is None:
             source = ["read_2", "read_3"]
         _check_arg(given=source, accepted=self.gp_map, arg_type="source")
         sources = _to_list_type(source)
@@ -173,19 +177,21 @@
         df = pd.concat(df_list)
         df["value"] = 1
 
         return df.rename({"date": "date_of_visit"}, axis=1)
 
     def get_gp_medication_data(self, patient_list: np.ndarray = None) -> pd.DataFrame:
         """
+        Method that fetches GP medication data for the UKBB population.
+
         Args:
             patient_list (np.ndarray): The patients to fetch medication data for.
                 If this is empty, all UKBB patients will be used.
         Returns:
-            df (pandas dataframe): A canonical long dataframe with patients as the index and
+            df (pd.DataFrame): A canonical long dataframe with patients as the index and
                 features as columns.
         """
         df = pd.read_parquet(pjoin(self.data_path, "gp_medications.parquet"))
         if (patient_list is not None) and (len(patient_list) > 0):
             df = df.loc[df.index.isin(patient_list)]
         df = df.rename({"date": "date_of_issue"}, axis=1)
         return df
```

### Comparing `ukbiobank_loaders-1.0.0/ukbb_parser/update_data.py` & `ukbiobank_loaders-1.1.0/ukbb_parser/update_data.py`

 * *Files identical despite different names*

### Comparing `ukbiobank_loaders-1.0.0/ukbb_parser/updater/derive_death.py` & `ukbiobank_loaders-1.1.0/ukbb_parser/updater/derive_death.py`

 * *Files identical despite different names*

### Comparing `ukbiobank_loaders-1.0.0/ukbb_parser/updater/derive_gp.py` & `ukbiobank_loaders-1.1.0/ukbb_parser/updater/derive_gp.py`

 * *Files identical despite different names*

### Comparing `ukbiobank_loaders-1.0.0/ukbb_parser/updater/derive_hospital.py` & `ukbiobank_loaders-1.1.0/ukbb_parser/updater/derive_hospital.py`

 * *Files identical despite different names*

### Comparing `ukbiobank_loaders-1.0.0/ukbb_parser/updater/standardise_raw.py` & `ukbiobank_loaders-1.1.0/ukbb_parser/updater/standardise_raw.py`

 * *Files identical despite different names*

### Comparing `ukbiobank_loaders-1.0.0/ukbb_parser/updater/utils.py` & `ukbiobank_loaders-1.1.0/ukbb_parser/updater/utils.py`

 * *Files identical despite different names*

### Comparing `ukbiobank_loaders-1.0.0/ukbiobank_loaders.egg-info/PKG-INFO` & `ukbiobank_loaders-1.1.0/ukbiobank_loaders.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ukbiobank-loaders
-Version: 1.0.0
+Version: 1.1.0
 Summary: Utility package for handling UK Biobank data
 Home-page: https://github.com/BenevolentAI/ukbiobank-loaders
 Author: BenevolentAI
 Author-email: ukbiobank.loaders@benevolent.ai
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -81,31 +81,88 @@
 73            NaT  icd10    N181      1
 48     1997-06-20  icd10    N181      1
 48     1945-03-05  icd10    N181      1
 48     1956-02-25  icd10    N181      1
 48     1981-04-08  icd10    N181      1
 ```
 
-### Documentation for ukbb\_loaders.loaders.load
+### Documentation for ukbb\_loaders.loaders
 
-#### Table of Contents
+### Table of Contents
 
-* [DataLoader](#ukbb_loaders.loaders.load.DataLoader)
-  * [\_\_init\_\_](#ukbb_loaders.loaders.load.DataLoader.__init__)
-  * [get\_hospital\_data](#ukbb_loaders.loaders.load.DataLoader.get_hospital_data)
-  * [get\_death\_data](#ukbb_loaders.loaders.load.DataLoader.get_death_data)
-  * [get\_gp\_clinical\_data](#ukbb_loaders.loaders.load.DataLoader.get_gp_clinical_data)
-  * [get\_gp\_medication\_data](#ukbb_loaders.loaders.load.DataLoader.get_gp_medication_data)
+* [ukbb\_loaders.utilities.util](#ukbb_loaders.utilities.util)
+  * [load\_lookup](#ukbb_loaders.utilities.util.load_lookup)
+  * [load\_mapper](#ukbb_loaders.utilities.util.load_mapper)
+* [ukbb\_loaders.loaders.load](#ukbb_loaders.loaders.load)
+  * [DataLoader](#ukbb_loaders.loaders.load.DataLoader)
+    * [\_\_init\_\_](#ukbb_loaders.loaders.load.DataLoader.__init__)
+    * [get\_hospital\_data](#ukbb_loaders.loaders.load.DataLoader.get_hospital_data)
+    * [get\_death\_data](#ukbb_loaders.loaders.load.DataLoader.get_death_data)
+    * [get\_gp\_clinical\_data](#ukbb_loaders.loaders.load.DataLoader.get_gp_clinical_data)
+    * [get\_gp\_medication\_data](#ukbb_loaders.loaders.load.DataLoader.get_gp_medication_data)
 
+<a id="ukbb_loaders"></a>
+
+### ukbb\_loaders.utilities.util
+
+<a id="ukbb_loaders.utilities.util.load_lookup"></a>
+
+#### load\_lookup
+
+```python
+def load_lookup(lookup_name: str) -> pd.DataFrame
+```
+
+Loads lookup table.
+
+**Arguments**:
+
+- `lookup_name` _str_ - The name of the lookup table to be loaded.
+  
+
+**Returns**:
+
+- `(pd.DataFrame)` - The lookup table of interest.
+  
+
+**Example**:
+  Load lookup of ICD10 diagnosis codes:
+  >>> load_lookup("ehr_diagnosis_icd10")
+  
+
+<a id="ukbb_loaders.utilities.util.load_mapper"></a>
+
+#### load\_mapper
+
+```python
+def load_mapper(mapper_name: str) -> pd.DataFrame
+```
+Loads ontology mapper.
+
+**Arguments**:
+
+- `mapper_name` _str_ - The name of the mapper to be loaded.
+
+**Returns**:
+
+- `(pd.DataFrame)` - The mapper of interest.
+  
+
+**Example**:
+  Load mapping from ICD10 codes to Phecodes:
+  >>> load_mapper("icd10_to_phecodes")
+  
+
+### ukbb\_loaders.loaders.load
 
 Loaders for versioned UKBB data.
 
 <a id="ukbb_loaders.loaders.load.DataLoader"></a>
 
-#### DataLoader Objects
+### DataLoader Objects
 
 ```python
 class DataLoader()
 ```
 
 <a id="ukbb_loaders.loaders.load.DataLoader.__init__"></a>
 
@@ -115,48 +172,51 @@
 def __init__(data_dir: str)
 ```
 
 Class for loading UKBB data.
 
 **Arguments**:
 
-- `data_dir` _str_ - The path to the directory containing the processed data. Note that on Windows the path must
-  have forward slashes, e.g.  "C:/Users/john/Documents/data_dir"
+- `data_dir` _str_ - The path to the directory containing the processed data.
+  Note that on Windows the path must have forward-slashes,
+  e.g.  "C:/Users/john/Documents/data_dir"
 
 <a id="ukbb_loaders.loaders.load.DataLoader.get_hospital_data"></a>
 
 #### get\_hospital\_data
 
 ```python
 def get_hospital_data(source: Union[str, List[str]],
                       level=None,
                       patient_list: np.ndarray = None) -> pd.DataFrame
 ```
 
+Method that fetches hospital data for the UKBB population.
+
 **Arguments**:
 
 - `source` _str or list_ - The coding/representation/source we would like to fetch.
   It needs to be one or more of:
-  - `icd10` - for fetching all icd10 related diagnoses.
-  - `icd9` - for fetching all icd9 related diagnoses.
-  - `opcs3` - for fetching all opcs4 related operational codes.
-  - `opcs4` - for fetching all opcs4 related operational codes.
+- `icd10` - for fetching all icd10 related diagnoses.
+- `icd9` - for fetching all icd9 related diagnoses.
+- `opcs3` - for fetching all opcs4 related operational codes.
+- `opcs4` - for fetching all opcs4 related operational codes.
 - `level` _list or string_ - The level/significance of diagnoses we would like to fetch.
   It needs to be one or both of:
-  - `primary` - for fetching only the primary code related to one diagnosis.
-  - `secondary` - for fetching all the secondary (complementary) codes for one
-    diagnosis.
-  - `external` - For fetching diagnosis codes from external sources.
-    Defaults to all of them.
+- `primary` - for fetching only the primary code related to one diagnosis.
+- `secondary` - for fetching all the secondary (complementary) codes for one
+  diagnosis.
+- `external` - For fetching diagnosis codes from external sources.
+  Defaults to all of them.
 - `patient_list` _np.ndarray_ - The patients to fetch characteristics for. If this is empty,
   all UKBB patients will be used.
 
 **Returns**:
 
-- `df` _pandas dataframe_ - A long canonical dataframe with patients as the index and the
+- `df` _pd.DataFrame_ - A long canonical dataframe with patients as the index and the
   following columns:
   - date_of_visit: pandas datetime for each hospital visit
   - feature: the different codes used (e.g. the different icd10 codes)
   - source: this is relevant to the source the feature is referring to (e.g. icd10)
   - value: the occurrence value for each row combination (initially 1.)
 
 <a id="ukbb_loaders.loaders.load.DataLoader.get_death_data"></a>
@@ -175,50 +235,51 @@
 - `level` _list or string_ - The level/significance of deaths we would like to fetch.
   It needs to be one or both of: primary (main reason of death), secondary. Defaults to both.
 - `patient_list` _np.ndarray_ - The patients to fetch characteristics for.
   If this is empty, all UKBB patients will be used.
 
 **Returns**:
 
-- `df` _pandas dataframe_ : A long canonical dataframe with patients as the index and all
+- `df` _pd.DataFrame_ - A long canonical dataframe with patients as the index and all
   recorded death information including death date in the right format.
 
 <a id="ukbb_loaders.loaders.load.DataLoader.get_gp_clinical_data"></a>
 
 #### get\_gp\_clinical\_data
 
 ```python
 def get_gp_clinical_data(source=None, patient_list: np.ndarray = None)
 ```
 
-Method that fetches gp diagnosis information for the UKBB population.
+Method that fetches GP diagnosis information for the UKBB population.
 
 **Arguments**:
 
 - `source` _str or list_ - Whether to load read_2, read_3 or both. Defaults to both.
 - `patient_list` _np.ndarray_ - The patients to fetch characteristics for.
   If this is empty, all UKBB patients will be used.
 
 **Returns**:
 
-- `df` _pandas dataframe_: A long canonical dataframe with patients as the index and all
+- `df` _pd.DataFrame_ - A long canonical dataframe with patients as the index and all
   recorded gp information including date in the right format.
 
 <a id="ukbb_loaders.loaders.load.DataLoader.get_gp_medication_data"></a>
 
 #### get\_gp\_medication\_data
 
 ```python
 def get_gp_medication_data(patient_list: np.ndarray = None) -> pd.DataFrame
 ```
 
+Method that fetches GP medication data for the UKBB population.
+
 **Arguments**:
 
 - `patient_list` _np.ndarray_ - The patients to fetch medication data for.
   If this is empty, all UKBB patients will be used.
 
 **Returns**:
-- `df` _pandas dataframe_ : A canonical long dataframe with patients as the index and
+
+- `df` _pd.DataFrame_ - A canonical long dataframe with patients as the index and
   features as columns.
 
-## Acknowledgments
-This package is developed using the UK Biobank Resource under Application Number 43138.
```

