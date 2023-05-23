# Comparing `tmp/django_htmx_ui-0.1.7.tar.gz` & `tmp/django_htmx_ui-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_htmx_ui-0.1.7.tar", last modified: Sat May 13 15:18:50 2023, max compression
+gzip compressed data, was "django_htmx_ui-0.1.8.tar", last modified: Tue May 23 09:04:51 2023, max compression
```

## Comparing `django_htmx_ui-0.1.7.tar` & `django_htmx_ui-0.1.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 nikalexis  (1000) nikalexis  (1000)        0 2023-05-13 15:18:50.639803 django_htmx_ui-0.1.7/
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)     1075 2023-02-27 22:03:36.000000 django_htmx_ui-0.1.7/LICENSE
--rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)    31385 2023-05-13 15:18:50.639803 django_htmx_ui-0.1.7/PKG-INFO
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)    30835 2023-05-13 15:16:36.000000 django_htmx_ui-0.1.7/README.md
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)      721 2023-05-13 15:17:17.000000 django_htmx_ui-0.1.7/pyproject.toml
--rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)       38 2023-05-13 15:18:50.639803 django_htmx_ui-0.1.7/setup.cfg
-drwxr-xr-x   0 nikalexis  (1000) nikalexis  (1000)        0 2023-05-13 15:18:50.639803 django_htmx_ui-0.1.7/src/
-drwxr-xr-x   0 nikalexis  (1000) nikalexis  (1000)        0 2023-05-13 15:18:50.639803 django_htmx_ui-0.1.7/src/django_htmx_ui/
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)        0 2023-02-08 11:09:09.000000 django_htmx_ui-0.1.7/src/django_htmx_ui/__init__.py
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)        0 2023-02-08 11:09:09.000000 django_htmx_ui-0.1.7/src/django_htmx_ui/admin.py
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)      158 2023-02-08 11:09:09.000000 django_htmx_ui-0.1.7/src/django_htmx_ui/apps.py
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)        0 2023-02-08 11:09:09.000000 django_htmx_ui-0.1.7/src/django_htmx_ui/forms.py
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)     1877 2023-05-05 09:20:03.000000 django_htmx_ui-0.1.7/src/django_htmx_ui/jinja.py
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)     1744 2023-02-08 11:09:09.000000 django_htmx_ui-0.1.7/src/django_htmx_ui/middleware.py
-drwxr-xr-x   0 nikalexis  (1000) nikalexis  (1000)        0 2023-05-13 15:18:50.639803 django_htmx_ui-0.1.7/src/django_htmx_ui/migrations/
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)        0 2023-02-08 11:09:09.000000 django_htmx_ui-0.1.7/src/django_htmx_ui/migrations/__init__.py
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)        0 2023-02-08 11:09:09.000000 django_htmx_ui-0.1.7/src/django_htmx_ui/models.py
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)       60 2023-02-08 11:09:09.000000 django_htmx_ui-0.1.7/src/django_htmx_ui/tests.py
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)        0 2023-02-08 11:09:09.000000 django_htmx_ui-0.1.7/src/django_htmx_ui/urls.py
--rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)     7557 2023-04-25 13:45:56.000000 django_htmx_ui-0.1.7/src/django_htmx_ui/utils.py
-drwxr-xr-x   0 nikalexis  (1000) nikalexis  (1000)        0 2023-05-13 15:18:50.639803 django_htmx_ui-0.1.7/src/django_htmx_ui/views/
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)     1929 2023-02-26 11:45:23.000000 django_htmx_ui-0.1.7/src/django_htmx_ui/views/crud.py
--rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)     7167 2023-04-25 13:45:56.000000 django_htmx_ui-0.1.7/src/django_htmx_ui/views/generic.py
--rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)     7764 2023-04-25 13:45:56.000000 django_htmx_ui-0.1.7/src/django_htmx_ui/views/mixins.py
-drwxr-xr-x   0 nikalexis  (1000) nikalexis  (1000)        0 2023-05-13 15:18:50.639803 django_htmx_ui-0.1.7/src/django_htmx_ui.egg-info/
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)    31385 2023-05-13 15:18:50.000000 django_htmx_ui-0.1.7/src/django_htmx_ui.egg-info/PKG-INFO
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)      674 2023-05-13 15:18:50.000000 django_htmx_ui-0.1.7/src/django_htmx_ui.egg-info/SOURCES.txt
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)        1 2023-05-13 15:18:50.000000 django_htmx_ui-0.1.7/src/django_htmx_ui.egg-info/dependency_links.txt
--rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)       50 2023-05-13 15:18:50.000000 django_htmx_ui-0.1.7/src/django_htmx_ui.egg-info/requires.txt
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)       15 2023-05-13 15:18:50.000000 django_htmx_ui-0.1.7/src/django_htmx_ui.egg-info/top_level.txt
+drwxr-xr-x   0 nikalexis  (1000) nikalexis  (1000)        0 2023-05-23 09:04:51.053531 django_htmx_ui-0.1.8/
+-rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)     1075 2023-02-28 15:45:04.000000 django_htmx_ui-0.1.8/LICENSE
+-rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)    31385 2023-05-23 09:04:51.053531 django_htmx_ui-0.1.8/PKG-INFO
+-rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)    30835 2023-05-13 15:25:42.000000 django_htmx_ui-0.1.8/README.md
+-rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)      721 2023-05-23 09:03:39.000000 django_htmx_ui-0.1.8/pyproject.toml
+-rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)       38 2023-05-23 09:04:51.053531 django_htmx_ui-0.1.8/setup.cfg
+drwxr-xr-x   0 nikalexis  (1000) nikalexis  (1000)        0 2023-05-23 09:04:51.043531 django_htmx_ui-0.1.8/src/
+drwxr-xr-x   0 nikalexis  (1000) nikalexis  (1000)        0 2023-05-23 09:04:51.053531 django_htmx_ui-0.1.8/src/django_htmx_ui/
+-rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)        0 2023-04-26 08:53:11.000000 django_htmx_ui-0.1.8/src/django_htmx_ui/__init__.py
+-rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)        0 2023-02-28 15:45:04.000000 django_htmx_ui-0.1.8/src/django_htmx_ui/admin.py
+-rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)      158 2023-02-28 15:45:04.000000 django_htmx_ui-0.1.8/src/django_htmx_ui/apps.py
+-rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)        0 2023-02-28 15:45:04.000000 django_htmx_ui-0.1.8/src/django_htmx_ui/forms.py
+-rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)     1877 2023-05-13 15:25:42.000000 django_htmx_ui-0.1.8/src/django_htmx_ui/jinja.py
+-rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)     1744 2023-02-28 15:45:04.000000 django_htmx_ui-0.1.8/src/django_htmx_ui/middleware.py
+drwxr-xr-x   0 nikalexis  (1000) nikalexis  (1000)        0 2023-05-23 09:04:51.053531 django_htmx_ui-0.1.8/src/django_htmx_ui/migrations/
+-rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)        0 2023-02-28 15:45:04.000000 django_htmx_ui-0.1.8/src/django_htmx_ui/migrations/__init__.py
+-rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)        0 2023-02-28 15:45:04.000000 django_htmx_ui-0.1.8/src/django_htmx_ui/models.py
+-rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)       60 2023-02-28 15:45:04.000000 django_htmx_ui-0.1.8/src/django_htmx_ui/tests.py
+-rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)        0 2023-02-28 15:45:04.000000 django_htmx_ui-0.1.8/src/django_htmx_ui/urls.py
+-rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)     7557 2023-04-25 13:39:33.000000 django_htmx_ui-0.1.8/src/django_htmx_ui/utils.py
+drwxr-xr-x   0 nikalexis  (1000) nikalexis  (1000)        0 2023-05-23 09:04:51.053531 django_htmx_ui-0.1.8/src/django_htmx_ui/views/
+-rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)     1929 2023-02-28 15:45:04.000000 django_htmx_ui-0.1.8/src/django_htmx_ui/views/crud.py
+-rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)     7167 2023-04-25 13:35:41.000000 django_htmx_ui-0.1.8/src/django_htmx_ui/views/generic.py
+-rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)     7804 2023-05-22 11:38:41.000000 django_htmx_ui-0.1.8/src/django_htmx_ui/views/mixins.py
+drwxr-xr-x   0 nikalexis  (1000) nikalexis  (1000)        0 2023-05-23 09:04:51.053531 django_htmx_ui-0.1.8/src/django_htmx_ui.egg-info/
+-rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)    31385 2023-05-23 09:04:51.000000 django_htmx_ui-0.1.8/src/django_htmx_ui.egg-info/PKG-INFO
+-rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)      674 2023-05-23 09:04:51.000000 django_htmx_ui-0.1.8/src/django_htmx_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)        1 2023-05-23 09:04:51.000000 django_htmx_ui-0.1.8/src/django_htmx_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)       50 2023-05-23 09:04:51.000000 django_htmx_ui-0.1.8/src/django_htmx_ui.egg-info/requires.txt
+-rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)       15 2023-05-23 09:04:51.000000 django_htmx_ui-0.1.8/src/django_htmx_ui.egg-info/top_level.txt
```

### Comparing `django_htmx_ui-0.1.7/LICENSE` & `django_htmx_ui-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django_htmx_ui-0.1.7/PKG-INFO` & `django_htmx_ui-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_htmx_ui
-Version: 0.1.7
+Version: 0.1.8
 Summary: Django - HTMX - Jinja powerful combination library
 Author-email: Nikalexis Nikolaos <nikalexis@gmail.com>
 Project-URL: Homepage, https://github.com/nikalexis/django_htmx_ui
 Project-URL: Bug Tracker, https://github.com/nikalexis/django_htmx_ui/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `django_htmx_ui-0.1.7/README.md` & `django_htmx_ui-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `django_htmx_ui-0.1.7/pyproject.toml` & `django_htmx_ui-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django_htmx_ui"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   { name="Nikalexis Nikolaos", email="nikalexis@gmail.com" },
 ]
 description = "Django - HTMX - Jinja powerful combination library"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `django_htmx_ui-0.1.7/src/django_htmx_ui/jinja.py` & `django_htmx_ui-0.1.8/src/django_htmx_ui/jinja.py`

 * *Files identical despite different names*

