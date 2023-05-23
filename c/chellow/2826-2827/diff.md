# Comparing `tmp/chellow-2826.tar.gz` & `tmp/chellow-2827.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chellow-2826.tar", last modified: Fri Jan 27 13:23:43 2023, max compression
+gzip compressed data, was "chellow-2827.tar", last modified: Wed Feb  1 16:30:13 2023, max compression
```

## Comparing `chellow-2826.tar` & `chellow-2827.tar`

### file list

```diff
@@ -1,389 +1,389 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 13:23:43.635947 chellow-2826/
--rw-r--r--   0 root         (0) root         (0)       78 2023-01-27 13:23:42.000000 chellow-2826/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    10650 2023-01-27 13:23:43.635947 chellow-2826/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10362 2023-01-27 13:23:42.000000 chellow-2826/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 13:23:43.571946 chellow-2826/bin/
--rwxr-xr-x   0 root         (0) root         (0)      814 2023-01-27 13:23:42.000000 chellow-2826/bin/chellow_service_monitor.sh
--rwxr-xr-x   0 root         (0) root         (0)      160 2023-01-27 13:23:42.000000 chellow-2826/bin/chellow_start.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 13:23:43.635947 chellow-2826/chellow/
--rw-r--r--   0 root         (0) root         (0)    10020 2023-01-27 13:23:42.000000 chellow-2826/chellow/__init__.py
--rw-r--r--   0 root         (0) root         (0)      496 2023-01-27 13:23:43.635947 chellow-2826/chellow/_version.py
--rw-r--r--   0 root         (0) root         (0)    11036 2023-01-27 13:23:42.000000 chellow-2826/chellow/api.py
--rw-r--r--   0 root         (0) root         (0)     5713 2023-01-27 13:23:42.000000 chellow-2826/chellow/bank_holidays.py
--rw-r--r--   0 root         (0) root         (0)     1302 2023-01-27 13:23:42.000000 chellow-2826/chellow/commands.py
--rw-r--r--   0 root         (0) root         (0)     3941 2023-01-27 13:23:42.000000 chellow-2826/chellow/dloads.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 13:23:43.583946 chellow-2826/chellow/e/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/__init__.py
--rw-r--r--   0 root         (0) root         (0)      706 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/aahedc.py
--rw-r--r--   0 root         (0) root         (0)     7071 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/bill_importer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 13:23:43.583946 chellow-2826/chellow/e/bill_parsers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/bill_parsers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4234 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/bill_parsers/activity_mop_stark_xlsx.py
--rw-r--r--   0 root         (0) root         (0)     4382 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/bill_parsers/annual_mop_stark_xlsx.py
--rw-r--r--   0 root         (0) root         (0)     4828 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/bill_parsers/bgb_edi.py
--rw-r--r--   0 root         (0) root         (0)     5133 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/bill_parsers/csv.py
--rw-r--r--   0 root         (0) root         (0)    12912 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/bill_parsers/engie_edi.py
--rw-r--r--   0 root         (0) root         (0)    14010 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/bill_parsers/engie_xls.py
--rw-r--r--   0 root         (0) root         (0)     7382 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/bill_parsers/gdf_csv.py
--rw-r--r--   0 root         (0) root         (0)    13607 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/bill_parsers/haven_csv.py
--rw-r--r--   0 root         (0) root         (0)    16188 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/bill_parsers/haven_edi.py
--rw-r--r--   0 root         (0) root         (0)    10472 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/bill_parsers/haven_edi_tprs.py
--rw-r--r--   0 root         (0) root         (0)     1929 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/bill_parsers/mm.py
--rw-r--r--   0 root         (0) root         (0)     4581 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/bill_parsers/nonsettlement_dc_stark_xlsx.py
--rw-r--r--   0 root         (0) root         (0)     6007 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/bill_parsers/settlement_dc_stark_xlsx.py
--rw-r--r--   0 root         (0) root         (0)    15287 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/bill_parsers/sse_edi.py
--rw-r--r--   0 root         (0) root         (0)     7533 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/bill_parsers/sww_xls.py
--rw-r--r--   0 root         (0) root         (0)     7041 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/bmarketidx.py
--rw-r--r--   0 root         (0) root         (0)    10905 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/bsuos.py
--rw-r--r--   0 root         (0) root         (0)      664 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/ccl.py
--rw-r--r--   0 root         (0) root         (0)    66344 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/computer.py
--rw-r--r--   0 root         (0) root         (0)    20205 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/dno_rate_parser.py
--rw-r--r--   0 root         (0) root         (0)    29091 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/duos.py
--rw-r--r--   0 root         (0) root         (0)    11491 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/energy_management.py
--rw-r--r--   0 root         (0) root         (0)    16466 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/hh_importer.py
--rw-r--r--   0 root         (0) root         (0)     2423 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/hh_parser_bg_csv.py
--rw-r--r--   0 root         (0) root         (0)     3558 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/hh_parser_df2.py
--rw-r--r--   0 root         (0) root         (0)     2082 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/hh_parser_simple_csv.py
--rw-r--r--   0 root         (0) root         (0)     5350 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/laf_import.py
--rw-r--r--   0 root         (0) root         (0)    32047 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/mdd_importer.py
--rw-r--r--   0 root         (0) root         (0)     6182 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/rcrc.py
--rw-r--r--   0 root         (0) root         (0)      696 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/ro.py
--rw-r--r--   0 root         (0) root         (0)    23242 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/scenario.py
--rw-r--r--   0 root         (0) root         (0)     8145 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/system_price.py
--rw-r--r--   0 root         (0) root         (0)     9550 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/tlms.py
--rw-r--r--   0 root         (0) root         (0)    12586 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/tnuos.py
--rw-r--r--   0 root         (0) root         (0)   174283 2023-01-27 13:23:42.000000 chellow-2826/chellow/e/views.py
--rw-r--r--   0 root         (0) root         (0)    51859 2023-01-27 13:23:42.000000 chellow-2826/chellow/edi_lib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 13:23:43.587946 chellow-2826/chellow/gas/
--rw-r--r--   0 root         (0) root         (0)     6627 2023-01-27 13:23:42.000000 chellow-2826/chellow/gas/bill_import.py
--rw-r--r--   0 root         (0) root         (0)     5558 2023-01-27 13:23:42.000000 chellow-2826/chellow/gas/bill_parser_csv.py
--rw-r--r--   0 root         (0) root         (0)     8703 2023-01-27 13:23:42.000000 chellow-2826/chellow/gas/bill_parser_engie_edi.py
--rw-r--r--   0 root         (0) root         (0)      347 2023-01-27 13:23:42.000000 chellow-2826/chellow/gas/ccl.py
--rw-r--r--   0 root         (0) root         (0)     6949 2023-01-27 13:23:42.000000 chellow-2826/chellow/gas/cv.py
--rw-r--r--   0 root         (0) root         (0)    11340 2023-01-27 13:23:42.000000 chellow-2826/chellow/gas/dn_rate_parser.py
--rw-r--r--   0 root         (0) root         (0)    24429 2023-01-27 13:23:42.000000 chellow-2826/chellow/gas/engine.py
--rw-r--r--   0 root         (0) root         (0)     5525 2023-01-27 13:23:42.000000 chellow-2826/chellow/gas/transportation.py
--rw-r--r--   0 root         (0) root         (0)    54376 2023-01-27 13:23:42.000000 chellow-2826/chellow/gas/views.py
--rw-r--r--   0 root         (0) root         (0)    58470 2023-01-27 13:23:42.000000 chellow-2826/chellow/general_import.py
--rw-r--r--   0 root         (0) root         (0)   233514 2023-01-27 13:23:42.000000 chellow-2826/chellow/models.py
--rw-r--r--   0 root         (0) root         (0)     1388 2023-01-27 13:23:42.000000 chellow-2826/chellow/proxy.py
--rw-r--r--   0 root         (0) root         (0)     3846 2023-01-27 13:23:42.000000 chellow-2826/chellow/rate_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 13:23:43.595946 chellow-2826/chellow/reports/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-27 13:23:42.000000 chellow-2826/chellow/reports/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10182 2023-01-27 13:23:42.000000 chellow-2826/chellow/reports/report_109.py
--rw-r--r--   0 root         (0) root         (0)    27604 2023-01-27 13:23:42.000000 chellow-2826/chellow/reports/report_111.py
--rw-r--r--   0 root         (0) root         (0)      305 2023-01-27 13:23:42.000000 chellow-2826/chellow/reports/report_155.py
--rw-r--r--   0 root         (0) root         (0)     7087 2023-01-27 13:23:42.000000 chellow-2826/chellow/reports/report_169.py
--rw-r--r--   0 root         (0) root         (0)    11500 2023-01-27 13:23:42.000000 chellow-2826/chellow/reports/report_177.py
--rw-r--r--   0 root         (0) root         (0)     5027 2023-01-27 13:23:42.000000 chellow-2826/chellow/reports/report_181.py
--rw-r--r--   0 root         (0) root         (0)     8222 2023-01-27 13:23:42.000000 chellow-2826/chellow/reports/report_183.py
--rw-r--r--   0 root         (0) root         (0)     9547 2023-01-27 13:23:42.000000 chellow-2826/chellow/reports/report_187.py
--rw-r--r--   0 root         (0) root         (0)     6127 2023-01-27 13:23:42.000000 chellow-2826/chellow/reports/report_215.py
--rw-r--r--   0 root         (0) root         (0)     6186 2023-01-27 13:23:42.000000 chellow-2826/chellow/reports/report_219.py
--rw-r--r--   0 root         (0) root         (0)     3968 2023-01-27 13:23:42.000000 chellow-2826/chellow/reports/report_231.py
--rw-r--r--   0 root         (0) root         (0)     4130 2023-01-27 13:23:42.000000 chellow-2826/chellow/reports/report_233.py
--rw-r--r--   0 root         (0) root         (0)     5325 2023-01-27 13:23:42.000000 chellow-2826/chellow/reports/report_241.py
--rw-r--r--   0 root         (0) root         (0)    40220 2023-01-27 13:23:42.000000 chellow-2826/chellow/reports/report_247.py
--rw-r--r--   0 root         (0) root         (0)     2096 2023-01-27 13:23:42.000000 chellow-2826/chellow/reports/report_29.py
--rw-r--r--   0 root         (0) root         (0)     7113 2023-01-27 13:23:42.000000 chellow-2826/chellow/reports/report_291.py
--rw-r--r--   0 root         (0) root         (0)    16826 2023-01-27 13:23:42.000000 chellow-2826/chellow/reports/report_33.py
--rw-r--r--   0 root         (0) root         (0)     5406 2023-01-27 13:23:42.000000 chellow-2826/chellow/reports/report_387.py
--rw-r--r--   0 root         (0) root         (0)     7075 2023-01-27 13:23:42.000000 chellow-2826/chellow/reports/report_41.py
--rw-r--r--   0 root         (0) root         (0)    11538 2023-01-27 13:23:42.000000 chellow-2826/chellow/reports/report_429.py
--rw-r--r--   0 root         (0) root         (0)    39409 2023-01-27 13:23:42.000000 chellow-2826/chellow/reports/report_59.py
--rw-r--r--   0 root         (0) root         (0)     4200 2023-01-27 13:23:42.000000 chellow-2826/chellow/reports/report_81.py
--rw-r--r--   0 root         (0) root         (0)     5768 2023-01-27 13:23:42.000000 chellow-2826/chellow/reports/report_87.py
--rw-r--r--   0 root         (0) root         (0)     6112 2023-01-27 13:23:42.000000 chellow-2826/chellow/reports/report_asset_comparison.py
--rw-r--r--   0 root         (0) root         (0)     4573 2023-01-27 13:23:42.000000 chellow-2826/chellow/reports/report_batches.py
--rw-r--r--   0 root         (0) root         (0)     1852 2023-01-27 13:23:42.000000 chellow-2826/chellow/reports/report_csv_llfcs.py
--rw-r--r--   0 root         (0) root         (0)     4067 2023-01-27 13:23:42.000000 chellow-2826/chellow/reports/report_csv_site_hh_data.py
--rw-r--r--   0 root         (0) root         (0)     2591 2023-01-27 13:23:42.000000 chellow-2826/chellow/reports/report_csv_site_snags.py
--rw-r--r--   0 root         (0) root         (0)    20986 2023-01-27 13:23:42.000000 chellow-2826/chellow/reports/report_ecoes_comparison.py
--rw-r--r--   0 root         (0) root         (0)    12218 2023-01-27 13:23:42.000000 chellow-2826/chellow/reports/report_g_monthly_duration.py
--rw-r--r--   0 root         (0) root         (0)     3772 2023-01-27 13:23:42.000000 chellow-2826/chellow/reports/report_g_supplies_snapshot.py
--rw-r--r--   0 root         (0) root         (0)     3618 2023-01-27 13:23:42.000000 chellow-2826/chellow/reports/report_g_supply_virtual_bill.py
--rw-r--r--   0 root         (0) root         (0)     4250 2023-01-27 13:23:42.000000 chellow-2826/chellow/reports/report_g_virtual_bills.py
--rw-r--r--   0 root         (0) root         (0)     3306 2023-01-27 13:23:42.000000 chellow-2826/chellow/reports/report_g_virtual_bills_hh.py
--rw-r--r--   0 root         (0) root         (0)     4883 2023-01-27 13:23:42.000000 chellow-2826/chellow/reports/report_laf_parser.py
--rw-r--r--   0 root         (0) root         (0)     3837 2023-01-27 13:23:42.000000 chellow-2826/chellow/reports/report_supply_contacts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 13:23:43.571946 chellow-2826/chellow/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 13:23:43.595946 chellow-2826/chellow/static/css/
--rw-r--r--   0 root         (0) root         (0)     5355 2023-01-27 13:23:42.000000 chellow-2826/chellow/static/css/chellow.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 13:23:43.595946 chellow-2826/chellow/static/images/
--rw-r--r--   0 root         (0) root         (0)     2339 2023-01-27 13:23:42.000000 chellow-2826/chellow/static/images/favicon.svg
--rw-r--r--   0 root         (0) root         (0)     2346 2023-01-27 13:23:42.000000 chellow-2826/chellow/static/images/favicon_test.svg
--rw-r--r--   0 root         (0) root         (0)     1569 2023-01-27 13:23:42.000000 chellow-2826/chellow/static/images/logo.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 13:23:43.595946 chellow-2826/chellow/static/js/
--rw-r--r--   0 root         (0) root         (0)    39958 2023-01-27 13:23:42.000000 chellow-2826/chellow/static/js/htmx.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 13:23:43.607946 chellow-2826/chellow/templates/
--rw-r--r--   0 root         (0) root         (0)      344 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/403.html
--rw-r--r--   0 root         (0) root         (0)    11983 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/base.html
--rw-r--r--   0 root         (0) root         (0)      402 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/bill_type.html
--rw-r--r--   0 root         (0) root         (0)      471 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/bill_types.html
--rw-r--r--   0 root         (0) root         (0)      775 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/chain.html
--rw-r--r--   0 root         (0) root         (0)      486 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/csv_sites_monthly_duration.html
--rw-r--r--   0 root         (0) root         (0)      994 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/downloads.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 13:23:43.627947 chellow-2826/chellow/templates/e/
--rw-r--r--   0 root         (0) root         (0)      678 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/asset_comparison.html
--rw-r--r--   0 root         (0) root         (0)     2056 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/channel.html
--rw-r--r--   0 root         (0) root         (0)     1479 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/channel_add.html
--rw-r--r--   0 root         (0) root         (0)     2198 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/channel_edit.html
--rw-r--r--   0 root         (0) root         (0)     1477 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/channel_snag.html
--rw-r--r--   0 root         (0) root         (0)     1911 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/channel_snag_edit.html
--rw-r--r--   0 root         (0) root         (0)     2899 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/channel_snags.html
--rw-r--r--   0 root         (0) root         (0)      384 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/comm.html
--rw-r--r--   0 root         (0) root         (0)      434 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/comms.html
--rw-r--r--   0 root         (0) root         (0)      376 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/cop.html
--rw-r--r--   0 root         (0) root         (0)      425 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/cops.html
--rw-r--r--   0 root         (0) root         (0)      437 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/csv_bills.html
--rw-r--r--   0 root         (0) root         (0)      763 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/csv_register_reads.html
--rw-r--r--   0 root         (0) root         (0)      930 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/csv_sites_hh_data.html
--rw-r--r--   0 root         (0) root         (0)      433 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/csv_sites_triad.html
--rw-r--r--   0 root         (0) root         (0)     1613 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/csv_supplies_hh_data.html
--rw-r--r--   0 root         (0) root         (0)      727 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/csv_supplies_snapshot.html
--rw-r--r--   0 root         (0) root         (0)      422 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/csv_supplies_triad.html
--rw-r--r--   0 root         (0) root         (0)     1165 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/dc_auto_importer.html
--rw-r--r--   0 root         (0) root         (0)     4795 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/dc_batch.html
--rw-r--r--   0 root         (0) root         (0)     1113 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/dc_batch_add.html
--rw-r--r--   0 root         (0) root         (0)     1962 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/dc_batch_edit.html
--rw-r--r--   0 root         (0) root         (0)     1157 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/dc_batch_file.html
--rw-r--r--   0 root         (0) root         (0)     1876 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/dc_batch_file_edit.html
--rw-r--r--   0 root         (0) root         (0)     1556 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/dc_batch_upload_file.html
--rw-r--r--   0 root         (0) root         (0)     1007 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/dc_batches.html
--rw-r--r--   0 root         (0) root         (0)     2028 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/dc_bill.html
--rw-r--r--   0 root         (0) root         (0)     1648 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/dc_bill_add.html
--rw-r--r--   0 root         (0) root         (0)     2707 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/dc_bill_edit.html
--rw-r--r--   0 root         (0) root         (0)     2188 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/dc_bill_import.html
--rw-r--r--   0 root         (0) root         (0)     2135 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/dc_bill_imports.html
--rw-r--r--   0 root         (0) root         (0)     2322 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/dc_contract.html
--rw-r--r--   0 root         (0) root         (0)     2963 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/dc_contract_edit.html
--rw-r--r--   0 root         (0) root         (0)      848 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/dc_contract_hh_import.html
--rw-r--r--   0 root         (0) root         (0)     8172 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/dc_contract_hh_imports.html
--rw-r--r--   0 root         (0) root         (0)      773 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/dc_contracts.html
--rw-r--r--   0 root         (0) root         (0)      711 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/dc_contracts_add.html
--rw-r--r--   0 root         (0) root         (0)     1219 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/dc_rate_script.html
--rw-r--r--   0 root         (0) root         (0)      644 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/dc_rate_script_add.html
--rw-r--r--   0 root         (0) root         (0)     1955 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/dc_rate_script_edit.html
--rw-r--r--   0 root         (0) root         (0)     2515 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/dno.html
--rw-r--r--   0 root         (0) root         (0)      753 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/dno_rate_script.html
--rw-r--r--   0 root         (0) root         (0)      559 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/dno_rate_script_add.html
--rw-r--r--   0 root         (0) root         (0)     1275 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/dno_rate_script_edit.html
--rw-r--r--   0 root         (0) root         (0)      702 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/dnos.html
--rw-r--r--   0 root         (0) root         (0)      440 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/dtc_meter_type.html
--rw-r--r--   0 root         (0) root         (0)      467 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/dtc_meter_types.html
--rw-r--r--   0 root         (0) root         (0)     1493 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/duration_report.html
--rw-r--r--   0 root         (0) root         (0)     2033 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/em_hh_data.html
--rw-r--r--   0 root         (0) root         (0)     6647 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/em_months.html
--rw-r--r--   0 root         (0) root         (0)     2890 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/em_site.html
--rw-r--r--   0 root         (0) root         (0)      678 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/em_totals.html
--rw-r--r--   0 root         (0) root         (0)      478 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/energisation_status.html
--rw-r--r--   0 root         (0) root         (0)      587 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/energisation_statuses.html
--rw-r--r--   0 root         (0) root         (0)     6396 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/era_edit.html
--rw-r--r--   0 root         (0) root         (0)     2128 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/era_supplier_bill_add.html
--rw-r--r--   0 root         (0) root         (0)      439 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/generator_type.html
--rw-r--r--   0 root         (0) root         (0)      535 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/generator_types.html
--rw-r--r--   0 root         (0) root         (0)      405 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/gsp_group.html
--rw-r--r--   0 root         (0) root         (0)      453 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/gsp_groups.html
--rw-r--r--   0 root         (0) root         (0)     1824 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/hh_datum_edit.html
--rw-r--r--   0 root         (0) root         (0)      996 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/lafs.html
--rw-r--r--   0 root         (0) root         (0)     1168 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/llfc.html
--rw-r--r--   0 root         (0) root         (0)     1038 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/llfc_edit.html
--rw-r--r--   0 root         (0) root         (0)     1143 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/llfcs.html
--rw-r--r--   0 root         (0) root         (0)     1025 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/market_role.html
--rw-r--r--   0 root         (0) root         (0)      464 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/market_roles.html
--rw-r--r--   0 root         (0) root         (0)      659 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/meter_payment_type.html
--rw-r--r--   0 root         (0) root         (0)      770 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/meter_payment_types.html
--rw-r--r--   0 root         (0) root         (0)      642 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/meter_type.html
--rw-r--r--   0 root         (0) root         (0)      661 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/meter_types.html
--rw-r--r--   0 root         (0) root         (0)     4821 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/mop_batch.html
--rw-r--r--   0 root         (0) root         (0)     1104 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/mop_batch_add.html
--rw-r--r--   0 root         (0) root         (0)     2089 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/mop_batch_edit.html
--rw-r--r--   0 root         (0) root         (0)     1167 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/mop_batch_file.html
--rw-r--r--   0 root         (0) root         (0)     1899 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/mop_batch_file_edit.html
--rw-r--r--   0 root         (0) root         (0)     1584 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/mop_batch_upload_file.html
--rw-r--r--   0 root         (0) root         (0)     1015 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/mop_batches.html
--rw-r--r--   0 root         (0) root         (0)     2105 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/mop_bill.html
--rw-r--r--   0 root         (0) root         (0)     1712 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/mop_bill_add.html
--rw-r--r--   0 root         (0) root         (0)     2748 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/mop_bill_edit.html
--rw-r--r--   0 root         (0) root         (0)     3201 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/mop_bill_import.html
--rw-r--r--   0 root         (0) root         (0)     1610 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/mop_bill_imports.html
--rw-r--r--   0 root         (0) root         (0)     1748 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/mop_contract.html
--rw-r--r--   0 root         (0) root         (0)      738 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/mop_contract_add.html
--rw-r--r--   0 root         (0) root         (0)     2204 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/mop_contract_edit.html
--rw-r--r--   0 root         (0) root         (0)      768 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/mop_contracts.html
--rw-r--r--   0 root         (0) root         (0)     1170 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/mop_rate_script.html
--rw-r--r--   0 root         (0) root         (0)      643 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/mop_rate_script_add.html
--rw-r--r--   0 root         (0) root         (0)     1817 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/mop_rate_script_edit.html
--rw-r--r--   0 root         (0) root         (0)     2014 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/mtc.html
--rw-r--r--   0 root         (0) root         (0)     1004 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/mtc_llfc.html
--rw-r--r--   0 root         (0) root         (0)     1400 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/mtc_llfc_ssc.html
--rw-r--r--   0 root         (0) root         (0)     1516 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/mtc_llfc_ssc_pc.html
--rw-r--r--   0 root         (0) root         (0)     1504 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/mtc_llfc_ssc_pcs.html
--rw-r--r--   0 root         (0) root         (0)     1596 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/mtc_llfc_sscs.html
--rw-r--r--   0 root         (0) root         (0)     1296 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/mtc_llfcs.html
--rw-r--r--   0 root         (0) root         (0)     2232 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/mtc_participant.html
--rw-r--r--   0 root         (0) root         (0)     1500 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/mtc_participants.html
--rw-r--r--   0 root         (0) root         (0)      985 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/mtc_ssc.html
--rw-r--r--   0 root         (0) root         (0)     1276 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/mtc_sscs.html
--rw-r--r--   0 root         (0) root         (0)      853 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/mtcs.html
--rw-r--r--   0 root         (0) root         (0)     1367 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/ods_monthly_duration.html
--rw-r--r--   0 root         (0) root         (0)     1022 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/participant.html
--rw-r--r--   0 root         (0) root         (0)      500 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/participants.html
--rw-r--r--   0 root         (0) root         (0)      666 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/parties.html
--rw-r--r--   0 root         (0) root         (0)     1915 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/party.html
--rw-r--r--   0 root         (0) root         (0)      521 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/pc.html
--rw-r--r--   0 root         (0) root         (0)      560 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/pcs.html
--rw-r--r--   0 root         (0) root         (0)     2289 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/read_add.html
--rw-r--r--   0 root         (0) root         (0)     3147 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/read_edit.html
--rw-r--r--   0 root         (0) root         (0)      403 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/read_type.html
--rw-r--r--   0 root         (0) root         (0)      473 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/read_types.html
--rw-r--r--   0 root         (0) root         (0)     1153 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/scenario.html
--rw-r--r--   0 root         (0) root         (0)      516 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/scenario_add.html
--rw-r--r--   0 root         (0) root         (0)     5162 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/scenario_docs.html
--rw-r--r--   0 root         (0) root         (0)     1070 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/scenario_edit.html
--rw-r--r--   0 root         (0) root         (0)      847 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/scenarios.html
--rw-r--r--   0 root         (0) root         (0)     1413 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/site_hh_data.html
--rw-r--r--   0 root         (0) root         (0)      847 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/site_site_snags.html
--rw-r--r--   0 root         (0) root         (0)      924 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/site_snag.html
--rw-r--r--   0 root         (0) root         (0)     1436 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/site_snag_edit.html
--rw-r--r--   0 root         (0) root         (0)     1175 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/site_snags.html
--rw-r--r--   0 root         (0) root         (0)      427 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/site_snags_edit.html
--rw-r--r--   0 root         (0) root         (0)      373 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/source.html
--rw-r--r--   0 root         (0) root         (0)      453 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/sources.html
--rw-r--r--   0 root         (0) root         (0)      811 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/ssc.html
--rw-r--r--   0 root         (0) root         (0)      918 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/sscs.html
--rw-r--r--   0 root         (0) root         (0)     5647 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/supplier_batch.html
--rw-r--r--   0 root         (0) root         (0)     1240 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/supplier_batch_add.html
--rw-r--r--   0 root         (0) root         (0)     1420 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/supplier_batch_edit.html
--rw-r--r--   0 root         (0) root         (0)     1226 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/supplier_batch_file.html
--rw-r--r--   0 root         (0) root         (0)     7618 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/supplier_batch_file_add.html
--rw-r--r--   0 root         (0) root         (0)     2009 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/supplier_batch_file_edit.html
--rw-r--r--   0 root         (0) root         (0)     8533 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/supplier_batch_upload_file.html
--rw-r--r--   0 root         (0) root         (0)     1164 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/supplier_batches.html
--rw-r--r--   0 root         (0) root         (0)     3797 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/supplier_bill.html
--rw-r--r--   0 root         (0) root         (0)     2184 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/supplier_bill_add.html
--rw-r--r--   0 root         (0) root         (0)     2732 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/supplier_bill_edit.html
--rw-r--r--   0 root         (0) root         (0)     4291 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/supplier_bill_import.html
--rw-r--r--   0 root         (0) root         (0)     9356 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/supplier_bill_imports.html
--rw-r--r--   0 root         (0) root         (0)     2863 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/supplier_contract.html
--rw-r--r--   0 root         (0) root         (0)      899 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/supplier_contract_add.html
--rw-r--r--   0 root         (0) root         (0)     1463 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/supplier_contract_edit.html
--rw-r--r--   0 root         (0) root         (0)     1508 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/supplier_contracts.html
--rw-r--r--   0 root         (0) root         (0)     1245 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/supplier_rate_script.html
--rw-r--r--   0 root         (0) root         (0)      690 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/supplier_rate_script_add.html
--rw-r--r--   0 root         (0) root         (0)     1968 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/supplier_rate_script_edit.html
--rw-r--r--   0 root         (0) root         (0)    28697 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/supply.html
--rw-r--r--   0 root         (0) root         (0)     2723 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/supply_edit.html
--rw-r--r--   0 root         (0) root         (0)     3587 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/supply_hh_data.html
--rw-r--r--   0 root         (0) root         (0)     1927 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/supply_months.html
--rw-r--r--   0 root         (0) root         (0)      553 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/supply_note_add.html
--rw-r--r--   0 root         (0) root         (0)      954 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/supply_note_edit.html
--rw-r--r--   0 root         (0) root         (0)      863 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/supply_notes.html
--rw-r--r--   0 root         (0) root         (0)      180 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/supply_post.html
--rw-r--r--   0 root         (0) root         (0)     1239 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/supply_virtual_bill.html
--rw-r--r--   0 root         (0) root         (0)     1452 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/tpr.html
--rw-r--r--   0 root         (0) root         (0)      258 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/e/tprs.html
--rw-r--r--   0 root         (0) root         (0)     1437 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/edi_viewer.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 13:23:43.631947 chellow-2826/chellow/templates/g/
--rw-r--r--   0 root         (0) root         (0)     3487 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/batch.html
--rw-r--r--   0 root         (0) root         (0)     1035 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/batch_add.html
--rw-r--r--   0 root         (0) root         (0)     2132 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/batch_edit.html
--rw-r--r--   0 root         (0) root         (0)      730 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/batches.html
--rw-r--r--   0 root         (0) root         (0)     3455 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/bill.html
--rw-r--r--   0 root         (0) root         (0)     1674 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/bill_add.html
--rw-r--r--   0 root         (0) root         (0)     2754 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/bill_edit.html
--rw-r--r--   0 root         (0) root         (0)     4292 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/bill_import.html
--rw-r--r--   0 root         (0) root         (0)     2795 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/bill_imports.html
--rw-r--r--   0 root         (0) root         (0)      481 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/dn.html
--rw-r--r--   0 root         (0) root         (0)      403 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/dns.html
--rw-r--r--   0 root         (0) root         (0)     4024 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/era_edit.html
--rw-r--r--   0 root         (0) root         (0)      584 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/exit_zone.html
--rw-r--r--   0 root         (0) root         (0)     1011 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/industry_auto_importer.html
--rw-r--r--   0 root         (0) root         (0)     1451 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/industry_contract.html
--rw-r--r--   0 root         (0) root         (0)      667 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/industry_contract_add.html
--rw-r--r--   0 root         (0) root         (0)     1377 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/industry_contract_edit.html
--rw-r--r--   0 root         (0) root         (0)      710 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/industry_contracts.html
--rw-r--r--   0 root         (0) root         (0)     1283 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/industry_rate_script.html
--rw-r--r--   0 root         (0) root         (0)      638 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/industry_rate_script_add.html
--rw-r--r--   0 root         (0) root         (0)     2401 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/industry_rate_script_edit.html
--rw-r--r--   0 root         (0) root         (0)      560 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/ldz.html
--rw-r--r--   0 root         (0) root         (0)     2220 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/read_add.html
--rw-r--r--   0 root         (0) root         (0)     3181 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/read_edit.html
--rw-r--r--   0 root         (0) root         (0)      409 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/read_type.html
--rw-r--r--   0 root         (0) root         (0)      481 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/read_types.html
--rw-r--r--   0 root         (0) root         (0)      577 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/reading_frequencies.html
--rw-r--r--   0 root         (0) root         (0)      472 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/reading_frequency.html
--rw-r--r--   0 root         (0) root         (0)      655 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/reports.html
--rw-r--r--   0 root         (0) root         (0)     1795 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/supplier_contract.html
--rw-r--r--   0 root         (0) root         (0)      656 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/supplier_contract_add.html
--rw-r--r--   0 root         (0) root         (0)     1399 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/supplier_contract_edit.html
--rw-r--r--   0 root         (0) root         (0)      710 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/supplier_contracts.html
--rw-r--r--   0 root         (0) root         (0)     1283 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/supplier_rate_script.html
--rw-r--r--   0 root         (0) root         (0)      620 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/supplier_rate_script_add.html
--rw-r--r--   0 root         (0) root         (0)     1950 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/supplier_rate_script_edit.html
--rw-r--r--   0 root         (0) root         (0)     1267 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/supplies.html
--rw-r--r--   0 root         (0) root         (0)    10885 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/supply.html
--rw-r--r--   0 root         (0) root         (0)     2022 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/supply_edit.html
--rw-r--r--   0 root         (0) root         (0)      744 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/supply_note_add.html
--rw-r--r--   0 root         (0) root         (0)     1043 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/supply_note_edit.html
--rw-r--r--   0 root         (0) root         (0)      936 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/supply_notes.html
--rw-r--r--   0 root         (0) root         (0)      438 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/unit.html
--rw-r--r--   0 root         (0) root         (0)      441 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/g/units.html
--rw-r--r--   0 root         (0) root         (0)     1013 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/general_import.html
--rw-r--r--   0 root         (0) root         (0)    12208 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/general_imports.html
--rw-r--r--   0 root         (0) root         (0)     5437 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/home.html
--rw-r--r--   0 root         (0) root         (0)     1332 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/local_report.html
--rw-r--r--   0 root         (0) root         (0)      701 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/local_reports.html
--rw-r--r--   0 root         (0) root         (0)      944 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/non_core_auto_importer.html
--rw-r--r--   0 root         (0) root         (0)     1173 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/non_core_contract.html
--rw-r--r--   0 root         (0) root         (0)     3005 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/non_core_contract_edit.html
--rw-r--r--   0 root         (0) root         (0)      661 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/non_core_contracts.html
--rw-r--r--   0 root         (0) root         (0)     1283 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/non_core_rate_script.html
--rw-r--r--   0 root         (0) root         (0)      690 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/non_core_rate_script_add.html
--rw-r--r--   0 root         (0) root         (0)     1868 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/non_core_rate_script_edit.html
--rw-r--r--   0 root         (0) root         (0)      244 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/object_summary.html
--rw-r--r--   0 root         (0) root         (0)     1002 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/rate_server.html
--rw-r--r--   0 root         (0) root         (0)     4040 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/report_run.html
--rw-r--r--   0 root         (0) root         (0)     2305 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/report_run_asset_comparison.html
--rw-r--r--   0 root         (0) root         (0)     6330 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/report_run_bill_check.html
--rw-r--r--   0 root         (0) root         (0)     4086 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/report_run_ecoes_comparison.html
--rw-r--r--   0 root         (0) root         (0)     3791 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/report_run_row.html
--rw-r--r--   0 root         (0) root         (0)     4683 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/report_run_row_bill_check.html
--rw-r--r--   0 root         (0) root         (0)     2117 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/report_run_supply_contacts.html
--rw-r--r--   0 root         (0) root         (0)      667 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/report_runs.html
--rw-r--r--   0 root         (0) root         (0)    10016 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/site.html
--rw-r--r--   0 root         (0) root         (0)      422 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/site_add.html
--rw-r--r--   0 root         (0) root         (0)     7803 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/site_edit.html
--rw-r--r--   0 root         (0) root         (0)     3468 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/site_gen_graph.html
--rw-r--r--   0 root         (0) root         (0)     1766 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/site_hh_data.html
--rw-r--r--   0 root         (0) root         (0)     6562 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/site_months.html
--rw-r--r--   0 root         (0) root         (0)     3094 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/site_used_graph.html
--rw-r--r--   0 root         (0) root         (0)      621 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/sites.html
--rw-r--r--   0 root         (0) root         (0)     3530 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/supplies.html
--rw-r--r--   0 root         (0) root         (0)     2048 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/system.html
--rw-r--r--   0 root         (0) root         (0)      623 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/tester.html
--rw-r--r--   0 root         (0) root         (0)     3255 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/user.html
--rw-r--r--   0 root         (0) root         (0)      399 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/user_roles.html
--rw-r--r--   0 root         (0) root         (0)     2244 2023-01-27 13:23:42.000000 chellow-2826/chellow/templates/users.html
--rw-r--r--   0 root         (0) root         (0)     3915 2023-01-27 13:23:42.000000 chellow-2826/chellow/testing.py
--rw-r--r--   0 root         (0) root         (0)    18984 2023-01-27 13:23:42.000000 chellow-2826/chellow/utils.py
--rw-r--r--   0 root         (0) root         (0)    80371 2023-01-27 13:23:42.000000 chellow-2826/chellow/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 13:23:43.579946 chellow-2826/chellow.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10650 2023-01-27 13:23:43.000000 chellow-2826/chellow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13096 2023-01-27 13:23:43.000000 chellow-2826/chellow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-27 13:23:43.000000 chellow-2826/chellow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      119 2023-01-27 13:23:43.000000 chellow-2826/chellow.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      265 2023-01-27 13:23:43.000000 chellow-2826/chellow.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-01-27 13:23:43.000000 chellow-2826/chellow.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 13:23:43.631947 chellow-2826/config/
--rw-r--r--   0 root         (0) root         (0)      434 2023-01-27 13:23:42.000000 chellow-2826/config/chellow.conf
--rw-r--r--   0 root         (0) root         (0)      777 2023-01-27 13:23:43.635947 chellow-2826/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1952 2023-01-27 13:23:42.000000 chellow-2826/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 13:23:43.635947 chellow-2826/test/
--rw-r--r--   0 root         (0) root         (0)      635 2023-01-27 13:23:42.000000 chellow-2826/test/test_chellow.py
--rw-r--r--   0 root         (0) root         (0)    12897 2023-01-27 13:23:42.000000 chellow-2826/test/test_general_import.py
--rw-r--r--   0 root         (0) root         (0)    25018 2023-01-27 13:23:42.000000 chellow-2826/test/test_models.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-01-27 13:23:42.000000 chellow-2826/test/test_testing.py
--rw-r--r--   0 root         (0) root         (0)     2668 2023-01-27 13:23:42.000000 chellow-2826/test/test_utils.py
--rw-r--r--   0 root         (0) root         (0)    39838 2023-01-27 13:23:42.000000 chellow-2826/test/test_views.py
--rw-r--r--   0 root         (0) root         (0)    70668 2023-01-27 13:23:42.000000 chellow-2826/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 16:30:13.171385 chellow-2827/
+-rw-r--r--   0 root         (0) root         (0)       78 2023-02-01 16:30:10.000000 chellow-2827/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    10650 2023-02-01 16:30:13.171385 chellow-2827/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10362 2023-02-01 16:30:10.000000 chellow-2827/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 16:30:13.119385 chellow-2827/bin/
+-rwxr-xr-x   0 root         (0) root         (0)      814 2023-02-01 16:30:10.000000 chellow-2827/bin/chellow_service_monitor.sh
+-rwxr-xr-x   0 root         (0) root         (0)      160 2023-02-01 16:30:10.000000 chellow-2827/bin/chellow_start.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 16:30:13.175385 chellow-2827/chellow/
+-rw-r--r--   0 root         (0) root         (0)    10020 2023-02-01 16:30:10.000000 chellow-2827/chellow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      496 2023-02-01 16:30:13.175385 chellow-2827/chellow/_version.py
+-rw-r--r--   0 root         (0) root         (0)    11036 2023-02-01 16:30:10.000000 chellow-2827/chellow/api.py
+-rw-r--r--   0 root         (0) root         (0)     5713 2023-02-01 16:30:10.000000 chellow-2827/chellow/bank_holidays.py
+-rw-r--r--   0 root         (0) root         (0)     1302 2023-02-01 16:30:10.000000 chellow-2827/chellow/commands.py
+-rw-r--r--   0 root         (0) root         (0)     3941 2023-02-01 16:30:10.000000 chellow-2827/chellow/dloads.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 16:30:13.127385 chellow-2827/chellow/e/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/aahedc.py
+-rw-r--r--   0 root         (0) root         (0)     7069 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/bill_importer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 16:30:13.127385 chellow-2827/chellow/e/bill_parsers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/bill_parsers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4234 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/bill_parsers/activity_mop_stark_xlsx.py
+-rw-r--r--   0 root         (0) root         (0)     4382 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/bill_parsers/annual_mop_stark_xlsx.py
+-rw-r--r--   0 root         (0) root         (0)     4828 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/bill_parsers/bgb_edi.py
+-rw-r--r--   0 root         (0) root         (0)     5132 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/bill_parsers/csv.py
+-rw-r--r--   0 root         (0) root         (0)    12911 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/bill_parsers/engie_edi.py
+-rw-r--r--   0 root         (0) root         (0)    14009 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/bill_parsers/engie_xls.py
+-rw-r--r--   0 root         (0) root         (0)     7382 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/bill_parsers/gdf_csv.py
+-rw-r--r--   0 root         (0) root         (0)    13606 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/bill_parsers/haven_csv.py
+-rw-r--r--   0 root         (0) root         (0)    16188 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/bill_parsers/haven_edi.py
+-rw-r--r--   0 root         (0) root         (0)    10470 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/bill_parsers/haven_edi_tprs.py
+-rw-r--r--   0 root         (0) root         (0)     1929 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/bill_parsers/mm.py
+-rw-r--r--   0 root         (0) root         (0)     4576 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/bill_parsers/nonsettlement_dc_stark_xlsx.py
+-rw-r--r--   0 root         (0) root         (0)     6007 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/bill_parsers/settlement_dc_stark_xlsx.py
+-rw-r--r--   0 root         (0) root         (0)    15285 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/bill_parsers/sse_edi.py
+-rw-r--r--   0 root         (0) root         (0)     7533 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/bill_parsers/sww_xls.py
+-rw-r--r--   0 root         (0) root         (0)     7041 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/bmarketidx.py
+-rw-r--r--   0 root         (0) root         (0)    10905 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/bsuos.py
+-rw-r--r--   0 root         (0) root         (0)      664 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/ccl.py
+-rw-r--r--   0 root         (0) root         (0)    66337 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/computer.py
+-rw-r--r--   0 root         (0) root         (0)    20203 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/dno_rate_parser.py
+-rw-r--r--   0 root         (0) root         (0)    29089 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/duos.py
+-rw-r--r--   0 root         (0) root         (0)    11490 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/energy_management.py
+-rw-r--r--   0 root         (0) root         (0)    16466 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/hh_importer.py
+-rw-r--r--   0 root         (0) root         (0)     2423 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/hh_parser_bg_csv.py
+-rw-r--r--   0 root         (0) root         (0)     3558 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/hh_parser_df2.py
+-rw-r--r--   0 root         (0) root         (0)     2082 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/hh_parser_simple_csv.py
+-rw-r--r--   0 root         (0) root         (0)     5349 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/laf_import.py
+-rw-r--r--   0 root         (0) root         (0)    32042 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/mdd_importer.py
+-rw-r--r--   0 root         (0) root         (0)     6182 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/rcrc.py
+-rw-r--r--   0 root         (0) root         (0)      696 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/ro.py
+-rw-r--r--   0 root         (0) root         (0)    23239 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/scenario.py
+-rw-r--r--   0 root         (0) root         (0)     8145 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/system_price.py
+-rw-r--r--   0 root         (0) root         (0)     9549 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/tlms.py
+-rw-r--r--   0 root         (0) root         (0)    13863 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/tnuos.py
+-rw-r--r--   0 root         (0) root         (0)   174281 2023-02-01 16:30:10.000000 chellow-2827/chellow/e/views.py
+-rw-r--r--   0 root         (0) root         (0)    51859 2023-02-01 16:30:10.000000 chellow-2827/chellow/edi_lib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 16:30:13.131385 chellow-2827/chellow/gas/
+-rw-r--r--   0 root         (0) root         (0)     6627 2023-02-01 16:30:10.000000 chellow-2827/chellow/gas/bill_import.py
+-rw-r--r--   0 root         (0) root         (0)     5557 2023-02-01 16:30:10.000000 chellow-2827/chellow/gas/bill_parser_csv.py
+-rw-r--r--   0 root         (0) root         (0)     8702 2023-02-01 16:30:10.000000 chellow-2827/chellow/gas/bill_parser_engie_edi.py
+-rw-r--r--   0 root         (0) root         (0)      347 2023-02-01 16:30:10.000000 chellow-2827/chellow/gas/ccl.py
+-rw-r--r--   0 root         (0) root         (0)     6949 2023-02-01 16:30:10.000000 chellow-2827/chellow/gas/cv.py
+-rw-r--r--   0 root         (0) root         (0)    11338 2023-02-01 16:30:10.000000 chellow-2827/chellow/gas/dn_rate_parser.py
+-rw-r--r--   0 root         (0) root         (0)    24426 2023-02-01 16:30:10.000000 chellow-2827/chellow/gas/engine.py
+-rw-r--r--   0 root         (0) root         (0)     5525 2023-02-01 16:30:10.000000 chellow-2827/chellow/gas/transportation.py
+-rw-r--r--   0 root         (0) root         (0)    54376 2023-02-01 16:30:10.000000 chellow-2827/chellow/gas/views.py
+-rw-r--r--   0 root         (0) root         (0)    58470 2023-02-01 16:30:10.000000 chellow-2827/chellow/general_import.py
+-rw-r--r--   0 root         (0) root         (0)   233497 2023-02-01 16:30:10.000000 chellow-2827/chellow/models.py
+-rw-r--r--   0 root         (0) root         (0)     1387 2023-02-01 16:30:10.000000 chellow-2827/chellow/proxy.py
+-rw-r--r--   0 root         (0) root         (0)     3844 2023-02-01 16:30:10.000000 chellow-2827/chellow/rate_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 16:30:13.135385 chellow-2827/chellow/reports/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-01 16:30:10.000000 chellow-2827/chellow/reports/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10182 2023-02-01 16:30:10.000000 chellow-2827/chellow/reports/report_109.py
+-rw-r--r--   0 root         (0) root         (0)    27601 2023-02-01 16:30:10.000000 chellow-2827/chellow/reports/report_111.py
+-rw-r--r--   0 root         (0) root         (0)      305 2023-02-01 16:30:10.000000 chellow-2827/chellow/reports/report_155.py
+-rw-r--r--   0 root         (0) root         (0)     7087 2023-02-01 16:30:10.000000 chellow-2827/chellow/reports/report_169.py
+-rw-r--r--   0 root         (0) root         (0)    11499 2023-02-01 16:30:10.000000 chellow-2827/chellow/reports/report_177.py
+-rw-r--r--   0 root         (0) root         (0)     5027 2023-02-01 16:30:10.000000 chellow-2827/chellow/reports/report_181.py
+-rw-r--r--   0 root         (0) root         (0)     8222 2023-02-01 16:30:10.000000 chellow-2827/chellow/reports/report_183.py
+-rw-r--r--   0 root         (0) root         (0)     9547 2023-02-01 16:30:10.000000 chellow-2827/chellow/reports/report_187.py
+-rw-r--r--   0 root         (0) root         (0)     6127 2023-02-01 16:30:10.000000 chellow-2827/chellow/reports/report_215.py
+-rw-r--r--   0 root         (0) root         (0)     6184 2023-02-01 16:30:10.000000 chellow-2827/chellow/reports/report_219.py
+-rw-r--r--   0 root         (0) root         (0)     3968 2023-02-01 16:30:10.000000 chellow-2827/chellow/reports/report_231.py
+-rw-r--r--   0 root         (0) root         (0)     4129 2023-02-01 16:30:10.000000 chellow-2827/chellow/reports/report_233.py
+-rw-r--r--   0 root         (0) root         (0)     5324 2023-02-01 16:30:10.000000 chellow-2827/chellow/reports/report_241.py
+-rw-r--r--   0 root         (0) root         (0)    40219 2023-02-01 16:30:10.000000 chellow-2827/chellow/reports/report_247.py
+-rw-r--r--   0 root         (0) root         (0)     2096 2023-02-01 16:30:10.000000 chellow-2827/chellow/reports/report_29.py
+-rw-r--r--   0 root         (0) root         (0)     7112 2023-02-01 16:30:10.000000 chellow-2827/chellow/reports/report_291.py
+-rw-r--r--   0 root         (0) root         (0)    16826 2023-02-01 16:30:10.000000 chellow-2827/chellow/reports/report_33.py
+-rw-r--r--   0 root         (0) root         (0)     5405 2023-02-01 16:30:10.000000 chellow-2827/chellow/reports/report_387.py
+-rw-r--r--   0 root         (0) root         (0)     7075 2023-02-01 16:30:10.000000 chellow-2827/chellow/reports/report_41.py
+-rw-r--r--   0 root         (0) root         (0)    11537 2023-02-01 16:30:10.000000 chellow-2827/chellow/reports/report_429.py
+-rw-r--r--   0 root         (0) root         (0)    39406 2023-02-01 16:30:10.000000 chellow-2827/chellow/reports/report_59.py
+-rw-r--r--   0 root         (0) root         (0)     4199 2023-02-01 16:30:10.000000 chellow-2827/chellow/reports/report_81.py
+-rw-r--r--   0 root         (0) root         (0)     5768 2023-02-01 16:30:10.000000 chellow-2827/chellow/reports/report_87.py
+-rw-r--r--   0 root         (0) root         (0)     6111 2023-02-01 16:30:10.000000 chellow-2827/chellow/reports/report_asset_comparison.py
+-rw-r--r--   0 root         (0) root         (0)     4571 2023-02-01 16:30:10.000000 chellow-2827/chellow/reports/report_batches.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2023-02-01 16:30:10.000000 chellow-2827/chellow/reports/report_csv_llfcs.py
+-rw-r--r--   0 root         (0) root         (0)     4067 2023-02-01 16:30:10.000000 chellow-2827/chellow/reports/report_csv_site_hh_data.py
+-rw-r--r--   0 root         (0) root         (0)     2591 2023-02-01 16:30:10.000000 chellow-2827/chellow/reports/report_csv_site_snags.py
+-rw-r--r--   0 root         (0) root         (0)    20986 2023-02-01 16:30:10.000000 chellow-2827/chellow/reports/report_ecoes_comparison.py
+-rw-r--r--   0 root         (0) root         (0)    12217 2023-02-01 16:30:10.000000 chellow-2827/chellow/reports/report_g_monthly_duration.py
+-rw-r--r--   0 root         (0) root         (0)     3772 2023-02-01 16:30:10.000000 chellow-2827/chellow/reports/report_g_supplies_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     3617 2023-02-01 16:30:10.000000 chellow-2827/chellow/reports/report_g_supply_virtual_bill.py
+-rw-r--r--   0 root         (0) root         (0)     4249 2023-02-01 16:30:10.000000 chellow-2827/chellow/reports/report_g_virtual_bills.py
+-rw-r--r--   0 root         (0) root         (0)     3306 2023-02-01 16:30:10.000000 chellow-2827/chellow/reports/report_g_virtual_bills_hh.py
+-rw-r--r--   0 root         (0) root         (0)     4882 2023-02-01 16:30:10.000000 chellow-2827/chellow/reports/report_laf_parser.py
+-rw-r--r--   0 root         (0) root         (0)     3836 2023-02-01 16:30:10.000000 chellow-2827/chellow/reports/report_supply_contacts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 16:30:13.115385 chellow-2827/chellow/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 16:30:13.135385 chellow-2827/chellow/static/css/
+-rw-r--r--   0 root         (0) root         (0)     5355 2023-02-01 16:30:10.000000 chellow-2827/chellow/static/css/chellow.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 16:30:13.135385 chellow-2827/chellow/static/images/
+-rw-r--r--   0 root         (0) root         (0)     2339 2023-02-01 16:30:10.000000 chellow-2827/chellow/static/images/favicon.svg
+-rw-r--r--   0 root         (0) root         (0)     2346 2023-02-01 16:30:10.000000 chellow-2827/chellow/static/images/favicon_test.svg
+-rw-r--r--   0 root         (0) root         (0)     1569 2023-02-01 16:30:10.000000 chellow-2827/chellow/static/images/logo.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 16:30:13.135385 chellow-2827/chellow/static/js/
+-rw-r--r--   0 root         (0) root         (0)    39958 2023-02-01 16:30:10.000000 chellow-2827/chellow/static/js/htmx.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 16:30:13.143385 chellow-2827/chellow/templates/
+-rw-r--r--   0 root         (0) root         (0)      344 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/403.html
+-rw-r--r--   0 root         (0) root         (0)    11983 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/base.html
+-rw-r--r--   0 root         (0) root         (0)      402 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/bill_type.html
+-rw-r--r--   0 root         (0) root         (0)      471 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/bill_types.html
+-rw-r--r--   0 root         (0) root         (0)      775 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/chain.html
+-rw-r--r--   0 root         (0) root         (0)      486 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/csv_sites_monthly_duration.html
+-rw-r--r--   0 root         (0) root         (0)      994 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/downloads.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 16:30:13.163385 chellow-2827/chellow/templates/e/
+-rw-r--r--   0 root         (0) root         (0)      678 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/asset_comparison.html
+-rw-r--r--   0 root         (0) root         (0)     2056 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/channel.html
+-rw-r--r--   0 root         (0) root         (0)     1479 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/channel_add.html
+-rw-r--r--   0 root         (0) root         (0)     2198 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/channel_edit.html
+-rw-r--r--   0 root         (0) root         (0)     1477 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/channel_snag.html
+-rw-r--r--   0 root         (0) root         (0)     1911 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/channel_snag_edit.html
+-rw-r--r--   0 root         (0) root         (0)     2899 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/channel_snags.html
+-rw-r--r--   0 root         (0) root         (0)      384 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/comm.html
+-rw-r--r--   0 root         (0) root         (0)      434 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/comms.html
+-rw-r--r--   0 root         (0) root         (0)      376 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/cop.html
+-rw-r--r--   0 root         (0) root         (0)      425 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/cops.html
+-rw-r--r--   0 root         (0) root         (0)      437 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/csv_bills.html
+-rw-r--r--   0 root         (0) root         (0)      763 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/csv_register_reads.html
+-rw-r--r--   0 root         (0) root         (0)      930 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/csv_sites_hh_data.html
+-rw-r--r--   0 root         (0) root         (0)      433 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/csv_sites_triad.html
+-rw-r--r--   0 root         (0) root         (0)     1613 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/csv_supplies_hh_data.html
+-rw-r--r--   0 root         (0) root         (0)      727 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/csv_supplies_snapshot.html
+-rw-r--r--   0 root         (0) root         (0)      422 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/csv_supplies_triad.html
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/dc_auto_importer.html
+-rw-r--r--   0 root         (0) root         (0)     4795 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/dc_batch.html
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/dc_batch_add.html
+-rw-r--r--   0 root         (0) root         (0)     1962 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/dc_batch_edit.html
+-rw-r--r--   0 root         (0) root         (0)     1157 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/dc_batch_file.html
+-rw-r--r--   0 root         (0) root         (0)     1876 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/dc_batch_file_edit.html
+-rw-r--r--   0 root         (0) root         (0)     1556 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/dc_batch_upload_file.html
+-rw-r--r--   0 root         (0) root         (0)     1007 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/dc_batches.html
+-rw-r--r--   0 root         (0) root         (0)     2028 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/dc_bill.html
+-rw-r--r--   0 root         (0) root         (0)     1648 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/dc_bill_add.html
+-rw-r--r--   0 root         (0) root         (0)     2707 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/dc_bill_edit.html
+-rw-r--r--   0 root         (0) root         (0)     2188 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/dc_bill_import.html
+-rw-r--r--   0 root         (0) root         (0)     2135 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/dc_bill_imports.html
+-rw-r--r--   0 root         (0) root         (0)     2322 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/dc_contract.html
+-rw-r--r--   0 root         (0) root         (0)     2963 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/dc_contract_edit.html
+-rw-r--r--   0 root         (0) root         (0)      848 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/dc_contract_hh_import.html
+-rw-r--r--   0 root         (0) root         (0)     8172 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/dc_contract_hh_imports.html
+-rw-r--r--   0 root         (0) root         (0)      773 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/dc_contracts.html
+-rw-r--r--   0 root         (0) root         (0)      711 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/dc_contracts_add.html
+-rw-r--r--   0 root         (0) root         (0)     1219 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/dc_rate_script.html
+-rw-r--r--   0 root         (0) root         (0)      644 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/dc_rate_script_add.html
+-rw-r--r--   0 root         (0) root         (0)     1955 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/dc_rate_script_edit.html
+-rw-r--r--   0 root         (0) root         (0)     2515 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/dno.html
+-rw-r--r--   0 root         (0) root         (0)      753 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/dno_rate_script.html
+-rw-r--r--   0 root         (0) root         (0)      559 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/dno_rate_script_add.html
+-rw-r--r--   0 root         (0) root         (0)     1275 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/dno_rate_script_edit.html
+-rw-r--r--   0 root         (0) root         (0)      702 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/dnos.html
+-rw-r--r--   0 root         (0) root         (0)      440 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/dtc_meter_type.html
+-rw-r--r--   0 root         (0) root         (0)      467 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/dtc_meter_types.html
+-rw-r--r--   0 root         (0) root         (0)     1493 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/duration_report.html
+-rw-r--r--   0 root         (0) root         (0)     2033 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/em_hh_data.html
+-rw-r--r--   0 root         (0) root         (0)     6647 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/em_months.html
+-rw-r--r--   0 root         (0) root         (0)     2890 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/em_site.html
+-rw-r--r--   0 root         (0) root         (0)      678 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/em_totals.html
+-rw-r--r--   0 root         (0) root         (0)      478 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/energisation_status.html
+-rw-r--r--   0 root         (0) root         (0)      587 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/energisation_statuses.html
+-rw-r--r--   0 root         (0) root         (0)     6396 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/era_edit.html
+-rw-r--r--   0 root         (0) root         (0)     2128 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/era_supplier_bill_add.html
+-rw-r--r--   0 root         (0) root         (0)      439 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/generator_type.html
+-rw-r--r--   0 root         (0) root         (0)      535 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/generator_types.html
+-rw-r--r--   0 root         (0) root         (0)      405 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/gsp_group.html
+-rw-r--r--   0 root         (0) root         (0)      453 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/gsp_groups.html
+-rw-r--r--   0 root         (0) root         (0)     1824 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/hh_datum_edit.html
+-rw-r--r--   0 root         (0) root         (0)      996 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/lafs.html
+-rw-r--r--   0 root         (0) root         (0)     1168 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/llfc.html
+-rw-r--r--   0 root         (0) root         (0)     1038 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/llfc_edit.html
+-rw-r--r--   0 root         (0) root         (0)     1143 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/llfcs.html
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/market_role.html
+-rw-r--r--   0 root         (0) root         (0)      464 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/market_roles.html
+-rw-r--r--   0 root         (0) root         (0)      659 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/meter_payment_type.html
+-rw-r--r--   0 root         (0) root         (0)      770 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/meter_payment_types.html
+-rw-r--r--   0 root         (0) root         (0)      642 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/meter_type.html
+-rw-r--r--   0 root         (0) root         (0)      661 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/meter_types.html
+-rw-r--r--   0 root         (0) root         (0)     4821 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/mop_batch.html
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/mop_batch_add.html
+-rw-r--r--   0 root         (0) root         (0)     2089 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/mop_batch_edit.html
+-rw-r--r--   0 root         (0) root         (0)     1167 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/mop_batch_file.html
+-rw-r--r--   0 root         (0) root         (0)     1899 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/mop_batch_file_edit.html
+-rw-r--r--   0 root         (0) root         (0)     1584 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/mop_batch_upload_file.html
+-rw-r--r--   0 root         (0) root         (0)     1015 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/mop_batches.html
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/mop_bill.html
+-rw-r--r--   0 root         (0) root         (0)     1712 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/mop_bill_add.html
+-rw-r--r--   0 root         (0) root         (0)     2748 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/mop_bill_edit.html
+-rw-r--r--   0 root         (0) root         (0)     3201 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/mop_bill_import.html
+-rw-r--r--   0 root         (0) root         (0)     1610 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/mop_bill_imports.html
+-rw-r--r--   0 root         (0) root         (0)     1748 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/mop_contract.html
+-rw-r--r--   0 root         (0) root         (0)      738 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/mop_contract_add.html
+-rw-r--r--   0 root         (0) root         (0)     2204 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/mop_contract_edit.html
+-rw-r--r--   0 root         (0) root         (0)      768 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/mop_contracts.html
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/mop_rate_script.html
+-rw-r--r--   0 root         (0) root         (0)      643 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/mop_rate_script_add.html
+-rw-r--r--   0 root         (0) root         (0)     1817 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/mop_rate_script_edit.html
+-rw-r--r--   0 root         (0) root         (0)     2014 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/mtc.html
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/mtc_llfc.html
+-rw-r--r--   0 root         (0) root         (0)     1400 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/mtc_llfc_ssc.html
+-rw-r--r--   0 root         (0) root         (0)     1516 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/mtc_llfc_ssc_pc.html
+-rw-r--r--   0 root         (0) root         (0)     1504 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/mtc_llfc_ssc_pcs.html
+-rw-r--r--   0 root         (0) root         (0)     1596 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/mtc_llfc_sscs.html
+-rw-r--r--   0 root         (0) root         (0)     1296 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/mtc_llfcs.html
+-rw-r--r--   0 root         (0) root         (0)     2232 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/mtc_participant.html
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/mtc_participants.html
+-rw-r--r--   0 root         (0) root         (0)      985 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/mtc_ssc.html
+-rw-r--r--   0 root         (0) root         (0)     1276 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/mtc_sscs.html
+-rw-r--r--   0 root         (0) root         (0)      853 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/mtcs.html
+-rw-r--r--   0 root         (0) root         (0)     1367 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/ods_monthly_duration.html
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/participant.html
+-rw-r--r--   0 root         (0) root         (0)      500 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/participants.html
+-rw-r--r--   0 root         (0) root         (0)      666 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/parties.html
+-rw-r--r--   0 root         (0) root         (0)     1915 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/party.html
+-rw-r--r--   0 root         (0) root         (0)      521 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/pc.html
+-rw-r--r--   0 root         (0) root         (0)      560 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/pcs.html
+-rw-r--r--   0 root         (0) root         (0)     2289 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/read_add.html
+-rw-r--r--   0 root         (0) root         (0)     3147 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/read_edit.html
+-rw-r--r--   0 root         (0) root         (0)      403 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/read_type.html
+-rw-r--r--   0 root         (0) root         (0)      473 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/read_types.html
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/scenario.html
+-rw-r--r--   0 root         (0) root         (0)      516 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/scenario_add.html
+-rw-r--r--   0 root         (0) root         (0)     5162 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/scenario_docs.html
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/scenario_edit.html
+-rw-r--r--   0 root         (0) root         (0)      847 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/scenarios.html
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/site_hh_data.html
+-rw-r--r--   0 root         (0) root         (0)      847 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/site_site_snags.html
+-rw-r--r--   0 root         (0) root         (0)      924 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/site_snag.html
+-rw-r--r--   0 root         (0) root         (0)     1436 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/site_snag_edit.html
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/site_snags.html
+-rw-r--r--   0 root         (0) root         (0)      427 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/site_snags_edit.html
+-rw-r--r--   0 root         (0) root         (0)      373 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/source.html
+-rw-r--r--   0 root         (0) root         (0)      453 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/sources.html
+-rw-r--r--   0 root         (0) root         (0)      811 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/ssc.html
+-rw-r--r--   0 root         (0) root         (0)      918 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/sscs.html
+-rw-r--r--   0 root         (0) root         (0)     5647 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/supplier_batch.html
+-rw-r--r--   0 root         (0) root         (0)     1240 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/supplier_batch_add.html
+-rw-r--r--   0 root         (0) root         (0)     1420 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/supplier_batch_edit.html
+-rw-r--r--   0 root         (0) root         (0)     1226 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/supplier_batch_file.html
+-rw-r--r--   0 root         (0) root         (0)     7618 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/supplier_batch_file_add.html
+-rw-r--r--   0 root         (0) root         (0)     2009 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/supplier_batch_file_edit.html
+-rw-r--r--   0 root         (0) root         (0)     8533 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/supplier_batch_upload_file.html
+-rw-r--r--   0 root         (0) root         (0)     1164 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/supplier_batches.html
+-rw-r--r--   0 root         (0) root         (0)     3797 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/supplier_bill.html
+-rw-r--r--   0 root         (0) root         (0)     2184 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/supplier_bill_add.html
+-rw-r--r--   0 root         (0) root         (0)     2732 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/supplier_bill_edit.html
+-rw-r--r--   0 root         (0) root         (0)     4291 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/supplier_bill_import.html
+-rw-r--r--   0 root         (0) root         (0)     9356 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/supplier_bill_imports.html
+-rw-r--r--   0 root         (0) root         (0)     2863 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/supplier_contract.html
+-rw-r--r--   0 root         (0) root         (0)      899 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/supplier_contract_add.html
+-rw-r--r--   0 root         (0) root         (0)     1463 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/supplier_contract_edit.html
+-rw-r--r--   0 root         (0) root         (0)     1508 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/supplier_contracts.html
+-rw-r--r--   0 root         (0) root         (0)     1245 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/supplier_rate_script.html
+-rw-r--r--   0 root         (0) root         (0)      690 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/supplier_rate_script_add.html
+-rw-r--r--   0 root         (0) root         (0)     1968 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/supplier_rate_script_edit.html
+-rw-r--r--   0 root         (0) root         (0)    28697 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/supply.html
+-rw-r--r--   0 root         (0) root         (0)     2723 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/supply_edit.html
+-rw-r--r--   0 root         (0) root         (0)     3587 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/supply_hh_data.html
+-rw-r--r--   0 root         (0) root         (0)     1927 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/supply_months.html
+-rw-r--r--   0 root         (0) root         (0)      553 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/supply_note_add.html
+-rw-r--r--   0 root         (0) root         (0)      954 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/supply_note_edit.html
+-rw-r--r--   0 root         (0) root         (0)      863 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/supply_notes.html
+-rw-r--r--   0 root         (0) root         (0)      180 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/supply_post.html
+-rw-r--r--   0 root         (0) root         (0)     1239 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/supply_virtual_bill.html
+-rw-r--r--   0 root         (0) root         (0)     1452 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/tpr.html
+-rw-r--r--   0 root         (0) root         (0)      258 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/e/tprs.html
+-rw-r--r--   0 root         (0) root         (0)     1437 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/edi_viewer.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 16:30:13.171385 chellow-2827/chellow/templates/g/
+-rw-r--r--   0 root         (0) root         (0)     3487 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/batch.html
+-rw-r--r--   0 root         (0) root         (0)     1035 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/batch_add.html
+-rw-r--r--   0 root         (0) root         (0)     2132 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/batch_edit.html
+-rw-r--r--   0 root         (0) root         (0)      730 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/batches.html
+-rw-r--r--   0 root         (0) root         (0)     3455 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/bill.html
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/bill_add.html
+-rw-r--r--   0 root         (0) root         (0)     2754 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/bill_edit.html
+-rw-r--r--   0 root         (0) root         (0)     4292 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/bill_import.html
+-rw-r--r--   0 root         (0) root         (0)     2795 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/bill_imports.html
+-rw-r--r--   0 root         (0) root         (0)      481 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/dn.html
+-rw-r--r--   0 root         (0) root         (0)      403 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/dns.html
+-rw-r--r--   0 root         (0) root         (0)     4024 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/era_edit.html
+-rw-r--r--   0 root         (0) root         (0)      584 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/exit_zone.html
+-rw-r--r--   0 root         (0) root         (0)     1011 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/industry_auto_importer.html
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/industry_contract.html
+-rw-r--r--   0 root         (0) root         (0)      667 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/industry_contract_add.html
+-rw-r--r--   0 root         (0) root         (0)     1377 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/industry_contract_edit.html
+-rw-r--r--   0 root         (0) root         (0)      710 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/industry_contracts.html
+-rw-r--r--   0 root         (0) root         (0)     1283 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/industry_rate_script.html
+-rw-r--r--   0 root         (0) root         (0)      638 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/industry_rate_script_add.html
+-rw-r--r--   0 root         (0) root         (0)     2401 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/industry_rate_script_edit.html
+-rw-r--r--   0 root         (0) root         (0)      560 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/ldz.html
+-rw-r--r--   0 root         (0) root         (0)     2220 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/read_add.html
+-rw-r--r--   0 root         (0) root         (0)     3181 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/read_edit.html
+-rw-r--r--   0 root         (0) root         (0)      409 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/read_type.html
+-rw-r--r--   0 root         (0) root         (0)      481 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/read_types.html
+-rw-r--r--   0 root         (0) root         (0)      577 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/reading_frequencies.html
+-rw-r--r--   0 root         (0) root         (0)      472 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/reading_frequency.html
+-rw-r--r--   0 root         (0) root         (0)      655 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/reports.html
+-rw-r--r--   0 root         (0) root         (0)     1795 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/supplier_contract.html
+-rw-r--r--   0 root         (0) root         (0)      656 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/supplier_contract_add.html
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/supplier_contract_edit.html
+-rw-r--r--   0 root         (0) root         (0)      710 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/supplier_contracts.html
+-rw-r--r--   0 root         (0) root         (0)     1283 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/supplier_rate_script.html
+-rw-r--r--   0 root         (0) root         (0)      620 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/supplier_rate_script_add.html
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/supplier_rate_script_edit.html
+-rw-r--r--   0 root         (0) root         (0)     1267 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/supplies.html
+-rw-r--r--   0 root         (0) root         (0)    10885 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/supply.html
+-rw-r--r--   0 root         (0) root         (0)     2022 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/supply_edit.html
+-rw-r--r--   0 root         (0) root         (0)      744 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/supply_note_add.html
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/supply_note_edit.html
+-rw-r--r--   0 root         (0) root         (0)      936 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/supply_notes.html
+-rw-r--r--   0 root         (0) root         (0)      438 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/unit.html
+-rw-r--r--   0 root         (0) root         (0)      441 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/g/units.html
+-rw-r--r--   0 root         (0) root         (0)     1013 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/general_import.html
+-rw-r--r--   0 root         (0) root         (0)    12208 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/general_imports.html
+-rw-r--r--   0 root         (0) root         (0)     5437 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/home.html
+-rw-r--r--   0 root         (0) root         (0)     1332 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/local_report.html
+-rw-r--r--   0 root         (0) root         (0)      701 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/local_reports.html
+-rw-r--r--   0 root         (0) root         (0)      944 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/non_core_auto_importer.html
+-rw-r--r--   0 root         (0) root         (0)     1173 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/non_core_contract.html
+-rw-r--r--   0 root         (0) root         (0)     3005 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/non_core_contract_edit.html
+-rw-r--r--   0 root         (0) root         (0)      661 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/non_core_contracts.html
+-rw-r--r--   0 root         (0) root         (0)     1283 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/non_core_rate_script.html
+-rw-r--r--   0 root         (0) root         (0)      690 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/non_core_rate_script_add.html
+-rw-r--r--   0 root         (0) root         (0)     1868 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/non_core_rate_script_edit.html
+-rw-r--r--   0 root         (0) root         (0)      244 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/object_summary.html
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/rate_server.html
+-rw-r--r--   0 root         (0) root         (0)     4040 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/report_run.html
+-rw-r--r--   0 root         (0) root         (0)     2305 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/report_run_asset_comparison.html
+-rw-r--r--   0 root         (0) root         (0)     6330 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/report_run_bill_check.html
+-rw-r--r--   0 root         (0) root         (0)     4086 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/report_run_ecoes_comparison.html
+-rw-r--r--   0 root         (0) root         (0)     3791 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/report_run_row.html
+-rw-r--r--   0 root         (0) root         (0)     4683 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/report_run_row_bill_check.html
+-rw-r--r--   0 root         (0) root         (0)     2117 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/report_run_supply_contacts.html
+-rw-r--r--   0 root         (0) root         (0)      667 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/report_runs.html
+-rw-r--r--   0 root         (0) root         (0)    10016 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/site.html
+-rw-r--r--   0 root         (0) root         (0)      422 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/site_add.html
+-rw-r--r--   0 root         (0) root         (0)     7803 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/site_edit.html
+-rw-r--r--   0 root         (0) root         (0)     3468 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/site_gen_graph.html
+-rw-r--r--   0 root         (0) root         (0)     1766 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/site_hh_data.html
+-rw-r--r--   0 root         (0) root         (0)     6562 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/site_months.html
+-rw-r--r--   0 root         (0) root         (0)     3094 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/site_used_graph.html
+-rw-r--r--   0 root         (0) root         (0)      621 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/sites.html
+-rw-r--r--   0 root         (0) root         (0)     3530 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/supplies.html
+-rw-r--r--   0 root         (0) root         (0)     2048 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/system.html
+-rw-r--r--   0 root         (0) root         (0)      623 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/tester.html
+-rw-r--r--   0 root         (0) root         (0)     3255 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/user.html
+-rw-r--r--   0 root         (0) root         (0)      399 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/user_roles.html
+-rw-r--r--   0 root         (0) root         (0)     2244 2023-02-01 16:30:10.000000 chellow-2827/chellow/templates/users.html
+-rw-r--r--   0 root         (0) root         (0)     3915 2023-02-01 16:30:10.000000 chellow-2827/chellow/testing.py
+-rw-r--r--   0 root         (0) root         (0)    18981 2023-02-01 16:30:10.000000 chellow-2827/chellow/utils.py
+-rw-r--r--   0 root         (0) root         (0)    80369 2023-02-01 16:30:10.000000 chellow-2827/chellow/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 16:30:13.123385 chellow-2827/chellow.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10650 2023-02-01 16:30:13.000000 chellow-2827/chellow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13096 2023-02-01 16:30:13.000000 chellow-2827/chellow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-01 16:30:13.000000 chellow-2827/chellow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      119 2023-02-01 16:30:13.000000 chellow-2827/chellow.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      265 2023-02-01 16:30:13.000000 chellow-2827/chellow.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-02-01 16:30:13.000000 chellow-2827/chellow.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 16:30:13.171385 chellow-2827/config/
+-rw-r--r--   0 root         (0) root         (0)      434 2023-02-01 16:30:10.000000 chellow-2827/config/chellow.conf
+-rw-r--r--   0 root         (0) root         (0)      777 2023-02-01 16:30:13.175385 chellow-2827/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1952 2023-02-01 16:30:10.000000 chellow-2827/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 16:30:13.171385 chellow-2827/test/
+-rw-r--r--   0 root         (0) root         (0)      635 2023-02-01 16:30:10.000000 chellow-2827/test/test_chellow.py
+-rw-r--r--   0 root         (0) root         (0)    12897 2023-02-01 16:30:10.000000 chellow-2827/test/test_general_import.py
+-rw-r--r--   0 root         (0) root         (0)    25017 2023-02-01 16:30:10.000000 chellow-2827/test/test_models.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-02-01 16:30:10.000000 chellow-2827/test/test_testing.py
+-rw-r--r--   0 root         (0) root         (0)     2668 2023-02-01 16:30:10.000000 chellow-2827/test/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)    39838 2023-02-01 16:30:10.000000 chellow-2827/test/test_views.py
+-rw-r--r--   0 root         (0) root         (0)    70668 2023-02-01 16:30:10.000000 chellow-2827/versioneer.py
```

### Comparing `chellow-2826/PKG-INFO` & `chellow-2827/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chellow
-Version: 2826
+Version: 2827
 Summary: Web Application for checking UK utility bills.
 Home-page: https://github.com/WessexWater/chellow
 Author: Tony Locke
 Author-email: tlocke@tlocke.org.uk
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `chellow-2826/README.md` & `chellow-2827/README.md`

 * *Files identical despite different names*

