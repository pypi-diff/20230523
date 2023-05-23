# Comparing `tmp/eia-odin-pkg-rioatmadja2018-0.1.1684804895.tar.gz` & `tmp/eia-odin-pkg-rioatmadja2018-0.1.1684806114.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eia-odin-pkg-rioatmadja2018-0.1.1684804895.tar", last modified: Tue May 23 01:21:35 2023, max compression
+gzip compressed data, was "eia-odin-pkg-rioatmadja2018-0.1.1684806114.tar", last modified: Tue May 23 01:41:55 2023, max compression
```

## Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684804895.tar` & `eia-odin-pkg-rioatmadja2018-0.1.1684806114.tar`

### file list

```diff
@@ -1,76 +1,36 @@
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 01:21:35.183475 eia-odin-pkg-rioatmadja2018-0.1.1684804895/
--rw-r--r--   0 debian    (1000) debian    (1000)     1800 2023-05-23 01:21:35.183475 eia-odin-pkg-rioatmadja2018-0.1.1684804895/PKG-INFO
--rw-r--r--   0 debian    (1000) debian    (1000)     1445 2023-04-26 16:19:11.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/README.md
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 01:21:35.167475 eia-odin-pkg-rioatmadja2018-0.1.1684804895/cronjob/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-05-05 04:31:42.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/cronjob/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)     3904 2023-05-19 03:25:49.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/cronjob/download_stocks_pickle.py
--rw-r--r--   0 debian    (1000) debian    (1000)     4750 2023-05-18 01:57:25.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/cronjob/forecast_padd_weekly_pricing.py
--rw-r--r--   0 debian    (1000) debian    (1000)     7742 2023-05-23 01:00:17.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/cronjob/get_live_gasoline_prices.py
--rw-r--r--   0 debian    (1000) debian    (1000)     4118 2023-05-22 23:51:19.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/cronjob/lives_gasprices_db.py
--rw-r--r--   0 debian    (1000) debian    (1000)     2682 2023-05-18 02:27:03.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/cronjob/update_odin_db.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 01:21:35.167475 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-26 16:17:16.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/__init__.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 01:21:35.167475 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/crude_oil/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-27 23:49:08.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/crude_oil/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)      789 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/crude_oil/consumption_sales.py
--rw-r--r--   0 debian    (1000) debian    (1000)     2176 2023-05-04 06:19:24.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/crude_oil/import_export.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1252 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/crude_oil/movements.py
--rw-r--r--   0 debian    (1000) debian    (1000)      888 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/crude_oil/pricing.py
--rw-r--r--   0 debian    (1000) debian    (1000)      879 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/crude_oil/production.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1234 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/crude_oil/refining_processing.py
--rw-r--r--   0 debian    (1000) debian    (1000)     4067 2023-05-10 03:19:22.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/crude_oil/stocks.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 01:21:35.167475 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/db/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-05-09 04:02:50.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/db/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)     9702 2023-05-22 23:48:16.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/db/odin_db.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 01:21:35.175475 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/utils/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-26 18:20:07.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/utils/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)     5718 2023-05-18 01:57:25.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/utils/aws_resources.py
--rw-r--r--   0 debian    (1000) debian    (1000)      534 2023-04-27 23:49:08.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/utils/browser.py
--rw-r--r--   0 debian    (1000) debian    (1000)     5888 2023-05-22 06:33:23.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/utils/constants.py
--rw-r--r--   0 debian    (1000) debian    (1000)      389 2023-05-14 07:07:07.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/utils/credentials.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1004 2023-04-28 03:34:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/utils/facets.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1590 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/utils/tools.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 01:21:35.179475 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia_odin_pkg_rioatmadja2018.egg-info/
--rw-r--r--   0 debian    (1000) debian    (1000)     1800 2023-05-23 01:21:35.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia_odin_pkg_rioatmadja2018.egg-info/PKG-INFO
--rw-r--r--   0 debian    (1000) debian    (1000)     2133 2023-05-23 01:21:35.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia_odin_pkg_rioatmadja2018.egg-info/SOURCES.txt
--rw-r--r--   0 debian    (1000) debian    (1000)        1 2023-05-23 01:21:35.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia_odin_pkg_rioatmadja2018.egg-info/dependency_links.txt
--rw-r--r--   0 debian    (1000) debian    (1000)       41 2023-05-23 01:21:35.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia_odin_pkg_rioatmadja2018.egg-info/requires.txt
--rw-r--r--   0 debian    (1000) debian    (1000)       38 2023-05-23 01:21:35.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia_odin_pkg_rioatmadja2018.egg-info/top_level.txt
--rw-r--r--   0 debian    (1000) debian    (1000)        1 2023-05-23 01:21:26.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia_odin_pkg_rioatmadja2018.egg-info/zip-safe
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 01:21:35.179475 eia-odin-pkg-rioatmadja2018-0.1.1684804895/images/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-26 16:17:11.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/images/__init__.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 01:21:35.179475 eia-odin-pkg-rioatmadja2018-0.1.1684804895/lambda_funcs/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/lambda_funcs/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)     3241 2023-05-14 06:18:32.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/lambda_funcs/lambda_function.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1645 2023-05-10 06:22:42.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/lambda_funcs/lambda_function_bulk_import.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1295 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/lambda_funcs/lambda_function_consumption_sales.py
--rw-r--r--   0 debian    (1000) debian    (1000)     3533 2023-05-04 06:41:42.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/lambda_funcs/lambda_function_crude_oil_bulk_old_ver.py
--rw-r--r--   0 debian    (1000) debian    (1000)      822 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/lambda_funcs/lambda_function_import_export.py
--rw-r--r--   0 debian    (1000) debian    (1000)      790 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/lambda_funcs/lambda_function_movements.py
--rw-r--r--   0 debian    (1000) debian    (1000)     5829 2023-05-14 06:18:32.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/lambda_funcs/lambda_function_petroleum_stocks.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1268 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/lambda_funcs/lambda_function_productions.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1332 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/lambda_funcs/lambda_function_refining_processing.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1225 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/lambda_funcs/lambda_function_stocks.py
--rw-r--r--   0 debian    (1000) debian    (1000)      821 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/lambda_funcs/lambda_function_weekly_pricing.py
--rw-r--r--   0 debian    (1000) debian    (1000)       38 2023-05-23 01:21:35.183475 eia-odin-pkg-rioatmadja2018-0.1.1684804895/setup.cfg
--rw-r--r--   0 debian    (1000) debian    (1000)     1562 2023-04-26 16:26:50.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/setup.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 01:21:35.179475 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-27 23:49:08.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/__init__.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 01:21:35.183475 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/functionals/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-05-09 04:02:50.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/functionals/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)      409 2023-05-22 23:48:16.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/functionals/test_get_live_gasprices.py
--rw-r--r--   0 debian    (1000) debian    (1000)      885 2023-05-09 04:02:50.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/functionals/test_odin_crude_oil_bulk_imports.py
--rw-r--r--   0 debian    (1000) debian    (1000)     2854 2023-05-09 04:02:50.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/functionals/test_odin_db.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1687 2023-05-11 16:13:42.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/functionals/test_odin_petroleum_stocks.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 01:21:35.183475 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/integrations/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/integrations/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1270 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/integrations/test_crude_oil_file_conversition.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 01:21:35.183475 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/units/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-27 23:49:08.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/units/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)      438 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/units/test_crude_oil_consumption_sales.py
--rw-r--r--   0 debian    (1000) debian    (1000)      731 2023-05-04 06:19:24.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/units/test_crude_oil_import_export.py
--rw-r--r--   0 debian    (1000) debian    (1000)      475 2023-04-30 22:13:11.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/units/test_crude_oil_movements.py
--rw-r--r--   0 debian    (1000) debian    (1000)      879 2023-04-28 03:34:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/units/test_crude_oil_production.py
--rw-r--r--   0 debian    (1000) debian    (1000)      602 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/units/test_crude_oil_refining_processing.py
--rw-r--r--   0 debian    (1000) debian    (1000)     2444 2023-05-10 03:19:22.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/units/test_crude_oil_stocks.py
--rw-r--r--   0 debian    (1000) debian    (1000)      992 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/units/test_crude_oil_weekly_price.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 01:41:55.118422 eia-odin-pkg-rioatmadja2018-0.1.1684806114/
+-rw-r--r--   0 debian    (1000) debian    (1000)     1800 2023-05-23 01:41:55.118422 eia-odin-pkg-rioatmadja2018-0.1.1684806114/PKG-INFO
+-rw-r--r--   0 debian    (1000) debian    (1000)     1445 2023-04-26 16:19:11.000000 eia-odin-pkg-rioatmadja2018-0.1.1684806114/README.md
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 01:41:55.098422 eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-26 16:17:16.000000 eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia/__init__.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 01:41:55.098422 eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia/crude_oil/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-27 23:49:08.000000 eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia/crude_oil/__init__.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      789 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia/crude_oil/consumption_sales.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     2176 2023-05-04 06:19:24.000000 eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia/crude_oil/import_export.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1252 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia/crude_oil/movements.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      888 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia/crude_oil/pricing.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      879 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia/crude_oil/production.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1234 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia/crude_oil/refining_processing.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     4067 2023-05-10 03:19:22.000000 eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia/crude_oil/stocks.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 01:41:55.098422 eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia/db/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-05-09 04:02:50.000000 eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia/db/__init__.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     9702 2023-05-22 23:48:16.000000 eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia/db/odin_db.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 01:41:55.118422 eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia/utils/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-26 18:20:07.000000 eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia/utils/__init__.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     5718 2023-05-18 01:57:25.000000 eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia/utils/aws_resources.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      534 2023-04-27 23:49:08.000000 eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia/utils/browser.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     5888 2023-05-22 06:33:23.000000 eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia/utils/constants.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      389 2023-05-14 07:07:07.000000 eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia/utils/credentials.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1004 2023-04-28 03:34:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia/utils/facets.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1590 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia/utils/tools.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 01:41:55.118422 eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia_odin_pkg_rioatmadja2018.egg-info/
+-rw-r--r--   0 debian    (1000) debian    (1000)     1800 2023-05-23 01:41:55.000000 eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia_odin_pkg_rioatmadja2018.egg-info/PKG-INFO
+-rw-r--r--   0 debian    (1000) debian    (1000)      780 2023-05-23 01:41:55.000000 eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia_odin_pkg_rioatmadja2018.egg-info/SOURCES.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)        1 2023-05-23 01:41:55.000000 eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia_odin_pkg_rioatmadja2018.egg-info/dependency_links.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)       41 2023-05-23 01:41:55.000000 eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia_odin_pkg_rioatmadja2018.egg-info/requires.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)       11 2023-05-23 01:41:55.000000 eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia_odin_pkg_rioatmadja2018.egg-info/top_level.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)        1 2023-05-23 01:41:51.000000 eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia_odin_pkg_rioatmadja2018.egg-info/zip-safe
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 01:41:55.118422 eia-odin-pkg-rioatmadja2018-0.1.1684806114/images/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-26 16:17:11.000000 eia-odin-pkg-rioatmadja2018-0.1.1684806114/images/__init__.py
+-rw-r--r--   0 debian    (1000) debian    (1000)       38 2023-05-23 01:41:55.118422 eia-odin-pkg-rioatmadja2018-0.1.1684806114/setup.cfg
+-rw-r--r--   0 debian    (1000) debian    (1000)     1613 2023-05-23 01:41:23.000000 eia-odin-pkg-rioatmadja2018-0.1.1684806114/setup.py
```

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684804895/PKG-INFO` & `eia-odin-pkg-rioatmadja2018-0.1.1684806114/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eia-odin-pkg-rioatmadja2018
-Version: 0.1.1684804895
+Version: 0.1.1684806114
 Summary: Python Wheels to interact with the EIA APIs
 Author: Rio Atmadja
 Author-email: rioatmadja2018@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.8
