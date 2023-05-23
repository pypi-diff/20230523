# Comparing `tmp/django-content-blocks-1.3.0.tar.gz` & `tmp/django-content-blocks-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-content-blocks-1.3.0.tar", last modified: Tue May 23 18:32:22 2023, max compression
+gzip compressed data, was "django-content-blocks-1.3.1.tar", last modified: Tue May 23 19:01:06 2023, max compression
```

## Comparing `django-content-blocks-1.3.0.tar` & `django-content-blocks-1.3.1.tar`

### file list

```diff
@@ -1,110 +1,115 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.799921 django-content-blocks-1.3.0/
--rw-r--r--   0 root         (0) root         (0)     1076 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      147 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4662 2023-05-23 18:32:22.800523 django-content-blocks-1.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3166 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.419444 django-content-blocks-1.3.0/content_blocks/
--rw-r--r--   0 root         (0) root         (0)        0 2020-06-25 15:36:02.000000 django-content-blocks-1.3.0/content_blocks/__init__.py
--rw-r--r--   0 root         (0) root         (0)      850 2023-05-23 18:04:22.000000 django-content-blocks-1.3.0/content_blocks/abstract_models.py
--rw-r--r--   0 root         (0) root         (0)    11884 2023-05-23 18:04:22.000000 django-content-blocks-1.3.0/content_blocks/admin.py
--rw-r--r--   0 root         (0) root         (0)     5070 2023-05-23 18:04:22.000000 django-content-blocks-1.3.0/content_blocks/admin_forms.py
--rw-r--r--   0 root         (0) root         (0)     1110 2023-05-23 18:04:22.000000 django-content-blocks-1.3.0/content_blocks/apps.py
--rw-r--r--   0 root         (0) root         (0)     1704 2023-05-23 18:04:22.000000 django-content-blocks-1.3.0/content_blocks/conf.py
--rw-r--r--   0 root         (0) root         (0)     1685 2023-05-03 13:23:45.000000 django-content-blocks-1.3.0/content_blocks/fields.py
--rw-r--r--   0 root         (0) root         (0)     8031 2023-05-23 18:04:22.000000 django-content-blocks-1.3.0/content_blocks/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.431400 django-content-blocks-1.3.0/content_blocks/management/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-05 20:58:44.000000 django-content-blocks-1.3.0/content_blocks/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.456405 django-content-blocks-1.3.0/content_blocks/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-05 20:59:01.000000 django-content-blocks-1.3.0/content_blocks/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-05-23 18:04:22.000000 django-content-blocks-1.3.0/content_blocks/management/commands/clear_content_blocks_cache.py
--rw-r--r--   0 root         (0) root         (0)      542 2023-05-23 18:04:22.000000 django-content-blocks-1.3.0/content_blocks/management/commands/export_content_block_templates.py
--rw-r--r--   0 root         (0) root         (0)     1461 2023-05-23 18:04:22.000000 django-content-blocks-1.3.0/content_blocks/management/commands/import_content_block_templates.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-05-23 18:04:22.000000 django-content-blocks-1.3.0/content_blocks/management/commands/set_content_blocks_cache.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.477091 django-content-blocks-1.3.0/content_blocks/migrations/
--rw-r--r--   0 root         (0) root         (0)    12063 2023-03-17 11:59:08.000000 django-content-blocks-1.3.0/content_blocks/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)     1784 2023-04-14 09:38:36.000000 django-content-blocks-1.3.0/content_blocks/migrations/0002_alter_contentblock_css_class_and_more.py
--rw-r--r--   0 root         (0) root         (0)     1154 2023-05-01 12:02:10.000000 django-content-blocks-1.3.0/content_blocks/migrations/0003_alter_contentblocktemplatefield_unique_together_and_more.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-06-25 15:36:02.000000 django-content-blocks-1.3.0/content_blocks/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22721 2023-05-23 18:04:22.000000 django-content-blocks-1.3.0/content_blocks/models.py
--rw-r--r--   0 root         (0) root         (0)     5042 2023-05-23 18:04:22.000000 django-content-blocks-1.3.0/content_blocks/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.324019 django-content-blocks-1.3.0/content_blocks/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.480197 django-content-blocks-1.3.0/content_blocks/static/content_blocks/
--rw-r--r--   0 root         (0) root         (0)     6148 2023-02-28 23:45:54.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/.DS_Store
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.492948 django-content-blocks-1.3.0/content_blocks/static/content_blocks/css/
--rw-r--r--   0 root         (0) root         (0)     6148 2022-12-22 00:43:03.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/css/.DS_Store
--rw-r--r--   0 root         (0) root         (0)      709 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/css/content_block_template_admin.css
--rw-r--r--   0 root         (0) root         (0)    10043 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/css/content_blocks.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.331012 django-content-blocks-1.3.0/content_blocks/static/content_blocks/fontawesome/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.521895 django-content-blocks-1.3.0/content_blocks/static/content_blocks/fontawesome/css/
--rw-r--r--   0 root         (0) root         (0)    95481 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/fontawesome/css/fontawesome.min.css
--rw-r--r--   0 root         (0) root         (0)      110 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/fontawesome/css/light.min.css
--rw-r--r--   0 root         (0) root         (0)      747 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/fontawesome/css/procompatibility.css
--rw-r--r--   0 root         (0) root         (0)      573 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/fontawesome/css/solid.min.css
--rw-r--r--   0 root         (0) root         (0)      110 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/fontawesome/css/thin.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.544249 django-content-blocks-1.3.0/content_blocks/static/content_blocks/fontawesome/webfonts/
--rw-r--r--   0 root         (0) root         (0)   394832 2023-05-02 13:45:50.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.ttf
--rw-r--r--   0 root         (0) root         (0)   149908 2023-05-02 13:45:50.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.woff2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.559707 django-content-blocks-1.3.0/content_blocks/static/content_blocks/iframeresizer/
--rw-r--r--   0 root         (0) root         (0)    34811 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/iframeresizer/iframeResizer.contentWindow.js
--rw-r--r--   0 root         (0) root         (0)    37781 2023-05-02 13:45:50.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/iframeresizer/iframeResizer.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.573325 django-content-blocks-1.3.0/content_blocks/static/content_blocks/jqueryform/
--rw-r--r--   0 root         (0) root         (0)    17094 2023-05-02 13:45:50.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js
--rw-r--r--   0 root         (0) root         (0)    22565 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.583442 django-content-blocks-1.3.0/content_blocks/static/content_blocks/jqueryui/
--rw-r--r--   0 root         (0) root         (0)    30802 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.css
--rw-r--r--   0 root         (0) root         (0)   255080 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.614575 django-content-blocks-1.3.0/content_blocks/static/content_blocks/js/
--rw-r--r--   0 root         (0) root         (0)     1894 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/js/admin_choices_widget.js
--rw-r--r--   0 root         (0) root         (0)      980 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/js/ajax_setup.js
--rw-r--r--   0 root         (0) root         (0)    19428 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/js/content_block_editor.js
--rw-r--r--   0 root         (0) root         (0)     2015 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/js/content_block_template_admin.js
--rw-r--r--   0 root         (0) root         (0)     2201 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/js/popup.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.629718 django-content-blocks-1.3.0/content_blocks/templates/
--rw-r--r--   0 root         (0) root         (0)     6148 2023-03-16 15:09:32.000000 django-content-blocks-1.3.0/content_blocks/templates/.DS_Store
--rw-r--r--   0 root         (0) root         (0)      137 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.663828 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/
--rw-r--r--   0 root         (0) root         (0)     6148 2023-02-07 23:05:50.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/.DS_Store
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.672497 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/admin/
--rw-r--r--   0 root         (0) root         (0)      324 2023-05-05 14:20:51.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/admin/content_block_template_change_list.html
--rw-r--r--   0 root         (0) root         (0)     1366 2023-05-03 12:36:26.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/admin/content_block_template_import_form.html
--rw-r--r--   0 root         (0) root         (0)      305 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/content_block_collection.html
--rw-r--r--   0 root         (0) root         (0)      494 2023-05-23 18:04:22.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/content_block_preview.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.693904 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/editor/
--rw-r--r--   0 root         (0) root         (0)     1997 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/editor/base.html
--rw-r--r--   0 root         (0) root         (0)     2656 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/editor/content_block_form.html
--rw-r--r--   0 root         (0) root         (0)     4886 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/editor/content_block_form_wrapper.html
--rw-r--r--   0 root         (0) root         (0)      439 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/editor/content_block_forms.html
--rw-r--r--   0 root         (0) root         (0)     4886 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/editor/editor.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.710132 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/partials/
--rw-r--r--   0 root         (0) root         (0)      187 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/partials/delete_popup.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.717881 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/partials/fields/
--rw-r--r--   0 root         (0) root         (0)      149 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/partials/fields/checkbox.html
--rw-r--r--   0 root         (0) root         (0)      497 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/partials/fields/default.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.738093 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/partials/fields/previews/
--rw-r--r--   0 root         (0) root         (0)      144 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/partials/fields/previews/base.html
--rw-r--r--   0 root         (0) root         (0)      464 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/partials/fields/previews/embedded_video.html
--rw-r--r--   0 root         (0) root         (0)      286 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/partials/fields/previews/image.html
--rw-r--r--   0 root         (0) root         (0)      389 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/partials/fields/previews/video.html
--rw-r--r--   0 root         (0) root         (0)      442 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/partials/loader.html
--rw-r--r--   0 root         (0) root         (0)      499 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/partials/popup.html
--rw-r--r--   0 root         (0) root         (0)      221 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/partials/reset_popup.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.752789 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/widgets/
--rw-r--r--   0 root         (0) root         (0)      499 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/widgets/choices.html
--rw-r--r--   0 root         (0) root         (0)      574 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/widgets/clearable_file.html
--rw-r--r--   0 root         (0) root         (0)      207 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/widgets/filename_autocomplete.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.766814 django-content-blocks-1.3.0/content_blocks/templatetags/
--rw-r--r--   0 root         (0) root         (0)        0 2020-06-26 15:01:37.000000 django-content-blocks-1.3.0/content_blocks/templatetags/__init__.py
--rw-r--r--   0 root         (0) root         (0)      514 2023-03-03 23:30:41.000000 django-content-blocks-1.3.0/content_blocks/templatetags/content_block_admin.py
--rw-r--r--   0 root         (0) root         (0)     1555 2023-05-23 18:04:22.000000 django-content-blocks-1.3.0/content_blocks/templatetags/content_blocks.py
--rw-r--r--   0 root         (0) root         (0)      699 2023-05-02 18:54:11.000000 django-content-blocks-1.3.0/content_blocks/urls.py
--rw-r--r--   0 root         (0) root         (0)    12326 2023-05-23 18:04:22.000000 django-content-blocks-1.3.0/content_blocks/views.py
--rw-r--r--   0 root         (0) root         (0)     1834 2023-04-13 17:44:10.000000 django-content-blocks-1.3.0/content_blocks/widgets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.796844 django-content-blocks-1.3.0/django_content_blocks.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4662 2023-05-23 18:32:22.000000 django-content-blocks-1.3.0/django_content_blocks.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4478 2023-05-23 18:32:22.000000 django-content-blocks-1.3.0/django_content_blocks.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-23 18:32:22.000000 django-content-blocks-1.3.0/django_content_blocks.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-05-23 18:32:22.000000 django-content-blocks-1.3.0/django_content_blocks.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-23 18:32:22.000000 django-content-blocks-1.3.0/django_content_blocks.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       89 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1945 2023-05-23 18:32:22.806117 django-content-blocks-1.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-21 13:27:13.000000 django-content-blocks-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:01:06.037326 django-content-blocks-1.3.1/
+-rw-r--r--   0 root         (0) root         (0)     1076 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      147 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4662 2023-05-23 19:01:06.038047 django-content-blocks-1.3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3166 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:01:05.670289 django-content-blocks-1.3.1/content_blocks/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-06-25 15:36:02.000000 django-content-blocks-1.3.1/content_blocks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      850 2023-05-23 18:04:22.000000 django-content-blocks-1.3.1/content_blocks/abstract_models.py
+-rw-r--r--   0 root         (0) root         (0)    11884 2023-05-23 18:04:22.000000 django-content-blocks-1.3.1/content_blocks/admin.py
+-rw-r--r--   0 root         (0) root         (0)     5070 2023-05-23 18:04:22.000000 django-content-blocks-1.3.1/content_blocks/admin_forms.py
+-rw-r--r--   0 root         (0) root         (0)     1110 2023-05-23 18:04:22.000000 django-content-blocks-1.3.1/content_blocks/apps.py
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-05-23 18:04:22.000000 django-content-blocks-1.3.1/content_blocks/conf.py
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-05-03 13:23:45.000000 django-content-blocks-1.3.1/content_blocks/fields.py
+-rw-r--r--   0 root         (0) root         (0)     8031 2023-05-23 18:04:22.000000 django-content-blocks-1.3.1/content_blocks/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:01:05.674437 django-content-blocks-1.3.1/content_blocks/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-09-05 20:58:44.000000 django-content-blocks-1.3.1/content_blocks/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:01:05.692458 django-content-blocks-1.3.1/content_blocks/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-09-05 20:59:01.000000 django-content-blocks-1.3.1/content_blocks/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-05-23 18:04:22.000000 django-content-blocks-1.3.1/content_blocks/management/commands/clear_content_blocks_cache.py
+-rw-r--r--   0 root         (0) root         (0)      542 2023-05-23 18:04:22.000000 django-content-blocks-1.3.1/content_blocks/management/commands/export_content_block_templates.py
+-rw-r--r--   0 root         (0) root         (0)     1461 2023-05-23 18:04:22.000000 django-content-blocks-1.3.1/content_blocks/management/commands/import_content_block_templates.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-05-23 18:04:22.000000 django-content-blocks-1.3.1/content_blocks/management/commands/set_content_blocks_cache.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:01:05.706878 django-content-blocks-1.3.1/content_blocks/migrations/
+-rw-r--r--   0 root         (0) root         (0)    12063 2023-03-17 11:59:08.000000 django-content-blocks-1.3.1/content_blocks/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)     1784 2023-04-14 09:38:36.000000 django-content-blocks-1.3.1/content_blocks/migrations/0002_alter_contentblock_css_class_and_more.py
+-rw-r--r--   0 root         (0) root         (0)     1154 2023-05-01 12:02:10.000000 django-content-blocks-1.3.1/content_blocks/migrations/0003_alter_contentblocktemplatefield_unique_together_and_more.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-06-25 15:36:02.000000 django-content-blocks-1.3.1/content_blocks/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22721 2023-05-23 18:04:22.000000 django-content-blocks-1.3.1/content_blocks/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:01:05.719947 django-content-blocks-1.3.1/content_blocks/services/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 18:56:52.000000 django-content-blocks-1.3.1/content_blocks/services/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12032 2023-05-23 18:04:22.000000 django-content-blocks-1.3.1/content_blocks/services/content_block.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-05-23 18:04:22.000000 django-content-blocks-1.3.1/content_blocks/services/content_block_parent.py
+-rw-r--r--   0 root         (0) root         (0)     5188 2023-05-23 18:04:22.000000 django-content-blocks-1.3.1/content_blocks/services/content_block_template.py
+-rw-r--r--   0 root         (0) root         (0)     5042 2023-05-23 18:04:22.000000 django-content-blocks-1.3.1/content_blocks/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:01:05.574862 django-content-blocks-1.3.1/content_blocks/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:01:05.723199 django-content-blocks-1.3.1/content_blocks/static/content_blocks/
+-rw-r--r--   0 root         (0) root         (0)     6148 2023-02-28 23:45:54.000000 django-content-blocks-1.3.1/content_blocks/static/content_blocks/.DS_Store
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:01:05.735978 django-content-blocks-1.3.1/content_blocks/static/content_blocks/css/
+-rw-r--r--   0 root         (0) root         (0)     6148 2022-12-22 00:43:03.000000 django-content-blocks-1.3.1/content_blocks/static/content_blocks/css/.DS_Store
+-rw-r--r--   0 root         (0) root         (0)      709 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/content_blocks/static/content_blocks/css/content_block_template_admin.css
+-rw-r--r--   0 root         (0) root         (0)    10043 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/content_blocks/static/content_blocks/css/content_blocks.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:01:05.581421 django-content-blocks-1.3.1/content_blocks/static/content_blocks/fontawesome/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:01:05.756549 django-content-blocks-1.3.1/content_blocks/static/content_blocks/fontawesome/css/
+-rw-r--r--   0 root         (0) root         (0)    95481 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/content_blocks/static/content_blocks/fontawesome/css/fontawesome.min.css
+-rw-r--r--   0 root         (0) root         (0)      110 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/content_blocks/static/content_blocks/fontawesome/css/light.min.css
+-rw-r--r--   0 root         (0) root         (0)      747 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/content_blocks/static/content_blocks/fontawesome/css/procompatibility.css
+-rw-r--r--   0 root         (0) root         (0)      573 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/content_blocks/static/content_blocks/fontawesome/css/solid.min.css
+-rw-r--r--   0 root         (0) root         (0)      110 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/content_blocks/static/content_blocks/fontawesome/css/thin.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:01:05.772063 django-content-blocks-1.3.1/content_blocks/static/content_blocks/fontawesome/webfonts/
+-rw-r--r--   0 root         (0) root         (0)   394832 2023-05-02 13:45:50.000000 django-content-blocks-1.3.1/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 root         (0) root         (0)   149908 2023-05-02 13:45:50.000000 django-content-blocks-1.3.1/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.woff2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:01:05.785235 django-content-blocks-1.3.1/content_blocks/static/content_blocks/iframeresizer/
+-rw-r--r--   0 root         (0) root         (0)    34811 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/content_blocks/static/content_blocks/iframeresizer/iframeResizer.contentWindow.js
+-rw-r--r--   0 root         (0) root         (0)    37781 2023-05-02 13:45:50.000000 django-content-blocks-1.3.1/content_blocks/static/content_blocks/iframeresizer/iframeResizer.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:01:05.799233 django-content-blocks-1.3.1/content_blocks/static/content_blocks/jqueryform/
+-rw-r--r--   0 root         (0) root         (0)    17094 2023-05-02 13:45:50.000000 django-content-blocks-1.3.1/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js
+-rw-r--r--   0 root         (0) root         (0)    22565 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:01:05.811993 django-content-blocks-1.3.1/content_blocks/static/content_blocks/jqueryui/
+-rw-r--r--   0 root         (0) root         (0)    30802 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.css
+-rw-r--r--   0 root         (0) root         (0)   255080 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:01:05.862307 django-content-blocks-1.3.1/content_blocks/static/content_blocks/js/
+-rw-r--r--   0 root         (0) root         (0)     1894 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/content_blocks/static/content_blocks/js/admin_choices_widget.js
+-rw-r--r--   0 root         (0) root         (0)      980 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/content_blocks/static/content_blocks/js/ajax_setup.js
+-rw-r--r--   0 root         (0) root         (0)    19428 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/content_blocks/static/content_blocks/js/content_block_editor.js
+-rw-r--r--   0 root         (0) root         (0)     2015 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/content_blocks/static/content_blocks/js/content_block_template_admin.js
+-rw-r--r--   0 root         (0) root         (0)     2201 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/content_blocks/static/content_blocks/js/popup.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:01:05.872643 django-content-blocks-1.3.1/content_blocks/templates/
+-rw-r--r--   0 root         (0) root         (0)     6148 2023-03-16 15:09:32.000000 django-content-blocks-1.3.1/content_blocks/templates/.DS_Store
+-rw-r--r--   0 root         (0) root         (0)      137 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/content_blocks/templates/base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:01:05.885353 django-content-blocks-1.3.1/content_blocks/templates/content_blocks/
+-rw-r--r--   0 root         (0) root         (0)     6148 2023-02-07 23:05:50.000000 django-content-blocks-1.3.1/content_blocks/templates/content_blocks/.DS_Store
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:01:05.895801 django-content-blocks-1.3.1/content_blocks/templates/content_blocks/admin/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-05-05 14:20:51.000000 django-content-blocks-1.3.1/content_blocks/templates/content_blocks/admin/content_block_template_change_list.html
+-rw-r--r--   0 root         (0) root         (0)     1366 2023-05-03 12:36:26.000000 django-content-blocks-1.3.1/content_blocks/templates/content_blocks/admin/content_block_template_import_form.html
+-rw-r--r--   0 root         (0) root         (0)      305 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/content_blocks/templates/content_blocks/content_block_collection.html
+-rw-r--r--   0 root         (0) root         (0)      494 2023-05-23 18:04:22.000000 django-content-blocks-1.3.1/content_blocks/templates/content_blocks/content_block_preview.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:01:05.917035 django-content-blocks-1.3.1/content_blocks/templates/content_blocks/editor/
+-rw-r--r--   0 root         (0) root         (0)     1997 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/content_blocks/templates/content_blocks/editor/base.html
+-rw-r--r--   0 root         (0) root         (0)     2656 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/content_blocks/templates/content_blocks/editor/content_block_form.html
+-rw-r--r--   0 root         (0) root         (0)     4886 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/content_blocks/templates/content_blocks/editor/content_block_form_wrapper.html
+-rw-r--r--   0 root         (0) root         (0)      439 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/content_blocks/templates/content_blocks/editor/content_block_forms.html
+-rw-r--r--   0 root         (0) root         (0)     4886 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/content_blocks/templates/content_blocks/editor/editor.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:01:05.932679 django-content-blocks-1.3.1/content_blocks/templates/content_blocks/partials/
+-rw-r--r--   0 root         (0) root         (0)      187 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/content_blocks/templates/content_blocks/partials/delete_popup.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:01:05.939108 django-content-blocks-1.3.1/content_blocks/templates/content_blocks/partials/fields/
+-rw-r--r--   0 root         (0) root         (0)      149 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/content_blocks/templates/content_blocks/partials/fields/checkbox.html
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/content_blocks/templates/content_blocks/partials/fields/default.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:01:05.953430 django-content-blocks-1.3.1/content_blocks/templates/content_blocks/partials/fields/previews/
+-rw-r--r--   0 root         (0) root         (0)      144 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/content_blocks/templates/content_blocks/partials/fields/previews/base.html
+-rw-r--r--   0 root         (0) root         (0)      464 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/content_blocks/templates/content_blocks/partials/fields/previews/embedded_video.html
+-rw-r--r--   0 root         (0) root         (0)      286 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/content_blocks/templates/content_blocks/partials/fields/previews/image.html
+-rw-r--r--   0 root         (0) root         (0)      389 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/content_blocks/templates/content_blocks/partials/fields/previews/video.html
+-rw-r--r--   0 root         (0) root         (0)      442 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/content_blocks/templates/content_blocks/partials/loader.html
+-rw-r--r--   0 root         (0) root         (0)      499 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/content_blocks/templates/content_blocks/partials/popup.html
+-rw-r--r--   0 root         (0) root         (0)      221 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/content_blocks/templates/content_blocks/partials/reset_popup.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:01:05.964035 django-content-blocks-1.3.1/content_blocks/templates/content_blocks/widgets/
+-rw-r--r--   0 root         (0) root         (0)      499 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/content_blocks/templates/content_blocks/widgets/choices.html
+-rw-r--r--   0 root         (0) root         (0)      574 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/content_blocks/templates/content_blocks/widgets/clearable_file.html
+-rw-r--r--   0 root         (0) root         (0)      207 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/content_blocks/templates/content_blocks/widgets/filename_autocomplete.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:01:05.992917 django-content-blocks-1.3.1/content_blocks/templatetags/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-06-26 15:01:37.000000 django-content-blocks-1.3.1/content_blocks/templatetags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      514 2023-03-03 23:30:41.000000 django-content-blocks-1.3.1/content_blocks/templatetags/content_block_admin.py
+-rw-r--r--   0 root         (0) root         (0)     1555 2023-05-23 18:04:22.000000 django-content-blocks-1.3.1/content_blocks/templatetags/content_blocks.py
+-rw-r--r--   0 root         (0) root         (0)      699 2023-05-02 18:54:11.000000 django-content-blocks-1.3.1/content_blocks/urls.py
+-rw-r--r--   0 root         (0) root         (0)    12326 2023-05-23 18:04:22.000000 django-content-blocks-1.3.1/content_blocks/views.py
+-rw-r--r--   0 root         (0) root         (0)     1834 2023-04-13 17:44:10.000000 django-content-blocks-1.3.1/content_blocks/widgets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 19:01:06.034145 django-content-blocks-1.3.1/django_content_blocks.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4662 2023-05-23 19:01:05.000000 django-content-blocks-1.3.1/django_content_blocks.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4653 2023-05-23 19:01:05.000000 django-content-blocks-1.3.1/django_content_blocks.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-23 19:01:05.000000 django-content-blocks-1.3.1/django_content_blocks.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-05-23 19:01:05.000000 django-content-blocks-1.3.1/django_content_blocks.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-23 19:01:05.000000 django-content-blocks-1.3.1/django_content_blocks.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       89 2023-05-02 22:05:05.000000 django-content-blocks-1.3.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1945 2023-05-23 19:01:06.043438 django-content-blocks-1.3.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2022-12-21 13:27:13.000000 django-content-blocks-1.3.1/setup.py
```

### Comparing `django-content-blocks-1.3.0/LICENSE` & `django-content-blocks-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/PKG-INFO` & `django-content-blocks-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-content-blocks
-Version: 1.3.0
+Version: 1.3.1
 Summary: HTML content blocks for Django.
 Home-page: https://github.com/Quantra/django-content-blocks
 Author: Vince Coleman
 Author-email: vince@shystudios.co.uk
 License: MIT
 Project-URL: Documentation, https://django-content-blocks.readthedocs.io
 Project-URL: Source, https://github.com/Quantra/django-content-blocks
