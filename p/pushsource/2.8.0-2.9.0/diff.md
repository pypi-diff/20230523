# Comparing `tmp/pushsource-2.8.0.tar.gz` & `tmp/pushsource-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pushsource-2.8.0.tar", last modified: Thu Jun 24 21:11:31 2021, max compression
+gzip compressed data, was "pushsource-2.9.0.tar", last modified: Sun Jul  4 22:06:03 2021, max compression
```

## Comparing `pushsource-2.8.0.tar` & `pushsource-2.9.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-24 21:11:31.137032 pushsource-2.8.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5032 2021-06-24 21:09:29.000000 pushsource-2.8.0/CHANGELOG.md
--rw-rw-r--   0 travis    (2000) travis    (2000)    35149 2021-06-24 21:09:29.000000 pushsource-2.8.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       90 2021-06-24 21:09:29.000000 pushsource-2.8.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     2839 2021-06-24 21:11:31.133030 pushsource-2.8.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1919 2021-06-24 21:09:29.000000 pushsource-2.8.0/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      126 2021-06-24 21:09:29.000000 pushsource-2.8.0/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-06-24 21:11:31.137032 pushsource-2.8.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1563 2021-06-24 21:09:29.000000 pushsource-2.8.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-24 21:11:31.125026 pushsource-2.8.0/src/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-24 21:11:31.129028 pushsource-2.8.0/src/pushsource/
--rw-rw-r--   0 travis    (2000) travis    (2000)      710 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-24 21:11:31.129028 pushsource-2.8.0/src/pushsource/_impl/
--rw-rw-r--   0 travis    (2000) travis    (2000)      122 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-24 21:11:31.129028 pushsource-2.8.0/src/pushsource/_impl/backend/
--rw-rw-r--   0 travis    (2000) travis    (2000)      109 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/backend/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-24 21:11:31.129028 pushsource-2.8.0/src/pushsource/_impl/backend/errata_source/
--rw-rw-r--   0 travis    (2000) travis    (2000)       40 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/backend/errata_source/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4158 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/backend/errata_source/errata_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17923 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/backend/errata_source/errata_source.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5525 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/backend/koji_containers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22633 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/backend/koji_source.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1094 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/backend/modulemd.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-24 21:11:31.133030 pushsource-2.8.0/src/pushsource/_impl/backend/staged/
--rw-rw-r--   0 travis    (2000) travis    (2000)       40 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/backend/staged/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2055 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/backend/staged/staged_ami.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1351 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/backend/staged/staged_base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      343 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/backend/staged/staged_compsxml.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1028 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/backend/staged/staged_errata.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      779 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/backend/staged/staged_files.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      346 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/backend/staged/staged_modulemd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      350 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/backend/staged/staged_productid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      949 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/backend/staged/staged_rpm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5675 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/backend/staged/staged_source.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      360 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/backend/staged/staged_unsupported.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/backend/staged/staged_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      487 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/compat.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      328 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/compat_attr.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2423 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/helpers.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-24 21:11:31.133030 pushsource-2.8.0/src/pushsource/_impl/model/
--rw-rw-r--   0 travis    (2000) travis    (2000)      677 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/model/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4130 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/model/ami.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7518 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/model/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      450 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/model/comps.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10419 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/model/container.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3215 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/model/conv.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12996 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/model/erratum.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4700 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/model/erratum_fixup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      757 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/model/file.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      895 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/model/modulemd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      436 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/model/productid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1475 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/model/rpm.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-24 21:11:31.133030 pushsource-2.8.0/src/pushsource/_impl/schema/
--rw-rw-r--   0 travis    (2000) travis    (2000)      252 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/schema/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3805 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/schema/errata-schema.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)     6257 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/schema/staged-schema.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)     7494 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/source.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4513 2021-06-24 21:09:29.000000 pushsource-2.8.0/src/pushsource/_impl/validator.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-24 21:11:31.129028 pushsource-2.8.0/src/pushsource.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2839 2021-06-24 21:11:31.000000 pushsource-2.8.0/src/pushsource.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2046 2021-06-24 21:11:31.000000 pushsource-2.8.0/src/pushsource.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-06-24 21:11:31.000000 pushsource-2.8.0/src/pushsource.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      129 2021-06-24 21:11:31.000000 pushsource-2.8.0/src/pushsource.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       11 2021-06-24 21:11:31.000000 pushsource-2.8.0/src/pushsource.egg-info/top_level.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-07-04 22:06:03.764846 pushsource-2.9.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5267 2021-07-04 22:04:05.000000 pushsource-2.9.0/CHANGELOG.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35149 2021-07-04 22:04:05.000000 pushsource-2.9.0/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)       90 2021-07-04 22:04:05.000000 pushsource-2.9.0/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2849 2021-07-04 22:06:03.764846 pushsource-2.9.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1929 2021-07-04 22:04:05.000000 pushsource-2.9.0/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      126 2021-07-04 22:04:05.000000 pushsource-2.9.0/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-07-04 22:06:03.764846 pushsource-2.9.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1563 2021-07-04 22:04:05.000000 pushsource-2.9.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-07-04 22:06:03.756846 pushsource-2.9.0/src/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-07-04 22:06:03.756846 pushsource-2.9.0/src/pushsource/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      710 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-07-04 22:06:03.760846 pushsource-2.9.0/src/pushsource/_impl/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      122 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-07-04 22:06:03.760846 pushsource-2.9.0/src/pushsource/_impl/backend/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      109 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/backend/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-07-04 22:06:03.760846 pushsource-2.9.0/src/pushsource/_impl/backend/errata_source/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       40 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/backend/errata_source/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4275 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/backend/errata_source/errata_client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18436 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/backend/errata_source/errata_source.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5525 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/backend/koji_containers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23447 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/backend/koji_source.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1094 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/backend/modulemd.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-07-04 22:06:03.760846 pushsource-2.9.0/src/pushsource/_impl/backend/staged/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       40 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/backend/staged/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2055 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/backend/staged/staged_ami.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1351 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/backend/staged/staged_base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      343 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/backend/staged/staged_compsxml.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1028 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/backend/staged/staged_errata.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      779 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/backend/staged/staged_files.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      346 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/backend/staged/staged_modulemd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      350 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/backend/staged/staged_productid.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      949 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/backend/staged/staged_rpm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5861 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/backend/staged/staged_source.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      360 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/backend/staged/staged_unsupported.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/backend/staged/staged_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      487 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/compat.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      328 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/compat_attr.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2423 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/helpers.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-07-04 22:06:03.764846 pushsource-2.9.0/src/pushsource/_impl/model/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      677 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/model/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4130 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/model/ami.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7518 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/model/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      450 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/model/comps.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10419 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/model/container.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3215 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/model/conv.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12996 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/model/erratum.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4700 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/model/erratum_fixup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      757 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/model/file.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      895 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/model/modulemd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      436 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/model/productid.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1475 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/model/rpm.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-07-04 22:06:03.764846 pushsource-2.9.0/src/pushsource/_impl/schema/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      252 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/schema/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3805 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/schema/errata-schema.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6257 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/schema/staged-schema.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8862 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/source.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4513 2021-07-04 22:04:05.000000 pushsource-2.9.0/src/pushsource/_impl/validator.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-07-04 22:06:03.756846 pushsource-2.9.0/src/pushsource.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2849 2021-07-04 22:06:03.000000 pushsource-2.9.0/src/pushsource.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2046 2021-07-04 22:06:03.000000 pushsource-2.9.0/src/pushsource.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-07-04 22:06:03.000000 pushsource-2.9.0/src/pushsource.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      129 2021-07-04 22:06:03.000000 pushsource-2.9.0/src/pushsource.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       11 2021-07-04 22:06:03.000000 pushsource-2.9.0/src/pushsource.egg-info/top_level.txt
```

### Comparing `pushsource-2.8.0/CHANGELOG.md` & `pushsource-2.9.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
 - n/a
 
