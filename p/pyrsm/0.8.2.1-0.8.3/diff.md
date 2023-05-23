# Comparing `tmp/pyrsm-0.8.2.1.tar.gz` & `tmp/pyrsm-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrsm-0.8.2.1.tar", last modified: Thu May 18 20:07:17 2023, max compression
+gzip compressed data, was "pyrsm-0.8.3.tar", last modified: Tue May 23 07:26:20 2023, max compression
```

## Comparing `pyrsm-0.8.2.1.tar` & `pyrsm-0.8.3.tar`

### file list

```diff
@@ -1,82 +1,84 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-18 20:07:17.398175 pyrsm-0.8.2.1/
--rw-r--r--   0 root         (0) staff       (20)    34523 2022-03-19 20:23:12.000000 pyrsm-0.8.2.1/LICENSE
--rw-r--r--   0 root         (0) staff       (20)      243 2023-05-16 06:57:58.000000 pyrsm-0.8.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) staff       (20)      594 2023-05-18 20:07:17.398282 pyrsm-0.8.2.1/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     2625 2023-05-16 19:42:31.000000 pyrsm-0.8.2.1/README.md
--rw-r--r--   0 root         (0) staff       (20)       80 2022-02-19 01:02:39.000000 pyrsm-0.8.2.1/pyproject.toml
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-18 20:07:17.384165 pyrsm-0.8.2.1/pyrsm/
--rw-r--r--   0 root         (0) staff       (20)      314 2023-05-18 20:01:35.000000 pyrsm-0.8.2.1/pyrsm/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    54279 2023-05-15 06:31:28.000000 pyrsm-0.8.2.1/pyrsm/basics.py
--rw-r--r--   0 root         (0) staff       (20)     2843 2023-01-31 17:36:18.000000 pyrsm-0.8.2.1/pyrsm/bins.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-18 20:07:17.384940 pyrsm-0.8.2.1/pyrsm/data/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.2.1/pyrsm/data/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-18 20:07:17.386125 pyrsm-0.8.2.1/pyrsm/data/basics/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.2.1/pyrsm/data/basics/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     6996 2022-02-13 01:24:09.000000 pyrsm-0.8.2.1/pyrsm/data/basics/consider.pkl
--rw-r--r--   0 root         (0) staff       (20)    13754 2022-02-13 01:24:09.000000 pyrsm-0.8.2.1/pyrsm/data/basics/demand_uk.pkl
--rw-r--r--   0 root         (0) staff       (20)     5508 2022-02-13 01:24:09.000000 pyrsm-0.8.2.1/pyrsm/data/basics/newspaper.pkl
--rw-r--r--   0 root         (0) staff       (20)     8545 2022-02-13 01:24:09.000000 pyrsm-0.8.2.1/pyrsm/data/basics/salary.pkl
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-18 20:07:17.387641 pyrsm-0.8.2.1/pyrsm/data/data/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.2.1/pyrsm/data/data/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1620 2022-02-13 01:24:09.000000 pyrsm-0.8.2.1/pyrsm/data/data/avengers.pkl
--rw-r--r--   0 root         (0) staff       (20)   207435 2022-02-13 01:24:09.000000 pyrsm-0.8.2.1/pyrsm/data/data/diamonds.pkl
--rw-r--r--   0 root         (0) staff       (20)     1557 2022-02-13 01:24:09.000000 pyrsm-0.8.2.1/pyrsm/data/data/publishers.pkl
--rw-r--r--   0 root         (0) staff       (20)     1660 2022-02-13 01:24:09.000000 pyrsm-0.8.2.1/pyrsm/data/data/superheroes.pkl
--rw-r--r--   0 root         (0) staff       (20)    69129 2022-02-13 01:24:09.000000 pyrsm-0.8.2.1/pyrsm/data/data/titanic.pkl
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-18 20:07:17.388153 pyrsm-0.8.2.1/pyrsm/data/design/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.2.1/pyrsm/data/design/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     3414 2022-02-13 01:24:09.000000 pyrsm-0.8.2.1/pyrsm/data/design/rndnames.pkl
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-18 20:07:17.391615 pyrsm-0.8.2.1/pyrsm/data/model/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.2.1/pyrsm/data/model/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     8197 2022-02-13 01:24:09.000000 pyrsm-0.8.2.1/pyrsm/data/model/catalog.pkl
--rw-r--r--   0 root         (0) staff       (20)    41039 2022-02-13 01:24:09.000000 pyrsm-0.8.2.1/pyrsm/data/model/direct_marketing.pkl
--rw-r--r--   0 root         (0) staff       (20)   342723 2022-02-13 01:24:09.000000 pyrsm-0.8.2.1/pyrsm/data/model/dvd.pkl
--rw-r--r--   0 root         (0) staff       (20)     4468 2022-02-13 01:24:09.000000 pyrsm-0.8.2.1/pyrsm/data/model/houseprices.pkl
--rw-r--r--   0 root         (0) staff       (20)    33206 2022-02-13 01:24:09.000000 pyrsm-0.8.2.1/pyrsm/data/model/ideal.pkl
--rw-r--r--   0 root         (0) staff       (20)   126402 2022-02-13 01:24:09.000000 pyrsm-0.8.2.1/pyrsm/data/model/ketchup.pkl
--rw-r--r--   0 root         (0) staff       (20)      315 2022-02-13 01:24:09.000000 pyrsm-0.8.2.1/pyrsm/data/model/movie_contract.pkl
--rw-r--r--   0 root         (0) staff       (20)     3123 2022-02-13 01:24:09.000000 pyrsm-0.8.2.1/pyrsm/data/model/ratings.pkl
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-18 20:07:17.393530 pyrsm-0.8.2.1/pyrsm/data/multivariate/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.2.1/pyrsm/data/multivariate/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     3125 2022-02-13 01:24:09.000000 pyrsm-0.8.2.1/pyrsm/data/multivariate/carpet.pkl
--rw-r--r--   0 root         (0) staff       (20)     2423 2022-02-13 01:24:09.000000 pyrsm-0.8.2.1/pyrsm/data/multivariate/city.pkl
--rw-r--r--   0 root         (0) staff       (20)     3923 2022-02-13 01:24:09.000000 pyrsm-0.8.2.1/pyrsm/data/multivariate/city2.pkl
--rw-r--r--   0 root         (0) staff       (20)     2625 2022-02-13 01:24:09.000000 pyrsm-0.8.2.1/pyrsm/data/multivariate/computer.pkl
--rw-r--r--   0 root         (0) staff       (20)     3442 2022-02-13 01:24:09.000000 pyrsm-0.8.2.1/pyrsm/data/multivariate/movie.pkl
--rw-r--r--   0 root         (0) staff       (20)     2994 2022-02-13 01:24:09.000000 pyrsm-0.8.2.1/pyrsm/data/multivariate/mp3.pkl
--rw-r--r--   0 root         (0) staff       (20)     3278 2022-02-13 01:24:09.000000 pyrsm-0.8.2.1/pyrsm/data/multivariate/retailers.pkl
--rw-r--r--   0 root         (0) staff       (20)     2357 2022-02-13 01:24:09.000000 pyrsm-0.8.2.1/pyrsm/data/multivariate/shopping.pkl
--rw-r--r--   0 root         (0) staff       (20)     4872 2022-02-13 01:24:09.000000 pyrsm-0.8.2.1/pyrsm/data/multivariate/toothpaste.pkl
--rw-r--r--   0 root         (0) staff       (20)     3678 2022-02-13 01:24:09.000000 pyrsm-0.8.2.1/pyrsm/data/multivariate/tpbrands.pkl
--rw-r--r--   0 root         (0) staff       (20)     1966 2023-01-26 08:23:23.000000 pyrsm-0.8.2.1/pyrsm/example_data.py
--rw-r--r--   0 root         (0) staff       (20)     5271 2023-05-07 05:21:24.000000 pyrsm-0.8.2.1/pyrsm/logit.py
--rw-r--r--   0 root         (0) staff       (20)    25101 2023-05-15 06:38:12.000000 pyrsm-0.8.2.1/pyrsm/model.py
--rw-r--r--   0 root         (0) staff       (20)     2214 2023-05-15 20:48:14.000000 pyrsm-0.8.2.1/pyrsm/notebook.py
--rw-r--r--   0 root         (0) staff       (20)    37519 2023-04-16 05:51:16.000000 pyrsm-0.8.2.1/pyrsm/perf.py
--rw-r--r--   0 root         (0) staff       (20)     1835 2022-02-13 01:24:09.000000 pyrsm-0.8.2.1/pyrsm/props.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-18 20:07:17.394852 pyrsm-0.8.2.1/pyrsm/radiant/
--rw-r--r--   0 root         (0) staff       (20)       23 2023-05-18 03:04:58.000000 pyrsm-0.8.2.1/pyrsm/radiant/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     9489 2023-05-15 05:18:12.000000 pyrsm-0.8.2.1/pyrsm/radiant/logit.py
--rw-r--r--   0 root         (0) staff       (20)    11114 2023-05-18 17:30:15.000000 pyrsm-0.8.2.1/pyrsm/radiant/regress.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-18 20:07:17.395666 pyrsm-0.8.2.1/pyrsm/radiant/www/
--rw-r--r--   0 root         (0) staff       (20)      230 2023-05-11 03:12:37.000000 pyrsm-0.8.2.1/pyrsm/radiant/www/copy.js
--rw-r--r--   0 root         (0) staff       (20)     3597 2023-05-11 03:12:22.000000 pyrsm-0.8.2.1/pyrsm/radiant/www/style.css
--rw-r--r--   0 root         (0) staff       (20)     7156 2023-05-18 03:08:18.000000 pyrsm-0.8.2.1/pyrsm/regress.py
--rw-r--r--   0 root         (0) staff       (20)     5411 2023-03-27 22:17:11.000000 pyrsm-0.8.2.1/pyrsm/stats.py
--rw-r--r--   0 root         (0) staff       (20)    10313 2023-05-14 21:06:56.000000 pyrsm-0.8.2.1/pyrsm/utils.py
--rw-r--r--   0 root         (0) staff       (20)    22540 2023-05-15 06:30:36.000000 pyrsm-0.8.2.1/pyrsm/visualize.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-18 20:07:17.384828 pyrsm-0.8.2.1/pyrsm.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      594 2023-05-18 20:07:17.000000 pyrsm-0.8.2.1/pyrsm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     1772 2023-05-18 20:07:17.000000 pyrsm-0.8.2.1/pyrsm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-05-18 20:07:17.000000 pyrsm-0.8.2.1/pyrsm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)      205 2023-05-18 20:07:17.000000 pyrsm-0.8.2.1/pyrsm.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)        6 2023-05-18 20:07:17.000000 pyrsm-0.8.2.1/pyrsm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)     1016 2023-05-18 20:07:17.398656 pyrsm-0.8.2.1/setup.cfg
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-18 20:07:17.397932 pyrsm-0.8.2.1/tests/
--rw-r--r--   0 root         (0) staff       (20)      722 2023-05-16 05:24:37.000000 pyrsm-0.8.2.1/tests/test_basics.py
--rw-r--r--   0 root         (0) staff       (20)     1072 2023-03-05 06:28:28.000000 pyrsm-0.8.2.1/tests/test_bins.py
--rw-r--r--   0 root         (0) staff       (20)      794 2023-05-16 05:39:55.000000 pyrsm-0.8.2.1/tests/test_example_data.py
--rw-r--r--   0 root         (0) staff       (20)     2756 2023-01-21 01:15:24.000000 pyrsm-0.8.2.1/tests/test_perf.py
--rw-r--r--   0 root         (0) staff       (20)      615 2023-05-16 05:41:07.000000 pyrsm-0.8.2.1/tests/test_regression.py
--rw-r--r--   0 root         (0) staff       (20)     2036 2023-03-05 06:38:03.000000 pyrsm-0.8.2.1/tests/test_stats.py
--rw-r--r--   0 root         (0) staff       (20)     1979 2022-02-13 01:24:09.000000 pyrsm-0.8.2.1/tests/test_utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-23 07:26:20.193928 pyrsm-0.8.3/
+-rw-r--r--   0 root         (0) staff       (20)    34523 2022-03-19 20:23:12.000000 pyrsm-0.8.3/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)      243 2023-05-16 06:57:58.000000 pyrsm-0.8.3/MANIFEST.in
+-rw-r--r--   0 root         (0) staff       (20)      592 2023-05-23 07:26:20.194016 pyrsm-0.8.3/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     2625 2023-05-16 19:42:31.000000 pyrsm-0.8.3/README.md
+-rw-r--r--   0 root         (0) staff       (20)       80 2022-02-19 01:02:39.000000 pyrsm-0.8.3/pyproject.toml
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-23 07:26:20.180406 pyrsm-0.8.3/pyrsm/
+-rw-r--r--   0 root         (0) staff       (20)      312 2023-05-23 07:25:55.000000 pyrsm-0.8.3/pyrsm/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)    54279 2023-05-15 06:31:28.000000 pyrsm-0.8.3/pyrsm/basics.py
+-rw-r--r--   0 root         (0) staff       (20)     2843 2023-01-31 17:36:18.000000 pyrsm-0.8.3/pyrsm/bins.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-23 07:26:20.181347 pyrsm-0.8.3/pyrsm/data/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-23 07:26:20.182220 pyrsm-0.8.3/pyrsm/data/basics/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/basics/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     6996 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/basics/consider.pkl
+-rw-r--r--   0 root         (0) staff       (20)    13754 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/basics/demand_uk.pkl
+-rw-r--r--   0 root         (0) staff       (20)     5508 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/basics/newspaper.pkl
+-rw-r--r--   0 root         (0) staff       (20)     8545 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/basics/salary.pkl
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-23 07:26:20.183857 pyrsm-0.8.3/pyrsm/data/data/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/data/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1620 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/data/avengers.pkl
+-rw-r--r--   0 root         (0) staff       (20)   207435 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/data/diamonds.pkl
+-rw-r--r--   0 root         (0) staff       (20)     1557 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/data/publishers.pkl
+-rw-r--r--   0 root         (0) staff       (20)     1660 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/data/superheroes.pkl
+-rw-r--r--   0 root         (0) staff       (20)    69129 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/data/titanic.pkl
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-23 07:26:20.184304 pyrsm-0.8.3/pyrsm/data/design/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/design/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3414 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/design/rndnames.pkl
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-23 07:26:20.187716 pyrsm-0.8.3/pyrsm/data/model/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/model/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     8197 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/model/catalog.pkl
+-rw-r--r--   0 root         (0) staff       (20)    41039 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/model/direct_marketing.pkl
+-rw-r--r--   0 root         (0) staff       (20)   342723 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/model/dvd.pkl
+-rw-r--r--   0 root         (0) staff       (20)     4468 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/model/houseprices.pkl
+-rw-r--r--   0 root         (0) staff       (20)    33206 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/model/ideal.pkl
+-rw-r--r--   0 root         (0) staff       (20)   126402 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/model/ketchup.pkl
+-rw-r--r--   0 root         (0) staff       (20)      315 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/model/movie_contract.pkl
+-rw-r--r--   0 root         (0) staff       (20)     3123 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/model/ratings.pkl
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-23 07:26:20.189531 pyrsm-0.8.3/pyrsm/data/multivariate/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/multivariate/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3125 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/multivariate/carpet.pkl
+-rw-r--r--   0 root         (0) staff       (20)     2423 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/multivariate/city.pkl
+-rw-r--r--   0 root         (0) staff       (20)     3923 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/multivariate/city2.pkl
+-rw-r--r--   0 root         (0) staff       (20)     2625 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/multivariate/computer.pkl
+-rw-r--r--   0 root         (0) staff       (20)     3442 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/multivariate/movie.pkl
+-rw-r--r--   0 root         (0) staff       (20)     2994 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/multivariate/mp3.pkl
+-rw-r--r--   0 root         (0) staff       (20)     3278 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/multivariate/retailers.pkl
+-rw-r--r--   0 root         (0) staff       (20)     2357 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/multivariate/shopping.pkl
+-rw-r--r--   0 root         (0) staff       (20)     4872 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/multivariate/toothpaste.pkl
+-rw-r--r--   0 root         (0) staff       (20)     3678 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/data/multivariate/tpbrands.pkl
+-rw-r--r--   0 root         (0) staff       (20)     1966 2023-01-26 08:23:23.000000 pyrsm-0.8.3/pyrsm/example_data.py
+-rw-r--r--   0 root         (0) staff       (20)     5271 2023-05-07 05:21:24.000000 pyrsm-0.8.3/pyrsm/logit.py
+-rw-r--r--   0 root         (0) staff       (20)    25270 2023-05-21 21:48:34.000000 pyrsm-0.8.3/pyrsm/model.py
+-rw-r--r--   0 root         (0) staff       (20)     2214 2023-05-15 20:48:14.000000 pyrsm-0.8.3/pyrsm/notebook.py
+-rw-r--r--   0 root         (0) staff       (20)    37519 2023-04-16 05:51:16.000000 pyrsm-0.8.3/pyrsm/perf.py
+-rw-r--r--   0 root         (0) staff       (20)     1835 2022-02-13 01:24:09.000000 pyrsm-0.8.3/pyrsm/props.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-23 07:26:20.190646 pyrsm-0.8.3/pyrsm/radiant/
+-rw-r--r--   0 root         (0) staff       (20)       23 2023-05-18 03:04:58.000000 pyrsm-0.8.3/pyrsm/radiant/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     9489 2023-05-15 05:18:12.000000 pyrsm-0.8.3/pyrsm/radiant/logit.py
+-rw-r--r--   0 root         (0) staff       (20)    19960 2023-05-23 03:13:46.000000 pyrsm-0.8.3/pyrsm/radiant/regress.py
+-rw-r--r--   0 root         (0) staff       (20)     1200 2023-05-23 03:10:54.000000 pyrsm-0.8.3/pyrsm/radiant/utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-23 07:26:20.191551 pyrsm-0.8.3/pyrsm/radiant/www/
+-rw-r--r--   0 root         (0) staff       (20)      230 2023-05-11 03:12:37.000000 pyrsm-0.8.3/pyrsm/radiant/www/copy.js
+-rw-r--r--   0 root         (0) staff       (20)     1964 2023-05-23 02:45:36.000000 pyrsm-0.8.3/pyrsm/radiant/www/returnTextAreaBinding.js
+-rw-r--r--   0 root         (0) staff       (20)     3597 2023-05-11 03:12:22.000000 pyrsm-0.8.3/pyrsm/radiant/www/style.css
+-rw-r--r--   0 root         (0) staff       (20)     7564 2023-05-23 03:00:47.000000 pyrsm-0.8.3/pyrsm/regress.py
+-rw-r--r--   0 root         (0) staff       (20)     5411 2023-03-27 22:17:11.000000 pyrsm-0.8.3/pyrsm/stats.py
+-rw-r--r--   0 root         (0) staff       (20)    10313 2023-05-14 21:06:56.000000 pyrsm-0.8.3/pyrsm/utils.py
+-rw-r--r--   0 root         (0) staff       (20)    22603 2023-05-22 00:34:13.000000 pyrsm-0.8.3/pyrsm/visualize.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-23 07:26:20.181227 pyrsm-0.8.3/pyrsm.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      592 2023-05-23 07:26:20.000000 pyrsm-0.8.3/pyrsm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     1838 2023-05-23 07:26:20.000000 pyrsm-0.8.3/pyrsm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-05-23 07:26:20.000000 pyrsm-0.8.3/pyrsm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)      193 2023-05-23 07:26:20.000000 pyrsm-0.8.3/pyrsm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)        6 2023-05-23 07:26:20.000000 pyrsm-0.8.3/pyrsm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)     1003 2023-05-23 07:26:20.194387 pyrsm-0.8.3/setup.cfg
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-23 07:26:20.193681 pyrsm-0.8.3/tests/
+-rw-r--r--   0 root         (0) staff       (20)      722 2023-05-16 05:24:37.000000 pyrsm-0.8.3/tests/test_basics.py
+-rw-r--r--   0 root         (0) staff       (20)     1072 2023-03-05 06:28:28.000000 pyrsm-0.8.3/tests/test_bins.py
+-rw-r--r--   0 root         (0) staff       (20)      794 2023-05-16 05:39:55.000000 pyrsm-0.8.3/tests/test_example_data.py
+-rw-r--r--   0 root         (0) staff       (20)     2756 2023-01-21 01:15:24.000000 pyrsm-0.8.3/tests/test_perf.py
+-rw-r--r--   0 root         (0) staff       (20)      615 2023-05-16 05:41:07.000000 pyrsm-0.8.3/tests/test_regression.py
+-rw-r--r--   0 root         (0) staff       (20)     2036 2023-03-05 06:38:03.000000 pyrsm-0.8.3/tests/test_stats.py
+-rw-r--r--   0 root         (0) staff       (20)     1979 2022-02-13 01:24:09.000000 pyrsm-0.8.3/tests/test_utils.py
```

### Comparing `pyrsm-0.8.2.1/LICENSE` & `pyrsm-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/PKG-INFO` & `pyrsm-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsm
-Version: 0.8.2.1
+Version: 0.8.3
 Summary: Python functions for Customer Analytics at the Rady School of Management (RSM)
 Author: Vincent Nijs <vnijs@ucsd.edu>, Vikram Jambulapati <vikjam@ucsd.edu>, Suhas Goutham <sgoutham@ucsd.edu>, Raghav Prasad <rprasad@ucsd.edu>
 Author-email: vnijs@ucsd.edu
 License: AGPL-3.0-only
 Project-URL: Bug Reports, https://github.com/vnijs/pyrsm/issues
 Project-URL: Source, https://github.com/vnijs/pyrsm
 Description-Content-Type: text/markdown
