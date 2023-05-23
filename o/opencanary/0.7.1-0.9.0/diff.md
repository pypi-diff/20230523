# Comparing `tmp/opencanary-0.7.1.tar.gz` & `tmp/opencanary-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/opencanary-0.7.1.tar", last modified: Fri Jul  1 10:07:48 2022, max compression
+gzip compressed data, was "opencanary-0.9.0.tar", last modified: Tue May 23 12:36:08 2023, max compression
```

## Comparing `opencanary-0.7.1.tar` & `opencanary-0.9.0.tar`

### file list

```diff
@@ -1,325 +1,303 @@
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/.github/
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/.github/workflows/
--rw-r--r--   0 jay        (501) staff       (20)     1262 2022-06-23 08:31:57.000000 opencanary-0.7.1/.github/workflows/opencanary_tests.yml
--rw-r--r--   0 jay        (501) staff       (20)     1417 2022-06-23 10:42:17.000000 opencanary-0.7.1/.gitignore
--rw-r--r--   0 jay        (501) staff       (20)      856 2022-06-23 08:31:57.000000 opencanary-0.7.1/Dockerfile.latest
--rw-r--r--   0 jay        (501) staff       (20)      664 2022-06-23 08:31:57.000000 opencanary-0.7.1/Dockerfile.stable
--rw-r--r--   0 jay        (501) staff       (20)     1495 2018-10-11 07:15:41.000000 opencanary-0.7.1/LICENSE
--rw-r--r--   0 jay        (501) staff       (20)     1028 2022-07-01 10:07:48.000000 opencanary-0.7.1/PKG-INFO
--rw-r--r--   0 jay        (501) staff       (20)     5807 2022-06-23 08:31:57.000000 opencanary-0.7.1/README.md
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/bin/
--rwxr-xr-x   0 jay        (501) staff       (20)      240 2020-05-11 08:35:29.000000 opencanary-0.7.1/bin/honeycred
--rwxr-xr-x   0 jay        (501) staff       (20)      107 2018-06-14 14:00:23.000000 opencanary-0.7.1/bin/opencanary-correlator
--rw-r--r--   0 jay        (501) staff       (20)     4903 2021-09-15 12:40:44.000000 opencanary-0.7.1/bin/opencanary.tac
--rwxr-xr-x   0 jay        (501) staff       (20)     3053 2022-07-01 09:21:13.000000 opencanary-0.7.1/bin/opencanaryd
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/data/
--rw-r--r--   0 jay        (501) staff       (20)     3353 2022-06-23 08:31:57.000000 opencanary-0.7.1/data/.opencanary.conf
--rw-r--r--   0 jay        (501) staff       (20)     1068 2022-06-23 08:31:57.000000 opencanary-0.7.1/docker-compose.yml
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/docs/
--rw-r--r--   0 jay        (501) staff       (20)     7425 2018-06-14 14:00:23.000000 opencanary-0.7.1/docs/Makefile
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/docs/alerts/
--rw-r--r--   0 jay        (501) staff       (20)     3222 2022-06-23 08:31:57.000000 opencanary-0.7.1/docs/alerts/email.rst
--rw-r--r--   0 jay        (501) staff       (20)      787 2022-06-23 08:31:57.000000 opencanary-0.7.1/docs/alerts/hpfeeds.rst
--rw-r--r--   0 jay        (501) staff       (20)     3348 2022-06-30 07:24:28.000000 opencanary-0.7.1/docs/alerts/webhook.rst
--rw-r--r--   0 jay        (501) staff       (20)     9294 2021-09-15 04:53:55.000000 opencanary-0.7.1/docs/conf.py
--rw-r--r--   0 jay        (501) staff       (20)     2083 2022-06-23 14:49:53.000000 opencanary-0.7.1/docs/index.rst
--rw-r--r--   0 jay        (501) staff       (20)   175916 2018-10-09 12:31:45.000000 opencanary-0.7.1/docs/logo.png
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/docs/services/
--rw-r--r--   0 jay        (501) staff       (20)      266 2018-06-14 14:00:23.000000 opencanary-0.7.1/docs/services/mssql.rst
--rw-r--r--   0 jay        (501) staff       (20)      307 2018-06-14 14:00:23.000000 opencanary-0.7.1/docs/services/mysql.rst
--rw-r--r--   0 jay        (501) staff       (20)      650 2018-06-14 14:00:23.000000 opencanary-0.7.1/docs/services/webserver.rst
--rw-r--r--   0 jay        (501) staff       (20)     2169 2022-06-15 16:04:22.000000 opencanary-0.7.1/docs/services/windows.rst
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/docs/starting/
--rw-r--r--   0 jay        (501) staff       (20)    10668 2022-06-30 07:24:28.000000 opencanary-0.7.1/docs/starting/configuration.rst
--rw-r--r--   0 jay        (501) staff       (20)     2655 2022-06-15 16:04:22.000000 opencanary-0.7.1/docs/starting/correlator.rst
--rw-r--r--   0 jay        (501) staff       (20)     1895 2022-06-15 16:04:22.000000 opencanary-0.7.1/docs/starting/opencanary.rst
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/
--rw-r--r--   0 jay        (501) staff       (20)       19 2022-07-01 10:07:44.000000 opencanary-0.7.1/opencanary/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)     9587 2022-06-23 08:31:57.000000 opencanary-0.7.1/opencanary/config.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/data/
--rw-r--r--   0 jay        (501) staff       (20)      341 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/data/settings-usermodule.json
--rw-r--r--   0 jay        (501) staff       (20)     2920 2021-09-15 12:40:44.000000 opencanary-0.7.1/opencanary/data/settings.json
--rw-r--r--   0 jay        (501) staff       (20)     1062 2022-06-30 07:25:10.000000 opencanary-0.7.1/opencanary/honeycred.py
--rw-r--r--   0 jay        (501) staff       (20)      752 2021-02-22 09:01:56.000000 opencanary-0.7.1/opencanary/iphelper.py
--rw-r--r--   0 jay        (501) staff       (20)    12733 2022-06-23 14:49:53.000000 opencanary-0.7.1/opencanary/logger.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/
--rw-r--r--   0 jay        (501) staff       (20)     5967 2021-05-26 07:19:26.000000 opencanary-0.7.1/opencanary/modules/__init__.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/http/
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/basicLogin/
--rw-r--r--   0 jay        (501) staff       (20)      250 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/basicLogin/403.html
--rw-r--r--   0 jay        (501) staff       (20)      246 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/basicLogin/404.html
--rw-r--r--   0 jay        (501) staff       (20)     1146 2021-05-26 06:15:33.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/basicLogin/index.html
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/
--rw-r--r--   0 jay        (501) staff       (20)      250 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/403.html
--rw-r--r--   0 jay        (501) staff       (20)      246 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/404.html
--rw-r--r--   0 jay        (501) staff       (20)    10293 2022-06-15 16:04:22.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/index.html
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/css/
--rw-r--r--   0 jay        (501) staff       (20)   259371 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/css/desktop.css
--rw-r--r--   0 jay        (501) staff       (20)   117346 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/css/ext-all.css
--rw-r--r--   0 jay        (501) staff       (20)     1417 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/css/style.css
--rw-r--r--   0 jay        (501) staff       (20)   193133 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/css/ux-all.css
--rw-r--r--   0 jay        (501) staff       (20)    38501 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/css/xtheme-gray.css
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/fonts/
--rw-r--r--   0 jay        (501) staff       (20)    22172 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/fonts/roboto.woff
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/
--rw-r--r--   0 jay        (501) staff       (20)   305783 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/02.jpg
--rw-r--r--   0 jay        (501) staff       (20)    15086 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/favicon.ico
--rw-r--r--   0 jay        (501) staff       (20)     1191 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/icon_dsm_16.png
--rw-r--r--   0 jay        (501) staff       (20)     1351 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/icon_dsm_32.png
--rw-r--r--   0 jay        (501) staff       (20)     1603 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/icon_dsm_48.png
--rw-r--r--   0 jay        (501) staff       (20)     1706 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/icon_dsm_64.png
--rw-r--r--   0 jay        (501) staff       (20)     2123 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/icon_dsm_96.png
--rw-r--r--   0 jay        (501) staff       (20)     2093 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/icon_tile.png
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/
--rw-r--r--   0 jay        (501) staff       (20)     1208 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/bt_dropdown.png
--rw-r--r--   0 jay        (501) staff       (20)      455 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/bt_grid_dropdown.png
--rw-r--r--   0 jay        (501) staff       (20)     4750 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/bt_pagebar.png
--rw-r--r--   0 jay        (501) staff       (20)     8754 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/c_icon_general.png
--rw-r--r--   0 jay        (501) staff       (20)      907 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/category_expand.png
--rw-r--r--   0 jay        (501) staff       (20)     3535 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/checkbox.png
--rw-r--r--   0 jay        (501) staff       (20)     1027 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/col-move-bottom.png
--rw-r--r--   0 jay        (501) staff       (20)      343 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/date_dropdown.png
--rw-r--r--   0 jay        (501) staff       (20)     1374 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/date_prev_next.png
--rw-r--r--   0 jay        (501) staff       (20)      344 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/dropdown_menu_parent.png
--rw-r--r--   0 jay        (501) staff       (20)      823 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/dropdown_menu_tick.png
--rw-r--r--   0 jay        (501) staff       (20)     2729 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/fieldset_expand.png
--rw-r--r--   0 jay        (501) staff       (20)     1975 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/icon_advanced_search.png
--rw-r--r--   0 jay        (501) staff       (20)      644 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/icon_error.png
--rw-r--r--   0 jay        (501) staff       (20)      372 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/icon_filter.png
--rw-r--r--   0 jay        (501) staff       (20)     3373 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/icon_information.png
--rw-r--r--   0 jay        (501) staff       (20)      491 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/icon_loading.gif
--rw-r--r--   0 jay        (501) staff       (20)      842 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/icon_search.png
--rw-r--r--   0 jay        (501) staff       (20)     6219 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/icon_search_clear.png
--rw-r--r--   0 jay        (501) staff       (20)      972 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/icon_success.png
--rw-r--r--   0 jay        (501) staff       (20)     4979 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/radio_button.png
--rw-r--r--   0 jay        (501) staff       (20)      137 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/shadow_category.png
--rw-r--r--   0 jay        (501) staff       (20)      138 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/shadow_footbar.png
--rw-r--r--   0 jay        (501) staff       (20)     1649 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/superbox_button_cancel.png
--rw-r--r--   0 jay        (501) staff       (20)      501 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/tab_arrow.png
--rw-r--r--   0 jay        (501) staff       (20)     1065 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/tab_shadow.png
--rw-r--r--   0 jay        (501) staff       (20)      372 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/tree_arrow.png
--rw-r--r--   0 jay        (501) staff       (20)      517 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/trigger.png
--rw-r--r--   0 jay        (501) staff       (20)      472 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/trigger_date.png
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/ExternalDevices/
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/ExternalDevices/images/
--rw-r--r--   0 jay        (501) staff       (20)     4156 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/ExternalDevices/images/tray_icon_device.png
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/FileTaskMonitor/
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/FileTaskMonitor/images/
--rw-r--r--   0 jay        (501) staff       (20)     5812 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/FileTaskMonitor/images/tray_icon_bgtask.gif
--rw-r--r--   0 jay        (501) staff       (20)      928 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/FileTaskMonitor/images/tray_icon_bgtask.png
--rw-r--r--   0 jay        (501) staff       (20)     6810 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/FileTaskMonitor/images/tray_icon_download.gif
--rw-r--r--   0 jay        (501) staff       (20)     1192 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/FileTaskMonitor/images/tray_icon_download.png
--rw-r--r--   0 jay        (501) staff       (20)     6658 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/FileTaskMonitor/images/tray_icon_upload.gif
--rw-r--r--   0 jay        (501) staff       (20)     1129 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/FileTaskMonitor/images/tray_icon_upload.png
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/PollingTask/
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/PollingTask/images/
--rw-r--r--   0 jay        (501) staff       (20)     5685 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/PollingTask/images/tray_icon_disk_port.png
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/ThumbConvertProgress/
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/ThumbConvertProgress/images/
--rw-r--r--   0 jay        (501) staff       (20)     3073 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/ThumbConvertProgress/images/tray_icon_creating_thumbnail.gif
--rw-r--r--   0 jay        (501) staff       (20)     2125 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/ThumbConvertProgress/images/tray_icon_creating_thumbnail.png
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/
--rw-r--r--   0 jay        (501) staff       (20)    35658 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/bt_bugs.png
--rw-r--r--   0 jay        (501) staff       (20)    27469 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/bt_dsm_mobile.png
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/components/
--rw-r--r--   0 jay        (501) staff       (20)     2031 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/components/icon_error.png
--rw-r--r--   0 jay        (501) staff       (20)     1748 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/components/icon_image_selector.png
--rw-r--r--   0 jay        (501) staff       (20)     1372 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/components/status_fail.png
--rw-r--r--   0 jay        (501) staff       (20)     1549 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/components/status_loading.gif
--rw-r--r--   0 jay        (501) staff       (20)     1322 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/components/status_success.png
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/desktop/
--rw-r--r--   0 jay        (501) staff       (20)     2537 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/desktop/add_one.png
--rw-r--r--   0 jay        (501) staff       (20)     8458 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/desktop/icon_app_category.png
--rw-r--r--   0 jay        (501) staff       (20)    11321 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/desktop/spotlight.png
--rw-r--r--   0 jay        (501) staff       (20)     2164 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/desktop/taskbar_spinner.gif
--rw-r--r--   0 jay        (501) staff       (20)    36970 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/dsm5_badge_num.png
--rw-r--r--   0 jay        (501) staff       (20)    21353 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/dsm5_notification_num.png
--rw-r--r--   0 jay        (501) staff       (20)     9530 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/dsmv5_wizard_bkg_v_01.png
--rw-r--r--   0 jay        (501) staff       (20)    63006 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/dsmv5_wizard_bkg_v_02.png
--rw-r--r--   0 jay        (501) staff       (20)      590 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/folder.png
--rw-r--r--   0 jay        (501) staff       (20)     2536 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/icon_drag_add.png
--rw-r--r--   0 jay        (501) staff       (20)     2388 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/icon_drag_ban.png
--rw-r--r--   0 jay        (501) staff       (20)     3630 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/icon_question.png
--rw-r--r--   0 jay        (501) staff       (20)     1637 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/item_drag_status.png
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/
--rw-r--r--   0 jay        (501) staff       (20)     1565 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/0.png
--rw-r--r--   0 jay        (501) staff       (20)     1165 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/1.png
--rw-r--r--   0 jay        (501) staff       (20)     1554 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/2.png
--rw-r--r--   0 jay        (501) staff       (20)     1704 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/3.png
--rw-r--r--   0 jay        (501) staff       (20)     1419 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/4.png
--rw-r--r--   0 jay        (501) staff       (20)     1589 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/5dot.png
--rw-r--r--   0 jay        (501) staff       (20)     2462 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/DSM.png
--rw-r--r--   0 jay        (501) staff       (20)     1735 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/beta.png
--rw-r--r--   0 jay        (501) staff       (20)     8323 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/copyright_2014.png
--rw-r--r--   0 jay        (501) staff       (20)     8318 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/copyright_2015.png
--rw-r--r--   0 jay        (501) staff       (20)     7719 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/synology.png
--rw-r--r--   0 jay        (501) staff       (20)      698 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/icon_phone.png
--rw-r--r--   0 jay        (501) staff       (20)     3913 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/icon_pw.png
--rw-r--r--   0 jay        (501) staff       (20)     3730 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/icon_user.png
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/
--rw-r--r--   0 jay        (501) staff       (20)      834 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/0.png
--rw-r--r--   0 jay        (501) staff       (20)      318 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/1.png
--rw-r--r--   0 jay        (501) staff       (20)      780 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/2.png
--rw-r--r--   0 jay        (501) staff       (20)      982 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/3.png
--rw-r--r--   0 jay        (501) staff       (20)      680 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/4.png
--rw-r--r--   0 jay        (501) staff       (20)      868 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/5dot.png
--rw-r--r--   0 jay        (501) staff       (20)     2070 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/DSM.png
--rw-r--r--   0 jay        (501) staff       (20)     1162 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/beta.png
--rw-r--r--   0 jay        (501) staff       (20)     8323 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/copyright_2014.png
--rw-r--r--   0 jay        (501) staff       (20)     8318 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/copyright_2015.png
--rw-r--r--   0 jay        (501) staff       (20)     8469 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/synology.png
--rw-r--r--   0 jay        (501) staff       (20)     6772 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/login_bkg_highlight_bottom.png
--rw-r--r--   0 jay        (501) staff       (20)     8683 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/login_bkg_highlight_top.png
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/
--rw-r--r--   0 jay        (501) staff       (20)    23041 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_cloudy.png
--rw-r--r--   0 jay        (501) staff       (20)    33681 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_cold.png
--rw-r--r--   0 jay        (501) staff       (20)    10119 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_fog.png
--rw-r--r--   0 jay        (501) staff       (20)    27277 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_hail.png
--rw-r--r--   0 jay        (501) staff       (20)    16586 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_moon.png
--rw-r--r--   0 jay        (501) staff       (20)    28148 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_moon_clouds.png
--rw-r--r--   0 jay        (501) staff       (20)    28152 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_rain.png
--rw-r--r--   0 jay        (501) staff       (20)    31584 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_snow.png
--rw-r--r--   0 jay        (501) staff       (20)    21959 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_sun.png
--rw-r--r--   0 jay        (501) staff       (20)    37181 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_sun_clouds.png
--rw-r--r--   0 jay        (501) staff       (20)    27481 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_thunder.png
--rw-r--r--   0 jay        (501) staff       (20)    37188 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_tornado.png
--rw-r--r--   0 jay        (501) staff       (20)    22230 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_windy.png
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/
--rw-r--r--   0 jay        (501) staff       (20)     5229 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_CMS.png
--rw-r--r--   0 jay        (501) staff       (20)     5973 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_backup.png
--rw-r--r--   0 jay        (501) staff       (20)     3767 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_business.png
--rw-r--r--   0 jay        (501) staff       (20)     5282 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_community.png
--rw-r--r--   0 jay        (501) staff       (20)     7444 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_connect.png
--rw-r--r--   0 jay        (501) staff       (20)     5907 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_contact.png
--rw-r--r--   0 jay        (501) staff       (20)     4389 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_directory_service.png
--rw-r--r--   0 jay        (501) staff       (20)     5446 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_dsm_apps.png
--rw-r--r--   0 jay        (501) staff       (20)     4339 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_expansion.png
--rw-r--r--   0 jay        (501) staff       (20)     4126 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_external_devices.png
--rw-r--r--   0 jay        (501) staff       (20)     4867 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_file_services.png
--rw-r--r--   0 jay        (501) staff       (20)     8754 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_general.png
--rw-r--r--   0 jay        (501) staff       (20)     7877 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_groups.png
--rw-r--r--   0 jay        (501) staff       (20)     5937 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_hardware_and_power.png
--rw-r--r--   0 jay        (501) staff       (20)     6498 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_hdd_management.png
--rw-r--r--   0 jay        (501) staff       (20)     4823 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_hot_spare.png
--rw-r--r--   0 jay        (501) staff       (20)     8171 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_info_center.png
--rw-r--r--   0 jay        (501) staff       (20)     4191 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_installed.png
--rw-r--r--   0 jay        (501) staff       (20)     7993 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_iscsi_lun.png
--rw-r--r--   0 jay        (501) staff       (20)    10534 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_iscsi_target.png
--rw-r--r--   0 jay        (501) staff       (20)     8216 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_login_style.png
--rw-r--r--   0 jay        (501) staff       (20)    10244 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_media_library.png
--rw-r--r--   0 jay        (501) staff       (20)     5374 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_network.png
--rw-r--r--   0 jay        (501) staff       (20)     5660 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_networkmap.png
--rw-r--r--   0 jay        (501) staff       (20)     6352 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_notifications.png
--rw-r--r--   0 jay        (501) staff       (20)     5299 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_overview.png
--rw-r--r--   0 jay        (501) staff       (20)     8245 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_performance.png
--rw-r--r--   0 jay        (501) staff       (20)     5136 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_portal.png
--rw-r--r--   0 jay        (501) staff       (20)     4734 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_privilege.png
--rw-r--r--   0 jay        (501) staff       (20)     6985 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_process.png
--rw-r--r--   0 jay        (501) staff       (20)    10097 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_public_access.png
--rw-r--r--   0 jay        (501) staff       (20)     7973 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_purchases.png
--rw-r--r--   0 jay        (501) staff       (20)     6400 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_quickconnect.png
--rw-r--r--   0 jay        (501) staff       (20)     3621 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_raid_group.png
--rw-r--r--   0 jay        (501) staff       (20)     5128 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_recommend.png
--rw-r--r--   0 jay        (501) staff       (20)     9903 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_region.png
--rw-r--r--   0 jay        (501) staff       (20)     7168 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_security.png
--rw-r--r--   0 jay        (501) staff       (20)     5473 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_shared_folders.png
--rw-r--r--   0 jay        (501) staff       (20)    10382 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_speed.png
--rw-r--r--   0 jay        (501) staff       (20)     5255 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_ssd_cache.png
--rw-r--r--   0 jay        (501) staff       (20)     5349 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_syslog.png
--rw-r--r--   0 jay        (501) staff       (20)     5984 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_task_scheduler.png
--rw-r--r--   0 jay        (501) staff       (20)     4008 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_terminal_and_SNMP.png
--rw-r--r--   0 jay        (501) staff       (20)     8440 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_update_and_reset.png
--rw-r--r--   0 jay        (501) staff       (20)     5905 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_users.png
--rw-r--r--   0 jay        (501) staff       (20)     9565 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_utilities.png
--rw-r--r--   0 jay        (501) staff       (20)     8423 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_volume.png
--rw-r--r--   0 jay        (501) staff       (20)     9096 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_web_server.png
--rw-r--r--   0 jay        (501) staff       (20)     7619 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_wireless.png
--rw-r--r--   0 jay        (501) staff       (20)     7805 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/rt_button.png
--rw-r--r--   0 jay        (501) staff       (20)      138 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/shadow_footbar.png
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/
--rw-r--r--   0 jay        (501) staff       (20)     1915 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/more_apps.png
--rw-r--r--   0 jay        (501) staff       (20)     1445 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/showdesktop.png
--rw-r--r--   0 jay        (501) staff       (20)      159 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/taskbar_bg.png
--rw-r--r--   0 jay        (501) staff       (20)     4445 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/taskbar_bt.png
--rw-r--r--   0 jay        (501) staff       (20)    10062 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/taskbar_bt_apps.png
--rw-r--r--   0 jay        (501) staff       (20)      506 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/taskbar_bt_widgets_shadow.png
--rw-r--r--   0 jay        (501) staff       (20)      132 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/taskbar_shadow.png
--rw-r--r--   0 jay        (501) staff       (20)      183 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/taskbar_split.png
--rw-r--r--   0 jay        (501) staff       (20)     6147 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/tray_icon_notification.png
--rw-r--r--   0 jay        (501) staff       (20)     6852 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/tray_icon_pilot_view.png
--rw-r--r--   0 jay        (501) staff       (20)     7569 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/tray_icon_search.png
--rw-r--r--   0 jay        (501) staff       (20)     5077 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/tray_icon_user_menu.png
--rw-r--r--   0 jay        (501) staff       (20)    10337 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/tray_icon_widget.png
--rw-r--r--   0 jay        (501) staff       (20)     3622 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/user_menu_about.png
--rw-r--r--   0 jay        (501) staff       (20)     3876 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/user_menu_logout.png
--rw-r--r--   0 jay        (501) staff       (20)     5337 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/user_menu_options.png
--rw-r--r--   0 jay        (501) staff       (20)     4950 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/user_menu_restart.png
--rw-r--r--   0 jay        (501) staff       (20)     5475 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/user_menu_shutdown.png
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/widget_window/
--rw-r--r--   0 jay        (501) staff       (20)     9577 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/widget_window/widget_rt_button.png
--rw-r--r--   0 jay        (501) staff       (20)    50783 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/wizard_bkg_h.png
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/scrollbar/
--rw-r--r--   0 jay        (501) staff       (20)      134 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/scrollbar/scrollbar_black_h.png
--rw-r--r--   0 jay        (501) staff       (20)      136 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/scrollbar/scrollbar_black_v.png
--rw-r--r--   0 jay        (501) staff       (20)      135 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/scrollbar/scrollbar_white_h.png
--rw-r--r--   0 jay        (501) staff       (20)      127 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/scrollbar/scrollbar_white_v.png
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/js/
--rw-r--r--   0 jay        (501) staff       (20)     1056 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/js/misc.js
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/httpproxy/
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/httpproxy/skin/
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/httpproxy/skin/squid/
--rw-r--r--   0 jay        (501) staff       (20)     2898 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/httpproxy/skin/squid/auth.html
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/modules/data/rdp/
--rw-r--r--   0 jay        (501) staff       (20)  2088348 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/rdp/default.rss
--rw-r--r--   0 jay        (501) staff       (20)   302478 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/rdp/login-failed.rss
--rw-r--r--   0 jay        (501) staff       (20)  1459822 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/rdp/login-passreset.rss
--rw-r--r--   0 jay        (501) staff       (20)   262442 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/data/rdp/login.rss
--rw-r--r--   0 jay        (501) staff       (20)    32259 2020-05-11 08:35:29.000000 opencanary-0.7.1/opencanary/modules/des.py
--rw-r--r--   0 jay        (501) staff       (20)     1430 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/example0.py
--rw-r--r--   0 jay        (501) staff       (20)     2263 2020-05-11 08:35:29.000000 opencanary-0.7.1/opencanary/modules/example1.py
--rw-r--r--   0 jay        (501) staff       (20)     3095 2020-05-11 08:35:29.000000 opencanary-0.7.1/opencanary/modules/ftp.py
--rw-r--r--   0 jay        (501) staff       (20)     2518 2022-06-30 07:24:28.000000 opencanary-0.7.1/opencanary/modules/git.py
--rw-r--r--   0 jay        (501) staff       (20)     6375 2021-01-04 06:54:19.000000 opencanary-0.7.1/opencanary/modules/http.py
--rw-r--r--   0 jay        (501) staff       (20)     5606 2021-09-15 19:16:59.000000 opencanary-0.7.1/opencanary/modules/httpproxy.py
--rw-r--r--   0 jay        (501) staff       (20)    15454 2020-05-11 08:35:29.000000 opencanary-0.7.1/opencanary/modules/mssql.py
--rw-r--r--   0 jay        (501) staff       (20)     6271 2021-08-26 09:18:23.000000 opencanary-0.7.1/opencanary/modules/mysql.py
--rw-r--r--   0 jay        (501) staff       (20)     1615 2021-09-14 05:01:16.000000 opencanary-0.7.1/opencanary/modules/ntp.py
--rw-r--r--   0 jay        (501) staff       (20)     7447 2021-09-15 12:40:44.000000 opencanary-0.7.1/opencanary/modules/portscan.py
--rw-r--r--   0 jay        (501) staff       (20)     3177 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/rdp.py
--rw-r--r--   0 jay        (501) staff       (20)    13263 2020-05-11 08:35:29.000000 opencanary-0.7.1/opencanary/modules/redis.py
--rw-r--r--   0 jay        (501) staff       (20)     2774 2022-03-01 06:51:14.000000 opencanary-0.7.1/opencanary/modules/samba.py
--rw-r--r--   0 jay        (501) staff       (20)     1183 2020-05-11 08:35:29.000000 opencanary-0.7.1/opencanary/modules/sip.py
--rw-r--r--   0 jay        (501) staff       (20)     1364 2020-05-11 08:35:29.000000 opencanary-0.7.1/opencanary/modules/snmp.py
--rw-r--r--   0 jay        (501) staff       (20)    15350 2021-06-04 13:50:32.000000 opencanary-0.7.1/opencanary/modules/ssh.py
--rw-r--r--   0 jay        (501) staff       (20)     7520 2020-05-11 08:35:29.000000 opencanary-0.7.1/opencanary/modules/tcpbanner.py
--rw-r--r--   0 jay        (501) staff       (20)     2909 2020-05-11 08:35:29.000000 opencanary-0.7.1/opencanary/modules/telnet.py
--rw-r--r--   0 jay        (501) staff       (20)        0 2019-09-03 20:04:12.000000 opencanary-0.7.1/opencanary/modules/test.py
--rw-r--r--   0 jay        (501) staff       (20)     3215 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/modules/testpdf.py
--rw-r--r--   0 jay        (501) staff       (20)     1527 2020-05-11 08:35:29.000000 opencanary-0.7.1/opencanary/modules/tftp.py
--rw-r--r--   0 jay        (501) staff       (20)     5461 2021-08-25 12:52:28.000000 opencanary-0.7.1/opencanary/modules/vnc.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary/test/
--rw-r--r--   0 jay        (501) staff       (20)      115 2018-06-14 14:00:23.000000 opencanary-0.7.1/opencanary/test/logger.py
--rw-r--r--   0 jay        (501) staff       (20)    10768 2022-06-23 08:31:57.000000 opencanary-0.7.1/opencanary/test/module_test.py
--rw-r--r--   0 jay        (501) staff       (20)     3351 2022-06-23 08:31:57.000000 opencanary-0.7.1/opencanary/test/opencanary.conf
--rw-r--r--   0 jay        (501) staff       (20)       43 2022-06-23 08:31:57.000000 opencanary-0.7.1/opencanary/test/requirements.txt
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary.egg-info/
--rw-r--r--   0 jay        (501) staff       (20)     1028 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary.egg-info/PKG-INFO
--rw-r--r--   0 jay        (501) staff       (20)    24274 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary.egg-info/SOURCES.txt
--rw-r--r--   0 jay        (501) staff       (20)        1 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary.egg-info/dependency_links.txt
--rw-r--r--   0 jay        (501) staff       (20)      225 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary.egg-info/requires.txt
--rw-r--r--   0 jay        (501) staff       (20)       11 2022-07-01 10:07:48.000000 opencanary-0.7.1/opencanary.egg-info/top_level.txt
--rw-r--r--   0 jay        (501) staff       (20)      288 2021-08-26 09:15:18.000000 opencanary-0.7.1/opencanary.service
--rw-r--r--   0 jay        (501) staff       (20)        5 2018-06-14 14:00:23.000000 opencanary-0.7.1/requirements.txt
--rw-r--r--   0 jay        (501) staff       (20)      391 2021-05-26 06:15:33.000000 opencanary-0.7.1/run.sh
--rw-r--r--   0 jay        (501) staff       (20)       38 2022-07-01 10:07:48.000000 opencanary-0.7.1/setup.cfg
--rw-r--r--   0 jay        (501) staff       (20)     2657 2022-07-01 09:23:07.000000 opencanary-0.7.1/setup.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.175515 opencanary-0.9.0/
+-rw-r--r--   0 jay        (501) staff       (20)     1495 2018-10-11 07:15:41.000000 opencanary-0.9.0/LICENSE
+-rw-r--r--   0 jay        (501) staff       (20)      263 2023-02-21 19:54:37.000000 opencanary-0.9.0/MANIFEST.in
+-rw-r--r--   0 jay        (501) staff       (20)      988 2023-05-23 12:36:08.175332 opencanary-0.9.0/PKG-INFO
+-rw-r--r--   0 jay        (501) staff       (20)     5671 2023-05-19 11:08:10.000000 opencanary-0.9.0/README.md
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.110637 opencanary-0.9.0/bin/
+-rwxr-xr-x   0 jay        (501) staff       (20)      199 2022-07-27 09:45:25.000000 opencanary-0.9.0/bin/honeycred
+-rwxr-xr-x   0 jay        (501) staff       (20)      107 2018-06-14 14:00:23.000000 opencanary-0.9.0/bin/opencanary-correlator
+-rw-r--r--   0 jay        (501) staff       (20)     4920 2023-05-19 11:08:10.000000 opencanary-0.9.0/bin/opencanary.tac
+-rwxr-xr-x   0 jay        (501) staff       (20)     2776 2022-07-27 09:46:56.000000 opencanary-0.9.0/bin/opencanaryd
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.111081 opencanary-0.9.0/build_scripts/
+-rwxr-xr-x   0 jay        (501) staff       (20)     6349 2023-05-19 11:08:10.000000 opencanary-0.9.0/build_scripts/generate_macOS_launchctl_service_files.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.111322 opencanary-0.9.0/data/
+-rw-r--r--   0 jay        (501) staff       (20)     3551 2023-05-18 06:56:45.000000 opencanary-0.9.0/data/.opencanary.conf
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.112420 opencanary-0.9.0/opencanary/
+-rw-r--r--   0 jay        (501) staff       (20)       19 2023-05-23 10:19:20.000000 opencanary-0.9.0/opencanary/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)     8891 2023-02-21 19:54:37.000000 opencanary-0.9.0/opencanary/config.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.113584 opencanary-0.9.0/opencanary/data/
+-rw-r--r--   0 jay        (501) staff       (20)      341 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/data/settings-usermodule.json
+-rw-r--r--   0 jay        (501) staff       (20)     3119 2023-05-18 06:56:45.000000 opencanary-0.9.0/opencanary/data/settings.json
+-rw-r--r--   0 jay        (501) staff       (20)     1062 2022-06-30 07:25:10.000000 opencanary-0.9.0/opencanary/honeycred.py
+-rw-r--r--   0 jay        (501) staff       (20)      752 2021-02-22 09:01:56.000000 opencanary-0.9.0/opencanary/iphelper.py
+-rw-r--r--   0 jay        (501) staff       (20)    12835 2023-05-23 10:18:33.000000 opencanary-0.9.0/opencanary/logger.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.119187 opencanary-0.9.0/opencanary/modules/
+-rw-r--r--   0 jay        (501) staff       (20)     5967 2021-05-26 07:19:26.000000 opencanary-0.9.0/opencanary/modules/__init__.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.108175 opencanary-0.9.0/opencanary/modules/data/
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.105892 opencanary-0.9.0/opencanary/modules/data/http/
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.105994 opencanary-0.9.0/opencanary/modules/data/http/skin/
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.119827 opencanary-0.9.0/opencanary/modules/data/http/skin/basicLogin/
+-rw-r--r--   0 jay        (501) staff       (20)      250 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/basicLogin/403.html
+-rw-r--r--   0 jay        (501) staff       (20)      246 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/basicLogin/404.html
+-rw-r--r--   0 jay        (501) staff       (20)     1146 2021-05-26 06:15:33.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/basicLogin/index.html
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.120259 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/
+-rw-r--r--   0 jay        (501) staff       (20)      250 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/403.html
+-rw-r--r--   0 jay        (501) staff       (20)      246 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/404.html
+-rw-r--r--   0 jay        (501) staff       (20)    10293 2022-06-15 16:04:22.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/index.html
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.107922 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.122644 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/css/
+-rw-r--r--   0 jay        (501) staff       (20)   259371 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/css/desktop.css
+-rw-r--r--   0 jay        (501) staff       (20)   117346 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/css/ext-all.css
+-rw-r--r--   0 jay        (501) staff       (20)     1417 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/css/style.css
+-rw-r--r--   0 jay        (501) staff       (20)   193133 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/css/ux-all.css
+-rw-r--r--   0 jay        (501) staff       (20)    38501 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/css/xtheme-gray.css
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.122838 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/fonts/
+-rw-r--r--   0 jay        (501) staff       (20)    22172 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/fonts/roboto.woff
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.124646 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/
+-rw-r--r--   0 jay        (501) staff       (20)   305783 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/02.jpg
+-rw-r--r--   0 jay        (501) staff       (20)    15086 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/favicon.ico
+-rw-r--r--   0 jay        (501) staff       (20)     1191 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/icon_dsm_16.png
+-rw-r--r--   0 jay        (501) staff       (20)     1351 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/icon_dsm_32.png
+-rw-r--r--   0 jay        (501) staff       (20)     1603 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/icon_dsm_48.png
+-rw-r--r--   0 jay        (501) staff       (20)     1706 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/icon_dsm_64.png
+-rw-r--r--   0 jay        (501) staff       (20)     2123 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/icon_dsm_96.png
+-rw-r--r--   0 jay        (501) staff       (20)     2093 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/icon_tile.png
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.106330 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.107833 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.129622 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/
+-rw-r--r--   0 jay        (501) staff       (20)     1208 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/bt_dropdown.png
+-rw-r--r--   0 jay        (501) staff       (20)      455 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/bt_grid_dropdown.png
+-rw-r--r--   0 jay        (501) staff       (20)     4750 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/bt_pagebar.png
+-rw-r--r--   0 jay        (501) staff       (20)     8754 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/c_icon_general.png
+-rw-r--r--   0 jay        (501) staff       (20)      907 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/category_expand.png
+-rw-r--r--   0 jay        (501) staff       (20)     3535 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/checkbox.png
+-rw-r--r--   0 jay        (501) staff       (20)     1027 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/col-move-bottom.png
+-rw-r--r--   0 jay        (501) staff       (20)      343 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/date_dropdown.png
+-rw-r--r--   0 jay        (501) staff       (20)     1374 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/date_prev_next.png
+-rw-r--r--   0 jay        (501) staff       (20)      344 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/dropdown_menu_parent.png
+-rw-r--r--   0 jay        (501) staff       (20)      823 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/dropdown_menu_tick.png
+-rw-r--r--   0 jay        (501) staff       (20)     2729 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/fieldset_expand.png
+-rw-r--r--   0 jay        (501) staff       (20)     1975 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/icon_advanced_search.png
+-rw-r--r--   0 jay        (501) staff       (20)      644 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/icon_error.png
+-rw-r--r--   0 jay        (501) staff       (20)      372 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/icon_filter.png
+-rw-r--r--   0 jay        (501) staff       (20)     3373 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/icon_information.png
+-rw-r--r--   0 jay        (501) staff       (20)      491 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/icon_loading.gif
+-rw-r--r--   0 jay        (501) staff       (20)      842 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/icon_search.png
+-rw-r--r--   0 jay        (501) staff       (20)     6219 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/icon_search_clear.png
+-rw-r--r--   0 jay        (501) staff       (20)      972 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/icon_success.png
+-rw-r--r--   0 jay        (501) staff       (20)     4979 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/radio_button.png
+-rw-r--r--   0 jay        (501) staff       (20)      137 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/shadow_category.png
+-rw-r--r--   0 jay        (501) staff       (20)      138 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/shadow_footbar.png
+-rw-r--r--   0 jay        (501) staff       (20)     1649 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/superbox_button_cancel.png
+-rw-r--r--   0 jay        (501) staff       (20)      501 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/tab_arrow.png
+-rw-r--r--   0 jay        (501) staff       (20)     1065 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/tab_shadow.png
+-rw-r--r--   0 jay        (501) staff       (20)      372 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/tree_arrow.png
+-rw-r--r--   0 jay        (501) staff       (20)      517 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/trigger.png
+-rw-r--r--   0 jay        (501) staff       (20)      472 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/trigger_date.png
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.106976 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.106868 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.106575 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/ExternalDevices/
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.129780 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/ExternalDevices/images/
+-rw-r--r--   0 jay        (501) staff       (20)     4156 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/ExternalDevices/images/tray_icon_device.png
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.106684 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/FileTaskMonitor/
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.130740 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/FileTaskMonitor/images/
+-rw-r--r--   0 jay        (501) staff       (20)     5812 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/FileTaskMonitor/images/tray_icon_bgtask.gif
+-rw-r--r--   0 jay        (501) staff       (20)      928 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/FileTaskMonitor/images/tray_icon_bgtask.png
+-rw-r--r--   0 jay        (501) staff       (20)     6810 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/FileTaskMonitor/images/tray_icon_download.gif
+-rw-r--r--   0 jay        (501) staff       (20)     1192 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/FileTaskMonitor/images/tray_icon_download.png
+-rw-r--r--   0 jay        (501) staff       (20)     6658 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/FileTaskMonitor/images/tray_icon_upload.gif
+-rw-r--r--   0 jay        (501) staff       (20)     1129 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/FileTaskMonitor/images/tray_icon_upload.png
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.106791 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/PollingTask/
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.130886 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/PollingTask/images/
+-rw-r--r--   0 jay        (501) staff       (20)     5685 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/PollingTask/images/tray_icon_disk_port.png
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.106910 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/ThumbConvertProgress/
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.131229 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/ThumbConvertProgress/images/
+-rw-r--r--   0 jay        (501) staff       (20)     3073 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/ThumbConvertProgress/images/tray_icon_creating_thumbnail.gif
+-rw-r--r--   0 jay        (501) staff       (20)     2125 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/ThumbConvertProgress/images/tray_icon_creating_thumbnail.png
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.107016 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.133796 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/
+-rw-r--r--   0 jay        (501) staff       (20)    35658 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/bt_bugs.png
+-rw-r--r--   0 jay        (501) staff       (20)    27469 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/bt_dsm_mobile.png
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.134981 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/components/
+-rw-r--r--   0 jay        (501) staff       (20)     2031 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/components/icon_error.png
+-rw-r--r--   0 jay        (501) staff       (20)     1748 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/components/icon_image_selector.png
+-rw-r--r--   0 jay        (501) staff       (20)     1372 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/components/status_fail.png
+-rw-r--r--   0 jay        (501) staff       (20)     1549 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/components/status_loading.gif
+-rw-r--r--   0 jay        (501) staff       (20)     1322 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/components/status_success.png
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.135757 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/desktop/
+-rw-r--r--   0 jay        (501) staff       (20)     2537 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/desktop/add_one.png
+-rw-r--r--   0 jay        (501) staff       (20)     8458 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/desktop/icon_app_category.png
+-rw-r--r--   0 jay        (501) staff       (20)    11321 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/desktop/spotlight.png
+-rw-r--r--   0 jay        (501) staff       (20)     2164 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/desktop/taskbar_spinner.gif
+-rw-r--r--   0 jay        (501) staff       (20)    36970 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/dsm5_badge_num.png
+-rw-r--r--   0 jay        (501) staff       (20)    21353 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/dsm5_notification_num.png
+-rw-r--r--   0 jay        (501) staff       (20)     9530 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/dsmv5_wizard_bkg_v_01.png
+-rw-r--r--   0 jay        (501) staff       (20)    63006 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/dsmv5_wizard_bkg_v_02.png
+-rw-r--r--   0 jay        (501) staff       (20)      590 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/folder.png
+-rw-r--r--   0 jay        (501) staff       (20)     2536 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/icon_drag_add.png
+-rw-r--r--   0 jay        (501) staff       (20)     2388 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/icon_drag_ban.png
+-rw-r--r--   0 jay        (501) staff       (20)     3630 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/icon_question.png
+-rw-r--r--   0 jay        (501) staff       (20)     1637 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/item_drag_status.png
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.136566 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.138381 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/
+-rw-r--r--   0 jay        (501) staff       (20)     1565 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/0.png
+-rw-r--r--   0 jay        (501) staff       (20)     1165 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/1.png
+-rw-r--r--   0 jay        (501) staff       (20)     1554 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/2.png
+-rw-r--r--   0 jay        (501) staff       (20)     1704 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/3.png
+-rw-r--r--   0 jay        (501) staff       (20)     1419 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/4.png
+-rw-r--r--   0 jay        (501) staff       (20)     1589 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/5dot.png
+-rw-r--r--   0 jay        (501) staff       (20)     2462 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/DSM.png
+-rw-r--r--   0 jay        (501) staff       (20)     1735 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/beta.png
+-rw-r--r--   0 jay        (501) staff       (20)     8323 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/copyright_2014.png
+-rw-r--r--   0 jay        (501) staff       (20)     8318 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/copyright_2015.png
+-rw-r--r--   0 jay        (501) staff       (20)     7719 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/synology.png
+-rw-r--r--   0 jay        (501) staff       (20)      698 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/icon_phone.png
+-rw-r--r--   0 jay        (501) staff       (20)     3913 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/icon_pw.png
+-rw-r--r--   0 jay        (501) staff       (20)     3730 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/icon_user.png
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.140237 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/
+-rw-r--r--   0 jay        (501) staff       (20)      834 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/0.png
+-rw-r--r--   0 jay        (501) staff       (20)      318 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/1.png
+-rw-r--r--   0 jay        (501) staff       (20)      780 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/2.png
+-rw-r--r--   0 jay        (501) staff       (20)      982 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/3.png
+-rw-r--r--   0 jay        (501) staff       (20)      680 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/4.png
+-rw-r--r--   0 jay        (501) staff       (20)      868 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/5dot.png
+-rw-r--r--   0 jay        (501) staff       (20)     2070 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/DSM.png
+-rw-r--r--   0 jay        (501) staff       (20)     1162 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/beta.png
+-rw-r--r--   0 jay        (501) staff       (20)     8323 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/copyright_2014.png
+-rw-r--r--   0 jay        (501) staff       (20)     8318 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/copyright_2015.png
+-rw-r--r--   0 jay        (501) staff       (20)     8469 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/synology.png
+-rw-r--r--   0 jay        (501) staff       (20)     6772 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/login_bkg_highlight_bottom.png
+-rw-r--r--   0 jay        (501) staff       (20)     8683 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/login_bkg_highlight_top.png
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.142806 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/
+-rw-r--r--   0 jay        (501) staff       (20)    23041 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_cloudy.png
+-rw-r--r--   0 jay        (501) staff       (20)    33681 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_cold.png
+-rw-r--r--   0 jay        (501) staff       (20)    10119 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_fog.png
+-rw-r--r--   0 jay        (501) staff       (20)    27277 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_hail.png
+-rw-r--r--   0 jay        (501) staff       (20)    16586 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_moon.png
+-rw-r--r--   0 jay        (501) staff       (20)    28148 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_moon_clouds.png
+-rw-r--r--   0 jay        (501) staff       (20)    28152 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_rain.png
+-rw-r--r--   0 jay        (501) staff       (20)    31584 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_snow.png
+-rw-r--r--   0 jay        (501) staff       (20)    21959 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_sun.png
+-rw-r--r--   0 jay        (501) staff       (20)    37181 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_sun_clouds.png
+-rw-r--r--   0 jay        (501) staff       (20)    27481 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_thunder.png
+-rw-r--r--   0 jay        (501) staff       (20)    37188 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_tornado.png
+-rw-r--r--   0 jay        (501) staff       (20)    22230 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_windy.png
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.156728 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/
+-rw-r--r--   0 jay        (501) staff       (20)     5229 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_CMS.png
+-rw-r--r--   0 jay        (501) staff       (20)     5973 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_backup.png
+-rw-r--r--   0 jay        (501) staff       (20)     3767 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_business.png
+-rw-r--r--   0 jay        (501) staff       (20)     5282 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_community.png
+-rw-r--r--   0 jay        (501) staff       (20)     7444 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_connect.png
+-rw-r--r--   0 jay        (501) staff       (20)     5907 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_contact.png
+-rw-r--r--   0 jay        (501) staff       (20)     4389 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_directory_service.png
+-rw-r--r--   0 jay        (501) staff       (20)     5446 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_dsm_apps.png
+-rw-r--r--   0 jay        (501) staff       (20)     4339 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_expansion.png
+-rw-r--r--   0 jay        (501) staff       (20)     4126 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_external_devices.png
+-rw-r--r--   0 jay        (501) staff       (20)     4867 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_file_services.png
+-rw-r--r--   0 jay        (501) staff       (20)     8754 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_general.png
+-rw-r--r--   0 jay        (501) staff       (20)     7877 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_groups.png
+-rw-r--r--   0 jay        (501) staff       (20)     5937 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_hardware_and_power.png
+-rw-r--r--   0 jay        (501) staff       (20)     6498 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_hdd_management.png
+-rw-r--r--   0 jay        (501) staff       (20)     4823 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_hot_spare.png
+-rw-r--r--   0 jay        (501) staff       (20)     8171 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_info_center.png
+-rw-r--r--   0 jay        (501) staff       (20)     4191 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_installed.png
+-rw-r--r--   0 jay        (501) staff       (20)     7993 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_iscsi_lun.png
+-rw-r--r--   0 jay        (501) staff       (20)    10534 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_iscsi_target.png
+-rw-r--r--   0 jay        (501) staff       (20)     8216 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_login_style.png
+-rw-r--r--   0 jay        (501) staff       (20)    10244 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_media_library.png
+-rw-r--r--   0 jay        (501) staff       (20)     5374 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_network.png
+-rw-r--r--   0 jay        (501) staff       (20)     5660 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_networkmap.png
+-rw-r--r--   0 jay        (501) staff       (20)     6352 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_notifications.png
+-rw-r--r--   0 jay        (501) staff       (20)     5299 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_overview.png
+-rw-r--r--   0 jay        (501) staff       (20)     8245 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_performance.png
+-rw-r--r--   0 jay        (501) staff       (20)     5136 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_portal.png
+-rw-r--r--   0 jay        (501) staff       (20)     4734 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_privilege.png
+-rw-r--r--   0 jay        (501) staff       (20)     6985 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_process.png
+-rw-r--r--   0 jay        (501) staff       (20)    10097 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_public_access.png
+-rw-r--r--   0 jay        (501) staff       (20)     7973 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_purchases.png
+-rw-r--r--   0 jay        (501) staff       (20)     6400 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_quickconnect.png
+-rw-r--r--   0 jay        (501) staff       (20)     3621 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_raid_group.png
+-rw-r--r--   0 jay        (501) staff       (20)     5128 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_recommend.png
+-rw-r--r--   0 jay        (501) staff       (20)     9903 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_region.png
+-rw-r--r--   0 jay        (501) staff       (20)     7168 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_security.png
+-rw-r--r--   0 jay        (501) staff       (20)     5473 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_shared_folders.png
+-rw-r--r--   0 jay        (501) staff       (20)    10382 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_speed.png
+-rw-r--r--   0 jay        (501) staff       (20)     5255 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_ssd_cache.png
+-rw-r--r--   0 jay        (501) staff       (20)     5349 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_syslog.png
+-rw-r--r--   0 jay        (501) staff       (20)     5984 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_task_scheduler.png
+-rw-r--r--   0 jay        (501) staff       (20)     4008 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_terminal_and_SNMP.png
+-rw-r--r--   0 jay        (501) staff       (20)     8440 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_update_and_reset.png
+-rw-r--r--   0 jay        (501) staff       (20)     5905 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_users.png
+-rw-r--r--   0 jay        (501) staff       (20)     9565 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_utilities.png
+-rw-r--r--   0 jay        (501) staff       (20)     8423 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_volume.png
+-rw-r--r--   0 jay        (501) staff       (20)     9096 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_web_server.png
+-rw-r--r--   0 jay        (501) staff       (20)     7619 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_wireless.png
+-rw-r--r--   0 jay        (501) staff       (20)     7805 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/rt_button.png
+-rw-r--r--   0 jay        (501) staff       (20)      138 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/shadow_footbar.png
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.161764 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/
+-rw-r--r--   0 jay        (501) staff       (20)     1915 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/more_apps.png
+-rw-r--r--   0 jay        (501) staff       (20)     1445 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/showdesktop.png
+-rw-r--r--   0 jay        (501) staff       (20)      159 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/taskbar_bg.png
+-rw-r--r--   0 jay        (501) staff       (20)     4445 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/taskbar_bt.png
+-rw-r--r--   0 jay        (501) staff       (20)    10062 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/taskbar_bt_apps.png
+-rw-r--r--   0 jay        (501) staff       (20)      506 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/taskbar_bt_widgets_shadow.png
+-rw-r--r--   0 jay        (501) staff       (20)      132 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/taskbar_shadow.png
+-rw-r--r--   0 jay        (501) staff       (20)      183 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/taskbar_split.png
+-rw-r--r--   0 jay        (501) staff       (20)     6147 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/tray_icon_notification.png
+-rw-r--r--   0 jay        (501) staff       (20)     6852 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/tray_icon_pilot_view.png
+-rw-r--r--   0 jay        (501) staff       (20)     7569 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/tray_icon_search.png
+-rw-r--r--   0 jay        (501) staff       (20)     5077 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/tray_icon_user_menu.png
+-rw-r--r--   0 jay        (501) staff       (20)    10337 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/tray_icon_widget.png
+-rw-r--r--   0 jay        (501) staff       (20)     3622 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/user_menu_about.png
+-rw-r--r--   0 jay        (501) staff       (20)     3876 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/user_menu_logout.png
+-rw-r--r--   0 jay        (501) staff       (20)     5337 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/user_menu_options.png
+-rw-r--r--   0 jay        (501) staff       (20)     4950 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/user_menu_restart.png
+-rw-r--r--   0 jay        (501) staff       (20)     5475 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/user_menu_shutdown.png
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.162011 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/widget_window/
+-rw-r--r--   0 jay        (501) staff       (20)     9577 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/widget_window/widget_rt_button.png
+-rw-r--r--   0 jay        (501) staff       (20)    50783 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/wizard_bkg_h.png
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.162757 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/scrollbar/
+-rw-r--r--   0 jay        (501) staff       (20)      134 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/scrollbar/scrollbar_black_h.png
+-rw-r--r--   0 jay        (501) staff       (20)      136 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/scrollbar/scrollbar_black_v.png
+-rw-r--r--   0 jay        (501) staff       (20)      135 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/scrollbar/scrollbar_white_h.png
+-rw-r--r--   0 jay        (501) staff       (20)      127 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/scrollbar/scrollbar_white_v.png
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.162944 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/js/
+-rw-r--r--   0 jay        (501) staff       (20)     1056 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/js/misc.js
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.108044 opencanary-0.9.0/opencanary/modules/data/httpproxy/
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.108093 opencanary-0.9.0/opencanary/modules/data/httpproxy/skin/
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.163170 opencanary-0.9.0/opencanary/modules/data/httpproxy/skin/squid/
+-rw-r--r--   0 jay        (501) staff       (20)     2899 2023-05-18 06:56:45.000000 opencanary-0.9.0/opencanary/modules/data/httpproxy/skin/squid/auth.html
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.173989 opencanary-0.9.0/opencanary/modules/data/rdp/
+-rw-r--r--   0 jay        (501) staff       (20)  2088348 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/rdp/default.rss
+-rw-r--r--   0 jay        (501) staff       (20)   302478 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/rdp/login-failed.rss
+-rw-r--r--   0 jay        (501) staff       (20)  1459822 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/rdp/login-passreset.rss
+-rw-r--r--   0 jay        (501) staff       (20)   262442 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/data/rdp/login.rss
+-rw-r--r--   0 jay        (501) staff       (20)    32259 2023-02-21 19:54:37.000000 opencanary-0.9.0/opencanary/modules/des.py
+-rw-r--r--   0 jay        (501) staff       (20)     1430 2023-02-21 19:54:37.000000 opencanary-0.9.0/opencanary/modules/example0.py
+-rw-r--r--   0 jay        (501) staff       (20)     2225 2023-02-21 19:54:37.000000 opencanary-0.9.0/opencanary/modules/example1.py
+-rw-r--r--   0 jay        (501) staff       (20)     3095 2020-05-11 08:35:29.000000 opencanary-0.9.0/opencanary/modules/ftp.py
+-rw-r--r--   0 jay        (501) staff       (20)     2518 2022-06-30 07:24:28.000000 opencanary-0.9.0/opencanary/modules/git.py
+-rw-r--r--   0 jay        (501) staff       (20)     6375 2021-01-04 06:54:19.000000 opencanary-0.9.0/opencanary/modules/http.py
+-rw-r--r--   0 jay        (501) staff       (20)     5606 2021-09-15 19:16:59.000000 opencanary-0.9.0/opencanary/modules/httpproxy.py
+-rw-r--r--   0 jay        (501) staff       (20)     5073 2023-05-18 06:56:45.000000 opencanary-0.9.0/opencanary/modules/https.py
+-rw-r--r--   0 jay        (501) staff       (20)    15416 2023-02-21 19:54:37.000000 opencanary-0.9.0/opencanary/modules/mssql.py
+-rw-r--r--   0 jay        (501) staff       (20)     6198 2023-05-18 06:56:45.000000 opencanary-0.9.0/opencanary/modules/mysql.py
+-rw-r--r--   0 jay        (501) staff       (20)     1615 2021-09-14 05:01:16.000000 opencanary-0.9.0/opencanary/modules/ntp.py
+-rw-r--r--   0 jay        (501) staff       (20)     7646 2023-05-18 06:56:45.000000 opencanary-0.9.0/opencanary/modules/portscan.py
+-rw-r--r--   0 jay        (501) staff       (20)     1847 2023-05-19 11:08:10.000000 opencanary-0.9.0/opencanary/modules/rdp.py
+-rw-r--r--   0 jay        (501) staff       (20)    13263 2023-02-21 19:54:37.000000 opencanary-0.9.0/opencanary/modules/redis.py
+-rw-r--r--   0 jay        (501) staff       (20)     2774 2022-03-01 06:51:14.000000 opencanary-0.9.0/opencanary/modules/samba.py
+-rw-r--r--   0 jay        (501) staff       (20)     1183 2020-05-11 08:35:29.000000 opencanary-0.9.0/opencanary/modules/sip.py
+-rw-r--r--   0 jay        (501) staff       (20)     1364 2020-05-11 08:35:29.000000 opencanary-0.9.0/opencanary/modules/snmp.py
+-rw-r--r--   0 jay        (501) staff       (20)    15123 2022-07-27 09:44:18.000000 opencanary-0.9.0/opencanary/modules/ssh.py
+-rw-r--r--   0 jay        (501) staff       (20)     8028 2023-05-19 11:08:10.000000 opencanary-0.9.0/opencanary/modules/tcpbanner.py
+-rw-r--r--   0 jay        (501) staff       (20)     2909 2020-05-11 08:35:29.000000 opencanary-0.9.0/opencanary/modules/telnet.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.108307 opencanary-0.9.0/opencanary/modules/test/
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.175013 opencanary-0.9.0/opencanary/modules/test/ftp/
+-rw-r--r--   0 jay        (501) staff       (20)     3095 2019-09-03 20:24:40.000000 opencanary-0.9.0/opencanary/modules/test/ftp/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)     1608 2019-09-04 19:59:07.000000 opencanary-0.9.0/opencanary/modules/test/ftp/test_ftp.py
+-rw-r--r--   0 jay        (501) staff       (20)        0 2019-09-03 20:04:12.000000 opencanary-0.9.0/opencanary/modules/test.py
+-rw-r--r--   0 jay        (501) staff       (20)     3215 2018-06-14 14:00:23.000000 opencanary-0.9.0/opencanary/modules/testpdf.py
+-rw-r--r--   0 jay        (501) staff       (20)     1527 2020-05-11 08:35:29.000000 opencanary-0.9.0/opencanary/modules/tftp.py
+-rw-r--r--   0 jay        (501) staff       (20)     4851 2023-02-21 19:54:37.000000 opencanary-0.9.0/opencanary/modules/vnc.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-05-23 12:36:08.113236 opencanary-0.9.0/opencanary.egg-info/
+-rw-r--r--   0 jay        (501) staff       (20)      988 2023-05-23 12:36:08.000000 opencanary-0.9.0/opencanary.egg-info/PKG-INFO
+-rw-r--r--   0 jay        (501) staff       (20)    23905 2023-05-23 12:36:08.000000 opencanary-0.9.0/opencanary.egg-info/SOURCES.txt
+-rw-r--r--   0 jay        (501) staff       (20)        1 2023-05-23 12:36:08.000000 opencanary-0.9.0/opencanary.egg-info/dependency_links.txt
+-rw-r--r--   0 jay        (501) staff       (20)      270 2023-05-23 12:36:08.000000 opencanary-0.9.0/opencanary.egg-info/requires.txt
+-rw-r--r--   0 jay        (501) staff       (20)       57 2023-05-23 12:36:08.000000 opencanary-0.9.0/opencanary.egg-info/top_level.txt
+-rw-r--r--   0 jay        (501) staff       (20)      288 2021-08-26 09:15:18.000000 opencanary-0.9.0/opencanary.service
+-rw-r--r--   0 jay        (501) staff       (20)        5 2018-06-14 14:00:23.000000 opencanary-0.9.0/requirements.txt
+-rw-r--r--   0 jay        (501) staff       (20)      391 2021-05-26 06:15:33.000000 opencanary-0.9.0/run.sh
+-rw-r--r--   0 jay        (501) staff       (20)       38 2023-05-23 12:36:08.175573 opencanary-0.9.0/setup.cfg
+-rw-r--r--   0 jay        (501) staff       (20)     2414 2023-05-23 10:23:15.000000 opencanary-0.9.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `opencanary-0.7.1/LICENSE` & `opencanary-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/PKG-INFO` & `opencanary-0.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: opencanary
-Version: 0.7.1
+Version: 0.9.0
 Summary: OpenCanary daemon
 Home-page: http://www.thinkst.com/
 Author: Thinkst Applied Research
 Author-email: info@thinkst.com
 License: BSD
-Description: A low interaction honeypot intended to be run on internal networks.
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: Twisted
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Networking :: Monitoring
 Classifier: Natural Language :: English
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: POSIX :: BSD :: FreeBSD
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: BSD License
+License-File: LICENSE
+
+A low interaction honeypot intended to be run on internal networks.
```

