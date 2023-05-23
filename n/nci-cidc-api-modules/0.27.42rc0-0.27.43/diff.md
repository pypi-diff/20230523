# Comparing `tmp/nci_cidc_api_modules-0.27.42rc0.tar.gz` & `tmp/nci_cidc_api_modules-0.27.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/cidc-api-gae/cidc-api-gae/dist/.tmp-7xdq6_e9/nci_cidc_api_modules-0.27.42rc0.tar", last modified: Fri May  5 14:16:32 2023, max compression
+gzip compressed data, was "/home/runner/work/cidc-api-gae/cidc-api-gae/dist/.tmp-hyr3rb8v/nci_cidc_api_modules-0.27.43.tar", last modified: Tue May 23 17:43:32 2023, max compression
```

## Comparing `nci_cidc_api_modules-0.27.42rc0.tar` & `nci_cidc_api_modules-0.27.43.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:16:32.000000 nci_cidc_api_modules-0.27.42rc0/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    35182 2023-05-05 14:16:32.000000 nci_cidc_api_modules-0.27.42rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    34873 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:16:32.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:16:32.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/config/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/config/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/config/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/config/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/config/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:16:32.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/csms/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/csms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/csms/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:16:32.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/models/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31379 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/models/csms_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:16:32.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/models/files/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/models/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62285 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/models/files/details.py
--rw-r--r--   0 runner    (1001) docker     (123)    28653 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/models/files/facets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/models/migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)   100053 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/models/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:16:32.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/shared/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11474 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/shared/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/shared/emails.py
--rw-r--r--   0 runner    (1001) docker     (123)    32533 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/shared/gcloud_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/cidc_api/shared/rest_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:16:32.000000 nci_cidc_api_modules-0.27.42rc0/nci_cidc_api_modules.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    35182 2023-05-05 14:16:32.000000 nci_cidc_api_modules-0.27.42rc0/nci_cidc_api_modules.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-05 14:16:32.000000 nci_cidc_api_modules-0.27.42rc0/nci_cidc_api_modules.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 14:16:32.000000 nci_cidc_api_modules-0.27.42rc0/nci_cidc_api_modules.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 14:16:32.000000 nci_cidc_api_modules-0.27.42rc0/nci_cidc_api_modules.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-05 14:16:32.000000 nci_cidc_api_modules-0.27.42rc0/nci_cidc_api_modules.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 14:16:32.000000 nci_cidc_api_modules-0.27.42rc0/nci_cidc_api_modules.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/requirements.modules.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 14:16:32.000000 nci_cidc_api_modules-0.27.42rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:16:32.000000 nci_cidc_api_modules-0.27.42rc0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17108 2023-05-05 14:16:22.000000 nci_cidc_api_modules-0.27.42rc0/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:43:32.000000 nci_cidc_api_modules-0.27.43/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    35145 2023-05-23 17:43:32.000000 nci_cidc_api_modules-0.27.43/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    34839 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:43:32.000000 nci_cidc_api_modules-0.27.43/cidc_api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:43:32.000000 nci_cidc_api_modules-0.27.43/cidc_api/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/config/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/config/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/config/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/config/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:43:32.000000 nci_cidc_api_modules-0.27.43/cidc_api/csms/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/csms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/csms/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:43:32.000000 nci_cidc_api_modules-0.27.43/cidc_api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31379 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/models/csms_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:43:32.000000 nci_cidc_api_modules-0.27.43/cidc_api/models/files/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/models/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63004 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/models/files/details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28653 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/models/files/facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/models/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100053 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/models/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:43:32.000000 nci_cidc_api_modules-0.27.43/cidc_api/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11474 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/shared/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/shared/emails.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32533 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/shared/gcloud_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/shared/rest_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:43:32.000000 nci_cidc_api_modules-0.27.43/nci_cidc_api_modules.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    35145 2023-05-23 17:43:32.000000 nci_cidc_api_modules-0.27.43/nci_cidc_api_modules.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-23 17:43:32.000000 nci_cidc_api_modules-0.27.43/nci_cidc_api_modules.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:43:32.000000 nci_cidc_api_modules-0.27.43/nci_cidc_api_modules.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:43:32.000000 nci_cidc_api_modules-0.27.43/nci_cidc_api_modules.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-23 17:43:32.000000 nci_cidc_api_modules-0.27.43/nci_cidc_api_modules.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 17:43:32.000000 nci_cidc_api_modules-0.27.43/nci_cidc_api_modules.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/requirements.modules.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 17:43:32.000000 nci_cidc_api_modules-0.27.43/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:43:32.000000 nci_cidc_api_modules-0.27.43/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17108 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/tests/test_api.py
```

### Comparing `nci_cidc_api_modules-0.27.42rc0/LICENSE` & `nci_cidc_api_modules-0.27.43/LICENSE`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.42rc0/PKG-INFO` & `nci_cidc_api_modules-0.27.43/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nci_cidc_api_modules
-Version: 0.27.42rc0
+Version: 0.27.43
 Summary: SQLAlchemy data models and configuration tools used in the NCI CIDC API
 Home-page: https://github.com/NCI-CIDC/cidc-api-gae
 License: MIT license
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -236,19 +236,19 @@
 gcloud app deploy <app.staging.yaml or app.prod.yaml> --project <gcloud project id>
 ```
 
 That being said, avoid doing this! Deploying this way circumvents the safety checks built into the CI/CD pipeline and can lead to inconsistencies between the code running on GAE and the code present in this repository. Luckily, though, GAE's built-in versioning system makes it hard to do anything catastrophic :-)
 
 ## Connecting to the API
 
-Currently, the staging API is hosted at https://staging-api.cimac-network.org and the production instance is hosted at https://api.cimac-network.org.
+Currently, the staging API is hosted at https://api.cidc-stage.nci.nih.gov and the production instance is hosted at https://api.cidc.nci.nih.gov.
 
-To connect to the staging API with `curl` or a REST API client like Insomnia, get an id token from stagingportal.cimac-network.org, and include the header `Authorization: Bearer YOUR_ID_TOKEN` in requests you make to the staging API. If your token expires, generate a new one following this same procedure.
+To connect to the staging API with `curl` or a REST API client like Insomnia, get an id token from cidc-stage.nci.nih.gov, and include the header `Authorization: Bearer YOUR_ID_TOKEN` in requests you make to the staging API. If your token expires, generate a new one following this same procedure.
 
-To connect to the production API locally, follow the same procedure, but instead get your token from portal.cimac-network.org.
+To connect to the production API locally, follow the same procedure, but instead get your token from cidc.nci.nih.gov.
 
 ## Provisioning the system from scratch
 
 For an overview of how to set up the CIDC API service from scratch, see the step-by-step guide in `PROVISION.md`.
 
 ## JIRA Integration
 