+## [2.9.0] - 2021-07-05
+
+### Changed
+
+- `Source` instances now support `with` statements to ensure that resources are freed
+  when no longer required.
+
 ## [2.8.0] - 2021-06-25
 
 ### Added
 
 - Added `build_info` attribute to push items.
 - Added `module_build` attribute to RPM push items.
 - Added `rpm_filter_arch` parameter to errata source, to select a subset of RPMs
@@ -132,15 +139,16 @@
 ### Changed
 - Improved log message details in some cases of error
 
 ## 1.0.0 - 2020-06-16
 
 - Initial stable release of project
 
-[Unreleased]: https://github.com/release-engineering/pushsource/compare/v2.8.0...HEAD
+[Unreleased]: https://github.com/release-engineering/pushsource/compare/v2.9.0...HEAD
+[2.9.0]: https://github.com/release-engineering/pushsource/compare/v2.8.0...v2.9.0
 [2.8.0]: https://github.com/release-engineering/pushsource/compare/v2.7.0...v2.8.0
 [2.7.0]: https://github.com/release-engineering/pushsource/compare/v2.6.0...v2.7.0
 [2.6.0]: https://github.com/release-engineering/pushsource/compare/v2.5.0...v2.6.0
 [2.5.0]: https://github.com/release-engineering/pushsource/compare/v2.4.0...v2.5.0
 [2.4.0]: https://github.com/release-engineering/pushsource/compare/v2.3.0...v2.4.0
 [2.3.0]: https://github.com/release-engineering/pushsource/compare/v2.2.0...v2.3.0
 [2.2.0]: https://github.com/release-engineering/pushsource/compare/v2.1.0...v2.2.0
