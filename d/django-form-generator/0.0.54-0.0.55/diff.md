# Comparing `tmp/django_form_generator-0.0.54.tar.gz` & `tmp/django_form_generator-0.0.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_form_generator-0.0.54.tar", last modified: Wed Mar  1 06:57:18 2023, max compression
+gzip compressed data, was "django_form_generator-0.0.55.tar", last modified: Tue May 23 17:46:53 2023, max compression
```

## Comparing `django_form_generator-0.0.54.tar` & `django_form_generator-0.0.55.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 06:57:18.949197 django_form_generator-0.0.54/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-03-01 06:57:18.949197 django_form_generator-0.0.54/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 06:57:18.941197 django_form_generator-0.0.54/django_form_generator/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-01 06:57:18.000000 django_form_generator-0.0.54/django_form_generator/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 06:57:18.945197 django_form_generator-0.0.54/django_form_generator/api/
--rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 06:57:18.945197 django_form_generator-0.0.54/django_form_generator/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/common/admins.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/common/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/common/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/common/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 06:57:18.937197 django_form_generator-0.0.54/django_form_generator/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 06:57:18.945197 django_form_generator-0.0.54/django_form_generator/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    29856 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/docs/images/apiManagerCreateUser.png
--rw-r--r--   0 runner    (1001) docker     (123)    36492 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/docs/images/apiManagerGetUser.png
--rw-r--r--   0 runner    (1001) docker     (123)    29753 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/docs/images/ckEditor.png
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    12043 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 06:57:18.949197 django_form_generator-0.0.54/django_form_generator/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    16882 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/migrations/0002_field_read_only_field_write_only.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/migrations/0003_remove_field_error_message_remove_field_file_size_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/migrations/0004_fieldoptionthrough_remove_fieldvaluethrough_field_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/migrations/0005_alter_field_genre_alter_fieldvalidator_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/migrations/0006_alter_fieldvalidator_unique_together_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23488 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 06:57:18.949197 django_form_generator-0.0.54/django_form_generator/static/
--rw-r--r--   0 runner    (1001) docker     (123)    39434 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/static/htmx.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 06:57:18.937197 django_form_generator-0.0.54/django_form_generator/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 06:57:18.949197 django_form_generator-0.0.54/django_form_generator/templates/django_form_generator/
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/templates/django_form_generator/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 06:57:18.949197 django_form_generator-0.0.54/django_form_generator/templates/django_form_generator/fields/
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/templates/django_form_generator/fields/dynamic_fields.html
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/templates/django_form_generator/fields/inline_fields.html
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/templates/django_form_generator/fields/inorder_fields.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 06:57:18.949197 django_form_generator-0.0.54/django_form_generator/templates/django_form_generator/filters/
--rw-r--r--   0 runner    (1001) docker     (123)    13246 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/templates/django_form_generator/filters/form_response_filter.html
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/templates/django_form_generator/form.html
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/templates/django_form_generator/form_response.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 06:57:18.949197 django_form_generator-0.0.54/django_form_generator/templates/django_form_generator/tags/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/templates/django_form_generator/tags/form_tag.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 06:57:18.949197 django_form_generator-0.0.54/django_form_generator/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/templatetags/django_form_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/django_form_generator/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 06:57:18.945197 django_form_generator-0.0.54/django_form_generator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-03-01 06:57:18.000000 django_form_generator-0.0.54/django_form_generator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-03-01 06:57:18.000000 django_form_generator-0.0.54/django_form_generator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 06:57:18.000000 django_form_generator-0.0.54/django_form_generator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-03-01 06:57:18.000000 django_form_generator-0.0.54/django_form_generator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-01 06:57:18.000000 django_form_generator-0.0.54/django_form_generator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-03-01 06:57:18.949197 django_form_generator-0.0.54/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-03-01 06:57:03.000000 django_form_generator-0.0.54/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:46:53.525342 django_form_generator-0.0.55/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-05-23 17:46:53.525342 django_form_generator-0.0.55/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:46:53.513342 django_form_generator-0.0.55/django_form_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-23 17:46:53.000000 django_form_generator-0.0.55/django_form_generator/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:46:53.517342 django_form_generator-0.0.55/django_form_generator/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:46:53.517342 django_form_generator-0.0.55/django_form_generator/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/common/admins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/common/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/common/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/common/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:46:53.505342 django_form_generator-0.0.55/django_form_generator/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:46:53.521342 django_form_generator-0.0.55/django_form_generator/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    29856 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/docs/images/apiManagerCreateUser.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36492 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/docs/images/apiManagerGetUser.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29753 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/docs/images/ckEditor.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12043 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:46:53.521342 django_form_generator-0.0.55/django_form_generator/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    16882 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/migrations/0002_field_read_only_field_write_only.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/migrations/0003_remove_field_error_message_remove_field_file_size_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/migrations/0004_fieldoptionthrough_remove_fieldvaluethrough_field_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/migrations/0005_alter_field_genre_alter_fieldvalidator_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/migrations/0006_alter_fieldvalidator_unique_together_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23488 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:46:53.521342 django_form_generator-0.0.55/django_form_generator/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    39434 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/static/htmx.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:46:53.505342 django_form_generator-0.0.55/django_form_generator/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:46:53.525342 django_form_generator-0.0.55/django_form_generator/templates/django_form_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/templates/django_form_generator/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:46:53.525342 django_form_generator-0.0.55/django_form_generator/templates/django_form_generator/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/templates/django_form_generator/fields/dynamic_fields.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/templates/django_form_generator/fields/inline_fields.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/templates/django_form_generator/fields/inorder_fields.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:46:53.525342 django_form_generator-0.0.55/django_form_generator/templates/django_form_generator/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)    21573 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/templates/django_form_generator/filters/form_response_filter.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/templates/django_form_generator/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/templates/django_form_generator/form_response.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:46:53.525342 django_form_generator-0.0.55/django_form_generator/templates/django_form_generator/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/templates/django_form_generator/tags/form_tag.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:46:53.525342 django_form_generator-0.0.55/django_form_generator/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/templatetags/django_form_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/django_form_generator/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:46:53.517342 django_form_generator-0.0.55/django_form_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-05-23 17:46:53.000000 django_form_generator-0.0.55/django_form_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-23 17:46:53.000000 django_form_generator-0.0.55/django_form_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:46:53.000000 django_form_generator-0.0.55/django_form_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-23 17:46:53.000000 django_form_generator-0.0.55/django_form_generator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-23 17:46:53.000000 django_form_generator-0.0.55/django_form_generator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-23 17:46:53.529342 django_form_generator-0.0.55/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-23 17:46:41.000000 django_form_generator-0.0.55/setup.py
```

### Comparing `django_form_generator-0.0.54/LICENSE` & `django_form_generator-0.0.55/LICENSE`

 * *Files identical despite different names*

### Comparing `django_form_generator-0.0.54/PKG-INFO` & `django_form_generator-0.0.55/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_form_generator
-Version: 0.0.54
+Version: 0.0.55
 Summary: An app to create any form in django admin panel.
 Home-page: https://github.com/m3h-D/Form-Generator/tree/main
 Author: Mahdi Asadnejad
 Maintainer: Mahdi Asadnejad
 License: MIT
 Keywords: django form generator form_generator django_form_generator
 Classifier: Environment :: Web Environment
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django_form_generator Version: 0.0.54 Summary: An
+Metadata-Version: 2.1 Name: django_form_generator Version: 0.0.55 Summary: An
 app to create any form in django admin panel. Home-page: https://github.com/
 m3h-D/Form-Generator/tree/main Author: Mahdi Asadnejad Maintainer: Mahdi
 Asadnejad License: MIT Keywords: django form generator form_generator
 django_form_generator Classifier: Environment :: Web Environment Classifier:
 Framework :: Django :: 4.1 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3.10