### Comparing `django_htmx_ui-0.1.7/src/django_htmx_ui/middleware.py` & `django_htmx_ui-0.1.8/src/django_htmx_ui/middleware.py`

 * *Files identical despite different names*

### Comparing `django_htmx_ui-0.1.7/src/django_htmx_ui/utils.py` & `django_htmx_ui-0.1.8/src/django_htmx_ui/utils.py`

 * *Files identical despite different names*

### Comparing `django_htmx_ui-0.1.7/src/django_htmx_ui/views/crud.py` & `django_htmx_ui-0.1.8/src/django_htmx_ui/views/crud.py`

 * *Files identical despite different names*

### Comparing `django_htmx_ui-0.1.7/src/django_htmx_ui/views/generic.py` & `django_htmx_ui-0.1.8/src/django_htmx_ui/views/generic.py`

 * *Files identical despite different names*

### Comparing `django_htmx_ui-0.1.7/src/django_htmx_ui/views/mixins.py` & `django_htmx_ui-0.1.8/src/django_htmx_ui/views/mixins.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,17 +43,17 @@
             if self.request.method == 'GET':
                 if self.form_instance:
                     return Form(instance=self.form_instance, initial=self.form_initial)
                 else:
                     return Form(initial=self.form_initial)
             if self.request.method == 'POST':
                 if self.form_instance:
-                    return Form(self.request.POST, instance=self.form_instance)
+                    return Form(self.request.POST, self.request.FILES, instance=self.form_instance)
                 else:
-                    return Form(self.request.POST)
+                    return Form(self.request.POST, self.request.FILES)
 
     def on_post(self, request, *args, **kwargs):
         if self.form.is_valid():
             self.form.save()
             self.on_post_success_message(request, *args, **kwargs)
             return self.on_post_success(request, *args, **kwargs)
         else:
```

### Comparing `django_htmx_ui-0.1.7/src/django_htmx_ui.egg-info/PKG-INFO` & `django_htmx_ui-0.1.8/src/django_htmx_ui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-htmx-ui
-Version: 0.1.7
+Version: 0.1.8
 Summary: Django - HTMX - Jinja powerful combination library
 Author-email: Nikalexis Nikolaos <nikalexis@gmail.com>
 Project-URL: Homepage, https://github.com/nikalexis/django_htmx_ui
 Project-URL: Bug Tracker, https://github.com/nikalexis/django_htmx_ui/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `django_htmx_ui-0.1.7/src/django_htmx_ui.egg-info/SOURCES.txt` & `django_htmx_ui-0.1.8/src/django_htmx_ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

