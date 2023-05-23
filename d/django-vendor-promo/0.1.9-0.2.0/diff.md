# Comparing `tmp/django-vendor-promo-0.1.9.tar.gz` & `tmp/django-vendor-promo-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-vendor-promo-0.1.9.tar", last modified: Mon Oct  4 15:07:46 2021, max compression
+gzip compressed data, was "django-vendor-promo-0.2.0.tar", last modified: Tue May 23 21:53:47 2023, max compression
```

## Comparing `django-vendor-promo-0.1.9.tar` & `django-vendor-promo-0.2.0.tar`

### file list

```diff
@@ -1,46 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 15:07:46.000000 django-vendor-promo-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1451 2021-10-04 15:07:46.000000 django-vendor-promo-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      338 2021-10-04 15:07:21.000000 django-vendor-promo-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 15:07:46.000000 django-vendor-promo-0.1.9/django_vendor_promo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1451 2021-10-04 15:07:46.000000 django-vendor-promo-0.1.9/django_vendor_promo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2021-10-04 15:07:46.000000 django-vendor-promo-0.1.9/django_vendor_promo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-04 15:07:46.000000 django-vendor-promo-0.1.9/django_vendor_promo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      331 2021-10-04 15:07:46.000000 django-vendor-promo-0.1.9/django_vendor_promo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-10-04 15:07:46.000000 django-vendor-promo-0.1.9/django_vendor_promo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-04 15:07:46.000000 django-vendor-promo-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2563 2021-10-04 15:07:21.000000 django-vendor-promo-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 15:07:46.000000 django-vendor-promo-0.1.9/vendorpromo/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-04 15:07:21.000000 django-vendor-promo-0.1.9/vendorpromo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-10-04 15:07:21.000000 django-vendor-promo-0.1.9/vendorpromo/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)      361 2021-10-04 15:07:21.000000 django-vendor-promo-0.1.9/vendorpromo/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 15:07:46.000000 django-vendor-promo-0.1.9/vendorpromo/api/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-04 15:07:21.000000 django-vendor-promo-0.1.9/vendorpromo/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 15:07:46.000000 django-vendor-promo-0.1.9/vendorpromo/api/v1/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-04 15:07:21.000000 django-vendor-promo-0.1.9/vendorpromo/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1443 2021-10-04 15:07:21.000000 django-vendor-promo-0.1.9/vendorpromo/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     5257 2021-10-04 15:07:21.000000 django-vendor-promo-0.1.9/vendorpromo/api/v1/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 15:07:46.000000 django-vendor-promo-0.1.9/vendorpromo/api/v1/vouchery/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-04 15:07:21.000000 django-vendor-promo-0.1.9/vendorpromo/api/v1/vouchery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-04 15:07:21.000000 django-vendor-promo-0.1.9/vendorpromo/api/v1/vouchery/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     5874 2021-10-04 15:07:21.000000 django-vendor-promo-0.1.9/vendorpromo/api/v1/vouchery/views.py
--rw-r--r--   0 runner    (1001) docker     (121)      103 2021-10-04 15:07:21.000000 django-vendor-promo-0.1.9/vendorpromo/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     2175 2021-10-04 15:07:21.000000 django-vendor-promo-0.1.9/vendorpromo/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2371 2021-10-04 15:07:21.000000 django-vendor-promo-0.1.9/vendorpromo/forms.py
--rw-r--r--   0 runner    (1001) docker     (121)     1232 2021-10-04 15:07:21.000000 django-vendor-promo-0.1.9/vendorpromo/integrations.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 15:07:46.000000 django-vendor-promo-0.1.9/vendorpromo/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     1932 2021-10-04 15:07:21.000000 django-vendor-promo-0.1.9/vendorpromo/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-04 15:07:21.000000 django-vendor-promo-0.1.9/vendorpromo/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2008 2021-10-04 15:07:21.000000 django-vendor-promo-0.1.9/vendorpromo/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 15:07:46.000000 django-vendor-promo-0.1.9/vendorpromo/processors/
--rw-r--r--   0 runner    (1001) docker     (121)      157 2021-10-04 15:07:21.000000 django-vendor-promo-0.1.9/vendorpromo/processors/DummyProcessor.py
--rw-r--r--   0 runner    (1001) docker     (121)      405 2021-10-04 15:07:21.000000 django-vendor-promo-0.1.9/vendorpromo/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3356 2021-10-04 15:07:21.000000 django-vendor-promo-0.1.9/vendorpromo/processors/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    17114 2021-10-04 15:07:21.000000 django-vendor-promo-0.1.9/vendorpromo/processors/vouchery.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 15:07:46.000000 django-vendor-promo-0.1.9/vendorpromo/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-04 15:07:21.000000 django-vendor-promo-0.1.9/vendorpromo/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      509 2021-10-04 15:07:21.000000 django-vendor-promo-0.1.9/vendorpromo/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    20722 2021-10-04 15:07:21.000000 django-vendor-promo-0.1.9/vendorpromo/tests/test_processor.py
--rw-r--r--   0 runner    (1001) docker     (121)     2363 2021-10-04 15:07:21.000000 django-vendor-promo-0.1.9/vendorpromo/tests/test_promo.py
--rw-r--r--   0 runner    (1001) docker     (121)     1011 2021-10-04 15:07:21.000000 django-vendor-promo-0.1.9/vendorpromo/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      292 2021-10-04 15:07:21.000000 django-vendor-promo-0.1.9/vendorpromo/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5737 2021-10-04 15:07:21.000000 django-vendor-promo-0.1.9/vendorpromo/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:53:47.936495 django-vendor-promo-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/LICENSE.mit.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-23 21:53:47.936495 django-vendor-promo-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 21:53:47.936495 django-vendor-promo-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:53:47.924493 django-vendor-promo-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:53:47.928494 django-vendor-promo-0.2.0/src/django_vendor_promo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-23 21:53:47.000000 django-vendor-promo-0.2.0/src/django_vendor_promo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-05-23 21:53:47.000000 django-vendor-promo-0.2.0/src/django_vendor_promo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 21:53:47.000000 django-vendor-promo-0.2.0/src/django_vendor_promo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-23 21:53:47.000000 django-vendor-promo-0.2.0/src/django_vendor_promo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 21:53:47.000000 django-vendor-promo-0.2.0/src/django_vendor_promo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:53:47.928494 django-vendor-promo-0.2.0/src/vendorpromo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:53:47.928494 django-vendor-promo-0.2.0/src/vendorpromo/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:53:47.928494 django-vendor-promo-0.2.0/src/vendorpromo/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/api/v1/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:53:47.932494 django-vendor-promo-0.2.0/src/vendorpromo/api/v1/vouchery/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/api/v1/vouchery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/api/v1/vouchery/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/api/v1/vouchery/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/integrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:53:47.932494 django-vendor-promo-0.2.0/src/vendorpromo/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/migrations/0002_affiliate_couponcode_promotionalcampaign.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:53:47.932494 django-vendor-promo-0.2.0/src/vendorpromo/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/processors/DummyProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/processors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/processors/stripe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17373 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/processors/vouchery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:53:47.928494 django-vendor-promo-0.2.0/src/vendorpromo/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:53:47.932494 django-vendor-promo-0.2.0/src/vendorpromo/templates/vendorpromo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/templates/vendorpromo/affiliate_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/templates/vendorpromo/affiliate_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/templates/vendorpromo/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/templates/vendorpromo/coupon_code_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/templates/vendorpromo/coupon_code_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:53:47.932494 django-vendor-promo-0.2.0/src/vendorpromo/templates/vendorpromo/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/templates/vendorpromo/includes/promocode_apply.html
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/templates/vendorpromo/processor_site_config.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/templates/vendorpromo/processor_site_config_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/templates/vendorpromo/promo.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/templates/vendorpromo/promo_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/templates/vendorpromo/promocode_formset.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/templates/vendorpromo/promotional_campaign_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/templates/vendorpromo/promotional_campaign_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/templates/vendorpromo/vouchery_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/templates/vendorpromo/vouchery_integration.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/templates/vendorpromo/vouchery_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:53:47.936495 django-vendor-promo-0.2.0/src/vendorpromo/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/tests/test_affiliate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/tests/test_coupon_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21273 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/tests/test_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/tests/test_promo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/tests/test_promotional_campaign.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20938 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/tests/test_stripe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15017 2023-05-23 21:52:43.000000 django-vendor-promo-0.2.0/src/vendorpromo/views.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-vendor-promo-0.1.9/vendorpromo/api/v1/urls.py` & `django-vendor-promo-0.2.0/src/vendorpromo/api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.1.9/vendorpromo/api/v1/views.py` & `django-vendor-promo-0.2.0/src/vendorpromo/api/v1/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from django.contrib import messages
 from django.contrib.auth.mixins import LoginRequiredMixin
 from django.shortcuts import get_object_or_404, redirect
 from django.http.response import HttpResponse, HttpResponseBadRequest, Http404
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from django.views.generic import DeleteView, View
 
 from vendor.models import Invoice