```

### Comparing `django_form_generator-0.0.54/README.md` & `django_form_generator-0.0.55/README.md`

 * *Files identical despite different names*

### Comparing `django_form_generator-0.0.54/django_form_generator/admin.py` & `django_form_generator-0.0.55/django_form_generator/admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import uuid
-from django.db import models
 from django.http import JsonResponse
-from django.contrib import admin, messages
+from django.contrib import admin
 from django.utils.text import slugify
 from django.urls import reverse
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext as _
 from django.db.transaction import atomic
 
 from django_form_generator import const
@@ -26,36 +25,33 @@
 )
 
 
 class FormResponseFilter(FilterMixin, FormFilter):
 
     template = "django_form_generator/filters/form_response_filter.html"
     form_class = FormResponseFilterForm
+    title = _('Search on data')
+    parameter_name = 'data'
 
-    def get_parameters(self, request) -> tuple[str, list[str], list[str], list[str], list[str]]:
-        form_id: str = request.GET.get(f'{self.field.name}-form_id')
-        field_ids: list[str] = self.clean_parameters(request.GET.getlist(f'{self.field.name}-field'))
-        field_lookups: list[str] = self.clean_parameters(request.GET.getlist(f'{self.field.name}-field_lookup'))
-        operands: list[str] = self.clean_parameters(request.GET.getlist(f'{self.field.name}-operand'))
-        values: list[str] = self.clean_parameters(request.GET.getlist(f'{self.field.name}-value'))
-        return form_id ,field_ids ,field_lookups ,operands ,values
-
+    def get_parameters(self, request) -> list[str]:
+        params = []
+        for param in self.expected_parameters():
+            url_param = self.clean_parameters(request.GET.getlist(param))
+            if param == f'{self.field.name}-form_id':
+                params.append(self.request.GET.get(param))
+            else:
+                params.append(url_param)
+        return params
+    
     def queryset(self, request, queryset):
         response_filters, response_annotations = self.get_lookups(request)
         return queryset.alias(**response_annotations).filter(response_filters)
 
