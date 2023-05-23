# Comparing `tmp/hxl-proxy-1.9.1.tar.gz` & `tmp/hxl-proxy-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hxl-proxy-1.9.1.tar", last modified: Thu Jul  5 18:57:36 2018, max compression
+gzip compressed data, was "hxl-proxy-2.0.tar", last modified: Tue May 23 20:32:22 2023, max compression
```

## Comparing `hxl-proxy-1.9.1.tar` & `hxl-proxy-2.0.tar`

### file list

```diff
@@ -1,552 +1,157 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/
--rw-rw-r--   0 david     (1000) david     (1000)       77 2015-09-22 20:37:21.000000 hxl-proxy-1.9.1/MANIFEST.in
--rw-rw-r--   0 david     (1000) david     (1000)     2990 2018-06-27 20:58:15.000000 hxl-proxy-1.9.1/README.md
--rw-rw-r--   0 david     (1000) david     (1000)      260 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/PKG-INFO
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)    28674 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)      260 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)       10 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy.egg-info/top_level.txt
--rw-rw-r--   0 david     (1000) david     (1000)      109 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2015-12-19 19:33:34.000000 hxl-proxy-1.9.1/hxl_proxy.egg-info/not-zip-safe
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/
--rw-rw-r--   0 david     (1000) david     (1000)      929 2016-12-02 21:07:03.000000 hxl-proxy-1.9.1/hxl_proxy/preview.py
--rw-rw-r--   0 david     (1000) david     (1000)    11883 2018-03-29 19:54:05.000000 hxl-proxy-1.9.1/hxl_proxy/dao.py
--rw-rw-r--   0 david     (1000) david     (1000)      324 2016-08-30 19:10:00.000000 hxl-proxy-1.9.1/hxl_proxy/exceptions.py
--rw-rw-r--   0 david     (1000) david     (1000)      316 2016-02-26 20:05:02.000000 hxl-proxy-1.9.1/hxl_proxy/default_config.py
--rw-rw-r--   0 david     (1000) david     (1000)    11904 2018-06-29 14:15:31.000000 hxl-proxy-1.9.1/hxl_proxy/util.py
--rw-rw-r--   0 david     (1000) david     (1000)     1925 2016-02-18 15:46:10.000000 hxl-proxy-1.9.1/hxl_proxy/auth.py
--rw-rw-r--   0 david     (1000) david     (1000)    12540 2018-06-27 20:58:15.000000 hxl-proxy-1.9.1/hxl_proxy/filters.py
--rw-rw-r--   0 david     (1000) david     (1000)     1465 2017-11-22 15:54:40.000000 hxl-proxy-1.9.1/hxl_proxy/reverse_proxied.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/templates/
--rw-rw-r--   0 david     (1000) david     (1000)     1807 2018-01-30 18:41:49.000000 hxl-proxy-1.9.1/hxl_proxy/templates/error.html
--rw-rw-r--   0 david     (1000) david     (1000)     2547 2018-04-09 15:38:13.000000 hxl-proxy-1.9.1/hxl_proxy/templates/data-view.html
--rw-rw-r--   0 david     (1000) david     (1000)      954 2017-11-22 15:54:40.000000 hxl-proxy-1.9.1/hxl_proxy/templates/data-login.html
--rw-rw-r--   0 david     (1000) david     (1000)     4611 2017-11-22 15:54:40.000000 hxl-proxy-1.9.1/hxl_proxy/templates/visualise-map.html
--rw-rw-r--   0 david     (1000) david     (1000)     2433 2018-06-29 14:15:31.000000 hxl-proxy-1.9.1/hxl_proxy/templates/validate-issue.html
--rw-rw-r--   0 david     (1000) david     (1000)     7118 2017-11-22 15:54:40.000000 hxl-proxy-1.9.1/hxl_proxy/templates/visualise-chart.html
--rw-rw-r--   0 david     (1000) david     (1000)     4107 2018-01-30 18:41:49.000000 hxl-proxy-1.9.1/hxl_proxy/templates/data-source.html
--rw-rw-r--   0 david     (1000) david     (1000)     3165 2017-11-22 15:54:40.000000 hxl-proxy-1.9.1/hxl_proxy/templates/data-save.html
--rw-rw-r--   0 david     (1000) david     (1000)     2671 2017-11-22 15:54:40.000000 hxl-proxy-1.9.1/hxl_proxy/templates/hxl-test.html
--rw-rw-r--   0 david     (1000) david     (1000)     4581 2018-05-31 13:18:37.000000 hxl-proxy-1.9.1/hxl_proxy/templates/about.html
--rw-rw-r--   0 david     (1000) david     (1000)     6177 2018-03-29 19:54:05.000000 hxl-proxy-1.9.1/hxl_proxy/templates/data-tagger.html
--rw-rw-r--   0 david     (1000) david     (1000)     3372 2018-03-29 19:54:05.000000 hxl-proxy-1.9.1/hxl_proxy/templates/data-advanced.html
--rw-rw-r--   0 david     (1000) david     (1000)     1042 2018-06-29 14:15:31.000000 hxl-proxy-1.9.1/hxl_proxy/templates/iati2hxl.html
--rw-rw-r--   0 david     (1000) david     (1000)     5379 2018-06-29 14:15:31.000000 hxl-proxy-1.9.1/hxl_proxy/templates/validate-summary.html
--rw-rw-r--   0 david     (1000) david     (1000)     1633 2016-02-22 19:11:17.000000 hxl-proxy-1.9.1/hxl_proxy/templates/settings-user.html
--rw-rw-r--   0 david     (1000) david     (1000)     8511 2017-11-22 15:54:40.000000 hxl-proxy-1.9.1/hxl_proxy/templates/data-recipe.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/templates/includes/
--rw-rw-r--   0 david     (1000) david     (1000)      847 2018-05-04 01:59:37.000000 hxl-proxy-1.9.1/hxl_proxy/templates/includes/hxltable.html
--rw-rw-r--   0 david     (1000) david     (1000)      368 2016-04-29 17:37:43.000000 hxl-proxy-1.9.1/hxl_proxy/templates/includes/selectors.html
--rw-rw-r--   0 david     (1000) david     (1000)      142 2016-02-26 20:05:02.000000 hxl-proxy-1.9.1/hxl_proxy/templates/includes/recipe-form.html
--rw-rw-r--   0 david     (1000) david     (1000)      382 2016-12-02 21:07:03.000000 hxl-proxy-1.9.1/hxl_proxy/templates/includes/tagger-params.html
--rw-rw-r--   0 david     (1000) david     (1000)      496 2016-02-18 15:46:10.000000 hxl-proxy-1.9.1/hxl_proxy/templates/includes/chooser-scripts.html
--rw-rw-r--   0 david     (1000) david     (1000)      153 2016-12-02 21:07:03.000000 hxl-proxy-1.9.1/hxl_proxy/templates/includes/params.html
--rw-rw-r--   0 david     (1000) david     (1000)      790 2016-02-18 15:46:10.000000 hxl-proxy-1.9.1/hxl_proxy/templates/includes/postcards.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/
--rw-rw-r--   0 david     (1000) david     (1000)     5287 2016-12-02 21:07:03.000000 hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/count.html
--rw-rw-r--   0 david     (1000) david     (1000)      630 2016-12-02 21:07:03.000000 hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/filter-list.html
--rw-rw-r--   0 david     (1000) david     (1000)     1669 2018-06-27 20:58:15.000000 hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/jsonpath.html
--rw-rw-r--   0 david     (1000) david     (1000)     1854 2016-12-02 21:07:03.000000 hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/append.html
--rw-rw-r--   0 david     (1000) david     (1000)      546 2018-06-27 20:58:15.000000 hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/filter-types.j2
--rw-rw-r--   0 david     (1000) david     (1000)      643 2016-12-02 21:07:03.000000 hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/filter-selector.html
--rw-rw-r--   0 david     (1000) david     (1000)     1278 2016-12-02 21:07:03.000000 hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/explode.html
--rw-rw-r--   0 david     (1000) david     (1000)     2139 2018-07-05 18:51:25.000000 hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/replace.html
--rw-rw-r--   0 david     (1000) david     (1000)     1762 2016-12-02 21:07:03.000000 hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/add.html
--rw-rw-r--   0 david     (1000) david     (1000)     1258 2016-12-02 21:07:03.000000 hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/replace-map.html
--rw-rw-r--   0 david     (1000) david     (1000)     1514 2016-12-02 21:07:03.000000 hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/rename.html
--rw-rw-r--   0 david     (1000) david     (1000)     1205 2016-12-02 21:07:03.000000 hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/dedup.html
--rw-rw-r--   0 david     (1000) david     (1000)     1459 2018-01-30 18:41:49.000000 hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/cut.html
--rw-rw-r--   0 david     (1000) david     (1000)     5128 2018-03-29 19:54:05.000000 hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/clean.html
--rw-rw-r--   0 david     (1000) david     (1000)     1182 2018-07-05 18:56:48.000000 hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/filter-variables.j2
--rw-rw-r--   0 david     (1000) david     (1000)     2427 2016-12-02 21:07:03.000000 hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/merge.html
--rw-rw-r--   0 david     (1000) david     (1000)     1187 2016-12-02 21:07:03.000000 hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/select.html
--rw-rw-r--   0 david     (1000) david     (1000)     1174 2018-06-27 20:58:15.000000 hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/fill.html
--rw-rw-r--   0 david     (1000) david     (1000)      910 2016-12-02 21:07:03.000000 hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/sort.html
--rw-rw-r--   0 david     (1000) david     (1000)      171 2016-12-02 21:07:03.000000 hxl-proxy-1.9.1/hxl_proxy/templates/includes/help.html
--rw-rw-r--   0 david     (1000) david     (1000)      329 2016-12-02 21:07:03.000000 hxl-proxy-1.9.1/hxl_proxy/templates/includes/metadata-params.html
--rw-rw-r--   0 david     (1000) david     (1000)      443 2016-07-30 02:21:45.000000 hxl-proxy-1.9.1/hxl_proxy/templates/includes/scripts.html
--rw-rw-r--   0 david     (1000) david     (1000)      923 2017-11-22 15:54:40.000000 hxl-proxy-1.9.1/hxl_proxy/templates/includes/data-tabs.html
--rw-rw-r--   0 david     (1000) david     (1000)      182 2016-02-26 20:05:02.000000 hxl-proxy-1.9.1/hxl_proxy/templates/includes/source.html
--rw-rw-r--   0 david     (1000) david     (1000)     2317 2016-02-18 15:46:10.000000 hxl-proxy-1.9.1/hxl_proxy/templates/includes/headers.html
--rw-rw-r--   0 david     (1000) david     (1000)     3569 2018-05-31 13:18:37.000000 hxl-proxy-1.9.1/hxl_proxy/templates/includes/navbar.html
--rw-rw-r--   0 david     (1000) david     (1000)      412 2016-12-02 21:07:03.000000 hxl-proxy-1.9.1/hxl_proxy/templates/includes/recipe-params.html
--rw-rw-r--   0 david     (1000) david     (1000)      259 2016-02-18 15:46:10.000000 hxl-proxy-1.9.1/hxl_proxy/templates/includes/messages.html
--rw-rw-r--   0 david     (1000) david     (1000)     4269 2018-05-02 16:05:10.000000 hxl-proxy-1.9.1/hxl_proxy/pcodes.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/libhxl/
--rw-rw-r--   0 david     (1000) david     (1000)    52355 2016-06-22 20:48:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/libhxl/hxl.js
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/leaflet/
--rw-rw-r--   0 david     (1000) david     (1000)   125410 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/leaflet/leaflet.js
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/leaflet/images/
--rw-rw-r--   0 david     (1000) david     (1000)     4033 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/leaflet/images/marker-icon-2x.png
--rw-rw-r--   0 david     (1000) david     (1000)     2898 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/leaflet/images/layers-2x.png
--rw-rw-r--   0 david     (1000) david     (1000)     1747 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/leaflet/images/marker-icon.png
--rw-rw-r--   0 david     (1000) david     (1000)     1502 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/leaflet/images/layers.png
--rw-rw-r--   0 david     (1000) david     (1000)      797 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/leaflet/images/marker-shadow.png
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/leaflet/plugins/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/leaflet/plugins/markercluster/
--rw-rw-r--   0 david     (1000) david     (1000)      366 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/leaflet/plugins/markercluster/MarkerCluster.css
--rw-rw-r--   0 david     (1000) david     (1000)    58364 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/leaflet/plugins/markercluster/leaflet.markercluster-src.js
--rw-rw-r--   0 david     (1000) david     (1000)     1287 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/leaflet/plugins/markercluster/MarkerCluster.Default.css
--rw-rw-r--   0 david     (1000) david     (1000)    28286 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/leaflet/plugins/markercluster/leaflet.markercluster.js
--rw-rw-r--   0 david     (1000) david     (1000)   222761 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/leaflet/leaflet-src.js
--rw-rw-r--   0 david     (1000) david     (1000)    10161 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/leaflet/leaflet.css
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/images/
--rw-rw-r--   0 david     (1000) david     (1000)     2454 2016-02-18 15:46:10.000000 hxl-proxy-1.9.1/hxl_proxy/static/images/hxl-logo-white.png
--rw-rw-r--   0 david     (1000) david     (1000)     8850 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/images/csv-icon.png
--rw-rw-r--   0 david     (1000) david     (1000)    13225 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/images/dropbox-logo.png
--rw-rw-r--   0 david     (1000) david     (1000)     7767 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/images/hdx-logo.png
--rw-rw-r--   0 david     (1000) david     (1000)    22085 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/images/google-drive-logo.png
--rw-rw-r--   0 david     (1000) david     (1000)    55429 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/images/json-icon.png
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/compat/
--rw-rw-r--   0 david     (1000) david     (1000)     4377 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/compat/respond.min.js
--rw-rw-r--   0 david     (1000) david     (1000)     2636 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/compat/html5shiv.min.js
--rw-rw-r--   0 david     (1000) david     (1000)      694 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/compat/ie10-viewport-bug-workaround.js
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/jquery/
--rw-rw-r--   0 david     (1000) david     (1000)    84320 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/jquery/jquery.js
--rw-rw-r--   0 david     (1000) david     (1000)    10469 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/jquery/jquery.csv.js
--rw-rw-r--   0 david     (1000) david     (1000)   240427 2016-08-30 19:10:00.000000 hxl-proxy-1.9.1/hxl_proxy/static/jquery/jquery-ui.min.js
--rw-rw-r--   0 david     (1000) david     (1000)     1291 2016-12-02 21:07:03.000000 hxl-proxy-1.9.1/hxl_proxy/static/jquery/jquery.ui.touch-punch.min.js
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/
--rw-rw-r--   0 david     (1000) david     (1000)     3309 2018-05-04 01:59:37.000000 hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/hxl-proxy.css
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/
--rw-rw-r--   0 david     (1000) david     (1000)     4171 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/android-icon-72x72.png
--rw-rw-r--   0 david     (1000) david     (1000)     1249 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/favicon-16x16.png
--rw-rw-r--   0 david     (1000) david     (1000)     2618 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-57x57.png
--rw-rw-r--   0 david     (1000) david     (1000)    12219 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-precomposed.png
--rw-rw-r--   0 david     (1000) david     (1000)     3820 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-60x60.png
--rw-rw-r--   0 david     (1000) david     (1000)     4125 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/ms-icon-70x70.png
--rw-rw-r--   0 david     (1000) david     (1000)    27390 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/ms-icon-310x310.png
--rw-rw-r--   0 david     (1000) david     (1000)     7631 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-120x120.png
--rw-rw-r--   0 david     (1000) david     (1000)    11645 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/android-icon-192x192.png
--rw-rw-r--   0 david     (1000) david     (1000)     9448 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/ms-icon-144x144.png
--rw-rw-r--   0 david     (1000) david     (1000)    12668 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-180x180.png
--rw-rw-r--   0 david     (1000) david     (1000)     5857 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/android-icon-96x96.png
--rw-rw-r--   0 david     (1000) david     (1000)     3057 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/android-icon-48x48.png
--rw-rw-r--   0 david     (1000) david     (1000)     1150 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/favicon.ico
--rw-rw-r--   0 david     (1000) david     (1000)     7317 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-114x114.png
--rw-rw-r--   0 david     (1000) david     (1000)      727 2016-02-18 15:46:10.000000 hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/manifest.json
--rw-rw-r--   0 david     (1000) david     (1000)    10073 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/ms-icon-150x150.png
--rw-rw-r--   0 david     (1000) david     (1000)     4171 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-72x72.png
--rw-rw-r--   0 david     (1000) david     (1000)     9448 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/android-icon-144x144.png
--rw-rw-r--   0 david     (1000) david     (1000)     1960 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/android-icon-36x36.png
--rw-rw-r--   0 david     (1000) david     (1000)     4491 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-76x76.png
--rw-rw-r--   0 david     (1000) david     (1000)      281 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/browserconfig.xml
--rw-rw-r--   0 david     (1000) david     (1000)    10058 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-152x152.png
--rw-rw-r--   0 david     (1000) david     (1000)    12219 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/apple-icon.png
--rw-rw-r--   0 david     (1000) david     (1000)     1899 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/favicon-32x32.png
--rw-rw-r--   0 david     (1000) david     (1000)     5857 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/favicon-96x96.png
--rw-rw-r--   0 david     (1000) david     (1000)     9448 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-144x144.png
--rw-rw-r--   0 david     (1000) david     (1000)    29251 2017-06-13 22:33:38.000000 hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/hxl-proxy.js
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/bootstrap/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/bootstrap/css/
--rw-rw-r--   0 david     (1000) david     (1000)    19963 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/bootstrap/css/bootstrap-theme.min.css
--rw-rw-r--   0 david     (1000) david     (1000)    43339 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/bootstrap/css/bootstrap-theme.css.map
--rw-rw-r--   0 david     (1000) david     (1000)   117150 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/bootstrap/css/bootstrap.min.css
--rw-rw-r--   0 david     (1000) david     (1000)   379710 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/bootstrap/css/bootstrap.css.map
--rw-rw-r--   0 david     (1000) david     (1000)    22608 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/bootstrap/css/bootstrap-theme.css
--rw-rw-r--   0 david     (1000) david     (1000)   141414 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/bootstrap/css/bootstrap.css
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/bootstrap/fonts/
--rw-rw-r--   0 david     (1000) david     (1000)    18028 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.woff2
--rw-rw-r--   0 david     (1000) david     (1000)   108738 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.svg
--rw-rw-r--   0 david     (1000) david     (1000)    45404 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.ttf
--rw-rw-r--   0 david     (1000) david     (1000)    23424 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.woff
--rw-rw-r--   0 david     (1000) david     (1000)    20127 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.eot
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/bootstrap/js/
--rw-rw-r--   0 david     (1000) david     (1000)      484 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/bootstrap/js/npm.js
--rw-rw-r--   0 david     (1000) david     (1000)    35452 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/bootstrap/js/bootstrap.min.js
--rw-rw-r--   0 david     (1000) david     (1000)    66732 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/bootstrap/js/bootstrap.js
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/
--rw-rw-r--   0 david     (1000) david     (1000)      526 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/composer.json
--rw-rw-r--   0 david     (1000) david     (1000)      436 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/bower.json
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/server_side/
--rw-rw-r--   0 david     (1000) david     (1000)    16275 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/server_side/defer_loading.html
--rw-rw-r--   0 david     (1000) david     (1000)    14676 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/server_side/ids.html
--rw-rw-r--   0 david     (1000) david     (1000)    14341 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/server_side/custom_vars.html
--rw-rw-r--   0 david     (1000) david     (1000)    18382 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/server_side/row_details.html
--rw-rw-r--   0 david     (1000) david     (1000)    14851 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/server_side/post.html
--rw-rw-r--   0 david     (1000) david     (1000)     3735 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/server_side/index.html
--rw-rw-r--   0 david     (1000) david     (1000)    14301 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/server_side/object_data.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/server_side/scripts/
--rw-rw-r--   0 david     (1000) david     (1000)     7793 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/server_side/scripts/sqlserver.sql
--rw-rw-r--   0 david     (1000) david     (1000)    14161 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/server_side/scripts/ssp.class.php
--rw-rw-r--   0 david     (1000) david     (1000)     7689 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/server_side/scripts/postgres.sql
--rw-rw-r--   0 david     (1000) david     (1000)     1894 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/server_side/scripts/server_processing.php
--rw-rw-r--   0 david     (1000) david     (1000)     7711 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/server_side/scripts/mysql.sql
--rw-rw-r--   0 david     (1000) david     (1000)     1957 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/server_side/scripts/post.php
--rw-rw-r--   0 david     (1000) david     (1000)     1882 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/server_side/scripts/jsonp.php
--rw-rw-r--   0 david     (1000) david     (1000)     2244 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/server_side/scripts/ids-arrays.php
--rw-rw-r--   0 david     (1000) david     (1000)     7625 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/server_side/scripts/sqlite.sql
--rw-rw-r--   0 david     (1000) david     (1000)     1453 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/server_side/scripts/objects.php
--rw-rw-r--   0 david     (1000) david     (1000)     2235 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/server_side/scripts/ids-objects.php
--rw-rw-r--   0 david     (1000) david     (1000)    14515 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/server_side/select_rows.html
--rw-rw-r--   0 david     (1000) david     (1000)    14599 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/server_side/jsonp.html
--rw-rw-r--   0 david     (1000) david     (1000)    21611 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/server_side/pipeline.html
--rw-rw-r--   0 david     (1000) david     (1000)    14230 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/server_side/simple.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/plug-ins/
--rw-rw-r--   0 david     (1000) david     (1000)    55974 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/plug-ins/dom_sort.html
--rw-rw-r--   0 david     (1000) david     (1000)    24396 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/plug-ins/sorting_manual.html
--rw-rw-r--   0 david     (1000) david     (1000)     2652 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/plug-ins/index.html
--rw-rw-r--   0 david     (1000) david     (1000)    24277 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/plug-ins/sorting_auto.html
--rw-rw-r--   0 david     (1000) david     (1000)    25340 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/plug-ins/api.html
--rw-rw-r--   0 david     (1000) david     (1000)    25157 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/plug-ins/range_filtering.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/api/
--rw-rw-r--   0 david     (1000) david     (1000)    24896 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/api/highlight.html
--rw-rw-r--   0 david     (1000) david     (1000)    24397 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/api/counter_columns.html
--rw-rw-r--   0 david     (1000) david     (1000)    24173 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/api/select_row.html
--rw-rw-r--   0 david     (1000) david     (1000)    17340 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/api/row_details.html
--rw-rw-r--   0 david     (1000) david     (1000)    53252 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/api/form.html
--rw-rw-r--   0 david     (1000) david     (1000)     3069 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/api/index.html
--rw-rw-r--   0 david     (1000) david     (1000)    24783 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/api/api_in_init.html
--rw-rw-r--   0 david     (1000) david     (1000)    14328 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/api/add_row.html
--rw-rw-r--   0 david     (1000) david     (1000)    25203 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/api/tabs_and_scrolling.html
--rw-rw-r--   0 david     (1000) david     (1000)    25725 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/api/multi_filter.html
--rw-rw-r--   0 david     (1000) david     (1000)    28286 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/api/regex.html
--rw-rw-r--   0 david     (1000) david     (1000)    27188 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/api/multi_filter_select.html
--rw-rw-r--   0 david     (1000) david     (1000)    24832 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/api/select_single_row.html
--rw-rw-r--   0 david     (1000) david     (1000)    25049 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/api/show_hide.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/data_sources/
--rw-rw-r--   0 david     (1000) david     (1000)    14443 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/data_sources/server_side.html
--rw-rw-r--   0 david     (1000) david     (1000)    23392 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/data_sources/dom.html
--rw-rw-r--   0 david     (1000) david     (1000)     2609 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/data_sources/index.html
--rw-rw-r--   0 david     (1000) david     (1000)    14149 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/data_sources/ajax.html
--rw-rw-r--   0 david     (1000) david     (1000)    20167 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/data_sources/js_array.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/advanced_init/
--rw-rw-r--   0 david     (1000) david     (1000)    23502 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/advanced_init/events_live.html
--rw-rw-r--   0 david     (1000) david     (1000)    23643 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/advanced_init/length_menu.html
--rw-rw-r--   0 david     (1000) david     (1000)    24076 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/advanced_init/dom_multiple_elements.html
--rw-rw-r--   0 david     (1000) david     (1000)    24442 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/advanced_init/column_render.html
--rw-rw-r--   0 david     (1000) david     (1000)    24585 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/advanced_init/html5-data-options.html
--rw-rw-r--   0 david     (1000) david     (1000)    24767 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/advanced_init/dt_events.html
--rw-rw-r--   0 david     (1000) david     (1000)    28683 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/advanced_init/html5-data-attributes.html
--rw-rw-r--   0 david     (1000) david     (1000)    24753 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/advanced_init/object_dom_read.html
--rw-rw-r--   0 david     (1000) david     (1000)     3594 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/advanced_init/index.html
--rw-rw-r--   0 david     (1000) david     (1000)    25388 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/advanced_init/row_grouping.html
--rw-rw-r--   0 david     (1000) david     (1000)    23999 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/advanced_init/row_callback.html
--rw-rw-r--   0 david     (1000) david     (1000)    25076 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/advanced_init/complex_header.html
--rw-rw-r--   0 david     (1000) david     (1000)    23619 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/advanced_init/language_file.html
--rw-rw-r--   0 david     (1000) david     (1000)    24459 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/advanced_init/dom_toolbar.html
--rw-rw-r--   0 david     (1000) david     (1000)    24382 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/advanced_init/sort_direction_control.html
--rw-rw-r--   0 david     (1000) david     (1000)    23678 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/advanced_init/defaults.html
--rw-rw-r--   0 david     (1000) david     (1000)    23622 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/advanced_init/footer_callback.html
--rw-rw-r--   0 david     (1000) david     (1000)    10294 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/index.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/styling/
--rw-rw-r--   0 david     (1000) david     (1000)    23004 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/styling/no-classes.html
--rw-rw-r--   0 david     (1000) david     (1000)    24301 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/styling/bootstrap.html
--rw-rw-r--   0 david     (1000) david     (1000)     3226 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/styling/index.html
--rw-rw-r--   0 david     (1000) david     (1000)     1199 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/styling/hover.html
--rw-rw-r--   0 david     (1000) david     (1000)    23029 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/styling/row-border.html
--rw-rw-r--   0 david     (1000) david     (1000)    23182 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/styling/order-column.html
--rw-rw-r--   0 david     (1000) david     (1000)    23058 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/styling/compact.html
--rw-rw-r--   0 david     (1000) david     (1000)    22943 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/styling/stripe.html
--rw-rw-r--   0 david     (1000) david     (1000)    24682 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/styling/jqueryUI.html
--rw-rw-r--   0 david     (1000) david     (1000)    23972 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/styling/display.html
--rw-rw-r--   0 david     (1000) david     (1000)    24287 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/styling/foundation.html
--rw-rw-r--   0 david     (1000) david     (1000)    23019 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/styling/cell-border.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/ajax/
--rw-rw-r--   0 david     (1000) david     (1000)    14992 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/ajax/deep.html
--rw-rw-r--   0 david     (1000) david     (1000)    14784 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/ajax/custom_data_property.html
--rw-rw-r--   0 david     (1000) david     (1000)    15365 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/ajax/null_data_source.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/ajax/data/
--rw-rw-r--   0 david     (1000) david     (1000)    18795 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/ajax/data/orthogonal.txt
--rw-rw-r--   0 david     (1000) david     (1000)    11897 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/ajax/data/objects_root_array.txt
--rw-rw-r--   0 david     (1000) david     (1000)    10207 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/ajax/data/arrays.txt
--rw-rw-r--   0 david     (1000) david     (1000)    18871 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/ajax/data/arrays_subobjects.txt
--rw-rw-r--   0 david     (1000) david     (1000)    10207 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/ajax/data/arrays_custom_prop.txt
--rw-rw-r--   0 david     (1000) david     (1000)    18016 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/ajax/data/objects_deep.txt
--rw-rw-r--   0 david     (1000) david     (1000)    13741 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/ajax/data/objects.txt
--rw-rw-r--   0 david     (1000) david     (1000)    17218 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/ajax/data/objects_subarrays.txt
--rw-rw-r--   0 david     (1000) david     (1000)    15146 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/ajax/custom_data_flat.html
--rw-rw-r--   0 david     (1000) david     (1000)    14669 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/ajax/orthogonal-data.html
--rw-rw-r--   0 david     (1000) david     (1000)     3064 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/ajax/index.html
--rw-rw-r--   0 david     (1000) david     (1000)    14617 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/ajax/objects.html
--rw-rw-r--   0 david     (1000) david     (1000)    14210 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/ajax/defer_render.html
--rw-rw-r--   0 david     (1000) david     (1000)    14636 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/ajax/simple.html
--rw-rw-r--   0 david     (1000) david     (1000)    15854 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/ajax/objects_subarrays.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/basic_init/
--rw-rw-r--   0 david     (1000) david     (1000)    17148 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/basic_init/multiple_tables.html
--rw-rw-r--   0 david     (1000) david     (1000)    28003 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/basic_init/scroll_x.html
--rw-rw-r--   0 david     (1000) david     (1000)    23946 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/basic_init/table_sorting.html
--rw-rw-r--   0 david     (1000) david     (1000)    24681 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/basic_init/comma-decimal.html
--rw-rw-r--   0 david     (1000) david     (1000)    25952 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/basic_init/dom.html
--rw-rw-r--   0 david     (1000) david     (1000)    23771 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/basic_init/language.html
--rw-rw-r--   0 david     (1000) david     (1000)     3372 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/basic_init/index.html
--rw-rw-r--   0 david     (1000) david     (1000)    24745 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/basic_init/state_save.html
--rw-rw-r--   0 david     (1000) david     (1000)    23491 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/basic_init/scroll_y_theme.html
--rw-rw-r--   0 david     (1000) david     (1000)    24204 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/basic_init/scroll_y.html
--rw-rw-r--   0 david     (1000) david     (1000)    24631 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/basic_init/complex_header.html
--rw-rw-r--   0 david     (1000) david     (1000)    23014 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/basic_init/zero_configuration.html
--rw-rw-r--   0 david     (1000) david     (1000)    23440 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/basic_init/flexible_width.html
--rw-rw-r--   0 david     (1000) david     (1000)    27390 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/basic_init/scroll_xy.html
--rw-rw-r--   0 david     (1000) david     (1000)    22874 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/basic_init/multi_col_sort.html
--rw-rw-r--   0 david     (1000) david     (1000)    24161 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/basic_init/hidden_columns.html
--rw-rw-r--   0 david     (1000) david     (1000)    23167 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/basic_init/filter_only.html
--rw-rw-r--   0 david     (1000) david     (1000)    24819 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/basic_init/alt_pagination.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/resources/
--rw-rw-r--   0 david     (1000) david     (1000)     2881 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/resources/demo.js
--rw-rw-r--   0 david     (1000) david     (1000)      709 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/resources/details_open.png
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/resources/syntax/
--rw-rw-r--   0 david     (1000) david     (1000)    82302 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/resources/syntax/shCore.js
--rw-rw-r--   0 david     (1000) david     (1000)    10098 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/resources/syntax/shCore.css
--rw-rw-r--   0 david     (1000) david     (1000)     1061 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/resources/syntax/Syntax Highlighter license
--rw-rw-r--   0 david     (1000) david     (1000)      212 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/resources/examples.php
--rw-rw-r--   0 david     (1000) david     (1000)     5734 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/resources/demo.css
--rw-rw-r--   0 david     (1000) david     (1000)      686 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/examples/resources/details_close.png
--rw-rw-r--   0 david     (1000) david     (1000)     1096 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/Contributing.md
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/FixedColumns/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/FixedColumns/examples/
--rw-rw-r--   0 david     (1000) david     (1000)    22152 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/FixedColumns/examples/bootstrap.html
--rw-rw-r--   0 david     (1000) david     (1000)    21099 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/FixedColumns/examples/two_columns.html
--rw-rw-r--   0 david     (1000) david     (1000)    18293 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/FixedColumns/examples/rowspan.html
--rw-rw-r--   0 david     (1000) david     (1000)     3564 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/FixedColumns/examples/index.html
--rw-rw-r--   0 david     (1000) david     (1000)    21794 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/FixedColumns/examples/size_fluid.html
--rw-rw-r--   0 david     (1000) david     (1000)    21367 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/FixedColumns/examples/left_right_columns.html
--rw-rw-r--   0 david     (1000) david     (1000)    22185 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/FixedColumns/examples/css_size.html
--rw-rw-r--   0 david     (1000) david     (1000)    21801 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/FixedColumns/examples/size_fixed.html
--rw-rw-r--   0 david     (1000) david     (1000)    22394 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/FixedColumns/examples/colvis.html
--rw-rw-r--   0 david     (1000) david     (1000)    21377 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/FixedColumns/examples/right_column.html
--rw-rw-r--   0 david     (1000) david     (1000)    22483 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/FixedColumns/examples/col_filter.html
--rw-rw-r--   0 david     (1000) david     (1000)    23755 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/FixedColumns/examples/index_column.html
--rw-rw-r--   0 david     (1000) david     (1000)     7602 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/FixedColumns/examples/server-side-processing.html
--rw-rw-r--   0 david     (1000) david     (1000)    21676 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/FixedColumns/examples/simple.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/FixedColumns/css/
--rw-rw-r--   0 david     (1000) david     (1000)      517 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/FixedColumns/css/dataTables.fixedColumns.css
--rw-rw-r--   0 david     (1000) david     (1000)      317 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/FixedColumns/css/dataTables.fixedColumns.min.css
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/FixedColumns/js/
--rw-rw-r--   0 david     (1000) david     (1000)    14107 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/FixedColumns/js/dataTables.fixedColumns.min.js
--rw-rw-r--   0 david     (1000) david     (1000)    40727 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/FixedColumns/js/dataTables.fixedColumns.js
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/
--rw-rw-r--   0 david     (1000) david     (1000)     1331 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/Readme.txt
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/images/
--rw-rw-r--   0 david     (1000) david     (1000)      944 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/images/background.png
--rw-rw-r--   0 david     (1000) david     (1000)     2786 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/images/pdf_hover.png
--rwxrwxr-x   0 david     (1000) david     (1000)     2797 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/images/copy_hover.png
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/images/psd/
--rwxrwxr-x   0 david     (1000) david     (1000)   104729 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/images/psd/copy document.psd
--rwxrwxr-x   0 david     (1000) david     (1000)  1090645 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/images/psd/file_types.psd
--rwxrwxr-x   0 david     (1000) david     (1000)   119952 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/images/psd/printer.psd
--rw-rw-r--   0 david     (1000) david     (1000)    25792 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/images/psd/collection.psd
--rwxrwxr-x   0 david     (1000) david     (1000)     1607 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/images/csv.png
--rwxrwxr-x   0 david     (1000) david     (1000)     2230 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/images/print_hover.png
--rw-rw-r--   0 david     (1000) david     (1000)     4325 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/images/pdf.png
--rwxrwxr-x   0 david     (1000) david     (1000)     1641 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/images/xls.png
--rw-rw-r--   0 david     (1000) david     (1000)     1194 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/images/collection_hover.png
--rw-rw-r--   0 david     (1000) david     (1000)     1166 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/images/collection.png
--rwxrwxr-x   0 david     (1000) david     (1000)     2061 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/images/xls_hover.png
--rwxrwxr-x   0 david     (1000) david     (1000)     2184 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/images/copy.png
--rwxrwxr-x   0 david     (1000) david     (1000)     1854 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/images/csv_hover.png
--rwxrwxr-x   0 david     (1000) david     (1000)     2123 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/images/print.png
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/examples/
--rw-rw-r--   0 david     (1000) david     (1000)    10334 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/examples/multiple_tables.html
--rw-rw-r--   0 david     (1000) david     (1000)    17426 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/examples/pdf_message.html
--rw-rw-r--   0 david     (1000) david     (1000)    17316 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/examples/alter_buttons.html
--rw-rw-r--   0 david     (1000) david     (1000)    18515 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/examples/bootstrap.html
--rw-rw-r--   0 david     (1000) david     (1000)    17856 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/examples/select_os.html
--rw-rw-r--   0 david     (1000) david     (1000)     9072 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/examples/select_column.html
--rw-rw-r--   0 david     (1000) david     (1000)    17823 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/examples/select_multi.html
--rw-rw-r--   0 david     (1000) david     (1000)    17468 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/examples/swf_path.html
--rw-rw-r--   0 david     (1000) david     (1000)     3701 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/examples/index.html
--rw-rw-r--   0 david     (1000) david     (1000)    17508 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/examples/select_single.html
--rw-rw-r--   0 david     (1000) david     (1000)    18017 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/examples/button_text.html
--rw-rw-r--   0 david     (1000) david     (1000)    17446 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/examples/new_init.html
--rw-rw-r--   0 david     (1000) david     (1000)    17339 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/examples/multi_instance.html
--rw-rw-r--   0 david     (1000) david     (1000)     7495 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/examples/ajax.html
--rw-rw-r--   0 david     (1000) david     (1000)    18480 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/examples/plug-in.html
--rw-rw-r--   0 david     (1000) david     (1000)    17516 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/examples/jqueryui.html
--rw-rw-r--   0 david     (1000) david     (1000)    17195 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/examples/defaults.html
--rw-rw-r--   0 david     (1000) david     (1000)    17688 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/examples/collection.html
--rw-rw-r--   0 david     (1000) david     (1000)    17307 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/examples/simple.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/swf/
--rw-rw-r--   0 david     (1000) david     (1000)     2232 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/swf/copy_csv_xls.swf
--rw-rw-r--   0 david     (1000) david     (1000)    58845 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/swf/copy_csv_xls_pdf.swf
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/css/
--rwxrwxr-x   0 david     (1000) david     (1000)    10617 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/css/dataTables.tableTools.css
--rw-rw-r--   0 david     (1000) david     (1000)     6601 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/css/dataTables.tableTools.min.css
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/js/
--rwxrwxr-x   0 david     (1000) david     (1000)    84214 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/js/dataTables.tableTools.js
--rw-rw-r--   0 david     (1000) david     (1000)    31619 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/TableTools/js/dataTables.tableTools.min.js
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Scroller/
--rw-rw-r--   0 david     (1000) david     (1000)     2251 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Scroller/Readme.txt
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Scroller/images/
--rw-rw-r--   0 david     (1000) david     (1000)     1013 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Scroller/images/loading-background.png
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Scroller/examples/
--rw-rw-r--   0 david     (1000) david     (1000)     7943 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Scroller/examples/server-side_processing.html
--rw-rw-r--   0 david     (1000) david     (1000)     6111 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Scroller/examples/api_scrolling.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Scroller/examples/data/
--rw-rw-r--   0 david     (1000) david     (1000)   142087 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Scroller/examples/data/2500.txt
--rw-rw-r--   0 david     (1000) david     (1000)     1684 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Scroller/examples/data/ssp.php
--rw-rw-r--   0 david     (1000) david     (1000)     6557 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Scroller/examples/large_js_source.html
--rw-rw-r--   0 david     (1000) david     (1000)     3846 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Scroller/examples/index.html
--rw-rw-r--   0 david     (1000) david     (1000)     6186 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Scroller/examples/state_saving.html
--rw-rw-r--   0 david     (1000) david     (1000)     6602 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Scroller/examples/simple.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Scroller/css/
--rw-rw-r--   0 david     (1000) david     (1000)      572 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Scroller/css/dataTables.scroller.min.css
--rw-rw-r--   0 david     (1000) david     (1000)      710 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Scroller/css/dataTables.scroller.css
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Scroller/js/
--rw-rw-r--   0 david     (1000) david     (1000)    37984 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Scroller/js/dataTables.scroller.js
--rw-rw-r--   0 david     (1000) david     (1000)    10485 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Scroller/js/dataTables.scroller.min.js
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColVis/
--rw-rw-r--   0 david     (1000) david     (1000)     1259 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColVis/Readme.txt
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColVis/examples/
--rw-rw-r--   0 david     (1000) david     (1000)    16882 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColVis/examples/exclude_columns.html
--rw-rw-r--   0 david     (1000) david     (1000)    16967 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColVis/examples/restore.html
--rw-rw-r--   0 david     (1000) david     (1000)     3217 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColVis/examples/index.html
--rw-rw-r--   0 david     (1000) david     (1000)    16901 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColVis/examples/title_callback.html
--rw-rw-r--   0 david     (1000) david     (1000)    17030 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColVis/examples/new_init.html
--rw-rw-r--   0 david     (1000) david     (1000)    16697 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColVis/examples/button_order.html
--rw-rw-r--   0 david     (1000) david     (1000)    10021 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColVis/examples/two_tables.html
--rw-rw-r--   0 david     (1000) david     (1000)    17387 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColVis/examples/group_columns.html
--rw-rw-r--   0 david     (1000) david     (1000)    17456 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColVis/examples/jqueryui.html
--rw-rw-r--   0 david     (1000) david     (1000)    16682 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColVis/examples/text.html
--rw-rw-r--   0 david     (1000) david     (1000)    16804 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColVis/examples/mouseover.html
--rw-rw-r--   0 david     (1000) david     (1000)    16835 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColVis/examples/simple.html
--rw-rw-r--   0 david     (1000) david     (1000)    11366 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColVis/examples/two_tables_identical.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColVis/css/
--rwxrwxr-x   0 david     (1000) david     (1000)     5824 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColVis/css/dataTables.colVis.css
--rw-rw-r--   0 david     (1000) david     (1000)     4376 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColVis/css/dataTables.colVis.min.css
--rw-rw-r--   0 david     (1000) david     (1000)      316 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColVis/css/dataTables.colvis.jqueryui.css
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColVis/js/
--rw-rw-r--   0 david     (1000) david     (1000)     9805 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColVis/js/dataTables.colVis.min.js
--rwxrwxr-x   0 david     (1000) david     (1000)    26545 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColVis/js/dataTables.colVis.js
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/FixedHeader/
--rw-rw-r--   0 david     (1000) david     (1000)     1404 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/FixedHeader/Readme.txt
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/FixedHeader/examples/
--rw-rw-r--   0 david     (1000) david     (1000)    16321 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/FixedHeader/examples/header_footer.html
--rw-rw-r--   0 david     (1000) david     (1000)     2893 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/FixedHeader/examples/index.html
--rw-rw-r--   0 david     (1000) david     (1000)     9731 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/FixedHeader/examples/two_tables.html
--rw-rw-r--   0 david     (1000) david     (1000)    16702 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/FixedHeader/examples/zIndexes.html
--rw-rw-r--   0 david     (1000) david     (1000)     8406 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/FixedHeader/examples/top_left_right.html
--rw-rw-r--   0 david     (1000) david     (1000)    16589 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/FixedHeader/examples/simple.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/FixedHeader/css/
--rw-rw-r--   0 david     (1000) david     (1000)       87 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/FixedHeader/css/dataTables.fixedHeader.min.css
--rw-rw-r--   0 david     (1000) david     (1000)       97 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/FixedHeader/css/dataTables.fixedHeader.css
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/FixedHeader/js/
--rw-rw-r--   0 david     (1000) david     (1000)    29308 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/FixedHeader/js/dataTables.fixedHeader.js
--rw-rw-r--   0 david     (1000) david     (1000)    12590 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/FixedHeader/js/dataTables.fixedHeader.min.js
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/KeyTable/
--rw-rw-r--   0 david     (1000) david     (1000)     1334 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/KeyTable/Readme.txt
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/KeyTable/examples/
--rw-rw-r--   0 david     (1000) david     (1000)    19576 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/KeyTable/examples/events.html
--rw-rw-r--   0 david     (1000) david     (1000)     2737 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/KeyTable/examples/index.html
--rw-rw-r--   0 david     (1000) david     (1000)    15959 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/KeyTable/examples/html.html
--rw-rw-r--   0 david     (1000) david     (1000)    16257 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/KeyTable/examples/scrolling.html
--rw-rw-r--   0 david     (1000) david     (1000)    16133 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/KeyTable/examples/simple.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/KeyTable/css/
--rw-rw-r--   0 david     (1000) david     (1000)      107 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/KeyTable/css/dataTables.keyTable.css
--rw-rw-r--   0 david     (1000) david     (1000)       95 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/KeyTable/css/dataTables.keyTable.min.css
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/KeyTable/js/
--rw-rw-r--   0 david     (1000) david     (1000)     6663 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/KeyTable/js/dataTables.keyTable.min.js
--rw-rw-r--   0 david     (1000) david     (1000)    29477 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/KeyTable/js/dataTables.keyTable.js
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/AutoFill/
--rw-rw-r--   0 david     (1000) david     (1000)     1332 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/AutoFill/Readme.txt
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/AutoFill/images/
--rw-rw-r--   0 david     (1000) david     (1000)     1040 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/AutoFill/images/filler.png
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/AutoFill/examples/
--rw-rw-r--   0 david     (1000) david     (1000)    16578 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/AutoFill/examples/columns.html
--rw-rw-r--   0 david     (1000) david     (1000)    16597 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/AutoFill/examples/fill-both.html
--rw-rw-r--   0 david     (1000) david     (1000)     2705 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/AutoFill/examples/index.html
--rw-rw-r--   0 david     (1000) david     (1000)    16883 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/AutoFill/examples/complete-callback.html
--rw-rw-r--   0 david     (1000) david     (1000)    17417 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/AutoFill/examples/step-callback.html
--rw-rw-r--   0 david     (1000) david     (1000)    16544 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/AutoFill/examples/fill-horizontal.html
--rw-rw-r--   0 david     (1000) david     (1000)    16270 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/AutoFill/examples/scrolling.html
--rw-rw-r--   0 david     (1000) david     (1000)    16348 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/AutoFill/examples/simple.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/AutoFill/css/
--rw-rw-r--   0 david     (1000) david     (1000)      493 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/AutoFill/css/dataTables.autoFill.css
--rw-rw-r--   0 david     (1000) david     (1000)      344 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/AutoFill/css/dataTables.autoFill.min.css
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/AutoFill/js/
--rw-rw-r--   0 david     (1000) david     (1000)     9046 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/AutoFill/js/dataTables.autoFill.min.js
--rwxrwxr-x   0 david     (1000) david     (1000)    22645 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/AutoFill/js/dataTables.autoFill.js
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColReorder/
--rw-rw-r--   0 david     (1000) david     (1000)     1302 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColReorder/Readme.txt
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColReorder/images/
--rw-rw-r--   0 david     (1000) david     (1000)     1885 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColReorder/images/insert.png
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColReorder/examples/
--rw-rw-r--   0 david     (1000) david     (1000)    17175 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColReorder/examples/fixedheader.html
--rw-rw-r--   0 david     (1000) david     (1000)     7323 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColReorder/examples/server_side.html
--rw-rw-r--   0 david     (1000) david     (1000)    17264 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColReorder/examples/reset.html
--rw-rw-r--   0 david     (1000) david     (1000)    16914 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColReorder/examples/realtime.html
--rw-rw-r--   0 david     (1000) david     (1000)    22302 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColReorder/examples/fixedcolumns.html
--rw-rw-r--   0 david     (1000) david     (1000)     3382 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColReorder/examples/index.html
--rw-rw-r--   0 david     (1000) david     (1000)    16817 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColReorder/examples/state_save.html
--rw-rw-r--   0 david     (1000) david     (1000)    16851 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColReorder/examples/alt_insert.html
--rw-rw-r--   0 david     (1000) david     (1000)    16774 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColReorder/examples/new_init.html
--rw-rw-r--   0 david     (1000) david     (1000)    17257 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColReorder/examples/colvis.html
--rw-rw-r--   0 david     (1000) david     (1000)    16857 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColReorder/examples/predefined.html
--rw-rw-r--   0 david     (1000) david     (1000)    17593 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColReorder/examples/jqueryui.html
--rw-rw-r--   0 david     (1000) david     (1000)    17855 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColReorder/examples/col_filter.html
--rw-rw-r--   0 david     (1000) david     (1000)    16785 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColReorder/examples/scrolling.html
--rw-rw-r--   0 david     (1000) david     (1000)    17084 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColReorder/examples/simple.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColReorder/css/
--rw-rw-r--   0 david     (1000) david     (1000)      224 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColReorder/css/dataTables.colReorder.css
--rw-rw-r--   0 david     (1000) david     (1000)      139 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColReorder/css/dataTables.colReorder.min.css
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColReorder/js/
--rwxrwxr-x   0 david     (1000) david     (1000)    36465 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColReorder/js/dataTables.colReorder.js
--rw-rw-r--   0 david     (1000) david     (1000)    11006 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/ColReorder/js/dataTables.colReorder.min.js
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Responsive/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Responsive/examples/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Responsive/examples/display-control/
--rw-rw-r--   0 david     (1000) david     (1000)    10254 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Responsive/examples/display-control/classes.html
--rw-rw-r--   0 david     (1000) david     (1000)    21758 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Responsive/examples/display-control/auto.html
--rw-rw-r--   0 david     (1000) david     (1000)     2721 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Responsive/examples/display-control/index.html
--rw-rw-r--   0 david     (1000) david     (1000)    22131 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Responsive/examples/display-control/fixedHeader.html
--rw-rw-r--   0 david     (1000) david     (1000)     8479 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Responsive/examples/display-control/init-classes.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Responsive/examples/initialisation/
--rw-rw-r--   0 david     (1000) david     (1000)     2778 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Responsive/examples/initialisation/index.html
--rw-rw-r--   0 david     (1000) david     (1000)    22032 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Responsive/examples/initialisation/option.html
--rw-rw-r--   0 david     (1000) david     (1000)     7980 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Responsive/examples/initialisation/ajax.html
--rw-rw-r--   0 david     (1000) david     (1000)    21631 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Responsive/examples/initialisation/className.html
--rw-rw-r--   0 david     (1000) david     (1000)    22064 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Responsive/examples/initialisation/new.html
--rw-rw-r--   0 david     (1000) david     (1000)    22071 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Responsive/examples/initialisation/default.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Responsive/examples/child-rows/
--rw-rw-r--   0 david     (1000) david     (1000)    23161 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Responsive/examples/child-rows/custom-renderer.html
--rw-rw-r--   0 david     (1000) david     (1000)    21613 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Responsive/examples/child-rows/column-control.html
--rw-rw-r--   0 david     (1000) david     (1000)     3666 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Responsive/examples/child-rows/index.html
--rw-rw-r--   0 david     (1000) david     (1000)    21759 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Responsive/examples/child-rows/disable-child-rows.html
--rw-rw-r--   0 david     (1000) david     (1000)    20959 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Responsive/examples/child-rows/right-column.html
--rw-rw-r--   0 david     (1000) david     (1000)    20956 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Responsive/examples/child-rows/whole-row-control.html
--rw-rw-r--   0 david     (1000) david     (1000)     3561 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Responsive/examples/index.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Responsive/examples/styling/
--rw-rw-r--   0 david     (1000) david     (1000)    22851 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Responsive/examples/styling/bootstrap.html
--rw-rw-r--   0 david     (1000) david     (1000)     2294 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Responsive/examples/styling/index.html
--rw-rw-r--   0 david     (1000) david     (1000)    22323 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Responsive/examples/styling/foundation.html
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Responsive/css/
--rw-rw-r--   0 david     (1000) david     (1000)     1870 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Responsive/css/dataTables.responsive.scss
--rw-rw-r--   0 david     (1000) david     (1000)     2444 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Responsive/css/dataTables.responsive.css
--rw-rw-r--   0 david     (1000) david     (1000)        0 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Responsive/Readme.md
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Responsive/js/
--rw-rw-r--   0 david     (1000) david     (1000)    23611 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Responsive/js/dataTables.responsive.js
--rw-rw-r--   0 david     (1000) david     (1000)     6955 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/extensions/Responsive/js/dataTables.responsive.min.js
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/media/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/media/images/
--rw-rw-r--   0 david     (1000) david     (1000)      160 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/media/images/sort_asc.png
--rw-rw-r--   0 david     (1000) david     (1000)      201 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/media/images/sort_both.png
--rw-rw-r--   0 david     (1000) david     (1000)      345 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/media/images/back_disabled.png
--rw-rw-r--   0 david     (1000) david     (1000)      444 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/media/images/forward_enabled_hover.png
--rw-rw-r--   0 david     (1000) david     (1000)      445 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/media/images/forward_enabled.png
--rw-rw-r--   0 david     (1000) david     (1000)      148 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/media/images/sort_asc_disabled.png
--rw-rw-r--   0 david     (1000) david     (1000)      453 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/media/images/back_enabled.png
--rw-rw-r--   0 david     (1000) david     (1000)      450 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/media/images/back_enabled_hover.png
--rw-rw-r--   0 david     (1000) david     (1000)      894 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/media/images/favicon.ico
--rw-rw-r--   0 david     (1000) david     (1000)    27490 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/media/images/Sorting icons.psd
--rw-rw-r--   0 david     (1000) david     (1000)      335 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/media/images/forward_disabled.png
--rw-rw-r--   0 david     (1000) david     (1000)      158 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/media/images/sort_desc.png
--rw-rw-r--   0 david     (1000) david     (1000)      146 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/media/images/sort_desc_disabled.png
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/media/css/
--rw-rw-r--   0 david     (1000) david     (1000)    17203 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/media/css/jquery.dataTables.css
--rw-rw-r--   0 david     (1000) david     (1000)    14245 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/media/css/jquery.dataTables_themeroller.css
--rw-rw-r--   0 david     (1000) david     (1000)    15128 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/media/css/jquery.dataTables.min.css
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/media/js/
--rw-rw-r--   0 david     (1000) david     (1000)    78980 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/media/js/jquery.dataTables.min.js
--rw-rw-r--   0 david     (1000) david     (1000)    95785 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/media/js/jquery.js
--rw-rw-r--   0 david     (1000) david     (1000)   435687 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/media/js/jquery.dataTables.js
--rw-rw-r--   0 david     (1000) david     (1000)     2621 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/Readme.md
--rw-rw-r--   0 david     (1000) david     (1000)      806 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/dataTables.jquery.json
--rw-rw-r--   0 david     (1000) david     (1000)     1088 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/license.txt
--rw-rw-r--   0 david     (1000) david     (1000)      950 2015-12-19 19:43:26.000000 hxl-proxy-1.9.1/hxl_proxy/static/dataTables/package.json
--rw-rw-r--   0 david     (1000) david     (1000)    27007 2018-06-29 14:15:31.000000 hxl-proxy-1.9.1/hxl_proxy/controllers.py
--rw-rw-r--   0 david     (1000) david     (1000)     1160 2018-07-05 18:56:48.000000 hxl-proxy-1.9.1/hxl_proxy/__init__.py
--rwxrwxr-x   0 david     (1000) david     (1000)      858 2018-07-05 18:56:48.000000 hxl-proxy-1.9.1/setup.py
--rw-rw-r--   0 david     (1000) david     (1000)       38 2018-07-05 18:57:36.000000 hxl-proxy-1.9.1/setup.cfg
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-23 20:32:22.019588 hxl-proxy-2.0/
+-rw-rw-r--   0 david     (1001) david     (1001)     1210 2022-10-28 23:21:23.000000 hxl-proxy-2.0/LICENSE.md
+-rw-rw-r--   0 david     (1001) david     (1001)       77 2022-10-28 23:21:23.000000 hxl-proxy-2.0/MANIFEST.in
+-rw-rw-r--   0 david     (1001) david     (1001)     3514 2023-05-23 20:32:22.019588 hxl-proxy-2.0/PKG-INFO
+-rw-rw-r--   0 david     (1001) david     (1001)     3209 2022-10-28 23:21:23.000000 hxl-proxy-2.0/README.md
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-23 20:32:22.003588 hxl-proxy-2.0/hxl_proxy/
+-rw-rw-r--   0 david     (1001) david     (1001)     4356 2023-05-23 20:30:05.000000 hxl-proxy-2.0/hxl_proxy/__init__.py
+-rw-rw-r--   0 david     (1001) david     (1001)     3194 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/admin.py
+-rw-rw-r--   0 david     (1001) david     (1001)     1925 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/auth.py
+-rw-rw-r--   0 david     (1001) david     (1001)     1660 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/caching.py
+-rw-rw-r--   0 david     (1001) david     (1001)    51713 2023-05-23 20:28:31.000000 hxl-proxy-2.0/hxl_proxy/controllers.py
+-rw-rw-r--   0 david     (1001) david     (1001)    12898 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/dao.py
+-rw-rw-r--   0 david     (1001) david     (1001)      352 2022-11-25 16:22:47.000000 hxl-proxy-2.0/hxl_proxy/default_config.py
+-rw-rw-r--   0 david     (1001) david     (1001)     1878 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/exceptions.py
+-rw-rw-r--   0 david     (1001) david     (1001)    14423 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/filters.py
+-rw-rw-r--   0 david     (1001) david     (1001)     4223 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/pcodes.py
+-rw-rw-r--   0 david     (1001) david     (1001)      929 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/preview.py
+-rw-rw-r--   0 david     (1001) david     (1001)     5398 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/recipes.py
+-rw-rw-r--   0 david     (1001) david     (1001)     1465 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/reverse_proxied.py
+-rw-rw-r--   0 david     (1001) david     (1001)      929 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/schema-mysql.sql
+-rw-rw-r--   0 david     (1001) david     (1001)      650 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/schema-sqlite3.sql
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-23 20:32:21.999588 hxl-proxy-2.0/hxl_proxy/static/
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-23 20:32:21.999588 hxl-proxy-2.0/hxl_proxy/static/bootstrap/
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-23 20:32:22.003588 hxl-proxy-2.0/hxl_proxy/static/bootstrap/css/
+-rw-rw-r--   0 david     (1001) david     (1001)    22608 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/bootstrap/css/bootstrap-theme.css
+-rw-rw-r--   0 david     (1001) david     (1001)    43339 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/bootstrap/css/bootstrap-theme.css.map
+-rw-rw-r--   0 david     (1001) david     (1001)    19963 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/bootstrap/css/bootstrap-theme.min.css
+-rw-rw-r--   0 david     (1001) david     (1001)   141414 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/bootstrap/css/bootstrap.css
+-rw-rw-r--   0 david     (1001) david     (1001)   379710 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/bootstrap/css/bootstrap.css.map
+-rw-rw-r--   0 david     (1001) david     (1001)   117150 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/bootstrap/css/bootstrap.min.css
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-23 20:32:22.007588 hxl-proxy-2.0/hxl_proxy/static/bootstrap/fonts/
+-rw-rw-r--   0 david     (1001) david     (1001)    20127 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.eot
+-rw-rw-r--   0 david     (1001) david     (1001)   108738 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.svg
+-rw-rw-r--   0 david     (1001) david     (1001)    45404 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-r--   0 david     (1001) david     (1001)    23424 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.woff
+-rw-rw-r--   0 david     (1001) david     (1001)    18028 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.woff2
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-23 20:32:22.007588 hxl-proxy-2.0/hxl_proxy/static/bootstrap/js/
+-rw-rw-r--   0 david     (1001) david     (1001)    66732 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/bootstrap/js/bootstrap.js
+-rw-rw-r--   0 david     (1001) david     (1001)    35452 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/bootstrap/js/bootstrap.min.js
+-rw-rw-r--   0 david     (1001) david     (1001)      484 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/bootstrap/js/npm.js
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-23 20:32:22.007588 hxl-proxy-2.0/hxl_proxy/static/compat/
+-rw-rw-r--   0 david     (1001) david     (1001)     2636 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/compat/html5shiv.min.js
+-rw-rw-r--   0 david     (1001) david     (1001)      694 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/compat/ie10-viewport-bug-workaround.js
+-rw-rw-r--   0 david     (1001) david     (1001)     4377 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/compat/respond.min.js
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-23 20:32:22.007588 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/
+-rw-rw-r--   0 david     (1001) david     (1001)     3470 2023-04-04 17:11:40.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/hxl-proxy.css
+-rw-rw-r--   0 david     (1001) david     (1001)    15879 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/hxl-proxy.js
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-23 20:32:22.011588 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/
+-rw-rw-r--   0 david     (1001) david     (1001)     9448 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/android-icon-144x144.png
+-rw-rw-r--   0 david     (1001) david     (1001)    11645 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/android-icon-192x192.png
+-rw-rw-r--   0 david     (1001) david     (1001)     1960 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/android-icon-36x36.png
+-rw-rw-r--   0 david     (1001) david     (1001)     3057 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/android-icon-48x48.png
+-rw-rw-r--   0 david     (1001) david     (1001)     4171 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/android-icon-72x72.png
+-rw-rw-r--   0 david     (1001) david     (1001)     5857 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/android-icon-96x96.png
+-rw-rw-r--   0 david     (1001) david     (1001)     7317 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-114x114.png
+-rw-rw-r--   0 david     (1001) david     (1001)     7631 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-120x120.png
+-rw-rw-r--   0 david     (1001) david     (1001)     9448 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-144x144.png
+-rw-rw-r--   0 david     (1001) david     (1001)    10058 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-152x152.png
+-rw-rw-r--   0 david     (1001) david     (1001)    12668 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-180x180.png
+-rw-rw-r--   0 david     (1001) david     (1001)     2618 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-57x57.png
+-rw-rw-r--   0 david     (1001) david     (1001)     3820 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-60x60.png
+-rw-rw-r--   0 david     (1001) david     (1001)     4171 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-72x72.png
+-rw-rw-r--   0 david     (1001) david     (1001)     4491 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-76x76.png
+-rw-rw-r--   0 david     (1001) david     (1001)    12219 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-precomposed.png
+-rw-rw-r--   0 david     (1001) david     (1001)    12219 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon.png
+-rw-rw-r--   0 david     (1001) david     (1001)      281 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/browserconfig.xml
+-rw-rw-r--   0 david     (1001) david     (1001)     1249 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/favicon-16x16.png
+-rw-rw-r--   0 david     (1001) david     (1001)     1899 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/favicon-32x32.png
+-rw-rw-r--   0 david     (1001) david     (1001)     5857 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/favicon-96x96.png
+-rw-rw-r--   0 david     (1001) david     (1001)     1150 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/favicon.ico
+-rw-rw-r--   0 david     (1001) david     (1001)     1165 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/manifest.json
+-rw-rw-r--   0 david     (1001) david     (1001)     9448 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/ms-icon-144x144.png
+-rw-rw-r--   0 david     (1001) david     (1001)    10073 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/ms-icon-150x150.png
+-rw-rw-r--   0 david     (1001) david     (1001)    27390 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/ms-icon-310x310.png
+-rw-rw-r--   0 david     (1001) david     (1001)     4125 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/ms-icon-70x70.png
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-23 20:32:22.015588 hxl-proxy-2.0/hxl_proxy/static/images/
+-rw-rw-r--   0 david     (1001) david     (1001)     8850 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/images/csv-icon.png
+-rw-rw-r--   0 david     (1001) david     (1001)    13225 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/images/dropbox-logo.png
+-rw-rw-r--   0 david     (1001) david     (1001)    22085 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/images/google-drive-logo.png
+-rw-rw-r--   0 david     (1001) david     (1001)     7767 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/images/hdx-logo.png
+-rw-rw-r--   0 david     (1001) david     (1001)     2454 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/images/hxl-logo-white.png
+-rw-rw-r--   0 david     (1001) david     (1001)    55429 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/images/json-icon.png
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-23 20:32:22.015588 hxl-proxy-2.0/hxl_proxy/static/jquery/
+-rw-rw-r--   0 david     (1001) david     (1001)   240427 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/jquery/jquery-ui.min.js
+-rw-rw-r--   0 david     (1001) david     (1001)    10469 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/jquery/jquery.csv.js
+-rw-rw-r--   0 david     (1001) david     (1001)    84320 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/jquery/jquery.js
+-rw-rw-r--   0 david     (1001) david     (1001)     1291 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/jquery/jquery.ui.touch-punch.min.js
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-23 20:32:22.015588 hxl-proxy-2.0/hxl_proxy/templates/
+-rw-rw-r--   0 david     (1001) david     (1001)     4570 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/about.html
+-rw-rw-r--   0 david     (1001) david     (1001)     5224 2023-03-20 15:47:35.000000 hxl-proxy-2.0/hxl_proxy/templates/api-data-preview.html
+-rw-rw-r--   0 david     (1001) david     (1001)     4462 2023-03-20 15:47:35.000000 hxl-proxy-2.0/hxl_proxy/templates/api-from-spec.html
+-rw-rw-r--   0 david     (1001) david     (1001)     3506 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/data-advanced.html
+-rw-rw-r--   0 david     (1001) david     (1001)     2227 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/data-logs.html
+-rw-rw-r--   0 david     (1001) david     (1001)     9122 2023-04-04 17:11:40.000000 hxl-proxy-2.0/hxl_proxy/templates/data-recipe.html
+-rw-rw-r--   0 david     (1001) david     (1001)     5109 2023-03-20 15:47:35.000000 hxl-proxy-2.0/hxl_proxy/templates/data-source.html
+-rw-rw-r--   0 david     (1001) david     (1001)     6758 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/data-tagger.html
+-rw-rw-r--   0 david     (1001) david     (1001)     2547 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/data-view.html
+-rw-rw-r--   0 david     (1001) david     (1001)     1206 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/error.html
+-rw-rw-r--   0 david     (1001) david     (1001)     1247 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/hash.html
+-rw-rw-r--   0 david     (1001) david     (1001)     2672 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/hxl-test.html
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-23 20:32:22.019588 hxl-proxy-2.0/hxl_proxy/templates/includes/
+-rw-rw-r--   0 david     (1001) david     (1001)      153 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/admin-alert.html
+-rw-rw-r--   0 david     (1001) david     (1001)      496 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/chooser-scripts.html
+-rw-rw-r--   0 david     (1001) david     (1001)      959 2023-03-20 15:47:35.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/data-tabs.html
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-23 20:32:22.019588 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/
+-rw-rw-r--   0 david     (1001) david     (1001)     1815 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/add.html
+-rw-rw-r--   0 david     (1001) david     (1001)     1737 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/append-list.html
+-rw-rw-r--   0 david     (1001) david     (1001)     2308 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/append.html
+-rw-rw-r--   0 david     (1001) david     (1001)     5188 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/clean.html
+-rw-rw-r--   0 david     (1001) david     (1001)     6021 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/count.html
+-rw-rw-r--   0 david     (1001) david     (1001)     1510 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/cut.html
+-rw-rw-r--   0 david     (1001) david     (1001)     1258 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/dedup.html
+-rw-rw-r--   0 david     (1001) david     (1001)     2166 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/expand.html
+-rw-rw-r--   0 david     (1001) david     (1001)     1344 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/explode.html
+-rw-rw-r--   0 david     (1001) david     (1001)     1227 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/fill.html
+-rw-rw-r--   0 david     (1001) david     (1001)      630 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/filter-list.html
+-rw-rw-r--   0 david     (1001) david     (1001)      643 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/filter-selector.html
+-rw-rw-r--   0 david     (1001) david     (1001)      691 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/filter-types.j2
+-rw-rw-r--   0 david     (1001) david     (1001)     1191 2023-03-20 15:47:35.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/filter-variables.j2
+-rw-rw-r--   0 david     (1001) david     (1001)     1258 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/implode.html
+-rw-rw-r--   0 david     (1001) david     (1001)     2051 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/jsonpath.html
+-rw-rw-r--   0 david     (1001) david     (1001)      334 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/label-field-multicol.html
+-rw-rw-r--   0 david     (1001) david     (1001)      324 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/label-field.html
+-rw-rw-r--   0 david     (1001) david     (1001)     2480 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/merge.html
+-rw-rw-r--   0 david     (1001) david     (1001)     1931 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/rename.html
+-rw-rw-r--   0 david     (1001) david     (1001)     1311 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/replace-map.html
+-rw-rw-r--   0 david     (1001) david     (1001)     2192 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/replace.html
+-rw-rw-r--   0 david     (1001) david     (1001)     1240 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/select.html
+-rw-rw-r--   0 david     (1001) david     (1001)      963 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/sort.html
+-rw-rw-r--   0 david     (1001) david     (1001)     2317 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/headers.html
+-rw-rw-r--   0 david     (1001) david     (1001)      171 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/help.html
+-rw-rw-r--   0 david     (1001) david     (1001)      847 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/hxltable.html
+-rw-rw-r--   0 david     (1001) david     (1001)      259 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/messages.html
+-rw-rw-r--   0 david     (1001) david     (1001)      365 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/metadata-params.html
+-rw-rw-r--   0 david     (1001) david     (1001)     3378 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/navbar.html
+-rw-rw-r--   0 david     (1001) david     (1001)      153 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/params.html
+-rw-rw-r--   0 david     (1001) david     (1001)      790 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/postcards.html
+-rw-rw-r--   0 david     (1001) david     (1001)      142 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/recipe-form.html
+-rw-rw-r--   0 david     (1001) david     (1001)      412 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/recipe-params.html
+-rw-rw-r--   0 david     (1001) david     (1001)      443 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/scripts.html
+-rw-rw-r--   0 david     (1001) david     (1001)      368 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/selectors.html
+-rw-rw-r--   0 david     (1001) david     (1001)      182 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/source.html
+-rw-rw-r--   0 david     (1001) david     (1001)      382 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/tagger-params.html
+-rw-rw-r--   0 david     (1001) david     (1001)     1633 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/settings-user.html
+-rw-rw-r--   0 david     (1001) david     (1001)     2433 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/validate-issue.html
+-rw-rw-r--   0 david     (1001) david     (1001)     5437 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/validate-summary.html
+-rw-rw-r--   0 david     (1001) david     (1001)    16476 2023-03-20 15:47:35.000000 hxl-proxy-2.0/hxl_proxy/util.py
+-rw-rw-r--   0 david     (1001) david     (1001)     3270 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/validate.py
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-23 20:32:22.003588 hxl-proxy-2.0/hxl_proxy.egg-info/
+-rw-rw-r--   0 david     (1001) david     (1001)     3514 2023-05-23 20:32:21.000000 hxl-proxy-2.0/hxl_proxy.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1001) david     (1001)     5980 2023-05-23 20:32:21.000000 hxl-proxy-2.0/hxl_proxy.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1001) david     (1001)       64 2023-05-23 20:32:21.000000 hxl-proxy-2.0/hxl_proxy.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1001) david     (1001)        1 2022-10-29 17:11:19.000000 hxl-proxy-2.0/hxl_proxy.egg-info/not-zip-safe
+-rw-rw-r--   0 david     (1001) david     (1001)      151 2023-05-23 20:32:21.000000 hxl-proxy-2.0/hxl_proxy.egg-info/requires.txt
+-rw-rw-r--   0 david     (1001) david     (1001)       10 2023-05-23 20:32:21.000000 hxl-proxy-2.0/hxl_proxy.egg-info/top_level.txt
+-rw-rw-r--   0 david     (1001) david     (1001)       38 2023-05-23 20:32:22.019588 hxl-proxy-2.0/setup.cfg
+-rwxrwxr-x   0 david     (1001) david     (1001)     1337 2023-05-23 20:30:05.000000 hxl-proxy-2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `hxl-proxy-1.9.1/README.md` & `hxl-proxy-2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -26,18 +26,23 @@
 python setup.py test
 ```
 
 # Configuration
 
 To configure the proxy, make a copy of config.py.TEMPLATE (e.g. to config.py), and change its values as necessary. The environment variable HXL\_PROXY\_CONFIG should point to your local config file's location.  More details appear below.
 
