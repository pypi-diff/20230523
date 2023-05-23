# Comparing `tmp/careless-0.2.9.tar.gz` & `tmp/careless-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "careless-0.2.9.tar", last modified: Thu Mar 30 13:44:11 2023, max compression
+gzip compressed data, was "careless-0.3.0.tar", last modified: Tue May 23 21:55:50 2023, max compression
```

## Comparing `careless-0.2.9.tar` & `careless-0.3.0.tar`

### file list

```diff
@@ -1,84 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:44:11.156362 careless-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-03-30 13:43:58.000000 careless-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-30 13:43:58.000000 careless-0.2.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-03-30 13:44:11.156362 careless-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-03-30 13:43:58.000000 careless-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:44:11.148362 careless-0.2.9/careless/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-30 13:43:58.000000 careless-0.2.9/careless/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-30 13:43:58.000000 careless-0.2.9/careless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:44:11.152362 careless-0.2.9/careless/args/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-03-30 13:43:58.000000 careless-0.2.9/careless/args/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-03-30 13:43:58.000000 careless-0.2.9/careless/args/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-03-30 13:43:58.000000 careless-0.2.9/careless/args/crossvalidation.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-30 13:43:58.000000 careless-0.2.9/careless/args/filtration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-03-30 13:43:58.000000 careless-0.2.9/careless/args/interpretation.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-03-30 13:43:58.000000 careless-0.2.9/careless/args/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-03-30 13:43:58.000000 careless-0.2.9/careless/args/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-03-30 13:43:58.000000 careless-0.2.9/careless/args/poly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-03-30 13:43:58.000000 careless-0.2.9/careless/args/positional_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-03-30 13:43:58.000000 careless-0.2.9/careless/args/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-03-30 13:43:58.000000 careless-0.2.9/careless/args/required.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-03-30 13:43:58.000000 careless-0.2.9/careless/args/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-03-30 13:43:58.000000 careless-0.2.9/careless/args/tf_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:44:11.152362 careless-0.2.9/careless/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 13:43:58.000000 careless-0.2.9/careless/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-30 13:43:58.000000 careless-0.2.9/careless/callbacks/progress_bar.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4766 2023-03-30 13:43:58.000000 careless-0.2.9/careless/careless.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:44:11.156362 careless-0.2.9/careless/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 13:43:58.000000 careless-0.2.9/careless/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-03-30 13:43:58.000000 careless-0.2.9/careless/io/asu.py
--rw-r--r--   0 runner    (1001) docker     (123)    22392 2023-03-30 13:43:58.000000 careless-0.2.9/careless/io/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16251 2023-03-30 13:43:58.000000 careless-0.2.9/careless/io/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:44:11.156362 careless-0.2.9/careless/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 13:43:58.000000 careless-0.2.9/careless/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-03-30 13:43:58.000000 careless-0.2.9/careless/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:44:11.156362 careless-0.2.9/careless/models/likelihoods/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 13:43:58.000000 careless-0.2.9/careless/models/likelihoods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-30 13:43:58.000000 careless-0.2.9/careless/models/likelihoods/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-03-30 13:43:58.000000 careless-0.2.9/careless/models/likelihoods/laue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-03-30 13:43:58.000000 careless-0.2.9/careless/models/likelihoods/mono.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:44:11.156362 careless-0.2.9/careless/models/merging/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-30 13:43:58.000000 careless-0.2.9/careless/models/merging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-03-30 13:43:58.000000 careless-0.2.9/careless/models/merging/surrogate_posteriors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-03-30 13:43:58.000000 careless-0.2.9/careless/models/merging/variational.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:44:11.156362 careless-0.2.9/careless/models/priors/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-30 13:43:58.000000 careless-0.2.9/careless/models/priors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-30 13:43:58.000000 careless-0.2.9/careless/models/priors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-03-30 13:43:58.000000 careless-0.2.9/careless/models/priors/empirical.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-03-30 13:43:58.000000 careless-0.2.9/careless/models/priors/wilson.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:44:11.156362 careless-0.2.9/careless/models/scaling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 13:43:58.000000 careless-0.2.9/careless/models/scaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-30 13:43:58.000000 careless-0.2.9/careless/models/scaling/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-03-30 13:43:58.000000 careless-0.2.9/careless/models/scaling/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-03-30 13:43:58.000000 careless-0.2.9/careless/models/scaling/nn.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4389 2023-03-30 13:43:58.000000 careless-0.2.9/careless/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:44:11.156362 careless-0.2.9/careless/stats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 13:43:58.000000 careless-0.2.9/careless/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-03-30 13:43:58.000000 careless-0.2.9/careless/stats/ccanom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-03-30 13:43:58.000000 careless-0.2.9/careless/stats/cchalf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-03-30 13:43:58.000000 careless-0.2.9/careless/stats/ccpred.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-03-30 13:43:58.000000 careless-0.2.9/careless/stats/completeness.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-03-30 13:43:58.000000 careless-0.2.9/careless/stats/rsplit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:44:11.156362 careless-0.2.9/careless/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 13:43:58.000000 careless-0.2.9/careless/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-03-30 13:43:58.000000 careless-0.2.9/careless/utils/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-03-30 13:43:58.000000 careless-0.2.9/careless/utils/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-03-30 13:43:58.000000 careless-0.2.9/careless/utils/laue.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-03-30 13:43:58.000000 careless-0.2.9/careless/utils/positional_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-30 13:43:58.000000 careless-0.2.9/careless/utils/shame.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:44:11.148362 careless-0.2.9/careless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-03-30 13:44:11.000000 careless-0.2.9/careless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-03-30 13:44:11.000000 careless-0.2.9/careless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 13:44:11.000000 careless-0.2.9/careless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-30 13:44:11.000000 careless-0.2.9/careless.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-30 13:44:11.000000 careless-0.2.9/careless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-30 13:44:11.000000 careless-0.2.9/careless.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:44:11.156362 careless-0.2.9/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3872 2023-03-30 13:43:58.000000 careless-0.2.9/scripts/make_difference_map
--rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-03-30 13:43:58.000000 careless-0.2.9/scripts/stream2mtz
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-30 13:44:11.156362 careless-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-03-30 13:43:58.000000 careless-0.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 13:44:11.156362 careless-0.2.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 13:43:58.000000 careless-0.2.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-03-30 13:43:58.000000 careless-0.2.9/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-03-30 13:43:58.000000 careless-0.2.9/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:50.126896 careless-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-23 21:55:39.000000 careless-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-23 21:55:39.000000 careless-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-23 21:55:50.126896 careless-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-05-23 21:55:39.000000 careless-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:50.110895 careless-0.3.0/careless/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 21:55:39.000000 careless-0.3.0/careless/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-23 21:55:39.000000 careless-0.3.0/careless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:50.114896 careless-0.3.0/careless/args/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-23 21:55:39.000000 careless-0.3.0/careless/args/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-23 21:55:39.000000 careless-0.3.0/careless/args/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-23 21:55:39.000000 careless-0.3.0/careless/args/crossvalidation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-23 21:55:39.000000 careless-0.3.0/careless/args/filtration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-23 21:55:39.000000 careless-0.3.0/careless/args/interpretation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-23 21:55:39.000000 careless-0.3.0/careless/args/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-23 21:55:39.000000 careless-0.3.0/careless/args/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-23 21:55:39.000000 careless-0.3.0/careless/args/poly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-23 21:55:39.000000 careless-0.3.0/careless/args/positional_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-05-23 21:55:39.000000 careless-0.3.0/careless/args/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-23 21:55:39.000000 careless-0.3.0/careless/args/required.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-23 21:55:39.000000 careless-0.3.0/careless/args/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-23 21:55:39.000000 careless-0.3.0/careless/args/tf_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:50.118896 careless-0.3.0/careless/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:39.000000 careless-0.3.0/careless/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-23 21:55:39.000000 careless-0.3.0/careless/callbacks/progress_bar.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4879 2023-05-23 21:55:39.000000 careless-0.3.0/careless/careless.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:50.118896 careless-0.3.0/careless/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:39.000000 careless-0.3.0/careless/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-05-23 21:55:39.000000 careless-0.3.0/careless/io/asu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22392 2023-05-23 21:55:39.000000 careless-0.3.0/careless/io/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16476 2023-05-23 21:55:39.000000 careless-0.3.0/careless/io/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-23 21:55:39.000000 careless-0.3.0/careless/io/xds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:50.118896 careless-0.3.0/careless/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:39.000000 careless-0.3.0/careless/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-23 21:55:39.000000 careless-0.3.0/careless/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:50.118896 careless-0.3.0/careless/models/likelihoods/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 21:55:39.000000 careless-0.3.0/careless/models/likelihoods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-23 21:55:39.000000 careless-0.3.0/careless/models/likelihoods/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-23 21:55:39.000000 careless-0.3.0/careless/models/likelihoods/laue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-23 21:55:39.000000 careless-0.3.0/careless/models/likelihoods/mono.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:50.122896 careless-0.3.0/careless/models/merging/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-23 21:55:39.000000 careless-0.3.0/careless/models/merging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-05-23 21:55:39.000000 careless-0.3.0/careless/models/merging/surrogate_posteriors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-05-23 21:55:39.000000 careless-0.3.0/careless/models/merging/variational.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:50.122896 careless-0.3.0/careless/models/priors/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-23 21:55:39.000000 careless-0.3.0/careless/models/priors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-23 21:55:39.000000 careless-0.3.0/careless/models/priors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-05-23 21:55:39.000000 careless-0.3.0/careless/models/priors/empirical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-05-23 21:55:39.000000 careless-0.3.0/careless/models/priors/wilson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:50.122896 careless-0.3.0/careless/models/scaling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:39.000000 careless-0.3.0/careless/models/scaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-23 21:55:39.000000 careless-0.3.0/careless/models/scaling/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-05-23 21:55:39.000000 careless-0.3.0/careless/models/scaling/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-23 21:55:39.000000 careless-0.3.0/careless/models/scaling/nn.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4389 2023-05-23 21:55:39.000000 careless-0.3.0/careless/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:50.126896 careless-0.3.0/careless/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:39.000000 careless-0.3.0/careless/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-05-23 21:55:39.000000 careless-0.3.0/careless/stats/ccanom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-05-23 21:55:39.000000 careless-0.3.0/careless/stats/cchalf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-05-23 21:55:39.000000 careless-0.3.0/careless/stats/ccpred.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-23 21:55:39.000000 careless-0.3.0/careless/stats/completeness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-23 21:55:39.000000 careless-0.3.0/careless/stats/rsplit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:50.126896 careless-0.3.0/careless/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:39.000000 careless-0.3.0/careless/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-23 21:55:39.000000 careless-0.3.0/careless/utils/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-05-23 21:55:39.000000 careless-0.3.0/careless/utils/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-05-23 21:55:39.000000 careless-0.3.0/careless/utils/laue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-23 21:55:39.000000 careless-0.3.0/careless/utils/positional_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-23 21:55:39.000000 careless-0.3.0/careless/utils/shame.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:50.114896 careless-0.3.0/careless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-23 21:55:50.000000 careless-0.3.0/careless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-23 21:55:50.000000 careless-0.3.0/careless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 21:55:50.000000 careless-0.3.0/careless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-23 21:55:50.000000 careless-0.3.0/careless.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-23 21:55:50.000000 careless-0.3.0/careless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-23 21:55:50.000000 careless-0.3.0/careless.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:50.126896 careless-0.3.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3872 2023-05-23 21:55:39.000000 careless-0.3.0/scripts/make_difference_map
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-05-23 21:55:39.000000 careless-0.3.0/scripts/stream2mtz
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-23 21:55:50.130896 careless-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-23 21:55:39.000000 careless-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:50.126896 careless-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:39.000000 careless-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-05-23 21:55:39.000000 careless-0.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-05-23 21:55:39.000000 careless-0.3.0/tests/test_cli.py
```

### Comparing `careless-0.2.9/LICENSE` & `careless-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `careless-0.2.9/PKG-INFO` & `careless-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: careless
-Version: 0.2.9
+Version: 0.3.0
 Summary: Merging crystallography data without much physics.
 Home-page: https://github.com/rs-station/careless
 Author: Kevin M. Dalton
 Author-email: kmdalton@fas.harvard.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/rs-station/careless/issues
 Project-URL: Source Code, https://github.com/rs-station/careless
-Platform: UNKNOWN
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<3.12
 License-File: LICENSE
 
 
 ``careless`` is a command line utility for merging 
 data from x-ray crystallography experiments. It 
 can be used to simultaneously scale and merge integrated
 reflection intensities from conventional, laue, 
 and free-electron laser experiments. It uses approximate 
 Bayesian inference and deep learning to estimate
 merged structure factor amplitudes under a Wilson prior.
-
-
```