### Comparing `opencanary-0.7.1/README.md` & `opencanary-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 * Receive email alerts as soon as potential threats are detected, highlighting the threat source IP address and where the breach may have taken place.
 
 Prerequisites
 ----------------
 
 * Python 2.7, 3.7 (Recommended Python 3.7+)
 * [Optional] SNMP requires the Python library scapy
-* ~[Optional] RDP requires the Python library rdpy~ (this module has been removed; we are currently determining a way forward with this.)
 * [Optional] Samba module needs a working installation of samba
 
 Installation [UBUNTU]
 ----------
 
 For updated and cleaner documentation, please head over to http://opencanary.org
 
@@ -102,21 +101,21 @@
 
 On the first run, instructions are printed that will get to a working config.
 
 ```
 $ opencanaryd --copyconfig
 ```
 
-Which will create a folder, `/etc/opencanary` and a config file inside that folder `opencanary.conf`. You must now edit the config file to determine which services and logging options you would like to enable.
+Which will create a folder, `/etc/opencanaryd` and a config file inside that folder `opencanary.conf`. You must now edit the config file to determine which services and logging options you would like to enable.
 
 When OpenCanary starts it looks for config files in the following order:
 
 1. ./opencanary.conf (i.e. the directory where OpenCanary is installed)
 2. ~/.opencanary.conf (i.e. the home directory of the user, usually this will be root so /root/.opencanary.conf)
