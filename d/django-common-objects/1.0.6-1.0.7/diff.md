# Comparing `tmp/django-common-objects-1.0.6.tar.gz` & `tmp/django-common-objects-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-common-objects-1.0.6.tar", last modified: Wed May 17 03:16:49 2023, max compression
+gzip compressed data, was "django-common-objects-1.0.7.tar", last modified: Tue May 23 08:58:55 2023, max compression
```

## Comparing `django-common-objects-1.0.6.tar` & `django-common-objects-1.0.7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 03:16:49.919515 django-common-objects-1.0.6/
--rw-rw-rw-   0        0        0     1085 2023-02-28 03:17:44.000000 django-common-objects-1.0.6/LICENSE
--rw-rw-rw-   0        0        0      296 2023-05-17 03:16:49.919515 django-common-objects-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       21 2023-02-28 03:17:44.000000 django-common-objects-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 03:16:49.865767 django-common-objects-1.0.6/django_common_objects/
--rw-rw-rw-   0        0        0        0 2023-02-28 03:21:57.000000 django-common-objects-1.0.6/django_common_objects/__init__.py
--rw-rw-rw-   0        0        0     5521 2023-02-28 03:24:51.000000 django-common-objects-1.0.6/django_common_objects/admin.py
--rw-rw-rw-   0        0        0      155 2023-02-28 03:45:02.000000 django-common-objects-1.0.6/django_common_objects/apps.py
--rw-rw-rw-   0        0        0     2580 2023-02-28 03:45:52.000000 django-common-objects-1.0.6/django_common_objects/choices.py
--rw-rw-rw-   0        0        0     1498 2023-02-28 03:29:27.000000 django-common-objects-1.0.6/django_common_objects/fields.py
--rw-rw-rw-   0        0        0     2033 2023-05-17 02:59:55.000000 django-common-objects-1.0.6/django_common_objects/forms.py
-drwxrwxrwx   0        0        0        0 2023-05-17 03:16:49.897309 django-common-objects-1.0.6/django_common_objects/migrations/
--rw-rw-rw-   0        0        0     4132 2023-05-17 03:14:17.000000 django-common-objects-1.0.6/django_common_objects/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      832 2023-04-04 01:15:03.000000 django-common-objects-1.0.6/django_common_objects/migrations/0002_alter_commoncategory_model_and_more.py
--rw-rw-rw-   0        0        0      751 2023-05-17 03:14:29.000000 django-common-objects-1.0.6/django_common_objects/migrations/0003_alter_commoncategory_unique_together_and_more.py
--rw-rw-rw-   0        0        0        0 2023-03-07 07:13:25.000000 django-common-objects-1.0.6/django_common_objects/migrations/__init__.py
--rw-rw-rw-   0        0        0     3612 2023-05-17 03:13:33.000000 django-common-objects-1.0.6/django_common_objects/models.py
--rw-rw-rw-   0        0        0      488 2023-02-16 05:39:51.000000 django-common-objects-1.0.6/django_common_objects/rest_view.py
--rw-rw-rw-   0        0        0      738 2023-02-16 09:09:26.000000 django-common-objects-1.0.6/django_common_objects/serializers.py
--rw-rw-rw-   0        0        0      439 2023-03-13 09:48:04.000000 django-common-objects-1.0.6/django_common_objects/settings.py
--rw-rw-rw-   0        0        0      804 2023-03-13 09:30:10.000000 django-common-objects-1.0.6/django_common_objects/site.py
--rw-rw-rw-   0        0        0       63 2023-02-28 03:21:57.000000 django-common-objects-1.0.6/django_common_objects/tests.py
-drwxrwxrwx   0        0        0        0 2023-05-17 03:16:49.917308 django-common-objects-1.0.6/django_common_objects/utils/
--rw-rw-rw-   0        0        0        0 2023-02-16 03:57:14.000000 django-common-objects-1.0.6/django_common_objects/utils/__init__.py
--rw-rw-rw-   0        0        0      166 2023-02-28 03:30:14.000000 django-common-objects-1.0.6/django_common_objects/utils/admin.py
--rw-rw-rw-   0        0        0      904 2023-02-17 06:35:48.000000 django-common-objects-1.0.6/django_common_objects/utils/algorithm.py
--rw-rw-rw-   0        0        0      522 2023-02-28 03:46:13.000000 django-common-objects-1.0.6/django_common_objects/utils/foreign_key.py
--rw-rw-rw-   0        0        0      880 2023-02-15 06:14:26.000000 django-common-objects-1.0.6/django_common_objects/validator.py
--rw-rw-rw-   0        0        0       66 2023-02-28 03:21:57.000000 django-common-objects-1.0.6/django_common_objects/views.py
--rw-rw-rw-   0        0        0     2183 2023-03-07 02:46:25.000000 django-common-objects-1.0.6/django_common_objects/widgets.py
-drwxrwxrwx   0        0        0        0 2023-05-17 03:16:49.888407 django-common-objects-1.0.6/django_common_objects.egg-info/
--rw-rw-rw-   0        0        0      296 2023-05-17 03:16:49.000000 django-common-objects-1.0.6/django_common_objects.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1176 2023-05-17 03:16:49.000000 django-common-objects-1.0.6/django_common_objects.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 03:16:49.000000 django-common-objects-1.0.6/django_common_objects.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-05-17 03:16:49.000000 django-common-objects-1.0.6/django_common_objects.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-05-17 03:16:49.000000 django-common-objects-1.0.6/django_common_objects.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 03:16:49.919515 django-common-objects-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      456 2023-05-17 03:16:16.000000 django-common-objects-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-17 03:16:49.918506 django-common-objects-1.0.6/tests/
--rw-rw-rw-   0        0        0        0 2023-04-04 01:09:57.000000 django-common-objects-1.0.6/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 08:58:55.566970 django-common-objects-1.0.7/
+-rw-rw-rw-   0        0        0     1085 2023-02-28 03:17:44.000000 django-common-objects-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0      296 2023-05-23 08:58:55.565969 django-common-objects-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       21 2023-02-28 03:17:44.000000 django-common-objects-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 08:58:55.501475 django-common-objects-1.0.7/django_common_objects/
+-rw-rw-rw-   0        0        0        0 2023-02-28 03:21:57.000000 django-common-objects-1.0.7/django_common_objects/__init__.py
+-rw-rw-rw-   0        0        0     5521 2023-02-28 03:24:51.000000 django-common-objects-1.0.7/django_common_objects/admin.py
+-rw-rw-rw-   0        0        0      155 2023-02-28 03:45:02.000000 django-common-objects-1.0.7/django_common_objects/apps.py
+-rw-rw-rw-   0        0        0     2580 2023-02-28 03:45:52.000000 django-common-objects-1.0.7/django_common_objects/choices.py
+-rw-rw-rw-   0        0        0      801 2023-05-23 08:58:12.000000 django-common-objects-1.0.7/django_common_objects/fields.py
+-rw-rw-rw-   0        0        0     2033 2023-05-17 02:59:55.000000 django-common-objects-1.0.7/django_common_objects/forms.py
+drwxrwxrwx   0        0        0        0 2023-05-23 08:58:55.543263 django-common-objects-1.0.7/django_common_objects/migrations/
+-rw-rw-rw-   0        0        0     4132 2023-05-17 03:14:17.000000 django-common-objects-1.0.7/django_common_objects/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      832 2023-04-04 01:15:03.000000 django-common-objects-1.0.7/django_common_objects/migrations/0002_alter_commoncategory_model_and_more.py
+-rw-rw-rw-   0        0        0      751 2023-05-17 03:14:29.000000 django-common-objects-1.0.7/django_common_objects/migrations/0003_alter_commoncategory_unique_together_and_more.py
+-rw-rw-rw-   0        0        0        0 2023-03-07 07:13:25.000000 django-common-objects-1.0.7/django_common_objects/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3612 2023-05-17 03:13:33.000000 django-common-objects-1.0.7/django_common_objects/models.py
+-rw-rw-rw-   0        0        0      488 2023-02-16 05:39:51.000000 django-common-objects-1.0.7/django_common_objects/rest_view.py
+-rw-rw-rw-   0        0        0      738 2023-02-16 09:09:26.000000 django-common-objects-1.0.7/django_common_objects/serializers.py
+-rw-rw-rw-   0        0        0      439 2023-03-13 09:48:04.000000 django-common-objects-1.0.7/django_common_objects/settings.py
+-rw-rw-rw-   0        0        0      804 2023-03-13 09:30:10.000000 django-common-objects-1.0.7/django_common_objects/site.py
+-rw-rw-rw-   0        0        0       63 2023-02-28 03:21:57.000000 django-common-objects-1.0.7/django_common_objects/tests.py
+drwxrwxrwx   0        0        0        0 2023-05-23 08:58:55.564969 django-common-objects-1.0.7/django_common_objects/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-16 03:57:14.000000 django-common-objects-1.0.7/django_common_objects/utils/__init__.py
+-rw-rw-rw-   0        0        0      166 2023-02-28 03:30:14.000000 django-common-objects-1.0.7/django_common_objects/utils/admin.py
+-rw-rw-rw-   0        0        0      904 2023-02-17 06:35:48.000000 django-common-objects-1.0.7/django_common_objects/utils/algorithm.py
+-rw-rw-rw-   0        0        0      522 2023-02-28 03:46:13.000000 django-common-objects-1.0.7/django_common_objects/utils/foreign_key.py
+-rw-rw-rw-   0        0        0      880 2023-02-15 06:14:26.000000 django-common-objects-1.0.7/django_common_objects/validator.py
+-rw-rw-rw-   0        0        0       66 2023-02-28 03:21:57.000000 django-common-objects-1.0.7/django_common_objects/views.py
+-rw-rw-rw-   0        0        0     2183 2023-03-07 02:46:25.000000 django-common-objects-1.0.7/django_common_objects/widgets.py
+drwxrwxrwx   0        0        0        0 2023-05-23 08:58:55.523080 django-common-objects-1.0.7/django_common_objects.egg-info/
+-rw-rw-rw-   0        0        0      296 2023-05-23 08:58:55.000000 django-common-objects-1.0.7/django_common_objects.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1176 2023-05-23 08:58:55.000000 django-common-objects-1.0.7/django_common_objects.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 08:58:55.000000 django-common-objects-1.0.7/django_common_objects.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-23 08:58:55.000000 django-common-objects-1.0.7/django_common_objects.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-05-23 08:58:55.000000 django-common-objects-1.0.7/django_common_objects.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 08:58:55.566970 django-common-objects-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      456 2023-05-23 08:58:02.000000 django-common-objects-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 08:58:55.565969 django-common-objects-1.0.7/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-04 01:09:57.000000 django-common-objects-1.0.7/tests/__init__.py
```

### Comparing `django-common-objects-1.0.6/LICENSE` & `django-common-objects-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django-common-objects-1.0.6/django_common_objects/admin.py` & `django-common-objects-1.0.7/django_common_objects/admin.py`

 * *Files identical despite different names*

### Comparing `django-common-objects-1.0.6/django_common_objects/choices.py` & `django-common-objects-1.0.7/django_common_objects/choices.py`

 * *Files identical despite different names*

### Comparing `django-common-objects-1.0.6/django_common_objects/forms.py` & `django-common-objects-1.0.7/django_common_objects/forms.py`

 * *Files identical despite different names*

### Comparing `django-common-objects-1.0.6/django_common_objects/migrations/0001_initial.py` & `django-common-objects-1.0.7/django_common_objects/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-common-objects-1.0.6/django_common_objects/migrations/0002_alter_commoncategory_model_and_more.py` & `django-common-objects-1.0.7/django_common_objects/migrations/0002_alter_commoncategory_model_and_more.py`

 * *Files identical despite different names*

### Comparing `django-common-objects-1.0.6/django_common_objects/migrations/0003_alter_commoncategory_unique_together_and_more.py` & `django-common-objects-1.0.7/django_common_objects/migrations/0003_alter_commoncategory_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `django-common-objects-1.0.6/django_common_objects/models.py` & `django-common-objects-1.0.7/django_common_objects/models.py`

 * *Files identical despite different names*