```

### Comparing `django-content-blocks-1.3.0/README.rst` & `django-content-blocks-1.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/abstract_models.py` & `django-content-blocks-1.3.1/content_blocks/abstract_models.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/admin.py` & `django-content-blocks-1.3.1/content_blocks/admin.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/admin_forms.py` & `django-content-blocks-1.3.1/content_blocks/admin_forms.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/apps.py` & `django-content-blocks-1.3.1/content_blocks/apps.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/conf.py` & `django-content-blocks-1.3.1/content_blocks/conf.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/fields.py` & `django-content-blocks-1.3.1/content_blocks/fields.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/forms.py` & `django-content-blocks-1.3.1/content_blocks/forms.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/management/commands/export_content_block_templates.py` & `django-content-blocks-1.3.1/content_blocks/management/commands/export_content_block_templates.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/management/commands/import_content_block_templates.py` & `django-content-blocks-1.3.1/content_blocks/management/commands/import_content_block_templates.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/migrations/0001_initial.py` & `django-content-blocks-1.3.1/content_blocks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/migrations/0002_alter_contentblock_css_class_and_more.py` & `django-content-blocks-1.3.1/content_blocks/migrations/0002_alter_contentblock_css_class_and_more.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/migrations/0003_alter_contentblocktemplatefield_unique_together_and_more.py` & `django-content-blocks-1.3.1/content_blocks/migrations/0003_alter_contentblocktemplatefield_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/models.py` & `django-content-blocks-1.3.1/content_blocks/models.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/signals.py` & `django-content-blocks-1.3.1/content_blocks/signals.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/static/content_blocks/.DS_Store` & `django-content-blocks-1.3.1/content_blocks/static/content_blocks/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/static/content_blocks/css/.DS_Store` & `django-content-blocks-1.3.1/content_blocks/static/content_blocks/css/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/static/content_blocks/css/content_block_template_admin.css` & `django-content-blocks-1.3.1/content_blocks/static/content_blocks/css/content_block_template_admin.css`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/static/content_blocks/css/content_blocks.css` & `django-content-blocks-1.3.1/content_blocks/static/content_blocks/css/content_blocks.css`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/static/content_blocks/fontawesome/css/fontawesome.min.css` & `django-content-blocks-1.3.1/content_blocks/static/content_blocks/fontawesome/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/static/content_blocks/fontawesome/css/procompatibility.css` & `django-content-blocks-1.3.1/content_blocks/static/content_blocks/fontawesome/css/procompatibility.css`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/static/content_blocks/fontawesome/css/solid.min.css` & `django-content-blocks-1.3.1/content_blocks/static/content_blocks/fontawesome/css/solid.min.css`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.ttf` & `django-content-blocks-1.3.1/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.woff2` & `django-content-blocks-1.3.1/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/static/content_blocks/iframeresizer/iframeResizer.contentWindow.js` & `django-content-blocks-1.3.1/content_blocks/static/content_blocks/iframeresizer/iframeResizer.contentWindow.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/static/content_blocks/iframeresizer/iframeResizer.js` & `django-content-blocks-1.3.1/content_blocks/static/content_blocks/iframeresizer/iframeResizer.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js` & `django-content-blocks-1.3.1/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js.map` & `django-content-blocks-1.3.1/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js.map`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.css` & `django-content-blocks-1.3.1/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.js` & `django-content-blocks-1.3.1/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/static/content_blocks/js/admin_choices_widget.js` & `django-content-blocks-1.3.1/content_blocks/static/content_blocks/js/admin_choices_widget.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/static/content_blocks/js/ajax_setup.js` & `django-content-blocks-1.3.1/content_blocks/static/content_blocks/js/ajax_setup.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/static/content_blocks/js/content_block_editor.js` & `django-content-blocks-1.3.1/content_blocks/static/content_blocks/js/content_block_editor.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/static/content_blocks/js/content_block_template_admin.js` & `django-content-blocks-1.3.1/content_blocks/static/content_blocks/js/content_block_template_admin.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/static/content_blocks/js/popup.js` & `django-content-blocks-1.3.1/content_blocks/static/content_blocks/js/popup.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/templates/.DS_Store` & `django-content-blocks-1.3.1/content_blocks/templates/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/templates/content_blocks/.DS_Store` & `django-content-blocks-1.3.1/content_blocks/templates/content_blocks/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/templates/content_blocks/admin/content_block_template_import_form.html` & `django-content-blocks-1.3.1/content_blocks/templates/content_blocks/admin/content_block_template_import_form.html`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/templates/content_blocks/editor/base.html` & `django-content-blocks-1.3.1/content_blocks/templates/content_blocks/editor/base.html`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/templates/content_blocks/editor/content_block_form.html` & `django-content-blocks-1.3.1/content_blocks/templates/content_blocks/editor/content_block_form.html`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/templates/content_blocks/editor/content_block_form_wrapper.html` & `django-content-blocks-1.3.1/content_blocks/templates/content_blocks/editor/content_block_form_wrapper.html`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/templates/content_blocks/editor/editor.html` & `django-content-blocks-1.3.1/content_blocks/templates/content_blocks/editor/editor.html`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/templates/content_blocks/widgets/clearable_file.html` & `django-content-blocks-1.3.1/content_blocks/templates/content_blocks/widgets/clearable_file.html`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/templatetags/content_block_admin.py` & `django-content-blocks-1.3.1/content_blocks/templatetags/content_block_admin.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/templatetags/content_blocks.py` & `django-content-blocks-1.3.1/content_blocks/templatetags/content_blocks.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/urls.py` & `django-content-blocks-1.3.1/content_blocks/urls.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/views.py` & `django-content-blocks-1.3.1/content_blocks/views.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/content_blocks/widgets.py` & `django-content-blocks-1.3.1/content_blocks/widgets.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.3.0/django_content_blocks.egg-info/PKG-INFO` & `django-content-blocks-1.3.1/django_content_blocks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-content-blocks
-Version: 1.3.0
+Version: 1.3.1
 Summary: HTML content blocks for Django.
 Home-page: https://github.com/Quantra/django-content-blocks
 Author: Vince Coleman
 Author-email: vince@shystudios.co.uk
 License: MIT
 Project-URL: Documentation, https://django-content-blocks.readthedocs.io
 Project-URL: Source, https://github.com/Quantra/django-content-blocks
```