```

### Comparing `pushsource-2.8.0/LICENSE` & `pushsource-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pushsource-2.8.0/PKG-INFO` & `pushsource-2.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pushsource
-Version: 2.8.0
+Version: 2.9.0
 Summary: A library to load push items from a variety of sources
 Home-page: https://github.com/release-engineering/pushsource
 License: GNU General Public License
 Project-URL: Documentation, https://release-engineering.github.io/pushsource/
 Project-URL: Changelog, https://github.com/release-engineering/pushsource/blob/master/CHANGELOG.md
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -47,18 +47,17 @@
 
 ```python
 from pushsource import Source
 
 # Get a source of content; sources and their parameters can be
 # specified by URL. This source will use a couple of RPMs from
 # Fedora koji as the content source.
-source = Source.get('koji:https://koji.fedoraproject.org/kojihub?rpm=python3-3.7.5-2.fc31.x86_64.rpm,python3-3.7.5-2.fc31.src.rpm')
-
-# Iterate over the content and do something with it:
-for push_item in source:
+with Source.get('koji:https://koji.fedoraproject.org/kojihub?rpm=python3-3.7.5-2.fc31.x86_64.rpm,python3-3.7.5-2.fc31.src.rpm') as source:
+  # Iterate over the content and do something with it:
+  for push_item in source:
     publish(push_item)
 ```
 
 Development
 -----------
 
 Patches may be contributed via pull requests to
```

### Comparing `pushsource-2.8.0/README.md` & `pushsource-2.9.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -27,18 +27,17 @@
 
 ```python
 from pushsource import Source
 
 # Get a source of content; sources and their parameters can be
 # specified by URL. This source will use a couple of RPMs from
 # Fedora koji as the content source.
-source = Source.get('koji:https://koji.fedoraproject.org/kojihub?rpm=python3-3.7.5-2.fc31.x86_64.rpm,python3-3.7.5-2.fc31.src.rpm')
-
-# Iterate over the content and do something with it:
-for push_item in source:
+with Source.get('koji:https://koji.fedoraproject.org/kojihub?rpm=python3-3.7.5-2.fc31.x86_64.rpm,python3-3.7.5-2.fc31.src.rpm') as source:
+  # Iterate over the content and do something with it:
+  for push_item in source:
     publish(push_item)
 ```
 
 Development
 -----------
 
 Patches may be contributed via pull requests to