-3. /etc/opencanary/opencanary.conf
+3. /etc/opencanaryd/opencanary.conf
 
 It will use the first config file that exists.
 
 Samba Setup (optional)
 ----------------------
 This is required for the `smb` module.
```

### Comparing `opencanary-0.7.1/bin/opencanary.tac` & `opencanary-0.9.0/bin/opencanary.tac`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,62 @@
 import traceback
-
+# import warnings
+# warnings.filterwarnings("ignore", category=DeprecationWarning)
+def warn(*args, **kwargs):
+    pass
+import warnings
+warnings.warn = warn
 from twisted.application import service
 from twisted.application import internet
 from twisted.internet.protocol import Factory
 from pkg_resources import iter_entry_points
 
 from opencanary.config import config
 from opencanary.logger import getLogger
 from opencanary.modules.http import CanaryHTTP
+from opencanary.modules.https import CanaryHTTPS
 from opencanary.modules.ftp import CanaryFTP
 from opencanary.modules.ssh import CanarySSH
 from opencanary.modules.telnet import Telnet
 from opencanary.modules.httpproxy import HTTPProxy
 from opencanary.modules.mysql import CanaryMySQL
 from opencanary.modules.mssql import MSSQL
 from opencanary.modules.ntp import CanaryNtp
 from opencanary.modules.tftp import CanaryTftp
 from opencanary.modules.vnc import CanaryVNC
 from opencanary.modules.sip import CanarySIP
 from opencanary.modules.git import CanaryGit
 from opencanary.modules.redis import CanaryRedis
 from opencanary.modules.tcpbanner import CanaryTCPBanner
+from opencanary.modules.rdp import CanaryRDP
 
 #from opencanary.modules.example0 import CanaryExample0
 #from opencanary.modules.example1 import CanaryExample1
 
 ENTRYPOINT = "canary.usermodule"
-MODULES = [Telnet, CanaryHTTP, CanaryFTP, CanarySSH, HTTPProxy, CanaryMySQL,
-           MSSQL, CanaryVNC, CanaryTftp, CanaryNtp, CanarySIP, CanaryGit,
-           CanaryTCPBanner, CanaryRedis]
-           #CanaryExample0, CanaryExample1]
-
-if config.moduleEnabled('rdp'):
-    try:
-        #Module needs RDP, but the rest of OpenCanary doesn't
-        from opencanary.modules.rdp import CanaryRDP
-        MODULES.append(CanaryRDP)
-    except ImportError:
-        print("Can't import RDP. Please ensure you have RDP installed.")
-        pass
+MODULES = [
+    CanaryFTP,
+    CanaryGit,
+    CanaryHTTP,
+    CanaryHTTPS,
+    CanaryMySQL,
+    CanaryNtp,
+    CanaryRDP,
+    CanaryRedis,
+    CanarySIP,
+    CanarySSH,
+    CanaryTCPBanner,
+    CanaryTftp,
+    CanaryVNC,
+    HTTPProxy,
+    MSSQL,
+    Telnet,
+    # CanaryExample0,
+    # CanaryExample1,
+]
 
 if config.moduleEnabled('snmp'):
     try:
         #Module need Scapy, but the rest of OpenCanary doesn't
         from opencanary.modules.snmp import CanarySNMP
         MODULES.append(CanarySNMP)
     except ImportError:
```