```

### Comparing `pyrsm-0.8.2.1/README.md` & `pyrsm-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/basics.py` & `pyrsm-0.8.3/pyrsm/basics.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/bins.py` & `pyrsm-0.8.3/pyrsm/bins.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/data/basics/consider.pkl` & `pyrsm-0.8.3/pyrsm/data/basics/consider.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/data/basics/demand_uk.pkl` & `pyrsm-0.8.3/pyrsm/data/basics/demand_uk.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/data/basics/newspaper.pkl` & `pyrsm-0.8.3/pyrsm/data/basics/newspaper.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/data/basics/salary.pkl` & `pyrsm-0.8.3/pyrsm/data/basics/salary.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/data/data/avengers.pkl` & `pyrsm-0.8.3/pyrsm/data/data/avengers.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/data/data/diamonds.pkl` & `pyrsm-0.8.3/pyrsm/data/data/diamonds.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/data/data/publishers.pkl` & `pyrsm-0.8.3/pyrsm/data/data/publishers.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/data/data/superheroes.pkl` & `pyrsm-0.8.3/pyrsm/data/data/superheroes.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/data/data/titanic.pkl` & `pyrsm-0.8.3/pyrsm/data/data/titanic.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/data/design/rndnames.pkl` & `pyrsm-0.8.3/pyrsm/data/design/rndnames.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/data/model/catalog.pkl` & `pyrsm-0.8.3/pyrsm/data/model/catalog.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/data/model/direct_marketing.pkl` & `pyrsm-0.8.3/pyrsm/data/model/direct_marketing.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/data/model/dvd.pkl` & `pyrsm-0.8.3/pyrsm/data/model/dvd.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/data/model/houseprices.pkl` & `pyrsm-0.8.3/pyrsm/data/model/houseprices.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/data/model/ideal.pkl` & `pyrsm-0.8.3/pyrsm/data/model/ideal.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/data/model/ketchup.pkl` & `pyrsm-0.8.3/pyrsm/data/model/ketchup.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/data/model/ratings.pkl` & `pyrsm-0.8.3/pyrsm/data/model/ratings.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/data/multivariate/carpet.pkl` & `pyrsm-0.8.3/pyrsm/data/multivariate/carpet.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/data/multivariate/city.pkl` & `pyrsm-0.8.3/pyrsm/data/multivariate/city.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/data/multivariate/city2.pkl` & `pyrsm-0.8.3/pyrsm/data/multivariate/city2.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/data/multivariate/computer.pkl` & `pyrsm-0.8.3/pyrsm/data/multivariate/computer.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/data/multivariate/movie.pkl` & `pyrsm-0.8.3/pyrsm/data/multivariate/movie.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/data/multivariate/mp3.pkl` & `pyrsm-0.8.3/pyrsm/data/multivariate/mp3.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/data/multivariate/retailers.pkl` & `pyrsm-0.8.3/pyrsm/data/multivariate/retailers.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/data/multivariate/shopping.pkl` & `pyrsm-0.8.3/pyrsm/data/multivariate/shopping.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/data/multivariate/toothpaste.pkl` & `pyrsm-0.8.3/pyrsm/data/multivariate/toothpaste.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/data/multivariate/tpbrands.pkl` & `pyrsm-0.8.3/pyrsm/data/multivariate/tpbrands.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/example_data.py` & `pyrsm-0.8.3/pyrsm/example_data.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/logit.py` & `pyrsm-0.8.3/pyrsm/logit.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/model.py` & `pyrsm-0.8.3/pyrsm/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,35 +256,36 @@
         vif = []
         for col, cat in is_categorical.items():
             if col == "Intercept":
                 continue
             elif cat:
                 select = [f"{col}[T." in c for c in df.columns]
                 Vcorr = np.linalg.det(df.loc[:, select].corr().values)
