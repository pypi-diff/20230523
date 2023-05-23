# Comparing `tmp/djangorestfilemanager-2.0.2.tar.gz` & `tmp/djangorestfilemanager-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangorestfilemanager-2.0.2.tar", last modified: Tue May 16 09:53:14 2023, max compression
+gzip compressed data, was "dist/djangorestfilemanager-2.0.3.tar", last modified: Tue May 23 12:58:22 2023, max compression
```

## Comparing `djangorestfilemanager-2.0.2.tar` & `djangorestfilemanager-2.0.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:53:14.000000 djangorestfilemanager-2.0.2/
--rw-rw-rw-   0 root         (0) root         (0)     1053 2023-05-16 09:53:03.000000 djangorestfilemanager-2.0.2/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)      262 2023-05-16 09:53:03.000000 djangorestfilemanager-2.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4601 2023-05-16 09:53:14.000000 djangorestfilemanager-2.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4261 2023-05-16 09:53:03.000000 djangorestfilemanager-2.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:53:14.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 09:53:03.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      598 2023-05-16 09:53:03.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      823 2023-05-16 09:53:03.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/app_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-05-16 09:53:03.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      306 2023-05-16 09:53:03.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:53:14.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:53:14.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/locale/en/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:53:14.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/locale/en/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      856 2023-05-16 09:53:03.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/locale/en/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)     1595 2023-05-16 09:53:03.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:53:14.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:53:14.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/locale/es/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      878 2023-05-16 09:53:03.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/locale/es/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)     1618 2023-05-16 09:53:03.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:53:14.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1537 2023-05-16 09:53:03.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      778 2023-05-16 09:53:03.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/migrations/0002_auto_20200302_0947.py
--rw-rw-rw-   0 root         (0) root         (0)      860 2023-05-16 09:53:03.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/migrations/0003_auto_20200311_1022.py
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-05-16 09:53:03.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/migrations/0004_auto_20200318_1806.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2023-05-16 09:53:03.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/migrations/0005_auto_20200319_1235.py
--rw-rw-rw-   0 root         (0) root         (0)      482 2023-05-16 09:53:03.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/migrations/0006_auto_20200429_1220.py
--rw-rw-rw-   0 root         (0) root         (0)      405 2023-05-16 09:53:03.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/migrations/0007_alter_file_name.py
--rw-rw-rw-   0 root         (0) root         (0)      474 2023-05-16 09:53:03.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/migrations/0008_alter_file_field.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2023-05-16 09:53:03.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/migrations/0009_auto_20210810_0945.py
--rw-rw-rw-   0 root         (0) root         (0)      368 2023-05-16 09:53:03.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/migrations/0010_auto_alter_data.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-05-16 09:53:03.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/migrations/0011_alter_file_file.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 09:53:03.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2839 2023-05-16 09:53:03.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/models.py
--rw-rw-rw-   0 root         (0) root         (0)      485 2023-05-16 09:53:03.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     1023 2023-05-16 09:53:03.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)      424 2023-05-16 09:53:03.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:53:14.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 09:53:03.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4561 2023-05-16 09:53:03.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/tests/test_download_files.py
--rw-rw-rw-   0 root         (0) root         (0)     1831 2023-05-16 09:53:03.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/tests/test_upload_files.py
--rw-rw-rw-   0 root         (0) root         (0)      280 2023-05-16 09:53:03.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     1663 2023-05-16 09:53:03.000000 djangorestfilemanager-2.0.2/djangorestfilemanager/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:53:14.000000 djangorestfilemanager-2.0.2/djangorestfilemanager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4601 2023-05-16 09:53:14.000000 djangorestfilemanager-2.0.2/djangorestfilemanager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1682 2023-05-16 09:53:14.000000 djangorestfilemanager-2.0.2/djangorestfilemanager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 09:53:14.000000 djangorestfilemanager-2.0.2/djangorestfilemanager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      151 2023-05-16 09:53:14.000000 djangorestfilemanager-2.0.2/djangorestfilemanager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 09:53:14.000000 djangorestfilemanager-2.0.2/djangorestfilemanager.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      602 2023-05-16 09:53:14.000000 djangorestfilemanager-2.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-16 09:53:03.000000 djangorestfilemanager-2.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:58:22.000000 djangorestfilemanager-2.0.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2023-05-23 12:58:13.000000 djangorestfilemanager-2.0.3/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)      262 2023-05-23 12:58:13.000000 djangorestfilemanager-2.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4601 2023-05-23 12:58:22.000000 djangorestfilemanager-2.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4261 2023-05-23 12:58:13.000000 djangorestfilemanager-2.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:58:22.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-23 12:58:13.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      598 2023-05-23 12:58:13.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      823 2023-05-23 12:58:13.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/app_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-05-23 12:58:13.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      306 2023-05-23 12:58:13.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:58:22.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:58:22.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/locale/en/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:58:22.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/locale/en/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      856 2023-05-23 12:58:13.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/locale/en/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2023-05-23 12:58:13.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:58:22.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:58:22.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      878 2023-05-23 12:58:13.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/locale/es/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     1618 2023-05-23 12:58:13.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:58:22.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1537 2023-05-23 12:58:13.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      778 2023-05-23 12:58:13.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/migrations/0002_auto_20200302_0947.py
+-rw-rw-rw-   0 root         (0) root         (0)      860 2023-05-23 12:58:13.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/migrations/0003_auto_20200311_1022.py
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-05-23 12:58:13.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/migrations/0004_auto_20200318_1806.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-05-23 12:58:13.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/migrations/0005_auto_20200319_1235.py
+-rw-rw-rw-   0 root         (0) root         (0)      482 2023-05-23 12:58:13.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/migrations/0006_auto_20200429_1220.py
+-rw-rw-rw-   0 root         (0) root         (0)      405 2023-05-23 12:58:13.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/migrations/0007_alter_file_name.py
+-rw-rw-rw-   0 root         (0) root         (0)      474 2023-05-23 12:58:13.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/migrations/0008_alter_file_field.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2023-05-23 12:58:13.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/migrations/0009_auto_20210810_0945.py
+-rw-rw-rw-   0 root         (0) root         (0)      368 2023-05-23 12:58:13.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/migrations/0010_auto_alter_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      521 2023-05-23 12:58:13.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/migrations/0011_alter_file_file.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-23 12:58:13.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2839 2023-05-23 12:58:13.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      485 2023-05-23 12:58:13.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2023-05-23 12:58:13.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)      424 2023-05-23 12:58:13.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:58:22.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-23 12:58:13.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4561 2023-05-23 12:58:13.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/tests/test_download_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     1831 2023-05-23 12:58:13.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/tests/test_upload_files.py
+-rw-rw-rw-   0 root         (0) root         (0)      280 2023-05-23 12:58:13.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     1663 2023-05-23 12:58:13.000000 djangorestfilemanager-2.0.3/djangorestfilemanager/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:58:22.000000 djangorestfilemanager-2.0.3/djangorestfilemanager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4601 2023-05-23 12:58:21.000000 djangorestfilemanager-2.0.3/djangorestfilemanager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1682 2023-05-23 12:58:22.000000 djangorestfilemanager-2.0.3/djangorestfilemanager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 12:58:22.000000 djangorestfilemanager-2.0.3/djangorestfilemanager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      151 2023-05-23 12:58:22.000000 djangorestfilemanager-2.0.3/djangorestfilemanager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-23 12:58:22.000000 djangorestfilemanager-2.0.3/djangorestfilemanager.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      602 2023-05-23 12:58:22.000000 djangorestfilemanager-2.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-23 12:58:13.000000 djangorestfilemanager-2.0.3/setup.py
```

### Comparing `djangorestfilemanager-2.0.2/LICENSE.txt` & `djangorestfilemanager-2.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djangorestfilemanager-2.0.2/PKG-INFO` & `djangorestfilemanager-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangorestfilemanager
-Version: 2.0.2
+Version: 2.0.3
 Summary: Django REST File Manager.
 Home-page: https://gitlab.com/kas-factory/packages/django-rest-file-manager
 Author: Avelino @ KF
 Author-email: avelino@kasfactory.net
 License: COPYRIGHT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `djangorestfilemanager-2.0.2/README.md` & `djangorestfilemanager-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `djangorestfilemanager-2.0.2/djangorestfilemanager/admin.py` & `djangorestfilemanager-2.0.3/djangorestfilemanager/admin.py`

 * *Files identical despite different names*

### Comparing `djangorestfilemanager-2.0.2/djangorestfilemanager/app_settings.py` & `djangorestfilemanager-2.0.3/djangorestfilemanager/app_settings.py`

 * *Files identical despite different names*

### Comparing `djangorestfilemanager-2.0.2/djangorestfilemanager/locale/en/LC_MESSAGES/django.mo` & `djangorestfilemanager-2.0.3/djangorestfilemanager/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangorestfilemanager-2.0.2/djangorestfilemanager/locale/en/LC_MESSAGES/django.po` & `djangorestfilemanager-2.0.3/djangorestfilemanager/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangorestfilemanager-2.0.2/djangorestfilemanager/locale/es/LC_MESSAGES/django.mo` & `djangorestfilemanager-2.0.3/djangorestfilemanager/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangorestfilemanager-2.0.2/djangorestfilemanager/locale/es/LC_MESSAGES/django.po` & `djangorestfilemanager-2.0.3/djangorestfilemanager/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangorestfilemanager-2.0.2/djangorestfilemanager/migrations/0001_initial.py` & `djangorestfilemanager-2.0.3/djangorestfilemanager/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangorestfilemanager-2.0.2/djangorestfilemanager/migrations/0002_auto_20200302_0947.py` & `djangorestfilemanager-2.0.3/djangorestfilemanager/migrations/0002_auto_20200302_0947.py`

 * *Files identical despite different names*

### Comparing `djangorestfilemanager-2.0.2/djangorestfilemanager/migrations/0003_auto_20200311_1022.py` & `djangorestfilemanager-2.0.3/djangorestfilemanager/migrations/0003_auto_20200311_1022.py`

 * *Files identical despite different names*

### Comparing `djangorestfilemanager-2.0.2/djangorestfilemanager/migrations/0004_auto_20200318_1806.py` & `djangorestfilemanager-2.0.3/djangorestfilemanager/migrations/0004_auto_20200318_1806.py`

 * *Files identical despite different names*

### Comparing `djangorestfilemanager-2.0.2/djangorestfilemanager/migrations/0009_auto_20210810_0945.py` & `djangorestfilemanager-2.0.3/djangorestfilemanager/migrations/0009_auto_20210810_0945.py`

 * *Files identical despite different names*

### Comparing `djangorestfilemanager-2.0.2/djangorestfilemanager/models.py` & `djangorestfilemanager-2.0.3/djangorestfilemanager/models.py`

 * *Files identical despite different names*

### Comparing `djangorestfilemanager-2.0.2/djangorestfilemanager/serializers.py` & `djangorestfilemanager-2.0.3/djangorestfilemanager/serializers.py`

 * *Files identical despite different names*

### Comparing `djangorestfilemanager-2.0.2/djangorestfilemanager/tests/test_download_files.py` & `djangorestfilemanager-2.0.3/djangorestfilemanager/tests/test_download_files.py`

 * *Files identical despite different names*

### Comparing `djangorestfilemanager-2.0.2/djangorestfilemanager/tests/test_upload_files.py` & `djangorestfilemanager-2.0.3/djangorestfilemanager/tests/test_upload_files.py`

 * *Files identical despite different names*

### Comparing `djangorestfilemanager-2.0.2/djangorestfilemanager/views.py` & `djangorestfilemanager-2.0.3/djangorestfilemanager/views.py`

 * *Files identical despite different names*

### Comparing `djangorestfilemanager-2.0.2/djangorestfilemanager.egg-info/PKG-INFO` & `djangorestfilemanager-2.0.3/djangorestfilemanager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangorestfilemanager
-Version: 2.0.2
+Version: 2.0.3
 Summary: Django REST File Manager.
 Home-page: https://gitlab.com/kas-factory/packages/django-rest-file-manager
 Author: Avelino @ KF
 Author-email: avelino@kasfactory.net
 License: COPYRIGHT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `djangorestfilemanager-2.0.2/djangorestfilemanager.egg-info/SOURCES.txt` & `djangorestfilemanager-2.0.3/djangorestfilemanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangorestfilemanager-2.0.2/setup.cfg` & `djangorestfilemanager-2.0.3/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = djangorestfilemanager
-version = 2.0.2
+version = 2.0.3
 description = Django REST File Manager.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/kas-factory/packages/django-rest-file-manager
 author = Avelino @ KF
 author_email = avelino@kasfactory.net
 license = COPYRIGHT
```