-    def form_lookups(self):
-        name = self.field.name
-        return (
-            ("%s-form_id" % name, "%s__exact" % name),
-            ("%s-field" % name, "%s__exact" % name),
-            ("%s-field_lookup" % name, "%s__exact" % name),
-            ("%s-operand" % name, "%s__exact" % name),
-            ("%s-value" % name, "%s__icontains" % name),
-        )
+    def expected_parameters(self):
+        return [f'{self.field.name}-form_id', f'{self.field.name}-field', f'{self.field.name}-field_lookup', f'{self.field.name}-operand', f'{self.field.name}-value']
 
 
 class FormFieldThroughInlineAdmin(admin.TabularInline):
     model = FormFieldThrough
     extra = 1
     raw_id_fields = ("field",)
     verbose_name = _('Field')
@@ -169,33 +165,42 @@
 class FormResponseAdmin(AdminMixin, admin.ModelAdmin):
     list_display = ["id", "get_form_title", "user_ip", "show_response"]
     list_display_links = ["id", "get_form_title"]
     list_filter = [('data', FormResponseFilter)]
     search_fields = ['form__title', 'form__slug', 'unique_id']
     search_help_text = 'Search on Form title & Form slug & unique_id'
     readonly_fields = ['id', 'unique_id', 'created_at', 'updated_at']
-    extra_views = [('fetch_options', 'options/<int:field_id>')]
+    extra_views = [
+        ('fetch_options', 'options/<int:field_id>'),
+        ('fetch_fields', 'fields/<int:form_id>')
+        ]
+
 
     @admin.display(description="Form Title")
     def get_form_title(self, obj):
         return obj.form.title
 
     @admin.display(description="Response")
     def show_response(self, obj):
         return mark_safe(
             f"<a href='{reverse('django_form_generator:form_response', args=(obj.unique_id, ))}'>Response</a>"
         )
     
-    def fetch_options(self, request, field_id):
+    def fetch_options(self, request, field_id: int):
         options = {}
         field = Field.objects.get(id=field_id)
         if field.genre in (const.FieldGenre.selectable_fields()):
             options = Option.objects.filter(fields__id=field_id).values('id', 'name')
         return JsonResponse(list(options), safe=False)
+    
+    def fetch_fields(self, request, form_id: int):
+        fields = Form.objects.get(id=form_id).get_fields().values('id', 'label')
+        return JsonResponse(list(fields), safe=False)
 
+        
 @admin.register(FormAPIManager)
 class FormAPIManagerAdmin(admin.ModelAdmin):
     list_display = ["id", "title", "method", "execute_time", "is_active", "cache_by", "created_at", "updated_at"]
     list_display_links = ["id", "title"]
     list_filter = ['is_active', 'created_at', 'execute_time', 'method']
     list_editable = ['is_active']
     search_fields = ['title', 'forms__title', 'forms__slug']