### Comparing `opencanary-0.7.1/bin/opencanaryd` & `opencanary-0.9.0/bin/opencanaryd`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 }
 
 if [ "${cmd}" == "--start" ]; then
     sudo -E "${DIR}/twistd" -y "${DIR}/opencanary.tac" --pidfile "${PIDFILE}" --syslog --prefix=opencanaryd
 elif [ "${cmd}" == "--dev" ]; then
     sudo -E "${DIR}/twistd" -noy "${DIR}/opencanary.tac"
 elif [ "${cmd}" == "--usermodule" ]; then
-  usermodconf=$(python -c "from __future__ import print_function; from pkg_resources import resource_filename; print(resource_filename('opencanary', 'data/settings-usermodule.json'))")
+  usermodconf=$(python -c "from pkg_resources import resource_filename; print(resource_filename('opencanary', 'data/settings-usermodule.json'))")
 
   if [ -f opencanary.conf ]; then
     if ! diff -q opencanary.conf "${usermodconf}" 2>&1 >/dev/null; then
       echo "Backing up old config to ./opencanary.conf.old"
       cp opencanary.conf{,.old}
     fi
   fi
@@ -53,19 +53,15 @@
     pid=`sudo -E cat "${PIDFILE}"`
     sudo -E kill "$pid"
 elif [ "${cmd}" == "--copyconfig" ]; then
     if [ -f /etc/opencanaryd/opencanary.conf ]; then
         echo "A config file already exists at /etc/opencanaryd/opencanary.conf, please move it first"
         exit 1
     fi
