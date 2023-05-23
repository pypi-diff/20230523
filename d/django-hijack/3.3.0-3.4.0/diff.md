# Comparing `tmp/django-hijack-3.3.0.tar.gz` & `tmp/django-hijack-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-hijack-3.3.0.tar", last modified: Wed Mar 15 13:45:31 2023, max compression
+gzip compressed data, was "django-hijack-3.4.0.tar", last modified: Tue May 23 13:27:59 2023, max compression
```

## Comparing `django-hijack-3.3.0.tar` & `django-hijack-3.4.0.tar`

### file list

```diff
@@ -1,114 +1,117 @@
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.920097 django-hijack-3.3.0/
--rw-r--r--   0 johannes   (501) wheel        (0)      350 2023-03-15 13:45:11.000000 django-hijack-3.3.0/.editorconfig
--rw-r--r--   0 johannes   (501) wheel        (0)       25 2023-03-15 13:45:11.000000 django-hijack-3.3.0/.gitattributes
--rw-r--r--   0 johannes   (501) wheel        (0)        6 2023-03-15 13:45:11.000000 django-hijack-3.3.0/.nvmrc
--rw-r--r--   0 johannes   (501) wheel        (0)      364 2023-03-15 13:45:11.000000 django-hijack-3.3.0/.readthedocs.yaml
--rw-r--r--   0 johannes   (501) wheel        (0)      129 2023-03-15 13:45:11.000000 django-hijack-3.3.0/.stylelintrc.json
--rw-r--r--   0 johannes   (501) wheel        (0)      579 2023-03-15 13:45:11.000000 django-hijack-3.3.0/CONTRIBUTING.md
--rw-r--r--   0 johannes   (501) wheel        (0)     1107 2023-03-15 13:45:11.000000 django-hijack-3.3.0/LICENSE
--rw-r--r--   0 johannes   (501) wheel        (0)      138 2023-03-15 13:45:11.000000 django-hijack-3.3.0/MANIFEST.in
--rw-r--r--   0 johannes   (501) wheel        (0)     2838 2023-03-15 13:45:31.920182 django-hijack-3.3.0/PKG-INFO
--rw-r--r--   0 johannes   (501) wheel        (0)     1843 2023-03-15 13:45:11.000000 django-hijack-3.3.0/README.md
--rw-r--r--   0 johannes   (501) wheel        (0)     2528 2023-03-15 13:45:11.000000 django-hijack-3.3.0/SECURITY.md
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.914001 django-hijack-3.3.0/django_hijack.egg-info/
--rw-r--r--   0 johannes   (501) wheel        (0)     2838 2023-03-15 13:45:31.000000 django-hijack-3.3.0/django_hijack.egg-info/PKG-INFO
--rw-r--r--   0 johannes   (501) wheel        (0)     1998 2023-03-15 13:45:31.000000 django-hijack-3.3.0/django_hijack.egg-info/SOURCES.txt
--rw-r--r--   0 johannes   (501) wheel        (0)        1 2023-03-15 13:45:31.000000 django-hijack-3.3.0/django_hijack.egg-info/dependency_links.txt
--rw-r--r--   0 johannes   (501) wheel        (0)       52 2023-03-15 13:45:31.000000 django-hijack-3.3.0/django_hijack.egg-info/requires.txt
--rw-r--r--   0 johannes   (501) wheel        (0)        7 2023-03-15 13:45:31.000000 django-hijack-3.3.0/django_hijack.egg-info/top_level.txt
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.914864 django-hijack-3.3.0/docs/
--rw-r--r--   0 johannes   (501) wheel        (0)   118448 2023-03-15 13:45:11.000000 django-hijack-3.3.0/docs/admin-screenshot.png
--rw-r--r--   0 johannes   (501) wheel        (0)     5951 2023-03-15 13:45:11.000000 django-hijack-3.3.0/docs/customization.md
--rw-r--r--   0 johannes   (501) wheel        (0)    24164 2023-03-15 13:45:11.000000 django-hijack-3.3.0/docs/django-hijack.jpg
--rw-r--r--   0 johannes   (501) wheel        (0)     2706 2023-03-15 13:45:11.000000 django-hijack-3.3.0/docs/index.md
--rw-r--r--   0 johannes   (501) wheel        (0)    21330 2023-03-15 13:45:11.000000 django-hijack-3.3.0/docs/release-button.png
--rw-r--r--   0 johannes   (501) wheel        (0)     2528 2023-03-15 13:45:11.000000 django-hijack-3.3.0/docs/security.md
--rw-r--r--   0 johannes   (501) wheel        (0)      485 2023-03-15 13:45:11.000000 django-hijack-3.3.0/docs/troubleshooting.md
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.915710 django-hijack-3.3.0/hijack/
--rw-r--r--   0 johannes   (501) wheel        (0)       95 2023-03-15 13:45:11.000000 django-hijack-3.3.0/hijack/__init__.py
--rw-r--r--   0 johannes   (501) wheel        (0)      115 2023-03-15 13:45:11.000000 django-hijack-3.3.0/hijack/apps.py
--rw-r--r--   0 johannes   (501) wheel        (0)      413 2023-03-15 13:45:11.000000 django-hijack-3.3.0/hijack/conf.py
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.915820 django-hijack-3.3.0/hijack/contrib/
--rw-r--r--   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:11.000000 django-hijack-3.3.0/hijack/contrib/__init__.py
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.916118 django-hijack-3.3.0/hijack/contrib/admin/
--rw-r--r--   0 johannes   (501) wheel        (0)      163 2023-03-15 13:45:11.000000 django-hijack-3.3.0/hijack/contrib/admin/__init__.py
--rw-r--r--   0 johannes   (501) wheel        (0)     3393 2023-03-15 13:45:11.000000 django-hijack-3.3.0/hijack/contrib/admin/admin.py
--rw-r--r--   0 johannes   (501) wheel        (0)     1605 2023-03-15 13:45:11.000000 django-hijack-3.3.0/hijack/contrib/admin/apps.py
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.909707 django-hijack-3.3.0/hijack/contrib/admin/templates/
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.909752 django-hijack-3.3.0/hijack/contrib/admin/templates/hijack/
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.909799 django-hijack-3.3.0/hijack/contrib/admin/templates/hijack/contrib/
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.916227 django-hijack-3.3.0/hijack/contrib/admin/templates/hijack/contrib/admin/
--rw-r--r--   0 johannes   (501) wheel        (0)      430 2023-03-15 13:45:11.000000 django-hijack-3.3.0/hijack/contrib/admin/templates/hijack/contrib/admin/button.html
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.910885 django-hijack-3.3.0/hijack/locale/
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.909957 django-hijack-3.3.0/hijack/locale/cs/
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.916340 django-hijack-3.3.0/hijack/locale/cs/LC_MESSAGES/
--rw-r--r--   0 johannes   (501) wheel        (0)     1107 2023-03-15 13:45:11.000000 django-hijack-3.3.0/hijack/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.910064 django-hijack-3.3.0/hijack/locale/da/
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.916446 django-hijack-3.3.0/hijack/locale/da/LC_MESSAGES/
--rw-r--r--   0 johannes   (501) wheel        (0)     1080 2023-03-15 13:45:11.000000 django-hijack-3.3.0/hijack/locale/da/LC_MESSAGES/django.po
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.910182 django-hijack-3.3.0/hijack/locale/de/
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.916551 django-hijack-3.3.0/hijack/locale/de/LC_MESSAGES/
--rw-r--r--   0 johannes   (501) wheel        (0)     1092 2023-03-15 13:45:11.000000 django-hijack-3.3.0/hijack/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.910288 django-hijack-3.3.0/hijack/locale/es/
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.916664 django-hijack-3.3.0/hijack/locale/es/LC_MESSAGES/
--rw-r--r--   0 johannes   (501) wheel        (0)     1050 2023-03-15 13:45:11.000000 django-hijack-3.3.0/hijack/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.910397 django-hijack-3.3.0/hijack/locale/fr/
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.916773 django-hijack-3.3.0/hijack/locale/fr/LC_MESSAGES/
--rw-r--r--   0 johannes   (501) wheel        (0)     1172 2023-03-15 13:45:11.000000 django-hijack-3.3.0/hijack/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.910510 django-hijack-3.3.0/hijack/locale/ja/
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.916888 django-hijack-3.3.0/hijack/locale/ja/LC_MESSAGES/
--rw-r--r--   0 johannes   (501) wheel        (0)     1157 2023-03-15 13:45:11.000000 django-hijack-3.3.0/hijack/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.910614 django-hijack-3.3.0/hijack/locale/nl/
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.916994 django-hijack-3.3.0/hijack/locale/nl/LC_MESSAGES/
--rw-r--r--   0 johannes   (501) wheel        (0)     1218 2023-03-15 13:45:11.000000 django-hijack-3.3.0/hijack/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.910722 django-hijack-3.3.0/hijack/locale/pt_BR/
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.917104 django-hijack-3.3.0/hijack/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 johannes   (501) wheel        (0)     1094 2023-03-15 13:45:11.000000 django-hijack-3.3.0/hijack/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.910826 django-hijack-3.3.0/hijack/locale/ru/
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.917215 django-hijack-3.3.0/hijack/locale/ru/LC_MESSAGES/
--rw-r--r--   0 johannes   (501) wheel        (0)     1135 2023-03-15 13:45:11.000000 django-hijack-3.3.0/hijack/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.910929 django-hijack-3.3.0/hijack/locale/sk/
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.917326 django-hijack-3.3.0/hijack/locale/sk/LC_MESSAGES/
--rw-r--r--   0 johannes   (501) wheel        (0)     1115 2023-03-15 13:45:11.000000 django-hijack-3.3.0/hijack/locale/sk/LC_MESSAGES/django.po
--rw-r--r--   0 johannes   (501) wheel        (0)     2492 2023-03-15 13:45:11.000000 django-hijack-3.3.0/hijack/middleware.py
--rw-r--r--   0 johannes   (501) wheel        (0)      642 2023-03-15 13:45:11.000000 django-hijack-3.3.0/hijack/permissions.py
--rw-r--r--   0 johannes   (501) wheel        (0)      774 2023-03-15 13:45:11.000000 django-hijack-3.3.0/hijack/signals.py
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.911037 django-hijack-3.3.0/hijack/static/
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.917542 django-hijack-3.3.0/hijack/static/hijack/
--rw-r--r--   0 johannes   (501) wheel        (0)      743 2023-03-15 13:45:11.000000 django-hijack-3.3.0/hijack/static/hijack/hijack.js
--rw-r--r--   0 johannes   (501) wheel        (0)     1372 2023-03-15 13:45:11.000000 django-hijack-3.3.0/hijack/static/hijack/hijack.scss
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.911148 django-hijack-3.3.0/hijack/templates/
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.917659 django-hijack-3.3.0/hijack/templates/hijack/
--rw-r--r--   0 johannes   (501) wheel        (0)      912 2023-03-15 13:45:12.000000 django-hijack-3.3.0/hijack/templates/hijack/notification.html
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.917875 django-hijack-3.3.0/hijack/templatetags/
--rw-r--r--   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:12.000000 django-hijack-3.3.0/hijack/templatetags/__init__.py
--rw-r--r--   0 johannes   (501) wheel        (0)      548 2023-03-15 13:45:12.000000 django-hijack-3.3.0/hijack/templatetags/hijack.py
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.918807 django-hijack-3.3.0/hijack/tests/
--rw-r--r--   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:12.000000 django-hijack-3.3.0/hijack/tests/__init__.py
--rw-r--r--   0 johannes   (501) wheel        (0)      752 2023-03-15 13:45:12.000000 django-hijack-3.3.0/hijack/tests/conftest.py
--rw-r--r--   0 johannes   (501) wheel        (0)     2945 2023-03-15 13:45:12.000000 django-hijack-3.3.0/hijack/tests/test_admin.py
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.919688 django-hijack-3.3.0/hijack/tests/test_app/
--rw-r--r--   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:12.000000 django-hijack-3.3.0/hijack/tests/test_app/__init__.py
--rw-r--r--   0 johannes   (501) wheel        (0)      388 2023-03-15 13:45:12.000000 django-hijack-3.3.0/hijack/tests/test_app/admin.py
--rw-r--r--   0 johannes   (501) wheel        (0)      539 2023-03-15 13:45:12.000000 django-hijack-3.3.0/hijack/tests/test_app/models.py
--rw-r--r--   0 johannes   (501) wheel        (0)      110 2023-03-15 13:45:12.000000 django-hijack-3.3.0/hijack/tests/test_app/permissions.py
--rw-r--r--   0 johannes   (501) wheel        (0)     3290 2023-03-15 13:45:12.000000 django-hijack-3.3.0/hijack/tests/test_app/settings.py
-drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-03-15 13:45:31.919967 django-hijack-3.3.0/hijack/tests/test_app/templates/
--rw-r--r--   0 johannes   (501) wheel        (0)       47 2023-03-15 13:45:12.000000 django-hijack-3.3.0/hijack/tests/test_app/templates/bye_bye.html
--rw-r--r--   0 johannes   (501) wheel        (0)      460 2023-03-15 13:45:12.000000 django-hijack-3.3.0/hijack/tests/test_app/templates/user_list.html
--rw-r--r--   0 johannes   (501) wheel        (0)      536 2023-03-15 13:45:12.000000 django-hijack-3.3.0/hijack/tests/test_app/urls.py
--rw-r--r--   0 johannes   (501) wheel        (0)      371 2023-03-15 13:45:12.000000 django-hijack-3.3.0/hijack/tests/test_app/views.py
--rw-r--r--   0 johannes   (501) wheel        (0)     5821 2023-03-15 13:45:12.000000 django-hijack-3.3.0/hijack/tests/test_middleware.py
--rw-r--r--   0 johannes   (501) wheel        (0)     2008 2023-03-15 13:45:12.000000 django-hijack-3.3.0/hijack/tests/test_permissions.py
--rw-r--r--   0 johannes   (501) wheel        (0)      619 2023-03-15 13:45:12.000000 django-hijack-3.3.0/hijack/tests/test_signals.py
--rw-r--r--   0 johannes   (501) wheel        (0)      705 2023-03-15 13:45:12.000000 django-hijack-3.3.0/hijack/tests/test_templatetags.py
--rw-r--r--   0 johannes   (501) wheel        (0)     7089 2023-03-15 13:45:12.000000 django-hijack-3.3.0/hijack/tests/test_views.py
--rw-r--r--   0 johannes   (501) wheel        (0)      236 2023-03-15 13:45:12.000000 django-hijack-3.3.0/hijack/urls.py
--rwxr-xr-x   0 johannes   (501) wheel        (0)     4896 2023-03-15 13:45:12.000000 django-hijack-3.3.0/hijack/views.py
--rw-r--r--   0 johannes   (501) wheel        (0)      332 2023-03-15 13:45:12.000000 django-hijack-3.3.0/mkdocs.yml
--rw-r--r--   0 johannes   (501) wheel        (0)   353498 2023-03-15 13:45:12.000000 django-hijack-3.3.0/package-lock.json
--rw-r--r--   0 johannes   (501) wheel        (0)     1125 2023-03-15 13:45:12.000000 django-hijack-3.3.0/package.json
--rw-r--r--   0 johannes   (501) wheel        (0)       47 2023-03-15 13:45:12.000000 django-hijack-3.3.0/postcss.config.js
--rw-r--r--   0 johannes   (501) wheel        (0)     1741 2023-03-15 13:45:31.920542 django-hijack-3.3.0/setup.cfg
--rwxr-xr-x   0 johannes   (501) wheel        (0)     2301 2023-03-15 13:45:12.000000 django-hijack-3.3.0/setup.py
--rw-r--r--   0 johannes   (501) wheel        (0)      682 2023-03-15 13:45:12.000000 django-hijack-3.3.0/webpack.config.js
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.290235 django-hijack-3.4.0/
+-rw-r--r--   0 johannes   (501) wheel        (0)      350 2023-05-23 13:27:00.000000 django-hijack-3.4.0/.editorconfig
+-rw-r--r--   0 johannes   (501) wheel        (0)       25 2023-05-23 13:27:00.000000 django-hijack-3.4.0/.gitattributes
+-rw-r--r--   0 johannes   (501) wheel        (0)        6 2023-05-23 13:27:00.000000 django-hijack-3.4.0/.nvmrc
+-rw-r--r--   0 johannes   (501) wheel        (0)      364 2023-05-23 13:27:00.000000 django-hijack-3.4.0/.readthedocs.yaml
+-rw-r--r--   0 johannes   (501) wheel        (0)      129 2023-05-23 13:27:00.000000 django-hijack-3.4.0/.stylelintrc.json
+-rw-r--r--   0 johannes   (501) wheel        (0)      579 2023-05-23 13:27:00.000000 django-hijack-3.4.0/CONTRIBUTING.md
+-rw-r--r--   0 johannes   (501) wheel        (0)     1107 2023-05-23 13:27:00.000000 django-hijack-3.4.0/LICENSE
+-rw-r--r--   0 johannes   (501) wheel        (0)      138 2023-05-23 13:27:00.000000 django-hijack-3.4.0/MANIFEST.in
+-rw-r--r--   0 johannes   (501) wheel        (0)     2838 2023-05-23 13:27:59.290325 django-hijack-3.4.0/PKG-INFO
+-rw-r--r--   0 johannes   (501) wheel        (0)     1843 2023-05-23 13:27:00.000000 django-hijack-3.4.0/README.md
+-rw-r--r--   0 johannes   (501) wheel        (0)     2528 2023-05-23 13:27:00.000000 django-hijack-3.4.0/SECURITY.md
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.281928 django-hijack-3.4.0/django_hijack.egg-info/
+-rw-r--r--   0 johannes   (501) wheel        (0)     2838 2023-05-23 13:27:59.000000 django-hijack-3.4.0/django_hijack.egg-info/PKG-INFO
+-rw-r--r--   0 johannes   (501) wheel        (0)     2037 2023-05-23 13:27:59.000000 django-hijack-3.4.0/django_hijack.egg-info/SOURCES.txt
+-rw-r--r--   0 johannes   (501) wheel        (0)        1 2023-05-23 13:27:59.000000 django-hijack-3.4.0/django_hijack.egg-info/dependency_links.txt
+-rw-r--r--   0 johannes   (501) wheel        (0)       52 2023-05-23 13:27:59.000000 django-hijack-3.4.0/django_hijack.egg-info/requires.txt
+-rw-r--r--   0 johannes   (501) wheel        (0)        7 2023-05-23 13:27:59.000000 django-hijack-3.4.0/django_hijack.egg-info/top_level.txt
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.283600 django-hijack-3.4.0/docs/
+-rw-r--r--   0 johannes   (501) wheel        (0)   118448 2023-05-23 13:27:00.000000 django-hijack-3.4.0/docs/admin-screenshot.png
+-rw-r--r--   0 johannes   (501) wheel        (0)     5951 2023-05-23 13:27:00.000000 django-hijack-3.4.0/docs/customization.md
+-rw-r--r--   0 johannes   (501) wheel        (0)    24164 2023-05-23 13:27:00.000000 django-hijack-3.4.0/docs/django-hijack.jpg
+-rw-r--r--   0 johannes   (501) wheel        (0)     2706 2023-05-23 13:27:00.000000 django-hijack-3.4.0/docs/index.md
+-rw-r--r--   0 johannes   (501) wheel        (0)    21330 2023-05-23 13:27:00.000000 django-hijack-3.4.0/docs/release-button.png
+-rw-r--r--   0 johannes   (501) wheel        (0)     2528 2023-05-23 13:27:00.000000 django-hijack-3.4.0/docs/security.md
+-rw-r--r--   0 johannes   (501) wheel        (0)      485 2023-05-23 13:27:00.000000 django-hijack-3.4.0/docs/troubleshooting.md
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.284747 django-hijack-3.4.0/hijack/
+-rw-r--r--   0 johannes   (501) wheel        (0)       95 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/__init__.py
+-rw-r--r--   0 johannes   (501) wheel        (0)      115 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/apps.py
+-rw-r--r--   0 johannes   (501) wheel        (0)      413 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/conf.py
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.284896 django-hijack-3.4.0/hijack/contrib/
+-rw-r--r--   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/contrib/__init__.py
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.285285 django-hijack-3.4.0/hijack/contrib/admin/
+-rw-r--r--   0 johannes   (501) wheel        (0)      163 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/contrib/admin/__init__.py
+-rw-r--r--   0 johannes   (501) wheel        (0)     3393 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/contrib/admin/admin.py
+-rw-r--r--   0 johannes   (501) wheel        (0)     1605 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/contrib/admin/apps.py
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.275983 django-hijack-3.4.0/hijack/contrib/admin/templates/
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.276032 django-hijack-3.4.0/hijack/contrib/admin/templates/hijack/
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.276082 django-hijack-3.4.0/hijack/contrib/admin/templates/hijack/contrib/
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.285433 django-hijack-3.4.0/hijack/contrib/admin/templates/hijack/contrib/admin/
+-rw-r--r--   0 johannes   (501) wheel        (0)      430 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/contrib/admin/templates/hijack/contrib/admin/button.html
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.277326 django-hijack-3.4.0/hijack/locale/
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.276247 django-hijack-3.4.0/hijack/locale/cs/
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.285583 django-hijack-3.4.0/hijack/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 johannes   (501) wheel        (0)     1107 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.276359 django-hijack-3.4.0/hijack/locale/da/
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.285723 django-hijack-3.4.0/hijack/locale/da/LC_MESSAGES/
+-rw-r--r--   0 johannes   (501) wheel        (0)     1080 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/locale/da/LC_MESSAGES/django.po
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.276477 django-hijack-3.4.0/hijack/locale/de/
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.285871 django-hijack-3.4.0/hijack/locale/de/LC_MESSAGES/
+-rw-r--r--   0 johannes   (501) wheel        (0)     1092 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.276589 django-hijack-3.4.0/hijack/locale/es/
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.286013 django-hijack-3.4.0/hijack/locale/es/LC_MESSAGES/
+-rw-r--r--   0 johannes   (501) wheel        (0)     1050 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.276705 django-hijack-3.4.0/hijack/locale/fr/
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.286161 django-hijack-3.4.0/hijack/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 johannes   (501) wheel        (0)     1172 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.276818 django-hijack-3.4.0/hijack/locale/ja/
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.286312 django-hijack-3.4.0/hijack/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 johannes   (501) wheel        (0)     1157 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.276928 django-hijack-3.4.0/hijack/locale/nl/
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.286455 django-hijack-3.4.0/hijack/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 johannes   (501) wheel        (0)     1218 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.277040 django-hijack-3.4.0/hijack/locale/pl/
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.286603 django-hijack-3.4.0/hijack/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 johannes   (501) wheel        (0)     1136 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.277151 django-hijack-3.4.0/hijack/locale/pt_BR/
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.286755 django-hijack-3.4.0/hijack/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 johannes   (501) wheel        (0)     1094 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.277262 django-hijack-3.4.0/hijack/locale/ru/
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.286902 django-hijack-3.4.0/hijack/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 johannes   (501) wheel        (0)     1135 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.277376 django-hijack-3.4.0/hijack/locale/sk/
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.287050 django-hijack-3.4.0/hijack/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 johannes   (501) wheel        (0)     1115 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/locale/sk/LC_MESSAGES/django.po
+-rw-r--r--   0 johannes   (501) wheel        (0)     2492 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/middleware.py
+-rw-r--r--   0 johannes   (501) wheel        (0)      642 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/permissions.py
+-rw-r--r--   0 johannes   (501) wheel        (0)      774 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/signals.py
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.277485 django-hijack-3.4.0/hijack/static/
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.287343 django-hijack-3.4.0/hijack/static/hijack/
+-rw-r--r--   0 johannes   (501) wheel        (0)      743 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/static/hijack/hijack.js
+-rw-r--r--   0 johannes   (501) wheel        (0)     1372 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/static/hijack/hijack.scss
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.277595 django-hijack-3.4.0/hijack/templates/
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.287476 django-hijack-3.4.0/hijack/templates/hijack/
+-rw-r--r--   0 johannes   (501) wheel        (0)      912 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/templates/hijack/notification.html
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.287700 django-hijack-3.4.0/hijack/templatetags/
+-rw-r--r--   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/templatetags/__init__.py
+-rw-r--r--   0 johannes   (501) wheel        (0)      548 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/templatetags/hijack.py
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.288698 django-hijack-3.4.0/hijack/tests/
+-rw-r--r--   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/tests/__init__.py
+-rw-r--r--   0 johannes   (501) wheel        (0)      752 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/tests/conftest.py
+-rw-r--r--   0 johannes   (501) wheel        (0)     2945 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/tests/test_admin.py
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.289578 django-hijack-3.4.0/hijack/tests/test_app/
+-rw-r--r--   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/tests/test_app/__init__.py
+-rw-r--r--   0 johannes   (501) wheel        (0)      388 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/tests/test_app/admin.py
+-rw-r--r--   0 johannes   (501) wheel        (0)      539 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/tests/test_app/models.py
+-rw-r--r--   0 johannes   (501) wheel        (0)      110 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/tests/test_app/permissions.py
+-rw-r--r--   0 johannes   (501) wheel        (0)     3290 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/tests/test_app/settings.py
+drwxr-xr-x   0 johannes   (501) wheel        (0)        0 2023-05-23 13:27:59.290069 django-hijack-3.4.0/hijack/tests/test_app/templates/
+-rw-r--r--   0 johannes   (501) wheel        (0)       47 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/tests/test_app/templates/bye_bye.html
+-rw-r--r--   0 johannes   (501) wheel        (0)      460 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/tests/test_app/templates/user_list.html
+-rw-r--r--   0 johannes   (501) wheel        (0)      536 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/tests/test_app/urls.py
+-rw-r--r--   0 johannes   (501) wheel        (0)      371 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/tests/test_app/views.py
+-rw-r--r--   0 johannes   (501) wheel        (0)     5821 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/tests/test_middleware.py
+-rw-r--r--   0 johannes   (501) wheel        (0)     2008 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/tests/test_permissions.py
+-rw-r--r--   0 johannes   (501) wheel        (0)      619 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/tests/test_signals.py
+-rw-r--r--   0 johannes   (501) wheel        (0)      705 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/tests/test_templatetags.py
+-rw-r--r--   0 johannes   (501) wheel        (0)     7089 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/tests/test_views.py
+-rw-r--r--   0 johannes   (501) wheel        (0)      236 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/urls.py
+-rwxr-xr-x   0 johannes   (501) wheel        (0)     4896 2023-05-23 13:27:00.000000 django-hijack-3.4.0/hijack/views.py
+-rw-r--r--   0 johannes   (501) wheel        (0)      332 2023-05-23 13:27:00.000000 django-hijack-3.4.0/mkdocs.yml
+-rw-r--r--   0 johannes   (501) wheel        (0)   357954 2023-05-23 13:27:00.000000 django-hijack-3.4.0/package-lock.json
+-rw-r--r--   0 johannes   (501) wheel        (0)     1124 2023-05-23 13:27:00.000000 django-hijack-3.4.0/package.json
+-rw-r--r--   0 johannes   (501) wheel        (0)       47 2023-05-23 13:27:00.000000 django-hijack-3.4.0/postcss.config.js
+-rw-r--r--   0 johannes   (501) wheel        (0)     1742 2023-05-23 13:27:59.290749 django-hijack-3.4.0/setup.cfg
+-rwxr-xr-x   0 johannes   (501) wheel        (0)     2581 2023-05-23 13:27:00.000000 django-hijack-3.4.0/setup.py
+-rw-r--r--   0 johannes   (501) wheel        (0)      682 2023-05-23 13:27:00.000000 django-hijack-3.4.0/webpack.config.js
```

### Comparing `django-hijack-3.3.0/CONTRIBUTING.md` & `django-hijack-3.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/LICENSE` & `django-hijack-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/PKG-INFO` & `django-hijack-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-hijack
-Version: 3.3.0
+Version: 3.4.0
 Summary: django-hijack allows superusers to hijack (=login as) and work on behalf of another user.
 Home-page: https://github.com/django-hijack/django-hijack
 Author: arteria GmbH
 Author-email: admin@arteria.ch
 License: MIT
 Keywords: django,hijack,support,customer support,debugging
 Platform: OS Independent
