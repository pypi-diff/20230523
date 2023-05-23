# Comparing `tmp/django-content-blocks-1.2.1.tar.gz` & `tmp/django-content-blocks-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-content-blocks-1.2.1.tar", last modified: Fri Apr 14 14:54:37 2023, max compression
+gzip compressed data, was "django-content-blocks-1.3.0.tar", last modified: Tue May 23 18:32:22 2023, max compression
```

## Comparing `django-content-blocks-1.2.1.tar` & `django-content-blocks-1.3.0.tar`

### file list

```diff
@@ -1,108 +1,110 @@
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 14:54:37.304686 django-content-blocks-1.2.1/
--rw-r--r--   0 quantra    (501) staff       (20)     1075 2023-03-16 15:50:21.000000 django-content-blocks-1.2.1/LICENSE
--rw-r--r--   0 quantra    (501) staff       (20)      146 2023-03-07 15:39:03.000000 django-content-blocks-1.2.1/MANIFEST.in
--rw-r--r--   0 quantra    (501) staff       (20)     3497 2023-04-14 14:54:37.304811 django-content-blocks-1.2.1/PKG-INFO
--rw-r--r--   0 quantra    (501) staff       (20)     2001 2023-03-20 13:07:58.000000 django-content-blocks-1.2.1/README.rst
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 14:54:37.167091 django-content-blocks-1.2.1/content_blocks/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2020-06-25 15:36:02.000000 django-content-blocks-1.2.1/content_blocks/__init__.py
--rw-r--r--   0 quantra    (501) staff       (20)     3047 2023-03-01 13:20:40.000000 django-content-blocks-1.2.1/content_blocks/abstract_models.py
--rw-r--r--   0 quantra    (501) staff       (20)    10457 2023-03-07 16:00:12.000000 django-content-blocks-1.2.1/content_blocks/admin.py
--rw-r--r--   0 quantra    (501) staff       (20)     4008 2023-04-13 17:44:10.000000 django-content-blocks-1.2.1/content_blocks/admin_forms.py
--rw-r--r--   0 quantra    (501) staff       (20)     1601 2023-02-23 15:19:48.000000 django-content-blocks-1.2.1/content_blocks/apps.py
--rw-r--r--   0 quantra    (501) staff       (20)      158 2023-01-05 16:14:15.000000 django-content-blocks-1.2.1/content_blocks/cache.py
--rw-r--r--   0 quantra    (501) staff       (20)     1654 2023-03-10 11:51:54.000000 django-content-blocks-1.2.1/content_blocks/conf.py
--rw-r--r--   0 quantra    (501) staff       (20)     1686 2023-04-13 17:44:10.000000 django-content-blocks-1.2.1/content_blocks/fields.py
--rw-r--r--   0 quantra    (501) staff       (20)     7501 2023-04-04 14:24:55.000000 django-content-blocks-1.2.1/content_blocks/forms.py
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 14:54:37.168052 django-content-blocks-1.2.1/content_blocks/management/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2022-09-05 20:58:44.000000 django-content-blocks-1.2.1/content_blocks/management/__init__.py
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 14:54:37.182522 django-content-blocks-1.2.1/content_blocks/management/commands/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2022-09-05 20:59:01.000000 django-content-blocks-1.2.1/content_blocks/management/commands/__init__.py
--rw-r--r--   0 quantra    (501) staff       (20)      459 2023-02-27 23:55:14.000000 django-content-blocks-1.2.1/content_blocks/management/commands/clear_content_blocks_cache.py
--rw-r--r--   0 quantra    (501) staff       (20)      461 2023-02-27 23:57:07.000000 django-content-blocks-1.2.1/content_blocks/management/commands/update_content_blocks_cache.py
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 14:54:37.184259 django-content-blocks-1.2.1/content_blocks/migrations/
--rw-r--r--   0 quantra    (501) staff       (20)    12063 2023-03-17 11:59:08.000000 django-content-blocks-1.2.1/content_blocks/migrations/0001_initial.py
--rw-r--r--   0 quantra    (501) staff       (20)     1784 2023-04-14 09:38:36.000000 django-content-blocks-1.2.1/content_blocks/migrations/0002_alter_contentblock_css_class_and_more.py
--rw-r--r--   0 quantra    (501) staff       (20)        0 2020-06-25 15:36:02.000000 django-content-blocks-1.2.1/content_blocks/migrations/__init__.py
--rw-r--r--   0 quantra    (501) staff       (20)    22463 2023-04-14 14:51:58.000000 django-content-blocks-1.2.1/content_blocks/models.py
--rw-r--r--   0 quantra    (501) staff       (20)      410 2023-02-28 12:22:17.000000 django-content-blocks-1.2.1/content_blocks/permissions.py
--rw-r--r--   0 quantra    (501) staff       (20)     4874 2023-02-28 19:46:26.000000 django-content-blocks-1.2.1/content_blocks/signals.py
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 14:54:37.103192 django-content-blocks-1.2.1/content_blocks/static/
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 14:54:37.186581 django-content-blocks-1.2.1/content_blocks/static/content_blocks/
--rw-r--r--   0 quantra    (501) staff       (20)     6148 2023-02-28 23:45:54.000000 django-content-blocks-1.2.1/content_blocks/static/content_blocks/.DS_Store
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 14:54:37.192114 django-content-blocks-1.2.1/content_blocks/static/content_blocks/css/
--rw-r--r--   0 quantra    (501) staff       (20)     6148 2022-12-22 00:43:03.000000 django-content-blocks-1.2.1/content_blocks/static/content_blocks/css/.DS_Store
--rw-r--r--   0 quantra    (501) staff       (20)      722 2023-02-17 13:42:24.000000 django-content-blocks-1.2.1/content_blocks/static/content_blocks/css/content_block_template_admin.css
--rw-r--r--   0 quantra    (501) staff       (20)     9689 2023-04-14 14:53:10.000000 django-content-blocks-1.2.1/content_blocks/static/content_blocks/css/content_blocks.css
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 14:54:37.194166 django-content-blocks-1.2.1/content_blocks/static/content_blocks/fontawesome/
--rw-r--r--   0 quantra    (501) staff       (20)     6148 2023-02-27 19:46:37.000000 django-content-blocks-1.2.1/content_blocks/static/content_blocks/fontawesome/.DS_Store
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 14:54:37.206779 django-content-blocks-1.2.1/content_blocks/static/content_blocks/fontawesome/css/
--rw-r--r--   0 quantra    (501) staff       (20)     6148 2023-02-27 18:56:30.000000 django-content-blocks-1.2.1/content_blocks/static/content_blocks/fontawesome/css/.DS_Store
--rw-r--r--   0 quantra    (501) staff       (20)    80823 2023-01-30 19:05:04.000000 django-content-blocks-1.2.1/content_blocks/static/content_blocks/fontawesome/css/fontawesome.min.css
--rw-r--r--   0 quantra    (501) staff       (20)      109 2023-02-27 19:28:56.000000 django-content-blocks-1.2.1/content_blocks/static/content_blocks/fontawesome/css/light.min.css
--rw-r--r--   0 quantra    (501) staff       (20)      753 2023-03-04 01:20:32.000000 django-content-blocks-1.2.1/content_blocks/static/content_blocks/fontawesome/css/procompatibility.css
--rw-r--r--   0 quantra    (501) staff       (20)      572 2023-01-30 19:05:04.000000 django-content-blocks-1.2.1/content_blocks/static/content_blocks/fontawesome/css/solid.min.css
--rw-r--r--   0 quantra    (501) staff       (20)      109 2023-02-27 19:28:56.000000 django-content-blocks-1.2.1/content_blocks/static/content_blocks/fontawesome/css/thin.min.css
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 14:54:37.216784 django-content-blocks-1.2.1/content_blocks/static/content_blocks/fontawesome/webfonts/
--rw-r--r--   0 quantra    (501) staff       (20)   394832 2023-01-30 19:05:04.000000 django-content-blocks-1.2.1/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.ttf
--rw-r--r--   0 quantra    (501) staff       (20)   149908 2023-01-30 19:05:04.000000 django-content-blocks-1.2.1/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.woff2
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 14:54:37.223600 django-content-blocks-1.2.1/content_blocks/static/content_blocks/iframeresizer/
--rw-rw-r--   0 quantra    (501) staff       (20)    34813 2021-04-26 11:15:23.000000 django-content-blocks-1.2.1/content_blocks/static/content_blocks/iframeresizer/iframeResizer.contentWindow.js
--rw-rw-r--   0 quantra    (501) staff       (20)    37781 2021-04-26 11:15:23.000000 django-content-blocks-1.2.1/content_blocks/static/content_blocks/iframeresizer/iframeResizer.js
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 14:54:37.224813 django-content-blocks-1.2.1/content_blocks/static/content_blocks/jqueryform/
--rw-r--r--   0 quantra    (501) staff       (20)    17094 2022-09-08 20:48:29.000000 django-content-blocks-1.2.1/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js
--rw-r--r--   0 quantra    (501) staff       (20)    22564 2022-09-08 20:48:29.000000 django-content-blocks-1.2.1/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js.map
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 14:54:37.226028 django-content-blocks-1.2.1/content_blocks/static/content_blocks/jqueryui/
--rw-r--r--   0 quantra    (501) staff       (20)    30801 2022-09-08 20:48:29.000000 django-content-blocks-1.2.1/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.css
--rw-r--r--   0 quantra    (501) staff       (20)   255079 2022-09-08 20:48:29.000000 django-content-blocks-1.2.1/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.js
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 14:54:37.239234 django-content-blocks-1.2.1/content_blocks/static/content_blocks/js/
--rw-r--r--   0 quantra    (501) staff       (20)     1892 2023-03-07 15:33:44.000000 django-content-blocks-1.2.1/content_blocks/static/content_blocks/js/admin_choices_widget.js
--rw-r--r--   0 quantra    (501) staff       (20)     1065 2023-02-06 13:17:16.000000 django-content-blocks-1.2.1/content_blocks/static/content_blocks/js/ajax_setup.js
--rw-r--r--   0 quantra    (501) staff       (20)    22492 2023-03-10 11:51:54.000000 django-content-blocks-1.2.1/content_blocks/static/content_blocks/js/content_block_editor.js
--rw-r--r--   0 quantra    (501) staff       (20)     2213 2023-03-07 15:42:59.000000 django-content-blocks-1.2.1/content_blocks/static/content_blocks/js/content_block_template_admin.js
--rw-r--r--   0 quantra    (501) staff       (20)     2303 2023-02-28 22:47:03.000000 django-content-blocks-1.2.1/content_blocks/static/content_blocks/js/popup.js
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 14:54:37.246310 django-content-blocks-1.2.1/content_blocks/templates/
--rw-r--r--   0 quantra    (501) staff       (20)     6148 2023-03-16 15:09:32.000000 django-content-blocks-1.2.1/content_blocks/templates/.DS_Store
--rw-r--r--   0 quantra    (501) staff       (20)      136 2023-01-03 19:48:12.000000 django-content-blocks-1.2.1/content_blocks/templates/base.html
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 14:54:37.254466 django-content-blocks-1.2.1/content_blocks/templates/content_blocks/
--rw-r--r--   0 quantra    (501) staff       (20)     6148 2023-02-07 23:05:50.000000 django-content-blocks-1.2.1/content_blocks/templates/content_blocks/.DS_Store
--rw-r--r--   0 quantra    (501) staff       (20)      307 2023-04-02 17:26:54.000000 django-content-blocks-1.2.1/content_blocks/templates/content_blocks/content_block_collection.html
--rw-r--r--   0 quantra    (501) staff       (20)      457 2023-03-03 16:05:10.000000 django-content-blocks-1.2.1/content_blocks/templates/content_blocks/content_block_preview.html
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 14:54:37.256511 django-content-blocks-1.2.1/content_blocks/templates/content_blocks/editor/
--rw-r--r--   0 quantra    (501) staff       (20)     2042 2023-02-28 22:49:36.000000 django-content-blocks-1.2.1/content_blocks/templates/content_blocks/editor/base.html
--rw-r--r--   0 quantra    (501) staff       (20)     3012 2023-03-10 11:51:54.000000 django-content-blocks-1.2.1/content_blocks/templates/content_blocks/editor/content_block_form.html
--rw-r--r--   0 quantra    (501) staff       (20)     5310 2023-04-14 14:52:35.000000 django-content-blocks-1.2.1/content_blocks/templates/content_blocks/editor/content_block_form_wrapper.html
--rw-r--r--   0 quantra    (501) staff       (20)      442 2023-02-25 02:17:35.000000 django-content-blocks-1.2.1/content_blocks/templates/content_blocks/editor/content_block_forms.html
--rw-r--r--   0 quantra    (501) staff       (20)     5461 2023-02-28 23:38:02.000000 django-content-blocks-1.2.1/content_blocks/templates/content_blocks/editor/editor.html
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 14:54:37.258382 django-content-blocks-1.2.1/content_blocks/templates/content_blocks/partials/
--rw-r--r--   0 quantra    (501) staff       (20)      190 2023-02-23 13:56:34.000000 django-content-blocks-1.2.1/content_blocks/templates/content_blocks/partials/delete_popup.html
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 14:54:37.263473 django-content-blocks-1.2.1/content_blocks/templates/content_blocks/partials/fields/
--rw-r--r--   0 quantra    (501) staff       (20)      150 2023-02-23 13:56:28.000000 django-content-blocks-1.2.1/content_blocks/templates/content_blocks/partials/fields/checkbox.html
--rw-r--r--   0 quantra    (501) staff       (20)      516 2023-02-27 19:02:42.000000 django-content-blocks-1.2.1/content_blocks/templates/content_blocks/partials/fields/default.html
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 14:54:37.277665 django-content-blocks-1.2.1/content_blocks/templates/content_blocks/partials/fields/previews/
--rw-r--r--   0 quantra    (501) staff       (20)      145 2023-02-23 13:56:16.000000 django-content-blocks-1.2.1/content_blocks/templates/content_blocks/partials/fields/previews/base.html
--rw-r--r--   0 quantra    (501) staff       (20)      477 2023-02-27 19:02:42.000000 django-content-blocks-1.2.1/content_blocks/templates/content_blocks/partials/fields/previews/embedded_video.html
--rw-r--r--   0 quantra    (501) staff       (20)      299 2023-02-27 19:02:42.000000 django-content-blocks-1.2.1/content_blocks/templates/content_blocks/partials/fields/previews/image.html
--rw-r--r--   0 quantra    (501) staff       (20)      412 2023-02-27 19:02:42.000000 django-content-blocks-1.2.1/content_blocks/templates/content_blocks/partials/fields/previews/video.html
--rw-r--r--   0 quantra    (501) staff       (20)      545 2023-02-27 19:02:42.000000 django-content-blocks-1.2.1/content_blocks/templates/content_blocks/partials/loader.html
--rw-r--r--   0 quantra    (501) staff       (20)      566 2023-02-27 19:02:42.000000 django-content-blocks-1.2.1/content_blocks/templates/content_blocks/partials/popup.html
--rw-r--r--   0 quantra    (501) staff       (20)      224 2023-02-23 13:56:43.000000 django-content-blocks-1.2.1/content_blocks/templates/content_blocks/partials/reset_popup.html
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 14:54:37.284805 django-content-blocks-1.2.1/content_blocks/templates/content_blocks/widgets/
--rw-r--r--   0 quantra    (501) staff       (20)      536 2023-02-23 13:54:11.000000 django-content-blocks-1.2.1/content_blocks/templates/content_blocks/widgets/choices.html
--rw-r--r--   0 quantra    (501) staff       (20)      605 2023-02-23 13:54:23.000000 django-content-blocks-1.2.1/content_blocks/templates/content_blocks/widgets/clearable_file.html
--rw-r--r--   0 quantra    (501) staff       (20)      214 2023-02-24 02:12:55.000000 django-content-blocks-1.2.1/content_blocks/templates/content_blocks/widgets/filename_autocomplete.html
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 14:54:37.286616 django-content-blocks-1.2.1/content_blocks/templatetags/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2020-06-26 15:01:37.000000 django-content-blocks-1.2.1/content_blocks/templatetags/__init__.py
--rw-r--r--   0 quantra    (501) staff       (20)      514 2023-03-03 23:30:41.000000 django-content-blocks-1.2.1/content_blocks/templatetags/content_block_admin.py
--rw-r--r--   0 quantra    (501) staff       (20)     1351 2023-04-14 12:49:12.000000 django-content-blocks-1.2.1/content_blocks/templatetags/content_blocks.py
--rw-r--r--   0 quantra    (501) staff       (20)      699 2023-01-05 14:16:33.000000 django-content-blocks-1.2.1/content_blocks/urls.py
--rw-r--r--   0 quantra    (501) staff       (20)     9667 2023-04-14 10:35:29.000000 django-content-blocks-1.2.1/content_blocks/views.py
--rw-r--r--   0 quantra    (501) staff       (20)     1834 2023-04-13 17:44:10.000000 django-content-blocks-1.2.1/content_blocks/widgets.py
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-04-14 14:54:37.304447 django-content-blocks-1.2.1/django_content_blocks.egg-info/
--rw-r--r--   0 quantra    (501) staff       (20)     3497 2023-04-14 14:54:37.000000 django-content-blocks-1.2.1/django_content_blocks.egg-info/PKG-INFO
--rw-r--r--   0 quantra    (501) staff       (20)     4256 2023-04-14 14:54:37.000000 django-content-blocks-1.2.1/django_content_blocks.egg-info/SOURCES.txt
--rw-r--r--   0 quantra    (501) staff       (20)       40 2023-04-14 14:54:37.000000 django-content-blocks-1.2.1/django_content_blocks.egg-info/dependency_links.txt
--rw-r--r--   0 quantra    (501) staff       (20)       55 2023-04-14 14:54:37.000000 django-content-blocks-1.2.1/django_content_blocks.egg-info/requires.txt
--rw-r--r--   0 quantra    (501) staff       (20)       23 2023-04-14 14:54:37.000000 django-content-blocks-1.2.1/django_content_blocks.egg-info/top_level.txt
--rw-r--r--   0 quantra    (501) staff       (20)       88 2023-03-02 00:40:47.000000 django-content-blocks-1.2.1/pyproject.toml
--rw-r--r--   0 quantra    (501) staff       (20)     1945 2023-04-14 14:54:37.307873 django-content-blocks-1.2.1/setup.cfg
--rw-r--r--   0 quantra    (501) staff       (20)       38 2022-12-21 13:27:13.000000 django-content-blocks-1.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.799921 django-content-blocks-1.3.0/
+-rw-r--r--   0 root         (0) root         (0)     1076 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      147 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4662 2023-05-23 18:32:22.800523 django-content-blocks-1.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3166 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.419444 django-content-blocks-1.3.0/content_blocks/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-06-25 15:36:02.000000 django-content-blocks-1.3.0/content_blocks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      850 2023-05-23 18:04:22.000000 django-content-blocks-1.3.0/content_blocks/abstract_models.py
+-rw-r--r--   0 root         (0) root         (0)    11884 2023-05-23 18:04:22.000000 django-content-blocks-1.3.0/content_blocks/admin.py
+-rw-r--r--   0 root         (0) root         (0)     5070 2023-05-23 18:04:22.000000 django-content-blocks-1.3.0/content_blocks/admin_forms.py
+-rw-r--r--   0 root         (0) root         (0)     1110 2023-05-23 18:04:22.000000 django-content-blocks-1.3.0/content_blocks/apps.py
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-05-23 18:04:22.000000 django-content-blocks-1.3.0/content_blocks/conf.py
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-05-03 13:23:45.000000 django-content-blocks-1.3.0/content_blocks/fields.py
+-rw-r--r--   0 root         (0) root         (0)     8031 2023-05-23 18:04:22.000000 django-content-blocks-1.3.0/content_blocks/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.431400 django-content-blocks-1.3.0/content_blocks/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-09-05 20:58:44.000000 django-content-blocks-1.3.0/content_blocks/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.456405 django-content-blocks-1.3.0/content_blocks/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-09-05 20:59:01.000000 django-content-blocks-1.3.0/content_blocks/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-05-23 18:04:22.000000 django-content-blocks-1.3.0/content_blocks/management/commands/clear_content_blocks_cache.py
+-rw-r--r--   0 root         (0) root         (0)      542 2023-05-23 18:04:22.000000 django-content-blocks-1.3.0/content_blocks/management/commands/export_content_block_templates.py
+-rw-r--r--   0 root         (0) root         (0)     1461 2023-05-23 18:04:22.000000 django-content-blocks-1.3.0/content_blocks/management/commands/import_content_block_templates.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-05-23 18:04:22.000000 django-content-blocks-1.3.0/content_blocks/management/commands/set_content_blocks_cache.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.477091 django-content-blocks-1.3.0/content_blocks/migrations/
+-rw-r--r--   0 root         (0) root         (0)    12063 2023-03-17 11:59:08.000000 django-content-blocks-1.3.0/content_blocks/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)     1784 2023-04-14 09:38:36.000000 django-content-blocks-1.3.0/content_blocks/migrations/0002_alter_contentblock_css_class_and_more.py
+-rw-r--r--   0 root         (0) root         (0)     1154 2023-05-01 12:02:10.000000 django-content-blocks-1.3.0/content_blocks/migrations/0003_alter_contentblocktemplatefield_unique_together_and_more.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-06-25 15:36:02.000000 django-content-blocks-1.3.0/content_blocks/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22721 2023-05-23 18:04:22.000000 django-content-blocks-1.3.0/content_blocks/models.py
+-rw-r--r--   0 root         (0) root         (0)     5042 2023-05-23 18:04:22.000000 django-content-blocks-1.3.0/content_blocks/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.324019 django-content-blocks-1.3.0/content_blocks/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.480197 django-content-blocks-1.3.0/content_blocks/static/content_blocks/
+-rw-r--r--   0 root         (0) root         (0)     6148 2023-02-28 23:45:54.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/.DS_Store
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.492948 django-content-blocks-1.3.0/content_blocks/static/content_blocks/css/
+-rw-r--r--   0 root         (0) root         (0)     6148 2022-12-22 00:43:03.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/css/.DS_Store
+-rw-r--r--   0 root         (0) root         (0)      709 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/css/content_block_template_admin.css
+-rw-r--r--   0 root         (0) root         (0)    10043 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/css/content_blocks.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.331012 django-content-blocks-1.3.0/content_blocks/static/content_blocks/fontawesome/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.521895 django-content-blocks-1.3.0/content_blocks/static/content_blocks/fontawesome/css/
+-rw-r--r--   0 root         (0) root         (0)    95481 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/fontawesome/css/fontawesome.min.css
+-rw-r--r--   0 root         (0) root         (0)      110 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/fontawesome/css/light.min.css
+-rw-r--r--   0 root         (0) root         (0)      747 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/fontawesome/css/procompatibility.css
+-rw-r--r--   0 root         (0) root         (0)      573 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/fontawesome/css/solid.min.css
+-rw-r--r--   0 root         (0) root         (0)      110 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/fontawesome/css/thin.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.544249 django-content-blocks-1.3.0/content_blocks/static/content_blocks/fontawesome/webfonts/
+-rw-r--r--   0 root         (0) root         (0)   394832 2023-05-02 13:45:50.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 root         (0) root         (0)   149908 2023-05-02 13:45:50.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.woff2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.559707 django-content-blocks-1.3.0/content_blocks/static/content_blocks/iframeresizer/
+-rw-r--r--   0 root         (0) root         (0)    34811 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/iframeresizer/iframeResizer.contentWindow.js
+-rw-r--r--   0 root         (0) root         (0)    37781 2023-05-02 13:45:50.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/iframeresizer/iframeResizer.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.573325 django-content-blocks-1.3.0/content_blocks/static/content_blocks/jqueryform/
+-rw-r--r--   0 root         (0) root         (0)    17094 2023-05-02 13:45:50.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js
+-rw-r--r--   0 root         (0) root         (0)    22565 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.583442 django-content-blocks-1.3.0/content_blocks/static/content_blocks/jqueryui/
+-rw-r--r--   0 root         (0) root         (0)    30802 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.css
+-rw-r--r--   0 root         (0) root         (0)   255080 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.614575 django-content-blocks-1.3.0/content_blocks/static/content_blocks/js/
+-rw-r--r--   0 root         (0) root         (0)     1894 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/js/admin_choices_widget.js
+-rw-r--r--   0 root         (0) root         (0)      980 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/js/ajax_setup.js
+-rw-r--r--   0 root         (0) root         (0)    19428 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/js/content_block_editor.js
+-rw-r--r--   0 root         (0) root         (0)     2015 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/js/content_block_template_admin.js
+-rw-r--r--   0 root         (0) root         (0)     2201 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/static/content_blocks/js/popup.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.629718 django-content-blocks-1.3.0/content_blocks/templates/
+-rw-r--r--   0 root         (0) root         (0)     6148 2023-03-16 15:09:32.000000 django-content-blocks-1.3.0/content_blocks/templates/.DS_Store
+-rw-r--r--   0 root         (0) root         (0)      137 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.663828 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/
+-rw-r--r--   0 root         (0) root         (0)     6148 2023-02-07 23:05:50.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/.DS_Store
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.672497 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/admin/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-05-05 14:20:51.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/admin/content_block_template_change_list.html
+-rw-r--r--   0 root         (0) root         (0)     1366 2023-05-03 12:36:26.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/admin/content_block_template_import_form.html
+-rw-r--r--   0 root         (0) root         (0)      305 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/content_block_collection.html
+-rw-r--r--   0 root         (0) root         (0)      494 2023-05-23 18:04:22.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/content_block_preview.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.693904 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/editor/
+-rw-r--r--   0 root         (0) root         (0)     1997 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/editor/base.html
+-rw-r--r--   0 root         (0) root         (0)     2656 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/editor/content_block_form.html
+-rw-r--r--   0 root         (0) root         (0)     4886 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/editor/content_block_form_wrapper.html
+-rw-r--r--   0 root         (0) root         (0)      439 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/editor/content_block_forms.html
+-rw-r--r--   0 root         (0) root         (0)     4886 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/editor/editor.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.710132 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/partials/
+-rw-r--r--   0 root         (0) root         (0)      187 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/partials/delete_popup.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.717881 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/partials/fields/
+-rw-r--r--   0 root         (0) root         (0)      149 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/partials/fields/checkbox.html
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/partials/fields/default.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.738093 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/partials/fields/previews/
+-rw-r--r--   0 root         (0) root         (0)      144 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/partials/fields/previews/base.html
+-rw-r--r--   0 root         (0) root         (0)      464 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/partials/fields/previews/embedded_video.html
+-rw-r--r--   0 root         (0) root         (0)      286 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/partials/fields/previews/image.html
+-rw-r--r--   0 root         (0) root         (0)      389 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/partials/fields/previews/video.html
+-rw-r--r--   0 root         (0) root         (0)      442 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/partials/loader.html
+-rw-r--r--   0 root         (0) root         (0)      499 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/partials/popup.html
+-rw-r--r--   0 root         (0) root         (0)      221 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/partials/reset_popup.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.752789 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/widgets/
+-rw-r--r--   0 root         (0) root         (0)      499 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/widgets/choices.html
+-rw-r--r--   0 root         (0) root         (0)      574 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/widgets/clearable_file.html
+-rw-r--r--   0 root         (0) root         (0)      207 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/content_blocks/templates/content_blocks/widgets/filename_autocomplete.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.766814 django-content-blocks-1.3.0/content_blocks/templatetags/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-06-26 15:01:37.000000 django-content-blocks-1.3.0/content_blocks/templatetags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      514 2023-03-03 23:30:41.000000 django-content-blocks-1.3.0/content_blocks/templatetags/content_block_admin.py
+-rw-r--r--   0 root         (0) root         (0)     1555 2023-05-23 18:04:22.000000 django-content-blocks-1.3.0/content_blocks/templatetags/content_blocks.py
+-rw-r--r--   0 root         (0) root         (0)      699 2023-05-02 18:54:11.000000 django-content-blocks-1.3.0/content_blocks/urls.py
+-rw-r--r--   0 root         (0) root         (0)    12326 2023-05-23 18:04:22.000000 django-content-blocks-1.3.0/content_blocks/views.py
+-rw-r--r--   0 root         (0) root         (0)     1834 2023-04-13 17:44:10.000000 django-content-blocks-1.3.0/content_blocks/widgets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 18:32:22.796844 django-content-blocks-1.3.0/django_content_blocks.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4662 2023-05-23 18:32:22.000000 django-content-blocks-1.3.0/django_content_blocks.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4478 2023-05-23 18:32:22.000000 django-content-blocks-1.3.0/django_content_blocks.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-23 18:32:22.000000 django-content-blocks-1.3.0/django_content_blocks.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-05-23 18:32:22.000000 django-content-blocks-1.3.0/django_content_blocks.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-23 18:32:22.000000 django-content-blocks-1.3.0/django_content_blocks.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       89 2023-05-02 22:05:05.000000 django-content-blocks-1.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1945 2023-05-23 18:32:22.806117 django-content-blocks-1.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2022-12-21 13:27:13.000000 django-content-blocks-1.3.0/setup.py
```

### Comparing `django-content-blocks-1.2.1/LICENSE` & `django-content-blocks-1.3.0/LICENSE`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `django-content-blocks-1.2.1/PKG-INFO` & `django-content-blocks-1.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-content-blocks
-Version: 1.2.1
+Version: 1.3.0
 Summary: HTML content blocks for Django.
 Home-page: https://github.com/Quantra/django-content-blocks
 Author: Vince Coleman
 Author-email: vince@shystudios.co.uk
 License: MIT
 Project-URL: Documentation, https://django-content-blocks.readthedocs.io
 Project-URL: Source, https://github.com/Quantra/django-content-blocks
