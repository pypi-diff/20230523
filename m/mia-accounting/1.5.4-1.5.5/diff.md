# Comparing `tmp/mia-accounting-1.5.4.tar.gz` & `tmp/mia-accounting-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mia-accounting-1.5.4.tar", last modified: Wed May 17 16:11:23 2023, max compression
+gzip compressed data, was "mia-accounting-1.5.5.tar", last modified: Tue May 23 00:45:05 2023, max compression
```

## Comparing `mia-accounting-1.5.4.tar` & `mia-accounting-1.5.5.tar`

### file list

```diff
@@ -1,305 +1,305 @@
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:23.422509 mia-accounting-1.5.4/
--rw-r--r--   0 imacat    (1000) users      (100)    11358 2015-02-17 18:06:12.000000 mia-accounting-1.5.4/LICENSE
--rw-r--r--   0 imacat    (1000) users      (100)     1070 2023-04-05 11:25:31.000000 mia-accounting-1.5.4/MANIFEST.in
--rw-r--r--   0 imacat    (1000) users      (100)     3412 2023-05-17 16:11:23.418509 mia-accounting-1.5.4/PKG-INFO
--rw-r--r--   0 imacat    (1000) users      (100)     2525 2023-04-23 12:04:20.000000 mia-accounting-1.5.4/README.rst
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:20.566549 mia-accounting-1.5.4/docs/
--rw-r--r--   0 imacat    (1000) users      (100)      638 2023-01-27 04:20:04.000000 mia-accounting-1.5.4/docs/Makefile
--rw-r--r--   0 imacat    (1000) users      (100)      804 2023-01-27 04:20:04.000000 mia-accounting-1.5.4/docs/make.bat
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.838531 mia-accounting-1.5.4/docs/source/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.894530 mia-accounting-1.5.4/docs/source/_static/
--rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:08.000000 mia-accounting-1.5.4/docs/source/_static/.keep
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.894530 mia-accounting-1.5.4/docs/source/_templates/
--rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:11.000000 mia-accounting-1.5.4/docs/source/_templates/.keep
--rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-18 01:25:56.000000 mia-accounting-1.5.4/docs/source/accounting.account.rst
--rw-r--r--   0 imacat    (1000) users      (100)      959 2023-04-18 01:25:56.000000 mia-accounting-1.5.4/docs/source/accounting.base_account.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1053 2023-04-18 01:25:56.000000 mia-accounting-1.5.4/docs/source/accounting.currency.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1089 2023-04-18 01:25:56.000000 mia-accounting-1.5.4/docs/source/accounting.journal_entry.forms.rst
--rw-r--r--   0 imacat    (1000) users      (100)      937 2023-04-18 01:25:56.000000 mia-accounting-1.5.4/docs/source/accounting.journal_entry.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1162 2023-04-18 01:25:56.000000 mia-accounting-1.5.4/docs/source/accounting.journal_entry.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)      513 2023-04-18 01:25:56.000000 mia-accounting-1.5.4/docs/source/accounting.option.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1551 2023-04-18 01:25:56.000000 mia-accounting-1.5.4/docs/source/accounting.report.period.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2460 2023-04-18 01:32:44.000000 mia-accounting-1.5.4/docs/source/accounting.report.reports.rst
--rw-r--r--   0 imacat    (1000) users      (100)      861 2023-04-18 01:25:56.000000 mia-accounting-1.5.4/docs/source/accounting.report.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2168 2023-04-18 01:32:44.000000 mia-accounting-1.5.4/docs/source/accounting.report.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1301 2023-04-18 01:32:44.000000 mia-accounting-1.5.4/docs/source/accounting.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2405 2023-04-18 01:32:44.000000 mia-accounting-1.5.4/docs/source/accounting.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)     8083 2023-05-17 16:05:22.000000 mia-accounting-1.5.4/docs/source/changelog.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1051 2023-04-23 12:12:53.000000 mia-accounting-1.5.4/docs/source/conf.py
--rw-r--r--   0 imacat    (1000) users      (100)     1508 2023-04-06 00:38:39.000000 mia-accounting-1.5.4/docs/source/examples.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2837 2023-04-06 00:21:32.000000 mia-accounting-1.5.4/docs/source/history.rst
--rw-r--r--   0 imacat    (1000) users      (100)      521 2023-04-23 12:04:21.000000 mia-accounting-1.5.4/docs/source/index.rst
--rw-r--r--   0 imacat    (1000) users      (100)     3568 2023-05-06 15:58:29.000000 mia-accounting-1.5.4/docs/source/intro.rst
--rw-r--r--   0 imacat    (1000) users      (100)       53 2023-04-04 10:25:53.000000 mia-accounting-1.5.4/docs/source/modules.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1994 2023-05-09 00:42:23.000000 mia-accounting-1.5.4/pyproject.toml
--rw-r--r--   0 imacat    (1000) users      (100)       38 2023-05-17 16:11:23.422509 mia-accounting-1.5.4/setup.cfg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:20.322552 mia-accounting-1.5.4/src/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.898530 mia-accounting-1.5.4/src/accounting/
--rw-r--r--   0 imacat    (1000) users      (100)     3045 2023-05-17 14:58:29.000000 mia-accounting-1.5.4/src/accounting/__init__.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.902530 mia-accounting-1.5.4/src/accounting/account/
--rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-10 15:59:48.000000 mia-accounting-1.5.4/src/accounting/account/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3868 2023-04-29 21:45:45.000000 mia-accounting-1.5.4/src/accounting/account/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1512 2023-04-04 09:21:35.000000 mia-accounting-1.5.4/src/accounting/account/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     7145 2023-04-04 09:21:33.000000 mia-accounting-1.5.4/src/accounting/account/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     2209 2023-04-04 09:21:35.000000 mia-accounting-1.5.4/src/accounting/account/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     7416 2023-04-09 02:08:22.000000 mia-accounting-1.5.4/src/accounting/account/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.902530 mia-accounting-1.5.4/src/accounting/base_account/
--rw-r--r--   0 imacat    (1000) users      (100)     1240 2023-04-10 15:59:48.000000 mia-accounting-1.5.4/src/accounting/base_account/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     1800 2023-04-10 15:59:48.000000 mia-accounting-1.5.4/src/accounting/base_account/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1592 2023-04-04 09:21:35.000000 mia-accounting-1.5.4/src/accounting/base_account/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     1769 2023-04-04 09:21:37.000000 mia-accounting-1.5.4/src/accounting/base_account/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     1812 2023-04-09 02:08:22.000000 mia-accounting-1.5.4/src/accounting/base_account/views.py
--rw-r--r--   0 imacat    (1000) users      (100)     2138 2023-04-10 15:59:48.000000 mia-accounting-1.5.4/src/accounting/commands.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.906530 mia-accounting-1.5.4/src/accounting/currency/
--rw-r--r--   0 imacat    (1000) users      (100)     1312 2023-04-10 15:59:48.000000 mia-accounting-1.5.4/src/accounting/currency/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     2206 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/currency/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1556 2023-04-04 09:21:35.000000 mia-accounting-1.5.4/src/accounting/currency/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     3172 2023-04-04 09:21:36.000000 mia-accounting-1.5.4/src/accounting/currency/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     1720 2023-04-04 09:21:34.000000 mia-accounting-1.5.4/src/accounting/currency/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     6609 2023-04-09 02:08:22.000000 mia-accounting-1.5.4/src/accounting/currency/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.906530 mia-accounting-1.5.4/src/accounting/data/
--rw-r--r--   0 imacat    (1000) users      (100)    36368 2023-03-14 01:04:26.000000 mia-accounting-1.5.4/src/accounting/data/base_accounts.csv
--rw-r--r--   0 imacat    (1000) users      (100)      370 2023-03-14 01:04:26.000000 mia-accounting-1.5.4/src/accounting/data/currencies.csv
--rw-r--r--   0 imacat    (1000) users      (100)     3144 2023-04-04 09:21:33.000000 mia-accounting-1.5.4/src/accounting/forms.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.910530 mia-accounting-1.5.4/src/accounting/journal_entry/
--rw-r--r--   0 imacat    (1000) users      (100)     1376 2023-04-04 09:21:35.000000 mia-accounting-1.5.4/src/accounting/journal_entry/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3302 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/journal_entry/converters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.914530 mia-accounting-1.5.4/src/accounting/journal_entry/forms/
--rw-r--r--   0 imacat    (1000) users      (100)      934 2023-04-04 09:21:37.000000 mia-accounting-1.5.4/src/accounting/journal_entry/forms/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)    11003 2023-04-23 05:21:41.000000 mia-accounting-1.5.4/src/accounting/journal_entry/forms/currency.py
--rw-r--r--   0 imacat    (1000) users      (100)    24568 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/journal_entry/forms/journal_entry.py
--rw-r--r--   0 imacat    (1000) users      (100)    19807 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/journal_entry/forms/line_item.py
--rw-r--r--   0 imacat    (1000) users      (100)     3291 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/journal_entry/forms/reorder.py
--rw-r--r--   0 imacat    (1000) users      (100)     2535 2023-04-04 09:21:32.000000 mia-accounting-1.5.4/src/accounting/journal_entry/template_filters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.914530 mia-accounting-1.5.4/src/accounting/journal_entry/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      729 2023-04-04 09:21:32.000000 mia-accounting-1.5.4/src/accounting/journal_entry/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     1802 2023-04-17 23:37:17.000000 mia-accounting-1.5.4/src/accounting/journal_entry/utils/account_option.py
--rw-r--r--   0 imacat    (1000) users      (100)    12981 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/journal_entry/utils/description_editor.py
--rw-r--r--   0 imacat    (1000) users      (100)    12676 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/journal_entry/utils/operators.py
--rw-r--r--   0 imacat    (1000) users      (100)     3722 2023-04-23 05:21:41.000000 mia-accounting-1.5.4/src/accounting/journal_entry/utils/original_line_items.py
--rw-r--r--   0 imacat    (1000) users      (100)     9351 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/journal_entry/views.py
--rw-r--r--   0 imacat    (1000) users      (100)     3809 2023-04-04 09:21:33.000000 mia-accounting-1.5.4/src/accounting/locale.py
--rw-r--r--   0 imacat    (1000) users      (100)    32618 2023-04-30 07:03:58.000000 mia-accounting-1.5.4/src/accounting/models.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.918530 mia-accounting-1.5.4/src/accounting/option/
--rw-r--r--   0 imacat    (1000) users      (100)      993 2023-04-04 09:21:35.000000 mia-accounting-1.5.4/src/accounting/option/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     9762 2023-04-08 00:27:23.000000 mia-accounting-1.5.4/src/accounting/option/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     2827 2023-04-04 09:21:32.000000 mia-accounting-1.5.4/src/accounting/option/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.918530 mia-accounting-1.5.4/src/accounting/report/
--rw-r--r--   0 imacat    (1000) users      (100)     1362 2023-04-08 10:12:56.000000 mia-accounting-1.5.4/src/accounting/report/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-08 10:12:56.000000 mia-accounting-1.5.4/src/accounting/report/converters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.922530 mia-accounting-1.5.4/src/accounting/report/period/
--rw-r--r--   0 imacat    (1000) users      (100)      793 2023-04-04 09:21:32.000000 mia-accounting-1.5.4/src/accounting/report/period/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3702 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/report/period/chooser.py
--rw-r--r--   0 imacat    (1000) users      (100)     5557 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/report/period/description.py
--rw-r--r--   0 imacat    (1000) users      (100)     1050 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/report/period/month_end.py
--rw-r--r--   0 imacat    (1000) users      (100)     4127 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/report/period/parser.py
--rw-r--r--   0 imacat    (1000) users      (100)     4522 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/report/period/period.py
--rw-r--r--   0 imacat    (1000) users      (100)     4785 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/report/period/shortcuts.py
--rw-r--r--   0 imacat    (1000) users      (100)     3915 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/report/period/specification.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.926530 mia-accounting-1.5.4/src/accounting/report/reports/
--rw-r--r--   0 imacat    (1000) users      (100)      946 2023-04-04 09:21:36.000000 mia-accounting-1.5.4/src/accounting/report/reports/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)    17920 2023-04-06 01:50:58.000000 mia-accounting-1.5.4/src/accounting/report/reports/balance_sheet.py
--rw-r--r--   0 imacat    (1000) users      (100)    18807 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/report/reports/income_expenses.py
--rw-r--r--   0 imacat    (1000) users      (100)    11733 2023-04-06 01:50:58.000000 mia-accounting-1.5.4/src/accounting/report/reports/income_statement.py
--rw-r--r--   0 imacat    (1000) users      (100)     8130 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/report/reports/journal.py
--rw-r--r--   0 imacat    (1000) users      (100)    16530 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/report/reports/ledger.py
--rw-r--r--   0 imacat    (1000) users      (100)     8472 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/report/reports/search.py
--rw-r--r--   0 imacat    (1000) users      (100)     8853 2023-04-06 01:50:58.000000 mia-accounting-1.5.4/src/accounting/report/reports/trial_balance.py
--rw-r--r--   0 imacat    (1000) users      (100)     8099 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/report/reports/unapplied.py
--rw-r--r--   0 imacat    (1000) users      (100)     5210 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/report/reports/unapplied_accounts.py
--rw-r--r--   0 imacat    (1000) users      (100)     8169 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/report/reports/unmatched.py
--rw-r--r--   0 imacat    (1000) users      (100)     5191 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/report/reports/unmatched_accounts.py
--rw-r--r--   0 imacat    (1000) users      (100)     1205 2023-04-04 09:21:33.000000 mia-accounting-1.5.4/src/accounting/report/template_filters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.926530 mia-accounting-1.5.4/src/accounting/report/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      711 2023-04-04 09:21:34.000000 mia-accounting-1.5.4/src/accounting/report/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3034 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/report/utils/base_page_params.py
--rw-r--r--   0 imacat    (1000) users      (100)     1143 2023-04-04 09:21:36.000000 mia-accounting-1.5.4/src/accounting/report/utils/base_report.py
--rw-r--r--   0 imacat    (1000) users      (100)     3334 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/report/utils/csv_export.py
--rw-r--r--   0 imacat    (1000) users      (100)     7321 2023-04-29 22:38:16.000000 mia-accounting-1.5.4/src/accounting/report/utils/offset_matcher.py
--rw-r--r--   0 imacat    (1000) users      (100)     1368 2023-04-04 09:21:37.000000 mia-accounting-1.5.4/src/accounting/report/utils/option_link.py
--rw-r--r--   0 imacat    (1000) users      (100)     7881 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/report/utils/report_chooser.py
--rw-r--r--   0 imacat    (1000) users      (100)     1371 2023-04-17 08:41:57.000000 mia-accounting-1.5.4/src/accounting/report/utils/report_type.py
--rw-r--r--   0 imacat    (1000) users      (100)     4385 2023-04-23 05:21:41.000000 mia-accounting-1.5.4/src/accounting/report/utils/unapplied.py
--rw-r--r--   0 imacat    (1000) users      (100)     2221 2023-04-23 05:21:41.000000 mia-accounting-1.5.4/src/accounting/report/utils/unmatched.py
--rw-r--r--   0 imacat    (1000) users      (100)     5440 2023-04-18 00:59:05.000000 mia-accounting-1.5.4/src/accounting/report/utils/urls.py
--rw-r--r--   0 imacat    (1000) users      (100)    14167 2023-04-18 01:14:44.000000 mia-accounting-1.5.4/src/accounting/report/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:20.322552 mia-accounting-1.5.4/src/accounting/static/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.930530 mia-accounting-1.5.4/src/accounting/static/css/
--rw-r--r--   0 imacat    (1000) users      (100)    13431 2023-04-18 00:10:33.000000 mia-accounting-1.5.4/src/accounting/static/css/style.css
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.930530 mia-accounting-1.5.4/src/accounting/static/js/
--rw-r--r--   0 imacat    (1000) users      (100)    10921 2023-04-04 10:05:35.000000 mia-accounting-1.5.4/src/accounting/static/js/account-form.js
--rw-r--r--   0 imacat    (1000) users      (100)     1599 2023-04-04 10:05:35.000000 mia-accounting-1.5.4/src/accounting/static/js/account-order.js
--rw-r--r--   0 imacat    (1000) users      (100)     4955 2023-04-04 10:05:35.000000 mia-accounting-1.5.4/src/accounting/static/js/currency-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    38865 2023-04-17 23:44:56.000000 mia-accounting-1.5.4/src/accounting/static/js/description-editor.js
--rw-r--r--   0 imacat    (1000) users      (100)     3564 2023-04-04 10:05:35.000000 mia-accounting-1.5.4/src/accounting/static/js/drag-and-drop-reorder.js
--rw-r--r--   0 imacat    (1000) users      (100)     9211 2023-04-17 23:32:14.000000 mia-accounting-1.5.4/src/accounting/static/js/journal-entry-account-selector.js
--rw-r--r--   0 imacat    (1000) users      (100)    33086 2023-04-17 23:52:58.000000 mia-accounting-1.5.4/src/accounting/static/js/journal-entry-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    19665 2023-04-30 07:03:59.000000 mia-accounting-1.5.4/src/accounting/static/js/journal-entry-line-item-editor.js
--rw-r--r--   0 imacat    (1000) users      (100)     1366 2023-04-04 10:05:35.000000 mia-accounting-1.5.4/src/accounting/static/js/journal-entry-order.js
--rw-r--r--   0 imacat    (1000) users      (100)     1436 2023-04-04 10:05:35.000000 mia-accounting-1.5.4/src/accounting/static/js/material-fab-speed-dial.js
--rw-r--r--   0 imacat    (1000) users      (100)    28660 2023-04-04 10:05:35.000000 mia-accounting-1.5.4/src/accounting/static/js/option-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    11670 2023-04-17 23:40:31.000000 mia-accounting-1.5.4/src/accounting/static/js/original-line-item-selector.js
--rw-r--r--   0 imacat    (1000) users      (100)    10374 2023-04-04 10:05:35.000000 mia-accounting-1.5.4/src/accounting/static/js/period-chooser.js
--rw-r--r--   0 imacat    (1000) users      (100)     2712 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/template_filters.py
--rw-r--r--   0 imacat    (1000) users      (100)     1137 2023-04-23 01:43:59.000000 mia-accounting-1.5.4/src/accounting/template_globals.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:20.322552 mia-accounting-1.5.4/src/accounting/templates/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.930530 mia-accounting-1.5.4/src/accounting/templates/accounting/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.934529 mia-accounting-1.5.4/src/accounting/templates/accounting/account/
--rw-r--r--   0 imacat    (1000) users      (100)     1034 2023-04-04 10:04:10.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/account/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     4266 2023-04-04 10:04:11.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/account/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1081 2023-04-04 10:04:11.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/account/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.934529 mia-accounting-1.5.4/src/accounting/templates/accounting/account/include/
--rw-r--r--   0 imacat    (1000) users      (100)     5704 2023-04-04 10:04:10.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/account/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     2734 2023-05-17 13:41:19.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/account/list.html
--rw-r--r--   0 imacat    (1000) users      (100)     3052 2023-04-04 10:04:12.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/account/order.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.934529 mia-accounting-1.5.4/src/accounting/templates/accounting/base-account/
--rw-r--r--   0 imacat    (1000) users      (100)     1581 2023-04-04 10:04:10.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/base-account/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     2095 2023-05-17 13:41:20.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/base-account/list.html
--rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-04 10:04:10.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/base.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.934529 mia-accounting-1.5.4/src/accounting/templates/accounting/currency/
--rw-r--r--   0 imacat    (1000) users      (100)     1039 2023-04-04 10:04:12.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/currency/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     3883 2023-04-04 10:04:10.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/currency/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1152 2023-04-04 10:04:11.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/currency/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.934529 mia-accounting-1.5.4/src/accounting/templates/accounting/currency/include/
--rw-r--r--   0 imacat    (1000) users      (100)     2850 2023-04-04 10:04:10.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/currency/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     2606 2023-05-17 13:41:19.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/currency/list.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.934529 mia-accounting-1.5.4/src/accounting/templates/accounting/include/
--rw-r--r--   0 imacat    (1000) users      (100)     2706 2023-04-17 15:07:31.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/include/nav.html
--rw-r--r--   0 imacat    (1000) users      (100)     1986 2023-04-04 10:04:11.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/include/pagination.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.934529 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.934529 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/disbursement/
--rw-r--r--   0 imacat    (1000) users      (100)     1149 2023-04-04 23:56:52.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/disbursement/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2028 2023-04-04 10:04:11.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/disbursement/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1213 2023-04-04 10:04:09.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/disbursement/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.934529 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/disbursement/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1195 2023-04-04 10:04:10.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2283 2023-04-04 10:04:12.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.938529 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/
--rw-r--r--   0 imacat    (1000) users      (100)     3406 2023-04-17 23:32:14.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)    14521 2023-05-17 13:55:39.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     3242 2023-04-17 23:11:57.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html
--rw-r--r--   0 imacat    (1000) users      (100)     4554 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     2726 2023-04-04 10:04:10.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html
--rw-r--r--   0 imacat    (1000) users      (100)     6442 2023-04-17 23:54:15.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/form-line-item.html
--rw-r--r--   0 imacat    (1000) users      (100)     4370 2023-04-04 10:04:12.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     4191 2023-05-17 13:55:40.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     2093 2023-04-04 10:04:11.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html
--rw-r--r--   0 imacat    (1000) users      (100)     3791 2023-04-18 00:10:33.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     3069 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/order.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.938529 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/receipt/
--rw-r--r--   0 imacat    (1000) users      (100)     1134 2023-04-04 23:56:52.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/receipt/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2025 2023-04-04 10:04:12.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/receipt/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-04 10:04:11.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/receipt/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.938529 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/receipt/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1194 2023-04-04 10:04:12.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2278 2023-04-04 10:04:11.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/receipt/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.938529 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/transfer/
--rw-r--r--   0 imacat    (1000) users      (100)     1127 2023-04-04 23:56:52.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/transfer/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2691 2023-04-04 10:04:09.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/transfer/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1200 2023-04-04 10:04:10.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/transfer/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.942529 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/transfer/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1649 2023-04-04 10:04:11.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2845 2023-04-04 10:04:12.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/transfer/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.942529 mia-accounting-1.5.4/src/accounting/templates/accounting/option/
--rw-r--r--   0 imacat    (1000) users      (100)     2765 2023-04-08 10:12:54.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/option/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     4699 2023-04-08 00:27:23.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/option/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.942529 mia-accounting-1.5.4/src/accounting/templates/accounting/option/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1851 2023-04-04 10:04:10.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html
--rw-r--r--   0 imacat    (1000) users      (100)     3214 2023-04-04 10:04:12.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/option/include/form-recurring-item.html
--rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-04 10:04:12.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     4305 2023-05-17 13:55:39.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.942529 mia-accounting-1.5.4/src/accounting/templates/accounting/report/
--rw-r--r--   0 imacat    (1000) users      (100)     5435 2023-04-18 00:39:27.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/balance-sheet.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:21.942529 mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1970 2023-04-04 10:04:12.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html
--rw-r--r--   0 imacat    (1000) users      (100)     1708 2023-04-04 10:04:12.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/balance-sheet-section.html
--rw-r--r--   0 imacat    (1000) users      (100)     1281 2023-04-04 10:04:10.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html
--rw-r--r--   0 imacat    (1000) users      (100)     1760 2023-04-04 10:04:12.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html
--rw-r--r--   0 imacat    (1000) users      (100)     1252 2023-04-04 10:04:11.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/ledger-row-desktop.html
--rw-r--r--   0 imacat    (1000) users      (100)     1429 2023-04-04 10:04:10.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/ledger-row-mobile.html
--rw-r--r--   0 imacat    (1000) users      (100)     8857 2023-04-04 10:04:12.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/period-chooser.html
--rw-r--r--   0 imacat    (1000) users      (100)     1963 2023-05-17 13:41:20.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/search-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     5630 2023-05-17 13:41:20.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/toolbar-buttons.html
--rw-r--r--   0 imacat    (1000) users      (100)     4841 2023-04-18 00:34:44.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/income-expenses.html
--rw-r--r--   0 imacat    (1000) users      (100)     4618 2023-04-18 00:37:47.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/income-statement.html
--rw-r--r--   0 imacat    (1000) users      (100)     4202 2023-04-04 10:04:10.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/journal.html
--rw-r--r--   0 imacat    (1000) users      (100)     4946 2023-04-18 00:33:38.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/ledger.html
--rw-r--r--   0 imacat    (1000) users      (100)     4044 2023-04-04 10:04:11.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/search.html
--rw-r--r--   0 imacat    (1000) users      (100)     3710 2023-04-18 00:36:16.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/trial-balance.html
--rw-r--r--   0 imacat    (1000) users      (100)     3037 2023-04-18 00:59:05.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/unapplied-accounts.html
--rw-r--r--   0 imacat    (1000) users      (100)     3843 2023-04-18 00:59:06.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/unapplied.html
--rw-r--r--   0 imacat    (1000) users      (100)     3034 2023-04-18 00:59:05.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/unmatched-accounts.html
--rw-r--r--   0 imacat    (1000) users      (100)     6998 2023-04-18 00:59:05.000000 mia-accounting-1.5.4/src/accounting/templates/accounting/report/unmatched.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:22.186526 mia-accounting-1.5.4/src/accounting/translations/
--rw-r--r--   0 imacat    (1000) users      (100)    49437 2023-04-18 01:32:01.000000 mia-accounting-1.5.4/src/accounting/translations/accounting.pot
--rw-r--r--   0 imacat    (1000) users      (100)       80 2023-01-27 03:33:36.000000 mia-accounting-1.5.4/src/accounting/translations/babel.cfg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:20.322552 mia-accounting-1.5.4/src/accounting/translations/zh_Hans/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:22.286525 mia-accounting-1.5.4/src/accounting/translations/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)    16202 2023-04-18 01:32:11.000000 mia-accounting-1.5.4/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo
--rw-r--r--   0 imacat    (1000) users      (100)    54246 2023-04-18 01:32:11.000000 mia-accounting-1.5.4/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:20.322552 mia-accounting-1.5.4/src/accounting/translations/zh_Hant/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:22.542521 mia-accounting-1.5.4/src/accounting/translations/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)    16202 2023-04-18 01:32:11.000000 mia-accounting-1.5.4/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo
--rw-r--r--   0 imacat    (1000) users      (100)    54246 2023-04-18 01:32:11.000000 mia-accounting-1.5.4/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:22.754518 mia-accounting-1.5.4/src/accounting/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      778 2023-04-04 09:21:31.000000 mia-accounting-1.5.4/src/accounting/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     1036 2023-05-17 07:33:36.000000 mia-accounting-1.5.4/src/accounting/utils/cast.py
--rw-r--r--   0 imacat    (1000) users      (100)     3325 2023-05-04 01:35:20.000000 mia-accounting-1.5.4/src/accounting/utils/current_account.py
--rw-r--r--   0 imacat    (1000) users      (100)     1426 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/utils/flash_errors.py
--rw-r--r--   0 imacat    (1000) users      (100)     1030 2023-04-04 09:21:32.000000 mia-accounting-1.5.4/src/accounting/utils/journal_entry_types.py
--rw-r--r--   0 imacat    (1000) users      (100)     3086 2023-05-17 08:11:10.000000 mia-accounting-1.5.4/src/accounting/utils/next_uri.py
--rw-r--r--   0 imacat    (1000) users      (100)     1198 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/utils/offset_alias.py
--rw-r--r--   0 imacat    (1000) users      (100)     6906 2023-04-08 10:12:55.000000 mia-accounting-1.5.4/src/accounting/utils/options.py
--rw-r--r--   0 imacat    (1000) users      (100)    11745 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/utils/pagination.py
--rw-r--r--   0 imacat    (1000) users      (100)     4262 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/utils/permission.py
--rw-r--r--   0 imacat    (1000) users      (100)     1638 2023-04-04 09:21:34.000000 mia-accounting-1.5.4/src/accounting/utils/query.py
--rw-r--r--   0 imacat    (1000) users      (100)     1221 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/utils/random_id.py
--rw-r--r--   0 imacat    (1000) users      (100)     1396 2023-04-04 09:21:37.000000 mia-accounting-1.5.4/src/accounting/utils/strip_text.py
--rw-r--r--   0 imacat    (1000) users      (100)     4985 2023-04-29 21:45:46.000000 mia-accounting-1.5.4/src/accounting/utils/user.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:22.754518 mia-accounting-1.5.4/src/mia_accounting.egg-info/
--rw-r--r--   0 imacat    (1000) users      (100)     3412 2023-05-17 16:11:20.000000 mia-accounting-1.5.4/src/mia_accounting.egg-info/PKG-INFO
--rw-r--r--   0 imacat    (1000) users      (100)    11434 2023-05-17 16:11:20.000000 mia-accounting-1.5.4/src/mia_accounting.egg-info/SOURCES.txt
--rw-r--r--   0 imacat    (1000) users      (100)        1 2023-05-17 16:11:20.000000 mia-accounting-1.5.4/src/mia_accounting.egg-info/dependency_links.txt
--rw-r--r--   0 imacat    (1000) users      (100)      107 2023-05-17 16:11:20.000000 mia-accounting-1.5.4/src/mia_accounting.egg-info/requires.txt
--rw-r--r--   0 imacat    (1000) users      (100)       11 2023-05-17 16:11:20.000000 mia-accounting-1.5.4/src/mia_accounting.egg-info/top_level.txt
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:22.762518 mia-accounting-1.5.4/tests/
--rwxr-xr-x   0 imacat    (1000) users      (100)     4341 2023-04-12 07:04:32.000000 mia-accounting-1.5.4/tests/babel-utils-test-site.py
--rwxr-xr-x   0 imacat    (1000) users      (100)     4297 2023-04-12 07:04:32.000000 mia-accounting-1.5.4/tests/babel-utils.py
--rw-r--r--   0 imacat    (1000) users      (100)    32727 2023-04-29 21:45:47.000000 mia-accounting-1.5.4/tests/test_account.py
--rw-r--r--   0 imacat    (1000) users      (100)     2409 2023-04-10 15:59:48.000000 mia-accounting-1.5.4/tests/test_base_account.py
--rw-r--r--   0 imacat    (1000) users      (100)     6113 2023-04-29 21:45:47.000000 mia-accounting-1.5.4/tests/test_commands.py
--rw-r--r--   0 imacat    (1000) users      (100)    23815 2023-04-29 21:45:47.000000 mia-accounting-1.5.4/tests/test_currency.py
--rw-r--r--   0 imacat    (1000) users      (100)    15998 2023-04-29 21:45:47.000000 mia-accounting-1.5.4/tests/test_description_editor.py
--rw-r--r--   0 imacat    (1000) users      (100)   103433 2023-05-17 16:04:33.000000 mia-accounting-1.5.4/tests/test_journal_entry.py
--rw-r--r--   0 imacat    (1000) users      (100)    38887 2023-04-13 01:09:51.000000 mia-accounting-1.5.4/tests/test_offset.py
--rw-r--r--   0 imacat    (1000) users      (100)    15940 2023-04-29 21:45:47.000000 mia-accounting-1.5.4/tests/test_option.py
--rw-r--r--   0 imacat    (1000) users      (100)    17864 2023-04-29 21:45:47.000000 mia-accounting-1.5.4/tests/test_report.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:22.762518 mia-accounting-1.5.4/tests/test_site/
--rw-r--r--   0 imacat    (1000) users      (100)     4589 2023-05-17 11:57:24.000000 mia-accounting-1.5.4/tests/test_site/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3958 2023-04-29 21:45:47.000000 mia-accounting-1.5.4/tests/test_site/auth.py
--rw-r--r--   0 imacat    (1000) users      (100)    13199 2023-04-29 21:45:47.000000 mia-accounting-1.5.4/tests/test_site/lib.py
--rw-r--r--   0 imacat    (1000) users      (100)     3367 2023-05-17 11:57:23.000000 mia-accounting-1.5.4/tests/test_site/locale.py
--rw-r--r--   0 imacat    (1000) users      (100)    13050 2023-04-29 21:45:47.000000 mia-accounting-1.5.4/tests/test_site/reset.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:22.762518 mia-accounting-1.5.4/tests/test_site/static/
--rw-r--r--   0 imacat    (1000) users      (100)     1420 2023-04-03 07:56:03.000000 mia-accounting-1.5.4/tests/test_site/static/favicon.svg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:22.834517 mia-accounting-1.5.4/tests/test_site/templates/
--rw-r--r--   0 imacat    (1000) users      (100)     6435 2023-05-06 15:53:46.000000 mia-accounting-1.5.4/tests/test_site/templates/base.html
--rw-r--r--   0 imacat    (1000) users      (100)     1239 2023-04-11 14:27:31.000000 mia-accounting-1.5.4/tests/test_site/templates/home.html
--rw-r--r--   0 imacat    (1000) users      (100)     1532 2023-04-11 14:03:59.000000 mia-accounting-1.5.4/tests/test_site/templates/login.html
--rw-r--r--   0 imacat    (1000) users      (100)     1838 2023-04-12 10:05:13.000000 mia-accounting-1.5.4/tests/test_site/templates/reset.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:22.986515 mia-accounting-1.5.4/tests/test_site/translations/
--rw-r--r--   0 imacat    (1000) users      (100)       80 2023-02-03 05:00:02.000000 mia-accounting-1.5.4/tests/test_site/translations/babel.cfg
--rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-12 09:59:51.000000 mia-accounting-1.5.4/tests/test_site/translations/messages.pot
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:20.322552 mia-accounting-1.5.4/tests/test_site/translations/zh_Hans/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:23.162512 mia-accounting-1.5.4/tests/test_site/translations/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)     2275 2023-04-12 10:00:18.000000 mia-accounting-1.5.4/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo
--rw-r--r--   0 imacat    (1000) users      (100)     3505 2023-04-12 10:00:18.000000 mia-accounting-1.5.4/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:20.322552 mia-accounting-1.5.4/tests/test_site/translations/zh_Hant/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-17 16:11:23.378509 mia-accounting-1.5.4/tests/test_site/translations/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)     2275 2023-04-12 10:00:18.000000 mia-accounting-1.5.4/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo
--rw-r--r--   0 imacat    (1000) users      (100)     3505 2023-04-12 10:05:13.000000 mia-accounting-1.5.4/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po
--rw-r--r--   0 imacat    (1000) users      (100)    27794 2023-04-18 01:14:44.000000 mia-accounting-1.5.4/tests/test_unmatched_offset.py
--rw-r--r--   0 imacat    (1000) users      (100)    16216 2023-05-17 08:26:34.000000 mia-accounting-1.5.4/tests/test_utils.py
--rw-r--r--   0 imacat    (1000) users      (100)     5175 2023-04-29 21:45:47.000000 mia-accounting-1.5.4/tests/testlib.py
--rw-r--r--   0 imacat    (1000) users      (100)    16669 2023-04-29 21:45:47.000000 mia-accounting-1.5.4/tests/testlib_journal_entry.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.649698 mia-accounting-1.5.5/
+-rw-r--r--   0 imacat    (1000) users      (100)    11358 2015-02-17 18:06:12.000000 mia-accounting-1.5.5/LICENSE
+-rw-r--r--   0 imacat    (1000) users      (100)     1070 2023-04-05 11:25:31.000000 mia-accounting-1.5.5/MANIFEST.in
+-rw-r--r--   0 imacat    (1000) users      (100)     3412 2023-05-23 00:45:05.649698 mia-accounting-1.5.5/PKG-INFO
+-rw-r--r--   0 imacat    (1000) users      (100)     2525 2023-04-23 12:04:20.000000 mia-accounting-1.5.5/README.rst
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.601698 mia-accounting-1.5.5/docs/
+-rw-r--r--   0 imacat    (1000) users      (100)      638 2023-01-27 04:20:04.000000 mia-accounting-1.5.5/docs/Makefile
+-rw-r--r--   0 imacat    (1000) users      (100)      804 2023-01-27 04:20:04.000000 mia-accounting-1.5.5/docs/make.bat
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.609698 mia-accounting-1.5.5/docs/source/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.609698 mia-accounting-1.5.5/docs/source/_static/
+-rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:08.000000 mia-accounting-1.5.5/docs/source/_static/.keep
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.609698 mia-accounting-1.5.5/docs/source/_templates/
+-rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:11.000000 mia-accounting-1.5.5/docs/source/_templates/.keep
+-rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-05-23 00:37:49.000000 mia-accounting-1.5.5/docs/source/accounting.account.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      959 2023-05-23 00:37:49.000000 mia-accounting-1.5.5/docs/source/accounting.base_account.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1053 2023-05-23 00:37:49.000000 mia-accounting-1.5.5/docs/source/accounting.currency.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1089 2023-05-23 00:37:49.000000 mia-accounting-1.5.5/docs/source/accounting.journal_entry.forms.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      937 2023-05-23 00:37:49.000000 mia-accounting-1.5.5/docs/source/accounting.journal_entry.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1162 2023-05-23 00:37:49.000000 mia-accounting-1.5.5/docs/source/accounting.journal_entry.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      513 2023-05-23 00:37:49.000000 mia-accounting-1.5.5/docs/source/accounting.option.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1551 2023-05-23 00:37:49.000000 mia-accounting-1.5.5/docs/source/accounting.report.period.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2460 2023-05-23 00:37:49.000000 mia-accounting-1.5.5/docs/source/accounting.report.reports.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      861 2023-05-23 00:37:49.000000 mia-accounting-1.5.5/docs/source/accounting.report.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2168 2023-05-23 00:37:49.000000 mia-accounting-1.5.5/docs/source/accounting.report.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1301 2023-05-23 00:37:49.000000 mia-accounting-1.5.5/docs/source/accounting.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2405 2023-05-23 00:37:49.000000 mia-accounting-1.5.5/docs/source/accounting.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     8334 2023-05-23 00:42:24.000000 mia-accounting-1.5.5/docs/source/changelog.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1051 2023-04-23 12:12:53.000000 mia-accounting-1.5.5/docs/source/conf.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1508 2023-04-06 00:38:39.000000 mia-accounting-1.5.5/docs/source/examples.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2837 2023-04-06 00:21:32.000000 mia-accounting-1.5.5/docs/source/history.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      521 2023-04-23 12:04:21.000000 mia-accounting-1.5.5/docs/source/index.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     3568 2023-05-06 15:58:29.000000 mia-accounting-1.5.5/docs/source/intro.rst
+-rw-r--r--   0 imacat    (1000) users      (100)       53 2023-04-04 10:25:53.000000 mia-accounting-1.5.5/docs/source/modules.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1994 2023-05-09 00:42:23.000000 mia-accounting-1.5.5/pyproject.toml
+-rw-r--r--   0 imacat    (1000) users      (100)       38 2023-05-23 00:45:05.649698 mia-accounting-1.5.5/setup.cfg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.597699 mia-accounting-1.5.5/src/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.613698 mia-accounting-1.5.5/src/accounting/
+-rw-r--r--   0 imacat    (1000) users      (100)     3045 2023-05-23 00:43:07.000000 mia-accounting-1.5.5/src/accounting/__init__.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.613698 mia-accounting-1.5.5/src/accounting/account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-10 15:59:48.000000 mia-accounting-1.5.5/src/accounting/account/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3868 2023-04-29 21:45:45.000000 mia-accounting-1.5.5/src/accounting/account/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1512 2023-04-04 09:21:35.000000 mia-accounting-1.5.5/src/accounting/account/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7145 2023-04-04 09:21:33.000000 mia-accounting-1.5.5/src/accounting/account/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2209 2023-04-04 09:21:35.000000 mia-accounting-1.5.5/src/accounting/account/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7416 2023-04-09 02:08:22.000000 mia-accounting-1.5.5/src/accounting/account/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.613698 mia-accounting-1.5.5/src/accounting/base_account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1240 2023-04-10 15:59:48.000000 mia-accounting-1.5.5/src/accounting/base_account/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1800 2023-04-10 15:59:48.000000 mia-accounting-1.5.5/src/accounting/base_account/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1592 2023-04-04 09:21:35.000000 mia-accounting-1.5.5/src/accounting/base_account/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1769 2023-04-04 09:21:37.000000 mia-accounting-1.5.5/src/accounting/base_account/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1812 2023-04-09 02:08:22.000000 mia-accounting-1.5.5/src/accounting/base_account/views.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2138 2023-04-10 15:59:48.000000 mia-accounting-1.5.5/src/accounting/commands.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.617698 mia-accounting-1.5.5/src/accounting/currency/
+-rw-r--r--   0 imacat    (1000) users      (100)     1312 2023-04-10 15:59:48.000000 mia-accounting-1.5.5/src/accounting/currency/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2206 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/currency/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1556 2023-04-04 09:21:35.000000 mia-accounting-1.5.5/src/accounting/currency/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3172 2023-04-04 09:21:36.000000 mia-accounting-1.5.5/src/accounting/currency/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1720 2023-04-04 09:21:34.000000 mia-accounting-1.5.5/src/accounting/currency/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6609 2023-04-09 02:08:22.000000 mia-accounting-1.5.5/src/accounting/currency/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.617698 mia-accounting-1.5.5/src/accounting/data/
+-rw-r--r--   0 imacat    (1000) users      (100)    36368 2023-03-14 01:04:26.000000 mia-accounting-1.5.5/src/accounting/data/base_accounts.csv
+-rw-r--r--   0 imacat    (1000) users      (100)      370 2023-03-14 01:04:26.000000 mia-accounting-1.5.5/src/accounting/data/currencies.csv
+-rw-r--r--   0 imacat    (1000) users      (100)     3144 2023-04-04 09:21:33.000000 mia-accounting-1.5.5/src/accounting/forms.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.617698 mia-accounting-1.5.5/src/accounting/journal_entry/
+-rw-r--r--   0 imacat    (1000) users      (100)     1376 2023-04-04 09:21:35.000000 mia-accounting-1.5.5/src/accounting/journal_entry/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3302 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/journal_entry/converters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.617698 mia-accounting-1.5.5/src/accounting/journal_entry/forms/
+-rw-r--r--   0 imacat    (1000) users      (100)      934 2023-04-04 09:21:37.000000 mia-accounting-1.5.5/src/accounting/journal_entry/forms/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11003 2023-04-23 05:21:41.000000 mia-accounting-1.5.5/src/accounting/journal_entry/forms/currency.py
+-rw-r--r--   0 imacat    (1000) users      (100)    24568 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/journal_entry/forms/journal_entry.py
+-rw-r--r--   0 imacat    (1000) users      (100)    19807 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/journal_entry/forms/line_item.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3291 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/journal_entry/forms/reorder.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2535 2023-04-04 09:21:32.000000 mia-accounting-1.5.5/src/accounting/journal_entry/template_filters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.621698 mia-accounting-1.5.5/src/accounting/journal_entry/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      729 2023-04-04 09:21:32.000000 mia-accounting-1.5.5/src/accounting/journal_entry/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1802 2023-04-17 23:37:17.000000 mia-accounting-1.5.5/src/accounting/journal_entry/utils/account_option.py
+-rw-r--r--   0 imacat    (1000) users      (100)    12981 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/journal_entry/utils/description_editor.py
+-rw-r--r--   0 imacat    (1000) users      (100)    12676 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/journal_entry/utils/operators.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3722 2023-04-23 05:21:41.000000 mia-accounting-1.5.5/src/accounting/journal_entry/utils/original_line_items.py
+-rw-r--r--   0 imacat    (1000) users      (100)     9351 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/journal_entry/views.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3809 2023-04-04 09:21:33.000000 mia-accounting-1.5.5/src/accounting/locale.py
+-rw-r--r--   0 imacat    (1000) users      (100)    32618 2023-04-30 07:03:58.000000 mia-accounting-1.5.5/src/accounting/models.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.621698 mia-accounting-1.5.5/src/accounting/option/
+-rw-r--r--   0 imacat    (1000) users      (100)      993 2023-04-04 09:21:35.000000 mia-accounting-1.5.5/src/accounting/option/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     9762 2023-04-08 00:27:23.000000 mia-accounting-1.5.5/src/accounting/option/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2827 2023-04-04 09:21:32.000000 mia-accounting-1.5.5/src/accounting/option/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.621698 mia-accounting-1.5.5/src/accounting/report/
+-rw-r--r--   0 imacat    (1000) users      (100)     1362 2023-04-08 10:12:56.000000 mia-accounting-1.5.5/src/accounting/report/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-08 10:12:56.000000 mia-accounting-1.5.5/src/accounting/report/converters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.621698 mia-accounting-1.5.5/src/accounting/report/period/
+-rw-r--r--   0 imacat    (1000) users      (100)      793 2023-04-04 09:21:32.000000 mia-accounting-1.5.5/src/accounting/report/period/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3702 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/report/period/chooser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5557 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/report/period/description.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1050 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/report/period/month_end.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4127 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/report/period/parser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4522 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/report/period/period.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4785 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/report/period/shortcuts.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3915 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/report/period/specification.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.625698 mia-accounting-1.5.5/src/accounting/report/reports/
+-rw-r--r--   0 imacat    (1000) users      (100)      946 2023-04-04 09:21:36.000000 mia-accounting-1.5.5/src/accounting/report/reports/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)    17920 2023-04-06 01:50:58.000000 mia-accounting-1.5.5/src/accounting/report/reports/balance_sheet.py
+-rw-r--r--   0 imacat    (1000) users      (100)    18807 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/report/reports/income_expenses.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11733 2023-04-06 01:50:58.000000 mia-accounting-1.5.5/src/accounting/report/reports/income_statement.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8130 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/report/reports/journal.py
+-rw-r--r--   0 imacat    (1000) users      (100)    16530 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/report/reports/ledger.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8472 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/report/reports/search.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8853 2023-04-06 01:50:58.000000 mia-accounting-1.5.5/src/accounting/report/reports/trial_balance.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8099 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/report/reports/unapplied.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5210 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/report/reports/unapplied_accounts.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8169 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/report/reports/unmatched.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5191 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/report/reports/unmatched_accounts.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1205 2023-04-04 09:21:33.000000 mia-accounting-1.5.5/src/accounting/report/template_filters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.625698 mia-accounting-1.5.5/src/accounting/report/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      711 2023-04-04 09:21:34.000000 mia-accounting-1.5.5/src/accounting/report/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3034 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/report/utils/base_page_params.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1143 2023-04-04 09:21:36.000000 mia-accounting-1.5.5/src/accounting/report/utils/base_report.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3334 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/report/utils/csv_export.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7321 2023-04-29 22:38:16.000000 mia-accounting-1.5.5/src/accounting/report/utils/offset_matcher.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1368 2023-04-04 09:21:37.000000 mia-accounting-1.5.5/src/accounting/report/utils/option_link.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7881 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/report/utils/report_chooser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1371 2023-04-17 08:41:57.000000 mia-accounting-1.5.5/src/accounting/report/utils/report_type.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4385 2023-04-23 05:21:41.000000 mia-accounting-1.5.5/src/accounting/report/utils/unapplied.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2221 2023-04-23 05:21:41.000000 mia-accounting-1.5.5/src/accounting/report/utils/unmatched.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5440 2023-04-18 00:59:05.000000 mia-accounting-1.5.5/src/accounting/report/utils/urls.py
+-rw-r--r--   0 imacat    (1000) users      (100)    14167 2023-04-18 01:14:44.000000 mia-accounting-1.5.5/src/accounting/report/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.589699 mia-accounting-1.5.5/src/accounting/static/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.629698 mia-accounting-1.5.5/src/accounting/static/css/
+-rw-r--r--   0 imacat    (1000) users      (100)    13431 2023-04-18 00:10:33.000000 mia-accounting-1.5.5/src/accounting/static/css/style.css
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.629698 mia-accounting-1.5.5/src/accounting/static/js/
+-rw-r--r--   0 imacat    (1000) users      (100)    10921 2023-04-04 10:05:35.000000 mia-accounting-1.5.5/src/accounting/static/js/account-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1599 2023-04-04 10:05:35.000000 mia-accounting-1.5.5/src/accounting/static/js/account-order.js
+-rw-r--r--   0 imacat    (1000) users      (100)     4955 2023-04-04 10:05:35.000000 mia-accounting-1.5.5/src/accounting/static/js/currency-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    38865 2023-04-17 23:44:56.000000 mia-accounting-1.5.5/src/accounting/static/js/description-editor.js
+-rw-r--r--   0 imacat    (1000) users      (100)     3564 2023-04-04 10:05:35.000000 mia-accounting-1.5.5/src/accounting/static/js/drag-and-drop-reorder.js
+-rw-r--r--   0 imacat    (1000) users      (100)     9211 2023-04-17 23:32:14.000000 mia-accounting-1.5.5/src/accounting/static/js/journal-entry-account-selector.js
+-rw-r--r--   0 imacat    (1000) users      (100)    33086 2023-04-17 23:52:58.000000 mia-accounting-1.5.5/src/accounting/static/js/journal-entry-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    19665 2023-04-30 07:03:59.000000 mia-accounting-1.5.5/src/accounting/static/js/journal-entry-line-item-editor.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1366 2023-04-04 10:05:35.000000 mia-accounting-1.5.5/src/accounting/static/js/journal-entry-order.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1436 2023-04-04 10:05:35.000000 mia-accounting-1.5.5/src/accounting/static/js/material-fab-speed-dial.js
+-rw-r--r--   0 imacat    (1000) users      (100)    28660 2023-04-04 10:05:35.000000 mia-accounting-1.5.5/src/accounting/static/js/option-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    11670 2023-04-17 23:40:31.000000 mia-accounting-1.5.5/src/accounting/static/js/original-line-item-selector.js
+-rw-r--r--   0 imacat    (1000) users      (100)    10374 2023-04-04 10:05:35.000000 mia-accounting-1.5.5/src/accounting/static/js/period-chooser.js
+-rw-r--r--   0 imacat    (1000) users      (100)     2712 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/template_filters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1137 2023-04-23 01:43:59.000000 mia-accounting-1.5.5/src/accounting/template_globals.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.589699 mia-accounting-1.5.5/src/accounting/templates/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.629698 mia-accounting-1.5.5/src/accounting/templates/accounting/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.629698 mia-accounting-1.5.5/src/accounting/templates/accounting/account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1034 2023-04-04 10:04:10.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/account/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4266 2023-04-04 10:04:11.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/account/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1081 2023-04-04 10:04:11.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/account/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.629698 mia-accounting-1.5.5/src/accounting/templates/accounting/account/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     5704 2023-04-04 10:04:10.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/account/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2734 2023-05-17 13:41:19.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/account/list.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3052 2023-04-04 10:04:12.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/account/order.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.629698 mia-accounting-1.5.5/src/accounting/templates/accounting/base-account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1581 2023-04-04 10:04:10.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/base-account/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2095 2023-05-17 13:41:20.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/base-account/list.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-04 10:04:10.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/base.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.633698 mia-accounting-1.5.5/src/accounting/templates/accounting/currency/
+-rw-r--r--   0 imacat    (1000) users      (100)     1039 2023-04-04 10:04:12.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/currency/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3883 2023-04-04 10:04:10.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/currency/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1152 2023-04-04 10:04:11.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/currency/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.633698 mia-accounting-1.5.5/src/accounting/templates/accounting/currency/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     2850 2023-04-04 10:04:10.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/currency/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2606 2023-05-17 13:41:19.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/currency/list.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.633698 mia-accounting-1.5.5/src/accounting/templates/accounting/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     2706 2023-04-17 15:07:31.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/include/nav.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1986 2023-04-04 10:04:11.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/include/pagination.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.633698 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.633698 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/disbursement/
+-rw-r--r--   0 imacat    (1000) users      (100)     1149 2023-04-04 23:56:52.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/disbursement/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2028 2023-04-04 10:04:11.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/disbursement/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1213 2023-04-04 10:04:09.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/disbursement/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.633698 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/disbursement/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1195 2023-04-04 10:04:10.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2283 2023-04-04 10:04:12.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.633698 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     3406 2023-04-17 23:32:14.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)    14561 2023-05-22 10:32:23.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3242 2023-04-17 23:11:57.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4554 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2726 2023-04-04 10:04:10.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html
+-rw-r--r--   0 imacat    (1000) users      (100)     6442 2023-04-17 23:54:15.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/form-line-item.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4370 2023-04-04 10:04:12.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4231 2023-05-22 09:36:19.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2093 2023-04-04 10:04:11.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3791 2023-04-18 00:10:33.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3069 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/order.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.633698 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/receipt/
+-rw-r--r--   0 imacat    (1000) users      (100)     1134 2023-04-04 23:56:52.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/receipt/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2025 2023-04-04 10:04:12.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/receipt/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-04 10:04:11.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/receipt/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.633698 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/receipt/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1194 2023-04-04 10:04:12.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2278 2023-04-04 10:04:11.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/receipt/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.633698 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/transfer/
+-rw-r--r--   0 imacat    (1000) users      (100)     1127 2023-04-04 23:56:52.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/transfer/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2691 2023-04-04 10:04:09.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/transfer/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1200 2023-04-04 10:04:10.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/transfer/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.637698 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/transfer/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1649 2023-04-04 10:04:11.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2845 2023-04-04 10:04:12.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/transfer/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.637698 mia-accounting-1.5.5/src/accounting/templates/accounting/option/
+-rw-r--r--   0 imacat    (1000) users      (100)     2765 2023-04-08 10:12:54.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/option/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4699 2023-04-08 00:27:23.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/option/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.637698 mia-accounting-1.5.5/src/accounting/templates/accounting/option/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1851 2023-04-04 10:04:10.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3214 2023-04-04 10:04:12.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/option/include/form-recurring-item.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-04 10:04:12.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4345 2023-05-22 09:36:19.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.637698 mia-accounting-1.5.5/src/accounting/templates/accounting/report/
+-rw-r--r--   0 imacat    (1000) users      (100)     5435 2023-04-18 00:39:27.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/balance-sheet.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.637698 mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1970 2023-04-04 10:04:12.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1708 2023-04-04 10:04:12.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/balance-sheet-section.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1281 2023-04-04 10:04:10.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1760 2023-04-04 10:04:12.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1252 2023-04-04 10:04:11.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/ledger-row-desktop.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1429 2023-04-04 10:04:10.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/ledger-row-mobile.html
+-rw-r--r--   0 imacat    (1000) users      (100)     8857 2023-04-04 10:04:12.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/period-chooser.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1963 2023-05-17 13:41:20.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/search-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     5630 2023-05-17 13:41:20.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/toolbar-buttons.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4841 2023-04-18 00:34:44.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/income-expenses.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4618 2023-04-18 00:37:47.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/income-statement.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4202 2023-04-04 10:04:10.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/journal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4946 2023-04-18 00:33:38.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/ledger.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4044 2023-04-04 10:04:11.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/search.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3710 2023-04-18 00:36:16.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/trial-balance.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3037 2023-04-18 00:59:05.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/unapplied-accounts.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3843 2023-04-18 00:59:06.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/unapplied.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3034 2023-04-18 00:59:05.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/unmatched-accounts.html
+-rw-r--r--   0 imacat    (1000) users      (100)     6998 2023-04-18 00:59:05.000000 mia-accounting-1.5.5/src/accounting/templates/accounting/report/unmatched.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.641698 mia-accounting-1.5.5/src/accounting/translations/
+-rw-r--r--   0 imacat    (1000) users      (100)    49437 2023-04-18 01:32:01.000000 mia-accounting-1.5.5/src/accounting/translations/accounting.pot
+-rw-r--r--   0 imacat    (1000) users      (100)       80 2023-01-27 03:33:36.000000 mia-accounting-1.5.5/src/accounting/translations/babel.cfg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.593699 mia-accounting-1.5.5/src/accounting/translations/zh_Hans/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.641698 mia-accounting-1.5.5/src/accounting/translations/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)    16202 2023-04-18 01:32:11.000000 mia-accounting-1.5.5/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo
+-rw-r--r--   0 imacat    (1000) users      (100)    54246 2023-04-18 01:32:11.000000 mia-accounting-1.5.5/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.593699 mia-accounting-1.5.5/src/accounting/translations/zh_Hant/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.641698 mia-accounting-1.5.5/src/accounting/translations/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)    16202 2023-04-18 01:32:11.000000 mia-accounting-1.5.5/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo
+-rw-r--r--   0 imacat    (1000) users      (100)    54246 2023-04-18 01:32:11.000000 mia-accounting-1.5.5/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.641698 mia-accounting-1.5.5/src/accounting/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      778 2023-04-04 09:21:31.000000 mia-accounting-1.5.5/src/accounting/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1036 2023-05-17 07:33:36.000000 mia-accounting-1.5.5/src/accounting/utils/cast.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3325 2023-05-04 01:35:20.000000 mia-accounting-1.5.5/src/accounting/utils/current_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1426 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/utils/flash_errors.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1030 2023-04-04 09:21:32.000000 mia-accounting-1.5.5/src/accounting/utils/journal_entry_types.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3427 2023-05-22 23:11:54.000000 mia-accounting-1.5.5/src/accounting/utils/next_uri.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1198 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/utils/offset_alias.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6906 2023-04-08 10:12:55.000000 mia-accounting-1.5.5/src/accounting/utils/options.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11745 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/utils/pagination.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4262 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/utils/permission.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1638 2023-04-04 09:21:34.000000 mia-accounting-1.5.5/src/accounting/utils/query.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1221 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/utils/random_id.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1396 2023-04-04 09:21:37.000000 mia-accounting-1.5.5/src/accounting/utils/strip_text.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4985 2023-04-29 21:45:46.000000 mia-accounting-1.5.5/src/accounting/utils/user.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.641698 mia-accounting-1.5.5/src/mia_accounting.egg-info/
+-rw-r--r--   0 imacat    (1000) users      (100)     3412 2023-05-23 00:45:05.000000 mia-accounting-1.5.5/src/mia_accounting.egg-info/PKG-INFO
+-rw-r--r--   0 imacat    (1000) users      (100)    11434 2023-05-23 00:45:05.000000 mia-accounting-1.5.5/src/mia_accounting.egg-info/SOURCES.txt
+-rw-r--r--   0 imacat    (1000) users      (100)        1 2023-05-23 00:45:05.000000 mia-accounting-1.5.5/src/mia_accounting.egg-info/dependency_links.txt
+-rw-r--r--   0 imacat    (1000) users      (100)      107 2023-05-23 00:45:05.000000 mia-accounting-1.5.5/src/mia_accounting.egg-info/requires.txt
+-rw-r--r--   0 imacat    (1000) users      (100)       11 2023-05-23 00:45:05.000000 mia-accounting-1.5.5/src/mia_accounting.egg-info/top_level.txt
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.645698 mia-accounting-1.5.5/tests/
+-rwxr-xr-x   0 imacat    (1000) users      (100)     4341 2023-04-12 07:04:32.000000 mia-accounting-1.5.5/tests/babel-utils-test-site.py
+-rwxr-xr-x   0 imacat    (1000) users      (100)     4297 2023-04-12 07:04:32.000000 mia-accounting-1.5.5/tests/babel-utils.py
+-rw-r--r--   0 imacat    (1000) users      (100)    32948 2023-05-22 23:22:24.000000 mia-accounting-1.5.5/tests/test_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2409 2023-04-10 15:59:48.000000 mia-accounting-1.5.5/tests/test_base_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6113 2023-04-29 21:45:47.000000 mia-accounting-1.5.5/tests/test_commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)    23998 2023-05-22 23:24:38.000000 mia-accounting-1.5.5/tests/test_currency.py
+-rw-r--r--   0 imacat    (1000) users      (100)    16282 2023-05-22 23:26:32.000000 mia-accounting-1.5.5/tests/test_description_editor.py
+-rw-r--r--   0 imacat    (1000) users      (100)   105500 2023-05-23 00:40:17.000000 mia-accounting-1.5.5/tests/test_journal_entry.py
+-rw-r--r--   0 imacat    (1000) users      (100)    42546 2023-05-23 00:01:57.000000 mia-accounting-1.5.5/tests/test_offset.py
+-rw-r--r--   0 imacat    (1000) users      (100)    16950 2023-05-23 00:10:42.000000 mia-accounting-1.5.5/tests/test_option.py
+-rw-r--r--   0 imacat    (1000) users      (100)    17864 2023-04-29 21:45:47.000000 mia-accounting-1.5.5/tests/test_report.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.645698 mia-accounting-1.5.5/tests/test_site/
+-rw-r--r--   0 imacat    (1000) users      (100)     4968 2023-05-23 00:22:47.000000 mia-accounting-1.5.5/tests/test_site/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3958 2023-04-29 21:45:47.000000 mia-accounting-1.5.5/tests/test_site/auth.py
+-rw-r--r--   0 imacat    (1000) users      (100)    13324 2023-05-23 00:02:48.000000 mia-accounting-1.5.5/tests/test_site/lib.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3367 2023-05-17 11:57:23.000000 mia-accounting-1.5.5/tests/test_site/locale.py
+-rw-r--r--   0 imacat    (1000) users      (100)    13050 2023-04-29 21:45:47.000000 mia-accounting-1.5.5/tests/test_site/reset.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.645698 mia-accounting-1.5.5/tests/test_site/static/
+-rw-r--r--   0 imacat    (1000) users      (100)     1420 2023-04-03 07:56:03.000000 mia-accounting-1.5.5/tests/test_site/static/favicon.svg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.645698 mia-accounting-1.5.5/tests/test_site/templates/
+-rw-r--r--   0 imacat    (1000) users      (100)     6656 2023-05-23 00:22:47.000000 mia-accounting-1.5.5/tests/test_site/templates/base.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1239 2023-04-11 14:27:31.000000 mia-accounting-1.5.5/tests/test_site/templates/home.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1532 2023-04-11 14:03:59.000000 mia-accounting-1.5.5/tests/test_site/templates/login.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1838 2023-04-12 10:05:13.000000 mia-accounting-1.5.5/tests/test_site/templates/reset.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.645698 mia-accounting-1.5.5/tests/test_site/translations/
+-rw-r--r--   0 imacat    (1000) users      (100)       80 2023-02-03 05:00:02.000000 mia-accounting-1.5.5/tests/test_site/translations/babel.cfg
+-rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-12 09:59:51.000000 mia-accounting-1.5.5/tests/test_site/translations/messages.pot
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.597699 mia-accounting-1.5.5/tests/test_site/translations/zh_Hans/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.645698 mia-accounting-1.5.5/tests/test_site/translations/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)     2275 2023-04-12 10:00:18.000000 mia-accounting-1.5.5/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo
+-rw-r--r--   0 imacat    (1000) users      (100)     3505 2023-04-12 10:00:18.000000 mia-accounting-1.5.5/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.597699 mia-accounting-1.5.5/tests/test_site/translations/zh_Hant/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-23 00:45:05.649698 mia-accounting-1.5.5/tests/test_site/translations/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)     2275 2023-04-12 10:00:18.000000 mia-accounting-1.5.5/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo
+-rw-r--r--   0 imacat    (1000) users      (100)     3505 2023-04-12 10:05:13.000000 mia-accounting-1.5.5/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po
+-rw-r--r--   0 imacat    (1000) users      (100)    28011 2023-05-23 00:12:12.000000 mia-accounting-1.5.5/tests/test_unmatched_offset.py
+-rw-r--r--   0 imacat    (1000) users      (100)    15328 2023-05-23 00:16:21.000000 mia-accounting-1.5.5/tests/test_utils.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5470 2023-05-22 23:23:54.000000 mia-accounting-1.5.5/tests/testlib.py
+-rw-r--r--   0 imacat    (1000) users      (100)    16955 2023-05-22 23:52:24.000000 mia-accounting-1.5.5/tests/testlib_journal_entry.py
```

### Comparing `mia-accounting-1.5.4/LICENSE` & `mia-accounting-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/MANIFEST.in` & `mia-accounting-1.5.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/PKG-INFO` & `mia-accounting-1.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mia-accounting
-Version: 1.5.4
+Version: 1.5.5
 Summary: A Flask accounting module.
 Author-email: imacat <imacat@mail.imacat.idv.tw>
 Project-URL: Documentation, https://mia-accounting.readthedocs.io
 Project-URL: Change Log, https://mia-accounting.readthedocs.io/en/latest/changelog.html
 Project-URL: Repository, https://github.com/imacat/mia-accounting
 Project-URL: Bug Tracker, https://github.com/imacat/mia-accounting/issues
 Project-URL: Demonstration, https://accounting.imacat.idv.tw
