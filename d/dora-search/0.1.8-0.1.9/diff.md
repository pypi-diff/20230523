# Comparing `tmp/dora_search-0.1.8.tar.gz` & `tmp/dora_search-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dora_search-0.1.8.tar", last modified: Thu Dec 30 10:32:42 2021, max compression
+gzip compressed data, was "dora_search-0.1.9.tar", last modified: Mon Feb 28 10:02:07 2022, max compression
```

## Comparing `dora_search-0.1.8.tar` & `dora_search-0.1.9.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2021-12-30 10:32:42.462625 dora_search-0.1.8/
--rw-r--r--   0 defossez   (501) staff       (20)     1085 2021-09-15 08:56:32.000000 dora_search-0.1.8/LICENSE
--rw-r--r--   0 defossez   (501) staff       (20)      258 2021-11-08 13:15:46.000000 dora_search-0.1.8/MANIFEST.in
--rw-r--r--   0 defossez   (501) staff       (20)      413 2021-09-07 13:13:40.000000 dora_search-0.1.8/Makefile
--rw-r--r--   0 defossez   (501) staff       (20)    34876 2021-12-30 10:32:42.462941 dora_search-0.1.8/PKG-INFO
--rw-r--r--   0 defossez   (501) staff       (20)    28782 2021-12-30 10:31:43.000000 dora_search-0.1.8/README.md
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2021-12-30 10:32:42.438321 dora_search-0.1.8/dora/
--rw-r--r--   0 defossez   (501) staff       (20)     2938 2021-12-30 10:31:53.000000 dora_search-0.1.8/dora/__init__.py
--rw-r--r--   0 defossez   (501) staff       (20)     9255 2021-12-10 10:23:25.000000 dora_search-0.1.8/dora/__main__.py
--rw-r--r--   0 defossez   (501) staff       (20)     6352 2021-12-10 10:23:25.000000 dora_search-0.1.8/dora/conf.py
--rw-r--r--   0 defossez   (501) staff       (20)     2364 2021-11-25 17:37:58.000000 dora_search-0.1.8/dora/distrib.py
--rw-r--r--   0 defossez   (501) staff       (20)     2757 2021-09-15 09:02:44.000000 dora_search-0.1.8/dora/executor.py
--rw-r--r--   0 defossez   (501) staff       (20)     8406 2021-12-07 12:58:28.000000 dora_search-0.1.8/dora/explore.py
--rw-r--r--   0 defossez   (501) staff       (20)     4663 2021-11-25 17:39:20.000000 dora_search-0.1.8/dora/git_save.py
--rw-r--r--   0 defossez   (501) staff       (20)    14105 2021-12-08 15:45:17.000000 dora_search-0.1.8/dora/grid.py
--rw-r--r--   0 defossez   (501) staff       (20)     8747 2021-12-07 14:46:57.000000 dora_search-0.1.8/dora/hydra.py
--rw-r--r--   0 defossez   (501) staff       (20)     1908 2021-09-15 09:03:07.000000 dora_search-0.1.8/dora/info.py
--rw-r--r--   0 defossez   (501) staff       (20)     2422 2021-09-15 09:03:15.000000 dora_search-0.1.8/dora/launch.py
--rw-r--r--   0 defossez   (501) staff       (20)     7507 2021-09-15 09:03:24.000000 dora_search-0.1.8/dora/lightning.py
--rw-r--r--   0 defossez   (501) staff       (20)     1873 2021-12-07 12:57:08.000000 dora_search-0.1.8/dora/link.py
--rw-r--r--   0 defossez   (501) staff       (20)     4402 2021-12-07 14:24:32.000000 dora_search-0.1.8/dora/log.py
--rw-r--r--   0 defossez   (501) staff       (20)     9252 2021-12-14 08:54:46.000000 dora_search-0.1.8/dora/main.py
--rw-r--r--   0 defossez   (501) staff       (20)     2493 2021-09-15 09:03:31.000000 dora_search-0.1.8/dora/names.py
--rw-r--r--   0 defossez   (501) staff       (20)        0 2021-04-09 10:27:27.000000 dora_search-0.1.8/dora/py.typed
--rw-r--r--   0 defossez   (501) staff       (20)     2599 2021-11-02 13:12:44.000000 dora_search-0.1.8/dora/run.py
--rw-r--r--   0 defossez   (501) staff       (20)     1652 2021-12-13 08:48:52.000000 dora_search-0.1.8/dora/share.py
--rw-r--r--   0 defossez   (501) staff       (20)    14512 2021-11-25 18:02:55.000000 dora_search-0.1.8/dora/shep.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2021-12-30 10:32:42.444723 dora_search-0.1.8/dora/tests/
--rw-r--r--   0 defossez   (501) staff       (20)      196 2021-09-15 09:01:36.000000 dora_search-0.1.8/dora/tests/__init__.py
--rw-r--r--   0 defossez   (501) staff       (20)     1691 2021-11-02 13:12:44.000000 dora_search-0.1.8/dora/tests/fake_shep.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2021-12-30 10:32:42.446881 dora_search-0.1.8/dora/tests/integ/
--rw-r--r--   0 defossez   (501) staff       (20)      196 2021-09-15 09:01:23.000000 dora_search-0.1.8/dora/tests/integ/__init__.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2021-12-30 10:32:42.447766 dora_search-0.1.8/dora/tests/integ/grids/
--rw-r--r--   0 defossez   (501) staff       (20)        0 2021-04-01 17:57:07.000000 dora_search-0.1.8/dora/tests/integ/grids/__init__.py
--rw-r--r--   0 defossez   (501) staff       (20)      629 2021-11-02 13:12:44.000000 dora_search-0.1.8/dora/tests/integ/grids/test.py
--rw-r--r--   0 defossez   (501) staff       (20)      299 2021-09-15 09:00:55.000000 dora_search-0.1.8/dora/tests/integ/other_train.py
--rw-r--r--   0 defossez   (501) staff       (20)      299 2021-09-15 09:01:25.000000 dora_search-0.1.8/dora/tests/integ/train.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2021-12-30 10:32:42.448492 dora_search-0.1.8/dora/tests/test_conf/
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2021-12-30 10:32:42.449637 dora_search-0.1.8/dora/tests/test_conf/group/
--rw-r--r--   0 defossez   (501) staff       (20)       34 2021-04-09 09:45:35.000000 dora_search-0.1.8/dora/tests/test_conf/group/lapin.yaml
--rw-r--r--   0 defossez   (501) staff       (20)       33 2021-06-21 17:58:17.000000 dora_search-0.1.8/dora/tests/test_conf/group/plop.yaml
--rw-r--r--   0 defossez   (501) staff       (20)      219 2021-11-25 17:39:59.000000 dora_search-0.1.8/dora/tests/test_conf/test_conf.yaml
--rw-r--r--   0 defossez   (501) staff       (20)     2029 2021-11-02 13:12:44.000000 dora_search-0.1.8/dora/tests/test_explore.py
--rw-r--r--   0 defossez   (501) staff       (20)     1970 2021-09-15 09:01:50.000000 dora_search-0.1.8/dora/tests/test_grid.py
--rw-r--r--   0 defossez   (501) staff       (20)     2915 2021-11-02 13:12:44.000000 dora_search-0.1.8/dora/tests/test_hydra.py
--rw-r--r--   0 defossez   (501) staff       (20)     1886 2021-12-10 10:23:25.000000 dora_search-0.1.8/dora/tests/test_integration.py
--rw-r--r--   0 defossez   (501) staff       (20)     2771 2021-12-10 10:23:25.000000 dora_search-0.1.8/dora/tests/test_main.py
--rw-r--r--   0 defossez   (501) staff       (20)      136 2021-12-10 10:23:25.000000 dora_search-0.1.8/dora/tests/test_share.py
--rw-r--r--   0 defossez   (501) staff       (20)     2343 2021-11-02 13:12:44.000000 dora_search-0.1.8/dora/tests/test_shep.py
--rw-r--r--   0 defossez   (501) staff       (20)     2056 2021-09-29 11:44:14.000000 dora_search-0.1.8/dora/tests/test_xp.py
--rw-r--r--   0 defossez   (501) staff       (20)     2458 2021-12-08 15:44:51.000000 dora_search-0.1.8/dora/utils.py
--rw-r--r--   0 defossez   (501) staff       (20)     4213 2021-12-10 10:23:25.000000 dora_search-0.1.8/dora/xp.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2021-12-30 10:32:42.452596 dora_search-0.1.8/dora_search.egg-info/
--rw-r--r--   0 defossez   (501) staff       (20)    34876 2021-12-30 10:32:41.000000 dora_search-0.1.8/dora_search.egg-info/PKG-INFO
--rw-r--r--   0 defossez   (501) staff       (20)     1515 2021-12-30 10:32:42.000000 dora_search-0.1.8/dora_search.egg-info/SOURCES.txt
--rw-r--r--   0 defossez   (501) staff       (20)        1 2021-12-30 10:32:41.000000 dora_search-0.1.8/dora_search.egg-info/dependency_links.txt
--rw-r--r--   0 defossez   (501) staff       (20)       45 2021-12-30 10:32:41.000000 dora_search-0.1.8/dora_search.egg-info/entry_points.txt
--rw-r--r--   0 defossez   (501) staff       (20)      129 2021-12-30 10:32:41.000000 dora_search-0.1.8/dora_search.egg-info/requires.txt
--rw-r--r--   0 defossez   (501) staff       (20)        5 2021-12-30 10:32:41.000000 dora_search-0.1.8/dora_search.egg-info/top_level.txt
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2021-12-30 10:32:42.418100 dora_search-0.1.8/examples/
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2021-12-30 10:32:42.453737 dora_search-0.1.8/examples/mnist/
--rw-r--r--   0 defossez   (501) staff       (20)      196 2021-09-15 09:04:22.000000 dora_search-0.1.8/examples/mnist/__init__.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2021-12-30 10:32:42.455192 dora_search-0.1.8/examples/mnist/grids/
--rw-r--r--   0 defossez   (501) staff       (20)      196 2021-09-15 09:04:16.000000 dora_search-0.1.8/examples/mnist/grids/__init__.py
--rw-r--r--   0 defossez   (501) staff       (20)      628 2021-09-15 09:04:19.000000 dora_search-0.1.8/examples/mnist/grids/test.py
--rw-r--r--   0 defossez   (501) staff       (20)     5956 2021-09-15 09:04:33.000000 dora_search-0.1.8/examples/mnist/train.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2021-12-30 10:32:42.456604 dora_search-0.1.8/examples/mnist_hydra/
--rw-r--r--   0 defossez   (501) staff       (20)      196 2021-09-15 09:04:42.000000 dora_search-0.1.8/examples/mnist_hydra/__init__.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2021-12-30 10:32:42.457300 dora_search-0.1.8/examples/mnist_hydra/conf/
--rw-r--r--   0 defossez   (501) staff       (20)      426 2021-09-15 08:56:30.000000 dora_search-0.1.8/examples/mnist_hydra/conf/config.yaml
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2021-12-30 10:32:42.458941 dora_search-0.1.8/examples/mnist_hydra/grids/
--rw-r--r--   0 defossez   (501) staff       (20)      196 2021-09-15 09:04:37.000000 dora_search-0.1.8/examples/mnist_hydra/grids/__init__.py
--rw-r--r--   0 defossez   (501) staff       (20)      756 2021-11-02 13:12:44.000000 dora_search-0.1.8/examples/mnist_hydra/grids/test.py
--rw-r--r--   0 defossez   (501) staff       (20)     4493 2021-09-15 09:04:49.000000 dora_search-0.1.8/examples/mnist_hydra/train.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2021-12-30 10:32:42.460528 dora_search-0.1.8/examples/pl/
--rw-r--r--   0 defossez   (501) staff       (20)     2074 2021-09-15 09:05:00.000000 dora_search-0.1.8/examples/pl/data.py
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2021-12-30 10:32:42.462120 dora_search-0.1.8/examples/pl/grids/
--rw-r--r--   0 defossez   (501) staff       (20)      196 2021-09-15 09:04:55.000000 dora_search-0.1.8/examples/pl/grids/__init__.py
--rw-r--r--   0 defossez   (501) staff       (20)      832 2021-09-15 09:04:58.000000 dora_search-0.1.8/examples/pl/grids/test.py
--rw-r--r--   0 defossez   (501) staff       (20)     2834 2021-10-29 15:25:40.000000 dora_search-0.1.8/examples/pl/train.py
--rw-r--r--   0 defossez   (501) staff       (20)       54 2021-09-15 08:56:30.000000 dora_search-0.1.8/pyproject.toml
--rw-r--r--   0 defossez   (501) staff       (20)      122 2021-12-09 15:52:35.000000 dora_search-0.1.8/requirements.txt
--rw-r--r--   0 defossez   (501) staff       (20)      244 2021-12-30 10:32:42.463577 dora_search-0.1.8/setup.cfg
--rw-r--r--   0 defossez   (501) staff       (20)     1955 2021-10-20 13:34:39.000000 dora_search-0.1.8/setup.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2022-02-28 10:02:07.732311 dora_search-0.1.9/
+-rw-r--r--   0 defossez   (501) staff       (20)     1085 2021-09-15 08:56:32.000000 dora_search-0.1.9/LICENSE
+-rw-r--r--   0 defossez   (501) staff       (20)      258 2021-11-08 13:15:46.000000 dora_search-0.1.9/MANIFEST.in
+-rw-r--r--   0 defossez   (501) staff       (20)      413 2021-09-07 13:13:40.000000 dora_search-0.1.9/Makefile
+-rw-r--r--   0 defossez   (501) staff       (20)    34939 2022-02-28 10:02:07.732701 dora_search-0.1.9/PKG-INFO
+-rw-r--r--   0 defossez   (501) staff       (20)    28845 2022-01-26 17:22:57.000000 dora_search-0.1.9/README.md
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2022-02-28 10:02:07.707583 dora_search-0.1.9/dora/
+-rw-r--r--   0 defossez   (501) staff       (20)     2938 2022-02-28 10:00:42.000000 dora_search-0.1.9/dora/__init__.py
+-rw-r--r--   0 defossez   (501) staff       (20)     9255 2021-12-10 10:23:25.000000 dora_search-0.1.9/dora/__main__.py
+-rw-r--r--   0 defossez   (501) staff       (20)     6384 2022-02-28 10:00:08.000000 dora_search-0.1.9/dora/conf.py
+-rw-r--r--   0 defossez   (501) staff       (20)     4004 2022-02-28 10:00:08.000000 dora_search-0.1.9/dora/distrib.py
+-rw-r--r--   0 defossez   (501) staff       (20)     2802 2022-02-28 10:00:08.000000 dora_search-0.1.9/dora/executor.py
+-rw-r--r--   0 defossez   (501) staff       (20)     8406 2021-12-07 12:58:28.000000 dora_search-0.1.9/dora/explore.py
+-rw-r--r--   0 defossez   (501) staff       (20)     6006 2022-02-28 10:00:08.000000 dora_search-0.1.9/dora/git_save.py
+-rw-r--r--   0 defossez   (501) staff       (20)    14207 2022-01-26 17:22:57.000000 dora_search-0.1.9/dora/grid.py
+-rw-r--r--   0 defossez   (501) staff       (20)     8747 2021-12-07 14:46:57.000000 dora_search-0.1.9/dora/hydra.py
+-rw-r--r--   0 defossez   (501) staff       (20)     1908 2021-09-15 09:03:07.000000 dora_search-0.1.9/dora/info.py
+-rw-r--r--   0 defossez   (501) staff       (20)     2445 2022-01-26 17:22:57.000000 dora_search-0.1.9/dora/launch.py
+-rw-r--r--   0 defossez   (501) staff       (20)     7594 2022-02-09 13:49:39.000000 dora_search-0.1.9/dora/lightning.py
+-rw-r--r--   0 defossez   (501) staff       (20)     1873 2021-12-07 12:57:08.000000 dora_search-0.1.9/dora/link.py
+-rw-r--r--   0 defossez   (501) staff       (20)     4402 2021-12-07 14:24:32.000000 dora_search-0.1.9/dora/log.py
+-rw-r--r--   0 defossez   (501) staff       (20)     9252 2021-12-14 08:54:46.000000 dora_search-0.1.9/dora/main.py
+-rw-r--r--   0 defossez   (501) staff       (20)     2493 2021-09-15 09:03:31.000000 dora_search-0.1.9/dora/names.py
+-rw-r--r--   0 defossez   (501) staff       (20)        0 2021-04-09 10:27:27.000000 dora_search-0.1.9/dora/py.typed
+-rw-r--r--   0 defossez   (501) staff       (20)     2594 2022-02-09 13:49:39.000000 dora_search-0.1.9/dora/run.py
+-rw-r--r--   0 defossez   (501) staff       (20)     1652 2021-12-13 08:48:52.000000 dora_search-0.1.9/dora/share.py
+-rw-r--r--   0 defossez   (501) staff       (20)    14507 2022-02-09 13:49:39.000000 dora_search-0.1.9/dora/shep.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2022-02-28 10:02:07.712160 dora_search-0.1.9/dora/tests/
+-rw-r--r--   0 defossez   (501) staff       (20)      196 2021-09-15 09:01:36.000000 dora_search-0.1.9/dora/tests/__init__.py
+-rw-r--r--   0 defossez   (501) staff       (20)     1691 2021-11-02 13:12:44.000000 dora_search-0.1.9/dora/tests/fake_shep.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2022-02-28 10:02:07.714445 dora_search-0.1.9/dora/tests/integ/
+-rw-r--r--   0 defossez   (501) staff       (20)      196 2021-09-15 09:01:23.000000 dora_search-0.1.9/dora/tests/integ/__init__.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2022-02-28 10:02:07.715701 dora_search-0.1.9/dora/tests/integ/grids/
+-rw-r--r--   0 defossez   (501) staff       (20)        0 2021-04-01 17:57:07.000000 dora_search-0.1.9/dora/tests/integ/grids/__init__.py
+-rw-r--r--   0 defossez   (501) staff       (20)      629 2021-11-02 13:12:44.000000 dora_search-0.1.9/dora/tests/integ/grids/test.py
+-rw-r--r--   0 defossez   (501) staff       (20)      299 2021-09-15 09:00:55.000000 dora_search-0.1.9/dora/tests/integ/other_train.py
+-rw-r--r--   0 defossez   (501) staff       (20)      299 2021-09-15 09:01:25.000000 dora_search-0.1.9/dora/tests/integ/train.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2022-02-28 10:02:07.716691 dora_search-0.1.9/dora/tests/test_conf/
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2022-02-28 10:02:07.717838 dora_search-0.1.9/dora/tests/test_conf/group/
+-rw-r--r--   0 defossez   (501) staff       (20)       34 2021-04-09 09:45:35.000000 dora_search-0.1.9/dora/tests/test_conf/group/lapin.yaml
+-rw-r--r--   0 defossez   (501) staff       (20)       33 2021-06-21 17:58:17.000000 dora_search-0.1.9/dora/tests/test_conf/group/plop.yaml
+-rw-r--r--   0 defossez   (501) staff       (20)      219 2021-11-25 17:39:59.000000 dora_search-0.1.9/dora/tests/test_conf/test_conf.yaml
+-rw-r--r--   0 defossez   (501) staff       (20)     2029 2021-11-02 13:12:44.000000 dora_search-0.1.9/dora/tests/test_explore.py
+-rw-r--r--   0 defossez   (501) staff       (20)     1970 2021-09-15 09:01:50.000000 dora_search-0.1.9/dora/tests/test_grid.py
+-rw-r--r--   0 defossez   (501) staff       (20)     2912 2022-02-09 13:49:39.000000 dora_search-0.1.9/dora/tests/test_hydra.py
+-rw-r--r--   0 defossez   (501) staff       (20)     1886 2021-12-10 10:23:25.000000 dora_search-0.1.9/dora/tests/test_integration.py
+-rw-r--r--   0 defossez   (501) staff       (20)     2771 2021-12-10 10:23:25.000000 dora_search-0.1.9/dora/tests/test_main.py
+-rw-r--r--   0 defossez   (501) staff       (20)      333 2022-02-28 10:00:08.000000 dora_search-0.1.9/dora/tests/test_share.py
+-rw-r--r--   0 defossez   (501) staff       (20)     2343 2021-11-02 13:12:44.000000 dora_search-0.1.9/dora/tests/test_shep.py
+-rw-r--r--   0 defossez   (501) staff       (20)     2056 2021-09-29 11:44:14.000000 dora_search-0.1.9/dora/tests/test_xp.py
+-rw-r--r--   0 defossez   (501) staff       (20)     3180 2022-01-26 17:22:57.000000 dora_search-0.1.9/dora/utils.py
+-rw-r--r--   0 defossez   (501) staff       (20)     4213 2021-12-10 10:23:25.000000 dora_search-0.1.9/dora/xp.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2022-02-28 10:02:07.721563 dora_search-0.1.9/dora_search.egg-info/
+-rw-r--r--   0 defossez   (501) staff       (20)    34939 2022-02-28 10:02:06.000000 dora_search-0.1.9/dora_search.egg-info/PKG-INFO
+-rw-r--r--   0 defossez   (501) staff       (20)     1515 2022-02-28 10:02:06.000000 dora_search-0.1.9/dora_search.egg-info/SOURCES.txt
+-rw-r--r--   0 defossez   (501) staff       (20)        1 2022-02-28 10:02:06.000000 dora_search-0.1.9/dora_search.egg-info/dependency_links.txt
+-rw-r--r--   0 defossez   (501) staff       (20)       45 2022-02-28 10:02:06.000000 dora_search-0.1.9/dora_search.egg-info/entry_points.txt
+-rw-r--r--   0 defossez   (501) staff       (20)      129 2022-02-28 10:02:06.000000 dora_search-0.1.9/dora_search.egg-info/requires.txt
+-rw-r--r--   0 defossez   (501) staff       (20)        5 2022-02-28 10:02:06.000000 dora_search-0.1.9/dora_search.egg-info/top_level.txt
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2022-02-28 10:02:07.692220 dora_search-0.1.9/examples/
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2022-02-28 10:02:07.722736 dora_search-0.1.9/examples/mnist/
+-rw-r--r--   0 defossez   (501) staff       (20)      196 2021-09-15 09:04:22.000000 dora_search-0.1.9/examples/mnist/__init__.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2022-02-28 10:02:07.724174 dora_search-0.1.9/examples/mnist/grids/
+-rw-r--r--   0 defossez   (501) staff       (20)      196 2021-09-15 09:04:16.000000 dora_search-0.1.9/examples/mnist/grids/__init__.py
+-rw-r--r--   0 defossez   (501) staff       (20)      628 2021-09-15 09:04:19.000000 dora_search-0.1.9/examples/mnist/grids/test.py
+-rw-r--r--   0 defossez   (501) staff       (20)     5956 2021-09-15 09:04:33.000000 dora_search-0.1.9/examples/mnist/train.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2022-02-28 10:02:07.725473 dora_search-0.1.9/examples/mnist_hydra/
+-rw-r--r--   0 defossez   (501) staff       (20)      196 2021-09-15 09:04:42.000000 dora_search-0.1.9/examples/mnist_hydra/__init__.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2022-02-28 10:02:07.726291 dora_search-0.1.9/examples/mnist_hydra/conf/
+-rw-r--r--   0 defossez   (501) staff       (20)      426 2021-09-15 08:56:30.000000 dora_search-0.1.9/examples/mnist_hydra/conf/config.yaml
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2022-02-28 10:02:07.728147 dora_search-0.1.9/examples/mnist_hydra/grids/
+-rw-r--r--   0 defossez   (501) staff       (20)      196 2021-09-15 09:04:37.000000 dora_search-0.1.9/examples/mnist_hydra/grids/__init__.py
+-rw-r--r--   0 defossez   (501) staff       (20)      756 2021-11-02 13:12:44.000000 dora_search-0.1.9/examples/mnist_hydra/grids/test.py
+-rw-r--r--   0 defossez   (501) staff       (20)     4493 2021-09-15 09:04:49.000000 dora_search-0.1.9/examples/mnist_hydra/train.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2022-02-28 10:02:07.730090 dora_search-0.1.9/examples/pl/
+-rw-r--r--   0 defossez   (501) staff       (20)     2074 2021-09-15 09:05:00.000000 dora_search-0.1.9/examples/pl/data.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2022-02-28 10:02:07.731494 dora_search-0.1.9/examples/pl/grids/
+-rw-r--r--   0 defossez   (501) staff       (20)      196 2021-09-15 09:04:55.000000 dora_search-0.1.9/examples/pl/grids/__init__.py
+-rw-r--r--   0 defossez   (501) staff       (20)      832 2021-09-15 09:04:58.000000 dora_search-0.1.9/examples/pl/grids/test.py
+-rw-r--r--   0 defossez   (501) staff       (20)     2834 2021-10-29 15:25:40.000000 dora_search-0.1.9/examples/pl/train.py
+-rw-r--r--   0 defossez   (501) staff       (20)       54 2021-09-15 08:56:30.000000 dora_search-0.1.9/pyproject.toml
+-rw-r--r--   0 defossez   (501) staff       (20)      122 2021-12-09 15:52:35.000000 dora_search-0.1.9/requirements.txt
+-rw-r--r--   0 defossez   (501) staff       (20)      244 2022-02-28 10:02:07.733837 dora_search-0.1.9/setup.cfg
+-rw-r--r--   0 defossez   (501) staff       (20)     1955 2021-10-20 13:34:39.000000 dora_search-0.1.9/setup.py
```

### Comparing `dora_search-0.1.8/LICENSE` & `dora_search-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dora_search-0.1.8/PKG-INFO` & `dora_search-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dora_search
-Version: 0.1.8
+Version: 0.1.9
 Summary: Easy grid searches for ML.
 Home-page: https://github.com/facebookresearch/dora
 Author: Alexandre Défossez
 Author-email: defossez@fb.com
 License: MIT
 Description: 
         # Dora The Explorer, a friendly experiment manager
