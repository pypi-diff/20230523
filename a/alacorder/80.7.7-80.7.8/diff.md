# Comparing `tmp/alacorder-80.7.7.tar.gz` & `tmp/alacorder-80.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.7.7.tar", max compression
+gzip compressed data, was "alacorder-80.7.8.tar", max compression
```

## Comparing `alacorder-80.7.7.tar` & `alacorder-80.7.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.7.7/LICENSE
--rw-r--r--   0        0        0     6518 2023-05-23 14:35:47.192010 alacorder-80.7.7/README.md
--rw-r--r--   0        0        0      746 2023-05-23 14:41:36.020247 alacorder-80.7.7/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-23 14:31:25.922596 alacorder-80.7.7/src/alacorder/.DS_Store
--rw-r--r--   0        0        0   234455 2023-05-18 23:58:39.588863 alacorder-80.7.7/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.7.7/src/alacorder/__init__.py
--rw-r--r--   0        0        0   241423 2023-05-23 14:41:06.651769 alacorder-80.7.7/src/alacorder/__main__.py
--rw-r--r--   0        0        0   241423 2023-05-23 14:41:02.392991 alacorder-80.7.7/src/alacorder/alac.py
--rw-r--r--   0        0        0     7489 1970-01-01 00:00:00.000000 alacorder-80.7.7/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.7.8/LICENSE
+-rw-r--r--   0        0        0     6518 2023-05-23 14:35:47.192010 alacorder-80.7.8/README.md
+-rw-r--r--   0        0        0      746 2023-05-23 15:45:17.010465 alacorder-80.7.8/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-23 14:31:25.922596 alacorder-80.7.8/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0   234455 2023-05-18 23:58:39.588863 alacorder-80.7.8/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.7.8/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   241654 2023-05-23 15:44:47.065973 alacorder-80.7.8/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   241654 2023-05-23 15:44:41.862761 alacorder-80.7.8/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7489 1970-01-01 00:00:00.000000 alacorder-80.7.8/PKG-INFO
```

### Comparing `alacorder-80.7.7/LICENSE` & `alacorder-80.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.7.7/README.md` & `alacorder-80.7.8/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.7.7/pyproject.toml` & `alacorder-80.7.8/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.7.7"
+version = "80.7.8"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.7.7/src/alacorder/.DS_Store` & `alacorder-80.7.8/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-80.7.7/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py` & `alacorder-80.7.8/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py`

 * *Files identical despite different names*

### Comparing `alacorder-80.7.7/src/alacorder/__main__.py` & `alacorder-80.7.8/src/alacorder/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt and crawl ADOC
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.7.6"
+version = "80.7.8"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -2302,15 +2302,15 @@
             pl.col("SEG_2")
             .str.extract(
                 r"(ALCOHOL|BOND|CONSERVATION|DOCKET|DRUG|GOVERNMENT|HEALTH|MUNICIPAL|OTHER|PERSONAL|PROPERTY|SEX|TRAFFIC)",
                 group_index=1,
             )
             .alias("Category"),
             pl.col("RAWDESC")
-            .str.contains(r"(A ATT|ATTEMPT|S SOLICIT|CONSP|SOLICITATION|COMPLICITY)")
+            .str.contains(r"(A ATT|ATTEMPT|S SOLICIT|CONSP|SOLICITATION|COMPLICITY|CONSPIRACY|SOLICIT)")
             .is_not()
             .alias("A_S_C_DISQ"),
             pl.col("Code")
             .str.contains(
                 r"(OSUA|EGUA|MAN1|MAN2|MANS|ASS1|ASS2|KID1|KID2|HUT1|HUT2|BUR1|BUR2|TOP1|TOP2|TP2D|TP2G|TPCS|TPCD|TPC1|TET2|TOD2|ROB1|ROB2|ROB3|FOR1|FOR2|FR2D|MIOB|TRAK|TRAG|VDRU|VDRY|TRAO|TRFT|TRMA|TROP|CHAB|WABC|ACHA|ACAL)"
             )
             .alias("CERV_DISQ_MATCH"),