```

### Comparing `mia-accounting-1.5.4/README.rst` & `mia-accounting-1.5.5/README.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/docs/Makefile` & `mia-accounting-1.5.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/docs/make.bat` & `mia-accounting-1.5.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/docs/source/accounting.account.rst` & `mia-accounting-1.5.5/docs/source/accounting.account.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/docs/source/accounting.base_account.rst` & `mia-accounting-1.5.5/docs/source/accounting.base_account.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/docs/source/accounting.currency.rst` & `mia-accounting-1.5.5/docs/source/accounting.currency.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/docs/source/accounting.journal_entry.forms.rst` & `mia-accounting-1.5.5/docs/source/accounting.journal_entry.forms.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/docs/source/accounting.journal_entry.rst` & `mia-accounting-1.5.5/docs/source/accounting.journal_entry.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/docs/source/accounting.journal_entry.utils.rst` & `mia-accounting-1.5.5/docs/source/accounting.journal_entry.utils.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/docs/source/accounting.option.rst` & `mia-accounting-1.5.5/docs/source/accounting.option.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/docs/source/accounting.report.period.rst` & `mia-accounting-1.5.5/docs/source/accounting.report.period.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/docs/source/accounting.report.reports.rst` & `mia-accounting-1.5.5/docs/source/accounting.report.reports.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/docs/source/accounting.report.rst` & `mia-accounting-1.5.5/docs/source/accounting.report.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/docs/source/accounting.report.utils.rst` & `mia-accounting-1.5.5/docs/source/accounting.report.utils.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/docs/source/accounting.rst` & `mia-accounting-1.5.5/docs/source/accounting.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/docs/source/accounting.utils.rst` & `mia-accounting-1.5.5/docs/source/accounting.utils.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/docs/source/changelog.rst` & `mia-accounting-1.5.5/docs/source/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 Change Log
 ==========
 
 