### Comparing `chellow-2826/bin/chellow_service_monitor.sh` & `chellow-2827/bin/chellow_service_monitor.sh`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/__init__.py` & `chellow-2827/chellow/__init__.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/api.py` & `chellow-2827/chellow/api.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/bank_holidays.py` & `chellow-2827/chellow/bank_holidays.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/commands.py` & `chellow-2827/chellow/commands.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/dloads.py` & `chellow-2827/chellow/dloads.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/e/aahedc.py` & `chellow-2827/chellow/e/aahedc.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/e/bill_importer.py` & `chellow-2827/chellow/e/bill_importer.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,18 +78,16 @@
             read_types = keydefaultdict(lambda k: ReadType.get_by_code(sess, k))
 
             for bf in (
                 sess.query(BatchFile)
                 .filter(BatchFile.batch == batch)
                 .order_by(BatchFile.upload_timestamp)
             ):
-
                 self.parser = _process_batch_file(sess, bf, self._log)
                 for self.bill_num, raw_bill in enumerate(self.parser.make_raw_bills()):
-
                     if "error" in raw_bill:
                         self.failed_bills.append(raw_bill)
                     else:
                         try:
                             mpan_core = raw_bill["mpan_core"]
                             supply = Supply.get_by_mpan_core(sess, mpan_core)
                             with sess.begin_nested():
