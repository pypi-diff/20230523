# Comparing `tmp/nexus-utilities-0.5.0.tar.gz` & `tmp/nexus-utilities-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexus-utilities-0.5.0.tar", last modified: Mon May 22 14:43:42 2023, max compression
+gzip compressed data, was "nexus-utilities-0.5.1.tar", last modified: Mon May 22 18:07:40 2023, max compression
```

## Comparing `nexus-utilities-0.5.0.tar` & `nexus-utilities-0.5.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:43:42.113603 nexus-utilities-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-22 14:43:31.000000 nexus-utilities-0.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-22 14:43:42.113603 nexus-utilities-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13576 2023-05-22 14:43:31.000000 nexus-utilities-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:43:42.113603 nexus-utilities-0.5.0/nexus_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-22 14:43:41.000000 nexus-utilities-0.5.0/nexus_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-22 14:43:42.000000 nexus-utilities-0.5.0/nexus_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 14:43:41.000000 nexus-utilities-0.5.0/nexus_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-22 14:43:41.000000 nexus-utilities-0.5.0/nexus_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 14:43:41.000000 nexus-utilities-0.5.0/nexus_utilities.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:43:42.113603 nexus-utilities-0.5.0/nexus_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-22 14:43:31.000000 nexus-utilities-0.5.0/nexus_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-22 14:43:31.000000 nexus-utilities-0.5.0/nexus_utils/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11114 2023-05-22 14:43:31.000000 nexus-utilities-0.5.0/nexus_utils/database_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-05-22 14:43:31.000000 nexus-utilities-0.5.0/nexus_utils/datetime_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-05-22 14:43:31.000000 nexus-utilities-0.5.0/nexus_utils/flatfile_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-22 14:43:31.000000 nexus-utilities-0.5.0/nexus_utils/package_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-22 14:43:31.000000 nexus-utilities-0.5.0/nexus_utils/password_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-22 14:43:31.000000 nexus-utilities-0.5.0/nexus_utils/string_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 14:43:42.113603 nexus-utilities-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-22 14:43:31.000000 nexus-utilities-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:07:40.804371 nexus-utilities-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-22 18:07:29.000000 nexus-utilities-0.5.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-22 18:07:40.804371 nexus-utilities-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15684 2023-05-22 18:07:29.000000 nexus-utilities-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:07:40.804371 nexus-utilities-0.5.1/nexus_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-22 18:07:40.000000 nexus-utilities-0.5.1/nexus_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-22 18:07:40.000000 nexus-utilities-0.5.1/nexus_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 18:07:40.000000 nexus-utilities-0.5.1/nexus_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-22 18:07:40.000000 nexus-utilities-0.5.1/nexus_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 18:07:40.000000 nexus-utilities-0.5.1/nexus_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:07:40.804371 nexus-utilities-0.5.1/nexus_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-22 18:07:29.000000 nexus-utilities-0.5.1/nexus_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-22 18:07:29.000000 nexus-utilities-0.5.1/nexus_utils/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11114 2023-05-22 18:07:29.000000 nexus-utilities-0.5.1/nexus_utils/database_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-05-22 18:07:29.000000 nexus-utilities-0.5.1/nexus_utils/datetime_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-05-22 18:07:29.000000 nexus-utilities-0.5.1/nexus_utils/flatfile_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-22 18:07:29.000000 nexus-utilities-0.5.1/nexus_utils/package_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-22 18:07:29.000000 nexus-utilities-0.5.1/nexus_utils/password_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-22 18:07:29.000000 nexus-utilities-0.5.1/nexus_utils/string_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 18:07:40.804371 nexus-utilities-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-22 18:07:29.000000 nexus-utilities-0.5.1/setup.py
```

### Comparing `nexus-utilities-0.5.0/LICENSE.txt` & `nexus-utilities-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.5.0/PKG-INFO` & `nexus-utilities-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-utilities
-Version: 0.5.0
+Version: 0.5.1
 Summary: Common python utilities
 Home-page: https://github.com/james-larsen/nexus-utilities
 Author: James Larsen
 Author-email: james.larsen42@gmail.com
 License: UNKNOWN
 Description: This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.
 Platform: UNKNOWN