+Version 1.5.5
+-------------
+
+Released 2023/5/23
+
+Security fixes.
+
+* Revised the next URI utilities to encode and decode the next URI
+  preventing tampering with the next URI.
+* Added the integrity value of the CDN stylesheet links.
+* Various fixes.
+
+
 Version 1.5.4
 -------------
 
 Released 2023/5/18
 
 Security fixes.
```

### Comparing `mia-accounting-1.5.4/docs/source/conf.py` & `mia-accounting-1.5.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/docs/source/examples.rst` & `mia-accounting-1.5.5/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/docs/source/history.rst` & `mia-accounting-1.5.5/docs/source/history.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/docs/source/index.rst` & `mia-accounting-1.5.5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/docs/source/intro.rst` & `mia-accounting-1.5.5/docs/source/intro.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/pyproject.toml` & `mia-accounting-1.5.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/__init__.py` & `mia-accounting-1.5.5/src/accounting/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from pathlib import Path
 
 from flask import Flask, Blueprint
 from flask_sqlalchemy import SQLAlchemy
 
 from accounting.utils.user import UserUtilityInterface
 
-VERSION: str = "1.5.4"
+VERSION: str = "1.5.5"
 """The package version."""
 db: SQLAlchemy = SQLAlchemy()
 """The database instance."""
 data_dir: Path = Path(__file__).parent / "data"
 """The data directory."""
```

### Comparing `mia-accounting-1.5.4/src/accounting/account/__init__.py` & `mia-accounting-1.5.5/src/accounting/account/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/account/commands.py` & `mia-accounting-1.5.5/src/accounting/account/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/account/converters.py` & `mia-accounting-1.5.5/src/accounting/account/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/account/forms.py` & `mia-accounting-1.5.5/src/accounting/account/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/account/queries.py` & `mia-accounting-1.5.5/src/accounting/account/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/account/views.py` & `mia-accounting-1.5.5/src/accounting/account/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/base_account/__init__.py` & `mia-accounting-1.5.5/src/accounting/base_account/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/base_account/commands.py` & `mia-accounting-1.5.5/src/accounting/base_account/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/base_account/converters.py` & `mia-accounting-1.5.5/src/accounting/base_account/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/base_account/queries.py` & `mia-accounting-1.5.5/src/accounting/base_account/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/base_account/views.py` & `mia-accounting-1.5.5/src/accounting/base_account/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/commands.py` & `mia-accounting-1.5.5/src/accounting/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/currency/__init__.py` & `mia-accounting-1.5.5/src/accounting/currency/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/currency/commands.py` & `mia-accounting-1.5.5/src/accounting/currency/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/currency/converters.py` & `mia-accounting-1.5.5/src/accounting/currency/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/currency/forms.py` & `mia-accounting-1.5.5/src/accounting/currency/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/currency/queries.py` & `mia-accounting-1.5.5/src/accounting/currency/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/currency/views.py` & `mia-accounting-1.5.5/src/accounting/currency/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/data/base_accounts.csv` & `mia-accounting-1.5.5/src/accounting/data/base_accounts.csv`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/forms.py` & `mia-accounting-1.5.5/src/accounting/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/journal_entry/__init__.py` & `mia-accounting-1.5.5/src/accounting/journal_entry/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/journal_entry/converters.py` & `mia-accounting-1.5.5/src/accounting/journal_entry/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/journal_entry/forms/__init__.py` & `mia-accounting-1.5.5/src/accounting/journal_entry/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/journal_entry/forms/currency.py` & `mia-accounting-1.5.5/src/accounting/journal_entry/forms/currency.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/journal_entry/forms/journal_entry.py` & `mia-accounting-1.5.5/src/accounting/journal_entry/forms/journal_entry.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/journal_entry/forms/line_item.py` & `mia-accounting-1.5.5/src/accounting/journal_entry/forms/line_item.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/journal_entry/forms/reorder.py` & `mia-accounting-1.5.5/src/accounting/journal_entry/forms/reorder.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/journal_entry/template_filters.py` & `mia-accounting-1.5.5/src/accounting/journal_entry/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/journal_entry/utils/__init__.py` & `mia-accounting-1.5.5/src/accounting/journal_entry/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/journal_entry/utils/account_option.py` & `mia-accounting-1.5.5/src/accounting/journal_entry/utils/account_option.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/journal_entry/utils/description_editor.py` & `mia-accounting-1.5.5/src/accounting/journal_entry/utils/description_editor.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/journal_entry/utils/operators.py` & `mia-accounting-1.5.5/src/accounting/journal_entry/utils/operators.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/journal_entry/utils/original_line_items.py` & `mia-accounting-1.5.5/src/accounting/journal_entry/utils/original_line_items.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/journal_entry/views.py` & `mia-accounting-1.5.5/src/accounting/journal_entry/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/locale.py` & `mia-accounting-1.5.5/src/accounting/locale.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/models.py` & `mia-accounting-1.5.5/src/accounting/models.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/option/__init__.py` & `mia-accounting-1.5.5/src/accounting/option/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/option/forms.py` & `mia-accounting-1.5.5/src/accounting/option/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/option/views.py` & `mia-accounting-1.5.5/src/accounting/option/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/report/__init__.py` & `mia-accounting-1.5.5/src/accounting/report/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/report/converters.py` & `mia-accounting-1.5.5/src/accounting/report/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/report/period/__init__.py` & `mia-accounting-1.5.5/src/accounting/report/period/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/report/period/chooser.py` & `mia-accounting-1.5.5/src/accounting/report/period/chooser.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/report/period/description.py` & `mia-accounting-1.5.5/src/accounting/report/period/description.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/report/period/month_end.py` & `mia-accounting-1.5.5/src/accounting/report/period/month_end.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/report/period/parser.py` & `mia-accounting-1.5.5/src/accounting/report/period/parser.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/report/period/period.py` & `mia-accounting-1.5.5/src/accounting/report/period/period.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/report/period/shortcuts.py` & `mia-accounting-1.5.5/src/accounting/report/period/shortcuts.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/report/period/specification.py` & `mia-accounting-1.5.5/src/accounting/report/period/specification.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/report/reports/__init__.py` & `mia-accounting-1.5.5/src/accounting/report/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/report/reports/balance_sheet.py` & `mia-accounting-1.5.5/src/accounting/report/reports/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/report/reports/income_expenses.py` & `mia-accounting-1.5.5/src/accounting/report/reports/income_expenses.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/report/reports/income_statement.py` & `mia-accounting-1.5.5/src/accounting/report/reports/income_statement.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/report/reports/journal.py` & `mia-accounting-1.5.5/src/accounting/report/reports/journal.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/report/reports/ledger.py` & `mia-accounting-1.5.5/src/accounting/report/reports/ledger.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/report/reports/search.py` & `mia-accounting-1.5.5/src/accounting/report/reports/search.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/report/reports/trial_balance.py` & `mia-accounting-1.5.5/src/accounting/report/reports/trial_balance.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/report/reports/unapplied.py` & `mia-accounting-1.5.5/src/accounting/report/reports/unapplied.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/report/reports/unapplied_accounts.py` & `mia-accounting-1.5.5/src/accounting/report/reports/unapplied_accounts.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/report/reports/unmatched.py` & `mia-accounting-1.5.5/src/accounting/report/reports/unmatched.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/report/reports/unmatched_accounts.py` & `mia-accounting-1.5.5/src/accounting/report/reports/unmatched_accounts.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/report/template_filters.py` & `mia-accounting-1.5.5/src/accounting/report/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/report/utils/__init__.py` & `mia-accounting-1.5.5/src/accounting/report/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/report/utils/base_page_params.py` & `mia-accounting-1.5.5/src/accounting/report/utils/base_page_params.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/report/utils/base_report.py` & `mia-accounting-1.5.5/src/accounting/report/utils/base_report.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/report/utils/csv_export.py` & `mia-accounting-1.5.5/src/accounting/report/utils/csv_export.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/report/utils/offset_matcher.py` & `mia-accounting-1.5.5/src/accounting/report/utils/offset_matcher.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/report/utils/option_link.py` & `mia-accounting-1.5.5/src/accounting/report/utils/option_link.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/report/utils/report_chooser.py` & `mia-accounting-1.5.5/src/accounting/report/utils/report_chooser.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/report/utils/report_type.py` & `mia-accounting-1.5.5/src/accounting/report/utils/report_type.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/report/utils/unapplied.py` & `mia-accounting-1.5.5/src/accounting/report/utils/unapplied.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/report/utils/unmatched.py` & `mia-accounting-1.5.5/src/accounting/report/utils/unmatched.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/report/utils/urls.py` & `mia-accounting-1.5.5/src/accounting/report/utils/urls.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/report/views.py` & `mia-accounting-1.5.5/src/accounting/report/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/static/css/style.css` & `mia-accounting-1.5.5/src/accounting/static/css/style.css`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/static/js/account-form.js` & `mia-accounting-1.5.5/src/accounting/static/js/account-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/static/js/account-order.js` & `mia-accounting-1.5.5/src/accounting/static/js/account-order.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/static/js/currency-form.js` & `mia-accounting-1.5.5/src/accounting/static/js/currency-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/static/js/description-editor.js` & `mia-accounting-1.5.5/src/accounting/static/js/description-editor.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/static/js/drag-and-drop-reorder.js` & `mia-accounting-1.5.5/src/accounting/static/js/drag-and-drop-reorder.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/static/js/journal-entry-account-selector.js` & `mia-accounting-1.5.5/src/accounting/static/js/journal-entry-account-selector.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/static/js/journal-entry-form.js` & `mia-accounting-1.5.5/src/accounting/static/js/journal-entry-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/static/js/journal-entry-line-item-editor.js` & `mia-accounting-1.5.5/src/accounting/static/js/journal-entry-line-item-editor.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/static/js/journal-entry-order.js` & `mia-accounting-1.5.5/src/accounting/static/js/journal-entry-order.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/static/js/material-fab-speed-dial.js` & `mia-accounting-1.5.5/src/accounting/static/js/material-fab-speed-dial.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/static/js/option-form.js` & `mia-accounting-1.5.5/src/accounting/static/js/option-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/static/js/original-line-item-selector.js` & `mia-accounting-1.5.5/src/accounting/static/js/original-line-item-selector.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/static/js/period-chooser.js` & `mia-accounting-1.5.5/src/accounting/static/js/period-chooser.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/template_filters.py` & `mia-accounting-1.5.5/src/accounting/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/template_globals.py` & `mia-accounting-1.5.5/src/accounting/template_globals.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/account/create.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/account/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/account/detail.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/account/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/account/edit.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/account/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/account/include/form.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/account/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/account/list.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/account/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/account/order.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/account/order.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/base-account/detail.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/base-account/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/base-account/list.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/base-account/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/base.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/base.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/currency/create.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/currency/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/currency/detail.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/currency/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/currency/edit.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/currency/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/currency/include/form.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/currency/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/currency/list.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/currency/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/include/nav.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/include/nav.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/include/pagination.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/include/pagination.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/disbursement/create.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/disbursement/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/disbursement/detail.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/disbursement/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/disbursement/edit.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/disbursement/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,16 @@
  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  See the License for the specific language governing permissions and
  limitations under the License.
 
 Author: imacat@mail.imacat.idv.tw (imacat)
 First written: 2023/2/28
 #}
