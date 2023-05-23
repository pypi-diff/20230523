# Comparing `tmp/mindee-3.8.1.tar.gz` & `tmp/mindee-3.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mindee-3.8.1.tar", last modified: Thu May 11 14:53:19 2023, max compression
+gzip compressed data, was "mindee-3.8.2.tar", last modified: Tue May 23 13:54:57 2023, max compression
```

## Comparing `mindee-3.8.1.tar` & `mindee-3.8.2.tar`

### file list

```diff
@@ -1,147 +1,148 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.870598 mindee-3.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-11 14:52:52.000000 mindee-3.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-11 14:53:19.870598 mindee-3.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-11 14:52:52.000000 mindee-3.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.854597 mindee-3.8.1/mindee/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11467 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    21238 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.858598 mindee-3.8.1/mindee/documents/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.858598 mindee-3.8.1/mindee/documents/cropper/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/cropper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/cropper/cropper_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.858598 mindee-3.8.1/mindee/documents/custom/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/custom/custom_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.858598 mindee-3.8.1/mindee/documents/eu/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/eu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.858598 mindee-3.8.1/mindee/documents/eu/license_plate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/eu/license_plate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/eu/license_plate/license_plate_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.858598 mindee-3.8.1/mindee/documents/financial/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/financial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/financial/financial_document_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/financial/financial_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.858598 mindee-3.8.1/mindee/documents/fr/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/fr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.858598 mindee-3.8.1/mindee/documents/fr/bank_account_details/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/fr/bank_account_details/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/fr/bank_account_details/bank_account_details_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.858598 mindee-3.8.1/mindee/documents/fr/carte_grise/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/fr/carte_grise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/fr/carte_grise/carte_grise_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.858598 mindee-3.8.1/mindee/documents/fr/carte_vitale/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/fr/carte_vitale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/fr/carte_vitale/carte_vitale_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.858598 mindee-3.8.1/mindee/documents/fr/id_card/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/fr/id_card/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/fr/id_card/id_card_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.862598 mindee-3.8.1/mindee/documents/invoice/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/invoice/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/invoice/invoice_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/invoice/invoice_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/invoice/line_item_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/invoice/reconstruct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.862598 mindee-3.8.1/mindee/documents/invoice_splitter/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/invoice_splitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/invoice_splitter/invoice_splitter_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.862598 mindee-3.8.1/mindee/documents/passport/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/passport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/passport/passport_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.862598 mindee-3.8.1/mindee/documents/proof_of_address/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/proof_of_address/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/proof_of_address/proof_of_address_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.862598 mindee-3.8.1/mindee/documents/receipt/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/receipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/receipt/line_item_v5.py
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/receipt/receipt_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/receipt/receipt_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/receipt/receipt_v5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.862598 mindee-3.8.1/mindee/documents/shipping_container/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/shipping_container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/shipping_container/shipping_container_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.862598 mindee-3.8.1/mindee/documents/us/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/us/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.862598 mindee-3.8.1/mindee/documents/us/bank_check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/us/bank_check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/documents/us/bank_check/bank_check_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.866598 mindee-3.8.1/mindee/fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/fields/amount.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/fields/api_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/fields/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/fields/company_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/fields/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/fields/locale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/fields/orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/fields/payment_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/fields/position.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/fields/tax.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/fields/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.866598 mindee-3.8.1/mindee/input/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/input/page_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/input/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/response.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/version
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-11 14:52:52.000000 mindee-3.8.1/mindee/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.854597 mindee-3.8.1/mindee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-11 14:53:19.000000 mindee-3.8.1/mindee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-05-11 14:53:19.000000 mindee-3.8.1/mindee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 14:53:19.000000 mindee-3.8.1/mindee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-11 14:53:19.000000 mindee-3.8.1/mindee.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 14:53:01.000000 mindee-3.8.1/mindee.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-11 14:53:19.000000 mindee-3.8.1/mindee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-11 14:53:19.000000 mindee-3.8.1/mindee.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-11 14:52:52.000000 mindee-3.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-11 14:53:19.870598 mindee-3.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-11 14:52:52.000000 mindee-3.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.866598 mindee-3.8.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.870598 mindee-3.8.1/tests/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.870598 mindee-3.8.1/tests/documents/fr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/fr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/fr/test_bank_account_details_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/fr/test_carte_grise_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/fr/test_carte_vitale_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/fr/test_id_card_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/test_cropper_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/test_custom_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/test_financial_document_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/test_financial_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/test_invoice_splitter_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/test_invoice_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    13481 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/test_invoice_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/test_passport_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/test_proof_of_address_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/test_receipt_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/test_receipt_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/test_receipt_v5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/test_shipping_container_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.870598 mindee-3.8.1/tests/documents/us/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/us/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/documents/us/test_bank_check_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:53:19.870598 mindee-3.8.1/tests/fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/fields/test_amount.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/fields/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/fields/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/fields/test_locale.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/fields/test_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/fields/test_payment_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/fields/test_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/fields/test_tax.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/test_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-11 14:52:52.000000 mindee-3.8.1/tests/test_pkg_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.980667 mindee-3.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-23 13:54:29.000000 mindee-3.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-23 13:54:57.980667 mindee-3.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-23 13:54:29.000000 mindee-3.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.956667 mindee-3.8.2/mindee/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11467 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21238 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.960667 mindee-3.8.2/mindee/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.960667 mindee-3.8.2/mindee/documents/cropper/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/cropper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/cropper/cropper_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.960667 mindee-3.8.2/mindee/documents/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/custom/custom_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/custom/custom_v1_fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.960667 mindee-3.8.2/mindee/documents/eu/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/eu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.960667 mindee-3.8.2/mindee/documents/eu/license_plate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/eu/license_plate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/eu/license_plate/license_plate_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.960667 mindee-3.8.2/mindee/documents/financial/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/financial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/financial/financial_document_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/financial/financial_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.960667 mindee-3.8.2/mindee/documents/fr/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/fr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.960667 mindee-3.8.2/mindee/documents/fr/bank_account_details/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/fr/bank_account_details/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/fr/bank_account_details/bank_account_details_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.960667 mindee-3.8.2/mindee/documents/fr/carte_grise/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/fr/carte_grise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/fr/carte_grise/carte_grise_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.964667 mindee-3.8.2/mindee/documents/fr/carte_vitale/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/fr/carte_vitale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/fr/carte_vitale/carte_vitale_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.964667 mindee-3.8.2/mindee/documents/fr/id_card/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/fr/id_card/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/fr/id_card/id_card_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.964667 mindee-3.8.2/mindee/documents/invoice/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/invoice/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/invoice/invoice_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/invoice/invoice_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/invoice/line_item_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/invoice/reconstruct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.964667 mindee-3.8.2/mindee/documents/invoice_splitter/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/invoice_splitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/invoice_splitter/invoice_splitter_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.964667 mindee-3.8.2/mindee/documents/passport/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/passport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/passport/passport_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.964667 mindee-3.8.2/mindee/documents/proof_of_address/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/proof_of_address/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/proof_of_address/proof_of_address_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.968667 mindee-3.8.2/mindee/documents/receipt/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/receipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/receipt/line_item_v5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/receipt/receipt_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/receipt/receipt_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/receipt/receipt_v5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.968667 mindee-3.8.2/mindee/documents/shipping_container/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/shipping_container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/shipping_container/shipping_container_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.968667 mindee-3.8.2/mindee/documents/us/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/us/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.968667 mindee-3.8.2/mindee/documents/us/bank_check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/us/bank_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/us/bank_check/bank_check_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.972667 mindee-3.8.2/mindee/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/fields/amount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/fields/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/fields/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/fields/company_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/fields/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/fields/locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/fields/orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/fields/payment_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/fields/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/fields/tax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/fields/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.972667 mindee-3.8.2/mindee/input/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/input/page_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/input/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/version
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.960667 mindee-3.8.2/mindee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-23 13:54:57.000000 mindee-3.8.2/mindee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-23 13:54:57.000000 mindee-3.8.2/mindee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:54:57.000000 mindee-3.8.2/mindee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-23 13:54:57.000000 mindee-3.8.2/mindee.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:54:35.000000 mindee-3.8.2/mindee.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-23 13:54:57.000000 mindee-3.8.2/mindee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-23 13:54:57.000000 mindee-3.8.2/mindee.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-23 13:54:29.000000 mindee-3.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-23 13:54:57.980667 mindee-3.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-23 13:54:29.000000 mindee-3.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.972667 mindee-3.8.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.976667 mindee-3.8.2/tests/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.976667 mindee-3.8.2/tests/documents/fr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/fr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/fr/test_bank_account_details_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/fr/test_carte_grise_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/fr/test_carte_vitale_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/fr/test_id_card_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/test_cropper_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/test_custom_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/test_financial_document_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/test_financial_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/test_invoice_splitter_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/test_invoice_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13481 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/test_invoice_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/test_passport_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/test_proof_of_address_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/test_receipt_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/test_receipt_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/test_receipt_v5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/test_shipping_container_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.976667 mindee-3.8.2/tests/documents/us/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/us/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/us/test_bank_check_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.980667 mindee-3.8.2/tests/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/fields/test_amount.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/fields/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/fields/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/fields/test_locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/fields/test_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/fields/test_payment_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/fields/test_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/fields/test_tax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/test_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/test_pkg_versions.py
```

### Comparing `mindee-3.8.1/LICENSE` & `mindee-3.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/PKG-INFO` & `mindee-3.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindee
-Version: 3.8.1
+Version: 3.8.2
 Summary: Mindee API helper library for Python
 Home-page: https://mindee.com/
 Author: Mindee
 Author-email: devrel@mindee.com
 License: MIT
 Project-URL: Documentation, https://developers.mindee.com/docs/python-sdk
 Project-URL: Source, https://github.com/publicMindee/mindee-api-python