@@ -28,15 +28,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 Requires-Python: >=3.7
 License-File: LICENSE
 
-.. todo shields.io badges
+|coverage|
+|package version|
+|python versions supported|
+|django versions supported|
+|code style black|
+|license|
 
 =====================
 Django Content Blocks
 =====================
 
 Django Content Blocks is a reusable Django app that allows users to create and manage custom content blocks for their website. Via the django admin site it provides an easy-to-use interface for creating content blocks that can be inserted into any page, as well as a powerful template system for customizing the appearance of those blocks.
 
@@ -70,7 +75,27 @@
 * Dmitry Sobolev for so graciously transferring the django-content-blocks name on pypi
 * Margo Yaguda for linguistic assistance in contacting Dmitry
 
 Contributing
 ------------
 
 Contributions, advice and guidance are welcome. Please make contact **before** writing any code!
+
+
+.. shields.io badges
+
+.. |package version| image:: https://img.shields.io/pypi/v/django-content-blocks
+   :target: https://pypi.python.org/pypi/django-content-blocks/
+
+.. |python versions supported| image:: https://img.shields.io/pypi/pyversions/django-content-blocks
+   :target: https://pypi.python.org/pypi/django-content-blocks/
+
+.. |django versions supported| image:: https://img.shields.io/pypi/frameworkversions/django/django-content-blocks
+   :target: https://pypi.python.org/pypi/django-content-blocks/
+
+.. |coverage| image:: https://img.shields.io/badge/dynamic/xml?color=success&label=coverage&query=round%28%2F%2Fcoverage%2F%40line-rate%20%2A%20100%29&suffix=%25&url=https%3A%2F%2Fraw.githubusercontent.com%2FQuantra%2Fdjango-content-blocks%2Fmaster%2Fcoverage.xml
+
+.. |code style black| image:: https://img.shields.io/badge/code%20style-black-black
+    :target: https://github.com/psf/black
+
+.. |license| image:: https://img.shields.io/github/license/Quantra/django-content-blocks
+    :target: https://github.com/Quantra/django-content-blocks/blob/master/LICENSE
```

### Comparing `django-content-blocks-1.2.1/content_blocks/admin.py` & `django-content-blocks-1.3.0/content_blocks/admin.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 Content blocks admin.py
 """
+from io import StringIO
+
 from adminsortable2.admin import SortableAdminMixin, SortableInlineAdminMixin
 from django.conf import settings
 from django.contrib import admin, messages
-from django.http import HttpResponseRedirect
+from django.http import HttpResponseRedirect, StreamingHttpResponse
 from django.template import TemplateDoesNotExist
 from django.template.loader import get_template
 from django.urls import path, reverse
 from django.utils.safestring import mark_safe
 
 from content_blocks.admin_forms import (
     ContentBlockTemplateAdminForm,
@@ -16,27 +18,28 @@
 )
 from content_blocks.models import (
     ContentBlockAvailability,
     ContentBlockCollection,
     ContentBlockTemplate,
     ContentBlockTemplateField,
 )
+from content_blocks.services.content_block_template import ImportExportServices
 from content_blocks.views import (
     content_block_create,
     content_block_editor,
     content_block_preview,
+    content_block_template_export,
+    content_block_template_import,
     discard_changes,
     import_content_blocks,
     nested_block_create,
     publish_content_blocks,
 )
 
-"""
-Admin constants and base classes
-"""
+#  Admin constants and base classes
 
 # Auto dates
 AUTO_DATE_FIELDS = ["create_date", "mod_date"]
 AUTO_DATE_FIELDSET = (
     "Dates",
     {"fields": (("create_date", "mod_date"),)},
 )
@@ -48,32 +51,36 @@
 
 class ContentBlockTemplateFieldInline(SortableInlineAdminMixin, admin.StackedInline):
     model = ContentBlockTemplateField
     fk_name = "content_block_template"
     form = ContentBlockTemplateFieldAdminForm
     min_num = 0
     extra = 0
-    filter_horizontal = ["nested_templates"]
+    autocomplete_fields = ["nested_templates"]
 
 
 @admin.register(ContentBlockTemplate)
 class ContentBlockTemplateAdmin(SortableAdminMixin, admin.ModelAdmin):
     form = ContentBlockTemplateAdminForm
 
+    change_list_template = (
+        "content_blocks/admin/content_block_template_change_list.html"
+    )
     list_display = [
         "name",
         "template_filename",
         "visible",
     ] + AUTO_DATE_FIELDS
     list_editable = ("visible",)
     list_filter = AUTO_DATE_FIELDS + ["visible"]
     search_fields = ("name", "template_filename")
 
     readonly_fields = AUTO_DATE_FIELDS
     inlines = [ContentBlockTemplateFieldInline]
+    actions = ["export_content_block_templates"]
 
     class Media:
         css = {"all": ["content_blocks/css/content_block_template_admin.css"]}
         js = (
             "content_blocks/js/content_block_template_admin.js",
             "content_blocks/js/admin_choices_widget.js",
         )
@@ -113,34 +120,66 @@
             msg = (
                 f"Couldn't load a template for the content block template "
                 f'"<a href="{url}">{obj}</a>". '
                 f'No template found at "{template_filename}".'
             )
             messages.warning(request, mark_safe(msg))
 
+    def get_urls(self):
+        urls = [
+            path(
+                "export/",
+                content_block_template_export,
+                name="content_blocks_contentblocktemplate_export",
+            ),
+            path(
+                "import/",
+                content_block_template_import,
+                {"model_admin": self},
+                name="content_blocks_contentblocktemplate_import",
+            ),
+        ]
+        return urls + super().get_urls()
+
+    @admin.action(description="Export selected content block templates")
+    def export_content_block_templates(self, request, queryset):
+        """
+        Export the selected ContentBlockTemplate objects as JSON suitable for import.
+        """
+        buffer = StringIO()
+        ImportExportServices.export_content_block_templates(queryset, buffer)
+        buffer.seek(0)
+
+        return StreamingHttpResponse(
+            buffer,
+            content_type="application/json",
+            headers={
+                "Content-Disposition": 'attachment; filename="content_block_templates.json"'
+            },
+        )
+
 
 if "dbtemplates" in settings.INSTALLED_APPS:
     from dbtemplates.models import Template
 
     admin.site.unregister(ContentBlockTemplate)
 
     @admin.register(ContentBlockTemplate)
     class ContentBlockTemplateDBTemplatesAdmin(ContentBlockTemplateAdmin):
         @property
         def content_block_template_fields(self):
             return super().content_block_template_fields + ["db_template_button"]
 
+        @admin.display(description="HTML Template")
         def db_template_button(self, obj):
             if not obj.template_filename:
                 return "-"
             button = '<input type="submit" value="Save and edit HTML template" name="_dbtemplate">'
             return mark_safe(button)
 
-        db_template_button.short_description = "HTML Template"
-
         def get_readonly_fields(self, request, obj=None):
             return [
                 *super().get_readonly_fields(request, obj=obj),
                 "db_template_button",
             ]
 
         def _response(self, response, request, obj):
@@ -183,29 +222,28 @@
 
 class ContentBlockModelAdmin(admin.ModelAdmin):
     """
     Base class to be added to the admin of any model which has a content_blocks m2m.  This will then add
     content_blocks_button which can then be added to the formset.
     """
 
+    @admin.display(description="Content blocks")
     def content_blocks_link(self, obj):
         """
         A link to the content block editor for this object.
         Intended to be used on admin changelist.
         :param obj: subclass of :py:class:`ContentBlockParentModel`.
         """
         app_label, model_name = self.model._meta.app_label, self.model._meta.model_name
         url = reverse(
             f"admin:{app_label}_{model_name}_content_block_editor", args=[obj.id]
         )
         link = f'<a href="{url}">Edit content blocks</a>'
         return mark_safe(link)
 
-    content_blocks_link.short_description = "Content blocks"
-
     def content_blocks_button(self, *args):
         """
         A button which will save the object then, if successful, will redirect to the content block editor for this
         object.
         Intended to be used on the admin changepage.
         """
         button = '<input type="submit" value="Save and edit content blocks" name="_contentblocks">'
```

### Comparing `django-content-blocks-1.2.1/content_blocks/admin_forms.py` & `django-content-blocks-1.3.0/content_blocks/signals.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,126 +1,138 @@
-import json
-
-from django import forms
+"""
+Content blocks app signals.py
+"""
+from django.contrib.contenttypes.models import ContentType
+from django.db import IntegrityError, OperationalError, ProgrammingError
+from django.db.migrations.recorder import MigrationRecorder
+from django.db.models.signals import post_delete, post_save, pre_delete, pre_save
+from django.dispatch import receiver
 
+from content_blocks.conf import settings
 from content_blocks.models import (
     ContentBlock,
     ContentBlockField,
     ContentBlockFields,
-    ContentBlockTemplate,
-    ContentBlockTemplateField,
+    FileField,
+    ImageField,
+    VideoField,
 )
-from content_blocks.widgets import ChoicesWidget, TemplateFilenameAutocompleteWidget
-
-REQUIRED_ERROR_MSG = "This field is required"
+from content_blocks.services.content_block import CacheServices
 
+if not settings.CONTENT_BLOCKS_DISABLE_UPDATE_CACHE_MODEL_CHOICE:
 
-class ContentBlockTemplateAdminForm(forms.ModelForm):
-    class Meta:
-        model = ContentBlockTemplate
-        exclude = []
-        widgets = {
-            "template_filename": TemplateFilenameAutocompleteWidget(
-                "/content_blocks/content_blocks"
+    @receiver(post_save, dispatch_uid="update_cache_model_choice_save")
+    @receiver(post_delete, dispatch_uid="update_cache_model_choice_delete")
+    def update_cache_model_choice(sender, instance, **kwargs):
+        """
+        Clear the cache for content blocks when related objects are saved. Model choice fields.
+        """
+        # todo:
+        #  remove this.  updating cache is flakey at best because changes to related objects can also require a
+        #  cache update but this won't trigger it.  It is better to document the need to set no_cache=True for
+        #  ContentBlockTemplate containing ContentBlockModelChoiceField or to manage updating the cache yourself.
+        if kwargs.get("raw", False):
+            # Prevent this signal from running during loaddata.
+            return
+
+        if sender == MigrationRecorder.Migration:
+            # Do not run the signal for MigrationRecorder.Migration otherwise migrations will fail
+            return
+
+        try:
+            content_block_fields = ContentBlockField.objects.filter(
+                model_choice_content_type=ContentType.objects.get_for_model(sender),
+                model_choice_object_id=getattr(instance, "id", None),
             )
-        }
-
-
-def validate_choices(choices):
-    try:
-        choices = json.loads(choices)
-    except json.JSONDecodeError:
-        return False
-
-    if not isinstance(choices, list):
-        return False
-
-    for choice in choices:
-        if not isinstance(choice, list):
-            return False
-
-        if not len(choice) == 2:
-            return False
-
-    return True
-
 
-class ContentBlockTemplateFieldAdminForm(forms.ModelForm):
-    class Meta:
-        model = ContentBlockTemplateField
-        exclude = []
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.fields["choices"] = forms.CharField(
-            widget=ChoicesWidget(),
-            help_text="You must provide a value and label for each choice or it will be ignored.",
-            required=False,
-        )
-
-    def clean(self):
-        cleaned_data = super().clean()
-
-        field_type = cleaned_data.get("field_type")
-
-        if field_type == ContentBlockFields.NESTED_FIELD:
-            nested_templates = cleaned_data.get("nested_templates")
-            if not nested_templates:
-                self.add_error("nested_templates", REQUIRED_ERROR_MSG)
-
-            min_num = cleaned_data.get("min_num")
-            max_num = cleaned_data.get("max_num")
-
-            if min_num > max_num:
-                self.add_error(
-                    "min_num", "Min num must be less than or equal to max num."
-                )
-                self.add_error(
-                    "max_num", "Max num must be greater than or equal to min num."
-                )
-
-        elif field_type == ContentBlockFields.CHOICE_FIELD:
-            choices = cleaned_data.get("choices")
-            if not choices:
-                self.add_error("choices", REQUIRED_ERROR_MSG)
-            elif not validate_choices(choices):
-                # Validate choices
-                self.add_error("choices", "Invalid choices")
-
-        elif field_type == ContentBlockFields.MODEL_CHOICE_FIELD:
-            model_choice_content_type = cleaned_data.get("model_choice_content_type")
-            if not model_choice_content_type:
-                self.add_error("model_choice_content_type", REQUIRED_ERROR_MSG)
-
-        if self.instance.pk and "field_type" in self.changed_data:
-            self.add_error("field_type", "Field type cannot be changed after save")
+            content_blocks = ContentBlock.objects.filter(
+                content_block_fields__in=content_block_fields
+            )
 
-        return cleaned_data
+            CacheServices.set_cache_all(queryset=content_blocks)
 
-    def save(self, commit=True):
+        except (
+            OperationalError,
+            ProgrammingError,
+            IntegrityError,
+            ContentType.DoesNotExist,
+        ):  # pragma: no cover
+            """
+            Content blocks not migrated yet.
+            """
+            return
+
+
+if "dbtemplates" in settings.INSTALLED_APPS:
+    from dbtemplates.models import Template
+
+    @receiver(post_save, sender=Template, dispatch_uid="update_cache_template_save")
+    @receiver(post_delete, sender=Template, dispatch_uid="update_cache_template_delete")
+    def update_cache_template(sender, instance, **kwargs):
         """
-        Update content block fields based on this template field.
+        Update the cache for content blocks when their db template is saved.
         """
-        template_field = super().save(commit=False)
-
-        created = False if template_field.pk else True
+        if kwargs.get("raw", False):
+            # Prevent this signal from running during loaddata.
+            return
 
-        # Find existing content blocks using this field
         content_blocks = ContentBlock.objects.filter(
-            content_block_template=template_field.content_block_template
+            content_block_template__template_filename=instance.name.split("/")[-1]
         )
-        create_content_block_fields = created and content_blocks.exists()
 
-        if commit or create_content_block_fields:
-            template_field.save()
-            self.save_m2m()
-
-        if create_content_block_fields:
-            # Create a new field for existing content blocks
-            for content_block in content_blocks:
-                ContentBlockField.objects.create(
-                    template_field=template_field,
-                    content_block=content_block,
-                    field_type=template_field.field_type,
-                )
+        CacheServices.set_cache_all(queryset=content_blocks)
 
-        return template_field
+
+def cleanup_media(sender, instance, delete=False, **kwargs):
+    """
+    Delete old media files when no longer needed.
+    """
+    if kwargs.get("raw", False):
+        # Prevent this signal from running during loaddata.
+        return
+
+    if instance.id is None:
+        return  # New object being created
+
+    object_types = {
+        ContentBlockFields.IMAGE_FIELD: "image",
+        ContentBlockFields.FILE_FIELD: "file",
+        ContentBlockFields.VIDEO_FIELD: "video",
+    }
+
+    object_type = object_types.get(instance.field_type)
+    if object_type is None:
+        return  # pragma: no cover
+
+    if delete:
+        old_file = getattr(instance, object_type)
+        new_file = None
+    else:
+        try:
+            old_file = getattr(
+                ContentBlockField.objects.get(id=instance.id), object_type
+            )
+            new_file = getattr(instance, object_type)
+        except ContentBlockField.DoesNotExist:  # pragma: no cover
+            return
+
+    if (
+        old_file != new_file
+        and not ContentBlockField.objects.filter(**{object_type: old_file})
+        .exclude(id=instance.id)
+        .exists()
+    ):
+        old_file.delete(save=False)
+
+
+@receiver(pre_save, sender=ImageField, dispatch_uid="cleanup_image_media_save")
+@receiver(pre_save, sender=FileField, dispatch_uid="cleanup_file_media_save")
+@receiver(pre_save, sender=VideoField, dispatch_uid="cleanup_video_media_save")
+def cleanup_media_save(sender, instance, **kwargs):
+    return cleanup_media(sender, instance, delete=False, **kwargs)
+
+
+@receiver(pre_delete, sender=ImageField, dispatch_uid="cleanup_image_media_delete")
+@receiver(pre_delete, sender=FileField, dispatch_uid="cleanup_file_media_delete")
+@receiver(pre_delete, sender=VideoField, dispatch_uid="cleanup_video_media_delete")
+def cleanup_media_delete(sender, instance, **kwargs):
+    return cleanup_media(sender, instance, delete=True, **kwargs)
```

### Comparing `django-content-blocks-1.2.1/content_blocks/apps.py` & `django-content-blocks-1.3.0/content_blocks/apps.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,35 @@
 import logging
 
 from django.apps import AppConfig
 from django.db import OperationalError, ProgrammingError
-from django.template import TemplateDoesNotExist
 
 from content_blocks.conf import settings
 
 logger = logging.getLogger(__name__)
 
 
 class ContentBlocksConfig(AppConfig):
     name = "content_blocks"
     verbose_name = "Content blocks"
 
     def ready(self):
-        from content_blocks.models import ContentBlock
         from content_blocks.signals import (  # noqa
             cleanup_media_delete,
             cleanup_media_save,
         )
 
         if not settings.CONTENT_BLOCKS_DISABLE_UPDATE_CACHE_MODEL_CHOICE:
             from content_blocks.signals import update_cache_model_choice  # noqa
 
         if "dbtemplates" in settings.INSTALLED_APPS:
             from content_blocks.signals import update_cache_template  # noqa
 
         if not settings.CONTENT_BLOCKS_DISABLE_CACHE_ON_START:
             try:
-                for content_block in ContentBlock.objects.filter(
-                    parent__isnull=True,
-                    content_block_template__template_filename__isnull=False,
-                    draft=False,
-                ):
-                    try:
-                        content_block.render()
-                    except TemplateDoesNotExist:  # pragma: no cover
-                        logger.error(
-                            f"No template found when rendering {content_block}"
-                        )
+                from content_blocks.services.content_block import CacheServices
+
+                CacheServices.get_or_set_cache_all()
 
             except (OperationalError, ProgrammingError):  # pragma: no cover
                 # Migrate hasn't been run yet.
                 pass  # pragma: no cover
```

### Comparing `django-content-blocks-1.2.1/content_blocks/conf.py` & `django-content-blocks-1.3.0/content_blocks/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 from django.conf import settings as django_settings
 
 
 class ContentBlocksSettings:
     # Choose which cache to use for content blocks
     CONTENT_BLOCKS_CACHE = "default"
+    CONTENT_BLOCKS_CACHE_PREFIX = "content_block"
 
     # Disable caching of content blocks
     CONTENT_BLOCKS_DISABLE_CACHE = False
 
     # Disable caching of content blocks on start
     CONTENT_BLOCKS_DISABLE_CACHE_ON_START = False
 
@@ -31,21 +32,21 @@
         "DEFAULT_FILE_STORAGE",
         "django.core.files.storage.FileSystemStorage",
     )
 
     # Set the default status message.  Can be a callable.
     CONTENT_BLOCKS_DEFAULT_STATUS_MESSAGE = ""
 
-    def __getattribute__(self, name):
-        try:
-            return getattr(django_settings, name)
-        except AttributeError:
-            return super().__getattribute__(name)
-
     # Mark context for TextField and ContentField as safe. Useful for allowing html in these fields.
     CONTENT_BLOCKS_MARK_SAFE = False
 
     # Use a textarea widget for TextFields.
     CONTENT_BLOCKS_TEXTFIELD_TEXTAREA = False
 
+    def __getattribute__(self, name):
+        try:
+            return getattr(django_settings, name)
+        except AttributeError:
+            return super().__getattribute__(name)
+
 
 settings = ContentBlocksSettings()
```

### Comparing `django-content-blocks-1.2.1/content_blocks/fields.py` & `django-content-blocks-1.3.0/content_blocks/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import xml.etree.cElementTree as et
+import xml.etree.ElementTree as et
 from pathlib import Path
 
 from django import forms
 from django.core.exceptions import ValidationError
 from django.core.validators import (
     FileExtensionValidator,
     get_available_image_extensions,
```

### Comparing `django-content-blocks-1.2.1/content_blocks/forms.py` & `django-content-blocks-1.3.0/content_blocks/forms.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from content_blocks.models import (
     ContentBlock,
     ContentBlockAvailability,
     ContentBlockField,
     ContentBlockFields,
     ContentBlockTemplate,
 )
+from content_blocks.services.content_block import CacheServices, CloneServices
 
 
 class ParentModelForm(forms.Form):
     """
     Adds parent object to form from kwargs.
     """
 
@@ -45,14 +46,15 @@
     def get_available_templates(self):
         """
         Must be provided by subclasses.
         """
         raise NotImplementedError  # pragma: no cover
 
     def create_content_block(self, content_block_template, draft=False, **kwargs):
+        # todo refactor to service class
         content_block = ContentBlock.objects.create(
             content_block_template=content_block_template,
             draft=draft,
             position=self.cleaned_data.get("position", 0),
             **kwargs,
         )
 
@@ -84,27 +86,29 @@
     Creates new content block object with appropriate fields on save.
     Updates the parent which the content block belongs to m2m on save.
     """
 
     auto_id = "new_cb_%s"
 
     def get_available_templates(self):
+        # todo refactor to service class
         try:
             content_type = ContentType.objects.get_for_model(self.parent)
             content_block_availability = ContentBlockAvailability.objects.get(
                 content_type=content_type
             )
             return content_block_availability.content_block_templates.visible()
         except ContentBlockAvailability.DoesNotExist:
             return ContentBlockTemplate.objects.visible()
 
     def update_parent_m2m(self, content_block):
         self.parent.content_blocks.add(content_block)
 
     def save(self):
+        # todo call service class
         content_block = self.create_content_block(
             self.cleaned_data["content_block_template"], draft=True
         )
         self.update_parent_m2m(content_block)
         return content_block
 
 
@@ -116,21 +120,23 @@
     parent = forms.ModelChoiceField(
         widget=forms.HiddenInput(), queryset=ContentBlockField.objects.all()
     )
 
     auto_id = False
 
     def get_available_templates(self):
+        # todo refactor to service class
         try:
             parent = self.initial["parent"]
             return parent.template_field.nested_templates.visible()
         except KeyError:
             return ContentBlockTemplate.objects.all()
 
     def save(self):
+        # todo call service class
         return self.create_content_block(
             self.cleaned_data["content_block_template"],
             draft=False,
             parent=self.cleaned_data["parent"],
         )
 
 
@@ -158,54 +164,61 @@
     def set_fields(self):
         for key, field in self.content_block.fields.items():
             form_field = field.form_field
             if form_field:
                 self.fields[key] = form_field
 
     def save(self):
+        # todo refactor to service class?
         with transaction.atomic():
             for key, field in self.content_block.fields.items():
                 if key in self.cleaned_data.keys():
                     field.save_value(self.cleaned_data.get(key))
 
             self.content_block.css_class = self.cleaned_data.get("css_class")
             self.content_block.saved = True
             self.content_block.save()
-            # This is problematic as parent blocks can try to render without nested blocks validating
-            # self.content_block.update_cache()
-            self.content_block.clear_cache()
+
+            # We no longer manage the cache here as drafts and nested blocks are not cached.
+
         return self.content_block
 
 
 class PublishContentBlocksForm(ParentModelForm):
     """
     Form for publishing content blocks.
     Duplicates all content blocks and fields and nested blocks and sets draft=False
     """
 
     def save(self):
+        # todo refactor to service class
         self.parent.content_blocks.published().delete()
 
         for content_block in self.parent.content_blocks.drafts():
-            new_content_block = content_block.clone(attrs={"draft": False})
+            new_content_block = CloneServices.clone_content_block(
+                content_block, attrs={"draft": False}
+            )
             self.parent.content_blocks.add(new_content_block)
             # Cache the html
-            new_content_block.render()
+            CacheServices.set_cache_content_block_parent(new_content_block, self.parent)
 
 
 class ResetContentBlocksForm(ParentModelForm):
     """
     Deletes existing draft content blocks and creates new from published content blocks.
     """
 
     def save(self):
+        # todo refactor to service class
         self.parent.content_blocks.drafts().delete()
 
         for content_block in self.parent.content_blocks.published():
-            new_content_block = content_block.clone(attrs={"draft": True})
+            new_content_block = CloneServices.clone_content_block(
+                content_block, attrs={"draft": True}
+            )
             self.parent.content_blocks.add(new_content_block)
 
 
 class ImportContentBlocksForm(ParentModelForm):
     """
     Import content blocks from another master object of the same type as parent.
     """
@@ -216,12 +229,13 @@
         super().__init__(*args, **kwargs)
         self.fields["master"].queryset = self.get_master_queryset()
 
     def get_master_queryset(self):
         return self.parent._meta.model.objects.exclude(id=self.parent.id)
 
     def save(self):
+        # todo refactor to service class
         self.parent.content_blocks.drafts().delete()
 
         for content_block in self.cleaned_data["master"].content_blocks.drafts():
-            new_content_block = content_block.clone()
+            new_content_block = CloneServices.clone_content_block(content_block)
             self.parent.content_blocks.add(new_content_block)
```

### Comparing `django-content-blocks-1.2.1/content_blocks/migrations/0001_initial.py` & `django-content-blocks-1.3.0/content_blocks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.2.1/content_blocks/migrations/0002_alter_contentblock_css_class_and_more.py` & `django-content-blocks-1.3.0/content_blocks/migrations/0002_alter_contentblock_css_class_and_more.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.2.1/content_blocks/models.py` & `django-content-blocks-1.3.0/content_blocks/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,27 +7,26 @@
 from django import forms
 from django.contrib.contenttypes.fields import GenericForeignKey
 from django.contrib.contenttypes.models import ContentType
 from django.core.files.storage import get_storage_class
 from django.core.validators import RegexValidator
 from django.db import models
 from django.forms.utils import pretty_name
-from django.template.loader import render_to_string
+from django.template.exceptions import TemplateDoesNotExist
+from django.template.loader import get_template
 from django.utils.functional import cached_property
 from django.utils.safestring import mark_safe
 from model_clone import CloneMixin
 
 from content_blocks.abstract_models import (
     AutoDateModel,
-    CachedHtmlModel,
     PositionModel,
     VisibleManager,
     VisibleModel,
 )
-from content_blocks.cache import cache
 from content_blocks.conf import settings
 from content_blocks.fields import (
     SVGAndImageField,
     SVGAndImageFieldFormField,
     VideoField,
 )
 from content_blocks.widgets import FileWidget
