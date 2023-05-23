# Comparing `tmp/django-select2-8.1.1.tar.gz` & `tmp/django_select2-8.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-select2-8.1.1.tar", last modified: Fri Mar 10 20:21:51 2023, max compression
+gzip compressed data, was "django_select2-8.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django-select2-8.1.1.tar` & `django_select2-8.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1094 2023-03-10 20:21:31.010087 django-select2-8.1.1/LICENSE
--rw-r--r--   0        0        0     1119 2023-03-10 20:21:31.010087 django-select2-8.1.1/README.rst
--rw-r--r--   0        0        0      414 2023-03-10 20:21:31.010087 django-select2-8.1.1/django_select2/__init__.py
--rw-r--r--   0        0        0      160 2023-03-10 20:21:51.094092 django-select2-8.1.1/django_select2/_version.py
--rw-r--r--   0        0        0      270 2023-03-10 20:21:31.010087 django-select2-8.1.1/django_select2/apps.py
--rw-r--r--   0        0        0      549 2023-03-10 20:21:31.010087 django-select2-8.1.1/django_select2/cache.py
--rw-r--r--   0        0        0     5401 2023-03-10 20:21:31.010087 django-select2-8.1.1/django_select2/conf.py
--rw-r--r--   0        0        0    20409 2023-03-10 20:21:31.010087 django-select2-8.1.1/django_select2/forms.py
--rw-r--r--   0        0        0       54 2023-03-10 20:21:31.010087 django-select2-8.1.1/django_select2/static/django_select2/django_select2.css
--rw-r--r--   0        0        0     2051 2023-03-10 20:21:31.010087 django-select2-8.1.1/django_select2/static/django_select2/django_select2.js
--rw-r--r--   0        0        0      400 2023-03-10 20:21:31.010087 django-select2-8.1.1/django_select2/urls.py
--rw-r--r--   0        0        0     3440 2023-03-10 20:21:31.010087 django-select2-8.1.1/django_select2/views.py
--rw-r--r--   0        0        0     2195 2023-03-10 20:21:31.014087 django-select2-8.1.1/pyproject.toml
--rw-r--r--   0        0        0     2863 1970-01-01 00:00:00.000000 django-select2-8.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-05-23 14:31:36.392133 django_select2-8.1.2/LICENSE
+-rw-r--r--   0        0        0     1119 2023-05-23 14:31:36.392133 django_select2-8.1.2/README.rst
+-rw-r--r--   0        0        0      414 2023-05-23 14:31:36.392133 django_select2-8.1.2/django_select2/__init__.py
+-rw-r--r--   0        0        0      160 2023-05-23 14:31:59.216147 django_select2-8.1.2/django_select2/_version.py
+-rw-r--r--   0        0        0      270 2023-05-23 14:31:36.392133 django_select2-8.1.2/django_select2/apps.py
+-rw-r--r--   0        0        0      549 2023-05-23 14:31:36.392133 django_select2-8.1.2/django_select2/cache.py
+-rw-r--r--   0        0        0     5401 2023-05-23 14:31:36.392133 django_select2-8.1.2/django_select2/conf.py
+-rw-r--r--   0        0        0    20646 2023-05-23 14:31:36.392133 django_select2-8.1.2/django_select2/forms.py
+-rw-r--r--   0        0        0       54 2023-05-23 14:31:36.392133 django_select2-8.1.2/django_select2/static/django_select2/django_select2.css
+-rw-r--r--   0        0        0     2051 2023-05-23 14:31:36.392133 django_select2-8.1.2/django_select2/static/django_select2/django_select2.js
+-rw-r--r--   0        0        0      400 2023-05-23 14:31:36.392133 django_select2-8.1.2/django_select2/urls.py
+-rw-r--r--   0        0        0     3440 2023-05-23 14:31:36.392133 django_select2-8.1.2/django_select2/views.py
+-rw-r--r--   0        0        0     2319 2023-05-23 14:31:36.396133 django_select2-8.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2914 1970-01-01 00:00:00.000000 django_select2-8.1.2/PKG-INFO
```

### Comparing `django-select2-8.1.1/LICENSE` & `django_select2-8.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-select2-8.1.1/README.rst` & `django_select2-8.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `django-select2-8.1.1/django_select2/cache.py` & `django_select2-8.1.2/django_select2/cache.py`

 * *Files identical despite different names*

### Comparing `django-select2-8.1.1/django_select2/conf.py` & `django_select2-8.1.2/django_select2/conf.py`

 * *Files identical despite different names*

