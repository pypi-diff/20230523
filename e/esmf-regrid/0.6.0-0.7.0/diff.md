# Comparing `tmp/esmf_regrid-0.6.0.tar.gz` & `tmp/esmf_regrid-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esmf_regrid-0.6.0.tar", last modified: Fri Mar 31 13:09:01 2023, max compression
+gzip compressed data, was "esmf_regrid-0.7.0.tar", last modified: Tue May 23 12:39:39 2023, max compression
```

## Comparing `esmf_regrid-0.6.0.tar` & `esmf_regrid-0.7.0.tar`

### file list

```diff
@@ -1,70 +1,89 @@
-drwxr-xr-x   0 sworsley (11933) users     (1000)        0 2023-03-31 13:09:01.769360 esmf_regrid-0.6.0/
--rw-r--r--   0 sworsley (11933) users     (1000)     1533 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/LICENSE
--rw-r--r--   0 sworsley (11933) users     (1000)     4510 2023-03-31 13:09:01.770354 esmf_regrid-0.6.0/PKG-INFO
--rw-r--r--   0 sworsley (11933) users     (1000)     3463 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/README.md
-drwxr-xr-x   0 sworsley (11933) users     (1000)        0 2023-03-31 13:09:01.411336 esmf_regrid-0.6.0/esmf_regrid/
--rw-r--r--   0 sworsley (11933) users     (1000)      252 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/__init__.py
--rw-r--r--   0 sworsley (11933) users     (1000)    19216 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/_esmf_sdo.py
--rw-r--r--   0 sworsley (11933) users     (1000)     8682 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/esmf_regridder.py
-drwxr-xr-x   0 sworsley (11933) users     (1000)        0 2023-03-31 13:09:01.459366 esmf_regrid-0.6.0/esmf_regrid/experimental/
--rw-r--r--   0 sworsley (11933) users     (1000)       84 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/experimental/__init__.py
--rw-r--r--   0 sworsley (11933) users     (1000)     8630 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/experimental/io.py
--rw-r--r--   0 sworsley (11933) users     (1000)     5810 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/experimental/unstructured_regrid.py
--rw-r--r--   0 sworsley (11933) users     (1000)    34371 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/experimental/unstructured_scheme.py
--rw-r--r--   0 sworsley (11933) users     (1000)    22748 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/schemes.py
-drwxr-xr-x   0 sworsley (11933) users     (1000)        0 2023-03-31 13:09:01.478410 esmf_regrid-0.6.0/esmf_regrid/tests/
--rw-r--r--   0 sworsley (11933) users     (1000)     1722 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/tests/__init__.py
-drwxr-xr-x   0 sworsley (11933) users     (1000)        0 2023-03-31 13:09:01.482388 esmf_regrid-0.6.0/esmf_regrid/tests/integration/
--rw-r--r--   0 sworsley (11933) users     (1000)       41 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/tests/integration/__init__.py
-drwxr-xr-x   0 sworsley (11933) users     (1000)        0 2023-03-31 13:09:01.488361 esmf_regrid-0.6.0/esmf_regrid/tests/integration/esmf_regridder/
--rw-r--r--   0 sworsley (11933) users     (1000)       63 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/tests/integration/esmf_regridder/__init__.py
--rw-r--r--   0 sworsley (11933) users     (1000)     2332 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/tests/integration/esmf_regridder/test_Regridder.py
-drwxr-xr-x   0 sworsley (11933) users     (1000)        0 2023-03-31 13:09:01.492337 esmf_regrid-0.6.0/esmf_regrid/tests/integration/experimental/
--rw-r--r--   0 sworsley (11933) users     (1000)       61 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/tests/integration/experimental/__init__.py
-drwxr-xr-x   0 sworsley (11933) users     (1000)        0 2023-03-31 13:09:01.515376 esmf_regrid-0.6.0/esmf_regrid/tests/integration/experimental/unstructured_scheme/
--rw-r--r--   0 sworsley (11933) users     (1000)       81 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/tests/integration/experimental/unstructured_scheme/__init__.py
--rw-r--r--   0 sworsley (11933) users     (1000)     1606 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/tests/integration/experimental/unstructured_scheme/test_regrid_unstructured_to_rectilinear.py
-drwxr-xr-x   0 sworsley (11933) users     (1000)        0 2023-03-31 13:09:01.518380 esmf_regrid-0.6.0/esmf_regrid/tests/unit/
--rw-r--r--   0 sworsley (11933) users     (1000)       35 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/tests/unit/__init__.py
-drwxr-xr-x   0 sworsley (11933) users     (1000)        0 2023-03-31 13:09:01.550337 esmf_regrid-0.6.0/esmf_regrid/tests/unit/_esmf_sdo/
--rw-r--r--   0 sworsley (11933) users     (1000)       51 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/tests/unit/_esmf_sdo/__init__.py
--rw-r--r--   0 sworsley (11933) users     (1000)     2707 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/tests/unit/_esmf_sdo/test_GridInfo.py
--rw-r--r--   0 sworsley (11933) users     (1000)     4028 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/tests/unit/_esmf_sdo/test_RefinedGridInfo.py
-drwxr-xr-x   0 sworsley (11933) users     (1000)        0 2023-03-31 13:09:01.573366 esmf_regrid-0.6.0/esmf_regrid/tests/unit/esmf_regridder/
--rw-r--r--   0 sworsley (11933) users     (1000)       56 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/tests/unit/esmf_regridder/__init__.py
--rw-r--r--   0 sworsley (11933) users     (1000)     8023 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/tests/unit/esmf_regridder/test_Regridder.py
-drwxr-xr-x   0 sworsley (11933) users     (1000)        0 2023-03-31 13:09:01.576353 esmf_regrid-0.6.0/esmf_regrid/tests/unit/experimental/
--rw-r--r--   0 sworsley (11933) users     (1000)       54 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/tests/unit/experimental/__init__.py
-drwxr-xr-x   0 sworsley (11933) users     (1000)        0 2023-03-31 13:09:01.586353 esmf_regrid-0.6.0/esmf_regrid/tests/unit/experimental/io/
--rw-r--r--   0 sworsley (11933) users     (1000)       57 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/tests/unit/experimental/io/__init__.py
--rw-r--r--   0 sworsley (11933) users     (1000)    14766 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/tests/unit/experimental/io/test_round_tripping.py
--rw-r--r--   0 sworsley (11933) users     (1000)      398 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/tests/unit/experimental/io/test_save_regridder.py
-drwxr-xr-x   0 sworsley (11933) users     (1000)        0 2023-03-31 13:09:01.611380 esmf_regrid-0.6.0/esmf_regrid/tests/unit/experimental/unstructured_regrid/
--rw-r--r--   0 sworsley (11933) users     (1000)       74 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/tests/unit/experimental/unstructured_regrid/__init__.py
--rw-r--r--   0 sworsley (11933) users     (1000)     6521 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/tests/unit/experimental/unstructured_regrid/test_MeshInfo.py
-drwxr-xr-x   0 sworsley (11933) users     (1000)        0 2023-03-31 13:09:01.702353 esmf_regrid-0.6.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/
--rw-r--r--   0 sworsley (11933) users     (1000)       74 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/__init__.py
--rw-r--r--   0 sworsley (11933) users     (1000)    16375 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test_GridToMeshESMFRegridder.py
--rw-r--r--   0 sworsley (11933) users     (1000)    15731 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test_MeshToGridESMFRegridder.py
--rw-r--r--   0 sworsley (11933) users     (1000)     3037 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test__create_cube.py
--rw-r--r--   0 sworsley (11933) users     (1000)     3412 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test__cube_to_GridInfo.py
--rw-r--r--   0 sworsley (11933) users     (1000)    10037 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test__mesh_to_MeshInfo.py
--rw-r--r--   0 sworsley (11933) users     (1000)     2478 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test__regrid_unstructured_to_rectilinear__prepare.py
--rw-r--r--   0 sworsley (11933) users     (1000)     9657 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test_regrid_rectilinear_to_unstructured.py
--rw-r--r--   0 sworsley (11933) users     (1000)     7408 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test_regrid_unstructured_to_rectilinear.py
-drwxr-xr-x   0 sworsley (11933) users     (1000)        0 2023-03-31 13:09:01.766351 esmf_regrid-0.6.0/esmf_regrid/tests/unit/schemes/
--rw-r--r--   0 sworsley (11933) users     (1000)       44 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/tests/unit/schemes/__init__.py
--rw-r--r--   0 sworsley (11933) users     (1000)     2042 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/tests/unit/schemes/test_ESMFAreaWeighted.py
--rw-r--r--   0 sworsley (11933) users     (1000)    10198 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/tests/unit/schemes/test_ESMFAreaWeightedRegridder.py
--rw-r--r--   0 sworsley (11933) users     (1000)     8573 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/tests/unit/schemes/test__cube_to_GridInfo.py
--rw-r--r--   0 sworsley (11933) users     (1000)    15034 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/esmf_regrid/tests/unit/schemes/test_regrid_rectilinear_to_rectilinear.py
-drwxr-xr-x   0 sworsley (11933) users     (1000)        0 2023-03-31 13:09:01.449340 esmf_regrid-0.6.0/esmf_regrid.egg-info/
--rw-r--r--   0 sworsley (11933) users     (1000)     4510 2023-03-31 13:09:00.000000 esmf_regrid-0.6.0/esmf_regrid.egg-info/PKG-INFO
--rw-r--r--   0 sworsley (11933) users     (1000)     2696 2023-03-31 13:09:01.000000 esmf_regrid-0.6.0/esmf_regrid.egg-info/SOURCES.txt
--rw-r--r--   0 sworsley (11933) users     (1000)        1 2023-03-31 13:09:01.000000 esmf_regrid-0.6.0/esmf_regrid.egg-info/dependency_links.txt
--rw-r--r--   0 sworsley (11933) users     (1000)        1 2023-03-31 13:09:01.000000 esmf_regrid-0.6.0/esmf_regrid.egg-info/not-zip-safe
--rw-r--r--   0 sworsley (11933) users     (1000)       74 2023-03-31 13:09:01.000000 esmf_regrid-0.6.0/esmf_regrid.egg-info/requires.txt
--rw-r--r--   0 sworsley (11933) users     (1000)       12 2023-03-31 13:09:01.000000 esmf_regrid-0.6.0/esmf_regrid.egg-info/top_level.txt
--rw-r--r--   0 sworsley (11933) users     (1000)      512 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/pyproject.toml
--rw-r--r--   0 sworsley (11933) users     (1000)     1357 2023-03-31 13:09:01.778336 esmf_regrid-0.6.0/setup.cfg
--rw-r--r--   0 sworsley (11933) users     (1000)      109 2023-03-31 12:55:52.000000 esmf_regrid-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:39:39.107131 esmf_regrid-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7733 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-23 12:39:39.107131 esmf_regrid-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:39:39.099130 esmf_regrid-0.7.0/esmf_regrid/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19216 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/_esmf_sdo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8894 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/esmf_regridder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:39:39.099130 esmf_regrid-0.7.0/esmf_regrid/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8886 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/experimental/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/experimental/unstructured_regrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16244 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/experimental/unstructured_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53639 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/schemes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:39:39.099130 esmf_regrid-0.7.0/esmf_regrid/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:39:39.099130 esmf_regrid-0.7.0/esmf_regrid/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:39:39.099130 esmf_regrid-0.7.0/esmf_regrid/tests/integration/esmf_regridder/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/integration/esmf_regridder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/integration/esmf_regridder/test_Regridder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:39:39.099130 esmf_regrid-0.7.0/esmf_regrid/tests/integration/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/integration/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:39:39.103131 esmf_regrid-0.7.0/esmf_regrid/tests/integration/experimental/unstructured_scheme/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/integration/experimental/unstructured_scheme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/integration/experimental/unstructured_scheme/test_regrid_unstructured_to_rectilinear.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:39:39.095131 esmf_regrid-0.7.0/esmf_regrid/tests/results/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:39:39.095131 esmf_regrid-0.7.0/esmf_regrid/tests/results/unit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:39:39.095131 esmf_regrid-0.7.0/esmf_regrid/tests/results/unit/_esmf_sdo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:39:39.103131 esmf_regrid-0.7.0/esmf_regrid/tests/results/unit/_esmf_sdo/test_GridInfo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/results/unit/_esmf_sdo/test_GridInfo/small_grid.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:39:39.095131 esmf_regrid-0.7.0/esmf_regrid/tests/results/unit/experimental/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:39:39.095131 esmf_regrid-0.7.0/esmf_regrid/tests/results/unit/experimental/unstructured_regrid/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:39:39.103131 esmf_regrid-0.7.0/esmf_regrid/tests/results/unit/experimental/unstructured_regrid/test_MeshInfo/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/results/unit/experimental/unstructured_regrid/test_MeshInfo/small_mesh.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:39:39.103131 esmf_regrid-0.7.0/esmf_regrid/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:39:39.103131 esmf_regrid-0.7.0/esmf_regrid/tests/unit/_esmf_sdo/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/unit/_esmf_sdo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/unit/_esmf_sdo/test_GridInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/unit/_esmf_sdo/test_RefinedGridInfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:39:39.103131 esmf_regrid-0.7.0/esmf_regrid/tests/unit/esmf_regridder/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/unit/esmf_regridder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/unit/esmf_regridder/test_Regridder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:39:39.103131 esmf_regrid-0.7.0/esmf_regrid/tests/unit/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/unit/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:39:39.103131 esmf_regrid-0.7.0/esmf_regrid/tests/unit/experimental/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/unit/experimental/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/unit/experimental/io/test_round_tripping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/unit/experimental/io/test_save_regridder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:39:39.103131 esmf_regrid-0.7.0/esmf_regrid/tests/unit/experimental/unstructured_regrid/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/unit/experimental/unstructured_regrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6521 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/unit/experimental/unstructured_regrid/test_MeshInfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:39:39.103131 esmf_regrid-0.7.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16784 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test_GridToMeshESMFRegridder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16171 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test_MeshToGridESMFRegridder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10026 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test_regrid_rectilinear_to_unstructured.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test_regrid_unstructured_to_rectilinear.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:39:39.103131 esmf_regrid-0.7.0/esmf_regrid/tests/unit/schemes/
+-rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/unit/schemes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/unit/schemes/test_ESMFAreaWeighted.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/unit/schemes/test_ESMFAreaWeightedRegridder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/unit/schemes/test_ESMFBilinear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11626 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/unit/schemes/test_ESMFBilinearRegridder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/unit/schemes/test_ESMFNearest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/unit/schemes/test_ESMFNearestRegridder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/unit/schemes/test__ESMFRegridder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/unit/schemes/test__create_cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/unit/schemes/test__cube_to_GridInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10012 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/unit/schemes/test__mesh_to_MeshInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/unit/schemes/test__regrid_unstructured_to_rectilinear__prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15808 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/esmf_regrid/tests/unit/schemes/test_regrid_rectilinear_to_rectilinear.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:39:39.099130 esmf_regrid-0.7.0/esmf_regrid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-23 12:39:39.000000 esmf_regrid-0.7.0/esmf_regrid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-23 12:39:39.000000 esmf_regrid-0.7.0/esmf_regrid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 12:39:39.000000 esmf_regrid-0.7.0/esmf_regrid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 12:39:38.000000 esmf_regrid-0.7.0/esmf_regrid.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-23 12:39:39.000000 esmf_regrid-0.7.0/esmf_regrid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 12:39:39.000000 esmf_regrid-0.7.0/esmf_regrid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:39:39.103131 esmf_regrid-0.7.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/requirements/core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/requirements/optional-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/requirements/optional-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 12:39:39.107131 esmf_regrid-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-23 12:39:30.000000 esmf_regrid-0.7.0/setup.py
```

### Comparing `esmf_regrid-0.6.0/LICENSE` & `esmf_regrid-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `esmf_regrid-0.6.0/esmf_regrid/_esmf_sdo.py` & `esmf_regrid-0.7.0/esmf_regrid/_esmf_sdo.py`

 * *Files identical despite different names*

