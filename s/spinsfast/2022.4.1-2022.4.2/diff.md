# Comparing `tmp/spinsfast-2022.4.1.tar.gz` & `tmp/spinsfast-2022.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spinsfast-2022.4.1.tar", last modified: Fri Apr  1 14:36:21 2022, max compression
+gzip compressed data, was "spinsfast-2022.4.2.tar", last modified: Tue May 23 03:34:03 2023, max compression
```

## Comparing `spinsfast-2022.4.1.tar` & `spinsfast-2022.4.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 14:36:21.100908 spinsfast-2022.4.1/
--rw-r--r--   0 runner    (1001) docker     (121)    35147 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)    35122 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1130 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      547 2022-04-01 14:36:21.100908 spinsfast-2022.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6388 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/README
--rw-r--r--   0 runner    (1001) docker     (121)     6388 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 14:36:21.092908 spinsfast-2022.4.1/code/
--rw-r--r--   0 runner    (1001) docker     (121)     1412 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/code/alm.c
--rw-r--r--   0 runner    (1001) docker     (121)     2046 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/code/dump_cimage.c
--rw-r--r--   0 runner    (1001) docker     (121)     3386 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/code/healpix_convert.c
--rw-r--r--   0 runner    (1001) docker     (121)     2533 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/code/module.mk
--rw-r--r--   0 runner    (1001) docker     (121)     6141 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/code/spinsfast_backward_Gmm.c
--rw-r--r--   0 runner    (1001) docker     (121)     6398 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/code/spinsfast_backward_Gmm_alm2iqu.c
--rw-r--r--   0 runner    (1001) docker     (121)     6065 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/code/spinsfast_backward_transform.c
--rw-r--r--   0 runner    (1001) docker     (121)    12218 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/code/spinsfast_forward_Imm.c
--rw-r--r--   0 runner    (1001) docker     (121)     2607 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/code/spinsfast_forward_Jmm.c
--rw-r--r--   0 runner    (1001) docker     (121)     6201 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/code/spinsfast_forward_transform.c
--rw-r--r--   0 runner    (1001) docker     (121)     7879 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/code/spinsfast_forward_transform_eo.c
--rw-r--r--   0 runner    (1001) docker     (121)     3318 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/code/spinsfast_forward_transform_from_Imm.c
--rw-r--r--   0 runner    (1001) docker     (121)     9771 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/code/spinsfast_forward_transform_iqu2alm.c
--rw-r--r--   0 runner    (1001) docker     (121)     8235 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/code/wigner_d_halfpi_Risbo.c
--rw-r--r--   0 runner    (1001) docker     (121)     8259 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/code/wigner_d_halfpi_TN.c
--rw-r--r--   0 runner    (1001) docker     (121)     2875 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/code/wigner_d_halfpi_methods.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 14:36:21.092908 spinsfast-2022.4.1/example/
--rw-r--r--   0 runner    (1001) docker     (121)     6124 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/example/example_iqu.c
--rw-r--r--   0 runner    (1001) docker     (121)     5830 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/example/example_multispin.c
--rw-r--r--   0 runner    (1001) docker     (121)     4748 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/example/example_spin.c
--rw-r--r--   0 runner    (1001) docker     (121)     2304 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/example/example_spin.py
--rw-r--r--   0 runner    (1001) docker     (121)      459 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/example/module.mk
--rw-r--r--   0 runner    (1001) docker     (121)  1406131 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/example/spinsfast.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 14:36:21.096908 spinsfast-2022.4.1/include/
--rw-r--r--   0 runner    (1001) docker     (121)     1170 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/include/alm.h
--rw-r--r--   0 runner    (1001) docker     (121)      289 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/include/fftw.h
--rw-r--r--   0 runner    (1001) docker     (121)    31394 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/include/fftw3.h
--rw-r--r--   0 runner    (1001) docker     (121)     1589 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/include/healpix_convert.h
--rw-r--r--   0 runner    (1001) docker     (121)      223 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/include/inline.h
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/include/restrict.h
--rw-r--r--   0 runner    (1001) docker     (121)     2611 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/include/spinsfast_backward.h
--rw-r--r--   0 runner    (1001) docker     (121)     3414 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/include/spinsfast_forward.h
--rw-r--r--   0 runner    (1001) docker     (121)     1172 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/include/wigner_d_halfpi.h
--rw-r--r--   0 runner    (1001) docker     (121)     1917 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/include/wigner_d_halfpi_Risbo.h
--rw-r--r--   0 runner    (1001) docker     (121)     2648 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/include/wigner_d_halfpi_TN.h
--rw-r--r--   0 runner    (1001) docker     (121)     1611 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/include/wigner_d_halfpi_methods.h
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-04-01 14:36:09.000000 spinsfast-2022.4.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 14:36:21.096908 spinsfast-2022.4.1/python/
--rw-r--r--   0 runner    (1001) docker     (121)    11917 2022-04-01 14:36:09.000000 spinsfast-2022.4.1/python/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1624 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/python/build_macosx_wheels.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     2692 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/python/build_manylinux_wheels.sh
--rw-r--r--   0 runner    (1001) docker     (121)     9311 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/python/cextension.c
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/python/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-04-01 14:36:08.000000 spinsfast-2022.4.1/python/module.mk
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-01 14:36:21.100908 spinsfast-2022.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3449 2022-04-01 14:36:09.000000 spinsfast-2022.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 14:36:21.100908 spinsfast-2022.4.1/spinsfast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      547 2022-04-01 14:36:20.000000 spinsfast-2022.4.1/spinsfast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1256 2022-04-01 14:36:21.000000 spinsfast-2022.4.1/spinsfast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-01 14:36:20.000000 spinsfast-2022.4.1/spinsfast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-04-01 14:36:20.000000 spinsfast-2022.4.1/spinsfast.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:34:03.965162 spinsfast-2022.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)    35122 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-23 03:34:03.965162 spinsfast-2022.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/README
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:34:03.961162 spinsfast-2022.4.2/code/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/code/alm.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/code/dump_cimage.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/code/healpix_convert.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/code/module.mk
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/code/spinsfast_backward_Gmm.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/code/spinsfast_backward_Gmm_alm2iqu.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/code/spinsfast_backward_transform.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/code/spinsfast_forward_Imm.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/code/spinsfast_forward_Jmm.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/code/spinsfast_forward_transform.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/code/spinsfast_forward_transform_eo.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/code/spinsfast_forward_transform_from_Imm.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9771 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/code/spinsfast_forward_transform_iqu2alm.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/code/wigner_d_halfpi_Risbo.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/code/wigner_d_halfpi_TN.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/code/wigner_d_halfpi_methods.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:34:03.961162 spinsfast-2022.4.2/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/example/example_iqu.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/example/example_multispin.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/example/example_spin.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/example/example_spin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/example/module.mk
+-rw-r--r--   0 runner    (1001) docker     (123)  1406131 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/example/spinsfast.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:34:03.965162 spinsfast-2022.4.2/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/include/alm.h
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/include/fftw.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31394 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/include/fftw3.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/include/healpix_convert.h
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/include/inline.h
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/include/restrict.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/include/spinsfast_backward.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/include/spinsfast_forward.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/include/wigner_d_halfpi.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/include/wigner_d_halfpi_Risbo.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/include/wigner_d_halfpi_TN.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/include/wigner_d_halfpi_methods.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:34:03.965162 spinsfast-2022.4.2/python/
+-rw-r--r--   0 runner    (1001) docker     (123)    11917 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/python/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1624 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/python/build_macosx_wheels.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2692 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/python/build_manylinux_wheels.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/python/cextension.c
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/python/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/python/module.mk
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 03:34:03.965162 spinsfast-2022.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-23 03:33:58.000000 spinsfast-2022.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:34:03.965162 spinsfast-2022.4.2/spinsfast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-23 03:34:03.000000 spinsfast-2022.4.2/spinsfast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-23 03:34:03.000000 spinsfast-2022.4.2/spinsfast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 03:34:03.000000 spinsfast-2022.4.2/spinsfast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 03:34:03.000000 spinsfast-2022.4.2/spinsfast.egg-info/top_level.txt
```

### Comparing `spinsfast-2022.4.1/COPYING` & `spinsfast-2022.4.2/COPYING`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.1/LICENSE` & `spinsfast-2022.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.1/Makefile` & `spinsfast-2022.4.2/Makefile`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.1/PKG-INFO` & `spinsfast-2022.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: spinsfast
-Version: 2022.4.1
+Version: 2022.4.2
 Summary: Fast and exact spin-s spherical-harmonic transforms
 Home-page: https://github.com/moble/spinsfast
 Maintainer: Mike Boyle
 Maintainer-email: mob22@cornell.edu
 License: UNKNOWN
 Description: This module is a lightly modified version of the code originally written by Huffenberger and
         Wandelt.  It enables the user to transform between modes of a spin-weighted spherical-harmonic
