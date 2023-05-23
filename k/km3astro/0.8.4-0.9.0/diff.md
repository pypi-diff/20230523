# Comparing `tmp/km3astro-0.8.4.tar.gz` & `tmp/km3astro-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/km3astro-0.8.4.tar", last modified: Wed Feb 10 11:17:55 2021, max compression
+gzip compressed data, was "dist/km3astro-0.9.0.tar", last modified: Mon May  2 15:06:16 2022, max compression
```

## Comparing `km3astro-0.8.4.tar` & `km3astro-0.9.0.tar`

### file list

```diff
@@ -1,72 +1,75 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-10 11:17:55.000000 km3astro-0.8.4/
--rw-rw-rw-   0 root         (0) root         (0)      270 2021-02-09 11:36:49.000000 km3astro-0.8.4/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)      837 2021-02-09 11:36:49.000000 km3astro-0.8.4/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     3640 2021-02-10 11:11:47.000000 km3astro-0.8.4/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      569 2021-02-09 11:36:49.000000 km3astro-0.8.4/.rtd-environment.yml
--rw-rw-rw-   0 root         (0) root         (0)     1109 2021-02-09 11:36:49.000000 km3astro-0.8.4/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     6678 2021-02-09 11:36:49.000000 km3astro-0.8.4/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)     1513 2021-02-09 11:36:49.000000 km3astro-0.8.4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      188 2021-02-09 11:36:49.000000 km3astro-0.8.4/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      912 2021-02-09 11:51:28.000000 km3astro-0.8.4/Makefile
--rw-r--r--   0 root         (0) root         (0)     1466 2021-02-10 11:17:55.000000 km3astro-0.8.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      796 2021-02-09 11:36:49.000000 km3astro-0.8.4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-10 11:17:55.000000 km3astro-0.8.4/doc/
--rw-rw-rw-   0 root         (0) root         (0)     7693 2021-02-09 11:36:49.000000 km3astro-0.8.4/doc/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-10 11:17:55.000000 km3astro-0.8.4/doc/_static/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-02-09 11:36:49.000000 km3astro-0.8.4/doc/_static/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)    24268 2021-02-09 11:36:49.000000 km3astro-0.8.4/doc/_static/default_gallery_thumbnail.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-10 11:17:55.000000 km3astro-0.8.4/doc/_templates/
--rw-rw-rw-   0 root         (0) root         (0)      767 2021-02-09 11:36:49.000000 km3astro-0.8.4/doc/_templates/module.rst
--rw-rw-rw-   0 root         (0) root         (0)       51 2021-02-09 11:36:49.000000 km3astro-0.8.4/doc/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     3091 2021-02-09 11:36:49.000000 km3astro-0.8.4/doc/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      257 2021-02-09 11:36:49.000000 km3astro-0.8.4/doc/contribute.rst
--rw-rw-rw-   0 root         (0) root         (0)     1788 2021-02-09 11:36:49.000000 km3astro-0.8.4/doc/coordinates.rst
--rw-rw-rw-   0 root         (0) root         (0)       33 2021-02-09 11:36:49.000000 km3astro-0.8.4/doc/dev.rst
--rw-rw-rw-   0 root         (0) root         (0)      534 2021-02-09 11:36:49.000000 km3astro-0.8.4/doc/doc.rst
--rw-rw-rw-   0 root         (0) root         (0)       70 2021-02-09 11:36:49.000000 km3astro-0.8.4/doc/examples.rst
--rw-rw-rw-   0 root         (0) root         (0)      366 2021-02-09 11:36:49.000000 km3astro-0.8.4/doc/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-10 11:17:55.000000 km3astro-0.8.4/doc/modules/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-10 11:17:55.000000 km3astro-0.8.4/doc/modules/generated/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-02-09 11:36:49.000000 km3astro-0.8.4/doc/modules/generated/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-10 11:17:55.000000 km3astro-0.8.4/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-02-09 11:36:49.000000 km3astro-0.8.4/examples/README.txt
--rw-rw-rw-   0 root         (0) root         (0)     2660 2021-02-09 11:36:49.000000 km3astro-0.8.4/examples/plot_benchmarks.py
--rw-rw-rw-   0 root         (0) root         (0)     2921 2021-02-09 11:36:49.000000 km3astro-0.8.4/examples/plot_local_to_equatorial.py
--rw-rw-rw-   0 root         (0) root         (0)     1425 2021-02-09 11:36:49.000000 km3astro-0.8.4/examples/plot_source_separation.py
--rw-rw-rw-   0 root         (0) root         (0)     1682 2021-02-09 11:36:49.000000 km3astro-0.8.4/examples/plot_sun_in_local.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-10 11:17:55.000000 km3astro-0.8.4/km3astro/
--rw-rw-rw-   0 root         (0) root         (0)      181 2021-02-09 11:36:49.000000 km3astro-0.8.4/km3astro/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      548 2021-02-09 11:36:49.000000 km3astro-0.8.4/km3astro/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)     1442 2021-02-09 11:36:49.000000 km3astro-0.8.4/km3astro/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     9493 2021-02-09 11:36:49.000000 km3astro-0.8.4/km3astro/coord.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-10 11:17:55.000000 km3astro-0.8.4/km3astro/data/
--rw-rw-rw-   0 root         (0) root         (0)    18624 2021-02-09 11:36:49.000000 km3astro-0.8.4/km3astro/data/orca_sun_isup.h5
--rw-rw-rw-   0 root         (0) root         (0)      359 2021-02-09 11:36:49.000000 km3astro-0.8.4/km3astro/extras.py
--rw-rw-rw-   0 root         (0) root         (0)      976 2021-02-09 11:36:49.000000 km3astro-0.8.4/km3astro/plot.py
--rw-rw-rw-   0 root         (0) root         (0)     1960 2021-02-09 11:36:49.000000 km3astro-0.8.4/km3astro/random.py
--rw-rw-rw-   0 root         (0) root         (0)      756 2021-02-09 11:36:49.000000 km3astro-0.8.4/km3astro/sources.py
--rw-rw-rw-   0 root         (0) root         (0)      603 2021-02-09 11:36:49.000000 km3astro-0.8.4/km3astro/time.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-10 11:17:55.000000 km3astro-0.8.4/km3astro/wip/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-02-09 11:36:49.000000 km3astro-0.8.4/km3astro/wip/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1019 2021-02-09 11:36:49.000000 km3astro-0.8.4/km3astro/wip/below_horiz_orca.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-10 11:17:55.000000 km3astro-0.8.4/km3astro.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1466 2021-02-10 11:17:54.000000 km3astro-0.8.4/km3astro.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1184 2021-02-10 11:17:54.000000 km3astro-0.8.4/km3astro.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-02-10 11:17:54.000000 km3astro-0.8.4/km3astro.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      440 2021-02-10 11:17:54.000000 km3astro-0.8.4/km3astro.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2021-02-10 11:17:54.000000 km3astro-0.8.4/km3astro.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)      465 2021-02-09 11:36:49.000000 km3astro-0.8.4/release.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-10 11:17:55.000000 km3astro-0.8.4/requirements/
--rw-rw-rw-   0 root         (0) root         (0)      329 2021-02-09 11:36:49.000000 km3astro-0.8.4/requirements/dev.txt
--rw-rw-rw-   0 root         (0) root         (0)        7 2021-02-09 11:36:49.000000 km3astro-0.8.4/requirements/extras.txt
--rw-rw-rw-   0 root         (0) root         (0)       87 2021-02-09 11:36:49.000000 km3astro-0.8.4/requirements/install.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-10 11:17:55.000000 km3astro-0.8.4/scripts/
--rwxrwxrwx   0 root         (0) root         (0)    18545 2021-02-09 11:36:49.000000 km3astro-0.8.4/scripts/run_tests.py
--rw-rw-rw-   0 root         (0) root         (0)      102 2021-02-10 11:17:55.000000 km3astro-0.8.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1484 2021-02-09 11:36:49.000000 km3astro-0.8.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-10 11:17:55.000000 km3astro-0.8.4/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-02-09 11:36:49.000000 km3astro-0.8.4/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1089 2021-02-09 11:36:49.000000 km3astro-0.8.4/tests/test_constants.py
--rw-rw-rw-   0 root         (0) root         (0)     4946 2021-02-09 11:36:49.000000 km3astro-0.8.4/tests/test_coord.py
--rw-rw-rw-   0 root         (0) root         (0)      907 2021-02-09 11:36:49.000000 km3astro-0.8.4/tests/test_random.py
--rw-rw-rw-   0 root         (0) root         (0)      662 2021-02-09 11:36:49.000000 km3astro-0.8.4/tests/test_time.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-02 15:06:16.000000 km3astro-0.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)      270 2022-04-26 12:24:14.000000 km3astro-0.9.0/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)      837 2022-04-26 12:24:14.000000 km3astro-0.9.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     3804 2022-04-28 13:44:27.000000 km3astro-0.9.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      569 2022-04-26 12:24:14.000000 km3astro-0.9.0/.rtd-environment.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1279 2022-05-02 14:53:54.000000 km3astro-0.9.0/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6678 2022-04-26 12:24:14.000000 km3astro-0.9.0/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1513 2022-04-26 12:24:14.000000 km3astro-0.9.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      188 2022-04-26 12:24:14.000000 km3astro-0.9.0/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      912 2022-04-26 12:45:03.000000 km3astro-0.9.0/Makefile
+-rw-r--r--   0 root         (0) root         (0)     1757 2022-05-02 15:06:16.000000 km3astro-0.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1015 2022-04-26 12:24:14.000000 km3astro-0.9.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-02 15:06:16.000000 km3astro-0.9.0/doc/
+-rw-rw-rw-   0 root         (0) root         (0)     7693 2022-04-26 12:24:14.000000 km3astro-0.9.0/doc/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-02 15:06:16.000000 km3astro-0.9.0/doc/_static/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-26 12:24:14.000000 km3astro-0.9.0/doc/_static/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)    24268 2022-04-26 12:24:14.000000 km3astro-0.9.0/doc/_static/default_gallery_thumbnail.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-02 15:06:16.000000 km3astro-0.9.0/doc/_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      767 2022-04-26 12:24:14.000000 km3astro-0.9.0/doc/_templates/module.rst
+-rw-rw-rw-   0 root         (0) root         (0)       51 2022-04-26 12:24:14.000000 km3astro-0.9.0/doc/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3091 2022-04-26 12:24:14.000000 km3astro-0.9.0/doc/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      257 2022-04-26 12:24:14.000000 km3astro-0.9.0/doc/contribute.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1788 2022-04-26 12:24:14.000000 km3astro-0.9.0/doc/coordinates.rst
+-rw-rw-rw-   0 root         (0) root         (0)       33 2022-04-26 12:24:14.000000 km3astro-0.9.0/doc/dev.rst
+-rw-rw-rw-   0 root         (0) root         (0)      534 2022-04-26 12:24:14.000000 km3astro-0.9.0/doc/doc.rst
+-rw-rw-rw-   0 root         (0) root         (0)       70 2022-04-26 12:24:14.000000 km3astro-0.9.0/doc/examples.rst
+-rw-rw-rw-   0 root         (0) root         (0)      366 2022-04-26 12:24:14.000000 km3astro-0.9.0/doc/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-02 15:06:16.000000 km3astro-0.9.0/doc/modules/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-02 15:06:16.000000 km3astro-0.9.0/doc/modules/generated/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-26 12:24:14.000000 km3astro-0.9.0/doc/modules/generated/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-02 15:06:16.000000 km3astro-0.9.0/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-26 12:24:14.000000 km3astro-0.9.0/examples/README.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2660 2022-04-26 12:24:14.000000 km3astro-0.9.0/examples/plot_benchmarks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2947 2022-04-29 15:45:51.000000 km3astro-0.9.0/examples/plot_local_to_equatorial.py
+-rw-rw-rw-   0 root         (0) root         (0)     1425 2022-04-26 12:24:14.000000 km3astro-0.9.0/examples/plot_source_separation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1682 2022-04-26 12:24:14.000000 km3astro-0.9.0/examples/plot_sun_in_local.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-02 15:06:16.000000 km3astro-0.9.0/km3astro/
+-rw-rw-rw-   0 root         (0) root         (0)      181 2022-04-26 12:24:14.000000 km3astro-0.9.0/km3astro/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      548 2022-04-26 12:24:14.000000 km3astro-0.9.0/km3astro/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1442 2022-04-26 12:24:14.000000 km3astro-0.9.0/km3astro/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    14847 2022-04-29 15:25:17.000000 km3astro-0.9.0/km3astro/coord.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-02 15:06:16.000000 km3astro-0.9.0/km3astro/data/
+-rw-rw-rw-   0 root         (0) root         (0)    18624 2022-04-26 12:24:14.000000 km3astro-0.9.0/km3astro/data/orca_sun_isup.h5
+-rw-rw-rw-   0 root         (0) root         (0)      359 2022-04-26 12:24:14.000000 km3astro-0.9.0/km3astro/extras.py
+-rw-rw-rw-   0 root         (0) root         (0)     7782 2022-04-28 10:59:33.000000 km3astro-0.9.0/km3astro/frame.py
+-rw-rw-rw-   0 root         (0) root         (0)      976 2022-04-26 12:24:14.000000 km3astro-0.9.0/km3astro/plot.py
+-rw-rw-rw-   0 root         (0) root         (0)     1960 2022-04-26 12:24:14.000000 km3astro-0.9.0/km3astro/random.py
+-rw-rw-rw-   0 root         (0) root         (0)      756 2022-04-26 12:24:14.000000 km3astro-0.9.0/km3astro/sources.py
+-rw-rw-rw-   0 root         (0) root         (0)     9485 2022-05-02 09:49:49.000000 km3astro-0.9.0/km3astro/testing_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)      603 2022-04-26 12:24:14.000000 km3astro-0.9.0/km3astro/time.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-02 15:06:16.000000 km3astro-0.9.0/km3astro/wip/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-26 12:24:14.000000 km3astro-0.9.0/km3astro/wip/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1019 2022-04-26 12:24:14.000000 km3astro-0.9.0/km3astro/wip/below_horiz_orca.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-02 15:06:16.000000 km3astro-0.9.0/km3astro.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1757 2022-05-02 15:06:15.000000 km3astro-0.9.0/km3astro.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1253 2022-05-02 15:06:15.000000 km3astro-0.9.0/km3astro.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-05-02 15:06:15.000000 km3astro-0.9.0/km3astro.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      440 2022-05-02 15:06:15.000000 km3astro-0.9.0/km3astro.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2022-05-02 15:06:15.000000 km3astro-0.9.0/km3astro.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)      465 2022-04-26 12:24:14.000000 km3astro-0.9.0/release.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-02 15:06:16.000000 km3astro-0.9.0/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)      329 2022-04-26 12:24:14.000000 km3astro-0.9.0/requirements/dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)        7 2022-04-26 12:24:14.000000 km3astro-0.9.0/requirements/extras.txt
+-rw-rw-rw-   0 root         (0) root         (0)       87 2022-04-26 12:24:14.000000 km3astro-0.9.0/requirements/install.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-02 15:06:16.000000 km3astro-0.9.0/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)    18545 2022-04-26 12:24:14.000000 km3astro-0.9.0/scripts/run_tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      102 2022-05-02 15:06:16.000000 km3astro-0.9.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1484 2022-04-26 12:24:14.000000 km3astro-0.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-02 15:06:16.000000 km3astro-0.9.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-26 12:24:14.000000 km3astro-0.9.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1596 2022-05-02 09:49:49.000000 km3astro-0.9.0/tests/test_benchmarks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2022-04-26 12:24:14.000000 km3astro-0.9.0/tests/test_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     4949 2022-05-02 09:49:49.000000 km3astro-0.9.0/tests/test_coord.py
+-rw-rw-rw-   0 root         (0) root         (0)      907 2022-04-26 12:24:14.000000 km3astro-0.9.0/tests/test_random.py
+-rw-rw-rw-   0 root         (0) root         (0)      662 2022-04-26 12:24:14.000000 km3astro-0.9.0/tests/test_time.py
```

### Comparing `km3astro-0.8.4/.gitignore` & `km3astro-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `km3astro-0.8.4/.gitlab-ci.yml` & `km3astro-0.9.0/.gitlab-ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,22 @@
     image: docker.km3net.de/base/python:3.8
     stage: test
     script:
         - *virtualenv_definition
         - make test
     <<: *junit_definition
 
+test-py3.9:
+    image: docker.km3net.de/base/python:3.9
+    stage: test
+    script:
+        - *virtualenv_definition
+        - make test
+    <<: *junit_definition
+
 benchmarks:
     image: docker.km3net.de/base/python:3.7
     stage: test
     script:
         - *virtualenv_definition
         - make benchmark
     <<: *junit_definition
```