### Comparing `careless-0.2.9/README.md` & `careless-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `careless-0.2.9/careless/args/common.py` & `careless-0.3.0/careless/args/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,8 +42,14 @@
     }),
 
     (("--disable-metadata-standardization",), {
         "help": "By default careless will convert metadata to z-scores. This flag disables that behavior. In general, unstandardized metadata will lead to unstable optimization. However, this flag might be useful if the user wants to use their own normalization scheme." ,
         "action": "store_false", 
         "dest" : "standardize_metadata", 
     }),
+
+    (("--disable-progress-bar", ),  {
+        "help":"Disable the progress bar. This is helpful if you're logging stderr.",
+        "action" : "store_true",
+        "default" : False,
+    }),
 )
```

### Comparing `careless-0.2.9/careless/args/crossvalidation.py` & `careless-0.3.0/careless/args/crossvalidation.py`

 * *Files identical despite different names*

### Comparing `careless-0.2.9/careless/args/filtration.py` & `careless-0.3.0/careless/args/filtration.py`

 * *Files identical despite different names*

### Comparing `careless-0.2.9/careless/args/interpretation.py` & `careless-0.3.0/careless/args/interpretation.py`

 * *Files identical despite different names*

### Comparing `careless-0.2.9/careless/args/optimizer.py` & `careless-0.3.0/careless/args/optimizer.py`

 * *Files identical despite different names*

### Comparing `careless-0.2.9/careless/args/poly.py` & `careless-0.3.0/careless/args/poly.py`

 * *Files identical despite different names*

### Comparing `careless-0.2.9/careless/args/positional_encoding.py` & `careless-0.3.0/careless/args/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `careless-0.2.9/careless/args/prior.py` & `careless-0.3.0/careless/args/prior.py`

 * *Files identical despite different names*