### Comparing `django-select2-8.1.1/django_select2/forms.py` & `django_select2-8.1.2/django_select2/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,20 +50,19 @@
 import uuid
 from functools import reduce
 from itertools import chain
 from pickle import PicklingError  # nosec
 
 import django
 from django import forms
-from django.contrib.admin.widgets import SELECT2_TRANSLATIONS, AutocompleteMixin
+from django.contrib.admin.widgets import AutocompleteMixin
 from django.core import signing
 from django.db.models import Q
 from django.forms.models import ModelChoiceIterator
 from django.urls import reverse
-from django.utils.translation import get_language
 
 from .cache import cache
 from .conf import settings
 
 if django.VERSION < (4, 0):
     from django.contrib.admin.utils import (
         lookup_needs_distinct as lookup_spawns_duplicates,
@@ -85,15 +84,23 @@
     theme = None
 
     empty_label = ""
 
     @property
     def i18n_name(self):
         """Name of the i18n file for the current language."""
-        return SELECT2_TRANSLATIONS.get(get_language())
+        if django.VERSION < (4, 1):
+            from django.contrib.admin.widgets import SELECT2_TRANSLATIONS
+            from django.utils.translation import get_language
+
+            return SELECT2_TRANSLATIONS.get(get_language())
+        else:
+            from django.contrib.admin.widgets import get_select2_language
+
+            return get_select2_language()
 
     def build_attrs(self, base_attrs, extra_attrs=None):
         """Add select2 data attributes."""
         default_attrs = {
             "lang": self.i18n_name,
             "data-minimum-input-length": 0,
             "data-theme": self.theme or settings.SELECT2_THEME,
@@ -254,15 +261,15 @@
         self.data_view = kwargs.pop("data_view", self.data_view)
         self.data_url = kwargs.pop("data_url", self.data_url)
 
         dependent_fields = kwargs.pop("dependent_fields", None)
         if dependent_fields is not None:
             self.dependent_fields = dict(dependent_fields)
         if not (self.data_view or self.data_url):
-            raise ValueError('You must ether specify "data_view" or "data_url".')
+            raise ValueError('You must either specify "data_view" or "data_url".')
         self.userGetValTextFuncName = kwargs.pop("userGetValTextFuncName", "null")
 
     def get_url(self):
         """Return URL from instance or by reversing :attr:`.data_view`."""
         if self.data_url:
             return self.data_url
         return reverse(self.data_view)
```

### Comparing `django-select2-8.1.1/django_select2/static/django_select2/django_select2.js` & `django_select2-8.1.2/django_select2/static/django_select2/django_select2.js`

 * *Files identical despite different names*

### Comparing `django-select2-8.1.1/django_select2/views.py` & `django_select2-8.1.2/django_select2/views.py`

 * *Files identical despite different names*

### Comparing `django-select2-8.1.1/pyproject.toml` & `django_select2-8.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -16,21 +16,22 @@
   "License :: OSI Approved :: MIT License",
   "Intended Audience :: Developers",
   "Environment :: Web Environment",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
-  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
   "Framework :: Django",
   "Framework :: Django :: 3.2",
-  "Framework :: Django :: 4.0",
   "Framework :: Django :: 4.1",
+  "Framework :: Django :: 4.2",
   "Topic :: Software Development",
 ]
 requires-python = ">=3.8"
 dependencies = [
   "django>=3.2",
   "django-appconf>=0.6.0"
 ]
@@ -63,14 +64,15 @@
 write_to = "django_select2/_version.py"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "--cov --tb=short -rxs"
 testpaths = ["tests"]
 DJANGO_SETTINGS_MODULE = "tests.testapp.settings"
+filterwarnings = ["ignore::PendingDeprecationWarning", "error::RuntimeWarning"]
 
 [tool.coverage.run]
 source = ["django_select2"]
 
 [tool.coverage.report]
 show_missing = true
```

### Comparing `django-select2-8.1.1/PKG-INFO` & `django_select2-8.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: django-select2
-Version: 8.1.1
+Version: 8.1.2
 Summary: This is a Django_ integration of Select2_.
 Keywords: Django,select2,autocomplete,typeahead
 Author-email: Johannes Maron <johannes@maron.family>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Topic :: Software Development
 Requires-Dist: django>=3.2
 Requires-Dist: django-appconf>=0.6.0
 Requires-Dist: sphinx ; extra == "docs"
 Requires-Dist: selenium ; extra == "selenium"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
```