### Comparing `km3astro-0.8.4/.rtd-environment.yml` & `km3astro-0.9.0/.rtd-environment.yml`

 * *Files identical despite different names*

### Comparing `km3astro-0.8.4/CHANGELOG.rst` & `km3astro-0.9.0/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 Unreleased Changes
 ------------------
 
 Version 0
 ---------
 
+0.9.0 / 2022-05-02
+~~~~~~~~~~~~~~~~~~
+* Refactoring
+* Coordinate transformation is now fully based on astropy.SkyCoord with
+  a new frame designed for KM3NeT
+* Bugfixes
+
 0.8.4 / 2020-01-23
 ~~~~~~~~~~~~~~~~~~
 * Cleanup and remove unnecessary requirements (scipy, km3pipe, ...)
 * Bug fixes
 * Preparation for API clean-up
 
 0.8.3
```

### Comparing `km3astro-0.8.4/CONTRIBUTING.rst` & `km3astro-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `km3astro-0.8.4/LICENSE` & `km3astro-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `km3astro-0.8.4/Makefile` & `km3astro-0.9.0/Makefile`

 * *Files identical despite different names*

### Comparing `km3astro-0.8.4/PKG-INFO` & `km3astro-0.9.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,48 @@
 Metadata-Version: 2.1
 Name: km3astro
