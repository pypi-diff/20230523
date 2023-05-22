# Comparing `tmp/core_models-0.0.4.tar.gz` & `tmp/core_models-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_models-0.0.4.tar", last modified: Thu May 18 20:38:35 2023, max compression
+gzip compressed data, was "core_models-0.0.5.tar", last modified: Mon May 22 22:45:06 2023, max compression
```

## Comparing `core_models-0.0.4.tar` & `core_models-0.0.5.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-18 20:38:35.500532 core_models-0.0.4/
--rw-r--r--   0 macbookpro   (501) staff       (20)     1073 2022-06-15 18:33:30.000000 core_models-0.0.4/LICENSE
--rw-r--r--   0 macbookpro   (501) staff       (20)      422 2023-05-18 20:38:35.500303 core_models-0.0.4/PKG-INFO
--rw-r--r--   0 macbookpro   (501) staff       (20)     6234 2023-04-18 09:31:52.000000 core_models-0.0.4/README.md
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-18 20:38:35.487085 core_models-0.0.4/core_models/
--rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-04-18 09:44:55.000000 core_models-0.0.4/core_models/__init__.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      851 2023-05-07 10:35:43.000000 core_models-0.0.4/core_models/api_response.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-18 20:38:35.489686 core_models-0.0.4/core_models/app/
--rw-r--r--   0 macbookpro   (501) staff       (20)      109 2023-04-26 13:38:04.000000 core_models-0.0.4/core_models/app/__init__.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     9301 2023-05-12 19:47:36.000000 core_models-0.0.4/core_models/app/admin.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      114 2023-04-19 22:18:54.000000 core_models-0.0.4/core_models/app/apps.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      163 2023-04-29 15:41:05.000000 core_models-0.0.4/core_models/app/context_processors.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-18 20:38:35.490383 core_models-0.0.4/core_models/app/managers/
--rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-04-26 12:17:14.000000 core_models-0.0.4/core_models/app/managers/__init__.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     2844 2023-05-01 17:47:00.000000 core_models-0.0.4/core_models/app/managers/notification_manager.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-18 20:38:35.493679 core_models-0.0.4/core_models/app/migrations/
--rw-r--r--   0 macbookpro   (501) staff       (20)     8126 2023-04-19 22:19:11.000000 core_models-0.0.4/core_models/app/migrations/0001_initial.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      569 2023-04-19 22:36:45.000000 core_models-0.0.4/core_models/app/migrations/0002_alter_user_name_alter_user_phone_number.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      408 2023-04-19 23:19:29.000000 core_models-0.0.4/core_models/app/migrations/0003_alter_user_onboarding_stage.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      586 2023-04-22 08:50:49.000000 core_models-0.0.4/core_models/app/migrations/0004_user_reset_token_user_reset_token_expiry.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     2143 2023-04-26 06:58:10.000000 core_models-0.0.4/core_models/app/migrations/0005_remove_bankaccount_user_remove_user_name_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     4814 2023-04-26 19:53:31.000000 core_models-0.0.4/core_models/app/migrations/0006_currency_invoice_alter_company_options_invoiceitem.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     2747 2023-04-27 05:17:16.000000 core_models-0.0.4/core_models/app/migrations/0007_remove_invoice_paid_invoice_status_invoice_subtotal_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     8196 2023-04-28 12:13:35.000000 core_models-0.0.4/core_models/app/migrations/0008_alter_contract_options_contract_status_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      682 2023-04-28 12:38:08.000000 core_models-0.0.4/core_models/app/migrations/0009_alter_currency_options_alter_companydocument_company.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     6021 2023-05-12 21:02:21.000000 core_models-0.0.4/core_models/app/migrations/0010_rename_discount_invoice_interest_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-04-19 22:18:28.000000 core_models-0.0.4/core_models/app/migrations/__init__.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-18 20:38:35.498196 core_models-0.0.4/core_models/app/models/
--rw-r--r--   0 macbookpro   (501) staff       (20)      365 2023-04-28 12:03:37.000000 core_models-0.0.4/core_models/app/models/__init__.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      373 2023-04-26 06:22:29.000000 core_models-0.0.4/core_models/app/models/bank_account.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1189 2023-05-01 18:18:35.000000 core_models-0.0.4/core_models/app/models/base.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     2046 2023-04-28 12:37:27.000000 core_models-0.0.4/core_models/app/models/company.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      514 2023-04-28 11:34:04.000000 core_models-0.0.4/core_models/app/models/configuration.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     2727 2023-05-01 17:53:25.000000 core_models-0.0.4/core_models/app/models/contract.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      591 2023-05-12 19:41:41.000000 core_models-0.0.4/core_models/app/models/currency.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     3280 2023-05-13 01:34:48.000000 core_models-0.0.4/core_models/app/models/invoice.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      464 2023-04-26 12:59:06.000000 core_models-0.0.4/core_models/app/models/notification.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      867 2023-04-26 23:25:11.000000 core_models-0.0.4/core_models/app/models/transaction.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1654 2023-04-30 21:58:23.000000 core_models-0.0.4/core_models/app/models/user.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-18 20:38:35.499144 core_models-0.0.4/core_models/app/templates/
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-18 20:38:35.499830 core_models-0.0.4/core_models/app/templates/core_models/
--rwxr-xr-x   0 macbookpro   (501) staff       (20)    15388 2023-05-12 10:38:46.000000 core_models-0.0.4/core_models/app/templates/core_models/mail-base.html
--rw-r--r--   0 macbookpro   (501) staff       (20)      696 2023-04-29 21:56:01.000000 core_models-0.0.4/core_models/app/templates/core_models/mail-base.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)    15204 2023-04-29 13:48:29.000000 core_models-0.0.4/core_models/app/templates/invoice.html
--rw-r--r--   0 macbookpro   (501) staff       (20)    12372 2023-04-29 13:43:51.000000 core_models-0.0.4/core_models/app/templates/reset.html
--rw-r--r--   0 macbookpro   (501) staff       (20)     3022 2023-05-11 22:07:09.000000 core_models-0.0.4/core_models/base_views.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     2062 2023-05-12 21:33:33.000000 core_models-0.0.4/core_models/constants.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     4433 2023-04-18 15:27:44.000000 core_models-0.0.4/core_models/settings.example.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     7480 2023-05-18 20:24:12.000000 core_models-0.0.4/core_models/settings.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      942 2023-04-30 10:17:16.000000 core_models-0.0.4/core_models/utils.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-18 20:38:35.488158 core_models-0.0.4/core_models.egg-info/
--rw-r--r--   0 macbookpro   (501) staff       (20)      422 2023-05-18 20:38:35.000000 core_models-0.0.4/core_models.egg-info/PKG-INFO
--rw-r--r--   0 macbookpro   (501) staff       (20)     1979 2023-05-18 20:38:35.000000 core_models-0.0.4/core_models.egg-info/SOURCES.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)        1 2023-05-18 20:38:35.000000 core_models-0.0.4/core_models.egg-info/dependency_links.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)      176 2023-05-18 20:38:35.000000 core_models-0.0.4/core_models.egg-info/requires.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)       12 2023-05-18 20:38:35.000000 core_models-0.0.4/core_models.egg-info/top_level.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)       84 2022-06-15 18:10:36.000000 core_models-0.0.4/pyproject.toml
--rw-r--r--   0 macbookpro   (501) staff       (20)       38 2023-05-18 20:38:35.500599 core_models-0.0.4/setup.cfg
--rw-r--r--   0 macbookpro   (501) staff       (20)     1213 2023-05-18 20:38:27.000000 core_models-0.0.4/setup.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-22 22:45:06.093120 core_models-0.0.5/
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1073 2022-06-15 18:33:30.000000 core_models-0.0.5/LICENSE
+-rw-r--r--   0 macbookpro   (501) staff       (20)      422 2023-05-22 22:45:06.092897 core_models-0.0.5/PKG-INFO
+-rw-r--r--   0 macbookpro   (501) staff       (20)     6234 2023-04-18 09:31:52.000000 core_models-0.0.5/README.md
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-22 22:45:06.082069 core_models-0.0.5/core_models/
+-rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-04-18 09:44:55.000000 core_models-0.0.5/core_models/__init__.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      851 2023-05-07 10:35:43.000000 core_models-0.0.5/core_models/api_response.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-22 22:45:06.084126 core_models-0.0.5/core_models/app/
+-rw-r--r--   0 macbookpro   (501) staff       (20)      109 2023-04-26 13:38:04.000000 core_models-0.0.5/core_models/app/__init__.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     9351 2023-05-22 22:44:46.000000 core_models-0.0.5/core_models/app/admin.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      114 2023-04-19 22:18:54.000000 core_models-0.0.5/core_models/app/apps.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      163 2023-04-29 15:41:05.000000 core_models-0.0.5/core_models/app/context_processors.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-22 22:45:06.084732 core_models-0.0.5/core_models/app/managers/
+-rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-04-26 12:17:14.000000 core_models-0.0.5/core_models/app/managers/__init__.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     2844 2023-05-01 17:47:00.000000 core_models-0.0.5/core_models/app/managers/notification_manager.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-22 22:45:06.087510 core_models-0.0.5/core_models/app/migrations/
+-rw-r--r--   0 macbookpro   (501) staff       (20)     8126 2023-04-19 22:19:11.000000 core_models-0.0.5/core_models/app/migrations/0001_initial.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      569 2023-04-19 22:36:45.000000 core_models-0.0.5/core_models/app/migrations/0002_alter_user_name_alter_user_phone_number.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      408 2023-04-19 23:19:29.000000 core_models-0.0.5/core_models/app/migrations/0003_alter_user_onboarding_stage.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      586 2023-04-22 08:50:49.000000 core_models-0.0.5/core_models/app/migrations/0004_user_reset_token_user_reset_token_expiry.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     2143 2023-04-26 06:58:10.000000 core_models-0.0.5/core_models/app/migrations/0005_remove_bankaccount_user_remove_user_name_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     4814 2023-04-26 19:53:31.000000 core_models-0.0.5/core_models/app/migrations/0006_currency_invoice_alter_company_options_invoiceitem.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     2747 2023-04-27 05:17:16.000000 core_models-0.0.5/core_models/app/migrations/0007_remove_invoice_paid_invoice_status_invoice_subtotal_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     8196 2023-04-28 12:13:35.000000 core_models-0.0.5/core_models/app/migrations/0008_alter_contract_options_contract_status_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      682 2023-04-28 12:38:08.000000 core_models-0.0.5/core_models/app/migrations/0009_alter_currency_options_alter_companydocument_company.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     6021 2023-05-12 21:02:21.000000 core_models-0.0.5/core_models/app/migrations/0010_rename_discount_invoice_interest_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-04-19 22:18:28.000000 core_models-0.0.5/core_models/app/migrations/__init__.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-22 22:45:06.091308 core_models-0.0.5/core_models/app/models/
+-rw-r--r--   0 macbookpro   (501) staff       (20)      365 2023-04-28 12:03:37.000000 core_models-0.0.5/core_models/app/models/__init__.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      373 2023-04-26 06:22:29.000000 core_models-0.0.5/core_models/app/models/bank_account.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1189 2023-05-01 18:18:35.000000 core_models-0.0.5/core_models/app/models/base.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     2046 2023-04-28 12:37:27.000000 core_models-0.0.5/core_models/app/models/company.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      514 2023-04-28 11:34:04.000000 core_models-0.0.5/core_models/app/models/configuration.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     2727 2023-05-01 17:53:25.000000 core_models-0.0.5/core_models/app/models/contract.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      591 2023-05-12 19:41:41.000000 core_models-0.0.5/core_models/app/models/currency.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     3335 2023-05-22 15:16:58.000000 core_models-0.0.5/core_models/app/models/invoice.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      464 2023-04-26 12:59:06.000000 core_models-0.0.5/core_models/app/models/notification.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      867 2023-04-26 23:25:11.000000 core_models-0.0.5/core_models/app/models/transaction.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1654 2023-04-30 21:58:23.000000 core_models-0.0.5/core_models/app/models/user.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-22 22:45:06.091931 core_models-0.0.5/core_models/app/templates/
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-22 22:45:06.092494 core_models-0.0.5/core_models/app/templates/core_models/
+-rwxr-xr-x   0 macbookpro   (501) staff       (20)    15388 2023-05-12 10:38:46.000000 core_models-0.0.5/core_models/app/templates/core_models/mail-base.html
+-rw-r--r--   0 macbookpro   (501) staff       (20)      696 2023-04-29 21:56:01.000000 core_models-0.0.5/core_models/app/templates/core_models/mail-base.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)    15204 2023-04-29 13:48:29.000000 core_models-0.0.5/core_models/app/templates/invoice.html
+-rw-r--r--   0 macbookpro   (501) staff       (20)    12372 2023-04-29 13:43:51.000000 core_models-0.0.5/core_models/app/templates/reset.html
+-rw-r--r--   0 macbookpro   (501) staff       (20)     3022 2023-05-11 22:07:09.000000 core_models-0.0.5/core_models/base_views.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     2062 2023-05-12 21:33:33.000000 core_models-0.0.5/core_models/constants.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     4433 2023-04-18 15:27:44.000000 core_models-0.0.5/core_models/settings.example.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     7481 2023-05-18 23:28:36.000000 core_models-0.0.5/core_models/settings.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      942 2023-04-30 10:17:16.000000 core_models-0.0.5/core_models/utils.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-22 22:45:06.083014 core_models-0.0.5/core_models.egg-info/
+-rw-r--r--   0 macbookpro   (501) staff       (20)      422 2023-05-22 22:45:06.000000 core_models-0.0.5/core_models.egg-info/PKG-INFO
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1979 2023-05-22 22:45:06.000000 core_models-0.0.5/core_models.egg-info/SOURCES.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)        1 2023-05-22 22:45:06.000000 core_models-0.0.5/core_models.egg-info/dependency_links.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)      176 2023-05-22 22:45:06.000000 core_models-0.0.5/core_models.egg-info/requires.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)       12 2023-05-22 22:45:06.000000 core_models-0.0.5/core_models.egg-info/top_level.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)       84 2022-06-15 18:10:36.000000 core_models-0.0.5/pyproject.toml
+-rw-r--r--   0 macbookpro   (501) staff       (20)       38 2023-05-22 22:45:06.093174 core_models-0.0.5/setup.cfg
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1213 2023-05-22 22:44:46.000000 core_models-0.0.5/setup.py
```

### Comparing `core_models-0.0.4/LICENSE` & `core_models-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `core_models-0.0.4/README.md` & `core_models-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `core_models-0.0.4/core_models/api_response.py` & `core_models-0.0.5/core_models/api_response.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.4/core_models/app/admin.py` & `core_models-0.0.5/core_models/app/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     fk_name = 'user'
 
 
 class BankAccountInline(admin.TabularInline):
     model = BankAccount
     can_delete = False
     fk_name = 'created_by'
