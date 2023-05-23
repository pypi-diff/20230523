# Comparing `tmp/djangoldp_tzcld-1.0.8.tar.gz` & `tmp/djangoldp_tzcld-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_tzcld-1.0.8.tar", last modified: Tue May 16 10:54:50 2023, max compression
+gzip compressed data, was "dist/djangoldp_tzcld-1.0.9.tar", last modified: Tue May 16 17:54:04 2023, max compression
```

## Comparing `djangoldp_tzcld-1.0.8.tar` & `djangoldp_tzcld-1.0.9.tar`

### file list

```diff
@@ -1,47 +1,71 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:54:50.000000 djangoldp_tzcld-1.0.8/
--rw-rw-rw-   0 root         (0) root         (0)       65 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/setup.py
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      559 2023-05-16 10:54:50.000000 djangoldp_tzcld-1.0.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:54:50.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld.egg-info/
--rw-r--r--   0 root         (0) root         (0)      309 2023-05-16 10:54:50.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 10:54:50.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1801 2023-05-16 10:54:50.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-16 10:54:50.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-16 10:54:50.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      309 2023-05-16 10:54:50.000000 djangoldp_tzcld-1.0.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:54:50.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/
--rw-rw-rw-   0 root         (0) root         (0)    18337 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1085 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/permissions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:54:50.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:54:50.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/templates/django_registration/
--rw-rw-rw-   0 root         (0) root         (0)     3189 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/templates/django_registration/registration_form.html
--rw-rw-rw-   0 root         (0) root         (0)     2347 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/admin.py
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-16 10:54:48.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/settings.py
--rw-rw-rw-   0 root         (0) root         (0)       96 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/djangoldp_settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:54:50.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     5896 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0004_tzcldprofilejob_tzcldprofilejobemail_tzcldprofilejobphone.py
--rw-rw-rw-   0 root         (0) root         (0)      836 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0007_auto_20230327_1451.py
--rw-rw-rw-   0 root         (0) root         (0)     9812 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      889 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0013_auto_20230330_1246.py
--rw-rw-rw-   0 root         (0) root         (0)     1889 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0016_tzcldcontactmember.py
--rw-rw-rw-   0 root         (0) root         (0)      501 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0014_auto_20230330_1258.py
--rw-rw-rw-   0 root         (0) root         (0)     1099 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0019_auto_20230414_1634.py
--rw-rw-rw-   0 root         (0) root         (0)      960 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0021_auto_20230510_1232.py
--rw-rw-rw-   0 root         (0) root         (0)      431 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0002_tzcldcommunity_contact_job.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1033 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0012_auto_20230330_1233.py
--rw-rw-rw-   0 root         (0) root         (0)     1774 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0003_auto_20220720_1242.py
--rw-rw-rw-   0 root         (0) root         (0)    18022 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0006_auto_20230327_1449.py
--rw-rw-rw-   0 root         (0) root         (0)      652 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0005_auto_20230325_1335.py
--rw-rw-rw-   0 root         (0) root         (0)     4403 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0011_auto_20230328_1045.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0018_auto_20230406_1755.py
--rw-rw-rw-   0 root         (0) root         (0)      459 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0022_tzcldcommunity_membership_organisation_name.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0017_tzcldcontactmember_community.py
--rw-rw-rw-   0 root         (0) root         (0)     1816 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0015_auto_20230330_1439.py
--rw-rw-rw-   0 root         (0) root         (0)      653 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0010_auto_20230327_1629.py
--rw-rw-rw-   0 root         (0) root         (0)     1750 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0020_auto_20230417_1242.py
--rw-rw-rw-   0 root         (0) root         (0)     1270 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0009_auto_20230327_1623.py
--rw-rw-rw-   0 root         (0) root         (0)      711 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0008_auto_20230327_1602.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:54:03.000000 djangoldp_tzcld-1.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)       65 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-05-16 17:54:03.000000 djangoldp_tzcld-1.0.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:54:03.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      309 2023-05-16 17:54:03.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 17:54:03.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     3176 2023-05-16 17:54:03.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-16 17:54:03.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-16 17:54:03.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      309 2023-05-16 17:54:03.000000 djangoldp_tzcld-1.0.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:54:03.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/
+-rw-rw-rw-   0 root         (0) root         (0)    18337 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/permissions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:54:03.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:54:03.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/templates/registration/
+-rw-rw-rw-   0 root         (0) root         (0)      349 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/templates/registration/password_reset_done.html
+-rw-rw-rw-   0 root         (0) root         (0)     2088 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/templates/registration/password_change_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     2333 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/templates/registration/password_reset_email.html
+-rw-rw-rw-   0 root         (0) root         (0)     1970 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/templates/registration/password_reset_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      650 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/templates/registration/activation_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)     1290 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/templates/registration/password_reset_form.html
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/templates/registration/registration_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      538 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/templates/registration/password_reset_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)      497 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/templates/registration/lost_user.html
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/templates/registration/activate.html
+-rw-rw-rw-   0 root         (0) root         (0)      459 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/templates/registration/password_reset_email.txt
+-rw-rw-rw-   0 root         (0) root         (0)      489 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/templates/registration/logged_out.html
+-rw-rw-rw-   0 root         (0) root         (0)      545 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/templates/registration/registration_closed.html
+-rw-rw-rw-   0 root         (0) root         (0)      482 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/templates/registration/logout.html
+-rw-rw-rw-   0 root         (0) root         (0)     4167 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/templates/registration/login.html
+-rw-rw-rw-   0 root         (0) root         (0)      500 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/templates/registration/password_change_done.html
+-rw-rw-rw-   0 root         (0) root         (0)      297 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/templates/registration/registration_complete.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:54:03.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/templates/admin/
+-rw-rw-rw-   0 root         (0) root         (0)     2458 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/templates/admin/login.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:54:03.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/templates/django_registration/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/templates/django_registration/activation_email_subject.txt
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/templates/django_registration/activation_email_body.txt
+-rw-rw-rw-   0 root         (0) root         (0)      668 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/templates/django_registration/activation_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)     3470 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/templates/django_registration/registration_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      399 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/templates/django_registration/registration_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)     2347 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-16 17:54:01.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)       96 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/djangoldp_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:54:03.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     5896 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0004_tzcldprofilejob_tzcldprofilejobemail_tzcldprofilejobphone.py
+-rw-rw-rw-   0 root         (0) root         (0)      836 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0007_auto_20230327_1451.py
+-rw-rw-rw-   0 root         (0) root         (0)     9812 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      889 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0013_auto_20230330_1246.py
+-rw-rw-rw-   0 root         (0) root         (0)     1889 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0016_tzcldcontactmember.py
+-rw-rw-rw-   0 root         (0) root         (0)      501 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0014_auto_20230330_1258.py
+-rw-rw-rw-   0 root         (0) root         (0)     1099 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0019_auto_20230414_1634.py
+-rw-rw-rw-   0 root         (0) root         (0)      960 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0021_auto_20230510_1232.py
+-rw-rw-rw-   0 root         (0) root         (0)      431 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0002_tzcldcommunity_contact_job.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1033 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0012_auto_20230330_1233.py
+-rw-rw-rw-   0 root         (0) root         (0)     1774 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0003_auto_20220720_1242.py
+-rw-rw-rw-   0 root         (0) root         (0)    18022 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0006_auto_20230327_1449.py
+-rw-rw-rw-   0 root         (0) root         (0)      652 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0005_auto_20230325_1335.py
+-rw-rw-rw-   0 root         (0) root         (0)     4403 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0011_auto_20230328_1045.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0018_auto_20230406_1755.py
+-rw-rw-rw-   0 root         (0) root         (0)      459 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0022_tzcldcommunity_membership_organisation_name.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0017_tzcldcontactmember_community.py
+-rw-rw-rw-   0 root         (0) root         (0)     1816 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0015_auto_20230330_1439.py
+-rw-rw-rw-   0 root         (0) root         (0)      653 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0010_auto_20230327_1629.py
+-rw-rw-rw-   0 root         (0) root         (0)     1750 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0020_auto_20230417_1242.py
+-rw-rw-rw-   0 root         (0) root         (0)     1270 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0009_auto_20230327_1623.py
+-rw-rw-rw-   0 root         (0) root         (0)      711 2023-05-16 17:53:46.000000 djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0008_auto_20230327_1602.py
```

### Comparing `djangoldp_tzcld-1.0.8/setup.cfg` & `djangoldp_tzcld-1.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.8/djangoldp_tzcld/models.py` & `djangoldp_tzcld-1.0.9/djangoldp_tzcld/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.8/djangoldp_tzcld/permissions.py` & `djangoldp_tzcld-1.0.9/djangoldp_tzcld/permissions.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.8/djangoldp_tzcld/templates/django_registration/registration_form.html` & `djangoldp_tzcld-1.0.9/djangoldp_tzcld/templates/django_registration/registration_form.html`

 * *Files 5% similar despite different names*

```diff
@@ -28,16 +28,19 @@
       <span class="text-bold" style="color: red; text-transform: lowercase;">
         {{ form.last_name.errors }}
       </span>
     </div>
     <div
       class="segment margin-bottom-medium full padding-right-small sm-padding-none text-small text-semibold text-uppercase text-color-heading"
     >
