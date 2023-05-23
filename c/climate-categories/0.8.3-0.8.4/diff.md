# Comparing `tmp/climate_categories-0.8.3.tar.gz` & `tmp/climate_categories-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climate_categories-0.8.3.tar", last modified: Tue May 23 14:46:12 2023, max compression
+gzip compressed data, was "climate_categories-0.8.4.tar", last modified: Tue May 23 15:04:28 2023, max compression
```

## Comparing `climate_categories-0.8.3.tar` & `climate_categories-0.8.4.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-23 14:46:12.291657 climate_categories-0.8.3/
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-23 14:46:12.259657 climate_categories-0.8.3/.github/
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-23 14:46:12.259657 climate_categories-0.8.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      671 2023-04-26 09:04:13.000000 climate_categories-0.8.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      548 2023-04-26 09:04:13.000000 climate_categories-0.8.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      571 2023-04-26 09:04:13.000000 climate_categories-0.8.3/.github/ISSUE_TEMPLATE/new_categorization.md
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      369 2023-04-26 13:19:45.000000 climate_categories-0.8.3/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-23 14:46:12.259657 climate_categories-0.8.3/.github/workflows/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      963 2023-04-26 11:23:54.000000 climate_categories-0.8.3/.github/workflows/ci.yml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1331 2023-04-26 11:23:54.000000 climate_categories-0.8.3/.gitignore
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1253 2023-05-23 14:10:09.000000 climate_categories-0.8.3/.pre-commit-config.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      297 2023-04-26 13:26:25.000000 climate_categories-0.8.3/.readthedocs.yml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       38 2023-04-26 09:04:13.000000 climate_categories-0.8.3/.sourcery.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      216 2023-04-26 14:19:11.000000 climate_categories-0.8.3/AUTHORS.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     4897 2023-05-23 14:45:32.000000 climate_categories-0.8.3/CHANGELOG.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5446 2023-04-26 11:23:54.000000 climate_categories-0.8.3/CONTRIBUTING.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      696 2023-04-26 14:19:11.000000 climate_categories-0.8.3/LICENSE
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3267 2023-05-15 16:33:50.000000 climate_categories-0.8.3/Makefile
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     9300 2023-05-23 14:46:12.291657 climate_categories-0.8.3/PKG-INFO
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3386 2023-05-23 14:45:55.000000 climate_categories-0.8.3/README.rst
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-23 14:46:12.259657 climate_categories-0.8.3/climate_categories/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1949 2023-05-23 14:15:26.000000 climate_categories-0.8.3/climate_categories/__init__.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    43152 2023-05-15 16:28:37.000000 climate_categories-0.8.3/climate_categories/_categories.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    47235 2023-04-26 12:57:44.000000 climate_categories-0.8.3/climate_categories/_conversions.py
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-23 14:46:12.275657 climate_categories-0.8.3/climate_categories/data/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    48820 2023-04-26 13:51:54.000000 climate_categories-0.8.3/climate_categories/data/BURDI.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    39603 2023-04-26 13:51:50.000000 climate_categories-0.8.3/climate_categories/data/BURDI.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    91320 2023-04-26 13:52:03.000000 climate_categories-0.8.3/climate_categories/data/BURDI_class.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    64321 2023-04-26 13:51:56.000000 climate_categories-0.8.3/climate_categories/data/BURDI_class.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    84030 2023-04-26 13:49:12.000000 climate_categories-0.8.3/climate_categories/data/CRF1999.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    69834 2023-04-26 13:49:07.000000 climate_categories-0.8.3/climate_categories/data/CRF1999.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   172563 2023-04-26 13:59:42.000000 climate_categories-0.8.3/climate_categories/data/CRF2013.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   136709 2023-04-26 13:59:42.000000 climate_categories-0.8.3/climate_categories/data/CRF2013.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   213803 2023-04-26 13:59:42.000000 climate_categories-0.8.3/climate_categories/data/CRF2013_2021.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   165299 2023-04-26 13:59:42.000000 climate_categories-0.8.3/climate_categories/data/CRF2013_2021.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   214940 2023-04-26 13:59:42.000000 climate_categories-0.8.3/climate_categories/data/CRF2013_2022.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   165976 2023-04-26 13:59:42.000000 climate_categories-0.8.3/climate_categories/data/CRF2013_2022.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   215236 2023-04-26 13:59:42.000000 climate_categories-0.8.3/climate_categories/data/CRF2013_2023.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   166217 2023-04-26 13:59:42.000000 climate_categories-0.8.3/climate_categories/data/CRF2013_2023.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    85443 2023-04-26 13:51:04.000000 climate_categories-0.8.3/climate_categories/data/CRFDI.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    68686 2023-04-26 13:50:55.000000 climate_categories-0.8.3/climate_categories/data/CRFDI.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   252079 2023-04-26 13:51:45.000000 climate_categories-0.8.3/climate_categories/data/CRFDI_class.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   172924 2023-04-26 13:51:08.000000 climate_categories-0.8.3/climate_categories/data/CRFDI_class.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2039 2023-04-26 13:48:45.000000 climate_categories-0.8.3/climate_categories/data/GCB.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1795 2023-04-26 09:04:13.000000 climate_categories-0.8.3/climate_categories/data/GCB.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    60150 2023-04-26 13:49:07.000000 climate_categories-0.8.3/climate_categories/data/IPCC1996.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    51928 2023-04-26 13:49:05.000000 climate_categories-0.8.3/climate_categories/data/IPCC1996.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   146256 2023-04-26 13:48:54.000000 climate_categories-0.8.3/climate_categories/data/IPCC2006.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   126862 2023-04-26 13:48:48.000000 climate_categories-0.8.3/climate_categories/data/IPCC2006.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   149225 2023-04-26 13:49:01.000000 climate_categories-0.8.3/climate_categories/data/IPCC2006_PRIMAP.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   128959 2023-04-26 13:48:55.000000 climate_categories-0.8.3/climate_categories/data/IPCC2006_PRIMAP.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    24803 2023-04-26 13:59:42.000000 climate_categories-0.8.3/climate_categories/data/RCMIP.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    18549 2023-04-26 13:59:42.000000 climate_categories-0.8.3/climate_categories/data/RCMIP.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 09:04:13.000000 climate_categories-0.8.3/climate_categories/data/__init__.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3761 2023-04-26 09:06:11.000000 climate_categories-0.8.3/climate_categories/data/conversion.IPCC1996.IPCC2006.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    32498 2023-04-26 13:50:50.000000 climate_categories-0.8.3/climate_categories/data/gas.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    23635 2023-04-26 13:50:49.000000 climate_categories-0.8.3/climate_categories/data/gas.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-23 14:12:58.000000 climate_categories-0.8.3/climate_categories/py.typed
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      304 2023-04-26 11:23:54.000000 climate_categories-0.8.3/climate_categories/search.py
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-23 14:46:12.279657 climate_categories-0.8.3/climate_categories/tests/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       48 2023-04-26 09:04:13.000000 climate_categories-0.8.3/climate_categories/tests/__init__.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3795 2023-04-26 11:23:55.000000 climate_categories-0.8.3/climate_categories/tests/conftest.py
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-23 14:46:12.283657 climate_categories-0.8.3/climate_categories/tests/data/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 10:17:34.000000 climate_categories-0.8.3/climate_categories/tests/data/__init__.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      359 2023-04-26 09:06:11.000000 climate_categories-0.8.3/climate_categories/tests/data/broken_conversion_not_allowed.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      359 2023-04-26 09:06:11.000000 climate_categories-0.8.3/climate_categories/tests/data/broken_conversion_not_existing.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1387 2023-04-26 09:04:13.000000 climate_categories-0.8.3/climate_categories/tests/data/broken_hierarchical_categorization.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      705 2023-04-26 09:04:13.000000 climate_categories-0.8.3/climate_categories/tests/data/broken_simple_categorization.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      350 2023-04-26 09:06:11.000000 climate_categories-0.8.3/climate_categories/tests/data/good_conversion.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      650 2023-04-26 09:04:13.000000 climate_categories-0.8.3/climate_categories/tests/data/good_conversion_A.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      341 2023-04-26 09:04:13.000000 climate_categories-0.8.3/climate_categories/tests/data/good_conversion_B.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      372 2023-04-26 09:04:13.000000 climate_categories-0.8.3/climate_categories/tests/data/good_conversion_aux1.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      349 2023-04-26 09:04:13.000000 climate_categories-0.8.3/climate_categories/tests/data/good_conversion_aux2.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      350 2023-04-26 09:06:11.000000 climate_categories-0.8.3/climate_categories/tests/data/good_conversion_reversed.csv
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1387 2023-04-26 09:04:13.000000 climate_categories-0.8.3/climate_categories/tests/data/hierarchical_categorization.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      702 2023-04-26 09:04:13.000000 climate_categories-0.8.3/climate_categories/tests/data/simple_categorization.yaml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1665 2023-04-26 09:04:13.000000 climate_categories-0.8.3/climate_categories/tests/examples.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    21970 2023-05-15 16:28:37.000000 climate_categories-0.8.3/climate_categories/tests/test_climate_categories.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    14271 2023-04-26 11:23:55.000000 climate_categories-0.8.3/climate_categories/tests/test_conversions.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1205 2023-04-26 11:23:54.000000 climate_categories-0.8.3/climate_categories/tests/test_crf.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      769 2023-04-26 09:04:13.000000 climate_categories-0.8.3/climate_categories/tests/test_di.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      508 2023-04-26 09:04:13.000000 climate_categories-0.8.3/climate_categories/tests/test_gas.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1296 2023-04-26 09:04:13.000000 climate_categories-0.8.3/climate_categories/tests/test_ipcc.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     7703 2023-04-26 09:04:13.000000 climate_categories-0.8.3/climate_categories/tests/test_overcounting.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      596 2023-04-26 09:04:13.000000 climate_categories-0.8.3/climate_categories/tests/test_primap.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      305 2023-04-26 09:06:11.000000 climate_categories-0.8.3/climate_categories/tests/test_rcmip.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      649 2023-04-26 11:23:54.000000 climate_categories-0.8.3/climate_categories/tests/test_search.py
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-23 14:46:12.263657 climate_categories-0.8.3/climate_categories.egg-info/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     9300 2023-05-23 14:46:12.000000 climate_categories-0.8.3/climate_categories.egg-info/PKG-INFO
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     4029 2023-05-23 14:46:12.000000 climate_categories-0.8.3/climate_categories.egg-info/SOURCES.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        1 2023-05-23 14:46:12.000000 climate_categories-0.8.3/climate_categories.egg-info/dependency_links.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      307 2023-05-23 14:46:12.000000 climate_categories-0.8.3/climate_categories.egg-info/requires.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       19 2023-05-23 14:46:12.000000 climate_categories-0.8.3/climate_categories.egg-info/top_level.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      130 2023-04-26 09:04:13.000000 climate_categories-0.8.3/codecov.yml
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-23 14:46:12.287657 climate_categories-0.8.3/data_generation/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       62 2023-04-26 09:06:11.000000 climate_categories-0.8.3/data_generation/.gitignore
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5819 2023-04-26 13:44:45.000000 climate_categories-0.8.3/data_generation/BURDI.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3177 2023-04-26 13:44:45.000000 climate_categories-0.8.3/data_generation/BURDI_class.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    17598 2023-04-26 13:44:45.000000 climate_categories-0.8.3/data_generation/CRF1999.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    65761 2023-04-26 13:44:45.000000 climate_categories-0.8.3/data_generation/CRF2013.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    30906 2023-04-26 13:44:45.000000 climate_categories-0.8.3/data_generation/CRF2013_2021.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    31721 2023-04-26 13:44:45.000000 climate_categories-0.8.3/data_generation/CRF2013_2022.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    32225 2023-04-26 13:44:45.000000 climate_categories-0.8.3/data_generation/CRF2013_2023.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5318 2023-04-26 13:44:45.000000 climate_categories-0.8.3/data_generation/CRFDI.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5232 2023-04-26 13:44:45.000000 climate_categories-0.8.3/data_generation/CRFDI_class.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    11562 2023-04-26 13:44:45.000000 climate_categories-0.8.3/data_generation/IPCC1996.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8947 2023-04-26 13:44:45.000000 climate_categories-0.8.3/data_generation/IPCC2006.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     4254 2023-04-26 13:44:45.000000 climate_categories-0.8.3/data_generation/IPCC2006_PRIMAP.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8134 2023-04-26 13:44:45.000000 climate_categories-0.8.3/data_generation/RCMIP.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      272 2023-04-26 13:44:45.000000 climate_categories-0.8.3/data_generation/convert_yaml_to_python.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3318 2023-04-26 13:44:45.000000 climate_categories-0.8.3/data_generation/gas.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1082 2023-04-26 13:44:45.000000 climate_categories-0.8.3/data_generation/utils.py
-drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-23 14:46:12.291657 climate_categories-0.8.3/docs/
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      631 2023-04-26 09:04:13.000000 climate_categories-0.8.3/docs/Makefile
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      241 2023-04-26 09:04:13.000000 climate_categories-0.8.3/docs/api.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       30 2023-04-26 09:04:13.000000 climate_categories-0.8.3/docs/changelog.rst
--rwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)     5232 2023-05-10 09:47:08.000000 climate_categories-0.8.3/docs/conf.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       33 2023-04-26 09:04:13.000000 climate_categories-0.8.3/docs/contributing.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      337 2023-04-26 09:04:13.000000 climate_categories-0.8.3/docs/credits.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8179 2023-05-10 10:01:49.000000 climate_categories-0.8.3/docs/data.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      325 2023-04-26 09:04:13.000000 climate_categories-0.8.3/docs/index.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1209 2023-04-26 09:04:13.000000 climate_categories-0.8.3/docs/installation.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      780 2023-04-26 09:04:13.000000 climate_categories-0.8.3/docs/make.bat
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       27 2023-04-26 09:04:13.000000 climate_categories-0.8.3/docs/readme.rst
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       21 2023-05-10 09:48:15.000000 climate_categories-0.8.3/docs/requirements.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    18889 2023-05-15 16:28:37.000000 climate_categories-0.8.3/docs/usage.ipynb
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      328 2023-04-26 12:59:50.000000 climate_categories-0.8.3/pyproject.toml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        2 2023-04-26 09:04:13.000000 climate_categories-0.8.3/requirements.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        7 2023-04-26 09:04:13.000000 climate_categories-0.8.3/requirements_dev.txt
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1647 2023-05-23 14:46:12.291657 climate_categories-0.8.3/setup.cfg
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       61 2023-04-26 09:08:24.000000 climate_categories-0.8.3/setup.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1381 2023-05-23 14:15:26.000000 climate_categories-0.8.3/tbump.toml
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      379 2023-04-26 11:23:54.000000 climate_categories-0.8.3/tox.ini
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      773 2023-04-26 09:04:13.000000 climate_categories-0.8.3/update_changelog.py
--rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1181 2023-04-26 11:23:54.000000 climate_categories-0.8.3/update_citation_info.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-23 15:04:28.020310 climate_categories-0.8.4/
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-23 15:04:28.012310 climate_categories-0.8.4/.github/
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-23 15:04:28.012310 climate_categories-0.8.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      671 2023-04-26 09:04:13.000000 climate_categories-0.8.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      548 2023-04-26 09:04:13.000000 climate_categories-0.8.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      571 2023-04-26 09:04:13.000000 climate_categories-0.8.4/.github/ISSUE_TEMPLATE/new_categorization.md
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      369 2023-04-26 13:19:45.000000 climate_categories-0.8.4/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-23 15:04:28.012310 climate_categories-0.8.4/.github/workflows/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      963 2023-04-26 11:23:54.000000 climate_categories-0.8.4/.github/workflows/ci.yml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1331 2023-04-26 11:23:54.000000 climate_categories-0.8.4/.gitignore
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1253 2023-05-23 14:10:09.000000 climate_categories-0.8.4/.pre-commit-config.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      297 2023-04-26 13:26:25.000000 climate_categories-0.8.4/.readthedocs.yml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       38 2023-04-26 09:04:13.000000 climate_categories-0.8.4/.sourcery.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      216 2023-04-26 14:19:11.000000 climate_categories-0.8.4/AUTHORS.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5002 2023-05-23 15:02:58.000000 climate_categories-0.8.4/CHANGELOG.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5446 2023-04-26 11:23:54.000000 climate_categories-0.8.4/CONTRIBUTING.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      696 2023-04-26 14:19:11.000000 climate_categories-0.8.4/LICENSE
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3267 2023-05-15 16:33:50.000000 climate_categories-0.8.4/Makefile
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     9405 2023-05-23 15:04:28.020310 climate_categories-0.8.4/PKG-INFO
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3386 2023-05-23 15:03:36.000000 climate_categories-0.8.4/README.rst
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-23 15:04:28.012310 climate_categories-0.8.4/climate_categories/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1949 2023-05-23 15:02:46.000000 climate_categories-0.8.4/climate_categories/__init__.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    43152 2023-05-15 16:28:37.000000 climate_categories-0.8.4/climate_categories/_categories.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    47235 2023-04-26 12:57:44.000000 climate_categories-0.8.4/climate_categories/_conversions.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-23 15:04:28.016310 climate_categories-0.8.4/climate_categories/data/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    48820 2023-04-26 13:51:54.000000 climate_categories-0.8.4/climate_categories/data/BURDI.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    39603 2023-04-26 13:51:50.000000 climate_categories-0.8.4/climate_categories/data/BURDI.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    91320 2023-04-26 13:52:03.000000 climate_categories-0.8.4/climate_categories/data/BURDI_class.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    64321 2023-04-26 13:51:56.000000 climate_categories-0.8.4/climate_categories/data/BURDI_class.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    84030 2023-04-26 13:49:12.000000 climate_categories-0.8.4/climate_categories/data/CRF1999.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    69834 2023-04-26 13:49:07.000000 climate_categories-0.8.4/climate_categories/data/CRF1999.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   172563 2023-04-26 13:59:42.000000 climate_categories-0.8.4/climate_categories/data/CRF2013.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   136709 2023-04-26 13:59:42.000000 climate_categories-0.8.4/climate_categories/data/CRF2013.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   213803 2023-04-26 13:59:42.000000 climate_categories-0.8.4/climate_categories/data/CRF2013_2021.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   165299 2023-04-26 13:59:42.000000 climate_categories-0.8.4/climate_categories/data/CRF2013_2021.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   214940 2023-04-26 13:59:42.000000 climate_categories-0.8.4/climate_categories/data/CRF2013_2022.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   165976 2023-04-26 13:59:42.000000 climate_categories-0.8.4/climate_categories/data/CRF2013_2022.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   215236 2023-04-26 13:59:42.000000 climate_categories-0.8.4/climate_categories/data/CRF2013_2023.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   166217 2023-04-26 13:59:42.000000 climate_categories-0.8.4/climate_categories/data/CRF2013_2023.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    85443 2023-04-26 13:51:04.000000 climate_categories-0.8.4/climate_categories/data/CRFDI.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    68686 2023-04-26 13:50:55.000000 climate_categories-0.8.4/climate_categories/data/CRFDI.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   252079 2023-04-26 13:51:45.000000 climate_categories-0.8.4/climate_categories/data/CRFDI_class.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   172924 2023-04-26 13:51:08.000000 climate_categories-0.8.4/climate_categories/data/CRFDI_class.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2039 2023-04-26 13:48:45.000000 climate_categories-0.8.4/climate_categories/data/GCB.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1795 2023-04-26 09:04:13.000000 climate_categories-0.8.4/climate_categories/data/GCB.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    60150 2023-04-26 13:49:07.000000 climate_categories-0.8.4/climate_categories/data/IPCC1996.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    51928 2023-04-26 13:49:05.000000 climate_categories-0.8.4/climate_categories/data/IPCC1996.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   146256 2023-04-26 13:48:54.000000 climate_categories-0.8.4/climate_categories/data/IPCC2006.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   126862 2023-04-26 13:48:48.000000 climate_categories-0.8.4/climate_categories/data/IPCC2006.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   149225 2023-04-26 13:49:01.000000 climate_categories-0.8.4/climate_categories/data/IPCC2006_PRIMAP.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)   128959 2023-04-26 13:48:55.000000 climate_categories-0.8.4/climate_categories/data/IPCC2006_PRIMAP.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    24803 2023-04-26 13:59:42.000000 climate_categories-0.8.4/climate_categories/data/RCMIP.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    18549 2023-04-26 13:59:42.000000 climate_categories-0.8.4/climate_categories/data/RCMIP.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 09:04:13.000000 climate_categories-0.8.4/climate_categories/data/__init__.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3761 2023-04-26 09:06:11.000000 climate_categories-0.8.4/climate_categories/data/conversion.IPCC1996.IPCC2006.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    32498 2023-04-26 13:50:50.000000 climate_categories-0.8.4/climate_categories/data/gas.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    23635 2023-04-26 13:50:49.000000 climate_categories-0.8.4/climate_categories/data/gas.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-23 14:12:58.000000 climate_categories-0.8.4/climate_categories/py.typed
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      304 2023-04-26 11:23:54.000000 climate_categories-0.8.4/climate_categories/search.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-23 15:04:28.016310 climate_categories-0.8.4/climate_categories/tests/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       48 2023-04-26 09:04:13.000000 climate_categories-0.8.4/climate_categories/tests/__init__.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3795 2023-04-26 11:23:55.000000 climate_categories-0.8.4/climate_categories/tests/conftest.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-23 15:04:28.020310 climate_categories-0.8.4/climate_categories/tests/data/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        0 2023-04-26 10:17:34.000000 climate_categories-0.8.4/climate_categories/tests/data/__init__.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      359 2023-04-26 09:06:11.000000 climate_categories-0.8.4/climate_categories/tests/data/broken_conversion_not_allowed.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      359 2023-04-26 09:06:11.000000 climate_categories-0.8.4/climate_categories/tests/data/broken_conversion_not_existing.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1387 2023-04-26 09:04:13.000000 climate_categories-0.8.4/climate_categories/tests/data/broken_hierarchical_categorization.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      705 2023-04-26 09:04:13.000000 climate_categories-0.8.4/climate_categories/tests/data/broken_simple_categorization.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      350 2023-04-26 09:06:11.000000 climate_categories-0.8.4/climate_categories/tests/data/good_conversion.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      650 2023-04-26 09:04:13.000000 climate_categories-0.8.4/climate_categories/tests/data/good_conversion_A.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      341 2023-04-26 09:04:13.000000 climate_categories-0.8.4/climate_categories/tests/data/good_conversion_B.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      372 2023-04-26 09:04:13.000000 climate_categories-0.8.4/climate_categories/tests/data/good_conversion_aux1.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      349 2023-04-26 09:04:13.000000 climate_categories-0.8.4/climate_categories/tests/data/good_conversion_aux2.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      350 2023-04-26 09:06:11.000000 climate_categories-0.8.4/climate_categories/tests/data/good_conversion_reversed.csv
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1387 2023-04-26 09:04:13.000000 climate_categories-0.8.4/climate_categories/tests/data/hierarchical_categorization.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      702 2023-04-26 09:04:13.000000 climate_categories-0.8.4/climate_categories/tests/data/simple_categorization.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1665 2023-04-26 09:04:13.000000 climate_categories-0.8.4/climate_categories/tests/examples.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    21970 2023-05-15 16:28:37.000000 climate_categories-0.8.4/climate_categories/tests/test_climate_categories.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    14271 2023-04-26 11:23:55.000000 climate_categories-0.8.4/climate_categories/tests/test_conversions.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1205 2023-04-26 11:23:54.000000 climate_categories-0.8.4/climate_categories/tests/test_crf.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      769 2023-04-26 09:04:13.000000 climate_categories-0.8.4/climate_categories/tests/test_di.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      508 2023-04-26 09:04:13.000000 climate_categories-0.8.4/climate_categories/tests/test_gas.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1296 2023-04-26 09:04:13.000000 climate_categories-0.8.4/climate_categories/tests/test_ipcc.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     7703 2023-04-26 09:04:13.000000 climate_categories-0.8.4/climate_categories/tests/test_overcounting.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      596 2023-04-26 09:04:13.000000 climate_categories-0.8.4/climate_categories/tests/test_primap.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      305 2023-04-26 09:06:11.000000 climate_categories-0.8.4/climate_categories/tests/test_rcmip.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      649 2023-04-26 11:23:54.000000 climate_categories-0.8.4/climate_categories/tests/test_search.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-23 15:04:28.012310 climate_categories-0.8.4/climate_categories.egg-info/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     9405 2023-05-23 15:04:27.000000 climate_categories-0.8.4/climate_categories.egg-info/PKG-INFO
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     4029 2023-05-23 15:04:28.000000 climate_categories-0.8.4/climate_categories.egg-info/SOURCES.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        1 2023-05-23 15:04:27.000000 climate_categories-0.8.4/climate_categories.egg-info/dependency_links.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      307 2023-05-23 15:04:27.000000 climate_categories-0.8.4/climate_categories.egg-info/requires.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       19 2023-05-23 15:04:27.000000 climate_categories-0.8.4/climate_categories.egg-info/top_level.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      130 2023-04-26 09:04:13.000000 climate_categories-0.8.4/codecov.yml
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-23 15:04:28.020310 climate_categories-0.8.4/data_generation/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       62 2023-04-26 09:06:11.000000 climate_categories-0.8.4/data_generation/.gitignore
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5819 2023-04-26 13:44:45.000000 climate_categories-0.8.4/data_generation/BURDI.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3177 2023-04-26 13:44:45.000000 climate_categories-0.8.4/data_generation/BURDI_class.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    17598 2023-04-26 13:44:45.000000 climate_categories-0.8.4/data_generation/CRF1999.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    65761 2023-04-26 13:44:45.000000 climate_categories-0.8.4/data_generation/CRF2013.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    30906 2023-04-26 13:44:45.000000 climate_categories-0.8.4/data_generation/CRF2013_2021.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    31721 2023-04-26 13:44:45.000000 climate_categories-0.8.4/data_generation/CRF2013_2022.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    32225 2023-04-26 13:44:45.000000 climate_categories-0.8.4/data_generation/CRF2013_2023.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5318 2023-04-26 13:44:45.000000 climate_categories-0.8.4/data_generation/CRFDI.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5232 2023-04-26 13:44:45.000000 climate_categories-0.8.4/data_generation/CRFDI_class.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    11562 2023-04-26 13:44:45.000000 climate_categories-0.8.4/data_generation/IPCC1996.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8947 2023-04-26 13:44:45.000000 climate_categories-0.8.4/data_generation/IPCC2006.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     4254 2023-04-26 13:44:45.000000 climate_categories-0.8.4/data_generation/IPCC2006_PRIMAP.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8134 2023-04-26 13:44:45.000000 climate_categories-0.8.4/data_generation/RCMIP.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      272 2023-04-26 13:44:45.000000 climate_categories-0.8.4/data_generation/convert_yaml_to_python.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3318 2023-04-26 13:44:45.000000 climate_categories-0.8.4/data_generation/gas.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1082 2023-04-26 13:44:45.000000 climate_categories-0.8.4/data_generation/utils.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-05-23 15:04:28.020310 climate_categories-0.8.4/docs/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      631 2023-04-26 09:04:13.000000 climate_categories-0.8.4/docs/Makefile
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      241 2023-04-26 09:04:13.000000 climate_categories-0.8.4/docs/api.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       30 2023-04-26 09:04:13.000000 climate_categories-0.8.4/docs/changelog.rst
+-rwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)     5232 2023-05-10 09:47:08.000000 climate_categories-0.8.4/docs/conf.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       33 2023-04-26 09:04:13.000000 climate_categories-0.8.4/docs/contributing.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      337 2023-04-26 09:04:13.000000 climate_categories-0.8.4/docs/credits.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     8179 2023-05-10 10:01:49.000000 climate_categories-0.8.4/docs/data.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      325 2023-04-26 09:04:13.000000 climate_categories-0.8.4/docs/index.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1209 2023-04-26 09:04:13.000000 climate_categories-0.8.4/docs/installation.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      780 2023-04-26 09:04:13.000000 climate_categories-0.8.4/docs/make.bat
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       27 2023-04-26 09:04:13.000000 climate_categories-0.8.4/docs/readme.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       21 2023-05-10 09:48:15.000000 climate_categories-0.8.4/docs/requirements.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    18889 2023-05-15 16:28:37.000000 climate_categories-0.8.4/docs/usage.ipynb
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      328 2023-04-26 12:59:50.000000 climate_categories-0.8.4/pyproject.toml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        2 2023-04-26 09:04:13.000000 climate_categories-0.8.4/requirements.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        7 2023-04-26 09:04:13.000000 climate_categories-0.8.4/requirements_dev.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1658 2023-05-23 15:04:28.020310 climate_categories-0.8.4/setup.cfg
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       61 2023-04-26 09:08:24.000000 climate_categories-0.8.4/setup.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1381 2023-05-23 15:02:46.000000 climate_categories-0.8.4/tbump.toml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      379 2023-04-26 11:23:54.000000 climate_categories-0.8.4/tox.ini
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      773 2023-04-26 09:04:13.000000 climate_categories-0.8.4/update_changelog.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1181 2023-04-26 11:23:54.000000 climate_categories-0.8.4/update_citation_info.py
```

### Comparing `climate_categories-0.8.3/.github/ISSUE_TEMPLATE/bug_report.md` & `climate_categories-0.8.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/.github/ISSUE_TEMPLATE/feature_request.md` & `climate_categories-0.8.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/.github/ISSUE_TEMPLATE/new_categorization.md` & `climate_categories-0.8.4/.github/ISSUE_TEMPLATE/new_categorization.md`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/.github/workflows/ci.yml` & `climate_categories-0.8.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/.gitignore` & `climate_categories-0.8.4/.gitignore`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/.pre-commit-config.yaml` & `climate_categories-0.8.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/CHANGELOG.rst` & `climate_categories-0.8.4/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+0.8.4 (2023-05-23)
+------------------
+* Re-release to make sure py.typed is included in built package.
+
+
 0.8.3 (2023-05-23)
 ------------------
 * add py.typed file to announce this library is using type hints.
 
 0.8.2 (2023-05-15)
 ------------------
 * Remove pygments-csv-lexer dependency for docs building.
