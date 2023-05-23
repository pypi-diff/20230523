# Comparing `tmp/alacorder-80.7.6.tar.gz` & `tmp/alacorder-80.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.7.6.tar", max compression
+gzip compressed data, was "alacorder-80.7.7.tar", max compression
```

## Comparing `alacorder-80.7.6.tar` & `alacorder-80.7.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.7.6/LICENSE
--rw-r--r--   0        0        0     6518 2023-05-23 14:35:47.192010 alacorder-80.7.6/README.md
--rw-r--r--   0        0        0      746 2023-05-23 14:34:18.978330 alacorder-80.7.6/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-23 14:31:25.922596 alacorder-80.7.6/src/alacorder/.DS_Store
--rw-r--r--   0        0        0   234455 2023-05-18 23:58:39.588863 alacorder-80.7.6/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.7.6/src/alacorder/__init__.py
--rw-r--r--   0        0        0   241431 2023-05-23 14:36:11.324709 alacorder-80.7.6/src/alacorder/__main__.py
--rw-r--r--   0        0        0   241431 2023-05-23 14:36:15.027110 alacorder-80.7.6/src/alacorder/alac.py
--rw-r--r--   0        0        0     7489 1970-01-01 00:00:00.000000 alacorder-80.7.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.7.7/LICENSE
+-rw-r--r--   0        0        0     6518 2023-05-23 14:35:47.192010 alacorder-80.7.7/README.md
+-rw-r--r--   0        0        0      746 2023-05-23 14:41:36.020247 alacorder-80.7.7/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-23 14:31:25.922596 alacorder-80.7.7/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0   234455 2023-05-18 23:58:39.588863 alacorder-80.7.7/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.7.7/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   241423 2023-05-23 14:41:06.651769 alacorder-80.7.7/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   241423 2023-05-23 14:41:02.392991 alacorder-80.7.7/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7489 1970-01-01 00:00:00.000000 alacorder-80.7.7/PKG-INFO
```

### Comparing `alacorder-80.7.6/LICENSE` & `alacorder-80.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.7.6/README.md` & `alacorder-80.7.7/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.7.6/pyproject.toml` & `alacorder-80.7.7/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.7.6"
+version = "80.7.7"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.7.6/src/alacorder/.DS_Store` & `alacorder-80.7.7/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-80.7.6/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py` & `alacorder-80.7.7/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py`

 * *Files identical despite different names*

### Comparing `alacorder-80.7.6/src/alacorder/__main__.py` & `alacorder-80.7.7/src/alacorder/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3269,15 +3269,15 @@
     else:
         print(
             "Try again with at least one valid column header: [NAME, PARTY_TYPE, SSN, DOB, COUNTY, DIVISION, CASE_YEAR, NO_RECORDS, FILED_BEFORE, FILED_AFTER, RETRIEVED, CASES_FOUND, QUERY_COMPLETE]"
         )
         return None
 
 def crawl_adoc(path):
-    alphabet = ['AMOS', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z']
+    alphabet = ['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z']
     print("Connecting to ADOC...")
     driver = webdriver.Chrome()
     driver.get("http://www.doc.state.al.us/inmatesearch")
     results = []
     for x in alphabet:
         last_name_box = driver.find_element(by=By.NAME, value="ctl00$MainContent$txtLName")
         last_name_box.send_keys(x)
@@ -3322,15 +3322,15 @@
                 pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w (\w) \d\d\d\d').alias("Sex"),
                 pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w (\d\d\d\d)').alias("YOB").cast(pl.Int64, strict=False),
                 pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w \d\d\d\d ([A-Z\s]+)').str.strip().alias("Institution"),
                 pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w \d\d\d\d [A-Z\s]+ (\d\d/\d\d/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("ReleaseDate")
             ]
         )
         print(out)
-        alac.write(out, sheet_names=['inmates'], path=path, overwrite=True)
+        write(out, sheet_names=['inmates'], path=path, overwrite=True)
     return out
 
 def fetch(
     querypath="",
     dirpath="",
     cID="",
     uID="",
```

### Comparing `alacorder-80.7.6/src/alacorder/alac.py` & `alacorder-80.7.7/src/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -3269,15 +3269,15 @@
     else:
         print(
             "Try again with at least one valid column header: [NAME, PARTY_TYPE, SSN, DOB, COUNTY, DIVISION, CASE_YEAR, NO_RECORDS, FILED_BEFORE, FILED_AFTER, RETRIEVED, CASES_FOUND, QUERY_COMPLETE]"
         )
         return None
 
 def crawl_adoc(path):
-    alphabet = ['AMOS', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z']
+    alphabet = ['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z']
     print("Connecting to ADOC...")
     driver = webdriver.Chrome()
     driver.get("http://www.doc.state.al.us/inmatesearch")
     results = []
     for x in alphabet:
         last_name_box = driver.find_element(by=By.NAME, value="ctl00$MainContent$txtLName")
         last_name_box.send_keys(x)
@@ -3322,15 +3322,15 @@
                 pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w (\w) \d\d\d\d').alias("Sex"),
                 pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w (\d\d\d\d)').alias("YOB").cast(pl.Int64, strict=False),
                 pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w \d\d\d\d ([A-Z\s]+)').str.strip().alias("Institution"),
                 pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w \d\d\d\d [A-Z\s]+ (\d\d/\d\d/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("ReleaseDate")
             ]
         )
         print(out)
-        alac.write(out, sheet_names=['inmates'], path=path, overwrite=True)
+        write(out, sheet_names=['inmates'], path=path, overwrite=True)
     return out
 
 def fetch(
     querypath="",
     dirpath="",
     cID="",
     uID="",
```

### Comparing `alacorder-80.7.6/PKG-INFO` & `alacorder-80.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.7.6
+Version: 80.7.7
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

