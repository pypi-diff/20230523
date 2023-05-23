# Comparing `tmp/alacorder-80.7.4.tar.gz` & `tmp/alacorder-80.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.7.4.tar", max compression
+gzip compressed data, was "alacorder-80.7.5.tar", max compression
```

## Comparing `alacorder-80.7.4.tar` & `alacorder-80.7.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.7.4/LICENSE
--rw-r--r--   0        0        0     6455 2023-05-17 18:00:53.819885 alacorder-80.7.4/README.md
--rw-r--r--   0        0        0      746 2023-05-22 15:54:21.376314 alacorder-80.7.4/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-22 15:54:13.690662 alacorder-80.7.4/src/alacorder/.DS_Store
--rw-r--r--   0        0        0   234455 2023-05-18 23:58:39.588863 alacorder-80.7.4/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.7.4/src/alacorder/__init__.py
--rw-r--r--   0        0        0   237981 2023-05-22 15:54:01.326616 alacorder-80.7.4/src/alacorder/__main__.py
--rw-r--r--   0        0        0   237981 2023-05-22 15:53:56.041241 alacorder-80.7.4/src/alacorder/alac.py
--rw-r--r--   0        0        0     7426 1970-01-01 00:00:00.000000 alacorder-80.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.7.5/LICENSE
+-rw-r--r--   0        0        0     6455 2023-05-17 18:00:53.819885 alacorder-80.7.5/README.md
+-rw-r--r--   0        0        0      746 2023-05-23 14:32:23.303614 alacorder-80.7.5/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-23 14:31:25.922596 alacorder-80.7.5/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0   234455 2023-05-18 23:58:39.588863 alacorder-80.7.5/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.7.5/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   241431 2023-05-23 14:31:02.858041 alacorder-80.7.5/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   241431 2023-05-23 14:30:55.288548 alacorder-80.7.5/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7426 1970-01-01 00:00:00.000000 alacorder-80.7.5/PKG-INFO
```

### Comparing `alacorder-80.7.4/LICENSE` & `alacorder-80.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.7.4/README.md` & `alacorder-80.7.5/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.7.4/pyproject.toml` & `alacorder-80.7.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.7.4"
+version = "80.7.5"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.7.4/src/alacorder/.DS_Store` & `alacorder-80.7.5/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-80.7.4/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py` & `alacorder-80.7.5/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py`

 * *Files identical despite different names*

### Comparing `alacorder-80.7.4/src/alacorder/__main__.py` & `alacorder-80.7.5/src/alacorder/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 Dependencies: 
     python 3.9+, brotli ^1.0.9, click ^8.1.3,
     polars ^0.17.6, PyMuPDF ^1.21.1,
     PySimpleGUI ^4.60.4, selenium ^4.8.3, 
     tqdm ^4.65.0, xlsx2csv ^0.8.1, XlsxWriter ^3.0.9
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
-    Google Chrome required to fetch cases from Alacourt
+    Google Chrome required to fetch cases from Alacourt and crawl ADOC
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.7.4"
+version = "80.7.5"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -3268,14 +3268,70 @@
         return query
     else:
         print(
             "Try again with at least one valid column header: [NAME, PARTY_TYPE, SSN, DOB, COUNTY, DIVISION, CASE_YEAR, NO_RECORDS, FILED_BEFORE, FILED_AFTER, RETRIEVED, CASES_FOUND, QUERY_COMPLETE]"
         )
         return None
 