### Comparing `careless-0.2.9/careless/args/required.py` & `careless-0.3.0/careless/args/required.py`

 * *Files identical despite different names*

### Comparing `careless-0.2.9/careless/args/scaling.py` & `careless-0.3.0/careless/args/scaling.py`

 * *Files identical despite different names*

### Comparing `careless-0.2.9/careless/args/tf_options.py` & `careless-0.3.0/careless/args/tf_options.py`

 * *Files identical despite different names*

### Comparing `careless-0.2.9/careless/callbacks/progress_bar.py` & `careless-0.3.0/careless/callbacks/progress_bar.py`

 * *Files identical despite different names*

### Comparing `careless-0.2.9/careless/careless.py` & `careless-0.3.0/careless/careless.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,21 +44,23 @@
 
     if parser.structure_factor_file is not None:
         model.surrogate_posterior.load_weights(parser.structure_factor_file)
     if parser.freeze_structure_factors:
         model.surrogate_posterior.trainable = False
 
     validation_frequency = parser.validation_frequency
+    progress = not parser.disable_progress_bar
 
     history = model.train_model(
         tuple(map(tf.convert_to_tensor, train)),
         parser.iterations,
         message="Training",
         validation_data=test,
         validation_frequency=validation_frequency,
+        progress=progress,
     )
 
     for i,ds in enumerate(dm.get_results(model.surrogate_posterior, inputs=train)):
         filename = parser.output_base + f'_{i}.mtz'
         ds.write_mtz(filename)
 
     filename = parser.output_base + f'_history.csv'