-<form id="accounting-description-editor-{{ description_editor.debit_credit }}" class="accounting-description-editor" name="accounting-dummy-form" data-debit-credit="{{ description_editor.debit_credit }}">
+<form id="accounting-description-editor-{{ description_editor.debit_credit }}" class="accounting-description-editor" data-debit-credit="{{ description_editor.debit_credit }}">
+  <input type="hidden" name="csrf_token" value="{{ csrf_token() }}">
   <div id="accounting-description-editor-{{ description_editor.debit_credit }}-modal" class="modal fade" tabindex="-1" aria-labelledby="accounting-description-editor-{{ description_editor.debit_credit }}-modal-label" aria-hidden="true">
     <div class="modal-dialog">
       <div class="modal-content">
         <div class="modal-header">
           <h1 class="modal-title fs-5" id="accounting-description-editor-{{ description_editor.debit_credit }}-modal-label">
             <label for="accounting-description-editor-{{ description_editor.debit_credit }}-description">{{ A_("Description") }}</label>
           </h1>
```

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/detail.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/form-currency.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/form-line-item.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/form-line-item.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/form.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,16 @@
  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  See the License for the specific language governing permissions and
  limitations under the License.
 
 Author: imacat@mail.imacat.idv.tw (imacat)
 First written: 2023/2/25
 #}
-<form id="accounting-line-item-editor" name="accounting-dummy-form">
+<form id="accounting-line-item-editor">
+  <input type="hidden" name="csrf_token" value="{{ csrf_token() }}">
   <div id="accounting-line-item-editor-modal" class="modal fade" tabindex="-1" aria-labelledby="accounting-line-item-editor-modal-label" aria-hidden="true">
     <div class="modal-dialog">
       <div class="modal-content">
         <div class="modal-header">
           <h1 class="modal-title fs-5" id="accounting-line-item-editor-modal-label">{{ A_("Line Item Content") }}</h1>
           <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="{{ A_("Close") }}"></button>
         </div>
```

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/order.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/order.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/receipt/create.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/receipt/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/receipt/detail.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/receipt/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/receipt/edit.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/receipt/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/receipt/include/form.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/receipt/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/transfer/create.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/transfer/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/transfer/detail.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/transfer/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/transfer/edit.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/transfer/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/journal-entry/transfer/include/form.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/journal-entry/transfer/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/option/detail.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/option/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/option/form.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/option/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/option/include/form-recurring-item.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/option/include/form-recurring-item.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,16 @@
  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  See the License for the specific language governing permissions and
  limitations under the License.
 
 Author: imacat@mail.imacat.idv.tw (imacat)
 First written: 2023/3/22
 #}
-<form id="accounting-recurring-item-editor-{{ expense_income }}" name="accounting-dummy-form">
+<form id="accounting-recurring-item-editor-{{ expense_income }}">
+  <input type="hidden" name="csrf_token" value="{{ csrf_token() }}">
   <div id="accounting-recurring-item-editor-{{ expense_income }}-modal" class="modal fade" tabindex="-1" aria-labelledby="accounting-recurring-item-editor-{{ expense_income }}-modal-label" aria-hidden="true">
     <div class="modal-dialog">
       <div class="modal-content">
         <div class="modal-header">
           <h1 class="modal-title fs-5" id="accounting-recurring-item-editor-{{ expense_income }}-modal-label">{{ title }}</h1>
           <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="{{ A_("Close") }}"></button>
         </div>
```

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/report/balance-sheet.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/report/balance-sheet.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/balance-sheet-section.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/balance-sheet-section.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/ledger-row-desktop.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/ledger-row-desktop.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/ledger-row-mobile.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/ledger-row-mobile.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/period-chooser.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/period-chooser.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/search-modal.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/search-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/report/include/toolbar-buttons.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/report/include/toolbar-buttons.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/report/income-expenses.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/report/income-expenses.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/report/income-statement.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/report/income-statement.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/report/journal.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/report/journal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/report/ledger.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/report/ledger.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/report/search.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/report/search.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/report/trial-balance.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/report/trial-balance.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/report/unapplied-accounts.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/report/unapplied-accounts.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/report/unapplied.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/report/unapplied.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/report/unmatched-accounts.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/report/unmatched-accounts.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/templates/accounting/report/unmatched.html` & `mia-accounting-1.5.5/src/accounting/templates/accounting/report/unmatched.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/translations/accounting.pot` & `mia-accounting-1.5.5/src/accounting/translations/accounting.pot`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo` & `mia-accounting-1.5.5/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po` & `mia-accounting-1.5.5/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo` & `mia-accounting-1.5.5/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po` & `mia-accounting-1.5.5/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/utils/__init__.py` & `mia-accounting-1.5.5/src/accounting/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/utils/cast.py` & `mia-accounting-1.5.5/src/accounting/utils/cast.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/utils/current_account.py` & `mia-accounting-1.5.5/src/accounting/utils/current_account.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/utils/flash_errors.py` & `mia-accounting-1.5.5/src/accounting/utils/flash_errors.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/utils/journal_entry_types.py` & `mia-accounting-1.5.5/src/accounting/utils/journal_entry_types.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/utils/next_uri.py` & `mia-accounting-1.5.5/src/accounting/utils/next_uri.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 
 This module should not import any other module from the application.
 
 """
 from urllib.parse import urlparse, parse_qsl, ParseResult, urlencode, \
     urlunparse
 
-from flask import request, Blueprint
+from flask import request, Blueprint, current_app
+from itsdangerous import URLSafeSerializer, BadData
 
 
 def append_next(uri: str) -> str:
     """Appends the current URI as the next URI to the query argument.
 
     :param uri: The URI.
     :return: The URI with the current URI appended as the next URI.
@@ -37,58 +38,70 @@
 
 def inherit_next(uri: str) -> str:
     """Inherits the current next URI to the query argument, if exists.
 
     :param uri: The URI.
     :return: The URI with the current next URI added at the query argument.
     """
-    next_uri: str | None = __get_next_uri()
+    next_uri: str | None = __get_next()
     return uri if next_uri is None else __set_next(uri, next_uri)
 
 
 def or_next(uri: str) -> str:
     """Returns the next URI, if exists, or the supplied URI.
 
     :param uri: The URI.
     :return: The next URI or the supplied URI.
     """
-    next_uri: str | None = __get_next_uri()
+    next_uri: str | None = __get_next()
     return uri if next_uri is None else next_uri
 
 
-def __get_next_uri() -> str | None:
+def __get_next() -> str | None:
     """Returns the valid next URI.
 
     :return: The valid next URI.
     """
     next_uri: str | None = request.form.get("next") \
         if request.method == "POST" else request.args.get("next")
-    if next_uri is None or not next_uri.startswith("/"):
+    if next_uri is None:
+        return None
+    try:
+        return URLSafeSerializer(current_app.config["SECRET_KEY"])\
+            .loads(next_uri, "next")
+    except BadData:
         return None
-    if len(next_uri) > 512:
-        return next_uri[:512]
-    return next_uri
 
 
 def __set_next(uri: str, next_uri: str) -> str:
     """Sets the next URI to the query arguments.
 
     :param uri: The URI.
     :param next_uri: The next URI.
     :return: The URI with the next URI set.
     """
     uri_p: ParseResult = urlparse(uri)
     params: list[tuple[str, str]] = parse_qsl(uri_p.query)
     params = [x for x in params if x[0] != "next"]
-    params.append(("next", next_uri))
+    params.append(("next", encode_next(next_uri)))
     parts: list[str] = list(uri_p)
     parts[4] = urlencode(params)
     return urlunparse(parts)
 
 
+def encode_next(uri: str) -> str:
+    """Encodes the next URI.
+
+    :param uri: The next URI.
+    :return: The encoded next URI.
+    """
+    return URLSafeSerializer(current_app.config["SECRET_KEY"])\
+        .dumps(uri, "next")
+
+
 def init_app(bp: Blueprint) -> None:
     """Initializes the application.
 
     :param bp: The blueprint of the accounting application.
     :return: None.
     """
     bp.add_app_template_filter(append_next, "accounting_append_next")
```

### Comparing `mia-accounting-1.5.4/src/accounting/utils/offset_alias.py` & `mia-accounting-1.5.5/src/accounting/utils/offset_alias.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/utils/options.py` & `mia-accounting-1.5.5/src/accounting/utils/options.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/utils/pagination.py` & `mia-accounting-1.5.5/src/accounting/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/utils/permission.py` & `mia-accounting-1.5.5/src/accounting/utils/permission.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/utils/query.py` & `mia-accounting-1.5.5/src/accounting/utils/query.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/utils/random_id.py` & `mia-accounting-1.5.5/src/accounting/utils/random_id.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/utils/strip_text.py` & `mia-accounting-1.5.5/src/accounting/utils/strip_text.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/accounting/utils/user.py` & `mia-accounting-1.5.5/src/accounting/utils/user.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/src/mia_accounting.egg-info/PKG-INFO` & `mia-accounting-1.5.5/src/mia_accounting.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mia-accounting
-Version: 1.5.4
+Version: 1.5.5
 Summary: A Flask accounting module.
 Author-email: imacat <imacat@mail.imacat.idv.tw>
 Project-URL: Documentation, https://mia-accounting.readthedocs.io
 Project-URL: Change Log, https://mia-accounting.readthedocs.io/en/latest/changelog.html
 Project-URL: Repository, https://github.com/imacat/mia-accounting
 Project-URL: Bug Tracker, https://github.com/imacat/mia-accounting/issues
 Project-URL: Demonstration, https://accounting.imacat.idv.tw
```

### Comparing `mia-accounting-1.5.4/src/mia_accounting.egg-info/SOURCES.txt` & `mia-accounting-1.5.5/src/mia_accounting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/tests/babel-utils-test-site.py` & `mia-accounting-1.5.5/tests/babel-utils-test-site.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/tests/babel-utils.py` & `mia-accounting-1.5.5/tests/babel-utils.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/tests/test_account.py` & `mia-accounting-1.5.5/tests/test_account.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 """
 import datetime as dt
 import unittest
 
 import httpx
 from flask import Flask
 
+from accounting.utils.next_uri import encode_next
 from test_site import db
 from testlib import NEXT_URI, create_test_app, get_client, set_locale, \
     add_journal_entry
 
 
 class AccountData:
     """The account data."""
@@ -74,14 +75,15 @@
         self.app: Flask = create_test_app()
 
         with self.app.app_context():
             from accounting.models import Account, AccountL10n
             AccountL10n.query.delete()
             Account.query.delete()
             db.session.commit()
+            self.encoded_next_uri: str = encode_next(NEXT_URI)
 
         self.client, self.csrf_token = get_client(self.app, "editor")
         response: httpx.Response
 
         response = self.client.post(f"{PREFIX}/store",
                                     data={"csrf_token": self.csrf_token,
                                           "base_code": CASH.base_code,
@@ -139,15 +141,15 @@
         self.assertEqual(response.status_code, 403)
 
         with self.app.app_context():
             cash_id: int = Account.find_by_code(CASH.code).id
 
         response = client.post(f"{PREFIX}/bases/{CASH.base_code}",
                                data={"csrf_token": csrf_token,
-                                     "next": NEXT_URI,
+                                     "next": self.encoded_next_uri,
                                      f"{cash_id}-no": "5"})
         self.assertEqual(response.status_code, 403)
 
     def test_viewer(self) -> None:
         """Test the permission as viewer.
 
         :return: None.
@@ -188,15 +190,15 @@
         self.assertEqual(response.status_code, 200)
 
         with self.app.app_context():
             cash_id: int = Account.find_by_code(CASH.code).id
 
         response = client.post(f"{PREFIX}/bases/{CASH.base_code}",
                                data={"csrf_token": csrf_token,
-                                     "next": NEXT_URI,
+                                     "next": self.encoded_next_uri,
                                      f"{cash_id}-no": "5"})
         self.assertEqual(response.status_code, 403)
 
     def test_editor(self) -> None:
         """Test the permission as editor.
 
         :return: None.
@@ -240,15 +242,15 @@
         self.assertEqual(response.status_code, 200)
 
         with self.app.app_context():
             cash_id: int = Account.find_by_code(CASH.code).id
 
         response = self.client.post(f"{PREFIX}/bases/{CASH.base_code}",
                                     data={"csrf_token": self.csrf_token,
-                                          "next": NEXT_URI,
+                                          "next": self.encoded_next_uri,
                                           f"{cash_id}-no": "5"})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], NEXT_URI)
 
     def test_add(self) -> None:
         """Tests to add the currencies.
 
@@ -522,45 +524,45 @@
         response: httpx.Response
 
         with self.app.app_context():
             account = Account.find_by_code(CASH.code)
             self.assertEqual(account.title_l10n, CASH.title)
             self.assertEqual(account.l10n, [])
 
-        set_locale(self.client, self.csrf_token, "zh_Hant")
+        set_locale(self.app, self.client, self.csrf_token, "zh_Hant")
 
         response = self.client.post(update_uri,
                                     data={"csrf_token": self.csrf_token,
                                           "base_code": CASH.base_code,
                                           "title": f"{CASH.title}-zh_Hant"})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
         with self.app.app_context():
             account = Account.find_by_code(CASH.code)
             self.assertEqual(account.title_l10n, CASH.title)
             self.assertEqual({(x.locale, x.title) for x in account.l10n},
                              {("zh_Hant", f"{CASH.title}-zh_Hant")})
 
-        set_locale(self.client, self.csrf_token, "en")
+        set_locale(self.app, self.client, self.csrf_token, "en")
 
         response = self.client.post(update_uri,
                                     data={"csrf_token": self.csrf_token,
                                           "base_code": CASH.base_code,
                                           "title": f"{CASH.title}-2"})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
         with self.app.app_context():
             account = Account.find_by_code(CASH.code)
             self.assertEqual(account.title_l10n, f"{CASH.title}-2")
             self.assertEqual({(x.locale, x.title) for x in account.l10n},
                              {("zh_Hant", f"{CASH.title}-zh_Hant")})
 
-        set_locale(self.client, self.csrf_token, "zh_Hant")
+        set_locale(self.app, self.client, self.csrf_token, "zh_Hant")
 
         response = self.client.post(update_uri,
                                     data={"csrf_token": self.csrf_token,
                                           "base_code": CASH.base_code,
                                           "title": f"{CASH.title}-zh_Hant-2"})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
@@ -587,15 +589,15 @@
                                           "base_code": PETTY.base_code,
                                           "title": PETTY.title})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
         add_journal_entry(self.client,
                           form={"csrf_token": self.csrf_token,
-                                "next": NEXT_URI,
+                                "next": self.encoded_next_uri,
                                 "date": dt.date.today().isoformat(),
                                 "currency-1-code": "USD",
                                 "currency-1-credit-1-account_code": BANK.code,
                                 "currency-1-credit-1-amount": "20"})
 
         with self.app.app_context():
             self.assertEqual({x.code for x in Account.query.all()},
@@ -705,15 +707,15 @@
             id_2: int = Account.find_by_code("1111-002").id
             id_3: int = Account.find_by_code("1111-003").id
             id_4: int = Account.find_by_code("1111-004").id
             id_5: int = Account.find_by_code("1111-005").id
 
         response = self.client.post(f"{PREFIX}/bases/1111",
                                     data={"csrf_token": self.csrf_token,
-                                          "next": NEXT_URI,
+                                          "next": self.encoded_next_uri,
                                           f"{id_1}-no": "4",
                                           f"{id_2}-no": "1",
                                           f"{id_3}-no": "5",
                                           f"{id_4}-no": "2",
                                           f"{id_5}-no": "3"})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], NEXT_URI)
@@ -732,15 +734,15 @@
             db.session.get(Account, id_3).no = 6
             db.session.get(Account, id_4).no = 8
             db.session.get(Account, id_5).no = 9
             db.session.commit()
 
         response = self.client.post(f"{PREFIX}/bases/1111",
                                     data={"csrf_token": self.csrf_token,
-                                          "next": NEXT_URI,
+                                          "next": self.encoded_next_uri,
                                           f"{id_2}-no": "3a",
                                           f"{id_3}-no": "5",
                                           f"{id_4}-no": "2"})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], NEXT_URI)
 
         with self.app.app_context():
```

### Comparing `mia-accounting-1.5.4/tests/test_base_account.py` & `mia-accounting-1.5.5/tests/test_base_account.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/tests/test_commands.py` & `mia-accounting-1.5.5/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/tests/test_currency.py` & `mia-accounting-1.5.5/tests/test_currency.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 """
 import datetime as dt
 import unittest
 
 import httpx
 from flask import Flask
 
+from accounting.utils.next_uri import encode_next
 from test_site import db
 from testlib import NEXT_URI, create_test_app, get_client, set_locale, \
     add_journal_entry
 
 
 class CurrencyData:
     """The currency data."""
@@ -464,45 +465,45 @@
         response: httpx.Response
 
         with self.app.app_context():
             currency = db.session.get(Currency, USD.code)
             self.assertEqual(currency.name_l10n, USD.name)
             self.assertEqual(currency.l10n, [])
 
-        set_locale(self.client, self.csrf_token, "zh_Hant")
+        set_locale(self.app, self.client, self.csrf_token, "zh_Hant")
 
         response = self.client.post(update_uri,
                                     data={"csrf_token": self.csrf_token,
                                           "code": USD.code,
                                           "name": f"{USD.name}-zh_Hant"})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
         with self.app.app_context():
             currency = db.session.get(Currency, USD.code)
             self.assertEqual(currency.name_l10n, USD.name)
             self.assertEqual({(x.locale, x.name) for x in currency.l10n},
                              {("zh_Hant", f"{USD.name}-zh_Hant")})
 
-        set_locale(self.client, self.csrf_token, "en")
+        set_locale(self.app, self.client, self.csrf_token, "en")
 
         response = self.client.post(update_uri,
                                     data={"csrf_token": self.csrf_token,
                                           "code": USD.code,
                                           "name": f"{USD.name}-2"})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
         with self.app.app_context():
             currency = db.session.get(Currency, USD.code)
             self.assertEqual(currency.name_l10n, f"{USD.name}-2")
             self.assertEqual({(x.locale, x.name) for x in currency.l10n},
                              {("zh_Hant", f"{USD.name}-zh_Hant")})
 
-        set_locale(self.client, self.csrf_token, "zh_Hant")
+        set_locale(self.app, self.client, self.csrf_token, "zh_Hant")
 
         response = self.client.post(update_uri,
                                     data={"csrf_token": self.csrf_token,
                                           "code": USD.code,
                                           "name": f"{USD.name}-zh_Hant-2"})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
@@ -517,27 +518,29 @@
         """Tests to delete a currency.
 
         :return: None.
         """
         from accounting.models import Currency
         detail_uri: str = f"{PREFIX}/{JPY.code}"
         delete_uri: str = f"{PREFIX}/{JPY.code}/delete"
+        with self.app.app_context():
+            encoded_next_uri: str = encode_next(NEXT_URI)
         list_uri: str = PREFIX
         response: httpx.Response
 
         response = self.client.post(f"{PREFIX}/store",
                                     data={"csrf_token": self.csrf_token,
                                           "code": JPY.code,
                                           "name": JPY.name})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
         add_journal_entry(self.client,
                           form={"csrf_token": self.csrf_token,
-                                "next": NEXT_URI,
+                                "next": encoded_next_uri,
                                 "date": dt.date.today().isoformat(),
                                 "currency-1-code": EUR.code,
                                 "currency-1-credit-1-account_code": "1111-001",
                                 "currency-1-credit-1-amount": "20"})
 
         with self.app.app_context():
             self.assertEqual({x.code for x in Currency.query.all()},
```

### Comparing `mia-accounting-1.5.4/tests/test_description_editor.py` & `mia-accounting-1.5.5/tests/test_description_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 """
 import datetime as dt
 import unittest
 
 from flask import Flask
 
+from accounting.utils.next_uri import encode_next
 from testlib import NEXT_URI, Accounts, create_test_app, get_client, \
     add_journal_entry
 
 
 class DescriptionEditorTestCase(unittest.TestCase):
     """The description editor test case."""
 
@@ -37,25 +38,26 @@
         """
         self.app: Flask = create_test_app()
 
         with self.app.app_context():
             from accounting.models import JournalEntry, JournalEntryLineItem
             JournalEntry.query.delete()
             JournalEntryLineItem.query.delete()
+            self.encoded_next_uri: str = encode_next(NEXT_URI)
 
         self.client, self.csrf_token = get_client(self.app, "editor")
 
     def test_description_editor(self) -> None:
         """Test the description editor.
 
         :return: None.
         """
         from accounting.journal_entry.utils.description_editor import \
             DescriptionEditor
-        for form in get_form_data(self.csrf_token):
+        for form in get_form_data(self.csrf_token, self.encoded_next_uri):
             add_journal_entry(self.client, form)
         with self.app.app_context():
             editor: DescriptionEditor = DescriptionEditor()
 
         # Debit-General
         self.assertEqual(len(editor.debit.general.tags), 2)
         self.assertEqual(editor.debit.general.tags[0].name, "Lunch")
@@ -139,30 +141,32 @@
                          Accounts.PETTY_CASH)
         self.assertEqual(editor.credit.bus.tags[1].name, "Bus")
         self.assertEqual(len(editor.credit.bus.tags[1].accounts), 1)
         self.assertEqual(editor.credit.bus.tags[1].accounts[0].code,
                          Accounts.PREPAID)
 
 
-def get_form_data(csrf_token: str) -> list[dict[str, str]]:
+def get_form_data(csrf_token: str, encoded_next_uri: str) \
+        -> list[dict[str, str]]:
     """Returns the form data for multiple journal entry forms.
 
     :param csrf_token: The CSRF token.