-                drop = [lcl == False for lcl in select]
+                drop = [f"{col}[T." not in c for c in df.columns]
                 Ocorr = np.linalg.det(df.loc[:, drop].corr().values)
             else:
                 Vcorr = 1
                 Ocorr = np.linalg.det(df.drop(col, axis=1).corr().values)
 
             vif.append(Vcorr * Ocorr / Xcorr)
-        df = pd.DataFrame(evar, columns=[" "])
+        df = pd.DataFrame(evar, columns=["index"])
     else:
         vif = [
             variance_inflation_factor(model.exog, i) for i in range(model.exog.shape[1])
         ]
-        df = pd.DataFrame(model.exog_names, columns=[" "])
+        df = pd.DataFrame(model.exog_names, columns=["index"])
 
     df["vif"] = vif
     df["Rsq"] = 1 - 1 / df["vif"]
 
     if "Intercept" in model.exog_names:
-        df = df[df[" "] != "Intercept"]
+        df = df[df["index"] != "Intercept"]
 
-    df = df.sort_values("vif", ascending=False).reset_index(drop=True)
+    df = df.sort_values("vif", ascending=False).set_index("index")
+    df.index.name = None
 
     if dec is not None:
         df = df.round(dec)
 
     return df
 
 
@@ -357,15 +358,17 @@
         )
     elif isinstance(fitted, sm.regression.linear_model.RegressionResultsWrapper):
         return pd.DataFrame(
             {"prediction": prediction, f"{low*100}%": Xb - me, f"{high*100}%": Xb + me}
         )
 
 