```

### Comparing `mindee-3.8.1/README.md` & `mindee-3.8.2/README.md`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee/cli.py` & `mindee-3.8.2/mindee/cli.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee/client.py` & `mindee-3.8.2/mindee/client.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee/documents/__init__.py` & `mindee-3.8.2/mindee/documents/__init__.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee/documents/base.py` & `mindee-3.8.2/mindee/documents/base.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee/documents/config.py` & `mindee-3.8.2/mindee/documents/config.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee/documents/cropper/cropper_v1.py` & `mindee-3.8.2/mindee/documents/cropper/cropper_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee/documents/custom/custom_v1.py` & `mindee-3.8.2/mindee/documents/custom/custom_v1.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, Optional, TypeVar
 
 from mindee.documents.base import Document, TypeApiPrediction, clean_out_string
-from mindee.fields.api_builder import ClassificationField, ListField
+from mindee.documents.custom.custom_v1_fields import ClassificationField, ListField
 
 
 class CustomV1(Document):
     fields: Dict[str, ListField]
     """Dictionary of all fields in the document"""
     classifications: Dict[str, ClassificationField]
     """Dictionary of all classifications in the document"""
```

### Comparing `mindee-3.8.1/mindee/documents/eu/license_plate/license_plate_v1.py` & `mindee-3.8.2/mindee/documents/eu/license_plate/license_plate_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee/documents/financial/financial_document_v1.py` & `mindee-3.8.2/mindee/documents/financial/financial_document_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import List, Optional, TypeVar
 
 from mindee.documents.base import Document, TypeApiPrediction, clean_out_string
 from mindee.documents.invoice.line_item_v4 import InvoiceLineItemV4
 from mindee.fields.amount import AmountField