-## Filesystem
+## Admin interface
 
-* CACHE_DIR - a directory where the proxy can cache output files. The directory must exist and be readable and writable by the web-server process.
-* REQUEST_CACHE - a file (which the proxy will create if necessary) where the proxy can cache input files. The file's directory must exist and be readable and writable by the web-server process.
+To enable the admin interface, you need to enter the MD5 hash of a password into the ADMIN_PASSWORD_MD5 field in the config file. If your password were "hello-kitty" (don't do that!), you could generate the hash like this using Python3:
+
+    $ python -c 'import hashlib; print(hashlib.md5("hello-kitty".encode("utf-8")).hexdigest())'
+
+## Caching
+
+Choose and configure your input and output caches as needed, following the examples in the config template. You may need to create local directories or databases, depending on the caching backends you choose.
 
 ## Database support
 
 ### Using SQLite3
 
 * DB_TYPE - (required) set to "sqlite3"
 * DB_FILE - (required) a file (which the proxy will create if necessary) containing a SQLite3 database of saved configurations. The file's directory must exist and be readable and writable by the web-server process.
```

### Comparing `hxl-proxy-1.9.1/hxl_proxy/preview.py` & `hxl-proxy-2.0/hxl_proxy/preview.py`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/dao.py` & `hxl-proxy-2.0/hxl_proxy/dao.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,27 +26,29 @@
 import sqlite3, mysql.connector, json, os, random, time, base64, hashlib, flask
 import hxl_proxy
 
 
 class db:
     """Low-level database functions"""
 
-    TEST_SCHEMA_FILE = os.path.join(os.path.dirname(__file__), 'schema-sqlite3.sql')
+    schema_file = hxl_proxy.app.config.get('DB_SCHEMA_FILE', 'schema-sqlite3.sql')
+
+    TEST_SCHEMA_FILE = os.path.join(os.path.dirname(__file__), schema_file)
     """The filename of the SQL schema."""
 
     type = hxl_proxy.app.config.get('DB_TYPE', 'sqlite3')
 
 
     _database = None
     """Internal connection, for testing use outside a request context."""
 
 
     @staticmethod
     def connect():
-        """Get a database connection 
+        """Get a database connection
 
         Will reuse the same connection throughout a request
         context. Uses the C{DB_FILE} Flask config option for the
         location of SQLite3 file.
 
         @return: a SQLite3 database connection
         """
@@ -89,15 +91,15 @@
             return database.cursor(dictionary=True)
         else:
             return database.cursor()
 
     @staticmethod
     def commit():
         db.connect().commit()
-        
+
     @staticmethod
     def execute_statement(statement, params=(), commit=False):
         """Execute a single SQL statement, and optionally commit.
 
         @param statement: the SQL statement to execute.
         @param params: sequence of values for any C{%s} placeholders in the statement.
         @param commit: if True, autocommit at the end of the statement (default: False)
@@ -113,15 +115,20 @@
     def execute_script(sql_statements, commit=True):
         """Execute a script of statements, and optionally commit.
         @param sql_statements: a string containing multiple SQL statements, separated by ';'
         @param commit: if True, autocommit after executing the statements (default: True)
         @return: a SQLite3 cursor object.
         """
         cursor = db.cursor()
-        cursor.executescript(sql_statements)
+        if db.type == 'mysql':
+            for _ in cursor.execute(sql_statements, multi=True):
+                pass
+        else:
+            cursor.executescript(sql_statements)
+
         if commit:
             db.commit()
         return cursor
 
     @staticmethod
     def execute_file(filename, commit=True):
         """Open a SQL file and execute it as a script.
@@ -318,7 +325,33 @@
         @return: a SQLite3 cursor object.
         """
         return db.execute_statement(
             "delete from Recipes where recipe_id=%s",
             (recipe_id,),
             commit=commit
         )
+
+    @staticmethod
+    def list():
+        """List all existing recipes, sorted in descending creation-date order"""
+        return db.fetchall("select * from Recipes order by date_created desc")
+
+
+########################################################################
+# Support functions
+########################################################################
+
+def gen_recipe_id():
+    """
+    Generate a pseudo-random, 6-character hash for use as a recipe_id.
+    """
+    salt = str(time.time() * random.random())
+    encoded_hash = hxl_proxy.util.make_md5(salt)
+    return encoded_hash[:6]
+
+def make_recipe_id():
+    """Make a unique recipe_id for a saved recipe."""
+    recipe_id = gen_recipe_id()
+    while hxl_proxy.dao.recipes.read(recipe_id):
+        recipe_id = gen_recipe_id()
+    return recipe_id
+
```

### Comparing `hxl-proxy-1.9.1/hxl_proxy/auth.py` & `hxl-proxy-2.0/hxl_proxy/auth.py`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/filters.py` & `hxl-proxy-2.0/hxl_proxy/filters.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,82 +15,93 @@
 
 # Maximum number of filters to check
 MAX_FILTER_COUNT = 99
 
 def setup_filters(recipe, data_content=None):
     """
     Open a stream to a data source URL, and create a filter pipeline based on the arguments.
-    @param recipe the GET-request recipe (uses only recipe['args']).
-    @return a HXL DataSource representing the full pipeline.
+    @param: recipe the GET-request recipe (uses only recipe.args).
+    @param data_content: a dataset uploaded directly via a POST request.
+    @returns: a HXL DataSource representing the full pipeline.
     """
 
     # null recipe or url means null source
-    if not data_content and (not recipe or not recipe['args'].get('url')):
+    if not data_content and (not recipe or not recipe.url):
         return None
 
     # Basic input source
+
+    input_options = util.make_input_options(recipe.args)
+
     if data_content:
-        source = hxl.data(io.BytesIO(data_content.encode('utf-8')))
+        source = util.hxl_data(io.BytesIO(data_content.encode('utf-8')), input_options)
     else:
-        source = hxl.data(make_tagged_input(recipe['args']))
+        try:
+            source = util.hxl_data(recipe.args["url"], input_options)
+            source.columns
+        except hxl.input.HXLTagsNotFoundException:
+            source = util.hxl_data(make_tagged_input(recipe.args, input_options), input_options)
 
     # Do we have a JSON recipe? Load it first.
-    if recipe['args'].get('recipe'):
-        source = source.recipe(recipe['args'].get('recipe'))
+    if recipe.args.get('recipe'):
+        source = source.recipe(recipe.args.get('recipe'))
 
     # Intercept missing hashtags here
     try:
         source.columns
-    except hxl.io.HXLTagsNotFoundException:
+    except hxl.input.HXLTagsNotFoundException:
         raise exceptions.RedirectException(util.data_url_for('data_tagger', recipe), 303, 'No HXL hashtags found')
 
     # Create the filter pipeline from the source
     for index in range(1, MAX_FILTER_COUNT):
-        filter = recipe['args'].get('filter%02d' % index)
+        filter = recipe.args.get('filter%02d' % index)
         if filter == 'add':
-            source = add_add_filter(source, recipe['args'], index)
+            source = add_add_filter(source, recipe.args, index)
         elif filter == 'append':
-            source = add_append_filter(source, recipe['args'], index)
+            source = add_append_filter(source, recipe.args, index)
+        elif filter == 'append-list':
+            source = add_append_list_filter(source, recipe.args, index)
         elif filter == 'clean':
-            source = add_clean_filter(source, recipe['args'], index)
+            source = add_clean_filter(source, recipe.args, index)
         elif filter == 'count':
-            source = add_count_filter(source, recipe['args'], index)
+            source = add_count_filter(source, recipe.args, index)
         elif filter == 'column' or filter == 'cut':
-            source = add_column_filter(source, recipe['args'], index)
+            source = add_column_filter(source, recipe.args, index)
         elif filter == 'dedup':
-            source = add_dedup_filter(source, recipe['args'], index)
+            source = add_dedup_filter(source, recipe.args, index)
+        elif filter == 'expand':
+            source = add_expand_filter(source, recipe.args, index)
         elif filter == 'explode':
-            source = add_explode_filter(source, recipe['args'], index)
+            source = add_explode_filter(source, recipe.args, index)
         elif filter == 'fill':
-            source = add_fill_filter(source, recipe['args'], index)
+            source = add_fill_filter(source, recipe.args, index)
+        elif filter == 'implode':
+            source = add_implode_filter(source, recipe.args, index)
         elif filter == 'jsonpath':
-            source = add_jsonpath_filter(source, recipe['args'], index)
+            source = add_jsonpath_filter(source, recipe.args, index)
         elif filter == 'merge':
-            source = add_merge_filter(source, recipe['args'], index)
+            source = add_merge_filter(source, recipe.args, index)
         elif filter == 'rename':
-            source = add_rename_filter(source, recipe['args'], index)
+            source = add_rename_filter(source, recipe.args, index)
         elif filter == 'replace':
-            source = add_replace_filter(source, recipe['args'], index)
+            source = add_replace_filter(source, recipe.args, index)
         elif filter == 'replace-map':
-            source = add_replace_map_filter(source, recipe['args'], index)
+            source = add_replace_map_filter(source, recipe.args, index)
         elif filter == 'rows' or filter == 'select':
-            source = add_row_filter(source, recipe['args'], index)
+            source = add_row_filter(source, recipe.args, index)
         elif filter == 'sort':
-            source = add_sort_filter(source, recipe['args'], index)
+            source = add_sort_filter(source, recipe.args, index)
         elif filter:
             raise Exception("Unknown filter type '{}'".format(filter))
 
     return source
 
-def make_tagged_input(args):
+def make_tagged_input(args, input_options):
     """Create the raw input, optionally using the Tagger filter."""
-    url = args.get('url')
-    sheet_index = int(args.get('sheet')) if args.get('sheet') else None
-    selector = args.get('selector', None)
-    input = hxl.io.make_input(url, sheet_index=sheet_index, verify_ssl=util.check_verify_ssl(args), selector=selector)
+    input = util.hxl_make_input(args.get("url"), input_options)
 
     # Intercept tagging as a special data input
     specs = []
     for n in range(1, 101):
         header = args.get('tagger-%02d-header' % n)
         tag = _parse_tagspec(args.get('tagger-%02d-tag' % n))
         if header and tag:
@@ -117,15 +128,31 @@
     """Add the hxlappend filter to the end of the chain."""
     exclude_columns = args.get('append-exclude-columns%02d' % index, False)
     append_sources = []
     for subindex in range(1, 100):
         append_source = args.get('append-dataset%02d-%02d' % (index, subindex))
         if append_source:
             append_sources.append(append_source)
-    return source.append(append_sources=append_sources, add_columns=(not exclude_columns))
+    row_query = args.get('append-where%02d' % index, None)
+    return source.append(
+        append_sources=append_sources,
+        add_columns=(not exclude_columns),
+        queries=row_query
+    )
+
+def add_append_list_filter(source, args, index):
+    """Add the hxlappend filter to the end of the chain with an external list."""
+    exclude_columns = args.get('append-list-exclude-columns%02d' % index, False)
+    source_list_url = args.get('append-list-url%02d' % index, None)
+    row_query = args.get('append-list-where%02d' % index, None)
+    return source.append_external_list(
+        source_list_url=source_list_url,
+        add_columns=(not exclude_columns),
+        queries=row_query
+    )
 
 def add_clean_filter(source, args, index):
     """Add the hxlclean filter to the end of the pipeline."""
     whitespace_tags = hxl.TagPattern.parse_list(args.get('clean-whitespace-tags%02d' % index, ''))
     upper_tags = hxl.TagPattern.parse_list(args.get('clean-toupper-tags%02d' % index, ''))
     lower_tags = hxl.TagPattern.parse_list(args.get('clean-tolower-tags%02d' % index, ''))
     date_tags = hxl.TagPattern.parse_list(args.get('clean-date-tags%02d' % index, ''))
@@ -186,15 +213,15 @@
             ))
         for count_type in ['sum', 'average', 'min', 'max']:
             aggregators.append(hxl.filters.Aggregator(
                 type = count_type,
                 pattern = aggregate_pattern,
                 column = hxl.model.Column.parse("#meta+" + count_type, header=count_type.title())
             ))