-def model_fit(fitted, dec: int = 3, prn: bool = True) -> Union[str, pd.DataFrame]:
+def model_fit(
+    fitted, dec: int = 3, prn: bool = True, shiny=False
+) -> Union[str, pd.DataFrame]:
     """
     Compute various model fit statistics for a fitted linear or logistic regression model
 
     Parameters
     ----------
     fitted : statmodels ols or glm object
         Regression model fitted using statsmodels
@@ -387,27 +390,31 @@
     mfit_dct, model_type = get_mfit(fitted)
     if not mfit_dct:
         return "Only linear and logistic regression models are currently supported."
 
     mfit = pd.DataFrame(mfit_dct)
 
     if prn:
-        output = "Model type not supported"
         if model_type == "logistic":
             output = f"""Pseudo R-squared (McFadden): {mfit.pseudo_rsq_mcf.values[0].round(dec)}
 Pseudo R-squared (McFadden adjusted): {mfit.pseudo_rsq_mcf_adj.values[0].round(dec)}
 Area under the RO Curve (AUC): {mfit.AUC.values[0].round(dec)}
 Log-likelihood: {mfit.log_likelihood.values[0].round(dec)}, AIC: {mfit.AIC.values[0].round(dec)}, BIC: {mfit.BIC.values[0].round(dec)}
 Chi-squared: {mfit.chisq.values[0].round(dec)}, df({mfit.chisq_df.values[0]}), p.value {np.where(mfit.chisq_pval.values[0] < .001, "< 0.001", mfit.chisq_pval.values[0].round(dec))} 
 Nr obs: {mfit.nobs.values[0]:,.0f}"""
         elif model_type == "regression":
             output = f"""R-squared: {mfit.rsq.values[0].round(dec)}, Adjusted R-squared: {mfit.rsq_adj.values[0].round(dec)}
 F-statistic: {mfit.fvalue[0].round(dec)} df({mfit.ftest_df_model.values[0]:.0f}, {mfit.ftest_df_resid.values[0]:.0f}), p.value {np.where(mfit.ftest_pval.values[0] < .001, "< 0.001", mfit.ftest_pval.values[0].round(dec))}
 Nr obs: {mfit.nobs.values[0]:,.0f}"""
-        return output
+        else:
+            output = "Model type not supported"
+        if shiny:
+            return output
+        else:
+            print(output)
     else:
         return mfit
 
 
 def coef_plot(
     fitted,
     alpha: float = 0.05,
@@ -500,18 +507,19 @@
     else:
         df = df.round(dec)
         df["p.values"] = ifelse(
             fitted.pvalues < 0.001, "< .001", fitted.pvalues.round(dec)
         )
 
     df["  "] = sig_stars(fitted.pvalues)
-    df = df.reset_index()
-
     if intercept is False:
-        df = df.loc[df["index"] != "Intercept"]
+        df = df[df.index != "Intercept"]
+
+    # df = df.set_index("index")
+    # df.index.name = None
 
     return df
 
 
 def evalreg(df, rvar: str, pred: str, dec: int = 3):
     """
     Evaluate regression models. Calculates R-squared, MSE, and MAE