+from mindee.fields.classification import ClassificationField
 from mindee.fields.company_registration import CompanyRegistrationField
 from mindee.fields.date import DateField
 from mindee.fields.locale import LocaleField
 from mindee.fields.payment_details import PaymentDetails
 from mindee.fields.tax import TaxField
 from mindee.fields.text import TextField
 
@@ -46,19 +47,19 @@
     """Payment details"""
     line_items: List[InvoiceLineItemV4]
     """Details of line items"""
     tip: AmountField
     """Total amount of tip and gratuity."""
     time: TextField
     """Time as seen on the receipt in HH:MM format."""
-    document_type: TextField
+    document_type: ClassificationField
     """A classification field, among predefined classes."""
-    category: TextField
+    category: ClassificationField
     """The invoice or receipt category among predefined classes."""
-    subcategory: TextField
+    subcategory: ClassificationField
     """The invoice or receipt sub-category among predefined classes."""
 
     def __init__(
         self,
         api_prediction=None,
         input_source=None,
         page_n: Optional[int] = None,
@@ -130,17 +131,21 @@
             for line_item in api_prediction["line_items"]
         ]
         self.total_amount = AmountField(api_prediction["total_amount"], page_n=page_n)
         self.total_net = AmountField(api_prediction["total_net"], page_n=page_n)
         self.total_tax = AmountField(api_prediction["total_tax"], page_n=page_n)
         self.tip = AmountField(api_prediction["tip"], page_n=page_n)
         self.time = TextField(api_prediction["time"], page_n=page_n)
