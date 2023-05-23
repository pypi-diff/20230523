# Comparing `tmp/django-oasis4-auth-1.0.9.tar.gz` & `tmp/django-oasis4-auth-1.0.9b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-oasis4-auth-1.0.9.tar", last modified: Sat Mar 18 15:01:42 2023, max compression
+gzip compressed data, was "django-oasis4-auth-1.0.9b0.tar", last modified: Thu Mar 16 19:27:28 2023, max compression
```

## Comparing `django-oasis4-auth-1.0.9.tar` & `django-oasis4-auth-1.0.9b0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 15:01:42.948891 django-oasis4-auth-1.0.9/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    11375 2023-01-23 20:26:24.000000 django-oasis4-auth-1.0.9/LICENSE
--rw-rw-r--   0 macercha  (1000) macercha  (1000)       93 2023-01-18 12:21:52.000000 django-oasis4-auth-1.0.9/MANIFEST.in
--rw-r--r--   0 macercha  (1000) macercha  (1000)    22688 2023-03-18 15:01:42.947891 django-oasis4-auth-1.0.9/PKG-INFO
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     9810 2023-02-15 19:15:25.000000 django-oasis4-auth-1.0.9/README.md
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 15:01:42.942891 django-oasis4-auth-1.0.9/django_oasis4_auth.egg-info/
--rw-r--r--   0 macercha  (1000) macercha  (1000)    22688 2023-03-18 15:01:42.000000 django-oasis4-auth-1.0.9/django_oasis4_auth.egg-info/PKG-INFO
--rw-r--r--   0 macercha  (1000) macercha  (1000)     1413 2023-03-18 15:01:42.000000 django-oasis4-auth-1.0.9/django_oasis4_auth.egg-info/SOURCES.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2023-03-18 15:01:42.000000 django-oasis4-auth-1.0.9/django_oasis4_auth.egg-info/dependency_links.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)       67 2023-03-18 15:01:42.000000 django-oasis4-auth-1.0.9/django_oasis4_auth.egg-info/requires.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)       11 2023-03-18 15:01:42.000000 django-oasis4-auth-1.0.9/django_oasis4_auth.egg-info/top_level.txt
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 15:01:42.942891 django-oasis4-auth-1.0.9/oasis_auth/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-20 02:22:34.000000 django-oasis4-auth-1.0.9/oasis_auth/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 15:01:42.943891 django-oasis4-auth-1.0.9/oasis_auth/api/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      507 2023-01-07 20:01:29.000000 django-oasis4-auth-1.0.9/oasis_auth/api/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 15:01:42.943891 django-oasis4-auth-1.0.9/oasis_auth/api/serializers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      578 2023-01-27 22:32:38.000000 django-oasis4-auth-1.0.9/oasis_auth/api/serializers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      786 2023-01-27 22:44:36.000000 django-oasis4-auth-1.0.9/oasis_auth/api/serializers/user.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 15:01:42.943891 django-oasis4-auth-1.0.9/oasis_auth/api/services/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      590 2023-01-18 03:44:01.000000 django-oasis4-auth-1.0.9/oasis_auth/api/services/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    16006 2023-03-16 16:26:19.000000 django-oasis4-auth-1.0.9/oasis_auth/api/services/oasis_auth.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1090 2023-03-16 14:42:57.000000 django-oasis4-auth-1.0.9/oasis_auth/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 15:01:42.943891 django-oasis4-auth-1.0.9/oasis_auth/lib/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      509 2022-12-20 17:00:22.000000 django-oasis4-auth-1.0.9/oasis_auth/lib/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 15:01:42.944891 django-oasis4-auth-1.0.9/oasis_auth/lib/managers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      580 2023-01-18 20:29:06.000000 django-oasis4-auth-1.0.9/oasis_auth/lib/managers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2368 2023-03-16 14:42:57.000000 django-oasis4-auth-1.0.9/oasis_auth/lib/managers/user_profile.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 15:01:42.944891 django-oasis4-auth-1.0.9/oasis_auth/lib/utils/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      627 2023-01-18 15:44:17.000000 django-oasis4-auth-1.0.9/oasis_auth/lib/utils/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2944 2023-03-16 14:42:57.000000 django-oasis4-auth-1.0.9/oasis_auth/lib/utils/auth_actions.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2207 2023-03-16 14:42:57.000000 django-oasis4-auth-1.0.9/oasis_auth/lib/utils/send_code.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 15:01:42.939891 django-oasis4-auth-1.0.9/oasis_auth/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 15:01:42.940891 django-oasis4-auth-1.0.9/oasis_auth/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 15:01:42.945891 django-oasis4-auth-1.0.9/oasis_auth/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     4792 2023-03-16 16:15:08.000000 django-oasis4-auth-1.0.9/oasis_auth/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     7121 2023-03-16 16:14:53.000000 django-oasis4-auth-1.0.9/oasis_auth/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 15:01:42.946890 django-oasis4-auth-1.0.9/oasis_auth/migrations/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2055 2023-01-18 02:10:57.000000 django-oasis4-auth-1.0.9/oasis_auth/migrations/0001_initial.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      438 2023-01-18 20:03:48.000000 django-oasis4-auth-1.0.9/oasis_auth/migrations/0002_remove_userprofile_first_name_and_more.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      598 2023-03-01 16:07:21.000000 django-oasis4-auth-1.0.9/oasis_auth/migrations/0003_userprofile_quota_userprofile_segment.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      354 2023-03-01 16:22:58.000000 django-oasis4-auth-1.0.9/oasis_auth/migrations/0004_remove_userprofile_quota.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)        0 2023-01-18 02:10:57.000000 django-oasis4-auth-1.0.9/oasis_auth/migrations/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2222 2023-03-16 14:42:57.000000 django-oasis4-auth-1.0.9/oasis_auth/models.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 15:01:42.946890 django-oasis4-auth-1.0.9/oasis_auth/tasks/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      581 2023-02-15 14:18:51.000000 django-oasis4-auth-1.0.9/oasis_auth/tasks/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2211 2023-03-01 16:31:30.000000 django-oasis4-auth-1.0.9/oasis_auth/tasks/sync_users.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 15:01:42.947891 django-oasis4-auth-1.0.9/oasis_auth/templates/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      742 2022-12-22 15:55:10.000000 django-oasis4-auth-1.0.9/oasis_auth/templates/default.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-02 19:51:33.000000 django-oasis4-auth-1.0.9/oasis_auth/templates/default.txt
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      742 2022-12-22 15:55:10.000000 django-oasis4-auth-1.0.9/oasis_auth/templates/login.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-01 21:00:33.000000 django-oasis4-auth-1.0.9/oasis_auth/templates/login.txt
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      745 2023-01-18 04:44:01.000000 django-oasis4-auth-1.0.9/oasis_auth/templates/register.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      509 2023-03-01 21:00:33.000000 django-oasis4-auth-1.0.9/oasis_auth/templates/register.txt
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      634 2023-03-16 14:42:57.000000 django-oasis4-auth-1.0.9/oasis_auth/templates/retrieve_password.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      405 2023-03-16 14:42:57.000000 django-oasis4-auth-1.0.9/oasis_auth/templates/retrieve_password.txt
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1151 2023-03-16 14:42:57.000000 django-oasis4-auth-1.0.9/oasis_auth/urls.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      857 2023-03-18 14:49:02.000000 django-oasis4-auth-1.0.9/pyproject.toml
--rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2023-03-18 15:01:42.948891 django-oasis4-auth-1.0.9/setup.cfg
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 19:27:28.095507 django-oasis4-auth-1.0.9b0/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    11375 2023-01-23 20:26:24.000000 django-oasis4-auth-1.0.9b0/LICENSE
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)       93 2023-01-18 12:21:52.000000 django-oasis4-auth-1.0.9b0/MANIFEST.in
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    22677 2023-03-16 19:27:28.095507 django-oasis4-auth-1.0.9b0/PKG-INFO
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     9810 2023-02-15 19:15:25.000000 django-oasis4-auth-1.0.9b0/README.md
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 19:27:28.088507 django-oasis4-auth-1.0.9b0/django_oasis4_auth.egg-info/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    22677 2023-03-16 19:27:28.000000 django-oasis4-auth-1.0.9b0/django_oasis4_auth.egg-info/PKG-INFO
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     1413 2023-03-16 19:27:28.000000 django-oasis4-auth-1.0.9b0/django_oasis4_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2023-03-16 19:27:28.000000 django-oasis4-auth-1.0.9b0/django_oasis4_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       67 2023-03-16 19:27:28.000000 django-oasis4-auth-1.0.9b0/django_oasis4_auth.egg-info/requires.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       11 2023-03-16 19:27:28.000000 django-oasis4-auth-1.0.9b0/django_oasis4_auth.egg-info/top_level.txt
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 19:27:28.088507 django-oasis4-auth-1.0.9b0/oasis_auth/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-20 02:22:34.000000 django-oasis4-auth-1.0.9b0/oasis_auth/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 19:27:28.089506 django-oasis4-auth-1.0.9b0/oasis_auth/api/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      507 2023-01-07 20:01:29.000000 django-oasis4-auth-1.0.9b0/oasis_auth/api/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 19:27:28.089506 django-oasis4-auth-1.0.9b0/oasis_auth/api/serializers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      578 2023-01-27 22:32:38.000000 django-oasis4-auth-1.0.9b0/oasis_auth/api/serializers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      786 2023-01-27 22:44:36.000000 django-oasis4-auth-1.0.9b0/oasis_auth/api/serializers/user.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 19:27:28.089506 django-oasis4-auth-1.0.9b0/oasis_auth/api/services/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      590 2023-01-18 03:44:01.000000 django-oasis4-auth-1.0.9b0/oasis_auth/api/services/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    16006 2023-03-16 16:26:19.000000 django-oasis4-auth-1.0.9b0/oasis_auth/api/services/oasis_auth.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1090 2023-03-16 14:42:57.000000 django-oasis4-auth-1.0.9b0/oasis_auth/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 19:27:28.090507 django-oasis4-auth-1.0.9b0/oasis_auth/lib/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      509 2022-12-20 17:00:22.000000 django-oasis4-auth-1.0.9b0/oasis_auth/lib/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 19:27:28.090507 django-oasis4-auth-1.0.9b0/oasis_auth/lib/managers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      580 2023-01-18 20:29:06.000000 django-oasis4-auth-1.0.9b0/oasis_auth/lib/managers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2368 2023-03-16 14:42:57.000000 django-oasis4-auth-1.0.9b0/oasis_auth/lib/managers/user_profile.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 19:27:28.091507 django-oasis4-auth-1.0.9b0/oasis_auth/lib/utils/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      627 2023-01-18 15:44:17.000000 django-oasis4-auth-1.0.9b0/oasis_auth/lib/utils/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2944 2023-03-16 14:42:57.000000 django-oasis4-auth-1.0.9b0/oasis_auth/lib/utils/auth_actions.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2207 2023-03-16 14:42:57.000000 django-oasis4-auth-1.0.9b0/oasis_auth/lib/utils/send_code.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 19:27:28.086507 django-oasis4-auth-1.0.9b0/oasis_auth/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 19:27:28.086507 django-oasis4-auth-1.0.9b0/oasis_auth/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 19:27:28.091507 django-oasis4-auth-1.0.9b0/oasis_auth/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     4792 2023-03-16 16:15:08.000000 django-oasis4-auth-1.0.9b0/oasis_auth/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     7121 2023-03-16 16:14:53.000000 django-oasis4-auth-1.0.9b0/oasis_auth/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 19:27:28.092507 django-oasis4-auth-1.0.9b0/oasis_auth/migrations/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2055 2023-01-18 02:10:57.000000 django-oasis4-auth-1.0.9b0/oasis_auth/migrations/0001_initial.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      438 2023-01-18 20:03:48.000000 django-oasis4-auth-1.0.9b0/oasis_auth/migrations/0002_remove_userprofile_first_name_and_more.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      598 2023-03-01 16:07:21.000000 django-oasis4-auth-1.0.9b0/oasis_auth/migrations/0003_userprofile_quota_userprofile_segment.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      354 2023-03-01 16:22:58.000000 django-oasis4-auth-1.0.9b0/oasis_auth/migrations/0004_remove_userprofile_quota.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)        0 2023-01-18 02:10:57.000000 django-oasis4-auth-1.0.9b0/oasis_auth/migrations/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2222 2023-03-16 14:42:57.000000 django-oasis4-auth-1.0.9b0/oasis_auth/models.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 19:27:28.093506 django-oasis4-auth-1.0.9b0/oasis_auth/tasks/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      581 2023-02-15 14:18:51.000000 django-oasis4-auth-1.0.9b0/oasis_auth/tasks/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2211 2023-03-01 16:31:30.000000 django-oasis4-auth-1.0.9b0/oasis_auth/tasks/sync_users.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 19:27:28.094506 django-oasis4-auth-1.0.9b0/oasis_auth/templates/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      742 2022-12-22 15:55:10.000000 django-oasis4-auth-1.0.9b0/oasis_auth/templates/default.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-02 19:51:33.000000 django-oasis4-auth-1.0.9b0/oasis_auth/templates/default.txt
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      742 2022-12-22 15:55:10.000000 django-oasis4-auth-1.0.9b0/oasis_auth/templates/login.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-03-01 21:00:33.000000 django-oasis4-auth-1.0.9b0/oasis_auth/templates/login.txt
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      745 2023-01-18 04:44:01.000000 django-oasis4-auth-1.0.9b0/oasis_auth/templates/register.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      509 2023-03-01 21:00:33.000000 django-oasis4-auth-1.0.9b0/oasis_auth/templates/register.txt
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      634 2023-03-16 14:42:57.000000 django-oasis4-auth-1.0.9b0/oasis_auth/templates/retrieve_password.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      405 2023-03-16 14:42:57.000000 django-oasis4-auth-1.0.9b0/oasis_auth/templates/retrieve_password.txt
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1151 2023-03-16 14:42:57.000000 django-oasis4-auth-1.0.9b0/oasis_auth/urls.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      851 2023-03-16 19:26:27.000000 django-oasis4-auth-1.0.9b0/pyproject.toml
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2023-03-16 19:27:28.095507 django-oasis4-auth-1.0.9b0/setup.cfg
```

### Comparing `django-oasis4-auth-1.0.9/LICENSE` & `django-oasis4-auth-1.0.9b0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9/PKG-INFO` & `django-oasis4-auth-1.0.9b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oasis4-auth
-Version: 1.0.9
+Version: 1.0.9b0
 Summary: Oasis 4 Authorization System for django
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                                     CQ INVERSIONES S.A.S.
                                       CONTRATO DE LICENCIA DE SOFTWARE
                                                     NO OEM
                                              (Version 2.0 - 2023)
         