```

### Comparing `pushsource-2.8.0/setup.py` & `pushsource-2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 def get_requirements():
     with open("requirements.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="pushsource",
-    version="2.8.0",
+    version="2.9.0",
     packages=find_packages("src"),
     package_dir={"": "src"},
     include_package_data=True,
     url="https://github.com/release-engineering/pushsource",
     license="GNU General Public License",
     description=get_description(),
     long_description=get_long_description(),
```

### Comparing `pushsource-2.8.0/src/pushsource/__init__.py` & `pushsource-2.9.0/src/pushsource/__init__.py`

 * *Files identical despite different names*

### Comparing `pushsource-2.8.0/src/pushsource/_impl/backend/errata_source/errata_client.py` & `pushsource-2.9.0/src/pushsource/_impl/backend/errata_source/errata_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,16 +18,18 @@
     advisory_cdn_file_list = attr.ib(type=dict)
     advisory_cdn_docker_file_list = attr.ib(type=dict)
     ftp_paths = attr.ib(type=dict)
 
 
 class ErrataClient(object):
     def __init__(self, threads, url, **retry_args):
-        self._executor = Executors.thread_pool(max_workers=threads).with_retry(
-            **retry_args
+        self._executor = (
+            Executors.thread_pool(max_workers=threads)
+            .with_retry(**retry_args)
+            .with_cancel_on_shutdown()
         )
         self._url = url
         self._tls = threading.local()
 
         self._get_advisory_cdn_metadata = partial(
             self._call_et, "get_advisory_cdn_metadata"
         )
@@ -35,14 +37,17 @@
             self._call_et, "get_advisory_cdn_file_list"
         )
         self._get_advisory_cdn_docker_file_list = partial(
             self._call_et, "get_advisory_cdn_docker_file_list"
         )
         self._get_ftp_paths = partial(self._call_et, "get_ftp_paths")
 
+    def shutdown(self):
+        self._executor.shutdown(True)
+
     @property
     def _errata_service(self):
         # XML-RPC client connected to errata_service.
         # Each thread uses a separate client.
         if not hasattr(self._tls, "errata_service"):
             LOG.debug("Creating XML-RPC client for Errata Tool: %s", self._url)
             self._tls.errata_service = xmlrpc_client.ServerProxy(self._url)
```

### Comparing `pushsource-2.8.0/src/pushsource/_impl/backend/errata_source/errata_source.py` & `pushsource-2.9.0/src/pushsource/_impl/backend/errata_source/errata_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,26 +75,40 @@
         self._url = url
         self._errata = list_argument(errata)
         self._client = ErrataClient(threads=threads, url=self._errata_service_url)
 
         self._rpm_filter_arch = list_argument(rpm_filter_arch, retain_none=True)
 
         # This executor doesn't use retry because koji & ET executors already do that.
-        self._executor = Executors.thread_pool(max_workers=threads)
+        self._executor = Executors.thread_pool(
+            max_workers=threads
+        ).with_cancel_on_shutdown()
 
         # We set aside a separate thread pool for koji so that there are separate
         # queues for ET and koji calls, yet we avoid creating a new thread pool for
         # each koji source.
-        self._koji_executor = Executors.thread_pool(max_workers=threads).with_retry()
+        self._koji_executor = (
+            Executors.thread_pool(max_workers=threads)
+            .with_retry()
+            .with_cancel_on_shutdown()
+        )
         self._koji_cache = {}
         self._koji_source_url = koji_source
 
         self._legacy_container_repos = try_bool(legacy_container_repos)
         self._timeout = timeout
 
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self._client.shutdown()
+        self._executor.shutdown(True)
+        self._koji_executor.shutdown(True)
+
     @property
     def _errata_service_url(self):
         # URL for the errata_service XML-RPC endpoint provided by ET.
         #
         # Note the odd handling of scheme here. The reason is that
         # ET oddly provides different APIs over http and https.
         #
@@ -164,35 +178,39 @@
         #             }
         #         }
         #     }
         # }
         #
 
         # We'll be getting container metadata from these builds.
-        koji_source = self._koji_source(container_build=list(docker_file_list.keys()))
-
-        out = []
-
-        for item in koji_source:
-            if isinstance(item, ContainerImagePushItem):
-                item = self._enrich_container_push_item(erratum, docker_file_list, item)
-            elif isinstance(item, OperatorManifestPushItem):
-                # Accept this item but nothing special to do
-                pass
-            else:
-                # If build contained anything else, ignore it
-                LOG.debug(
-                    "Erratum %s: ignored unexpected item from koji source: %s",
-                    erratum.name,
-                    item,
-                )
-                continue
+        with self._koji_source(
+            container_build=list(docker_file_list.keys())
+        ) as koji_source:
+
+            out = []
+
+            for item in koji_source:
+                if isinstance(item, ContainerImagePushItem):
+                    item = self._enrich_container_push_item(
+                        erratum, docker_file_list, item
+                    )
+                elif isinstance(item, OperatorManifestPushItem):
+                    # Accept this item but nothing special to do
+                    pass
+                else:
+                    # If build contained anything else, ignore it
+                    LOG.debug(
+                        "Erratum %s: ignored unexpected item from koji source: %s",
+                        erratum.name,
+                        item,
+                    )
+                    continue
 
-            item = attr.evolve(item, origin=erratum.name)
-            out.append(item)
+                item = attr.evolve(item, origin=erratum.name)
+                out.append(item)
 
         return out
 
     def _enrich_container_push_item(self, erratum, docker_file_list, item):
         # metadata from koji doesn't contain info about where the image should be
         # pushed and a few other things - enrich it now
         errata_meta = docker_file_list.get(item.build) or {}
@@ -256,30 +274,30 @@
 
         module_filenames = list(modules.keys())
 
         # We always request the modulemd.src.txt because we might need it later
         # depending on the ftp_paths response.
         module_filenames.append("modulemd.src.txt")
 
+        out = []
+
         # Get a koji source which will yield all modules from the build
-        koji_source = self._koji_source(
+        with self._koji_source(
             module_build=[build_nvr], module_filter_filename=module_filenames
-        )
-
-        out = []
+        ) as koji_source:
 
-        for push_item in koji_source:
-            # ET uses filenames to identify the modules here, we must do the same.
-            basename = os.path.basename(push_item.src)
-            dest = modules.pop(basename, [])
+            for push_item in koji_source:
+                # ET uses filenames to identify the modules here, we must do the same.
+                basename = os.path.basename(push_item.src)
+                dest = modules.pop(basename, [])
 
-            # Fill in more push item details based on the info provided by ET.
-            push_item = attr.evolve(push_item, dest=dest, origin=erratum.name)
+                # Fill in more push item details based on the info provided by ET.
+                push_item = attr.evolve(push_item, dest=dest, origin=erratum.name)
 
-            out.append(push_item)
+                out.append(push_item)
 
         # Were there any requested modules we couldn't find?
         missing_modules = ", ".join(sorted(modules.keys()))
         if missing_modules:
             msg = "koji build {nvr} does not contain {missing} (requested by advisory {erratum})".format(
                 nvr=build_nvr, missing=missing_modules, erratum=erratum.name
             )
```

### Comparing `pushsource-2.8.0/src/pushsource/_impl/backend/koji_containers.py` & `pushsource-2.9.0/src/pushsource/_impl/backend/koji_containers.py`

 * *Files identical despite different names*

### Comparing `pushsource-2.8.0/src/pushsource/_impl/backend/koji_source.py` & `pushsource-2.9.0/src/pushsource/_impl/backend/koji_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,17 +199,31 @@
         self._signing_key = list_argument(signing_key)
         self._dest = list_argument(dest)
         self._timeout = timeout
         self._pathinfo = koji.PathInfo(basedir)
         self._cache = {} if cache is None else cache
         self._threads = threads
         self._executor = (
-            executor or Executors.thread_pool(max_workers=threads).with_retry()
+            executor
+            or Executors.thread_pool(max_workers=threads)
+            .with_retry()
+            .with_cancel_on_shutdown()
         )
 
+        self._on_shutdown = []
+        if not executor:
+            self._on_shutdown.append(lambda: self._executor.shutdown(True))
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        for cb in self._on_shutdown:
+            cb()
+
     @property
     def _koji_session(self):
         # A koji client session.
         # Each thread uses a separate client.
         with CACHE_LOCK:
             tls = self._cache.setdefault("tls", threading.local())
             if not hasattr(tls, "koji_session"):
@@ -587,14 +601,31 @@
             )
             for i in range(0, self._threads)
         ]
 
         # Wait for all fetches to finish
         for t in fetch_threads:
             t.start()
