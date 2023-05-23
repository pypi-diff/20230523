# Comparing `tmp/mia-accounting-1.5.5.tar.gz` & `tmp/mia-accounting-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mia-accounting-1.5.5.tar", last modified: Tue May 23 00:45:05 2023, max compression
+gzip compressed data, was "mia-accounting-1.5.6.tar", last modified: Tue May 23 01:08:21 2023, max compression
```

## Comparing `mia-accounting-1.5.5.tar` & `mia-accounting-1.5.6.tar`

### file list

```diff
@@ -1,305 +1,305 @@
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.649698 mia-accounting-1.5.5/
--rw-r--r--   0 imacat    (1000) users      (100)    11358 2015-02-17 18:06:12.000000 mia-accounting-1.5.5/LICENSE
--rw-r--r--   0 imacat    (1000) users      (100)     1070 2023-04-05 11:25:31.000000 mia-accounting-1.5.5/MANIFEST.in
--rw-r--r--   0 imacat    (1000) users      (100)     3412 2023-05-23 00:45:05.649698 mia-accounting-1.5.5/PKG-INFO
--rw-r--r--   0 imacat    (1000) users      (100)     2525 2023-04-23 12:04:20.000000 mia-accounting-1.5.5/README.rst
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.601698 mia-accounting-1.5.5/docs/
--rw-r--r--   0 imacat    (1000) users      (100)      638 2023-01-27 04:20:04.000000 mia-accounting-1.5.5/docs/Makefile
--rw-r--r--   0 imacat    (1000) users      (100)      804 2023-01-27 04:20:04.000000 mia-accounting-1.5.5/docs/make.bat
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.609698 mia-accounting-1.5.5/docs/source/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.609698 mia-accounting-1.5.5/docs/source/_static/
--rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:08.000000 mia-accounting-1.5.5/docs/source/_static/.keep
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.609698 mia-accounting-1.5.5/docs/source/_templates/
--rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:11.000000 mia-accounting-1.5.5/docs/source/_templates/.keep
--rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-05-23 00:37:49.000000 mia-accounting-1.5.5/docs/source/accounting.account.rst
--rw-r--r--   0 imacat    (1000) users      (100)      959 2023-05-23 00:37:49.000000 mia-accounting-1.5.5/docs/source/accounting.base_account.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1053 2023-05-23 00:37:49.000000 mia-accounting-1.5.5/docs/source/accounting.currency.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1089 2023-05-23 00:37:49.000000 mia-accounting-1.5.5/docs/source/accounting.journal_entry.forms.rst
--rw-r--r--   0 imacat    (1000) users      (100)      937 2023-05-23 00:37:49.000000 mia-accounting-1.5.5/docs/source/accounting.journal_entry.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1162 2023-05-23 00:37:49.000000 mia-accounting-1.5.5/docs/source/accounting.journal_entry.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)      513 2023-05-23 00:37:49.000000 mia-accounting-1.5.5/docs/source/accounting.option.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1551 2023-05-23 00:37:49.000000 mia-accounting-1.5.5/docs/source/accounting.report.period.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2460 2023-05-23 00:37:49.000000 mia-accounting-1.5.5/docs/source/accounting.report.reports.rst
--rw-r--r--   0 imacat    (1000) users      (100)      861 2023-05-23 00:37:49.000000 mia-accounting-1.5.5/docs/source/accounting.report.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2168 2023-05-23 00:37:49.000000 mia-accounting-1.5.5/docs/source/accounting.report.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1301 2023-05-23 00:37:49.000000 mia-accounting-1.5.5/docs/source/accounting.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2405 2023-05-23 00:37:49.000000 mia-accounting-1.5.5/docs/source/accounting.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)     8334 2023-05-23 00:42:24.000000 mia-accounting-1.5.5/docs/source/changelog.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1051 2023-04-23 12:12:53.000000 mia-accounting-1.5.5/docs/source/conf.py
--rw-r--r--   0 imacat    (1000) users      (100)     1508 2023-04-06 00:38:39.000000 mia-accounting-1.5.5/docs/source/examples.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2837 2023-04-06 00:21:32.000000 mia-accounting-1.5.5/docs/source/history.rst
--rw-r--r--   0 imacat    (1000) users      (100)      521 2023-04-23 12:04:21.000000 mia-accounting-1.5.5/docs/source/index.rst
--rw-r--r--   0 imacat    (1000) users      (100)     3568 2023-05-06 15:58:29.000000 mia-accounting-1.5.5/docs/source/intro.rst
--rw-r--r--   0 imacat    (1000) users      (100)       53 2023-04-04 10:25:53.000000 mia-accounting-1.5.5/docs/source/modules.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1994 2023-05-09 00:42:23.000000 mia-accounting-1.5.5/pyproject.toml
--rw-r--r--   0 imacat    (1000) users      (100)       38 2023-05-23 00:45:05.649698 mia-accounting-1.5.5/setup.cfg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.597699 mia-accounting-1.5.5/src/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.613698 mia-accounting-1.5.5/src/accounting/
--rw-r--r--   0 imacat    (1000) users      (100)     3045 2023-05-23 00:43:07.000000 mia-accounting-1.5.5/src/accounting/__init__.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.613698 mia-accounting-1.5.5/src/accounting/account/
--rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-10 15:59:48.000000 mia-accounting-1.5.5/src/accounting/account/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3868 2023-04-29 21:45:45.000000 mia-accounting-1.5.5/src/accounting/account/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1512 2023-04-04 09:21:35.000000 mia-accounting-1.5.5/src/accounting/account/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     7145 2023-04-04 09:21:33.000000 mia-accounting-1.5.5/src/accounting/account/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     2209 2023-04-04 09:21:35.000000 mia-accounting-1.5.5/src/accounting/account/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     7416 2023-04-09 02:08:22.000000 mia-accounting-1.5.5/src/accounting/account/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.613698 mia-accounting-1.5.5/src/accounting/base_account/
--rw-r--r--   0 imacat    (1000) users      (100)     1240 2023-04-10 15:59:48.000000 mia-accounting-1.5.5/src/accounting/base_account/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     1800 2023-04-10 15:59:48.000000 mia-accounting-1.5.5/src/accounting/base_account/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1592 2023-04-04 09:21:35.000000 mia-accounting-1.5.5/src/accounting/base_account/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     1769 2023-04-04 09:21:37.000000 mia-accounting-1.5.5/src/accounting/base_account/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     1812 2023-04-09 02:08:22.000000 mia-accounting-1.5.5/src/accounting/base_account/views.py
--rw-r--r--   0 imacat    (1000) users      (100)     2138 2023-04-10 15:59:48.000000 mia-accounting-1.5.5/src/accounting/commands.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.617698 mia-accounting-1.5.5/src/accounting/currency/
--rw-r--r--   0 imacat    (1000) users      (100)     1312 2023-04-10 15:59:48.000000 mia-accounting-1.5.5/src/accounting/currency/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     2206 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/currency/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1556 2023-04-04 09:21:35.000000 mia-accounting-1.5.5/src/accounting/currency/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     3172 2023-04-04 09:21:36.000000 mia-accounting-1.5.5/src/accounting/currency/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     1720 2023-04-04 09:21:34.000000 mia-accounting-1.5.5/src/accounting/currency/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     6609 2023-04-09 02:08:22.000000 mia-accounting-1.5.5/src/accounting/currency/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.617698 mia-accounting-1.5.5/src/accounting/data/
--rw-r--r--   0 imacat    (1000) users      (100)    36368 2023-03-14 01:04:26.000000 mia-accounting-1.5.5/src/accounting/data/base_accounts.csv
--rw-r--r--   0 imacat    (1000) users      (100)      370 2023-03-14 01:04:26.000000 mia-accounting-1.5.5/src/accounting/data/currencies.csv
--rw-r--r--   0 imacat    (1000) users      (100)     3144 2023-04-04 09:21:33.000000 mia-accounting-1.5.5/src/accounting/forms.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.617698 mia-accounting-1.5.5/src/accounting/journal_entry/
--rw-r--r--   0 imacat    (1000) users      (100)     1376 2023-04-04 09:21:35.000000 mia-accounting-1.5.5/src/accounting/journal_entry/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3302 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/journal_entry/converters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.617698 mia-accounting-1.5.5/src/accounting/journal_entry/forms/
--rw-r--r--   0 imacat    (1000) users      (100)      934 2023-04-04 09:21:37.000000 mia-accounting-1.5.5/src/accounting/journal_entry/forms/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)    11003 2023-04-23 05:21:41.000000 mia-accounting-1.5.5/src/accounting/journal_entry/forms/currency.py
--rw-r--r--   0 imacat    (1000) users      (100)    24568 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/journal_entry/forms/journal_entry.py
--rw-r--r--   0 imacat    (1000) users      (100)    19807 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/journal_entry/forms/line_item.py
--rw-r--r--   0 imacat    (1000) users      (100)     3291 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/journal_entry/forms/reorder.py
--rw-r--r--   0 imacat    (1000) users      (100)     2535 2023-04-04 09:21:32.000000 mia-accounting-1.5.5/src/accounting/journal_entry/template_filters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.621698 mia-accounting-1.5.5/src/accounting/journal_entry/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      729 2023-04-04 09:21:32.000000 mia-accounting-1.5.5/src/accounting/journal_entry/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     1802 2023-04-17 23:37:17.000000 mia-accounting-1.5.5/src/accounting/journal_entry/utils/account_option.py
--rw-r--r--   0 imacat    (1000) users      (100)    12981 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/journal_entry/utils/description_editor.py
--rw-r--r--   0 imacat    (1000) users      (100)    12676 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/journal_entry/utils/operators.py
--rw-r--r--   0 imacat    (1000) users      (100)     3722 2023-04-23 05:21:41.000000 mia-accounting-1.5.5/src/accounting/journal_entry/utils/original_line_items.py
--rw-r--r--   0 imacat    (1000) users      (100)     9351 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/journal_entry/views.py
--rw-r--r--   0 imacat    (1000) users      (100)     3809 2023-04-04 09:21:33.000000 mia-accounting-1.5.5/src/accounting/locale.py
--rw-r--r--   0 imacat    (1000) users      (100)    32618 2023-04-30 07:03:58.000000 mia-accounting-1.5.5/src/accounting/models.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.621698 mia-accounting-1.5.5/src/accounting/option/
--rw-r--r--   0 imacat    (1000) users      (100)      993 2023-04-04 09:21:35.000000 mia-accounting-1.5.5/src/accounting/option/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     9762 2023-04-08 00:27:23.000000 mia-accounting-1.5.5/src/accounting/option/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     2827 2023-04-04 09:21:32.000000 mia-accounting-1.5.5/src/accounting/option/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.621698 mia-accounting-1.5.5/src/accounting/report/
--rw-r--r--   0 imacat    (1000) users      (100)     1362 2023-04-08 10:12:56.000000 mia-accounting-1.5.5/src/accounting/report/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-08 10:12:56.000000 mia-accounting-1.5.5/src/accounting/report/converters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.621698 mia-accounting-1.5.5/src/accounting/report/period/
--rw-r--r--   0 imacat    (1000) users      (100)      793 2023-04-04 09:21:32.000000 mia-accounting-1.5.5/src/accounting/report/period/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3702 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/report/period/chooser.py
--rw-r--r--   0 imacat    (1000) users      (100)     5557 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/report/period/description.py
--rw-r--r--   0 imacat    (1000) users      (100)     1050 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/report/period/month_end.py
--rw-r--r--   0 imacat    (1000) users      (100)     4127 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/report/period/parser.py
--rw-r--r--   0 imacat    (1000) users      (100)     4522 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/report/period/period.py
--rw-r--r--   0 imacat    (1000) users      (100)     4785 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/report/period/shortcuts.py
--rw-r--r--   0 imacat    (1000) users      (100)     3915 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/report/period/specification.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.625698 mia-accounting-1.5.5/src/accounting/report/reports/
--rw-r--r--   0 imacat    (1000) users      (100)      946 2023-04-04 09:21:36.000000 mia-accounting-1.5.5/src/accounting/report/reports/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)    17920 2023-04-06 01:50:58.000000 mia-accounting-1.5.5/src/accounting/report/reports/balance_sheet.py
--rw-r--r--   0 imacat    (1000) users      (100)    18807 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/report/reports/income_expenses.py
--rw-r--r--   0 imacat    (1000) users      (100)    11733 2023-04-06 01:50:58.000000 mia-accounting-1.5.5/src/accounting/report/reports/income_statement.py
--rw-r--r--   0 imacat    (1000) users      (100)     8130 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/report/reports/journal.py
--rw-r--r--   0 imacat    (1000) users      (100)    16530 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/report/reports/ledger.py
--rw-r--r--   0 imacat    (1000) users      (100)     8472 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/report/reports/search.py
--rw-r--r--   0 imacat    (1000) users      (100)     8853 2023-04-06 01:50:58.000000 mia-accounting-1.5.5/src/accounting/report/reports/trial_balance.py
--rw-r--r--   0 imacat    (1000) users      (100)     8099 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/report/reports/unapplied.py
--rw-r--r--   0 imacat    (1000) users      (100)     5210 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/report/reports/unapplied_accounts.py
--rw-r--r--   0 imacat    (1000) users      (100)     8169 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/report/reports/unmatched.py
--rw-r--r--   0 imacat    (1000) users      (100)     5191 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/report/reports/unmatched_accounts.py
--rw-r--r--   0 imacat    (1000) users      (100)     1205 2023-04-04 09:21:33.000000 mia-accounting-1.5.5/src/accounting/report/template_filters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.625698 mia-accounting-1.5.5/src/accounting/report/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      711 2023-04-04 09:21:34.000000 mia-accounting-1.5.5/src/accounting/report/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3034 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/report/utils/base_page_params.py
--rw-r--r--   0 imacat    (1000) users      (100)     1143 2023-04-04 09:21:36.000000 mia-accounting-1.5.5/src/accounting/report/utils/base_report.py
--rw-r--r--   0 imacat    (1000) users      (100)     3334 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/report/utils/csv_export.py
--rw-r--r--   0 imacat    (1000) users      (100)     7321 2023-04-29 22:38:16.000000 mia-accounting-1.5.5/src/accounting/report/utils/offset_matcher.py
--rw-r--r--   0 imacat    (1000) users      (100)     1368 2023-04-04 09:21:37.000000 mia-accounting-1.5.5/src/accounting/report/utils/option_link.py
--rw-r--r--   0 imacat    (1000) users      (100)     7881 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/report/utils/report_chooser.py
--rw-r--r--   0 imacat    (1000) users      (100)     1371 2023-04-17 08:41:57.000000 mia-accounting-1.5.5/src/accounting/report/utils/report_type.py
--rw-r--r--   0 imacat    (1000) users      (100)     4385 2023-04-23 05:21:41.000000 mia-accounting-1.5.5/src/accounting/report/utils/unapplied.py
--rw-r--r--   0 imacat    (1000) users      (100)     2221 2023-04-23 05:21:41.000000 mia-accounting-1.5.5/src/accounting/report/utils/unmatched.py
--rw-r--r--   0 imacat    (1000) users      (100)     5440 2023-04-18 00:59:05.000000 mia-accounting-1.5.5/src/accounting/report/utils/urls.py
--rw-r--r--   0 imacat    (1000) users      (100)    14167 2023-04-18 01:14:44.000000 mia-accounting-1.5.5/src/accounting/report/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.589699 mia-accounting-1.5.5/src/accounting/static/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.629698 mia-accounting-1.5.5/src/accounting/static/css/
--rw-r--r--   0 imacat    (1000) users      (100)    13431 2023-04-18 00:10:33.000000 mia-accounting-1.5.5/src/accounting/static/css/style.css
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.629698 mia-accounting-1.5.5/src/accounting/static/js/
--rw-r--r--   0 imacat    (1000) users      (100)    10921 2023-04-04 10:05:35.000000 mia-accounting-1.5.5/src/accounting/static/js/account-form.js
--rw-r--r--   0 imacat    (1000) users      (100)     1599 2023-04-04 10:05:35.000000 mia-accounting-1.5.5/src/accounting/static/js/account-order.js
--rw-r--r--   0 imacat    (1000) users      (100)     4955 2023-04-04 10:05:35.000000 mia-accounting-1.5.5/src/accounting/static/js/currency-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    38865 2023-04-17 23:44:56.000000 mia-accounting-1.5.5/src/accounting/static/js/description-editor.js
--rw-r--r--   0 imacat    (1000) users      (100)     3564 2023-04-04 10:05:35.000000 mia-accounting-1.5.5/src/accounting/static/js/drag-and-drop-reorder.js
--rw-r--r--   0 imacat    (1000) users      (100)     9211 2023-04-17 23:32:14.000000 mia-accounting-1.5.5/src/accounting/static/js/journal-entry-account-selector.js
--rw-r--r--   0 imacat    (1000) users      (100)    33086 2023-04-17 23:52:58.000000 mia-accounting-1.5.5/src/accounting/static/js/journal-entry-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    19665 2023-04-30 07:03:59.000000 mia-accounting-1.5.5/src/accounting/static/js/journal-entry-line-item-editor.js
--rw-r--r--   0 imacat    (1000) users      (100)     1366 2023-04-04 10:05:35.000000 mia-accounting-1.5.5/src/accounting/static/js/journal-entry-order.js
--rw-r--r--   0 imacat    (1000) users      (100)     1436 2023-04-04 10:05:35.000000 mia-accounting-1.5.5/src/accounting/static/js/material-fab-speed-dial.js
--rw-r--r--   0 imacat    (1000) users      (100)    28660 2023-04-04 10:05:35.000000 mia-accounting-1.5.5/src/accounting/static/js/option-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    11670 2023-04-17 23:40:31.000000 mia-accounting-1.5.5/src/accounting/static/js/original-line-item-selector.js
--rw-r--r--   0 imacat    (1000) users      (100)    10374 2023-04-04 10:05:35.000000 mia-accounting-1.5.5/src/accounting/static/js/period-chooser.js
--rw-r--r--   0 imacat    (1000) users      (100)     2712 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/template_filters.py
--rw-r--r--   0 imacat    (1000) users      (100)     1137 2023-04-23 01:43:59.000000 mia-accounting-1.5.5/src/accounting/template_globals.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.589699 mia-accounting-1.5.5/src/accounting/templates/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.629698 mia-accounting-1.5.5/src/accounting/templates/accounting/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.629698 mia-accounting-1.5.5/src/accounting/templates/accounting/account/
--rw-r--r--   0 imacat    (1000) users      (100)     1034 2023-04-04 10:04:10.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/account/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     4266 2023-04-04 10:04:11.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/account/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1081 2023-04-04 10:04:11.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/account/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.629698 mia-accounting-1.5.5/src/accounting/templates/accounting/account/include/
--rw-r--r--   0 imacat    (1000) users      (100)     5704 2023-04-04 10:04:10.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/account/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     2734 2023-05-17 13:41:19.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/account/list.html
--rw-r--r--   0 imacat    (1000) users      (100)     3052 2023-04-04 10:04:12.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/account/order.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.629698 mia-accounting-1.5.5/src/accounting/templates/accounting/base-account/
--rw-r--r--   0 imacat    (1000) users      (100)     1581 2023-04-04 10:04:10.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/base-account/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     2095 2023-05-17 13:41:20.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/base-account/list.html
--rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-04 10:04:10.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/base.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.633698 mia-accounting-1.5.5/src/accounting/templates/accounting/currency/
--rw-r--r--   0 imacat    (1000) users      (100)     1039 2023-04-04 10:04:12.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/currency/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     3883 2023-04-04 10:04:10.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/currency/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1152 2023-04-04 10:04:11.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/currency/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.633698 mia-accounting-1.5.5/src/accounting/templates/accounting/currency/include/
--rw-r--r--   0 imacat    (1000) users      (100)     2850 2023-04-04 10:04:10.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/currency/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     2606 2023-05-17 13:41:19.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/currency/list.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.633698 mia-accounting-1.5.5/src/accounting/templates/accounting/include/
--rw-r--r--   0 imacat    (1000) users      (100)     2706 2023-04-17 15:07:31.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/include/nav.html
--rw-r--r--   0 imacat    (1000) users      (100)     1986 2023-04-04 10:04:11.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/include/pagination.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.633698 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.633698 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/disbursement/
--rw-r--r--   0 imacat    (1000) users      (100)     1149 2023-04-04 23:56:52.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/disbursement/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2028 2023-04-04 10:04:11.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/disbursement/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1213 2023-04-04 10:04:09.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/disbursement/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.633698 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/disbursement/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1195 2023-04-04 10:04:10.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2283 2023-04-04 10:04:12.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.633698 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/
--rw-r--r--   0 imacat    (1000) users      (100)     3406 2023-04-17 23:32:14.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)    14561 2023-05-22 10:32:23.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     3242 2023-04-17 23:11:57.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html
--rw-r--r--   0 imacat    (1000) users      (100)     4554 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     2726 2023-04-04 10:04:10.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html
--rw-r--r--   0 imacat    (1000) users      (100)     6442 2023-04-17 23:54:15.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/form-line-item.html
--rw-r--r--   0 imacat    (1000) users      (100)     4370 2023-04-04 10:04:12.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     4231 2023-05-22 09:36:19.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     2093 2023-04-04 10:04:11.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html
--rw-r--r--   0 imacat    (1000) users      (100)     3791 2023-04-18 00:10:33.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     3069 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/order.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.633698 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/receipt/
--rw-r--r--   0 imacat    (1000) users      (100)     1134 2023-04-04 23:56:52.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/receipt/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2025 2023-04-04 10:04:12.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/receipt/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-04 10:04:11.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/receipt/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.633698 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/receipt/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1194 2023-04-04 10:04:12.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2278 2023-04-04 10:04:11.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/receipt/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.633698 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/transfer/
--rw-r--r--   0 imacat    (1000) users      (100)     1127 2023-04-04 23:56:52.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/transfer/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2691 2023-04-04 10:04:09.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/transfer/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1200 2023-04-04 10:04:10.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/transfer/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.637698 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/transfer/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1649 2023-04-04 10:04:11.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2845 2023-04-04 10:04:12.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/transfer/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.637698 mia-accounting-1.5.5/src/accounting/templates/accounting/option/
--rw-r--r--   0 imacat    (1000) users      (100)     2765 2023-04-08 10:12:54.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/option/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     4699 2023-04-08 00:27:23.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/option/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.637698 mia-accounting-1.5.5/src/accounting/templates/accounting/option/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1851 2023-04-04 10:04:10.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html
--rw-r--r--   0 imacat    (1000) users      (100)     3214 2023-04-04 10:04:12.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/option/include/form-recurring-item.html
--rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-04 10:04:12.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     4345 2023-05-22 09:36:19.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.637698 mia-accounting-1.5.5/src/accounting/templates/accounting/report/
--rw-r--r--   0 imacat    (1000) users      (100)     5435 2023-04-18 00:39:27.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/balance-sheet.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.637698 mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1970 2023-04-04 10:04:12.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html
--rw-r--r--   0 imacat    (1000) users      (100)     1708 2023-04-04 10:04:12.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/balance-sheet-section.html
--rw-r--r--   0 imacat    (1000) users      (100)     1281 2023-04-04 10:04:10.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html
--rw-r--r--   0 imacat    (1000) users      (100)     1760 2023-04-04 10:04:12.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html
--rw-r--r--   0 imacat    (1000) users      (100)     1252 2023-04-04 10:04:11.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/ledger-row-desktop.html
--rw-r--r--   0 imacat    (1000) users      (100)     1429 2023-04-04 10:04:10.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/ledger-row-mobile.html
--rw-r--r--   0 imacat    (1000) users      (100)     8857 2023-04-04 10:04:12.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/period-chooser.html
--rw-r--r--   0 imacat    (1000) users      (100)     1963 2023-05-17 13:41:20.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/search-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     5630 2023-05-17 13:41:20.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/toolbar-buttons.html
--rw-r--r--   0 imacat    (1000) users      (100)     4841 2023-04-18 00:34:44.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/income-expenses.html
--rw-r--r--   0 imacat    (1000) users      (100)     4618 2023-04-18 00:37:47.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/income-statement.html
--rw-r--r--   0 imacat    (1000) users      (100)     4202 2023-04-04 10:04:10.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/journal.html
--rw-r--r--   0 imacat    (1000) users      (100)     4946 2023-04-18 00:33:38.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/ledger.html
--rw-r--r--   0 imacat    (1000) users      (100)     4044 2023-04-04 10:04:11.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/search.html
--rw-r--r--   0 imacat    (1000) users      (100)     3710 2023-04-18 00:36:16.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/trial-balance.html
--rw-r--r--   0 imacat    (1000) users      (100)     3037 2023-04-18 00:59:05.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/unapplied-accounts.html
--rw-r--r--   0 imacat    (1000) users      (100)     3843 2023-04-18 00:59:06.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/unapplied.html
--rw-r--r--   0 imacat    (1000) users      (100)     3034 2023-04-18 00:59:05.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/unmatched-accounts.html
--rw-r--r--   0 imacat    (1000) users      (100)     6998 2023-04-18 00:59:05.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/unmatched.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.641698 mia-accounting-1.5.5/src/accounting/translations/
--rw-r--r--   0 imacat    (1000) users      (100)    49437 2023-04-18 01:32:01.000000 mia-accounting-1.5.5/src/accounting/translations/accounting.pot
--rw-r--r--   0 imacat    (1000) users      (100)       80 2023-01-27 03:33:36.000000 mia-accounting-1.5.5/src/accounting/translations/babel.cfg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.593699 mia-accounting-1.5.5/src/accounting/translations/zh_Hans/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.641698 mia-accounting-1.5.5/src/accounting/translations/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)    16202 2023-04-18 01:32:11.000000 mia-accounting-1.5.5/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo
--rw-r--r--   0 imacat    (1000) users      (100)    54246 2023-04-18 01:32:11.000000 mia-accounting-1.5.5/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.593699 mia-accounting-1.5.5/src/accounting/translations/zh_Hant/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.641698 mia-accounting-1.5.5/src/accounting/translations/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)    16202 2023-04-18 01:32:11.000000 mia-accounting-1.5.5/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo
--rw-r--r--   0 imacat    (1000) users      (100)    54246 2023-04-18 01:32:11.000000 mia-accounting-1.5.5/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.641698 mia-accounting-1.5.5/src/accounting/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      778 2023-04-04 09:21:31.000000 mia-accounting-1.5.5/src/accounting/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     1036 2023-05-17 07:33:36.000000 mia-accounting-1.5.5/src/accounting/utils/cast.py
--rw-r--r--   0 imacat    (1000) users      (100)     3325 2023-05-04 01:35:20.000000 mia-accounting-1.5.5/src/accounting/utils/current_account.py
--rw-r--r--   0 imacat    (1000) users      (100)     1426 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/utils/flash_errors.py
--rw-r--r--   0 imacat    (1000) users      (100)     1030 2023-04-04 09:21:32.000000 mia-accounting-1.5.5/src/accounting/utils/journal_entry_types.py
--rw-r--r--   0 imacat    (1000) users      (100)     3427 2023-05-22 23:11:54.000000 mia-accounting-1.5.5/src/accounting/utils/next_uri.py
--rw-r--r--   0 imacat    (1000) users      (100)     1198 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/utils/offset_alias.py
--rw-r--r--   0 imacat    (1000) users      (100)     6906 2023-04-08 10:12:55.000000 mia-accounting-1.5.5/src/accounting/utils/options.py
--rw-r--r--   0 imacat    (1000) users      (100)    11745 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/utils/pagination.py
--rw-r--r--   0 imacat    (1000) users      (100)     4262 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/utils/permission.py
--rw-r--r--   0 imacat    (1000) users      (100)     1638 2023-04-04 09:21:34.000000 mia-accounting-1.5.5/src/accounting/utils/query.py
--rw-r--r--   0 imacat    (1000) users      (100)     1221 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/utils/random_id.py
--rw-r--r--   0 imacat    (1000) users      (100)     1396 2023-04-04 09:21:37.000000 mia-accounting-1.5.5/src/accounting/utils/strip_text.py
--rw-r--r--   0 imacat    (1000) users      (100)     4985 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/utils/user.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.641698 mia-accounting-1.5.5/src/mia_accounting.egg-info/
--rw-r--r--   0 imacat    (1000) users      (100)     3412 2023-05-23 00:45:05.000000 mia-accounting-1.5.5/src/mia_accounting.egg-info/PKG-INFO
--rw-r--r--   0 imacat    (1000) users      (100)    11434 2023-05-23 00:45:05.000000 mia-accounting-1.5.5/src/mia_accounting.egg-info/SOURCES.txt
--rw-r--r--   0 imacat    (1000) users      (100)        1 2023-05-23 00:45:05.000000 mia-accounting-1.5.5/src/mia_accounting.egg-info/dependency_links.txt
--rw-r--r--   0 imacat    (1000) users      (100)      107 2023-05-23 00:45:05.000000 mia-accounting-1.5.5/src/mia_accounting.egg-info/requires.txt
--rw-r--r--   0 imacat    (1000) users      (100)       11 2023-05-23 00:45:05.000000 mia-accounting-1.5.5/src/mia_accounting.egg-info/top_level.txt
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.645698 mia-accounting-1.5.5/tests/
--rwxr-xr-x   0 imacat    (1000) users      (100)     4341 2023-04-12 07:04:32.000000 mia-accounting-1.5.5/tests/babel-utils-test-site.py
--rwxr-xr-x   0 imacat    (1000) users      (100)     4297 2023-04-12 07:04:32.000000 mia-accounting-1.5.5/tests/babel-utils.py
--rw-r--r--   0 imacat    (1000) users      (100)    32948 2023-05-22 23:22:24.000000 mia-accounting-1.5.5/tests/test_account.py
--rw-r--r--   0 imacat    (1000) users      (100)     2409 2023-04-10 15:59:48.000000 mia-accounting-1.5.5/tests/test_base_account.py
--rw-r--r--   0 imacat    (1000) users      (100)     6113 2023-04-29 21:45:47.000000 mia-accounting-1.5.5/tests/test_commands.py
--rw-r--r--   0 imacat    (1000) users      (100)    23998 2023-05-22 23:24:38.000000 mia-accounting-1.5.5/tests/test_currency.py
--rw-r--r--   0 imacat    (1000) users      (100)    16282 2023-05-22 23:26:32.000000 mia-accounting-1.5.5/tests/test_description_editor.py
--rw-r--r--   0 imacat    (1000) users      (100)   105500 2023-05-23 00:40:17.000000 mia-accounting-1.5.5/tests/test_journal_entry.py
--rw-r--r--   0 imacat    (1000) users      (100)    42546 2023-05-23 00:01:57.000000 mia-accounting-1.5.5/tests/test_offset.py
--rw-r--r--   0 imacat    (1000) users      (100)    16950 2023-05-23 00:10:42.000000 mia-accounting-1.5.5/tests/test_option.py
--rw-r--r--   0 imacat    (1000) users      (100)    17864 2023-04-29 21:45:47.000000 mia-accounting-1.5.5/tests/test_report.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.645698 mia-accounting-1.5.5/tests/test_site/
--rw-r--r--   0 imacat    (1000) users      (100)     4968 2023-05-23 00:22:47.000000 mia-accounting-1.5.5/tests/test_site/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3958 2023-04-29 21:45:47.000000 mia-accounting-1.5.5/tests/test_site/auth.py
--rw-r--r--   0 imacat    (1000) users      (100)    13324 2023-05-23 00:02:48.000000 mia-accounting-1.5.5/tests/test_site/lib.py
--rw-r--r--   0 imacat    (1000) users      (100)     3367 2023-05-17 11:57:23.000000 mia-accounting-1.5.5/tests/test_site/locale.py
--rw-r--r--   0 imacat    (1000) users      (100)    13050 2023-04-29 21:45:47.000000 mia-accounting-1.5.5/tests/test_site/reset.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.645698 mia-accounting-1.5.5/tests/test_site/static/
--rw-r--r--   0 imacat    (1000) users      (100)     1420 2023-04-03 07:56:03.000000 mia-accounting-1.5.5/tests/test_site/static/favicon.svg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.645698 mia-accounting-1.5.5/tests/test_site/templates/
--rw-r--r--   0 imacat    (1000) users      (100)     6656 2023-05-23 00:22:47.000000 mia-accounting-1.5.5/tests/test_site/templates/base.html
--rw-r--r--   0 imacat    (1000) users      (100)     1239 2023-04-11 14:27:31.000000 mia-accounting-1.5.5/tests/test_site/templates/home.html
--rw-r--r--   0 imacat    (1000) users      (100)     1532 2023-04-11 14:03:59.000000 mia-accounting-1.5.5/tests/test_site/templates/login.html
--rw-r--r--   0 imacat    (1000) users      (100)     1838 2023-04-12 10:05:13.000000 mia-accounting-1.5.5/tests/test_site/templates/reset.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.645698 mia-accounting-1.5.5/tests/test_site/translations/
--rw-r--r--   0 imacat    (1000) users      (100)       80 2023-02-03 05:00:02.000000 mia-accounting-1.5.5/tests/test_site/translations/babel.cfg
--rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-12 09:59:51.000000 mia-accounting-1.5.5/tests/test_site/translations/messages.pot
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.597699 mia-accounting-1.5.5/tests/test_site/translations/zh_Hans/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.645698 mia-accounting-1.5.5/tests/test_site/translations/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)     2275 2023-04-12 10:00:18.000000 mia-accounting-1.5.5/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo
--rw-r--r--   0 imacat    (1000) users      (100)     3505 2023-04-12 10:00:18.000000 mia-accounting-1.5.5/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.597699 mia-accounting-1.5.5/tests/test_site/translations/zh_Hant/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.649698 mia-accounting-1.5.5/tests/test_site/translations/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)     2275 2023-04-12 10:00:18.000000 mia-accounting-1.5.5/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo
--rw-r--r--   0 imacat    (1000) users      (100)     3505 2023-04-12 10:05:13.000000 mia-accounting-1.5.5/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po
--rw-r--r--   0 imacat    (1000) users      (100)    28011 2023-05-23 00:12:12.000000 mia-accounting-1.5.5/tests/test_unmatched_offset.py
--rw-r--r--   0 imacat    (1000) users      (100)    15328 2023-05-23 00:16:21.000000 mia-accounting-1.5.5/tests/test_utils.py
--rw-r--r--   0 imacat    (1000) users      (100)     5470 2023-05-22 23:23:54.000000 mia-accounting-1.5.5/tests/testlib.py
--rw-r--r--   0 imacat    (1000) users      (100)    16955 2023-05-22 23:52:24.000000 mia-accounting-1.5.5/tests/testlib_journal_entry.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.606039 mia-accounting-1.5.6/
+-rw-r--r--   0 imacat    (1000) users      (100)    11358 2015-02-17 18:06:12.000000 mia-accounting-1.5.6/LICENSE
+-rw-r--r--   0 imacat    (1000) users      (100)     1070 2023-04-05 11:25:31.000000 mia-accounting-1.5.6/MANIFEST.in
+-rw-r--r--   0 imacat    (1000) users      (100)     3412 2023-05-23 01:08:21.606039 mia-accounting-1.5.6/PKG-INFO
+-rw-r--r--   0 imacat    (1000) users      (100)     2525 2023-04-23 12:04:20.000000 mia-accounting-1.5.6/README.rst
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.574039 mia-accounting-1.5.6/docs/
+-rw-r--r--   0 imacat    (1000) users      (100)      638 2023-01-27 04:20:04.000000 mia-accounting-1.5.6/docs/Makefile
+-rw-r--r--   0 imacat    (1000) users      (100)      804 2023-01-27 04:20:04.000000 mia-accounting-1.5.6/docs/make.bat
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.574039 mia-accounting-1.5.6/docs/source/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.574039 mia-accounting-1.5.6/docs/source/_static/
+-rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:08.000000 mia-accounting-1.5.6/docs/source/_static/.keep
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.574039 mia-accounting-1.5.6/docs/source/_templates/
+-rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:11.000000 mia-accounting-1.5.6/docs/source/_templates/.keep
+-rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-05-23 00:37:49.000000 mia-accounting-1.5.6/docs/source/accounting.account.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      959 2023-05-23 00:37:49.000000 mia-accounting-1.5.6/docs/source/accounting.base_account.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1053 2023-05-23 00:37:49.000000 mia-accounting-1.5.6/docs/source/accounting.currency.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1089 2023-05-23 00:37:49.000000 mia-accounting-1.5.6/docs/source/accounting.journal_entry.forms.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      937 2023-05-23 00:37:49.000000 mia-accounting-1.5.6/docs/source/accounting.journal_entry.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1162 2023-05-23 00:37:49.000000 mia-accounting-1.5.6/docs/source/accounting.journal_entry.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      513 2023-05-23 00:37:49.000000 mia-accounting-1.5.6/docs/source/accounting.option.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1551 2023-05-23 00:37:49.000000 mia-accounting-1.5.6/docs/source/accounting.report.period.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2460 2023-05-23 00:37:49.000000 mia-accounting-1.5.6/docs/source/accounting.report.reports.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      861 2023-05-23 00:37:49.000000 mia-accounting-1.5.6/docs/source/accounting.report.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2168 2023-05-23 00:37:49.000000 mia-accounting-1.5.6/docs/source/accounting.report.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1301 2023-05-23 00:37:49.000000 mia-accounting-1.5.6/docs/source/accounting.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2405 2023-05-23 00:37:49.000000 mia-accounting-1.5.6/docs/source/accounting.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     8529 2023-05-23 01:07:11.000000 mia-accounting-1.5.6/docs/source/changelog.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1051 2023-04-23 12:12:53.000000 mia-accounting-1.5.6/docs/source/conf.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1508 2023-04-06 00:38:39.000000 mia-accounting-1.5.6/docs/source/examples.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2837 2023-04-06 00:21:32.000000 mia-accounting-1.5.6/docs/source/history.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      521 2023-04-23 12:04:21.000000 mia-accounting-1.5.6/docs/source/index.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     3568 2023-05-06 15:58:29.000000 mia-accounting-1.5.6/docs/source/intro.rst
+-rw-r--r--   0 imacat    (1000) users      (100)       53 2023-04-04 10:25:53.000000 mia-accounting-1.5.6/docs/source/modules.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1994 2023-05-09 00:42:23.000000 mia-accounting-1.5.6/pyproject.toml
+-rw-r--r--   0 imacat    (1000) users      (100)       38 2023-05-23 01:08:21.610039 mia-accounting-1.5.6/setup.cfg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.570039 mia-accounting-1.5.6/src/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.578039 mia-accounting-1.5.6/src/accounting/
+-rw-r--r--   0 imacat    (1000) users      (100)     3045 2023-05-23 01:07:41.000000 mia-accounting-1.5.6/src/accounting/__init__.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.578039 mia-accounting-1.5.6/src/accounting/account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-10 15:59:48.000000 mia-accounting-1.5.6/src/accounting/account/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3868 2023-04-29 21:45:45.000000 mia-accounting-1.5.6/src/accounting/account/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1512 2023-04-04 09:21:35.000000 mia-accounting-1.5.6/src/accounting/account/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7145 2023-04-04 09:21:33.000000 mia-accounting-1.5.6/src/accounting/account/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2209 2023-04-04 09:21:35.000000 mia-accounting-1.5.6/src/accounting/account/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7416 2023-04-09 02:08:22.000000 mia-accounting-1.5.6/src/accounting/account/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.578039 mia-accounting-1.5.6/src/accounting/base_account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1240 2023-04-10 15:59:48.000000 mia-accounting-1.5.6/src/accounting/base_account/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1800 2023-04-10 15:59:48.000000 mia-accounting-1.5.6/src/accounting/base_account/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1592 2023-04-04 09:21:35.000000 mia-accounting-1.5.6/src/accounting/base_account/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1769 2023-04-04 09:21:37.000000 mia-accounting-1.5.6/src/accounting/base_account/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1812 2023-04-09 02:08:22.000000 mia-accounting-1.5.6/src/accounting/base_account/views.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2138 2023-04-10 15:59:48.000000 mia-accounting-1.5.6/src/accounting/commands.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.578039 mia-accounting-1.5.6/src/accounting/currency/
+-rw-r--r--   0 imacat    (1000) users      (100)     1312 2023-04-10 15:59:48.000000 mia-accounting-1.5.6/src/accounting/currency/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2206 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/currency/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1556 2023-04-04 09:21:35.000000 mia-accounting-1.5.6/src/accounting/currency/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3172 2023-04-04 09:21:36.000000 mia-accounting-1.5.6/src/accounting/currency/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1720 2023-04-04 09:21:34.000000 mia-accounting-1.5.6/src/accounting/currency/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6609 2023-04-09 02:08:22.000000 mia-accounting-1.5.6/src/accounting/currency/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.578039 mia-accounting-1.5.6/src/accounting/data/
+-rw-r--r--   0 imacat    (1000) users      (100)    36368 2023-03-14 01:04:26.000000 mia-accounting-1.5.6/src/accounting/data/base_accounts.csv
+-rw-r--r--   0 imacat    (1000) users      (100)      370 2023-03-14 01:04:26.000000 mia-accounting-1.5.6/src/accounting/data/currencies.csv
+-rw-r--r--   0 imacat    (1000) users      (100)     3144 2023-04-04 09:21:33.000000 mia-accounting-1.5.6/src/accounting/forms.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.582039 mia-accounting-1.5.6/src/accounting/journal_entry/
+-rw-r--r--   0 imacat    (1000) users      (100)     1376 2023-04-04 09:21:35.000000 mia-accounting-1.5.6/src/accounting/journal_entry/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3302 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/journal_entry/converters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.582039 mia-accounting-1.5.6/src/accounting/journal_entry/forms/
+-rw-r--r--   0 imacat    (1000) users      (100)      934 2023-04-04 09:21:37.000000 mia-accounting-1.5.6/src/accounting/journal_entry/forms/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11003 2023-04-23 05:21:41.000000 mia-accounting-1.5.6/src/accounting/journal_entry/forms/currency.py
+-rw-r--r--   0 imacat    (1000) users      (100)    24568 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/journal_entry/forms/journal_entry.py
+-rw-r--r--   0 imacat    (1000) users      (100)    19807 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/journal_entry/forms/line_item.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3291 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/journal_entry/forms/reorder.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2535 2023-04-04 09:21:32.000000 mia-accounting-1.5.6/src/accounting/journal_entry/template_filters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.582039 mia-accounting-1.5.6/src/accounting/journal_entry/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      729 2023-04-04 09:21:32.000000 mia-accounting-1.5.6/src/accounting/journal_entry/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1802 2023-04-17 23:37:17.000000 mia-accounting-1.5.6/src/accounting/journal_entry/utils/account_option.py
+-rw-r--r--   0 imacat    (1000) users      (100)    12981 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/journal_entry/utils/description_editor.py
+-rw-r--r--   0 imacat    (1000) users      (100)    12676 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/journal_entry/utils/operators.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3722 2023-04-23 05:21:41.000000 mia-accounting-1.5.6/src/accounting/journal_entry/utils/original_line_items.py
+-rw-r--r--   0 imacat    (1000) users      (100)     9351 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/journal_entry/views.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3809 2023-04-04 09:21:33.000000 mia-accounting-1.5.6/src/accounting/locale.py
+-rw-r--r--   0 imacat    (1000) users      (100)    32618 2023-04-30 07:03:58.000000 mia-accounting-1.5.6/src/accounting/models.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.582039 mia-accounting-1.5.6/src/accounting/option/
+-rw-r--r--   0 imacat    (1000) users      (100)      993 2023-04-04 09:21:35.000000 mia-accounting-1.5.6/src/accounting/option/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     9762 2023-04-08 00:27:23.000000 mia-accounting-1.5.6/src/accounting/option/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2827 2023-04-04 09:21:32.000000 mia-accounting-1.5.6/src/accounting/option/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.582039 mia-accounting-1.5.6/src/accounting/report/
+-rw-r--r--   0 imacat    (1000) users      (100)     1362 2023-04-08 10:12:56.000000 mia-accounting-1.5.6/src/accounting/report/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-08 10:12:56.000000 mia-accounting-1.5.6/src/accounting/report/converters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.582039 mia-accounting-1.5.6/src/accounting/report/period/
+-rw-r--r--   0 imacat    (1000) users      (100)      793 2023-04-04 09:21:32.000000 mia-accounting-1.5.6/src/accounting/report/period/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3702 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/report/period/chooser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5557 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/report/period/description.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1050 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/report/period/month_end.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4127 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/report/period/parser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4522 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/report/period/period.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4785 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/report/period/shortcuts.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3915 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/report/period/specification.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.586039 mia-accounting-1.5.6/src/accounting/report/reports/
+-rw-r--r--   0 imacat    (1000) users      (100)      946 2023-04-04 09:21:36.000000 mia-accounting-1.5.6/src/accounting/report/reports/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)    17920 2023-04-06 01:50:58.000000 mia-accounting-1.5.6/src/accounting/report/reports/balance_sheet.py
+-rw-r--r--   0 imacat    (1000) users      (100)    18807 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/report/reports/income_expenses.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11733 2023-04-06 01:50:58.000000 mia-accounting-1.5.6/src/accounting/report/reports/income_statement.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8130 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/report/reports/journal.py
+-rw-r--r--   0 imacat    (1000) users      (100)    16530 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/report/reports/ledger.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8472 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/report/reports/search.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8853 2023-04-06 01:50:58.000000 mia-accounting-1.5.6/src/accounting/report/reports/trial_balance.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8099 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/report/reports/unapplied.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5210 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/report/reports/unapplied_accounts.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8169 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/report/reports/unmatched.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5191 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/report/reports/unmatched_accounts.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1205 2023-04-04 09:21:33.000000 mia-accounting-1.5.6/src/accounting/report/template_filters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.586039 mia-accounting-1.5.6/src/accounting/report/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      711 2023-04-04 09:21:34.000000 mia-accounting-1.5.6/src/accounting/report/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3034 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/report/utils/base_page_params.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1143 2023-04-04 09:21:36.000000 mia-accounting-1.5.6/src/accounting/report/utils/base_report.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3334 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/report/utils/csv_export.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7321 2023-04-29 22:38:16.000000 mia-accounting-1.5.6/src/accounting/report/utils/offset_matcher.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1368 2023-04-04 09:21:37.000000 mia-accounting-1.5.6/src/accounting/report/utils/option_link.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7881 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/report/utils/report_chooser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1371 2023-04-17 08:41:57.000000 mia-accounting-1.5.6/src/accounting/report/utils/report_type.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4385 2023-04-23 05:21:41.000000 mia-accounting-1.5.6/src/accounting/report/utils/unapplied.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2221 2023-04-23 05:21:41.000000 mia-accounting-1.5.6/src/accounting/report/utils/unmatched.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5440 2023-04-18 00:59:05.000000 mia-accounting-1.5.6/src/accounting/report/utils/urls.py
+-rw-r--r--   0 imacat    (1000) users      (100)    14167 2023-04-18 01:14:44.000000 mia-accounting-1.5.6/src/accounting/report/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.570039 mia-accounting-1.5.6/src/accounting/static/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.586039 mia-accounting-1.5.6/src/accounting/static/css/
+-rw-r--r--   0 imacat    (1000) users      (100)    13431 2023-04-18 00:10:33.000000 mia-accounting-1.5.6/src/accounting/static/css/style.css
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.590039 mia-accounting-1.5.6/src/accounting/static/js/
+-rw-r--r--   0 imacat    (1000) users      (100)    10921 2023-04-04 10:05:35.000000 mia-accounting-1.5.6/src/accounting/static/js/account-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1599 2023-04-04 10:05:35.000000 mia-accounting-1.5.6/src/accounting/static/js/account-order.js
+-rw-r--r--   0 imacat    (1000) users      (100)     4955 2023-04-04 10:05:35.000000 mia-accounting-1.5.6/src/accounting/static/js/currency-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    38865 2023-04-17 23:44:56.000000 mia-accounting-1.5.6/src/accounting/static/js/description-editor.js
+-rw-r--r--   0 imacat    (1000) users      (100)     3564 2023-04-04 10:05:35.000000 mia-accounting-1.5.6/src/accounting/static/js/drag-and-drop-reorder.js
+-rw-r--r--   0 imacat    (1000) users      (100)     9211 2023-04-17 23:32:14.000000 mia-accounting-1.5.6/src/accounting/static/js/journal-entry-account-selector.js
+-rw-r--r--   0 imacat    (1000) users      (100)    33086 2023-04-17 23:52:58.000000 mia-accounting-1.5.6/src/accounting/static/js/journal-entry-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    19665 2023-04-30 07:03:59.000000 mia-accounting-1.5.6/src/accounting/static/js/journal-entry-line-item-editor.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1366 2023-04-04 10:05:35.000000 mia-accounting-1.5.6/src/accounting/static/js/journal-entry-order.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1436 2023-04-04 10:05:35.000000 mia-accounting-1.5.6/src/accounting/static/js/material-fab-speed-dial.js
+-rw-r--r--   0 imacat    (1000) users      (100)    28660 2023-04-04 10:05:35.000000 mia-accounting-1.5.6/src/accounting/static/js/option-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    11670 2023-04-17 23:40:31.000000 mia-accounting-1.5.6/src/accounting/static/js/original-line-item-selector.js
+-rw-r--r--   0 imacat    (1000) users      (100)    10374 2023-04-04 10:05:35.000000 mia-accounting-1.5.6/src/accounting/static/js/period-chooser.js
+-rw-r--r--   0 imacat    (1000) users      (100)     2712 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/template_filters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1137 2023-04-23 01:43:59.000000 mia-accounting-1.5.6/src/accounting/template_globals.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.570039 mia-accounting-1.5.6/src/accounting/templates/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.590039 mia-accounting-1.5.6/src/accounting/templates/accounting/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.590039 mia-accounting-1.5.6/src/accounting/templates/accounting/account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1025 2023-05-23 01:03:30.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/account/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4266 2023-04-04 10:04:11.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/account/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1081 2023-04-04 10:04:11.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/account/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.590039 mia-accounting-1.5.6/src/accounting/templates/accounting/account/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     5704 2023-04-04 10:04:10.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/account/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2734 2023-05-17 13:41:19.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/account/list.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3052 2023-04-04 10:04:12.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/account/order.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.590039 mia-accounting-1.5.6/src/accounting/templates/accounting/base-account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1581 2023-04-04 10:04:10.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/base-account/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2095 2023-05-17 13:41:20.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/base-account/list.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-04 10:04:10.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/base.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.590039 mia-accounting-1.5.6/src/accounting/templates/accounting/currency/
+-rw-r--r--   0 imacat    (1000) users      (100)     1030 2023-05-23 01:03:29.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/currency/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3883 2023-04-04 10:04:10.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/currency/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1152 2023-04-04 10:04:11.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/currency/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.590039 mia-accounting-1.5.6/src/accounting/templates/accounting/currency/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     2850 2023-04-04 10:04:10.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/currency/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2606 2023-05-17 13:41:19.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/currency/list.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.590039 mia-accounting-1.5.6/src/accounting/templates/accounting/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     2706 2023-04-17 15:07:31.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/include/nav.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1986 2023-04-04 10:04:11.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/include/pagination.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.590039 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.590039 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/disbursement/
+-rw-r--r--   0 imacat    (1000) users      (100)     1140 2023-05-23 01:03:30.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/disbursement/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2028 2023-04-04 10:04:11.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/disbursement/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1213 2023-04-04 10:04:09.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/disbursement/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.594039 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/disbursement/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1195 2023-04-04 10:04:10.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2283 2023-04-04 10:04:12.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.594039 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     3406 2023-04-17 23:32:14.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)    14561 2023-05-22 10:32:23.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3242 2023-04-17 23:11:57.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4554 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2726 2023-04-04 10:04:10.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html
+-rw-r--r--   0 imacat    (1000) users      (100)     6442 2023-04-17 23:54:15.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/form-line-item.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4370 2023-04-04 10:04:12.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4231 2023-05-22 09:36:19.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2093 2023-04-04 10:04:11.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3791 2023-04-18 00:10:33.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3069 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/order.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.594039 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/receipt/
+-rw-r--r--   0 imacat    (1000) users      (100)     1125 2023-05-23 01:03:29.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/receipt/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2025 2023-04-04 10:04:12.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/receipt/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-04 10:04:11.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/receipt/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.594039 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/receipt/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1194 2023-04-04 10:04:12.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2278 2023-04-04 10:04:11.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/receipt/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.594039 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/transfer/
+-rw-r--r--   0 imacat    (1000) users      (100)     1118 2023-05-23 01:03:55.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/transfer/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2691 2023-04-04 10:04:09.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/transfer/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1200 2023-04-04 10:04:10.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/transfer/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.594039 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/transfer/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1649 2023-04-04 10:04:11.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2845 2023-04-04 10:04:12.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/transfer/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.594039 mia-accounting-1.5.6/src/accounting/templates/accounting/option/
+-rw-r--r--   0 imacat    (1000) users      (100)     2765 2023-04-08 10:12:54.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/option/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4699 2023-04-08 00:27:23.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/option/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.598039 mia-accounting-1.5.6/src/accounting/templates/accounting/option/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1851 2023-04-04 10:04:10.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3214 2023-04-04 10:04:12.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/option/include/form-recurring-item.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-04 10:04:12.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4345 2023-05-22 09:36:19.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.598039 mia-accounting-1.5.6/src/accounting/templates/accounting/report/
+-rw-r--r--   0 imacat    (1000) users      (100)     5435 2023-04-18 00:39:27.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/balance-sheet.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.598039 mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1970 2023-04-04 10:04:12.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1708 2023-04-04 10:04:12.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/balance-sheet-section.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1281 2023-04-04 10:04:10.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1760 2023-04-04 10:04:12.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1252 2023-04-04 10:04:11.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/ledger-row-desktop.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1429 2023-04-04 10:04:10.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/ledger-row-mobile.html
+-rw-r--r--   0 imacat    (1000) users      (100)     8857 2023-04-04 10:04:12.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/period-chooser.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1963 2023-05-17 13:41:20.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/search-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     5630 2023-05-17 13:41:20.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/toolbar-buttons.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4841 2023-04-18 00:34:44.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/income-expenses.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4618 2023-04-18 00:37:47.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/income-statement.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4202 2023-04-04 10:04:10.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/journal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4946 2023-04-18 00:33:38.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/ledger.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4044 2023-04-04 10:04:11.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/search.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3710 2023-04-18 00:36:16.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/trial-balance.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3037 2023-04-18 00:59:05.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/unapplied-accounts.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3843 2023-04-18 00:59:06.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/unapplied.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3034 2023-04-18 00:59:05.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/unmatched-accounts.html
+-rw-r--r--   0 imacat    (1000) users      (100)     6959 2023-05-23 00:59:42.000000 mia-accounting-1.5.6/src/accounting/templates/accounting/report/unmatched.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.598039 mia-accounting-1.5.6/src/accounting/translations/
+-rw-r--r--   0 imacat    (1000) users      (100)    49437 2023-04-18 01:32:01.000000 mia-accounting-1.5.6/src/accounting/translations/accounting.pot
+-rw-r--r--   0 imacat    (1000) users      (100)       80 2023-01-27 03:33:36.000000 mia-accounting-1.5.6/src/accounting/translations/babel.cfg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.570039 mia-accounting-1.5.6/src/accounting/translations/zh_Hans/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.598039 mia-accounting-1.5.6/src/accounting/translations/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)    16202 2023-04-18 01:32:11.000000 mia-accounting-1.5.6/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo
+-rw-r--r--   0 imacat    (1000) users      (100)    54246 2023-04-18 01:32:11.000000 mia-accounting-1.5.6/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.570039 mia-accounting-1.5.6/src/accounting/translations/zh_Hant/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.602039 mia-accounting-1.5.6/src/accounting/translations/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)    16202 2023-04-18 01:32:11.000000 mia-accounting-1.5.6/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo
+-rw-r--r--   0 imacat    (1000) users      (100)    54246 2023-04-18 01:32:11.000000 mia-accounting-1.5.6/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.602039 mia-accounting-1.5.6/src/accounting/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      778 2023-04-04 09:21:31.000000 mia-accounting-1.5.6/src/accounting/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1036 2023-05-17 07:33:36.000000 mia-accounting-1.5.6/src/accounting/utils/cast.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3325 2023-05-04 01:35:20.000000 mia-accounting-1.5.6/src/accounting/utils/current_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1426 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/utils/flash_errors.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1030 2023-04-04 09:21:32.000000 mia-accounting-1.5.6/src/accounting/utils/journal_entry_types.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3749 2023-05-23 00:59:42.000000 mia-accounting-1.5.6/src/accounting/utils/next_uri.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1198 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/utils/offset_alias.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6906 2023-04-08 10:12:55.000000 mia-accounting-1.5.6/src/accounting/utils/options.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11745 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/utils/pagination.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4262 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/utils/permission.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1638 2023-04-04 09:21:34.000000 mia-accounting-1.5.6/src/accounting/utils/query.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1221 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/utils/random_id.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1396 2023-04-04 09:21:37.000000 mia-accounting-1.5.6/src/accounting/utils/strip_text.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4985 2023-04-29 21:45:46.000000 mia-accounting-1.5.6/src/accounting/utils/user.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.602039 mia-accounting-1.5.6/src/mia_accounting.egg-info/
+-rw-r--r--   0 imacat    (1000) users      (100)     3412 2023-05-23 01:08:21.000000 mia-accounting-1.5.6/src/mia_accounting.egg-info/PKG-INFO
+-rw-r--r--   0 imacat    (1000) users      (100)    11434 2023-05-23 01:08:21.000000 mia-accounting-1.5.6/src/mia_accounting.egg-info/SOURCES.txt
+-rw-r--r--   0 imacat    (1000) users      (100)        1 2023-05-23 01:08:21.000000 mia-accounting-1.5.6/src/mia_accounting.egg-info/dependency_links.txt
+-rw-r--r--   0 imacat    (1000) users      (100)      107 2023-05-23 01:08:21.000000 mia-accounting-1.5.6/src/mia_accounting.egg-info/requires.txt
+-rw-r--r--   0 imacat    (1000) users      (100)       11 2023-05-23 01:08:21.000000 mia-accounting-1.5.6/src/mia_accounting.egg-info/top_level.txt
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.606039 mia-accounting-1.5.6/tests/
+-rwxr-xr-x   0 imacat    (1000) users      (100)     4341 2023-04-12 07:04:32.000000 mia-accounting-1.5.6/tests/babel-utils-test-site.py
+-rwxr-xr-x   0 imacat    (1000) users      (100)     4297 2023-04-12 07:04:32.000000 mia-accounting-1.5.6/tests/babel-utils.py
+-rw-r--r--   0 imacat    (1000) users      (100)    32948 2023-05-22 23:22:24.000000 mia-accounting-1.5.6/tests/test_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2409 2023-04-10 15:59:48.000000 mia-accounting-1.5.6/tests/test_base_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6113 2023-04-29 21:45:47.000000 mia-accounting-1.5.6/tests/test_commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)    23998 2023-05-22 23:24:38.000000 mia-accounting-1.5.6/tests/test_currency.py
+-rw-r--r--   0 imacat    (1000) users      (100)    16282 2023-05-22 23:26:32.000000 mia-accounting-1.5.6/tests/test_description_editor.py
+-rw-r--r--   0 imacat    (1000) users      (100)   105500 2023-05-23 00:40:17.000000 mia-accounting-1.5.6/tests/test_journal_entry.py
+-rw-r--r--   0 imacat    (1000) users      (100)    42546 2023-05-23 00:01:57.000000 mia-accounting-1.5.6/tests/test_offset.py
+-rw-r--r--   0 imacat    (1000) users      (100)    16950 2023-05-23 00:10:42.000000 mia-accounting-1.5.6/tests/test_option.py
+-rw-r--r--   0 imacat    (1000) users      (100)    17864 2023-04-29 21:45:47.000000 mia-accounting-1.5.6/tests/test_report.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.606039 mia-accounting-1.5.6/tests/test_site/
+-rw-r--r--   0 imacat    (1000) users      (100)     4649 2023-05-23 00:59:42.000000 mia-accounting-1.5.6/tests/test_site/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3958 2023-04-29 21:45:47.000000 mia-accounting-1.5.6/tests/test_site/auth.py
+-rw-r--r--   0 imacat    (1000) users      (100)    13324 2023-05-23 00:02:48.000000 mia-accounting-1.5.6/tests/test_site/lib.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3367 2023-05-17 11:57:23.000000 mia-accounting-1.5.6/tests/test_site/locale.py
+-rw-r--r--   0 imacat    (1000) users      (100)    13050 2023-04-29 21:45:47.000000 mia-accounting-1.5.6/tests/test_site/reset.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.606039 mia-accounting-1.5.6/tests/test_site/static/
+-rw-r--r--   0 imacat    (1000) users      (100)     1420 2023-04-03 07:56:03.000000 mia-accounting-1.5.6/tests/test_site/static/favicon.svg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.606039 mia-accounting-1.5.6/tests/test_site/templates/
+-rw-r--r--   0 imacat    (1000) users      (100)     6656 2023-05-23 00:22:47.000000 mia-accounting-1.5.6/tests/test_site/templates/base.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1239 2023-04-11 14:27:31.000000 mia-accounting-1.5.6/tests/test_site/templates/home.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1532 2023-04-11 14:03:59.000000 mia-accounting-1.5.6/tests/test_site/templates/login.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1838 2023-04-12 10:05:13.000000 mia-accounting-1.5.6/tests/test_site/templates/reset.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.606039 mia-accounting-1.5.6/tests/test_site/translations/
+-rw-r--r--   0 imacat    (1000) users      (100)       80 2023-02-03 05:00:02.000000 mia-accounting-1.5.6/tests/test_site/translations/babel.cfg
+-rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-12 09:59:51.000000 mia-accounting-1.5.6/tests/test_site/translations/messages.pot
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.570039 mia-accounting-1.5.6/tests/test_site/translations/zh_Hans/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.606039 mia-accounting-1.5.6/tests/test_site/translations/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)     2275 2023-04-12 10:00:18.000000 mia-accounting-1.5.6/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo
+-rw-r--r--   0 imacat    (1000) users      (100)     3505 2023-04-12 10:00:18.000000 mia-accounting-1.5.6/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.570039 mia-accounting-1.5.6/tests/test_site/translations/zh_Hant/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 01:08:21.606039 mia-accounting-1.5.6/tests/test_site/translations/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)     2275 2023-04-12 10:00:18.000000 mia-accounting-1.5.6/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo
+-rw-r--r--   0 imacat    (1000) users      (100)     3505 2023-04-12 10:05:13.000000 mia-accounting-1.5.6/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po
+-rw-r--r--   0 imacat    (1000) users      (100)    28011 2023-05-23 00:12:12.000000 mia-accounting-1.5.6/tests/test_unmatched_offset.py
+-rw-r--r--   0 imacat    (1000) users      (100)    15328 2023-05-23 00:16:21.000000 mia-accounting-1.5.6/tests/test_utils.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5470 2023-05-22 23:23:54.000000 mia-accounting-1.5.6/tests/testlib.py
+-rw-r--r--   0 imacat    (1000) users      (100)    16955 2023-05-22 23:52:24.000000 mia-accounting-1.5.6/tests/testlib_journal_entry.py
```

### Comparing `mia-accounting-1.5.5/LICENSE` & `mia-accounting-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/MANIFEST.in` & `mia-accounting-1.5.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/PKG-INFO` & `mia-accounting-1.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mia-accounting
-Version: 1.5.5
+Version: 1.5.6
 Summary: A Flask accounting module.
 Author-email: imacat <imacat@mail.imacat.idv.tw>
 Project-URL: Documentation, https://mia-accounting.readthedocs.io
 Project-URL: Change Log, https://mia-accounting.readthedocs.io/en/latest/changelog.html
 Project-URL: Repository, https://github.com/imacat/mia-accounting
 Project-URL: Bug Tracker, https://github.com/imacat/mia-accounting/issues
 Project-URL: Demonstration, https://accounting.imacat.idv.tw
