# Comparing `tmp/django-autoutils-1.2.0.tar.gz` & `tmp/django_autoutils-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-autoutils-1.2.0.tar", max compression
+gzip compressed data, was "django_autoutils-1.3.0.tar", max compression
```

## Comparing `django-autoutils-1.2.0.tar` & `django_autoutils-1.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1067 2022-01-21 08:24:24.883039 django-autoutils-1.2.0/LICENSE
--rw-r--r--   0        0        0       18 2022-01-21 08:24:24.883039 django-autoutils-1.2.0/README.md
--rw-r--r--   0        0        0        0 2022-01-21 08:27:10.740707 django-autoutils-1.2.0/django_autoutils/__init__.py
--rw-r--r--   0        0        0        0 2022-12-16 15:20:19.866000 django-autoutils-1.2.0/django_autoutils/admin_numeric_filter/__init__.py
--rw-r--r--   0        0        0     6217 2022-12-16 15:20:19.866000 django-autoutils-1.2.0/django_autoutils/admin_numeric_filter/admin.py
--rw-r--r--   0        0        0     1218 2022-12-16 15:20:19.866000 django-autoutils-1.2.0/django_autoutils/admin_numeric_filter/forms.py
--rw-r--r--   0        0        0     2552 2022-12-16 15:20:19.866000 django-autoutils-1.2.0/django_autoutils/admin_numeric_filter/static/css/admin-numeric-filter.css
--rw-r--r--   0        0        0     1604 2022-12-16 15:20:19.866000 django-autoutils-1.2.0/django_autoutils/admin_numeric_filter/static/js/admin-numeric-filter.js
--rw-r--r--   0        0        0     3843 2022-12-16 15:20:19.866000 django-autoutils-1.2.0/django_autoutils/admin_numeric_filter/static/js/nouislider.min.css
--rw-r--r--   0        0        0    22056 2022-12-16 15:20:19.866000 django-autoutils-1.2.0/django_autoutils/admin_numeric_filter/static/js/nouislider.min.js
--rwxr-xr-x   0        0        0     2286 2022-12-16 15:20:19.866000 django-autoutils-1.2.0/django_autoutils/admin_numeric_filter/static/js/wNumb.min.js
--rw-r--r--   0        0        0      736 2022-12-16 15:20:19.870000 django-autoutils-1.2.0/django_autoutils/admin_numeric_filter/templates/admin/filter_numeric_range.html
--rw-r--r--   0        0        0      557 2022-12-16 15:20:19.870000 django-autoutils-1.2.0/django_autoutils/admin_numeric_filter/templates/admin/filter_numeric_single.html
--rw-r--r--   0        0        0     1711 2022-12-16 15:20:19.870000 django-autoutils-1.2.0/django_autoutils/admin_numeric_filter/templates/admin/filter_numeric_slider.html
--rw-r--r--   0        0        0     9207 2022-12-16 15:29:47.520813 django-autoutils-1.2.0/django_autoutils/admin_utils.py
--rw-r--r--   0        0        0      991 2022-05-20 11:54:20.568959 django-autoutils-1.2.0/django_autoutils/exceptions.py
--rw-r--r--   0        0        0     3537 2022-05-21 14:25:24.315842 django-autoutils-1.2.0/django_autoutils/html_tag.py
--rw-r--r--   0        0        0     8546 2023-01-27 19:49:34.614085 django-autoutils-1.2.0/django_autoutils/model_utils.py
--rw-r--r--   0        0        0      792 2022-05-27 07:59:32.911496 django-autoutils-1.2.0/django_autoutils/serializer_utils.py
--rw-r--r--   0        0        0     2093 2022-05-27 08:26:01.726972 django-autoutils-1.2.0/django_autoutils/utils.py
--rw-r--r--   0        0        0      891 2023-04-18 20:33:59.462818 django-autoutils-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1125 2023-04-18 20:34:01.327783 django-autoutils-1.2.0/setup.py
--rw-r--r--   0        0        0     1057 2023-04-18 20:34:01.328040 django-autoutils-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-23 17:20:49.044355 django_autoutils-1.3.0/LICENSE
+-rw-r--r--   0        0        0       18 2023-05-23 17:20:49.044355 django_autoutils-1.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 17:20:49.044355 django_autoutils-1.3.0/django_autoutils/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 17:20:49.044355 django_autoutils-1.3.0/django_autoutils/admin_numeric_filter/__init__.py
+-rw-r--r--   0        0        0     6217 2023-05-23 17:20:49.044355 django_autoutils-1.3.0/django_autoutils/admin_numeric_filter/admin.py
+-rw-r--r--   0        0        0     1218 2023-05-23 17:20:49.044355 django_autoutils-1.3.0/django_autoutils/admin_numeric_filter/forms.py
+-rw-r--r--   0        0        0     2552 2023-05-23 17:20:49.044355 django_autoutils-1.3.0/django_autoutils/admin_numeric_filter/static/css/admin-numeric-filter.css
+-rw-r--r--   0        0        0     1604 2023-05-23 17:20:49.044355 django_autoutils-1.3.0/django_autoutils/admin_numeric_filter/static/js/admin-numeric-filter.js
+-rw-r--r--   0        0        0     3843 2023-05-23 17:20:49.044355 django_autoutils-1.3.0/django_autoutils/admin_numeric_filter/static/js/nouislider.min.css
+-rw-r--r--   0        0        0    22056 2023-05-23 17:20:49.044355 django_autoutils-1.3.0/django_autoutils/admin_numeric_filter/static/js/nouislider.min.js
+-rwxr-xr-x   0        0        0     2286 2023-05-23 17:20:49.048354 django_autoutils-1.3.0/django_autoutils/admin_numeric_filter/static/js/wNumb.min.js
+-rw-r--r--   0        0        0      736 2023-05-23 17:20:49.048354 django_autoutils-1.3.0/django_autoutils/admin_numeric_filter/templates/admin/filter_numeric_range.html
+-rw-r--r--   0        0        0      557 2023-05-23 17:20:49.048354 django_autoutils-1.3.0/django_autoutils/admin_numeric_filter/templates/admin/filter_numeric_single.html
+-rw-r--r--   0        0        0     1711 2023-05-23 17:20:49.048354 django_autoutils-1.3.0/django_autoutils/admin_numeric_filter/templates/admin/filter_numeric_slider.html
+-rw-r--r--   0        0        0     9207 2023-05-23 17:20:49.048354 django_autoutils-1.3.0/django_autoutils/admin_utils.py
+-rw-r--r--   0        0        0      991 2023-05-23 17:20:49.048354 django_autoutils-1.3.0/django_autoutils/exceptions.py
+-rw-r--r--   0        0        0     3537 2023-05-23 17:20:49.048354 django_autoutils-1.3.0/django_autoutils/html_tag.py
+-rw-r--r--   0        0        0     1486 2023-05-23 17:24:37.691716 django_autoutils-1.3.0/django_autoutils/managers.py
+-rw-r--r--   0        0        0     8546 2023-05-23 17:20:49.048354 django_autoutils-1.3.0/django_autoutils/model_utils.py
+-rw-r--r--   0        0        0      792 2023-05-23 17:20:49.048354 django_autoutils-1.3.0/django_autoutils/serializer_utils.py
+-rw-r--r--   0        0        0     2093 2023-05-23 17:20:49.048354 django_autoutils-1.3.0/django_autoutils/utils.py
+-rw-r--r--   0        0        0      890 2023-05-23 17:24:21.836500 django_autoutils-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1161 1970-01-01 00:00:00.000000 django_autoutils-1.3.0/PKG-INFO
```

### Comparing `django-autoutils-1.2.0/LICENSE` & `django_autoutils-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-autoutils-1.2.0/django_autoutils/admin_numeric_filter/admin.py` & `django_autoutils-1.3.0/django_autoutils/admin_numeric_filter/admin.py`

 * *Files identical despite different names*

### Comparing `django-autoutils-1.2.0/django_autoutils/admin_numeric_filter/forms.py` & `django_autoutils-1.3.0/django_autoutils/admin_numeric_filter/forms.py`

 * *Files identical despite different names*

### Comparing `django-autoutils-1.2.0/django_autoutils/admin_numeric_filter/static/css/admin-numeric-filter.css` & `django_autoutils-1.3.0/django_autoutils/admin_numeric_filter/static/css/admin-numeric-filter.css`

 * *Files identical despite different names*

### Comparing `django-autoutils-1.2.0/django_autoutils/admin_numeric_filter/static/js/admin-numeric-filter.js` & `django_autoutils-1.3.0/django_autoutils/admin_numeric_filter/static/js/admin-numeric-filter.js`

 * *Files identical despite different names*

### Comparing `django-autoutils-1.2.0/django_autoutils/admin_numeric_filter/static/js/nouislider.min.css` & `django_autoutils-1.3.0/django_autoutils/admin_numeric_filter/static/js/nouislider.min.css`

 * *Files identical despite different names*

### Comparing `django-autoutils-1.2.0/django_autoutils/admin_numeric_filter/static/js/nouislider.min.js` & `django_autoutils-1.3.0/django_autoutils/admin_numeric_filter/static/js/nouislider.min.js`

 * *Files identical despite different names*

### Comparing `django-autoutils-1.2.0/django_autoutils/admin_numeric_filter/static/js/wNumb.min.js` & `django_autoutils-1.3.0/django_autoutils/admin_numeric_filter/static/js/wNumb.min.js`

 * *Files identical despite different names*

### Comparing `django-autoutils-1.2.0/django_autoutils/admin_numeric_filter/templates/admin/filter_numeric_range.html` & `django_autoutils-1.3.0/django_autoutils/admin_numeric_filter/templates/admin/filter_numeric_range.html`

 * *Files identical despite different names*

### Comparing `django-autoutils-1.2.0/django_autoutils/admin_numeric_filter/templates/admin/filter_numeric_single.html` & `django_autoutils-1.3.0/django_autoutils/admin_numeric_filter/templates/admin/filter_numeric_single.html`

 * *Files identical despite different names*

### Comparing `django-autoutils-1.2.0/django_autoutils/admin_numeric_filter/templates/admin/filter_numeric_slider.html` & `django_autoutils-1.3.0/django_autoutils/admin_numeric_filter/templates/admin/filter_numeric_slider.html`

 * *Files identical despite different names*

### Comparing `django-autoutils-1.2.0/django_autoutils/admin_utils.py` & `django_autoutils-1.3.0/django_autoutils/admin_utils.py`

 * *Files identical despite different names*

### Comparing `django-autoutils-1.2.0/django_autoutils/exceptions.py` & `django_autoutils-1.3.0/django_autoutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-autoutils-1.2.0/django_autoutils/html_tag.py` & `django_autoutils-1.3.0/django_autoutils/html_tag.py`

 * *Files identical despite different names*

### Comparing `django-autoutils-1.2.0/django_autoutils/model_utils.py` & `django_autoutils-1.3.0/django_autoutils/model_utils.py`

 * *Files identical despite different names*

### Comparing `django-autoutils-1.2.0/django_autoutils/serializer_utils.py` & `django_autoutils-1.3.0/django_autoutils/serializer_utils.py`

 * *Files identical despite different names*

### Comparing `django-autoutils-1.2.0/django_autoutils/utils.py` & `django_autoutils-1.3.0/django_autoutils/utils.py`

 * *Files identical despite different names*

### Comparing `django-autoutils-1.2.0/pyproject.toml` & `django_autoutils-1.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-autoutils"
-version = "1.2.0"
+version = "1.3.0"
 description = "Some Good Function In Django"
 authors = ["Reza Zeiny <rezazeiny1998@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/rezazeiny/django-autoutils"
 repository = "https://github.com/rezazeiny/django-autoutils"
 keywords = ["django-autoutils"]
@@ -17,15 +17,15 @@
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 Django = "^4.0"
 djangorestframework = "^3.0"
-autoutils = ">=0.5"
+autoutils = "^0.5"
 Pygments = "^2.0"
 django-admin-autocomplete-filter = "^0.7"
 Markdown = "^3.0"
 Pillow = "^9.0"
 django-admin-list-filter-dropdown = "^1.0"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `django-autoutils-1.2.0/PKG-INFO` & `django_autoutils-1.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: django-autoutils
-Version: 1.2.0
+Version: 1.3.0
 Summary: Some Good Function In Django
 Home-page: https://github.com/rezazeiny/django-autoutils
 License: MIT
 Keywords: django-autoutils
 Author: Reza Zeiny
 Author-email: rezazeiny1998@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Requires-Dist: Django (>=4.0,<5.0)
 Requires-Dist: Markdown (>=3.0,<4.0)
 Requires-Dist: Pillow (>=9.0,<10.0)
 Requires-Dist: Pygments (>=2.0,<3.0)
-Requires-Dist: autoutils (>=0.5)
+Requires-Dist: autoutils (>=0.5,<0.6)
 Requires-Dist: django-admin-autocomplete-filter (>=0.7,<0.8)
 Requires-Dist: django-admin-list-filter-dropdown (>=1.0,<2.0)
 Requires-Dist: djangorestframework (>=3.0,<4.0)
 Project-URL: Repository, https://github.com/rezazeiny/django-autoutils
 Description-Content-Type: text/markdown
 
 # django-autoutils
```