+    :param encoded_next_uri: The encoded next URI.
     :return: A list of the form data.
     """
     journal_entry_date: str = dt.date.today().isoformat()
     return [{"csrf_token": csrf_token,
-             "next": NEXT_URI,
+             "next": encoded_next_uri,
              "date": journal_entry_date,
              "currency-0-code": "USD",
              "currency-0-credit-0-account_code": Accounts.SERVICE,
              "currency-0-credit-0-description": " Salary ",
              "currency-0-credit-0-amount": "2500"},
             {"csrf_token": csrf_token,
-             "next": NEXT_URI,
+             "next": encoded_next_uri,
              "date": journal_entry_date,
              "currency-0-code": "USD",
              "currency-0-debit-0-account_code": Accounts.MEAL,
              "currency-0-debit-0-description": " Lunch—Fish ",
              "currency-0-debit-0-amount": "4.7",
              "currency-0-credit-0-account_code": Accounts.BANK,
              "currency-0-credit-0-description": " Lunch—Fish ",
@@ -176,15 +180,15 @@
              "currency-0-debit-2-account_code": Accounts.MEAL,
              "currency-0-debit-2-description": " Dinner—Hamburger ",
              "currency-0-debit-2-amount": "4.25",
              "currency-0-credit-2-account_code": Accounts.BANK,
              "currency-0-credit-2-description": " Dinner—Hamburger ",
              "currency-0-credit-2-amount": "4.25"},
             {"csrf_token": csrf_token,
-             "next": NEXT_URI,
+             "next": encoded_next_uri,
              "date": journal_entry_date,
              "currency-0-code": "USD",
              "currency-0-debit-0-account_code": Accounts.MEAL,
              "currency-0-debit-0-description": " Lunch—Salad ",
              "currency-0-debit-0-amount": "4.99",
              "currency-0-credit-0-account_code": Accounts.CASH,
              "currency-0-credit-0-description": " Lunch—Salad ",
@@ -192,15 +196,15 @@
              "currency-0-debit-1-account_code": Accounts.MEAL,
              "currency-0-debit-1-description": " Dinner—Steak  ",
              "currency-0-debit-1-amount": "8.28",
              "currency-0-credit-1-account_code": Accounts.PETTY_CASH,
              "currency-0-credit-1-description": " Dinner—Steak ",
              "currency-0-credit-1-amount": "8.28"},
             {"csrf_token": csrf_token,
-             "next": NEXT_URI,
+             "next": encoded_next_uri,
              "date": journal_entry_date,
              "currency-0-code": "USD",
              "currency-0-debit-0-account_code": Accounts.MEAL,
              "currency-0-debit-0-description": " Lunch—Pizza  ",
              "currency-0-debit-0-amount": "5.49",
              "currency-0-credit-0-account_code": Accounts.PETTY_CASH,
              "currency-0-credit-0-description": " Lunch—Pizza ",
@@ -208,22 +212,22 @@
              "currency-0-debit-1-account_code": Accounts.MEAL,
              "currency-0-debit-1-description": " Lunch—Noodles ",
              "currency-0-debit-1-amount": "7.47",
              "currency-0-credit-1-account_code": Accounts.PETTY_CASH,
              "currency-0-credit-1-description": " Lunch—Noodles ",
              "currency-0-credit-1-amount": "7.47"},
             {"csrf_token": csrf_token,
-             "next": NEXT_URI,
+             "next": encoded_next_uri,
              "date": journal_entry_date,
              "currency-0-code": "USD",
              "currency-0-debit-0-account_code": Accounts.TRAVEL,
              "currency-0-debit-0-description": " Airplane—Lake City↔Hill Town",
              "currency-0-debit-0-amount": "800"},
             {"csrf_token": csrf_token,
-             "next": NEXT_URI,
+             "next": encoded_next_uri,
              "date": journal_entry_date,
              "currency-0-code": "USD",
              "currency-0-debit-0-account_code": Accounts.TRAVEL,
              "currency-0-debit-0-description": " Bus—323—Downtown→Museum ",
              "currency-0-debit-0-amount": "2.5",
              "currency-0-credit-0-account_code": Accounts.PREPAID,
              "currency-0-credit-0-description": " Bus—323—Downtown→Museum ",
@@ -243,15 +247,15 @@
              "currency-0-debit-3-account_code": Accounts.TRAVEL,
              "currency-0-debit-3-description": " Train—Red—Mall→Museum ",
              "currency-0-debit-3-amount": "4.4",
              "currency-0-credit-3-account_code": Accounts.PETTY_CASH,
              "currency-0-credit-3-description": " Train—Red—Mall→Museum ",
              "currency-0-credit-3-amount": "4.4"},
             {"csrf_token": csrf_token,
-             "next": NEXT_URI,
+             "next": encoded_next_uri,
              "date": journal_entry_date,
              "currency-0-code": "USD",
              "currency-0-debit-0-account_code": Accounts.TRAVEL,
              "currency-0-debit-0-description": " Taxi—Museum→Office ",
              "currency-0-debit-0-amount": "15.5",
              "currency-0-credit-0-account_code": Accounts.CASH,
              "currency-0-credit-0-description": " Taxi—Museum→Office ",
@@ -289,15 +293,15 @@
              "currency-0-debit-6-account_code": Accounts.TRAVEL,
              "currency-0-debit-6-description": " Bike—Theatre→Home ",
              "currency-0-debit-6-amount": "5.5",
              "currency-0-credit-6-account_code": Accounts.PREPAID,
              "currency-0-credit-6-description": " Bike—Theatre→Home ",
              "currency-0-credit-6-amount": "5.5"},
             {"csrf_token": csrf_token,
-             "next": NEXT_URI,
+             "next": encoded_next_uri,
              "date": journal_entry_date,
              "currency-0-code": "USD",
              "currency-0-debit-0-account_code": Accounts.PETTY_CASH,
              "currency-0-debit-0-description": " Dinner—Steak  ",
              "currency-0-debit-0-amount": "8.28",
              "currency-0-credit-0-account_code": Accounts.BANK,
              "currency-0-credit-0-description": " Dinner—Steak ",
```

### Comparing `mia-accounting-1.5.4/tests/test_journal_entry.py` & `mia-accounting-1.5.5/tests/test_journal_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import datetime as dt
 import unittest
 from decimal import Decimal
 
 import httpx
 from flask import Flask
 
+from accounting.utils.next_uri import encode_next
 from test_site import db
 from testlib import NEXT_URI, Accounts, create_test_app, get_client, \
     add_journal_entry, match_journal_entry_detail
 from testlib_journal_entry import NON_EMPTY_NOTE, EMPTY_NOTE, \
     get_add_form, get_unchanged_update_form, get_update_form, \
     set_negative_amount, remove_debit_in_a_currency, \
     remove_credit_in_a_currency
@@ -49,14 +50,15 @@
         """
         self.app: Flask = create_test_app()
 
         with self.app.app_context():
             from accounting.models import JournalEntry, JournalEntryLineItem
             JournalEntry.query.delete()
             JournalEntryLineItem.query.delete()
+            self.encoded_next_uri: str = encode_next(NEXT_URI)
 
         self.client, self.csrf_token = get_client(self.app, "editor")
 
     def test_nobody(self) -> None:
         """Test the permission as nobody.
 
         :return: None.
@@ -149,28 +151,30 @@
         response = self.client.get(f"{PREFIX}/{journal_entry_id}/edit")
         self.assertEqual(response.status_code, 200)
 
         response = self.client.post(f"{PREFIX}/{journal_entry_id}/update",
                                     data=update_form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"],
-                         f"{PREFIX}/{journal_entry_id}?next=%2F_next")
+                         f"{PREFIX}/{journal_entry_id}?"
+                         f"next={self.encoded_next_uri}")
 
         response = self.client.post(f"{PREFIX}/{journal_entry_id}/delete",
                                     data={"csrf_token": self.csrf_token})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], RETURN_TO_URI)
 
     def test_add(self) -> None:
         """Tests to add the journal entries.
 
         :return: None.
         """
         from accounting.models import JournalEntry, JournalEntryCurrency
-        create_uri: str = f"{PREFIX}/create/receipt?next=%2F_next"
+        create_uri: str = (f"{PREFIX}/create/receipt?"
+                           f"next={self.encoded_next_uri}")
         store_uri: str = f"{PREFIX}/store/receipt"
         response: httpx.Response
         form: dict[str, str]
         journal_entry: JournalEntry | None
 
         # No currency content
         form = self.__get_add_form()
@@ -318,16 +322,18 @@
         """Tests the basic rules to update a journal entry.
 
         :return: None.
         """
         from accounting.models import JournalEntry, JournalEntryCurrency
         journal_entry_id: int \
             = add_journal_entry(self.client, self.__get_add_form())
-        detail_uri: str = f"{PREFIX}/{journal_entry_id}?next=%2F_next"
-        edit_uri: str = f"{PREFIX}/{journal_entry_id}/edit?next=%2F_next"
+        detail_uri: str = (f"{PREFIX}/{journal_entry_id}?"
+                           f"next={self.encoded_next_uri}")
+        edit_uri: str = (f"{PREFIX}/{journal_entry_id}/edit?"
+                         f"next={self.encoded_next_uri}")
         update_uri: str = f"{PREFIX}/{journal_entry_id}/update"
         form_0: dict[str, str] = self.__get_update_form(journal_entry_id)
 
         with self.app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertIsNotNone(journal_entry)
             currencies0: list[JournalEntryCurrency] = journal_entry.currencies
@@ -481,15 +487,16 @@
         """Tests that the data is not modified.
 
         :return: None.
         """
         from accounting.models import JournalEntry
         journal_entry_id: int \
             = add_journal_entry(self.client, self.__get_add_form())
-        detail_uri: str = f"{PREFIX}/{journal_entry_id}?next=%2F_next"
+        detail_uri: str = (f"{PREFIX}/{journal_entry_id}?"
+                           f"next={self.encoded_next_uri}")
         update_uri: str = f"{PREFIX}/{journal_entry_id}/update"
         journal_entry: JournalEntry
         response: httpx.Response
 
         response = self.client.post(
             update_uri,
             data=self.__get_unchanged_update_form(journal_entry_id))
@@ -520,15 +527,16 @@
         :return: None.
         """
         from accounting.models import JournalEntry
         journal_entry_id: int \
             = add_journal_entry(self.client, self.__get_add_form())
         editor_username, admin_username = "editor", "admin"
         client, csrf_token = get_client(self.app, admin_username)
-        detail_uri: str = f"{PREFIX}/{journal_entry_id}?next=%2F_next"
+        detail_uri: str = (f"{PREFIX}/{journal_entry_id}?"
+                           f"next={self.encoded_next_uri}")
         update_uri: str = f"{PREFIX}/{journal_entry_id}/update"
         journal_entry: JournalEntry
         response: httpx.Response
 
         with self.app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertEqual(journal_entry.created_by.username,
@@ -553,15 +561,16 @@
         """Tests to delete a journal entry.
 
         :return: None.
         """
         from accounting.models import JournalEntry, JournalEntryLineItem
         journal_entry_id_1: int \
             = add_journal_entry(self.client, self.__get_add_form())
-        detail_uri: str = f"{PREFIX}/{journal_entry_id_1}?next=%2F_next"
+        detail_uri: str = (f"{PREFIX}/{journal_entry_id_1}?"
+                           f"next={self.encoded_next_uri}")
         delete_uri: str = f"{PREFIX}/{journal_entry_id_1}/delete"
         response: httpx.Response
 
         form: dict[str, str] = self.__get_add_form()
         key: str = [x for x in form if x.endswith("-account_code")][0]
         form[key] = Accounts.PAYABLE
         journal_entry_id_2: int = add_journal_entry(self.client, form)
@@ -571,78 +580,81 @@
             self.assertIsNotNone(journal_entry)
             line_item: JournalEntryLineItem \
                 = [x for x in journal_entry.line_items
                    if x.account_code == Accounts.PAYABLE][0]
         add_journal_entry(
             self.client,
             form={"csrf_token": self.csrf_token,
-                  "next": NEXT_URI,
+                  "next": self.encoded_next_uri,
                   "date": dt.date.today().isoformat(),
                   "currency-1-code": line_item.currency_code,
                   "currency-1-debit-1-original_line_item_id": line_item.id,
                   "currency-1-debit-1-account_code": line_item.account_code,
                   "currency-1-debit-1-amount": "1"})
 
         # Cannot delete the journal entry that is in use
         response = self.client.post(f"{PREFIX}/{journal_entry_id_2}/delete",
                                     data={"csrf_token": self.csrf_token,
-                                          "next": NEXT_URI})
+                                          "next": self.encoded_next_uri})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"],
-                         f"{PREFIX}/{journal_entry_id_2}?next=%2F_next")
+                         f"{PREFIX}/{journal_entry_id_2}?"
+                         f"next={self.encoded_next_uri}")
 
         # Success
         response = self.client.get(detail_uri)
         self.assertEqual(response.status_code, 200)
         response = self.client.post(delete_uri,
                                     data={"csrf_token": self.csrf_token,
-                                          "next": NEXT_URI})
+                                          "next": self.encoded_next_uri})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], NEXT_URI)
 
         response = self.client.get(detail_uri)
         self.assertEqual(response.status_code, 404)
         response = self.client.post(delete_uri,
                                     data={"csrf_token": self.csrf_token,
-                                          "next": NEXT_URI})
+                                          "next": self.encoded_next_uri})
         self.assertEqual(response.status_code, 404)
 
     def __get_add_form(self) -> dict[str, str]:
         """Returns the form data to add a new journal entry.
 
         :return: The form data to add a new journal entry.
         """
-        form: dict[str, str] = get_add_form(self.csrf_token)
+        form: dict[str, str] = get_add_form(self.csrf_token,
+                                            self.encoded_next_uri)
         form = {x: form[x] for x in form if "-debit-" not in x}
         return form
 
     def __get_unchanged_update_form(self, journal_entry_id: int) \
             -> dict[str, str]:
         """Returns the form data to update a journal entry, where the data are
         not changed.
 
         :param journal_entry_id: The journal entry ID.
         :return: The form data to update the journal entry, where the data are
             not changed.
         """
         form: dict[str, str] = get_unchanged_update_form(
-            journal_entry_id, self.app, self.csrf_token)
+            journal_entry_id, self.app, self.csrf_token, self.encoded_next_uri)
         form = {x: form[x] for x in form if "-debit-" not in x}
         return form
 
     def __get_update_form(self, journal_entry_id: int) -> dict[str, str]:
         """Returns the form data to update a journal entry, where the data are
         changed.
 
         :param journal_entry_id: The journal entry ID.
         :return: The form data to update the journal entry, where the data are
             changed.
         """
         form: dict[str, str] = get_update_form(
-            journal_entry_id, self.app, self.csrf_token, False)
+            journal_entry_id, self.app, self.csrf_token, self.encoded_next_uri,
+            False)
         form = {x: form[x] for x in form if "-debit-" not in x}
         return form
 
 
 class CashDisbursementJournalEntryTestCase(unittest.TestCase):
     """The cash disbursement journal entry test case."""
 
@@ -654,14 +666,15 @@
         """
         self.app: Flask = create_test_app()
 
         with self.app.app_context():
             from accounting.models import JournalEntry, JournalEntryLineItem
             JournalEntry.query.delete()
             JournalEntryLineItem.query.delete()
+            self.encoded_next_uri: str = encode_next(NEXT_URI)
 
         self.client, self.csrf_token = get_client(self.app, "editor")
 
     def test_nobody(self) -> None:
         """Test the permission as nobody.
 
         :return: None.
@@ -754,28 +767,30 @@
         response = self.client.get(f"{PREFIX}/{journal_entry_id}/edit")
         self.assertEqual(response.status_code, 200)
 
         response = self.client.post(f"{PREFIX}/{journal_entry_id}/update",
                                     data=update_form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"],
-                         f"{PREFIX}/{journal_entry_id}?next=%2F_next")
+                         f"{PREFIX}/{journal_entry_id}?"
+                         f"next={self.encoded_next_uri}")
 
         response = self.client.post(f"{PREFIX}/{journal_entry_id}/delete",
                                     data={"csrf_token": self.csrf_token})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], RETURN_TO_URI)
 
     def test_add(self) -> None:
         """Tests to add the journal entries.
 
         :return: None.
         """
         from accounting.models import JournalEntry, JournalEntryCurrency
-        create_uri: str = f"{PREFIX}/create/disbursement?next=%2F_next"
+        create_uri: str = (f"{PREFIX}/create/disbursement?"
+                           f"next={self.encoded_next_uri}")
         store_uri: str = f"{PREFIX}/store/disbursement"
         response: httpx.Response
         form: dict[str, str]
         journal_entry: JournalEntry | None
 
         # No currency content
         form = self.__get_add_form()
@@ -926,16 +941,18 @@
         """Tests the basic rules to update a journal entry.
 
         :return: None.
         """
         from accounting.models import JournalEntry, JournalEntryCurrency
         journal_entry_id: int \
             = add_journal_entry(self.client, self.__get_add_form())
-        detail_uri: str = f"{PREFIX}/{journal_entry_id}?next=%2F_next"
-        edit_uri: str = f"{PREFIX}/{journal_entry_id}/edit?next=%2F_next"
+        detail_uri: str = (f"{PREFIX}/{journal_entry_id}?"
+                           f"next={self.encoded_next_uri}")
+        edit_uri: str = (f"{PREFIX}/{journal_entry_id}/edit?"
+                         f"next={self.encoded_next_uri}")
         update_uri: str = f"{PREFIX}/{journal_entry_id}/update"
         form_0: dict[str, str] = self.__get_update_form(journal_entry_id)
 
         with self.app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertIsNotNone(journal_entry)
             currencies0: list[JournalEntryCurrency] = journal_entry.currencies
@@ -1093,15 +1110,16 @@
         """Tests that the data is not modified.
 
         :return: None.
         """
         from accounting.models import JournalEntry
         journal_entry_id: int \
             = add_journal_entry(self.client, self.__get_add_form())
-        detail_uri: str = f"{PREFIX}/{journal_entry_id}?next=%2F_next"
+        detail_uri: str = (f"{PREFIX}/{journal_entry_id}?"
+                           f"next={self.encoded_next_uri}")
         update_uri: str = f"{PREFIX}/{journal_entry_id}/update"
         journal_entry: JournalEntry
         response: httpx.Response
 
         response = self.client.post(
             update_uri,
             data=self.__get_unchanged_update_form(journal_entry_id))
@@ -1132,15 +1150,16 @@
         :return: None.
         """
         from accounting.models import JournalEntry
         journal_entry_id: int \
             = add_journal_entry(self.client, self.__get_add_form())
         editor_username, admin_username = "editor", "admin"
         client, csrf_token = get_client(self.app, admin_username)
-        detail_uri: str = f"{PREFIX}/{journal_entry_id}?next=%2F_next"
+        detail_uri: str = (f"{PREFIX}/{journal_entry_id}?"
+                           f"next={self.encoded_next_uri}")
         update_uri: str = f"{PREFIX}/{journal_entry_id}/update"
         journal_entry: JournalEntry
         response: httpx.Response
 
         with self.app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertEqual(journal_entry.created_by.username,
@@ -1164,66 +1183,69 @@
     def test_delete(self) -> None:
         """Tests to delete a journal entry.
 
         :return: None.
         """
         journal_entry_id: int \
             = add_journal_entry(self.client, self.__get_add_form())
-        detail_uri: str = f"{PREFIX}/{journal_entry_id}?next=%2F_next"
+        detail_uri: str = (f"{PREFIX}/{journal_entry_id}?"
+                           f"next={self.encoded_next_uri}")
         delete_uri: str = f"{PREFIX}/{journal_entry_id}/delete"
         response: httpx.Response
 
         response = self.client.get(detail_uri)
         self.assertEqual(response.status_code, 200)
         response = self.client.post(delete_uri,
                                     data={"csrf_token": self.csrf_token,
-                                          "next": NEXT_URI})
+                                          "next": self.encoded_next_uri})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], NEXT_URI)
 
         response = self.client.get(detail_uri)
         self.assertEqual(response.status_code, 404)
         response = self.client.post(delete_uri,
                                     data={"csrf_token": self.csrf_token,
-                                          "next": NEXT_URI})
+                                          "next": self.encoded_next_uri})
         self.assertEqual(response.status_code, 404)
 
     def __get_add_form(self) -> dict[str, str]:
         """Returns the form data to add a new journal entry.
 
         :return: The form data to add a new journal entry.
         """
-        form: dict[str, str] = get_add_form(self.csrf_token)
+        form: dict[str, str] = get_add_form(self.csrf_token,
+                                            self.encoded_next_uri)
         form = {x: form[x] for x in form if "-credit-" not in x}
         return form
 
     def __get_unchanged_update_form(self, journal_entry_id: int) \
             -> dict[str, str]:
         """Returns the form data to update a journal entry, where the data are
         not changed.
 
         :param journal_entry_id: The journal entry ID.
         :return: The form data to update the journal entry, where the data are
             not changed.
         """
         form: dict[str, str] = get_unchanged_update_form(
-            journal_entry_id, self.app, self.csrf_token)
+            journal_entry_id, self.app, self.csrf_token, self.encoded_next_uri)
         form = {x: form[x] for x in form if "-credit-" not in x}
         return form
 
     def __get_update_form(self, journal_entry_id: int) -> dict[str, str]:
         """Returns the form data to update a journal entry, where the data are
         changed.
 
         :param journal_entry_id: The journal entry ID.
         :return: The form data to update the journal entry, where the data are
             changed.
         """
         form: dict[str, str] = get_update_form(
-            journal_entry_id, self.app, self.csrf_token, True)
+            journal_entry_id, self.app, self.csrf_token, self.encoded_next_uri,
+            True)
         form = {x: form[x] for x in form if "-credit-" not in x}
         return form
 
 
 class TransferJournalEntryTestCase(unittest.TestCase):
     """The transfer journal entry test case."""
 
@@ -1236,14 +1258,15 @@
         self.app: Flask = create_test_app()
 
         with self.app.app_context():
             from accounting.models import JournalEntry, \
                 JournalEntryLineItem
             JournalEntry.query.delete()
             JournalEntryLineItem.query.delete()
+            self.encoded_next_uri: str = encode_next(NEXT_URI)
 
         self.client, self.csrf_token = get_client(self.app, "editor")
 
     def test_nobody(self) -> None:
         """Test the permission as nobody.
 
         :return: None.
@@ -1336,28 +1359,30 @@
         response = self.client.get(f"{PREFIX}/{journal_entry_id}/edit")
         self.assertEqual(response.status_code, 200)
 
         response = self.client.post(f"{PREFIX}/{journal_entry_id}/update",
                                     data=update_form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"],
-                         f"{PREFIX}/{journal_entry_id}?next=%2F_next")
+                         f"{PREFIX}/{journal_entry_id}?"
+                         f"next={self.encoded_next_uri}")
 
         response = self.client.post(f"{PREFIX}/{journal_entry_id}/delete",
                                     data={"csrf_token": self.csrf_token})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], RETURN_TO_URI)
 
     def test_add(self) -> None:
         """Tests to add the journal entries.
 
         :return: None.
         """
         from accounting.models import JournalEntry, JournalEntryCurrency
-        create_uri: str = f"{PREFIX}/create/transfer?next=%2F_next"
+        create_uri: str = (f"{PREFIX}/create/transfer?"
+                           f"next={self.encoded_next_uri}")
         store_uri: str = f"{PREFIX}/store/transfer"
         response: httpx.Response
         form: dict[str, str]
         journal_entry: JournalEntry | None
 
         # No currency content
         form = self.__get_add_form()
@@ -1544,16 +1569,18 @@
         """Tests the basic rules to update a journal entry.
 
         :return: None.
         """
         from accounting.models import JournalEntry, JournalEntryCurrency
         journal_entry_id: int \
             = add_journal_entry(self.client, self.__get_add_form())
-        detail_uri: str = f"{PREFIX}/{journal_entry_id}?next=%2F_next"
-        edit_uri: str = f"{PREFIX}/{journal_entry_id}/edit?next=%2F_next"
+        detail_uri: str = (f"{PREFIX}/{journal_entry_id}?"
+                           f"next={self.encoded_next_uri}")
+        edit_uri: str = (f"{PREFIX}/{journal_entry_id}/edit?"
+                         f"next={self.encoded_next_uri}")
         update_uri: str = f"{PREFIX}/{journal_entry_id}/update"
         form_0: dict[str, str] = self.__get_update_form(journal_entry_id)
 
         with self.app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertIsNotNone(journal_entry)
             currencies0: list[JournalEntryCurrency] = journal_entry.currencies
@@ -1754,15 +1781,16 @@
         """Tests that the data is not modified.
 
         :return: None.
         """
         from accounting.models import JournalEntry
         journal_entry_id: int \
             = add_journal_entry(self.client, self.__get_add_form())
-        detail_uri: str = f"{PREFIX}/{journal_entry_id}?next=%2F_next"
+        detail_uri: str = (f"{PREFIX}/{journal_entry_id}?"
+                           f"next={self.encoded_next_uri}")
         update_uri: str = f"{PREFIX}/{journal_entry_id}/update"
         journal_entry: JournalEntry
         response: httpx.Response
 
         response = self.client.post(
             update_uri,
             data=self.__get_unchanged_update_form(journal_entry_id))
@@ -1793,15 +1821,16 @@
         :return: None.
         """
         from accounting.models import JournalEntry
         journal_entry_id: int \
             = add_journal_entry(self.client, self.__get_add_form())
         editor_username, admin_username = "editor", "admin"
         client, csrf_token = get_client(self.app, admin_username)
-        detail_uri: str = f"{PREFIX}/{journal_entry_id}?next=%2F_next"
+        detail_uri: str = (f"{PREFIX}/{journal_entry_id}?"
+                           f"next={self.encoded_next_uri}")
         update_uri: str = f"{PREFIX}/{journal_entry_id}/update"
         journal_entry: JournalEntry
         response: httpx.Response
 
         with self.app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertEqual(journal_entry.created_by.username,
@@ -1827,15 +1856,16 @@
         entry.
 
         :return: None.
         """
         from accounting.models import JournalEntry, JournalEntryCurrency
         journal_entry_id: int \
             = add_journal_entry(self.client, self.__get_add_form())
-        detail_uri: str = f"{PREFIX}/{journal_entry_id}?next=%2F_next"
+        detail_uri: str = (f"{PREFIX}/{journal_entry_id}?"
+                           f"next={self.encoded_next_uri}")
         update_uri: str = f"{PREFIX}/{journal_entry_id}/update?as=receipt"
         form_0: dict[str, str] = self.__get_update_form(journal_entry_id)
         form_0 = {x: form_0[x] for x in form_0 if "-debit-" not in x}
 
         with self.app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertIsNotNone(journal_entry)
