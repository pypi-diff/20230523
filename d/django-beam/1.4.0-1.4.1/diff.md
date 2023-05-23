# Comparing `tmp/django-beam-1.4.0.tar.gz` & `tmp/django-beam-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-beam-1.4.0.tar", last modified: Wed May 17 08:51:14 2023, max compression
+gzip compressed data, was "django-beam-1.4.1.tar", last modified: Tue May 23 09:27:00 2023, max compression
```

## Comparing `django-beam-1.4.0.tar` & `django-beam-1.4.1.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.664585 django-beam-1.4.0/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1511 2022-04-27 09:12:32.000000 django-beam-1.4.0/LICENSE
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      284 2023-01-09 10:44:11.000000 django-beam-1.4.0/MANIFEST.in
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3403 2023-05-17 08:51:14.664677 django-beam-1.4.0/PKG-INFO
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2954 2023-03-28 08:37:32.000000 django-beam-1.4.0/README.md
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      740 2023-05-17 08:51:14.665074 django-beam-1.4.0/setup.cfg
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)       53 2022-04-27 09:12:32.000000 django-beam-1.4.0/setup.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.644819 django-beam-1.4.0/src/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.648121 django-beam-1.4.0/src/beam/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      105 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/__init__.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4680 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/actions.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     7485 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/components.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.648272 django-beam-1.4.0/src/beam/contrib/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/contrib/__init__.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.649167 django-beam-1.4.0/src/beam/contrib/auth/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/contrib/auth/__init__.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      196 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/contrib/auth/apps.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      903 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/contrib/auth/forms.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.643530 django-beam-1.4.0/src/beam/contrib/auth/templates/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.650959 django-beam-1.4.0/src/beam/contrib/auth/templates/registration/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      296 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/contrib/auth/templates/registration/logged_out.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1136 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/contrib/auth/templates/registration/login.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      261 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/contrib/auth/templates/registration/password_change_done.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      837 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/contrib/auth/templates/registration/password_change_form.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      364 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/contrib/auth/templates/registration/password_reset_complete.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      980 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/contrib/auth/templates/registration/password_reset_confirm.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      535 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/contrib/auth/templates/registration/password_reset_done.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      616 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/contrib/auth/templates/registration/password_reset_email.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      531 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/contrib/auth/templates/registration/password_reset_form.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      230 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/contrib/auth/urls.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3881 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/contrib/auth/views.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.651150 django-beam-1.4.0/src/beam/contrib/autocomplete_light/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2940 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/contrib/autocomplete_light/__init__.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.643729 django-beam-1.4.0/src/beam/contrib/autocomplete_light/static/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.651347 django-beam-1.4.0/src/beam/contrib/autocomplete_light/static/autocomplete_light/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1011 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/contrib/autocomplete_light/static/autocomplete_light/select2.css
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.651984 django-beam-1.4.0/src/beam/contrib/reversion/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/contrib/reversion/__init__.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      150 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/contrib/reversion/apps.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.643915 django-beam-1.4.0/src/beam/contrib/reversion/templates/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.652332 django-beam-1.4.0/src/beam/contrib/reversion/templates/beam_reversion/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1140 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/contrib/reversion/templates/beam_reversion/version_detail.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1879 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/contrib/reversion/templates/beam_reversion/version_list.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4032 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/contrib/reversion/views.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     7137 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/contrib/reversion/viewsets.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    11062 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/inlines.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1235 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/layouts.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.644036 django-beam-1.4.0/src/beam/locale/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.644087 django-beam-1.4.0/src/beam/locale/de/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.652499 django-beam-1.4.0/src/beam/locale/de/LC_MESSAGES/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     5525 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2814 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/registry.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.652806 django-beam-1.4.0/src/beam/templatetags/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/templatetags/__init__.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     8705 2023-05-17 08:50:04.000000 django-beam-1.4.0/src/beam/templatetags/beam_tags.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.653098 django-beam-1.4.0/src/beam/themes/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/__init__.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.653338 django-beam-1.4.0/src/beam/themes/bootstrap4/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/__init__.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.644411 django-beam-1.4.0/src/beam/themes/bootstrap4/static/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.644533 django-beam-1.4.0/src/beam/themes/bootstrap4/static/beam/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.653555 django-beam-1.4.0/src/beam/themes/bootstrap4/static/beam/css/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    12660 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/static/beam/css/bootstrap-select.min.css
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.654692 django-beam-1.4.0/src/beam/themes/bootstrap4/static/beam/js/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3291 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/static/beam/js/actions.js
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1328 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/static/beam/js/add_related.js
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    94341 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/static/beam/js/bootstrap-select.min.js
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     6007 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/static/beam/js/inlines.js
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    82676 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/static/beam/js/sortable.min.js
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.644667 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.656670 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3374 2023-05-17 08:50:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/base.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      261 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/create.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1668 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/dashboard.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2444 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/delete.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2894 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/detail.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4361 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/form.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     8134 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/list.html
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.659600 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1756 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/actions.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1954 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/detail_field.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4380 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3284 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline_tabular.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1289 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/filters.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      553 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/form_field.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     6084 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/form_inline.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3061 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2865 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular_row.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4586 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/form_layout.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2072 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/layout.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      666 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/links.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      635 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/list_links.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      776 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/messages.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4826 2023-05-17 08:50:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/navigation.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4968 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/pagination.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1489 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/update.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      946 2023-04-27 07:29:04.000000 django-beam-1.4.0/src/beam/themes/bootstrap4/widgets.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      127 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/types.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      983 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/urls.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1584 2023-05-17 08:50:04.000000 django-beam-1.4.0/src/beam/utils.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    21601 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/views.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     7528 2023-04-27 07:29:03.000000 django-beam-1.4.0/src/beam/viewsets.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.660361 django-beam-1.4.0/src/django_beam.egg-info/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3403 2023-05-17 08:51:14.000000 django-beam-1.4.0/src/django_beam.egg-info/PKG-INFO
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4077 2023-05-17 08:51:14.000000 django-beam-1.4.0/src/django_beam.egg-info/SOURCES.txt
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        1 2023-05-17 08:51:14.000000 django-beam-1.4.0/src/django_beam.egg-info/dependency_links.txt
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)       88 2023-05-17 08:51:14.000000 django-beam-1.4.0/src/django_beam.egg-info/requires.txt
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        5 2023-05-17 08:51:14.000000 django-beam-1.4.0/src/django_beam.egg-info/top_level.txt
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-17 08:51:14.664416 django-beam-1.4.0/tests/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    15449 2022-04-27 09:12:32.000000 django-beam-1.4.0/tests/test_actions.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2782 2023-01-11 09:59:58.000000 django-beam-1.4.0/tests/test_components.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    14309 2023-01-23 10:38:56.000000 django-beam-1.4.0/tests/test_contrib_auth.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2040 2022-04-27 09:12:32.000000 django-beam-1.4.0/tests/test_contrib_autocomplete.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    10694 2023-04-27 06:08:23.000000 django-beam-1.4.0/tests/test_contrib_reversion.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      850 2022-04-27 09:12:32.000000 django-beam-1.4.0/tests/test_inlines.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2022-04-27 09:12:32.000000 django-beam-1.4.0/tests/test_layouts.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1849 2022-04-27 09:12:32.000000 django-beam-1.4.0/tests/test_registry.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3284 2023-05-17 08:50:04.000000 django-beam-1.4.0/tests/test_tags.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4771 2023-01-11 09:59:58.000000 django-beam-1.4.0/tests/test_urls.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3946 2023-01-11 09:59:58.000000 django-beam-1.4.0/tests/test_utils.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    31258 2023-03-30 10:35:40.000000 django-beam-1.4.0/tests/test_views.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4275 2022-04-27 09:12:32.000000 django-beam-1.4.0/tests/test_viewsets.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.422494 django-beam-1.4.1/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1511 2022-04-27 09:12:32.000000 django-beam-1.4.1/LICENSE
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      284 2023-01-09 10:44:11.000000 django-beam-1.4.1/MANIFEST.in
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3403 2023-05-23 09:27:00.422703 django-beam-1.4.1/PKG-INFO
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2954 2023-03-28 08:37:32.000000 django-beam-1.4.1/README.md
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      740 2023-05-23 09:27:00.423228 django-beam-1.4.1/setup.cfg
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)       53 2022-04-27 09:12:32.000000 django-beam-1.4.1/setup.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.391719 django-beam-1.4.1/src/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.398187 django-beam-1.4.1/src/beam/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      105 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/__init__.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4680 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/actions.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     7485 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/components.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.398499 django-beam-1.4.1/src/beam/contrib/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/contrib/__init__.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.399575 django-beam-1.4.1/src/beam/contrib/auth/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/contrib/auth/__init__.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      196 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/contrib/auth/apps.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      903 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/contrib/auth/forms.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.390044 django-beam-1.4.1/src/beam/contrib/auth/templates/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.401625 django-beam-1.4.1/src/beam/contrib/auth/templates/registration/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      296 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/contrib/auth/templates/registration/logged_out.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1136 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/contrib/auth/templates/registration/login.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      261 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/contrib/auth/templates/registration/password_change_done.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      837 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/contrib/auth/templates/registration/password_change_form.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      364 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/contrib/auth/templates/registration/password_reset_complete.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      980 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/contrib/auth/templates/registration/password_reset_confirm.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      535 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/contrib/auth/templates/registration/password_reset_done.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      616 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/contrib/auth/templates/registration/password_reset_email.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      531 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/contrib/auth/templates/registration/password_reset_form.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      230 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/contrib/auth/urls.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3881 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/contrib/auth/views.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.401942 django-beam-1.4.1/src/beam/contrib/autocomplete_light/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2940 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/contrib/autocomplete_light/__init__.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.390290 django-beam-1.4.1/src/beam/contrib/autocomplete_light/static/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.402176 django-beam-1.4.1/src/beam/contrib/autocomplete_light/static/autocomplete_light/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1011 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/contrib/autocomplete_light/static/autocomplete_light/select2.css
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.403026 django-beam-1.4.1/src/beam/contrib/reversion/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/contrib/reversion/__init__.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      150 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/contrib/reversion/apps.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.390539 django-beam-1.4.1/src/beam/contrib/reversion/templates/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.403577 django-beam-1.4.1/src/beam/contrib/reversion/templates/beam_reversion/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1140 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/contrib/reversion/templates/beam_reversion/version_detail.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1879 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/contrib/reversion/templates/beam_reversion/version_list.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4032 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/contrib/reversion/views.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     7137 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/contrib/reversion/viewsets.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    11062 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/inlines.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1235 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/layouts.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.390707 django-beam-1.4.1/src/beam/locale/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.390776 django-beam-1.4.1/src/beam/locale/de/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.403798 django-beam-1.4.1/src/beam/locale/de/LC_MESSAGES/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     5525 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2814 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/registry.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.404177 django-beam-1.4.1/src/beam/templatetags/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/templatetags/__init__.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     8705 2023-05-17 08:50:04.000000 django-beam-1.4.1/src/beam/templatetags/beam_tags.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.404509 django-beam-1.4.1/src/beam/themes/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/themes/__init__.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.404786 django-beam-1.4.1/src/beam/themes/bootstrap4/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/__init__.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.391203 django-beam-1.4.1/src/beam/themes/bootstrap4/static/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.391360 django-beam-1.4.1/src/beam/themes/bootstrap4/static/beam/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.405012 django-beam-1.4.1/src/beam/themes/bootstrap4/static/beam/css/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    12660 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/static/beam/css/bootstrap-select.min.css
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.406572 django-beam-1.4.1/src/beam/themes/bootstrap4/static/beam/js/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3291 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/static/beam/js/actions.js
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1328 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/static/beam/js/add_related.js
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    94341 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/static/beam/js/bootstrap-select.min.js
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     6007 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/static/beam/js/inlines.js
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    82676 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/static/beam/js/sortable.min.js
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.391516 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.409258 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3374 2023-05-17 08:50:04.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/base.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      261 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/create.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1537 2023-05-23 09:24:24.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/dashboard.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2265 2023-05-23 09:24:24.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/delete.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2894 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/detail.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4361 2023-05-23 09:24:24.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/form.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     7895 2023-05-23 09:24:24.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/list.html
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.414663 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1750 2023-05-23 09:24:24.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/actions.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2168 2023-05-23 09:24:24.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/detail_field.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4596 2023-05-23 09:24:24.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3298 2023-05-23 09:24:24.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline_tabular.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1289 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/filters.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      604 2023-05-23 09:24:24.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/form_field.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     6373 2023-05-23 09:24:24.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/form_inline.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3075 2023-05-23 09:24:24.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2865 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular_row.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4856 2023-05-23 09:24:24.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/form_layout.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2094 2023-05-23 09:24:24.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/layout.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      666 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/links.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      635 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/list_links.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      776 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/messages.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4826 2023-05-17 08:50:04.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/navigation.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     5068 2023-05-23 09:24:24.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/pagination.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1489 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/update.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      946 2023-04-27 07:29:04.000000 django-beam-1.4.1/src/beam/themes/bootstrap4/widgets.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      127 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/types.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      983 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/urls.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1584 2023-05-17 08:50:04.000000 django-beam-1.4.1/src/beam/utils.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    21601 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/views.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     7528 2023-04-27 07:29:03.000000 django-beam-1.4.1/src/beam/viewsets.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.415548 django-beam-1.4.1/src/django_beam.egg-info/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3403 2023-05-23 09:27:00.000000 django-beam-1.4.1/src/django_beam.egg-info/PKG-INFO
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4077 2023-05-23 09:27:00.000000 django-beam-1.4.1/src/django_beam.egg-info/SOURCES.txt
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        1 2023-05-23 09:27:00.000000 django-beam-1.4.1/src/django_beam.egg-info/dependency_links.txt
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)       88 2023-05-23 09:27:00.000000 django-beam-1.4.1/src/django_beam.egg-info/requires.txt
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        5 2023-05-23 09:27:00.000000 django-beam-1.4.1/src/django_beam.egg-info/top_level.txt
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-05-23 09:27:00.422086 django-beam-1.4.1/tests/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    15449 2022-04-27 09:12:32.000000 django-beam-1.4.1/tests/test_actions.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2782 2023-01-11 09:59:58.000000 django-beam-1.4.1/tests/test_components.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    14309 2023-01-23 10:38:56.000000 django-beam-1.4.1/tests/test_contrib_auth.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2040 2022-04-27 09:12:32.000000 django-beam-1.4.1/tests/test_contrib_autocomplete.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    10694 2023-04-27 06:08:23.000000 django-beam-1.4.1/tests/test_contrib_reversion.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      850 2022-04-27 09:12:32.000000 django-beam-1.4.1/tests/test_inlines.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2022-04-27 09:12:32.000000 django-beam-1.4.1/tests/test_layouts.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1849 2022-04-27 09:12:32.000000 django-beam-1.4.1/tests/test_registry.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3284 2023-05-17 08:50:04.000000 django-beam-1.4.1/tests/test_tags.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4771 2023-01-11 09:59:58.000000 django-beam-1.4.1/tests/test_urls.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3946 2023-01-11 09:59:58.000000 django-beam-1.4.1/tests/test_utils.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    31258 2023-03-30 10:35:40.000000 django-beam-1.4.1/tests/test_views.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4275 2022-04-27 09:12:32.000000 django-beam-1.4.1/tests/test_viewsets.py
```

### Comparing `django-beam-1.4.0/LICENSE` & `django-beam-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/PKG-INFO` & `django-beam-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-beam
-Version: 1.4.0
+Version: 1.4.1
 Summary: A crud library for python
 Home-page: https://github.com/django-beam/django-beam