+
+        # If we are asked to shut down early then also shut down those threads
+        # as soon as we can.
+        def fetch_shutdown():
+            try:
+                # Empty the queue
+                while True:
+                    koji_queue.get_nowait()
+            except Empty:
+                pass
+
+            # Then ask the threads to join
+            for t in fetch_threads:
+                t.join()
+
+        self._on_shutdown.append(fetch_shutdown)
+
         for t in fetch_threads:
             t.join(self._timeout)
 
         # Re-raise exceptions, if any.
         # If we got more than one, we're only propagating the first.
         if fetch_exceptions:
             raise fetch_exceptions[0]
```

### Comparing `pushsource-2.8.0/src/pushsource/_impl/backend/modulemd.py` & `pushsource-2.9.0/src/pushsource/_impl/backend/modulemd.py`

 * *Files identical despite different names*

### Comparing `pushsource-2.8.0/src/pushsource/_impl/backend/staged/staged_ami.py` & `pushsource-2.9.0/src/pushsource/_impl/backend/staged/staged_ami.py`

 * *Files identical despite different names*

### Comparing `pushsource-2.8.0/src/pushsource/_impl/backend/staged/staged_base.py` & `pushsource-2.9.0/src/pushsource/_impl/backend/staged/staged_base.py`

 * *Files identical despite different names*

### Comparing `pushsource-2.8.0/src/pushsource/_impl/backend/staged/staged_errata.py` & `pushsource-2.9.0/src/pushsource/_impl/backend/staged/staged_errata.py`

 * *Files identical despite different names*

### Comparing `pushsource-2.8.0/src/pushsource/_impl/backend/staged/staged_files.py` & `pushsource-2.9.0/src/pushsource/_impl/backend/staged/staged_files.py`

 * *Files identical despite different names*

### Comparing `pushsource-2.8.0/src/pushsource/_impl/backend/staged/staged_rpm.py` & `pushsource-2.9.0/src/pushsource/_impl/backend/staged/staged_rpm.py`

 * *Files identical despite different names*

### Comparing `pushsource-2.8.0/src/pushsource/_impl/backend/staged/staged_source.py` & `pushsource-2.9.0/src/pushsource/_impl/backend/staged/staged_source.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,18 +71,26 @@
         super(StagedSource, self).__init__()
         self._url = list_argument(url)
         self._threads = threads
         self._timeout = timeout
 
         # Note: this executor does not have a retry.
         # NFS already does a lot of its own retries.