-    
+
     return source.count(patterns=tags, aggregators=aggregators, queries=row_query)
 
 def add_column_filter(source, args, index):
     """Add the hxlcut filter to the end of the pipeline."""
     include_tags = hxl.TagPattern.parse_list(args.get('cut-include-tags%02d' % index, []))
     exclude_tags = hxl.TagPattern.parse_list(args.get('cut-exclude-tags%02d' % index, []))
     skip_untagged = args.get('cut-skip-untagged%02d' % index, False)
@@ -205,66 +232,86 @@
     return source
 
 def add_dedup_filter(source, args, index):
     tags = args.get('dedup-tags%02d' % index, [])
     row_query = args.get('dedup-where%02d' % index, '')
     return source.dedup(tags, queries=row_query)
 
+def add_expand_filter(source, args, index):
+    tags = args.get('expand-tags%02d' % index, [])
+    separator = args.get('expand-separator%02d' % index, "|")
+    correlate = (args.get('expand-correlate%02d' % index) == 'on')
+    row_query = args.get('expand-where%02d' % index, '')
+    return source.expand_lists(
+        patterns = tags,
+        separator=separator,
+        correlate=correlate,
+        queries=row_query
+    )
+
 def add_explode_filter(source, args, index):
     return source.explode(
         args.get('explode-header-att%02d' % index, 'header'),
         args.get('explode-value-att%02d' % index, 'value')
     )
 
 def add_fill_filter(source, args, index):
     patterns = args.get('fill-patterns%02d' % index, None)
     if not patterns:
         # deprecated
         patterns = args.get('fill-pattern%02d' % index, None)
     queries = args.get('fill-where%02d' % index, None)
     return source.fill_data(patterns=patterns, queries=queries)
 