@@ -64,16 +63,14 @@
 
 
 def get_storage(field_type):
     """
     Get the storage class from dotted strings in settings.
     If the field storage class is in settings use that otherwise use the general storage class setting for content
     blocks, which will default to STORAGES["default"].
-    :param field_type:
-    :return:
     """
     storage_setting = getattr(settings, field_type, None)
     if storage_setting is not None:
         return get_storage_class(
             storage_setting
         )()  # pragma: no cover (covered by settings specific tests)
     return get_storage_class(settings.CONTENT_BLOCKS_STORAGE)()
@@ -468,65 +465,62 @@
         """
         :return: Nested content blocks which we can then call render or access context on.
         """
         return self.content_blocks.nested()
 
 
 class ContentBlockManager(VisibleManager):
+    # todo consider moving some of these to service classes. Only need to keep those used in templates here?
     def get_queryset(self):
+        """
+        Basic optimisation.
+        """
         return (
             super()
             .get_queryset()
             .prefetch_related("content_block_fields")
             .select_related("content_block_template")
         )
 
     def visible(self):
         """
         Visible published only.
         Used in templates to render published content blocks.
-        :return:
         """
         return super().visible().filter(draft=False)
 
     def previews(self):
         """
         Visible drafts only. Exclude those which haven't been saved via the editor yet (empties).
         Can be used in page previews.
-        :return:
         """
         return super().visible().filter(draft=True, saved=True)
 
     def nested(self):
         """
         Used in the context for NestedField objects. Visible but with unsaved excluded.
-        :return:
         """
         return super().visible().filter(draft=False, saved=True)
 
     def published(self):
         """
         All published including visible=False.
         Used by the publishing/reset mechanism.
-        :return:
         """
         return self.get_queryset().filter(draft=False)
 
     def drafts(self):
         """
         All drafts including visible=False.
         Used by the editor and publishing/reset mechanism.
-        :return:
         """
         return self.get_queryset().filter(draft=True)
 
 
-class ContentBlock(
-    PositionModel, AutoDateModel, VisibleModel, CloneMixin, CachedHtmlModel
-):
+class ContentBlock(PositionModel, AutoDateModel, VisibleModel, CloneMixin):
     """
     Content Block Model
     Content block fields point here.  Those created are based on the content block template.
     """
 
     objects = ContentBlockManager()
 
@@ -544,15 +538,14 @@
     css_class = models.CharField(max_length=64, blank=True)
 
     draft = models.BooleanField(blank=True, default=False)
 
     saved = models.BooleanField(blank=True, default=False)
 
     context_name = "content_block"
-    cache_prefix = "content_block"
 
     @cached_property
     def template(self):
         """
         HTML template
         """
         return self.content_block_template.template or None
@@ -589,113 +582,98 @@
         """
         Return dictionary of template context for this content block
         """
         context = {key: field.context_value for key, field in self.fields.items()}
         context["css_class"] = self.css_class
         return context
 
-    def render(self, context=None, request=None):
+    @cached_property
+    def can_render(self):
         """
-        Render html for this block and cache
+        :return: True if the template exists.
         """
-        if not self.can_render:
-            return ""
-
-        context = context or {}
-        request = request or context.get("request")
-
-        context[self.context_name] = self.context
-        context["request"] = request
-
-        cache_enabled = (
-            not self.content_block_template.no_cache
-            and not settings.CONTENT_BLOCKS_DISABLE_CACHE
-        )
-
-        html = None
-        if cache_enabled:
-            html = cache.get(self.cache_key)
+        if not self.template:
+            return False
+        try:
+            get_template(self.template)
+            return True
+        except TemplateDoesNotExist:
+            return False
 
-        if html is None:
-            html = render_to_string(
-                self.template,
-                context,
-                request=request,
-            )
-
-            if cache_enabled:
-                cache.set(self.cache_key, html)
-
-        return html
-
-    def clear_cache(self):
+    @cached_property
+    def can_cache(self):
         """
-        Clear the cache for this block and any parent blocks
+        :return: True if the ContentBlock can be cached.
         """
-        super().clear_cache()
-        if self.parent:
-            self.parent.content_block.clear_cache()
-
-    def update_cache(self):
-        if "context" in self.__dict__.keys():
-            # Clear the context cached property if present
-            del self.__dict__["context"]
-
-        super().update_cache()
-        if self.parent:
-            self.parent.content_block.update_cache()
+        return (
+            not settings.CONTENT_BLOCKS_DISABLE_CACHE  # Don't cache if disabled in settings
+            and not self.draft  # Don't cache drafts
+            and self.parent is None  # Don't cache nested content blocks
+            and not self.content_block_template.no_cache  # Don't cache if the template is marked no_cache
+            and self.can_render  # Can't cache what can't be rendered
+        )
 
-    def clone(self, attrs=None):
+    def render(self):
         """
-        Clones the given content block and all content block fields.
+        Render html for this block and cache.
+        This should only be called by the template and exists to support legacy projects.
+        The {% render_content_block %} template tag should be used in preference.
         """
-        new_content_block = self.make_clone(attrs=attrs)
+        from content_blocks.services.content_block import RenderServices
 
-        for field in self.content_block_fields.all():
-            new_field = field.make_clone(attrs={"content_block": new_content_block})
+        return RenderServices.render_content_block(self)
 
-            if field.template_field.field_type == ContentBlockFields.NESTED_FIELD:
-                for nested_block in field.content_blocks.all():
-                    nested_block.clone(attrs={"parent": new_field})
 
-        return new_content_block
+class ContentBlockTemplateManager(VisibleManager):
+    def get_by_natural_key(self, name):
+        return self.get(name=name)
 
 
 class ContentBlockTemplate(PositionModel, AutoDateModel, VisibleModel):
     """
     Content Block Template model.
     Used to define content block types.
     """
 
-    objects = VisibleManager()
+    objects = ContentBlockTemplateManager()
 
     name = models.CharField(max_length=256, unique=True)
 
     template_filename = models.CharField(max_length=256, blank=True)
 
     no_cache = models.BooleanField(
         default=False,
         help_text="Disable caching for content blocks created with this template.",
     )
 
     def __str__(self):
         return self.name
 
+    def natural_key(self):
+        return (self.name,)
+
     @property
     def template(self):
         if self.template_filename:
             return f"content_blocks/content_blocks/{self.template_filename}"
 
 
+class ContentBlockTemplateFieldManager(models.Manager):
+    def get_by_natural_key(self, key, content_block_template):
+        return self.get(key=key, content_block_template=content_block_template)
+
+
 class ContentBlockTemplateField(PositionModel):
     """
     Content Block Template Field model.
     Used to define content block types.
     """
 
+    objects = ContentBlockTemplateFieldManager()
+
     content_block_template = models.ForeignKey(
         ContentBlockTemplate,
         on_delete=models.CASCADE,
         related_name="content_block_template_fields",
     )
 
     field_type = models.CharField(max_length=32, choices=ContentBlockFields.choices)
@@ -737,19 +715,30 @@
 
     # Only used if field_type == ModelChoiceField
     model_choice_content_type = models.ForeignKey(
         ContentType, on_delete=models.CASCADE, blank=True, null=True
     )
 
     class Meta(PositionModel.Meta):
-        unique_together = ("key", "content_block_template")
+        constraints = [
+            models.UniqueConstraint(
+                fields=["key", "content_block_template"],
+                name="unique_key_content_block_template",
+            )
+        ]
 
     def __str__(self):
         return self.key or super().__str__()
 
+    def natural_key(self):
+        return (
+            self.key,
+            self.content_block_template,
+        )
+
 
 class ContentBlockAvailability(AutoDateModel):
     """
     Used to set which content block templates can be added to a model.
     """
 
     # null=True is required for admin list to work. blank=False because this is a required field.
@@ -776,14 +765,23 @@
     class Meta:
         abstract = True
 
     def delete(self, using=None, keep_parents=False):
         self.content_blocks.all().delete()
         return super().delete(using=using, keep_parents=keep_parents)
 
+    @property
+    def content_blocks_sites_field(self):
+        """
+        For use with per site cacheing. Define which field on your model is either a FK or M2M to Site.
+        E.g.
+        return self.sites
+        """
+        return None
+
 
 class ContentBlockCollection(AutoDateModel, ContentBlockParentModel):
     """
     Simple collections of content blocks identified by slug.
     Use the content_blocks_collection template tag to render a content block collection in a template.
     """
```

### Comparing `django-content-blocks-1.2.1/content_blocks/static/content_blocks/.DS_Store` & `django-content-blocks-1.3.0/content_blocks/static/content_blocks/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.2.1/content_blocks/static/content_blocks/css/.DS_Store` & `django-content-blocks-1.3.0/content_blocks/static/content_blocks/css/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.2.1/content_blocks/static/content_blocks/css/content_block_template_admin.css` & `django-content-blocks-1.3.0/content_blocks/static/content_blocks/css/content_block_template_admin.css`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 /*CSS for Content Block Template admin change page*/
 
 /* Choices widget */
 
 .choices-widget {
-    padding-left:170px;
+  padding-left: 170px;
 }
 
 .choices-widget .inputs {
-    clear:left;
+  clear: left;
 }
 
 .choices-widget .input-row {
-    padding-bottom:5px;
+  padding-bottom: 5px;
 }
 
 .choices-widget .input-row input:first-child {
-    margin-right:18px;
+  margin-right: 18px;
 }
 
 .choices-widget button {
-    outline: none;
-    border:none;
-    background-color: transparent;
-    color: var(--link-fg);
-    cursor: pointer;
-    font-size: 12px;
-    transition: color 0.15s, background 0.15s;
+  outline: none;
+  border: none;
+  background-color: transparent;
+  color: var(--link-fg);
+  cursor: pointer;
+  font-size: 12px;
+  transition:
+    color 0.15s,
+    background 0.15s;
 }
 .choices-widget button:hover {
-    color: var(--link-hover-color);
+  color: var(--link-hover-color);
 }
 
 .choices-widget button.add-choice-row {
-    padding-left:0;
+  padding-left: 0;
 }
 
 /* Smaller help text textarea */
 .field-help_text textarea {
-    height: 50px;
-}
+  height: 50px;
+}
```

### Comparing `django-content-blocks-1.2.1/content_blocks/static/content_blocks/fontawesome/.DS_Store` & `django-content-blocks-1.3.0/content_blocks/templates/content_blocks/.DS_Store`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
 00000010: 0000 1000 0000 0209 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0008  ................
-00000050: 0000 0001 0000 1000 3153 636f 6d70 0000  ........1Scomp..
-00000060: 0000 0001 0000 0000 0000 0000 0000 0000  ................
+00000040: 0000 0000 0000 0002 0000 0000 0000 000c  ................
+00000050: 0000 0001 0000 1000 0065 006e 0074 005f  .........e.n.t._
+00000060: 0062 006c 0000 0000 0000 0000 0000 0000  .b.l............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -26,46 +26,46 @@
 00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000200: 0000 0000 0000 0000 0000 0008 0000 0003  ................
-00000210: 0063 0073 0073 6c67 3153 636f 6d70 0000  .c.s.slg1Scomp..
-00000220: 0000 0001 58ed 0000 0003 0063 0073 0073  ....X......c.s.s
-00000230: 6d6f 4444 626c 6f62 0000 0008 e346 aea9  moDDblob.....F..
-00000240: 9fd6 c441 0000 0003 0063 0073 0073 6d6f  ...A.....c.s.smo
-00000250: 6444 626c 6f62 0000 0008 e346 aea9 9fd6  dDblob.....F....
-00000260: c441 0000 0003 0063 0073 0073 7068 3153  .A.....c.s.sph1S
-00000270: 636f 6d70 0000 0000 0001 a000 0000 0008  comp............
-00000280: 0077 0065 0062 0066 006f 006e 0074 0073  .w.e.b.f.o.n.t.s
-00000290: 6c67 3153 636f 6d70 0000 0000 0008 4fe4  lg1Scomp......O.
-000002a0: 0000 0008 0077 0065 0062 0066 006f 006e  .....w.e.b.f.o.n
-000002b0: 0074 0073 6d6f 4444 626c 6f62 0000 0008  .t.smoDDblob....
-000002c0: c13f ab9b 9dd6 c441 0000 0008 0077 0065  .?.....A.....w.e
-000002d0: 0062 0066 006f 006e 0074 0073 6d6f 6444  .b.f.o.n.t.smodD
-000002e0: 626c 6f62 0000 0008 c13f ab9b 9dd6 c441  blob.....?.....A
-000002f0: 0000 0008 0077 0065 0062 0066 006f 006e  .....w.e.b.f.o.n
-00000300: 0074 0073 7068 3153 636f 6d70 0000 0000  .t.sph1Scomp....
-00000310: 0008 6000 0000 0000 0000 0000 0000 0000  ..`.............
-00000320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000003c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000003d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000200: 0000 0000 0000 0000 0000 000c 0000 000e  ................
+00000210: 0063 006f 006e 0074 0065 006e 0074 005f  .c.o.n.t.e.n.t._
+00000220: 0062 006c 006f 0063 006b 0073 6c67 3153  .b.l.o.c.k.slg1S
+00000230: 636f 6d70 0000 0000 0000 42a3 0000 000e  comp......B.....
+00000240: 0063 006f 006e 0074 0065 006e 0074 005f  .c.o.n.t.e.n.t._
+00000250: 0062 006c 006f 0063 006b 0073 6d6f 4444  .b.l.o.c.k.smoDD
+00000260: 626c 6f62 0000 0008 a41a 51e1 4fc9 c441  blob......Q.O..A
+00000270: 0000 000e 0063 006f 006e 0074 0065 006e  .....c.o.n.t.e.n
+00000280: 0074 005f 0062 006c 006f 0063 006b 0073  .t._.b.l.o.c.k.s
+00000290: 6d6f 6444 626c 6f62 0000 0008 a41a 51e1  modDblob......Q.
+000002a0: 4fc9 c441 0000 000e 0063 006f 006e 0074  O..A.....c.o.n.t
+000002b0: 0065 006e 0074 005f 0062 006c 006f 0063  .e.n.t._.b.l.o.c
+000002c0: 006b 0073 7068 3153 636f 6d70 0000 0000  .k.sph1Scomp....
+000002d0: 0001 7000 0000 0008 0070 0061 0072 0074  ..p......p.a.r.t
+000002e0: 0069 0061 006c 0073 6c67 3153 636f 6d70  .i.a.l.slg1Scomp
+000002f0: 0000 0000 0000 0c82 0000 0008 0070 0061  .............p.a
+00000300: 0072 0074 0069 0061 006c 0073 6d6f 4444  .r.t.i.a.l.smoDD
+00000310: 626c 6f62 0000 0008 871d 0e3c 4dc4 c441  blob.......<M..A
+00000320: 0000 0008 0070 0061 0072 0074 0069 0061  .....p.a.r.t.i.a
+00000330: 006c 0073 6d6f 6444 626c 6f62 0000 0008  .l.smodDblob....
+00000340: 871d 0e3c 4dc4 c441 0000 0008 0070 0061  ...<M..A.....p.a
+00000350: 0072 0074 0069 0061 006c 0073 7068 3153  .r.t.i.a.l.sph1S
+00000360: 636f 6d70 0000 0000 0000 a000 0000 0007  comp............
+00000370: 0077 0069 0064 0067 0065 0074 0073 6c67  .w.i.d.g.e.t.slg
+00000380: 3153 636f 6d70 0000 0000 0000 0445 0000  1Scomp.......E..
+00000390: 0007 0077 0069 0064 0067 0065 0074 0073  ...w.i.d.g.e.t.s
+000003a0: 6d6f 4444 626c 6f62 0000 0008 ff52 1d2c  moDDblob.....R.,
+000003b0: edc4 c441 0000 0007 0077 0069 0064 0067  ...A.....w.i.d.g
+000003c0: 0065 0074 0073 6d6f 6444 626c 6f62 0000  .e.t.smodDblob..
+000003d0: 0008 ff52 1d2c edc4 c441 0000 0007 0077  ...R.,...A.....w
+000003e0: 0069 0064 0067 0065 0074 0073 7068 3153  .i.d.g.e.t.sph1S
+000003f0: 636f 6d70 0000 0000 0000 2000 0000 0000  comp...... .....
 00000400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000430: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000440: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000450: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000460: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `django-content-blocks-1.2.1/content_blocks/static/content_blocks/fontawesome/css/procompatibility.css` & `django-content-blocks-1.3.0/content_blocks/static/content_blocks/fontawesome/css/procompatibility.css`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 /*
 Some icons do not exist in the free fa-solid set.
 So we replace them with icons that do exist here.
 This file should be loaded before fontawesome.css so when a pro fontawesome.css is used this is overridden.
 */
 
 .fa-chevrons-down::before {
-  content: "\f078"; }
+  content: '\f078';
+}
 .fa-chevrons-up::before {
-  content: "\f077"; }
+  content: '\f077';
+}
 
 .fa-floppy-disk-circle-arrow-right::before {
-    content: "\f061";}
+  content: '\f061';
+}
 
 .fa-floppy-disk-circle-xmark::before {
-    content: "\f0c7";}
+  content: '\f0c7';
+}
 
 .fa-image-slash::before {
-    content: "\f03e";}
+  content: '\f03e';
+}
 
 .fa-film-slash::before {
-    content: "\f008";}
+  content: '\f008';
+}
 
 .fa-trash-slash::before {
-    content: "\f1f8";}
+  content: '\f1f8';
+}
 
 /* Because we can't always change icons now use opacity to differentiate states */
 
 .controls .fa-floppy-disk,
 .controls .fa-trash-slash {
-    opacity: 0.4;
-}
+  opacity: 0.4;
+}
```

### Comparing `django-content-blocks-1.2.1/content_blocks/static/content_blocks/fontawesome/css/solid.min.css` & `django-content-blocks-1.3.0/content_blocks/static/content_blocks/fontawesome/css/solid.min.css`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 /*!
  * Font Awesome Free 6.3.0 by @fontawesome - https://fontawesome.com
  * License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License)
  * Copyright 2023 Fonticons, Inc.
  */
-:host,:root{--fa-style-family-classic:"Font Awesome 6 Free";--fa-font-solid:normal 900 1em/1 "Font Awesome 6 Free"}@font-face{font-family:"Font Awesome 6 Free";font-style:normal;font-weight:900;font-display:block;src:url(../webfonts/fa-solid-900.woff2) format("woff2"),url(../webfonts/fa-solid-900.ttf) format("truetype")}.fa-solid,.fas{font-weight:900}
+:host,:root{--fa-style-family-classic:"Font Awesome 6 Free";--fa-font-solid:normal 900 1em/1 "Font Awesome 6 Free"}@font-face{font-family:"Font Awesome 6 Free";font-style:normal;font-weight:900;font-display:block;src:url(../webfonts/fa-solid-900.woff2) format("woff2"),url(../webfonts/fa-solid-900.ttf) format("truetype")}.fa-solid,.fas{font-weight:900}
```

### Comparing `django-content-blocks-1.2.1/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.ttf` & `django-content-blocks-1.3.0/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.2.1/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.woff2` & `django-content-blocks-1.3.0/content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.2.1/content_blocks/static/content_blocks/iframeresizer/iframeResizer.contentWindow.js` & `django-content-blocks-1.3.0/content_blocks/static/content_blocks/iframeresizer/iframeResizer.contentWindow.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, ASCII text*

 * *Files 0% similar despite different names*

```diff
@@ -2169,8 +2169,8 @@
 00008780: 7374 656e 6572 2877 696e 646f 772c 2027  stener(window, '
 00008790: 6d65 7373 6167 6527 2c20 7265 6365 6976  message', receiv
 000087a0: 6572 290a 2020 6164 6445 7665 6e74 4c69  er).  addEventLi
 000087b0: 7374 656e 6572 2877 696e 646f 772c 2027  stener(window, '
 000087c0: 7265 6164 7973 7461 7465 6368 616e 6765  readystatechange
 000087d0: 272c 2063 686b 4c61 7465 4c6f 6164 6564  ', chkLateLoaded
 000087e0: 290a 2020 6368 6b4c 6174 654c 6f61 6465  ).  chkLateLoade
-000087f0: 6428 290a 0a20 200a 7d29 2829 0a         d()..  .})().
+000087f0: 6428 290a 0a0a 7d29 2829 0a              d()...})().
```

### Comparing `django-content-blocks-1.2.1/content_blocks/static/content_blocks/iframeresizer/iframeResizer.js` & `django-content-blocks-1.3.0/content_blocks/static/content_blocks/iframeresizer/iframeResizer.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.2.1/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js` & `django-content-blocks-1.3.0/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.2.1/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js.map` & `django-content-blocks-1.3.0/content_blocks/static/content_blocks/jqueryform/jquery.form.min.js.map`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -1404,8 +1404,8 @@
 000057b0: 572c 4541 414b 2c49 4141 7542 2c65 4141  W,EAAK,IAAuB,eAA
 000057c0: 6a42 412c 4541 414b 2c47 4141 476c 532c  jBA,EAAK,GAAGlS,
 000057d0: 4d41 4568 436b 532c 4541 414b 502c 4b41  MAEhCkS,EAAKP,KA
 000057e0: 414b 2c55 4141 5564 2c55 4141 532c 4741  AK,UAAUd,UAAS,GA
 000057f0: 4739 4272 502c 4b41 414b 7150 2c53 4141  G9BrP,KAAKqP,SAA
 00005800: 5755 2c4d 414d 6e42 7054 2c45 4141 4555  WU,MAMnBpT,EAAEU
 00005810: 2c47 4141 4755 2c57 4141 5775 422c 4f41  ,GAAGU,WAAWuB,OA