### Comparing `esmf_regrid-0.6.0/esmf_regrid/esmf_regridder.py` & `esmf_regrid-0.7.0/esmf_regrid/esmf_regridder.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import esmf_regrid
 from . import esmpy
 from ._esmf_sdo import GridInfo, RefinedGridInfo
 
 __all__ = [
     "GridInfo",
+    "RefinedGridInfo",
     "Regridder",
 ]
 
 
 def _get_regrid_weights_dict(src_field, tgt_field, regrid_method):
     # The value, in array form, that ESMF should treat as an affirmative mask.
     expected_mask = np.array([True])
@@ -72,32 +73,35 @@
             Data supplied to this regridder should be in a :class:`numpy.ndarray`
             whose shape is compatible with ``src``.
         tgt : :class:`~esmf_regrid.experimental.unstructured_regrid.MeshInfo` or :class:`GridInfo`
             Describes the target mesh/grid.
             Data output by this regridder will be a :class:`numpy.ndarray` whose
             shape is compatible with ``tgt``.
         method : str
-            Either "conservative" or "bilinear". Corresponds to the :mod:`esmpy` methods
-            :attr:`~esmpy.api.constants.RegridMethod.CONSERVE` or
-            :attr:`~esmpy.api.constants.RegridMethod.BILINEAR` used to calculate weights.
+            Either "conservative", "bilinear" or "nearest". Corresponds to the :mod:`esmpy` methods
+            :attr:`~esmpy.api.constants.RegridMethod.CONSERVE`,
+            :attr:`~esmpy.api.constants.RegridMethod.BILINEAR` or
+            :attr:`~esmpy.api.constants.RegridMethod.NEAREST_STOD` used to calculate weights.
         precomputed_weights : :class:`scipy.sparse.spmatrix`, optional
             If ``None``, :mod:`esmpy` will be used to
             calculate regridding weights. Otherwise, :mod:`esmpy` will be bypassed
             and ``precomputed_weights`` will be used as the regridding weights.
         """
         self.src = src
         self.tgt = tgt
 
         if method == "conservative":
             esmf_regrid_method = esmpy.RegridMethod.CONSERVE
         elif method == "bilinear":
             esmf_regrid_method = esmpy.RegridMethod.BILINEAR
+        elif method == "nearest":
+            esmf_regrid_method = esmpy.RegridMethod.NEAREST_STOD
         else:
             raise ValueError(
-                f"method must be either 'bilinear' or 'conservative', got '{method}'."
+                f"method must be either 'bilinear', 'conservative' or 'nearest', got '{method}'."
             )
         self.method = method
 
         self.esmf_regrid_version = esmf_regrid.__version__
         if precomputed_weights is None:
             self.esmf_version = esmpy.__version__
             weights_dict = _get_regrid_weights_dict(
```

### Comparing `esmf_regrid-0.6.0/esmf_regrid/experimental/io.py` & `esmf_regrid-0.7.0/esmf_regrid/experimental/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,23 +224,31 @@
     else:
         use_src_mask = False
     if tgt_cube.coords(TARGET_MASK_NAME):
         use_tgt_mask = tgt_cube.coord(TARGET_MASK_NAME).points
     else:
         use_tgt_mask = False
 
+    if scheme is GridToMeshESMFRegridder:
+        resolution_keyword = "src_resolution"
+    elif scheme is MeshToGridESMFRegridder:
+        resolution_keyword = "tgt_resolution"
+    else:
+        raise NotImplementedError
+    kwargs = {resolution_keyword: resolution}
+
     regridder = scheme(
         src_cube,
         tgt_cube,
         mdtol=mdtol,
         method=method,
         precomputed_weights=weight_matrix,
-        resolution=resolution,
         use_src_mask=use_src_mask,
         use_tgt_mask=use_tgt_mask,
+        **kwargs,
     )
 
     esmf_version = weights_cube.attributes[VERSION_ESMF]
     regridder.regridder.esmf_version = esmf_version
     esmf_regrid_version = weights_cube.attributes[VERSION_INITIAL]
     regridder.regridder.esmf_regrid_version = esmf_regrid_version
     return regridder
```

### Comparing `esmf_regrid-0.6.0/esmf_regrid/experimental/unstructured_regrid.py` & `esmf_regrid-0.7.0/esmf_regrid/experimental/unstructured_regrid.py`

 * *Files identical despite different names*

### Comparing `esmf_regrid-0.6.0/esmf_regrid/tests/__init__.py` & `esmf_regrid-0.7.0/esmf_regrid/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `esmf_regrid-0.6.0/esmf_regrid/tests/integration/esmf_regridder/test_Regridder.py` & `esmf_regrid-0.7.0/esmf_regrid/tests/integration/esmf_regridder/test_Regridder.py`

 * *Files identical despite different names*

### Comparing `esmf_regrid-0.6.0/esmf_regrid/tests/integration/experimental/unstructured_scheme/test_regrid_unstructured_to_rectilinear.py` & `esmf_regrid-0.7.0/esmf_regrid/tests/integration/experimental/unstructured_scheme/test_regrid_unstructured_to_rectilinear.py`

 * *Files identical despite different names*

### Comparing `esmf_regrid-0.6.0/esmf_regrid/tests/unit/_esmf_sdo/test_GridInfo.py` & `esmf_regrid-0.7.0/esmf_regrid/tests/unit/_esmf_sdo/test_GridInfo.py`

 * *Files identical despite different names*

### Comparing `esmf_regrid-0.6.0/esmf_regrid/tests/unit/_esmf_sdo/test_RefinedGridInfo.py` & `esmf_regrid-0.7.0/esmf_regrid/tests/unit/_esmf_sdo/test_RefinedGridInfo.py`

 * *Files identical despite different names*

### Comparing `esmf_regrid-0.6.0/esmf_regrid/tests/unit/esmf_regridder/test_Regridder.py` & `esmf_regrid-0.7.0/esmf_regrid/tests/unit/esmf_regridder/test_Regridder.py`

 * *Files identical despite different names*

### Comparing `esmf_regrid-0.6.0/esmf_regrid/tests/unit/experimental/io/test_round_tripping.py` & `esmf_regrid-0.7.0/esmf_regrid/tests/unit/experimental/io/test_round_tripping.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 import pytest
 
 from esmf_regrid.experimental.io import load_regridder, save_regridder
 from esmf_regrid.experimental.unstructured_scheme import (
     GridToMeshESMFRegridder,
     MeshToGridESMFRegridder,
 )
-from esmf_regrid.tests.unit.experimental.unstructured_scheme.test__mesh_to_MeshInfo import (
-    _gridlike_mesh_cube,
-)
 from esmf_regrid.tests.unit.schemes.test__cube_to_GridInfo import (
     _curvilinear_cube,
     _grid_cube,
 )
+from esmf_regrid.tests.unit.schemes.test__mesh_to_MeshInfo import (
+    _gridlike_mesh_cube,
+)
 
 
 def _make_grid_to_mesh_regridder(
     method="conservative",
     resolution=None,
     grid_dims=1,
     circular=True,
@@ -60,15 +60,15 @@
         use_tgt_mask = False
 
     rg = GridToMeshESMFRegridder(
         src,
         tgt,
         method=method,
         mdtol=0.5,
-        resolution=resolution,
+        src_resolution=resolution,
         use_src_mask=use_src_mask,
         use_tgt_mask=use_tgt_mask,
     )
     return rg, src
 
 
 def _make_mesh_to_grid_regridder(
@@ -106,24 +106,25 @@
         use_tgt_mask = False
 
     rg = MeshToGridESMFRegridder(
         src,
         tgt,
         method=method,
         mdtol=0.5,
-        resolution=resolution,
+        tgt_resolution=resolution,
         use_src_mask=use_src_mask,
         use_tgt_mask=use_tgt_mask,
     )
     return rg, src
 
 
-def test_GridToMeshESMFRegridder_round_trip(tmp_path):
+@pytest.mark.parametrize("method", ["conservative", "bilinear", "nearest"])
+def test_GridToMeshESMFRegridder_round_trip(tmp_path, method):
     """Test save/load round tripping for `GridToMeshESMFRegridder`."""
-    original_rg, src = _make_grid_to_mesh_regridder(circular=True)
+    original_rg, src = _make_grid_to_mesh_regridder(method=method, circular=True)
     filename = tmp_path / "regridder.nc"
     save_regridder(original_rg, filename)
     loaded_rg = load_regridder(str(filename))
 
     assert original_rg.location == loaded_rg.location
     assert original_rg.method == loaded_rg.method
     assert original_rg.mdtol == loaded_rg.mdtol
@@ -152,75 +153,36 @@
     # Ensure version data is equal.
     assert original_rg.regridder.esmf_version == loaded_rg.regridder.esmf_version
     assert (
         original_rg.regridder.esmf_regrid_version
         == loaded_rg.regridder.esmf_regrid_version
     )
 
-    # Ensure resolution is equal.
-    assert original_rg.resolution == loaded_rg.resolution
-    original_res_rg, _ = _make_grid_to_mesh_regridder(resolution=8)
-    res_filename = tmp_path / "regridder_res.nc"
-    save_regridder(original_res_rg, res_filename)
-    loaded_res_rg = load_regridder(str(res_filename))
-    assert original_res_rg.resolution == loaded_res_rg.resolution
-    assert (
-        original_res_rg.regridder.src.resolution
-        == loaded_res_rg.regridder.src.resolution
-    )
+    if method == "conservative":
+        # Ensure resolution is equal.
+        assert original_rg.resolution == loaded_rg.resolution
+        original_res_rg, _ = _make_grid_to_mesh_regridder(method=method, resolution=8)
+        res_filename = tmp_path / "regridder_res.nc"
+        save_regridder(original_res_rg, res_filename)
+        loaded_res_rg = load_regridder(str(res_filename))
+        assert original_res_rg.resolution == loaded_res_rg.resolution
+        assert (
+            original_res_rg.regridder.src.resolution
+            == loaded_res_rg.regridder.src.resolution
+        )
 
     # Ensure grid equality for non-circular coords.
-    original_nc_rg, _ = _make_grid_to_mesh_regridder(circular=False)
+    original_nc_rg, _ = _make_grid_to_mesh_regridder(method=method, circular=False)
     nc_filename = tmp_path / "non_circular_regridder.nc"
     save_regridder(original_nc_rg, nc_filename)
     loaded_nc_rg = load_regridder(str(nc_filename))
     assert original_nc_rg.grid_x == loaded_nc_rg.grid_x
     assert original_nc_rg.grid_y == loaded_nc_rg.grid_y
 
 
-def test_GridToMeshESMFRegridder_bilinear_round_trip(tmp_path):
-    """Test save/load round tripping for `GridToMeshESMFRegridder`."""
-    original_rg, src = _make_grid_to_mesh_regridder(method="bilinear")
-    filename = tmp_path / "regridder.nc"
-    save_regridder(original_rg, filename)
-    loaded_rg = load_regridder(str(filename))
-
-    assert original_rg.location == loaded_rg.location
-    assert original_rg.method == loaded_rg.method
-    assert original_rg.mdtol == loaded_rg.mdtol
-    assert original_rg.grid_x == loaded_rg.grid_x
-    assert original_rg.grid_y == loaded_rg.grid_y
-    # TODO: uncomment when iris mesh comparison becomes available.
-    # assert original_rg.mesh == loaded_rg.mesh
-
-    # Compare the weight matrices.
-    original_matrix = original_rg.regridder.weight_matrix
-    loaded_matrix = loaded_rg.regridder.weight_matrix
-    # Ensure the original and loaded weight matrix have identical type.
-    assert type(original_matrix) is type(loaded_matrix)  # noqa E721
-    assert np.array_equal(original_matrix.todense(), loaded_matrix.todense())
-
-    # Demonstrate regridding still gives the same results.
-    src_data = ma.arange(np.product(src.data.shape)).reshape(src.data.shape)
-    src_data[0, 0] = ma.masked
-    src.data = src_data
-    # TODO: make this a cube comparison when mesh comparison becomes available.
-    original_result = original_rg(src).data
-    loaded_result = loaded_rg(src).data
-    assert np.array_equal(original_result, loaded_result)
-    assert np.array_equal(original_result.mask, loaded_result.mask)
-
-    # Ensure version data is equal.
-    assert original_rg.regridder.esmf_version == loaded_rg.regridder.esmf_version
-    assert (
-        original_rg.regridder.esmf_regrid_version
-        == loaded_rg.regridder.esmf_regrid_version
-    )
-
-
 def test_GridToMeshESMFRegridder_curvilinear_round_trip(tmp_path):
     """Test save/load round tripping for `GridToMeshESMFRegridder`."""
     original_rg, src = _make_grid_to_mesh_regridder(grid_dims=2)
     filename = tmp_path / "regridder.nc"
     save_regridder(original_rg, filename)
     loaded_rg = load_regridder(str(filename))
 
@@ -259,17 +221,18 @@
     assert np.array_equal(original_matrix.todense(), loaded_matrix.todense())
 
     # Ensure the masks are preserved
     assert np.array_equal(loaded_rg.src_mask, original_rg.src_mask)
     assert np.array_equal(loaded_rg.tgt_mask, original_rg.tgt_mask)
 
 
-def test_MeshToGridESMFRegridder_round_trip(tmp_path):
+@pytest.mark.parametrize("method", ["conservative", "bilinear", "nearest"])
+def test_MeshToGridESMFRegridder_round_trip(tmp_path, method):
     """Test save/load round tripping for `MeshToGridESMFRegridder`."""
-    original_rg, src = _make_mesh_to_grid_regridder(circular=True)
+    original_rg, src = _make_mesh_to_grid_regridder(method=method, circular=True)
     filename = tmp_path / "regridder.nc"
     save_regridder(original_rg, filename)
     loaded_rg = load_regridder(str(filename))
 
     assert original_rg.location == loaded_rg.location
     assert original_rg.method == loaded_rg.method
     assert original_rg.mdtol == loaded_rg.mdtol
@@ -297,74 +260,36 @@
     # Ensure version data is equal.
     assert original_rg.regridder.esmf_version == loaded_rg.regridder.esmf_version
     assert (
         original_rg.regridder.esmf_regrid_version
         == loaded_rg.regridder.esmf_regrid_version
     )
 
-    # Ensure resolution is equal.
-    assert original_rg.resolution == loaded_rg.resolution
-    original_res_rg, _ = _make_mesh_to_grid_regridder(resolution=8)
-    res_filename = tmp_path / "regridder_res.nc"
-    save_regridder(original_res_rg, res_filename)
-    loaded_res_rg = load_regridder(str(res_filename))
-    assert original_res_rg.resolution == loaded_res_rg.resolution
-    assert (
-        original_res_rg.regridder.tgt.resolution
-        == loaded_res_rg.regridder.tgt.resolution
-    )
+    if method == "conservative":
+        # Ensure resolution is equal.
+        assert original_rg.resolution == loaded_rg.resolution
+        original_res_rg, _ = _make_mesh_to_grid_regridder(method=method, resolution=8)
+        res_filename = tmp_path / "regridder_res.nc"
+        save_regridder(original_res_rg, res_filename)
+        loaded_res_rg = load_regridder(str(res_filename))
+        assert original_res_rg.resolution == loaded_res_rg.resolution
+        assert (
+            original_res_rg.regridder.tgt.resolution
+            == loaded_res_rg.regridder.tgt.resolution
+        )
 
     # Ensure grid equality for non-circular coords.
-    original_nc_rg, _ = _make_grid_to_mesh_regridder(circular=False)
+    original_nc_rg, _ = _make_grid_to_mesh_regridder(method=method, circular=False)
     nc_filename = tmp_path / "non_circular_regridder.nc"
     save_regridder(original_nc_rg, nc_filename)
     loaded_nc_rg = load_regridder(str(nc_filename))
     assert original_nc_rg.grid_x == loaded_nc_rg.grid_x
     assert original_nc_rg.grid_y == loaded_nc_rg.grid_y
 
 
-def test_MeshToGridESMFRegridder_bilinear_round_trip(tmp_path):
-    """Test save/load round tripping for `MeshToGridESMFRegridder`."""
-    original_rg, src = _make_mesh_to_grid_regridder(method="bilinear")
-    filename = tmp_path / "regridder.nc"
-    save_regridder(original_rg, filename)
-    loaded_rg = load_regridder(str(filename))
-
-    assert original_rg.location == loaded_rg.location
-    assert original_rg.method == loaded_rg.method
-    assert original_rg.mdtol == loaded_rg.mdtol
-    assert original_rg.grid_x == loaded_rg.grid_x
-    assert original_rg.grid_y == loaded_rg.grid_y
-    # TODO: uncomment when iris mesh comparison becomes available.
-    # assert original_rg.mesh == loaded_rg.mesh
-
-    # Compare the weight matrices.
-    original_matrix = original_rg.regridder.weight_matrix
-    loaded_matrix = loaded_rg.regridder.weight_matrix
-    # Ensure the original and loaded weight matrix have identical type.
-    assert type(original_matrix) is type(loaded_matrix)  # noqa E721
-    assert np.array_equal(original_matrix.todense(), loaded_matrix.todense())
-
-    # Demonstrate regridding still gives the same results.
-    src_data = ma.arange(np.product(src.data.shape)).reshape(src.data.shape)
-    src_data[0] = ma.masked
-    src.data = src_data
-    original_result = original_rg(src).data
-    loaded_result = loaded_rg(src).data
-    assert np.array_equal(original_result, loaded_result)
-    assert np.array_equal(original_result.mask, loaded_result.mask)
-
-    # Ensure version data is equal.
-    assert original_rg.regridder.esmf_version == loaded_rg.regridder.esmf_version
-    assert (
-        original_rg.regridder.esmf_regrid_version
-        == loaded_rg.regridder.esmf_regrid_version
-    )
-
-
 def test_MeshToGridESMFRegridder_curvilinear_round_trip(tmp_path):
     """Test save/load round tripping for `MeshToGridESMFRegridder`."""
     original_rg, src = _make_mesh_to_grid_regridder(grid_dims=2)
     filename = tmp_path / "regridder.nc"
     save_regridder(original_rg, filename)
     loaded_rg = load_regridder(str(filename))
```

### Comparing `esmf_regrid-0.6.0/esmf_regrid/tests/unit/experimental/unstructured_regrid/test_MeshInfo.py` & `esmf_regrid-0.7.0/esmf_regrid/tests/unit/experimental/unstructured_regrid/test_MeshInfo.py`

 * *Files identical despite different names*

### Comparing `esmf_regrid-0.6.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test_GridToMeshESMFRegridder.py` & `esmf_regrid-0.7.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test_GridToMeshESMFRegridder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-"""Unit tests for :func:`esmf_regrid.experimental.unstructured_scheme.GridToMeshESMFRegridder`."""
+"""Unit tests for :class:`esmf_regrid.experimental.unstructured_scheme.GridToMeshESMFRegridder`."""
 
 import dask.array as da
 from iris.coords import AuxCoord, DimCoord
 from iris.cube import Cube
 import numpy as np
 from numpy import ma
 import pytest
 
 from esmf_regrid.experimental.unstructured_scheme import (
     GridToMeshESMFRegridder,
 )
-from esmf_regrid.tests.unit.experimental.unstructured_scheme.test__mesh_to_MeshInfo import (
+from esmf_regrid.tests.unit.schemes.test__cube_to_GridInfo import (
+    _curvilinear_cube,
+    _grid_cube,
+)
+from esmf_regrid.tests.unit.schemes.test__mesh_to_MeshInfo import (
     _gridlike_mesh,
     _gridlike_mesh_cube,
 )
-from esmf_regrid.tests.unit.experimental.unstructured_scheme.test__regrid_unstructured_to_rectilinear__prepare import (
+from esmf_regrid.tests.unit.schemes.test__regrid_unstructured_to_rectilinear__prepare import (
     _flat_mesh_cube,
 )
-from esmf_regrid.tests.unit.schemes.test__cube_to_GridInfo import (
-    _curvilinear_cube,
-    _grid_cube,
-)
 
 
 def _add_metadata(cube):
     result = cube.copy()
     result.units = "K"
     result.attributes = {"a": 1}
     result.standard_name = "air_temperature"
@@ -33,15 +33,15 @@
     result.add_aux_coord(scalar_height)
     result.add_aux_coord(scalar_time)
     return result
 
 
 def test_flat_cubes():
     """