-        self._executor = Executors.thread_pool(max_workers=threads).with_timeout(
-            timeout
+        self._executor = (
+            Executors.thread_pool(max_workers=threads)
+            .with_timeout(timeout)
+            .with_cancel_on_shutdown()
         )
 
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self._executor.shutdown()
+
     def __iter__(self):
         # Possible improvement would be to handle the separate dirs concurrently.
         # However, may not be worthwhile, as  in practice I'm not sure the ability
         # to pass more than a single staging directory is ever used (?)
         return itertools.chain(
             *[self._push_items_for_topdir(x) for x in self._url]
         ).__iter__()
```

### Comparing `pushsource-2.8.0/src/pushsource/_impl/backend/staged/staged_utils.py` & `pushsource-2.9.0/src/pushsource/_impl/backend/staged/staged_utils.py`

 * *Files identical despite different names*

### Comparing `pushsource-2.8.0/src/pushsource/_impl/helpers.py` & `pushsource-2.9.0/src/pushsource/_impl/helpers.py`

 * *Files identical despite different names*

### Comparing `pushsource-2.8.0/src/pushsource/_impl/model/__init__.py` & `pushsource-2.9.0/src/pushsource/_impl/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pushsource-2.8.0/src/pushsource/_impl/model/ami.py` & `pushsource-2.9.0/src/pushsource/_impl/model/ami.py`

 * *Files identical despite different names*

### Comparing `pushsource-2.8.0/src/pushsource/_impl/model/base.py` & `pushsource-2.9.0/src/pushsource/_impl/model/base.py`

 * *Files identical despite different names*

### Comparing `pushsource-2.8.0/src/pushsource/_impl/model/container.py` & `pushsource-2.9.0/src/pushsource/_impl/model/container.py`

 * *Files identical despite different names*

### Comparing `pushsource-2.8.0/src/pushsource/_impl/model/conv.py` & `pushsource-2.9.0/src/pushsource/_impl/model/conv.py`

 * *Files identical despite different names*

### Comparing `pushsource-2.8.0/src/pushsource/_impl/model/erratum.py` & `pushsource-2.9.0/src/pushsource/_impl/model/erratum.py`

 * *Files identical despite different names*

### Comparing `pushsource-2.8.0/src/pushsource/_impl/model/erratum_fixup.py` & `pushsource-2.9.0/src/pushsource/_impl/model/erratum_fixup.py`

 * *Files identical despite different names*

### Comparing `pushsource-2.8.0/src/pushsource/_impl/model/file.py` & `pushsource-2.9.0/src/pushsource/_impl/model/file.py`

 * *Files identical despite different names*

### Comparing `pushsource-2.8.0/src/pushsource/_impl/model/modulemd.py` & `pushsource-2.9.0/src/pushsource/_impl/model/modulemd.py`

 * *Files identical despite different names*

### Comparing `pushsource-2.8.0/src/pushsource/_impl/model/rpm.py` & `pushsource-2.9.0/src/pushsource/_impl/model/rpm.py`

 * *Files identical despite different names*

### Comparing `pushsource-2.8.0/src/pushsource/_impl/schema/errata-schema.yaml` & `pushsource-2.9.0/src/pushsource/_impl/schema/errata-schema.yaml`

 * *Files identical despite different names*

### Comparing `pushsource-2.8.0/src/pushsource/_impl/schema/staged-schema.yaml` & `pushsource-2.9.0/src/pushsource/_impl/schema/staged-schema.yaml`

 * *Files identical despite different names*

### Comparing `pushsource-2.8.0/src/pushsource/_impl/source.py` & `pushsource-2.9.0/src/pushsource/_impl/source.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,25 +21,70 @@
 
 class SourceUrlError(ValueError):
     """Errors of this type are raised when an invalid URL is provided
     to :meth:`~pushsource.Source.get` and related methods.
     """
 
 
+class SourceWrapper(object):
+    # Internal class to ensure that all source instances support enter/exit
+    # for with statements even if underlying instance doesn't implement it
+    # (since it originally was not mandatory).
+    def __init__(self, delegate):
+        self.__delegate = delegate
+
+    def __iter__(self):
+        return self.__delegate.__iter__()
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        pass
+
+    @classmethod
+    def _maybe_wrap(cls, delegate):
+        if hasattr(delegate, "__enter__"):
+            # no wrapping needed
+            return delegate
+        # wrap with a no-op enter/exit
+        return cls(delegate)
+
+
 class Source(object):
     """A source of push items.
 
     This base class defines the interface for all pushsource backends.
     Instances of a specific backend can be obtained using
     the :meth:`~pushsource.Source.get` method.
+
+    Though not mandatory, instances of ``Source`` are preferably used
+    via ``with`` statements to ensure that all resources are cleaned up
+    when no longer needed, as in example:
+
+    .. code-block:: python
+
+        with Source.get('some-url') as source:
+            for item in source:
+                do_something(item)
+
+    Note that the items produced by a source are not bound to the lifecycle
+    of a source instance, so it's safe to store them and continue using
+    them beyond the end of the ``with`` statement.
     """
 
     _BACKENDS = {}
     _BACKENDS_BUILTIN = {}
 
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        pass
+
     def __iter__(self):
         """Iterate over the push items contained within this source.
 
         Yields a series of :class:`~pushsource.PushItem` instances.
         """
         raise NotImplementedError()
 
@@ -155,15 +200,15 @@
 
         url_kwargs.update(kwargs)
 
         @functools.wraps(klass)
         def partial_source(*inner_args, **inner_kwargs):
             kwargs = url_kwargs.copy()
             kwargs.update(inner_kwargs)
-            return klass(*inner_args, **kwargs)
+            return SourceWrapper._maybe_wrap(klass(*inner_args, **kwargs))
 
         return partial_source
 
     @classmethod
     def register_backend(cls, name, factory):
         """Register a new pushsource backend.
```

### Comparing `pushsource-2.8.0/src/pushsource/_impl/validator.py` & `pushsource-2.9.0/src/pushsource/_impl/validator.py`

 * *Files identical despite different names*

### Comparing `pushsource-2.8.0/src/pushsource.egg-info/PKG-INFO` & `pushsource-2.9.0/src/pushsource.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pushsource
-Version: 2.8.0
+Version: 2.9.0
 Summary: A library to load push items from a variety of sources
 Home-page: https://github.com/release-engineering/pushsource
 License: GNU General Public License
 Project-URL: Documentation, https://release-engineering.github.io/pushsource/
 Project-URL: Changelog, https://github.com/release-engineering/pushsource/blob/master/CHANGELOG.md
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -47,18 +47,17 @@
 
 ```python
 from pushsource import Source
 
 # Get a source of content; sources and their parameters can be
 # specified by URL. This source will use a couple of RPMs from
 # Fedora koji as the content source.
-source = Source.get('koji:https://koji.fedoraproject.org/kojihub?rpm=python3-3.7.5-2.fc31.x86_64.rpm,python3-3.7.5-2.fc31.src.rpm')
-
-# Iterate over the content and do something with it:
-for push_item in source:
+with Source.get('koji:https://koji.fedoraproject.org/kojihub?rpm=python3-3.7.5-2.fc31.x86_64.rpm,python3-3.7.5-2.fc31.src.rpm') as source:
+  # Iterate over the content and do something with it:
+  for push_item in source:
     publish(push_item)
 ```
 
 Development
 -----------
 
 Patches may be contributed via pull requests to
```

### Comparing `pushsource-2.8.0/src/pushsource.egg-info/SOURCES.txt` & `pushsource-2.9.0/src/pushsource.egg-info/SOURCES.txt`

 * *Files identical despite different names*