```

### Comparing `django_form_generator-0.0.54/django_form_generator/api/serializers.py` & `django_form_generator-0.0.55/django_form_generator/api/serializers.py`

 * *Files identical despite different names*

### Comparing `django_form_generator-0.0.54/django_form_generator/api/views.py` & `django_form_generator-0.0.55/django_form_generator/api/views.py`

 * *Files identical despite different names*

### Comparing `django_form_generator-0.0.54/django_form_generator/common/admins.py` & `django_form_generator-0.0.55/django_form_generator/common/admins.py`

 * *Files identical despite different names*

### Comparing `django_form_generator-0.0.54/django_form_generator/common/helpers.py` & `django_form_generator-0.0.55/django_form_generator/common/helpers.py`

 * *Files identical despite different names*

### Comparing `django_form_generator-0.0.54/django_form_generator/common/utils.py` & `django_form_generator-0.0.55/django_form_generator/common/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 import os
 import ast
 from pathlib import Path
 from typing import Any
 from django.conf import settings
 from django.template import Template, Context
 from django.utils.safestring import mark_safe
+from django.contrib import messages
 from django.utils.translation import gettext as _
 from django.core.validators import BaseValidator
 from django.utils.module_loading import import_string
 from django.db import models
 
-from django_form_generator.const import FormAPIManagerMethod, FieldLookupType
+from django_form_generator.const import FormAPIManagerMethod, FieldLookupType, FieldGenre
 from django_form_generator.settings import form_generator_settings as fg_settings
 
 
 FILE_UPLOAD_DIRECTORY = os.path.join(settings.MEDIA_ROOT, 'django_form_generator')
 
 try:
     Path(FILE_UPLOAD_DIRECTORY).mkdir(exist_ok=True)
@@ -103,102 +104,111 @@
 
     def compare(self, file_, limit_value):
         return file_.size > limit_value
 
 
 class FilterMixin:
 
-    field_path = 'data'
+    field_path: str = 'data'
     _filters: set = set()
     
     def clean_parameters(self, item):
         return list(filter(lambda x: x != '', item))
 
-    def _evaluate_value(self, value):
+    def _evaluate_value(self, value, genre):
         try:
             value = ast.literal_eval(value)
         except (ValueError, SyntaxError):
             value = str(value)
-        return value
+        if isinstance(value, (list, tuple)):
+            temp_val = []
+            for v in value:
+                temp_val.append(FieldGenre(genre).evaluate(v, regex=True))
+        else:
+            temp_val = FieldGenre(genre).evaluate(value, regex=True)
+        return temp_val
 
     def _evaluate_filter(self, field_id:int, index: int, value: Any, field_lookup: str) -> models.Q:
         if field_lookup.startswith('not'):
             field_lookup = field_lookup.lstrip('not_')
             negate = True
         else:
             negate = False
         lookup = '__' + FieldLookupType(field_lookup).value
-        inner_lookup = models.Q(**{f"{self.field_path}__{index}__value{lookup}": value}) \
-            & models.Q(**{f"{self.field_path}__{index}__id": field_id})
+        if field_lookup == 'range':
+            inner_lookup = models.Q(**{f"{self.field_path}__{index}__value__gte": value[0], 
+                                       f"{self.field_path}__{index}__value__lte": value[1]})
+        else:
+            inner_lookup = models.Q(**{f"{self.field_path}__{index}__value{lookup}": value})
+        inner_lookup &= models.Q(**{f"{self.field_path}__{index}__id": field_id})
         if negate:
             i_lookup = ~inner_lookup
             inner_lookup = i_lookup
         
         return inner_lookup
 
     def _evaluate_related_field(self, response: "FormResponse", form: "Form", field_id: int, field_ids: list[str], values:list[str], index:int, field_lookup: str):
         fields = form.get_fields(extra={"object_id": field_id, "content_type__model": 'field', "id__in": field_ids})
         for field in fields.iterator():
-            value =  self._evaluate_value(values[index])
+            value =  self._evaluate_value(values[index], field.genre)
             new_filters = self._evaluate_filter(field.pk, index, value, field_lookup)
             if str(new_filters) not in self._filters:
                 query = response.filter(new_filters)
                 self._filters.add(str(new_filters))
                 return models.Exists(query)
 
