# Comparing `tmp/scikit-rt-0.4.7.tar.gz` & `tmp/scikit-rt-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-rt-0.4.7.tar", last modified: Mon May 22 09:23:11 2023, max compression
+gzip compressed data, was "scikit-rt-0.4.8.tar", last modified: Tue May 23 18:00:02 2023, max compression
```

## Comparing `scikit-rt-0.4.7.tar` & `scikit-rt-0.4.8.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:23:11.882695 scikit-rt-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-22 09:23:11.882695 scikit-rt-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/pypi.md
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-22 09:23:11.882695 scikit-rt-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:23:11.850695 scikit-rt-0.4.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:23:11.854694 scikit-rt-0.4.7/src/scikit_rt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-22 09:23:11.000000 scikit-rt-0.4.7/src/scikit_rt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-22 09:23:11.000000 scikit-rt-0.4.7/src/scikit_rt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 09:23:11.000000 scikit-rt-0.4.7/src/scikit_rt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-22 09:23:11.000000 scikit-rt-0.4.7/src/scikit_rt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-22 09:23:11.000000 scikit-rt-0.4.7/src/scikit_rt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:23:11.862695 scikit-rt-0.4.7/src/skrt/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:23:11.866695 scikit-rt-0.4.7/src/skrt/better_viewer/
--rw-r--r--   0 runner    (1001) docker     (123)   132455 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/better_viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/better_viewer/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    73387 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:23:11.854694 scikit-rt-0.4.7/src/skrt/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:23:11.870695 scikit-rt-0.4.7/src/skrt/data/elastix_parameter_files/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1732 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/data/elastix_parameter_files/BE_BSpline05.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1801 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/data/elastix_parameter_files/MI_Affine.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1649 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/data/elastix_parameter_files/MI_BSpline05.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/data/elastix_parameter_files/MI_BSpline15.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/data/elastix_parameter_files/MI_BSpline30.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1798 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/data/elastix_parameter_files/MI_Rigid.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1804 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/data/elastix_parameter_files/MI_Translation.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:23:11.870695 scikit-rt-0.4.7/src/skrt/data/niftyreg_parameter_files/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/data/niftyreg_parameter_files/Affine.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/data/niftyreg_parameter_files/BE_BSpline05.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/data/niftyreg_parameter_files/NMI_BSpline05.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/data/niftyreg_parameter_files/NMI_BSpline15.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/data/niftyreg_parameter_files/NMI_BSpline30.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/data/niftyreg_parameter_files/Rigid.txt
--rw-r--r--   0 runner    (1001) docker     (123)    26897 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/dicom_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    39911 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/dose.py
--rw-r--r--   0 runner    (1001) docker     (123)   255921 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)   118731 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/patient.py
--rw-r--r--   0 runner    (1001) docker     (123)   134908 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)    60958 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17553 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)   352303 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:23:11.870695 scikit-rt-0.4.7/src/skrt/viewer/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   154795 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/viewer/core.py
--rw-r--r--   0 runner    (1001) docker     (123)   113136 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/src/skrt/viewer/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:23:11.882695 scikit-rt-0.4.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_01_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    15414 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_dose.py
--rw-r--r--   0 runner    (1001) docker     (123)    61981 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_patient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_qv_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_qv_quickviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_qv_struct_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_qv_struct_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_qv_structs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34152 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)    21138 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_roi_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    65888 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_synthetic_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-05-22 09:18:39.000000 scikit-rt-0.4.7/tests/test_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:00:02.087981 scikit-rt-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-23 18:00:02.087981 scikit-rt-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/pypi.md
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-23 18:00:02.091981 scikit-rt-0.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:00:02.071981 scikit-rt-0.4.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:00:02.075981 scikit-rt-0.4.8/src/scikit_rt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-23 18:00:01.000000 scikit-rt-0.4.8/src/scikit_rt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-23 18:00:02.000000 scikit-rt-0.4.8/src/scikit_rt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 18:00:01.000000 scikit-rt-0.4.8/src/scikit_rt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-23 18:00:01.000000 scikit-rt-0.4.8/src/scikit_rt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-23 18:00:01.000000 scikit-rt-0.4.8/src/scikit_rt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:00:02.079981 scikit-rt-0.4.8/src/skrt/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/src/skrt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/src/skrt/application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:00:02.079981 scikit-rt-0.4.8/src/skrt/better_viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)   132455 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/src/skrt/better_viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/src/skrt/better_viewer/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75197 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/src/skrt/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:00:02.071981 scikit-rt-0.4.8/src/skrt/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:00:02.083981 scikit-rt-0.4.8/src/skrt/data/elastix_parameter_files/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1732 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/src/skrt/data/elastix_parameter_files/BE_BSpline05.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1801 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/src/skrt/data/elastix_parameter_files/MI_Affine.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1649 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/src/skrt/data/elastix_parameter_files/MI_BSpline05.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/src/skrt/data/elastix_parameter_files/MI_BSpline15.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/src/skrt/data/elastix_parameter_files/MI_BSpline30.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1798 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/src/skrt/data/elastix_parameter_files/MI_Rigid.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1804 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/src/skrt/data/elastix_parameter_files/MI_Translation.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:00:02.083981 scikit-rt-0.4.8/src/skrt/data/niftyreg_parameter_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/src/skrt/data/niftyreg_parameter_files/Affine.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/src/skrt/data/niftyreg_parameter_files/BE_BSpline05.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/src/skrt/data/niftyreg_parameter_files/NMI_BSpline05.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/src/skrt/data/niftyreg_parameter_files/NMI_BSpline15.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/src/skrt/data/niftyreg_parameter_files/NMI_BSpline30.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/src/skrt/data/niftyreg_parameter_files/Rigid.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    26897 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/src/skrt/dicom_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39911 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/src/skrt/dose.py
+-rw-r--r--   0 runner    (1001) docker     (123)   255921 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/src/skrt/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/src/skrt/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118731 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/src/skrt/patient.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134908 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/src/skrt/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60958 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/src/skrt/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24714 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/src/skrt/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)   352303 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/src/skrt/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:00:02.083981 scikit-rt-0.4.8/src/skrt/viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/src/skrt/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   154795 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/src/skrt/viewer/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113136 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/src/skrt/viewer/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:00:02.087981 scikit-rt-0.4.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/tests/test_01_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/tests/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15414 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/tests/test_dose.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61981 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/tests/test_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/tests/test_patient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/tests/test_qv_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/tests/test_qv_quickviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/tests/test_qv_struct_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/tests/test_qv_struct_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/tests/test_qv_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34152 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/tests/test_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21138 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/tests/test_roi_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/tests/test_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/tests/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65888 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/tests/test_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/tests/test_synthetic_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-05-23 17:54:51.000000 scikit-rt-0.4.8/tests/test_viewer.py
```

### Comparing `scikit-rt-0.4.7/LICENSE` & `scikit-rt-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/PKG-INFO` & `scikit-rt-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-rt
-Version: 0.4.7
+Version: 0.4.8
 Summary: Toolkit for analysis of radiotherapy data
 Home-page: https://github.com/scikit-rt/scikit-rt
 Author: H. Pullen, K. Harrison
 Author-email: scikit-rt@hep.phy.cam.ac.uk
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/scikit-rt/scikit-rt/issues
 Description: # Scikit-rt