```

### Comparing `mia-accounting-1.5.5/README.rst` & `mia-accounting-1.5.6/README.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/docs/Makefile` & `mia-accounting-1.5.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/docs/make.bat` & `mia-accounting-1.5.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/docs/source/accounting.account.rst` & `mia-accounting-1.5.6/docs/source/accounting.account.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/docs/source/accounting.base_account.rst` & `mia-accounting-1.5.6/docs/source/accounting.base_account.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/docs/source/accounting.currency.rst` & `mia-accounting-1.5.6/docs/source/accounting.currency.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/docs/source/accounting.journal_entry.forms.rst` & `mia-accounting-1.5.6/docs/source/accounting.journal_entry.forms.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/docs/source/accounting.journal_entry.rst` & `mia-accounting-1.5.6/docs/source/accounting.journal_entry.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/docs/source/accounting.journal_entry.utils.rst` & `mia-accounting-1.5.6/docs/source/accounting.journal_entry.utils.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/docs/source/accounting.option.rst` & `mia-accounting-1.5.6/docs/source/accounting.option.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/docs/source/accounting.report.period.rst` & `mia-accounting-1.5.6/docs/source/accounting.report.period.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/docs/source/accounting.report.reports.rst` & `mia-accounting-1.5.6/docs/source/accounting.report.reports.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/docs/source/accounting.report.rst` & `mia-accounting-1.5.6/docs/source/accounting.report.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/docs/source/accounting.report.utils.rst` & `mia-accounting-1.5.6/docs/source/accounting.report.utils.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/docs/source/accounting.rst` & `mia-accounting-1.5.6/docs/source/accounting.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/docs/source/accounting.utils.rst` & `mia-accounting-1.5.6/docs/source/accounting.utils.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/docs/source/changelog.rst` & `mia-accounting-1.5.6/docs/source/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 Change Log
 ==========
 
 
