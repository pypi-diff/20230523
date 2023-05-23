# Comparing `tmp/mercury-2.2.9.tar.gz` & `tmp/mercury-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercury-2.2.9.tar", last modified: Fri Apr 28 10:32:36 2023, max compression
+gzip compressed data, was "mercury-2.3.0.tar", last modified: Tue May 23 13:30:21 2023, max compression
```

## Comparing `mercury-2.2.9.tar` & `mercury-2.3.0.tar`

### file list

```diff
@@ -1,211 +1,212 @@
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-28 10:32:36.372500 mercury-2.2.9/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      149 2022-04-19 12:37:24.000000 mercury-2.2.9/MANIFEST.in
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5674 2023-04-28 10:32:36.372500 mercury-2.2.9/PKG-INFO
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4214 2023-02-15 10:26:45.000000 mercury-2.2.9/README.md
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-28 10:32:36.360500 mercury-2.2.9/mercury/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       54 2023-04-28 10:31:42.000000 mercury-2.2.9/mercury/__init__.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-28 10:32:36.360500 mercury-2.2.9/mercury/apps/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.9/mercury/apps/__init__.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-28 10:32:36.360500 mercury-2.2.9/mercury/apps/accounts/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-01 11:11:00.000000 mercury-2.2.9/mercury/apps/accounts/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      459 2023-03-17 11:37:23.000000 mercury-2.2.9/mercury/apps/accounts/admin.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      153 2023-03-01 11:11:00.000000 mercury-2.2.9/mercury/apps/accounts/apps.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      801 2023-03-01 11:11:00.000000 mercury-2.2.9/mercury/apps/accounts/fields.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-28 10:32:36.360500 mercury-2.2.9/mercury/apps/accounts/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     9132 2023-03-29 09:06:05.000000 mercury-2.2.9/mercury/apps/accounts/migrations/0001_initial.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-01 11:11:00.000000 mercury-2.2.9/mercury/apps/accounts/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4715 2023-03-28 08:49:03.000000 mercury-2.2.9/mercury/apps/accounts/models.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2086 2023-04-06 13:33:42.000000 mercury-2.2.9/mercury/apps/accounts/serializers.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2937 2023-03-27 12:26:01.000000 mercury-2.2.9/mercury/apps/accounts/tasks.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-28 10:32:36.360500 mercury-2.2.9/mercury/apps/accounts/tests/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-16 13:27:44.000000 mercury-2.2.9/mercury/apps/accounts/tests/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     7289 2023-03-29 09:06:05.000000 mercury-2.2.9/mercury/apps/accounts/tests/test_accounts.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5543 2023-03-31 10:36:11.000000 mercury-2.2.9/mercury/apps/accounts/tests/test_invitations.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6078 2023-04-06 13:49:54.000000 mercury-2.2.9/mercury/apps/accounts/tests/test_secrets.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    11402 2023-03-31 10:52:58.000000 mercury-2.2.9/mercury/apps/accounts/tests/test_sites.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3426 2023-03-29 09:06:05.000000 mercury-2.2.9/mercury/apps/accounts/tests/test_subscription.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2645 2023-04-25 12:36:08.000000 mercury-2.2.9/mercury/apps/accounts/urls.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-28 10:32:36.360500 mercury-2.2.9/mercury/apps/accounts/views/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-17 08:20:29.000000 mercury-2.2.9/mercury/apps/accounts/views/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2006 2023-03-27 08:34:35.000000 mercury-2.2.9/mercury/apps/accounts/views/accounts.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4308 2023-03-31 10:36:11.000000 mercury-2.2.9/mercury/apps/accounts/views/invitations.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      789 2023-03-24 08:45:58.000000 mercury-2.2.9/mercury/apps/accounts/views/permissions.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2922 2023-04-06 14:49:43.000000 mercury-2.2.9/mercury/apps/accounts/views/secrets.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6576 2023-04-27 14:55:46.000000 mercury-2.2.9/mercury/apps/accounts/views/sites.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4152 2023-03-29 09:06:05.000000 mercury-2.2.9/mercury/apps/accounts/views/subscription.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      436 2023-03-24 08:45:58.000000 mercury-2.2.9/mercury/apps/accounts/views/utils.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-28 10:32:36.360500 mercury-2.2.9/mercury/apps/nb/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.9/mercury/apps/nb/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5845 2023-04-06 13:49:54.000000 mercury-2.2.9/mercury/apps/nb/exporter.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4086 2023-04-06 13:49:54.000000 mercury-2.2.9/mercury/apps/nb/nbrun.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-28 10:32:36.360500 mercury-2.2.9/mercury/apps/nb/tests/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-04-05 08:19:32.000000 mercury-2.2.9/mercury/apps/nb/tests/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      854 2023-04-06 13:49:54.000000 mercury-2.2.9/mercury/apps/nb/tests/test_nbrun.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1265 2023-03-17 12:41:34.000000 mercury-2.2.9/mercury/apps/nb/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      403 2023-02-13 14:05:12.000000 mercury-2.2.9/mercury/apps/nb/utils.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-28 10:32:36.360500 mercury-2.2.9/mercury/apps/nbworker/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.9/mercury/apps/nbworker/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1950 2023-04-27 15:29:23.000000 mercury-2.2.9/mercury/apps/nbworker/__main__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    17411 2023-04-12 08:48:16.000000 mercury-2.2.9/mercury/apps/nbworker/nb.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     7485 2023-04-06 14:49:56.000000 mercury-2.2.9/mercury/apps/nbworker/rest.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4864 2023-03-17 08:55:41.000000 mercury-2.2.9/mercury/apps/nbworker/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      701 2023-03-14 07:49:44.000000 mercury-2.2.9/mercury/apps/nbworker/utils.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2927 2023-04-20 13:08:01.000000 mercury-2.2.9/mercury/apps/nbworker/ws.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-28 10:32:36.360500 mercury-2.2.9/mercury/apps/notebooks/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.9/mercury/apps/notebooks/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      277 2022-03-09 11:04:20.000000 mercury-2.2.9/mercury/apps/notebooks/admin.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      155 2022-03-09 11:04:20.000000 mercury-2.2.9/mercury/apps/notebooks/apps.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-28 10:32:36.360500 mercury-2.2.9/mercury/apps/notebooks/management/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.9/mercury/apps/notebooks/management/__init__.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-28 10:32:36.360500 mercury-2.2.9/mercury/apps/notebooks/management/commands/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.9/mercury/apps/notebooks/management/commands/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1279 2022-03-09 11:06:47.000000 mercury-2.2.9/mercury/apps/notebooks/management/commands/add.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      864 2022-03-09 11:06:47.000000 mercury-2.2.9/mercury/apps/notebooks/management/commands/delete.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      545 2022-03-09 11:06:47.000000 mercury-2.2.9/mercury/apps/notebooks/management/commands/list.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3702 2023-02-13 14:05:12.000000 mercury-2.2.9/mercury/apps/notebooks/management/commands/watch.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-28 10:32:36.360500 mercury-2.2.9/mercury/apps/notebooks/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2300 2023-03-29 09:06:05.000000 mercury-2.2.9/mercury/apps/notebooks/migrations/0001_initial.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.9/mercury/apps/notebooks/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1067 2023-03-27 08:29:11.000000 mercury-2.2.9/mercury/apps/notebooks/models.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      617 2023-03-17 11:38:01.000000 mercury-2.2.9/mercury/apps/notebooks/serializers.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4093 2022-05-18 10:19:32.000000 mercury-2.2.9/mercury/apps/notebooks/slides_themes.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    11689 2023-04-03 14:44:43.000000 mercury-2.2.9/mercury/apps/notebooks/tasks.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2023-03-01 11:11:00.000000 mercury-2.2.9/mercury/apps/notebooks/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      582 2023-04-25 12:40:05.000000 mercury-2.2.9/mercury/apps/notebooks/urls.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3798 2023-04-27 15:18:53.000000 mercury-2.2.9/mercury/apps/notebooks/views.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-28 10:32:36.364500 mercury-2.2.9/mercury/apps/storage/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.9/mercury/apps/storage/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       63 2023-02-13 14:05:12.000000 mercury-2.2.9/mercury/apps/storage/admin.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      151 2023-02-13 14:05:12.000000 mercury-2.2.9/mercury/apps/storage/apps.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-28 10:32:36.364500 mercury-2.2.9/mercury/apps/storage/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2949 2023-03-29 09:06:05.000000 mercury-2.2.9/mercury/apps/storage/migrations/0001_initial.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1404 2023-03-31 09:54:03.000000 mercury-2.2.9/mercury/apps/storage/migrations/0002_useruploadedfile.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.9/mercury/apps/storage/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1787 2023-03-29 09:06:05.000000 mercury-2.2.9/mercury/apps/storage/models.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3540 2023-03-31 09:54:03.000000 mercury-2.2.9/mercury/apps/storage/s3utils.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      469 2023-03-31 14:19:15.000000 mercury-2.2.9/mercury/apps/storage/serializers.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    11397 2023-03-31 09:54:03.000000 mercury-2.2.9/mercury/apps/storage/storage.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3158 2023-03-17 08:55:41.000000 mercury-2.2.9/mercury/apps/storage/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2132 2023-03-29 09:56:45.000000 mercury-2.2.9/mercury/apps/storage/urls.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      445 2023-03-31 09:54:03.000000 mercury-2.2.9/mercury/apps/storage/utils.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-28 10:32:36.364500 mercury-2.2.9/mercury/apps/storage/views/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-31 12:45:08.000000 mercury-2.2.9/mercury/apps/storage/views/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6182 2023-03-31 11:42:07.000000 mercury-2.2.9/mercury/apps/storage/views/dashboardfiles.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4935 2023-03-31 11:42:07.000000 mercury-2.2.9/mercury/apps/storage/views/notebookfiles.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3737 2023-03-31 11:42:07.000000 mercury-2.2.9/mercury/apps/storage/views/workerfiles.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-28 10:32:36.364500 mercury-2.2.9/mercury/apps/tasks/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.9/mercury/apps/tasks/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      287 2022-03-09 11:04:20.000000 mercury-2.2.9/mercury/apps/tasks/admin.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      153 2022-03-09 11:04:20.000000 mercury-2.2.9/mercury/apps/tasks/apps.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      412 2022-03-09 11:06:47.000000 mercury-2.2.9/mercury/apps/tasks/clean_service.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3840 2023-04-03 14:18:32.000000 mercury-2.2.9/mercury/apps/tasks/export_pdf.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3805 2023-04-06 13:49:54.000000 mercury-2.2.9/mercury/apps/tasks/export_png.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-28 10:32:36.364500 mercury-2.2.9/mercury/apps/tasks/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1328 2023-03-29 09:06:05.000000 mercury-2.2.9/mercury/apps/tasks/migrations/0001_initial.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.2.9/mercury/apps/tasks/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      762 2022-05-18 10:19:32.000000 mercury-2.2.9/mercury/apps/tasks/models.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3659 2023-02-13 14:05:12.000000 mercury-2.2.9/mercury/apps/tasks/notify.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      433 2022-03-09 11:06:47.000000 mercury-2.2.9/mercury/apps/tasks/serializers.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    15223 2023-02-23 14:52:12.000000 mercury-2.2.9/mercury/apps/tasks/tasks.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1314 2023-02-13 14:05:12.000000 mercury-2.2.9/mercury/apps/tasks/tasks_export.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      571 2023-03-14 07:49:44.000000 mercury-2.2.9/mercury/apps/tasks/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1431 2023-04-25 12:37:36.000000 mercury-2.2.9/mercury/apps/tasks/urls.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     8619 2023-03-17 08:55:41.000000 mercury-2.2.9/mercury/apps/tasks/views.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-28 10:32:36.364500 mercury-2.2.9/mercury/apps/workers/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-14 07:49:44.000000 mercury-2.2.9/mercury/apps/workers/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       63 2023-03-14 07:49:44.000000 mercury-2.2.9/mercury/apps/workers/admin.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      151 2023-03-14 07:49:44.000000 mercury-2.2.9/mercury/apps/workers/apps.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-28 10:32:36.364500 mercury-2.2.9/mercury/apps/workers/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1286 2023-03-29 09:06:05.000000 mercury-2.2.9/mercury/apps/workers/migrations/0001_initial.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-14 07:49:44.000000 mercury-2.2.9/mercury/apps/workers/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      798 2023-03-29 09:06:05.000000 mercury-2.2.9/mercury/apps/workers/models.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      296 2023-03-14 07:49:44.000000 mercury-2.2.9/mercury/apps/workers/serializers.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       60 2023-03-14 07:49:44.000000 mercury-2.2.9/mercury/apps/workers/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1076 2023-04-25 12:37:59.000000 mercury-2.2.9/mercury/apps/workers/urls.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3881 2023-03-31 09:54:03.000000 mercury-2.2.9/mercury/apps/workers/views.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-28 10:32:36.364500 mercury-2.2.9/mercury/apps/ws/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.9/mercury/apps/ws/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      141 2023-02-13 14:05:12.000000 mercury-2.2.9/mercury/apps/ws/apps.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6162 2023-04-20 13:43:38.000000 mercury-2.2.9/mercury/apps/ws/client.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      947 2023-03-14 07:49:44.000000 mercury-2.2.9/mercury/apps/ws/middleware.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-28 10:32:36.364500 mercury-2.2.9/mercury/apps/ws/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.9/mercury/apps/ws/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      386 2023-02-28 13:59:46.000000 mercury-2.2.9/mercury/apps/ws/routing.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2495 2023-04-06 13:49:54.000000 mercury-2.2.9/mercury/apps/ws/tasks.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      137 2023-03-01 11:07:38.000000 mercury-2.2.9/mercury/apps/ws/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5106 2023-04-06 13:49:54.000000 mercury-2.2.9/mercury/apps/ws/utils.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1754 2023-03-14 07:49:44.000000 mercury-2.2.9/mercury/apps/ws/worker.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     7191 2023-03-31 14:11:10.000000 mercury-2.2.9/mercury/demo.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-28 10:32:36.364500 mercury-2.2.9/mercury/frontend-dist/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1158 2023-04-28 10:32:35.000000 mercury-2.2.9/mercury/frontend-dist/asset-manifest.json
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    15406 2023-04-28 10:32:20.000000 mercury-2.2.9/mercury/frontend-dist/favicon-old.ico
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    15086 2023-04-28 10:32:20.000000 mercury-2.2.9/mercury/frontend-dist/favicon.ico
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3086 2023-04-28 10:32:35.000000 mercury-2.2.9/mercury/frontend-dist/index.html
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    17406 2023-04-28 10:32:20.000000 mercury-2.2.9/mercury/frontend-dist/jupyter-additional.css
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4539 2023-04-28 10:32:20.000000 mercury-2.2.9/mercury/frontend-dist/jupyter-syntax.css
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   580386 2023-04-28 10:32:20.000000 mercury-2.2.9/mercury/frontend-dist/jupyter-theme-light.css
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      324 2023-04-28 10:32:20.000000 mercury-2.2.9/mercury/frontend-dist/manifest.json
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6237 2023-04-28 10:32:20.000000 mercury-2.2.9/mercury/frontend-dist/mercury_black_logo.svg
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6997 2023-04-28 10:32:20.000000 mercury-2.2.9/mercury/frontend-dist/mercury_logo.svg
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       67 2023-04-28 10:32:20.000000 mercury-2.2.9/mercury/frontend-dist/robots.txt
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-28 10:32:36.360500 mercury-2.2.9/mercury/frontend-dist/static/
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-28 10:32:36.364500 mercury-2.2.9/mercury/frontend-dist/static/css/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   229115 2023-04-28 10:32:35.000000 mercury-2.2.9/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   612316 2023-04-28 10:32:35.000000 mercury-2.2.9/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css.map
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2831 2023-04-28 10:32:35.000000 mercury-2.2.9/mercury/frontend-dist/static/css/main.26f96620.chunk.css
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5260 2023-04-28 10:32:35.000000 mercury-2.2.9/mercury/frontend-dist/static/css/main.26f96620.chunk.css.map
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-28 10:32:36.372500 mercury-2.2.9/mercury/frontend-dist/static/js/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)  1311795 2023-04-28 10:32:35.000000 mercury-2.2.9/mercury/frontend-dist/static/js/2.6305b467.chunk.js
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3383 2023-04-28 10:32:35.000000 mercury-2.2.9/mercury/frontend-dist/static/js/2.6305b467.chunk.js.LICENSE.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)  4973509 2023-04-28 10:32:35.000000 mercury-2.2.9/mercury/frontend-dist/static/js/2.6305b467.chunk.js.map
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    85854 2023-04-28 10:32:35.000000 mercury-2.2.9/mercury/frontend-dist/static/js/main.f9a369a0.chunk.js
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   262205 2023-04-28 10:32:35.000000 mercury-2.2.9/mercury/frontend-dist/static/js/main.f9a369a0.chunk.js.map
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1557 2023-04-28 10:32:35.000000 mercury-2.2.9/mercury/frontend-dist/static/js/runtime-main.248907bc.js
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     8276 2023-04-28 10:32:35.000000 mercury-2.2.9/mercury/frontend-dist/static/js/runtime-main.248907bc.js.map
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-28 10:32:36.372500 mercury-2.2.9/mercury/frontend-dist/static/media/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   165548 2023-04-28 10:32:35.000000 mercury-2.2.9/mercury/frontend-dist/static/media/fontawesome-webfont.1e59d233.ttf
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    77160 2023-04-28 10:32:35.000000 mercury-2.2.9/mercury/frontend-dist/static/media/fontawesome-webfont.20fd1704.woff2
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   165742 2023-04-28 10:32:35.000000 mercury-2.2.9/mercury/frontend-dist/static/media/fontawesome-webfont.8b43027f.eot
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   444379 2023-04-28 10:32:35.000000 mercury-2.2.9/mercury/frontend-dist/static/media/fontawesome-webfont.c1e38fd9.svg
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    98024 2023-04-28 10:32:35.000000 mercury-2.2.9/mercury/frontend-dist/static/media/fontawesome-webfont.f691f37e.woff
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      684 2022-03-09 11:04:20.000000 mercury-2.2.9/mercury/manage.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     8556 2023-04-27 14:42:46.000000 mercury-2.2.9/mercury/mercury.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      545 2023-04-25 12:41:47.000000 mercury-2.2.9/mercury/requirements.txt
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-28 10:32:36.372500 mercury-2.2.9/mercury/server/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       68 2022-03-09 11:04:20.000000 mercury-2.2.9/mercury/server/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      837 2023-03-14 07:49:44.000000 mercury-2.2.9/mercury/server/asgi.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2771 2023-03-24 08:43:00.000000 mercury-2.2.9/mercury/server/celery.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     9844 2023-04-05 13:16:51.000000 mercury-2.2.9/mercury/server/settings.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1575 2023-04-25 12:38:18.000000 mercury-2.2.9/mercury/server/urls.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1645 2023-03-01 12:07:40.000000 mercury-2.2.9/mercury/server/views.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      405 2022-05-18 11:03:41.000000 mercury-2.2.9/mercury/server/wsgi.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-28 10:32:36.372500 mercury-2.2.9/mercury/widgets/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.2.9/mercury/widgets/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2029 2023-03-17 11:39:55.000000 mercury-2.2.9/mercury/widgets/app.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2294 2023-04-07 10:30:37.000000 mercury-2.2.9/mercury/widgets/button.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      826 2023-04-07 10:43:02.000000 mercury-2.2.9/mercury/widgets/chat.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2127 2023-04-07 10:30:37.000000 mercury-2.2.9/mercury/widgets/checkbox.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      408 2023-04-07 10:32:14.000000 mercury-2.2.9/mercury/widgets/confetti.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3393 2023-04-07 10:30:37.000000 mercury-2.2.9/mercury/widgets/file.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4828 2023-02-21 07:28:26.000000 mercury-2.2.9/mercury/widgets/json.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6894 2023-04-07 10:30:37.000000 mercury-2.2.9/mercury/widgets/manager.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      104 2023-02-21 07:28:26.000000 mercury-2.2.9/mercury/widgets/md.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2690 2023-04-07 10:30:37.000000 mercury-2.2.9/mercury/widgets/multiselect.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1219 2023-02-21 07:48:36.000000 mercury-2.2.9/mercury/widgets/note.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3016 2023-04-07 10:30:37.000000 mercury-2.2.9/mercury/widgets/numeric.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1255 2023-02-21 07:48:36.000000 mercury-2.2.9/mercury/widgets/outputdir.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3025 2023-04-07 10:30:37.000000 mercury-2.2.9/mercury/widgets/range.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2403 2023-04-07 10:30:37.000000 mercury-2.2.9/mercury/widgets/select.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2949 2023-04-07 10:30:37.000000 mercury-2.2.9/mercury/widgets/slider.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      222 2023-02-21 07:28:26.000000 mercury-2.2.9/mercury/widgets/stop.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2039 2023-04-07 10:30:37.000000 mercury-2.2.9/mercury/widgets/text.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-04-28 10:32:36.360500 mercury-2.2.9/mercury.egg-info/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5674 2023-04-28 10:32:36.000000 mercury-2.2.9/mercury.egg-info/PKG-INFO
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6285 2023-04-28 10:32:36.000000 mercury-2.2.9/mercury.egg-info/SOURCES.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2023-04-28 10:32:36.000000 mercury-2.2.9/mercury.egg-info/dependency_links.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       50 2023-04-28 10:32:36.000000 mercury-2.2.9/mercury.egg-info/entry_points.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      489 2023-04-28 10:32:36.000000 mercury-2.2.9/mercury.egg-info/requires.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        8 2023-04-28 10:32:36.000000 mercury-2.2.9/mercury.egg-info/top_level.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      106 2022-03-09 11:04:20.000000 mercury-2.2.9/pyproject.toml
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       38 2023-04-28 10:32:36.372500 mercury-2.2.9/setup.cfg
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1163 2023-04-28 10:31:57.000000 mercury-2.2.9/setup.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-05-23 13:30:21.568417 mercury-2.3.0/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      149 2022-04-19 12:37:24.000000 mercury-2.3.0/MANIFEST.in
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6016 2023-05-23 13:30:21.568417 mercury-2.3.0/PKG-INFO
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4326 2023-05-22 10:58:50.000000 mercury-2.3.0/README.md
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-05-23 13:30:21.552417 mercury-2.3.0/mercury/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       54 2023-05-23 13:29:17.000000 mercury-2.3.0/mercury/__init__.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-05-23 13:30:21.552417 mercury-2.3.0/mercury/apps/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.3.0/mercury/apps/__init__.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-05-23 13:30:21.552417 mercury-2.3.0/mercury/apps/accounts/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-01 11:11:00.000000 mercury-2.3.0/mercury/apps/accounts/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      459 2023-03-17 11:37:23.000000 mercury-2.3.0/mercury/apps/accounts/admin.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      153 2023-03-01 11:11:00.000000 mercury-2.3.0/mercury/apps/accounts/apps.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      801 2023-03-01 11:11:00.000000 mercury-2.3.0/mercury/apps/accounts/fields.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-05-23 13:30:21.552417 mercury-2.3.0/mercury/apps/accounts/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     9132 2023-03-29 09:06:05.000000 mercury-2.3.0/mercury/apps/accounts/migrations/0001_initial.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-01 11:11:00.000000 mercury-2.3.0/mercury/apps/accounts/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4715 2023-03-28 08:49:03.000000 mercury-2.3.0/mercury/apps/accounts/models.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2086 2023-04-06 13:33:42.000000 mercury-2.3.0/mercury/apps/accounts/serializers.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2937 2023-03-27 12:26:01.000000 mercury-2.3.0/mercury/apps/accounts/tasks.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-05-23 13:30:21.552417 mercury-2.3.0/mercury/apps/accounts/tests/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-16 13:27:44.000000 mercury-2.3.0/mercury/apps/accounts/tests/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     7289 2023-03-29 09:06:05.000000 mercury-2.3.0/mercury/apps/accounts/tests/test_accounts.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5543 2023-03-31 10:36:11.000000 mercury-2.3.0/mercury/apps/accounts/tests/test_invitations.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6078 2023-04-06 13:49:54.000000 mercury-2.3.0/mercury/apps/accounts/tests/test_secrets.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    11402 2023-03-31 10:52:58.000000 mercury-2.3.0/mercury/apps/accounts/tests/test_sites.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3426 2023-03-29 09:06:05.000000 mercury-2.3.0/mercury/apps/accounts/tests/test_subscription.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2645 2023-04-25 12:36:08.000000 mercury-2.3.0/mercury/apps/accounts/urls.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-05-23 13:30:21.556417 mercury-2.3.0/mercury/apps/accounts/views/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-17 08:20:29.000000 mercury-2.3.0/mercury/apps/accounts/views/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2006 2023-03-27 08:34:35.000000 mercury-2.3.0/mercury/apps/accounts/views/accounts.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4308 2023-03-31 10:36:11.000000 mercury-2.3.0/mercury/apps/accounts/views/invitations.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      789 2023-03-24 08:45:58.000000 mercury-2.3.0/mercury/apps/accounts/views/permissions.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2922 2023-04-06 14:49:43.000000 mercury-2.3.0/mercury/apps/accounts/views/secrets.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6578 2023-05-16 15:07:21.000000 mercury-2.3.0/mercury/apps/accounts/views/sites.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4152 2023-03-29 09:06:05.000000 mercury-2.3.0/mercury/apps/accounts/views/subscription.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      436 2023-03-24 08:45:58.000000 mercury-2.3.0/mercury/apps/accounts/views/utils.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-05-23 13:30:21.556417 mercury-2.3.0/mercury/apps/nb/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.3.0/mercury/apps/nb/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5845 2023-04-06 13:49:54.000000 mercury-2.3.0/mercury/apps/nb/exporter.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4086 2023-04-06 13:49:54.000000 mercury-2.3.0/mercury/apps/nb/nbrun.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-05-23 13:30:21.556417 mercury-2.3.0/mercury/apps/nb/tests/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-04-05 08:19:32.000000 mercury-2.3.0/mercury/apps/nb/tests/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      854 2023-04-06 13:49:54.000000 mercury-2.3.0/mercury/apps/nb/tests/test_nbrun.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1265 2023-03-17 12:41:34.000000 mercury-2.3.0/mercury/apps/nb/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      403 2023-02-13 14:05:12.000000 mercury-2.3.0/mercury/apps/nb/utils.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-05-23 13:30:21.556417 mercury-2.3.0/mercury/apps/nbworker/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.3.0/mercury/apps/nbworker/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1950 2023-04-27 15:29:23.000000 mercury-2.3.0/mercury/apps/nbworker/__main__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    17411 2023-04-12 08:48:16.000000 mercury-2.3.0/mercury/apps/nbworker/nb.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     7485 2023-04-06 14:49:56.000000 mercury-2.3.0/mercury/apps/nbworker/rest.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4864 2023-03-17 08:55:41.000000 mercury-2.3.0/mercury/apps/nbworker/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      701 2023-03-14 07:49:44.000000 mercury-2.3.0/mercury/apps/nbworker/utils.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2927 2023-04-20 13:08:01.000000 mercury-2.3.0/mercury/apps/nbworker/ws.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-05-23 13:30:21.556417 mercury-2.3.0/mercury/apps/notebooks/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.3.0/mercury/apps/notebooks/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      277 2022-03-09 11:04:20.000000 mercury-2.3.0/mercury/apps/notebooks/admin.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      155 2022-03-09 11:04:20.000000 mercury-2.3.0/mercury/apps/notebooks/apps.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-05-23 13:30:21.556417 mercury-2.3.0/mercury/apps/notebooks/management/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.3.0/mercury/apps/notebooks/management/__init__.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-05-23 13:30:21.556417 mercury-2.3.0/mercury/apps/notebooks/management/commands/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.3.0/mercury/apps/notebooks/management/commands/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1279 2022-03-09 11:06:47.000000 mercury-2.3.0/mercury/apps/notebooks/management/commands/add.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      864 2022-03-09 11:06:47.000000 mercury-2.3.0/mercury/apps/notebooks/management/commands/delete.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      545 2022-03-09 11:06:47.000000 mercury-2.3.0/mercury/apps/notebooks/management/commands/list.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3702 2023-02-13 14:05:12.000000 mercury-2.3.0/mercury/apps/notebooks/management/commands/watch.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-05-23 13:30:21.556417 mercury-2.3.0/mercury/apps/notebooks/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2300 2023-03-29 09:06:05.000000 mercury-2.3.0/mercury/apps/notebooks/migrations/0001_initial.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.3.0/mercury/apps/notebooks/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1067 2023-03-27 08:29:11.000000 mercury-2.3.0/mercury/apps/notebooks/models.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      617 2023-03-17 11:38:01.000000 mercury-2.3.0/mercury/apps/notebooks/serializers.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4093 2022-05-18 10:19:32.000000 mercury-2.3.0/mercury/apps/notebooks/slides_themes.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    11852 2023-05-22 13:27:15.000000 mercury-2.3.0/mercury/apps/notebooks/tasks.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2023-03-01 11:11:00.000000 mercury-2.3.0/mercury/apps/notebooks/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      582 2023-04-25 12:40:05.000000 mercury-2.3.0/mercury/apps/notebooks/urls.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3798 2023-04-27 15:18:53.000000 mercury-2.3.0/mercury/apps/notebooks/views.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-05-23 13:30:21.556417 mercury-2.3.0/mercury/apps/storage/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.3.0/mercury/apps/storage/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       63 2023-02-13 14:05:12.000000 mercury-2.3.0/mercury/apps/storage/admin.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      151 2023-02-13 14:05:12.000000 mercury-2.3.0/mercury/apps/storage/apps.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-05-23 13:30:21.556417 mercury-2.3.0/mercury/apps/storage/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2949 2023-03-29 09:06:05.000000 mercury-2.3.0/mercury/apps/storage/migrations/0001_initial.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1404 2023-03-31 09:54:03.000000 mercury-2.3.0/mercury/apps/storage/migrations/0002_useruploadedfile.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.3.0/mercury/apps/storage/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1787 2023-03-29 09:06:05.000000 mercury-2.3.0/mercury/apps/storage/models.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3540 2023-03-31 09:54:03.000000 mercury-2.3.0/mercury/apps/storage/s3utils.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      469 2023-03-31 14:19:15.000000 mercury-2.3.0/mercury/apps/storage/serializers.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    11397 2023-05-22 12:14:16.000000 mercury-2.3.0/mercury/apps/storage/storage.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3158 2023-03-17 08:55:41.000000 mercury-2.3.0/mercury/apps/storage/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2132 2023-03-29 09:56:45.000000 mercury-2.3.0/mercury/apps/storage/urls.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      445 2023-03-31 09:54:03.000000 mercury-2.3.0/mercury/apps/storage/utils.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-05-23 13:30:21.556417 mercury-2.3.0/mercury/apps/storage/views/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-31 12:45:08.000000 mercury-2.3.0/mercury/apps/storage/views/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6182 2023-03-31 11:42:07.000000 mercury-2.3.0/mercury/apps/storage/views/dashboardfiles.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4935 2023-03-31 11:42:07.000000 mercury-2.3.0/mercury/apps/storage/views/notebookfiles.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3737 2023-03-31 11:42:07.000000 mercury-2.3.0/mercury/apps/storage/views/workerfiles.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-05-23 13:30:21.556417 mercury-2.3.0/mercury/apps/tasks/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.3.0/mercury/apps/tasks/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      287 2022-03-09 11:04:20.000000 mercury-2.3.0/mercury/apps/tasks/admin.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      153 2022-03-09 11:04:20.000000 mercury-2.3.0/mercury/apps/tasks/apps.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      412 2022-03-09 11:06:47.000000 mercury-2.3.0/mercury/apps/tasks/clean_service.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4021 2023-05-23 13:11:25.000000 mercury-2.3.0/mercury/apps/tasks/export_pdf.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3805 2023-04-06 13:49:54.000000 mercury-2.3.0/mercury/apps/tasks/export_png.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-05-23 13:30:21.556417 mercury-2.3.0/mercury/apps/tasks/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1328 2023-03-29 09:06:05.000000 mercury-2.3.0/mercury/apps/tasks/migrations/0001_initial.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.3.0/mercury/apps/tasks/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      762 2022-05-18 10:19:32.000000 mercury-2.3.0/mercury/apps/tasks/models.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3659 2023-02-13 14:05:12.000000 mercury-2.3.0/mercury/apps/tasks/notify.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      433 2022-03-09 11:06:47.000000 mercury-2.3.0/mercury/apps/tasks/serializers.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    15223 2023-02-23 14:52:12.000000 mercury-2.3.0/mercury/apps/tasks/tasks.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1314 2023-02-13 14:05:12.000000 mercury-2.3.0/mercury/apps/tasks/tasks_export.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      571 2023-03-14 07:49:44.000000 mercury-2.3.0/mercury/apps/tasks/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1431 2023-04-25 12:37:36.000000 mercury-2.3.0/mercury/apps/tasks/urls.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     8714 2023-05-23 13:27:23.000000 mercury-2.3.0/mercury/apps/tasks/views.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-05-23 13:30:21.556417 mercury-2.3.0/mercury/apps/workers/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-14 07:49:44.000000 mercury-2.3.0/mercury/apps/workers/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       63 2023-03-14 07:49:44.000000 mercury-2.3.0/mercury/apps/workers/admin.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      151 2023-03-14 07:49:44.000000 mercury-2.3.0/mercury/apps/workers/apps.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-05-23 13:30:21.556417 mercury-2.3.0/mercury/apps/workers/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1286 2023-03-29 09:06:05.000000 mercury-2.3.0/mercury/apps/workers/migrations/0001_initial.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-14 07:49:44.000000 mercury-2.3.0/mercury/apps/workers/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      798 2023-03-29 09:06:05.000000 mercury-2.3.0/mercury/apps/workers/models.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      296 2023-03-14 07:49:44.000000 mercury-2.3.0/mercury/apps/workers/serializers.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       60 2023-03-14 07:49:44.000000 mercury-2.3.0/mercury/apps/workers/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1076 2023-04-25 12:37:59.000000 mercury-2.3.0/mercury/apps/workers/urls.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3881 2023-03-31 09:54:03.000000 mercury-2.3.0/mercury/apps/workers/views.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-05-23 13:30:21.560417 mercury-2.3.0/mercury/apps/ws/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.3.0/mercury/apps/ws/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      141 2023-02-13 14:05:12.000000 mercury-2.3.0/mercury/apps/ws/apps.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6162 2023-04-20 13:43:38.000000 mercury-2.3.0/mercury/apps/ws/client.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      947 2023-03-14 07:49:44.000000 mercury-2.3.0/mercury/apps/ws/middleware.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-05-23 13:30:21.560417 mercury-2.3.0/mercury/apps/ws/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.3.0/mercury/apps/ws/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      386 2023-02-28 13:59:46.000000 mercury-2.3.0/mercury/apps/ws/routing.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2495 2023-04-06 13:49:54.000000 mercury-2.3.0/mercury/apps/ws/tasks.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      137 2023-03-01 11:07:38.000000 mercury-2.3.0/mercury/apps/ws/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5106 2023-04-06 13:49:54.000000 mercury-2.3.0/mercury/apps/ws/utils.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1754 2023-03-14 07:49:44.000000 mercury-2.3.0/mercury/apps/ws/worker.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     7191 2023-03-31 14:11:10.000000 mercury-2.3.0/mercury/demo.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-05-23 13:30:21.560417 mercury-2.3.0/mercury/frontend-dist/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1158 2023-05-23 13:30:21.000000 mercury-2.3.0/mercury/frontend-dist/asset-manifest.json
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    15406 2023-05-23 13:30:06.000000 mercury-2.3.0/mercury/frontend-dist/favicon-old.ico
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    15086 2023-05-23 13:30:06.000000 mercury-2.3.0/mercury/frontend-dist/favicon.ico
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3086 2023-05-23 13:30:21.000000 mercury-2.3.0/mercury/frontend-dist/index.html
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    17406 2023-05-23 13:30:06.000000 mercury-2.3.0/mercury/frontend-dist/jupyter-additional.css
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4539 2023-05-23 13:30:06.000000 mercury-2.3.0/mercury/frontend-dist/jupyter-syntax.css
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   580392 2023-05-23 13:30:06.000000 mercury-2.3.0/mercury/frontend-dist/jupyter-theme-light.css
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      324 2023-05-23 13:30:06.000000 mercury-2.3.0/mercury/frontend-dist/manifest.json
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6237 2023-05-23 13:30:06.000000 mercury-2.3.0/mercury/frontend-dist/mercury_black_logo.svg
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6997 2023-05-23 13:30:06.000000 mercury-2.3.0/mercury/frontend-dist/mercury_logo.svg
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       67 2023-05-23 13:30:06.000000 mercury-2.3.0/mercury/frontend-dist/robots.txt
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-05-23 13:30:21.552417 mercury-2.3.0/mercury/frontend-dist/static/
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-05-23 13:30:21.560417 mercury-2.3.0/mercury/frontend-dist/static/css/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   229115 2023-05-23 13:30:21.000000 mercury-2.3.0/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   612316 2023-05-23 13:30:21.000000 mercury-2.3.0/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css.map
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3021 2023-05-23 13:30:21.000000 mercury-2.3.0/mercury/frontend-dist/static/css/main.80c2d41b.chunk.css
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5576 2023-05-23 13:30:21.000000 mercury-2.3.0/mercury/frontend-dist/static/css/main.80c2d41b.chunk.css.map
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-05-23 13:30:21.564417 mercury-2.3.0/mercury/frontend-dist/static/js/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)  1311795 2023-05-23 13:30:21.000000 mercury-2.3.0/mercury/frontend-dist/static/js/2.206848a5.chunk.js
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3383 2023-05-23 13:30:21.000000 mercury-2.3.0/mercury/frontend-dist/static/js/2.206848a5.chunk.js.LICENSE.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)  4972965 2023-05-23 13:30:21.000000 mercury-2.3.0/mercury/frontend-dist/static/js/2.206848a5.chunk.js.map
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    87682 2023-05-23 13:30:21.000000 mercury-2.3.0/mercury/frontend-dist/static/js/main.f1889776.chunk.js
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   267841 2023-05-23 13:30:21.000000 mercury-2.3.0/mercury/frontend-dist/static/js/main.f1889776.chunk.js.map
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1557 2023-05-23 13:30:21.000000 mercury-2.3.0/mercury/frontend-dist/static/js/runtime-main.248907bc.js
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     8276 2023-05-23 13:30:21.000000 mercury-2.3.0/mercury/frontend-dist/static/js/runtime-main.248907bc.js.map
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-05-23 13:30:21.568417 mercury-2.3.0/mercury/frontend-dist/static/media/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   165548 2023-05-23 13:30:21.000000 mercury-2.3.0/mercury/frontend-dist/static/media/fontawesome-webfont.1e59d233.ttf
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    77160 2023-05-23 13:30:21.000000 mercury-2.3.0/mercury/frontend-dist/static/media/fontawesome-webfont.20fd1704.woff2
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   165742 2023-05-23 13:30:21.000000 mercury-2.3.0/mercury/frontend-dist/static/media/fontawesome-webfont.8b43027f.eot
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   444379 2023-05-23 13:30:21.000000 mercury-2.3.0/mercury/frontend-dist/static/media/fontawesome-webfont.c1e38fd9.svg
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    98024 2023-05-23 13:30:21.000000 mercury-2.3.0/mercury/frontend-dist/static/media/fontawesome-webfont.f691f37e.woff
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      684 2022-03-09 11:04:20.000000 mercury-2.3.0/mercury/manage.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     9259 2023-05-23 11:37:47.000000 mercury-2.3.0/mercury/mercury.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      545 2023-04-25 12:41:47.000000 mercury-2.3.0/mercury/requirements.txt
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-05-23 13:30:21.568417 mercury-2.3.0/mercury/server/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       68 2022-03-09 11:04:20.000000 mercury-2.3.0/mercury/server/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      837 2023-03-14 07:49:44.000000 mercury-2.3.0/mercury/server/asgi.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2771 2023-03-24 08:43:00.000000 mercury-2.3.0/mercury/server/celery.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     9844 2023-04-05 13:16:51.000000 mercury-2.3.0/mercury/server/settings.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1575 2023-04-25 12:38:18.000000 mercury-2.3.0/mercury/server/urls.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1645 2023-03-01 12:07:40.000000 mercury-2.3.0/mercury/server/views.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      405 2022-05-18 11:03:41.000000 mercury-2.3.0/mercury/server/wsgi.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-05-23 13:30:21.568417 mercury-2.3.0/mercury/widgets/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.3.0/mercury/widgets/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2029 2023-05-23 08:29:51.000000 mercury-2.3.0/mercury/widgets/app.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2294 2023-04-07 10:30:37.000000 mercury-2.3.0/mercury/widgets/button.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      826 2023-04-07 10:43:02.000000 mercury-2.3.0/mercury/widgets/chat.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2140 2023-05-23 08:29:43.000000 mercury-2.3.0/mercury/widgets/checkbox.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      408 2023-04-07 10:32:14.000000 mercury-2.3.0/mercury/widgets/confetti.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3393 2023-04-07 10:30:37.000000 mercury-2.3.0/mercury/widgets/file.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4828 2023-02-21 07:28:26.000000 mercury-2.3.0/mercury/widgets/json.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6894 2023-04-07 10:30:37.000000 mercury-2.3.0/mercury/widgets/manager.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      104 2023-02-21 07:28:26.000000 mercury-2.3.0/mercury/widgets/md.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2703 2023-05-23 08:29:29.000000 mercury-2.3.0/mercury/widgets/multiselect.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1219 2023-02-21 07:48:36.000000 mercury-2.3.0/mercury/widgets/note.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2947 2023-05-23 12:22:38.000000 mercury-2.3.0/mercury/widgets/numberbox.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3029 2023-05-23 08:29:18.000000 mercury-2.3.0/mercury/widgets/numeric.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1255 2023-02-21 07:48:36.000000 mercury-2.3.0/mercury/widgets/outputdir.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3038 2023-05-23 08:29:05.000000 mercury-2.3.0/mercury/widgets/range.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2416 2023-05-23 08:28:57.000000 mercury-2.3.0/mercury/widgets/select.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2962 2023-05-23 08:28:46.000000 mercury-2.3.0/mercury/widgets/slider.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      222 2023-02-21 07:28:26.000000 mercury-2.3.0/mercury/widgets/stop.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2052 2023-05-23 08:26:54.000000 mercury-2.3.0/mercury/widgets/text.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-05-23 13:30:21.552417 mercury-2.3.0/mercury.egg-info/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6016 2023-05-23 13:30:21.000000 mercury-2.3.0/mercury.egg-info/PKG-INFO
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6314 2023-05-23 13:30:21.000000 mercury-2.3.0/mercury.egg-info/SOURCES.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2023-05-23 13:30:21.000000 mercury-2.3.0/mercury.egg-info/dependency_links.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       50 2023-05-23 13:30:21.000000 mercury-2.3.0/mercury.egg-info/entry_points.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      489 2023-05-23 13:30:21.000000 mercury-2.3.0/mercury.egg-info/requires.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        8 2023-05-23 13:30:21.000000 mercury-2.3.0/mercury.egg-info/top_level.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      106 2022-03-09 11:04:20.000000 mercury-2.3.0/pyproject.toml
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       38 2023-05-23 13:30:21.568417 mercury-2.3.0/setup.cfg
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1386 2023-05-23 13:29:36.000000 mercury-2.3.0/setup.py
```

### Comparing `mercury-2.2.9/PKG-INFO` & `mercury-2.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: mercury
-Version: 2.2.9
+Version: 2.3.0
 Summary: Turn Jupyter Notebook to Web App and share with non-technical users
 Home-page: https://github.com/mljar/mercury
+Author: MLJAR Sp. z o.o.
 Maintainer: MLJAR Sp. z o.o.
 Maintainer-email: contact@mljar.com
 License: UNKNOWN
 Description: 
         
         <p align="center">
           <img 
             alt="Mercury convert Jupyter Notebook to Web App"
             src="https://raw.githubusercontent.com/mljar/visual-identity/main/mercury/mercury-og.png" width="100%" />  
         </p>
         
         [![Tests](https://github.com/mljar/mercury/actions/workflows/run-tests.yml/badge.svg)](https://github.com/mljar/mercury/actions/workflows/run-tests.yml)
         [![PyPI version](https://badge.fury.io/py/mercury.svg)](https://badge.fury.io/py/mercury)
+        [![PyPI pyversions](https://img.shields.io/pypi/pyversions/mercury.svg)](https://pypi.python.org/pypi/mercury/)
         [![Anaconda-Server Badge](https://anaconda.org/conda-forge/mljar-mercury/badges/license.svg)](https://anaconda.org/conda-forge/mljar-mercury)
         
         # Build Web Apps in Jupyter Notebook
         
         Mercury allows you to add interactive widgets in Python notebooks, so you can share notebooks as web applications. Forget about rewriting notebooks to web frameworks just to share your results. Mercury offers a set of widgets with simple re-execution of cells.
         
         You can build with Mercury:
@@ -131,11 +133,15 @@
         Mercury is released with AGPL v3 license.
         
         Looking for dedicated support, a commercial-friendly license, and more features? The Mercury Pro is for you. Please see the details at [our website](https://mljar.com/pricing).
         
         
         
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mercury-2.2.9/README.md` & `mercury-2.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
   <img 
     alt="Mercury convert Jupyter Notebook to Web App"
     src="https://raw.githubusercontent.com/mljar/visual-identity/main/mercury/mercury-og.png" width="100%" />  
 </p>
 
 [![Tests](https://github.com/mljar/mercury/actions/workflows/run-tests.yml/badge.svg)](https://github.com/mljar/mercury/actions/workflows/run-tests.yml)
 [![PyPI version](https://badge.fury.io/py/mercury.svg)](https://badge.fury.io/py/mercury)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/mercury.svg)](https://pypi.python.org/pypi/mercury/)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/mljar-mercury/badges/license.svg)](https://anaconda.org/conda-forge/mljar-mercury)
 
 # Build Web Apps in Jupyter Notebook
 
 Mercury allows you to add interactive widgets in Python notebooks, so you can share notebooks as web applications. Forget about rewriting notebooks to web frameworks just to share your results. Mercury offers a set of widgets with simple re-execution of cells.
 
 You can build with Mercury:
```

### Comparing `mercury-2.2.9/mercury/apps/accounts/fields.py` & `mercury-2.3.0/mercury/apps/accounts/fields.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/accounts/migrations/0001_initial.py` & `mercury-2.3.0/mercury/apps/accounts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/accounts/models.py` & `mercury-2.3.0/mercury/apps/accounts/models.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/accounts/serializers.py` & `mercury-2.3.0/mercury/apps/accounts/serializers.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/accounts/tasks.py` & `mercury-2.3.0/mercury/apps/accounts/tasks.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/accounts/tests/test_accounts.py` & `mercury-2.3.0/mercury/apps/accounts/tests/test_accounts.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/accounts/tests/test_invitations.py` & `mercury-2.3.0/mercury/apps/accounts/tests/test_invitations.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/accounts/tests/test_secrets.py` & `mercury-2.3.0/mercury/apps/accounts/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/accounts/tests/test_sites.py` & `mercury-2.3.0/mercury/apps/accounts/tests/test_sites.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/accounts/tests/test_subscription.py` & `mercury-2.3.0/mercury/apps/accounts/tests/test_subscription.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/accounts/urls.py` & `mercury-2.3.0/mercury/apps/accounts/urls.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/accounts/views/accounts.py` & `mercury-2.3.0/mercury/apps/accounts/views/accounts.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/accounts/views/invitations.py` & `mercury-2.3.0/mercury/apps/accounts/views/invitations.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/accounts/views/permissions.py` & `mercury-2.3.0/mercury/apps/accounts/views/permissions.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/accounts/views/secrets.py` & `mercury-2.3.0/mercury/apps/accounts/views/secrets.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/accounts/views/sites.py` & `mercury-2.3.0/mercury/apps/accounts/views/sites.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
             subdomain = "single-site"
             domain = "runmercury.com"
 
         if request.build_absolute_uri().startswith("http://127.0.0.1"):
             subdomain = "single-site"
             domain = "runmercury.com"
 
-        print(f"{url}|{request.build_absolute_uri()}|{subdomain}|{domain}|{custom_domain}")
+        # print(f"{url}|{request.build_absolute_uri()}|{subdomain}|{domain}|{custom_domain}")
 
         sites = Site.objects.filter(
             Q(custom_domain=custom_domain) | Q(slug=subdomain, domain=domain)
         )
         if not sites:
             return Response(status=status.HTTP_404_NOT_FOUND)
```

### Comparing `mercury-2.2.9/mercury/apps/accounts/views/subscription.py` & `mercury-2.3.0/mercury/apps/accounts/views/subscription.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/nb/exporter.py` & `mercury-2.3.0/mercury/apps/nb/exporter.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/nb/nbrun.py` & `mercury-2.3.0/mercury/apps/nb/nbrun.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/nb/tests/test_nbrun.py` & `mercury-2.3.0/mercury/apps/nb/tests/test_nbrun.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/nb/tests.py` & `mercury-2.3.0/mercury/apps/nb/tests.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/nbworker/__main__.py` & `mercury-2.3.0/mercury/apps/nbworker/__main__.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/nbworker/nb.py` & `mercury-2.3.0/mercury/apps/nbworker/nb.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/nbworker/rest.py` & `mercury-2.3.0/mercury/apps/nbworker/rest.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/nbworker/tests.py` & `mercury-2.3.0/mercury/apps/nbworker/tests.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/nbworker/utils.py` & `mercury-2.3.0/mercury/apps/nbworker/utils.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/nbworker/ws.py` & `mercury-2.3.0/mercury/apps/nbworker/ws.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/notebooks/management/commands/add.py` & `mercury-2.3.0/mercury/apps/notebooks/management/commands/add.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/notebooks/management/commands/delete.py` & `mercury-2.3.0/mercury/apps/notebooks/management/commands/delete.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/notebooks/management/commands/list.py` & `mercury-2.3.0/mercury/apps/notebooks/management/commands/list.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/notebooks/management/commands/watch.py` & `mercury-2.3.0/mercury/apps/notebooks/management/commands/watch.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/notebooks/migrations/0001_initial.py` & `mercury-2.3.0/mercury/apps/notebooks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/notebooks/models.py` & `mercury-2.3.0/mercury/apps/notebooks/models.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/notebooks/serializers.py` & `mercury-2.3.0/mercury/apps/notebooks/serializers.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/notebooks/slides_themes.py` & `mercury-2.3.0/mercury/apps/notebooks/slides_themes.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/notebooks/tasks.py` & `mercury-2.3.0/mercury/apps/notebooks/tasks.py`

 * *Files 3% similar despite different names*

```diff
@@ -232,14 +232,16 @@
                 if not Site.objects.filter(slug="single-site"):
                     site = Site.objects.create(
                         title="Mercury",
                         slug="single-site",
                         share=Site.PUBLIC,
                         created_by=user,
                         status=SiteStatus.READY,
+                        domain=os.environ.get("MERCURY_DOMAIN", "runmercury.com"),
+                        custom_domain=os.environ.get("MERCURY_CUSTOM_DOMAIN")
                     )
                 else:
                     site = Site.objects.get(slug="single-site")
 
             bucket_key_fname = ""
             if bucket_key is not None:
                 s3 = S3()
```

### Comparing `mercury-2.2.9/mercury/apps/notebooks/urls.py` & `mercury-2.3.0/mercury/apps/notebooks/urls.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/notebooks/views.py` & `mercury-2.3.0/mercury/apps/notebooks/views.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/storage/migrations/0001_initial.py` & `mercury-2.3.0/mercury/apps/storage/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/storage/migrations/0002_useruploadedfile.py` & `mercury-2.3.0/mercury/apps/storage/migrations/0002_useruploadedfile.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/storage/models.py` & `mercury-2.3.0/mercury/apps/storage/models.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/storage/s3utils.py` & `mercury-2.3.0/mercury/apps/storage/s3utils.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/storage/storage.py` & `mercury-2.3.0/mercury/apps/storage/storage.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/storage/tests.py` & `mercury-2.3.0/mercury/apps/storage/tests.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/storage/urls.py` & `mercury-2.3.0/mercury/apps/storage/urls.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/storage/views/dashboardfiles.py` & `mercury-2.3.0/mercury/apps/storage/views/dashboardfiles.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/storage/views/notebookfiles.py` & `mercury-2.3.0/mercury/apps/storage/views/notebookfiles.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/storage/views/workerfiles.py` & `mercury-2.3.0/mercury/apps/storage/views/workerfiles.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/tasks/export_pdf.py` & `mercury-2.3.0/mercury/apps/tasks/export_pdf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import asyncio
 import concurrent.futures
 import logging
 import os
 import tempfile
 from subprocess import PIPE, Popen
 
-from pyppeteer import launch
-
-
+pdf_export_available = True
+try:
+    from pyppeteer import launch
+except Exception:
+    pdf_export_available = False
+    
 async def html_to_pdf(html_file, pdf_file, pyppeteer_args=None):
     """Convert a HTML file to a PDF"""
     browser = await launch(
         handleSIGINT=False,
         handleSIGTERM=False,
         handleSIGHUP=False,
         headless=True,
@@ -116,14 +119,17 @@
     command = ["pyppeteer-install"]
     with Popen(command, stdout=PIPE, stderr=PIPE) as proc:
         print(proc.stdout.read())
         print(proc.stderr.read())
 
 
 def to_pdf(html_input_file, pdf_output_file):
+    if not pdf_export_available:
+        print("PDF export not available")
+        return
     # make sure chromium is installed
     # install_chromium()
 
     # dont want to see DEBUG logs for chromium ...
     prev_log_level = logging.getLogger().getEffectiveLevel()
     logging.getLogger().setLevel(logging.ERROR)
```

### Comparing `mercury-2.2.9/mercury/apps/tasks/export_png.py` & `mercury-2.3.0/mercury/apps/tasks/export_png.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/tasks/migrations/0001_initial.py` & `mercury-2.3.0/mercury/apps/tasks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/tasks/models.py` & `mercury-2.3.0/mercury/apps/tasks/models.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/tasks/notify.py` & `mercury-2.3.0/mercury/apps/tasks/notify.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/tasks/tasks.py` & `mercury-2.3.0/mercury/apps/tasks/tasks.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/tasks/tasks_export.py` & `mercury-2.3.0/mercury/apps/tasks/tasks_export.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/tasks/tests.py` & `mercury-2.3.0/mercury/apps/tasks/tests.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/tasks/urls.py` & `mercury-2.3.0/mercury/apps/tasks/urls.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/tasks/views.py` & `mercury-2.3.0/mercury/apps/tasks/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,19 +194,22 @@
             raise Http404()
 
 
 class ExportPDF(APIView):
     def post(self, request):
         try:
             # check if user can access the notebook
-            notebook = notebooks_queryset(request).get(pk=request.data["notebook_id"])
+            notebook = notebooks_queryset(request, request.data.get("site_id")).get(
+                pk=request.data["notebook_id"]
+            )
         except Notebook.DoesNotExist:
             raise Http404()
         try:
             celery_job = export_to_pdf.delay(request.data)
+            print(celery_job.id)
             return Response({"job_id": celery_job.id}, status=status.HTTP_201_CREATED)
         except Exception as e:
             raise APIException(str(e))
 
 
 class GetPDFAddress(APIView):
     def get(self, request, job_id):
```

### Comparing `mercury-2.2.9/mercury/apps/workers/migrations/0001_initial.py` & `mercury-2.3.0/mercury/apps/workers/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/workers/models.py` & `mercury-2.3.0/mercury/apps/workers/models.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/workers/urls.py` & `mercury-2.3.0/mercury/apps/workers/urls.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/workers/views.py` & `mercury-2.3.0/mercury/apps/workers/views.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/ws/client.py` & `mercury-2.3.0/mercury/apps/ws/client.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/ws/middleware.py` & `mercury-2.3.0/mercury/apps/ws/middleware.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/ws/tasks.py` & `mercury-2.3.0/mercury/apps/ws/tasks.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/ws/utils.py` & `mercury-2.3.0/mercury/apps/ws/utils.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/apps/ws/worker.py` & `mercury-2.3.0/mercury/apps/ws/worker.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/demo.py` & `mercury-2.3.0/mercury/demo.py`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/frontend-dist/favicon-old.ico` & `mercury-2.3.0/mercury/frontend-dist/favicon-old.ico`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/frontend-dist/favicon.ico` & `mercury-2.3.0/mercury/frontend-dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/frontend-dist/index.html` & `mercury-2.3.0/mercury/frontend-dist/index.html`

 * *Files 6% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="/static/favicon.ico"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Mercury: Easily share your Python notebooks"/><link rel="manifest" href="/static/manifest.json"/><script src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.1.10/require.min.js"></script><link rel="stylesheet" href="/static/jupyter-syntax.css"/><link rel="stylesheet" href="/static/jupyter-additional.css"/><link rel="stylesheet" href="/static/jupyter-theme-light.css"/><title>Mercury - Turn Jupyter Notebook to Web App</title><script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/latest.js?config=TeX-AMS_CHTML-full,Safe"></script><script>init_mathjax=function(){window.MathJax&&(MathJax.Hub.Config({showProcessingMessages:!1,TeX:{equationNumbers:{autoNumber:"AMS",useLabelIds:!0}},tex2jax:{inlineMath:[["$","$"],["\\(","\\)"]],displayMath:[["$$","$$"],["\\[","\\]"]],processEscapes:!0,processEnvironments:!0},displayAlign:"center",CommonHTML:{linebreaks:{automatic:!0}}}),MathJax.Hub.Queue(["Typeset",MathJax.Hub]))},init_mathjax()</script><link href="/static/css/2.c6cf5ff9.chunk.css" rel="stylesheet"><link href="/static/css/main.26f96620.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function r(r){for(var n,f,l=r[0],i=r[1],a=r[2],c=0,s=[];c<l.length;c++)f=l[c],Object.prototype.hasOwnProperty.call(o,f)&&o[f]&&s.push(o[f][0]),o[f]=0;for(n in i)Object.prototype.hasOwnProperty.call(i,n)&&(e[n]=i[n]);for(p&&p(r);s.length;)s.shift()();return u.push.apply(u,a||[]),t()}function t(){for(var e,r=0;r<u.length;r++){for(var t=u[r],n=!0,l=1;l<t.length;l++){var i=t[l];0!==o[i]&&(n=!1)}n&&(u.splice(r--,1),e=f(f.s=t[0]))}return e}var n={},o={1:0},u=[];function f(r){if(n[r])return n[r].exports;var t=n[r]={i:r,l:!1,exports:{}};return e[r].call(t.exports,t,t.exports,f),t.l=!0,t.exports}f.m=e,f.c=n,f.d=function(e,r,t){f.o(e,r)||Object.defineProperty(e,r,{enumerable:!0,get:t})},f.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},f.t=function(e,r){if(1&r&&(e=f(e)),8&r)return e;if(4&r&&"object"==typeof e&&e&&e.__esModule)return e;var t=Object.create(null);if(f.r(t),Object.defineProperty(t,"default",{enumerable:!0,value:e}),2&r&&"string"!=typeof e)for(var n in e)f.d(t,n,function(r){return e[r]}.bind(null,n));return t},f.n=function(e){var r=e&&e.__esModule?function(){return e.default}:function(){return e};return f.d(r,"a",r),r},f.o=function(e,r){return Object.prototype.hasOwnProperty.call(e,r)},f.p="/";var l=this.webpackJsonpfrontend=this.webpackJsonpfrontend||[],i=l.push.bind(l);l.push=r,l=l.slice();for(var a=0;a<l.length;a++)r(l[a]);var p=i;t()}([])</script><script src="/static/js/2.6305b467.chunk.js"></script><script src="/static/js/main.f9a369a0.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="/static/favicon.ico"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Mercury: Easily share your Python notebooks"/><link rel="manifest" href="/static/manifest.json"/><script src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.1.10/require.min.js"></script><link rel="stylesheet" href="/static/jupyter-syntax.css"/><link rel="stylesheet" href="/static/jupyter-additional.css"/><link rel="stylesheet" href="/static/jupyter-theme-light.css"/><title>Mercury - Turn Jupyter Notebook to Web App</title><script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/latest.js?config=TeX-AMS_CHTML-full,Safe"></script><script>init_mathjax=function(){window.MathJax&&(MathJax.Hub.Config({showProcessingMessages:!1,TeX:{equationNumbers:{autoNumber:"AMS",useLabelIds:!0}},tex2jax:{inlineMath:[["$","$"],["\\(","\\)"]],displayMath:[["$$","$$"],["\\[","\\]"]],processEscapes:!0,processEnvironments:!0},displayAlign:"center",CommonHTML:{linebreaks:{automatic:!0}}}),MathJax.Hub.Queue(["Typeset",MathJax.Hub]))},init_mathjax()</script><link href="/static/css/2.c6cf5ff9.chunk.css" rel="stylesheet"><link href="/static/css/main.80c2d41b.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function r(r){for(var n,f,l=r[0],i=r[1],a=r[2],c=0,s=[];c<l.length;c++)f=l[c],Object.prototype.hasOwnProperty.call(o,f)&&o[f]&&s.push(o[f][0]),o[f]=0;for(n in i)Object.prototype.hasOwnProperty.call(i,n)&&(e[n]=i[n]);for(p&&p(r);s.length;)s.shift()();return u.push.apply(u,a||[]),t()}function t(){for(var e,r=0;r<u.length;r++){for(var t=u[r],n=!0,l=1;l<t.length;l++){var i=t[l];0!==o[i]&&(n=!1)}n&&(u.splice(r--,1),e=f(f.s=t[0]))}return e}var n={},o={1:0},u=[];function f(r){if(n[r])return n[r].exports;var t=n[r]={i:r,l:!1,exports:{}};return e[r].call(t.exports,t,t.exports,f),t.l=!0,t.exports}f.m=e,f.c=n,f.d=function(e,r,t){f.o(e,r)||Object.defineProperty(e,r,{enumerable:!0,get:t})},f.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},f.t=function(e,r){if(1&r&&(e=f(e)),8&r)return e;if(4&r&&"object"==typeof e&&e&&e.__esModule)return e;var t=Object.create(null);if(f.r(t),Object.defineProperty(t,"default",{enumerable:!0,value:e}),2&r&&"string"!=typeof e)for(var n in e)f.d(t,n,function(r){return e[r]}.bind(null,n));return t},f.n=function(e){var r=e&&e.__esModule?function(){return e.default}:function(){return e};return f.d(r,"a",r),r},f.o=function(e,r){return Object.prototype.hasOwnProperty.call(e,r)},f.p="/";var l=this.webpackJsonpfrontend=this.webpackJsonpfrontend||[],i=l.push.bind(l);l.push=r,l=l.slice();for(var a=0;a<l.length;a++)r(l[a]);var p=i;t()}([])</script><script src="/static/js/2.206848a5.chunk.js"></script><script src="/static/js/main.f1889776.chunk.js"></script></body></html>
```

### Comparing `mercury-2.2.9/mercury/frontend-dist/jupyter-additional.css` & `mercury-2.3.0/mercury/frontend-dist/jupyter-additional.css`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/frontend-dist/jupyter-syntax.css` & `mercury-2.3.0/mercury/frontend-dist/jupyter-syntax.css`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/frontend-dist/jupyter-theme-light.css` & `mercury-2.3.0/mercury/frontend-dist/jupyter-theme-light.css`

 * *Files 0% similar despite different names*

```diff
@@ -35206,1070 +35206,1070 @@
 00089850: 2774 2077 7261 7020 746f 2068 616e 646c  't wrap to handl
 00089860: 6520 6c61 7267 6520 7072 6f6d 7074 206e  e large prompt n
 00089870: 756d 6265 7273 202a 2f0a 2020 2020 7465  umbers */.    te
 00089880: 7874 2d61 6c69 676e 3a20 7269 6768 743b  xt-align: right;
 00089890: 0a20 2020 2077 6869 7465 2d73 7061 6365  .    white-space
 000898a0: 3a20 6e6f 7772 6170 3b0a 2020 2020 6f76  : nowrap;.    ov
 000898b0: 6572 666c 6f77 3a20 6869 6464 656e 3b0a  erflow: hidden;.
-000898c0: 2020 2020 7465 7874 2d6f 7665 7266 6c6f      text-overflo
-000898d0: 773a 2065 6c6c 6970 7369 733b 0a20 2020  w: ellipsis;.   
-000898e0: 202f 2a20 4469 7361 626c 6520 7465 7874   /* Disable text
-000898f0: 2073 656c 6563 7469 6f6e 202a 2f0a 2020   selection */.  
-00089900: 2020 2d77 6562 6b69 742d 7573 6572 2d73    -webkit-user-s
-00089910: 656c 6563 743a 206e 6f6e 653b 0a20 2020  elect: none;.   
-00089920: 202d 6d6f 7a2d 7573 6572 2d73 656c 6563   -moz-user-selec
-00089930: 743a 206e 6f6e 653b 0a20 2020 202d 6d73  t: none;.    -ms
-00089940: 2d75 7365 722d 7365 6c65 6374 3a20 6e6f  -user-select: no
-00089950: 6e65 3b0a 2020 2020 7573 6572 2d73 656c  ne;.    user-sel
-00089960: 6563 743a 206e 6f6e 653b 0a20 2020 2070  ect: none;.    p
-00089970: 6164 6469 6e67 2d72 6967 6874 3a20 3630  adding-right: 60
-00089980: 7078 3b0a 2020 7d0a 2020 0a20 2062 6f64  px;.  }.  .  bod
-00089990: 795b 6461 7461 2d66 6f72 6d61 743d 276d  y[data-format='m
-000899a0: 6f62 696c 6527 5d20 2e6a 702d 496e 7075  obile'] .jp-Inpu
-000899b0: 7450 726f 6d70 7420 7b0a 2020 2020 666c  tPrompt {.    fl
-000899c0: 6578 3a20 3020 3020 6175 746f 3b0a 2020  ex: 0 0 auto;.  
-000899d0: 2020 7465 7874 2d61 6c69 676e 3a20 6c65    text-align: le
-000899e0: 6674 3b0a 2020 7d0a 2020 0a20 202f 2a2d  ft;.  }.  .  /*-
-000899f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000898c0: 2020 2020 2f2a 2074 6578 742d 6f76 6572      /* text-over
+000898d0: 666c 6f77 3a20 656c 6c69 7073 6973 3b20  flow: ellipsis; 
+000898e0: 2a2f 0a20 2020 202f 2a20 4469 7361 626c  */.    /* Disabl
+000898f0: 6520 7465 7874 2073 656c 6563 7469 6f6e  e text selection
+00089900: 202a 2f0a 2020 2020 2d77 6562 6b69 742d   */.    -webkit-
+00089910: 7573 6572 2d73 656c 6563 743a 206e 6f6e  user-select: non
+00089920: 653b 0a20 2020 202d 6d6f 7a2d 7573 6572  e;.    -moz-user
+00089930: 2d73 656c 6563 743a 206e 6f6e 653b 0a20  -select: none;. 
+00089940: 2020 202d 6d73 2d75 7365 722d 7365 6c65     -ms-user-sele
+00089950: 6374 3a20 6e6f 6e65 3b0a 2020 2020 7573  ct: none;.    us
+00089960: 6572 2d73 656c 6563 743a 206e 6f6e 653b  er-select: none;
+00089970: 0a20 2020 2070 6164 6469 6e67 2d72 6967  .    padding-rig
+00089980: 6874 3a20 3630 7078 3b0a 2020 7d0a 2020  ht: 60px;.  }.  
+00089990: 0a20 2062 6f64 795b 6461 7461 2d66 6f72  .  body[data-for
+000899a0: 6d61 743d 276d 6f62 696c 6527 5d20 2e6a  mat='mobile'] .j
+000899b0: 702d 496e 7075 7450 726f 6d70 7420 7b0a  p-InputPrompt {.
+000899c0: 2020 2020 666c 6578 3a20 3020 3020 6175      flex: 0 0 au
+000899d0: 746f 3b0a 2020 2020 7465 7874 2d61 6c69  to;.    text-ali
+000899e0: 676e 3a20 6c65 6674 3b0a 2020 7d0a 2020  gn: left;.  }.  
+000899f0: 0a20 202f 2a2d 2d2d 2d2d 2d2d 2d2d 2d2d  .  /*-----------
 00089a00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00089a10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00089a20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00089a30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 207c  ------------.  |
-00089a40: 2043 6f70 7972 6967 6874 2028 6329 204a   Copyright (c) J
-00089a50: 7570 7974 6572 2044 6576 656c 6f70 6d65  upyter Developme
-00089a60: 6e74 2054 6561 6d2e 0a20 207c 2044 6973  nt Team..  | Dis
-00089a70: 7472 6962 7574 6564 2075 6e64 6572 2074  tributed under t
-00089a80: 6865 2074 6572 6d73 206f 6620 7468 6520  he terms of the 
-00089a90: 4d6f 6469 6669 6564 2042 5344 204c 6963  Modified BSD Lic
-00089aa0: 656e 7365 2e0a 2020 7c2d 2d2d 2d2d 2d2d  ense..  |-------
+00089a30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00089a40: 2d2d 0a20 207c 2043 6f70 7972 6967 6874  --.  | Copyright
+00089a50: 2028 6329 204a 7570 7974 6572 2044 6576   (c) Jupyter Dev
+00089a60: 656c 6f70 6d65 6e74 2054 6561 6d2e 0a20  elopment Team.. 
+00089a70: 207c 2044 6973 7472 6962 7574 6564 2075   | Distributed u
+00089a80: 6e64 6572 2074 6865 2074 6572 6d73 206f  nder the terms o
+00089a90: 6620 7468 6520 4d6f 6469 6669 6564 2042  f the Modified B
+00089aa0: 5344 204c 6963 656e 7365 2e0a 2020 7c2d  SD License..  |-
 00089ab0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00089ac0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00089ad0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00089ae0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00089af0: 2d2d 2d2d 2d2a 2f0a 2020 0a20 202f 2a2d  -----*/.  .  /*-
-00089b00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00089af0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2a 2f0a 2020  -----------*/.  
+00089b00: 0a20 202f 2a2d 2d2d 2d2d 2d2d 2d2d 2d2d  .  /*-----------
 00089b10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00089b20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00089b30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00089b40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 207c  ------------.  |
-00089b50: 2050 6c61 6365 686f 6c64 6572 0a20 207c   Placeholder.  |
-00089b60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00089b40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00089b50: 2d2d 0a20 207c 2050 6c61 6365 686f 6c64  --.  | Placehold
+00089b60: 6572 0a20 207c 2d2d 2d2d 2d2d 2d2d 2d2d  er.  |----------
 00089b70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00089b80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00089b90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00089ba0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2a2f 0a20  ------------*/. 
-00089bb0: 200a 2020 2e6a 702d 506c 6163 6568 6f6c   .  .jp-Placehol
-00089bc0: 6465 7220 7b0a 2020 2020 6469 7370 6c61  der {.    displa
-00089bd0: 793a 2066 6c65 783b 0a20 2020 2066 6c65  y: flex;.    fle
-00089be0: 782d 6469 7265 6374 696f 6e3a 2072 6f77  x-direction: row
-00089bf0: 3b0a 2020 2020 666c 6578 3a20 3120 3120  ;.    flex: 1 1 
-00089c00: 6175 746f 3b0a 2020 7d0a 2020 0a20 202e  auto;.  }.  .  .
-00089c10: 6a70 2d50 6c61 6365 686f 6c64 6572 2d70  jp-Placeholder-p
-00089c20: 726f 6d70 7420 7b0a 2020 2020 626f 782d  rompt {.    box-
-00089c30: 7369 7a69 6e67 3a20 626f 7264 6572 2d62  sizing: border-b
-00089c40: 6f78 3b0a 2020 7d0a 2020 0a20 202e 6a70  ox;.  }.  .  .jp
-00089c50: 2d50 6c61 6365 686f 6c64 6572 2d63 6f6e  -Placeholder-con
-00089c60: 7465 6e74 207b 0a20 2020 2066 6c65 783a  tent {.    flex:
-00089c70: 2031 2031 2061 7574 6f3b 0a20 2020 2062   1 1 auto;.    b
-00089c80: 6f72 6465 723a 206e 6f6e 653b 0a20 2020  order: none;.   
-00089c90: 2062 6163 6b67 726f 756e 643a 2074 7261   background: tra
-00089ca0: 6e73 7061 7265 6e74 3b0a 2020 2020 6865  nsparent;.    he
-00089cb0: 6967 6874 3a20 3230 7078 3b0a 2020 2020  ight: 20px;.    
-00089cc0: 626f 782d 7369 7a69 6e67 3a20 626f 7264  box-sizing: bord
-00089cd0: 6572 2d62 6f78 3b0a 2020 7d0a 2020 0a20  er-box;.  }.  . 
-00089ce0: 202e 6a70 2d50 6c61 6365 686f 6c64 6572   .jp-Placeholder
-00089cf0: 2d63 6f6e 7465 6e74 202e 6a70 2d4d 6f72  -content .jp-Mor
-00089d00: 6548 6f72 697a 4963 6f6e 207b 0a20 2020  eHorizIcon {.   
-00089d10: 2077 6964 7468 3a20 3332 7078 3b0a 2020   width: 32px;.  
-00089d20: 2020 6865 6967 6874 3a20 3136 7078 3b0a    height: 16px;.
-00089d30: 2020 2020 626f 7264 6572 3a20 3170 7820      border: 1px 
-00089d40: 736f 6c69 6420 7472 616e 7370 6172 656e  solid transparen
-00089d50: 743b 0a20 2020 2062 6f72 6465 722d 7261  t;.    border-ra
-00089d60: 6469 7573 3a20 7661 7228 2d2d 6a70 2d62  dius: var(--jp-b
-00089d70: 6f72 6465 722d 7261 6469 7573 293b 0a20  order-radius);. 
-00089d80: 207d 0a20 200a 2020 2e6a 702d 506c 6163   }.  .  .jp-Plac
-00089d90: 6568 6f6c 6465 722d 636f 6e74 656e 7420  eholder-content 
-00089da0: 2e6a 702d 4d6f 7265 486f 7269 7a49 636f  .jp-MoreHorizIco
-00089db0: 6e3a 686f 7665 7220 7b0a 2020 2020 626f  n:hover {.    bo
-00089dc0: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
-00089dd0: 7661 7228 2d2d 6a70 2d62 6f72 6465 722d  var(--jp-border-
-00089de0: 636f 6c6f 7231 293b 0a20 2020 2062 6f78  color1);.    box
-00089df0: 2d73 6861 646f 773a 2030 7078 2030 7078  -shadow: 0px 0px
-00089e00: 2032 7078 2030 7078 2072 6762 6128 302c   2px 0px rgba(0,
-00089e10: 2030 2c20 302c 2030 2e32 3529 3b0a 2020   0, 0, 0.25);.  
-00089e20: 2020 6261 636b 6772 6f75 6e64 2d63 6f6c    background-col
-00089e30: 6f72 3a20 7661 7228 2d2d 6a70 2d6c 6179  or: var(--jp-lay
-00089e40: 6f75 742d 636f 6c6f 7230 293b 0a20 207d  out-color0);.  }
-00089e50: 0a20 200a 2020 2f2a 2d2d 2d2d 2d2d 2d2d  .  .  /*--------
+00089ba0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00089bb0: 2d2d 2a2f 0a20 200a 2020 2e6a 702d 506c  --*/.  .  .jp-Pl
+00089bc0: 6163 6568 6f6c 6465 7220 7b0a 2020 2020  aceholder {.    
+00089bd0: 6469 7370 6c61 793a 2066 6c65 783b 0a20  display: flex;. 
+00089be0: 2020 2066 6c65 782d 6469 7265 6374 696f     flex-directio
+00089bf0: 6e3a 2072 6f77 3b0a 2020 2020 666c 6578  n: row;.    flex
+00089c00: 3a20 3120 3120 6175 746f 3b0a 2020 7d0a  : 1 1 auto;.  }.
+00089c10: 2020 0a20 202e 6a70 2d50 6c61 6365 686f    .  .jp-Placeho
+00089c20: 6c64 6572 2d70 726f 6d70 7420 7b0a 2020  lder-prompt {.  
+00089c30: 2020 626f 782d 7369 7a69 6e67 3a20 626f    box-sizing: bo
+00089c40: 7264 6572 2d62 6f78 3b0a 2020 7d0a 2020  rder-box;.  }.  
+00089c50: 0a20 202e 6a70 2d50 6c61 6365 686f 6c64  .  .jp-Placehold
+00089c60: 6572 2d63 6f6e 7465 6e74 207b 0a20 2020  er-content {.   
+00089c70: 2066 6c65 783a 2031 2031 2061 7574 6f3b   flex: 1 1 auto;
+00089c80: 0a20 2020 2062 6f72 6465 723a 206e 6f6e  .    border: non
+00089c90: 653b 0a20 2020 2062 6163 6b67 726f 756e  e;.    backgroun
+00089ca0: 643a 2074 7261 6e73 7061 7265 6e74 3b0a  d: transparent;.
+00089cb0: 2020 2020 6865 6967 6874 3a20 3230 7078      height: 20px
+00089cc0: 3b0a 2020 2020 626f 782d 7369 7a69 6e67  ;.    box-sizing
+00089cd0: 3a20 626f 7264 6572 2d62 6f78 3b0a 2020  : border-box;.  
+00089ce0: 7d0a 2020 0a20 202e 6a70 2d50 6c61 6365  }.  .  .jp-Place
+00089cf0: 686f 6c64 6572 2d63 6f6e 7465 6e74 202e  holder-content .
+00089d00: 6a70 2d4d 6f72 6548 6f72 697a 4963 6f6e  jp-MoreHorizIcon
+00089d10: 207b 0a20 2020 2077 6964 7468 3a20 3332   {.    width: 32
+00089d20: 7078 3b0a 2020 2020 6865 6967 6874 3a20  px;.    height: 
+00089d30: 3136 7078 3b0a 2020 2020 626f 7264 6572  16px;.    border
+00089d40: 3a20 3170 7820 736f 6c69 6420 7472 616e  : 1px solid tran
+00089d50: 7370 6172 656e 743b 0a20 2020 2062 6f72  sparent;.    bor
+00089d60: 6465 722d 7261 6469 7573 3a20 7661 7228  der-radius: var(
+00089d70: 2d2d 6a70 2d62 6f72 6465 722d 7261 6469  --jp-border-radi
+00089d80: 7573 293b 0a20 207d 0a20 200a 2020 2e6a  us);.  }.  .  .j
+00089d90: 702d 506c 6163 6568 6f6c 6465 722d 636f  p-Placeholder-co
+00089da0: 6e74 656e 7420 2e6a 702d 4d6f 7265 486f  ntent .jp-MoreHo
+00089db0: 7269 7a49 636f 6e3a 686f 7665 7220 7b0a  rizIcon:hover {.
+00089dc0: 2020 2020 626f 7264 6572 3a20 3170 7820      border: 1px 
+00089dd0: 736f 6c69 6420 7661 7228 2d2d 6a70 2d62  solid var(--jp-b
+00089de0: 6f72 6465 722d 636f 6c6f 7231 293b 0a20  order-color1);. 
+00089df0: 2020 2062 6f78 2d73 6861 646f 773a 2030     box-shadow: 0
+00089e00: 7078 2030 7078 2032 7078 2030 7078 2072  px 0px 2px 0px r
+00089e10: 6762 6128 302c 2030 2c20 302c 2030 2e32  gba(0, 0, 0, 0.2
+00089e20: 3529 3b0a 2020 2020 6261 636b 6772 6f75  5);.    backgrou
+00089e30: 6e64 2d63 6f6c 6f72 3a20 7661 7228 2d2d  nd-color: var(--
+00089e40: 6a70 2d6c 6179 6f75 742d 636f 6c6f 7230  jp-layout-color0
+00089e50: 293b 0a20 207d 0a20 200a 2020 2f2a 2d2d  );.  }.  .  /*--
 00089e60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00089e70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00089e80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00089e90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00089ea0: 2d2d 2d2d 2d0a 2020 7c20 436f 7079 7269  -----.  | Copyri
-00089eb0: 6768 7420 2863 2920 4a75 7079 7465 7220  ght (c) Jupyter 
-00089ec0: 4465 7665 6c6f 706d 656e 7420 5465 616d  Development Team
-00089ed0: 2e0a 2020 7c20 4469 7374 7269 6275 7465  ..  | Distribute
-00089ee0: 6420 756e 6465 7220 7468 6520 7465 726d  d under the term
-00089ef0: 7320 6f66 2074 6865 204d 6f64 6966 6965  s of the Modifie
-00089f00: 6420 4253 4420 4c69 6365 6e73 652e 0a20  d BSD License.. 
-00089f10: 207c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |--------------
+00089ea0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 7c20  -----------.  | 
+00089eb0: 436f 7079 7269 6768 7420 2863 2920 4a75  Copyright (c) Ju
+00089ec0: 7079 7465 7220 4465 7665 6c6f 706d 656e  pyter Developmen
+00089ed0: 7420 5465 616d 2e0a 2020 7c20 4469 7374  t Team..  | Dist
+00089ee0: 7269 6275 7465 6420 756e 6465 7220 7468  ributed under th
+00089ef0: 6520 7465 726d 7320 6f66 2074 6865 204d  e terms of the M
+00089f00: 6f64 6966 6965 6420 4253 4420 4c69 6365  odified BSD Lice
+00089f10: 6e73 652e 0a20 207c 2d2d 2d2d 2d2d 2d2d  nse..  |--------
 00089f20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00089f30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00089f40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00089f50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2a2f  --------------*/
-00089f60: 0a20 200a 2020 2f2a 2d2d 2d2d 2d2d 2d2d  .  .  /*--------
+00089f50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00089f60: 2d2d 2d2d 2a2f 0a20 200a 2020 2f2a 2d2d  ----*/.  .  /*--
 00089f70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00089f80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00089f90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00089fa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00089fb0: 2d2d 2d2d 2d0a 2020 7c20 5072 6976 6174  -----.  | Privat
-00089fc0: 6520 4353 5320 7661 7269 6162 6c65 730a  e CSS variables.
-00089fd0: 2020 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    |-------------
+00089fb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 7c20  -----------.  | 
+00089fc0: 5072 6976 6174 6520 4353 5320 7661 7269  Private CSS vari
+00089fd0: 6162 6c65 730a 2020 7c2d 2d2d 2d2d 2d2d  ables.  |-------
 00089fe0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00089ff0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008a000: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008a010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2a  ---------------*
-0008a020: 2f0a 2020 0a20 203a 726f 6f74 207b 0a20  /.  .  :root {. 
-0008a030: 2020 202d 2d6a 702d 7072 6976 6174 652d     --jp-private-
-0008a040: 6365 6c6c 2d73 6372 6f6c 6c69 6e67 2d6f  cell-scrolling-o
-0008a050: 7574 7075 742d 6f66 6673 6574 3a20 3570  utput-offset: 5p
-0008a060: 783b 0a20 207d 0a20 200a 2020 2f2a 2d2d  x;.  }.  .  /*--
-0008a070: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0008a010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0008a020: 2d2d 2d2d 2d2a 2f0a 2020 0a20 203a 726f  -----*/.  .  :ro
+0008a030: 6f74 207b 0a20 2020 202d 2d6a 702d 7072  ot {.    --jp-pr
+0008a040: 6976 6174 652d 6365 6c6c 2d73 6372 6f6c  ivate-cell-scrol
+0008a050: 6c69 6e67 2d6f 7574 7075 742d 6f66 6673  ling-output-offs
+0008a060: 6574 3a20 3570 783b 0a20 207d 0a20 200a  et: 5px;.  }.  .
+0008a070: 2020 2f2a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    /*------------
 0008a080: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008a090: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008a0a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008a0b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 7c20  -----------.  | 
-0008a0c0: 4365 6c6c 0a20 207c 2d2d 2d2d 2d2d 2d2d  Cell.  |--------
+0008a0b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0008a0c0: 2d0a 2020 7c20 4365 6c6c 0a20 207c 2d2d  -.  | Cell.  |--
 0008a0d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008a0e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008a0f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008a100: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008a110: 2d2d 2d2d 2a2f 0a20 200a 2020 2e6a 702d  ----*/.  .  .jp-
-0008a120: 4365 6c6c 207b 0a20 2020 2070 6164 6469  Cell {.    paddi
-0008a130: 6e67 3a20 7661 7228 2d2d 6a70 2d63 656c  ng: var(--jp-cel
-0008a140: 6c2d 7061 6464 696e 6729 3b0a 2020 2020  l-padding);.    
-0008a150: 6d61 7267 696e 3a20 3070 783b 0a20 2020  margin: 0px;.   
-0008a160: 2062 6f72 6465 723a 206e 6f6e 653b 0a20   border: none;. 
-0008a170: 2020 206f 7574 6c69 6e65 3a20 6e6f 6e65     outline: none
-0008a180: 3b0a 2020 2020 6261 636b 6772 6f75 6e64  ;.    background
-0008a190: 3a20 7472 616e 7370 6172 656e 743b 0a20  : transparent;. 
-0008a1a0: 207d 0a20 200a 2020 2f2a 2d2d 2d2d 2d2d   }.  .  /*------
+0008a110: 2d2d 2d2d 2d2d 2d2d 2d2d 2a2f 0a20 200a  ----------*/.  .
+0008a120: 2020 2e6a 702d 4365 6c6c 207b 0a20 2020    .jp-Cell {.   
+0008a130: 2070 6164 6469 6e67 3a20 7661 7228 2d2d   padding: var(--
+0008a140: 6a70 2d63 656c 6c2d 7061 6464 696e 6729  jp-cell-padding)
+0008a150: 3b0a 2020 2020 6d61 7267 696e 3a20 3070  ;.    margin: 0p
+0008a160: 783b 0a20 2020 2062 6f72 6465 723a 206e  x;.    border: n
+0008a170: 6f6e 653b 0a20 2020 206f 7574 6c69 6e65  one;.    outline
+0008a180: 3a20 6e6f 6e65 3b0a 2020 2020 6261 636b  : none;.    back
+0008a190: 6772 6f75 6e64 3a20 7472 616e 7370 6172  ground: transpar
+0008a1a0: 656e 743b 0a20 207d 0a20 200a 2020 2f2a  ent;.  }.  .  /*
 0008a1b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008a1c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008a1d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008a1e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008a1f0: 2d2d 2d2d 2d2d 2d0a 2020 7c20 436f 6d6d  -------.  | Comm
-0008a200: 6f6e 2069 6e70 7574 2f6f 7574 7075 740a  on input/output.
-0008a210: 2020 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    |-------------
+0008a1f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
+0008a200: 7c20 436f 6d6d 6f6e 2069 6e70 7574 2f6f  | Common input/o
+0008a210: 7574 7075 740a 2020 7c2d 2d2d 2d2d 2d2d  utput.  |-------
 0008a220: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008a230: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008a240: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008a250: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2a  ---------------*
-0008a260: 2f0a 2020 0a20 202e 6a70 2d43 656c 6c2d  /.  .  .jp-Cell-
-0008a270: 696e 7075 7457 7261 7070 6572 2c0a 2020  inputWrapper,.  
-0008a280: 2e6a 702d 4365 6c6c 2d6f 7574 7075 7457  .jp-Cell-outputW
-0008a290: 7261 7070 6572 207b 0a20 2020 2064 6973  rapper {.    dis
-0008a2a0: 706c 6179 3a20 666c 6578 3b0a 2020 2020  play: flex;.    
-0008a2b0: 666c 6578 2d64 6972 6563 7469 6f6e 3a20  flex-direction: 
-0008a2c0: 726f 773b 0a20 2020 2070 6164 6469 6e67  row;.    padding
-0008a2d0: 3a20 3070 783b 0a20 2020 206d 6172 6769  : 0px;.    margi
-0008a2e0: 6e3a 2030 7078 3b0a 2020 2020 2f2a 2041  n: 0px;.    /* A
-0008a2f0: 6464 6564 2074 6f20 7265 7665 616c 2074  dded to reveal t
-0008a300: 6865 2062 6f78 2d73 6861 646f 7720 6f6e  he box-shadow on
-0008a310: 2074 6865 2069 6e70 7574 2061 6e64 206f   the input and o
-0008a320: 7574 7075 7420 636f 6c6c 6170 7365 7273  utput collapsers
-0008a330: 2e20 2a2f 0a20 2020 206f 7665 7266 6c6f  . */.    overflo
-0008a340: 773a 2076 6973 6962 6c65 3b0a 2020 7d0a  w: visible;.  }.
-0008a350: 2020 0a20 202f 2a20 4f6e 6c79 2069 6e70    .  /* Only inp
-0008a360: 7574 2f6f 7574 7075 7420 6172 6561 7320  ut/output areas 
-0008a370: 696e 7369 6465 2063 656c 6c73 202a 2f0a  inside cells */.
-0008a380: 2020 2e6a 702d 4365 6c6c 2d69 6e70 7574    .jp-Cell-input
-0008a390: 4172 6561 2c0a 2020 2e6a 702d 4365 6c6c  Area,.  .jp-Cell
-0008a3a0: 2d6f 7574 7075 7441 7265 6120 7b0a 2020  -outputArea {.  
-0008a3b0: 2020 666c 6578 3a20 3120 3120 6175 746f    flex: 1 1 auto
-0008a3c0: 3b0a 2020 7d0a 2020 0a20 202f 2a2d 2d2d  ;.  }.  .  /*---
-0008a3d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0008a250: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0008a260: 2d2d 2d2d 2d2a 2f0a 2020 0a20 202e 6a70  -----*/.  .  .jp
+0008a270: 2d43 656c 6c2d 696e 7075 7457 7261 7070  -Cell-inputWrapp
+0008a280: 6572 2c0a 2020 2e6a 702d 4365 6c6c 2d6f  er,.  .jp-Cell-o
+0008a290: 7574 7075 7457 7261 7070 6572 207b 0a20  utputWrapper {. 
+0008a2a0: 2020 2064 6973 706c 6179 3a20 666c 6578     display: flex
+0008a2b0: 3b0a 2020 2020 666c 6578 2d64 6972 6563  ;.    flex-direc
+0008a2c0: 7469 6f6e 3a20 726f 773b 0a20 2020 2070  tion: row;.    p
+0008a2d0: 6164 6469 6e67 3a20 3070 783b 0a20 2020  adding: 0px;.   
+0008a2e0: 206d 6172 6769 6e3a 2030 7078 3b0a 2020   margin: 0px;.  
+0008a2f0: 2020 2f2a 2041 6464 6564 2074 6f20 7265    /* Added to re
+0008a300: 7665 616c 2074 6865 2062 6f78 2d73 6861  veal the box-sha
+0008a310: 646f 7720 6f6e 2074 6865 2069 6e70 7574  dow on the input
+0008a320: 2061 6e64 206f 7574 7075 7420 636f 6c6c   and output coll
+0008a330: 6170 7365 7273 2e20 2a2f 0a20 2020 206f  apsers. */.    o
+0008a340: 7665 7266 6c6f 773a 2076 6973 6962 6c65  verflow: visible
+0008a350: 3b0a 2020 7d0a 2020 0a20 202f 2a20 4f6e  ;.  }.  .  /* On
+0008a360: 6c79 2069 6e70 7574 2f6f 7574 7075 7420  ly input/output 
+0008a370: 6172 6561 7320 696e 7369 6465 2063 656c  areas inside cel
+0008a380: 6c73 202a 2f0a 2020 2e6a 702d 4365 6c6c  ls */.  .jp-Cell
+0008a390: 2d69 6e70 7574 4172 6561 2c0a 2020 2e6a  -inputArea,.  .j
+0008a3a0: 702d 4365 6c6c 2d6f 7574 7075 7441 7265  p-Cell-outputAre
+0008a3b0: 6120 7b0a 2020 2020 666c 6578 3a20 3120  a {.    flex: 1 
+0008a3c0: 3120 6175 746f 3b0a 2020 7d0a 2020 0a20  1 auto;.  }.  . 
+0008a3d0: 202f 2a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   /*-------------
 0008a3e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008a3f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008a400: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008a410: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 207c 2043  ----------.  | C
-0008a420: 6f6c 6c61 7073 6572 0a20 207c 2d2d 2d2d  ollapser.  |----
-0008a430: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0008a410: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0008a420: 0a20 207c 2043 6f6c 6c61 7073 6572 0a20  .  | Collapser. 
+0008a430: 207c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |--------------
 0008a440: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008a450: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008a460: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008a470: 2d2d 2d2d 2d2d 2d2d 2a2f 0a20 200a 2020  --------*/.  .  
-0008a480: 2f2a 204d 616b 6520 7468 6520 6f75 7470  /* Make the outp
-0008a490: 7574 2063 6f6c 6c61 7073 6572 2064 6973  ut collapser dis
-0008a4a0: 6170 7065 6172 2077 6865 6e20 7468 6572  appear when ther
-0008a4b0: 6520 6973 206e 6f74 206f 7574 7075 742c  e is not output,
-0008a4c0: 2062 7574 2064 6f20 736f 0a20 2020 2a20   but do so.   * 
-0008a4d0: 696e 2061 206d 616e 6e65 7220 7468 6174  in a manner that
-0008a4e0: 206c 6561 7665 7320 6974 2069 6e20 7468   leaves it in th
-0008a4f0: 6520 6c61 796f 7574 2061 6e64 2070 7265  e layout and pre
-0008a500: 7365 7276 6573 2069 7473 2077 6964 7468  serves its width
-0008a510: 2e0a 2020 202a 2f0a 2020 2e6a 702d 4365  ..   */.  .jp-Ce
-0008a520: 6c6c 2e6a 702d 6d6f 642d 6e6f 4f75 7470  ll.jp-mod-noOutp
-0008a530: 7574 7320 2e6a 702d 4365 6c6c 2d6f 7574  uts .jp-Cell-out
-0008a540: 7075 7443 6f6c 6c61 7073 6572 207b 0a20  putCollapser {. 
-0008a550: 2020 2062 6f72 6465 723a 206e 6f6e 6520     border: none 
-0008a560: 2169 6d70 6f72 7461 6e74 3b0a 2020 2020  !important;.    
-0008a570: 6261 636b 6772 6f75 6e64 3a20 7472 616e  background: tran
-0008a580: 7370 6172 656e 7420 2169 6d70 6f72 7461  sparent !importa
-0008a590: 6e74 3b0a 2020 7d0a 2020 0a20 202e 6a70  nt;.  }.  .  .jp
-0008a5a0: 2d43 656c 6c3a 6e6f 7428 2e6a 702d 6d6f  -Cell:not(.jp-mo
-0008a5b0: 642d 6e6f 4f75 7470 7574 7329 202e 6a70  d-noOutputs) .jp
-0008a5c0: 2d43 656c 6c2d 6f75 7470 7574 436f 6c6c  -Cell-outputColl
-0008a5d0: 6170 7365 7220 7b0a 2020 2020 6d69 6e2d  apser {.    min-
-0008a5e0: 6865 6967 6874 3a20 7661 7228 2d2d 6a70  height: var(--jp
-0008a5f0: 2d63 656c 6c2d 636f 6c6c 6170 7365 722d  -cell-collapser-
-0008a600: 6d69 6e2d 6865 6967 6874 293b 0a20 207d  min-height);.  }
-0008a610: 0a20 200a 2020 2f2a 2d2d 2d2d 2d2d 2d2d  .  .  /*--------
+0008a470: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2a2f  --------------*/
+0008a480: 0a20 200a 2020 2f2a 204d 616b 6520 7468  .  .  /* Make th
+0008a490: 6520 6f75 7470 7574 2063 6f6c 6c61 7073  e output collaps
+0008a4a0: 6572 2064 6973 6170 7065 6172 2077 6865  er disappear whe
+0008a4b0: 6e20 7468 6572 6520 6973 206e 6f74 206f  n there is not o
+0008a4c0: 7574 7075 742c 2062 7574 2064 6f20 736f  utput, but do so
+0008a4d0: 0a20 2020 2a20 696e 2061 206d 616e 6e65  .   * in a manne
+0008a4e0: 7220 7468 6174 206c 6561 7665 7320 6974  r that leaves it
+0008a4f0: 2069 6e20 7468 6520 6c61 796f 7574 2061   in the layout a
+0008a500: 6e64 2070 7265 7365 7276 6573 2069 7473  nd preserves its
+0008a510: 2077 6964 7468 2e0a 2020 202a 2f0a 2020   width..   */.  
+0008a520: 2e6a 702d 4365 6c6c 2e6a 702d 6d6f 642d  .jp-Cell.jp-mod-
+0008a530: 6e6f 4f75 7470 7574 7320 2e6a 702d 4365  noOutputs .jp-Ce
+0008a540: 6c6c 2d6f 7574 7075 7443 6f6c 6c61 7073  ll-outputCollaps
+0008a550: 6572 207b 0a20 2020 2062 6f72 6465 723a  er {.    border:
+0008a560: 206e 6f6e 6520 2169 6d70 6f72 7461 6e74   none !important
+0008a570: 3b0a 2020 2020 6261 636b 6772 6f75 6e64  ;.    background
+0008a580: 3a20 7472 616e 7370 6172 656e 7420 2169  : transparent !i
+0008a590: 6d70 6f72 7461 6e74 3b0a 2020 7d0a 2020  mportant;.  }.  
+0008a5a0: 0a20 202e 6a70 2d43 656c 6c3a 6e6f 7428  .  .jp-Cell:not(
+0008a5b0: 2e6a 702d 6d6f 642d 6e6f 4f75 7470 7574  .jp-mod-noOutput
+0008a5c0: 7329 202e 6a70 2d43 656c 6c2d 6f75 7470  s) .jp-Cell-outp
+0008a5d0: 7574 436f 6c6c 6170 7365 7220 7b0a 2020  utCollapser {.  
+0008a5e0: 2020 6d69 6e2d 6865 6967 6874 3a20 7661    min-height: va
+0008a5f0: 7228 2d2d 6a70 2d63 656c 6c2d 636f 6c6c  r(--jp-cell-coll
+0008a600: 6170 7365 722d 6d69 6e2d 6865 6967 6874  apser-min-height
+0008a610: 293b 0a20 207d 0a20 200a 2020 2f2a 2d2d  );.  }.  .  /*--
 0008a620: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008a630: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008a640: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008a650: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008a660: 2d2d 2d2d 2d0a 2020 7c20 4f75 7470 7574  -----.  | Output
-0008a670: 0a20 207c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .  |------------
+0008a660: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 7c20  -----------.  | 
+0008a670: 4f75 7470 7574 0a20 207c 2d2d 2d2d 2d2d  Output.  |------
 0008a680: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008a690: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008a6a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008a6b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008a6c0: 2a2f 0a20 200a 2020 2f2a 2050 7574 2061  */.  .  /* Put a
-0008a6d0: 2073 7061 6365 2062 6574 7765 656e 2069   space between i
-0008a6e0: 6e70 7574 2061 6e64 206f 7574 7075 7420  nput and output 
-0008a6f0: 7768 656e 2074 6865 7265 2049 5320 6f75  when there IS ou
-0008a700: 7470 7574 202a 2f0a 2020 2e6a 702d 4365  tput */.  .jp-Ce
-0008a710: 6c6c 3a6e 6f74 282e 6a70 2d6d 6f64 2d6e  ll:not(.jp-mod-n
-0008a720: 6f4f 7574 7075 7473 2920 2e6a 702d 4365  oOutputs) .jp-Ce
-0008a730: 6c6c 2d6f 7574 7075 7457 7261 7070 6572  ll-outputWrapper
-0008a740: 207b 0a20 2020 206d 6172 6769 6e2d 746f   {.    margin-to
-0008a750: 703a 2035 7078 3b0a 2020 7d0a 2020 0a20  p: 5px;.  }.  . 
-0008a760: 202e 6a70 2d43 6f64 6543 656c 6c2e 6a70   .jp-CodeCell.jp
-0008a770: 2d6d 6f64 2d6f 7574 7075 7473 5363 726f  -mod-outputsScro
-0008a780: 6c6c 6564 202e 6a70 2d43 656c 6c2d 6f75  lled .jp-Cell-ou
-0008a790: 7470 7574 4172 6561 207b 0a20 2020 206f  tputArea {.    o
-0008a7a0: 7665 7266 6c6f 772d 793a 2061 7574 6f3b  verflow-y: auto;
-0008a7b0: 0a20 2020 206d 6178 2d68 6569 6768 743a  .    max-height:
-0008a7c0: 2032 3030 7078 3b0a 2020 2020 626f 782d   200px;.    box-
-0008a7d0: 7368 6164 6f77 3a20 696e 7365 7420 3020  shadow: inset 0 
-0008a7e0: 3020 3670 7820 3270 7820 7267 6261 2830  0 6px 2px rgba(0
-0008a7f0: 2c20 302c 2030 2c20 302e 3329 3b0a 2020  , 0, 0, 0.3);.  
-0008a800: 2020 6d61 7267 696e 2d6c 6566 743a 2076    margin-left: v
-0008a810: 6172 282d 2d6a 702d 7072 6976 6174 652d  ar(--jp-private-
-0008a820: 6365 6c6c 2d73 6372 6f6c 6c69 6e67 2d6f  cell-scrolling-o
-0008a830: 7574 7075 742d 6f66 6673 6574 293b 0a20  utput-offset);. 
-0008a840: 207d 0a20 200a 2020 2e6a 702d 436f 6465   }.  .  .jp-Code
-0008a850: 4365 6c6c 2e6a 702d 6d6f 642d 6f75 7470  Cell.jp-mod-outp
-0008a860: 7574 7353 6372 6f6c 6c65 6420 2e6a 702d  utsScrolled .jp-
-0008a870: 4f75 7470 7574 4172 6561 2d70 726f 6d70  OutputArea-promp
-0008a880: 7420 7b0a 2020 2020 666c 6578 3a20 3020  t {.    flex: 0 
-0008a890: 300a 2020 2020 2020 6361 6c63 280a 2020  0.      calc(.  
-0008a8a0: 2020 2020 2020 7661 7228 2d2d 6a70 2d63        var(--jp-c
-0008a8b0: 656c 6c2d 7072 6f6d 7074 2d77 6964 7468  ell-prompt-width
-0008a8c0: 2920 2d0a 2020 2020 2020 2020 2020 7661  ) -.          va
-0008a8d0: 7228 2d2d 6a70 2d70 7269 7661 7465 2d63  r(--jp-private-c
-0008a8e0: 656c 6c2d 7363 726f 6c6c 696e 672d 6f75  ell-scrolling-ou
-0008a8f0: 7470 7574 2d6f 6666 7365 7429 0a20 2020  tput-offset).   
-0008a900: 2020 2029 3b0a 2020 7d0a 2020 0a20 202f     );.  }.  .  /
-0008a910: 2a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  *---------------
+0008a6c0: 2d2d 2d2d 2d2d 2a2f 0a20 200a 2020 2f2a  ------*/.  .  /*
+0008a6d0: 2050 7574 2061 2073 7061 6365 2062 6574   Put a space bet
+0008a6e0: 7765 656e 2069 6e70 7574 2061 6e64 206f  ween input and o
+0008a6f0: 7574 7075 7420 7768 656e 2074 6865 7265  utput when there
+0008a700: 2049 5320 6f75 7470 7574 202a 2f0a 2020   IS output */.  
+0008a710: 2e6a 702d 4365 6c6c 3a6e 6f74 282e 6a70  .jp-Cell:not(.jp
+0008a720: 2d6d 6f64 2d6e 6f4f 7574 7075 7473 2920  -mod-noOutputs) 
+0008a730: 2e6a 702d 4365 6c6c 2d6f 7574 7075 7457  .jp-Cell-outputW
+0008a740: 7261 7070 6572 207b 0a20 2020 206d 6172  rapper {.    mar
+0008a750: 6769 6e2d 746f 703a 2035 7078 3b0a 2020  gin-top: 5px;.  
+0008a760: 7d0a 2020 0a20 202e 6a70 2d43 6f64 6543  }.  .  .jp-CodeC
+0008a770: 656c 6c2e 6a70 2d6d 6f64 2d6f 7574 7075  ell.jp-mod-outpu
+0008a780: 7473 5363 726f 6c6c 6564 202e 6a70 2d43  tsScrolled .jp-C
+0008a790: 656c 6c2d 6f75 7470 7574 4172 6561 207b  ell-outputArea {
+0008a7a0: 0a20 2020 206f 7665 7266 6c6f 772d 793a  .    overflow-y:
+0008a7b0: 2061 7574 6f3b 0a20 2020 206d 6178 2d68   auto;.    max-h
+0008a7c0: 6569 6768 743a 2032 3030 7078 3b0a 2020  eight: 200px;.  
+0008a7d0: 2020 626f 782d 7368 6164 6f77 3a20 696e    box-shadow: in
+0008a7e0: 7365 7420 3020 3020 3670 7820 3270 7820  set 0 0 6px 2px 
+0008a7f0: 7267 6261 2830 2c20 302c 2030 2c20 302e  rgba(0, 0, 0, 0.
+0008a800: 3329 3b0a 2020 2020 6d61 7267 696e 2d6c  3);.    margin-l
+0008a810: 6566 743a 2076 6172 282d 2d6a 702d 7072  eft: var(--jp-pr
+0008a820: 6976 6174 652d 6365 6c6c 2d73 6372 6f6c  ivate-cell-scrol
+0008a830: 6c69 6e67 2d6f 7574 7075 742d 6f66 6673  ling-output-offs
+0008a840: 6574 293b 0a20 207d 0a20 200a 2020 2e6a  et);.  }.  .  .j
+0008a850: 702d 436f 6465 4365 6c6c 2e6a 702d 6d6f  p-CodeCell.jp-mo
+0008a860: 642d 6f75 7470 7574 7353 6372 6f6c 6c65  d-outputsScrolle
+0008a870: 6420 2e6a 702d 4f75 7470 7574 4172 6561  d .jp-OutputArea
+0008a880: 2d70 726f 6d70 7420 7b0a 2020 2020 666c  -prompt {.    fl
+0008a890: 6578 3a20 3020 300a 2020 2020 2020 6361  ex: 0 0.      ca
+0008a8a0: 6c63 280a 2020 2020 2020 2020 7661 7228  lc(.        var(
+0008a8b0: 2d2d 6a70 2d63 656c 6c2d 7072 6f6d 7074  --jp-cell-prompt
+0008a8c0: 2d77 6964 7468 2920 2d0a 2020 2020 2020  -width) -.      
+0008a8d0: 2020 2020 7661 7228 2d2d 6a70 2d70 7269      var(--jp-pri
+0008a8e0: 7661 7465 2d63 656c 6c2d 7363 726f 6c6c  vate-cell-scroll
+0008a8f0: 696e 672d 6f75 7470 7574 2d6f 6666 7365  ing-output-offse
+0008a900: 7429 0a20 2020 2020 2029 3b0a 2020 7d0a  t).      );.  }.
+0008a910: 2020 0a20 202f 2a2d 2d2d 2d2d 2d2d 2d2d    .  /*---------
 0008a920: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008a930: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008a940: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008a950: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
-0008a960: 207c 2043 6f64 6543 656c 6c0a 2020 7c2d   | CodeCell.  |-
-0008a970: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0008a950: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0008a960: 2d2d 2d2d 0a20 207c 2043 6f64 6543 656c  ----.  | CodeCel
+0008a970: 6c0a 2020 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d  l.  |-----------
 0008a980: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008a990: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008a9a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008a9b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2a 2f0a 2020  -----------*/.  
-0008a9c0: 0a20 202f 2a2d 2d2d 2d2d 2d2d 2d2d 2d2d  .  /*-----------
+0008a9b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0008a9c0: 2d2a 2f0a 2020 0a20 202f 2a2d 2d2d 2d2d  -*/.  .  /*-----
 0008a9d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008a9e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008a9f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008aa00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008aa10: 2d2d 0a20 207c 204d 6172 6b64 6f77 6e43  --.  | MarkdownC
-0008aa20: 656c 6c0a 2020 7c2d 2d2d 2d2d 2d2d 2d2d  ell.  |---------
+0008aa10: 2d2d 2d2d 2d2d 2d2d 0a20 207c 204d 6172  --------.  | Mar
+0008aa20: 6b64 6f77 6e43 656c 6c0a 2020 7c2d 2d2d  kdownCell.  |---
 0008aa30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008aa40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008aa50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008aa60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008aa70: 2d2d 2d2a 2f0a 2020 0a20 202e 6a70 2d4d  ---*/.  .  .jp-M
-0008aa80: 6172 6b64 6f77 6e4f 7574 7075 7420 7b0a  arkdownOutput {.
-0008aa90: 2020 2020 666c 6578 3a20 3120 3120 6175      flex: 1 1 au
-0008aaa0: 746f 3b0a 2020 2020 6d61 7267 696e 2d74  to;.    margin-t
-0008aab0: 6f70 3a20 303b 0a20 2020 206d 6172 6769  op: 0;.    margi
-0008aac0: 6e2d 626f 7474 6f6d 3a20 303b 0a20 2020  n-bottom: 0;.   
-0008aad0: 2070 6164 6469 6e67 2d6c 6566 743a 2076   padding-left: v
-0008aae0: 6172 282d 2d6a 702d 636f 6465 2d70 6164  ar(--jp-code-pad
-0008aaf0: 6469 6e67 293b 0a20 207d 0a20 200a 2020  ding);.  }.  .  
-0008ab00: 2e6a 702d 4d61 726b 646f 776e 4f75 7470  .jp-MarkdownOutp
-0008ab10: 7574 2e6a 702d 5265 6e64 6572 6564 4854  ut.jp-RenderedHT
-0008ab20: 4d4c 436f 6d6d 6f6e 207b 0a20 2020 206f  MLCommon {.    o
-0008ab30: 7665 7266 6c6f 773a 2061 7574 6f3b 0a20  verflow: auto;. 
-0008ab40: 207d 0a20 200a 2020 2e6a 702d 7368 6f77   }.  .  .jp-show
-0008ab50: 4869 6464 656e 4365 6c6c 7342 7574 746f  HiddenCellsButto
-0008ab60: 6e20 7b0a 2020 2020 6d61 7267 696e 2d6c  n {.    margin-l
-0008ab70: 6566 743a 2063 616c 6328 7661 7228 2d2d  eft: calc(var(--
-0008ab80: 6a70 2d63 656c 6c2d 7072 6f6d 7074 2d77  jp-cell-prompt-w
-0008ab90: 6964 7468 2920 2b20 3220 2a20 7661 7228  idth) + 2 * var(
-0008aba0: 2d2d 6a70 2d63 6f64 652d 7061 6464 696e  --jp-code-paddin
-0008abb0: 6729 293b 0a20 2020 206d 6172 6769 6e2d  g));.    margin-
-0008abc0: 746f 703a 2076 6172 282d 2d6a 702d 636f  top: var(--jp-co
-0008abd0: 6465 2d70 6164 6469 6e67 293b 0a20 2020  de-padding);.   
-0008abe0: 2062 6f72 6465 723a 2031 7078 2073 6f6c   border: 1px sol
-0008abf0: 6964 2076 6172 282d 2d6a 702d 626f 7264  id var(--jp-bord
-0008ac00: 6572 2d63 6f6c 6f72 3229 3b0a 2020 2020  er-color2);.    
-0008ac10: 6261 636b 6772 6f75 6e64 2d63 6f6c 6f72  background-color
-0008ac20: 3a20 7661 7228 2d2d 6a70 2d62 6f72 6465  : var(--jp-borde
-0008ac30: 722d 636f 6c6f 7233 2920 2169 6d70 6f72  r-color3) !impor
-0008ac40: 7461 6e74 3b0a 2020 2020 636f 6c6f 723a  tant;.    color:
-0008ac50: 2076 6172 282d 2d6a 702d 636f 6e74 656e   var(--jp-conten
-0008ac60: 742d 666f 6e74 2d63 6f6c 6f72 3029 2021  t-font-color0) !
-0008ac70: 696d 706f 7274 616e 743b 0a20 207d 0a20  important;.  }. 
-0008ac80: 200a 2020 2e6a 702d 7368 6f77 4869 6464   .  .jp-showHidd
-0008ac90: 656e 4365 6c6c 7342 7574 746f 6e3a 686f  enCellsButton:ho
-0008aca0: 7665 7220 7b0a 2020 2020 6261 636b 6772  ver {.    backgr
-0008acb0: 6f75 6e64 2d63 6f6c 6f72 3a20 7661 7228  ound-color: var(
-0008acc0: 2d2d 6a70 2d62 6f72 6465 722d 636f 6c6f  --jp-border-colo
-0008acd0: 7232 2920 2169 6d70 6f72 7461 6e74 3b0a  r2) !important;.
-0008ace0: 2020 7d0a 2020 0a20 202e 6a70 2d63 6f6c    }.  .  .jp-col
-0008acf0: 6c61 7073 6548 6561 6469 6e67 4275 7474  lapseHeadingButt
-0008ad00: 6f6e 207b 0a20 2020 2064 6973 706c 6179  on {.    display
-0008ad10: 3a20 6e6f 6e65 3b0a 2020 7d0a 2020 0a20  : none;.  }.  . 
-0008ad20: 202e 6a70 2d4d 6172 6b64 6f77 6e43 656c   .jp-MarkdownCel
-0008ad30: 6c3a 686f 7665 7220 2e6a 702d 636f 6c6c  l:hover .jp-coll
-0008ad40: 6170 7365 4865 6164 696e 6742 7574 746f  apseHeadingButto
-0008ad50: 6e20 7b0a 2020 2020 6469 7370 6c61 793a  n {.    display:
-0008ad60: 2066 6c65 783b 0a20 2020 206d 696e 2d68   flex;.    min-h
-0008ad70: 6569 6768 743a 2076 6172 282d 2d6a 702d  eight: var(--jp-
-0008ad80: 6365 6c6c 2d63 6f6c 6c61 7073 6572 2d6d  cell-collapser-m
-0008ad90: 696e 2d68 6569 6768 7429 3b0a 2020 2020  in-height);.    
-0008ada0: 706f 7369 7469 6f6e 3a20 6162 736f 6c75  position: absolu
-0008adb0: 7465 3b0a 2020 2020 7269 6768 743a 2030  te;.    right: 0
-0008adc0: 3b0a 2020 2020 746f 703a 2030 3b0a 2020  ;.    top: 0;.  
-0008add0: 2020 626f 7474 6f6d 3a20 303b 0a20 207d    bottom: 0;.  }
-0008ade0: 0a20 200a 2020 2f2a 2d2d 2d2d 2d2d 2d2d  .  .  /*--------
+0008aa70: 2d2d 2d2d 2d2d 2d2d 2d2a 2f0a 2020 0a20  ---------*/.  . 
+0008aa80: 202e 6a70 2d4d 6172 6b64 6f77 6e4f 7574   .jp-MarkdownOut
+0008aa90: 7075 7420 7b0a 2020 2020 666c 6578 3a20  put {.    flex: 
+0008aaa0: 3120 3120 6175 746f 3b0a 2020 2020 6d61  1 1 auto;.    ma
+0008aab0: 7267 696e 2d74 6f70 3a20 303b 0a20 2020  rgin-top: 0;.   
+0008aac0: 206d 6172 6769 6e2d 626f 7474 6f6d 3a20   margin-bottom: 
+0008aad0: 303b 0a20 2020 2070 6164 6469 6e67 2d6c  0;.    padding-l
+0008aae0: 6566 743a 2076 6172 282d 2d6a 702d 636f  eft: var(--jp-co
+0008aaf0: 6465 2d70 6164 6469 6e67 293b 0a20 207d  de-padding);.  }
+0008ab00: 0a20 200a 2020 2e6a 702d 4d61 726b 646f  .  .  .jp-Markdo
+0008ab10: 776e 4f75 7470 7574 2e6a 702d 5265 6e64  wnOutput.jp-Rend
+0008ab20: 6572 6564 4854 4d4c 436f 6d6d 6f6e 207b  eredHTMLCommon {
+0008ab30: 0a20 2020 206f 7665 7266 6c6f 773a 2061  .    overflow: a
+0008ab40: 7574 6f3b 0a20 207d 0a20 200a 2020 2e6a  uto;.  }.  .  .j
+0008ab50: 702d 7368 6f77 4869 6464 656e 4365 6c6c  p-showHiddenCell
+0008ab60: 7342 7574 746f 6e20 7b0a 2020 2020 6d61  sButton {.    ma
+0008ab70: 7267 696e 2d6c 6566 743a 2063 616c 6328  rgin-left: calc(
+0008ab80: 7661 7228 2d2d 6a70 2d63 656c 6c2d 7072  var(--jp-cell-pr
+0008ab90: 6f6d 7074 2d77 6964 7468 2920 2b20 3220  ompt-width) + 2 
+0008aba0: 2a20 7661 7228 2d2d 6a70 2d63 6f64 652d  * var(--jp-code-
+0008abb0: 7061 6464 696e 6729 293b 0a20 2020 206d  padding));.    m
+0008abc0: 6172 6769 6e2d 746f 703a 2076 6172 282d  argin-top: var(-
+0008abd0: 2d6a 702d 636f 6465 2d70 6164 6469 6e67  -jp-code-padding
+0008abe0: 293b 0a20 2020 2062 6f72 6465 723a 2031  );.    border: 1
+0008abf0: 7078 2073 6f6c 6964 2076 6172 282d 2d6a  px solid var(--j
+0008ac00: 702d 626f 7264 6572 2d63 6f6c 6f72 3229  p-border-color2)
+0008ac10: 3b0a 2020 2020 6261 636b 6772 6f75 6e64  ;.    background
+0008ac20: 2d63 6f6c 6f72 3a20 7661 7228 2d2d 6a70  -color: var(--jp
+0008ac30: 2d62 6f72 6465 722d 636f 6c6f 7233 2920  -border-color3) 
+0008ac40: 2169 6d70 6f72 7461 6e74 3b0a 2020 2020  !important;.    
+0008ac50: 636f 6c6f 723a 2076 6172 282d 2d6a 702d  color: var(--jp-
+0008ac60: 636f 6e74 656e 742d 666f 6e74 2d63 6f6c  content-font-col
+0008ac70: 6f72 3029 2021 696d 706f 7274 616e 743b  or0) !important;
+0008ac80: 0a20 207d 0a20 200a 2020 2e6a 702d 7368  .  }.  .  .jp-sh
+0008ac90: 6f77 4869 6464 656e 4365 6c6c 7342 7574  owHiddenCellsBut
+0008aca0: 746f 6e3a 686f 7665 7220 7b0a 2020 2020  ton:hover {.    
+0008acb0: 6261 636b 6772 6f75 6e64 2d63 6f6c 6f72  background-color
+0008acc0: 3a20 7661 7228 2d2d 6a70 2d62 6f72 6465  : var(--jp-borde
+0008acd0: 722d 636f 6c6f 7232 2920 2169 6d70 6f72  r-color2) !impor
+0008ace0: 7461 6e74 3b0a 2020 7d0a 2020 0a20 202e  tant;.  }.  .  .
+0008acf0: 6a70 2d63 6f6c 6c61 7073 6548 6561 6469  jp-collapseHeadi
+0008ad00: 6e67 4275 7474 6f6e 207b 0a20 2020 2064  ngButton {.    d
+0008ad10: 6973 706c 6179 3a20 6e6f 6e65 3b0a 2020  isplay: none;.  
+0008ad20: 7d0a 2020 0a20 202e 6a70 2d4d 6172 6b64  }.  .  .jp-Markd
+0008ad30: 6f77 6e43 656c 6c3a 686f 7665 7220 2e6a  ownCell:hover .j
+0008ad40: 702d 636f 6c6c 6170 7365 4865 6164 696e  p-collapseHeadin
+0008ad50: 6742 7574 746f 6e20 7b0a 2020 2020 6469  gButton {.    di
+0008ad60: 7370 6c61 793a 2066 6c65 783b 0a20 2020  splay: flex;.   
+0008ad70: 206d 696e 2d68 6569 6768 743a 2076 6172   min-height: var
+0008ad80: 282d 2d6a 702d 6365 6c6c 2d63 6f6c 6c61  (--jp-cell-colla
+0008ad90: 7073 6572 2d6d 696e 2d68 6569 6768 7429  pser-min-height)
+0008ada0: 3b0a 2020 2020 706f 7369 7469 6f6e 3a20  ;.    position: 
+0008adb0: 6162 736f 6c75 7465 3b0a 2020 2020 7269  absolute;.    ri
+0008adc0: 6768 743a 2030 3b0a 2020 2020 746f 703a  ght: 0;.    top:
+0008add0: 2030 3b0a 2020 2020 626f 7474 6f6d 3a20   0;.    bottom: 
+0008ade0: 303b 0a20 207d 0a20 200a 2020 2f2a 2d2d  0;.  }.  .  /*--
 0008adf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008ae00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008ae10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008ae20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008ae30: 2d2d 2d2d 2d0a 2020 7c20 436f 7079 7269  -----.  | Copyri
-0008ae40: 6768 7420 2863 2920 4a75 7079 7465 7220  ght (c) Jupyter 
-0008ae50: 4465 7665 6c6f 706d 656e 7420 5465 616d  Development Team
-0008ae60: 2e0a 2020 7c20 4469 7374 7269 6275 7465  ..  | Distribute
-0008ae70: 6420 756e 6465 7220 7468 6520 7465 726d  d under the term
-0008ae80: 7320 6f66 2074 6865 204d 6f64 6966 6965  s of the Modifie
-0008ae90: 6420 4253 4420 4c69 6365 6e73 652e 0a20  d BSD License.. 
-0008aea0: 207c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |--------------
+0008ae30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 7c20  -----------.  | 
+0008ae40: 436f 7079 7269 6768 7420 2863 2920 4a75  Copyright (c) Ju
+0008ae50: 7079 7465 7220 4465 7665 6c6f 706d 656e  pyter Developmen
+0008ae60: 7420 5465 616d 2e0a 2020 7c20 4469 7374  t Team..  | Dist
+0008ae70: 7269 6275 7465 6420 756e 6465 7220 7468  ributed under th
+0008ae80: 6520 7465 726d 7320 6f66 2074 6865 204d  e terms of the M
+0008ae90: 6f64 6966 6965 6420 4253 4420 4c69 6365  odified BSD Lice
+0008aea0: 6e73 652e 0a20 207c 2d2d 2d2d 2d2d 2d2d  nse..  |--------
 0008aeb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008aec0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008aed0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008aee0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2a2f  --------------*/
-0008aef0: 0a20 200a 2020 2f2a 2d2d 2d2d 2d2d 2d2d  .  .  /*--------
+0008aee0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0008aef0: 2d2d 2d2d 2a2f 0a20 200a 2020 2f2a 2d2d  ----*/.  .  /*--
 0008af00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008af10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008af20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008af30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008af40: 2d2d 2d2d 2d0a 2020 7c20 436f 7079 7269  -----.  | Copyri
-0008af50: 6768 7420 2863 2920 4a75 7079 7465 7220  ght (c) Jupyter 
-0008af60: 4465 7665 6c6f 706d 656e 7420 5465 616d  Development Team
-0008af70: 2e0a 2020 7c20 4469 7374 7269 6275 7465  ..  | Distribute
-0008af80: 6420 756e 6465 7220 7468 6520 7465 726d  d under the term
-0008af90: 7320 6f66 2074 6865 204d 6f64 6966 6965  s of the Modifie
-0008afa0: 6420 4253 4420 4c69 6365 6e73 652e 0a20  d BSD License.. 
-0008afb0: 207c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |--------------
+0008af40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 7c20  -----------.  | 
+0008af50: 436f 7079 7269 6768 7420 2863 2920 4a75  Copyright (c) Ju
+0008af60: 7079 7465 7220 4465 7665 6c6f 706d 656e  pyter Developmen
+0008af70: 7420 5465 616d 2e0a 2020 7c20 4469 7374  t Team..  | Dist
+0008af80: 7269 6275 7465 6420 756e 6465 7220 7468  ributed under th
+0008af90: 6520 7465 726d 7320 6f66 2074 6865 204d  e terms of the M
+0008afa0: 6f64 6966 6965 6420 4253 4420 4c69 6365  odified BSD Lice
+0008afb0: 6e73 652e 0a20 207c 2d2d 2d2d 2d2d 2d2d  nse..  |--------
 0008afc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008afd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008afe0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008aff0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2a2f  --------------*/
-0008b000: 0a20 200a 2020 2f2a 2d2d 2d2d 2d2d 2d2d  .  .  /*--------
+0008aff0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0008b000: 2d2d 2d2d 2a2f 0a20 200a 2020 2f2a 2d2d  ----*/.  .  /*--
 0008b010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008b020: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008b030: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008b040: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008b050: 2d2d 2d2d 2d0a 2020 7c20 5661 7269 6162  -----.  | Variab
-0008b060: 6c65 730a 2020 7c2d 2d2d 2d2d 2d2d 2d2d  les.  |---------
+0008b050: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 7c20  -----------.  | 
+0008b060: 5661 7269 6162 6c65 730a 2020 7c2d 2d2d  Variables.  |---
 0008b070: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008b080: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008b090: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008b0a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008b0b0: 2d2d 2d2a 2f0a 2020 0a20 202f 2a2d 2d2d  ---*/.  .  /*---
-0008b0c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0008b0b0: 2d2d 2d2d 2d2d 2d2d 2d2a 2f0a 2020 0a20  ---------*/.  . 
+0008b0c0: 202f 2a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   /*-------------
 0008b0d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008b0e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008b0f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008b100: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 200a 2020  ----------.  .  
-0008b110: 2f2a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  /*--------------
+0008b100: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0008b110: 0a20 200a 2020 2f2a 2d2d 2d2d 2d2d 2d2d  .  .  /*--------
 0008b120: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008b130: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008b140: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008b150: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
-0008b160: 2020 7c20 5374 796c 6573 0a20 207c 2d2d    | Styles.  |--
-0008b170: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0008b150: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0008b160: 2d2d 2d2d 2d0a 2020 7c20 5374 796c 6573  -----.  | Styles
+0008b170: 0a20 207c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .  |------------
 0008b180: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008b190: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008b1a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008b1b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2a2f 0a20 200a  ----------*/.  .
-0008b1c0: 2020 2e6a 702d 4e6f 7465 626f 6f6b 5061    .jp-NotebookPa
-0008b1d0: 6e65 6c2d 746f 6f6c 6261 7220 7b0a 2020  nel-toolbar {.  
-0008b1e0: 2020 7061 6464 696e 673a 2032 7078 3b0a    padding: 2px;.
-0008b1f0: 2020 7d0a 2020 0a20 202e 6a70 2d54 6f6f    }.  .  .jp-Too
-0008b200: 6c62 6172 2d69 7465 6d2e 6a70 2d4e 6f74  lbar-item.jp-Not
-0008b210: 6562 6f6f 6b2d 746f 6f6c 6261 7243 656c  ebook-toolbarCel
-0008b220: 6c54 7970 6520 2e6a 702d 7365 6c65 6374  lType .jp-select
-0008b230: 2d77 7261 7070 6572 2e6a 702d 6d6f 642d  -wrapper.jp-mod-
-0008b240: 666f 6375 7365 6420 7b0a 2020 2020 626f  focused {.    bo
-0008b250: 7264 6572 3a20 6e6f 6e65 3b0a 2020 2020  rder: none;.    
-0008b260: 626f 782d 7368 6164 6f77 3a20 6e6f 6e65  box-shadow: none
-0008b270: 3b0a 2020 7d0a 2020 0a20 202e 6a70 2d4e  ;.  }.  .  .jp-N
-0008b280: 6f74 6562 6f6f 6b2d 746f 6f6c 6261 7243  otebook-toolbarC
-0008b290: 656c 6c54 7970 6544 726f 7064 6f77 6e20  ellTypeDropdown 
-0008b2a0: 7365 6c65 6374 207b 0a20 2020 2068 6569  select {.    hei
-0008b2b0: 6768 743a 2032 3470 783b 0a20 2020 2066  ght: 24px;.    f
-0008b2c0: 6f6e 742d 7369 7a65 3a20 7661 7228 2d2d  ont-size: var(--
-0008b2d0: 6a70 2d75 692d 666f 6e74 2d73 697a 6531  jp-ui-font-size1
-0008b2e0: 293b 0a20 2020 206c 696e 652d 6865 6967  );.    line-heig
-0008b2f0: 6874 3a20 3134 7078 3b0a 2020 2020 626f  ht: 14px;.    bo
-0008b300: 7264 6572 2d72 6164 6975 733a 2030 3b0a  rder-radius: 0;.
-0008b310: 2020 2020 6469 7370 6c61 793a 2062 6c6f      display: blo
-0008b320: 636b 3b0a 2020 7d0a 2020 0a20 202e 6a70  ck;.  }.  .  .jp
-0008b330: 2d4e 6f74 6562 6f6f 6b2d 746f 6f6c 6261  -Notebook-toolba
-0008b340: 7243 656c 6c54 7970 6544 726f 7064 6f77  rCellTypeDropdow
-0008b350: 6e20 7370 616e 207b 0a20 2020 2074 6f70  n span {.    top
-0008b360: 3a20 3570 7820 2169 6d70 6f72 7461 6e74  : 5px !important
-0008b370: 3b0a 2020 7d0a 2020 0a20 202f 2a2d 2d2d  ;.  }.  .  /*---
-0008b380: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0008b1b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0008b1c0: 2a2f 0a20 200a 2020 2e6a 702d 4e6f 7465  */.  .  .jp-Note
+0008b1d0: 626f 6f6b 5061 6e65 6c2d 746f 6f6c 6261  bookPanel-toolba
+0008b1e0: 7220 7b0a 2020 2020 7061 6464 696e 673a  r {.    padding:
+0008b1f0: 2032 7078 3b0a 2020 7d0a 2020 0a20 202e   2px;.  }.  .  .
+0008b200: 6a70 2d54 6f6f 6c62 6172 2d69 7465 6d2e  jp-Toolbar-item.
+0008b210: 6a70 2d4e 6f74 6562 6f6f 6b2d 746f 6f6c  jp-Notebook-tool
+0008b220: 6261 7243 656c 6c54 7970 6520 2e6a 702d  barCellType .jp-
+0008b230: 7365 6c65 6374 2d77 7261 7070 6572 2e6a  select-wrapper.j
+0008b240: 702d 6d6f 642d 666f 6375 7365 6420 7b0a  p-mod-focused {.
+0008b250: 2020 2020 626f 7264 6572 3a20 6e6f 6e65      border: none
+0008b260: 3b0a 2020 2020 626f 782d 7368 6164 6f77  ;.    box-shadow
+0008b270: 3a20 6e6f 6e65 3b0a 2020 7d0a 2020 0a20  : none;.  }.  . 
+0008b280: 202e 6a70 2d4e 6f74 6562 6f6f 6b2d 746f   .jp-Notebook-to
+0008b290: 6f6c 6261 7243 656c 6c54 7970 6544 726f  olbarCellTypeDro
+0008b2a0: 7064 6f77 6e20 7365 6c65 6374 207b 0a20  pdown select {. 
+0008b2b0: 2020 2068 6569 6768 743a 2032 3470 783b     height: 24px;
+0008b2c0: 0a20 2020 2066 6f6e 742d 7369 7a65 3a20  .    font-size: 
+0008b2d0: 7661 7228 2d2d 6a70 2d75 692d 666f 6e74  var(--jp-ui-font
+0008b2e0: 2d73 697a 6531 293b 0a20 2020 206c 696e  -size1);.    lin
+0008b2f0: 652d 6865 6967 6874 3a20 3134 7078 3b0a  e-height: 14px;.
+0008b300: 2020 2020 626f 7264 6572 2d72 6164 6975      border-radiu
+0008b310: 733a 2030 3b0a 2020 2020 6469 7370 6c61  s: 0;.    displa
+0008b320: 793a 2062 6c6f 636b 3b0a 2020 7d0a 2020  y: block;.  }.  
+0008b330: 0a20 202e 6a70 2d4e 6f74 6562 6f6f 6b2d  .  .jp-Notebook-
+0008b340: 746f 6f6c 6261 7243 656c 6c54 7970 6544  toolbarCellTypeD
+0008b350: 726f 7064 6f77 6e20 7370 616e 207b 0a20  ropdown span {. 
+0008b360: 2020 2074 6f70 3a20 3570 7820 2169 6d70     top: 5px !imp
+0008b370: 6f72 7461 6e74 3b0a 2020 7d0a 2020 0a20  ortant;.  }.  . 
+0008b380: 202f 2a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   /*-------------
 0008b390: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008b3a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008b3b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008b3c0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 207c 2043  ----------.  | C
-0008b3d0: 6f70 7972 6967 6874 2028 6329 204a 7570  opyright (c) Jup
-0008b3e0: 7974 6572 2044 6576 656c 6f70 6d65 6e74  yter Development
-0008b3f0: 2054 6561 6d2e 0a20 207c 2044 6973 7472   Team..  | Distr
-0008b400: 6962 7574 6564 2075 6e64 6572 2074 6865  ibuted under the
-0008b410: 2074 6572 6d73 206f 6620 7468 6520 4d6f   terms of the Mo
-0008b420: 6469 6669 6564 2042 5344 204c 6963 656e  dified BSD Licen
-0008b430: 7365 2e0a 2020 7c2d 2d2d 2d2d 2d2d 2d2d  se..  |---------
+0008b3c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0008b3d0: 0a20 207c 2043 6f70 7972 6967 6874 2028  .  | Copyright (
+0008b3e0: 6329 204a 7570 7974 6572 2044 6576 656c  c) Jupyter Devel
+0008b3f0: 6f70 6d65 6e74 2054 6561 6d2e 0a20 207c  opment Team..  |
+0008b400: 2044 6973 7472 6962 7574 6564 2075 6e64   Distributed und
+0008b410: 6572 2074 6865 2074 6572 6d73 206f 6620  er the terms of 
+0008b420: 7468 6520 4d6f 6469 6669 6564 2042 5344  the Modified BSD
+0008b430: 204c 6963 656e 7365 2e0a 2020 7c2d 2d2d   License..  |---
 0008b440: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008b450: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008b460: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008b470: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008b480: 2d2d 2d2a 2f0a 2020 0a20 202f 2a2d 2d2d  ---*/.  .  /*---
-0008b490: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0008b480: 2d2d 2d2d 2d2d 2d2d 2d2a 2f0a 2020 0a20  ---------*/.  . 
+0008b490: 202f 2a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   /*-------------
 0008b4a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008b4b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008b4c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008b4d0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 207c 2050  ----------.  | P
-0008b4e0: 7269 7661 7465 2043 5353 2076 6172 6961  rivate CSS varia
-0008b4f0: 626c 6573 0a20 207c 2d2d 2d2d 2d2d 2d2d  bles.  |--------
+0008b4d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0008b4e0: 0a20 207c 2050 7269 7661 7465 2043 5353  .  | Private CSS
+0008b4f0: 2076 6172 6961 626c 6573 0a20 207c 2d2d   variables.  |--
 0008b500: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008b510: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008b520: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008b530: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008b540: 2d2d 2d2d 2a2f 0a20 200a 2020 3a72 6f6f  ----*/.  .  :roo
-0008b550: 7420 7b0a 2020 2020 2d2d 6a70 2d70 7269  t {.    --jp-pri
-0008b560: 7661 7465 2d6e 6f74 6562 6f6f 6b2d 6472  vate-notebook-dr
-0008b570: 6167 496d 6167 652d 7769 6474 683a 2033  agImage-width: 3
-0008b580: 3034 7078 3b0a 2020 2020 2d2d 6a70 2d70  04px;.    --jp-p
-0008b590: 7269 7661 7465 2d6e 6f74 6562 6f6f 6b2d  rivate-notebook-
-0008b5a0: 6472 6167 496d 6167 652d 6865 6967 6874  dragImage-height
-0008b5b0: 3a20 3336 7078 3b0a 2020 2020 2d2d 6a70  : 36px;.    --jp
-0008b5c0: 2d70 7269 7661 7465 2d6e 6f74 6562 6f6f  -private-noteboo
-0008b5d0: 6b2d 7365 6c65 6374 6564 2d63 6f6c 6f72  k-selected-color
-0008b5e0: 3a20 7661 7228 2d2d 6d64 2d62 6c75 652d  : var(--md-blue-
-0008b5f0: 3430 3029 3b0a 2020 2020 2d2d 6a70 2d70  400);.    --jp-p
-0008b600: 7269 7661 7465 2d6e 6f74 6562 6f6f 6b2d  rivate-notebook-
-0008b610: 6163 7469 7665 2d63 6f6c 6f72 3a20 7661  active-color: va
-0008b620: 7228 2d2d 6d64 2d67 7265 656e 2d34 3030  r(--md-green-400
-0008b630: 293b 0a20 207d 0a20 200a 2020 2f2a 2d2d  );.  }.  .  /*--
-0008b640: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0008b540: 2d2d 2d2d 2d2d 2d2d 2d2d 2a2f 0a20 200a  ----------*/.  .
+0008b550: 2020 3a72 6f6f 7420 7b0a 2020 2020 2d2d    :root {.    --
+0008b560: 6a70 2d70 7269 7661 7465 2d6e 6f74 6562  jp-private-noteb
+0008b570: 6f6f 6b2d 6472 6167 496d 6167 652d 7769  ook-dragImage-wi
+0008b580: 6474 683a 2033 3034 7078 3b0a 2020 2020  dth: 304px;.    
+0008b590: 2d2d 6a70 2d70 7269 7661 7465 2d6e 6f74  --jp-private-not
+0008b5a0: 6562 6f6f 6b2d 6472 6167 496d 6167 652d  ebook-dragImage-
+0008b5b0: 6865 6967 6874 3a20 3336 7078 3b0a 2020  height: 36px;.  
+0008b5c0: 2020 2d2d 6a70 2d70 7269 7661 7465 2d6e    --jp-private-n
+0008b5d0: 6f74 6562 6f6f 6b2d 7365 6c65 6374 6564  otebook-selected
+0008b5e0: 2d63 6f6c 6f72 3a20 7661 7228 2d2d 6d64  -color: var(--md
+0008b5f0: 2d62 6c75 652d 3430 3029 3b0a 2020 2020  -blue-400);.    
+0008b600: 2d2d 6a70 2d70 7269 7661 7465 2d6e 6f74  --jp-private-not
+0008b610: 6562 6f6f 6b2d 6163 7469 7665 2d63 6f6c  ebook-active-col
+0008b620: 6f72 3a20 7661 7228 2d2d 6d64 2d67 7265  or: var(--md-gre
+0008b630: 656e 2d34 3030 293b 0a20 207d 0a20 200a  en-400);.  }.  .
+0008b640: 2020 2f2a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    /*------------
 0008b650: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008b660: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008b670: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008b680: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 7c20  -----------.  | 
-0008b690: 496d 706f 7274 730a 2020 7c2d 2d2d 2d2d  Imports.  |-----
-0008b6a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0008b680: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0008b690: 2d0a 2020 7c20 496d 706f 7274 730a 2020  -.  | Imports.  
+0008b6a0: 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |---------------
 0008b6b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008b6c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008b6d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008b6e0: 2d2d 2d2d 2d2d 2d2a 2f0a 2020 0a20 202f  -------*/.  .  /
-0008b6f0: 2a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  *---------------
+0008b6e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2a 2f0a  -------------*/.
+0008b6f0: 2020 0a20 202f 2a2d 2d2d 2d2d 2d2d 2d2d    .  /*---------
 0008b700: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008b710: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008b720: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008b730: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
-0008b740: 207c 204e 6f74 6562 6f6f 6b0a 2020 7c2d   | Notebook.  |-
-0008b750: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0008b730: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0008b740: 2d2d 2d2d 0a20 207c 204e 6f74 6562 6f6f  ----.  | Noteboo
+0008b750: 6b0a 2020 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d  k.  |-----------
 0008b760: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008b770: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008b780: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008b790: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2a 2f0a 2020  -----------*/.  
-0008b7a0: 0a20 202e 6a70 2d4e 6f74 6562 6f6f 6b50  .  .jp-NotebookP
-0008b7b0: 616e 656c 207b 0a20 2020 2064 6973 706c  anel {.    displ
-0008b7c0: 6179 3a20 626c 6f63 6b3b 0a20 2020 2068  ay: block;.    h
-0008b7d0: 6569 6768 743a 2031 3030 253b 0a20 207d  eight: 100%;.  }
-0008b7e0: 0a20 200a 2020 2e6a 702d 4e6f 7465 626f  .  .  .jp-Notebo
-0008b7f0: 6f6b 5061 6e65 6c2e 6a70 2d44 6f63 756d  okPanel.jp-Docum
-0008b800: 656e 7420 7b0a 2020 2020 6d69 6e2d 7769  ent {.    min-wi
-0008b810: 6474 683a 2032 3430 7078 3b0a 2020 2020  dth: 240px;.    
-0008b820: 6d69 6e2d 6865 6967 6874 3a20 3132 3070  min-height: 120p
-0008b830: 783b 0a20 207d 0a20 200a 2020 2e6a 702d  x;.  }.  .  .jp-
-0008b840: 4e6f 7465 626f 6f6b 207b 0a20 2020 2070  Notebook {.    p
-0008b850: 6164 6469 6e67 3a20 7661 7228 2d2d 6a70  adding: var(--jp
-0008b860: 2d6e 6f74 6562 6f6f 6b2d 7061 6464 696e  -notebook-paddin
-0008b870: 6729 3b0a 2020 2020 6f75 746c 696e 653a  g);.    outline:
-0008b880: 206e 6f6e 653b 0a20 2020 206f 7665 7266   none;.    overf
-0008b890: 6c6f 773a 2061 7574 6f3b 0a20 2020 2062  low: auto;.    b
-0008b8a0: 6163 6b67 726f 756e 643a 2076 6172 282d  ackground: var(-
-0008b8b0: 2d6a 702d 6c61 796f 7574 2d63 6f6c 6f72  -jp-layout-color
-0008b8c0: 3029 3b0a 2020 7d0a 2020 0a20 202e 6a70  0);.  }.  .  .jp
-0008b8d0: 2d4e 6f74 6562 6f6f 6b2e 6a70 2d6d 6f64  -Notebook.jp-mod
-0008b8e0: 2d73 6372 6f6c 6c50 6173 7445 6e64 3a3a  -scrollPastEnd::
-0008b8f0: 6166 7465 7220 7b0a 2020 2020 6469 7370  after {.    disp
-0008b900: 6c61 793a 2062 6c6f 636b 3b0a 2020 2020  lay: block;.    
-0008b910: 636f 6e74 656e 743a 2027 273b 0a20 2020  content: '';.   
-0008b920: 206d 696e 2d68 6569 6768 743a 2076 6172   min-height: var
-0008b930: 282d 2d6a 702d 6e6f 7465 626f 6f6b 2d73  (--jp-notebook-s
-0008b940: 6372 6f6c 6c2d 7061 6464 696e 6729 3b0a  croll-padding);.
-0008b950: 2020 7d0a 2020 0a20 202e 6a70 2d4d 6169    }.  .  .jp-Mai
-0008b960: 6e41 7265 6157 6964 6765 742d 436f 6e74  nAreaWidget-Cont
-0008b970: 6169 6e53 7472 6963 7420 2e6a 702d 4e6f  ainStrict .jp-No
-0008b980: 7465 626f 6f6b 202a 207b 0a20 2020 2063  tebook * {.    c
-0008b990: 6f6e 7461 696e 3a20 7374 7269 6374 3b0a  ontain: strict;.
-0008b9a0: 2020 7d0a 2020 0a20 202e 6a70 2d4e 6f74    }.  .  .jp-Not
-0008b9b0: 6562 6f6f 6b2d 7265 6e64 6572 202a 207b  ebook-render * {
-0008b9c0: 0a20 2020 2063 6f6e 7461 696e 3a20 6e6f  .    contain: no
-0008b9d0: 6e65 2021 696d 706f 7274 616e 743b 0a20  ne !important;. 
-0008b9e0: 207d 0a20 200a 2020 2e6a 702d 4e6f 7465   }.  .  .jp-Note
-0008b9f0: 626f 6f6b 202e 6a70 2d43 656c 6c20 7b0a  book .jp-Cell {.
-0008ba00: 2020 2020 6f76 6572 666c 6f77 3a20 7669      overflow: vi
-0008ba10: 7369 626c 653b 0a20 207d 0a20 200a 200a  sible;.  }.  . .
-0008ba20: 2020 0a20 202f 2a2d 2d2d 2d2d 2d2d 2d2d    .  /*---------
+0008b790: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0008b7a0: 2d2a 2f0a 2020 0a20 202e 6a70 2d4e 6f74  -*/.  .  .jp-Not
+0008b7b0: 6562 6f6f 6b50 616e 656c 207b 0a20 2020  ebookPanel {.   
+0008b7c0: 2064 6973 706c 6179 3a20 626c 6f63 6b3b   display: block;
+0008b7d0: 0a20 2020 2068 6569 6768 743a 2031 3030  .    height: 100
+0008b7e0: 253b 0a20 207d 0a20 200a 2020 2e6a 702d  %;.  }.  .  .jp-
+0008b7f0: 4e6f 7465 626f 6f6b 5061 6e65 6c2e 6a70  NotebookPanel.jp
+0008b800: 2d44 6f63 756d 656e 7420 7b0a 2020 2020  -Document {.    
+0008b810: 6d69 6e2d 7769 6474 683a 2032 3430 7078  min-width: 240px
+0008b820: 3b0a 2020 2020 6d69 6e2d 6865 6967 6874  ;.    min-height
+0008b830: 3a20 3132 3070 783b 0a20 207d 0a20 200a  : 120px;.  }.  .
+0008b840: 2020 2e6a 702d 4e6f 7465 626f 6f6b 207b    .jp-Notebook {
+0008b850: 0a20 2020 2070 6164 6469 6e67 3a20 7661  .    padding: va
+0008b860: 7228 2d2d 6a70 2d6e 6f74 6562 6f6f 6b2d  r(--jp-notebook-
+0008b870: 7061 6464 696e 6729 3b0a 2020 2020 6f75  padding);.    ou
+0008b880: 746c 696e 653a 206e 6f6e 653b 0a20 2020  tline: none;.   
+0008b890: 206f 7665 7266 6c6f 773a 2061 7574 6f3b   overflow: auto;
+0008b8a0: 0a20 2020 2062 6163 6b67 726f 756e 643a  .    background:
+0008b8b0: 2076 6172 282d 2d6a 702d 6c61 796f 7574   var(--jp-layout
+0008b8c0: 2d63 6f6c 6f72 3029 3b0a 2020 7d0a 2020  -color0);.  }.  
+0008b8d0: 0a20 202e 6a70 2d4e 6f74 6562 6f6f 6b2e  .  .jp-Notebook.
+0008b8e0: 6a70 2d6d 6f64 2d73 6372 6f6c 6c50 6173  jp-mod-scrollPas
+0008b8f0: 7445 6e64 3a3a 6166 7465 7220 7b0a 2020  tEnd::after {.  
+0008b900: 2020 6469 7370 6c61 793a 2062 6c6f 636b    display: block
+0008b910: 3b0a 2020 2020 636f 6e74 656e 743a 2027  ;.    content: '
+0008b920: 273b 0a20 2020 206d 696e 2d68 6569 6768  ';.    min-heigh
+0008b930: 743a 2076 6172 282d 2d6a 702d 6e6f 7465  t: var(--jp-note
+0008b940: 626f 6f6b 2d73 6372 6f6c 6c2d 7061 6464  book-scroll-padd
+0008b950: 696e 6729 3b0a 2020 7d0a 2020 0a20 202e  ing);.  }.  .  .
+0008b960: 6a70 2d4d 6169 6e41 7265 6157 6964 6765  jp-MainAreaWidge
+0008b970: 742d 436f 6e74 6169 6e53 7472 6963 7420  t-ContainStrict 
+0008b980: 2e6a 702d 4e6f 7465 626f 6f6b 202a 207b  .jp-Notebook * {
+0008b990: 0a20 2020 2063 6f6e 7461 696e 3a20 7374  .    contain: st
+0008b9a0: 7269 6374 3b0a 2020 7d0a 2020 0a20 202e  rict;.  }.  .  .
+0008b9b0: 6a70 2d4e 6f74 6562 6f6f 6b2d 7265 6e64  jp-Notebook-rend
+0008b9c0: 6572 202a 207b 0a20 2020 2063 6f6e 7461  er * {.    conta
+0008b9d0: 696e 3a20 6e6f 6e65 2021 696d 706f 7274  in: none !import
+0008b9e0: 616e 743b 0a20 207d 0a20 200a 2020 2e6a  ant;.  }.  .  .j
+0008b9f0: 702d 4e6f 7465 626f 6f6b 202e 6a70 2d43  p-Notebook .jp-C
+0008ba00: 656c 6c20 7b0a 2020 2020 6f76 6572 666c  ell {.    overfl
+0008ba10: 6f77 3a20 7669 7369 626c 653b 0a20 207d  ow: visible;.  }
+0008ba20: 0a20 200a 200a 2020 0a20 202f 2a2d 2d2d  .  . .  .  /*---
 0008ba30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008ba40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008ba50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008ba60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008ba70: 2d2d 2d2d 0a20 207c 204e 6f74 6562 6f6f  ----.  | Noteboo
-0008ba80: 6b20 7374 6174 6520 7265 6c61 7465 6420  k state related 
-0008ba90: 7374 796c 696e 670a 2020 7c0a 2020 7c20  styling.  |.  | 
-0008baa0: 5468 6520 6e6f 7465 626f 6f6b 2061 6e64  The notebook and
-0008bab0: 2063 656c 6c73 2065 6163 6820 6861 7665   cells each have
-0008bac0: 2073 7461 7465 732c 2068 6572 6520 6172   states, here ar
-0008bad0: 6520 7468 6520 706f 7373 6962 696c 6974  e the possibilit
-0008bae0: 6965 733a 0a20 207c 0a20 207c 202d 204e  ies:.  |.  | - N
-0008baf0: 6f74 6562 6f6f 6b0a 2020 7c20 2020 2d20  otebook.  |   - 
-0008bb00: 436f 6d6d 616e 640a 2020 7c20 2020 2d20  Command.  |   - 
-0008bb10: 4564 6974 0a20 207c 202d 2043 656c 6c0a  Edit.  | - Cell.
-0008bb20: 2020 7c20 2020 2d20 4e6f 6e65 0a20 207c    |   - None.  |
-0008bb30: 2020 202d 2041 6374 6976 6520 286f 6e6c     - Active (onl
-0008bb40: 7920 6f6e 6520 6361 6e20 6265 2061 6374  y one can be act
-0008bb50: 6976 6529 0a20 207c 2020 202d 2053 656c  ive).  |   - Sel
-0008bb60: 6563 7465 6420 2874 6865 2063 656c 6c73  ected (the cells
-0008bb70: 2061 6374 696f 6e73 2061 7265 2061 7070   actions are app
-0008bb80: 6c69 6564 2074 6f29 0a20 207c 2020 202d  lied to).  |   -
-0008bb90: 204d 756c 7469 7365 6c65 6374 6564 2028   Multiselected (
-0008bba0: 7768 656e 206d 756c 7469 706c 6520 7365  when multiple se
-0008bbb0: 6c65 6374 6564 2c20 7468 6520 6375 7273  lected, the curs
-0008bbc0: 6f72 290a 2020 7c20 2020 2d20 4e6f 206f  or).  |   - No o
-0008bbd0: 7574 7075 7473 0a20 207c 2d2d 2d2d 2d2d  utputs.  |------
+0008ba70: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 207c 204e  ----------.  | N
+0008ba80: 6f74 6562 6f6f 6b20 7374 6174 6520 7265  otebook state re
+0008ba90: 6c61 7465 6420 7374 796c 696e 670a 2020  lated styling.  
+0008baa0: 7c0a 2020 7c20 5468 6520 6e6f 7465 626f  |.  | The notebo
+0008bab0: 6f6b 2061 6e64 2063 656c 6c73 2065 6163  ok and cells eac
+0008bac0: 6820 6861 7665 2073 7461 7465 732c 2068  h have states, h
+0008bad0: 6572 6520 6172 6520 7468 6520 706f 7373  ere are the poss
+0008bae0: 6962 696c 6974 6965 733a 0a20 207c 0a20  ibilities:.  |. 
+0008baf0: 207c 202d 204e 6f74 6562 6f6f 6b0a 2020   | - Notebook.  
+0008bb00: 7c20 2020 2d20 436f 6d6d 616e 640a 2020  |   - Command.  
+0008bb10: 7c20 2020 2d20 4564 6974 0a20 207c 202d  |   - Edit.  | -
+0008bb20: 2043 656c 6c0a 2020 7c20 2020 2d20 4e6f   Cell.  |   - No
+0008bb30: 6e65 0a20 207c 2020 202d 2041 6374 6976  ne.  |   - Activ
+0008bb40: 6520 286f 6e6c 7920 6f6e 6520 6361 6e20  e (only one can 
+0008bb50: 6265 2061 6374 6976 6529 0a20 207c 2020  be active).  |  
+0008bb60: 202d 2053 656c 6563 7465 6420 2874 6865   - Selected (the
+0008bb70: 2063 656c 6c73 2061 6374 696f 6e73 2061   cells actions a
+0008bb80: 7265 2061 7070 6c69 6564 2074 6f29 0a20  re applied to). 
+0008bb90: 207c 2020 202d 204d 756c 7469 7365 6c65   |   - Multisele
+0008bba0: 6374 6564 2028 7768 656e 206d 756c 7469  cted (when multi
+0008bbb0: 706c 6520 7365 6c65 6374 6564 2c20 7468  ple selected, th
+0008bbc0: 6520 6375 7273 6f72 290a 2020 7c20 2020  e cursor).  |   
+0008bbd0: 2d20 4e6f 206f 7574 7075 7473 0a20 207c  - No outputs.  |
 0008bbe0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008bbf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008bc00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008bc10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008bc20: 2d2d 2d2d 2d2d 2a2f 0a20 200a 2020 2f2a  ------*/.  .  /*
-0008bc30: 2043 6f6d 6d61 6e64 206f 7220 6564 6974   Command or edit
-0008bc40: 206d 6f64 6573 202a 2f0a 2020 0a20 202f   modes */.  .  /
-0008bc50: 2a20 2e6a 702d 4e6f 7465 626f 6f6b 202e  * .jp-Notebook .
-0008bc60: 6a70 2d43 656c 6c3a 6e6f 7428 2e6a 702d  jp-Cell:not(.jp-
-0008bc70: 6d6f 642d 6163 7469 7665 2920 2e6a 702d  mod-active) .jp-
-0008bc80: 496e 7075 7450 726f 6d70 7420 7b0a 2020  InputPrompt {.  
-0008bc90: 2020 6f70 6163 6974 793a 2076 6172 282d    opacity: var(-
-0008bca0: 2d6a 702d 6365 6c6c 2d70 726f 6d70 742d  -jp-cell-prompt-
-0008bcb0: 6e6f 742d 6163 7469 7665 2d6f 7061 6369  not-active-opaci
-0008bcc0: 7479 293b 0a20 2020 2063 6f6c 6f72 3a20  ty);.    color: 
-0008bcd0: 7661 7228 2d2d 6a70 2d63 656c 6c2d 7072  var(--jp-cell-pr
-0008bce0: 6f6d 7074 2d6e 6f74 2d61 6374 6976 652d  ompt-not-active-
-0008bcf0: 666f 6e74 2d63 6f6c 6f72 293b 0a20 207d  font-color);.  }
-0008bd00: 0a20 200a 2020 2e6a 702d 4e6f 7465 626f  .  .  .jp-Notebo
-0008bd10: 6f6b 202e 6a70 2d43 656c 6c3a 6e6f 7428  ok .jp-Cell:not(
-0008bd20: 2e6a 702d 6d6f 642d 6163 7469 7665 2920  .jp-mod-active) 
-0008bd30: 2e6a 702d 4f75 7470 7574 5072 6f6d 7074  .jp-OutputPrompt
-0008bd40: 207b 0a20 2020 206f 7061 6369 7479 3a20   {.    opacity: 
-0008bd50: 7661 7228 2d2d 6a70 2d63 656c 6c2d 7072  var(--jp-cell-pr
-0008bd60: 6f6d 7074 2d6e 6f74 2d61 6374 6976 652d  ompt-not-active-
-0008bd70: 6f70 6163 6974 7929 3b0a 2020 2020 636f  opacity);.    co
-0008bd80: 6c6f 723a 2076 6172 282d 2d6a 702d 6365  lor: var(--jp-ce
-0008bd90: 6c6c 2d70 726f 6d70 742d 6e6f 742d 6163  ll-prompt-not-ac
-0008bda0: 7469 7665 2d66 6f6e 742d 636f 6c6f 7229  tive-font-color)
-0008bdb0: 3b0a 2020 7d20 2a2f 0a20 200a 2020 2f2a  ;.  } */.  .  /*
-0008bdc0: 2063 656c 6c20 6973 2061 6374 6976 6520   cell is active 
-0008bdd0: 2a2f 0a20 202e 6a70 2d4e 6f74 6562 6f6f  */.  .jp-Noteboo
-0008bde0: 6b20 2e6a 702d 4365 6c6c 2e6a 702d 6d6f  k .jp-Cell.jp-mo
-0008bdf0: 642d 6163 7469 7665 202e 6a70 2d43 6f6c  d-active .jp-Col
-0008be00: 6c61 7073 6572 207b 0a20 2020 2062 6163  lapser {.    bac
-0008be10: 6b67 726f 756e 643a 2076 6172 282d 2d6a  kground: var(--j
-0008be20: 702d 6272 616e 642d 636f 6c6f 7231 293b  p-brand-color1);
-0008be30: 0a20 207d 0a20 200a 2020 2f2a 2063 656c  .  }.  .  /* cel
-0008be40: 6c20 6973 2064 6972 7479 202a 2f0a 2020  l is dirty */.  
-0008be50: 2f2a 202e 6a70 2d4e 6f74 6562 6f6f 6b20  /* .jp-Notebook 
-0008be60: 2e6a 702d 4365 6c6c 2e6a 702d 6d6f 642d  .jp-Cell.jp-mod-
-0008be70: 6469 7274 7920 2e6a 702d 496e 7075 7450  dirty .jp-InputP
-0008be80: 726f 6d70 7420 7b0a 2020 2020 636f 6c6f  rompt {.    colo
-0008be90: 723a 2076 6172 282d 2d6a 702d 7761 726e  r: var(--jp-warn
-0008bea0: 2d63 6f6c 6f72 3129 3b0a 2020 7d0a 2020  -color1);.  }.  
-0008beb0: 2e6a 702d 4e6f 7465 626f 6f6b 202e 6a70  .jp-Notebook .jp
-0008bec0: 2d43 656c 6c2e 6a70 2d6d 6f64 2d64 6972  -Cell.jp-mod-dir
-0008bed0: 7479 202e 6a70 2d49 6e70 7574 5072 6f6d  ty .jp-InputProm
-0008bee0: 7074 3a62 6566 6f72 6520 7b0a 2020 2020  pt:before {.    
-0008bef0: 636f 6c6f 723a 2076 6172 282d 2d6a 702d  color: var(--jp-
-0008bf00: 7761 726e 2d63 6f6c 6f72 3129 3b0a 2020  warn-color1);.  
-0008bf10: 2020 636f 6e74 656e 743a 2027 e280 a227    content: '...'
-0008bf20: 3b0a 2020 7d20 2a2f 0a20 200a 2020 2e6a  ;.  } */.  .  .j
-0008bf30: 702d 4e6f 7465 626f 6f6b 202e 6a70 2d43  p-Notebook .jp-C
-0008bf40: 656c 6c2e 6a70 2d6d 6f64 2d61 6374 6976  ell.jp-mod-activ
-0008bf50: 652e 6a70 2d6d 6f64 2d64 6972 7479 202e  e.jp-mod-dirty .
-0008bf60: 6a70 2d43 6f6c 6c61 7073 6572 207b 0a20  jp-Collapser {. 
-0008bf70: 2020 2062 6163 6b67 726f 756e 643a 2076     background: v
-0008bf80: 6172 282d 2d6a 702d 7761 726e 2d63 6f6c  ar(--jp-warn-col
-0008bf90: 6f72 3129 3b0a 2020 7d0a 2020 0a20 202f  or1);.  }.  .  /
-0008bfa0: 2a20 636f 6c6c 6170 7365 7220 6973 2068  * collapser is h
-0008bfb0: 6f76 6572 6564 202a 2f0a 2020 2e6a 702d  overed */.  .jp-
-0008bfc0: 4e6f 7465 626f 6f6b 202e 6a70 2d43 656c  Notebook .jp-Cel
-0008bfd0: 6c20 2e6a 702d 436f 6c6c 6170 7365 723a  l .jp-Collapser:
-0008bfe0: 686f 7665 7220 7b0a 2020 2020 626f 782d  hover {.    box-
-0008bff0: 7368 6164 6f77 3a20 7661 7228 2d2d 6a70  shadow: var(--jp
-0008c000: 2d65 6c65 7661 7469 6f6e 2d7a 3229 3b0a  -elevation-z2);.
-0008c010: 2020 2020 6261 636b 6772 6f75 6e64 3a20      background: 
-0008c020: 7661 7228 2d2d 6a70 2d62 7261 6e64 2d63  var(--jp-brand-c
-0008c030: 6f6c 6f72 3129 3b0a 2020 2020 6f70 6163  olor1);.    opac
-0008c040: 6974 793a 2076 6172 282d 2d6a 702d 6365  ity: var(--jp-ce
-0008c050: 6c6c 2d63 6f6c 6c61 7073 6572 2d6e 6f74  ll-collapser-not
-0008c060: 2d61 6374 6976 652d 686f 7665 722d 6f70  -active-hover-op
-0008c070: 6163 6974 7929 3b0a 2020 7d0a 2020 0a20  acity);.  }.  . 
-0008c080: 202f 2a20 6365 6c6c 2069 7320 6163 7469   /* cell is acti
-0008c090: 7665 2061 6e64 2063 6f6c 6c61 7073 6572  ve and collapser
-0008c0a0: 2069 7320 686f 7665 7265 6420 2a2f 0a20   is hovered */. 
-0008c0b0: 202e 6a70 2d4e 6f74 6562 6f6f 6b20 2e6a   .jp-Notebook .j
-0008c0c0: 702d 4365 6c6c 2e6a 702d 6d6f 642d 6163  p-Cell.jp-mod-ac
-0008c0d0: 7469 7665 202e 6a70 2d43 6f6c 6c61 7073  tive .jp-Collaps
-0008c0e0: 6572 3a68 6f76 6572 207b 0a20 2020 2062  er:hover {.    b
-0008c0f0: 6163 6b67 726f 756e 643a 2076 6172 282d  ackground: var(-
-0008c100: 2d6a 702d 6272 616e 642d 636f 6c6f 7230  -jp-brand-color0
-0008c110: 293b 0a20 2020 206f 7061 6369 7479 3a20  );.    opacity: 
-0008c120: 313b 0a20 207d 0a20 200a 2020 2f2a 2043  1;.  }.  .  /* C
-0008c130: 6f6d 6d61 6e64 206d 6f64 6520 2a2f 0a20  ommand mode */. 
-0008c140: 200a 2020 2e6a 702d 4e6f 7465 626f 6f6b   .  .jp-Notebook
-0008c150: 2e6a 702d 6d6f 642d 636f 6d6d 616e 644d  .jp-mod-commandM
-0008c160: 6f64 6520 2e6a 702d 4365 6c6c 2e6a 702d  ode .jp-Cell.jp-
-0008c170: 6d6f 642d 7365 6c65 6374 6564 207b 0a20  mod-selected {. 
-0008c180: 2020 2062 6163 6b67 726f 756e 643a 2076     background: v
-0008c190: 6172 282d 2d6a 702d 6e6f 7465 626f 6f6b  ar(--jp-notebook
-0008c1a0: 2d6d 756c 7469 7365 6c65 6374 6564 2d63  -multiselected-c
-0008c1b0: 6f6c 6f72 293b 0a20 207d 0a20 200a 2020  olor);.  }.  .  
-0008c1c0: 2e6a 702d 4e6f 7465 626f 6f6b 2e6a 702d  .jp-Notebook.jp-
-0008c1d0: 6d6f 642d 636f 6d6d 616e 644d 6f64 650a  mod-commandMode.
-0008c1e0: 2020 2020 2e6a 702d 4365 6c6c 2e6a 702d      .jp-Cell.jp-
-0008c1f0: 6d6f 642d 6163 7469 7665 2e6a 702d 6d6f  mod-active.jp-mo
-0008c200: 642d 7365 6c65 6374 6564 3a6e 6f74 282e  d-selected:not(.
-0008c210: 6a70 2d6d 6f64 2d6d 756c 7469 5365 6c65  jp-mod-multiSele
-0008c220: 6374 6564 2920 7b0a 2020 2020 6261 636b  cted) {.    back
-0008c230: 6772 6f75 6e64 3a20 7472 616e 7370 6172  ground: transpar
-0008c240: 656e 743b 0a20 207d 0a20 200a 2020 2f2a  ent;.  }.  .  /*
-0008c250: 2045 6469 7420 6d6f 6465 202a 2f0a 2020   Edit mode */.  
-0008c260: 0a20 202e 6a70 2d4e 6f74 6562 6f6f 6b2e  .  .jp-Notebook.
-0008c270: 6a70 2d6d 6f64 2d65 6469 744d 6f64 6520  jp-mod-editMode 
-0008c280: 2e6a 702d 4365 6c6c 2e6a 702d 6d6f 642d  .jp-Cell.jp-mod-
-0008c290: 6163 7469 7665 202e 6a70 2d49 6e70 7574  active .jp-Input
-0008c2a0: 4172 6561 2d65 6469 746f 7220 7b0a 2020  Area-editor {.  
-0008c2b0: 2020 626f 7264 6572 3a20 7661 7228 2d2d    border: var(--
-0008c2c0: 6a70 2d62 6f72 6465 722d 7769 6474 6829  jp-border-width)
-0008c2d0: 2073 6f6c 6964 2076 6172 282d 2d6a 702d   solid var(--jp-
-0008c2e0: 6365 6c6c 2d65 6469 746f 722d 6163 7469  cell-editor-acti
-0008c2f0: 7665 2d62 6f72 6465 722d 636f 6c6f 7229  ve-border-color)
-0008c300: 3b0a 2020 2020 626f 782d 7368 6164 6f77  ;.    box-shadow
-0008c310: 3a20 7661 7228 2d2d 6a70 2d69 6e70 7574  : var(--jp-input
-0008c320: 2d62 6f78 2d73 6861 646f 7729 3b0a 2020  -box-shadow);.  
-0008c330: 2020 6261 636b 6772 6f75 6e64 2d63 6f6c    background-col
-0008c340: 6f72 3a20 7661 7228 2d2d 6a70 2d63 656c  or: var(--jp-cel
-0008c350: 6c2d 6564 6974 6f72 2d61 6374 6976 652d  l-editor-active-
-0008c360: 6261 636b 6772 6f75 6e64 293b 0a20 207d  background);.  }
-0008c370: 0a20 200a 2020 2f2a 2d2d 2d2d 2d2d 2d2d  .  .  /*--------
+0008bc20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2a2f 0a20  ------------*/. 
+0008bc30: 200a 2020 2f2a 2043 6f6d 6d61 6e64 206f   .  /* Command o
+0008bc40: 7220 6564 6974 206d 6f64 6573 202a 2f0a  r edit modes */.
+0008bc50: 2020 0a20 202f 2a20 2e6a 702d 4e6f 7465    .  /* .jp-Note
+0008bc60: 626f 6f6b 202e 6a70 2d43 656c 6c3a 6e6f  book .jp-Cell:no
+0008bc70: 7428 2e6a 702d 6d6f 642d 6163 7469 7665  t(.jp-mod-active
+0008bc80: 2920 2e6a 702d 496e 7075 7450 726f 6d70  ) .jp-InputPromp
+0008bc90: 7420 7b0a 2020 2020 6f70 6163 6974 793a  t {.    opacity:
+0008bca0: 2076 6172 282d 2d6a 702d 6365 6c6c 2d70   var(--jp-cell-p
+0008bcb0: 726f 6d70 742d 6e6f 742d 6163 7469 7665  rompt-not-active
+0008bcc0: 2d6f 7061 6369 7479 293b 0a20 2020 2063  -opacity);.    c
+0008bcd0: 6f6c 6f72 3a20 7661 7228 2d2d 6a70 2d63  olor: var(--jp-c
+0008bce0: 656c 6c2d 7072 6f6d 7074 2d6e 6f74 2d61  ell-prompt-not-a
+0008bcf0: 6374 6976 652d 666f 6e74 2d63 6f6c 6f72  ctive-font-color
+0008bd00: 293b 0a20 207d 0a20 200a 2020 2e6a 702d  );.  }.  .  .jp-
+0008bd10: 4e6f 7465 626f 6f6b 202e 6a70 2d43 656c  Notebook .jp-Cel
+0008bd20: 6c3a 6e6f 7428 2e6a 702d 6d6f 642d 6163  l:not(.jp-mod-ac
+0008bd30: 7469 7665 2920 2e6a 702d 4f75 7470 7574  tive) .jp-Output
+0008bd40: 5072 6f6d 7074 207b 0a20 2020 206f 7061  Prompt {.    opa
+0008bd50: 6369 7479 3a20 7661 7228 2d2d 6a70 2d63  city: var(--jp-c
+0008bd60: 656c 6c2d 7072 6f6d 7074 2d6e 6f74 2d61  ell-prompt-not-a
+0008bd70: 6374 6976 652d 6f70 6163 6974 7929 3b0a  ctive-opacity);.
+0008bd80: 2020 2020 636f 6c6f 723a 2076 6172 282d      color: var(-
+0008bd90: 2d6a 702d 6365 6c6c 2d70 726f 6d70 742d  -jp-cell-prompt-
+0008bda0: 6e6f 742d 6163 7469 7665 2d66 6f6e 742d  not-active-font-
+0008bdb0: 636f 6c6f 7229 3b0a 2020 7d20 2a2f 0a20  color);.  } */. 
+0008bdc0: 200a 2020 2f2a 2063 656c 6c20 6973 2061   .  /* cell is a
+0008bdd0: 6374 6976 6520 2a2f 0a20 202e 6a70 2d4e  ctive */.  .jp-N
+0008bde0: 6f74 6562 6f6f 6b20 2e6a 702d 4365 6c6c  otebook .jp-Cell
+0008bdf0: 2e6a 702d 6d6f 642d 6163 7469 7665 202e  .jp-mod-active .
+0008be00: 6a70 2d43 6f6c 6c61 7073 6572 207b 0a20  jp-Collapser {. 
+0008be10: 2020 2062 6163 6b67 726f 756e 643a 2076     background: v
+0008be20: 6172 282d 2d6a 702d 6272 616e 642d 636f  ar(--jp-brand-co
+0008be30: 6c6f 7231 293b 0a20 207d 0a20 200a 2020  lor1);.  }.  .  
+0008be40: 2f2a 2063 656c 6c20 6973 2064 6972 7479  /* cell is dirty
+0008be50: 202a 2f0a 2020 2f2a 202e 6a70 2d4e 6f74   */.  /* .jp-Not
+0008be60: 6562 6f6f 6b20 2e6a 702d 4365 6c6c 2e6a  ebook .jp-Cell.j
+0008be70: 702d 6d6f 642d 6469 7274 7920 2e6a 702d  p-mod-dirty .jp-
+0008be80: 496e 7075 7450 726f 6d70 7420 7b0a 2020  InputPrompt {.  
+0008be90: 2020 636f 6c6f 723a 2076 6172 282d 2d6a    color: var(--j
+0008bea0: 702d 7761 726e 2d63 6f6c 6f72 3129 3b0a  p-warn-color1);.
+0008beb0: 2020 7d0a 2020 2e6a 702d 4e6f 7465 626f    }.  .jp-Notebo
+0008bec0: 6f6b 202e 6a70 2d43 656c 6c2e 6a70 2d6d  ok .jp-Cell.jp-m
+0008bed0: 6f64 2d64 6972 7479 202e 6a70 2d49 6e70  od-dirty .jp-Inp
+0008bee0: 7574 5072 6f6d 7074 3a62 6566 6f72 6520  utPrompt:before 
+0008bef0: 7b0a 2020 2020 636f 6c6f 723a 2076 6172  {.    color: var
+0008bf00: 282d 2d6a 702d 7761 726e 2d63 6f6c 6f72  (--jp-warn-color
+0008bf10: 3129 3b0a 2020 2020 636f 6e74 656e 743a  1);.    content:
+0008bf20: 2027 e280 a227 3b0a 2020 7d20 2a2f 0a20   '...';.  } */. 
+0008bf30: 200a 2020 2e6a 702d 4e6f 7465 626f 6f6b   .  .jp-Notebook
+0008bf40: 202e 6a70 2d43 656c 6c2e 6a70 2d6d 6f64   .jp-Cell.jp-mod
+0008bf50: 2d61 6374 6976 652e 6a70 2d6d 6f64 2d64  -active.jp-mod-d
+0008bf60: 6972 7479 202e 6a70 2d43 6f6c 6c61 7073  irty .jp-Collaps
+0008bf70: 6572 207b 0a20 2020 2062 6163 6b67 726f  er {.    backgro
+0008bf80: 756e 643a 2076 6172 282d 2d6a 702d 7761  und: var(--jp-wa
+0008bf90: 726e 2d63 6f6c 6f72 3129 3b0a 2020 7d0a  rn-color1);.  }.
+0008bfa0: 2020 0a20 202f 2a20 636f 6c6c 6170 7365    .  /* collapse
+0008bfb0: 7220 6973 2068 6f76 6572 6564 202a 2f0a  r is hovered */.
+0008bfc0: 2020 2e6a 702d 4e6f 7465 626f 6f6b 202e    .jp-Notebook .
+0008bfd0: 6a70 2d43 656c 6c20 2e6a 702d 436f 6c6c  jp-Cell .jp-Coll
+0008bfe0: 6170 7365 723a 686f 7665 7220 7b0a 2020  apser:hover {.  
+0008bff0: 2020 626f 782d 7368 6164 6f77 3a20 7661    box-shadow: va
+0008c000: 7228 2d2d 6a70 2d65 6c65 7661 7469 6f6e  r(--jp-elevation
+0008c010: 2d7a 3229 3b0a 2020 2020 6261 636b 6772  -z2);.    backgr
+0008c020: 6f75 6e64 3a20 7661 7228 2d2d 6a70 2d62  ound: var(--jp-b
+0008c030: 7261 6e64 2d63 6f6c 6f72 3129 3b0a 2020  rand-color1);.  
+0008c040: 2020 6f70 6163 6974 793a 2076 6172 282d    opacity: var(-
+0008c050: 2d6a 702d 6365 6c6c 2d63 6f6c 6c61 7073  -jp-cell-collaps
+0008c060: 6572 2d6e 6f74 2d61 6374 6976 652d 686f  er-not-active-ho
+0008c070: 7665 722d 6f70 6163 6974 7929 3b0a 2020  ver-opacity);.  
+0008c080: 7d0a 2020 0a20 202f 2a20 6365 6c6c 2069  }.  .  /* cell i
+0008c090: 7320 6163 7469 7665 2061 6e64 2063 6f6c  s active and col
+0008c0a0: 6c61 7073 6572 2069 7320 686f 7665 7265  lapser is hovere
+0008c0b0: 6420 2a2f 0a20 202e 6a70 2d4e 6f74 6562  d */.  .jp-Noteb
+0008c0c0: 6f6f 6b20 2e6a 702d 4365 6c6c 2e6a 702d  ook .jp-Cell.jp-
+0008c0d0: 6d6f 642d 6163 7469 7665 202e 6a70 2d43  mod-active .jp-C
+0008c0e0: 6f6c 6c61 7073 6572 3a68 6f76 6572 207b  ollapser:hover {
+0008c0f0: 0a20 2020 2062 6163 6b67 726f 756e 643a  .    background:
+0008c100: 2076 6172 282d 2d6a 702d 6272 616e 642d   var(--jp-brand-
+0008c110: 636f 6c6f 7230 293b 0a20 2020 206f 7061  color0);.    opa
+0008c120: 6369 7479 3a20 313b 0a20 207d 0a20 200a  city: 1;.  }.  .
+0008c130: 2020 2f2a 2043 6f6d 6d61 6e64 206d 6f64    /* Command mod
+0008c140: 6520 2a2f 0a20 200a 2020 2e6a 702d 4e6f  e */.  .  .jp-No
+0008c150: 7465 626f 6f6b 2e6a 702d 6d6f 642d 636f  tebook.jp-mod-co
+0008c160: 6d6d 616e 644d 6f64 6520 2e6a 702d 4365  mmandMode .jp-Ce
+0008c170: 6c6c 2e6a 702d 6d6f 642d 7365 6c65 6374  ll.jp-mod-select
+0008c180: 6564 207b 0a20 2020 2062 6163 6b67 726f  ed {.    backgro
+0008c190: 756e 643a 2076 6172 282d 2d6a 702d 6e6f  und: var(--jp-no
+0008c1a0: 7465 626f 6f6b 2d6d 756c 7469 7365 6c65  tebook-multisele
+0008c1b0: 6374 6564 2d63 6f6c 6f72 293b 0a20 207d  cted-color);.  }
+0008c1c0: 0a20 200a 2020 2e6a 702d 4e6f 7465 626f  .  .  .jp-Notebo
+0008c1d0: 6f6b 2e6a 702d 6d6f 642d 636f 6d6d 616e  ok.jp-mod-comman
+0008c1e0: 644d 6f64 650a 2020 2020 2e6a 702d 4365  dMode.    .jp-Ce
+0008c1f0: 6c6c 2e6a 702d 6d6f 642d 6163 7469 7665  ll.jp-mod-active
+0008c200: 2e6a 702d 6d6f 642d 7365 6c65 6374 6564  .jp-mod-selected
+0008c210: 3a6e 6f74 282e 6a70 2d6d 6f64 2d6d 756c  :not(.jp-mod-mul
+0008c220: 7469 5365 6c65 6374 6564 2920 7b0a 2020  tiSelected) {.  
+0008c230: 2020 6261 636b 6772 6f75 6e64 3a20 7472    background: tr
+0008c240: 616e 7370 6172 656e 743b 0a20 207d 0a20  ansparent;.  }. 
+0008c250: 200a 2020 2f2a 2045 6469 7420 6d6f 6465   .  /* Edit mode
+0008c260: 202a 2f0a 2020 0a20 202e 6a70 2d4e 6f74   */.  .  .jp-Not
+0008c270: 6562 6f6f 6b2e 6a70 2d6d 6f64 2d65 6469  ebook.jp-mod-edi
+0008c280: 744d 6f64 6520 2e6a 702d 4365 6c6c 2e6a  tMode .jp-Cell.j
+0008c290: 702d 6d6f 642d 6163 7469 7665 202e 6a70  p-mod-active .jp
+0008c2a0: 2d49 6e70 7574 4172 6561 2d65 6469 746f  -InputArea-edito
+0008c2b0: 7220 7b0a 2020 2020 626f 7264 6572 3a20  r {.    border: 
+0008c2c0: 7661 7228 2d2d 6a70 2d62 6f72 6465 722d  var(--jp-border-
+0008c2d0: 7769 6474 6829 2073 6f6c 6964 2076 6172  width) solid var
+0008c2e0: 282d 2d6a 702d 6365 6c6c 2d65 6469 746f  (--jp-cell-edito
+0008c2f0: 722d 6163 7469 7665 2d62 6f72 6465 722d  r-active-border-
+0008c300: 636f 6c6f 7229 3b0a 2020 2020 626f 782d  color);.    box-
+0008c310: 7368 6164 6f77 3a20 7661 7228 2d2d 6a70  shadow: var(--jp
+0008c320: 2d69 6e70 7574 2d62 6f78 2d73 6861 646f  -input-box-shado
+0008c330: 7729 3b0a 2020 2020 6261 636b 6772 6f75  w);.    backgrou
+0008c340: 6e64 2d63 6f6c 6f72 3a20 7661 7228 2d2d  nd-color: var(--
+0008c350: 6a70 2d63 656c 6c2d 6564 6974 6f72 2d61  jp-cell-editor-a
+0008c360: 6374 6976 652d 6261 636b 6772 6f75 6e64  ctive-background
+0008c370: 293b 0a20 207d 0a20 200a 2020 2f2a 2d2d  );.  }.  .  /*--
 0008c380: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008c390: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008c3a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008c3b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008c3c0: 2d2d 2d2d 2d0a 2020 7c20 4e6f 7465 626f  -----.  | Notebo
-0008c3d0: 6f6b 2064 7261 6720 616e 6420 6472 6f70  ok drag and drop
-0008c3e0: 0a20 207c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .  |------------
+0008c3c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 7c20  -----------.  | 
+0008c3d0: 4e6f 7465 626f 6f6b 2064 7261 6720 616e  Notebook drag an
+0008c3e0: 6420 6472 6f70 0a20 207c 2d2d 2d2d 2d2d  d drop.  |------
 0008c3f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008c400: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008c410: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008c420: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008c430: 2a2f 0a20 200a 2020 2e6a 702d 4e6f 7465  */.  .  .jp-Note
-0008c440: 626f 6f6b 2d63 656c 6c2e 6a70 2d6d 6f64  book-cell.jp-mod
-0008c450: 2d64 726f 7053 6f75 7263 6520 7b0a 2020  -dropSource {.  
-0008c460: 2020 6f70 6163 6974 793a 2030 2e35 3b0a    opacity: 0.5;.
-0008c470: 2020 7d0a 2020 0a20 202e 6a70 2d4e 6f74    }.  .  .jp-Not
-0008c480: 6562 6f6f 6b2d 6365 6c6c 2e6a 702d 6d6f  ebook-cell.jp-mo
-0008c490: 642d 6472 6f70 5461 7267 6574 2c0a 2020  d-dropTarget,.  
-0008c4a0: 2e6a 702d 4e6f 7465 626f 6f6b 2e6a 702d  .jp-Notebook.jp-
-0008c4b0: 6d6f 642d 636f 6d6d 616e 644d 6f64 650a  mod-commandMode.
-0008c4c0: 2020 2020 2e6a 702d 4e6f 7465 626f 6f6b      .jp-Notebook
-0008c4d0: 2d63 656c 6c2e 6a70 2d6d 6f64 2d61 6374  -cell.jp-mod-act
-0008c4e0: 6976 652e 6a70 2d6d 6f64 2d73 656c 6563  ive.jp-mod-selec
-0008c4f0: 7465 642e 6a70 2d6d 6f64 2d64 726f 7054  ted.jp-mod-dropT
-0008c500: 6172 6765 7420 7b0a 2020 2020 626f 7264  arget {.    bord
-0008c510: 6572 2d74 6f70 2d63 6f6c 6f72 3a20 7661  er-top-color: va
-0008c520: 7228 2d2d 6a70 2d70 7269 7661 7465 2d6e  r(--jp-private-n
-0008c530: 6f74 6562 6f6f 6b2d 7365 6c65 6374 6564  otebook-selected
-0008c540: 2d63 6f6c 6f72 293b 0a20 2020 2062 6f72  -color);.    bor
-0008c550: 6465 722d 746f 702d 7374 796c 653a 2073  der-top-style: s
-0008c560: 6f6c 6964 3b0a 2020 2020 626f 7264 6572  olid;.    border
-0008c570: 2d74 6f70 2d77 6964 7468 3a20 3270 783b  -top-width: 2px;
-0008c580: 0a20 207d 0a20 200a 2020 2e6a 702d 6472  .  }.  .  .jp-dr
-0008c590: 6167 496d 6167 6520 7b0a 2020 2020 6469  agImage {.    di
-0008c5a0: 7370 6c61 793a 2062 6c6f 636b 3b0a 2020  splay: block;.  
-0008c5b0: 2020 666c 6578 2d64 6972 6563 7469 6f6e    flex-direction
-0008c5c0: 3a20 726f 773b 0a20 2020 2077 6964 7468  : row;.    width
-0008c5d0: 3a20 7661 7228 2d2d 6a70 2d70 7269 7661  : var(--jp-priva
-0008c5e0: 7465 2d6e 6f74 6562 6f6f 6b2d 6472 6167  te-notebook-drag
-0008c5f0: 496d 6167 652d 7769 6474 6829 3b0a 2020  Image-width);.  
-0008c600: 2020 6865 6967 6874 3a20 7661 7228 2d2d    height: var(--
-0008c610: 6a70 2d70 7269 7661 7465 2d6e 6f74 6562  jp-private-noteb
-0008c620: 6f6f 6b2d 6472 6167 496d 6167 652d 6865  ook-dragImage-he
-0008c630: 6967 6874 293b 0a20 2020 2062 6f72 6465  ight);.    borde
-0008c640: 723a 2076 6172 282d 2d6a 702d 626f 7264  r: var(--jp-bord
-0008c650: 6572 2d77 6964 7468 2920 736f 6c69 6420  er-width) solid 
-0008c660: 7661 7228 2d2d 6a70 2d63 656c 6c2d 6564  var(--jp-cell-ed
-0008c670: 6974 6f72 2d62 6f72 6465 722d 636f 6c6f  itor-border-colo
-0008c680: 7229 3b0a 2020 2020 6261 636b 6772 6f75  r);.    backgrou
-0008c690: 6e64 3a20 7661 7228 2d2d 6a70 2d63 656c  nd: var(--jp-cel
-0008c6a0: 6c2d 6564 6974 6f72 2d62 6163 6b67 726f  l-editor-backgro
-0008c6b0: 756e 6429 3b0a 2020 2020 6f76 6572 666c  und);.    overfl
-0008c6c0: 6f77 3a20 7669 7369 626c 653b 0a20 207d  ow: visible;.  }
-0008c6d0: 0a20 200a 2020 2e6a 702d 6472 6167 496d  .  .  .jp-dragIm
-0008c6e0: 6167 652d 7369 6e67 6c65 5072 6f6d 7074  age-singlePrompt
-0008c6f0: 207b 0a20 2020 2062 6f78 2d73 6861 646f   {.    box-shado
-0008c700: 773a 2032 7078 2032 7078 2034 7078 2030  w: 2px 2px 4px 0
-0008c710: 7078 2072 6762 6128 302c 2030 2c20 302c  px rgba(0, 0, 0,
-0008c720: 2030 2e31 3229 3b0a 2020 7d0a 2020 0a20   0.12);.  }.  . 
-0008c730: 202e 6a70 2d64 7261 6749 6d61 6765 202e   .jp-dragImage .
-0008c740: 6a70 2d64 7261 6749 6d61 6765 2d63 6f6e  jp-dragImage-con
-0008c750: 7465 6e74 207b 0a20 2020 2066 6c65 783a  tent {.    flex:
-0008c760: 2031 2031 2061 7574 6f3b 0a20 2020 207a   1 1 auto;.    z
-0008c770: 2d69 6e64 6578 3a20 323b 0a20 2020 2066  -index: 2;.    f
-0008c780: 6f6e 742d 7369 7a65 3a20 7661 7228 2d2d  ont-size: var(--
-0008c790: 6a70 2d63 6f64 652d 666f 6e74 2d73 697a  jp-code-font-siz
-0008c7a0: 6529 3b0a 2020 2020 666f 6e74 2d66 616d  e);.    font-fam
-0008c7b0: 696c 793a 2076 6172 282d 2d6a 702d 636f  ily: var(--jp-co
-0008c7c0: 6465 2d66 6f6e 742d 6661 6d69 6c79 293b  de-font-family);
-0008c7d0: 0a20 2020 206c 696e 652d 6865 6967 6874  .    line-height
-0008c7e0: 3a20 7661 7228 2d2d 6a70 2d63 6f64 652d  : var(--jp-code-
-0008c7f0: 6c69 6e65 2d68 6569 6768 7429 3b0a 2020  line-height);.  
-0008c800: 2020 7061 6464 696e 673a 2076 6172 282d    padding: var(-
-0008c810: 2d6a 702d 636f 6465 2d70 6164 6469 6e67  -jp-code-padding
-0008c820: 293b 0a20 2020 2062 6f72 6465 723a 2076  );.    border: v
-0008c830: 6172 282d 2d6a 702d 626f 7264 6572 2d77  ar(--jp-border-w
-0008c840: 6964 7468 2920 736f 6c69 6420 7661 7228  idth) solid var(
-0008c850: 2d2d 6a70 2d63 656c 6c2d 6564 6974 6f72  --jp-cell-editor
-0008c860: 2d62 6f72 6465 722d 636f 6c6f 7229 3b0a  -border-color);.
-0008c870: 2020 2020 6261 636b 6772 6f75 6e64 3a20      background: 
-0008c880: 7661 7228 2d2d 6a70 2d63 656c 6c2d 6564  var(--jp-cell-ed
-0008c890: 6974 6f72 2d62 6163 6b67 726f 756e 642d  itor-background-
-0008c8a0: 636f 6c6f 7229 3b0a 2020 2020 636f 6c6f  color);.    colo
-0008c8b0: 723a 2076 6172 282d 2d6a 702d 636f 6e74  r: var(--jp-cont
-0008c8c0: 656e 742d 666f 6e74 2d63 6f6c 6f72 3329  ent-font-color3)
-0008c8d0: 3b0a 2020 2020 7465 7874 2d61 6c69 676e  ;.    text-align
-0008c8e0: 3a20 6c65 6674 3b0a 2020 2020 6d61 7267  : left;.    marg
-0008c8f0: 696e 3a20 3470 7820 3470 7820 3470 7820  in: 4px 4px 4px 
-0008c900: 3070 783b 0a20 207d 0a20 200a 2020 2e6a  0px;.  }.  .  .j
-0008c910: 702d 6472 6167 496d 6167 6520 2e6a 702d  p-dragImage .jp-
-0008c920: 6472 6167 496d 6167 652d 7072 6f6d 7074  dragImage-prompt
-0008c930: 207b 0a20 2020 2066 6c65 783a 2030 2030   {.    flex: 0 0
-0008c940: 2061 7574 6f3b 0a20 2020 206d 696e 2d77   auto;.    min-w
-0008c950: 6964 7468 3a20 3336 7078 3b0a 2020 2020  idth: 36px;.    
-0008c960: 636f 6c6f 723a 2076 6172 282d 2d6a 702d  color: var(--jp-
-0008c970: 6365 6c6c 2d69 6e70 726f 6d70 742d 666f  cell-inprompt-fo
-0008c980: 6e74 2d63 6f6c 6f72 293b 0a20 2020 2070  nt-color);.    p
-0008c990: 6164 6469 6e67 3a20 7661 7228 2d2d 6a70  adding: var(--jp
-0008c9a0: 2d63 6f64 652d 7061 6464 696e 6729 3b0a  -code-padding);.
-0008c9b0: 2020 2020 7061 6464 696e 672d 6c65 6674      padding-left
-0008c9c0: 3a20 3132 7078 3b0a 2020 2020 666f 6e74  : 12px;.    font
-0008c9d0: 2d66 616d 696c 793a 2076 6172 282d 2d6a  -family: var(--j
-0008c9e0: 702d 6365 6c6c 2d70 726f 6d70 742d 666f  p-cell-prompt-fo
-0008c9f0: 6e74 2d66 616d 696c 7929 3b0a 2020 2020  nt-family);.    
-0008ca00: 6c65 7474 6572 2d73 7061 6369 6e67 3a20  letter-spacing: 
-0008ca10: 7661 7228 2d2d 6a70 2d63 656c 6c2d 7072  var(--jp-cell-pr
-0008ca20: 6f6d 7074 2d6c 6574 7465 722d 7370 6163  ompt-letter-spac
-0008ca30: 696e 6729 3b0a 2020 2020 6c69 6e65 2d68  ing);.    line-h
-0008ca40: 6569 6768 743a 2031 2e39 3b0a 2020 2020  eight: 1.9;.    
-0008ca50: 666f 6e74 2d73 697a 653a 2076 6172 282d  font-size: var(-
-0008ca60: 2d6a 702d 636f 6465 2d66 6f6e 742d 7369  -jp-code-font-si
-0008ca70: 7a65 293b 0a20 2020 2062 6f72 6465 723a  ze);.    border:
-0008ca80: 2076 6172 282d 2d6a 702d 626f 7264 6572   var(--jp-border
-0008ca90: 2d77 6964 7468 2920 736f 6c69 6420 7472  -width) solid tr
-0008caa0: 616e 7370 6172 656e 743b 0a20 207d 0a20  ansparent;.  }. 
-0008cab0: 200a 2020 2e6a 702d 6472 6167 496d 6167   .  .jp-dragImag
-0008cac0: 652d 6d75 6c74 6970 6c65 4261 636b 207b  e-multipleBack {
-0008cad0: 0a20 2020 207a 2d69 6e64 6578 3a20 2d31  .    z-index: -1
-0008cae0: 3b0a 2020 2020 706f 7369 7469 6f6e 3a20  ;.    position: 
-0008caf0: 6162 736f 6c75 7465 3b0a 2020 2020 6865  absolute;.    he
-0008cb00: 6967 6874 3a20 3332 7078 3b0a 2020 2020  ight: 32px;.    
-0008cb10: 7769 6474 683a 2033 3030 7078 3b0a 2020  width: 300px;.  
-0008cb20: 2020 746f 703a 2038 7078 3b0a 2020 2020    top: 8px;.    
-0008cb30: 6c65 6674 3a20 3870 783b 0a20 2020 2062  left: 8px;.    b
-0008cb40: 6163 6b67 726f 756e 643a 2076 6172 282d  ackground: var(-
-0008cb50: 2d6a 702d 6c61 796f 7574 2d63 6f6c 6f72  -jp-layout-color
-0008cb60: 3229 3b0a 2020 2020 626f 7264 6572 3a20  2);.    border: 
-0008cb70: 7661 7228 2d2d 6a70 2d62 6f72 6465 722d  var(--jp-border-
-0008cb80: 7769 6474 6829 2073 6f6c 6964 2076 6172  width) solid var
-0008cb90: 282d 2d6a 702d 696e 7075 742d 626f 7264  (--jp-input-bord
-0008cba0: 6572 2d63 6f6c 6f72 293b 0a20 2020 2062  er-color);.    b
-0008cbb0: 6f78 2d73 6861 646f 773a 2032 7078 2032  ox-shadow: 2px 2
-0008cbc0: 7078 2034 7078 2030 7078 2072 6762 6128  px 4px 0px rgba(
-0008cbd0: 302c 2030 2c20 302c 2030 2e31 3229 3b0a  0, 0, 0, 0.12);.
-0008cbe0: 2020 7d0a 2020 0a20 202f 2a2d 2d2d 2d2d    }.  .  /*-----
-0008cbf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0008c430: 2d2d 2d2d 2d2d 2a2f 0a20 200a 2020 2e6a  ------*/.  .  .j
+0008c440: 702d 4e6f 7465 626f 6f6b 2d63 656c 6c2e  p-Notebook-cell.
+0008c450: 6a70 2d6d 6f64 2d64 726f 7053 6f75 7263  jp-mod-dropSourc
+0008c460: 6520 7b0a 2020 2020 6f70 6163 6974 793a  e {.    opacity:
+0008c470: 2030 2e35 3b0a 2020 7d0a 2020 0a20 202e   0.5;.  }.  .  .
+0008c480: 6a70 2d4e 6f74 6562 6f6f 6b2d 6365 6c6c  jp-Notebook-cell
+0008c490: 2e6a 702d 6d6f 642d 6472 6f70 5461 7267  .jp-mod-dropTarg
+0008c4a0: 6574 2c0a 2020 2e6a 702d 4e6f 7465 626f  et,.  .jp-Notebo
+0008c4b0: 6f6b 2e6a 702d 6d6f 642d 636f 6d6d 616e  ok.jp-mod-comman
+0008c4c0: 644d 6f64 650a 2020 2020 2e6a 702d 4e6f  dMode.    .jp-No
+0008c4d0: 7465 626f 6f6b 2d63 656c 6c2e 6a70 2d6d  tebook-cell.jp-m
+0008c4e0: 6f64 2d61 6374 6976 652e 6a70 2d6d 6f64  od-active.jp-mod
+0008c4f0: 2d73 656c 6563 7465 642e 6a70 2d6d 6f64  -selected.jp-mod
+0008c500: 2d64 726f 7054 6172 6765 7420 7b0a 2020  -dropTarget {.  
+0008c510: 2020 626f 7264 6572 2d74 6f70 2d63 6f6c    border-top-col
+0008c520: 6f72 3a20 7661 7228 2d2d 6a70 2d70 7269  or: var(--jp-pri
+0008c530: 7661 7465 2d6e 6f74 6562 6f6f 6b2d 7365  vate-notebook-se
+0008c540: 6c65 6374 6564 2d63 6f6c 6f72 293b 0a20  lected-color);. 
+0008c550: 2020 2062 6f72 6465 722d 746f 702d 7374     border-top-st
+0008c560: 796c 653a 2073 6f6c 6964 3b0a 2020 2020  yle: solid;.    
+0008c570: 626f 7264 6572 2d74 6f70 2d77 6964 7468  border-top-width
+0008c580: 3a20 3270 783b 0a20 207d 0a20 200a 2020  : 2px;.  }.  .  
+0008c590: 2e6a 702d 6472 6167 496d 6167 6520 7b0a  .jp-dragImage {.
+0008c5a0: 2020 2020 6469 7370 6c61 793a 2062 6c6f      display: blo
+0008c5b0: 636b 3b0a 2020 2020 666c 6578 2d64 6972  ck;.    flex-dir
+0008c5c0: 6563 7469 6f6e 3a20 726f 773b 0a20 2020  ection: row;.   
+0008c5d0: 2077 6964 7468 3a20 7661 7228 2d2d 6a70   width: var(--jp
+0008c5e0: 2d70 7269 7661 7465 2d6e 6f74 6562 6f6f  -private-noteboo
+0008c5f0: 6b2d 6472 6167 496d 6167 652d 7769 6474  k-dragImage-widt
+0008c600: 6829 3b0a 2020 2020 6865 6967 6874 3a20  h);.    height: 
+0008c610: 7661 7228 2d2d 6a70 2d70 7269 7661 7465  var(--jp-private
+0008c620: 2d6e 6f74 6562 6f6f 6b2d 6472 6167 496d  -notebook-dragIm
+0008c630: 6167 652d 6865 6967 6874 293b 0a20 2020  age-height);.   
+0008c640: 2062 6f72 6465 723a 2076 6172 282d 2d6a   border: var(--j
+0008c650: 702d 626f 7264 6572 2d77 6964 7468 2920  p-border-width) 
+0008c660: 736f 6c69 6420 7661 7228 2d2d 6a70 2d63  solid var(--jp-c
+0008c670: 656c 6c2d 6564 6974 6f72 2d62 6f72 6465  ell-editor-borde
+0008c680: 722d 636f 6c6f 7229 3b0a 2020 2020 6261  r-color);.    ba
+0008c690: 636b 6772 6f75 6e64 3a20 7661 7228 2d2d  ckground: var(--
+0008c6a0: 6a70 2d63 656c 6c2d 6564 6974 6f72 2d62  jp-cell-editor-b
+0008c6b0: 6163 6b67 726f 756e 6429 3b0a 2020 2020  ackground);.    
+0008c6c0: 6f76 6572 666c 6f77 3a20 7669 7369 626c  overflow: visibl
+0008c6d0: 653b 0a20 207d 0a20 200a 2020 2e6a 702d  e;.  }.  .  .jp-
+0008c6e0: 6472 6167 496d 6167 652d 7369 6e67 6c65  dragImage-single
+0008c6f0: 5072 6f6d 7074 207b 0a20 2020 2062 6f78  Prompt {.    box
+0008c700: 2d73 6861 646f 773a 2032 7078 2032 7078  -shadow: 2px 2px
+0008c710: 2034 7078 2030 7078 2072 6762 6128 302c   4px 0px rgba(0,
+0008c720: 2030 2c20 302c 2030 2e31 3229 3b0a 2020   0, 0, 0.12);.  
+0008c730: 7d0a 2020 0a20 202e 6a70 2d64 7261 6749  }.  .  .jp-dragI
+0008c740: 6d61 6765 202e 6a70 2d64 7261 6749 6d61  mage .jp-dragIma
+0008c750: 6765 2d63 6f6e 7465 6e74 207b 0a20 2020  ge-content {.   
+0008c760: 2066 6c65 783a 2031 2031 2061 7574 6f3b   flex: 1 1 auto;
+0008c770: 0a20 2020 207a 2d69 6e64 6578 3a20 323b  .    z-index: 2;
+0008c780: 0a20 2020 2066 6f6e 742d 7369 7a65 3a20  .    font-size: 
+0008c790: 7661 7228 2d2d 6a70 2d63 6f64 652d 666f  var(--jp-code-fo
+0008c7a0: 6e74 2d73 697a 6529 3b0a 2020 2020 666f  nt-size);.    fo
+0008c7b0: 6e74 2d66 616d 696c 793a 2076 6172 282d  nt-family: var(-
+0008c7c0: 2d6a 702d 636f 6465 2d66 6f6e 742d 6661  -jp-code-font-fa
+0008c7d0: 6d69 6c79 293b 0a20 2020 206c 696e 652d  mily);.    line-
+0008c7e0: 6865 6967 6874 3a20 7661 7228 2d2d 6a70  height: var(--jp
+0008c7f0: 2d63 6f64 652d 6c69 6e65 2d68 6569 6768  -code-line-heigh
+0008c800: 7429 3b0a 2020 2020 7061 6464 696e 673a  t);.    padding:
+0008c810: 2076 6172 282d 2d6a 702d 636f 6465 2d70   var(--jp-code-p
+0008c820: 6164 6469 6e67 293b 0a20 2020 2062 6f72  adding);.    bor
+0008c830: 6465 723a 2076 6172 282d 2d6a 702d 626f  der: var(--jp-bo
+0008c840: 7264 6572 2d77 6964 7468 2920 736f 6c69  rder-width) soli
+0008c850: 6420 7661 7228 2d2d 6a70 2d63 656c 6c2d  d var(--jp-cell-
+0008c860: 6564 6974 6f72 2d62 6f72 6465 722d 636f  editor-border-co
+0008c870: 6c6f 7229 3b0a 2020 2020 6261 636b 6772  lor);.    backgr
+0008c880: 6f75 6e64 3a20 7661 7228 2d2d 6a70 2d63  ound: var(--jp-c
+0008c890: 656c 6c2d 6564 6974 6f72 2d62 6163 6b67  ell-editor-backg
+0008c8a0: 726f 756e 642d 636f 6c6f 7229 3b0a 2020  round-color);.  
+0008c8b0: 2020 636f 6c6f 723a 2076 6172 282d 2d6a    color: var(--j
+0008c8c0: 702d 636f 6e74 656e 742d 666f 6e74 2d63  p-content-font-c
+0008c8d0: 6f6c 6f72 3329 3b0a 2020 2020 7465 7874  olor3);.    text
+0008c8e0: 2d61 6c69 676e 3a20 6c65 6674 3b0a 2020  -align: left;.  
+0008c8f0: 2020 6d61 7267 696e 3a20 3470 7820 3470    margin: 4px 4p
+0008c900: 7820 3470 7820 3070 783b 0a20 207d 0a20  x 4px 0px;.  }. 
+0008c910: 200a 2020 2e6a 702d 6472 6167 496d 6167   .  .jp-dragImag
+0008c920: 6520 2e6a 702d 6472 6167 496d 6167 652d  e .jp-dragImage-
+0008c930: 7072 6f6d 7074 207b 0a20 2020 2066 6c65  prompt {.    fle
+0008c940: 783a 2030 2030 2061 7574 6f3b 0a20 2020  x: 0 0 auto;.   
+0008c950: 206d 696e 2d77 6964 7468 3a20 3336 7078   min-width: 36px
+0008c960: 3b0a 2020 2020 636f 6c6f 723a 2076 6172  ;.    color: var
+0008c970: 282d 2d6a 702d 6365 6c6c 2d69 6e70 726f  (--jp-cell-inpro
+0008c980: 6d70 742d 666f 6e74 2d63 6f6c 6f72 293b  mpt-font-color);
+0008c990: 0a20 2020 2070 6164 6469 6e67 3a20 7661  .    padding: va
+0008c9a0: 7228 2d2d 6a70 2d63 6f64 652d 7061 6464  r(--jp-code-padd
+0008c9b0: 696e 6729 3b0a 2020 2020 7061 6464 696e  ing);.    paddin
+0008c9c0: 672d 6c65 6674 3a20 3132 7078 3b0a 2020  g-left: 12px;.  
+0008c9d0: 2020 666f 6e74 2d66 616d 696c 793a 2076    font-family: v
+0008c9e0: 6172 282d 2d6a 702d 6365 6c6c 2d70 726f  ar(--jp-cell-pro
+0008c9f0: 6d70 742d 666f 6e74 2d66 616d 696c 7929  mpt-font-family)
+0008ca00: 3b0a 2020 2020 6c65 7474 6572 2d73 7061  ;.    letter-spa
+0008ca10: 6369 6e67 3a20 7661 7228 2d2d 6a70 2d63  cing: var(--jp-c
+0008ca20: 656c 6c2d 7072 6f6d 7074 2d6c 6574 7465  ell-prompt-lette
+0008ca30: 722d 7370 6163 696e 6729 3b0a 2020 2020  r-spacing);.    
+0008ca40: 6c69 6e65 2d68 6569 6768 743a 2031 2e39  line-height: 1.9
+0008ca50: 3b0a 2020 2020 666f 6e74 2d73 697a 653a  ;.    font-size:
+0008ca60: 2076 6172 282d 2d6a 702d 636f 6465 2d66   var(--jp-code-f
+0008ca70: 6f6e 742d 7369 7a65 293b 0a20 2020 2062  ont-size);.    b
+0008ca80: 6f72 6465 723a 2076 6172 282d 2d6a 702d  order: var(--jp-
+0008ca90: 626f 7264 6572 2d77 6964 7468 2920 736f  border-width) so
+0008caa0: 6c69 6420 7472 616e 7370 6172 656e 743b  lid transparent;
+0008cab0: 0a20 207d 0a20 200a 2020 2e6a 702d 6472  .  }.  .  .jp-dr
+0008cac0: 6167 496d 6167 652d 6d75 6c74 6970 6c65  agImage-multiple
+0008cad0: 4261 636b 207b 0a20 2020 207a 2d69 6e64  Back {.    z-ind
+0008cae0: 6578 3a20 2d31 3b0a 2020 2020 706f 7369  ex: -1;.    posi
+0008caf0: 7469 6f6e 3a20 6162 736f 6c75 7465 3b0a  tion: absolute;.
+0008cb00: 2020 2020 6865 6967 6874 3a20 3332 7078      height: 32px
+0008cb10: 3b0a 2020 2020 7769 6474 683a 2033 3030  ;.    width: 300
+0008cb20: 7078 3b0a 2020 2020 746f 703a 2038 7078  px;.    top: 8px
+0008cb30: 3b0a 2020 2020 6c65 6674 3a20 3870 783b  ;.    left: 8px;
+0008cb40: 0a20 2020 2062 6163 6b67 726f 756e 643a  .    background:
+0008cb50: 2076 6172 282d 2d6a 702d 6c61 796f 7574   var(--jp-layout
+0008cb60: 2d63 6f6c 6f72 3229 3b0a 2020 2020 626f  -color2);.    bo
+0008cb70: 7264 6572 3a20 7661 7228 2d2d 6a70 2d62  rder: var(--jp-b
+0008cb80: 6f72 6465 722d 7769 6474 6829 2073 6f6c  order-width) sol
+0008cb90: 6964 2076 6172 282d 2d6a 702d 696e 7075  id var(--jp-inpu
+0008cba0: 742d 626f 7264 6572 2d63 6f6c 6f72 293b  t-border-color);
+0008cbb0: 0a20 2020 2062 6f78 2d73 6861 646f 773a  .    box-shadow:
+0008cbc0: 2032 7078 2032 7078 2034 7078 2030 7078   2px 2px 4px 0px
+0008cbd0: 2072 6762 6128 302c 2030 2c20 302c 2030   rgba(0, 0, 0, 0
+0008cbe0: 2e31 3229 3b0a 2020 7d0a 2020 0a20 202f  .12);.  }.  .  /
+0008cbf0: 2a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  *---------------
 0008cc00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008cc10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008cc20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008cc30: 2d2d 2d2d 2d2d 2d2d 0a20 207c 2043 656c  --------.  | Cel
-0008cc40: 6c20 746f 6f6c 6261 720a 2020 7c2d 2d2d  l toolbar.  |---
-0008cc50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0008cc30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
+0008cc40: 207c 2043 656c 6c20 746f 6f6c 6261 720a   | Cell toolbar.
+0008cc50: 2020 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    |-------------
 0008cc60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008cc70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008cc80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008cc90: 2d2d 2d2d 2d2d 2d2d 2d2a 2f0a 2020 0a20  ---------*/.  . 
-0008cca0: 202e 6a70 2d4e 6f74 6562 6f6f 6b54 6f6f   .jp-NotebookToo
-0008ccb0: 6c73 207b 0a20 2020 2064 6973 706c 6179  ls {.    display
-0008ccc0: 3a20 626c 6f63 6b3b 0a20 2020 206d 696e  : block;.    min
-0008ccd0: 2d77 6964 7468 3a20 7661 7228 2d2d 6a70  -width: var(--jp
-0008cce0: 2d73 6964 6562 6172 2d6d 696e 2d77 6964  -sidebar-min-wid
-0008ccf0: 7468 293b 0a20 2020 2063 6f6c 6f72 3a20  th);.    color: 
-0008cd00: 7661 7228 2d2d 6a70 2d75 692d 666f 6e74  var(--jp-ui-font
-0008cd10: 2d63 6f6c 6f72 3129 3b0a 2020 2020 6261  -color1);.    ba
-0008cd20: 636b 6772 6f75 6e64 3a20 7661 7228 2d2d  ckground: var(--
-0008cd30: 6a70 2d6c 6179 6f75 742d 636f 6c6f 7231  jp-layout-color1
-0008cd40: 293b 0a20 2020 202f 2a20 5468 6973 2069  );.    /* This i
-0008cd50: 7320 6e65 6564 6564 2073 6f20 7468 6174  s needed so that
-0008cd60: 2061 6c6c 2066 6f6e 7420 7369 7a69 6e67   all font sizing
-0008cd70: 206f 6620 6368 696c 6472 656e 2064 6f6e   of children don
-0008cd80: 6520 696e 2065 6d73 2069 730a 2020 2020  e in ems is.    
-0008cd90: 2020 2a20 7265 6c61 7469 7665 2074 6f20    * relative to 
-0008cda0: 7468 6973 2062 6173 6520 7369 7a65 202a  this base size *
-0008cdb0: 2f0a 2020 2020 666f 6e74 2d73 697a 653a  /.    font-size:
-0008cdc0: 2076 6172 282d 2d6a 702d 7569 2d66 6f6e   var(--jp-ui-fon
-0008cdd0: 742d 7369 7a65 3129 3b0a 2020 2020 6f76  t-size1);.    ov
-0008cde0: 6572 666c 6f77 3a20 6175 746f 3b0a 2020  erflow: auto;.  
-0008cdf0: 7d0a 2020 0a20 202e 6a70 2d4e 6f74 6562  }.  .  .jp-Noteb
-0008ce00: 6f6f 6b54 6f6f 6c73 2d74 6f6f 6c20 7b0a  ookTools-tool {.
-0008ce10: 2020 2020 7061 6464 696e 673a 2030 7078      padding: 0px
-0008ce20: 2031 3270 7820 3020 3132 7078 3b0a 2020   12px 0 12px;.  
-0008ce30: 7d0a 2020 0a20 202e 6a70 2d41 6374 6976  }.  .  .jp-Activ
-0008ce40: 6543 656c 6c54 6f6f 6c20 7b0a 2020 2020  eCellTool {.    
-0008ce50: 7061 6464 696e 673a 2031 3270 783b 0a20  padding: 12px;. 
-0008ce60: 2020 2062 6163 6b67 726f 756e 642d 636f     background-co
-0008ce70: 6c6f 723a 2076 6172 282d 2d6a 702d 6c61  lor: var(--jp-la
-0008ce80: 796f 7574 2d63 6f6c 6f72 3129 3b0a 2020  yout-color1);.  
-0008ce90: 2020 626f 7264 6572 2d74 6f70 3a20 6e6f    border-top: no
-0008cea0: 6e65 2021 696d 706f 7274 616e 743b 0a20  ne !important;. 
-0008ceb0: 207d 0a20 200a 2020 2e6a 702d 4163 7469   }.  .  .jp-Acti
-0008cec0: 7665 4365 6c6c 546f 6f6c 202e 6a70 2d49  veCellTool .jp-I
-0008ced0: 6e70 7574 4172 6561 2d70 726f 6d70 7420  nputArea-prompt 
-0008cee0: 7b0a 2020 2020 666c 6578 3a20 3020 3020  {.    flex: 0 0 
-0008cef0: 6175 746f 3b0a 2020 2020 7061 6464 696e  auto;.    paddin
-0008cf00: 672d 6c65 6674 3a20 3070 783b 0a20 207d  g-left: 0px;.  }
-0008cf10: 0a20 200a 2020 2e6a 702d 4163 7469 7665  .  .  .jp-Active
-0008cf20: 4365 6c6c 546f 6f6c 202e 6a70 2d49 6e70  CellTool .jp-Inp
-0008cf30: 7574 4172 6561 2d65 6469 746f 7220 7b0a  utArea-editor {.
-0008cf40: 2020 2020 666c 6578 3a20 3120 3120 6175      flex: 1 1 au
-0008cf50: 746f 3b0a 2020 2020 6261 636b 6772 6f75  to;.    backgrou
-0008cf60: 6e64 3a20 7661 7228 2d2d 6a70 2d63 656c  nd: var(--jp-cel
-0008cf70: 6c2d 6564 6974 6f72 2d62 6163 6b67 726f  l-editor-backgro
-0008cf80: 756e 6429 3b0a 2020 2020 626f 7264 6572  und);.    border
-0008cf90: 2d63 6f6c 6f72 3a20 7661 7228 2d2d 6a70  -color: var(--jp
-0008cfa0: 2d63 656c 6c2d 6564 6974 6f72 2d62 6f72  -cell-editor-bor
-0008cfb0: 6465 722d 636f 6c6f 7229 3b0a 2020 7d0a  der-color);.  }.
-0008cfc0: 2020 0a20 202e 6a70 2d41 6374 6976 6543    .  .jp-ActiveC
-0008cfd0: 656c 6c54 6f6f 6c20 2e6a 702d 496e 7075  ellTool .jp-Inpu
-0008cfe0: 7441 7265 612d 6564 6974 6f72 202e 436f  tArea-editor .Co
-0008cff0: 6465 4d69 7272 6f72 207b 0a20 2020 2062  deMirror {.    b
-0008d000: 6163 6b67 726f 756e 643a 2074 7261 6e73  ackground: trans
-0008d010: 7061 7265 6e74 3b0a 2020 7d0a 2020 0a20  parent;.  }.  . 
-0008d020: 202e 6a70 2d4d 6574 6164 6174 6145 6469   .jp-MetadataEdi
-0008d030: 746f 7254 6f6f 6c20 7b0a 2020 2020 666c  torTool {.    fl
-0008d040: 6578 2d64 6972 6563 7469 6f6e 3a20 636f  ex-direction: co
-0008d050: 6c75 6d6e 3b0a 2020 2020 7061 6464 696e  lumn;.    paddin
-0008d060: 673a 2031 3270 7820 3070 7820 3132 7078  g: 12px 0px 12px
-0008d070: 2030 7078 3b0a 2020 7d0a 2020 0a20 202e   0px;.  }.  .  .
-0008d080: 6a70 2d52 616e 6b65 6450 616e 656c 203e  jp-RankedPanel >
-0008d090: 203a 6e6f 7428 3a66 6972 7374 2d63 6869   :not(:first-chi
-0008d0a0: 6c64 2920 7b0a 2020 2020 6d61 7267 696e  ld) {.    margin
-0008d0b0: 2d74 6f70 3a20 3132 7078 3b0a 2020 7d0a  -top: 12px;.  }.
-0008d0c0: 2020 0a20 202e 6a70 2d4b 6579 5365 6c65    .  .jp-KeySele
-0008d0d0: 6374 6f72 2073 656c 6563 742e 6a70 2d6d  ctor select.jp-m
-0008d0e0: 6f64 2d73 7479 6c65 6420 7b0a 2020 2020  od-styled {.    
-0008d0f0: 666f 6e74 2d73 697a 653a 2076 6172 282d  font-size: var(-
-0008d100: 2d6a 702d 7569 2d66 6f6e 742d 7369 7a65  -jp-ui-font-size
-0008d110: 3129 3b0a 2020 2020 636f 6c6f 723a 2076  1);.    color: v
-0008d120: 6172 282d 2d6a 702d 7569 2d66 6f6e 742d  ar(--jp-ui-font-
-0008d130: 636f 6c6f 7230 293b 0a20 2020 2062 6f72  color0);.    bor
-0008d140: 6465 723a 2076 6172 282d 2d6a 702d 626f  der: var(--jp-bo
-0008d150: 7264 6572 2d77 6964 7468 2920 736f 6c69  rder-width) soli
-0008d160: 6420 7661 7228 2d2d 6a70 2d62 6f72 6465  d var(--jp-borde
-0008d170: 722d 636f 6c6f 7231 293b 0a20 207d 0a20  r-color1);.  }. 
-0008d180: 200a 2020 2e6a 702d 4b65 7953 656c 6563   .  .jp-KeySelec
-0008d190: 746f 7220 6c61 6265 6c2c 0a20 202e 6a70  tor label,.  .jp
-0008d1a0: 2d4d 6574 6164 6174 6145 6469 746f 7254  -MetadataEditorT
-0008d1b0: 6f6f 6c20 6c61 6265 6c20 7b0a 2020 2020  ool label {.    
-0008d1c0: 6c69 6e65 2d68 6569 6768 743a 2031 2e34  line-height: 1.4
-0008d1d0: 3b0a 2020 7d0a 2020 0a20 202e 6a70 2d4e  ;.  }.  .  .jp-N
-0008d1e0: 6f74 6562 6f6f 6b54 6f6f 6c73 202e 6a70  otebookTools .jp
-0008d1f0: 2d73 656c 6563 742d 7772 6170 7065 7220  -select-wrapper 
-0008d200: 7b0a 2020 2020 6d61 7267 696e 2d74 6f70  {.    margin-top
-0008d210: 3a20 3470 783b 0a20 2020 206d 6172 6769  : 4px;.    margi
-0008d220: 6e2d 626f 7474 6f6d 3a20 3070 783b 0a20  n-bottom: 0px;. 
-0008d230: 207d 0a20 200a 2020 2e6a 702d 4e6f 7465   }.  .  .jp-Note
-0008d240: 626f 6f6b 546f 6f6c 7320 2e6a 702d 436f  bookTools .jp-Co
-0008d250: 6c6c 6170 7365 207b 0a20 2020 206d 6172  llapse {.    mar
-0008d260: 6769 6e2d 746f 703a 2031 3670 783b 0a20  gin-top: 16px;. 
-0008d270: 207d 0a20 200a 2020 2f2a 2d2d 2d2d 2d2d   }.  .  /*------
+0008cc90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2a  ---------------*
+0008cca0: 2f0a 2020 0a20 202e 6a70 2d4e 6f74 6562  /.  .  .jp-Noteb
+0008ccb0: 6f6f 6b54 6f6f 6c73 207b 0a20 2020 2064  ookTools {.    d
+0008ccc0: 6973 706c 6179 3a20 626c 6f63 6b3b 0a20  isplay: block;. 
+0008ccd0: 2020 206d 696e 2d77 6964 7468 3a20 7661     min-width: va
+0008cce0: 7228 2d2d 6a70 2d73 6964 6562 6172 2d6d  r(--jp-sidebar-m
+0008ccf0: 696e 2d77 6964 7468 293b 0a20 2020 2063  in-width);.    c
+0008cd00: 6f6c 6f72 3a20 7661 7228 2d2d 6a70 2d75  olor: var(--jp-u
+0008cd10: 692d 666f 6e74 2d63 6f6c 6f72 3129 3b0a  i-font-color1);.
+0008cd20: 2020 2020 6261 636b 6772 6f75 6e64 3a20      background: 
+0008cd30: 7661 7228 2d2d 6a70 2d6c 6179 6f75 742d  var(--jp-layout-
+0008cd40: 636f 6c6f 7231 293b 0a20 2020 202f 2a20  color1);.    /* 
+0008cd50: 5468 6973 2069 7320 6e65 6564 6564 2073  This is needed s
+0008cd60: 6f20 7468 6174 2061 6c6c 2066 6f6e 7420  o that all font 
+0008cd70: 7369 7a69 6e67 206f 6620 6368 696c 6472  sizing of childr
+0008cd80: 656e 2064 6f6e 6520 696e 2065 6d73 2069  en done in ems i
+0008cd90: 730a 2020 2020 2020 2a20 7265 6c61 7469  s.      * relati
+0008cda0: 7665 2074 6f20 7468 6973 2062 6173 6520  ve to this base 
+0008cdb0: 7369 7a65 202a 2f0a 2020 2020 666f 6e74  size */.    font
+0008cdc0: 2d73 697a 653a 2076 6172 282d 2d6a 702d  -size: var(--jp-
+0008cdd0: 7569 2d66 6f6e 742d 7369 7a65 3129 3b0a  ui-font-size1);.
+0008cde0: 2020 2020 6f76 6572 666c 6f77 3a20 6175      overflow: au
+0008cdf0: 746f 3b0a 2020 7d0a 2020 0a20 202e 6a70  to;.  }.  .  .jp
+0008ce00: 2d4e 6f74 6562 6f6f 6b54 6f6f 6c73 2d74  -NotebookTools-t
+0008ce10: 6f6f 6c20 7b0a 2020 2020 7061 6464 696e  ool {.    paddin
+0008ce20: 673a 2030 7078 2031 3270 7820 3020 3132  g: 0px 12px 0 12
+0008ce30: 7078 3b0a 2020 7d0a 2020 0a20 202e 6a70  px;.  }.  .  .jp
+0008ce40: 2d41 6374 6976 6543 656c 6c54 6f6f 6c20  -ActiveCellTool 
+0008ce50: 7b0a 2020 2020 7061 6464 696e 673a 2031  {.    padding: 1
+0008ce60: 3270 783b 0a20 2020 2062 6163 6b67 726f  2px;.    backgro
+0008ce70: 756e 642d 636f 6c6f 723a 2076 6172 282d  und-color: var(-
+0008ce80: 2d6a 702d 6c61 796f 7574 2d63 6f6c 6f72  -jp-layout-color
+0008ce90: 3129 3b0a 2020 2020 626f 7264 6572 2d74  1);.    border-t
+0008cea0: 6f70 3a20 6e6f 6e65 2021 696d 706f 7274  op: none !import
+0008ceb0: 616e 743b 0a20 207d 0a20 200a 2020 2e6a  ant;.  }.  .  .j
+0008cec0: 702d 4163 7469 7665 4365 6c6c 546f 6f6c  p-ActiveCellTool
+0008ced0: 202e 6a70 2d49 6e70 7574 4172 6561 2d70   .jp-InputArea-p
+0008cee0: 726f 6d70 7420 7b0a 2020 2020 666c 6578  rompt {.    flex
+0008cef0: 3a20 3020 3020 6175 746f 3b0a 2020 2020  : 0 0 auto;.    
+0008cf00: 7061 6464 696e 672d 6c65 6674 3a20 3070  padding-left: 0p
+0008cf10: 783b 0a20 207d 0a20 200a 2020 2e6a 702d  x;.  }.  .  .jp-
+0008cf20: 4163 7469 7665 4365 6c6c 546f 6f6c 202e  ActiveCellTool .
+0008cf30: 6a70 2d49 6e70 7574 4172 6561 2d65 6469  jp-InputArea-edi
+0008cf40: 746f 7220 7b0a 2020 2020 666c 6578 3a20  tor {.    flex: 
+0008cf50: 3120 3120 6175 746f 3b0a 2020 2020 6261  1 1 auto;.    ba
+0008cf60: 636b 6772 6f75 6e64 3a20 7661 7228 2d2d  ckground: var(--
+0008cf70: 6a70 2d63 656c 6c2d 6564 6974 6f72 2d62  jp-cell-editor-b
+0008cf80: 6163 6b67 726f 756e 6429 3b0a 2020 2020  ackground);.    
+0008cf90: 626f 7264 6572 2d63 6f6c 6f72 3a20 7661  border-color: va
+0008cfa0: 7228 2d2d 6a70 2d63 656c 6c2d 6564 6974  r(--jp-cell-edit
+0008cfb0: 6f72 2d62 6f72 6465 722d 636f 6c6f 7229  or-border-color)
+0008cfc0: 3b0a 2020 7d0a 2020 0a20 202e 6a70 2d41  ;.  }.  .  .jp-A
+0008cfd0: 6374 6976 6543 656c 6c54 6f6f 6c20 2e6a  ctiveCellTool .j
+0008cfe0: 702d 496e 7075 7441 7265 612d 6564 6974  p-InputArea-edit
+0008cff0: 6f72 202e 436f 6465 4d69 7272 6f72 207b  or .CodeMirror {
+0008d000: 0a20 2020 2062 6163 6b67 726f 756e 643a  .    background:
+0008d010: 2074 7261 6e73 7061 7265 6e74 3b0a 2020   transparent;.  
+0008d020: 7d0a 2020 0a20 202e 6a70 2d4d 6574 6164  }.  .  .jp-Metad
+0008d030: 6174 6145 6469 746f 7254 6f6f 6c20 7b0a  ataEditorTool {.
+0008d040: 2020 2020 666c 6578 2d64 6972 6563 7469      flex-directi
+0008d050: 6f6e 3a20 636f 6c75 6d6e 3b0a 2020 2020  on: column;.    
+0008d060: 7061 6464 696e 673a 2031 3270 7820 3070  padding: 12px 0p
+0008d070: 7820 3132 7078 2030 7078 3b0a 2020 7d0a  x 12px 0px;.  }.
+0008d080: 2020 0a20 202e 6a70 2d52 616e 6b65 6450    .  .jp-RankedP
+0008d090: 616e 656c 203e 203a 6e6f 7428 3a66 6972  anel > :not(:fir
+0008d0a0: 7374 2d63 6869 6c64 2920 7b0a 2020 2020  st-child) {.    
+0008d0b0: 6d61 7267 696e 2d74 6f70 3a20 3132 7078  margin-top: 12px
+0008d0c0: 3b0a 2020 7d0a 2020 0a20 202e 6a70 2d4b  ;.  }.  .  .jp-K
+0008d0d0: 6579 5365 6c65 6374 6f72 2073 656c 6563  eySelector selec
+0008d0e0: 742e 6a70 2d6d 6f64 2d73 7479 6c65 6420  t.jp-mod-styled 
+0008d0f0: 7b0a 2020 2020 666f 6e74 2d73 697a 653a  {.    font-size:
+0008d100: 2076 6172 282d 2d6a 702d 7569 2d66 6f6e   var(--jp-ui-fon
+0008d110: 742d 7369 7a65 3129 3b0a 2020 2020 636f  t-size1);.    co
+0008d120: 6c6f 723a 2076 6172 282d 2d6a 702d 7569  lor: var(--jp-ui
+0008d130: 2d66 6f6e 742d 636f 6c6f 7230 293b 0a20  -font-color0);. 
+0008d140: 2020 2062 6f72 6465 723a 2076 6172 282d     border: var(-
+0008d150: 2d6a 702d 626f 7264 6572 2d77 6964 7468  -jp-border-width
+0008d160: 2920 736f 6c69 6420 7661 7228 2d2d 6a70  ) solid var(--jp
+0008d170: 2d62 6f72 6465 722d 636f 6c6f 7231 293b  -border-color1);
+0008d180: 0a20 207d 0a20 200a 2020 2e6a 702d 4b65  .  }.  .  .jp-Ke
+0008d190: 7953 656c 6563 746f 7220 6c61 6265 6c2c  ySelector label,
+0008d1a0: 0a20 202e 6a70 2d4d 6574 6164 6174 6145  .  .jp-MetadataE
+0008d1b0: 6469 746f 7254 6f6f 6c20 6c61 6265 6c20  ditorTool label 
+0008d1c0: 7b0a 2020 2020 6c69 6e65 2d68 6569 6768  {.    line-heigh
+0008d1d0: 743a 2031 2e34 3b0a 2020 7d0a 2020 0a20  t: 1.4;.  }.  . 
+0008d1e0: 202e 6a70 2d4e 6f74 6562 6f6f 6b54 6f6f   .jp-NotebookToo
+0008d1f0: 6c73 202e 6a70 2d73 656c 6563 742d 7772  ls .jp-select-wr
+0008d200: 6170 7065 7220 7b0a 2020 2020 6d61 7267  apper {.    marg
+0008d210: 696e 2d74 6f70 3a20 3470 783b 0a20 2020  in-top: 4px;.   
+0008d220: 206d 6172 6769 6e2d 626f 7474 6f6d 3a20   margin-bottom: 
+0008d230: 3070 783b 0a20 207d 0a20 200a 2020 2e6a  0px;.  }.  .  .j
+0008d240: 702d 4e6f 7465 626f 6f6b 546f 6f6c 7320  p-NotebookTools 
+0008d250: 2e6a 702d 436f 6c6c 6170 7365 207b 0a20  .jp-Collapse {. 
+0008d260: 2020 206d 6172 6769 6e2d 746f 703a 2031     margin-top: 1
+0008d270: 3670 783b 0a20 207d 0a20 200a 2020 2f2a  6px;.  }.  .  /*
 0008d280: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008d290: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008d2a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008d2b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008d2c0: 2d2d 2d2d 2d2d 2d0a 2020 7c20 5072 6573  -------.  | Pres
-0008d2d0: 656e 7461 7469 6f6e 204d 6f64 6520 282e  entation Mode (.
-0008d2e0: 6a70 2d6d 6f64 2d70 7265 7365 6e74 6174  jp-mod-presentat
-0008d2f0: 696f 6e4d 6f64 6529 0a20 207c 2d2d 2d2d  ionMode).  |----
-0008d300: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0008d2c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
+0008d2d0: 7c20 5072 6573 656e 7461 7469 6f6e 204d  | Presentation M
+0008d2e0: 6f64 6520 282e 6a70 2d6d 6f64 2d70 7265  ode (.jp-mod-pre
+0008d2f0: 7365 6e74 6174 696f 6e4d 6f64 6529 0a20  sentationMode). 
+0008d300: 207c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |--------------
 0008d310: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008d320: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008d330: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008d340: 2d2d 2d2d 2d2d 2d2d 2a2f 0a20 200a 2020  --------*/.  .  
-0008d350: 2e6a 702d 6d6f 642d 7072 6573 656e 7461  .jp-mod-presenta
-0008d360: 7469 6f6e 4d6f 6465 202e 6a70 2d4e 6f74  tionMode .jp-Not
-0008d370: 6562 6f6f 6b20 7b0a 2020 2020 2d2d 6a70  ebook {.    --jp
-0008d380: 2d63 6f6e 7465 6e74 2d66 6f6e 742d 7369  -content-font-si
-0008d390: 7a65 313a 2076 6172 282d 2d6a 702d 636f  ze1: var(--jp-co
-0008d3a0: 6e74 656e 742d 7072 6573 656e 7461 7469  ntent-presentati
-0008d3b0: 6f6e 2d66 6f6e 742d 7369 7a65 3129 3b0a  on-font-size1);.
-0008d3c0: 2020 2020 2d2d 6a70 2d63 6f64 652d 666f      --jp-code-fo
-0008d3d0: 6e74 2d73 697a 653a 2076 6172 282d 2d6a  nt-size: var(--j
-0008d3e0: 702d 636f 6465 2d70 7265 7365 6e74 6174  p-code-presentat
-0008d3f0: 696f 6e2d 666f 6e74 2d73 697a 6529 3b0a  ion-font-size);.
-0008d400: 2020 7d0a 2020 0a20 202f 2a20 2e6a 702d    }.  .  /* .jp-
-0008d410: 6d6f 642d 7072 6573 656e 7461 7469 6f6e  mod-presentation
-0008d420: 4d6f 6465 202e 6a70 2d4e 6f74 6562 6f6f  Mode .jp-Noteboo
-0008d430: 6b20 2e6a 702d 4365 6c6c 202e 6a70 2d49  k .jp-Cell .jp-I
-0008d440: 6e70 7574 5072 6f6d 7074 2c0a 2020 2e6a  nputPrompt,.  .j
-0008d450: 702d 6d6f 642d 7072 6573 656e 7461 7469  p-mod-presentati
-0008d460: 6f6e 4d6f 6465 202e 6a70 2d4e 6f74 6562  onMode .jp-Noteb
-0008d470: 6f6f 6b20 2e6a 702d 4365 6c6c 202e 6a70  ook .jp-Cell .jp
-0008d480: 2d4f 7574 7075 7450 726f 6d70 7420 7b0a  -OutputPrompt {.
-0008d490: 2020 2020 666c 6578 3a20 3020 3020 3131      flex: 0 0 11
-0008d4a0: 3070 783b 0a20 207d 202a 2f0a 2020 0a20  0px;.  } */.  . 
-0008d4b0: 202f 2a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   /*-------------
+0008d340: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2a2f  --------------*/
+0008d350: 0a20 200a 2020 2e6a 702d 6d6f 642d 7072  .  .  .jp-mod-pr
+0008d360: 6573 656e 7461 7469 6f6e 4d6f 6465 202e  esentationMode .
+0008d370: 6a70 2d4e 6f74 6562 6f6f 6b20 7b0a 2020  jp-Notebook {.  
+0008d380: 2020 2d2d 6a70 2d63 6f6e 7465 6e74 2d66    --jp-content-f
+0008d390: 6f6e 742d 7369 7a65 313a 2076 6172 282d  ont-size1: var(-
+0008d3a0: 2d6a 702d 636f 6e74 656e 742d 7072 6573  -jp-content-pres
+0008d3b0: 656e 7461 7469 6f6e 2d66 6f6e 742d 7369  entation-font-si
+0008d3c0: 7a65 3129 3b0a 2020 2020 2d2d 6a70 2d63  ze1);.    --jp-c
+0008d3d0: 6f64 652d 666f 6e74 2d73 697a 653a 2076  ode-font-size: v
+0008d3e0: 6172 282d 2d6a 702d 636f 6465 2d70 7265  ar(--jp-code-pre
+0008d3f0: 7365 6e74 6174 696f 6e2d 666f 6e74 2d73  sentation-font-s
+0008d400: 697a 6529 3b0a 2020 7d0a 2020 0a20 202f  ize);.  }.  .  /
+0008d410: 2a20 2e6a 702d 6d6f 642d 7072 6573 656e  * .jp-mod-presen
+0008d420: 7461 7469 6f6e 4d6f 6465 202e 6a70 2d4e  tationMode .jp-N
+0008d430: 6f74 6562 6f6f 6b20 2e6a 702d 4365 6c6c  otebook .jp-Cell
+0008d440: 202e 6a70 2d49 6e70 7574 5072 6f6d 7074   .jp-InputPrompt
+0008d450: 2c0a 2020 2e6a 702d 6d6f 642d 7072 6573  ,.  .jp-mod-pres
+0008d460: 656e 7461 7469 6f6e 4d6f 6465 202e 6a70  entationMode .jp
+0008d470: 2d4e 6f74 6562 6f6f 6b20 2e6a 702d 4365  -Notebook .jp-Ce
+0008d480: 6c6c 202e 6a70 2d4f 7574 7075 7450 726f  ll .jp-OutputPro
+0008d490: 6d70 7420 7b0a 2020 2020 666c 6578 3a20  mpt {.    flex: 
+0008d4a0: 3020 3020 3131 3070 783b 0a20 207d 202a  0 0 110px;.  } *
+0008d4b0: 2f0a 2020 0a20 202f 2a2d 2d2d 2d2d 2d2d  /.  .  /*-------
 0008d4c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008d4d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008d4e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008d4f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008d500: 0a20 207c 2050 6c61 6365 686f 6c64 6572  .  | Placeholder
-0008d510: 0a20 207c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .  |------------
+0008d500: 2d2d 2d2d 2d2d 0a20 207c 2050 6c61 6365  ------.  | Place
+0008d510: 686f 6c64 6572 0a20 207c 2d2d 2d2d 2d2d  holder.  |------
 0008d520: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008d530: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008d540: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0008d550: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0008d560: 2a2f 0a20 200a 2020 2e6a 702d 4365 6c6c  */.  .  .jp-Cell
-0008d570: 2d50 6c61 6365 686f 6c64 6572 207b 0a20  -Placeholder {. 
-0008d580: 2020 2070 6164 6469 6e67 2d6c 6566 743a     padding-left:
-0008d590: 2035 3570 783b 0a20 207d 0a20 200a 2020   55px;.  }.  .  
-0008d5a0: 2e6a 702d 4365 6c6c 2d50 6c61 6365 686f  .jp-Cell-Placeho
-0008d5b0: 6c64 6572 2d77 7261 7070 6572 207b 0a20  lder-wrapper {. 
-0008d5c0: 2020 2062 6163 6b67 726f 756e 643a 2023     background: #
-0008d5d0: 6666 663b 0a20 2020 2062 6f72 6465 723a  fff;.    border:
-0008d5e0: 2031 7078 2073 6f6c 6964 3b0a 2020 2020   1px solid;.    
-0008d5f0: 626f 7264 6572 2d63 6f6c 6f72 3a20 2365  border-color: #e
-0008d600: 3565 3665 3920 2364 6665 3065 3420 2364  5e6e9 #dfe0e4 #d
-0008d610: 3064 3164 353b 0a20 2020 2062 6f72 6465  0d1d5;.    borde
-0008d620: 722d 7261 6469 7573 3a20 3470 783b 0a20  r-radius: 4px;. 
-0008d630: 2020 202d 7765 626b 6974 2d62 6f72 6465     -webkit-borde
-0008d640: 722d 7261 6469 7573 3a20 3470 783b 0a20  r-radius: 4px;. 
-0008d650: 2020 206d 6172 6769 6e3a 2031 3070 7820     margin: 10px 
-0008d660: 3135 7078 3b0a 2020 7d0a 2020 0a20 202e  15px;.  }.  .  .
-0008d670: 6a70 2d43 656c 6c2d 506c 6163 6568 6f6c  jp-Cell-Placehol
-0008d680: 6465 722d 7772 6170 7065 722d 696e 6e65  der-wrapper-inne
-0008d690: 7220 7b0a 2020 2020 7061 6464 696e 673a  r {.    padding:
-0008d6a0: 2031 3570 783b 0a20 2020 2070 6f73 6974   15px;.    posit
-0008d6b0: 696f 6e3a 2072 656c 6174 6976 653b 0a20  ion: relative;. 
-0008d6c0: 207d 0a20 200a 2020 2e6a 702d 4365 6c6c   }.  .  .jp-Cell
-0008d6d0: 2d50 6c61 6365 686f 6c64 6572 2d77 7261  -Placeholder-wra
-0008d6e0: 7070 6572 2d62 6f64 7920 7b0a 2020 2020  pper-body {.    
-0008d6f0: 6261 636b 6772 6f75 6e64 2d72 6570 6561  background-repea
-0008d700: 743a 2072 6570 6561 743b 0a20 2020 2062  t: repeat;.    b
-0008d710: 6163 6b67 726f 756e 642d 7369 7a65 3a20  ackground-size: 
-0008d720: 3530 2520 6175 746f 3b0a 2020 7d0a 2020  50% auto;.  }.  
-0008d730: 0a20 202e 6a70 2d43 656c 6c2d 506c 6163  .  .jp-Cell-Plac
-0008d740: 6568 6f6c 6465 722d 7772 6170 7065 722d  eholder-wrapper-
-0008d750: 626f 6479 2064 6976 207b 0a20 2020 2062  body div {.    b
-0008d760: 6163 6b67 726f 756e 643a 2023 6636 6637  ackground: #f6f7
-0008d770: 6638 3b0a 2020 2020 6261 636b 6772 6f75  f8;.    backgrou
-0008d780: 6e64 2d69 6d61 6765 3a20 2d77 6562 6b69  nd-image: -webki
-0008d790: 742d 6c69 6e65 6172 2d67 7261 6469 656e  t-linear-gradien
-0008d7a0: 7428 0a20 2020 2020 206c 6566 742c 0a20  t(.      left,. 
-0008d7b0: 2020 2020 2023 6636 6637 6638 2030 252c       #f6f7f8 0%,
-0008d7c0: 0a20 2020 2020 2023 6564 6565 6631 2032  .      #edeef1 2
-0008d7d0: 3025 2c0a 2020 2020 2020 2366 3666 3766  0%,.      #f6f7f
-0008d7e0: 3820 3430 252c 0a20 2020 2020 2023 6636  8 40%,.      #f6
-0008d7f0: 6637 6638 2031 3030 250a 2020 2020 293b  f7f8 100%.    );
-0008d800: 0a20 2020 2062 6163 6b67 726f 756e 642d  .    background-
-0008d810: 7265 7065 6174 3a20 6e6f 2d72 6570 6561  repeat: no-repea
-0008d820: 743b 0a20 2020 2062 6163 6b67 726f 756e  t;.    backgroun
-0008d830: 642d 7369 7a65 3a20 3830 3070 7820 3130  d-size: 800px 10
-0008d840: 3470 783b 0a20 2020 2068 6569 6768 743a  4px;.    height:
-0008d850: 2031 3034 7078 3b0a 2020 2020 706f 7369   104px;.    posi
-0008d860: 7469 6f6e 3a20 7265 6c61 7469 7665 3b0a  tion: relative;.
-0008d870: 2020 7d0a 2020 0a20 202e 6a70 2d43 656c    }.  .  .jp-Cel
-0008d880: 6c2d 506c 6163 6568 6f6c 6465 722d 7772  l-Placeholder-wr
-0008d890: 6170 7065 722d 626f 6479 2064 6976 207b  apper-body div {
-0008d8a0: 0a20 2020 2070 6f73 6974 696f 6e3a 2061  .    position: a
-0008d8b0: 6273 6f6c 7574 653b 0a20 2020 2072 6967  bsolute;.    rig
-0008d8c0: 6874 3a20 3135 7078 3b0a 2020 2020 6c65  ht: 15px;.    le
-0008d8d0: 6674 3a20 3135 7078 3b0a 2020 2020 746f  ft: 15px;.    to
-0008d8e0: 703a 2031 3570 783b 0a20 207d 0a20 200a  p: 15px;.  }.  .
-0008d8f0: 2020 6469 762e 6a70 2d43 656c 6c2d 506c    div.jp-Cell-Pl
-0008d900: 6163 6568 6f6c 6465 722d 6831 207b 0a20  aceholder-h1 {. 
-0008d910: 2020 2074 6f70 3a20 3230 7078 3b0a 2020     top: 20px;.  
-0008d920: 2020 6865 6967 6874 3a20 3230 7078 3b0a    height: 20px;.
-0008d930: 2020 2020 6c65 6674 3a20 3135 7078 3b0a      left: 15px;.
-0008d940: 2020 2020 7769 6474 683a 2031 3530 7078      width: 150px
-0008d950: 3b0a 2020 7d0a 2020 0a20 2064 6976 2e6a  ;.  }.  .  div.j
-0008d960: 702d 4365 6c6c 2d50 6c61 6365 686f 6c64  p-Cell-Placehold
-0008d970: 6572 2d68 3220 7b0a 2020 2020 6c65 6674  er-h2 {.    left
-0008d980: 3a20 3135 7078 3b0a 2020 2020 746f 703a  : 15px;.    top:
-0008d990: 2035 3070 783b 0a20 2020 2068 6569 6768   50px;.    heigh
-0008d9a0: 743a 2031 3070 783b 0a20 2020 2077 6964  t: 10px;.    wid
-0008d9b0: 7468 3a20 3130 3070 783b 0a20 207d 0a20  th: 100px;.  }. 
-0008d9c0: 200a 2020 6469 762e 6a70 2d43 656c 6c2d   .  div.jp-Cell-
-0008d9d0: 506c 6163 6568 6f6c 6465 722d 636f 6e74  Placeholder-cont
-0008d9e0: 656e 742d 312c 0a20 2064 6976 2e6a 702d  ent-1,.  div.jp-
-0008d9f0: 4365 6c6c 2d50 6c61 6365 686f 6c64 6572  Cell-Placeholder
-0008da00: 2d63 6f6e 7465 6e74 2d32 2c0a 2020 6469  -content-2,.  di
-0008da10: 762e 6a70 2d43 656c 6c2d 506c 6163 6568  v.jp-Cell-Placeh
-0008da20: 6f6c 6465 722d 636f 6e74 656e 742d 3320  older-content-3 
-0008da30: 7b0a 2020 2020 6c65 6674 3a20 3135 7078  {.    left: 15px
-0008da40: 3b0a 2020 2020 7269 6768 743a 2031 3570  ;.    right: 15p
-0008da50: 783b 0a20 2020 2068 6569 6768 743a 2031  x;.    height: 1
-0008da60: 3070 783b 0a20 207d 0a20 200a 2020 6469  0px;.  }.  .  di
-0008da70: 762e 6a70 2d43 656c 6c2d 506c 6163 6568  v.jp-Cell-Placeh
-0008da80: 6f6c 6465 722d 636f 6e74 656e 742d 3120  older-content-1 
-0008da90: 7b0a 2020 2020 746f 703a 2031 3030 7078  {.    top: 100px
-0008daa0: 3b0a 2020 7d0a 2020 0a20 2064 6976 2e6a  ;.  }.  .  div.j
-0008dab0: 702d 4365 6c6c 2d50 6c61 6365 686f 6c64  p-Cell-Placehold
-0008dac0: 6572 2d63 6f6e 7465 6e74 2d32 207b 0a20  er-content-2 {. 
-0008dad0: 2020 2074 6f70 3a20 3132 3070 783b 0a20     top: 120px;. 
-0008dae0: 207d 0a20 200a 2020 6469 762e 6a70 2d43   }.  .  div.jp-C
-0008daf0: 656c 6c2d 506c 6163 6568 6f6c 6465 722d  ell-Placeholder-
-0008db00: 636f 6e74 656e 742d 3320 7b0a 2020 2020  content-3 {.    
-0008db10: 746f 703a 2031 3430 7078 3b0a 2020 7d0a  top: 140px;.  }.
-0008db20: 2020                                       
+0008d560: 2d2d 2d2d 2d2d 2a2f 0a20 200a 2020 2e6a  ------*/.  .  .j
+0008d570: 702d 4365 6c6c 2d50 6c61 6365 686f 6c64  p-Cell-Placehold
+0008d580: 6572 207b 0a20 2020 2070 6164 6469 6e67  er {.    padding
+0008d590: 2d6c 6566 743a 2035 3570 783b 0a20 207d  -left: 55px;.  }
+0008d5a0: 0a20 200a 2020 2e6a 702d 4365 6c6c 2d50  .  .  .jp-Cell-P
+0008d5b0: 6c61 6365 686f 6c64 6572 2d77 7261 7070  laceholder-wrapp
+0008d5c0: 6572 207b 0a20 2020 2062 6163 6b67 726f  er {.    backgro
+0008d5d0: 756e 643a 2023 6666 663b 0a20 2020 2062  und: #fff;.    b
+0008d5e0: 6f72 6465 723a 2031 7078 2073 6f6c 6964  order: 1px solid
+0008d5f0: 3b0a 2020 2020 626f 7264 6572 2d63 6f6c  ;.    border-col
+0008d600: 6f72 3a20 2365 3565 3665 3920 2364 6665  or: #e5e6e9 #dfe
+0008d610: 3065 3420 2364 3064 3164 353b 0a20 2020  0e4 #d0d1d5;.   
+0008d620: 2062 6f72 6465 722d 7261 6469 7573 3a20   border-radius: 
+0008d630: 3470 783b 0a20 2020 202d 7765 626b 6974  4px;.    -webkit
+0008d640: 2d62 6f72 6465 722d 7261 6469 7573 3a20  -border-radius: 
+0008d650: 3470 783b 0a20 2020 206d 6172 6769 6e3a  4px;.    margin:
+0008d660: 2031 3070 7820 3135 7078 3b0a 2020 7d0a   10px 15px;.  }.
+0008d670: 2020 0a20 202e 6a70 2d43 656c 6c2d 506c    .  .jp-Cell-Pl
+0008d680: 6163 6568 6f6c 6465 722d 7772 6170 7065  aceholder-wrappe
+0008d690: 722d 696e 6e65 7220 7b0a 2020 2020 7061  r-inner {.    pa
+0008d6a0: 6464 696e 673a 2031 3570 783b 0a20 2020  dding: 15px;.   
+0008d6b0: 2070 6f73 6974 696f 6e3a 2072 656c 6174   position: relat
+0008d6c0: 6976 653b 0a20 207d 0a20 200a 2020 2e6a  ive;.  }.  .  .j
+0008d6d0: 702d 4365 6c6c 2d50 6c61 6365 686f 6c64  p-Cell-Placehold
+0008d6e0: 6572 2d77 7261 7070 6572 2d62 6f64 7920  er-wrapper-body 
+0008d6f0: 7b0a 2020 2020 6261 636b 6772 6f75 6e64  {.    background
+0008d700: 2d72 6570 6561 743a 2072 6570 6561 743b  -repeat: repeat;
+0008d710: 0a20 2020 2062 6163 6b67 726f 756e 642d  .    background-
+0008d720: 7369 7a65 3a20 3530 2520 6175 746f 3b0a  size: 50% auto;.
+0008d730: 2020 7d0a 2020 0a20 202e 6a70 2d43 656c    }.  .  .jp-Cel
+0008d740: 6c2d 506c 6163 6568 6f6c 6465 722d 7772  l-Placeholder-wr
+0008d750: 6170 7065 722d 626f 6479 2064 6976 207b  apper-body div {
+0008d760: 0a20 2020 2062 6163 6b67 726f 756e 643a  .    background:
+0008d770: 2023 6636 6637 6638 3b0a 2020 2020 6261   #f6f7f8;.    ba
+0008d780: 636b 6772 6f75 6e64 2d69 6d61 6765 3a20  ckground-image: 
+0008d790: 2d77 6562 6b69 742d 6c69 6e65 6172 2d67  -webkit-linear-g
+0008d7a0: 7261 6469 656e 7428 0a20 2020 2020 206c  radient(.      l
+0008d7b0: 6566 742c 0a20 2020 2020 2023 6636 6637  eft,.      #f6f7
+0008d7c0: 6638 2030 252c 0a20 2020 2020 2023 6564  f8 0%,.      #ed
+0008d7d0: 6565 6631 2032 3025 2c0a 2020 2020 2020  eef1 20%,.      
+0008d7e0: 2366 3666 3766 3820 3430 252c 0a20 2020  #f6f7f8 40%,.   
+0008d7f0: 2020 2023 6636 6637 6638 2031 3030 250a     #f6f7f8 100%.
+0008d800: 2020 2020 293b 0a20 2020 2062 6163 6b67      );.    backg
+0008d810: 726f 756e 642d 7265 7065 6174 3a20 6e6f  round-repeat: no
+0008d820: 2d72 6570 6561 743b 0a20 2020 2062 6163  -repeat;.    bac
+0008d830: 6b67 726f 756e 642d 7369 7a65 3a20 3830  kground-size: 80
+0008d840: 3070 7820 3130 3470 783b 0a20 2020 2068  0px 104px;.    h
+0008d850: 6569 6768 743a 2031 3034 7078 3b0a 2020  eight: 104px;.  
+0008d860: 2020 706f 7369 7469 6f6e 3a20 7265 6c61    position: rela
+0008d870: 7469 7665 3b0a 2020 7d0a 2020 0a20 202e  tive;.  }.  .  .
+0008d880: 6a70 2d43 656c 6c2d 506c 6163 6568 6f6c  jp-Cell-Placehol
+0008d890: 6465 722d 7772 6170 7065 722d 626f 6479  der-wrapper-body
+0008d8a0: 2064 6976 207b 0a20 2020 2070 6f73 6974   div {.    posit
+0008d8b0: 696f 6e3a 2061 6273 6f6c 7574 653b 0a20  ion: absolute;. 
+0008d8c0: 2020 2072 6967 6874 3a20 3135 7078 3b0a     right: 15px;.
+0008d8d0: 2020 2020 6c65 6674 3a20 3135 7078 3b0a      left: 15px;.
+0008d8e0: 2020 2020 746f 703a 2031 3570 783b 0a20      top: 15px;. 
+0008d8f0: 207d 0a20 200a 2020 6469 762e 6a70 2d43   }.  .  div.jp-C
+0008d900: 656c 6c2d 506c 6163 6568 6f6c 6465 722d  ell-Placeholder-
+0008d910: 6831 207b 0a20 2020 2074 6f70 3a20 3230  h1 {.    top: 20
+0008d920: 7078 3b0a 2020 2020 6865 6967 6874 3a20  px;.    height: 
+0008d930: 3230 7078 3b0a 2020 2020 6c65 6674 3a20  20px;.    left: 
+0008d940: 3135 7078 3b0a 2020 2020 7769 6474 683a  15px;.    width:
+0008d950: 2031 3530 7078 3b0a 2020 7d0a 2020 0a20   150px;.  }.  . 
+0008d960: 2064 6976 2e6a 702d 4365 6c6c 2d50 6c61   div.jp-Cell-Pla
+0008d970: 6365 686f 6c64 6572 2d68 3220 7b0a 2020  ceholder-h2 {.  
+0008d980: 2020 6c65 6674 3a20 3135 7078 3b0a 2020    left: 15px;.  
+0008d990: 2020 746f 703a 2035 3070 783b 0a20 2020    top: 50px;.   
+0008d9a0: 2068 6569 6768 743a 2031 3070 783b 0a20   height: 10px;. 
+0008d9b0: 2020 2077 6964 7468 3a20 3130 3070 783b     width: 100px;
+0008d9c0: 0a20 207d 0a20 200a 2020 6469 762e 6a70  .  }.  .  div.jp
+0008d9d0: 2d43 656c 6c2d 506c 6163 6568 6f6c 6465  -Cell-Placeholde
+0008d9e0: 722d 636f 6e74 656e 742d 312c 0a20 2064  r-content-1,.  d
+0008d9f0: 6976 2e6a 702d 4365 6c6c 2d50 6c61 6365  iv.jp-Cell-Place
+0008da00: 686f 6c64 6572 2d63 6f6e 7465 6e74 2d32  holder-content-2
+0008da10: 2c0a 2020 6469 762e 6a70 2d43 656c 6c2d  ,.  div.jp-Cell-
+0008da20: 506c 6163 6568 6f6c 6465 722d 636f 6e74  Placeholder-cont
+0008da30: 656e 742d 3320 7b0a 2020 2020 6c65 6674  ent-3 {.    left
+0008da40: 3a20 3135 7078 3b0a 2020 2020 7269 6768  : 15px;.    righ
+0008da50: 743a 2031 3570 783b 0a20 2020 2068 6569  t: 15px;.    hei
+0008da60: 6768 743a 2031 3070 783b 0a20 207d 0a20  ght: 10px;.  }. 
+0008da70: 200a 2020 6469 762e 6a70 2d43 656c 6c2d   .  div.jp-Cell-
+0008da80: 506c 6163 6568 6f6c 6465 722d 636f 6e74  Placeholder-cont
+0008da90: 656e 742d 3120 7b0a 2020 2020 746f 703a  ent-1 {.    top:
+0008daa0: 2031 3030 7078 3b0a 2020 7d0a 2020 0a20   100px;.  }.  . 
+0008dab0: 2064 6976 2e6a 702d 4365 6c6c 2d50 6c61   div.jp-Cell-Pla
+0008dac0: 6365 686f 6c64 6572 2d63 6f6e 7465 6e74  ceholder-content
+0008dad0: 2d32 207b 0a20 2020 2074 6f70 3a20 3132  -2 {.    top: 12
+0008dae0: 3070 783b 0a20 207d 0a20 200a 2020 6469  0px;.  }.  .  di
+0008daf0: 762e 6a70 2d43 656c 6c2d 506c 6163 6568  v.jp-Cell-Placeh
+0008db00: 6f6c 6465 722d 636f 6e74 656e 742d 3320  older-content-3 
+0008db10: 7b0a 2020 2020 746f 703a 2031 3430 7078  {.    top: 140px
+0008db20: 3b0a 2020 7d0a 2020                      ;.  }.
```

### Comparing `mercury-2.2.9/mercury/frontend-dist/mercury_black_logo.svg` & `mercury-2.3.0/mercury/frontend-dist/mercury_black_logo.svg`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/frontend-dist/mercury_logo.svg` & `mercury-2.3.0/mercury/frontend-dist/mercury_logo.svg`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css` & `mercury-2.3.0/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css.map` & `mercury-2.3.0/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css.map`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/frontend-dist/static/css/main.26f96620.chunk.css` & `mercury-2.3.0/mercury/frontend-dist/static/css/main.80c2d41b.chunk.css`

 * *Files 6% similar despite different names*

```diff
@@ -1,2 +1,2 @@
-.filepond--credits{display:none}.loading-bullet{color:#09c!important}.uneditable-input:focus,input[type=checkbox]:focus,input[type=color]:focus,input[type=date]:focus,input[type=datetime-local]:focus,input[type=datetime]:focus,input[type=email]:focus,input[type=month]:focus,input[type=number]:focus,input[type=password]:focus,input[type=search]:focus,input[type=tel]:focus,input[type=text]:focus,input[type=time]:focus,input[type=url]:focus,input[type=week]:focus,textarea:focus{box-shadow:none;border:2px solid #2684ff}.uneditable-input:focus,div[role=slider]:focus{border:2px solid #2684ff!important}.form-check-input:checked{background-color:#2684ff!important}.thumbnailIframe{-ms-zoom:.5;zoom:.5;-moz-transform:scale(.5);-moz-transform-origin:0 0;-o-transform:scale(.5);-o-transform-origin:0 0;-webkit-transform:scale(.5);-webkit-transform-origin:0 0;transform:scale(.5);transform-origin:0 0}.sidebar{position:fixed;top:0;bottom:0;left:0;z-index:100;padding:48px 0 0;box-shadow:inset -1px 0 0 rgba(0,0,0,.1);border-left:1px solid #eee}.sidebar-sticky{position:relative;top:0;height:calc(100vh - 48px);padding-top:.5rem;overflow-x:hidden;overflow-y:auto}.sidebar .nav-link{font-weight:500;color:#333}.sidebar .nav-link .feather{margin-right:4px;color:#727272}.sidebar .nav-link.active{color:#2470dc}.sidebar .nav-link.active .feather,.sidebar .nav-link:hover .feather{color:inherit}.sidebar-heading{font-size:.75rem;text-transform:uppercase}.navbar-brand{padding-top:.75rem;padding-bottom:.75rem;font-size:1rem;background-color:rgba(0,0,0,.25);box-shadow:inset -1px 0 0 rgba(0,0,0,.25)}.navbar .navbar-toggler{top:.25rem;right:1rem}.div-signin{padding-top:60px;padding-bottom:40px}.form-signin{width:100%;max-width:330px;padding:15px;margin:0 auto}.form-signin .form-control{position:relative;box-sizing:border-box;height:auto;padding:10px;font-size:16px}.form-signin .form-control:focus{z-index:2}.form-signin input[type=email]{margin-bottom:-1px;border-bottom-right-radius:0;border-bottom-left-radius:0}.form-signin input[type=password]{margin-bottom:10px;border-top-left-radius:0;border-top-right-radius:0}.poweredby{position:absolute;top:5px;right:5px}.btn-primary{border-color:#2684ff!important;background-color:#2684ff!important}.btn-primary:hover{border-color:#217bf1!important;background-color:#217bf1!important}.title-card{background-color:rgba(38,132,255,.04)}.title-card:hover{background-color:rgba(38,132,255,.08)}body{margin:0;font-family:-apple-system,BlinkMacSystemFont,"Segoe UI","Roboto","Oxygen","Ubuntu","Cantarell","Fira Sans","Droid Sans","Helvetica Neue",sans-serif;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}code{font-family:source-code-pro,Menlo,Monaco,Consolas,"Courier New",monospace}html{position:relative;min-height:100%}
-/*# sourceMappingURL=main.26f96620.chunk.css.map */
+.filepond--credits{display:none}.loading-bullet{color:#09c!important}.uneditable-input:focus,input[type=checkbox]:focus,input[type=color]:focus,input[type=date]:focus,input[type=datetime-local]:focus,input[type=datetime]:focus,input[type=email]:focus,input[type=month]:focus,input[type=number]:focus,input[type=password]:focus,input[type=search]:focus,input[type=tel]:focus,input[type=text]:focus,input[type=time]:focus,input[type=url]:focus,input[type=week]:focus,textarea:focus{box-shadow:none;border:2px solid #2684ff}.uneditable-input:focus,div[role=slider]:focus{border:2px solid #2684ff!important}.form-check-input:checked{background-color:#2684ff!important}.thumbnailIframe{-ms-zoom:.5;zoom:.5;-moz-transform:scale(.5);-moz-transform-origin:0 0;-o-transform:scale(.5);-o-transform-origin:0 0;-webkit-transform:scale(.5);-webkit-transform-origin:0 0;transform:scale(.5);transform-origin:0 0}.sidebar{position:fixed;top:0;bottom:0;left:0;z-index:100;padding:48px 0 0;box-shadow:inset -1px 0 0 rgba(0,0,0,.1);border-left:1px solid #eee}.sidebar-sticky{position:relative;top:0;height:calc(100vh - 48px);padding-top:.5rem;overflow-x:hidden;overflow-y:auto}.sidebar .nav-link{font-weight:500;color:#333}.sidebar .nav-link .feather{margin-right:4px;color:#727272}.sidebar .nav-link.active{color:#2470dc}.sidebar .nav-link.active .feather,.sidebar .nav-link:hover .feather{color:inherit}.sidebar-heading{font-size:.75rem;text-transform:uppercase}.navbar-brand{padding-top:.75rem;padding-bottom:.75rem;font-size:1rem;background-color:rgba(0,0,0,.25);box-shadow:inset -1px 0 0 rgba(0,0,0,.25)}.navbar .navbar-toggler{top:.25rem;right:1rem}.div-signin{padding-top:60px;padding-bottom:40px}.form-signin{width:100%;max-width:330px;padding:15px;margin:0 auto}.form-signin .form-control{position:relative;box-sizing:border-box;height:auto;padding:10px;font-size:16px}.form-signin .form-control:focus{z-index:2}.form-signin input[type=email]{margin-bottom:-1px;border-bottom-right-radius:0;border-bottom-left-radius:0}.form-signin input[type=password]{margin-bottom:10px;border-top-left-radius:0;border-top-right-radius:0}.poweredby{position:absolute;top:5px;right:5px}.btn-primary{border-color:#2684ff!important;background-color:#2684ff!important}.btn-primary:hover{border-color:#217bf1!important;background-color:#217bf1!important}.btn-outline-primary{border-color:#2684ff!important;color:#2684ff!important}.btn-outline-primary:hover{border-color:#2684ff!important;color:#fff!important;background-color:#2684ff!important}.title-card{background-color:rgba(38,132,255,.04)}.title-card:hover{background-color:rgba(38,132,255,.08)}body{margin:0;font-family:-apple-system,BlinkMacSystemFont,"Segoe UI","Roboto","Oxygen","Ubuntu","Cantarell","Fira Sans","Droid Sans","Helvetica Neue",sans-serif;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}code{font-family:source-code-pro,Menlo,Monaco,Consolas,"Courier New",monospace}html{position:relative;min-height:100%}
+/*# sourceMappingURL=main.80c2d41b.chunk.css.map */
```

### Comparing `mercury-2.2.9/mercury/frontend-dist/static/css/main.26f96620.chunk.css.map` & `mercury-2.3.0/mercury/frontend-dist/static/css/main.80c2d41b.chunk.css.map`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7777777777777778%*

 * *Differences: {"'file'": "'main.80c2d41b.chunk.css'",*

 * * "'mappings'": "'AAEA,mBACE,YACF,CAIA,gBACE,oBACF,CAGA,2ZAiBE,eAAgB,CAChB,wBACF,CAEA,+CAGE,kCACF,CAEA,0BACE,kCACF,CAEA,iBACE,WAAa,CACb,OAAS,CACT,wBAA0B,CAC1B,yBAA0B,CAC1B,sBAAwB,CACxB,uBAAwB,CACxB,2BAA6B,CAC7B,4BAA6B,CAC7B,mBAAqB,CACrB,oBACF,CAMA,SACE,cAAe,CACf,KAAM,CACN,QAAS,CACT,MAAO,CACP,WAAY,CACZ,gBAAiB,CACjB,wCAA6C,CAC7C,0BACF,CAQA,gBACE,iBAAkB,CAClB,KAAM,CACN,yBAA0B,CAC1B,iBAAmB,CACnB,iBAAkB,CAClB,eACF,CAEA,mBACE,eAAgB,CAChB,UACF,CAEA,4BACE,gBAAiB,CACjB,aACF,CAE […]*

```diff
@@ -1,14 +1,14 @@
 {
-    "file": "main.26f96620.chunk.css",
-    "mappings": "AAEA,mBACE,YACF,CAIA,gBACE,oBACF,CAGA,2ZAiBE,eAAgB,CAChB,wBACF,CAEA,+CAGE,kCACF,CAEA,0BACE,kCACF,CAEA,iBACE,WAAa,CACb,OAAS,CACT,wBAA0B,CAC1B,yBAA0B,CAC1B,sBAAwB,CACxB,uBAAwB,CACxB,2BAA6B,CAC7B,4BAA6B,CAC7B,mBAAqB,CACrB,oBACF,CAMA,SACE,cAAe,CACf,KAAM,CACN,QAAS,CACT,MAAO,CACP,WAAY,CACZ,gBAAiB,CACjB,wCAA6C,CAC7C,0BACF,CAQA,gBACE,iBAAkB,CAClB,KAAM,CACN,yBAA0B,CAC1B,iBAAmB,CACnB,iBAAkB,CAClB,eACF,CAEA,mBACE,eAAgB,CAChB,UACF,CAEA,4BACE,gBAAiB,CACjB,aACF,CAEA,0BACE,aACF,CAEA,qEAEE,aACF,CAEA,iBACE,gBAAkB,CAClB,wBACF,CAMA,cACE,kBAAoB,CACpB,qBAAuB,CACvB,cAAe,CACf,gCAAqC,CACrC,yCACF,CAEA,wBACE,UAAY,CACZ,UACF,CAMA,YACE,gBAAiB,CACjB,mBAEF,CAEA,aACE,UAAW,CACX,eAAgB,CAChB,YAAa,CACb,aACF,CAEA,2BACE,iBAAkB,CAClB,qBAAsB,CACtB,WAAY,CACZ,YAAa,CACb,cACF,CACA,iCACE,SACF,CACA,+BACE,kBAAmB,CACnB,4BAA6B,CAC7B,2BACF,CACA,kCACE,kBAAmB,CACnB,wBAAyB,CACzB,yBACF,CAEA,WACE,iBAAkB,CAElB,OAAQ,CACR,SAEF,CAEA,aACE,8BAAgC,CAChC,kCACF,CAEA,mBACE,8BAAgC,CAChC,kCACF,CAEA,YACE,qCACF,CAEA,kBACE,qCACF,CC9LA,KACE,QAAS,CACT,mJAEY,CACZ,kCAAmC,CACnC,iCACF,CAEA,KACE,yEAEF,CAEA,KACE,iBAAkB,CAClB,eACF",
+    "file": "main.80c2d41b.chunk.css",
+    "mappings": "AAEA,mBACE,YACF,CAIA,gBACE,oBACF,CAGA,2ZAiBE,eAAgB,CAChB,wBACF,CAEA,+CAGE,kCACF,CAEA,0BACE,kCACF,CAEA,iBACE,WAAa,CACb,OAAS,CACT,wBAA0B,CAC1B,yBAA0B,CAC1B,sBAAwB,CACxB,uBAAwB,CACxB,2BAA6B,CAC7B,4BAA6B,CAC7B,mBAAqB,CACrB,oBACF,CAMA,SACE,cAAe,CACf,KAAM,CACN,QAAS,CACT,MAAO,CACP,WAAY,CACZ,gBAAiB,CACjB,wCAA6C,CAC7C,0BACF,CAQA,gBACE,iBAAkB,CAClB,KAAM,CACN,yBAA0B,CAC1B,iBAAmB,CACnB,iBAAkB,CAClB,eACF,CAEA,mBACE,eAAgB,CAChB,UACF,CAEA,4BACE,gBAAiB,CACjB,aACF,CAEA,0BACE,aACF,CAEA,qEAEE,aACF,CAEA,iBACE,gBAAkB,CAClB,wBACF,CAMA,cACE,kBAAoB,CACpB,qBAAuB,CACvB,cAAe,CACf,gCAAqC,CACrC,yCACF,CAEA,wBACE,UAAY,CACZ,UACF,CAMA,YACE,gBAAiB,CACjB,mBAEF,CAEA,aACE,UAAW,CACX,eAAgB,CAChB,YAAa,CACb,aACF,CAEA,2BACE,iBAAkB,CAClB,qBAAsB,CACtB,WAAY,CACZ,YAAa,CACb,cACF,CACA,iCACE,SACF,CACA,+BACE,kBAAmB,CACnB,4BAA6B,CAC7B,2BACF,CACA,kCACE,kBAAmB,CACnB,wBAAyB,CACzB,yBACF,CAEA,WACE,iBAAkB,CAElB,OAAQ,CACR,SAEF,CAEA,aACE,8BAAgC,CAChC,kCACF,CAEA,mBACE,8BAAgC,CAChC,kCACF,CAEA,qBACE,8BAAgC,CAChC,uBACF,CAEA,2BACE,8BAAgC,CAChC,oBAAuB,CACvB,kCACF,CAEA,YACE,qCACF,CAEA,kBACE,qCACF,CCzMA,KACE,QAAS,CACT,mJAEY,CACZ,kCAAmC,CACnC,iCACF,CAEA,KACE,yEAEF,CAEA,KACE,iBAAkB,CAClB,eACF",
     "names": [],
     "sources": [
         "webpack://src/views/App.css",
         "webpack://src/index.css"
     ],
     "sourcesContent": [
-        "/* file upload widget */\n\n.filepond--credits {\n  display: none;\n}\n\n/* Loading Bullet in BlockUI */\n\n.loading-bullet {\n  color: #0099cc !important;\n}\n\n/* widgets */\ntextarea:focus,\ninput[type=\"text\"]:focus,\ninput[type=\"password\"]:focus,\ninput[type=\"datetime\"]:focus,\ninput[type=\"datetime-local\"]:focus,\ninput[type=\"date\"]:focus,\ninput[type=\"month\"]:focus,\ninput[type=\"time\"]:focus,\ninput[type=\"week\"]:focus,\ninput[type=\"number\"]:focus,\ninput[type=\"email\"]:focus,\ninput[type=\"url\"]:focus,\ninput[type=\"search\"]:focus,\ninput[type=\"tel\"]:focus,\ninput[type=\"color\"]:focus,\ninput[type=\"checkbox\"]:focus,\n.uneditable-input:focus {\n  box-shadow: none;\n  border: 2px solid #2684ff;\n}\n\ndiv[role=\"slider\"]:focus,\n.uneditable-input:focus {\n  /* box-shadow: none; */\n  border: 2px solid #2684ff !important;\n}\n\n.form-check-input:checked {\n  background-color: #2684ff !important;\n}\n\n.thumbnailIframe {\n  -ms-zoom: 0.5;\n  zoom: 0.5;\n  -moz-transform: scale(0.5);\n  -moz-transform-origin: 0 0;\n  -o-transform: scale(0.5);\n  -o-transform-origin: 0 0;\n  -webkit-transform: scale(0.5);\n  -webkit-transform-origin: 0 0;\n  transform: scale(0.5);\n  transform-origin: 0 0;\n}\n\n/*\n * Sidebar\n */\n\n.sidebar {\n  position: fixed;\n  top: 0;\n  bottom: 0;\n  left: 0;\n  z-index: 100; /* Behind the navbar */\n  padding: 48px 0 0; /* Height of navbar */\n  box-shadow: inset -1px 0 0 rgba(0, 0, 0, 0.1);\n  border-left: 1px solid #eeeeee;\n}\n\n/* @media (max-width: 767.98px) {\n  .sidebar {\n    top: 0rem;\n  }\n} */\n\n.sidebar-sticky {\n  position: relative;\n  top: 0;\n  height: calc(100vh - 48px);\n  padding-top: 0.5rem;\n  overflow-x: hidden;\n  overflow-y: auto; /* Scrollable contents if viewport is shorter than content. */\n}\n\n.sidebar .nav-link {\n  font-weight: 500;\n  color: #333;\n}\n\n.sidebar .nav-link .feather {\n  margin-right: 4px;\n  color: #727272;\n}\n\n.sidebar .nav-link.active {\n  color: #2470dc;\n}\n\n.sidebar .nav-link:hover .feather,\n.sidebar .nav-link.active .feather {\n  color: inherit;\n}\n\n.sidebar-heading {\n  font-size: 0.75rem;\n  text-transform: uppercase;\n}\n\n/*\n * Navbar\n */\n\n.navbar-brand {\n  padding-top: 0.75rem;\n  padding-bottom: 0.75rem;\n  font-size: 1rem;\n  background-color: rgba(0, 0, 0, 0.25);\n  box-shadow: inset -1px 0 0 rgba(0, 0, 0, 0.25);\n}\n\n.navbar .navbar-toggler {\n  top: 0.25rem;\n  right: 1rem;\n}\n\n/*\n  Login\n*/\n\n.div-signin {\n  padding-top: 60px;\n  padding-bottom: 40px;\n  /* background-color: #f5f5f5; */\n}\n\n.form-signin {\n  width: 100%;\n  max-width: 330px;\n  padding: 15px;\n  margin: 0 auto;\n}\n\n.form-signin .form-control {\n  position: relative;\n  box-sizing: border-box;\n  height: auto;\n  padding: 10px;\n  font-size: 16px;\n}\n.form-signin .form-control:focus {\n  z-index: 2;\n}\n.form-signin input[type=\"email\"] {\n  margin-bottom: -1px;\n  border-bottom-right-radius: 0;\n  border-bottom-left-radius: 0;\n}\n.form-signin input[type=\"password\"] {\n  margin-bottom: 10px;\n  border-top-left-radius: 0;\n  border-top-right-radius: 0;\n}\n\n.poweredby {\n  position: absolute;\n  /* bottom: 10px; */\n  top: 5px;\n  right: 5px;\n  /* border: 1px solid #e5e5e5; */\n}\n\n.btn-primary {\n  border-color: #2684ff !important;\n  background-color: #2684ff !important;\n}\n\n.btn-primary:hover {\n  border-color: #217BF1 !important;\n  background-color: #217BF1 !important;\n}\n\n.title-card {\n  background-color: rgba(38,132,255,0.04);\n}\n\n.title-card:hover {\n  background-color: rgba(38,132,255,0.08);\n}\n",
+        "/* file upload widget */\n\n.filepond--credits {\n  display: none;\n}\n\n/* Loading Bullet in BlockUI */\n\n.loading-bullet {\n  color: #0099cc !important;\n}\n\n/* widgets */\ntextarea:focus,\ninput[type=\"text\"]:focus,\ninput[type=\"password\"]:focus,\ninput[type=\"datetime\"]:focus,\ninput[type=\"datetime-local\"]:focus,\ninput[type=\"date\"]:focus,\ninput[type=\"month\"]:focus,\ninput[type=\"time\"]:focus,\ninput[type=\"week\"]:focus,\ninput[type=\"number\"]:focus,\ninput[type=\"email\"]:focus,\ninput[type=\"url\"]:focus,\ninput[type=\"search\"]:focus,\ninput[type=\"tel\"]:focus,\ninput[type=\"color\"]:focus,\ninput[type=\"checkbox\"]:focus,\n.uneditable-input:focus {\n  box-shadow: none;\n  border: 2px solid #2684ff;\n}\n\ndiv[role=\"slider\"]:focus,\n.uneditable-input:focus {\n  /* box-shadow: none; */\n  border: 2px solid #2684ff !important;\n}\n\n.form-check-input:checked {\n  background-color: #2684ff !important;\n}\n\n.thumbnailIframe {\n  -ms-zoom: 0.5;\n  zoom: 0.5;\n  -moz-transform: scale(0.5);\n  -moz-transform-origin: 0 0;\n  -o-transform: scale(0.5);\n  -o-transform-origin: 0 0;\n  -webkit-transform: scale(0.5);\n  -webkit-transform-origin: 0 0;\n  transform: scale(0.5);\n  transform-origin: 0 0;\n}\n\n/*\n * Sidebar\n */\n\n.sidebar {\n  position: fixed;\n  top: 0;\n  bottom: 0;\n  left: 0;\n  z-index: 100; /* Behind the navbar */\n  padding: 48px 0 0; /* Height of navbar */\n  box-shadow: inset -1px 0 0 rgba(0, 0, 0, 0.1);\n  border-left: 1px solid #eeeeee;\n}\n\n/* @media (max-width: 767.98px) {\n  .sidebar {\n    top: 0rem;\n  }\n} */\n\n.sidebar-sticky {\n  position: relative;\n  top: 0;\n  height: calc(100vh - 48px);\n  padding-top: 0.5rem;\n  overflow-x: hidden;\n  overflow-y: auto; /* Scrollable contents if viewport is shorter than content. */\n}\n\n.sidebar .nav-link {\n  font-weight: 500;\n  color: #333;\n}\n\n.sidebar .nav-link .feather {\n  margin-right: 4px;\n  color: #727272;\n}\n\n.sidebar .nav-link.active {\n  color: #2470dc;\n}\n\n.sidebar .nav-link:hover .feather,\n.sidebar .nav-link.active .feather {\n  color: inherit;\n}\n\n.sidebar-heading {\n  font-size: 0.75rem;\n  text-transform: uppercase;\n}\n\n/*\n * Navbar\n */\n\n.navbar-brand {\n  padding-top: 0.75rem;\n  padding-bottom: 0.75rem;\n  font-size: 1rem;\n  background-color: rgba(0, 0, 0, 0.25);\n  box-shadow: inset -1px 0 0 rgba(0, 0, 0, 0.25);\n}\n\n.navbar .navbar-toggler {\n  top: 0.25rem;\n  right: 1rem;\n}\n\n/*\n  Login\n*/\n\n.div-signin {\n  padding-top: 60px;\n  padding-bottom: 40px;\n  /* background-color: #f5f5f5; */\n}\n\n.form-signin {\n  width: 100%;\n  max-width: 330px;\n  padding: 15px;\n  margin: 0 auto;\n}\n\n.form-signin .form-control {\n  position: relative;\n  box-sizing: border-box;\n  height: auto;\n  padding: 10px;\n  font-size: 16px;\n}\n.form-signin .form-control:focus {\n  z-index: 2;\n}\n.form-signin input[type=\"email\"] {\n  margin-bottom: -1px;\n  border-bottom-right-radius: 0;\n  border-bottom-left-radius: 0;\n}\n.form-signin input[type=\"password\"] {\n  margin-bottom: 10px;\n  border-top-left-radius: 0;\n  border-top-right-radius: 0;\n}\n\n.poweredby {\n  position: absolute;\n  /* bottom: 10px; */\n  top: 5px;\n  right: 5px;\n  /* border: 1px solid #e5e5e5; */\n}\n\n.btn-primary {\n  border-color: #2684ff !important;\n  background-color: #2684ff !important;\n}\n\n.btn-primary:hover {\n  border-color: #217bf1 !important;\n  background-color: #217bf1 !important;\n}\n\n.btn-outline-primary {\n  border-color: #2684ff !important;\n  color: #2684ff !important;\n}\n\n.btn-outline-primary:hover {\n  border-color: #2684ff !important;\n  color: white !important;\n  background-color: #2684ff !important;\n}\n\n.title-card {\n  background-color: rgba(38, 132, 255, 0.04);\n}\n\n.title-card:hover {\n  background-color: rgba(38, 132, 255, 0.08);\n}\n",
         "body {\n  margin: 0; \n  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Roboto', 'Oxygen',\n    'Ubuntu', 'Cantarell', 'Fira Sans', 'Droid Sans', 'Helvetica Neue',\n    sans-serif;\n  -webkit-font-smoothing: antialiased;\n  -moz-osx-font-smoothing: grayscale;\n}\n\ncode {\n  font-family: source-code-pro, Menlo, Monaco, Consolas, 'Courier New',\n    monospace;\n}\n\nhtml {\n  position: relative;\n  min-height: 100%;\n}\n\n"
     ],
     "version": 3
 }
```

### Comparing `mercury-2.2.9/mercury/frontend-dist/static/js/2.6305b467.chunk.js` & `mercury-2.3.0/mercury/frontend-dist/static/js/2.206848a5.chunk.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 2.6305b467.chunk.js.LICENSE.txt */
+/*! For license information please see 2.206848a5.chunk.js.LICENSE.txt */
 (this.webpackJsonpfrontend = this.webpackJsonpfrontend || []).push([
     [2],
     [function(e, t, n) {
         "use strict";
         e.exports = n(194)
     }, function(e, t, n) {
         "use strict";
@@ -447,15 +447,15 @@
                     }
             }), [s, u]);
             var f = n || o;
             return i.a.createElement(f.Provider, {
                 value: s
             }, a)
         };
-        n(10), n(40), n(55), n(126);
+        n(10), n(40), n(55), n(125);
 
         function d() {
             return Object(r.useContext)(o)
         }
 
         function p(e) {
             void 0 === e && (e = o);
@@ -3759,14 +3759,842 @@
         })(m || (m = {})),
         function(e) {
             e.UseFetchers = "useFetchers", e.UseScrollRestoration = "useScrollRestoration"
         }(g || (g = {}))
     }, function(e, t, n) {
         "use strict";
         n.d(t, "a", (function() {
+            return L
+        })), n.d(t, "b", (function() {
+            return K
+        }));
+        var r = n(1),
+            i = n.n(r);
+
+        function o(e) {
+            var t, n, r = "";
+            if ("string" === typeof e || "number" === typeof e) r += e;
+            else if ("object" === typeof e)
+                if (Array.isArray(e))
+                    for (t = 0; t < e.length; t++) e[t] && (n = o(e[t])) && (r && (r += " "), r += n);
+                else
+                    for (t in e) e[t] && (r && (r += " "), r += t);
+            return r
+        }
+        var a = function() {
+                for (var e, t, n = 0, r = ""; n < arguments.length;)(e = arguments[n++]) && (t = o(e)) && (r && (r += " "), r += t);
+                return r
+            },
+            s = n(39);
+
+        function u() {
+            return (u = Object.assign || function(e) {
+                for (var t = 1; t < arguments.length; t++) {
+                    var n = arguments[t];
+                    for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
+                }
+                return e
+            }).apply(this, arguments)
+        }
+
+        function l(e, t) {
+            if (null == e) return {};
+            var n, r, i = {},
+                o = Object.keys(e);
+            for (r = 0; r < o.length; r++) n = o[r], t.indexOf(n) >= 0 || (i[n] = e[n]);
+            return i
+        }
+
+        function c(e) {
+            return "number" === typeof e && !isNaN(e)
+        }
+
+        function f(e) {
+            return "boolean" === typeof e
+        }
+
+        function d(e) {
+            return "string" === typeof e
+        }
+
+        function p(e) {
+            return "function" === typeof e
+        }
+
+        function h(e) {
+            return d(e) || p(e) ? e : null
+        }
+
+        function m(e) {
+            return 0 === e || e
+        }
+        var g = !("undefined" === typeof window || !window.document || !window.document.createElement);
+
+        function v(e) {
+            return Object(r.isValidElement)(e) || d(e) || p(e) || c(e)
+        }
+        var b = {
+                TOP_LEFT: "top-left",
+                TOP_RIGHT: "top-right",
+                TOP_CENTER: "top-center",
+                BOTTOM_LEFT: "bottom-left",
+                BOTTOM_RIGHT: "bottom-right",
+                BOTTOM_CENTER: "bottom-center"
+            },
+            E = {
+                INFO: "info",
+                SUCCESS: "success",
+                WARNING: "warning",
+                ERROR: "error",
+                DEFAULT: "default"
+            };
+
+        function y(e) {
+            var t = e.enter,
+                n = e.exit,
+                o = e.appendPosition,
+                a = void 0 !== o && o,
+                s = e.collapse,
+                u = void 0 === s || s,
+                l = e.collapseDuration,
+                c = void 0 === l ? 300 : l;
+            return function(e) {
+                var o = e.children,
+                    s = e.position,
+                    l = e.preventExitTransition,
+                    f = e.done,
+                    d = e.nodeRef,
+                    p = e.isIn,
+                    h = a ? t + "--" + s : t,
+                    m = a ? n + "--" + s : n,
+                    g = Object(r.useRef)(),
+                    v = Object(r.useRef)(0);
+
+                function b(e) {
+                    if (e.target === d.current) {
+                        var t = d.current;
+                        t.dispatchEvent(new Event("d")), t.removeEventListener("animationend", b), 0 === v.current && (t.className = g.current)
+                    }
+                }
+
+                function E() {
+                    var e = d.current;
+                    e.removeEventListener("animationend", E), u ? function(e, t, n) {
+                        void 0 === n && (n = 300);
+                        var r = e.scrollHeight,
+                            i = e.style;
+                        requestAnimationFrame((function() {
+                            i.minHeight = "initial", i.height = r + "px", i.transition = "all " + n + "ms", requestAnimationFrame((function() {
+                                i.height = "0", i.padding = "0", i.margin = "0", setTimeout(t, n)
+                            }))
+                        }))
+                    }(e, f, c) : f()
+                }
+                return Object(r.useLayoutEffect)((function() {
+                    ! function() {
+                        var e = d.current;
+                        g.current = e.className, e.className += " " + h, e.addEventListener("animationend", b)
+                    }()
+                }), []), Object(r.useEffect)((function() {
+                    p || (l ? E() : function() {
+                        v.current = 1;
+                        var e = d.current;
+                        e.className += " " + m, e.addEventListener("animationend", E)
+                    }())
+                }), [p]), i.a.createElement(i.a.Fragment, null, o)
+            }
+        }
+        var _ = {
+                list: new Map,
+                emitQueue: new Map,
+                on: function(e, t) {
+                    return this.list.has(e) || this.list.set(e, []), this.list.get(e).push(t), this
+                },
+                off: function(e, t) {
+                    if (t) {
+                        var n = this.list.get(e).filter((function(e) {
+                            return e !== t
+                        }));
+                        return this.list.set(e, n), this
+                    }
+                    return this.list.delete(e), this
+                },
+                cancelEmit: function(e) {
+                    var t = this.emitQueue.get(e);
+                    return t && (t.forEach(clearTimeout), this.emitQueue.delete(e)), this
+                },
+                emit: function(e) {
+                    for (var t = this, n = arguments.length, r = new Array(n > 1 ? n - 1 : 0), i = 1; i < n; i++) r[i - 1] = arguments[i];
+                    this.list.has(e) && this.list.get(e).forEach((function(n) {
+                        var i = setTimeout((function() {
+                            n.apply(void 0, r)
+                        }), 0);
+                        t.emitQueue.has(e) || t.emitQueue.set(e, []), t.emitQueue.get(e).push(i)
+                    }))
+                }
+            },
+            T = ["delay", "staleId"];
+
+        function w(e) {
+            var t = Object(r.useReducer)((function(e) {
+                    return e + 1
+                }), 0)[1],
+                n = Object(r.useState)([]),
+                i = n[0],
+                o = n[1],
+                a = Object(r.useRef)(null),
+                s = Object(r.useRef)(new Map).current,
+                u = function(e) {
+                    return -1 !== i.indexOf(e)
+                },
+                g = Object(r.useRef)({
+                    toastKey: 1,
+                    displayedToast: 0,
+                    count: 0,
+                    queue: [],
+                    props: e,
+                    containerId: null,
+                    isToastActive: u,
+                    getToast: function(e) {
+                        return s.get(e)
+                    }
+                }).current;
+
+            function b(e) {
+                var t = e.containerId;
+                !g.props.limit || t && g.containerId !== t || (g.count -= g.queue.length, g.queue = [])
+            }
+
+            function E(e) {
+                o((function(t) {
+                    return m(e) ? t.filter((function(t) {
+                        return t !== e
+                    })) : []
+                }))
+            }
+
+            function y() {
+                var e = g.queue.shift();
+                O(e.toastContent, e.toastProps, e.staleId)
+            }
+
+            function w(e, n) {
+                var i = n.delay,
+                    o = n.staleId,
+                    u = l(n, T);
+                if (v(e) && ! function(e) {
+                        return !a.current || g.props.enableMultiContainer && e.containerId !== g.props.containerId || s.has(e.toastId) && null == e.updateId
+                    }(u)) {
+                    var b = u.toastId,
+                        _ = u.updateId,
+                        w = u.data,
+                        A = g.props,
+                        k = function() {
+                            return E(b)
+                        },
+                        D = null == _;
+                    D && g.count++;
+                    var C, S, I = {
+                        toastId: b,
+                        updateId: _,
+                        isLoading: u.isLoading,
+                        theme: u.theme || A.theme,
+                        icon: null != u.icon ? u.icon : A.icon,
+                        isIn: !1,
+                        key: u.key || g.toastKey++,
+                        type: u.type,
+                        closeToast: k,
+                        closeButton: u.closeButton,
+                        rtl: A.rtl,
+                        position: u.position || A.position,
+                        transition: u.transition || A.transition,
+                        className: h(u.className || A.toastClassName),
+                        bodyClassName: h(u.bodyClassName || A.bodyClassName),
+                        style: u.style || A.toastStyle,
+                        bodyStyle: u.bodyStyle || A.bodyStyle,
+                        onClick: u.onClick || A.onClick,
+                        pauseOnHover: f(u.pauseOnHover) ? u.pauseOnHover : A.pauseOnHover,
+                        pauseOnFocusLoss: f(u.pauseOnFocusLoss) ? u.pauseOnFocusLoss : A.pauseOnFocusLoss,
+                        draggable: f(u.draggable) ? u.draggable : A.draggable,
+                        draggablePercent: u.draggablePercent || A.draggablePercent,
+                        draggableDirection: u.draggableDirection || A.draggableDirection,
+                        closeOnClick: f(u.closeOnClick) ? u.closeOnClick : A.closeOnClick,
+                        progressClassName: h(u.progressClassName || A.progressClassName),
+                        progressStyle: u.progressStyle || A.progressStyle,
+                        autoClose: !u.isLoading && (C = u.autoClose, S = A.autoClose, !1 === C || c(C) && C > 0 ? C : S),
+                        hideProgressBar: f(u.hideProgressBar) ? u.hideProgressBar : A.hideProgressBar,
+                        progress: u.progress,
+                        role: u.role || A.role,
+                        deleteToast: function() {
+                            s.delete(b);
+                            var e = g.queue.length;
+                            if (g.count = m(b) ? g.count - 1 : g.count - g.displayedToast, g.count < 0 && (g.count = 0), e > 0) {
+                                var n = m(b) ? 1 : g.props.limit;
+                                if (1 === e || 1 === n) g.displayedToast++, y();
+                                else {
+                                    var r = n > e ? e : n;
+                                    g.displayedToast = r;
+                                    for (var i = 0; i < r; i++) y()
+                                }
+                            } else t()
+                        }
+                    };
+                    p(u.onOpen) && (I.onOpen = u.onOpen), p(u.onClose) && (I.onClose = u.onClose), I.closeButton = A.closeButton, !1 === u.closeButton || v(u.closeButton) ? I.closeButton = u.closeButton : !0 === u.closeButton && (I.closeButton = !v(A.closeButton) || A.closeButton);
+                    var N = e;
+                    Object(r.isValidElement)(e) && !d(e.type) ? N = Object(r.cloneElement)(e, {
+                        closeToast: k,
+                        toastProps: I,
+                        data: w
+                    }) : p(e) && (N = e({
+                        closeToast: k,
+                        toastProps: I,
+                        data: w
+                    })), A.limit && A.limit > 0 && g.count > A.limit && D ? g.queue.push({
+                        toastContent: N,
+                        toastProps: I,
+                        staleId: o
+                    }) : c(i) && i > 0 ? setTimeout((function() {
+                        O(N, I, o)
+                    }), i) : O(N, I, o)
+                }
+            }
+
+            function O(e, t, n) {
+                var r = t.toastId;
+                n && s.delete(n), s.set(r, {
+                    content: e,
+                    props: t
+                }), o((function(e) {
+                    return [].concat(e, [r]).filter((function(e) {
+                        return e !== n
+                    }))
+                }))
+            }
+            return Object(r.useEffect)((function() {
+                return g.containerId = e.containerId, _.cancelEmit(3).on(0, w).on(1, (function(e) {
+                        return a.current && E(e)
+                    })).on(5, b).emit(2, g),
+                    function() {
+                        return _.emit(3, g)
+                    }
+            }), []), Object(r.useEffect)((function() {
+                g.isToastActive = u, g.displayedToast = i.length, _.emit(4, i.length, e.containerId)
+            }), [i]), Object(r.useEffect)((function() {
+                g.props = e
+            })), {
+                getToastToRender: function(t) {
+                    var n = new Map,
+                        r = Array.from(s.values());
+                    return e.newestOnTop && r.reverse(), r.forEach((function(e) {
+                        var t = e.props.position;
+                        n.has(t) || n.set(t, []), n.get(t).push(e)
+                    })), Array.from(n, (function(e) {
+                        return t(e[0], e[1])
+                    }))
+                },
+                containerRef: a,
+                isToastActive: u
+            }
+        }
+
+        function O(e) {
+            return e.targetTouches && e.targetTouches.length >= 1 ? e.targetTouches[0].clientX : e.clientX
+        }
+
+        function A(e) {
+            return e.targetTouches && e.targetTouches.length >= 1 ? e.targetTouches[0].clientY : e.clientY
+        }
+
+        function k(e) {
+            var t = Object(r.useState)(!1),
+                n = t[0],
+                i = t[1],
+                o = Object(r.useState)(!1),
+                a = o[0],
+                s = o[1],
+                u = Object(r.useRef)(null),
+                l = Object(r.useRef)({
+                    start: 0,
+                    x: 0,
+                    y: 0,
+                    delta: 0,
+                    removalDistance: 0,
+                    canCloseOnClick: !0,
+                    canDrag: !1,
+                    boundingRect: null,
+                    didMove: !1
+                }).current,
+                c = Object(r.useRef)(e),
+                f = e.autoClose,
+                d = e.pauseOnHover,
+                h = e.closeToast,
+                m = e.onClick,
+                g = e.closeOnClick;
+
+            function v(t) {
+                if (e.draggable) {
+                    l.didMove = !1, document.addEventListener("mousemove", _), document.addEventListener("mouseup", T), document.addEventListener("touchmove", _), document.addEventListener("touchend", T);
+                    var n = u.current;
+                    l.canCloseOnClick = !0, l.canDrag = !0, l.boundingRect = n.getBoundingClientRect(), n.style.transition = "", l.x = O(t.nativeEvent), l.y = A(t.nativeEvent), "x" === e.draggableDirection ? (l.start = l.x, l.removalDistance = n.offsetWidth * (e.draggablePercent / 100)) : (l.start = l.y, l.removalDistance = n.offsetHeight * (80 === e.draggablePercent ? 1.5 * e.draggablePercent : e.draggablePercent / 100))
+                }
+            }
+
+            function b() {
+                if (l.boundingRect) {
+                    var t = l.boundingRect,
+                        n = t.top,
+                        r = t.bottom,
+                        i = t.left,
+                        o = t.right;
+                    e.pauseOnHover && l.x >= i && l.x <= o && l.y >= n && l.y <= r ? y() : E()
+                }
+            }
+
+            function E() {
+                i(!0)
+            }
+
+            function y() {
+                i(!1)
+            }
+
+            function _(t) {
+                var r = u.current;
+                l.canDrag && r && (l.didMove = !0, n && y(), l.x = O(t), l.y = A(t), "x" === e.draggableDirection ? l.delta = l.x - l.start : l.delta = l.y - l.start, l.start !== l.x && (l.canCloseOnClick = !1), r.style.transform = "translate" + e.draggableDirection + "(" + l.delta + "px)", r.style.opacity = "" + (1 - Math.abs(l.delta / l.removalDistance)))
+            }
+
+            function T() {
+                document.removeEventListener("mousemove", _), document.removeEventListener("mouseup", T), document.removeEventListener("touchmove", _), document.removeEventListener("touchend", T);
+                var t = u.current;
+                if (l.canDrag && l.didMove && t) {
+                    if (l.canDrag = !1, Math.abs(l.delta) > l.removalDistance) return s(!0), void e.closeToast();
+                    t.style.transition = "transform 0.2s, opacity 0.2s", t.style.transform = "translate" + e.draggableDirection + "(0)", t.style.opacity = "1"
+                }
+            }
+            Object(r.useEffect)((function() {
+                c.current = e
+            })), Object(r.useEffect)((function() {
+                return u.current && u.current.addEventListener("d", E, {
+                        once: !0
+                    }), p(e.onOpen) && e.onOpen(Object(r.isValidElement)(e.children) && e.children.props),
+                    function() {
+                        var e = c.current;
+                        p(e.onClose) && e.onClose(Object(r.isValidElement)(e.children) && e.children.props)
+                    }
+            }), []), Object(r.useEffect)((function() {
+                return e.pauseOnFocusLoss && function() {
+                        document.hasFocus() || y();
+                        window.addEventListener("focus", E), window.addEventListener("blur", y)
+                    }(),
+                    function() {
+                        e.pauseOnFocusLoss && (window.removeEventListener("focus", E), window.removeEventListener("blur", y))
+                    }
+            }), [e.pauseOnFocusLoss]);
+            var w = {
+                onMouseDown: v,
+                onTouchStart: v,
+                onMouseUp: b,
+                onTouchEnd: b
+            };
+            return f && d && (w.onMouseEnter = y, w.onMouseLeave = E), g && (w.onClick = function(e) {
+                m && m(e), l.canCloseOnClick && h()
+            }), {
+                playToast: E,
+                pauseToast: y,
+                isRunning: n,
+                preventExitTransition: a,
+                toastRef: u,
+                eventHandlers: w
+            }
+        }
+
+        function D(e) {
+            var t = e.closeToast,
+                n = e.theme,
+                i = e.ariaLabel,
+                o = void 0 === i ? "close" : i;
+            return Object(r.createElement)("button", {
+                className: "Toastify__close-button Toastify__close-button--" + n,
+                type: "button",
+                onClick: function(e) {
+                    e.stopPropagation(), t(e)
+                },
+                "aria-label": o
+            }, Object(r.createElement)("svg", {
+                "aria-hidden": "true",
+                viewBox: "0 0 14 16"
+            }, Object(r.createElement)("path", {
+                fillRule: "evenodd",
+                d: "M7.71 8.23l3.75 3.75-1.48 1.48-3.75-3.75-3.75 3.75L1 11.98l3.75-3.75L1 4.48 2.48 3l3.75 3.75L9.98 3l1.48 1.48-3.75 3.75z"
+            })))
+        }
+
+        function C(e) {
+            var t, n, i = e.delay,
+                o = e.isRunning,
+                s = e.closeToast,
+                l = e.type,
+                c = e.hide,
+                f = e.className,
+                d = e.style,
+                h = e.controlledProgress,
+                m = e.progress,
+                g = e.rtl,
+                v = e.isIn,
+                b = e.theme,
+                E = u({}, d, {
+                    animationDuration: i + "ms",
+                    animationPlayState: o ? "running" : "paused",
+                    opacity: c ? 0 : 1
+                });
+            h && (E.transform = "scaleX(" + m + ")");
+            var y = a("Toastify__progress-bar", h ? "Toastify__progress-bar--controlled" : "Toastify__progress-bar--animated", "Toastify__progress-bar-theme--" + b, "Toastify__progress-bar--" + l, ((t = {})["Toastify__progress-bar--rtl"] = g, t)),
+                _ = p(f) ? f({
+                    rtl: g,
+                    type: l,
+                    defaultClassName: y
+                }) : a(y, f),
+                T = ((n = {})[h && m >= 1 ? "onTransitionEnd" : "onAnimationEnd"] = h && m < 1 ? null : function() {
+                    v && s()
+                }, n);
+            return Object(r.createElement)("div", Object.assign({
+                role: "progressbar",
+                "aria-hidden": c ? "true" : "false",
+                "aria-label": "notification timer",
+                className: _,
+                style: E
+            }, T))
+        }
+        C.defaultProps = {
+            type: E.DEFAULT,
+            hide: !1
+        };
+        var S = ["theme", "type"],
+            I = function(e) {
+                var t = e.theme,
+                    n = e.type,
+                    i = l(e, S);
+                return Object(r.createElement)("svg", Object.assign({
+                    viewBox: "0 0 24 24",
+                    width: "100%",
+                    height: "100%",
+                    fill: "colored" === t ? "currentColor" : "var(--toastify-icon-color-" + n + ")"
+                }, i))
+            };
+        var N = {
+                info: function(e) {
+                    return Object(r.createElement)(I, Object.assign({}, e), Object(r.createElement)("path", {
+                        d: "M12 0a12 12 0 1012 12A12.013 12.013 0 0012 0zm.25 5a1.5 1.5 0 11-1.5 1.5 1.5 1.5 0 011.5-1.5zm2.25 13.5h-4a1 1 0 010-2h.75a.25.25 0 00.25-.25v-4.5a.25.25 0 00-.25-.25h-.75a1 1 0 010-2h1a2 2 0 012 2v4.75a.25.25 0 00.25.25h.75a1 1 0 110 2z"
+                    }))
+                },
+                warning: function(e) {
+                    return Object(r.createElement)(I, Object.assign({}, e), Object(r.createElement)("path", {
+                        d: "M23.32 17.191L15.438 2.184C14.728.833 13.416 0 11.996 0c-1.42 0-2.733.833-3.443 2.184L.533 17.448a4.744 4.744 0 000 4.368C1.243 23.167 2.555 24 3.975 24h16.05C22.22 24 24 22.044 24 19.632c0-.904-.251-1.746-.68-2.44zm-9.622 1.46c0 1.033-.724 1.823-1.698 1.823s-1.698-.79-1.698-1.822v-.043c0-1.028.724-1.822 1.698-1.822s1.698.79 1.698 1.822v.043zm.039-12.285l-.84 8.06c-.057.581-.408.943-.897.943-.49 0-.84-.367-.896-.942l-.84-8.065c-.057-.624.25-1.095.779-1.095h1.91c.528.005.84.476.784 1.1z"
+                    }))
+                },
+                success: function(e) {
+                    return Object(r.createElement)(I, Object.assign({}, e), Object(r.createElement)("path", {
+                        d: "M12 0a12 12 0 1012 12A12.014 12.014 0 0012 0zm6.927 8.2l-6.845 9.289a1.011 1.011 0 01-1.43.188l-4.888-3.908a1 1 0 111.25-1.562l4.076 3.261 6.227-8.451a1 1 0 111.61 1.183z"
+                    }))
+                },
+                error: function(e) {
+                    return Object(r.createElement)(I, Object.assign({}, e), Object(r.createElement)("path", {
+                        d: "M11.983 0a12.206 12.206 0 00-8.51 3.653A11.8 11.8 0 000 12.207 11.779 11.779 0 0011.8 24h.214A12.111 12.111 0 0024 11.791 11.766 11.766 0 0011.983 0zM10.5 16.542a1.476 1.476 0 011.449-1.53h.027a1.527 1.527 0 011.523 1.47 1.475 1.475 0 01-1.449 1.53h-.027a1.529 1.529 0 01-1.523-1.47zM11 12.5v-6a1 1 0 012 0v6a1 1 0 11-2 0z"
+                    }))
+                },
+                spinner: function() {
+                    return Object(r.createElement)("div", {
+                        className: "Toastify__spinner"
+                    })
+                }
+            },
+            x = function(e) {
+                var t, n, i = k(e),
+                    o = i.isRunning,
+                    s = i.preventExitTransition,
+                    u = i.toastRef,
+                    l = i.eventHandlers,
+                    c = e.closeButton,
+                    f = e.children,
+                    h = e.autoClose,
+                    m = e.onClick,
+                    g = e.type,
+                    v = e.hideProgressBar,
+                    b = e.closeToast,
+                    E = e.transition,
+                    y = e.position,
+                    _ = e.className,
+                    T = e.style,
+                    w = e.bodyClassName,
+                    O = e.bodyStyle,
+                    A = e.progressClassName,
+                    D = e.progressStyle,
+                    S = e.updateId,
+                    I = e.role,
+                    x = e.progress,
+                    R = e.rtl,
+                    L = e.toastId,
+                    M = e.deleteToast,
+                    P = e.isIn,
+                    F = e.isLoading,
+                    B = e.icon,
+                    j = e.theme,
+                    U = a("Toastify__toast", "Toastify__toast-theme--" + j, "Toastify__toast--" + g, ((t = {})["Toastify__toast--rtl"] = R, t)),
+                    H = p(_) ? _({
+                        rtl: R,
+                        position: y,
+                        type: g,
+                        defaultClassName: U
+                    }) : a(U, _),
+                    G = !!x,
+                    z = N[g],
+                    q = {
+                        theme: j,
+                        type: g
+                    },
+                    V = z && z(q);
+                return !1 === B ? V = void 0 : p(B) ? V = B(q) : Object(r.isValidElement)(B) ? V = Object(r.cloneElement)(B, q) : d(B) ? V = B : F && (V = N.spinner()), Object(r.createElement)(E, {
+                    isIn: P,
+                    done: M,
+                    position: y,
+                    preventExitTransition: s,
+                    nodeRef: u
+                }, Object(r.createElement)("div", Object.assign({
+                    id: L,
+                    onClick: m,
+                    className: H
+                }, l, {
+                    style: T,
+                    ref: u
+                }), Object(r.createElement)("div", Object.assign({}, P && {
+                    role: I
+                }, {
+                    className: p(w) ? w({
+                        type: g
+                    }) : a("Toastify__toast-body", w),
+                    style: O
+                }), V && Object(r.createElement)("div", {
+                    className: a("Toastify__toast-icon", (n = {}, n["Toastify--animate-icon Toastify__zoom-enter"] = !F, n))
+                }, V), Object(r.createElement)("div", null, f)), function(e) {
+                    if (e) {
+                        var t = {
+                            closeToast: b,
+                            type: g,
+                            theme: j
+                        };
+                        return p(e) ? e(t) : Object(r.isValidElement)(e) ? Object(r.cloneElement)(e, t) : void 0
+                    }
+                }(c), (h || G) && Object(r.createElement)(C, Object.assign({}, S && !G ? {
+                    key: "pb-" + S
+                } : {}, {
+                    rtl: R,
+                    theme: j,
+                    delay: h,
+                    isRunning: o,
+                    isIn: P,
+                    closeToast: b,
+                    hide: v,
+                    type: g,
+                    style: D,
+                    className: A,
+                    controlledProgress: G,
+                    progress: x
+                }))))
+            },
+            R = y({
+                enter: "Toastify--animate Toastify__bounce-enter",
+                exit: "Toastify--animate Toastify__bounce-exit",
+                appendPosition: !0
+            }),
+            L = function(e) {
+                var t = w(e),
+                    n = t.getToastToRender,
+                    i = t.containerRef,
+                    o = t.isToastActive,
+                    s = e.className,
+                    l = e.style,
+                    c = e.rtl,
+                    f = e.containerId;
+
+                function d(e) {
+                    var t, n = a("Toastify__toast-container", "Toastify__toast-container--" + e, ((t = {})["Toastify__toast-container--rtl"] = c, t));
+                    return p(s) ? s({
+                        position: e,
+                        rtl: c,
+                        defaultClassName: n
+                    }) : a(n, h(s))
+                }
+                return Object(r.createElement)("div", {
+                    ref: i,
+                    className: "Toastify",
+                    id: f
+                }, n((function(e, t) {
+                    var n = t.length ? u({}, l) : u({}, l, {
+                        pointerEvents: "none"
+                    });
+                    return Object(r.createElement)("div", {
+                        className: d(e),
+                        style: n,
+                        key: "container-" + e
+                    }, t.map((function(e) {
+                        var t = e.content,
+                            n = e.props;
+                        return Object(r.createElement)(x, Object.assign({}, n, {
+                            isIn: o(n.toastId),
+                            key: "toast-" + n.key,
+                            closeButton: !0 === n.closeButton ? D : n.closeButton
+                        }), t)
+                    })))
+                })))
+            };
+        L.defaultProps = {
+            position: b.TOP_RIGHT,
+            transition: R,
+            rtl: !1,
+            autoClose: 5e3,
+            hideProgressBar: !1,
+            closeButton: D,
+            pauseOnHover: !0,
+            pauseOnFocusLoss: !0,
+            closeOnClick: !0,
+            newestOnTop: !1,
+            draggable: !0,
+            draggablePercent: 80,
+            draggableDirection: "x",
+            role: "alert",
+            theme: "light"
+        };
+        var M, P, F, B = new Map,
+            j = [],
+            U = !1;
+
+        function H() {
+            return Math.random().toString(36).substring(2, 9)
+        }
+
+        function G(e) {
+            return e && (d(e.toastId) || c(e.toastId)) ? e.toastId : H()
+        }
+
+        function z(e, t) {
+            return B.size > 0 ? _.emit(0, e, t) : (j.push({
+                content: e,
+                options: t
+            }), U && g && (U = !1, P = document.createElement("div"), document.body.appendChild(P), Object(s.render)(Object(r.createElement)(L, Object.assign({}, F)), P))), t.toastId
+        }
+
+        function q(e, t) {
+            return u({}, t, {
+                type: t && t.type || e,
+                toastId: G(t)
+            })
+        }
+
+        function V(e) {
+            return function(t, n) {
+                return z(t, q(e, n))
+            }
+        }
+
+        function K(e, t) {
+            return z(e, q(E.DEFAULT, t))
+        }
+        K.loading = function(e, t) {
+            return z(e, q(E.DEFAULT, u({
+                isLoading: !0,
+                autoClose: !1,
+                closeOnClick: !1,
+                closeButton: !1,
+                draggable: !1
+            }, t)))
+        }, K.promise = function(e, t, n) {
+            var r, i = t.pending,
+                o = t.error,
+                a = t.success;
+            i && (r = d(i) ? K.loading(i, n) : K.loading(i.render, u({}, n, i)));
+            var s = {
+                    isLoading: null,
+                    autoClose: null,
+                    closeOnClick: null,
+                    closeButton: null,
+                    draggable: null
+                },
+                l = function(e, t, i) {
+                    if (null != t) {
+                        var o = u({
+                                type: e
+                            }, s, n, {
+                                data: i
+                            }),
+                            a = d(t) ? {
+                                render: t
+                            } : t;
+                        return r ? K.update(r, u({}, o, a)) : K(a.render, u({}, o, a)), i
+                    }
+                    K.dismiss(r)
+                },
+                c = p(e) ? e() : e;
+            return c.then((function(e) {
+                return l("success", a, e)
+            })).catch((function(e) {
+                return l("error", o, e)
+            })), c
+        }, K.success = V(E.SUCCESS), K.info = V(E.INFO), K.error = V(E.ERROR), K.warning = V(E.WARNING), K.warn = K.warning, K.dark = function(e, t) {
+            return z(e, q(E.DEFAULT, u({
+                theme: "dark"
+            }, t)))
+        }, K.dismiss = function(e) {
+            return _.emit(1, e)
+        }, K.clearWaitingQueue = function(e) {
+            return void 0 === e && (e = {}), _.emit(5, e)
+        }, K.isActive = function(e) {
+            var t = !1;
+            return B.forEach((function(n) {
+                n.isToastActive && n.isToastActive(e) && (t = !0)
+            })), t
+        }, K.update = function(e, t) {
+            void 0 === t && (t = {}), setTimeout((function() {
+                var n = function(e, t) {
+                    var n = t.containerId,
+                        r = B.get(n || M);
+                    return r ? r.getToast(e) : null
+                }(e, t);
+                if (n) {
+                    var r = n.props,
+                        i = n.content,
+                        o = u({}, r, t, {
+                            toastId: t.toastId || e,
+                            updateId: H()
+                        });
+                    o.toastId !== e && (o.staleId = e);
+                    var a = o.render || i;
+                    delete o.render, z(a, o)
+                }
+            }), 0)
+        }, K.done = function(e) {
+            K.update(e, {
+                progress: 1
+            })
+        }, K.onChange = function(e) {
+            return p(e) && _.on(4, e),
+                function() {
+                    p(e) && _.off(4, e)
+                }
+        }, K.configure = function(e) {
+            void 0 === e && (e = {}), U = !0, F = e
+        }, K.POSITION = b, K.TYPE = E, _.on(2, (function(e) {
+            M = e.containerId || e, B.set(M, e), j.forEach((function(e) {
+                _.emit(0, e.content, e.options)
+            })), j = []
+        })).on(3, (function(e) {
+            B.delete(e.containerId || e), 0 === B.size && _.off(0).off(1).off(5), g && P && document.body.removeChild(P)
+        }))
+    }, function(e, t, n) {
+        "use strict";
+        n.d(t, "a", (function() {
             return E
         })), n.d(t, "b", (function() {
             return y
         }));
         var r = n(19),
             i = function e(t, n, i) {
                 Object(r.a)(this, e), this.property = t, this.normal = n, i && (this.space = i)
@@ -4739,842 +5567,14 @@
                     zoomAndPan: null
                 }
             }),
             E = o([f, c, h, g, v], "html"),
             y = o([f, c, h, g, b], "svg")
     }, function(e, t, n) {
         "use strict";
-        n.d(t, "a", (function() {
-            return L
-        })), n.d(t, "b", (function() {
-            return K
-        }));
-        var r = n(1),
-            i = n.n(r);
-
-        function o(e) {
-            var t, n, r = "";
-            if ("string" === typeof e || "number" === typeof e) r += e;
-            else if ("object" === typeof e)
-                if (Array.isArray(e))
-                    for (t = 0; t < e.length; t++) e[t] && (n = o(e[t])) && (r && (r += " "), r += n);
-                else
-                    for (t in e) e[t] && (r && (r += " "), r += t);
-            return r
-        }
-        var a = function() {
-                for (var e, t, n = 0, r = ""; n < arguments.length;)(e = arguments[n++]) && (t = o(e)) && (r && (r += " "), r += t);
-                return r
-            },
-            s = n(39);
-
-        function u() {
-            return (u = Object.assign || function(e) {
-                for (var t = 1; t < arguments.length; t++) {
-                    var n = arguments[t];
-                    for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
-                }
-                return e
-            }).apply(this, arguments)
-        }
-
-        function l(e, t) {
-            if (null == e) return {};
-            var n, r, i = {},
-                o = Object.keys(e);
-            for (r = 0; r < o.length; r++) n = o[r], t.indexOf(n) >= 0 || (i[n] = e[n]);
-            return i
-        }
-
-        function c(e) {
-            return "number" === typeof e && !isNaN(e)
-        }
-
-        function f(e) {
-            return "boolean" === typeof e
-        }
-
-        function d(e) {
-            return "string" === typeof e
-        }
-
-        function p(e) {
-            return "function" === typeof e
-        }
-
-        function h(e) {
-            return d(e) || p(e) ? e : null
-        }
-
-        function m(e) {
-            return 0 === e || e
-        }
-        var g = !("undefined" === typeof window || !window.document || !window.document.createElement);
-
-        function v(e) {
-            return Object(r.isValidElement)(e) || d(e) || p(e) || c(e)
-        }
-        var b = {
-                TOP_LEFT: "top-left",
-                TOP_RIGHT: "top-right",
-                TOP_CENTER: "top-center",
-                BOTTOM_LEFT: "bottom-left",
-                BOTTOM_RIGHT: "bottom-right",
-                BOTTOM_CENTER: "bottom-center"
-            },
-            E = {
-                INFO: "info",
-                SUCCESS: "success",
-                WARNING: "warning",
-                ERROR: "error",
-                DEFAULT: "default"
-            };
-
-        function y(e) {
-            var t = e.enter,
-                n = e.exit,
-                o = e.appendPosition,
-                a = void 0 !== o && o,
-                s = e.collapse,
-                u = void 0 === s || s,
-                l = e.collapseDuration,
-                c = void 0 === l ? 300 : l;
-            return function(e) {
-                var o = e.children,
-                    s = e.position,
-                    l = e.preventExitTransition,
-                    f = e.done,
-                    d = e.nodeRef,
-                    p = e.isIn,
-                    h = a ? t + "--" + s : t,
-                    m = a ? n + "--" + s : n,
-                    g = Object(r.useRef)(),
-                    v = Object(r.useRef)(0);
-
-                function b(e) {
-                    if (e.target === d.current) {
-                        var t = d.current;
-                        t.dispatchEvent(new Event("d")), t.removeEventListener("animationend", b), 0 === v.current && (t.className = g.current)
-                    }
-                }
-
-                function E() {
-                    var e = d.current;
-                    e.removeEventListener("animationend", E), u ? function(e, t, n) {
-                        void 0 === n && (n = 300);
-                        var r = e.scrollHeight,
-                            i = e.style;
-                        requestAnimationFrame((function() {
-                            i.minHeight = "initial", i.height = r + "px", i.transition = "all " + n + "ms", requestAnimationFrame((function() {
-                                i.height = "0", i.padding = "0", i.margin = "0", setTimeout(t, n)
-                            }))
-                        }))
-                    }(e, f, c) : f()
-                }
-                return Object(r.useLayoutEffect)((function() {
-                    ! function() {
-                        var e = d.current;
-                        g.current = e.className, e.className += " " + h, e.addEventListener("animationend", b)
-                    }()
-                }), []), Object(r.useEffect)((function() {
-                    p || (l ? E() : function() {
-                        v.current = 1;
-                        var e = d.current;
-                        e.className += " " + m, e.addEventListener("animationend", E)
-                    }())
-                }), [p]), i.a.createElement(i.a.Fragment, null, o)
-            }
-        }
-        var _ = {
-                list: new Map,
-                emitQueue: new Map,
-                on: function(e, t) {
-                    return this.list.has(e) || this.list.set(e, []), this.list.get(e).push(t), this
-                },
-                off: function(e, t) {
-                    if (t) {
-                        var n = this.list.get(e).filter((function(e) {
-                            return e !== t
-                        }));
-                        return this.list.set(e, n), this
-                    }
-                    return this.list.delete(e), this
-                },
-                cancelEmit: function(e) {
-                    var t = this.emitQueue.get(e);
-                    return t && (t.forEach(clearTimeout), this.emitQueue.delete(e)), this
-                },
-                emit: function(e) {
-                    for (var t = this, n = arguments.length, r = new Array(n > 1 ? n - 1 : 0), i = 1; i < n; i++) r[i - 1] = arguments[i];
-                    this.list.has(e) && this.list.get(e).forEach((function(n) {
-                        var i = setTimeout((function() {
-                            n.apply(void 0, r)
-                        }), 0);
-                        t.emitQueue.has(e) || t.emitQueue.set(e, []), t.emitQueue.get(e).push(i)
-                    }))
-                }
-            },
-            T = ["delay", "staleId"];
-
-        function w(e) {
-            var t = Object(r.useReducer)((function(e) {
-                    return e + 1
-                }), 0)[1],
-                n = Object(r.useState)([]),
-                i = n[0],
-                o = n[1],
-                a = Object(r.useRef)(null),
-                s = Object(r.useRef)(new Map).current,
-                u = function(e) {
-                    return -1 !== i.indexOf(e)
-                },
-                g = Object(r.useRef)({
-                    toastKey: 1,
-                    displayedToast: 0,
-                    count: 0,
-                    queue: [],
-                    props: e,
-                    containerId: null,
-                    isToastActive: u,
-                    getToast: function(e) {
-                        return s.get(e)
-                    }
-                }).current;
-
-            function b(e) {
-                var t = e.containerId;
-                !g.props.limit || t && g.containerId !== t || (g.count -= g.queue.length, g.queue = [])
-            }
-
-            function E(e) {
-                o((function(t) {
-                    return m(e) ? t.filter((function(t) {
-                        return t !== e
-                    })) : []
-                }))
-            }
-
-            function y() {
-                var e = g.queue.shift();
-                O(e.toastContent, e.toastProps, e.staleId)
-            }
-
-            function w(e, n) {
-                var i = n.delay,
-                    o = n.staleId,
-                    u = l(n, T);
-                if (v(e) && ! function(e) {
-                        return !a.current || g.props.enableMultiContainer && e.containerId !== g.props.containerId || s.has(e.toastId) && null == e.updateId
-                    }(u)) {
-                    var b = u.toastId,
-                        _ = u.updateId,
-                        w = u.data,
-                        A = g.props,
-                        k = function() {
-                            return E(b)
-                        },
-                        D = null == _;
-                    D && g.count++;
-                    var C, S, I = {
-                        toastId: b,
-                        updateId: _,
-                        isLoading: u.isLoading,
-                        theme: u.theme || A.theme,
-                        icon: null != u.icon ? u.icon : A.icon,
-                        isIn: !1,
-                        key: u.key || g.toastKey++,
-                        type: u.type,
-                        closeToast: k,
-                        closeButton: u.closeButton,
-                        rtl: A.rtl,
-                        position: u.position || A.position,
-                        transition: u.transition || A.transition,
-                        className: h(u.className || A.toastClassName),
-                        bodyClassName: h(u.bodyClassName || A.bodyClassName),
-                        style: u.style || A.toastStyle,
-                        bodyStyle: u.bodyStyle || A.bodyStyle,
-                        onClick: u.onClick || A.onClick,
-                        pauseOnHover: f(u.pauseOnHover) ? u.pauseOnHover : A.pauseOnHover,
-                        pauseOnFocusLoss: f(u.pauseOnFocusLoss) ? u.pauseOnFocusLoss : A.pauseOnFocusLoss,
-                        draggable: f(u.draggable) ? u.draggable : A.draggable,
-                        draggablePercent: u.draggablePercent || A.draggablePercent,
-                        draggableDirection: u.draggableDirection || A.draggableDirection,
-                        closeOnClick: f(u.closeOnClick) ? u.closeOnClick : A.closeOnClick,
-                        progressClassName: h(u.progressClassName || A.progressClassName),
-                        progressStyle: u.progressStyle || A.progressStyle,
-                        autoClose: !u.isLoading && (C = u.autoClose, S = A.autoClose, !1 === C || c(C) && C > 0 ? C : S),
-                        hideProgressBar: f(u.hideProgressBar) ? u.hideProgressBar : A.hideProgressBar,
-                        progress: u.progress,
-                        role: u.role || A.role,
-                        deleteToast: function() {
-                            s.delete(b);
-                            var e = g.queue.length;
-                            if (g.count = m(b) ? g.count - 1 : g.count - g.displayedToast, g.count < 0 && (g.count = 0), e > 0) {
-                                var n = m(b) ? 1 : g.props.limit;
-                                if (1 === e || 1 === n) g.displayedToast++, y();
-                                else {
-                                    var r = n > e ? e : n;
-                                    g.displayedToast = r;
-                                    for (var i = 0; i < r; i++) y()
-                                }
-                            } else t()
-                        }
-                    };
-                    p(u.onOpen) && (I.onOpen = u.onOpen), p(u.onClose) && (I.onClose = u.onClose), I.closeButton = A.closeButton, !1 === u.closeButton || v(u.closeButton) ? I.closeButton = u.closeButton : !0 === u.closeButton && (I.closeButton = !v(A.closeButton) || A.closeButton);
-                    var N = e;
-                    Object(r.isValidElement)(e) && !d(e.type) ? N = Object(r.cloneElement)(e, {
-                        closeToast: k,
-                        toastProps: I,
-                        data: w
-                    }) : p(e) && (N = e({
-                        closeToast: k,
-                        toastProps: I,
-                        data: w
-                    })), A.limit && A.limit > 0 && g.count > A.limit && D ? g.queue.push({
-                        toastContent: N,
-                        toastProps: I,
-                        staleId: o
-                    }) : c(i) && i > 0 ? setTimeout((function() {
-                        O(N, I, o)
-                    }), i) : O(N, I, o)
-                }
-            }
-
-            function O(e, t, n) {
-                var r = t.toastId;
-                n && s.delete(n), s.set(r, {
-                    content: e,
-                    props: t
-                }), o((function(e) {
-                    return [].concat(e, [r]).filter((function(e) {
-                        return e !== n
-                    }))
-                }))
-            }
-            return Object(r.useEffect)((function() {
-                return g.containerId = e.containerId, _.cancelEmit(3).on(0, w).on(1, (function(e) {
-                        return a.current && E(e)
-                    })).on(5, b).emit(2, g),
-                    function() {
-                        return _.emit(3, g)
-                    }
-            }), []), Object(r.useEffect)((function() {
-                g.isToastActive = u, g.displayedToast = i.length, _.emit(4, i.length, e.containerId)
-            }), [i]), Object(r.useEffect)((function() {
-                g.props = e
-            })), {
-                getToastToRender: function(t) {
-                    var n = new Map,
-                        r = Array.from(s.values());
-                    return e.newestOnTop && r.reverse(), r.forEach((function(e) {
-                        var t = e.props.position;
-                        n.has(t) || n.set(t, []), n.get(t).push(e)
-                    })), Array.from(n, (function(e) {
-                        return t(e[0], e[1])
-                    }))
-                },
-                containerRef: a,
-                isToastActive: u
-            }
-        }
-
-        function O(e) {
-            return e.targetTouches && e.targetTouches.length >= 1 ? e.targetTouches[0].clientX : e.clientX
-        }
-
-        function A(e) {
-            return e.targetTouches && e.targetTouches.length >= 1 ? e.targetTouches[0].clientY : e.clientY
-        }
-
-        function k(e) {
-            var t = Object(r.useState)(!1),
-                n = t[0],
-                i = t[1],
-                o = Object(r.useState)(!1),
-                a = o[0],
-                s = o[1],
-                u = Object(r.useRef)(null),
-                l = Object(r.useRef)({
-                    start: 0,
-                    x: 0,
-                    y: 0,
-                    delta: 0,
-                    removalDistance: 0,
-                    canCloseOnClick: !0,
-                    canDrag: !1,
-                    boundingRect: null,
-                    didMove: !1
-                }).current,
-                c = Object(r.useRef)(e),
-                f = e.autoClose,
-                d = e.pauseOnHover,
-                h = e.closeToast,
-                m = e.onClick,
-                g = e.closeOnClick;
-
-            function v(t) {
-                if (e.draggable) {
-                    l.didMove = !1, document.addEventListener("mousemove", _), document.addEventListener("mouseup", T), document.addEventListener("touchmove", _), document.addEventListener("touchend", T);
-                    var n = u.current;
-                    l.canCloseOnClick = !0, l.canDrag = !0, l.boundingRect = n.getBoundingClientRect(), n.style.transition = "", l.x = O(t.nativeEvent), l.y = A(t.nativeEvent), "x" === e.draggableDirection ? (l.start = l.x, l.removalDistance = n.offsetWidth * (e.draggablePercent / 100)) : (l.start = l.y, l.removalDistance = n.offsetHeight * (80 === e.draggablePercent ? 1.5 * e.draggablePercent : e.draggablePercent / 100))
-                }
-            }
-
-            function b() {
-                if (l.boundingRect) {
-                    var t = l.boundingRect,
-                        n = t.top,
-                        r = t.bottom,
-                        i = t.left,
-                        o = t.right;
-                    e.pauseOnHover && l.x >= i && l.x <= o && l.y >= n && l.y <= r ? y() : E()
-                }
-            }
-
-            function E() {
-                i(!0)
-            }
-
-            function y() {
-                i(!1)
-            }
-
-            function _(t) {
-                var r = u.current;
-                l.canDrag && r && (l.didMove = !0, n && y(), l.x = O(t), l.y = A(t), "x" === e.draggableDirection ? l.delta = l.x - l.start : l.delta = l.y - l.start, l.start !== l.x && (l.canCloseOnClick = !1), r.style.transform = "translate" + e.draggableDirection + "(" + l.delta + "px)", r.style.opacity = "" + (1 - Math.abs(l.delta / l.removalDistance)))
-            }
-
-            function T() {
-                document.removeEventListener("mousemove", _), document.removeEventListener("mouseup", T), document.removeEventListener("touchmove", _), document.removeEventListener("touchend", T);
-                var t = u.current;
-                if (l.canDrag && l.didMove && t) {
-                    if (l.canDrag = !1, Math.abs(l.delta) > l.removalDistance) return s(!0), void e.closeToast();
-                    t.style.transition = "transform 0.2s, opacity 0.2s", t.style.transform = "translate" + e.draggableDirection + "(0)", t.style.opacity = "1"
-                }
-            }
-            Object(r.useEffect)((function() {
-                c.current = e
-            })), Object(r.useEffect)((function() {
-                return u.current && u.current.addEventListener("d", E, {
-                        once: !0
-                    }), p(e.onOpen) && e.onOpen(Object(r.isValidElement)(e.children) && e.children.props),
-                    function() {
-                        var e = c.current;
-                        p(e.onClose) && e.onClose(Object(r.isValidElement)(e.children) && e.children.props)
-                    }
-            }), []), Object(r.useEffect)((function() {
-                return e.pauseOnFocusLoss && function() {
-                        document.hasFocus() || y();
-                        window.addEventListener("focus", E), window.addEventListener("blur", y)
-                    }(),
-                    function() {
-                        e.pauseOnFocusLoss && (window.removeEventListener("focus", E), window.removeEventListener("blur", y))
-                    }
-            }), [e.pauseOnFocusLoss]);
-            var w = {
-                onMouseDown: v,
-                onTouchStart: v,
-                onMouseUp: b,
-                onTouchEnd: b
-            };
-            return f && d && (w.onMouseEnter = y, w.onMouseLeave = E), g && (w.onClick = function(e) {
-                m && m(e), l.canCloseOnClick && h()
-            }), {
-                playToast: E,
-                pauseToast: y,
-                isRunning: n,
-                preventExitTransition: a,
-                toastRef: u,
-                eventHandlers: w
-            }
-        }
-
-        function D(e) {
-            var t = e.closeToast,
-                n = e.theme,
-                i = e.ariaLabel,
-                o = void 0 === i ? "close" : i;
-            return Object(r.createElement)("button", {
-                className: "Toastify__close-button Toastify__close-button--" + n,
-                type: "button",
-                onClick: function(e) {
-                    e.stopPropagation(), t(e)
-                },
-                "aria-label": o
-            }, Object(r.createElement)("svg", {
-                "aria-hidden": "true",
-                viewBox: "0 0 14 16"
-            }, Object(r.createElement)("path", {
-                fillRule: "evenodd",
-                d: "M7.71 8.23l3.75 3.75-1.48 1.48-3.75-3.75-3.75 3.75L1 11.98l3.75-3.75L1 4.48 2.48 3l3.75 3.75L9.98 3l1.48 1.48-3.75 3.75z"
-            })))
-        }
-
-        function C(e) {
-            var t, n, i = e.delay,
-                o = e.isRunning,
-                s = e.closeToast,
-                l = e.type,
-                c = e.hide,
-                f = e.className,
-                d = e.style,
-                h = e.controlledProgress,
-                m = e.progress,
-                g = e.rtl,
-                v = e.isIn,
-                b = e.theme,
-                E = u({}, d, {
-                    animationDuration: i + "ms",
-                    animationPlayState: o ? "running" : "paused",
-                    opacity: c ? 0 : 1
-                });
-            h && (E.transform = "scaleX(" + m + ")");
-            var y = a("Toastify__progress-bar", h ? "Toastify__progress-bar--controlled" : "Toastify__progress-bar--animated", "Toastify__progress-bar-theme--" + b, "Toastify__progress-bar--" + l, ((t = {})["Toastify__progress-bar--rtl"] = g, t)),
-                _ = p(f) ? f({
-                    rtl: g,
-                    type: l,
-                    defaultClassName: y
-                }) : a(y, f),
-                T = ((n = {})[h && m >= 1 ? "onTransitionEnd" : "onAnimationEnd"] = h && m < 1 ? null : function() {
-                    v && s()
-                }, n);
-            return Object(r.createElement)("div", Object.assign({
-                role: "progressbar",
-                "aria-hidden": c ? "true" : "false",
-                "aria-label": "notification timer",
-                className: _,
-                style: E
-            }, T))
-        }
-        C.defaultProps = {
-            type: E.DEFAULT,
-            hide: !1
-        };
-        var S = ["theme", "type"],
-            I = function(e) {
-                var t = e.theme,
-                    n = e.type,
-                    i = l(e, S);
-                return Object(r.createElement)("svg", Object.assign({
-                    viewBox: "0 0 24 24",
-                    width: "100%",
-                    height: "100%",
-                    fill: "colored" === t ? "currentColor" : "var(--toastify-icon-color-" + n + ")"
-                }, i))
-            };
-        var N = {
-                info: function(e) {
-                    return Object(r.createElement)(I, Object.assign({}, e), Object(r.createElement)("path", {
-                        d: "M12 0a12 12 0 1012 12A12.013 12.013 0 0012 0zm.25 5a1.5 1.5 0 11-1.5 1.5 1.5 1.5 0 011.5-1.5zm2.25 13.5h-4a1 1 0 010-2h.75a.25.25 0 00.25-.25v-4.5a.25.25 0 00-.25-.25h-.75a1 1 0 010-2h1a2 2 0 012 2v4.75a.25.25 0 00.25.25h.75a1 1 0 110 2z"
-                    }))
-                },
-                warning: function(e) {
-                    return Object(r.createElement)(I, Object.assign({}, e), Object(r.createElement)("path", {
-                        d: "M23.32 17.191L15.438 2.184C14.728.833 13.416 0 11.996 0c-1.42 0-2.733.833-3.443 2.184L.533 17.448a4.744 4.744 0 000 4.368C1.243 23.167 2.555 24 3.975 24h16.05C22.22 24 24 22.044 24 19.632c0-.904-.251-1.746-.68-2.44zm-9.622 1.46c0 1.033-.724 1.823-1.698 1.823s-1.698-.79-1.698-1.822v-.043c0-1.028.724-1.822 1.698-1.822s1.698.79 1.698 1.822v.043zm.039-12.285l-.84 8.06c-.057.581-.408.943-.897.943-.49 0-.84-.367-.896-.942l-.84-8.065c-.057-.624.25-1.095.779-1.095h1.91c.528.005.84.476.784 1.1z"
-                    }))
-                },
-                success: function(e) {
-                    return Object(r.createElement)(I, Object.assign({}, e), Object(r.createElement)("path", {
-                        d: "M12 0a12 12 0 1012 12A12.014 12.014 0 0012 0zm6.927 8.2l-6.845 9.289a1.011 1.011 0 01-1.43.188l-4.888-3.908a1 1 0 111.25-1.562l4.076 3.261 6.227-8.451a1 1 0 111.61 1.183z"
-                    }))
-                },
-                error: function(e) {
-                    return Object(r.createElement)(I, Object.assign({}, e), Object(r.createElement)("path", {
-                        d: "M11.983 0a12.206 12.206 0 00-8.51 3.653A11.8 11.8 0 000 12.207 11.779 11.779 0 0011.8 24h.214A12.111 12.111 0 0024 11.791 11.766 11.766 0 0011.983 0zM10.5 16.542a1.476 1.476 0 011.449-1.53h.027a1.527 1.527 0 011.523 1.47 1.475 1.475 0 01-1.449 1.53h-.027a1.529 1.529 0 01-1.523-1.47zM11 12.5v-6a1 1 0 012 0v6a1 1 0 11-2 0z"
-                    }))
-                },
-                spinner: function() {
-                    return Object(r.createElement)("div", {
-                        className: "Toastify__spinner"
-                    })
-                }
-            },
-            x = function(e) {
-                var t, n, i = k(e),
-                    o = i.isRunning,
-                    s = i.preventExitTransition,
-                    u = i.toastRef,
-                    l = i.eventHandlers,
-                    c = e.closeButton,
-                    f = e.children,
-                    h = e.autoClose,
-                    m = e.onClick,
-                    g = e.type,
-                    v = e.hideProgressBar,
-                    b = e.closeToast,
-                    E = e.transition,
-                    y = e.position,
-                    _ = e.className,
-                    T = e.style,
-                    w = e.bodyClassName,
-                    O = e.bodyStyle,
-                    A = e.progressClassName,
-                    D = e.progressStyle,
-                    S = e.updateId,
-                    I = e.role,
-                    x = e.progress,
-                    R = e.rtl,
-                    L = e.toastId,
-                    M = e.deleteToast,
-                    P = e.isIn,
-                    F = e.isLoading,
-                    B = e.icon,
-                    j = e.theme,
-                    U = a("Toastify__toast", "Toastify__toast-theme--" + j, "Toastify__toast--" + g, ((t = {})["Toastify__toast--rtl"] = R, t)),
-                    H = p(_) ? _({
-                        rtl: R,
-                        position: y,
-                        type: g,
-                        defaultClassName: U
-                    }) : a(U, _),
-                    G = !!x,
-                    z = N[g],
-                    q = {
-                        theme: j,
-                        type: g
-                    },
-                    V = z && z(q);
-                return !1 === B ? V = void 0 : p(B) ? V = B(q) : Object(r.isValidElement)(B) ? V = Object(r.cloneElement)(B, q) : d(B) ? V = B : F && (V = N.spinner()), Object(r.createElement)(E, {
-                    isIn: P,
-                    done: M,
-                    position: y,
-                    preventExitTransition: s,
-                    nodeRef: u
-                }, Object(r.createElement)("div", Object.assign({
-                    id: L,
-                    onClick: m,
-                    className: H
-                }, l, {
-                    style: T,
-                    ref: u
-                }), Object(r.createElement)("div", Object.assign({}, P && {
-                    role: I
-                }, {
-                    className: p(w) ? w({
-                        type: g
-                    }) : a("Toastify__toast-body", w),
-                    style: O
-                }), V && Object(r.createElement)("div", {
-                    className: a("Toastify__toast-icon", (n = {}, n["Toastify--animate-icon Toastify__zoom-enter"] = !F, n))
-                }, V), Object(r.createElement)("div", null, f)), function(e) {
-                    if (e) {
-                        var t = {
-                            closeToast: b,
-                            type: g,
-                            theme: j
-                        };
-                        return p(e) ? e(t) : Object(r.isValidElement)(e) ? Object(r.cloneElement)(e, t) : void 0
-                    }
-                }(c), (h || G) && Object(r.createElement)(C, Object.assign({}, S && !G ? {
-                    key: "pb-" + S
-                } : {}, {
-                    rtl: R,
-                    theme: j,
-                    delay: h,
-                    isRunning: o,
-                    isIn: P,
-                    closeToast: b,
-                    hide: v,
-                    type: g,
-                    style: D,
-                    className: A,
-                    controlledProgress: G,
-                    progress: x
-                }))))
-            },
-            R = y({
-                enter: "Toastify--animate Toastify__bounce-enter",
-                exit: "Toastify--animate Toastify__bounce-exit",
-                appendPosition: !0
-            }),
-            L = function(e) {
-                var t = w(e),
-                    n = t.getToastToRender,
-                    i = t.containerRef,
-                    o = t.isToastActive,
-                    s = e.className,
-                    l = e.style,
-                    c = e.rtl,
-                    f = e.containerId;
-
-                function d(e) {
-                    var t, n = a("Toastify__toast-container", "Toastify__toast-container--" + e, ((t = {})["Toastify__toast-container--rtl"] = c, t));
-                    return p(s) ? s({
-                        position: e,
-                        rtl: c,
-                        defaultClassName: n
-                    }) : a(n, h(s))
-                }
-                return Object(r.createElement)("div", {
-                    ref: i,
-                    className: "Toastify",
-                    id: f
-                }, n((function(e, t) {
-                    var n = t.length ? u({}, l) : u({}, l, {
-                        pointerEvents: "none"
-                    });
-                    return Object(r.createElement)("div", {
-                        className: d(e),
-                        style: n,
-                        key: "container-" + e
-                    }, t.map((function(e) {
-                        var t = e.content,
-                            n = e.props;
-                        return Object(r.createElement)(x, Object.assign({}, n, {
-                            isIn: o(n.toastId),
-                            key: "toast-" + n.key,
-                            closeButton: !0 === n.closeButton ? D : n.closeButton
-                        }), t)
-                    })))
-                })))
-            };
-        L.defaultProps = {
-            position: b.TOP_RIGHT,
-            transition: R,
-            rtl: !1,
-            autoClose: 5e3,
-            hideProgressBar: !1,
-            closeButton: D,
-            pauseOnHover: !0,
-            pauseOnFocusLoss: !0,
-            closeOnClick: !0,
-            newestOnTop: !1,
-            draggable: !0,
-            draggablePercent: 80,
-            draggableDirection: "x",
-            role: "alert",
-            theme: "light"
-        };
-        var M, P, F, B = new Map,
-            j = [],
-            U = !1;
-
-        function H() {
-            return Math.random().toString(36).substring(2, 9)
-        }
-
-        function G(e) {
-            return e && (d(e.toastId) || c(e.toastId)) ? e.toastId : H()
-        }
-
-        function z(e, t) {
-            return B.size > 0 ? _.emit(0, e, t) : (j.push({
-                content: e,
-                options: t
-            }), U && g && (U = !1, P = document.createElement("div"), document.body.appendChild(P), Object(s.render)(Object(r.createElement)(L, Object.assign({}, F)), P))), t.toastId
-        }
-
-        function q(e, t) {
-            return u({}, t, {
-                type: t && t.type || e,
-                toastId: G(t)
-            })
-        }
-
-        function V(e) {
-            return function(t, n) {
-                return z(t, q(e, n))
-            }
-        }
-
-        function K(e, t) {
-            return z(e, q(E.DEFAULT, t))
-        }
-        K.loading = function(e, t) {
-            return z(e, q(E.DEFAULT, u({
-                isLoading: !0,
-                autoClose: !1,
-                closeOnClick: !1,
-                closeButton: !1,
-                draggable: !1
-            }, t)))
-        }, K.promise = function(e, t, n) {
-            var r, i = t.pending,
-                o = t.error,
-                a = t.success;
-            i && (r = d(i) ? K.loading(i, n) : K.loading(i.render, u({}, n, i)));
-            var s = {
-                    isLoading: null,
-                    autoClose: null,
-                    closeOnClick: null,
-                    closeButton: null,
-                    draggable: null
-                },
-                l = function(e, t, i) {
-                    if (null != t) {
-                        var o = u({
-                                type: e
-                            }, s, n, {
-                                data: i
-                            }),
-                            a = d(t) ? {
-                                render: t
-                            } : t;
-                        return r ? K.update(r, u({}, o, a)) : K(a.render, u({}, o, a)), i
-                    }
-                    K.dismiss(r)
-                },
-                c = p(e) ? e() : e;
-            return c.then((function(e) {
-                return l("success", a, e)
-            })).catch((function(e) {
-                return l("error", o, e)
-            })), c
-        }, K.success = V(E.SUCCESS), K.info = V(E.INFO), K.error = V(E.ERROR), K.warning = V(E.WARNING), K.warn = K.warning, K.dark = function(e, t) {
-            return z(e, q(E.DEFAULT, u({
-                theme: "dark"
-            }, t)))
-        }, K.dismiss = function(e) {
-            return _.emit(1, e)
-        }, K.clearWaitingQueue = function(e) {
-            return void 0 === e && (e = {}), _.emit(5, e)
-        }, K.isActive = function(e) {
-            var t = !1;
-            return B.forEach((function(n) {
-                n.isToastActive && n.isToastActive(e) && (t = !0)
-            })), t
-        }, K.update = function(e, t) {
-            void 0 === t && (t = {}), setTimeout((function() {
-                var n = function(e, t) {
-                    var n = t.containerId,
-                        r = B.get(n || M);
-                    return r ? r.getToast(e) : null
-                }(e, t);
-                if (n) {
-                    var r = n.props,
-                        i = n.content,
-                        o = u({}, r, t, {
-                            toastId: t.toastId || e,
-                            updateId: H()
-                        });
-                    o.toastId !== e && (o.staleId = e);
-                    var a = o.render || i;
-                    delete o.render, z(a, o)
-                }
-            }), 0)
-        }, K.done = function(e) {
-            K.update(e, {
-                progress: 1
-            })
-        }, K.onChange = function(e) {
-            return p(e) && _.on(4, e),
-                function() {
-                    p(e) && _.off(4, e)
-                }
-        }, K.configure = function(e) {
-            void 0 === e && (e = {}), U = !0, F = e
-        }, K.POSITION = b, K.TYPE = E, _.on(2, (function(e) {
-            M = e.containerId || e, B.set(M, e), j.forEach((function(e) {
-                _.emit(0, e.content, e.options)
-            })), j = []
-        })).on(3, (function(e) {
-            B.delete(e.containerId || e), 0 === B.size && _.off(0).off(1).off(5), g && P && document.body.removeChild(P)
-        }))
-    }, function(e, t, n) {
-        "use strict";
 
         function r(e) {
             return e.replace(/[\t\n\r ]+/g, " ").replace(/^ | $/g, "").toLowerCase().toUpperCase()
         }
         n.d(t, "a", (function() {
             return r
         }))
@@ -6736,15 +6736,15 @@
             }) : e[t] = n, e
         }
         n.d(t, "a", (function() {
             return r
         }))
     }, function(e, t, n) {
         var r = n(262),
-            i = n(122),
+            i = n(121),
             o = n(35),
             a = n(36),
             s = n(72),
             u = n(26),
             l = n(28),
             c = {
                 exports: {}
@@ -7820,15 +7820,15 @@
                     writable: !0,
                     configurable: !0
                 }
             }), t && r(e, t)
         }
     }, function(e, t, n) {
         var r = n(62),
-            i = n(121),
+            i = n(120),
             o = n(268);
         e.exports = function(e) {
             var t = i();
             return function() {
                 var n, i = r(e);
                 if (t) {
                     var a = r(this).constructor;
@@ -7994,15 +7994,15 @@
             var o = n.indexOf(":"),
                 a = n.indexOf("?"),
                 s = n.indexOf("#"),
                 u = n.indexOf("/");
             return o < 0 || u > -1 && o > u || a > -1 && o > a || s > -1 && o > s || t.test(n.slice(0, o)) ? n : ""
         }
     }, function(e, t, n) {
-        var r = n(110),
+        var r = n(109),
             i = "object" == typeof self && self && self.Object === Object && self,
             o = r || i || Function("return this")();
         e.exports = o
     }, function(e, t, n) {
         "use strict";
         n.d(t, "a", (function() {
             return i
@@ -10891,15 +10891,15 @@
             }
         };
         Object.defineProperty(t, "__esModule", {
             value: !0
         }), t.checkValuesAgainstBoundaries = t.relativeValue = t.useThumbOverlap = t.Direction = t.getTrackBackground = t.Range = void 0;
         var i = r(n(195));
         t.Range = i.default;
-        var o = n(107);
+        var o = n(106);
         Object.defineProperty(t, "getTrackBackground", {
             enumerable: !0,
             get: function() {
                 return o.getTrackBackground
             }
         }), Object.defineProperty(t, "useThumbOverlap", {
             enumerable: !0,
@@ -13565,16 +13565,16 @@
             return ue
         }));
         var r = n(14),
             i = n(169),
             o = n.n(i),
             a = n(37),
             s = n(30),
-            u = n(21),
-            l = n(118),
+            u = n(22),
+            l = n(117),
             c = n(51),
             f = /[#.]/g,
             d = function(e) {
                 for (var t, n, r, i = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "div", o = e || "", a = {}, s = 0; s < o.length;) f.lastIndex = s, r = f.exec(o), (t = o.slice(s, r ? r.index : o.length)) && (n ? "#" === n ? a.id = t : Array.isArray(a.className) ? a.className.push(t) : a.className = [t] : i = t, s += t.length), r && (n = r[0], s++);
                 return {
                     type: "element",
                     tagName: i,
@@ -13807,15 +13807,15 @@
             return e.line && e.column ? e : null
         }
 
         function x(e) {
             return "messages" in e
         }
         var R = n(8),
-            L = n(119),
+            L = n(118),
             M = n(84),
             P = n.n(M),
             F = n(31),
             B = O,
             j = L.a,
             U = {}.hasOwnProperty,
             H = Object(F.a)("root"),
@@ -14497,15 +14497,15 @@
             function(e) {
                 e.Right = "to right", e.Left = "to left", e.Down = "to bottom", e.Up = "to top"
             }(t.Direction || (t.Direction = {}))
     }, function(e, t, n) {
         var r = n(44).Symbol;
         e.exports = r
     }, function(e, t, n) {
-        var r = n(120);
+        var r = n(119);
         e.exports = function(e, t) {
             if (e) {
                 if ("string" === typeof e) return r(e, t);
                 var n = Object.prototype.toString.call(e).slice(8, -1);
                 return "Object" === n && e.constructor && (n = e.constructor.name), "Map" === n || "Set" === n ? Array.from(e) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? r(e, t) : void 0
             }
         }
@@ -14676,19 +14676,14 @@
                             }
                         }
                     }
                 }]), n
             }(n(38));
         e.exports = s
     }, function(e, t, n) {
-        var r = n(187),
-            i = n(188),
-            o = i;
-        o.v1 = r, o.v4 = i, e.exports = o
-    }, function(e, t, n) {
         "use strict";
         Object.defineProperty(t, "__esModule", {
             value: !0
         }), t.FilePond = t.FileStatus = t.registerPlugin = void 0;
         var r, i = function() {
                 function e(e, t) {
                     for (var n = 0; n < t.length; n++) {
@@ -15057,15 +15052,15 @@
                         } else i.visibility = "hidden"
                     }
                     g(d), p(i)
                 }
             }), [e, n]), [m, d]
         }
     }, function(e, t, n) {
-        var r = n(109);
+        var r = n(108);
         e.exports = function(e, t) {
             if (e) {
                 if ("string" === typeof e) return r(e, t);
                 var n = Object.prototype.toString.call(e).slice(8, -1);
                 return "Object" === n && e.constructor && (n = e.constructor.name), "Map" === n || "Set" === n ? Array.from(e) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? r(e, t) : void 0
             }
         }, e.exports.default = e.exports, e.exports.__esModule = !0
@@ -15078,15 +15073,15 @@
     }, function(e, t, n) {
         (function(t) {
             var n = "object" == typeof t && t && t.Object === Object && t;
             e.exports = n
         }).call(this, n(93))
     }, function(e, t, n) {
         var r = n(61),
-            i = n(112);
+            i = n(111);
         e.exports = function(e) {
             if (!i(e)) return !1;
             var t = r(e);
             return "[object Function]" == t || "[object GeneratorFunction]" == t || "[object AsyncFunction]" == t || "[object Proxy]" == t
         }
     }, function(e, t) {
         e.exports = function(e) {
@@ -15103,16 +15098,16 @@
                 try {
                     return e + ""
                 } catch (t) {}
             }
             return ""
         }
     }, function(e, t, n) {
-        var r = n(111),
-            i = n(115);
+        var r = n(110),
+            i = n(114);
         e.exports = function(e) {
             return null != e && i(e.length) && !r(e)
         }
     }, function(e, t) {
         e.exports = function(e) {
             return "number" == typeof e && e > -1 && e % 1 == 0 && e <= 9007199254740991
         }
@@ -15226,15 +15221,15 @@
         "use strict";
         var r = n(26),
             i = n(28),
             o = n(35),
             a = n(36),
             s = n(38),
             u = n(74),
-            l = n(124),
+            l = n(123),
             c = function(e) {
                 o(n, e);
                 var t = a(n);
 
                 function n(e) {
                     var i;
                     return r(this, n), (i = t.call(this, e)).tokenizer = e, i.posTracker = s.install(e.preprocessor, l), i.currentAttrLocation = null, i.ctLoc = null, i
@@ -15359,14 +15354,19 @@
             }, i(t, n, o || t)
         }
         e.exports = i
     }, function(e, t, n) {
         "use strict";
         e.exports = n(185)
     }, function(e, t, n) {
+        var r = n(187),
+            i = n(188),
+            o = i;
+        o.v1 = r, o.v4 = i, e.exports = o
+    }, function(e, t, n) {
         e.exports = function() {
             "use strict";
             var e = function(e) {
                     return /^image\/jpeg/.test(e.type)
                 },
                 t = {
                     JPEG: 65496,
@@ -33013,16 +33013,16 @@
         }(e.exports);
         try {
             regeneratorRuntime = r
         } catch (i) {
             "object" === typeof globalThis ? globalThis.regeneratorRuntime = r : Function("r", "regeneratorRuntime = r")(r)
         }
     }, function(e, t, n) {
-        var r, i, o = n(105),
-            a = n(106),
+        var r, i, o = n(104),
+            a = n(105),
             s = 0,
             u = 0;
         e.exports = function(e, t, n) {
             var l = t && n || 0,
                 c = t || [],
                 f = (e = e || {}).node || r,
                 d = void 0 !== e.clockseq ? e.clockseq : i;
@@ -33039,16 +33039,16 @@
             c[l++] = v >>> 24 & 255, c[l++] = v >>> 16 & 255, c[l++] = v >>> 8 & 255, c[l++] = 255 & v;
             var b = h / 4294967296 * 1e4 & 268435455;
             c[l++] = b >>> 8 & 255, c[l++] = 255 & b, c[l++] = b >>> 24 & 15 | 16, c[l++] = b >>> 16 & 255, c[l++] = d >>> 8 | 128, c[l++] = 255 & d;
             for (var E = 0; E < 6; ++E) c[l + E] = f[E];
             return t || a(c)
         }
     }, function(e, t, n) {
-        var r = n(105),
-            i = n(106);
+        var r = n(104),
+            i = n(105);
         e.exports = function(e, t, n) {
             var o = t && n || 0;
             "string" == typeof e && (t = "binary" === e ? new Array(16) : null, e = null);
             var a = (e = e || {}).random || (e.rng || r)();
             if (a[6] = 15 & a[6] | 64, a[8] = 63 & a[8] | 128, t)
                 for (var s = 0; s < 16; ++s) t[o + s] = a[s];
             return t || i(a)
@@ -33900,15 +33900,15 @@
                     for (var o = arguments[t], a = 0, s = o.length; a < s; a++, i++) r[i] = o[a];
                 return r
             };
         Object.defineProperty(t, "__esModule", {
             value: !0
         });
         var u = a(n(1)),
-            l = n(107),
+            l = n(106),
             c = n(94),
             f = ["ArrowRight", "ArrowUp", "k", "PageUp"],
             d = ["ArrowLeft", "ArrowDown", "j", "PageDown"],
             p = function(e) {
                 function t(t) {
                     var n = e.call(this, t) || this;
                     if (n.trackRef = u.createRef(), n.thumbRefs = [], n.markRefs = [], n.state = {
@@ -34295,15 +34295,15 @@
                     max: 100
                 }, t
             }(u.Component);
         t.default = p
     }, function(e, t, n) {
         var r = n(197),
             i = n(198),
-            o = n(108),
+            o = n(107),
             a = n(199);
         e.exports = function(e, t) {
             return r(e) || i(e, t) || o(e, t) || a()
         }, e.exports.default = e.exports, e.exports.__esModule = !0
     }, function(e, t) {
         e.exports = function(e) {
             if (Array.isArray(e)) return e
@@ -34351,21 +34351,21 @@
                 o = Object.keys(e);
             for (r = 0; r < o.length; r++) n = o[r], t.indexOf(n) >= 0 || (i[n] = e[n]);
             return i
         }, e.exports.default = e.exports, e.exports.__esModule = !0
     }, function(e, t, n) {
         var r = n(203),
             i = n(204),
-            o = n(108),
+            o = n(107),
             a = n(205);
         e.exports = function(e) {
             return r(e) || i(e) || o(e) || a()
         }, e.exports.default = e.exports, e.exports.__esModule = !0
     }, function(e, t, n) {
-        var r = n(109);
+        var r = n(108);
         e.exports = function(e) {
             if (Array.isArray(e)) return r(e)
         }, e.exports.default = e.exports, e.exports.__esModule = !0
     }, function(e, t) {
         e.exports = function(e) {
             if ("undefined" !== typeof Symbol && null != e[Symbol.iterator] || null != e["@@iterator"]) return Array.from(e)
         }, e.exports.default = e.exports, e.exports.__esModule = !0
@@ -40326,15 +40326,15 @@
         }, p.strip = function(e) {
             return p.replace(e, "", !0)
         }, e.exports = p
     }, function(e, t, n) {
         var r = n(95),
             i = n(213),
             o = n(214),
-            a = n(114),
+            a = n(113),
             s = n(226),
             u = n(227),
             l = n(228),
             c = n(229),
             f = n(230),
             d = n(234),
             p = r ? r.iterator : void 0;
@@ -40355,15 +40355,15 @@
     }, function(e, t, n) {
         var r = n(215),
             i = n(222),
             o = n(223),
             a = n(224),
             s = n(225),
             u = n(61),
-            l = n(113),
+            l = n(112),
             c = "[object Map]",
             f = "[object Promise]",
             d = "[object Set]",
             p = "[object WeakMap]",
             h = "[object DataView]",
             m = l(r),
             g = l(i),
@@ -40389,18 +40389,18 @@
             }
             return t
         }), e.exports = y
     }, function(e, t, n) {
         var r = n(60)(n(44), "DataView");
         e.exports = r
     }, function(e, t, n) {
-        var r = n(111),
+        var r = n(110),
             i = n(219),
-            o = n(112),
-            a = n(113),
+            o = n(111),
+            a = n(112),
             s = /^\[object .+?Constructor\]$/,
             u = Function.prototype,
             l = Object.prototype,
             c = u.toString,
             f = l.hasOwnProperty,
             d = RegExp("^" + c.call(f).replace(/[\\^$.*+?()[\]{}|]/g, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$");
         e.exports = function(e) {
@@ -40453,15 +40453,15 @@
         var r = n(60)(n(44), "Set");
         e.exports = r
     }, function(e, t, n) {
         var r = n(60)(n(44), "WeakMap");
         e.exports = r
     }, function(e, t, n) {
         var r = n(61),
-            i = n(116),
+            i = n(115),
             o = n(71);
         e.exports = function(e) {
             return "string" == typeof e || !i(e) && o(e) && "[object String]" == r(e)
         }
     }, function(e, t) {
         e.exports = function(e) {
             for (var t, n = []; !(t = e.next()).done;) n.push(t.value);
@@ -40531,22 +40531,22 @@
         e.exports = function(e, t) {
             for (var n = -1, r = null == e ? 0 : e.length, i = Array(r); ++n < r;) i[n] = t(e[n], n, e);
             return i
         }
     }, function(e, t, n) {
         var r = n(238),
             i = n(249),
-            o = n(114);
+            o = n(113);
         e.exports = function(e) {
             return o(e) ? r(e) : i(e)
         }
     }, function(e, t, n) {
         var r = n(239),
             i = n(240),
-            o = n(116),
+            o = n(115),
             a = n(242),
             s = n(244),
             u = n(245),
             l = Object.prototype.hasOwnProperty;
         e.exports = function(e, t) {
             var n = o(e),
                 c = !n && i(e),
@@ -40586,15 +40586,15 @@
             var r = n(44),
                 i = n(243),
                 o = t && !t.nodeType && t,
                 a = o && "object" == typeof e && e && !e.nodeType && e,
                 s = a && a.exports === o ? r.Buffer : void 0,
                 u = (s ? s.isBuffer : void 0) || i;
             e.exports = u
-        }).call(this, n(117)(e))
+        }).call(this, n(116)(e))
     }, function(e, t) {
         e.exports = function() {
             return !1
         }
     }, function(e, t) {
         var n = /^(?:0|[1-9]\d*)$/;
         e.exports = function(e, t) {
@@ -40606,40 +40606,40 @@
             i = n(247),
             o = n(248),
             a = o && o.isTypedArray,
             s = a ? i(a) : r;
         e.exports = s
     }, function(e, t, n) {
         var r = n(61),
-            i = n(115),
+            i = n(114),
             o = n(71),
             a = {};
         a["[object Float32Array]"] = a["[object Float64Array]"] = a["[object Int8Array]"] = a["[object Int16Array]"] = a["[object Int32Array]"] = a["[object Uint8Array]"] = a["[object Uint8ClampedArray]"] = a["[object Uint16Array]"] = a["[object Uint32Array]"] = !0, a["[object Arguments]"] = a["[object Array]"] = a["[object ArrayBuffer]"] = a["[object Boolean]"] = a["[object DataView]"] = a["[object Date]"] = a["[object Error]"] = a["[object Function]"] = a["[object Map]"] = a["[object Number]"] = a["[object Object]"] = a["[object RegExp]"] = a["[object Set]"] = a["[object String]"] = a["[object WeakMap]"] = !1, e.exports = function(e) {
             return o(e) && i(e.length) && !!a[r(e)]
         }
     }, function(e, t) {
         e.exports = function(e) {
             return function(t) {
                 return e(t)
             }
         }
     }, function(e, t, n) {
         (function(e) {
-            var r = n(110),
+            var r = n(109),
                 i = t && !t.nodeType && t,
                 o = i && "object" == typeof e && e && !e.nodeType && e,
                 a = o && o.exports === i && r.process,
                 s = function() {
                     try {
                         var e = o && o.require && o.require("util").types;
                         return e || a && a.binding && a.binding("util")
                     } catch (t) {}
                 }();
             e.exports = s
-        }).call(this, n(117)(e))
+        }).call(this, n(116)(e))
     }, function(e, t, n) {
         var r = n(250),
             i = n(251),
             o = Object.prototype.hasOwnProperty;
         e.exports = function(e) {
             if (!r(e)) return i(e);
             var t = [];
@@ -40904,15 +40904,15 @@
             };
             return n.PropTypes = n, n
         }
     }, function(e, t, n) {
         "use strict";
         e.exports = "SECRET_DO_NOT_PASS_THIS_OR_YOU_WILL_BE_FIRED"
     }, function(e, t, n) {
-        var r = n(120);
+        var r = n(119);
         e.exports = function(e) {
             if (Array.isArray(e)) return r(e)
         }
     }, function(e, t) {
         e.exports = function(e) {
             if ("undefined" !== typeof Symbol && Symbol.iterator in Object(e)) return Array.from(e)
         }
@@ -41001,15 +41001,15 @@
         e.exports = s
     }, function(e, t) {
         e.exports = function(e) {
             return -1 !== Function.toString.call(e).indexOf("[native code]")
         }
     }, function(e, t, n) {
         var r = n(97),
-            i = n(121);
+            i = n(120);
 
         function o(t, n, a) {
             return i() ? e.exports = o = Reflect.construct : e.exports = o = function(e, t, n) {
                 var i = [null];
                 i.push.apply(i, t);
                 var o = new(Function.bind.apply(e, i));
                 return n && r(o, n.prototype), o
@@ -41544,15 +41544,15 @@
         "use strict";
         var r = n(26),
             i = n(28),
             o = n(35),
             a = n(36),
             s = n(38),
             u = n(74),
-            l = n(123),
+            l = n(122),
             c = n(276),
             f = n(54).TAG_NAMES,
             d = function(e) {
                 o(n, e);
                 var t = a(n);
 
                 function n(e) {
@@ -41702,15 +41702,15 @@
         "use strict";
         var r = n(26),
             i = n(28),
             o = n(35),
             a = n(36),
             s = n(100),
             u = n(278),
-            l = n(123),
+            l = n(122),
             c = n(38),
             f = function(e) {
                 o(n, e);
                 var t = a(n);
 
                 function n(e, i) {
                     var o;
@@ -41760,20 +41760,20 @@
                 return n
             }(a);
         e.exports = l
     }, function(e, t, n) {
         "use strict";
         var r = n(26),
             i = n(28),
-            o = n(125),
+            o = n(124),
             a = n(62),
             s = n(35),
             u = n(36),
             l = n(100),
-            c = n(124),
+            c = n(123),
             f = n(38),
             d = function(e) {
                 s(n, e);
                 var t = u(n);
 
                 function n(e, i) {
                     var o;
@@ -42159,23 +42159,23 @@
                             return i === c || i === f
                         } return t === u.SVG && (e === s.FOREIGN_OBJECT || e === s.DESC || e === s.TITLE)
             }(e, t, n)) || !(r && r !== u.MATHML || ! function(e, t) {
                 return t === u.MATHML && (e === s.MI || e === s.MO || e === s.MN || e === s.MS || e === s.MTEXT)
             }(e, t))
         }
     }, function(e, t, n) {}, function(e, t, n) {
-        var r = n(125),
+        var r = n(124),
             i = n(62),
             o = n(287),
             a = n(72),
             s = n(35),
             u = n(36),
             l = n(26),
             c = n(28),
-            f = n(122);
+            f = n(121);
         e.exports = function(e) {
             "use strict";
 
             function t(e) {
                 if (e && e.__esModule) return e;
                 var t = Object.create(null);
                 if (e) {
@@ -46341,15 +46341,15 @@
         var x = n(67);
 
         function R(e) {
             if (e) throw e
         }
         var L = n(130),
             M = n.n(L),
-            P = n(103),
+            P = n(102),
             F = n.n(P);
 
         function B(e) {
             if ("[object Object]" !== Object.prototype.toString.call(e)) return !1;
             var t = Object.getPrototypeOf(e);
             return null === t || t === Object.prototype
         }
@@ -49209,15 +49209,15 @@
                 return function(t) {
                     return $t(t, e)
                 }
             }(e || t)
         };
         var Qt = n(16),
             Zt = n.n(Qt),
-            Jt = n(21);
+            Jt = n(22);
 
         function en(e) {
             if (e.allowedElements && e.disallowedElements) throw new TypeError("Only one of `allowedElements` and `disallowedElements` should be defined");
             if (e.allowedElements || e.disallowedElements || e.allowElement) return function(t) {
                 Object(Ct.a)(t, "element", (function(t, n, r) {
                     var i, o = r;
                     if (e.allowedElements ? i = !e.allowedElements.includes(t.tagName) : e.disallowedElements && (i = e.disallowedElements.includes(t.tagName)), !i && e.allowElement && "number" === typeof n && (i = !e.allowElement(t, n, o)), i && "number" === typeof n) {
@@ -49233,16 +49233,16 @@
         var nn = n(132),
             rn = n.n(nn);
 
         function on(e) {
             var t = e && "object" === typeof e && "text" === e.type ? e.value || "" : e;
             return "string" === typeof t && "" === t.replace(/[ \t\n\f\r]/g, "")
         }
-        var an = n(118),
-            sn = n(119),
+        var an = n(117),
+            sn = n(118),
             un = n(53),
             ln = n(52),
             cn = n(84),
             fn = n.n(cn),
             dn = {}.hasOwnProperty,
             pn = new Set(["table", "thead", "tbody", "tfoot", "tr"]);
 
@@ -50788,8 +50788,8 @@
                     if ("no-highlight" === r || "nohighlight" === r) return !1;
                     if ("lang-" === r.slice(0, 5)) return r.slice(5);
                     if ("language-" === r.slice(0, 9)) return r.slice(9)
                 }
         }
     }]
 ]);
-//# sourceMappingURL=2.6305b467.chunk.js.map
+//# sourceMappingURL=2.206848a5.chunk.js.map
```

### Comparing `mercury-2.2.9/mercury/frontend-dist/static/js/2.6305b467.chunk.js.LICENSE.txt` & `mercury-2.3.0/mercury/frontend-dist/static/js/2.206848a5.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mercury-2.2.9/mercury/frontend-dist/static/js/2.6305b467.chunk.js.map` & `mercury-2.3.0/mercury/frontend-dist/static/js/2.206848a5.chunk.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8489968961941072%*

 * *Differences: {"'file'": "'static/js/2.206848a5.chunk.js'",*

 * * "'mappings'": "';kGAGEA,EAAOC,QAAUC,EAAQ,M,6BCAzBF,EAAOC,QAAUC,EAAQ,M,6BCH3B,2UAAIC,EAAS,EAEAC,EAAUC,IACVC,EAAaD,IACbE,EAAoBF,IACpBG,EAASH,IACTI,EAAiBJ,IACjBK,EAAiBL,IACjBM,EAAwBN,IAErC,SAASA,IACP,gBAAO,IAAOF,K,qbCLT,ICWMS,EAAaC,EAAW,YAQxBC,EAAaD,EAAW,MAexBE,EAAgBF,EAAW,cAS3BG,EAAoBH,EAAW,cAU/BI,EAAmBJ,EAAW,kBAkB9BK,EAAaL,EAAW,uBAW9B,SAASM,EAAaC,GAC3B,OAGW,OAATA,IAAkBA,EAAO,IAAe,MAATA,GAW5B,SAASC,EAA0BD,GACxC,OAAgB,OAATA,IAAkBA,EAAO,GAAc,KAATA,GAgBhC,SAASE,EAAm […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/2.6305b467.chunk.js",
+    "file": "static/js/2.206848a5.chunk.js",
     "names": [
         "module",
         "exports",
         "require",
         "powers",
         "boolean",
         "increment",
@@ -861,14 +861,214 @@
         "onClick",
         "defaultSearchParamsRef",
         "hasSetSearchParamsRef",
         "defaultSearchParams",
         "setSearchParams",
         "newSearchParams",
         "nextInit",
+        "toVal",
+        "mix",
+        "k",
+        "tmp",
+        "isNum",
+        "isNaN",
+        "isBool",
+        "isStr",
+        "isFn",
+        "parseClassName",
+        "isToastIdValid",
+        "toastId",
+        "canUseDom",
+        "canBeRendered",
+        "isValidElement",
+        "POSITION",
+        "TOP_LEFT",
+        "TOP_RIGHT",
+        "TOP_CENTER",
+        "BOTTOM_LEFT",
+        "BOTTOM_RIGHT",
+        "BOTTOM_CENTER",
+        "TYPE",
+        "INFO",
+        "SUCCESS",
+        "WARNING",
+        "ERROR",
+        "DEFAULT",
+        "cssTransition",
+        "appendPosition",
+        "collapse",
+        "collapseDuration",
+        "preventExitTransition",
+        "nodeRef",
+        "isIn",
+        "enterClassName",
+        "exitClassName",
+        "baseClassName",
+        "animationStep",
+        "node",
+        "Event",
+        "duration",
+        "scrollHeight",
+        "requestAnimationFrame",
+        "setTimeout",
+        "collapseToast",
+        "onEnter",
+        "onExited",
+        "onExit",
+        "eventManager",
+        "emitQueue",
+        "on",
+        "off",
+        "cb",
+        "cancelEmit",
+        "timers",
+        "timer",
+        "useToastContainer",
+        "toastIds",
+        "setToastIds",
+        "containerRef",
+        "toastToRender",
+        "isToastActive",
+        "toastKey",
+        "displayedToast",
+        "count",
+        "queue",
+        "containerId",
+        "getToast",
+        "appendToast",
+        "delay",
+        "staleId",
+        "isNotValid",
+        "updateId",
+        "closeToast",
+        "removeToast",
+        "isNotAnUpdate",
+        "toastAutoClose",
+        "containerAutoClose",
+        "toastProps",
+        "isLoading",
+        "theme",
+        "icon",
+        "closeButton",
+        "rtl",
+        "transition",
+        "className",
+        "bodyClassName",
+        "bodyStyle",
+        "pauseOnHover",
+        "pauseOnFocusLoss",
+        "draggable",
+        "draggablePercent",
+        "draggableDirection",
+        "closeOnClick",
+        "progressClassName",
+        "progressStyle",
+        "autoClose",
+        "hideProgressBar",
+        "progress",
+        "role",
+        "deleteToast",
+        "queueLen",
+        "freeSlot",
+        "dequeueToast",
+        "toDequeue",
+        "toastContent",
+        "cloneElement",
+        "getToastToRender",
+        "toRender",
+        "collection",
+        "toast",
+        "p",
+        "getX",
+        "getY",
+        "useToast",
+        "isRunning",
+        "setIsRunning",
+        "setPreventExitTransition",
+        "toastRef",
+        "drag",
+        "removalDistance",
+        "canCloseOnClick",
+        "canDrag",
+        "boundingRect",
+        "didMove",
+        "syncProps",
+        "top",
+        "bottom",
+        "left",
+        "right",
+        "pauseToast",
+        "playToast",
+        "once",
+        "bindFocusEvents",
+        "eventHandlers",
+        "onMouseDown",
+        "onTouchStart",
+        "onMouseUp",
+        "onTouchEnd",
+        "onDragTransitionEnd",
+        "CloseButton",
+        "ariaLabel",
+        "viewBox",
+        "fillRule",
+        "d",
+        "ProgressBar",
+        "hide",
+        "userStyle",
+        "controlledProgress",
+        "animationDuration",
+        "animationPlayState",
+        "opacity",
+        "defaultClassName",
+        "cx",
+        "classNames",
+        "animationEvent",
+        "Svg",
+        "width",
+        "height",
+        "fill",
+        "Icons",
+        "success",
+        "spinner",
+        "Toast",
+        "Transition",
+        "cssClasses",
+        "isProgressControlled",
+        "maybeIcon",
+        "iconProps",
+        "Icon",
+        "renderCloseButton",
+        "Bounce",
+        "ToastContainer",
+        "containerStyle",
+        "toastList",
+        "pointerEvents",
+        "getClassName",
+        "newestOnTop",
+        "containers",
+        "lazy",
+        "generateToastId",
+        "getToastId",
+        "dispatchToast",
+        "containerDomNode",
+        "mergeOptions",
+        "createToastByType",
+        "pending",
+        "resetParams",
+        "resolver",
+        "input",
+        "baseParams",
+        "container",
+        "oldOptions",
+        "oldContent",
+        "nextOptions",
+        "containerConfig",
+        "latestInstance",
+        "containerInstance",
+        "item",
         "Schema",
         "property",
         "normal",
         "space",
         "definitions",
         "own",
         "definition",
@@ -917,15 +1117,14 @@
         "ariaExpanded",
         "ariaFlowTo",
         "ariaGrabbed",
         "ariaHasPopup",
         "ariaHidden",
         "ariaInvalid",
         "ariaKeyShortcuts",
-        "ariaLabel",
         "ariaLabelledBy",
         "ariaLevel",
         "ariaLive",
         "ariaModal",
         "ariaMultiLine",
         "ariaMultiSelectable",
         "ariaOrientation",
@@ -943,15 +1142,14 @@
         "ariaSelected",
         "ariaSetSize",
         "ariaSort",
         "ariaValueMax",
         "ariaValueMin",
         "ariaValueNow",
         "ariaValueText",
-        "role",
         "html",
         "acceptcharset",
         "classname",
         "htmlfor",
         "httpequiv",
         "abbr",
         "accept",
@@ -968,15 +1166,14 @@
         "autoComplete",
         "autoFocus",
         "autoPlay",
         "capture",
         "charSet",
         "checked",
         "cite",
-        "className",
         "cols",
         "colSpan",
         "contentEditable",
         "controls",
         "controlsList",
         "coords",
         "crossOrigin",
@@ -984,21 +1181,19 @@
         "decoding",
         "default",
         "defer",
         "dir",
         "dirName",
         "disabled",
         "download",
-        "draggable",
         "encType",
         "enterKeyHint",
         "form",
         "formNoValidate",
         "formTarget",
-        "height",
         "hidden",
         "high",
         "hrefLang",
         "htmlFor",
         "httpEquiv",
         "imageSizes",
         "imageSrcSet",
@@ -1068,21 +1263,19 @@
         "onLoad",
         "onLoadedData",
         "onLoadedMetadata",
         "onLoadEnd",
         "onLoadStart",
         "onMessage",
         "onMessageError",
-        "onMouseDown",
         "onMouseEnter",
         "onMouseLeave",
         "onMouseMove",
         "onMouseOut",
         "onMouseOver",
-        "onMouseUp",
         "onOffline",
         "onOnline",
         "onPageHide",
         "onPageShow",
         "onPaste",
         "onPause",
         "onPlay",
@@ -1139,15 +1332,14 @@
         "srcSet",
         "step",
         "tabIndex",
         "title",
         "translate",
         "typeMustMatch",
         "useMap",
-        "width",
         "wrap",
         "align",
         "aLink",
         "archive",
         "axis",
         "background",
         "bgColor",
@@ -1213,15 +1405,14 @@
         "colorInterpolationFilters",
         "colorProfile",
         "colorRendering",
         "dataType",
         "dominantBaseline",
         "enableBackground",
         "fillOpacity",
-        "fillRule",
         "floodColor",
         "floodOpacity",
         "fontFamily",
         "fontSize",
         "fontSizeAdjust",
         "fontStretch",
         "fontVariant",
@@ -1257,15 +1448,14 @@
         "onRepeat",
         "onShow",
         "onZoom",
         "overlinePosition",
         "overlineThickness",
         "paintOrder",
         "panose1",
-        "pointerEvents",
         "renderingIntent",
         "shapeRendering",
         "stopColor",
         "stopOpacity",
         "strikethroughPosition",
         "strikethroughThickness",
         "strokeDashArray",
@@ -1315,32 +1505,29 @@
         "by",
         "calcMode",
         "clip",
         "clipPathUnits",
         "contentScriptType",
         "contentStyleType",
         "cursor",
-        "cx",
         "cy",
-        "d",
         "defaultAction",
         "descent",
         "diffuseConstant",
         "direction",
         "display",
         "dur",
         "divisor",
         "dx",
         "dy",
         "edgeMode",
         "editable",
         "elevation",
         "exponent",
         "externalResourcesRequired",
-        "fill",
         "filterRes",
         "filterUnits",
         "focusable",
         "focusHighlight",
         "format",
         "fr",
         "fx",
@@ -1354,15 +1541,14 @@
         "hatchContentUnits",
         "hatchUnits",
         "ideographic",
         "initialVisibility",
         "in",
         "in2",
         "intercept",
-        "k",
         "k1",
         "k2",
         "k3",
         "k4",
         "kernelMatrix",
         "kernelUnitLength",
         "keyPoints",
@@ -1383,15 +1569,14 @@
         "mediaContentEncodings",
         "mediaSize",
         "mediaTime",
         "mode",
         "numOctaves",
         "observer",
         "offset",
-        "opacity",
         "operator",
         "order",
         "orient",
         "orientation",
         "origin",
         "overflow",
         "overlay",
@@ -1451,212 +1636,27 @@
         "targetY",
         "textLength",
         "transformBehavior",
         "u1",
         "u2",
         "unicode",
         "values",
-        "viewBox",
         "viewTarget",
         "visibility",
         "widths",
         "x1",
         "x2",
         "xChannelSelector",
         "y1",
         "y2",
         "yChannelSelector",
         "z",
         "zoomAndPan",
         "htmlBase",
         "svgBase",
-        "toVal",
-        "mix",
-        "tmp",
-        "isNum",
-        "isNaN",
-        "isBool",
-        "isStr",
-        "isFn",
-        "parseClassName",
-        "isToastIdValid",
-        "toastId",
-        "canUseDom",
-        "canBeRendered",
-        "isValidElement",
-        "POSITION",
-        "TOP_LEFT",
-        "TOP_RIGHT",
-        "TOP_CENTER",
-        "BOTTOM_LEFT",
-        "BOTTOM_RIGHT",
-        "BOTTOM_CENTER",
-        "TYPE",
-        "INFO",
-        "SUCCESS",
-        "WARNING",
-        "ERROR",
-        "DEFAULT",
-        "cssTransition",
-        "appendPosition",
-        "collapse",
-        "collapseDuration",
-        "preventExitTransition",
-        "nodeRef",
-        "isIn",
-        "enterClassName",
-        "exitClassName",
-        "baseClassName",
-        "animationStep",
-        "node",
-        "Event",
-        "duration",
-        "scrollHeight",
-        "requestAnimationFrame",
-        "setTimeout",
-        "collapseToast",
-        "onEnter",
-        "onExited",
-        "onExit",
-        "eventManager",
-        "emitQueue",
-        "on",
-        "off",
-        "cb",
-        "cancelEmit",
-        "timers",
-        "timer",
-        "useToastContainer",
-        "toastIds",
-        "setToastIds",
-        "containerRef",
-        "toastToRender",
-        "isToastActive",
-        "toastKey",
-        "displayedToast",
-        "count",
-        "queue",
-        "containerId",
-        "getToast",
-        "appendToast",
-        "delay",
-        "staleId",
-        "isNotValid",
-        "updateId",
-        "closeToast",
-        "removeToast",
-        "isNotAnUpdate",
-        "toastAutoClose",
-        "containerAutoClose",
-        "toastProps",
-        "isLoading",
-        "theme",
-        "icon",
-        "closeButton",
-        "rtl",
-        "transition",
-        "bodyClassName",
-        "bodyStyle",
-        "pauseOnHover",
-        "pauseOnFocusLoss",
-        "draggablePercent",
-        "draggableDirection",
-        "closeOnClick",
-        "progressClassName",
-        "progressStyle",
-        "autoClose",
-        "hideProgressBar",
-        "progress",
-        "deleteToast",
-        "queueLen",
-        "freeSlot",
-        "dequeueToast",
-        "toDequeue",
-        "toastContent",
-        "cloneElement",
-        "getToastToRender",
-        "toRender",
-        "collection",
-        "toast",
-        "p",
-        "getX",
-        "getY",
-        "useToast",
-        "isRunning",
-        "setIsRunning",
-        "setPreventExitTransition",
-        "toastRef",
-        "drag",
-        "removalDistance",
-        "canCloseOnClick",
-        "canDrag",
-        "boundingRect",
-        "didMove",
-        "syncProps",
-        "top",
-        "bottom",
-        "left",
-        "right",
-        "pauseToast",
-        "playToast",
-        "once",
-        "bindFocusEvents",
-        "eventHandlers",
-        "onTouchStart",
-        "onTouchEnd",
-        "onDragTransitionEnd",
-        "CloseButton",
-        "ProgressBar",
-        "hide",
-        "userStyle",
-        "controlledProgress",
-        "animationDuration",
-        "animationPlayState",
-        "defaultClassName",
-        "classNames",
-        "animationEvent",
-        "Svg",
-        "Icons",
-        "success",
-        "spinner",
-        "Toast",
-        "Transition",
-        "cssClasses",
-        "isProgressControlled",
-        "maybeIcon",
-        "iconProps",
-        "Icon",
-        "renderCloseButton",
-        "Bounce",
-        "ToastContainer",
-        "containerStyle",
-        "toastList",
-        "getClassName",
-        "newestOnTop",
-        "containers",
-        "lazy",
-        "generateToastId",
-        "getToastId",
-        "dispatchToast",
-        "containerDomNode",
-        "mergeOptions",
-        "createToastByType",
-        "pending",
-        "resetParams",
-        "resolver",
-        "input",
-        "baseParams",
-        "container",
-        "oldOptions",
-        "oldContent",
-        "nextOptions",
-        "containerConfig",
-        "latestInstance",
-        "containerInstance",
-        "item",
         "normalizeIdentifier",
         "_defineProperties",
         "_createClass",
         "protoProps",
         "staticProps",
         "die",
         "msg",
@@ -5497,17 +5497,14 @@
         "nestedNoscriptInHead",
         "eofInElementThatCanContainOnlyText",
         "ErrorReportingMixinBase",
         "onParseError",
         "_setErrorLocation",
         "mxn",
         "_reportError",
-        "v1",
-        "v4",
-        "uuid",
         "FilePond",
         "FileStatus",
         "registerPlugin",
         "_react",
         "_react2",
         "_filepond",
         "isSupported",
@@ -5653,14 +5650,17 @@
         "_attachCurrentAttrLocationInfo",
         "modeName",
         "prevPos",
         "reduction",
         "superPropBase",
         "_get",
         "receiver",
+        "v1",
+        "v4",
+        "uuid",
         "isJPEG",
         "Marker",
         "JPEG",
         "APP1",
         "EXIF",
         "TIFF",
         "Orientation",
@@ -11515,26 +11515,14 @@
         "../node_modules/babel-preset-react-app/node_modules/@babel/runtime/helpers/esm/nonIterableSpread.js",
         "../node_modules/react-markdown/node_modules/prop-types/index.js",
         "../node_modules/axios/lib/core/AxiosError.js",
         "../node_modules/micromark-util-chunked/index.js",
         "../node_modules/babel-preset-react-app/node_modules/@babel/runtime/helpers/esm/classCallCheck.js",
         "../../dom.ts",
         "../../index.tsx",
-        "../node_modules/property-information/lib/util/schema.js",
-        "../node_modules/property-information/lib/util/merge.js",
-        "../node_modules/property-information/lib/util/create.js",
-        "../node_modules/property-information/lib/xlink.js",
-        "../node_modules/property-information/lib/xml.js",
-        "../node_modules/property-information/lib/util/case-sensitive-transform.js",
-        "../node_modules/property-information/lib/util/case-insensitive-transform.js",
-        "../node_modules/property-information/lib/xmlns.js",
-        "../node_modules/property-information/lib/aria.js",
-        "../node_modules/property-information/lib/html.js",
-        "../node_modules/property-information/lib/svg.js",
-        "../node_modules/property-information/index.js",
         "../node_modules/clsx/dist/clsx.m.js",
         "../../src/utils/propValidator.ts",
         "../../src/utils/constant.ts",
         "../../src/utils/cssTransition.tsx",
         "../../src/utils/collapseToast.ts",
         "../../src/core/eventManager.ts",
         "../../src/hooks/useToastContainer.ts",
@@ -11542,14 +11530,26 @@
         "../../src/components/CloseButton.tsx",
         "../../src/components/ProgressBar.tsx",
         "../../src/components/Icons.tsx",
         "../../src/components/Toast.tsx",
         "../../src/components/Transitions.tsx",
         "../../src/components/ToastContainer.tsx",
         "../../src/core/toast.tsx",
+        "../node_modules/property-information/lib/util/schema.js",
+        "../node_modules/property-information/lib/util/merge.js",
+        "../node_modules/property-information/lib/util/create.js",
+        "../node_modules/property-information/lib/xlink.js",
+        "../node_modules/property-information/lib/xml.js",
+        "../node_modules/property-information/lib/util/case-sensitive-transform.js",
+        "../node_modules/property-information/lib/util/case-insensitive-transform.js",
+        "../node_modules/property-information/lib/xmlns.js",
+        "../node_modules/property-information/lib/aria.js",
+        "../node_modules/property-information/lib/html.js",
+        "../node_modules/property-information/lib/svg.js",
+        "../node_modules/property-information/index.js",
         "../node_modules/micromark-util-normalize-identifier/index.js",
         "../node_modules/babel-preset-react-app/node_modules/@babel/runtime/helpers/esm/createClass.js",
         "../../src/utils/errors.ts",
         "../../src/utils/common.ts",
         "../../src/utils/plugins.ts",
         "../../src/core/scope.ts",
         "../../src/core/finalize.ts",
@@ -11692,15 +11692,14 @@
         "../node_modules/react-range/lib/types.js",
         "../node_modules/lodash/_Symbol.js",
         "../node_modules/babel-preset-react-app/node_modules/@babel/runtime/helpers/unsupportedIterableToArray.js",
         "../node_modules/babel-preset-react-app/node_modules/@babel/runtime/helpers/setPrototypeOf.js",
         "../node_modules/parse5/lib/common/unicode.js",
         "../node_modules/parse5/lib/common/error-codes.js",
         "../node_modules/parse5/lib/extensions/error-reporting/mixin-base.js",
-        "../node_modules/uuid/index.js",
         "../node_modules/react-filepond/dist/react-filepond.js",
         "../node_modules/extend/index.js",
         "../node_modules/uuid/lib/rng-browser.js",
         "../node_modules/uuid/lib/bytesToUuid.js",
         "../node_modules/react-range/lib/utils.js",
         "../node_modules/@babel/runtime/helpers/unsupportedIterableToArray.js",
         "../node_modules/@babel/runtime/helpers/arrayLikeToArray.js",
@@ -11717,14 +11716,15 @@
         "../node_modules/babel-preset-react-app/node_modules/@babel/runtime/helpers/arrayLikeToArray.js",
         "../node_modules/babel-preset-react-app/node_modules/@babel/runtime/helpers/isNativeReflectConstruct.js",
         "../node_modules/babel-preset-react-app/node_modules/@babel/runtime/helpers/slicedToArray.js",
         "../node_modules/parse5/lib/extensions/location-info/tokenizer-mixin.js",
         "../node_modules/parse5/lib/extensions/position-tracking/preprocessor-mixin.js",
         "../node_modules/babel-preset-react-app/node_modules/@babel/runtime/helpers/get.js",
         "../node_modules/react-redux/node_modules/react-is/index.js",
+        "../node_modules/uuid/index.js",
         "../node_modules/filepond-plugin-image-exif-orientation/dist/filepond-plugin-image-exif-orientation.js",
         "../node_modules/filepond-plugin-image-preview/dist/filepond-plugin-image-preview.js",
         "../node_modules/filepond-plugin-file-validate-size/dist/filepond-plugin-file-validate-size.js",
         "../node_modules/unified/node_modules/is-buffer/index.js",
         "../node_modules/vfile/node_modules/is-buffer/index.js",
         "../node_modules/react-markdown/node_modules/react-is/index.js",
         "../node_modules/highlight.js/lib/languages/arduino.js",
@@ -12160,26 +12160,14 @@
         "export default function _nonIterableSpread() {\n  throw new TypeError(\"Invalid attempt to spread non-iterable instance.\\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.\");\n}",
         "/**\n * Copyright (c) 2013-present, Facebook, Inc.\n *\n * This source code is licensed under the MIT license found in the\n * LICENSE file in the root directory of this source tree.\n */\n\nif (process.env.NODE_ENV !== 'production') {\n  var ReactIs = require('react-is');\n\n  // By explicitly using `prop-types` you are opting into new development behavior.\n  // http://fb.me/prop-types-in-prod\n  var throwOnDirectAccess = true;\n  module.exports = require('./factoryWithTypeCheckers')(ReactIs.isElement, throwOnDirectAccess);\n} else {\n  // By explicitly using `prop-types` you are opting into new production behavior.\n  // http://fb.me/prop-types-in-prod\n  module.exports = require('./factoryWithThrowingShims')();\n}\n",
         "'use strict';\n\nimport utils from '../utils.js';\n\n/**\n * Create an Error with the specified message, config, error code, request and response.\n *\n * @param {string} message The error message.\n * @param {string} [code] The error code (for example, 'ECONNABORTED').\n * @param {Object} [config] The config.\n * @param {Object} [request] The request.\n * @param {Object} [response] The response.\n *\n * @returns {Error} The created error.\n */\nfunction AxiosError(message, code, config, request, response) {\n  Error.call(this);\n\n  if (Error.captureStackTrace) {\n    Error.captureStackTrace(this, this.constructor);\n  } else {\n    this.stack = (new Error()).stack;\n  }\n\n  this.message = message;\n  this.name = 'AxiosError';\n  code && (this.code = code);\n  config && (this.config = config);\n  request && (this.request = request);\n  response && (this.response = response);\n}\n\nutils.inherits(AxiosError, Error, {\n  toJSON: function toJSON() {\n    return {\n      // Standard\n      message: this.message,\n      name: this.name,\n      // Microsoft\n      description: this.description,\n      number: this.number,\n      // Mozilla\n      fileName: this.fileName,\n      lineNumber: this.lineNumber,\n      columnNumber: this.columnNumber,\n      stack: this.stack,\n      // Axios\n      config: utils.toJSONObject(this.config),\n      code: this.code,\n      status: this.response && this.response.status ? this.response.status : null\n    };\n  }\n});\n\nconst prototype = AxiosError.prototype;\nconst descriptors = {};\n\n[\n  'ERR_BAD_OPTION_VALUE',\n  'ERR_BAD_OPTION',\n  'ECONNABORTED',\n  'ETIMEDOUT',\n  'ERR_NETWORK',\n  'ERR_FR_TOO_MANY_REDIRECTS',\n  'ERR_DEPRECATED',\n  'ERR_BAD_RESPONSE',\n  'ERR_BAD_REQUEST',\n  'ERR_CANCELED',\n  'ERR_NOT_SUPPORT',\n  'ERR_INVALID_URL'\n// eslint-disable-next-line func-names\n].forEach(code => {\n  descriptors[code] = {value: code};\n});\n\nObject.defineProperties(AxiosError, descriptors);\nObject.defineProperty(prototype, 'isAxiosError', {value: true});\n\n// eslint-disable-next-line func-names\nAxiosError.from = (error, code, config, request, response, customProps) => {\n  const axiosError = Object.create(prototype);\n\n  utils.toFlatObject(error, axiosError, function filter(obj) {\n    return obj !== Error.prototype;\n  }, prop => {\n    return prop !== 'isAxiosError';\n  });\n\n  AxiosError.call(axiosError, error.message, code, config, request, response);\n\n  axiosError.cause = error;\n\n  axiosError.name = error.name;\n\n  customProps && Object.assign(axiosError, customProps);\n\n  return axiosError;\n};\n\nexport default AxiosError;\n",
         "/**\n * Like `Array#splice`, but smarter for giant arrays.\n *\n * `Array#splice` takes all items to be inserted as individual argument which\n * causes a stack overflow in V8 when trying to insert 100k items for instance.\n *\n * Otherwise, this does not return the removed items, and takes `items` as an\n * array instead of rest parameters.\n *\n * @template {unknown} T\n * @param {T[]} list\n * @param {number} start\n * @param {number} remove\n * @param {T[]} items\n * @returns {void}\n */\nexport function splice(list, start, remove, items) {\n  const end = list.length\n  let chunkStart = 0\n  /** @type {unknown[]} */\n\n  let parameters // Make start between zero and `end` (included).\n\n  if (start < 0) {\n    start = -start > end ? 0 : end + start\n  } else {\n    start = start > end ? end : start\n  }\n\n  remove = remove > 0 ? remove : 0 // No need to chunk the items if there\u2019s only a couple (10k) items.\n\n  if (items.length < 10000) {\n    parameters = Array.from(items)\n    parameters.unshift(start, remove) // @ts-expect-error Hush, it\u2019s fine.\n    ;[].splice.apply(list, parameters)\n  } else {\n    // Delete `remove` items starting from `start`\n    if (remove) [].splice.apply(list, [start, remove]) // Insert the items in chunks to not cause stack overflows.\n\n    while (chunkStart < items.length) {\n      parameters = items.slice(chunkStart, chunkStart + 10000)\n      parameters.unshift(start, 0) // @ts-expect-error Hush, it\u2019s fine.\n      ;[].splice.apply(list, parameters)\n      chunkStart += 10000\n      start += 10000\n    }\n  }\n}\n/**\n * Append `items` (an array) at the end of `list` (another array).\n * When `list` was empty, returns `items` instead.\n *\n * This prevents a potentially expensive operation when `list` is empty,\n * and adds items in batches to prevent V8 from hanging.\n *\n * @template {unknown} T\n * @param {T[]} list\n * @param {T[]} items\n * @returns {T[]}\n */\n\nexport function push(list, items) {\n  if (list.length > 0) {\n    splice(list, list.length, 0, items)\n    return list\n  }\n\n  return items\n}\n",
         "export default function _classCallCheck(instance, Constructor) {\n  if (!(instance instanceof Constructor)) {\n    throw new TypeError(\"Cannot call a class as a function\");\n  }\n}",
         "import type { FormEncType, FormMethod } from \"@remix-run/router\";\nimport type { RelativeRoutingType } from \"react-router\";\n\nexport const defaultMethod = \"get\";\nconst defaultEncType = \"application/x-www-form-urlencoded\";\n\nexport function isHtmlElement(object: any): object is HTMLElement {\n  return object != null && typeof object.tagName === \"string\";\n}\n\nexport function isButtonElement(object: any): object is HTMLButtonElement {\n  return isHtmlElement(object) && object.tagName.toLowerCase() === \"button\";\n}\n\nexport function isFormElement(object: any): object is HTMLFormElement {\n  return isHtmlElement(object) && object.tagName.toLowerCase() === \"form\";\n}\n\nexport function isInputElement(object: any): object is HTMLInputElement {\n  return isHtmlElement(object) && object.tagName.toLowerCase() === \"input\";\n}\n\ntype LimitedMouseEvent = Pick<\n  MouseEvent,\n  \"button\" | \"metaKey\" | \"altKey\" | \"ctrlKey\" | \"shiftKey\"\n>;\n\nfunction isModifiedEvent(event: LimitedMouseEvent) {\n  return !!(event.metaKey || event.altKey || event.ctrlKey || event.shiftKey);\n}\n\nexport function shouldProcessLinkClick(\n  event: LimitedMouseEvent,\n  target?: string\n) {\n  return (\n    event.button === 0 && // Ignore everything but left clicks\n    (!target || target === \"_self\") && // Let browser handle \"target=_blank\" etc.\n    !isModifiedEvent(event) // Ignore clicks with modifier keys\n  );\n}\n\nexport type ParamKeyValuePair = [string, string];\n\nexport type URLSearchParamsInit =\n  | string\n  | ParamKeyValuePair[]\n  | Record<string, string | string[]>\n  | URLSearchParams;\n\n/**\n * Creates a URLSearchParams object using the given initializer.\n *\n * This is identical to `new URLSearchParams(init)` except it also\n * supports arrays as values in the object form of the initializer\n * instead of just strings. This is convenient when you need multiple\n * values for a given key, but don't want to use an array initializer.\n *\n * For example, instead of:\n *\n *   let searchParams = new URLSearchParams([\n *     ['sort', 'name'],\n *     ['sort', 'price']\n *   ]);\n *\n * you can do:\n *\n *   let searchParams = createSearchParams({\n *     sort: ['name', 'price']\n *   });\n */\nexport function createSearchParams(\n  init: URLSearchParamsInit = \"\"\n): URLSearchParams {\n  return new URLSearchParams(\n    typeof init === \"string\" ||\n    Array.isArray(init) ||\n    init instanceof URLSearchParams\n      ? init\n      : Object.keys(init).reduce((memo, key) => {\n          let value = init[key];\n          return memo.concat(\n            Array.isArray(value) ? value.map((v) => [key, v]) : [[key, value]]\n          );\n        }, [] as ParamKeyValuePair[])\n  );\n}\n\nexport function getSearchParamsForLocation(\n  locationSearch: string,\n  defaultSearchParams: URLSearchParams | null\n) {\n  let searchParams = createSearchParams(locationSearch);\n\n  if (defaultSearchParams) {\n    for (let key of defaultSearchParams.keys()) {\n      if (!searchParams.has(key)) {\n        defaultSearchParams.getAll(key).forEach((value) => {\n          searchParams.append(key, value);\n        });\n      }\n    }\n  }\n\n  return searchParams;\n}\n\nexport interface SubmitOptions {\n  /**\n   * The HTTP method used to submit the form. Overrides `<form method>`.\n   * Defaults to \"GET\".\n   */\n  method?: FormMethod;\n\n  /**\n   * The action URL path used to submit the form. Overrides `<form action>`.\n   * Defaults to the path of the current route.\n   *\n   * Note: It is assumed the path is already resolved. If you need to resolve a\n   * relative path, use `useFormAction`.\n   */\n  action?: string;\n\n  /**\n   * The action URL used to submit the form. Overrides `<form encType>`.\n   * Defaults to \"application/x-www-form-urlencoded\".\n   */\n  encType?: FormEncType;\n\n  /**\n   * Set `true` to replace the current entry in the browser's history stack\n   * instead of creating a new one (i.e. stay on \"the same page\"). Defaults\n   * to `false`.\n   */\n  replace?: boolean;\n\n  /**\n   * Determines whether the form action is relative to the route hierarchy or\n   * the pathname.  Use this if you want to opt out of navigating the route\n   * hierarchy and want to instead route based on /-delimited URL segments\n   */\n  relative?: RelativeRoutingType;\n\n  /**\n   * In browser-based environments, prevent resetting scroll after this\n   * navigation when using the <ScrollRestoration> component\n   */\n  preventScrollReset?: boolean;\n}\n\nexport function getFormSubmissionInfo(\n  target:\n    | HTMLFormElement\n    | HTMLButtonElement\n    | HTMLInputElement\n    | FormData\n    | URLSearchParams\n    | { [name: string]: string }\n    | null,\n  defaultAction: string,\n  options: SubmitOptions\n): {\n  url: URL;\n  method: string;\n  encType: string;\n  formData: FormData;\n} {\n  let method: string;\n  let action: string;\n  let encType: string;\n  let formData: FormData;\n\n  if (isFormElement(target)) {\n    let submissionTrigger: HTMLButtonElement | HTMLInputElement = (\n      options as any\n    ).submissionTrigger;\n\n    method = options.method || target.getAttribute(\"method\") || defaultMethod;\n    action = options.action || target.getAttribute(\"action\") || defaultAction;\n    encType =\n      options.encType || target.getAttribute(\"enctype\") || defaultEncType;\n\n    formData = new FormData(target);\n\n    if (submissionTrigger && submissionTrigger.name) {\n      formData.append(submissionTrigger.name, submissionTrigger.value);\n    }\n  } else if (\n    isButtonElement(target) ||\n    (isInputElement(target) &&\n      (target.type === \"submit\" || target.type === \"image\"))\n  ) {\n    let form = target.form;\n\n    if (form == null) {\n      throw new Error(\n        `Cannot submit a <button> or <input type=\"submit\"> without a <form>`\n      );\n    }\n\n    // <button>/<input type=\"submit\"> may override attributes of <form>\n\n    method =\n      options.method ||\n      target.getAttribute(\"formmethod\") ||\n      form.getAttribute(\"method\") ||\n      defaultMethod;\n    action =\n      options.action ||\n      target.getAttribute(\"formaction\") ||\n      form.getAttribute(\"action\") ||\n      defaultAction;\n    encType =\n      options.encType ||\n      target.getAttribute(\"formenctype\") ||\n      form.getAttribute(\"enctype\") ||\n      defaultEncType;\n\n    formData = new FormData(form);\n\n    // Include name + value from a <button>, appending in case the button name\n    // matches an existing input name\n    if (target.name) {\n      formData.append(target.name, target.value);\n    }\n  } else if (isHtmlElement(target)) {\n    throw new Error(\n      `Cannot submit element that is not <form>, <button>, or ` +\n        `<input type=\"submit|image\">`\n    );\n  } else {\n    method = options.method || defaultMethod;\n    action = options.action || defaultAction;\n    encType = options.encType || defaultEncType;\n\n    if (target instanceof FormData) {\n      formData = target;\n    } else {\n      formData = new FormData();\n\n      if (target instanceof URLSearchParams) {\n        for (let [name, value] of target) {\n          formData.append(name, value);\n        }\n      } else if (target != null) {\n        for (let name of Object.keys(target)) {\n          formData.append(name, target[name]);\n        }\n      }\n    }\n  }\n\n  let { protocol, host } = window.location;\n  let url = new URL(action, `${protocol}//${host}`);\n\n  return { url, method: method.toLowerCase(), encType, formData };\n}\n",
-        "/**\n * @typedef {import('./info.js').Info} Info\n * @typedef {Record<string, Info>} Properties\n * @typedef {Record<string, string>} Normal\n */\n\nexport class Schema {\n  /**\n   * @constructor\n   * @param {Properties} property\n   * @param {Normal} normal\n   * @param {string} [space]\n   */\n  constructor(property, normal, space) {\n    this.property = property\n    this.normal = normal\n    if (space) {\n      this.space = space\n    }\n  }\n}\n\n/** @type {Properties} */\nSchema.prototype.property = {}\n/** @type {Normal} */\nSchema.prototype.normal = {}\n/** @type {string|null} */\nSchema.prototype.space = null\n",
-        "/**\n * @typedef {import('./schema.js').Properties} Properties\n * @typedef {import('./schema.js').Normal} Normal\n */\n\nimport {Schema} from './schema.js'\n\n/**\n * @param {Schema[]} definitions\n * @param {string} [space]\n * @returns {Schema}\n */\nexport function merge(definitions, space) {\n  /** @type {Properties} */\n  const property = {}\n  /** @type {Normal} */\n  const normal = {}\n  let index = -1\n\n  while (++index < definitions.length) {\n    Object.assign(property, definitions[index].property)\n    Object.assign(normal, definitions[index].normal)\n  }\n\n  return new Schema(property, normal, space)\n}\n",
-        "import {create} from './util/create.js'\n\nexport const xlink = create({\n  space: 'xlink',\n  transform(_, prop) {\n    return 'xlink:' + prop.slice(5).toLowerCase()\n  },\n  properties: {\n    xLinkActuate: null,\n    xLinkArcRole: null,\n    xLinkHref: null,\n    xLinkRole: null,\n    xLinkShow: null,\n    xLinkTitle: null,\n    xLinkType: null\n  }\n})\n",
-        "import {create} from './util/create.js'\n\nexport const xml = create({\n  space: 'xml',\n  transform(_, prop) {\n    return 'xml:' + prop.slice(3).toLowerCase()\n  },\n  properties: {xmlLang: null, xmlBase: null, xmlSpace: null}\n})\n",
-        "/**\n * @param {Record<string, string>} attributes\n * @param {string} attribute\n * @returns {string}\n */\nexport function caseSensitiveTransform(attributes, attribute) {\n  return attribute in attributes ? attributes[attribute] : attribute\n}\n",