# Comparing `tmp/prospr-0.2a8.tar.gz` & `tmp/prospr-0.2a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prospr-0.2a8.tar", last modified: Mon Nov 14 14:11:13 2022, max compression
+gzip compressed data, was "prospr-0.2a9.tar", last modified: Mon Nov 14 17:29:55 2022, max compression
```

## Comparing `prospr-0.2a8.tar` & `prospr-0.2a9.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 14:11:13.276898 prospr-0.2a8/
--rw-r--r--   0 runner    (1001) docker     (121)     7652 2022-11-14 14:10:58.000000 prospr-0.2a8/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (121)     7652 2022-11-14 14:10:58.000000 prospr-0.2a8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3883 2022-11-14 14:11:13.276898 prospr-0.2a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3093 2022-11-14 14:10:58.000000 prospr-0.2a8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 14:11:13.268898 prospr-0.2a8/prospr/
--rw-r--r--   0 runner    (1001) docker     (121)      317 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 14:11:13.268898 prospr-0.2a8/prospr/core/
--rw-r--r--   0 runner    (1001) docker     (121)     4040 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/core/core_module.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 14:11:13.268898 prospr-0.2a8/prospr/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 14:11:13.272898 prospr-0.2a8/prospr/data/vanEck1000/
--rw-r--r--   0 runner    (1001) docker     (121)    14902 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck1000/HP10.csv
--rw-r--r--   0 runner    (1001) docker     (121)   104902 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck1000/HP100.csv
--rw-r--r--   0 runner    (1001) docker     (121)    19902 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck1000/HP15.csv
--rw-r--r--   0 runner    (1001) docker     (121)    24902 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck1000/HP20.csv
--rw-r--r--   0 runner    (1001) docker     (121)    29902 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck1000/HP25.csv
--rw-r--r--   0 runner    (1001) docker     (121)    34902 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck1000/HP30.csv
--rw-r--r--   0 runner    (1001) docker     (121)    39902 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck1000/HP35.csv
--rw-r--r--   0 runner    (1001) docker     (121)    44902 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck1000/HP40.csv
--rw-r--r--   0 runner    (1001) docker     (121)    49902 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck1000/HP45.csv
--rw-r--r--   0 runner    (1001) docker     (121)    54902 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck1000/HP50.csv
--rw-r--r--   0 runner    (1001) docker     (121)    59902 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck1000/HP55.csv
--rw-r--r--   0 runner    (1001) docker     (121)    64902 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck1000/HP60.csv
--rw-r--r--   0 runner    (1001) docker     (121)    69902 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck1000/HP65.csv
--rw-r--r--   0 runner    (1001) docker     (121)    74902 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck1000/HP70.csv
--rw-r--r--   0 runner    (1001) docker     (121)    79902 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck1000/HP75.csv
--rw-r--r--   0 runner    (1001) docker     (121)    84902 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck1000/HP80.csv
--rw-r--r--   0 runner    (1001) docker     (121)    89902 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck1000/HP85.csv
--rw-r--r--   0 runner    (1001) docker     (121)    94902 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck1000/HP90.csv
--rw-r--r--   0 runner    (1001) docker     (121)    99902 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck1000/HP95.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 14:11:13.276898 prospr-0.2a8/prospr/data/vanEck250/
--rw-r--r--   0 runner    (1001) docker     (121)     3652 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck250/HP10.csv
--rw-r--r--   0 runner    (1001) docker     (121)    26152 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck250/HP100.csv
--rw-r--r--   0 runner    (1001) docker     (121)     4902 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck250/HP15.csv
--rw-r--r--   0 runner    (1001) docker     (121)     6152 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck250/HP20.csv
--rw-r--r--   0 runner    (1001) docker     (121)     7402 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck250/HP25.csv
--rw-r--r--   0 runner    (1001) docker     (121)     8652 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck250/HP30.csv
--rw-r--r--   0 runner    (1001) docker     (121)     9902 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck250/HP35.csv
--rw-r--r--   0 runner    (1001) docker     (121)    11152 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck250/HP40.csv
--rw-r--r--   0 runner    (1001) docker     (121)    12402 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck250/HP45.csv
--rw-r--r--   0 runner    (1001) docker     (121)    13652 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck250/HP50.csv
--rw-r--r--   0 runner    (1001) docker     (121)    14902 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck250/HP55.csv
--rw-r--r--   0 runner    (1001) docker     (121)    16152 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck250/HP60.csv
--rw-r--r--   0 runner    (1001) docker     (121)    17402 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck250/HP65.csv
--rw-r--r--   0 runner    (1001) docker     (121)    18652 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck250/HP70.csv
--rw-r--r--   0 runner    (1001) docker     (121)    19902 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck250/HP75.csv
--rw-r--r--   0 runner    (1001) docker     (121)    21152 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck250/HP80.csv
--rw-r--r--   0 runner    (1001) docker     (121)    22402 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck250/HP85.csv
--rw-r--r--   0 runner    (1001) docker     (121)    23652 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck250/HP90.csv
--rw-r--r--   0 runner    (1001) docker     (121)    24902 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/data/vanEck250/HP95.csv
--rw-r--r--   0 runner    (1001) docker     (121)      861 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/datasets.py
--rw-r--r--   0 runner    (1001) docker     (121)     3274 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    10107 2022-11-14 14:10:58.000000 prospr-0.2a8/prospr/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 14:11:13.268898 prospr-0.2a8/prospr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3883 2022-11-14 14:11:13.000000 prospr-0.2a8/prospr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1537 2022-11-14 14:11:13.000000 prospr-0.2a8/prospr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 14:11:13.000000 prospr-0.2a8/prospr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 14:11:12.000000 prospr-0.2a8/prospr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-11-14 14:11:13.000000 prospr-0.2a8/prospr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-11-14 14:11:13.000000 prospr-0.2a8/prospr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-11-14 14:10:58.000000 prospr-0.2a8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-14 14:11:13.276898 prospr-0.2a8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2015 2022-11-14 14:10:58.000000 prospr-0.2a8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 17:29:55.483569 prospr-0.2a9/
+-rw-r--r--   0 runner    (1001) docker     (121)     7652 2022-11-14 17:29:39.000000 prospr-0.2a9/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (121)     7652 2022-11-14 17:29:39.000000 prospr-0.2a9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     3883 2022-11-14 17:29:55.479569 prospr-0.2a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3093 2022-11-14 17:29:39.000000 prospr-0.2a9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 17:29:55.471568 prospr-0.2a9/prospr/
+-rw-r--r--   0 runner    (1001) docker     (121)      317 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 17:29:55.471568 prospr-0.2a9/prospr/core/
+-rw-r--r--   0 runner    (1001) docker     (121)     4040 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/core/core_module.cpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 17:29:55.467568 prospr-0.2a9/prospr/data/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 17:29:55.475568 prospr-0.2a9/prospr/data/vanEck1000/
+-rw-r--r--   0 runner    (1001) docker     (121)    14902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP10.csv
+-rw-r--r--   0 runner    (1001) docker     (121)   104902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP100.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    19902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP15.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    24902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP20.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    29902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP25.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    34902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP30.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    39902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP35.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    44902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP40.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    49902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP45.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    54902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP50.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    59902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP55.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    64902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP60.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    69902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP65.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    74902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP70.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    79902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP75.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    84902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP80.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    89902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP85.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    94902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP90.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    99902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP95.csv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 17:29:55.479569 prospr-0.2a9/prospr/data/vanEck250/
+-rw-r--r--   0 runner    (1001) docker     (121)     3652 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP10.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    26152 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP100.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     4902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP15.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     6152 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP20.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     7402 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP25.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     8652 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP30.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     9902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP35.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    11152 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP40.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    12402 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP45.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    13652 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP50.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    14902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP55.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    16152 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP60.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    17402 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP65.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    18652 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP70.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    19902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP75.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    21152 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP80.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    22402 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP85.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    23652 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP90.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    24902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP95.csv
+-rw-r--r--   0 runner    (1001) docker     (121)      861 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3274 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10318 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 17:29:55.471568 prospr-0.2a9/prospr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3883 2022-11-14 17:29:55.000000 prospr-0.2a9/prospr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1537 2022-11-14 17:29:55.000000 prospr-0.2a9/prospr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 17:29:55.000000 prospr-0.2a9/prospr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 17:29:55.000000 prospr-0.2a9/prospr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-11-14 17:29:55.000000 prospr-0.2a9/prospr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2022-11-14 17:29:55.000000 prospr-0.2a9/prospr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2022-11-14 17:29:39.000000 prospr-0.2a9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-14 17:29:55.483569 prospr-0.2a9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2015 2022-11-14 17:29:39.000000 prospr-0.2a9/setup.py
```

### Comparing `prospr-0.2a8/COPYING.LESSER` & `prospr-0.2a9/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/LICENSE` & `prospr-0.2a9/LICENSE`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/PKG-INFO` & `prospr-0.2a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prospr
-Version: 0.2a8
+Version: 0.2a9
 Summary: A toolbox for protein folding with Python.
 Home-page: https://github.com/okkevaneck/prospr
 Author: okkevaneck
 License: LGPLv3
 Keywords: prospr protein structure prediction toolbox python c++ swig cmake extension heuristics pypi package
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `prospr-0.2a8/README.md` & `prospr-0.2a9/README.md`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/core/core_module.cpp` & `prospr-0.2a9/prospr/core/core_module.cpp`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck1000/HP10.csv` & `prospr-0.2a9/prospr/data/vanEck1000/HP10.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck1000/HP100.csv` & `prospr-0.2a9/prospr/data/vanEck1000/HP100.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck1000/HP15.csv` & `prospr-0.2a9/prospr/data/vanEck1000/HP15.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck1000/HP20.csv` & `prospr-0.2a9/prospr/data/vanEck1000/HP20.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck1000/HP25.csv` & `prospr-0.2a9/prospr/data/vanEck1000/HP25.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck1000/HP30.csv` & `prospr-0.2a9/prospr/data/vanEck1000/HP30.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck1000/HP35.csv` & `prospr-0.2a9/prospr/data/vanEck1000/HP35.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck1000/HP40.csv` & `prospr-0.2a9/prospr/data/vanEck1000/HP40.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck1000/HP45.csv` & `prospr-0.2a9/prospr/data/vanEck1000/HP45.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck1000/HP50.csv` & `prospr-0.2a9/prospr/data/vanEck1000/HP50.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck1000/HP55.csv` & `prospr-0.2a9/prospr/data/vanEck1000/HP55.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck1000/HP60.csv` & `prospr-0.2a9/prospr/data/vanEck1000/HP60.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck1000/HP65.csv` & `prospr-0.2a9/prospr/data/vanEck1000/HP65.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck1000/HP70.csv` & `prospr-0.2a9/prospr/data/vanEck1000/HP70.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck1000/HP75.csv` & `prospr-0.2a9/prospr/data/vanEck1000/HP75.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck1000/HP80.csv` & `prospr-0.2a9/prospr/data/vanEck1000/HP80.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck1000/HP85.csv` & `prospr-0.2a9/prospr/data/vanEck1000/HP85.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck1000/HP90.csv` & `prospr-0.2a9/prospr/data/vanEck1000/HP90.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck1000/HP95.csv` & `prospr-0.2a9/prospr/data/vanEck1000/HP95.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck250/HP10.csv` & `prospr-0.2a9/prospr/data/vanEck250/HP10.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck250/HP100.csv` & `prospr-0.2a9/prospr/data/vanEck250/HP100.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck250/HP15.csv` & `prospr-0.2a9/prospr/data/vanEck250/HP15.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck250/HP20.csv` & `prospr-0.2a9/prospr/data/vanEck250/HP20.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck250/HP25.csv` & `prospr-0.2a9/prospr/data/vanEck250/HP25.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck250/HP30.csv` & `prospr-0.2a9/prospr/data/vanEck250/HP30.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck250/HP35.csv` & `prospr-0.2a9/prospr/data/vanEck250/HP35.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck250/HP40.csv` & `prospr-0.2a9/prospr/data/vanEck250/HP40.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck250/HP45.csv` & `prospr-0.2a9/prospr/data/vanEck250/HP45.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck250/HP50.csv` & `prospr-0.2a9/prospr/data/vanEck250/HP50.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck250/HP55.csv` & `prospr-0.2a9/prospr/data/vanEck250/HP55.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck250/HP60.csv` & `prospr-0.2a9/prospr/data/vanEck250/HP60.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck250/HP65.csv` & `prospr-0.2a9/prospr/data/vanEck250/HP65.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck250/HP70.csv` & `prospr-0.2a9/prospr/data/vanEck250/HP70.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck250/HP75.csv` & `prospr-0.2a9/prospr/data/vanEck250/HP75.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck250/HP80.csv` & `prospr-0.2a9/prospr/data/vanEck250/HP80.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck250/HP85.csv` & `prospr-0.2a9/prospr/data/vanEck250/HP85.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck250/HP90.csv` & `prospr-0.2a9/prospr/data/vanEck250/HP90.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/data/vanEck250/HP95.csv` & `prospr-0.2a9/prospr/data/vanEck250/HP95.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/datasets.py` & `prospr-0.2a9/prospr/datasets.py`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/helpers.py` & `prospr-0.2a9/prospr/helpers.py`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/prospr/visualize.py` & `prospr-0.2a9/prospr/visualize.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,22 +263,30 @@
             lw=2,
         )
 
     # Remove axis, and position legend in the upper right with created space.
     ax.axis("off")
 
 