+def add_implode_filter(source, args, index):
+    return source.implode(
+        label_pattern=args.get('implode-label-pattern%02d' % index, 'header'),
+        value_pattern=args.get('implode-value-pattern%02d' % index, 'value')
+    )
+
 def add_jsonpath_filter(source, args, index):
     path = args.get('jsonpath-path%02d' % index)
     patterns = args.get('jsonpath-patterns%02d' % index, None)
     queries = args.get('jsonpath-where%02d' % index, None)
-    return source.jsonpath(path, patterns=patterns, queries=queries)
+    use_json = (args.get('jsonpath-flatten%02d' % index) != 'on')
+    return source.jsonpath(path, patterns=patterns, queries=queries, use_json=use_json)
 
 def add_merge_filter(source, args, index):
     """Add the hxlmerge filter to the end of the pipeline."""
     tags = hxl.TagPattern.parse_list(args.get('merge-tags%02d' % index, []))
     keys = hxl.TagPattern.parse_list(args.get('merge-keys%02d' % index, []))
     replace = (args.get('merge-replace%02d' % index) == 'on')
     overwrite = (args.get('merge-overwrite%02d' % index) == 'on')
     url = args.get('merge-url%02d' % index)
-    merge_source = hxl.data(url, util.check_verify_ssl(args))
+    merge_source = util.hxl_data(url, util.make_input_options(args))
     return source.merge_data(merge_source, keys=keys, tags=tags, replace=replace, overwrite=overwrite)
 
 def add_rename_filter(source, args, index):
     """Add the hxlrename filter to the end of the pipeline."""
     oldtag = hxl.TagPattern.parse(args.get('rename-oldtag%02d' % index))