@@ -110,15 +110,15 @@
         IDIOMA; TRADUCCIONES. En el caso de que la versión en español de este Contrato esté acompañada por cualquier otra
         versión traducida a otro idioma, dicha versión traducida sólo se ofrece a título informativo y prevalecerá la versión
         en español.
         
 Keywords: django,OASIS4
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.1
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `django-oasis4-auth-1.0.9/README.md` & `django-oasis4-auth-1.0.9b0/README.md`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9/django_oasis4_auth.egg-info/PKG-INFO` & `django-oasis4-auth-1.0.9b0/django_oasis4_auth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oasis4-auth
-Version: 1.0.9
+Version: 1.0.9b0
 Summary: Oasis 4 Authorization System for django
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                                     CQ INVERSIONES S.A.S.
                                       CONTRATO DE LICENCIA DE SOFTWARE
                                                     NO OEM
                                              (Version 2.0 - 2023)
         
@@ -110,15 +110,15 @@
         IDIOMA; TRADUCCIONES. En el caso de que la versión en español de este Contrato esté acompañada por cualquier otra
         versión traducida a otro idioma, dicha versión traducida sólo se ofrece a título informativo y prevalecerá la versión
         en español.
         
 Keywords: django,OASIS4
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.1
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `django-oasis4-auth-1.0.9/django_oasis4_auth.egg-info/SOURCES.txt` & `django-oasis4-auth-1.0.9b0/django_oasis4_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9/oasis_auth/api/serializers/__init__.py` & `django-oasis4-auth-1.0.9b0/oasis_auth/api/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9/oasis_auth/api/serializers/user.py` & `django-oasis4-auth-1.0.9b0/oasis_auth/api/serializers/user.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9/oasis_auth/api/services/__init__.py` & `django-oasis4-auth-1.0.9b0/oasis_auth/api/services/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9/oasis_auth/api/services/oasis_auth.py` & `django-oasis4-auth-1.0.9b0/oasis_auth/api/services/oasis_auth.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9/oasis_auth/apps.py` & `django-oasis4-auth-1.0.9b0/oasis_auth/apps.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9/oasis_auth/lib/managers/__init__.py` & `django-oasis4-auth-1.0.9b0/oasis_auth/lib/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9/oasis_auth/lib/managers/user_profile.py` & `django-oasis4-auth-1.0.9b0/oasis_auth/lib/managers/user_profile.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9/oasis_auth/lib/utils/__init__.py` & `django-oasis4-auth-1.0.9b0/oasis_auth/lib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9/oasis_auth/lib/utils/auth_actions.py` & `django-oasis4-auth-1.0.9b0/oasis_auth/lib/utils/auth_actions.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9/oasis_auth/lib/utils/send_code.py` & `django-oasis4-auth-1.0.9b0/oasis_auth/lib/utils/send_code.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9/oasis_auth/locale/es/LC_MESSAGES/django.mo` & `django-oasis4-auth-1.0.9b0/oasis_auth/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9/oasis_auth/locale/es/LC_MESSAGES/django.po` & `django-oasis4-auth-1.0.9b0/oasis_auth/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9/oasis_auth/migrations/0001_initial.py` & `django-oasis4-auth-1.0.9b0/oasis_auth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9/oasis_auth/migrations/0003_userprofile_quota_userprofile_segment.py` & `django-oasis4-auth-1.0.9b0/oasis_auth/migrations/0003_userprofile_quota_userprofile_segment.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9/oasis_auth/models.py` & `django-oasis4-auth-1.0.9b0/oasis_auth/models.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9/oasis_auth/tasks/__init__.py` & `django-oasis4-auth-1.0.9b0/oasis_auth/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9/oasis_auth/tasks/sync_users.py` & `django-oasis4-auth-1.0.9b0/oasis_auth/tasks/sync_users.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9/oasis_auth/templates/default.html` & `django-oasis4-auth-1.0.9b0/oasis_auth/templates/default.html`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9/oasis_auth/templates/login.html` & `django-oasis4-auth-1.0.9b0/oasis_auth/templates/login.html`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9/oasis_auth/templates/register.html` & `django-oasis4-auth-1.0.9b0/oasis_auth/templates/register.html`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9/oasis_auth/templates/retrieve_password.html` & `django-oasis4-auth-1.0.9b0/oasis_auth/templates/retrieve_password.html`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9/oasis_auth/urls.py` & `django-oasis4-auth-1.0.9b0/oasis_auth/urls.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-auth-1.0.9/pyproject.toml` & `django-oasis4-auth-1.0.9b0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,26 +3,26 @@
     "setuptools>=42",
     "wheel",
 ]
 build-backend="setuptools.build_meta"
 
 [project]
 name = "django-oasis4-auth"
-version = "1.0.9"
+version = "1.0.9-beta.0"
 authors = [
     {name="Mario Cerón", email="mario.ceron@cqinversiones.co"}
 ]
 description = "Oasis 4 Authorization System for django"
 readme = "README.md"
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     "License :: Other/Proprietary License",
     "Programming Language :: Python :: 3.9",
-    "Development Status :: 5 - Production/Stable",
+    "Development Status :: 4 - Beta",
     "Framework :: Django",
     "Framework :: Django :: 4.1",
     "Environment :: Web Environment",
     "Operating System :: OS Independent",
     "Topic :: Internet :: WWW/HTTP"
 ]
 dependencies = [
```