```

### Comparing `climate_categories-0.8.3/CONTRIBUTING.rst` & `climate_categories-0.8.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/LICENSE` & `climate_categories-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/Makefile` & `climate_categories-0.8.4/Makefile`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/PKG-INFO` & `climate_categories-0.8.4/climate_categories.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: climate_categories
-Version: 0.8.3
+Name: climate-categories
+Version: 0.8.4
 Summary: Commonly used codes, categories, terminologies, and nomenclatures used in climate policy analysis as a Python package.
 Home-page: https://github.com/pik-primap/climate_categories
 Author: Mika Pflüger
 Author-email: mika.pflueger@climate-resource.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://climate-categories.readthedocs.io/
 Classifier: Development Status :: 4 - Beta
@@ -96,21 +96,26 @@
 permissions and limitations under the License.
 
 Citation
 --------
 If you use this library and want to cite it, please cite it as:
 
 Mika Pflüger, Annika Günther, Johannes Gütschow, and Robert Gieseke. (2023-05-23).
-pik-primap/climate_categories: climate_categories Version 0.8.3.
-Zenodo. https://doi.org/10.5281/zenodo.7962902
+pik-primap/climate_categories: climate_categories Version 0.8.4.
+Zenodo. https://doi.org/10.5281/zenodo.7963059
 
 =========
 Changelog
 =========
 
+0.8.4 (2023-05-23)
+------------------
+* Re-release to make sure py.typed is included in built package.
+
+
 0.8.3 (2023-05-23)
 ------------------
 * add py.typed file to announce this library is using type hints.
 
 0.8.2 (2023-05-15)
 ------------------
 * Remove pygments-csv-lexer dependency for docs building.
```

