# Comparing `tmp/certego_saas-0.5.0.tar.gz` & `tmp/certego_saas-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certego_saas-0.5.0.tar", last modified: Wed Mar 29 09:24:00 2023, max compression
+gzip compressed data, was "certego_saas-0.6.0.tar", last modified: Tue May 23 13:10:09 2023, max compression
```

## Comparing `certego_saas-0.5.0.tar` & `certego_saas-0.6.0.tar`

### file list

```diff
@@ -1,179 +1,179 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:24:00.007206 certego_saas-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-29 09:23:50.000000 certego_saas-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-29 09:23:50.000000 certego_saas-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-03-29 09:24:00.007206 certego_saas-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-03-29 09:23:50.000000 certego_saas-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:59.991205 certego_saas-0.5.0/certego_saas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:59.995205 certego_saas-0.5.0/certego_saas/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:59.995205 certego_saas-0.5.0/certego_saas/apps/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/auth/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/auth/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/auth/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/auth/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:59.995205 certego_saas-0.5.0/certego_saas/apps/feedback/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/feedback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/feedback/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/feedback/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:59.995205 certego_saas-0.5.0/certego_saas/apps/feedback/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/feedback/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/feedback/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/feedback/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/feedback/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/feedback/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/feedback/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:59.995205 certego_saas-0.5.0/certego_saas/apps/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/notifications/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/notifications/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/notifications/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:59.995205 certego_saas-0.5.0/certego_saas/apps/notifications/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/notifications/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:59.995205 certego_saas-0.5.0/certego_saas/apps/notifications/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/notifications/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/notifications/management/commands/changelog_notification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:59.995205 certego_saas-0.5.0/certego_saas/apps/notifications/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/notifications/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/notifications/migrations/0002_alter_notification_appname.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/notifications/migrations/0003_for_user.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/notifications/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/notifications/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/notifications/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/notifications/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/notifications/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:59.999205 certego_saas-0.5.0/certego_saas/apps/organization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/organization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/organization/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/organization/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/organization/invitation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/organization/membership.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:59.999205 certego_saas-0.5.0/certego_saas/apps/organization/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/organization/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/organization/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/organization/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/organization/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/organization/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/organization/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/organization/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/organization/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/organization/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:59.999205 certego_saas-0.5.0/certego_saas/apps/payments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/payments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/payments/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/payments/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/payments/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/payments/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/payments/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:59.999205 certego_saas-0.5.0/certego_saas/apps/payments/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/payments/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/payments/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10336 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/payments/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/payments/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/payments/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/payments/throttling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/payments/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:59.999205 certego_saas-0.5.0/certego_saas/apps/user/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/user/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/user/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/user/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:59.999205 certego_saas-0.5.0/certego_saas/apps/user/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/user/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/user/migrations/0002_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/user/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/user/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/user/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/user/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps/user/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:24:00.003205 certego_saas-0.5.0/certego_saas/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/ext/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/ext/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/ext/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/ext/managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/ext/middlewares.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/ext/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/ext/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/ext/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/ext/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:24:00.003205 certego_saas-0.5.0/certego_saas/ext/test_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/ext/test_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/ext/test_utilities/no_logs_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/ext/test_utilities/timed_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/ext/throttling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:24:00.003205 certego_saas-0.5.0/certego_saas/ext/upload/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/ext/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/ext/upload/elastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/ext/upload/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/ext/upload/twitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/ext/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/ext/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:24:00.003205 certego_saas-0.5.0/certego_saas/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:24:00.003205 certego_saas-0.5.0/certego_saas/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/management/commands/celery.py
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/management/commands/duplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/management/commands/queues.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:24:00.003205 certego_saas-0.5.0/certego_saas/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:59.991205 certego_saas-0.5.0/certego_saas/templates/certego_saas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:24:00.003205 certego_saas-0.5.0/certego_saas/templates/certego_saas/emails/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/templates/certego_saas/emails/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/templates/certego_saas/emails/certego-logo-positive.png
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/templates/certego_saas/emails/org-invitation.html
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/templates/context_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-29 09:23:50.000000 certego_saas-0.5.0/certego_saas/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:59.995205 certego_saas-0.5.0/certego_saas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-03-29 09:23:59.000000 certego_saas-0.5.0/certego_saas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-03-29 09:23:59.000000 certego_saas-0.5.0/certego_saas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 09:23:59.000000 certego_saas-0.5.0/certego_saas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-03-29 09:23:59.000000 certego_saas-0.5.0/certego_saas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-29 09:23:59.000000 certego_saas-0.5.0/certego_saas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-03-29 09:23:50.000000 certego_saas-0.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:24:00.003205 certego_saas-0.5.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-29 09:23:50.000000 certego_saas-0.5.0/requirements/requirements.dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-03-29 09:23:50.000000 certego_saas-0.5.0/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 09:24:00.007206 certego_saas-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-03-29 09:23:50.000000 certego_saas-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:24:00.003205 certego_saas-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-03-29 09:23:50.000000 certego_saas-0.5.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:24:00.003205 certego_saas-0.5.0/tests/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:50.000000 certego_saas-0.5.0/tests/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:24:00.003205 certego_saas-0.5.0/tests/apps/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:50.000000 certego_saas-0.5.0/tests/apps/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-03-29 09:23:50.000000 certego_saas-0.5.0/tests/apps/auth/test_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:24:00.003205 certego_saas-0.5.0/tests/apps/feedback/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:50.000000 certego_saas-0.5.0/tests/apps/feedback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-03-29 09:23:50.000000 certego_saas-0.5.0/tests/apps/feedback/test_feedback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:24:00.003205 certego_saas-0.5.0/tests/apps/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:50.000000 certego_saas-0.5.0/tests/apps/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-03-29 09:23:50.000000 certego_saas-0.5.0/tests/apps/notifications/test_notifications.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:24:00.003205 certego_saas-0.5.0/tests/apps/organization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:50.000000 certego_saas-0.5.0/tests/apps/organization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-03-29 09:23:50.000000 certego_saas-0.5.0/tests/apps/organization/test_invitation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-03-29 09:23:50.000000 certego_saas-0.5.0/tests/apps/organization/test_organization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:24:00.003205 certego_saas-0.5.0/tests/apps/payments/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-03-29 09:23:50.000000 certego_saas-0.5.0/tests/apps/payments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-03-29 09:23:50.000000 certego_saas-0.5.0/tests/apps/payments/test_payments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:24:00.003205 certego_saas-0.5.0/tests/apps/user/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:50.000000 certego_saas-0.5.0/tests/apps/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-03-29 09:23:50.000000 certego_saas-0.5.0/tests/apps/user/test_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:24:00.003205 certego_saas-0.5.0/tests/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:50.000000 certego_saas-0.5.0/tests/ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:24:00.003205 certego_saas-0.5.0/tests/ext/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:50.000000 certego_saas-0.5.0/tests/ext/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-03-29 09:23:50.000000 certego_saas-0.5.0/tests/ext/upload/test_slack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:24:00.003205 certego_saas-0.5.0/tests/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:50.000000 certego_saas-0.5.0/tests/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 09:24:00.007206 certego_saas-0.5.0/tests/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:50.000000 certego_saas-0.5.0/tests/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:50.000000 certego_saas-0.5.0/tests/management/commands/test_celery.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 09:23:50.000000 certego_saas-0.5.0/tests/management/commands/test_duplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-29 09:23:50.000000 certego_saas-0.5.0/tests/management/commands/test_queues.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.676961 certego_saas-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-23 13:09:58.000000 certego_saas-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-23 13:09:58.000000 certego_saas-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-23 13:10:09.676961 certego_saas-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-23 13:09:58.000000 certego_saas-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.664960 certego_saas-0.6.0/certego_saas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.664960 certego_saas-0.6.0/certego_saas/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.668961 certego_saas-0.6.0/certego_saas/apps/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/auth/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/auth/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/auth/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/auth/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.668961 certego_saas-0.6.0/certego_saas/apps/feedback/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/feedback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/feedback/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/feedback/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.668961 certego_saas-0.6.0/certego_saas/apps/feedback/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/feedback/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/feedback/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/feedback/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/feedback/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/feedback/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/feedback/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.668961 certego_saas-0.6.0/certego_saas/apps/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/notifications/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/notifications/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/notifications/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.668961 certego_saas-0.6.0/certego_saas/apps/notifications/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/notifications/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.668961 certego_saas-0.6.0/certego_saas/apps/notifications/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/notifications/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/notifications/management/commands/changelog_notification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.668961 certego_saas-0.6.0/certego_saas/apps/notifications/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/notifications/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/notifications/migrations/0002_alter_notification_appname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/notifications/migrations/0003_for_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/notifications/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/notifications/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/notifications/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/notifications/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/notifications/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.668961 certego_saas-0.6.0/certego_saas/apps/organization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/organization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/organization/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/organization/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/organization/invitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/organization/membership.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.668961 certego_saas-0.6.0/certego_saas/apps/organization/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/organization/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/organization/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/organization/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/organization/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/organization/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/organization/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/organization/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/organization/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/organization/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.672961 certego_saas-0.6.0/certego_saas/apps/payments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/payments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/payments/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/payments/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/payments/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/payments/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/payments/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.672961 certego_saas-0.6.0/certego_saas/apps/payments/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/payments/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/payments/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10336 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/payments/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/payments/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/payments/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/payments/throttling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/payments/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.672961 certego_saas-0.6.0/certego_saas/apps/user/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/user/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/user/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/user/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.672961 certego_saas-0.6.0/certego_saas/apps/user/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/user/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/user/migrations/0002_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/user/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/user/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/user/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/user/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps/user/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.672961 certego_saas-0.6.0/certego_saas/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/ext/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/ext/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/ext/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/ext/managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/ext/middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/ext/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/ext/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/ext/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/ext/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.672961 certego_saas-0.6.0/certego_saas/ext/test_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/ext/test_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/ext/test_utilities/no_logs_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/ext/test_utilities/timed_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/ext/throttling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.672961 certego_saas-0.6.0/certego_saas/ext/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/ext/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/ext/upload/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/ext/upload/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/ext/upload/twitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/ext/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/ext/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.672961 certego_saas-0.6.0/certego_saas/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.672961 certego_saas-0.6.0/certego_saas/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/management/commands/celery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/management/commands/duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/management/commands/queues.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.672961 certego_saas-0.6.0/certego_saas/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.664960 certego_saas-0.6.0/certego_saas/templates/certego_saas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.676961 certego_saas-0.6.0/certego_saas/templates/certego_saas/emails/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/templates/certego_saas/emails/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/templates/certego_saas/emails/certego-logo-positive.png
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/templates/certego_saas/emails/org-invitation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/templates/context_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 13:09:58.000000 certego_saas-0.6.0/certego_saas/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.664960 certego_saas-0.6.0/certego_saas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-23 13:10:09.000000 certego_saas-0.6.0/certego_saas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-05-23 13:10:09.000000 certego_saas-0.6.0/certego_saas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:10:09.000000 certego_saas-0.6.0/certego_saas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-23 13:10:09.000000 certego_saas-0.6.0/certego_saas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-23 13:10:09.000000 certego_saas-0.6.0/certego_saas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-23 13:09:58.000000 certego_saas-0.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.676961 certego_saas-0.6.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-23 13:09:58.000000 certego_saas-0.6.0/requirements/requirements.dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-23 13:09:58.000000 certego_saas-0.6.0/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 13:10:09.676961 certego_saas-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-23 13:09:58.000000 certego_saas-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.676961 certego_saas-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-23 13:09:58.000000 certego_saas-0.6.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.676961 certego_saas-0.6.0/tests/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:09:58.000000 certego_saas-0.6.0/tests/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.676961 certego_saas-0.6.0/tests/apps/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:09:58.000000 certego_saas-0.6.0/tests/apps/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-23 13:09:58.000000 certego_saas-0.6.0/tests/apps/auth/test_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.676961 certego_saas-0.6.0/tests/apps/feedback/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:09:58.000000 certego_saas-0.6.0/tests/apps/feedback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-23 13:09:58.000000 certego_saas-0.6.0/tests/apps/feedback/test_feedback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.676961 certego_saas-0.6.0/tests/apps/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:09:58.000000 certego_saas-0.6.0/tests/apps/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-05-23 13:09:58.000000 certego_saas-0.6.0/tests/apps/notifications/test_notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.676961 certego_saas-0.6.0/tests/apps/organization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:09:58.000000 certego_saas-0.6.0/tests/apps/organization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-05-23 13:09:58.000000 certego_saas-0.6.0/tests/apps/organization/test_invitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-05-23 13:09:58.000000 certego_saas-0.6.0/tests/apps/organization/test_organization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.676961 certego_saas-0.6.0/tests/apps/payments/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-23 13:09:58.000000 certego_saas-0.6.0/tests/apps/payments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-23 13:09:58.000000 certego_saas-0.6.0/tests/apps/payments/test_payments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.676961 certego_saas-0.6.0/tests/apps/user/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:09:58.000000 certego_saas-0.6.0/tests/apps/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-23 13:09:58.000000 certego_saas-0.6.0/tests/apps/user/test_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.676961 certego_saas-0.6.0/tests/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:09:58.000000 certego_saas-0.6.0/tests/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.676961 certego_saas-0.6.0/tests/ext/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:09:58.000000 certego_saas-0.6.0/tests/ext/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-23 13:09:58.000000 certego_saas-0.6.0/tests/ext/upload/test_slack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.676961 certego_saas-0.6.0/tests/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:09:58.000000 certego_saas-0.6.0/tests/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:10:09.676961 certego_saas-0.6.0/tests/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:09:58.000000 certego_saas-0.6.0/tests/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:09:58.000000 certego_saas-0.6.0/tests/management/commands/test_celery.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:09:58.000000 certego_saas-0.6.0/tests/management/commands/test_duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-23 13:09:58.000000 certego_saas-0.6.0/tests/management/commands/test_queues.py
```

### Comparing `certego_saas-0.5.0/LICENSE` & `certego_saas-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/PKG-INFO` & `certego_saas-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certego_saas
-Version: 0.5.0
+Version: 0.6.0
 Summary: Certego SaaS
 Home-page: https://github.com/certego/certego-saas
 Author: Certego S.R.L
 License: MIT
 Project-URL: Documentation, https://github.com/certego/certego-saas
 Project-URL: Source, https://github.com/certego/certego-saas
 Project-URL: Tracker, https://github.com/certego/certego-saas/issues