@@ -98,14 +100,15 @@
         for repeat in range(parser.half_dataset_repeats):
             for half_id, half in enumerate(dm.split_data_by_image()):
                 model = dm.build_model(scaling_model=scaling_model)
                 history = model.train_model(
                     tuple(map(tf.convert_to_tensor, half)), 
                     parser.iterations,
                     message=f"Merging repeat {repeat+1} half {half_id+1}",
+                    progress=progress,
                 )
 
                 for file_id,ds in enumerate(dm.get_results(model.surrogate_posterior, inputs=half)):
                     ds['repeat'] = rs.DataSeries(repeat, index=ds.index, dtype='I')
                     ds['half'] = rs.DataSeries(half_id, index=ds.index, dtype='I')
                     if xval_data[file_id] is None:
                         xval_data[file_id] = ds
```

### Comparing `careless-0.2.9/careless/io/asu.py` & `careless-0.3.0/careless/io/asu.py`

 * *Files identical despite different names*

### Comparing `careless-0.2.9/careless/io/formatter.py` & `careless-0.3.0/careless/io/formatter.py`

 * *Files identical despite different names*

### Comparing `careless-0.2.9/careless/io/manager.py` & `careless-0.3.0/careless/io/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,20 +34,26 @@
     def from_mtz_files(cls, filenames, formatter):
         return cls.from_datasets((rs.read_mtz(i) for i in filenames), formatter)
 
     @classmethod
     def from_stream_files(cls, filenames, formatter):
         return cls.from_datasets((rs.read_crystfel(i) for i in filenames), formatter)
 