-Download-URL: https://github.com/django-beam/django-beam/archive/1.4.0.tar.gz
+Download-URL: https://github.com/django-beam/django-beam/archive/1.4.1.tar.gz
 Author: Raphael Kimmig
 Author-email: raphael@ampad.de
 License: BSD 3-Clause License
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `django-beam-1.4.0/README.md` & `django-beam-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/setup.cfg` & `django-beam-1.4.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [metadata]
 name = django-beam
-version = 1.4.0
+version = 1.4.1
 description = A crud library for python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/django-beam/django-beam
-download_url = https://github.com/django-beam/django-beam/archive/1.4.0.tar.gz
+download_url = https://github.com/django-beam/django-beam/archive/1.4.1.tar.gz
 author = Raphael Kimmig
 author_email = raphael@ampad.de
 keywords = 
 license = BSD 3-Clause License
 classifiers = 
 	Framework :: Django
 	Programming Language :: Python :: 3
```

### Comparing `django-beam-1.4.0/src/beam/actions.py` & `django-beam-1.4.1/src/beam/actions.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/components.py` & `django-beam-1.4.1/src/beam/components.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/contrib/auth/forms.py` & `django-beam-1.4.1/src/beam/contrib/auth/forms.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/contrib/auth/templates/registration/login.html` & `django-beam-1.4.1/src/beam/contrib/auth/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/contrib/auth/templates/registration/password_change_form.html` & `django-beam-1.4.1/src/beam/contrib/auth/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/contrib/auth/templates/registration/password_reset_confirm.html` & `django-beam-1.4.1/src/beam/contrib/auth/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/contrib/auth/templates/registration/password_reset_done.html` & `django-beam-1.4.1/src/beam/contrib/auth/templates/registration/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/contrib/auth/templates/registration/password_reset_email.html` & `django-beam-1.4.1/src/beam/contrib/auth/templates/registration/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/contrib/auth/templates/registration/password_reset_form.html` & `django-beam-1.4.1/src/beam/contrib/auth/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/contrib/auth/views.py` & `django-beam-1.4.1/src/beam/contrib/auth/views.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/contrib/autocomplete_light/__init__.py` & `django-beam-1.4.1/src/beam/contrib/autocomplete_light/__init__.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/contrib/autocomplete_light/static/autocomplete_light/select2.css` & `django-beam-1.4.1/src/beam/contrib/autocomplete_light/static/autocomplete_light/select2.css`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/contrib/reversion/templates/beam_reversion/version_detail.html` & `django-beam-1.4.1/src/beam/contrib/reversion/templates/beam_reversion/version_detail.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/contrib/reversion/templates/beam_reversion/version_list.html` & `django-beam-1.4.1/src/beam/contrib/reversion/templates/beam_reversion/version_list.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/contrib/reversion/views.py` & `django-beam-1.4.1/src/beam/contrib/reversion/views.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/contrib/reversion/viewsets.py` & `django-beam-1.4.1/src/beam/contrib/reversion/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/inlines.py` & `django-beam-1.4.1/src/beam/inlines.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/layouts.py` & `django-beam-1.4.1/src/beam/layouts.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/locale/de/LC_MESSAGES/django.mo` & `django-beam-1.4.1/src/beam/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/registry.py` & `django-beam-1.4.1/src/beam/registry.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/templatetags/beam_tags.py` & `django-beam-1.4.1/src/beam/templatetags/beam_tags.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/themes/bootstrap4/static/beam/css/bootstrap-select.min.css` & `django-beam-1.4.1/src/beam/themes/bootstrap4/static/beam/css/bootstrap-select.min.css`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/themes/bootstrap4/static/beam/js/actions.js` & `django-beam-1.4.1/src/beam/themes/bootstrap4/static/beam/js/actions.js`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/themes/bootstrap4/static/beam/js/add_related.js` & `django-beam-1.4.1/src/beam/themes/bootstrap4/static/beam/js/add_related.js`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/themes/bootstrap4/static/beam/js/bootstrap-select.min.js` & `django-beam-1.4.1/src/beam/themes/bootstrap4/static/beam/js/bootstrap-select.min.js`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/themes/bootstrap4/static/beam/js/inlines.js` & `django-beam-1.4.1/src/beam/themes/bootstrap4/static/beam/js/inlines.js`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/themes/bootstrap4/static/beam/js/sortable.min.js` & `django-beam-1.4.1/src/beam/themes/bootstrap4/static/beam/js/sortable.min.js`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/base.html` & `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/base.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/dashboard.html` & `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/dashboard.html`

 * *Files 2% similar despite different names*