+    oldheader = hxl.datatypes.normalise_string(args.get('rename-oldheader%02d' % index))
     tagspec = _parse_tagspec(args.get('rename-newtag%02d' % index))
     header = args.get('rename-header%02d' % index)
     column = hxl.Column.parse(tagspec, header=header)
-    return source.rename_columns([(oldtag, column)])
+    return source.rename_columns([(oldtag, column, oldheader)])
 
 def add_replace_filter(source, args, index):
     """Add the hxlreplace filter to the end of the pipeline."""
     original = args.get('replace-pattern%02d' % index)
     replacement = args.get('replace-value%02d' % index)
     tags = args.get('replace-tags%02d' % index)
     use_regex = args.get('replace-regex%02d' % index)
     row_query = args.get('replace-where%02d' % index)
     return source.replace_data(original, replacement, tags, use_regex, queries=row_query)
 
 def add_replace_map_filter(source, args, index):
     """Add the hxlreplace filter to the end of the pipeline."""
     url = args.get('replace-map-url%02d' % index)
     row_query = args.get('replace-map-where%02d' % index)
-    return source.replace_data_map(hxl.data(url, util.check_verify_ssl(args)), queries=row_query)
+    return source.replace_data_map(util.hxl_data(url, util.make_input_options(args)), queries=row_query)
 
 def add_row_filter(source, args, index):
     """Add the hxlselect filter to the end of the pipeline."""
     queries = []
     for subindex in range(1, 6):
         query = args.get('select-query%02d-%02d' % (index, subindex))
         if query:
```

### Comparing `hxl-proxy-1.9.1/hxl_proxy/reverse_proxied.py` & `hxl-proxy-2.0/hxl_proxy/reverse_proxied.py`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/templates/data-view.html` & `hxl-proxy-2.0/hxl_proxy/templates/data-view.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/templates/data-login.html` & `hxl-proxy-2.0/hxl_proxy/templates/hash.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,43 @@
 <!DOCTYPE html>
 <html lang="en">
-  {% set facet='edit' %}
   <head>
-    <title>Password @ HXL Proxy</title>
+    <title>
+      HXL MD5 hash
+    </title>
     {% include "includes/headers.html" %}
   </head>
   <body class="container-fluid">
+    {% set page_help='Home' %}
     {% include "includes/navbar.html" %}
     <header>
-      <h1>Password required</h1>
+      <h1>
+        Generate an MD5 hash for HXL data
+      </h1>
     </header>
-    <main>
-      <p>You need to enter the correct password to edit <a href="{{ data_url_for('data_view', recipe) }}">{{ recipe.name }}</a></p>
-      <form class="theme-form" method="POST" action="{{ url_for('do_data_login') }}">
-        <div class="required form-group">
-          <label for="password">Password</label>
-          <input name="password" type="password" required="required" class="form-control" />
+    <main class="row">
+      <form method="get" action="" class="col-sm-12">
+        <div class="checkbox">
+          <label>
+            <input type="checkbox" name="headers_only" id="headers_only"
+                   />
+            Use header rows only.
+          </label>
+        </div>
+        <label for="url">URL of a HXL dataset:</label>
+        <div class="input-group required">
+          <input name="url"
+                 class="form-control"
+                 required="required"
+                 placeholder="http://example.org/hxl-dataset.csv" />
+          <span class="input-group-btn">
+            <button class="btn btn-success">Hash</button>
+          </span>
         </div>
-        <input type="hidden" name="from" value="{{data_url_for('data_edit', recipe) }}"/>
-        <button type="submit">Edit this recipe</button>
       </form>
     </main>
+    <footer>
+      <p>Read more about the <a href="http://hxlstandard.org">Humanitarian Exchange Language</a> (HXL).</p>
+    </footer>
     {% include "includes/scripts.html" %}
   </body>
 </html>
-
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
-{% set facet='edit' %}
 {% include "includes/headers.html" %}
-{% include "includes/navbar.html" %}
-****** Password required ******
+{% set page_help='Home' %} {% include "includes/navbar.html" %}
+****** Generate an MD5 hash for HXL data ******
 
-You need to enter the correct password to edit {{_recipe.name_}}
-Password [********************]
- Edit this recipe
+ ⁰ Use header rows only.
+URL of a HXL dataset:
+[url                 ]  Hash
+
+Read more about the Humanitarian_Exchange_Language (HXL).
  {% include "includes/scripts.html" %}
```

### Comparing `hxl-proxy-1.9.1/hxl_proxy/templates/validate-issue.html` & `hxl-proxy-2.0/hxl_proxy/templates/validate-issue.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/templates/data-source.html` & `hxl-proxy-2.0/hxl_proxy/templates/data-source.html`

 * *Files 19% similar despite different names*

```diff
@@ -32,14 +32,15 @@
           {% set method="POST" %}
           {% set action=url_for('do_data_save') %}
           {% else %}
           {% set method="GET" %}
           {% set action=url_for("data_edit") %}
           {% endif %}
           <form action="{{ action }}" method="{{ method }}">
+            <input type="hidden" name="dest" value="data_view"/>
             <div class="col-sm-8 col-md-10">
               <div class="input-group required">
                 <input id='dataset-url'
                        class="form-control" 
                        name="url"
                        type="url"
                        required="required"
@@ -52,34 +53,56 @@
               </div>
               <p class="help-block small">
                 Type or paste the URL of an online spreadsheet or API containing <a
                 href="http://hxlstandard.org/">HXL hashtags</a>.
               </p>
             </div>
 
-            <div class="form-group form-inline">
+            <div class="form-group col-sm-6">
 
-              <div class="col-sm-6">
-                <label for="sheet">
-                  Tab #
+              <div class="row">
+                <label for="sheet" class="col-sm-6 col-md-4 col-lg-3">
+                  Tab # (Excel)
                 </label>
-                <div class="form-group">
-                  <input name="sheet" value="{{ recipe.args.sheet }}" type="number" size="2" min="0" max="100" class="form-control"/>
+                <div class="form-group col-sm-6 col-md-8 col-lg-9">
+                  <input name="sheet" value="{{ recipe.args.sheet }}" type="number" min="0" max="100" class="form-control" placeholder="0 or higher"/>
                 </div>
               </div>
 
-              <div class="col-sm-6 checkbox">
-                <label>
-                  <input type="checkbox" name="skip_verify_ssl" {% if (recipe.args.skip_verify_ssl == 'on') %}checked="checked"{% endif %}/>
-                  Don't verify SSL certificates
+
+              <div class="row">
+                <label for="selector" class="col-sm-6 col-md-4 col-lg-3">
+                  Selector (JSON)
                 </label>
+                <div class="form-group col-sm-6 col-md-8 col-lg-9">
+                  <input name="selector" value="{{ recipe.args.selector }}" class="form-control" placeholder="JSONpath"/>
+                </div>
               </div>
+
+            </div>
+
+            <div class="form-group col-sm-6">
+              
+                <div class="col-sm-12 checkbox">
+                  <label>
+                    <input type="checkbox" name="expand_merged" {% if (recipe.args.expand_merged == 'on') %}checked="checked"{% endif %}/>
+                    Duplicate values in merged areas (Excel)
+                  </label>
+                </div>
+
+                <div class="col-sm-12 checkbox">
+                  <label>
+                    <input type="checkbox" name="scan_ckan_resources" {% if (recipe.args.scan_ckan_resources == 'on') %}checked="checked"{% endif %}/>
+                    Scan CKAN datasets for HXL resources
+                  </label>
+                </div>
+
             </div>
 
-            {% with excludes=['url', 'skip_verify_ssl', 'sheet'] %}
+            {% with excludes=['url', 'sheet', 'expand_merged', 'scan_ckan_resources'] %}
             {% if recipe.recipe_id %}
             <input type="hidden" name="recipe_id" value="{{ recipe.recipe_id }}"/>
             {% endif %}
             {% include "includes/params.html" %}
             {% endwith %}
 
           </form>
```

#### html2text {}