+    def get_wilson_sigma(self, b=None):
+        if b is None:
+            return 1.
+        sigma = np.exp(-0.25 * b * self.asu_collection.dHKL**-2.)
+        return sigma
+
     def get_wilson_prior(self, b=None, k=1.):
         """ Construct a wilson prior with an optional temperature factor, b, appropriate for self.asu_collection. """
         if b is None:
             sigma = 1.
         elif isinstance(b, float):
-            sigma = np.exp(-0.25 * b * self.asu_collection.dHKL**-2.)
+            sigma = self.get_wilson_sigma(b)
         else:
             raise ValueError(f"parameter b has type{type(b)} but float was expected")
         sigma = sigma * k
 
         return WilsonPrior(
             self.asu_collection.centric,
             self.asu_collection.multiplicity,
@@ -367,15 +373,16 @@
         parents = parser.parents
         r_values = parser.dwr
         if prior is None and parents is None:
             prior = self.get_wilson_prior(parser.wilson_prior_b)
         elif prior is None and parser.parents is not None:
             parents = [None if i == 'None' else int(i) for i in parents.split(',')]
             r_values = [float(i) for i in r_values.split(',')]
-            prior = DoubleWilsonPrior(self.asu_collection, parents, r_values)
+            sigma = self.get_wilson_sigma(parser.wilson_prior_b)
+            prior = DoubleWilsonPrior(self.asu_collection, parents, r_values, sigma=sigma)
 
         loc,scale = prior.mean(),prior.stddev()
         scale = scale * parser.structure_factor_init_scale
         low = (1e-32 * ~self.asu_collection.centric).astype('float32')
         if surrogate_posterior is None:
             surrogate_posterior = TruncatedNormal.from_loc_and_scale(loc, scale, low, scale_shift=parser.epsilon)
```

### Comparing `careless-0.2.9/careless/models/base.py` & `careless-0.3.0/careless/models/base.py`

 * *Files identical despite different names*

### Comparing `careless-0.2.9/careless/models/likelihoods/laue.py` & `careless-0.3.0/careless/models/likelihoods/laue.py`

 * *Files identical despite different names*

### Comparing `careless-0.2.9/careless/models/likelihoods/mono.py` & `careless-0.3.0/careless/models/likelihoods/mono.py`

 * *Files identical despite different names*

### Comparing `careless-0.2.9/careless/models/merging/surrogate_posteriors.py` & `careless-0.3.0/careless/models/merging/surrogate_posteriors.py`

 * *Files identical despite different names*

### Comparing `careless-0.2.9/careless/models/merging/variational.py` & `careless-0.3.0/careless/models/merging/variational.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
 
         #Do some keras-y stuff
         self.add_loss(-ll)
         self.add_metric(-ll, name="NLL")
 
         return ipred
 
-    def train_model(self, data, steps, message=None, format_string="{:0.2e}", validation_data=None, validation_frequency=10):
+    def train_model(self, data, steps, message=None, format_string="{:0.2e}", validation_data=None, validation_frequency=10, progress=True):
         """
         Alternative to the keras backed VariationalMergingModel.fit method. This method is much faster at the moment but less flexible.
         """
         def train_step(model_and_data):
             model, data = model_and_data
             model.reset_metrics()
             history = model.train_step((data,))
@@ -163,15 +163,16 @@
             train_step = tf.function(train_step, reduce_retracing=True)
 
         if validation_data is not None:
             val_scale = len(data[0]) / len(validation_data[0])
 
         history = {}
         from tqdm import trange
-        bar = trange(steps, desc=message)
+        disable_progress = not progress
+        bar = trange(steps, desc=message, disable=disable_progress)
         for i in bar:
             _history = train_step((self, data))
             if validation_data is not None:
                 if i%validation_frequency==0:
                     validation_metrics = self.test_on_batch(validation_data, return_dict=True)
                 _history['NLL_val'] = val_scale * validation_metrics['NLL']
```

### Comparing `careless-0.2.9/careless/models/priors/empirical.py` & `careless-0.3.0/careless/models/priors/empirical.py`

 * *Files identical despite different names*

### Comparing `careless-0.2.9/careless/models/priors/wilson.py` & `careless-0.3.0/careless/models/priors/wilson.py`

 * *Files identical despite different names*

### Comparing `careless-0.2.9/careless/models/scaling/image.py` & `careless-0.3.0/careless/models/scaling/image.py`

 * *Files identical despite different names*

### Comparing `careless-0.2.9/careless/models/scaling/nn.py` & `careless-0.3.0/careless/models/scaling/nn.py`

 * *Files identical despite different names*

### Comparing `careless-0.2.9/careless/parser.py` & `careless-0.3.0/careless/parser.py`

 * *Files identical despite different names*

### Comparing `careless-0.2.9/careless/stats/ccanom.py` & `careless-0.3.0/careless/stats/ccanom.py`

 * *Files identical despite different names*

### Comparing `careless-0.2.9/careless/stats/cchalf.py` & `careless-0.3.0/careless/stats/cchalf.py`

 * *Files identical despite different names*

### Comparing `careless-0.2.9/careless/stats/ccpred.py` & `careless-0.3.0/careless/stats/ccpred.py`

 * *Files 5% similar despite different names*

```diff
@@ -118,21 +118,29 @@
 
     results['bin'] = results['bin'].to_numpy('int32')
     results['test'] = np.array(['Train', 'Test'])[results['test']]
 
     if args.output is not None:
         results.to_csv(args.output)
 
-    sns.lineplot(
-        data = results,
-        x = 'bin',
-        y = 'CCpred',
-        style = 'test',
-        color="k",
-    )
+    plot_kwargs = {
+        'data' : results,
+        'x' : 'bin',
+        'y' : 'CCpred',
+        'style' : 'test',
+    }
+
+    if 'file' in results:
+        plot_kwargs['hue'] = 'file'
+        plot_kwargs['palette'] = "Dark2"
+    else:
+        plot_kwargs['color'] = 'k'
+
+    sns.lineplot(**plot_kwargs)
+
     plt.xticks(range(args.bins), labels, rotation=45, ha="right", rotation_mode="anchor")
     plt.ylabel(r"$\mathrm{CC_{pred}}$ " + f"({args.method})")
     plt.legend(loc="center left", bbox_to_anchor=(1, 0.5))
     plt.xlabel("Resolution ($\mathrm{\AA}$)")
     plt.grid(which='both', axis='both', ls='dashdot')
     plt.tight_layout()
     print(results.to_string())
```

### Comparing `careless-0.2.9/careless/stats/completeness.py` & `careless-0.3.0/careless/stats/completeness.py`

 * *Files identical despite different names*

### Comparing `careless-0.2.9/careless/stats/rsplit.py` & `careless-0.3.0/careless/stats/rsplit.py`

 * *Files identical despite different names*

### Comparing `careless-0.2.9/careless/utils/distributions.py` & `careless-0.3.0/careless/utils/distributions.py`

 * *Files identical despite different names*

### Comparing `careless-0.2.9/careless/utils/laue.py` & `careless-0.3.0/careless/utils/laue.py`

 * *Files identical despite different names*

### Comparing `careless-0.2.9/careless/utils/positional_encoding.py` & `careless-0.3.0/careless/utils/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `careless-0.2.9/careless.egg-info/PKG-INFO` & `careless-0.3.0/careless.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: careless
-Version: 0.2.9
+Version: 0.3.0
 Summary: Merging crystallography data without much physics.
 Home-page: https://github.com/rs-station/careless
 Author: Kevin M. Dalton
 Author-email: kmdalton@fas.harvard.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/rs-station/careless/issues
 Project-URL: Source Code, https://github.com/rs-station/careless
-Platform: UNKNOWN
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<3.12
 License-File: LICENSE
 
 
 ``careless`` is a command line utility for merging 
 data from x-ray crystallography experiments. It 
 can be used to simultaneously scale and merge integrated
 reflection intensities from conventional, laue, 
 and free-electron laser experiments. It uses approximate 
 Bayesian inference and deep learning to estimate
 merged structure factor amplitudes under a Wilson prior.
-
-
```

### Comparing `careless-0.2.9/careless.egg-info/SOURCES.txt` & `careless-0.3.0/careless.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 careless/args/tf_options.py
 careless/callbacks/__init__.py
 careless/callbacks/progress_bar.py
 careless/io/__init__.py
 careless/io/asu.py
 careless/io/formatter.py
 careless/io/manager.py
+careless/io/xds.py
 careless/models/__init__.py
 careless/models/base.py
 careless/models/likelihoods/__init__.py
 careless/models/likelihoods/base.py
 careless/models/likelihoods/laue.py
 careless/models/likelihoods/mono.py
 careless/models/merging/__init__.py
```

### Comparing `careless-0.2.9/scripts/make_difference_map` & `careless-0.3.0/scripts/make_difference_map`

 * *Files identical despite different names*

### Comparing `careless-0.2.9/scripts/stream2mtz` & `careless-0.3.0/scripts/stream2mtz`

 * *Files identical despite different names*

### Comparing `careless-0.2.9/setup.py` & `careless-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     author_email="kmdalton@fas.harvard.edu",
     license="MIT",
     include_package_data=True,
     packages=find_packages(),
     long_description=LONG_DESCRIPTION,
     description="Merging crystallography data without much physics.",
     project_urls=PROJECT_URLS,
-    python_requires=">=3.8,<3.11",
+    python_requires=">=3.8,<3.12",
     url="https://github.com/rs-station/careless",
     install_requires=[
         "reciprocalspaceship>=0.9.16",
         "tqdm",
         "tensorflow>=2.8",
         "tensorflow-probability",
         "matplotlib",
@@ -54,12 +54,13 @@
         "console_scripts": [
             "careless=careless.careless:main",
             "careless.ccanom=careless.stats.ccanom:main",
             "careless.cchalf=careless.stats.cchalf:main",
             "careless.ccpred=careless.stats.ccpred:main",
             "careless.completeness=careless.stats.completeness:main",
             "careless.rsplit=careless.stats.rsplit:main",
+            "careless.xds2mtz=careless.io.xds:main",
         ]
     },
     setup_requires=["pytest-runner"],
     tests_require=["pytest", "pytest-cov", "pytest-xdist>=3"],
 )
```

### Comparing `careless-0.2.9/tests/conftest.py` & `careless-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `careless-0.2.9/tests/test_cli.py` & `careless-0.3.0/tests/test_cli.py`

 * *Files identical despite different names*