@@ -1928,15 +1958,16 @@
         journal entry.
 
         :return: None.
         """
         from accounting.models import JournalEntry, JournalEntryCurrency
         journal_entry_id: int \
             = add_journal_entry(self.client, self.__get_add_form())
-        detail_uri: str = f"{PREFIX}/{journal_entry_id}?next=%2F_next"
+        detail_uri: str = (f"{PREFIX}/{journal_entry_id}?"
+                           f"next={self.encoded_next_uri}")
         update_uri: str = f"{PREFIX}/{journal_entry_id}/update?as=disbursement"
         form_0: dict[str, str] = self.__get_update_form(journal_entry_id)
         form_0 = {x: form_0[x] for x in form_0 if "-credit-" not in x}
 
         with self.app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             self.assertIsNotNone(journal_entry)
@@ -2031,62 +2062,64 @@
     def test_delete(self) -> None:
         """Tests to delete a journal entry.
 
         :return: None.
         """
         journal_entry_id: int \
             = add_journal_entry(self.client, self.__get_add_form())
-        detail_uri: str = f"{PREFIX}/{journal_entry_id}?next=%2F_next"
+        detail_uri: str = (f"{PREFIX}/{journal_entry_id}?"
+                           f"next={self.encoded_next_uri}")
         delete_uri: str = f"{PREFIX}/{journal_entry_id}/delete"
         response: httpx.Response
 
         response = self.client.get(detail_uri)
         self.assertEqual(response.status_code, 200)
         response = self.client.post(delete_uri,
                                     data={"csrf_token": self.csrf_token,
-                                          "next": NEXT_URI})
+                                          "next": self.encoded_next_uri})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], NEXT_URI)
 
         response = self.client.get(detail_uri)
         self.assertEqual(response.status_code, 404)
         response = self.client.post(delete_uri,
                                     data={"csrf_token": self.csrf_token,
-                                          "next": NEXT_URI})
+                                          "next": self.encoded_next_uri})
         self.assertEqual(response.status_code, 404)
 
     def __get_add_form(self) -> dict[str, str]:
         """Returns the form data to add a new journal entry.
 
         :return: The form data to add a new journal entry.
         """
-        return get_add_form(self.csrf_token)
+        return get_add_form(self.csrf_token, self.encoded_next_uri)
 
     def __get_unchanged_update_form(self, journal_entry_id: int) \
             -> dict[str, str]:
         """Returns the form data to update a journal entry, where the data are
         not changed.
 
         :param journal_entry_id: The journal entry ID.
         :return: The form data to update the journal entry, where the data are
             not changed.
         """
         return get_unchanged_update_form(
-            journal_entry_id, self.app, self.csrf_token)
+            journal_entry_id, self.app, self.csrf_token, self.encoded_next_uri)
 
     def __get_update_form(self, journal_entry_id: int) -> dict[str, str]:
         """Returns the form data to update a journal entry, where the data are
         changed.
 
         :param journal_entry_id: The journal entry ID.
         :return: The form data to update the journal entry, where the data are
             changed.
         """
-        return get_update_form(journal_entry_id,
-                               self.app, self.csrf_token, None)
+        return get_update_form(
+            journal_entry_id, self.app, self.csrf_token, self.encoded_next_uri,
+            None)
 
 
 class JournalEntryReorderTestCase(unittest.TestCase):
     """The journal entry reorder test case."""
 
     def setUp(self) -> None:
         """Sets up the test.
@@ -2096,14 +2129,15 @@
         """
         self.app: Flask = create_test_app()
 
         with self.app.app_context():
             from accounting.models import JournalEntry, JournalEntryLineItem
             JournalEntry.query.delete()
             JournalEntryLineItem.query.delete()
+            self.encoded_next_uri: str = encode_next(NEXT_URI)
 
         self.client, self.csrf_token = get_client(self.app, "editor")
 
     def test_change_date(self) -> None:
         """Tests to change the date of a journal entry.
 
         :return: None.
@@ -2143,21 +2177,21 @@
 
         form: dict[str, str] \
             = self.__get_disbursement_unchanged_update_form(id_2)
         form["date"] = journal_entry_date_2.isoformat()
         response = self.client.post(f"{PREFIX}/{id_2}/update", data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"],
-                         f"{PREFIX}/{id_2}?next=%2F_next")
+                         f"{PREFIX}/{id_2}?next={self.encoded_next_uri}")
 
         with self.app.app_context():
             self.assertEqual(db.session.get(JournalEntry, id_1).no, 1)
             self.assertEqual(db.session.get(JournalEntry, id_2).no, 3)
             self.assertEqual(db.session.get(JournalEntry, id_3).no, 2)
-            self.assertEqual(   db.session.get(JournalEntry, id_4).no, 1)
+            self.assertEqual(db.session.get(JournalEntry, id_4).no, 1)
             self.assertEqual(db.session.get(JournalEntry, id_5).no, 2)
 
     def test_reorder(self) -> None:
         """Tests to reorder the journal entries in a same day.
 
         :return: None.
         """
@@ -2177,15 +2211,15 @@
 
         with self.app.app_context():
             date: dt.date = db.session.get(JournalEntry, id_1).date
 
         response = self.client.post(
             f"{PREFIX}/dates/{date.isoformat()}",
             data={"csrf_token": self.csrf_token,
-                  "next": NEXT_URI,
+                  "next": self.encoded_next_uri,
                   f"{id_1}-no": "4",
                   f"{id_2}-no": "1",
                   f"{id_3}-no": "5",
                   f"{id_4}-no": "2",
                   f"{id_5}-no": "3"})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], NEXT_URI)
@@ -2205,15 +2239,15 @@
             db.session.get(JournalEntry, id_4).no = 8
             db.session.get(JournalEntry, id_5).no = 9
             db.session.commit()
 
         response = self.client.post(
             f"{PREFIX}/dates/{date.isoformat()}",
             data={"csrf_token": self.csrf_token,
-                  "next": NEXT_URI,
+                  "next": self.encoded_next_uri,
                   f"{id_2}-no": "3a",
                   f"{id_3}-no": "5",
                   f"{id_4}-no": "2"})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], NEXT_URI)
 
         with self.app.app_context():
@@ -2224,40 +2258,42 @@
             self.assertEqual(db.session.get(JournalEntry, id_5).no, 5)
 
     def __get_add_receipt_form(self) -> dict[str, str]:
         """Returns the form data to add a new cash receipt journal entry.
 
         :return: The form data to add a new cash receipt journal entry.
         """
-        form: dict[str, str] = get_add_form(self.csrf_token)
+        form: dict[str, str] = get_add_form(self.csrf_token,
+                                            self.encoded_next_uri)
         form = {x: form[x] for x in form if "-debit-" not in x}
         return form
 
     def __get_add_disbursement_form(self) -> dict[str, str]:
         """Returns the form data to add a new cash disbursement journal entry.
 
         :return: The form data to add a new cash disbursement journal entry.
         """
-        form: dict[str, str] = get_add_form(self.csrf_token)
+        form: dict[str, str] = get_add_form(self.csrf_token,
+                                            self.encoded_next_uri)
         form = {x: form[x] for x in form if "-credit-" not in x}
         return form
 
     def __get_disbursement_unchanged_update_form(self, journal_entry_id: int) \
             -> dict[str, str]:
         """Returns the form data to update a cash disbursement journal entry,
         where the data are not changed.
 
         :param journal_entry_id: The journal entry ID.
         :return: The form data to update the cash disbursement journal entry,
             where the data are not changed.
         """
         form: dict[str, str] = get_unchanged_update_form(
-            journal_entry_id, self.app, self.csrf_token)
+            journal_entry_id, self.app, self.csrf_token, self.encoded_next_uri)
         form = {x: form[x] for x in form if "-credit-" not in x}
         return form
 
     def __get_add_transfer_form(self) -> dict[str, str]:
         """Returns the form data to add a new journal entry.
 
         :return: The form data to add a new journal entry.
         """
-        return get_add_form(self.csrf_token)
+        return get_add_form(self.csrf_token, self.encoded_next_uri)
```

### Comparing `mia-accounting-1.5.4/tests/test_offset.py` & `mia-accounting-1.5.5/tests/test_offset.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 import unittest
 from decimal import Decimal
 
 import httpx
 from flask import Flask
 
+from accounting.utils.next_uri import encode_next
 from test_site import db
 from test_site.lib import JournalEntryLineItemData, JournalEntryCurrencyData, \
     JournalEntryData, BaseTestData
 from testlib import NEXT_URI, Accounts, create_test_app, get_client, \
     match_journal_entry_detail
 
 PREFIX: str = "/accounting/journal-entries"
@@ -46,26 +47,28 @@
         """
         self.app: Flask = create_test_app()
 
         with self.app.app_context():
             from accounting.models import JournalEntry, JournalEntryLineItem
             JournalEntry.query.delete()
             JournalEntryLineItem.query.delete()
+            self.encoded_next_uri: str = encode_next(NEXT_URI)
 
         self.client, self.csrf_token = get_client(self.app, "editor")
         self.data: OffsetTestData = OffsetTestData(self.app, "editor")
         self.data.populate()
 
     def test_add_receivable_offset(self) -> None:
         """Tests to add the receivable offset.
 
         :return: None.
         """
         from accounting.models import Account, JournalEntry
-        create_uri: str = f"{PREFIX}/create/receipt?next=%2F_next"
+        create_uri: str = (f"{PREFIX}/create/receipt?"
+                           f"next={self.encoded_next_uri}")
         store_uri: str = f"{PREFIX}/store/receipt"
         form: dict[str, str]
         old_amount: Decimal
         response: httpx.Response
 
         journal_entry_data: JournalEntryData = JournalEntryData(
             self.data.l_r_or3d.journal_entry.days, [JournalEntryCurrencyData(
@@ -81,22 +84,24 @@
                      original_line_item=self.data.l_r_or1d),
                  JournalEntryLineItemData(
                      Accounts.RECEIVABLE,
                      self.data.l_r_or3d.description, "100",
                      original_line_item=self.data.l_r_or3d)])])
 
         # Non-existing original line item ID
-        form = journal_entry_data.new_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.new_form(self.csrf_token,
+                                           self.encoded_next_uri)
         form["currency-1-credit-1-original_line_item_id"] = "9999"
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # The same debit or credit
-        form = journal_entry_data.new_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.new_form(self.csrf_token,
+                                           self.encoded_next_uri)
         form["currency-1-credit-1-original_line_item_id"] \
             = str(self.data.l_p_or1c.id)
         form["currency-1-credit-1-account_code"] = self.data.l_p_or1c.account
         form["currency-1-credit-1-amount"] = "100"
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
@@ -104,74 +109,82 @@
         # The original line item does not need offset
         with self.app.app_context():
             account = Account.find_by_code(Accounts.RECEIVABLE)
             account.is_need_offset = False
             db.session.commit()
         response = self.client.post(
             store_uri,
-            data=journal_entry_data.new_form(self.csrf_token, NEXT_URI))
+            data=journal_entry_data.new_form(self.csrf_token,
+                                             self.encoded_next_uri))
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
         with self.app.app_context():
             account = Account.find_by_code(Accounts.RECEIVABLE)
             account.is_need_offset = True
             db.session.commit()
 
         # The original line item is also an offset
-        form = journal_entry_data.new_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.new_form(self.csrf_token,
+                                           self.encoded_next_uri)
         form["currency-1-credit-1-original_line_item_id"] \
             = str(self.data.l_p_of1d.id)
         form["currency-1-credit-1-account_code"] = self.data.l_p_of1d.account
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Not the same currency
-        form = journal_entry_data.new_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.new_form(self.csrf_token,
+                                           self.encoded_next_uri)
         form["currency-1-code"] = "EUR"
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Not the same account
-        form = journal_entry_data.new_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.new_form(self.csrf_token,
+                                           self.encoded_next_uri)
         form["currency-1-credit-1-account_code"] = Accounts.NOTES_RECEIVABLE
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Not exceeding net balance - partially offset
-        form = journal_entry_data.new_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.new_form(self.csrf_token,
+                                           self.encoded_next_uri)
         form["currency-1-credit-1-amount"] \
             = str(journal_entry_data.currencies[0].credit[0].amount
                   + Decimal("0.01"))
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Not exceeding net balance - unmatched
-        form = journal_entry_data.new_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.new_form(self.csrf_token,
+                                           self.encoded_next_uri)
         form["currency-1-credit-3-amount"] \
             = str(journal_entry_data.currencies[0].credit[2].amount
                   + Decimal("0.01"))
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Not before the original line items
         old_days = journal_entry_data.days
         journal_entry_data.days = old_days + 1
-        form = journal_entry_data.new_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.new_form(self.csrf_token,
+                                           self.encoded_next_uri)
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
         journal_entry_data.days = old_days
 
         # Success
-        form = journal_entry_data.new_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.new_form(self.csrf_token,
+                                           self.encoded_next_uri)
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         journal_entry_id: int \
             = match_journal_entry_detail(response.headers["Location"])
         with self.app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             for offset in journal_entry.currencies[0].credit:
@@ -180,34 +193,37 @@
     def test_edit_receivable_offset(self) -> None:
         """Tests to edit the receivable offset.
 
         :return: None.
         """
         from accounting.models import Account
         journal_entry_data: JournalEntryData = self.data.j_r_of2
-        edit_uri: str = f"{PREFIX}/{journal_entry_data.id}/edit?next=%2F_next"
+        edit_uri: str = (f"{PREFIX}/{journal_entry_data.id}/edit?"
+                         f"next={self.encoded_next_uri}")
         update_uri: str = f"{PREFIX}/{journal_entry_data.id}/update"
         form: dict[str, str]
         response: httpx.Response
 
         journal_entry_data.days = self.data.j_r_or2.days
         journal_entry_data.currencies[0].debit[0].amount = Decimal("600")
         journal_entry_data.currencies[0].credit[0].amount = Decimal("600")
         journal_entry_data.currencies[0].debit[2].amount = Decimal("600")
         journal_entry_data.currencies[0].credit[2].amount = Decimal("600")
 
         # Non-existing original line item ID
-        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.update_form(self.csrf_token,
+                                              self.encoded_next_uri)
         form["currency-1-credit-1-original_line_item_id"] = "9999"
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # The same debit or credit
-        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.update_form(self.csrf_token,
+                                              self.encoded_next_uri)
         form["currency-1-credit-1-original_line_item_id"] \
             = str(self.data.l_p_or1c.id)
         form["currency-1-credit-1-account_code"] = self.data.l_p_or1c.account
         form["currency-1-debit-1-amount"] = "100"
         form["currency-1-credit-1-amount"] = "100"
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
@@ -216,163 +232,181 @@
         # The original line item does not need offset
         with self.app.app_context():
             account = Account.find_by_code(Accounts.RECEIVABLE)
             account.is_need_offset = False
             db.session.commit()
         response = self.client.post(
             update_uri,
-            data=journal_entry_data.update_form(self.csrf_token, NEXT_URI))
+            data=journal_entry_data.update_form(self.csrf_token,
+                                                self.encoded_next_uri))
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
         with self.app.app_context():
             account = Account.find_by_code(Accounts.RECEIVABLE)
             account.is_need_offset = True
             db.session.commit()
 
         # The original line item is also an offset
-        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.update_form(self.csrf_token,
+                                              self.encoded_next_uri)
         form["currency-1-credit-1-original_line_item_id"] \
             = str(self.data.l_p_of1d.id)
         form["currency-1-credit-1-account_code"] = self.data.l_p_of1d.account
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not the same currency
-        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.update_form(self.csrf_token,
+                                              self.encoded_next_uri)
         form["currency-1-code"] = "EUR"
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not the same account
-        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.update_form(self.csrf_token,
+                                              self.encoded_next_uri)
         form["currency-1-credit-1-account_code"] = Accounts.NOTES_RECEIVABLE
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not exceeding net balance - partially offset
-        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.update_form(self.csrf_token,
+                                              self.encoded_next_uri)
         form["currency-1-debit-1-amount"] \
             = str(journal_entry_data.currencies[0].debit[0].amount
                   + Decimal("0.01"))
         form["currency-1-credit-1-amount"] \
             = str(journal_entry_data.currencies[0].credit[0].amount
                   + Decimal("0.01"))
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not exceeding net balance - unmatched
-        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.update_form(self.csrf_token,
+                                              self.encoded_next_uri)
         form["currency-1-debit-3-amount"] \
             = str(journal_entry_data.currencies[0].debit[2].amount
                   + Decimal("0.01"))
         form["currency-1-credit-3-amount"] \
             = str(journal_entry_data.currencies[0].credit[2].amount
                   + Decimal("0.01"))
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not before the original line items
         old_days: int = journal_entry_data.days
         journal_entry_data.days = old_days + 1
-        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.update_form(self.csrf_token,
+                                              self.encoded_next_uri)
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
         journal_entry_data.days = old_days
 
         # Success
-        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.update_form(self.csrf_token,
+                                              self.encoded_next_uri)
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"],
-                         f"{PREFIX}/{journal_entry_data.id}?next=%2F_next")
+                         f"{PREFIX}/{journal_entry_data.id}?"
+                         f"next={self.encoded_next_uri}")
 
     def test_edit_receivable_original_line_item(self) -> None:
         """Tests to edit the receivable original line item.
 
         :return: None.
         """
         from accounting.models import JournalEntry
         journal_entry_data: JournalEntryData = self.data.j_r_or1
-        edit_uri: str = f"{PREFIX}/{journal_entry_data.id}/edit?next=%2F_next"
+        edit_uri: str = (f"{PREFIX}/{journal_entry_data.id}/edit?"
+                         f"next={self.encoded_next_uri}")
         update_uri: str = f"{PREFIX}/{journal_entry_data.id}/update"
         form: dict[str, str]
         response: httpx.Response
 
         journal_entry_data.days = self.data.j_r_of1.days
         journal_entry_data.currencies[0].debit[0].amount = Decimal("800")
         journal_entry_data.currencies[0].credit[0].amount = Decimal("800")
         journal_entry_data.currencies[0].debit[1].amount = Decimal("3.4")
         journal_entry_data.currencies[0].credit[1].amount = Decimal("3.4")
 
         # Not the same currency
-        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.update_form(self.csrf_token,
+                                              self.encoded_next_uri)
         form["currency-1-code"] = "EUR"
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not the same account
-        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.update_form(self.csrf_token,
+                                              self.encoded_next_uri)
         form["currency-1-debit-1-account_code"] = Accounts.NOTES_RECEIVABLE
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not less than offset total - partially offset
-        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.update_form(self.csrf_token,
+                                              self.encoded_next_uri)
         form["currency-1-debit-1-amount"] \
             = str(journal_entry_data.currencies[0].debit[0].amount
                   - Decimal("0.01"))
         form["currency-1-credit-1-amount"] \
             = str(journal_entry_data.currencies[0].credit[0].amount
                   - Decimal("0.01"))
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not less than offset total - fully offset
-        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.update_form(self.csrf_token,
+                                              self.encoded_next_uri)
         form["currency-1-debit-2-amount"] \
             = str(journal_entry_data.currencies[0].debit[1].amount
                   - Decimal("0.01"))
         form["currency-1-credit-2-amount"] \
             = str(journal_entry_data.currencies[0].credit[1].amount
                   - Decimal("0.01"))
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not after the offset items
         old_days: int = journal_entry_data.days
         journal_entry_data.days = old_days - 1
-        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.update_form(self.csrf_token,
+                                              self.encoded_next_uri)
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
         journal_entry_data.days = old_days
 
         # Not deleting matched original line items
-        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.update_form(self.csrf_token,
+                                              self.encoded_next_uri)
         del form["currency-1-debit-1-id"]
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Success
-        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.update_form(self.csrf_token,
+                                              self.encoded_next_uri)
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"],
-                         f"{PREFIX}/{journal_entry_data.id}?next=%2F_next")
+                         f"{PREFIX}/{journal_entry_data.id}?"
+                         f"next={self.encoded_next_uri}")
 
         # The original line item is always before the offset item, even when
         # they happen in the same day.
         with self.app.app_context():
             journal_entry_or: JournalEntry | None = db.session.get(
                 JournalEntry, journal_entry_data.id)
             self.assertIsNotNone(journal_entry_or)
@@ -384,15 +418,16 @@
 
     def test_add_payable_offset(self) -> None:
         """Tests to add the payable offset.
 
         :return: None.
         """
         from accounting.models import Account, JournalEntry
-        create_uri: str = f"{PREFIX}/create/disbursement?next=%2F_next"
+        create_uri: str = (f"{PREFIX}/create/disbursement?"
+                           f"next={self.encoded_next_uri}")
         store_uri: str = f"{PREFIX}/store/disbursement"
         form: dict[str, str]
         response: httpx.Response
 
         journal_entry_data: JournalEntryData = JournalEntryData(
             self.data.l_p_or3c.journal_entry.days, [JournalEntryCurrencyData(
                 "USD",
@@ -407,22 +442,24 @@
                  JournalEntryLineItemData(
                      Accounts.PAYABLE,
                      self.data.l_p_or3c.description, "120",
                      original_line_item=self.data.l_p_or3c)],
                 [])])
 
         # Non-existing original line item ID
-        form = journal_entry_data.new_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.new_form(self.csrf_token,
+                                           self.encoded_next_uri)
         form["currency-1-debit-1-original_line_item_id"] = "9999"
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # The same debit or credit
-        form = journal_entry_data.new_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.new_form(self.csrf_token,
+                                           self.encoded_next_uri)
         form["currency-1-debit-1-original_line_item_id"] \
             = str(self.data.l_r_or1d.id)
         form["currency-1-debit-1-account_code"] = self.data.l_r_or1d.account
         form["currency-1-debit-1-amount"] = "100"
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
@@ -430,74 +467,82 @@
         # The original line item does not need offset
         with self.app.app_context():
             account = Account.find_by_code(Accounts.PAYABLE)
             account.is_need_offset = False
             db.session.commit()
         response = self.client.post(
             store_uri,
-            data=journal_entry_data.new_form(self.csrf_token, NEXT_URI))
+            data=journal_entry_data.new_form(self.csrf_token,
+                                             self.encoded_next_uri))
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
         with self.app.app_context():
             account = Account.find_by_code(Accounts.PAYABLE)
             account.is_need_offset = True
             db.session.commit()
 
         # The original line item is also an offset
-        form = journal_entry_data.new_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.new_form(self.csrf_token,
+                                           self.encoded_next_uri)
         form["currency-1-debit-1-original_line_item_id"] \
             = str(self.data.l_r_of1c.id)
         form["currency-1-debit-1-account_code"] = self.data.l_r_of1c.account
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Not the same currency
-        form = journal_entry_data.new_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.new_form(self.csrf_token,
+                                           self.encoded_next_uri)
         form["currency-1-code"] = "EUR"
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Not the same account
-        form = journal_entry_data.new_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.new_form(self.csrf_token,
+                                           self.encoded_next_uri)
         form["currency-1-debit-1-account_code"] = Accounts.NOTES_PAYABLE
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Not exceeding net balance - partially offset
-        form = journal_entry_data.new_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.new_form(self.csrf_token,
+                                           self.encoded_next_uri)
         form["currency-1-debit-1-amount"] \
             = str(journal_entry_data.currencies[0].debit[0].amount
                   + Decimal("0.01"))
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Not exceeding net balance - unmatched
-        form = journal_entry_data.new_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.new_form(self.csrf_token,
+                                           self.encoded_next_uri)
         form["currency-1-debit-3-amount"] \
             = str(journal_entry_data.currencies[0].debit[2].amount
                   + Decimal("0.01"))
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Not before the original line items
         old_days: int = journal_entry_data.days
         journal_entry_data.days = old_days + 1
-        form = journal_entry_data.new_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.new_form(self.csrf_token,
+                                           self.encoded_next_uri)
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
         journal_entry_data.days = old_days
 
         # Success
-        form = journal_entry_data.new_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.new_form(self.csrf_token,
+                                           self.encoded_next_uri)
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         journal_entry_id: int \
             = match_journal_entry_detail(response.headers["Location"])
         with self.app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             for offset in journal_entry.currencies[0].debit:
@@ -506,34 +551,37 @@
     def test_edit_payable_offset(self) -> None:
         """Tests to edit the payable offset.
 
         :return: None.
         """
         from accounting.models import Account, JournalEntry
         journal_entry_data: JournalEntryData = self.data.j_p_of2
-        edit_uri: str = f"{PREFIX}/{journal_entry_data.id}/edit?next=%2F_next"
+        edit_uri: str = (f"{PREFIX}/{journal_entry_data.id}/edit?"
+                         f"next={self.encoded_next_uri}")
         update_uri: str = f"{PREFIX}/{journal_entry_data.id}/update"
         form: dict[str, str]
         response: httpx.Response
 
         journal_entry_data.days = self.data.j_p_or2.days
         journal_entry_data.currencies[0].debit[0].amount = Decimal("1100")
         journal_entry_data.currencies[0].credit[0].amount = Decimal("1100")
         journal_entry_data.currencies[0].debit[2].amount = Decimal("900")
         journal_entry_data.currencies[0].credit[2].amount = Decimal("900")
 
         # Non-existing original line item ID
-        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.update_form(self.csrf_token,
+                                              self.encoded_next_uri)
         form["currency-1-debit-1-original_line_item_id"] = "9999"
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # The same debit or credit
-        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.update_form(self.csrf_token,
+                                              self.encoded_next_uri)
         form["currency-1-debit-1-original_line_item_id"] \
             = str(self.data.l_r_or1d.id)
         form["currency-1-debit-1-account_code"] = self.data.l_r_or1d.account
         form["currency-1-debit-1-amount"] = "100"
         form["currency-1-credit-1-amount"] = "100"
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
@@ -542,80 +590,88 @@
         # The original line item does not need offset
         with self.app.app_context():
             account = Account.find_by_code(Accounts.PAYABLE)
             account.is_need_offset = False
             db.session.commit()
         response = self.client.post(
             update_uri,
-            data=journal_entry_data.update_form(self.csrf_token, NEXT_URI))
+            data=journal_entry_data.update_form(self.csrf_token,
+                                                self.encoded_next_uri))
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
         with self.app.app_context():
             account = Account.find_by_code(Accounts.PAYABLE)
             account.is_need_offset = True
             db.session.commit()
 
         # The original line item is also an offset
-        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.update_form(self.csrf_token,
+                                              self.encoded_next_uri)
         form["currency-1-debit-1-original_line_item_id"] \
             = str(self.data.l_r_of1c.id)
         form["currency-1-debit-1-account_code"] = self.data.l_r_of1c.account
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not the same currency
-        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.update_form(self.csrf_token,
+                                              self.encoded_next_uri)
         form["currency-1-code"] = "EUR"
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not the same account
-        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.update_form(self.csrf_token,
+                                              self.encoded_next_uri)
         form["currency-1-debit-1-account_code"] = Accounts.NOTES_PAYABLE
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not exceeding net balance - partially offset
-        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.update_form(self.csrf_token,
+                                              self.encoded_next_uri)
         form["currency-1-debit-1-amount"] \
             = str(journal_entry_data.currencies[0].debit[0].amount
                   + Decimal("0.01"))
         form["currency-1-credit-1-amount"] \
             = str(journal_entry_data.currencies[0].credit[0].amount
                   + Decimal("0.01"))
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not exceeding net balance - unmatched
-        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.update_form(self.csrf_token,
+                                              self.encoded_next_uri)
         form["currency-1-debit-3-amount"] \
             = str(journal_entry_data.currencies[0].debit[2].amount
                   + Decimal("0.01"))
         form["currency-1-credit-3-amount"] \
             = str(journal_entry_data.currencies[0].credit[2].amount
                   + Decimal("0.01"))
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not before the original line items
         old_days: int = journal_entry_data.days
         journal_entry_data.days = old_days + 1
-        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.update_form(self.csrf_token,
+                                              self.encoded_next_uri)
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
         journal_entry_data.days = old_days
 
         # Success
-        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.update_form(self.csrf_token,
+                                              self.encoded_next_uri)
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         journal_entry_id: int \
             = match_journal_entry_detail(response.headers["Location"])
         with self.app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             for offset in journal_entry.currencies[0].debit:
@@ -624,85 +680,94 @@
     def test_edit_payable_original_line_item(self) -> None:
         """Tests to edit the payable original line item.
 
         :return: None.
         """
         from accounting.models import JournalEntry
         journal_entry_data: JournalEntryData = self.data.j_p_or1
-        edit_uri: str = f"{PREFIX}/{journal_entry_data.id}/edit?next=%2F_next"
+        edit_uri: str = (f"{PREFIX}/{journal_entry_data.id}/edit?"
+                         f"next={self.encoded_next_uri}")
         update_uri: str = f"{PREFIX}/{journal_entry_data.id}/update"
         form: dict[str, str]
         response: httpx.Response
 
         journal_entry_data.days = self.data.j_p_of1.days
         journal_entry_data.currencies[0].debit[0].amount = Decimal("1200")
         journal_entry_data.currencies[0].credit[0].amount = Decimal("1200")
         journal_entry_data.currencies[0].debit[1].amount = Decimal("0.9")
         journal_entry_data.currencies[0].credit[1].amount = Decimal("0.9")
 
         # Not the same currency
-        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.update_form(self.csrf_token,
+                                              self.encoded_next_uri)
         form["currency-1-code"] = "EUR"
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not the same account
-        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.update_form(self.csrf_token,
+                                              self.encoded_next_uri)
         form["currency-1-credit-1-account_code"] = Accounts.NOTES_PAYABLE
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not less than offset total - partially offset
-        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.update_form(self.csrf_token,
+                                              self.encoded_next_uri)
         form["currency-1-debit-1-amount"] \
             = str(journal_entry_data.currencies[0].debit[0].amount
                   - Decimal("0.01"))
         form["currency-1-credit-1-amount"] \
             = str(journal_entry_data.currencies[0].credit[0].amount
                   - Decimal("0.01"))
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not less than offset total - fully offset
-        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.update_form(self.csrf_token,
+                                              self.encoded_next_uri)
         form["currency-1-debit-2-amount"] \
             = str(journal_entry_data.currencies[0].debit[1].amount
                   - Decimal("0.01"))
         form["currency-1-credit-2-amount"] \
             = str(journal_entry_data.currencies[0].credit[1].amount
                   - Decimal("0.01"))
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not after the offset items
         old_days: int = journal_entry_data.days
         journal_entry_data.days = old_days - 1
-        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.update_form(self.csrf_token,
+                                              self.encoded_next_uri)
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
         journal_entry_data.days = old_days
 
         # Not deleting matched original line items
-        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.update_form(self.csrf_token,
+                                              self.encoded_next_uri)
         del form["currency-1-credit-1-id"]
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Success
-        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
+        form = journal_entry_data.update_form(self.csrf_token,
+                                              self.encoded_next_uri)
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"],
-                         f"{PREFIX}/{journal_entry_data.id}?next=%2F_next")
+                         f"{PREFIX}/{journal_entry_data.id}?"
+                         f"next={self.encoded_next_uri}")
 
         # The original line item is always before the offset item, even when
         # they happen in the same day
         with self.app.app_context():
             journal_entry_or: JournalEntry | None = db.session.get(
                 JournalEntry, journal_entry_data.id)
             self.assertIsNotNone(journal_entry_or)
```

### Comparing `mia-accounting-1.5.4/tests/test_option.py` & `mia-accounting-1.5.5/tests/test_option.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,25 +19,20 @@
 """
 import datetime as dt
 import unittest
 
 import httpx
 from flask import Flask
 