```

### Comparing `chellow-2826/chellow/e/bill_parsers/activity_mop_stark_xlsx.py` & `chellow-2827/chellow/e/bill_parsers/activity_mop_stark_xlsx.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/e/bill_parsers/annual_mop_stark_xlsx.py` & `chellow-2827/chellow/e/bill_parsers/annual_mop_stark_xlsx.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/e/bill_parsers/bgb_edi.py` & `chellow-2827/chellow/e/bill_parsers/bgb_edi.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/e/bill_parsers/csv.py` & `chellow-2827/chellow/e/bill_parsers/csv.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,14 @@
         self.line_number = None
 
     def make_raw_bills(self):
         raw_bills = []
         next(iter(self.reader))  # skip title row
         blank_set = set(("",))
         for self.line_number, self.vals in enumerate(self.reader):
-
             # skip blank lines
             if len(self.vals) == 0 or set(self.vals) == blank_set:
                 continue
 
             bill_type_code = self.vals[0]
             if bill_type_code.startswith("#"):
                 continue  # skip comment lines
```

### Comparing `chellow-2826/chellow/e/bill_parsers/engie_edi.py` & `chellow-2827/chellow/e/bill_parsers/engie_edi.py`

 * *Files 0% similar despite different names*

```diff
@@ -388,15 +388,14 @@
         self.line_number = None
 
     def make_raw_bills(self):
         bills = []
         headers = {}
         bill = None
         for self.line_number, line, seg_name, elements in parse_edi(self.edi_str):