```

### Comparing `pyrsm-0.8.2.1/pyrsm/notebook.py` & `pyrsm-0.8.3/pyrsm/notebook.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/perf.py` & `pyrsm-0.8.3/pyrsm/perf.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/props.py` & `pyrsm-0.8.3/pyrsm/props.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/radiant/logit.py` & `pyrsm-0.8.3/pyrsm/radiant/logit.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/radiant/www/style.css` & `pyrsm-0.8.3/pyrsm/radiant/www/style.css`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/regress.py` & `pyrsm-0.8.3/pyrsm/regress.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,27 +11,29 @@
     model_fit,
     extract_evars,
     extract_rvar,
     scatter_plot,
     reg_dashboard,
     residual_plot,
     coef_plot,
+    coef_ci,
     predict_ci,
 )
 from .model import vif as calc_vif
 from .visualize import distr_plot
 from .basics import correlation
 
 
 class regress:
     def __init__(
         self,
         dataset: pd.DataFrame,
         rvar: Optional[str] = None,
         evar: Optional[list[str]] = None,
+        int: Optional[list[str]] = None,
         form: Optional[str] = None,
     ) -> None:
 
         """
         Estimate linear regression model
 
         Parameters
@@ -40,32 +42,37 @@
         evar: List of strings; contains the names of the columns of data to be used as explanatory variables
         rvar: String; name of the column to be used as the response variable
         form: String; formula for the regression equation to use if evar and rvar are not provided
         """
         self.dataset = dataset
         self.rvar = rvar
         self.evar = ifelse(isinstance(evar, str), [evar], evar)
+        self.int = ifelse(isinstance(int, str), [int], int)
         self.form = form
 
         if self.form:
             self.fitted = smf.ols(formula=self.form, data=self.dataset).fit()
             self.evar = extract_evars(self.fitted.model, self.dataset.columns)
             self.rvar = extract_rvar(self.fitted.model, self.dataset.columns)
         else:
             self.form = f"{self.rvar} ~ {' + '.join(self.evar)}"
+            if self.int:
+                self.form += f"+ {' + '.join(self.int)}"
             self.fitted = smf.ols(self.form, data=self.dataset).fit()
 
         df = pd.DataFrame(self.fitted.params, columns=["coefficient"]).dropna()
         df["std.error"] = self.fitted.params / self.fitted.tvalues
         df["t.value"] = self.fitted.tvalues
         df["p.value"] = self.fitted.pvalues
         df["  "] = sig_stars(self.fitted.pvalues)
         self.coef = df.reset_index()
 
-    def summary(self, ssq=False, vif=False, dec=3, name="Not provided") -> None:
+    def summary(
+        self, ssq=False, vif=False, ci=False, dec=3, name="Not provided", shiny=False
+    ) -> None:
         """
         Summarize output from a linear regression model
 
         parameters
         ----------
         ssq: Boolean; if True, include sum of squares
         vif: Boolean; if True, include variance inflation factors
@@ -80,17 +87,23 @@
         df = self.coef.copy()
         df["coefficient"] = df["coefficient"].round(2)
         df["std.error"] = df["std.error"].round(dec)
         df["t.value"] = df["t.value"].round(dec)
         df["p.value"] = ifelse(
             df["p.value"] < 0.001, "< .001", df["p.value"].round(dec)
         )
-        print(f"\n{df.to_string(index=False)}")
+        df = df.set_index("index")
+        df.index.name = None
+        print(f"\n{df.to_string()}")
         print("\nSignif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1")
-        print(f"\n{model_fit(self.fitted)}")
+        print(f"\n{model_fit(self.fitted, shiny=shiny)}")
+
+        if ci:
+            print("\nConfidence intervals:")
+            print(f"\n{coef_ci(self.fitted).to_string()}")
 
         if ssq:
             print("\nSum of squares:")
             index = ["Regression", "Error", "Total"]
             sum_of_squares = [
                 self.fitted.ess,
                 self.fitted.ssr,
@@ -107,15 +120,15 @@
                 ),
                 SS=format_nr(sum_of_squares, dec=0),
             )
             print(f"\n{sum_of_squares.to_string()}")
 
         if vif:
             print("\nVariance inflation factors:")
-            print(f"\n{calc_vif(self.fitted).to_string(index=False)}")
+            print(f"\n{calc_vif(self.fitted).to_string()}")
 
     def predict(self, df=None, ci=False, alpha=0.05) -> pd.DataFrame:
         """
         Predict values for a linear regression model
         """
         if df is None:
             df = self.dataset
```

