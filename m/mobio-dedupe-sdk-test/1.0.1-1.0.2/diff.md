# Comparing `tmp/mobio-dedupe-sdk-test-1.0.1.tar.gz` & `tmp/mobio-dedupe-sdk-test-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobio-dedupe-sdk-test-1.0.1.tar", last modified: Mon May 15 10:29:11 2023, max compression
+gzip compressed data, was "mobio-dedupe-sdk-test-1.0.2.tar", last modified: Tue May 23 07:12:10 2023, max compression
```

## Comparing `mobio-dedupe-sdk-test-1.0.1.tar` & `mobio-dedupe-sdk-test-1.0.2.tar`

### file list

```diff
@@ -1,78 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:29:11.260314 mobio-dedupe-sdk-test-1.0.1/
--rw-r--r--   0 root         (0) root         (0)      871 2023-05-15 10:29:11.260314 mobio-dedupe-sdk-test-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 10:10:41.000000 mobio-dedupe-sdk-test-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:29:11.211312 mobio-dedupe-sdk-test-1.0.1/mobio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:29:11.217312 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:29:11.217312 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:29:11.218313 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/benchmarks/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:29:11.221313 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/benchmarks/benchmarks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/benchmarks/benchmarks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2558 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/benchmarks/benchmarks/canonical.py
--rw-r--r--   0 root         (0) root         (0)     2113 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/benchmarks/benchmarks/canonical_gazetteer.py
--rw-r--r--   0 root         (0) root         (0)     3035 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/benchmarks/benchmarks/canonical_matching.py
--rw-r--r--   0 root         (0) root         (0)     2093 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/benchmarks/benchmarks/common.py
--rw-r--r--   0 root         (0) root         (0)      190 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/benchmarks/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:29:11.236313 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/
--rw-r--r--   0 root         (0) root         (0)      154 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/__init__.py
--rw-r--r--   0 root         (0) root         (0)      355 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/_init.py
--rw-r--r--   0 root         (0) root         (0)     3995 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/_typing.py
--rw-r--r--   0 root         (0) root         (0)    55383 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/api.py
--rw-r--r--   0 root         (0) root         (0)      435 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/backport.py
--rw-r--r--   0 root         (0) root         (0)     7450 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/blocking.py
--rw-r--r--   0 root         (0) root         (0)     2485 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/canonical.py
--rw-r--r--   0 root         (0) root         (0)     2603 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/canopy_index.py
--rw-r--r--   0 root         (0) root         (0)    12921 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/clustering.py
--rw-r--r--   0 root         (0) root         (0)    11674 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/convenience.py
--rw-r--r--   0 root         (0) root         (0)     9296 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/core.py
--rw-r--r--   0 root         (0) root         (0)     8385 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/datamodel.py
--rw-r--r--   0 root         (0) root         (0)      746 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/index.py
--rw-r--r--   0 root         (0) root         (0)    15806 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/labeler.py
--rw-r--r--   0 root         (0) root         (0)     1249 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/levenshtein.py
--rw-r--r--   0 root         (0) root         (0)     6898 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/predicate_functions.py
--rw-r--r--   0 root         (0) root         (0)    10952 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/predicates.py
--rw-r--r--   0 root         (0) root         (0)     2463 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/serializer.py
--rw-r--r--   0 root         (0) root         (0)     1141 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/tfidf.py
--rw-r--r--   0 root         (0) root         (0)    14462 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/training.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:29:11.244313 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/variables/
--rw-r--r--   0 root         (0) root         (0)       76 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/variables/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3858 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/variables/base.py
--rw-r--r--   0 root         (0) root         (0)     1249 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/variables/categorical_type.py
--rw-r--r--   0 root         (0) root         (0)      368 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/variables/exact.py
--rw-r--r--   0 root         (0) root         (0)     1280 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/variables/exists.py
--rw-r--r--   0 root         (0) root         (0)     2693 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/variables/interaction.py
--rw-r--r--   0 root         (0) root         (0)      414 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/variables/latlong.py
--rw-r--r--   0 root         (0) root         (0)      598 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/variables/price.py
--rw-r--r--   0 root         (0) root         (0)     1014 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/variables/set.py
--rw-r--r--   0 root         (0) root         (0)     3241 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/variables/string.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:29:11.244313 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/docs/
--rw-r--r--   0 root         (0) root         (0)     8895 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/docs/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:29:11.246313 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/pgsql_example/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/pgsql_example/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    14565 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/pgsql_example/pgsql_big_dedupe_example.py
--rw-r--r--   0 root         (0) root         (0)      378 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:29:11.255313 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/tests/
--rw-r--r--   0 root         (0) root         (0)     1156 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/tests/duplicateCluster_memory_case.py
--rw-r--r--   0 root         (0) root         (0)     3708 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/tests/test_api.py
--rw-r--r--   0 root         (0) root         (0)     4893 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/tests/test_blocking.py
--rw-r--r--   0 root         (0) root         (0)     2295 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/tests/test_canonical.py
--rw-r--r--   0 root         (0) root         (0)     5403 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/tests/test_core.py
--rw-r--r--   0 root         (0) root         (0)     4740 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/tests/test_cpredicates.py
--rw-r--r--   0 root         (0) root         (0)     7607 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/tests/test_dedupe.py
--rw-r--r--   0 root         (0) root         (0)     2336 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/tests/test_labeler.py
--rw-r--r--   0 root         (0) root         (0)    13832 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/tests/test_predicate_functions.py
--rw-r--r--   0 root         (0) root         (0)     4932 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/tests/test_predicates.py
--rw-r--r--   0 root         (0) root         (0)      227 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/tests/test_price.py
--rw-r--r--   0 root         (0) root         (0)     1833 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/tests/test_serializer.py
--rw-r--r--   0 root         (0) root         (0)      888 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/tests/test_tfidf.py
--rw-r--r--   0 root         (0) root         (0)     3353 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/tests/test_training.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:29:11.259314 mobio-dedupe-sdk-test-1.0.1/mobio_dedupe_sdk_test.egg-info/
--rw-r--r--   0 root         (0) root         (0)      871 2023-05-15 10:29:11.000000 mobio-dedupe-sdk-test-1.0.1/mobio_dedupe_sdk_test.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2614 2023-05-15 10:29:11.000000 mobio-dedupe-sdk-test-1.0.1/mobio_dedupe_sdk_test.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 10:29:11.000000 mobio-dedupe-sdk-test-1.0.1/mobio_dedupe_sdk_test.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-15 10:29:11.000000 mobio-dedupe-sdk-test-1.0.1/mobio_dedupe_sdk_test.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)      688 2023-05-15 10:29:11.000000 mobio-dedupe-sdk-test-1.0.1/mobio_dedupe_sdk_test.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-15 10:29:11.000000 mobio-dedupe-sdk-test-1.0.1/mobio_dedupe_sdk_test.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-05-15 10:10:41.000000 mobio-dedupe-sdk-test-1.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 10:29:11.260314 mobio-dedupe-sdk-test-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)    10247 2023-05-15 10:29:10.000000 mobio-dedupe-sdk-test-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:12:10.067006 mobio-dedupe-sdk-test-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)      871 2023-05-23 07:12:10.066006 mobio-dedupe-sdk-test-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 10:10:41.000000 mobio-dedupe-sdk-test-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:12:10.017005 mobio-dedupe-sdk-test-1.0.2/mobio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:12:10.021005 mobio-dedupe-sdk-test-1.0.2/mobio/sdks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 10:01:09.000000 mobio-dedupe-sdk-test-1.0.2/mobio/sdks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:12:10.047006 mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/
+-rw-r--r--   0 root         (0) root         (0)      148 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      388 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/_init.py
+-rw-r--r--   0 root         (0) root         (0)     3995 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/_typing.py
+-rw-r--r--   0 root         (0) root         (0)    55436 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/api.py
+-rw-r--r--   0 root         (0) root         (0)      435 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/backport.py
+-rw-r--r--   0 root         (0) root         (0)    11058 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/blocking.py
+-rw-r--r--   0 root         (0) root         (0)     2496 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/canonical.py
+-rw-r--r--   0 root         (0) root         (0)     2603 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/canopy_index.py
+-rw-r--r--   0 root         (0) root         (0)    12932 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/clustering.py
+-rw-r--r--   0 root         (0) root         (0)    11718 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/convenience.py
+-rw-r--r--   0 root         (0) root         (0)     9307 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/core.py
+-rw-r--r--   0 root         (0) root         (0)     8410 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/datamodel.py
+-rw-r--r--   0 root         (0) root         (0)      746 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/index.py
+-rw-r--r--   0 root         (0) root         (0)    15883 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/labeler.py
+-rw-r--r--   0 root         (0) root         (0)     1249 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/levenshtein.py
+-rw-r--r--   0 root         (0) root         (0)     6898 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/predicate_functions.py
+-rw-r--r--   0 root         (0) root         (0)    11150 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/predicates.py
+-rw-r--r--   0 root         (0) root         (0)     2474 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/serializer.py
+-rw-r--r--   0 root         (0) root         (0)     1174 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/tfidf.py
+-rw-r--r--   0 root         (0) root         (0)    14462 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/training.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:12:10.060006 mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/variables/
+-rw-r--r--   0 root         (0) root         (0)       76 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/variables/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3880 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/variables/base.py
+-rw-r--r--   0 root         (0) root         (0)     1282 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/variables/categorical_type.py
+-rw-r--r--   0 root         (0) root         (0)      390 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/variables/exact.py
+-rw-r--r--   0 root         (0) root         (0)     1313 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/variables/exists.py
+-rw-r--r--   0 root         (0) root         (0)     2726 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/variables/interaction.py
+-rw-r--r--   0 root         (0) root         (0)      436 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/variables/latlong.py
+-rw-r--r--   0 root         (0) root         (0)      620 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/variables/price.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/variables/set.py
+-rw-r--r--   0 root         (0) root         (0)     3274 2023-05-23 07:08:56.000000 mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/variables/string.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:12:10.065006 mobio-dedupe-sdk-test-1.0.2/mobio_dedupe_sdk_test.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      871 2023-05-23 07:12:09.000000 mobio-dedupe-sdk-test-1.0.2/mobio_dedupe_sdk_test.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1334 2023-05-23 07:12:09.000000 mobio-dedupe-sdk-test-1.0.2/mobio_dedupe_sdk_test.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 07:12:09.000000 mobio-dedupe-sdk-test-1.0.2/mobio_dedupe_sdk_test.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-23 07:12:09.000000 mobio-dedupe-sdk-test-1.0.2/mobio_dedupe_sdk_test.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)      688 2023-05-23 07:12:09.000000 mobio-dedupe-sdk-test-1.0.2/mobio_dedupe_sdk_test.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-23 07:12:09.000000 mobio-dedupe-sdk-test-1.0.2/mobio_dedupe_sdk_test.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-05-15 10:10:41.000000 mobio-dedupe-sdk-test-1.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 07:12:10.067006 mobio-dedupe-sdk-test-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)    10247 2023-05-23 07:12:08.000000 mobio-dedupe-sdk-test-1.0.2/setup.py
```

### Comparing `mobio-dedupe-sdk-test-1.0.1/PKG-INFO` & `mobio-dedupe-sdk-test-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobio-dedupe-sdk-test
-Version: 1.0.1
+Version: 1.0.2
 Summary: Mobio dedupe SDK
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Description: UNKNOWN
```

### Comparing `mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/_typing.py` & `mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/_typing.py`

 * *Files identical despite different names*

### Comparing `mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/api.py` & `mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,37 +16,37 @@
 import warnings
 from typing import TYPE_CHECKING, cast, overload
 
 import numpy
 import sklearn.linear_model
 import sklearn.model_selection
 