+from accounting.utils.next_uri import encode_next
 from test_site import db
 from testlib import NEXT_URI, Accounts, create_test_app, get_client
 
 PREFIX: str = "/accounting/options"
 """The URL prefix for the option management."""
-DETAIL_URI: str = f"{PREFIX}?next=%2F_next"
-"""THE URI for the option detail."""
-EDIT_URI: str = f"{PREFIX}/edit?next=%2F_next"
-"""THE URI for the form to edit the options."""
-UPDATE_URI: str = f"{PREFIX}/update"
-"""THE URI to update the options."""
 
 
 class OptionTestCase(unittest.TestCase):
     """The option test case."""
 
     def setUp(self) -> None:
         """Sets up the test.
@@ -46,203 +41,219 @@
         :return: None.
         """
         self.app: Flask = create_test_app()
 
         with self.app.app_context():
             from accounting.models import Option
             Option.query.delete()
+            self.encoded_next_uri: str = encode_next(NEXT_URI)
 
         self.client, self.csrf_token = get_client(self.app, "admin")
 
     def test_nobody(self) -> None:
         """Test the permission as nobody.
 
         :return: None.
         """
         client, csrf_token = get_client(self.app, "nobody")
+        detail_uri: str = f"{PREFIX}?next={self.encoded_next_uri}"
+        edit_uri: str = f"{PREFIX}/edit?next={self.encoded_next_uri}"
+        update_uri: str = f"{PREFIX}/update"
         response: httpx.Response
 
-        response = client.get(DETAIL_URI)
+        response = client.get(detail_uri)
         self.assertEqual(response.status_code, 403)
 
-        response = client.get(EDIT_URI)
+        response = client.get(edit_uri)
         self.assertEqual(response.status_code, 403)
 
-        response = client.post(UPDATE_URI, data=self.__get_form(csrf_token))
+        response = client.post(update_uri, data=self.__get_form(csrf_token))
         self.assertEqual(response.status_code, 403)
 
     def test_viewer(self) -> None:
         """Test the permission as viewer.
 
         :return: None.
         """
         client, csrf_token = get_client(self.app, "viewer")
+        detail_uri: str = f"{PREFIX}?next={self.encoded_next_uri}"
+        edit_uri: str = f"{PREFIX}/edit?next={self.encoded_next_uri}"
+        update_uri: str = f"{PREFIX}/update"
         response: httpx.Response
 
-        response = client.get(DETAIL_URI)
+        response = client.get(detail_uri)
         self.assertEqual(response.status_code, 403)
 
-        response = client.get(EDIT_URI)
+        response = client.get(edit_uri)
         self.assertEqual(response.status_code, 403)
 
-        response = client.post(UPDATE_URI, data=self.__get_form(csrf_token))
+        response = client.post(update_uri, data=self.__get_form(csrf_token))
         self.assertEqual(response.status_code, 403)
 
     def test_editor(self) -> None:
         """Test the permission as editor.
 
         :return: None.
         """
         client, csrf_token = get_client(self.app, "editor")
+        detail_uri: str = f"{PREFIX}?next={self.encoded_next_uri}"
+        edit_uri: str = f"{PREFIX}/edit?next={self.encoded_next_uri}"
+        update_uri: str = f"{PREFIX}/update"
         response: httpx.Response
 
-        response = client.get(DETAIL_URI)
+        response = client.get(detail_uri)
         self.assertEqual(response.status_code, 403)
 
-        response = client.get(EDIT_URI)
+        response = client.get(edit_uri)
         self.assertEqual(response.status_code, 403)
 
-        response = client.post(UPDATE_URI, data=self.__get_form(csrf_token))
+        response = client.post(update_uri, data=self.__get_form(csrf_token))
         self.assertEqual(response.status_code, 403)
 
     def test_admin(self) -> None:
         """Test the permission as administrator.
 
         :return: None.
         """
+        detail_uri: str = f"{PREFIX}?next={self.encoded_next_uri}"
+        edit_uri: str = f"{PREFIX}/edit?next={self.encoded_next_uri}"
+        update_uri: str = f"{PREFIX}/update"
         response: httpx.Response
 
-        response = self.client.get(DETAIL_URI)
+        response = self.client.get(detail_uri)
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.get(EDIT_URI)
+        response = self.client.get(edit_uri)
         self.assertEqual(response.status_code, 200)
 
-        response = self.client.post(UPDATE_URI, data=self.__get_form())
+        response = self.client.post(update_uri, data=self.__get_form())
         self.assertEqual(response.status_code, 302)
-        self.assertEqual(response.headers["Location"], DETAIL_URI)
+        self.assertEqual(response.headers["Location"], detail_uri)
 
     def test_set(self) -> None:
         """Test to set the options.
 
         :return: None.
         """
         from accounting.utils.options import options
+        detail_uri: str = f"{PREFIX}?next={self.encoded_next_uri}"
+        edit_uri: str = f"{PREFIX}/edit?next={self.encoded_next_uri}"
+        update_uri: str = f"{PREFIX}/update"
         form: dict[str, str]
         response: httpx.Response
 
         # Empty currency code
         form = self.__get_form()
         form["default_currency_code"] = " "
-        response = self.client.post(UPDATE_URI, data=form)
+        response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
-        self.assertEqual(response.headers["Location"], EDIT_URI)
+        self.assertEqual(response.headers["Location"], edit_uri)
 
         # Non-existing currency code
         form = self.__get_form()
         form["default_currency_code"] = "ZZZ"
-        response = self.client.post(UPDATE_URI, data=form)
+        response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
-        self.assertEqual(response.headers["Location"], EDIT_URI)
+        self.assertEqual(response.headers["Location"], edit_uri)
 
         # Empty current account
         form = self.__get_form()
         form["default_ie_account_code"] = " "
-        response = self.client.post(UPDATE_URI, data=form)
+        response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
-        self.assertEqual(response.headers["Location"], EDIT_URI)
+        self.assertEqual(response.headers["Location"], edit_uri)
 
         # Non-existing current account
         form = self.__get_form()
         form["default_ie_account_code"] = "9999-999"
-        response = self.client.post(UPDATE_URI, data=form)
+        response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
-        self.assertEqual(response.headers["Location"], EDIT_URI)
+        self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not a current account
         form = self.__get_form()
         form["default_ie_account_code"] = Accounts.MEAL
-        response = self.client.post(UPDATE_URI, data=form)
+        response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
-        self.assertEqual(response.headers["Location"], EDIT_URI)
+        self.assertEqual(response.headers["Location"], edit_uri)
 
         # Recurring item name empty
         form = self.__get_form()
         key = [x for x in form if x.endswith("-name")][0]
         form[key] = " "
-        response = self.client.post(UPDATE_URI, data=form)
+        response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
-        self.assertEqual(response.headers["Location"], EDIT_URI)
+        self.assertEqual(response.headers["Location"], edit_uri)
 
         # Recurring item account empty
         form = self.__get_form()
         key = [x for x in form if x.endswith("-account_code")][0]
         form[key] = " "
-        response = self.client.post(UPDATE_URI, data=form)
+        response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
-        self.assertEqual(response.headers["Location"], EDIT_URI)
+        self.assertEqual(response.headers["Location"], edit_uri)
 
         # Recurring item non-expense account
         form = self.__get_form()
         key = [x for x in form
                if x.startswith("recurring-expense-")
                and x.endswith("-account_code")][0]
         form[key] = Accounts.SERVICE
-        response = self.client.post(UPDATE_URI, data=form)
+        response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
-        self.assertEqual(response.headers["Location"], EDIT_URI)
+        self.assertEqual(response.headers["Location"], edit_uri)
 
         # Recurring item non-income account
         form = self.__get_form()
         key = [x for x in form
                if x.startswith("recurring-income-")
                and x.endswith("-account_code")][0]
         form[key] = Accounts.UTILITIES
-        response = self.client.post(UPDATE_URI, data=form)
+        response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
-        self.assertEqual(response.headers["Location"], EDIT_URI)
+        self.assertEqual(response.headers["Location"], edit_uri)
 
         # Recurring item payable expense
         form = self.__get_form()
         key = [x for x in form
                if x.startswith("recurring-expense-")
                and x.endswith("-account_code")][0]
         form[key] = Accounts.PAYABLE
-        response = self.client.post(UPDATE_URI, data=form)
+        response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
-        self.assertEqual(response.headers["Location"], EDIT_URI)
+        self.assertEqual(response.headers["Location"], edit_uri)
 
         # Recurring item receivable income
         form = self.__get_form()
         key = [x for x in form
                if x.startswith("recurring-income-")
                and x.endswith("-account_code")][0]
         form[key] = Accounts.RECEIVABLE
-        response = self.client.post(UPDATE_URI, data=form)
+        response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
-        self.assertEqual(response.headers["Location"], EDIT_URI)
+        self.assertEqual(response.headers["Location"], edit_uri)
 
         # Recurring item description template empty
         form = self.__get_form()
         key = [x for x in form if x.endswith("-description_template")][0]
         form[key] = " "
-        response = self.client.post(UPDATE_URI, data=form)
+        response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
-        self.assertEqual(response.headers["Location"], EDIT_URI)
+        self.assertEqual(response.headers["Location"], edit_uri)
 
         # Success, with malformed order
         with self.app.app_context():
             self.assertEqual(options.default_currency_code, "USD")
             self.assertEqual(options.default_ie_account_code, "1111-001")
             self.assertEqual(len(options.recurring.expenses), 0)
             self.assertEqual(len(options.recurring.incomes), 0)
 
-        response = self.client.post(UPDATE_URI, data=self.__get_form())
+        response = self.client.post(update_uri, data=self.__get_form())
         self.assertEqual(response.status_code, 302)
-        self.assertEqual(response.headers["Location"], DETAIL_URI)
+        self.assertEqual(response.headers["Location"], detail_uri)
 
         with self.app.app_context():
             self.assertEqual(options.default_currency_code, "EUR")
             self.assertEqual(options.default_ie_account_code, "0000-000")
             self.assertEqual(len(options.recurring.expenses), 4)
             self.assertEqual(options.recurring.expenses[0].account_code,
                              Accounts.INSURANCE)
@@ -257,104 +268,108 @@
                              Accounts.SERVICE)
             self.assertEqual(options.recurring.incomes[1].account_code,
                              Accounts.DONATION)
 
         # Success, with no recurring data
         form = self.__get_form()
         form = {x: form[x] for x in form if not x.startswith("recurring-")}
-        response = self.client.post(UPDATE_URI, data=form)
+        response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
-        self.assertEqual(response.headers["Location"], DETAIL_URI)
+        self.assertEqual(response.headers["Location"], detail_uri)
 
         with self.app.app_context():
             self.assertEqual(len(options.recurring.expenses), 0)
             self.assertEqual(len(options.recurring.incomes), 0)
 
     def test_update_not_modified(self) -> None:
         """Tests that the data is not modified.
 
         :return: None.
         """
         from accounting.models import Option
+        detail_uri: str = f"{PREFIX}?next={self.encoded_next_uri}"
+        update_uri: str = f"{PREFIX}/update"
         form: dict[str, str]
         option: Option | None
         resource: httpx.Response
 
-        response = self.client.post(UPDATE_URI, data=self.__get_form())
+        response = self.client.post(update_uri, data=self.__get_form())
         self.assertEqual(response.status_code, 302)
-        self.assertEqual(response.headers["Location"], DETAIL_URI)
+        self.assertEqual(response.headers["Location"], detail_uri)
 
         with self.app.app_context():
             option = db.session.get(Option, "recurring")
             self.assertIsNotNone(option)
             timestamp: dt.datetime \
                 = option.created_at - dt.timedelta(seconds=5)
             option.created_at = timestamp
             option.updated_at = timestamp
             db.session.commit()
 
         # The recurring setting was not modified
         form = self.__get_form()
         form["default_currency_code"] = "JPY"
-        response = self.client.post(UPDATE_URI, data=form)
+        response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
-        self.assertEqual(response.headers["Location"], DETAIL_URI)
+        self.assertEqual(response.headers["Location"], detail_uri)
 
         with self.app.app_context():
             option = db.session.get(Option, "recurring")
             self.assertIsNotNone(option)
             self.assertEqual(option.created_at, timestamp)
             self.assertEqual(option.updated_at, timestamp)
 
         # The recurring setting was modified
         form = self.__get_form()
         key: str = [x for x in form
                     if x.startswith("recurring-expense-")
                     and x.endswith("-account_code")][0]
         form[key] = Accounts.MEAL
-        response = self.client.post(UPDATE_URI, data=form)
+        response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
-        self.assertEqual(response.headers["Location"], DETAIL_URI)
+        self.assertEqual(response.headers["Location"], detail_uri)
 
         with self.app.app_context():
             option = db.session.get(Option, "recurring")
             self.assertIsNotNone(option)
             self.assertLess(option.created_at, option.updated_at)
 
     def test_created_updated_by(self) -> None:
         """Tests the created-by and updated-by record.
 
         :return: None.
         """
         from accounting.models import Option
         from accounting.utils.user import get_user_pk
         admin_username, editor_username = "admin", "editor"
+        detail_uri: str = f"{PREFIX}?next={self.encoded_next_uri}"
+        update_uri: str = f"{PREFIX}/update"
         option: Option | None
         response: httpx.Response
 
-        response = self.client.post(UPDATE_URI, data=self.__get_form())
+        response = self.client.post(update_uri, data=self.__get_form())
         self.assertEqual(response.status_code, 302)
-        self.assertEqual(response.headers["Location"], DETAIL_URI)
+        self.assertEqual(response.headers["Location"], detail_uri)
 
         with self.app.app_context():
             editor_pk: int = get_user_pk(editor_username)
             option = db.session.get(Option, "recurring")
             self.assertIsNotNone(option)
             option.created_by_id = editor_pk
             option.updated_by_id = editor_pk
             db.session.commit()
 
         form: dict[str, str] = self.__get_form()
         key: str = [x for x in form
                     if x.startswith("recurring-expense-")
                     and x.endswith("-account_code")][0]
         form[key] = Accounts.MEAL
-        response = self.client.post(UPDATE_URI, data=form)
+        response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
-        self.assertEqual(response.headers["Location"], DETAIL_URI)
+        self.assertEqual(response.headers["Location"], detail_uri)
 
         with self.app.app_context():
             option = db.session.get(Option, "recurring")
             self.assertIsNotNone(option)
             self.assertEqual(option.created_by.username, editor_username)
             self.assertEqual(option.updated_by.username, admin_username)
 
@@ -363,15 +378,15 @@
 
         :param csrf_token: The CSRF token.
         :return: The option form.
         """
         if csrf_token is None:
             csrf_token = self.csrf_token
         return {"csrf_token": csrf_token,
-                "next": NEXT_URI,
+                "next": self.encoded_next_uri,
                 "default_currency_code": "EUR",
                 "default_ie_account_code": "0000-000",
                 "recurring-expense-1-name": "Water bill",
                 "recurring-expense-1-account_code": Accounts.UTILITIES,
                 "recurring-expense-1-description_template":
                     "Water bill for {last_bimonthly_name}",
                 "recurring-expense-3-no": "16",
```

### Comparing `mia-accounting-1.5.4/tests/test_report.py` & `mia-accounting-1.5.5/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/tests/test_site/__init__.py` & `mia-accounting-1.5.5/tests/test_site/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,21 +19,23 @@
 """
 import os
 from secrets import token_urlsafe
 from typing import Type
 
 from click.testing import Result
 from flask import Flask, Blueprint, render_template, redirect, Response, \
-    url_for
+    url_for, request
 from flask.testing import FlaskCliRunner
 from flask_babel_js import BabelJS
 from flask_sqlalchemy import SQLAlchemy
 from flask_wtf import CSRFProtect
 from sqlalchemy import Column
 
+from accounting.utils.next_uri import encode_next
+
 bp: Blueprint = Blueprint("home", __name__)
 """The global blueprint."""
 babel_js: BabelJS = BabelJS()
 """The Babel JavaScript instance."""
 csrf: CSRFProtect = CSRFProtect()
 """The CSRF protector."""
 db: SQLAlchemy = SQLAlchemy()
@@ -62,14 +64,15 @@
         app.config["TESTING"] = True
 
     babel_js.init_app(app)
     csrf.init_app(app)
     db.init_app(app)
 
     app.register_blueprint(bp, url_prefix="/")
+    app.add_template_global(__as_next, "accounting_as_next")
 
     from . import locale
     locale.init_app(app)
 
     from . import auth
     auth.init_app(app)
 
@@ -142,7 +145,16 @@
 @bp.get("/", endpoint="home")
 def get_home() -> str:
     """Returns the home page.
 
     :return: The home page.
     """
     return render_template("home.html")
+
+
+def __as_next() -> str:
+    """Encodes the current request URI as value for the next URI.
+
+    :return: The current request URI as value for the next URI.
+    """
+    return encode_next(
+        request.full_path if request.query_string else request.path)
```

### Comparing `mia-accounting-1.5.4/tests/test_site/auth.py` & `mia-accounting-1.5.5/tests/test_site/auth.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/tests/test_site/lib.py` & `mia-accounting-1.5.5/tests/test_site/lib.py`

 * *Files 4% similar despite different names*

```diff
@@ -136,44 +136,46 @@
         self.note: str | None = None
         for currency in self.currencies:
             for line_item in currency.debit:
                 line_item.journal_entry = self
             for line_item in currency.credit:
                 line_item.journal_entry = self
 
-    def new_form(self, csrf_token: str, next_uri: str) -> dict[str, str]:
+    def new_form(self, csrf_token: str, encoded_next_uri: str) \
+            -> dict[str, str]:
         """Returns the journal entry as a creation form.
 
         :param csrf_token: The CSRF token.
-        :param next_uri: The next URI.
+        :param encoded_next_uri: The encoded next URI.
         :return: The journal entry as a creation form.
         """
-        return self.__form(csrf_token, next_uri, is_update=False)
+        return self.__form(csrf_token, encoded_next_uri, is_update=False)
 
-    def update_form(self, csrf_token: str, next_uri: str) -> dict[str, str]:
+    def update_form(self, csrf_token: str, encoded_next_uri: str) \
+            -> dict[str, str]:
         """Returns the journal entry as an update form.
 
         :param csrf_token: The CSRF token.
-        :param next_uri: The next URI.
+        :param encoded_next_uri: The encoded next URI.
         :return: The journal entry as an update form.
         """
-        return self.__form(csrf_token, next_uri, is_update=True)
+        return self.__form(csrf_token, encoded_next_uri, is_update=True)
 
-    def __form(self, csrf_token: str, next_uri: str, is_update: bool = False) \
-            -> dict[str, str]:
+    def __form(self, csrf_token: str, encoded_next_uri: str,
+               is_update: bool = False) -> dict[str, str]:
         """Returns the journal entry as a form.
 
         :param csrf_token: The CSRF token.
-        :param next_uri: The next URI.
+        :param encoded_next_uri: The encoded next URI.
         :param is_update: True for an update operation, or False otherwise
         :return: The journal entry as a form.
         """
         date: dt.date = dt.date.today() - dt.timedelta(days=self.days)
         form: dict[str, str] = {"csrf_token": csrf_token,
-                                "next": next_uri,
+                                "next": encoded_next_uri,
                                 "date": date.isoformat()}
         for i in range(len(self.currencies)):
             form.update(self.currencies[i].form(i + 1, is_update))
         if self.note is not None:
             form["note"] = self.note
         return form