### Comparing `pyrsm-0.8.2.1/pyrsm/stats.py` & `pyrsm-0.8.3/pyrsm/stats.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/utils.py` & `pyrsm-0.8.3/pyrsm/utils.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/pyrsm/visualize.py` & `pyrsm-0.8.3/pyrsm/visualize.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,14 +166,16 @@
     excl = ifelse(isinstance(excl, str), [excl], excl)
     incl_int = ifelse(isinstance(incl_int, str), [incl_int], incl_int)
 
     if len(excl) > 0:
         incl = [i for i in incl if i not in excl]
 
     nr_plots = len(incl) + len(incl_int)
+    if nr_plots == 0:
+        return None
     fig, ax = plt.subplots(
         max(math.ceil(nr_plots / 2), 2), 2, figsize=(10, 2 * max(nr_plots, 4))
     )
     plt.subplots_adjust(wspace=0.25, hspace=0.25)
 
     pred_dict = {}
     for v in incl:
@@ -218,15 +220,15 @@
         is_num = [
             pd.api.types.is_numeric_dtype(df[c].dtype) and df[c].nunique() > 5
             for c in vl
         ]
         if sum(is_num) == 2:
             plot_data = (
                 pred_dict[v]
-                .pivot(vl[0], vl[1], "prediction")
+                .pivot(index=vl[0], columns=vl[1], values="prediction")
                 .transpose()
                 .sort_values(vl[1], ascending=False)
             )
             fig = sns.heatmap(
                 plot_data, ax=ax[row, col], xticklabels=False, yticklabels=False
             )
             # ax[i+j].imshow(plot_data) # not bad - investigate more