### Comparing `climate_categories-0.8.3/README.rst` & `climate_categories-0.8.4/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -72,9 +72,9 @@
 permissions and limitations under the License.
 
 Citation
 --------
 If you use this library and want to cite it, please cite it as:
 
 Mika Pflüger, Annika Günther, Johannes Gütschow, and Robert Gieseke. (2023-05-23).
-pik-primap/climate_categories: climate_categories Version 0.8.3.
-Zenodo. https://doi.org/10.5281/zenodo.7962902
+pik-primap/climate_categories: climate_categories Version 0.8.4.
+Zenodo. https://doi.org/10.5281/zenodo.7963059
```

### Comparing `climate_categories-0.8.3/climate_categories/__init__.py` & `climate_categories-0.8.4/climate_categories/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Access to all categorizations is provided directly at the module level, using the
 names of categorizations. To access the example categorization `Excat`, simply use
 `climate_categories.Excat` .
 """
 
 __author__ = """Mika Pflüger"""
 __email__ = "mika.pflueger@climate-resource.com"
-__version__ = "0.8.3"
+__version__ = "0.8.4"
 
 import importlib
 import importlib.resources
 
 from . import (
     search,
 )
```

### Comparing `climate_categories-0.8.3/climate_categories/_categories.py` & `climate_categories-0.8.4/climate_categories/_categories.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/_conversions.py` & `climate_categories-0.8.4/climate_categories/_conversions.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/data/BURDI.py` & `climate_categories-0.8.4/climate_categories/data/BURDI.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/data/BURDI.yaml` & `climate_categories-0.8.4/climate_categories/data/BURDI.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/data/BURDI_class.py` & `climate_categories-0.8.4/climate_categories/data/BURDI_class.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/data/BURDI_class.yaml` & `climate_categories-0.8.4/climate_categories/data/BURDI_class.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/data/CRF1999.py` & `climate_categories-0.8.4/climate_categories/data/CRF1999.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/data/CRF1999.yaml` & `climate_categories-0.8.4/climate_categories/data/CRF1999.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/data/CRF2013.py` & `climate_categories-0.8.4/climate_categories/data/CRF2013.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/data/CRF2013.yaml` & `climate_categories-0.8.4/climate_categories/data/CRF2013.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/data/CRF2013_2021.py` & `climate_categories-0.8.4/climate_categories/data/CRF2013_2021.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/data/CRF2013_2021.yaml` & `climate_categories-0.8.4/climate_categories/data/CRF2013_2021.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/data/CRF2013_2022.py` & `climate_categories-0.8.4/climate_categories/data/CRF2013_2022.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/data/CRF2013_2022.yaml` & `climate_categories-0.8.4/climate_categories/data/CRF2013_2022.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/data/CRF2013_2023.py` & `climate_categories-0.8.4/climate_categories/data/CRF2013_2023.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/data/CRF2013_2023.yaml` & `climate_categories-0.8.4/climate_categories/data/CRF2013_2023.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/data/CRFDI.py` & `climate_categories-0.8.4/climate_categories/data/CRFDI.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/data/CRFDI.yaml` & `climate_categories-0.8.4/climate_categories/data/CRFDI.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/data/CRFDI_class.py` & `climate_categories-0.8.4/climate_categories/data/CRFDI_class.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/data/CRFDI_class.yaml` & `climate_categories-0.8.4/climate_categories/data/CRFDI_class.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/data/GCB.py` & `climate_categories-0.8.4/climate_categories/data/GCB.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/data/GCB.yaml` & `climate_categories-0.8.4/climate_categories/data/GCB.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/data/IPCC1996.py` & `climate_categories-0.8.4/climate_categories/data/IPCC1996.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/data/IPCC1996.yaml` & `climate_categories-0.8.4/climate_categories/data/IPCC1996.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/data/IPCC2006.py` & `climate_categories-0.8.4/climate_categories/data/IPCC2006.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/data/IPCC2006.yaml` & `climate_categories-0.8.4/climate_categories/data/IPCC2006.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/data/IPCC2006_PRIMAP.py` & `climate_categories-0.8.4/climate_categories/data/IPCC2006_PRIMAP.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/data/IPCC2006_PRIMAP.yaml` & `climate_categories-0.8.4/climate_categories/data/IPCC2006_PRIMAP.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/data/RCMIP.py` & `climate_categories-0.8.4/climate_categories/data/RCMIP.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/data/RCMIP.yaml` & `climate_categories-0.8.4/climate_categories/data/RCMIP.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/data/conversion.IPCC1996.IPCC2006.csv` & `climate_categories-0.8.4/climate_categories/data/conversion.IPCC1996.IPCC2006.csv`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/data/gas.py` & `climate_categories-0.8.4/climate_categories/data/gas.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/data/gas.yaml` & `climate_categories-0.8.4/climate_categories/data/gas.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/tests/conftest.py` & `climate_categories-0.8.4/climate_categories/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/tests/data/broken_hierarchical_categorization.yaml` & `climate_categories-0.8.4/climate_categories/tests/data/broken_hierarchical_categorization.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/tests/data/broken_simple_categorization.yaml` & `climate_categories-0.8.4/climate_categories/tests/data/broken_simple_categorization.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/tests/data/good_conversion_A.yaml` & `climate_categories-0.8.4/climate_categories/tests/data/good_conversion_A.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/tests/data/hierarchical_categorization.yaml` & `climate_categories-0.8.4/climate_categories/tests/data/hierarchical_categorization.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/tests/data/simple_categorization.yaml` & `climate_categories-0.8.4/climate_categories/tests/data/simple_categorization.yaml`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/tests/examples.py` & `climate_categories-0.8.4/climate_categories/tests/examples.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/tests/test_climate_categories.py` & `climate_categories-0.8.4/climate_categories/tests/test_climate_categories.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/tests/test_conversions.py` & `climate_categories-0.8.4/climate_categories/tests/test_conversions.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/tests/test_crf.py` & `climate_categories-0.8.4/climate_categories/tests/test_crf.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/tests/test_di.py` & `climate_categories-0.8.4/climate_categories/tests/test_di.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/tests/test_ipcc.py` & `climate_categories-0.8.4/climate_categories/tests/test_ipcc.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/tests/test_overcounting.py` & `climate_categories-0.8.4/climate_categories/tests/test_overcounting.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/tests/test_primap.py` & `climate_categories-0.8.4/climate_categories/tests/test_primap.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories/tests/test_search.py` & `climate_categories-0.8.4/climate_categories/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/climate_categories.egg-info/PKG-INFO` & `climate_categories-0.8.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: climate-categories
-Version: 0.8.3
+Name: climate_categories
+Version: 0.8.4
 Summary: Commonly used codes, categories, terminologies, and nomenclatures used in climate policy analysis as a Python package.
 Home-page: https://github.com/pik-primap/climate_categories
 Author: Mika Pflüger
 Author-email: mika.pflueger@climate-resource.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://climate-categories.readthedocs.io/
 Classifier: Development Status :: 4 - Beta
@@ -96,21 +96,26 @@
 permissions and limitations under the License.
 
 Citation
 --------
 If you use this library and want to cite it, please cite it as:
 
 Mika Pflüger, Annika Günther, Johannes Gütschow, and Robert Gieseke. (2023-05-23).
-pik-primap/climate_categories: climate_categories Version 0.8.3.
-Zenodo. https://doi.org/10.5281/zenodo.7962902
+pik-primap/climate_categories: climate_categories Version 0.8.4.
+Zenodo. https://doi.org/10.5281/zenodo.7963059
 
 =========
 Changelog
 =========
 
+0.8.4 (2023-05-23)
+------------------
+* Re-release to make sure py.typed is included in built package.
+
+
 0.8.3 (2023-05-23)
 ------------------
 * add py.typed file to announce this library is using type hints.
 
 0.8.2 (2023-05-15)
 ------------------
 * Remove pygments-csv-lexer dependency for docs building.
```

### Comparing `climate_categories-0.8.3/climate_categories.egg-info/SOURCES.txt` & `climate_categories-0.8.4/climate_categories.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/data_generation/BURDI.py` & `climate_categories-0.8.4/data_generation/BURDI.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/data_generation/BURDI_class.py` & `climate_categories-0.8.4/data_generation/BURDI_class.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/data_generation/CRF1999.py` & `climate_categories-0.8.4/data_generation/CRF1999.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/data_generation/CRF2013.py` & `climate_categories-0.8.4/data_generation/CRF2013.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/data_generation/CRF2013_2021.py` & `climate_categories-0.8.4/data_generation/CRF2013_2021.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/data_generation/CRF2013_2022.py` & `climate_categories-0.8.4/data_generation/CRF2013_2022.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/data_generation/CRF2013_2023.py` & `climate_categories-0.8.4/data_generation/CRF2013_2023.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/data_generation/CRFDI.py` & `climate_categories-0.8.4/data_generation/CRFDI.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/data_generation/CRFDI_class.py` & `climate_categories-0.8.4/data_generation/CRFDI_class.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/data_generation/IPCC1996.py` & `climate_categories-0.8.4/data_generation/IPCC1996.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/data_generation/IPCC2006.py` & `climate_categories-0.8.4/data_generation/IPCC2006.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/data_generation/IPCC2006_PRIMAP.py` & `climate_categories-0.8.4/data_generation/IPCC2006_PRIMAP.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/data_generation/RCMIP.py` & `climate_categories-0.8.4/data_generation/RCMIP.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/data_generation/gas.py` & `climate_categories-0.8.4/data_generation/gas.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/data_generation/utils.py` & `climate_categories-0.8.4/data_generation/utils.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/docs/Makefile` & `climate_categories-0.8.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/docs/conf.py` & `climate_categories-0.8.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/docs/data.rst` & `climate_categories-0.8.4/docs/data.rst`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/docs/installation.rst` & `climate_categories-0.8.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/docs/make.bat` & `climate_categories-0.8.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/docs/usage.ipynb` & `climate_categories-0.8.4/docs/usage.ipynb`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/setup.cfg` & `climate_categories-0.8.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = climate_categories
-version = 0.8.3
+version = 0.8.4
 author = Mika Pflüger
 author_email = mika.pflueger@climate-resource.com
 description = Commonly used codes, categories, terminologies, and nomenclatures used in climate policy analysis as a Python package.
 long_description = file: README.rst, CHANGELOG.rst
 long_description_content_type = text/x-rst
 url = https://github.com/pik-primap/climate_categories
 project_urls = 
@@ -16,15 +16,15 @@
 	License :: OSI Approved :: Apache Software License
 	Natural Language :: English
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 license = Apache Software License 2.0
-license_file = LICENSE
+license_files = LICENSE
 
 [options]
 packages = 
 	climate_categories
 	climate_categories.data
 	climate_categories.tests
 	climate_categories.tests.data
@@ -68,14 +68,15 @@
 	openscm-units
 	black
 
 [options.package_data]
 * = 
 	*.yaml
 	*.csv
+	py.typed
 
 [doc8]
 max-line-length = 88
 ignore-path-errors = docs/data.rst;D001
 
 [egg_info]
 tag_build =
```

### Comparing `climate_categories-0.8.3/tbump.toml` & `climate_categories-0.8.4/tbump.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Uncomment this if your project is hosted on GitHub:
 github_url = "https://github.com/pik-primap/climate_categories/"
 
 [version]
-current = "0.8.3"
+current = "0.8.4"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
```

### Comparing `climate_categories-0.8.3/update_changelog.py` & `climate_categories-0.8.4/update_changelog.py`

 * *Files identical despite different names*

### Comparing `climate_categories-0.8.3/update_citation_info.py` & `climate_categories-0.8.4/update_citation_info.py`

 * *Files identical despite different names*

