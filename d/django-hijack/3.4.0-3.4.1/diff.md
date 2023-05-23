# Comparing `tmp/django-hijack-3.4.0.tar.gz` & `tmp/django-hijack-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-hijack-3.4.0.tar", last modified: Tue May 23 13:27:59 2023, max compression
+gzip compressed data, was "django-hijack-3.4.1.tar", last modified: Tue May 23 14:32:59 2023, max compression
```

## Comparing `django-hijack-3.4.0.tar` & `django-hijack-3.4.1.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.290235 django-hijack-3.4.0/
--rw-r--r--   0 johannes   (501) wheel        (0)      350 2023-05-23 13:27:00.000000 django-hijack-3.4.0/.editorconfig
--rw-r--r--   0 johannes   (501) wheel        (0)       25 2023-05-23 13:27:00.000000 django-hijack-3.4.0/.gitattributes
--rw-r--r--   0 johannes   (501) wheel        (0)        6 2023-05-23 13:27:00.000000 django-hijack-3.4.0/.nvmrc
--rw-r--r--   0 johannes   (501) wheel        (0)      364 2023-05-23 13:27:00.000000 django-hijack-3.4.0/.readthedocs.yaml
--rw-r--r--   0 johannes   (501) wheel        (0)      129 2023-05-23 13:27:00.000000 django-hijack-3.4.0/.stylelintrc.json
--rw-r--r--   0 johannes   (501) wheel        (0)      579 2023-05-23 13:27:00.000000 django-hijack-3.4.0/CONTRIBUTING.md
--rw-r--r--   0 johannes   (501) wheel        (0)     1107 2023-05-23 13:27:00.000000 django-hijack-3.4.0/LICENSE
--rw-r--r--   0 johannes   (501) wheel        (0)      138 2023-05-23 13:27:00.000000 django-hijack-3.4.0/MANIFEST.in
--rw-r--r--   0 johannes   (501) wheel        (0)     2838 2023-05-23 13:27:59.290325 django-hijack-3.4.0/PKG-INFO
--rw-r--r--   0 johannes   (501) wheel        (0)     1843 2023-05-23 13:27:00.000000 django-hijack-3.4.0/README.md
--rw-r--r--   0 johannes   (501) wheel        (0)     2528 2023-05-23 13:27:00.000000 django-hijack-3.4.0/SECURITY.md
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.281928 django-hijack-3.4.0/django_hijack.egg-info/
--rw-r--r--   0 johannes   (501) wheel        (0)     2838 2023-05-23 13:27:59.000000 django-hijack-3.4.0/django_hijack.egg-info/PKG-INFO
--rw-r--r--   0 johannes   (501) wheel        (0)     2037 2023-05-23 13:27:59.000000 django-hijack-3.4.0/django_hijack.egg-info/SOURCES.txt
--rw-r--r--   0 johannes   (501) wheel        (0)        1 2023-05-23 13:27:59.000000 django-hijack-3.4.0/django_hijack.egg-info/dependency_links.txt
--rw-r--r--   0 johannes   (501) wheel        (0)       52 2023-05-23 13:27:59.000000 django-hijack-3.4.0/django_hijack.egg-info/requires.txt
--rw-r--r--   0 johannes   (501) wheel        (0)        7 2023-05-23 13:27:59.000000 django-hijack-3.4.0/django_hijack.egg-info/top_level.txt
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.283600 django-hijack-3.4.0/docs/
--rw-r--r--   0 johannes   (501) wheel        (0)   118448 2023-05-23 13:27:00.000000 django-hijack-3.4.0/docs/admin-screenshot.png
--rw-r--r--   0 johannes   (501) wheel        (0)     5951 2023-05-23 13:27:00.000000 django-hijack-3.4.0/docs/customization.md
--rw-r--r--   0 johannes   (501) wheel        (0)    24164 2023-05-23 13:27:00.000000 django-hijack-3.4.0/docs/django-hijack.jpg
--rw-r--r--   0 johannes   (501) wheel        (0)     2706 2023-05-23 13:27:00.000000 django-hijack-3.4.0/docs/index.md
--rw-r--r--   0 johannes   (501) wheel        (0)    21330 2023-05-23 13:27:00.000000 django-hijack-3.4.0/docs/release-button.png
--rw-r--r--   0 johannes   (501) wheel        (0)     2528 2023-05-23 13:27:00.000000 django-hijack-3.4.0/docs/security.md
--rw-r--r--   0 johannes   (501) wheel        (0)      485 2023-05-23 13:27:00.000000 django-hijack-3.4.0/docs/troubleshooting.md
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.284747 django-hijack-3.4.0/hijack/
--rw-r--r--   0 johannes   (501) wheel        (0)       95 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/__init__.py
--rw-r--r--   0 johannes   (501) wheel        (0)      115 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/apps.py
--rw-r--r--   0 johannes   (501) wheel        (0)      413 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/conf.py
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.284896 django-hijack-3.4.0/hijack/contrib/
--rw-r--r--   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/contrib/__init__.py
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.285285 django-hijack-3.4.0/hijack/contrib/admin/
--rw-r--r--   0 johannes   (501) wheel        (0)      163 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/contrib/admin/__init__.py
--rw-r--r--   0 johannes   (501) wheel        (0)     3393 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/contrib/admin/admin.py
--rw-r--r--   0 johannes   (501) wheel        (0)     1605 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/contrib/admin/apps.py
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.275983 django-hijack-3.4.0/hijack/contrib/admin/templates/
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.276032 django-hijack-3.4.0/hijack/contrib/admin/templates/hijack/
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.276082 django-hijack-3.4.0/hijack/contrib/admin/templates/hijack/contrib/
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.285433 django-hijack-3.4.0/hijack/contrib/admin/templates/hijack/contrib/admin/
--rw-r--r--   0 johannes   (501) wheel        (0)      430 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/contrib/admin/templates/hijack/contrib/admin/button.html
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.277326 django-hijack-3.4.0/hijack/locale/
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.276247 django-hijack-3.4.0/hijack/locale/cs/
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.285583 django-hijack-3.4.0/hijack/locale/cs/LC_MESSAGES/
--rw-r--r--   0 johannes   (501) wheel        (0)     1107 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.276359 django-hijack-3.4.0/hijack/locale/da/
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.285723 django-hijack-3.4.0/hijack/locale/da/LC_MESSAGES/
--rw-r--r--   0 johannes   (501) wheel        (0)     1080 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/locale/da/LC_MESSAGES/django.po
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.276477 django-hijack-3.4.0/hijack/locale/de/
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.285871 django-hijack-3.4.0/hijack/locale/de/LC_MESSAGES/
--rw-r--r--   0 johannes   (501) wheel        (0)     1092 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.276589 django-hijack-3.4.0/hijack/locale/es/
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.286013 django-hijack-3.4.0/hijack/locale/es/LC_MESSAGES/
--rw-r--r--   0 johannes   (501) wheel        (0)     1050 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.276705 django-hijack-3.4.0/hijack/locale/fr/
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.286161 django-hijack-3.4.0/hijack/locale/fr/LC_MESSAGES/
--rw-r--r--   0 johannes   (501) wheel        (0)     1172 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.276818 django-hijack-3.4.0/hijack/locale/ja/
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.286312 django-hijack-3.4.0/hijack/locale/ja/LC_MESSAGES/
--rw-r--r--   0 johannes   (501) wheel        (0)     1157 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.276928 django-hijack-3.4.0/hijack/locale/nl/
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.286455 django-hijack-3.4.0/hijack/locale/nl/LC_MESSAGES/
--rw-r--r--   0 johannes   (501) wheel        (0)     1218 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.277040 django-hijack-3.4.0/hijack/locale/pl/
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.286603 django-hijack-3.4.0/hijack/locale/pl/LC_MESSAGES/
--rw-r--r--   0 johannes   (501) wheel        (0)     1136 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.277151 django-hijack-3.4.0/hijack/locale/pt_BR/
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.286755 django-hijack-3.4.0/hijack/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 johannes   (501) wheel        (0)     1094 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.277262 django-hijack-3.4.0/hijack/locale/ru/
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.286902 django-hijack-3.4.0/hijack/locale/ru/LC_MESSAGES/
--rw-r--r--   0 johannes   (501) wheel        (0)     1135 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.277376 django-hijack-3.4.0/hijack/locale/sk/
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.287050 django-hijack-3.4.0/hijack/locale/sk/LC_MESSAGES/
--rw-r--r--   0 johannes   (501) wheel        (0)     1115 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/locale/sk/LC_MESSAGES/django.po
--rw-r--r--   0 johannes   (501) wheel        (0)     2492 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/middleware.py
--rw-r--r--   0 johannes   (501) wheel        (0)      642 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/permissions.py
--rw-r--r--   0 johannes   (501) wheel        (0)      774 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/signals.py
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.277485 django-hijack-3.4.0/hijack/static/
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.287343 django-hijack-3.4.0/hijack/static/hijack/
--rw-r--r--   0 johannes   (501) wheel        (0)      743 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/static/hijack/hijack.js
--rw-r--r--   0 johannes   (501) wheel        (0)     1372 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/static/hijack/hijack.scss
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.277595 django-hijack-3.4.0/hijack/templates/
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.287476 django-hijack-3.4.0/hijack/templates/hijack/
--rw-r--r--   0 johannes   (501) wheel        (0)      912 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/templates/hijack/notification.html
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.287700 django-hijack-3.4.0/hijack/templatetags/
--rw-r--r--   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/templatetags/__init__.py
--rw-r--r--   0 johannes   (501) wheel        (0)      548 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/templatetags/hijack.py
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.288698 django-hijack-3.4.0/hijack/tests/
--rw-r--r--   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/tests/__init__.py
--rw-r--r--   0 johannes   (501) wheel        (0)      752 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/tests/conftest.py
--rw-r--r--   0 johannes   (501) wheel        (0)     2945 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/tests/test_admin.py
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.289578 django-hijack-3.4.0/hijack/tests/test_app/
--rw-r--r--   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/tests/test_app/__init__.py
--rw-r--r--   0 johannes   (501) wheel        (0)      388 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/tests/test_app/admin.py
--rw-r--r--   0 johannes   (501) wheel        (0)      539 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/tests/test_app/models.py
--rw-r--r--   0 johannes   (501) wheel        (0)      110 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/tests/test_app/permissions.py
--rw-r--r--   0 johannes   (501) wheel        (0)     3290 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/tests/test_app/settings.py
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.290069 django-hijack-3.4.0/hijack/tests/test_app/templates/
--rw-r--r--   0 johannes   (501) wheel        (0)       47 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/tests/test_app/templates/bye_bye.html
--rw-r--r--   0 johannes   (501) wheel        (0)      460 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/tests/test_app/templates/user_list.html
--rw-r--r--   0 johannes   (501) wheel        (0)      536 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/tests/test_app/urls.py
--rw-r--r--   0 johannes   (501) wheel        (0)      371 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/tests/test_app/views.py
--rw-r--r--   0 johannes   (501) wheel        (0)     5821 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/tests/test_middleware.py
--rw-r--r--   0 johannes   (501) wheel        (0)     2008 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/tests/test_permissions.py
--rw-r--r--   0 johannes   (501) wheel        (0)      619 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/tests/test_signals.py
--rw-r--r--   0 johannes   (501) wheel        (0)      705 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/tests/test_templatetags.py
--rw-r--r--   0 johannes   (501) wheel        (0)     7089 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/tests/test_views.py
--rw-r--r--   0 johannes   (501) wheel        (0)      236 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/urls.py
--rwxr-xr-x   0 johannes   (501) wheel        (0)     4896 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/views.py
--rw-r--r--   0 johannes   (501) wheel        (0)      332 2023-05-23 13:27:00.000000 django-hijack-3.4.0/mkdocs.yml
--rw-r--r--   0 johannes   (501) wheel        (0)   357954 2023-05-23 13:27:00.000000 django-hijack-3.4.0/package-lock.json
--rw-r--r--   0 johannes   (501) wheel        (0)     1124 2023-05-23 13:27:00.000000 django-hijack-3.4.0/package.json
--rw-r--r--   0 johannes   (501) wheel        (0)       47 2023-05-23 13:27:00.000000 django-hijack-3.4.0/postcss.config.js
--rw-r--r--   0 johannes   (501) wheel        (0)     1742 2023-05-23 13:27:59.290749 django-hijack-3.4.0/setup.cfg
--rwxr-xr-x   0 johannes   (501) wheel        (0)     2581 2023-05-23 13:27:00.000000 django-hijack-3.4.0/setup.py
--rw-r--r--   0 johannes   (501) wheel        (0)      682 2023-05-23 13:27:00.000000 django-hijack-3.4.0/webpack.config.js
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.538749 django-hijack-3.4.1/
+-rw-r--r--   0 johannes   (501) wheel        (0)      350 2023-05-23 13:27:00.000000 django-hijack-3.4.1/.editorconfig
+-rw-r--r--   0 johannes   (501) wheel        (0)       25 2023-05-23 13:27:00.000000 django-hijack-3.4.1/.gitattributes
+-rw-r--r--   0 johannes   (501) wheel        (0)        6 2023-05-23 13:27:00.000000 django-hijack-3.4.1/.nvmrc
+-rw-r--r--   0 johannes   (501) wheel        (0)      364 2023-05-23 13:27:00.000000 django-hijack-3.4.1/.readthedocs.yaml
+-rw-r--r--   0 johannes   (501) wheel        (0)      129 2023-05-23 13:27:00.000000 django-hijack-3.4.1/.stylelintrc.json
+-rw-r--r--   0 johannes   (501) wheel        (0)      579 2023-05-23 13:27:00.000000 django-hijack-3.4.1/CONTRIBUTING.md
+-rw-r--r--   0 johannes   (501) wheel        (0)     1107 2023-05-23 13:27:00.000000 django-hijack-3.4.1/LICENSE
+-rw-r--r--   0 johannes   (501) wheel        (0)      138 2023-05-23 13:27:00.000000 django-hijack-3.4.1/MANIFEST.in
+-rw-r--r--   0 johannes   (501) wheel        (0)     2839 2023-05-23 14:32:59.538849 django-hijack-3.4.1/PKG-INFO
+-rw-r--r--   0 johannes   (501) wheel        (0)     1843 2023-05-23 13:27:00.000000 django-hijack-3.4.1/README.md
+-rw-r--r--   0 johannes   (501) wheel        (0)     2528 2023-05-23 13:27:00.000000 django-hijack-3.4.1/SECURITY.md
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.530446 django-hijack-3.4.1/django_hijack.egg-info/
+-rw-r--r--   0 johannes   (501) wheel        (0)     2839 2023-05-23 14:32:59.000000 django-hijack-3.4.1/django_hijack.egg-info/PKG-INFO
+-rw-r--r--   0 johannes   (501) wheel        (0)     2037 2023-05-23 14:32:59.000000 django-hijack-3.4.1/django_hijack.egg-info/SOURCES.txt
+-rw-r--r--   0 johannes   (501) wheel        (0)        1 2023-05-23 14:32:59.000000 django-hijack-3.4.1/django_hijack.egg-info/dependency_links.txt
+-rw-r--r--   0 johannes   (501) wheel        (0)       52 2023-05-23 14:32:59.000000 django-hijack-3.4.1/django_hijack.egg-info/requires.txt
+-rw-r--r--   0 johannes   (501) wheel        (0)        7 2023-05-23 14:32:59.000000 django-hijack-3.4.1/django_hijack.egg-info/top_level.txt
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.531847 django-hijack-3.4.1/docs/
+-rw-r--r--   0 johannes   (501) wheel        (0)   118448 2023-05-23 13:27:00.000000 django-hijack-3.4.1/docs/admin-screenshot.png
+-rw-r--r--   0 johannes   (501) wheel        (0)     5951 2023-05-23 13:27:00.000000 django-hijack-3.4.1/docs/customization.md
+-rw-r--r--   0 johannes   (501) wheel        (0)    24164 2023-05-23 13:27:00.000000 django-hijack-3.4.1/docs/django-hijack.jpg
+-rw-r--r--   0 johannes   (501) wheel        (0)     2706 2023-05-23 13:27:00.000000 django-hijack-3.4.1/docs/index.md
+-rw-r--r--   0 johannes   (501) wheel        (0)    21330 2023-05-23 13:27:00.000000 django-hijack-3.4.1/docs/release-button.png
+-rw-r--r--   0 johannes   (501) wheel        (0)     2528 2023-05-23 13:27:00.000000 django-hijack-3.4.1/docs/security.md
+-rw-r--r--   0 johannes   (501) wheel        (0)      485 2023-05-23 13:27:00.000000 django-hijack-3.4.1/docs/troubleshooting.md
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.533107 django-hijack-3.4.1/hijack/
+-rw-r--r--   0 johannes   (501) wheel        (0)       95 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/__init__.py
+-rw-r--r--   0 johannes   (501) wheel        (0)      115 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/apps.py
+-rw-r--r--   0 johannes   (501) wheel        (0)      413 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/conf.py
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.533261 django-hijack-3.4.1/hijack/contrib/
+-rw-r--r--   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/contrib/__init__.py
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.533669 django-hijack-3.4.1/hijack/contrib/admin/
+-rw-r--r--   0 johannes   (501) wheel        (0)      163 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/contrib/admin/__init__.py
+-rw-r--r--   0 johannes   (501) wheel        (0)     3393 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/contrib/admin/admin.py
+-rw-r--r--   0 johannes   (501) wheel        (0)     1605 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/contrib/admin/apps.py
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.524393 django-hijack-3.4.1/hijack/contrib/admin/templates/
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.524447 django-hijack-3.4.1/hijack/contrib/admin/templates/hijack/
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.524498 django-hijack-3.4.1/hijack/contrib/admin/templates/hijack/contrib/
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.533826 django-hijack-3.4.1/hijack/contrib/admin/templates/hijack/contrib/admin/
+-rw-r--r--   0 johannes   (501) wheel        (0)      430 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/contrib/admin/templates/hijack/contrib/admin/button.html
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.525795 django-hijack-3.4.1/hijack/locale/
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.524670 django-hijack-3.4.1/hijack/locale/cs/
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.534003 django-hijack-3.4.1/hijack/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 johannes   (501) wheel        (0)     1107 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.524796 django-hijack-3.4.1/hijack/locale/da/
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.534166 django-hijack-3.4.1/hijack/locale/da/LC_MESSAGES/
+-rw-r--r--   0 johannes   (501) wheel        (0)     1080 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/locale/da/LC_MESSAGES/django.po
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.524926 django-hijack-3.4.1/hijack/locale/de/
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.534326 django-hijack-3.4.1/hijack/locale/de/LC_MESSAGES/
+-rw-r--r--   0 johannes   (501) wheel        (0)     1092 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.525045 django-hijack-3.4.1/hijack/locale/es/
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.534491 django-hijack-3.4.1/hijack/locale/es/LC_MESSAGES/
+-rw-r--r--   0 johannes   (501) wheel        (0)     1050 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.525163 django-hijack-3.4.1/hijack/locale/fr/
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.534649 django-hijack-3.4.1/hijack/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 johannes   (501) wheel        (0)     1172 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.525282 django-hijack-3.4.1/hijack/locale/ja/
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.534807 django-hijack-3.4.1/hijack/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 johannes   (501) wheel        (0)     1157 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.525399 django-hijack-3.4.1/hijack/locale/nl/
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.534958 django-hijack-3.4.1/hijack/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 johannes   (501) wheel        (0)     1218 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.525510 django-hijack-3.4.1/hijack/locale/pl/
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.535104 django-hijack-3.4.1/hijack/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 johannes   (501) wheel        (0)     1136 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.525621 django-hijack-3.4.1/hijack/locale/pt_BR/
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.535251 django-hijack-3.4.1/hijack/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 johannes   (501) wheel        (0)     1094 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.525732 django-hijack-3.4.1/hijack/locale/ru/
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.535403 django-hijack-3.4.1/hijack/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 johannes   (501) wheel        (0)     1135 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.525843 django-hijack-3.4.1/hijack/locale/sk/
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.535565 django-hijack-3.4.1/hijack/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 johannes   (501) wheel        (0)     1115 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/locale/sk/LC_MESSAGES/django.po
+-rw-r--r--   0 johannes   (501) wheel        (0)     2492 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/middleware.py
+-rw-r--r--   0 johannes   (501) wheel        (0)      642 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/permissions.py
+-rw-r--r--   0 johannes   (501) wheel        (0)      774 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/signals.py
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.525954 django-hijack-3.4.1/hijack/static/
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.535865 django-hijack-3.4.1/hijack/static/hijack/
+-rw-r--r--   0 johannes   (501) wheel        (0)      743 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/static/hijack/hijack.js
+-rw-r--r--   0 johannes   (501) wheel        (0)     1372 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/static/hijack/hijack.scss
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.526064 django-hijack-3.4.1/hijack/templates/
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.536014 django-hijack-3.4.1/hijack/templates/hijack/
+-rw-r--r--   0 johannes   (501) wheel        (0)      912 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/templates/hijack/notification.html
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.536267 django-hijack-3.4.1/hijack/templatetags/
+-rw-r--r--   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/templatetags/__init__.py
+-rw-r--r--   0 johannes   (501) wheel        (0)      548 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/templatetags/hijack.py
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.537428 django-hijack-3.4.1/hijack/tests/
+-rw-r--r--   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/tests/__init__.py
+-rw-r--r--   0 johannes   (501) wheel        (0)      752 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/tests/conftest.py
+-rw-r--r--   0 johannes   (501) wheel        (0)     2945 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/tests/test_admin.py
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.538340 django-hijack-3.4.1/hijack/tests/test_app/
+-rw-r--r--   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/tests/test_app/__init__.py
+-rw-r--r--   0 johannes   (501) wheel        (0)      388 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/tests/test_app/admin.py
+-rw-r--r--   0 johannes   (501) wheel        (0)      539 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/tests/test_app/models.py
+-rw-r--r--   0 johannes   (501) wheel        (0)      110 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/tests/test_app/permissions.py
+-rw-r--r--   0 johannes   (501) wheel        (0)     2932 2023-05-23 14:32:52.000000 django-hijack-3.4.1/hijack/tests/test_app/settings.py
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 14:32:59.538615 django-hijack-3.4.1/hijack/tests/test_app/templates/
+-rw-r--r--   0 johannes   (501) wheel        (0)       47 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/tests/test_app/templates/bye_bye.html
+-rw-r--r--   0 johannes   (501) wheel        (0)      460 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/tests/test_app/templates/user_list.html
+-rw-r--r--   0 johannes   (501) wheel        (0)      536 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/tests/test_app/urls.py
+-rw-r--r--   0 johannes   (501) wheel        (0)      371 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/tests/test_app/views.py
+-rw-r--r--   0 johannes   (501) wheel        (0)     5821 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/tests/test_middleware.py
+-rw-r--r--   0 johannes   (501) wheel        (0)     2008 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/tests/test_permissions.py
+-rw-r--r--   0 johannes   (501) wheel        (0)      619 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/tests/test_signals.py
+-rw-r--r--   0 johannes   (501) wheel        (0)      705 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/tests/test_templatetags.py
+-rw-r--r--   0 johannes   (501) wheel        (0)     7089 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/tests/test_views.py
+-rw-r--r--   0 johannes   (501) wheel        (0)      236 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/urls.py
+-rwxr-xr-x   0 johannes   (501) wheel        (0)     4896 2023-05-23 13:27:00.000000 django-hijack-3.4.1/hijack/views.py
+-rw-r--r--   0 johannes   (501) wheel        (0)      332 2023-05-23 13:27:00.000000 django-hijack-3.4.1/mkdocs.yml
+-rw-r--r--   0 johannes   (501) wheel        (0)   357954 2023-05-23 13:27:00.000000 django-hijack-3.4.1/package-lock.json
+-rw-r--r--   0 johannes   (501) wheel        (0)     1124 2023-05-23 13:27:00.000000 django-hijack-3.4.1/package.json
+-rw-r--r--   0 johannes   (501) wheel        (0)       47 2023-05-23 13:27:00.000000 django-hijack-3.4.1/postcss.config.js
+-rw-r--r--   0 johannes   (501) wheel        (0)     1752 2023-05-23 14:32:59.539244 django-hijack-3.4.1/setup.cfg
+-rwxr-xr-x   0 johannes   (501) wheel        (0)     2581 2023-05-23 13:27:00.000000 django-hijack-3.4.1/setup.py
+-rw-r--r--   0 johannes   (501) wheel        (0)      682 2023-05-23 13:27:00.000000 django-hijack-3.4.1/webpack.config.js
```

### Comparing `django-hijack-3.4.0/CONTRIBUTING.md` & `django-hijack-3.4.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/LICENSE` & `django-hijack-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/PKG-INFO` & `django-hijack-3.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: django-hijack
-Version: 3.4.0
+Version: 3.4.1
 Summary: django-hijack allows superusers to hijack (=login as) and work on behalf of another user.
 Home-page: https://github.com/django-hijack/django-hijack
 Author: arteria GmbH
 Author-email: admin@arteria.ch
 License: MIT
 Keywords: django,hijack,support,customer support,debugging
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # Django Hijack
 
 [![CI](https://github.com/django-hijack/django-hijack/workflows/CI/badge.svg?branch=master)](https://github.com/django-hijack/django-hijack/actions)
```

### Comparing `django-hijack-3.4.0/README.md` & `django-hijack-3.4.1/README.md`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/SECURITY.md` & `django-hijack-3.4.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/django_hijack.egg-info/PKG-INFO` & `django-hijack-3.4.1/django_hijack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: django-hijack
-Version: 3.4.0
+Version: 3.4.1
 Summary: django-hijack allows superusers to hijack (=login as) and work on behalf of another user.
 Home-page: https://github.com/django-hijack/django-hijack
 Author: arteria GmbH
 Author-email: admin@arteria.ch
 License: MIT
 Keywords: django,hijack,support,customer support,debugging
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # Django Hijack
 
 [![CI](https://github.com/django-hijack/django-hijack/workflows/CI/badge.svg?branch=master)](https://github.com/django-hijack/django-hijack/actions)
```

### Comparing `django-hijack-3.4.0/django_hijack.egg-info/SOURCES.txt` & `django-hijack-3.4.1/django_hijack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/docs/admin-screenshot.png` & `django-hijack-3.4.1/docs/admin-screenshot.png`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/docs/customization.md` & `django-hijack-3.4.1/docs/customization.md`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/docs/django-hijack.jpg` & `django-hijack-3.4.1/docs/django-hijack.jpg`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/docs/index.md` & `django-hijack-3.4.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/docs/release-button.png` & `django-hijack-3.4.1/docs/release-button.png`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/docs/security.md` & `django-hijack-3.4.1/docs/security.md`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/hijack/contrib/admin/admin.py` & `django-hijack-3.4.1/hijack/contrib/admin/admin.py`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/hijack/contrib/admin/apps.py` & `django-hijack-3.4.1/hijack/contrib/admin/apps.py`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/hijack/locale/cs/LC_MESSAGES/django.po` & `django-hijack-3.4.1/hijack/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/hijack/locale/da/LC_MESSAGES/django.po` & `django-hijack-3.4.1/hijack/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/hijack/locale/de/LC_MESSAGES/django.po` & `django-hijack-3.4.1/hijack/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/hijack/locale/es/LC_MESSAGES/django.po` & `django-hijack-3.4.1/hijack/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/hijack/locale/fr/LC_MESSAGES/django.po` & `django-hijack-3.4.1/hijack/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/hijack/locale/ja/LC_MESSAGES/django.po` & `django-hijack-3.4.1/hijack/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/hijack/locale/nl/LC_MESSAGES/django.po` & `django-hijack-3.4.1/hijack/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/hijack/locale/pl/LC_MESSAGES/django.po` & `django-hijack-3.4.1/hijack/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/hijack/locale/pt_BR/LC_MESSAGES/django.po` & `django-hijack-3.4.1/hijack/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/hijack/locale/ru/LC_MESSAGES/django.po` & `django-hijack-3.4.1/hijack/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/hijack/locale/sk/LC_MESSAGES/django.po` & `django-hijack-3.4.1/hijack/locale/sk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/hijack/middleware.py` & `django-hijack-3.4.1/hijack/middleware.py`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/hijack/permissions.py` & `django-hijack-3.4.1/hijack/permissions.py`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/hijack/signals.py` & `django-hijack-3.4.1/hijack/signals.py`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/hijack/static/hijack/hijack.js` & `django-hijack-3.4.1/hijack/static/hijack/hijack.js`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/hijack/static/hijack/hijack.scss` & `django-hijack-3.4.1/hijack/static/hijack/hijack.scss`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/hijack/templates/hijack/notification.html` & `django-hijack-3.4.1/hijack/templates/hijack/notification.html`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/hijack/templatetags/hijack.py` & `django-hijack-3.4.1/hijack/templatetags/hijack.py`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/hijack/tests/conftest.py` & `django-hijack-3.4.1/hijack/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/hijack/tests/test_admin.py` & `django-hijack-3.4.1/hijack/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/hijack/tests/test_app/models.py` & `django-hijack-3.4.1/hijack/tests/test_app/models.py`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/hijack/tests/test_app/settings.py` & `django-hijack-3.4.1/hijack/tests/test_app/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,23 +24,14 @@
 MEDIA_ROOT = os.path.join(APP_ROOT, "../app_media")
 STATICFILES_DIRS = (os.path.join(APP_ROOT, "static"),)
 
 NOSE_ARGS = []
 
 TEMPLATE_DIRS = (os.path.join(APP_ROOT, "tests/test_app/templates"),)
 
-PASSWORD_HASHERS = (
-    "django.contrib.auth.hashers.PBKDF2PasswordHasher",
-    "django.contrib.auth.hashers.PBKDF2SHA1PasswordHasher",
-    "django.contrib.auth.hashers.BCryptPasswordHasher",
-    "django.contrib.auth.hashers.SHA1PasswordHasher",
-    "django.contrib.auth.hashers.MD5PasswordHasher",
-    "django.contrib.auth.hashers.CryptPasswordHasher",
-)
-
 MIDDLEWARE = (
     "django.middleware.security.SecurityMiddleware",
     "django.contrib.sessions.middleware.SessionMiddleware",
     "django.middleware.common.CommonMiddleware",
     "django.middleware.csrf.CsrfViewMiddleware",
     "django.contrib.auth.middleware.AuthenticationMiddleware",
     "hijack.middleware.HijackUserMiddleware",
```

### Comparing `django-hijack-3.4.0/hijack/tests/test_app/urls.py` & `django-hijack-3.4.1/hijack/tests/test_app/urls.py`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/hijack/tests/test_middleware.py` & `django-hijack-3.4.1/hijack/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/hijack/tests/test_permissions.py` & `django-hijack-3.4.1/hijack/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/hijack/tests/test_signals.py` & `django-hijack-3.4.1/hijack/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/hijack/tests/test_templatetags.py` & `django-hijack-3.4.1/hijack/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/hijack/tests/test_views.py` & `django-hijack-3.4.1/hijack/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/hijack/views.py` & `django-hijack-3.4.1/hijack/views.py`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/package-lock.json` & `django-hijack-3.4.1/package-lock.json`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/package.json` & `django-hijack-3.4.1/package.json`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/setup.cfg` & `django-hijack-3.4.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -17,22 +17,22 @@
 	customer support
 	debugging
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	License :: OSI Approved :: MIT License
 	Framework :: Django
 	Framework :: Django :: 3.2
-	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 include_package_data = True
 packages = hijack
 install_requires = 
 	django>=2.2
 setup_requires = 
@@ -45,16 +45,16 @@
 	pytest-django
 
 [tool:pytest]
 addopts = --cov --tb=short
 testpaths = 
 	hijack
 filterwarnings = 
-	error
-	ignore::PendingDeprecationWarning
+	ignore::DeprecationWarning
+	error::RuntimeWarning
 DJANGO_SETTINGS_MODULE = hijack.tests.test_app.settings
 
 [coverage:run]
 source = hijack
 omit = 
 	hijack/tests/*
```

### Comparing `django-hijack-3.4.0/setup.py` & `django-hijack-3.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `django-hijack-3.4.0/webpack.config.js` & `django-hijack-3.4.1/webpack.config.js`

 * *Files identical despite different names*