```

### Comparing `certego_saas-0.5.0/README.md` & `certego_saas-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/auth/backend.py` & `certego_saas-0.6.0/certego_saas/apps/auth/backend.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/auth/views.py` & `certego_saas-0.6.0/certego_saas/apps/auth/views.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/feedback/migrations/0001_initial.py` & `certego_saas-0.6.0/certego_saas/apps/feedback/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/feedback/models.py` & `certego_saas-0.6.0/certego_saas/apps/feedback/models.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/feedback/serializers.py` & `certego_saas-0.6.0/certego_saas/apps/feedback/serializers.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/feedback/views.py` & `certego_saas-0.6.0/certego_saas/apps/feedback/views.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/notifications/filters.py` & `certego_saas-0.6.0/certego_saas/apps/notifications/filters.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/notifications/management/commands/changelog_notification.py` & `certego_saas-0.6.0/certego_saas/apps/notifications/management/commands/changelog_notification.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/notifications/migrations/0001_initial.py` & `certego_saas-0.6.0/certego_saas/apps/notifications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/notifications/migrations/0002_alter_notification_appname.py` & `certego_saas-0.6.0/certego_saas/apps/notifications/migrations/0002_alter_notification_appname.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/notifications/migrations/0003_for_user.py` & `certego_saas-0.6.0/certego_saas/apps/notifications/migrations/0003_for_user.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/notifications/models.py` & `certego_saas-0.6.0/certego_saas/apps/notifications/models.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/notifications/serializers.py` & `certego_saas-0.6.0/certego_saas/apps/notifications/serializers.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/notifications/views.py` & `certego_saas-0.6.0/certego_saas/apps/notifications/views.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/organization/admin.py` & `certego_saas-0.6.0/certego_saas/apps/organization/admin.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/organization/invitation.py` & `certego_saas-0.6.0/certego_saas/apps/organization/invitation.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/organization/membership.py` & `certego_saas-0.6.0/certego_saas/apps/organization/membership.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/organization/migrations/0001_initial.py` & `certego_saas-0.6.0/certego_saas/apps/organization/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/organization/mixins.py` & `certego_saas-0.6.0/certego_saas/apps/organization/mixins.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/organization/organization.py` & `certego_saas-0.6.0/certego_saas/apps/organization/organization.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/organization/permissions.py` & `certego_saas-0.6.0/certego_saas/apps/organization/permissions.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/organization/serializers.py` & `certego_saas-0.6.0/certego_saas/apps/organization/serializers.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/organization/views.py` & `certego_saas-0.6.0/certego_saas/apps/organization/views.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/payments/admin.py` & `certego_saas-0.6.0/certego_saas/apps/payments/admin.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/payments/cache.py` & `certego_saas-0.6.0/certego_saas/apps/payments/cache.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/payments/consts.py` & `certego_saas-0.6.0/certego_saas/apps/payments/consts.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/payments/exceptions.py` & `certego_saas-0.6.0/certego_saas/apps/payments/exceptions.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/payments/migrations/0001_initial.py` & `certego_saas-0.6.0/certego_saas/apps/payments/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/payments/models.py` & `certego_saas-0.6.0/certego_saas/apps/payments/models.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/payments/permissions.py` & `certego_saas-0.6.0/certego_saas/apps/payments/permissions.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/payments/serializers.py` & `certego_saas-0.6.0/certego_saas/apps/payments/serializers.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/payments/throttling.py` & `certego_saas-0.6.0/certego_saas/apps/payments/throttling.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/payments/utils.py` & `certego_saas-0.6.0/certego_saas/apps/payments/utils.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/user/admin.py` & `certego_saas-0.6.0/certego_saas/apps/user/admin.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/user/forms.py` & `certego_saas-0.6.0/certego_saas/apps/user/forms.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/user/migrations/0001_initial.py` & `certego_saas-0.6.0/certego_saas/apps/user/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/user/migrations/0002_migration.py` & `certego_saas-0.6.0/certego_saas/apps/user/migrations/0002_migration.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/user/models.py` & `certego_saas-0.6.0/certego_saas/apps/user/models.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/user/serializers.py` & `certego_saas-0.6.0/certego_saas/apps/user/serializers.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/apps/user/views.py` & `certego_saas-0.6.0/certego_saas/apps/user/views.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/ext/exceptions.py` & `certego_saas-0.6.0/certego_saas/ext/exceptions.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/ext/helpers.py` & `certego_saas-0.6.0/certego_saas/ext/helpers.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/ext/log.py` & `certego_saas-0.6.0/certego_saas/ext/log.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/ext/managers.py` & `certego_saas-0.6.0/certego_saas/ext/managers.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/ext/middlewares.py` & `certego_saas-0.6.0/certego_saas/ext/middlewares.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,15 @@
+import logging
 import time
 