-00005820: 4151 227d                                AQ"}
+00005820: 4151 227d 0a                             AQ"}.
```

### Comparing `django-content-blocks-1.2.1/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.css` & `django-content-blocks-1.3.0/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.css`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 /*! jQuery UI - v1.13.2 - 2022-08-17
 * http://jqueryui.com
 * Includes: draggable.css, core.css, resizable.css, selectable.css, sortable.css, accordion.css, autocomplete.css, menu.css, button.css, controlgroup.css, checkboxradio.css, datepicker.css, dialog.css, progressbar.css, selectmenu.css, slider.css, spinner.css, tabs.css, tooltip.css, theme.css
 * To view and modify this theme, visit http://jqueryui.com/themeroller/?scope=&folderName=base&cornerRadiusShadow=8px&offsetLeftShadow=0px&offsetTopShadow=0px&thicknessShadow=5px&opacityShadow=30&bgImgOpacityShadow=0&bgTextureShadow=flat&bgColorShadow=666666&opacityOverlay=30&bgImgOpacityOverlay=0&bgTextureOverlay=flat&bgColorOverlay=aaaaaa&iconColorError=cc0000&fcError=5f3f3f&borderColorError=f1a899&bgTextureError=flat&bgColorError=fddfdf&iconColorHighlight=777620&fcHighlight=777620&borderColorHighlight=dad55e&bgTextureHighlight=flat&bgColorHighlight=fffa90&iconColorActive=ffffff&fcActive=ffffff&borderColorActive=003eff&bgTextureActive=flat&bgColorActive=007fff&iconColorHover=555555&fcHover=2b2b2b&borderColorHover=cccccc&bgTextureHover=flat&bgColorHover=ededed&iconColorDefault=777777&fcDefault=454545&borderColorDefault=c5c5c5&bgTextureDefault=flat&bgColorDefault=f6f6f6&iconColorContent=444444&fcContent=333333&borderColorContent=dddddd&bgTextureContent=flat&bgColorContent=ffffff&iconColorHeader=444444&fcHeader=333333&borderColorHeader=dddddd&bgTextureHeader=flat&bgColorHeader=e9e9e9&cornerRadius=3px&fwDefault=normal&fsDefault=1em&ffDefault=Arial%2CHelvetica%2Csans-serif
 * Copyright jQuery Foundation and other contributors; Licensed MIT */
 
-.ui-draggable-handle{-ms-touch-action:none;touch-action:none}.ui-helper-hidden{display:none}.ui-helper-hidden-accessible{border:0;clip:rect(0 0 0 0);height:1px;margin:-1px;overflow:hidden;padding:0;position:absolute;width:1px}.ui-helper-reset{margin:0;padding:0;border:0;outline:0;line-height:1.3;text-decoration:none;font-size:100%;list-style:none}.ui-helper-clearfix:before,.ui-helper-clearfix:after{content:"";display:table;border-collapse:collapse}.ui-helper-clearfix:after{clear:both}.ui-helper-zfix{width:100%;height:100%;top:0;left:0;position:absolute;opacity:0;-ms-filter:"alpha(opacity=0)"}.ui-front{z-index:100}.ui-state-disabled{cursor:default!important;pointer-events:none}.ui-icon{display:inline-block;vertical-align:middle;margin-top:-.25em;position:relative;text-indent:-99999px;overflow:hidden;background-repeat:no-repeat}.ui-widget-icon-block{left:50%;margin-left:-8px;display:block}.ui-widget-overlay{position:fixed;top:0;left:0;width:100%;height:100%}.ui-resizable{position:relative}.ui-resizable-handle{position:absolute;font-size:0.1px;display:block;-ms-touch-action:none;touch-action:none}.ui-resizable-disabled .ui-resizable-handle,.ui-resizable-autohide .ui-resizable-handle{display:none}.ui-resizable-n{cursor:n-resize;height:7px;width:100%;top:-5px;left:0}.ui-resizable-s{cursor:s-resize;height:7px;width:100%;bottom:-5px;left:0}.ui-resizable-e{cursor:e-resize;width:7px;right:-5px;top:0;height:100%}.ui-resizable-w{cursor:w-resize;width:7px;left:-5px;top:0;height:100%}.ui-resizable-se{cursor:se-resize;width:12px;height:12px;right:1px;bottom:1px}.ui-resizable-sw{cursor:sw-resize;width:9px;height:9px;left:-5px;bottom:-5px}.ui-resizable-nw{cursor:nw-resize;width:9px;height:9px;left:-5px;top:-5px}.ui-resizable-ne{cursor:ne-resize;width:9px;height:9px;right:-5px;top:-5px}.ui-selectable{-ms-touch-action:none;touch-action:none}.ui-selectable-helper{position:absolute;z-index:100;border:1px dotted black}.ui-sortable-handle{-ms-touch-action:none;touch-action:none}.ui-accordion .ui-accordion-header{display:block;cursor:pointer;position:relative;margin:2px 0 0 0;padding:.5em .5em .5em .7em;font-size:100%}.ui-accordion .ui-accordion-content{padding:1em 2.2em;border-top:0;overflow:auto}.ui-autocomplete{position:absolute;top:0;left:0;cursor:default}.ui-menu{list-style:none;padding:0;margin:0;display:block;outline:0}.ui-menu .ui-menu{position:absolute}.ui-menu .ui-menu-item{margin:0;cursor:pointer;list-style-image:url("data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7")}.ui-menu .ui-menu-item-wrapper{position:relative;padding:3px 1em 3px .4em}.ui-menu .ui-menu-divider{margin:5px 0;height:0;font-size:0;line-height:0;border-width:1px 0 0 0}.ui-menu .ui-state-focus,.ui-menu .ui-state-active{margin:-1px}.ui-menu-icons{position:relative}.ui-menu-icons .ui-menu-item-wrapper{padding-left:2em}.ui-menu .ui-icon{position:absolute;top:0;bottom:0;left:.2em;margin:auto 0}.ui-menu .ui-menu-icon{left:auto;right:0}.ui-button{padding:.4em 1em;display:inline-block;position:relative;line-height:normal;margin-right:.1em;cursor:pointer;vertical-align:middle;text-align:center;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;overflow:visible}.ui-button,.ui-button:link,.ui-button:visited,.ui-button:hover,.ui-button:active{text-decoration:none}.ui-button-icon-only{width:2em;box-sizing:border-box;text-indent:-9999px;white-space:nowrap}input.ui-button.ui-button-icon-only{text-indent:0}.ui-button-icon-only .ui-icon{position:absolute;top:50%;left:50%;margin-top:-8px;margin-left:-8px}.ui-button.ui-icon-notext .ui-icon{padding:0;width:2.1em;height:2.1em;text-indent:-9999px;white-space:nowrap}input.ui-button.ui-icon-notext .ui-icon{width:auto;height:auto;text-indent:0;white-space:normal;padding:.4em 1em}input.ui-button::-moz-focus-inner,button.ui-button::-moz-focus-inner{border:0;padding:0}.ui-controlgroup{vertical-align:middle;display:inline-block}.ui-controlgroup > .ui-controlgroup-item{float:left;margin-left:0;margin-right:0}.ui-controlgroup > .ui-controlgroup-item:focus,.ui-controlgroup > .ui-controlgroup-item.ui-visual-focus{z-index:9999}.ui-controlgroup-vertical > .ui-controlgroup-item{display:block;float:none;width:100%;margin-top:0;margin-bottom:0;text-align:left}.ui-controlgroup-vertical .ui-controlgroup-item{box-sizing:border-box}.ui-controlgroup .ui-controlgroup-label{padding:.4em 1em}.ui-controlgroup .ui-controlgroup-label span{font-size:80%}.ui-controlgroup-horizontal .ui-controlgroup-label + .ui-controlgroup-item{border-left:none}.ui-controlgroup-vertical .ui-controlgroup-label + .ui-controlgroup-item{border-top:none}.ui-controlgroup-horizontal .ui-controlgroup-label.ui-widget-content{border-right:none}.ui-controlgroup-vertical .ui-controlgroup-label.ui-widget-content{border-bottom:none}.ui-controlgroup-vertical .ui-spinner-input{width:75%;width:calc( 100% - 2.4em )}.ui-controlgroup-vertical .ui-spinner .ui-spinner-up{border-top-style:solid}.ui-checkboxradio-label .ui-icon-background{box-shadow:inset 1px 1px 1px #ccc;border-radius:.12em;border:none}.ui-checkboxradio-radio-label .ui-icon-background{width:16px;height:16px;border-radius:1em;overflow:visible;border:none}.ui-checkboxradio-radio-label.ui-checkboxradio-checked .ui-icon,.ui-checkboxradio-radio-label.ui-checkboxradio-checked:hover .ui-icon{background-image:none;width:8px;height:8px;border-width:4px;border-style:solid}.ui-checkboxradio-disabled{pointer-events:none}.ui-datepicker{width:17em;padding:.2em .2em 0;display:none}.ui-datepicker .ui-datepicker-header{position:relative;padding:.2em 0}.ui-datepicker .ui-datepicker-prev,.ui-datepicker .ui-datepicker-next{position:absolute;top:2px;width:1.8em;height:1.8em}.ui-datepicker .ui-datepicker-prev-hover,.ui-datepicker .ui-datepicker-next-hover{top:1px}.ui-datepicker .ui-datepicker-prev{left:2px}.ui-datepicker .ui-datepicker-next{right:2px}.ui-datepicker .ui-datepicker-prev-hover{left:1px}.ui-datepicker .ui-datepicker-next-hover{right:1px}.ui-datepicker .ui-datepicker-prev span,.ui-datepicker .ui-datepicker-next span{display:block;position:absolute;left:50%;margin-left:-8px;top:50%;margin-top:-8px}.ui-datepicker .ui-datepicker-title{margin:0 2.3em;line-height:1.8em;text-align:center}.ui-datepicker .ui-datepicker-title select{font-size:1em;margin:1px 0}.ui-datepicker select.ui-datepicker-month,.ui-datepicker select.ui-datepicker-year{width:45%}.ui-datepicker table{width:100%;font-size:.9em;border-collapse:collapse;margin:0 0 .4em}.ui-datepicker th{padding:.7em .3em;text-align:center;font-weight:bold;border:0}.ui-datepicker td{border:0;padding:1px}.ui-datepicker td span,.ui-datepicker td a{display:block;padding:.2em;text-align:right;text-decoration:none}.ui-datepicker .ui-datepicker-buttonpane{background-image:none;margin:.7em 0 0 0;padding:0 .2em;border-left:0;border-right:0;border-bottom:0}.ui-datepicker .ui-datepicker-buttonpane button{float:right;margin:.5em .2em .4em;cursor:pointer;padding:.2em .6em .3em .6em;width:auto;overflow:visible}.ui-datepicker .ui-datepicker-buttonpane button.ui-datepicker-current{float:left}.ui-datepicker.ui-datepicker-multi{width:auto}.ui-datepicker-multi .ui-datepicker-group{float:left}.ui-datepicker-multi .ui-datepicker-group table{width:95%;margin:0 auto .4em}.ui-datepicker-multi-2 .ui-datepicker-group{width:50%}.ui-datepicker-multi-3 .ui-datepicker-group{width:33.3%}.ui-datepicker-multi-4 .ui-datepicker-group{width:25%}.ui-datepicker-multi .ui-datepicker-group-last .ui-datepicker-header,.ui-datepicker-multi .ui-datepicker-group-middle .ui-datepicker-header{border-left-width:0}.ui-datepicker-multi .ui-datepicker-buttonpane{clear:left}.ui-datepicker-row-break{clear:both;width:100%;font-size:0}.ui-datepicker-rtl{direction:rtl}.ui-datepicker-rtl .ui-datepicker-prev{right:2px;left:auto}.ui-datepicker-rtl .ui-datepicker-next{left:2px;right:auto}.ui-datepicker-rtl .ui-datepicker-prev:hover{right:1px;left:auto}.ui-datepicker-rtl .ui-datepicker-next:hover{left:1px;right:auto}.ui-datepicker-rtl .ui-datepicker-buttonpane{clear:right}.ui-datepicker-rtl .ui-datepicker-buttonpane button{float:left}.ui-datepicker-rtl .ui-datepicker-buttonpane button.ui-datepicker-current,.ui-datepicker-rtl .ui-datepicker-group{float:right}.ui-datepicker-rtl .ui-datepicker-group-last .ui-datepicker-header,.ui-datepicker-rtl .ui-datepicker-group-middle .ui-datepicker-header{border-right-width:0;border-left-width:1px}.ui-datepicker .ui-icon{display:block;text-indent:-99999px;overflow:hidden;background-repeat:no-repeat;left:.5em;top:.3em}.ui-dialog{position:absolute;top:0;left:0;padding:.2em;outline:0}.ui-dialog .ui-dialog-titlebar{padding:.4em 1em;position:relative}.ui-dialog .ui-dialog-title{float:left;margin:.1em 0;white-space:nowrap;width:90%;overflow:hidden;text-overflow:ellipsis}.ui-dialog .ui-dialog-titlebar-close{position:absolute;right:.3em;top:50%;width:20px;margin:-10px 0 0 0;padding:1px;height:20px}.ui-dialog .ui-dialog-content{position:relative;border:0;padding:.5em 1em;background:none;overflow:auto}.ui-dialog .ui-dialog-buttonpane{text-align:left;border-width:1px 0 0 0;background-image:none;margin-top:.5em;padding:.3em 1em .5em .4em}.ui-dialog .ui-dialog-buttonpane .ui-dialog-buttonset{float:right}.ui-dialog .ui-dialog-buttonpane button{margin:.5em .4em .5em 0;cursor:pointer}.ui-dialog .ui-resizable-n{height:2px;top:0}.ui-dialog .ui-resizable-e{width:2px;right:0}.ui-dialog .ui-resizable-s{height:2px;bottom:0}.ui-dialog .ui-resizable-w{width:2px;left:0}.ui-dialog .ui-resizable-se,.ui-dialog .ui-resizable-sw,.ui-dialog .ui-resizable-ne,.ui-dialog .ui-resizable-nw{width:7px;height:7px}.ui-dialog .ui-resizable-se{right:0;bottom:0}.ui-dialog .ui-resizable-sw{left:0;bottom:0}.ui-dialog .ui-resizable-ne{right:0;top:0}.ui-dialog .ui-resizable-nw{left:0;top:0}.ui-draggable .ui-dialog-titlebar{cursor:move}.ui-progressbar{height:2em;text-align:left;overflow:hidden}.ui-progressbar .ui-progressbar-value{margin:-1px;height:100%}.ui-progressbar .ui-progressbar-overlay{background:url("data:image/gif;base64,R0lGODlhKAAoAIABAAAAAP///yH/C05FVFNDQVBFMi4wAwEAAAAh+QQJAQABACwAAAAAKAAoAAACkYwNqXrdC52DS06a7MFZI+4FHBCKoDeWKXqymPqGqxvJrXZbMx7Ttc+w9XgU2FB3lOyQRWET2IFGiU9m1frDVpxZZc6bfHwv4c1YXP6k1Vdy292Fb6UkuvFtXpvWSzA+HycXJHUXiGYIiMg2R6W459gnWGfHNdjIqDWVqemH2ekpObkpOlppWUqZiqr6edqqWQAAIfkECQEAAQAsAAAAACgAKAAAApSMgZnGfaqcg1E2uuzDmmHUBR8Qil95hiPKqWn3aqtLsS18y7G1SzNeowWBENtQd+T1JktP05nzPTdJZlR6vUxNWWjV+vUWhWNkWFwxl9VpZRedYcflIOLafaa28XdsH/ynlcc1uPVDZxQIR0K25+cICCmoqCe5mGhZOfeYSUh5yJcJyrkZWWpaR8doJ2o4NYq62lAAACH5BAkBAAEALAAAAAAoACgAAAKVDI4Yy22ZnINRNqosw0Bv7i1gyHUkFj7oSaWlu3ovC8GxNso5fluz3qLVhBVeT/Lz7ZTHyxL5dDalQWPVOsQWtRnuwXaFTj9jVVh8pma9JjZ4zYSj5ZOyma7uuolffh+IR5aW97cHuBUXKGKXlKjn+DiHWMcYJah4N0lYCMlJOXipGRr5qdgoSTrqWSq6WFl2ypoaUAAAIfkECQEAAQAsAAAAACgAKAAAApaEb6HLgd/iO7FNWtcFWe+ufODGjRfoiJ2akShbueb0wtI50zm02pbvwfWEMWBQ1zKGlLIhskiEPm9R6vRXxV4ZzWT2yHOGpWMyorblKlNp8HmHEb/lCXjcW7bmtXP8Xt229OVWR1fod2eWqNfHuMjXCPkIGNileOiImVmCOEmoSfn3yXlJWmoHGhqp6ilYuWYpmTqKUgAAIfkECQEAAQAsAAAAACgAKAAAApiEH6kb58biQ3FNWtMFWW3eNVcojuFGfqnZqSebuS06w5V80/X02pKe8zFwP6EFWOT1lDFk8rGERh1TTNOocQ61Hm4Xm2VexUHpzjymViHrFbiELsefVrn6XKfnt2Q9G/+Xdie499XHd2g4h7ioOGhXGJboGAnXSBnoBwKYyfioubZJ2Hn0RuRZaflZOil56Zp6iioKSXpUAAAh+QQJAQABACwAAAAAKAAoAAACkoQRqRvnxuI7kU1a1UU5bd5tnSeOZXhmn5lWK3qNTWvRdQxP8qvaC+/yaYQzXO7BMvaUEmJRd3TsiMAgswmNYrSgZdYrTX6tSHGZO73ezuAw2uxuQ+BbeZfMxsexY35+/Qe4J1inV0g4x3WHuMhIl2jXOKT2Q+VU5fgoSUI52VfZyfkJGkha6jmY+aaYdirq+lQAACH5BAkBAAEALAAAAAAoACgAAAKWBIKpYe0L3YNKToqswUlvznigd4wiR4KhZrKt9Upqip61i9E3vMvxRdHlbEFiEXfk9YARYxOZZD6VQ2pUunBmtRXo1Lf8hMVVcNl8JafV38aM2/Fu5V16Bn63r6xt97j09+MXSFi4BniGFae3hzbH9+hYBzkpuUh5aZmHuanZOZgIuvbGiNeomCnaxxap2upaCZsq+1kAACH5BAkBAAEALAAAAAAoACgAAAKXjI8By5zf4kOxTVrXNVlv1X0d8IGZGKLnNpYtm8Lr9cqVeuOSvfOW79D9aDHizNhDJidFZhNydEahOaDH6nomtJjp1tutKoNWkvA6JqfRVLHU/QUfau9l2x7G54d1fl995xcIGAdXqMfBNadoYrhH+Mg2KBlpVpbluCiXmMnZ2Sh4GBqJ+ckIOqqJ6LmKSllZmsoq6wpQAAAh+QQJAQABACwAAAAAKAAoAAAClYx/oLvoxuJDkU1a1YUZbJ59nSd2ZXhWqbRa2/gF8Gu2DY3iqs7yrq+xBYEkYvFSM8aSSObE+ZgRl1BHFZNr7pRCavZ5BW2142hY3AN/zWtsmf12p9XxxFl2lpLn1rseztfXZjdIWIf2s5dItwjYKBgo9yg5pHgzJXTEeGlZuenpyPmpGQoKOWkYmSpaSnqKileI2FAAACH5BAkBAAEALAAAAAAoACgAAAKVjB+gu+jG4kORTVrVhRlsnn2dJ3ZleFaptFrb+CXmO9OozeL5VfP99HvAWhpiUdcwkpBH3825AwYdU8xTqlLGhtCosArKMpvfa1mMRae9VvWZfeB2XfPkeLmm18lUcBj+p5dnN8jXZ3YIGEhYuOUn45aoCDkp16hl5IjYJvjWKcnoGQpqyPlpOhr3aElaqrq56Bq7VAAAOw==");height:100%;-ms-filter:"alpha(opacity=25)";opacity:0.25}.ui-progressbar-indeterminate .ui-progressbar-value{background-image:none}.ui-selectmenu-menu{padding:0;margin:0;position:absolute;top:0;left:0;display:none}.ui-selectmenu-menu .ui-menu{overflow:auto;overflow-x:hidden;padding-bottom:1px}.ui-selectmenu-menu .ui-menu .ui-selectmenu-optgroup{font-size:1em;font-weight:bold;line-height:1.5;padding:2px 0.4em;margin:0.5em 0 0 0;height:auto;border:0}.ui-selectmenu-open{display:block}.ui-selectmenu-text{display:block;margin-right:20px;overflow:hidden;text-overflow:ellipsis}.ui-selectmenu-button.ui-button{text-align:left;white-space:nowrap;width:14em}.ui-selectmenu-icon.ui-icon{float:right;margin-top:0}.ui-slider{position:relative;text-align:left}.ui-slider .ui-slider-handle{position:absolute;z-index:2;width:1.2em;height:1.2em;cursor:pointer;-ms-touch-action:none;touch-action:none}.ui-slider .ui-slider-range{position:absolute;z-index:1;font-size:.7em;display:block;border:0;background-position:0 0}.ui-slider.ui-state-disabled .ui-slider-handle,.ui-slider.ui-state-disabled .ui-slider-range{filter:inherit}.ui-slider-horizontal{height:.8em}.ui-slider-horizontal .ui-slider-handle{top:-.3em;margin-left:-.6em}.ui-slider-horizontal .ui-slider-range{top:0;height:100%}.ui-slider-horizontal .ui-slider-range-min{left:0}.ui-slider-horizontal .ui-slider-range-max{right:0}.ui-slider-vertical{width:.8em;height:100px}.ui-slider-vertical .ui-slider-handle{left:-.3em;margin-left:0;margin-bottom:-.6em}.ui-slider-vertical .ui-slider-range{left:0;width:100%}.ui-slider-vertical .ui-slider-range-min{bottom:0}.ui-slider-vertical .ui-slider-range-max{top:0}.ui-spinner{position:relative;display:inline-block;overflow:hidden;padding:0;vertical-align:middle}.ui-spinner-input{border:none;background:none;color:inherit;padding:.222em 0;margin:.2em 0;vertical-align:middle;margin-left:.4em;margin-right:2em}.ui-spinner-button{width:1.6em;height:50%;font-size:.5em;padding:0;margin:0;text-align:center;position:absolute;cursor:default;display:block;overflow:hidden;right:0}.ui-spinner a.ui-spinner-button{border-top-style:none;border-bottom-style:none;border-right-style:none}.ui-spinner-up{top:0}.ui-spinner-down{bottom:0}.ui-tabs{position:relative;padding:.2em}.ui-tabs .ui-tabs-nav{margin:0;padding:.2em .2em 0}.ui-tabs .ui-tabs-nav li{list-style:none;float:left;position:relative;top:0;margin:1px .2em 0 0;border-bottom-width:0;padding:0;white-space:nowrap}.ui-tabs .ui-tabs-nav .ui-tabs-anchor{float:left;padding:.5em 1em;text-decoration:none}.ui-tabs .ui-tabs-nav li.ui-tabs-active{margin-bottom:-1px;padding-bottom:1px}.ui-tabs .ui-tabs-nav li.ui-tabs-active .ui-tabs-anchor,.ui-tabs .ui-tabs-nav li.ui-state-disabled .ui-tabs-anchor,.ui-tabs .ui-tabs-nav li.ui-tabs-loading .ui-tabs-anchor{cursor:text}.ui-tabs-collapsible .ui-tabs-nav li.ui-tabs-active .ui-tabs-anchor{cursor:pointer}.ui-tabs .ui-tabs-panel{display:block;border-width:0;padding:1em 1.4em;background:none}.ui-tooltip{padding:8px;position:absolute;z-index:9999;max-width:300px}body .ui-tooltip{border-width:2px}.ui-widget{font-family:Arial,Helvetica,sans-serif;font-size:1em}.ui-widget .ui-widget{font-size:1em}.ui-widget input,.ui-widget select,.ui-widget textarea,.ui-widget button{font-family:Arial,Helvetica,sans-serif;font-size:1em}.ui-widget.ui-widget-content{border:1px solid #c5c5c5}.ui-widget-content{border:1px solid #ddd;background:#fff;color:#333}.ui-widget-content a{color:#333}.ui-widget-header{border:1px solid #ddd;background:#e9e9e9;color:#333;font-weight:bold}.ui-widget-header a{color:#333}.ui-state-default,.ui-widget-content .ui-state-default,.ui-widget-header .ui-state-default,.ui-button,html .ui-button.ui-state-disabled:hover,html .ui-button.ui-state-disabled:active{border:1px solid #c5c5c5;background:#f6f6f6;font-weight:normal;color:#454545}.ui-state-default a,.ui-state-default a:link,.ui-state-default a:visited,a.ui-button,a:link.ui-button,a:visited.ui-button,.ui-button{color:#454545;text-decoration:none}.ui-state-hover,.ui-widget-content .ui-state-hover,.ui-widget-header .ui-state-hover,.ui-state-focus,.ui-widget-content .ui-state-focus,.ui-widget-header .ui-state-focus,.ui-button:hover,.ui-button:focus{border:1px solid #ccc;background:#ededed;font-weight:normal;color:#2b2b2b}.ui-state-hover a,.ui-state-hover a:hover,.ui-state-hover a:link,.ui-state-hover a:visited,.ui-state-focus a,.ui-state-focus a:hover,.ui-state-focus a:link,.ui-state-focus a:visited,a.ui-button:hover,a.ui-button:focus{color:#2b2b2b;text-decoration:none}.ui-visual-focus{box-shadow:0 0 3px 1px rgb(94,158,214)}.ui-state-active,.ui-widget-content .ui-state-active,.ui-widget-header .ui-state-active,a.ui-button:active,.ui-button:active,.ui-button.ui-state-active:hover{border:1px solid #003eff;background:#007fff;font-weight:normal;color:#fff}.ui-icon-background,.ui-state-active .ui-icon-background{border:#003eff;background-color:#fff}.ui-state-active a,.ui-state-active a:link,.ui-state-active a:visited{color:#fff;text-decoration:none}.ui-state-highlight,.ui-widget-content .ui-state-highlight,.ui-widget-header .ui-state-highlight{border:1px solid #dad55e;background:#fffa90;color:#777620}.ui-state-checked{border:1px solid #dad55e;background:#fffa90}.ui-state-highlight a,.ui-widget-content .ui-state-highlight a,.ui-widget-header .ui-state-highlight a{color:#777620}.ui-state-error,.ui-widget-content .ui-state-error,.ui-widget-header .ui-state-error{border:1px solid #f1a899;background:#fddfdf;color:#5f3f3f}.ui-state-error a,.ui-widget-content .ui-state-error a,.ui-widget-header .ui-state-error a{color:#5f3f3f}.ui-state-error-text,.ui-widget-content .ui-state-error-text,.ui-widget-header .ui-state-error-text{color:#5f3f3f}.ui-priority-primary,.ui-widget-content .ui-priority-primary,.ui-widget-header .ui-priority-primary{font-weight:bold}.ui-priority-secondary,.ui-widget-content .ui-priority-secondary,.ui-widget-header .ui-priority-secondary{opacity:.7;-ms-filter:"alpha(opacity=70)";font-weight:normal}.ui-state-disabled,.ui-widget-content .ui-state-disabled,.ui-widget-header .ui-state-disabled{opacity:.35;-ms-filter:"alpha(opacity=35)";background-image:none}.ui-state-disabled .ui-icon{-ms-filter:"alpha(opacity=35)"}.ui-icon{width:16px;height:16px}.ui-icon,.ui-widget-content .ui-icon{background-image:url("images/ui-icons_444444_256x240.png")}.ui-widget-header .ui-icon{background-image:url("images/ui-icons_444444_256x240.png")}.ui-state-hover .ui-icon,.ui-state-focus .ui-icon,.ui-button:hover .ui-icon,.ui-button:focus .ui-icon{background-image:url("images/ui-icons_555555_256x240.png")}.ui-state-active .ui-icon,.ui-button:active .ui-icon{background-image:url("images/ui-icons_ffffff_256x240.png")}.ui-state-highlight .ui-icon,.ui-button .ui-state-highlight.ui-icon{background-image:url("images/ui-icons_777620_256x240.png")}.ui-state-error .ui-icon,.ui-state-error-text .ui-icon{background-image:url("images/ui-icons_cc0000_256x240.png")}.ui-button .ui-icon{background-image:url("images/ui-icons_777777_256x240.png")}.ui-icon-blank.ui-icon-blank.ui-icon-blank{background-image:none}.ui-icon-caret-1-n{background-position:0 0}.ui-icon-caret-1-ne{background-position:-16px 0}.ui-icon-caret-1-e{background-position:-32px 0}.ui-icon-caret-1-se{background-position:-48px 0}.ui-icon-caret-1-s{background-position:-65px 0}.ui-icon-caret-1-sw{background-position:-80px 0}.ui-icon-caret-1-w{background-position:-96px 0}.ui-icon-caret-1-nw{background-position:-112px 0}.ui-icon-caret-2-n-s{background-position:-128px 0}.ui-icon-caret-2-e-w{background-position:-144px 0}.ui-icon-triangle-1-n{background-position:0 -16px}.ui-icon-triangle-1-ne{background-position:-16px -16px}.ui-icon-triangle-1-e{background-position:-32px -16px}.ui-icon-triangle-1-se{background-position:-48px -16px}.ui-icon-triangle-1-s{background-position:-65px -16px}.ui-icon-triangle-1-sw{background-position:-80px -16px}.ui-icon-triangle-1-w{background-position:-96px -16px}.ui-icon-triangle-1-nw{background-position:-112px -16px}.ui-icon-triangle-2-n-s{background-position:-128px -16px}.ui-icon-triangle-2-e-w{background-position:-144px -16px}.ui-icon-arrow-1-n{background-position:0 -32px}.ui-icon-arrow-1-ne{background-position:-16px -32px}.ui-icon-arrow-1-e{background-position:-32px -32px}.ui-icon-arrow-1-se{background-position:-48px -32px}.ui-icon-arrow-1-s{background-position:-65px -32px}.ui-icon-arrow-1-sw{background-position:-80px -32px}.ui-icon-arrow-1-w{background-position:-96px -32px}.ui-icon-arrow-1-nw{background-position:-112px -32px}.ui-icon-arrow-2-n-s{background-position:-128px -32px}.ui-icon-arrow-2-ne-sw{background-position:-144px -32px}.ui-icon-arrow-2-e-w{background-position:-160px -32px}.ui-icon-arrow-2-se-nw{background-position:-176px -32px}.ui-icon-arrowstop-1-n{background-position:-192px -32px}.ui-icon-arrowstop-1-e{background-position:-208px -32px}.ui-icon-arrowstop-1-s{background-position:-224px -32px}.ui-icon-arrowstop-1-w{background-position:-240px -32px}.ui-icon-arrowthick-1-n{background-position:1px -48px}.ui-icon-arrowthick-1-ne{background-position:-16px -48px}.ui-icon-arrowthick-1-e{background-position:-32px -48px}.ui-icon-arrowthick-1-se{background-position:-48px -48px}.ui-icon-arrowthick-1-s{background-position:-64px -48px}.ui-icon-arrowthick-1-sw{background-position:-80px -48px}.ui-icon-arrowthick-1-w{background-position:-96px -48px}.ui-icon-arrowthick-1-nw{background-position:-112px -48px}.ui-icon-arrowthick-2-n-s{background-position:-128px -48px}.ui-icon-arrowthick-2-ne-sw{background-position:-144px -48px}.ui-icon-arrowthick-2-e-w{background-position:-160px -48px}.ui-icon-arrowthick-2-se-nw{background-position:-176px -48px}.ui-icon-arrowthickstop-1-n{background-position:-192px -48px}.ui-icon-arrowthickstop-1-e{background-position:-208px -48px}.ui-icon-arrowthickstop-1-s{background-position:-224px -48px}.ui-icon-arrowthickstop-1-w{background-position:-240px -48px}.ui-icon-arrowreturnthick-1-w{background-position:0 -64px}.ui-icon-arrowreturnthick-1-n{background-position:-16px -64px}.ui-icon-arrowreturnthick-1-e{background-position:-32px -64px}.ui-icon-arrowreturnthick-1-s{background-position:-48px -64px}.ui-icon-arrowreturn-1-w{background-position:-64px -64px}.ui-icon-arrowreturn-1-n{background-position:-80px -64px}.ui-icon-arrowreturn-1-e{background-position:-96px -64px}.ui-icon-arrowreturn-1-s{background-position:-112px -64px}.ui-icon-arrowrefresh-1-w{background-position:-128px -64px}.ui-icon-arrowrefresh-1-n{background-position:-144px -64px}.ui-icon-arrowrefresh-1-e{background-position:-160px -64px}.ui-icon-arrowrefresh-1-s{background-position:-176px -64px}.ui-icon-arrow-4{background-position:0 -80px}.ui-icon-arrow-4-diag{background-position:-16px -80px}.ui-icon-extlink{background-position:-32px -80px}.ui-icon-newwin{background-position:-48px -80px}.ui-icon-refresh{background-position:-64px -80px}.ui-icon-shuffle{background-position:-80px -80px}.ui-icon-transfer-e-w{background-position:-96px -80px}.ui-icon-transferthick-e-w{background-position:-112px -80px}.ui-icon-folder-collapsed{background-position:0 -96px}.ui-icon-folder-open{background-position:-16px -96px}.ui-icon-document{background-position:-32px -96px}.ui-icon-document-b{background-position:-48px -96px}.ui-icon-note{background-position:-64px -96px}.ui-icon-mail-closed{background-position:-80px -96px}.ui-icon-mail-open{background-position:-96px -96px}.ui-icon-suitcase{background-position:-112px -96px}.ui-icon-comment{background-position:-128px -96px}.ui-icon-person{background-position:-144px -96px}.ui-icon-print{background-position:-160px -96px}.ui-icon-trash{background-position:-176px -96px}.ui-icon-locked{background-position:-192px -96px}.ui-icon-unlocked{background-position:-208px -96px}.ui-icon-bookmark{background-position:-224px -96px}.ui-icon-tag{background-position:-240px -96px}.ui-icon-home{background-position:0 -112px}.ui-icon-flag{background-position:-16px -112px}.ui-icon-calendar{background-position:-32px -112px}.ui-icon-cart{background-position:-48px -112px}.ui-icon-pencil{background-position:-64px -112px}.ui-icon-clock{background-position:-80px -112px}.ui-icon-disk{background-position:-96px -112px}.ui-icon-calculator{background-position:-112px -112px}.ui-icon-zoomin{background-position:-128px -112px}.ui-icon-zoomout{background-position:-144px -112px}.ui-icon-search{background-position:-160px -112px}.ui-icon-wrench{background-position:-176px -112px}.ui-icon-gear{background-position:-192px -112px}.ui-icon-heart{background-position:-208px -112px}.ui-icon-star{background-position:-224px -112px}.ui-icon-link{background-position:-240px -112px}.ui-icon-cancel{background-position:0 -128px}.ui-icon-plus{background-position:-16px -128px}.ui-icon-plusthick{background-position:-32px -128px}.ui-icon-minus{background-position:-48px -128px}.ui-icon-minusthick{background-position:-64px -128px}.ui-icon-close{background-position:-80px -128px}.ui-icon-closethick{background-position:-96px -128px}.ui-icon-key{background-position:-112px -128px}.ui-icon-lightbulb{background-position:-128px -128px}.ui-icon-scissors{background-position:-144px -128px}.ui-icon-clipboard{background-position:-160px -128px}.ui-icon-copy{background-position:-176px -128px}.ui-icon-contact{background-position:-192px -128px}.ui-icon-image{background-position:-208px -128px}.ui-icon-video{background-position:-224px -128px}.ui-icon-script{background-position:-240px -128px}.ui-icon-alert{background-position:0 -144px}.ui-icon-info{background-position:-16px -144px}.ui-icon-notice{background-position:-32px -144px}.ui-icon-help{background-position:-48px -144px}.ui-icon-check{background-position:-64px -144px}.ui-icon-bullet{background-position:-80px -144px}.ui-icon-radio-on{background-position:-96px -144px}.ui-icon-radio-off{background-position:-112px -144px}.ui-icon-pin-w{background-position:-128px -144px}.ui-icon-pin-s{background-position:-144px -144px}.ui-icon-play{background-position:0 -160px}.ui-icon-pause{background-position:-16px -160px}.ui-icon-seek-next{background-position:-32px -160px}.ui-icon-seek-prev{background-position:-48px -160px}.ui-icon-seek-end{background-position:-64px -160px}.ui-icon-seek-start{background-position:-80px -160px}.ui-icon-seek-first{background-position:-80px -160px}.ui-icon-stop{background-position:-96px -160px}.ui-icon-eject{background-position:-112px -160px}.ui-icon-volume-off{background-position:-128px -160px}.ui-icon-volume-on{background-position:-144px -160px}.ui-icon-power{background-position:0 -176px}.ui-icon-signal-diag{background-position:-16px -176px}.ui-icon-signal{background-position:-32px -176px}.ui-icon-battery-0{background-position:-48px -176px}.ui-icon-battery-1{background-position:-64px -176px}.ui-icon-battery-2{background-position:-80px -176px}.ui-icon-battery-3{background-position:-96px -176px}.ui-icon-circle-plus{background-position:0 -192px}.ui-icon-circle-minus{background-position:-16px -192px}.ui-icon-circle-close{background-position:-32px -192px}.ui-icon-circle-triangle-e{background-position:-48px -192px}.ui-icon-circle-triangle-s{background-position:-64px -192px}.ui-icon-circle-triangle-w{background-position:-80px -192px}.ui-icon-circle-triangle-n{background-position:-96px -192px}.ui-icon-circle-arrow-e{background-position:-112px -192px}.ui-icon-circle-arrow-s{background-position:-128px -192px}.ui-icon-circle-arrow-w{background-position:-144px -192px}.ui-icon-circle-arrow-n{background-position:-160px -192px}.ui-icon-circle-zoomin{background-position:-176px -192px}.ui-icon-circle-zoomout{background-position:-192px -192px}.ui-icon-circle-check{background-position:-208px -192px}.ui-icon-circlesmall-plus{background-position:0 -208px}.ui-icon-circlesmall-minus{background-position:-16px -208px}.ui-icon-circlesmall-close{background-position:-32px -208px}.ui-icon-squaresmall-plus{background-position:-48px -208px}.ui-icon-squaresmall-minus{background-position:-64px -208px}.ui-icon-squaresmall-close{background-position:-80px -208px}.ui-icon-grip-dotted-vertical{background-position:0 -224px}.ui-icon-grip-dotted-horizontal{background-position:-16px -224px}.ui-icon-grip-solid-vertical{background-position:-32px -224px}.ui-icon-grip-solid-horizontal{background-position:-48px -224px}.ui-icon-gripsmall-diagonal-se{background-position:-64px -224px}.ui-icon-grip-diagonal-se{background-position:-80px -224px}.ui-corner-all,.ui-corner-top,.ui-corner-left,.ui-corner-tl{border-top-left-radius:3px}.ui-corner-all,.ui-corner-top,.ui-corner-right,.ui-corner-tr{border-top-right-radius:3px}.ui-corner-all,.ui-corner-bottom,.ui-corner-left,.ui-corner-bl{border-bottom-left-radius:3px}.ui-corner-all,.ui-corner-bottom,.ui-corner-right,.ui-corner-br{border-bottom-right-radius:3px}.ui-widget-overlay{background:#aaa;opacity:.3;-ms-filter:Alpha(Opacity=30)}.ui-widget-shadow{-webkit-box-shadow:0 0 5px #666;box-shadow:0 0 5px #666}
+.ui-draggable-handle{-ms-touch-action:none;touch-action:none}.ui-helper-hidden{display:none}.ui-helper-hidden-accessible{border:0;clip:rect(0 0 0 0);height:1px;margin:-1px;overflow:hidden;padding:0;position:absolute;width:1px}.ui-helper-reset{margin:0;padding:0;border:0;outline:0;line-height:1.3;text-decoration:none;font-size:100%;list-style:none}.ui-helper-clearfix:before,.ui-helper-clearfix:after{content:"";display:table;border-collapse:collapse}.ui-helper-clearfix:after{clear:both}.ui-helper-zfix{width:100%;height:100%;top:0;left:0;position:absolute;opacity:0;-ms-filter:"alpha(opacity=0)"}.ui-front{z-index:100}.ui-state-disabled{cursor:default!important;pointer-events:none}.ui-icon{display:inline-block;vertical-align:middle;margin-top:-.25em;position:relative;text-indent:-99999px;overflow:hidden;background-repeat:no-repeat}.ui-widget-icon-block{left:50%;margin-left:-8px;display:block}.ui-widget-overlay{position:fixed;top:0;left:0;width:100%;height:100%}.ui-resizable{position:relative}.ui-resizable-handle{position:absolute;font-size:0.1px;display:block;-ms-touch-action:none;touch-action:none}.ui-resizable-disabled .ui-resizable-handle,.ui-resizable-autohide .ui-resizable-handle{display:none}.ui-resizable-n{cursor:n-resize;height:7px;width:100%;top:-5px;left:0}.ui-resizable-s{cursor:s-resize;height:7px;width:100%;bottom:-5px;left:0}.ui-resizable-e{cursor:e-resize;width:7px;right:-5px;top:0;height:100%}.ui-resizable-w{cursor:w-resize;width:7px;left:-5px;top:0;height:100%}.ui-resizable-se{cursor:se-resize;width:12px;height:12px;right:1px;bottom:1px}.ui-resizable-sw{cursor:sw-resize;width:9px;height:9px;left:-5px;bottom:-5px}.ui-resizable-nw{cursor:nw-resize;width:9px;height:9px;left:-5px;top:-5px}.ui-resizable-ne{cursor:ne-resize;width:9px;height:9px;right:-5px;top:-5px}.ui-selectable{-ms-touch-action:none;touch-action:none}.ui-selectable-helper{position:absolute;z-index:100;border:1px dotted black}.ui-sortable-handle{-ms-touch-action:none;touch-action:none}.ui-accordion .ui-accordion-header{display:block;cursor:pointer;position:relative;margin:2px 0 0 0;padding:.5em .5em .5em .7em;font-size:100%}.ui-accordion .ui-accordion-content{padding:1em 2.2em;border-top:0;overflow:auto}.ui-autocomplete{position:absolute;top:0;left:0;cursor:default}.ui-menu{list-style:none;padding:0;margin:0;display:block;outline:0}.ui-menu .ui-menu{position:absolute}.ui-menu .ui-menu-item{margin:0;cursor:pointer;list-style-image:url("data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7")}.ui-menu .ui-menu-item-wrapper{position:relative;padding:3px 1em 3px .4em}.ui-menu .ui-menu-divider{margin:5px 0;height:0;font-size:0;line-height:0;border-width:1px 0 0 0}.ui-menu .ui-state-focus,.ui-menu .ui-state-active{margin:-1px}.ui-menu-icons{position:relative}.ui-menu-icons .ui-menu-item-wrapper{padding-left:2em}.ui-menu .ui-icon{position:absolute;top:0;bottom:0;left:.2em;margin:auto 0}.ui-menu .ui-menu-icon{left:auto;right:0}.ui-button{padding:.4em 1em;display:inline-block;position:relative;line-height:normal;margin-right:.1em;cursor:pointer;vertical-align:middle;text-align:center;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;overflow:visible}.ui-button,.ui-button:link,.ui-button:visited,.ui-button:hover,.ui-button:active{text-decoration:none}.ui-button-icon-only{width:2em;box-sizing:border-box;text-indent:-9999px;white-space:nowrap}input.ui-button.ui-button-icon-only{text-indent:0}.ui-button-icon-only .ui-icon{position:absolute;top:50%;left:50%;margin-top:-8px;margin-left:-8px}.ui-button.ui-icon-notext .ui-icon{padding:0;width:2.1em;height:2.1em;text-indent:-9999px;white-space:nowrap}input.ui-button.ui-icon-notext .ui-icon{width:auto;height:auto;text-indent:0;white-space:normal;padding:.4em 1em}input.ui-button::-moz-focus-inner,button.ui-button::-moz-focus-inner{border:0;padding:0}.ui-controlgroup{vertical-align:middle;display:inline-block}.ui-controlgroup > .ui-controlgroup-item{float:left;margin-left:0;margin-right:0}.ui-controlgroup > .ui-controlgroup-item:focus,.ui-controlgroup > .ui-controlgroup-item.ui-visual-focus{z-index:9999}.ui-controlgroup-vertical > .ui-controlgroup-item{display:block;float:none;width:100%;margin-top:0;margin-bottom:0;text-align:left}.ui-controlgroup-vertical .ui-controlgroup-item{box-sizing:border-box}.ui-controlgroup .ui-controlgroup-label{padding:.4em 1em}.ui-controlgroup .ui-controlgroup-label span{font-size:80%}.ui-controlgroup-horizontal .ui-controlgroup-label + .ui-controlgroup-item{border-left:none}.ui-controlgroup-vertical .ui-controlgroup-label + .ui-controlgroup-item{border-top:none}.ui-controlgroup-horizontal .ui-controlgroup-label.ui-widget-content{border-right:none}.ui-controlgroup-vertical .ui-controlgroup-label.ui-widget-content{border-bottom:none}.ui-controlgroup-vertical .ui-spinner-input{width:75%;width:calc( 100% - 2.4em )}.ui-controlgroup-vertical .ui-spinner .ui-spinner-up{border-top-style:solid}.ui-checkboxradio-label .ui-icon-background{box-shadow:inset 1px 1px 1px #ccc;border-radius:.12em;border:none}.ui-checkboxradio-radio-label .ui-icon-background{width:16px;height:16px;border-radius:1em;overflow:visible;border:none}.ui-checkboxradio-radio-label.ui-checkboxradio-checked .ui-icon,.ui-checkboxradio-radio-label.ui-checkboxradio-checked:hover .ui-icon{background-image:none;width:8px;height:8px;border-width:4px;border-style:solid}.ui-checkboxradio-disabled{pointer-events:none}.ui-datepicker{width:17em;padding:.2em .2em 0;display:none}.ui-datepicker .ui-datepicker-header{position:relative;padding:.2em 0}.ui-datepicker .ui-datepicker-prev,.ui-datepicker .ui-datepicker-next{position:absolute;top:2px;width:1.8em;height:1.8em}.ui-datepicker .ui-datepicker-prev-hover,.ui-datepicker .ui-datepicker-next-hover{top:1px}.ui-datepicker .ui-datepicker-prev{left:2px}.ui-datepicker .ui-datepicker-next{right:2px}.ui-datepicker .ui-datepicker-prev-hover{left:1px}.ui-datepicker .ui-datepicker-next-hover{right:1px}.ui-datepicker .ui-datepicker-prev span,.ui-datepicker .ui-datepicker-next span{display:block;position:absolute;left:50%;margin-left:-8px;top:50%;margin-top:-8px}.ui-datepicker .ui-datepicker-title{margin:0 2.3em;line-height:1.8em;text-align:center}.ui-datepicker .ui-datepicker-title select{font-size:1em;margin:1px 0}.ui-datepicker select.ui-datepicker-month,.ui-datepicker select.ui-datepicker-year{width:45%}.ui-datepicker table{width:100%;font-size:.9em;border-collapse:collapse;margin:0 0 .4em}.ui-datepicker th{padding:.7em .3em;text-align:center;font-weight:bold;border:0}.ui-datepicker td{border:0;padding:1px}.ui-datepicker td span,.ui-datepicker td a{display:block;padding:.2em;text-align:right;text-decoration:none}.ui-datepicker .ui-datepicker-buttonpane{background-image:none;margin:.7em 0 0 0;padding:0 .2em;border-left:0;border-right:0;border-bottom:0}.ui-datepicker .ui-datepicker-buttonpane button{float:right;margin:.5em .2em .4em;cursor:pointer;padding:.2em .6em .3em .6em;width:auto;overflow:visible}.ui-datepicker .ui-datepicker-buttonpane button.ui-datepicker-current{float:left}.ui-datepicker.ui-datepicker-multi{width:auto}.ui-datepicker-multi .ui-datepicker-group{float:left}.ui-datepicker-multi .ui-datepicker-group table{width:95%;margin:0 auto .4em}.ui-datepicker-multi-2 .ui-datepicker-group{width:50%}.ui-datepicker-multi-3 .ui-datepicker-group{width:33.3%}.ui-datepicker-multi-4 .ui-datepicker-group{width:25%}.ui-datepicker-multi .ui-datepicker-group-last .ui-datepicker-header,.ui-datepicker-multi .ui-datepicker-group-middle .ui-datepicker-header{border-left-width:0}.ui-datepicker-multi .ui-datepicker-buttonpane{clear:left}.ui-datepicker-row-break{clear:both;width:100%;font-size:0}.ui-datepicker-rtl{direction:rtl}.ui-datepicker-rtl .ui-datepicker-prev{right:2px;left:auto}.ui-datepicker-rtl .ui-datepicker-next{left:2px;right:auto}.ui-datepicker-rtl .ui-datepicker-prev:hover{right:1px;left:auto}.ui-datepicker-rtl .ui-datepicker-next:hover{left:1px;right:auto}.ui-datepicker-rtl .ui-datepicker-buttonpane{clear:right}.ui-datepicker-rtl .ui-datepicker-buttonpane button{float:left}.ui-datepicker-rtl .ui-datepicker-buttonpane button.ui-datepicker-current,.ui-datepicker-rtl .ui-datepicker-group{float:right}.ui-datepicker-rtl .ui-datepicker-group-last .ui-datepicker-header,.ui-datepicker-rtl .ui-datepicker-group-middle .ui-datepicker-header{border-right-width:0;border-left-width:1px}.ui-datepicker .ui-icon{display:block;text-indent:-99999px;overflow:hidden;background-repeat:no-repeat;left:.5em;top:.3em}.ui-dialog{position:absolute;top:0;left:0;padding:.2em;outline:0}.ui-dialog .ui-dialog-titlebar{padding:.4em 1em;position:relative}.ui-dialog .ui-dialog-title{float:left;margin:.1em 0;white-space:nowrap;width:90%;overflow:hidden;text-overflow:ellipsis}.ui-dialog .ui-dialog-titlebar-close{position:absolute;right:.3em;top:50%;width:20px;margin:-10px 0 0 0;padding:1px;height:20px}.ui-dialog .ui-dialog-content{position:relative;border:0;padding:.5em 1em;background:none;overflow:auto}.ui-dialog .ui-dialog-buttonpane{text-align:left;border-width:1px 0 0 0;background-image:none;margin-top:.5em;padding:.3em 1em .5em .4em}.ui-dialog .ui-dialog-buttonpane .ui-dialog-buttonset{float:right}.ui-dialog .ui-dialog-buttonpane button{margin:.5em .4em .5em 0;cursor:pointer}.ui-dialog .ui-resizable-n{height:2px;top:0}.ui-dialog .ui-resizable-e{width:2px;right:0}.ui-dialog .ui-resizable-s{height:2px;bottom:0}.ui-dialog .ui-resizable-w{width:2px;left:0}.ui-dialog .ui-resizable-se,.ui-dialog .ui-resizable-sw,.ui-dialog .ui-resizable-ne,.ui-dialog .ui-resizable-nw{width:7px;height:7px}.ui-dialog .ui-resizable-se{right:0;bottom:0}.ui-dialog .ui-resizable-sw{left:0;bottom:0}.ui-dialog .ui-resizable-ne{right:0;top:0}.ui-dialog .ui-resizable-nw{left:0;top:0}.ui-draggable .ui-dialog-titlebar{cursor:move}.ui-progressbar{height:2em;text-align:left;overflow:hidden}.ui-progressbar .ui-progressbar-value{margin:-1px;height:100%}.ui-progressbar .ui-progressbar-overlay{background:url("data:image/gif;base64,R0lGODlhKAAoAIABAAAAAP///yH/C05FVFNDQVBFMi4wAwEAAAAh+QQJAQABACwAAAAAKAAoAAACkYwNqXrdC52DS06a7MFZI+4FHBCKoDeWKXqymPqGqxvJrXZbMx7Ttc+w9XgU2FB3lOyQRWET2IFGiU9m1frDVpxZZc6bfHwv4c1YXP6k1Vdy292Fb6UkuvFtXpvWSzA+HycXJHUXiGYIiMg2R6W459gnWGfHNdjIqDWVqemH2ekpObkpOlppWUqZiqr6edqqWQAAIfkECQEAAQAsAAAAACgAKAAAApSMgZnGfaqcg1E2uuzDmmHUBR8Qil95hiPKqWn3aqtLsS18y7G1SzNeowWBENtQd+T1JktP05nzPTdJZlR6vUxNWWjV+vUWhWNkWFwxl9VpZRedYcflIOLafaa28XdsH/ynlcc1uPVDZxQIR0K25+cICCmoqCe5mGhZOfeYSUh5yJcJyrkZWWpaR8doJ2o4NYq62lAAACH5BAkBAAEALAAAAAAoACgAAAKVDI4Yy22ZnINRNqosw0Bv7i1gyHUkFj7oSaWlu3ovC8GxNso5fluz3qLVhBVeT/Lz7ZTHyxL5dDalQWPVOsQWtRnuwXaFTj9jVVh8pma9JjZ4zYSj5ZOyma7uuolffh+IR5aW97cHuBUXKGKXlKjn+DiHWMcYJah4N0lYCMlJOXipGRr5qdgoSTrqWSq6WFl2ypoaUAAAIfkECQEAAQAsAAAAACgAKAAAApaEb6HLgd/iO7FNWtcFWe+ufODGjRfoiJ2akShbueb0wtI50zm02pbvwfWEMWBQ1zKGlLIhskiEPm9R6vRXxV4ZzWT2yHOGpWMyorblKlNp8HmHEb/lCXjcW7bmtXP8Xt229OVWR1fod2eWqNfHuMjXCPkIGNileOiImVmCOEmoSfn3yXlJWmoHGhqp6ilYuWYpmTqKUgAAIfkECQEAAQAsAAAAACgAKAAAApiEH6kb58biQ3FNWtMFWW3eNVcojuFGfqnZqSebuS06w5V80/X02pKe8zFwP6EFWOT1lDFk8rGERh1TTNOocQ61Hm4Xm2VexUHpzjymViHrFbiELsefVrn6XKfnt2Q9G/+Xdie499XHd2g4h7ioOGhXGJboGAnXSBnoBwKYyfioubZJ2Hn0RuRZaflZOil56Zp6iioKSXpUAAAh+QQJAQABACwAAAAAKAAoAAACkoQRqRvnxuI7kU1a1UU5bd5tnSeOZXhmn5lWK3qNTWvRdQxP8qvaC+/yaYQzXO7BMvaUEmJRd3TsiMAgswmNYrSgZdYrTX6tSHGZO73ezuAw2uxuQ+BbeZfMxsexY35+/Qe4J1inV0g4x3WHuMhIl2jXOKT2Q+VU5fgoSUI52VfZyfkJGkha6jmY+aaYdirq+lQAACH5BAkBAAEALAAAAAAoACgAAAKWBIKpYe0L3YNKToqswUlvznigd4wiR4KhZrKt9Upqip61i9E3vMvxRdHlbEFiEXfk9YARYxOZZD6VQ2pUunBmtRXo1Lf8hMVVcNl8JafV38aM2/Fu5V16Bn63r6xt97j09+MXSFi4BniGFae3hzbH9+hYBzkpuUh5aZmHuanZOZgIuvbGiNeomCnaxxap2upaCZsq+1kAACH5BAkBAAEALAAAAAAoACgAAAKXjI8By5zf4kOxTVrXNVlv1X0d8IGZGKLnNpYtm8Lr9cqVeuOSvfOW79D9aDHizNhDJidFZhNydEahOaDH6nomtJjp1tutKoNWkvA6JqfRVLHU/QUfau9l2x7G54d1fl995xcIGAdXqMfBNadoYrhH+Mg2KBlpVpbluCiXmMnZ2Sh4GBqJ+ckIOqqJ6LmKSllZmsoq6wpQAAAh+QQJAQABACwAAAAAKAAoAAAClYx/oLvoxuJDkU1a1YUZbJ59nSd2ZXhWqbRa2/gF8Gu2DY3iqs7yrq+xBYEkYvFSM8aSSObE+ZgRl1BHFZNr7pRCavZ5BW2142hY3AN/zWtsmf12p9XxxFl2lpLn1rseztfXZjdIWIf2s5dItwjYKBgo9yg5pHgzJXTEeGlZuenpyPmpGQoKOWkYmSpaSnqKileI2FAAACH5BAkBAAEALAAAAAAoACgAAAKVjB+gu+jG4kORTVrVhRlsnn2dJ3ZleFaptFrb+CXmO9OozeL5VfP99HvAWhpiUdcwkpBH3825AwYdU8xTqlLGhtCosArKMpvfa1mMRae9VvWZfeB2XfPkeLmm18lUcBj+p5dnN8jXZ3YIGEhYuOUn45aoCDkp16hl5IjYJvjWKcnoGQpqyPlpOhr3aElaqrq56Bq7VAAAOw==");height:100%;-ms-filter:"alpha(opacity=25)";opacity:0.25}.ui-progressbar-indeterminate .ui-progressbar-value{background-image:none}.ui-selectmenu-menu{padding:0;margin:0;position:absolute;top:0;left:0;display:none}.ui-selectmenu-menu .ui-menu{overflow:auto;overflow-x:hidden;padding-bottom:1px}.ui-selectmenu-menu .ui-menu .ui-selectmenu-optgroup{font-size:1em;font-weight:bold;line-height:1.5;padding:2px 0.4em;margin:0.5em 0 0 0;height:auto;border:0}.ui-selectmenu-open{display:block}.ui-selectmenu-text{display:block;margin-right:20px;overflow:hidden;text-overflow:ellipsis}.ui-selectmenu-button.ui-button{text-align:left;white-space:nowrap;width:14em}.ui-selectmenu-icon.ui-icon{float:right;margin-top:0}.ui-slider{position:relative;text-align:left}.ui-slider .ui-slider-handle{position:absolute;z-index:2;width:1.2em;height:1.2em;cursor:pointer;-ms-touch-action:none;touch-action:none}.ui-slider .ui-slider-range{position:absolute;z-index:1;font-size:.7em;display:block;border:0;background-position:0 0}.ui-slider.ui-state-disabled .ui-slider-handle,.ui-slider.ui-state-disabled .ui-slider-range{filter:inherit}.ui-slider-horizontal{height:.8em}.ui-slider-horizontal .ui-slider-handle{top:-.3em;margin-left:-.6em}.ui-slider-horizontal .ui-slider-range{top:0;height:100%}.ui-slider-horizontal .ui-slider-range-min{left:0}.ui-slider-horizontal .ui-slider-range-max{right:0}.ui-slider-vertical{width:.8em;height:100px}.ui-slider-vertical .ui-slider-handle{left:-.3em;margin-left:0;margin-bottom:-.6em}.ui-slider-vertical .ui-slider-range{left:0;width:100%}.ui-slider-vertical .ui-slider-range-min{bottom:0}.ui-slider-vertical .ui-slider-range-max{top:0}.ui-spinner{position:relative;display:inline-block;overflow:hidden;padding:0;vertical-align:middle}.ui-spinner-input{border:none;background:none;color:inherit;padding:.222em 0;margin:.2em 0;vertical-align:middle;margin-left:.4em;margin-right:2em}.ui-spinner-button{width:1.6em;height:50%;font-size:.5em;padding:0;margin:0;text-align:center;position:absolute;cursor:default;display:block;overflow:hidden;right:0}.ui-spinner a.ui-spinner-button{border-top-style:none;border-bottom-style:none;border-right-style:none}.ui-spinner-up{top:0}.ui-spinner-down{bottom:0}.ui-tabs{position:relative;padding:.2em}.ui-tabs .ui-tabs-nav{margin:0;padding:.2em .2em 0}.ui-tabs .ui-tabs-nav li{list-style:none;float:left;position:relative;top:0;margin:1px .2em 0 0;border-bottom-width:0;padding:0;white-space:nowrap}.ui-tabs .ui-tabs-nav .ui-tabs-anchor{float:left;padding:.5em 1em;text-decoration:none}.ui-tabs .ui-tabs-nav li.ui-tabs-active{margin-bottom:-1px;padding-bottom:1px}.ui-tabs .ui-tabs-nav li.ui-tabs-active .ui-tabs-anchor,.ui-tabs .ui-tabs-nav li.ui-state-disabled .ui-tabs-anchor,.ui-tabs .ui-tabs-nav li.ui-tabs-loading .ui-tabs-anchor{cursor:text}.ui-tabs-collapsible .ui-tabs-nav li.ui-tabs-active .ui-tabs-anchor{cursor:pointer}.ui-tabs .ui-tabs-panel{display:block;border-width:0;padding:1em 1.4em;background:none}.ui-tooltip{padding:8px;position:absolute;z-index:9999;max-width:300px}body .ui-tooltip{border-width:2px}.ui-widget{font-family:Arial,Helvetica,sans-serif;font-size:1em}.ui-widget .ui-widget{font-size:1em}.ui-widget input,.ui-widget select,.ui-widget textarea,.ui-widget button{font-family:Arial,Helvetica,sans-serif;font-size:1em}.ui-widget.ui-widget-content{border:1px solid #c5c5c5}.ui-widget-content{border:1px solid #ddd;background:#fff;color:#333}.ui-widget-content a{color:#333}.ui-widget-header{border:1px solid #ddd;background:#e9e9e9;color:#333;font-weight:bold}.ui-widget-header a{color:#333}.ui-state-default,.ui-widget-content .ui-state-default,.ui-widget-header .ui-state-default,.ui-button,html .ui-button.ui-state-disabled:hover,html .ui-button.ui-state-disabled:active{border:1px solid #c5c5c5;background:#f6f6f6;font-weight:normal;color:#454545}.ui-state-default a,.ui-state-default a:link,.ui-state-default a:visited,a.ui-button,a:link.ui-button,a:visited.ui-button,.ui-button{color:#454545;text-decoration:none}.ui-state-hover,.ui-widget-content .ui-state-hover,.ui-widget-header .ui-state-hover,.ui-state-focus,.ui-widget-content .ui-state-focus,.ui-widget-header .ui-state-focus,.ui-button:hover,.ui-button:focus{border:1px solid #ccc;background:#ededed;font-weight:normal;color:#2b2b2b}.ui-state-hover a,.ui-state-hover a:hover,.ui-state-hover a:link,.ui-state-hover a:visited,.ui-state-focus a,.ui-state-focus a:hover,.ui-state-focus a:link,.ui-state-focus a:visited,a.ui-button:hover,a.ui-button:focus{color:#2b2b2b;text-decoration:none}.ui-visual-focus{box-shadow:0 0 3px 1px rgb(94,158,214)}.ui-state-active,.ui-widget-content .ui-state-active,.ui-widget-header .ui-state-active,a.ui-button:active,.ui-button:active,.ui-button.ui-state-active:hover{border:1px solid #003eff;background:#007fff;font-weight:normal;color:#fff}.ui-icon-background,.ui-state-active .ui-icon-background{border:#003eff;background-color:#fff}.ui-state-active a,.ui-state-active a:link,.ui-state-active a:visited{color:#fff;text-decoration:none}.ui-state-highlight,.ui-widget-content .ui-state-highlight,.ui-widget-header .ui-state-highlight{border:1px solid #dad55e;background:#fffa90;color:#777620}.ui-state-checked{border:1px solid #dad55e;background:#fffa90}.ui-state-highlight a,.ui-widget-content .ui-state-highlight a,.ui-widget-header .ui-state-highlight a{color:#777620}.ui-state-error,.ui-widget-content .ui-state-error,.ui-widget-header .ui-state-error{border:1px solid #f1a899;background:#fddfdf;color:#5f3f3f}.ui-state-error a,.ui-widget-content .ui-state-error a,.ui-widget-header .ui-state-error a{color:#5f3f3f}.ui-state-error-text,.ui-widget-content .ui-state-error-text,.ui-widget-header .ui-state-error-text{color:#5f3f3f}.ui-priority-primary,.ui-widget-content .ui-priority-primary,.ui-widget-header .ui-priority-primary{font-weight:bold}.ui-priority-secondary,.ui-widget-content .ui-priority-secondary,.ui-widget-header .ui-priority-secondary{opacity:.7;-ms-filter:"alpha(opacity=70)";font-weight:normal}.ui-state-disabled,.ui-widget-content .ui-state-disabled,.ui-widget-header .ui-state-disabled{opacity:.35;-ms-filter:"alpha(opacity=35)";background-image:none}.ui-state-disabled .ui-icon{-ms-filter:"alpha(opacity=35)"}.ui-icon{width:16px;height:16px}.ui-icon,.ui-widget-content .ui-icon{background-image:url("images/ui-icons_444444_256x240.png")}.ui-widget-header .ui-icon{background-image:url("images/ui-icons_444444_256x240.png")}.ui-state-hover .ui-icon,.ui-state-focus .ui-icon,.ui-button:hover .ui-icon,.ui-button:focus .ui-icon{background-image:url("images/ui-icons_555555_256x240.png")}.ui-state-active .ui-icon,.ui-button:active .ui-icon{background-image:url("images/ui-icons_ffffff_256x240.png")}.ui-state-highlight .ui-icon,.ui-button .ui-state-highlight.ui-icon{background-image:url("images/ui-icons_777620_256x240.png")}.ui-state-error .ui-icon,.ui-state-error-text .ui-icon{background-image:url("images/ui-icons_cc0000_256x240.png")}.ui-button .ui-icon{background-image:url("images/ui-icons_777777_256x240.png")}.ui-icon-blank.ui-icon-blank.ui-icon-blank{background-image:none}.ui-icon-caret-1-n{background-position:0 0}.ui-icon-caret-1-ne{background-position:-16px 0}.ui-icon-caret-1-e{background-position:-32px 0}.ui-icon-caret-1-se{background-position:-48px 0}.ui-icon-caret-1-s{background-position:-65px 0}.ui-icon-caret-1-sw{background-position:-80px 0}.ui-icon-caret-1-w{background-position:-96px 0}.ui-icon-caret-1-nw{background-position:-112px 0}.ui-icon-caret-2-n-s{background-position:-128px 0}.ui-icon-caret-2-e-w{background-position:-144px 0}.ui-icon-triangle-1-n{background-position:0 -16px}.ui-icon-triangle-1-ne{background-position:-16px -16px}.ui-icon-triangle-1-e{background-position:-32px -16px}.ui-icon-triangle-1-se{background-position:-48px -16px}.ui-icon-triangle-1-s{background-position:-65px -16px}.ui-icon-triangle-1-sw{background-position:-80px -16px}.ui-icon-triangle-1-w{background-position:-96px -16px}.ui-icon-triangle-1-nw{background-position:-112px -16px}.ui-icon-triangle-2-n-s{background-position:-128px -16px}.ui-icon-triangle-2-e-w{background-position:-144px -16px}.ui-icon-arrow-1-n{background-position:0 -32px}.ui-icon-arrow-1-ne{background-position:-16px -32px}.ui-icon-arrow-1-e{background-position:-32px -32px}.ui-icon-arrow-1-se{background-position:-48px -32px}.ui-icon-arrow-1-s{background-position:-65px -32px}.ui-icon-arrow-1-sw{background-position:-80px -32px}.ui-icon-arrow-1-w{background-position:-96px -32px}.ui-icon-arrow-1-nw{background-position:-112px -32px}.ui-icon-arrow-2-n-s{background-position:-128px -32px}.ui-icon-arrow-2-ne-sw{background-position:-144px -32px}.ui-icon-arrow-2-e-w{background-position:-160px -32px}.ui-icon-arrow-2-se-nw{background-position:-176px -32px}.ui-icon-arrowstop-1-n{background-position:-192px -32px}.ui-icon-arrowstop-1-e{background-position:-208px -32px}.ui-icon-arrowstop-1-s{background-position:-224px -32px}.ui-icon-arrowstop-1-w{background-position:-240px -32px}.ui-icon-arrowthick-1-n{background-position:1px -48px}.ui-icon-arrowthick-1-ne{background-position:-16px -48px}.ui-icon-arrowthick-1-e{background-position:-32px -48px}.ui-icon-arrowthick-1-se{background-position:-48px -48px}.ui-icon-arrowthick-1-s{background-position:-64px -48px}.ui-icon-arrowthick-1-sw{background-position:-80px -48px}.ui-icon-arrowthick-1-w{background-position:-96px -48px}.ui-icon-arrowthick-1-nw{background-position:-112px -48px}.ui-icon-arrowthick-2-n-s{background-position:-128px -48px}.ui-icon-arrowthick-2-ne-sw{background-position:-144px -48px}.ui-icon-arrowthick-2-e-w{background-position:-160px -48px}.ui-icon-arrowthick-2-se-nw{background-position:-176px -48px}.ui-icon-arrowthickstop-1-n{background-position:-192px -48px}.ui-icon-arrowthickstop-1-e{background-position:-208px -48px}.ui-icon-arrowthickstop-1-s{background-position:-224px -48px}.ui-icon-arrowthickstop-1-w{background-position:-240px -48px}.ui-icon-arrowreturnthick-1-w{background-position:0 -64px}.ui-icon-arrowreturnthick-1-n{background-position:-16px -64px}.ui-icon-arrowreturnthick-1-e{background-position:-32px -64px}.ui-icon-arrowreturnthick-1-s{background-position:-48px -64px}.ui-icon-arrowreturn-1-w{background-position:-64px -64px}.ui-icon-arrowreturn-1-n{background-position:-80px -64px}.ui-icon-arrowreturn-1-e{background-position:-96px -64px}.ui-icon-arrowreturn-1-s{background-position:-112px -64px}.ui-icon-arrowrefresh-1-w{background-position:-128px -64px}.ui-icon-arrowrefresh-1-n{background-position:-144px -64px}.ui-icon-arrowrefresh-1-e{background-position:-160px -64px}.ui-icon-arrowrefresh-1-s{background-position:-176px -64px}.ui-icon-arrow-4{background-position:0 -80px}.ui-icon-arrow-4-diag{background-position:-16px -80px}.ui-icon-extlink{background-position:-32px -80px}.ui-icon-newwin{background-position:-48px -80px}.ui-icon-refresh{background-position:-64px -80px}.ui-icon-shuffle{background-position:-80px -80px}.ui-icon-transfer-e-w{background-position:-96px -80px}.ui-icon-transferthick-e-w{background-position:-112px -80px}.ui-icon-folder-collapsed{background-position:0 -96px}.ui-icon-folder-open{background-position:-16px -96px}.ui-icon-document{background-position:-32px -96px}.ui-icon-document-b{background-position:-48px -96px}.ui-icon-note{background-position:-64px -96px}.ui-icon-mail-closed{background-position:-80px -96px}.ui-icon-mail-open{background-position:-96px -96px}.ui-icon-suitcase{background-position:-112px -96px}.ui-icon-comment{background-position:-128px -96px}.ui-icon-person{background-position:-144px -96px}.ui-icon-print{background-position:-160px -96px}.ui-icon-trash{background-position:-176px -96px}.ui-icon-locked{background-position:-192px -96px}.ui-icon-unlocked{background-position:-208px -96px}.ui-icon-bookmark{background-position:-224px -96px}.ui-icon-tag{background-position:-240px -96px}.ui-icon-home{background-position:0 -112px}.ui-icon-flag{background-position:-16px -112px}.ui-icon-calendar{background-position:-32px -112px}.ui-icon-cart{background-position:-48px -112px}.ui-icon-pencil{background-position:-64px -112px}.ui-icon-clock{background-position:-80px -112px}.ui-icon-disk{background-position:-96px -112px}.ui-icon-calculator{background-position:-112px -112px}.ui-icon-zoomin{background-position:-128px -112px}.ui-icon-zoomout{background-position:-144px -112px}.ui-icon-search{background-position:-160px -112px}.ui-icon-wrench{background-position:-176px -112px}.ui-icon-gear{background-position:-192px -112px}.ui-icon-heart{background-position:-208px -112px}.ui-icon-star{background-position:-224px -112px}.ui-icon-link{background-position:-240px -112px}.ui-icon-cancel{background-position:0 -128px}.ui-icon-plus{background-position:-16px -128px}.ui-icon-plusthick{background-position:-32px -128px}.ui-icon-minus{background-position:-48px -128px}.ui-icon-minusthick{background-position:-64px -128px}.ui-icon-close{background-position:-80px -128px}.ui-icon-closethick{background-position:-96px -128px}.ui-icon-key{background-position:-112px -128px}.ui-icon-lightbulb{background-position:-128px -128px}.ui-icon-scissors{background-position:-144px -128px}.ui-icon-clipboard{background-position:-160px -128px}.ui-icon-copy{background-position:-176px -128px}.ui-icon-contact{background-position:-192px -128px}.ui-icon-image{background-position:-208px -128px}.ui-icon-video{background-position:-224px -128px}.ui-icon-script{background-position:-240px -128px}.ui-icon-alert{background-position:0 -144px}.ui-icon-info{background-position:-16px -144px}.ui-icon-notice{background-position:-32px -144px}.ui-icon-help{background-position:-48px -144px}.ui-icon-check{background-position:-64px -144px}.ui-icon-bullet{background-position:-80px -144px}.ui-icon-radio-on{background-position:-96px -144px}.ui-icon-radio-off{background-position:-112px -144px}.ui-icon-pin-w{background-position:-128px -144px}.ui-icon-pin-s{background-position:-144px -144px}.ui-icon-play{background-position:0 -160px}.ui-icon-pause{background-position:-16px -160px}.ui-icon-seek-next{background-position:-32px -160px}.ui-icon-seek-prev{background-position:-48px -160px}.ui-icon-seek-end{background-position:-64px -160px}.ui-icon-seek-start{background-position:-80px -160px}.ui-icon-seek-first{background-position:-80px -160px}.ui-icon-stop{background-position:-96px -160px}.ui-icon-eject{background-position:-112px -160px}.ui-icon-volume-off{background-position:-128px -160px}.ui-icon-volume-on{background-position:-144px -160px}.ui-icon-power{background-position:0 -176px}.ui-icon-signal-diag{background-position:-16px -176px}.ui-icon-signal{background-position:-32px -176px}.ui-icon-battery-0{background-position:-48px -176px}.ui-icon-battery-1{background-position:-64px -176px}.ui-icon-battery-2{background-position:-80px -176px}.ui-icon-battery-3{background-position:-96px -176px}.ui-icon-circle-plus{background-position:0 -192px}.ui-icon-circle-minus{background-position:-16px -192px}.ui-icon-circle-close{background-position:-32px -192px}.ui-icon-circle-triangle-e{background-position:-48px -192px}.ui-icon-circle-triangle-s{background-position:-64px -192px}.ui-icon-circle-triangle-w{background-position:-80px -192px}.ui-icon-circle-triangle-n{background-position:-96px -192px}.ui-icon-circle-arrow-e{background-position:-112px -192px}.ui-icon-circle-arrow-s{background-position:-128px -192px}.ui-icon-circle-arrow-w{background-position:-144px -192px}.ui-icon-circle-arrow-n{background-position:-160px -192px}.ui-icon-circle-zoomin{background-position:-176px -192px}.ui-icon-circle-zoomout{background-position:-192px -192px}.ui-icon-circle-check{background-position:-208px -192px}.ui-icon-circlesmall-plus{background-position:0 -208px}.ui-icon-circlesmall-minus{background-position:-16px -208px}.ui-icon-circlesmall-close{background-position:-32px -208px}.ui-icon-squaresmall-plus{background-position:-48px -208px}.ui-icon-squaresmall-minus{background-position:-64px -208px}.ui-icon-squaresmall-close{background-position:-80px -208px}.ui-icon-grip-dotted-vertical{background-position:0 -224px}.ui-icon-grip-dotted-horizontal{background-position:-16px -224px}.ui-icon-grip-solid-vertical{background-position:-32px -224px}.ui-icon-grip-solid-horizontal{background-position:-48px -224px}.ui-icon-gripsmall-diagonal-se{background-position:-64px -224px}.ui-icon-grip-diagonal-se{background-position:-80px -224px}.ui-corner-all,.ui-corner-top,.ui-corner-left,.ui-corner-tl{border-top-left-radius:3px}.ui-corner-all,.ui-corner-top,.ui-corner-right,.ui-corner-tr{border-top-right-radius:3px}.ui-corner-all,.ui-corner-bottom,.ui-corner-left,.ui-corner-bl{border-bottom-left-radius:3px}.ui-corner-all,.ui-corner-bottom,.ui-corner-right,.ui-corner-br{border-bottom-right-radius:3px}.ui-widget-overlay{background:#aaa;opacity:.3;-ms-filter:Alpha(Opacity=30)}.ui-widget-shadow{-webkit-box-shadow:0 0 5px #666;box-shadow:0 0 5px #666}
```