-
             try:
                 func = CODE_FUNCS[seg_name]
             except KeyError:
                 raise BadRequest(f"Code {seg_name} not recognized.")
 
             try:
                 bill = func(elements, headers)
```

### Comparing `chellow-2826/chellow/e/bill_parsers/engie_xls.py` & `chellow-2827/chellow/e/bill_parsers/engie_xls.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,15 +377,14 @@
     bills = []
     title_row = sheet.row(0)
     for row_index in range(1, sheet.nrows):
         row = sheet.row(row_index)
         if len(row) > 21:
             val = row[21].value
             if val not in (None, ""):
-
                 try:
                     bills.append(_parse_row(row, row_index, datemode, title_row))
                 except BadRequest as e:
                     raise BadRequest(f"On row {row_index + 1}: {e.description}")
 
     return bills
```

### Comparing `chellow-2826/chellow/e/bill_parsers/gdf_csv.py` & `chellow-2827/chellow/e/bill_parsers/gdf_csv.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/e/bill_parsers/haven_csv.py` & `chellow-2827/chellow/e/bill_parsers/haven_csv.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,14 @@
     def make_raw_bills(self):
         raw_bills = []
         sess = Session()
         headers = {"sess": sess}
 
         blank_set = set(("",))
         for self.line_number, row in enumerate(self.reader):