```

### Comparing `pyrsm-0.8.2.1/pyrsm.egg-info/PKG-INFO` & `pyrsm-0.8.3/pyrsm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsm
-Version: 0.8.2.1
+Version: 0.8.3
 Summary: Python functions for Customer Analytics at the Rady School of Management (RSM)
 Author: Vincent Nijs <vnijs@ucsd.edu>, Vikram Jambulapati <vikjam@ucsd.edu>, Suhas Goutham <sgoutham@ucsd.edu>, Raghav Prasad <rprasad@ucsd.edu>
 Author-email: vnijs@ucsd.edu
 License: AGPL-3.0-only
 Project-URL: Bug Reports, https://github.com/vnijs/pyrsm/issues
 Project-URL: Source, https://github.com/vnijs/pyrsm
 Description-Content-Type: text/markdown
```

### Comparing `pyrsm-0.8.2.1/pyrsm.egg-info/SOURCES.txt` & `pyrsm-0.8.3/pyrsm.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,17 @@
 pyrsm/data/multivariate/retailers.pkl
 pyrsm/data/multivariate/shopping.pkl
 pyrsm/data/multivariate/toothpaste.pkl
 pyrsm/data/multivariate/tpbrands.pkl
 pyrsm/radiant/__init__.py
 pyrsm/radiant/logit.py
 pyrsm/radiant/regress.py