### Comparing `django-content-blocks-1.2.1/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.js` & `django-content-blocks-1.3.0/content_blocks/static/content_blocks/jqueryui/jquery-ui.min.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, Unicode text, UTF-8 text, with very long lines (64399)*

 * *Files 0% similar despite different names*

```diff
@@ -15936,8 +15936,8 @@
 0003e3f0: 6173 696e 673a 742e 6561 7369 6e67 2c63  asing:t.easing,c
 0003e400: 6f6d 706c 6574 653a 657d 297d 292c 2131  omplete:e})}),!1
 0003e410: 213d 3d56 2e75 6942 6163 6b43 6f6d 7061  !==V.uiBackCompa
 0003e420: 7426 2656 2e65 6666 6563 7473 2e64 6566  t&&V.effects.def
 0003e430: 696e 6528 2274 7261 6e73 6665 7222 2c66  ine("transfer",f
 0003e440: 756e 6374 696f 6e28 742c 6529 7b56 2874  unction(t,e){V(t
 0003e450: 6869 7329 2e74 7261 6e73 6665 7228 742c  his).transfer(t,
-0003e460: 6529 7d29 7d29 3b                        e)})});
+0003e460: 6529 7d29 7d29 3b0a                      e)})});.
```

### Comparing `django-content-blocks-1.2.1/content_blocks/static/content_blocks/js/admin_choices_widget.js` & `django-content-blocks-1.3.0/content_blocks/static/content_blocks/js/admin_choices_widget.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-window.addEventListener("load", function() {
+window.addEventListener('load', function() {
     let $ = django.jQuery;
     // CHOICES WIDGET //
     let $row = $('.input-row').first();
 
     $('.choices-widget').each(function() {
         loadChoices($(this));
     });
@@ -22,20 +22,20 @@
 
     $(document).on('change', '.choices-widget .input-row input', function() {
         let $choices_widget = $(this).closest('.choices-widget');
         saveChoices($choices_widget);
     });
 
     function loadChoices($choices_widget) {
-        let $input = $choices_widget.find("input[type=hidden]");
+        let $input = $choices_widget.find('input[type=hidden]');
         let choices = $input.val();
 
-        if (!choices || choices === "[]") return;
+        if (!choices || choices === '[]') return;
 
-        $choices_widget.find(".input-row").remove();
+        $choices_widget.find('.input-row').remove();
 
         choices = JSON.parse(choices);
 
         $.each(choices, function() {
             addRow($choices_widget, this);
         });
     }
@@ -53,23 +53,23 @@
             if (!val_1 || !val_2) return;
 
             choices.push([val_1, val_2]);
         });
 
         choices = JSON.stringify(choices);
 