```

### Comparing `django-hijack-3.3.0/README.md` & `django-hijack-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/SECURITY.md` & `django-hijack-3.4.0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/django_hijack.egg-info/PKG-INFO` & `django-hijack-3.4.0/django_hijack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-hijack
-Version: 3.3.0
+Version: 3.4.0
 Summary: django-hijack allows superusers to hijack (=login as) and work on behalf of another user.
 Home-page: https://github.com/django-hijack/django-hijack
 Author: arteria GmbH
 Author-email: admin@arteria.ch
 License: MIT
 Keywords: django,hijack,support,customer support,debugging
 Platform: OS Independent
```

### Comparing `django-hijack-3.3.0/django_hijack.egg-info/SOURCES.txt` & `django-hijack-3.4.0/django_hijack.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 hijack/locale/cs/LC_MESSAGES/django.po
 hijack/locale/da/LC_MESSAGES/django.po
 hijack/locale/de/LC_MESSAGES/django.po
 hijack/locale/es/LC_MESSAGES/django.po
 hijack/locale/fr/LC_MESSAGES/django.po
 hijack/locale/ja/LC_MESSAGES/django.po
 hijack/locale/nl/LC_MESSAGES/django.po
+hijack/locale/pl/LC_MESSAGES/django.po
 hijack/locale/pt_BR/LC_MESSAGES/django.po
 hijack/locale/ru/LC_MESSAGES/django.po
 hijack/locale/sk/LC_MESSAGES/django.po
 hijack/static/hijack/hijack.js
 hijack/static/hijack/hijack.scss
 hijack/templates/hijack/notification.html
 hijack/templatetags/__init__.py
```

### Comparing `django-hijack-3.3.0/docs/admin-screenshot.png` & `django-hijack-3.4.0/docs/admin-screenshot.png`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/docs/customization.md` & `django-hijack-3.4.0/docs/customization.md`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/docs/django-hijack.jpg` & `django-hijack-3.4.0/docs/django-hijack.jpg`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/docs/index.md` & `django-hijack-3.4.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/docs/release-button.png` & `django-hijack-3.4.0/docs/release-button.png`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/docs/security.md` & `django-hijack-3.4.0/docs/security.md`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/hijack/contrib/admin/admin.py` & `django-hijack-3.4.0/hijack/contrib/admin/admin.py`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/hijack/contrib/admin/apps.py` & `django-hijack-3.4.0/hijack/contrib/admin/apps.py`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/hijack/locale/cs/LC_MESSAGES/django.po` & `django-hijack-3.4.0/hijack/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/hijack/locale/da/LC_MESSAGES/django.po` & `django-hijack-3.4.0/hijack/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/hijack/locale/de/LC_MESSAGES/django.po` & `django-hijack-3.4.0/hijack/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/hijack/locale/es/LC_MESSAGES/django.po` & `django-hijack-3.4.0/hijack/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/hijack/locale/fr/LC_MESSAGES/django.po` & `django-hijack-3.4.0/hijack/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/hijack/locale/ja/LC_MESSAGES/django.po` & `django-hijack-3.4.0/hijack/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/hijack/locale/nl/LC_MESSAGES/django.po` & `django-hijack-3.4.0/hijack/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/hijack/locale/pt_BR/LC_MESSAGES/django.po` & `django-hijack-3.4.0/hijack/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/hijack/locale/ru/LC_MESSAGES/django.po` & `django-hijack-3.4.0/hijack/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/hijack/locale/sk/LC_MESSAGES/django.po` & `django-hijack-3.4.0/hijack/locale/sk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/hijack/middleware.py` & `django-hijack-3.4.0/hijack/middleware.py`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/hijack/permissions.py` & `django-hijack-3.4.0/hijack/permissions.py`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/hijack/signals.py` & `django-hijack-3.4.0/hijack/signals.py`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/hijack/static/hijack/hijack.js` & `django-hijack-3.4.0/hijack/static/hijack/hijack.js`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/hijack/static/hijack/hijack.scss` & `django-hijack-3.4.0/hijack/static/hijack/hijack.scss`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/hijack/templates/hijack/notification.html` & `django-hijack-3.4.0/hijack/templates/hijack/notification.html`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/hijack/templatetags/hijack.py` & `django-hijack-3.4.0/hijack/templatetags/hijack.py`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/hijack/tests/conftest.py` & `django-hijack-3.4.0/hijack/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/hijack/tests/test_admin.py` & `django-hijack-3.4.0/hijack/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/hijack/tests/test_app/models.py` & `django-hijack-3.4.0/hijack/tests/test_app/models.py`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/hijack/tests/test_app/settings.py` & `django-hijack-3.4.0/hijack/tests/test_app/settings.py`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/hijack/tests/test_app/urls.py` & `django-hijack-3.4.0/hijack/tests/test_app/urls.py`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/hijack/tests/test_middleware.py` & `django-hijack-3.4.0/hijack/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/hijack/tests/test_permissions.py` & `django-hijack-3.4.0/hijack/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/hijack/tests/test_signals.py` & `django-hijack-3.4.0/hijack/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/hijack/tests/test_templatetags.py` & `django-hijack-3.4.0/hijack/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/hijack/tests/test_views.py` & `django-hijack-3.4.0/hijack/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/hijack/views.py` & `django-hijack-3.4.0/hijack/views.py`

 * *Files identical despite different names*