+pyrsm/radiant/utils.py
 pyrsm/radiant/www/copy.js
+pyrsm/radiant/www/returnTextAreaBinding.js
 pyrsm/radiant/www/style.css
 tests/test_basics.py
 tests/test_bins.py
 tests/test_example_data.py
 tests/test_perf.py
 tests/test_regression.py
 tests/test_stats.py
```

### Comparing `pyrsm-0.8.2.1/setup.cfg` & `pyrsm-0.8.3/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -11,19 +11,18 @@
 	Bug Reports=https://github.com/vnijs/pyrsm/issues
 	Source=https://github.com/vnijs/pyrsm
 
 [options]
 include_package_data = True
 packages = find:
 install_requires = 
-	contextvars
-	mdit-py-plugins
-	shiny>=0.2.9
+	shiny>=0.3.3
 	numpy>=1.17.3
 	pandas>=0.25.2
+	polars>=0.17.14
 	seaborn>=0.9.0
 	matplotlib>=3.1.1
 	statsmodels>=0.10.1
 	scipy>=1.4.1
 	scikit-learn>=1.0.2
 	IPython>=8.0.1
 	nest-asyncio>=1.5.6
```

### Comparing `pyrsm-0.8.2.1/tests/test_basics.py` & `pyrsm-0.8.3/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/tests/test_bins.py` & `pyrsm-0.8.3/tests/test_bins.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/tests/test_example_data.py` & `pyrsm-0.8.3/tests/test_example_data.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/tests/test_perf.py` & `pyrsm-0.8.3/tests/test_perf.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/tests/test_regression.py` & `pyrsm-0.8.3/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/tests/test_stats.py` & `pyrsm-0.8.3/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.2.1/tests/test_utils.py` & `pyrsm-0.8.3/tests/test_utils.py`

 * *Files identical despite different names*