@@ -47,15 +47,15 @@
         pip install -U dora-search
         ```
         
         ## What's up?
         
         See [the changelog](CHANGELOG.md) for details on releases.
         
-        - 2021-12-10: version 0.1.8a: see changelog, many of small changes.
+        - 2021-12-10: version 0.1.8: see changelog, many of small changes.
         - 2021-11-08: version 0.1.7: support for job arrays added.
         - 2021-10-20: version 0.1.6 released, bug fixes.
         - 2021-09-29: version 0.1.5 released.
         - 2021-09-07: added support for a `git_save` option. This will ensure that the project git is clean
             and make a clone from which the experiment will run. This does not apply to `dora run` for easier
             debugging (but you can force it with `--git_save`).
         - 2021-06-21: added support for Hydra 1.1. Be very careful if you update to Hydra 1.1, there are some non backward compatible changes in the way group config are parsed, see [the Hydra release notes](https://hydra.cc/docs/upgrades/1.0_to_1.1/default_composition_order) for more information.
@@ -475,16 +475,16 @@
         Dora provides some API, including the possibility to run grid searches
         directly from an IPython notebook. See the
         [Dora API](https://facebookresearch.github.io/dora/dora).
         
         ### DecoratedMain
         
         The most useful class is the
-        [DecoratedMain](https://share.honu.io/dora/dora/main.html#dora.main.DecoratedMain), which is the decorated main function in your project. You can use it
-        to retrieve an [XP object](https://share.honu.io/dora/dora/xp.html#dora.xp.XP)
+        [DecoratedMain](https://facebookresearch.github.io/dora/dora/main.html#dora.main.DecoratedMain), which is the decorated main function in your project. You can use it
+        to retrieve an [XP object](https://facebookresearch.github.io/dora/dora/xp.html#dora.xp.XP)
         from a list of argv, or a signature:
         
         ```python
         
         from myproj.train import main
         
         xp = main.get_xp_from_sig('ae43f645')