+Version 1.5.6
+-------------
+
+Released 2023/5/23
+
+Bug fixes.
+
+* Fixed the return URI of the creation forms to decode the next URI.
+* Fixed the unmatched offset list to use the encoded next URI.
+
+
 Version 1.5.5
 -------------
 
 Released 2023/5/23
 
 Security fixes.
```

### Comparing `mia-accounting-1.5.5/docs/source/conf.py` & `mia-accounting-1.5.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/docs/source/examples.rst` & `mia-accounting-1.5.6/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/docs/source/history.rst` & `mia-accounting-1.5.6/docs/source/history.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/docs/source/index.rst` & `mia-accounting-1.5.6/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/docs/source/intro.rst` & `mia-accounting-1.5.6/docs/source/intro.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/pyproject.toml` & `mia-accounting-1.5.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/__init__.py` & `mia-accounting-1.5.6/src/accounting/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from pathlib import Path
 
 from flask import Flask, Blueprint
 from flask_sqlalchemy import SQLAlchemy
 
 from accounting.utils.user import UserUtilityInterface
 
-VERSION: str = "1.5.5"
+VERSION: str = "1.5.6"
 """The package version."""
 db: SQLAlchemy = SQLAlchemy()
 """The database instance."""
 data_dir: Path = Path(__file__).parent / "data"
 """The data directory."""