-import dedupe.blocking as blocking
-import dedupe.clustering as clustering
-import dedupe.core as core
-import dedupe.datamodel as datamodel
-import dedupe.labeler as labeler
-import dedupe.predicates
-import dedupe.serializer as serializer
-from dedupe._typing import Literal
+import mobio.sdks.dedupe.blocking as blocking
+import mobio.sdks.dedupe.clustering as clustering
+import mobio.sdks.dedupe.core as core
+import mobio.sdks.dedupe.datamodel as datamodel
+import mobio.sdks.dedupe.labeler as labeler
+import mobio.sdks.dedupe.predicates
+import mobio.sdks.dedupe.serializer as serializer
+from mobio.sdks.dedupe._typing import Literal
 
 if TYPE_CHECKING:
     from typing import (
         BinaryIO,
         Collection,
         Generator,
         Iterable,
         MutableMapping,
         TextIO,
         Union,
     )
 
     import numpy.typing
 
-    from dedupe._typing import (
+    from _typing import (
         ArrayLinks,
         Blocks,
         BlocksInt,
         BlocksStr,
         Classifier,
         Clusters,
         ClustersInt,
@@ -58,17 +58,17 @@
         LabelsLike,
         Links,
         LookupResultsInt,
         LookupResultsStr,
         PathLike,
         RecordDict,
     )
-    from dedupe._typing import RecordDictPair as TrainingExample
-    from dedupe._typing import RecordDictPairs as TrainingExamples
-    from dedupe._typing import (
+    from _typing import RecordDictPair as TrainingExample
+    from _typing import RecordDictPairs as TrainingExamples
+    from _typing import (
         RecordID,
         RecordPairs,
         Scores,
         TrainingData,
         TupleLinks,
         VariableDefinition,
     )
@@ -89,15 +89,15 @@
         else:
             self.num_cores = num_cores
 
         self.in_memory = in_memory
         self._fingerprinter: blocking.Fingerprinter | None = None
         self.data_model: datamodel.DataModel
         self.classifier: Classifier
-        self.predicates: Collection[dedupe.predicates.Predicate]
+        self.predicates: Collection[predicates.Predicate]
 
     @property
     def fingerprinter(self) -> blocking.Fingerprinter:
         if self._fingerprinter is None:
             raise ValueError(
                 "the record fingerprinter is not intialized, "
                 "please run the train method"
```

### Comparing `mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/canonical.py` & `mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/canonical.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Mapping, Sequence
 
 import numpy
 import numpy.typing
 from affinegap import normalizedAffineGapDistance as affine
 
-from dedupe._typing import Comparator, RecordDict
+from mobio.sdks.dedupe._typing import Comparator, RecordDict
 
 
 def getCentroid(attribute_variants: Sequence[str], comparator: Comparator) -> str:
     """
     Takes in a list of attribute values for a field,
     evaluates the centroid using the comparator,
     & returns the centroid (i.e. the 'best' value for the field)
```

### Comparing `mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/canopy_index.py` & `mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/canopy_index.py`

 * *Files identical despite different names*

### Comparing `mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/clustering.py` & `mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/clustering.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from collections import defaultdict
 from typing import Generator, Iterable, Sequence, cast
 
 import numpy
 import numpy.typing
 import scipy.cluster.hierarchy
 
-from dedupe._typing import ArrayLinks, Clusters, RecordID, Scores, TupleLinks
+from mobio.sdks.dedupe._typing import ArrayLinks, Clusters, RecordID, Scores, TupleLinks
 
 logger = logging.getLogger(__name__)
 
 
 def connected_components(
     edgelist: Scores, max_components: int
 ) -> Generator[Scores, None, None]:
```

### Comparing `mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/convenience.py` & `mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/convenience.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 import random
 import sys
 import warnings
 from typing import Iterator, Tuple, overload
 
 import numpy
 
-import dedupe
-from dedupe._typing import (
+import mobio.sdks.dedupe
+from mobio.sdks.dedupe._typing import (
     DataInt,
     DataStr,
     Literal,
     RecordDict,
     RecordDictPair,
     RecordID,
     TrainingData,
 )
-from dedupe.canonical import getCanonicalRep
-from dedupe.core import unique
+from mobio.sdks.dedupe.canonical import getCanonicalRep
+from mobio.sdks.dedupe.core import unique
 
 IndicesIterator = Iterator[Tuple[int, int]]
 
 
 def randomPairs(n_records: int, sample_size: int) -> IndicesIterator:
     """
     Return random combinations of indices for a square matrix of size n
```

### Comparing `mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/core.py` & `mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import os
 import queue
 import tempfile
 from typing import TYPE_CHECKING, overload
 
 import numpy
 
-from dedupe.backport import RLock
+from mobio.sdks.dedupe.backport import RLock
 
 if TYPE_CHECKING:
     from typing import (
         Any,
         Generator,
         Iterable,
         Iterator,
```

### Comparing `mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/datamodel.py` & `mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/datamodel.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,34 +3,35 @@
 import copyreg
 import pkgutil
 import types
 from typing import TYPE_CHECKING, cast
 
 import numpy
 
-import dedupe.variables
-from dedupe.variables.base import FieldType as FieldVariable
-from dedupe.variables.base import MissingDataType, Variable
-from dedupe.variables.interaction import InteractionType
+# import variables
+from .variables.base import FieldType as FieldVariable
+from .variables.base import MissingDataType, Variable
+from .variables.interaction import InteractionType
+from .variables import __path__
 
 for _, module, _ in pkgutil.iter_modules(  # type: ignore
-    dedupe.variables.__path__, "dedupe.variables."
+    __path__, "mobio.sdks.dedupe.variables."
 ):
     __import__(module)
 
 if TYPE_CHECKING:
     from typing import Generator, Iterable, Sequence
 
-    from dedupe._typing import (
+    from mobio.sdks.dedupe._typing import (
         Comparator,
         RecordDict,
         RecordDictPair,
         VariableDefinition,
     )
-    from dedupe.predicates import Predicate
+    from mobio.sdks.dedupe.predicates import Predicate
 
 VARIABLE_CLASSES = {k: v for k, v in FieldVariable.all_subclasses() if k}
 
 
 class DataModel(object):
     version = 1
```

### Comparing `mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/index.py` & `mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/index.py`

 * *Files identical despite different names*

### Comparing `mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/labeler.py` & `mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/labeler.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,32 +6,32 @@
 from typing import TYPE_CHECKING, overload
 from warnings import warn
 
 import numpy
 import numpy.typing
 import sklearn.linear_model
 
-import dedupe.core as core
-import dedupe.training as training
+import mobio.sdks.dedupe.core as core
+import mobio.sdks.dedupe.training as training
 
 if TYPE_CHECKING:
     from typing import Dict, Iterable, Literal, Mapping
 
-    from dedupe._typing import (
+    from mobio.sdks.dedupe._typing import (
         Data,
         DataInt,
         DataStr,
         FeaturizerFunction,
         Labels,
         LabelsLike,
     )
-    from dedupe._typing import RecordDictPair as TrainingExample
-    from dedupe._typing import RecordDictPairs as TrainingExamples
-    from dedupe._typing import RecordIDPair
-    from dedupe.predicates import Predicate
+    from mobio.sdks.dedupe._typing import RecordDictPair as TrainingExample
+    from mobio.sdks.dedupe._typing import RecordDictPairs as TrainingExamples
+    from mobio.sdks.dedupe._typing import RecordIDPair
+    from mobio.sdks.dedupe.predicates import Predicate
 
 
 logger = logging.getLogger(__name__)
 
 
 class HasCandidates:
     """Has a list of pairs that we could ask the user to label."""
```

### Comparing `mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/levenshtein.py` & `mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/levenshtein.py`

 * *Files identical despite different names*

### Comparing `mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/predicate_functions.py` & `mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/predicate_functions.py`

 * *Files identical despite different names*

### Comparing `mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/predicates.py` & `mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/predicates.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 
 import abc
 import re
 import string
 from itertools import product
 from typing import TYPE_CHECKING
 
-import dedupe.levenshtein as levenshtein
-import dedupe.tfidf as tfidf
-from dedupe.cpredicates import ngrams
+import mobio.sdks.dedupe.levenshtein as levenshtein
+import mobio.sdks.dedupe.tfidf as tfidf
+from mobio.sdks.dedupe.cpredicates import ngrams
 
 # This allows to import predicate functions from this module
 # and ensure backward compatibility.
-from dedupe.predicate_functions import *  # noqa: F401, F403
+from mobio.sdks.dedupe.predicate_functions import *  # noqa: F401, F403
 
 if TYPE_CHECKING:
     from typing import AbstractSet, Any, FrozenSet, Iterable, Mapping, Sequence
 
-    from dedupe._typing import Literal, PredicateFunction, RecordDict
-    from dedupe.index import Index
+    from mobio.sdks.dedupe._typing import Literal, PredicateFunction, RecordDict
+    from mobio.sdks.dedupe.index import Index
 
 
 words = re.compile(r"[\w']+").findall
 
 PUNCTABLE = str.maketrans("", "", string.punctuation)
 
 
@@ -82,14 +82,16 @@
 class SimplePredicate(Predicate):
     type = "SimplePredicate"
 
     def __init__(self, func: PredicateFunction, field: str):
         self.func = func
         self.__name__ = "(%s, %s)" % (func.__name__, field)
         self.field = field
+        self.is_array = False
+        self.is_approximate = False
 
     def __call__(self, record: RecordDict, **kwargs) -> FrozenSet[str]:
         column = record[self.field]
         if column:
             return self.func(column)
         else:
             return frozenset()
@@ -130,14 +132,16 @@
     _cache: dict[Any, FrozenSet[str]]
 
     def __init__(self, threshold: float, field: str):
         self.__name__ = "(%s, %s)" % (threshold, field)
         self.field = field
         self.threshold = threshold
         self.index = None
+        self.is_array = False
+        self.is_approximate = False
 
     def __getstate__(self) -> dict[str, Any]:
         odict = self.__dict__.copy()
         odict["index"] = None
         odict["_cache"] = {}
         if "canopy" in odict:
             odict["canopy"] = {}
```

### Comparing `mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/serializer.py` & `mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 from typing import Any, Iterator, TextIO
 
-from dedupe._typing import TrainingData
+from mobio.sdks.dedupe._typing import TrainingData
 
 
 def _from_json(json_object: Any) -> Any:
     if "__class__" in json_object:
         if json_object["__class__"] == "frozenset":
             return frozenset(json_object["__value__"])
         if json_object["__class__"] == "tuple":
```

### Comparing `mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/tfidf.py` & `mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/tfidf.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 import logging
 from typing import List, Tuple
 
-from dedupe.canopy_index import CanopyIndex
-from dedupe.core import Enumerator
-from dedupe.index import Index
+from mobio.sdks.dedupe.canopy_index import CanopyIndex
+from mobio.sdks.dedupe.core import Enumerator
+from mobio.sdks.dedupe.index import Index
 
 logger = logging.getLogger(__name__)
 
 Doc = Tuple[str, ...]
 
 
 class TfIdfIndex(Index):
```

### Comparing `mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/training.py` & `mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/training.py`

 * *Files identical despite different names*

### Comparing `mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/variables/base.py` & `mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/variables/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-from dedupe import predicates
+from mobio.sdks.dedupe import predicates
 
 if TYPE_CHECKING:
     from typing import Any, ClassVar, Generator, Iterable, Optional, Sequence, Type
 
-    from dedupe._typing import Comparator, PredicateFunction, VariableDefinition
+    from mobio.sdks.dedupe._typing import Comparator, PredicateFunction, VariableDefinition
 
 
 class Variable(object):
     name: str
     type: ClassVar[str]
     predicates: list[predicates.Predicate]
     higher_vars: Sequence["Variable"]
```

### Comparing `mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/variables/categorical_type.py` & `mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/variables/categorical_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from categorical import CategoricalComparator
 
-from dedupe import predicates
-from dedupe._typing import PredicateFunction, VariableDefinition
-from dedupe.variables.base import DerivedType, FieldType
+from mobio.sdks.dedupe import predicates
+from mobio.sdks.dedupe._typing import PredicateFunction, VariableDefinition
+from mobio.sdks.dedupe.variables.base import DerivedType, FieldType
 
 
 class CategoricalType(FieldType):
     type = "Categorical"
     _predicate_functions: list[PredicateFunction] = [predicates.wholeFieldPredicate]
 
     def _categories(self, definition: VariableDefinition) -> list[str]:
```

### Comparing `mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/variables/exists.py` & `mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/variables/exists.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 from typing import Any
 
 from categorical import CategoricalComparator
 
-from dedupe._typing import PredicateFunction, VariableDefinition
-from dedupe.variables.base import DerivedType
-from dedupe.variables.categorical_type import CategoricalType
+from mobio.sdks.dedupe._typing import PredicateFunction, VariableDefinition
+from mobio.sdks.dedupe.variables.base import DerivedType
+from mobio.sdks.dedupe.variables.categorical_type import CategoricalType
 
 
 class ExistsType(CategoricalType):
     type = "Exists"
     _predicate_functions: list[PredicateFunction] = []
 
     def __init__(self, definition: VariableDefinition):
```

### Comparing `mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/variables/interaction.py` & `mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/variables/interaction.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import itertools
 from typing import Mapping
 
-from dedupe._typing import VariableDefinition
-from dedupe.variables.base import FieldType as FieldVariable
-from dedupe.variables.base import Variable
+from mobio.sdks.dedupe._typing import VariableDefinition
+from mobio.sdks.dedupe.variables.base import FieldType as FieldVariable
+from mobio.sdks.dedupe.variables.base import Variable
 
 
 class InteractionType(Variable):
     type = "Interaction"
     higher_vars: list["InteractionType"]
 
     def __init__(self, definition: VariableDefinition):
```

### Comparing `mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/variables/price.py` & `mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/variables/price.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import numpy
 
-from dedupe import predicates
-from dedupe.variables.base import FieldType
+from mobio.sdks.dedupe import predicates
+from mobio.sdks.dedupe.variables.base import FieldType
 
 
 class PriceType(FieldType):
     _predicate_functions = [
         predicates.orderOfMagnitude,
         predicates.wholeFieldPredicate,
         predicates.roundTo1,
```

### Comparing `mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/variables/set.py` & `mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/variables/set.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from simplecosine.cosine import CosineSetSimilarity
 
-from dedupe import predicates
-from dedupe._typing import VariableDefinition
-from dedupe.variables.base import FieldType
+from mobio.sdks.dedupe import predicates
+from mobio.sdks.dedupe._typing import VariableDefinition
+from mobio.sdks.dedupe.variables.base import FieldType
 
 
 class SetType(FieldType):
     type = "Set"
 
     _predicate_functions = (
         predicates.wholeSetPredicate,
```

### Comparing `mobio-dedupe-sdk-test-1.0.1/mobio/sdks/dedupe/dedupe/variables/string.py` & `mobio-dedupe-sdk-test-1.0.2/mobio/sdks/dedupe/variables/string.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Sequence, Type
 
 from affinegap import normalizedAffineGapDistance as affineGap
 from highered import CRFEditDistance
 from simplecosine.cosine import CosineTextSimilarity
 
-from dedupe import predicates
-from dedupe._typing import PredicateFunction, VariableDefinition
-from dedupe.variables.base import FieldType, indexPredicates
+from mobio.sdks.dedupe import predicates
+from mobio.sdks.dedupe._typing import PredicateFunction, VariableDefinition
+from mobio.sdks.dedupe.variables.base import FieldType, indexPredicates
 
 crfEd = CRFEditDistance()
 
 base_predicates = (
     predicates.wholeFieldPredicate,
     predicates.firstTokenPredicate,
     predicates.firstTwoTokensPredicate,
```

### Comparing `mobio-dedupe-sdk-test-1.0.1/mobio_dedupe_sdk_test.egg-info/PKG-INFO` & `mobio-dedupe-sdk-test-1.0.2/mobio_dedupe_sdk_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobio-dedupe-sdk-test
-Version: 1.0.1
+Version: 1.0.2
 Summary: Mobio dedupe SDK
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Description: UNKNOWN
```

### Comparing `mobio-dedupe-sdk-test-1.0.1/mobio_dedupe_sdk_test.egg-info/requires.txt` & `mobio-dedupe-sdk-test-1.0.2/mobio_dedupe_sdk_test.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mobio-dedupe-sdk-test-1.0.1/setup.py` & `mobio-dedupe-sdk-test-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                         'pycodestyle==2.9.1', 'pycparser==2.21', 'pyflakes==2.5.0', 'pyhacrf-datamade==0.2.6',
                         'PyLBFGS==0.2.0.14', 'python-dateutil==2.8.2', 'scikit-learn==1.2.2', 'scipy==1.10.1',
                         'simplecosine==1.2', 'six==1.16.0', 'threadpoolctl==3.1.0', 'toml==0.10.2',
                         'typing_extensions==4.5.0', 'zope.index==6.0', 'zope.interface==6.0']
         return requirements
 
 
-version_dev='1.0.1'  # Giữ nguyên định dạng không được format file có khoảng trống theo Pycharm (version_dev = '1.0.9' là file run.sh sẽ không bắt được current_version)
+version_dev='1.0.2'  # Giữ nguyên định dạng không được format file có khoảng trống theo Pycharm (version_dev = '1.0.9' là file run.sh sẽ không bắt được current_version)
 version_prod='1.0.0'  # Giữ nguyên định dạng không được format file có khoảng trống theo Pycharm (version_dev = '1.0.9' là file run.sh sẽ không bắt được current_version)
 
 run_mode='-test'
 
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
@@ -57,15 +57,15 @@
     name="mobio-dedupe-sdk" + run_mode,  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.0.1',  # Required, Phần này cũng không được format file.
+    version='1.0.2',  # Required, Phần này cũng không được format file.
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Mobio dedupe SDK",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