-      <label for="id_username">{% trans "Nom d'utilisateur:" %}</label>
+      <label for="id_username">{% trans "Nom d'utilisateur·rice:" %}</label>
       {{ form.username }}
+      <p class="text-color-primary" style="text-transform: initial; white-space: initial;">
+        C'est le nom qui s'affichera pour votre profil sur la Plateforme, nous vous invitons à le choisir selon l'un de ces formats : PrénomNom, Prénom-Nom, Prénom_Nom
+      </p>
       <span class="text-bold" style="color: red; text-transform: lowercase;">
         {{ form.username.errors }}
       </span>
     </div>
     <div
       class="segment margin-bottom-medium full padding-right-small sm-padding-none text-small text-semibold text-uppercase text-color-heading"
     >
```

### Comparing `djangoldp_tzcld-1.0.8/djangoldp_tzcld/admin.py` & `djangoldp_tzcld-1.0.9/djangoldp_tzcld/admin.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0004_tzcldprofilejob_tzcldprofilejobemail_tzcldprofilejobphone.py` & `djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0004_tzcldprofilejob_tzcldprofilejobemail_tzcldprofilejobphone.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0007_auto_20230327_1451.py` & `djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0007_auto_20230327_1451.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0001_initial.py` & `djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0013_auto_20230330_1246.py` & `djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0013_auto_20230330_1246.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0016_tzcldcontactmember.py` & `djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0016_tzcldcontactmember.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0019_auto_20230414_1634.py` & `djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0019_auto_20230414_1634.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0021_auto_20230510_1232.py` & `djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0021_auto_20230510_1232.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0012_auto_20230330_1233.py` & `djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0012_auto_20230330_1233.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0003_auto_20220720_1242.py` & `djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0003_auto_20220720_1242.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0006_auto_20230327_1449.py` & `djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0006_auto_20230327_1449.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0005_auto_20230325_1335.py` & `djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0005_auto_20230325_1335.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0011_auto_20230328_1045.py` & `djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0011_auto_20230328_1045.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0018_auto_20230406_1755.py` & `djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0018_auto_20230406_1755.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0017_tzcldcontactmember_community.py` & `djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0017_tzcldcontactmember_community.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0015_auto_20230330_1439.py` & `djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0015_auto_20230330_1439.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0010_auto_20230327_1629.py` & `djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0010_auto_20230327_1629.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0020_auto_20230417_1242.py` & `djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0020_auto_20230417_1242.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0009_auto_20230327_1623.py` & `djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0009_auto_20230327_1623.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0008_auto_20230327_1602.py` & `djangoldp_tzcld-1.0.9/djangoldp_tzcld/migrations/0008_auto_20230327_1602.py`

 * *Files identical despite different names*