-    if [[ -f `which python` ]] ; then
-        defaultconf=$(python -c "from __future__ import print_function; from pkg_resources import resource_filename; print(resource_filename('opencanary', 'data/settings.json'))")
-    else
-        defaultconf=$(python3 -c "from pkg_resources import resource_filename; print(resource_filename('opencanary', 'data/settings.json'))")
-    fi
+    defaultconf=$(python3 -c "from pkg_resources import resource_filename; print(resource_filename('opencanary', 'data/settings.json'))")
     sudo -E mkdir -p /etc/opencanaryd
     sudo -E cp "${defaultconf}" /etc/opencanaryd/opencanary.conf
     echo -e "[*] A sample config file is ready /etc/opencanaryd/opencanary.conf\n"
     echo    "[*] Edit your configuration, then launch with \"opencanaryd --start\""
 elif [ "${cmd}" == "--version" ]; then
     python -c "from opencanary import __version__; print(__version__);"
 else
```

### Comparing `opencanary-0.7.1/data/.opencanary.conf` & `opencanary-0.9.0/data/.opencanary.conf`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'https.certificate'": "'/etc/ssl/opencanary/opencanary.pem'",*

 * * "'https.enabled'": 'True',*

 * * "'https.key'": "'/etc/ssl/opencanary/opencanary.key'",*

 * * "'https.port'": '443',*

 * * "'https.skin'": "'nasLogin'"}*

```diff
@@ -28,14 +28,19 @@
             "name": "squid"
         },
         {
             "desc": "Microsoft ISA Server Web Proxy",
             "name": "ms-isa"
         }
     ],