```

### Comparing `scikit-rt-0.4.7/README.md` & `scikit-rt-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/pypi.md` & `scikit-rt-0.4.8/pypi.md`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/setup.cfg` & `scikit-rt-0.4.8/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = scikit-rt
-version = 0.4.7
+version = 0.4.8
 author = H. Pullen, K. Harrison
 author_email = scikit-rt@hep.phy.cam.ac.uk
 description = Toolkit for analysis of radiotherapy data
 long_description = file: pypi.md
 long_description_content_type = text/markdown
 url = https://github.com/scikit-rt/scikit-rt
 project_urls =
```

### Comparing `scikit-rt-0.4.7/src/scikit_rt.egg-info/PKG-INFO` & `scikit-rt-0.4.8/src/scikit_rt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-rt
-Version: 0.4.7
+Version: 0.4.8
 Summary: Toolkit for analysis of radiotherapy data
 Home-page: https://github.com/scikit-rt/scikit-rt
 Author: H. Pullen, K. Harrison
 Author-email: scikit-rt@hep.phy.cam.ac.uk
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/scikit-rt/scikit-rt/issues
 Description: # Scikit-rt
```

### Comparing `scikit-rt-0.4.7/src/scikit_rt.egg-info/SOURCES.txt` & `scikit-rt-0.4.8/src/scikit_rt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/src/scikit_rt.egg-info/requires.txt` & `scikit-rt-0.4.8/src/scikit_rt.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/src/skrt/__init__.py` & `scikit-rt-0.4.8/src/skrt/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/src/skrt/application.py` & `scikit-rt-0.4.8/src/skrt/application.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/src/skrt/better_viewer/__init__.py` & `scikit-rt-0.4.8/src/skrt/better_viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/src/skrt/better_viewer/options.py` & `scikit-rt-0.4.8/src/skrt/better_viewer/options.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/src/skrt/core.py` & `scikit-rt-0.4.8/src/skrt/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -742,14 +742,32 @@
     def get_n_file(self):
         '''
         Return number of data files associated with this object.
         '''
         # Only 1 data file associated with a non-Archive object.
         return 1
 