-    Basic test for :func:`esmf_regrid.experimental.unstructured_scheme.GridToMeshESMFRegridder`.
+    Basic test for :class:`esmf_regrid.experimental.unstructured_scheme.GridToMeshESMFRegridder`.
 
     Tests with flat cubes as input (a 2D grid cube and a 1D mesh cube).
     """
     tgt = _flat_mesh_cube()
 
     n_lons = 6
     n_lats = 5
@@ -70,35 +70,36 @@
     # Check metadata and scalar coords.
     expected_cube.data = result.data
     assert expected_cube == result
     expected_cube.data = result_transposed.data
     assert expected_cube == result_transposed
 
 
-def test_bilinear():
+@pytest.mark.parametrize("method", ["bilinear", "nearest"])
+def test_node_friendly_methods(method):
     """
-    Basic test for :func:`esmf_regrid.experimental.unstructured_scheme.GridToMeshESMFRegridder`.
+    Basic test for :class:`esmf_regrid.experimental.unstructured_scheme.GridToMeshESMFRegridder`.
 
-    Tests with method="bilinear".
+    Tests with method="bilinear" and method="nearest".
     """
     n_lons = 6
     n_lats = 5
     lon_bounds = (-180, 180)
     lat_bounds = (-90, 90)
     src = _grid_cube(n_lons, n_lats, lon_bounds, lat_bounds, circular=True)
     face_tgt = _gridlike_mesh_cube(n_lons, n_lats, location="face")
     node_tgt = _gridlike_mesh_cube(n_lons, n_lats, location="node")
 
     src = _add_metadata(src)
     src.data[:] = 1  # Ensure all data in the source is one.
-    face_regridder = GridToMeshESMFRegridder(src, face_tgt, method="bilinear")
-    node_regridder = GridToMeshESMFRegridder(src, node_tgt, method="bilinear")
+    face_regridder = GridToMeshESMFRegridder(src, face_tgt, method=method)
+    node_regridder = GridToMeshESMFRegridder(src, node_tgt, method=method)
 
-    assert face_regridder.regridder.method == "bilinear"
-    assert node_regridder.regridder.method == "bilinear"
+    assert face_regridder.regridder.method == method
+    assert node_regridder.regridder.method == method
 
     face_expected_data = np.ones_like(face_tgt.data)
     node_expected_data = np.ones_like(node_tgt.data)
     face_result = face_regridder(src)
     node_result = node_regridder(src)
 
     # Lenient check for data.
@@ -112,15 +113,15 @@
     node_expected_cube.data = node_result.data
     assert face_expected_cube == face_result
     assert node_expected_cube == node_result
 
 
 def test_multidim_cubes():
     """