-    def get_parameters(self, request) -> tuple[str, list[str], list[str], list[str], list[str]]:
-        form_id: str = request.GET.get('form_id')
-        field_ids: list[str] = self.clean_parameters(request.GET.getlist('field_id'))
-        field_lookups: list[str] = self.clean_parameters(request.GET.getlist('field_lookup'))
-        operands: list[str] = self.clean_parameters(request.GET.getlist('operand'))
-        values: list[str] = self.clean_parameters(request.GET.getlist('value'))
-        return form_id ,field_ids ,field_lookups ,operands ,values
-
 
-    def get_lookups(self, request):
+    def get_lookups(self, request) -> tuple[models.Q, dict]:
         form_id ,field_ids ,field_lookups ,operands ,values = self.get_parameters(request)
         if form_id:
+            form_id = int(form_id)
             Form = import_string('django_form_generator.models.Form')
             FormResponse = import_string('django_form_generator.models.FormResponse')
 
-            form = Form.objects.prefetch_related('fields').get(id=int(form_id))
-            response = FormResponse.objects.filter(form_id=int(form_id))
+            form = Form.objects.prefetch_related('fields').get(id=form_id)
+            response = FormResponse.objects.filter(form_id=form_id)
             if response.exists():
                 self._filters: set = set()
                 response_annotations: dict = {}
                 response_filters: models.Q = models.Q()
-                for i in range(len(values)):
-                    field_id = int(field_ids[i])
-                    field_lookup = field_lookups[i]
-                    operand = operands[i]
+                for i, value in enumerate(values):
+                    try:
+                        field_id = int(field_ids[i])
+                        field_lookup = field_lookups[i]
+                        operand = operands[i]
+                    except IndexError:
+                        messages.add_message(request, messages.ERROR, _("Please make sure you filled all the fields [Operand, Field, Field lookup, Value] for Data filter."))
+                        return models.Q(), {}
                     form_fields_list = form.get_fields()
-                    value = self._evaluate_value(values[i])
                     current_field = form_fields_list.only('id', 'name').get(id=field_id)
+                    value = self._evaluate_value(value, current_field.genre)
                     related_index = next((field_ids.index(str(f.id)) 
                                         for f in current_field.depends.values_list('id', flat=True) 
                                         if str(f.id) in field_ids), None)
                     index = list(form_fields_list.values_list('id', flat=True)).index(field_id)
                     new_filters = self._evaluate_filter(field_id, index, value, field_lookup)
                     new_filters_ = models.Q()
                     if related_index:
                         # generate related field lookup & annotation and add it to current field lookup
-                        related_exists = self._evaluate_related_field(response, form, field_id, field_ids, values, related_index, filters, field_lookups[related_index])
+                        related_exists = self._evaluate_related_field(response, form, field_id, field_ids, values, related_index, field_lookups[related_index])
                         if related_exists:
-                            response_annotations.update({f'{field_id}_related_exists': related_exists})
-                            related_lookup = models.Q(**{f'{field_id}_related_exists': True})
+                            response_annotations.update({f'{field_id}_{i}_related_exists': related_exists})
+                            related_lookup = models.Q(**{f'{field_id}_{i}_related_exists': True})
 
                             new_filters.add(related_lookup, models.Q.AND)
                             new_filters_.add(related_lookup, models.Q.AND)
                     if str(new_filters) not in self._filters: # check if this filter is not duplicate
                         self._filters.add(str(new_filters))
                         exists = models.Exists(response.filter(new_filters, id=models.OuterRef('id')))
-                        response_annotations.update({f'{field_id}_exists':exists})
-                        new_filters_.add(models.Q(**{f'{field_id}_exists': True}), operand)
+                        response_annotations.update({f'{field_id}_{i}_exists':exists})
+                        new_filters_.add(models.Q(**{f'{field_id}_{i}_exists': True}), operand)
                         response_filters.add(new_filters_, operand)
 
-                response_filters.add(models.Q(form_id=int(form_id)), models.Q.AND)
+                response_filters.add(models.Q(form_id=form_id), models.Q.AND)
                 return response_filters, response_annotations
+        if len(values) > 0:
+            messages.add_message(request, messages.ERROR, _("Please make sure you have entered form id for Data filter."))
         return models.Q(), {}
 
-    def get_queryset(self, request, queryset):
+    def queryset(self, request, queryset):
         response_filters, response_annotations = self.get_lookups(request)
         return queryset.alias(**response_annotations).filter(response_filters)