```diff
@@ -8,20 +8,26 @@
 ***** Option 1: enter a URL *****
 {% if recipe.recipe_id %} {% set method="POST" %} {% set action=url_for
 ('do_data_save') %} {% else %} {% set method="GET" %} {% set action=url_for
 ("data_edit") %} {% endif %}
 [Unknown INPUT type]
 Next
 Type or paste the URL of an online spreadsheet or API containing HXL_hashtags.
- Tab #
+ Tab # (Excel)
 [Unknown INPUT type]
+ Selector (JSON)
+[{{ recipe.args.selector }}]
 
-% if (recipe.args.skip_verify_ssl == 'on') %}checked="checked"{% endif %}/
-> Don't verify SSL certificates
-{% with excludes=['url', 'skip_verify_ssl', 'sheet'] %} {% if recipe.recipe_id
-%}  {% endif %} {% include "includes/params.html" %} {% endwith %}
+% if (recipe.args.expand_merged == 'on') %}checked="checked"{% endif %}/
+> Duplicate values in merged areas (Excel)
+
+% if (recipe.args.scan_ckan_resources == 'on') %}checked="checked"{% endif %}/
+> Scan CKAN datasets for HXL resources
+{% with excludes=['url', 'sheet', 'expand_merged', 'scan_ckan_resources'] %} {%
+if recipe.recipe_id %}  {% endif %} {% include "includes/params.html" %} {%
+endwith %}
 
 ***** Option 2: choose from the cloud *****
 [Humanitarian_Data_Exchange_logo]_HDX [Dropbox_logo]_Dropbox [Google_Drive
 logo]_Google_Drive
   {% include "includes/scripts.html" %} {% include "includes/chooser-
 scripts.html" %}
```

### Comparing `hxl-proxy-1.9.1/hxl_proxy/templates/hxl-test.html` & `hxl-proxy-2.0/hxl_proxy/templates/hxl-test.html`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             </dd>
             {% endif %}
             {% endif %}
           </dl>
           {% if result.status %}
           <a class="btn btn-default" href="{{ url_for('data_edit', url=result.url) }}">Open in HXL Proxy</a>
           {% elif result.exception=='HXLTagsNotFoundException' %}
-          <a class="btn btn-default" href="{{ url_for('data_tagger', url=result.url }}">Try tagging</a>
+          <a class="btn btn-default" href="{{ url_for('data_tagger', url=result.url) }}">Try tagging</a>
           {% endif %}
           <a class="btn btn-link pull-right icons small" href="/hxl-test.json?url={{ result.url|urlencode }}">JSON version</a>
         </div>
       </div>
       </section>
       {% endif %}
     </main>
```

### Comparing `hxl-proxy-1.9.1/hxl_proxy/templates/about.html` & `hxl-proxy-2.0/hxl_proxy/templates/about.html`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
             programmes.
           </li>
           <li>
             You are welcome to install your own version of the HXL
             Proxy web application on your personal computer, or on an
             Intranet inside your organisation's firewall. There is a
             <a
-                href="https://hub.docker.com/r/teodorescuserban/hxl-proxy/">Docker
+                href="https://hub.docker.com/r/unocha/hxl-proxy">Docker
             image</a> available for fast deployment.
           </li>
         </ol>
       </section>
       <section id="packages">
         <h3>What software does it use?</h3>
         <p>(For a complete list of requirements, see the source code.)</p>
```

### Comparing `hxl-proxy-1.9.1/hxl_proxy/templates/data-tagger.html` & `hxl-proxy-2.0/hxl_proxy/templates/data-tagger.html`

 * *Files 26% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         tags to go with your headers below, and the HXL Proxy will add
         them automatically.
       </p>
       {% endif %}
 
     </header>
     <main id="tagger" class="col-md-6 col-lg-5">
-      {% if (not recipe.recipe_id) and (not header_row) %}
+      {% if header_row is none %}
       <section class="col-sm-12">
         {% include "includes/source.html" %}
 
         {% if not using_tagger_p(recipe) %}
         <p class="alert alert-warning">
           We can't find any <a href="http://hxlstandard.org">HXL
           hashtags</a> in your data, but all is not lost!  You can define
@@ -41,15 +41,27 @@
 
         <p>First, select the <b>last header row</b> before the data starts.</p>
 
         <table class="table">
           {% for row in preview %}
           <tr>
             <td>
-              <form method="GET" action="">
+              {% if recipe.recipe_id %}
+              {% set method="POST" %}
+              {% set action=url_for('do_data_save') %}
+              {% else %}
+              {% set method="GET" %}
+              {% set action="" %}
+              {% endif %}
+              <form method="{{ method }}" action="{{ action }}">
+                {% if recipe.recipe_id %}
+                <input type="hidden" name="recipe_id" value="{{ recipe.recipe_id }}"/>
+                {% endif %}
+                {% import 'includes/filters/filter-variables.j2' as vars %}
+
                 <input type="hidden" name="header-row" value="{{ loop.index }}" />
                 {% include "includes/metadata-params.html" %}
                 {% include "includes/recipe-params.html" %}
                 <button class="btn btn-default">Row {{ loop.index }}</button>
               </form>
             </td>
             {% for value in row %}
@@ -66,15 +78,15 @@
         {% if recipe.recipe_id %}
         {% set method="POST" %}
         {% set action=url_for('do_data_save') %}
         {% else %}
         {% set method="GET" %}
         {% set action=url_for('data_edit') %}
         {% endif %}
-        <form class="tagger" action="{{ action }}" method="{{ method }}">
+        <form id="tagger" class="tagger" action="{{ action }}" method="{{ method }}">
 
           {% if recipe.recipe_id %}
           <input type="hidden" name="recipe_id" value="{{ recipe.recipe_id }}"/>
           {% endif %}
           {% import 'includes/filters/filter-variables.j2' as vars %}
 
           <div class="panel panel-primary">
@@ -105,15 +117,15 @@
                        placeholder="#tag"/>
               </div>
 
             </div>
           </div>
 
           <p class="alert alert-info">
-            Pick HXL tags for some or all of your headers.
+            Pick HXL tags for some or all of your headers. Note that each string may have only one hashtag spec mapped to it (it is not possible to distinguish multiple columns with identical header text).
           </p>
 
           <p class="visible-xs visible-sm">
             (<a href="#preview">jump to raw source data preview</a>)
           </p>
 
           <div class="form-group">
@@ -127,26 +139,26 @@
                 <tr>
                   <td><i>E.g.</i></td>
                   <td><code>Province</code></td>
                   <td><code>#adm1</code></td>
                 </tr>
               </thead>
               <tbody>
-                {% for value in preview[header_row-1] %}
+                {% for mapping in mappings %}
                 {% set name='tagger-%02d' % loop.index %}
                 <tr>
                   <td>{{ loop.index }}</td>
                   <td>
                     <input class="form-control" name="{{ name + '-header' }}"
-                           value="{{ recipe.args[name + '-header'] or value|strnorm }}"
+                           value="{{ mapping[0] }}"
                            placeholder="Header text" />
                   </td>
                   <td>
                     <input class="form-control" name="{{ name + '-tag' }}"
-                           value="{{ recipe.args[name + '-tag'] }}"
+                           value="{{ mapping[1] }}"
                            pattern="^{{ vars.tag_pattern }}$" title="{{ vars.tag_help }}"
                            placeholder="{{ vars.tag_placeholder }}" />
                   </td>
                 </tr>
                 {% endfor %}
               </tbody>
             </table>
```

#### html2text {}

```diff
@@ -3,39 +3,45 @@
 {% set page_help='Tagger-page' %} {% include "includes/navbar.html" %}  {%
 include "includes/data-tabs.html" %}
 ****** Tag a non-HXL dataset ******
 {% include "includes/source.html" %} {% if not using_tagger_p(recipe) %}
 We can't find any HXL_hashtags in your data, but all is not lost! You can
 define tags to go with your headers below, and the HXL Proxy will add them
 automatically.
-{% endif %}   {% if (not recipe.recipe_id) and (not header_row) %}  {% include
-"includes/source.html" %} {% if not using_tagger_p(recipe) %}
+{% endif %}   {% if header_row is none %}  {% include "includes/source.html" %}
+{% if not using_tagger_p(recipe) %}
 We can't find any HXL_hashtags in your data, but all is not lost! You can
 define tags to go with your headers below, and the HXL Proxy will add them
 automatically.
 {% endif %}
 First, select the last header row before the data starts.
- {% include "includes/metadata-params.html" %} {% include {{ value }}
-"includes/recipe-params.html" %} Row {{ loop.index }}
+{% if recipe.recipe_id %} {% set method="POST" %} {% set
+action=url_for('do_data_save') %} {% else %} {% set method="GET" %}
+{% set action="" %} {% endif %}
+{% if recipe.recipe_id %}  {% endif %} {% import 'includes/filters/ {{ value }}
+filter-variables.j2' as vars %}  {% include "includes/metadata-
+params.html" %} {% include "includes/recipe-params.html" %} Row {
+{ loop.index }}
  {% else %}  {% if recipe.recipe_id %} {% set method="POST" %} {% set
 action=url_for('do_data_save') %} {% else %} {% set method="GET" %} {% set
 action=url_for('data_edit') %} {% endif %}
 {% if recipe.recipe_id %}  {% endif %} {% import 'includes/filters/filter-
 variables.j2' as vars %}
 ***** Tagger settings *****
 
 % if recipe.args.get('tagger-match-all') or not using_tagger_p(recipe) %}
 checked="checked" {% endif %}/> Match full header text?
  Default HXL hashtag  [{{recipe.args['tagger-default-tag']}}]
-Pick HXL tags for some or all of your headers.
+Pick HXL tags for some or all of your headers. Note that each string may have
+only one hashtag spec mapped to it (it is not possible to distinguish multiple
+columns with identical header text).
 (jump_to_raw_source_data_preview)