### Comparing `django-hijack-3.3.0/package-lock.json` & `django-hijack-3.4.0/package-lock.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9915293057018831%*

 * *Differences: {"'dependencies'": "{'@csstools/selector-specificity': {'version': '2.2.0', 'resolved': "*

 * *                   "'https://registry.npmjs.org/@csstools/selector-specificity/-/selector-specificity-2.2.0.tgz', "*

 * *                   "'integrity': "*

 * *                   "'sha512-+OJ9konv95ClSTOJCmMZqpd5+YGsB2S+x6w3E1oaM8UuR5j8nTNHYSz8c9BEPGDOCMQYIEEGlVPj/VY64iTbGw=='}, "*

 * *                   "'@jridgewell/gen-mapping': {'version': '0.3.3', 'resolved': "*

 * *                   "'https://registry.npmjs.org/@jridgewell/gen-map […]*

```diff
@@ -22,20 +22,40 @@
                 "@babel/helper-validator-identifier": "^7.16.7",
                 "chalk": "^2.0.0",
                 "js-tokens": "^4.0.0"
             },
             "resolved": "https://registry.npmjs.org/@babel/highlight/-/highlight-7.16.10.tgz",
             "version": "7.16.10"
         },
+        "@csstools/css-parser-algorithms": {
+            "dev": true,
+            "integrity": "sha512-viRnRh02AgO4mwIQb2xQNJju0i+Fh9roNgmbR5xEuG7J3TGgxjnE95HnBLgsFJOJOksvcfxOUCgODcft6Y07cA==",
+            "requires": {},
+            "resolved": "https://registry.npmjs.org/@csstools/css-parser-algorithms/-/css-parser-algorithms-2.1.1.tgz",
+            "version": "2.1.1"
+        },
+        "@csstools/css-tokenizer": {
+            "dev": true,
+            "integrity": "sha512-GbrTj2Z8MCTUv+52GE0RbFGM527xuXZ0Xa5g0Z+YN573uveS4G0qi6WNOMyz3yrFM/jaILTTwJ0+umx81EzqfA==",
+            "resolved": "https://registry.npmjs.org/@csstools/css-tokenizer/-/css-tokenizer-2.1.1.tgz",
+            "version": "2.1.1"
+        },
+        "@csstools/media-query-list-parser": {
+            "dev": true,
+            "integrity": "sha512-GyYot6jHgcSDZZ+tLSnrzkR7aJhF2ZW6d+CXH66mjy5WpAQhZD4HDke2OQ36SivGRWlZJpAz7TzbW6OKlEpxAA==",
+            "requires": {},
+            "resolved": "https://registry.npmjs.org/@csstools/media-query-list-parser/-/media-query-list-parser-2.0.4.tgz",
+            "version": "2.0.4"
+        },
         "@csstools/selector-specificity": {
             "dev": true,
-            "integrity": "sha512-IkpVW/ehM1hWKln4fCA3NzJU8KwD+kIOvPZA4cqxoJHtE21CCzjyp+Kxbu0i5I4tBNOlXPL9mjwnWlL0VEG4Fg==",
+            "integrity": "sha512-+OJ9konv95ClSTOJCmMZqpd5+YGsB2S+x6w3E1oaM8UuR5j8nTNHYSz8c9BEPGDOCMQYIEEGlVPj/VY64iTbGw==",
             "requires": {},
-            "resolved": "https://registry.npmjs.org/@csstools/selector-specificity/-/selector-specificity-2.0.2.tgz",
-            "version": "2.0.2"
+            "resolved": "https://registry.npmjs.org/@csstools/selector-specificity/-/selector-specificity-2.2.0.tgz",
+            "version": "2.2.0"
         },
         "@discoveryjs/json-ext": {
             "dev": true,
             "integrity": "sha512-dBVuXR082gk3jsFp7Rd/JI4kytwGHecnCoTtXFb7DB6CNHp4rg5k1bhg0nWdLGLnOV71lmDzGQaLMy8iPLY0pw==",
             "resolved": "https://registry.npmjs.org/@discoveryjs/json-ext/-/json-ext-0.5.7.tgz",
             "version": "0.5.7"
         },
@@ -91,22 +111,22 @@
             "dev": true,
             "integrity": "sha512-ZnQMnLV4e7hDlUvw8H+U8ASL02SS2Gn6+9Ac3wGGLIe7+je2AeAOxPY+izIPJDfFDb7eDjev0Us8MO1iFRN8hA==",
             "resolved": "https://registry.npmjs.org/@humanwhocodes/object-schema/-/object-schema-1.2.1.tgz",
             "version": "1.2.1"
         },
         "@jridgewell/gen-mapping": {
             "dev": true,
-            "integrity": "sha512-mh65xKQAzI6iBcFzwv28KVWSmCkdRBWoOh+bYQGW3+6OZvbbN3TqMGo5hqYxQniRcH9F2VZIoJCm4pa3BPDK/A==",
+            "integrity": "sha512-HLhSWOLRi875zjjMG/r+Nv0oCW8umGb0BgEhyX3dDX3egwZtB8PqLnjz3yedt8R5StBrzcg4aBpnh8UA9D1BoQ==",
             "requires": {
                 "@jridgewell/set-array": "^1.0.1",
                 "@jridgewell/sourcemap-codec": "^1.4.10",
                 "@jridgewell/trace-mapping": "^0.3.9"
             },
-            "resolved": "https://registry.npmjs.org/@jridgewell/gen-mapping/-/gen-mapping-0.3.2.tgz",
-            "version": "0.3.2"
+            "resolved": "https://registry.npmjs.org/@jridgewell/gen-mapping/-/gen-mapping-0.3.3.tgz",
+            "version": "0.3.3"
         },
         "@jridgewell/resolve-uri": {
             "dev": true,
             "integrity": "sha512-F2msla3tad+Mfht5cJq7LSXcdudKTWCVYUgw6pLFOOHSTtZlj6SWNYAp+AhuqLmWdBO2X5hPrLcu8cVP8fy28w==",
             "resolved": "https://registry.npmjs.org/@jridgewell/resolve-uri/-/resolve-uri-3.1.0.tgz",
             "version": "3.1.0"
         },
@@ -114,37 +134,37 @@
             "dev": true,
             "integrity": "sha512-xnkseuNADM0gt2bs+BvhO0p78Mk762YnZdsuzFV018NoG1Sj1SCQvpSqa7XUaTam5vAGasABV9qXASMKnFMwMw==",
             "resolved": "https://registry.npmjs.org/@jridgewell/set-array/-/set-array-1.1.2.tgz",
             "version": "1.1.2"
         },
         "@jridgewell/source-map": {
             "dev": true,
-            "integrity": "sha512-m7O9o2uR8k2ObDysZYzdfhb08VuEml5oWGiosa1VdaPZ/A6QyPkAJuwN0Q1lhULOf6B7MtQmHENS743hWtCrgw==",
+            "integrity": "sha512-b+fsZXeLYi9fEULmfBrhxn4IrPlINf8fiNarzTof004v3lFdntdwa9PF7vFJqm3mg7s+ScJMxXaE3Acp1irZcg==",
             "requires": {
                 "@jridgewell/gen-mapping": "^0.3.0",
                 "@jridgewell/trace-mapping": "^0.3.9"
             },
-            "resolved": "https://registry.npmjs.org/@jridgewell/source-map/-/source-map-0.3.2.tgz",
-            "version": "0.3.2"
+            "resolved": "https://registry.npmjs.org/@jridgewell/source-map/-/source-map-0.3.3.tgz",
+            "version": "0.3.3"
         },
         "@jridgewell/sourcemap-codec": {
             "dev": true,
             "integrity": "sha512-XPSJHWmi394fuUuzDnGz1wiKqWfo1yXecHQMRf2l6hztTO+nPru658AyDngaBe7isIxEkRsPR3FZh+s7iVa4Uw==",
             "resolved": "https://registry.npmjs.org/@jridgewell/sourcemap-codec/-/sourcemap-codec-1.4.14.tgz",
             "version": "1.4.14"
         },
         "@jridgewell/trace-mapping": {
             "dev": true,
-            "integrity": "sha512-bJWEfQ9lPTvm3SneWwRFVLzrh6nhjwqw7TUFFBEMzwvg7t7PCDenf2lDwqo4NQXzdpgBXyFgDWnQA+2vkruksQ==",
+            "integrity": "sha512-w+niJYzMHdd7USdiH2U6869nqhD2nbfZXND5Yp93qIbEmnDNk7PD48o+YchRVpzMU7M6jVCbenTR7PA1FLQ9pA==",
             "requires": {
-                "@jridgewell/resolve-uri": "^3.0.3",
-                "@jridgewell/sourcemap-codec": "^1.4.10"
+                "@jridgewell/resolve-uri": "3.1.0",
+                "@jridgewell/sourcemap-codec": "1.4.14"
             },
-            "resolved": "https://registry.npmjs.org/@jridgewell/trace-mapping/-/trace-mapping-0.3.14.tgz",
-            "version": "0.3.14"
+            "resolved": "https://registry.npmjs.org/@jridgewell/trace-mapping/-/trace-mapping-0.3.18.tgz",
+            "version": "0.3.18"
         },
         "@nodelib/fs.scandir": {
             "dev": true,
             "integrity": "sha512-vq24Bq3ym5HEQm2NKCr3yXDwjc7vTsEThRDnkp2DK9p1uqLR+DHurm/NOTo0KG7HYHU7eppKZj3MyqYuMBf62g==",
             "requires": {
                 "@nodelib/fs.stat": "2.0.5",
                 "run-parallel": "^1.1.9"
@@ -186,17 +206,17 @@
                 "@types/estree": "*"
             },
             "resolved": "https://registry.npmjs.org/@types/eslint-scope/-/eslint-scope-3.7.3.tgz",
             "version": "3.7.3"
         },
         "@types/estree": {
             "dev": true,
-            "integrity": "sha512-CuPgU6f3eT/XgKKPqKd/gLZV1Xmvf1a2R5POBOGQa6uv82xpls89HU5zKeVoyR8XzHd1RGNOlQlvUe3CFkjWNQ==",
-            "resolved": "https://registry.npmjs.org/@types/estree/-/estree-0.0.51.tgz",
-            "version": "0.0.51"
+            "integrity": "sha512-LG4opVs2ANWZ1TJoKc937iMmNstM/d0ae1vNbnBvBhqCSezgVUOzcLCqbI5elV8Vy6WKwKjaqR+zO9VKirBBCA==",
+            "resolved": "https://registry.npmjs.org/@types/estree/-/estree-1.0.1.tgz",
+            "version": "1.0.1"
         },
         "@types/json-schema": {
             "dev": true,
             "integrity": "sha512-wOuvG1SN4Us4rez+tylwwwCV1psiNVOkJeM3AUWUNWg/jDQY2+HE/444y5gc+jBmRqASOm2Oeh5c1axHobwRKQ==",
             "resolved": "https://registry.npmjs.org/@types/json-schema/-/json-schema-7.0.11.tgz",
             "version": "7.0.11"
         },
@@ -210,196 +230,190 @@
             "dev": true,
             "integrity": "sha512-jhuKLIRrhvCPLqwPcx6INqmKeiA5EWrsCOPhrlFSrbrmU4ZMPjj5Ul/oLCMDO98XRUIwVm78xICz4EPCektzeQ==",
             "resolved": "https://registry.npmjs.org/@types/minimist/-/minimist-1.2.2.tgz",
             "version": "1.2.2"
         },
         "@types/node": {
             "dev": true,
-            "integrity": "sha512-UxDxWn7dl97rKVeVS61vErvw086aCYhDLyvRQZ5Rk65rZKepaFdm53GeqXaKBuOhED4e9uWq34IC3TdSdJJ2Gw==",
-            "resolved": "https://registry.npmjs.org/@types/node/-/node-17.0.23.tgz",
-            "version": "17.0.23"
+            "integrity": "sha512-OPs5WnnT1xkCBiuQrZA4+YAV4HEJejmHneyraIaxsbev5yCEr6KMwINNFP9wQeFIw8FWcoTqF3vQsa5CDaI+8Q==",
+            "resolved": "https://registry.npmjs.org/@types/node/-/node-18.16.3.tgz",
+            "version": "18.16.3"
         },
         "@types/normalize-package-data": {
             "dev": true,
             "integrity": "sha512-Gj7cI7z+98M282Tqmp2K5EIsoouUEzbBJhQQzDE3jSIRk6r9gsz0oUokqIUR4u1R3dMHo0pDHM7sNOHyhulypw==",
             "resolved": "https://registry.npmjs.org/@types/normalize-package-data/-/normalize-package-data-2.4.1.tgz",
             "version": "2.4.1"
         },
-        "@types/parse-json": {
-            "dev": true,
-            "integrity": "sha512-//oorEZjL6sbPcKUaCdIGlIUeH26mgzimjBB77G6XRgnDl/L5wOnpyBGRe/Mmf5CVW3PwEBE1NjiMZ/ssFh4wA==",
-            "resolved": "https://registry.npmjs.org/@types/parse-json/-/parse-json-4.0.0.tgz",
-            "version": "4.0.0"
-        },
         "@webassemblyjs/ast": {
             "dev": true,
-            "integrity": "sha512-ukBh14qFLjxTQNTXocdyksN5QdM28S1CxHt2rdskFyL+xFV7VremuBLVbmCePj+URalXBENx/9Lm7lnhihtCSw==",
+            "integrity": "sha512-LHY/GSAZZRpsNQH+/oHqhRQ5FT7eoULcBqgfyTB5nQHogFnK3/7QoN7dLnwSE/JkUAF0SrRuclT7ODqMFtWxxQ==",
             "requires": {
-                "@webassemblyjs/helper-numbers": "1.11.1",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.1"
+                "@webassemblyjs/helper-numbers": "1.11.5",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.5"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/ast/-/ast-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/ast/-/ast-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/floating-point-hex-parser": {
             "dev": true,
-            "integrity": "sha512-iGRfyc5Bq+NnNuX8b5hwBrRjzf0ocrJPI6GWFodBFzmFnyvrQ83SHKhmilCU/8Jv67i4GJZBMhEzltxzcNagtQ==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/floating-point-hex-parser/-/floating-point-hex-parser-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-1j1zTIC5EZOtCplMBG/IEwLtUojtwFVwdyVMbL/hwWqbzlQoJsWCOavrdnLkemwNoC/EOwtUFch3fuo+cbcXYQ==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/floating-point-hex-parser/-/floating-point-hex-parser-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/helper-api-error": {
             "dev": true,
-            "integrity": "sha512-RlhS8CBCXfRUR/cwo2ho9bkheSXG0+NwooXcc3PAILALf2QLdFyj7KGsKRbVc95hZnhnERon4kW/D3SZpp6Tcg==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-api-error/-/helper-api-error-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-L65bDPmfpY0+yFrsgz8b6LhXmbbs38OnwDCf6NpnMUYqa+ENfE5Dq9E42ny0qz/PdR0LJyq/T5YijPnU8AXEpA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-api-error/-/helper-api-error-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/helper-buffer": {
             "dev": true,
-            "integrity": "sha512-gwikF65aDNeeXa8JxXa2BAk+REjSyhrNC9ZwdT0f8jc4dQQeDQ7G4m0f2QCLPJiMTTO6wfDmRmj/pW0PsUvIcA==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-buffer/-/helper-buffer-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-fDKo1gstwFFSfacIeH5KfwzjykIE6ldh1iH9Y/8YkAZrhmu4TctqYjSh7t0K2VyDSXOZJ1MLhht/k9IvYGcIxg==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-buffer/-/helper-buffer-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/helper-numbers": {
             "dev": true,
-            "integrity": "sha512-vDkbxiB8zfnPdNK9Rajcey5C0w+QJugEglN0of+kmO8l7lDb77AnlKYQF7aarZuCrv+l0UvqL+68gSDr3k9LPQ==",
+            "integrity": "sha512-DhykHXM0ZABqfIGYNv93A5KKDw/+ywBFnuWybZZWcuzWHfbp21wUfRkbtz7dMGwGgT4iXjWuhRMA2Mzod6W4WA==",
             "requires": {
-                "@webassemblyjs/floating-point-hex-parser": "1.11.1",
-                "@webassemblyjs/helper-api-error": "1.11.1",
+                "@webassemblyjs/floating-point-hex-parser": "1.11.5",
+                "@webassemblyjs/helper-api-error": "1.11.5",
                 "@xtuc/long": "4.2.2"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-numbers/-/helper-numbers-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-numbers/-/helper-numbers-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/helper-wasm-bytecode": {
             "dev": true,
-            "integrity": "sha512-PvpoOGiJwXeTrSf/qfudJhwlvDQxFgelbMqtq52WWiXC6Xgg1IREdngmPN3bs4RoO83PnL/nFrxucXj1+BX62Q==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-bytecode/-/helper-wasm-bytecode-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-oC4Qa0bNcqnjAowFn7MPCETQgDYytpsfvz4ujZz63Zu/a/v71HeCAAmZsgZ3YVKec3zSPYytG3/PrRCqbtcAvA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-bytecode/-/helper-wasm-bytecode-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/helper-wasm-section": {
             "dev": true,
-            "integrity": "sha512-10P9No29rYX1j7F3EVPX3JvGPQPae+AomuSTPiF9eBQeChHI6iqjMIwR9JmOJXwpnn/oVGDk7I5IlskuMwU/pg==",
+            "integrity": "sha512-uEoThA1LN2NA+K3B9wDo3yKlBfVtC6rh0i4/6hvbz071E8gTNZD/pT0MsBf7MeD6KbApMSkaAK0XeKyOZC7CIA==",
             "requires": {
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/helper-buffer": "1.11.1",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.1",
-                "@webassemblyjs/wasm-gen": "1.11.1"
+                "@webassemblyjs/ast": "1.11.5",
+                "@webassemblyjs/helper-buffer": "1.11.5",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.5",
+                "@webassemblyjs/wasm-gen": "1.11.5"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-section/-/helper-wasm-section-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-section/-/helper-wasm-section-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/ieee754": {
             "dev": true,
-            "integrity": "sha512-hJ87QIPtAMKbFq6CGTkZYJivEwZDbQUgYd3qKSadTNOhVY7p+gfP6Sr0lLRVTaG1JjFj+r3YchoqRYxNH3M0GQ==",
+            "integrity": "sha512-37aGq6qVL8A8oPbPrSGMBcp38YZFXcHfiROflJn9jxSdSMMM5dS5P/9e2/TpaJuhE+wFrbukN2WI6Hw9MH5acg==",
             "requires": {
                 "@xtuc/ieee754": "^1.2.0"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/ieee754/-/ieee754-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/ieee754/-/ieee754-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/leb128": {
             "dev": true,
-            "integrity": "sha512-BJ2P0hNZ0u+Th1YZXJpzW6miwqQUGcIHT1G/sf72gLVD9DZ5AdYTqPNbHZh6K1M5VmKvFXwGSWZADz+qBWxeRw==",
+            "integrity": "sha512-ajqrRSXaTJoPW+xmkfYN6l8VIeNnR4vBOTQO9HzR7IygoCcKWkICbKFbVTNMjMgMREqXEr0+2M6zukzM47ZUfQ==",
             "requires": {
                 "@xtuc/long": "4.2.2"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/leb128/-/leb128-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/leb128/-/leb128-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/utf8": {
             "dev": true,
-            "integrity": "sha512-9kqcxAEdMhiwQkHpkNiorZzqpGrodQQ2IGrHHxCy+Ozng0ofyMA0lTqiLkVs1uzTRejX+/O0EOT7KxqVPuXosQ==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/utf8/-/utf8-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-WiOhulHKTZU5UPlRl53gHR8OxdGsSOxqfpqWeA2FmcwBMaoEdz6b2x2si3IwC9/fSPLfe8pBMRTHVMk5nlwnFQ==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/utf8/-/utf8-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/wasm-edit": {
             "dev": true,
-            "integrity": "sha512-g+RsupUC1aTHfR8CDgnsVRVZFJqdkFHpsHMfJuWQzWU3tvnLC07UqHICfP+4XyL2tnr1amvl1Sdp06TnYCmVkA==",
+            "integrity": "sha512-C0p9D2fAu3Twwqvygvf42iGCQ4av8MFBLiTb+08SZ4cEdwzWx9QeAHDo1E2k+9s/0w1DM40oflJOpkZ8jW4HCQ==",
             "requires": {
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/helper-buffer": "1.11.1",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.1",
-                "@webassemblyjs/helper-wasm-section": "1.11.1",
-                "@webassemblyjs/wasm-gen": "1.11.1",
-                "@webassemblyjs/wasm-opt": "1.11.1",
-                "@webassemblyjs/wasm-parser": "1.11.1",
-                "@webassemblyjs/wast-printer": "1.11.1"
+                "@webassemblyjs/ast": "1.11.5",
+                "@webassemblyjs/helper-buffer": "1.11.5",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.5",
+                "@webassemblyjs/helper-wasm-section": "1.11.5",
+                "@webassemblyjs/wasm-gen": "1.11.5",
+                "@webassemblyjs/wasm-opt": "1.11.5",
+                "@webassemblyjs/wasm-parser": "1.11.5",
+                "@webassemblyjs/wast-printer": "1.11.5"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-edit/-/wasm-edit-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-edit/-/wasm-edit-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/wasm-gen": {
             "dev": true,
-            "integrity": "sha512-F7QqKXwwNlMmsulj6+O7r4mmtAlCWfO/0HdgOxSklZfQcDu0TpLiD1mRt/zF25Bk59FIjEuGAIyn5ei4yMfLhA==",
+            "integrity": "sha512-14vteRlRjxLK9eSyYFvw1K8Vv+iPdZU0Aebk3j6oB8TQiQYuO6hj9s4d7qf6f2HJr2khzvNldAFG13CgdkAIfA==",
             "requires": {
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.1",
-                "@webassemblyjs/ieee754": "1.11.1",
-                "@webassemblyjs/leb128": "1.11.1",
-                "@webassemblyjs/utf8": "1.11.1"
+                "@webassemblyjs/ast": "1.11.5",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.5",
+                "@webassemblyjs/ieee754": "1.11.5",
+                "@webassemblyjs/leb128": "1.11.5",
+                "@webassemblyjs/utf8": "1.11.5"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-gen/-/wasm-gen-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-gen/-/wasm-gen-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/wasm-opt": {
             "dev": true,
-            "integrity": "sha512-VqnkNqnZlU5EB64pp1l7hdm3hmQw7Vgqa0KF/KCNO9sIpI6Fk6brDEiX+iCOYrvMuBWDws0NkTOxYEb85XQHHw==",
+            "integrity": "sha512-tcKwlIXstBQgbKy1MlbDMlXaxpucn42eb17H29rawYLxm5+MsEmgPzeCP8B1Cl69hCice8LeKgZpRUAPtqYPgw==",
             "requires": {
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/helper-buffer": "1.11.1",
-                "@webassemblyjs/wasm-gen": "1.11.1",
-                "@webassemblyjs/wasm-parser": "1.11.1"
+                "@webassemblyjs/ast": "1.11.5",
+                "@webassemblyjs/helper-buffer": "1.11.5",
+                "@webassemblyjs/wasm-gen": "1.11.5",
+                "@webassemblyjs/wasm-parser": "1.11.5"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-opt/-/wasm-opt-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-opt/-/wasm-opt-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/wasm-parser": {
             "dev": true,
-            "integrity": "sha512-rrBujw+dJu32gYB7/Lup6UhdkPx9S9SnobZzRVL7VcBH9Bt9bCBLEuX/YXOOtBsOZ4NQrRykKhffRWHvigQvOA==",
+            "integrity": "sha512-SVXUIwsLQlc8srSD7jejsfTU83g7pIGr2YYNb9oHdtldSxaOhvA5xwvIiWIfcX8PlSakgqMXsLpLfbbJ4cBYew==",
             "requires": {
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/helper-api-error": "1.11.1",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.1",
-                "@webassemblyjs/ieee754": "1.11.1",
-                "@webassemblyjs/leb128": "1.11.1",
-                "@webassemblyjs/utf8": "1.11.1"
+                "@webassemblyjs/ast": "1.11.5",
+                "@webassemblyjs/helper-api-error": "1.11.5",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.5",
+                "@webassemblyjs/ieee754": "1.11.5",
+                "@webassemblyjs/leb128": "1.11.5",
+                "@webassemblyjs/utf8": "1.11.5"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-parser/-/wasm-parser-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-parser/-/wasm-parser-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webassemblyjs/wast-printer": {
             "dev": true,
-            "integrity": "sha512-IQboUWM4eKzWW+N/jij2sRatKMh99QEelo3Eb2q0qXkvPRISAj8Qxtmw5itwqK+TTkBuUIE45AxYPToqPtL5gg==",
+            "integrity": "sha512-f7Pq3wvg3GSPUPzR0F6bmI89Hdb+u9WXrSKc4v+N0aV0q6r42WoF92Jp2jEorBEBRoRNXgjp53nBniDXcqZYPA==",
             "requires": {
-                "@webassemblyjs/ast": "1.11.1",
+                "@webassemblyjs/ast": "1.11.5",
                 "@xtuc/long": "4.2.2"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wast-printer/-/wast-printer-1.11.1.tgz",
-            "version": "1.11.1"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wast-printer/-/wast-printer-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "@webpack-cli/configtest": {
             "dev": true,
-            "integrity": "sha512-njsdJXJSiS2iNbQVS0eT8A/KPnmyH4pv1APj2K0d1wrZcBLw+yppxOy4CGqa0OxDJkzfL/XELDhD8rocnIwB5A==",
+            "integrity": "sha512-K/vuv72vpfSEZoo5KIU0a2FsEoYdW0DUMtMpB5X3LlUwshetMZRZRxB7sCsVji/lFaSxtQQ3aM9O4eMolXkU9w==",
             "requires": {},
-            "resolved": "https://registry.npmjs.org/@webpack-cli/configtest/-/configtest-2.0.1.tgz",
-            "version": "2.0.1"
+            "resolved": "https://registry.npmjs.org/@webpack-cli/configtest/-/configtest-2.1.0.tgz",
+            "version": "2.1.0"
         },
         "@webpack-cli/info": {
             "dev": true,
             "integrity": "sha512-fE1UEWTwsAxRhrJNikE7v4EotYflkEhBL7EbajfkPlf6E37/2QshOy/D48Mw8G5XMFlQtS6YV42vtbG9zBpIQA==",
             "requires": {},
             "resolved": "https://registry.npmjs.org/@webpack-cli/info/-/info-2.0.1.tgz",
             "version": "2.0.1"
         },
         "@webpack-cli/serve": {
             "dev": true,
-            "integrity": "sha512-0G7tNyS+yW8TdgHwZKlDWYXFA6OJQnoLCQvYKkQP0Q2X205PSQ6RNUj0M+1OB/9gRQaUZ/ccYfaxd0nhaWKfjw==",
+            "integrity": "sha512-0xRgjgDLdz6G7+vvDLlaRpFatJaJ69uTalZLRSMX5B3VUrDmXcrVA3+6fXXQgmYz7bY9AAgs348XQdmtLsK41A==",
             "requires": {},
-            "resolved": "https://registry.npmjs.org/@webpack-cli/serve/-/serve-2.0.1.tgz",
-            "version": "2.0.1"
+            "resolved": "https://registry.npmjs.org/@webpack-cli/serve/-/serve-2.0.4.tgz",
+            "version": "2.0.4"
         },
         "@xtuc/ieee754": {
             "dev": true,
             "integrity": "sha512-DX8nKgqcGwsc0eJSqYt5lwP4DH5FlHnmuWWBRy7X0NcaGR0ZtuyeESgMwTYVEtxmsNGY+qit4QYT/MIYTOTPeA==",
             "resolved": "https://registry.npmjs.org/@xtuc/ieee754/-/ieee754-1.2.0.tgz",
             "version": "1.2.0"
         },
@@ -533,25 +547,25 @@
             "dev": true,
             "integrity": "sha512-Z7tMw1ytTXt5jqMcOP+OQteU1VuNK9Y02uuJtKQ1Sv69jXQKKg5cibLwGJow8yzZP+eAc18EmLGPal0bp36rvQ==",
             "resolved": "https://registry.npmjs.org/astral-regex/-/astral-regex-2.0.0.tgz",
             "version": "2.0.0"
         },
         "autoprefixer": {
             "dev": true,
-            "integrity": "sha512-49vKpMqcZYsJjwotvt4+h/BCjJVnhGwcLpDt5xkcaOG3eLrG/HUYLagrihYsQ+qrIBgIzX1Rw7a6L8I/ZA1Atg==",
+            "integrity": "sha512-FQzyfOsTlwVzjHxKEqRIAdJx9niO6VCBCoEwax/VLSoQF29ggECcPuBqUMZ+u8jCZOPSy8b8/8KnuFbp0SaFZQ==",
             "requires": {
-                "browserslist": "^4.21.4",
-                "caniuse-lite": "^1.0.30001426",
+                "browserslist": "^4.21.5",
+                "caniuse-lite": "^1.0.30001464",
                 "fraction.js": "^4.2.0",
                 "normalize-range": "^0.1.2",
                 "picocolors": "^1.0.0",
                 "postcss-value-parser": "^4.2.0"
             },
-            "resolved": "https://registry.npmjs.org/autoprefixer/-/autoprefixer-10.4.13.tgz",
-            "version": "10.4.13"
+            "resolved": "https://registry.npmjs.org/autoprefixer/-/autoprefixer-10.4.14.tgz",
+            "version": "10.4.14"
         },
         "balanced-match": {
             "dev": true,
             "integrity": "sha512-1ugUSr8BHXRnK23KfuYS+gVMC3LB8QGH9W1iGtDPsNWoQbgtXSExkBu2aDR4epiGWZOjZsj6lDl/N/AqqTC3UA==",
             "resolved": "https://registry.npmjs.org/balanced-match/-/balanced-match-2.0.0.tgz",
             "version": "2.0.0"
         },
@@ -571,23 +585,23 @@
                 "concat-map": "0.0.1"
             },
             "resolved": "https://registry.npmjs.org/brace-expansion/-/brace-expansion-1.1.11.tgz",
             "version": "1.1.11"
         },
         "browserslist": {
             "dev": true,
-            "integrity": "sha512-CBHJJdDmgjl3daYjN5Cp5kbTf1mUhZoS+beLklHIvkOWscs83YAhLlF3Wsh/lciQYAcbBJgTOD44VtG31ZM4Hw==",
+            "integrity": "sha512-tUkiguQGW7S3IhB7N+c2MV/HZPSCPAAiYBZXLsBhFB/PCy6ZKKsZrmBayHV9fdGV/ARIfJ14NkxKzRDjvp7L6w==",
             "requires": {
-                "caniuse-lite": "^1.0.30001400",
-                "electron-to-chromium": "^1.4.251",
-                "node-releases": "^2.0.6",
-                "update-browserslist-db": "^1.0.9"
+                "caniuse-lite": "^1.0.30001449",
+                "electron-to-chromium": "^1.4.284",
+                "node-releases": "^2.0.8",
+                "update-browserslist-db": "^1.0.10"
             },
-            "resolved": "https://registry.npmjs.org/browserslist/-/browserslist-4.21.4.tgz",
-            "version": "4.21.4"
+            "resolved": "https://registry.npmjs.org/browserslist/-/browserslist-4.21.5.tgz",
+            "version": "4.21.5"
         },
         "buffer-from": {
             "dev": true,
             "integrity": "sha512-E+XQCRwSbaaiChtv6k6Dwgc+bx+Bs6vuKJHHl5kox/BaKbhiXzqQOwK4cO22yElGp2OCmjwVhT3HmxgyPGnJfQ==",
             "resolved": "https://registry.npmjs.org/buffer-from/-/buffer-from-1.1.2.tgz",
             "version": "1.1.2"
         },
@@ -631,17 +645,17 @@
                 "quick-lru": "^4.0.1"
             },
             "resolved": "https://registry.npmjs.org/camelcase-keys/-/camelcase-keys-6.2.2.tgz",
             "version": "6.2.2"
         },
         "caniuse-lite": {
             "dev": true,
-            "integrity": "sha512-511ThLu1hF+5RRRt0zYCf2U2yRr9GPF6m5y90SBCWsvSoYoW7yAGlv/elyPaNfvGCkp6kj/KFZWU0BMA69Prsg==",
-            "resolved": "https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001429.tgz",
-            "version": "1.0.30001429"
+            "integrity": "sha512-ewDad7+D2vlyy+E4UJuVfiBsU69IL+8oVmTuZnH5Q6CIUbxNfI50uVpRHbUPDD6SUaN2o0Lh4DhTrvLG/Tn1yg==",
+            "resolved": "https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001473.tgz",
+            "version": "1.0.30001473"
         },
         "chalk": {
             "dev": true,
             "integrity": "sha512-Mti+f9lpJNcwF4tWV8/OrTTtF1gZi+f8FqlyAdouralcFWFQWF2+NgCHShjkCb+IFBLq9buZwE1xckQU4peSuQ==",
             "requires": {
                 "ansi-styles": "^3.2.1",
                 "escape-string-regexp": "^1.0.5",
@@ -709,36 +723,35 @@
             "dev": true,
             "integrity": "sha512-hUewv7oMjCp+wkBv5Rm0v87eJhq4woh5rSR+42YSQJKecCqgIqNkZ6lAlQms/BwHPJA5NKMRlpxPRv0n8HQW6g==",
             "resolved": "https://registry.npmjs.org/colorette/-/colorette-2.0.16.tgz",
             "version": "2.0.16"
         },
         "commander": {
             "dev": true,
-            "integrity": "sha512-KRs7WVDKg86PWiuAqhDrAQnTXZKraVcCc6vFdL14qrZ/DcWwuRo7VoiYXalXO7S5GKpqYiVEwCbgFDfxNHKJBQ==",
-            "resolved": "https://registry.npmjs.org/commander/-/commander-9.5.0.tgz",
-            "version": "9.5.0"
+            "integrity": "sha512-y4Mg2tXshplEbSGzx7amzPwKKOCGuoSRP/CjEdwwk0FOGlUbq6lKuoyDZTNZkmxHdJtp54hdfY/JUrdL7Xfdug==",
+            "resolved": "https://registry.npmjs.org/commander/-/commander-10.0.1.tgz",
+            "version": "10.0.1"
         },
         "concat-map": {
             "dev": true,
             "integrity": "sha1-2Klr13/Wjfd5OnMDajug1UBdR3s=",
             "resolved": "https://registry.npmjs.org/concat-map/-/concat-map-0.0.1.tgz",
             "version": "0.0.1"
         },
         "cosmiconfig": {
             "dev": true,
-            "integrity": "sha512-AdmX6xUzdNASswsFtmwSt7Vj8po9IuqXm0UXz7QKPuEUmPB4XyjGfaAr2PSuELMwkRMVH1EpIkX5bTZGRB3eCA==",
+            "integrity": "sha512-/UkO2JKI18b5jVMJUp0lvKFMpa/Gye+ZgZjKD+DGEN9y7NRcf/nK1A0sp67ONmKtnDCNMS44E6jrk0Yc3bDuUw==",
             "requires": {
-                "@types/parse-json": "^4.0.0",
                 "import-fresh": "^3.2.1",
+                "js-yaml": "^4.1.0",
                 "parse-json": "^5.0.0",
-                "path-type": "^4.0.0",
-                "yaml": "^1.10.0"
+                "path-type": "^4.0.0"
             },
-            "resolved": "https://registry.npmjs.org/cosmiconfig/-/cosmiconfig-7.1.0.tgz",
-            "version": "7.1.0"
+            "resolved": "https://registry.npmjs.org/cosmiconfig/-/cosmiconfig-8.1.3.tgz",
+            "version": "8.1.3"
         },
         "cross-spawn": {
             "dependencies": {
                 "which": {
                     "dev": true,
                     "integrity": "sha512-BLI3Tl1TW3Pvl70l3yq3Y64i+awpwXqsGBYWkkqMtnbXgrMD+yj7rhW0kuEDxzJaYXGjEW5ogapKNMEKNMjibA==",
                     "requires": {
@@ -776,14 +789,24 @@
                 "postcss-modules-values": "^4.0.0",
                 "postcss-value-parser": "^4.2.0",
                 "semver": "^7.3.8"
             },
             "resolved": "https://registry.npmjs.org/css-loader/-/css-loader-6.7.3.tgz",
             "version": "6.7.3"
         },
+        "css-tree": {
+            "dev": true,
+            "integrity": "sha512-6Fv1DV/TYw//QF5IzQdqsNDjx/wc8TrMBZsqjL9eW01tWb7R7k/mq+/VXfJCl7SoD5emsJop9cOByJZfs8hYIw==",
+            "requires": {
+                "mdn-data": "2.0.30",
+                "source-map-js": "^1.0.1"
+            },
+            "resolved": "https://registry.npmjs.org/css-tree/-/css-tree-2.3.1.tgz",
+            "version": "2.3.1"
+        },
         "cssesc": {
             "dev": true,
             "integrity": "sha512-/Tb/JcjK111nNScGob5MNtsntNM1aCNUDipB/TkwZFhyDrrE47SOx/18wF2bbjgc3ZzCSKW1T5nt5EbFoAz/Vg==",
             "resolved": "https://registry.npmjs.org/cssesc/-/cssesc-3.0.0.tgz",
             "version": "3.0.0"
         },
         "debug": {
@@ -851,33 +874,33 @@
                 "esutils": "^2.0.2"
             },
             "resolved": "https://registry.npmjs.org/doctrine/-/doctrine-3.0.0.tgz",
             "version": "3.0.0"
         },
         "electron-to-chromium": {
             "dev": true,
-            "integrity": "sha512-KNhIzgLiJmDDC444dj9vEOpZEgsV96ult9Iff98Vanumn+ShJHd5se8aX6KeVxdc0YQeqdrezBZv89rleDbvSg==",
-            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.270.tgz",
-            "version": "1.4.270"
+            "integrity": "sha512-gM7TdwuG3amns/1rlgxMbeeyNoBFPa+4Uu0c7FeROWh4qWmvSOnvcslKmWy51ggLKZ2n/F/4i2HJ+PVNxH9uCQ==",
+            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.348.tgz",
+            "version": "1.4.348"
         },
         "emoji-regex": {
             "dev": true,
             "integrity": "sha512-MSjYzcWNOA0ewAHpz0MxpYFvwg6yjy1NG3xteoqz644VCo/RPgnr1/GGt+ic3iJTzQ8Eu3TdM14SawnVUmGE6A==",
             "resolved": "https://registry.npmjs.org/emoji-regex/-/emoji-regex-8.0.0.tgz",
             "version": "8.0.0"
         },
         "enhanced-resolve": {
             "dev": true,
-            "integrity": "sha512-T0yTFjdpldGY8PmuXXR0PyQ1ufZpEGiHVrp7zHKB7jdR4qlmZHhONVM5AQOAWXuF/w3dnHbEQVrNptJgt7F+cQ==",
+            "integrity": "sha512-eyV8f0y1+bzyfh8xAwW/WTSZpLbjhqc4ne9eGSH4Zo2ejdyiNG9pU6mf9DG8a7+Auk6MFTlNOT4Y2y/9k8GKVg==",
             "requires": {
                 "graceful-fs": "^4.2.4",
                 "tapable": "^2.2.0"
             },
-            "resolved": "https://registry.npmjs.org/enhanced-resolve/-/enhanced-resolve-5.10.0.tgz",
-            "version": "5.10.0"
+            "resolved": "https://registry.npmjs.org/enhanced-resolve/-/enhanced-resolve-5.13.0.tgz",
+            "version": "5.13.0"
         },
         "envinfo": {
             "dev": true,
             "integrity": "sha512-/o+BXHmB7ocbHEAs6F2EnG0ogybVVUdkRunTT2glZU9XAaGmhqskrvKwqXuDfNjEO0LZKWdejEEpnq8aM0tOaw==",
             "resolved": "https://registry.npmjs.org/envinfo/-/envinfo-7.8.1.tgz",
             "version": "7.8.1"
         },
@@ -916,17 +939,17 @@
                 "unbox-primitive": "^1.0.1"
             },
             "resolved": "https://registry.npmjs.org/es-abstract/-/es-abstract-1.19.5.tgz",
             "version": "1.19.5"
         },
         "es-module-lexer": {
             "dev": true,
-            "integrity": "sha512-1HQ2M2sPtxwnvOvT1ZClHyQDiggdNjURWpY2we6aMKCQiUVxTmVs2UYPLIrD84sS+kMdUwfBSylbJPwNnBrnHQ==",
-            "resolved": "https://registry.npmjs.org/es-module-lexer/-/es-module-lexer-0.9.3.tgz",
-            "version": "0.9.3"
+            "integrity": "sha512-9978wrXM50Y4rTMmW5kXIC09ZdXQZqkE4mxhwkd8VbzsGkXGPgV4zWuqQJgCEzYngdo2dYDa0l8xhX4fkSwJSg==",
+            "resolved": "https://registry.npmjs.org/es-module-lexer/-/es-module-lexer-1.2.1.tgz",
+            "version": "1.2.1"
         },
         "es-shim-unscopables": {
             "dev": true,
             "integrity": "sha512-Jm6GPcCdC30eMLbZ2x8z2WuRwAws3zTBBKuusffYVUrNj/GVSUAZ+xKMaUpfNDR5IbyNA5LJbaecoUVbmUcB1w==",
             "requires": {
                 "has": "^1.0.3"
             },
@@ -1773,17 +1796,17 @@
                 "lru-cache": "^6.0.0"
             },
             "resolved": "https://registry.npmjs.org/hosted-git-info/-/hosted-git-info-4.1.0.tgz",
             "version": "4.1.0"
         },
         "html-tags": {
             "dev": true,
-            "integrity": "sha512-vy7ClnArOZwCnqZgvv+ddgHgJiAFXe3Ge9ML5/mBctVJoUoYPCdxVucOywjDARn6CVoh3dRSFdPHy2sX80L0Wg==",
-            "resolved": "https://registry.npmjs.org/html-tags/-/html-tags-3.2.0.tgz",
-            "version": "3.2.0"
+            "integrity": "sha512-ztqyC3kLto0e9WbNp0aeP+M3kTt+nbaIveGmUxAtZa+8iFgKLUOD4YKM5j+f3QD89bra7UeumolZHKuOXnTmeQ==",
+            "resolved": "https://registry.npmjs.org/html-tags/-/html-tags-3.3.1.tgz",
+            "version": "3.3.1"
         },
         "icss-utils": {
             "dev": true,
             "integrity": "sha512-soFhflCVWLfRNOPU3iv5Z9VUdT44xFRbzjLsEzSr5AQmgqPMTHdU3PMT1Cf1ssx8fLNJDA1juftYl+PUcv3MqA==",
             "requires": {},
             "resolved": "https://registry.npmjs.org/icss-utils/-/icss-utils-5.1.0.tgz",
             "version": "5.1.0"
@@ -2064,14 +2087,20 @@
                 "@types/node": "*",
                 "merge-stream": "^2.0.0",
                 "supports-color": "^8.0.0"
             },
             "resolved": "https://registry.npmjs.org/jest-worker/-/jest-worker-27.5.1.tgz",
             "version": "27.5.1"
         },
+        "jiti": {
+            "dev": true,
+            "integrity": "sha512-QAdOptna2NYiSSpv0O/BwoHBSmz4YhpzJHyi+fnMRTXFjp7B8i/YG5Z8IfusxB1ufjcD2Sre1F3R+nX3fvy7gg==",
+            "resolved": "https://registry.npmjs.org/jiti/-/jiti-1.18.2.tgz",
+            "version": "1.18.2"
+        },
         "js-tokens": {
             "dev": true,
             "integrity": "sha512-RdJUflcE3cUzKiMqQgsCu06FPu9UdIJO0beYbPhHN4k6apgJtifcoCtT9bcxOpYBtpD2kCM6Sbzg4CausW/PKQ==",
             "resolved": "https://registry.npmjs.org/js-tokens/-/js-tokens-4.0.0.tgz",
             "version": "4.0.0"
         },
         "js-yaml": {
@@ -2124,23 +2153,23 @@
                 "object.assign": "^4.1.2"
             },
             "resolved": "https://registry.npmjs.org/jsx-ast-utils/-/jsx-ast-utils-3.3.0.tgz",
             "version": "3.3.0"
         },
         "klona": {
             "dev": true,
-            "integrity": "sha512-pJiBpiXMbt7dkzXe8Ghj/u4FfXOOa98fPW+bihOJ4SjnoijweJrNThJfd3ifXpXhREjpoF2mZVH1GfS9LV3kHQ==",
-            "resolved": "https://registry.npmjs.org/klona/-/klona-2.0.5.tgz",
-            "version": "2.0.5"
+            "integrity": "sha512-dhG34DXATL5hSxJbIexCft8FChFXtmskoZYnoPWjXQuebWYCNkVeV3KkGegCK9CP1oswI/vQibS2GY7Em/sJJA==",
+            "resolved": "https://registry.npmjs.org/klona/-/klona-2.0.6.tgz",
+            "version": "2.0.6"
         },
         "known-css-properties": {
             "dev": true,
-            "integrity": "sha512-5FZRzrZzNTBruuurWpvZnvP9pum+fe0HcK8z/ooo+U+Hmp4vtbyp1/QDsqmufirXy4egGzbaH/y2uCZf+6W5Kg==",
-            "resolved": "https://registry.npmjs.org/known-css-properties/-/known-css-properties-0.26.0.tgz",
-            "version": "0.26.0"
+            "integrity": "sha512-uMCj6+hZYDoffuvAJjFAPz56E9uoowFHmTkqRtRq5WyC5Q6Cu/fTZKNQpX/RbzChBYLLl3lo8CjFZBAZXq9qFg==",
+            "resolved": "https://registry.npmjs.org/known-css-properties/-/known-css-properties-0.27.0.tgz",
+            "version": "0.27.0"
         },
         "levn": {
             "dev": true,
             "integrity": "sha512-+bT2uH4E5LGE7h/n3evcS/sQlJXCpIp6ym8OWJ5eV6+67Dsql/LaaT7qJBAt2rzfoa/5QBGBhxDix1dMt2kQKQ==",
             "requires": {
                 "prelude-ls": "^1.2.1",
                 "type-check": "~0.4.0"
@@ -2196,20 +2225,14 @@
             "integrity": "sha512-t7hw9pI+WvuwNJXwk5zVHpyhIqzg2qTlklJOf0mVxGSbe3Fp2VieZcduNYjaLDoy6p9uGpQEGWG87WpMKlNq8g==",
             "requires": {
                 "p-locate": "^4.1.0"
             },
             "resolved": "https://registry.npmjs.org/locate-path/-/locate-path-5.0.0.tgz",
             "version": "5.0.0"
         },
-        "lodash": {
-            "dev": true,
-            "integrity": "sha512-v2kDEe57lecTulaDIuNTPy3Ry4gLGJ6Z1O3vE1krgXZNrsQ+LFTGHVxVjcXPs17LhbZVGedAJv8XZ1tvj5FvSg==",
-            "resolved": "https://registry.npmjs.org/lodash/-/lodash-4.17.21.tgz",
-            "version": "4.17.21"
-        },
         "lodash.merge": {
             "dev": true,
             "integrity": "sha512-0KpjqXRVvrYyCsX1swR/XTK0va6VQkQM6MNo7PqW77ByjAhoARA8EfrP1N4+KlKj8YS0ZUCtRT/YUuhyYDujIQ==",
             "resolved": "https://registry.npmjs.org/lodash.merge/-/lodash.merge-4.6.2.tgz",
             "version": "4.6.2"
         },
         "lodash.truncate": {
@@ -2244,14 +2267,20 @@
         },
         "mathml-tag-names": {
             "dev": true,
             "integrity": "sha512-APMBEanjybaPzUrfqU0IMU5I0AswKMH7k8OTLs0vvV4KZpExkTkY87nR/zpbuTPj+gARop7aGUbl11pnDfW6xg==",
             "resolved": "https://registry.npmjs.org/mathml-tag-names/-/mathml-tag-names-2.1.3.tgz",
             "version": "2.1.3"
         },
+        "mdn-data": {
+            "dev": true,
+            "integrity": "sha512-GaqWWShW4kv/G9IEucWScBx9G1/vsFZZJUO+tD26M8J8z3Kw5RDQjaoZe03YAClgeS/SWPOcb4nkFBTEi5DUEA==",
+            "resolved": "https://registry.npmjs.org/mdn-data/-/mdn-data-2.0.30.tgz",
+            "version": "2.0.30"
+        },
         "meow": {
             "dev": true,
             "integrity": "sha512-+obSblOQmRhcyBt62furQqRAQpNyWXo8BuQ5bN7dG8wmwQ+vwHKp/rCFD4CrTP8CsDQD1sjoZ94K417XEUk8IQ==",
             "requires": {
                 "@types/minimist": "^1.2.0",
                 "camelcase-keys": "^6.2.2",
                 "decamelize": "^1.2.0",
@@ -2313,20 +2342,20 @@
                         "ajv-keywords": "^5.0.0"
                     },
                     "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-4.0.0.tgz",
                     "version": "4.0.0"
                 }
             },
             "dev": true,
-            "integrity": "sha512-EdlUizq13o0Pd+uCp+WO/JpkLvHRVGt97RqfeGhXqAcorYo1ypJSpkV+WDT0vY/kmh/p7wRdJNJtuyK540PXDw==",
+            "integrity": "sha512-9HaR++0mlgom81s95vvNjxkg52n2b5s//3ZTI1EtzFb98awsLSivs2LMsVqnQ3ay0PVhqWcGNyDaTE961FOcjQ==",
             "requires": {
                 "schema-utils": "^4.0.0"
             },
-            "resolved": "https://registry.npmjs.org/mini-css-extract-plugin/-/mini-css-extract-plugin-2.7.2.tgz",
-            "version": "2.7.2"
+            "resolved": "https://registry.npmjs.org/mini-css-extract-plugin/-/mini-css-extract-plugin-2.7.5.tgz",
+            "version": "2.7.5"
         },
         "minimatch": {
             "dev": true,
             "integrity": "sha512-J7p63hRiAjw1NDEww1W7i37+ByIrOWO5XQQAzZ3VOcL0PNybwpfmV/N05zFAzwQ9USyEcX6t3UO+K5aqBQOIHw==",
             "requires": {
                 "brace-expansion": "^1.1.7"
             },
@@ -2362,17 +2391,17 @@
             "dev": true,
             "integrity": "sha512-sGkPx+VjMtmA6MX27oA4FBFELFCZZ4S4XqeGOXCv68tT+jb3vk/RyaKWP0PTKyWtmLSM0b+adUTEvbs1PEaH2w==",
             "resolved": "https://registry.npmjs.org/ms/-/ms-2.1.2.tgz",
             "version": "2.1.2"
         },
         "nanoid": {
             "dev": true,
-            "integrity": "sha512-MqBkQh/OHTS2egovRtLk45wEyNXwF+cokD+1YPf9u5VfJiRdAiRwB2froX5Co9Rh20xs4siNPm8naNotSD6RBw==",
-            "resolved": "https://registry.npmjs.org/nanoid/-/nanoid-3.3.4.tgz",
-            "version": "3.3.4"
+            "integrity": "sha512-BGcqMMJuToF7i1rt+2PWSNVnWIkGCU78jBG3RxO/bZlnZPK2Cmi2QaffxGO/2RvWi9sL+FAiRiXMgsyxQ1DIDA==",
+            "resolved": "https://registry.npmjs.org/nanoid/-/nanoid-3.3.6.tgz",
+            "version": "3.3.6"
         },
         "natural-compare": {
             "dev": true,
             "integrity": "sha1-Sr6/7tdUHywnrPspvbvRXI1bpPc=",
             "resolved": "https://registry.npmjs.org/natural-compare/-/natural-compare-1.4.0.tgz",
             "version": "1.4.0"
         },
@@ -2380,17 +2409,17 @@
             "dev": true,
             "integrity": "sha512-Yd3UES5mWCSqR+qNT93S3UoYUkqAZ9lLg8a7g9rimsWmYGK8cVToA4/sF3RrshdyV3sAGMXVUmpMYOw+dLpOuw==",
             "resolved": "https://registry.npmjs.org/neo-async/-/neo-async-2.6.2.tgz",
             "version": "2.6.2"
         },
         "node-releases": {
             "dev": true,
-            "integrity": "sha512-PiVXnNuFm5+iYkLBNeq5211hvO38y63T0i2KKh2KnUs3RpzJ+JtODFjkD8yjLwnDkTYF1eKXheUwdssR+NRZdg==",
-            "resolved": "https://registry.npmjs.org/node-releases/-/node-releases-2.0.6.tgz",
-            "version": "2.0.6"
+            "integrity": "sha512-5GFldHPXVG/YZmFzJvKK2zDSzPKhEp0+ZR5SVaoSag9fsL5YgHbUHDfnG5494ISANDcK4KwPXAx2xqVEydmd7w==",
+            "resolved": "https://registry.npmjs.org/node-releases/-/node-releases-2.0.10.tgz",
+            "version": "2.0.10"
         },
         "normalize-package-data": {
             "dev": true,
             "integrity": "sha512-p2W1sgqij3zMMyRC067Dg16bfzVH+w7hyegmpIvZ4JNjqtGOVAIvLmjBx3yP7YTe9vKJgkoNOPjwQGogDoMXFA==",
             "requires": {
                 "hosted-git-info": "^4.0.1",
                 "is-core-module": "^2.5.0",
@@ -2654,33 +2683,34 @@
                 "find-up": "^4.0.0"
             },
             "resolved": "https://registry.npmjs.org/pkg-dir/-/pkg-dir-4.2.0.tgz",
             "version": "4.2.0"
         },
         "postcss": {
             "dev": true,
-            "integrity": "sha512-tP7u/Sn/dVxK2NnruI4H9BG+x+Wxz6oeZ1cJ8P6G/PZY0IKk4k/63TDsQf2kQq3+qoJeLm2kIBUNlZe3zgb4Zg==",
+            "integrity": "sha512-bQ3qMcpF6A/YjR55xtoTr0jGOlnPOKAIMdOWiv0EIT6HVPEaJiJB4NLljSbiHoC2RX7DN5Uvjtpbg1NPdwv1oA==",
             "requires": {
-                "nanoid": "^3.3.4",
+                "nanoid": "^3.3.6",
                 "picocolors": "^1.0.0",
                 "source-map-js": "^1.0.2"
             },
-            "resolved": "https://registry.npmjs.org/postcss/-/postcss-8.4.21.tgz",
-            "version": "8.4.21"
+            "resolved": "https://registry.npmjs.org/postcss/-/postcss-8.4.23.tgz",
+            "version": "8.4.23"
         },
         "postcss-loader": {
             "dev": true,
-            "integrity": "sha512-fUJzV/QH7NXUAqV8dWJ9Lg4aTkDCezpTS5HgJ2DvqznexTbSTxgi/dTECvTZ15BwKTtk8G/bqI/QTu2HPd3ZCg==",
+            "integrity": "sha512-qLAFjvR2BFNz1H930P7mj1iuWJFjGey/nVhimfOAAQ1ZyPpcClAxP8+A55Sl8mBvM+K2a9Pjgdj10KpANWrNfw==",
             "requires": {
-                "cosmiconfig": "^7.0.0",
-                "klona": "^2.0.5",
+                "cosmiconfig": "^8.1.3",
+                "jiti": "^1.18.2",
+                "klona": "^2.0.6",
                 "semver": "^7.3.8"
             },
-            "resolved": "https://registry.npmjs.org/postcss-loader/-/postcss-loader-7.0.2.tgz",
-            "version": "7.0.2"
+            "resolved": "https://registry.npmjs.org/postcss-loader/-/postcss-loader-7.3.0.tgz",
+            "version": "7.3.0"
         },
         "postcss-media-query-parser": {
             "dev": true,
             "integrity": "sha1-J7Ocb02U+Bsac7j3Y1HGCeXO8kQ=",
             "resolved": "https://registry.npmjs.org/postcss-media-query-parser/-/postcss-media-query-parser-0.2.3.tgz",
             "version": "0.2.3"
         },
@@ -2731,18 +2761,18 @@
             "integrity": "sha512-FARHN8pwH+WiS2OPCxJI8FuRJpTVnn6ZNFiqAM2aeW2LwTHWWmWgIyKC6cUo0L8aeKiF/14MNvnpls6R2PBeMQ==",
             "requires": {},
             "resolved": "https://registry.npmjs.org/postcss-safe-parser/-/postcss-safe-parser-6.0.0.tgz",
             "version": "6.0.0"
         },
         "postcss-scss": {
             "dev": true,
-            "integrity": "sha512-F7xpB6TrXyqUh3GKdyB4Gkp3QL3DDW1+uI+gxx/oJnUt/qXI4trj5OGlp9rOKdoABGULuqtqeG+3HEVQk4DjmA==",
+            "integrity": "sha512-rLDPhJY4z/i4nVFZ27j9GqLxj1pwxE80eAzUNRMXtcpipFYIeowerzBgG3yJhMtObGEXidtIgbUpQ3eLDsf5OQ==",
             "requires": {},
-            "resolved": "https://registry.npmjs.org/postcss-scss/-/postcss-scss-4.0.5.tgz",
-            "version": "4.0.5"
+            "resolved": "https://registry.npmjs.org/postcss-scss/-/postcss-scss-4.0.6.tgz",
+            "version": "4.0.6"
         },
         "postcss-selector-parser": {
             "dev": true,
             "integrity": "sha512-zbARubNdogI9j7WY4nQJBiNqQf3sLS3wCP4WfOidu+p28LofJqDH1tcXypGrcmMHhDk2t9wGhCsYe/+szLTy1g==",
             "requires": {
                 "cssesc": "^3.0.0",
                 "util-deprecate": "^1.0.2"
@@ -2959,17 +2989,17 @@
                 "queue-microtask": "^1.2.2"
             },
             "resolved": "https://registry.npmjs.org/run-parallel/-/run-parallel-1.2.0.tgz",
             "version": "1.2.0"
         },
         "safe-buffer": {
             "dev": true,
-            "integrity": "sha512-Gd2UZBJDkXlY7GbJxfsE8/nvKkUEU1G38c1siN6QP6a9PT9MmHB8GnpscSmMJSoF8LOIrt8ud/wPtojys4G6+g==",
-            "resolved": "https://registry.npmjs.org/safe-buffer/-/safe-buffer-5.1.2.tgz",
-            "version": "5.1.2"
+            "integrity": "sha512-rp3So07KcdmmKbGvgaNxQSJr7bGVSVk5S9Eq1F+ppbRo70+YeaDxkw5Dd8NPN+GD6bjnYm2VuPuCXmpuYvmCXQ==",
+            "resolved": "https://registry.npmjs.org/safe-buffer/-/safe-buffer-5.2.1.tgz",
+            "version": "5.2.1"
         },
         "sass": {
             "dependencies": {
                 "anymatch": {
                     "dev": true,
                     "integrity": "sha512-P43ePfOAIupkguHUycrc4qJ9kz8ZiuOUijaETwX7THt0Y/GNK7v0aa8rY816xWjZ7rJdA5XdMcpVFTKMq+RvWg==",
                     "requires": {
@@ -3057,32 +3087,32 @@
                         "is-number": "^7.0.0"
                     },
                     "resolved": "https://registry.npmjs.org/to-regex-range/-/to-regex-range-5.0.1.tgz",
                     "version": "5.0.1"
                 }
             },
             "dev": true,
-            "integrity": "sha512-Q7RaEtYf6BflYrQ+buPudKR26/lH+10EmO9bBqbmPh/KeLqv8bjpTNqxe71ocONqXq+jYiCbpPUmQMS+JJPk4A==",
+            "integrity": "sha512-NHpxIzN29MXvWiuswfc1W3I0N8SXBd8UR26WntmDlRYf0bSADnwnOjsyMZ3lMezSlArD33Vs3YFhp7dWvL770A==",
             "requires": {
                 "chokidar": ">=3.0.0 <4.0.0",
                 "immutable": "^4.0.0",
                 "source-map-js": ">=0.6.2 <2.0.0"
             },
-            "resolved": "https://registry.npmjs.org/sass/-/sass-1.58.3.tgz",
-            "version": "1.58.3"
+            "resolved": "https://registry.npmjs.org/sass/-/sass-1.62.1.tgz",
+            "version": "1.62.1"
         },
         "sass-loader": {
             "dev": true,
-            "integrity": "sha512-JWEp48djQA4nbZxmgC02/Wh0eroSUutulROUusYJO9P9zltRbNN80JCBHqRGzjd4cmZCa/r88xgfkjGD0TXsHg==",
+            "integrity": "sha512-nrIdVAAte3B9icfBiGWvmMhT/D+eCDwnk+yA7VE/76dp/WkHX+i44Q/pfo71NYbwj0Ap+PGsn0ekOuU1WFJ2AA==",
             "requires": {
-                "klona": "^2.0.4",
+                "klona": "^2.0.6",
                 "neo-async": "^2.6.2"
             },
-            "resolved": "https://registry.npmjs.org/sass-loader/-/sass-loader-13.2.0.tgz",
-            "version": "13.2.0"
+            "resolved": "https://registry.npmjs.org/sass-loader/-/sass-loader-13.2.2.tgz",
+            "version": "13.2.2"
         },
         "schema-utils": {
             "dependencies": {
                 "ajv": {
                     "dev": true,
                     "integrity": "sha512-j3fVLgvTo527anyYyJOGTYJbG+vnnQYvE0m5mmkc1TK+nxAppkCLMIL0aZ4dblVCNoGShhm+kzE4ZUykBoMg4g==",
                     "requires": {
@@ -3105,40 +3135,40 @@
                     "dev": true,
                     "integrity": "sha512-xbbCH5dCYU5T8LcEhhuh7HJ88HXuW3qsI3Y0zOZFKfZEHcpWiHU/Jxzk629Brsab/mMiHQti9wMP+845RPe3Vg==",
                     "resolved": "https://registry.npmjs.org/json-schema-traverse/-/json-schema-traverse-0.4.1.tgz",
                     "version": "0.4.1"
                 }
             },
             "dev": true,
-            "integrity": "sha512-Y5PQxS4ITlC+EahLuXaY86TXfR7Dc5lw294alXOq86JAHCihAIZfqv8nNCWvaEJvaC51uN9hbLGeV0cFBdH+Fw==",
+            "integrity": "sha512-pvjEHOgWc9OWA/f/DE3ohBWTD6EleVLf7iFUkoSwAxttdBhB9QUebQgxER2kWueOvRJXPHNnyrvvh9eZINB8Eg==",
             "requires": {
                 "@types/json-schema": "^7.0.8",
                 "ajv": "^6.12.5",
                 "ajv-keywords": "^3.5.2"
             },
-            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-3.1.1.tgz",
-            "version": "3.1.1"
+            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-3.1.2.tgz",
+            "version": "3.1.2"
         },
         "semver": {
             "dev": true,
             "integrity": "sha512-NB1ctGL5rlHrPJtFDVIVzTyQylMLu9N9VICA6HSFJo8MCGVTMW6gfpicwKmmK/dAjTOrqu5l63JJOpDSrAis3A==",
             "requires": {
                 "lru-cache": "^6.0.0"
             },
             "resolved": "https://registry.npmjs.org/semver/-/semver-7.3.8.tgz",
             "version": "7.3.8"
         },
         "serialize-javascript": {
             "dev": true,
-            "integrity": "sha512-Qr3TosvguFt8ePWqsvRfrKyQXIiW+nGbYpy8XK24NQHE83caxWt+mIymTT19DGFbNWNLfEwsrkSmN64lVWB9ag==",
+            "integrity": "sha512-owoXEFjWRllis8/M1Q+Cw5k8ZH40e3zhp/ovX+Xr/vi1qj6QesbyXXViFbpNvWvPNAD62SutwEXavefrLJWj7w==",
             "requires": {
                 "randombytes": "^2.1.0"
             },
-            "resolved": "https://registry.npmjs.org/serialize-javascript/-/serialize-javascript-6.0.0.tgz",
-            "version": "6.0.0"
+            "resolved": "https://registry.npmjs.org/serialize-javascript/-/serialize-javascript-6.0.1.tgz",
+            "version": "6.0.1"
         },
         "shallow-clone": {
             "dependencies": {
                 "kind-of": {
                     "dev": true,
                     "integrity": "sha512-dcS1ul+9tmeD95T+x28/ehLgd9mENa3LsvDTtzm3vyBEO7RPptvAD+t44WVXaUjTBRcrpFeFlC8WCruUR456hw==",
                     "resolved": "https://registry.npmjs.org/kind-of/-/kind-of-6.0.3.tgz",
@@ -3224,29 +3254,27 @@
                 "ansi-styles": "^4.0.0",
                 "astral-regex": "^2.0.0",
                 "is-fullwidth-code-point": "^3.0.0"
             },
             "resolved": "https://registry.npmjs.org/slice-ansi/-/slice-ansi-4.0.0.tgz",
             "version": "4.0.0"
         },
+        "source-map": {
+            "dev": true,
+            "integrity": "sha512-UjgapumWlbMhkBgzT7Ykc5YXUT46F0iKu8SGXq0bcwP5dz/h0Plj6enJqjz1Zbq2l5WaqYnrVbwWOWMyF3F47g==",
+            "resolved": "https://registry.npmjs.org/source-map/-/source-map-0.6.1.tgz",
+            "version": "0.6.1"
+        },
         "source-map-js": {
             "dev": true,
             "integrity": "sha512-R0XvVJ9WusLiqTCEiGCmICCMplcCkIwwR11mOSD9CR5u+IXYdiseeEuXCVAjS54zqwkLcPNnmU4OeJ6tUrWhDw==",
             "resolved": "https://registry.npmjs.org/source-map-js/-/source-map-js-1.0.2.tgz",
             "version": "1.0.2"
         },
         "source-map-support": {
-            "dependencies": {
-                "source-map": {
-                    "dev": true,
-                    "integrity": "sha512-UjgapumWlbMhkBgzT7Ykc5YXUT46F0iKu8SGXq0bcwP5dz/h0Plj6enJqjz1Zbq2l5WaqYnrVbwWOWMyF3F47g==",
-                    "resolved": "https://registry.npmjs.org/source-map/-/source-map-0.6.1.tgz",
-                    "version": "0.6.1"
-                }
-            },
             "dev": true,
             "integrity": "sha512-uBHU3L3czsIyYXKX88fdrGovxdSCoTGDRZ6SYXtSRxLZUzHg5P/66Ht6uoUlHu9EZod+inXhKo3qQgwXUT/y1w==",
             "requires": {
                 "buffer-from": "^1.0.0",
                 "source-map": "^0.6.0"
             },
             "resolved": "https://registry.npmjs.org/source-map-support/-/source-map-support-0.5.21.tgz",
@@ -3464,107 +3492,124 @@
                         "is-number": "^7.0.0"
                     },
                     "resolved": "https://registry.npmjs.org/to-regex-range/-/to-regex-range-5.0.1.tgz",
                     "version": "5.0.1"
                 }
             },
             "dev": true,
-            "integrity": "sha512-ErlzR/T3hhbV+a925/gbfc3f3Fep9/bnspMiJPorfGEmcBbXdS+oo6LrVtoUZ/w9fqD6o6k7PtUlCOsCRdjX/A==",
+            "integrity": "sha512-Cqzpc8tvJm77KaM8qUbhpJ/UYK55Ia0whQXj4b9IId9dlPICO7J8Lyo15SZWiHxKjlvy3p5FQor/3n6i8ignXg==",
             "requires": {
-                "@csstools/selector-specificity": "^2.0.2",
+                "@csstools/css-parser-algorithms": "^2.1.1",
+                "@csstools/css-tokenizer": "^2.1.1",
+                "@csstools/media-query-list-parser": "^2.0.4",
+                "@csstools/selector-specificity": "^2.2.0",
                 "balanced-match": "^2.0.0",
                 "colord": "^2.9.3",
-                "cosmiconfig": "^7.1.0",
+                "cosmiconfig": "^8.1.3",
                 "css-functions-list": "^3.1.0",
+                "css-tree": "^2.3.1",
                 "debug": "^4.3.4",
                 "fast-glob": "^3.2.12",
                 "fastest-levenshtein": "^1.0.16",
                 "file-entry-cache": "^6.0.1",
                 "global-modules": "^2.0.0",
                 "globby": "^11.1.0",
                 "globjoin": "^0.1.4",
-                "html-tags": "^3.2.0",
-                "ignore": "^5.2.1",
+                "html-tags": "^3.3.1",
+                "ignore": "^5.2.4",
                 "import-lazy": "^4.0.0",
                 "imurmurhash": "^0.1.4",
                 "is-plain-object": "^5.0.0",
-                "known-css-properties": "^0.26.0",
+                "known-css-properties": "^0.27.0",
                 "mathml-tag-names": "^2.1.3",
                 "meow": "^9.0.0",
                 "micromatch": "^4.0.5",
                 "normalize-path": "^3.0.0",
                 "picocolors": "^1.0.0",
-                "postcss": "^8.4.19",
+                "postcss": "^8.4.22",
                 "postcss-media-query-parser": "^0.2.3",
                 "postcss-resolve-nested-selector": "^0.1.1",
                 "postcss-safe-parser": "^6.0.0",
                 "postcss-selector-parser": "^6.0.11",
                 "postcss-value-parser": "^4.2.0",
                 "resolve-from": "^5.0.0",
                 "string-width": "^4.2.3",
                 "strip-ansi": "^6.0.1",
                 "style-search": "^0.1.0",
-                "supports-hyperlinks": "^2.3.0",
+                "supports-hyperlinks": "^3.0.0",
                 "svg-tags": "^1.0.0",
                 "table": "^6.8.1",
                 "v8-compile-cache": "^2.3.0",
-                "write-file-atomic": "^4.0.2"
+                "write-file-atomic": "^5.0.0"
             },
-            "resolved": "https://registry.npmjs.org/stylelint/-/stylelint-14.16.1.tgz",
-            "version": "14.16.1"
+            "resolved": "https://registry.npmjs.org/stylelint/-/stylelint-15.6.0.tgz",
+            "version": "15.6.0"
         },
         "stylelint-config-recommended": {
             "dev": true,
-            "integrity": "sha512-9YQSrJq4NvvRuTbzDsWX3rrFOzOlYBmZP+o513BJN/yfEmGSr0AxdvrWs0P/ilSpVV/wisamAHu5XSk8Rcf4CQ==",
+            "integrity": "sha512-x6x8QNARrGO2sG6iURkzqL+Dp+4bJorPMMRNPScdvaUK8PsynriOcMW7AFDKqkWAS5wbue/u8fUT/4ynzcmqdQ==",
             "requires": {},
-            "resolved": "https://registry.npmjs.org/stylelint-config-recommended/-/stylelint-config-recommended-9.0.0.tgz",
-            "version": "9.0.0"
+            "resolved": "https://registry.npmjs.org/stylelint-config-recommended/-/stylelint-config-recommended-12.0.0.tgz",
+            "version": "12.0.0"
         },
         "stylelint-config-recommended-scss": {
+            "dependencies": {
+                "stylelint-scss": {
+                    "dev": true,
+                    "integrity": "sha512-TSUgIeS0H3jqDZnby1UO1Qv3poi1N8wUYIJY6D1tuUq2MN3lwp/rITVo0wD+1SWTmRm0tNmGO0b7nKInnqF6Hg==",
+                    "requires": {
+                        "postcss-media-query-parser": "^0.2.3",
+                        "postcss-resolve-nested-selector": "^0.1.1",
+                        "postcss-selector-parser": "^6.0.11",
+                        "postcss-value-parser": "^4.2.0"
+                    },
+                    "resolved": "https://registry.npmjs.org/stylelint-scss/-/stylelint-scss-4.7.0.tgz",
+                    "version": "4.7.0"
+                }
+            },
             "dev": true,
-            "integrity": "sha512-BxjxEzRaZoQb7Iinc3p92GS6zRdRAkIuEu2ZFLTxJK2e1AIcCb5B5MXY9KOXdGTnYFZ+KKx6R4Fv9zU6CtMYPQ==",
+            "integrity": "sha512-EDghTDU7aOv2LTsRZvcT1w8mcjUaMhuy+t38iV5I/0Qiu6ixdkRwhLEMul3K/fnB2v9Nwqvb3xpvJfPH+HduDw==",
             "requires": {
-                "postcss-scss": "^4.0.2",
-                "stylelint-config-recommended": "^9.0.0",
-                "stylelint-scss": "^4.0.0"
+                "postcss-scss": "^4.0.6",
+                "stylelint-config-recommended": "^12.0.0",
+                "stylelint-scss": "^4.6.0"
             },
-            "resolved": "https://registry.npmjs.org/stylelint-config-recommended-scss/-/stylelint-config-recommended-scss-8.0.0.tgz",
-            "version": "8.0.0"
+            "resolved": "https://registry.npmjs.org/stylelint-config-recommended-scss/-/stylelint-config-recommended-scss-11.0.0.tgz",
+            "version": "11.0.0"
         },
         "stylelint-config-standard": {
             "dev": true,
-            "integrity": "sha512-uy8tZLbfq6ZrXy4JKu3W+7lYLgRQBxYTUUB88vPgQ+ZzAxdrvcaSUW9hOMNLYBnwH+9Kkj19M2DHdZ4gKwI7tg==",
+            "integrity": "sha512-eyxnLWoXImUn77+ODIuW9qXBDNM+ALN68L3wT1lN2oNspZ7D9NVGlNHb2QCUn4xDug6VZLsh0tF8NyoYzkgTzg==",
             "requires": {
-                "stylelint-config-recommended": "^9.0.0"
+                "stylelint-config-recommended": "^12.0.0"
             },
-            "resolved": "https://registry.npmjs.org/stylelint-config-standard/-/stylelint-config-standard-29.0.0.tgz",
-            "version": "29.0.0"
+            "resolved": "https://registry.npmjs.org/stylelint-config-standard/-/stylelint-config-standard-33.0.0.tgz",
+            "version": "33.0.0"
         },
         "stylelint-config-standard-scss": {
             "dev": true,
-            "integrity": "sha512-iZ2B5kQT2G3rUzx+437cEpdcnFOQkwnwqXuY8Z0QUwIHQVE8mnYChGAquyKFUKZRZ0pRnrciARlPaR1RBtPb0Q==",
+            "integrity": "sha512-yPKpJsrZn4ybuQZx/DkEHuCjw7pJginErE/47dFhCnrvD48IJ4UYec8tSiCuJWMA3HRjbIa3nh5ZeSauDGuVAg==",
             "requires": {
-                "stylelint-config-recommended-scss": "^8.0.0",
-                "stylelint-config-standard": "^29.0.0"
+                "stylelint-config-recommended-scss": "^11.0.0",
+                "stylelint-config-standard": "^33.0.0"
             },
-            "resolved": "https://registry.npmjs.org/stylelint-config-standard-scss/-/stylelint-config-standard-scss-6.1.0.tgz",
-            "version": "6.1.0"
+            "resolved": "https://registry.npmjs.org/stylelint-config-standard-scss/-/stylelint-config-standard-scss-9.0.0.tgz",
+            "version": "9.0.0"
         },
         "stylelint-scss": {
             "dev": true,
-            "integrity": "sha512-Qy66a+/30aylFhPmUArHhVsHOun1qrO93LGT15uzLuLjWS7hKDfpFm34mYo1ndR4MCo8W4bEZM1+AlJRJORaaw==",
+            "integrity": "sha512-5Ee5kG3JIcP2jk2PMoFMiNmW/815V+wK5o37X5ke90ihWMpPXI9iyqeA6zEWipWSRXeQc0kqbd7hKqiR+wPKNA==",
             "requires": {
-                "lodash": "^4.17.21",
                 "postcss-media-query-parser": "^0.2.3",
                 "postcss-resolve-nested-selector": "^0.1.1",
-                "postcss-selector-parser": "^6.0.6",
-                "postcss-value-parser": "^4.1.0"
+                "postcss-selector-parser": "^6.0.11",
+                "postcss-value-parser": "^4.2.0"
             },
-            "resolved": "https://registry.npmjs.org/stylelint-scss/-/stylelint-scss-4.4.0.tgz",
-            "version": "4.4.0"
+            "resolved": "https://registry.npmjs.org/stylelint-scss/-/stylelint-scss-5.0.0.tgz",
+            "version": "5.0.0"
         },
         "supports-color": {
             "dev": true,
             "integrity": "sha512-QjVjwdXIt408MIiAqCX4oUKsgU2EqAGzs2Ppkm4aQYbjm+ZEWEcW4SfFNTr4uMNZma0ey4f5lgLrkB0aX0QMow==",
             "requires": {
                 "has-flag": "^3.0.0"
             },
@@ -3586,21 +3631,21 @@
                         "has-flag": "^4.0.0"
                     },
                     "resolved": "https://registry.npmjs.org/supports-color/-/supports-color-7.2.0.tgz",
                     "version": "7.2.0"
                 }
             },
             "dev": true,
-            "integrity": "sha512-RpsAZlpWcDwOPQA22aCH4J0t7L8JmAvsCxfOSEwm7cQs3LshN36QaTkwd70DnBOXDWGssw2eUoc8CaRWT0XunA==",
+            "integrity": "sha512-QBDPHyPQDRTy9ku4URNGY5Lah8PAaXs6tAAwp55sL5WCsSW7GIfdf6W5ixfziW+t7wh3GVvHyHHyQ1ESsoRvaA==",
             "requires": {
                 "has-flag": "^4.0.0",
                 "supports-color": "^7.0.0"
             },
-            "resolved": "https://registry.npmjs.org/supports-hyperlinks/-/supports-hyperlinks-2.3.0.tgz",
-            "version": "2.3.0"
+            "resolved": "https://registry.npmjs.org/supports-hyperlinks/-/supports-hyperlinks-3.0.0.tgz",
+            "version": "3.0.0"
         },
         "supports-preserve-symlinks-flag": {
             "dev": true,
             "integrity": "sha512-ot0WnXS9fgdkgIcePe6RHNk1WA8+muPa6cSjeR3V8K27q9BB1rTE3R1p7Hv0z1ZyAc8s6Vvv8DIyWf681MAt0w==",
             "resolved": "https://registry.npmjs.org/supports-preserve-symlinks-flag/-/supports-preserve-symlinks-flag-1.0.0.tgz",
             "version": "1.0.0"
         },
@@ -3635,44 +3680,36 @@
                     "dev": true,
                     "integrity": "sha512-GpVkmM8vF2vQUkj2LvZmD35JxeJOLCwJ9cUkugyk2nuhbv3+mJvpLYYt+0+USMxE+oj+ey/lJEnhZw75x/OMcQ==",
                     "resolved": "https://registry.npmjs.org/commander/-/commander-2.20.3.tgz",
                     "version": "2.20.3"
                 }
             },
             "dev": true,
-            "integrity": "sha512-oL0rGeM/WFQCUd0y2QrWxYnq7tfSuKBiqTjRPWrRgB46WD/kiwHwF8T23z78H6Q6kGCuuHcPB+KULHRdxvVGQA==",
+            "integrity": "sha512-hVl35zClmpisy6oaoKALOpS0rDYLxRFLHhRuDlEGTKey9qHjS1w9GMORjuwIMt70Wan4lwsLYyWDVnWgF+KUEw==",
             "requires": {
                 "@jridgewell/source-map": "^0.3.2",
                 "acorn": "^8.5.0",
                 "commander": "^2.20.0",
                 "source-map-support": "~0.5.20"
             },
-            "resolved": "https://registry.npmjs.org/terser/-/terser-5.14.2.tgz",
-            "version": "5.14.2"
+            "resolved": "https://registry.npmjs.org/terser/-/terser-5.17.1.tgz",
+            "version": "5.17.1"
         },
         "terser-webpack-plugin": {
-            "dependencies": {
-                "source-map": {
-                    "dev": true,
-                    "integrity": "sha512-UjgapumWlbMhkBgzT7Ykc5YXUT46F0iKu8SGXq0bcwP5dz/h0Plj6enJqjz1Zbq2l5WaqYnrVbwWOWMyF3F47g==",
-                    "resolved": "https://registry.npmjs.org/source-map/-/source-map-0.6.1.tgz",
-                    "version": "0.6.1"
-                }
-            },
             "dev": true,
-            "integrity": "sha512-GvlZdT6wPQKbDNW/GDQzZFg/j4vKU96yl2q6mcUkzKOgW4gwf1Z8cZToUCrz31XHlPWH8MVb1r2tFtdDtTGJ7g==",
+            "integrity": "sha512-AfKwIktyP7Cu50xNjXF/6Qb5lBNzYaWpU6YfoX3uZicTx0zTy0stDDCsvjDapKsSDvOeWo5MEq4TmdBy2cNoHw==",
             "requires": {
+                "@jridgewell/trace-mapping": "^0.3.17",
                 "jest-worker": "^27.4.5",
                 "schema-utils": "^3.1.1",
-                "serialize-javascript": "^6.0.0",
-                "source-map": "^0.6.1",
-                "terser": "^5.7.2"
+                "serialize-javascript": "^6.0.1",
+                "terser": "^5.16.5"
             },
-            "resolved": "https://registry.npmjs.org/terser-webpack-plugin/-/terser-webpack-plugin-5.3.1.tgz",
-            "version": "5.3.1"
+            "resolved": "https://registry.npmjs.org/terser-webpack-plugin/-/terser-webpack-plugin-5.3.7.tgz",
+            "version": "5.3.7"
         },
         "text-table": {
             "dev": true,
             "integrity": "sha1-f17oI66AUgfACvLfSoTsP8+lcLQ=",
             "resolved": "https://registry.npmjs.org/text-table/-/text-table-0.2.0.tgz",
             "version": "0.2.0"
         },
@@ -3719,21 +3756,21 @@
                 "which-boxed-primitive": "^1.0.2"
             },
             "resolved": "https://registry.npmjs.org/unbox-primitive/-/unbox-primitive-1.0.2.tgz",
             "version": "1.0.2"
         },
         "update-browserslist-db": {
             "dev": true,
-            "integrity": "sha512-/xsqn21EGVdXI3EXSum1Yckj3ZVZugqyOZQ/CxYPBD/R+ko9NSUScf8tFF4dOKY+2pvSSJA/S+5B8s4Zr4kyvg==",
+            "integrity": "sha512-OztqDenkfFkbSG+tRxBeAnCVPckDBcvibKd35yDONx6OU8N7sqgwc7rCbkJ/WcYtVRZ4ba68d6byhC21GFh7sQ==",
             "requires": {
                 "escalade": "^3.1.1",
                 "picocolors": "^1.0.0"
             },
-            "resolved": "https://registry.npmjs.org/update-browserslist-db/-/update-browserslist-db-1.0.9.tgz",
-            "version": "1.0.9"
+            "resolved": "https://registry.npmjs.org/update-browserslist-db/-/update-browserslist-db-1.0.10.tgz",
+            "version": "1.0.10"
         },
         "uri-js": {
             "dev": true,
             "integrity": "sha512-7rKUyy33Q1yc98pQ1DAmLtwX109F7TIfWlW1Ydo8Wl1ii1SeHieeh0HHfPeL2fMXK6z0s8ecKs9frCuLJvndBg==",
             "requires": {
                 "punycode": "^2.1.0"
             },
@@ -3770,64 +3807,64 @@
                 "graceful-fs": "^4.1.2"
             },
             "resolved": "https://registry.npmjs.org/watchpack/-/watchpack-2.4.0.tgz",
             "version": "2.4.0"
         },
         "webpack": {
             "dev": true,
-            "integrity": "sha512-l5sOdYBDunyf72HW8dF23rFtWq/7Zgvt/9ftMof71E/yUb1YLOBmTgA2K4vQthB3kotMrSj609txVE0dnr2fjA==",
+            "integrity": "sha512-AAjaJ9S4hYCVODKLQTgG5p5e11hiMawBwV2v8MYLE0C/6UAGLuAF4n1qa9GOwdxnicaP+5k6M5HrLmD4+gIB8Q==",
             "requires": {
                 "@types/eslint-scope": "^3.7.3",
-                "@types/estree": "^0.0.51",
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/wasm-edit": "1.11.1",
-                "@webassemblyjs/wasm-parser": "1.11.1",
+                "@types/estree": "^1.0.0",
+                "@webassemblyjs/ast": "^1.11.5",
+                "@webassemblyjs/wasm-edit": "^1.11.5",
+                "@webassemblyjs/wasm-parser": "^1.11.5",
                 "acorn": "^8.7.1",
                 "acorn-import-assertions": "^1.7.6",
                 "browserslist": "^4.14.5",
                 "chrome-trace-event": "^1.0.2",
-                "enhanced-resolve": "^5.10.0",
-                "es-module-lexer": "^0.9.0",
+                "enhanced-resolve": "^5.13.0",
+                "es-module-lexer": "^1.2.1",
                 "eslint-scope": "5.1.1",
                 "events": "^3.2.0",
                 "glob-to-regexp": "^0.4.1",
                 "graceful-fs": "^4.2.9",
                 "json-parse-even-better-errors": "^2.3.1",
                 "loader-runner": "^4.2.0",
                 "mime-types": "^2.1.27",
                 "neo-async": "^2.6.2",
-                "schema-utils": "^3.1.0",
+                "schema-utils": "^3.1.2",
                 "tapable": "^2.1.1",
-                "terser-webpack-plugin": "^5.1.3",
+                "terser-webpack-plugin": "^5.3.7",
                 "watchpack": "^2.4.0",
                 "webpack-sources": "^3.2.3"
             },
-            "resolved": "https://registry.npmjs.org/webpack/-/webpack-5.76.0.tgz",
-            "version": "5.76.0"
+            "resolved": "https://registry.npmjs.org/webpack/-/webpack-5.81.0.tgz",
+            "version": "5.81.0"
         },
         "webpack-cli": {
             "dev": true,
-            "integrity": "sha512-S3KVAyfwUqr0Mo/ur3NzIp6jnerNpo7GUO6so51mxLi1spqsA17YcMXy0WOIJtBSnj748lthxC6XLbNKh/ZC+A==",
+            "integrity": "sha512-OLJwVMoXnXYH2ncNGU8gxVpUtm3ybvdioiTvHgUyBuyMLKiVvWy+QObzBsMtp5pH7qQoEuWgeEUQ/sU3ZJFzAw==",
             "requires": {
                 "@discoveryjs/json-ext": "^0.5.0",
-                "@webpack-cli/configtest": "^2.0.1",
+                "@webpack-cli/configtest": "^2.1.0",
                 "@webpack-cli/info": "^2.0.1",
-                "@webpack-cli/serve": "^2.0.1",
+                "@webpack-cli/serve": "^2.0.4",
                 "colorette": "^2.0.14",
-                "commander": "^9.4.1",
+                "commander": "^10.0.1",
                 "cross-spawn": "^7.0.3",
                 "envinfo": "^7.7.3",
                 "fastest-levenshtein": "^1.0.12",
                 "import-local": "^3.0.2",
                 "interpret": "^3.1.1",
                 "rechoir": "^0.8.0",
                 "webpack-merge": "^5.7.3"
             },
-            "resolved": "https://registry.npmjs.org/webpack-cli/-/webpack-cli-5.0.1.tgz",
-            "version": "5.0.1"
+            "resolved": "https://registry.npmjs.org/webpack-cli/-/webpack-cli-5.1.1.tgz",
+            "version": "5.1.1"
         },
         "webpack-merge": {
             "dev": true,
             "integrity": "sha512-/SaI7xY0831XwP6kzuwhKWVKDP9t1QY1h65lAFLbZqMPIuYcD9QAW4u9STIbU9kaJbPBB/geU/gLr1wDjOhQ+Q==",
             "requires": {
                 "clone-deep": "^4.0.1",
                 "wildcard": "^2.0.0"
@@ -3879,65 +3916,59 @@
             "dev": true,
             "integrity": "sha1-tSQ9jz7BqjXxNkYFvA0QNuMKtp8=",
             "resolved": "https://registry.npmjs.org/wrappy/-/wrappy-1.0.2.tgz",
             "version": "1.0.2"
         },
         "write-file-atomic": {
             "dev": true,
-            "integrity": "sha512-7KxauUdBmSdWnmpaGFg+ppNjKF8uNLry8LyzjauQDOVONfFLNKrKvQOxZ/VuTIcS/gge/YNahf5RIIQWTSarlg==",
+            "integrity": "sha512-R7NYMnHSlV42K54lwY9lvW6MnSm1HSJqZL3xiSgi9E7//FYaI74r2G0rd+/X6VAMkHEdzxQaU5HUOXWUz5kA/w==",
             "requires": {
                 "imurmurhash": "^0.1.4",
                 "signal-exit": "^3.0.7"
             },
-            "resolved": "https://registry.npmjs.org/write-file-atomic/-/write-file-atomic-4.0.2.tgz",
-            "version": "4.0.2"
+            "resolved": "https://registry.npmjs.org/write-file-atomic/-/write-file-atomic-5.0.0.tgz",
+            "version": "5.0.0"
         },
         "xdg-basedir": {
             "dev": true,
             "integrity": "sha512-PSNhEJDejZYV7h50BohL09Er9VaIefr2LMAf3OEmpCkjOi34eYyQYAXUTjEQtZJTKcF0E2UKTh+osDLsgNim9Q==",
             "resolved": "https://registry.npmjs.org/xdg-basedir/-/xdg-basedir-4.0.0.tgz",
             "version": "4.0.0"
         },
         "yallist": {
             "dev": true,
             "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
             "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
             "version": "4.0.0"
         },
-        "yaml": {
-            "dev": true,
-            "integrity": "sha512-r3vXyErRCYJ7wg28yvBY5VSoAF8ZvlcW9/BwUzEtUsjvX/DKs24dIkuwjtuprwJJHsbyUbLApepYTR1BN4uHrg==",
-            "resolved": "https://registry.npmjs.org/yaml/-/yaml-1.10.2.tgz",
-            "version": "1.10.2"
-        },
         "yargs-parser": {
             "dev": true,
             "integrity": "sha512-y11nGElTIV+CT3Zv9t7VKl+Q3hTQoT9a1Qzezhhl6Rp21gJ/IVTW7Z3y9EWXhuUBC2Shnf+DX0antecpAwSP8w==",
             "resolved": "https://registry.npmjs.org/yargs-parser/-/yargs-parser-20.2.9.tgz",
             "version": "20.2.9"
         }
     },
     "lockfileVersion": 2,
     "name": "django-hijack",
     "packages": {
         "": {
             "devDependencies": {
-                "autoprefixer": "^10.4.13",
+                "autoprefixer": "^10.4.14",
                 "css-loader": "^6.7.3",
-                "mini-css-extract-plugin": "^2.7.2",
+                "mini-css-extract-plugin": "^2.7.5",
                 "postcss": "^8.4.21",
-                "postcss-loader": "^7.0.2",
-                "sass": "^1.58.3",
-                "sass-loader": "^13.2.0",
+                "postcss-loader": "^7.3.0",
+                "sass": "^1.62.1",
+                "sass-loader": "^13.2.2",
                 "standard": "^17.0.0",
-                "stylelint": "^14.16.1",
-                "stylelint-config-standard-scss": "^6.1.0",
-                "stylelint-scss": "^4.4.0",
-                "webpack": "^5.76.0",
-                "webpack-cli": "^5.0.1"
+                "stylelint": "^15.6.0",
+                "stylelint-config-standard-scss": "^9.0.0",
+                "stylelint-scss": "^5.0.0",
+                "webpack": "^5.81.0",
+                "webpack-cli": "^5.1.1"
             },
             "license": "MIT",
             "name": "django-hijack",
             "version": "1.0.0"
         },
         "node_modules/@babel/code-frame": {
             "dependencies": {
@@ -3970,30 +4001,75 @@
             "engines": {
                 "node": ">=6.9.0"
             },
             "integrity": "sha512-5FnTQLSLswEj6IkgVw5KusNUUFY9ZGqe/TRFnP/BKYHYgfh7tc+C7mwiy95/yNP7Dh9x580Vv8r7u7ZfTBFxdw==",
             "resolved": "https://registry.npmjs.org/@babel/highlight/-/highlight-7.16.10.tgz",
             "version": "7.16.10"
         },
+        "node_modules/@csstools/css-parser-algorithms": {
+            "dev": true,
+            "engines": {
+                "node": "^14 || ^16 || >=18"
+            },
+            "funding": {
+                "type": "opencollective",
+                "url": "https://opencollective.com/csstools"
+            },
+            "integrity": "sha512-viRnRh02AgO4mwIQb2xQNJju0i+Fh9roNgmbR5xEuG7J3TGgxjnE95HnBLgsFJOJOksvcfxOUCgODcft6Y07cA==",
+            "peerDependencies": {
+                "@csstools/css-tokenizer": "^2.1.1"
+            },
+            "resolved": "https://registry.npmjs.org/@csstools/css-parser-algorithms/-/css-parser-algorithms-2.1.1.tgz",
+            "version": "2.1.1"
+        },
+        "node_modules/@csstools/css-tokenizer": {
+            "dev": true,
+            "engines": {
+                "node": "^14 || ^16 || >=18"
+            },
+            "funding": {
+                "type": "opencollective",
+                "url": "https://opencollective.com/csstools"
+            },
+            "integrity": "sha512-GbrTj2Z8MCTUv+52GE0RbFGM527xuXZ0Xa5g0Z+YN573uveS4G0qi6WNOMyz3yrFM/jaILTTwJ0+umx81EzqfA==",
+            "resolved": "https://registry.npmjs.org/@csstools/css-tokenizer/-/css-tokenizer-2.1.1.tgz",
+            "version": "2.1.1"
+        },
+        "node_modules/@csstools/media-query-list-parser": {
+            "dev": true,
+            "engines": {
+                "node": "^14 || ^16 || >=18"
+            },
+            "funding": {
+                "type": "opencollective",
+                "url": "https://opencollective.com/csstools"
+            },
+            "integrity": "sha512-GyYot6jHgcSDZZ+tLSnrzkR7aJhF2ZW6d+CXH66mjy5WpAQhZD4HDke2OQ36SivGRWlZJpAz7TzbW6OKlEpxAA==",
+            "peerDependencies": {
+                "@csstools/css-parser-algorithms": "^2.1.1",
+                "@csstools/css-tokenizer": "^2.1.1"
+            },
+            "resolved": "https://registry.npmjs.org/@csstools/media-query-list-parser/-/media-query-list-parser-2.0.4.tgz",
+            "version": "2.0.4"
+        },
         "node_modules/@csstools/selector-specificity": {
             "dev": true,
             "engines": {
-                "node": "^12 || ^14 || >=16"
+                "node": "^14 || ^16 || >=18"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/csstools"
             },
-            "integrity": "sha512-IkpVW/ehM1hWKln4fCA3NzJU8KwD+kIOvPZA4cqxoJHtE21CCzjyp+Kxbu0i5I4tBNOlXPL9mjwnWlL0VEG4Fg==",
+            "integrity": "sha512-+OJ9konv95ClSTOJCmMZqpd5+YGsB2S+x6w3E1oaM8UuR5j8nTNHYSz8c9BEPGDOCMQYIEEGlVPj/VY64iTbGw==",
             "peerDependencies": {
-                "postcss": "^8.2",
                 "postcss-selector-parser": "^6.0.10"
             },
-            "resolved": "https://registry.npmjs.org/@csstools/selector-specificity/-/selector-specificity-2.0.2.tgz",
-            "version": "2.0.2"
+            "resolved": "https://registry.npmjs.org/@csstools/selector-specificity/-/selector-specificity-2.2.0.tgz",
+            "version": "2.2.0"
         },
         "node_modules/@discoveryjs/json-ext": {
             "dev": true,
             "engines": {
                 "node": ">=10.0.0"
             },
             "integrity": "sha512-dBVuXR082gk3jsFp7Rd/JI4kytwGHecnCoTtXFb7DB6CNHp4rg5k1bhg0nWdLGLnOV71lmDzGQaLMy8iPLY0pw==",
@@ -4068,17 +4144,17 @@
                 "@jridgewell/sourcemap-codec": "^1.4.10",
                 "@jridgewell/trace-mapping": "^0.3.9"
             },
             "dev": true,
             "engines": {
                 "node": ">=6.0.0"
             },
-            "integrity": "sha512-mh65xKQAzI6iBcFzwv28KVWSmCkdRBWoOh+bYQGW3+6OZvbbN3TqMGo5hqYxQniRcH9F2VZIoJCm4pa3BPDK/A==",
-            "resolved": "https://registry.npmjs.org/@jridgewell/gen-mapping/-/gen-mapping-0.3.2.tgz",
-            "version": "0.3.2"
+            "integrity": "sha512-HLhSWOLRi875zjjMG/r+Nv0oCW8umGb0BgEhyX3dDX3egwZtB8PqLnjz3yedt8R5StBrzcg4aBpnh8UA9D1BoQ==",
+            "resolved": "https://registry.npmjs.org/@jridgewell/gen-mapping/-/gen-mapping-0.3.3.tgz",
+            "version": "0.3.3"
         },
         "node_modules/@jridgewell/resolve-uri": {
             "dev": true,
             "engines": {
                 "node": ">=6.0.0"
             },
             "integrity": "sha512-F2msla3tad+Mfht5cJq7LSXcdudKTWCVYUgw6pLFOOHSTtZlj6SWNYAp+AhuqLmWdBO2X5hPrLcu8cVP8fy28w==",
@@ -4096,33 +4172,33 @@
         },
         "node_modules/@jridgewell/source-map": {
             "dependencies": {
                 "@jridgewell/gen-mapping": "^0.3.0",
                 "@jridgewell/trace-mapping": "^0.3.9"
             },
             "dev": true,
-            "integrity": "sha512-m7O9o2uR8k2ObDysZYzdfhb08VuEml5oWGiosa1VdaPZ/A6QyPkAJuwN0Q1lhULOf6B7MtQmHENS743hWtCrgw==",
-            "resolved": "https://registry.npmjs.org/@jridgewell/source-map/-/source-map-0.3.2.tgz",
-            "version": "0.3.2"
+            "integrity": "sha512-b+fsZXeLYi9fEULmfBrhxn4IrPlINf8fiNarzTof004v3lFdntdwa9PF7vFJqm3mg7s+ScJMxXaE3Acp1irZcg==",
+            "resolved": "https://registry.npmjs.org/@jridgewell/source-map/-/source-map-0.3.3.tgz",
+            "version": "0.3.3"
         },
         "node_modules/@jridgewell/sourcemap-codec": {
             "dev": true,
             "integrity": "sha512-XPSJHWmi394fuUuzDnGz1wiKqWfo1yXecHQMRf2l6hztTO+nPru658AyDngaBe7isIxEkRsPR3FZh+s7iVa4Uw==",
             "resolved": "https://registry.npmjs.org/@jridgewell/sourcemap-codec/-/sourcemap-codec-1.4.14.tgz",
             "version": "1.4.14"
         },
         "node_modules/@jridgewell/trace-mapping": {
             "dependencies": {
-                "@jridgewell/resolve-uri": "^3.0.3",
-                "@jridgewell/sourcemap-codec": "^1.4.10"
+                "@jridgewell/resolve-uri": "3.1.0",
+                "@jridgewell/sourcemap-codec": "1.4.14"
             },
             "dev": true,
-            "integrity": "sha512-bJWEfQ9lPTvm3SneWwRFVLzrh6nhjwqw7TUFFBEMzwvg7t7PCDenf2lDwqo4NQXzdpgBXyFgDWnQA+2vkruksQ==",
-            "resolved": "https://registry.npmjs.org/@jridgewell/trace-mapping/-/trace-mapping-0.3.14.tgz",
-            "version": "0.3.14"
+            "integrity": "sha512-w+niJYzMHdd7USdiH2U6869nqhD2nbfZXND5Yp93qIbEmnDNk7PD48o+YchRVpzMU7M6jVCbenTR7PA1FLQ9pA==",
+            "resolved": "https://registry.npmjs.org/@jridgewell/trace-mapping/-/trace-mapping-0.3.18.tgz",
+            "version": "0.3.18"
         },
         "node_modules/@nodelib/fs.scandir": {
             "dependencies": {
                 "@nodelib/fs.stat": "2.0.5",
                 "run-parallel": "^1.1.9"
             },
             "dev": true,
@@ -4173,17 +4249,17 @@
             "dev": true,
             "integrity": "sha512-PB3ldyrcnAicT35TWPs5IcwKD8S333HMaa2VVv4+wdvebJkjWuW/xESoB8IwRcog8HYVYamb1g/R31Qv5Bx03g==",
             "resolved": "https://registry.npmjs.org/@types/eslint-scope/-/eslint-scope-3.7.3.tgz",
             "version": "3.7.3"
         },
         "node_modules/@types/estree": {
             "dev": true,
-            "integrity": "sha512-CuPgU6f3eT/XgKKPqKd/gLZV1Xmvf1a2R5POBOGQa6uv82xpls89HU5zKeVoyR8XzHd1RGNOlQlvUe3CFkjWNQ==",
-            "resolved": "https://registry.npmjs.org/@types/estree/-/estree-0.0.51.tgz",
-            "version": "0.0.51"
+            "integrity": "sha512-LG4opVs2ANWZ1TJoKc937iMmNstM/d0ae1vNbnBvBhqCSezgVUOzcLCqbI5elV8Vy6WKwKjaqR+zO9VKirBBCA==",
+            "resolved": "https://registry.npmjs.org/@types/estree/-/estree-1.0.1.tgz",
+            "version": "1.0.1"
         },
         "node_modules/@types/json-schema": {
             "dev": true,
             "integrity": "sha512-wOuvG1SN4Us4rez+tylwwwCV1psiNVOkJeM3AUWUNWg/jDQY2+HE/444y5gc+jBmRqASOm2Oeh5c1axHobwRKQ==",
             "resolved": "https://registry.npmjs.org/@types/json-schema/-/json-schema-7.0.11.tgz",
             "version": "7.0.11"
         },
@@ -4197,188 +4273,182 @@
             "dev": true,
             "integrity": "sha512-jhuKLIRrhvCPLqwPcx6INqmKeiA5EWrsCOPhrlFSrbrmU4ZMPjj5Ul/oLCMDO98XRUIwVm78xICz4EPCektzeQ==",
             "resolved": "https://registry.npmjs.org/@types/minimist/-/minimist-1.2.2.tgz",
             "version": "1.2.2"
         },
         "node_modules/@types/node": {
             "dev": true,
-            "integrity": "sha512-UxDxWn7dl97rKVeVS61vErvw086aCYhDLyvRQZ5Rk65rZKepaFdm53GeqXaKBuOhED4e9uWq34IC3TdSdJJ2Gw==",
-            "resolved": "https://registry.npmjs.org/@types/node/-/node-17.0.23.tgz",
-            "version": "17.0.23"
+            "integrity": "sha512-OPs5WnnT1xkCBiuQrZA4+YAV4HEJejmHneyraIaxsbev5yCEr6KMwINNFP9wQeFIw8FWcoTqF3vQsa5CDaI+8Q==",
+            "resolved": "https://registry.npmjs.org/@types/node/-/node-18.16.3.tgz",
+            "version": "18.16.3"
         },
         "node_modules/@types/normalize-package-data": {
             "dev": true,
             "integrity": "sha512-Gj7cI7z+98M282Tqmp2K5EIsoouUEzbBJhQQzDE3jSIRk6r9gsz0oUokqIUR4u1R3dMHo0pDHM7sNOHyhulypw==",
             "resolved": "https://registry.npmjs.org/@types/normalize-package-data/-/normalize-package-data-2.4.1.tgz",
             "version": "2.4.1"
         },
-        "node_modules/@types/parse-json": {
-            "dev": true,
-            "integrity": "sha512-//oorEZjL6sbPcKUaCdIGlIUeH26mgzimjBB77G6XRgnDl/L5wOnpyBGRe/Mmf5CVW3PwEBE1NjiMZ/ssFh4wA==",
-            "resolved": "https://registry.npmjs.org/@types/parse-json/-/parse-json-4.0.0.tgz",
-            "version": "4.0.0"
-        },
         "node_modules/@webassemblyjs/ast": {
             "dependencies": {
-                "@webassemblyjs/helper-numbers": "1.11.1",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.1"
+                "@webassemblyjs/helper-numbers": "1.11.5",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.5"
             },
             "dev": true,
-            "integrity": "sha512-ukBh14qFLjxTQNTXocdyksN5QdM28S1CxHt2rdskFyL+xFV7VremuBLVbmCePj+URalXBENx/9Lm7lnhihtCSw==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/ast/-/ast-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-LHY/GSAZZRpsNQH+/oHqhRQ5FT7eoULcBqgfyTB5nQHogFnK3/7QoN7dLnwSE/JkUAF0SrRuclT7ODqMFtWxxQ==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/ast/-/ast-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/floating-point-hex-parser": {
             "dev": true,
-            "integrity": "sha512-iGRfyc5Bq+NnNuX8b5hwBrRjzf0ocrJPI6GWFodBFzmFnyvrQ83SHKhmilCU/8Jv67i4GJZBMhEzltxzcNagtQ==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/floating-point-hex-parser/-/floating-point-hex-parser-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-1j1zTIC5EZOtCplMBG/IEwLtUojtwFVwdyVMbL/hwWqbzlQoJsWCOavrdnLkemwNoC/EOwtUFch3fuo+cbcXYQ==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/floating-point-hex-parser/-/floating-point-hex-parser-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/helper-api-error": {
             "dev": true,
-            "integrity": "sha512-RlhS8CBCXfRUR/cwo2ho9bkheSXG0+NwooXcc3PAILALf2QLdFyj7KGsKRbVc95hZnhnERon4kW/D3SZpp6Tcg==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-api-error/-/helper-api-error-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-L65bDPmfpY0+yFrsgz8b6LhXmbbs38OnwDCf6NpnMUYqa+ENfE5Dq9E42ny0qz/PdR0LJyq/T5YijPnU8AXEpA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-api-error/-/helper-api-error-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/helper-buffer": {
             "dev": true,
-            "integrity": "sha512-gwikF65aDNeeXa8JxXa2BAk+REjSyhrNC9ZwdT0f8jc4dQQeDQ7G4m0f2QCLPJiMTTO6wfDmRmj/pW0PsUvIcA==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-buffer/-/helper-buffer-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-fDKo1gstwFFSfacIeH5KfwzjykIE6ldh1iH9Y/8YkAZrhmu4TctqYjSh7t0K2VyDSXOZJ1MLhht/k9IvYGcIxg==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-buffer/-/helper-buffer-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/helper-numbers": {
             "dependencies": {
-                "@webassemblyjs/floating-point-hex-parser": "1.11.1",
-                "@webassemblyjs/helper-api-error": "1.11.1",
+                "@webassemblyjs/floating-point-hex-parser": "1.11.5",
+                "@webassemblyjs/helper-api-error": "1.11.5",
                 "@xtuc/long": "4.2.2"
             },
             "dev": true,
-            "integrity": "sha512-vDkbxiB8zfnPdNK9Rajcey5C0w+QJugEglN0of+kmO8l7lDb77AnlKYQF7aarZuCrv+l0UvqL+68gSDr3k9LPQ==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-numbers/-/helper-numbers-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-DhykHXM0ZABqfIGYNv93A5KKDw/+ywBFnuWybZZWcuzWHfbp21wUfRkbtz7dMGwGgT4iXjWuhRMA2Mzod6W4WA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-numbers/-/helper-numbers-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/helper-wasm-bytecode": {
             "dev": true,
-            "integrity": "sha512-PvpoOGiJwXeTrSf/qfudJhwlvDQxFgelbMqtq52WWiXC6Xgg1IREdngmPN3bs4RoO83PnL/nFrxucXj1+BX62Q==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-bytecode/-/helper-wasm-bytecode-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-oC4Qa0bNcqnjAowFn7MPCETQgDYytpsfvz4ujZz63Zu/a/v71HeCAAmZsgZ3YVKec3zSPYytG3/PrRCqbtcAvA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-bytecode/-/helper-wasm-bytecode-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/helper-wasm-section": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/helper-buffer": "1.11.1",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.1",
-                "@webassemblyjs/wasm-gen": "1.11.1"
+                "@webassemblyjs/ast": "1.11.5",
+                "@webassemblyjs/helper-buffer": "1.11.5",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.5",
+                "@webassemblyjs/wasm-gen": "1.11.5"
             },
             "dev": true,
-            "integrity": "sha512-10P9No29rYX1j7F3EVPX3JvGPQPae+AomuSTPiF9eBQeChHI6iqjMIwR9JmOJXwpnn/oVGDk7I5IlskuMwU/pg==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-section/-/helper-wasm-section-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-uEoThA1LN2NA+K3B9wDo3yKlBfVtC6rh0i4/6hvbz071E8gTNZD/pT0MsBf7MeD6KbApMSkaAK0XeKyOZC7CIA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-section/-/helper-wasm-section-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/ieee754": {
             "dependencies": {
                 "@xtuc/ieee754": "^1.2.0"
             },
             "dev": true,
-            "integrity": "sha512-hJ87QIPtAMKbFq6CGTkZYJivEwZDbQUgYd3qKSadTNOhVY7p+gfP6Sr0lLRVTaG1JjFj+r3YchoqRYxNH3M0GQ==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/ieee754/-/ieee754-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-37aGq6qVL8A8oPbPrSGMBcp38YZFXcHfiROflJn9jxSdSMMM5dS5P/9e2/TpaJuhE+wFrbukN2WI6Hw9MH5acg==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/ieee754/-/ieee754-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/leb128": {
             "dependencies": {
                 "@xtuc/long": "4.2.2"
             },
             "dev": true,
-            "integrity": "sha512-BJ2P0hNZ0u+Th1YZXJpzW6miwqQUGcIHT1G/sf72gLVD9DZ5AdYTqPNbHZh6K1M5VmKvFXwGSWZADz+qBWxeRw==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/leb128/-/leb128-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-ajqrRSXaTJoPW+xmkfYN6l8VIeNnR4vBOTQO9HzR7IygoCcKWkICbKFbVTNMjMgMREqXEr0+2M6zukzM47ZUfQ==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/leb128/-/leb128-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/utf8": {
             "dev": true,
-            "integrity": "sha512-9kqcxAEdMhiwQkHpkNiorZzqpGrodQQ2IGrHHxCy+Ozng0ofyMA0lTqiLkVs1uzTRejX+/O0EOT7KxqVPuXosQ==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/utf8/-/utf8-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-WiOhulHKTZU5UPlRl53gHR8OxdGsSOxqfpqWeA2FmcwBMaoEdz6b2x2si3IwC9/fSPLfe8pBMRTHVMk5nlwnFQ==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/utf8/-/utf8-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/wasm-edit": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/helper-buffer": "1.11.1",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.1",
-                "@webassemblyjs/helper-wasm-section": "1.11.1",
-                "@webassemblyjs/wasm-gen": "1.11.1",
-                "@webassemblyjs/wasm-opt": "1.11.1",
-                "@webassemblyjs/wasm-parser": "1.11.1",
-                "@webassemblyjs/wast-printer": "1.11.1"
+                "@webassemblyjs/ast": "1.11.5",
+                "@webassemblyjs/helper-buffer": "1.11.5",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.5",
+                "@webassemblyjs/helper-wasm-section": "1.11.5",
+                "@webassemblyjs/wasm-gen": "1.11.5",
+                "@webassemblyjs/wasm-opt": "1.11.5",
+                "@webassemblyjs/wasm-parser": "1.11.5",
+                "@webassemblyjs/wast-printer": "1.11.5"
             },
             "dev": true,
-            "integrity": "sha512-g+RsupUC1aTHfR8CDgnsVRVZFJqdkFHpsHMfJuWQzWU3tvnLC07UqHICfP+4XyL2tnr1amvl1Sdp06TnYCmVkA==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-edit/-/wasm-edit-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-C0p9D2fAu3Twwqvygvf42iGCQ4av8MFBLiTb+08SZ4cEdwzWx9QeAHDo1E2k+9s/0w1DM40oflJOpkZ8jW4HCQ==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-edit/-/wasm-edit-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/wasm-gen": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.1",
-                "@webassemblyjs/ieee754": "1.11.1",
-                "@webassemblyjs/leb128": "1.11.1",
-                "@webassemblyjs/utf8": "1.11.1"
+                "@webassemblyjs/ast": "1.11.5",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.5",
+                "@webassemblyjs/ieee754": "1.11.5",
+                "@webassemblyjs/leb128": "1.11.5",
+                "@webassemblyjs/utf8": "1.11.5"
             },
             "dev": true,
-            "integrity": "sha512-F7QqKXwwNlMmsulj6+O7r4mmtAlCWfO/0HdgOxSklZfQcDu0TpLiD1mRt/zF25Bk59FIjEuGAIyn5ei4yMfLhA==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-gen/-/wasm-gen-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-14vteRlRjxLK9eSyYFvw1K8Vv+iPdZU0Aebk3j6oB8TQiQYuO6hj9s4d7qf6f2HJr2khzvNldAFG13CgdkAIfA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-gen/-/wasm-gen-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/wasm-opt": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/helper-buffer": "1.11.1",
-                "@webassemblyjs/wasm-gen": "1.11.1",
-                "@webassemblyjs/wasm-parser": "1.11.1"
+                "@webassemblyjs/ast": "1.11.5",
+                "@webassemblyjs/helper-buffer": "1.11.5",
+                "@webassemblyjs/wasm-gen": "1.11.5",
+                "@webassemblyjs/wasm-parser": "1.11.5"
             },
             "dev": true,
-            "integrity": "sha512-VqnkNqnZlU5EB64pp1l7hdm3hmQw7Vgqa0KF/KCNO9sIpI6Fk6brDEiX+iCOYrvMuBWDws0NkTOxYEb85XQHHw==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-opt/-/wasm-opt-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-tcKwlIXstBQgbKy1MlbDMlXaxpucn42eb17H29rawYLxm5+MsEmgPzeCP8B1Cl69hCice8LeKgZpRUAPtqYPgw==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-opt/-/wasm-opt-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/wasm-parser": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/helper-api-error": "1.11.1",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.1",
-                "@webassemblyjs/ieee754": "1.11.1",
-                "@webassemblyjs/leb128": "1.11.1",
-                "@webassemblyjs/utf8": "1.11.1"
+                "@webassemblyjs/ast": "1.11.5",
+                "@webassemblyjs/helper-api-error": "1.11.5",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.5",
+                "@webassemblyjs/ieee754": "1.11.5",
+                "@webassemblyjs/leb128": "1.11.5",
+                "@webassemblyjs/utf8": "1.11.5"
             },
             "dev": true,
-            "integrity": "sha512-rrBujw+dJu32gYB7/Lup6UhdkPx9S9SnobZzRVL7VcBH9Bt9bCBLEuX/YXOOtBsOZ4NQrRykKhffRWHvigQvOA==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-parser/-/wasm-parser-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-SVXUIwsLQlc8srSD7jejsfTU83g7pIGr2YYNb9oHdtldSxaOhvA5xwvIiWIfcX8PlSakgqMXsLpLfbbJ4cBYew==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-parser/-/wasm-parser-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webassemblyjs/wast-printer": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.1",
+                "@webassemblyjs/ast": "1.11.5",
                 "@xtuc/long": "4.2.2"
             },
             "dev": true,
-            "integrity": "sha512-IQboUWM4eKzWW+N/jij2sRatKMh99QEelo3Eb2q0qXkvPRISAj8Qxtmw5itwqK+TTkBuUIE45AxYPToqPtL5gg==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wast-printer/-/wast-printer-1.11.1.tgz",
-            "version": "1.11.1"
+            "integrity": "sha512-f7Pq3wvg3GSPUPzR0F6bmI89Hdb+u9WXrSKc4v+N0aV0q6r42WoF92Jp2jEorBEBRoRNXgjp53nBniDXcqZYPA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wast-printer/-/wast-printer-1.11.5.tgz",
+            "version": "1.11.5"
         },
         "node_modules/@webpack-cli/configtest": {
             "dev": true,
             "engines": {
                 "node": ">=14.15.0"
             },
-            "integrity": "sha512-njsdJXJSiS2iNbQVS0eT8A/KPnmyH4pv1APj2K0d1wrZcBLw+yppxOy4CGqa0OxDJkzfL/XELDhD8rocnIwB5A==",
+            "integrity": "sha512-K/vuv72vpfSEZoo5KIU0a2FsEoYdW0DUMtMpB5X3LlUwshetMZRZRxB7sCsVji/lFaSxtQQ3aM9O4eMolXkU9w==",
             "peerDependencies": {
                 "webpack": "5.x.x",
                 "webpack-cli": "5.x.x"
             },
-            "resolved": "https://registry.npmjs.org/@webpack-cli/configtest/-/configtest-2.0.1.tgz",
-            "version": "2.0.1"
+            "resolved": "https://registry.npmjs.org/@webpack-cli/configtest/-/configtest-2.1.0.tgz",
+            "version": "2.1.0"
         },
         "node_modules/@webpack-cli/info": {
             "dev": true,
             "engines": {
                 "node": ">=14.15.0"
             },
             "integrity": "sha512-fE1UEWTwsAxRhrJNikE7v4EotYflkEhBL7EbajfkPlf6E37/2QshOy/D48Mw8G5XMFlQtS6YV42vtbG9zBpIQA==",
@@ -4390,26 +4460,26 @@
             "version": "2.0.1"
         },
         "node_modules/@webpack-cli/serve": {
             "dev": true,
             "engines": {
                 "node": ">=14.15.0"
             },
-            "integrity": "sha512-0G7tNyS+yW8TdgHwZKlDWYXFA6OJQnoLCQvYKkQP0Q2X205PSQ6RNUj0M+1OB/9gRQaUZ/ccYfaxd0nhaWKfjw==",
+            "integrity": "sha512-0xRgjgDLdz6G7+vvDLlaRpFatJaJ69uTalZLRSMX5B3VUrDmXcrVA3+6fXXQgmYz7bY9AAgs348XQdmtLsK41A==",
             "peerDependencies": {
                 "webpack": "5.x.x",
                 "webpack-cli": "5.x.x"
             },
             "peerDependenciesMeta": {
                 "webpack-dev-server": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/@webpack-cli/serve/-/serve-2.0.1.tgz",
-            "version": "2.0.1"
+            "resolved": "https://registry.npmjs.org/@webpack-cli/serve/-/serve-2.0.4.tgz",
+            "version": "2.0.4"
         },
         "node_modules/@xtuc/ieee754": {
             "dev": true,
             "integrity": "sha512-DX8nKgqcGwsc0eJSqYt5lwP4DH5FlHnmuWWBRy7X0NcaGR0ZtuyeESgMwTYVEtxmsNGY+qit4QYT/MIYTOTPeA==",
             "resolved": "https://registry.npmjs.org/@xtuc/ieee754/-/ieee754-1.2.0.tgz",
             "version": "1.2.0"
         },
@@ -4604,16 +4674,16 @@
             "version": "2.0.0"
         },
         "node_modules/autoprefixer": {
             "bin": {
                 "autoprefixer": "bin/autoprefixer"
             },
             "dependencies": {
-                "browserslist": "^4.21.4",
-                "caniuse-lite": "^1.0.30001426",
+                "browserslist": "^4.21.5",
+                "caniuse-lite": "^1.0.30001464",
                 "fraction.js": "^4.2.0",
                 "normalize-range": "^0.1.2",
                 "picocolors": "^1.0.0",
                 "postcss-value-parser": "^4.2.0"
             },
             "dev": true,
             "engines": {
@@ -4625,20 +4695,20 @@
                     "url": "https://opencollective.com/postcss/"
                 },
                 {
                     "type": "tidelift",
                     "url": "https://tidelift.com/funding/github/npm/autoprefixer"
                 }
             ],
-            "integrity": "sha512-49vKpMqcZYsJjwotvt4+h/BCjJVnhGwcLpDt5xkcaOG3eLrG/HUYLagrihYsQ+qrIBgIzX1Rw7a6L8I/ZA1Atg==",
+            "integrity": "sha512-FQzyfOsTlwVzjHxKEqRIAdJx9niO6VCBCoEwax/VLSoQF29ggECcPuBqUMZ+u8jCZOPSy8b8/8KnuFbp0SaFZQ==",
             "peerDependencies": {
                 "postcss": "^8.1.0"
             },
-            "resolved": "https://registry.npmjs.org/autoprefixer/-/autoprefixer-10.4.13.tgz",
-            "version": "10.4.13"
+            "resolved": "https://registry.npmjs.org/autoprefixer/-/autoprefixer-10.4.14.tgz",
+            "version": "10.4.14"
         },
         "node_modules/balanced-match": {
             "dev": true,
             "integrity": "sha512-1ugUSr8BHXRnK23KfuYS+gVMC3LB8QGH9W1iGtDPsNWoQbgtXSExkBu2aDR4epiGWZOjZsj6lDl/N/AqqTC3UA==",
             "resolved": "https://registry.npmjs.org/balanced-match/-/balanced-match-2.0.0.tgz",
             "version": "2.0.0"
         },
@@ -4659,18 +4729,18 @@
             "version": "1.0.2"
         },
         "node_modules/browserslist": {
             "bin": {
                 "browserslist": "cli.js"
             },
             "dependencies": {
-                "caniuse-lite": "^1.0.30001400",
-                "electron-to-chromium": "^1.4.251",
-                "node-releases": "^2.0.6",
-                "update-browserslist-db": "^1.0.9"
+                "caniuse-lite": "^1.0.30001449",
+                "electron-to-chromium": "^1.4.284",
+                "node-releases": "^2.0.8",
+                "update-browserslist-db": "^1.0.10"
             },
             "dev": true,
             "engines": {
                 "node": "^6 || ^7 || ^8 || ^9 || ^10 || ^11 || ^12 || >=13.7"
             },
             "funding": [
                 {
@@ -4678,17 +4748,17 @@
                     "url": "https://opencollective.com/browserslist"
                 },
                 {
                     "type": "tidelift",
                     "url": "https://tidelift.com/funding/github/npm/browserslist"
                 }
             ],
-            "integrity": "sha512-CBHJJdDmgjl3daYjN5Cp5kbTf1mUhZoS+beLklHIvkOWscs83YAhLlF3Wsh/lciQYAcbBJgTOD44VtG31ZM4Hw==",
-            "resolved": "https://registry.npmjs.org/browserslist/-/browserslist-4.21.4.tgz",
-            "version": "4.21.4"
+            "integrity": "sha512-tUkiguQGW7S3IhB7N+c2MV/HZPSCPAAiYBZXLsBhFB/PCy6ZKKsZrmBayHV9fdGV/ARIfJ14NkxKzRDjvp7L6w==",
+            "resolved": "https://registry.npmjs.org/browserslist/-/browserslist-4.21.5.tgz",
+            "version": "4.21.5"
         },
         "node_modules/buffer-from": {
             "dev": true,
             "integrity": "sha512-E+XQCRwSbaaiChtv6k6Dwgc+bx+Bs6vuKJHHl5kox/BaKbhiXzqQOwK4cO22yElGp2OCmjwVhT3HmxgyPGnJfQ==",
             "resolved": "https://registry.npmjs.org/buffer-from/-/buffer-from-1.1.2.tgz",
             "version": "1.1.2"
         },
@@ -4755,19 +4825,23 @@
                 {
                     "type": "opencollective",
                     "url": "https://opencollective.com/browserslist"
                 },
                 {
                     "type": "tidelift",
                     "url": "https://tidelift.com/funding/github/npm/caniuse-lite"
+                },
+                {
+                    "type": "github",
+                    "url": "https://github.com/sponsors/ai"
                 }
             ],
-            "integrity": "sha512-511ThLu1hF+5RRRt0zYCf2U2yRr9GPF6m5y90SBCWsvSoYoW7yAGlv/elyPaNfvGCkp6kj/KFZWU0BMA69Prsg==",
-            "resolved": "https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001429.tgz",
-            "version": "1.0.30001429"
+            "integrity": "sha512-ewDad7+D2vlyy+E4UJuVfiBsU69IL+8oVmTuZnH5Q6CIUbxNfI50uVpRHbUPDD6SUaN2o0Lh4DhTrvLG/Tn1yg==",
+            "resolved": "https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001473.tgz",
+            "version": "1.0.30001473"
         },
         "node_modules/chalk": {
             "dependencies": {
                 "ansi-styles": "^3.2.1",
                 "escape-string-regexp": "^1.0.5",
                 "supports-color": "^5.3.0"
             },
@@ -4849,41 +4923,43 @@
             "integrity": "sha512-hUewv7oMjCp+wkBv5Rm0v87eJhq4woh5rSR+42YSQJKecCqgIqNkZ6lAlQms/BwHPJA5NKMRlpxPRv0n8HQW6g==",
             "resolved": "https://registry.npmjs.org/colorette/-/colorette-2.0.16.tgz",
             "version": "2.0.16"
         },
         "node_modules/commander": {
             "dev": true,
             "engines": {
-                "node": "^12.20.0 || >=14"
+                "node": ">=14"
             },
-            "integrity": "sha512-KRs7WVDKg86PWiuAqhDrAQnTXZKraVcCc6vFdL14qrZ/DcWwuRo7VoiYXalXO7S5GKpqYiVEwCbgFDfxNHKJBQ==",
-            "resolved": "https://registry.npmjs.org/commander/-/commander-9.5.0.tgz",
-            "version": "9.5.0"
+            "integrity": "sha512-y4Mg2tXshplEbSGzx7amzPwKKOCGuoSRP/CjEdwwk0FOGlUbq6lKuoyDZTNZkmxHdJtp54hdfY/JUrdL7Xfdug==",
+            "resolved": "https://registry.npmjs.org/commander/-/commander-10.0.1.tgz",
+            "version": "10.0.1"
         },
         "node_modules/concat-map": {
             "dev": true,
             "integrity": "sha1-2Klr13/Wjfd5OnMDajug1UBdR3s=",
             "resolved": "https://registry.npmjs.org/concat-map/-/concat-map-0.0.1.tgz",
             "version": "0.0.1"
         },
         "node_modules/cosmiconfig": {
             "dependencies": {
-                "@types/parse-json": "^4.0.0",
                 "import-fresh": "^3.2.1",
+                "js-yaml": "^4.1.0",
                 "parse-json": "^5.0.0",
-                "path-type": "^4.0.0",
-                "yaml": "^1.10.0"
+                "path-type": "^4.0.0"
             },
             "dev": true,
             "engines": {
-                "node": ">=10"
+                "node": ">=14"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/d-fischer"
             },
-            "integrity": "sha512-AdmX6xUzdNASswsFtmwSt7Vj8po9IuqXm0UXz7QKPuEUmPB4XyjGfaAr2PSuELMwkRMVH1EpIkX5bTZGRB3eCA==",
-            "resolved": "https://registry.npmjs.org/cosmiconfig/-/cosmiconfig-7.1.0.tgz",
-            "version": "7.1.0"
+            "integrity": "sha512-/UkO2JKI18b5jVMJUp0lvKFMpa/Gye+ZgZjKD+DGEN9y7NRcf/nK1A0sp67ONmKtnDCNMS44E6jrk0Yc3bDuUw==",
+            "resolved": "https://registry.npmjs.org/cosmiconfig/-/cosmiconfig-8.1.3.tgz",
+            "version": "8.1.3"
         },
         "node_modules/cross-spawn": {
             "dependencies": {
                 "path-key": "^3.1.0",
                 "shebang-command": "^2.0.0",
                 "which": "^2.0.1"
             },
@@ -4941,14 +5017,27 @@
             "integrity": "sha512-qhOH1KlBMnZP8FzRO6YCH9UHXQhVMcEGLyNdb7Hv2cpcmJbW0YrddO+tG1ab5nT41KpHIYGsbeHqxB9xPu1pKQ==",
             "peerDependencies": {
                 "webpack": "^5.0.0"
             },
             "resolved": "https://registry.npmjs.org/css-loader/-/css-loader-6.7.3.tgz",
             "version": "6.7.3"
         },
+        "node_modules/css-tree": {
+            "dependencies": {
+                "mdn-data": "2.0.30",
+                "source-map-js": "^1.0.1"
+            },
+            "dev": true,
+            "engines": {
+                "node": "^10 || ^12.20.0 || ^14.13.0 || >=15.0.0"
+            },
+            "integrity": "sha512-6Fv1DV/TYw//QF5IzQdqsNDjx/wc8TrMBZsqjL9eW01tWb7R7k/mq+/VXfJCl7SoD5emsJop9cOByJZfs8hYIw==",
+            "resolved": "https://registry.npmjs.org/css-tree/-/css-tree-2.3.1.tgz",
+            "version": "2.3.1"
+        },
         "node_modules/cssesc": {
             "bin": {
                 "cssesc": "bin/cssesc"
             },
             "dev": true,
             "engines": {
                 "node": ">=4"
@@ -5049,17 +5138,17 @@
             },
             "integrity": "sha512-yS+Q5i3hBf7GBkd4KG8a7eBNNWNGLTaEwwYWUijIYM7zrlYDM0BFXHjjPWlWZ1Rg7UaddZeIDmi9jF3HmqiQ2w==",
             "resolved": "https://registry.npmjs.org/doctrine/-/doctrine-3.0.0.tgz",
             "version": "3.0.0"
         },
         "node_modules/electron-to-chromium": {
             "dev": true,
-            "integrity": "sha512-KNhIzgLiJmDDC444dj9vEOpZEgsV96ult9Iff98Vanumn+ShJHd5se8aX6KeVxdc0YQeqdrezBZv89rleDbvSg==",
-            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.270.tgz",
-            "version": "1.4.270"
+            "integrity": "sha512-gM7TdwuG3amns/1rlgxMbeeyNoBFPa+4Uu0c7FeROWh4qWmvSOnvcslKmWy51ggLKZ2n/F/4i2HJ+PVNxH9uCQ==",
+            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.348.tgz",
+            "version": "1.4.348"
         },
         "node_modules/emoji-regex": {
             "dev": true,
             "integrity": "sha512-MSjYzcWNOA0ewAHpz0MxpYFvwg6yjy1NG3xteoqz644VCo/RPgnr1/GGt+ic3iJTzQ8Eu3TdM14SawnVUmGE6A==",
             "resolved": "https://registry.npmjs.org/emoji-regex/-/emoji-regex-8.0.0.tgz",
             "version": "8.0.0"
         },
@@ -5068,17 +5157,17 @@
                 "graceful-fs": "^4.2.4",
                 "tapable": "^2.2.0"
             },
             "dev": true,
             "engines": {
                 "node": ">=10.13.0"
             },
-            "integrity": "sha512-T0yTFjdpldGY8PmuXXR0PyQ1ufZpEGiHVrp7zHKB7jdR4qlmZHhONVM5AQOAWXuF/w3dnHbEQVrNptJgt7F+cQ==",
-            "resolved": "https://registry.npmjs.org/enhanced-resolve/-/enhanced-resolve-5.10.0.tgz",
-            "version": "5.10.0"
+            "integrity": "sha512-eyV8f0y1+bzyfh8xAwW/WTSZpLbjhqc4ne9eGSH4Zo2ejdyiNG9pU6mf9DG8a7+Auk6MFTlNOT4Y2y/9k8GKVg==",
+            "resolved": "https://registry.npmjs.org/enhanced-resolve/-/enhanced-resolve-5.13.0.tgz",
+            "version": "5.13.0"
         },
         "node_modules/envinfo": {
             "bin": {
                 "envinfo": "dist/cli.js"
             },
             "dev": true,
             "engines": {
@@ -5129,17 +5218,17 @@
             },
             "integrity": "sha512-Aa2G2+Rd3b6kxEUKTF4TaW67czBLyAv3z7VOhYRU50YBx+bbsYZ9xQP4lMNazePuFlybXI0V4MruPos7qUo5fA==",
             "resolved": "https://registry.npmjs.org/es-abstract/-/es-abstract-1.19.5.tgz",
             "version": "1.19.5"
         },
         "node_modules/es-module-lexer": {
             "dev": true,
-            "integrity": "sha512-1HQ2M2sPtxwnvOvT1ZClHyQDiggdNjURWpY2we6aMKCQiUVxTmVs2UYPLIrD84sS+kMdUwfBSylbJPwNnBrnHQ==",
-            "resolved": "https://registry.npmjs.org/es-module-lexer/-/es-module-lexer-0.9.3.tgz",
-            "version": "0.9.3"
+            "integrity": "sha512-9978wrXM50Y4rTMmW5kXIC09ZdXQZqkE4mxhwkd8VbzsGkXGPgV4zWuqQJgCEzYngdo2dYDa0l8xhX4fkSwJSg==",
+            "resolved": "https://registry.npmjs.org/es-module-lexer/-/es-module-lexer-1.2.1.tgz",
+            "version": "1.2.1"
         },
         "node_modules/es-shim-unscopables": {
             "dependencies": {
                 "has": "^1.0.3"
             },
             "dev": true,
             "integrity": "sha512-Jm6GPcCdC30eMLbZ2x8z2WuRwAws3zTBBKuusffYVUrNj/GVSUAZ+xKMaUpfNDR5IbyNA5LJbaecoUVbmUcB1w==",
@@ -6302,17 +6391,17 @@
             "dev": true,
             "engines": {
                 "node": ">=8"
             },
             "funding": {
                 "url": "https://github.com/sponsors/sindresorhus"
             },
-            "integrity": "sha512-vy7ClnArOZwCnqZgvv+ddgHgJiAFXe3Ge9ML5/mBctVJoUoYPCdxVucOywjDARn6CVoh3dRSFdPHy2sX80L0Wg==",
-            "resolved": "https://registry.npmjs.org/html-tags/-/html-tags-3.2.0.tgz",
-            "version": "3.2.0"
+            "integrity": "sha512-ztqyC3kLto0e9WbNp0aeP+M3kTt+nbaIveGmUxAtZa+8iFgKLUOD4YKM5j+f3QD89bra7UeumolZHKuOXnTmeQ==",
+            "resolved": "https://registry.npmjs.org/html-tags/-/html-tags-3.3.1.tgz",
+            "version": "3.3.1"
         },
         "node_modules/icss-utils": {
             "dev": true,
             "engines": {
                 "node": "^10 || ^12 || >= 14"
             },
             "integrity": "sha512-soFhflCVWLfRNOPU3iv5Z9VUdT44xFRbzjLsEzSr5AQmgqPMTHdU3PMT1Cf1ssx8fLNJDA1juftYl+PUcv3MqA==",
@@ -6720,14 +6809,23 @@
             "funding": {
                 "url": "https://github.com/chalk/supports-color?sponsor=1"
             },
             "integrity": "sha512-MpUEN2OodtUzxvKQl72cUF7RQ5EiHsGvSsVG0ia9c5RbWGL2CI4C7EpPS8UTBIplnlzZiNuV56w+FuNxy3ty2Q==",
             "resolved": "https://registry.npmjs.org/supports-color/-/supports-color-8.1.1.tgz",
             "version": "8.1.1"
         },
+        "node_modules/jiti": {
+            "bin": {
+                "jiti": "bin/jiti.js"
+            },
+            "dev": true,
+            "integrity": "sha512-QAdOptna2NYiSSpv0O/BwoHBSmz4YhpzJHyi+fnMRTXFjp7B8i/YG5Z8IfusxB1ufjcD2Sre1F3R+nX3fvy7gg==",
+            "resolved": "https://registry.npmjs.org/jiti/-/jiti-1.18.2.tgz",
+            "version": "1.18.2"
+        },
         "node_modules/js-tokens": {
             "dev": true,
             "integrity": "sha512-RdJUflcE3cUzKiMqQgsCu06FPu9UdIJO0beYbPhHN4k6apgJtifcoCtT9bcxOpYBtpD2kCM6Sbzg4CausW/PKQ==",
             "resolved": "https://registry.npmjs.org/js-tokens/-/js-tokens-4.0.0.tgz",
             "version": "4.0.0"
         },
         "node_modules/js-yaml": {
@@ -6792,23 +6890,23 @@
             "version": "3.3.0"
         },
         "node_modules/klona": {
             "dev": true,
             "engines": {
                 "node": ">= 8"
             },
-            "integrity": "sha512-pJiBpiXMbt7dkzXe8Ghj/u4FfXOOa98fPW+bihOJ4SjnoijweJrNThJfd3ifXpXhREjpoF2mZVH1GfS9LV3kHQ==",
-            "resolved": "https://registry.npmjs.org/klona/-/klona-2.0.5.tgz",
-            "version": "2.0.5"
+            "integrity": "sha512-dhG34DXATL5hSxJbIexCft8FChFXtmskoZYnoPWjXQuebWYCNkVeV3KkGegCK9CP1oswI/vQibS2GY7Em/sJJA==",
+            "resolved": "https://registry.npmjs.org/klona/-/klona-2.0.6.tgz",
+            "version": "2.0.6"
         },
         "node_modules/known-css-properties": {
             "dev": true,
-            "integrity": "sha512-5FZRzrZzNTBruuurWpvZnvP9pum+fe0HcK8z/ooo+U+Hmp4vtbyp1/QDsqmufirXy4egGzbaH/y2uCZf+6W5Kg==",
-            "resolved": "https://registry.npmjs.org/known-css-properties/-/known-css-properties-0.26.0.tgz",
-            "version": "0.26.0"
+            "integrity": "sha512-uMCj6+hZYDoffuvAJjFAPz56E9uoowFHmTkqRtRq5WyC5Q6Cu/fTZKNQpX/RbzChBYLLl3lo8CjFZBAZXq9qFg==",
+            "resolved": "https://registry.npmjs.org/known-css-properties/-/known-css-properties-0.27.0.tgz",
+            "version": "0.27.0"
         },
         "node_modules/levn": {
             "dependencies": {
                 "prelude-ls": "^1.2.1",
                 "type-check": "~0.4.0"
             },
             "dev": true,
@@ -6880,20 +6978,14 @@
             "engines": {
                 "node": ">=8"
             },
             "integrity": "sha512-t7hw9pI+WvuwNJXwk5zVHpyhIqzg2qTlklJOf0mVxGSbe3Fp2VieZcduNYjaLDoy6p9uGpQEGWG87WpMKlNq8g==",
             "resolved": "https://registry.npmjs.org/locate-path/-/locate-path-5.0.0.tgz",
             "version": "5.0.0"
         },
-        "node_modules/lodash": {
-            "dev": true,
-            "integrity": "sha512-v2kDEe57lecTulaDIuNTPy3Ry4gLGJ6Z1O3vE1krgXZNrsQ+LFTGHVxVjcXPs17LhbZVGedAJv8XZ1tvj5FvSg==",
-            "resolved": "https://registry.npmjs.org/lodash/-/lodash-4.17.21.tgz",
-            "version": "4.17.21"
-        },
         "node_modules/lodash.merge": {
             "dev": true,
             "integrity": "sha512-0KpjqXRVvrYyCsX1swR/XTK0va6VQkQM6MNo7PqW77ByjAhoARA8EfrP1N4+KlKj8YS0ZUCtRT/YUuhyYDujIQ==",
             "resolved": "https://registry.npmjs.org/lodash.merge/-/lodash.merge-4.6.2.tgz",
             "version": "4.6.2"
         },
         "node_modules/lodash.truncate": {
@@ -6944,14 +7036,20 @@
                 "type": "github",
                 "url": "https://github.com/sponsors/wooorm"
             },
             "integrity": "sha512-APMBEanjybaPzUrfqU0IMU5I0AswKMH7k8OTLs0vvV4KZpExkTkY87nR/zpbuTPj+gARop7aGUbl11pnDfW6xg==",
             "resolved": "https://registry.npmjs.org/mathml-tag-names/-/mathml-tag-names-2.1.3.tgz",
             "version": "2.1.3"
         },
+        "node_modules/mdn-data": {
+            "dev": true,
+            "integrity": "sha512-GaqWWShW4kv/G9IEucWScBx9G1/vsFZZJUO+tD26M8J8z3Kw5RDQjaoZe03YAClgeS/SWPOcb4nkFBTEi5DUEA==",
+            "resolved": "https://registry.npmjs.org/mdn-data/-/mdn-data-2.0.30.tgz",
+            "version": "2.0.30"
+        },
         "node_modules/meow": {
             "dependencies": {
                 "@types/minimist": "^1.2.0",
                 "camelcase-keys": "^6.2.2",
                 "decamelize": "^1.2.0",
                 "decamelize-keys": "^1.1.0",
                 "hard-rejection": "^2.1.0",
@@ -7027,20 +7125,20 @@
             "engines": {
                 "node": ">= 12.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-EdlUizq13o0Pd+uCp+WO/JpkLvHRVGt97RqfeGhXqAcorYo1ypJSpkV+WDT0vY/kmh/p7wRdJNJtuyK540PXDw==",
+            "integrity": "sha512-9HaR++0mlgom81s95vvNjxkg52n2b5s//3ZTI1EtzFb98awsLSivs2LMsVqnQ3ay0PVhqWcGNyDaTE961FOcjQ==",
             "peerDependencies": {
                 "webpack": "^5.0.0"
             },
-            "resolved": "https://registry.npmjs.org/mini-css-extract-plugin/-/mini-css-extract-plugin-2.7.2.tgz",
-            "version": "2.7.2"
+            "resolved": "https://registry.npmjs.org/mini-css-extract-plugin/-/mini-css-extract-plugin-2.7.5.tgz",
+            "version": "2.7.5"
         },
         "node_modules/mini-css-extract-plugin/node_modules/schema-utils": {
             "dependencies": {
                 "@types/json-schema": "^7.0.9",
                 "ajv": "^8.8.0",
                 "ajv-formats": "^2.1.1",
                 "ajv-keywords": "^5.0.0"
@@ -7108,17 +7206,23 @@
             "bin": {
                 "nanoid": "bin/nanoid.cjs"
             },
             "dev": true,
             "engines": {
                 "node": "^10 || ^12 || ^13.7 || ^14 || >=15.0.1"
             },
-            "integrity": "sha512-MqBkQh/OHTS2egovRtLk45wEyNXwF+cokD+1YPf9u5VfJiRdAiRwB2froX5Co9Rh20xs4siNPm8naNotSD6RBw==",
-            "resolved": "https://registry.npmjs.org/nanoid/-/nanoid-3.3.4.tgz",
-            "version": "3.3.4"
+            "funding": [
+                {
+                    "type": "github",
+                    "url": "https://github.com/sponsors/ai"
+                }
+            ],
+            "integrity": "sha512-BGcqMMJuToF7i1rt+2PWSNVnWIkGCU78jBG3RxO/bZlnZPK2Cmi2QaffxGO/2RvWi9sL+FAiRiXMgsyxQ1DIDA==",
+            "resolved": "https://registry.npmjs.org/nanoid/-/nanoid-3.3.6.tgz",
+            "version": "3.3.6"
         },
         "node_modules/natural-compare": {
             "dev": true,
             "integrity": "sha1-Sr6/7tdUHywnrPspvbvRXI1bpPc=",
             "resolved": "https://registry.npmjs.org/natural-compare/-/natural-compare-1.4.0.tgz",
             "version": "1.4.0"
         },
@@ -7126,17 +7230,17 @@
             "dev": true,
             "integrity": "sha512-Yd3UES5mWCSqR+qNT93S3UoYUkqAZ9lLg8a7g9rimsWmYGK8cVToA4/sF3RrshdyV3sAGMXVUmpMYOw+dLpOuw==",
             "resolved": "https://registry.npmjs.org/neo-async/-/neo-async-2.6.2.tgz",
             "version": "2.6.2"
         },
         "node_modules/node-releases": {
             "dev": true,
-            "integrity": "sha512-PiVXnNuFm5+iYkLBNeq5211hvO38y63T0i2KKh2KnUs3RpzJ+JtODFjkD8yjLwnDkTYF1eKXheUwdssR+NRZdg==",
-            "resolved": "https://registry.npmjs.org/node-releases/-/node-releases-2.0.6.tgz",
-            "version": "2.0.6"
+            "integrity": "sha512-5GFldHPXVG/YZmFzJvKK2zDSzPKhEp0+ZR5SVaoSag9fsL5YgHbUHDfnG5494ISANDcK4KwPXAx2xqVEydmd7w==",
+            "resolved": "https://registry.npmjs.org/node-releases/-/node-releases-2.0.10.tgz",
+            "version": "2.0.10"
         },
         "node_modules/normalize-package-data": {
             "dependencies": {
                 "hosted-git-info": "^4.0.1",
                 "is-core-module": "^2.5.0",
                 "semver": "^7.3.4",
                 "validate-npm-package-license": "^3.0.1"
@@ -7503,15 +7607,15 @@
             },
             "integrity": "sha512-HRDzbaKjC+AOWVXxAU/x54COGeIv9eb+6CkDSQoNTt4XyWoIJvuPsXizxu/Fr23EiekbtZwmh1IcIG/l/a10GQ==",
             "resolved": "https://registry.npmjs.org/pkg-dir/-/pkg-dir-4.2.0.tgz",
             "version": "4.2.0"
         },
         "node_modules/postcss": {
             "dependencies": {
-                "nanoid": "^3.3.4",
+                "nanoid": "^3.3.6",
                 "picocolors": "^1.0.0",
                 "source-map-js": "^1.0.2"
             },
             "dev": true,
             "engines": {
                 "node": "^10 || ^12 || >=14"
             },
@@ -7519,41 +7623,46 @@
                 {
                     "type": "opencollective",
                     "url": "https://opencollective.com/postcss/"
                 },
                 {
                     "type": "tidelift",
                     "url": "https://tidelift.com/funding/github/npm/postcss"
+                },
+                {
+                    "type": "github",
+                    "url": "https://github.com/sponsors/ai"
                 }
             ],
-            "integrity": "sha512-tP7u/Sn/dVxK2NnruI4H9BG+x+Wxz6oeZ1cJ8P6G/PZY0IKk4k/63TDsQf2kQq3+qoJeLm2kIBUNlZe3zgb4Zg==",
-            "resolved": "https://registry.npmjs.org/postcss/-/postcss-8.4.21.tgz",
-            "version": "8.4.21"
+            "integrity": "sha512-bQ3qMcpF6A/YjR55xtoTr0jGOlnPOKAIMdOWiv0EIT6HVPEaJiJB4NLljSbiHoC2RX7DN5Uvjtpbg1NPdwv1oA==",
+            "resolved": "https://registry.npmjs.org/postcss/-/postcss-8.4.23.tgz",
+            "version": "8.4.23"
         },
         "node_modules/postcss-loader": {
             "dependencies": {
-                "cosmiconfig": "^7.0.0",
-                "klona": "^2.0.5",
+                "cosmiconfig": "^8.1.3",
+                "jiti": "^1.18.2",
+                "klona": "^2.0.6",
                 "semver": "^7.3.8"
             },
             "dev": true,
             "engines": {
                 "node": ">= 14.15.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-fUJzV/QH7NXUAqV8dWJ9Lg4aTkDCezpTS5HgJ2DvqznexTbSTxgi/dTECvTZ15BwKTtk8G/bqI/QTu2HPd3ZCg==",
+            "integrity": "sha512-qLAFjvR2BFNz1H930P7mj1iuWJFjGey/nVhimfOAAQ1ZyPpcClAxP8+A55Sl8mBvM+K2a9Pjgdj10KpANWrNfw==",
             "peerDependencies": {
                 "postcss": "^7.0.0 || ^8.0.1",
                 "webpack": "^5.0.0"
             },
-            "resolved": "https://registry.npmjs.org/postcss-loader/-/postcss-loader-7.0.2.tgz",
-            "version": "7.0.2"
+            "resolved": "https://registry.npmjs.org/postcss-loader/-/postcss-loader-7.3.0.tgz",
+            "version": "7.3.0"
         },
         "node_modules/postcss-media-query-parser": {
             "dev": true,
             "integrity": "sha1-J7Ocb02U+Bsac7j3Y1HGCeXO8kQ=",
             "resolved": "https://registry.npmjs.org/postcss-media-query-parser/-/postcss-media-query-parser-0.2.3.tgz",
             "version": "0.2.3"
         },
@@ -7649,20 +7758,20 @@
                     "url": "https://opencollective.com/postcss/"
                 },
                 {
                     "type": "tidelift",
                     "url": "https://tidelift.com/funding/github/npm/postcss-scss"
                 }
             ],
-            "integrity": "sha512-F7xpB6TrXyqUh3GKdyB4Gkp3QL3DDW1+uI+gxx/oJnUt/qXI4trj5OGlp9rOKdoABGULuqtqeG+3HEVQk4DjmA==",
+            "integrity": "sha512-rLDPhJY4z/i4nVFZ27j9GqLxj1pwxE80eAzUNRMXtcpipFYIeowerzBgG3yJhMtObGEXidtIgbUpQ3eLDsf5OQ==",
             "peerDependencies": {
-                "postcss": "^8.3.3"
+                "postcss": "^8.4.19"
             },
-            "resolved": "https://registry.npmjs.org/postcss-scss/-/postcss-scss-4.0.5.tgz",
-            "version": "4.0.5"
+            "resolved": "https://registry.npmjs.org/postcss-scss/-/postcss-scss-4.0.6.tgz",
+            "version": "4.0.6"
         },
         "node_modules/postcss-selector-parser": {
             "dependencies": {
                 "cssesc": "^3.0.0",
                 "util-deprecate": "^1.0.2"
             },
             "dev": true,
@@ -7976,49 +8085,63 @@
             ],
             "integrity": "sha512-5l4VyZR86LZ/lDxZTR6jqL8AFE2S0IFLMP26AbjsLVADxHdhB/c0GUsH+y39UfCi3dzz8OlQuPmnaJOMoDHQBA==",
             "resolved": "https://registry.npmjs.org/run-parallel/-/run-parallel-1.2.0.tgz",
             "version": "1.2.0"
         },
         "node_modules/safe-buffer": {
             "dev": true,
-            "integrity": "sha512-Gd2UZBJDkXlY7GbJxfsE8/nvKkUEU1G38c1siN6QP6a9PT9MmHB8GnpscSmMJSoF8LOIrt8ud/wPtojys4G6+g==",
-            "resolved": "https://registry.npmjs.org/safe-buffer/-/safe-buffer-5.1.2.tgz",
-            "version": "5.1.2"
+            "funding": [
+                {
+                    "type": "github",
+                    "url": "https://github.com/sponsors/feross"
+                },
+                {
+                    "type": "patreon",
+                    "url": "https://www.patreon.com/feross"
+                },
+                {
+                    "type": "consulting",
+                    "url": "https://feross.org/support"
+                }
+            ],
+            "integrity": "sha512-rp3So07KcdmmKbGvgaNxQSJr7bGVSVk5S9Eq1F+ppbRo70+YeaDxkw5Dd8NPN+GD6bjnYm2VuPuCXmpuYvmCXQ==",
+            "resolved": "https://registry.npmjs.org/safe-buffer/-/safe-buffer-5.2.1.tgz",
+            "version": "5.2.1"
         },
         "node_modules/sass": {
             "bin": {
                 "sass": "sass.js"
             },
             "dependencies": {
                 "chokidar": ">=3.0.0 <4.0.0",
                 "immutable": "^4.0.0",
                 "source-map-js": ">=0.6.2 <2.0.0"
             },
             "dev": true,
             "engines": {
-                "node": ">=12.0.0"
+                "node": ">=14.0.0"
             },
-            "integrity": "sha512-Q7RaEtYf6BflYrQ+buPudKR26/lH+10EmO9bBqbmPh/KeLqv8bjpTNqxe71ocONqXq+jYiCbpPUmQMS+JJPk4A==",
-            "resolved": "https://registry.npmjs.org/sass/-/sass-1.58.3.tgz",
-            "version": "1.58.3"
+            "integrity": "sha512-NHpxIzN29MXvWiuswfc1W3I0N8SXBd8UR26WntmDlRYf0bSADnwnOjsyMZ3lMezSlArD33Vs3YFhp7dWvL770A==",
+            "resolved": "https://registry.npmjs.org/sass/-/sass-1.62.1.tgz",
+            "version": "1.62.1"
         },
         "node_modules/sass-loader": {
             "dependencies": {
-                "klona": "^2.0.4",
+                "klona": "^2.0.6",
                 "neo-async": "^2.6.2"
             },
             "dev": true,
             "engines": {
                 "node": ">= 14.15.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-JWEp48djQA4nbZxmgC02/Wh0eroSUutulROUusYJO9P9zltRbNN80JCBHqRGzjd4cmZCa/r88xgfkjGD0TXsHg==",
+            "integrity": "sha512-nrIdVAAte3B9icfBiGWvmMhT/D+eCDwnk+yA7VE/76dp/WkHX+i44Q/pfo71NYbwj0Ap+PGsn0ekOuU1WFJ2AA==",
             "peerDependencies": {
                 "fibers": ">= 3.1.0",
                 "node-sass": "^4.0.0 || ^5.0.0 || ^6.0.0 || ^7.0.0 || ^8.0.0",
                 "sass": "^1.3.0",
                 "sass-embedded": "*",
                 "webpack": "^5.0.0"
             },
@@ -8032,16 +8155,16 @@
                 "sass": {
                     "optional": true
                 },
                 "sass-embedded": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/sass-loader/-/sass-loader-13.2.0.tgz",
-            "version": "13.2.0"
+            "resolved": "https://registry.npmjs.org/sass-loader/-/sass-loader-13.2.2.tgz",
+            "version": "13.2.2"
         },
         "node_modules/sass/node_modules/anymatch": {
             "dependencies": {
                 "normalize-path": "^3.0.0",
                 "picomatch": "^2.0.4"
             },
             "dev": true,
@@ -8181,17 +8304,17 @@
             "engines": {
                 "node": ">= 10.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-Y5PQxS4ITlC+EahLuXaY86TXfR7Dc5lw294alXOq86JAHCihAIZfqv8nNCWvaEJvaC51uN9hbLGeV0cFBdH+Fw==",
-            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-3.1.1.tgz",
-            "version": "3.1.1"
+            "integrity": "sha512-pvjEHOgWc9OWA/f/DE3ohBWTD6EleVLf7iFUkoSwAxttdBhB9QUebQgxER2kWueOvRJXPHNnyrvvh9eZINB8Eg==",
+            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-3.1.2.tgz",
+            "version": "3.1.2"
         },
         "node_modules/schema-utils/node_modules/ajv": {
             "dependencies": {
                 "fast-deep-equal": "^3.1.1",
                 "fast-json-stable-stringify": "^2.0.0",
                 "json-schema-traverse": "^0.4.1",
                 "uri-js": "^4.2.2"
@@ -8236,17 +8359,17 @@
             "version": "7.3.8"
         },
         "node_modules/serialize-javascript": {
             "dependencies": {
                 "randombytes": "^2.1.0"
             },
             "dev": true,
-            "integrity": "sha512-Qr3TosvguFt8ePWqsvRfrKyQXIiW+nGbYpy8XK24NQHE83caxWt+mIymTT19DGFbNWNLfEwsrkSmN64lVWB9ag==",
-            "resolved": "https://registry.npmjs.org/serialize-javascript/-/serialize-javascript-6.0.0.tgz",
-            "version": "6.0.0"
+            "integrity": "sha512-owoXEFjWRllis8/M1Q+Cw5k8ZH40e3zhp/ovX+Xr/vi1qj6QesbyXXViFbpNvWvPNAD62SutwEXavefrLJWj7w==",
+            "resolved": "https://registry.npmjs.org/serialize-javascript/-/serialize-javascript-6.0.1.tgz",
+            "version": "6.0.1"
         },
         "node_modules/shallow-clone": {
             "dependencies": {
                 "kind-of": "^6.0.2"
             },
             "dev": true,
             "engines": {
@@ -8361,14 +8484,23 @@
         },
         "node_modules/slice-ansi/node_modules/color-name": {
             "dev": true,
             "integrity": "sha512-dOy+3AuW3a2wNbZHIuMZpTcgjGuLU/uBL/ubcZF9OXbDo8ff4O8yVp5Bf0efS8uEoYo5q4Fx7dY9OgQGXgAsQA==",
             "resolved": "https://registry.npmjs.org/color-name/-/color-name-1.1.4.tgz",
             "version": "1.1.4"
         },
+        "node_modules/source-map": {
+            "dev": true,
+            "engines": {
+                "node": ">=0.10.0"
+            },
+            "integrity": "sha512-UjgapumWlbMhkBgzT7Ykc5YXUT46F0iKu8SGXq0bcwP5dz/h0Plj6enJqjz1Zbq2l5WaqYnrVbwWOWMyF3F47g==",
+            "resolved": "https://registry.npmjs.org/source-map/-/source-map-0.6.1.tgz",
+            "version": "0.6.1"
+        },
         "node_modules/source-map-js": {
             "dev": true,
             "engines": {
                 "node": ">=0.10.0"
             },
             "integrity": "sha512-R0XvVJ9WusLiqTCEiGCmICCMplcCkIwwR11mOSD9CR5u+IXYdiseeEuXCVAjS54zqwkLcPNnmU4OeJ6tUrWhDw==",
             "resolved": "https://registry.npmjs.org/source-map-js/-/source-map-js-1.0.2.tgz",
@@ -8380,23 +8512,14 @@
                 "source-map": "^0.6.0"
             },
             "dev": true,
             "integrity": "sha512-uBHU3L3czsIyYXKX88fdrGovxdSCoTGDRZ6SYXtSRxLZUzHg5P/66Ht6uoUlHu9EZod+inXhKo3qQgwXUT/y1w==",
             "resolved": "https://registry.npmjs.org/source-map-support/-/source-map-support-0.5.21.tgz",
             "version": "0.5.21"
         },
-        "node_modules/source-map-support/node_modules/source-map": {
-            "dev": true,
-            "engines": {
-                "node": ">=0.10.0"
-            },
-            "integrity": "sha512-UjgapumWlbMhkBgzT7Ykc5YXUT46F0iKu8SGXq0bcwP5dz/h0Plj6enJqjz1Zbq2l5WaqYnrVbwWOWMyF3F47g==",
-            "resolved": "https://registry.npmjs.org/source-map/-/source-map-0.6.1.tgz",
-            "version": "0.6.1"
-        },
         "node_modules/spdx-correct": {
             "dependencies": {
                 "spdx-expression-parse": "^3.0.0",
                 "spdx-license-ids": "^3.0.0"
             },
             "dev": true,
             "integrity": "sha512-cOYcUWwhCuHCXi49RhFRCyJEK3iPj1Ziz9DpViV3tbZOwXD49QzIN3MpOLJNxh2qwq2lJJZaKMVw9qNi4jTC0w==",
@@ -8601,140 +8724,158 @@
             "version": "0.1.0"
         },
         "node_modules/stylelint": {
             "bin": {
                 "stylelint": "bin/stylelint.js"
             },
             "dependencies": {
-                "@csstools/selector-specificity": "^2.0.2",
+                "@csstools/css-parser-algorithms": "^2.1.1",
+                "@csstools/css-tokenizer": "^2.1.1",
+                "@csstools/media-query-list-parser": "^2.0.4",
+                "@csstools/selector-specificity": "^2.2.0",
                 "balanced-match": "^2.0.0",
                 "colord": "^2.9.3",
-                "cosmiconfig": "^7.1.0",
+                "cosmiconfig": "^8.1.3",
                 "css-functions-list": "^3.1.0",
+                "css-tree": "^2.3.1",
                 "debug": "^4.3.4",
                 "fast-glob": "^3.2.12",
                 "fastest-levenshtein": "^1.0.16",
                 "file-entry-cache": "^6.0.1",
                 "global-modules": "^2.0.0",
                 "globby": "^11.1.0",
                 "globjoin": "^0.1.4",
-                "html-tags": "^3.2.0",
-                "ignore": "^5.2.1",
+                "html-tags": "^3.3.1",
+                "ignore": "^5.2.4",
                 "import-lazy": "^4.0.0",
                 "imurmurhash": "^0.1.4",
                 "is-plain-object": "^5.0.0",
-                "known-css-properties": "^0.26.0",
+                "known-css-properties": "^0.27.0",
                 "mathml-tag-names": "^2.1.3",
                 "meow": "^9.0.0",
                 "micromatch": "^4.0.5",
                 "normalize-path": "^3.0.0",
                 "picocolors": "^1.0.0",
-                "postcss": "^8.4.19",
+                "postcss": "^8.4.22",
                 "postcss-media-query-parser": "^0.2.3",
                 "postcss-resolve-nested-selector": "^0.1.1",
                 "postcss-safe-parser": "^6.0.0",
                 "postcss-selector-parser": "^6.0.11",
                 "postcss-value-parser": "^4.2.0",
                 "resolve-from": "^5.0.0",
                 "string-width": "^4.2.3",
                 "strip-ansi": "^6.0.1",
                 "style-search": "^0.1.0",
-                "supports-hyperlinks": "^2.3.0",
+                "supports-hyperlinks": "^3.0.0",
                 "svg-tags": "^1.0.0",
                 "table": "^6.8.1",
                 "v8-compile-cache": "^2.3.0",
-                "write-file-atomic": "^4.0.2"
+                "write-file-atomic": "^5.0.0"
             },
             "dev": true,
             "engines": {
-                "node": "^12.20.0 || ^14.13.1 || >=16.0.0"
+                "node": "^14.13.1 || >=16.0.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/stylelint"
             },
-            "integrity": "sha512-ErlzR/T3hhbV+a925/gbfc3f3Fep9/bnspMiJPorfGEmcBbXdS+oo6LrVtoUZ/w9fqD6o6k7PtUlCOsCRdjX/A==",
-            "resolved": "https://registry.npmjs.org/stylelint/-/stylelint-14.16.1.tgz",
-            "version": "14.16.1"
+            "integrity": "sha512-Cqzpc8tvJm77KaM8qUbhpJ/UYK55Ia0whQXj4b9IId9dlPICO7J8Lyo15SZWiHxKjlvy3p5FQor/3n6i8ignXg==",
+            "resolved": "https://registry.npmjs.org/stylelint/-/stylelint-15.6.0.tgz",
+            "version": "15.6.0"
         },
         "node_modules/stylelint-config-recommended": {
             "dev": true,
-            "integrity": "sha512-9YQSrJq4NvvRuTbzDsWX3rrFOzOlYBmZP+o513BJN/yfEmGSr0AxdvrWs0P/ilSpVV/wisamAHu5XSk8Rcf4CQ==",
+            "integrity": "sha512-x6x8QNARrGO2sG6iURkzqL+Dp+4bJorPMMRNPScdvaUK8PsynriOcMW7AFDKqkWAS5wbue/u8fUT/4ynzcmqdQ==",
             "peerDependencies": {
-                "stylelint": "^14.10.0"
+                "stylelint": "^15.5.0"
             },
-            "resolved": "https://registry.npmjs.org/stylelint-config-recommended/-/stylelint-config-recommended-9.0.0.tgz",
-            "version": "9.0.0"
+            "resolved": "https://registry.npmjs.org/stylelint-config-recommended/-/stylelint-config-recommended-12.0.0.tgz",
+            "version": "12.0.0"
         },
         "node_modules/stylelint-config-recommended-scss": {
             "dependencies": {
-                "postcss-scss": "^4.0.2",
-                "stylelint-config-recommended": "^9.0.0",
-                "stylelint-scss": "^4.0.0"
+                "postcss-scss": "^4.0.6",
+                "stylelint-config-recommended": "^12.0.0",
+                "stylelint-scss": "^4.6.0"
             },
             "dev": true,
-            "integrity": "sha512-BxjxEzRaZoQb7Iinc3p92GS6zRdRAkIuEu2ZFLTxJK2e1AIcCb5B5MXY9KOXdGTnYFZ+KKx6R4Fv9zU6CtMYPQ==",
+            "integrity": "sha512-EDghTDU7aOv2LTsRZvcT1w8mcjUaMhuy+t38iV5I/0Qiu6ixdkRwhLEMul3K/fnB2v9Nwqvb3xpvJfPH+HduDw==",
             "peerDependencies": {
                 "postcss": "^8.3.3",
-                "stylelint": "^14.10.0"
+                "stylelint": "^15.5.0"
             },
             "peerDependenciesMeta": {
                 "postcss": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/stylelint-config-recommended-scss/-/stylelint-config-recommended-scss-8.0.0.tgz",
-            "version": "8.0.0"
+            "resolved": "https://registry.npmjs.org/stylelint-config-recommended-scss/-/stylelint-config-recommended-scss-11.0.0.tgz",
+            "version": "11.0.0"
+        },
+        "node_modules/stylelint-config-recommended-scss/node_modules/stylelint-scss": {
+            "dependencies": {
+                "postcss-media-query-parser": "^0.2.3",
+                "postcss-resolve-nested-selector": "^0.1.1",
+                "postcss-selector-parser": "^6.0.11",
+                "postcss-value-parser": "^4.2.0"
+            },
+            "dev": true,
+            "integrity": "sha512-TSUgIeS0H3jqDZnby1UO1Qv3poi1N8wUYIJY6D1tuUq2MN3lwp/rITVo0wD+1SWTmRm0tNmGO0b7nKInnqF6Hg==",
+            "peerDependencies": {
+                "stylelint": "^14.5.1 || ^15.0.0"
+            },
+            "resolved": "https://registry.npmjs.org/stylelint-scss/-/stylelint-scss-4.7.0.tgz",
+            "version": "4.7.0"
         },
         "node_modules/stylelint-config-standard": {
             "dependencies": {
-                "stylelint-config-recommended": "^9.0.0"
+                "stylelint-config-recommended": "^12.0.0"
             },
             "dev": true,
-            "integrity": "sha512-uy8tZLbfq6ZrXy4JKu3W+7lYLgRQBxYTUUB88vPgQ+ZzAxdrvcaSUW9hOMNLYBnwH+9Kkj19M2DHdZ4gKwI7tg==",
+            "integrity": "sha512-eyxnLWoXImUn77+ODIuW9qXBDNM+ALN68L3wT1lN2oNspZ7D9NVGlNHb2QCUn4xDug6VZLsh0tF8NyoYzkgTzg==",
             "peerDependencies": {
-                "stylelint": "^14.14.0"
+                "stylelint": "^15.5.0"
             },
-            "resolved": "https://registry.npmjs.org/stylelint-config-standard/-/stylelint-config-standard-29.0.0.tgz",
-            "version": "29.0.0"
+            "resolved": "https://registry.npmjs.org/stylelint-config-standard/-/stylelint-config-standard-33.0.0.tgz",
+            "version": "33.0.0"
         },
         "node_modules/stylelint-config-standard-scss": {
             "dependencies": {
-                "stylelint-config-recommended-scss": "^8.0.0",
-                "stylelint-config-standard": "^29.0.0"
+                "stylelint-config-recommended-scss": "^11.0.0",
+                "stylelint-config-standard": "^33.0.0"
             },
             "dev": true,
-            "integrity": "sha512-iZ2B5kQT2G3rUzx+437cEpdcnFOQkwnwqXuY8Z0QUwIHQVE8mnYChGAquyKFUKZRZ0pRnrciARlPaR1RBtPb0Q==",
+            "integrity": "sha512-yPKpJsrZn4ybuQZx/DkEHuCjw7pJginErE/47dFhCnrvD48IJ4UYec8tSiCuJWMA3HRjbIa3nh5ZeSauDGuVAg==",
             "peerDependencies": {
                 "postcss": "^8.3.3",
-                "stylelint": "^14.14.0"
+                "stylelint": "^15.5.0"
             },
             "peerDependenciesMeta": {
                 "postcss": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/stylelint-config-standard-scss/-/stylelint-config-standard-scss-6.1.0.tgz",
-            "version": "6.1.0"
+            "resolved": "https://registry.npmjs.org/stylelint-config-standard-scss/-/stylelint-config-standard-scss-9.0.0.tgz",
+            "version": "9.0.0"
         },
         "node_modules/stylelint-scss": {
             "dependencies": {
-                "lodash": "^4.17.21",
                 "postcss-media-query-parser": "^0.2.3",
                 "postcss-resolve-nested-selector": "^0.1.1",
-                "postcss-selector-parser": "^6.0.6",
-                "postcss-value-parser": "^4.1.0"
+                "postcss-selector-parser": "^6.0.11",
+                "postcss-value-parser": "^4.2.0"
             },
             "dev": true,
-            "integrity": "sha512-Qy66a+/30aylFhPmUArHhVsHOun1qrO93LGT15uzLuLjWS7hKDfpFm34mYo1ndR4MCo8W4bEZM1+AlJRJORaaw==",
+            "integrity": "sha512-5Ee5kG3JIcP2jk2PMoFMiNmW/815V+wK5o37X5ke90ihWMpPXI9iyqeA6zEWipWSRXeQc0kqbd7hKqiR+wPKNA==",
             "peerDependencies": {
                 "stylelint": "^14.5.1 || ^15.0.0"
             },
-            "resolved": "https://registry.npmjs.org/stylelint-scss/-/stylelint-scss-4.4.0.tgz",
-            "version": "4.4.0"
+            "resolved": "https://registry.npmjs.org/stylelint-scss/-/stylelint-scss-5.0.0.tgz",
+            "version": "5.0.0"
         },
         "node_modules/stylelint/node_modules/braces": {
             "dependencies": {
                 "fill-range": "^7.0.1"
             },
             "dev": true,
             "engines": {
@@ -8840,19 +8981,19 @@
         "node_modules/supports-hyperlinks": {
             "dependencies": {
                 "has-flag": "^4.0.0",
                 "supports-color": "^7.0.0"
             },
             "dev": true,
             "engines": {
-                "node": ">=8"
+                "node": ">=14.18"
             },
-            "integrity": "sha512-RpsAZlpWcDwOPQA22aCH4J0t7L8JmAvsCxfOSEwm7cQs3LshN36QaTkwd70DnBOXDWGssw2eUoc8CaRWT0XunA==",
-            "resolved": "https://registry.npmjs.org/supports-hyperlinks/-/supports-hyperlinks-2.3.0.tgz",
-            "version": "2.3.0"
+            "integrity": "sha512-QBDPHyPQDRTy9ku4URNGY5Lah8PAaXs6tAAwp55sL5WCsSW7GIfdf6W5ixfziW+t7wh3GVvHyHHyQ1ESsoRvaA==",
+            "resolved": "https://registry.npmjs.org/supports-hyperlinks/-/supports-hyperlinks-3.0.0.tgz",
+            "version": "3.0.0"
         },
         "node_modules/supports-hyperlinks/node_modules/has-flag": {
             "dev": true,
             "engines": {
                 "node": ">=8"
             },
             "integrity": "sha512-EykJT/Q1KjTWctppgIAgfSO0tKVuZUjhgMr17kqTumMl6Afv3EISleU7qZUzoXDFTAHTDC4NOoG/ZxU3EvlMPQ==",
@@ -8924,60 +9065,51 @@
                 "commander": "^2.20.0",
                 "source-map-support": "~0.5.20"
             },
             "dev": true,
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-oL0rGeM/WFQCUd0y2QrWxYnq7tfSuKBiqTjRPWrRgB46WD/kiwHwF8T23z78H6Q6kGCuuHcPB+KULHRdxvVGQA==",
-            "resolved": "https://registry.npmjs.org/terser/-/terser-5.14.2.tgz",
-            "version": "5.14.2"
+            "integrity": "sha512-hVl35zClmpisy6oaoKALOpS0rDYLxRFLHhRuDlEGTKey9qHjS1w9GMORjuwIMt70Wan4lwsLYyWDVnWgF+KUEw==",
+            "resolved": "https://registry.npmjs.org/terser/-/terser-5.17.1.tgz",
+            "version": "5.17.1"
         },
         "node_modules/terser-webpack-plugin": {
             "dependencies": {
+                "@jridgewell/trace-mapping": "^0.3.17",
                 "jest-worker": "^27.4.5",
                 "schema-utils": "^3.1.1",
-                "serialize-javascript": "^6.0.0",
-                "source-map": "^0.6.1",
-                "terser": "^5.7.2"
+                "serialize-javascript": "^6.0.1",
+                "terser": "^5.16.5"
             },
             "dev": true,
             "engines": {
                 "node": ">= 10.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-GvlZdT6wPQKbDNW/GDQzZFg/j4vKU96yl2q6mcUkzKOgW4gwf1Z8cZToUCrz31XHlPWH8MVb1r2tFtdDtTGJ7g==",
+            "integrity": "sha512-AfKwIktyP7Cu50xNjXF/6Qb5lBNzYaWpU6YfoX3uZicTx0zTy0stDDCsvjDapKsSDvOeWo5MEq4TmdBy2cNoHw==",
             "peerDependencies": {
                 "webpack": "^5.1.0"
             },
             "peerDependenciesMeta": {
                 "@swc/core": {
                     "optional": true
                 },
                 "esbuild": {
                     "optional": true
                 },
                 "uglify-js": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/terser-webpack-plugin/-/terser-webpack-plugin-5.3.1.tgz",
-            "version": "5.3.1"
-        },
-        "node_modules/terser-webpack-plugin/node_modules/source-map": {
-            "dev": true,
-            "engines": {
-                "node": ">=0.10.0"
-            },
-            "integrity": "sha512-UjgapumWlbMhkBgzT7Ykc5YXUT46F0iKu8SGXq0bcwP5dz/h0Plj6enJqjz1Zbq2l5WaqYnrVbwWOWMyF3F47g==",
-            "resolved": "https://registry.npmjs.org/source-map/-/source-map-0.6.1.tgz",
-            "version": "0.6.1"
+            "resolved": "https://registry.npmjs.org/terser-webpack-plugin/-/terser-webpack-plugin-5.3.7.tgz",
+            "version": "5.3.7"
         },
         "node_modules/terser/node_modules/commander": {
             "dev": true,
             "integrity": "sha512-GpVkmM8vF2vQUkj2LvZmD35JxeJOLCwJ9cUkugyk2nuhbv3+mJvpLYYt+0+USMxE+oj+ey/lJEnhZw75x/OMcQ==",
             "resolved": "https://registry.npmjs.org/commander/-/commander-2.20.3.tgz",
             "version": "2.20.3"
         },
@@ -9062,20 +9194,20 @@
                     "url": "https://opencollective.com/browserslist"
                 },
                 {
                     "type": "tidelift",
                     "url": "https://tidelift.com/funding/github/npm/browserslist"
                 }
             ],
-            "integrity": "sha512-/xsqn21EGVdXI3EXSum1Yckj3ZVZugqyOZQ/CxYPBD/R+ko9NSUScf8tFF4dOKY+2pvSSJA/S+5B8s4Zr4kyvg==",
+            "integrity": "sha512-OztqDenkfFkbSG+tRxBeAnCVPckDBcvibKd35yDONx6OU8N7sqgwc7rCbkJ/WcYtVRZ4ba68d6byhC21GFh7sQ==",
             "peerDependencies": {
                 "browserslist": ">= 4.21.0"
             },
-            "resolved": "https://registry.npmjs.org/update-browserslist-db/-/update-browserslist-db-1.0.9.tgz",
-            "version": "1.0.9"
+            "resolved": "https://registry.npmjs.org/update-browserslist-db/-/update-browserslist-db-1.0.10.tgz",
+            "version": "1.0.10"
         },
         "node_modules/uri-js": {
             "dependencies": {
                 "punycode": "^2.1.0"
             },
             "dev": true,
             "integrity": "sha512-7rKUyy33Q1yc98pQ1DAmLtwX109F7TIfWlW1Ydo8Wl1ii1SeHieeh0HHfPeL2fMXK6z0s8ecKs9frCuLJvndBg==",
@@ -9119,66 +9251,66 @@
         },
         "node_modules/webpack": {
             "bin": {
                 "webpack": "bin/webpack.js"
             },
             "dependencies": {
                 "@types/eslint-scope": "^3.7.3",
-                "@types/estree": "^0.0.51",
-                "@webassemblyjs/ast": "1.11.1",
-                "@webassemblyjs/wasm-edit": "1.11.1",
-                "@webassemblyjs/wasm-parser": "1.11.1",
+                "@types/estree": "^1.0.0",
+                "@webassemblyjs/ast": "^1.11.5",
+                "@webassemblyjs/wasm-edit": "^1.11.5",
+                "@webassemblyjs/wasm-parser": "^1.11.5",
                 "acorn": "^8.7.1",
                 "acorn-import-assertions": "^1.7.6",
                 "browserslist": "^4.14.5",
                 "chrome-trace-event": "^1.0.2",
-                "enhanced-resolve": "^5.10.0",
-                "es-module-lexer": "^0.9.0",
+                "enhanced-resolve": "^5.13.0",
+                "es-module-lexer": "^1.2.1",
                 "eslint-scope": "5.1.1",
                 "events": "^3.2.0",
                 "glob-to-regexp": "^0.4.1",
                 "graceful-fs": "^4.2.9",
                 "json-parse-even-better-errors": "^2.3.1",
                 "loader-runner": "^4.2.0",
                 "mime-types": "^2.1.27",
                 "neo-async": "^2.6.2",
-                "schema-utils": "^3.1.0",
+                "schema-utils": "^3.1.2",
                 "tapable": "^2.1.1",
-                "terser-webpack-plugin": "^5.1.3",
+                "terser-webpack-plugin": "^5.3.7",
                 "watchpack": "^2.4.0",
                 "webpack-sources": "^3.2.3"
             },
             "dev": true,
             "engines": {
                 "node": ">=10.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-l5sOdYBDunyf72HW8dF23rFtWq/7Zgvt/9ftMof71E/yUb1YLOBmTgA2K4vQthB3kotMrSj609txVE0dnr2fjA==",
+            "integrity": "sha512-AAjaJ9S4hYCVODKLQTgG5p5e11hiMawBwV2v8MYLE0C/6UAGLuAF4n1qa9GOwdxnicaP+5k6M5HrLmD4+gIB8Q==",
             "peerDependenciesMeta": {
                 "webpack-cli": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/webpack/-/webpack-5.76.0.tgz",
-            "version": "5.76.0"
+            "resolved": "https://registry.npmjs.org/webpack/-/webpack-5.81.0.tgz",
+            "version": "5.81.0"
         },
         "node_modules/webpack-cli": {
             "bin": {
                 "webpack-cli": "bin/cli.js"
             },
             "dependencies": {
                 "@discoveryjs/json-ext": "^0.5.0",
-                "@webpack-cli/configtest": "^2.0.1",
+                "@webpack-cli/configtest": "^2.1.0",
                 "@webpack-cli/info": "^2.0.1",
-                "@webpack-cli/serve": "^2.0.1",
+                "@webpack-cli/serve": "^2.0.4",
                 "colorette": "^2.0.14",
-                "commander": "^9.4.1",
+                "commander": "^10.0.1",
                 "cross-spawn": "^7.0.3",
                 "envinfo": "^7.7.3",
                 "fastest-levenshtein": "^1.0.12",
                 "import-local": "^3.0.2",
                 "interpret": "^3.1.1",
                 "rechoir": "^0.8.0",
                 "webpack-merge": "^5.7.3"
@@ -9187,31 +9319,31 @@
             "engines": {
                 "node": ">=14.15.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-S3KVAyfwUqr0Mo/ur3NzIp6jnerNpo7GUO6so51mxLi1spqsA17YcMXy0WOIJtBSnj748lthxC6XLbNKh/ZC+A==",
+            "integrity": "sha512-OLJwVMoXnXYH2ncNGU8gxVpUtm3ybvdioiTvHgUyBuyMLKiVvWy+QObzBsMtp5pH7qQoEuWgeEUQ/sU3ZJFzAw==",
             "peerDependencies": {
                 "webpack": "5.x.x"
             },
             "peerDependenciesMeta": {
                 "@webpack-cli/generators": {
                     "optional": true
                 },
                 "webpack-bundle-analyzer": {
                     "optional": true
                 },
                 "webpack-dev-server": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/webpack-cli/-/webpack-cli-5.0.1.tgz",
-            "version": "5.0.1"
+            "resolved": "https://registry.npmjs.org/webpack-cli/-/webpack-cli-5.1.1.tgz",
+            "version": "5.1.1"
         },
         "node_modules/webpack-merge": {
             "dependencies": {
                 "clone-deep": "^4.0.1",
                 "wildcard": "^2.0.0"
             },
             "dev": true,
@@ -9283,19 +9415,19 @@
         "node_modules/write-file-atomic": {
             "dependencies": {
                 "imurmurhash": "^0.1.4",
                 "signal-exit": "^3.0.7"
             },
             "dev": true,
             "engines": {
-                "node": "^12.13.0 || ^14.15.0 || >=16.0.0"
+                "node": "^14.17.0 || ^16.13.0 || >=18.0.0"
             },
-            "integrity": "sha512-7KxauUdBmSdWnmpaGFg+ppNjKF8uNLry8LyzjauQDOVONfFLNKrKvQOxZ/VuTIcS/gge/YNahf5RIIQWTSarlg==",
-            "resolved": "https://registry.npmjs.org/write-file-atomic/-/write-file-atomic-4.0.2.tgz",
-            "version": "4.0.2"
+            "integrity": "sha512-R7NYMnHSlV42K54lwY9lvW6MnSm1HSJqZL3xiSgi9E7//FYaI74r2G0rd+/X6VAMkHEdzxQaU5HUOXWUz5kA/w==",
+            "resolved": "https://registry.npmjs.org/write-file-atomic/-/write-file-atomic-5.0.0.tgz",
+            "version": "5.0.0"
         },
         "node_modules/xdg-basedir": {
             "dev": true,
             "engines": {
                 "node": ">=8"
             },
             "integrity": "sha512-PSNhEJDejZYV7h50BohL09Er9VaIefr2LMAf3OEmpCkjOi34eYyQYAXUTjEQtZJTKcF0E2UKTh+osDLsgNim9Q==",
@@ -9304,23 +9436,14 @@
         },
         "node_modules/yallist": {
             "dev": true,
             "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
             "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
             "version": "4.0.0"
         },
-        "node_modules/yaml": {
-            "dev": true,
-            "engines": {
-                "node": ">= 6"
-            },
-            "integrity": "sha512-r3vXyErRCYJ7wg28yvBY5VSoAF8ZvlcW9/BwUzEtUsjvX/DKs24dIkuwjtuprwJJHsbyUbLApepYTR1BN4uHrg==",
-            "resolved": "https://registry.npmjs.org/yaml/-/yaml-1.10.2.tgz",
-            "version": "1.10.2"
-        },
         "node_modules/yargs-parser": {
             "dev": true,
             "engines": {
                 "node": ">=10"
             },
             "integrity": "sha512-y11nGElTIV+CT3Zv9t7VKl+Q3hTQoT9a1Qzezhhl6Rp21gJ/IVTW7Z3y9EWXhuUBC2Shnf+DX0antecpAwSP8w==",
             "resolved": "https://registry.npmjs.org/yargs-parser/-/yargs-parser-20.2.9.tgz",
```

### Comparing `django-hijack-3.3.0/package.json` & `django-hijack-3.4.0/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9807692307692308%*

 * *Differences: {"'devDependencies'": "{'autoprefixer': '^10.4.14', 'mini-css-extract-plugin': '^2.7.5', "*

 * *                      "'postcss-loader': '^7.3.0', 'sass': '^1.62.1', 'sass-loader': '^13.2.2', "*

 * *                      "'stylelint': '^15.6.0', 'stylelint-config-standard-scss': '^9.0.0', "*

 * *                      "'stylelint-scss': '^5.0.0', 'webpack': '^5.81.0', 'webpack-cli': '^5.1.1'}"}*

```diff
@@ -1,26 +1,26 @@
 {
     "author": "Johannes Maron",
     "bugs": {
         "url": "https://github.com/django-hijack/django-hijack/issues"
     },
     "devDependencies": {
-        "autoprefixer": "^10.4.13",
+        "autoprefixer": "^10.4.14",
         "css-loader": "^6.7.3",
-        "mini-css-extract-plugin": "^2.7.2",
+        "mini-css-extract-plugin": "^2.7.5",
         "postcss": "^8.4.21",
-        "postcss-loader": "^7.0.2",
-        "sass": "^1.58.3",
-        "sass-loader": "^13.2.0",
+        "postcss-loader": "^7.3.0",
+        "sass": "^1.62.1",
+        "sass-loader": "^13.2.2",
         "standard": "^17.0.0",
-        "stylelint": "^14.16.1",
-        "stylelint-config-standard-scss": "^6.1.0",
-        "stylelint-scss": "^4.4.0",
-        "webpack": "^5.76.0",
-        "webpack-cli": "^5.0.1"
+        "stylelint": "^15.6.0",
+        "stylelint-config-standard-scss": "^9.0.0",
+        "stylelint-scss": "^5.0.0",
+        "webpack": "^5.81.0",
+        "webpack-cli": "^5.1.1"
     },
     "homepage": "https://github.com/django-hijack/django-hijack#readme",
     "license": "MIT",
     "name": "django-hijack",
     "repository": {
         "type": "git",
         "url": "git+https://github.com/django-hijack/django-hijack.git"
```

### Comparing `django-hijack-3.3.0/setup.cfg` & `django-hijack-3.4.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 author = arteria GmbH
 author_email = admin@arteria.ch
 description = django-hijack allows superusers to hijack (=login as) and work on behalf of another user.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/django-hijack/django-hijack
 license = MIT
-license_file = LICENSE
+license_files = LICENSE
 platforms = 
 	OS Independent
 keywords = 
 	django
 	hijack
 	support
 	customer support
```

### Comparing `django-hijack-3.3.0/webpack.config.js` & `django-hijack-3.4.0/webpack.config.js`

 * *Files identical despite different names*