-from vendor.views.vendor import AddToCartView
+from vendor.api.v1.views import AddToCartView
 
 from vendorpromo.forms import PromoForm
 from vendorpromo.processors import get_site_promo_processor
 from vendorpromo.models import Promo
 
 
 class CreatePromoAPIView(LoginRequiredMixin, View):
@@ -18,27 +18,28 @@
     def post(self, request, *args, **kwargs):
         promo_form = PromoForm(request.POST)
         promo = promo_form.save(commit=False)
 
         if not promo_form.is_valid():
             messages.info(request, _(f'Create Promo Failed. Errors: {promo_form.errors}'))
             return redirect(request.META.get('HTTP_REFERER', "vendorpromo-list"))
-        processor = get_site_promo_processor(site=promo.offer.site)()
+            
+        processor = get_site_promo_processor(promo.offer.site)(promo.offer.site)
         processor.create_promo(promo_form)
         messages.success(request, _("Promo Code Created"))
         return redirect(request.META.get('HTTP_REFERER', "vendorpromo-list"))
 
 
 class DeletePromoAPIView(LoginRequiredMixin, DeleteView):
     model = Promo
     slug_field = 'uuid'
     slug_url_kwarg = 'uuid'
 
     def post(self, request, *args, **kwargs):
-        processor = get_site_promo_processor(self.get_object().offer.site)()
+        processor = get_site_promo_processor(self.get_object().offer.site)(self.get_object().offer.site)
         processor.delete_promo(self.get_object())
         return redirect(request.META.get('HTTP_REFERER'))
 
 
 class ValidateCodeCheckoutProcessAPIView(LoginRequiredMixin, View):
     """
     When a customer is applying a code during the checkout process
@@ -63,15 +64,15 @@
                 offer_in_cart = order_item.offer
                 break
 
         if offer_in_cart is None:
             messages.success(request, _("Invalid Promo Code"))
             return HttpResponseBadRequest(f"No related offer in cart for code: {promo.code}")
 
-        processor = get_site_promo_processor(site=invoice.site)(invoice=invoice)
+        processor = get_site_promo_processor(invoice.site)(invoice.site, invoice=invoice)
 
         if not processor.is_code_valid_on_checkout(promo.code, promo.offer.current_price()):
             messages.success(request, _("Invalid Promo Code"))
             return HttpResponseBadRequest(f"Processor rejected code {promo.code}\nmsg:{processor.response_message}\nerror: {processor.response_error}")
 
         invoice.swap_offer(offer_in_cart, promo.offer)
         messages.success(request, _("Promo Code Applied"))
```

### Comparing `django-vendor-promo-0.1.9/vendorpromo/api/v1/vouchery/views.py` & `django-vendor-promo-0.2.0/src/vendorpromo/api/v1/vouchery/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,59 +1,71 @@
 import json
+import logging
 
 from django.contrib.auth.mixins import LoginRequiredMixin
 from django.http.response import Http404, HttpResponseBadRequest, HttpResponseServerError
 from django.shortcuts import render, redirect
 from django.views.generic import TemplateView, FormView
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 
 from vendorpromo.processors.vouchery import VoucheryProcessor
 from vendorpromo.forms import VoucherySearchForm, PromoForm
 
+from vendor.utils import get_site_from_request
+
+logger = logging.getLogger(__name__)
 
 class VoucheryCreateOfferPromoAPIView(LoginRequiredMixin, FormView):
     form_class = PromoForm
 
     def post(self, request, *args, **kwargs):
         promo_form = PromoForm(request.POST)
+
         if not promo_form.is_valid():
             raise HttpResponseBadRequest()
 
-        processor = VoucheryProcessor()
+        processor = VoucheryProcessor(get_site_from_request(request))
+        try:
+            processor.create_promo_automate(promo_form)
 
-        processor.create_promo_automate(promo_form)
+            if not processor.is_request_success:
+                raise HttpResponseServerError(_(f"Createing Promo Failed: {processor.response_message}-{processor.response_error}"))
 
-        if not processor.is_request_success:
-            raise HttpResponseServerError(_(f"Createing Promo Failed: {processor.response_message}-{processor.response_errors}"))
+        except (HttpResponseServerError, Exception) as exce:
+            logger.error(f"VoucheryCreateOfferPromoAPIView: {exce}")
 
         return redirect(request.META.get('HTTP_REFERER'))
 
 
 # The following views are intended for Sys Admins to quickly and easy monitor
 # the state of there vouchery account. It is not recommended that this tools
 # are made available to commeners.
 # TODO: Should probably add more admin/perms
 class VoucheryCampaignsView(LoginRequiredMixin, TemplateView):
     template_name = 'vendorpromo/vouchery_list.html'
 
     def get(self, request, *args, **kwargs):
         context = super().get_context_data(*args, **kwargs)
-        processor = VoucheryProcessor()
+
+        processor = VoucheryProcessor(get_site_from_request(request))
         processor.get_campaigns()
+
         if not processor.is_request_success:
             raise HttpResponseBadRequest(_(f"Error: {processor.response_message}"))
+
         context['object_list'] = processor.response_content
         context['form'] = VoucherySearchForm
+
         return render(request, self.template_name, context)
 
     def post(self, request, *args, **kwargs):
         context = super().get_context_data(**kwargs)
         vouchery_search_form = VoucherySearchForm(request.POST)
 
-        processor = VoucheryProcessor()
+        processor = VoucheryProcessor(get_site_from_request(request))
         processor.get_campaigns(**json.loads(vouchery_search_form.data['querystring']))
 
         if not processor.is_request_success:
             raise HttpResponseBadRequest(_(f"Error: {processor.response_message}"))
 
         context['object_list'] = processor.response_content
         context['form'] = vouchery_search_form
@@ -61,75 +73,90 @@
 
 
 class VoucheryCampaignDetailView(LoginRequiredMixin, TemplateView):
     template_name = 'vendorpromo/vouchery_detail.html'
 
     def get(self, request, *args, **kwargs):
         context = super().get_context_data(*args, **kwargs)
-        processor = VoucheryProcessor()
+        
+        processor = VoucheryProcessor(get_site_from_request(request))
         processor.get_campaign(kwargs.get('campaign_id'))
+        
         if not processor.is_request_success:
             raise HttpResponseBadRequest(_(f"Error: {processor.response_message}"))
         context['object'] = processor.response_content
+        
         return render(request, self.template_name, context)
 
 
 class VoucheryRedeemListView(LoginRequiredMixin, TemplateView):
     template_name = 'vendorpromo/vouchery_list.html'
 
     def get(self, request, *args, **kwargs):
         context = super().get_context_data(*args, **kwargs)
-        processor = VoucheryProcessor()
+        
+        processor = VoucheryProcessor(get_site_from_request(request))
         processor.get_redeems(kwargs.get('campaign_id'))
+        
         if not processor.is_request_success:
             raise HttpResponseBadRequest(_(f"Error: {processor.response_message}"))
+        
         context['object_list'] = processor.response_content
+        
         return render(request, self.template_name, context)
 
 
 class VoucheryRedeemDetailView(LoginRequiredMixin, TemplateView):
     template_name = 'vendorpromo/vouchery_detail.html'
 
     def get(self, request, *args, **kwargs):
         context = super().get_context_data(*args, **kwargs)
+        
         processor = VoucheryProcessor()
         processor.get_redeem(kwargs.get('code'), kwargs.get('transaction_id'))
 
         if not processor.is_request_success:
             raise Http404()
 
         context['object'] = processor.response_content
+        
         return render(request, self.template_name, context)
 
 
 class VoucheryVouchersView(LoginRequiredMixin, TemplateView):
     template_name = 'vendorpromo/vouchery_list.html'
 
     def get(self, request, *args, **kwargs):
         context = super().get_context_data(*args, **kwargs)
+        
         processor = VoucheryProcessor()
         processor.get_vouchers(kwargs.get('campaign_id'))
+        
         if not processor.is_request_success:
             raise HttpResponseBadRequest(_(f"Error: {processor.response_message}"))
+        
         context['object_list'] = processor.response_content
         context['form'] = VoucherySearchForm
+        
         return render(request, self.template_name, context)
 
     def post(self, request, *args, **kwargs):
         context = super().get_context_data(**kwargs)
+        
         vouchery_search_form = VoucherySearchForm(request.POST)
 
         processor = VoucheryProcessor()
         processor.get_vouchers(kwargs.get('campaign_id'), **json.loads(vouchery_search_form.data['params']))
 
         if not processor.is_request_success:
             raise HttpResponseBadRequest(_(f"Error: {processor.response_message}"))
 
         context['object_list'] = processor.response_content
         context['form'] = vouchery_search_form
+        
         return render(request, self.template_name, context)
 
 
 class VoucheryVoucherDetailView(LoginRequiredMixin, TemplateView):
     template_name = 'vendorpromo/vouchery_detail.html'
 
     def get(self, request, *args, **kwargs):
@@ -137,8 +164,9 @@
         processor = VoucheryProcessor()
         processor.get_voucher(kwargs.get('code'))
 
         if not processor.is_request_success:
             raise Http404()
 
         context['object'] = processor.response_content
+        
         return render(request, self.template_name, context)
```

### Comparing `django-vendor-promo-0.1.9/vendorpromo/config.py` & `django-vendor-promo-0.2.0/src/vendorpromo/config.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.1.9/vendorpromo/integrations.py` & `django-vendor-promo-0.2.0/src/vendorpromo/integrations.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.1.9/vendorpromo/migrations/0001_initial.py` & `django-vendor-promo-0.2.0/src/vendorpromo/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-vendor-promo-0.1.9/vendorpromo/processors/vouchery.py` & `django-vendor-promo-0.2.0/src/vendorpromo/processors/vouchery.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 import json
 
 from django.core.exceptions import ImproperlyConfigured
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from vendorpromo.config import VENDOR_PROMO_PROCESSOR_URL, VENDOR_PROMO_PROCESSOR_BARRER_KEY
 from vendorpromo.integrations import VoucheryIntegration
 from vendorpromo.processors.base import PromoProcessorBase
 
 
 class VoucheryProcessor(PromoProcessorBase):
@@ -49,24 +49,24 @@
     REWARD_PARAMS = {
         "type": "SetDiscount",
         "discount_type": "percentage",
         "discount_value": 0  # The actual discount is set in the Offer instance.
     }
     credentials = None
 
-    def __init__(self, invoice=None):
+    def __init__(self, site, invoice=None):
         super().__init__(invoice=invoice)
-        self.set_credentials(invoice.site)
+        self.set_credentials(site)
 
 
     def set_credentials(self, site):
         self.credentials = VoucheryIntegration(site)
         if self.credentials.instance:
-           self.BASE_URL = self.credentials.client_url
-           self.BARRER_KEY = self.credentials.private_key
+           self.BASE_URL = self.credentials.instance.client_url
+           self.BARRER_KEY = self.credentials.instance.private_key
         elif VENDOR_PROMO_PROCESSOR_URL and VENDOR_PROMO_PROCESSOR_BARRER_KEY:
            self.BASE_URL = VENDOR_PROMO_PROCESSOR_URL
            self.BARRER_KEY = VENDOR_PROMO_PROCESSOR_BARRER_KEY
         else:
             raise ImproperlyConfigured("Vouchery is not properly Configured. Missing BASE_URL and/or BARRER_KEY")
 
 
@@ -76,20 +76,27 @@
         '''
         This function automates the steps required to create a voucher/promo-code
         in Vouchery. This means that it will create a campaign named affter the
         offer's product name, a sub-campaign named after the offer's a percentage reward
         and finally the voucher.
         After creation, a user can login to Vouchery and change the campaigns, and
         sub-campaigns name if desired. They should not change the promo code as it
-        needs to be sent form vendor-promo
+        needs to be sent from vendor-promo
         '''
         promo = promo_form.save(commit=False)
         promo.campaign_name = promo.offer.site.name
 
         self.get_campaigns(**{'name_cont': promo.campaign_name})
+        self.process_response()
+
+        if not self.is_request_success:
+            raise Exception(f"Create Promo Automate Failed: errors: {self.response_error}")
+        
+        self.is_request_success = False # Reset response flag
+
         # Checks if the Main Campaign already exists
         if not self.response_content:
             self.create_campaign(promo.campaign_name, **self.CAMPAIGN_PARAMS)
             if not self.is_request_success:
                 raise Exception(_("Create Campaing Failed"))
             promo.campaign_id = str(self.response_content['id'])
         else:
@@ -175,17 +182,17 @@
             self.is_request_success = True
             return None
         self.response_content = json.loads(self.response.content)
         if not isinstance(self.response_content, list):
             self.response_message = self.response_content.get('message')
             if self.response_content.get('type') == "Error":
                 if "error" in self.response_content:
-                    self.response_errors = self.response_content.get("error")
+                    self.response_error = self.response_content.get("error")
                 else:
-                    self.response_errors = self.response_content.get("errors")
+                    self.response_error = self.response_content.get("errors")
                 self.is_request_success = False
             else:
                 self.is_request_success = True
         else:
             if self.response.status_code == 200:
                 self.is_request_success = True
 
@@ -214,14 +221,15 @@
     #############
     # Campaigns
     def create_campaign(self, name, **optional_params):
         url = self.assemble_url([self.CAMPAIGN_URL])
 
         if not name:
             raise ValueError(_("name is required to create a campaign"))
+        
         base_payload = {
             "name": name,
         }
         payload = {**base_payload, **optional_params}
 
         self.response = requests.request("POST", url, json=payload, headers=self.get_headers())
         self.process_response()
```

### Comparing `django-vendor-promo-0.1.9/vendorpromo/tests/test_processor.py` & `django-vendor-promo-0.2.0/src/vendorpromo/tests/test_stripe.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,593 +1,546 @@
 
-from django.contrib.auth import get_user_model
-from django.test import TestCase
+# from django.contrib.auth import get_user_model
+# from django.contrib.sites.models import Site
+# from django.test import TestCase
+
+# from unittest import skipIf
+
+# from vendor.models import Offer
+# from vendor.models.utils import random_string
+
+# from vendorpromo.config import VENDOR_PROMO_PROCESSOR
+# from vendorpromo.forms import PromoForm
+# from vendorpromo.models import Promo
+# from vendorpromo.processors.stripe import VoucheryProcessor
+
+# User = get_user_model()
+
+
+
+
+# @skipIf(VENDOR_PROMO_PROCESSOR != "stripe.StripePromoProcessor", "StripePromoProcessor not set")
+# class VoucheryProcessorTests(TestCase):
+
+#     fixtures = ['user', 'unit_test']
+
+#     TEAM = "Whitemoon Dreams"
+
+#     def setUp(self):
+#         self.existing_campaigns = None
+#         self.promo_processor = VoucheryProcessor
+#         processor = self.promo_processor(Site.objects.get(pk=1))
+#         processor.get_campaigns(**{'team_eq': self.TEAM})
+#         if processor.response_content:
+#             self.existing_campaigns = [{'id': campaign['id'], 'name': campaign['name']} for campaign in processor.response_content]
+
+#     # Utils
+#     # def test_check_response_success(self, response):
+#     #     raise NotImplementedError
+
+#     # def test_check_response_fail(self, response):
+#     #     raise NotImplementedError
+
+#     # def test_get_headers_success(self):
+#     #     raise NotImplementedError
+
+#     # def test_get_headers_fail(self):
+#     #     raise NotImplementedError
+
+#     ############################
+#     # VOUCHERY API CALLS
+
+#     #############
+#     # Campaigns
+#     def test_create_campaign_success(self):
+#         campaign_name = "Django Vendor Promo Campaign"
+#         processor = self.promo_processor(Site.objects.get(pk=1))
+#         extra_params = {
+#             "type": "MainCampaign",
+#             "template": "discount",
+#             'team': self.TEAM
+#         }
+
+#         if self.existing_campaigns:
+#             if campaign_name in [campaign['name'] for campaign in self.existing_campaigns]:
+#                 campaign_id = next([campaign['id'] for campaign in self.existing_campaigns if campaign['name'] == campaign_name], None)
+#                 processor.delete_campaign(campaign_id)
+#                 processor.clear_response_variables()
+
+#         processor.create_campaign(campaign_name, **extra_params)
+#         self.assertTrue(processor.is_request_success)
+#         self.assertIn("id", processor.response_content)
+#         processor.delete_campaign(processor.response_content['id'])
+
+#     def test_create_campaign_additional_params_success(self):
+#         campaign_name = "Django Vendor Promo Campaign Description"
+#         description = 'Testing adding params'
+#         processor = self.promo_processor(Site.objects.get(pk=1))
+#         extra_params = {
+#             "type": "MainCampaign",
+#             "template": "discount",
+#             'description': description,
+#             'team': self.TEAM
+#         }
+
+#         if self.existing_campaigns:
+#             if campaign_name in [campaign['name'] for campaign in self.existing_campaigns]:
+#                 campaign_id = next([campaign['id'] for campaign in self.existing_campaigns if campaign['name'] == campaign_name])
+#                 processor.delete_campaign(campaign_id)
+#                 processor.clear_response_variables()
+
+#         processor.create_campaign(campaign_name, **extra_params)
+#         self.assertTrue(processor.is_request_success)
+#         self.assertIn("id", processor.response_content)
+#         self.assertEquals(description, processor.response_content['description'])
+#         processor.delete_campaign(processor.response_content['id'])
+
+#     def test_create_campaign_existing_name_fail(self):
+#         processor = self.promo_processor(Site.objects.get(pk=1))
+#         extra_params = {
+#             "type": "MainCampaign",
+#             "template": "discount",
+#             'team': self.TEAM
+#         }
+
+#         if not self.existing_campaigns:
+#             campaign_name = "Django Vendor Promo Campaign"
+#             extra_params = {"type": "MainCampaign", "template": "discount", 'team': self.TEAM}
+#             processor.create_campaign(campaign_name, **extra_params)
+#             processor.clear_response_variables()
+#         else:
+#             campaign_name = self.existing_campaigns[0]['name']
+
+#         processor.create_campaign(campaign_name, **extra_params)
+#         self.assertFalse(processor.is_request_success)
+
+#     def test_get_campaign_success(self):
+#         campaign_name = "Test Get Campaign"
+#         campaign_id = None
+#         extra_params = {
+#             "type": "MainCampaign",
+#             "template": "discount",
+#             'team': self.TEAM
+#         }
+
+#         if not self.existing_campaigns:
+#             create_processor = self.promo_processor(Site.objects.get(pk=1))
+#             create_processor.create_campaign(campaign_name, **extra_params)
+#             campaign_id = create_processor.response_content['id']
+#         else:
+#             campaign_id = self.existing_campaigns[0]['id']
+#             campaign_name = self.existing_campaigns[0]['name']
+
+#         processor = self.promo_processor(Site.objects.get(pk=1))
+#         processor.get_campaign(campaign_id)
+#         self.assertTrue(processor.is_request_success)
+#         self.assertEquals(campaign_name, processor.response_content['name'])
+
+#     def test_get_campaign_fail(self):
+#         processor = self.promo_processor(Site.objects.get(pk=1))
+#         processor.get_campaign(-2)
+#         self.assertFalse(processor.is_request_success)
+
+#     def test_update_campaign_success(self):
+#         campaign_name = "Test Updateing Campaign"
+#         campaign_id = None
+#         update_value = {"description": "Update campaign works"}
+#         extra_params = {
+#             "type": "MainCampaign",
+#             "template": "discount",
+#             "team": self.TEAM
+#         }
+
+#         if not self.existing_campaigns:
+#             create_processor = self.promo_processor(Site.objects.get(pk=1))
+#             create_processor.create_campaign(campaign_name, **extra_params)
+#             campaign_id = create_processor.response_content['id']
+#         else:
+#             campaign_name = self.existing_campaigns[0]['name']
+#             campaign_id = self.existing_campaigns[0]['id']
+
+#         processor = self.promo_processor(Site.objects.get(pk=1))
+#         processor.update_campaign(campaign_id, **update_value)
+#         self.assertTrue(processor.is_request_success)
+#         processor.clear_response_variables()
+#         processor.get_campaign(campaign_id)
+#         self.assertEquals(update_value['description'], processor.response_content['description'])
+
+#     def test_update_campaign_fail(self):
+#         processor = self.promo_processor(Site.objects.get(pk=1))
+#         processor.update_campaign(-2, **{"type": "MainCampaign"})
+#         self.assertFalse(processor.is_request_success)
+
+#     def test_delete_campaign_success(self):
+#         campaign_params = {
+#             "type": "MainCampaign",
+#             "template": "discount",
+#             'team': self.TEAM
+#         }
+#         create_processor = self.promo_processor(Site.objects.get(pk=1))
+#         create_processor.create_campaign(random_string(), **campaign_params)
+#         campaign_id = create_processor.response_content['id']
+
+#         processor = self.promo_processor(Site.objects.get(pk=1))
+#         processor.delete_campaign(campaign_id)
+#         self.assertTrue(processor.is_request_success)
+
+#     def test_delete_campaign_fail(self):
+#         processor = self.promo_processor(Site.objects.get(pk=1))
+#         processor.delete_campaign(-2)
+#         self.assertFalse(processor.is_request_success)
+
+#     # def test_delete_full_campaign_success(self):
+#     #     campaing_ids = []
+#     #     processor = self.promo_processor(Site.objects.get(pk=1))
+
+#     #     for campaign_id in campaing_ids:
+#     #         processor.delete_full_campaign(campaign_id)
+
+#     #     self.assertTrue(processor.is_request_success)
+
+#     #############
+#     # Reward
+#     def test_create_reward_success(self):
+#         campaign_name = random_string()
+#         campaign_id = None
+#         sub_campaign_name = random_string()
+#         sub_campaign_id = None
+#         reward_id = None
+#         processor = self.promo_processor(Site.objects.get(pk=1))
+#         campaign_params = {
+#             "type": "MainCampaign",
+#             "template": "discount",
+#             "team": self.TEAM,
+#             "status": "active"
+#         }
+#         sub_campaign_params = {
+#             "type": "SubCampaign",
+#             "template": "sub_redemption",
+#             "voucher_type": "generic",
+#             "triggers_on": "redemption",
+#             "status": "active"
+#         }
+#         reward_params = {
+#             "type": "SetDiscount",
+#             "discount_type": "percentage",
+#             "discount_value": 15
+#         }
+
+#         processor.create_campaign(campaign_name, **campaign_params)
+#         campaign_id = processor.response_content['id']
+#         processor.clear_response_variables()
+#         sub_campaign_params["parent_id"] = campaign_id
+#         processor.create_campaign(sub_campaign_name, **sub_campaign_params)
+#         sub_campaign_id = processor.response_content['id']
+#         processor.clear_response_variables()
+#         processor.create_reward(sub_campaign_id, **reward_params)
+#         reward_id = processor.response_content['id']
+
+#         processor.get_reward(reward_id)
+#         self.assertTrue(processor.is_request_success)
+#         self.assertGreater(len(processor.response_content), 0)
+
+#         processor.delete_reward(reward_id)
+#         processor.delete_campaign(sub_campaign_id)
+#         processor.delete_campaign(campaign_id)
+
+#     def test_create_reward_fail(self):
+#         processor = self.promo_processor(Site.objects.get(pk=1))
+#         processor.create_reward(-2)
+#         self.assertFalse(processor.is_request_success)
+
+#     def test_get_reward_success(self):
+#         campaign_name = random_string()
+#         campaign_id = None
+#         sub_campaign_name = random_string()
+#         sub_campaign_id = None
+#         voucher_code = random_string(length=5, check=[campaign_name, sub_campaign_name])
+#         reward_id = None
+#         processor = self.promo_processor(Site.objects.get(pk=1))
+#         campaign_params = {
+#             "type": "MainCampaign",
+#             "template": "discount",
+#             "team": self.TEAM,
+#             "status": "active"
+#         }
+#         sub_campaign_params = {
+#             "type": "SubCampaign",
+#             "template": "sub_redemption",
+#             "voucher_type": "generic",
+#             "triggers_on": "redemption",
+#             "status": "active"
+#         }
+#         reward_params = {
+#             "type": "SetDiscount",
+#             "discount_type": "percentage",
+#             "discount_value": 15
+#         }
+
+#         processor.create_campaign(campaign_name, **campaign_params)
+#         campaign_id = processor.response_content['id']
+#         processor.clear_response_variables()
+#         sub_campaign_params["parent_id"] = campaign_id
+#         processor.create_campaign(sub_campaign_name, **sub_campaign_params)
+#         sub_campaign_id = processor.response_content['id']
+#         processor.clear_response_variables()
+#         processor.create_reward(sub_campaign_id, **reward_params)
+#         reward_id = processor.response_content['id']
+#         processor.clear_response_variables()
+#         processor.create_voucher(voucher_code, campaign_id)
+#         processor.clear_response_variables()
+
+#         processor.get_reward(reward_id)
+#         self.assertTrue(processor.is_request_success)
+#         self.assertGreater(len(processor.response_content), 0)
+
+#         processor.delete_voucher(voucher_code)
+#         processor.delete_reward(reward_id)
+#         processor.delete_campaign(sub_campaign_id)
+#         processor.delete_campaign(campaign_id)
+
+#     def test_get_reward_fail(self):
+#         processor = self.promo_processor(Site.objects.get(pk=1))
+#         processor.get_reward(-2)
+#         self.assertFalse(processor.is_request_success)
+
+#     # def test_update_reward_success(self):
+#     #     raise NotImplementedError
+
+#     # def test_update_reward_fail(self):
+#     #     raise NotImplementedError
+
+#     # def test_delete_reward_success(self):
+#     #     raise NotImplementedError
+
+#     # def test_delete_reward_fail(self):
+#     #     raise NotImplementedError
+
+#     #############
+#     # Voucher
+#     def test_create_voucher_success(self):
+#         campaign_name = random_string()
+#         campaign_id = None
+#         sub_campaign_name = random_string()
+#         sub_campaign_id = None
+#         voucher_code = random_string(length=5, check=[campaign_name, sub_campaign_name])
+#         reward_id = None
+#         processor = self.promo_processor(Site.objects.get(pk=1))
+#         campaign_params = {
+#             "type": "MainCampaign",
+#             "template": "discount",
+#             "team": self.TEAM,
+#             "status": "active"
+#         }
+#         sub_campaign_params = {
+#             "type": "SubCampaign",
+#             "template": "sub_redemption",
+#             "voucher_type": "generic",
+#             "triggers_on": "redemption",
+#             "status": "active"
+#         }
+#         reward_params = {
+#             "type": "SetDiscount",
+#             "discount_type": "percentage",
+#             "discount_value": 15
+#         }
+
+#         processor.create_campaign(campaign_name, **campaign_params)
+#         campaign_id = processor.response_content['id']
+#         processor.clear_response_variables()
+#         sub_campaign_params["parent_id"] = campaign_id
+#         processor.create_campaign(sub_campaign_name, **sub_campaign_params)
+#         sub_campaign_id = processor.response_content['id']
+#         processor.clear_response_variables()
+#         processor.create_reward(sub_campaign_id, **reward_params)
+#         reward_id = processor.response_content['id']
+#         processor.clear_response_variables()
+#         processor.create_voucher(voucher_code, sub_campaign_id)
+
+#         self.assertTrue(processor.is_request_success)
+#         self.assertIn('id', processor.response_content)
+
+#         processor.delete_voucher(voucher_code)
+#         processor.delete_reward(reward_id)
+#         processor.delete_campaign(sub_campaign_id)
+#         processor.delete_campaign(campaign_id)
+
+#     def test_create_voucher_fail(self):
+#         processor = self.promo_processor(Site.objects.get(pk=1))
+#         processor.create_voucher(random_string(), -2)
+#         self.assertFalse(processor.is_request_success)
+
+#     def test_get_vouchers_success(self):
+#         campaign_name = random_string()
+#         campaign_id = None
+#         sub_campaign_name = random_string()
+#         sub_campaign_id = None
+#         voucher_code = random_string(length=5, check=[campaign_name, sub_campaign_name])
+#         reward_id = None
+#         processor = self.promo_processor(Site.objects.get(pk=1))
+#         campaign_params = {
+#             "type": "MainCampaign",
+#             "template": "discount",
+#             "team": self.TEAM,
+#             "status": "active"
+#         }
+#         sub_campaign_params = {
+#             "type": "SubCampaign",
+#             "template": "sub_redemption",
+#             "voucher_type": "generic",
+#             "triggers_on": "redemption",
+#             "status": "active"
+#         }
+#         reward_params = {
+#             "type": "SetDiscount",
+#             "discount_type": "percentage",
+#             "discount_value": 15
+#         }
+
+#         processor.create_campaign(campaign_name, **campaign_params)
+#         campaign_id = processor.response_content['id']
+#         processor.clear_response_variables()
+#         sub_campaign_params["parent_id"] = campaign_id
+#         processor.create_campaign(sub_campaign_name, **sub_campaign_params)
+#         sub_campaign_id = processor.response_content['id']
+#         processor.clear_response_variables()
+#         processor.create_reward(sub_campaign_id, **reward_params)
+#         reward_id = processor.response_content['id']
+#         processor.clear_response_variables()
+#         processor.create_voucher(voucher_code, sub_campaign_id)
+#         processor.clear_response_variables()
+
+#         processor.get_vouchers(sub_campaign_id)
+#         self.assertTrue(processor.is_request_success)
+#         self.assertGreater(len(processor.response_content), 0)
+
+#         processor.delete_voucher(voucher_code)
+#         processor.delete_reward(reward_id)
+#         processor.delete_campaign(sub_campaign_id)
+#         processor.delete_campaign(campaign_id)
+
+#     def test_get_vouchers_fail(self):
+#         processor = self.promo_processor(Site.objects.get(pk=1))
+#         processor.get_vouchers(-2)
+#         self.assertFalse(processor.is_request_success)
+
+#     # def test_get_voucher_success(self):
+#     #     raise NotImplementedError
+
+#     # def test_get_voucher_fail(self):
+#     #     raise NotImplementedError
+
+#     # def test_update_voucher_success(self):
+#     #     raise NotImplementedError
+
+#     # def test_update_voucher_fail(self):
+#     #     raise NotImplementedError
+
+#     # def test_delete_voucher_success(self):
+#     #     raise NotImplementedError
+
+#     # def test_delete_voucher_fail(self):
+#     #     raise NotImplementedError
+
+#     #############
+#     # Redeem
+#     # def test_create_redeem_success(self):
+#     #     raise NotImplementedError
+
+#     # def test_create_redeem_fail(self):
+#     #     raise NotImplementedError
+
+#     # def test_get_redeem_success(self):
+#     #     raise NotImplementedError
+
+#     # def test_get_redeem_fail(self):
+#     #     raise NotImplementedError
+
+#     # def test_update_redeem_success(self):
+#     #     raise NotImplementedError
+
+#     # def test_update_redeem_fail(self):
+#     #     raise NotImplementedError
+
+#     # def test_delete_redeem_success(self):
+#     #     raise NotImplementedError
+
+#     # def test_delete_redeem_fail(self):
+#     #     raise NotImplementedError
+
+#     # def test_confirm_redeem_success(self):
+#     #     raise NotImplementedError
+
+#     # def test_confirm_redeem_fail(self):
+#     #     raise NotImplementedError
+
+#     ################
+#     # Promotion Management
+#     def create_promo_automate_success(self):
+#         promo_code = 'PROMO-TEST'
+#         promo_offer = Offer.objects.get(pk=1)
+#         promo_name = f"{promo_offer.name}-{promo_code}"
+#         promo_form = PromoForm({
+#             'name': promo_name,
+#             'code': promo_code,
+#             'offer': promo_offer})
+#         promo_form.is_bound = True
+#         processor = self.promo_processor(Site.objects.get(pk=1))
+
+#         processor.create_promo_automate(promo_form)
+#         self.assertTrue(processor.is_request_success)
+#         self.assertEquals(Promo.objects.all().last().code, promo_code)
+
+#         promo = Promo.objects.get(name=promo_name)
+#         processor.get_campaign(promo.campaign_id)
+#         campaign_detials = processor.response_content
+#         reward_id = campaign_detials['children'][0]['rewards'][0]['id']
+#         subcampaign_id = campaign_detials['children'][0]['id']
+
+#         processor.delete_voucher(promo.code)
+#         processor.delete_reward(reward_id)
+#         processor.delete_campaign(subcampaign_id)
+#         processor.delete_campaign(campaign_detials['id'])
+
+#     # def test_create_promo_success(self, promo_form):
+#     #     raise NotImplementedError
+
+#     # def test_create_promo_fail(self, promo_form):
+#     #     raise NotImplementedError
+
+#     # def test_update_promo_success(self, promo_form):
+#     #     raise NotImplementedError
+
+#     # def test_update_promo_fail(self, promo_form):
+#     #     raise NotImplementedError
+
+#     # def test_delete_promo_success(self, promo):
+#     #     raise NotImplementedError
+
+#     # def test_delete_promo_fail(self, promo):
+#     #     raise NotImplementedError
+
+#     ################
+#     # Processor Functions
+#     # def test_is_code_valid_success(self, code):
+#     #     raise NotImplementedError
+
+#     # def test_is_code_valid_fail(self, code):
+#     #     raise NotImplementedError
+
+#     # def test_redeem_code_success(self, code):
+#     #     raise NotImplementedError
+
+#     # def test_redeem_code_fail(self, code):
+#     #     raise NotImplementedError
+
+#     # def test_confirm_redeemed_code_success(self, code):
+#     #     raise NotImplementedError
 
-from unittest import skipIf
+#     # def test_confirm_redeemed_code_fail(self, code):
+#     #     raise NotImplementedError
 
-from vendor.models import Offer
-from vendor.models.utils import random_string
+#     # def test_process_promo_success(self, offer, promo_code):
+#     #     raise NotImplementedError
 
-from vendorpromo.config import VENDOR_PROMO_PROCESSOR
-from vendorpromo.forms import PromoForm
-from vendorpromo.models import Promo
-from vendorpromo.processors.vouchery import VoucheryProcessor
-
-User = get_user_model()
-
-
-class BaseProcessorTests(TestCase):
-
-    fixtures = ['user', 'unit_test']
-
-    def setUp(self):
-        pass
-
-    # def test_create_promo_success(self):
-    #     raise NotImplementedError
-
-    # def test_create_promo_fail(self):
-    #     raise NotImplementedError
-
-    # def test_update_promo_success(self):
-    #     raise NotImplementedError
-
-    # def test_update_promo_fail(self):
-    #     raise NotImplementedError
-
-    # def test_delete_promo_success(self):
-    #     raise NotImplementedError
-
-    # def test_delete_promo_fail(self):
-    #     raise NotImplementedError
-
-    # def test_is_code_valid_success(self):
-    #     raise NotImplementedError
-
-    # def test_is_code_valid_fail(self):
-    #     raise NotImplementedError
-
-    # def test_redeem_code_success(self):
-    #     raise NotImplementedError
-
-    # def test_redeem_code_fail(self):
-    #     raise NotImplementedError
-
-    # def test_confirm_redeemed_code_success(self):
-    #     raise NotImplementedError
-
-    # def test_confirm_redeemed_code_fail(self):
-    #     raise NotImplementedError
-
-    # def test_process_promo_success(self):
-    #     raise NotImplementedError
-
-    # def test_process_promo_fail(self):
-    #     raise NotImplementedError
-
-
-@skipIf(VENDOR_PROMO_PROCESSOR != "vouchery.VoucheryProcessor", "VoucheryPromoProcessor not set")
-class VoucheryProcessorTests(TestCase):
-
-    fixtures = ['user', 'unit_test']
-
-    TEAM = "Whitemoon Dreams"
-
-    def setUp(self):
-        self.existing_campaigns = None
-        self.promo_processor = VoucheryProcessor
-        processor = self.promo_processor()
-        processor.get_campaigns(**{'team_eq': self.TEAM})
-        if processor.response_content:
-            self.existing_campaigns = [{'id': campaign['id'], 'name': campaign['name']} for campaign in processor.response_content]
-
-    # Utils
-    # def test_check_response_success(self, response):
-    #     raise NotImplementedError
-
-    # def test_check_response_fail(self, response):
-    #     raise NotImplementedError
-
-    # def test_get_headers_success(self):
-    #     raise NotImplementedError
-
-    # def test_get_headers_fail(self):
-    #     raise NotImplementedError
-
-    ############################
-    # VOUCHERY API CALLS
-
-    #############
-    # Campaigns
-    def test_create_campaign_success(self):
-        campaign_name = "Django Vendor Promo Campaign"
-        processor = self.promo_processor()
-        extra_params = {
-            "type": "MainCampaign",
-            "template": "discount",
-            'team': self.TEAM
-        }
-
-        if self.existing_campaigns:
-            if campaign_name in [campaign['name'] for campaign in self.existing_campaigns]:
-                campaign_id = next([campaign['id'] for campaign in self.existing_campaigns if campaign['name'] == campaign_name], None)
-                processor.delete_campaign(campaign_id)
-                processor.clear_response_variables()
-
-        processor.create_campaign(campaign_name, **extra_params)
-        self.assertTrue(processor.is_request_success)
-        self.assertIn("id", processor.response_content)
-        processor.delete_campaign(processor.response_content['id'])
-
-    def test_create_campaign_additional_params_success(self):
-        campaign_name = "Django Vendor Promo Campaign Description"
-        description = 'Testing adding params'
-        processor = self.promo_processor()
-        extra_params = {
-            "type": "MainCampaign",
-            "template": "discount",
-            'description': description,
-            'team': self.TEAM
-        }
-
-        if self.existing_campaigns:
-            if campaign_name in [campaign['name'] for campaign in self.existing_campaigns]:
-                campaign_id = next([campaign['id'] for campaign in self.existing_campaigns if campaign['name'] == campaign_name])
-                processor.delete_campaign(campaign_id)
-                processor.clear_response_variables()
-
-        processor.create_campaign(campaign_name, **extra_params)
-        self.assertTrue(processor.is_request_success)
-        self.assertIn("id", processor.response_content)
-        self.assertEquals(description, processor.response_content['description'])
-        processor.delete_campaign(processor.response_content['id'])
-
-    def test_create_campaign_existing_name_fail(self):
-        processor = self.promo_processor()
-        extra_params = {
-            "type": "MainCampaign",
-            "template": "discount",
-            'team': self.TEAM
-        }
-
-        if not self.existing_campaigns:
-            campaign_name = "Django Vendor Promo Campaign"
-            extra_params = {"type": "MainCampaign", "template": "discount", 'team': self.TEAM}
-            processor.create_campaign(campaign_name, **extra_params)
-            processor.clear_response_variables()
-        else:
-            campaign_name = self.existing_campaigns[0]['name']
-
-        processor.create_campaign(campaign_name, **extra_params)
-        self.assertFalse(processor.is_request_success)
-
-    def test_get_campaign_success(self):
-        campaign_name = "Test Get Campaign"
-        campaign_id = None
-        extra_params = {
-            "type": "MainCampaign",
-            "template": "discount",
-            'team': self.TEAM
-        }
-
-        if not self.existing_campaigns:
-            create_processor = self.promo_processor()
-            create_processor.create_campaign(campaign_name, **extra_params)
-            campaign_id = create_processor.response_content['id']
-        else:
-            campaign_id = self.existing_campaigns[0]['id']
-            campaign_name = self.existing_campaigns[0]['name']
-
-        processor = self.promo_processor()
-        processor.get_campaign(campaign_id)
-        self.assertTrue(processor.is_request_success)
-        self.assertEquals(campaign_name, processor.response_content['name'])
-
-    def test_get_campaign_fail(self):
-        processor = self.promo_processor()
-        processor.get_campaign(-2)
-        self.assertFalse(processor.is_request_success)
-
-    def test_update_campaign_success(self):
-        campaign_name = "Test Updateing Campaign"
-        campaign_id = None
-        update_value = {"description": "Update campaign works"}
-        extra_params = {
-            "type": "MainCampaign",
-            "template": "discount",
-            "team": self.TEAM
-        }
-
-        if not self.existing_campaigns:
-            create_processor = self.promo_processor()
-            create_processor.create_campaign(campaign_name, **extra_params)
-            campaign_id = create_processor.response_content['id']
-        else:
-            campaign_name = self.existing_campaigns[0]['name']
-            campaign_id = self.existing_campaigns[0]['id']
-
-        processor = self.promo_processor()
-        processor.update_campaign(campaign_id, **update_value)
-        self.assertTrue(processor.is_request_success)
-        processor.clear_response_variables()
-        processor.get_campaign(campaign_id)
-        self.assertEquals(update_value['description'], processor.response_content['description'])
-
-    def test_update_campaign_fail(self):
-        processor = self.promo_processor()
-        processor.update_campaign(-2, **{"type": "MainCampaign"})
-        self.assertFalse(processor.is_request_success)
-
-    def test_delete_campaign_success(self):
-        campaign_params = {
-            "type": "MainCampaign",
-            "template": "discount",
-            'team': self.TEAM
-        }
-        create_processor = self.promo_processor()
-        create_processor.create_campaign(random_string(), **campaign_params)
-        campaign_id = create_processor.response_content['id']
-
-        processor = self.promo_processor()
-        processor.delete_campaign(campaign_id)
-        self.assertTrue(processor.is_request_success)
-
-    def test_delete_campaign_fail(self):
-        processor = self.promo_processor()
-        processor.delete_campaign(-2)
-        self.assertFalse(processor.is_request_success)
-
-    # def test_delete_full_campaign_success(self):
-    #     campaing_ids = []
-    #     processor = self.promo_processor()
-
-    #     for campaign_id in campaing_ids:
-    #         processor.delete_full_campaign(campaign_id)
-
-    #     self.assertTrue(processor.is_request_success)
-
-    #############
-    # Reward
-    def test_create_reward_success(self):
-        campaign_name = random_string()
-        campaign_id = None
-        sub_campaign_name = random_string()
-        sub_campaign_id = None
-        reward_id = None
-        processor = self.promo_processor()
-        campaign_params = {
-            "type": "MainCampaign",
-            "template": "discount",
-            "team": self.TEAM,
-            "status": "active"
-        }
-        sub_campaign_params = {
-            "type": "SubCampaign",
-            "template": "sub_redemption",
-            "voucher_type": "generic",
-            "triggers_on": "redemption",
-            "status": "active"
-        }
-        reward_params = {
-            "type": "SetDiscount",
-            "discount_type": "percentage",
-            "discount_value": 15
-        }
-
-        processor.create_campaign(campaign_name, **campaign_params)
-        campaign_id = processor.response_content['id']
-        processor.clear_response_variables()
-        sub_campaign_params["parent_id"] = campaign_id
-        processor.create_campaign(sub_campaign_name, **sub_campaign_params)
-        sub_campaign_id = processor.response_content['id']
-        processor.clear_response_variables()
-        processor.create_reward(sub_campaign_id, **reward_params)
-        reward_id = processor.response_content['id']
-
-        processor.get_reward(reward_id)
-        self.assertTrue(processor.is_request_success)
-        self.assertGreater(len(processor.response_content), 0)
-
-        processor.delete_reward(reward_id)
-        processor.delete_campaign(sub_campaign_id)
-        processor.delete_campaign(campaign_id)
-
-    def test_create_reward_fail(self):
-        processor = self.promo_processor()
-        processor.create_reward(-2)
-        self.assertFalse(processor.is_request_success)
-
-    def test_get_reward_success(self):
-        campaign_name = random_string()
-        campaign_id = None
-        sub_campaign_name = random_string()
-        sub_campaign_id = None
-        voucher_code = random_string(length=5, check=[campaign_name, sub_campaign_name])
-        reward_id = None
-        processor = self.promo_processor()
-        campaign_params = {
-            "type": "MainCampaign",
-            "template": "discount",
-            "team": self.TEAM,
-            "status": "active"
-        }
-        sub_campaign_params = {
-            "type": "SubCampaign",
-            "template": "sub_redemption",
-            "voucher_type": "generic",
-            "triggers_on": "redemption",
-            "status": "active"
-        }
-        reward_params = {
-            "type": "SetDiscount",
-            "discount_type": "percentage",
-            "discount_value": 15
-        }
-
-        processor.create_campaign(campaign_name, **campaign_params)
-        campaign_id = processor.response_content['id']
-        processor.clear_response_variables()
-        sub_campaign_params["parent_id"] = campaign_id
-        processor.create_campaign(sub_campaign_name, **sub_campaign_params)
-        sub_campaign_id = processor.response_content['id']
-        processor.clear_response_variables()
-        processor.create_reward(sub_campaign_id, **reward_params)
-        reward_id = processor.response_content['id']
-        processor.clear_response_variables()
-        processor.create_voucher(voucher_code, campaign_id)
-        processor.clear_response_variables()
-
-        processor.get_reward(reward_id)
-        self.assertTrue(processor.is_request_success)
-        self.assertGreater(len(processor.response_content), 0)
-
-        processor.delete_voucher(voucher_code)
-        processor.delete_reward(reward_id)
-        processor.delete_campaign(sub_campaign_id)
-        processor.delete_campaign(campaign_id)
-
-    def test_get_reward_fail(self):
-        processor = self.promo_processor()
-        processor.get_reward(-2)
-        self.assertFalse(processor.is_request_success)
-
-    # def test_update_reward_success(self):
-    #     raise NotImplementedError
-
-    # def test_update_reward_fail(self):
-    #     raise NotImplementedError
-
-    # def test_delete_reward_success(self):
-    #     raise NotImplementedError
-
-    # def test_delete_reward_fail(self):
-    #     raise NotImplementedError
-
-    #############
-    # Voucher
-    def test_create_voucher_success(self):
-        campaign_name = random_string()
-        campaign_id = None
-        sub_campaign_name = random_string()
-        sub_campaign_id = None
-        voucher_code = random_string(length=5, check=[campaign_name, sub_campaign_name])
-        reward_id = None
-        processor = self.promo_processor()
-        campaign_params = {
-            "type": "MainCampaign",
-            "template": "discount",
-            "team": self.TEAM,
-            "status": "active"
-        }
-        sub_campaign_params = {
-            "type": "SubCampaign",
-            "template": "sub_redemption",
-            "voucher_type": "generic",
-            "triggers_on": "redemption",
-            "status": "active"
-        }
-        reward_params = {
-            "type": "SetDiscount",
-            "discount_type": "percentage",
-            "discount_value": 15
-        }
-
-        processor.create_campaign(campaign_name, **campaign_params)
-        campaign_id = processor.response_content['id']
-        processor.clear_response_variables()
-        sub_campaign_params["parent_id"] = campaign_id
-        processor.create_campaign(sub_campaign_name, **sub_campaign_params)
-        sub_campaign_id = processor.response_content['id']
-        processor.clear_response_variables()
-        processor.create_reward(sub_campaign_id, **reward_params)
-        reward_id = processor.response_content['id']
-        processor.clear_response_variables()
-        processor.create_voucher(voucher_code, sub_campaign_id)
-
-        self.assertTrue(processor.is_request_success)
-        self.assertIn('id', processor.response_content)
-
-        processor.delete_voucher(voucher_code)
-        processor.delete_reward(reward_id)
-        processor.delete_campaign(sub_campaign_id)
-        processor.delete_campaign(campaign_id)
-
-    def test_create_voucher_fail(self):
-        processor = self.promo_processor()
-        processor.create_voucher(random_string(), -2)
-        self.assertFalse(processor.is_request_success)
-
-    def test_get_vouchers_success(self):
-        campaign_name = random_string()
-        campaign_id = None
-        sub_campaign_name = random_string()
-        sub_campaign_id = None
-        voucher_code = random_string(length=5, check=[campaign_name, sub_campaign_name])
-        reward_id = None
-        processor = self.promo_processor()
-        campaign_params = {
-            "type": "MainCampaign",
-            "template": "discount",
-            "team": self.TEAM,
-            "status": "active"
-        }
-        sub_campaign_params = {
-            "type": "SubCampaign",
-            "template": "sub_redemption",
-            "voucher_type": "generic",
-            "triggers_on": "redemption",
-            "status": "active"
-        }
-        reward_params = {
-            "type": "SetDiscount",
-            "discount_type": "percentage",
-            "discount_value": 15
-        }
-
-        processor.create_campaign(campaign_name, **campaign_params)
-        campaign_id = processor.response_content['id']
-        processor.clear_response_variables()
-        sub_campaign_params["parent_id"] = campaign_id
-        processor.create_campaign(sub_campaign_name, **sub_campaign_params)
-        sub_campaign_id = processor.response_content['id']
-        processor.clear_response_variables()
-        processor.create_reward(sub_campaign_id, **reward_params)
-        reward_id = processor.response_content['id']
-        processor.clear_response_variables()
-        processor.create_voucher(voucher_code, sub_campaign_id)
-        processor.clear_response_variables()
-
-        processor.get_vouchers(sub_campaign_id)
-        self.assertTrue(processor.is_request_success)
-        self.assertGreater(len(processor.response_content), 0)
-
-        processor.delete_voucher(voucher_code)
-        processor.delete_reward(reward_id)
-        processor.delete_campaign(sub_campaign_id)
-        processor.delete_campaign(campaign_id)
-
-    def test_get_vouchers_fail(self):
-        processor = self.promo_processor()
-        processor.get_vouchers(-2)
-        self.assertFalse(processor.is_request_success)
-
-    # def test_get_voucher_success(self):
-    #     raise NotImplementedError
-
-    # def test_get_voucher_fail(self):
-    #     raise NotImplementedError
-
-    # def test_update_voucher_success(self):
-    #     raise NotImplementedError
-
-    # def test_update_voucher_fail(self):
-    #     raise NotImplementedError
-
-    # def test_delete_voucher_success(self):
-    #     raise NotImplementedError
-
-    # def test_delete_voucher_fail(self):
-    #     raise NotImplementedError
-
-    #############
-    # Redeem
-    # def test_create_redeem_success(self):
-    #     raise NotImplementedError
-
-    # def test_create_redeem_fail(self):
-    #     raise NotImplementedError
-
-    # def test_get_redeem_success(self):
-    #     raise NotImplementedError
-
-    # def test_get_redeem_fail(self):
-    #     raise NotImplementedError
-
-    # def test_update_redeem_success(self):
-    #     raise NotImplementedError
-
-    # def test_update_redeem_fail(self):
-    #     raise NotImplementedError
-
-    # def test_delete_redeem_success(self):
-    #     raise NotImplementedError
-
-    # def test_delete_redeem_fail(self):
-    #     raise NotImplementedError
-
-    # def test_confirm_redeem_success(self):
-    #     raise NotImplementedError
-
-    # def test_confirm_redeem_fail(self):
-    #     raise NotImplementedError
-
-    ################
-    # Promotion Management
-    def create_promo_automate_success(self):
-        promo_code = 'PROMO-TEST'
-        promo_offer = Offer.objects.get(pk=1)
-        promo_name = f"{promo_offer.name}-{promo_code}"
-        promo_form = PromoForm({
-            'name': promo_name,
-            'code': promo_code,
-            'offer': promo_offer})
-        promo_form.is_bound = True
-        processor = self.promo_processor()
-
-        processor.create_promo_automate(promo_form)
-        self.assertTrue(processor.is_request_success)
-        self.assertEquals(Promo.objects.all().last().code, promo_code)
-
-        promo = Promo.objects.get(name=promo_name)
-        processor.get_campaign(promo.campaign_id)
-        campaign_detials = processor.response_content
-        reward_id = campaign_detials['children'][0]['rewards'][0]['id']
-        subcampaign_id = campaign_detials['children'][0]['id']
-
-        processor.delete_voucher(promo.code)
-        processor.delete_reward(reward_id)
-        processor.delete_campaign(subcampaign_id)
-        processor.delete_campaign(campaign_detials['id'])
-
-    # def test_create_promo_success(self, promo_form):
-    #     raise NotImplementedError
-
-    # def test_create_promo_fail(self, promo_form):
-    #     raise NotImplementedError
-
-    # def test_update_promo_success(self, promo_form):
-    #     raise NotImplementedError
-
-    # def test_update_promo_fail(self, promo_form):
-    #     raise NotImplementedError
-
-    # def test_delete_promo_success(self, promo):
-    #     raise NotImplementedError
-
-    # def test_delete_promo_fail(self, promo):
-    #     raise NotImplementedError
-
-    ################
-    # Processor Functions
-    # def test_is_code_valid_success(self, code):
-    #     raise NotImplementedError
-
-    # def test_is_code_valid_fail(self, code):
-    #     raise NotImplementedError
-
-    # def test_redeem_code_success(self, code):
-    #     raise NotImplementedError
-
-    # def test_redeem_code_fail(self, code):
-    #     raise NotImplementedError
-
-    # def test_confirm_redeemed_code_success(self, code):
-    #     raise NotImplementedError
-
-    # def test_confirm_redeemed_code_fail(self, code):
-    #     raise NotImplementedError
-
-    # def test_process_promo_success(self, offer, promo_code):
-    #     raise NotImplementedError
-
-    # def test_process_promo_fail(self, offer, promo_code):
-    #     raise NotImplementedError
+#     # def test_process_promo_fail(self, offer, promo_code):
+#     #     raise NotImplementedError
```

### Comparing `django-vendor-promo-0.1.9/vendorpromo/tests/test_promo.py` & `django-vendor-promo-0.2.0/src/vendorpromo/tests/test_promo.py`

 * *Files identical despite different names*