```diff
@@ -5,36 +5,34 @@
 
 {% block title %}{% trans "Dashboard" %} | {{ block.super }}{% endblock %}
 
 
 {% block content %}
     {% for entry in grouped_by_app %}
         <section>
-            <div class="container">
-                <h2>{{ entry.app_config.verbose_name|capfirst }}</h2>
-                <div class="card-columns">
-                {% for viewset, links in entry.viewsets %}
-                    <div class="card">
-                        <div class="card-header">
-                            {% get_options viewset.model as options %}
-                            <h3 class="card-title">{{ options.verbose_name_plural|capfirst }}</h3>
-                        </div>
-                        <div class="card-body">
-                            {% for link in links %}
-                                <a class="btn btn-{% if link.name == 'list' %}primary{% else %}secondary{% endif %}" href="{{ link.reverse }}">
-                                    {{ link.verbose_name|capfirst }}
-                                </a>
-                            {% endfor %}
-                        </div>
+            <h2>{{ entry.app_config.verbose_name|capfirst }}</h2>
+            <div class="card-columns">
+            {% for viewset, links in entry.viewsets %}
+                <div class="card">
+                    <div class="card-header">
+                        {% get_options viewset.model as options %}
+                        <h3 class="card-title">{{ options.verbose_name_plural|capfirst }}</h3>
+                    </div>
+                    <div class="card-body">
+                        {% for link in links %}
+                            <a class="btn btn-{% if link.name == 'list' %}primary{% else %}secondary{% endif %}" href="{{ link.reverse }}">
+                                {{ link.verbose_name|capfirst }}
+                            </a>
+                        {% endfor %}
                     </div>
-                {% endfor %}
                 </div>
+            {% endfor %}
             </div>
         </section>
-        {% empty %}
+    {% empty %}
         {% if not request.user.is_authenticated %}
             <p>
             {% trans "You don't have permission to view anything, try logging in."  %}
             </p>
             {% url 'login' as login_url %}
             {% if login_url %}
                 <a href="{{ login_url }}">{% trans "Log in" %}</a>
```