-Version: 0.8.4
+Version: 0.9.0
 Summary: Astronomical utilities for KM3NeT
 Home-page: http://git.km3net.de/km3py/km3astro
 Author: Tamas Gal and Moritz Lotze
 Author-email: tgal@km3net.de
 License: UNKNOWN
 Description: km3astro
         ========
         
         .. image:: https://git.km3net.de/km3py/km3astro/badges/master/pipeline.svg
             :target: https://git.km3net.de/km3py/km3astro/pipelines
         
         .. image:: https://git.km3net.de/km3py/km3astro/badges/master/coverage.svg
             :target: https://km3py.pages.km3net.de/km3astro/coverage
         
-        .. image:: https://examples.pages.km3net.de/km3badges/docs-latest-brightgreen.svg
+        .. image:: https://git.km3net.de/examples/km3badges/-/raw/master/docs-latest-brightgreen.svg
             :target: https://km3py.pages.km3net.de/km3astro
         
         About
         -----
         
         KM3Astro is a collection astronomy utils, like coordinate transformations.
         
         Install
         -------
         
         This is developed on python >=3.5. Lower versions (especially py2)
         might or might not work. Use ``pip`` to install the latest
         version::
         
+          pip install km3astro
+        
+        
+        Install the latest development version
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        To get the latest and greatest stable development version, use ``pip``
+        and the URL to the repository::
+        
           pip install git+http://git.km3net.de/km3py/km3astro.git
         
         or just clone the git repository and install via ``pip install .``
         
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `km3astro-0.8.4/doc/Makefile` & `km3astro-0.9.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `km3astro-0.8.4/doc/_static/default_gallery_thumbnail.png` & `km3astro-0.9.0/doc/_static/default_gallery_thumbnail.png`

 * *Files identical despite different names*

### Comparing `km3astro-0.8.4/doc/_templates/module.rst` & `km3astro-0.9.0/doc/_templates/module.rst`

 * *Files identical despite different names*

### Comparing `km3astro-0.8.4/doc/conf.py` & `km3astro-0.9.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `km3astro-0.8.4/doc/coordinates.rst` & `km3astro-0.9.0/doc/coordinates.rst`

 * *Files identical despite different names*