-
             # skip blank lines
             if len(row) == 0 or set(row) == blank_set:
                 continue
 
             try:
                 bill = _process_line(row[0], row[1:], headers)
             except BadRequest as e:
```

### Comparing `chellow-2826/chellow/e/bill_parsers/haven_edi.py` & `chellow-2827/chellow/e/bill_parsers/haven_edi.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/e/bill_parsers/haven_edi_tprs.py` & `chellow-2827/chellow/e/bill_parsers/haven_edi_tprs.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,15 +242,14 @@
     ctot = elements["CTOT"]
     if len(ctot[0]) > 0:
         breakdown["standing-gbp"] += to_decimal(ctot) / Decimal("100")
 
 
 def _process_MTR(elements, headers):
     if headers["message_type"] == "UTLBIL":
-
         if headers["mpan_core"] is None:
             sess = headers["sess"]
             era = (
                 sess.query(Era)
                 .filter(Era.imp_supplier_account == headers["account"])
                 .first()
             )
@@ -333,15 +332,14 @@
     def make_raw_bills(self):
         bills = []
         sess = Session()
         headers = {"sess": sess}
         bill = None
         try:
             for self.line_number, line, seg_name, elements in parse_edi(self.edi_str):
-
                 try:
                     func = CODE_FUNCS[seg_name]
                 except KeyError:
                     raise BadRequest(f"Code {seg_name} not recognized.")
 
                 try:
                     bill = func(elements, headers)
```

### Comparing `chellow-2826/chellow/e/bill_parsers/mm.py` & `chellow-2827/chellow/e/bill_parsers/mm.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/e/bill_parsers/nonsettlement_dc_stark_xlsx.py` & `chellow-2827/chellow/e/bill_parsers/nonsettlement_dc_stark_xlsx.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,25 +5,22 @@
 from werkzeug.exceptions import BadRequest
 
 from chellow.models import Session
 from chellow.utils import ct_datetime, parse_mpan_core, to_utc
 
 
 def get_ct_date(title_row, row, name):
-
     return get_value(title_row, row, name)
 
 
 def get_start_date(title_row, row, name):
-
     return to_utc(get_ct_date(title_row, row, name))
 
 
 def get_finish_date(title_row, row, name):
-
     d = get_ct_date(title_row, row, name)
 
     return to_utc(ct_datetime(d.year, d.month, d.day, 23, 30))
 
 
 def get_value(title_row, row, name):
     idx = None
@@ -37,15 +34,14 @@
     if idx is None:
         raise BadRequest(
             "The name '{name}' can't be found in the titles "
             "{title_row}.".format(name=name, title_row=title_row)
         )
 
     try:
-
         return row[idx].value
 
     except IndexError:
         raise BadRequest(
             f"For the row {row}, the index is {idx} which is beyond the end of the row."
         )
 
@@ -58,15 +54,14 @@
     try:
         return Decimal(str(get_value(title_row, row, name)))
     except InvalidOperation:
         return None
 
 
 def get_int(title_row, row, name):
-
     return int(get_value(title_row, row, name))
 
 
 METER_RATE = Decimal("60.00")
 
 
 class Parser:
```

### Comparing `chellow-2826/chellow/e/bill_parsers/settlement_dc_stark_xlsx.py` & `chellow-2827/chellow/e/bill_parsers/settlement_dc_stark_xlsx.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/e/bill_parsers/sse_edi.py` & `chellow-2827/chellow/e/bill_parsers/sse_edi.py`

 * *Files 0% similar despite different names*

```diff
@@ -437,15 +437,14 @@
     ctot = elements["CTOT"]
     if len(ctot[0]) > 0:
         breakdown["standing-gbp"] += to_decimal(ctot) / Decimal("100")
 
 
 def _process_MTR(elements, headers):
     if headers["message_type"] == "UTLBIL":
-
         if headers["mpan_core"] is None:
             sess = headers["sess"]
             era = (
                 sess.query(Era)
                 .filter(Era.imp_supplier_account == headers["account"])
                 .first()
             )
@@ -528,15 +527,14 @@
     def make_raw_bills(self):
         bills = []
         sess = Session()
         headers = {"sess": sess}
         bill = None
         try:
             for self.line_number, line, seg_name, elements in parse_edi(self.edi_str):
-
                 try:
                     func = CODE_FUNCS[seg_name]
                 except KeyError:
                     raise BadRequest(f"Code {seg_name} not recognized.")
 
                 try:
                     bill = func(elements, headers)
```

### Comparing `chellow-2826/chellow/e/bill_parsers/sww_xls.py` & `chellow-2827/chellow/e/bill_parsers/sww_xls.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/e/bmarketidx.py` & `chellow-2827/chellow/e/bmarketidx.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/e/bsuos.py` & `chellow-2827/chellow/e/bsuos.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/e/ccl.py` & `chellow-2827/chellow/e/ccl.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/e/computer.py` & `chellow-2827/chellow/e/computer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1135,15 +1135,14 @@
 
             if hist_measurement_type == "amr" and self.era_map.get(
                 "use_amr_hh_data", False
             ):
                 hist_measurement_type = "hh"
 
             if hist_measurement_type == "unmetered":
-
                 kwh = (
                     hist_era.imp_sc
                     * 60
                     * 30
                     / (
                         Datetime(chunk_start.year + 1, 1, 1)
                         - Datetime(chunk_start.year, 1, 1)
@@ -1266,15 +1265,14 @@
                             .join(
                                 pres_type_alias,
                                 RegisterRead.present_type_id == pres_type_alias.id,
                             )
                             .filter(RegisterRead.bill == bill, RegisterRead.units == 0)
                             .order_by(RegisterRead.present_date)
                         ):
-
                             if tpr_code not in tpr_codes:
                                 self._add_problem(
                                     f"The TPR {tpr_code} from the register read does "
                                     f"not match any of the TPRs "
                                     f"({', '.join(tpr_codes)}) associated with the "
                                     f"MPAN."
                                 )
@@ -1295,15 +1293,14 @@
                                 f"{hh_format(chunk_start)} to "
                                 f"{hh_format(chunk_finish)} is {kwh}\n"
                             )
 
                             kws[tpr_code] += kwh
 
                         for tpr_code, kwh in kws.items():
-
                             if (
                                 present_type in ACTUAL_READ_TYPES
                                 and previous_type in ACTUAL_READ_TYPES
                             ):
                                 status = "A"
                             else:
                                 status = "E"
@@ -1690,15 +1687,14 @@
 
 
 def _make_reads(forwards, prev_reads, pres_reads):
     prev_read = next(prev_reads, None)
     pres_read = next(pres_reads, None)
 
     while prev_read is not None or pres_read is not None:
-
         if prev_read is None:
             yield pres_read
             pres_read = next(pres_reads, None)
 
         elif pres_read is None:
             yield prev_read
             prev_read = next(prev_reads, None)
@@ -1833,16 +1829,15 @@
                     "start_date": chunk_start,
                     "finish_date": chunk_finish,
                     "is_import": is_import,
                 },
             )
         )
 
-        for (hist_start, status, msp_kwh, imp_kvarh, exp_kvarh) in data:
-
+        for hist_start, status, msp_kwh, imp_kvarh, exp_kvarh in data:
             datum = {
                 "imp-msp-kvarh": imp_kvarh,
                 "imp-msp-kvar": imp_kvarh * 2,
                 "exp-msp-kvarh": exp_kvarh,
                 "exp-msp-kvar": exp_kvarh * 2,
             }
             if msp_kwh is not None:
```

### Comparing `chellow-2826/chellow/e/dno_rate_parser.py` & `chellow-2827/chellow/e/dno_rate_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -478,24 +478,22 @@
 
 
 def rate_server_import(sess, log, set_progress, s, paths):
     log("Starting to check for new DNO spreadsheets")
     year_entries = {}
     for path, url in paths:
         if len(path) == 5:
-
             year_str, utility, rate_type, dno_code, file_name = path
             year = int(year_str)
             try:
                 dno_entries = year_entries[year]
             except KeyError:
                 dno_entries = year_entries[year] = {}
 
             if utility == "electricity" and rate_type == "duos":
-
                 try:
                     fl_entries = dno_entries[dno_code]
                 except KeyError:
                     fl_entries = dno_entries[dno_code] = {}
 
                 fl_entries[file_name] = url
```

### Comparing `chellow-2826/chellow/e/duos.py` & `chellow-2827/chellow/e/duos.py`

 * *Files 0% similar despite different names*

```diff
@@ -504,15 +504,14 @@
         try:
             laf = laf_cache_llfc[start_date]
         except KeyError:
             dno_code = ds.dno_code
             if dno_code in ("88", "99"):
                 laf_cache_llfc[start_date] = 1
             else:
-
                 m_start, m_finish = next(
                     c_months_u(
                         start_year=hh["ct-year"], start_month=hh["ct-month"], months=1
                     )
                 )
                 for (laf,) in ds.sess.execute(
                     select(Laf)
@@ -701,15 +700,14 @@
             laf_cache_llfc = laf_cache[ds.llfc_code]
         except KeyError:
             laf_cache_llfc = laf_cache[ds.llfc_code] = {}
 
         try:
             laf = laf_cache_llfc[start_date]
         except KeyError:
-
             for laf_obj in ds.sess.execute(
                 select(Laf)
                 .join(Llfc)
                 .join(Party)
                 .where(
                     Party.dno_code == ds.dno_code,
                     Llfc.code == ds.llfc_code,
```

### Comparing `chellow-2826/chellow/e/energy_management.py` & `chellow-2827/chellow/e/energy_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,14 @@
                 .options(
                     joinedload(Era.imp_supplier_contract),
                     joinedload(Era.exp_supplier_contract),
                     joinedload(Era.mop_contract),
                     joinedload(Era.dc_contract),
                 )
             ).scalars():
-
                 chunk_start = hh_max(era.start_date, month_start)
                 chunk_finish = hh_min(era.finish_date, month_finish)
 
                 log("about to call first supplysource")
                 supply_ds = SupplySource(
                     sess,
                     chunk_start,
```

### Comparing `chellow-2826/chellow/e/hh_importer.py` & `chellow-2827/chellow/e/hh_importer.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/e/hh_parser_bg_csv.py` & `chellow-2827/chellow/e/hh_parser_bg_csv.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/e/hh_parser_df2.py` & `chellow-2827/chellow/e/hh_parser_df2.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/e/hh_parser_simple_csv.py` & `chellow-2827/chellow/e/hh_parser_simple_csv.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/e/laf_import.py` & `chellow-2827/chellow/e/laf_import.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,14 @@
     try:
         laf_state = state["laf_importer"]
     except KeyError:
         laf_state = state["laf_importer"] = {}
 
     for path, url in paths:
         if len(path) == 4:
-
             year_str, utility, rate_type, file_name = path
 
             if utility == "electricity" and rate_type == "lafs":
                 # File name llfetcl20220401ptf.zip
                 if not file_name.startswith(LAF_START):
                     raise BadRequest(f"A laf file must begin with '{LAF_START}'")
                 if not file_name.endswith(LAF_END):
```

### Comparing `chellow-2826/chellow/e/mdd_importer.py` & `chellow-2827/chellow/e/mdd_importer.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,14 @@
             c.start_minute,
             c.end_hour,
             c.end_minute,
         )
         for c in sess.execute(select(ClockInterval)).scalars()
     }
     for values in rows:
-
         tpr_code = values[0].zfill(5)
         day_of_week = int(values[1])
         start_day = int(values[2])
         start_month = int(values[3])
         end_day = int(values[4])
         end_month = int(values[5])
         start_hour, start_minute = [int(v) for v in values[6].split(":")]
@@ -271,15 +270,14 @@
 
 def _import_Measurement_Requirement(sess, rows, ctx):
     mrs = {
         (mr.ssc.code, mr.tpr.code)
         for mr in sess.execute(select(MeasurementRequirement)).scalars()
     }
     for values in rows:
-
         ssc_code = Ssc.normalise_code(values[0])
         tpr_code = Tpr.normalise_code(values[1])
 
         if (ssc_code, tpr_code) not in mrs:
             ssc = sess.execute(
                 select(Ssc).where(Ssc.code == ssc_code).order_by(Ssc.valid_from.desc())
             ).scalar()
@@ -398,15 +396,14 @@
             meter_payment_type = meter_payment_types[meter_payment_type_code]
             has_comms = values[8] == "Y"  # MTC Comm. Indicator
             is_hh = values[9] == "H"  # MTC Type Indicator
             tpr_count_str = values[10]  # TPR Count
             tpr_count = 0 if tpr_count_str == "" else int(tpr_count_str)
 
         if mtc_participant is None:
-
             MtcParticipant.insert(
                 sess,
                 mtc,
                 participant,
                 description,
                 has_comms,
                 is_hh,
@@ -835,15 +832,14 @@
 
 
 def rate_server_import(sess, log, set_progress, s, paths):
     log("Starting to check for a new MDD version")
     mdd_entries = {}
     for path, url in paths:
         if len(path) == 5:
-
             _, utility, rate_type, mdd_version_str, file_name = path
 
             if utility == "electricity" and rate_type == "mdd":
                 mdd_version = int(mdd_version_str)
                 try:
                     fl_entries = mdd_entries[mdd_version]
                 except KeyError:
@@ -918,15 +914,14 @@
             "Valid_MTC_LLFC_SSC_PC_Combination",
             _import_Valid_MTC_LLFC_SSC_PC_Combination,
         ),
         ("Time_Pattern_Regime", _import_Time_Pattern_Regime),
         ("Clock_Interval", _import_Clock_Interval),
         ("Measurement_Requirement", _import_Measurement_Requirement),
     ]:
-
         if tname in gnames:
             log(f"Found {tname} and will now import it.")
             func(sess, gnames[tname], ctx)
         else:
             raise BadRequest(f"Can't find {tname} on the rate server.")
 
     config = Contract.get_non_core_by_name(sess, "configuration")
```

### Comparing `chellow-2826/chellow/e/rcrc.py` & `chellow-2827/chellow/e/rcrc.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/e/ro.py` & `chellow-2827/chellow/e/ro.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/e/scenario.py` & `chellow-2827/chellow/e/scenario.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,14 @@
                 SiteEra.is_physical == true(),
                 Era.imp_mpan_core != null(),
                 Pc.code != "00",
                 Era.start_date <= chunk_finish,
                 or_(Era.finish_date == null(), Era.finish_date >= chunk_start),
             )
         ):
-
             if supply_ids is not None and era.supply_id not in supply_ids:
                 continue
 
             ss_start = hh_max(era.start_date, chunk_start)
             ss_finish = hh_min(era.finish_date, chunk_finish)
 
             ss = SupplySource(
@@ -185,15 +184,14 @@
                 SiteEra.is_physical == true(),
                 Era.imp_mpan_core != null(),
                 Era.start_date <= chunk_finish,
                 or_(Era.finish_date == null(), Era.finish_date >= chunk_start),
                 Source.code == "gen-net",
             )
         ):
