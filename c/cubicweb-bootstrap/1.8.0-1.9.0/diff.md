# Comparing `tmp/cubicweb-bootstrap-1.8.0.tar.gz` & `tmp/cubicweb-bootstrap-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-bootstrap-1.8.0.tar", last modified: Tue Apr 12 16:38:45 2022, max compression
+gzip compressed data, was "cubicweb-bootstrap-1.9.0.tar", last modified: Thu Nov 24 02:18:45 2022, max compression
```

## Comparing `cubicweb-bootstrap-1.8.0.tar` & `cubicweb-bootstrap-1.9.0.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 16:38:45.346229 cubicweb-bootstrap-1.8.0/
--rw-rw-rw-   0 root         (0) root         (0)      695 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)      505 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      556 2022-04-12 16:38:45.346229 cubicweb-bootstrap-1.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       17 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 16:38:45.330229 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/
--rw-rw-rw-   0 root         (0) root         (0)      974 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      749 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 16:38:45.334229 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/
--rw-rw-rw-   0 root         (0) root         (0)     1737 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/ajax-loader.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 16:38:45.334229 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/css/
--rw-rw-rw-   0 root         (0) root         (0)    26133 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/css/bootstrap-theme.css
--rw-rw-rw-   0 root         (0) root         (0)    23358 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/css/bootstrap-theme.min.css
--rw-rw-rw-   0 root         (0) root         (0)   122932 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/css/bootstrap.min.css
--rw-rw-rw-   0 root         (0) root         (0)     8972 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/cubes.bootstrap.css
--rw-rw-rw-   0 root         (0) root         (0)     1364 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/cubes.bootstrap.cw_compat.css
--rw-rw-rw-   0 root         (0) root         (0)     2979 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/cubes.bootstrap.edition.js
--rw-rw-rw-   0 root         (0) root         (0)      280 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/cubes.bootstrap.js
--rw-rw-rw-   0 root         (0) root         (0)       23 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/cubicweb.form.css
--rw-rw-rw-   0 root         (0) root         (0)      109 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/cubicweb.tableview.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 16:38:45.334229 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/fonts/
--rw-rw-rw-   0 root         (0) root         (0)    20127 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.eot
--rw-rw-rw-   0 root         (0) root         (0)   108738 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.svg
--rw-rw-rw-   0 root         (0) root         (0)    45404 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.ttf
--rw-rw-rw-   0 root         (0) root         (0)    23424 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.woff
--rw-rw-rw-   0 root         (0) root         (0)    18028 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.woff2
--rw-rw-rw-   0 root         (0) root         (0)      308 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/go_next.png
--rw-rw-rw-   0 root         (0) root         (0)      265 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/go_prev.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 16:38:45.334229 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/img/
--rw-rw-rw-   0 root         (0) root         (0)      209 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/img/facet_selected.png
--rw-rw-rw-   0 root         (0) root         (0)      255 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/img/facet_unselected.png
--rw-rw-rw-   0 root         (0) root         (0)      243 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/img/table_down.png
--rw-rw-rw-   0 root         (0) root         (0)      254 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/img/table_sortable.png
--rw-rw-rw-   0 root         (0) root         (0)      247 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/img/table_up.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 16:38:45.334229 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/js/
--rw-rw-rw-   0 root         (0) root         (0)    36817 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/js/bootstrap.min.js
--rw-rw-rw-   0 root         (0) root         (0)     9202 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/logo-cubicweb.svg
--rw-rw-rw-   0 root         (0) root         (0)      459 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/pen_icon.png
--rw-rw-rw-   0 root         (0) root         (0)       86 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/required.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 16:38:45.338229 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/i18n/
--rw-rw-rw-   0 root         (0) root         (0)      203 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/i18n/en.po
--rw-rw-rw-   0 root         (0) root         (0)      203 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/i18n/es.po
--rw-rw-rw-   0 root         (0) root         (0)      203 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/i18n/fr.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 16:38:45.338229 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/migration/
--rw-rw-rw-   0 root         (0) root         (0)     1095 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/migration/postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)     3070 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/site_cubicweb.py
--rw-rw-rw-   0 root         (0) root         (0)      661 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/uiprops.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 16:38:45.342229 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/
--rw-rw-rw-   0 root         (0) root         (0)     1515 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5687 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/basecomponents.py
--rw-rw-rw-   0 root         (0) root         (0)     2495 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/basetemplates.py
--rw-rw-rw-   0 root         (0) root         (0)     3391 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/baseviews.py
--rw-rw-rw-   0 root         (0) root         (0)     2165 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/boxes.py
--rw-rw-rw-   0 root         (0) root         (0)      450 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/component.py
--rw-rw-rw-   0 root         (0) root         (0)     1666 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/cwproperties.py
--rw-rw-rw-   0 root         (0) root         (0)     4705 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/debug.py
--rw-rw-rw-   0 root         (0) root         (0)     1793 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/editforms.py
--rw-rw-rw-   0 root         (0) root         (0)      349 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/facets.py
--rw-rw-rw-   0 root         (0) root         (0)      877 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/formfields.py
--rw-rw-rw-   0 root         (0) root         (0)    11353 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/formrenderers.py
--rw-rw-rw-   0 root         (0) root         (0)     1145 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     1461 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/formwidgets.py
--rw-rw-rw-   0 root         (0) root         (0)     1344 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/htmlwidgets.py
--rw-rw-rw-   0 root         (0) root         (0)     1623 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/ibreadcrumbs.py
--rw-rw-rw-   0 root         (0) root         (0)     7402 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/navigation.py
--rw-rw-rw-   0 root         (0) root         (0)     4769 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/primary.py
--rw-rw-rw-   0 root         (0) root         (0)      962 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/reledit.py
--rw-rw-rw-   0 root         (0) root         (0)     2891 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/startup.py
--rw-rw-rw-   0 root         (0) root         (0)      678 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/tableview.py
--rw-rw-rw-   0 root         (0) root         (0)     2264 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/tabs.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/tag.py
--rw-rw-rw-   0 root         (0) root         (0)     1072 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 16:38:45.330229 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap.egg-info/
--rw-r--r--   0 root         (0) root         (0)      556 2022-04-12 16:38:44.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2977 2022-04-12 16:38:45.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-04-12 16:38:44.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2022-04-12 16:38:45.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-04-12 16:38:44.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       37 2022-04-12 16:38:45.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2022-04-12 16:38:45.000000 cubicweb-bootstrap-1.8.0/cubicweb_bootstrap.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 16:38:45.342229 cubicweb-bootstrap-1.8.0/doc/
--rw-rw-rw-   0 root         (0) root         (0)     4605 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/doc/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      779 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/doc/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     7382 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/doc/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      469 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/doc/dependencies.rst
--rw-rw-rw-   0 root         (0) root         (0)      209 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/doc/header.rst
--rw-rw-rw-   0 root         (0) root         (0)      396 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/doc/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      141 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/doc/primary.rst
--rw-rw-rw-   0 root         (0) root         (0)      983 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/doc/release_0.5.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      257 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/doc/release_0.6.0.rst
--rw-r--r--   0 root         (0) root         (0)       38 2022-04-12 16:38:45.346229 cubicweb-bootstrap-1.8.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2557 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 16:38:45.346229 cubicweb-bootstrap-1.8.0/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 16:38:45.346229 cubicweb-bootstrap-1.8.0/test/data/
--rw-rw-rw-   0 root         (0) root         (0)       10 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/test/data/bootstrap_cubes
--rw-rw-rw-   0 root         (0) root         (0)     2324 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/test/test_bootstrap.py
--rw-rw-rw-   0 root         (0) root         (0)      787 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/test/unittest_views.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2022-04-12 16:38:32.000000 cubicweb-bootstrap-1.8.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:18:45.452827 cubicweb-bootstrap-1.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)      974 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)      505 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      556 2022-11-24 02:18:45.448827 cubicweb-bootstrap-1.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       17 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:18:45.436827 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/
+-rw-rw-rw-   0 root         (0) root         (0)      974 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      749 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:18:45.436827 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/
+-rw-rw-rw-   0 root         (0) root         (0)     1737 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/ajax-loader.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:18:45.440827 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/css/
+-rw-rw-rw-   0 root         (0) root         (0)    26133 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/css/bootstrap-theme.css
+-rw-rw-rw-   0 root         (0) root         (0)    23358 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/css/bootstrap-theme.min.css
+-rw-rw-rw-   0 root         (0) root         (0)   122932 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/css/bootstrap.min.css
+-rw-rw-rw-   0 root         (0) root         (0)     8972 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/cubes.bootstrap.css
+-rw-rw-rw-   0 root         (0) root         (0)     1364 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/cubes.bootstrap.cw_compat.css
+-rw-rw-rw-   0 root         (0) root         (0)     2979 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/cubes.bootstrap.edition.js
+-rw-rw-rw-   0 root         (0) root         (0)      280 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/cubes.bootstrap.js
+-rw-rw-rw-   0 root         (0) root         (0)       23 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/cubicweb.form.css
+-rw-rw-rw-   0 root         (0) root         (0)      109 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/cubicweb.tableview.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:18:45.440827 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)    20127 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.eot
+-rw-rw-rw-   0 root         (0) root         (0)   108738 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.svg
+-rw-rw-rw-   0 root         (0) root         (0)    45404 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)    23424 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.woff
+-rw-rw-rw-   0 root         (0) root         (0)    18028 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.woff2
+-rw-rw-rw-   0 root         (0) root         (0)      308 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/go_next.png
+-rw-rw-rw-   0 root         (0) root         (0)      265 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/go_prev.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:18:45.440827 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/img/
+-rw-rw-rw-   0 root         (0) root         (0)      209 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/img/facet_selected.png
+-rw-rw-rw-   0 root         (0) root         (0)      255 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/img/facet_unselected.png
+-rw-rw-rw-   0 root         (0) root         (0)      243 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/img/table_down.png
+-rw-rw-rw-   0 root         (0) root         (0)      254 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/img/table_sortable.png
+-rw-rw-rw-   0 root         (0) root         (0)      247 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/img/table_up.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:18:45.440827 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/js/
+-rw-rw-rw-   0 root         (0) root         (0)    36817 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/js/bootstrap.min.js
+-rw-rw-rw-   0 root         (0) root         (0)     9202 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/logo-cubicweb.svg
+-rw-rw-rw-   0 root         (0) root         (0)      459 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/pen_icon.png
+-rw-rw-rw-   0 root         (0) root         (0)       86 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/required.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:18:45.440827 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)      203 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)      203 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)      203 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/i18n/fr.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:18:45.440827 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/migration/
+-rw-rw-rw-   0 root         (0) root         (0)     1095 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)     3070 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/site_cubicweb.py
+-rw-rw-rw-   0 root         (0) root         (0)      661 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/uiprops.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:18:45.448827 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/
+-rw-rw-rw-   0 root         (0) root         (0)     1515 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5687 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/basecomponents.py
+-rw-rw-rw-   0 root         (0) root         (0)     2495 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/basetemplates.py
+-rw-rw-rw-   0 root         (0) root         (0)     3391 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/baseviews.py
+-rw-rw-rw-   0 root         (0) root         (0)     2165 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/boxes.py
+-rw-rw-rw-   0 root         (0) root         (0)      450 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/component.py
+-rw-rw-rw-   0 root         (0) root         (0)     1666 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/cwproperties.py
+-rw-rw-rw-   0 root         (0) root         (0)     4705 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/debug.py
+-rw-rw-rw-   0 root         (0) root         (0)     1793 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/editforms.py
+-rw-rw-rw-   0 root         (0) root         (0)      349 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/facets.py
+-rw-rw-rw-   0 root         (0) root         (0)      877 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/formfields.py
+-rw-rw-rw-   0 root         (0) root         (0)    11353 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/formrenderers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1145 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/formwidgets.py
+-rw-rw-rw-   0 root         (0) root         (0)     1344 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/htmlwidgets.py
+-rw-rw-rw-   0 root         (0) root         (0)     1623 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/ibreadcrumbs.py
+-rw-rw-rw-   0 root         (0) root         (0)     7406 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/navigation.py
+-rw-rw-rw-   0 root         (0) root         (0)     4769 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/primary.py
+-rw-rw-rw-   0 root         (0) root         (0)      962 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/reledit.py
+-rw-rw-rw-   0 root         (0) root         (0)     2891 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/startup.py
+-rw-rw-rw-   0 root         (0) root         (0)      678 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/tableview.py
+-rw-rw-rw-   0 root         (0) root         (0)     2264 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/tabs.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/tag.py
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:18:45.436827 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      556 2022-11-24 02:18:44.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2977 2022-11-24 02:18:45.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-24 02:18:44.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2022-11-24 02:18:45.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-24 02:18:44.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       37 2022-11-24 02:18:45.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2022-11-24 02:18:45.000000 cubicweb-bootstrap-1.9.0/cubicweb_bootstrap.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:18:45.448827 cubicweb-bootstrap-1.9.0/doc/
+-rw-rw-rw-   0 root         (0) root         (0)     4605 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/doc/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      779 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/doc/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7382 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/doc/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      469 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/doc/dependencies.rst
+-rw-rw-rw-   0 root         (0) root         (0)      209 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/doc/header.rst
+-rw-rw-rw-   0 root         (0) root         (0)      396 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/doc/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      141 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/doc/primary.rst
+-rw-rw-rw-   0 root         (0) root         (0)      983 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/doc/release_0.5.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      257 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/doc/release_0.6.0.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2022-11-24 02:18:45.452827 cubicweb-bootstrap-1.9.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2557 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:18:45.448827 cubicweb-bootstrap-1.9.0/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-24 02:18:45.448827 cubicweb-bootstrap-1.9.0/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)       10 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)     2324 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/test/test_bootstrap.py
+-rw-rw-rw-   0 root         (0) root         (0)      787 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/test/unittest_views.py
+-rw-rw-rw-   0 root         (0) root         (0)      980 2022-11-24 02:18:33.000000 cubicweb-bootstrap-1.9.0/tox.ini
```

### Comparing `cubicweb-bootstrap-1.8.0/PKG-INFO` & `cubicweb-bootstrap-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubicweb-bootstrap
-Version: 1.8.0
+Version: 1.9.0
 Summary: UNKNOWN
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-bootstrap
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/__init__.py` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/__pkginfo__.py` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/__pkginfo__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # pylint: disable=W0622
 """cubicweb-bootstrap application packaging information"""
 
 modname = 'bootstrap'
 distname = 'cubicweb-bootstrap'
 