```

### Comparing `mia-accounting-1.5.5/src/accounting/account/__init__.py` & `mia-accounting-1.5.6/src/accounting/account/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/account/commands.py` & `mia-accounting-1.5.6/src/accounting/account/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/account/converters.py` & `mia-accounting-1.5.6/src/accounting/account/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/account/forms.py` & `mia-accounting-1.5.6/src/accounting/account/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/account/queries.py` & `mia-accounting-1.5.6/src/accounting/account/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/account/views.py` & `mia-accounting-1.5.6/src/accounting/account/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/base_account/__init__.py` & `mia-accounting-1.5.6/src/accounting/base_account/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/base_account/commands.py` & `mia-accounting-1.5.6/src/accounting/base_account/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/base_account/converters.py` & `mia-accounting-1.5.6/src/accounting/base_account/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/base_account/queries.py` & `mia-accounting-1.5.6/src/accounting/base_account/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/base_account/views.py` & `mia-accounting-1.5.6/src/accounting/base_account/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/commands.py` & `mia-accounting-1.5.6/src/accounting/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/currency/__init__.py` & `mia-accounting-1.5.6/src/accounting/currency/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/currency/commands.py` & `mia-accounting-1.5.6/src/accounting/currency/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/currency/converters.py` & `mia-accounting-1.5.6/src/accounting/currency/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/currency/forms.py` & `mia-accounting-1.5.6/src/accounting/currency/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/currency/queries.py` & `mia-accounting-1.5.6/src/accounting/currency/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/currency/views.py` & `mia-accounting-1.5.6/src/accounting/currency/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/data/base_accounts.csv` & `mia-accounting-1.5.6/src/accounting/data/base_accounts.csv`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/forms.py` & `mia-accounting-1.5.6/src/accounting/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/journal_entry/__init__.py` & `mia-accounting-1.5.6/src/accounting/journal_entry/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/journal_entry/converters.py` & `mia-accounting-1.5.6/src/accounting/journal_entry/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/journal_entry/forms/__init__.py` & `mia-accounting-1.5.6/src/accounting/journal_entry/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/journal_entry/forms/currency.py` & `mia-accounting-1.5.6/src/accounting/journal_entry/forms/currency.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/journal_entry/forms/journal_entry.py` & `mia-accounting-1.5.6/src/accounting/journal_entry/forms/journal_entry.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/journal_entry/forms/line_item.py` & `mia-accounting-1.5.6/src/accounting/journal_entry/forms/line_item.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/journal_entry/forms/reorder.py` & `mia-accounting-1.5.6/src/accounting/journal_entry/forms/reorder.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/journal_entry/template_filters.py` & `mia-accounting-1.5.6/src/accounting/journal_entry/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/journal_entry/utils/__init__.py` & `mia-accounting-1.5.6/src/accounting/journal_entry/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/journal_entry/utils/account_option.py` & `mia-accounting-1.5.6/src/accounting/journal_entry/utils/account_option.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/journal_entry/utils/description_editor.py` & `mia-accounting-1.5.6/src/accounting/journal_entry/utils/description_editor.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/journal_entry/utils/operators.py` & `mia-accounting-1.5.6/src/accounting/journal_entry/utils/operators.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/journal_entry/utils/original_line_items.py` & `mia-accounting-1.5.6/src/accounting/journal_entry/utils/original_line_items.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/journal_entry/views.py` & `mia-accounting-1.5.6/src/accounting/journal_entry/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/locale.py` & `mia-accounting-1.5.6/src/accounting/locale.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/models.py` & `mia-accounting-1.5.6/src/accounting/models.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/option/__init__.py` & `mia-accounting-1.5.6/src/accounting/option/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/option/forms.py` & `mia-accounting-1.5.6/src/accounting/option/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/option/views.py` & `mia-accounting-1.5.6/src/accounting/option/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/report/__init__.py` & `mia-accounting-1.5.6/src/accounting/report/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/report/converters.py` & `mia-accounting-1.5.6/src/accounting/report/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/report/period/__init__.py` & `mia-accounting-1.5.6/src/accounting/report/period/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/report/period/chooser.py` & `mia-accounting-1.5.6/src/accounting/report/period/chooser.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/report/period/description.py` & `mia-accounting-1.5.6/src/accounting/report/period/description.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/report/period/month_end.py` & `mia-accounting-1.5.6/src/accounting/report/period/month_end.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/report/period/parser.py` & `mia-accounting-1.5.6/src/accounting/report/period/parser.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/report/period/period.py` & `mia-accounting-1.5.6/src/accounting/report/period/period.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/report/period/shortcuts.py` & `mia-accounting-1.5.6/src/accounting/report/period/shortcuts.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/report/period/specification.py` & `mia-accounting-1.5.6/src/accounting/report/period/specification.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/report/reports/__init__.py` & `mia-accounting-1.5.6/src/accounting/report/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/report/reports/balance_sheet.py` & `mia-accounting-1.5.6/src/accounting/report/reports/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/report/reports/income_expenses.py` & `mia-accounting-1.5.6/src/accounting/report/reports/income_expenses.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/report/reports/income_statement.py` & `mia-accounting-1.5.6/src/accounting/report/reports/income_statement.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/report/reports/journal.py` & `mia-accounting-1.5.6/src/accounting/report/reports/journal.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/report/reports/ledger.py` & `mia-accounting-1.5.6/src/accounting/report/reports/ledger.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/report/reports/search.py` & `mia-accounting-1.5.6/src/accounting/report/reports/search.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/report/reports/trial_balance.py` & `mia-accounting-1.5.6/src/accounting/report/reports/trial_balance.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/report/reports/unapplied.py` & `mia-accounting-1.5.6/src/accounting/report/reports/unapplied.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/report/reports/unapplied_accounts.py` & `mia-accounting-1.5.6/src/accounting/report/reports/unapplied_accounts.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/report/reports/unmatched.py` & `mia-accounting-1.5.6/src/accounting/report/reports/unmatched.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/report/reports/unmatched_accounts.py` & `mia-accounting-1.5.6/src/accounting/report/reports/unmatched_accounts.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/report/template_filters.py` & `mia-accounting-1.5.6/src/accounting/report/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/report/utils/__init__.py` & `mia-accounting-1.5.6/src/accounting/report/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/report/utils/base_page_params.py` & `mia-accounting-1.5.6/src/accounting/report/utils/base_page_params.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/report/utils/base_report.py` & `mia-accounting-1.5.6/src/accounting/report/utils/base_report.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/report/utils/csv_export.py` & `mia-accounting-1.5.6/src/accounting/report/utils/csv_export.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/report/utils/offset_matcher.py` & `mia-accounting-1.5.6/src/accounting/report/utils/offset_matcher.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/report/utils/option_link.py` & `mia-accounting-1.5.6/src/accounting/report/utils/option_link.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/report/utils/report_chooser.py` & `mia-accounting-1.5.6/src/accounting/report/utils/report_chooser.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/report/utils/report_type.py` & `mia-accounting-1.5.6/src/accounting/report/utils/report_type.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/report/utils/unapplied.py` & `mia-accounting-1.5.6/src/accounting/report/utils/unapplied.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/report/utils/unmatched.py` & `mia-accounting-1.5.6/src/accounting/report/utils/unmatched.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/report/utils/urls.py` & `mia-accounting-1.5.6/src/accounting/report/utils/urls.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/report/views.py` & `mia-accounting-1.5.6/src/accounting/report/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/static/css/style.css` & `mia-accounting-1.5.6/src/accounting/static/css/style.css`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/static/js/account-form.js` & `mia-accounting-1.5.6/src/accounting/static/js/account-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/static/js/account-order.js` & `mia-accounting-1.5.6/src/accounting/static/js/account-order.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/static/js/currency-form.js` & `mia-accounting-1.5.6/src/accounting/static/js/currency-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/static/js/description-editor.js` & `mia-accounting-1.5.6/src/accounting/static/js/description-editor.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/static/js/drag-and-drop-reorder.js` & `mia-accounting-1.5.6/src/accounting/static/js/drag-and-drop-reorder.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/static/js/journal-entry-account-selector.js` & `mia-accounting-1.5.6/src/accounting/static/js/journal-entry-account-selector.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/static/js/journal-entry-form.js` & `mia-accounting-1.5.6/src/accounting/static/js/journal-entry-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/static/js/journal-entry-line-item-editor.js` & `mia-accounting-1.5.6/src/accounting/static/js/journal-entry-line-item-editor.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/static/js/journal-entry-order.js` & `mia-accounting-1.5.6/src/accounting/static/js/journal-entry-order.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/static/js/material-fab-speed-dial.js` & `mia-accounting-1.5.6/src/accounting/static/js/material-fab-speed-dial.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/static/js/option-form.js` & `mia-accounting-1.5.6/src/accounting/static/js/option-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/static/js/original-line-item-selector.js` & `mia-accounting-1.5.6/src/accounting/static/js/original-line-item-selector.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/static/js/period-chooser.js` & `mia-accounting-1.5.6/src/accounting/static/js/period-chooser.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/template_filters.py` & `mia-accounting-1.5.6/src/accounting/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/template_globals.py` & `mia-accounting-1.5.6/src/accounting/template_globals.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/account/create.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/account/create.html`

 * *Files 2% similar despite different names*

```diff
@@ -19,10 +19,10 @@
 Author: imacat@mail.imacat.idv.tw (imacat)
 First written: 2023/2/1
 #}
 {% extends "accounting/account/include/form.html" %}
 
 {% block header %}{% block title %}{{ A_("Add a New Account") }}{% endblock %}{% endblock %}
 
