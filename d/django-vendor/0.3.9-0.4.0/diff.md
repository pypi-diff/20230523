# Comparing `tmp/django-vendor-0.3.9.tar.gz` & `tmp/django-vendor-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-vendor-0.3.9.tar", last modified: Thu Jan 12 01:45:47 2023, max compression
+gzip compressed data, was "django-vendor-0.4.0.tar", last modified: Tue May 23 21:10:54 2023, max compression
```

## Comparing `django-vendor-0.3.9.tar` & `django-vendor-0.4.0.tar`

### file list

```diff
@@ -1,121 +1,179 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:45:47.291328 django-vendor-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-01-12 01:45:47.291328 django-vendor-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-01-12 01:44:51.000000 django-vendor-0.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:45:47.271326 django-vendor-0.3.9/django_vendor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-01-12 01:45:47.000000 django-vendor-0.3.9/django_vendor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-01-12 01:45:47.000000 django-vendor-0.3.9/django_vendor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 01:45:47.000000 django-vendor-0.3.9/django_vendor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-01-12 01:45:47.000000 django-vendor-0.3.9/django_vendor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-12 01:45:47.000000 django-vendor-0.3.9/django_vendor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-12 01:45:47.291328 django-vendor-0.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-01-12 01:44:51.000000 django-vendor-0.3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:45:47.271326 django-vendor-0.3.9/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:45:47.271326 django-vendor-0.3.9/vendor/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:45:47.271326 django-vendor-0.3.9/vendor/api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/api/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:45:47.271326 django-vendor-0.3.9/vendor/api/v1/authorizenet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/api/v1/authorizenet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11912 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/api/v1/authorizenet/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:45:47.275327 django-vendor-0.3.9/vendor/api/v1/stripe/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/api/v1/stripe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13379 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/api/v1/stripe/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/api/v1/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:45:47.275327 django-vendor-0.3.9/vendor/encrypt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/encrypt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/encrypt/cleartext.py
--rw-r--r--   0 runner    (1001) docker     (123)    18432 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/integrations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:45:47.283327 django-vendor-0.3.9/vendor/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    22899 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0002_auto_20200912_0142.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0003_auto_20200915_1839.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0004_offer_offer_description.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0005_auto_20200930_2037.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0006_auto_20201005_2257.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0007_offer_list_bundle_items.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0008_offer_allow_multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0009_auto_20201111_0743.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0010_auto_20201112_0138.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0011_auto_20201120_1750.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0012_auto_20201123_1848.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0013_auto_20201202_1759.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0014_term_types_update_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0015_uuid_payments_receipts.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0016_auto_20201203_2011.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0017_auto_20201203_2107.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0018_add_uuid_address_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0019_fill_uuid_address_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0020_lock_uuid_address_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0021_auto_20210408_2303.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0022_offer_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0023_profile_null_false.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0024_offer_deleted.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0025_auto_20210914_0025.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0026_auto_20210914_1209.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0027_bugfix_vendor_notes_invoice_history.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0028_add_trial_date_term_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0029_alter_customerprofile_currency_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0030_auto_20220414_1055.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0031_pre_invoice_status_change.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0032_alter_invoice_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0033_payment_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0034_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0035_add_subscription_relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0036_post_payment_status_change.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0037_auto_20220609_1644.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0038_auto_20220719_0944.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0039_customerprofile_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/0040_auto_20221020_1617.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:45:47.287328 django-vendor-0.3.9/vendor/models/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/models/address.py
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11425 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/models/choice.py
--rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/models/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/models/modelmanagers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10336 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/models/offer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/models/payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/models/price.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/models/product.py
--rw-r--r--   0 runner    (1001) docker     (123)    10020 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/models/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/models/receipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/models/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/models/tax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/models/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/models/wishlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:45:47.287328 django-vendor-0.3.9/vendor/processors/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52310 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/processors/authorizenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    20302 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/processors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/processors/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)    48404 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/processors/stripe_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:45:47.287328 django-vendor-0.3.9/vendor/signals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/signals/stripe_signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:45:47.287328 django-vendor-0.3.9/vendor/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    30579 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42645 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/tests/test_authorizenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    13322 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/tests/test_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    41664 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/tests/test_stripe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:45:47.291328 django-vendor-0.3.9/vendor/urls/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/urls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/urls/vendor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/urls/vendor_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:45:47.291328 django-vendor-0.3.9/vendor/views/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10743 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/views/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/views/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/views/mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/views/report.py
--rw-r--r--   0 runner    (1001) docker     (123)    14989 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/views/vendor.py
--rw-r--r--   0 runner    (1001) docker     (123)    18171 2023-01-12 01:44:51.000000 django-vendor-0.3.9/vendor/views/vendor_admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:10:54.008260 django-vendor-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-05-23 21:10:54.008260 django-vendor-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-23 21:09:17.000000 django-vendor-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-23 21:09:17.000000 django-vendor-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 21:10:54.008260 django-vendor-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:10:53.968260 django-vendor-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:10:53.972260 django-vendor-0.4.0/src/django_vendor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-05-23 21:10:53.000000 django-vendor-0.4.0/src/django_vendor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-05-23 21:10:53.000000 django-vendor-0.4.0/src/django_vendor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 21:10:53.000000 django-vendor-0.4.0/src/django_vendor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-23 21:10:53.000000 django-vendor-0.4.0/src/django_vendor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 21:10:53.000000 django-vendor-0.4.0/src/django_vendor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:10:53.976260 django-vendor-0.4.0/src/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:10:53.976260 django-vendor-0.4.0/src/vendor/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:10:53.976260 django-vendor-0.4.0/src/vendor/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/api/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:10:53.976260 django-vendor-0.4.0/src/vendor/api/v1/authorizenet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/api/v1/authorizenet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14742 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/api/v1/authorizenet/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:10:53.976260 django-vendor-0.4.0/src/vendor/api/v1/stripe/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/api/v1/stripe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13494 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/api/v1/stripe/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/api/v1/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:10:53.976260 django-vendor-0.4.0/src/vendor/encrypt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/encrypt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/encrypt/cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18432 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/integrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:10:53.984260 django-vendor-0.4.0/src/vendor/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    22899 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0002_auto_20200912_0142.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0003_auto_20200915_1839.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0004_offer_offer_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0005_auto_20200930_2037.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0006_auto_20201005_2257.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0007_offer_list_bundle_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0008_offer_allow_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0009_auto_20201111_0743.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0010_auto_20201112_0138.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0011_auto_20201120_1750.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0012_auto_20201123_1848.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0013_auto_20201202_1759.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0014_term_types_update_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0015_uuid_payments_receipts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0016_auto_20201203_2011.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0017_auto_20201203_2107.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0018_add_uuid_address_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0019_fill_uuid_address_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0020_lock_uuid_address_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0021_auto_20210408_2303.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0022_offer_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0023_profile_null_false.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0024_offer_deleted.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0025_auto_20210914_0025.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0026_auto_20210914_1209.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0027_bugfix_vendor_notes_invoice_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0028_add_trial_date_term_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0029_alter_customerprofile_currency_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0030_auto_20220414_1055.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0031_pre_invoice_status_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0032_alter_invoice_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0033_payment_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0034_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0035_add_subscription_relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0036_post_payment_status_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0037_auto_20220609_1644.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0038_auto_20220719_0944.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0039_customerprofile_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0040_auto_20221020_1617.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0041_offer_billing_start_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0042_offer_is_promotional.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/0043_invoice_global_discount.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:10:53.992260 django-vendor-0.4.0/src/vendor/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/models/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/models/choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15906 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/models/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/models/modelmanagers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/models/offer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/models/payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/models/price.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/models/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/models/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/models/receipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/models/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/models/tax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/models/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/models/wishlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:10:53.992260 django-vendor-0.4.0/src/vendor/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62438 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/processors/authorizenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22899 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/processors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/processors/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53235 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/processors/stripe_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:10:53.992260 django-vendor-0.4.0/src/vendor/signals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/signals/stripe_signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:10:53.972260 django-vendor-0.4.0/src/vendor/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:10:53.996260 django-vendor-0.4.0/src/vendor/templates/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/address_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10728 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/checkout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:10:53.996260 django-vendor-0.4.0/src/vendor/templates/vendor/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/dummy/payment_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:10:53.996260 django-vendor-0.4.0/src/vendor/templates/vendor/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/includes/account_info_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/includes/billing_address_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/includes/cost_overview.html
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/includes/edit_link.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/includes/payment_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/integration_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/invoice_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/invoice_history_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/invoice_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:10:54.004260 django-vendor-0.4.0/src/vendor/templates/vendor/manage/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/manage/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/manage/config.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/manage/config_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/manage/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/manage/invoice_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/manage/invoice_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)    20128 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/manage/offer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/manage/offers.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/manage/payment_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/manage/processor_site_config.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/manage/processor_site_config_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/manage/product.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/manage/products.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/manage/profile_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/manage/profile_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/manage/receipt_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/manage/receipt_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/manage/subscription_add_payment.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/manage/subscription_create.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12741 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/manage/subscription_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/orderitem_confirm_delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/orderitem_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/orderitem_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/ordersummary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/payment.html
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/payment_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/payment_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/payment_summary.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/purchase_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/purchase_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/refund_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templates/vendor/refund_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:10:54.004260 django-vendor-0.4.0/src/vendor/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/templatetags/admin_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:10:54.004260 django-vendor-0.4.0/src/vendor/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    30579 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49307 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/tests/test_authorizenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16951 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/tests/test_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42811 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/tests/test_stripe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:10:54.004260 django-vendor-0.4.0/src/vendor/urls/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/urls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/urls/vendor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/urls/vendor_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:10:54.008260 django-vendor-0.4.0/src/vendor/views/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10743 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/views/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/views/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/views/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/views/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/views/vendor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18072 2023-05-23 21:09:17.000000 django-vendor-0.4.0/src/vendor/views/vendor_admin.py
```

### Comparing `django-vendor-0.3.9/README.md` & `django-vendor-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/admin.py` & `django-vendor-0.4.0/src/vendor/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from django.contrib import admin
 from django.db.models import Count
 
 from vendor.models import TaxClassifier, Offer, Price, CustomerProfile, \
     Invoice, OrderItem, Receipt, Wishlist, WishlistItem, Address, Payment, \
     Subscription
 from vendor.models.choice import InvoiceStatus
-
+from vendor.models.base import get_product_model
 
 logger = logging.getLogger(__name__)
 
 
 ################
 # ADMIN ACTIONS
 ################
@@ -110,17 +110,17 @@
 class AddressAdmin(admin.ModelAdmin):
     readonly_fields = ('uuid',)
     list_display = ('name', 'profile', 'postal_code')
     search_fields = ('postal_code', )
 
 
 class CustomerProfileAdmin(admin.ModelAdmin):
-    readonly_fields = ('uuid', 'user', 'currency', 'site')
+    readonly_fields = ('uuid', )
     list_display = ('pk', 'user', 'email', 'site', 'currency', 'created')
-    search_fields = ('profile__user__username', 'profile__user__email')
+    search_fields = ('user__username', 'user__email')
     list_filter = ('site__domain', )
 
 
 class InvoiceAdmin(admin.ModelAdmin):
     readonly_fields = ('uuid', 'shipping_address', 'profile')
     list_display = ('__str__', 'profile', 'site', 'status', 'total', 'created', 'deleted')
     search_fields = ('uuid', 'profile__user__username', )
```

### Comparing `django-vendor-0.3.9/vendor/api/v1/authorizenet/views.py` & `django-vendor-0.4.0/src/vendor/api/v1/authorizenet/views.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,30 @@
-import json
 import hashlib
 import hmac
+import json
 import logging
 
+from datetime import datetime
 from django.conf import settings
-from django.core.exceptions import PermissionDenied, MultipleObjectsReturned, ObjectDoesNotExist
-from django.http import JsonResponse, HttpResponseRedirect
+from django.core.exceptions import (MultipleObjectsReturned,
+                                    ObjectDoesNotExist, PermissionDenied)
+from django.db.models import Q
+from django.http import HttpResponse, HttpResponseRedirect, JsonResponse
+from django.urls import reverse_lazy
+from django.utils import timezone
 from django.views import View
-from django.views.generic.edit import FormMixin
 from django.views.decorators.csrf import csrf_exempt
-from django.utils import timezone
-from django.urls import reverse_lazy
+from django.views.generic.edit import FormMixin
 
 from vendor.forms import DateTimeRangeForm
 from vendor.integrations import AuthorizeNetIntegration
-from vendor.models import Receipt, Invoice, Subscription, Payment
+from vendor.models import Invoice, Payment, Subscription
 from vendor.models.choice import InvoiceStatus, PurchaseStatus
-from vendor.processors.authorizenet import AuthorizeNetProcessor, sync_subscriptions
+from vendor.processors.authorizenet import (AuthorizeNetProcessor,
+                                            sync_subscriptions)
 from vendor.utils import get_site_from_request
 
 logger = logging.getLogger(__name__)
 
 
 def update_payment(site, transaction_id, transaction_detail):
     processor = AuthorizeNetProcessor(site)
@@ -29,89 +33,127 @@
     payment_info = processor.get_payment_info(transaction_detail)
     payment_status = processor.get_payment_status(transaction_detail.transactionStatus.text)
     payment_success = processor.get_payment_success(transaction_detail.responseCode.text)
 
     try:
         payment = Payment.objects.get(profile__site=site, transaction=transaction_id, status__lt=PurchaseStatus.VOID)
         payment.submitted_date = submitted_datetime
-        payment.result[timezone.now().strftime("%Y-%m-%d_%H:%M:%S")] = payment_info
+        
+        if not isinstance(payment.result, dict):
+            payment.result = {}
+            payment.result[timezone.now().strftime("%Y-%m-%d_%H:%M:%S")] = payment_info
+        else:
+            payment.result.update({
+                timezone.now().strftime("%Y-%m-%d_%H:%M:%S"): payment_info
+            })
         payment.status = payment_status
         payment.success = payment_success
         payment.save()
+        
     except MultipleObjectsReturned as exce:
-        logger.error(f"AuthorizeCaptureAPI update_payment multiple payments for transaction: {transaction_id} error: {exce}")
+        logger.error(f"ERROR AuthorizeCaptureAPI update_payment multiple payments for transaction: {transaction_id} error: {exce}")
 
     except ObjectDoesNotExist as exce:
-        logger.error(f"AuthorizeCaptureAPI update_payment payment does not exist for transaction: {transaction_id} error: {exce}")
+        logger.error(f"ERROR AuthorizeCaptureAPI update_payment payment does not exist for transaction: {transaction_id} error: {exce}")
 
     except Exception as exce:
-        logger.error(f"AuthorizeCaptureAPI update_payment error: {exce}")
-        
+        logger.error(f"ERROR AuthorizeCaptureAPI update_payment transaction: {transaction_id}, error: {exce}")
+
+
 def subscription_save_transaction(site, transaction_id, transaction_detail):
     processor = AuthorizeNetProcessor(site)
 
     subscription_id = transaction_detail.subscription.id.text
     logger.info(f"AuthorizeCaptureAPI subscription_save_transaction saving subscription transaction: {transaction_id} for subscription {subscription_id}")
 
     submitted_datetime = datetime.strptime(transaction_detail.submitTimeUTC.pyval, '%Y-%m-%dT%H:%M:%S.%f%z')
     payment_info = processor.get_payment_info(transaction_detail)
     payment_status = processor.get_payment_status(transaction_detail.transactionStatus.text)
     payment_success = processor.get_payment_success(transaction_detail.responseCode.text)
 
+    logger.info(f"AuthorizeCaptureAPI subscription_save_transaction detail: submitted_date: {submitted_datetime}, payment_info: {payment_info}, payment_status: {payment_status}, payment_success: {payment_success}")
+
     try:
         subscription = Subscription.objects.get(gateway_id=subscription_id, profile__site=site)
 
     except MultipleObjectsReturned as exce:
-        logger.error(f"AuthorizeCaptureAPI subscription_save_transaction multiple subscription for id: {subscription_id} error: {exce}")
+        logger.error(f"ERROR AuthorizeCaptureAPI subscription_save_transaction multiple subscription for id: {subscription_id} error: {exce}")
         subscription = Subscription.objects.filter(gateway_id=subscription_id, profile__site=site).first()
 
     except ObjectDoesNotExist as exce:
-        logger.error(f"subscription_save_transaction subscription does not exist {subscription_id} exce: {exce}")
+        logger.error(f"ERROR AuthorizeCaptureAPI subscription_save_transaction subscription does not exist {subscription_id} exce: {exce}")
+        return None
+
+    if not subscription.get_offer():
+        logger.error(f"ERROR AuthorizeCaptureAPI subscription_save_transaction subscription does not have an Offer, subscription: {subscription.pk} - {subscription.gateway_id}")
         return None
 
     try:
-        payment = subscription.payments.get(transaction=None, status=PurchaseStatus.QUEUED)
-        payment.transaction = transaction_id
-        payment.submitted_date = submitted_datetime
-        payment.result[timezone.now().strftime("%Y-%m-%d_%H:%M:%S")] = payment_info
-        payment.status = payment_status
-        payment.success = payment_success
-        payment.save()
-        logger.info(f"AuthorizeCaptureAPI subscription_save_transaction: payment {payment.pk} updated")
-        
-        if payment_status == PurchaseStatus.SETTLED:
-            processor = AuthorizeNetProcessor(site, payment.invoice)
-            processor.payment = payment
-            processor.create_receipts(payment.invoice.order_items.all())
-            logger.info(f"AuthorizeCaptureAPI subscription_save_transaction: subscription renewed {subscription.pk}")
+        payment = subscription.payments.get(Q(transaction="") | Q(transaction=None), Q(status=PurchaseStatus.QUEUED))
 
     except MultipleObjectsReturned as exce:
         # There should be none or only one payment with transaction None and status in Queue
-        logger.error(f"AuthorizeCaptureAPI subscription_save_transaction multiple payments returned with None as Transaction, for {subscription_id} exce: {exce}")
-        return None
+        logger.error(f"ERROR AuthorizeCaptureAPI MultipleObjectsReturned subscription_save_transaction multiple payments returned with None as Transaction, for {subscription_id} exce: {exce}")
+        subscription.payments.filter(Q(transaction="") | Q(transaction=None), Q(status=PurchaseStatus.QUEUED)).delete()
+        logger.info(f"AuthorizeCaptureAPI renew_subscription_task subscription {subscription.pk} renewed")
+        invoice = Invoice.objects.create(
+            profile=subscription.profile,
+            site=site,
+            ordered_date=submitted_datetime,
+            total=transaction_detail.settleAmount.pyval,
+            status=InvoiceStatus.COMPLETE
+        )
+        invoice.add_offer(subscription.get_offer())
+        invoice.save()
+
+        processor = AuthorizeNetProcessor(site, invoice)
+        processor.subscription = subscription
+        
+        processor.renew_subscription(subscription, transaction_id, payment_status, payment_success, submitted_date=submitted_datetime)
+        logger.info(f"AuthorizeCaptureAPI subscription_save_transaction creating new payment and receipt for subscription, for {subscription_id}")
+
+        return None # No need to continue to create receipt as it is done in the above function
 
     except ObjectDoesNotExist as exce:
+        logger.info(f"AuthorizeCaptureAPI ObjectDoesNotExist Payment for subscription: {subscription_id} - exce: {exce}")
         logger.info(f"AuthorizeCaptureAPI renew_subscription_task subscription {subscription.pk} renewed")
         invoice = Invoice.objects.create(
-            profile=customer_profile,
+            profile=subscription.profile,
             site=site,
             ordered_date=submitted_datetime,
             total=transaction_detail.settleAmount.pyval,
             status=InvoiceStatus.COMPLETE
         )
-        invoice.add_offer(offer)
+        invoice.add_offer(subscription.get_offer())
         invoice.save()
 
         processor = AuthorizeNetProcessor(site, invoice)
         processor.subscription = subscription
         
-        processor.renew_subscription(subscription, transaction_id, payment_status, payment_success)
+        processor.renew_subscription(subscription, transaction_id, payment_status, payment_success, submitted_date=submitted_datetime)
         logger.info(f"AuthorizeCaptureAPI subscription_save_transaction creating new payment and receipt for subscription, for {subscription_id}")
         
         return None # No need to continue to create receipt as it is done in the above function
+    
+    payment.amount = transaction_detail.settleAmount.pyval
+    payment.transaction = transaction_id
+    payment.submitted_date = submitted_datetime
+    payment.result = {}
+    payment.result[timezone.now().strftime("%Y-%m-%d_%H:%M:%S")] = payment_info
+    payment.status = payment_status
+    payment.success = payment_success
+    payment.save()
+    logger.info(f"AuthorizeCaptureAPI subscription_save_transaction: payment {payment.pk} updated")
+    
+    if payment_status == PurchaseStatus.SETTLED:
+        processor = AuthorizeNetProcessor(site, payment.invoice)
+        processor.payment = payment
+        processor.subscription = subscription
+        processor.create_receipts(payment.invoice.order_items.all())
+        logger.info(f"AuthorizeCaptureAPI subscription_save_transaction: subscription renewed {subscription.pk}")
 
 def settle_authorizenet_transactions(site, start_date, end_date):
     processor = AuthorizeNetProcessor(site)
 
     settled_transactions = processor.get_settled_transactions(start_date, end_date)
     processor.update_payments_to_settled(site, settled_transactions)
 
@@ -151,15 +193,15 @@
 
             logger.info(f"AuthorizeNetBaseAPI is_valid_post: Checking hashs\nCALCULATED: {hash_value}\nREQUEST VALUE: {self.request.META.get('HTTP_X_ANET_SIGNATURE')[7:]}")
 
             if hash_value.upper() == self.request.META.get('HTTP_X_ANET_SIGNATURE')[7:]:
                 return True
 
         except TypeError as exce:
-            logger.error(f'AuthorizeNetBaseAPI is_valid_post: TypeError Exception: {exce}')
+            logger.error(f'ERROR AuthorizeNetBaseAPI is_valid_post: TypeError Exception: {exce}')
 
         return False
 
 
 class AuthorizeCaptureAPI(AuthorizeNetBaseAPI):
     """
     API endpoint to get event notifications from authorizenet when a authcaputre is created.
@@ -167,73 +209,80 @@
     """
     def is_request_valid(self, site, request_data):
         if not request_data:
             logger.warning("AuthorizeCaptureAPI post: Webhook event has no body")
             return False
 
         if not request_data.get('payload', {}).get('id'):
-            logger.error(f"AuthorizeCaptureAPI post: No transaction id request data: {request_data}")
+            logger.error(f"ERROR AuthorizeCaptureAPI post: No transaction id request data: {request_data}")
             return False
             
         if not self.is_valid_post(site):
-            logger.error(f"AuthorizeCaptureAPI post: Request was denied: {self.request}")
+            logger.error(f"ERROR AuthorizeCaptureAPI post: Request was denied: {self.request}")
             return False
 
-            
         return True
 
     def post(self, *args, **kwargs):
-        logger.info(f"AuthorizeCaptureAPI post: Event webhook: {self.request.body}")
+        try:
+            logger.info(f"AuthorizeCaptureAPI post: Event webhook: {self.request.body}")
 
-        site = get_site_from_request(self.request)
-        logger.info(f"AuthorizeCaptureAPI post: site: {site}")
+            site = get_site_from_request(self.request)
+            logger.info(f"AuthorizeCaptureAPI post: site: {site}")
 
-        request_data = json.loads(self.request.body)
-        logger.info(f"AuthorizeCaptureAPI post: request data: {request_data}")
+            request_data = json.loads(self.request.body)
+            logger.info(f"AuthorizeCaptureAPI post: request data: {request_data}")
 
-        if not self.is_request_valid(site, request_data):
-            return JsonResponse({"msg": "AuthorizeCaptureAPI post: Request is invalid"})
+            if not self.is_request_valid(site, request_data):
+                logger.error("AuthorizeCaptureAPI post: Request is invalid")
+                return HttpResponse(status=200, content="AuthorizeCaptureAPI post: Request is invalid")
 
-        transaction_id = request_data.get('payload').get('id')
-        logger.info(f"AuthorizeCaptureAPI post: Getting transaction detail for id: {transaction_id}")
+            transaction_id = request_data.get('payload').get('id')
+            logger.info(f"AuthorizeCaptureAPI post: Getting transaction detail for id: {transaction_id}")
 
-        processor = AuthorizeNetProcessor(site)
-        transaction_detail = processor.get_transaction_detail(transaction_id)
+            processor = AuthorizeNetProcessor(site)
+            transaction_detail = processor.get_transaction_detail(transaction_id)
 
-        if not hasattr(transaction_detail, 'subscription'):
-            logger.info(f"AuthorizeCaptureAPI post: updating payment for transaction detail: {transaction_detail}")
-            update_payment(site, transaction_id, transaction_detail)
+            if not hasattr(transaction_detail, 'subscription'):
+                logger.info(f"AuthorizeCaptureAPI post: updating payment for transaction: {transaction_id}")
+                update_payment(site, transaction_id, transaction_detail)
 
-        else:
-            logger.info(f"AuthorizeCaptureAPI post: saving subscription transaction: {transaction_detail}")
-            subscription_save_transaction(site, request_data.get('payload'), transaction_detail)
+            elif transaction_detail:
+                logger.info(f"AuthorizeCaptureAPI post: saving subscription transaction: {transaction_id}")
+                subscription_save_transaction(site, transaction_id, transaction_detail)
+            else:
+                logger.error(f"ERROR AuthorizeCaptureAPI post: No transaction detail for transaction: {transaction_id}")
 
-        return JsonResponse({"msg": "AuthorizeCaptureAPI post event finished"})
+        except Exception as exce:
+            logger.error(f"ERROR AuthorizeCaptureAPI post: exception: {exce}")
+            
+        logger.info("AuthorizeCaptureAPI post event finished")
+        return HttpResponse(status=200, content="AuthorizeCaptureAPI post event finished")
 
 
 class VoidAPI(AuthorizeNetBaseAPI):
 
     def post(self, *args, **kwargs):
         logger.info(f"VoidAPI post: Event webhook: {self.request.body}")
         site = get_site_from_request(self.request)
         logger.info(f"VoidAPI post: site: {site}")
 
         if not self.request.body:
             logger.warning("VoidAPI post: Webhook event has no body")
             return JsonResponse({"msg": "VoidAPI post: Webhook event has no body"})
 
         if not self.is_valid_post(site):
-            logger.error(f"VoidAPI post: Request was denied: {self.request}")
+            logger.error(f"ERROR VoidAPI post: Request was denied: {self.request}")
             raise PermissionDenied()
         
         request_data = json.loads(self.request.body)
         logger.info(f"VoidAPI post: request data: {request_data}")
 
         if request_data.get('eventType') != 'net.authorize.payment.void.created':
-            logger.error(f"VoidAPI post: wrong event type: {request_data.get('eventType')}")
+            logger.error(f"ERROR VoidAPI post: wrong event type: {request_data.get('eventType')}")
             return JsonResponse({"msg": "Event type is incorrect"})
         
         Payment.objects.filter(profile__site=site, transaction=request_data.get('payload').get('id')).update(status=PurchaseStatus.VOID)
         logger.info(f"VoidAPI post: payment with transaction voided: {request_data.get('payload').get('id')}")
 
         return JsonResponse({"msg": "VoidAPI post: success"})
 
@@ -251,10 +300,10 @@
     success_url = reverse_lazy('vendor:vendor-home')
 
     def post(self, request, *args, **kwargs):
         form = self.get_form_class()(request.POST)
         site = get_site_from_request(self.request)
 
         if form.is_valid():
-            settle_authorizenet_transactions(site, start_date, end_date)
+            settle_authorizenet_transactions(site, form.cleaned_data['start_date'], form.cleaned_data['end_date'])
 
         return HttpResponseRedirect(self.request.META.get('HTTP_REFERER', self.get_success_url()))
```

### Comparing `django-vendor-0.3.9/vendor/api/v1/stripe/views.py` & `django-vendor-0.4.0/src/vendor/api/v1/stripe/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,56 +95,56 @@
 
         if not self.is_valid_post(site):
             logger.error(f"StripeSubscriptionInvoicePaid error: invalid post")
             return HttpResponse(status=400, content="StripeSubscriptionInvoicePaid invalid post")
 
         if not self.is_incoming_event_correct_and_recurring(self.event, StripeEvents.INVOICE_PAID):
             logger.error(f"StripeSubscriptionInvoicePaid error: invalid event: {self.event}")
-            return HttpResponse(status=400, content=f"StripeSubscriptionInvoicePaid error: invalid event: {self.event}")
+            return HttpResponse(status=200, content=f"StripeSubscriptionInvoicePaid error: invalid event: {self.event}")
 
         stripe_invoice = self.event.data.object
-        paid_date = timezone.datetime.fromtimestamp(stripe_invoice.status_transitions.paid_at)
+        paid_date = timezone.datetime.fromtimestamp(stripe_invoice.status_transitions.paid_at, tz=timezone.utc)
         amount_paid = convert_integer_to_float(stripe_invoice.total)
 
         # TODO nice to move this try/except blocks inside a generic function in the StripeBaseAPI class
         try:
             customer_profile = CustomerProfile.objects.get(site=site, user__email=stripe_invoice.customer_email)
         except ObjectDoesNotExist:
             logger.error(f"StripeSubscriptionInvoicePaid error: email: {stripe_invoice.customer_email} does not exist")
             return HttpResponse(status=400, content=f"StripeSubscriptionInvoicePaid error: email: {stripe_invoice.customer_email} does not exist")
 
         if 'stripe_id' not in customer_profile.meta:
             customer_profile.meta['stripe_id'] = stripe_invoice.customer
             customer_profile.save()
 
         try:
-            subscription = Subscription.objects.get(meta__stripe_id=stripe_invoice.subscription, profile=customer_profile)
+            subscription = Subscription.objects.get(gateway_id=stripe_invoice.subscription, profile=customer_profile)
         except ObjectDoesNotExist:
             logger.error(f"StripeSubscriptionInvoicePaid customer: {customer_profile} does not have a subscription with stripe_id: {stripe_invoice.subscription}")
             return HttpResponse(status=400, content=f"StripeSubscriptionInvoicePaid customer: {customer_profile} does not have a subscription with stripe_id: {stripe_invoice.subscription}")
 
         offer = subscription.get_offer()
 
         if not offer:
             logger.error(f"StripeSubscriptionInvoicePaid {subscription} has no offer attached")
             return HttpResponse(status=400, content=f"StripeSubscriptionInvoicePaid {subscription} has no offer attached")
 
         invoice = Invoice.objects.create(
             profile=customer_profile,
             site=site,
             ordered_date=paid_date,
-            total=amount_paid,
             status=InvoiceStatus.COMPLETE
         )
         invoice.add_offer(offer)
+        invoice.total = amount_paid
         invoice.vendor_notes = {'stripe_id': stripe_invoice.stripe_id}
         invoice.save()
 
         processor = StripeProcessor(site, invoice)
-        processor.renew_subscription(subscription, stripe_invoice.charge, PurchaseStatus.SETTLED, payment_success=True)
+        processor.renew_subscription(subscription, stripe_invoice.charge, PurchaseStatus.SETTLED, payment_success=True, submitted_date=paid_date)
 
         return HttpResponse(status=200)
 
 
 class StripeSubscriptionPaymentFailed(StripeBaseAPI):
 
     def post(self, request, *args, **kwargs):
@@ -152,32 +152,32 @@
 
         if not self.is_valid_post(site):
             logger.error("StripeSubscriptionPaymentFailed error: invalid post")
             return HttpResponse(status=400, content="StripeSubscriptionPaymentFailed error: invalid post")
 
         if not self.is_incoming_event_correct_and_recurring(self.event, StripeEvents.INVOICE_PAYMENT_FAILED):
             logger.error(f"StripeSubscriptionPaymentFailed error: invalid event: {self.event}")
-            return HttpResponse(status=400, content=f"StripeSubscriptionPaymentFailed error: invalid event: {self.event}")
+            return HttpResponse(status=200, content=f"StripeSubscriptionPaymentFailed error: invalid event: {self.event}")
 
         stripe_invoice = self.event.data.object
-        paid_date = timezone.datetime.fromtimestamp(stripe_invoice.status_transitions.paid_at)
+        paid_date = timezone.datetime.fromtimestamp(stripe_invoice.status_transitions.paid_at, tz=timezone.utc)
 
         # TODO nice to move this try/except blocks inside a generic function in the StripeBaseAPI class
         try:
             customer_profile = CustomerProfile.objects.get(site=site, user__email=stripe_invoice.customer_email)
         except ObjectDoesNotExist:
             logger.error(f"StripeSubscriptionPaymentFailed error: email: {stripe_invoice.customer_email} does not exist")
             return HttpResponse(status=400, content=f"StripeSubscriptionPaymentFailed error: email: {stripe_invoice.customer_email} does not exist")
 
         if 'stripe_id' not in customer_profile.meta:
             customer_profile.meta['stripe_id'] = stripe_invoice.customer
             customer_profile.save()
 
         try:
-            subscription = Subscription.objects.get(meta__stripe_id=stripe_invoice.subscription, profile=customer_profile)
+            subscription = Subscription.objects.get(gateway_id=stripe_invoice.subscription, profile=customer_profile)
         except ObjectDoesNotExist:
             logger.error(f"StripeSubscriptionPaymentFailed customer: {customer_profile} does not have a subscription with stripe_id: {stripe_invoice.subscription}")
             return HttpResponse(status=400, content=f"StripeSubscriptionPaymentFailed customer: {customer_profile} does not have a subscription with stripe_id: {stripe_invoice.subscription}")
 
         offer = subscription.get_offer()
 
         if not offer:
@@ -209,15 +209,15 @@
 
         if not self.is_valid_post(site):
             logger.error("StripeInvoicePaid error: invalid post")
             return HttpResponse(status=400, content="StripeInvoicePaid error: invalid post")
 
         if not self.is_incoming_event_correct(self.event, StripeEvents.INOVICE_PAYMENT_SUCCEEDED):
             logger.error(f"StripeInvoicePaid error: invalid event {self.event}")
-            return HttpResponse(status=400, content=f"StripeInvoicePaid error: invalid event {self.event}")
+            return HttpResponse(status=200, content=f"StripeInvoicePaid error: invalid event {self.event}")
 
         stripe_invoice = self.event.data.object
 
         try:
             customer_profile = CustomerProfile.objects.get(site=site, user__email=stripe_invoice.customer_email)
         except ObjectDoesNotExist:
             logger.error(f"StripeInvoicePaid error: email: {stripe_invoice.customer_email} does not exist")
@@ -234,22 +234,24 @@
             return HttpResponse(status=400, content=f"StripeInvoicePaid customer: {customer_profile} does not have a subscription with stripe_id: {stripe_invoice.subscription}")
 
         payment = subscription.payments.filter(Q(transaction="") | Q(transaction=None), status=PurchaseStatus.QUEUED).first()
         receipt = subscription.receipts.filter(Q(transaction="") | Q(transaction=None)).first()
 
         if not payment and not receipt:
             logger.warning(f"There are no payments to update for subscription: {subscription}. Stripe Invoice: {stripe_invoice.id}")
-            return HttpResponse(status=400, content=f"There are no payments to update for subscription: {subscription}. Stripe Invoice: {stripe_invoice.id}")
+            return HttpResponse(status=200, content=f"There are no payments to update for subscription: {subscription}. Stripe Invoice: {stripe_invoice.id}")
         
-        payment.transaction = stripe_invoice.charge
-        payment.status = PurchaseStatus.SETTLED
-        payment.save()
-
-        receipt.transaction = stripe_invoice.charge
-        receipt.save()
+        if payment:
+            payment.transaction = stripe_invoice.charge
+            payment.status = PurchaseStatus.SETTLED
+            payment.save()
+
+        if receipt:
+            receipt.transaction = stripe_invoice.charge
+            receipt.save()
 
         return HttpResponse(status=200)
 
 
 class StripeCardExpiring(StripeBaseAPI):
 
     def post(self, request, *args, **kwargs):
@@ -257,15 +259,15 @@
 
         if not self.is_valid_post(site):
             logger.error("StripeCardExpiring error: invalid event post")
             return HttpResponse(status=400, content="StripeCardExpiring error: invalid event post")
 
         if not self.is_incoming_event_correct(self.event, StripeEvents.SOURCE_EXPIRED):
             logger.error(f"StripeCardExpiring error: invalid event {self.event}")
-            return HttpResponse(status=400, content=f"StripeCardExpiring error: invalid event {self.event}")
+            return HttpResponse(status=200, content=f"StripeCardExpiring error: invalid event {self.event}")
 
         stripe_card = self.event.data.object
 
         stripe_customer_id = stripe_card['customer']
         if stripe_customer_id:
             try:
                 customer_profile = CustomerProfile.objects.get(meta__stripe_id=stripe_customer_id)
```

### Comparing `django-vendor-0.3.9/vendor/api/v1/urls.py` & `django-vendor-0.4.0/src/vendor/api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/api/v1/views.py` & `django-vendor-0.4.0/src/vendor/api/v1/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,40 +42,62 @@
 
         session_cart[offer_key]['quantity'] += 1
 
         if not offer.allow_multiple:
             session_cart[offer_key]['quantity'] = 1
 
         return session_cart
+    
+    def add_offer_to_customer_profile_cart(self, customer_profile, offer):
+        cart = customer_profile.get_cart_or_checkout_cart()
+        all_products = offer.products.all()
+
+        if cart.status == InvoiceStatus.CHECKOUT:
+            cart.status = InvoiceStatus.CART
+            cart.save()
+
+        if customer_profile.has_product(all_products) and not offer.allow_multiple:
+            messages.info(self.request, _("You Have Already Purchased This Item"))
+        elif cart.order_items.filter(offer__products__in=all_products).exists() and not offer.allow_multiple:
+            messages.info(self.request, _("You already have this product in you cart. You can only buy one"))
+        else:
+            messages.info(self.request, _("Added item to cart."))
+            cart.add_offer(offer)
 
     def post(self, request, *args, **kwargs):
         try:
             offer = Offer.objects.get(site=get_site_from_request(request), slug=self.kwargs["slug"], available=True)
         except ObjectDoesNotExist:
             messages.error(_("Offer does not exist or is unavailable"))
             return redirect('vendor:cart')
 
         if not request.user.is_authenticated:
             request.session['session_cart'] = self.session_cart(request, offer)