```

### Comparing `mia-accounting-1.5.4/tests/test_site/locale.py` & `mia-accounting-1.5.5/tests/test_site/locale.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/tests/test_site/reset.py` & `mia-accounting-1.5.5/tests/test_site/reset.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/tests/test_site/static/favicon.svg` & `mia-accounting-1.5.5/tests/test_site/static/favicon.svg`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/tests/test_site/templates/base.html` & `mia-accounting-1.5.5/tests/test_site/templates/base.html`

 * *Files 4% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 #}
 <!doctype html>
 <html xmlns="http://www.w3.org/1999/xhtml" lang="{{ _("en") }}">
 <head>
   <meta charset="UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <meta name="author" content="{{ "imacat" }}" />
-  <link rel="stylesheet" type="text/css" href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/css/bootstrap.min.css" crossorigin="anonymous">
-  <link rel="stylesheet" type="text/css" href="https://cdn.jsdelivr.net/npm/@fortawesome/fontawesome-free@6.4.0/css/all.min.css" crossorigin="anonymous">
-  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@eonasdan/tempus-dominus@6.7.7/dist/css/tempus-dominus.min.css" crossorigin="anonymous">
+  <link rel="stylesheet" type="text/css" href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/css/bootstrap.min.css" integrity="sha384-rbsA2VBKQhggwzxH7pPCaAqO46MgnOM80zW1RWuH61DGLwZJEdK2Kadq2F9CUG65" crossorigin="anonymous">
+  <link rel="stylesheet" type="text/css" href="https://cdn.jsdelivr.net/npm/@fortawesome/fontawesome-free@6.4.0/css/all.min.css" integrity="sha384-iw3OoTErCYJJB9mCa8LNS2hbsQ7M3C0EpIsO/H5+EGAkPGc6rk+V8i04oW/K5xq0" crossorigin="anonymous">
+  <link rel="stylesheet" type="text/css" href="https://cdn.jsdelivr.net/npm/@eonasdan/tempus-dominus@6.7.7/dist/css/tempus-dominus.min.css" integrity="sha384-l66rSL7gUubrdJxFRbXUo/tO7eNPAcCiZXFs/Xl147146xNqQ1qt4oPW6jlVezsS" crossorigin="anonymous">
   {% block styles %}{% endblock %}
   <script src="{{ url_for("babel_catalog") }}"></script>
   <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-kenU1KFdBIe4zVF0s0G1M5b4hcpxyD9F7jL+jjXkk+Q2h455rYXK/7HAuoJl+0I4" crossorigin="anonymous"></script>
   <script src="https://cdn.jsdelivr.net/npm/decimal.js-light@2.5.1/decimal.min.js" integrity="sha384-QdsxGEq4Y0erX8WUIsZJDtfoSSyBF6dmNCnzRNYCa2AOM/xzNsyhHu0RbdFBAm+l" crossorigin="anonymous"></script>
   <script src="https://cdn.jsdelivr.net/npm/@eonasdan/tempus-dominus@6.7.7/dist/js/tempus-dominus.min.js" integrity="sha384-MxHp+/TqTjbku1jSTIe1e/4l6CZTLhACLDbWyxYaFRgD3AM4oh99AY8bxsGhIoRc" crossorigin="anonymous"></script>
   {% block scripts %}{% endblock %}
   <link rel="shortcut icon" href="{{ url_for("static", filename="favicon.svg") }}">
@@ -92,15 +92,15 @@
         {% endif %}
         <li class="nav-item dropdown">
           <span class="nav-link dropdown-toggle" data-bs-toggle="dropdown">
             <i class="fa-solid fa-language"></i>
           </span>
           <form action="{{ url_for("locale.set-locale") }}" method="post">
             <input type="hidden" name="csrf_token" value="{{ csrf_token() }}">
-            <input type="hidden" name="next" value="{{ request.full_path if request.query_string else request.path }}">
+            <input type="hidden" name="next" value="{{ accounting_as_next() }}">
             <ul class="dropdown-menu dropdown-menu-end">
               {% for locale_code, locale_name in get_all_linguas().items() %}
                 <li>
                   <button class="dropdown-item {% if locale_code == get_locale() %} active {% endif %}" type="submit" name="locale" value="{{ locale_code }}">
                     {{ locale_name }}
                   </button>
                 </li>
@@ -117,18 +117,18 @@
 
 <h1>{% block header %}{% endblock %}</h1>
 
 {% with messages = get_flashed_messages(with_categories=true) %}
   {% if messages %}
     {% for category, message in messages %}
       {% if category == "success" %}
-          <div class="alert alert-success alert-dismissible fade show" role="alert">
-            {{ message }}
-            <button type="button" class="btn-close" data-bs-dismiss="alert" aria-label="Close"></button>
-          </div>
+        <div class="alert alert-success alert-dismissible fade show" role="alert">
+          {{ message }}
+          <button type="button" class="btn-close" data-bs-dismiss="alert" aria-label="Close"></button>
+        </div>
       {% elif category == "error" %}
         <div class="alert alert-danger alert-dismissible fade show" role="alert">
           <strong>{{ _("Error:") }}</strong> {{ message }}
           <button type="button" class="btn-close" data-bs-dismiss="alert" aria-label="Close"></button>
         </div>
       {% endif %}
     {% endfor %}
```

### Comparing `mia-accounting-1.5.4/tests/test_site/templates/home.html` & `mia-accounting-1.5.5/tests/test_site/templates/home.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/tests/test_site/templates/login.html` & `mia-accounting-1.5.5/tests/test_site/templates/login.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/tests/test_site/templates/reset.html` & `mia-accounting-1.5.5/tests/test_site/templates/reset.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/tests/test_site/translations/messages.pot` & `mia-accounting-1.5.5/tests/test_site/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo` & `mia-accounting-1.5.5/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po` & `mia-accounting-1.5.5/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo` & `mia-accounting-1.5.5/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po` & `mia-accounting-1.5.5/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.5.4/tests/test_unmatched_offset.py` & `mia-accounting-1.5.5/tests/test_unmatched_offset.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 """
 import unittest
 
 import httpx
 from flask import Flask
 
+from accounting.utils.next_uri import encode_next
 from test_site import db
 from test_site.lib import JournalEntryCurrencyData, JournalEntryData, \
     BaseTestData
 from testlib import NEXT_URI, create_test_app, get_client, Accounts
 
 PREFIX: str = "/accounting/match-offsets/USD"
 """The URL prefix for the unmatched offset management."""
@@ -42,69 +43,70 @@
         """
         self.app: Flask = create_test_app()
 
         with self.app.app_context():
             from accounting.models import JournalEntry, JournalEntryLineItem
             JournalEntry.query.delete()
             JournalEntryLineItem.query.delete()
+            self.encoded_next_uri: str = encode_next(NEXT_URI)
 
         self.client, self.csrf_token = get_client(self.app, "editor")
 
     def test_nobody(self) -> None:
         """Test the permission as nobody.
 
         :return: None.
         """
         client, csrf_token = get_client(self.app, "nobody")
         DifferentTestData(self.app, "nobody").populate()
         response: httpx.Response
 
         response = client.post(f"{PREFIX}/{Accounts.PAYABLE}",
                                data={"csrf_token": csrf_token,
-                                     "next": NEXT_URI})
+                                     "next": self.encoded_next_uri})
         self.assertEqual(response.status_code, 403)
 
     def test_viewer(self) -> None:
         """Test the permission as viewer.
 
         :return: None.
         """
         client, csrf_token = get_client(self.app, "viewer")
         DifferentTestData(self.app, "viewer").populate()
         response: httpx.Response
 
         response = client.post(f"{PREFIX}/{Accounts.PAYABLE}",
                                data={"csrf_token": csrf_token,
-                                     "next": NEXT_URI})
+                                     "next": self.encoded_next_uri})
         self.assertEqual(response.status_code, 403)
 
     def test_editor(self) -> None:
         """Test the permission as editor.
 
         :return: None.
         """
         DifferentTestData(self.app, "editor").populate()
         response: httpx.Response
 
         response = self.client.post(f"{PREFIX}/{Accounts.PAYABLE}",
                                     data={"csrf_token": self.csrf_token,
-                                          "next": NEXT_URI})
+                                          "next": self.encoded_next_uri})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], NEXT_URI)
 
     def test_empty_db(self) -> None:
         """Test the empty database.
 
         :return: None.
         """
         response: httpx.Response
 
         response = self.client.post(f"{PREFIX}/{Accounts.PAYABLE}",
                                     data={"csrf_token": self.csrf_token,
-                                          "next": NEXT_URI})
+                                          "next": self.encoded_next_uri})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], NEXT_URI)
 
     def test_different(self) -> None:
         """Tests to match against different descriptions and amounts.
 
         :return: None.
@@ -146,15 +148,15 @@
                 line_item = db.session.get(JournalEntryLineItem, line_item_id)
                 self.assertIsNotNone(line_item)
                 self.assertIsNone(line_item.original_line_item_id)
 
         match_uri = f"{PREFIX}/{Accounts.RECEIVABLE}"
         response = self.client.post(match_uri,
                                     data={"csrf_token": self.csrf_token,
-                                          "next": NEXT_URI})
+                                          "next": self.encoded_next_uri})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], NEXT_URI)
 
         with self.app.app_context():
             account = Account.find_by_code(Accounts.RECEIVABLE)
             assert account is not None
             matcher = OffsetMatcher(currency, account)
@@ -196,15 +198,15 @@
                 line_item = db.session.get(JournalEntryLineItem, line_item_id)
                 self.assertIsNotNone(line_item)
                 self.assertIsNone(line_item.original_line_item_id)
 
         match_uri = f"{PREFIX}/{Accounts.PAYABLE}"
         response = self.client.post(match_uri,
                                     data={"csrf_token": self.csrf_token,
-                                          "next": NEXT_URI})
+                                          "next": self.encoded_next_uri})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], NEXT_URI)
 
         with self.app.app_context():
             account = Account.find_by_code(Accounts.PAYABLE)
             assert account is not None
             matcher = OffsetMatcher(currency, account)
@@ -274,15 +276,15 @@
             self.assertIsNotNone(line_item)
             self.assertIsNotNone(line_item.original_line_item_id)
             self.assertEqual(line_item.original_line_item_id, data.l_r_or2d.id)
 
         match_uri = f"{PREFIX}/{Accounts.RECEIVABLE}"
         response = self.client.post(match_uri,
                                     data={"csrf_token": self.csrf_token,
-                                          "next": NEXT_URI})
+                                          "next": self.encoded_next_uri})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], NEXT_URI)
 
         with self.app.app_context():
             account = Account.find_by_code(Accounts.RECEIVABLE)
             assert account is not None
             matcher = OffsetMatcher(currency, account)
@@ -340,15 +342,15 @@
             self.assertIsNotNone(line_item)
             self.assertIsNotNone(line_item.original_line_item_id)
             self.assertEqual(line_item.original_line_item_id, data.l_p_or2c.id)
 
         match_uri = f"{PREFIX}/{Accounts.PAYABLE}"
         response = self.client.post(match_uri,
                                     data={"csrf_token": self.csrf_token,
-                                          "next": NEXT_URI})
+                                          "next": self.encoded_next_uri})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], NEXT_URI)
 
         with self.app.app_context():
             account = Account.find_by_code(Accounts.PAYABLE)
             assert account is not None
             matcher = OffsetMatcher(currency, account)
```

### Comparing `mia-accounting-1.5.4/tests/test_utils.py` & `mia-accounting-1.5.5/tests/test_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,76 +18,76 @@
 
 """
 import unittest
 from urllib.parse import quote_plus
 
 import httpx
 from flask import Flask, request
+from itsdangerous import URLSafeSerializer
 
 from accounting.utils.next_uri import append_next, inherit_next, or_next
 from accounting.utils.pagination import Pagination, DEFAULT_PAGE_SIZE
 from accounting.utils.query import parse_query_keywords
-from testlib import TEST_SERVER, create_test_app, get_csrf_token
+from testlib import TEST_SERVER, create_test_app, get_csrf_token, NEXT_URI
 
 
 class NextUriTestCase(unittest.TestCase):
     """The test case for the next URI utilities."""
     TARGET: str = "/target"
 
     def setUp(self) -> None:
         """Sets up the test.
         This is run once per test.
 
         :return: None.
         """
         self.app: Flask = create_test_app()
+        self.serializer: URLSafeSerializer \
+            = URLSafeSerializer(self.app.config["SECRET_KEY"])
 
     def test_next_uri(self) -> None:
         """Tests the next URI utilities with the next URI.
 
         :return: None.
         """
         def test_next_uri_view() -> str:
             """The test view with the next URI."""
             current_uri: str = request.full_path if request.query_string \
                 else request.path
             self.assertEqual(append_next(self.TARGET),
-                             f"{self.TARGET}?next={quote_plus(current_uri)}")
+                             f"{self.TARGET}?next={self.__encode(current_uri)}")
             next_uri: str = request.form["next"] if request.method == "POST" \
                 else request.args["next"]
             self.assertEqual(inherit_next(self.TARGET),
-                             f"{self.TARGET}?next={quote_plus(next_uri)}")
-            self.assertEqual(or_next(self.TARGET), next_uri)
+                             f"{self.TARGET}?next={next_uri}")
+            self.assertEqual(or_next(self.TARGET), self.__decode(next_uri))
             return ""
 
         self.app.add_url_rule("/test-next", view_func=test_next_uri_view,
                               methods=["GET", "POST"])
         client: httpx.Client = httpx.Client(app=self.app, base_url=TEST_SERVER)
         client.headers["Referer"] = TEST_SERVER
         csrf_token: str = get_csrf_token(client)
         response: httpx.Response
 
-        response = client.get("/test-next?next=/next&q=abc&page-no=4")
+        encoded_uri: str = self.__encode(NEXT_URI)
+        response = client.get(f"/test-next?next={encoded_uri}&q=abc&page-no=4")
         self.assertEqual(response.status_code, 200)
         response = client.post("/test-next", data={"csrf_token": csrf_token,
-                                                   "next": "/next",
+                                                   "next": encoded_uri,
                                                    "name": "viewer"})
         self.assertEqual(response.status_code, 200)
 
     def test_no_next_uri(self) -> None:
         """Tests the next URI utilities without the next URI.
 
         :return: None.
         """
         def test_no_next_uri_view() -> str:
             """The test view without the next URI."""
-            current_uri: str = request.full_path if request.query_string \
-                else request.path
-            self.assertEqual(append_next(self.TARGET),
-                             f"{self.TARGET}?next={quote_plus(current_uri)}")
             self.assertEqual(inherit_next(self.TARGET), self.TARGET)
             self.assertEqual(or_next(self.TARGET), self.TARGET)
             return ""
 
         self.app.add_url_rule("/test-no-next", view_func=test_no_next_uri_view,
                               methods=["GET", "POST"])
         client: httpx.Client = httpx.Client(app=self.app, base_url=TEST_SERVER)
@@ -104,18 +104,16 @@
     def test_invalid(self) -> None:
         """Tests the next URI utilities without an invalid next URI.
 
         :return: None.
         """
         def test_invalid_next_uri_view() -> str:
             """The test view without the next URI."""
-            self.assertEqual(inherit_next(self.TARGET),
-                             request.args.get("inherit-expected"))
-            self.assertEqual(or_next(self.TARGET),
-                             request.args.get("or-expected"))
+            self.assertEqual(inherit_next(self.TARGET), self.TARGET)
+            self.assertEqual(or_next(self.TARGET), self.TARGET)
             return ""
 
         self.app.add_url_rule("/test-invalid-next",
                               view_func=test_invalid_next_uri_view,
                               methods=["GET", "POST"])
         client: httpx.Client = httpx.Client(app=self.app, base_url=TEST_SERVER)
         client.headers["Referer"] = TEST_SERVER
@@ -123,42 +121,37 @@
         next_uri: str
         expected1: str
         expected2: str
         response: httpx.Response
 
         # A foreign URI
         next_uri = "https://example.com"
-        expected1 = self.TARGET
-        expected2 = self.TARGET
-        response = client.get(f"/test-invalid-next?next={quote_plus(next_uri)}"
-                              f"&inherit-expected={quote_plus(expected1)}"
-                              f"&or-expected={quote_plus(expected2)}")
-        self.assertEqual(response.status_code, 200)
-        response = client.post("/test-invalid-next"
-                               f"?inherit-expected={quote_plus(expected1)}"
-                               f"&or-expected={quote_plus(expected2)}",
-                               data={"csrf_token": csrf_token,
-                                     "next": next_uri})
+        response = client.get(f"/test-invalid-next?next={quote_plus(next_uri)}")
         self.assertEqual(response.status_code, 200)
-
-        # An extremely-long URI to trigger the error
-        next_uri = "/" + "x" * 1024
-        expected2 = next_uri[:512]
-        expected1 = f"{self.TARGET}?next={quote_plus(expected2)}"
-        response = client.get(f"/test-invalid-next?next={quote_plus(next_uri)}"
-                              f"&inherit-expected={quote_plus(expected1)}"
-                              f"&or-expected={quote_plus(expected2)}")
-        self.assertEqual(response.status_code, 200)
-        response = client.post("/test-invalid-next"
-                               f"?inherit-expected={quote_plus(expected1)}"
-                               f"&or-expected={quote_plus(expected2)}",
+        response = client.post("/test-invalid-next",
                                data={"csrf_token": csrf_token,
                                      "next": next_uri})
         self.assertEqual(response.status_code, 200)
 
+    def __encode(self, uri: str) -> str:
+        """Encodes the next URI.
+
+        :param uri: The next URI.
+        :return: The encoded next URI.
+        """
+        return self.serializer.dumps(uri, "next")
+
+    def __decode(self, uri: str) -> str:
+        """Decodes the next URI.
+
+        :param uri: The encoded next URI.
+        :return: The next URI.
+        """
+        return self.serializer.loads(uri, "next")
+
 
 class QueryKeywordParserTestCase(unittest.TestCase):
     """The test case for the query keyword parser."""
 
     def test_default(self) -> None:
         """Tests the query keyword parser.
```

### Comparing `mia-accounting-1.5.4/tests/testlib.py` & `mia-accounting-1.5.5/tests/testlib.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 import re
 from typing import Literal
 
 import httpx
 from flask import Flask, render_template_string
 
+from accounting.utils.next_uri import encode_next
 from test_site import create_app
 
 TEST_SERVER: str = "https://testserver"
 """The test server URI."""
 NEXT_URI: str = "/_next"
 """The next URI."""
 
@@ -67,17 +68,17 @@
     app: Flask = create_app(is_testing=True)
 
     @app.get("/.csrf-token")
     def get_csrf_token_view() -> str:
         """The test view to return the CSRF token."""
         return render_template_string("{{csrf_token()}}")
 
-    @app.get("/.errors")
-    def get_errors_view() -> str:
-        """The test view to return the CSRF token."""
+    @app.get("/.messages")
+    def get_messages_view() -> str:
+        """The test view to return the flashed messages."""
         return render_template_string("{{get_flashed_messages()|tojson}}")
 
     return app
 
 
 def get_csrf_token(client: httpx.Client) -> str:
     """Returns the CSRF token.
@@ -94,38 +95,43 @@
     :param app: The Flask application.
     :param username: The username.
     :return: A tuple of the client and the CSRF token.
     """
     client: httpx.Client = httpx.Client(app=app, base_url=TEST_SERVER)
     client.headers["Referer"] = TEST_SERVER
     csrf_token: str = get_csrf_token(client)
+    with app.app_context():
+        encoded_next_uri: str = encode_next(NEXT_URI)
     response: httpx.Response = client.post("/login",
                                            data={"csrf_token": csrf_token,
-                                                 "next": "/",
+                                                 "next": encoded_next_uri,
                                                  "username": username})
     assert response.status_code == 302
-    assert response.headers["Location"] == "/"
+    assert response.headers["Location"] == NEXT_URI
     return client, csrf_token
 
 
-def set_locale(client: httpx.Client, csrf_token: str,
+def set_locale(app: Flask, client: httpx.Client, csrf_token: str,
                locale: Literal["en", "zh_Hant", "zh_Hans"]) -> None:
     """Sets the current locale.
 
+    :param app: The Flask application.
     :param client: The test client.
     :param csrf_token: The CSRF token.
     :param locale: The locale.
     :return: None.
     """
+    with app.app_context():
+        encoded_next_uri: str = encode_next(NEXT_URI)
     response: httpx.Response = client.post("/locale",
                                            data={"csrf_token": csrf_token,
                                                  "locale": locale,
-                                                 "next": "/next"})
+                                                 "next": encoded_next_uri})
     assert response.status_code == 302
-    assert response.headers["Location"] == "/next"
+    assert response.headers["Location"] == NEXT_URI
 
 
 def add_journal_entry(client: httpx.Client, form: dict[str, str]) -> int:
     """Adds a transfer journal entry.
 
     :param client: The client.
     :param form: The form data.
@@ -148,10 +154,10 @@
     returns the journal entry ID on success.
 
     :param location: The redirect location.
     :return: The journal entry ID.
     :raise AssertionError: When the location is not the journal entry detail.
     """
     m: re.Match = re.match(
-        r"^/accounting/journal-entries/(\d+)\?next=%2F_next", location)
+        r"^/accounting/journal-entries/(\d+)\?next=", location)
     assert m is not None
     return int(m.group(1))
```

### Comparing `mia-accounting-1.5.4/tests/testlib_journal_entry.py` & `mia-accounting-1.5.5/tests/testlib_journal_entry.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,22 +29,23 @@
 
 NON_EMPTY_NOTE: str = "  This is \n\na test."
 """The stripped content of an non-empty note."""
 EMPTY_NOTE: str = " \n\n  "
 """The empty note content."""
 
 
-def get_add_form(csrf_token: str) -> dict[str, str]:
+def get_add_form(csrf_token: str, encoded_next_uri: str) -> dict[str, str]:
     """Returns the form data to add a new journal entry.
 
     :param csrf_token: The CSRF token.
+    :param encoded_next_uri: The encoded next URI.
     :return: The form data to add a new journal entry.
     """
     return {"csrf_token": csrf_token,
-            "next": NEXT_URI,
+            "next": encoded_next_uri,
             "date": dt.date.today().isoformat(),
             "currency-0-code": "USD",
             "currency-0-debit-0-no": "16",
             "currency-0-debit-0-account_code": Accounts.CASH,
             "currency-0-debit-0-description": " ",
             "currency-0-debit-0-amount": " 495.26 ",
             "currency-0-debit-6-no": "2",
@@ -98,34 +99,36 @@
             "currency-16-credit-9-account_code": Accounts.DONATION,
             "currency-16-credit-9-description": " Donation ",
             "currency-16-credit-9-amount": "5000",
             "note": f"\n \n\n  \n{NON_EMPTY_NOTE}  \n  \n\n  "}
 
 
 def get_unchanged_update_form(journal_entry_id: int, app: Flask,
-                              csrf_token: str) -> dict[str, str]:
+                              csrf_token: str, encoded_next_uri: str) \
+        -> dict[str, str]:
     """Returns the form data to update a journal entry, where the data are not
     changed.
 
     :param journal_entry_id: The journal entry ID.
     :param app: The Flask application.
     :param csrf_token: The CSRF token.
+    :param encoded_next_uri: The encoded next URI.
     :return: The form data to update the journal entry, where the data are not
         changed.
     """
     from accounting.models import JournalEntry, JournalEntryCurrency
     with app.app_context():
         journal_entry: JournalEntry | None \
             = db.session.get(JournalEntry, journal_entry_id)
         assert journal_entry is not None
         currencies: list[JournalEntryCurrency] = journal_entry.currencies
 
     form: dict[str, str] \
         = {"csrf_token": csrf_token,
-           "next": NEXT_URI,
+           "next": encoded_next_uri,
            "date": journal_entry.date,
            "note": "  \n \n\n  " if journal_entry.note is None
            else f"\n    \n\n \n  \n{journal_entry.note}  \n\n   "}
     currency_indices_used: set[int] = set()
     currency_no: int = 0
     for currency in currencies:
         currency_index: int = __get_new_index(currency_indices_used)
@@ -178,28 +181,30 @@
         index: int = randbelow(100)
         if index not in indices_used:
             indices_used.add(index)
             return index
 
 
 def get_update_form(journal_entry_id: int, app: Flask,
-                    csrf_token: str, is_debit: bool | None) -> dict[str, str]:
+                    csrf_token: str, encoded_next_uri: str,
+                    is_debit: bool | None) -> dict[str, str]:
     """Returns the form data to update a journal entry, where the data are
     changed.
 
     :param journal_entry_id: The journal entry ID.
     :param app: The Flask application.
     :param csrf_token: The CSRF token.
+    :param encoded_next_uri: The encoded next URI.
     :param is_debit: True for a cash disbursement journal entry, False for a
         cash receipt journal entry, or None for a transfer journal entry.
     :return: The form data to update the journal entry, where the data are
         changed.
     """
     form: dict[str, str] = get_unchanged_update_form(
-        journal_entry_id, app, csrf_token)
+        journal_entry_id, app, csrf_token, encoded_next_uri)
 
     # Mess up the line items in a currency
     currency_prefix: str = __get_currency_prefix(form, "USD")
     if is_debit is None or is_debit:
         form = __mess_up_debit(form, currency_prefix)
     if is_debit is None or not is_debit:
         form = __mess_up_credit(form, currency_prefix)
```