-    Test for :func:`esmf_regrid.experimental.unstructured_scheme.regrid_rectilinear_to_unstructured`.
+    Test for :class:`esmf_regrid.experimental.unstructured_scheme.regrid_rectilinear_to_unstructured`.
 
     Tests with multidimensional cubes. The source cube contains
     coordinates on the dimensions before and after the grid dimensions.
     """
     tgt = _flat_mesh_cube()
     mesh = tgt.mesh
     mesh_length = mesh.connectivity(contains_face=True).shape[0]
@@ -161,15 +162,15 @@
     # Check metadata and scalar coords.
     result.data = expected_data
     assert expected_cube == result
 
 
 def test_invalid_mdtol():
     """
-    Test initialisation of :func:`esmf_regrid.experimental.unstructured_scheme.GridToMeshESMFRegridder`.
+    Test initialisation of :class:`esmf_regrid.experimental.unstructured_scheme.GridToMeshESMFRegridder`.
 
     Checks that an error is raised when mdtol is out of range.
     """
     tgt = _flat_mesh_cube()
 
     n_lons = 6
     n_lats = 5
@@ -181,72 +182,79 @@
         _ = GridToMeshESMFRegridder(src, tgt, mdtol=2)
     with pytest.raises(ValueError):
         _ = GridToMeshESMFRegridder(src, tgt, mdtol=-1)
 
 
 def test_invalid_method():
     """
-    Test initialisation of :func:`esmf_regrid.experimental.unstructured_scheme.GridToMeshESMFRegridder`.
+    Test initialisation of :class:`esmf_regrid.experimental.unstructured_scheme.GridToMeshESMFRegridder`.
 
     Checks that an error is raised when the method is invalid.
     """
     n_lons = 6
     n_lats = 5
     lon_bounds = (-180, 180)
     lat_bounds = (-90, 90)
     face_tgt = _gridlike_mesh_cube(n_lons, n_lats, location="face")
     edge_tgt = _gridlike_mesh_cube(n_lons, n_lats, location="edge")
     node_tgt = _gridlike_mesh_cube(n_lons, n_lats, location="node")
     src = _grid_cube(n_lons, n_lats, lon_bounds, lat_bounds, circular=True)
 
-    with pytest.raises(ValueError):
+    with pytest.raises(NotImplementedError):
         _ = GridToMeshESMFRegridder(src, face_tgt, method="other")
     with pytest.raises(ValueError) as excinfo:
         _ = GridToMeshESMFRegridder(src, node_tgt, method="conservative")
     expected_message = (
         "Conservative regridding requires a target cube located on "
         "the face of a cube, target cube had the node location."
     )
     assert expected_message in str(excinfo.value)
     with pytest.raises(ValueError) as excinfo:
         _ = GridToMeshESMFRegridder(src, edge_tgt, method="bilinear")
     expected_message = (
-        "Bilinear regridding requires a target cube with a node "
+        "bilinear regridding requires a target cube with a node "
+        "or face location, target cube had the edge location."
+    )
+    assert expected_message in str(excinfo.value)
+    with pytest.raises(ValueError) as excinfo:
+        _ = GridToMeshESMFRegridder(src, edge_tgt, method="nearest")
+    expected_message = (
+        "nearest regridding requires a target cube with a node "
         "or face location, target cube had the edge location."
     )
     assert expected_message in str(excinfo.value)
 
 
 def test_invalid_resolution():
     """
-    Test initialisation of :func:`esmf_regrid.experimental.unstructured_scheme.GridToMeshESMFRegridder`.
+    Test initialisation of :class:`esmf_regrid.experimental.unstructured_scheme.GridToMeshESMFRegridder`.
 
     Checks that an error is raised when the resolution is invalid.
     """
     n_lons = 6
     n_lats = 5
     lon_bounds = (-180, 180)
     lat_bounds = (-90, 90)
     tgt = _gridlike_mesh_cube(n_lons, n_lats, location="face")
     src = _grid_cube(n_lons, n_lats, lon_bounds, lat_bounds, circular=True)
 
     with pytest.raises(ValueError) as excinfo:
-        _ = GridToMeshESMFRegridder(src, tgt, method="conservative", resolution=-1)
+        _ = GridToMeshESMFRegridder(src, tgt, method="conservative", src_resolution=-1)
     expected_message = "resolution must be a positive integer."
     assert expected_message in str(excinfo.value)
 
     with pytest.raises(ValueError) as excinfo:
-        _ = GridToMeshESMFRegridder(src, tgt, method="bilinear", resolution=4)
+        _ = GridToMeshESMFRegridder(src, tgt, method="bilinear", src_resolution=4)
     expected_message = "resolution can only be set for conservative regridding."
     assert expected_message in str(excinfo.value)
 
 
 def test_default_mdtol():
     """
-    Test initialisation of :func:`esmf_regrid.experimental.unstructured_scheme.GridToMeshESMFRegridder`.
+    Test initialisation of :class:`esmf_regrid.experimental.unstructured_scheme.GridToMeshESMFRegridder`.
 
     Checks that default mdtol values are as expected.
     """
     n_lons = 6
     n_lats = 5
     lon_bounds = (-180, 180)
     lat_bounds = (-90, 90)
@@ -257,15 +265,15 @@
     assert rg_con.mdtol == 1
     rg_bi = GridToMeshESMFRegridder(src, tgt, method="bilinear")
     assert rg_bi.mdtol == 0
 
 
 def test_mismatched_grids():
     """
-    Test error handling in calling of :func:`esmf_regrid.experimental.unstructured_scheme.GridToMeshESMFRegridder`.
+    Test error handling in calling of :class:`esmf_regrid.experimental.unstructured_scheme.GridToMeshESMFRegridder`.
 
     Checks that an error is raised when the regridder is called with a
     cube whose grid does not match with the one used when initialising
     the regridder.
     """
     tgt = _flat_mesh_cube()
     n_lons = 6
@@ -283,15 +291,15 @@
     )
     with pytest.raises(ValueError):
         _ = regridder(src_other)
 
 
 def test_mask_handling():
     """
-    Test masked data handling for :func:`esmf_regrid.experimental.unstructured_scheme.GridToMeshESMFRegridder`.
+    Test masked data handling for :class:`esmf_regrid.experimental.unstructured_scheme.GridToMeshESMFRegridder`.
 
     Tests masked data handling for multiple valid values for mdtol.
     """
     tgt = _flat_mesh_cube()
 
     n_lons = 6
     n_lats = 5
@@ -353,35 +361,35 @@
     expected_chunks = ((120,), (2, 2))
     assert out_chunks == expected_chunks
     assert np.allclose(result.data, src_data.reshape([-1, h]))
 
 
 def test_resolution():
     """
-    Test for :func:`esmf_regrid.experimental.unstructured_scheme.GridToMeshESMFRegridder`.
+    Test for :class:`esmf_regrid.experimental.unstructured_scheme.GridToMeshESMFRegridder`.
 
-    Tests for the resolution keyword.
+    Tests for the src_resolution keyword.
     """
     tgt = _flat_mesh_cube()
     n_lons = 6
     n_lats = 5
     lon_bounds = (-180, 180)
     lat_bounds = (-90, 90)
     grid = _grid_cube(n_lons, n_lats, lon_bounds, lat_bounds, circular=True)
 
     resolution = 8
 
-    result = GridToMeshESMFRegridder(grid, tgt, resolution=resolution)
+    result = GridToMeshESMFRegridder(grid, tgt, src_resolution=resolution)
     assert result.resolution == resolution
     assert result.regridder.src.resolution == resolution
 
 
 def test_curvilinear():
     """
-    Test for :func:`esmf_regrid.experimental.unstructured_scheme.regrid_rectilinear_to_unstructured`.
+    Test for :class:`esmf_regrid.experimental.unstructured_scheme.regrid_rectilinear_to_unstructured`.
 
     Tests with curvilinear target cube.
     """
     tgt = _flat_mesh_cube()
     mesh = tgt.mesh
     mesh_length = mesh.connectivity(contains_face=True).shape[0]
     n_lons = 6
@@ -427,15 +435,15 @@
 
 
 @pytest.mark.parametrize(
     "resolution", (None, 2), ids=("no resolution", "with resolution")
 )
 def test_masks(resolution):
     """
