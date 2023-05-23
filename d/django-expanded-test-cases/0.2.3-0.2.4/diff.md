# Comparing `tmp/django-expanded-test-cases-0.2.3.tar.gz` & `tmp/django-expanded-test-cases-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-expanded-test-cases-0.2.3.tar", last modified: Sun Mar  5 08:45:35 2023, max compression
+gzip compressed data, was "django-expanded-test-cases-0.2.4.tar", last modified: Tue May 23 03:26:21 2023, max compression
```

## Comparing `django-expanded-test-cases-0.2.3.tar` & `django-expanded-test-cases-0.2.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-03-05 08:45:35.279630 django-expanded-test-cases-0.2.3/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1074 2022-06-02 21:49:59.000000 django-expanded-test-cases-0.2.3/LICENSE
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)       91 2023-03-05 08:40:41.000000 django-expanded-test-cases-0.2.3/MANIFEST.in
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     4514 2023-03-05 08:45:35.279630 django-expanded-test-cases-0.2.3/PKG-INFO
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-03-05 08:45:35.279630 django-expanded-test-cases-0.2.3/django_expanded_test_cases/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      181 2022-06-02 21:49:59.000000 django-expanded-test-cases-0.2.3/django_expanded_test_cases/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     7303 2023-03-05 08:40:41.000000 django-expanded-test-cases-0.2.3/django_expanded_test_cases/constants.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-03-05 08:45:35.279630 django-expanded-test-cases-0.2.3/django_expanded_test_cases/mixins/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      325 2022-10-11 03:11:48.000000 django-expanded-test-cases-0.2.3/django_expanded_test_cases/mixins/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    35675 2023-03-05 08:40:41.000000 django-expanded-test-cases-0.2.3/django_expanded_test_cases/mixins/core_mixin.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    29165 2023-03-05 08:40:41.000000 django-expanded-test-cases-0.2.3/django_expanded_test_cases/mixins/response_mixin.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-03-05 08:45:35.275629 django-expanded-test-cases-0.2.3/django_expanded_test_cases/templates/
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-03-05 08:45:35.279630 django-expanded-test-cases-0.2.3/django_expanded_test_cases/templates/django_expanded_test_cases/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      528 2023-03-05 08:40:41.000000 django-expanded-test-cases-0.2.3/django_expanded_test_cases/templates/django_expanded_test_cases/index.html
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-03-05 08:45:35.279630 django-expanded-test-cases-0.2.3/django_expanded_test_cases/test_cases/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1376 2023-02-17 03:47:57.000000 django-expanded-test-cases-0.2.3/django_expanded_test_cases/test_cases/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    16682 2023-03-05 08:40:41.000000 django-expanded-test-cases-0.2.3/django_expanded_test_cases/test_cases/base_test_case.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    55191 2023-03-05 08:40:41.000000 django-expanded-test-cases-0.2.3/django_expanded_test_cases/test_cases/integration_test_case.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     7790 2023-02-17 03:47:57.000000 django-expanded-test-cases-0.2.3/django_expanded_test_cases/test_cases/live_server_test_case.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1093 2023-03-05 08:40:41.000000 django-expanded-test-cases-0.2.3/django_expanded_test_cases/test_urls.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-03-05 08:45:35.279630 django-expanded-test-cases-0.2.3/django_expanded_test_cases.egg-info/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     4514 2023-03-05 08:45:35.000000 django-expanded-test-cases-0.2.3/django_expanded_test_cases.egg-info/PKG-INFO
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1116 2023-03-05 08:45:35.000000 django-expanded-test-cases-0.2.3/django_expanded_test_cases.egg-info/SOURCES.txt
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        1 2023-03-05 08:45:35.000000 django-expanded-test-cases-0.2.3/django_expanded_test_cases.egg-info/dependency_links.txt
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      112 2023-03-05 08:45:35.000000 django-expanded-test-cases-0.2.3/django_expanded_test_cases.egg-info/requires.txt
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)       33 2023-03-05 08:45:35.000000 django-expanded-test-cases-0.2.3/django_expanded_test_cases.egg-info/top_level.txt
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1735 2023-03-05 08:44:30.000000 django-expanded-test-cases-0.2.3/pyproject.toml
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1732 2023-02-17 03:47:57.000000 django-expanded-test-cases-0.2.3/readme.md
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1192 2023-03-05 08:45:35.279630 django-expanded-test-cases-0.2.3/setup.cfg
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-03-05 08:45:35.279630 django-expanded-test-cases-0.2.3/tests/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        0 2022-05-23 23:45:09.000000 django-expanded-test-cases-0.2.3/tests/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      198 2023-02-17 03:47:57.000000 django-expanded-test-cases-0.2.3/tests/apps.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      360 2023-02-17 03:47:57.000000 django-expanded-test-cases-0.2.3/tests/asgi.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3527 2023-03-05 08:40:41.000000 django-expanded-test-cases-0.2.3/tests/settings.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-03-05 08:45:35.279630 django-expanded-test-cases-0.2.3/tests/test_cases/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        0 2022-06-02 21:49:59.000000 django-expanded-test-cases-0.2.3/tests/test_cases/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    96771 2023-03-05 08:40:41.000000 django-expanded-test-cases-0.2.3/tests/test_cases/test_base_case.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)   269449 2023-03-05 08:40:41.000000 django-expanded-test-cases-0.2.3/tests/test_cases/test_integration_case.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2230 2023-02-17 03:47:57.000000 django-expanded-test-cases-0.2.3/tests/test_cases/test_live_server_case.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      316 2023-03-05 08:40:41.000000 django-expanded-test-cases-0.2.3/tests/urls.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3964 2023-03-05 08:40:41.000000 django-expanded-test-cases-0.2.3/tests/views.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-05-23 03:26:21.051754 django-expanded-test-cases-0.2.4/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1074 2022-06-02 21:49:59.000000 django-expanded-test-cases-0.2.4/LICENSE
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)       91 2023-03-05 08:40:41.000000 django-expanded-test-cases-0.2.4/MANIFEST.in
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     5168 2023-05-23 03:26:21.051754 django-expanded-test-cases-0.2.4/PKG-INFO
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-05-23 03:26:21.051754 django-expanded-test-cases-0.2.4/django_expanded_test_cases/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      181 2022-06-02 21:49:59.000000 django-expanded-test-cases-0.2.4/django_expanded_test_cases/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     7303 2023-05-23 03:17:15.000000 django-expanded-test-cases-0.2.4/django_expanded_test_cases/constants.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-05-23 03:26:21.051754 django-expanded-test-cases-0.2.4/django_expanded_test_cases/mixins/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      325 2022-10-11 03:11:48.000000 django-expanded-test-cases-0.2.4/django_expanded_test_cases/mixins/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    35675 2023-05-23 03:17:15.000000 django-expanded-test-cases-0.2.4/django_expanded_test_cases/mixins/core_mixin.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    29221 2023-04-11 22:52:56.000000 django-expanded-test-cases-0.2.4/django_expanded_test_cases/mixins/response_mixin.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-05-23 03:26:21.047754 django-expanded-test-cases-0.2.4/django_expanded_test_cases/templates/
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-05-23 03:26:21.051754 django-expanded-test-cases-0.2.4/django_expanded_test_cases/templates/django_expanded_test_cases/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      528 2023-03-05 08:40:41.000000 django-expanded-test-cases-0.2.4/django_expanded_test_cases/templates/django_expanded_test_cases/index.html
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-05-23 03:26:21.051754 django-expanded-test-cases-0.2.4/django_expanded_test_cases/test_cases/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1376 2023-02-17 03:47:57.000000 django-expanded-test-cases-0.2.4/django_expanded_test_cases/test_cases/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    16682 2023-03-05 08:40:41.000000 django-expanded-test-cases-0.2.4/django_expanded_test_cases/test_cases/base_test_case.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    55191 2023-03-05 08:40:41.000000 django-expanded-test-cases-0.2.4/django_expanded_test_cases/test_cases/integration_test_case.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     7790 2023-02-17 03:47:57.000000 django-expanded-test-cases-0.2.4/django_expanded_test_cases/test_cases/live_server_test_case.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1093 2023-03-05 08:40:41.000000 django-expanded-test-cases-0.2.4/django_expanded_test_cases/test_urls.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-05-23 03:26:21.051754 django-expanded-test-cases-0.2.4/django_expanded_test_cases.egg-info/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     5168 2023-05-23 03:26:21.000000 django-expanded-test-cases-0.2.4/django_expanded_test_cases.egg-info/PKG-INFO
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1116 2023-05-23 03:26:21.000000 django-expanded-test-cases-0.2.4/django_expanded_test_cases.egg-info/SOURCES.txt
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        1 2023-05-23 03:26:21.000000 django-expanded-test-cases-0.2.4/django_expanded_test_cases.egg-info/dependency_links.txt
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      112 2023-05-23 03:26:21.000000 django-expanded-test-cases-0.2.4/django_expanded_test_cases.egg-info/requires.txt
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)       33 2023-05-23 03:26:21.000000 django-expanded-test-cases-0.2.4/django_expanded_test_cases.egg-info/top_level.txt
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1781 2023-05-23 03:23:42.000000 django-expanded-test-cases-0.2.4/pyproject.toml
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2335 2023-04-11 23:02:41.000000 django-expanded-test-cases-0.2.4/readme.md
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1192 2023-05-23 03:26:21.051754 django-expanded-test-cases-0.2.4/setup.cfg
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-05-23 03:26:21.051754 django-expanded-test-cases-0.2.4/tests/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        0 2022-05-23 23:45:09.000000 django-expanded-test-cases-0.2.4/tests/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      198 2023-02-17 03:47:57.000000 django-expanded-test-cases-0.2.4/tests/apps.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      360 2023-02-17 03:47:57.000000 django-expanded-test-cases-0.2.4/tests/asgi.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3527 2023-03-05 08:40:41.000000 django-expanded-test-cases-0.2.4/tests/settings.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-05-23 03:26:21.051754 django-expanded-test-cases-0.2.4/tests/test_cases/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        0 2022-06-02 21:49:59.000000 django-expanded-test-cases-0.2.4/tests/test_cases/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    96771 2023-03-05 08:40:41.000000 django-expanded-test-cases-0.2.4/tests/test_cases/test_base_case.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)   269449 2023-04-11 23:12:20.000000 django-expanded-test-cases-0.2.4/tests/test_cases/test_integration_case.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2230 2023-02-17 03:47:57.000000 django-expanded-test-cases-0.2.4/tests/test_cases/test_live_server_case.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      316 2023-03-05 08:40:41.000000 django-expanded-test-cases-0.2.4/tests/urls.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3964 2023-03-05 08:40:41.000000 django-expanded-test-cases-0.2.4/tests/views.py
```

### Comparing `django-expanded-test-cases-0.2.3/LICENSE` & `django-expanded-test-cases-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.2.3/PKG-INFO` & `django-expanded-test-cases-0.2.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-expanded-test-cases
-Version: 0.2.3
+Version: 0.2.4
 Summary: Expands the existing Django TestCase class with extra functionality.
 Home-page: https://github.com/brodriguez8774/django-expanded-test-cases
 Author: Brandon Rodriguez
 Author-email: Brandon Rodriguez <brodriguez8774@gmail.com>
 Maintainer-email: Brandon Rodriguez <brodriguez8774@gmail.com>
 License: MIT License
         