```

### Comparing `django_form_generator-0.0.54/django_form_generator/common/views.py` & `django_form_generator-0.0.55/django_form_generator/common/views.py`

 * *Files identical despite different names*

### Comparing `django_form_generator-0.0.54/django_form_generator/const.py` & `django_form_generator-0.0.55/django_form_generator/const.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,14 +62,16 @@
 
     def eval_number(self, value, **kwargs):
         if value is None or value == '':
             return None
         return int(value)
 
     def eval_dropdown(self, value, **kwargs):
+        if kwargs.get('regex'):
+            return self.eval_text_input(value)
         return self.eval_number(value)
 
     def eval_date(self, value, **kwargs):
         return self.eval_text_input(value)
 
     def eval_time(self, value, **kwargs):
         return self.eval_text_input(value)
@@ -91,14 +93,16 @@
             return []
         if isinstance(value, list):
             return [int(val) for val in value]
         else:
             return []
 
     def eval_radio(self, value, **kwargs):
+        if kwargs.get('regex'):
+            return self.eval_text_input(value)
         return self.eval_number(value)
 
     def eval_hidden(self, value, **kwargs):
         return self.eval_text_input(value)
 
     def eval_captcha(self, value, **kwargs):
         return None
```

### Comparing `django_form_generator-0.0.54/django_form_generator/docs/images/apiManagerCreateUser.png` & `django_form_generator-0.0.55/django_form_generator/docs/images/apiManagerCreateUser.png`

 * *Files identical despite different names*

### Comparing `django_form_generator-0.0.54/django_form_generator/docs/images/apiManagerGetUser.png` & `django_form_generator-0.0.55/django_form_generator/docs/images/apiManagerGetUser.png`

 * *Files identical despite different names*

### Comparing `django_form_generator-0.0.54/django_form_generator/docs/images/ckEditor.png` & `django_form_generator-0.0.55/django_form_generator/docs/images/ckEditor.png`

 * *Files identical despite different names*

### Comparing `django_form_generator-0.0.54/django_form_generator/fields.py` & `django_form_generator-0.0.55/django_form_generator/fields.py`

 * *Files identical despite different names*

### Comparing `django_form_generator-0.0.54/django_form_generator/forms.py` & `django_form_generator-0.0.55/django_form_generator/forms.py`

 * *Files identical despite different names*

### Comparing `django_form_generator-0.0.54/django_form_generator/managers.py` & `django_form_generator-0.0.55/django_form_generator/managers.py`

 * *Files identical despite different names*

### Comparing `django_form_generator-0.0.54/django_form_generator/migrations/0001_initial.py` & `django_form_generator-0.0.55/django_form_generator/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_form_generator-0.0.54/django_form_generator/migrations/0002_field_read_only_field_write_only.py` & `django_form_generator-0.0.55/django_form_generator/migrations/0002_field_read_only_field_write_only.py`

 * *Files identical despite different names*

### Comparing `django_form_generator-0.0.54/django_form_generator/migrations/0003_remove_field_error_message_remove_field_file_size_and_more.py` & `django_form_generator-0.0.55/django_form_generator/migrations/0003_remove_field_error_message_remove_field_file_size_and_more.py`

 * *Files identical despite different names*

### Comparing `django_form_generator-0.0.54/django_form_generator/migrations/0004_fieldoptionthrough_remove_fieldvaluethrough_field_and_more.py` & `django_form_generator-0.0.55/django_form_generator/migrations/0004_fieldoptionthrough_remove_fieldvaluethrough_field_and_more.py`

 * *Files identical despite different names*

### Comparing `django_form_generator-0.0.54/django_form_generator/migrations/0005_alter_field_genre_alter_fieldvalidator_validator.py` & `django_form_generator-0.0.55/django_form_generator/migrations/0005_alter_field_genre_alter_fieldvalidator_validator.py`

 * *Files identical despite different names*

### Comparing `django_form_generator-0.0.54/django_form_generator/migrations/0006_alter_fieldvalidator_unique_together_and_more.py` & `django_form_generator-0.0.55/django_form_generator/migrations/0006_alter_fieldvalidator_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `django_form_generator-0.0.54/django_form_generator/models.py` & `django_form_generator-0.0.55/django_form_generator/models.py`

 * *Files identical despite different names*