-    Test initialisation of :func:`esmf_regrid.experimental.unstructured_scheme.GridToMeshESMFRegridder`.
+    Test initialisation of :class:`esmf_regrid.experimental.unstructured_scheme.GridToMeshESMFRegridder`.
 
     Checks that the `use_src_mask` and `use_tgt_mask` keywords work properly.
     """
     if resolution is None:
         src = _curvilinear_cube(7, 6, [-180, 180], [-90, 90])
     else:
         # The resolution keyword is only valid for rectilinear grids.
@@ -452,20 +460,20 @@
         src_discontiguous.coord("longitude").bounds[0, 0] = 0
 
     tgt_mask = np.zeros([7 * 6], dtype=bool)
     tgt_mask[0] = True
     tgt.data = np.ma.array(tgt.data, mask=tgt_mask)
 
     rg_src_masked = GridToMeshESMFRegridder(
-        src_discontiguous, tgt, use_src_mask=True, resolution=resolution
+        src_discontiguous, tgt, use_src_mask=True, src_resolution=resolution
     )
     rg_tgt_masked = GridToMeshESMFRegridder(
-        src, tgt, use_tgt_mask=True, resolution=resolution
+        src, tgt, use_tgt_mask=True, src_resolution=resolution
     )
-    rg_unmasked = GridToMeshESMFRegridder(src, tgt, resolution=resolution)
+    rg_unmasked = GridToMeshESMFRegridder(src, tgt, src_resolution=resolution)
 
     weights_src_masked = rg_src_masked.regridder.weight_matrix
     weights_tgt_masked = rg_tgt_masked.regridder.weight_matrix
     weights_unmasked = rg_unmasked.regridder.weight_matrix
 
     # Check there are no weights associated with the masked point.
     assert weights_src_masked[:, 0].nnz == 0
```

### Comparing `esmf_regrid-0.6.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test_MeshToGridESMFRegridder.py` & `esmf_regrid-0.7.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test_MeshToGridESMFRegridder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-"""Unit tests for :func:`esmf_regrid.experimental.unstructured_scheme.MeshToGridESMFRegridder`."""
+"""Unit tests for :class:`esmf_regrid.experimental.unstructured_scheme.MeshToGridESMFRegridder`."""
 
 import dask.array as da
 from iris.coords import AuxCoord, DimCoord
 from iris.cube import Cube
 import numpy as np
 import pytest
 
 from esmf_regrid.experimental.unstructured_scheme import (
     MeshToGridESMFRegridder,
 )
-from esmf_regrid.tests.unit.experimental.unstructured_scheme.test__mesh_to_MeshInfo import (
+from esmf_regrid.tests.unit.schemes.test__cube_to_GridInfo import (
+    _curvilinear_cube,
+    _grid_cube,
+)
+from esmf_regrid.tests.unit.schemes.test__mesh_to_MeshInfo import (
     _gridlike_mesh,
     _gridlike_mesh_cube,
 )
-from esmf_regrid.tests.unit.experimental.unstructured_scheme.test__regrid_unstructured_to_rectilinear__prepare import (
+from esmf_regrid.tests.unit.schemes.test__regrid_unstructured_to_rectilinear__prepare import (
     _flat_mesh_cube,
     _full_mesh,
 )
-from esmf_regrid.tests.unit.schemes.test__cube_to_GridInfo import (
-    _curvilinear_cube,
-    _grid_cube,
-)
 
 
 def _add_metadata(cube):
     result = cube.copy()
     result.units = "K"
     result.attributes = {"a": 1}
     result.standard_name = "air_temperature"
@@ -33,15 +33,15 @@
     result.add_aux_coord(scalar_height)
     result.add_aux_coord(scalar_time)
     return result
 
 
 def test_flat_cubes():
     """
-    Basic test for :func:`esmf_regrid.experimental.unstructured_scheme.MeshToGridESMFRegridder`.
+    Basic test for :class:`esmf_regrid.experimental.unstructured_scheme.MeshToGridESMFRegridder`.
 
     Tests with flat cubes as input (a 1D mesh cube and a 2D grid cube).
     """
     src = _flat_mesh_cube()
 
     n_lons = 6
     n_lats = 5
@@ -64,38 +64,39 @@
     assert np.allclose(expected_data, result.data)
 
     # Check metadata and scalar coords.
     expected_cube.data = result.data
     assert expected_cube == result
 
 
-def test_bilinear():
+@pytest.mark.parametrize("method", ["bilinear", "nearest"])
+def test_node_friendly_methods(method):
     """
-    Basic test for :func:`esmf_regrid.experimental.unstructured_scheme.MeshToGridESMFRegridder`.
+    Basic test for :class:`esmf_regrid.experimental.unstructured_scheme.MeshToGridESMFRegridder`.
 
-    Tests with method="bilinear".
+    Tests with method="bilinear" and method="nearest".
     """
     n_lons = 6
     n_lats = 5
     lon_bounds = (-180, 180)
     lat_bounds = (-90, 90)
     tgt = _grid_cube(n_lons, n_lats, lon_bounds, lat_bounds, circular=True)
     face_src = _gridlike_mesh_cube(n_lons, n_lats, location="face")
     node_src = _gridlike_mesh_cube(n_lons, n_lats, location="node")
 
     face_src = _add_metadata(face_src)
     node_src = _add_metadata(node_src)
     # Ensure all data in the source is one.
     face_src.data[:] = 1
     node_src.data[:] = 1
-    face_regridder = MeshToGridESMFRegridder(face_src, tgt, method="bilinear")
-    node_regridder = MeshToGridESMFRegridder(node_src, tgt, method="bilinear")
+    face_regridder = MeshToGridESMFRegridder(face_src, tgt, method=method)
+    node_regridder = MeshToGridESMFRegridder(node_src, tgt, method=method)
 
-    assert face_regridder.regridder.method == "bilinear"
-    assert node_regridder.regridder.method == "bilinear"
+    assert face_regridder.regridder.method == method
+    assert node_regridder.regridder.method == method
 
     expected_data = np.ones_like(tgt.data)
     face_result = face_regridder(face_src)
     node_result = node_regridder(node_src)
 
     # Lenient check for data.
     assert np.allclose(expected_data, face_result.data)
@@ -105,15 +106,15 @@
     expected_cube = _add_metadata(tgt)
     expected_cube.data = face_result.data = node_result.data
     assert expected_cube == face_result == node_result
 
 
 def test_multidim_cubes():
     """
-    Test for :func:`esmf_regrid.experimental.unstructured_scheme.MeshToGridESMFRegridder`.
+    Test for :class:`esmf_regrid.experimental.unstructured_scheme.MeshToGridESMFRegridder`.
 
     Tests with multidimensional cubes. The source cube contains
     coordinates on the dimensions before and after the mesh dimension.
     """
     mesh = _full_mesh()
     mesh_length = mesh.connectivity(contains_face=True).shape[0]
 
@@ -156,15 +157,15 @@
     # Check metadata and scalar coords.
     result.data = expected_data
     assert expected_cube == result
 
 
 def test_invalid_mdtol():
     """
-    Test initialisation of :func:`esmf_regrid.experimental.unstructured_scheme.MeshToGridESMFRegridder`.
+    Test initialisation of :class:`esmf_regrid.experimental.unstructured_scheme.MeshToGridESMFRegridder`.
 
     Checks that an error is raised when mdtol is out of range.
     """
     src = _flat_mesh_cube()
 
     n_lons = 6
     n_lats = 5
@@ -176,72 +177,79 @@
         _ = MeshToGridESMFRegridder(src, tgt, mdtol=2)
     with pytest.raises(ValueError):
         _ = MeshToGridESMFRegridder(src, tgt, mdtol=-1)
 
 
 def test_invalid_method():
     """
-    Test initialisation of :func:`esmf_regrid.experimental.unstructured_scheme.MeshToGridESMFRegridder`.
+    Test initialisation of :class:`esmf_regrid.experimental.unstructured_scheme.MeshToGridESMFRegridder`.
 
     Checks that an error is raised when method is invalid.
     """
     n_lons = 6
     n_lats = 5
     lon_bounds = (-180, 180)
     lat_bounds = (-90, 90)
     face_src = _gridlike_mesh_cube(n_lons, n_lats, location="face")
     edge_src = _gridlike_mesh_cube(n_lons, n_lats, location="edge")
     node_src = _gridlike_mesh_cube(n_lons, n_lats, location="node")
     tgt = _grid_cube(n_lons, n_lats, lon_bounds, lat_bounds, circular=True)
 
-    with pytest.raises(ValueError):
+    with pytest.raises(NotImplementedError):
         _ = MeshToGridESMFRegridder(face_src, tgt, method="other")
     with pytest.raises(ValueError) as excinfo:
         _ = MeshToGridESMFRegridder(node_src, tgt, method="conservative")
     expected_message = (
         "Conservative regridding requires a source cube located on "
         "the face of a cube, target cube had the node location."
     )
     assert expected_message in str(excinfo.value)
     with pytest.raises(ValueError) as excinfo:
         _ = MeshToGridESMFRegridder(edge_src, tgt, method="bilinear")
     expected_message = (
-        "Bilinear regridding requires a source cube with a node "
+        "bilinear regridding requires a source cube with a node "
+        "or face location, target cube had the edge location."
+    )
+    assert expected_message in str(excinfo.value)
+    with pytest.raises(ValueError) as excinfo:
+        _ = MeshToGridESMFRegridder(edge_src, tgt, method="nearest")
+    expected_message = (
+        "nearest regridding requires a source cube with a node "
         "or face location, target cube had the edge location."
     )
     assert expected_message in str(excinfo.value)
 
 
 def test_invalid_resolution():
     """
-    Test initialisation of :func:`esmf_regrid.experimental.unstructured_scheme.MeshToGridESMFRegridder`.
+    Test initialisation of :class:`esmf_regrid.experimental.unstructured_scheme.MeshToGridESMFRegridder`.
 
     Checks that an error is raised when the resolution is invalid.
     """
     n_lons = 6
     n_lats = 5
     lon_bounds = (-180, 180)
     lat_bounds = (-90, 90)
     src = _gridlike_mesh_cube(n_lons, n_lats, location="face")
     tgt = _grid_cube(n_lons, n_lats, lon_bounds, lat_bounds, circular=True)
 
     with pytest.raises(ValueError) as excinfo:
-        _ = MeshToGridESMFRegridder(src, tgt, method="conservative", resolution=-1)
+        _ = MeshToGridESMFRegridder(src, tgt, method="conservative", tgt_resolution=-1)
     expected_message = "resolution must be a positive integer."
     assert expected_message in str(excinfo.value)
 
     with pytest.raises(ValueError) as excinfo:
-        _ = MeshToGridESMFRegridder(src, tgt, method="bilinear", resolution=4)
+        _ = MeshToGridESMFRegridder(src, tgt, method="bilinear", tgt_resolution=4)
     expected_message = "resolution can only be set for conservative regridding."
     assert expected_message in str(excinfo.value)
 
 
 def test_default_mdtol():
     """
-    Test initialisation of :func:`esmf_regrid.experimental.unstructured_scheme.MeshToGridESMFRegridder`.
+    Test initialisation of :class:`esmf_regrid.experimental.unstructured_scheme.MeshToGridESMFRegridder`.
 
     Checks that default mdtol values are as expected.
     """
     n_lons = 6
     n_lats = 5
     lon_bounds = (-180, 180)
     lat_bounds = (-90, 90)
@@ -253,15 +261,15 @@
     rg_bi = MeshToGridESMFRegridder(src, tgt, method="bilinear")
     assert rg_bi.mdtol == 0
 
 
 @pytest.mark.xfail
 def test_mistmatched_mesh():
     """
-    Test the calling of :func:`esmf_regrid.experimental.unstructured_scheme.MeshToGridESMFRegridder`.
+    Test the calling of :class:`esmf_regrid.experimental.unstructured_scheme.MeshToGridESMFRegridder`.
 
     Checks that an error is raised when the regridder is called with a cube
     whose mesh does not match the one used for initialisation.
     """
     n_lons = 6
     n_lats = 5
     lon_bounds = (-180, 180)
@@ -323,39 +331,43 @@
     expected_chunks = ((1,), (3, 3, 3), (10,), (12,), (2, 2))
     assert out_chunks == expected_chunks
     assert np.allclose(result.data.reshape([1, i, -1, h]), src_data)
 
 
 def test_resolution():
     """
-    Test for :func:`esmf_regrid.experimental.unstructured_scheme.MeshToGridESMFRegridder`.
+    Test for :class:`esmf_regrid.experimental.unstructured_scheme.MeshToGridESMFRegridder`.
 
-    Tests for the resolution keyword.
+    Tests for the tgt_resolution keyword.
     """
     mesh_cube = _flat_mesh_cube()
 
     lon_bounds = (-180, 180)
     lat_bounds = (-90, 90)
     lon_bands = _grid_cube(1, 4, lon_bounds, lat_bounds)
     lat_bands = _grid_cube(4, 1, lon_bounds, lat_bounds)
 
     resolution = 8
 
-    lon_band_rg = MeshToGridESMFRegridder(mesh_cube, lon_bands, resolution=resolution)
+    lon_band_rg = MeshToGridESMFRegridder(
+        mesh_cube, lon_bands, tgt_resolution=resolution
+    )
     assert lon_band_rg.resolution == resolution
     assert lon_band_rg.regridder.tgt.resolution == resolution
 
-    lat_band_rg = MeshToGridESMFRegridder(mesh_cube, lat_bands, resolution=resolution)
+    lat_band_rg = MeshToGridESMFRegridder(
+        mesh_cube, lat_bands, tgt_resolution=resolution
+    )
     assert lat_band_rg.resolution == resolution
     assert lat_band_rg.regridder.tgt.resolution == resolution
 
 
 def test_curvilinear():
     """