-
             if supply_ids is not None and era.supply_id not in supply_ids:
                 continue
 
             ss_start = hh_max(era.start_date, chunk_start)
             ss_finish = hh_min(era.finish_date, chunk_finish)
 
             ss = SupplySource(
@@ -383,15 +381,14 @@
             joinedload(Era.supply).joinedload(Supply.source),
             joinedload(Era.mtc_participant).joinedload(MtcParticipant.meter_type),
             joinedload(Era.pc),
             joinedload(Era.site_eras),
         )
         .order_by(Era.supply_id, Era.start_date)
     ):
-
         supply = era.supply
         if data_source_bill is not None and supply.dno.dno_code in ("88", "99"):
             continue
 
         if supply.generator_type is not None:
             site_gen_types.add(supply.generator_type.code)
```

### Comparing `chellow-2826/chellow/e/system_price.py` & `chellow-2827/chellow/e/system_price.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/e/tlms.py` & `chellow-2827/chellow/e/tlms.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,14 @@
     cache = {}
     try:
         sess = Session()
         log_func("Starting to check TLMs.")
         contract = Contract.get_non_core_by_name(sess, "tlms")
         contract_props = contract.make_properties()
         if contract_props.get("enabled", False):
-
             config = Contract.get_non_core_by_name(sess, "configuration")
             props = config.make_properties()
             scripting_key = props.get(ELEXON_PORTAL_SCRIPTING_KEY_KEY)
             if scripting_key is None:
                 raise BadRequest(
                     f"The property {ELEXON_PORTAL_SCRIPTING_KEY_KEY} cannot be found "
                     f"in the configuration properties."
```

### Comparing `chellow-2826/chellow/e/tnuos.py` & `chellow-2827/chellow/e/tnuos.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     to_utc,
 )
 
 BANDED_START = to_utc(ct_datetime(2023, 4, 1))
 
 
 def hh(ds, rate_period="monthly", est_kw=None):
-
     for hh in ds.hh_data:
         if hh["start-date"] >= BANDED_START:
             if hh["ct-decimal-hour"] == 12:
                 _process_banded_hh(ds, hh)
         else:
             if hh["ct-is-month-end"]:
                 _process_triad_hh(ds, rate_period, est_kw, hh)
@@ -298,19 +297,15 @@
     val = row[idx].value
     if isinstance(val, str):
         return val.strip()
     else:
         return val
 
 
-def find_bands(file_like):
-    book = load_workbook(file_like, data_only=True)
-
-    tabs = {sheet.title.strip(): sheet for sheet in book.worksheets}
-
+def find_bands(tabs):
     tab_name = "T10"
     try:
         sheet = tabs[tab_name]
     except KeyError:
         raise BadRequest(f"Can't find the tab named '{tab_name}'")
 
     bands = {}
@@ -327,25 +322,73 @@
 
         elif val_0 == "Band":
             in_bands = True
 
     return bands
 
 
+def find_triad(tabs):
+    GSP_LOOKUP = {
+        1: "_P",
+        2: "_N",
+        3: "_F",
+        4: "_G",
+        5: "_M",
+        6: "_D",
+        7: "_B",
+        8: "_E",
+        9: "_A",
+        10: "_K",
+        11: "_J",
+        12: "_C",
+        13: "_H",
+        14: "_L",
+    }
+
+    tab_name = "T9"
+    try:
+        sheet = tabs[tab_name]
+    except KeyError:
+        raise BadRequest(f"Can't find the tab named '{tab_name}'")
+
+    triads = {"import": {}, "export": {}}
+
+    in_triads = False
+    for row in range(1, len(sheet["A"]) + 1):
+        val = get_cell(sheet, "A", row).value
+        if val is None:
+            val_0 = None
+        elif isinstance(val, str):
+            val_0 = " ".join(val.split())
+        else:
+            val_0 = val
+
+        if in_triads:
+            if val_0 is None or val_0 == "":
+                in_triads = False
+            else:
+                gsp_group_code = GSP_LOOKUP[val_0]
+                triads["import"][gsp_group_code] = get_dec(sheet, "C", row)
+                triads["export"][gsp_group_code] = get_dec(sheet, "E", row)
+
+        elif val_0 == "Zone":
+            in_triads = True
+
+    return triads
+
+
 def rate_server_import(sess, log, set_progress, s, paths):
     log("Starting to check for new TNUoS spreadsheets")
     year_entries = {}
     for path, url in paths:
         if len(path) == 4:
-
             year_str, utility, rate_type, file_name = path
             year = int(year_str)
 
             if utility == "electricity" and rate_type == "tnuos":
-
                 try:
                     fl_entries = year_entries[year]
                 except KeyError:
                     fl_entries = year_entries[year] = {}
 
                 fl_entries[file_name] = url
 
@@ -366,21 +409,25 @@
 
         file_name, url = sorted(fl_entries.items())[-1]
 
         rs_script = rs.make_script()
         if rs_script.get("a_file_name") != file_name:
             try:
                 fl = BytesIO(download(s, url))
+                book = load_workbook(fl, data_only=True)
+                tabs = {sheet.title.strip(): sheet for sheet in book.worksheets}
                 try:
-                    bands = find_bands(fl)
+                    bands = find_bands(tabs)
+                    triad = find_triad(tabs)
                 except BadRequest as e:
                     raise BadRequest(
                         f"Problem with file '{file_name}': {e.description}"
                     )
                 rs_script["bands"] = bands
+                rs_script["triad_gbp_per_gsp_kw"] = triad
                 rs_script["a_file_name"] = file_name
                 rs.update(rs_script)
                 log(f"Updated TNUoS rate script for " f"{hh_format(fy_start)}")
             except BadRequest as e:
                 raise BadRequest(f"Problem with year {year}: {e.description}")
 
     log("Finished TNUoS spreadsheets")
```

### Comparing `chellow-2826/chellow/e/views.py` & `chellow-2827/chellow/e/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -3517,15 +3517,14 @@
 
 
 @e.route("/sites/<int:site_id>/energy_management/totals")
 def em_totals(site_id):
     site = Site.get_by_id(g.sess, site_id)
 
     if "mem_id" in request.values:
-
         mem_id = req_int("mem_id")
         site_info = chellow.dloads.get_mem_val(mem_id)
         random_number = random()
 
         status_code = 200 if site_info["status"] == "running" else 286
         return make_response(
             render_template(
@@ -4627,15 +4626,14 @@
                 Channel.id.in_(channel_ids),
                 HhDatum.start_date >= month_start,
                 HhDatum.start_date <= month_finish,
             )
             .group_by(HhDatum.start_date)
         )
         for kwh, kvarh, hh_date in g.sess.execute(s):
-
             kvah = (kwh**2 + kvarh**2) ** 0.5
             if kvah > md_kvah:
                 md_kvah = kvah
                 month_data["md_kva"] = 2 * md_kvah
                 month_data["md_kvar"] = kvarh * 2
                 month_data["md_kw"] = kwh * 2
                 month_data["md_pf"] = kwh / kvah
```

### Comparing `chellow-2826/chellow/edi_lib.py` & `chellow-2827/chellow/edi_lib.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/gas/bill_import.py` & `chellow-2827/chellow/gas/bill_import.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/gas/bill_parser_csv.py` & `chellow-2827/chellow/gas/bill_parser_csv.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,14 @@
     def _set_last_line(self, line):
         self.last_line = line
         return line
 
     def make_raw_bills(self):
         raw_bills = []
         for self._line_number, row in enumerate(self.csv_reader):
-
             bill_reference = row[0]
             if bill_reference == "" or bill_reference.startswith("#"):
                 continue
 
             mprn = row[1]
             bill_type = row[2]
             account = row[3]
```

### Comparing `chellow-2826/chellow/gas/bill_parser_engie_edi.py` & `chellow-2827/chellow/gas/bill_parser_engie_edi.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,15 +291,14 @@
         self.line_number = None
 
     def make_raw_bills(self):
         bills = []
         headers = {}
         bill = None
         for self.line_number, line, seg_name, elements in parse_edi(self.edi_str):
-
             try:
                 func = CODE_FUNCS[seg_name]
             except KeyError:
                 raise BadRequest(f"Code {seg_name} not recognized.")
 
             bill = func(elements, headers)
```

### Comparing `chellow-2826/chellow/gas/cv.py` & `chellow-2827/chellow/gas/cv.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/gas/dn_rate_parser.py` & `chellow-2827/chellow/gas/dn_rate_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,15 +196,14 @@
     "ldz customer fixed charges": State.CUSTOMER_FIXED,
     "csep administration charge": State.ADMIN_CHARGE,
     "exit capacity unit rates by exit zone": State.EXIT_CAPACITY,
 }
 
 
 def tab_gdn_unit_rates(sheet, rates):
-
     state = State.BLANK
     networks = {}
 
     for row in range(1, len(sheet["B"]) + 1):
         cell_1 = get_cell(sheet, "B", row)
         if isinstance(cell_1, openpyxl.cell.cell.Cell):
             val_1 = normalize_text(get_value(sheet, "B", row))
@@ -260,15 +259,14 @@
 
 def rate_server_import(sess, log, set_progress, s, paths):
     log("Starting to check for new DN spreadsheets")
 
     year_entries = {}
     for path, url in paths:
         if len(path) == 4:
-
             year_str, utility, rate_type, file_name = path
             if utility == "gas" and rate_type == "dn":
                 year = int(year_str)
                 try:
                     fl_entries = year_entries[year]
                 except KeyError:
                     fl_entries = year_entries[year] = {}
```

### Comparing `chellow-2826/chellow/gas/engine.py` & `chellow-2827/chellow/gas/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,14 @@
 
 def forecast_date():
     now = utc_datetime_now()
     return utc_datetime(now.year, now.month, 1)
 
 
 def get_data_sources(ds, start_date, finish_date, forecast_date=None):
-
     if forecast_date is None:
         forecast_date = ds.forecast_date
 
     if (
         ds.start_date == start_date
         and ds.finish_date == finish_date
         and forecast_date == ds.forecast_date
@@ -571,15 +570,14 @@
     hist_g_era,
     chunk_start,
     chunk_finish,
     cv_id,
     hist_map,
     g_ldz_code,
 ):
-
     cf = float(hist_g_era.correction_factor)
     g_unit = hist_g_era.g_unit
     unit_code, unit_factor = g_unit.code, float(g_unit.factor)
 
     for hh_date in hh_range(caches, chunk_start, chunk_finish):
         cv, avg_cv = find_cv(sess, caches, cv_id, hh_date, g_ldz_code)
         hist_map[hh_date] = {
@@ -736,15 +734,14 @@
     return hhs
 
 
 def _make_reads(forwards, prev_reads, pres_reads):
     prev_read = next(prev_reads, None)
     pres_read = next(pres_reads, None)
     while prev_read is not None or pres_read is not None:
-
         if prev_read is None:
             yield pres_read
             pres_read = next(pres_reads, None)
 
         elif pres_read is None:
             yield prev_read
             prev_read = next(prev_reads, None)
```

### Comparing `chellow-2826/chellow/gas/transportation.py` & `chellow-2827/chellow/gas/transportation.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/gas/views.py` & `chellow-2827/chellow/gas/views.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/general_import.py` & `chellow-2827/chellow/general_import.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/models.py` & `chellow-2827/chellow/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -407,15 +407,14 @@
 
     def __init__(self, code, description):
         self.code = code
         self.description = description
 
 
 class VoltageLevel(Base, PersistentClass):
-
     __tablename__ = "voltage_level"
     id = Column(Integer, primary_key=True)
     code = Column(String, unique=True, nullable=False)
     name = Column(String, unique=True, nullable=False)
     llfcs = relationship("Llfc", backref="voltage_level")
 
     def __init__(self, code, name):
@@ -599,15 +598,14 @@
         previous_date,
         previous_value,
         previous_type,
         present_date,
         present_value,
         present_type,
     ):
-
         self.bill = bill
         self.update(
             tpr,
             coefficient,
             units,
             msn,
             mpan_str,
@@ -657,15 +655,14 @@
         sess.flush()
 
     def units_as_str(self):
         return self.UNITS_INT[self.units]
 
 
 class BatchFile(Base, PersistentClass):
-
     __tablename__ = "batch_file"
     id = Column(Integer, primary_key=True)
     batch_id = Column(
         Integer, ForeignKey("batch.id", ondelete="CASCADE"), nullable=False, index=True
     )
     filename = Column(String, nullable=False, index=True)
     upload_timestamp = Column(DateTime(timezone=True), nullable=False, index=True)
@@ -684,15 +681,14 @@
 
     def delete(self, sess):
         sess.delete(self)
         sess.flush()
 
 
 class Bill(Base, PersistentClass):
-
     __tablename__ = "bill"
     id = Column(Integer, primary_key=True)
     batch_id = Column(Integer, ForeignKey("batch.id"), nullable=False, index=True)
     supply_id = Column(Integer, ForeignKey("supply.id"), nullable=False)
     issue_date = Column(DateTime(timezone=True), nullable=False, index=True)
     start_date = Column(DateTime(timezone=True), nullable=False, index=True)
     finish_date = Column(DateTime(timezone=True), nullable=False, index=True)
@@ -1054,15 +1050,14 @@
         description,
         voltage_level,
         is_substation,
         is_import,
         valid_from,
         valid_to,
     ):
-
         if self.market_role.code == "R":
             llfc = Llfc(
                 self,
                 code,
                 description,
                 voltage_level,
                 is_substation,
@@ -2365,15 +2360,14 @@
         self.update(
             description, voltage_level, is_substation, is_import, valid_from, valid_to
         )
 
     def update(
         self, description, voltage_level, is_substation, is_import, valid_from, valid_to
     ):
-
         self.description = description
         self.voltage_level = voltage_level
         self.is_substation = is_substation
         self.is_import = is_import
         self.valid_from = valid_from
         self.valid_to = valid_to
 
@@ -2630,15 +2624,14 @@
         is_hh,
         meter_type,
         meter_payment_type,
         tpr_count,
         valid_from,
         valid_to,
     ):
-
         self.description = description
         self.has_comms = has_comms
         self.is_hh = is_hh
         self.meter_type = meter_type
         self.meter_payment_type = meter_payment_type
         self.tpr_count = tpr_count
         self.valid_from = valid_from
@@ -2727,15 +2720,14 @@
             valid_to,
         )
 
     def update(
         self,
         valid_to,
     ):
-
         self.valid_to = valid_to
 
         if hh_after(self.valid_from, valid_to):
             raise BadRequest("The valid_from date can't be after the valid_to date.")
 
     @classmethod
     def insert(
@@ -2814,15 +2806,14 @@
             valid_to,
         )
 
     def update(
         self,
         valid_to,
     ):
-
         self.valid_to = valid_to
 
         if hh_after(self.valid_from, valid_to):
             raise BadRequest("The valid_from date can't be after the valid_to date.")
 
     @classmethod
     def insert(
@@ -2894,15 +2885,14 @@
             valid_to,
         )
 
     def update(
         self,
         valid_to,
     ):
-
         self.valid_to = valid_to
 
         if hh_after(self.valid_from, valid_to):
             raise BadRequest("The valid_from date can't be after the valid_to date.")
 
     @classmethod
     def insert(
@@ -3481,15 +3471,14 @@
         imp_sc,
         exp_mpan_core,
         exp_llfc_code,
         exp_supplier_contract,
         exp_supplier_account,
         exp_sc,
     ):
-
         orig_start_date = self.start_date
         orig_finish_date = self.finish_date
 
         if hh_after(start_date, finish_date):
             raise BadRequest("The era start date can't be after the finish date.")
 
         if imp_mpan_core is None and exp_mpan_core is None:
@@ -4022,15 +4011,14 @@
                     or_(Era.imp_mpan_core == mpan_core, Era.exp_mpan_core == mpan_core)
                 )
                 .first()
             )
 
     @staticmethod
     def _settle_stripe(sess, start_date, finish_date, old_era, new_era):
-
         # move snags from old to new
         if old_era is None:
             for channel in (
                 sess.query(Channel).filter(Channel.era == new_era).order_by(Channel.id)
             ):
                 channel.add_snag(sess, Snag.MISSING, start_date, finish_date)
 
@@ -4052,15 +4040,14 @@
                         f"and {hh_format(finish_date)}."
                     )
 
         if old_era is not None and new_era is not None:
             for channel in (
                 sess.query(Channel).filter(Channel.era == old_era).order_by(Channel.id)
             ):
-
                 snags = (
                     sess.query(Snag)
                     .filter(
                         Snag.channel == channel,
                         or_(Snag.finish_date == null(), Snag.finish_date >= start_date),
                     )
                     .order_by(Snag.id)
@@ -4746,15 +4733,14 @@
         self.value = value
         self.status = status
         nw = utc_datetime_now()
         self.last_modified = utc_datetime(year=nw.year, month=nw.month, day=nw.day)
 
 
 class Report(Base, PersistentClass):
-
     __tablename__ = "report"
     id = Column(Integer, primary_key=True)
     name = Column(String, unique=True, nullable=False)
     script = Column(Text, nullable=False)
     template = Column(Text, nullable=False)
 
     def __init__(self, name, script, template):
@@ -5222,15 +5208,14 @@
         msn,
         correction_factor,
         g_unit,
         g_contract,
         account,
         g_reading_frequency,
     ):
-
         if hh_after(start_date, finish_date):
             raise BadRequest("The era start date can't be after the finish date.")
 
         self.start_date = start_date
         self.finish_date = finish_date
         self.msn = msn
         self.correction_factor = correction_factor
@@ -5654,15 +5639,14 @@
         prev_value,
         prev_date,
         prev_type,
         pres_value,
         pres_date,
         pres_type,
     ):
-
         read = GRegisterRead(
             self,
             msn,
             g_units,
             correction_factor,
             calorific_value,
             prev_value,
@@ -5737,15 +5721,14 @@
         kwh,
         net_gbp,
         vat_gbp,
         gross_gbp,
         raw_lines,
         breakdown,
     ):
-
         g_bill = GBill(
             self,
             g_supply,
             bill_type,
             reference,
             account,
             issue_date,
```

### Comparing `chellow-2826/chellow/proxy.py` & `chellow-2827/chellow/proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     ) -> None:
         self.app = app
         self.x_proto = None
 
     def __call__(
         self, environ: "WSGIEnvironment", start_response: "StartResponse"
     ) -> t.Iterable[bytes]:
-
         try:
             x_proto = environ["HTTP_X_FORWARDED_PROTO"]
         except KeyError:
             x_proto = _get_proto_override()
 
         if x_proto is not None:
             environ["wsgi.url_scheme"] = x_proto
```

### Comparing `chellow-2826/chellow/rate_server.py` & `chellow-2827/chellow/rate_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 def download(s, url):
     fl_json = s.get(url).json()
     return b64decode(fl_json["content"])
 
 
 def run_import(sess, log, set_progress):
-
     log("Starting to import rates from the rate server")
     conf = Contract.get_non_core_by_name(sess, "configuration")
     props = conf.make_properties()
     repo_props = props.get("rate_server", {})
     repo_url = repo_props.get(
         "url", "https://api.github.com/repos/WessexWater/chellow-rates"
     )
