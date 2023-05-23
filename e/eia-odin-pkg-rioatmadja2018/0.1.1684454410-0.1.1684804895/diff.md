# Comparing `tmp/eia-odin-pkg-rioatmadja2018-0.1.1684454410.tar.gz` & `tmp/eia-odin-pkg-rioatmadja2018-0.1.1684804895.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eia-odin-pkg-rioatmadja2018-0.1.1684454410.tar", last modified: Fri May 19 00:00:10 2023, max compression
+gzip compressed data, was "eia-odin-pkg-rioatmadja2018-0.1.1684804895.tar", last modified: Tue May 23 01:21:35 2023, max compression
```

## Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410.tar` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895.tar`

### file list

```diff
@@ -1,73 +1,76 @@
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-19 00:00:10.205639 eia-odin-pkg-rioatmadja2018-0.1.1684454410/
--rw-r--r--   0 debian    (1000) debian    (1000)     1800 2023-05-19 00:00:10.205639 eia-odin-pkg-rioatmadja2018-0.1.1684454410/PKG-INFO
--rw-r--r--   0 debian    (1000) debian    (1000)     1445 2023-04-26 16:19:11.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/README.md
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-19 00:00:10.197639 eia-odin-pkg-rioatmadja2018-0.1.1684454410/cronjob/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-05-05 04:31:42.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/cronjob/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)     3596 2023-05-18 23:59:21.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/cronjob/download_stocks_pickle.py
--rw-r--r--   0 debian    (1000) debian    (1000)     4750 2023-05-18 01:57:25.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/cronjob/forecast_padd_weekly_pricing.py
--rw-r--r--   0 debian    (1000) debian    (1000)     2682 2023-05-18 02:27:03.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/cronjob/update_odin_db.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-19 00:00:10.197639 eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-26 16:17:16.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia/__init__.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-19 00:00:10.197639 eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia/crude_oil/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-27 23:49:08.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia/crude_oil/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)      789 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia/crude_oil/consumption_sales.py
--rw-r--r--   0 debian    (1000) debian    (1000)     2176 2023-05-04 06:19:24.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia/crude_oil/import_export.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1252 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia/crude_oil/movements.py
--rw-r--r--   0 debian    (1000) debian    (1000)      888 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia/crude_oil/pricing.py
--rw-r--r--   0 debian    (1000) debian    (1000)      879 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia/crude_oil/production.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1234 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia/crude_oil/refining_processing.py
--rw-r--r--   0 debian    (1000) debian    (1000)     4067 2023-05-10 03:19:22.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia/crude_oil/stocks.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-19 00:00:10.201639 eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia/db/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-05-09 04:02:50.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia/db/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)     8279 2023-05-11 16:13:42.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia/db/odin_db.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-19 00:00:10.201639 eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia/utils/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-26 18:20:07.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia/utils/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)     5718 2023-05-18 01:57:25.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia/utils/aws_resources.py
--rw-r--r--   0 debian    (1000) debian    (1000)      534 2023-04-27 23:49:08.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia/utils/browser.py
--rw-r--r--   0 debian    (1000) debian    (1000)     3853 2023-05-09 04:02:50.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia/utils/constants.py
--rw-r--r--   0 debian    (1000) debian    (1000)      389 2023-05-14 07:07:07.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia/utils/credentials.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1004 2023-04-28 03:34:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia/utils/facets.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1590 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia/utils/tools.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-19 00:00:10.201639 eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia_odin_pkg_rioatmadja2018.egg-info/
--rw-r--r--   0 debian    (1000) debian    (1000)     1800 2023-05-19 00:00:10.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia_odin_pkg_rioatmadja2018.egg-info/PKG-INFO
--rw-r--r--   0 debian    (1000) debian    (1000)     2022 2023-05-19 00:00:10.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia_odin_pkg_rioatmadja2018.egg-info/SOURCES.txt
--rw-r--r--   0 debian    (1000) debian    (1000)        1 2023-05-19 00:00:10.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia_odin_pkg_rioatmadja2018.egg-info/dependency_links.txt
--rw-r--r--   0 debian    (1000) debian    (1000)       41 2023-05-19 00:00:10.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia_odin_pkg_rioatmadja2018.egg-info/requires.txt
--rw-r--r--   0 debian    (1000) debian    (1000)       38 2023-05-19 00:00:10.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia_odin_pkg_rioatmadja2018.egg-info/top_level.txt
--rw-r--r--   0 debian    (1000) debian    (1000)        1 2023-05-19 00:00:06.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia_odin_pkg_rioatmadja2018.egg-info/zip-safe
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-19 00:00:10.201639 eia-odin-pkg-rioatmadja2018-0.1.1684454410/images/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-26 16:17:11.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/images/__init__.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-19 00:00:10.201639 eia-odin-pkg-rioatmadja2018-0.1.1684454410/lambda_funcs/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/lambda_funcs/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)     3241 2023-05-14 06:18:32.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/lambda_funcs/lambda_function.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1645 2023-05-10 06:22:42.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/lambda_funcs/lambda_function_bulk_import.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1295 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/lambda_funcs/lambda_function_consumption_sales.py
--rw-r--r--   0 debian    (1000) debian    (1000)     3533 2023-05-04 06:41:42.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/lambda_funcs/lambda_function_crude_oil_bulk_old_ver.py
--rw-r--r--   0 debian    (1000) debian    (1000)      822 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/lambda_funcs/lambda_function_import_export.py
--rw-r--r--   0 debian    (1000) debian    (1000)      790 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/lambda_funcs/lambda_function_movements.py
--rw-r--r--   0 debian    (1000) debian    (1000)     5829 2023-05-14 06:18:32.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/lambda_funcs/lambda_function_petroleum_stocks.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1268 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/lambda_funcs/lambda_function_productions.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1332 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/lambda_funcs/lambda_function_refining_processing.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1225 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/lambda_funcs/lambda_function_stocks.py
--rw-r--r--   0 debian    (1000) debian    (1000)      821 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/lambda_funcs/lambda_function_weekly_pricing.py
--rw-r--r--   0 debian    (1000) debian    (1000)       38 2023-05-19 00:00:10.205639 eia-odin-pkg-rioatmadja2018-0.1.1684454410/setup.cfg
--rw-r--r--   0 debian    (1000) debian    (1000)     1562 2023-04-26 16:26:50.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/setup.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-19 00:00:10.201639 eia-odin-pkg-rioatmadja2018-0.1.1684454410/tests/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-27 23:49:08.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/tests/__init__.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-19 00:00:10.205639 eia-odin-pkg-rioatmadja2018-0.1.1684454410/tests/functionals/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-05-09 04:02:50.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/tests/functionals/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)      885 2023-05-09 04:02:50.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/tests/functionals/test_odin_crude_oil_bulk_imports.py
--rw-r--r--   0 debian    (1000) debian    (1000)     2854 2023-05-09 04:02:50.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/tests/functionals/test_odin_db.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1687 2023-05-11 16:13:42.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/tests/functionals/test_odin_petroleum_stocks.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-19 00:00:10.205639 eia-odin-pkg-rioatmadja2018-0.1.1684454410/tests/integrations/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/tests/integrations/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1270 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/tests/integrations/test_crude_oil_file_conversition.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-19 00:00:10.205639 eia-odin-pkg-rioatmadja2018-0.1.1684454410/tests/units/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-27 23:49:08.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/tests/units/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)      438 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/tests/units/test_crude_oil_consumption_sales.py
--rw-r--r--   0 debian    (1000) debian    (1000)      731 2023-05-04 06:19:24.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/tests/units/test_crude_oil_import_export.py
--rw-r--r--   0 debian    (1000) debian    (1000)      475 2023-04-30 22:13:11.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/tests/units/test_crude_oil_movements.py
--rw-r--r--   0 debian    (1000) debian    (1000)      879 2023-04-28 03:34:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/tests/units/test_crude_oil_production.py
--rw-r--r--   0 debian    (1000) debian    (1000)      602 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/tests/units/test_crude_oil_refining_processing.py
--rw-r--r--   0 debian    (1000) debian    (1000)     2444 2023-05-10 03:19:22.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/tests/units/test_crude_oil_stocks.py
--rw-r--r--   0 debian    (1000) debian    (1000)      992 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684454410/tests/units/test_crude_oil_weekly_price.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 01:21:35.183475 eia-odin-pkg-rioatmadja2018-0.1.1684804895/
+-rw-r--r--   0 debian    (1000) debian    (1000)     1800 2023-05-23 01:21:35.183475 eia-odin-pkg-rioatmadja2018-0.1.1684804895/PKG-INFO
+-rw-r--r--   0 debian    (1000) debian    (1000)     1445 2023-04-26 16:19:11.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/README.md
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 01:21:35.167475 eia-odin-pkg-rioatmadja2018-0.1.1684804895/cronjob/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-05-05 04:31:42.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/cronjob/__init__.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     3904 2023-05-19 03:25:49.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/cronjob/download_stocks_pickle.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     4750 2023-05-18 01:57:25.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/cronjob/forecast_padd_weekly_pricing.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     7742 2023-05-23 01:00:17.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/cronjob/get_live_gasoline_prices.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     4118 2023-05-22 23:51:19.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/cronjob/lives_gasprices_db.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     2682 2023-05-18 02:27:03.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/cronjob/update_odin_db.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 01:21:35.167475 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-26 16:17:16.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/__init__.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 01:21:35.167475 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/crude_oil/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-27 23:49:08.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/crude_oil/__init__.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      789 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/crude_oil/consumption_sales.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     2176 2023-05-04 06:19:24.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/crude_oil/import_export.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1252 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/crude_oil/movements.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      888 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/crude_oil/pricing.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      879 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/crude_oil/production.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1234 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/crude_oil/refining_processing.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     4067 2023-05-10 03:19:22.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/crude_oil/stocks.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 01:21:35.167475 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/db/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-05-09 04:02:50.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/db/__init__.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     9702 2023-05-22 23:48:16.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/db/odin_db.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 01:21:35.175475 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/utils/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-26 18:20:07.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/utils/__init__.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     5718 2023-05-18 01:57:25.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/utils/aws_resources.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      534 2023-04-27 23:49:08.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/utils/browser.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     5888 2023-05-22 06:33:23.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/utils/constants.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      389 2023-05-14 07:07:07.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/utils/credentials.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1004 2023-04-28 03:34:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/utils/facets.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1590 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/utils/tools.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 01:21:35.179475 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia_odin_pkg_rioatmadja2018.egg-info/
+-rw-r--r--   0 debian    (1000) debian    (1000)     1800 2023-05-23 01:21:35.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia_odin_pkg_rioatmadja2018.egg-info/PKG-INFO
+-rw-r--r--   0 debian    (1000) debian    (1000)     2133 2023-05-23 01:21:35.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia_odin_pkg_rioatmadja2018.egg-info/SOURCES.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)        1 2023-05-23 01:21:35.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia_odin_pkg_rioatmadja2018.egg-info/dependency_links.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)       41 2023-05-23 01:21:35.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia_odin_pkg_rioatmadja2018.egg-info/requires.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)       38 2023-05-23 01:21:35.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia_odin_pkg_rioatmadja2018.egg-info/top_level.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)        1 2023-05-23 01:21:26.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia_odin_pkg_rioatmadja2018.egg-info/zip-safe
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 01:21:35.179475 eia-odin-pkg-rioatmadja2018-0.1.1684804895/images/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-26 16:17:11.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/images/__init__.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 01:21:35.179475 eia-odin-pkg-rioatmadja2018-0.1.1684804895/lambda_funcs/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/lambda_funcs/__init__.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     3241 2023-05-14 06:18:32.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/lambda_funcs/lambda_function.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1645 2023-05-10 06:22:42.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/lambda_funcs/lambda_function_bulk_import.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1295 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/lambda_funcs/lambda_function_consumption_sales.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     3533 2023-05-04 06:41:42.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/lambda_funcs/lambda_function_crude_oil_bulk_old_ver.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      822 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/lambda_funcs/lambda_function_import_export.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      790 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/lambda_funcs/lambda_function_movements.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     5829 2023-05-14 06:18:32.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/lambda_funcs/lambda_function_petroleum_stocks.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1268 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/lambda_funcs/lambda_function_productions.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1332 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/lambda_funcs/lambda_function_refining_processing.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1225 2023-05-01 03:13:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/lambda_funcs/lambda_function_stocks.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      821 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/lambda_funcs/lambda_function_weekly_pricing.py
+-rw-r--r--   0 debian    (1000) debian    (1000)       38 2023-05-23 01:21:35.183475 eia-odin-pkg-rioatmadja2018-0.1.1684804895/setup.cfg
+-rw-r--r--   0 debian    (1000) debian    (1000)     1562 2023-04-26 16:26:50.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/setup.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 01:21:35.179475 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-27 23:49:08.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/__init__.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 01:21:35.183475 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/functionals/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-05-09 04:02:50.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/functionals/__init__.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      409 2023-05-22 23:48:16.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/functionals/test_get_live_gasprices.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      885 2023-05-09 04:02:50.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/functionals/test_odin_crude_oil_bulk_imports.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     2854 2023-05-09 04:02:50.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/functionals/test_odin_db.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1687 2023-05-11 16:13:42.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/functionals/test_odin_petroleum_stocks.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 01:21:35.183475 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/integrations/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/integrations/__init__.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1270 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/integrations/test_crude_oil_file_conversition.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-05-23 01:21:35.183475 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/units/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2023-04-27 23:49:08.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/units/__init__.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      438 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/units/test_crude_oil_consumption_sales.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      731 2023-05-04 06:19:24.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/units/test_crude_oil_import_export.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      475 2023-04-30 22:13:11.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/units/test_crude_oil_movements.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      879 2023-04-28 03:34:44.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/units/test_crude_oil_production.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      602 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/units/test_crude_oil_refining_processing.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     2444 2023-05-10 03:19:22.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/units/test_crude_oil_stocks.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      992 2023-04-30 20:40:52.000000 eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/units/test_crude_oil_weekly_price.py
```

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/PKG-INFO` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eia-odin-pkg-rioatmadja2018
-Version: 0.1.1684454410
+Version: 0.1.1684804895
 Summary: Python Wheels to interact with the EIA APIs
 Author: Rio Atmadja
 Author-email: rioatmadja2018@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.8