-    Test for :func:`esmf_regrid.experimental.unstructured_scheme.MeshToGridESMFRegridder`.
+    Test for :class:`esmf_regrid.experimental.unstructured_scheme.MeshToGridESMFRegridder`.
 
     Tests with curvilinear source cube.
     """
     mesh = _full_mesh()
     mesh_length = mesh.connectivity(contains_face=True).shape[0]
 
     h = 2
@@ -403,15 +415,15 @@
 
 
 @pytest.mark.parametrize(
     "resolution", (None, 2), ids=("no resolution", "with resolution")
 )
 def test_masks(resolution):
     """
-    Test initialisation of :func:`esmf_regrid.experimental.unstructured_scheme.MeshToGridESMFRegridder`.
+    Test initialisation of :class:`esmf_regrid.experimental.unstructured_scheme.MeshToGridESMFRegridder`.
 
     Checks that the `use_src_mask` and `use_tgt_mask` keywords work properly.
     """
     src = _gridlike_mesh_cube(7, 6)
     if resolution is None:
         tgt = _curvilinear_cube(6, 7, [-180, 180], [-90, 90])
     else:
@@ -428,20 +440,20 @@
     tgt.data = np.ma.array(tgt.data, mask=tgt_mask)
     tgt_discontiguous = tgt.copy()
     if resolution is None:
         tgt_discontiguous.coord("latitude").bounds[0, 0] = 0
         tgt_discontiguous.coord("longitude").bounds[0, 0] = 0
 
     rg_src_masked = MeshToGridESMFRegridder(
-        src, tgt, use_src_mask=True, resolution=resolution
+        src, tgt, use_src_mask=True, tgt_resolution=resolution
     )
     rg_tgt_masked = MeshToGridESMFRegridder(
-        src, tgt_discontiguous, use_tgt_mask=True, resolution=resolution
+        src, tgt_discontiguous, use_tgt_mask=True, tgt_resolution=resolution
     )
-    rg_unmasked = MeshToGridESMFRegridder(src, tgt, resolution=resolution)
+    rg_unmasked = MeshToGridESMFRegridder(src, tgt, tgt_resolution=resolution)
 
     weights_src_masked = rg_src_masked.regridder.weight_matrix
     weights_tgt_masked = rg_tgt_masked.regridder.weight_matrix
     weights_unmasked = rg_unmasked.regridder.weight_matrix
 
     # Check there are no weights associated with the masked point.
     assert weights_src_masked[:, 0].nnz == 0
```

### Comparing `esmf_regrid-0.6.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test__create_cube.py` & `esmf_regrid-0.7.0/esmf_regrid/tests/unit/schemes/test__create_cube.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Unit tests for miscellaneous helper functions in `esmf_regrid.experimental.unstructured_scheme`."""
 
 import iris
 from iris.coords import AuxCoord, DimCoord
 from iris.cube import Cube
 import numpy as np
 
-from esmf_regrid.experimental.unstructured_scheme import _create_cube
+from esmf_regrid.schemes import _create_cube
 
 
 def test_create_cube_2D():
     """Test creation of 2D output grid."""
     data = np.ones([2, 3])
 
     # Create a source cube with metadata and scalar coords
```

### Comparing `esmf_regrid-0.6.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test__mesh_to_MeshInfo.py` & `esmf_regrid-0.7.0/esmf_regrid/tests/unit/schemes/test__mesh_to_MeshInfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from iris.cube import Cube
 from iris.experimental.ugrid import Connectivity, Mesh
 import numpy as np
 from numpy import ma
 import scipy.sparse
 
 from esmf_regrid.esmf_regridder import Regridder
-from esmf_regrid.experimental.unstructured_scheme import _mesh_to_MeshInfo
+from esmf_regrid.schemes import _mesh_to_MeshInfo
 
 
 def _pyramid_topology_connectivity_array():
     """
     Generate the face_node_connectivity array for a topological pyramid.
 
     The mesh described is a topological pyramid in the sense that there
```

### Comparing `esmf_regrid-0.6.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test__regrid_unstructured_to_rectilinear__prepare.py` & `esmf_regrid-0.7.0/esmf_regrid/tests/unit/schemes/test__regrid_unstructured_to_rectilinear__prepare.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 from iris.coords import AuxCoord
 from iris.cube import Cube
 import numpy as np
 
 from esmf_regrid.esmf_regridder import GridInfo
 from esmf_regrid.experimental.unstructured_regrid import MeshInfo
-from esmf_regrid.experimental.unstructured_scheme import (
+from esmf_regrid.schemes import (
     _regrid_unstructured_to_rectilinear__prepare,
 )
-from esmf_regrid.tests.unit.experimental.unstructured_scheme.test__cube_to_GridInfo import (
+from esmf_regrid.tests.unit.schemes.test__cube_to_GridInfo import (
     _grid_cube,
 )
-from esmf_regrid.tests.unit.experimental.unstructured_scheme.test__mesh_to_MeshInfo import (
+from esmf_regrid.tests.unit.schemes.test__mesh_to_MeshInfo import (
     _example_mesh,
 )
 
 
 def _full_mesh():
     mesh = _example_mesh()
 
@@ -59,14 +59,14 @@
     n_lats = 5
     lon_bounds = (-180, 180)
     lat_bounds = (-90, 90)
     tgt = _grid_cube(n_lons, n_lats, lon_bounds, lat_bounds, circular=True)
     regrid_info = _regrid_unstructured_to_rectilinear__prepare(
         src, tgt, method="conservative"
     )
-    mesh_dim, grid_x, grid_y, regridder = regrid_info
+    (mesh_dim,), (grid_x, grid_y), regridder = regrid_info
 
     assert mesh_dim == 0
     assert grid_x == tgt.coord("longitude")
     assert grid_y == tgt.coord("latitude")
     assert type(regridder.tgt) == GridInfo
     assert type(regridder.src) == MeshInfo
```

### Comparing `esmf_regrid-0.6.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test_regrid_rectilinear_to_unstructured.py` & `esmf_regrid-0.7.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test_regrid_rectilinear_to_unstructured.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 import numpy as np
 from numpy import ma
 import pytest
 
 from esmf_regrid.experimental.unstructured_scheme import (
     regrid_rectilinear_to_unstructured,
 )
-from esmf_regrid.tests.unit.experimental.unstructured_scheme.test__cube_to_GridInfo import (
+from esmf_regrid.tests.unit.schemes.test__cube_to_GridInfo import (
     _grid_cube,
 )
-from esmf_regrid.tests.unit.experimental.unstructured_scheme.test__mesh_to_MeshInfo import (
+from esmf_regrid.tests.unit.schemes.test__mesh_to_MeshInfo import (
     _gridlike_mesh_cube,
 )
-from esmf_regrid.tests.unit.experimental.unstructured_scheme.test__regrid_unstructured_to_rectilinear__prepare import (
+from esmf_regrid.tests.unit.schemes.test__regrid_unstructured_to_rectilinear__prepare import (
     _flat_mesh_cube,
 )
 
 
 def _add_metadata(cube):
     result = cube.copy()
     result.units = "K"
@@ -66,33 +66,34 @@
     # Check metadata and scalar coords.
     expected_cube.data = result.data
     assert expected_cube == result
     expected_cube.data = result_transposed.data
     assert expected_cube == result_transposed
 
 
-def test_bilinear():
+@pytest.mark.parametrize("method", ("bilinear", "nearest"))
+def test_node_friendly_methods(method):
     """
     Basic test for :func:`esmf_regrid.experimental.unstructured_scheme.regrid_rectilinear_to_unstructured`.
 
-    Tests with the bilinear method.
+    Tests with the bilinear and nearest method.
     """
     n_lons = 6
     n_lats = 5
     lon_bounds = (-180, 180)
     lat_bounds = (-90, 90)
     tgt = _gridlike_mesh_cube(n_lons, n_lats, location="node")
     src = _grid_cube(n_lons, n_lats, lon_bounds, lat_bounds, circular=True)
     # Ensure data in the target grid is different to the expected data.
     # i.e. target grid data is all zero, expected data is all one
     tgt.data[:] = 0
 
     src = _add_metadata(src)
     src.data[:] = 1  # Ensure all data in the source is one.
-    result = regrid_rectilinear_to_unstructured(src, tgt, method="bilinear")
+    result = regrid_rectilinear_to_unstructured(src, tgt, method=method)
 
     expected_data = np.ones_like(tgt.data)
     expected_cube = _add_metadata(tgt)
 
     # Lenient check for data.
     assert np.allclose(expected_data, result.data)
 
@@ -114,27 +115,34 @@
     node_tgt = _gridlike_mesh_cube(n_lons, n_lats, location="node")
     edge_tgt = _gridlike_mesh_cube(n_lons, n_lats, location="edge")
     face_tgt = _gridlike_mesh_cube(n_lons, n_lats, location="face")
     src = _grid_cube(n_lons, n_lats, lon_bounds, lat_bounds, circular=True)
 
     with pytest.raises(ValueError):
         _ = regrid_rectilinear_to_unstructured(src, src, method="bilinear")
-    with pytest.raises(ValueError):
+    with pytest.raises(NotImplementedError):
         _ = regrid_rectilinear_to_unstructured(src, face_tgt, method="other")
     with pytest.raises(ValueError) as excinfo:
         _ = regrid_rectilinear_to_unstructured(src, node_tgt, method="conservative")
     expected_message = (
         "Conservative regridding requires a target cube located on "
         "the face of a cube, target cube had the node location."
     )
     assert expected_message in str(excinfo.value)
     with pytest.raises(ValueError) as excinfo:
         _ = regrid_rectilinear_to_unstructured(src, edge_tgt, method="bilinear")
     expected_message = (
-        "Bilinear regridding requires a target cube with a node "
+        "bilinear regridding requires a target cube with a node "
+        "or face location, target cube had the edge location."
+    )
+    assert expected_message in str(excinfo.value)
+    with pytest.raises(ValueError) as excinfo:
+        _ = regrid_rectilinear_to_unstructured(src, edge_tgt, method="nearest")
+    expected_message = (
+        "nearest regridding requires a target cube with a node "
         "or face location, target cube had the edge location."
     )
     assert expected_message in str(excinfo.value)
 
 
 def test_multidim_cubes():
     """
@@ -235,15 +243,15 @@
     assert ma.allclose(expected_1, result_1.data)
 
 
 def test_resolution():
     """
     Basic test for :func:`esmf_regrid.experimental.unstructured_scheme.regrid_rectilinear_to_unstructured`.
 
-    Tests the resolution keyword with grids that would otherwise not work.
+    Tests the src_resolution keyword with grids that would otherwise not work.
     """
     tgt = _flat_mesh_cube()
 
     # The resulting grid has full latitude bounds and cells must be split up.
     n_lons = 1
     n_lats = 4
     lon_bounds = (-180, 180)
@@ -251,19 +259,19 @@
     src = _grid_cube(n_lons, n_lats, lon_bounds, lat_bounds)
     # Ensure data in the target grid is different to the expected data.
     # i.e. target grid data is all zero, expected data is all one
     tgt.data[:] = 0
 
     src = _add_metadata(src)
     src.data[:] = 1  # Ensure all data in the source is one.
-    result = regrid_rectilinear_to_unstructured(src, tgt, resolution=8)
+    result = regrid_rectilinear_to_unstructured(src, tgt, src_resolution=8)
 
     expected_data = np.ones_like(tgt.data)
     expected_cube = _add_metadata(tgt)
 
     # Lenient check for data.
-    # Note that when resolution=None, this would be a fully masked array.
+    # Note that when src_resolution=None, this would be a fully masked array.
     assert np.allclose(expected_data, result.data)
 
     # Check metadata and scalar coords.
     expected_cube.data = result.data
     assert expected_cube == result
```

### Comparing `esmf_regrid-0.6.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test_regrid_unstructured_to_rectilinear.py` & `esmf_regrid-0.7.0/esmf_regrid/tests/unit/experimental/unstructured_scheme/test_regrid_unstructured_to_rectilinear.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 from iris.cube import Cube
 import numpy as np
 import pytest
 
 from esmf_regrid.experimental.unstructured_scheme import (
     regrid_unstructured_to_rectilinear,
 )