@@ -275,15 +275,15 @@
 
 [The migrations/versions directory](https://github.com/NCI-CIDC/cidc-api-gae/tree/master/migrations/versions) contains SQLAlchemy database migrations generated using flask-sqlalchemy.
 
 The core API code lives in a python module in the [cidc_api](https://github.com/NCI-CIDC/cidc-api-gae/tree/master/cidc_api) subdirectory. In this subdirectory, the [app.py](https://github.com/NCI-CIDC/cidc-api-gae/blob/master/cidc_api/app.py) file contains the code that instantiates/exports the API’s flask app. Stepping through that file top to bottom is probably the best way to get an overall picture of the structure of the API code:
 
 - [get_logger](https://github.com/NCI-CIDC/cidc-api-gae/blob/1de8b59e87eb71a3f8f8e997225e81d6b04b73fd/cidc_api/config/logging.py#L11) instantiates a logger instance based on whether the app is running in a flask development server or gunicorn production server. We need this helper function (or something like it), because logs must be routed in a particular manner for them to show up in stderr when the app is running as a gunicorn server. Any python file in the cidc_api module that includes logging should call this get_logger helper at the top of the file.
 - Next, the Flask app instance is created and configured using settings loaded from [settings.py](https://github.com/NCI-CIDC/cidc-api-gae/blob/master/cidc_api/config/settings.py). This file contains a handful of constants used throughout the app code. Additionally, it contains code for [setting up the temporary directories](https://github.com/NCI-CIDC/cidc-api-gae/blob/001e12ac276a9632260fbddd54419cbcb8a5e2b5/cidc_api/config/settings.py#L37) where empty manifest/assay/analysis templates will live. [This line](https://github.com/NCI-CIDC/cidc-api-gae/blob/001e12ac276a9632260fbddd54419cbcb8a5e2b5/cidc_api/config/settings.py#L118) at the bottom of the file builds a settings dictionary mapping variable names to values for all constants (i.e., uppercase variables) defined above it.
-- Next, [CORS](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS) is enabled. CORS allows the API to respond to requests originating from domains other than the API’s domain. If we didn’t do this, then an API instance running at “api.cimac-network.org” would be prohibited from responding to requests from a UI instance running at “portal.cimac-network.org”.
+- Next, [CORS](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS) is enabled. CORS allows the API to respond to requests originating from domains other than the API’s domain. If we didn’t do this, then an API instance running at “api.cidc.nci.nih.gov” would be prohibited from responding to requests from a UI instance running at “cidc.nci.nih.gov”.
 - Next, [init_db](https://github.com/NCI-CIDC/cidc-api-gae/blob/1de8b59e87eb71a3f8f8e997225e81d6b04b73fd/cidc_api/config/db.py#L17) connects the flask-sqlalchemy package to a given API app instance. Moreover, it sets up our database migration utility, [flask-migrate](https://flask-migrate.readthedocs.io/en/latest/), which provides CLI shortcuts for generating migrations based on changes to the API’s sqlalchemy models. Currently, db migrations are [run every time init_db is called](https://github.com/NCI-CIDC/cidc-api-gae/blob/1de8b59e87eb71a3f8f8e997225e81d6b04b73fd/cidc_api/config/db.py#L23), but this is arguably tech debt, since it slows down app startup for no good reason - it might be better to try running db migrations as part of CI. (All other code in this file is related to building database connections based on the environment in which the app is running).
 - Next, [register_resources](https://github.com/NCI-CIDC/cidc-api-gae/blob/1de8b59e87eb71a3f8f8e997225e81d6b04b73fd/cidc_api/resources/__init__.py#L12) “wires up” all of the REST resources in the API, which are organized as independent flask [blueprints](https://flask.palletsprojects.com/en/2.0.x/blueprints/). Each resource blueprint is a collection of flask endpoints. Resources are split up into separate blueprints solely for code organization purposes.
 - Next, [validate_api_auth](https://github.com/NCI-CIDC/cidc-api-gae/blob/1de8b59e87eb71a3f8f8e997225e81d6b04b73fd/cidc_api/shared/auth.py#L17) enforces that all endpoints configured in the API are explicitly flagged as public or private using the [public](https://github.com/NCI-CIDC/cidc-api-gae/blob/1de8b59e87eb71a3f8f8e997225e81d6b04b73fd/cidc_api/shared/auth.py#L75) and [requires_auth](https://github.com/NCI-CIDC/cidc-api-gae/blob/1de8b59e87eb71a3f8f8e997225e81d6b04b73fd/cidc_api/shared/auth.py#L34) decorators, respectively. This is intended to help prevent a developer from accidentally making a private endpoint public by forgetting to include the requires_auth decorator. If this validation check fails, the app won’t start up.
 - Next, [register_dashboards](https://github.com/NCI-CIDC/cidc-api-gae/blob/1de8b59e87eb71a3f8f8e997225e81d6b04b73fd/cidc_api/dashboards/__init__.py#L6) wires up our plot.ly dash dashboards.
 - Next, [handle_errors](https://github.com/NCI-CIDC/cidc-api-gae/blob/1de8b59e87eb71a3f8f8e997225e81d6b04b73fd/cidc_api/app.py#L37) adds generic code for formatting any error thrown while a request is being handled as JSON.
 - Finally, if the app submodule is being run directly via “python -m cidc_api.app”, [this code](https://github.com/NCI-CIDC/cidc-api-gae/blob/1de8b59e87eb71a3f8f8e997225e81d6b04b73fd/cidc_api/app.py#L65) will start a flask (non-gunicorn) server.
 
@@ -349,25 +349,25 @@
 
 **Note:** although flask-migrate and alembic, the tool flask-migrate uses under the hood, can automatically pick up certain sqlalchemy model class changes (e.g., adding/removing models, adding/removing columns, column data type changes), there are other changes that it can’t pick up automatically. Two examples I’ve encountered are adding/removing values from enum types and adding/updating [CHECK constraints](https://docs.sqlalchemy.org/en/14/core/constraints.html#check-constraint). For this reason, always review the auto-generated migration file before applying it, making any required manually edits/additions.
 
 #### How can I check that a database migration works?
 
 First, I run the “flask db upgrade” against my local database - this can catch basic errors, like syntax or type issues, even if there’s no data currently stored in the local database.
 
-Next, I’ll try running the migration against the staging database from my local computer (since the staging db generally has representative data in it, this can catch further errors you might miss in a local db test). To do this, you need to [set up a connection to the staging db](https://github.com/cimac-cidc/cidc-api-gae#connecting-to-a-cloud-sql-database-instance) and to [update your .env file](https://github.com/NCI-CIDC/cidc-api-gae/blob/75e88280e1103b530f6e7bd7261ca90f933159b2/.env#L23) to tell your local api code to use this connection. **Make sure that no one else is using the staging db for anything critical**, then run the db upgrade. If you encounter new errors, fix them. Once the upgrade succeeds, undo it with “flask db downgrade”, then make a PR to deploy the new migration.
+Next, I’ll try running the migration against the staging database from my local computer (since the staging db generally has representative data in it, this can catch further errors you might miss in a local db test). To do this, you need to [set up a connection to the staging db](https://github.com/nci-cidc/cidc-api-gae#connecting-to-a-cloud-sql-database-instance) and to [update your .env file](https://github.com/NCI-CIDC/cidc-api-gae/blob/75e88280e1103b530f6e7bd7261ca90f933159b2/.env#L23) to tell your local api code to use this connection. **Make sure that no one else is using the staging db for anything critical**, then run the db upgrade. If you encounter new errors, fix them. Once the upgrade succeeds, undo it with “flask db downgrade”, then make a PR to deploy the new migration.
 
 #### What happens when a database migration fails, and what should I do to remediate the situation?
 
 Because database migrations are run when the app starts up, failed database migrations manifest as the API failing to start up. This usually looks like the “failed to load account information” error message appearing 5-10 seconds after trying to load the portal.
 
 Remediating a failing migration requires two steps:
 
 1. Redirect traffic to a previous app engine version that does not include the failing migration code. You can select a known-good version from [this page](https://console.cloud.google.com/appengine/versions) in the GCP console.
 2. Debug and fix the migration locally following a process like the one described above.
 
-**Note:** when you want to undo a migration that **did not fail to run**, but has some other issue with it, the solution is different. If you try to simply send traffic to a previous app engine version without the migration you want to undo included in it, you’ll get an error on app startup (something like “alembic.util.CommandError: Can't locate revision identified by '31b8ab83c7d'”). In order to undo this migration, you’ll need to [manually connect to the cloud sql instance](https://github.com/cimac-cidc/cidc-api-gae#connecting-to-a-cloud-sql-database-instance), [update your .env file](https://github.com/NCI-CIDC/cidc-api-gae/blob/75e88280e1103b530f6e7bd7261ca90f933159b2/.env#L23) to tell your local api code to use this connection, then run “flask db downgrade”. Once that command succeeds, you’ve rolled back the unwanted migration, and you can safely send traffic to a previous app engine version that doesn’t include the migration.
+**Note:** when you want to undo a migration that **did not fail to run**, but has some other issue with it, the solution is different. If you try to simply send traffic to a previous app engine version without the migration you want to undo included in it, you’ll get an error on app startup (something like “alembic.util.CommandError: Can't locate revision identified by '31b8ab83c7d'”). In order to undo this migration, you’ll need to [manually connect to the cloud sql instance](https://github.com/nci-cidc/cidc-api-gae#connecting-to-a-cloud-sql-database-instance), [update your .env file](https://github.com/NCI-CIDC/cidc-api-gae/blob/75e88280e1103b530f6e7bd7261ca90f933159b2/.env#L23) to tell your local api code to use this connection, then run “flask db downgrade”. Once that command succeeds, you’ve rolled back the unwanted migration, and you can safely send traffic to a previous app engine version that doesn’t include the migration.
 
 #### What’s packaged up in cidc-api-modules pypi package?
 
 The cidc-api-modules package includes only the submodules used in the cidc-cloud-functions module. Here’s the [full list](https://github.com/NCI-CIDC/cidc-api-gae/blob/ed18274bd413444157fb3d7af8e0dc3925079e6a/setup.py#L14). Notably, the “cidc_api.app” and “cidc_api.resources” submodules are excluded, since these pertain only to the API. To be perfectly honest, I don’t remember the issue that led to the decision to not simply package up and public the top-level “cidc_api” module (it’s possible even if it’s not necessary). Anyhow, this means that bumping the cidc-api-modules version is only necessary when making changes to the included submodules that you want to propagate to the cloud functions repo.
 
 Relatedly, it could be worth looking into combining the cloud functions repo into the cidc-api-gae repo. There’s no great reason for them to be separate. In fact, since they share code related to interacting with the database and with GCP, the decision to separate the two repos likely creates more friction than it alleviates.
```

### Comparing `nci_cidc_api_modules-0.27.42rc0/README.md` & `nci_cidc_api_modules-0.27.43/nci_cidc_api_modules.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: nci-cidc-api-modules
+Version: 0.27.43
+Summary: SQLAlchemy data models and configuration tools used in the NCI CIDC API
+Home-page: https://github.com/NCI-CIDC/cidc-api-gae
+License: MIT license
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # NCI CIDC API <!-- omit in TOC -->
 
 The next generation of the CIDC API, reworked to use Google Cloud-managed services. This API is built with the Flask REST API framework backed by Google Cloud SQL, running on Google App Engine.
 
 ## Development <!-- omit in TOC -->
 
 - [Install Python dependencies](#install-python-dependencies)
@@ -226,19 +236,19 @@
 gcloud app deploy <app.staging.yaml or app.prod.yaml> --project <gcloud project id>
 ```
 
 That being said, avoid doing this! Deploying this way circumvents the safety checks built into the CI/CD pipeline and can lead to inconsistencies between the code running on GAE and the code present in this repository. Luckily, though, GAE's built-in versioning system makes it hard to do anything catastrophic :-)
 
 ## Connecting to the API
 
-Currently, the staging API is hosted at https://staging-api.cimac-network.org and the production instance is hosted at https://api.cimac-network.org.
+Currently, the staging API is hosted at https://api.cidc-stage.nci.nih.gov and the production instance is hosted at https://api.cidc.nci.nih.gov.
 
-To connect to the staging API with `curl` or a REST API client like Insomnia, get an id token from stagingportal.cimac-network.org, and include the header `Authorization: Bearer YOUR_ID_TOKEN` in requests you make to the staging API. If your token expires, generate a new one following this same procedure.
+To connect to the staging API with `curl` or a REST API client like Insomnia, get an id token from cidc-stage.nci.nih.gov, and include the header `Authorization: Bearer YOUR_ID_TOKEN` in requests you make to the staging API. If your token expires, generate a new one following this same procedure.
 
-To connect to the production API locally, follow the same procedure, but instead get your token from portal.cimac-network.org.
+To connect to the production API locally, follow the same procedure, but instead get your token from cidc.nci.nih.gov.
 
 ## Provisioning the system from scratch
 
 For an overview of how to set up the CIDC API service from scratch, see the step-by-step guide in `PROVISION.md`.
 
 ## JIRA Integration
 
@@ -265,15 +275,15 @@
 
 [The migrations/versions directory](https://github.com/NCI-CIDC/cidc-api-gae/tree/master/migrations/versions) contains SQLAlchemy database migrations generated using flask-sqlalchemy.
 
 The core API code lives in a python module in the [cidc_api](https://github.com/NCI-CIDC/cidc-api-gae/tree/master/cidc_api) subdirectory. In this subdirectory, the [app.py](https://github.com/NCI-CIDC/cidc-api-gae/blob/master/cidc_api/app.py) file contains the code that instantiates/exports the API’s flask app. Stepping through that file top to bottom is probably the best way to get an overall picture of the structure of the API code:
 
 - [get_logger](https://github.com/NCI-CIDC/cidc-api-gae/blob/1de8b59e87eb71a3f8f8e997225e81d6b04b73fd/cidc_api/config/logging.py#L11) instantiates a logger instance based on whether the app is running in a flask development server or gunicorn production server. We need this helper function (or something like it), because logs must be routed in a particular manner for them to show up in stderr when the app is running as a gunicorn server. Any python file in the cidc_api module that includes logging should call this get_logger helper at the top of the file.
 - Next, the Flask app instance is created and configured using settings loaded from [settings.py](https://github.com/NCI-CIDC/cidc-api-gae/blob/master/cidc_api/config/settings.py). This file contains a handful of constants used throughout the app code. Additionally, it contains code for [setting up the temporary directories](https://github.com/NCI-CIDC/cidc-api-gae/blob/001e12ac276a9632260fbddd54419cbcb8a5e2b5/cidc_api/config/settings.py#L37) where empty manifest/assay/analysis templates will live. [This line](https://github.com/NCI-CIDC/cidc-api-gae/blob/001e12ac276a9632260fbddd54419cbcb8a5e2b5/cidc_api/config/settings.py#L118) at the bottom of the file builds a settings dictionary mapping variable names to values for all constants (i.e., uppercase variables) defined above it.
-- Next, [CORS](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS) is enabled. CORS allows the API to respond to requests originating from domains other than the API’s domain. If we didn’t do this, then an API instance running at “api.cimac-network.org” would be prohibited from responding to requests from a UI instance running at “portal.cimac-network.org”.
+- Next, [CORS](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS) is enabled. CORS allows the API to respond to requests originating from domains other than the API’s domain. If we didn’t do this, then an API instance running at “api.cidc.nci.nih.gov” would be prohibited from responding to requests from a UI instance running at “cidc.nci.nih.gov”.
 - Next, [init_db](https://github.com/NCI-CIDC/cidc-api-gae/blob/1de8b59e87eb71a3f8f8e997225e81d6b04b73fd/cidc_api/config/db.py#L17) connects the flask-sqlalchemy package to a given API app instance. Moreover, it sets up our database migration utility, [flask-migrate](https://flask-migrate.readthedocs.io/en/latest/), which provides CLI shortcuts for generating migrations based on changes to the API’s sqlalchemy models. Currently, db migrations are [run every time init_db is called](https://github.com/NCI-CIDC/cidc-api-gae/blob/1de8b59e87eb71a3f8f8e997225e81d6b04b73fd/cidc_api/config/db.py#L23), but this is arguably tech debt, since it slows down app startup for no good reason - it might be better to try running db migrations as part of CI. (All other code in this file is related to building database connections based on the environment in which the app is running).
 - Next, [register_resources](https://github.com/NCI-CIDC/cidc-api-gae/blob/1de8b59e87eb71a3f8f8e997225e81d6b04b73fd/cidc_api/resources/__init__.py#L12) “wires up” all of the REST resources in the API, which are organized as independent flask [blueprints](https://flask.palletsprojects.com/en/2.0.x/blueprints/). Each resource blueprint is a collection of flask endpoints. Resources are split up into separate blueprints solely for code organization purposes.
 - Next, [validate_api_auth](https://github.com/NCI-CIDC/cidc-api-gae/blob/1de8b59e87eb71a3f8f8e997225e81d6b04b73fd/cidc_api/shared/auth.py#L17) enforces that all endpoints configured in the API are explicitly flagged as public or private using the [public](https://github.com/NCI-CIDC/cidc-api-gae/blob/1de8b59e87eb71a3f8f8e997225e81d6b04b73fd/cidc_api/shared/auth.py#L75) and [requires_auth](https://github.com/NCI-CIDC/cidc-api-gae/blob/1de8b59e87eb71a3f8f8e997225e81d6b04b73fd/cidc_api/shared/auth.py#L34) decorators, respectively. This is intended to help prevent a developer from accidentally making a private endpoint public by forgetting to include the requires_auth decorator. If this validation check fails, the app won’t start up.
 - Next, [register_dashboards](https://github.com/NCI-CIDC/cidc-api-gae/blob/1de8b59e87eb71a3f8f8e997225e81d6b04b73fd/cidc_api/dashboards/__init__.py#L6) wires up our plot.ly dash dashboards.
 - Next, [handle_errors](https://github.com/NCI-CIDC/cidc-api-gae/blob/1de8b59e87eb71a3f8f8e997225e81d6b04b73fd/cidc_api/app.py#L37) adds generic code for formatting any error thrown while a request is being handled as JSON.
 - Finally, if the app submodule is being run directly via “python -m cidc_api.app”, [this code](https://github.com/NCI-CIDC/cidc-api-gae/blob/1de8b59e87eb71a3f8f8e997225e81d6b04b73fd/cidc_api/app.py#L65) will start a flask (non-gunicorn) server.
 
@@ -339,25 +349,25 @@
 
 **Note:** although flask-migrate and alembic, the tool flask-migrate uses under the hood, can automatically pick up certain sqlalchemy model class changes (e.g., adding/removing models, adding/removing columns, column data type changes), there are other changes that it can’t pick up automatically. Two examples I’ve encountered are adding/removing values from enum types and adding/updating [CHECK constraints](https://docs.sqlalchemy.org/en/14/core/constraints.html#check-constraint). For this reason, always review the auto-generated migration file before applying it, making any required manually edits/additions.
 
 #### How can I check that a database migration works?
 
 First, I run the “flask db upgrade” against my local database - this can catch basic errors, like syntax or type issues, even if there’s no data currently stored in the local database.
 
-Next, I’ll try running the migration against the staging database from my local computer (since the staging db generally has representative data in it, this can catch further errors you might miss in a local db test). To do this, you need to [set up a connection to the staging db](https://github.com/cimac-cidc/cidc-api-gae#connecting-to-a-cloud-sql-database-instance) and to [update your .env file](https://github.com/NCI-CIDC/cidc-api-gae/blob/75e88280e1103b530f6e7bd7261ca90f933159b2/.env#L23) to tell your local api code to use this connection. **Make sure that no one else is using the staging db for anything critical**, then run the db upgrade. If you encounter new errors, fix them. Once the upgrade succeeds, undo it with “flask db downgrade”, then make a PR to deploy the new migration.
+Next, I’ll try running the migration against the staging database from my local computer (since the staging db generally has representative data in it, this can catch further errors you might miss in a local db test). To do this, you need to [set up a connection to the staging db](https://github.com/nci-cidc/cidc-api-gae#connecting-to-a-cloud-sql-database-instance) and to [update your .env file](https://github.com/NCI-CIDC/cidc-api-gae/blob/75e88280e1103b530f6e7bd7261ca90f933159b2/.env#L23) to tell your local api code to use this connection. **Make sure that no one else is using the staging db for anything critical**, then run the db upgrade. If you encounter new errors, fix them. Once the upgrade succeeds, undo it with “flask db downgrade”, then make a PR to deploy the new migration.
 
 #### What happens when a database migration fails, and what should I do to remediate the situation?
 
 Because database migrations are run when the app starts up, failed database migrations manifest as the API failing to start up. This usually looks like the “failed to load account information” error message appearing 5-10 seconds after trying to load the portal.
 
 Remediating a failing migration requires two steps:
 
 1. Redirect traffic to a previous app engine version that does not include the failing migration code. You can select a known-good version from [this page](https://console.cloud.google.com/appengine/versions) in the GCP console.
 2. Debug and fix the migration locally following a process like the one described above.
 
-**Note:** when you want to undo a migration that **did not fail to run**, but has some other issue with it, the solution is different. If you try to simply send traffic to a previous app engine version without the migration you want to undo included in it, you’ll get an error on app startup (something like “alembic.util.CommandError: Can't locate revision identified by '31b8ab83c7d'”). In order to undo this migration, you’ll need to [manually connect to the cloud sql instance](https://github.com/cimac-cidc/cidc-api-gae#connecting-to-a-cloud-sql-database-instance), [update your .env file](https://github.com/NCI-CIDC/cidc-api-gae/blob/75e88280e1103b530f6e7bd7261ca90f933159b2/.env#L23) to tell your local api code to use this connection, then run “flask db downgrade”. Once that command succeeds, you’ve rolled back the unwanted migration, and you can safely send traffic to a previous app engine version that doesn’t include the migration.
+**Note:** when you want to undo a migration that **did not fail to run**, but has some other issue with it, the solution is different. If you try to simply send traffic to a previous app engine version without the migration you want to undo included in it, you’ll get an error on app startup (something like “alembic.util.CommandError: Can't locate revision identified by '31b8ab83c7d'”). In order to undo this migration, you’ll need to [manually connect to the cloud sql instance](https://github.com/nci-cidc/cidc-api-gae#connecting-to-a-cloud-sql-database-instance), [update your .env file](https://github.com/NCI-CIDC/cidc-api-gae/blob/75e88280e1103b530f6e7bd7261ca90f933159b2/.env#L23) to tell your local api code to use this connection, then run “flask db downgrade”. Once that command succeeds, you’ve rolled back the unwanted migration, and you can safely send traffic to a previous app engine version that doesn’t include the migration.
 
 #### What’s packaged up in cidc-api-modules pypi package?
 
 The cidc-api-modules package includes only the submodules used in the cidc-cloud-functions module. Here’s the [full list](https://github.com/NCI-CIDC/cidc-api-gae/blob/ed18274bd413444157fb3d7af8e0dc3925079e6a/setup.py#L14). Notably, the “cidc_api.app” and “cidc_api.resources” submodules are excluded, since these pertain only to the API. To be perfectly honest, I don’t remember the issue that led to the decision to not simply package up and public the top-level “cidc_api” module (it’s possible even if it’s not necessary). Anyhow, this means that bumping the cidc-api-modules version is only necessary when making changes to the included submodules that you want to propagate to the cloud functions repo.
 
 Relatedly, it could be worth looking into combining the cloud functions repo into the cidc-api-gae repo. There’s no great reason for them to be separate. In fact, since they share code related to interacting with the database and with GCP, the decision to separate the two repos likely creates more friction than it alleviates.
```

### Comparing `nci_cidc_api_modules-0.27.42rc0/cidc_api/config/db.py` & `nci_cidc_api_modules-0.27.43/cidc_api/config/db.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.42rc0/cidc_api/config/logging.py` & `nci_cidc_api_modules-0.27.43/cidc_api/config/logging.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.42rc0/cidc_api/config/secrets.py` & `nci_cidc_api_modules-0.27.43/cidc_api/config/secrets.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.42rc0/cidc_api/config/settings.py` & `nci_cidc_api_modules-0.27.43/cidc_api/config/settings.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.42rc0/cidc_api/csms/auth.py` & `nci_cidc_api_modules-0.27.43/cidc_api/csms/auth.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.42rc0/cidc_api/models/csms_api.py` & `nci_cidc_api_modules-0.27.43/cidc_api/models/csms_api.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.42rc0/cidc_api/models/files/details.py` & `nci_cidc_api_modules-0.27.43/cidc_api/models/files/details.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         "The gzipped, FASTQ file that represents the 3' read of paired sequencing. Generated by the sequencing machine defined by the RNA assay this file is associated with.",
     ),
     "/wes/reads_.bam": FileDetails(
         "source",
         "bam file containing both pairs of sequencing libraries",
         "The paired raw reads in the standard BAM binary format, generated from the raw R1 and R2 FASTQ files.",
     ),
-    ## see: https://github.com/CIMAC-CIDC/cidc-ngs-pipeline-api/blob/master/cidc_ngs_pipeline_api/wes/wes_output_API.json
+    ## see: https://github.com/NCI-CIDC/cidc-ngs-pipeline-api/blob/master/cidc_ngs_pipeline_api/wes/wes_output_API.json
     "/wes/analysis/error.yaml": FileDetails(
         "analysis",
         "yaml file that specifies error codes for files",
         "Explanation of all files which are expected to be empty due to a failed/missing module.",
     ),
     "/wes/analysis/copynumber_segments.txt": FileDetails(
         "analysis",
@@ -170,25 +170,25 @@
         "analysis",
         "somatic variants: vcf file of somatic variants in TWIST targed capture region",
         "VCF file of variants that fall within the TWIST excome capture regions.  bcftools is used to filter reads in output.vcf.gz that intersect with the TWIST capture regions.",
     ),
     "/wes/analysis/tnscope_output_twist.maf": FileDetails(
         "analysis",
         "somatic variants: maf file of somatic variants in TWIST targed capture region",
-        "MAF file of variants that fall within the TWIST excome capture regions generated using vcf2maf tool (https://github.com/mskcc/vcf2maf). VEP was used to annotate twist.vcf file, which was then used as input to vcf2maf.",
+        "MAF file of variants that fall within the TWIST excome capture regions generated using vcf2maf tool (https://github.com/mskcc/vcf2maf). VEP was used to annotate twist.vcf file, which was then used as input to vcf2maf. NOTE: Some columns in this maf file may be affected by the ExACdb assembly compatibility issue discussed in the WES pipeline overview page (https://cidc.nci.nih.gov/pipelines/wes).",
     ),
     "/wes/analysis/tnscope_output_twist_filtered.vcf": FileDetails(
         "analysis",
         "somatic variants: vcf file of somatic variants in TWIST targed capture region filtered by PASS column",
         "VCF file of variants that fall within the TWIST excome capture regions filtered to remove vairants where the PASS column contained one of the following- germline-risk, low_t_alt_frac, t_lod_fstar, or triallelic_site",
     ),
     "/wes/analysis/tnscope_output_twist_filtered.maf": FileDetails(
         "analysis",
         "somatic variants: maf file of somatic variants in TWIST targed capture region filtered by PASS column",
-        "MAF file generated by converting twist.filtered.vcf to maf using VEP to annotate variants and vcf2maf to do the conversion.",
+        "MAF file generated by converting twist.filtered.vcf to maf using VEP to annotate variants and vcf2maf to do the conversion. NOTE: Some columns in this maf file may be affected by the ExACdb assembly compatibility issue discussed in the WES pipeline overview page (https://cidc.nci.nih.gov/pipelines/wes).",
     ),
     "/wes/analysis/tcellextrect.txt": FileDetails(
         "analysis",
         "tcell: TCell fraction estimates generated by TcellExTRECT",
         "TCell fraction estimates generated by the TcellExTRECT software (https://github.com/McGranahanLab/TcellExTRECT)",
     ),
     "/wes/analysis/tumor/hla_final_result.txt": FileDetails(
@@ -364,25 +364,25 @@
         "analysis",
         "somatic variants: vcf file of somatic variants in TWIST targed capture region",
         "VCF file of variants that fall within the TWIST excome capture regions.  bcftools is used to filter reads in output.vcf.gz that intersect with the TWIST capture regions.",
     ),
     "/wes_tumor_only/analysis/tnscope_output_twist.maf": FileDetails(
         "analysis",
         "somatic variants: maf file of somatic variants in TWIST targed capture region",
-        "MAF file of variants that fall within the TWIST excome capture regions generated using vcf2maf tool (https://github.com/mskcc/vcf2maf). VEP was used to annotate twist.vcf file, which was then used as input to vcf2maf.",
+        "MAF file of variants that fall within the TWIST excome capture regions generated using vcf2maf tool (https://github.com/mskcc/vcf2maf). VEP was used to annotate twist.vcf file, which was then used as input to vcf2maf.NOTE: Some columns in this maf file may be affected by the ExACdb assembly compatibility issue discussed in the WES pipeline overview page (https://cidc.nci.nih.gov/pipelines/wes).",
     ),
     "/wes_tumor_only/analysis/tnscope_output_twist_filtered.vcf": FileDetails(
         "analysis",
         "somatic variants: vcf file of somatic variants in TWIST targed capture region filtered by PASS column",
         "VCF file of variants that fall within the TWIST excome capture regions filtered to remove vairants where the PASS column contained one of the following- germline-risk, low_t_alt_frac, t_lod_fstar, or triallelic_site",
     ),
     "/wes_tumor_only/analysis/tnscope_output_twist_filtered.maf": FileDetails(
         "analysis",
         "somatic variants: maf file of somatic variants in TWIST targed capture region filtered by PASS column",
-        "MAF file generated by converting twist.filtered.vcf to maf using VEP to annotate variants and vcf2maf to do the conversion.",
+        "MAF file generated by converting twist.filtered.vcf to maf using VEP to annotate variants and vcf2maf to do the conversion. NOTE: Some columns in this maf file may be affected by the ExACdb assembly compatibility issue discussed in the WES pipeline overview page (https://cidc.nci.nih.gov/pipelines/wes).",
     ),
     "/wes_tumor_only/analysis/tcellextrect.txt": FileDetails(
         "analysis",
         "tcell: TCell fraction estimates generated by TcellExTRECT",
         "TCell fraction estimates generated by the TcellExTRECT software (https://github.com/McGranahanLab/TcellExTRECT)",
     ),
     "/wes_tumor_only/analysis/tumor/hla_final_result.txt": FileDetails(
@@ -516,15 +516,15 @@
         "The gzipped, FASTQ file that represents the 3' read of paired sequencing. Generated by the sequencing machine defined by the RNA assay this file is associated with.",
     ),
     "/rna/reads_.bam": FileDetails(
         "source",
         "bam file containing the paired pairs",
         "The paired raw reads in the standard BAM binary format, generated from the raw R1 and R2 FASTQ files.",
     ),
-    ## see: https://github.com/CIMAC-CIDC/cidc-ngs-pipeline-api/blob/master/rna/rna_level1_output_API.json
+    ## see: https://github.com/NCI-CIDC/cidc-ngs-pipeline-api/blob/master/rna/rna_level1_output_API.json
     "/rna/analysis/star/sorted.bam": FileDetails(
         "analysis",
         "bam file of the aligned reads with index sorted.bam.bai, sorted by their location in the genome from STAR",
         "Aligned reads in the standard BAM binary format, sorted by their coordinate in the genome (similar to `samtools sort`) which is required by many downstream applications.",
     ),
     "/rna/analysis/star/sorted.bam.bai": FileDetails(
         "analysis",
```

### Comparing `nci_cidc_api_modules-0.27.42rc0/cidc_api/models/files/facets.py` & `nci_cidc_api_modules-0.27.43/cidc_api/models/files/facets.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.42rc0/cidc_api/models/migrations.py` & `nci_cidc_api_modules-0.27.43/cidc_api/models/migrations.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.42rc0/cidc_api/models/models.py` & `nci_cidc_api_modules-0.27.43/cidc_api/models/models.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.42rc0/cidc_api/models/schemas.py` & `nci_cidc_api_modules-0.27.43/cidc_api/models/schemas.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.42rc0/cidc_api/shared/auth.py` & `nci_cidc_api_modules-0.27.43/cidc_api/shared/auth.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.42rc0/cidc_api/shared/emails.py` & `nci_cidc_api_modules-0.27.43/cidc_api/shared/emails.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,18 +43,18 @@
 
     subject = "CIDC Account Approval"
 
     html_content = f"""
     <p>Hello {user.first_n},</p>
     <p>
         Your CIMAC-CIDC Portal account has been approved! 
-        To begin browsing and downloading data, visit https://portal.cimac-network.org.
+        To begin browsing and downloading data, visit https://cidc.nci.nih.gov.
     </p>
     <p>
-        <strong>Note:</strong> If you haven't already, please email cidc-admin@mail.nih.gov to request permission to view data for the trials and assays relevant to your work.</p>
+        <strong>Note:</strong> If you haven't already, please email NCICIDCAdmin@mail.nih.gov to request permission to view data for the trials and assays relevant to your work.</p>
     <p>Thanks,<br/>The CIDC Project Team</p>
     """
 
     email = {
         "to_emails": [user.email],
         "subject": subject,
         "html_content": html_content,
```

### Comparing `nci_cidc_api_modules-0.27.42rc0/cidc_api/shared/gcloud_client.py` & `nci_cidc_api_modules-0.27.43/cidc_api/shared/gcloud_client.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.42rc0/cidc_api/shared/rest_utils.py` & `nci_cidc_api_modules-0.27.43/cidc_api/shared/rest_utils.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.42rc0/nci_cidc_api_modules.egg-info/PKG-INFO` & `nci_cidc_api_modules-0.27.43/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: nci-cidc-api-modules
-Version: 0.27.42rc0
-Summary: SQLAlchemy data models and configuration tools used in the NCI CIDC API
-Home-page: https://github.com/NCI-CIDC/cidc-api-gae
-License: MIT license
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # NCI CIDC API <!-- omit in TOC -->
 
 The next generation of the CIDC API, reworked to use Google Cloud-managed services. This API is built with the Flask REST API framework backed by Google Cloud SQL, running on Google App Engine.
 
 ## Development <!-- omit in TOC -->
 
 - [Install Python dependencies](#install-python-dependencies)
@@ -236,19 +226,19 @@
 gcloud app deploy <app.staging.yaml or app.prod.yaml> --project <gcloud project id>
 ```
 
 That being said, avoid doing this! Deploying this way circumvents the safety checks built into the CI/CD pipeline and can lead to inconsistencies between the code running on GAE and the code present in this repository. Luckily, though, GAE's built-in versioning system makes it hard to do anything catastrophic :-)
 
 ## Connecting to the API
 
-Currently, the staging API is hosted at https://staging-api.cimac-network.org and the production instance is hosted at https://api.cimac-network.org.
+Currently, the staging API is hosted at https://api.cidc-stage.nci.nih.gov and the production instance is hosted at https://api.cidc.nci.nih.gov.
 
-To connect to the staging API with `curl` or a REST API client like Insomnia, get an id token from stagingportal.cimac-network.org, and include the header `Authorization: Bearer YOUR_ID_TOKEN` in requests you make to the staging API. If your token expires, generate a new one following this same procedure.
+To connect to the staging API with `curl` or a REST API client like Insomnia, get an id token from cidc-stage.nci.nih.gov, and include the header `Authorization: Bearer YOUR_ID_TOKEN` in requests you make to the staging API. If your token expires, generate a new one following this same procedure.
 
-To connect to the production API locally, follow the same procedure, but instead get your token from portal.cimac-network.org.
+To connect to the production API locally, follow the same procedure, but instead get your token from cidc.nci.nih.gov.
 
 ## Provisioning the system from scratch
 
 For an overview of how to set up the CIDC API service from scratch, see the step-by-step guide in `PROVISION.md`.
 
 ## JIRA Integration
 
@@ -275,15 +265,15 @@
 
 [The migrations/versions directory](https://github.com/NCI-CIDC/cidc-api-gae/tree/master/migrations/versions) contains SQLAlchemy database migrations generated using flask-sqlalchemy.
 
 The core API code lives in a python module in the [cidc_api](https://github.com/NCI-CIDC/cidc-api-gae/tree/master/cidc_api) subdirectory. In this subdirectory, the [app.py](https://github.com/NCI-CIDC/cidc-api-gae/blob/master/cidc_api/app.py) file contains the code that instantiates/exports the API’s flask app. Stepping through that file top to bottom is probably the best way to get an overall picture of the structure of the API code:
 
 - [get_logger](https://github.com/NCI-CIDC/cidc-api-gae/blob/1de8b59e87eb71a3f8f8e997225e81d6b04b73fd/cidc_api/config/logging.py#L11) instantiates a logger instance based on whether the app is running in a flask development server or gunicorn production server. We need this helper function (or something like it), because logs must be routed in a particular manner for them to show up in stderr when the app is running as a gunicorn server. Any python file in the cidc_api module that includes logging should call this get_logger helper at the top of the file.
 - Next, the Flask app instance is created and configured using settings loaded from [settings.py](https://github.com/NCI-CIDC/cidc-api-gae/blob/master/cidc_api/config/settings.py). This file contains a handful of constants used throughout the app code. Additionally, it contains code for [setting up the temporary directories](https://github.com/NCI-CIDC/cidc-api-gae/blob/001e12ac276a9632260fbddd54419cbcb8a5e2b5/cidc_api/config/settings.py#L37) where empty manifest/assay/analysis templates will live. [This line](https://github.com/NCI-CIDC/cidc-api-gae/blob/001e12ac276a9632260fbddd54419cbcb8a5e2b5/cidc_api/config/settings.py#L118) at the bottom of the file builds a settings dictionary mapping variable names to values for all constants (i.e., uppercase variables) defined above it.
-- Next, [CORS](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS) is enabled. CORS allows the API to respond to requests originating from domains other than the API’s domain. If we didn’t do this, then an API instance running at “api.cimac-network.org” would be prohibited from responding to requests from a UI instance running at “portal.cimac-network.org”.
+- Next, [CORS](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS) is enabled. CORS allows the API to respond to requests originating from domains other than the API’s domain. If we didn’t do this, then an API instance running at “api.cidc.nci.nih.gov” would be prohibited from responding to requests from a UI instance running at “cidc.nci.nih.gov”.
 - Next, [init_db](https://github.com/NCI-CIDC/cidc-api-gae/blob/1de8b59e87eb71a3f8f8e997225e81d6b04b73fd/cidc_api/config/db.py#L17) connects the flask-sqlalchemy package to a given API app instance. Moreover, it sets up our database migration utility, [flask-migrate](https://flask-migrate.readthedocs.io/en/latest/), which provides CLI shortcuts for generating migrations based on changes to the API’s sqlalchemy models. Currently, db migrations are [run every time init_db is called](https://github.com/NCI-CIDC/cidc-api-gae/blob/1de8b59e87eb71a3f8f8e997225e81d6b04b73fd/cidc_api/config/db.py#L23), but this is arguably tech debt, since it slows down app startup for no good reason - it might be better to try running db migrations as part of CI. (All other code in this file is related to building database connections based on the environment in which the app is running).
 - Next, [register_resources](https://github.com/NCI-CIDC/cidc-api-gae/blob/1de8b59e87eb71a3f8f8e997225e81d6b04b73fd/cidc_api/resources/__init__.py#L12) “wires up” all of the REST resources in the API, which are organized as independent flask [blueprints](https://flask.palletsprojects.com/en/2.0.x/blueprints/). Each resource blueprint is a collection of flask endpoints. Resources are split up into separate blueprints solely for code organization purposes.
 - Next, [validate_api_auth](https://github.com/NCI-CIDC/cidc-api-gae/blob/1de8b59e87eb71a3f8f8e997225e81d6b04b73fd/cidc_api/shared/auth.py#L17) enforces that all endpoints configured in the API are explicitly flagged as public or private using the [public](https://github.com/NCI-CIDC/cidc-api-gae/blob/1de8b59e87eb71a3f8f8e997225e81d6b04b73fd/cidc_api/shared/auth.py#L75) and [requires_auth](https://github.com/NCI-CIDC/cidc-api-gae/blob/1de8b59e87eb71a3f8f8e997225e81d6b04b73fd/cidc_api/shared/auth.py#L34) decorators, respectively. This is intended to help prevent a developer from accidentally making a private endpoint public by forgetting to include the requires_auth decorator. If this validation check fails, the app won’t start up.
 - Next, [register_dashboards](https://github.com/NCI-CIDC/cidc-api-gae/blob/1de8b59e87eb71a3f8f8e997225e81d6b04b73fd/cidc_api/dashboards/__init__.py#L6) wires up our plot.ly dash dashboards.
 - Next, [handle_errors](https://github.com/NCI-CIDC/cidc-api-gae/blob/1de8b59e87eb71a3f8f8e997225e81d6b04b73fd/cidc_api/app.py#L37) adds generic code for formatting any error thrown while a request is being handled as JSON.
 - Finally, if the app submodule is being run directly via “python -m cidc_api.app”, [this code](https://github.com/NCI-CIDC/cidc-api-gae/blob/1de8b59e87eb71a3f8f8e997225e81d6b04b73fd/cidc_api/app.py#L65) will start a flask (non-gunicorn) server.
 
@@ -349,25 +339,25 @@
 
 **Note:** although flask-migrate and alembic, the tool flask-migrate uses under the hood, can automatically pick up certain sqlalchemy model class changes (e.g., adding/removing models, adding/removing columns, column data type changes), there are other changes that it can’t pick up automatically. Two examples I’ve encountered are adding/removing values from enum types and adding/updating [CHECK constraints](https://docs.sqlalchemy.org/en/14/core/constraints.html#check-constraint). For this reason, always review the auto-generated migration file before applying it, making any required manually edits/additions.
 
 #### How can I check that a database migration works?
 
 First, I run the “flask db upgrade” against my local database - this can catch basic errors, like syntax or type issues, even if there’s no data currently stored in the local database.
 
-Next, I’ll try running the migration against the staging database from my local computer (since the staging db generally has representative data in it, this can catch further errors you might miss in a local db test). To do this, you need to [set up a connection to the staging db](https://github.com/cimac-cidc/cidc-api-gae#connecting-to-a-cloud-sql-database-instance) and to [update your .env file](https://github.com/NCI-CIDC/cidc-api-gae/blob/75e88280e1103b530f6e7bd7261ca90f933159b2/.env#L23) to tell your local api code to use this connection. **Make sure that no one else is using the staging db for anything critical**, then run the db upgrade. If you encounter new errors, fix them. Once the upgrade succeeds, undo it with “flask db downgrade”, then make a PR to deploy the new migration.
+Next, I’ll try running the migration against the staging database from my local computer (since the staging db generally has representative data in it, this can catch further errors you might miss in a local db test). To do this, you need to [set up a connection to the staging db](https://github.com/nci-cidc/cidc-api-gae#connecting-to-a-cloud-sql-database-instance) and to [update your .env file](https://github.com/NCI-CIDC/cidc-api-gae/blob/75e88280e1103b530f6e7bd7261ca90f933159b2/.env#L23) to tell your local api code to use this connection. **Make sure that no one else is using the staging db for anything critical**, then run the db upgrade. If you encounter new errors, fix them. Once the upgrade succeeds, undo it with “flask db downgrade”, then make a PR to deploy the new migration.
 
 #### What happens when a database migration fails, and what should I do to remediate the situation?
 
 Because database migrations are run when the app starts up, failed database migrations manifest as the API failing to start up. This usually looks like the “failed to load account information” error message appearing 5-10 seconds after trying to load the portal.
 
 Remediating a failing migration requires two steps:
 
 1. Redirect traffic to a previous app engine version that does not include the failing migration code. You can select a known-good version from [this page](https://console.cloud.google.com/appengine/versions) in the GCP console.
 2. Debug and fix the migration locally following a process like the one described above.
 
-**Note:** when you want to undo a migration that **did not fail to run**, but has some other issue with it, the solution is different. If you try to simply send traffic to a previous app engine version without the migration you want to undo included in it, you’ll get an error on app startup (something like “alembic.util.CommandError: Can't locate revision identified by '31b8ab83c7d'”). In order to undo this migration, you’ll need to [manually connect to the cloud sql instance](https://github.com/cimac-cidc/cidc-api-gae#connecting-to-a-cloud-sql-database-instance), [update your .env file](https://github.com/NCI-CIDC/cidc-api-gae/blob/75e88280e1103b530f6e7bd7261ca90f933159b2/.env#L23) to tell your local api code to use this connection, then run “flask db downgrade”. Once that command succeeds, you’ve rolled back the unwanted migration, and you can safely send traffic to a previous app engine version that doesn’t include the migration.
+**Note:** when you want to undo a migration that **did not fail to run**, but has some other issue with it, the solution is different. If you try to simply send traffic to a previous app engine version without the migration you want to undo included in it, you’ll get an error on app startup (something like “alembic.util.CommandError: Can't locate revision identified by '31b8ab83c7d'”). In order to undo this migration, you’ll need to [manually connect to the cloud sql instance](https://github.com/nci-cidc/cidc-api-gae#connecting-to-a-cloud-sql-database-instance), [update your .env file](https://github.com/NCI-CIDC/cidc-api-gae/blob/75e88280e1103b530f6e7bd7261ca90f933159b2/.env#L23) to tell your local api code to use this connection, then run “flask db downgrade”. Once that command succeeds, you’ve rolled back the unwanted migration, and you can safely send traffic to a previous app engine version that doesn’t include the migration.
 
 #### What’s packaged up in cidc-api-modules pypi package?
 
 The cidc-api-modules package includes only the submodules used in the cidc-cloud-functions module. Here’s the [full list](https://github.com/NCI-CIDC/cidc-api-gae/blob/ed18274bd413444157fb3d7af8e0dc3925079e6a/setup.py#L14). Notably, the “cidc_api.app” and “cidc_api.resources” submodules are excluded, since these pertain only to the API. To be perfectly honest, I don’t remember the issue that led to the decision to not simply package up and public the top-level “cidc_api” module (it’s possible even if it’s not necessary). Anyhow, this means that bumping the cidc-api-modules version is only necessary when making changes to the included submodules that you want to propagate to the cloud functions repo.
 
 Relatedly, it could be worth looking into combining the cloud functions repo into the cidc-api-gae repo. There’s no great reason for them to be separate. In fact, since they share code related to interacting with the database and with GCP, the decision to separate the two repos likely creates more friction than it alleviates.
```

### Comparing `nci_cidc_api_modules-0.27.42rc0/nci_cidc_api_modules.egg-info/SOURCES.txt` & `nci_cidc_api_modules-0.27.43/nci_cidc_api_modules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.42rc0/setup.py` & `nci_cidc_api_modules-0.27.43/setup.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.42rc0/tests/test_api.py` & `nci_cidc_api_modules-0.27.43/tests/test_api.py`

 * *Files identical despite different names*