### Comparing `km3astro-0.8.4/doc/doc.rst` & `km3astro-0.9.0/doc/doc.rst`

 * *Files identical despite different names*

### Comparing `km3astro-0.8.4/examples/plot_benchmarks.py` & `km3astro-0.9.0/examples/plot_benchmarks.py`

 * *Files identical despite different names*

### Comparing `km3astro-0.8.4/examples/plot_local_to_equatorial.py` & `km3astro-0.9.0/examples/plot_local_to_equatorial.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 
 __author__ = "moritz"
 
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 
-from km3astro.coord import local_event, get_location, neutrino_to_source_direction
+from km3astro.coord import local_event, neutrino_to_source_direction
+from km3astro.frame import get_location
 from km3astro.plot import plot_equatorial
 from km3astro.sources import VELA_X
 
 
 ##########################################################
 # Detector Coordinates
 # --------------------
```

### Comparing `km3astro-0.8.4/examples/plot_source_separation.py` & `km3astro-0.9.0/examples/plot_source_separation.py`

 * *Files identical despite different names*

### Comparing `km3astro-0.8.4/examples/plot_sun_in_local.py` & `km3astro-0.9.0/examples/plot_sun_in_local.py`

 * *Files identical despite different names*

### Comparing `km3astro-0.8.4/km3astro/__version__.py` & `km3astro-0.9.0/km3astro/__version__.py`

 * *Files identical despite different names*

### Comparing `km3astro-0.8.4/km3astro/constants.py` & `km3astro-0.9.0/km3astro/constants.py`

 * *Files identical despite different names*

### Comparing `km3astro-0.8.4/km3astro/data/orca_sun_isup.h5` & `km3astro-0.9.0/km3astro/data/orca_sun_isup.h5`

 * *Files identical despite different names*

### Comparing `km3astro-0.8.4/km3astro/plot.py` & `km3astro-0.9.0/km3astro/plot.py`

 * *Files identical despite different names*

### Comparing `km3astro-0.8.4/km3astro/random.py` & `km3astro-0.9.0/km3astro/random.py`

 * *Files identical despite different names*

### Comparing `km3astro-0.8.4/km3astro/sources.py` & `km3astro-0.9.0/km3astro/sources.py`

 * *Files identical despite different names*

### Comparing `km3astro-0.8.4/km3astro/time.py` & `km3astro-0.9.0/km3astro/time.py`

 * *Files identical despite different names*

### Comparing `km3astro-0.8.4/km3astro/wip/below_horiz_orca.py` & `km3astro-0.9.0/km3astro/wip/below_horiz_orca.py`

 * *Files identical despite different names*

### Comparing `km3astro-0.8.4/km3astro.egg-info/PKG-INFO` & `km3astro-0.9.0/km3astro.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,48 @@
 Metadata-Version: 2.1
 Name: km3astro