@@ -502,17 +502,17 @@
         to inherit `dora.main.ArgparseMain` or `dora.hydra.HydraMain` and use your
         custom class instead.
         
         ### Grid API
         
         You can schedule and manage grids from the Dora API rather than the command-line.
         This is useful to manage XPs from a notebook for instance!
-        See the [dora.grid.run_grid](https://share.honu.io/dora/dora/grid.html#dora.grid.run_grid).
-        Flags are passed with as an instance of  [dora.grid.RunGridArgs](https://share.honu.io/dora/dora/grid.html#dora.grid.RunGridArgs).
-        Submission rules (e.g. cancel, retry etc.) are passed as a [dora.conf.SubmitRules](https://share.honu.io/dora/dora/conf.html#dora.conf.SubmitRules).
+        See the [dora.grid.run_grid](https://facebookresearch.github.io/dora/dora/grid.html#dora.grid.run_grid).
+        Flags are passed with as an instance of  [dora.grid.RunGridArgs](https://facebookresearch.github.io/dora/dora/grid.html#dora.grid.RunGridArgs).
+        Submission rules (e.g. cancel, retry etc.) are passed as a [dora.conf.SubmitRules](https://facebookresearch.github.io/dora/dora/conf.html#dora.conf.SubmitRules).
         
         ```python
         import dora
         import dora.grid
         
         from myproj.train import main
         
@@ -579,15 +579,15 @@
         
         You can now configure a secondary shared XPs repository where only mappings from SIG -> hyper params are stored. With Hydra you can add
         ```yaml
         dora:
             dir: outputs
             shared: /shared_folder/shared_xps
         ```
-        Then other teammates can reference any SIG from an XP launched by other team members within the Dora commands. 
+        Then other teammates can reference any SIG from an XP launched by other team members within the Dora commands.
         
         
         ## Advanced configuration
         
         
         ### Setting SLURM default parameters
```

### Comparing `dora_search-0.1.8/README.md` & `dora_search-0.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 pip install -U dora-search
 ```
 
 ## What's up?
 
 See [the changelog](CHANGELOG.md) for details on releases.
 
-- 2021-12-10: version 0.1.8a: see changelog, many of small changes.
+- 2021-12-10: version 0.1.8: see changelog, many of small changes.
 - 2021-11-08: version 0.1.7: support for job arrays added.
 - 2021-10-20: version 0.1.6 released, bug fixes.
 - 2021-09-29: version 0.1.5 released.
 - 2021-09-07: added support for a `git_save` option. This will ensure that the project git is clean
     and make a clone from which the experiment will run. This does not apply to `dora run` for easier
     debugging (but you can force it with `--git_save`).
 - 2021-06-21: added support for Hydra 1.1. Be very careful if you update to Hydra 1.1, there are some non backward compatible changes in the way group config are parsed, see [the Hydra release notes](https://hydra.cc/docs/upgrades/1.0_to_1.1/default_composition_order) for more information.
@@ -466,16 +466,16 @@
 Dora provides some API, including the possibility to run grid searches
 directly from an IPython notebook. See the
 [Dora API](https://facebookresearch.github.io/dora/dora).
 
 ### DecoratedMain
 
 The most useful class is the
-[DecoratedMain](https://share.honu.io/dora/dora/main.html#dora.main.DecoratedMain), which is the decorated main function in your project. You can use it
-to retrieve an [XP object](https://share.honu.io/dora/dora/xp.html#dora.xp.XP)
+[DecoratedMain](https://facebookresearch.github.io/dora/dora/main.html#dora.main.DecoratedMain), which is the decorated main function in your project. You can use it
+to retrieve an [XP object](https://facebookresearch.github.io/dora/dora/xp.html#dora.xp.XP)
 from a list of argv, or a signature:
 
 ```python
 
 from myproj.train import main
 
 xp = main.get_xp_from_sig('ae43f645')
@@ -493,17 +493,17 @@
 to inherit `dora.main.ArgparseMain` or `dora.hydra.HydraMain` and use your
 custom class instead.
 
 ### Grid API
 
 You can schedule and manage grids from the Dora API rather than the command-line.
 This is useful to manage XPs from a notebook for instance!
-See the [dora.grid.run_grid](https://share.honu.io/dora/dora/grid.html#dora.grid.run_grid).
-Flags are passed with as an instance of  [dora.grid.RunGridArgs](https://share.honu.io/dora/dora/grid.html#dora.grid.RunGridArgs).
-Submission rules (e.g. cancel, retry etc.) are passed as a [dora.conf.SubmitRules](https://share.honu.io/dora/dora/conf.html#dora.conf.SubmitRules).
+See the [dora.grid.run_grid](https://facebookresearch.github.io/dora/dora/grid.html#dora.grid.run_grid).
+Flags are passed with as an instance of  [dora.grid.RunGridArgs](https://facebookresearch.github.io/dora/dora/grid.html#dora.grid.RunGridArgs).
+Submission rules (e.g. cancel, retry etc.) are passed as a [dora.conf.SubmitRules](https://facebookresearch.github.io/dora/dora/conf.html#dora.conf.SubmitRules).
 
 ```python
 import dora
 import dora.grid
 
 from myproj.train import main
 
@@ -570,15 +570,15 @@
 
 You can now configure a secondary shared XPs repository where only mappings from SIG -> hyper params are stored. With Hydra you can add
 ```yaml
 dora:
     dir: outputs
     shared: /shared_folder/shared_xps
 ```
-Then other teammates can reference any SIG from an XP launched by other team members within the Dora commands. 
+Then other teammates can reference any SIG from an XP launched by other team members within the Dora commands.
 
 
 ## Advanced configuration
 
 
 ### Setting SLURM default parameters
```

### Comparing `dora_search-0.1.8/dora/__init__.py` & `dora_search-0.1.9/dora/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 
 
 """
 __pdoc__ = {}
 __pdoc__['tests'] = False
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 
 # flake8: noqa
 from .explore import Explorer, Launcher
 try:
     import hydra
 except ImportError:
     pass
```

### Comparing `dora_search-0.1.8/dora/__main__.py` & `dora_search-0.1.9/dora/__main__.py`

 * *Files identical despite different names*

### Comparing `dora_search-0.1.8/dora/conf.py` & `dora_search-0.1.9/dora/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,14 +149,15 @@
 
     # Those are internal config values and are unlikely to be changed
     history: str = "history.json"  # where metrics will be stored
     xps: str = "xps"  # subfolder to store xps
 
     shep: ShepConfig = field(default_factory=ShepConfig)
     rendezvous_file: str = "rendezvous.txt"
+    use_rendezvous: bool = True
     grids: str = "grids"
     codes: str = "codes"
 
     def is_excluded(self, arg_name: str) -> bool:
         """Return True if the given argument name should be excluded from
         the signature."""
         for pattern in self.exclude:
```

### Comparing `dora_search-0.1.8/dora/executor.py` & `dora_search-0.1.9/dora/executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,14 +71,15 @@
     log(f"Starting {world_size} worker processes for DDP.")
     with ChildrenManager() as manager:
         for rank in range(world_size):
             kwargs = {}
             env = dict(os.environ)
             env['RANK'] = str(rank)
             env['WORLD_SIZE'] = str(world_size)
+            env['MASTER_ADDR'] = '127.0.0.1'
             args = ["-m", "dora", "-P", package, "run", "--"]
             args += argv
             if rank > 0:
                 kwargs['stdin'] = sp.DEVNULL
                 kwargs['stdout'] = open(xp.folder / f'worker_{rank}.log', 'w')
                 kwargs['stderr'] = sp.STDOUT
             manager.add(
```

### Comparing `dora_search-0.1.8/dora/explore.py` & `dora_search-0.1.9/dora/explore.py`

 * *Files identical despite different names*

### Comparing `dora_search-0.1.8/dora/git_save.py` & `dora_search-0.1.9/dora/git_save.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # Copyright (c) Facebook, Inc. and its affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 
 from contextlib import contextmanager
+import importlib.util
 import logging
 import os
 import shlex
 import subprocess as sp
 import typing as tp
 from pathlib import Path
 
-from .conf import DoraConfig
+from .main import DecoratedMain
 from .log import fatal
 from .xp import XP
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -29,20 +30,54 @@
     if proc.returncode:
         command_str = " ".join(shlex.quote(c) for c in command)
         raise CommandError(
             f"Command {command_str} failed ({proc.returncode}): \n" + proc.stdout.decode())
     return proc.stdout.decode().strip()
 
 
-def check_repo_clean():
+def check_repo_clean(root: Path, main: DecoratedMain):
     out = run_command(['git', 'status', '--porcelain'])
-    clean = out == ""
-    if not clean:
+    filtered = []
+    # Here we try to detect the grids package and allow uncommitted changes
+    # only to that folder. The rational is that as we edit the grid file, it is a pain
+    # to constantly be commiting change to it and it should not impact the actual run code.
+    grid_name = main.name + ".grids"
+    spec = importlib.util.find_spec(grid_name)
+    grid_path: tp.Optional[Path] = None
+    if spec is not None:
+        assert spec.origin is not None
+        grid_path = Path(spec.origin).resolve().parent
+    for line in out.split("\n"):
+        if not line:
+            continue
+        parts = shlex.split(line)
+        paths: tp.List[str] = []
+        if len(parts) == 2:
+            paths.append(parts[1])
+        elif len(parts) == 4:
+            assert parts[3] == "->"
+            paths += [parts[1], parts[2]]
+        else:
+            assert "Invalid parts", parts
+        line_clean = True
+        for path in paths:
+            if grid_path is None:
+                line_clean = False
+                break
+            rpath = (root / path).resolve()
+            try:
+                rpath.relative_to(grid_path)
+            except ValueError:
+                line_clean = False
+        if not line_clean:
+            filtered.append(line)
+    if filtered:
+        files = '\n'.join(filtered)
         fatal("Repository is not clean! The following files should be commited "
-              f"or git ignored: \n {out}")
+              f"or git ignored: \n {files}")
 
 
 def get_git_root():
     return Path(run_command(['git', 'rev-parse', '--show-toplevel'])).resolve()
 
 
 def get_git_commit(repo: Path = Path('.')):
@@ -58,20 +93,20 @@
     # clone to a specific commit (only specific branch or tag).
     actual_commit = get_git_commit(tmp_target)
     actual_target = target.parent / actual_commit
     tmp_target.rename(actual_target)
     return actual_target
 
 
-def get_new_clone(dora_conf: DoraConfig) -> Path:
+def get_new_clone(main: DecoratedMain) -> Path:
     """Return a fresh clone in side the given path."""
     source = get_git_root()
     commit = get_git_commit()
-    check_repo_clean()
-    codes = dora_conf.dir / dora_conf.codes
+    check_repo_clean(source, main)
+    codes = main.dora.dir / main.dora.codes
     codes.mkdir(parents=True, exist_ok=True)
     target = codes / commit
     if not target.exists():
         target = shallow_clone(source, target)
     assert target.exists()
     return target
```

### Comparing `dora_search-0.1.8/dora/grid.py` & `dora_search-0.1.9/dora/grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import time
 
 from .conf import SlurmConfig, SubmitRules, update_from_args
 from .explore import Explorer, Launcher, Herd
 from .main import DecoratedMain
 from .log import colorize, simple_log, fatal
 from .shep import Sheep, Shepherd
-from .utils import import_or_fatal, try_load
+from .utils import import_or_fatal, reliable_rmtree, try_load
 
 import treetable as tt
 
 log: tp.Callable[[str], None] = partial(simple_log, "Grid:")
 
 
 def no_print(*args, **kwargs):
@@ -187,15 +187,15 @@
         for sheep in sheeps:
             if sheep.job is not None:
                 shepherd.cancel_lazy(sheep.job)
         shepherd.commit()
         log("Deleting XP folders...")
         for sheep in sheeps:
             if sheep.xp.folder.exists():
-                shutil.rmtree(sheep.xp.folder)
+                reliable_rmtree(sheep.xp.folder)
             sheep.job = None
 
     to_unlink = []
     old_sheeps = []
     for child in grid_folder.iterdir():
         if child.name not in herd.sheeps:
             to_unlink.append(child)
@@ -300,19 +300,19 @@
     maybe_print: tp.Callable
     if args.silent:
         maybe_print = no_print
     else:
         maybe_print = print
     maybe_print(f"Monitoring Grid {grid_name}")
     while True:
-        if args.jupyter:
+        if args.jupyter and not args.silent:
             from IPython import display
             display.clear_output(wait=True)
         shepherd.update()
-        if monitor(args, main, explorer, sheeps):
+        if monitor(args, main, explorer, sheeps, maybe_print):
             # All jobs finished or failed, stop monitoring
             break
         if not args.monitor:
             break
         sleep = int(args.interval * 60)
         maybe_print()
         for ela in range(sleep):
@@ -358,15 +358,16 @@
         if _match_name(name, patterns):
             out.append(sheep)
     if indexes:
         out = [out[idx] for idx in indexes]
     return out
 
 
-def monitor(args: tp.Any, main: DecoratedMain, explorer: Explorer, herd: tp.List[Sheep]) -> bool:
+def monitor(args: tp.Any, main: DecoratedMain, explorer: Explorer, herd: tp.List[Sheep],
+            maybe_print: tp.Callable) -> bool:
     """Single iteration of monitoring of the jobs in a Grid.
     Returns `True` if all jobs are done or failed, and `False` otherwise.
     """
     names, base_name = main.get_names([sheep.xp for sheep in herd])
     histories = [main.get_xp_history(sheep.xp) for sheep in herd]
 
     trim = None
@@ -401,16 +402,16 @@
             other = explorer.process_sheep(sheep, history)
         except NotImplementedError:
             other = explorer.process_history(history)
         line.update(other)
         lines.append(line)
 
     if base_name:
-        print("Base name: ", base_name)
+        maybe_print("Base name: ", base_name)
     table = tt.table(
         shorten=True,
         groups=[
             tt.group("Meta", explorer.get_grid_meta()),
         ] + explorer.get_grid_metrics()
     )
-    print(tt.treetable(lines, table, colors=explorer.get_colors()))
+    maybe_print(tt.treetable(lines, table, colors=explorer.get_colors()))
     return finished
```

### Comparing `dora_search-0.1.8/dora/hydra.py` & `dora_search-0.1.9/dora/hydra.py`

 * *Files identical despite different names*

### Comparing `dora_search-0.1.8/dora/info.py` & `dora_search-0.1.9/dora/info.py`

 * *Files identical despite different names*

### Comparing `dora_search-0.1.8/dora/launch.py` & `dora_search-0.1.9/dora/launch.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 
 """
 Launch command.
 """
 from functools import partial
-import shutil
 import subprocess as sp
 import time
 
 from .conf import SubmitRules, update_from_args
 from .main import DecoratedMain
 from .shep import Shepherd
 from .log import simple_log
+from .utils import reliable_rmtree
 
 log = partial(simple_log, "Launch:")
 
 
 def launch_action(args, main: DecoratedMain):
     shepherd = Shepherd(main, log=log)
     slurm = main.get_slurm_config()
@@ -42,15 +42,15 @@
     if args.clear:
         log("Canceling current job...")
         if sheep.job is not None:
             shepherd.cancel_lazy(sheep.job)
         shepherd.commit()
         log("Deleting XP folder...")
         if sheep.xp.folder.exists():
-            shutil.rmtree(sheep.xp.folder)
+            reliable_rmtree(sheep.xp.folder)
         sheep.job = None
 
     shepherd.maybe_submit_lazy(sheep, slurm, rules)
     shepherd.commit()
 
     if args.tail or args.attach:
         done = False
```

### Comparing `dora_search-0.1.8/dora/lightning.py` & `dora_search-0.1.9/dora/lightning.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,18 @@
     def __init__(self):
         super().__init__()
         self.spec = distrib.get_distrib_spec()
 
     def creates_children(self) -> bool:
         return True
 
+    @property
+    def creates_processes_externally(self) -> bool:
+        return True
+
     def master_address(self) -> str:
         return ""
 
     def master_port(self) -> int:
         assert False
 
     def world_size(self) -> int:
```

### Comparing `dora_search-0.1.8/dora/link.py` & `dora_search-0.1.9/dora/link.py`

 * *Files identical despite different names*

### Comparing `dora_search-0.1.8/dora/log.py` & `dora_search-0.1.9/dora/log.py`

 * *Files identical despite different names*

### Comparing `dora_search-0.1.8/dora/main.py` & `dora_search-0.1.9/dora/main.py`

 * *Files identical despite different names*

### Comparing `dora_search-0.1.8/dora/names.py` & `dora_search-0.1.9/dora/names.py`

 * *Files identical despite different names*

### Comparing `dora_search-0.1.8/dora/run.py` & `dora_search-0.1.9/dora/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 
 def run_action(args, main: DecoratedMain):
     xp = main.get_xp(args.argv)
     with ExitStack() as stack:
         if args.git_save and '_DORA_GIT_SAVE_DONE' not in os.environ:
             os.environ['_DORA_GIT_SAVE_DONE'] = '1'
-            clone = git_save.get_new_clone(main.dora)
+            clone = git_save.get_new_clone(main)
             git_save.assign_clone(xp, clone)
             stack.enter_context(git_save.enter_clone(clone))
             os.execv(sys.executable, [sys.executable, "-m", "dora"] + sys.argv[1:])
         if args.ddp and not os.environ.get('RANK'):
             check_job_and_clear(args.argv, main, args.clear)
             start_ddp_workers(args.package, main, args.argv)
         else:
```

### Comparing `dora_search-0.1.8/dora/share.py` & `dora_search-0.1.9/dora/share.py`

 * *Files identical despite different names*

### Comparing `dora_search-0.1.8/dora/shep.py` & `dora_search-0.1.9/dora/shep.py`

 * *Files 1% similar despite different names*

```diff
@@ -352,15 +352,15 @@
             self.main.init_xp(xp)
             if xp.rendezvous_file.exists():
                 xp.rendezvous_file.unlink()
 
         executor = self._get_submitit_executor(name, submitit_folder, slurm_config)
         jobs: tp.List[submitit.Job] = []
         if use_git_save and self._existing_git_clone is None:
-            self._existing_git_clone = git_save.get_new_clone(self.main.dora)
+            self._existing_git_clone = git_save.get_new_clone(self.main)
         with self._enter_orphan(name):
             with ExitStack() as stack:
                 if use_git_save:
                     assert self._existing_git_clone is not None
                     stack.enter_context(git_save.enter_clone(self._existing_git_clone))
                 if is_array:
                     stack.enter_context(executor.batch())
```

### Comparing `dora_search-0.1.8/dora/tests/fake_shep.py` & `dora_search-0.1.9/dora/tests/fake_shep.py`

 * *Files identical despite different names*

### Comparing `dora_search-0.1.8/dora/tests/integ/grids/test.py` & `dora_search-0.1.9/dora/tests/integ/grids/test.py`

 * *Files identical despite different names*

### Comparing `dora_search-0.1.8/dora/tests/test_explore.py` & `dora_search-0.1.9/dora/tests/test_explore.py`

 * *Files identical despite different names*

### Comparing `dora_search-0.1.8/dora/tests/test_grid.py` & `dora_search-0.1.9/dora/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `dora_search-0.1.8/dora/tests/test_hydra.py` & `dora_search-0.1.9/dora/tests/test_hydra.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     _main.__module__ = __name__
     main = get_main(tmpdir)
     argv = ['optim.loss=git_save']
     xp = main.get_xp(argv)
     main.init_xp(xp)
     xp.dora.git_save = True
 
-    clone = get_new_clone(xp.dora)
+    clone = get_new_clone(main)
     assign_clone(xp, clone)
     with enter_clone(clone):
         call(main, argv)
 
 
 def test_hydra(tmpdir):
     _main.__module__ = __name__
```

### Comparing `dora_search-0.1.8/dora/tests/test_integration.py` & `dora_search-0.1.9/dora/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `dora_search-0.1.8/dora/tests/test_main.py` & `dora_search-0.1.9/dora/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `dora_search-0.1.8/dora/tests/test_shep.py` & `dora_search-0.1.9/dora/tests/test_shep.py`

 * *Files identical despite different names*

### Comparing `dora_search-0.1.8/dora/tests/test_xp.py` & `dora_search-0.1.9/dora/tests/test_xp.py`

 * *Files identical despite different names*

### Comparing `dora_search-0.1.8/dora/utils.py` & `dora_search-0.1.9/dora/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 from contextlib import contextmanager
 import importlib
 import logging
 import os
 from pathlib import Path
 import pickle
+from shutil import rmtree
+import tempfile
 import typing as tp
 
 from omegaconf.basecontainer import BaseContainer
 from omegaconf import OmegaConf
 
 from .log import fatal
 
@@ -72,7 +74,27 @@
 
 def import_or_fatal(module_name: str) -> tp.Any:
     try:
         return importlib.import_module(module_name)
     except ImportError:
         logger.info("Could not import module %s", module_name, exc_info=True)
         fatal(f"Failed to import module {module_name}.")
+
+
+def reliable_rmtree(path: Path):
+    """Reliably delete the given folder, trying to remove while ignoring errors,
+    and if any files remain, renaming to some trash folder."""
+    error = False
+
+    def _on_error(func, error_path, exc_info):
+        nonlocal error
+        error = True
+        logger.warning(f"Error deleting file {error_path}")
+
+    rmtree(path, onerror=_on_error)
+    if error:
+        assert path.exists()
+        target_name = tempfile.mkdtemp(dir=path.parent, prefix=path.name + "_", suffix="_trash")
+        logger.warning(f"Deletion of {path} failed, moving to {target_name}")
+        path.rename(target_name)
+    else:
+        assert not path.exists()
```

### Comparing `dora_search-0.1.8/dora/xp.py` & `dora_search-0.1.9/dora/xp.py`

 * *Files identical despite different names*

### Comparing `dora_search-0.1.8/dora_search.egg-info/PKG-INFO` & `dora_search-0.1.9/dora_search.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dora-search
-Version: 0.1.8
+Version: 0.1.9
 Summary: Easy grid searches for ML.
 Home-page: https://github.com/facebookresearch/dora
 Author: Alexandre Défossez
 Author-email: defossez@fb.com
 License: MIT
 Description: 
         # Dora The Explorer, a friendly experiment manager
@@ -47,15 +47,15 @@
         pip install -U dora-search
         ```
         
         ## What's up?
         
         See [the changelog](CHANGELOG.md) for details on releases.
         
-        - 2021-12-10: version 0.1.8a: see changelog, many of small changes.
+        - 2021-12-10: version 0.1.8: see changelog, many of small changes.
         - 2021-11-08: version 0.1.7: support for job arrays added.
         - 2021-10-20: version 0.1.6 released, bug fixes.
         - 2021-09-29: version 0.1.5 released.
         - 2021-09-07: added support for a `git_save` option. This will ensure that the project git is clean
             and make a clone from which the experiment will run. This does not apply to `dora run` for easier
             debugging (but you can force it with `--git_save`).
         - 2021-06-21: added support for Hydra 1.1. Be very careful if you update to Hydra 1.1, there are some non backward compatible changes in the way group config are parsed, see [the Hydra release notes](https://hydra.cc/docs/upgrades/1.0_to_1.1/default_composition_order) for more information.
@@ -475,16 +475,16 @@
         Dora provides some API, including the possibility to run grid searches
         directly from an IPython notebook. See the
         [Dora API](https://facebookresearch.github.io/dora/dora).
         
         ### DecoratedMain
         
         The most useful class is the
-        [DecoratedMain](https://share.honu.io/dora/dora/main.html#dora.main.DecoratedMain), which is the decorated main function in your project. You can use it
-        to retrieve an [XP object](https://share.honu.io/dora/dora/xp.html#dora.xp.XP)
+        [DecoratedMain](https://facebookresearch.github.io/dora/dora/main.html#dora.main.DecoratedMain), which is the decorated main function in your project. You can use it
+        to retrieve an [XP object](https://facebookresearch.github.io/dora/dora/xp.html#dora.xp.XP)
         from a list of argv, or a signature:
         
         ```python
         
         from myproj.train import main
         
         xp = main.get_xp_from_sig('ae43f645')
@@ -502,17 +502,17 @@
         to inherit `dora.main.ArgparseMain` or `dora.hydra.HydraMain` and use your
         custom class instead.
         
         ### Grid API
         
         You can schedule and manage grids from the Dora API rather than the command-line.
         This is useful to manage XPs from a notebook for instance!
-        See the [dora.grid.run_grid](https://share.honu.io/dora/dora/grid.html#dora.grid.run_grid).
-        Flags are passed with as an instance of  [dora.grid.RunGridArgs](https://share.honu.io/dora/dora/grid.html#dora.grid.RunGridArgs).
-        Submission rules (e.g. cancel, retry etc.) are passed as a [dora.conf.SubmitRules](https://share.honu.io/dora/dora/conf.html#dora.conf.SubmitRules).
+        See the [dora.grid.run_grid](https://facebookresearch.github.io/dora/dora/grid.html#dora.grid.run_grid).
+        Flags are passed with as an instance of  [dora.grid.RunGridArgs](https://facebookresearch.github.io/dora/dora/grid.html#dora.grid.RunGridArgs).
+        Submission rules (e.g. cancel, retry etc.) are passed as a [dora.conf.SubmitRules](https://facebookresearch.github.io/dora/dora/conf.html#dora.conf.SubmitRules).
         
         ```python
         import dora
         import dora.grid
         
         from myproj.train import main
         
@@ -579,15 +579,15 @@
         
         You can now configure a secondary shared XPs repository where only mappings from SIG -> hyper params are stored. With Hydra you can add
         ```yaml
         dora:
             dir: outputs
             shared: /shared_folder/shared_xps
         ```
-        Then other teammates can reference any SIG from an XP launched by other team members within the Dora commands. 
+        Then other teammates can reference any SIG from an XP launched by other team members within the Dora commands.
         
         
         ## Advanced configuration
         
         
         ### Setting SLURM default parameters
```

### Comparing `dora_search-0.1.8/dora_search.egg-info/SOURCES.txt` & `dora_search-0.1.9/dora_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dora_search-0.1.8/examples/mnist/grids/test.py` & `dora_search-0.1.9/examples/mnist/grids/test.py`

 * *Files identical despite different names*

### Comparing `dora_search-0.1.8/examples/mnist/train.py` & `dora_search-0.1.9/examples/mnist/train.py`

 * *Files identical despite different names*

### Comparing `dora_search-0.1.8/examples/mnist_hydra/grids/test.py` & `dora_search-0.1.9/examples/mnist_hydra/grids/test.py`

 * *Files identical despite different names*

### Comparing `dora_search-0.1.8/examples/mnist_hydra/train.py` & `dora_search-0.1.9/examples/mnist_hydra/train.py`

 * *Files identical despite different names*

### Comparing `dora_search-0.1.8/examples/pl/data.py` & `dora_search-0.1.9/examples/pl/data.py`

 * *Files identical despite different names*

### Comparing `dora_search-0.1.8/examples/pl/grids/test.py` & `dora_search-0.1.9/examples/pl/grids/test.py`

 * *Files identical despite different names*

### Comparing `dora_search-0.1.8/examples/pl/train.py` & `dora_search-0.1.9/examples/pl/train.py`

 * *Files identical despite different names*

### Comparing `dora_search-0.1.8/setup.py` & `dora_search-0.1.9/setup.py`

 * *Files identical despite different names*