```

### Comparing `spinsfast-2022.4.1/README` & `spinsfast-2022.4.2/README`

 * *Files 6% similar despite different names*

```diff
@@ -1,400 +1,429 @@
-00000000: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00000010: 2f7a 656e 6f64 6f2e 6f72 672f 6261 6467  /zenodo.org/badg
-00000020: 652f 6c61 7465 7374 646f 692f 3330 3334  e/latestdoi/3034
-00000030: 3035 3832 223e 3c69 6d67 2061 6c69 676e  0582"><img align
-00000040: 3d22 7269 6768 7422 2073 7263 3d22 6874  ="right" src="ht
-00000050: 7470 733a 2f2f 7a65 6e6f 646f 2e6f 7267  tps://zenodo.org
-00000060: 2f62 6164 6765 2f33 3033 3430 3538 322e  /badge/30340582.
-00000070: 7376 6722 2061 6c74 3d22 444f 4922 3e3c  svg" alt="DOI"><
-00000080: 2f61 3e0a 0a23 2073 7069 6e73 6661 7374  /a>..# spinsfast
-00000090: 0a46 6173 7420 616e 6420 6578 6163 7420  .Fast and exact 
-000000a0: 7370 696e 2d73 2073 7068 6572 6963 616c  spin-s spherical
-000000b0: 2d68 6172 6d6f 6e69 6320 7472 616e 7366  -harmonic transf
-000000c0: 6f72 6d73 0a0a 5468 6973 2063 6f64 6520  orms..This code 
-000000d0: 6973 2061 206c 6967 6874 6c79 206d 6f64  is a lightly mod
-000000e0: 6966 6965 6420 7665 7273 696f 6e20 6f66  ified version of
-000000f0: 2074 6865 2063 6f64 6520 686f 7374 6564   the code hosted
-00000100: 0a5b 6865 7265 5d28 6874 7470 3a2f 2f61  .[here](http://a
-00000110: 7374 726f 7068 7973 6963 732e 7068 7973  strophysics.phys
-00000120: 6963 732e 6673 752e 6564 752f 7e68 7566  ics.fsu.edu/~huf
-00000130: 6665 6e62 652f 7265 7365 6172 6368 2f73  fenbe/research/s
-00000140: 7069 6e73 6661 7374 2f69 6e64 6578 2e68  pinsfast/index.h
-00000150: 746d 6c29 0a62 7920 4875 6666 656e 6265  tml).by Huffenbe
-00000160: 7267 6572 2c20 6261 7365 6420 6f6e 2077  rger, based on w
-00000170: 6f72 6b20 6279 0a5b 4875 6666 656e 6265  ork by.[Huffenbe
-00000180: 7267 6572 2061 6e64 2057 616e 6465 6c74  rger and Wandelt
-00000190: 5d28 6874 7470 3a2f 2f73 7461 636b 732e  ](http://stacks.
-000001a0: 696f 702e 6f72 672f 3030 3637 2d30 3034  iop.org/0067-004
-000001b0: 392f 3138 392f 3235 3529 2e0a 0a4d 7920  9/189/255)...My 
-000001c0: 6d6f 6469 6669 6361 7469 6f6e 7320 6d6f  modifications mo
-000001d0: 7374 6c79 2064 6561 6c20 7769 7468 2074  stly deal with t
-000001e0: 6865 2075 7365 7220 696e 7465 7266 6163  he user interfac
-000001f0: 653a 0a0a 2020 2a20 6164 6420 606d 756c  e:..  * add `mul
-00000200: 7469 5f6d 6170 3273 616c 6d60 2061 6e64  ti_map2salm` and
-00000210: 2060 6d75 6c74 695f 7361 6c6d 326d 6170   `multi_salm2map
-00000220: 6020 666f 7220 7275 6e6e 696e 6720 6d61  ` for running ma
-00000230: 6e79 2073 696d 696c 6172 2074 7261 6e73  ny similar trans
-00000240: 666f 726d 6174 696f 6e73 2065 6666 6963  formations effic
-00000250: 6965 6e74 6c79 3b0a 2020 2a20 6372 6561  iently;.  * crea
-00000260: 7465 2070 7974 686f 6e20 7772 6170 7065  te python wrappe
-00000270: 7273 2066 6f72 2074 6865 2060 6d61 7032  rs for the `map2
-00000280: 7361 6c6d 6020 616e 6420 6073 616c 6d32  salm` and `salm2
-00000290: 6d61 7060 2066 756e 6374 696f 6e73 2074  map` functions t
-000002a0: 6f20 6465 616c 2077 6974 6820 616e 7920  o deal with any 
-000002b0: 2872 6561 736f 6e61 626c 6529 0a20 2020  (reasonable).   
-000002c0: 2074 7970 6520 6f72 2073 6861 7065 206f   type or shape o
-000002d0: 6620 696e 7075 7420 6461 7461 2c20 696e  f input data, in
-000002e0: 636c 7564 696e 6720 6d75 6c74 692d 6469  cluding multi-di
-000002f0: 6d65 6e73 696f 6e61 6c3b 0a20 202a 2061  mensional;.  * a
-00000300: 6464 2070 7974 686f 6e20 332e 7820 636f  dd python 3.x co
-00000310: 6d70 6174 6962 696c 6974 7920 746f 2060  mpatibility to `
-00000320: 7079 7468 6f6e 2f73 7069 6e73 6661 7374  python/spinsfast
-00000330: 5f6d 6f64 756c 652e 6360 3b0a 2020 2a20  _module.c`;.  * 
-00000340: 6669 7820 7365 6766 6175 6c74 7320 6475  fix segfaults du
-00000350: 6520 746f 2075 7365 206f 6620 6066 7265  e to use of `fre
-00000360: 6560 2069 6e73 7465 6164 206f 6620 6066  e` instead of `f
-00000370: 6674 775f 6672 6565 6020 7768 656e 2060  ftw_free` when `
-00000380: 6666 7477 5f6d 616c 6c6f 6360 2077 6173  fftw_malloc` was
-00000390: 2075 7365 643b 0a20 202a 206d 616b 6520   used;.  * make 
-000003a0: 6974 2065 6173 6965 7220 746f 2069 6e73  it easier to ins
-000003b0: 7461 6c6c 2061 7320 6120 7079 7468 6f6e  tall as a python
-000003c0: 206d 6f64 756c 6520 6279 2074 7279 696e   module by tryin
-000003d0: 6720 746f 2064 6574 6563 7420 7061 7468  g to detect path
-000003e0: 7320 746f 0a20 2020 2046 4654 573b 0a20  s to.    FFTW;. 
-000003f0: 202a 2066 6978 206e 756d 6572 6f75 7320   * fix numerous 
-00000400: 6d61 7373 6976 6520 6d65 6d6f 7279 206c  massive memory l
-00000410: 6561 6b73 2069 6e20 7079 7468 6f6e 2065  eaks in python e
-00000420: 7874 656e 7369 6f6e 206d 6f64 756c 653b  xtension module;
-00000430: 0a20 202a 2069 6e63 6c75 6465 2061 6e20  .  * include an 
-00000440: 6970 7974 686f 6e2f 6a75 7079 7465 7220  ipython/jupyter 
-00000450: 6e6f 7465 626f 6f6b 2069 6e20 7468 6520  notebook in the 
-00000460: 6065 7861 6d70 6c65 6020 6469 7265 6374  `example` direct
-00000470: 6f72 793b 0a20 202a 2061 6464 2069 6e74  ory;.  * add int
-00000480: 6567 7261 7469 6f6e 2077 6974 6820 5b70  egration with [p
-00000490: 6970 5d28 6874 7470 733a 2f2f 7079 7069  ip](https://pypi
-000004a0: 2e70 7974 686f 6e2e 6f72 672f 7079 7069  .python.org/pypi
-000004b0: 2f70 6970 290a 2020 2020 616e 6420 5b70  /pip).    and [p
-000004c0: 7970 695d 2868 7474 7073 3a2f 2f70 7970  ypi](https://pyp
-000004d0: 692e 7079 7468 6f6e 2e6f 7267 2f70 7970  i.python.org/pyp
-000004e0: 692f 7370 696e 7366 6173 7429 2c20 666f  i/spinsfast), fo
-000004f0: 7220 6561 7379 2069 6e73 7461 6c6c 6174  r easy installat
-00000500: 696f 6e0a 2020 2020 285b 7365 6520 6265  ion.    ([see be
-00000510: 6c6f 775d 2823 696e 7374 616c 6c61 7469  low](#installati
-00000520: 6f6e 2929 3b0a 2020 2a20 6164 6420 696e  on));.  * add in
-00000530: 7465 6772 6174 696f 6e20 7769 7468 205b  tegration with [
-00000540: 636f 6e64 615d 2868 7474 7073 3a2f 2f63  conda](https://c
-00000550: 6f6e 6461 2e69 6f2f 646f 6373 2f29 0a20  onda.io/docs/). 
-00000560: 2020 2061 6e64 205b 616e 6163 6f6e 6461     and [anaconda
-00000570: 2e6f 7267 5d28 6874 7470 733a 2f2f 616e  .org](https://an
-00000580: 6163 6f6e 6461 2e6f 7267 2f6d 6f62 6c65  aconda.org/moble
-00000590: 2f73 7069 6e73 6661 7374 292c 2066 6f72  /spinsfast), for
-000005a0: 2065 6173 6965 7374 2069 6e73 7461 6c6c   easiest install
-000005b0: 6174 696f 6e0a 2020 2020 285b 7365 6520  ation.    ([see 
-000005c0: 6265 6c6f 775d 2823 696e 7374 616c 6c61  below](#installa
-000005d0: 7469 6f6e 2929 2e0a 0a23 204c 6963 656e  tion))...# Licen
-000005e0: 7365 0a0a 5468 6520 6f72 6967 696e 616c  se..The original
-000005f0: 2077 6f72 6b20 6973 206c 6963 656e 7365   work is license
-00000600: 6420 756e 6465 7220 4750 4c2c 2073 6f20  d under GPL, so 
-00000610: 7468 6174 2773 2077 6861 7420 4920 6861  that's what I ha
-00000620: 7665 2074 6f20 6c69 6365 6e73 6520 7468  ve to license th
-00000630: 6973 0a75 6e64 6572 2061 7320 7765 6c6c  is.under as well
-00000640: 2e20 2028 4920 7573 7561 6c6c 7920 676f  .  (I usually go
-00000650: 2066 6f72 2074 6865 206d 6f72 6520 6c69   for the more li
-00000660: 6265 7261 6c20 4d49 5420 6c69 6365 6e73  beral MIT licens
-00000670: 652c 2062 7574 2047 504c 2069 730a 6669  e, but GPL is.fi
-00000680: 6e65 2e29 2020 5365 6520 7468 6520 604c  ne.)  See the `L
-00000690: 4943 454e 5345 6020 6669 6c65 2069 6e20  ICENSE` file in 
-000006a0: 7468 6973 2064 6972 6563 746f 7279 2066  this directory f
-000006b0: 6f72 206d 6f72 6520 6465 7461 696c 732e  or more details.
-000006c0: 0a0a 4920 6261 7365 6420 6d79 2077 6f72  ..I based my wor
-000006d0: 6b20 6f6e 2048 7566 6665 6e62 6572 6765  k on Huffenberge
-000006e0: 7220 616e 6420 5761 6e64 656c 7427 7320  r and Wandelt's 
-000006f0: 2252 6576 6973 696f 6e20 3130 342c 2031  "Revision 104, 1
-00000700: 3320 4170 7220 3230 3132 222c 0a77 6869  3 Apr 2012",.whi
-00000710: 6368 2069 7320 6375 7272 656e 7420 6173  ch is current as
-00000720: 206f 6620 7468 6973 2077 7269 7469 6e67   of this writing
-00000730: 2028 4175 6775 7374 2032 3031 3529 2e20   (August 2015). 
-00000740: 2057 6865 6e65 7665 7220 4920 6e6f 7469   Whenever I noti
-00000750: 6365 2075 7064 6174 6573 0a6f 6e20 7468  ce updates.on th
-00000760: 6569 7220 656e 642c 2049 2077 696c 6c20  eir end, I will 
-00000770: 676c 6164 6c79 2075 7064 6174 6520 7468  gladly update th
-00000780: 6973 2063 6f64 652c 2073 6f20 6665 656c  is code, so feel
-00000790: 2066 7265 6520 746f 206f 7065 6e20 616e   free to open an
-000007a0: 0a5b 6973 7375 655d 2868 7474 7073 3a2f  .[issue](https:/
-000007b0: 2f67 6974 6875 622e 636f 6d2f 6d6f 626c  /github.com/mobl
-000007c0: 652f 7370 696e 7366 6173 742f 6973 7375  e/spinsfast/issu
-000007d0: 6573 2920 746f 206e 6f74 6966 7920 6d65  es) to notify me
-000007e0: 2e20 2054 6f20 7365 6520 6d6f 7265 0a73  .  To see more.s
-000007f0: 7065 6369 6669 6361 6c6c 7920 7768 6174  pecifically what
-00000800: 2049 2776 6520 6164 6465 642c 206c 6f6f   I've added, loo
-00000810: 6b20 7468 726f 7567 6820 7468 650a 5b63  k through the.[c
-00000820: 6f6d 6d69 7473 5d28 6874 7470 733a 2f2f  ommits](https://
-00000830: 6769 7468 7562 2e63 6f6d 2f6d 6f62 6c65  github.com/moble
-00000840: 2f73 7069 6e73 6661 7374 2f63 6f6d 6d69  /spinsfast/commi
-00000850: 7473 2f6d 6173 7465 7229 3b20 6d79 2063  ts/master); my c
-00000860: 6f6e 7472 6962 7574 696f 6e73 0a61 7265  ontributions.are
-00000870: 206a 7573 7420 6576 6572 7974 6869 6e67   just everything
-00000880: 2073 696e 6365 2074 6865 2069 6e69 7469   since the initi
-00000890: 616c 2063 6f6d 6d69 742e 0a0a 0a23 2045  al commit....# E
-000008a0: 7861 6d70 6c65 2055 7361 6765 0a0a 4120  xample Usage..A 
-000008b0: 636f 6e76 656e 6965 6e74 2069 7079 7468  convenient ipyth
-000008c0: 6f6e 2f6a 7570 7974 6572 206e 6f74 6562  on/jupyter noteb
-000008d0: 6f6f 6b20 6973 2066 6f75 6e64 2069 6e20  ook is found in 
-000008e0: 7468 6520 6065 7861 6d70 6c65 6020 6469  the `example` di
-000008f0: 7265 6374 6f72 792c 2061 6e64 0a63 616e  rectory, and.can
-00000900: 2061 6c73 6f20 6265 0a5b 7669 6577 6564   also be.[viewed
-00000910: 2064 6972 6563 746c 7920 6f6e 6c69 6e65   directly online
-00000920: 5d28 6874 7470 3a2f 2f6e 6276 6965 7765  ](http://nbviewe
-00000930: 722e 6970 7974 686f 6e2e 6f72 672f 6769  r.ipython.org/gi
-00000940: 7468 7562 2f6d 6f62 6c65 2f73 7069 6e73  thub/moble/spins
-00000950: 6661 7374 2f62 6c6f 622f 6d61 7374 6572  fast/blob/master
-00000960: 2f65 7861 6d70 6c65 2f73 7069 6e73 6661  /example/spinsfa
-00000970: 7374 2e69 7079 6e62 292e 0a49 7420 7368  st.ipynb)..It sh
-00000980: 6f77 7320 736f 6d65 2065 7861 6d70 6c65  ows some example
-00000990: 2070 7974 686f 6e20 636f 6465 2074 6861   python code tha
-000009a0: 7420 6361 6e20 6265 2075 7365 6420 746f  t can be used to
-000009b0: 2072 756e 2074 6869 7320 6d6f 6475 6c65   run this module
-000009c0: 2c20 616e 640a 6578 706c 6169 6e73 2073  , and.explains s
-000009d0: 6f6d 6520 6f66 2074 6865 2063 6f6e 7665  ome of the conve
-000009e0: 6e74 696f 6e73 2065 7374 6162 6c69 7368  ntions establish
-000009f0: 6564 2062 7920 7468 6520 6073 7069 6e73  ed by the `spins
-00000a00: 6661 7374 6020 6175 7468 6f72 732e 0a0a  fast` authors...
-00000a10: 496e 2074 6865 2069 6e74 6572 6573 7473  In the interests
-00000a20: 206f 6620 6120 7665 7279 2073 686f 7274   of a very short
-00000a30: 2c20 6578 706c 6963 6974 2065 7861 6d70  , explicit examp
-00000a40: 6c65 2c20 6865 7265 2069 7320 6f6e 6520  le, here is one 
-00000a50: 7573 696e 6720 7261 6e64 6f6d 2060 2865  using random `(e
-00000a60: 6c6c 2c6d 2960 206d 6f64 6573 3a0a 0a60  ll,m)` modes:..`
-00000a70: 6060 7079 7468 6f6e 0a66 726f 6d20 6e75  ``python.from nu
-00000a80: 6d70 792e 7261 6e64 6f6d 2069 6d70 6f72  mpy.random impor
-00000a90: 7420 6e6f 726d 616c 2c20 7365 6564 0a69  t normal, seed.i
-00000aa0: 6d70 6f72 7420 7370 696e 7366 6173 740a  mport spinsfast.
-00000ab0: 0a23 2053 6f6d 6520 626f 696c 6572 706c  .# Some boilerpl
-00000ac0: 6174 6520 666f 7220 7365 7474 696e 6720  ate for setting 
-00000ad0: 7468 696e 6773 2075 703a 0a73 203d 2031  things up:.s = 1
-00000ae0: 2020 2320 7370 696e 2077 6569 6768 7420    # spin weight 
-00000af0: 6f66 2074 6865 2066 6965 6c64 0a6c 6d61  of the field.lma
-00000b00: 7820 3d20 3820 2023 206d 6178 696d 756d  x = 8  # maximum
-00000b10: 2065 6c6c 2076 616c 7565 2075 7365 640a   ell value used.
-00000b20: 4e74 6865 7461 203d 2032 2a6c 6d61 782b  Ntheta = 2*lmax+
-00000b30: 3120 2023 204d 696e 696d 756d 2076 616c  1  # Minimum val
-00000b40: 7565 2066 6f72 2061 6363 7572 6163 790a  ue for accuracy.
-00000b50: 4e70 6869 203d 2032 2a6c 6d61 782b 3120  Nphi = 2*lmax+1 
-00000b60: 2023 204d 696e 696d 756d 2076 616c 7565   # Minimum value
-00000b70: 2066 6f72 2061 6363 7572 6163 790a 4e6c   for accuracy.Nl
-00000b80: 6d20 3d20 7370 696e 7366 6173 742e 4e5f  m = spinsfast.N_
-00000b90: 6c6d 286c 6d61 7829 3b20 2023 2054 6f74  lm(lmax);  # Tot
-00000ba0: 616c 206e 756d 6265 7220 6f66 2063 6f6d  al number of com
-00000bb0: 706c 6578 2063 6f6d 706f 6e65 6e74 7320  plex components 
-00000bc0: 6f66 2074 6865 206d 6f64 6520 6465 636f  of the mode deco
-00000bd0: 6d70 6f73 6974 696f 6e0a 0a23 2060 616c  mposition..# `al
-00000be0: 6d60 2077 696c 6c20 686f 6c64 2074 6865  m` will hold the
-00000bf0: 206d 6f64 6520 636f 6d70 6f6e 656e 7473   mode components
-00000c00: 2061 7320 6469 7363 7573 7365 6420 696e   as discussed in
-00000c10: 2060 6578 616d 706c 652f 7370 696e 7366   `example/spinsf
-00000c20: 6173 742e 6970 796e 6260 0a23 2048 6572  ast.ipynb`.# Her
-00000c30: 6520 7765 206a 7573 7420 6669 6c6c 2069  e we just fill i
-00000c40: 7420 7769 7468 2073 6f6d 6520 7261 6e64  t with some rand
-00000c50: 6f6d 206e 756d 6265 7273 2074 6f20 7465  om numbers to te
-00000c60: 7374 2069 740a 7365 6564 2833 3132 3434  st it.seed(31244
-00000c70: 3332 2920 2023 2053 6565 6420 7468 6520  32)  # Seed the 
-00000c80: 7261 6e64 6f6d 2d6e 756d 6265 7220 6765  random-number ge
-00000c90: 6e65 7261 746f 722c 2066 6f72 2072 6570  nerator, for rep
-00000ca0: 726f 6475 6369 6269 6c69 7479 0a61 6c6d  roducibility.alm
-00000cb0: 203d 206e 6f72 6d61 6c28 7369 7a65 3d28   = normal(size=(
-00000cc0: 4e6c 6d2c 2929 202b 2031 6a2a 6e6f 726d  Nlm,)) + 1j*norm
-00000cd0: 616c 2873 697a 653d 284e 6c6d 2c29 290a  al(size=(Nlm,)).
-00000ce0: 0a23 2054 6869 7320 6973 2074 6865 206b  .# This is the k
-00000cf0: 6579 206c 696e 652c 2077 6865 7265 2073  ey line, where s
-00000d00: 7069 6e73 6661 7374 2063 6f6e 7665 7274  pinsfast convert
-00000d10: 7320 6672 6f6d 2028 656c 6c2c 6d29 206d  s from (ell,m) m
-00000d20: 6f64 6573 2074 6f20 7661 6c75 6573 2069  odes to values i
-00000d30: 6e20 7068 7973 6963 616c 2073 7061 6365  n physical space
-00000d40: 0a66 203d 2020 7370 696e 7366 6173 742e  .f =  spinsfast.
-00000d50: 7361 6c6d 326d 6170 2861 6c6d 2c73 2c6c  salm2map(alm,s,l
-00000d60: 6d61 782c 4e74 6865 7461 2c4e 7068 6929  max,Ntheta,Nphi)
-00000d70: 0a0a 2320 5765 2063 616e 2061 6c73 6f20  ..# We can also 
-00000d80: 636f 6e76 6572 7420 696e 2074 6865 206f  convert in the o
-00000d90: 7070 6f73 6974 6520 6469 7265 6374 696f  pposite directio
-00000da0: 6e20 6c69 6b65 2074 6869 733a 0a61 6c6d  n like this:.alm
-00000db0: 3220 3d20 7370 696e 7366 6173 742e 6d61  2 = spinsfast.ma
-00000dc0: 7032 7361 6c6d 2866 2c73 2c6c 6d61 7829  p2salm(f,s,lmax)
-00000dd0: 0a60 6060 0a0a 0a23 2049 6e73 7461 6c6c  .```...# Install
-00000de0: 6174 696f 6e0a 0a23 2320 416e 6163 6f6e  ation..## Anacon
-00000df0: 6461 0a0a 5468 6f75 6768 206d 616e 7561  da..Though manua
-00000e00: 6c20 696e 7374 616c 6c61 7469 6f6e 2069  l installation i
-00000e10: 7320 706f 7373 6962 6c65 2c20 7468 6520  s possible, the 
-00000e20: 6265 7374 2077 6179 2062 7920 6661 7220  best way by far 
-00000e30: 746f 2073 6174 6973 6679 2074 6865 7365  to satisfy these
-00000e40: 0a64 6570 656e 6465 6e63 6965 7320 6973  .dependencies is
-00000e50: 2074 6f20 7573 6520 7468 6520 5b60 616e   to use the [`an
-00000e60: 6163 6f6e 6461 605d 2868 7474 703a 2f2f  aconda`](http://
-00000e70: 636f 6e74 696e 7575 6d2e 696f 2f64 6f77  continuum.io/dow
-00000e80: 6e6c 6f61 6473 290a 6469 7374 7269 6275  nloads).distribu
-00000e90: 7469 6f6e 2e20 2054 6869 7320 6469 7374  tion.  This dist
-00000ea0: 7269 6275 7469 6f6e 2063 616e 2063 6f2d  ribution can co-
-00000eb0: 6578 6973 7420 7769 7468 2079 6f75 7220  exist with your 
-00000ec0: 7379 7374 656d 2070 7974 686f 6e20 7769  system python wi
-00000ed0: 7468 206e 6f0a 7472 6f75 626c 6520 2d2d  th no.trouble --
-00000ee0: 2079 6f75 2073 696d 706c 7920 6164 6420   you simply add 
-00000ef0: 7468 6520 7061 7468 2074 6f20 616e 6163  the path to anac
-00000f00: 6f6e 6461 2062 6566 6f72 6520 796f 7572  onda before your
-00000f10: 2073 7973 7465 6d20 6578 6563 7574 6162   system executab
-00000f20: 6c65 732e 0a49 7420 696e 7374 616c 6c73  les..It installs
-00000f30: 2069 6e74 6f20 796f 7572 2068 6f6d 6520   into your home 
-00000f40: 6469 7265 6374 6f72 792c 2073 6f20 6974  directory, so it
-00000f50: 2064 6f65 736e 2774 2072 6571 7569 7265   doesn't require
-00000f60: 2072 6f6f 7420 6163 6365 7373 2e20 2049   root access.  I
-00000f70: 740a 6361 6e20 6265 2075 6e69 6e73 7461  t.can be uninsta
-00000f80: 6c6c 6564 2065 6173 696c 792c 2073 696e  lled easily, sin
-00000f90: 6365 2069 7420 6578 6973 7473 2065 6e74  ce it exists ent
-00000fa0: 6972 656c 7920 696e 7369 6465 2069 7473  irely inside its
-00000fb0: 206f 776e 2064 6972 6563 746f 7279 2e0a   own directory..
-00000fc0: 416e 6420 7570 6461 7465 7320 6172 6520  And updates are 
-00000fd0: 7472 6976 6961 6c2e 0a0a 4f6e 6365 2060  trivial...Once `
-00000fe0: 616e 6163 6f6e 6461 6020 6973 2069 6e73  anaconda` is ins
-00000ff0: 7461 6c6c 6564 2c20 7468 6973 2070 6163  talled, this pac
-00001000: 6b61 6765 206d 6179 2062 6520 696e 7374  kage may be inst
-00001010: 616c 6c65 6420 7769 7468 2074 6865 2063  alled with the c
-00001020: 6f6d 6d61 6e64 0a0a 6060 6062 6173 680a  ommand..```bash.
-00001030: 636f 6e64 6120 696e 7374 616c 6c20 2d2d  conda install --
-00001040: 6368 616e 6e65 6c20 636f 6e64 612d 666f  channel conda-fo
-00001050: 7267 6520 7370 696e 7366 6173 740a 6060  rge spinsfast.``
-00001060: 600a 0a4e 6f74 6520 7468 6973 206d 6179  `..Note this may
-00001070: 2061 6c73 6f20 696e 7374 616c 6c20 606e   also install `n
-00001080: 756d 7079 6020 616e 6420 6066 6674 7760  umpy` and `fftw`
-00001090: 2061 7574 6f6d 6174 6963 616c 6c79 2e0a   automatically..
-000010a0: 0a0a 2323 2050 6970 0a0a 5768 696c 6520  ..## Pip..While 
-000010b0: 6765 6e65 7261 6c6c 7920 6c65 7373 2072  generally less r
-000010c0: 6f62 7573 742c 2074 6869 7320 7061 636b  obust, this pack
-000010d0: 6167 6520 6973 2061 6c73 6f20 6176 6169  age is also avai
-000010e0: 6c61 626c 6520 7669 6120 6070 6970 603a  lable via `pip`:
-000010f0: 0a0a 6060 6062 6173 680a 7069 7020 696e  ..```bash.pip in
-00001100: 7374 616c 6c20 7370 696e 7366 6173 740a  stall spinsfast.
-00001110: 6060 600a 0a55 6e66 6f72 7475 6e61 7465  ```..Unfortunate
-00001120: 6c79 2c20 6d61 696e 7461 696e 696e 6720  ly, maintaining 
-00001130: 6269 6e61 7279 2064 6973 7472 6962 7574  binary distribut
-00001140: 696f 6e73 206f 6e20 7069 7020 6973 2074  ions on pip is t
-00001150: 6f6f 2074 696d 652d 636f 6e73 756d 696e  oo time-consumin
-00001160: 672c 2073 6f20 6070 6970 6020 7769 6c6c  g, so `pip` will
-00001170: 2074 7279 2074 6f0a 636f 6d70 696c 6520   try to.compile 
-00001180: 7468 6520 736f 7572 6365 2063 6f64 6520  the source code 
-00001190: 666f 7220 796f 752c 2069 6e20 7768 6963  for you, in whic
-000011a0: 6820 6361 7365 2079 6f75 2077 696c 6c20  h case you will 
-000011b0: 6e65 6564 2074 6f20 6861 7665 2046 4654  need to have FFT
-000011c0: 5720 616e 6420 6120 636f 6d70 696c 6572  W and a compiler
-000011d0: 2069 6e73 7461 6c6c 6564 2e0a 556e 666f   installed..Unfo
-000011e0: 7274 756e 6174 656c 792c 2060 7069 7060  rtunately, `pip`
-000011f0: 2068 6173 206e 6f20 676f 6f64 2077 6179   has no good way
-00001200: 206f 6620 6861 6e64 6c69 6e67 2074 6865   of handling the
-00001210: 7365 2064 6570 656e 6465 6e63 6965 732e  se dependencies.
-00001220: 2020 5365 6520 6265 6c6f 7720 666f 7220    See below for 
-00001230: 656e 7669 726f 6e6d 656e 740a 7661 7269  environment.vari
-00001240: 6162 6c65 7320 796f 7520 6d61 7920 6e65  ables you may ne
-00001250: 6564 2074 6f20 7365 7420 746f 2067 6574  ed to set to get
-00001260: 2063 6f6d 7069 6c61 7469 6f6e 2077 6f72   compilation wor
-00001270: 6b69 6e67 2070 726f 7065 726c 792e 0a0a  king properly...
-00001280: 0a23 2320 4d61 6e75 616c 2069 6e73 7461  .## Manual insta
-00001290: 6c6c 6174 696f 6e0a 0a4d 616e 7561 6c20  llation..Manual 
-000012a0: 696e 7374 616c 6c61 7469 6f6e 206f 6620  installation of 
-000012b0: 7468 6973 2070 6163 6b61 6765 2069 7320  this package is 
-000012c0: 736c 6967 6874 6c79 206d 6f72 6520 6465  slightly more de
-000012d0: 6c69 6361 7465 2e20 2054 6865 0a5b 4646  licate.  The.[FF
-000012e0: 5457 2070 6163 6b61 6765 5d28 6874 7470  TW package](http
-000012f0: 3a2f 2f77 7777 2e66 6674 772e 6f72 672f  ://www.fftw.org/
-00001300: 2920 6d75 7374 2062 6520 696e 7374 616c  ) must be instal
-00001310: 6c65 6420 6669 7273 742e 2020 5468 6973  led first.  This
-00001320: 2069 7320 7573 7561 6c6c 790a 7665 7279   is usually.very
-00001330: 2073 696d 706c 652e 2020 4275 7420 7468   simple.  But th
-00001340: 6520 7265 7375 6c74 696e 6720 6865 6164  e resulting head
-00001350: 6572 2061 6e64 206c 6962 7261 7279 206d  er and library m
-00001360: 7573 7420 6265 2066 6f75 6e64 2062 7920  ust be found by 
-00001370: 7468 650a 636f 6d70 696c 6174 696f 6e20  the.compilation 
-00001380: 7374 6570 2066 6f72 2074 6869 7320 7061  step for this pa
-00001390: 636b 6167 652e 2020 596f 7520 6361 6e20  ckage.  You can 
-000013a0: 6669 7273 7420 7369 6d70 6c79 2074 7279  first simply try
-000013b0: 2074 6f20 7275 6e0a 0a60 6060 6261 7368   to run..```bash
-000013c0: 0a70 7974 686f 6e20 7365 7475 702e 7079  .python setup.py
-000013d0: 2069 6e73 7461 6c6c 0a60 6060 0a0a 6672   install.```..fr
-000013e0: 6f6d 2074 6865 2074 6f70 2064 6972 6563  om the top direc
-000013f0: 746f 7279 206f 6620 7468 6520 6073 7069  tory of the `spi
-00001400: 6e73 6661 7374 6020 636f 6465 2e0a 0a49  nsfast` code...I
-00001410: 6620 7468 6973 2064 6f65 736e 2774 2077  f this doesn't w
-00001420: 6f72 6b2c 2079 6f75 2063 616e 2072 6561  ork, you can rea
-00001430: 6420 7468 6520 6572 726f 7220 6d65 7373  d the error mess
-00001440: 6167 652c 2062 7574 2074 6865 206d 6f73  age, but the mos
-00001450: 7420 6c69 6b65 6c79 0a70 726f 626c 656d  t likely.problem
-00001460: 2069 7320 7468 6174 2074 6865 2063 6f6d   is that the com
-00001470: 7069 6c65 7220 6361 6e6e 6f74 2066 696e  piler cannot fin
-00001480: 6420 7468 6520 6066 6674 7760 2068 6561  d the `fftw` hea
-00001490: 6465 722c 206f 7220 7468 6520 6c69 6e6b  der, or the link
-000014a0: 6572 0a63 616e 6e6f 7420 6669 6e64 2074  er.cannot find t
-000014b0: 6865 2060 6666 7477 6020 6c69 6272 6172  he `fftw` librar
-000014c0: 792e 2020 546f 2073 6f6c 7665 2074 6865  y.  To solve the
-000014d0: 7365 2070 726f 626c 656d 732c 2079 6f75  se problems, you
-000014e0: 2077 696c 6c20 6e65 6564 2074 6f20 7275   will need to ru
-000014f0: 6e0a 736f 6d65 7468 696e 6720 6d6f 7265  n.something more
-00001500: 206c 696b 6520 7468 6973 3a0a 0a60 6060   like this:..```
-00001510: 6261 7368 0a65 7870 6f72 7420 4c49 4252  bash.export LIBR
-00001520: 4152 595f 5041 5448 3d2f 7061 7468 2f74  ARY_PATH=/path/t
-00001530: 6f2f 6666 7477 2f6c 6962 0a65 7870 6f72  o/fftw/lib.expor
-00001540: 7420 435f 494e 434c 5544 455f 5041 5448  t C_INCLUDE_PATH
-00001550: 3d2f 7061 7468 2f74 6f2f 6666 7477 2f69  =/path/to/fftw/i
-00001560: 6e63 6c75 6465 0a70 7974 686f 6e20 7365  nclude.python se
-00001570: 7475 702e 7079 2069 6e73 7461 6c6c 0a60  tup.py install.`
-00001580: 6060 0a0a 416c 7465 726e 6174 6976 656c  ``..Alternativel
-00001590: 792c 2079 6f75 2063 6f75 6c64 2074 7279  y, you could try
-000015a0: 2074 6f20 616c 7465 7220 6073 6574 7570   to alter `setup
-000015b0: 2e70 7960 2074 6f20 706f 696e 7420 746f  .py` to point to
-000015c0: 2074 6865 2072 6967 6874 0a70 6174 6873   the right.paths
-000015d0: 2e0a 0a0a 2320 4f72 6967 696e 616c 2069  ....# Original i
-000015e0: 6e73 7461 6c6c 6174 696f 6e20 696e 7374  nstallation inst
-000015f0: 7275 6374 696f 6e73 0a0a 5468 6f75 6768  ructions..Though
-00001600: 2074 6865 7365 2061 7265 206e 6f74 206e   these are not n
-00001610: 6563 6573 7361 7279 2066 6f72 2069 6e73  ecessary for ins
-00001620: 7461 6c6c 696e 6720 7468 6520 7079 7468  talling the pyth
-00001630: 6f6e 206d 6f64 756c 652c 2074 6865 2066  on module, the f
-00001640: 6f6c 6c6f 7769 6e67 0a61 7265 2074 6865  ollowing.are the
-00001650: 2069 6e73 7472 7563 7469 6f6e 7320 696e   instructions in
-00001660: 2074 6865 206f 7269 6769 6e61 6c20 736f   the original so
-00001670: 7572 6365 2063 6f64 6520 666f 7220 6275  urce code for bu
-00001680: 696c 6469 6e67 2074 6865 2043 2063 6f64  ilding the C cod
-00001690: 652e 0a0a 4765 7420 7468 6520 6c61 7465  e...Get the late
-000016a0: 7374 2076 6572 7369 6f6e 2061 743a 0a0a  st version at:..
-000016b0: 2020 2020 6874 7470 3a2f 2f77 7777 2e70      http://www.p
-000016c0: 6879 7369 6373 2e6d 6961 6d69 2e65 6475  hysics.miami.edu
-000016d0: 2f7e 6875 6666 656e 6265 2f72 6573 6561  /~huffenbe/resea
-000016e0: 7263 682f 7370 696e 7366 6173 742f 0a0a  rch/spinsfast/..
-000016f0: 2323 2043 6f6d 7069 6c61 7469 6f6e 2069  ## Compilation i
-00001700: 6e73 7472 7563 7469 6f6e 730a 0a20 2031  nstructions..  1
-00001710: 2e20 4564 6974 2074 6865 2066 696c 6520  . Edit the file 
-00001720: 286f 7220 6d61 6b65 2061 206e 6577 2066  (or make a new f
-00001730: 696c 6529 2063 616c 6c65 6420 6275 696c  ile) called buil
-00001740: 642f 636f 6e66 6967 2e6d 6b20 736f 2074  d/config.mk so t
-00001750: 6861 7420 7468 6520 7072 6f70 6572 206c  hat the proper l
-00001760: 6f63 6174 696f 6e73 2066 6f72 2068 6561  ocations for hea
-00001770: 6465 7220 616e 6420 6c69 6272 6172 7920  der and library 
-00001780: 6669 6c65 7320 6172 6520 696e 636c 7564  files are includ
-00001790: 6564 2e0a 0a20 2032 2e20 5365 7420 7468  ed...  2. Set th
-000017a0: 6520 656e 7669 726f 6e6d 656e 7420 7661  e environment va
-000017b0: 7269 6162 6c65 2022 6275 696c 6422 2073  riable "build" s
-000017c0: 6f20 7468 6174 2069 7420 706f 696e 7473  o that it points
-000017d0: 2074 6f20 7468 6174 2066 696c 652e 2049   to that file. I
-000017e0: 2e65 2e2c 2069 6e20 6261 7368 2c20 7361  .e., in bash, sa
-000017f0: 790a 0a20 2020 2020 2020 2065 7870 6f72  y..        expor
-00001800: 7420 6275 696c 643d 6275 696c 642f 636f  t build=build/co
-00001810: 6e66 6967 2e6d 6b20 0a0a 2020 332e 2042  nfig.mk ..  3. B
-00001820: 7569 6c64 2074 6865 206c 6962 7261 7279  uild the library
-00001830: 2061 6e64 2065 7861 6d70 6c65 2063 6f64   and example cod
-00001840: 6573 2077 6974 6820 0a0a 2020 2020 2020  es with ..      
-00001850: 2020 6d61 6b65 0a0a 2323 2028 4f70 7469    make..## (Opti
-00001860: 6f6e 616c 2920 4368 6563 6b69 6e67 2074  onal) Checking t
-00001870: 6865 2063 6f6d 7069 6c61 7469 6f6e 0a0a  he compilation..
-00001880: 5275 6e20 7468 6520 6578 616d 706c 6520  Run the example 
-00001890: 636f 6465 2066 6f6c 6c6f 7769 6e67 2074  code following t
-000018a0: 6865 2069 6e73 7472 7563 7469 6f6e 7320  he instructions 
-000018b0: 6174 200a 0a20 2020 2068 7474 703a 2f2f  at ..    http://
-000018c0: 7777 772e 7068 7973 6963 732e 6d69 616d  www.physics.miam
-000018d0: 692e 6564 752f 7e68 7566 6665 6e62 652f  i.edu/~huffenbe/
-000018e0: 7265 7365 6172 6368 2f73 7069 6e73 6661  research/spinsfa
-000018f0: 7374 2f0a                                st/.
+00000000: 5b21 5b42 7569 6c64 5d28 6874 7470 733a  [![Build](https:
+00000010: 2f2f 6769 7468 7562 2e63 6f6d 2f6d 6f62  //github.com/mob
+00000020: 6c65 2f73 7069 6e73 6661 7374 2f61 6374  le/spinsfast/act
+00000030: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f62  ions/workflows/b
+00000040: 7569 6c64 2e79 6d6c 2f62 6164 6765 2e73  uild.yml/badge.s
+00000050: 7667 295d 2868 7474 7073 3a2f 2f67 6974  vg)](https://git
+00000060: 6875 622e 636f 6d2f 6d6f 626c 652f 7370  hub.com/moble/sp
+00000070: 696e 7366 6173 742f 6163 7469 6f6e 732f  insfast/actions/
+00000080: 776f 726b 666c 6f77 732f 6275 696c 642e  workflows/build.
+00000090: 796d 6c29 0a5b 215b 5079 5049 2056 6572  yml).[![PyPI Ver
+000000a0: 7369 6f6e 5d28 6874 7470 733a 2f2f 696d  sion](https://im
+000000b0: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
+000000c0: 692f 762f 7370 696e 7366 6173 743f 636f  i/v/spinsfast?co
+000000d0: 6c6f 723d 295d 2868 7474 7073 3a2f 2f70  lor=)](https://p
+000000e0: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
+000000f0: 7370 696e 7366 6173 742f 290a 5b21 5b43  spinsfast/).[![C
+00000100: 6f6e 6461 2056 6572 7369 6f6e 5d28 6874  onda Version](ht
+00000110: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000120: 732e 696f 2f63 6f6e 6461 2f76 6e2f 636f  s.io/conda/vn/co
+00000130: 6e64 612d 666f 7267 652f 7370 696e 7366  nda-forge/spinsf
+00000140: 6173 742e 7376 673f 636f 6c6f 723d 295d  ast.svg?color=)]
+00000150: 2868 7474 7073 3a2f 2f61 6e61 636f 6e64  (https://anacond
+00000160: 612e 6f72 672f 636f 6e64 612d 666f 7267  a.org/conda-forg
+00000170: 652f 7370 696e 7366 6173 7429 0a5b 215b  e/spinsfast).[![
+00000180: 4750 4c2d 332e 3020 4c69 6365 6e73 655d  GPL-3.0 License]
+00000190: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+000001a0: 656c 6473 2e69 6f2f 6769 7468 7562 2f6c  elds.io/github/l
+000001b0: 6963 656e 7365 2f6d 6f62 6c65 2f73 7069  icense/moble/spi
+000001c0: 6e73 6661 7374 2e73 7667 295d 2868 7474  nsfast.svg)](htt
+000001d0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000001e0: 6d6f 626c 652f 7370 696e 7366 6173 742f  moble/spinsfast/
+000001f0: 626c 6f62 2f6d 6169 6e2f 4c49 4345 4e53  blob/main/LICENS
+00000200: 4529 0a5b 215b 444f 495d 2868 7474 7073  E).[![DOI](https
+00000210: 3a2f 2f7a 656e 6f64 6f2e 6f72 672f 6261  ://zenodo.org/ba
+00000220: 6467 652f 3330 3334 3035 3832 2e73 7667  dge/30340582.svg
+00000230: 295d 2868 7474 7073 3a2f 2f7a 656e 6f64  )](https://zenod
+00000240: 6f2e 6f72 672f 6261 6467 652f 6c61 7465  o.org/badge/late
+00000250: 7374 646f 692f 3330 3334 3035 3832 290a  stdoi/30340582).
+00000260: 0a23 2073 7069 6e73 6661 7374 0a46 6173  .# spinsfast.Fas
+00000270: 7420 616e 6420 6578 6163 7420 7370 696e  t and exact spin
+00000280: 2d73 2073 7068 6572 6963 616c 2d68 6172  -s spherical-har
+00000290: 6d6f 6e69 6320 7472 616e 7366 6f72 6d73  monic transforms
+000002a0: 0a0a 5468 6973 2063 6f64 6520 6973 2061  ..This code is a
+000002b0: 206c 6967 6874 6c79 206d 6f64 6966 6965   lightly modifie
+000002c0: 6420 7665 7273 696f 6e20 6f66 2074 6865  d version of the
+000002d0: 2063 6f64 6520 686f 7374 6564 0a5b 6865   code hosted.[he
+000002e0: 7265 5d28 6874 7470 3a2f 2f61 7374 726f  re](http://astro
+000002f0: 7068 7973 6963 732e 7068 7973 6963 732e  physics.physics.
+00000300: 6673 752e 6564 752f 7e68 7566 6665 6e62  fsu.edu/~huffenb
+00000310: 652f 7265 7365 6172 6368 2f73 7069 6e73  e/research/spins
+00000320: 6661 7374 2f69 6e64 6578 2e68 746d 6c29  fast/index.html)
+00000330: 0a62 7920 4875 6666 656e 6265 7267 6572  .by Huffenberger
+00000340: 2c20 6261 7365 6420 6f6e 2077 6f72 6b20  , based on work 
+00000350: 6279 0a5b 4875 6666 656e 6265 7267 6572  by.[Huffenberger
+00000360: 2061 6e64 2057 616e 6465 6c74 5d28 6874   and Wandelt](ht
+00000370: 7470 3a2f 2f73 7461 636b 732e 696f 702e  tp://stacks.iop.
+00000380: 6f72 672f 3030 3637 2d30 3034 392f 3138  org/0067-0049/18
+00000390: 392f 3235 3529 2e0a 0a4d 7920 6d6f 6469  9/255)...My modi
+000003a0: 6669 6361 7469 6f6e 7320 6d6f 7374 6c79  fications mostly
+000003b0: 2064 6561 6c20 7769 7468 2074 6865 2075   deal with the u
+000003c0: 7365 7220 696e 7465 7266 6163 653a 0a0a  ser interface:..
+000003d0: 2020 2a20 6164 6420 606d 756c 7469 5f6d    * add `multi_m
+000003e0: 6170 3273 616c 6d60 2061 6e64 2060 6d75  ap2salm` and `mu
+000003f0: 6c74 695f 7361 6c6d 326d 6170 6020 666f  lti_salm2map` fo
+00000400: 7220 7275 6e6e 696e 6720 6d61 6e79 2073  r running many s
+00000410: 696d 696c 6172 2074 7261 6e73 666f 726d  imilar transform
+00000420: 6174 696f 6e73 2065 6666 6963 6965 6e74  ations efficient
+00000430: 6c79 3b0a 2020 2a20 6372 6561 7465 2070  ly;.  * create p
+00000440: 7974 686f 6e20 7772 6170 7065 7273 2066  ython wrappers f
+00000450: 6f72 2074 6865 2060 6d61 7032 7361 6c6d  or the `map2salm
+00000460: 6020 616e 6420 6073 616c 6d32 6d61 7060  ` and `salm2map`
+00000470: 2066 756e 6374 696f 6e73 2074 6f20 6465   functions to de
+00000480: 616c 2077 6974 6820 616e 7920 2872 6561  al with any (rea
+00000490: 736f 6e61 626c 6529 0a20 2020 2074 7970  sonable).    typ
+000004a0: 6520 6f72 2073 6861 7065 206f 6620 696e  e or shape of in
+000004b0: 7075 7420 6461 7461 2c20 696e 636c 7564  put data, includ
+000004c0: 696e 6720 6d75 6c74 692d 6469 6d65 6e73  ing multi-dimens
+000004d0: 696f 6e61 6c3b 0a20 202a 2061 6464 2070  ional;.  * add p
+000004e0: 7974 686f 6e20 332e 7820 636f 6d70 6174  ython 3.x compat
+000004f0: 6962 696c 6974 7920 746f 2060 7079 7468  ibility to `pyth
+00000500: 6f6e 2f73 7069 6e73 6661 7374 5f6d 6f64  on/spinsfast_mod
+00000510: 756c 652e 6360 3b0a 2020 2a20 6669 7820  ule.c`;.  * fix 
+00000520: 7365 6766 6175 6c74 7320 6475 6520 746f  segfaults due to
+00000530: 2075 7365 206f 6620 6066 7265 6560 2069   use of `free` i
+00000540: 6e73 7465 6164 206f 6620 6066 6674 775f  nstead of `fftw_
+00000550: 6672 6565 6020 7768 656e 2060 6666 7477  free` when `fftw
+00000560: 5f6d 616c 6c6f 6360 2077 6173 2075 7365  _malloc` was use
+00000570: 643b 0a20 202a 206d 616b 6520 6974 2065  d;.  * make it e
+00000580: 6173 6965 7220 746f 2069 6e73 7461 6c6c  asier to install
+00000590: 2061 7320 6120 7079 7468 6f6e 206d 6f64   as a python mod
+000005a0: 756c 6520 6279 2074 7279 696e 6720 746f  ule by trying to
+000005b0: 2064 6574 6563 7420 7061 7468 7320 746f   detect paths to
+000005c0: 0a20 2020 2046 4654 573b 0a20 202a 2066  .    FFTW;.  * f
+000005d0: 6978 206e 756d 6572 6f75 7320 6d61 7373  ix numerous mass
+000005e0: 6976 6520 6d65 6d6f 7279 206c 6561 6b73  ive memory leaks
+000005f0: 2069 6e20 7079 7468 6f6e 2065 7874 656e   in python exten
+00000600: 7369 6f6e 206d 6f64 756c 653b 0a20 202a  sion module;.  *
+00000610: 2069 6e63 6c75 6465 2061 6e20 6970 7974   include an ipyt
+00000620: 686f 6e2f 6a75 7079 7465 7220 6e6f 7465  hon/jupyter note
+00000630: 626f 6f6b 2069 6e20 7468 6520 6065 7861  book in the `exa
+00000640: 6d70 6c65 6020 6469 7265 6374 6f72 793b  mple` directory;
+00000650: 0a20 202a 2061 6464 2069 6e74 6567 7261  .  * add integra
+00000660: 7469 6f6e 2077 6974 6820 5b70 6970 5d28  tion with [pip](
+00000670: 6874 7470 733a 2f2f 7079 7069 2e70 7974  https://pypi.pyt
+00000680: 686f 6e2e 6f72 672f 7079 7069 2f70 6970  hon.org/pypi/pip
+00000690: 290a 2020 2020 616e 6420 5b70 7970 695d  ).    and [pypi]
+000006a0: 2868 7474 7073 3a2f 2f70 7970 692e 7079  (https://pypi.py
+000006b0: 7468 6f6e 2e6f 7267 2f70 7970 692f 7370  thon.org/pypi/sp
+000006c0: 696e 7366 6173 7429 2c20 666f 7220 6561  insfast), for ea
+000006d0: 7379 2069 6e73 7461 6c6c 6174 696f 6e0a  sy installation.
+000006e0: 2020 2020 285b 7365 6520 6265 6c6f 775d      ([see below]
+000006f0: 2823 696e 7374 616c 6c61 7469 6f6e 2929  (#installation))
+00000700: 3b0a 2020 2a20 6164 6420 696e 7465 6772  ;.  * add integr
+00000710: 6174 696f 6e20 7769 7468 205b 636f 6e64  ation with [cond
+00000720: 615d 2868 7474 7073 3a2f 2f63 6f6e 6461  a](https://conda
+00000730: 2e69 6f2f 646f 6373 2f29 0a20 2020 2061  .io/docs/).    a
+00000740: 6e64 205b 616e 6163 6f6e 6461 2e6f 7267  nd [anaconda.org
+00000750: 5d28 6874 7470 733a 2f2f 616e 6163 6f6e  ](https://anacon
+00000760: 6461 2e6f 7267 2f6d 6f62 6c65 2f73 7069  da.org/moble/spi
+00000770: 6e73 6661 7374 292c 2066 6f72 2065 6173  nsfast), for eas
+00000780: 6965 7374 2069 6e73 7461 6c6c 6174 696f  iest installatio
+00000790: 6e0a 2020 2020 285b 7365 6520 6265 6c6f  n.    ([see belo
+000007a0: 775d 2823 696e 7374 616c 6c61 7469 6f6e  w](#installation
+000007b0: 2929 2e0a 0a23 204c 6963 656e 7365 0a0a  ))...# License..
+000007c0: 5468 6520 6f72 6967 696e 616c 2077 6f72  The original wor
+000007d0: 6b20 6973 206c 6963 656e 7365 6420 756e  k is licensed un
+000007e0: 6465 7220 4750 4c2c 2073 6f20 7468 6174  der GPL, so that
+000007f0: 2773 2077 6861 7420 4920 6861 7665 2074  's what I have t
+00000800: 6f20 6c69 6365 6e73 6520 7468 6973 0a75  o license this.u
+00000810: 6e64 6572 2061 7320 7765 6c6c 2e20 2028  nder as well.  (
+00000820: 4920 7573 7561 6c6c 7920 676f 2066 6f72  I usually go for
+00000830: 2074 6865 206d 6f72 6520 6c69 6265 7261   the more libera
+00000840: 6c20 4d49 5420 6c69 6365 6e73 652c 2062  l MIT license, b
+00000850: 7574 2047 504c 2069 730a 6669 6e65 2e29  ut GPL is.fine.)
+00000860: 2020 5365 6520 7468 6520 604c 4943 454e    See the `LICEN
+00000870: 5345 6020 6669 6c65 2069 6e20 7468 6973  SE` file in this
+00000880: 2064 6972 6563 746f 7279 2066 6f72 206d   directory for m
+00000890: 6f72 6520 6465 7461 696c 732e 0a0a 4920  ore details...I 
+000008a0: 6261 7365 6420 6d79 2077 6f72 6b20 6f6e  based my work on
+000008b0: 2048 7566 6665 6e62 6572 6765 7220 616e   Huffenberger an
+000008c0: 6420 5761 6e64 656c 7427 7320 2252 6576  d Wandelt's "Rev
+000008d0: 6973 696f 6e20 3130 342c 2031 3320 4170  ision 104, 13 Ap
+000008e0: 7220 3230 3132 222c 0a77 6869 6368 2069  r 2012",.which i
+000008f0: 7320 6375 7272 656e 7420 6173 206f 6620  s current as of 
+00000900: 7468 6973 2077 7269 7469 6e67 2028 4175  this writing (Au
+00000910: 6775 7374 2032 3031 3529 2e20 2057 6865  gust 2015).  Whe
+00000920: 6e65 7665 7220 4920 6e6f 7469 6365 2075  never I notice u
+00000930: 7064 6174 6573 0a6f 6e20 7468 6569 7220  pdates.on their 
+00000940: 656e 642c 2049 2077 696c 6c20 676c 6164  end, I will glad
+00000950: 6c79 2075 7064 6174 6520 7468 6973 2063  ly update this c
+00000960: 6f64 652c 2073 6f20 6665 656c 2066 7265  ode, so feel fre
+00000970: 6520 746f 206f 7065 6e20 616e 0a5b 6973  e to open an.[is
+00000980: 7375 655d 2868 7474 7073 3a2f 2f67 6974  sue](https://git
+00000990: 6875 622e 636f 6d2f 6d6f 626c 652f 7370  hub.com/moble/sp
+000009a0: 696e 7366 6173 742f 6973 7375 6573 2920  insfast/issues) 
+000009b0: 746f 206e 6f74 6966 7920 6d65 2e20 2054  to notify me.  T
+000009c0: 6f20 7365 6520 6d6f 7265 0a73 7065 6369  o see more.speci
+000009d0: 6669 6361 6c6c 7920 7768 6174 2049 2776  fically what I'v
+000009e0: 6520 6164 6465 642c 206c 6f6f 6b20 7468  e added, look th
+000009f0: 726f 7567 6820 7468 650a 5b63 6f6d 6d69  rough the.[commi
+00000a00: 7473 5d28 6874 7470 733a 2f2f 6769 7468  ts](https://gith
+00000a10: 7562 2e63 6f6d 2f6d 6f62 6c65 2f73 7069  ub.com/moble/spi
+00000a20: 6e73 6661 7374 2f63 6f6d 6d69 7473 2f6d  nsfast/commits/m
+00000a30: 6173 7465 7229 3b20 6d79 2063 6f6e 7472  aster); my contr
+00000a40: 6962 7574 696f 6e73 0a61 7265 206a 7573  ibutions.are jus
+00000a50: 7420 6576 6572 7974 6869 6e67 2073 696e  t everything sin
+00000a60: 6365 2074 6865 2069 6e69 7469 616c 2063  ce the initial c
+00000a70: 6f6d 6d69 742e 0a0a 0a23 2045 7861 6d70  ommit....# Examp
+00000a80: 6c65 2055 7361 6765 0a0a 4120 636f 6e76  le Usage..A conv
+00000a90: 656e 6965 6e74 2069 7079 7468 6f6e 2f6a  enient ipython/j
+00000aa0: 7570 7974 6572 206e 6f74 6562 6f6f 6b20  upyter notebook 
+00000ab0: 6973 2066 6f75 6e64 2069 6e20 7468 6520  is found in the 
+00000ac0: 6065 7861 6d70 6c65 6020 6469 7265 6374  `example` direct
+00000ad0: 6f72 792c 2061 6e64 0a63 616e 2061 6c73  ory, and.can als
+00000ae0: 6f20 6265 0a5b 7669 6577 6564 2064 6972  o be.[viewed dir
+00000af0: 6563 746c 7920 6f6e 6c69 6e65 5d28 6874  ectly online](ht
+00000b00: 7470 3a2f 2f6e 6276 6965 7765 722e 6970  tp://nbviewer.ip
+00000b10: 7974 686f 6e2e 6f72 672f 6769 7468 7562  ython.org/github
+00000b20: 2f6d 6f62 6c65 2f73 7069 6e73 6661 7374  /moble/spinsfast
+00000b30: 2f62 6c6f 622f 6d61 7374 6572 2f65 7861  /blob/master/exa
+00000b40: 6d70 6c65 2f73 7069 6e73 6661 7374 2e69  mple/spinsfast.i
+00000b50: 7079 6e62 292e 0a49 7420 7368 6f77 7320  pynb)..It shows 
+00000b60: 736f 6d65 2065 7861 6d70 6c65 2070 7974  some example pyt
+00000b70: 686f 6e20 636f 6465 2074 6861 7420 6361  hon code that ca
+00000b80: 6e20 6265 2075 7365 6420 746f 2072 756e  n be used to run
+00000b90: 2074 6869 7320 6d6f 6475 6c65 2c20 616e   this module, an
+00000ba0: 640a 6578 706c 6169 6e73 2073 6f6d 6520  d.explains some 
+00000bb0: 6f66 2074 6865 2063 6f6e 7665 6e74 696f  of the conventio
+00000bc0: 6e73 2065 7374 6162 6c69 7368 6564 2062  ns established b
+00000bd0: 7920 7468 6520 6073 7069 6e73 6661 7374  y the `spinsfast
+00000be0: 6020 6175 7468 6f72 732e 0a0a 496e 2074  ` authors...In t
+00000bf0: 6865 2069 6e74 6572 6573 7473 206f 6620  he interests of 
+00000c00: 6120 7665 7279 2073 686f 7274 2c20 6578  a very short, ex
+00000c10: 706c 6963 6974 2065 7861 6d70 6c65 2c20  plicit example, 
+00000c20: 6865 7265 2069 7320 6f6e 6520 7573 696e  here is one usin
+00000c30: 6720 7261 6e64 6f6d 2060 2865 6c6c 2c6d  g random `(ell,m
+00000c40: 2960 206d 6f64 6573 3a0a 0a60 6060 7079  )` modes:..```py
+00000c50: 7468 6f6e 0a66 726f 6d20 6e75 6d70 792e  thon.from numpy.
+00000c60: 7261 6e64 6f6d 2069 6d70 6f72 7420 6e6f  random import no
+00000c70: 726d 616c 2c20 7365 6564 0a69 6d70 6f72  rmal, seed.impor
+00000c80: 7420 7370 696e 7366 6173 740a 0a23 2053  t spinsfast..# S
+00000c90: 6f6d 6520 626f 696c 6572 706c 6174 6520  ome boilerplate 
+00000ca0: 666f 7220 7365 7474 696e 6720 7468 696e  for setting thin
+00000cb0: 6773 2075 703a 0a73 203d 2031 2020 2320  gs up:.s = 1  # 
+00000cc0: 7370 696e 2077 6569 6768 7420 6f66 2074  spin weight of t
+00000cd0: 6865 2066 6965 6c64 0a6c 6d61 7820 3d20  he field.lmax = 
+00000ce0: 3820 2023 206d 6178 696d 756d 2065 6c6c  8  # maximum ell
+00000cf0: 2076 616c 7565 2075 7365 640a 4e74 6865   value used.Nthe
+00000d00: 7461 203d 2032 2a6c 6d61 782b 3120 2023  ta = 2*lmax+1  #
+00000d10: 204d 696e 696d 756d 2076 616c 7565 2066   Minimum value f
+00000d20: 6f72 2061 6363 7572 6163 790a 4e70 6869  or accuracy.Nphi
+00000d30: 203d 2032 2a6c 6d61 782b 3120 2023 204d   = 2*lmax+1  # M
+00000d40: 696e 696d 756d 2076 616c 7565 2066 6f72  inimum value for
+00000d50: 2061 6363 7572 6163 790a 4e6c 6d20 3d20   accuracy.Nlm = 
+00000d60: 7370 696e 7366 6173 742e 4e5f 6c6d 286c  spinsfast.N_lm(l
+00000d70: 6d61 7829 3b20 2023 2054 6f74 616c 206e  max);  # Total n
+00000d80: 756d 6265 7220 6f66 2063 6f6d 706c 6578  umber of complex
+00000d90: 2063 6f6d 706f 6e65 6e74 7320 6f66 2074   components of t
+00000da0: 6865 206d 6f64 6520 6465 636f 6d70 6f73  he mode decompos
+00000db0: 6974 696f 6e0a 0a23 2060 616c 6d60 2077  ition..# `alm` w
+00000dc0: 696c 6c20 686f 6c64 2074 6865 206d 6f64  ill hold the mod
+00000dd0: 6520 636f 6d70 6f6e 656e 7473 2061 7320  e components as 
+00000de0: 6469 7363 7573 7365 6420 696e 2060 6578  discussed in `ex
+00000df0: 616d 706c 652f 7370 696e 7366 6173 742e  ample/spinsfast.
+00000e00: 6970 796e 6260 0a23 2048 6572 6520 7765  ipynb`.# Here we
+00000e10: 206a 7573 7420 6669 6c6c 2069 7420 7769   just fill it wi
+00000e20: 7468 2073 6f6d 6520 7261 6e64 6f6d 206e  th some random n
+00000e30: 756d 6265 7273 2074 6f20 7465 7374 2069  umbers to test i
+00000e40: 740a 7365 6564 2833 3132 3434 3332 2920  t.seed(3124432) 
+00000e50: 2023 2053 6565 6420 7468 6520 7261 6e64   # Seed the rand
+00000e60: 6f6d 2d6e 756d 6265 7220 6765 6e65 7261  om-number genera
+00000e70: 746f 722c 2066 6f72 2072 6570 726f 6475  tor, for reprodu
+00000e80: 6369 6269 6c69 7479 0a61 6c6d 203d 206e  cibility.alm = n
+00000e90: 6f72 6d61 6c28 7369 7a65 3d28 4e6c 6d2c  ormal(size=(Nlm,
+00000ea0: 2929 202b 2031 6a2a 6e6f 726d 616c 2873  )) + 1j*normal(s
+00000eb0: 697a 653d 284e 6c6d 2c29 290a 0a23 2054  ize=(Nlm,))..# T
+00000ec0: 6869 7320 6973 2074 6865 206b 6579 206c  his is the key l
+00000ed0: 696e 652c 2077 6865 7265 2073 7069 6e73  ine, where spins
+00000ee0: 6661 7374 2063 6f6e 7665 7274 7320 6672  fast converts fr
+00000ef0: 6f6d 2028 656c 6c2c 6d29 206d 6f64 6573  om (ell,m) modes
+00000f00: 2074 6f20 7661 6c75 6573 2069 6e20 7068   to values in ph
+00000f10: 7973 6963 616c 2073 7061 6365 0a66 203d  ysical space.f =
+00000f20: 2020 7370 696e 7366 6173 742e 7361 6c6d    spinsfast.salm
+00000f30: 326d 6170 2861 6c6d 2c73 2c6c 6d61 782c  2map(alm,s,lmax,
+00000f40: 4e74 6865 7461 2c4e 7068 6929 0a0a 2320  Ntheta,Nphi)..# 
+00000f50: 5765 2063 616e 2061 6c73 6f20 636f 6e76  We can also conv
+00000f60: 6572 7420 696e 2074 6865 206f 7070 6f73  ert in the oppos
+00000f70: 6974 6520 6469 7265 6374 696f 6e20 6c69  ite direction li
+00000f80: 6b65 2074 6869 733a 0a61 6c6d 3220 3d20  ke this:.alm2 = 
+00000f90: 7370 696e 7366 6173 742e 6d61 7032 7361  spinsfast.map2sa
+00000fa0: 6c6d 2866 2c73 2c6c 6d61 7829 0a60 6060  lm(f,s,lmax).```
+00000fb0: 0a0a 0a23 2049 6e73 7461 6c6c 6174 696f  ...# Installatio
+00000fc0: 6e0a 0a23 2320 416e 6163 6f6e 6461 0a0a  n..## Anaconda..
+00000fd0: 5468 6f75 6768 206d 616e 7561 6c20 696e  Though manual in
+00000fe0: 7374 616c 6c61 7469 6f6e 2069 7320 706f  stallation is po
+00000ff0: 7373 6962 6c65 2c20 7468 6520 6265 7374  ssible, the best
+00001000: 2077 6179 2062 7920 6661 7220 746f 2073   way by far to s
+00001010: 6174 6973 6679 2074 6865 7365 0a64 6570  atisfy these.dep
+00001020: 656e 6465 6e63 6965 7320 6973 2074 6f20  endencies is to 
+00001030: 7573 6520 7468 6520 5b60 616e 6163 6f6e  use the [`anacon
+00001040: 6461 605d 2868 7474 703a 2f2f 636f 6e74  da`](http://cont
+00001050: 696e 7575 6d2e 696f 2f64 6f77 6e6c 6f61  inuum.io/downloa
+00001060: 6473 290a 6469 7374 7269 6275 7469 6f6e  ds).distribution
+00001070: 2e20 2054 6869 7320 6469 7374 7269 6275  .  This distribu
+00001080: 7469 6f6e 2063 616e 2063 6f2d 6578 6973  tion can co-exis
+00001090: 7420 7769 7468 2079 6f75 7220 7379 7374  t with your syst
+000010a0: 656d 2070 7974 686f 6e20 7769 7468 206e  em python with n
+000010b0: 6f0a 7472 6f75 626c 6520 2d2d 2079 6f75  o.trouble -- you
+000010c0: 2073 696d 706c 7920 6164 6420 7468 6520   simply add the 
+000010d0: 7061 7468 2074 6f20 616e 6163 6f6e 6461  path to anaconda
+000010e0: 2062 6566 6f72 6520 796f 7572 2073 7973   before your sys
+000010f0: 7465 6d20 6578 6563 7574 6162 6c65 732e  tem executables.
+00001100: 0a49 7420 696e 7374 616c 6c73 2069 6e74  .It installs int
+00001110: 6f20 796f 7572 2068 6f6d 6520 6469 7265  o your home dire
+00001120: 6374 6f72 792c 2073 6f20 6974 2064 6f65  ctory, so it doe
+00001130: 736e 2774 2072 6571 7569 7265 2072 6f6f  sn't require roo
+00001140: 7420 6163 6365 7373 2e20 2049 740a 6361  t access.  It.ca
+00001150: 6e20 6265 2075 6e69 6e73 7461 6c6c 6564  n be uninstalled
+00001160: 2065 6173 696c 792c 2073 696e 6365 2069   easily, since i
+00001170: 7420 6578 6973 7473 2065 6e74 6972 656c  t exists entirel
+00001180: 7920 696e 7369 6465 2069 7473 206f 776e  y inside its own
+00001190: 2064 6972 6563 746f 7279 2e0a 416e 6420   directory..And 
+000011a0: 7570 6461 7465 7320 6172 6520 7472 6976  updates are triv
+000011b0: 6961 6c2e 0a0a 4f6e 6365 2060 616e 6163  ial...Once `anac
+000011c0: 6f6e 6461 6020 6973 2069 6e73 7461 6c6c  onda` is install
+000011d0: 6564 2c20 7468 6973 2070 6163 6b61 6765  ed, this package
+000011e0: 206d 6179 2062 6520 696e 7374 616c 6c65   may be installe
+000011f0: 6420 7769 7468 2074 6865 2063 6f6d 6d61  d with the comma
+00001200: 6e64 0a0a 6060 6062 6173 680a 636f 6e64  nd..```bash.cond
+00001210: 6120 696e 7374 616c 6c20 2d2d 6368 616e  a install --chan
+00001220: 6e65 6c20 636f 6e64 612d 666f 7267 6520  nel conda-forge 
+00001230: 7370 696e 7366 6173 740a 6060 600a 0a4e  spinsfast.```..N
+00001240: 6f74 6520 7468 6973 206d 6179 2061 6c73  ote this may als
+00001250: 6f20 696e 7374 616c 6c20 606e 756d 7079  o install `numpy
+00001260: 6020 616e 6420 6066 6674 7760 2061 7574  ` and `fftw` aut
+00001270: 6f6d 6174 6963 616c 6c79 2e0a 0a0a 2323  omatically....##
+00001280: 2050 6970 0a0a 5768 696c 6520 6765 6e65   Pip..While gene
+00001290: 7261 6c6c 7920 6c65 7373 2072 6f62 7573  rally less robus
+000012a0: 742c 2074 6869 7320 7061 636b 6167 6520  t, this package 
+000012b0: 6973 2061 6c73 6f20 6176 6169 6c61 626c  is also availabl
+000012c0: 6520 7669 6120 6070 6970 603a 0a0a 6060  e via `pip`:..``
+000012d0: 6062 6173 680a 7069 7020 696e 7374 616c  `bash.pip instal
+000012e0: 6c20 7370 696e 7366 6173 740a 6060 600a  l spinsfast.```.
+000012f0: 0a55 6e66 6f72 7475 6e61 7465 6c79 2c20  .Unfortunately, 
+00001300: 6d61 696e 7461 696e 696e 6720 6269 6e61  maintaining bina
+00001310: 7279 2064 6973 7472 6962 7574 696f 6e73  ry distributions
+00001320: 206f 6e20 7069 7020 6973 2074 6f6f 2074   on pip is too t
+00001330: 696d 652d 636f 6e73 756d 696e 672c 2073  ime-consuming, s
+00001340: 6f20 6070 6970 6020 7769 6c6c 2074 7279  o `pip` will try
+00001350: 2074 6f0a 636f 6d70 696c 6520 7468 6520   to.compile the 
+00001360: 736f 7572 6365 2063 6f64 6520 666f 7220  source code for 
+00001370: 796f 752c 2069 6e20 7768 6963 6820 6361  you, in which ca
+00001380: 7365 2079 6f75 2077 696c 6c20 6e65 6564  se you will need
+00001390: 2074 6f20 6861 7665 2046 4654 5720 616e   to have FFTW an
+000013a0: 6420 6120 636f 6d70 696c 6572 2069 6e73  d a compiler ins
+000013b0: 7461 6c6c 6564 2e0a 556e 666f 7274 756e  talled..Unfortun
+000013c0: 6174 656c 792c 2060 7069 7060 2068 6173  ately, `pip` has
+000013d0: 206e 6f20 676f 6f64 2077 6179 206f 6620   no good way of 
+000013e0: 6861 6e64 6c69 6e67 2074 6865 7365 2064  handling these d
+000013f0: 6570 656e 6465 6e63 6965 732e 2020 5365  ependencies.  Se
+00001400: 6520 6265 6c6f 7720 666f 7220 656e 7669  e below for envi
+00001410: 726f 6e6d 656e 740a 7661 7269 6162 6c65  ronment.variable
+00001420: 7320 796f 7520 6d61 7920 6e65 6564 2074  s you may need t
+00001430: 6f20 7365 7420 746f 2067 6574 2063 6f6d  o set to get com
+00001440: 7069 6c61 7469 6f6e 2077 6f72 6b69 6e67  pilation working
+00001450: 2070 726f 7065 726c 792e 0a0a 0a23 2320   properly....## 
+00001460: 4d61 6e75 616c 2069 6e73 7461 6c6c 6174  Manual installat
+00001470: 696f 6e0a 0a4d 616e 7561 6c20 696e 7374  ion..Manual inst
+00001480: 616c 6c61 7469 6f6e 206f 6620 7468 6973  allation of this
+00001490: 2070 6163 6b61 6765 2069 7320 736c 6967   package is slig
+000014a0: 6874 6c79 206d 6f72 6520 6465 6c69 6361  htly more delica
+000014b0: 7465 2e20 2054 6865 0a5b 4646 5457 2070  te.  The.[FFTW p
+000014c0: 6163 6b61 6765 5d28 6874 7470 3a2f 2f77  ackage](http://w
+000014d0: 7777 2e66 6674 772e 6f72 672f 2920 6d75  ww.fftw.org/) mu
+000014e0: 7374 2062 6520 696e 7374 616c 6c65 6420  st be installed 
+000014f0: 6669 7273 742e 2020 5468 6973 2069 7320  first.  This is 
+00001500: 7573 7561 6c6c 790a 7665 7279 2073 696d  usually.very sim
+00001510: 706c 652e 2020 4275 7420 7468 6520 7265  ple.  But the re
+00001520: 7375 6c74 696e 6720 6865 6164 6572 2061  sulting header a
+00001530: 6e64 206c 6962 7261 7279 206d 7573 7420  nd library must 
+00001540: 6265 2066 6f75 6e64 2062 7920 7468 650a  be found by the.
+00001550: 636f 6d70 696c 6174 696f 6e20 7374 6570  compilation step
+00001560: 2066 6f72 2074 6869 7320 7061 636b 6167   for this packag
+00001570: 652e 2020 596f 7520 6361 6e20 6669 7273  e.  You can firs
+00001580: 7420 7369 6d70 6c79 2074 7279 2074 6f20  t simply try to 
+00001590: 7275 6e0a 0a60 6060 6261 7368 0a70 7974  run..```bash.pyt
+000015a0: 686f 6e20 7365 7475 702e 7079 2069 6e73  hon setup.py ins
+000015b0: 7461 6c6c 0a60 6060 0a0a 6672 6f6d 2074  tall.```..from t
+000015c0: 6865 2074 6f70 2064 6972 6563 746f 7279  he top directory
+000015d0: 206f 6620 7468 6520 6073 7069 6e73 6661   of the `spinsfa
+000015e0: 7374 6020 636f 6465 2e0a 0a49 6620 7468  st` code...If th
+000015f0: 6973 2064 6f65 736e 2774 2077 6f72 6b2c  is doesn't work,
+00001600: 2079 6f75 2063 616e 2072 6561 6420 7468   you can read th
+00001610: 6520 6572 726f 7220 6d65 7373 6167 652c  e error message,
+00001620: 2062 7574 2074 6865 206d 6f73 7420 6c69   but the most li
+00001630: 6b65 6c79 0a70 726f 626c 656d 2069 7320  kely.problem is 
+00001640: 7468 6174 2074 6865 2063 6f6d 7069 6c65  that the compile
+00001650: 7220 6361 6e6e 6f74 2066 696e 6420 7468  r cannot find th
+00001660: 6520 6066 6674 7760 2068 6561 6465 722c  e `fftw` header,
+00001670: 206f 7220 7468 6520 6c69 6e6b 6572 0a63   or the linker.c
+00001680: 616e 6e6f 7420 6669 6e64 2074 6865 2060  annot find the `
+00001690: 6666 7477 6020 6c69 6272 6172 792e 2020  fftw` library.  
+000016a0: 546f 2073 6f6c 7665 2074 6865 7365 2070  To solve these p
+000016b0: 726f 626c 656d 732c 2079 6f75 2077 696c  roblems, you wil
+000016c0: 6c20 6e65 6564 2074 6f20 7275 6e0a 736f  l need to run.so
+000016d0: 6d65 7468 696e 6720 6d6f 7265 206c 696b  mething more lik
+000016e0: 6520 7468 6973 3a0a 0a60 6060 6261 7368  e this:..```bash
+000016f0: 0a65 7870 6f72 7420 4c49 4252 4152 595f  .export LIBRARY_
+00001700: 5041 5448 3d2f 7061 7468 2f74 6f2f 6666  PATH=/path/to/ff
+00001710: 7477 2f6c 6962 0a65 7870 6f72 7420 435f  tw/lib.export C_
+00001720: 494e 434c 5544 455f 5041 5448 3d2f 7061  INCLUDE_PATH=/pa
+00001730: 7468 2f74 6f2f 6666 7477 2f69 6e63 6c75  th/to/fftw/inclu
+00001740: 6465 0a70 7974 686f 6e20 7365 7475 702e  de.python setup.
+00001750: 7079 2069 6e73 7461 6c6c 0a60 6060 0a0a  py install.```..
+00001760: 416c 7465 726e 6174 6976 656c 792c 2079  Alternatively, y
+00001770: 6f75 2063 6f75 6c64 2074 7279 2074 6f20  ou could try to 
+00001780: 616c 7465 7220 6073 6574 7570 2e70 7960  alter `setup.py`
+00001790: 2074 6f20 706f 696e 7420 746f 2074 6865   to point to the
+000017a0: 2072 6967 6874 0a70 6174 6873 2e0a 0a0a   right.paths....
+000017b0: 2320 4f72 6967 696e 616c 2069 6e73 7461  # Original insta
+000017c0: 6c6c 6174 696f 6e20 696e 7374 7275 6374  llation instruct
+000017d0: 696f 6e73 0a0a 5468 6f75 6768 2074 6865  ions..Though the
+000017e0: 7365 2061 7265 206e 6f74 206e 6563 6573  se are not neces
+000017f0: 7361 7279 2066 6f72 2069 6e73 7461 6c6c  sary for install
+00001800: 696e 6720 7468 6520 7079 7468 6f6e 206d  ing the python m
+00001810: 6f64 756c 652c 2074 6865 2066 6f6c 6c6f  odule, the follo
+00001820: 7769 6e67 0a61 7265 2074 6865 2069 6e73  wing.are the ins
+00001830: 7472 7563 7469 6f6e 7320 696e 2074 6865  tructions in the
+00001840: 206f 7269 6769 6e61 6c20 736f 7572 6365   original source
+00001850: 2063 6f64 6520 666f 7220 6275 696c 6469   code for buildi
+00001860: 6e67 2074 6865 2043 2063 6f64 652e 0a0a  ng the C code...
+00001870: 4765 7420 7468 6520 6c61 7465 7374 2076  Get the latest v
+00001880: 6572 7369 6f6e 2061 743a 0a0a 2020 2020  ersion at:..    
+00001890: 6874 7470 3a2f 2f77 7777 2e70 6879 7369  http://www.physi
+000018a0: 6373 2e6d 6961 6d69 2e65 6475 2f7e 6875  cs.miami.edu/~hu
+000018b0: 6666 656e 6265 2f72 6573 6561 7263 682f  ffenbe/research/
+000018c0: 7370 696e 7366 6173 742f 0a0a 2323 2043  spinsfast/..## C
+000018d0: 6f6d 7069 6c61 7469 6f6e 2069 6e73 7472  ompilation instr
+000018e0: 7563 7469 6f6e 730a 0a20 2031 2e20 4564  uctions..  1. Ed
+000018f0: 6974 2074 6865 2066 696c 6520 286f 7220  it the file (or 
+00001900: 6d61 6b65 2061 206e 6577 2066 696c 6529  make a new file)
+00001910: 2063 616c 6c65 6420 6275 696c 642f 636f   called build/co
+00001920: 6e66 6967 2e6d 6b20 736f 2074 6861 7420  nfig.mk so that 
+00001930: 7468 6520 7072 6f70 6572 206c 6f63 6174  the proper locat
+00001940: 696f 6e73 2066 6f72 2068 6561 6465 7220  ions for header 
+00001950: 616e 6420 6c69 6272 6172 7920 6669 6c65  and library file
+00001960: 7320 6172 6520 696e 636c 7564 6564 2e0a  s are included..
+00001970: 0a20 2032 2e20 5365 7420 7468 6520 656e  .  2. Set the en
+00001980: 7669 726f 6e6d 656e 7420 7661 7269 6162  vironment variab
+00001990: 6c65 2022 6275 696c 6422 2073 6f20 7468  le "build" so th
+000019a0: 6174 2069 7420 706f 696e 7473 2074 6f20  at it points to 
+000019b0: 7468 6174 2066 696c 652e 2049 2e65 2e2c  that file. I.e.,
+000019c0: 2069 6e20 6261 7368 2c20 7361 790a 0a20   in bash, say.. 
+000019d0: 2020 2020 2020 2065 7870 6f72 7420 6275         export bu
+000019e0: 696c 643d 6275 696c 642f 636f 6e66 6967  ild=build/config
+000019f0: 2e6d 6b20 0a0a 2020 332e 2042 7569 6c64  .mk ..  3. Build
+00001a00: 2074 6865 206c 6962 7261 7279 2061 6e64   the library and
+00001a10: 2065 7861 6d70 6c65 2063 6f64 6573 2077   example codes w
+00001a20: 6974 6820 0a0a 2020 2020 2020 2020 6d61  ith ..        ma
+00001a30: 6b65 0a0a 2323 2028 4f70 7469 6f6e 616c  ke..## (Optional
+00001a40: 2920 4368 6563 6b69 6e67 2074 6865 2063  ) Checking the c
+00001a50: 6f6d 7069 6c61 7469 6f6e 0a0a 5275 6e20  ompilation..Run 
+00001a60: 7468 6520 6578 616d 706c 6520 636f 6465  the example code
+00001a70: 2066 6f6c 6c6f 7769 6e67 2074 6865 2069   following the i
+00001a80: 6e73 7472 7563 7469 6f6e 7320 6174 200a  nstructions at .
+00001a90: 0a20 2020 2068 7474 703a 2f2f 7777 772e  .    http://www.
+00001aa0: 7068 7973 6963 732e 6d69 616d 692e 6564  physics.miami.ed
+00001ab0: 752f 7e68 7566 6665 6e62 652f 7265 7365  u/~huffenbe/rese
+00001ac0: 6172 6368 2f73 7069 6e73 6661 7374 2f0a  arch/spinsfast/.
```

### Comparing `spinsfast-2022.4.1/README.md` & `spinsfast-2022.4.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,400 +1,429 @@
-00000000: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00000010: 2f7a 656e 6f64 6f2e 6f72 672f 6261 6467  /zenodo.org/badg
-00000020: 652f 6c61 7465 7374 646f 692f 3330 3334  e/latestdoi/3034
-00000030: 3035 3832 223e 3c69 6d67 2061 6c69 676e  0582"><img align
-00000040: 3d22 7269 6768 7422 2073 7263 3d22 6874  ="right" src="ht
-00000050: 7470 733a 2f2f 7a65 6e6f 646f 2e6f 7267  tps://zenodo.org
-00000060: 2f62 6164 6765 2f33 3033 3430 3538 322e  /badge/30340582.
-00000070: 7376 6722 2061 6c74 3d22 444f 4922 3e3c  svg" alt="DOI"><
-00000080: 2f61 3e0a 0a23 2073 7069 6e73 6661 7374  /a>..# spinsfast
-00000090: 0a46 6173 7420 616e 6420 6578 6163 7420  .Fast and exact 
-000000a0: 7370 696e 2d73 2073 7068 6572 6963 616c  spin-s spherical
-000000b0: 2d68 6172 6d6f 6e69 6320 7472 616e 7366  -harmonic transf
-000000c0: 6f72 6d73 0a0a 5468 6973 2063 6f64 6520  orms..This code 
-000000d0: 6973 2061 206c 6967 6874 6c79 206d 6f64  is a lightly mod
-000000e0: 6966 6965 6420 7665 7273 696f 6e20 6f66  ified version of
-000000f0: 2074 6865 2063 6f64 6520 686f 7374 6564   the code hosted
-00000100: 0a5b 6865 7265 5d28 6874 7470 3a2f 2f61  .[here](http://a
-00000110: 7374 726f 7068 7973 6963 732e 7068 7973  strophysics.phys
-00000120: 6963 732e 6673 752e 6564 752f 7e68 7566  ics.fsu.edu/~huf
-00000130: 6665 6e62 652f 7265 7365 6172 6368 2f73  fenbe/research/s
-00000140: 7069 6e73 6661 7374 2f69 6e64 6578 2e68  pinsfast/index.h
-00000150: 746d 6c29 0a62 7920 4875 6666 656e 6265  tml).by Huffenbe
-00000160: 7267 6572 2c20 6261 7365 6420 6f6e 2077  rger, based on w
-00000170: 6f72 6b20 6279 0a5b 4875 6666 656e 6265  ork by.[Huffenbe
-00000180: 7267 6572 2061 6e64 2057 616e 6465 6c74  rger and Wandelt
-00000190: 5d28 6874 7470 3a2f 2f73 7461 636b 732e  ](http://stacks.
-000001a0: 696f 702e 6f72 672f 3030 3637 2d30 3034  iop.org/0067-004
-000001b0: 392f 3138 392f 3235 3529 2e0a 0a4d 7920  9/189/255)...My 
-000001c0: 6d6f 6469 6669 6361 7469 6f6e 7320 6d6f  modifications mo
-000001d0: 7374 6c79 2064 6561 6c20 7769 7468 2074  stly deal with t
-000001e0: 6865 2075 7365 7220 696e 7465 7266 6163  he user interfac
-000001f0: 653a 0a0a 2020 2a20 6164 6420 606d 756c  e:..  * add `mul
-00000200: 7469 5f6d 6170 3273 616c 6d60 2061 6e64  ti_map2salm` and
-00000210: 2060 6d75 6c74 695f 7361 6c6d 326d 6170   `multi_salm2map
-00000220: 6020 666f 7220 7275 6e6e 696e 6720 6d61  ` for running ma
-00000230: 6e79 2073 696d 696c 6172 2074 7261 6e73  ny similar trans
-00000240: 666f 726d 6174 696f 6e73 2065 6666 6963  formations effic
-00000250: 6965 6e74 6c79 3b0a 2020 2a20 6372 6561  iently;.  * crea
-00000260: 7465 2070 7974 686f 6e20 7772 6170 7065  te python wrappe
-00000270: 7273 2066 6f72 2074 6865 2060 6d61 7032  rs for the `map2
-00000280: 7361 6c6d 6020 616e 6420 6073 616c 6d32  salm` and `salm2
-00000290: 6d61 7060 2066 756e 6374 696f 6e73 2074  map` functions t
-000002a0: 6f20 6465 616c 2077 6974 6820 616e 7920  o deal with any 
-000002b0: 2872 6561 736f 6e61 626c 6529 0a20 2020  (reasonable).   
-000002c0: 2074 7970 6520 6f72 2073 6861 7065 206f   type or shape o
-000002d0: 6620 696e 7075 7420 6461 7461 2c20 696e  f input data, in
-000002e0: 636c 7564 696e 6720 6d75 6c74 692d 6469  cluding multi-di
-000002f0: 6d65 6e73 696f 6e61 6c3b 0a20 202a 2061  mensional;.  * a
-00000300: 6464 2070 7974 686f 6e20 332e 7820 636f  dd python 3.x co
-00000310: 6d70 6174 6962 696c 6974 7920 746f 2060  mpatibility to `
-00000320: 7079 7468 6f6e 2f73 7069 6e73 6661 7374  python/spinsfast
-00000330: 5f6d 6f64 756c 652e 6360 3b0a 2020 2a20  _module.c`;.  * 
-00000340: 6669 7820 7365 6766 6175 6c74 7320 6475  fix segfaults du
-00000350: 6520 746f 2075 7365 206f 6620 6066 7265  e to use of `fre
-00000360: 6560 2069 6e73 7465 6164 206f 6620 6066  e` instead of `f
-00000370: 6674 775f 6672 6565 6020 7768 656e 2060  ftw_free` when `
-00000380: 6666 7477 5f6d 616c 6c6f 6360 2077 6173  fftw_malloc` was
-00000390: 2075 7365 643b 0a20 202a 206d 616b 6520   used;.  * make 
-000003a0: 6974 2065 6173 6965 7220 746f 2069 6e73  it easier to ins
-000003b0: 7461 6c6c 2061 7320 6120 7079 7468 6f6e  tall as a python
-000003c0: 206d 6f64 756c 6520 6279 2074 7279 696e   module by tryin
-000003d0: 6720 746f 2064 6574 6563 7420 7061 7468  g to detect path
-000003e0: 7320 746f 0a20 2020 2046 4654 573b 0a20  s to.    FFTW;. 
-000003f0: 202a 2066 6978 206e 756d 6572 6f75 7320   * fix numerous 
-00000400: 6d61 7373 6976 6520 6d65 6d6f 7279 206c  massive memory l
-00000410: 6561 6b73 2069 6e20 7079 7468 6f6e 2065  eaks in python e
-00000420: 7874 656e 7369 6f6e 206d 6f64 756c 653b  xtension module;
-00000430: 0a20 202a 2069 6e63 6c75 6465 2061 6e20  .  * include an 
-00000440: 6970 7974 686f 6e2f 6a75 7079 7465 7220  ipython/jupyter 
-00000450: 6e6f 7465 626f 6f6b 2069 6e20 7468 6520  notebook in the 
-00000460: 6065 7861 6d70 6c65 6020 6469 7265 6374  `example` direct
-00000470: 6f72 793b 0a20 202a 2061 6464 2069 6e74  ory;.  * add int
-00000480: 6567 7261 7469 6f6e 2077 6974 6820 5b70  egration with [p
-00000490: 6970 5d28 6874 7470 733a 2f2f 7079 7069  ip](https://pypi
-000004a0: 2e70 7974 686f 6e2e 6f72 672f 7079 7069  .python.org/pypi
-000004b0: 2f70 6970 290a 2020 2020 616e 6420 5b70  /pip).    and [p
-000004c0: 7970 695d 2868 7474 7073 3a2f 2f70 7970  ypi](https://pyp
-000004d0: 692e 7079 7468 6f6e 2e6f 7267 2f70 7970  i.python.org/pyp
-000004e0: 692f 7370 696e 7366 6173 7429 2c20 666f  i/spinsfast), fo
-000004f0: 7220 6561 7379 2069 6e73 7461 6c6c 6174  r easy installat
-00000500: 696f 6e0a 2020 2020 285b 7365 6520 6265  ion.    ([see be
-00000510: 6c6f 775d 2823 696e 7374 616c 6c61 7469  low](#installati
-00000520: 6f6e 2929 3b0a 2020 2a20 6164 6420 696e  on));.  * add in
-00000530: 7465 6772 6174 696f 6e20 7769 7468 205b  tegration with [
-00000540: 636f 6e64 615d 2868 7474 7073 3a2f 2f63  conda](https://c
-00000550: 6f6e 6461 2e69 6f2f 646f 6373 2f29 0a20  onda.io/docs/). 
-00000560: 2020 2061 6e64 205b 616e 6163 6f6e 6461     and [anaconda
-00000570: 2e6f 7267 5d28 6874 7470 733a 2f2f 616e  .org](https://an
-00000580: 6163 6f6e 6461 2e6f 7267 2f6d 6f62 6c65  aconda.org/moble
-00000590: 2f73 7069 6e73 6661 7374 292c 2066 6f72  /spinsfast), for
-000005a0: 2065 6173 6965 7374 2069 6e73 7461 6c6c   easiest install
-000005b0: 6174 696f 6e0a 2020 2020 285b 7365 6520  ation.    ([see 
-000005c0: 6265 6c6f 775d 2823 696e 7374 616c 6c61  below](#installa
-000005d0: 7469 6f6e 2929 2e0a 0a23 204c 6963 656e  tion))...# Licen
-000005e0: 7365 0a0a 5468 6520 6f72 6967 696e 616c  se..The original
-000005f0: 2077 6f72 6b20 6973 206c 6963 656e 7365   work is license
-00000600: 6420 756e 6465 7220 4750 4c2c 2073 6f20  d under GPL, so 
-00000610: 7468 6174 2773 2077 6861 7420 4920 6861  that's what I ha
-00000620: 7665 2074 6f20 6c69 6365 6e73 6520 7468  ve to license th
-00000630: 6973 0a75 6e64 6572 2061 7320 7765 6c6c  is.under as well
-00000640: 2e20 2028 4920 7573 7561 6c6c 7920 676f  .  (I usually go
-00000650: 2066 6f72 2074 6865 206d 6f72 6520 6c69   for the more li
-00000660: 6265 7261 6c20 4d49 5420 6c69 6365 6e73  beral MIT licens
-00000670: 652c 2062 7574 2047 504c 2069 730a 6669  e, but GPL is.fi
-00000680: 6e65 2e29 2020 5365 6520 7468 6520 604c  ne.)  See the `L
-00000690: 4943 454e 5345 6020 6669 6c65 2069 6e20  ICENSE` file in 
-000006a0: 7468 6973 2064 6972 6563 746f 7279 2066  this directory f
-000006b0: 6f72 206d 6f72 6520 6465 7461 696c 732e  or more details.
-000006c0: 0a0a 4920 6261 7365 6420 6d79 2077 6f72  ..I based my wor
-000006d0: 6b20 6f6e 2048 7566 6665 6e62 6572 6765  k on Huffenberge
-000006e0: 7220 616e 6420 5761 6e64 656c 7427 7320  r and Wandelt's 
-000006f0: 2252 6576 6973 696f 6e20 3130 342c 2031  "Revision 104, 1
-00000700: 3320 4170 7220 3230 3132 222c 0a77 6869  3 Apr 2012",.whi
-00000710: 6368 2069 7320 6375 7272 656e 7420 6173  ch is current as
-00000720: 206f 6620 7468 6973 2077 7269 7469 6e67   of this writing
-00000730: 2028 4175 6775 7374 2032 3031 3529 2e20   (August 2015). 
-00000740: 2057 6865 6e65 7665 7220 4920 6e6f 7469   Whenever I noti
-00000750: 6365 2075 7064 6174 6573 0a6f 6e20 7468  ce updates.on th
-00000760: 6569 7220 656e 642c 2049 2077 696c 6c20  eir end, I will 
-00000770: 676c 6164 6c79 2075 7064 6174 6520 7468  gladly update th
-00000780: 6973 2063 6f64 652c 2073 6f20 6665 656c  is code, so feel
-00000790: 2066 7265 6520 746f 206f 7065 6e20 616e   free to open an
-000007a0: 0a5b 6973 7375 655d 2868 7474 7073 3a2f  .[issue](https:/
-000007b0: 2f67 6974 6875 622e 636f 6d2f 6d6f 626c  /github.com/mobl
-000007c0: 652f 7370 696e 7366 6173 742f 6973 7375  e/spinsfast/issu
-000007d0: 6573 2920 746f 206e 6f74 6966 7920 6d65  es) to notify me
-000007e0: 2e20 2054 6f20 7365 6520 6d6f 7265 0a73  .  To see more.s
-000007f0: 7065 6369 6669 6361 6c6c 7920 7768 6174  pecifically what
-00000800: 2049 2776 6520 6164 6465 642c 206c 6f6f   I've added, loo
-00000810: 6b20 7468 726f 7567 6820 7468 650a 5b63  k through the.[c
-00000820: 6f6d 6d69 7473 5d28 6874 7470 733a 2f2f  ommits](https://
-00000830: 6769 7468 7562 2e63 6f6d 2f6d 6f62 6c65  github.com/moble
-00000840: 2f73 7069 6e73 6661 7374 2f63 6f6d 6d69  /spinsfast/commi
-00000850: 7473 2f6d 6173 7465 7229 3b20 6d79 2063  ts/master); my c
-00000860: 6f6e 7472 6962 7574 696f 6e73 0a61 7265  ontributions.are
-00000870: 206a 7573 7420 6576 6572 7974 6869 6e67   just everything
-00000880: 2073 696e 6365 2074 6865 2069 6e69 7469   since the initi
-00000890: 616c 2063 6f6d 6d69 742e 0a0a 0a23 2045  al commit....# E
-000008a0: 7861 6d70 6c65 2055 7361 6765 0a0a 4120  xample Usage..A 
-000008b0: 636f 6e76 656e 6965 6e74 2069 7079 7468  convenient ipyth
-000008c0: 6f6e 2f6a 7570 7974 6572 206e 6f74 6562  on/jupyter noteb
-000008d0: 6f6f 6b20 6973 2066 6f75 6e64 2069 6e20  ook is found in 
-000008e0: 7468 6520 6065 7861 6d70 6c65 6020 6469  the `example` di
-000008f0: 7265 6374 6f72 792c 2061 6e64 0a63 616e  rectory, and.can
-00000900: 2061 6c73 6f20 6265 0a5b 7669 6577 6564   also be.[viewed
-00000910: 2064 6972 6563 746c 7920 6f6e 6c69 6e65   directly online
-00000920: 5d28 6874 7470 3a2f 2f6e 6276 6965 7765  ](http://nbviewe
-00000930: 722e 6970 7974 686f 6e2e 6f72 672f 6769  r.ipython.org/gi
-00000940: 7468 7562 2f6d 6f62 6c65 2f73 7069 6e73  thub/moble/spins
-00000950: 6661 7374 2f62 6c6f 622f 6d61 7374 6572  fast/blob/master
-00000960: 2f65 7861 6d70 6c65 2f73 7069 6e73 6661  /example/spinsfa
-00000970: 7374 2e69 7079 6e62 292e 0a49 7420 7368  st.ipynb)..It sh
-00000980: 6f77 7320 736f 6d65 2065 7861 6d70 6c65  ows some example
-00000990: 2070 7974 686f 6e20 636f 6465 2074 6861   python code tha
-000009a0: 7420 6361 6e20 6265 2075 7365 6420 746f  t can be used to
-000009b0: 2072 756e 2074 6869 7320 6d6f 6475 6c65   run this module
-000009c0: 2c20 616e 640a 6578 706c 6169 6e73 2073  , and.explains s
-000009d0: 6f6d 6520 6f66 2074 6865 2063 6f6e 7665  ome of the conve
-000009e0: 6e74 696f 6e73 2065 7374 6162 6c69 7368  ntions establish
-000009f0: 6564 2062 7920 7468 6520 6073 7069 6e73  ed by the `spins
-00000a00: 6661 7374 6020 6175 7468 6f72 732e 0a0a  fast` authors...
-00000a10: 496e 2074 6865 2069 6e74 6572 6573 7473  In the interests
-00000a20: 206f 6620 6120 7665 7279 2073 686f 7274   of a very short
-00000a30: 2c20 6578 706c 6963 6974 2065 7861 6d70  , explicit examp
-00000a40: 6c65 2c20 6865 7265 2069 7320 6f6e 6520  le, here is one 
-00000a50: 7573 696e 6720 7261 6e64 6f6d 2060 2865  using random `(e
-00000a60: 6c6c 2c6d 2960 206d 6f64 6573 3a0a 0a60  ll,m)` modes:..`
-00000a70: 6060 7079 7468 6f6e 0a66 726f 6d20 6e75  ``python.from nu
-00000a80: 6d70 792e 7261 6e64 6f6d 2069 6d70 6f72  mpy.random impor
-00000a90: 7420 6e6f 726d 616c 2c20 7365 6564 0a69  t normal, seed.i
-00000aa0: 6d70 6f72 7420 7370 696e 7366 6173 740a  mport spinsfast.
-00000ab0: 0a23 2053 6f6d 6520 626f 696c 6572 706c  .# Some boilerpl
-00000ac0: 6174 6520 666f 7220 7365 7474 696e 6720  ate for setting 
-00000ad0: 7468 696e 6773 2075 703a 0a73 203d 2031  things up:.s = 1
-00000ae0: 2020 2320 7370 696e 2077 6569 6768 7420    # spin weight 
-00000af0: 6f66 2074 6865 2066 6965 6c64 0a6c 6d61  of the field.lma
-00000b00: 7820 3d20 3820 2023 206d 6178 696d 756d  x = 8  # maximum
-00000b10: 2065 6c6c 2076 616c 7565 2075 7365 640a   ell value used.
-00000b20: 4e74 6865 7461 203d 2032 2a6c 6d61 782b  Ntheta = 2*lmax+
-00000b30: 3120 2023 204d 696e 696d 756d 2076 616c  1  # Minimum val
-00000b40: 7565 2066 6f72 2061 6363 7572 6163 790a  ue for accuracy.
-00000b50: 4e70 6869 203d 2032 2a6c 6d61 782b 3120  Nphi = 2*lmax+1 
-00000b60: 2023 204d 696e 696d 756d 2076 616c 7565   # Minimum value
-00000b70: 2066 6f72 2061 6363 7572 6163 790a 4e6c   for accuracy.Nl
-00000b80: 6d20 3d20 7370 696e 7366 6173 742e 4e5f  m = spinsfast.N_
-00000b90: 6c6d 286c 6d61 7829 3b20 2023 2054 6f74  lm(lmax);  # Tot
-00000ba0: 616c 206e 756d 6265 7220 6f66 2063 6f6d  al number of com
-00000bb0: 706c 6578 2063 6f6d 706f 6e65 6e74 7320  plex components 
-00000bc0: 6f66 2074 6865 206d 6f64 6520 6465 636f  of the mode deco
-00000bd0: 6d70 6f73 6974 696f 6e0a 0a23 2060 616c  mposition..# `al
-00000be0: 6d60 2077 696c 6c20 686f 6c64 2074 6865  m` will hold the
-00000bf0: 206d 6f64 6520 636f 6d70 6f6e 656e 7473   mode components
-00000c00: 2061 7320 6469 7363 7573 7365 6420 696e   as discussed in
-00000c10: 2060 6578 616d 706c 652f 7370 696e 7366   `example/spinsf
-00000c20: 6173 742e 6970 796e 6260 0a23 2048 6572  ast.ipynb`.# Her
-00000c30: 6520 7765 206a 7573 7420 6669 6c6c 2069  e we just fill i
-00000c40: 7420 7769 7468 2073 6f6d 6520 7261 6e64  t with some rand
-00000c50: 6f6d 206e 756d 6265 7273 2074 6f20 7465  om numbers to te
-00000c60: 7374 2069 740a 7365 6564 2833 3132 3434  st it.seed(31244
-00000c70: 3332 2920 2023 2053 6565 6420 7468 6520  32)  # Seed the 
-00000c80: 7261 6e64 6f6d 2d6e 756d 6265 7220 6765  random-number ge
-00000c90: 6e65 7261 746f 722c 2066 6f72 2072 6570  nerator, for rep
-00000ca0: 726f 6475 6369 6269 6c69 7479 0a61 6c6d  roducibility.alm
-00000cb0: 203d 206e 6f72 6d61 6c28 7369 7a65 3d28   = normal(size=(
-00000cc0: 4e6c 6d2c 2929 202b 2031 6a2a 6e6f 726d  Nlm,)) + 1j*norm
-00000cd0: 616c 2873 697a 653d 284e 6c6d 2c29 290a  al(size=(Nlm,)).
-00000ce0: 0a23 2054 6869 7320 6973 2074 6865 206b  .# This is the k
-00000cf0: 6579 206c 696e 652c 2077 6865 7265 2073  ey line, where s
-00000d00: 7069 6e73 6661 7374 2063 6f6e 7665 7274  pinsfast convert
-00000d10: 7320 6672 6f6d 2028 656c 6c2c 6d29 206d  s from (ell,m) m
-00000d20: 6f64 6573 2074 6f20 7661 6c75 6573 2069  odes to values i
-00000d30: 6e20 7068 7973 6963 616c 2073 7061 6365  n physical space
-00000d40: 0a66 203d 2020 7370 696e 7366 6173 742e  .f =  spinsfast.
-00000d50: 7361 6c6d 326d 6170 2861 6c6d 2c73 2c6c  salm2map(alm,s,l
-00000d60: 6d61 782c 4e74 6865 7461 2c4e 7068 6929  max,Ntheta,Nphi)
-00000d70: 0a0a 2320 5765 2063 616e 2061 6c73 6f20  ..# We can also 
-00000d80: 636f 6e76 6572 7420 696e 2074 6865 206f  convert in the o
-00000d90: 7070 6f73 6974 6520 6469 7265 6374 696f  pposite directio
-00000da0: 6e20 6c69 6b65 2074 6869 733a 0a61 6c6d  n like this:.alm
-00000db0: 3220 3d20 7370 696e 7366 6173 742e 6d61  2 = spinsfast.ma
-00000dc0: 7032 7361 6c6d 2866 2c73 2c6c 6d61 7829  p2salm(f,s,lmax)
-00000dd0: 0a60 6060 0a0a 0a23 2049 6e73 7461 6c6c  .```...# Install
-00000de0: 6174 696f 6e0a 0a23 2320 416e 6163 6f6e  ation..## Anacon
-00000df0: 6461 0a0a 5468 6f75 6768 206d 616e 7561  da..Though manua
-00000e00: 6c20 696e 7374 616c 6c61 7469 6f6e 2069  l installation i
-00000e10: 7320 706f 7373 6962 6c65 2c20 7468 6520  s possible, the 
-00000e20: 6265 7374 2077 6179 2062 7920 6661 7220  best way by far 
-00000e30: 746f 2073 6174 6973 6679 2074 6865 7365  to satisfy these
-00000e40: 0a64 6570 656e 6465 6e63 6965 7320 6973  .dependencies is
-00000e50: 2074 6f20 7573 6520 7468 6520 5b60 616e   to use the [`an
-00000e60: 6163 6f6e 6461 605d 2868 7474 703a 2f2f  aconda`](http://
-00000e70: 636f 6e74 696e 7575 6d2e 696f 2f64 6f77  continuum.io/dow
-00000e80: 6e6c 6f61 6473 290a 6469 7374 7269 6275  nloads).distribu
-00000e90: 7469 6f6e 2e20 2054 6869 7320 6469 7374  tion.  This dist
-00000ea0: 7269 6275 7469 6f6e 2063 616e 2063 6f2d  ribution can co-
-00000eb0: 6578 6973 7420 7769 7468 2079 6f75 7220  exist with your 
-00000ec0: 7379 7374 656d 2070 7974 686f 6e20 7769  system python wi
-00000ed0: 7468 206e 6f0a 7472 6f75 626c 6520 2d2d  th no.trouble --
-00000ee0: 2079 6f75 2073 696d 706c 7920 6164 6420   you simply add 
-00000ef0: 7468 6520 7061 7468 2074 6f20 616e 6163  the path to anac
-00000f00: 6f6e 6461 2062 6566 6f72 6520 796f 7572  onda before your
-00000f10: 2073 7973 7465 6d20 6578 6563 7574 6162   system executab
-00000f20: 6c65 732e 0a49 7420 696e 7374 616c 6c73  les..It installs
-00000f30: 2069 6e74 6f20 796f 7572 2068 6f6d 6520   into your home 
-00000f40: 6469 7265 6374 6f72 792c 2073 6f20 6974  directory, so it
-00000f50: 2064 6f65 736e 2774 2072 6571 7569 7265   doesn't require
-00000f60: 2072 6f6f 7420 6163 6365 7373 2e20 2049   root access.  I
-00000f70: 740a 6361 6e20 6265 2075 6e69 6e73 7461  t.can be uninsta
-00000f80: 6c6c 6564 2065 6173 696c 792c 2073 696e  lled easily, sin
-00000f90: 6365 2069 7420 6578 6973 7473 2065 6e74  ce it exists ent
-00000fa0: 6972 656c 7920 696e 7369 6465 2069 7473  irely inside its
-00000fb0: 206f 776e 2064 6972 6563 746f 7279 2e0a   own directory..
-00000fc0: 416e 6420 7570 6461 7465 7320 6172 6520  And updates are 
-00000fd0: 7472 6976 6961 6c2e 0a0a 4f6e 6365 2060  trivial...Once `
-00000fe0: 616e 6163 6f6e 6461 6020 6973 2069 6e73  anaconda` is ins
-00000ff0: 7461 6c6c 6564 2c20 7468 6973 2070 6163  talled, this pac
-00001000: 6b61 6765 206d 6179 2062 6520 696e 7374  kage may be inst
-00001010: 616c 6c65 6420 7769 7468 2074 6865 2063  alled with the c
-00001020: 6f6d 6d61 6e64 0a0a 6060 6062 6173 680a  ommand..```bash.
-00001030: 636f 6e64 6120 696e 7374 616c 6c20 2d2d  conda install --
-00001040: 6368 616e 6e65 6c20 636f 6e64 612d 666f  channel conda-fo
-00001050: 7267 6520 7370 696e 7366 6173 740a 6060  rge spinsfast.``
-00001060: 600a 0a4e 6f74 6520 7468 6973 206d 6179  `..Note this may
-00001070: 2061 6c73 6f20 696e 7374 616c 6c20 606e   also install `n
-00001080: 756d 7079 6020 616e 6420 6066 6674 7760  umpy` and `fftw`
-00001090: 2061 7574 6f6d 6174 6963 616c 6c79 2e0a   automatically..
-000010a0: 0a0a 2323 2050 6970 0a0a 5768 696c 6520  ..## Pip..While 
-000010b0: 6765 6e65 7261 6c6c 7920 6c65 7373 2072  generally less r
-000010c0: 6f62 7573 742c 2074 6869 7320 7061 636b  obust, this pack
-000010d0: 6167 6520 6973 2061 6c73 6f20 6176 6169  age is also avai
-000010e0: 6c61 626c 6520 7669 6120 6070 6970 603a  lable via `pip`:
-000010f0: 0a0a 6060 6062 6173 680a 7069 7020 696e  ..```bash.pip in
-00001100: 7374 616c 6c20 7370 696e 7366 6173 740a  stall spinsfast.
-00001110: 6060 600a 0a55 6e66 6f72 7475 6e61 7465  ```..Unfortunate
-00001120: 6c79 2c20 6d61 696e 7461 696e 696e 6720  ly, maintaining 
-00001130: 6269 6e61 7279 2064 6973 7472 6962 7574  binary distribut
-00001140: 696f 6e73 206f 6e20 7069 7020 6973 2074  ions on pip is t
-00001150: 6f6f 2074 696d 652d 636f 6e73 756d 696e  oo time-consumin
-00001160: 672c 2073 6f20 6070 6970 6020 7769 6c6c  g, so `pip` will
-00001170: 2074 7279 2074 6f0a 636f 6d70 696c 6520   try to.compile 
-00001180: 7468 6520 736f 7572 6365 2063 6f64 6520  the source code 
-00001190: 666f 7220 796f 752c 2069 6e20 7768 6963  for you, in whic
-000011a0: 6820 6361 7365 2079 6f75 2077 696c 6c20  h case you will 
-000011b0: 6e65 6564 2074 6f20 6861 7665 2046 4654  need to have FFT
-000011c0: 5720 616e 6420 6120 636f 6d70 696c 6572  W and a compiler
-000011d0: 2069 6e73 7461 6c6c 6564 2e0a 556e 666f   installed..Unfo
-000011e0: 7274 756e 6174 656c 792c 2060 7069 7060  rtunately, `pip`
-000011f0: 2068 6173 206e 6f20 676f 6f64 2077 6179   has no good way
-00001200: 206f 6620 6861 6e64 6c69 6e67 2074 6865   of handling the
-00001210: 7365 2064 6570 656e 6465 6e63 6965 732e  se dependencies.
-00001220: 2020 5365 6520 6265 6c6f 7720 666f 7220    See below for 
-00001230: 656e 7669 726f 6e6d 656e 740a 7661 7269  environment.vari
-00001240: 6162 6c65 7320 796f 7520 6d61 7920 6e65  ables you may ne
-00001250: 6564 2074 6f20 7365 7420 746f 2067 6574  ed to set to get
-00001260: 2063 6f6d 7069 6c61 7469 6f6e 2077 6f72   compilation wor
-00001270: 6b69 6e67 2070 726f 7065 726c 792e 0a0a  king properly...
-00001280: 0a23 2320 4d61 6e75 616c 2069 6e73 7461  .## Manual insta
-00001290: 6c6c 6174 696f 6e0a 0a4d 616e 7561 6c20  llation..Manual 
-000012a0: 696e 7374 616c 6c61 7469 6f6e 206f 6620  installation of 
-000012b0: 7468 6973 2070 6163 6b61 6765 2069 7320  this package is 
-000012c0: 736c 6967 6874 6c79 206d 6f72 6520 6465  slightly more de
-000012d0: 6c69 6361 7465 2e20 2054 6865 0a5b 4646  licate.  The.[FF
-000012e0: 5457 2070 6163 6b61 6765 5d28 6874 7470  TW package](http
-000012f0: 3a2f 2f77 7777 2e66 6674 772e 6f72 672f  ://www.fftw.org/
-00001300: 2920 6d75 7374 2062 6520 696e 7374 616c  ) must be instal
-00001310: 6c65 6420 6669 7273 742e 2020 5468 6973  led first.  This
-00001320: 2069 7320 7573 7561 6c6c 790a 7665 7279   is usually.very
-00001330: 2073 696d 706c 652e 2020 4275 7420 7468   simple.  But th
-00001340: 6520 7265 7375 6c74 696e 6720 6865 6164  e resulting head
-00001350: 6572 2061 6e64 206c 6962 7261 7279 206d  er and library m
-00001360: 7573 7420 6265 2066 6f75 6e64 2062 7920  ust be found by 
-00001370: 7468 650a 636f 6d70 696c 6174 696f 6e20  the.compilation 
-00001380: 7374 6570 2066 6f72 2074 6869 7320 7061  step for this pa
-00001390: 636b 6167 652e 2020 596f 7520 6361 6e20  ckage.  You can 
-000013a0: 6669 7273 7420 7369 6d70 6c79 2074 7279  first simply try
-000013b0: 2074 6f20 7275 6e0a 0a60 6060 6261 7368   to run..```bash
-000013c0: 0a70 7974 686f 6e20 7365 7475 702e 7079  .python setup.py
-000013d0: 2069 6e73 7461 6c6c 0a60 6060 0a0a 6672   install.```..fr
-000013e0: 6f6d 2074 6865 2074 6f70 2064 6972 6563  om the top direc
-000013f0: 746f 7279 206f 6620 7468 6520 6073 7069  tory of the `spi
-00001400: 6e73 6661 7374 6020 636f 6465 2e0a 0a49  nsfast` code...I
-00001410: 6620 7468 6973 2064 6f65 736e 2774 2077  f this doesn't w
-00001420: 6f72 6b2c 2079 6f75 2063 616e 2072 6561  ork, you can rea
-00001430: 6420 7468 6520 6572 726f 7220 6d65 7373  d the error mess
-00001440: 6167 652c 2062 7574 2074 6865 206d 6f73  age, but the mos
-00001450: 7420 6c69 6b65 6c79 0a70 726f 626c 656d  t likely.problem
-00001460: 2069 7320 7468 6174 2074 6865 2063 6f6d   is that the com
-00001470: 7069 6c65 7220 6361 6e6e 6f74 2066 696e  piler cannot fin
-00001480: 6420 7468 6520 6066 6674 7760 2068 6561  d the `fftw` hea
-00001490: 6465 722c 206f 7220 7468 6520 6c69 6e6b  der, or the link
-000014a0: 6572 0a63 616e 6e6f 7420 6669 6e64 2074  er.cannot find t
-000014b0: 6865 2060 6666 7477 6020 6c69 6272 6172  he `fftw` librar
-000014c0: 792e 2020 546f 2073 6f6c 7665 2074 6865  y.  To solve the
-000014d0: 7365 2070 726f 626c 656d 732c 2079 6f75  se problems, you
-000014e0: 2077 696c 6c20 6e65 6564 2074 6f20 7275   will need to ru
-000014f0: 6e0a 736f 6d65 7468 696e 6720 6d6f 7265  n.something more
-00001500: 206c 696b 6520 7468 6973 3a0a 0a60 6060   like this:..```
-00001510: 6261 7368 0a65 7870 6f72 7420 4c49 4252  bash.export LIBR
-00001520: 4152 595f 5041 5448 3d2f 7061 7468 2f74  ARY_PATH=/path/t
-00001530: 6f2f 6666 7477 2f6c 6962 0a65 7870 6f72  o/fftw/lib.expor
-00001540: 7420 435f 494e 434c 5544 455f 5041 5448  t C_INCLUDE_PATH
-00001550: 3d2f 7061 7468 2f74 6f2f 6666 7477 2f69  =/path/to/fftw/i
-00001560: 6e63 6c75 6465 0a70 7974 686f 6e20 7365  nclude.python se
-00001570: 7475 702e 7079 2069 6e73 7461 6c6c 0a60  tup.py install.`
-00001580: 6060 0a0a 416c 7465 726e 6174 6976 656c  ``..Alternativel
-00001590: 792c 2079 6f75 2063 6f75 6c64 2074 7279  y, you could try
-000015a0: 2074 6f20 616c 7465 7220 6073 6574 7570   to alter `setup
-000015b0: 2e70 7960 2074 6f20 706f 696e 7420 746f  .py` to point to
-000015c0: 2074 6865 2072 6967 6874 0a70 6174 6873   the right.paths
-000015d0: 2e0a 0a0a 2320 4f72 6967 696e 616c 2069  ....# Original i
-000015e0: 6e73 7461 6c6c 6174 696f 6e20 696e 7374  nstallation inst
-000015f0: 7275 6374 696f 6e73 0a0a 5468 6f75 6768  ructions..Though
-00001600: 2074 6865 7365 2061 7265 206e 6f74 206e   these are not n
-00001610: 6563 6573 7361 7279 2066 6f72 2069 6e73  ecessary for ins
-00001620: 7461 6c6c 696e 6720 7468 6520 7079 7468  talling the pyth
-00001630: 6f6e 206d 6f64 756c 652c 2074 6865 2066  on module, the f
-00001640: 6f6c 6c6f 7769 6e67 0a61 7265 2074 6865  ollowing.are the
-00001650: 2069 6e73 7472 7563 7469 6f6e 7320 696e   instructions in
-00001660: 2074 6865 206f 7269 6769 6e61 6c20 736f   the original so
-00001670: 7572 6365 2063 6f64 6520 666f 7220 6275  urce code for bu
-00001680: 696c 6469 6e67 2074 6865 2043 2063 6f64  ilding the C cod
-00001690: 652e 0a0a 4765 7420 7468 6520 6c61 7465  e...Get the late
-000016a0: 7374 2076 6572 7369 6f6e 2061 743a 0a0a  st version at:..
-000016b0: 2020 2020 6874 7470 3a2f 2f77 7777 2e70      http://www.p
-000016c0: 6879 7369 6373 2e6d 6961 6d69 2e65 6475  hysics.miami.edu
-000016d0: 2f7e 6875 6666 656e 6265 2f72 6573 6561  /~huffenbe/resea
-000016e0: 7263 682f 7370 696e 7366 6173 742f 0a0a  rch/spinsfast/..
-000016f0: 2323 2043 6f6d 7069 6c61 7469 6f6e 2069  ## Compilation i
-00001700: 6e73 7472 7563 7469 6f6e 730a 0a20 2031  nstructions..  1
-00001710: 2e20 4564 6974 2074 6865 2066 696c 6520  . Edit the file 
-00001720: 286f 7220 6d61 6b65 2061 206e 6577 2066  (or make a new f
-00001730: 696c 6529 2063 616c 6c65 6420 6275 696c  ile) called buil
-00001740: 642f 636f 6e66 6967 2e6d 6b20 736f 2074  d/config.mk so t
-00001750: 6861 7420 7468 6520 7072 6f70 6572 206c  hat the proper l
-00001760: 6f63 6174 696f 6e73 2066 6f72 2068 6561  ocations for hea
-00001770: 6465 7220 616e 6420 6c69 6272 6172 7920  der and library 
-00001780: 6669 6c65 7320 6172 6520 696e 636c 7564  files are includ
-00001790: 6564 2e0a 0a20 2032 2e20 5365 7420 7468  ed...  2. Set th
-000017a0: 6520 656e 7669 726f 6e6d 656e 7420 7661  e environment va
-000017b0: 7269 6162 6c65 2022 6275 696c 6422 2073  riable "build" s
-000017c0: 6f20 7468 6174 2069 7420 706f 696e 7473  o that it points
-000017d0: 2074 6f20 7468 6174 2066 696c 652e 2049   to that file. I
-000017e0: 2e65 2e2c 2069 6e20 6261 7368 2c20 7361  .e., in bash, sa
-000017f0: 790a 0a20 2020 2020 2020 2065 7870 6f72  y..        expor
-00001800: 7420 6275 696c 643d 6275 696c 642f 636f  t build=build/co
-00001810: 6e66 6967 2e6d 6b20 0a0a 2020 332e 2042  nfig.mk ..  3. B
-00001820: 7569 6c64 2074 6865 206c 6962 7261 7279  uild the library
-00001830: 2061 6e64 2065 7861 6d70 6c65 2063 6f64   and example cod
-00001840: 6573 2077 6974 6820 0a0a 2020 2020 2020  es with ..      
-00001850: 2020 6d61 6b65 0a0a 2323 2028 4f70 7469    make..## (Opti
-00001860: 6f6e 616c 2920 4368 6563 6b69 6e67 2074  onal) Checking t
-00001870: 6865 2063 6f6d 7069 6c61 7469 6f6e 0a0a  he compilation..
-00001880: 5275 6e20 7468 6520 6578 616d 706c 6520  Run the example 
-00001890: 636f 6465 2066 6f6c 6c6f 7769 6e67 2074  code following t
-000018a0: 6865 2069 6e73 7472 7563 7469 6f6e 7320  he instructions 
-000018b0: 6174 200a 0a20 2020 2068 7474 703a 2f2f  at ..    http://
-000018c0: 7777 772e 7068 7973 6963 732e 6d69 616d  www.physics.miam
-000018d0: 692e 6564 752f 7e68 7566 6665 6e62 652f  i.edu/~huffenbe/
-000018e0: 7265 7365 6172 6368 2f73 7069 6e73 6661  research/spinsfa
-000018f0: 7374 2f0a                                st/.
+00000000: 5b21 5b42 7569 6c64 5d28 6874 7470 733a  [![Build](https:
+00000010: 2f2f 6769 7468 7562 2e63 6f6d 2f6d 6f62  //github.com/mob
+00000020: 6c65 2f73 7069 6e73 6661 7374 2f61 6374  le/spinsfast/act
+00000030: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f62  ions/workflows/b
+00000040: 7569 6c64 2e79 6d6c 2f62 6164 6765 2e73  uild.yml/badge.s
+00000050: 7667 295d 2868 7474 7073 3a2f 2f67 6974  vg)](https://git
+00000060: 6875 622e 636f 6d2f 6d6f 626c 652f 7370  hub.com/moble/sp
+00000070: 696e 7366 6173 742f 6163 7469 6f6e 732f  insfast/actions/
+00000080: 776f 726b 666c 6f77 732f 6275 696c 642e  workflows/build.
+00000090: 796d 6c29 0a5b 215b 5079 5049 2056 6572  yml).[![PyPI Ver
+000000a0: 7369 6f6e 5d28 6874 7470 733a 2f2f 696d  sion](https://im
+000000b0: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
+000000c0: 692f 762f 7370 696e 7366 6173 743f 636f  i/v/spinsfast?co
+000000d0: 6c6f 723d 295d 2868 7474 7073 3a2f 2f70  lor=)](https://p
+000000e0: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
+000000f0: 7370 696e 7366 6173 742f 290a 5b21 5b43  spinsfast/).[![C
+00000100: 6f6e 6461 2056 6572 7369 6f6e 5d28 6874  onda Version](ht
+00000110: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000120: 732e 696f 2f63 6f6e 6461 2f76 6e2f 636f  s.io/conda/vn/co
+00000130: 6e64 612d 666f 7267 652f 7370 696e 7366  nda-forge/spinsf
+00000140: 6173 742e 7376 673f 636f 6c6f 723d 295d  ast.svg?color=)]
+00000150: 2868 7474 7073 3a2f 2f61 6e61 636f 6e64  (https://anacond
+00000160: 612e 6f72 672f 636f 6e64 612d 666f 7267  a.org/conda-forg
+00000170: 652f 7370 696e 7366 6173 7429 0a5b 215b  e/spinsfast).[![
+00000180: 4750 4c2d 332e 3020 4c69 6365 6e73 655d  GPL-3.0 License]
+00000190: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+000001a0: 656c 6473 2e69 6f2f 6769 7468 7562 2f6c  elds.io/github/l
+000001b0: 6963 656e 7365 2f6d 6f62 6c65 2f73 7069  icense/moble/spi
+000001c0: 6e73 6661 7374 2e73 7667 295d 2868 7474  nsfast.svg)](htt
+000001d0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000001e0: 6d6f 626c 652f 7370 696e 7366 6173 742f  moble/spinsfast/
+000001f0: 626c 6f62 2f6d 6169 6e2f 4c49 4345 4e53  blob/main/LICENS
+00000200: 4529 0a5b 215b 444f 495d 2868 7474 7073  E).[![DOI](https
+00000210: 3a2f 2f7a 656e 6f64 6f2e 6f72 672f 6261  ://zenodo.org/ba
+00000220: 6467 652f 3330 3334 3035 3832 2e73 7667  dge/30340582.svg
+00000230: 295d 2868 7474 7073 3a2f 2f7a 656e 6f64  )](https://zenod
+00000240: 6f2e 6f72 672f 6261 6467 652f 6c61 7465  o.org/badge/late
+00000250: 7374 646f 692f 3330 3334 3035 3832 290a  stdoi/30340582).
+00000260: 0a23 2073 7069 6e73 6661 7374 0a46 6173  .# spinsfast.Fas
+00000270: 7420 616e 6420 6578 6163 7420 7370 696e  t and exact spin
+00000280: 2d73 2073 7068 6572 6963 616c 2d68 6172  -s spherical-har
+00000290: 6d6f 6e69 6320 7472 616e 7366 6f72 6d73  monic transforms
+000002a0: 0a0a 5468 6973 2063 6f64 6520 6973 2061  ..This code is a
+000002b0: 206c 6967 6874 6c79 206d 6f64 6966 6965   lightly modifie
+000002c0: 6420 7665 7273 696f 6e20 6f66 2074 6865  d version of the
+000002d0: 2063 6f64 6520 686f 7374 6564 0a5b 6865   code hosted.[he
+000002e0: 7265 5d28 6874 7470 3a2f 2f61 7374 726f  re](http://astro
+000002f0: 7068 7973 6963 732e 7068 7973 6963 732e  physics.physics.
+00000300: 6673 752e 6564 752f 7e68 7566 6665 6e62  fsu.edu/~huffenb
+00000310: 652f 7265 7365 6172 6368 2f73 7069 6e73  e/research/spins
+00000320: 6661 7374 2f69 6e64 6578 2e68 746d 6c29  fast/index.html)
+00000330: 0a62 7920 4875 6666 656e 6265 7267 6572  .by Huffenberger
+00000340: 2c20 6261 7365 6420 6f6e 2077 6f72 6b20  , based on work 
+00000350: 6279 0a5b 4875 6666 656e 6265 7267 6572  by.[Huffenberger
+00000360: 2061 6e64 2057 616e 6465 6c74 5d28 6874   and Wandelt](ht
+00000370: 7470 3a2f 2f73 7461 636b 732e 696f 702e  tp://stacks.iop.
+00000380: 6f72 672f 3030 3637 2d30 3034 392f 3138  org/0067-0049/18
+00000390: 392f 3235 3529 2e0a 0a4d 7920 6d6f 6469  9/255)...My modi
+000003a0: 6669 6361 7469 6f6e 7320 6d6f 7374 6c79  fications mostly
+000003b0: 2064 6561 6c20 7769 7468 2074 6865 2075   deal with the u
+000003c0: 7365 7220 696e 7465 7266 6163 653a 0a0a  ser interface:..
+000003d0: 2020 2a20 6164 6420 606d 756c 7469 5f6d    * add `multi_m
+000003e0: 6170 3273 616c 6d60 2061 6e64 2060 6d75  ap2salm` and `mu
+000003f0: 6c74 695f 7361 6c6d 326d 6170 6020 666f  lti_salm2map` fo
+00000400: 7220 7275 6e6e 696e 6720 6d61 6e79 2073  r running many s
+00000410: 696d 696c 6172 2074 7261 6e73 666f 726d  imilar transform
+00000420: 6174 696f 6e73 2065 6666 6963 6965 6e74  ations efficient
+00000430: 6c79 3b0a 2020 2a20 6372 6561 7465 2070  ly;.  * create p
+00000440: 7974 686f 6e20 7772 6170 7065 7273 2066  ython wrappers f
+00000450: 6f72 2074 6865 2060 6d61 7032 7361 6c6d  or the `map2salm
+00000460: 6020 616e 6420 6073 616c 6d32 6d61 7060  ` and `salm2map`
+00000470: 2066 756e 6374 696f 6e73 2074 6f20 6465   functions to de
+00000480: 616c 2077 6974 6820 616e 7920 2872 6561  al with any (rea
+00000490: 736f 6e61 626c 6529 0a20 2020 2074 7970  sonable).    typ
+000004a0: 6520 6f72 2073 6861 7065 206f 6620 696e  e or shape of in
+000004b0: 7075 7420 6461 7461 2c20 696e 636c 7564  put data, includ
+000004c0: 696e 6720 6d75 6c74 692d 6469 6d65 6e73  ing multi-dimens
+000004d0: 696f 6e61 6c3b 0a20 202a 2061 6464 2070  ional;.  * add p
+000004e0: 7974 686f 6e20 332e 7820 636f 6d70 6174  ython 3.x compat
+000004f0: 6962 696c 6974 7920 746f 2060 7079 7468  ibility to `pyth
+00000500: 6f6e 2f73 7069 6e73 6661 7374 5f6d 6f64  on/spinsfast_mod
+00000510: 756c 652e 6360 3b0a 2020 2a20 6669 7820  ule.c`;.  * fix 
+00000520: 7365 6766 6175 6c74 7320 6475 6520 746f  segfaults due to
+00000530: 2075 7365 206f 6620 6066 7265 6560 2069   use of `free` i
+00000540: 6e73 7465 6164 206f 6620 6066 6674 775f  nstead of `fftw_
+00000550: 6672 6565 6020 7768 656e 2060 6666 7477  free` when `fftw
+00000560: 5f6d 616c 6c6f 6360 2077 6173 2075 7365  _malloc` was use
+00000570: 643b 0a20 202a 206d 616b 6520 6974 2065  d;.  * make it e
+00000580: 6173 6965 7220 746f 2069 6e73 7461 6c6c  asier to install
+00000590: 2061 7320 6120 7079 7468 6f6e 206d 6f64   as a python mod
+000005a0: 756c 6520 6279 2074 7279 696e 6720 746f  ule by trying to
+000005b0: 2064 6574 6563 7420 7061 7468 7320 746f   detect paths to
+000005c0: 0a20 2020 2046 4654 573b 0a20 202a 2066  .    FFTW;.  * f
+000005d0: 6978 206e 756d 6572 6f75 7320 6d61 7373  ix numerous mass
+000005e0: 6976 6520 6d65 6d6f 7279 206c 6561 6b73  ive memory leaks
+000005f0: 2069 6e20 7079 7468 6f6e 2065 7874 656e   in python exten
+00000600: 7369 6f6e 206d 6f64 756c 653b 0a20 202a  sion module;.  *
+00000610: 2069 6e63 6c75 6465 2061 6e20 6970 7974   include an ipyt
+00000620: 686f 6e2f 6a75 7079 7465 7220 6e6f 7465  hon/jupyter note
+00000630: 626f 6f6b 2069 6e20 7468 6520 6065 7861  book in the `exa
+00000640: 6d70 6c65 6020 6469 7265 6374 6f72 793b  mple` directory;
+00000650: 0a20 202a 2061 6464 2069 6e74 6567 7261  .  * add integra
+00000660: 7469 6f6e 2077 6974 6820 5b70 6970 5d28  tion with [pip](
+00000670: 6874 7470 733a 2f2f 7079 7069 2e70 7974  https://pypi.pyt
+00000680: 686f 6e2e 6f72 672f 7079 7069 2f70 6970  hon.org/pypi/pip
+00000690: 290a 2020 2020 616e 6420 5b70 7970 695d  ).    and [pypi]
+000006a0: 2868 7474 7073 3a2f 2f70 7970 692e 7079  (https://pypi.py
+000006b0: 7468 6f6e 2e6f 7267 2f70 7970 692f 7370  thon.org/pypi/sp
+000006c0: 696e 7366 6173 7429 2c20 666f 7220 6561  insfast), for ea
+000006d0: 7379 2069 6e73 7461 6c6c 6174 696f 6e0a  sy installation.
+000006e0: 2020 2020 285b 7365 6520 6265 6c6f 775d      ([see below]
+000006f0: 2823 696e 7374 616c 6c61 7469 6f6e 2929  (#installation))
+00000700: 3b0a 2020 2a20 6164 6420 696e 7465 6772  ;.  * add integr
+00000710: 6174 696f 6e20 7769 7468 205b 636f 6e64  ation with [cond
+00000720: 615d 2868 7474 7073 3a2f 2f63 6f6e 6461  a](https://conda
+00000730: 2e69 6f2f 646f 6373 2f29 0a20 2020 2061  .io/docs/).    a
+00000740: 6e64 205b 616e 6163 6f6e 6461 2e6f 7267  nd [anaconda.org
+00000750: 5d28 6874 7470 733a 2f2f 616e 6163 6f6e  ](https://anacon
+00000760: 6461 2e6f 7267 2f6d 6f62 6c65 2f73 7069  da.org/moble/spi
+00000770: 6e73 6661 7374 292c 2066 6f72 2065 6173  nsfast), for eas
+00000780: 6965 7374 2069 6e73 7461 6c6c 6174 696f  iest installatio
+00000790: 6e0a 2020 2020 285b 7365 6520 6265 6c6f  n.    ([see belo
+000007a0: 775d 2823 696e 7374 616c 6c61 7469 6f6e  w](#installation
+000007b0: 2929 2e0a 0a23 204c 6963 656e 7365 0a0a  ))...# License..
+000007c0: 5468 6520 6f72 6967 696e 616c 2077 6f72  The original wor
+000007d0: 6b20 6973 206c 6963 656e 7365 6420 756e  k is licensed un
+000007e0: 6465 7220 4750 4c2c 2073 6f20 7468 6174  der GPL, so that
+000007f0: 2773 2077 6861 7420 4920 6861 7665 2074  's what I have t
+00000800: 6f20 6c69 6365 6e73 6520 7468 6973 0a75  o license this.u
+00000810: 6e64 6572 2061 7320 7765 6c6c 2e20 2028  nder as well.  (
+00000820: 4920 7573 7561 6c6c 7920 676f 2066 6f72  I usually go for
+00000830: 2074 6865 206d 6f72 6520 6c69 6265 7261   the more libera
+00000840: 6c20 4d49 5420 6c69 6365 6e73 652c 2062  l MIT license, b
+00000850: 7574 2047 504c 2069 730a 6669 6e65 2e29  ut GPL is.fine.)
+00000860: 2020 5365 6520 7468 6520 604c 4943 454e    See the `LICEN
+00000870: 5345 6020 6669 6c65 2069 6e20 7468 6973  SE` file in this
+00000880: 2064 6972 6563 746f 7279 2066 6f72 206d   directory for m
+00000890: 6f72 6520 6465 7461 696c 732e 0a0a 4920  ore details...I 
+000008a0: 6261 7365 6420 6d79 2077 6f72 6b20 6f6e  based my work on
+000008b0: 2048 7566 6665 6e62 6572 6765 7220 616e   Huffenberger an
+000008c0: 6420 5761 6e64 656c 7427 7320 2252 6576  d Wandelt's "Rev
+000008d0: 6973 696f 6e20 3130 342c 2031 3320 4170  ision 104, 13 Ap
+000008e0: 7220 3230 3132 222c 0a77 6869 6368 2069  r 2012",.which i
+000008f0: 7320 6375 7272 656e 7420 6173 206f 6620  s current as of 
+00000900: 7468 6973 2077 7269 7469 6e67 2028 4175  this writing (Au
+00000910: 6775 7374 2032 3031 3529 2e20 2057 6865  gust 2015).  Whe
+00000920: 6e65 7665 7220 4920 6e6f 7469 6365 2075  never I notice u
+00000930: 7064 6174 6573 0a6f 6e20 7468 6569 7220  pdates.on their 
+00000940: 656e 642c 2049 2077 696c 6c20 676c 6164  end, I will glad
+00000950: 6c79 2075 7064 6174 6520 7468 6973 2063  ly update this c
+00000960: 6f64 652c 2073 6f20 6665 656c 2066 7265  ode, so feel fre
+00000970: 6520 746f 206f 7065 6e20 616e 0a5b 6973  e to open an.[is
+00000980: 7375 655d 2868 7474 7073 3a2f 2f67 6974  sue](https://git
+00000990: 6875 622e 636f 6d2f 6d6f 626c 652f 7370  hub.com/moble/sp
+000009a0: 696e 7366 6173 742f 6973 7375 6573 2920  insfast/issues) 
+000009b0: 746f 206e 6f74 6966 7920 6d65 2e20 2054  to notify me.  T
+000009c0: 6f20 7365 6520 6d6f 7265 0a73 7065 6369  o see more.speci
+000009d0: 6669 6361 6c6c 7920 7768 6174 2049 2776  fically what I'v
+000009e0: 6520 6164 6465 642c 206c 6f6f 6b20 7468  e added, look th
+000009f0: 726f 7567 6820 7468 650a 5b63 6f6d 6d69  rough the.[commi
+00000a00: 7473 5d28 6874 7470 733a 2f2f 6769 7468  ts](https://gith
+00000a10: 7562 2e63 6f6d 2f6d 6f62 6c65 2f73 7069  ub.com/moble/spi
+00000a20: 6e73 6661 7374 2f63 6f6d 6d69 7473 2f6d  nsfast/commits/m
+00000a30: 6173 7465 7229 3b20 6d79 2063 6f6e 7472  aster); my contr
+00000a40: 6962 7574 696f 6e73 0a61 7265 206a 7573  ibutions.are jus
+00000a50: 7420 6576 6572 7974 6869 6e67 2073 696e  t everything sin
+00000a60: 6365 2074 6865 2069 6e69 7469 616c 2063  ce the initial c
+00000a70: 6f6d 6d69 742e 0a0a 0a23 2045 7861 6d70  ommit....# Examp
+00000a80: 6c65 2055 7361 6765 0a0a 4120 636f 6e76  le Usage..A conv
+00000a90: 656e 6965 6e74 2069 7079 7468 6f6e 2f6a  enient ipython/j
+00000aa0: 7570 7974 6572 206e 6f74 6562 6f6f 6b20  upyter notebook 
+00000ab0: 6973 2066 6f75 6e64 2069 6e20 7468 6520  is found in the 
+00000ac0: 6065 7861 6d70 6c65 6020 6469 7265 6374  `example` direct
+00000ad0: 6f72 792c 2061 6e64 0a63 616e 2061 6c73  ory, and.can als
+00000ae0: 6f20 6265 0a5b 7669 6577 6564 2064 6972  o be.[viewed dir
+00000af0: 6563 746c 7920 6f6e 6c69 6e65 5d28 6874  ectly online](ht
+00000b00: 7470 3a2f 2f6e 6276 6965 7765 722e 6970  tp://nbviewer.ip
+00000b10: 7974 686f 6e2e 6f72 672f 6769 7468 7562  ython.org/github
+00000b20: 2f6d 6f62 6c65 2f73 7069 6e73 6661 7374  /moble/spinsfast
+00000b30: 2f62 6c6f 622f 6d61 7374 6572 2f65 7861  /blob/master/exa
+00000b40: 6d70 6c65 2f73 7069 6e73 6661 7374 2e69  mple/spinsfast.i
+00000b50: 7079 6e62 292e 0a49 7420 7368 6f77 7320  pynb)..It shows 
+00000b60: 736f 6d65 2065 7861 6d70 6c65 2070 7974  some example pyt
+00000b70: 686f 6e20 636f 6465 2074 6861 7420 6361  hon code that ca
+00000b80: 6e20 6265 2075 7365 6420 746f 2072 756e  n be used to run
+00000b90: 2074 6869 7320 6d6f 6475 6c65 2c20 616e   this module, an
+00000ba0: 640a 6578 706c 6169 6e73 2073 6f6d 6520  d.explains some 
+00000bb0: 6f66 2074 6865 2063 6f6e 7665 6e74 696f  of the conventio
+00000bc0: 6e73 2065 7374 6162 6c69 7368 6564 2062  ns established b
+00000bd0: 7920 7468 6520 6073 7069 6e73 6661 7374  y the `spinsfast
+00000be0: 6020 6175 7468 6f72 732e 0a0a 496e 2074  ` authors...In t
+00000bf0: 6865 2069 6e74 6572 6573 7473 206f 6620  he interests of 
+00000c00: 6120 7665 7279 2073 686f 7274 2c20 6578  a very short, ex
+00000c10: 706c 6963 6974 2065 7861 6d70 6c65 2c20  plicit example, 
+00000c20: 6865 7265 2069 7320 6f6e 6520 7573 696e  here is one usin
+00000c30: 6720 7261 6e64 6f6d 2060 2865 6c6c 2c6d  g random `(ell,m
+00000c40: 2960 206d 6f64 6573 3a0a 0a60 6060 7079  )` modes:..```py
+00000c50: 7468 6f6e 0a66 726f 6d20 6e75 6d70 792e  thon.from numpy.
+00000c60: 7261 6e64 6f6d 2069 6d70 6f72 7420 6e6f  random import no
+00000c70: 726d 616c 2c20 7365 6564 0a69 6d70 6f72  rmal, seed.impor
+00000c80: 7420 7370 696e 7366 6173 740a 0a23 2053  t spinsfast..# S
+00000c90: 6f6d 6520 626f 696c 6572 706c 6174 6520  ome boilerplate 
+00000ca0: 666f 7220 7365 7474 696e 6720 7468 696e  for setting thin
+00000cb0: 6773 2075 703a 0a73 203d 2031 2020 2320  gs up:.s = 1  # 
+00000cc0: 7370 696e 2077 6569 6768 7420 6f66 2074  spin weight of t
+00000cd0: 6865 2066 6965 6c64 0a6c 6d61 7820 3d20  he field.lmax = 
+00000ce0: 3820 2023 206d 6178 696d 756d 2065 6c6c  8  # maximum ell
+00000cf0: 2076 616c 7565 2075 7365 640a 4e74 6865   value used.Nthe
+00000d00: 7461 203d 2032 2a6c 6d61 782b 3120 2023  ta = 2*lmax+1  #
+00000d10: 204d 696e 696d 756d 2076 616c 7565 2066   Minimum value f
+00000d20: 6f72 2061 6363 7572 6163 790a 4e70 6869  or accuracy.Nphi
+00000d30: 203d 2032 2a6c 6d61 782b 3120 2023 204d   = 2*lmax+1  # M
+00000d40: 696e 696d 756d 2076 616c 7565 2066 6f72  inimum value for
+00000d50: 2061 6363 7572 6163 790a 4e6c 6d20 3d20   accuracy.Nlm = 
+00000d60: 7370 696e 7366 6173 742e 4e5f 6c6d 286c  spinsfast.N_lm(l
+00000d70: 6d61 7829 3b20 2023 2054 6f74 616c 206e  max);  # Total n
+00000d80: 756d 6265 7220 6f66 2063 6f6d 706c 6578  umber of complex
+00000d90: 2063 6f6d 706f 6e65 6e74 7320 6f66 2074   components of t
+00000da0: 6865 206d 6f64 6520 6465 636f 6d70 6f73  he mode decompos
+00000db0: 6974 696f 6e0a 0a23 2060 616c 6d60 2077  ition..# `alm` w
+00000dc0: 696c 6c20 686f 6c64 2074 6865 206d 6f64  ill hold the mod
+00000dd0: 6520 636f 6d70 6f6e 656e 7473 2061 7320  e components as 
+00000de0: 6469 7363 7573 7365 6420 696e 2060 6578  discussed in `ex
+00000df0: 616d 706c 652f 7370 696e 7366 6173 742e  ample/spinsfast.
+00000e00: 6970 796e 6260 0a23 2048 6572 6520 7765  ipynb`.# Here we
+00000e10: 206a 7573 7420 6669 6c6c 2069 7420 7769   just fill it wi
+00000e20: 7468 2073 6f6d 6520 7261 6e64 6f6d 206e  th some random n
+00000e30: 756d 6265 7273 2074 6f20 7465 7374 2069  umbers to test i
+00000e40: 740a 7365 6564 2833 3132 3434 3332 2920  t.seed(3124432) 
+00000e50: 2023 2053 6565 6420 7468 6520 7261 6e64   # Seed the rand
+00000e60: 6f6d 2d6e 756d 6265 7220 6765 6e65 7261  om-number genera
+00000e70: 746f 722c 2066 6f72 2072 6570 726f 6475  tor, for reprodu
+00000e80: 6369 6269 6c69 7479 0a61 6c6d 203d 206e  cibility.alm = n
+00000e90: 6f72 6d61 6c28 7369 7a65 3d28 4e6c 6d2c  ormal(size=(Nlm,
+00000ea0: 2929 202b 2031 6a2a 6e6f 726d 616c 2873  )) + 1j*normal(s
+00000eb0: 697a 653d 284e 6c6d 2c29 290a 0a23 2054  ize=(Nlm,))..# T
+00000ec0: 6869 7320 6973 2074 6865 206b 6579 206c  his is the key l
+00000ed0: 696e 652c 2077 6865 7265 2073 7069 6e73  ine, where spins
+00000ee0: 6661 7374 2063 6f6e 7665 7274 7320 6672  fast converts fr
+00000ef0: 6f6d 2028 656c 6c2c 6d29 206d 6f64 6573  om (ell,m) modes
+00000f00: 2074 6f20 7661 6c75 6573 2069 6e20 7068   to values in ph
+00000f10: 7973 6963 616c 2073 7061 6365 0a66 203d  ysical space.f =
+00000f20: 2020 7370 696e 7366 6173 742e 7361 6c6d    spinsfast.salm
+00000f30: 326d 6170 2861 6c6d 2c73 2c6c 6d61 782c  2map(alm,s,lmax,
+00000f40: 4e74 6865 7461 2c4e 7068 6929 0a0a 2320  Ntheta,Nphi)..# 
+00000f50: 5765 2063 616e 2061 6c73 6f20 636f 6e76  We can also conv
+00000f60: 6572 7420 696e 2074 6865 206f 7070 6f73  ert in the oppos
+00000f70: 6974 6520 6469 7265 6374 696f 6e20 6c69  ite direction li
+00000f80: 6b65 2074 6869 733a 0a61 6c6d 3220 3d20  ke this:.alm2 = 
+00000f90: 7370 696e 7366 6173 742e 6d61 7032 7361  spinsfast.map2sa
+00000fa0: 6c6d 2866 2c73 2c6c 6d61 7829 0a60 6060  lm(f,s,lmax).```
+00000fb0: 0a0a 0a23 2049 6e73 7461 6c6c 6174 696f  ...# Installatio
+00000fc0: 6e0a 0a23 2320 416e 6163 6f6e 6461 0a0a  n..## Anaconda..
+00000fd0: 5468 6f75 6768 206d 616e 7561 6c20 696e  Though manual in
+00000fe0: 7374 616c 6c61 7469 6f6e 2069 7320 706f  stallation is po
+00000ff0: 7373 6962 6c65 2c20 7468 6520 6265 7374  ssible, the best
+00001000: 2077 6179 2062 7920 6661 7220 746f 2073   way by far to s
+00001010: 6174 6973 6679 2074 6865 7365 0a64 6570  atisfy these.dep
+00001020: 656e 6465 6e63 6965 7320 6973 2074 6f20  endencies is to 
+00001030: 7573 6520 7468 6520 5b60 616e 6163 6f6e  use the [`anacon
+00001040: 6461 605d 2868 7474 703a 2f2f 636f 6e74  da`](http://cont
+00001050: 696e 7575 6d2e 696f 2f64 6f77 6e6c 6f61  inuum.io/downloa
+00001060: 6473 290a 6469 7374 7269 6275 7469 6f6e  ds).distribution
+00001070: 2e20 2054 6869 7320 6469 7374 7269 6275  .  This distribu
+00001080: 7469 6f6e 2063 616e 2063 6f2d 6578 6973  tion can co-exis
+00001090: 7420 7769 7468 2079 6f75 7220 7379 7374  t with your syst
+000010a0: 656d 2070 7974 686f 6e20 7769 7468 206e  em python with n
+000010b0: 6f0a 7472 6f75 626c 6520 2d2d 2079 6f75  o.trouble -- you
+000010c0: 2073 696d 706c 7920 6164 6420 7468 6520   simply add the 
+000010d0: 7061 7468 2074 6f20 616e 6163 6f6e 6461  path to anaconda
+000010e0: 2062 6566 6f72 6520 796f 7572 2073 7973   before your sys
+000010f0: 7465 6d20 6578 6563 7574 6162 6c65 732e  tem executables.
+00001100: 0a49 7420 696e 7374 616c 6c73 2069 6e74  .It installs int
+00001110: 6f20 796f 7572 2068 6f6d 6520 6469 7265  o your home dire
+00001120: 6374 6f72 792c 2073 6f20 6974 2064 6f65  ctory, so it doe
+00001130: 736e 2774 2072 6571 7569 7265 2072 6f6f  sn't require roo
+00001140: 7420 6163 6365 7373 2e20 2049 740a 6361  t access.  It.ca
+00001150: 6e20 6265 2075 6e69 6e73 7461 6c6c 6564  n be uninstalled
+00001160: 2065 6173 696c 792c 2073 696e 6365 2069   easily, since i
+00001170: 7420 6578 6973 7473 2065 6e74 6972 656c  t exists entirel
+00001180: 7920 696e 7369 6465 2069 7473 206f 776e  y inside its own
+00001190: 2064 6972 6563 746f 7279 2e0a 416e 6420   directory..And 
+000011a0: 7570 6461 7465 7320 6172 6520 7472 6976  updates are triv
+000011b0: 6961 6c2e 0a0a 4f6e 6365 2060 616e 6163  ial...Once `anac
+000011c0: 6f6e 6461 6020 6973 2069 6e73 7461 6c6c  onda` is install
+000011d0: 6564 2c20 7468 6973 2070 6163 6b61 6765  ed, this package
+000011e0: 206d 6179 2062 6520 696e 7374 616c 6c65   may be installe
+000011f0: 6420 7769 7468 2074 6865 2063 6f6d 6d61  d with the comma
+00001200: 6e64 0a0a 6060 6062 6173 680a 636f 6e64  nd..```bash.cond
+00001210: 6120 696e 7374 616c 6c20 2d2d 6368 616e  a install --chan
+00001220: 6e65 6c20 636f 6e64 612d 666f 7267 6520  nel conda-forge 
+00001230: 7370 696e 7366 6173 740a 6060 600a 0a4e  spinsfast.```..N
+00001240: 6f74 6520 7468 6973 206d 6179 2061 6c73  ote this may als
+00001250: 6f20 696e 7374 616c 6c20 606e 756d 7079  o install `numpy
+00001260: 6020 616e 6420 6066 6674 7760 2061 7574  ` and `fftw` aut
+00001270: 6f6d 6174 6963 616c 6c79 2e0a 0a0a 2323  omatically....##
+00001280: 2050 6970 0a0a 5768 696c 6520 6765 6e65   Pip..While gene
+00001290: 7261 6c6c 7920 6c65 7373 2072 6f62 7573  rally less robus
+000012a0: 742c 2074 6869 7320 7061 636b 6167 6520  t, this package 
+000012b0: 6973 2061 6c73 6f20 6176 6169 6c61 626c  is also availabl
+000012c0: 6520 7669 6120 6070 6970 603a 0a0a 6060  e via `pip`:..``
+000012d0: 6062 6173 680a 7069 7020 696e 7374 616c  `bash.pip instal
+000012e0: 6c20 7370 696e 7366 6173 740a 6060 600a  l spinsfast.```.
+000012f0: 0a55 6e66 6f72 7475 6e61 7465 6c79 2c20  .Unfortunately, 
+00001300: 6d61 696e 7461 696e 696e 6720 6269 6e61  maintaining bina
+00001310: 7279 2064 6973 7472 6962 7574 696f 6e73  ry distributions
+00001320: 206f 6e20 7069 7020 6973 2074 6f6f 2074   on pip is too t
+00001330: 696d 652d 636f 6e73 756d 696e 672c 2073  ime-consuming, s
+00001340: 6f20 6070 6970 6020 7769 6c6c 2074 7279  o `pip` will try
+00001350: 2074 6f0a 636f 6d70 696c 6520 7468 6520   to.compile the 
+00001360: 736f 7572 6365 2063 6f64 6520 666f 7220  source code for 
+00001370: 796f 752c 2069 6e20 7768 6963 6820 6361  you, in which ca
+00001380: 7365 2079 6f75 2077 696c 6c20 6e65 6564  se you will need
+00001390: 2074 6f20 6861 7665 2046 4654 5720 616e   to have FFTW an
+000013a0: 6420 6120 636f 6d70 696c 6572 2069 6e73  d a compiler ins
+000013b0: 7461 6c6c 6564 2e0a 556e 666f 7274 756e  talled..Unfortun
+000013c0: 6174 656c 792c 2060 7069 7060 2068 6173  ately, `pip` has
+000013d0: 206e 6f20 676f 6f64 2077 6179 206f 6620   no good way of 
+000013e0: 6861 6e64 6c69 6e67 2074 6865 7365 2064  handling these d
+000013f0: 6570 656e 6465 6e63 6965 732e 2020 5365  ependencies.  Se
+00001400: 6520 6265 6c6f 7720 666f 7220 656e 7669  e below for envi
+00001410: 726f 6e6d 656e 740a 7661 7269 6162 6c65  ronment.variable
+00001420: 7320 796f 7520 6d61 7920 6e65 6564 2074  s you may need t
+00001430: 6f20 7365 7420 746f 2067 6574 2063 6f6d  o set to get com
+00001440: 7069 6c61 7469 6f6e 2077 6f72 6b69 6e67  pilation working
+00001450: 2070 726f 7065 726c 792e 0a0a 0a23 2320   properly....## 
+00001460: 4d61 6e75 616c 2069 6e73 7461 6c6c 6174  Manual installat
+00001470: 696f 6e0a 0a4d 616e 7561 6c20 696e 7374  ion..Manual inst
+00001480: 616c 6c61 7469 6f6e 206f 6620 7468 6973  allation of this
+00001490: 2070 6163 6b61 6765 2069 7320 736c 6967   package is slig
+000014a0: 6874 6c79 206d 6f72 6520 6465 6c69 6361  htly more delica
+000014b0: 7465 2e20 2054 6865 0a5b 4646 5457 2070  te.  The.[FFTW p
+000014c0: 6163 6b61 6765 5d28 6874 7470 3a2f 2f77  ackage](http://w
+000014d0: 7777 2e66 6674 772e 6f72 672f 2920 6d75  ww.fftw.org/) mu
+000014e0: 7374 2062 6520 696e 7374 616c 6c65 6420  st be installed 
+000014f0: 6669 7273 742e 2020 5468 6973 2069 7320  first.  This is 
+00001500: 7573 7561 6c6c 790a 7665 7279 2073 696d  usually.very sim
+00001510: 706c 652e 2020 4275 7420 7468 6520 7265  ple.  But the re
+00001520: 7375 6c74 696e 6720 6865 6164 6572 2061  sulting header a
+00001530: 6e64 206c 6962 7261 7279 206d 7573 7420  nd library must 
+00001540: 6265 2066 6f75 6e64 2062 7920 7468 650a  be found by the.
+00001550: 636f 6d70 696c 6174 696f 6e20 7374 6570  compilation step
+00001560: 2066 6f72 2074 6869 7320 7061 636b 6167   for this packag
+00001570: 652e 2020 596f 7520 6361 6e20 6669 7273  e.  You can firs
+00001580: 7420 7369 6d70 6c79 2074 7279 2074 6f20  t simply try to 
+00001590: 7275 6e0a 0a60 6060 6261 7368 0a70 7974  run..```bash.pyt
+000015a0: 686f 6e20 7365 7475 702e 7079 2069 6e73  hon setup.py ins
+000015b0: 7461 6c6c 0a60 6060 0a0a 6672 6f6d 2074  tall.```..from t
+000015c0: 6865 2074 6f70 2064 6972 6563 746f 7279  he top directory
+000015d0: 206f 6620 7468 6520 6073 7069 6e73 6661   of the `spinsfa
+000015e0: 7374 6020 636f 6465 2e0a 0a49 6620 7468  st` code...If th
+000015f0: 6973 2064 6f65 736e 2774 2077 6f72 6b2c  is doesn't work,
+00001600: 2079 6f75 2063 616e 2072 6561 6420 7468   you can read th
+00001610: 6520 6572 726f 7220 6d65 7373 6167 652c  e error message,
+00001620: 2062 7574 2074 6865 206d 6f73 7420 6c69   but the most li
+00001630: 6b65 6c79 0a70 726f 626c 656d 2069 7320  kely.problem is 
+00001640: 7468 6174 2074 6865 2063 6f6d 7069 6c65  that the compile
+00001650: 7220 6361 6e6e 6f74 2066 696e 6420 7468  r cannot find th
+00001660: 6520 6066 6674 7760 2068 6561 6465 722c  e `fftw` header,
+00001670: 206f 7220 7468 6520 6c69 6e6b 6572 0a63   or the linker.c
+00001680: 616e 6e6f 7420 6669 6e64 2074 6865 2060  annot find the `
+00001690: 6666 7477 6020 6c69 6272 6172 792e 2020  fftw` library.  
+000016a0: 546f 2073 6f6c 7665 2074 6865 7365 2070  To solve these p
+000016b0: 726f 626c 656d 732c 2079 6f75 2077 696c  roblems, you wil
+000016c0: 6c20 6e65 6564 2074 6f20 7275 6e0a 736f  l need to run.so
+000016d0: 6d65 7468 696e 6720 6d6f 7265 206c 696b  mething more lik
+000016e0: 6520 7468 6973 3a0a 0a60 6060 6261 7368  e this:..```bash
+000016f0: 0a65 7870 6f72 7420 4c49 4252 4152 595f  .export LIBRARY_
+00001700: 5041 5448 3d2f 7061 7468 2f74 6f2f 6666  PATH=/path/to/ff
+00001710: 7477 2f6c 6962 0a65 7870 6f72 7420 435f  tw/lib.export C_
+00001720: 494e 434c 5544 455f 5041 5448 3d2f 7061  INCLUDE_PATH=/pa
+00001730: 7468 2f74 6f2f 6666 7477 2f69 6e63 6c75  th/to/fftw/inclu
+00001740: 6465 0a70 7974 686f 6e20 7365 7475 702e  de.python setup.
+00001750: 7079 2069 6e73 7461 6c6c 0a60 6060 0a0a  py install.```..
+00001760: 416c 7465 726e 6174 6976 656c 792c 2079  Alternatively, y
+00001770: 6f75 2063 6f75 6c64 2074 7279 2074 6f20  ou could try to 
+00001780: 616c 7465 7220 6073 6574 7570 2e70 7960  alter `setup.py`
+00001790: 2074 6f20 706f 696e 7420 746f 2074 6865   to point to the
+000017a0: 2072 6967 6874 0a70 6174 6873 2e0a 0a0a   right.paths....
+000017b0: 2320 4f72 6967 696e 616c 2069 6e73 7461  # Original insta
+000017c0: 6c6c 6174 696f 6e20 696e 7374 7275 6374  llation instruct
+000017d0: 696f 6e73 0a0a 5468 6f75 6768 2074 6865  ions..Though the
+000017e0: 7365 2061 7265 206e 6f74 206e 6563 6573  se are not neces
+000017f0: 7361 7279 2066 6f72 2069 6e73 7461 6c6c  sary for install
+00001800: 696e 6720 7468 6520 7079 7468 6f6e 206d  ing the python m
+00001810: 6f64 756c 652c 2074 6865 2066 6f6c 6c6f  odule, the follo
+00001820: 7769 6e67 0a61 7265 2074 6865 2069 6e73  wing.are the ins
+00001830: 7472 7563 7469 6f6e 7320 696e 2074 6865  tructions in the
+00001840: 206f 7269 6769 6e61 6c20 736f 7572 6365   original source
+00001850: 2063 6f64 6520 666f 7220 6275 696c 6469   code for buildi
+00001860: 6e67 2074 6865 2043 2063 6f64 652e 0a0a  ng the C code...
+00001870: 4765 7420 7468 6520 6c61 7465 7374 2076  Get the latest v
+00001880: 6572 7369 6f6e 2061 743a 0a0a 2020 2020  ersion at:..    
+00001890: 6874 7470 3a2f 2f77 7777 2e70 6879 7369  http://www.physi
+000018a0: 6373 2e6d 6961 6d69 2e65 6475 2f7e 6875  cs.miami.edu/~hu
+000018b0: 6666 656e 6265 2f72 6573 6561 7263 682f  ffenbe/research/
+000018c0: 7370 696e 7366 6173 742f 0a0a 2323 2043  spinsfast/..## C
+000018d0: 6f6d 7069 6c61 7469 6f6e 2069 6e73 7472  ompilation instr
+000018e0: 7563 7469 6f6e 730a 0a20 2031 2e20 4564  uctions..  1. Ed
+000018f0: 6974 2074 6865 2066 696c 6520 286f 7220  it the file (or 
+00001900: 6d61 6b65 2061 206e 6577 2066 696c 6529  make a new file)
+00001910: 2063 616c 6c65 6420 6275 696c 642f 636f   called build/co
+00001920: 6e66 6967 2e6d 6b20 736f 2074 6861 7420  nfig.mk so that 
+00001930: 7468 6520 7072 6f70 6572 206c 6f63 6174  the proper locat
+00001940: 696f 6e73 2066 6f72 2068 6561 6465 7220  ions for header 
+00001950: 616e 6420 6c69 6272 6172 7920 6669 6c65  and library file
+00001960: 7320 6172 6520 696e 636c 7564 6564 2e0a  s are included..
+00001970: 0a20 2032 2e20 5365 7420 7468 6520 656e  .  2. Set the en
+00001980: 7669 726f 6e6d 656e 7420 7661 7269 6162  vironment variab
+00001990: 6c65 2022 6275 696c 6422 2073 6f20 7468  le "build" so th
+000019a0: 6174 2069 7420 706f 696e 7473 2074 6f20  at it points to 
+000019b0: 7468 6174 2066 696c 652e 2049 2e65 2e2c  that file. I.e.,
+000019c0: 2069 6e20 6261 7368 2c20 7361 790a 0a20   in bash, say.. 
+000019d0: 2020 2020 2020 2065 7870 6f72 7420 6275         export bu
+000019e0: 696c 643d 6275 696c 642f 636f 6e66 6967  ild=build/config
+000019f0: 2e6d 6b20 0a0a 2020 332e 2042 7569 6c64  .mk ..  3. Build
+00001a00: 2074 6865 206c 6962 7261 7279 2061 6e64   the library and
+00001a10: 2065 7861 6d70 6c65 2063 6f64 6573 2077   example codes w
+00001a20: 6974 6820 0a0a 2020 2020 2020 2020 6d61  ith ..        ma
+00001a30: 6b65 0a0a 2323 2028 4f70 7469 6f6e 616c  ke..## (Optional
+00001a40: 2920 4368 6563 6b69 6e67 2074 6865 2063  ) Checking the c
+00001a50: 6f6d 7069 6c61 7469 6f6e 0a0a 5275 6e20  ompilation..Run 
+00001a60: 7468 6520 6578 616d 706c 6520 636f 6465  the example code
+00001a70: 2066 6f6c 6c6f 7769 6e67 2074 6865 2069   following the i
+00001a80: 6e73 7472 7563 7469 6f6e 7320 6174 200a  nstructions at .
+00001a90: 0a20 2020 2068 7474 703a 2f2f 7777 772e  .    http://www.
+00001aa0: 7068 7973 6963 732e 6d69 616d 692e 6564  physics.miami.ed
+00001ab0: 752f 7e68 7566 6665 6e62 652f 7265 7365  u/~huffenbe/rese
+00001ac0: 6172 6368 2f73 7069 6e73 6661 7374 2f0a  arch/spinsfast/.
```

### Comparing `spinsfast-2022.4.1/code/alm.c` & `spinsfast-2022.4.2/code/alm.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.1/code/dump_cimage.c` & `spinsfast-2022.4.2/code/dump_cimage.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.1/code/healpix_convert.c` & `spinsfast-2022.4.2/code/healpix_convert.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.1/code/module.mk` & `spinsfast-2022.4.2/code/module.mk`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.1/code/spinsfast_backward_Gmm.c` & `spinsfast-2022.4.2/code/spinsfast_backward_Gmm.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.1/code/spinsfast_backward_Gmm_alm2iqu.c` & `spinsfast-2022.4.2/code/spinsfast_backward_Gmm_alm2iqu.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.1/code/spinsfast_backward_transform.c` & `spinsfast-2022.4.2/code/spinsfast_backward_transform.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.1/code/spinsfast_forward_Imm.c` & `spinsfast-2022.4.2/code/spinsfast_forward_Imm.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.1/code/spinsfast_forward_Jmm.c` & `spinsfast-2022.4.2/code/spinsfast_forward_Jmm.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.1/code/spinsfast_forward_transform.c` & `spinsfast-2022.4.2/code/spinsfast_forward_transform.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.1/code/spinsfast_forward_transform_eo.c` & `spinsfast-2022.4.2/code/spinsfast_forward_transform_eo.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.1/code/spinsfast_forward_transform_from_Imm.c` & `spinsfast-2022.4.2/code/spinsfast_forward_transform_from_Imm.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.1/code/spinsfast_forward_transform_iqu2alm.c` & `spinsfast-2022.4.2/code/spinsfast_forward_transform_iqu2alm.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.1/code/wigner_d_halfpi_Risbo.c` & `spinsfast-2022.4.2/code/wigner_d_halfpi_Risbo.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.1/code/wigner_d_halfpi_TN.c` & `spinsfast-2022.4.2/code/wigner_d_halfpi_TN.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.1/code/wigner_d_halfpi_methods.c` & `spinsfast-2022.4.2/code/wigner_d_halfpi_methods.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.1/example/example_iqu.c` & `spinsfast-2022.4.2/example/example_iqu.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.1/example/example_multispin.c` & `spinsfast-2022.4.2/example/example_multispin.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.1/example/example_spin.c` & `spinsfast-2022.4.2/example/example_spin.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.1/example/example_spin.py` & `spinsfast-2022.4.2/example/example_spin.py`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.1/example/spinsfast.ipynb` & `spinsfast-2022.4.2/example/spinsfast.ipynb`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.1/include/alm.h` & `spinsfast-2022.4.2/include/alm.h`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.1/include/fftw3.h` & `spinsfast-2022.4.2/include/fftw3.h`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.1/include/healpix_convert.h` & `spinsfast-2022.4.2/include/healpix_convert.h`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.1/include/spinsfast_backward.h` & `spinsfast-2022.4.2/include/spinsfast_backward.h`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.1/include/spinsfast_forward.h` & `spinsfast-2022.4.2/include/spinsfast_forward.h`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.1/include/wigner_d_halfpi.h` & `spinsfast-2022.4.2/include/wigner_d_halfpi.h`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.1/include/wigner_d_halfpi_Risbo.h` & `spinsfast-2022.4.2/include/wigner_d_halfpi_Risbo.h`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.1/include/wigner_d_halfpi_TN.h` & `spinsfast-2022.4.2/include/wigner_d_halfpi_TN.h`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.1/include/wigner_d_halfpi_methods.h` & `spinsfast-2022.4.2/include/wigner_d_halfpi_methods.h`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.1/pyproject.toml` & `spinsfast-2022.4.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 [tool.poetry]
 name = "spinsfast"
-version = "2022.4.1"
+version = "2022.4.2"
 description = "Fast and exact spin-s spherical-harmonic transforms"
 readme = "README.md"
 license = "GPL-3.0-only"
 authors = ["Michael Boyle <mob22@cornell.edu>"]
 homepage = "https://github.com/moble/spinsfast"
 
 [tool.cibuildwheel]
-skip = "cp36-* cp37-* pp37-* pp38-*i686 *musl* pp38-macos* *310-*i686 *-win*"
-before-build = "python -m pip install --no-cache-dir --force-reinstall oldest-supported-numpy"
+#skip = "cp36-* cp37-* pp37-* pp38-*i686 pp38-macos* pp39-* *musl* *-win*"
+skip = "*p36-* *p37-* pp38-*i686 pp39-* *musl* *-win* cp310-manylinux_i686 cp311-manylinux_i686"
+# before-build = "python -m pip install --no-cache-dir --force-reinstall oldest-supported-numpy"
 
 [tool.cibuildwheel.environment]
 # this makes sure that we build only on platforms that have a corresponding numpy wheel
 PIP_ONLY_BINARY = ":all:"
 
 [tool.cibuildwheel.macos]
+# Docs say not to use homebrew: https://cibuildwheel.readthedocs.io/en/stable/faq/#missing-dependencies
+# If there are problems on macos arm or something, this is probably why
 before-all = "brew install fftw"
 before-test = "python -m pip install oldest-supported-numpy"
 test-command = "python -c 'import spinsfast'"
 
 [tool.cibuildwheel.linux]
 before-all = "yum install -y fftw fftw-devel"
 before-test = "python -m pip install oldest-supported-numpy"
```

### Comparing `spinsfast-2022.4.1/python/__init__.py` & `spinsfast-2022.4.2/python/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 """
 
 from __future__ import absolute_import
 
 # NOTE: Don't change the following line; it is modified automatically in the
 # github actions build step, based on the version given in pyproject.toml
-__version__ = "2022.4.1"
+__version__ = "2022.4.2"
 
 # explicitly import functions with underscores (which will be wrapped)
 from .cextension import (
     N_lm, _ind_lm, _lm_ind,
     _salm2map, _multi_salm2map, _map2salm, _multi_map2salm,
     _f_extend_MW, _f_extend_old, _Imm, _quadrature_weights
 )
```

### Comparing `spinsfast-2022.4.1/python/build_macosx_wheels.sh` & `spinsfast-2022.4.2/python/build_macosx_wheels.sh`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.1/python/build_manylinux_wheels.sh` & `spinsfast-2022.4.2/python/build_manylinux_wheels.sh`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.1/python/cextension.c` & `spinsfast-2022.4.2/python/cextension.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.1/setup.py` & `spinsfast-2022.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os.path import isdir, join, dirname, realpath
 from setuptools import setup, Extension
 from distutils.sysconfig import get_python_lib
 
 
 # NOTE: Don't change the following line; it is modified automatically in the
 # github actions build step, based on the version given in pyproject.toml
-version = "2022.4.1"
+version = "2022.4.2"
 
 try:
     import numpy
     numpy_inc = numpy.get_include()
 except:
     numpy_inc = os.path.join(get_python_lib(plat_specific=1), 'numpy', 'core', 'include')
```

### Comparing `spinsfast-2022.4.1/spinsfast.egg-info/PKG-INFO` & `spinsfast-2022.4.2/spinsfast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: spinsfast
-Version: 2022.4.1
+Version: 2022.4.2
 Summary: Fast and exact spin-s spherical-harmonic transforms
 Home-page: https://github.com/moble/spinsfast
 Maintainer: Mike Boyle
 Maintainer-email: mob22@cornell.edu
 License: UNKNOWN
 Description: This module is a lightly modified version of the code originally written by Huffenberger and
         Wandelt.  It enables the user to transform between modes of a spin-weighted spherical-harmonic
```

### Comparing `spinsfast-2022.4.1/spinsfast.egg-info/SOURCES.txt` & `spinsfast-2022.4.2/spinsfast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