-Version: 0.8.4
+Version: 0.9.0
 Summary: Astronomical utilities for KM3NeT
 Home-page: http://git.km3net.de/km3py/km3astro
 Author: Tamas Gal and Moritz Lotze
 Author-email: tgal@km3net.de
 License: UNKNOWN
 Description: km3astro
         ========
         
         .. image:: https://git.km3net.de/km3py/km3astro/badges/master/pipeline.svg
             :target: https://git.km3net.de/km3py/km3astro/pipelines
         
         .. image:: https://git.km3net.de/km3py/km3astro/badges/master/coverage.svg
             :target: https://km3py.pages.km3net.de/km3astro/coverage
         
-        .. image:: https://examples.pages.km3net.de/km3badges/docs-latest-brightgreen.svg
+        .. image:: https://git.km3net.de/examples/km3badges/-/raw/master/docs-latest-brightgreen.svg
             :target: https://km3py.pages.km3net.de/km3astro
         
         About
         -----
         
         KM3Astro is a collection astronomy utils, like coordinate transformations.
         
         Install
         -------
         
         This is developed on python >=3.5. Lower versions (especially py2)
         might or might not work. Use ``pip`` to install the latest
         version::
         
+          pip install km3astro
+        
+        
+        Install the latest development version
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        To get the latest and greatest stable development version, use ``pip``
+        and the URL to the repository::
+        
           pip install git+http://git.km3net.de/km3py/km3astro.git
         
         or just clone the git repository and install via ``pip install .``
         
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `km3astro-0.8.4/km3astro.egg-info/SOURCES.txt` & `km3astro-0.9.0/km3astro.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -30,28 +30,31 @@
 examples/plot_source_separation.py
 examples/plot_sun_in_local.py
 km3astro/__init__.py
 km3astro/__version__.py
 km3astro/constants.py
 km3astro/coord.py
 km3astro/extras.py
+km3astro/frame.py
 km3astro/plot.py
 km3astro/random.py
 km3astro/sources.py
+km3astro/testing_tools.py
 km3astro/time.py
 km3astro.egg-info/PKG-INFO
 km3astro.egg-info/SOURCES.txt
 km3astro.egg-info/dependency_links.txt
 km3astro.egg-info/requires.txt
 km3astro.egg-info/top_level.txt
 km3astro/data/orca_sun_isup.h5
 km3astro/wip/__init__.py
 km3astro/wip/below_horiz_orca.py
 requirements/dev.txt
 requirements/extras.txt
 requirements/install.txt
 scripts/run_tests.py
 tests/__init__.py
+tests/test_benchmarks.py
 tests/test_constants.py
 tests/test_coord.py
 tests/test_random.py
 tests/test_time.py
```