@@ -2474,18 +2474,22 @@
             .str.replace(r'^\.\d?\s','')
             .str.replace(r'\s[ASC]\s', " ")
             .str.replace(r'^[ASC]\s', "")
         ]
     )
     charges = charges.with_columns(
         [
-        pl.when(pl.col("ID").eq("C") & pl.col("Description").eq("ROBBERY 1ST"))
-        .then("CONSPIRACY -ROBBERY 1ST DEGREE")
-        .otherwise(pl.col("Description"))
-        .alias("Description")
+            pl.when(pl.col("ID").eq("C") & pl.col("Description").eq("ROBBERY 1ST"))
+            .then("CONSPIRACY -ROBBERY 1ST DEGREE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("ID").eq("C") & pl.col("Description").eq("ROBBERY 1ST"))
+            .then(False)
+            .otherwise(pl.col("CERVDisqCharge"))
+            .alias("CERVDisqCharge")
         ]
     )
     charges = charges.with_columns(
         [
             pl.when(pl.col("Charges").str.contains("WILFULL FAILURE TO RETURN TO P"))
             .then("")
             .otherwise(pl.col("ID"))
```

### Comparing `alacorder-80.7.7/src/alacorder/alac.py` & `alacorder-80.7.8/src/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt and crawl ADOC
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.7.6"
+version = "80.7.8"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -2302,15 +2302,15 @@
             pl.col("SEG_2")
             .str.extract(
                 r"(ALCOHOL|BOND|CONSERVATION|DOCKET|DRUG|GOVERNMENT|HEALTH|MUNICIPAL|OTHER|PERSONAL|PROPERTY|SEX|TRAFFIC)",
                 group_index=1,
             )
             .alias("Category"),
             pl.col("RAWDESC")
-            .str.contains(r"(A ATT|ATTEMPT|S SOLICIT|CONSP|SOLICITATION|COMPLICITY)")
+            .str.contains(r"(A ATT|ATTEMPT|S SOLICIT|CONSP|SOLICITATION|COMPLICITY|CONSPIRACY|SOLICIT)")
             .is_not()
             .alias("A_S_C_DISQ"),
             pl.col("Code")
             .str.contains(
                 r"(OSUA|EGUA|MAN1|MAN2|MANS|ASS1|ASS2|KID1|KID2|HUT1|HUT2|BUR1|BUR2|TOP1|TOP2|TP2D|TP2G|TPCS|TPCD|TPC1|TET2|TOD2|ROB1|ROB2|ROB3|FOR1|FOR2|FR2D|MIOB|TRAK|TRAG|VDRU|VDRY|TRAO|TRFT|TRMA|TROP|CHAB|WABC|ACHA|ACAL)"
             )
             .alias("CERV_DISQ_MATCH"),
@@ -2474,18 +2474,22 @@
             .str.replace(r'^\.\d?\s','')
             .str.replace(r'\s[ASC]\s', " ")
             .str.replace(r'^[ASC]\s', "")
         ]
     )
     charges = charges.with_columns(
         [
-        pl.when(pl.col("ID").eq("C") & pl.col("Description").eq("ROBBERY 1ST"))
-        .then("CONSPIRACY -ROBBERY 1ST DEGREE")
-        .otherwise(pl.col("Description"))
-        .alias("Description")
+            pl.when(pl.col("ID").eq("C") & pl.col("Description").eq("ROBBERY 1ST"))
+            .then("CONSPIRACY -ROBBERY 1ST DEGREE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("ID").eq("C") & pl.col("Description").eq("ROBBERY 1ST"))
+            .then(False)
+            .otherwise(pl.col("CERVDisqCharge"))
+            .alias("CERVDisqCharge")
         ]
     )
     charges = charges.with_columns(
         [
             pl.when(pl.col("Charges").str.contains("WILFULL FAILURE TO RETURN TO P"))
             .then("")
             .otherwise(pl.col("ID"))
```

### Comparing `alacorder-80.7.7/PKG-INFO` & `alacorder-80.7.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.7.7
+Version: 80.7.8
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