-        $choices_widget.find("input[type=hidden]").val(choices);
+        $choices_widget.find('input[type=hidden]').val(choices);
     }
 
     function addRow($choices_widget, values) {
         if (values === undefined) {
-            values = ["", ""]
+            values = ['', ''];
         }
 
         let $new_row = $row.clone();
-        $new_row.find("input").each(function(i) {
+        $new_row.find('input').each(function(i) {
             $(this).val(values[i]);
         });
 
-        $choices_widget.find(".inputs").append($new_row);
+        $choices_widget.find('.inputs').append($new_row);
     }
 });
```

### Comparing `django-content-blocks-1.2.1/content_blocks/static/content_blocks/js/ajax_setup.js` & `django-content-blocks-1.3.0/content_blocks/static/content_blocks/js/ajax_setup.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -2,32 +2,32 @@
 function getCookie(name) {
     let cookieValue = null;
     if (document.cookie && document.cookie !== '') {
         let cookies = document.cookie.split(';');
         for (let i = 0; i < cookies.length; i++) {
             let cookie = jQuery.trim(cookies[i]);
             // Does this cookie string begin with the name we want?
-            if (cookie.substring(0, name.length + 1) === (name + '=')) {
+            if (cookie.substring(0, name.length + 1) === name + '=') {
                 cookieValue = decodeURIComponent(cookie.substring(name.length + 1));
                 break;
             }
         }
     }
     return cookieValue;
 }
 
 let csrftoken = getCookie('csrftoken');
 
 //  Setup AJAX to send CSRF token as standard on POST
 function csrfSafeMethod(method) {
     // these HTTP methods do not require CSRF protection
-    return (/^(GET|HEAD|OPTIONS|TRACE)$/.test(method));
+    return /^(GET|HEAD|OPTIONS|TRACE)$/.test(method);
 }
 
 $.ajaxSetup({
     beforeSend: function(xhr, settings) {
         if (!csrfSafeMethod(settings.type) && !this.crossDomain) {
-            xhr.setRequestHeader("X-CSRFToken", csrftoken);
+            xhr.setRequestHeader('X-CSRFToken', csrftoken);
         }
     },
-    dataType: "json"
+    dataType: 'json',
 });
```

### Comparing `django-content-blocks-1.2.1/content_blocks/static/content_blocks/js/content_block_editor.js` & `django-content-blocks-1.3.0/content_blocks/static/content_blocks/js/content_block_editor.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 (function($) {
     $.fn.ContentBlockEditor = function(options) {
         let settings = $.extend({}, options);
 
-        const delete_active_class = "fa-trash";
-        const delete_disabled_class = "fa-trash-slash";
+        const delete_active_class = 'fa-trash';
+        const delete_disabled_class = 'fa-trash-slash';
 
         $(document).ajaxError(function(e, j, s, thrownError) {
             showStatus('Something went wrong. Please reload the page and try again.');
             console.log(thrownError);
         });
 
         // Initialise dragon drops.
@@ -34,15 +34,15 @@
             let title = $form.find('#cb_import_label').html();
             showStatus('Importing content blocks from ' + title);
             $form.ajaxSubmit({
                 success: function(data) {
                     renderAjaxResponse(data, $target, true);
                     hideLoader($loader);
                     showStatus('Content blocks imported from ' + title);
-                }
+                },
             });
 
             return false;
         });
 
         // Create button and select
         let $cb_template_select = $('#new_cb_content_block_template');
@@ -63,50 +63,53 @@
             let title = $form.find('#cb_create_label').html();
             showStatus('Creating ' + title);
 
             $form.ajaxSubmit({
                 success: function(data) {
                     renderAjaxResponse(data, $target, true);
                     showStatus(title + ' created');
-                }
+                },
             });
 
             return false;
         });
 
         // Create nested buttons and select
-        $(".nested-create-form").each(function() {
-            updateButtonLabel($(this).children("select"), $(this).find(".nested-create-label"));
+        $('.nested-create-form').each(function() {
+            updateButtonLabel(
+                $(this).children('select'),
+                $(this).find('.nested-create-label'),
+            );
         });
 
         $(document).on('change', '.nested-create-form select', function() {
             updateButtonLabel($(this), $(this).parent().find('.nested-create-label'));
         });
 
         $(document).on('submit', '.nested-create-form', function() {
             let $form = $(this);
 
-            if ($form.hasClass("disabled")) {
+            if ($form.hasClass('disabled')) {
                 return false;
             }
 
             let $target = $($form.data('target'));
             let $position = $form.find('input[name="position"]');
 
-            $position.val($target.children('.content-block-form').length)
+            $position.val($target.children('.content-block-form').length);
 
             let title = $form.find('.nested-create-label').html();
             showStatus('Creating ' + title);
 
             $form.ajaxSubmit({
                 success: function(data) {
                     renderAjaxResponse(data, $target, true);
                     enforceLimits($target);
                     showStatus(title + ' created');
-                }
+                },
             });
             return false;
         });
 
         // Content block save button
         $(document).on('click', 'button.save', function() {
             let $btn = $(this);
@@ -128,16 +131,16 @@
                     if (data.visible) {
                         $icon.addClass('fa-eye');
                         showStatus(label + ' shown');
                     } else {
                         $icon.addClass('fa-eye-slash');
                         showStatus(label + 'hidden');
                     }
-                }
-            })
+                },
+            });
         });
 
         // Preview button
         $(document).on('click', 'button.preview', function(e) {
             let $btn = $(this);
             let $target = $($btn.data('target'));
 
@@ -149,15 +152,15 @@
                 });
             }
         });
 
         // Delete button
         $(document).on('click', 'button.delete', function() {
             let $btn = $(this);
-            if ($btn.children("i").hasClass(delete_disabled_class)) {
+            if ($btn.children('i').hasClass(delete_disabled_class)) {
                 return false;
             }
 
             let $target = $($btn.data('target'));
             let $loader = $($btn.data('loader'));
             let ajax_url = $btn.data('ajax_url');
 
@@ -175,29 +178,29 @@
                         url: ajax_url,
                         type: 'POST',
                         dataType: 'json',
                         success: function(data) {
                             if (data.error) {
                                 console.log(data.error);
                             } else {
-                                let $wrapper = $target.closest(".content-blocks");
+                                let $wrapper = $target.closest('.content-blocks');
                                 $target.remove();
 
                                 $('.content-blocks').sortable('refresh');
                                 let positions = $wrapper.sortable('serialize');
                                 ajaxDragonDrop(positions);
                                 refreshDragonDrop();
 
                                 enforceLimits($wrapper);
                                 toggleImportForm();
                                 showStatus(label + ' deleted');
                             }
-                        }
+                        },
                     });
-                }
+                },
             });
         });
 
         const expand_open_class = 'fa-chevron-up';
         const expand_closed_class = 'fa-chevron-down';
 
         // Expander button
@@ -222,15 +225,16 @@
             }
         });
 
         // Collapse all button
         $(document).on('click', '.collapse-all', function() {
             let $target = $($(this).data('target'));
             $target.css('overflow', 'hidden');
-            $target.children('.content-block-form')
+            $target
+                .children('.content-block-form')
                 .children('.pos-rel')
                 .children('.controls')
                 .children('button.expand')
                 .each(function() {
                     let $button = $(this);
                     let $icon = $button.children('i');
                     let $expanders = $($button.data('target'));
@@ -241,15 +245,16 @@
                 });
         });
 
         // Expand all button
         $(document).on('click', '.expand-all', function() {
             let $target = $($(this).data('target'));
             $target.css('overflow', 'hidden');
-            $target.children('.content-block-form')
+            $target
+                .children('.content-block-form')
                 .children('.pos-rel')
                 .children('.controls')
                 .children('button.expand')
                 .each(function() {
                     let $button = $(this);
                     let $icon = $button.children('i');
                     let $expanders = $($button.data('target'));
@@ -284,25 +289,25 @@
 
         // Publish button
         $(document).on('submit', '#publish_form', function() {
             let $form = $(this);
             let $loader = $($(this).data('loader'));
 
             saveAll($loader, function() {
-                showStatus('Publishing content blocks')
+                showStatus('Publishing content blocks');
                 $form.ajaxSubmit({
                     success: function(data) {
                         hideLoader($loader);
-                        showStatus('Content blocks published')
-                    }
+                        showStatus('Content blocks published');
+                    },
                 });
             });
 
             return false;
-        })
+        });
 
         // Discard changes button
         $(document).on('submit', '#discard_form', function(e) {
             e.preventDefault();
             let $btn = $(this);
             showPopup($btn, {
                 css_class: 'small',
@@ -316,23 +321,22 @@
                     $btn.ajaxSubmit({
                         success: function(data) {
                             $('.content-block-form').remove();
                             renderAjaxResponse(data, $target, true);
                             toggleImportForm();
                             hideLoader($loader);
                             showStatus('Content blocks reset');
-                        }
+                        },
                     });
-                }
+                },
             });
 
             return false;
         });
 
-
         // Functions
         function renderAjaxResponse(data, $target, append = false, callback) {
             // Handle ajax which returns html
             if (data.error) {
                 console.log(data.error);
                 return;
             }
@@ -363,32 +367,34 @@
             $form.ajaxSubmit({
                 success: function(data) {
                     setSaveState($btn, data.saved);
                     renderAjaxResponse(data, $target);
                     hideLoader($loader);
 
                     if (data.saved) {
-                        showStatus(title + ' saved')
+                        showStatus(title + ' saved');
                     } else {
-                        showStatus('Please correct the errors')
+                        showStatus('Please correct the errors');
                     }
 
                     if (saved_callback && data.saved) {
                         return saved_callback();
                     }
                 },
                 uploadProgress: function(event, position, total, percentComplete) {
                     $loader.find('.progress-bar').width(percentComplete + '%');
                 },
             });
         }
 
         function updateButtonLabel($cb_type_select, $cb_create_button_label) {
             // Update the text in the create content block form submit button to match the selected content block type
-            $cb_create_button_label.html($cb_type_select.children('option:selected').text());
+            $cb_create_button_label.html(
+                $cb_type_select.children('option:selected').text(),
+            );
         }
 
         function saveAll($loader, callback) {
             // Save all unsaved content blocks sequentially.
             if (saving_all) {
                 return;
             }
@@ -399,15 +405,18 @@
             expandAll();
             let $buttons = $('button.save').not('.saved');
             return saveNext($buttons, callback, $loader);
         }
 
         function saveForPreview($btn, callback) {
             // Save unsaved content blocks and nested blocks for preview
-            let $buttons = $btn.closest('.content-block-form').find('button.save').not('.saved');
+            let $buttons = $btn
+                .closest('.content-block-form')
+                .find('button.save')
+                .not('.saved');
             return saveNext($buttons, callback);
         }
 
         function saveNext($buttons, callback, $loader, buttons) {
             // Used by save all to save sequentially then call callback if all saved OK or scroll to errors.
             let scroll_offset = 30;
 
@@ -415,16 +424,18 @@
 
             if (!buttons.length) {
                 // Finished saving everything
                 saving_all = false;
                 let $unsaved = $buttons.not('.saved');
                 if ($unsaved.length) {
                     $('html').animate({
-                        scrollTop: $unsaved.first().offset().top - scroll_offset
-                    }, 220);
+                            scrollTop: $unsaved.first().offset().top - scroll_offset
+                        },
+                        220,
+                    );
                     showStatus('Please correct the errors');
                 } else {
                     showStatus('All content blocks saved');
                     if (callback) {
                         return callback();
                     }
                 }