### Comparing `km3astro-0.8.4/scripts/run_tests.py` & `km3astro-0.9.0/scripts/run_tests.py`

 * *Files identical despite different names*

### Comparing `km3astro-0.8.4/setup.py` & `km3astro-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `km3astro-0.8.4/tests/test_constants.py` & `km3astro-0.9.0/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `km3astro-0.8.4/tests/test_coord.py` & `km3astro-0.9.0/tests/test_coord.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,71 +1,68 @@
 from unittest import TestCase
 
 import numpy as np
+import pandas as pd
+
 from numpy.testing import assert_allclose
 from astropy.coordinates import SkyCoord
 from astropy import units as u
 from astropy.time import Time
 from astropy.io import ascii
 from km3net_testdata import data_path
 
-from km3astro.coord import (
-    local_event,
-    neutrino_to_source_direction,
-    sun_local,
-    convergence_angle,
-    utm_zone,
-    longitude_of_central_meridian,
-)
+import km3astro.coord as kc
+import km3astro.frame as kf
+
 from km3astro.random import random_date
 
 
 class TestCoord(TestCase):
     def setUp(self):
         self.n_evts = 100
         self.n_evts_funny = 1e2
 
     def test_neutrino_flip_degree(self):
         phi = np.array([97.07, 23.46, 97.07, 192.5, 333.33])
         theta = np.array([135.0, 11.97, 22.97, 33.97, 85.23])
         azi_exp = np.array([277.07, 203.46, 277.07, 12.5, 153.33])
         zen_exp = np.array([45.0, 168.03, 157.03, 146.03, 94.77])