```

### Comparing `nexus-utilities-0.5.0/README.md` & `nexus-utilities-0.5.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 - [database\_utils.py](#database_utilspy)
   - [**build\_engine(connect\_type, server\_address, server\_port, server\_name, user\_name, password, schema=None)**](#build_engineconnect_type-server_address-server_port-server_name-user_name-password-schemanone)
   - [**clean\_sql\_statement(sql\_statement)**](#clean_sql_statementsql_statement)
 - [datetime\_utils.py](#datetime_utilspy)
   - [**get\_current\_timestamp()**](#get_current_timestamp)
   - [**get\_duration(then, now=datetime.datetime.now())**](#get_durationthen-nowdatetimedatetimenow)
   - [**determine\_date\_format(date\_list)**](#determine_date_formatdate_list)
+- [flatfile\_utils.py](#flatfile_utilspy)
+  - [**detect\_encoding(file\_path)**](#detect_encodingfile_path)
+  - [**analyze\_dataframe(df)**](#analyze_dataframedf)
 - [package\_utils.py](#package_utilspy)
   - [**add\_package\_to\_path()**](#add_package_to_path)
   - [**import\_relative(package\_root\_name, module\_path, import\_name, alias=None)**](#import_relativepackage_root_name-module_path-import_name-aliasnone)
 - [password\_utils.py](#password_utilspy)
   - [**get\_password(password\_method, password\_key, account\_name=None, access\_key=None, secret\_key=None, endpoint\_url=None, region\_name=None, password\_path=None, encoding='utf-8')**](#get_passwordpassword_method-password_key-account_namenone-access_keynone-secret_keynone-endpoint_urlnone-region_namenone-password_pathnone-encodingutf-8)
 - [string\_utils.py](#string_utilspy)
   - [**cleanse\_string(string, remove\_symbols=True, title\_to\_snake\_case=False, hyphen\_to\_underscore=True, period\_to\_underscore=True, to\_upper=False, to\_lower=True)**](#cleanse_stringstring-remove_symbolstrue-title_to_snake_casefalse-hyphen_to_underscoretrue-period_to_underscoretrue-to_upperfalse-to_lowertrue)
@@ -107,38 +110,79 @@
 Returns:
  * ***days_between (int):*** Days between two timestamps
  * ***hours_between (int):*** Hours between two timestamps
  * ***minutes_between (int):*** Minutes between two timestamps
  * ***seconds_between (int):*** Seconds between two timestamps
  * ***duration_string (str):*** String representation of difference between two timestamps
 
-Calculates the difference between two timestamps.  Provides absolute number of total days, hours, minutes, and seconds, as well as a string representation of the normalized difference, Eg. "5 days, 4 hours, 3 minutes, 2 seconds" or "32 seconds"
+Calculates the difference between two timestamps.  Provides absolute number of total days, hours, minutes, and seconds, as well as a string representation of the normalized difference, Eg. "5 days, 4 hours, 3 minutes, 2 seconds" or "32 seconds".
 
 ### **determine_date_format(date_list)**
 
 Arguments:
  * ***date_list (list):*** List of dates to analyze
 
 Returns:
  * ***date_format (str):*** Determined date format in plain text (Eg. "MM/DD/YYYY")
  * ***format_string (str)*** Date format string to be passed into the Python "datetime" library (Eg. "%m/%d/%Y")
 
 Attempts to isolate the date portion of a list of string values, and return the likely format.  Some sample return values are "MM/DD/YYYY", "DD-MM-YYYY or "YYYYMMDD".  The primary value of this function is to tell MM/DD from DD/MM formats, which many more traditional means of date parsing may struggle with.
 
-A few notes:
+***Notes:***
 
 * Only delimiters supported are "-", "/" and no delimiter
 * It is assumed that all dates in a given list are the same format.  For example, the function will not work properly if a list contains both "05/06/2000" and "05-07-2000"
 * Timestamp portions are ignored
 * Only works for numerical dates.  For example, will not work with "June 5, 2000"
 * Limited support for 2 digit years
 * Requires some form of differentiation between the included dates.  For example, if all dates in the list are "05/06/2000", it will be impossible to infer the date format.  However, if it sees "05/06/2000", "05/07/2000" and "05/08/2000" in the list, it will assume a "MM/DD" format based on the limited variance in one segment, and a higher variance in another segment
 
 ---
 
+## flatfile_utils.py
+
+This module contains functions for working with flat files.
+
+### **detect_encoding(file_path)**
+
+Arguments:
+ * ***file_path (str):*** Path to flat file to read
+
+Returns:
+ * ***encoding (str):*** String representation of encoding, such as 'utf-8' or 'ascii'
+
+Attempts to detect the encoding of a flat file.  It will scan the first 2,000 records of the file.  If the result is 'ascii', it will scan the entire file to confirm.  This is to prevent a false positive of 'ascii' if a non-ascii character happens to not be present in the first 2,000 rows.
+
+### **analyze_dataframe(df)**
+
+Arguments:
+ * ***df (pandas dataframe):*** Pandas dataframe of the flat file to be analyzed
+
+Returns:
+ * ***df_results (pandas dataframe):*** Pandas dataframe representing the analysis results
+
+Performs basic field profiling for a flat file read into a pandas dataframe.  Results come in 3-column groupings:
+
+|||||||
+| :--- | :--- | :--- | :--- | :--- | :--- |
+|*{column_name_01}*|*{summary_metric}*|&nbsp;|*{column_name_02}*|*{summary_metric}*|&nbsp;|
+|Distinct Values|Occurrences|&nbsp;|Distinct Values|Occurrences|&nbsp;|
+|*{value_01}*|*{occurrence_count}*|&nbsp;|*{value_01}*|*{occurrence_count}*|&nbsp;|
+|*{value_02}*|*{occurrence_count}*|&nbsp;|*{value_02}*|*{occurrence_count}*|&nbsp;|
+|...|...|&nbsp;|*{value_03}*|*{occurrence_count}*|&nbsp;|
+|*{value_50}*|*{occurrence_count}*|&nbsp;|&nbsp;|&nbsp;|&nbsp;|
+|More than 50 distinct values|Distinct Values: *{count}*|&nbsp;|&nbsp;|&nbsp;|&nbsp;|
+|||||||
+
+***Notes:***
+ * *{summary_metric}*: Will either be "Max Length: {value}" for strings, or "Max Value: {value}" for numeric values and dates.  Can be useful for estimating field size when designing tables
+ * Will show up to 50 distinct values, sorted by number of occurrences descending.  If there are more than 50 distinct values, a note will be shown at the bottom of the list, along with the total number of distinct values
+
+---
+
 ## package_utils.py
 
 This module contains functions for working with Python packages.
 
 ### **add_package_to_path()**
 
 Arguments:
```

### Comparing `nexus-utilities-0.5.0/nexus_utilities.egg-info/PKG-INFO` & `nexus-utilities-0.5.1/nexus_utilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-utilities
-Version: 0.5.0
+Version: 0.5.1
 Summary: Common python utilities
 Home-page: https://github.com/james-larsen/nexus-utilities
 Author: James Larsen
 Author-email: james.larsen42@gmail.com
 License: UNKNOWN
 Description: This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.
 Platform: UNKNOWN
```

### Comparing `nexus-utilities-0.5.0/nexus_utils/config_utils.py` & `nexus-utilities-0.5.1/nexus_utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.5.0/nexus_utils/database_utils.py` & `nexus-utilities-0.5.1/nexus_utils/database_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.5.0/nexus_utils/datetime_utils.py` & `nexus-utilities-0.5.1/nexus_utils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.5.0/nexus_utils/flatfile_utils.py` & `nexus-utilities-0.5.1/nexus_utils/flatfile_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,32 @@
 """Flatfile-related utilities"""
 import chardet
+import pandas as pd
+from openpyxl import Workbook
 
 def detect_encoding(file_path):
     """Attempt to determine the encoding of a file located at the provided file path"""
     # Open the file in binary mode to prevent any decoding errors
     with open(file_path, 'rb') as f:
-        # Read the first 10 rows of the file
-        content = b''.join([f.readline() for _ in range(10)])
+        # Read the first 2000 rows
+        content = b''.join([f.readline() for _ in range(2000)])
         # Determine the encoding of the content
         result = chardet.detect(content)
 
-    return result['encoding']
+    encoding = result['encoding']
+
+    # If the detected encoding is ASCII, read the entire file to confirm the encoding
+    if encoding.lower() == 'ascii':
+        with open(file_path, 'r', encoding=encoding) as f:
+            content = f.read()
+            # Determine the encoding of the entire file
+            result = chardet.detect(content)
+            encoding = result['encoding']
+
+    return encoding
 
 def analyze_dataframe(df):
     """Analyze distinct values in a dataframe"""
     analysis_dict = {}
 
     for col in df.columns:
         column_dict = {}
@@ -49,26 +61,30 @@
             max_date = df[col].max()
             max_date_string = str(max_date) if not pd.isna(max_date) else ''
             column_dict['Max Size'] = f'Max Value: {max_date_string}'
             column_dict['Type'] = 'Date/Time'
 
         # Get distinct values and their counts
         col_values = df[col].copy()
+        if col_values.dtype == float:
+            col_values = col_values.apply(lambda x: "{:.10f}".format(x).rstrip('0').rstrip('.') if not pd.isna(x) else '<NULL>')
         col_values = col_values.fillna("<NULL>")
         value_counts = col_values.value_counts(dropna=False).replace({pd.NA: "<NULL>", pd.NaT: "<NULL>", "nan": "<NULL>"})
         if len(value_counts) > 50:
             # If there are more than 50 distinct values, store top 50 and "More than 50 distinct values"
             top_50_values = value_counts.nlargest(50).to_dict()
             # top_50_values['More than 50 distinct values'] = str(len(value_counts) - 50)
-            column_dict['Distinct Values'] = {str(k): str(format(int(v), ',')) if v != '' else str(v) for k, v in top_50_values.items()}
+            # column_dict['Distinct Values'] = {str(k): str(format(int(v), ',')) if v != '' else str(v) for k, v in top_50_values.items()}
+            column_dict['Distinct Values'] = {('{:.10f}'.format(k) if isinstance(k, float) else str(k)): str(v) if v != '' else str(v) for k, v in top_50_values.items()}
             # top_50_values['More than 50 distinct values'] = f'Distinct Values: {distinct_value_count_string}'
             column_dict['Distinct Values']['More than 50 distinct values'] = f'Distinct Values: {distinct_value_count_string}'
 
         else:
-            column_dict['Distinct Values'] = {str(k): str(format(int(v), ',')) if v != '' else str(v) for k, v in value_counts.items()}
+            # column_dict['Distinct Values'] = {str(k): str(format(int(v), ',')) if v != '' else str(v) for k, v in value_counts.items()}
+            column_dict['Distinct Values'] = {('{:.10f}'.format(k) if isinstance(k, float) else str(k)): str(v) if v != '' else str(v) for k, v in top_50_values.items()}
 
         # Add the column dictionary to the analysis dictionary
         analysis_dict[col] = column_dict
 
     # Create a workbook and select the active sheet
     wb = Workbook()
     ws = wb.active
```

### Comparing `nexus-utilities-0.5.0/nexus_utils/package_utils.py` & `nexus-utilities-0.5.1/nexus_utils/package_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.5.0/nexus_utils/password_utils.py` & `nexus-utilities-0.5.1/nexus_utils/password_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.5.0/nexus_utils/string_utils.py` & `nexus-utilities-0.5.1/nexus_utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.5.0/setup.py` & `nexus-utilities-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nexus-utilities',
-    version='0.5.0',
+    version='0.5.1',
     author='James Larsen',
     author_email='james.larsen42@gmail.com',
     description='Common python utilities',
     long_description='This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.',
     long_description_content_type='text/markdown',
     url='https://github.com/james-larsen/nexus-utilities',
     packages=['nexus_utils'],
```