@@ -44,50 +44,60 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: doc
 License-File: LICENSE
 
 # Django Expanded Test Cases
 
 [![Documentation Status](https://readthedocs.org/projects/django-expanded-test-cases/badge/?version=latest)](https://django-expanded-test-cases.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/django-expanded-test-cases?color=blue)](https://img.shields.io/pypi/v/django-expanded-test-cases?color=blue)
-[![Python versions](https://img.shields.io/badge/python-%3E%3D3.7-brightgreen)](https://img.shields.io/badge/python-%3E%3D3.7-brightgreen)
+[![Python Versions](https://img.shields.io/badge/python-%3E%3D3.7-brightgreen)](https://img.shields.io/badge/python-%3E%3D3.7-brightgreen)
 [![Django Versions](https://img.shields.io/badge/django-%3E%3D3-brightgreen)](https://img.shields.io/badge/django-%3E%3D3-brightgreen)
 [![GitHub](https://img.shields.io/github/license/brodriguez8774/django-expanded-test-cases)](https://img.shields.io/github/license/brodriguez8774/django-expanded-test-cases)
+[![PyPI Downloads per Month](https://img.shields.io/pypi/dm/django-expanded-test-cases.svg)](https://pypi.python.org/pypi/django-expanded-test-cases)
 
 
 ## Description
 
 Expands the existing [Django](https://docs.djangoproject.com/en/dev/)
 [TestCase class](https://docs.djangoproject.com/en/dev/topics/testing/overview/) with extra functionality.
 
 Different TestCase classes are provided, each providing separate sets of functionality.
 
 
+For full documentation, see [ReadTheDocs](https://django-expanded-test-cases.readthedocs.io/en/latest/).
+
+
+## Example ETC Debug Output on UnitTest Error
+A main functionality that **ExpandedTestCases** provides is verbose response debug info on UnitTest errors.<br>
+Below is an example of such output, when a test fails while checking the `<h1>` tag for a very simple page.
+
+![ETC Error Debug Output Screenshot](https://user-images.githubusercontent.com/14208531/231304818-fb0dbe31-ead9-4de8-8efe-a3fc858cbddd.png)
+
+
 ## Installation
 
 Install with
 
     pip install django-expanded-test-cases
 
+For full color output, also install
 
-## Documentation
-
-For full documentation, see [ReadTheDocs](https://django-expanded-test-cases.readthedocs.io/en/latest/).
-
+    pip install colorama
 
 ## Package Development & Running Project Tests
 
 As standard for Python development, this project has its own testing to ensure it functions as desired.
 After installing dependencies, everything required to run tests are provided in one of two files:
 * To run tests via standard django `python manage.py test`, execute the `<project_root>/runtests.py` file.
 * To run tests via `pytest`, execute the `<project_root>/runpytests.py` file.
```

### Comparing `django-expanded-test-cases-0.2.3/django_expanded_test_cases/constants.py` & `django-expanded-test-cases-0.2.4/django_expanded_test_cases/constants.py`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.2.3/django_expanded_test_cases/mixins/core_mixin.py` & `django-expanded-test-cases-0.2.4/django_expanded_test_cases/mixins/core_mixin.py`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.2.3/django_expanded_test_cases/mixins/response_mixin.py` & `django-expanded-test-cases-0.2.4/django_expanded_test_cases/mixins/response_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,14 +264,15 @@
 
     def show_debug_user_info(self, user):
         """Prints debug user data."""
 
         # Imported here to prevent potential "Apps aren't loaded yet" error.
         from django.contrib.auth.models import AnonymousUser
 
+        self._debug_print()
         self._debug_print(
             '{0} {1} {0}'.format('=' * 10, 'User Info'),
             fore=RESPONSE_DEBUG_USER_INFO,
             style=OUTPUT_EMPHASIS,
         )
 
         # Only proceed if we got a proper user model.
@@ -305,14 +306,15 @@
         else:
             self._debug_print('    * Invalid user "{0}" of type "{1}". Expected "{2}".'.format(
                 user,
                 type(user),
                 type(get_user_model()),
             ), fore=OUTPUT_ERROR)
         self._debug_print()
+        self._debug_print()
 
     # endregion Debug Output Functions.
 
     def standardize_html_tags(self, value):
         """Standardizes spacing around html-esque elements, to remove unnecessary spacing.
 
         For example, "<h1> MyHeader </h1>" will simplify down to "<h1>MyHeader</h1>".
```

### Comparing `django-expanded-test-cases-0.2.3/django_expanded_test_cases/templates/django_expanded_test_cases/index.html` & `django-expanded-test-cases-0.2.4/django_expanded_test_cases/templates/django_expanded_test_cases/index.html`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.2.3/django_expanded_test_cases/test_cases/__init__.py` & `django-expanded-test-cases-0.2.4/django_expanded_test_cases/test_cases/__init__.py`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.2.3/django_expanded_test_cases/test_cases/base_test_case.py` & `django-expanded-test-cases-0.2.4/django_expanded_test_cases/test_cases/base_test_case.py`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.2.3/django_expanded_test_cases/test_cases/integration_test_case.py` & `django-expanded-test-cases-0.2.4/django_expanded_test_cases/test_cases/integration_test_case.py`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.2.3/django_expanded_test_cases/test_cases/live_server_test_case.py` & `django-expanded-test-cases-0.2.4/django_expanded_test_cases/test_cases/live_server_test_case.py`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.2.3/django_expanded_test_cases/test_urls.py` & `django-expanded-test-cases-0.2.4/django_expanded_test_cases/test_urls.py`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.2.3/django_expanded_test_cases.egg-info/PKG-INFO` & `django-expanded-test-cases-0.2.4/django_expanded_test_cases.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-expanded-test-cases
-Version: 0.2.3
+Version: 0.2.4
 Summary: Expands the existing Django TestCase class with extra functionality.
 Home-page: https://github.com/brodriguez8774/django-expanded-test-cases
 Author: Brandon Rodriguez
 Author-email: Brandon Rodriguez <brodriguez8774@gmail.com>
 Maintainer-email: Brandon Rodriguez <brodriguez8774@gmail.com>
 License: MIT License
         
@@ -44,50 +44,60 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: doc
 License-File: LICENSE
 
 # Django Expanded Test Cases
 
 [![Documentation Status](https://readthedocs.org/projects/django-expanded-test-cases/badge/?version=latest)](https://django-expanded-test-cases.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/django-expanded-test-cases?color=blue)](https://img.shields.io/pypi/v/django-expanded-test-cases?color=blue)
-[![Python versions](https://img.shields.io/badge/python-%3E%3D3.7-brightgreen)](https://img.shields.io/badge/python-%3E%3D3.7-brightgreen)
+[![Python Versions](https://img.shields.io/badge/python-%3E%3D3.7-brightgreen)](https://img.shields.io/badge/python-%3E%3D3.7-brightgreen)
 [![Django Versions](https://img.shields.io/badge/django-%3E%3D3-brightgreen)](https://img.shields.io/badge/django-%3E%3D3-brightgreen)
 [![GitHub](https://img.shields.io/github/license/brodriguez8774/django-expanded-test-cases)](https://img.shields.io/github/license/brodriguez8774/django-expanded-test-cases)
+[![PyPI Downloads per Month](https://img.shields.io/pypi/dm/django-expanded-test-cases.svg)](https://pypi.python.org/pypi/django-expanded-test-cases)
 
 
 ## Description
 
 Expands the existing [Django](https://docs.djangoproject.com/en/dev/)
 [TestCase class](https://docs.djangoproject.com/en/dev/topics/testing/overview/) with extra functionality.
 
 Different TestCase classes are provided, each providing separate sets of functionality.
 
 
+For full documentation, see [ReadTheDocs](https://django-expanded-test-cases.readthedocs.io/en/latest/).
+
+
+## Example ETC Debug Output on UnitTest Error
+A main functionality that **ExpandedTestCases** provides is verbose response debug info on UnitTest errors.<br>
+Below is an example of such output, when a test fails while checking the `<h1>` tag for a very simple page.
+
+![ETC Error Debug Output Screenshot](https://user-images.githubusercontent.com/14208531/231304818-fb0dbe31-ead9-4de8-8efe-a3fc858cbddd.png)
+
+
 ## Installation
 
 Install with
 
     pip install django-expanded-test-cases
 
+For full color output, also install
 
-## Documentation
-
-For full documentation, see [ReadTheDocs](https://django-expanded-test-cases.readthedocs.io/en/latest/).
-
+    pip install colorama
 
 ## Package Development & Running Project Tests
 
 As standard for Python development, this project has its own testing to ensure it functions as desired.
 After installing dependencies, everything required to run tests are provided in one of two files:
 * To run tests via standard django `python manage.py test`, execute the `<project_root>/runtests.py` file.
 * To run tests via `pytest`, execute the `<project_root>/runpytests.py` file.
```

### Comparing `django-expanded-test-cases-0.2.3/django_expanded_test_cases.egg-info/SOURCES.txt` & `django-expanded-test-cases-0.2.4/django_expanded_test_cases.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.2.3/pyproject.toml` & `django-expanded-test-cases-0.2.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=40.8.0', 'wheel']
 build-backend = 'setuptools.build_meta:__legacy__'
 
 [project]
 name = "django-expanded-test-cases"
-version = "0.2.3"
+version = "0.2.4"
 description = "Expands the existing Django TestCase class with extra functionality."
 readme = "readme.md"
 authors = [
     { name = "Brandon Rodriguez", email = "brodriguez8774@gmail.com" },
 ]
 maintainers = [
     { name = "Brandon Rodriguez", email = "brodriguez8774@gmail.com" },
@@ -29,14 +29,15 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
 ]
 keywords = [
     "django",
     "testcases",
     "tests",
```

### Comparing `django-expanded-test-cases-0.2.3/setup.cfg` & `django-expanded-test-cases-0.2.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-expanded-test-cases
-version = 0.2.3
+version = 0.2.4
 description = Expands the existing Django TestCase class with extra functionality.
 long_description = file: readme.md
 url = https://github.com/brodriguez8774/django-expanded-test-cases
 author = Brandon Rodriguez
 author_email = brodriguez8774@gmail.com
 license = MIT License
 classifiers =
```

### Comparing `django-expanded-test-cases-0.2.3/tests/settings.py` & `django-expanded-test-cases-0.2.4/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.2.3/tests/test_cases/test_base_case.py` & `django-expanded-test-cases-0.2.4/tests/test_cases/test_base_case.py`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.2.3/tests/test_cases/test_integration_case.py` & `django-expanded-test-cases-0.2.4/tests/test_cases/test_integration_case.py`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.2.3/tests/test_cases/test_live_server_case.py` & `django-expanded-test-cases-0.2.4/tests/test_cases/test_live_server_case.py`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.2.3/tests/views.py` & `django-expanded-test-cases-0.2.4/tests/views.py`

 * *Files identical despite different names*