@@ -52,15 +51,14 @@
     if tree_entry["truncated"]:
         raise Exception("Tree from rate server is truncated.")
 
     paths_list = []
     for sub_entry in tree_entry["tree"]:
         path = sub_entry["path"].split("/")
         if path[-1] != "README.md":
-
             paths_list.append((path, sub_entry["url"]))
 
     paths = tuple(paths_list)
 
     for mod_name in (
         "chellow.e.dno_rate_parser",
         "chellow.e.laf_import",
```

### Comparing `chellow-2826/chellow/reports/report_109.py` & `chellow-2827/chellow/reports/report_109.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/reports/report_111.py` & `chellow-2827/chellow/reports/report_111.py`

 * *Files 0% similar despite different names*

```diff
@@ -513,15 +513,14 @@
                 joinedload(Era.mtc_participant).joinedload(MtcParticipant.meter_type),
                 joinedload(Era.pc),
                 joinedload(Era.supply).joinedload(Supply.dno),
                 joinedload(Era.supply).joinedload(Supply.gsp_group),
                 joinedload(Era.supply).joinedload(Supply.source),
             )
         ):
-
             chunk_start = hh_max(covered_start, era.start_date)
             chunk_finish = hh_min(covered_finish, era.finish_date)
 
             if contract not in (
                 era.mop_contract,
                 era.dc_contract,
                 era.imp_supplier_contract,
@@ -754,15 +753,14 @@
         )
 
         for bill in sess.query(Bill).filter(
             Bill.supply == supply,
             Bill.start_date <= covered_finish,
             Bill.finish_date >= covered_start,
         ):
-
             for k, v in loads(bill.breakdown).items():
                 if k.endswith("-gbp"):
                     add_gap(
                         caches,
                         gaps,
                         k[:-4],
                         bill.start_date,
@@ -774,15 +772,14 @@
         # Avoid long-running transactions
         sess.commit()
 
     clumps = []
     for element, elgap in sorted(gaps.items()):
         for start_date, hhgap in sorted(elgap.items()):
             if hhgap["has_virtual"] and not hhgap["has_covered"]:
-
                 if len(clumps) == 0 or not all(
                     (
                         clumps[-1]["element"] == element,
                         clumps[-1]["finish_date"] + HH == start_date,
                     )
                 ):
                     clumps.append(
```

### Comparing `chellow-2826/chellow/reports/report_169.py` & `chellow-2827/chellow/reports/report_169.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/reports/report_177.py` & `chellow-2827/chellow/reports/report_177.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,14 @@
             month_start = start_date + relativedelta(months=i)
             month_finish = month_start + relativedelta(months=1) - HH
 
             for supply in supplies.filter(
                 Era.start_date <= month_finish,
                 or_(Era.finish_date == null(), Era.finish_date >= month_start),
             ):
-
                 generator_type = supply.generator_type
                 if generator_type is None:
                     generator_type = ""
                 else:
                     generator_type = generator_type.code
 
                 source_code = supply.source.code
```

### Comparing `chellow-2826/chellow/reports/report_181.py` & `chellow-2827/chellow/reports/report_181.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/reports/report_183.py` & `chellow-2827/chellow/reports/report_183.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/reports/report_187.py` & `chellow-2827/chellow/reports/report_187.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/reports/report_215.py` & `chellow-2827/chellow/reports/report_215.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/reports/report_219.py` & `chellow-2827/chellow/reports/report_219.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,14 @@
                         and_(
                             RegisterRead.previous_date >= start_date,
                             RegisterRead.previous_date <= finish_date,
                         ),
                     ),
                 )
             ):
-
                 era = supply.find_era_at(sess, bill.start_date)
                 if era is None:
                     eras = (
                         sess.query(Era)
                         .filter(Era.supply == supply)
                         .order_by(Era.start_date)
                         .all()
@@ -129,15 +128,14 @@
                     )
                     .options(
                         joinedload(RegisterRead.tpr),
                         joinedload(RegisterRead.previous_type),
                         joinedload(RegisterRead.present_type),
                     )
                 ):
-
                     vals = [
                         start_date,
                         finish_date,
                         supply_id,
                         era.imp_mpan_core,
                         era.exp_mpan_core,
                         batch.reference,
```

### Comparing `chellow-2826/chellow/reports/report_231.py` & `chellow-2827/chellow/reports/report_231.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/reports/report_233.py` & `chellow-2827/chellow/reports/report_233.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,14 @@
                 Channel.imp_related,
                 Channel.channel_type,
                 Snag.description,
                 Snag.start_date,
                 Snag.id,
             )
         ):
-
             snag_start = snag.start_date
             snag_finish = snag.finish_date
             imp_mc = "" if era.imp_mpan_core is None else era.imp_mpan_core
             exp_mc = "" if era.exp_mpan_core is None else era.exp_mpan_core
 
             if snag_finish is None:
                 duration = now - snag_start
```

### Comparing `chellow-2826/chellow/reports/report_241.py` & `chellow-2827/chellow/reports/report_241.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,14 @@
         bill_titles = []
         # Find titles
         for era in sess.query(Era).filter(
             Era.supply == supply,
             Era.start_date <= finish_date,
             or_(Era.finish_date == null(), Era.finish_date >= start_date),
         ):
-
             if is_import:
                 cont = era.imp_supplier_contract
             else:
                 cont = era.exp_supplier_contract
 
             for title in chellow.computer.contract_func(
                 caches, cont, "virtual_bill_titles"
```

### Comparing `chellow-2826/chellow/reports/report_247.py` & `chellow-2827/chellow/reports/report_247.py`

 * *Files 0% similar despite different names*

```diff
@@ -1029,15 +1029,14 @@
             sess.close()
         if rf is not None:
             rf.close()
             os.rename(running_name, finished_name)
 
 
 def do_post(sess):
-
     base_name = []
     now = utc_datetime_now()
 
     if "scenario_id" in request.values:
         scenario_id = req_int("scenario_id")
         scenario = Scenario.get_by_id(sess, scenario_id)
         scenario_props = scenario.props
```

### Comparing `chellow-2826/chellow/reports/report_29.py` & `chellow-2827/chellow/reports/report_29.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/reports/report_291.py` & `chellow-2827/chellow/reports/report_291.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
             .filter(
                 Era.supply == supply,
                 Era.start_date < finish_date,
                 or_(Era.finish_date == null(), Era.finish_date > start_date),
             )
             .order_by(Era.start_date)
         ):
-
             chunk_start = hh_max(era.start_date, start_date)
             chunk_finish = hh_min(era.finish_date, finish_date)
             site = (
                 sess.query(Site)
                 .join(SiteEra)
                 .filter(SiteEra.era == era, SiteEra.is_physical == true())
                 .one()
```

### Comparing `chellow-2826/chellow/reports/report_33.py` & `chellow-2827/chellow/reports/report_33.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/reports/report_387.py` & `chellow-2827/chellow/reports/report_387.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
         for era in sess.execute(
             select(Era).where(
                 Era.supply == supply,
                 Era.start_date <= finish_date,
                 or_(Era.finish_date == null(), Era.finish_date >= start_date),
             )
         ).scalars():
-
             ds = SupplySource(
                 sess, era.start_date, era.start_date, f_date, era, True, caches
             )
 
             for t in ds.contract_func(era.mop_contract, "virtual_bill_titles")():
                 if t not in mop_titles:
                     mop_titles.append(t)
```

### Comparing `chellow-2826/chellow/reports/report_41.py` & `chellow-2827/chellow/reports/report_41.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/reports/report_429.py` & `chellow-2827/chellow/reports/report_429.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,14 @@
     g_bill_ids,
     forecast_date,
     bill_titles,
     vbf,
     titles,
     csv_writer,
 ):
-
     g_bill_id = list(sorted(g_bill_ids))[0]
     g_bill_ids.remove(g_bill_id)
     g_bill = sess.query(GBill).filter(GBill.id == g_bill_id).one()
     problem = ""
     g_supply = g_bill.g_supply
     read_dict = defaultdict(set)
     for g_read in g_bill.g_reads:
```

### Comparing `chellow-2826/chellow/reports/report_59.py` & `chellow-2827/chellow/reports/report_59.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,14 @@
             "used-3rd-party",
             "billed-import-net",
         ):
             for xname in ("kwh", "gbp"):
                 vals[f"{sname}-{xname}"] = 0
 
         if imp_mpan_core == "displaced":
-
             vals["billed-supplier-import-net-gbp"] = None
             vals["billed-dc-import-net-gbp"] = None
             vals["billed-mop-import-net-gbp"] = None
 
             vals["used-kwh"] = vals["displaced-kwh"] = sum(
                 hh["msp-kwh"] for hh in imp_ss.hh_data
             )
@@ -1001,20 +1000,18 @@
             sess.close()
         if rf is not None:
             rf.close()
             os.rename(running_name, finished_name)
 
 
 def do_post(sess):
-
     base_name = ["duration"]
     compression = req_bool("compression")
 
     try:
-
         if "scenario_id" in request.values:
             scenario_id = req_int("scenario_id")
             scenario = Scenario.get_by_id(sess, scenario_id)
             props = scenario.props
             base_name.append(scenario.name)
 
         else:
```

### Comparing `chellow-2826/chellow/reports/report_81.py` & `chellow-2827/chellow/reports/report_81.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,14 @@
                 or_(Era.finish_date == null(), Era.finish_date >= start_date),
                 Era.start_date <= finish_date,
                 Era.dc_contract == contract,
             )
             .options(joinedload(Era.channels))
             .order_by(Era.supply_id)
         ):
-
             imp_mpan_core = era.imp_mpan_core
             if imp_mpan_core is None:
                 imp_mpan_core_str = ""
                 is_import = False
             else:
                 is_import = True
                 imp_mpan_core_str = imp_mpan_core
```

### Comparing `chellow-2826/chellow/reports/report_87.py` & `chellow-2827/chellow/reports/report_87.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/reports/report_asset_comparison.py` & `chellow-2827/chellow/reports/report_asset_comparison.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
     "UNDER CONSTRUCTION",
     "EMERGENCY",
     "",
 )
 
 
 def _process_sites(sess, file_like, writer, props, report_run):
-
     ASSET_KEY = "asset_comparison"
     try:
         asset_props = props[ASSET_KEY]
     except KeyError:
         raise BadRequest(
             f"The property {ASSET_KEY} cannot be found in the configuration properties."
         )
```

### Comparing `chellow-2826/chellow/reports/report_batches.py` & `chellow-2827/chellow/reports/report_batches.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,14 @@
             "max_finish_date",
         )
         writer.writerow(titles)
 
         for batch in sess.execute(
             select(Batch).order_by(Batch.contract_id, Batch.reference)
         ).scalars():
-
             (
                 num_bills,
                 sum_net_gbp,
                 sum_vat_gbp,
                 sum_gross_gbp,
                 sum_kwh,
                 min_start_date,
@@ -90,15 +89,14 @@
 
             # Avoid a long-running transaction
             sess.rollback()
 
         for g_batch in sess.execute(
             select(GBatch).order_by(GBatch.g_contract_id, GBatch.reference)
         ).scalars():
-
             (
                 num_bills,
                 sum_net_gbp,
                 sum_vat_gbp,
                 sum_gross_gbp,
                 sum_kwh,
                 min_start_date,
```

### Comparing `chellow-2826/chellow/reports/report_csv_llfcs.py` & `chellow-2827/chellow/reports/report_csv_llfcs.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/reports/report_csv_site_hh_data.py` & `chellow-2827/chellow/reports/report_csv_site_hh_data.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/reports/report_csv_site_snags.py` & `chellow-2827/chellow/reports/report_csv_site_snags.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/reports/report_ecoes_comparison.py` & `chellow-2827/chellow/reports/report_ecoes_comparison.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/reports/report_g_monthly_duration.py` & `chellow-2827/chellow/reports/report_g_monthly_duration.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,14 @@
                     .options(
                         joinedload(GEra.g_contract),
                         joinedload(GEra.g_supply),
                         joinedload(GEra.g_supply).joinedload(GSupply.g_exit_zone),
                     )
                     .order_by(GEra.id)
                 ):
-
                     g_supply = g_era.g_supply
 
                     if g_supply_id is not None and g_supply.id != g_supply_id:
                         continue
 
                     ss_start = hh_max(g_era.start_date, month_start)
                     ss_finish = hh_min(g_era.finish_date, month_finish)
```

### Comparing `chellow-2826/chellow/reports/report_g_supplies_snapshot.py` & `chellow-2827/chellow/reports/report_g_supplies_snapshot.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/reports/report_g_supply_virtual_bill.py` & `chellow-2827/chellow/reports/report_g_supply_virtual_bill.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,14 @@
             .filter(
                 GEra.g_supply == g_supply,
                 GEra.start_date < finish_date,
                 or_(GEra.finish_date == null(), GEra.finish_date > start_date),
             )
             .order_by(GEra.start_date)
         ):
-
             chunk_start = hh_max(g_era.start_date, start_date)
             chunk_finish = hh_min(g_era.finish_date, finish_date)
             site = (
                 sess.query(Site)
                 .join(SiteGEra)
                 .filter(SiteGEra.g_era == g_era, SiteGEra.is_physical == true())
                 .one()
```

### Comparing `chellow-2826/chellow/reports/report_g_virtual_bills.py` & `chellow-2827/chellow/reports/report_g_virtual_bills.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,14 @@
                 .distinct()
                 .filter(
                     GEra.g_contract == g_contract,
                     GEra.start_date <= period_finish,
                     or_(GEra.finish_date == null(), GEra.finish_date >= period_start),
                 )
             ):
-
                 chunk_start = hh_max(g_era.start_date, period_start)
                 chunk_finish = hh_min(g_era.finish_date, period_finish)
 
                 data_source = GDataSource(
                     sess,
                     chunk_start,
                     chunk_finish,
```

### Comparing `chellow-2826/chellow/reports/report_g_virtual_bills_hh.py` & `chellow-2827/chellow/reports/report_g_virtual_bills_hh.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/reports/report_laf_parser.py` & `chellow-2827/chellow/reports/report_laf_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,14 @@
             raise Exception("The zip archive must contain exactly one file.")
         csv_file = StringIO(zip_file.read(name_list[0]).decode("utf-8"))
         for vals in csv.reader(csv_file, delimiter="|"):
             code = vals[0]
 
             if code in ("LLF", "ZPT"):
                 if llfc_code is not None:
-
                     # Compress days
                     days = OrderedDict()
                     for dt, slots in llfc_data.items():
                         day = days[dt] = []
                         prev_laf = None
                         for slot, laf in slots.items():
                             if laf == prev_laf:
```

### Comparing `chellow-2826/chellow/reports/report_supply_contacts.py` & `chellow-2827/chellow/reports/report_supply_contacts.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,14 @@
                 joinedload(Era.imp_supplier_contract),
                 joinedload(Era.mop_contract),
             )
         )
         .scalars()
         .unique()
     ):
-
         for site_era in era.site_eras:
             if site_era.is_physical:
                 site = site_era.site
 
         dno = era.supply.dno
 
         imp_supplier_contract = era.imp_supplier_contract