-        self.document_type = TextField(api_prediction["document_type"], page_n=page_n)
-        self.category = TextField(api_prediction["category"], page_n=page_n)
-        self.subcategory = TextField(api_prediction["subcategory"], page_n=page_n)
+        self.document_type = ClassificationField(
+            api_prediction["document_type"], page_n=page_n
+        )
+        self.category = ClassificationField(api_prediction["category"], page_n=page_n)
+        self.subcategory = ClassificationField(
+            api_prediction["subcategory"], page_n=page_n
+        )
 
     def __str__(self) -> str:
         supplier_company_registrations = "; ".join(
             [str(n.value) for n in self.supplier_company_registrations]
         )
         customer_company_registrations = "; ".join(
             [str(n.value) for n in self.customer_company_registrations]
```

### Comparing `mindee-3.8.1/mindee/documents/financial/financial_v1.py` & `mindee-3.8.2/mindee/documents/financial/financial_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee/documents/fr/bank_account_details/bank_account_details_v1.py` & `mindee-3.8.2/mindee/documents/fr/bank_account_details/bank_account_details_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee/documents/fr/carte_grise/carte_grise_v1.py` & `mindee-3.8.2/mindee/documents/fr/carte_grise/carte_grise_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee/documents/fr/carte_vitale/carte_vitale_v1.py` & `mindee-3.8.2/mindee/documents/fr/carte_vitale/carte_vitale_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee/documents/fr/id_card/id_card_v1.py` & `mindee-3.8.2/mindee/documents/fr/id_card/id_card_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee/documents/invoice/checks.py` & `mindee-3.8.2/mindee/documents/invoice/checks.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee/documents/invoice/invoice_v3.py` & `mindee-3.8.2/mindee/documents/invoice/invoice_v3.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from typing import List, Optional, TypeVar
 
 from mindee.documents.base import Document, TypeApiPrediction, clean_out_string
 from mindee.documents.invoice import checks, reconstruct
 from mindee.fields.amount import AmountField
+from mindee.fields.classification import ClassificationField
 from mindee.fields.company_registration import CompanyRegistrationField
 from mindee.fields.date import DateField
 from mindee.fields.locale import LocaleField
 from mindee.fields.payment_details import PaymentDetails
 from mindee.fields.tax import TaxField
 from mindee.fields.text import TextField
 
 
 class InvoiceV3(Document):
     locale: LocaleField
     """locale information"""
+    document_type: ClassificationField
+    """Whether the document is an INVOICE or a CREDIT NOTE."""
     total_amount: AmountField
     """Total including taxes. Same as ``total_incl``."""
     total_net: AmountField
     """Total excluding taxes. Same as ``total_excl``."""
     invoice_date: DateField
     """Date the invoice was issued"""
     invoice_number: TextField
@@ -71,14 +74,17 @@
     ) -> None:
         """
         Build the object from the prediction API JSON.
 
         :param api_prediction: Raw prediction from HTTP response
         :param page_n: Page number for multi pages pdf input
         """
+        self.document_type = ClassificationField(
+            api_prediction["document_type"], page_n=page_n
+        )
         self.company_number = [
             CompanyRegistrationField(field_dict, page_n=page_n)
             for field_dict in api_prediction["company_registration"]
         ]
         self.invoice_date = DateField(api_prediction["date"], page_n=page_n)
         self.due_date = DateField(api_prediction["due_date"], page_n=page_n)
         self.invoice_number = TextField(api_prediction["invoice_number"], page_n=page_n)
```

### Comparing `mindee-3.8.1/mindee/documents/invoice/invoice_v4.py` & `mindee-3.8.2/mindee/documents/invoice/invoice_v4.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from typing import List, Optional, TypeVar
 
 from mindee.documents.base import Document, TypeApiPrediction, clean_out_string
 from mindee.documents.invoice import checks, reconstruct
 from mindee.documents.invoice.line_item_v4 import InvoiceLineItemV4
 from mindee.fields.amount import AmountField
+from mindee.fields.classification import ClassificationField
 from mindee.fields.company_registration import CompanyRegistrationField
 from mindee.fields.date import DateField
 from mindee.fields.locale import LocaleField
 from mindee.fields.payment_details import PaymentDetails
 from mindee.fields.tax import TaxField
 from mindee.fields.text import TextField
 
 
 class InvoiceV4(Document):
     locale: LocaleField
     """locale information"""
+    document_type: ClassificationField
+    """Whether the document is an INVOICE or a CREDIT NOTE."""
     total_amount: AmountField
     """Total including taxes"""
     total_net: AmountField
     """Total excluding taxes"""
     invoice_date: DateField
     """Date the invoice was issued"""
     invoice_number: TextField
@@ -76,14 +79,17 @@
     ) -> None:
         """
         Build the object from the prediction API JSON.
 
         :param api_prediction: Raw prediction from HTTP response
         :param page_n: Page number for multi pages pdf input
         """
+        self.document_type = ClassificationField(
+            api_prediction["document_type"], page_n=page_n
+        )
         self.supplier_company_registrations = [
             CompanyRegistrationField(field_dict, page_n=page_n)
             for field_dict in api_prediction["supplier_company_registrations"]
         ]
         self.invoice_date = DateField(api_prediction["date"], page_n=page_n)
         self.due_date = DateField(api_prediction["due_date"], page_n=page_n)
         self.invoice_number = TextField(api_prediction["invoice_number"], page_n=page_n)