### Comparing `django_form_generator-0.0.54/django_form_generator/settings.py` & `django_form_generator-0.0.55/django_form_generator/settings.py`

 * *Files identical despite different names*

### Comparing `django_form_generator-0.0.54/django_form_generator/static/htmx.min.js` & `django_form_generator-0.0.55/django_form_generator/static/htmx.min.js`

 * *Files identical despite different names*

### Comparing `django_form_generator-0.0.54/django_form_generator/templates/django_form_generator/base.html` & `django_form_generator-0.0.55/django_form_generator/templates/django_form_generator/base.html`

 * *Files identical despite different names*

### Comparing `django_form_generator-0.0.54/django_form_generator/templates/django_form_generator/fields/dynamic_fields.html` & `django_form_generator-0.0.55/django_form_generator/templates/django_form_generator/fields/dynamic_fields.html`

 * *Files identical despite different names*

### Comparing `django_form_generator-0.0.54/django_form_generator/templates/django_form_generator/fields/inline_fields.html` & `django_form_generator-0.0.55/django_form_generator/templates/django_form_generator/fields/inline_fields.html`

 * *Files identical despite different names*

### Comparing `django_form_generator-0.0.54/django_form_generator/templates/django_form_generator/fields/inorder_fields.html` & `django_form_generator-0.0.55/django_form_generator/templates/django_form_generator/fields/inorder_fields.html`

 * *Files identical despite different names*

### Comparing `django_form_generator-0.0.54/django_form_generator/templates/django_form_generator/form.html` & `django_form_generator-0.0.55/django_form_generator/templates/django_form_generator/form.html`

 * *Files identical despite different names*

### Comparing `django_form_generator-0.0.54/django_form_generator/templates/django_form_generator/form_response.html` & `django_form_generator-0.0.55/django_form_generator/templates/django_form_generator/form_response.html`

 * *Files identical despite different names*

### Comparing `django_form_generator-0.0.54/django_form_generator/templatetags/django_form_generator.py` & `django_form_generator-0.0.55/django_form_generator/templatetags/django_form_generator.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,8 +44,17 @@
 
 
 @register.filter(takes_context=True)
 def eval_data(context, body):
     tmp = template.Template(body)
     context = template.Context(context)
     data = tmp.render(context)
-    return data
+    return data
+
+
+@register.filter
+def clear_form(val):
+    val.data = {}
+    val.cleaned_data = {}
+    for field in val.visible_fields():
+        field.form.data = {}
+    return val.as_p()
```

### Comparing `django_form_generator-0.0.54/django_form_generator/tests.py` & `django_form_generator-0.0.55/django_form_generator/tests.py`

 * *Files identical despite different names*

### Comparing `django_form_generator-0.0.54/django_form_generator/views.py` & `django_form_generator-0.0.55/django_form_generator/views.py`

 * *Files identical despite different names*

### Comparing `django_form_generator-0.0.54/django_form_generator.egg-info/PKG-INFO` & `django_form_generator-0.0.55/django_form_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-form-generator
-Version: 0.0.54
+Version: 0.0.55
 Summary: An app to create any form in django admin panel.
 Home-page: https://github.com/m3h-D/Form-Generator/tree/main
 Author: Mahdi Asadnejad
 Maintainer: Mahdi Asadnejad
 License: MIT
 Keywords: django form generator form_generator django_form_generator
 Classifier: Environment :: Web Environment
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-form-generator Version: 0.0.54 Summary: An
+Metadata-Version: 2.1 Name: django-form-generator Version: 0.0.55 Summary: An
 app to create any form in django admin panel. Home-page: https://github.com/
 m3h-D/Form-Generator/tree/main Author: Mahdi Asadnejad Maintainer: Mahdi
 Asadnejad License: MIT Keywords: django form generator form_generator
 django_form_generator Classifier: Environment :: Web Environment Classifier:
 Framework :: Django :: 4.1 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3.10
```

### Comparing `django_form_generator-0.0.54/django_form_generator.egg-info/SOURCES.txt` & `django_form_generator-0.0.55/django_form_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_form_generator-0.0.54/setup.cfg` & `django_form_generator-0.0.55/setup.cfg`

 * *Files identical despite different names*