### Comparing `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/delete.html` & `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/delete.html`

 * *Files 2% similar despite different names*

```diff
@@ -16,47 +16,45 @@
     {% endif %}
     | {{ block.super }}
 {% endblock %}
 
 
 {% block content %}
     <section class="beam-main">
-        <div class="container">
-            {% block heading_container %}
-                <h1>
-                    {% block heading %}
-                        {% if heading %}
-                            {{ heading }}
-                        {% else %}
-                            {% get_options component.model as options %}
-                            {% blocktrans %}Delete {{ object }}{% endblocktrans %}
-                            <small class="text-muted">{{ options.verbose_name|capfirst }}</small>
-                        {% endif %}
-                    {% endblock %}
-                </h1>
-            {% endblock %}
+        {% block heading_container %}
+            <h1>
+                {% block heading %}
+                    {% if heading %}
+                        {{ heading }}
+                    {% else %}
+                        {% get_options component.model as options %}
+                        {% blocktrans %}Delete {{ object }}{% endblocktrans %}
+                        <small class="text-muted">{{ options.verbose_name|capfirst }}</small>
+                    {% endif %}
+                {% endblock %}
+            </h1>
+        {% endblock %}
 
-            {% if protected_objects %}
+        {% if protected_objects %}
 
-                <p>
-                    {% blocktrans with object_name=object_name %}You can't delete <em>{{ object_name }}</em> because the following objects depend on it:{% endblocktrans %}
-                </p>
-                <ul>{{ protected_objects|unordered_list }}</ul>
+            <p>
+                {% blocktrans with object_name=object_name %}You can't delete <em>{{ object_name }}</em> because the following objects depend on it:{% endblocktrans %}
+            </p>
+            <ul>{{ protected_objects|unordered_list }}</ul>
 
-            {% else %}
-                <p>
-                    {% blocktrans with object_name=object_name %}Are you sure you want to delete <em>{{ object_name }}</em>?{% endblocktrans %}
-                </p>
-                {% if nested_objects|length > 1 %}
-                <p>{%trans "The following objects will also be deleted:" %}</p>
-                <ul>{{ nested_objects|unordered_list }}</ul>
-                {% endif %}
-                <form method="post">
-                    {% csrf_token %}
-                    {{ form.as_p }}
-                    <button type="submit" class="btn btn-danger float-left">{% trans "Yes, I'm sure" %}</button>
-                </form>
-                <button class="btn btn-default float-left" onclick="window.history.back()">{% trans "No, go back." %}</button>
+        {% else %}
+            <p>
+                {% blocktrans with object_name=object_name %}Are you sure you want to delete <em>{{ object_name }}</em>?{% endblocktrans %}
+            </p>
+            {% if nested_objects|length > 1 %}
+            <p>{%trans "The following objects will also be deleted:" %}</p>
+            <ul>{{ nested_objects|unordered_list }}</ul>
             {% endif %}
-        </div>
+            <form method="post">
+                {% csrf_token %}
+                {{ form.as_p }}
+                <button type="submit" class="btn btn-danger float-left">{% trans "Yes, I'm sure" %}</button>
+            </form>
+            <button class="btn btn-default float-left" onclick="window.history.back()">{% trans "No, go back." %}</button>
+        {% endif %}
     </section>
 {% endblock %}
```

### Comparing `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/detail.html` & `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/detail.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/form.html` & `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/form.html`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
                             {% endif %}
                         {% endblock %}
                     </h1>
                 {% endblock %}
 
                 {% block form_buttons_top_container %}
                     <div class="beam-form__buttons-top clearfix">
-                        <div class="btn-group float-right mb-2">
+                        <div class="btn-group float-right mb-3">
                             {% block form_buttons_top %}
                                 <button type="submit" class="btn btn-primary">{% trans "Save" %}</button>
                             {% endblock %}
                         </div>
                     </div>
                 {% endblock %}
```

### Comparing `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/list.html` & `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/list.html`

 * *Files 1% similar despite different names*

```diff
@@ -18,144 +18,152 @@
     | {{ block.super }}
 {% endblock %}
 
 
 {% block content %}
     {% get_options component.model as options %}
     <section class="beam-main">
-        <div class="container">
-            {% block links_container %}
-                <div class="float-right beam-links">
-                    {% block links %}
-                        {% include "beam/partials/links.html" with links=viewset.links link_layout=component.link_layout %}
-                    {% endblock %}
-                </div>
-            {% endblock %}
-            {% block heading_container %}
-                <h1>
-                    {% block heading %}
-                        {% if heading %}
-                            {{ heading }}
-                        {% else %}
-                            {{ options.verbose_name_plural|capfirst }}
-                        {% endif %}
-                    {% endblock %}
-                </h1>
-            {% endblock %}
+        {% block links_container %}
+            <div class="float-right beam-links">
+                {% block links %}
+                    {% include "beam/partials/links.html" with links=viewset.links link_layout=component.link_layout %}
+                {% endblock %}
+            </div>
+        {% endblock %}
+        {% block heading_container %}
+            <h1>
+                {% block heading %}
+                    {% if heading %}
+                        {{ heading }}
+                    {% else %}
+                        {{ options.verbose_name_plural|capfirst }}
+                    {% endif %}
+                {% endblock %}
+            </h1>
+        {% endblock %}
 
-            {% block search %}
-                {% if view.search_fields %}
-                    <form method="get" id="search-form">
-                        <div class="input-group">
-                            <input name="q" type="text" value="{{ search_query }}" class="form-control"
-                                   placeholder="{% trans 'Search the list below' %}"
-                                   aria-label="{% trans 'Search the list below' %}"
-                                   aria-describedby="search-form-input">
-                            <div class="input-group-append">
-
-                                {% if search_query %}
-                                    <a href="{{ request.path }}"
-                                       class="btn btn-outline-secondary">{% trans "Clear" %}</a>
-                                {% endif %}
-                                <input type="submit" class="btn btn-outline-primary" value="{% trans 'Search' %}"/>
-                            </div>
+        {% block search %}
+            {% if view.search_fields %}
+                <form method="get" id="search-form">
+                    <div class="input-group">
+                        <input name="q" type="text" value="{{ search_query }}" class="form-control"
+                               placeholder="{% trans 'Search the list below' %}"
+                               aria-label="{% trans 'Search the list below' %}"
+                               aria-describedby="search-form-input">
+                        <div class="input-group-append">
+
+                            {% if search_query %}
+                                <a href="{{ request.path }}"
+                                   class="btn btn-outline-secondary">{% trans "Clear" %}</a>
+                            {% endif %}
+                            <input type="submit" class="btn btn-outline-primary" value="{% trans 'Search' %}"/>
                         </div>
-                    </form>
-                {% endif %}
-            {% endblock %}
-            {% block filters %}
-                {% include "beam/partials/filters.html" %}
-            {% endblock %}
-
-            {% if actions %}
-            <form method="post" id="list-action-form" novalidate>
-                {% csrf_token %}
-                {% block actions %}
-                    {% include "beam/partials/actions.html" %}
-                {% endblock %}
+                    </div>
+                </form>
             {% endif %}