```

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/README.md` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/README.md`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/cronjob/download_stocks_pickle.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/cronjob/download_stocks_pickle.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 #!/usr/bin/env python3
 from eia.utils.aws_resources import get_file, write_logs, job_status
+from eia.utils.credentials import load_credentials
 import os
 import logging
 from botocore.exceptions import ClientError
 import time
 from datetime import datetime
 from typing import List,Dict
 import pandas as pd
+import subprocess 
 
 logging.basicConfig(level=logging.INFO)
 log = logging.getLogger(__name__)
 log.setLevel(logging.DEBUG)
-
+load_credentials()
 
 def download_stock_objects():
     log_events: List = []
     job_start: str = datetime.utcnow().strftime('%Y-%m-%d %H:%M:%S')
     log.debug(f"[ \033[92mOK\033[0m ] Job started at {job_start}")
     log_events.append({'timestamp': int(time.time() * 1000),
                        'message': f"Job Started at {job_start}"
@@ -30,28 +32,28 @@
                        'Colorado': 'PADD 4',
                        'California': 'PADD 5',
                        'Washington': 'PADD 5'}
 
     try:
 
         log.debug(
-            f"[ \033[92mOK\033[0m ] Downloading https://gasprice-dataset.s3.amazonaws.com/pickle_obj/sarimax_padd_area_weekly_gasoline_retail_price.pkl ...")
+            f"[ \033[92mOK\033[0m ] Downloading https://odin.s3.amazonaws.com/pickle_obj/sarimax_padd_area_weekly_gasoline_retail_price.pkl ...")
         log_events.append({'timestamp': int(time.time() * 1000),
                            'message': f"Downloading sarimax_padd_area_weekly_gasoline_retail_price.pkl at {datetime.utcnow().strftime('%Y-%m-%d %H:%M:%S')}"})
 
         computed_model: Dict = get_file(file_name="pickle_obj/sarimax_padd_area_weekly_gasoline_retail_price.pkl",
                                         bucket_name="gasprice-dataset",
                                         dst_path="/tmp/")
 
         stocks_df: 'DataFrame' = pd.read_pickle(computed_model.get('file_name'))
         stocks_df.columns = [" ".join(col.split("_")[1:]).title() for col in stocks_df.columns]
         for col in stocks_df.columns:
             file_name: str = f"pickle_obj/sarimax_crude_oil_stocks_{PADD_AREA.get(col).replace(' ', '').lower()}.pkl"
             log.debug(
-                f"[ \033[92mOK\033[0m ] Downloading https://gasprice-dataset.s3.amazonaws.com/pickle_obj/{file_name} ...")
+                f"[ \033[92mOK\033[0m ] Downloading https://odin.s3.amazonaws.com/pickle_obj/{file_name} ...")
             log_events.append({'timestamp': int(time.time() * 1000),
                                'message': f"Downloading {file_name} at {datetime.utcnow().strftime('%Y-%m-%d %H:%M:%S')}"})
 
             get_file(file_name=file_name,
                      bucket_name="gasprice-dataset",
                      dst_path="/tmp")
 
@@ -59,14 +61,19 @@
         job_status(job_title="Download completed",
                    msg=f"Your files are ready:\n{all_files}",
                    topic_arn="arn:aws:sns:us-east-1:193235400604:crude_oil_import")
 
         log_events.append({'timestamp': int(time.time() * 1000),
                            'message': f"Jobs completed at {datetime.utcnow().strftime('%Y-%m-%d %H:%M:%S')}"})
 
+        for item in os.listdir("/tmp/"):
+            if 'pkl' in item:
+                log.debug(f"[ \033[92mOK\033[0m ] Changing Permission to -rw-rw-rw for /tmp/{item}")
+                subprocess.Popen(f"chmod 666 /tmp/{item}", shell=True)
+
         write_logs(log_group_name="download_stocks_pickles",
                    log_events=log_events)
 
         log.debug(f"[ \033[92mOK\033[0m ] Job ends at {datetime.utcnow().strftime('%Y-%m-%d %H:%M:%S')}")
 
     except ClientError as e:
         job_status(job_title="Download Failed",
```

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/cronjob/forecast_padd_weekly_pricing.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/cronjob/forecast_padd_weekly_pricing.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/cronjob/update_odin_db.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/cronjob/update_odin_db.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia/crude_oil/consumption_sales.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/crude_oil/consumption_sales.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia/crude_oil/import_export.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/crude_oil/import_export.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia/crude_oil/movements.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/crude_oil/movements.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia/crude_oil/pricing.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/crude_oil/pricing.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia/crude_oil/production.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/crude_oil/production.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia/crude_oil/refining_processing.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/crude_oil/refining_processing.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia/crude_oil/stocks.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/crude_oil/stocks.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia/db/odin_db.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/db/odin_db.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #!/usr/bin/env python3
 from functools import lru_cache
 import pymysql
 from pymysql import InternalError
 import os
 import pandas as pd