+from django.conf import settings
+from django.http.response import Http404
+
+logger = logging.getLogger(__name__)
+
 
 class StatsMiddleware:
     """
     Install this middleware if you are using
     :meth:`certego_saas.ext.exceptions.custom_exception_handler`.
     """
 
@@ -11,19 +17,14 @@
         self.get_response = get_response
 
     def __call__(self, request):
         request.x_request_time = time.time()  # used in exception logging
         return self.get_response(request)
 
 
-import logging
-
-logger = logging.getLogger(__name__)
-
-
 class LogMiddleware:
     """
     Install this middleware if you want to add basic logging to your API endpoints
     """
 
     def __init__(self, get_response):
         self.get_response = get_response
@@ -40,7 +41,36 @@
 
         logger.info(f"response {request.method} {request.path} sent to {request.user}")
 
         # Code to be executed for each request/response after
         # the view is called.
 
         return response
+
+
+class BlockListForwardedForMiddleware:
+    """
+    Every request that has the X-Forwarded-From set as an ip in BLOCKLIST_FORWARDED_FOR returns 404
+    """
+
+    def __init__(self, get_response):
+        self.get_response = get_response
+        # One-time configuration and initialization.
+
+    def __call__(self, request):
+        # Code to be executed for each request before
+        # the view (and later middleware) are called.
+
+        remote_addr = request.headers.get("X-Forwarded-For", "")
+        try:
+            blocklist = settings.BLOCKLIST_FORWARDED_FOR
+        except AttributeError:
+            blocklist = []
+        if remote_addr in blocklist:
+            raise Http404(f"Request has X-Forwarded-For set to {remote_addr}: blocked")
+
+        response = self.get_response(request)
+
+        # Code to be executed for each request/response after
+        # the view is called.
+
+        return response
```

### Comparing `certego_saas-0.5.0/certego_saas/ext/mixins.py` & `certego_saas-0.6.0/certego_saas/ext/mixins.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/ext/models.py` & `certego_saas-0.6.0/certego_saas/ext/models.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/ext/pagination.py` & `certego_saas-0.6.0/certego_saas/ext/pagination.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/ext/serializers.py` & `certego_saas-0.6.0/certego_saas/ext/serializers.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/ext/test_utilities/no_logs_test_case.py` & `certego_saas-0.6.0/certego_saas/ext/test_utilities/no_logs_test_case.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/ext/test_utilities/timed_runner.py` & `certego_saas-0.6.0/certego_saas/ext/test_utilities/timed_runner.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/ext/throttling.py` & `certego_saas-0.6.0/certego_saas/ext/throttling.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/ext/upload/elastic.py` & `certego_saas-0.6.0/certego_saas/ext/upload/elastic.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/ext/upload/slack.py` & `certego_saas-0.6.0/certego_saas/ext/upload/slack.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/ext/upload/twitter.py` & `certego_saas-0.6.0/certego_saas/ext/upload/twitter.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/ext/views.py` & `certego_saas-0.6.0/certego_saas/ext/views.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/ext/viewsets.py` & `certego_saas-0.6.0/certego_saas/ext/viewsets.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/management/commands/celery.py` & `certego_saas-0.6.0/certego_saas/management/commands/celery.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/management/commands/duplicates.py` & `certego_saas-0.6.0/certego_saas/management/commands/duplicates.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/management/commands/queues.py` & `certego_saas-0.6.0/certego_saas/management/commands/queues.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/models.py` & `certego_saas-0.6.0/certego_saas/models.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/settings.py` & `certego_saas-0.6.0/certego_saas/settings.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/templates/certego_saas/emails/base.html` & `certego_saas-0.6.0/certego_saas/templates/certego_saas/emails/base.html`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/templates/certego_saas/emails/certego-logo-positive.png` & `certego_saas-0.6.0/certego_saas/templates/certego_saas/emails/certego-logo-positive.png`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas/templates/certego_saas/emails/org-invitation.html` & `certego_saas-0.6.0/certego_saas/templates/certego_saas/emails/org-invitation.html`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas.egg-info/PKG-INFO` & `certego_saas-0.6.0/certego_saas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certego-saas
-Version: 0.5.0
+Version: 0.6.0
 Summary: Certego SaaS
 Home-page: https://github.com/certego/certego-saas
 Author: Certego S.R.L
 License: MIT
 Project-URL: Documentation, https://github.com/certego/certego-saas
 Project-URL: Source, https://github.com/certego/certego-saas
 Project-URL: Tracker, https://github.com/certego/certego-saas/issues
```

### Comparing `certego_saas-0.5.0/certego_saas.egg-info/SOURCES.txt` & `certego_saas-0.6.0/certego_saas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/certego_saas.egg-info/requires.txt` & `certego_saas-0.6.0/certego_saas.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/setup.py` & `certego_saas-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/tests/__init__.py` & `certego_saas-0.6.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/tests/apps/auth/test_auth.py` & `certego_saas-0.6.0/tests/apps/auth/test_auth.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/tests/apps/feedback/test_feedback.py` & `certego_saas-0.6.0/tests/apps/feedback/test_feedback.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/tests/apps/notifications/test_notifications.py` & `certego_saas-0.6.0/tests/apps/notifications/test_notifications.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/tests/apps/organization/test_invitation.py` & `certego_saas-0.6.0/tests/apps/organization/test_invitation.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/tests/apps/organization/test_organization.py` & `certego_saas-0.6.0/tests/apps/organization/test_organization.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/tests/apps/payments/__init__.py` & `certego_saas-0.6.0/tests/apps/payments/__init__.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.5.0/tests/apps/user/test_user.py` & `certego_saas-0.6.0/tests/apps/user/test_user.py`

 * *Files identical despite different names*