-
-            {% block table %}
-                <table class="table table-striped beam-list-table">
-                    {% block table_head %}
-                    <thead>
+        {% endblock %}
+        {% block filters %}
+            {% include "beam/partials/filters.html" %}
+        {% endblock %}
+
+        {% if actions %}
+        <form method="post" id="list-action-form" novalidate>
+            {% csrf_token %}
+            {% block actions %}
+                {% include "beam/partials/actions.html" %}
+            {% endblock %}
+        {% endif %}
+
+        {% block table %}
+            <div class="table-responsive">
+            <table class="table table-striped border-bottom beam-list-table">
+                {% block table_head %}
+                <thead>
+                <tr>
+                    {% if actions %}
+                    <th>
+                        <input class="beam-action__select-across" name="_action_select_across" type="hidden" value="">
+                        <input title="{% trans "Select all" %}" class="beam-action__select-all" type="checkbox">
+                    </th>
+                    {% endif %}
+                    {% for field in component.fields %}
+                        <th scope="col" class="beam-list-field-label beam-field-label-{{ field }}">
+                            {% with field_name=field|stringformat:"s" %}{# cast to string to support virtual fields #}
+                                {% if field_name in sortable_fields %}
+                                    {# fixme text-nowrap only if there is a chance to fit this?  #}
+                                    <a class="text-nowrap" href="{% sort_link field_name sorted_fields %}">
+                                        {{ component.model|field_verbose_name:field|capfirst }}&nbsp;{% if field_name in sorted_fields %}<i class="fa fa-caret-up"></i>{% elif "-"|add:field_name in sorted_fields %}<i class="fa fa-caret-down"></i>{% endif %}
+                                    </a>
+                                    {% if field_name in sorted_fields or "-"|add:field_name in sorted_fields %}
+                                        <a title="{% trans "reset sort" %}" href="{% sort_link "" "" %}"><i class="fa fa-remove"></i></a>
+                                    {% endif %}
+                                {% else %}
+                                    {{ component.model|field_verbose_name:field|capfirst }}
+                                {% endif %}
+                            {% endwith %}
+                        </th>
+                    {% endfor %}
+                    {% if component.list_item_link_layout %}
+                    <th>{% trans "Actions" %}</th>
+                    {% endif %}
+                </tr>
+                </thead>
+                    {% endblock %}
+                <tbody>
+                {% for object in object_list %}
                     <tr>
                         {% if actions %}
-                        <th>
-                            <input class="beam-action__select-across" name="_action_select_across" type="hidden" value="">
-                            <input title={% trans "Select all" %} class="beam-action__select-all" type="checkbox">
-                        </th>
+                        <td class="beam-list-action-checkbox">
+                            <input type="checkbox" class="beam-action__select-item" name="_action_select[]"
+                                   value="{{ object.pk }}">
+                        </td>
                         {% endif %}
                         {% for field in component.fields %}
-                            <th scope="col" class="beam-list-field-label beam-field-label-{{ field }}">
-                                {% with field_name=field|stringformat:"s" %}{# cast to string to support virtual fields #}
-                                    {% if field_name in sortable_fields %}
-                                        {# fixme text-nowrap only if there is a chance to fit this?  #}
-                                        <a class="text-nowrap" href="{% sort_link field_name sorted_fields %}">
-                                            {{ component.model|field_verbose_name:field|capfirst }}&nbsp;{% if field_name in sorted_fields %}<i class="fa fa-caret-up"></i>{% elif "-"|add:field_name in sorted_fields %}<i class="fa fa-caret-down"></i>{% endif %}
-                                        </a>
-                                        {% if field_name in sorted_fields or "-"|add:field_name in sorted_fields %}
-                                            <a title="{% trans "reset sort" %}" href="{% sort_link "" "" %}"><i class="fa fa-remove"></i></a>
-                                        {% endif %}
-                                    {% else %}
-                                        {{ component.model|field_verbose_name:field|capfirst }}
-                                    {% endif %}
-                                {% endwith %}
-                            </th>
+                            <td class="beam-list-field beam-field-{{ field }}">
+                                {% include "beam/partials/detail_field.html" with object=object field=field %}
+                            </td>
                         {% endfor %}
-                        {% if component.list_item_link_layout %}
-                        <th>{% trans "Actions" %}</th>
-                        {% endif %}
-                    </tr>
-                    </thead>
-                        {% endblock %}
-                    <tbody>
-                    {% for object in object_list %}
-                        <tr>
-                            {% if actions %}
-                            <td class="beam-list-action-checkbox">
-                                <input type="checkbox" class="beam-action__select-item" name="_action_select[]"
-                                       value="{{ object.pk }}">
+                        {% block list_item_links %}
+                            {% if component.list_item_link_layout %}
+                            <td class="beam-list-item-links">
+                                {% include "beam/partials/list_links.html" with links=viewset.links link_layout=component.list_item_link_layout object=object %}
                             </td>
                             {% endif %}
-                            {% for field in component.fields %}
-                                <td class="beam-list-field beam-field-{{ field }}">
-                                    {% include "beam/partials/detail_field.html" with object=object field=field %}
-                                </td>
-                            {% endfor %}
-                            {% block list_item_links %}
-                                {% if component.list_item_link_layout %}
-                                <td class="pt-2">
-                                    {% include "beam/partials/list_links.html" with links=viewset.links link_layout=component.list_item_link_layout object=object %}
-                                </td>
-                                {% endif %}
-                            {% endblock %}
-                        </tr>
-                    {% endfor %}
-                    </tbody>
-                </table>
-            {% endblock %}
+                        {% endblock %}
+                    </tr>
+                {% endfor %}
+                </tbody>
+            </table>
+            </div>
+        {% endblock %}
+
+        {% block no_results %}
+            {% if not object_list %}
+                <p class="alert alert-info" role="alert">
+                    {% if search_query %}
+                        {% blocktrans with name=options.verbose_name_plural %}Could not find any {{ name }} for query "{{ search_query }}"{% endblocktrans %}.
+                    {% elif filterset and filterset.is_bound and filterset.is_valid %}
+                        {% blocktrans with name=options.verbose_name_plural %}Could not find any {{ name }} that match the current filters{% endblocktrans %}.
+                    {% else %}
+                        {% blocktrans with name=options.verbose_name_plural %}Could not find any {{ name }}{% endblocktrans %}.
+                    {% endif %}
+                </p>
+            {% endif %}
+        {% endblock %}
 
-            {% block no_results %}
-                {% if not object_list %}
-                    <p class="alert alert-info" role="alert">
-                        {% if search_query %}
-                            {% blocktrans with name=options.verbose_name_plural %}Could not find any {{ name }} for query "{{ search_query }}"{% endblocktrans %}.
-                        {% elif filterset and filterset.is_bound and filterset.is_valid %}
-                            {% blocktrans with name=options.verbose_name_plural %}Could not find any {{ name }} that match the current filters{% endblocktrans %}.
-                        {% else %}
-                            {% blocktrans with name=options.verbose_name_plural %}Could not find any {{ name }}{% endblocktrans %}.
-                        {% endif %}
-                    </p>
-                {% endif %}
-            {% endblock %}
+        {% block pagination_container %}
+            <div class="row mb-4">
+                <div class="col-sm-9">
+                    {% block pagination %}
+                        {% include "beam/partials/pagination.html" with page_param=view.page_kwarg %}
+                    {% endblock %}
+                </div>
+            </div>
+        {% endblock %}
 
-            {% block pagination %}
-                {% include "beam/partials/pagination.html" with page_param=view.page_kwarg %}
-            {% endblock %}
 
-            {% if actions %}
-            </form>
-            {% endif %}
-        </div>
+
+        {% if actions %}
+        </form>
+        {% endif %}
     </section>
 {% endblock %}
```

#### html2text {}

```diff
@@ -5,31 +5,30 @@
 { block.super }}{{ filterset.form.media.js }}{% for action in actions %}{
 { action.get_form.media.js }}{% endfor %}{% endblock %} {% block extra_styles
 %}{{ block.super }}{{ filterset.form.media.css }}{% for action in actions %}{
 { action.get_form.media.css }}{% endfor %}{% endblock %} {% block title %} {%
 if heading %} {{ heading }} {% else %} {% get_options component.model as
 options %} {{ options.verbose_name_plural|capfirst }} {% endif %} | {
 { block.super }} {% endblock %} {% block content %} {% get_options
-component.model as options %}
-{% block links_container %}
+component.model as options %}  {% block links_container %}
 {% block links %} {% include "beam/partials/links.html" with
 links=viewset.links link_layout=component.link_layout %} {% endblock %}
 {% endblock %} {% block heading_container %}
 ****** {% block heading %} {% if heading %} {{ heading }} {% else %} {
 { options.verbose_name_plural|capfirst }} {% endif %} {% endblock %} ******
 {% endblock %} {% block search %} {% if view.search_fields %}
 [{{ search_query }}  ]
 {% if search_query %} {%_trans_"Clear"_%} {% endif %} [{% trans 'Search' %}]
 {% endif %} {% endblock %} {% block filters %} {% include "beam/partials/
 filters.html" %} {% endblock %} {% if actions %}
 {% csrf_token %} {% block actions %} {% include "beam/partials/actions.html" %}
 {% endblock %} {% endif %} {% block table %}
                  {% with field_name=field|stringformat:"s" %}{# cast to string to support
                  virtual fields #} {% if field_name in sortable_fields %} {# fixme text-
-Select all" %}   nowrap only if there is a chance to fit this? #}
+ %}"             nowrap only if there is a chance to fit this? #}
 class="beam-     {{_component.model|field_verbose_name:field|capfirst_}} {%_if_field_name_in
 action__select-  sorted_fields_%}{%_elif_"-"|add:field_name_in_sorted_fields_%}{%_endif_%}    {% trans "Actions" %}
 all"              {% if field_name in sorted_fields or "-"|add:field_name in sorted_fields %}
 type="checkbox">  %}" href="{% sort_link "" "" %}">
                   {% endif %} {% else %} {{ component.model|field_verbose_name:field|capfirst
                  }} {% endif %} {% endwith %}
                                                                                               {% include "beam/partials/list_links.html"
@@ -40,12 +39,12 @@
 {% if search_query %} {% blocktrans with name=options.verbose_name_plural
 %}Could not find any {{ name }} for query "{{ search_query }}"{% endblocktrans
 %}. {% elif filterset and filterset.is_bound and filterset.is_valid %} {%
 blocktrans with name=options.verbose_name_plural %}Could not find any {{ name
 }} that match the current filters{% endblocktrans %}. {% else %} {% blocktrans
 with name=options.verbose_name_plural %}Could not find any {{ name }}{%
 endblocktrans %}. {% endif %}
-{% endif %} {% endblock %} {% block pagination %} {% include "beam/partials/
-pagination.html" with page_param=view.page_kwarg %} {% endblock %} {% if
-actions %}
-{% endif %}
- {% endblock %}
+{% endif %} {% endblock %} {% block pagination_container %}
+{% block pagination %} {% include "beam/partials/pagination.html" with
+page_param=view.page_kwarg %} {% endblock %}
+{% endblock %} {% if actions %}
+{% endif %}  {% endblock %}
```

### Comparing `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/actions.html` & `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/actions.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {% load i18n %}
-<div class="beam-action border mb-2 p-4">
+<div class="beam-action mb-3 mt-3">
     <div class="form-inline">
         <label>
             {% trans "Action" %}
             <select name="_action_choice" class="form-control ml-2 mr-2 beam-action__choice">
                 <option value="_no_action_selected">--------</option>
                 {% for action in actions %}
                     <option value="{{ action.id }}" {% if action.is_bound %}selected="selected"{% endif %}>{{ action.verbose_name }}</option>
```

### Comparing `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/detail_field.html` & `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/detail_field.html`

 * *Files 13% similar despite different names*

```diff
@@ -47,15 +47,19 @@
                 &nbsp;
             {% endif %}
         {% endblock %}
 
     {% elif value|is_bool %}
 
         {% block bool %}
-            {{ value|yesno }}
+            {% if value %}
+                <i class="fa fa-check text-success" title="{% trans "yes"|capfirst %}"></i>
+            {% else %}
+                <i class="fa fa-times" title="{% trans "no"|capfirst %}"></i>
+            {% endif %}
         {% endblock %}
 
     {% elif value|is_int %}
 
         {% block int %}
             {{ value }}
         {% endblock %}
```

#### html2text {}

```diff
@@ -5,13 +5,16 @@
 {_related_}}{% else %}{{ related }}{% endif %}{% if not forloop.last %}, {%
 endif %} {% empty %}   {% endfor %} {% endblock %} {% elif value.pk %} {% block
 foreign_key %} {% get_url_for_related value "detail" as related_url %} {% if
 related_url %} {{_value_}} {% else %} {{ value }} {% endif %} {% endblock %} {%
 elif value|is_image %} {% block image %} {% if value %} [{{ value.url }}] {%
 else %}   {% endif %} {% endblock %} {% elif value|is_file %} {% block file %}
 {% if value %} {%_trans_"download"_%} {% else %}   {% endif %} {% endblock %}
-{% elif value|is_bool %} {% block bool %} {{ value|yesno }} {% endblock %} {%
-elif value|is_int %} {% block int %} {{ value }} {% endblock %} {% elif
-value|is_float %} {% block float %} {{ value }} {% endblock %} {% elif
-value|is_decimal %} {% block decimal %} {{ value }} {% endblock %} {% else %}
-{% block else %} {{ value|default:" " }} {% endblock %} {% endif %} {% endblock
-%} {% endblock %}
+{% elif value|is_bool %} {% block bool %} {% if value %}
+|capfirst %}">
+ {% else %}
+|capfirst %}">
+ {% endif %} {% endblock %} {% elif value|is_int %} {% block int %} {{ value }}
+{% endblock %} {% elif value|is_float %} {% block float %} {{ value }} {%
+endblock %} {% elif value|is_decimal %} {% block decimal %} {{ value }} {%
+endblock %} {% else %} {% block else %} {{ value|default:" " }} {% endblock %}
+{% endif %} {% endblock %} {% endblock %}
```

### Comparing `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline.html` & `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline.html`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
                 {% block actions %}
                     {% include "beam/partials/actions.html" %}
                 {% endblock %}
             {% endif %}
         {% endblock %}
 
         {% block inline_group_container %}
-        <div class="card mb-4">
+        <div class="card mb-3">
             <ul class="list-group list-group-flush mb-0">
             {% block inline_group %}
 
                 {% block inline_group_head %}
                     {% if actions %}
                         <li class="list-group-item">
                             {% block select_all %}
@@ -87,16 +87,22 @@
                 {% endblock %}
 
             {% endblock %}
             </ul>
         </div>
         {% endblock %}
 
-        {% block pagination %}
-            {% include "beam/partials/pagination.html" with page_param=inline.page_param paginator=page.paginator is_paginated=page.has_other_pages page_obj=page page_number=page.number object_list=page.object_list options=inline.model_options %}
+        {% block pagination_container %}
+            <div class="row mb-4">
+                <div class="col-sm-9">
+                    {% block pagination %}
+                        {% include "beam/partials/pagination.html" with page_param=inline.page_param paginator=page.paginator is_paginated=page.has_other_pages page_obj=page page_number=page.number object_list=page.object_list options=inline.model_options %}
+                    {% endblock %}
+                </div>
+            </div>
         {% endblock %}
 
         {% block actions_container_end %}
             {% if actions %}
                 </form>
             {% endif %}
         {% endblock %}
```