-def plot_protein(protein, style="basic", ax=None, legend=True, show=True):
+def plot_protein(
+    protein,
+    style="basic",
+    ax=None,
+    legend=True,
+    legend_style="inner",
+    show=True,
+):
     """
     Plot conformation of a protein.
-    :param Protein  protein:    Protein object to plot the hash of.
-    :param [str]    style:      What style to plot the proteins in.
-    :param Axes     ax:         Axis to plot Protein on.
-    :param bool     legend:     True if a legend needs to be added.
-    :param bool     show:       True if plot.show() needs to be called.
+    :param Protein  protein:        Protein object to plot the hash of.
+    :param [str]    style:          What style to plot the proteins in.
+    :param Axes     ax:             Axis to plot Protein on.
+    :param bool     legend:         True if a legend needs to be added.
+    :param str      legend_style:   Either 'inner' or 'outer'.
+    :param bool     show:           True if plot.show() needs to be called.
     """
     # Catch unplottable dimensions.
     if protein.dim != 2 and protein.dim != 3:
         raise RuntimeError(
             f"Cannot plot the structure of a protein with "
             f"dimension '{protein.dim}'"
         )
@@ -342,15 +350,17 @@
             label="Bond",
             lw=2,
         )
         handles.append(score_patch)
         labels.append(score_patch.get_label())
 
         # Style legend according to plotting style.
