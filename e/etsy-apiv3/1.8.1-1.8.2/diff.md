# Comparing `tmp/etsy-apiv3-1.8.1.tar.gz` & `tmp/etsy-apiv3-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etsy-apiv3-1.8.1.tar", last modified: Mon May 22 14:07:34 2023, max compression
+gzip compressed data, was "etsy-apiv3-1.8.2.tar", last modified: Tue May 23 09:28:06 2023, max compression
```

## Comparing `etsy-apiv3-1.8.1.tar` & `etsy-apiv3-1.8.2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 14:07:34.304916 etsy-apiv3-1.8.1/
--rw-rw-rw-   0        0        0     1089 2022-11-29 15:57:22.000000 etsy-apiv3-1.8.1/LICENSE
--rw-rw-rw-   0        0        0      342 2023-05-22 14:07:34.302916 etsy-apiv3-1.8.1/PKG-INFO
--rw-rw-rw-   0        0        0     1120 2022-12-02 14:38:46.000000 etsy-apiv3-1.8.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 14:07:34.168917 etsy-apiv3-1.8.1/etsy_apiv3/
--rw-rw-rw-   0        0        0       23 2023-05-22 14:07:29.000000 etsy-apiv3-1.8.1/etsy_apiv3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:07:34.205917 etsy-apiv3-1.8.1/etsy_apiv3/exceptions/
--rw-rw-rw-   0        0        0      549 2023-05-15 08:29:30.000000 etsy-apiv3-1.8.1/etsy_apiv3/exceptions/TokenExpiredError.py
--rw-rw-rw-   0        0        0        0 2023-05-20 08:39:21.000000 etsy-apiv3-1.8.1/etsy_apiv3/exceptions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:07:34.267917 etsy-apiv3-1.8.1/etsy_apiv3/models/
--rw-rw-rw-   0        0        0      126 2023-01-05 12:58:42.000000 etsy-apiv3-1.8.1/etsy_apiv3/models/Auth.py
--rw-rw-rw-   0        0        0      293 2023-01-05 11:18:24.000000 etsy-apiv3-1.8.1/etsy_apiv3/models/File.py
--rw-rw-rw-   0        0        0      604 2022-06-06 13:20:33.000000 etsy-apiv3-1.8.1/etsy_apiv3/models/ListingImageModel.py
--rw-rw-rw-   0        0        0     3966 2023-04-25 14:30:59.000000 etsy-apiv3-1.8.1/etsy_apiv3/models/ListingModel.py
--rw-rw-rw-   0        0        0      293 2022-04-23 21:35:29.000000 etsy-apiv3-1.8.1/etsy_apiv3/models/ListingPropertyModel.py
--rw-rw-rw-   0        0        0      255 2022-11-29 15:27:15.000000 etsy-apiv3-1.8.1/etsy_apiv3/models/OfferingModel.py
--rw-rw-rw-   0        0        0     2124 2023-01-12 13:28:51.000000 etsy-apiv3-1.8.1/etsy_apiv3/models/PaymentModel.py
--rw-rw-rw-   0        0        0      116 2022-04-04 14:44:43.000000 etsy-apiv3-1.8.1/etsy_apiv3/models/PriceModel.py
--rw-rw-rw-   0        0        0      334 2022-11-29 15:27:25.000000 etsy-apiv3-1.8.1/etsy_apiv3/models/ProductModel.py
--rw-rw-rw-   0        0        0      143 2022-04-05 14:24:47.000000 etsy-apiv3-1.8.1/etsy_apiv3/models/ProductionPartnerModel.py
--rw-rw-rw-   0        0        0      303 2022-07-02 07:06:56.000000 etsy-apiv3-1.8.1/etsy_apiv3/models/PropertyValueModel.py
--rw-rw-rw-   0        0        0     1961 2022-11-29 15:27:49.000000 etsy-apiv3-1.8.1/etsy_apiv3/models/ReceiptModel.py
--rw-rw-rw-   0        0        0      199 2022-11-29 15:27:55.000000 etsy-apiv3-1.8.1/etsy_apiv3/models/RefundModel.py
--rw-rw-rw-   0        0        0      245 2023-01-05 13:51:36.000000 etsy-apiv3-1.8.1/etsy_apiv3/models/ReturnPolicyModel.py
--rw-rw-rw-   0        0        0      394 2022-04-23 16:26:45.000000 etsy-apiv3-1.8.1/etsy_apiv3/models/ReviewModel.py
--rw-rw-rw-   0        0        0      254 2022-10-15 18:09:39.000000 etsy-apiv3-1.8.1/etsy_apiv3/models/ShipmentModel.py
--rw-rw-rw-   0        0        0      293 2023-01-06 08:26:38.000000 etsy-apiv3-1.8.1/etsy_apiv3/models/ShippingCarrierModel.py
--rw-rw-rw-   0        0        0      537 2023-01-28 10:35:20.000000 etsy-apiv3-1.8.1/etsy_apiv3/models/ShippingProfileDestinationModel.py
--rw-rw-rw-   0        0        0      698 2022-11-29 15:28:16.000000 etsy-apiv3-1.8.1/etsy_apiv3/models/ShippingProfileModel.py
--rw-rw-rw-   0        0        0      381 2022-11-29 15:28:31.000000 etsy-apiv3-1.8.1/etsy_apiv3/models/ShippingProfileUpgradeModel.py
--rw-rw-rw-   0        0        0     1609 2022-07-02 07:49:17.000000 etsy-apiv3-1.8.1/etsy_apiv3/models/ShopModel.py
--rw-rw-rw-   0        0        0      171 2023-01-05 13:22:47.000000 etsy-apiv3-1.8.1/etsy_apiv3/models/ShopSection.py
--rw-rw-rw-   0        0        0      930 2023-01-06 07:39:02.000000 etsy-apiv3-1.8.1/etsy_apiv3/models/TaxonomyModel.py
--rw-rw-rw-   0        0        0      146 2023-05-15 08:25:27.000000 etsy-apiv3-1.8.1/etsy_apiv3/models/TokenModel.py
--rw-rw-rw-   0        0        0      974 2023-02-18 13:56:54.000000 etsy-apiv3-1.8.1/etsy_apiv3/models/TransactionModel.py
--rw-rw-rw-   0        0        0      187 2022-04-05 14:20:33.000000 etsy-apiv3-1.8.1/etsy_apiv3/models/TranslationModel.py
--rw-rw-rw-   0        0        0      728 2023-01-05 12:33:05.000000 etsy-apiv3-1.8.1/etsy_apiv3/models/UserModel.py
--rw-rw-rw-   0        0        0      202 2022-04-05 14:03:40.000000 etsy-apiv3-1.8.1/etsy_apiv3/models/VariationModel.py
--rw-rw-rw-   0        0        0     1224 2023-01-06 12:04:29.000000 etsy-apiv3-1.8.1/etsy_apiv3/models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:07:34.285917 etsy-apiv3-1.8.1/etsy_apiv3/resources/
--rw-rw-rw-   0        0        0    17759 2023-05-20 08:40:27.000000 etsy-apiv3-1.8.1/etsy_apiv3/resources/ListingResource.py
--rw-rw-rw-   0        0        0     2645 2023-05-20 08:40:36.000000 etsy-apiv3-1.8.1/etsy_apiv3/resources/PaymentResource.py
--rw-rw-rw-   0        0        0     5940 2023-05-20 08:40:46.000000 etsy-apiv3-1.8.1/etsy_apiv3/resources/ReceiptResource.py
--rw-rw-rw-   0        0        0     1395 2023-05-20 08:41:00.000000 etsy-apiv3-1.8.1/etsy_apiv3/resources/ReviewResource.py
--rw-rw-rw-   0        0        0     6087 2023-05-20 08:41:07.000000 etsy-apiv3-1.8.1/etsy_apiv3/resources/ShippingProfileResource.py
--rw-rw-rw-   0        0        0     2792 2023-05-20 08:41:16.000000 etsy-apiv3-1.8.1/etsy_apiv3/resources/ShopPolicyResource.py
--rw-rw-rw-   0        0        0     3810 2023-05-20 08:41:27.000000 etsy-apiv3-1.8.1/etsy_apiv3/resources/ShopResource.py
--rw-rw-rw-   0        0        0      190 2023-01-06 12:19:53.000000 etsy-apiv3-1.8.1/etsy_apiv3/resources/UserResource.py
--rw-rw-rw-   0        0        0      222 2023-01-12 13:29:03.000000 etsy-apiv3-1.8.1/etsy_apiv3/resources/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:07:34.293917 etsy-apiv3-1.8.1/etsy_apiv3/utils/
--rw-rw-rw-   0        0        0     4091 2023-04-06 13:41:59.000000 etsy-apiv3-1.8.1/etsy_apiv3/utils/APIV3.py
--rw-rw-rw-   0        0        0     5445 2023-05-22 14:07:15.000000 etsy-apiv3-1.8.1/etsy_apiv3/utils/EtsyOauth2Session.py
--rw-rw-rw-   0        0        0      474 2022-04-22 20:27:32.000000 etsy-apiv3-1.8.1/etsy_apiv3/utils/RequestException.py
--rw-rw-rw-   0        0        0      218 2022-07-02 14:30:58.000000 etsy-apiv3-1.8.1/etsy_apiv3/utils/Response.py
--rw-rw-rw-   0        0        0      154 2023-05-20 08:15:27.000000 etsy-apiv3-1.8.1/etsy_apiv3/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:07:34.201916 etsy-apiv3-1.8.1/etsy_apiv3.egg-info/
--rw-rw-rw-   0        0        0      342 2023-05-22 14:07:33.000000 etsy-apiv3-1.8.1/etsy_apiv3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1962 2023-05-22 14:07:34.000000 etsy-apiv3-1.8.1/etsy_apiv3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 14:07:33.000000 etsy-apiv3-1.8.1/etsy_apiv3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2023-05-22 14:07:33.000000 etsy-apiv3-1.8.1/etsy_apiv3.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-22 14:07:33.000000 etsy-apiv3-1.8.1/etsy_apiv3.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 14:07:34.305917 etsy-apiv3-1.8.1/setup.cfg
--rw-rw-rw-   0        0        0      746 2023-02-18 14:12:46.000000 etsy-apiv3-1.8.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:07:34.301916 etsy-apiv3-1.8.1/tests/
--rw-rw-rw-   0        0        0     2246 2023-01-12 13:49:46.000000 etsy-apiv3-1.8.1/tests/Payment.py
--rw-rw-rw-   0        0        0     3880 2023-03-15 09:02:53.000000 etsy-apiv3-1.8.1/tests/Receipt.py
--rw-rw-rw-   0        0        0        0 2023-03-15 09:02:44.000000 etsy-apiv3-1.8.1/tests/__init__.py
--rw-rw-rw-   0        0        0      539 2023-01-13 08:43:06.000000 etsy-apiv3-1.8.1/tests/taxonomy_test.py
--rw-rw-rw-   0        0        0      426 2023-01-12 11:25:14.000000 etsy-apiv3-1.8.1/tests/test_credentials.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:28:06.869431 etsy-apiv3-1.8.2/
+-rw-rw-rw-   0        0        0     1089 2022-11-29 15:57:22.000000 etsy-apiv3-1.8.2/LICENSE
+-rw-rw-rw-   0        0        0      342 2023-05-23 09:28:06.869431 etsy-apiv3-1.8.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1120 2022-12-02 14:38:46.000000 etsy-apiv3-1.8.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 09:28:06.516000 etsy-apiv3-1.8.2/etsy_apiv3/
+-rw-rw-rw-   0        0        0       23 2023-05-23 09:27:59.000000 etsy-apiv3-1.8.2/etsy_apiv3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:28:06.547248 etsy-apiv3-1.8.2/etsy_apiv3/exceptions/
+-rw-rw-rw-   0        0        0      549 2023-05-15 08:29:30.000000 etsy-apiv3-1.8.2/etsy_apiv3/exceptions/TokenExpiredError.py
+-rw-rw-rw-   0        0        0        0 2023-05-20 08:39:21.000000 etsy-apiv3-1.8.2/etsy_apiv3/exceptions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:28:06.736347 etsy-apiv3-1.8.2/etsy_apiv3/models/
+-rw-rw-rw-   0        0        0      126 2023-01-05 12:58:42.000000 etsy-apiv3-1.8.2/etsy_apiv3/models/Auth.py
+-rw-rw-rw-   0        0        0      293 2023-01-05 11:18:24.000000 etsy-apiv3-1.8.2/etsy_apiv3/models/File.py
+-rw-rw-rw-   0        0        0      604 2022-06-06 13:20:33.000000 etsy-apiv3-1.8.2/etsy_apiv3/models/ListingImageModel.py
+-rw-rw-rw-   0        0        0     3966 2023-04-25 14:30:59.000000 etsy-apiv3-1.8.2/etsy_apiv3/models/ListingModel.py
+-rw-rw-rw-   0        0        0      293 2022-04-23 21:35:29.000000 etsy-apiv3-1.8.2/etsy_apiv3/models/ListingPropertyModel.py
+-rw-rw-rw-   0        0        0      255 2022-11-29 15:27:15.000000 etsy-apiv3-1.8.2/etsy_apiv3/models/OfferingModel.py
+-rw-rw-rw-   0        0        0     2124 2023-01-12 13:28:51.000000 etsy-apiv3-1.8.2/etsy_apiv3/models/PaymentModel.py
+-rw-rw-rw-   0        0        0      116 2022-04-04 14:44:43.000000 etsy-apiv3-1.8.2/etsy_apiv3/models/PriceModel.py
+-rw-rw-rw-   0        0        0      334 2022-11-29 15:27:25.000000 etsy-apiv3-1.8.2/etsy_apiv3/models/ProductModel.py
+-rw-rw-rw-   0        0        0      143 2022-04-05 14:24:47.000000 etsy-apiv3-1.8.2/etsy_apiv3/models/ProductionPartnerModel.py
+-rw-rw-rw-   0        0        0      303 2022-07-02 07:06:56.000000 etsy-apiv3-1.8.2/etsy_apiv3/models/PropertyValueModel.py
+-rw-rw-rw-   0        0        0     1961 2022-11-29 15:27:49.000000 etsy-apiv3-1.8.2/etsy_apiv3/models/ReceiptModel.py
+-rw-rw-rw-   0        0        0      199 2022-11-29 15:27:55.000000 etsy-apiv3-1.8.2/etsy_apiv3/models/RefundModel.py
+-rw-rw-rw-   0        0        0      245 2023-01-05 13:51:36.000000 etsy-apiv3-1.8.2/etsy_apiv3/models/ReturnPolicyModel.py
+-rw-rw-rw-   0        0        0      394 2022-04-23 16:26:45.000000 etsy-apiv3-1.8.2/etsy_apiv3/models/ReviewModel.py
+-rw-rw-rw-   0        0        0      254 2022-10-15 18:09:39.000000 etsy-apiv3-1.8.2/etsy_apiv3/models/ShipmentModel.py
+-rw-rw-rw-   0        0        0      293 2023-01-06 08:26:38.000000 etsy-apiv3-1.8.2/etsy_apiv3/models/ShippingCarrierModel.py
+-rw-rw-rw-   0        0        0      537 2023-01-28 10:35:20.000000 etsy-apiv3-1.8.2/etsy_apiv3/models/ShippingProfileDestinationModel.py
+-rw-rw-rw-   0        0        0      698 2022-11-29 15:28:16.000000 etsy-apiv3-1.8.2/etsy_apiv3/models/ShippingProfileModel.py
+-rw-rw-rw-   0        0        0      381 2022-11-29 15:28:31.000000 etsy-apiv3-1.8.2/etsy_apiv3/models/ShippingProfileUpgradeModel.py
+-rw-rw-rw-   0        0        0     1609 2022-07-02 07:49:17.000000 etsy-apiv3-1.8.2/etsy_apiv3/models/ShopModel.py
+-rw-rw-rw-   0        0        0      171 2023-01-05 13:22:47.000000 etsy-apiv3-1.8.2/etsy_apiv3/models/ShopSection.py
+-rw-rw-rw-   0        0        0      930 2023-01-06 07:39:02.000000 etsy-apiv3-1.8.2/etsy_apiv3/models/TaxonomyModel.py
+-rw-rw-rw-   0        0        0      146 2023-05-15 08:25:27.000000 etsy-apiv3-1.8.2/etsy_apiv3/models/TokenModel.py
+-rw-rw-rw-   0        0        0      974 2023-02-18 13:56:54.000000 etsy-apiv3-1.8.2/etsy_apiv3/models/TransactionModel.py
+-rw-rw-rw-   0        0        0      187 2022-04-05 14:20:33.000000 etsy-apiv3-1.8.2/etsy_apiv3/models/TranslationModel.py
+-rw-rw-rw-   0        0        0      728 2023-01-05 12:33:05.000000 etsy-apiv3-1.8.2/etsy_apiv3/models/UserModel.py
+-rw-rw-rw-   0        0        0      202 2022-04-05 14:03:40.000000 etsy-apiv3-1.8.2/etsy_apiv3/models/VariationModel.py
+-rw-rw-rw-   0        0        0     1224 2023-01-06 12:04:29.000000 etsy-apiv3-1.8.2/etsy_apiv3/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:28:06.816059 etsy-apiv3-1.8.2/etsy_apiv3/resources/
+-rw-rw-rw-   0        0        0    17759 2023-05-20 08:40:27.000000 etsy-apiv3-1.8.2/etsy_apiv3/resources/ListingResource.py
+-rw-rw-rw-   0        0        0     2645 2023-05-20 08:40:36.000000 etsy-apiv3-1.8.2/etsy_apiv3/resources/PaymentResource.py
+-rw-rw-rw-   0        0        0     5940 2023-05-20 08:40:46.000000 etsy-apiv3-1.8.2/etsy_apiv3/resources/ReceiptResource.py
+-rw-rw-rw-   0        0        0     1395 2023-05-20 08:41:00.000000 etsy-apiv3-1.8.2/etsy_apiv3/resources/ReviewResource.py
+-rw-rw-rw-   0        0        0     6087 2023-05-20 08:41:07.000000 etsy-apiv3-1.8.2/etsy_apiv3/resources/ShippingProfileResource.py
+-rw-rw-rw-   0        0        0     2792 2023-05-20 08:41:16.000000 etsy-apiv3-1.8.2/etsy_apiv3/resources/ShopPolicyResource.py
+-rw-rw-rw-   0        0        0     3810 2023-05-20 08:41:27.000000 etsy-apiv3-1.8.2/etsy_apiv3/resources/ShopResource.py
+-rw-rw-rw-   0        0        0      190 2023-01-06 12:19:53.000000 etsy-apiv3-1.8.2/etsy_apiv3/resources/UserResource.py
+-rw-rw-rw-   0        0        0      222 2023-01-12 13:29:03.000000 etsy-apiv3-1.8.2/etsy_apiv3/resources/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:28:06.833648 etsy-apiv3-1.8.2/etsy_apiv3/utils/
+-rw-rw-rw-   0        0        0     4091 2023-04-06 13:41:59.000000 etsy-apiv3-1.8.2/etsy_apiv3/utils/APIV3.py
+-rw-rw-rw-   0        0        0     5382 2023-05-23 09:27:53.000000 etsy-apiv3-1.8.2/etsy_apiv3/utils/EtsyOauth2Session.py
+-rw-rw-rw-   0        0        0      474 2022-04-22 20:27:32.000000 etsy-apiv3-1.8.2/etsy_apiv3/utils/RequestException.py
+-rw-rw-rw-   0        0        0      218 2022-07-02 14:30:58.000000 etsy-apiv3-1.8.2/etsy_apiv3/utils/Response.py
+-rw-rw-rw-   0        0        0      154 2023-05-20 08:15:27.000000 etsy-apiv3-1.8.2/etsy_apiv3/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:28:06.547248 etsy-apiv3-1.8.2/etsy_apiv3.egg-info/
+-rw-rw-rw-   0        0        0      342 2023-05-23 09:28:06.000000 etsy-apiv3-1.8.2/etsy_apiv3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1962 2023-05-23 09:28:06.000000 etsy-apiv3-1.8.2/etsy_apiv3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 09:28:06.000000 etsy-apiv3-1.8.2/etsy_apiv3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2023-05-23 09:28:06.000000 etsy-apiv3-1.8.2/etsy_apiv3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-23 09:28:06.000000 etsy-apiv3-1.8.2/etsy_apiv3.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 09:28:06.869431 etsy-apiv3-1.8.2/setup.cfg
+-rw-rw-rw-   0        0        0      746 2023-02-18 14:12:46.000000 etsy-apiv3-1.8.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:28:06.869431 etsy-apiv3-1.8.2/tests/
+-rw-rw-rw-   0        0        0     2246 2023-01-12 13:49:46.000000 etsy-apiv3-1.8.2/tests/Payment.py
+-rw-rw-rw-   0        0        0     3880 2023-03-15 09:02:53.000000 etsy-apiv3-1.8.2/tests/Receipt.py
+-rw-rw-rw-   0        0        0        0 2023-03-15 09:02:44.000000 etsy-apiv3-1.8.2/tests/__init__.py
+-rw-rw-rw-   0        0        0      539 2023-01-13 08:43:06.000000 etsy-apiv3-1.8.2/tests/taxonomy_test.py
+-rw-rw-rw-   0        0        0      426 2023-01-12 11:25:14.000000 etsy-apiv3-1.8.2/tests/test_credentials.py
```

### Comparing `etsy-apiv3-1.8.1/LICENSE` & `etsy-apiv3-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.8.1/README.md` & `etsy-apiv3-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.8.1/etsy_apiv3/exceptions/TokenExpiredError.py` & `etsy-apiv3-1.8.2/etsy_apiv3/exceptions/TokenExpiredError.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.8.1/etsy_apiv3/models/ListingImageModel.py` & `etsy-apiv3-1.8.2/etsy_apiv3/models/ListingImageModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.8.1/etsy_apiv3/models/ListingModel.py` & `etsy-apiv3-1.8.2/etsy_apiv3/models/ListingModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.8.1/etsy_apiv3/models/PaymentModel.py` & `etsy-apiv3-1.8.2/etsy_apiv3/models/PaymentModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.8.1/etsy_apiv3/models/ReceiptModel.py` & `etsy-apiv3-1.8.2/etsy_apiv3/models/ReceiptModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.8.1/etsy_apiv3/models/ShippingProfileDestinationModel.py` & `etsy-apiv3-1.8.2/etsy_apiv3/models/ShippingProfileDestinationModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.8.1/etsy_apiv3/models/ShippingProfileModel.py` & `etsy-apiv3-1.8.2/etsy_apiv3/models/ShippingProfileModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.8.1/etsy_apiv3/models/ShopModel.py` & `etsy-apiv3-1.8.2/etsy_apiv3/models/ShopModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.8.1/etsy_apiv3/models/TaxonomyModel.py` & `etsy-apiv3-1.8.2/etsy_apiv3/models/TaxonomyModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.8.1/etsy_apiv3/models/TransactionModel.py` & `etsy-apiv3-1.8.2/etsy_apiv3/models/TransactionModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.8.1/etsy_apiv3/models/UserModel.py` & `etsy-apiv3-1.8.2/etsy_apiv3/models/UserModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.8.1/etsy_apiv3/models/__init__.py` & `etsy-apiv3-1.8.2/etsy_apiv3/models/__init__.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.8.1/etsy_apiv3/resources/ListingResource.py` & `etsy-apiv3-1.8.2/etsy_apiv3/resources/ListingResource.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.8.1/etsy_apiv3/resources/PaymentResource.py` & `etsy-apiv3-1.8.2/etsy_apiv3/resources/PaymentResource.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.8.1/etsy_apiv3/resources/ReceiptResource.py` & `etsy-apiv3-1.8.2/etsy_apiv3/resources/ReceiptResource.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.8.1/etsy_apiv3/resources/ReviewResource.py` & `etsy-apiv3-1.8.2/etsy_apiv3/resources/ReviewResource.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.8.1/etsy_apiv3/resources/ShippingProfileResource.py` & `etsy-apiv3-1.8.2/etsy_apiv3/resources/ShippingProfileResource.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.8.1/etsy_apiv3/resources/ShopPolicyResource.py` & `etsy-apiv3-1.8.2/etsy_apiv3/resources/ShopPolicyResource.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.8.1/etsy_apiv3/resources/ShopResource.py` & `etsy-apiv3-1.8.2/etsy_apiv3/resources/ShopResource.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.8.1/etsy_apiv3/utils/APIV3.py` & `etsy-apiv3-1.8.2/etsy_apiv3/utils/APIV3.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.8.1/etsy_apiv3/utils/EtsyOauth2Session.py` & `etsy-apiv3-1.8.2/etsy_apiv3/utils/EtsyOauth2Session.py`

 * *Files 5% similar despite different names*

```diff
@@ -116,21 +116,20 @@
             raise EtsyRequestException(res.status_code, res_json["error"])
             
         
     
 
 class EtsyOauth2Helper:
     