-        else:
-            profile, created = self.request.user.customer_profile.get_or_create(site=get_site_from_request(request))
+            return redirect('vendor:cart')      # Redirect to cart on success
+
+        profile, created = self.request.user.customer_profile.get_or_create(site=get_site_from_request(request))
+
+        self.add_offer_to_customer_profile_cart(profile, offer)
+
+        return redirect('vendor:cart')      # Redirect to cart on success
+    
+    def get(self, request, *args, **kwargs):
+        try:
+            offer = Offer.objects.get(site=get_site_from_request(request), slug=self.kwargs["slug"], available=True)
+        except ObjectDoesNotExist:
+            messages.error(_("Offer does not exist or is unavailable"))
+            return redirect('vendor:cart')
+
+        if not request.user.is_authenticated:
+            request.session['session_cart'] = self.session_cart(request, offer)
+            return redirect('vendor:cart')      # Redirect to cart on success
 
-            cart = profile.get_cart_or_checkout_cart()
+        profile, created = self.request.user.customer_profile.get_or_create(site=get_site_from_request(request))
 
-            if cart.status == InvoiceStatus.CHECKOUT:
-                cart.status = InvoiceStatus.CART
-                cart.save()
-
-            if profile.has_product(offer.products.all()) and not offer.allow_multiple:
-                messages.info(self.request, _("You Have Already Purchased This Item"))
-            elif cart.order_items.filter(offer__products__in=offer.products.all()).count() and not offer.allow_multiple:
-                messages.info(self.request, _("You already have this product in you cart. You can only buy one"))
-            else:
-                messages.info(self.request, _("Added item to cart."))
-                cart.add_offer(offer)
+        self.add_offer_to_customer_profile_cart(profile, offer)
 
         return redirect('vendor:cart')      # Redirect to cart on success
 
 
 class RemoveFromCartView(View):
     '''
     Removes an order item and adds it to the order. No login required as the request can come
```

### Comparing `django-vendor-0.3.9/vendor/apps.py` & `django-vendor-0.4.0/src/vendor/apps.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/config.py` & `django-vendor-0.4.0/src/vendor/config.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/forms.py` & `django-vendor-0.4.0/src/vendor/forms.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/integrations.py` & `django-vendor-0.4.0/src/vendor/integrations.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/migrations/0001_initial.py` & `django-vendor-0.4.0/src/vendor/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/migrations/0003_auto_20200915_1839.py` & `django-vendor-0.4.0/src/vendor/migrations/0003_auto_20200915_1839.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/migrations/0005_auto_20200930_2037.py` & `django-vendor-0.4.0/src/vendor/migrations/0005_auto_20200930_2037.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/migrations/0006_auto_20201005_2257.py` & `django-vendor-0.4.0/src/vendor/migrations/0006_auto_20201005_2257.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/migrations/0008_offer_allow_multiple.py` & `django-vendor-0.4.0/src/vendor/migrations/0008_offer_allow_multiple.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/migrations/0009_auto_20201111_0743.py` & `django-vendor-0.4.0/src/vendor/migrations/0009_auto_20201111_0743.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/migrations/0010_auto_20201112_0138.py` & `django-vendor-0.4.0/src/vendor/migrations/0010_auto_20201112_0138.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/migrations/0011_auto_20201120_1750.py` & `django-vendor-0.4.0/src/vendor/migrations/0011_auto_20201120_1750.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/migrations/0012_auto_20201123_1848.py` & `django-vendor-0.4.0/src/vendor/migrations/0012_auto_20201123_1848.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/migrations/0013_auto_20201202_1759.py` & `django-vendor-0.4.0/src/vendor/migrations/0013_auto_20201202_1759.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/migrations/0014_term_types_update_value.py` & `django-vendor-0.4.0/src/vendor/migrations/0014_term_types_update_value.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/migrations/0015_uuid_payments_receipts.py` & `django-vendor-0.4.0/src/vendor/migrations/0015_uuid_payments_receipts.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/migrations/0016_auto_20201203_2011.py` & `django-vendor-0.4.0/src/vendor/migrations/0016_auto_20201203_2011.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/migrations/0017_auto_20201203_2107.py` & `django-vendor-0.4.0/src/vendor/migrations/0017_auto_20201203_2107.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/migrations/0018_add_uuid_address_profile.py` & `django-vendor-0.4.0/src/vendor/migrations/0018_add_uuid_address_profile.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/migrations/0019_fill_uuid_address_profile.py` & `django-vendor-0.4.0/src/vendor/migrations/0019_fill_uuid_address_profile.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/migrations/0020_lock_uuid_address_profile.py` & `django-vendor-0.4.0/src/vendor/migrations/0020_lock_uuid_address_profile.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/migrations/0021_auto_20210408_2303.py` & `django-vendor-0.4.0/src/vendor/migrations/0021_auto_20210408_2303.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/migrations/0023_profile_null_false.py` & `django-vendor-0.4.0/src/vendor/migrations/0023_profile_null_false.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/migrations/0025_auto_20210914_0025.py` & `django-vendor-0.4.0/src/vendor/migrations/0025_auto_20210914_0025.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/migrations/0026_auto_20210914_1209.py` & `django-vendor-0.4.0/src/vendor/migrations/0026_auto_20210914_1209.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/migrations/0027_bugfix_vendor_notes_invoice_history.py` & `django-vendor-0.4.0/src/vendor/migrations/0027_bugfix_vendor_notes_invoice_history.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/migrations/0028_add_trial_date_term_details.py` & `django-vendor-0.4.0/src/vendor/migrations/0028_add_trial_date_term_details.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/migrations/0029_alter_customerprofile_currency_and_more.py` & `django-vendor-0.4.0/src/vendor/migrations/0029_alter_customerprofile_currency_and_more.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/migrations/0030_auto_20220414_1055.py` & `django-vendor-0.4.0/src/vendor/migrations/0030_auto_20220414_1055.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/migrations/0031_pre_invoice_status_change.py` & `django-vendor-0.4.0/src/vendor/migrations/0031_pre_invoice_status_change.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/migrations/0033_payment_status.py` & `django-vendor-0.4.0/src/vendor/migrations/0033_payment_status.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/migrations/0034_subscription.py` & `django-vendor-0.4.0/src/vendor/migrations/0034_subscription.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/migrations/0035_add_subscription_relation.py` & `django-vendor-0.4.0/src/vendor/migrations/0035_add_subscription_relation.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/migrations/0036_post_payment_status_change.py` & `django-vendor-0.4.0/src/vendor/migrations/0036_post_payment_status_change.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/migrations/0037_auto_20220609_1644.py` & `django-vendor-0.4.0/src/vendor/migrations/0037_auto_20220609_1644.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/migrations/0038_auto_20220719_0944.py` & `django-vendor-0.4.0/src/vendor/migrations/0038_auto_20220719_0944.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/migrations/0040_auto_20221020_1617.py` & `django-vendor-0.4.0/src/vendor/migrations/0040_auto_20221020_1617.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/models/__init__.py` & `django-vendor-0.4.0/src/vendor/models/__init__.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/models/address.py` & `django-vendor-0.4.0/src/vendor/models/address.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/models/base.py` & `django-vendor-0.4.0/src/vendor/models/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from autoslug import AutoSlugField
 
 from django.apps import apps
 from django.conf import settings
 from django.contrib.sites.models import Site
 from django.contrib.sites.managers import CurrentSiteManager
 from django.db import models
+from django.utils import timezone
 from django.utils.translation import gettext_lazy as _
 
 from vendor.config import VENDOR_PRODUCT_MODEL, DEFAULT_CURRENCY
 
 from .validator import validate_msrp
 from .utils import is_currency_available
 from .modelmanagers import SoftDeleteManager
@@ -117,28 +118,37 @@
         else:
             return self.meta['msrp']['default']
 
     def active_profile_receipts(self):
         """
         Gets currently active reciepts by checking if the customer owns the product
         """
-        return [receipt for receipt in self.receipts.all() if receipt.profile.has_product(self)]
+        now = timezone.now()
+        return self.receipts.select_related("profile").filter(
+            models.Q(deleted=False),
+            models.Q(start_date__lte=now) | models.Q(start_date=None),
+            models.Q(end_date__gte=now) | models.Q(end_date=None)
+        )
     
     def owners(self):
         """
         Gets a set list of profiles that own the product
         """
         active_receipts = self.active_profile_receipts()
         return set([receipt.profile for receipt in active_receipts])
 
     def inactive_profile_receipts(self):
         """
         Gets a list of reciepts for customers that no longer own the product.
         """
-        return [receipt for receipt in self.receipts.all() if not receipt.profile.has_product(self)]
+        now = timezone.now()
+        return self.receipts.select_related("profile").filter(deleted=False).exclude(
+            models.Q(start_date__lte=now) | models.Q(start_date=None),
+            models.Q(end_date__gte=now) | models.Q(end_date=None)
+        )
 
     def expired_owners(self):
         """
         Gets a set list of profiles that no longer own the product
         """
         owners = self.owners()
         inactive_receipts = self.inactive_profile_receipts()
```

### Comparing `django-vendor-0.3.9/vendor/models/choice.py` & `django-vendor-0.4.0/src/vendor/models/choice.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # CHOICES
 ###########
 
 CURRENCY_CHOICES = [(c.name, c.value) for c in Currency]
 
 
 class InvoiceStatus(models.IntegerChoices):
-    CART = 0, _("Cart")               # total = subtotal = sum(OrderItems.Offer.Price + Product.TaxClassifier). Avalara
+    CART     = 0, _("Cart")               # total = subtotal = sum(OrderItems.Offer.Price + Product.TaxClassifier). Avalara
     CHECKOUT = 10, _("Checkout")      # total = subtotal + shipping + Tax against Addrr if any.
     COMPLETE = 20, _("Complete")      # Payment Processor Completed Transaction.
 
 
 class TermType(models.IntegerChoices):
     SUBSCRIPTION = 100, _("Subscription")
     MONTHLY_SUBSCRIPTION = 101, _("Monthly Subscription")
@@ -34,14 +34,15 @@
     SETTLED = 20, _("Settled")
     CANCELED = 30, _("Canceled")
     REFUNDED = 35, _("Refunded")
     DECLINED = 40, _("Declined")
     ERROR = 45, _("Error")
     VOID = 50, _('Void')
 
+
 class SubscriptionStatus(models.IntegerChoices):
     PAUSED = 10, _('Pause')
     ACTIVE = 20, _('Active')
     CANCELED = 30, _('Canceled')
     SUSPENDED = 40, _('Suspended')
     EXPIRED = 50, _('Expired')
```

### Comparing `django-vendor-0.3.9/vendor/models/invoice.py` & `django-vendor-0.4.0/src/vendor/models/invoice.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import itertools
 import uuid
+import math
 
 from allauth.account.signals import user_logged_in
 
 from django.core.exceptions import ObjectDoesNotExist
 from django.contrib.sites.models import Site
 from django.contrib.sites.managers import CurrentSiteManager
 from django.db import models
 from django.dispatch import receiver
 from django.utils import timezone
 from django.utils.translation import gettext_lazy as _
 from django.urls import reverse
 
 from vendor.models.utils import set_default_site_id
 from vendor.config import DEFAULT_CURRENCY
-from vendor.utils import get_site_from_request, get_subscription_start_date
+from vendor.utils import get_site_from_request
 from .base import CreateUpdateModelBase
 from .choice import CURRENCY_CHOICES, TermType, InvoiceStatus
 from .offer import Offer
 from .base import SoftDeleteModelBase
 
 
 #####################
@@ -37,14 +38,15 @@
     ordered_date = models.DateTimeField(_("Ordered Date"), blank=True, null=True)               # When was the purchase made?
     subtotal = models.FloatField(default=0.0)
     tax = models.FloatField(blank=True, null=True)                              # Set on checkout
     shipping = models.FloatField(blank=True, null=True)                         # Set on checkout
     total = models.FloatField(blank=True, null=True)                            # Set on purchase
     currency = models.CharField(_("Currency"), max_length=4, choices=CURRENCY_CHOICES, default=DEFAULT_CURRENCY)      # User's default currency
     shipping_address = models.ForeignKey("vendor.Address", verbose_name=_("Shipping Address"), on_delete=models.CASCADE, blank=True, null=True)
+    global_discount = models.FloatField(_("Global Discount"), blank=True, null=True, default=0)  # Any value that is set in this field will be subtracted
 
     objects = models.Manager()
     on_site = CurrentSiteManager()
 
     class Meta:
         verbose_name = "Invoice"
         verbose_name_plural = "Invoices"
@@ -62,42 +64,49 @@
 
     def get_invoice_display(self):
         if self.profile.user.username is None:
             return _(f"Invoice ({self.created:%Y-%m-%d %H:%M})")
         return _(f"{self.profile.user.username} Invoice ({self.created:%Y-%m-%d %H:%M})")
 
     def add_offer(self, offer, quantity=1):
+        self.global_discount = 0
 
         order_item, created = self.order_items.get_or_create(offer=offer)
         
         # make sure the invoice pk is also in the OriderItem
         if not created and order_item.offer.allow_multiple:
             order_item.quantity += quantity
             order_item.save()
 
         self.update_totals()
         self.save()
 
         return order_item
 
     def remove_offer(self, offer, clear=False):
+        self.global_discount = 0
         try:
             order_item = self.order_items.get(offer=offer)      # Get the order item if it's present
         except ObjectDoesNotExist:
             return 0
 
         order_item.quantity -= 1
 
         if order_item.quantity == 0 or clear:
             order_item.delete()
         else:
             order_item.save()
 
         self.update_totals()
         self.save()
+
+        if not (self.get_recurring_order_items().count() or self.get_one_time_transaction_order_items().count()):
+            for order_item in self.order_items.all():
+                order_item.delete()
+
         return order_item
 
     def swap_offer(self, existing_offer, new_offer):
         """
         Functions swaps offers that have the same linked product. It will not remove bundle offers
         that also have shared product with the new offer. The function comes in handy to swap
         an offer that has the normal price with one that has a discount price or terms.
@@ -126,26 +135,27 @@
         '''
         self.tax = 0
 
     def calculate_subtotal(self):
         """
         Get the total amount of the offer, which could be a set price or the products MSRP
         """
-        return sum([item.total for item in self.order_items.all() ])
+        return sum([item.total for item in self.order_items.exclude(offer__is_promotional=True)])
 
     def update_totals(self):
         """
         Sets the invoice total field by calculating its subtotal, any discounts, its shipping and tax.
         If by any reason the total is a negative value it will return 0 as vendor cannot credit any acount
         """
         self.subtotal = self.calculate_subtotal()
         discounts = self.get_discounts()
         self.calculate_shipping()
         self.calculate_tax()
         self.total = (self.subtotal - discounts) + self.tax + self.shipping
+
         if self.total < 0:
             self.total = 0
 
     def get_payment_billing_address(self):
         if not self.payments.first().billing_address:
             return ""
         return self.payments.first().billing_address.get_address_display()