-from esmf_regrid.tests.unit.experimental.unstructured_scheme.test__cube_to_GridInfo import (
+from esmf_regrid.tests.unit.schemes.test__cube_to_GridInfo import (
     _grid_cube,
 )
-from esmf_regrid.tests.unit.experimental.unstructured_scheme.test__mesh_to_MeshInfo import (
+from esmf_regrid.tests.unit.schemes.test__mesh_to_MeshInfo import (
     _gridlike_mesh_cube,
 )
-from esmf_regrid.tests.unit.experimental.unstructured_scheme.test__regrid_unstructured_to_rectilinear__prepare import (
+from esmf_regrid.tests.unit.schemes.test__regrid_unstructured_to_rectilinear__prepare import (
     _flat_mesh_cube,
     _full_mesh,
 )
 
 
 def _add_metadata(cube):
     result = cube.copy()
@@ -60,33 +60,34 @@
     assert np.allclose(expected_data, result.data)
 
     # Check metadata and scalar coords.
     expected_cube.data = result.data
     assert expected_cube == result
 
 
-def test_bilinear():
+@pytest.mark.parametrize("method", ("bilinear", "nearest"))
+def test_node_friendly_methods(method):
     """
     Basic test for :func:`esmf_regrid.experimental.unstructured_scheme.regrid_unstructured_to_rectilinear`.
 
-    Tests with the bilinear method.
+    Tests with the bilinear and nearest method.
     """
     n_lons = 6
     n_lats = 5
     lon_bounds = (-180, 180)
     lat_bounds = (-90, 90)
     src = _gridlike_mesh_cube(n_lons, n_lats, location="node")
     tgt = _grid_cube(n_lons, n_lats, lon_bounds, lat_bounds, circular=True)
     # Ensure data in the target grid is different to the expected data.
     # i.e. target grid data is all zero, expected data is all one
     tgt.data[:] = 0
 
     src = _add_metadata(src)
     src.data[:] = 1  # Ensure all data in the source is one.
-    result = regrid_unstructured_to_rectilinear(src, tgt, method="bilinear")
+    result = regrid_unstructured_to_rectilinear(src, tgt, method=method)
 
     expected_data = np.ones([n_lats, n_lons])
     expected_cube = _add_metadata(tgt)
 
     # Lenient check for data.
     assert np.allclose(expected_data, result.data)
 
@@ -108,27 +109,34 @@
     node_src = _gridlike_mesh_cube(n_lons, n_lats, location="node")
     edge_src = _gridlike_mesh_cube(n_lons, n_lats, location="edge")
     face_src = _gridlike_mesh_cube(n_lons, n_lats, location="face")
     tgt = _grid_cube(n_lons, n_lats, lon_bounds, lat_bounds, circular=True)
 
     with pytest.raises(ValueError):
         _ = regrid_unstructured_to_rectilinear(tgt, tgt, method="bilinear")
-    with pytest.raises(ValueError):
+    with pytest.raises(NotImplementedError):
         _ = regrid_unstructured_to_rectilinear(face_src, tgt, method="other")
     with pytest.raises(ValueError) as excinfo:
         _ = regrid_unstructured_to_rectilinear(node_src, tgt, method="conservative")
     expected_message = (
         "Conservative regridding requires a source cube located on "
         "the face of a cube, target cube had the node location."
     )
     assert expected_message in str(excinfo.value)
     with pytest.raises(ValueError) as excinfo:
         _ = regrid_unstructured_to_rectilinear(edge_src, tgt, method="bilinear")
     expected_message = (
-        "Bilinear regridding requires a source cube with a node "
+        "bilinear regridding requires a source cube with a node "
+        "or face location, target cube had the edge location."
+    )
+    assert expected_message in str(excinfo.value)
+    with pytest.raises(ValueError) as excinfo:
+        _ = regrid_unstructured_to_rectilinear(edge_src, tgt, method="nearest")
+    expected_message = (
+        "nearest regridding requires a source cube with a node "
         "or face location, target cube had the edge location."
     )
     assert expected_message in str(excinfo.value)
 
 
 def test_multidim_cubes():
     """
@@ -178,15 +186,15 @@
     assert expected_cube == result
 
 
 def test_resolution():
     """
     Basic test for :func:`esmf_regrid.experimental.unstructured_scheme.regrid_unstructured_to_rectilinear`.
 
-    Tests the resolution keyword with grids that would otherwise not work.
+    Tests the tgt_resolution keyword with grids that would otherwise not work.
     """
     src = _flat_mesh_cube()
 
     # The resulting grid has full latitude bounds and cells must be split up.
     n_lons = 1
     n_lats = 5
     lon_bounds = (-180, 180)
@@ -194,19 +202,19 @@
     tgt = _grid_cube(n_lons, n_lats, lon_bounds, lat_bounds)
     # Ensure data in the target grid is different to the expected data.
     # i.e. target grid data is all zero, expected data is all one
     tgt.data[:] = 0
 
     src = _add_metadata(src)
     src.data[:] = 1  # Ensure all data in the source is one.
-    result = regrid_unstructured_to_rectilinear(src, tgt, resolution=8)
+    result = regrid_unstructured_to_rectilinear(src, tgt, tgt_resolution=8)
 
     expected_data = np.ones([n_lats, n_lons])
     expected_cube = _add_metadata(tgt)
 
     # Lenient check for data.
-    # Note that when resolution=None, this would be a fully masked array.
+    # Note that when tgt_resolution=None, this would be a fully masked array.
     assert np.allclose(expected_data, result.data)
 
     # Check metadata and scalar coords.
     expected_cube.data = result.data
     assert expected_cube == result
```

### Comparing `esmf_regrid-0.6.0/esmf_regrid/tests/unit/schemes/test_ESMFAreaWeighted.py` & `esmf_regrid-0.7.0/esmf_regrid/tests/unit/schemes/test_ESMFNearest.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,62 +1,83 @@
-"""Unit tests for :func:`esmf_regrid.schemes.ESMFAreaWeighted`."""
+"""Unit tests for :class:`esmf_regrid.schemes.ESMFNearest`."""
 
 import numpy as np
 from numpy import ma
 import pytest
 
-from esmf_regrid.schemes import ESMFAreaWeighted
+from esmf_regrid.schemes import ESMFNearest
+from esmf_regrid.tests.unit.schemes.__init__ import (
+    _test_mask_from_init,
+    _test_mask_from_regridder,
+)
 from esmf_regrid.tests.unit.schemes.test__cube_to_GridInfo import _grid_cube
+from esmf_regrid.tests.unit.schemes.test__mesh_to_MeshInfo import (
+    _gridlike_mesh_cube,
+)
 
 
-def test_cube_regrid():
+@pytest.mark.parametrize(
+    "src_type,tgt_type", [("grid", "grid"), ("grid", "mesh"), ("mesh", "grid")]
+)
+def test_cube_regrid(src_type, tgt_type):
     """
-    Test that ESMFAreaWeighted can be passed to a cubes regrid method.
+    Test that ESMFNearest can be passed to a cubes regrid method.
 
-    Checks that regridding occurs and that mdtol is used correctly.
+    Checks that regridding occurs.
     """
-    scheme_default = ESMFAreaWeighted()
-    scheme_full_mdtol = ESMFAreaWeighted(mdtol=1)
+    scheme_default = ESMFNearest()
 
     n_lons_src = 6
     n_lons_tgt = 3
     n_lats_src = 4
     n_lats_tgt = 2
     lon_bounds = (-180, 180)
     lat_bounds = (-90, 90)
-    src = _grid_cube(n_lons_src, n_lats_src, lon_bounds, lat_bounds, circular=True)
-    tgt = _grid_cube(n_lons_tgt, n_lats_tgt, lon_bounds, lat_bounds, circular=True)
-    src_data = np.zeros([n_lats_src, n_lons_src])
-    src_mask = np.zeros([n_lats_src, n_lons_src])
-    src_mask[0, 0] = 1
+    if src_type == "grid":
+        src = _grid_cube(n_lons_src, n_lats_src, lon_bounds, lat_bounds, circular=True)
+        src_data = np.zeros([n_lats_src, n_lons_src])
+        src_mask = np.zeros([n_lats_src, n_lons_src])
+        src_mask[0, 0] = 1
+    else:
+        src = _gridlike_mesh_cube(n_lons_src, n_lats_src)
+        src_data = np.zeros([n_lats_src * n_lons_src])
+        src_mask = np.zeros([n_lats_src * n_lons_src])
+        src_mask[0] = 1
+    if tgt_type == "grid":
+        tgt = _grid_cube(n_lons_tgt, n_lats_tgt, lon_bounds, lat_bounds, circular=True)
+        expected_data_default = np.zeros([n_lats_tgt, n_lons_tgt])
+        expected_mask = np.zeros([n_lats_tgt, n_lons_tgt])
+        expected_mask[0, 0] = 1
+    else:
+        tgt = _gridlike_mesh_cube(n_lons_tgt, n_lats_tgt)
+        expected_data_default = np.zeros([n_lats_tgt * n_lons_tgt])
+        expected_mask = np.zeros([n_lats_tgt * n_lons_tgt])
+        expected_mask[0] = 1
     src_data = ma.array(src_data, mask=src_mask)
     src.data = src_data
 
     result_default = src.regrid(tgt, scheme_default)
-    result_full = src.regrid(tgt, scheme_full_mdtol)
-
-    expected_data_default = np.zeros([n_lats_tgt, n_lons_tgt])
-    expected_mask = np.zeros([n_lats_tgt, n_lons_tgt])
-    expected_mask[0, 0] = 1
-    expected_data_full = ma.array(expected_data_default, mask=expected_mask)
 
     expected_cube_default = tgt.copy()
     expected_cube_default.data = expected_data_default
 
-    expected_cube_full = tgt.copy()
-    expected_cube_full.data = expected_data_full
-
     assert expected_cube_default == result_default
-    assert expected_cube_full == result_full
 
 
-def test_invalid_mdtol():
+@pytest.mark.parametrize("mask_keyword", ["use_src_mask", "use_tgt_mask"])
+def test_mask_from_init(mask_keyword):
+    """
+    Test initialisation of :class:`esmf_regrid.schemes.ESMFNearest`.
+
+    Checks that use_src_mask and use_tgt_mask are passed down correctly.
+    """
+    _test_mask_from_init(ESMFNearest, mask_keyword)
+
+
+@pytest.mark.parametrize("mask_keyword", ["use_src_mask", "use_tgt_mask"])
+def test_mask_from_regridder(mask_keyword):
     """
-    Test initialisation of :func:`esmf_regrid.schemes.ESMFAreaWeighted`.
+    Test regridder method of :class:`esmf_regrid.schemes.ESMFNearest`.
 
-    Checks that an error is raised when mdtol is out of range.
+    Checks that use_src_mask and use_tgt_mask are passed down correctly.
     """
-    match = "Value for mdtol must be in range 0 - 1, got "
-    with pytest.raises(ValueError, match=match):
-        _ = ESMFAreaWeighted(mdtol=2)
-    with pytest.raises(ValueError, match=match):
-        _ = ESMFAreaWeighted(mdtol=-1)
+    _test_mask_from_regridder(ESMFNearest, mask_keyword)
```

### Comparing `esmf_regrid-0.6.0/esmf_regrid/tests/unit/schemes/test_ESMFAreaWeightedRegridder.py` & `esmf_regrid-0.7.0/esmf_regrid/tests/unit/schemes/test_ESMFAreaWeightedRegridder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-"""Unit tests for :func:`esmf_regrid.schemes.ESMFAreaWeightedRegridder`."""
+"""Unit tests for :class:`esmf_regrid.schemes.ESMFAreaWeightedRegridder`."""
 
 from cf_units import Unit
 import numpy as np
 import pytest
 
 from esmf_regrid.schemes import ESMFAreaWeightedRegridder
 from esmf_regrid.tests.unit.schemes.test__cube_to_GridInfo import (
     _curvilinear_cube,
     _grid_cube,
 )
 
 
 def test_dim_switching():
     """
-    Test calling of :func:`esmf_regrid.schemes.ESMFAreaWeightedRegridder`.
+    Test calling of :class:`esmf_regrid.schemes.ESMFAreaWeightedRegridder`.
 
     Checks that the regridder accepts a cube with dimensions in a different
     order than the cube which initialised it. Checks that dimension order is
     inherited from the cube in the calling function in both cases.
     """
     n_lons = 6
     n_lats = 5
@@ -37,15 +37,15 @@
     assert unswitched_result.coord(dimensions=(1,)).standard_name == "longitude"
     assert switched_result.coord(dimensions=(0,)).standard_name == "longitude"
     assert switched_result.coord(dimensions=(1,)).standard_name == "latitude"
 
 
 def test_differing_grids():
     """
-    Test calling of :func:`esmf_regrid.schemes.ESMFAreaWeightedRegridder`.
+    Test calling of :class:`esmf_regrid.schemes.ESMFAreaWeightedRegridder`.
 
     Checks that the regridder raises an error when given a cube with a different
     grid to the one it was initialised with.
     """
     n_lons = 6
     n_lats = 5
     lon_bounds = (-180, 180)
@@ -66,15 +66,15 @@
         _ = regridder(src_dif_coord)
     with pytest.raises(ValueError, match=msg):
         _ = regridder(src_dif_circ)
 
 
 def test_invalid_mdtol():
     """
-    Test initialisation of :func:`esmf_regrid.schemes.ESMFAreaWeightedRegridder`.
+    Test initialisation of :class:`esmf_regrid.schemes.ESMFAreaWeightedRegridder`.
 
     Checks that an error is raised when mdtol is out of range.
     """
     n_lons = 6
     n_lats = 5
     lon_bounds = (-180, 180)
     lat_bounds = (-90, 90)
@@ -86,15 +86,15 @@
         _ = ESMFAreaWeightedRegridder(src, tgt, mdtol=2)
     with pytest.raises(ValueError, match=match):
         _ = ESMFAreaWeightedRegridder(src, tgt, mdtol=-1)
 
 
 def test_curvilinear_equivalence():
     """
-    Test initialisation of :func:`esmf_regrid.schemes.ESMFAreaWeightedRegridder`.
+    Test initialisation of :class:`esmf_regrid.schemes.ESMFAreaWeightedRegridder`.
 
     Checks that equivalent curvilinear and rectilinear coordinates give the same
     results.
     """
     n_lons_src = 6
     n_lons_tgt = 3
     n_lats_src = 4
@@ -116,15 +116,15 @@
 
     for regridder in [grid_to_curv, curv_to_grid, curv_to_curv]:
         assert np.allclose(extract_weights(grid_to_grid), extract_weights(regridder))
 
 
 def test_curvilinear_and_rectilinear():
     """
-    Test :func:`esmf_regrid.schemes.ESMFAreaWeightedRegridder`.
+    Test :class:`esmf_regrid.schemes.ESMFAreaWeightedRegridder`.
 
     Checks that a cube with both curvilinear and rectilinear coords still works.
     Checks that the DimCoords have priority over AuxCoords.
     """
     n_lons_src = 6
     n_lons_tgt = 3
     n_lats_src = 4
@@ -169,15 +169,15 @@
     expected.data[:] = 1
     assert expected == result
     assert not np.ma.is_masked(result)
 
 
 def test_unit_equivalence():
     """
-    Test initialisation of :func:`esmf_regrid.schemes.ESMFAreaWeightedRegridder`.
+    Test initialisation of :class:`esmf_regrid.schemes.ESMFAreaWeightedRegridder`.
 
     Checks that equivalent coordinates in degrees and radians give the same results.
     """
     n_lons_src = 6
     n_lons_tgt = 3
     n_lats_src = 4
     n_lats_tgt = 2
@@ -229,15 +229,15 @@
         curv_to_curv_rad,
     ]:
         assert np.allclose(extract_weights(grid_to_grid), extract_weights(regridder))
 
 
 def test_masks():
     """
-    Test initialisation of :func:`esmf_regrid.schemes.ESMFAreaWeightedRegridder`.
+    Test initialisation of :class:`esmf_regrid.schemes.ESMFAreaWeightedRegridder`.
 
     Checks that the `use_src_mask` and `use_tgt_mask` keywords work properly.
     """
     src = _curvilinear_cube(7, 6, [-180, 180], [-90, 90])
     tgt = _curvilinear_cube(6, 7, [-180, 180], [-90, 90])
 
     # Make src and tgt discontiguous at (0, 0)
```

### Comparing `esmf_regrid-0.6.0/esmf_regrid/tests/unit/schemes/test__cube_to_GridInfo.py` & `esmf_regrid-0.7.0/esmf_regrid/tests/unit/schemes/test__cube_to_GridInfo.py`

 * *Files identical despite different names*

### Comparing `esmf_regrid-0.6.0/esmf_regrid/tests/unit/schemes/test_regrid_rectilinear_to_rectilinear.py` & `esmf_regrid-0.7.0/esmf_regrid/tests/unit/schemes/test_regrid_rectilinear_to_rectilinear.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import dask.array as da
 from iris.coord_systems import RotatedGeogCS
 from iris.coords import AuxCoord, DimCoord
 from iris.cube import Cube
 import numpy as np
 from numpy import ma
+import pytest
 
 from esmf_regrid.schemes import regrid_rectilinear_to_rectilinear
 from esmf_regrid.tests.unit.schemes.test__cube_to_GridInfo import (
     _curvilinear_cube,
     _grid_cube,
 )
 
@@ -151,15 +152,17 @@
     assert np.allclose(expected_data, result.data)
 
     # Check metadata and coords.
     result.data = expected_data
     assert expected_cube == result
 
 
-def test_laziness():
+@pytest.mark.parametrize("src_transposed", (False, True))
+@pytest.mark.parametrize("tgt_transposed", (False, True))
+def test_laziness(src_transposed, tgt_transposed):
     """Test that regridding is lazy when source data is lazy."""
     n_lons = 12
     n_lats = 10
     h = 4
     lon_bounds = (-180, 180)
     lat_bounds = (-90, 90)
 
@@ -167,21 +170,31 @@
     src_data = np.arange(n_lats * n_lons * h).reshape([n_lats, n_lons, h])
     src_data = da.from_array(src_data, chunks=[3, 5, 1])
     src = Cube(src_data)
     src.add_dim_coord(grid.coord("latitude"), 0)
     src.add_dim_coord(grid.coord("longitude"), 1)
     tgt = _grid_cube(n_lons, n_lats, lon_bounds, lat_bounds, circular=True)
 
+    # Transpose the data to ensure all possible combinations of dimension
+    # ordering are covered.
+    if src_transposed:
+        src.transpose()
+        src_data = src_data.T
+    if tgt_transposed:
+        tgt.transpose()
+
     assert src.has_lazy_data()
     result = regrid_rectilinear_to_rectilinear(src, tgt)
     assert result.has_lazy_data()
     assert np.allclose(result.data, src_data)
 
 
-def test_laziness_curvilinear():
+@pytest.mark.parametrize("src_transposed", (False, True))
+@pytest.mark.parametrize("tgt_transposed", (False, True))
+def test_laziness_curvilinear(src_transposed, tgt_transposed):
     """
     Test for :func:`esmf_regrid.schemes.regrid_rectilinear_to_rectilinear`.
 
     Tests the handling of lazy data. Ensures that handling is the same
     for non-lazy data.
     """
     h = 2
@@ -224,14 +237,22 @@
     src_cube.add_aux_coord(src_grid.coord("latitude"), (1, 3))
     src_cube.add_dim_coord(time, 2)
     src_cube.add_aux_coord(src_grid.coord("longitude"), (1, 3))
     src_cube.add_aux_coord(extra, 4)
 
     src_cube_lazy = src_cube.copy(src_data_lazy)
 
+    # Transpose the data to ensure all possible combinations of dimension
+    # ordering are covered.
+    if src_transposed:
+        src_cube_lazy.transpose()
+        src_cube.transpose()
+    if tgt_transposed:
+        tgt_grid.transpose()
+
     result = regrid_rectilinear_to_rectilinear(src_cube, tgt_grid)
     result_lazy = regrid_rectilinear_to_rectilinear(src_cube_lazy, tgt_grid)
 
     assert result_lazy.has_lazy_data()
 
     assert result_lazy == result
```

### Comparing `esmf_regrid-0.6.0/esmf_regrid.egg-info/SOURCES.txt` & `esmf_regrid-0.7.0/esmf_regrid.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+CHANGELOG.md
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
-setup.cfg
 setup.py
 esmf_regrid/__init__.py
 esmf_regrid/_esmf_sdo.py
 esmf_regrid/esmf_regridder.py
 esmf_regrid/schemes.py
 esmf_regrid.egg-info/PKG-INFO
 esmf_regrid.egg-info/SOURCES.txt
@@ -20,14 +21,16 @@
 esmf_regrid/tests/__init__.py
 esmf_regrid/tests/integration/__init__.py
 esmf_regrid/tests/integration/esmf_regridder/__init__.py
 esmf_regrid/tests/integration/esmf_regridder/test_Regridder.py
 esmf_regrid/tests/integration/experimental/__init__.py
 esmf_regrid/tests/integration/experimental/unstructured_scheme/__init__.py
 esmf_regrid/tests/integration/experimental/unstructured_scheme/test_regrid_unstructured_to_rectilinear.py
+esmf_regrid/tests/results/unit/_esmf_sdo/test_GridInfo/small_grid.txt
+esmf_regrid/tests/results/unit/experimental/unstructured_regrid/test_MeshInfo/small_mesh.txt
 esmf_regrid/tests/unit/__init__.py
 esmf_regrid/tests/unit/_esmf_sdo/__init__.py
 esmf_regrid/tests/unit/_esmf_sdo/test_GridInfo.py
 esmf_regrid/tests/unit/_esmf_sdo/test_RefinedGridInfo.py
 esmf_regrid/tests/unit/esmf_regridder/__init__.py
 esmf_regrid/tests/unit/esmf_regridder/test_Regridder.py
 esmf_regrid/tests/unit/experimental/__init__.py
@@ -35,18 +38,25 @@
 esmf_regrid/tests/unit/experimental/io/test_round_tripping.py
 esmf_regrid/tests/unit/experimental/io/test_save_regridder.py
 esmf_regrid/tests/unit/experimental/unstructured_regrid/__init__.py
 esmf_regrid/tests/unit/experimental/unstructured_regrid/test_MeshInfo.py
 esmf_regrid/tests/unit/experimental/unstructured_scheme/__init__.py
 esmf_regrid/tests/unit/experimental/unstructured_scheme/test_GridToMeshESMFRegridder.py
 esmf_regrid/tests/unit/experimental/unstructured_scheme/test_MeshToGridESMFRegridder.py
-esmf_regrid/tests/unit/experimental/unstructured_scheme/test__create_cube.py
-esmf_regrid/tests/unit/experimental/unstructured_scheme/test__cube_to_GridInfo.py
-esmf_regrid/tests/unit/experimental/unstructured_scheme/test__mesh_to_MeshInfo.py
-esmf_regrid/tests/unit/experimental/unstructured_scheme/test__regrid_unstructured_to_rectilinear__prepare.py
 esmf_regrid/tests/unit/experimental/unstructured_scheme/test_regrid_rectilinear_to_unstructured.py
 esmf_regrid/tests/unit/experimental/unstructured_scheme/test_regrid_unstructured_to_rectilinear.py
 esmf_regrid/tests/unit/schemes/__init__.py
 esmf_regrid/tests/unit/schemes/test_ESMFAreaWeighted.py
 esmf_regrid/tests/unit/schemes/test_ESMFAreaWeightedRegridder.py
+esmf_regrid/tests/unit/schemes/test_ESMFBilinear.py
+esmf_regrid/tests/unit/schemes/test_ESMFBilinearRegridder.py
+esmf_regrid/tests/unit/schemes/test_ESMFNearest.py
+esmf_regrid/tests/unit/schemes/test_ESMFNearestRegridder.py
+esmf_regrid/tests/unit/schemes/test__ESMFRegridder.py
+esmf_regrid/tests/unit/schemes/test__create_cube.py
 esmf_regrid/tests/unit/schemes/test__cube_to_GridInfo.py
-esmf_regrid/tests/unit/schemes/test_regrid_rectilinear_to_rectilinear.py
+esmf_regrid/tests/unit/schemes/test__mesh_to_MeshInfo.py
+esmf_regrid/tests/unit/schemes/test__regrid_unstructured_to_rectilinear__prepare.py
+esmf_regrid/tests/unit/schemes/test_regrid_rectilinear_to_rectilinear.py
+requirements/core.txt
+requirements/optional-dev.txt
+requirements/optional-docs.txt
```