+    extra = 0
 
 
 class UserAdmin(BaseUserAdmin):
     inlines = (CompanyInline, BankAccountInline)
     fieldsets = (
         (None, {"fields": ("email", "password")}),
         ("Personal info", {"fields": ("first_name", "last_name", "job_role", "phone_number", "onboarding_stage", "is_onboarding_complete", "notification_tokens")}),
@@ -70,14 +71,15 @@
         queryset.delete(force_policy=HARD_DELETE)
 
 
 class CompanyDocumentInline(admin.TabularInline):
     model = CompanyDocument
     can_delete = False
     fk_name = 'company'
+    extra = 0
 
 
 class CompanyAdmin(admin.ModelAdmin):
     inlines = (CompanyDocumentInline, )
     list_display = (
         "user", "name", "registration_number",
         "address_line1", "country", "is_verified",
@@ -106,24 +108,26 @@
         queryset.delete(force_policy=HARD_DELETE)
 
 
 class ContractDocumentItemInline(admin.TabularInline):
     model = ContractDocument
     can_delete = False
     fk_name = 'contract'
+    extra = 0
 
 
-class ContractDocumentItemInline(admin.TabularInline):
+class ContractStatusLogInline(admin.TabularInline):
     model = ContractStatusLog
     can_delete = False
     fk_name = 'contract'
+    extra = 0
 
 
 class ContractAdmin(admin.ModelAdmin):
-    inlines = (ContractDocumentItemInline, ContractDocumentItemInline)
+    inlines = (ContractDocumentItemInline, ContractStatusLogInline)
     list_display = (
         "reference", "seller", "buyer", "document",
         "status", "buyer_accepted_on", "buyer_accepted_via",
         "created_at", "updated_at", "deleted"
     )
     list_filter = ("status", )
     search_fields = ("reference", "seller", "buyer")
```

### Comparing `core_models-0.0.4/core_models/app/managers/notification_manager.py` & `core_models-0.0.5/core_models/app/managers/notification_manager.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.4/core_models/app/migrations/0001_initial.py` & `core_models-0.0.5/core_models/app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.4/core_models/app/migrations/0002_alter_user_name_alter_user_phone_number.py` & `core_models-0.0.5/core_models/app/migrations/0002_alter_user_name_alter_user_phone_number.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.4/core_models/app/migrations/0004_user_reset_token_user_reset_token_expiry.py` & `core_models-0.0.5/core_models/app/migrations/0004_user_reset_token_user_reset_token_expiry.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.4/core_models/app/migrations/0005_remove_bankaccount_user_remove_user_name_and_more.py` & `core_models-0.0.5/core_models/app/migrations/0005_remove_bankaccount_user_remove_user_name_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.4/core_models/app/migrations/0006_currency_invoice_alter_company_options_invoiceitem.py` & `core_models-0.0.5/core_models/app/migrations/0006_currency_invoice_alter_company_options_invoiceitem.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.4/core_models/app/migrations/0007_remove_invoice_paid_invoice_status_invoice_subtotal_and_more.py` & `core_models-0.0.5/core_models/app/migrations/0007_remove_invoice_paid_invoice_status_invoice_subtotal_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.4/core_models/app/migrations/0008_alter_contract_options_contract_status_and_more.py` & `core_models-0.0.5/core_models/app/migrations/0008_alter_contract_options_contract_status_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.4/core_models/app/migrations/0009_alter_currency_options_alter_companydocument_company.py` & `core_models-0.0.5/core_models/app/migrations/0009_alter_currency_options_alter_companydocument_company.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.4/core_models/app/migrations/0010_rename_discount_invoice_interest_and_more.py` & `core_models-0.0.5/core_models/app/migrations/0010_rename_discount_invoice_interest_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.4/core_models/app/models/base.py` & `core_models-0.0.5/core_models/app/models/base.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.4/core_models/app/models/company.py` & `core_models-0.0.5/core_models/app/models/company.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.4/core_models/app/models/configuration.py` & `core_models-0.0.5/core_models/app/models/configuration.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.4/core_models/app/models/contract.py` & `core_models-0.0.5/core_models/app/models/contract.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.4/core_models/app/models/currency.py` & `core_models-0.0.5/core_models/app/models/currency.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.4/core_models/app/models/invoice.py` & `core_models-0.0.5/core_models/app/models/invoice.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     base_rate = models.FloatField(default=0)
     interest_rate = models.FloatField(default=0, editable=False)
     interest = models.DecimalField(decimal_places=2, max_digits=30)
     liquify_fee = models.DecimalField(decimal_places=2, max_digits=30, default=0)
     buyer_amount = models.DecimalField(decimal_places=2, max_digits=30, default=0)
     seller_amount = models.DecimalField(decimal_places=2, max_digits=30, default=0)
     financier_amount = models.DecimalField(decimal_places=2, max_digits=30, default=0)
+    metadata = models.JSONField(null=True, blank=True)
 
     def save(self, keep_deleted=False, **kwargs):
         if not self.reference:
             now = timezone.now()
             self.reference = f"LQIN{now.strftime('%Y%m%d%H%M%S')}"
         if self.base_rate and self.seller_risk_percentage and self.buyer_risk_percentage:
             self.interest_rate = sum([self.base_rate, self.seller_risk_percentage, self.buyer_risk_percentage])
```

### Comparing `core_models-0.0.4/core_models/app/models/transaction.py` & `core_models-0.0.5/core_models/app/models/transaction.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.4/core_models/app/models/user.py` & `core_models-0.0.5/core_models/app/models/user.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.4/core_models/app/templates/core_models/mail-base.html` & `core_models-0.0.5/core_models/app/templates/core_models/mail-base.html`

 * *Files identical despite different names*

### Comparing `core_models-0.0.4/core_models/app/templates/core_models/mail-base.txt` & `core_models-0.0.5/core_models/app/templates/core_models/mail-base.txt`

 * *Files identical despite different names*

### Comparing `core_models-0.0.4/core_models/app/templates/invoice.html` & `core_models-0.0.5/core_models/app/templates/invoice.html`

 * *Files identical despite different names*

### Comparing `core_models-0.0.4/core_models/app/templates/reset.html` & `core_models-0.0.5/core_models/app/templates/reset.html`

 * *Files identical despite different names*

### Comparing `core_models-0.0.4/core_models/base_views.py` & `core_models-0.0.5/core_models/base_views.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.4/core_models/constants.py` & `core_models-0.0.5/core_models/constants.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.4/core_models/settings.example.py` & `core_models-0.0.5/core_models/settings.example.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.4/core_models/settings.py` & `core_models-0.0.5/core_models/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     DATABASES = {
         'default': {
             'ENGINE': "django.db.backends.sqlite3",
             'NAME': "test.db"
         }
     }
 else:
-    if db("DATABASE_URL"):
+    if env("DATABASE_URL"):
         DATABASES = {"default": env.db()}
     else:
         DATABASES = {
             'default': {
                 'ENGINE': db("DB_ENGINE"),
                 'NAME': db('POSTGRES_DB'),
                 'USER': db('POSTGRES_USER'),
```

### Comparing `core_models-0.0.4/core_models/utils.py` & `core_models-0.0.5/core_models/utils.py`

 * *Files identical despite different names*

### Comparing `core_models-0.0.4/core_models.egg-info/SOURCES.txt` & `core_models-0.0.5/core_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_models-0.0.4/setup.py` & `core_models-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'Liquify core package'
 LONG_DESCRIPTION = 'Package that holds all models and core ' \
                    'functions/classes of Liquify project'
 
 # Setting up
 setup(
     # the name must match the folder name 'verysimplemodule'
```