-        azi, zen = neutrino_to_source_direction(phi, theta, radian=False)
+        azi, zen = kc.neutrino_to_source_direction(phi, theta, radian=False)
         assert_allclose(azi, azi_exp)
         assert_allclose(zen, zen_exp)
 
     def test_neutrino_flip_radian(self):
         phi = np.array([97.07, 23.46, 97.07, 192.5, 333.33]) * np.pi / 180
         theta = np.array([135.0, 11.97, 22.97, 33.97, 85.23]) * np.pi / 180
         azi_exp = np.array([277.07, 203.46, 277.07, 12.5, 153.33]) * np.pi / 180
         zen_exp = np.array([45.0, 168.03, 157.03, 146.03, 94.77]) * np.pi / 180
-        azi, zen = neutrino_to_source_direction(phi, theta, radian=True)
+        azi, zen = kc.neutrino_to_source_direction(phi, theta, radian=True)
 
         assert_allclose(azi, azi_exp)
         assert_allclose(zen, zen_exp)
 
 
 class TestCoordRandom(TestCase):
     def test_sun(self):
         date = random_date(n=100)
-        sun = sun_local(date, loc="orca")
+        sun = kc.sun_local(date, loc="orca")
 
 
 class TestConvergenceAngle(TestCase):
     def test_convergence_angle(self):