@@ -156,99 +166,94 @@
         """
         return reverse('vendor_admin:manager-order-detail', kwargs={'uuid': self.uuid})
 
     def get_recurring_order_items(self):
         """
         Gets the recurring order items in the invoice
         """
-        return self.order_items.filter(offer__terms__lt=TermType.PERPETUAL)
+        return self.order_items.filter(offer__terms__lt=TermType.PERPETUAL, offer__is_promotional=False)
 
     def get_recurring_total(self):
         """
         Gets the total price for all recurring order items in the invoice and subtracting any discounts.
         """
         recurring_time_order_items = self.get_recurring_order_items()
-        return sum([ (order_item.total - order_item.discounts) for order_item in recurring_time_order_items.all()])
+        return sum([(order_item.total - order_item.discounts) for order_item in recurring_time_order_items.all()])
 
     def get_one_time_transaction_order_items(self):
         """
         Gets one time transation order items in the invoice
         """
-        return self.order_items.filter(offer__terms__gte=TermType.PERPETUAL)
+        return self.order_items.filter(offer__terms__gte=TermType.PERPETUAL, offer__is_promotional=False)
 
     def get_one_time_transaction_total(self):
         """
         Gets the total price for order items that will be purchased on a single transation. It also subtracts any discounts
         """
         one_time_order_items = self.get_one_time_transaction_order_items()
-        return sum([ (order_item.total - order_item.discounts) for order_item in one_time_order_items.all()])
+        return sum([(order_item.total - order_item.discounts) for order_item in one_time_order_items.all()])
 
     def empty_cart(self):
         """
         Remove any offer/order_item if the invoice is in Cart State.
         """
         offers = []
-        offers = list(itertools.chain.from_iterable([ [order_item.offer] * order_item.quantity for order_item in self.order_items.all()]))
+        offers = list(itertools.chain.from_iterable([[order_item.offer] * order_item.quantity for order_item in self.order_items.all()]))
         for offer in offers:
             self.remove_offer(offer)
 
     def get_next_billing_date(self):
         """
         Return the next billing date, if an invoice has two different billing dates it will return
         the upcoming one.
         """
-        recurring_offers = self.order_items.filter(offer__terms__lt=TermType.PERPETUAL)
+        recurring_offers = self.order_items.filter(offer__terms__lt=TermType.PERPETUAL, offer__is_promotional=False)
 
         if not recurring_offers.count():
             return None
 
         next_billing_dates = [order_item.offer.get_next_billing_date() for order_item in recurring_offers]
 
         next_billing_dates.sort()
 
         return next_billing_dates[0]
-
-    def get_subscription_start_date(self):
-        """
-        Return the date the subscription will go into effect.
-        """
-        recurring_offers = self.order_items.filter(offer__terms__lt=TermType.PERPETUAL)
-
-        if not recurring_offers.count():
-            return None
-
-        next_billing_dates = [get_subscription_start_date(order_item.offer, profile=self.profile) for order_item in recurring_offers]
-
-        next_billing_dates.sort()
-
-        return next_billing_dates[0]
     
     def get_billing_dates_and_prices(self):
         now = timezone.now()
-        payments_info = {now: self.get_one_time_transaction_total()}
+        payment_dates = {now: self.get_one_time_transaction_total()}
         
         for recurring_order_item in self.get_recurring_order_items():
-            offer_total = (recurring_order_item.total - recurring_order_item.discounts)
-            start_date = recurring_order_item.offer.get_term_start_date(now)
-            subscription_start_date = get_subscription_start_date(recurring_order_item.offer, self.profile, start_date)
+            offer_total = recurring_order_item.total
 
-            if subscription_start_date in payments_info:
-                payments_info.update({subscription_start_date: payments_info[subscription_start_date] + offer_total})
+            if recurring_order_item.discounts or self.global_discount:
+                offer_total = offer_total - (recurring_order_item.discounts + math.fabs(self.global_discount))
+
+            start_date = recurring_order_item.offer.get_offer_start_date(now)
+
+            if (recurring_order_item.offer.has_trial() or recurring_order_item.offer.billing_start_date) and\
+               not self.profile.has_owned_product(recurring_order_item.offer.products.all()):
+                start_date = recurring_order_item.offer.get_payment_start_date_trial_offset(now)
+                
+                if recurring_order_item.offer.get_trial_occurrences() > 1:
+                    offer_total = recurring_order_item.offer.get_trial_amount()
+
+            if start_date in payment_dates:
+                payment_dates.update({start_date: payment_dates[start_date] + offer_total})
             else:
-                payments_info[subscription_start_date] = offer_total
+                payment_dates[start_date] = offer_total
 
-        sorted_payments = {key: payments_info[key] for key in sorted(payments_info.keys()) }
+        sorted_payments = {key: payment_dates[key] for key in sorted(payment_dates.keys()) }
         
         return sorted_payments
 
     def get_next_billing_price(self):
         """
         Returns the price corresponding to the upcoming billing date.
         """
-        recurring_offers = self.order_items.filter(offer__terms__lt=TermType.PERPETUAL)
+        recurring_offers = self.order_items.filter(offer__terms__lt=TermType.PERPETUAL, offer__is_promotional=False)
 
         if not recurring_offers.count():
             return None
 
         if recurring_offers.count() == 1:
             return recurring_offers.first().total
 
@@ -277,17 +282,30 @@
         if 'discounts' in self.vendor_notes:
             return self.vendor_notes['discounts']
 
         discounts = 0
 
         discounts = sum([order_item.discounts for order_item in self.order_items.all() if not self.profile.has_owned_product(order_item.offer.products.all())])
 
-        trial_discounts = sum([order_item.price - order_item.trial_amount for order_item in self.order_items.all() if order_item.offer.has_trial_occurrences()])
+        trial_discounts = sum([order_item.trial_amount - order_item.price for order_item in self.order_items.all() if order_item.offer.has_trial_occurrences() or order_item.offer.get_trial_days()])
+
+        return discounts + math.fabs(trial_discounts) + math.fabs(self.global_discount)
+    
+    def get_discounts_display(self):
+        """
+        Only return promotional, and global discounts. If their is a trial period price it is not added to the display.
+        """
+        if 'discounts' in self.vendor_notes:
+            return self.vendor_notes['discounts']
+
+        discounts = 0
 
-        return discounts + trial_discounts
+        discounts = sum([order_item.discounts for order_item in self.order_items.all() if not self.profile.has_owned_product(order_item.offer.products.all())])
+
+        return discounts + math.fabs(self.global_discount)
 
     def save_discounts_vendor_notes(self):
         """
         Once an invoice has been completed, this method saves the discounts applied to the invoice
         in the vendor_notes field. This makes it for faster lookup on get_discounts for future invoice
         views.
         """
@@ -348,14 +366,16 @@
     def trial_amount(self):
         if self.receipts.count():
             if 'first' in self.receipts.first().meta:
                 return self.offer.get_trial_amount()
         else:
             if self.offer.has_trial_occurrences():
                 return self.offer.get_trial_amount()
+            elif self.offer.get_trial_days():
+                return self.offer.get_trial_amount()
         return self.offer.current_price()
 
     def get_total_display(self):
         if not self.total:
             return "0.00"
 
         return f'{self.total:2}'
```

### Comparing `django-vendor-0.3.9/vendor/models/modelmanagers.py` & `django-vendor-0.4.0/src/vendor/models/modelmanagers.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/models/offer.py` & `django-vendor-0.4.0/src/vendor/models/offer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,28 @@
-import uuid
 import math
+import uuid
+from datetime import timedelta
+
 from autoslug import AutoSlugField
-from django.contrib.sites.models import Site
 from django.contrib.sites.managers import CurrentSiteManager
+from django.contrib.sites.models import Site
 from django.db import models
 from django.db.models import Q
 from django.urls import reverse
 from django.utils import timezone
 from django.utils.translation import gettext_lazy as _
 
 from vendor.config import DEFAULT_CURRENCY
-from vendor.utils import get_payment_scheduled_end_date
+from vendor.utils import get_future_date_days, get_future_date_months
 
 from .base import CreateUpdateModelBase, SoftDeleteModelBase
-from .choice import TermType, TermDetailUnits
-from .utils import set_default_site_id, is_currency_available
-from .modelmanagers import ActiveManager, ActiveCurrentSiteManager, CurrentSiteSoftDeleteManager
+from .choice import TermDetailUnits, TermType
+from .modelmanagers import (ActiveCurrentSiteManager, ActiveManager,
+                            CurrentSiteSoftDeleteManager)
+from .utils import is_currency_available, set_default_site_id
 
 
 #########
 # OFFER
 #########
 def offer_term_details_default():
     """
@@ -28,39 +31,41 @@
     """
     return {
         "period_length": 1,
         "payment_occurrences": 12,
         "term_units": TermDetailUnits.MONTH,
         "trial_occurrences": 0,
         "trial_amount": 0,
-        "trial_days": 0
+        "trial_days": 0,
     }
 
 
 class Offer(SoftDeleteModelBase, CreateUpdateModelBase):
     '''
     Offer attaches to a record from the designated VENDOR_PRODUCT_MODEL.
     This is so more than one offer can be made per product, with different
     priorities.  It also allows for the bundling of several products into
     a single Offer on the site.
     '''
     uuid = models.UUIDField(default=uuid.uuid4, editable=False, unique=True)                                # Used to track the product
-    slug = AutoSlugField(populate_from='name', unique_with='site__id')                                               # SEO friendly
+    slug = AutoSlugField(populate_from='name', unique_with='site__id', editable=True)                                               # SEO friendly
     site = models.ForeignKey(Site, verbose_name=_("Site"), on_delete=models.CASCADE, default=set_default_site_id, related_name="product_offers")                      # For multi-site support
     name = models.CharField(_("Name"), max_length=80, blank=True)                                           # If there is only a Product and this is blank, the product's name will be used, oterhwise it will default to "Bundle: <product>, <product>""
     start_date = models.DateTimeField(_("Start Date"), help_text=_("What date should this offer become available?"))
     end_date = models.DateTimeField(_("End Date"), blank=True, null=True, help_text=_("Expiration Date?"))
     terms = models.IntegerField(_("Terms"), default=0, choices=TermType.choices)
     term_details = models.JSONField(_("Term Details"), default=offer_term_details_default, blank=True, null=True, help_text=_("term_units: 10/20(Day/Month), trial_occurrences: 1(defualt)"))
     term_start_date = models.DateTimeField(_("Term Start Date"), help_text=_("When is this product available to use?"), blank=True, null=True)  # Useful for Event Tickets or Pre-Orders
+    billing_start_date = models.DateTimeField(_("Billing Start Date"), blank=True, null=True, default=None, help_text=_("The start date to begin billing"))
     available = models.BooleanField(_("Available"), default=False, help_text=_("Is this currently available?"))
     bundle = models.BooleanField(_("Is a Bundle?"), default=False, help_text=_("Is this a product bundle? (auto-generated)"))  # Auto-generated based on if the count of the products is greater than 1.
     offer_description = models.TextField(_("Offer Description"), default=None, blank=True, null=True, help_text=_("You can enter a list of descriptions. Note: if you inputs something here the product description will not show up."))
     list_bundle_items = models.BooleanField(_("List Bundled Items"), default=False, help_text=_("When showing to customers, display the included items in a list?"))
     allow_multiple = models.BooleanField(_("Allow Multiple Purchase"), default=False, help_text=_("Confirm the user wants to buy multiples of the product where typically there is just one purchased at a time."))
+    is_promotional = models.BooleanField(_("Is Promotional"), default=False, help_text=_("You can mark this offer as promotional to help identify it between normal priced and discount priced offers."))
     meta = models.JSONField(_("Meta"), default=dict, blank=True, null=True)
 
     objects = models.Manager()
     on_site = CurrentSiteManager()
     active = ActiveManager()
     on_site_active = ActiveCurrentSiteManager()
     on_site_not_deleted = CurrentSiteSoftDeleteManager()
@@ -198,17 +203,19 @@
     def has_trial_occurrences(self):
         if self.term_details.get('trial_occurrences', 0) > 0:
             return True
         return False
 
     def get_next_billing_date(self):
         start_date = timezone.now()
-        if self.term_start_date:
+
+        if self.term_start_date and self.term_start_date > start_date:
             start_date = self.term_start_date
-        return get_payment_scheduled_end_date(self, start_date)
+
+        return self.get_offer_end_date(start_date)
 
     def get_period_length(self):
         if self.terms == TermType.SUBSCRIPTION:
             return self.term_details['period_length']
         else:
             return self.terms - 100   # You subtract 100 because enum are numbered according to their period length. eg Month = 101 and Year = 112
 
@@ -217,27 +224,70 @@
         Gets the defined payment ocurrences for a Subscription. It defaults to
         9999 which means it will charge that amount until the customer cancels the subscription.
         """
         return self.term_details.get('payment_occurrences', 9999)
 
     def get_trial_occurrences(self):
         return self.term_details.get('trial_occurrences', 0)
-
-    def get_trial_amount(self):
-        return self.term_details.get('trial_amount', 0)
     
     def get_trial_days(self):
         return self.term_details.get('trial_days', 0)
 
     def has_any_discount_or_trial(self):
         if self.discount() or self.get_trial_amount() or\
-           self.get_trial_occurrences() or self.get_trial_days():
+           self.get_trial_occurrences() or self.get_trial_days() or\
+           (self.billing_start_date and self.billing_start_date > timezone.now()):
             return True
             
         return False
     
-    def get_term_start_date(self, start_date=timezone.now()):
+    def has_trial(self):
+        if self.get_trial_occurrences() or self.get_trial_days():
+            return True
+        return False
+    
+    def has_valid_billing_start_date(self, today=timezone.now()):
+        if self.billing_start_date and self.billing_start_date > today:
+            return True
+        return False
+    
+    def get_offer_start_date(self, start_date=timezone.now()):
         if self.term_start_date and self.term_start_date > start_date:
             return self.term_start_date
         
         return start_date
 
+    def get_offer_end_date(self, start_date=timezone.now()):
+        """
+        Determines the start date offset so the payment gateway starts charging the monthly offer
+        """
+        units = self.term_details.get('term_units', TermDetailUnits.MONTH)
+        
+        if units == TermDetailUnits.MONTH:
+            return get_future_date_months(start_date, self.get_period_length())
+        
+        elif units == TermDetailUnits.DAY:
+            return get_future_date_days(start_date, self.get_period_length())
+    
+    def get_trial_end_date(self, start_date=timezone.now()):
+        if self.billing_start_date and self.billing_start_date > start_date:
+            return self.billing_start_date - timedelta(days=1)
+        
+        trial_occurrences = self.get_trial_occurrences()
+        if trial_occurrences:
+            units = self.term_details.get('term_units', TermDetailUnits.MONTH)
+
+            if units == TermDetailUnits.MONTH:
+                return get_future_date_months(start_date, self.get_period_length() * trial_occurrences)
+
+            elif units == TermDetailUnits.DAY:
+                return get_future_date_days(start_date, self.get_period_length() * trial_occurrences)
+
+        return start_date + timedelta(days=self.get_trial_days())
+
+    def get_payment_start_date_trial_offset(self, start_date=timezone.now()):
+        trial_end_date = self.get_trial_end_date(start_date)
+
+        if trial_end_date == start_date:
+            return start_date
+        
+        return trial_end_date + timedelta(days=1)
```

### Comparing `django-vendor-0.3.9/vendor/models/payment.py` & `django-vendor-0.4.0/src/vendor/models/payment.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/models/price.py` & `django-vendor-0.4.0/src/vendor/models/price.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/models/profile.py` & `django-vendor-0.4.0/src/vendor/models/profile.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import uuid
 
 from django.conf import settings
-from django.contrib.sites.models import Site
 from django.contrib.sites.managers import CurrentSiteManager
+from django.contrib.sites.models import Site
 from django.db import models
-from django.db.models import Q, QuerySet, Count, Sum
+from django.db.models import Count, Q, QuerySet, Sum
 from django.utils import timezone
 from django.utils.translation import gettext_lazy as _
-from .base import CreateUpdateModelBase
-from .choice import CURRENCY_CHOICES, TermType, PurchaseStatus, SubscriptionStatus
-from .invoice import Invoice
-from .utils import set_default_site_id
-from vendor.config import DEFAULT_CURRENCY
 
+from vendor.config import DEFAULT_CURRENCY
 from vendor.models.base import get_product_model
 from vendor.models.choice import InvoiceStatus
 