-    def authorize(self, client_id: str, client_secret: str, redirect_uri: str, scopes: List[str], state: str = "superuser", code_challange: str = None) -> str:
+    def authorize(self, client_id: str, redirect_uri: str, scopes: List[str], state: str = "superuser", code_challange: str = None) -> str:
         authorize_url = URL(AUTH_CONNECT_ENDPOINT, params={
             "response_type": "code",
             "client_id": client_id,
-            "client_secret": client_secret,
             "redirect_uri": redirect_uri,
-            "scope": ",".join(scopes),
+            "scope": "%20".join(scopes),
             "code_challenge": code_challange,
             "state": state,
             "code_challenge_method": "S256"
         })
         print(f"Go to the following URL: {authorize_url}")
         return authorize_url
```

### Comparing `etsy-apiv3-1.8.1/etsy_apiv3.egg-info/SOURCES.txt` & `etsy-apiv3-1.8.2/etsy_apiv3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.8.1/setup.py` & `etsy-apiv3-1.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.8.1/tests/Payment.py` & `etsy-apiv3-1.8.2/tests/Payment.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.8.1/tests/Receipt.py` & `etsy-apiv3-1.8.2/tests/Receipt.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.8.1/tests/taxonomy_test.py` & `etsy-apiv3-1.8.2/tests/taxonomy_test.py`

 * *Files identical despite different names*