+    def print_paths(self, max_path=None):
+        '''
+        Print paths of data files associated with this object.
+
+        File paths are listed in natural order, with one path per line.
+        
+        **Parameters:**
+        max_path: int/None, default=None
+            Indication of maximum number of paths to print.  If a positive
+            integer, the first <max_path> paths are printed.  If a negative
+            integer, the last <max_path> paths are printed.  If None,
+            all paths are printed.
+        '''
+        if os.path.isdir(self.path):
+            print_paths(self.path, max_path)
+        else:
+            print(self.path)
+
 
 class Dated(PathData):
     """PathData with an associated date and time, which can be used for
     sorting multiple Dateds."""
 
     def __init__(self, path: str = "", auto_timestamp=False):
         """
@@ -2167,7 +2185,42 @@
 
     cls : class
         Class for which qualified name is to be determined.  If non-class
         is passed as argument, None is returned.
     """
     if isinstance(cls, type):
         return f"{cls.__module__}.{cls.__name__}"
+
+
+def print_paths(data_dir, max_path=None):
+    """
+    Print paths to files below a directory, ignoring hidden files.
+    
+    File paths are listed in natural order, with one path per line.
+    
+    **Parameters:**
+    data_dir: str, pathlib.Path
+        Path to directory below which file paths are to be printed.
+        
+    max_path: int/None, default=None
+        Indication of maximum number of paths to print.  If a positive
+        integer, the first <max_path> paths are printed.  If a negative
+        integer, the last <max_path> paths are printed.  If None,
+        all paths are printed.
+    """
+    # Obtain sorted list of paths.
+    local_paths = sorted(
+            list(Path(data_dir).glob("**/[!.]*")), key=alphanumeric)
+
+    # Reduce number of paths as needed.
+    if max_path is None:
+        selected_paths = local_paths
+    else:
+        if max_path >= 0:
+            selected_paths = local_paths[: max_path]
+        else:
+            selected_paths = local_paths[max_path:]
+
+    # Print paths.
+    for path in selected_paths:
+        out_path = compress_user(path) if Defaults().compress_user else path
+        print(out_path)
```

### Comparing `scikit-rt-0.4.7/src/skrt/data/elastix_parameter_files/BE_BSpline05.txt` & `scikit-rt-0.4.8/src/skrt/data/elastix_parameter_files/BE_BSpline05.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/src/skrt/data/elastix_parameter_files/MI_Affine.txt` & `scikit-rt-0.4.8/src/skrt/data/elastix_parameter_files/MI_Affine.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/src/skrt/data/elastix_parameter_files/MI_BSpline05.txt` & `scikit-rt-0.4.8/src/skrt/data/elastix_parameter_files/MI_BSpline05.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/src/skrt/data/elastix_parameter_files/MI_BSpline15.txt` & `scikit-rt-0.4.8/src/skrt/data/elastix_parameter_files/MI_BSpline15.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/src/skrt/data/elastix_parameter_files/MI_BSpline30.txt` & `scikit-rt-0.4.8/src/skrt/data/elastix_parameter_files/MI_BSpline30.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/src/skrt/data/elastix_parameter_files/MI_Rigid.txt` & `scikit-rt-0.4.8/src/skrt/data/elastix_parameter_files/MI_Rigid.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/src/skrt/data/elastix_parameter_files/MI_Translation.txt` & `scikit-rt-0.4.8/src/skrt/data/elastix_parameter_files/MI_Translation.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/src/skrt/dicom_writer.py` & `scikit-rt-0.4.8/src/skrt/dicom_writer.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/src/skrt/dose.py` & `scikit-rt-0.4.8/src/skrt/dose.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/src/skrt/image.py` & `scikit-rt-0.4.8/src/skrt/image.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/src/skrt/multi.py` & `scikit-rt-0.4.8/src/skrt/multi.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/src/skrt/patient.py` & `scikit-rt-0.4.8/src/skrt/patient.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/src/skrt/registration.py` & `scikit-rt-0.4.8/src/skrt/registration.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/src/skrt/segmentation.py` & `scikit-rt-0.4.8/src/skrt/segmentation.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/src/skrt/structures.py` & `scikit-rt-0.4.8/src/skrt/structures.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/src/skrt/viewer/core.py` & `scikit-rt-0.4.8/src/skrt/viewer/core.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/src/skrt/viewer/viewer.py` & `scikit-rt-0.4.8/src/skrt/viewer/viewer.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/tests/test_01_setup.py` & `scikit-rt-0.4.8/tests/test_01_setup.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/tests/test_application.py` & `scikit-rt-0.4.8/tests/test_application.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/tests/test_core.py` & `scikit-rt-0.4.8/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/tests/test_dose.py` & `scikit-rt-0.4.8/tests/test_dose.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/tests/test_image.py` & `scikit-rt-0.4.8/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/tests/test_multi.py` & `scikit-rt-0.4.8/tests/test_multi.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/tests/test_patient.py` & `scikit-rt-0.4.8/tests/test_patient.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/tests/test_qv_image.py` & `scikit-rt-0.4.8/tests/test_qv_image.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/tests/test_qv_quickviewer.py` & `scikit-rt-0.4.8/tests/test_qv_quickviewer.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/tests/test_qv_struct_loader.py` & `scikit-rt-0.4.8/tests/test_qv_struct_loader.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/tests/test_qv_struct_metrics.py` & `scikit-rt-0.4.8/tests/test_qv_struct_metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/tests/test_qv_structs.py` & `scikit-rt-0.4.8/tests/test_qv_structs.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/tests/test_registration.py` & `scikit-rt-0.4.8/tests/test_registration.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/tests/test_roi_metrics.py` & `scikit-rt-0.4.8/tests/test_roi_metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/tests/test_segmentation.py` & `scikit-rt-0.4.8/tests/test_segmentation.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/tests/test_structs.py` & `scikit-rt-0.4.8/tests/test_structs.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/tests/test_synthetic_image.py` & `scikit-rt-0.4.8/tests/test_synthetic_image.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.7/tests/test_viewer.py` & `scikit-rt-0.4.8/tests/test_viewer.py`

 * *Files identical despite different names*