-        ca = convergence_angle(1.5, 1.3)
+        ca = kf.convergence_angle(1.5, 1.3)
         self.assertAlmostEqual(-0.00897440033130838, ca)
 
 
 class TestUTMStuff(TestCase):
     def test_utm_zone(self):
-        assert 38 == utm_zone(np.pi / 180 * 42.8871)
+        assert 38 == kf.utm_zone(np.pi / 180 * 42.8871)
 
     def test_longitude_of_central_meridian(self):
-        self.assertAlmostEqual(0.785398163397448, longitude_of_central_meridian(38))
+        self.assertAlmostEqual(0.785398163397448, kf.longitude_of_central_meridian(38))
 
 
 class TestAntaresBenchmark(TestCase):
     def setUp(self):
         self.tol = 0.01 * u.deg
         self.gal_tol = 0.02 * u.deg
 
@@ -77,19 +74,19 @@
         for obj in antares_objects_data:
             time = Time(" ".join([obj["date"], obj["time"]]))
 
             theta = np.deg2rad(obj["theta"])
             phi = np.deg2rad(obj["phi"])
 
             # check azimuth and zenith conversion
-            azimuth, zenith = neutrino_to_source_direction(phi, theta)
+            azimuth, zenith = kc.neutrino_to_source_direction(phi, theta)
             self.assertAlmostEqual(azimuth[0], np.deg2rad(obj["azimuth"]))
             self.assertAlmostEqual(zenith[0], np.deg2rad(obj["zenith"]))
 
-            event = local_event(phi, time, theta, location="antares")
+            event = kc.local_event(phi, time, theta, location="antares")
 
             equat = event.fk5
             dec = equat.dec
             ra = equat.ra
 
             ref = SkyCoord(
                 " ".join([obj["RA-J2000"], obj["DEC-J2000"]]),
@@ -112,25 +109,29 @@
             print(obj)
             time = Time(" ".join([obj["date"], obj["time"]]))
 
             theta = np.deg2rad(obj["theta"])
             phi = np.deg2rad(obj["phi"])
 
             # check azimuth and zenith conversion
-            azimuth, zenith = neutrino_to_source_direction(phi, theta)
+            azimuth, zenith = kc.neutrino_to_source_direction(phi, theta)
             print("azimuth: ", azimuth, np.rad2deg(azimuth))
             print("zenith: ", zenith, np.rad2deg(zenith))
             self.assertAlmostEqual(azimuth[0], np.deg2rad(obj["azimuth"]))
             self.assertAlmostEqual(zenith[0], np.deg2rad(obj["zenith"]))
 
-            event = local_event(phi, time, theta, location="antares")
+            event = kc.local_event(phi, time, theta, location="antares")
             print(event.fk5)
             print(event.galactic)
 
             # ref = SkyCoord(obj["RA-J2000"], obj["DEC-J2000"], unit=u.deg, frame="fk5")
 
             assert np.abs(obj["DEC-J2000"] * u.deg - event.fk5.dec) < self.tol
             assert np.abs(obj["RA-J2000"] * u.deg - event.fk5.ra) < self.tol
 
             print(obj["gal_lat"], event.galactic.b.deg[0])
-            assert np.abs(obj["gal_lat"] - event.galactic.b.deg[0]) * u.deg < self.gal_tol
-            assert np.abs(obj["gal_lon"] - event.galactic.l.deg[0])  * u.deg< self.gal_tol
+            assert (
+                np.abs(obj["gal_lat"] - event.galactic.b.deg[0]) * u.deg < self.gal_tol
+            )
+            assert (
+                np.abs(obj["gal_lon"] - event.galactic.l.deg[0]) * u.deg < self.gal_tol
+            )
```

### Comparing `km3astro-0.8.4/tests/test_random.py` & `km3astro-0.9.0/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `km3astro-0.8.4/tests/test_time.py` & `km3astro-0.9.0/tests/test_time.py`

 * *Files identical despite different names*