### Comparing `django-content-blocks-1.3.0/django_content_blocks.egg-info/SOURCES.txt` & `django-content-blocks-1.3.1/django_content_blocks.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,18 @@
 content_blocks/management/commands/export_content_block_templates.py
 content_blocks/management/commands/import_content_block_templates.py
 content_blocks/management/commands/set_content_blocks_cache.py
 content_blocks/migrations/0001_initial.py
 content_blocks/migrations/0002_alter_contentblock_css_class_and_more.py
 content_blocks/migrations/0003_alter_contentblocktemplatefield_unique_together_and_more.py
 content_blocks/migrations/__init__.py
+content_blocks/services/__init__.py
+content_blocks/services/content_block.py
+content_blocks/services/content_block_parent.py
+content_blocks/services/content_block_template.py
 content_blocks/static/content_blocks/.DS_Store
 content_blocks/static/content_blocks/css/.DS_Store
 content_blocks/static/content_blocks/css/content_block_template_admin.css
 content_blocks/static/content_blocks/css/content_blocks.css
 content_blocks/static/content_blocks/fontawesome/css/fontawesome.min.css
 content_blocks/static/content_blocks/fontawesome/css/light.min.css
 content_blocks/static/content_blocks/fontawesome/css/procompatibility.css
```

### Comparing `django-content-blocks-1.3.0/setup.cfg` & `django-content-blocks-1.3.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-content-blocks
-version = 1.3.0
+version = 1.3.1
 description = HTML content blocks for Django.
 long_description = file:README.rst
 url = https://github.com/Quantra/django-content-blocks
 author = Vince Coleman
 author_email = vince@shystudios.co.uk
 license = MIT
 classifiers =
```