+from eia.utils.constants import STATES_LOOKUP
+from datetime import datetime
 
 class OdinDB(object):
 
     @lru_cache
     def get_dashboard_data(self, tbl_name: str, limit: int = None) -> 'DataFrame':
         # period,area_name,product_name,process_name,value,units
 
@@ -231,8 +233,45 @@
                                             database=os.environ["MYSQL_DB"])
 
             df: 'DataFrame' = pd.read_sql(query, con=conn)
             conn.close()
             return df
 
         except InternalError as e:
-            raise InternalError() from e
+            raise InternalError() from e
+
+    def get_live_gasprices(self, state:str)  -> 'DataFrame':
+
+        dst_state: str = STATES_LOOKUP.get(state)
+        query: str = f"""
+            SELECT 
+                l.timestamp,
+                l.gas_station, 
+                l.country, 
+                l.city, 
+                l.address, 
+                l.zip_code, 
+                l.state, 
+                l.regular_gas, 
+                l.midgrade_gas, 
+                l.premium_gas, 
+                l.price_unit, 
+                l.star_rating,
+                l.latitude, 
+                l.longitude 
+
+            FROM live_gasoline_prices l
+            WHERE l.state = '{dst_state}' AND SUBSTRING_INDEX(l.timestamp, 'T', 1) = '{datetime.utcnow().strftime('%Y-%m-%d')}'
+            ORDER BY l.timestamp DESC 
+        """
+        try:
+            conn: 'MySQL' = pymysql.connect(host=os.environ["MYSQL_HOST"],
+                                            user=os.environ["MYSQL_USER"],
+                                            password=os.environ["MYSQL_PASSWD"],
+                                            database=os.environ["MYSQL_DB"])
+
+            df: 'DataFrame' = pd.read_sql(query, con=conn)
+            conn.close()
+            return df
+
+        except InternalError as e:
+            raise InternalError(f"Unable to execute the following query: {query}") from e
```

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia/utils/aws_resources.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/utils/aws_resources.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia/utils/browser.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/utils/browser.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia/utils/facets.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/utils/facets.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia/utils/tools.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia/utils/tools.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia_odin_pkg_rioatmadja2018.egg-info/PKG-INFO` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia_odin_pkg_rioatmadja2018.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eia-odin-pkg-rioatmadja2018
-Version: 0.1.1684454410
+Version: 0.1.1684804895
 Summary: Python Wheels to interact with the EIA APIs
 Author: Rio Atmadja
 Author-email: rioatmadja2018@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.8