```

### Comparing `chellow-2826/chellow/static/css/chellow.css` & `chellow-2827/chellow/static/css/chellow.css`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/static/images/favicon.svg` & `chellow-2827/chellow/static/images/favicon.svg`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/static/images/favicon_test.svg` & `chellow-2827/chellow/static/images/favicon_test.svg`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/static/images/logo.png` & `chellow-2827/chellow/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/static/js/htmx.min.js` & `chellow-2827/chellow/static/js/htmx.min.js`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/base.html` & `chellow-2827/chellow/templates/base.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/chain.html` & `chellow-2827/chellow/templates/chain.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/downloads.html` & `chellow-2827/chellow/templates/downloads.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/asset_comparison.html` & `chellow-2827/chellow/templates/e/asset_comparison.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/channel.html` & `chellow-2827/chellow/templates/e/channel.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/channel_add.html` & `chellow-2827/chellow/templates/e/channel_add.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/channel_edit.html` & `chellow-2827/chellow/templates/e/channel_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/channel_snag.html` & `chellow-2827/chellow/templates/e/channel_snag.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/channel_snag_edit.html` & `chellow-2827/chellow/templates/e/channel_snag_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/channel_snags.html` & `chellow-2827/chellow/templates/e/channel_snags.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/csv_register_reads.html` & `chellow-2827/chellow/templates/e/csv_register_reads.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/csv_sites_hh_data.html` & `chellow-2827/chellow/templates/e/csv_sites_hh_data.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/csv_supplies_hh_data.html` & `chellow-2827/chellow/templates/e/csv_supplies_hh_data.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/csv_supplies_snapshot.html` & `chellow-2827/chellow/templates/e/csv_supplies_snapshot.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/dc_auto_importer.html` & `chellow-2827/chellow/templates/e/dc_auto_importer.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/dc_batch.html` & `chellow-2827/chellow/templates/e/dc_batch.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/dc_batch_add.html` & `chellow-2827/chellow/templates/e/dc_batch_add.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/dc_batch_edit.html` & `chellow-2827/chellow/templates/e/dc_batch_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/dc_batch_file.html` & `chellow-2827/chellow/templates/e/dc_batch_file.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/dc_batch_file_edit.html` & `chellow-2827/chellow/templates/e/dc_batch_file_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/dc_batch_upload_file.html` & `chellow-2827/chellow/templates/e/dc_batch_upload_file.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/dc_batches.html` & `chellow-2827/chellow/templates/e/dc_batches.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/dc_bill.html` & `chellow-2827/chellow/templates/e/dc_bill.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/dc_bill_add.html` & `chellow-2827/chellow/templates/e/dc_bill_add.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/dc_bill_edit.html` & `chellow-2827/chellow/templates/e/dc_bill_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/dc_bill_import.html` & `chellow-2827/chellow/templates/e/dc_bill_import.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/dc_bill_imports.html` & `chellow-2827/chellow/templates/e/dc_bill_imports.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/dc_contract.html` & `chellow-2827/chellow/templates/e/dc_contract.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/dc_contract_edit.html` & `chellow-2827/chellow/templates/e/dc_contract_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/dc_contract_hh_import.html` & `chellow-2827/chellow/templates/e/dc_contract_hh_import.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/dc_contract_hh_imports.html` & `chellow-2827/chellow/templates/e/dc_contract_hh_imports.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/dc_contracts.html` & `chellow-2827/chellow/templates/e/dc_contracts.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/dc_contracts_add.html` & `chellow-2827/chellow/templates/e/dc_contracts_add.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/dc_rate_script.html` & `chellow-2827/chellow/templates/e/dc_rate_script.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/dc_rate_script_add.html` & `chellow-2827/chellow/templates/e/dc_rate_script_add.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/dc_rate_script_edit.html` & `chellow-2827/chellow/templates/e/dc_rate_script_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/dno.html` & `chellow-2827/chellow/templates/e/dno.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/dno_rate_script.html` & `chellow-2827/chellow/templates/e/dno_rate_script.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/dno_rate_script_add.html` & `chellow-2827/chellow/templates/e/dno_rate_script_add.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/dno_rate_script_edit.html` & `chellow-2827/chellow/templates/e/dno_rate_script_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/dnos.html` & `chellow-2827/chellow/templates/e/dnos.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/duration_report.html` & `chellow-2827/chellow/templates/e/duration_report.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/em_hh_data.html` & `chellow-2827/chellow/templates/e/em_hh_data.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/em_months.html` & `chellow-2827/chellow/templates/e/em_months.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/em_site.html` & `chellow-2827/chellow/templates/e/em_site.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/em_totals.html` & `chellow-2827/chellow/templates/e/em_totals.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/energisation_statuses.html` & `chellow-2827/chellow/templates/e/energisation_statuses.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/era_edit.html` & `chellow-2827/chellow/templates/e/era_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/era_supplier_bill_add.html` & `chellow-2827/chellow/templates/e/era_supplier_bill_add.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/generator_types.html` & `chellow-2827/chellow/templates/e/generator_types.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/hh_datum_edit.html` & `chellow-2827/chellow/templates/e/hh_datum_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/lafs.html` & `chellow-2827/chellow/templates/e/lafs.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/llfc.html` & `chellow-2827/chellow/templates/e/llfc.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/llfc_edit.html` & `chellow-2827/chellow/templates/e/llfc_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/llfcs.html` & `chellow-2827/chellow/templates/e/llfcs.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/market_role.html` & `chellow-2827/chellow/templates/e/market_role.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/meter_payment_type.html` & `chellow-2827/chellow/templates/e/meter_payment_type.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/meter_payment_types.html` & `chellow-2827/chellow/templates/e/meter_payment_types.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/meter_type.html` & `chellow-2827/chellow/templates/e/meter_type.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/meter_types.html` & `chellow-2827/chellow/templates/e/meter_types.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/mop_batch.html` & `chellow-2827/chellow/templates/e/mop_batch.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/mop_batch_add.html` & `chellow-2827/chellow/templates/e/mop_batch_add.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/mop_batch_edit.html` & `chellow-2827/chellow/templates/e/mop_batch_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/mop_batch_file.html` & `chellow-2827/chellow/templates/e/mop_batch_file.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/mop_batch_file_edit.html` & `chellow-2827/chellow/templates/e/mop_batch_file_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/mop_batch_upload_file.html` & `chellow-2827/chellow/templates/e/mop_batch_upload_file.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/mop_batches.html` & `chellow-2827/chellow/templates/e/mop_batches.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/mop_bill.html` & `chellow-2827/chellow/templates/e/mop_bill.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/mop_bill_add.html` & `chellow-2827/chellow/templates/e/mop_bill_add.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/mop_bill_edit.html` & `chellow-2827/chellow/templates/e/mop_bill_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/mop_bill_import.html` & `chellow-2827/chellow/templates/e/mop_bill_import.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/mop_bill_imports.html` & `chellow-2827/chellow/templates/e/mop_bill_imports.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/mop_contract.html` & `chellow-2827/chellow/templates/e/mop_contract.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/mop_contract_add.html` & `chellow-2827/chellow/templates/e/mop_contract_add.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/mop_contract_edit.html` & `chellow-2827/chellow/templates/e/mop_contract_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/mop_contracts.html` & `chellow-2827/chellow/templates/e/mop_contracts.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/mop_rate_script.html` & `chellow-2827/chellow/templates/e/mop_rate_script.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/mop_rate_script_add.html` & `chellow-2827/chellow/templates/e/mop_rate_script_add.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/mop_rate_script_edit.html` & `chellow-2827/chellow/templates/e/mop_rate_script_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/mtc.html` & `chellow-2827/chellow/templates/e/mtc.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/mtc_llfc.html` & `chellow-2827/chellow/templates/e/mtc_llfc.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/mtc_llfc_ssc.html` & `chellow-2827/chellow/templates/e/mtc_llfc_ssc.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/mtc_llfc_ssc_pc.html` & `chellow-2827/chellow/templates/e/mtc_llfc_ssc_pc.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/mtc_llfc_ssc_pcs.html` & `chellow-2827/chellow/templates/e/mtc_llfc_ssc_pcs.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/mtc_llfc_sscs.html` & `chellow-2827/chellow/templates/e/mtc_llfc_sscs.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/mtc_llfcs.html` & `chellow-2827/chellow/templates/e/mtc_llfcs.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/mtc_participant.html` & `chellow-2827/chellow/templates/e/mtc_participant.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/mtc_participants.html` & `chellow-2827/chellow/templates/e/mtc_participants.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/mtc_ssc.html` & `chellow-2827/chellow/templates/e/mtc_ssc.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/mtc_sscs.html` & `chellow-2827/chellow/templates/e/mtc_sscs.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/mtcs.html` & `chellow-2827/chellow/templates/e/mtcs.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/ods_monthly_duration.html` & `chellow-2827/chellow/templates/e/ods_monthly_duration.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/participant.html` & `chellow-2827/chellow/templates/e/participant.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/parties.html` & `chellow-2827/chellow/templates/e/parties.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/party.html` & `chellow-2827/chellow/templates/e/party.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/pc.html` & `chellow-2827/chellow/templates/e/pc.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/pcs.html` & `chellow-2827/chellow/templates/e/pcs.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/read_add.html` & `chellow-2827/chellow/templates/e/read_add.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/read_edit.html` & `chellow-2827/chellow/templates/e/read_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/scenario.html` & `chellow-2827/chellow/templates/e/scenario.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/scenario_add.html` & `chellow-2827/chellow/templates/e/scenario_add.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/scenario_docs.html` & `chellow-2827/chellow/templates/e/scenario_docs.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/scenario_edit.html` & `chellow-2827/chellow/templates/e/scenario_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/scenarios.html` & `chellow-2827/chellow/templates/e/scenarios.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/site_hh_data.html` & `chellow-2827/chellow/templates/e/site_hh_data.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/site_site_snags.html` & `chellow-2827/chellow/templates/e/site_site_snags.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/site_snag.html` & `chellow-2827/chellow/templates/e/site_snag.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/site_snag_edit.html` & `chellow-2827/chellow/templates/e/site_snag_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/site_snags.html` & `chellow-2827/chellow/templates/e/site_snags.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/ssc.html` & `chellow-2827/chellow/templates/e/ssc.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/sscs.html` & `chellow-2827/chellow/templates/e/sscs.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/supplier_batch.html` & `chellow-2827/chellow/templates/e/supplier_batch.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/supplier_batch_add.html` & `chellow-2827/chellow/templates/e/supplier_batch_add.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/supplier_batch_edit.html` & `chellow-2827/chellow/templates/e/supplier_batch_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/supplier_batch_file.html` & `chellow-2827/chellow/templates/e/supplier_batch_file.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/supplier_batch_file_add.html` & `chellow-2827/chellow/templates/e/supplier_batch_file_add.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/supplier_batch_file_edit.html` & `chellow-2827/chellow/templates/e/supplier_batch_file_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/supplier_batch_upload_file.html` & `chellow-2827/chellow/templates/e/supplier_batch_upload_file.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/supplier_batches.html` & `chellow-2827/chellow/templates/e/supplier_batches.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/supplier_bill.html` & `chellow-2827/chellow/templates/e/supplier_bill.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/supplier_bill_add.html` & `chellow-2827/chellow/templates/e/supplier_bill_add.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/supplier_bill_edit.html` & `chellow-2827/chellow/templates/e/supplier_bill_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/supplier_bill_import.html` & `chellow-2827/chellow/templates/e/supplier_bill_import.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/supplier_bill_imports.html` & `chellow-2827/chellow/templates/e/supplier_bill_imports.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/supplier_contract.html` & `chellow-2827/chellow/templates/e/supplier_contract.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/supplier_contract_add.html` & `chellow-2827/chellow/templates/e/supplier_contract_add.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/supplier_contract_edit.html` & `chellow-2827/chellow/templates/e/supplier_contract_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/supplier_contracts.html` & `chellow-2827/chellow/templates/e/supplier_contracts.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/supplier_rate_script.html` & `chellow-2827/chellow/templates/e/supplier_rate_script.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/supplier_rate_script_add.html` & `chellow-2827/chellow/templates/e/supplier_rate_script_add.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/supplier_rate_script_edit.html` & `chellow-2827/chellow/templates/e/supplier_rate_script_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/supply.html` & `chellow-2827/chellow/templates/e/supply.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/supply_edit.html` & `chellow-2827/chellow/templates/e/supply_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/supply_hh_data.html` & `chellow-2827/chellow/templates/e/supply_hh_data.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/supply_months.html` & `chellow-2827/chellow/templates/e/supply_months.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/supply_note_add.html` & `chellow-2827/chellow/templates/e/supply_note_add.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/supply_note_edit.html` & `chellow-2827/chellow/templates/e/supply_note_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/supply_notes.html` & `chellow-2827/chellow/templates/e/supply_notes.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/supply_virtual_bill.html` & `chellow-2827/chellow/templates/e/supply_virtual_bill.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/e/tpr.html` & `chellow-2827/chellow/templates/e/tpr.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/edi_viewer.html` & `chellow-2827/chellow/templates/edi_viewer.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/g/batch.html` & `chellow-2827/chellow/templates/g/batch.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/g/batch_add.html` & `chellow-2827/chellow/templates/g/batch_add.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/g/batch_edit.html` & `chellow-2827/chellow/templates/g/batch_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/g/batches.html` & `chellow-2827/chellow/templates/g/batches.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/g/bill.html` & `chellow-2827/chellow/templates/g/bill.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/g/bill_add.html` & `chellow-2827/chellow/templates/g/bill_add.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/g/bill_edit.html` & `chellow-2827/chellow/templates/g/bill_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/g/bill_import.html` & `chellow-2827/chellow/templates/g/bill_import.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/g/bill_imports.html` & `chellow-2827/chellow/templates/g/bill_imports.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/g/era_edit.html` & `chellow-2827/chellow/templates/g/era_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/g/exit_zone.html` & `chellow-2827/chellow/templates/g/exit_zone.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/g/industry_auto_importer.html` & `chellow-2827/chellow/templates/g/industry_auto_importer.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/g/industry_contract.html` & `chellow-2827/chellow/templates/g/industry_contract.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/g/industry_contract_add.html` & `chellow-2827/chellow/templates/g/industry_contract_add.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/g/industry_contract_edit.html` & `chellow-2827/chellow/templates/g/industry_contract_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/g/industry_contracts.html` & `chellow-2827/chellow/templates/g/industry_contracts.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/g/industry_rate_script.html` & `chellow-2827/chellow/templates/g/industry_rate_script.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/g/industry_rate_script_add.html` & `chellow-2827/chellow/templates/g/industry_rate_script_add.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/g/industry_rate_script_edit.html` & `chellow-2827/chellow/templates/g/industry_rate_script_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/g/ldz.html` & `chellow-2827/chellow/templates/g/ldz.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/g/read_add.html` & `chellow-2827/chellow/templates/g/read_add.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/g/read_edit.html` & `chellow-2827/chellow/templates/g/read_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/g/reading_frequencies.html` & `chellow-2827/chellow/templates/g/reading_frequencies.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/g/reports.html` & `chellow-2827/chellow/templates/g/reports.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/g/supplier_contract.html` & `chellow-2827/chellow/templates/g/supplier_contract.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/g/supplier_contract_add.html` & `chellow-2827/chellow/templates/g/supplier_contract_add.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/g/supplier_contract_edit.html` & `chellow-2827/chellow/templates/g/supplier_contract_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/g/supplier_contracts.html` & `chellow-2827/chellow/templates/g/supplier_contracts.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/g/supplier_rate_script.html` & `chellow-2827/chellow/templates/g/supplier_rate_script.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/g/supplier_rate_script_add.html` & `chellow-2827/chellow/templates/g/supplier_rate_script_add.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/g/supplier_rate_script_edit.html` & `chellow-2827/chellow/templates/g/supplier_rate_script_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/g/supplies.html` & `chellow-2827/chellow/templates/g/supplies.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/g/supply.html` & `chellow-2827/chellow/templates/g/supply.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/g/supply_edit.html` & `chellow-2827/chellow/templates/g/supply_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/g/supply_note_add.html` & `chellow-2827/chellow/templates/g/supply_note_add.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/g/supply_note_edit.html` & `chellow-2827/chellow/templates/g/supply_note_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/g/supply_notes.html` & `chellow-2827/chellow/templates/g/supply_notes.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/general_import.html` & `chellow-2827/chellow/templates/general_import.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/general_imports.html` & `chellow-2827/chellow/templates/general_imports.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/home.html` & `chellow-2827/chellow/templates/home.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/local_report.html` & `chellow-2827/chellow/templates/local_report.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/local_reports.html` & `chellow-2827/chellow/templates/local_reports.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/non_core_auto_importer.html` & `chellow-2827/chellow/templates/non_core_auto_importer.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/non_core_contract.html` & `chellow-2827/chellow/templates/non_core_contract.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/non_core_contract_edit.html` & `chellow-2827/chellow/templates/non_core_contract_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/non_core_contracts.html` & `chellow-2827/chellow/templates/non_core_contracts.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/non_core_rate_script.html` & `chellow-2827/chellow/templates/non_core_rate_script.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/non_core_rate_script_add.html` & `chellow-2827/chellow/templates/non_core_rate_script_add.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/non_core_rate_script_edit.html` & `chellow-2827/chellow/templates/non_core_rate_script_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/rate_server.html` & `chellow-2827/chellow/templates/rate_server.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/report_run.html` & `chellow-2827/chellow/templates/report_run.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/report_run_asset_comparison.html` & `chellow-2827/chellow/templates/report_run_asset_comparison.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/report_run_bill_check.html` & `chellow-2827/chellow/templates/report_run_bill_check.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/report_run_ecoes_comparison.html` & `chellow-2827/chellow/templates/report_run_ecoes_comparison.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/report_run_row.html` & `chellow-2827/chellow/templates/report_run_row.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/report_run_row_bill_check.html` & `chellow-2827/chellow/templates/report_run_row_bill_check.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/report_run_supply_contacts.html` & `chellow-2827/chellow/templates/report_run_supply_contacts.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/report_runs.html` & `chellow-2827/chellow/templates/report_runs.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/site.html` & `chellow-2827/chellow/templates/site.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/site_edit.html` & `chellow-2827/chellow/templates/site_edit.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/site_gen_graph.html` & `chellow-2827/chellow/templates/site_gen_graph.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/site_hh_data.html` & `chellow-2827/chellow/templates/site_hh_data.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/site_months.html` & `chellow-2827/chellow/templates/site_months.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/site_used_graph.html` & `chellow-2827/chellow/templates/site_used_graph.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/sites.html` & `chellow-2827/chellow/templates/sites.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/supplies.html` & `chellow-2827/chellow/templates/supplies.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/system.html` & `chellow-2827/chellow/templates/system.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/tester.html` & `chellow-2827/chellow/templates/tester.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/user.html` & `chellow-2827/chellow/templates/user.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/templates/users.html` & `chellow-2827/chellow/templates/users.html`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/testing.py` & `chellow-2827/chellow/testing.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/chellow/utils.py` & `chellow-2827/chellow/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -526,15 +526,14 @@
 def ct_datetime_parse(date_str, format_str):
     return to_ct(Datetime.strptime(date_str, format_str))
 
 
 def u_months_u(
     start_year=None, start_month=None, finish_year=None, finish_month=None, months=1
 ):
-
     if start_year is None:
         start = utc_datetime(finish_year, finish_month) - relativedelta(
             months=months - 1
         )
     else:
         start = utc_datetime(start_year, start_month)
 
@@ -551,29 +550,27 @@
         yield dt, dt + MONTH - HH
         dt += MONTH
 
 
 def c_months_u(
     start_year=None, start_month=None, finish_year=None, finish_month=None, months=1
 ):
-
     for c_m_start_c, c_m_finish_c in c_months_c(
         start_year=start_year,
         start_month=start_month,
         finish_year=finish_year,
         finish_month=finish_month,
         months=months,
     ):
         yield to_utc(c_m_start_c), to_utc(c_m_finish_c)
 
 
 def c_months_c(
     start_year=None, start_month=None, finish_year=None, finish_month=None, months=1
 ):
-
     for u_m_start_u, u_m_finish_u in u_months_u(
         start_year=start_year,
         start_month=start_month,
         finish_year=finish_year,
         finish_month=finish_month,
         months=months,
     ):
```

### Comparing `chellow-2826/chellow/views.py` & `chellow-2827/chellow/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -1648,15 +1648,14 @@
             ) and t not in (
                 "covered-from",
                 "covered-to",
                 "covered-bills",
                 "covered-problem",
                 "virtual-problem",
             ):
-
                 toks = t.split("-")
                 name = toks[1]
                 try:
                     table = elements[name]
                 except KeyError:
                     table = elements[name] = {"order": 0}
 
@@ -1677,15 +1676,14 @@
 
         tables.sort(key=lambda t: t["order"], reverse=True)
         return render_template(
             "report_run_row_bill_check.html", row=row, raw_data=raw_data, tables=tables
         )
 
     else:
-
         return render_template(
             "report_run_row.html", row=row, raw_data=raw_data, tables=tables
         )
 
 
 @home.route("/report_run_rows/<int:row_id>", methods=["POST"])
 def report_run_row_post(row_id):
```

### Comparing `chellow-2826/chellow.egg-info/PKG-INFO` & `chellow-2827/chellow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chellow
-Version: 2826
+Version: 2827
 Summary: Web Application for checking UK utility bills.
 Home-page: https://github.com/WessexWater/chellow
 Author: Tony Locke
 Author-email: tlocke@tlocke.org.uk
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `chellow-2826/chellow.egg-info/SOURCES.txt` & `chellow-2827/chellow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chellow-2826/setup.cfg` & `chellow-2827/setup.cfg`

 * *Files identical despite different names*

### Comparing `chellow-2826/setup.py` & `chellow-2827/setup.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/test/test_chellow.py` & `chellow-2827/test/test_chellow.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/test/test_general_import.py` & `chellow-2827/test/test_general_import.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/test/test_models.py` & `chellow-2827/test/test_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -716,15 +716,14 @@
 
 def test_Supply_get_by_MPAN_core(sess):
     mpan_core = "22 1737 1873 221"
 
     with pytest.raises(
         BadRequest, match=f"The MPAN core {mpan_core} is not set up in Chellow."
     ):
-
         Supply.get_by_mpan_core(sess, mpan_core)
 
 
 def test_Supply_insert_era_at(sess):
     """Where an era is inserted in the last HH of another era, check
     the template era is the one at the insertion date.
     """
```

### Comparing `chellow-2826/test/test_testing.py` & `chellow-2827/test/test_testing.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/test/test_utils.py` & `chellow-2827/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/test/test_views.py` & `chellow-2827/test/test_views.py`

 * *Files identical despite different names*

### Comparing `chellow-2826/versioneer.py` & `chellow-2827/versioneer.py`

 * *Files identical despite different names*