-{% block back_url %}{{ request.args.get("next") or url_for("accounting.account.list") }}{% endblock %}
+{% block back_url %}{{ url_for("accounting.account.list")|accounting_or_next }}{% endblock %}
 
 {% block action_url %}{{ url_for("accounting.account.store") }}{% endblock %}
```

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/account/detail.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/account/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/account/edit.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/account/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/account/include/form.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/account/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/account/list.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/account/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/account/order.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/account/order.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/base-account/detail.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/base-account/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/base-account/list.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/base-account/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/base.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/base.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/currency/create.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/currency/create.html`

 * *Files 4% similar despite different names*

```diff
@@ -19,10 +19,10 @@
 Author: imacat@mail.imacat.idv.tw (imacat)
 First written: 2023/2/6
 #}
 {% extends "accounting/currency/include/form.html" %}
 
 {% block header %}{% block title %}{{ A_("Add a New Currency") }}{% endblock %}{% endblock %}
 
-{% block back_url %}{{ request.args.get("next") or url_for("accounting.currency.list") }}{% endblock %}
+{% block back_url %}{{ url_for("accounting.currency.list")|accounting_or_next }}{% endblock %}
 
 {% block action_url %}{{ url_for("accounting.currency.store") }}{% endblock %}
```

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/currency/detail.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/currency/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/currency/edit.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/currency/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/currency/include/form.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/currency/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/currency/list.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/currency/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/include/nav.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/include/nav.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/include/pagination.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/include/pagination.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/disbursement/create.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/receipt/create.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {#
 The Mia! Accounting Project
-create.html: The cash disbursement journal entry creation form
+create.html: The cash receipt journal entry creation form
 
  Copyright (c) 2023 imacat.
 
  Licensed under the Apache License, Version 2.0 (the "License");
  you may not use this file except in compliance with the License.
  You may obtain a copy of the License at
 
@@ -15,14 +15,14 @@
  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  See the License for the specific language governing permissions and
  limitations under the License.
 
 Author: imacat@mail.imacat.idv.tw (imacat)
 First written: 2023/2/25
 #}
-{% extends "accounting/journal-entry/disbursement/include/form.html" %}
+{% extends "accounting/journal-entry/receipt/include/form.html" %}
 
-{% block header %}{% block title %}{{ A_("Add a New Cash Disbursement Journal Entry") }}{% endblock %}{% endblock %}
+{% block header %}{% block title %}{{ A_("Add a New Cash Receipt Journal Entry") }}{% endblock %}{% endblock %}
 
-{% block back_url %}{{ request.args.get("next") or url_for("accounting-report.default") }}{% endblock %}
+{% block back_url %}{{ url_for("accounting-report.default")|accounting_or_next }}{% endblock %}
 
 {% block action_url %}{{ url_for("accounting.journal-entry.store", journal_entry_type=journal_entry_type) }}{% endblock %}
```

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/disbursement/detail.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/disbursement/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/disbursement/edit.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/disbursement/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/detail.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/form-currency.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/form-line-item.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/form-line-item.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/form.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/order.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/order.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/receipt/create.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/transfer/create.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {#
 The Mia! Accounting Project
-create.html: The cash receipt journal entry creation form
+create.html: The transfer journal entry creation form
 
  Copyright (c) 2023 imacat.
 
  Licensed under the Apache License, Version 2.0 (the "License");
  you may not use this file except in compliance with the License.
  You may obtain a copy of the License at
 
@@ -15,14 +15,14 @@
  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  See the License for the specific language governing permissions and
  limitations under the License.
 
 Author: imacat@mail.imacat.idv.tw (imacat)
 First written: 2023/2/25
 #}
-{% extends "accounting/journal-entry/receipt/include/form.html" %}
+{% extends "accounting/journal-entry/transfer/include/form.html" %}
 
-{% block header %}{% block title %}{{ A_("Add a New Cash Receipt Journal Entry") }}{% endblock %}{% endblock %}
+{% block header %}{% block title %}{{ A_("Add a New Transfer Journal Entry") }}{% endblock %}{% endblock %}
 
-{% block back_url %}{{ request.args.get("next") or url_for("accounting-report.default") }}{% endblock %}
+{% block back_url %}{{ url_for("accounting-report.default")|accounting_or_next }}{% endblock %}
 
 {% block action_url %}{{ url_for("accounting.journal-entry.store", journal_entry_type=journal_entry_type) }}{% endblock %}
```

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/receipt/detail.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/receipt/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/receipt/edit.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/receipt/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/receipt/include/form.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/receipt/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/transfer/create.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/disbursement/create.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {#
 The Mia! Accounting Project
-create.html: The transfer journal entry creation form
+create.html: The cash disbursement journal entry creation form
 
  Copyright (c) 2023 imacat.
 
  Licensed under the Apache License, Version 2.0 (the "License");
  you may not use this file except in compliance with the License.
  You may obtain a copy of the License at
 
@@ -15,14 +15,14 @@
  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  See the License for the specific language governing permissions and
  limitations under the License.
 
 Author: imacat@mail.imacat.idv.tw (imacat)
 First written: 2023/2/25
 #}
-{% extends "accounting/journal-entry/transfer/include/form.html" %}
+{% extends "accounting/journal-entry/disbursement/include/form.html" %}
 
-{% block header %}{% block title %}{{ A_("Add a New Transfer Journal Entry") }}{% endblock %}{% endblock %}
+{% block header %}{% block title %}{{ A_("Add a New Cash Disbursement Journal Entry") }}{% endblock %}{% endblock %}
 
-{% block back_url %}{{ request.args.get("next") or url_for("accounting-report.default") }}{% endblock %}
+{% block back_url %}{{ url_for("accounting-report.default")|accounting_or_next }}{% endblock %}
 
 {% block action_url %}{{ url_for("accounting.journal-entry.store", journal_entry_type=journal_entry_type) }}{% endblock %}
```

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/transfer/detail.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/transfer/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/transfer/edit.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/transfer/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/transfer/include/form.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/journal-entry/transfer/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/option/detail.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/option/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/option/form.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/option/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/option/include/form-recurring-item.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/option/include/form-recurring-item.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/report/balance-sheet.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/report/balance-sheet.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/balance-sheet-section.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/balance-sheet-section.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/ledger-row-desktop.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/ledger-row-desktop.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/ledger-row-mobile.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/ledger-row-mobile.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/period-chooser.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/period-chooser.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/search-modal.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/search-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/toolbar-buttons.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/report/include/toolbar-buttons.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/report/income-expenses.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/report/income-expenses.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/report/income-statement.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/report/income-statement.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/report/journal.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/report/journal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/report/ledger.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/report/ledger.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/report/search.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/report/search.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/report/trial-balance.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/report/trial-balance.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/report/unapplied-accounts.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/report/unapplied-accounts.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/report/unapplied.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/report/unapplied.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/report/unmatched-accounts.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/report/unmatched-accounts.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/templates/accounting/report/unmatched.html` & `mia-accounting-1.5.6/src/accounting/templates/accounting/report/unmatched.html`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
   <button class="btn btn-primary" type="button" data-bs-toggle="modal" data-bs-target="#accounting-match-modal">
     <i class="fa-solid fa-link"></i>
     {{ A_("Match") }}
   </button>
 
   <form action="{{ url_for("accounting-report.match-offsets", currency=report.currency, account=report.account) }}" method="post">
     <input type="hidden" name="csrf_token" value="{{ csrf_token() }}">
-    <input type="hidden" name="next" value="{{ request.full_path if request.query_string else request.path }}">
+    <input type="hidden" name="next" value="{{ accounting_as_next() }}">
     <div class="modal fade" id="accounting-match-modal" tabindex="-1" aria-labelledby="accounting-match-modal-label" aria-hidden="true">
       <div class="modal-dialog">
         <div class="modal-content">
           <div class="modal-header">
             <h1 class="modal-title fs-5" id="accounting-match-modal-label">{{ A_("Confirm Match Offsets") }}</h1>
             <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="{{ A_("Close") }}"></button>
           </div>
```

### Comparing `mia-accounting-1.5.5/src/accounting/translations/accounting.pot` & `mia-accounting-1.5.6/src/accounting/translations/accounting.pot`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo` & `mia-accounting-1.5.6/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po` & `mia-accounting-1.5.6/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo` & `mia-accounting-1.5.6/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po` & `mia-accounting-1.5.6/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/utils/__init__.py` & `mia-accounting-1.5.6/src/accounting/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/utils/cast.py` & `mia-accounting-1.5.6/src/accounting/utils/cast.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/utils/current_account.py` & `mia-accounting-1.5.6/src/accounting/utils/current_account.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/utils/flash_errors.py` & `mia-accounting-1.5.6/src/accounting/utils/flash_errors.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/utils/journal_entry_types.py` & `mia-accounting-1.5.6/src/accounting/utils/journal_entry_types.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/utils/next_uri.py` & `mia-accounting-1.5.6/src/accounting/utils/next_uri.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,23 @@
 from urllib.parse import urlparse, parse_qsl, ParseResult, urlencode, \
     urlunparse
 
 from flask import request, Blueprint, current_app
 from itsdangerous import URLSafeSerializer, BadData
 
 
+def __as_next() -> str:
+    """Encodes the current request URI as value for the next URI.
+
+    :return: The current request URI as value for the next URI.
+    """
+    return encode_next(
+        request.full_path if request.query_string else request.path)
+
+
 def append_next(uri: str) -> str:
     """Appends the current URI as the next URI to the query argument.
 
     :param uri: The URI.
     :return: The URI with the current URI appended as the next URI.
     """
     next_uri: str = request.full_path if request.query_string else request.path
@@ -100,10 +109,11 @@
 
 def init_app(bp: Blueprint) -> None:
     """Initializes the application.
 
     :param bp: The blueprint of the accounting application.
     :return: None.
     """
+    bp.add_app_template_global(__as_next, "accounting_as_next")
     bp.add_app_template_filter(append_next, "accounting_append_next")
     bp.add_app_template_filter(inherit_next, "accounting_inherit_next")
     bp.add_app_template_filter(or_next, "accounting_or_next")
```

### Comparing `mia-accounting-1.5.5/src/accounting/utils/offset_alias.py` & `mia-accounting-1.5.6/src/accounting/utils/offset_alias.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/utils/options.py` & `mia-accounting-1.5.6/src/accounting/utils/options.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/utils/pagination.py` & `mia-accounting-1.5.6/src/accounting/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/utils/permission.py` & `mia-accounting-1.5.6/src/accounting/utils/permission.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/utils/query.py` & `mia-accounting-1.5.6/src/accounting/utils/query.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/utils/random_id.py` & `mia-accounting-1.5.6/src/accounting/utils/random_id.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/utils/strip_text.py` & `mia-accounting-1.5.6/src/accounting/utils/strip_text.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/accounting/utils/user.py` & `mia-accounting-1.5.6/src/accounting/utils/user.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/src/mia_accounting.egg-info/PKG-INFO` & `mia-accounting-1.5.6/src/mia_accounting.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mia-accounting
-Version: 1.5.5
+Version: 1.5.6
 Summary: A Flask accounting module.
 Author-email: imacat <imacat@mail.imacat.idv.tw>
 Project-URL: Documentation, https://mia-accounting.readthedocs.io
 Project-URL: Change Log, https://mia-accounting.readthedocs.io/en/latest/changelog.html
 Project-URL: Repository, https://github.com/imacat/mia-accounting
 Project-URL: Bug Tracker, https://github.com/imacat/mia-accounting/issues
 Project-URL: Demonstration, https://accounting.imacat.idv.tw
```

### Comparing `mia-accounting-1.5.5/src/mia_accounting.egg-info/SOURCES.txt` & `mia-accounting-1.5.6/src/mia_accounting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/tests/babel-utils-test-site.py` & `mia-accounting-1.5.6/tests/babel-utils-test-site.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/tests/babel-utils.py` & `mia-accounting-1.5.6/tests/babel-utils.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/tests/test_account.py` & `mia-accounting-1.5.6/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/tests/test_base_account.py` & `mia-accounting-1.5.6/tests/test_base_account.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/tests/test_commands.py` & `mia-accounting-1.5.6/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/tests/test_currency.py` & `mia-accounting-1.5.6/tests/test_currency.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/tests/test_description_editor.py` & `mia-accounting-1.5.6/tests/test_description_editor.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/tests/test_journal_entry.py` & `mia-accounting-1.5.6/tests/test_journal_entry.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/tests/test_offset.py` & `mia-accounting-1.5.6/tests/test_offset.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/tests/test_option.py` & `mia-accounting-1.5.6/tests/test_option.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/tests/test_report.py` & `mia-accounting-1.5.6/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/tests/test_site/__init__.py` & `mia-accounting-1.5.6/tests/test_site/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,15 +64,14 @@
         app.config["TESTING"] = True
 
     babel_js.init_app(app)
     csrf.init_app(app)
     db.init_app(app)
 
     app.register_blueprint(bp, url_prefix="/")
-    app.add_template_global(__as_next, "accounting_as_next")
 
     from . import locale
     locale.init_app(app)
 
     from . import auth
     auth.init_app(app)
 
@@ -145,16 +144,7 @@
 @bp.get("/", endpoint="home")
 def get_home() -> str:
     """Returns the home page.
 
     :return: The home page.
     """
     return render_template("home.html")
-
-
-def __as_next() -> str:
-    """Encodes the current request URI as value for the next URI.
-
-    :return: The current request URI as value for the next URI.
-    """
-    return encode_next(
-        request.full_path if request.query_string else request.path)
```

### Comparing `mia-accounting-1.5.5/tests/test_site/auth.py` & `mia-accounting-1.5.6/tests/test_site/auth.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/tests/test_site/lib.py` & `mia-accounting-1.5.6/tests/test_site/lib.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/tests/test_site/locale.py` & `mia-accounting-1.5.6/tests/test_site/locale.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/tests/test_site/reset.py` & `mia-accounting-1.5.6/tests/test_site/reset.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/tests/test_site/static/favicon.svg` & `mia-accounting-1.5.6/tests/test_site/static/favicon.svg`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/tests/test_site/templates/base.html` & `mia-accounting-1.5.6/tests/test_site/templates/base.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/tests/test_site/templates/home.html` & `mia-accounting-1.5.6/tests/test_site/templates/home.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/tests/test_site/templates/login.html` & `mia-accounting-1.5.6/tests/test_site/templates/login.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/tests/test_site/templates/reset.html` & `mia-accounting-1.5.6/tests/test_site/templates/reset.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/tests/test_site/translations/messages.pot` & `mia-accounting-1.5.6/tests/test_site/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo` & `mia-accounting-1.5.6/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po` & `mia-accounting-1.5.6/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo` & `mia-accounting-1.5.6/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po` & `mia-accounting-1.5.6/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/tests/test_unmatched_offset.py` & `mia-accounting-1.5.6/tests/test_unmatched_offset.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/tests/test_utils.py` & `mia-accounting-1.5.6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/tests/testlib.py` & `mia-accounting-1.5.6/tests/testlib.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.5/tests/testlib_journal_entry.py` & `mia-accounting-1.5.6/tests/testlib_journal_entry.py`

 * *Files identical despite different names*