-numversion = (1, 8, 0)
+numversion = (1, 9, 0)
 version = '.'.join(str(num) for num in numversion)
 
 license = 'LGPL'
 author = 'LOGILAB S.A. (Paris, FRANCE)'
 author_email = 'contact@logilab.fr'
 description = ''
 web = 'https://forge.extranet.logilab.fr/cubicweb/cubes/%s' % distname
 
 __depends__ = {
-    'cubicweb': ">= 3.26.0, < 3.38.0",
+    'cubicweb': ">= 3.38.0, < 3.39.0",
     'six': '>= 1.12.0',
 }
 __recommends__ = {}
 
 classifiers = [
     'Environment :: Web Environment',
     'Framework :: CubicWeb',
```

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/ajax-loader.gif` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/css/bootstrap-theme.css` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/css/bootstrap-theme.min.css` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/css/bootstrap.min.css` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/cubes.bootstrap.css` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/cubes.bootstrap.css`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/cubes.bootstrap.cw_compat.css` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/cubes.bootstrap.cw_compat.css`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/cubes.bootstrap.edition.js` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/cubes.bootstrap.edition.js`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.eot` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.svg` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.ttf` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.woff` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.woff2` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/js/bootstrap.min.js` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/data/logo-cubicweb.svg` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/data/logo-cubicweb.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/migration/postcreate.py` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/site_cubicweb.py` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/site_cubicweb.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # You should have received a copy of the GNU Lesser General Public License along
 # with this program. If not, see <https://www.gnu.org/licenses/>.
 """this is where you could register procedures for instance"""
 __docformat__ = "restructuredtext en"
 
 from logilab.common.decorators import monkeypatch
 
-from cubicweb.web import formwidgets, stdmsgs
+from cubicweb_web import formwidgets, stdmsgs
 
 from cubicweb_bootstrap import monkeypatch_default_value
 
 # put there monkeypatches of things that aren't reloaded automatically
 
 # monkeypatches #############################################################
```

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/uiprops.py` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/uiprops.py`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/__init__.py` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 :contact: https://www.logilab.fr/ -- mailto:contact@logilab.fr
 """
 
 from logilab.common.decorators import monkeypatch
 
 from cubicweb import view as cwview
 from cubicweb.schema import display_name
-from cubicweb.web.views.basetemplates import HTMLHeader
+from cubicweb_web.views.basetemplates import HTMLHeader
 
 # do not wrap cell_calls with <div class="section">
 
 cwview.View.add_div_section = False
 
 
 @monkeypatch(cwview.View)
```

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/basecomponents.py` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/basecomponents.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 __docformat__ = "restructuredtext en"
 
 from logilab.common.decorators import monkeypatch
 from logilab.mtconverter import xml_escape
 
-from cubicweb.web.views import basecomponents
+from cubicweb_web.views import basecomponents
 from cubicweb.uilib import js
 
 from cubicweb_bootstrap.views import utils
 from cubicweb_bootstrap import CW_325
 
 
 basecomponents.CookieLoginComponent._html = (
```

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/basetemplates.py` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/basetemplates.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 __docformat__ = "restructuredtext en"
 
 from logilab.common.decorators import monkeypatch
 from logilab.mtconverter import xml_escape
 
 from cubicweb import _
-from cubicweb.web import formwidgets as fw
-from cubicweb.web.views import basetemplates  # import LogForm, LogFormView
+from cubicweb_web import formwidgets as fw
+from cubicweb_web.views import basetemplates  # import LogForm, LogFormView
 
 from cubicweb_bootstrap import CW_325
 
 
 basetemplates.LogForm.needs_css = ()
 basetemplates.LogForm.form_buttons = [
     fw.ResetButton(label=_('cancel'),
```

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/baseviews.py` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/baseviews.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 
 __docformat__ = "restructuredtext en"
 
 from logilab.common.decorators import monkeypatch
 from six.moves import range
 
-from cubicweb.web.views import baseviews
+from cubicweb_web.views import baseviews
 
 baseviews.ListView.listtag = 'ul'
 
 
 @monkeypatch(baseviews.ListView)
 def call(self, klass='list-striped', title=None, subvid=None, listid=None, **kwargs):
     """display a list of entities by calling their <item_vid> view
```

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/boxes.py` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/boxes.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 __docformat__ = "restructuredtext en"
 
 from logilab.common.decorators import monkeypatch
 from logilab.mtconverter import xml_escape
 
 from cubicweb.utils import wrap_on_write
-from cubicweb.web.views import boxes
+from cubicweb_web.views import boxes
 
 from cubicweb_bootstrap import CW_325
 
 boxes.SearchBox.formdef = (
     u'<form action="%(action)s" id="search_box" class="navbar-form" role="search">\n'
     u'  <input id="norql" type="text" accesskey="q" tabindex="%(tabindex1)s"'
     u'    title="search text" value="%(value)s" name="rql"'
```

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/cwproperties.py` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/cwproperties.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 :copyright: 2013 LOGILAB S.A. (Paris, FRANCE), license is LGPL.
 :contact: https://www.logilab.fr/ -- mailto:contact@logilab.fr
 """
 
 __docformat__ = "restructuredtext en"
 
 from logilab.common.decorators import monkeypatch
-from cubicweb.web.views.cwproperties import (
+from cubicweb_web.views.cwproperties import (
     SystemCWPropertiesForm, make_togglable_link
 )
 
 
 @monkeypatch(SystemCWPropertiesForm)
 def wrap_main_form(self, group, label, form):
     label += u' <span class="caret"></span>'
```

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/debug.py` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/debug.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from six import text_type
 
 from logilab.common.decorators import monkeypatch
 
 from logilab.mtconverter import xml_escape
 
 from cubicweb import BadConnectionId
-from cubicweb.web.views import debug
+from cubicweb_web.views import debug
 
 
 def dict_to_html(w, dict):
     # XHTML doesn't allow emtpy <ul> nodes
     if dict:
         w(u'<dl>')
         for key in sorted(dict):
@@ -68,15 +68,15 @@
     w(u'<h2>%s</h2>' % _('Web server'))
     w(u'<table class="table table-striped table-condensed">')
     w(u'<tr><th>%s</th><td>%s</td></tr>' % (
         _('base url'), req.base_url()))
     w(u'<tr><th>%s</th><td>%s</td></tr>' % (
         _('data directory url'), req.datadir_url))
     w(u'</table>')
-    from cubicweb.web.application import SESSION_MANAGER
+    from cubicweb_web.application import SESSION_MANAGER
     if SESSION_MANAGER is not None and req.user.is_in_group('managers'):
         sessions = SESSION_MANAGER.current_sessions()
         w(u'<h3>%s</h3>' % _('opened web sessions'))
         if sessions:
             w(u'<ul>')
             for session in sessions:
                 if hasattr(session, 'cnx'):
```

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/editforms.py` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/editforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 :copyright: 2013 LOGILAB S.A. (Paris, FRANCE), license is LGPL.
 :contact: https://www.logilab.fr/ -- mailto:contact@logilab.fr
 """
 
 __docformat__ = "restructuredtext en"
 
 from logilab.common.decorators import monkeypatch
-from cubicweb.web.views import editforms
+from cubicweb_web.views import editforms
 
 
 @monkeypatch(editforms.EditionFormView)
 def form_title(self, entity):
     """the form view title"""
     ptitle = self._cw._(self.title)
     self.w(u'<div class="formTitle"><h1>%s %s</h1></div>' % (
```

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/formfields.py` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/formfields.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 
 __docformat__ = "restructuredtext en"
 
 from logilab.common.decorators import monkeypatch
 
 from cubicweb.utils import UStringIO
-from cubicweb.web import formfields
+from cubicweb_web import formfields
 
 
 @monkeypatch(formfields.FileField)
 def render_subfield(self, form, field, renderer):
     data = UStringIO()  # XXX add support for tracewrites
     w = data.write
     w(u'<div class="row">')
```

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/formrenderers.py` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/formrenderers.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from warnings import warn
 
 from logilab.common.decorators import monkeypatch
 
 from cubicweb import tags
 from cubicweb.utils import support_args
-from cubicweb.web.views import formrenderers
+from cubicweb_web.views import formrenderers
 
 
 @monkeypatch(formrenderers.EntityCompositeFormRenderer)
 def render_fields(self, w, form, values):
     if form.parent_form is None:
         # We should probably take those CSS classes to uiprops.py
         w(u'<table class="table table-striped table-bordered table-condensed">')
```

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/forms.py` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,14 @@
 # You should have received a copy of the GNU Lesser General Public License along
 # with this program. If not, see <https://www.gnu.org/licenses/>.
 """bootstrap implementation of forms"""
 
 __docformat__ = "restructuredtext en"
 
 
-from cubicweb.web.views.forms import FieldsForm
-from cubicweb.web.views.autoform import AutomaticEntityForm
+from cubicweb_web.views.forms import FieldsForm
+from cubicweb_web.views.autoform import AutomaticEntityForm
 
 # Forms
 FieldsForm.needs_js += ('cubes.bootstrap.edition.js',)
 FieldsForm.needs_css = ()
 FieldsForm.cssclass = AutomaticEntityForm.cssclass = 'form-horizontal'
```

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/formwidgets.py` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/formwidgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 __docformat__ = "restructuredtext en"
 
 from logilab.common.decorators import monkeypatch
 from logilab.mtconverter import xml_escape
 
 from cubicweb import tags, __version__ as cwver
-from cubicweb.web import formwidgets
+from cubicweb_web import formwidgets
 
 from cubicweb_bootstrap import CW_325
 
 
 # Buttons
 @monkeypatch(formwidgets.Button)
 def render(self, form, field=None, renderer=None):
```

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/htmlwidgets.py` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/htmlwidgets.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 :contact: https://www.logilab.fr/ -- mailto:contact@logilab.fr
 """
 
 __docformat__ = "restructuredtext en"
 
 from logilab.common.decorators import monkeypatch
 
-from cubicweb.web import htmlwidgets
-from cubicweb.web.component import Separator
+from cubicweb_web import htmlwidgets
+from cubicweb_web.component import Separator
 
 
 @monkeypatch(Separator)
 def render(self, w):
     w(u'<li class="divider"></li>')
```

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/ibreadcrumbs.py` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/ibreadcrumbs.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 
 __docformat__ = "restructuredtext en"
 
 from logilab.common.decorators import monkeypatch
 
 from cubicweb.entity import Entity
-from cubicweb.web.views import ibreadcrumbs
+from cubicweb_web.views import ibreadcrumbs
 
 
 ibreadcrumbs.BreadCrumbEntityVComponent.css_class = u'breadcrumb'
 
 
 @monkeypatch(ibreadcrumbs.BreadCrumbEntityVComponent)
 def open_breadcrumbs(self, w):
```

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/navigation.py` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/navigation.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 :contact: https://www.logilab.fr/ -- mailto:contact@logilab.fr
 """
 
 from logilab.common.decorators import monkeypatch
 
 from logilab.mtconverter import xml_escape
 
-from cubicweb.view import View
-from cubicweb.web.component import NavigationComponent
+from cubicweb_web.view import View
+from cubicweb_web.component import NavigationComponent
 
-from cubicweb.web.views.navigation import (NextPrevNavigationComponent,
+from cubicweb_web.views.navigation import (NextPrevNavigationComponent,
                                            SortedNavigation,
                                            PageNavigation,
                                            PageNavigationSelect)
 from cubicweb_bootstrap import CW_323
 
 __docformat__ = "restructuredtext en"
```

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/primary.py` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/primary.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 
 __docformat__ = "restructuredtext en"
 
 from logilab.common.decorators import monkeypatch
 from logilab.mtconverter import xml_escape
 
-from cubicweb.web.views import primary
+from cubicweb_web.views import primary
 
 
 @monkeypatch(primary.PrimaryView)
 def render_entity(self, entity):
     self.render_entity_toolbox(entity)
     self.render_entity_title(entity)
     # entity's attributes and relations, excluding meta data
```

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/reledit.py` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/reledit.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 :organization: Logilab
 :copyright: 2013-2022 LOGILAB S.A. (Paris, FRANCE), license is LGPL.
 :contact: https://www.logilab.fr/ -- mailto:contact@logilab.fr
 """
 __docformat__ = "restructuredtext en"
 
-from cubicweb.web.views.reledit import AutoClickAndEditFormView
+from cubicweb_web.views.reledit import AutoClickAndEditFormView
 AutoClickAndEditFormView._addzone = u' <span class="glyphicon glyphicon-plus"></span>'
 AutoClickAndEditFormView._deletezone = u' <span class="glyphicon glyphicon-remove"></span>'
 AutoClickAndEditFormView._editzone = u' <span class="glyphicon glyphicon-pencil"></span>'
 
 try:
     from cubicweb_inlinedit.views import reledit
 except ImportError:
```

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/startup.py` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/startup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 __docformat__ = "restructuredtext en"
 
 from logilab.common.decorators import monkeypatch
 from logilab.common.textutils import unormalize
 from logilab.mtconverter import xml_escape
 
-from cubicweb.web.views import startup, uicfg
+from cubicweb_web.views import startup, uicfg
 
 startup.ManageView.box_html = u'''<div class="panel panel-default">
     <div class="panel-heading">
         <div class="panel-title">%(title)s</div>
     </div>
     <div class="panel-body">%(content)s</div>
     </div>'''
```

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/tableview.py` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/tableview.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 :contact: https://www.logilab.fr/ -- mailto:contact@logilab.fr
 """
 
 __docformat__ = "restructuredtext en"
 
 from logilab.common.decorators import monkeypatch
 
-from cubicweb.web.views import tableview
+from cubicweb_web.views import tableview
 
 tableview.TableLayout.cssclass = 'listing table table-bordered table-condensed'
 
 
 _row_attributes = tableview.TableLayout.row_attributes
```

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/tabs.py` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/tabs.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 
 __docformat__ = "restructuredtext en"
 
 from logilab.common.decorators import monkeypatch
 
 from cubicweb import utils
-from cubicweb.web.views import tabs
+from cubicweb_web.views import tabs
 
 
 @monkeypatch(tabs.TabsMixin)
 def render_tabs(self, tabs, default, entity=None):
     # delegate to the default tab if there is more than one entity
     # in the result set (tabs are pretty useless there)
     if entity and len(self.cw_rset) > 1:
```

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/tag.py` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/tag.py`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap/views/utils.py` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap/views/utils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap.egg-info/PKG-INFO` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubicweb-bootstrap
-Version: 1.8.0
+Version: 1.9.0
 Summary: UNKNOWN
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-bootstrap
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `cubicweb-bootstrap-1.8.0/cubicweb_bootstrap.egg-info/SOURCES.txt` & `cubicweb-bootstrap-1.9.0/cubicweb_bootstrap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.8.0/doc/Makefile` & `cubicweb-bootstrap-1.9.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.8.0/doc/README.rst` & `cubicweb-bootstrap-1.9.0/doc/README.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.8.0/doc/conf.py` & `cubicweb-bootstrap-1.9.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.8.0/doc/release_0.5.0.rst` & `cubicweb-bootstrap-1.9.0/doc/release_0.5.0.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.8.0/setup.py` & `cubicweb-bootstrap-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.8.0/test/test_bootstrap.py` & `cubicweb-bootstrap-1.9.0/test/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.8.0/test/unittest_views.py` & `cubicweb-bootstrap-1.9.0/test/unittest_views.py`

 * *Files identical despite different names*

### Comparing `cubicweb-bootstrap-1.8.0/tox.ini` & `cubicweb-bootstrap-1.9.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tox]
-envlist = py27, py3, flake8, check-manifest, yamllint
+envlist =  py3, flake8, check-manifest, yamllint
 
 [testenv]
 deps =
   pytest
   git+https://github.com/psycojoker/pytest-capture-deprecatedwarnings
 commands =
   {envpython} -m pytest {posargs}
```