### Comparing `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline_tabular.html` & `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline_tabular.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {% extends "beam/partials/detail_inline.html" %}
 {% load i18n %}
 {% load beam_tags %}
 
 
 {% block inline_group_container %}
     <div class="table-responsive">
-    <table class="table table-sm table-striped" id="{{ inline.prefix }}-table">
+    <table class="table table-sm table-striped border-bottom" id="{{ inline.prefix }}-table">
         {% block inline_group %}
             {% block inline_group_head %}
             <thead>
                 <tr>
                     {% if actions %}
                         <th scope="col">
                             {% block select_all %}{{ block.super }}{% endblock %}
```

### Comparing `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/filters.html` & `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/filters.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/form_field.html` & `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/form_field.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 {% load crispy_forms_tags crispy_forms_field %}
+
+
 {# work around because we don't render the label using crispy #}
 {% if form_field|is_checkbox %}
     <div class="form-group form-check pt-1">
-    {% if field.errors %}
-        {% crispy_field form_field 'class' 'form-check-input is-invalid' %}
-    {% else %}
-        {% crispy_field form_field 'class' 'form-check-input' %}
-    {% endif %}
+        {% if field.errors %}
+            {% crispy_field form_field 'class' 'form-check-input is-invalid' %}
+        {% else %}
+            {% crispy_field form_field 'class' 'form-check-input' %}
+        {% endif %}
     </div>
 {% else %}
-{# fall back to crispy forms default tempalte #}
-{% include "bootstrap4/field.html" with field=form_field form_show_errors=True %}
+    {# fall back to crispy forms default tempalte #}
+    {% include "bootstrap4/field.html" with field=form_field form_show_errors=True wrapper_class="mb-0" %}
 {% endif %}
```

### Comparing `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/form_inline.html` & `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/form_inline.html`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                         {% endblock %}
                     </ul>
                 </div>
             {% endif %}
         {% endblock %}
 
         {% block inline_group_container %}
-        <div class="card mb-4">
+        <div class="card mb-3">
             <ul class="related-inline-group list-group list-group-flush mb-0">
 
                 {% block inline_group %}
                 {% for form in inline.formset %}
 
                     {% block inline_item_container %}
                     <li data-inline-id="{{ forloop.counter0 }}" id="{{ inline.prefix }}-{{ forloop.counter0 }}"
@@ -71,15 +71,15 @@
                             {% endif %}
                             {% endblock %}
 
                             {% block delete_container %}
                             {% if inline.formset.can_delete %}
                                 {% block delete %}
                                 <button class="btn btn-outline-danger related-inline-item-remove d-none float-right">
-                                    {% trans "delete" %}
+                                    {% trans "delete"|capfirst %}
                                 </button>
                                 {% endblock %}
                             {% endif %}
                             {% endblock %}
 
                             {% block inline_layout %}
                                 {% include "beam/partials/form_layout.html" with form=form fields=inline.fields layout=inline.layout %}
@@ -102,39 +102,43 @@
                         <div class="field-group float-left">
                             {% get_form_field inline.formset.empty_form inline.order_field as order_field %}
                             <div class="d-none">{{ order_field }}</div>
                         </div>
                     {% endif %}
                     {% if inline.formset.can_delete %}
                         <button class="btn btn-outline-danger related-inline-item-remove float-right d-none">
-                            {% trans "delete" %}</button>
+                            {% trans "delete"|capfirst %}
+                        </button>
                     {% endif %}
                     {% include "beam/partials/form_layout.html" with form=inline.formset.empty_form fields=inline.fields layout=inline.layout %}
                 </li>
                 {% endblock %}
             </ul>
         </div>
         {% endblock %}
 
-        {% block add_form %}
-            <div class="container-fluid mb-2">
-                <div class="row">
-                    <div class="btn-group ml-auto">
-                        {% block inline_add_button %}
-                            {% get_options inline.formset.model as inline_options %}
-                            <button class="btn btn-outline-primary related-inline-item-add d-none">
-                                {% blocktrans with name=inline_options.verbose_name %}add {{ name }}{% endblocktrans %}
-                            </button>
-                        {% endblock %}
-                    </div>
+        {% block pagination_and_add_form_container %}
+            <div class="row align-items-center mb-4">
+                <div class="col-sm-9">
+                    {% block pagination %}
+                        {% include "beam/partials/pagination.html" with page_param=inline.page_param paginator=page.paginator is_paginated=page.has_other_pages page_obj=page page_number=page.number object_list=page.object_list options=inline.model_options %}
+                    {% endblock %}
+                </div>
+                <div class="col-sm-3">
+                    {% block add_form %}
+                        <div class="btn-group float-right">
+                            {% block inline_add_button %}
+                                {% get_options inline.formset.model as inline_options %}
+                                <button class="btn btn-outline-primary related-inline-item-add d-none">
+                                    {% blocktrans with name=inline_options.verbose_name %}add {{ name }}{% endblocktrans %}
+                                </button>
+                            {% endblock %}
+                        </div>
+                    {% endblock %}
                 </div>
             </div>
         {% endblock %}
 
-        {% block pagination %}
-            {% include "beam/partials/pagination.html" with page_param=inline.page_param paginator=page.paginator is_paginated=page.has_other_pages page_obj=page page_number=page.number object_list=page.object_list options=inline.model_options %}
-        {% endblock %}
-
     {% endblock %}
 </section>
 {% endwith %}
 {% endblock %}
```

### Comparing `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular.html` & `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {% extends "beam/partials/form_inline.html" %}
 {% load i18n %}
 {% load beam_tags %}
 
 
 {% block inline_group_container %}
     <div class="table-responsive">
-    <table class="table table-sm table-striped" id="{{ inline.prefix }}-table">
+    <table class="table table-sm table-striped border-bottom" id="{{ inline.prefix }}-table">
         {% block inline_group %}
 
             {% block inline_group_head %}
             <thead>
                 <tr>
                     {% if inline.can_order %}<th scope="col"></th>{% endif %}
```

### Comparing `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular_row.html` & `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular_row.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/form_layout.html` & `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/form_layout.html`

 * *Files 7% similar despite different names*

```diff
@@ -23,28 +23,28 @@
                 {% block fields %}
                 {% for field in col %}
 
                     {% block field %}
                     {% if field.is_html %}
 
                         {% block html_field_container %}
-                        <div class="beam-field beam-html-field beam-field-{{ field.name|default:"html" }}">
+                        <div class="beam-field mb-3 beam-html-field beam-field-{{ field.name|default:"html" }}">
                             {% block html_field %}
                                 {{ field.content|safe }}
                             {% endblock %}
                         </div>
                         {% endblock %}
 
                     {% else %}
 
                         {% get_form_field form field as form_field %}
                         {% if form_field is None %}
 
                             {% block detail_field_container %}
-                            <div class="row">
+                            <div class="row field-group mb-3">
                                 <div class="col-sm-4 text-md-right beam-field-label beam-detail-field-label beam-field-label-{{ field }} ">
 
                                     {% block detail_field_label %}
                                         <label>
                                             {{ form.instance|field_verbose_name:field|capfirst }}
                                         </label>
                                     {% endblock %}
@@ -62,20 +62,22 @@
 
                         {% elif not form_field.is_hidden %}
 
                             {% get_url_for_related form_field.field.queryset.model "create" as create_url %}
                             {% get_options form_field.field.queryset.model as related_options %}
 
                             {% block form_field_container %}
-                            <div class="row field-group">
+                            <div class="row field-group mb-3">
                                 <div class="col-sm-4 text-md-right beam-field-label beam-form-field-label beam-field-label-{{ field }}">
 
                                     {% block form_field_label %}
-                                        <label class="col-form-label" for="{{ form_field.auto_id }}">
-                                            {{ form_field.label }}<span class="text-muted small">{% if form_field.field.required %}*{% else %}&nbsp;{% endif %}</span>
+                                        <label class="col-form-label {% if form_field.field.required %}required-field{% endif %}"
+                                               for="{{ form_field.auto_id }}"
+                                               {% if form_field.field.required %}title="{% trans "This field is required." %}"{% endif %}>
+                                            {{ form_field.label }}{% if form_field.field.required %}<span class="asterisk-field">*</span>{% else %}&nbsp;{% endif %}
                                         </label>
                                     {% endblock %}
 
                                 </div>
 
                                 <div class="col-sm-8 beam-field beam-form-field beam-field-{{ field }}"
                                         {% if create_url %}
```

### Comparing `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/layout.html` & `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/layout.html`

 * *Files 2% similar despite different names*

```diff
@@ -19,25 +19,25 @@
                 {% block fields %}
                 {% for field in col %}
 
                     {% block field %}
                     {% if field.is_html %}
 
                         {% block html_field_container %}
-                        <div class="beam-field beam-html-field beam-field-{{ field.name|default:"html" }}">
+                        <div class="beam-field mb-3 beam-html-field beam-field-{{ field.name|default:"html" }}">
                             {% block html_field %}
                                 {{ field.content|safe }}
                             {% endblock %}
                         </div>
                         {% endblock %}
 
                     {% else %}
 
                         {% block detail_field_container %}
-                        <div class="row">
+                        <div class="row field-group mb-3">
                             <div class="col-sm-4 text-md-right font-weight-bold beam-field-label beam-detail-field-label beam-field-label-{{ field }}">
 
                                 {% block detail_field_label %}
                                     {{ object|field_verbose_name:field|capfirst }}
                                 {% endblock %}
 
                             </div>
```

### Comparing `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/links.html` & `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/links.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/list_links.html` & `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/list_links.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/messages.html` & `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/messages.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/navigation.html` & `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/navigation.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/partials/pagination.html` & `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/partials/pagination.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,29 @@
-{% load i18n beam_tags %}
-<div class="row" data-object-count="{% if is_paginated %}{{ page_obj.paginator.count }}{% else %}{{ object_list.count }}{% endif %}">
-    <div class="col-sm-6">
-        <p class="pt-2">
+{% load i18n %}
+{% load beam_tags %}
+
+
+<div class="row align-items-center" data-object-count="{% if is_paginated %}{{ page_obj.paginator.count }}{% else %}{{ object_list.count }}{% endif %}">
+    <div class="{% if is_paginated %}col-sm-4{% else %}col-12{% endif %}">
+        <div class="object-count">
             {% if object_list %}
                 {% if is_paginated %}
                     {% blocktrans with total=page_obj.paginator.count start=page_obj.start_index end=page_obj.end_index name=options.verbose_name_plural %}Showing {{ start }} to {{ end }} of {{ total }} {{ name }}{% endblocktrans %}
                 {% elif page_obj.paginator.count == 1 %}
                     {% blocktrans with total=page_obj.paginator.count name_singular=options.verbose_name %}Showing {{ total }} {{ name_singular }}{% endblocktrans %}
                 {% else %}
                     {% blocktrans with total=object_list.count name_plural=options.verbose_name_plural %}Showing {{ total }} {{ name_plural }}{% endblocktrans %}
                 {% endif %}
             {% endif %}
-        </p>
+        </div>
     </div>
 
     {% if is_paginated %}
-        <nav class="col-sm-6" aria-label="{% trans 'pagination' %}">
-            <ul class="pagination justify-content-end">
+        <nav class="col-sm-8" aria-label="{% trans 'pagination' %}">
+            <ul class="pagination justify-content-center mb-0">
                 {% if page_obj.has_previous %}
                     <li class="page-item">
                         <a class="page-link" href="{% page_link page_param page_obj.previous_page_number  %}" aria-label="Previous">
                             <span aria-hidden="true">&laquo;</span>
                             <span class="sr-only">{% trans "Previous" %}</span>
                         </a>
                     </li>
```

### Comparing `django-beam-1.4.0/src/beam/themes/bootstrap4/templates/beam/update.html` & `django-beam-1.4.1/src/beam/themes/bootstrap4/templates/beam/update.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/themes/bootstrap4/widgets.py` & `django-beam-1.4.1/src/beam/themes/bootstrap4/widgets.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/urls.py` & `django-beam-1.4.1/src/beam/urls.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/utils.py` & `django-beam-1.4.1/src/beam/utils.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/views.py` & `django-beam-1.4.1/src/beam/views.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/beam/viewsets.py` & `django-beam-1.4.1/src/beam/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/src/django_beam.egg-info/PKG-INFO` & `django-beam-1.4.1/src/django_beam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-beam
-Version: 1.4.0
+Version: 1.4.1
 Summary: A crud library for python
 Home-page: https://github.com/django-beam/django-beam
-Download-URL: https://github.com/django-beam/django-beam/archive/1.4.0.tar.gz
+Download-URL: https://github.com/django-beam/django-beam/archive/1.4.1.tar.gz
 Author: Raphael Kimmig
 Author-email: raphael@ampad.de
 License: BSD 3-Clause License
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `django-beam-1.4.0/src/django_beam.egg-info/SOURCES.txt` & `django-beam-1.4.1/src/django_beam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/tests/test_actions.py` & `django-beam-1.4.1/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/tests/test_components.py` & `django-beam-1.4.1/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/tests/test_contrib_auth.py` & `django-beam-1.4.1/tests/test_contrib_auth.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/tests/test_contrib_autocomplete.py` & `django-beam-1.4.1/tests/test_contrib_autocomplete.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/tests/test_contrib_reversion.py` & `django-beam-1.4.1/tests/test_contrib_reversion.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/tests/test_inlines.py` & `django-beam-1.4.1/tests/test_inlines.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/tests/test_registry.py` & `django-beam-1.4.1/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/tests/test_tags.py` & `django-beam-1.4.1/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/tests/test_urls.py` & `django-beam-1.4.1/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/tests/test_utils.py` & `django-beam-1.4.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/tests/test_views.py` & `django-beam-1.4.1/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.4.0/tests/test_viewsets.py` & `django-beam-1.4.1/tests/test_viewsets.py`

 * *Files identical despite different names*