```

### Comparing `mindee-3.8.1/mindee/documents/invoice/line_item_v4.py` & `mindee-3.8.2/mindee/documents/invoice/line_item_v4.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee/documents/invoice/reconstruct.py` & `mindee-3.8.2/mindee/documents/invoice/reconstruct.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee/documents/invoice_splitter/invoice_splitter_v1.py` & `mindee-3.8.2/mindee/documents/invoice_splitter/invoice_splitter_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee/documents/passport/passport_v1.py` & `mindee-3.8.2/mindee/documents/passport/passport_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee/documents/proof_of_address/proof_of_address_v1.py` & `mindee-3.8.2/mindee/documents/proof_of_address/proof_of_address_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee/documents/receipt/line_item_v5.py` & `mindee-3.8.2/mindee/documents/receipt/line_item_v5.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee/documents/receipt/receipt_v3.py` & `mindee-3.8.2/mindee/documents/receipt/receipt_v3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import List, Optional, TypeVar
 
 from mindee.documents.base import Document, TypeApiPrediction, clean_out_string
 from mindee.fields.amount import AmountField
 from mindee.fields.base import field_array_confidence, field_array_sum
+from mindee.fields.classification import ClassificationField
 from mindee.fields.date import DateField
 from mindee.fields.locale import LocaleField
 from mindee.fields.tax import TaxField
 from mindee.fields.text import TextField
 
 
 class ReceiptV3(Document):
@@ -14,15 +15,15 @@
     """locale information"""
     total_incl: AmountField
     """Total including taxes"""
     date: DateField
     """Date the receipt was issued"""
     time: TextField
     """Time the receipt was issued"""
-    category: TextField
+    category: ClassificationField
     """Service category"""
     merchant_name: TextField
     """Merchant's name"""
     taxes: List[TaxField]
     """List of all taxes"""
     total_tax: AmountField
     """Sum total of all taxes"""
@@ -77,15 +78,15 @@
 
         :param api_prediction: Raw prediction from HTTP response
         :param page_n: Page number for multi pages pdf input
         """
         self.locale = LocaleField(api_prediction["locale"], page_n=page_n)
         self.total_incl = AmountField(api_prediction["total_incl"], page_n=page_n)
         self.date = DateField(api_prediction["date"], page_n=page_n)
-        self.category = TextField(api_prediction["category"], page_n=page_n)
+        self.category = ClassificationField(api_prediction["category"], page_n=page_n)
         self.merchant_name = TextField(
             api_prediction["supplier"], value_key="value", page_n=page_n
         )
         self.time = TextField(api_prediction["time"], value_key="value", page_n=page_n)
         self.taxes = [
             TaxField(
                 tax_prediction,
```

### Comparing `mindee-3.8.1/mindee/documents/receipt/receipt_v4.py` & `mindee-3.8.2/mindee/documents/receipt/receipt_v4.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import List, Optional, TypeVar
 
 from mindee.documents.base import Document, TypeApiPrediction, clean_out_string
 from mindee.fields.amount import AmountField
+from mindee.fields.classification import ClassificationField
 from mindee.fields.date import DateField
 from mindee.fields.locale import LocaleField
 from mindee.fields.tax import TaxField
 from mindee.fields.text import TextField
 
 
 class ReceiptV4(Document):
@@ -13,19 +14,19 @@
     """locale information"""
     total_amount: AmountField
     """Total including taxes"""
     date: DateField
     """Date the receipt was issued"""
     time: TextField
     """Time the receipt was issued, in HH: MM format."""
-    category: TextField
+    category: ClassificationField
     """The type, or service category, of the purchase."""
-    subcategory: TextField
+    subcategory: ClassificationField
     """The receipt sub category among predefined classes."""
-    document_type: TextField
+    document_type: ClassificationField
     """Whether the document is an expense receipt or a credit card receipt."""
     supplier: TextField
     """The merchant, or supplier, as found on the receipt."""
     taxes: List[TaxField]
     """List of all taxes."""
     total_tax: AmountField
     """Total tax amount of the purchase."""
@@ -66,17 +67,21 @@
         """
         self.locale = LocaleField(api_prediction["locale"], page_n=page_n)
         self.total_amount = AmountField(api_prediction["total_amount"], page_n=page_n)
         self.total_net = AmountField(api_prediction["total_net"], page_n=page_n)
         self.total_tax = AmountField(api_prediction["total_tax"], page_n=page_n)
         self.tip = AmountField(api_prediction["tip"], page_n=page_n)
         self.date = DateField(api_prediction["date"], page_n=page_n)