+from .base import CreateUpdateModelBase
+from .choice import (CURRENCY_CHOICES, PurchaseStatus, SubscriptionStatus,
+                     TermType)
+from .utils import set_default_site_id
+
 
 #####################
 # CUSTOMER PROFILE
 #####################
 class CustomerProfile(CreateUpdateModelBase):
     '''
     Additional customer information related to purchasing.
@@ -120,21 +121,21 @@
 
     def has_future_access(self, products):
         now = timezone.now()
 
         # Queryset or List of model records
         if isinstance(products, QuerySet) or isinstance(products, list):
             return bool(self.receipts.filter(Q(products__in=products),
-                                        Q(deleted=False),
-                                        Q(start_date__gte=now) | Q(start_date=None)).count())
+                                             Q(deleted=False),
+                                             Q(start_date__gte=now) | Q(start_date=None)).count())
 
         # Single model record
         return bool(self.receipts.filter(Q(products=products),
-                                    Q(deleted=False),
-                                    Q(start_date__gte=now) | Q(start_date=None)).count())
+                                         Q(deleted=False),
+                                         Q(start_date__gte=now) | Q(start_date=None)).count())
 
     def has_owned_product(self, products):
         # Queryset or List of model records
         if isinstance(products, QuerySet) or isinstance(products, list):
             return bool(self.receipts.filter(products__in=products).count())
 
         # Single model record
@@ -154,44 +155,57 @@
 
     def get_cart_items_count(self):
         cart = self.get_cart_or_checkout_cart()
 
         return cart.order_items.all().count()
 
     def get_or_create_address(self, address):
-        address, created = self.addresses.get_or_create(name=address.address_1, first_name=address.first_name, last_name=address.last_name, address_1=address.address_1, address_2=address.address_2, locality=address.locality, state=address.state, country=address.country, postal_code=address.postal_code, profile=self)
+        address, created = self.addresses.get_or_create(
+            name=address.address_1,
+            first_name=address.first_name,
+            last_name=address.last_name,
+            address_1=address.address_1,
+            address_2=address.address_2,
+            locality=address.locality,
+            state=address.state,
+            country=address.country,
+            postal_code=address.postal_code,
+            profile=self)
         return address, created
 
     def has_previously_owned_products(self, products):
         """
         Get all products that the customer has purchased and returns True if it has.
         """
         return bool(self.receipts.filter(products__in=products).first())
 
     def get_all_customer_products(self):
         Product = get_product_model()
         return Product.objects.filter(receipts__profile=self)
 
     def get_active_products(self):
-         return set([receipt.products.first()  for receipt in self.get_active_receipts()])
+        return set([receipt.products.first()
+                    for receipt in self.get_active_receipts()])
 
     def get_active_offer_receipts(self, offer):
-        return self.receipts.filter(Q(deleted=False), Q(order_item__offer=offer), Q(end_date__gte=timezone.now()) | Q(end_date=None))
+        return self.get_active_receipts().filter(Q(order_item__offer=offer))
 
     def get_active_receipts(self):
-        return self.receipts.filter(Q(end_date__gte=timezone.now()) | Q(end_date=None))
+        return self.receipts.filter(Q(deleted=False),
+                                    Q(end_date__gte=timezone.now()) | Q(end_date=None)).exclude(products=None)
 
     def get_inactive_receipts(self):
         return self.receipts.filter(end_date__lt=timezone.now())
 
     def get_active_product_and_offer(self):
         """
         Returns a tuple product and offer tuple that are related to the active receipt
         """
-        return [(receipt.products.first(), receipt.order_item.offer) for receipt in self.receipts.filter(Q(deleted=False), Q(end_date__gte=timezone.now()) | Q(end_date=None))]
+        return [(receipt.products.first(), receipt.order_item.offer)
+                for receipt in self.get_active_receipts()]
 
     def get_subscriptions(self):
         return self.subscriptions.all()
 
     def get_active_subscriptions(self):
         return self.subscriptions.filter(status=SubscriptionStatus.ACTIVE)
 
@@ -220,15 +234,15 @@
 
     def get_payment_sum(self):
         return self.payments.filter(deleted=False, status=PurchaseStatus.SETTLED).aggregate(Sum('amount'))
 
     def get_settled_payments(self):
         return self.payments.filter(deleted=False, status=PurchaseStatus.SETTLED).order_by('amount', 'submitted_date')
 
-    def is_on_trial(self, offer):
+    def is_offer_on_trial(self, offer):
 
         on_trial_receipt = next((receipt for receipt in self.get_active_offer_receipts(offer) if receipt.transaction and 'trial' in receipt.transaction), None)
 
         if on_trial_receipt:
             return True
 
         return False
```

### Comparing `django-vendor-0.3.9/vendor/models/receipt.py` & `django-vendor-0.4.0/src/vendor/models/receipt.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import uuid
 
 from django.db import models
-from django.utils.translation import gettext_lazy as _
 from django.urls import reverse
-from django.utils import timezone, dateformat
+from django.utils import timezone
+from django.utils.translation import gettext_lazy as _
 
 from vendor.models.base import CreateUpdateModelBase, SoftDeleteModelBase
-from vendor.models.choice import PurchaseStatus
-from vendor.utils import get_payment_scheduled_end_date
 
 
 class Receipt(SoftDeleteModelBase, CreateUpdateModelBase):
     '''
     A link for all the purchases a user has made. Contains subscription start and end date.
     This is generated for each item a user purchases so it can be checked in other code.
     '''
@@ -31,13 +29,13 @@
 
     def __str__(self):
         return f"{self.profile.user.username} - {self.order_item.offer.name}"
 
     def get_absolute_url(self):
         return reverse('vendor:customer-receipt', kwargs={'uuid': self.uuid})
 
-    def is_on_trial(self):
-        first_payment = Receipt.objects.filter(transaction=self.transaction, order_item__offer__site=self.order_item.offer.site).order_by('start_date').first()
-        
-        if self.end_date <= get_payment_scheduled_end_date(first_payment.order_item.offer, first_payment.start_date):
+    def is_on_trial(self, today=timezone.now()):
+
+        if 'trial' in self.transaction and self.end_date >= today:
             return True
+        
         return False
```

### Comparing `django-vendor-0.3.9/vendor/models/subscription.py` & `django-vendor-0.4.0/src/vendor/models/subscription.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import uuid
 
-from datetime import timedelta
 from django.db import models
 from django.db.models import Q
-from django.utils.translation import gettext_lazy as _
 from django.urls import reverse
-from django.utils import timezone, dateformat
+from django.utils import timezone
+from django.utils.translation import gettext_lazy as _
 
 from vendor.models.base import CreateUpdateModelBase, SoftDeleteModelBase
-from vendor.models.choice import SubscriptionStatus, PurchaseStatus
-from vendor.utils import get_payment_scheduled_end_date
+from vendor.models.choice import PurchaseStatus, SubscriptionStatus
 
 
 class SubscriptionReportModelManger(models.Manager):
     def get_total_cancelled_subscriptions(self, site, start_date=None, end_date=None):
         qs = super().get_queryset()
         
         if not (start_date and end_date):
@@ -98,18 +96,17 @@
 
         return payment.get_receipt().start_date
         
     def is_on_trial(self):
         if not self.receipts.filter(deleted=False).count():
             return False
 
-        receipt = self.receipts.filter(deleted=False).order_by('start_date').first()
-        trial_end_date = receipt.start_date + timedelta(days=receipt.order_item.offer.get_trial_days())
+        trial_receipt = self.receipts.filter(deleted=False, transaction__contains='trial').order_by('start_date').first()
 
-        if timezone.now() > trial_end_date:
+        if timezone.now() > trial_receipt.end_date:
             return False
         
         return True
 
     def get_total(self):
         return self.receipts.first().order_item.total
 
@@ -123,9 +120,7 @@
     def get_offer(self):
         receipt = self.receipts.first()
         
         if not receipt:
             return None
         
         return receipt.order_item.offer
-
-
```

### Comparing `django-vendor-0.3.9/vendor/models/tax.py` & `django-vendor-0.4.0/src/vendor/models/tax.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/models/utils.py` & `django-vendor-0.4.0/src/vendor/models/utils.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/models/validator.py` & `django-vendor-0.4.0/src/vendor/models/validator.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/models/wishlist.py` & `django-vendor-0.4.0/src/vendor/models/wishlist.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/processors/__init__.py` & `django-vendor-0.4.0/src/vendor/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/processors/authorizenet.py` & `django-vendor-0.4.0/src/vendor/processors/authorizenet.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,19 +3,16 @@
 """
 import ast
 import logging
 
 from datetime import datetime
 from django.conf import settings
 from django.core.exceptions import ObjectDoesNotExist, MultipleObjectsReturned
-from django.db.models import IntegerChoices
-from django.utils import timezone
 from math import ceil
 from vendor.config import VENDOR_PAYMENT_PROCESSOR, VENDOR_STATE
-from vendor.utils import get_future_date_days, get_payment_scheduled_end_date
 from vendor.integrations import AuthorizeNetIntegration
 
 logger = logging.getLogger(__name__)
 
 try:
     from authorizenet import apicontractsv1
     from authorizenet import constants
@@ -125,14 +122,40 @@
             self.API_ENDPOINT = constants.SANDBOX
         elif VENDOR_STATE == 'PRODUCTION':
             self.API_ENDPOINT = constants.PRODUCTION
 
     ##########
     # Authorize.net Object creations
     ##########
+    def save_customer_profile_id(self, customer_profile_id):
+        if 'authorizenet' not in self.invoice.profile.meta:
+            self.invoice.profile.meta['authorizenet'] = {}
+        
+        self.invoice.profile.meta['authorizenet']['customerProfileId'] = customer_profile_id
+        self.invoice.profile.save()
+    
+    def save_customer_payment_profile_id(self, customer_payment_profile_id):
+        if 'authorizenet' not in self.invoice.profile.meta:
+            self.invoice.profile.meta['authorizenet'] = {}
+        
+        self.invoice.profile.meta['authorizenet']['customerPaymentProfile'] = customer_payment_profile_id
+        self.invoice.profile.save()
+
+    def get_customer_profile_id(self):
+        if 'authorizenet' not in self.invoice.profile.meta:
+            return None
+        
+        return self.invoice.profile.meta['authorizenet'].get('customerProfileId')
+    
+    def get_customer_payment_profile_id(self):
+        if 'authorizenet' not in self.invoice.profile.meta:
+            return None
+        
+        return self.invoice.profile.meta['authorizenet'].get('customerPaymentProfile')
+
     def set_controller_api_endpoint(self):
         """
         Sets the endpoint for the controller to point to test or production.
         self.API_ENDPOINT is set on Processor Initialization
         """
         self.controller.setenvironment(self.API_ENDPOINT)
 
@@ -177,21 +200,36 @@
         """
         Creates a payment instance acording to the billing information captured
         """
         payment = apicontractsv1.paymentType()
         payment.creditCard = self.payment_type_switch[int(
             self.payment_info.cleaned_data.get('payment_type'))]()
         return payment
+    
+    def create_customer_profile_charge(self):
+        profile_to_charge = apicontractsv1.customerProfilePaymentType()
+        profile_to_charge.customerProfileId = self.get_customer_profile_id()
+        profile_to_charge.paymentProfile = apicontractsv1.paymentProfile()
+        profile_to_charge.paymentProfile.paymentProfileId = self.get_customer_payment_profile_id()
 
     def create_customer_data(self):
         customerData = apicontractsv1.customerDataType()
         customerData.type = "individual"
         customerData.id = str(self.invoice.profile.user.pk)
         customerData.email = self.invoice.profile.user.email
+        
         return customerData
+    
+    def create_customer_profile_data(self):
+        customerProfileData = apicontractsv1.customerProfileType()
+        customerProfileData.email = self.invoice.profile.user.email
+        customerProfileData.description = self.invoice.site.domain
+        customerProfileData.merchantCustomerId = str(self.invoice.profile.pk)[:20]
+
+        return customerProfileData
 
     def create_customer_data_recurring(self):
         customerData = apicontractsv1.customerType()
         customerData.type = "individual"
         customerData.id = str(self.invoice.profile.user.pk)
         customerData.email = self.invoice.profile.user.email
         return customerData
@@ -280,28 +318,32 @@
         Eg. for a 1 year 1 month free subscription:
             term_unit=20 (Month), trial_occurrences=1
             start_date = now + 1 month
         Eg. for a 7 day free 1 Month subscription:
             term_units=10 (Day), trial_occurrences=7
             start_date = now + 7 days
         """
-        start_date = subscription.offer.get_term_start_date()
+        start_date = subscription.offer.get_offer_start_date()
 
         payment_schedule = apicontractsv1.paymentScheduleType()
         payment_schedule.interval = apicontractsv1.paymentScheduleTypeInterval()
         payment_schedule.interval.unit = self.get_interval_units(subscription)
 
         payment_schedule.interval.length = subscription.offer.get_period_length()
         payment_schedule.totalOccurrences = subscription.offer.get_payment_occurrences()
 
         if self.invoice.profile.has_owned_product(subscription.offer.products.all()):
             payment_schedule.startDate = CustomDate(start_date)
             payment_schedule.trialOccurrences = 0
         else:
-            payment_schedule.startDate = CustomDate(get_future_date_days(start_date, subscription.offer.get_trial_days()))
+            if subscription.offer.has_trial():
+                payment_schedule.startDate = CustomDate(subscription.offer.get_payment_start_date_trial_offset(start_date))
+            else:
+                payment_schedule.startDate = CustomDate(start_date)
+
             payment_schedule.trialOccurrences = subscription.offer.get_trial_occurrences()
                 
         return payment_schedule
 
     def create_transaction_order_information(self, invoice_number, description):
         order = apicontractsv1.orderType()
         order.invoiceNumber = invoice_number
@@ -363,22 +405,22 @@
             raise TypeError(f"{transaction_status} is not supported, check Authorize.Net docs for transactionStatus field choices")
 
     def get_payment_info(self, transaction):
         account_number = transaction.payment.creditCard.cardNumber.text[-4:]
         full_name = " ".join([transaction.billTo.firstName.text, transaction.billTo.lastName.text])
 
         payment_info = super().get_payment_info(account_number, full_name)
-        
-        return payment_info.update({
+        payment_info.update({
             'account_type': transaction.payment.creditCard.cardType.text,
             'transaction_id': transaction.transId.text,
             'subscription_id': transaction.subscription.id.text if hasattr(transaction, 'subscription') else "-",
             'payment_number': transaction.subscription.payNum.text,
             'status': transaction.transactionStatus.text
         })
+        return payment_info
 
     def subscription_info_to_dict(self, subscription_info):
         return {
             'name': subscription_info.subscription.name.text,
             'interval': subscription_info.subscription.paymentSchedule.interval.length.text,
             'unit': subscription_info.subscription.paymentSchedule.interval.unit.text,
             'start_date': subscription_info.subscription.paymentSchedule.startDate.text,
@@ -501,14 +543,26 @@
            self.transaction_response.messages.resultCode == "Ok" and\
            not self.transaction_info['errors']:
             self.transaction_succeeded = True
 
     ##########
     # Base Processor Transaction Implementations
     ##########
+    def pre_authorization(self):
+        """
+        Called before the authorization begins.
+        """
+        if 'authorizenet' not in self.invoice.profile.meta and VENDOR_STATE != 'DEBUG':
+            self.create_customer_profile()
+            self.create_customer_profile_payment_id(self.get_customer_profile_id())
+
+        self.transaction_succeeded = False
+        self.transaction_info = None
+        self.transaction_response = None
+
     def process_payment(self):
         # Init transaction
         self.transaction = self.create_transaction()
         self.transaction_type = self.create_transaction_type(settings.AUTHORIZE_NET_TRANSACTION_TYPE_DEFAULT)
         self.transaction_type.amount = self.to_valid_decimal(self.invoice.get_one_time_transaction_total())
         self.transaction_type.payment = self.create_authorize_payment()
         self.transaction_type.customer = self.create_customer_data()
@@ -568,15 +622,50 @@
 
         # Getting the response
         self.transaction_response = self.controller.getresponse()
         self.parse_response(self.parse_transaction_response)
         self.parse_success()
 
         if self.transaction_succeeded:
-            self.subscription_id = self.transaction_info['data'].get('subscription_id', "")
+            self.subscription_id = self.transaction_info['data'].get('subscriptionId', "")
+            if self.transaction_response.profile and 'authorizenet' not in self.invoice.profile.meta:
+                self.save_customer_profile_id(self.transaction_response.profile.customerProfileId.text)
+                self.save_customer_payment_profile_id(self.transaction_response.profile.customerPaymentProfileId.text)
+
+    def charge_customer_profile(self):
+        # Init transaction
+        self.transaction = self.create_transaction()
+        self.transaction_type = self.create_transaction_type(settings.AUTHORIZE_NET_TRANSACTION_TYPE_DEFAULT)
+        self.transaction_type.amount = self.to_valid_decimal(self.invoice.total)
+        self.transaction_type.payment = self.create_authorize_payment()
+        self.transaction_type.profile = self.create_customer_profile_charge()
+
+        # Optional items for make it easier to read and use on the Authorize.net portal.
+        if self.invoice.order_items:
+            self.transaction_type.lineItems = self.create_line_item_array(self.invoice.order_items.all())
+
+        # You set the request to the transaction
+        self.transaction.transactionRequest = self.transaction_type
+        self.controller = createTransactionController(self.transaction)
+        self.set_controller_api_endpoint()
+        self.controller.execute()
+
+        # You execute and get the response
+        self.transaction_response = self.controller.getresponse()
+        self.parse_response(self.parse_payment_response)
+        self.parse_success()
+
+        self.transaction_id = self.transaction_info['data'].get('transId', "")
+
+        if self.transaction_succeeded:
+            self.payment.status = PurchaseStatus.CAPTURED
+        else:
+            self.payment.status = PurchaseStatus.DECLINED
+
+        self.payment.save()
 
     def subscription_update_payment(self, subscription):
         """
         Updates the credit card information for the subscriptions in authorize.net
         and updates the payment record associated with the receipt.
         """
         self.transaction_type = apicontractsv1.ARBSubscriptionType()
@@ -790,14 +879,68 @@
             self.parse_success()
 
             if self.transaction_succeeded and self.transaction_response.paymentProfiles:
                 customer_profile_ids.extend([customer_profile.customerProfileId.text for customer_profile in self.transaction_response.paymentProfiles.paymentProfile])
 
         return customer_profile_ids
     
+    def get_customer_and_payment_id_for_expiring_cards(self, month):
+        paging = apicontractsv1.Paging()
+        paging.limit = 10
+        paging.offset = 1
+
+        sorting = apicontractsv1.CustomerPaymentProfileSorting()
+        sorting.orderBy = apicontractsv1.CustomerPaymentProfileOrderFieldEnum.id
+        sorting.orderDescending = "false"
+
+        self.transaction = apicontractsv1.getCustomerPaymentProfileListRequest()
+        self.transaction.merchantAuthentication = self.merchant_auth
+
+        self.transaction.searchType = apicontractsv1.CustomerPaymentProfileSearchTypeEnum.cardsExpiringInMonth
+        self.transaction.month = month
+        self.transaction.sorting = sorting
+        self.transaction.paging = paging
+
+        self.controller = getCustomerPaymentProfileListController(self.transaction)
+        self.controller.execute()
+
+        self.transaction_response = self.controller.getresponse()
+        self.parse_response(self.parse_transaction_response)
+        self.parse_success()
+
+        customer_profile_ids = []
+        last_page = 1
+        
+        if self.transaction_succeeded and self.transaction_response.paymentProfiles:
+            last_page = ceil(self.transaction_response.totalNumInResultSet.pyval / paging.limit)
+            customer_profile_ids.extend(
+                [{
+                "customerProfileId": customer_profile.customerProfileId.text,
+                "customerPaymentProfileId": self.transaction_response.paymentProfiles.paymentProfile.customerPaymentProfileId.text
+                } for customer_profile in self.transaction_response.paymentProfiles.paymentProfile])
+
+        for previous_page in range(1, last_page):
+            paging.offset = previous_page + 1
+
+            self.transaction.paging = paging
+            self.controller = getCustomerPaymentProfileListController(self.transaction)
+            self.controller.execute()
+            self.transaction_response = self.controller.getresponse()
+            self.parse_response(self.parse_transaction_response)
+            self.parse_success()
+
+            if self.transaction_succeeded and self.transaction_response.paymentProfiles:
+                customer_profile_ids.extend([{
+                    "customerProfileId": customer_profile.customerProfileId.text,
+                    "customerPaymentProfileId": self.transaction_response.paymentProfiles.paymentProfile.customerPaymentProfileId.text}
+                    for customer_profile in self.transaction_response.paymentProfiles.paymentProfile
+                ])
+
+        return customer_profile_ids
+    
     def get_customer_email(self, customer_id):
         self.transaction = apicontractsv1.getCustomerProfileRequest()
         self.transaction.merchantAuthentication = self.merchant_auth
         self.transaction.customerProfileId = customer_id
 
         self.controller = getCustomerProfileController(self.transaction)
         self.controller.execute()
@@ -816,28 +959,93 @@
         successfull_transactions = []
 
         if not batch_list:
             return []
         
         for batch in batch_list:
             transaction_list = self.get_transaction_batch_list(str(batch.batchId))
-            successfull_transactions.extend([ transaction for transaction in transaction_list if transaction['transactionStatus'] == 'settledSuccessfully' ])
+            successfull_transactions.extend([transaction for transaction in transaction_list if transaction['transactionStatus'] == 'settledSuccessfully'])
 
         return successfull_transactions
     
     def update_payments_to_settled(self, site, settled_transactions):
         for settled_transaction in settled_transactions:
             try:
                 payment = Payment.objects.get(profile__site=site, transaction=settled_transaction.transId.text)
                 payment.status = PurchaseStatus.SETTLED
                 payment.submitted_date = settled_transaction.submitTimeUTC.pyval
                 payment.save()
-            except ObjectDoesNotExist as exce:
+            except ObjectDoesNotExist:
                 logger.error(f"update_payments_to_settled payment for transaction: {settled_transaction.transId.text} was not found for site: {site}")
+            except MultipleObjectsReturned:
+                logger.error(f"update_payments_to_settled multiple objects returned for transaction: {settled_transaction.transId.text}")
+                payment = Payment.objects.filter(profile__site=site, transaction=settled_transaction.transId.text).first()
+                payment.status = PurchaseStatus.SETTLED
+                payment.submitted_date = settled_transaction.submitTimeUTC.pyval
+                payment.save()
+
+    def create_customer_profile_by_transaction(self, transaction_id):
+        self.transaction = apicontractsv1.createCustomerProfileFromTransactionRequest()
+        self.transaction.merchantAuthentication = self.merchant_auth
+        self.transaction.transId = transaction_id
 
+        self.controller = createCustomerProfileFromTransactionController(self.transaction)
+        self.set_controller_api_endpoint()
+        self.controller.execute()
+
+        self.transaction_response = self.controller.getresponse()
+        self.parse_response(self.parse_transaction_response)
+        self.parse_success()
+
+        if self.transaction_succeeded:
+            if self.transaction_response.customerProfileId:
+                self.save_customer_profile_id(self.transaction_response.customerProfileId.text)
+                self.save_customer_payment_profile_id(self.transaction_response.customerPaymentProfileIdList[0].numericString.text)
+
+    def create_customer_profile(self):
+        self.transaction = apicontractsv1.createCustomerProfileRequest()
+        self.transaction.merchantAuthentication = self.merchant_auth
+        self.transaction.profile = self.create_customer_profile_data()
+
+        self.controller = createCustomerProfileController(self.transaction)
+        self.set_controller_api_endpoint()
+        self.controller.execute()
+
+        self.transaction_response = self.controller.getresponse()
+        self.parse_response(self.parse_transaction_response)
+        self.parse_success()
+
+        if self.transaction_succeeded:
+            if self.transaction_response.customerProfileId:
+                self.save_customer_profile_id(self.transaction_response.customerProfileId.text)
+        else:
+            logger.error(f"create_customer_profile error {self.transaction_info['errors']}")
+
+    def create_customer_profile_payment_id(self, customer_profile_id):
+        self.transaction = apicontractsv1.createCustomerPaymentProfileRequest()
+        self.transaction.merchantAuthentication = self.merchant_auth
+        self.transaction.paymentProfile = apicontractsv1.customerPaymentProfileType()
+        self.transaction.customerProfileId = customer_profile_id
+        
+        self.transaction.paymentProfile.payment = self.create_authorize_payment()
+        self.transaction.paymentProfile.payment.creditCard = self.create_credit_card_payment()
+        self.transaction.paymentProfile.billTo = self.create_billing_address(apicontractsv1.customerAddressType())
+        self.transaction.validationMode = 'liveMode'
+
+        self.controller = createCustomerPaymentProfileController(self.transaction)
+        self.set_controller_api_endpoint()
+        self.controller.execute()
+
+        self.transaction_response = self.controller.getresponse()
+        self.parse_response(self.parse_transaction_response)
+        self.parse_success()
+
+        if self.transaction_succeeded:
+            if self.transaction_response.customerProfileId:
+                self.save_customer_payment_profile_id(self.transaction_response.customerPaymentProfileId.text)
 
     ##########
     # Reporting API, for transaction retrieval information
     ##########
     def get_settled_batch_list(self, start_date, end_date):
         """
         Gets a list of batches for settled transaction between the start and end date.
@@ -999,15 +1207,15 @@
 
                         if payment_status == PurchaseStatus.SETTLED:
                             ### Create Receipt.
                             receipt = Receipt()
                             receipt.profile = customer_profile
                             receipt.order_item = invoice.order_items.first()
                             receipt.start_date = submitted_datetime
-                            receipt.end_date = get_payment_scheduled_end_date(offer, start_date=submitted_datetime)
+                            receipt.end_date = offer.get_offer_end_date(start_date=submitted_datetime)
                             receipt.transaction = payment.transaction
                             receipt.subscription = subscription
                             receipt.meta.update(payment.result)
                             receipt.meta['payment_amount'] = payment.amount
                             receipt.save()
                             
                             receipt.products.add(offer.products.first())
@@ -1046,15 +1254,15 @@
                         if Receipt.objects.filter(deleted=False, transaction=transaction_id, profile=customer_profile).count():
                             receipt = Receipt.objects.get(deleted=False, transaction=transaction_id, profile=customer_profile)
                             
                             if payment.status == PurchaseStatus.SETTLED:
                                 receipt.profile = customer_profile
                                 receipt.order_item = invoice.order_items.first()
                                 receipt.start_date = submitted_datetime
-                                receipt.end_date = get_payment_scheduled_end_date(offer, start_date=submitted_datetime)
+                                receipt.end_date = offer.get_offer_end_date(start_date=submitted_datetime)
                                 receipt.transaction = payment.transaction
                                 receipt.subscription = subscription
                                 receipt.meta.update(payment.result)
                                 receipt.meta['payment_amount'] = payment.amount
                                 receipt.save()
                                 
                                 receipt.products.add(offer.products.first())
@@ -1151,10 +1359,10 @@
                 receipt.transaction = payment.transaction
                 receipt.meta.update(payment.result)
                 receipt.meta['payment_amount'] = payment.amount
                 receipt.start_date = submitted_datetime
                 receipt.save()
 
                 receipt.products.add(offer.products.first())
-                receipt.end_date = get_payment_scheduled_end_date(offer, start_date=receipt.start_date)
+                receipt.end_date = offer.get_offer_end_date(start_date=receipt.start_date)
                 receipt.subscription = subscription
                 receipt.save()
```

### Comparing `django-vendor-0.3.9/vendor/processors/base.py` & `django-vendor-0.4.0/src/vendor/processors/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
 Base Payment processor used by all derived processors.
 """
 import django.dispatch
 
+from datetime import timedelta
 from decimal import Decimal, ROUND_DOWN
 from django.conf import settings
 from django.utils import timezone
 
 from vendor import config
 from vendor.forms import CreditCardForm, BillingAddressForm
 from vendor.models import Payment, Invoice, Receipt, Subscription
 from vendor.models.choice import PurchaseStatus, SubscriptionStatus, TermType, InvoiceStatus, PaymentTypes
-from vendor.utils import get_payment_scheduled_end_date, get_subscription_start_date, get_future_date_days
 
 ##########
 # SIGNALS
 vendor_pre_authorization = django.dispatch.Signal()
 vendor_process_payment = django.dispatch.Signal()
 vendor_post_authorization = django.dispatch.Signal()
 vendor_subscription_cancel = django.dispatch.Signal()
@@ -34,14 +34,15 @@
     invoice = None
     provider = None
     # TODO: Change payment to a list as an invoice can have multiple payment. EG: 1 for 1 type purchases and n for any amount of subscriptions. 
     payment = None
     subscription = None
     subscription_id = None
     receipt = None
+    trial_receipt = None
     payment_info = {}
     billing_address = {}
     transaction_token = None
     transaction_id = ""
     transaction_succeeded = False
     transaction_info = {}
     transaction_response = None
@@ -189,72 +190,94 @@
         today = timezone.now()
         self.receipt = Receipt()
         self.receipt.profile = self.invoice.profile
         self.receipt.order_item = order_item
         self.receipt.transaction = self.payment.transaction
         self.receipt.meta.update(self.payment.result)
         self.receipt.meta['payment_amount'] = self.payment.amount
-        start_date = order_item.offer.get_term_start_date(today)
-        self.receipt.start_date = get_subscription_start_date(order_item.offer, self.invoice.profile, start_date)
+
+        if today > (self.payment.submitted_date - timedelta(hours=1)) or today < (self.payment.submitted_date + timedelta(hours=1)):
+            start_date = order_item.offer.get_offer_start_date(self.payment.submitted_date)
+        else:
+            start_date = order_item.offer.get_offer_start_date(today)
+
+
+        if self.trial_receipt:
+            start_date = self.trial_receipt.end_date
+
+        self.receipt.start_date = start_date
         self.receipt.save()
 
         if term_type < TermType.PERPETUAL:
-            self.receipt.end_date = get_payment_scheduled_end_date(order_item.offer, self.receipt.start_date)
+            self.receipt.end_date = order_item.offer.get_offer_end_date(self.receipt.start_date)
             self.receipt.subscription = self.subscription
             
         self.receipt.save()
 
     def create_trial_receipt_payment(self, order_item):
-        if self.invoice.profile.has_owned_product(order_item.offer.products.all()):
-            return None  # Trial receipts are only created if the user has not owned the product previously 
+        today = timezone.now()
 
-        if not order_item.offer.get_trial_days():
-            return None
+        if today > (self.payment.submitted_date - timedelta(hours=1)) or today < (self.payment.submitted_date + timedelta(hours=1)):
+            start_date = order_item.offer.get_offer_start_date(self.payment.submitted_date)
+        else:
+            start_date = order_item.offer.get_offer_start_date(today)
 
-        start_date = order_item.offer.get_term_start_date()
+        end_date = order_item.offer.get_trial_end_date(start_date)
 
-        self.payment = Payment.objects.create(
+        if end_date == start_date:
+            self.trial_payment = None
+            self.trial_receipt = None
+            return None   # There is something wrong if both start and end date are the same
+
+        self.trial_payment, created = Payment.objects.get_or_create(
             profile=self.invoice.profile,
-            amount=0,
+            amount=order_item.offer.get_trial_amount(),
             provider=self.provider,
             invoice=self.invoice,
-            submitted_date=start_date,
-            success=True,
-            status=PurchaseStatus.SETTLED,
-            payee_full_name=" ".join([self.invoice.profile.user.first_name, self.invoice.profile.user.last_name])
+            defaults={
+                "submitted_date": start_date,
+                "payee_full_name": " ".join([self.invoice.profile.user.first_name, self.invoice.profile.user.last_name])
+            }
         )
         
-        self.payment.transaction = f"{self.payment.uuid}-trial"
-        self.payment.save()
+        self.trial_payment.transaction = f"{self.trial_payment.uuid}-trial"
+        self.trial_payment.status = PurchaseStatus.SETTLED
+        self.trial_payment.success = True
+        self.trial_payment.save()
 
-        self.receipt = Receipt.objects.create(
+        self.trial_receipt = Receipt.objects.create(
             profile=self.invoice.profile,
             order_item=order_item,
-            transaction=self.payment.transaction,
+            transaction=self.trial_payment.transaction,
             start_date=start_date,
-            end_date=get_future_date_days(start_date, order_item.offer.get_trial_days()),
+            end_date=end_date,
             subscription=self.subscription
         )
 
         if order_item.offer.terms < TermType.PERPETUAL:
-            self.payment.subscription = self.subscription
-            self.payment.save()
+            self.trial_payment.subscription = self.subscription
+            self.trial_payment.save()
             
-            self.receipt.subscription = self.subscription
-            self.receipt.save()
+            self.trial_receipt.subscription = self.subscription
+            self.trial_receipt.save()
             
     def create_order_item_receipt(self, order_item):
         """
         Creates a receipt for every product in the order item according to its,
         offering term type.
         """
         for product in order_item.offer.products.all():
-            self.create_receipt_by_term_type(order_item, order_item.offer.terms)
-            self.create_trial_receipt_payment(order_item)
-            self.receipt.products.add(product)
+            if (order_item.offer.has_trial() or order_item.offer.has_valid_billing_start_date()) and\
+                not self.invoice.profile.has_owned_product(order_item.offer.products.all()):
+                self.create_trial_receipt_payment(order_item)
+                if self.trial_receipt:
+                    self.trial_receipt.products.add(product)
+            else:
+                self.create_receipt_by_term_type(order_item, order_item.offer.terms)
+                self.receipt.products.add(product)
 
     def create_receipts(self, order_items):
         """
         It then creates receipt for the order items supplied.
         """
         for order_item in order_items.all():
             self.create_order_item_receipt(order_item)
@@ -377,17 +400,14 @@
 
         if self.invoice.get_recurring_order_items():
             self.process_subscriptions()
 
         vendor_post_authorization.send(sender=self.__class__, invoice=self.invoice)
         self.post_authorization()
 
-
-        #TODO: Set the status based on the result from the process_payment()
-
     def pre_authorization(self):
         """
         Called before the authorization begins.
         """
         pass
 
     def process_payment(self):
@@ -403,15 +423,16 @@
         Called to handle an invoice with total zero.
         This are the base internal steps to process a free payment.
         """
         self.payment = Payment(profile=self.invoice.profile,
                                amount=self.invoice.total,
                                provider=self.provider,
                                invoice=self.invoice,
-                               created=timezone.now()
+                               created=timezone.now(),
+                               submitted_date=timezone.now()
                                )
         self.payment.save()
         self.transaction_succeeded = True
         self.payment.success = True
         self.payment.status = PurchaseStatus.SETTLED
         self.payment.transaction = f"{self.payment.uuid}-free"
         self.payment.payee_full_name = " ".join([self.invoice.profile.user.first_name, self.invoice.profile.user.last_name])
@@ -463,15 +484,16 @@
                 self.create_order_item_receipt(subscription)
 
     def subscription_payment(self, subscription):
         """
         Call handels the authrization and creation for a subscription.
         """
         # Gateway Transaction goes here...
-        pass
+        self.subscription_id = 'Test ID'
+        ...
 
     def create_subscription_model(self):
         self.subscription = Subscription.objects.create(
             gateway_id=self.subscription_id,
             profile=self.invoice.profile,
             auto_renew=True,
             status=SubscriptionStatus.ACTIVE
@@ -496,33 +518,32 @@
         subscription.cancel()
         vendor_subscription_cancel.send(sender=self.__class__, subscription=subscription)
 
     def is_card_valid(self):
         """
         Function to validate a credit card by method of makeing a microtransaction and voiding it if authorized.
         """
-        pass
+        return True
 
-    def renew_subscription(self, subscription, payment_transaction_id="", payment_status=PurchaseStatus.QUEUED, payment_success=True):
+    def renew_subscription(self, subscription, payment_transaction_id="", payment_status=PurchaseStatus.QUEUED, payment_success=True, submitted_date=timezone.now()):
         """
         Function to renew already paid subscriptions form the payment gateway provider.
         """
         self.subscription = subscription
-        submitted_date = timezone.now()
 
         self.payment = Payment.objects.create(
             profile=subscription.profile,
             invoice=self.invoice,
             transaction=payment_transaction_id,
             submitted_date=submitted_date,
             subscription=subscription,
             amount=self.invoice.total,
             success=payment_success,
             status=payment_status,
-            payee_full_name = " ".join([self.invoice.profile.user.first_name, self.invoice.profile.user.last_name])
+            payee_full_name=" ".join([self.invoice.profile.user.first_name, self.invoice.profile.user.last_name])
         )
 
         self.create_receipts(self.invoice.order_items.all())
 
     def subscription_update_price(self, subscription, new_price, user):
         """
         Call to handle when a new subscription price needs to be approved.
@@ -545,16 +566,57 @@
             subscription=subscription,
             profile=self.invoice.profile,
             amount=self.invoice.total,
             provider=self.provider,
             invoice=self.invoice,
             submitted_date=self.invoice.ordered_date,
             transaction=transaction_id,
-            status = PurchaseStatus.DECLINED,
+            status=PurchaseStatus.DECLINED,
             payee_full_name=" ".join([self.invoice.profile.user.first_name, self.invoice.profile.user.last_name])
         )
 
+    # -------------------
+    # Charge a Customer Profile
+    def charge_customer_profile(self):
+        """
+        Each processor need to implement this functions
+        """
+        ...
+        
+    def process_customer_profile_payment(self):
+        """
+        This runs the chain of events in a transaction.
+        This should not be overriden.  Override one of the methods it calls if you need to.
+        """
+        self.invoice.ordered_date = timezone.now()
+        self.invoice.save()
+        if not self.invoice.calculate_subtotal():
+            self.free_payment()
+            return None
+
+        if not self.is_data_valid():
+            return None
+
+        self.status = PurchaseStatus.QUEUED     # TODO: Set the status on the invoice.  Processor status should be the invoice's status.
+        vendor_pre_authorization.send(sender=self.__class__, invoice=self.invoice)
+
+        self.pre_authorization()
+
+        self.status = PurchaseStatus.ACTIVE     # TODO: Set the status on the invoice.  Processor status should be the invoice's status.
+        vendor_process_payment.send(sender=self.__class__, invoice=self.invoice)
+
+        self.create_payment_model()
+        self.charge_customer_profile()
+        self.save_payment_transaction_result()
+        self.update_invoice_status(InvoiceStatus.COMPLETE)
+        if self.is_transaction_and_invoice_complete():
+            self.invoice.save_discounts_vendor_notes()
+            self.create_receipts(self.invoice.get_one_time_transaction_order_items())
+
+        vendor_post_authorization.send(sender=self.__class__, invoice=self.invoice)
+        self.post_authorization()
+
     ##########
     # Signals
     ##########
     def customer_card_expired(self, site, email):
         vendor_customer_card_expiring.send(sender=self.__class__, site_pk=site.pk, email=email)
```

### Comparing `django-vendor-0.3.9/vendor/processors/stripe_processor.py` & `django-vendor-0.4.0/src/vendor/processors/stripe_processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-"""
-Payment processor for Stripe.
-"""
 import json
 import logging
 import stripe
 
 from math import modf
 from django.conf import settings
 from django.utils import timezone
@@ -14,17 +11,17 @@
 from vendor.models.choice import (
     Country,
     TermType,
     TermDetailUnits,
 )
 from vendor.processors.base import PaymentProcessorBase
 
-
 logger = logging.getLogger(__name__)
 
+
 class StripeQueryBuilder:
     """
     Query builder that adheres to Stripe search rules found here https://stripe.com/docs/search
 
     Ex:
     To generate a query like 'name:"Johns Offer" AND metadata["site"]:"site4"'
 
@@ -193,15 +190,14 @@
 
             else:
                 logger.error(f'StripeQueryBuilder.build_search_query: {field} is not valid for {stripe_object_class}')
                 return query
 
         return query
 
-
 class StripeProcessor(PaymentProcessorBase):
     """ 
     Implementation of Stripe SDK
     https://self.stripe.com/docs/api/authentication?lang=python
     """
 
     TRANSACTION_SUCCESS_MESSAGE = 'message'
@@ -241,15 +237,15 @@
 
         if not stripe_customer:
             self.create_stripe_customers([self.invoice.profile])
 
     def subscription_offer_setup(self):
         offers_to_sync = []
         for order_item in self.invoice.order_items.all():
-            if not order_item.offer.meta.get('stripe_id'):
+            if not order_item.offer.meta.get('stripe'):
                 offers_to_sync.append(order_item.offer)
 
         self.create_offers(offers_to_sync)
 
     ##########
     # Parsers
     ##########
@@ -527,47 +523,51 @@
             }
         }
 
     def build_payment_intent(self, amount, currency=DEFAULT_CURRENCY):
         return {
             'amount': amount,
             'currency': currency,
+            'customer': self.invoice.profile.meta['stripe_id'],
             'application_fee_percent': self.get_application_fee_amount(),
-            'transfer_data': self.get_stripe_connect_account()
+            'transfer_data': self.get_stripe_connect_account(),
+            'on_behalf_of': self.get_stripe_connect_account()
         }
 
     def build_setup_intent(self, payment_method_id):
         return {
             'customer': self.invoice.profile.meta['stripe_id'],
             'confirm': True,
             'payment_method_types': ['card'],
             'payment_method': payment_method_id,
-            'metadata': {'site': self.invoice.site}
+            'metadata': {'site': self.invoice.site},
+            'on_behalf_of': self.get_stripe_connect_account()
         }
     
     def build_subscription(self, subscription, payment_method_id):
         return {
             'customer': self.invoice.profile.meta['stripe_id'],
-            'coupon': subscription.offer.meta['stripe'].get('coupon_id'),
+            'promotion_code': self.invoice.coupon_code.first().meta['stripe_id'] if self.invoice.coupon_code.count() else None,
             'items': [{'price': subscription.offer.meta['stripe']['price_id']}],
             'default_payment_method': payment_method_id,
             'metadata': {'site': self.invoice.site},
             'trial_period_days': subscription.offer.get_trial_days(),
             'application_fee_percent': self.get_application_fee_percent(),
-            'transfer_data': self.build_transfer_data()
+            'transfer_data': self.build_transfer_data(),
+            'on_behalf_of': self.get_stripe_connect_account()
         }
 
     def build_invoice_line_item(self, order_item, invoice_id):
         line_item = {
             'customer': self.invoice.profile.meta.get('stripe_id'),
             'invoice': invoice_id,
             'price': order_item.offer.meta['stripe'].get('price_id'),
         }
 
-        if order_item.offer.has_any_discount_or_trial():
+        if order_item.offer.has_trial() or order_item.offer.has_valid_billing_start_date() or order_item.offer.discount():
             line_item['discounts'] = [{'coupon': order_item.offer.meta['stripe'].get('coupon_id')}]
 
         return line_item
 
     def build_invoice(self, currency=DEFAULT_CURRENCY):
         return {
             'customer': self.invoice.profile.meta.get('stripe_id'),
@@ -638,14 +638,23 @@
 
             if existing_stripe_customer:
                 profile_meta = profile.meta
                 profile_meta['stripe_id'] = existing_stripe_customer['id']
                 CustomerProfile.objects.filter(pk=profile.pk).update(meta=profile_meta)
             else:
                 self.create_stripe_customers([profile])
+    
+    def get_customer_payment_methods(self, customer_id):
+        payment_methods = self.stripe_call(self.stripe.Customer.list_payment_methods, customer_id)
+
+        if not payment_methods.data:
+            return None
+
+        return payment_methods.data
+    
     ##########
     # Offers/Products
     ##########
     def does_product_exist(self, name, metadata):
         name_clause = self.query_builder.make_clause_template(
             field='name',
             value=name,
@@ -811,15 +820,15 @@
                         offer_meta['stripe']['price_id'] = stripe_price['id']
                     else:
                         offer_meta['stripe'] = {'price_id': stripe_price['id']}
 
                 # Handle Coupon
                 coupon_data = self.build_coupon(offer, DEFAULT_CURRENCY)
                 discount = self.convert_decimal_to_integer(offer.discount())
-                trial_days = offer.term_details.get('trial_days', 0)
+                trial_days = offer.get_trial_days()
 
                 # If this offer has a discount check if its on stripe to create, update, delete
                 if discount or trial_days:
                     stripe_coupon_matches = self.match_coupons(coupons, offer)
                     if not stripe_coupon_matches:
                         stripe_coupon = self.stripe_create_object(self.stripe.Coupon, coupon_data)
                     elif len(stripe_coupon_matches) == 1:
@@ -1195,22 +1204,21 @@
         if not stripe_payment_method:
             return None
 
         self.stripe_call(stripe_payment_method.attach, {'customer': self.invoice.profile.meta.get('stripe_id')})
         if not self.transaction_succeeded:
             return None
         
-        stripe_invoice
         self.invoice.vendor_notes['stripe_id'] = stripe_invoice.id
         self.invoice.save()
         
         stripe_line_items = []
         for order_item in self.invoice.get_one_time_transaction_order_items():
             line_item_data = self.build_invoice_line_item(order_item, stripe_invoice.id)
-            stripe_line_item = self.stripe_create_object(self.stripe.InvoiceItem, line_item_data) 
+            stripe_line_item = self.stripe_create_object(self.stripe.InvoiceItem, line_item_data)
             stripe_line_items.append(stripe_line_item)
         
         stripe_invoice.lines = stripe_line_items
 
         amount = self.convert_decimal_to_integer(self.invoice.get_one_time_transaction_total())
         payment_intent_data = self.build_payment_intent(amount)
         stripe_payment_intent = self.stripe_create_object(self.stripe.PaymentIntent, payment_intent_data)
@@ -1233,23 +1241,127 @@
         if not setup_intent_object:
             return None
 
         stripe_setup_intent = self.stripe_create_object(self.stripe.SetupIntent, setup_intent_object)
         if not stripe_setup_intent:
             return None
 
-        subscription_obj = self.build_subscription(subscription, stripe_payment_method.id)        
+        subscription_obj = self.build_subscription(subscription, stripe_payment_method.id)
         stripe_subscription = self.stripe_create_object(self.stripe.Subscription, subscription_obj)
         
         if not stripe_subscription or stripe_subscription.status == 'incomplete':
             self.transaction_succeeded = False
-            self.transaction_info['errors'] = "Subscription was not settled"
             return None
 
         if self.invoice.vendor_notes is None:
             self.invoice.vendor_notes = {}
 
         self.invoice.vendor_notes['stripe_id'] = stripe_subscription.latest_invoice
         self.invoice.save()
 
         self.subscription_id = stripe_subscription.id
 
+    def charge_customer_profile(self):
+        invoice_data = self.build_invoice()
+        stripe_invoice = self.stripe_create_object(self.stripe.Invoice, invoice_data)
+        if not stripe_invoice:
+            return None
+
+        stripe_customer_payment_methods = self.get_customer_payment_methods(self.invoice.profile.meta['stripe_id'])
+        if not stripe_customer_payment_methods:
+            return None
+        
+        self.invoice.vendor_notes['stripe_id'] = stripe_invoice.id
+        self.invoice.save()
+        
+        stripe_line_items = []
+        for order_item in self.invoice.get_one_time_transaction_order_items():
+            line_item_data = self.build_invoice_line_item(order_item, stripe_invoice.id)
+            stripe_line_item = self.stripe_create_object(self.stripe.InvoiceItem, line_item_data)
+            stripe_line_items.append(stripe_line_item)
+        
+        stripe_invoice.lines = stripe_line_items
+
+        amount = self.convert_decimal_to_integer(self.invoice.get_one_time_transaction_total())
+        payment_intent_data = self.build_payment_intent(amount)
+        stripe_payment_intent = self.stripe_create_object(self.stripe.PaymentIntent, payment_intent_data)
+
+        if not stripe_payment_intent:
+            return None
+
+        self.stripe_call(stripe_invoice.pay, {"payment_method": stripe_customer_payment_methods[0].id})
+
+        if self.transaction_succeeded:
+            self.transaction_id = stripe_invoice.payment_intent
+
+    def subscription_cancel(self, subscription):
+        super().subscription_cancel(subscription)
+        self.stripe_delete_object(self.stripe.Subscription, subscription.gateway_id)
+
+    def subscription_update_payment(self, subscription):
+        """
+        Updates the credit card information for the subscription in stripe
+        and updates the subscription model in vendor.
+        """
+
+        stripe_subscription_object = self.stripe_get_object(self.stripe.Subscription, subscription.gateway_id)
+        if not stripe_subscription_object:
+            return None
+
+        current_payment_method = self.stripe.Customer.retrieve_payment_method(
+            stripe_subscription_object.customer,
+            stripe_subscription_object.default_payment_method
+        )
+
+        payment_method_data = {
+            'type': 'card',
+            'card': {
+                'number': self.payment_info.cleaned_data.get('card_number'),
+                'exp_month': self.payment_info.cleaned_data.get('expire_month'),
+                'exp_year': self.payment_info.cleaned_data.get('expire_year'),
+                'cvc': self.payment_info.cleaned_data.get('cvv_number'),
+            },
+            'billing_details': {
+                'name': self.payment_info.cleaned_data.get('full_name', None),
+                'email': subscription.profile.user.email
+            }
+        }
+        # keep previous address
+        if current_payment_method:
+            payment_method_data['billing_details']['address'] = current_payment_method.billing_details.get("address")
+
+        # create payment method using new card
+        stripe_payment_method = self.stripe_create_object(self.stripe.PaymentMethod, payment_method_data)
+        if not stripe_payment_method:
+            return None
+
+        setup_intent_object = {
+            'customer': subscription.profile.meta['stripe_id'],
+            'confirm': True,
+            'payment_method_types': ['card'],
+            'payment_method': stripe_payment_method.id,
+            'metadata': {'site': subscription.profile.site}
+        }
+
+        # validate
+        stripe_setup_intent = self.stripe_create_object(self.stripe.SetupIntent, setup_intent_object)
+        if not stripe_setup_intent:
+            return None
+
+        # update subscription
+        self.stripe.Subscription.modify(
+            subscription.gateway_id,
+            default_payment_method=stripe_payment_method
+        )
+
+        # save payment info to subscription model
+        payment_info = {}
+        account_number = payment_method_data.get("card", {}).get("number", "")[-4:]
+        account_type = stripe_payment_method.card.get("brand", "")
+
+        if account_number:
+            payment_info['account_number'] = account_number
+
+        if account_type:
+            payment_info['account_type'] = account_type
+
+        subscription.save_payment_info(payment_info)
```

### Comparing `django-vendor-0.3.9/vendor/signals/stripe_signals.py` & `django-vendor-0.4.0/src/vendor/signals/stripe_signals.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/tests/__init__.py` & `django-vendor-0.4.0/src/vendor/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/tests/test_authorizenet.py` & `django-vendor-0.4.0/src/vendor/tests/test_authorizenet.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+from uuid import uuid4
 from core.models import Product
 from datetime import timedelta
 
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.contrib.sites.models import Site
 from django.utils import timezone
 from django.urls import reverse
 from django.test import TestCase, Client, tag
 
 from unittest import skipIf
 from random import randrange, choice
 from siteconfigs.models import SiteConfigModel
+from vendor.api.v1.authorizenet.views import subscription_save_transaction, update_payment
 from vendor.forms import CreditCardForm, BillingAddressForm
 from vendor.models import Invoice, Payment, Offer, Price, Receipt, CustomerProfile, OrderItem, Subscription
 from vendor.models.choice import PurchaseStatus, InvoiceStatus, SubscriptionStatus
 from vendor.processors import PaymentProcessorBase, AuthorizeNetProcessor
 
 User = get_user_model()
 
@@ -671,16 +673,16 @@
 
         self.processor.authorize_payment()
 
         # print(self.processor.transaction_info)
         self.assertTrue(self.processor.transaction_succeeded)
         self.assertIn('subscriptionId', self.processor.transaction_info['data'])
         self.assertIsNotNone(self.processor.subscription)
-        self.assertFalse(self.processor.payment.transaction)
-        self.assertFalse(self.processor.receipt.transaction)
+        self.assertTrue(self.processor.payment.transaction)
+        self.assertTrue(self.processor.receipt.transaction)
 
     def test_subscription_update_payment(self):
         self.form_data['credit_card_form']['card_number'] = choice(self.VALID_CARD_NUMBERS)
         subscription_list = self.processor.get_list_of_subscriptions()
 
         if not len(subscription_list):
             print("No subscriptions, Skipping Test")
@@ -790,17 +792,16 @@
         price.save()
         self.existing_invoice.update_totals()
         self.existing_invoice.save()
         self.form_data['credit_card_form']['card_number'] = choice(self.VALID_CARD_NUMBERS)
         self.processor = AuthorizeNetProcessor(self.site, self.existing_invoice)
         self.processor.set_billing_address_form_data(self.form_data.get('billing_address_form'), BillingAddressForm)
         self.processor.set_payment_info_form_data(self.form_data.get('credit_card_form'), CreditCardForm)
-        self.processor.is_data_valid()
-        self.processor.create_payment_model()
         is_valid = self.processor.is_card_valid()
+        self.processor.create_payment_model()
         print(f"Test is_card_valid_success\n")
         print(f"Transaction Submitted: {self.processor.transaction_succeeded}")
         print(f"Transaction Response: {self.processor.transaction_response}")
         print(f"Transaction Msg: {self.processor.transaction_info}")
         if 'duplicate' in str(self.processor.transaction_info):
             print(f"Skipping Test test_is_card_valid_success because of duplicate")
             return None
@@ -831,27 +832,86 @@
             response = self.processor.subscription_info(subscription.gateway_id)
             self.assertTrue(self.processor.transaction_succeeded)
             self.assertEqual(new_price, response.subscription.amount.pyval)
         else:
             print("No active Subscriptions, Skipping Test")
 
     ##########
+    # Charge Customer Profile Tests
+    ##########
+    def test_create_customer_profile(self):
+        self.processor.set_billing_address_form_data(self.form_data.get('billing_address_form'), BillingAddressForm)
+        self.processor.set_payment_info_form_data(self.form_data.get('credit_card_form'), CreditCardForm)
+        self.processor.is_data_valid()
+        self.processor.create_customer_profile()
+
+        self.assertIn('authorizenet', self.processor.invoice.profile.meta)
+        self.assertTrue(self.processor.get_customer_profile_id())
+
+    def test_create_customer_payment_profile(self):
+        self.processor.set_billing_address_form_data(self.form_data.get('billing_address_form'), BillingAddressForm)
+        self.processor.set_payment_info_form_data(self.form_data.get('credit_card_form'), CreditCardForm)
+        self.processor.is_data_valid()
+        self.processor.create_customer_profile()
+        self.processor.create_customer_profile_payment_id(self.processor.get_customer_profile_id())
+
+        self.assertIn('authorizenet', self.processor.invoice.profile.meta)
+        self.assertTrue(self.processor.get_customer_payment_profile_id())
+
+    def test_charge_customer_profile(self):
+        self.processor.set_billing_address_form_data(self.form_data.get('billing_address_form'), BillingAddressForm)
+        self.processor.set_payment_info_form_data(self.form_data.get('credit_card_form'), CreditCardForm)
+        
+        self.processor.invoice.total = randrange(1, 1000)
+        for recurring_order_items in self.processor.invoice.get_recurring_order_items():
+            self.processor.invoice.remove_offer(recurring_order_items.offer)
+
+        customer_profiles = self.processor.get_customer_and_payment_id_for_expiring_cards("2024-01")
+
+        self.processor.invoice.profile.meta = {}
+        self.processor.invoice.profile.meta['authorizenet'] = {}
+        self.processor.invoice.profile.meta['authorizenet']['customerProfileId'] = customer_profiles[0]['customerProfileId']
+        self.processor.invoice.profile.meta['authorizenet']['customerPaymentProfileId'] = customer_profiles[0]['customerPaymentProfileId']
+        self.processor.invoice.profile.save()
+        self.processor.is_data_valid()
+
+        self.processor.process_customer_profile_payment()
+
+        self.assertTrue(self.processor.transaction_succeeded)
+    
+    def test_create_customer_profile_by_transaction(self):
+        self.processor.set_billing_address_form_data(self.form_data.get('billing_address_form'), BillingAddressForm)
+        self.processor.set_payment_info_form_data(self.form_data.get('credit_card_form'), CreditCardForm)
+        
+        self.processor.invoice.total = randrange(1, 1000)
+        for recurring_order_items in self.processor.invoice.get_recurring_order_items():
+            self.processor.invoice.remove_offer(recurring_order_items.offer)
+
+        self.processor.is_data_valid()
+        self.processor.authorize_payment()
+
+        self.processor.create_customer_profile_by_transaction(self.processor.payment.transaction)
+
+        self.assertIn('authorizenet', self.processor.invoice.profile.meta)
+    
+    ##########
     # Report details
     ##########
     def test_get_transaction_details(self):
         transaction_id = '60160039986'
         self.processor = AuthorizeNetProcessor(self.site, self.existing_invoice)
         transaction_detail = self.processor.get_transaction_detail(transaction_id)
         self.assertTrue(transaction_detail)
 
     def test_get_settled_transaction(self):
         start_date, end_date = (timezone.now() - timedelta(days=3)), timezone.now()
         settled_transactions = self.processor.get_settled_transactions(start_date, end_date)
 
         self.assertTrue(settled_transactions)
+    
     ##########
     # Transaction View Tests
     ##########
     def test_view_checkout_account_success_code(self):
         response = self.client.get(reverse("vendor:checkout-account"))
 
         self.assertEquals(response.status_code, 200)
@@ -912,8 +972,79 @@
         ids = processor.get_customer_id_for_expiring_cards("2023-01")
         emails = []
 
         for cp_id in ids:
             emails.append(processor.get_customer_email(cp_id))
 
         self.assertTrue(emails)
-        
+    
+    ##########
+    # AutheCaputre functions
+    ##########
+    def test_subscription_save_transaction_success(self):
+        subscription = Subscription.objects.get(gateway_id="7127667")
+        transaction_id = '40060834171'
+        self.processor = AuthorizeNetProcessor(self.site, self.existing_invoice)
+        transaction_detail = self.processor.get_transaction_detail(transaction_id)
+        subscription_save_transaction(self.site, transaction_id, transaction_detail)
+
+        self.assertTrue(subscription.receipts.count())
+
+    def test_subscription_save_transaction_multiple_subscriptions(self):
+        subscription = Subscription.objects.get(gateway_id="7127667")
+        sub_a = Subscription.objects.create(
+            gateway_id="7127667",
+            profile=self.existing_invoice.profile,
+            status=SubscriptionStatus.ACTIVE
+        )
+        transaction_id = '40060834171'
+        self.processor = AuthorizeNetProcessor(self.site, self.existing_invoice)
+        transaction_detail = self.processor.get_transaction_detail(transaction_id)
+        subscription_save_transaction(self.site, transaction_id, transaction_detail)
+
+        self.assertTrue(subscription.receipts.count())
+
+    def test_subscription_save_transaction_subscription_not_found(self):
+        subscription_counter = Subscription.objects.all().count()
+        transaction_id = '40060834171'
+        self.processor = AuthorizeNetProcessor(self.site, self.existing_invoice)
+        transaction_detail = self.processor.get_transaction_detail(transaction_id)
+        subscription_save_transaction(self.site, transaction_id, transaction_detail)
+
+        self.assertEqual(subscription_counter, Subscription.objects.all().count())
+
+    def test_subscription_save_transaction_payment_not_found(self):
+        subscription = Subscription.objects.get(gateway_id="7127667")
+        Payment.objects.filter(pk=3).delete()
+        transaction_id = '40060834171'
+        self.processor = AuthorizeNetProcessor(self.site, self.existing_invoice)
+        transaction_detail = self.processor.get_transaction_detail(transaction_id)
+        subscription_save_transaction(self.site, transaction_id, transaction_detail)
+
+        self.assertEqual(1, subscription.payments.count())
+
+    def test_subscription_save_transaction_multiple_payments(self):
+        subscription = Subscription.objects.get(gateway_id="7127667")
+        duplicate_payment = Payment.objects.get(pk=3)
+        duplicate_payment.uuid = uuid4()
+        duplicate_payment.pk = None
+        duplicate_payment.save()
+        transaction_id = '40060834171'
+        self.processor = AuthorizeNetProcessor(self.site, self.existing_invoice)
+        transaction_detail = self.processor.get_transaction_detail(transaction_id)
+        subscription_save_transaction(self.site, transaction_id, transaction_detail)
+
+        self.assertEqual(1, subscription.payments.count())
+
+    def test_update_payment_success(self):
+        payment = Payment.objects.get(pk=3)
+        payment.transaction = '40060834171'
+        payment.save()
+        transaction_id = '40060834171'
+        self.processor = AuthorizeNetProcessor(self.site, self.existing_invoice)
+        transaction_detail = self.processor.get_transaction_detail(transaction_id)
+        update_payment(self.site, transaction_id, transaction_detail)
+        
+        payment.refresh_from_db()
+        self.assertEqual(payment.status, PurchaseStatus.SETTLED)
+
+
```

### Comparing `django-vendor-0.3.9/vendor/tests/test_processor.py` & `django-vendor-0.4.0/src/vendor/tests/test_processor.py`

 * *Files 11% similar despite different names*

```diff
@@ -212,14 +212,22 @@
         base_processor.authorize_payment()
 
         self.assertTrue(invoice.payments.count())
         self.assertTrue(customer.receipts.count())
 
     def test_renew_subscription(self):
         subscription = Subscription.objects.get(pk=1)
+        offer = subscription.get_offer()
+        offer.term_details['trial_occurrences'] = 0
+        offer.term_details['trial_days'] = 0
+        offer.save()
+        offer.refresh_from_db()
+        subscription.save()
+        subscription.refresh_from_db()
+
         submitted_datetime = timezone.now()
 
         invoice = Invoice.objects.create(
             profile=subscription.profile,
             site=subscription.profile.site,
             ordered_date=submitted_datetime,
             status=InvoiceStatus.COMPLETE
@@ -242,14 +250,71 @@
 
         processor = PaymentProcessorBase(subscription.profile.site)
         processor.subscription_update_price(subscription, price, self.user)
 
         subscription.refresh_from_db()
         self.assertIn('price_update', subscription.meta)
 
+    def test_subscription_payment_billing_start_date(self):
+        today = timezone.now()
+        self.subscription_offer.billing_start_date = today + timedelta(days=10)
+        self.subscription_offer.save()
+
+        self.base_processor.set_billing_address_form_data(self.form_data['billing_address_form'], BillingAddressForm)
+        self.base_processor.set_payment_info_form_data(self.form_data['credit_card_form'], CreditCardForm)
+        self.base_processor.is_data_valid()
+
+        self.base_processor.invoice.add_offer(self.subscription_offer)
+        self.base_processor.invoice.save()
+        self.base_processor.transaction_succeeded = True
+        self.base_processor.process_subscriptions()
+    
+        self.assertEqual(today.strftime("%y/%m/%d"), self.base_processor.trial_receipt.start_date.strftime("%y/%m/%d"))
+        self.assertEqual((self.subscription_offer.billing_start_date - timedelta(days=1)).strftime("%y/%m/%d"), self.base_processor.trial_receipt.end_date.strftime("%y/%m/%d"))
+
+    def test_subscription_payment_term_start_date(self):
+        today = timezone.now()
+        self.subscription_offer.term_start_date = today + timedelta(days=10)
+        self.subscription_offer.term_details['trial_amount'] = 0
+        self.subscription_offer.term_details['trial_occurrences'] = 0
+        self.subscription_offer.term_details['trial_days'] = 0
+        self.subscription_offer.save()
+
+        self.base_processor.set_billing_address_form_data(self.form_data['billing_address_form'], BillingAddressForm)
+        self.base_processor.set_payment_info_form_data(self.form_data['credit_card_form'], CreditCardForm)
+        self.base_processor.is_data_valid()
+
+        self.base_processor.invoice.add_offer(self.subscription_offer)
+        self.base_processor.invoice.save()
+        self.base_processor.transaction_succeeded = True
+        self.base_processor.process_subscriptions()
+    
+        self.assertIsNone(self.base_processor.trial_receipt)
+        self.assertEqual(self.subscription_offer.term_start_date, self.base_processor.receipt.start_date)
+    
+    def test_subscription_payment_trial_days(self):
+        today = timezone.now()
+        self.subscription_offer.term_start_date = today + timedelta(days=10)
+        self.subscription_offer.term_details['trial_amount'] = 10
+        self.subscription_offer.term_details['trial_occurrences'] = 0
+        self.subscription_offer.term_details['trial_days'] = 7
+        self.subscription_offer.save()
+
+        self.base_processor.set_billing_address_form_data(self.form_data['billing_address_form'], BillingAddressForm)
+        self.base_processor.set_payment_info_form_data(self.form_data['credit_card_form'], CreditCardForm)
+        self.base_processor.is_data_valid()
+
+        self.base_processor.invoice.add_offer(self.subscription_offer)
+        self.base_processor.invoice.save()
+        self.base_processor.transaction_succeeded = True
+        self.base_processor.process_subscriptions()
+    
+        self.assertEqual(self.subscription_offer.term_start_date.strftime("%y/%m/%d"), self.base_processor.trial_receipt.start_date.strftime("%y/%m/%d"))
+        self.assertEqual((self.base_processor.trial_receipt.end_date).strftime("%y/%m/%d"), (self.subscription_offer.term_start_date + timezone.timedelta(days=self.subscription_offer.term_details['trial_days'])).strftime("%y/%m/%d"))
+    
     # def test_get_header_javascript_success(self):
     #     raise NotImplementedError()
 
     # def test_get_javascript_success(self):
     #     raise NotImplementedError()
 
     # def test_get_template_success(self):
```

### Comparing `django-vendor-0.3.9/vendor/tests/test_stripe.py` & `django-vendor-0.4.0/src/vendor/tests/test_stripe.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import stripe
-from random import randrange
+
+from core.models import Product
 from django.conf import settings
-from django.test import TestCase, Client, tag
+from django.contrib.auth import get_user_model
 from django.contrib.sites.models import Site
-from django.db.models import signals
+from django.db.models import Q, signals
+from django.test import Client, TestCase
 from django.utils import timezone
-from django.db.models import Q
+from random import randrange
 from siteconfigs.models import SiteConfigModel
+
 from unittest import skipIf
-from vendor.forms import CreditCardForm, BillingAddressForm
-from vendor.processors import StripeProcessor
-from django.contrib.auth import get_user_model
-from vendor.models import Invoice, Payment, Offer, Price, Receipt, CustomerProfile, OrderItem, Subscription
-from core.models import Product
+from vendor.forms import BillingAddressForm, CreditCardForm
+from vendor.models import CustomerProfile, Invoice, Offer, Price
 from vendor.models.choice import InvoiceStatus
-
+from vendor.processors import StripeProcessor
 
 User = get_user_model()
 
 @skipIf((settings.STRIPE_PUBLIC_KEY or settings.STRIPE_SECRET_KEY) is None, "Stripe enviornment variables not set, skipping tests")
 class StripeProcessorTests(TestCase):
     fixtures = ['user', 'unit_test']
 
@@ -95,15 +95,14 @@
         self.cus_norrin_radd2 = {'name': 'Jake Paul', 'email': 'jpaul@radd.com', 'metadata': self.valid_metadata}
         self.pro_annual_license = {"name": "Annual Subscription", 'metadata': self.valid_metadata}
         self.pro_annual_license2 = {"name": "Annual Subscription 2", 'metadata': self.valid_metadata}
         self.pri_monthly = {"currency": "usd", "unit_amount": 1024,
                             "recurring": {"interval": "month", "interval_count": 1, "usage_type": "licensed"},
                             'metadata': self.valid_metadata}
 
-
     def test_environment_variables_set(self):
         self.assertIsNotNone(settings.STRIPE_PUBLIC_KEY)
 
     def test_processor_initialization_success(self):
         self.assertEquals(self.processor.provider, 'StripeProcessor')
         self.assertIsNotNone(self.processor.invoice)
         self.assertIsNotNone(self.processor.credentials)
@@ -411,15 +410,14 @@
         pk_list = [product['metadata']['pk'] for product in offers]
         vendor_offers_in_stripe = self.processor.get_vendor_offers_in_stripe(pk_list, self.site)
 
         self.assertIsNotNone(vendor_offers_in_stripe)
         self.assertIn(offer1, vendor_offers_in_stripe)
         self.assertIn(offer2, vendor_offers_in_stripe)
 
-
     def test_get_vendor_offers_not_in_stripe(self):
         offers = self.processor.get_site_offers(self.site)
         #stripe_offer_names = [product['name'] for product in offers]
         #vendor_offer_names = [self.pro_annual_license['name'], self.pro_annual_license2['name']]
 
         pk_list = [product['metadata']['pk'] for product in offers]
 
@@ -509,15 +507,14 @@
 
         self.processor.stripe_delete_object(self.processor.stripe.Customer, vendor_customer1.meta['stripe_id'])
         self.processor.stripe_delete_object(self.processor.stripe.Customer, vendor_customer2.meta['stripe_id'])
 
         self.assertIsNotNone(vendor_customer1.meta.get('stripe_id', None))
         self.assertIsNotNone(vendor_customer2.meta.get('stripe_id', None))
 
-
     def test_update_stripe_customers(self):
         stripe_customer1 = self.processor.stripe_create_object(self.processor.stripe.Customer, self.cus_norrin_radd)
         stripe_customer2 = self.processor.stripe_create_object(self.processor.stripe.Customer, self.cus_norrin_radd2)
 
         user1 = User.objects.create(email=self.cus_norrin_radd['email'], first_name='New First Name1', last_name='Last Name1', username='test1')
         user2 = User.objects.create(email=self.cus_norrin_radd2['email'], first_name='New First Name2', last_name='Last Name2', username='test2')
         vendor_customer1 = CustomerProfile.objects.create(site=self.site, user=user1, meta={'stripe_id': stripe_customer1.id})
@@ -564,14 +561,39 @@
         product_id = self.processor.get_product_id_with_name(self.pro_annual_license['name'], metadata=metadata)
 
         offers = self.processor.get_site_offers(self.site)
         stripe_offer_ids = [product['id'] for product in offers]
 
         self.assertIn(product_id, stripe_offer_ids)
 
+    def test_get_customer_payment_methods(self):
+        payment_methods = self.processor.get_customer_payment_methods("cus_Mt98i0KskNWP0X")
+
+        self.assertTrue(payment_methods)
+
+    def test_charge_customer_profile_success(self):
+        self.processor.invoice.profile.meta['stripe_id'] = "cus_Mt98i0KskNWP0X"
+        self.processor.invoice.profile.save()
+        self.processor.invoice.profile.refresh_from_db()
+        self.processor.set_billing_address_form_data(self.form_data.get('billing_address_form'), BillingAddressForm)
+        self.processor.set_payment_info_form_data(self.form_data.get('credit_card_form'), CreditCardForm)
+        self.processor.invoice.total = randrange(1, 1000)
+
+        for recurring_order_items in self.processor.invoice.get_recurring_order_items():
+            self.processor.invoice.remove_offer(recurring_order_items.offer)
+
+        self.processor.set_stripe_payment_source()
+        self.processor.transaction_succeeded = False
+
+        self.processor.process_customer_profile_payment()
+
+        self.assertIsNotNone(self.processor.payment)
+        self.assertTrue(self.processor.payment.success)
+        self.assertEquals(InvoiceStatus.COMPLETE, self.processor.invoice.status)
+    
 
     """
     Commenting out since stripe doesnt allow you to delete Price objects (weird)
     
     def test_check_price_does_exist(self):
         stripe_product = self.processor.stripe_create_object(self.processor.stripe.Product, self.pro_annual_license)
         self.pri_monthly['product'] = stripe_product.id
@@ -625,16 +647,14 @@
 
 
         self.assertTrue(stripe_meta)
         self.assertTrue(stripe_meta.get('product_id'))
         self.assertTrue(stripe_meta.get('price_id'))
 
 
-
-
 @skipIf((settings.STRIPE_PUBLIC_KEY or settings.STRIPE_SECRET_KEY) is None, "Strip enviornment variables not set, skipping tests")
 class StripeCRUDObjectTests(TestCase):
 
     def init_test_objects(self):
         self.valid_metadata = {'site': 'sc', 'pk':1}
         self.valid_addr = {'city': "na",'country': "US",'line1': "Salvatierra walk",'postal_code': "90321",'state': 'CA'}
```

### Comparing `django-vendor-0.3.9/vendor/urls/vendor.py` & `django-vendor-0.4.0/src/vendor/urls/vendor.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/urls/vendor_admin.py` & `django-vendor-0.4.0/src/vendor/urls/vendor_admin.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/utils.py` & `django-vendor-0.4.0/src/vendor/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -46,32 +46,35 @@
 def get_future_date_days(today, add_days):
     """
     Returns a datetime object with the a new added days
     """
     return today + timedelta(days=add_days)
 
 
-def get_payment_scheduled_end_date(offer, start_date=timezone.now()):
-    """
-    Determines the start date offset so the payment gateway starts charging the monthly offer
-    """
-    units = offer.term_details.get('term_units', TermDetailUnits.MONTH)
+# def get_payment_scheduled_end_date(offer, start_date=timezone.now()):
+#     """
+#     Determines the start date offset so the payment gateway starts charging the monthly offer
+#     """
+#     units = offer.term_details.get('term_units', TermDetailUnits.MONTH)
+    
+#     if units == TermDetailUnits.MONTH:
+#         return get_future_date_months(start_date, offer.get_period_length())
+    
+#     elif units == TermDetailUnits.DAY:
+#         return get_future_date_days(start_date, offer.get_period_length())
+
+# def get_subscription_start_date(offer, profile, start_date=timezone.now()):
+#     billing_date = offer.billing_start_date
 
-    if units == TermDetailUnits.MONTH:
-        return get_future_date_months(start_date, offer.get_period_length())
-    elif units == TermDetailUnits.DAY:
-        return get_future_date_days(start_date, offer.get_period_length())
-
-def get_subscription_start_date(offer, profile, start_date=timezone.now()):
-    if profile.is_on_trial(offer):
-        return start_date + timedelta(days=offer.get_trial_days())
+#     if profile.is_offer_on_trial(offer) or not profile.has_owned_product(offer.products.all()):
+#         if not billing_date:
+#             return start_date + timedelta(days=offer.get_trial_days())
     
-    if not profile.has_owned_product(offer.products.all()):
-        return start_date + timedelta(days=offer.get_trial_days())
+#         return billing_date
 
-    return start_date
+#     return start_date
         
 
 def get_display_decimal(amount):
     return Decimal(amount).quantize(Decimal('.00'), rounding=ROUND_UP)
```

### Comparing `django-vendor-0.3.9/vendor/views/__init__.py` & `django-vendor-0.4.0/src/vendor/views/__init__.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/views/config.py` & `django-vendor-0.4.0/src/vendor/views/config.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/views/integration.py` & `django-vendor-0.4.0/src/vendor/views/integration.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-
+from django.contrib.auth.mixins import LoginRequiredMixin
 from django.utils.translation import gettext as _
 from django.views.generic.edit import FormView
 from vendor.integrations import AuthorizeNetIntegration, StripeIntegration
 
 from vendor.forms import AuthorizeNetIntegrationForm, StripeIntegrationForm
 from django.urls import reverse_lazy
 from vendor.views.mixin import get_site_from_request
 
 
-class AuthorizeNetIntegrationView(FormView):
+class AuthorizeNetIntegrationView(LoginRequiredMixin, FormView):
     template_name = "vendor/integration_form.html"
     form_class = AuthorizeNetIntegrationForm
-    success_url = reverse_lazy('authorizenet-integration')
+    success_url = reverse_lazy('vendor_admin:authorizenet-integration')
 
     def get_context_data(self, *args, **kwargs):
         context = super().get_context_data(**kwargs)
         authorizenet_integration = AuthorizeNetIntegration(get_site_from_request(self.request))
         context['integration_name'] = _("AuthorizeNet Integration")
 
         context['form'] = AuthorizeNetIntegrationForm(instance=authorizenet_integration.instance)
@@ -25,18 +25,18 @@
     def form_valid(self, form):
         authorizenet_integration = AuthorizeNetIntegration(get_site_from_request(self.request))
         authorizenet_integration.save(form.cleaned_data)
 
         return super().form_valid(form)
 
 
-class StripeIntegrationView(FormView):
+class StripeIntegrationView(LoginRequiredMixin, FormView):
     template_name = "vendor/integration_form.html"
     form_class = StripeIntegrationForm
-    success_url = reverse_lazy('stripe-integration')
+    success_url = reverse_lazy('vendor_admin:stripe-integration')
 
     def get_context_data(self, *args, **kwargs):
         context = super().get_context_data(**kwargs)
         stripe_integration = StripeIntegration(get_site_from_request(self.request))
         context['integration_name'] = _("Stripe Integration")
 
         context['form'] = StripeIntegrationForm(instance=stripe_integration.instance)
```

### Comparing `django-vendor-0.3.9/vendor/views/mixin.py` & `django-vendor-0.4.0/src/vendor/views/mixin.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/views/report.py` & `django-vendor-0.4.0/src/vendor/views/report.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.3.9/vendor/views/vendor.py` & `django-vendor-0.4.0/src/vendor/views/vendor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import logging
 
 from django.contrib import messages
 from django.contrib.auth.mixins import LoginRequiredMixin
 from django.core.exceptions import ObjectDoesNotExist
-from django.shortcuts import render, redirect, Http404
-from django.utils.translation import gettext as _
+from django.shortcuts import Http404, redirect, render
 from django.urls import reverse_lazy
-from django.views.generic import TemplateView, View, FormView
-from django.views.generic.edit import UpdateView
+from django.utils.translation import gettext as _
+from django.views.generic import FormView, TemplateView
 from django.views.generic.detail import DetailView
+from django.views.generic.edit import UpdateView
 from django.views.generic.list import ListView
 
-
-from vendor.forms import BillingAddressForm, CreditCardForm, AccountInformationForm, AddressForm
-from vendor.models import Offer, Invoice, Address, OrderItem, Receipt, Subscription
-from vendor.models.choice import TermType, PurchaseStatus, InvoiceStatus
+from vendor.forms import (AccountInformationForm, AddressForm,
+                          BillingAddressForm, CreditCardForm)
+from vendor.models import (Address, Invoice, Offer, OrderItem, Receipt,
+                           Subscription)
+from vendor.models.choice import InvoiceStatus, TermType
 from vendor.processors import get_site_payment_processor
-from vendor.utils import get_site_from_request, get_or_create_session_cart, clear_session_purchase_data
+from vendor.utils import (clear_session_purchase_data,
+                          get_or_create_session_cart, get_site_from_request)
 
 logger = logging.getLogger(__name__)
 
 
 # TODO: Need to remove the login required
 def get_purchase_invoice(user, site):
     """
@@ -308,15 +310,15 @@
         payment_form = CreditCardForm(request.POST)
 
         if not payment_form.is_valid():
             messages.info(request, _("Invalid Card"))
             return redirect(request.META.get('HTTP_REFERER', self.success_url))
 
         processor = get_site_payment_processor(subscription.profile.site)(subscription.profile.site)
-        processor.set_payment_info_form_data(request.POST, CreditCardForm)
+        processor.payment_info = payment_form
         processor.subscription_update_payment(subscription)
 
         if not processor.transaction_succeeded:
             messages.info(request, _(f"Payment gateway error: {processor.transaction_info.get('errors', '')}"))
             return redirect(request.META.get('HTTP_REFERER', self.success_url))
 
         messages.info(request, _("Success: Payment Updated"))
```

### Comparing `django-vendor-0.3.9/vendor/views/vendor_admin.py` & `django-vendor-0.4.0/src/vendor/views/vendor_admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 from vendor.forms import OfferForm, PriceFormSet, CreditCardForm, AddressForm,\
     SubscriptionForm, SiteSelectForm, SubscriptionAddPaymentForm, OfferSiteSelectForm
 
 from vendor.models import Invoice, Offer, Receipt, CustomerProfile, Payment, Subscription
 from vendor.models.choice import PaymentTypes, InvoiceStatus, PurchaseStatus
 from vendor.views.mixin import PassRequestToFormKwargsMixin, SiteOnRequestFilterMixin, TableFilterMixin, get_site_from_request
 from vendor.processors import get_site_payment_processor
-from vendor.utils import get_subscription_start_date, get_payment_scheduled_end_date
 
 Product = apps.get_model(VENDOR_PRODUCT_MODEL)
 logger = logging.getLogger(__name__)
 
 
 #############
 # Admin Views
@@ -378,16 +377,16 @@
                 payment.save()
 
                 if payment.success and payment.status == PurchaseStatus.SETTLED:
                     receipt = Receipt.objects.create(
                         transaction=payment.transaction,
                         order_item=invoice.order_items.first(),
                         profile=payment.profile,
-                        start_date=get_subscription_start_date(offer, payment.profile, payment.submitted_date),
-                        end_date=get_payment_scheduled_end_date(offer, payment.submitted_date),
+                        start_date=offer.get_offer_start_date(payment.submitted_date),
+                        end_date=offer.get_offer_end_date(payment.submitted_date),
                         subscription=payment.subscription
                     )
 
             messages.info(request, _("Payment Added to Subscription"))
 
         except (IntegrityError, DatabaseError, Exception) as exce:
             logger.error(f"AdminSubscriptionCreateView error: {exce}")
@@ -401,24 +400,23 @@
     """
     List of CustomerProfiles on site
     """
     template_name = "vendor/manage/profile_list.html"
     model = CustomerProfile
     paginate_by = 100
 
-
     def search_filter(self, queryset):
         search_value = self.request.GET.get('search_filter')
         return queryset.filter(Q(pk__icontains=search_value) | \
                                Q(user__email__icontains=search_value) | \
                                Q(user__username__icontains=search_value))
 
     def get_paginated_by(self, queryset):
         if 'paginate_by' in self.request.kwargs:
-            return kwargs['paginate_by']
+            return self.kwargs['paginate_by']
         return self.paginate_by
     
     def get_queryset(self):
         queryset = super().get_queryset()
 
         return queryset.order_by('pk')
 
@@ -459,15 +457,15 @@
         )
         invoice.add_offer(offer)
         invoice.save()
 
         transaction_id = timezone.now().strftime("%Y-%m-%d_%H-%M-%S-Manual-Renewal")
 
         processor = get_site_payment_processor(invoice.site)(invoice.site, invoice)
-        processor.renew_subscription(subscription, transaction_id, PurchaseStatus.CAPTURED)
+        processor.renew_subscription(subscription, transaction_id, PurchaseStatus.CAPTURED, submitted_datetime)
 
         messages.info(request, _("Subscription Renewed"))
         return redirect(request.META.get('HTTP_REFERER', self.success_url))
 
 
 class PaymentWithNoReceiptListView(LoginRequiredMixin, ListView):
     template_name = "vendor/manage/payment_list.html"
```