### Comparing `django-common-objects-1.0.6/django_common_objects/serializers.py` & `django-common-objects-1.0.7/django_common_objects/serializers.py`

 * *Files identical despite different names*

### Comparing `django-common-objects-1.0.6/django_common_objects/site.py` & `django-common-objects-1.0.7/django_common_objects/site.py`

 * *Files identical despite different names*

### Comparing `django-common-objects-1.0.6/django_common_objects/utils/algorithm.py` & `django-common-objects-1.0.7/django_common_objects/utils/algorithm.py`

 * *Files identical despite different names*

### Comparing `django-common-objects-1.0.6/django_common_objects/utils/foreign_key.py` & `django-common-objects-1.0.7/django_common_objects/utils/foreign_key.py`

 * *Files identical despite different names*

### Comparing `django-common-objects-1.0.6/django_common_objects/validator.py` & `django-common-objects-1.0.7/django_common_objects/validator.py`

 * *Files identical despite different names*

### Comparing `django-common-objects-1.0.6/django_common_objects/widgets.py` & `django-common-objects-1.0.7/django_common_objects/widgets.py`

 * *Files identical despite different names*

### Comparing `django-common-objects-1.0.6/django_common_objects.egg-info/SOURCES.txt` & `django-common-objects-1.0.7/django_common_objects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

