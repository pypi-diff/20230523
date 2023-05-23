# Comparing `tmp/django_staff_sso_client-4.1.1.tar.gz` & `tmp/django_staff_sso_client-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_staff_sso_client-4.1.1.tar", last modified: Fri Nov 18 10:26:13 2022, max compression
+gzip compressed data, was "django_staff_sso_client-4.2.0.tar", last modified: Tue May 23 14:43:42 2023, max compression
```

## Comparing `django_staff_sso_client-4.1.1.tar` & `django_staff_sso_client-4.2.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-18 10:26:13.192589 django_staff_sso_client-4.1.1/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8228 2022-11-18 10:26:13.192589 django_staff_sso_client-4.1.1/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7398 2022-11-18 10:25:48.000000 django_staff_sso_client-4.1.1/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-18 10:26:13.192589 django_staff_sso_client-4.1.1/authbroker_client/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-11-18 10:25:48.000000 django_staff_sso_client-4.1.1/authbroker_client/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1639 2022-11-18 10:25:48.000000 django_staff_sso_client-4.1.1/authbroker_client/backends.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1545 2022-11-18 10:25:48.000000 django_staff_sso_client-4.1.1/authbroker_client/middleware.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      535 2022-11-18 10:25:48.000000 django_staff_sso_client-4.1.1/authbroker_client/urls.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1666 2022-11-18 10:25:48.000000 django_staff_sso_client-4.1.1/authbroker_client/utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       22 2022-11-18 10:25:48.000000 django_staff_sso_client-4.1.1/authbroker_client/version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3379 2022-11-18 10:25:48.000000 django_staff_sso_client-4.1.1/authbroker_client/views.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-18 10:26:13.192589 django_staff_sso_client-4.1.1/django_staff_sso_client.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8228 2022-11-18 10:26:13.000000 django_staff_sso_client-4.1.1/django_staff_sso_client.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      675 2022-11-18 10:26:13.000000 django_staff_sso_client-4.1.1/django_staff_sso_client.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-11-18 10:26:13.000000 django_staff_sso_client-4.1.1/django_staff_sso_client.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      153 2022-11-18 10:26:13.000000 django_staff_sso_client-4.1.1/django_staff_sso_client.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2022-11-18 10:26:13.000000 django_staff_sso_client-4.1.1/django_staff_sso_client.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       85 2022-11-18 10:25:48.000000 django_staff_sso_client-4.1.1/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      359 2022-11-18 10:26:13.192589 django_staff_sso_client-4.1.1/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1943 2022-11-18 10:25:48.000000 django_staff_sso_client-4.1.1/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-18 10:26:13.192589 django_staff_sso_client-4.1.1/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-11-18 10:25:48.000000 django_staff_sso_client-4.1.1/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2022-11-18 10:25:48.000000 django_staff_sso_client-4.1.1/tests/conftest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2041 2022-11-18 10:25:48.000000 django_staff_sso_client-4.1.1/tests/settings.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4154 2022-11-18 10:25:48.000000 django_staff_sso_client-4.1.1/tests/test_backends.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1665 2022-11-18 10:25:48.000000 django_staff_sso_client-4.1.1/tests/test_middleware.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      331 2022-11-18 10:25:48.000000 django_staff_sso_client-4.1.1/tests/test_urls.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3128 2022-11-18 10:25:48.000000 django_staff_sso_client-4.1.1/tests/test_utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      106 2022-11-18 10:25:48.000000 django_staff_sso_client-4.1.1/tests/test_version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3419 2022-11-18 10:25:48.000000 django_staff_sso_client-4.1.1/tests/test_views.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      716 2022-11-18 10:25:48.000000 django_staff_sso_client-4.1.1/tests/urls.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-23 14:43:42.577528 django_staff_sso_client-4.2.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8267 2023-05-23 14:43:42.577528 django_staff_sso_client-4.2.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7398 2023-05-23 14:43:15.000000 django_staff_sso_client-4.2.0/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-23 14:43:42.577528 django_staff_sso_client-4.2.0/authbroker_client/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-23 14:43:15.000000 django_staff_sso_client-4.2.0/authbroker_client/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1639 2023-05-23 14:43:15.000000 django_staff_sso_client-4.2.0/authbroker_client/backends.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1545 2023-05-23 14:43:15.000000 django_staff_sso_client-4.2.0/authbroker_client/middleware.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      535 2023-05-23 14:43:15.000000 django_staff_sso_client-4.2.0/authbroker_client/urls.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1666 2023-05-23 14:43:15.000000 django_staff_sso_client-4.2.0/authbroker_client/utils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       22 2023-05-23 14:43:15.000000 django_staff_sso_client-4.2.0/authbroker_client/version.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3379 2023-05-23 14:43:15.000000 django_staff_sso_client-4.2.0/authbroker_client/views.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-23 14:43:42.577528 django_staff_sso_client-4.2.0/django_staff_sso_client.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8267 2023-05-23 14:43:42.000000 django_staff_sso_client-4.2.0/django_staff_sso_client.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      675 2023-05-23 14:43:42.000000 django_staff_sso_client-4.2.0/django_staff_sso_client.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-05-23 14:43:42.000000 django_staff_sso_client-4.2.0/django_staff_sso_client.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      168 2023-05-23 14:43:42.000000 django_staff_sso_client-4.2.0/django_staff_sso_client.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2023-05-23 14:43:42.000000 django_staff_sso_client-4.2.0/django_staff_sso_client.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       85 2023-05-23 14:43:15.000000 django_staff_sso_client-4.2.0/pyproject.toml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      359 2023-05-23 14:43:42.581528 django_staff_sso_client-4.2.0/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1982 2023-05-23 14:43:15.000000 django_staff_sso_client-4.2.0/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-23 14:43:42.577528 django_staff_sso_client-4.2.0/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-23 14:43:15.000000 django_staff_sso_client-4.2.0/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-05-23 14:43:15.000000 django_staff_sso_client-4.2.0/tests/conftest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2041 2023-05-23 14:43:15.000000 django_staff_sso_client-4.2.0/tests/settings.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4154 2023-05-23 14:43:15.000000 django_staff_sso_client-4.2.0/tests/test_backends.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1665 2023-05-23 14:43:15.000000 django_staff_sso_client-4.2.0/tests/test_middleware.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      331 2023-05-23 14:43:15.000000 django_staff_sso_client-4.2.0/tests/test_urls.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3128 2023-05-23 14:43:15.000000 django_staff_sso_client-4.2.0/tests/test_utils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      106 2023-05-23 14:43:15.000000 django_staff_sso_client-4.2.0/tests/test_version.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3419 2023-05-23 14:43:15.000000 django_staff_sso_client-4.2.0/tests/test_views.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      716 2023-05-23 14:43:15.000000 django_staff_sso_client-4.2.0/tests/urls.py
```

### Comparing `django_staff_sso_client-4.1.1/PKG-INFO` & `django_staff_sso_client-4.2.0/django_staff_sso_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
-Name: django_staff_sso_client
-Version: 4.1.1
+Name: django-staff-sso-client
+Version: 4.2.0
 Summary: Reusable Django app to facilitate gov.uk Staff Single Sign On
 Home-page: https://github.com/uktrade/django-staff-sso-client/
 Author: Department for International Trade
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: test
 
 # Django-staff-sso-client
 
 [![CircleCI](https://circleci.com/gh/uktrade/django-staff-sso-client/tree/master.svg?style=svg)](https://circleci.com/gh/uktrade/django-staff-sso-client/tree/master)
```

### Comparing `django_staff_sso_client-4.1.1/README.md` & `django_staff_sso_client-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `django_staff_sso_client-4.1.1/authbroker_client/backends.py` & `django_staff_sso_client-4.2.0/authbroker_client/backends.py`

 * *Files identical despite different names*

### Comparing `django_staff_sso_client-4.1.1/authbroker_client/middleware.py` & `django_staff_sso_client-4.2.0/authbroker_client/middleware.py`

 * *Files identical despite different names*

### Comparing `django_staff_sso_client-4.1.1/authbroker_client/urls.py` & `django_staff_sso_client-4.2.0/authbroker_client/urls.py`

 * *Files identical despite different names*

### Comparing `django_staff_sso_client-4.1.1/authbroker_client/utils.py` & `django_staff_sso_client-4.2.0/authbroker_client/utils.py`

 * *Files identical despite different names*

### Comparing `django_staff_sso_client-4.1.1/authbroker_client/views.py` & `django_staff_sso_client-4.2.0/authbroker_client/views.py`

 * *Files identical despite different names*

### Comparing `django_staff_sso_client-4.1.1/django_staff_sso_client.egg-info/PKG-INFO` & `django_staff_sso_client-4.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
-Name: django-staff-sso-client
-Version: 4.1.1
+Name: django_staff_sso_client
+Version: 4.2.0
 Summary: Reusable Django app to facilitate gov.uk Staff Single Sign On
 Home-page: https://github.com/uktrade/django-staff-sso-client/
 Author: Department for International Trade
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: test
 
 # Django-staff-sso-client
 
 [![CircleCI](https://circleci.com/gh/uktrade/django-staff-sso-client/tree/master.svg?style=svg)](https://circleci.com/gh/uktrade/django-staff-sso-client/tree/master)
```

### Comparing `django_staff_sso_client-4.1.1/django_staff_sso_client.egg-info/SOURCES.txt` & `django_staff_sso_client-4.2.0/django_staff_sso_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_staff_sso_client-4.1.1/setup.py` & `django_staff_sso_client-4.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,18 +37,19 @@
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Framework :: Django',
         'Framework :: Django :: 3.0',
         'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.2',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     install_requires=[
-        'Django>=3.0,<4.2',
+        'Django>=3.0,<=4.2',
         'requests_oauthlib',
     ],
     extras_require={
         'test': [
             'pytest==7.1.1',
             'pytest-cov',
             'pytest-django',
```

### Comparing `django_staff_sso_client-4.1.1/tests/settings.py` & `django_staff_sso_client-4.2.0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_staff_sso_client-4.1.1/tests/test_backends.py` & `django_staff_sso_client-4.2.0/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `django_staff_sso_client-4.1.1/tests/test_middleware.py` & `django_staff_sso_client-4.2.0/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `django_staff_sso_client-4.1.1/tests/test_utils.py` & `django_staff_sso_client-4.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django_staff_sso_client-4.1.1/tests/test_views.py` & `django_staff_sso_client-4.2.0/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_staff_sso_client-4.1.1/tests/urls.py` & `django_staff_sso_client-4.2.0/tests/urls.py`

 * *Files identical despite different names*