```

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684804895/README.md` & `eia-odin-pkg-rioatmadja2018-0.1.1684806114/README.md`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/crude_oil/consumption_sales.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia/crude_oil/consumption_sales.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/crude_oil/import_export.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia/crude_oil/import_export.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/crude_oil/movements.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia/crude_oil/movements.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/crude_oil/pricing.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia/crude_oil/pricing.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/crude_oil/production.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia/crude_oil/production.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/crude_oil/refining_processing.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia/crude_oil/refining_processing.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/crude_oil/stocks.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia/crude_oil/stocks.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/db/odin_db.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia/db/odin_db.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/utils/aws_resources.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia/utils/aws_resources.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/utils/browser.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia/utils/browser.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/utils/constants.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia/utils/constants.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/utils/facets.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia/utils/facets.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/utils/tools.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia/utils/tools.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia_odin_pkg_rioatmadja2018.egg-info/PKG-INFO` & `eia-odin-pkg-rioatmadja2018-0.1.1684806114/eia_odin_pkg_rioatmadja2018.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eia-odin-pkg-rioatmadja2018
-Version: 0.1.1684804895
+Version: 0.1.1684806114
 Summary: Python Wheels to interact with the EIA APIs
 Author: Rio Atmadja
 Author-email: rioatmadja2018@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.8
```

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684804895/setup.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684806114/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 setup(
     name='eia-odin-pkg-rioatmadja2018',
     version=f'0.1.{VERSION_BRANCH}{int(time.time())}',
     description='Python Wheels to interact with the EIA APIs',
     long_description=open('README.md', 'r').read(),
     author='Rio Atmadja',
     author_email='rioatmadja2018@gmail.com',
-    packages=find_packages(),
+    packages=find_packages(".", exclude=["lambda_funcs", "*tests*", "cronjob"]),
     install_requires=install_requires,
     setup_requires=['pytest-runner'],
     tests_require=['pytest'],
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
```