@@ -499,58 +510,70 @@
             // Make the loader visible to the user
             $loader.find('.progress-bar').width('0%');
             $loader.children('.bg').show();
         }
 
         function enforceLimits($content_block_wrapper) {
             // Disable delete and add nested block buttons in the wrapper based on min_num and max_num
-            let min_num = $content_block_wrapper.data("min_num");
-            let max_num = $content_block_wrapper.data("max_num");
-
-            let num_blocks = $content_block_wrapper.children(".content-block-form").length;
+            let min_num = $content_block_wrapper.data('min_num');
+            let max_num = $content_block_wrapper.data('max_num');
 
-            let delete_buttons = $content_block_wrapper.children(".content-block-form").find("button.delete");
+            let num_blocks = $content_block_wrapper.children(
+                '.content-block-form',
+            ).length;
+
+            let delete_buttons = $content_block_wrapper
+                .children('.content-block-form')
+                .find('button.delete');
             if (num_blocks <= min_num) {
                 // Min num reached so disabled delete button.
-                delete_buttons.children("i").removeClass(delete_active_class).addClass(delete_disabled_class);
+                delete_buttons
+                    .children('i')
+                    .removeClass(delete_active_class)
+                    .addClass(delete_disabled_class);
             } else {
-                delete_buttons.children("i").removeClass(delete_disabled_class).addClass(delete_active_class);
+                delete_buttons
+                    .children('i')
+                    .removeClass(delete_disabled_class)
+                    .addClass(delete_active_class);
             }
 
-            let nested_form = $content_block_wrapper.siblings(".cb-nested-create-form").children(".nested-create-form");
+            let nested_form = $content_block_wrapper
+                .siblings('.cb-nested-create-form')
+                .children('.nested-create-form');
             if (num_blocks >= max_num) {
                 // Max num reached so disable nested form.
-                nested_form.addClass("disabled");
+                nested_form.addClass('disabled');
             } else {
-                nested_form.removeClass("disabled");
+                nested_form.removeClass('disabled');
             }
         }
 
         function dragonDrop($content_block) {
             // Make a group of content blocks dragon sortable with jquery ui sortable.
             $content_block.sortable({
                 axis: 'y',
                 handle: '.move',
                 cancel: '',
                 containment: $content_block,
                 update: function(event, ui) {
                     let positions = $(this).sortable('serialize');
                     ajaxDragonDrop(positions);
-                }
+                },
             });
         }
 
         function ajaxDragonDrop(positions) {
             // Post to updated positions in db.
             $.ajax({
                 data: {
                     positions: positions
                 },
                 type: 'POST',
-                url: settings.update_position_url
+                url: settings.update_position_url,
             });
         }
 
         function refreshDragonDrop() {
             // Refresh dragon drops and create new for new content blocks.
             let $content_blocks = $('.content-blocks');
             $content_blocks.not('.ui-sortable').each(function() {
@@ -558,19 +581,21 @@
             });
             $content_blocks.sortable('refresh');
         }
 
         function expandAll() {
             // Opens all expanders
             $('.expander').slideDown();
-            $('.' + expand_closed_class).removeClass(expand_closed_class).addClass(expand_open_class);
+            $('.' + expand_closed_class)
+                .removeClass(expand_closed_class)
+                .addClass(expand_open_class);
         }
 
-        const saved_class = 'fa-floppy-disk'
-        const unsaved_class = 'fa-floppy-disk-circle-xmark'
+        const saved_class = 'fa-floppy-disk';
+        const unsaved_class = 'fa-floppy-disk-circle-xmark';
 
         function setSaveState($btn, saved) {
             // Update the save state of the save button and change the icon.
             $btn.removeClass('saved');
 
             let $icon = $btn.children('i');
             $icon.removeClass(saved_class + ' ' + unsaved_class);
@@ -583,22 +608,24 @@
         }
 
         function loadPreview($btn) {
             // Render a content block and get the html via ajax
             let $target = $($btn.data('target'));
             let $iframe = $target.children('iframe');
 
-            $iframe.iFrameResize({
-                checkOrigin: false
-            }).on('load', function() {
-                $target.slideDown().addClass('open');
-                $iframe.off('load');
-            });
+            $iframe
+                .iFrameResize({
+                    checkOrigin: false,
+                })
+                .on('load', function() {
+                    $target.slideDown().addClass('open');
+                    $iframe.off('load');
+                });
 
-            $iframe.attr("src", $iframe.data("src"));
+            $iframe.attr('src', $iframe.data('src'));
         }
 
         function toggleImportForm() {
             let $cb_import_form = $('.cb-import-form');
             if ($('.content-block-form').length) {
                 $cb_import_form.hide();
             } else {
@@ -609,21 +636,21 @@
         let $status_bar = $('div.status');
         let status_off = $status_bar.html();
         let $status_timer;
 
         function renderStatus(status) {
             $status_bar.fadeOut(function() {
                 $(this).html(status).fadeIn();
-            })
+            });
         }
 
         function showStatus(status) {
             clearTimeout($status_timer);
             renderStatus(status);
             $status_timer = setTimeout(function() {
                 renderStatus(status_off);
             }, 5500);
         }
 
         return this;
     };
-}(jQuery));
+})(jQuery);
```

### Comparing `django-content-blocks-1.2.1/content_blocks/static/content_blocks/js/content_block_template_admin.js` & `django-content-blocks-1.3.0/content_blocks/static/content_blocks/js/content_block_template_admin.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -1,52 +1,52 @@
 // Wait for Django jQuery to load, so we can use it.