-        if style == "paper":
+        if (
+            style == "paper" and legend_style == "outer"
+        ) or legend_style == "outer":
             box = ax.get_position()
             ax.set_position([box.x0, box.y0, box.width * 0.7, box.height])
             ax.legend(
                 handles=handles,
                 labels=labels,
                 loc="upper left",
                 bbox_to_anchor=(1, 1),
```

### Comparing `prospr-0.2a8/prospr.egg-info/PKG-INFO` & `prospr-0.2a9/prospr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prospr
-Version: 0.2a8
+Version: 0.2a9
 Summary: A toolbox for protein folding with Python.
 Home-page: https://github.com/okkevaneck/prospr
 Author: okkevaneck
 License: LGPLv3
 Keywords: prospr protein structure prediction toolbox python c++ swig cmake extension heuristics pypi package
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `prospr-0.2a8/prospr.egg-info/SOURCES.txt` & `prospr-0.2a9/prospr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prospr-0.2a8/setup.py` & `prospr-0.2a9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
                 specifics.
 """
 
 import os
 from setuptools import setup
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 
-__version__ = "0.2a8"
+__version__ = "0.2a9"
 
 # Define core module extension.
 ext_modules = [
     Pybind11Extension(
         "prospr_core",
         ["prospr/core/core_module.cpp"],
         define_macros=[("VERSION_INFO", __version__)],
```