```

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/eia_odin_pkg_rioatmadja2018.egg-info/SOURCES.txt` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/eia_odin_pkg_rioatmadja2018.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 README.md
 setup.py
 cronjob/__init__.py
 cronjob/download_stocks_pickle.py
 cronjob/forecast_padd_weekly_pricing.py
+cronjob/get_live_gasoline_prices.py
+cronjob/lives_gasprices_db.py
 cronjob/update_odin_db.py
 eia/__init__.py
 eia/crude_oil/__init__.py
 eia/crude_oil/consumption_sales.py
 eia/crude_oil/import_export.py
 eia/crude_oil/movements.py
 eia/crude_oil/pricing.py
@@ -39,14 +41,15 @@
 lambda_funcs/lambda_function_petroleum_stocks.py
 lambda_funcs/lambda_function_productions.py
 lambda_funcs/lambda_function_refining_processing.py
 lambda_funcs/lambda_function_stocks.py
 lambda_funcs/lambda_function_weekly_pricing.py
 tests/__init__.py
 tests/functionals/__init__.py
+tests/functionals/test_get_live_gasprices.py
 tests/functionals/test_odin_crude_oil_bulk_imports.py
 tests/functionals/test_odin_db.py
 tests/functionals/test_odin_petroleum_stocks.py
 tests/integrations/__init__.py
 tests/integrations/test_crude_oil_file_conversition.py
 tests/units/__init__.py
 tests/units/test_crude_oil_consumption_sales.py