-window.addEventListener("load", function() {
+window.addEventListener('load', function() {
     let $ = django.jQuery;
 
     const FIELD_TYPES = {
-        NESTED_FIELD: "NestedField",
-        CHECKBOX_FIELD: "CheckboxField",
-        CHOICE_FIELD: "ChoiceField",
-        MODEL_CHOICE_FIELD: "ModelChoiceField",
-        CONTENT_FIELD: "ContentField",
+        NESTED_FIELD: 'NestedField',
+        CHECKBOX_FIELD: 'CheckboxField',
+        CHOICE_FIELD: 'ChoiceField',
+        MODEL_CHOICE_FIELD: 'ModelChoiceField',
+        CONTENT_FIELD: 'ContentField',
     };
 
     const FIELDS = {
-        MODEL_CHOICE_CONTENT_TYPE: ".field-model_choice_content_type",
-        NESTED_TEMPLATE: ".field-nested_templates",
-        CHOICES: ".field-choices",
-        REQUIRED: ".field-required",
-        HELP_TEXT: ".field-help_text",
-        CSS_CLASS: ".field-css_class",
-        MIN_NUM: ".field-min_num",
-        MAX_NUM: ".field-max_num"
-    }
+        MODEL_CHOICE_CONTENT_TYPE: '.field-model_choice_content_type',
+        NESTED_TEMPLATE: '.field-nested_templates',
+        CHOICES: '.field-choices',
+        REQUIRED: '.field-required',
+        HELP_TEXT: '.field-help_text',
+        CSS_CLASS: '.field-css_class',
+        MIN_NUM: '.field-min_num',
+        MAX_NUM: '.field-max_num',
+    };
 
     const ALWAYS_HIDE = [
         FIELDS.MODEL_CHOICE_CONTENT_TYPE,
         FIELDS.NESTED_TEMPLATE,
         FIELDS.CHOICES,
         FIELDS.MIN_NUM,
-        FIELDS.MAX_NUM
+        FIELDS.MAX_NUM,
     ];
     const ALWAYS_SHOW = [FIELDS.REQUIRED, FIELDS.HELP_TEXT, FIELDS.CSS_CLASS];
 
     let options = {};
     options[FIELD_TYPES.NESTED_FIELD] = {
         show: [FIELDS.NESTED_TEMPLATE, FIELDS.MIN_NUM, FIELDS.MAX_NUM],
-        hide: [FIELDS.REQUIRED, FIELDS.HELP_TEXT]
+        hide: [FIELDS.REQUIRED],
     };
     options[FIELD_TYPES.CHECKBOX_FIELD] = {
         hide: [FIELDS.REQUIRED]
     };
     options[FIELD_TYPES.CHOICE_FIELD] = {
         show: [FIELDS.CHOICES]
     };
     options[FIELD_TYPES.MODEL_CHOICE_FIELD] = {
-        show: [FIELDS.MODEL_CHOICE_CONTENT_TYPE]
+        show: [FIELDS.MODEL_CHOICE_CONTENT_TYPE],
     };
 
     function showFields($field_type) {
         let $parent = $field_type.parents('.field-field_type');
         $parent.siblings(ALWAYS_HIDE.toString()).hide();
         $parent.siblings(ALWAYS_SHOW.toString()).show();
```

### Comparing `django-content-blocks-1.2.1/content_blocks/static/content_blocks/js/popup.js` & `django-content-blocks-1.3.0/content_blocks/static/content_blocks/js/popup.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -12,37 +12,41 @@
 });
 
 function showPopup(caller, kwargs) {
     let default_kwargs = {
         open_callback: undefined,
         confirm_callback: undefined,
         css_class: undefined,
-        content: undefined
-    }
+        content: undefined,
+    };
     kwargs = $.extend({}, default_kwargs, kwargs);
 
     if (open_popups.callers.includes(caller)) return false;
 
     disableScroll();
 
     let $popup = $popup_base.clone();
     $popup.attr('id', '');
     open_popups.popups.push($popup);
     open_popups.callers.push(caller);
 
-    $popup.on('click', function() {
-        hidePopup($popup);
-    }).on('click', '.confirm', function() {
-        hidePopup($popup);
-        if (kwargs.confirm_callback) kwargs.confirm_callback($popup);
-    }).on('click', '.close-popup', function() {
-        hidePopup($popup)
-    }).on('click', '.popup-wrapper', function(e) {
-        e.stopPropagation();
-    });
+    $popup
+        .on('click', function() {
+            hidePopup($popup);
+        })
+        .on('click', '.confirm', function() {
+            hidePopup($popup);
+            if (kwargs.confirm_callback) kwargs.confirm_callback($popup);
+        })
+        .on('click', '.close-popup', function() {
+            hidePopup($popup);
+        })
+        .on('click', '.popup-wrapper', function(e) {
+            e.stopPropagation();
+        });
 
     if (kwargs.css_class) $popup.addClass(kwargs.css_class);
 
     if (kwargs.content) {
         $popup.find('.popup-content').html(kwargs.content);
     }
 
@@ -75,15 +79,15 @@
         }
     }
     return open_popups;
 }
 
 function disableScroll() {
     if ($(document).height() > $(window).height()) {
-        let scrollTop = ($html.scrollTop()) ? $html.scrollTop() : $body.scrollTop(); // Works for Chrome, Firefox, IE...
+        let scrollTop = $html.scrollTop() ? $html.scrollTop() : $body.scrollTop(); // Works for Chrome, Firefox, IE...
         $html.addClass('noscroll').css('top', -scrollTop);
     }
 }
 
 function enableScroll() {
     let scrollTop = parseInt($html.css('top'));
     $html.removeClass('noscroll');
```

### Comparing `django-content-blocks-1.2.1/content_blocks/templates/.DS_Store` & `django-content-blocks-1.3.0/content_blocks/templates/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.2.1/content_blocks/templates/content_blocks/editor/base.html` & `django-content-blocks-1.3.0/content_blocks/templates/content_blocks/editor/base.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 {#Base template for content block editor to define static files#}
 {% extends 'admin/base_site.html' %}
 {% load static %}
 
 {% block extrastyle %}
-    {{ block.super }}
-    <link rel="stylesheet" type="text/css" href="{% static 'admin/css/forms.css' %}" />
-    <link rel="stylesheet" type="text/css" href="{% static 'content_blocks/fontawesome/css/procompatibility.css' %}"/>
-    <link rel="stylesheet" type="text/css" href="{% static 'content_blocks/fontawesome/css/fontawesome.min.css' %}"/>
-    <link rel="stylesheet" type="text/css" href="{% static 'content_blocks/fontawesome/css/solid.min.css' %}"/>
-    <link rel="stylesheet" type="text/css" href="{% static 'content_blocks/fontawesome/css/light.min.css' %}"/>
-    <link rel="stylesheet" type="text/css" href="{% static 'content_blocks/fontawesome/css/thin.min.css' %}"/>
-    <link rel="stylesheet" type="text/css" href="{% static 'content_blocks/jqueryui/jquery-ui.min.css' %}"/>
-    <link rel="stylesheet" type="text/css" href="{% static 'content_blocks/css/content_blocks.css' %}" media="screen" />
+  {{ block.super }}
+  <link rel="stylesheet" type="text/css" href="{% static 'admin/css/forms.css' %}" />
+  <link rel="stylesheet" type="text/css" href="{% static 'content_blocks/fontawesome/css/procompatibility.css' %}"/>
+  <link rel="stylesheet" type="text/css" href="{% static 'content_blocks/fontawesome/css/fontawesome.min.css' %}"/>
+  <link rel="stylesheet" type="text/css" href="{% static 'content_blocks/fontawesome/css/solid.min.css' %}"/>
+  <link rel="stylesheet" type="text/css" href="{% static 'content_blocks/fontawesome/css/light.min.css' %}"/>
+  <link rel="stylesheet" type="text/css" href="{% static 'content_blocks/fontawesome/css/thin.min.css' %}"/>
+  <link rel="stylesheet" type="text/css" href="{% static 'content_blocks/jqueryui/jquery-ui.min.css' %}"/>
+  <link rel="stylesheet" type="text/css" href="{% static 'content_blocks/css/content_blocks.css' %}" media="screen" />
 {% endblock %}
 
 {% block extrahead %}
-    {{ block.super }}
-    <script type="text/javascript" src="{% static 'admin/js/vendor/jquery/jquery.min.js' %}"></script>
-    <script type="text/javascript" src="{% static 'content_blocks/jqueryui/jquery-ui.min.js' %}"></script>
-    <script type="text/javascript" src="{% static 'content_blocks/js/ajax_setup.js' %}"></script>
-    <script type="text/javascript" src="{% static 'content_blocks/jqueryform/jquery.form.min.js' %}"></script>
-    <script type="text/javascript" src="{% static 'content_blocks/iframeresizer/iframeResizer.js' %}"></script>
-    <script type="text/javascript" src="{% static 'content_blocks/js/popup.js' %}"></script>
-    <script type="text/javascript" src="{% static 'content_blocks/js/content_block_editor.js' %}"></script>
+  {{ block.super }}
+  <script type="text/javascript" src="{% static 'admin/js/vendor/jquery/jquery.min.js' %}"></script>
+  <script type="text/javascript" src="{% static 'content_blocks/jqueryui/jquery-ui.min.js' %}"></script>
+  <script type="text/javascript" src="{% static 'content_blocks/js/ajax_setup.js' %}"></script>
+  <script type="text/javascript" src="{% static 'content_blocks/jqueryform/jquery.form.min.js' %}"></script>
+  <script type="text/javascript" src="{% static 'content_blocks/iframeresizer/iframeResizer.js' %}"></script>
+  <script type="text/javascript" src="{% static 'content_blocks/js/popup.js' %}"></script>
+  <script type="text/javascript" src="{% static 'content_blocks/js/content_block_editor.js' %}"></script>
 {% endblock %}
 
 {% block content %}
-    <div class="cb-editor" id="content-main">
-        {% block object_tools %}{% endblock %}
-        {% block main %}{% endblock %}
-    </div>
-{% endblock %}
+  <div class="cb-editor" id="content-main">
+    {% block object_tools %}{% endblock %}
+    {% block main %}{% endblock %}
+  </div>
+{% endblock %}
```

### Comparing `django-content-blocks-1.2.1/content_blocks/templates/content_blocks/editor/content_block_form.html` & `django-content-blocks-1.3.0/content_blocks/templates/content_blocks/editor/content_block_form.html`

 * *Files 5% similar despite different names*

```diff
@@ -2,66 +2,67 @@
 <form action="{% url 'content_blocks:content_block_save' content_block.id %}"
       method="post"
       enctype="multipart/form-data"
       class="cb-form" id="cb_form_{{ content_block.id }}"
       data-target="#cb_form_wrapper_{{ content_block.id }}"
       data-btn="#save_{{ content_block.id }}"
 >
-    <div class="title-bar clearfix">
-        <div class="field-wrapper title col fl cl" id="title_{{ content_block.id }}">
-            <h2>{{ content_block.content_block_template }} #{{ content_block.id }}</h2>
-        </div>
+  <div class="title-bar clearfix">
+    <div class="field-wrapper title col fl cl" id="title_{{ content_block.id }}">
+      <h2>{{ content_block.content_block_template }} #{{ content_block.id }}</h2>
+    </div>
 
-        <div class="field-wrapper col fl clearfix">
-            <label for="id_{{ form.css_class.html_name }}" class="{{ form.css_class.html_name }} fl pos-rel">
-                {{ form.css_class.label }}:
-                {% if form.css_class.help_text %}
-                    <i class="fa-solid fa-light fa-info-circle tooltip help-text pos-abs" title="{{ form.css_class.help_text }}"></i>
-                {% endif %}
-            </label>
-
-            <div class="field fl">
-                {{ form.css_class }}
-            </div>
-        </div>
+    <div class="field-wrapper col fl clearfix">
+      <label for="id_{{ form.css_class.html_name }}" class="{{ form.css_class.html_name }} fl pos-rel">
+        {{ form.css_class.label }}:
+        {% if form.css_class.help_text %}
+          <i class="fa-solid fa-question-circle tooltip help-text pos-abs" title="{{ form.css_class.help_text }}"></i>
+        {% endif %}
+      </label>
+
+      <div class="field fl">
+        {{ form.css_class }}
+      </div>
     </div>
+  </div>
 
-    <div class="fields clearfix expander expander_{{ content_block.id }}">
-        {% for field in form %}
-            {% if field.html_name != 'css_class' %}
-                {% cycle 'cl-4 4c1' '4c2' '4c3' '4c4' as col4 silent %}
-                {% cycle 'cl-3 3c1' '3c2' '3c3' as col3 silent %}
-                {% cycle 'cl-2 2c1' '2c2' as col2 silent %}
-
-                {% if field.field.cb_field.preview_template_name and col4 == '4c4' %}
-                    {% resetcycle col4 %}
-                    {% cycle col4 %}
-                {% endif %}
-
-                {% if field.field.cb_field.preview_template_name and col3 == '3c3' %}
-                    {% resetcycle col3 %}
-                    {% cycle col3 %}
-                {% endif %}
-
-                {% if field.field.cb_field.preview_template_name and col2 == '2c2' %}
-                    {% resetcycle col2 %}
-                    {% cycle col2 %}
-                {% endif %}
-
-                <div class="field-wrapper {{ field.field.cb_field.field_type|slugify }} {% firstof field.field.widget.input_type "textarea" %} fl clearfix {{ col2 }} {{ col3 }} {{ col4 }} col {{ field.field.cb_field.template_field.css_class }}">
-
-                    {% include field.field.cb_field.template_name %}
-                </div>
-
-                {% if field.field.cb_field.preview_template_name %}
-                    {% cycle col4 %}
-                    {% cycle col3 %}
-                    {% cycle col2 %}
-                    <div class="field-wrapper {% firstof field.field.widget.name field.field.widget.input_type %} col fl clearfix {{ col2 }} {{ col3 }} {{ col4 }}">
-                        {% include field.field.cb_field.preview_template_name %}
-                    </div>
-                {% endif %}
+  <div class="fields clearfix expander expander_{{ content_block.id }}">
+    {% for field in form %}
+      {% if field.html_name != 'css_class' %}
+        {% cycle 'cl-4 4c1' '4c2' '4c3' '4c4' as col4 silent %}
+        {% cycle 'cl-3 3c1' '3c2' '3c3' as col3 silent %}
+        {% cycle 'cl-2 2c1' '2c2' as col2 silent %}
+
+        {% if field.field.cb_field.preview_template_name and col4 == '4c4' %}
+          {% resetcycle col4 %}
+          {% cycle col4 %}
+        {% endif %}
+
+        {% if field.field.cb_field.preview_template_name and col3 == '3c3' %}
+          {% resetcycle col3 %}
+          {% cycle col3 %}
+        {% endif %}
+
+        {% if field.field.cb_field.preview_template_name and col2 == '2c2' %}
+          {% resetcycle col2 %}
+          {% cycle col2 %}
+        {% endif %}
 
-            {% endif %}
-        {% endfor %}
-    </div>
+        <div class="field-wrapper {{ field.field.cb_field.field_type|slugify }} {% firstof field.field.widget.input_type "textarea" %} fl clearfix {{ col2 }} {{ col3 }} {{ col4 }} col {{ field.field.cb_field.template_field.css_class }}">
+
+          {% include field.field.cb_field.template_name %}
+        </div>
+
+
+        {% if field.field.cb_field.preview_template_name %}
+          {% cycle col4 %}
+          {% cycle col3 %}
+          {% cycle col2 %}
+          <div class="field-wrapper {% firstof field.field.widget.name field.field.widget.input_type %} col fl clearfix {{ col2 }} {{ col3 }} {{ col4 }}">
+            {% include field.field.cb_field.preview_template_name %}
+          </div>
+        {% endif %}
+
+      {% endif %}
+    {% endfor %}
+  </div>
 </form>
```

### Comparing `django-content-blocks-1.2.1/content_blocks/templates/content_blocks/editor/content_block_form_wrapper.html` & `django-content-blocks-1.3.0/content_blocks/templates/content_blocks/editor/content_block_form_wrapper.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,109 +1,113 @@
 {#Wrapper for the content block form.  Used when adding new content blocks.#}
 {% load content_block_admin %}
 {% load admin_urls %}
 
 <div class="content-block-form pos-rel clearfix" id="cb_{{ content_block.id }}">
 
-    {% include 'content_blocks/partials/loader.html' with loader_id=content_block.id %}
+  {% include 'content_blocks/partials/loader.html' with loader_id=content_block.id %}
 
-    <div class="preview" id="preview_{{ content_block.id }}">
-        <iframe data-src="{% url opts|admin_urlname:'content_block_preview' parent.id content_block.id %}"></iframe>
-    </div>
-
-    <div class="pos-rel">
-        <div class="controls">
-            <button class="expand"
-                    tabindex="-1"
-                    data-target=".expander_{{ content_block.id }}"
-            >
-                <i class="fa-solid fa-light fa-chevron-up"></i>
-            </button>
-
-            {% if content_block.can_render %}
-                <button class="preview"
-                        tabindex="-1"
-                        data-target="#preview_{{ content_block.id }}"
-                        data-save="#save_{{ content_block.id }}"
-                >
-                    <i class="fa-solid fa-light fa-image"></i>
-                </button>
-            {% endif %}
-
-            <button class="visible"
-                    tabindex="-1"
-                    data-ajax_url="{% url 'content_blocks:toggle_visible' content_block.id %}"
-                    data-label="#title_{{ content_block.id }}"
-            >
-                <i class="fa-solid fa-light {% if content_block.visible %}fa-eye{% else %}fa-eye-slash{% endif %}"></i>
-            </button>
-
-            <button class="delete"
-                    tabindex="-1"
-                    data-ajax_url="{% url 'content_blocks:content_block_delete' content_block.id %}"
-                    data-target="#cb_{{ content_block.id }}"
-                    data-label="#title_{{ content_block.id }}"
-                    data-loader="#loader_{{ content_block.id }}"
-            >
-                <i class="fa-solid fa-light {% if nested_num <= min_num %}fa-trash-slash{% else %}fa-trash{% endif %}"></i>
-            </button>
+  <div class="preview" id="preview_{{ content_block.id }}">
+    <iframe data-src="{% url opts|admin_urlname:'content_block_preview' parent.id content_block.id %}"></iframe>
+  </div>
+
+  <div class="pos-rel">
+    <div class="controls">
+      <button class="expand"
+              tabindex="-1"
+              data-target=".expander_{{ content_block.id }}"
+      >
+        <i class="fa-solid fa-light fa-chevron-up"></i>
+      </button>
+
+      {% if content_block.can_render %}
+        <button class="preview"
+                tabindex="-1"
+                data-target="#preview_{{ content_block.id }}"
+                data-save="#save_{{ content_block.id }}"
+        >
+          <i class="fa-solid fa-light fa-image"></i>
+        </button>
+      {% endif %}
+
+      <button class="visible"
+              tabindex="-1"
+              data-ajax_url="{% url 'content_blocks:toggle_visible' content_block.id %}"
+              data-label="#title_{{ content_block.id }}"
+      >
+        <i class="fa-solid fa-light {% if content_block.visible %}fa-eye{% else %}fa-eye-slash{% endif %}"></i>
+      </button>
+
+      <button class="delete"
+              tabindex="-1"
+              data-ajax_url="{% url 'content_blocks:content_block_delete' content_block.id %}"
+              data-target="#cb_{{ content_block.id }}"
+              data-label="#title_{{ content_block.id }}"
+              data-loader="#loader_{{ content_block.id }}"
+      >
+        <i class="fa-solid fa-light {% if nested_num <= min_num %}fa-trash-slash{% else %}fa-trash{% endif %}"></i>
+      </button>
+
+      <button class="save {% if saved %}saved{% endif %}"
+              tabindex="-1"
+              id="save_{{ content_block.id }}"
+              data-form="#cb_form_{{ content_block.id }}"
+              data-loader="#loader_{{ content_block.id }}"
+      >
+        <i class="fa-solid fa-light {% if saved %}fa-floppy-disk{% else %}fa-floppy-disk-circle-xmark{% endif %}"></i>
+      </button>
 
-            <button class="save {% if saved %}saved{% endif %}"
-                    tabindex="-1"
-                    id="save_{{ content_block.id }}"
-                    data-form="#cb_form_{{ content_block.id }}"
-                    data-loader="#loader_{{ content_block.id }}"
-            >
-                <i class="fa-solid fa-light {% if saved %}fa-floppy-disk{% else %}fa-floppy-disk-circle-xmark{% endif %}"></i>
-            </button>
+      <button class="move" tabindex="-1"><i class="fa-solid fa-light fa-sort"></i></button>
+    </div>
 
-            <button class="move" tabindex="-1"><i class="fa-solid fa-light fa-sort"></i></button>
-        </div>
+    <div class="cb-form-wrapper" id="cb_form_wrapper_{{ content_block.id }}">
+      {% include 'content_blocks/editor/content_block_form.html' %}
+    </div>
 
-        <div class="cb-form-wrapper" id="cb_form_wrapper_{{ content_block.id }}">
-            {% include 'content_blocks/editor/content_block_form.html' %}
+    <div class="expander expander_{{ content_block.id }}">
+            {#	Nested fields #}
+      {% for field in content_block.nested_fields.values %}
+        <div class="controls wrapper-controls">
+          <h3 class="nested-title">
+            {{ field.label }}
+
+            <i class="fa-solid fa-question-circle help-text" title="{% if field.template_field.help_text %}{{ field.template_field.help_text }}{% else %}Min: {{ field.template_field.min_num }} Max: {{ field.template_field.max_num }}{% endif %}"></i>
+          </h3>
+
+          <button tabindex="-1" class="collapse-all" data-target="#nested_blocks_{{ field.id }}">
+            <i class="fa-solid fa-light fa-chevrons-up"></i>
+          </button>
+          <button tabindex="-1" class="expand-all" data-target="#nested_blocks_{{ field.id }}">
+            <i class="fa-solid fa-light fa-chevrons-down"></i>
+          </button>
         </div>
 
-        <div class="expander expander_{{ content_block.id }}">
-            {#	Nested fields #}
-            {% for field in content_block.nested_fields.values %}
-                <div class="controls wrapper-controls">
-                    <h3 class="nested-title">{{ field.label }}</h3>
-
-                    <button tabindex="-1" class="collapse-all" data-target="#nested_blocks_{{ field.id }}">
-                        <i class="fa-solid fa-light fa-chevrons-up"></i>
-                    </button>
-                    <button tabindex="-1" class="expand-all" data-target="#nested_blocks_{{ field.id }}">
-                        <i class="fa-solid fa-light fa-chevrons-down"></i>
-                    </button>
-                </div>
-
-                {% with field.content_blocks.all as field_content_blocks %}
-                    <div class="content-blocks pos-rel"
-                         id="nested_blocks_{{ field.id }}"
-                         data-min_num="{{ field.template_field.min_num }}"
-                         data-max_num="{{ field.template_field.max_num }}"
-                    >
-                        {% for nested_block in field_content_blocks %}
-                            {% content_block_form nested_block as content_block_form %}
-                            {% include 'content_blocks/editor/content_block_form_wrapper.html' with form=content_block_form content_block=nested_block saved=nested_block.saved nested_num=field_content_blocks|length min_num=field.template_field.min_num %}
-                        {% endfor %}
-                    </div>
-
-                    <div class="cb-nested-create-form">
-                        {% new_nested_block_form field as new_nested_form %}
-                        <form action="{% url opts|admin_urlname:'nested_block_create' parent.id %}"
-                              method="post"
-                              class="nested-create-form {% if field_content_blocks|length >= field.template_field.max_num %}disabled{% endif %} clearfix"
-                              data-target="#nested_blocks_{{ field.id }}"
-                        >
-                            {% for f in new_nested_form %}
-                                {{ f }}
-                            {% endfor %}
-                            <button type="submit">Add <span class="nested-create-label"></span></button>
-                        </form>
-                    </div>
-                {% endwith %}
+        {% with field.content_blocks.all as field_content_blocks %}
+          <div class="content-blocks pos-rel"
+               id="nested_blocks_{{ field.id }}"
+               data-min_num="{{ field.template_field.min_num }}"
+               data-max_num="{{ field.template_field.max_num }}"
+          >
+            {% for nested_block in field_content_blocks %}
+              {% content_block_form nested_block as content_block_form %}
+              {% include 'content_blocks/editor/content_block_form_wrapper.html' with form=content_block_form content_block=nested_block saved=nested_block.saved nested_num=field_content_blocks|length min_num=field.template_field.min_num %}
             {% endfor %}
-        </div>
+          </div>
+
+          <div class="cb-nested-create-form">
+            {% new_nested_block_form field as new_nested_form %}
+            <form action="{% url opts|admin_urlname:'nested_block_create' parent.id %}"
+                  method="post"
+                  class="nested-create-form {% if field_content_blocks|length >= field.template_field.max_num %}disabled{% endif %} clearfix"
+                  data-target="#nested_blocks_{{ field.id }}"
+            >
+              {% for f in new_nested_form %}
+                {{ f }}
+              {% endfor %}
+              <button type="submit">Add <span class="nested-create-label"></span></button>
+            </form>
+          </div>
+        {% endwith %}
+      {% endfor %}
     </div>
-</div>
+  </div>
+</div>
```

### Comparing `django-content-blocks-1.2.1/content_blocks/templates/content_blocks/editor/editor.html` & `django-content-blocks-1.3.0/content_blocks/templates/content_blocks/editor/editor.html`

 * *Files 2% similar despite different names*

```diff
@@ -2,134 +2,134 @@
 {% load admin_urls %}
 {% load i18n %}
 {% load content_block_admin %}
 
 {% block title %}Change Content Blocks for {{ parent }}{% endblock %}
 
 {% block extrahead %}
-    {{ block.super }}
-    <script type="text/javascript">
-        $(document).ready(function() {
-            $('.cb-wrapper').ContentBlockEditor({
-                update_position_url: "{% url 'content_blocks:update_position' %}",
-                parent_model: "{% app_model_label parent %}",
-                parent_id: "{{ parent.id }}"
-            });
-        });
-    </script>
+  {{ block.super }}
+  <script type="text/javascript">
+    $(document).ready(function() {
+      $('.cb-wrapper').ContentBlockEditor({
+        update_position_url: "{% url 'content_blocks:update_position' %}",
+        parent_model: "{% app_model_label parent %}",
+        parent_id: "{{ parent.id }}"
+      });
+    });
+  </script>
 {% endblock %}
 
 <!-- BREADCRUMBS -->
 {% if not is_popup %}
-    {% block breadcrumbs %}
-        <div class="breadcrumbs">
-            <a href="{% url 'admin:index' %}">{% trans "Home" %}</a> &rsaquo;
-            <a href="{% url 'admin:app_list' app_label=opts.app_label %}">{{ opts.app_config.verbose_name }}</a> &rsaquo;
-            {% url opts|admin_urlname:'changelist' as changelist_url %}
-            <a href="{% add_preserved_filters changelist_url %}">{{ opts.verbose_name_plural|capfirst }}</a> &rsaquo;
-            <a href="{% url opts|admin_urlname:'change' parent.id %}">{{ parent }}</a> &rsaquo;
-            Change content blocks
-        </div>
-    {% endblock %}
+  {% block breadcrumbs %}
+    <div class="breadcrumbs">
+      <a href="{% url 'admin:index' %}">{% trans "Home" %}</a> &rsaquo;
+      <a href="{% url 'admin:app_list' app_label=opts.app_label %}">{{ opts.app_config.verbose_name }}</a> &rsaquo;
+      {% url opts|admin_urlname:'changelist' as changelist_url %}
+      <a href="{% add_preserved_filters changelist_url %}">{{ opts.verbose_name_plural|capfirst }}</a> &rsaquo;
+      <a href="{% url opts|admin_urlname:'change' parent.id %}">{{ parent }}</a> &rsaquo;
+      Change content blocks
+    </div>
+  {% endblock %}
 {% endif %}
 
 {% block messages %}{% endblock %}
 
 {% block object_tools %}
-    {% if parent.preview_url %}
-        <ul class="object-tools">
-            <li>
-                <a href="{{ parent.preview_url }}" target="_blank" class="viewsitelink">Preview on site</a>
-            </li>
-        </ul>
-    {% endif %}
+  {% if parent.preview_url %}
+    <ul class="object-tools">
+      <li>
+        <a href="{{ parent.preview_url }}" target="_blank" class="viewsitelink">Preview on site</a>
+      </li>
+    </ul>
+  {% endif %}
 {% endblock %}
 
 {% block content_title %}
-    <h1>Change Content Blocks for {{ parent }}</h1>
+  <h1>Change Content Blocks for {{ parent }}</h1>
 {% endblock %}
 
 {% block main %}
-    {% include 'content_blocks/partials/loader.html' with loader_id='root' %}
+  {% include 'content_blocks/partials/loader.html' with loader_id='root' %}
 
-    <div class="cb-wrapper">
-        <div class="controls wrapper-controls root-wrapper-controls">
-            <button tabindex="-1" class="collapse-all" data-target="#content-blocks-root">
-                <i class="fa-solid fa-light fa-chevrons-up"></i>
-            </button>
-            <button tabindex="-1" class="expand-all" data-target="#content-blocks-root">
-                <i class="fa-solid fa-light fa-chevrons-down"></i>
-            </button>
-        </div>
-
-        <div class="content-blocks pos-rel" id="content-blocks-root">
-            <div class="cb-import-form" {% if parent.content_blocks.drafts %}style="display: none;"{% endif %}>
-                {% if import_content_blocks_form.get_master_queryset %}
-
-                    <form
-                          action="{% url opts|admin_urlname:'import_content_blocks' parent.id %}"
-                          method="post"
-                          class="import-form clearfix"
-                          data-loader="#loader_root"
-                    >
-                        {% for field in import_content_blocks_form %}
-                            {{ field }}
-                        {% endfor %}
-                        <button class="button" type="submit">Import Blocks From <span id="cb_import_label"></span></button>
-                    </form>
-                    <p>-or-</p>
-                {% endif %}
-                <p><i class="fa-solid fa-light fa-arrow-down"></i> Start adding new blocks below <i class="fa-solid fa-light fa-arrow-down"></i></p>
-            </div>
-
-            {% include 'content_blocks/editor/content_block_forms.html' %}
-        </div>
-
-        <div class="cb-create-form clearfix">
-            <form action="{% url opts|admin_urlname:'content_block_create' parent.id %}" method="post" class="create-form">
-                {% for field in new_content_block_form %}
-                    {{ field }}
-                {% endfor %}
-                <button class="button" type="submit">Add <span id="cb_create_label"></span></button>
-            </form>
-        </div>
+  <div class="cb-wrapper">
+    <div class="controls wrapper-controls root-wrapper-controls">
+      <button tabindex="-1" class="collapse-all" data-target="#content-blocks-root">
+        <i class="fa-solid fa-light fa-chevrons-up"></i>
+      </button>
+      <button tabindex="-1" class="expand-all" data-target="#content-blocks-root">
+        <i class="fa-solid fa-light fa-chevrons-down"></i>
+      </button>
     </div>
 
-    <div class="publish-bar">
-
-        <div class="status">{{ status_message|safe }}</div>
-
-        <button class="button" id="save_exit" data-return_url="{{ return_url }}" data-loader="#loader_root">
-            <i class="fa-solid fa-light fa-floppy-disk-circle-arrow-right"></i> Exit
-        </button>
-
-        <form action="{% url opts|admin_urlname:'discard_changes' parent.id %}"
-              method="post"
-              id="discard_form"
-              data-return_url="{{ return_url }}"
-              data-loader="#loader_root"
-        >
-            {% for field in discard_form %}
-                {{ field }}
+    <div class="content-blocks pos-rel" id="content-blocks-root">
+      <div class="cb-import-form" {% if parent.content_blocks.drafts %}style="display: none;"{% endif %}>
+        {% if import_content_blocks_form.get_master_queryset %}
+
+          <form
+            action="{% url opts|admin_urlname:'import_content_blocks' parent.id %}"
+            method="post"
+            class="import-form clearfix"
+            data-loader="#loader_root"
+          >
+            {% for field in import_content_blocks_form %}
+              {{ field }}
             {% endfor %}
-            <button class="button" type="submit"><i class="fa-solid fa-light fa-arrow-rotate-left"></i> Reset</button>
-        </form>
+            <button class="button" type="submit">Import Blocks From <span id="cb_import_label"></span></button>
+          </form>
+          <p>-or-</p>
+        {% endif %}
+        <p><i class="fa-solid fa-light fa-arrow-down"></i> Start adding new blocks below <i class="fa-solid fa-light fa-arrow-down"></i></p>
+      </div>
 
-        <form action="{% url opts|admin_urlname:'publish_content_blocks' parent.id %}"
-              method="post"
-              id="publish_form"
-              data-return_url="{{ return_url }}"
-              data-loader="#loader_root"
-        >
-            {% for field in publish_form %}
-                {{ field }}
-            {% endfor %}
-            <button class="button" type="submit"><i class="fa-solid fa-light fa-cloud-arrow-up"></i> Publish</button>
-        </form>
+      {% include 'content_blocks/editor/content_block_forms.html' %}
+    </div>
 
-        <button class="button" id="save_continue" data-loader="#loader_root"><i class="fa-solid fa-light fa-floppy-disk"></i> Save</button>
+    <div class="cb-create-form clearfix">
+      <form action="{% url opts|admin_urlname:'content_block_create' parent.id %}" method="post" class="create-form">
+        {% for field in new_content_block_form %}
+          {{ field }}
+        {% endfor %}
+        <button class="button" type="submit">Add <span id="cb_create_label"></span></button>
+      </form>
     </div>
+  </div>
+
+  <div class="publish-bar">
 
-    {% include 'content_blocks/partials/popup.html' %}
-    {% include 'content_blocks/partials/delete_popup.html' %}
-    {% include 'content_blocks/partials/reset_popup.html' %}
-{% endblock %}
+    <div class="status">{{ status_message|safe }}</div>
+
+    <button class="button" id="save_exit" data-return_url="{{ return_url }}" data-loader="#loader_root">
+      <i class="fa-solid fa-light fa-floppy-disk-circle-arrow-right"></i> Exit
+    </button>
+
+    <form action="{% url opts|admin_urlname:'discard_changes' parent.id %}"
+          method="post"
+          id="discard_form"
+          data-return_url="{{ return_url }}"
+          data-loader="#loader_root"
+    >
+      {% for field in discard_form %}
+        {{ field }}
+      {% endfor %}
+      <button class="button" type="submit"><i class="fa-solid fa-light fa-arrow-rotate-left"></i> Reset</button>
+    </form>
+
+    <form action="{% url opts|admin_urlname:'publish_content_blocks' parent.id %}"
+          method="post"
+          id="publish_form"
+          data-return_url="{{ return_url }}"
+          data-loader="#loader_root"
+    >
+      {% for field in publish_form %}
+        {{ field }}
+      {% endfor %}
+      <button class="button" type="submit"><i class="fa-solid fa-light fa-cloud-arrow-up"></i> Publish</button>
+    </form>
+
+    <button class="button" id="save_continue" data-loader="#loader_root"><i class="fa-solid fa-light fa-floppy-disk"></i> Save</button>
+  </div>
+
+  {% include 'content_blocks/partials/popup.html' %}
+  {% include 'content_blocks/partials/delete_popup.html' %}
+  {% include 'content_blocks/partials/reset_popup.html' %}
+{% endblock %}
```

### Comparing `django-content-blocks-1.2.1/content_blocks/templates/content_blocks/widgets/clearable_file.html` & `django-content-blocks-1.3.0/content_blocks/templates/content_blocks/widgets/clearable_file.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <input type="{{ widget.type }}" name="{{ widget.name }}"{% include "django/forms/widgets/attrs.html" %}>
 {% if widget.is_initial %}
-    {% if not widget.required %}
-        <label class="checkbox" for="{{ widget.checkbox_id }}">
-            <input type="checkbox" name="{{ widget.checkbox_name }}" id="{{ widget.checkbox_id }}"{% if widget.attrs.disabled %} disabled{% endif %}>
-            <span></span>{{ widget.clear_checkbox_label }}
-        </label>
-    {% endif %}
-    <label class="currently">
-        <a href="{{ widget.value.url }}" target="_blank">{{ widget.value }}</a>
+  {% if not widget.required %}
+    <label class="checkbox" for="{{ widget.checkbox_id }}">
+      <input type="checkbox" name="{{ widget.checkbox_name }}" id="{{ widget.checkbox_id }}"{% if widget.attrs.disabled %} disabled{% endif %}>
+      <span></span>{{ widget.clear_checkbox_label }}
     </label>
-{% endif %}
+  {% endif %}
+  <label class="currently">
+    <a href="{{ widget.value.url }}" target="_blank">{{ widget.value }}</a>
+  </label>
+{% endif %}
```

### Comparing `django-content-blocks-1.2.1/content_blocks/templatetags/content_block_admin.py` & `django-content-blocks-1.3.0/content_blocks/templatetags/content_block_admin.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.2.1/content_blocks/templatetags/content_blocks.py` & `django-content-blocks-1.3.0/content_blocks/templatetags/content_blocks.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Content blocks template tags.
 """
 from django import template
 
 from content_blocks.models import ContentBlockCollection
+from content_blocks.services.content_block import RenderServices
 
 register = template.Library()
 
 
 @register.inclusion_tag(
     "content_blocks/content_block_collection.html", takes_context=True
 )
@@ -28,23 +29,25 @@
     return context
 
 
 @register.simple_tag(takes_context=True)
 def render_content_block(context, content_block):
     """
     Allows rendering of content blocks with request context.  Content blocks should have no_cache=True in this case.
-    :param context:
-    :param content_block:
-    :return:
     """
 
     # Because our context might have RequestContext already in it flatten ourselves
     context_dict = {}
     for d in context.dicts:
         try:
             d = d.flatten()
         except AttributeError:
             pass
 
         context_dict.update(d)
 
-    return content_block.render(context=context_dict)
+    return RenderServices.render_content_block(content_block, context=context_dict)
+
+
+# todo render_content_blocks template tag to render a set of blocks given the parent
+
+# todo render_content_block_previews template tag as above but renders previews
```

### Comparing `django-content-blocks-1.2.1/content_blocks/urls.py` & `django-content-blocks-1.3.0/content_blocks/urls.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.2.1/content_blocks/views.py` & `django-content-blocks-1.3.0/content_blocks/views.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,76 @@
 """
 Content Blocks views.py
 """
+from functools import wraps
+from io import StringIO
+
+from django.contrib import messages
 from django.contrib.admin.models import ADDITION, CHANGE, DELETION, LogEntry
 from django.contrib.admin.views.decorators import staff_member_required
 from django.contrib.contenttypes.models import ContentType
-from django.http import JsonResponse
-from django.shortcuts import get_object_or_404, render
+from django.core.exceptions import PermissionDenied
+from django.http import JsonResponse, StreamingHttpResponse
+from django.shortcuts import get_object_or_404, redirect, render
 from django.template.loader import render_to_string
 from django.urls import reverse
 from django.views.decorators.csrf import ensure_csrf_cookie
 from django.views.decorators.http import require_POST
 
+from content_blocks.admin_forms import ContentBlockTemplateImportForm
 from content_blocks.conf import settings
 from content_blocks.forms import (
     ContentBlockForm,
     ImportContentBlocksForm,
     NewContentBlockForm,
     NewNestedBlockForm,
     PublishContentBlocksForm,
     ResetContentBlocksForm,
 )
 from content_blocks.models import ContentBlock
-from content_blocks.permissions import require_ajax
+from content_blocks.services.content_block_template import ImportExportServices
+
+
+def require_ajax(view):
+    @wraps(view)
+    def _wrapped_view(request, *args, **kwargs):
+        if request.headers.get("x-requested-with") == "XMLHttpRequest":
+            return view(request, *args, **kwargs)
+        else:
+            raise PermissionDenied
+
+    return _wrapped_view
 
 
 def create_log_entry(request, obj, action_flag, change_message, **kwargs):
     params = {
         "user_id": request.user.id,
-        "content_type_id": ContentType.objects.get_for_model(obj.__class__).id,
-        "object_id": obj.id,
         "object_repr": obj.__str__(),
         "action_flag": action_flag,
         "change_message": change_message,
+        "content_type_id": None,
+        "object_id": None,
     }
 
+    if obj:
+        params.update(
+            {
+                "content_type_id": ContentType.objects.get_for_model(obj.__class__).id,
+                "object_id": obj.id,
+            }
+        )
+
     params.update(kwargs)
 
     LogEntry.objects.log_action(**params)
 
 
+# Content block editor views
+
+
 @staff_member_required
 @ensure_csrf_cookie
 def content_block_editor(request, object_id, model_admin=None):
     """
     Show the content block editor.
     """
     parent = get_object_or_404(model_admin.model, id=object_id)
@@ -183,14 +211,15 @@
 @staff_member_required
 @require_POST
 @require_ajax
 def update_position(request):
     """
     Update position after a content block has been dragon dropped.
     """
+    # todo refactor to service class
     positions = request.POST.get("positions", "")
     positions = f"&{positions}".split("&cb[]=")[1:]
     for i, id in enumerate(positions):
         ContentBlock.objects.filter(id=id).update(position=i)
     # Admin log entry?  Might be a bit spammy. Unless we pass the cb which was dragged and just log on that one?
     return JsonResponse({})
 
@@ -198,14 +227,15 @@
 @staff_member_required
 @require_POST
 @require_ajax
 def toggle_visible(request, content_block_id):
     """
     Toggle visible buttons
     """
+    # todo refactor to service class
     content_block = ContentBlock.objects.get(id=content_block_id)
     content_block.visible = not content_block.visible
     content_block.save()
 
     create_log_entry(
         request,
         content_block,
@@ -320,13 +350,76 @@
 @staff_member_required
 @require_POST
 @require_ajax
 def content_block_delete(request, content_block_id):
     """
     Delete a content block.
     """
+    # todo refactor to service class
     content_block = ContentBlock.objects.get(id=content_block_id)
 
     create_log_entry(request, content_block, DELETION, "")
 
     content_block.delete()
     return JsonResponse({})
+
+
+# ContentBlockTemplate import export views
+
+
+@staff_member_required
+def content_block_template_export(request):
+    """
+    Export content block template view used in admin site.
+    Uses the export_content_block_templates management command and streams the result directly to a file download.
+    """
+    buffer = StringIO()
+    ImportExportServices.export_content_block_templates(file_like=buffer)
+    buffer.seek(0)
+
+    return StreamingHttpResponse(
+        buffer,
+        content_type="application/json",
+        headers={
+            "Content-Disposition": 'attachment; filename="content_block_templates.json"'
+        },
+    )
+
+
+@staff_member_required
+def content_block_template_import(request, model_admin=None):
+    """
+    Form for importing ContentBlockTemplate from json created by export_content_block_templates management command.
+    """
+    post_data = None
+    files_data = None
+
+    if request.method == "POST":
+        post_data = request.POST
+        files_data = request.FILES
+
+    form = ContentBlockTemplateImportForm(post_data, files_data)
+
+    if form.is_valid():
+        fixture_file = files_data["fixture_file"]
+        form.import_content_block_templates(fixture_file)
+        messages.success(request, "Content block templates imported.")
+        create_log_entry(
+            request,
+            None,
+            CHANGE,
+            f"Content block templates imported from {fixture_file.name}",
+        )
+        return redirect("admin:content_blocks_contentblocktemplate_changelist")
+
+    context = {
+        "form": form,
+        "opts": model_admin.model._meta,
+    }
+
+    context.update(**model_admin.admin_site.each_context(request))
+
+    return render(
+        request,
+        "content_blocks/admin/content_block_template_import_form.html",
+        context,
+    )
```

### Comparing `django-content-blocks-1.2.1/content_blocks/widgets.py` & `django-content-blocks-1.3.0/content_blocks/widgets.py`

 * *Files identical despite different names*

### Comparing `django-content-blocks-1.2.1/django_content_blocks.egg-info/PKG-INFO` & `django-content-blocks-1.3.0/django_content_blocks.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-content-blocks
-Version: 1.2.1
+Version: 1.3.0
 Summary: HTML content blocks for Django.
 Home-page: https://github.com/Quantra/django-content-blocks
 Author: Vince Coleman
 Author-email: vince@shystudios.co.uk
 License: MIT
 Project-URL: Documentation, https://django-content-blocks.readthedocs.io
 Project-URL: Source, https://github.com/Quantra/django-content-blocks
@@ -28,15 +28,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 Requires-Python: >=3.7
 License-File: LICENSE
 
-.. todo shields.io badges
+|coverage|
+|package version|
+|python versions supported|
+|django versions supported|
+|code style black|
+|license|
 
 =====================
 Django Content Blocks
 =====================
 
 Django Content Blocks is a reusable Django app that allows users to create and manage custom content blocks for their website. Via the django admin site it provides an easy-to-use interface for creating content blocks that can be inserted into any page, as well as a powerful template system for customizing the appearance of those blocks.
 
@@ -70,7 +75,27 @@
 * Dmitry Sobolev for so graciously transferring the django-content-blocks name on pypi
 * Margo Yaguda for linguistic assistance in contacting Dmitry
 
 Contributing
 ------------
 
 Contributions, advice and guidance are welcome. Please make contact **before** writing any code!
+
+
+.. shields.io badges
+
+.. |package version| image:: https://img.shields.io/pypi/v/django-content-blocks
+   :target: https://pypi.python.org/pypi/django-content-blocks/
+
+.. |python versions supported| image:: https://img.shields.io/pypi/pyversions/django-content-blocks
+   :target: https://pypi.python.org/pypi/django-content-blocks/
+
+.. |django versions supported| image:: https://img.shields.io/pypi/frameworkversions/django/django-content-blocks
+   :target: https://pypi.python.org/pypi/django-content-blocks/
+
+.. |coverage| image:: https://img.shields.io/badge/dynamic/xml?color=success&label=coverage&query=round%28%2F%2Fcoverage%2F%40line-rate%20%2A%20100%29&suffix=%25&url=https%3A%2F%2Fraw.githubusercontent.com%2FQuantra%2Fdjango-content-blocks%2Fmaster%2Fcoverage.xml
+
+.. |code style black| image:: https://img.shields.io/badge/code%20style-black-black
+    :target: https://github.com/psf/black
+
+.. |license| image:: https://img.shields.io/github/license/Quantra/django-content-blocks
+    :target: https://github.com/Quantra/django-content-blocks/blob/master/LICENSE
```

### Comparing `django-content-blocks-1.2.1/django_content_blocks.egg-info/SOURCES.txt` & `django-content-blocks-1.3.0/django_content_blocks.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -5,37 +5,36 @@
 setup.cfg
 setup.py
 content_blocks/__init__.py
 content_blocks/abstract_models.py
 content_blocks/admin.py
 content_blocks/admin_forms.py
 content_blocks/apps.py
-content_blocks/cache.py
 content_blocks/conf.py
 content_blocks/fields.py
 content_blocks/forms.py
 content_blocks/models.py
-content_blocks/permissions.py
 content_blocks/signals.py
 content_blocks/urls.py
 content_blocks/views.py
 content_blocks/widgets.py
 content_blocks/management/__init__.py
 content_blocks/management/commands/__init__.py
 content_blocks/management/commands/clear_content_blocks_cache.py
-content_blocks/management/commands/update_content_blocks_cache.py
+content_blocks/management/commands/export_content_block_templates.py
+content_blocks/management/commands/import_content_block_templates.py
+content_blocks/management/commands/set_content_blocks_cache.py
 content_blocks/migrations/0001_initial.py
 content_blocks/migrations/0002_alter_contentblock_css_class_and_more.py
+content_blocks/migrations/0003_alter_contentblocktemplatefield_unique_together_and_more.py
 content_blocks/migrations/__init__.py
 content_blocks/static/content_blocks/.DS_Store
 content_blocks/static/content_blocks/css/.DS_Store
 content_blocks/static/content_blocks/css/content_block_template_admin.css
 content_blocks/static/content_blocks/css/content_blocks.css
-content_blocks/static/content_blocks/fontawesome/.DS_Store
-content_blocks/static/content_blocks/fontawesome/css/.DS_Store
 content_blocks/static/content_blocks/fontawesome/css/fontawesome.min.css
 content_blocks/static/content_blocks/fontawesome/css/light.min.css
 content_blocks/static/content_blocks/fontawesome/css/procompatibility.css
 content_blocks/static/content_blocks/fontawesome/css/solid.min.css
 content_blocks/static/content_blocks/fontawesome/css/thin.min.css
 content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.ttf
 content_blocks/static/content_blocks/fontawesome/webfonts/fa-solid-900.woff2
@@ -51,14 +50,16 @@
 content_blocks/static/content_blocks/js/content_block_template_admin.js
 content_blocks/static/content_blocks/js/popup.js
 content_blocks/templates/.DS_Store
 content_blocks/templates/base.html
 content_blocks/templates/content_blocks/.DS_Store
 content_blocks/templates/content_blocks/content_block_collection.html
 content_blocks/templates/content_blocks/content_block_preview.html
+content_blocks/templates/content_blocks/admin/content_block_template_change_list.html
+content_blocks/templates/content_blocks/admin/content_block_template_import_form.html
 content_blocks/templates/content_blocks/editor/base.html
 content_blocks/templates/content_blocks/editor/content_block_form.html
 content_blocks/templates/content_blocks/editor/content_block_form_wrapper.html
 content_blocks/templates/content_blocks/editor/content_block_forms.html
 content_blocks/templates/content_blocks/editor/editor.html
 content_blocks/templates/content_blocks/partials/delete_popup.html
 content_blocks/templates/content_blocks/partials/loader.html
```

### Comparing `django-content-blocks-1.2.1/setup.cfg` & `django-content-blocks-1.3.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-content-blocks
-version = 1.2.1
+version = 1.3.0
 description = HTML content blocks for Django.
 long_description = file:README.rst
 url = https://github.com/Quantra/django-content-blocks
 author = Vince Coleman
 author_email = vince@shystudios.co.uk
 license = MIT
 classifiers =
```

