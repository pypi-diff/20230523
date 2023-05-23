# Comparing `tmp/mitol-django-google-sheets-refunds-0.8.0.tar.gz` & `tmp/mitol-django-google-sheets-refunds-2023.5.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitol-django-google-sheets-refunds-0.8.0.tar", last modified: Tue Jan 17 16:32:35 2023, max compression
+gzip compressed data, was "mitol-django-google-sheets-refunds-2023.5.23.tar", last modified: Tue May 23 12:08:37 2023, max compression
```

## Comparing `mitol-django-google-sheets-refunds-0.8.0.tar` & `mitol-django-google-sheets-refunds-2023.5.23.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:32:35.358613 mitol-django-google-sheets-refunds-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-01-17 16:32:34.000000 mitol-django-google-sheets-refunds-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3116 2023-01-17 16:32:35.358613 mitol-django-google-sheets-refunds-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      625 2023-01-17 16:32:34.000000 mitol-django-google-sheets-refunds-0.8.0/backend_shim.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:32:35.354613 mitol-django-google-sheets-refunds-0.8.0/mitol/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-01-17 16:32:34.000000 mitol-django-google-sheets-refunds-0.8.0/mitol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:32:35.354613 mitol-django-google-sheets-refunds-0.8.0/mitol/google_sheets_refunds/
--rw-r--r--   0 runner    (1001) docker     (122)      456 2023-01-17 16:32:34.000000 mitol-django-google-sheets-refunds-0.8.0/mitol/google_sheets_refunds/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     2577 2023-01-17 16:32:34.000000 mitol-django-google-sheets-refunds-0.8.0/mitol/google_sheets_refunds/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      198 2023-01-17 16:32:34.000000 mitol-django-google-sheets-refunds-0.8.0/mitol/google_sheets_refunds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5437 2023-01-17 16:32:34.000000 mitol-django-google-sheets-refunds-0.8.0/mitol/google_sheets_refunds/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      444 2023-01-17 16:32:34.000000 mitol-django-google-sheets-refunds-0.8.0/mitol/google_sheets_refunds/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      264 2023-01-17 16:32:34.000000 mitol-django-google-sheets-refunds-0.8.0/mitol/google_sheets_refunds/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      805 2023-01-17 16:32:34.000000 mitol-django-google-sheets-refunds-0.8.0/mitol/google_sheets_refunds/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:32:35.354613 mitol-django-google-sheets-refunds-0.8.0/mitol/google_sheets_refunds/management/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:32:35.354613 mitol-django-google-sheets-refunds-0.8.0/mitol/google_sheets_refunds/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-01-17 16:32:34.000000 mitol-django-google-sheets-refunds-0.8.0/mitol/google_sheets_refunds/management/commands/process_refund_requests.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:32:35.354613 mitol-django-google-sheets-refunds-0.8.0/mitol/google_sheets_refunds/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-01-17 16:32:34.000000 mitol-django-google-sheets-refunds-0.8.0/mitol/google_sheets_refunds/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 16:32:34.000000 mitol-django-google-sheets-refunds-0.8.0/mitol/google_sheets_refunds/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      395 2023-01-17 16:32:34.000000 mitol-django-google-sheets-refunds-0.8.0/mitol/google_sheets_refunds/models.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 16:32:34.000000 mitol-django-google-sheets-refunds-0.8.0/mitol/google_sheets_refunds/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:32:35.354613 mitol-django-google-sheets-refunds-0.8.0/mitol/google_sheets_refunds/settings/
--rw-r--r--   0 runner    (1001) docker     (122)     1896 2023-01-17 16:32:34.000000 mitol-django-google-sheets-refunds-0.8.0/mitol/google_sheets_refunds/settings/google_sheets_refunds.py
--rw-r--r--   0 runner    (1001) docker     (122)     4687 2023-01-17 16:32:34.000000 mitol-django-google-sheets-refunds-0.8.0/mitol/google_sheets_refunds/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:32:35.354613 mitol-django-google-sheets-refunds-0.8.0/mitol_django_google_sheets_refunds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3116 2023-01-17 16:32:35.000000 mitol-django-google-sheets-refunds-0.8.0/mitol_django_google_sheets_refunds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1086 2023-01-17 16:32:35.000000 mitol-django-google-sheets-refunds-0.8.0/mitol_django_google_sheets_refunds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-17 16:32:35.000000 mitol-django-google-sheets-refunds-0.8.0/mitol_django_google_sheets_refunds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-01-17 16:32:35.000000 mitol-django-google-sheets-refunds-0.8.0/mitol_django_google_sheets_refunds.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (122)      107 2023-01-17 16:32:35.000000 mitol-django-google-sheets-refunds-0.8.0/mitol_django_google_sheets_refunds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-01-17 16:32:35.000000 mitol-django-google-sheets-refunds-0.8.0/mitol_django_google_sheets_refunds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-17 16:32:35.000000 mitol-django-google-sheets-refunds-0.8.0/mitol_django_google_sheets_refunds.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-17 16:32:35.358613 mitol-django-google-sheets-refunds-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4131 2023-01-17 16:32:34.000000 mitol-django-google-sheets-refunds-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:08:37.404707 mitol-django-google-sheets-refunds-2023.5.23/
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-23 12:08:36.000000 mitol-django-google-sheets-refunds-2023.5.23/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4587 2023-05-23 12:08:37.400707 mitol-django-google-sheets-refunds-2023.5.23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      625 2023-05-23 12:08:36.000000 mitol-django-google-sheets-refunds-2023.5.23/backend_shim.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:08:37.400707 mitol-django-google-sheets-refunds-2023.5.23/mitol/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-23 12:08:36.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:08:37.400707 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/
+-rw-r--r--   0 runner    (1001) docker     (122)      872 2023-05-23 12:08:36.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     4044 2023-05-23 12:08:36.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      202 2023-05-23 12:08:36.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5437 2023-05-23 12:08:36.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      444 2023-05-23 12:08:36.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-05-23 12:08:36.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      805 2023-05-23 12:08:36.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:08:37.400707 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/management/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:08:37.400707 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-05-23 12:08:36.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/management/commands/process_refund_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:08:37.400707 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-05-23 12:08:36.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 12:08:36.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      395 2023-05-23 12:08:36.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 12:08:36.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:08:37.400707 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)     1896 2023-05-23 12:08:36.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/settings/google_sheets_refunds.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4687 2023-05-23 12:08:36.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 12:08:37.400707 mitol-django-google-sheets-refunds-2023.5.23/mitol_django_google_sheets_refunds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4587 2023-05-23 12:08:37.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol_django_google_sheets_refunds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1086 2023-05-23 12:08:37.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol_django_google_sheets_refunds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 12:08:37.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol_django_google_sheets_refunds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-23 12:08:37.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol_django_google_sheets_refunds.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-05-23 12:08:37.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol_django_google_sheets_refunds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-23 12:08:37.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol_django_google_sheets_refunds.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 12:08:37.000000 mitol-django-google-sheets-refunds-2023.5.23/mitol_django_google_sheets_refunds.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-23 12:08:37.404707 mitol-django-google-sheets-refunds-2023.5.23/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5594 2023-05-23 12:08:36.000000 mitol-django-google-sheets-refunds-2023.5.23/setup.py
```

### Comparing `mitol-django-google-sheets-refunds-0.8.0/backend_shim.py` & `mitol-django-google-sheets-refunds-2023.5.23/backend_shim.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-refunds-0.8.0/mitol/google_sheets_refunds/api.py` & `mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/api.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-refunds-0.8.0/mitol/google_sheets_refunds/hooks.py` & `mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/hooks.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-refunds-0.8.0/mitol/google_sheets_refunds/management/commands/process_refund_requests.py` & `mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/management/commands/process_refund_requests.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-refunds-0.8.0/mitol/google_sheets_refunds/migrations/0001_initial.py` & `mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-refunds-0.8.0/mitol/google_sheets_refunds/settings/google_sheets_refunds.py` & `mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/settings/google_sheets_refunds.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-refunds-0.8.0/mitol/google_sheets_refunds/utils.py` & `mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/utils.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-refunds-0.8.0/mitol_django_google_sheets_refunds.egg-info/SOURCES.txt` & `mitol-django-google-sheets-refunds-2023.5.23/mitol_django_google_sheets_refunds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-refunds-0.8.0/setup.py` & `mitol-django-google-sheets-refunds-2023.5.23/mitol/google_sheets_refunds/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,71 @@
-
-# DO NOT EDIT THIS FILE -- AUTOGENERATED BY PANTS
-# Target: src/mitol/google_sheets_refunds:mitol-django-google-sheets-refunds
-
-from setuptools import setup
-
-setup(**{
-    'authors': [
-        'MIT Office of Open Learning <mitx-devops@mit.edu>',
-    ],
-    'classifiers': [
-        'Natural Language :: English',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-    ],
-    'description': 'Library to handle Refund requests using Google Sheets integrations in Django',
-    'install_requires': (
-        'django<4.0,>=2.2.12',
-        'mitol-django-common~=2.7.0',
-        'mitol-django-google-sheets~=2.6.0',
-        'pluggy==0.13.1',
-        'setuptools',
-    ),
-    'license': 'BSD 3-Clause License',
-    'long_description': """mitol-django-google-sheets-refunds
+mitol-django-google-sheets-refunds
 ---
 
 This is the Open Learning Django Google Sheets library for handling refund requests over Google Sheets
 ### Setup
+Before you begin setting up this library make sure you set up `mitol-django-google-sheets` first. Follow the instructions [here](https://github.com/mitodl/ol-django/blob/85bea3ec5da01180ef943deb89b14d1463eb7c21/src/mitol/google_sheets/README.md).
+
+Once you have `mitol-django-google-sheets` installed, then:
+
 `pip install mitol-django-google-sheets-refunds`
 
-Add the google sheets app:
+#### In `settings.py`
 
 ```python
 INSTALLED_APPS = [
     ...
     "mitol.google_sheets_refunds.apps.GoogleSheetsRefundsApp",
 ]
 ```
 
-### Configuration
 
-#### Gather Values
+```python
+MITOL_GOOGLE_SHEETS_REFUNDS_PLUGINS = [
+    "ecommerce.plugins.RefundPlugin"
+]
+```
 
+#### In `ecommerce/plugins.py`
+```python
+from mitol.google_sheets_refunds.hooks import hookimpl
 
-1. The IDs of the refund and deferral sheets in the change of enrollment spreadsheet. These can
-    be found by opening the spreadsheet, selecting the "Refunds" or "Deferrals" worksheets, and
-    copying down the `gid` value in the URL.
-    
-    Example: 
-      > `https://docs.google.com/spreadsheets/d/abcd1234efgh5678bQFCQ7SSFBH5xHip0Gx2wPKT4fUA/edit#gid=THIS_IS_THE_WORKSHEET_ID`
-1. The index of the first row where form-driven data begins in the refund worksheet.
-    If you're starting with no data already filled in these sheets (recommended), just use the index
-    of the first non-header row. Use the row index exactly as it appears in the spreadsheet.
+class RefundPlugin:
+    @hookimpl
+    def refunds_process_request(refund_request: RefundRequestRow) -> RefundResult:
+        # TODO: look up the user/order
+        # TODO: mark the order as refunded
+        # TODO: unenroll the user
+```
+
+#### Create your google sheets folder
+The structure of the folder should look as the following:
+
+1. Spreadsheet that contains sheets with 'Refund Form Responses' and the 'Refunds' sheets, that is being processed.
+2. Request Form
+
+Ask a developer for a template folder to copy this structure.
+
+
+#### Add settings to your app
 
+Set `MITOL_GOOGLE_SHEETS_REFUNDS_REQUEST_WORKSHEET_ID` in your .env file. It is required.
 
-Set the following:
+Some settings have default values, which you might need to update, if your sheet is different.
+
+Description of settings (in addition to the ones described in `mitol-django-google-sheets`):
 
 - `MITOL_GOOGLE_SHEETS_REFUNDS_REQUEST_WORKSHEET_ID`
-  > ID of the worksheet within the refund change request spreadsheet that contains enrollment refund requests from step 2
+  > The IDs of the refund and deferral sheets in the change of enrollment spreadsheet. These can
+    be found by opening the spreadsheet, selecting the "Refunds" or "Deferrals" worksheets, and
+    copying down the `gid` value in the URL.
+    
+    Example:
+    `https://docs.google.com/spreadsheets/d/<MITOL_GOOGLE_SHEETS_ENROLLMENT_CHANGE_SHEET_ID>/edit#gid=<MITOL_GOOGLE_SHEETS_REFUNDS_REQUEST_WORKSHEET_ID>`
+
 
 - `MITOL_GOOGLE_SHEETS_REFUNDS_PROCESSOR_COL` 
   > The zero-based index of the refund change sheet column that contains the user that processed the row
 
 - `MITOL_GOOGLE_SHEETS_REFUNDS_COMPLETED_DATE_COL`
   > The zero-based index of the refund change sheet column that contains the row completion date
 
@@ -73,53 +74,39 @@
 
 - `MITOL_GOOGLE_SHEETS_REFUNDS_SKIP_ROW_COL`
   > The zero-based index of the refund change sheet column that indicates whether the row should be skipped
 
 - `MITOL_GOOGLE_SHEETS_REFUNDS_FIRST_ROW`
   > The first row (as it appears in the spreadsheet) of data that our scripts should consider processing in the refund request spreadsheet
 
-# settings.py
 
-MITOL_GOOGLE_SHEETS_REFUNDS_PLUGINS = [
-    "ecommerce.plugins.RefundPlugin"
-]
-
-# ecommerce/plugins.py
-```python
-from mitol.google_sheets_refunds import hookimpl
-
-class RefundPlugin:
-    @hookimpl
-    def refunds_process_request(refund_request: RefundRequestRow) -> RefundResult:
-        # TODO: look up the user/order
-        # TODO: mark the order as refunded
-        # TODO: unenroll the user
-```
 ### Usage
-Processing refunds
+To processing your google sheet with refund requests simply add:
 ```python
 refund_request_handler = RefundRequestHandler()
 results = refund_request_handler.process_sheet()
-```""",
-    'long_description_content_type': 'text/markdown',
-    'name': 'mitol-django-google-sheets-refunds',
-    'namespace_packages': (
-        'mitol',
-    ),
-    'package_data': {
-        'mitol.google_sheets_refunds': (
-            'CHANGELOG.md',
-            'README.md',
-            'py.typed',
-        ),
-    },
-    'packages': (
-        'mitol',
-        'mitol.google_sheets_refunds',
-        'mitol.google_sheets_refunds.management.commands',
-        'mitol.google_sheets_refunds.migrations',
-        'mitol.google_sheets_refunds.settings',
-    ),
-    'python_requires': '>=3.7',
-    'version': '0.8.0',
-    'zip_safe': True,
-})
+```
+
+
+Here are two main ways that we are currently getting our Google Sheets Refunds processed:
+
+1. Run a management command. For example:
+`./manage.py process_refund_requests -i "<spreadsheet id>"`
+2. Set up a scheduled celery task. For example:
+```python
+from mitol.google_sheets_refunds.api import RefundRequestHandler
+from main.celery import app
+
+@app.task
+def process_refund_requests():
+    """
+    Task to process refund requests from Google sheets
+    """
+    refund_request_handler = RefundRequestHandler()
+    if not refund_request_handler.is_configured():
+        log.warning("MITOL_GOOGLE_SHEETS_* are not set")
+        return
+    refund_request_handler.process_sheet()
+```
+
+### Develper setup
+For local development setup and testing please follow the instructions `Developer Setup` [here](https://github.com/mitodl/ol-django/blob/85bea3ec5da01180ef943deb89b14d1463eb7c21/src/mitol/google_sheets/README.md#developer-setup).
```