+    "https.certificate": "/etc/ssl/opencanary/opencanary.pem",
+    "https.enabled": true,
+    "https.key": "/etc/ssl/opencanary/opencanary.key",
+    "https.port": 443,
+    "https.skin": "nasLogin",
     "ip.ignorelist": [],
     "logger": {
         "class": "PyLogger",
         "kwargs": {
             "formatters": {
                 "plain": {
                     "format": "%(message)s"
```

### Comparing `opencanary-0.7.1/opencanary/config.py` & `opencanary-0.9.0/opencanary/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,15 @@
-from __future__ import print_function
 from six import iteritems
 import os, sys, json, copy, socket, itertools, string, subprocess
 from os.path import expanduser
 from pkg_resources import resource_filename
 
 SAMPLE_SETTINGS = resource_filename(__name__, 'data/settings.json')
 SETTINGS = 'opencanary.conf'
 
-PY3 = sys.version_info > (3,)
-
-# Only check unicode on Python 2, In Python 3 unicode is the default and we can just return the input.
-if sys.version_info[0] < 3:
-    def byteify(input):
-        if isinstance(input, dict):
-            return {byteify(key): byteify(value)
-                    for key, value in iteritems(input)}
-        elif isinstance(input, list):
-            return [byteify(element) for element in input]
-        elif isinstance(input, unicode):
-                return input.encode('utf-8')
-        else:
-            return input
-else:
-    def byteify(input):
-        return input
-
 
 def expand_vars(var):
     """Recursively replace environment variables in a dictionary, list or string with their respective values."""
     if isinstance(var, dict):
         for key, value in var.items():
             var[key] = expand_vars(value)
         return var
@@ -47,24 +28,23 @@
         files = [configfile, "%s/.%s" % (expanduser("~"), configfile), "/etc/opencanaryd/%s"%configfile]
         print("** We hope you enjoy using OpenCanary. For more open source Canary goodness, head over to canarytokens.org. **")
         for fname in files:
             try:
                 with open(fname, "r") as f:
                     print("[-] Using config file: %s" % fname)
                     self.__config = json.load(f)
-                    self.__config = byteify(self.__config)
                     self.__config = expand_vars(self.__config)
                 return
             except IOError as e:
                 print("[-] Failed to open %s for reading (%s)" % (fname, e))
             except ValueError as e:
                 print("[-] Failed to decode json from %s (%s)" % (fname, e))
                 subprocess.call("cp -r %s /var/tmp/config-err-$(date +%%s)" % fname, shell=True)
             except Exception as e:
-                print("[-] An error occured loading %s (%s)" % (fname, e))
+                print("[-] An error occurred loading %s (%s)" % (fname, e))
         if self.__config is None:
             print('No config file found. Please create one with "opencanaryd --copyconfig"')
             sys.exit(1)
 
     def moduleEnabled(self, module_name):
         k = "%s.enabled" % module_name.lower()
         if k in self.__config:
@@ -136,15 +116,15 @@
         self.__config.update(params)
         return errors
 
     def setVal(self, key, val):
         """Set value only if valid otherwise throw exception"""
         errs = self.setValues({key: val})
 
-        # sucessful update
+        # successful update
         if not errs:
             return
 
         # raise first error reported on the update key
         for e in errs:
             if e.key == key:
                 raise e
```

### Comparing `opencanary-0.7.1/opencanary/data/settings.json` & `opencanary-0.9.0/opencanary/data/settings.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9264705882352942%*

 * *Differences: {"'https.certificate'": "'/etc/ssl/opencanary/opencanary.pem'",*

 * * "'https.enabled'": 'False',*

 * * "'https.key'": "'/etc/ssl/opencanary/opencanary.key'",*

 * * "'https.port'": '443',*

 * * "'https.skin'": "'nasLogin'"}*

```diff
@@ -8,14 +8,19 @@
     "http.banner": "Apache/2.2.22 (Ubuntu)",
     "http.enabled": false,
     "http.port": 80,
     "http.skin": "nasLogin",
     "httpproxy.enabled": false,
     "httpproxy.port": 8080,
     "httpproxy.skin": "squid",
+    "https.certificate": "/etc/ssl/opencanary/opencanary.pem",
+    "https.enabled": false,
+    "https.key": "/etc/ssl/opencanary/opencanary.key",
+    "https.port": 443,
+    "https.skin": "nasLogin",
     "ip.ignorelist": [],
     "logger": {
         "class": "PyLogger",
         "kwargs": {
             "formatters": {
                 "plain": {
                     "format": "%(message)s"
```

### Comparing `opencanary-0.7.1/opencanary/honeycred.py` & `opencanary-0.9.0/opencanary/honeycred.py`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/iphelper.py` & `opencanary-0.9.0/opencanary/iphelper.py`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/logger.py` & `opencanary-0.9.0/opencanary/logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import print_function
+from copy import deepcopy
 import simplejson as json
 import logging.config
 import socket
 import hpfeeds
 import sys
 
 from datetime import datetime
@@ -39,15 +39,15 @@
     kwargs = d.get('kwargs', None)
     if kwargs is None:
         print("Logger section is missing the kwargs key.", file=sys.stderr)
         exit(1)
     try:
         logger = LoggerClass(config, **kwargs)
     except Exception as e:
-        print("An error occured initialising the logger class", file=sys.stderr)
+        print("An error occurred initialising the logger class", file=sys.stderr)
         print(e)
         exit(1)
 
     return logger
 
 class LoggerBase(object):
     LOG_BASE_BOOT                               = 1000
@@ -331,16 +331,20 @@
             if any(e in message for e in self.ignore):
                 return
 
         mapping = {"message": message}
         if self.data is None:
             data = mapping
         else:
-            # Due to the recursive function, sending a shallow copy of self.data here is fine.
-            data = map_string(dict(self.data), mapping)
+            if isinstance(self.data, dict):
+                # Casting logging.config.ConvertingDict to a standard dict
+                data = dict(self.data)
+            else:
+                data = self.data
+            data = map_string(deepcopy(data), mapping)
 
         if "application/json" in self.kwargs.get("headers", {}).values():
             response = requests.request(method=self.method, url=self.url, json=data, **self.kwargs)
         else:
             response = requests.request(method=self.method, url=self.url, data=data, **self.kwargs)
 
         if response.status_code != self.status_code:
```

### Comparing `opencanary-0.7.1/opencanary/modules/__init__.py` & `opencanary-0.9.0/opencanary/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/basicLogin/index.html` & `opencanary-0.9.0/opencanary/modules/data/http/skin/basicLogin/index.html`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/index.html` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/index.html`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/css/desktop.css` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/css/desktop.css`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/css/ext-all.css` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/css/ext-all.css`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/css/style.css` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/css/style.css`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/css/ux-all.css` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/css/ux-all.css`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/css/xtheme-gray.css` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/css/xtheme-gray.css`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/fonts/roboto.woff` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/fonts/roboto.woff`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/02.jpg` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/02.jpg`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/favicon.ico` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/icon_dsm_16.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/icon_dsm_16.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/icon_dsm_32.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/icon_dsm_32.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/icon_dsm_48.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/icon_dsm_48.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/icon_dsm_64.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/icon_dsm_64.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/icon_dsm_96.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/icon_dsm_96.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/icon_tile.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/icon_tile.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/bt_dropdown.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/bt_dropdown.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/bt_pagebar.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/bt_pagebar.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/c_icon_general.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/c_icon_general.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/category_expand.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/category_expand.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/checkbox.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/checkbox.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/col-move-bottom.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/col-move-bottom.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/date_prev_next.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/date_prev_next.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/dropdown_menu_tick.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/dropdown_menu_tick.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/fieldset_expand.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/fieldset_expand.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/icon_advanced_search.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/icon_advanced_search.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/icon_error.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/icon_error.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/icon_information.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/icon_information.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/icon_search.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/icon_search.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/icon_search_clear.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/icon_search_clear.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/icon_success.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/icon_success.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/radio_button.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/radio_button.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/superbox_button_cancel.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/superbox_button_cancel.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/tab_shadow.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/tab_shadow.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/trigger.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/Components/trigger.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/ExternalDevices/images/tray_icon_device.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/ExternalDevices/images/tray_icon_device.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/FileTaskMonitor/images/tray_icon_bgtask.gif` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/FileTaskMonitor/images/tray_icon_bgtask.gif`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/FileTaskMonitor/images/tray_icon_bgtask.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/FileTaskMonitor/images/tray_icon_bgtask.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/FileTaskMonitor/images/tray_icon_download.gif` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/FileTaskMonitor/images/tray_icon_download.gif`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/FileTaskMonitor/images/tray_icon_download.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/FileTaskMonitor/images/tray_icon_download.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/FileTaskMonitor/images/tray_icon_upload.gif` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/FileTaskMonitor/images/tray_icon_upload.gif`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/FileTaskMonitor/images/tray_icon_upload.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/FileTaskMonitor/images/tray_icon_upload.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/PollingTask/images/tray_icon_disk_port.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/PollingTask/images/tray_icon_disk_port.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/ThumbConvertProgress/images/tray_icon_creating_thumbnail.gif` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/ThumbConvertProgress/images/tray_icon_creating_thumbnail.gif`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/ThumbConvertProgress/images/tray_icon_creating_thumbnail.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/modules/ThumbConvertProgress/images/tray_icon_creating_thumbnail.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/bt_bugs.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/bt_bugs.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/bt_dsm_mobile.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/bt_dsm_mobile.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/components/icon_error.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/components/icon_error.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/components/icon_image_selector.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/components/icon_image_selector.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/components/status_fail.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/components/status_fail.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/components/status_loading.gif` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/components/status_loading.gif`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/components/status_success.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/components/status_success.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/desktop/add_one.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/desktop/add_one.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/desktop/icon_app_category.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/desktop/icon_app_category.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/desktop/spotlight.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/desktop/spotlight.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/desktop/taskbar_spinner.gif` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/desktop/taskbar_spinner.gif`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/dsm5_badge_num.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/dsm5_badge_num.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/dsm5_notification_num.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/dsm5_notification_num.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/dsmv5_wizard_bkg_v_01.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/dsmv5_wizard_bkg_v_01.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/dsmv5_wizard_bkg_v_02.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/dsmv5_wizard_bkg_v_02.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/folder.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/folder.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/icon_drag_add.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/icon_drag_add.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/icon_drag_ban.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/icon_drag_ban.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/icon_question.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/icon_question.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/item_drag_status.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/item_drag_status.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/0.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/0.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/1.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/1.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/2.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/2.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/3.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/3.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/4.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/4.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/5dot.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/5dot.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/DSM.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/DSM.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/beta.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/beta.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/copyright_2014.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/copyright_2014.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/copyright_2015.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/copyright_2015.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/synology.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/dark/synology.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/icon_phone.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/icon_phone.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/icon_pw.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/icon_pw.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/icon_user.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/icon_user.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/0.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/0.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/2.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/2.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/3.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/3.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/4.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/4.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/5dot.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/5dot.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/DSM.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/DSM.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/beta.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/beta.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/copyright_2014.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/copyright_2014.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/copyright_2015.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/copyright_2015.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/synology.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/light/synology.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/login_bkg_highlight_bottom.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/login_bkg_highlight_bottom.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/login_bkg_highlight_top.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/login_bkg_highlight_top.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_cloudy.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_cloudy.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_cold.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_cold.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_fog.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_fog.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_hail.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_hail.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_moon.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_moon.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_moon_clouds.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_moon_clouds.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_rain.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_rain.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_snow.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_snow.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_sun.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_sun.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_sun_clouds.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_sun_clouds.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_thunder.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_thunder.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_tornado.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_tornado.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_windy.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/login/weather/login_icon_weather_windy.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_CMS.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_CMS.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_backup.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_backup.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_business.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_business.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_community.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_community.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_connect.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_connect.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_contact.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_contact.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_directory_service.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_directory_service.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_dsm_apps.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_dsm_apps.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_expansion.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_expansion.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_external_devices.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_external_devices.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_file_services.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_file_services.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_general.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_general.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_groups.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_groups.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_hardware_and_power.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_hardware_and_power.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_hdd_management.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_hdd_management.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_hot_spare.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_hot_spare.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_info_center.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_info_center.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_installed.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_installed.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_iscsi_lun.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_iscsi_lun.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_iscsi_target.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_iscsi_target.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_login_style.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_login_style.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_media_library.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_media_library.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_network.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_network.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_networkmap.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_networkmap.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_notifications.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_notifications.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_overview.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_overview.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_performance.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_performance.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_portal.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_portal.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_privilege.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_privilege.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_process.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_process.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_public_access.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_public_access.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_purchases.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_purchases.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_quickconnect.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_quickconnect.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_raid_group.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_raid_group.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_recommend.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_recommend.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_region.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_region.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_security.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_security.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_shared_folders.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_shared_folders.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_speed.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_speed.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_ssd_cache.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_ssd_cache.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_syslog.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_syslog.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_task_scheduler.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_task_scheduler.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_terminal_and_SNMP.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_terminal_and_SNMP.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_update_and_reset.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_update_and_reset.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_users.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_users.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_utilities.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_utilities.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_volume.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_volume.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_web_server.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_web_server.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_wireless.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/module_list_icon/c_icon_wireless.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/rt_button.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/rt_button.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/more_apps.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/more_apps.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/showdesktop.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/showdesktop.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/taskbar_bt.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/taskbar_bt.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/taskbar_bt_apps.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/taskbar_bt_apps.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/tray_icon_notification.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/tray_icon_notification.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/tray_icon_pilot_view.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/tray_icon_pilot_view.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/tray_icon_search.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/tray_icon_search.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/tray_icon_user_menu.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/tray_icon_user_menu.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/tray_icon_widget.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/tray_icon_widget.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/user_menu_about.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/user_menu_about.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/user_menu_logout.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/user_menu_logout.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/user_menu_options.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/user_menu_options.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/user_menu_restart.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/user_menu_restart.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/user_menu_shutdown.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/taskbar/user_menu_shutdown.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/widget_window/widget_rt_button.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/widget_window/widget_rt_button.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/wizard_bkg_h.png` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/dsm/resources/images/wizard_bkg_h.png`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/http/skin/nasLogin/static/js/misc.js` & `opencanary-0.9.0/opencanary/modules/data/http/skin/nasLogin/static/js/misc.js`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/httpproxy/skin/squid/auth.html` & `opencanary-0.9.0/opencanary/modules/data/httpproxy/skin/squid/auth.html`

 * *Files 0% similar despite different names*

```diff
@@ -130,7 +130,8 @@
 
 <hr> 
 <div id="footer">
 <p>Generated {{ date }} by localhost (squid/3.3.8)</p>
 <!-- ERR_CACHE_ACCESS_DENIED -->
 </div>
 </body></html>
+
```

### Comparing `opencanary-0.7.1/opencanary/modules/data/rdp/default.rss` & `opencanary-0.9.0/opencanary/modules/data/rdp/default.rss`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/rdp/login-failed.rss` & `opencanary-0.9.0/opencanary/modules/data/rdp/login-failed.rss`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/rdp/login-passreset.rss` & `opencanary-0.9.0/opencanary/modules/data/rdp/login-passreset.rss`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/data/rdp/login.rss` & `opencanary-0.9.0/opencanary/modules/data/rdp/login.rss`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/des.py` & `opencanary-0.9.0/opencanary/modules/des.py`

 * *Files 0% similar despite different names*

```diff
@@ -578,15 +578,15 @@
 
         if self.getMode() == CBC:
             if self.getIV():
                 iv = self.__String_to_BitList(self.getIV())
             else:
                 raise ValueError("For CBC mode, you must supply the Initial Value (IV) for ciphering")
 
-        # Split the data into blocks, crypting each one seperately
+        # Split the data into blocks, crypting each one separately
         i = 0
         dict = {}
         result = []
         #cached = 0
         #lines = 0
         while i < len(data):
             # Test code for caching encryption results
```

### Comparing `opencanary-0.7.1/opencanary/modules/example0.py` & `opencanary-0.9.0/opencanary/modules/example0.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     def connectionMade(self):
         self.transport.write("Welcome!\r\npassword: ")
         self.prompts += 1
 
     def dataReceived(self, data):
         """
-        Careful, data recieved here is unbuffered. See example1
+        Careful, data received here is unbuffered. See example1
         for how this can be better handled.
         """
         password = data.strip("\r\n")
         logdata = {"PASSWORD" : password}
         self.factory.log(logdata, transport=self.transport)
         
         if self.prompts < 3:
```

### Comparing `opencanary-0.7.1/opencanary/modules/example1.py` & `opencanary-0.9.0/opencanary/modules/example1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from opencanary.modules import CanaryService
 
 from twisted.internet.protocol import Protocol
 from twisted.internet.protocol import Factory
 from twisted.application import internet
-from __future__ import print_function
 
 class Example1Protocol(Protocol):
     """
     Example Telnet Protocol
 
     $ telnet localhost 8025
     Trying 127.0.0.1...
@@ -35,18 +34,18 @@
 
     def connectionMade(self):
         self.transport.write("\xff\xfb\x03\xff\xfb\x01password: ")
         self.prompts += 1
 
     def dataReceived(self, data):
         """
-        Recieved data is unbuffered so we buffer it for telnet.
+        Received data is unbuffered so we buffer it for telnet.
         """
         self.buffer += data
-        print("Recieved data: ", repr(data))
+        print("Received data: ", repr(data))
 
         # Discard inital telnet client control chars
         i = self.buffer.find("\x01")
         if i >= 0:
             self.buffer = self.buffer[i+1:]
             return
```

### Comparing `opencanary-0.7.1/opencanary/modules/ftp.py` & `opencanary-0.9.0/opencanary/modules/ftp.py`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/git.py` & `opencanary-0.9.0/opencanary/modules/git.py`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/http.py` & `opencanary-0.9.0/opencanary/modules/http.py`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/httpproxy.py` & `opencanary-0.9.0/opencanary/modules/httpproxy.py`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/mssql.py` & `opencanary-0.9.0/opencanary/modules/mssql.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from __future__ import print_function
 from opencanary.modules import CanaryService
 from opencanary.config import ConfigException
 
 from twisted.protocols.policies import TimeoutMixin
 from twisted.internet.protocol import Protocol
 from twisted.internet.protocol import Factory
 from twisted.application import internet
@@ -201,15 +200,15 @@
             del header[2]
             if len(self._buffer) >= plen:
                 payload = self._buffer[hlen: plen]
                 self._buffer = self._buffer[plen:]
                 tds = TDSPacket._make(header  + [payload])
                 return tds
             else:
-                # Whole payload not yet recieved. Leave header in
+                # Whole payload not yet received. Leave header in
                 # buffer but return copy of header anyway
                 return TDSPacket._make(header + [None])
         except Exception as e:
             print(e)
 
         return None
```

### Comparing `opencanary-0.7.1/opencanary/modules/mysql.py` & `opencanary-0.9.0/opencanary/modules/mysql.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from opencanary.modules import CanaryService
-from opencanary.config import ConfigException, PY3
+from opencanary.config import ConfigException
 
 from twisted.protocols.policies import TimeoutMixin
 from twisted.internet.protocol import Protocol
 from twisted.internet.protocol import Factory
 from twisted.application import internet
 from random import randint
 
 import struct
 import re
+import string
+import random
 
 UINT_MAX = 0xFFFFFFFF
 
 class MySQL(Protocol, TimeoutMixin):
     HEADER_LEN              = 4
     ERR_CODE_ACCESS_DENIED  = 1045
     ERR_CODE_PKT_ORDER      = 1156
@@ -48,53 +50,48 @@
         offset = 4 + 4 + 1 + 23
         i = data.find(b"\x00", offset)
         if i < 0:
             return None, None
 
         username = data[offset:i]
         i += 1
-        if PY3:
-            plen = data[i]
-        else:
-            plen = struct.unpack('B', data[i])[0]
+        plen = data[i]
         i+=1
         if plen == 0:
             return username, None
-        if PY3:
-            password="".join("{:02x}".format(c) for c in data[i:i+plen])
-        else:
-            password="".join("{:02x}".format(ord(c)) for c in data[i:i+plen])
+        password="".join("{:02x}".format(c) for c in data[i:i+plen])
         return username, password
 
     def consume_packet(self):
         if len(self._buffer) < MySQL.HEADER_LEN:
             return None, None
         length = struct.unpack('<I', self._buffer[:3] + b'\x00')[0]
-        if PY3:
-            seq_id = self._buffer[3]
-        else:
-            seq_id = struct.unpack('<B', self._buffer[3])[0]
+        seq_id = self._buffer[3]
 
         # enough buffer data to consume packet?
         if len(self._buffer) < MySQL.HEADER_LEN + length:
             return seq_id, None
 
         payload = self._buffer[MySQL.HEADER_LEN: MySQL.HEADER_LEN + length]
 
         self._buffer = self._buffer[MySQL.HEADER_LEN + length:]
 
         return seq_id, payload
 
     def server_greeting(self):
-        # struct.pack returns a byte string for py2 and py3
+        # struct.pack returns a byte string
         _threadid = struct.pack('<I', self.threadid)
-        # TODO: randomize salts embedded here
-        data = b'\x0a' + self.factory.canaryservice.banner + b'\x00' + _threadid + b'\x25\x73\x36\x51\x74\x77\x75\x69\x00\xff\xf7\x08\x02\x00\x0f\x80\x15\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x2e\x47\x5c\x78\x67\x7a\x4f\x5b\x5c\x3e\x5c\x39\x00\x6d\x79\x73\x71\x6c\x5f\x6e\x61\x74\x69\x76\x65\x5f\x70\x61\x73\x73\x77\x6f\x72\x64\x00'
+        salt1, salt2 = self.gen_salt(8), self.gen_salt(12) 
+        data = b'\x0a' + self.factory.canaryservice.banner + b'\x00' + _threadid + salt1 + b'\x00\xff\xf7\x08\x02\x00\x0f\x80\x15\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00' + salt2 + b'\x00\x6d\x79\x73\x71\x6c\x5f\x6e\x61\x74\x69\x76\x65\x5f\x70\x61\x73\x73\x77\x6f\x72\x64\x00'
         return self.build_packet(0x00, data)
 
+    def gen_salt(self, length):
+        charset = string.punctuation+string.ascii_letters+string.digits
+        return b''.join(bytes(random.choice(charset), "utf-8") for _ in range(length))
+
     def access_denied(self, seq_id, user, password=None):
         Y = "YES" if password else "NO"
         ip = self.transport.getPeer().host
         msg = "Access denied for user '{}'@'{}' (using password: {})".format(
             user.decode('utf8'), ip, Y)
         return self.error_pkt(seq_id, MySQL.ERR_CODE_ACCESS_DENIED,
                               MySQL.SQL_STATE_ACCESS_DENIED, msg.encode('utf8'))
@@ -127,14 +124,15 @@
                 # error on wrong seq_id, even if payload hasn't arrived yet
                 self.transport.write(self.unordered_pkt(0x01))
                 self.transport.loseConnection()
                 return
             elif payload is not None:
                 # seq_id == 1 and payload has arrived
                 username, password = self.parse_auth(payload)
+                username = bytes(str(username)[2:-1], "utf-8")
                 if username:
                     logdata = {'USERNAME': username, 'PASSWORD': password}
                     self.factory.canaryservice.log(logdata, transport=self.transport)
                     self.transport.write(self.access_denied(0x02, username, password))
                     self.transport.loseConnection()
         finally:
             self._busyReceiving = False
```

### Comparing `opencanary-0.7.1/opencanary/modules/ntp.py` & `opencanary-0.9.0/opencanary/modules/ntp.py`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/portscan.py` & `opencanary-0.9.0/opencanary/modules/portscan.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from opencanary.modules import CanaryService
 from opencanary.modules import FileSystemWatcher
 import os
 import re
+import shutil
 
 class SynLogWatcher(FileSystemWatcher):
     def __init__(self, logger=None, logFile=None, ignore_localhost=False):
         self.logger = logger
         self.ignore_localhost = ignore_localhost
         #print ('SynLogWatcher started')
         FileSystemWatcher.__init__(self, fileName=logFile)
@@ -84,47 +85,51 @@
             self.nmaposrate = 5
 
         try:
             self.lorate = int(self.lorate)
         except:
             self.lorate = 3
 
+    def getIptablesPath(self):
+        return shutil.which('iptables') or '/sbin/iptables'
+
     def startYourEngines(self, reactor=None):
         # Logging rules for loopback interface.
         # This is separate from the canaryfw rule as the canary watchdog was
         # causing console-side noise in the logs.
-        os.system('sudo /sbin/iptables -t mangle -D PREROUTING -p tcp -i lo -j LOG --log-level=warning --log-prefix="canaryfw: " -m limit --limit="{0}/hour"'.format(self.lorate))
-        os.system('sudo /sbin/iptables -t mangle -A PREROUTING -p tcp -i lo -j LOG --log-level=warning --log-prefix="canaryfw: " -m limit --limit="{0}/hour"'.format(self.lorate))
+        iptables_path=self.getIptablesPath()
+        os.system('sudo {0} -t mangle -D PREROUTING -p tcp -i lo -j LOG --log-level=warning --log-prefix="canaryfw: " -m limit --limit="{1}/hour"'.format(iptables_path, self.lorate))
+        os.system('sudo {0} -t mangle -A PREROUTING -p tcp -i lo -j LOG --log-level=warning --log-prefix="canaryfw: " -m limit --limit="{1}/hour"'.format(iptables_path, self.lorate))
 
         # Logging rules for canaryfw.
         # We ignore loopback interface traffic as it is taken care of in above rule
-        os.system('sudo /sbin/iptables -t mangle -D PREROUTING -p tcp --syn -j LOG --log-level=warning --log-prefix="canaryfw: " -m limit --limit="{0}/second" ! -i lo'.format(self.synrate))
-        os.system('sudo /sbin/iptables -t mangle -A PREROUTING -p tcp --syn -j LOG --log-level=warning --log-prefix="canaryfw: " -m limit --limit="{0}/second" ! -i lo'.format(self.synrate))
+        os.system('sudo {0} -t mangle -D PREROUTING -p tcp --syn -j LOG --log-level=warning --log-prefix="canaryfw: " -m limit --limit="{1}/second" ! -i lo'.format(iptables_path, self.synrate))
+        os.system('sudo {0} -t mangle -A PREROUTING -p tcp --syn -j LOG --log-level=warning --log-prefix="canaryfw: " -m limit --limit="{1}/second" ! -i lo'.format(iptables_path, self.synrate))
 
         # os.system('sudo /sbin/iptables -t mangle -D PREROUTING -p tcp {dst} --syn -j LOG --log-level=warning --log-prefix="canaryfw: " -m limit --limit="{synrate}/second"'
         #             .format(dst=(('--destination '+self.listen_addr) if len(self.listen_addr) else ''),
         #                 synrate=self.synrate))
         # os.system('sudo /sbin/iptables -t mangle -A PREROUTING -p tcp {dst} --syn -j LOG --log-level=warning --log-prefix="canaryfw: " -m limit --limit="{synrate}/second"'
         #             .format(dst=(('--destination '+self.listen_addr) if len(self.listen_addr) else ''),
         #                 synrate=self.synrate))
 
          # Match the T3 probe of the nmap OS detection based on TCP flags and TCP options string
-        os.system('sudo /sbin/iptables -t mangle -D PREROUTING -p tcp --tcp-flags ALL URG,PSH,SYN,FIN -m u32 --u32 "40=0x03030A01 && 44=0x02040109 && 48=0x080Affff && 52=0xffff0000 && 56=0x00000402" -j LOG --log-level=warning --log-prefix="canarynmap: " -m limit --limit="{0}/second"'.format(self.nmaposrate))
-        os.system('sudo /sbin/iptables -t mangle -A PREROUTING -p tcp --tcp-flags ALL URG,PSH,SYN,FIN -m u32 --u32 "40=0x03030A01 && 44=0x02040109 && 48=0x080Affff && 52=0xffff0000 && 56=0x00000402" -j LOG --log-level=warning --log-prefix="canarynmap: " -m limit --limit="{0}/second"'.format(self.nmaposrate))
+        os.system('sudo {0} -t mangle -D PREROUTING -p tcp --tcp-flags ALL URG,PSH,SYN,FIN -m u32 --u32 "40=0x03030A01 && 44=0x02040109 && 48=0x080Affff && 52=0xffff0000 && 56=0x00000402" -j LOG --log-level=warning --log-prefix="canarynmap: " -m limit --limit="{1}/second"'.format(iptables_path, self.nmaposrate))
+        os.system('sudo {0} -t mangle -A PREROUTING -p tcp --tcp-flags ALL URG,PSH,SYN,FIN -m u32 --u32 "40=0x03030A01 && 44=0x02040109 && 48=0x080Affff && 52=0xffff0000 && 56=0x00000402" -j LOG --log-level=warning --log-prefix="canarynmap: " -m limit --limit="{1}/second"'.format(iptables_path, self.nmaposrate))
 
         # Nmap Null Scan
-        os.system('sudo /sbin/iptables -t mangle -D PREROUTING -p tcp -m u32 --u32 "6&0xFF=0x6 && 0>>22&0x3C@12=0x50000400" -j LOG --log-level=warning --log-prefix="canarynmapNULL: " -m limit --limit="{0}/second"'.format(self.nmaposrate))
-        os.system('sudo /sbin/iptables -t mangle -A PREROUTING -p tcp -m u32 --u32 "6&0xFF=0x6 && 0>>22&0x3C@12=0x50000400" -j LOG --log-level=warning --log-prefix="canarynmapNULL: " -m limit --limit="{0}/second"'.format(self.nmaposrate))
+        os.system('sudo {0} -t mangle -D PREROUTING -p tcp -m u32 --u32 "6&0xFF=0x6 && 0>>22&0x3C@12=0x50000400" -j LOG --log-level=warning --log-prefix="canarynmapNULL: " -m limit --limit="{1}/second"'.format(iptables_path, self.nmaposrate))
+        os.system('sudo {0} -t mangle -A PREROUTING -p tcp -m u32 --u32 "6&0xFF=0x6 && 0>>22&0x3C@12=0x50000400" -j LOG --log-level=warning --log-prefix="canarynmapNULL: " -m limit --limit="{1}/second"'.format(iptables_path, self.nmaposrate))
 
         # Nmap Xmas Scan
-        os.system('sudo /sbin/iptables -t mangle -D PREROUTING -p tcp -m u32 --u32 "6&0xFF=0x6 && 0>>22&0x3C@12=0x50290400" -j LOG --log-level=warning --log-prefix="canarynmapXMAS: " -m limit --limit="{0}/second"'.format(self.nmaposrate))
-        os.system('sudo /sbin/iptables -t mangle -A PREROUTING -p tcp -m u32 --u32 "6&0xFF=0x6 && 0>>22&0x3C@12=0x50290400" -j LOG --log-level=warning --log-prefix="canarynmapXMAS: " -m limit --limit="{0}/second"'.format(self.nmaposrate))
+        os.system('sudo {0} -t mangle -D PREROUTING -p tcp -m u32 --u32 "6&0xFF=0x6 && 0>>22&0x3C@12=0x50290400" -j LOG --log-level=warning --log-prefix="canarynmapXMAS: " -m limit --limit="{1}/second"'.format(iptables_path, self.nmaposrate))
+        os.system('sudo {0} -t mangle -A PREROUTING -p tcp -m u32 --u32 "6&0xFF=0x6 && 0>>22&0x3C@12=0x50290400" -j LOG --log-level=warning --log-prefix="canarynmapXMAS: " -m limit --limit="{1}/second"'.format(iptables_path, self.nmaposrate))
 
         # Nmap Fin Scan
-        os.system('sudo /sbin/iptables -t mangle -D PREROUTING -p tcp -m u32 --u32 "6&0xFF=0x6 && 0>>22&0x3C@12=0x50010400" -j LOG --log-level=warning --log-prefix="canarynmapFIN: " -m limit --limit="{0}/second"'.format(self.nmaposrate))
-        os.system('sudo /sbin/iptables -t mangle -A PREROUTING -p tcp -m u32 --u32 "6&0xFF=0x6 && 0>>22&0x3C@12=0x50010400" -j LOG --log-level=warning --log-prefix="canarynmapFIN: " -m limit --limit="{0}/second"'.format(self.nmaposrate))
+        os.system('sudo {0} -t mangle -D PREROUTING -p tcp -m u32 --u32 "6&0xFF=0x6 && 0>>22&0x3C@12=0x50010400" -j LOG --log-level=warning --log-prefix="canarynmapFIN: " -m limit --limit="{1}/second"'.format(iptables_path, self.nmaposrate))
+        os.system('sudo {0} -t mangle -A PREROUTING -p tcp -m u32 --u32 "6&0xFF=0x6 && 0>>22&0x3C@12=0x50010400" -j LOG --log-level=warning --log-prefix="canarynmapFIN: " -m limit --limit="{1}/second"'.format(iptables_path, self.nmaposrate))
 
         fs = SynLogWatcher(logFile=self.audit_file, logger=self.logger, ignore_localhost=self.ignore_localhost)
         fs.start()
 
     def configUpdated(self,):
         pass
```

### Comparing `opencanary-0.7.1/opencanary/modules/redis.py` & `opencanary-0.9.0/opencanary/modules/redis.py`

 * *Files 0% similar despite different names*

```diff
@@ -377,15 +377,15 @@
                 cmd, args, self._data = _parseInlineCommand(self._data)
             commands.append((cmd, args))
 
         return commands
 
     def dataReceived(self, data):
         """
-        Recieved data is unbuffered so we buffer it for telnet.
+        Received data is unbuffered so we buffer it for telnet.
         """
         try:
             try:
                 #A command split over multiple packets is collected into a single
                 #string until it can all be processed. If multiple commands
                 #are in a single packet and missing some data, run again
```

### Comparing `opencanary-0.7.1/opencanary/modules/samba.py` & `opencanary-0.9.0/opencanary/modules/samba.py`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/sip.py` & `opencanary-0.9.0/opencanary/modules/sip.py`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/snmp.py` & `opencanary-0.9.0/opencanary/modules/snmp.py`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/ssh.py` & `opencanary-0.9.0/opencanary/modules/ssh.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-from __future__ import print_function
-from opencanary.modules import CanaryService
-from opencanary.config import PY3
 
+from opencanary.modules import CanaryService
 import twisted
 from twisted.cred import portal, checkers, credentials, error
 from twisted.conch import error, avatar, interfaces as conchinterfaces
 from twisted.conch.checkers import SSHPublicKeyDatabase
 from twisted.conch.ssh import factory, userauth, connection, keys, session, transport
 from twisted.conch.openssh_compat import primes
 from twisted.conch.ssh.common import MP
@@ -86,18 +84,15 @@
             key_blob = getNS(getNS(packet[1:])[1])[0]
         except:
             key_blob = "No public key found."
         try:
             #convert blob into openssh key format
             key = keys.Key.fromString(key_blob).toString('openssh')
         except:
-            if not PY3:
-                key = "Invalid SSH Public Key Submitted: {key_blob}".format(key_blob=key_blob.encode('hex'))
-            else:
-                key = "Invalid SSH Public Key Submitted: {key_blob}".format(key_blob=key_blob.hex())
+            key = "Invalid SSH Public Key Submitted: {key_blob}".format(key_blob=key_blob.hex())
             for keytype in [b'ecdsa-sha2-nistp256',b'ecdsa-sha2-nistp384',b'ecdsa-sha2-nistp521',b'ssh-ed25519']:
                 if keytype in key_blob:
                     key = '{keytype} {keydata}'.format(
                             keytype=keytype,
                             keydata=base64.b64encode(key_blob))
 
             print('Key was {key}'.format(key=key))
```

### Comparing `opencanary-0.7.1/opencanary/modules/tcpbanner.py` & `opencanary-0.9.0/opencanary/modules/tcpbanner.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,45 +31,53 @@
         self.keep_alive_secret = keep_alive_secret
         self.keep_alive_idle = keep_alive_idle
         self.keep_alive_interval = keep_alive_interval
         self.keep_alive_probes = keep_alive_probes
 
     def connectionMade(self):
         #We limit the data sent through to 255 chars
-        data = str(self.accept_banner)[:255]
+        try:
+            data = str(self.accept_banner)[:255]
 
-        logdata = {'FUNCTION': 'CONNECTION_MADE', 'DATA':data,
-                   'BANNER_ID':str(self.banner_id)}
+            logdata = {'FUNCTION': 'CONNECTION_MADE', 'DATA':data,
+                    'BANNER_ID':str(self.banner_id)}
 
-        if self.keep_alive_enabled:
-            if hasattr(socket, 'TCP_KEEPIDLE'):
-                # overrides value (in seconds) of system-wide ipv4 tcp_keepalive_time
-                self.transport.getHandle().setsockopt(socket.SOL_TCP, socket.TCP_KEEPIDLE, self.keep_alive_idle)
-            # overrides value (in seconds) of system-wide ipv4 tcp_keepalive_intvl
-            self.transport.getHandle().setsockopt(socket.SOL_TCP, socket.TCP_KEEPINTVL, self.keep_alive_interval)
-            # overrides value (in seconds) of system-wide ipv4 tcp_keepalive_probes
-            self.transport.getHandle().setsockopt(socket.SOL_TCP, socket.TCP_KEEPCNT, self.keep_alive_probes)
-            # set keep alive on socket
-            self.transport.setTcpKeepAlive(1)
+            if self.keep_alive_enabled:
+                if hasattr(socket, 'TCP_KEEPIDLE'):
+                    # overrides value (in seconds) of system-wide ipv4 tcp_keepalive_time
+                    self.transport.getHandle().setsockopt(socket.SOL_TCP, socket.TCP_KEEPIDLE, self.keep_alive_idle)
+                if hasattr(socket, 'TCP_KEEPINTVL'):
+                    # overrides value (in seconds) of system-wide ipv4 tcp_keepalive_intvl
+                    self.transport.getHandle().setsockopt(socket.SOL_TCP, socket.TCP_KEEPINTVL, int(self.keep_alive_interval))
+                if hasattr(socket, 'TCP_KEEPCNT'):
+                    # overrides value (in seconds) of system-wide ipv4 tcp_keepalive_probes
+                    self.transport.getHandle().setsockopt(socket.SOL_TCP, socket.TCP_KEEPCNT, self.keep_alive_probes)
+                # set keep alive on socket
+                self.transport.setTcpKeepAlive(1)
+
+                self.factory.canaryservice.logtype = self.factory.canaryservice.logger.LOG_TCP_BANNER_KEEP_ALIVE_CONNECTION_MADE
+                self.factory.canaryservice.log(logdata, transport=self.transport)
+
+            elif not self.alert_string_enabled:
+                #flag says we need to wait for incoming data to include a string
+                #so no point in logging anything here
 
-            self.factory.canaryservice.logtype = self.factory.canaryservice.logger.LOG_TCP_BANNER_KEEP_ALIVE_CONNECTION_MADE
-            self.factory.canaryservice.log(logdata, transport=self.transport)
+                self.factory.canaryservice.logtype = self.factory.canaryservice.logger.LOG_TCP_BANNER_CONNECTION_MADE
+                self.factory.canaryservice.log(logdata, transport=self.transport)
 
-        elif not self.alert_string_enabled:
-            #flag says we need to wait for incoming data to include a string
-            #so no point in logging anything here
+            self.transport.write(self.accept_banner)
 
+        except OSError:
+            print('Received an OSError. Likely the socket has closed.')
             self.factory.canaryservice.logtype = self.factory.canaryservice.logger.LOG_TCP_BANNER_CONNECTION_MADE
             self.factory.canaryservice.log(logdata, transport=self.transport)
 
-        self.transport.write(self.accept_banner)
-
     def dataReceived(self, data):
         """
-        Recieved data from tcp connection after connection has been made.
+        Received data from tcp connection after connection has been made.
         """
         try:
             if self.keep_alive_disable_alerting:
                 self.transport.write(self.send_banner)
                 return
 
             #We limit the data sent through to 255 chars
```

### Comparing `opencanary-0.7.1/opencanary/modules/telnet.py` & `opencanary-0.9.0/opencanary/modules/telnet.py`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/testpdf.py` & `opencanary-0.9.0/opencanary/modules/testpdf.py`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/tftp.py` & `opencanary-0.9.0/opencanary/modules/tftp.py`

 * *Files identical despite different names*

### Comparing `opencanary-0.7.1/opencanary/modules/vnc.py` & `opencanary-0.9.0/opencanary/modules/vnc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-from __future__ import print_function
 from opencanary.modules import CanaryService
 
 from twisted.internet.protocol import Protocol
 from twisted.internet.protocol import Factory
 from twisted.application import internet
 
 from opencanary.modules.des import des
-from opencanary.config import PY3
 import sys
 
 import os
 
 RFB_33  = b'003.003'
 RFB_37  = b'003.007'
 RFB_38  = b'003.008'
@@ -82,22 +80,16 @@
         self.state = AUTH_SEND
 
     def _recv_auth(self,data=None):
         print('got auth')
         if len(data) != 16:
             raise ProtocolError()
 
-        if PY3:
-            logdata = {"VNC Server Challenge" : self.challenge.hex(),
-                       "VNC Client Response": data.hex()
-                    }
-        else:
-            logdata = {"VNC Server Challenge" : self.challenge.encode('hex'),
-                       "VNC Client Response": data.encode('hex')
-                    }
+        logdata = {"VNC Server Challenge" : self.challenge.hex(),
+                    "VNC Client Response": data.hex()}
 
         used_password = self._try_decrypt_response(response=data)
         if used_password:
             logdata['VNC Password'] = used_password
         else:
             logdata['VNC Password'] = '<Password was not in the common list>'
         self.factory.log(logdata, transport=self.transport)
@@ -120,35 +112,29 @@
         #really inefficient, but it means we don't have to rely on
         #a static challenge
         for password in COMMON_PASSWORDS:
             pw = password[:8]#vnc passwords are max 8 chars
             if len(pw) < 8:
                 pw+= '\x00'*(8-len(pw))
 
-            if not PY3:
-                #VNC use of DES requires password bits to be mirrored
-                pw = ''.join([chr(int('{:08b}'.format(ord(x))[::-1], 2))
-                                                           for x in pw])
-                desbox = des(pw)
-            else:
-                pw = pw.encode('ascii')
-                # VNC use of DES requires password bits to be mirrored
-                values = bytearray()
-                for x in pw:
-                    values.append(int('{:08b}'.format(x)[::-1], 2))
-                desbox = des(values)
+            pw = pw.encode('ascii')
+            # VNC use of DES requires password bits to be mirrored
+            values = bytearray()
+            for x in pw:
+                values.append(int('{:08b}'.format(x)[::-1], 2))
+            desbox = des(values)
 
             decrypted_challenge = desbox.decrypt(response)
             if decrypted_challenge == self.challenge:
                 return password
         return None
 
     def dataReceived(self, data):
         """
-        Recieved data is unbuffered so we buffer it for telnet.
+        Received data is unbuffered so we buffer it for telnet.
         """
         try:
             if self.state == HANDSHAKE_SEND:
                 self._recv_handshake(data=data)
             elif self.state == SECURITY_SEND:
                 self._recv_security(data=data)
             elif self.state == AUTH_SEND:
```

### Comparing `opencanary-0.7.1/opencanary.egg-info/PKG-INFO` & `opencanary-0.9.0/opencanary.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: opencanary
-Version: 0.7.1
+Version: 0.9.0
 Summary: OpenCanary daemon
 Home-page: http://www.thinkst.com/
 Author: Thinkst Applied Research
 Author-email: info@thinkst.com
 License: BSD
-Description: A low interaction honeypot intended to be run on internal networks.
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: Twisted
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Networking :: Monitoring
 Classifier: Natural Language :: English
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: POSIX :: BSD :: FreeBSD
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: BSD License
+License-File: LICENSE
+
+A low interaction honeypot intended to be run on internal networks.
```

### Comparing `opencanary-0.7.1/opencanary.egg-info/SOURCES.txt` & `opencanary-0.9.0/opencanary.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,20 @@
-.gitignore
-Dockerfile.latest
-Dockerfile.stable
 LICENSE
+MANIFEST.in
 README.md
-docker-compose.yml
 opencanary.service
 requirements.txt
 run.sh
 setup.py
-.github/workflows/opencanary_tests.yml
 bin/honeycred
 bin/opencanary-correlator
 bin/opencanary.tac
 bin/opencanaryd
+build_scripts/generate_macOS_launchctl_service_files.py
 data/.opencanary.conf
-docs/Makefile
-docs/conf.py
-docs/index.rst
-docs/logo.png
-docs/alerts/email.rst
-docs/alerts/hpfeeds.rst
-docs/alerts/webhook.rst
-docs/services/mssql.rst
-docs/services/mysql.rst
-docs/services/webserver.rst
-docs/services/windows.rst
-docs/starting/configuration.rst
-docs/starting/correlator.rst
-docs/starting/opencanary.rst
 opencanary/__init__.py
 opencanary/config.py
 opencanary/honeycred.py
 opencanary/iphelper.py
 opencanary/logger.py
 opencanary.egg-info/PKG-INFO
 opencanary.egg-info/SOURCES.txt
@@ -44,14 +27,15 @@
 opencanary/modules/des.py
 opencanary/modules/example0.py
 opencanary/modules/example1.py
 opencanary/modules/ftp.py
 opencanary/modules/git.py
 opencanary/modules/http.py
 opencanary/modules/httpproxy.py
+opencanary/modules/https.py
 opencanary/modules/mssql.py
 opencanary/modules/mysql.py
 opencanary/modules/ntp.py
 opencanary/modules/portscan.py
 opencanary/modules/rdp.py
 opencanary/modules/redis.py
 opencanary/modules/samba.py
@@ -260,11 +244,9 @@
 opencanary/modules/data/http/skin/nasLogin/static/img/synohdpack/images/scrollbar/scrollbar_white_v.png
 opencanary/modules/data/http/skin/nasLogin/static/js/misc.js
 opencanary/modules/data/httpproxy/skin/squid/auth.html
 opencanary/modules/data/rdp/default.rss
 opencanary/modules/data/rdp/login-failed.rss
 opencanary/modules/data/rdp/login-passreset.rss
 opencanary/modules/data/rdp/login.rss
-opencanary/test/logger.py
-opencanary/test/module_test.py
-opencanary/test/opencanary.conf
-opencanary/test/requirements.txt
+opencanary/modules/test/ftp/__init__.py
+opencanary/modules/test/ftp/test_ftp.py
```

### Comparing `opencanary-0.7.1/setup.py` & `opencanary-0.9.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,12 @@
 import codecs
 import os.path
-from setuptools import setup, find_packages
+from setuptools import setup, find_namespace_packages
 import sys
 
-PY3 = sys.version_info > (3,)
-
-# Only check unicode on Python 2, In Python 3 unicode is the default and we can just return the input.
-if sys.version_info[0] < 3:
-    jinja_version = '2.10.1'
-else:
-    jinja_version = '3.0.1'
-
 
 def read(rel_path):
     here = os.path.abspath(os.path.dirname(__file__))
     with codecs.open(os.path.join(here, rel_path), 'r') as fp:
         return fp.read()
 
 def get_version(rel_path):
@@ -26,61 +18,63 @@
         if line.startswith('__version__'):
             delim = '"' if '"' in line else "'"
             return line.split(delim)[1]
     else:
         raise RuntimeError("Unable to find version string.")
 
 requirements = [
-    'Twisted==19.10.0',
+    'Twisted==22.8.0',
     'pyasn1==0.4.5',
-    'cryptography==3.0',
+    'cryptography==38.0.1',
     'simplejson==3.16.0',
     'requests==2.21.0',
     'zope.interface==5.0.0',
     'PyPDF2==1.26.0',
     'fpdf==1.7.2',
     'passlib==1.7.1',
-    'Jinja2=={}'.format(jinja_version),
+    'Jinja2==3.0.1',
     'ntlmlib==0.72',
     'bcrypt==3.1.7',
-    'setuptools==44.0.0',
-    'hpfeeds==3.0.0']
+    'setuptools==63.2.0',
+    'hpfeeds==3.0.0',
+    'pyOpenSSL==22.1.0',
+    "service-identity==21.1.0"
+]
 
-if sys.version_info.major < 3:
-    requirements.append('wsgiref==0.1.2')
 
 setup(
     name='opencanary',
     version=get_version("opencanary/__init__.py"),
     url='http://www.thinkst.com/',
     author='Thinkst Applied Research',
     author_email='info@thinkst.com',
     description='OpenCanary daemon',
     long_description='A low interaction honeypot intended to be run on internal networks.',
     install_requires=requirements,
-    setup_requires=[
-        'setuptools_git'
-    ],
     license='BSD',
-    packages=find_packages(exclude='test'),
+    packages=find_namespace_packages(
+        exclude=[
+            'docs','docs*'
+            'opencanary.test','opencanary.test*'
+        ]
+    ),
+    include_package_data = True,
     scripts=['bin/opencanaryd','bin/opencanary.tac'],
     platforms='any',
-    include_package_data=True,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Framework :: Twisted",
         "Topic :: System :: Networking",
         "Topic :: Security",
         "Topic :: System :: Networking :: Monitoring",
         "Natural Language :: English",
         "Operating System :: Unix",
         "Operating System :: POSIX :: Linux",
         "Operating System :: POSIX :: BSD :: FreeBSD",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "License :: OSI Approved :: BSD License",
     ],
 )
```