+def crawl_adoc(path):
+    alphabet = ['AMOS', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z']
+    print("Connecting to ADOC...")
+    driver = webdriver.Chrome()
+    driver.get("http://www.doc.state.al.us/inmatesearch")
+    results = []
+    for x in alphabet:
+        last_name_box = driver.find_element(by=By.NAME, value="ctl00$MainContent$txtLName")
+        last_name_box.send_keys(x)
+        driver.implicitly_wait(1)
+        send_button = driver.find_element(by=By.NAME, value="ctl00$MainContent$btnSearch")
+        send_button.click()
+        driver.implicitly_wait(1)
+        more_results = True
+        try:
+            while more_results:
+                driver.implicitly_wait(1)
+                lists = driver.find_elements(by=By.TAG_NAME, value="tr")
+                for x in lists:
+                    results += [x.text]
+                    print(x.text)
+                try:
+                    current_page = driver.find_element(by=By.ID, value="MainContent_gvInmateResults_lblCurrent")
+                    total_pages = driver.find_element(by=By.ID, value='MainContent_gvInmateResults_lblPages')
+                except:
+                    more_results = False
+                    search_again = driver.find_element(by=By.NAME, value="ctl00$MainContent$btnSearchAgain")
+                    search_again.click()
+                if int(current_page.text) == int(total_pages.text):
+                    more_results = False
+                    search_again = driver.find_element(by=By.NAME, value="ctl00$MainContent$btnSearchAgain")
+                    search_again.click()
+                else:
+                    next_button = driver.find_element(by=By.ID, value="MainContent_gvInmateResults_btnNext")
+                    next_button.click()
+        except:
+            time.sleep(2)
+            driver.get("http://www.doc.state.al.us/inmatesearch")
+
+        out = pl.DataFrame({'Rows': results})
+        out = out.filter(pl.col("Rows").str.contains("Inmate").is_not())
+        out = out.filter(pl.col("Rows").str.contains("Pages").is_not())
+        out = out.select(
+            [
+                pl.col("Rows").str.extract(r'^([0-9Z]{8})').alias("AIS"),
+                pl.col("Rows").str.extract(r'^[0-9Z]{8} ([A-Z]+, [A-Z\s]+?) \w \w \d\d\d\d').alias("Name"),
+                pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? (\w) \w \d\d\d\d').alias("Race"),
+                pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w (\w) \d\d\d\d').alias("Sex"),
+                pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w (\d\d\d\d)').alias("YOB").cast(pl.Int64, strict=False),
+                pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w \d\d\d\d ([A-Z\s]+)').str.strip().alias("Institution"),
+                pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w \d\d\d\d [A-Z\s]+ (\d\d/\d\d/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("ReleaseDate")
+            ]
+        )
+        print(out)
+        alac.write(out, sheet_names=['inmates'], path=path, overwrite=True)
+    return out
 
 def fetch(
     querypath="",
     dirpath="",
     cID="",
     uID="",
     pwd="",
@@ -4510,15 +4566,26 @@
     Returns:
         DataFrame: Appended archive
     """
     arc = append_archive(in_path, out_path)
     print("Completed task.")
     return arc
 
-
+@main.command(name="crawl", help="Retrieve current inmates list from ADOC")
+@click.option(
+    "--path",
+    "-out",
+    "path",
+    required=True,
+    prompt="Output table path",
+    help="Path to output table",
+    type=click.Path()
+)
+def _cli_crawl(path):
+    crawl_adoc(path)
 
 @main.command(name="fetch", help="Fetch cases from Alacourt.com")
 @click.option(
     "--input-path",
     "-in",
     "querypath",
     required=True,
```

### Comparing `alacorder-80.7.4/src/alacorder/alac.py` & `alacorder-80.7.5/src/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 Dependencies: 
     python 3.9+, brotli ^1.0.9, click ^8.1.3,
     polars ^0.17.6, PyMuPDF ^1.21.1,
     PySimpleGUI ^4.60.4, selenium ^4.8.3, 
     tqdm ^4.65.0, xlsx2csv ^0.8.1, XlsxWriter ^3.0.9
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
-    Google Chrome required to fetch cases from Alacourt
+    Google Chrome required to fetch cases from Alacourt and crawl ADOC
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.7.4"
+version = "80.7.5"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -3268,14 +3268,70 @@
         return query
     else:
         print(
             "Try again with at least one valid column header: [NAME, PARTY_TYPE, SSN, DOB, COUNTY, DIVISION, CASE_YEAR, NO_RECORDS, FILED_BEFORE, FILED_AFTER, RETRIEVED, CASES_FOUND, QUERY_COMPLETE]"
         )
         return None
 
+def crawl_adoc(path):
+    alphabet = ['AMOS', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z']
+    print("Connecting to ADOC...")
+    driver = webdriver.Chrome()
+    driver.get("http://www.doc.state.al.us/inmatesearch")
+    results = []
+    for x in alphabet:
+        last_name_box = driver.find_element(by=By.NAME, value="ctl00$MainContent$txtLName")
+        last_name_box.send_keys(x)
+        driver.implicitly_wait(1)
+        send_button = driver.find_element(by=By.NAME, value="ctl00$MainContent$btnSearch")
+        send_button.click()
+        driver.implicitly_wait(1)
+        more_results = True
+        try:
+            while more_results:
+                driver.implicitly_wait(1)
+                lists = driver.find_elements(by=By.TAG_NAME, value="tr")
+                for x in lists:
+                    results += [x.text]
+                    print(x.text)
+                try:
+                    current_page = driver.find_element(by=By.ID, value="MainContent_gvInmateResults_lblCurrent")
+                    total_pages = driver.find_element(by=By.ID, value='MainContent_gvInmateResults_lblPages')
+                except:
+                    more_results = False
+                    search_again = driver.find_element(by=By.NAME, value="ctl00$MainContent$btnSearchAgain")
+                    search_again.click()
+                if int(current_page.text) == int(total_pages.text):
+                    more_results = False
+                    search_again = driver.find_element(by=By.NAME, value="ctl00$MainContent$btnSearchAgain")
+                    search_again.click()
+                else:
+                    next_button = driver.find_element(by=By.ID, value="MainContent_gvInmateResults_btnNext")
+                    next_button.click()
+        except:
+            time.sleep(2)
+            driver.get("http://www.doc.state.al.us/inmatesearch")
+
+        out = pl.DataFrame({'Rows': results})
+        out = out.filter(pl.col("Rows").str.contains("Inmate").is_not())
+        out = out.filter(pl.col("Rows").str.contains("Pages").is_not())
+        out = out.select(
+            [
+                pl.col("Rows").str.extract(r'^([0-9Z]{8})').alias("AIS"),
+                pl.col("Rows").str.extract(r'^[0-9Z]{8} ([A-Z]+, [A-Z\s]+?) \w \w \d\d\d\d').alias("Name"),
+                pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? (\w) \w \d\d\d\d').alias("Race"),
+                pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w (\w) \d\d\d\d').alias("Sex"),
+                pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w (\d\d\d\d)').alias("YOB").cast(pl.Int64, strict=False),
+                pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w \d\d\d\d ([A-Z\s]+)').str.strip().alias("Institution"),
+                pl.col("Rows").str.extract(r'^[0-9Z]{8} [A-Z]+, [A-Z\s]+? \w \w \d\d\d\d [A-Z\s]+ (\d\d/\d\d/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("ReleaseDate")
+            ]
+        )
+        print(out)
+        alac.write(out, sheet_names=['inmates'], path=path, overwrite=True)
+    return out
 
 def fetch(
     querypath="",
     dirpath="",
     cID="",
     uID="",
     pwd="",
@@ -4510,15 +4566,26 @@
     Returns:
         DataFrame: Appended archive
     """
     arc = append_archive(in_path, out_path)
     print("Completed task.")
     return arc
 
-
+@main.command(name="crawl", help="Retrieve current inmates list from ADOC")
+@click.option(
+    "--path",
+    "-out",
+    "path",
+    required=True,
+    prompt="Output table path",
+    help="Path to output table",
+    type=click.Path()
+)
+def _cli_crawl(path):
+    crawl_adoc(path)
 
 @main.command(name="fetch", help="Fetch cases from Alacourt.com")
 @click.option(
     "--input-path",
     "-in",
     "querypath",
     required=True,
```

### Comparing `alacorder-80.7.4/PKG-INFO` & `alacorder-80.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.7.4
+Version: 80.7.5
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