-        self.category = TextField(api_prediction["category"], page_n=page_n)
-        self.subcategory = TextField(api_prediction["subcategory"], page_n=page_n)
-        self.document_type = TextField(api_prediction["document_type"], page_n=page_n)
+        self.category = ClassificationField(api_prediction["category"], page_n=page_n)
+        self.subcategory = ClassificationField(
+            api_prediction["subcategory"], page_n=page_n
+        )
+        self.document_type = ClassificationField(
+            api_prediction["document_type"], page_n=page_n
+        )
         self.supplier = TextField(
             api_prediction["supplier"], value_key="value", page_n=page_n
         )
         self.time = TextField(api_prediction["time"], value_key="value", page_n=page_n)
         self.taxes = [
             TaxField(
                 tax_prediction,
```

### Comparing `mindee-3.8.1/mindee/documents/receipt/receipt_v5.py` & `mindee-3.8.2/mindee/documents/receipt/receipt_v5.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import List, Optional, TypeVar
 
 from mindee.documents.base import Document, TypeApiPrediction, clean_out_string
 from mindee.documents.receipt.line_item_v5 import ReceiptV5LineItem
 from mindee.fields.amount import AmountField
+from mindee.fields.classification import ClassificationField
 from mindee.fields.company_registration import CompanyRegistrationField
 from mindee.fields.date import DateField
 from mindee.fields.locale import LocaleField
 from mindee.fields.tax import TaxField
 from mindee.fields.text import TextField
 
 
@@ -15,19 +16,19 @@
     """locale information"""
     total_amount: AmountField
     """The total amount paid including taxes, discounts, fees, tips, and gratuity."""
     date: DateField
     """The date the purchase was made."""
     time: TextField
     """Time of purchase with 24 hours formatting (HH:MM)."""
-    category: TextField
+    category: ClassificationField
     """The receipt category among predefined classes."""
-    subcategory: TextField
+    subcategory: ClassificationField
     """The receipt sub category among predefined classes for transport and food."""
-    document_type: TextField
+    document_type: ClassificationField
     """Whether the document is an expense receipt or a credit card receipt."""
     supplier_name: TextField
     """The name of the supplier or merchant."""
     supplier_phone_number: TextField
     """The Phone number of the supplier or merchant."""
     supplier_address: TextField
     """The address of the supplier or merchant."""
@@ -76,17 +77,21 @@
         """
         self.locale = LocaleField(api_prediction["locale"], page_n=page_n)
         self.total_amount = AmountField(api_prediction["total_amount"], page_n=page_n)
         self.total_net = AmountField(api_prediction["total_net"], page_n=page_n)
         self.total_tax = AmountField(api_prediction["total_tax"], page_n=page_n)
         self.tip = AmountField(api_prediction["tip"], page_n=page_n)
         self.date = DateField(api_prediction["date"], page_n=page_n)
-        self.category = TextField(api_prediction["category"], page_n=page_n)
-        self.subcategory = TextField(api_prediction["subcategory"], page_n=page_n)
-        self.document_type = TextField(api_prediction["document_type"], page_n=page_n)
+        self.category = ClassificationField(api_prediction["category"], page_n=page_n)
+        self.subcategory = ClassificationField(
+            api_prediction["subcategory"], page_n=page_n
+        )
+        self.document_type = ClassificationField(
+            api_prediction["document_type"], page_n=page_n
+        )
         self.supplier_name = TextField(
             api_prediction["supplier_name"], value_key="value", page_n=page_n
         )
         self.supplier_phone_number = TextField(
             api_prediction["supplier_phone_number"], value_key="value", page_n=page_n
         )
         self.supplier_address = TextField(
```

### Comparing `mindee-3.8.1/mindee/documents/shipping_container/shipping_container_v1.py` & `mindee-3.8.2/mindee/documents/shipping_container/shipping_container_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee/documents/us/bank_check/bank_check_v1.py` & `mindee-3.8.2/mindee/documents/us/bank_check/bank_check_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee/endpoints.py` & `mindee-3.8.2/mindee/endpoints.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee/fields/amount.py` & `mindee-3.8.2/mindee/fields/amount.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee/fields/api_builder.py` & `mindee-3.8.2/mindee/documents/custom/custom_v1_fields.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee/fields/base.py` & `mindee-3.8.2/mindee/fields/base.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee/fields/company_registration.py` & `mindee-3.8.2/mindee/fields/company_registration.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee/fields/date.py` & `mindee-3.8.2/mindee/fields/date.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee/fields/locale.py` & `mindee-3.8.2/mindee/fields/locale.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee/fields/orientation.py` & `mindee-3.8.2/mindee/fields/orientation.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee/fields/payment_details.py` & `mindee-3.8.2/mindee/fields/payment_details.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee/fields/position.py` & `mindee-3.8.2/mindee/fields/position.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee/fields/tax.py` & `mindee-3.8.2/mindee/fields/tax.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             self.code = str(prediction[code_key])
         except (TypeError, KeyError):
             self.code = None
         if self.code in ("N/A", "None"):
             self.code = None
 
         try:
-            self.basis = float(prediction["basis"])
+            self.basis = float(prediction["base"])
         except (ValueError, TypeError, KeyError):
             self.basis = None
 
         try:
             self.value = float(prediction[value_key])
         except (ValueError, TypeError, KeyError):
             self.value = None
```

### Comparing `mindee-3.8.1/mindee/fields/text.py` & `mindee-3.8.2/mindee/fields/text.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee/geometry.py` & `mindee-3.8.2/mindee/geometry.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee/input/page_options.py` & `mindee-3.8.2/mindee/input/page_options.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee/input/sources.py` & `mindee-3.8.2/mindee/input/sources.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee/response.py` & `mindee-3.8.2/mindee/response.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee/versions.py` & `mindee-3.8.2/mindee/versions.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/mindee.egg-info/PKG-INFO` & `mindee-3.8.2/mindee.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindee
-Version: 3.8.1
+Version: 3.8.2
 Summary: Mindee API helper library for Python
 Home-page: https://mindee.com/
 Author: Mindee
 Author-email: devrel@mindee.com
 License: MIT
 Project-URL: Documentation, https://developers.mindee.com/docs/python-sdk
 Project-URL: Source, https://github.com/publicMindee/mindee-api-python
```

### Comparing `mindee-3.8.1/mindee.egg-info/SOURCES.txt` & `mindee-3.8.2/mindee.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 mindee/documents/__init__.py
 mindee/documents/base.py
 mindee/documents/config.py
 mindee/documents/cropper/__init__.py
 mindee/documents/cropper/cropper_v1.py
 mindee/documents/custom/__init__.py
 mindee/documents/custom/custom_v1.py
+mindee/documents/custom/custom_v1_fields.py
 mindee/documents/eu/__init__.py
 mindee/documents/eu/license_plate/__init__.py
 mindee/documents/eu/license_plate/license_plate_v1.py
 mindee/documents/financial/__init__.py
 mindee/documents/financial/financial_document_v1.py
 mindee/documents/financial/financial_v1.py
 mindee/documents/fr/__init__.py
@@ -63,16 +64,16 @@
 mindee/documents/shipping_container/__init__.py
 mindee/documents/shipping_container/shipping_container_v1.py
 mindee/documents/us/__init__.py
 mindee/documents/us/bank_check/__init__.py
 mindee/documents/us/bank_check/bank_check_v1.py
 mindee/fields/__init__.py
 mindee/fields/amount.py
-mindee/fields/api_builder.py
 mindee/fields/base.py
+mindee/fields/classification.py
 mindee/fields/company_registration.py
 mindee/fields/date.py
 mindee/fields/locale.py
 mindee/fields/orientation.py
 mindee/fields/payment_details.py
 mindee/fields/position.py
 mindee/fields/tax.py
```

### Comparing `mindee-3.8.1/pyproject.toml` & `mindee-3.8.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/setup.cfg` & `mindee-3.8.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/tests/documents/fr/test_bank_account_details_v1.py` & `mindee-3.8.2/tests/documents/fr/test_bank_account_details_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/tests/documents/fr/test_carte_grise_v1.py` & `mindee-3.8.2/tests/documents/fr/test_carte_grise_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/tests/documents/fr/test_carte_vitale_v1.py` & `mindee-3.8.2/tests/documents/fr/test_carte_vitale_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/tests/documents/fr/test_id_card_v1.py` & `mindee-3.8.2/tests/documents/fr/test_id_card_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/tests/documents/test_cropper_v1.py` & `mindee-3.8.2/tests/documents/test_cropper_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/tests/documents/test_custom_v1.py` & `mindee-3.8.2/tests/documents/test_custom_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import json
 
 import pytest
 
 from mindee.documents import CustomV1
-from mindee.fields.api_builder import ClassificationField, ListField, ListFieldValue
+from mindee.documents.custom.custom_v1_fields import (
+    ClassificationField,
+    ListField,
+    ListFieldValue,
+)
 from tests import CUSTOM_DATA_DIR
 
 FILE_PATH_CUSTOM_V1_COMPLETE = f"{CUSTOM_DATA_DIR}/response_v1/complete.json"
 FILE_PATH_CUSTOM_V1_EMPTY = f"{CUSTOM_DATA_DIR}/response_v1/empty.json"
 
 
 @pytest.fixture
```

### Comparing `mindee-3.8.1/tests/documents/test_financial_document_v1.py` & `mindee-3.8.2/tests/documents/test_financial_document_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/tests/documents/test_financial_v1.py` & `mindee-3.8.2/tests/documents/test_financial_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/tests/documents/test_invoice_splitter_v1.py` & `mindee-3.8.2/tests/documents/test_invoice_splitter_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/tests/documents/test_invoice_v3.py` & `mindee-3.8.2/tests/documents/test_invoice_v3.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/tests/documents/test_invoice_v4.py` & `mindee-3.8.2/tests/documents/test_invoice_v4.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/tests/documents/test_passport_v1.py` & `mindee-3.8.2/tests/documents/test_passport_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/tests/documents/test_proof_of_address_v1.py` & `mindee-3.8.2/tests/documents/test_proof_of_address_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/tests/documents/test_receipt_v3.py` & `mindee-3.8.2/tests/documents/test_receipt_v3.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/tests/documents/test_receipt_v4.py` & `mindee-3.8.2/tests/documents/test_receipt_v4.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/tests/documents/test_receipt_v5.py` & `mindee-3.8.2/tests/documents/test_receipt_v5.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,24 +32,26 @@
 def test_doc_constructor(receipt_v5_doc_object: ReceiptV5):
     assert receipt_v5_doc_object.date.value == "2016-02-26"
     assert receipt_v5_doc_object.total_tax.value == 1.7
     doc_str = open(f"{RECEIPT_DATA_DIR}/response_v5/doc_to_string.rst").read()
     assert receipt_v5_doc_object.orientation is None
     assert receipt_v5_doc_object.date.page_n == 0
     assert str(receipt_v5_doc_object) == doc_str
+    assert receipt_v5_doc_object.taxes[0].basis == 8.5
 
 
 def test_page_constructor(receipt_v5_page_object: ReceiptV5):
     assert receipt_v5_page_object.date.value == "2016-02-26"
     assert receipt_v5_page_object.total_tax.value == 1.7
     doc_str = open(f"{RECEIPT_DATA_DIR}/response_v5/page0_to_string.rst").read()
     assert receipt_v5_page_object.orientation.value == 0
     assert receipt_v5_page_object.date.page_n == 0
     assert str(receipt_v5_page_object) == doc_str
     assert len(receipt_v5_page_object.cropper) == 0
+    assert receipt_v5_page_object.taxes[0].basis == 8.5
 
 
 def test_all_na(receipt_v5_doc_object_empty: ReceiptV5):
     assert receipt_v5_doc_object_empty.locale.value is None
     assert receipt_v5_doc_object_empty.total_amount.value is None
     assert receipt_v5_doc_object_empty.date.value is None
     assert receipt_v5_doc_object_empty.supplier_name.value is None
```

### Comparing `mindee-3.8.1/tests/documents/test_shipping_container_v1.py` & `mindee-3.8.2/tests/documents/test_shipping_container_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/tests/documents/us/test_bank_check_v1.py` & `mindee-3.8.2/tests/documents/us/test_bank_check_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/tests/fields/test_amount.py` & `mindee-3.8.2/tests/fields/test_amount.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/tests/fields/test_date.py` & `mindee-3.8.2/tests/fields/test_date.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/tests/fields/test_field.py` & `mindee-3.8.2/tests/fields/test_field.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/tests/fields/test_locale.py` & `mindee-3.8.2/tests/fields/test_locale.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/tests/fields/test_orientation.py` & `mindee-3.8.2/tests/fields/test_orientation.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/tests/fields/test_payment_details.py` & `mindee-3.8.2/tests/fields/test_payment_details.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/tests/fields/test_position.py` & `mindee-3.8.2/tests/fields/test_position.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/tests/fields/test_tax.py` & `mindee-3.8.2/tests/fields/test_tax.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/tests/test_cli.py` & `mindee-3.8.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/tests/test_client.py` & `mindee-3.8.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/tests/test_geometry.py` & `mindee-3.8.2/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/tests/test_inputs.py` & `mindee-3.8.2/tests/test_inputs.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.1/tests/test_pkg_versions.py` & `mindee-3.8.2/tests/test_pkg_versions.py`

 * *Files identical despite different names*