```

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/lambda_funcs/lambda_function.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/lambda_funcs/lambda_function.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/lambda_funcs/lambda_function_bulk_import.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/lambda_funcs/lambda_function_bulk_import.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/lambda_funcs/lambda_function_consumption_sales.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/lambda_funcs/lambda_function_consumption_sales.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/lambda_funcs/lambda_function_crude_oil_bulk_old_ver.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/lambda_funcs/lambda_function_crude_oil_bulk_old_ver.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/lambda_funcs/lambda_function_import_export.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/lambda_funcs/lambda_function_import_export.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/lambda_funcs/lambda_function_movements.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/lambda_funcs/lambda_function_movements.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/lambda_funcs/lambda_function_petroleum_stocks.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/lambda_funcs/lambda_function_petroleum_stocks.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/lambda_funcs/lambda_function_productions.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/lambda_funcs/lambda_function_productions.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/lambda_funcs/lambda_function_refining_processing.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/lambda_funcs/lambda_function_refining_processing.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/lambda_funcs/lambda_function_stocks.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/lambda_funcs/lambda_function_stocks.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/lambda_funcs/lambda_function_weekly_pricing.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/lambda_funcs/lambda_function_weekly_pricing.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/setup.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/setup.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/tests/functionals/test_odin_crude_oil_bulk_imports.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/functionals/test_odin_crude_oil_bulk_imports.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/tests/functionals/test_odin_db.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/functionals/test_odin_db.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/tests/functionals/test_odin_petroleum_stocks.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/functionals/test_odin_petroleum_stocks.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/tests/integrations/test_crude_oil_file_conversition.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/integrations/test_crude_oil_file_conversition.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/tests/units/test_crude_oil_import_export.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/units/test_crude_oil_import_export.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/tests/units/test_crude_oil_production.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/units/test_crude_oil_production.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/tests/units/test_crude_oil_refining_processing.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/units/test_crude_oil_refining_processing.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/tests/units/test_crude_oil_stocks.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/units/test_crude_oil_stocks.py`

 * *Files identical despite different names*

### Comparing `eia-odin-pkg-rioatmadja2018-0.1.1684454410/tests/units/test_crude_oil_weekly_price.py` & `eia-odin-pkg-rioatmadja2018-0.1.1684804895/tests/units/test_crude_oil_weekly_price.py`

 * *Files identical despite different names*