-                 Header (sub)string            HXL hashtag
-E.g.             Province                      #adm1
-{{ loop.index }} [{{ recipe.args[name + '-     [{{ recipe.args[name + '-tag']
-                 header'] or value|strnorm }}] }}]
+                 Header (sub)string     HXL hashtag
+E.g.             Province               #adm1
+{{ loop.index }} [{{ mapping[0] }}    ] [{{ mapping[1] }}    ]
 Next
 {% include "includes/metadata-params.html" %} {% include "includes/recipe-
 params.html" %}
  {% endif %}
 ***** Raw source data (preview) *****
 (jump_to_tagger)
 {{ cell }}
```

### Comparing `hxl-proxy-1.9.1/hxl_proxy/templates/data-advanced.html` & `hxl-proxy-2.0/hxl_proxy/templates/data-advanced.html`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,18 @@
       {% set action=url_for('do_data_save') %}
       {% else %}
       {% set method="GET" %}
       {% set action=url_for('data_view') %}
       {% endif %}
       <form action="{{ action }}" method="{{ method }}">
 
+        {% if recipe.recipe_id %}
+        <input type="hidden" name="recipe_id" value="{{ recipe.recipe_id }}"/>
+        {% endif %}
+
         <div class="form-group required col-sm-12">
           <label for="url">Data URL</label>
           <input class="form-control" name="url" required="required" type="url" value="{{ recipe.args.url|nonone }}"/>
         </div>
 
         <div class="form-group col-sm-3 col-xs-6">
           <label for="sheet">Tab number (starting at 0)</label>
```

#### html2text {}

```diff
@@ -4,14 +4,15 @@
 "includes/data-tabs.html" %} {% endwith %}
 ****** Advanced transformation ******
 
 This page is for developers and other advanced technical users.
 {% if recipe.recipe_id %} {% set method="POST" %} {% set action=url_for
 ('do_data_save') %} {% else %} {% set method="GET" %} {% set action=url_for
 ('data_view') %} {% endif %}
+{% if recipe.recipe_id %}  {% endif %}
 Data URL [Unknown INPUT type]
 Tab number (starting at 0) [Unknown INPUT type]
 Maximum rows [Unknown INPUT type]
 
 % if recipe.args['strip-headers'] %} checked="checked"{% endif %} /> Strip text
 headers
```

### Comparing `hxl-proxy-1.9.1/hxl_proxy/templates/iati2hxl.html` & `hxl-proxy-2.0/hxl_proxy/templates/error.html`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 <!DOCTYPE html>
 <html lang="en">
   <head>
-    <title>
-      Convert IATI to HXL
-    </title>
-    {% include "includes/headers.html" %}
+    <title>HXL Proxy error</title>
+    {% include "includes/scripts.html" %}
   </head>
   <body class="container-fluid">
-    {% set page_help='Home' %}
-    {% include "includes/navbar.html" %}
     <header>
-      <h1>
-        Convert IATI to HXL
-      </h1>
+      <h1>Something went wrong!</h1>
     </header>
-    <main class="row">
-      <form method="get" action="" class="col-sm-12">
-        <label for="url">URL of an iati-activities dataset:</label>
-        <div class="input-group required">
-          <input name="url"
-                 class="form-control"
-                 required="required"
-                 placeholder="http://example.org/iati-data.xml" />
-          <span class="input-group-btn">
-            <button class="btn btn-success">Convert</button>
-          </span>
+    <main>
+      <div class="panel panel-danger">
+        <div class="panel-heading">
+          <h2 class="panel-title">Details</h2>
+        </div>
+        <div class="panel-body">
+          {% if e.human %}
+          <p class="lead">
+            <b>In human-speak:</b>
+            {{ e.human }}
+          </p>
+          {% endif %}
+          <p>
+            <b>In machine-speak:</b>
+            <blockquote>
+            <pre>{% if e.message %}{{ e.message }}{% else %}{{ e }}{%
+            endif %}</pre>
+            </blockquote>
+          </p>
+        </div>
+        <div class="panel-footer small">
+          You can try using your browser's [Back] button to return to the previous page. If you cannot resolve the problem, please help us make the HXL Proxy better! <a href="https://github.com/HXLStandard/hxl-proxy/issues">Report this bug at GitHub</a> (and include the URL).
         </div>
-      </form>
+      </div>
     </main>
-    <footer>
-      <p>Read more about the <a href="http://hxlstandard.org">Humanitarian Exchange Language</a> (HXL).</p>
-    </footer>
     {% include "includes/scripts.html" %}
   </body>
 </html>
```

#### html2text {}

```diff
@@ -1,9 +1,14 @@
-{% include "includes/headers.html" %}
-{% set page_help='Home' %} {% include "includes/navbar.html" %}
-****** Convert IATI to HXL ******
+{% include "includes/scripts.html" %}
+****** Something went wrong! ******
 
-URL of an iati-activities dataset:
-[url                 ]  Convert
-
-Read more about the Humanitarian_Exchange_Language (HXL).
+***** Details *****
+{% if e.human %}
+In human-speak: {{ e.human }}
+{% endif %}
+In machine-speak:
+     {% if e.message %}{{ e.message }}{% else %}{{ e }}{%
+                 endif %}
+You can try using your browser's [Back] button to return to the previous page.
+If you cannot resolve the problem, please help us make the HXL Proxy better!
+Report_this_bug_at_GitHub (and include the URL).
  {% include "includes/scripts.html" %}
```

### Comparing `hxl-proxy-1.9.1/hxl_proxy/templates/validate-summary.html` & `hxl-proxy-2.0/hxl_proxy/templates/validate-summary.html`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,17 @@
           <select name="severity" class="form-control" onchange="$('#severity-form').submit();">
             <option value="info"{% if severity == 'info' %} selected="selected"{% endif %}>Info (most verbose)</option>
             <option value="warning"{% if severity == 'warning' %} selected="selected"{% endif %}>Warnings</option>
             <option value="error"{% if severity == 'error' %} selected="selected"{% endif %}>Errors (least verbose)</option>
           </select>
           <button class="hidden btn btn-default" type="submit">Change</button>
         </div>
+        {% if not recipe.recipe_id %}
         {% include "includes/params.html" %}
+        {% endif %}
       </form>
       <p class="alert alert-info">
         Showing {{ count }} of {{ error_report.stats.total }} issue location(s)
       </p>
       {% if count == 0 %}
       <p class="alert alert-warning">
         No issues to show at this level. Try a different error level to
```

#### html2text {}

```diff
@@ -15,15 +15,15 @@
 Validation succeeded with no issues.
 {% else %}
 % if severity == 'info' %} selected="selected"{% endif %}>Info (most verbose)
 % if severity == 'warning' %} selected="selected"{% endif %}>Warnings
 % if severity == 'error' %} selected="selected"{% endif %}>Errors (least
 verbose)
  Change
-{% include "includes/params.html" %}
+{% if not recipe.recipe_id %} {% include "includes/params.html" %} {% endif %}
 Showing {{ count }} of {{ error_report.stats.total }} issue location(s)
 {% if count == 0 %}
 No issues to show at this level. Try a different error level to see more.
 {% else %}
 Severity       Locations            Explanation       Scope       HXL tag pattern
 {              See_{                {                 {           {
 {              {                    {                 {           {
```

### Comparing `hxl-proxy-1.9.1/hxl_proxy/templates/settings-user.html` & `hxl-proxy-2.0/hxl_proxy/templates/settings-user.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/templates/data-recipe.html` & `hxl-proxy-2.0/hxl_proxy/templates/data-recipe.html`

 * *Files 6% similar despite different names*

```diff
@@ -27,30 +27,36 @@
         {% set method="POST" %}
         {% set action=url_for('do_data_save') %}
         {% else %}
         {% set method="GET" %}
         {% set action=url_for('data_edit') %}
         {% endif %}
         <form action="{{ action }}" method="{{ method }}" id="filter-form">
-
+          <input type="hidden" name="dest" value="data_edit"/>
           <ol class="filter-list" role="group" aria-label="Data filters">
             {# Filter types and names defined in this file: #}
             {% import 'includes/filters/filter-types.j2' as filter_types %}
             {% set vars = {'last_index': 0 } %}
             {% for n in range(1, 99) %}
             {% set filter_type = recipe.args['filter{0:02}'.format(n)] %}
+            {% set filter_label = recipe.args['filter-label{0:02}'.format(n)] %}
             {% if filter_type %}
             {% if vars.update({'last_index': n}) %}{% endif %}{# kludge to set var outside scope #}
             <li class="filter{% if n!=filter_count %} sort-item{% endif %}">
               <span class="handle glyphicon glyphicon-move"></span>
-              <a class="filter-button"
-                 data-toggle="modal"
-                 data-target="{{'#filter-dialog-%02d' % n }}" href="{{'#filter-dialog-%02d' % n}}">
-                {{ filter_types.names[filter_type] }}
-              </a>
+              <span class="filter-name">
+                <a class="filter-button"
+                   data-toggle="modal"
+                   data-target="{{'#filter-dialog-%02d' % n }}" href="{{'#filter-dialog-%02d' % n}}">
+                  {{ filter_types.names[filter_type] }}
+                </a>
+              </span>
+              {% if filter_label %}
+              <span class="filter-label">{{ filter_label }}</span>
+              {% endif %}
               <span class="filter-delete">[<a onclick="hxl_proxy.ui.removeFilter(this);">x</a>]</span>
               <div class="modal fade" id="{{ 'filter-dialog-%02d' % n }}" tabindex="-1" role="dialog" aria-hidden="true">
                 <div class="modal-dialog">
                   <div class="modal-content">
                     <div class="modal-header">
                       <h2 class="modal-title">{{ filter_types.names[filter_type] }}</h2>
                     </div>
@@ -159,23 +165,34 @@
           {% if recipe.args['recipe'] %}
           <input type="hidden" name="recipe" value="{{ recipe.args['recipe'] }}" />
           {% endif %}
         </form>
       </section>
 
       <section class="col-sm-8 col-md-9">
+        {% if source %}
         <h3>Result preview</h3>
         <div id="preview-table">
           {% include 'includes/hxltable.html' %}
         </div>
         {% if source.has_more_rows %}
         <p id="preview-warning" class="alert alert-warning hxltable-warning">
           Previewing the first {{ "{:,}".format(source.max_rows) }} data row(s).
         </p>
         {% endif %}
+        {% else %}
+        <h3>Error!</h3>
+        <p style="white-space: pre-line">
+        {% if error %}
+        {{ error }}
+        {% else %}
+        Unknown error - please fix recipe
+        {% endif %}
+        </p>
+        {% endif %}
       </section>
     </main>
     {% include "includes/scripts.html" %}
     {% include "includes/chooser-scripts.html" %}
     <script src="{{ static('jquery/jquery-ui.min.js') }}"></script>
     <script src="{{ static('jquery/jquery.ui.touch-punch.min.js') }}"></script>
     <script>
```

#### html2text {}

```diff
@@ -9,17 +9,19 @@
 {% endwith %} ****
 {% if recipe.recipe_id %} {% set method="POST" %} {% set action=url_for
 ('do_data_save') %} {% else %} {% set method="GET" %} {% set action=url_for
 ('data_edit') %} {% endif %}
    1. {# Filter types and names defined in this file: #} {% import 'includes/
       filters/filter-types.j2' as filter_types %} {% set vars = {'last_index':
       0 } %} {% for n in range(1, 99) %} {% set filter_type = recipe.args
-      ['filter{0:02}'.format(n)] %} {% if filter_type %} {% if vars.update(
+      ['filter{0:02}'.format(n)] %} {% set filter_label = recipe.args['filter-
+      label{0:02}'.format(n)] %} {% if filter_type %} {% if vars.update(
       {'last_index': n}) %}{% endif %}{# kludge to set var outside scope #}
-   2.  {{_filter_types.names[filter_type]_}} [x]
+   2.   {{_filter_types.names[filter_type]_}}  {% if filter_label %} {
+      { filter_label }} {% endif %} [x]
       ***** {{ filter_types.names[filter_type] }} *****
         {% include 'includes/filters/filter-list.html' %}
       Save changes Remove filter
    3. {% endif %} {% endfor %} {% set n = vars.last_index + 1 %}
    4.  (new_filter)
       ***** New filter *****
       {% include 'includes/filters/filter-selector.html' %}
@@ -32,14 +34,18 @@
 % if recipe.args['force'] %} checked="checked"{% endif %} /> Never cache
 Filename (no ext) [{{ recipe.stub|nonone }}]
 Max rows [Unknown INPUT type]
 Update preferences
  {% if recipe.recipe_id %}  {% endif %} {% include "includes/tagger-
 params.html" %} {% include "includes/metadata-params.html" %} {% if recipe.args
 ['recipe'] %}  {% endif %}
-
+  {% if source %}
 **** Result preview ****
 {% include 'includes/hxltable.html' %}
 {% if source.has_more_rows %}
 Previewing the first {{ "{:,}".format(source.max_rows) }} data row(s).
+{% endif %} {% else %}
+**** Error! ****
+{% if error %} {{ error }} {% else %} Unknown error - please fix recipe {%
+endif %}
 {% endif %}   {% include "includes/scripts.html" %} {% include "includes/
 chooser-scripts.html" %}
```

### Comparing `hxl-proxy-1.9.1/hxl_proxy/templates/includes/hxltable.html` & `hxl-proxy-2.0/hxl_proxy/templates/includes/hxltable.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/templates/includes/postcards.html` & `hxl-proxy-2.0/hxl_proxy/templates/includes/postcards.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/count.html` & `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/count.html`

 * *Files 6% similar despite different names*

```diff
@@ -2,42 +2,52 @@
   {% import 'includes/filters/filter-variables.j2' as vars %}
 
   <p class="doc">
     {% with key='Count-rows-filter' %}{% include "includes/help.html" %}{% endwith %}
     Aggregate HXL data to generate reports or protect private data.
   </p>
 
+  {% include 'includes/filters/label-field.html' %}
+
   {% set name='count-tags%02d' % n %}
   <div class="form-group">
-    <label for="{{ name }}">
-      Count unique combinations of these hashtags (comma-separated)
-    </label>
+    <label for="{{ name }}">Tag pattern(s) for column(s)</label>
     <input
         id="{{ name }}"
         class="form-control"
         name="{{ name }}"
         value="{{ recipe.args[name] }}"
         pattern="^{{ vars.filters_pattern }}$"
         title="{{ vars.filters_help }}"
         placeholder="{{ vars.filters_placeholder }}" />
+    <p class="help">
+      Count unique combinations of values from columns matching one or
+      more of these <a target="_blank"
+      href="https://github.com/HXLStandard/hxl-proxy/wiki/Tag-patterns">tag
+      patterns</a> (comma-separated). If blank, count unique
+      combinations of values from all columns.
+    </p>
   </div>
 
   {% set name='count-where%02d' % n %}
   <div class="form-group">
-    <label for="{{ name }}">
-      Count only rows that match this query
-    </label>
+    <label for="{{ name }}">Row query</label>
     <input
         id="{{ name }}"
         class="form-control"
         name="{{ name }}"
         value="{{ recipe.args[name] }}"
         pattern="^{{ vars.query_pattern }}$"
         title="{{ vars.query_help }}"
         placeholder="#tag=value" />
+    <p class="help">
+      Count values from rows matching this <a target="_blank"
+      href="https://github.com/HXLStandard/hxl-proxy/wiki/Row-queries">row
+      query</a>. If blank, count values from all rows.
+    </p>
   </div>
 
   <fieldset>
     <legend>Aggregate values to generate</legend>
 
     {% for m in range(1, 26) %}
     {% set type='count-type%02d-%02d' % (n, m,) %}
@@ -68,14 +78,19 @@
           <option value="min">Minimum</option>
           {% endif %}
           {% if recipe.args[type] == 'max' %}
           <option value="max" selected="selected">Maximum</option>
           {% else %}
           <option value="max">Maximum</option>
           {% endif %}
+          {% if recipe.args[type] == 'concat' %}
+          <option value="concat" selected="selected">Concatenate</option>
+          {% else %}
+          <option value="concat">Concatenate</option>
+          {% endif %}
         </select>
       </div>
       
       {% set name='count-pattern%02d-%02d' % (n, m,) %}
       <div class="form-group col-sm-6 aggregate-pattern required">
         <label for="{{ name }}">Source column</label>
         <input id="{{ name }}"
```

### Comparing `hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/filter-list.html` & `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/filter-list.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/jsonpath.html` & `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/jsonpath.html`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
   <p class="doc">
     {% with key='JSONPath-filter' %}{% include "includes/help.html" %}{% endwith %}
     Extract a value from a JSON expression in a cell using a <a
     href="http://goessner.net/articles/JsonPath/">JSONPath</a> expression.
   </p>
 
+  {% include 'includes/filters/label-field.html' %}
+
   {% set name='jsonpath-path%02d' % n %}
   <div class="form-group required">
     <label for="{{ name }}">
       JSONPath expression for extracting a value.
     </label>
     <input
         id="{{ name }}"
@@ -50,8 +52,22 @@
         value="{{ recipe.args[name] }}"
         pattern="^{{ vars.query_pattern }}$"
         title="{{ vars.query_help }}"
         placeholder="{{ vars.query_placeholder }}"
         />
   </div>
 
+  {% set name='jsonpath-flatten%02d' % n %}
+  <div class="checkbox">
+    <label>
+      <input
+          type="checkbox"
+          name="{{ name }}"
+          {% if recipe.args[name] %}
+          checked="checked"
+          {% endif %}
+          />
+          Flatten multiple results (separated by " | ")
+    </label>
+  </div>
+  
 </div>
```

#### html2text {}

```diff
@@ -1,10 +1,15 @@
 {% import 'includes/filters/filter-variables.j2' as vars %}
 {% with key='JSONPath-filter' %}{% include "includes/help.html" %}{% endwith %}
 Extract a value from a JSON expression in a cell using a JSONPath expression.
-{% set name='jsonpath-path%02d' % n %}
+{% include 'includes/filters/label-field.html' %} {% set name='jsonpath-
+path%02d' % n %}
  JSONPath expression for extracting a value.  [{{ recipe.args[name] }}]
 {% set name='jsonpath-patterns%02d' % n %}
  Tag patterns for applying the JSONPath (blank means apply to all).  [{
 { recipe.args[name] }}]
 {% set name='jsonpath-where%02d' % n %}
  Apply only to rows matching this query  [{{ recipe.args[name] }}]
+{% set name='jsonpath-flatten%02d' % n %}
+
+% if recipe.args[name] %} checked="checked" {% endif %} /> Flatten multiple
+results (separated by " | ")
```

### Comparing `hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/filter-types.j2` & `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/filter-types.j2`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 {# Recipe filter types and labels #}
 {% set names = {
     'add': 'Add column',
     'append': 'Append datasets',
+    'append-list': 'Append datasets (external list)',
     'clean': 'Clean data',
     'count': 'Count rows',
     'cut': 'Cut columns',
     'dedup': 'Deduplicate rows',
-    'explode': 'Explode data',
+    'expand': 'Expand lists',
+    'explode': 'Explode wide data to narrow',
     'fill': 'Fill empty cells',
+    'implode': 'Implode narrow data to wide',
     'jsonpath': 'JSONPath value extraction',
     'merge': 'Merge from another dataset',
     'rename': 'Rename column',
     'replace': 'Replace data',
     'replace-map': 'Replace data (external map)',
     'select': 'Select rows',
     'sort': 'Sort rows',
```

### Comparing `hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/filter-selector.html` & `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/filter-selector.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/explode.html` & `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/fill.html`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,43 @@
-<div class="filter-explode filter-body">
+<div class="filter-fill filter-body">
   {% import 'includes/filters/filter-variables.j2' as vars %}
 
   <p class="doc">
-    {% with key='Explode-data-filter' %}{% include "includes/help.html" %}{% endwith %}
-    Explode wide, series data using the headers as labels. This filter
-    uses the special <code>+label</code> attribute to identify columns.
+    {% with key='Fill-data-filter' %}{% include "includes/help.html" %}{% endwith %}
+    Fill empty cells from previous values in the same column.
   </p>
 
-  {% set name='explode-header-att%02d' % n %}
+  {% include 'includes/filters/label-field.html' %}
+
+  {% set name='fill-patterns%02d' % n %}
   <div class="form-group">
     <label for="{{ name }}">
-      Attribute for former header text.
+      Tag patterns for filling (blank means fill all).
     </label>
     <input
         id="{{ name }}"
         class="form-control"
         name="{{ name }}"
-        value="{{ recipe.args[name] or 'header' }}"
-        pattern="^{{ vars.filters_pattern }}$"
+        value="{{ recipe.args[name] }}"
+        patterns="^{{ vars.filters_pattern }}$"
         title="{{ vars.filters_help }}"
         placeholder="{{ vars.filters_placeholder }}"
         />
   </div>
 
-  {% set name='explode-value-att%02d' % n %}
+  {% set name='fill-where%02d' % n %}
   <div class="form-group">
     <label for="{{ name }}">
-      Attribute for original value.
+      Fill only in rows matching this query
     </label>
     <input
         id="{{ name }}"
         class="form-control"
         name="{{ name }}"
-        value="{{ recipe.args[name] or 'value' }}"
-        pattern="^{{ vars.filters_pattern }}$"
-        title="{{ vars.filters_help }}"
-        placeholder="{{ vars.filters_placeholder }}"
+        value="{{ recipe.args[name] }}"
+        pattern="^{{ vars.query_pattern }}$"
+        title="{{ vars.query_help }}"
+        placeholder="{{ vars.query_placeholder }}"
         />
   </div>
 
 </div>
```

### Comparing `hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/replace.html` & `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/replace.html`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,16 @@
   {% import 'includes/filters/filter-variables.j2' as vars %}
 
   <p class="doc">
     {% with key='Replace-data-filter' %}{% include "includes/help.html" %}{% endwith %}
     Replace values in the dataset.
   </p>
 
+  {% include 'includes/filters/label-field.html' %}
+
   {% set name='replace-pattern%02d' % n %}
   <div class="form-group required">
     <label for="{{ name }}">
       Text or pattern to replace
     </label>
     <input
         id="{{ name }}"
```

### Comparing `hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/add.html` & `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/add.html`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,16 @@
   {% import 'includes/filters/filter-variables.j2' as vars %}
 
   <p class="doc">
     {% with key='Add-column-filter' %}{% include "includes/help.html" %}{% endwith %}
     Add a new column (with a constant value) to the data.
   </p>
 
+  {% include 'includes/filters/label-field.html' %}
+
   {% set name='add-tag{0:02}'.format(n) %}
   <div class="form-group required">
     <label for="{{ name }}">
       Tag for new column.
     </label>
     <input
         id="{{ name }}"
```

### Comparing `hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/replace-map.html` & `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/replace-map.html`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,16 @@
   {% import 'includes/filters/filter-variables.j2' as vars %}
 
   <p class="doc">
     {% with key='Replace-data-%28mapping-table%29-filter' %}{% include "includes/help.html" %}{% endwith %}
     Replace values using an external mapping table.
   </p>
 
+  {% include 'includes/filters/label-field.html' %}
+
   {% set name='replace-map-url%02d' % n %}
   <div class="form-group required">
     <label for="{{ name }}">
       URL of the external mapping table
     </label>
     <input
         id="{{ name }}"
```

### Comparing `hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/rename.html` & `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/rename.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 <div class="filter-rename filter-body">
   {% import 'includes/filters/filter-variables.j2' as vars %}
   <p class="doc">
     {% with key='Rename-column-filter' %}{% include "includes/help.html" %}{% endwith %}
     Rename and retag an existing column.
   </p>
 
+  {% include 'includes/filters/label-field.html' %}
+
   {% set name='rename-oldtag%02d' % n %}
   <div class="form-group required">
     <label for="{{ name }}">
       Original hashtag pattern
     </label>
     <input
         id="{{ name }}"
@@ -18,14 +20,28 @@
         pattern="^{{ vars.filter_pattern }}$"
         title="{{ vars.filter_help }}"
         required="required"
         placeholder="{{ vars.filter_placeholder }}"
         />
   </div>
 
+  {% set name='rename-oldheader%02d' % n %}
+  <div class="form-group">
+    <label for="{{ name }}">
+      Choose only columns with this text header (optional)
+    </label>
+    <input
+        id="{{ name }}"
+        class="form-control"
+        name="{{ name }}"
+        value="{{ recipe.args[name] }}"
+        placeholder="Old display header"
+        />
+  </div>
+
   {% set name='rename-newtag%02d' % n %}
   <div class="form-group required">
     <label for="{{ name }}">
       New hashtag and attributes
     </label>
     <input
         id="{{ name }}"
```

### Comparing `hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/dedup.html` & `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/dedup.html`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,16 @@
   {% import 'includes/filters/filter-variables.j2' as vars %}
 
   <p class="doc">
     {% with key='Deduplicate-rows-filter' %}{% include "includes/help.html" %}{% endwith %}
     Remove duplicate rows from a dataset.
   </p>
 
+  {% include 'includes/filters/label-field.html' %}
+
   {% set name='dedup-tags%02d' % n %}
   <div class="form-group">
     <label for="{{ name }}">
       Tags to look at for deduplication (if blank, <i>all</i> columns
       must match for a duplicate).
     </label>
     <input
```

### Comparing `hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/cut.html` & `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/cut.html`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,20 @@
   {% import 'includes/filters/filter-variables.j2' as vars %}
 
   <p class="doc">
     {% with key='Cut-columns-filter' %}{% include "includes/help.html" %}{% endwith %}
     Remove columns from your dataset.
   </p>
 
+  {% include 'includes/filters/label-field.html' %}
+
   {% set name='cut-include-tags%02d' % n %}
   <div class="form-group">
     <label for="{{ name }}">
-      Whitelist: include only these tags (comma-separated)
+      Includes: include only these tags (comma-separated)
     </label>
     <input
         id="{{ name }}"
         class="form-control"
         name="{{ name }}"
         value="{{ recipe.args[name] }}"
         pattern="^{{ vars.filters_pattern }}$"
@@ -21,15 +23,15 @@
         placeholder="{{ vars.filters_placeholder }}"
         />
   </div>
 
   {% set name='cut-exclude-tags%02d' % n %}
   <div class="form-group">
     <label for="{{ name }}">
-      Blacklist: include everything <i>but</i> these tags
+      Excludes: include everything <i>but</i> these tags
       (comma-separated).
     </label>
     <input
         id="{{ name }}"
         class="form-control"
         name="{{ name }}"
         value="{{ recipe.args[name] }}"
```

### Comparing `hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/clean.html` & `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/clean.html`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,16 @@
       <p class="doc">
         {% with key='Clean-data-filter' %}{% include "includes/help.html" %}{% endwith %}
         Clean up your dataset by standardising dates and numbers, removing
         whitespace, etc.
       </p>
     </div>
 
+    {% include 'includes/filters/label-field-multicol.html' %}
+
     {% set name='clean-whitespace-tags{0:02}'.format(n) %}
     <div class="form-group col-sm-6">
       <label for="{{ name }}">
         Normalise whitespace for these hashtags
       </label>
       <input
           id="{{ name }}"
@@ -23,15 +25,15 @@
           value="{{ recipe.args[name] }}"
           pattern="^{{ vars.filters_pattern }}$"
           title="{{ vars.filters_help }}"
           placeholder="{{ vars.filters_placeholder }}"
           />
     </div>
 
-        {% set name='clean-latlon-tags{0:02}'.format(n) %}
+    {% set name='clean-latlon-tags{0:02}'.format(n) %}
     <div class="form-group col-sm-6">
       <label for="{{ name }}">
         Standardise lat/lon for these hashtags
       </label>
       <input
           id="{{ name }}"
           class="form-control"
```

### Comparing `hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/filter-variables.j2` & `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/filter-variables.j2`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 {% set token_pattern = '[A-Za-z][_0-9A-Za-z]*' %}
 
-{% set tag_pattern = '\s*#?' + token_pattern + '(\s*[+]' + token_pattern + ')*\s*' %}
+{% set tag_pattern = '\\s*#?' + token_pattern + '(\\s*[+]' + token_pattern + ')*\\s*' %}
 {% set tag_help = 'Hashtag spec, "#" optional (e.g. "country+code")' %}
 {% set tag_placeholder = '#hashtag +attr' %}
 
 {% set tags_pattern = '(' + tag_pattern + ')(,' + tag_pattern + ')*' %}
 {% set tags_help = 'Hashtag specs, comma-separated, "#" optional (e.g. "country+code,sector")' %}
 {% set tags_placeholder = '#hashtag1,#hashtag2+attr' %}
 
-{% set filter_pattern = '\s*#?(?:' + (token_pattern) + '|\*)(\s*[+-]' + token_pattern + ')*\s*!?\s*' %}
+{% set filter_pattern = '\\s*#?(?:' + (token_pattern) + '|\\*)(\\s*[+-]' + token_pattern + ')*\\s*!?\\s*' %}
 {% set filter_help = 'Tag pattern, "#" optional (e.g. "country+code-dest")' %}
 {% set filter_placeholder = '#hashtag +attr1 -attr2' %}
 
 {% set filters_pattern = '(' + filter_pattern + ')(,' + filter_pattern + ')*' %}
 {% set filters_help = 'Tag patterns, comma-separated, "#" optional, (e.g. "country,adm1+code,org-funder")' %}
 {% set filters_placeholder = '#hashtag1,#hashtag2+attr1-attr2' %}
 
-{% set query_pattern = filter_pattern + '\s*([=~<>]|<=|>=|!=|!~|is).*' %}
+{% set query_pattern = filter_pattern + '\\s*([=~<>]|<=|>=|!=|!~|is).*' %}
 {% set query_help = 'Row query, "#" optional (e.g. "country+code=SYR")' %}
 {% set query_placeholder = '#hashtag+attr=value' %}
```

### Comparing `hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/merge.html` & `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/merge.html`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,16 @@
   {% import 'includes/filters/filter-variables.j2' as vars %}
 
   <p class="doc">
     {% with key='Merge-columns-filter' %}{% include "includes/help.html" %}{% endwith %}
     Add columns from another dataset, based on common keys.
   </p>
 
+  {% include 'includes/filters/label-field.html' %}
+
   {% set name='merge-url%02d' % n %}
   <div class="form-group required">
     <label for="{{ name }}">
       URL of merge dataset (pull extra data from here)
     </label>
     <input
         id="{{ name }}"
```

### Comparing `hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/select.html` & `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/select.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 <div class="filter-select filter-body">
   {% import 'includes/filters/filter-variables.j2' as vars %}
   <p class="doc">
     {% with key='Select-rows-filter' %}{% include "includes/help.html" %}{% endwith %}
     Include rows that match <strong>any</strong> of the following queries
   </p>
 
+  {% include 'includes/filters/label-field.html' %}
+
   {% set name='select-query%02d' % n %}
   <div class="form-group required">
     <label>Queries (e.g. adm1=Bomo)</label>
     {% for n in range(1, 25) %}
     {% set query_name = '%s-%02d' % (name, n) %}
     {% if n == 1 or recipe.args[query_name] %}
     <input class="form-control" name="{{ query_name }}" value="{{ recipe.args[query_name] }}" pattern="^{{ vars.query_pattern }}$" title="{{ vars.query_help }}" placeholder="#tag=value" />
```

### Comparing `hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/fill.html` & `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/implode.html`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,45 @@
-<div class="filter-fill filter-body">
+<div class="filter-implode filter-body">
   {% import 'includes/filters/filter-variables.j2' as vars %}
 
   <p class="doc">
-    {% with key='Fill-data-filter' %}{% include "includes/help.html" %}{% endwith %}
-    Fill empty cells from previous values in the same column.
+    {% with key='Implode-data-filter' %}{% include "includes/help.html" %}{% endwith %}
+    Denormalise data from "narrow" to "wide".
   </p>
 
-  {% set name='fill-patterns%02d' % n %}
-  <div class="form-group">
+  {% include 'includes/filters/label-field.html' %}
+
+  {% set name='implode-label-pattern%02d' % n %}
+  <div class="form-group required">
     <label for="{{ name }}">
-      Tag patterns for filling (blank means fill all).
+      Labels column:
     </label>
     <input
         id="{{ name }}"
         class="form-control"
         name="{{ name }}"
         value="{{ recipe.args[name] }}"
-        patterns="^{{ vars.filters_pattern }}$"
+        pattern="^{{ vars.filters_pattern }}$"
         title="{{ vars.filters_help }}"
+        required="required"
         placeholder="{{ vars.filters_placeholder }}"
         />
   </div>
 
-  {% set name='fill-where%02d' % n %}
-  <div class="form-group">
+  {% set name='implode-value-pattern%02d' % n %}
+  <div class="form-group required">
     <label for="{{ name }}">
-      Fill only in rows matching this query
+      Values column:
     </label>
     <input
         id="{{ name }}"
         class="form-control"
         name="{{ name }}"
         value="{{ recipe.args[name] }}"
-        pattern="^{{ vars.query_pattern }}$"
-        title="{{ vars.query_help }}"
-        placeholder="{{ vars.query_placeholder }}"
+        pattern="^{{ vars.filters_pattern }}$"
+        title="{{ vars.filters_help }}"
+        required="required"
+        placeholder="{{ vars.filters_placeholder }}"
         />
   </div>
 
 </div>
```

### Comparing `hxl-proxy-1.9.1/hxl_proxy/templates/includes/filters/sort.html` & `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/sort.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 <div class="filter-sort filter-body">
   {% import 'includes/filters/filter-variables.j2' as vars %}
   <p class="doc">
     {% with key='Sort-rows-filter' %}{% include "includes/help.html" %}{% endwith %}
     Sort the records in a HXL dataset
   </p>
 
+  {% include 'includes/filters/label-field.html' %}
+
   {% set name='sort-tags{0:02}'.format(n) %}
   <div class="form-group">
     <label for="{{ name }}">Use these tags for sorting.</label>
     <input
         id="{{ name }}"
         class="form-control" name="{{ name }}"
         value="{{ recipe.args[name] }}"
```

### Comparing `hxl-proxy-1.9.1/hxl_proxy/templates/includes/data-tabs.html` & `hxl-proxy-2.0/hxl_proxy/templates/includes/data-tabs.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-<ul class="nav nav-tabs"> 
+<ul class="nav nav-tabs">
+  {% if not recipe.recipe_id %}
   <li class="{% if facet=='source' %}active{% endif %}">
     <a href="{{ data_url_for('data_source', recipe) }}">
       Source
     </a>
   </li>
   {% if recipe.args.url %}
   {% if using_tagger_p(recipe) or facet=='tagger' %}
   <li class="{% if facet=='tagger' %}active{% endif %}">
     <a href="{{ data_url_for('data_tagger', recipe) }}">
       Tags
     </a>
   </li>
   {% endif %}
+  {% if source or using_tagger_p(recipe) or in_logger %}
   <li class="{% if facet=='edit' %}active{% endif %}">
     <a href="{{ data_url_for('data_edit', recipe) }}">
       Recipe
     </a>
   </li>
-  <li class="{% if facet=='save' %}active{% endif %}">
-    <a href="{{ data_url_for('data_save', recipe) }}">
-      {% if recipe.recipe_id %}
-      Update
-      {% else %}
-      Save
-      {% endif %}
-    </a>
-  </li>
   {% endif %}
   <li class="{% if facet=='view' %}active{% endif %}">
     <a href="{{ data_url_for('data_view', recipe) }}">
       View
     </a>
   </li>
+  <li class="{% if facet=='logs' %}active{% endif %}">
+    <a href="{{ data_url_for('data_logs', recipe) }}">
+      Logs
+    </a>
+  </li>
+  {% endif %}
+  {% endif %}
 </ul>
```

#### html2text {}

```diff
@@ -1,9 +1,11 @@
+    * {% if not recipe.recipe_id %}
     * Source
     * {% if recipe.args.url %} {% if using_tagger_p(recipe) or facet=='tagger'
       %}
     * Tags
-    * {% endif %}
+    * {% endif %} {% if source or using_tagger_p(recipe) or in_logger %}
     * Recipe
-    * {%_if_recipe.recipe_id_%}_Update_{%_else_%}_Save_{%_endif_%}
     * {% endif %}
     * View
+    * Logs
+    * {% endif %} {% endif %}
```

### Comparing `hxl-proxy-1.9.1/hxl_proxy/templates/includes/headers.html` & `hxl-proxy-2.0/hxl_proxy/templates/includes/headers.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/templates/includes/navbar.html` & `hxl-proxy-2.0/hxl_proxy/templates/includes/navbar.html`

 * *Files 13% similar despite different names*

```diff
@@ -28,36 +28,29 @@
         </li>
         <li class="{% if facet=='validate' %}active{% endif %}">
           <a href="{{ data_url_for('data_validate', recipe) }}">
             <span class="glyphicon glyphicon-ok"></span>
             Validate
           </a>
         </li>
-        <li class="{% if facet=='chart' %}active{% endif %}">
-          <a href="{{ data_url_for('data_chart', recipe) }}">
-            <span class="glyphicon glyphicon-signal"></span>
-            Visualise
-          </a>
-        </li>
-        <li class="{% if facet=='map' %}active{% endif %}">
-          <a href="{{ data_url_for('data_map', recipe) }}">
-            <span class="glyphicon glyphicon-globe"></span>
-            Map
-          </a>
-        </li>
-        {% if recipe.recipe_id and recipe.cloneable %}
+        {% if recipe.recipe_id and recipe.cloneable and not recipe.args.authorization_token %}
         <li>
           <a href="{{ data_url_for('data_view', recipe, cloned=True) }}">
             <span class="glyphicon glyphicon-copy"></span>
             Clone
           </a>
         </li>
         {% endif %}
         {% endif %}
       </ul>
+      {% if session.is_admin %}
+      <form class="navbar-form navbar-right" method="POST" action="/admin/actions/logout">
+        <button type="submit" class="btn btn-danger">Admin logout</button>
+      </form>
+      {% endif %}
       <ul class="nav navbar-nav navbar-right">
         {#
         {* HID stuff commented out for now *}
         {% if g.member %}
         <li class="{% if facet=='settings' %}active{% endif %}">
           <a href="{{ url_for('user_settings') }}">
             <span class="glyphicon glyphicon-user"></span>
```

#### html2text {}

```diff
@@ -1,17 +1,19 @@
  Toggle navigation     [#HXL]
     * _New
     * {% if recipe and recipe.args.url %}
     * _Data
     * _Validate
-    * _Visualise
-    * _Map
-    * {% if recipe.recipe_id and recipe.cloneable %}
+    * {% if recipe.recipe_id and recipe.cloneable and not
+      recipe.args.authorization_token %}
     * _Clone
     * {% endif %} {% endif %}
+{% if session.is_admin %}
+Admin logout
+{% endif %}
     * {# {* HID stuff commented out for now *} {% if g.member %}
     * _{{_g.member.name_given_}}
     * _Logout
     * {% else %}
     * _Login
     * {% endif %} #}
     * _About
```

### Comparing `hxl-proxy-1.9.1/hxl_proxy/pcodes.py` & `hxl-proxy-2.0/hxl_proxy/pcodes.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 License: Public Domain
 Documentation: https://github.com/HXLStandard/hxl-proxy/wiki
 """
 
 import csv, logging, re, requests, requests_cache, sys, werkzeug
 
-from . import app
+from . import app, caching
 
 logger = logging.getLogger(__name__)
 
 #
 # Constants
 #
 COUNTRY_URL_PATTERN = 'http://gistmaps.itos.uga.edu/arcgis/rest/services/COD_External/{country}_pcode/MapServer/layers?f=pjson'
@@ -41,17 +41,17 @@
     @param country: the ISO3 country code (e.g. "GIN")
     @returns: a dict of HXL admin-level names and iTOS levels
     """
     levels = {}
     country = country.upper()
     url = COUNTRY_URL_PATTERN.format(country=country)
 
-    with requests_cache.enabled(
-            app.config.get('REQUEST_CACHE', '/tmp/hxl_proxy_requests'), 
-            expire_after=app.config.get('PCODE_CACHE_TIMEOUT_SECONDS', 604800)
+    with caching.input(
+            namespace=app.config.get('ITOS_CACHE_NAME', 'itos-in'), 
+            timeout=app.config.get('ITOS_CACHE_TIMEOUT', 604800)
     ):
         with requests.get(url) as result:
             data = result.json()
 
     if 'error' in data:
         raise werkzeug.exceptions.NotFound("iTOS P-code service does not support country: {}".format(country))
     for layer in result.json().get('layers'):
@@ -78,17 +78,17 @@
 
     country_levels = get_country_levels(country)
     if not level in country_levels:
         raise werkzeug.exceptions.NotFound("iTOS P-code service does support admin level {} for {}".format(level, country))
 
     # Read the data from iTOS
     url = PCODES_URL_PATTERN.format(country=country, level=country_levels[level])
-    with requests_cache.enabled(
-            app.config.get('REQUEST_CACHE', '/tmp/hxl_proxy_requests'), 
-            expire_after=app.config.get('PCODE_CACHE_TIMEOUT_SECONDS', 604800)
+    with caching.input(
+            namespace=app.config.get('ITOS_CACHE_NAME', 'itos-in'),
+            timeout=app.config.get('ITOS_CACHE_TIMEOUT', 604800)
     ):
         with requests.get(url) as result:
             data = result.json()
     if "error" in data:
         raise werkzeug.exceptions.BadGateway('Unexpected iTOS P-code service error (try again)')
 
     # Set up the header and hashtag rows
```

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/images/hxl-logo-white.png` & `hxl-proxy-2.0/hxl_proxy/static/images/hxl-logo-white.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/images/csv-icon.png` & `hxl-proxy-2.0/hxl_proxy/static/images/csv-icon.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/images/dropbox-logo.png` & `hxl-proxy-2.0/hxl_proxy/static/images/dropbox-logo.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/images/hdx-logo.png` & `hxl-proxy-2.0/hxl_proxy/static/images/hdx-logo.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/images/google-drive-logo.png` & `hxl-proxy-2.0/hxl_proxy/static/images/google-drive-logo.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/images/json-icon.png` & `hxl-proxy-2.0/hxl_proxy/static/images/json-icon.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/compat/respond.min.js` & `hxl-proxy-2.0/hxl_proxy/static/compat/respond.min.js`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/compat/html5shiv.min.js` & `hxl-proxy-2.0/hxl_proxy/static/compat/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/compat/ie10-viewport-bug-workaround.js` & `hxl-proxy-2.0/hxl_proxy/static/compat/ie10-viewport-bug-workaround.js`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/jquery/jquery.js` & `hxl-proxy-2.0/hxl_proxy/static/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/jquery/jquery.csv.js` & `hxl-proxy-2.0/hxl_proxy/static/jquery/jquery.csv.js`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/jquery/jquery-ui.min.js` & `hxl-proxy-2.0/hxl_proxy/static/jquery/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/jquery/jquery.ui.touch-punch.min.js` & `hxl-proxy-2.0/hxl_proxy/static/jquery/jquery.ui.touch-punch.min.js`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/hxl-proxy.css` & `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/hxl-proxy.css`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,13 @@
-#map-container {
-    position: relative;
-    height: 480px;
-}
-
-#map-div {
-    height: 100%;
-    width: 100%;
-}
-
-#map-loading {
-    display: none;
-    margin: auto;
-    position: absolute;
-    height: 4em;
-    width: 100%;
-    text-align: center;
-    top: 0;
-    bottom: 0;
-    left: 0;
-    right: 0;
-    color: #333333;
-    font-size: 120%;
-}
-
 body {
     padding-top: 50px;
 }
 
 main {
+    margin-top: 50px;
     overflow: auto;
 }
 
 .messages {
     margin-top: 1rem;
 }
 
@@ -208,33 +184,57 @@
 
 ol.filter-list {
     list-style: none;
     padding-left: 0;
 }
 
 ol.filter-list li.filter {
-    margin-bottom: 1ex;
+    position: relative;
+    margin-bottom: 2ex;
+    margin-left: 2em;
 }
 
 ol.filter-list li.placeholder:before {
     position: absolute;
     content: "\21D2";
     margin-left: -1em;
 }
 
+ol.filter-list .handle {
+    position: absolute;
+    left: -2em;;
+    top: .4ex;
+}
+
+ol.filter-list .filter-name {
+    display: inline-block;
+    font-weight: bold;
+}
+
+ol.filter-list .filter-label {
+    display: block;
+    font-style: italic;
+}
+
 ol.filter-list .filter-delete {
-    float: right;
+    position: absolute;
+    right: 0;
+    top: .4ex;
 }
 
 .help-link {
     float: right;
 }
 
-.handle {
-    margin-right: 1em;
+.form-group .help, .checkbox .help {
+    margin-top: 0;
+    padding-top: 0;
+    font-size: 83.333333%;
+    color: #555555;
+    font-style: italic;
 }
 
 fieldset legend {
     font-size: 120%;
     font-weight: bold;
 }
 
@@ -249,7 +249,11 @@
     margin-top: 3ex;
 }
 
 .filter-list {
     margin-top: 3ex;
     margin-bottom: 3ex;
 }
+
+.highlighted {
+    background: #F3E5AB;
+}
```

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/android-icon-72x72.png` & `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/android-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/favicon-16x16.png` & `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-57x57.png` & `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-57x57.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-precomposed.png` & `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-precomposed.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-60x60.png` & `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-60x60.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/ms-icon-70x70.png` & `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/ms-icon-70x70.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/ms-icon-310x310.png` & `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/ms-icon-310x310.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-120x120.png` & `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-120x120.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/android-icon-192x192.png` & `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/android-icon-192x192.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/ms-icon-144x144.png` & `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/android-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-180x180.png` & `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-180x180.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/android-icon-96x96.png` & `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/android-icon-96x96.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/android-icon-48x48.png` & `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/android-icon-48x48.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/favicon.ico` & `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/favicon.ico`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-114x114.png` & `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-114x114.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/ms-icon-150x150.png` & `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/ms-icon-150x150.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-72x72.png` & `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/android-icon-144x144.png` & `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/android-icon-36x36.png` & `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/android-icon-36x36.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-76x76.png` & `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-76x76.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-152x152.png` & `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-152x152.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/apple-icon.png` & `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/favicon-32x32.png` & `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/favicon-96x96.png` & `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-144x144.png` & `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/ms-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/bootstrap/css/bootstrap-theme.min.css` & `hxl-proxy-2.0/hxl_proxy/static/bootstrap/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/bootstrap/css/bootstrap-theme.css.map` & `hxl-proxy-2.0/hxl_proxy/static/bootstrap/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/bootstrap/css/bootstrap.min.css` & `hxl-proxy-2.0/hxl_proxy/static/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/bootstrap/css/bootstrap.css.map` & `hxl-proxy-2.0/hxl_proxy/static/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/bootstrap/css/bootstrap-theme.css` & `hxl-proxy-2.0/hxl_proxy/static/bootstrap/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/bootstrap/css/bootstrap.css` & `hxl-proxy-2.0/hxl_proxy/static/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.woff2` & `hxl-proxy-2.0/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.svg` & `hxl-proxy-2.0/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.ttf` & `hxl-proxy-2.0/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.woff` & `hxl-proxy-2.0/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.eot` & `hxl-proxy-2.0/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/bootstrap/js/bootstrap.min.js` & `hxl-proxy-2.0/hxl_proxy/static/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `hxl-proxy-1.9.1/hxl_proxy/static/bootstrap/js/bootstrap.js` & `hxl-proxy-2.0/hxl_proxy/static/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

