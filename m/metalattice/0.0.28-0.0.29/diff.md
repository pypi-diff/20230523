# Comparing `tmp/metalattice-0.0.28.tar.gz` & `tmp/metalattice-0.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metalattice-0.0.28.tar", last modified: Mon May 22 07:53:37 2023, max compression
+gzip compressed data, was "metalattice-0.0.29.tar", last modified: Tue May 23 03:25:32 2023, max compression
```

## Comparing `metalattice-0.0.28.tar` & `metalattice-0.0.29.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:53:37.016553 metalattice-0.0.28/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:53:37.012553 metalattice-0.0.28/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:53:37.012553 metalattice-0.0.28/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-22 07:53:23.000000 metalattice-0.0.28/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-22 07:53:23.000000 metalattice-0.0.28/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11071 2023-05-22 07:53:23.000000 metalattice-0.0.28/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-22 07:53:23.000000 metalattice-0.0.28/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-22 07:53:37.016553 metalattice-0.0.28/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-22 07:53:23.000000 metalattice-0.0.28/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-22 07:53:23.000000 metalattice-0.0.28/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 07:53:37.016553 metalattice-0.0.28/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:53:37.012553 metalattice-0.0.28/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:53:37.012553 metalattice-0.0.28/src/metalattice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-22 07:53:36.000000 metalattice-0.0.28/src/metalattice/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:53:37.012553 metalattice-0.0.28/src/metalattice/abaqus/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/abaqus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:53:37.016553 metalattice-0.0.28/src/metalattice/abaqus/fortran/
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/abaqus/fortran/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:53:37.016553 metalattice-0.0.28/src/metalattice/abaqus/fortran/code/
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/abaqus/fortran/code/custom_lattice.f
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/abaqus/fortran/code/cylin_lattice.f
--rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/abaqus/fortran/code/kshape20h.f
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/abaqus/fortran/code/kshape8h.f
--rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/abaqus/fortran/code/lattice.f
--rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/abaqus/fortran/code/mpc3d.f
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/abaqus/fortran/code/namelist_element.f
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/abaqus/fortran/code/namelist_info.f
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/abaqus/fortran/code/rect_lattice.f
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/abaqus/fortran/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:53:37.016553 metalattice-0.0.28/src/metalattice/abaqus/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/abaqus/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/abaqus/scripts/generate_beam_inp.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/abaqus/step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:53:37.016553 metalattice-0.0.28/src/metalattice/lattice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/lattice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13885 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/lattice/lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-22 07:53:23.000000 metalattice-0.0.28/src/metalattice/material.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:53:37.012553 metalattice-0.0.28/src/metalattice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-22 07:53:36.000000 metalattice-0.0.28/src/metalattice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-22 07:53:37.000000 metalattice-0.0.28/src/metalattice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 07:53:36.000000 metalattice-0.0.28/src/metalattice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-22 07:53:36.000000 metalattice-0.0.28/src/metalattice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 07:53:36.000000 metalattice-0.0.28/src/metalattice.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:53:37.016553 metalattice-0.0.28/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 07:53:23.000000 metalattice-0.0.28/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-22 07:53:23.000000 metalattice-0.0.28/tests/test_lattice_defination.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-22 07:53:23.000000 metalattice-0.0.28/tests/test_math_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-22 07:53:23.000000 metalattice-0.0.28/tests/test_output_to_abaqus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:32.441363 metalattice-0.0.29/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:32.433363 metalattice-0.0.29/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:32.437363 metalattice-0.0.29/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-23 03:25:17.000000 metalattice-0.0.29/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-23 03:25:17.000000 metalattice-0.0.29/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11124 2023-05-23 03:25:17.000000 metalattice-0.0.29/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-23 03:25:17.000000 metalattice-0.0.29/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-23 03:25:32.441363 metalattice-0.0.29/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-23 03:25:17.000000 metalattice-0.0.29/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-23 03:25:17.000000 metalattice-0.0.29/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 03:25:32.441363 metalattice-0.0.29/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:32.433363 metalattice-0.0.29/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:32.437363 metalattice-0.0.29/src/metalattice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:17.000000 metalattice-0.0.29/src/metalattice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-23 03:25:32.000000 metalattice-0.0.29/src/metalattice/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:32.437363 metalattice-0.0.29/src/metalattice/abaqus/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-23 03:25:17.000000 metalattice-0.0.29/src/metalattice/abaqus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:32.437363 metalattice-0.0.29/src/metalattice/abaqus/fortran/
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-23 03:25:17.000000 metalattice-0.0.29/src/metalattice/abaqus/fortran/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:32.437363 metalattice-0.0.29/src/metalattice/abaqus/fortran/code/
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-05-23 03:25:17.000000 metalattice-0.0.29/src/metalattice/abaqus/fortran/code/cylin_lattice.f
+-rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-05-23 03:25:17.000000 metalattice-0.0.29/src/metalattice/abaqus/fortran/code/kshape20h.f
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-05-23 03:25:17.000000 metalattice-0.0.29/src/metalattice/abaqus/fortran/code/kshape8h.f
+-rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-05-23 03:25:17.000000 metalattice-0.0.29/src/metalattice/abaqus/fortran/code/lattice.f
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-05-23 03:25:17.000000 metalattice-0.0.29/src/metalattice/abaqus/fortran/code/mpc3d.f
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-23 03:25:17.000000 metalattice-0.0.29/src/metalattice/abaqus/fortran/code/namelist_element.f
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-23 03:25:17.000000 metalattice-0.0.29/src/metalattice/abaqus/fortran/code/namelist_info.f
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-23 03:25:17.000000 metalattice-0.0.29/src/metalattice/abaqus/fortran/code/rect_lattice.f
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:17.000000 metalattice-0.0.29/src/metalattice/abaqus/fortran/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:32.437363 metalattice-0.0.29/src/metalattice/abaqus/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-23 03:25:17.000000 metalattice-0.0.29/src/metalattice/abaqus/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-05-23 03:25:17.000000 metalattice-0.0.29/src/metalattice/abaqus/scripts/generate_beam_inp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-23 03:25:17.000000 metalattice-0.0.29/src/metalattice/abaqus/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-05-23 03:25:17.000000 metalattice-0.0.29/src/metalattice/abaqus/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:32.437363 metalattice-0.0.29/src/metalattice/lattice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:17.000000 metalattice-0.0.29/src/metalattice/lattice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15602 2023-05-23 03:25:17.000000 metalattice-0.0.29/src/metalattice/lattice/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-23 03:25:17.000000 metalattice-0.0.29/src/metalattice/material.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:32.437363 metalattice-0.0.29/src/metalattice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-23 03:25:32.000000 metalattice-0.0.29/src/metalattice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-23 03:25:32.000000 metalattice-0.0.29/src/metalattice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 03:25:32.000000 metalattice-0.0.29/src/metalattice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-23 03:25:32.000000 metalattice-0.0.29/src/metalattice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 03:25:32.000000 metalattice-0.0.29/src/metalattice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:32.441363 metalattice-0.0.29/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:17.000000 metalattice-0.0.29/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-23 03:25:17.000000 metalattice-0.0.29/tests/test_lattice_defination.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-23 03:25:17.000000 metalattice-0.0.29/tests/test_math_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-23 03:25:17.000000 metalattice-0.0.29/tests/test_output_to_abaqus.py
```

### Comparing `metalattice-0.0.28/.github/workflows/python-package.yml` & `metalattice-0.0.29/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `metalattice-0.0.28/.github/workflows/python-publish.yml` & `metalattice-0.0.29/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `metalattice-0.0.28/.gitignore` & `metalattice-0.0.29/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -616,7 +616,8 @@
 ### VisualStudio Patch ###
 # Additional files built by Visual Studio
 
 # End of https://www.toptal.com/developers/gitignore/api/python,fortran,visualstudio,visualstudiocode
 src/metalattice/_version.py
 *.metalattice.*
 *.inp
+src/metalattice/abaqus/fortran/code/custom_lattice.f
```

### Comparing `metalattice-0.0.28/LICENSE` & `metalattice-0.0.29/LICENSE`

 * *Files identical despite different names*

### Comparing `metalattice-0.0.28/PKG-INFO` & `metalattice-0.0.29/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalattice
-Version: 0.0.28
+Version: 0.0.29
 Summary: A Python package to model lattice metamaterials, using Abaqus.
 Author-email: Huang Lihao <huang-lihao@outlook.com>
 Maintainer-email: Huang Lihao <huang-lihao@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 HUANG Lihao (huang-lihao)
```

### Comparing `metalattice-0.0.28/pyproject.toml` & `metalattice-0.0.29/pyproject.toml`

 * *Files identical despite different names*

### Comparing `metalattice-0.0.28/src/metalattice/abaqus/fortran/__init__.py` & `metalattice-0.0.29/src/metalattice/abaqus/fortran/__init__.py`

 * *Files identical despite different names*

### Comparing `metalattice-0.0.28/src/metalattice/abaqus/fortran/code/custom_lattice.f` & `metalattice-0.0.29/src/metalattice/abaqus/fortran/code/rect_lattice.f`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
         k1=ijk1(3)
         i2=ijk2(1)
         j2=ijk2(2)
         k2=ijk2(3)
         
         b%coord(:,1)=coord_of_idx(i1,j1,k1)
         b%coord(:,2)=coord_of_idx(i2,j2,k2)
-        b%indices(:,1)=modulo(nint([i1,j1,k1])-1, npps)+1
-        b%indices(:,2)=modulo(nint([i2,j2,k2])-1, npps)+1
+        b%indices(:,1)=modulo(nint([i1,j1,k1]), npps)
+        b%indices(:,2)=modulo(nint([i2,j2,k2]), npps)
         
         b%T(:,2)=(/1.d0,2.d0,3.d0/)                       ! editable: y direction of beam cross section
         call calc_T(b)
         
         b%section=S_CIRC                                  ! editable: shape of beam cross section
         allocate(b%geom(1))                               ! editable: len of geom of beam cross section
         b%geom(1)=b%L*0.1d0                               ! editable: geom of beam cross section
```

### Comparing `metalattice-0.0.28/src/metalattice/abaqus/fortran/code/cylin_lattice.f` & `metalattice-0.0.29/src/metalattice/abaqus/fortran/code/cylin_lattice.f`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,16 @@
         k1=ijk1(3)
         i2=ijk2(1)
         j2=ijk2(2)
         k2=ijk2(3)
         
         b%coord(:,1)=coord_of_idx(i1,j1,k1)
         b%coord(:,2)=coord_of_idx(i2,j2,k2)
-        b%indices(:,1)=modulo(nint([i1,j1,k1])-1, npps)+1
-        b%indices(:,2)=modulo(nint([i2,j2,k2])-1, npps)+1
+        b%indices(:,1)=modulo(nint([i1,j1,k1]), npps)
+        b%indices(:,2)=modulo(nint([i2,j2,k2]), npps)
         
         b%T(:,2)=(/1.d0,2.d0,3.d0/)                       ! editable: y direction of beam cross section
         call calc_T(b)
         
         b%section=S_CIRC                                  ! editable: shape of beam cross section
         allocate(b%geom(1))                               ! editable: len of geom of beam cross section
         b%geom(1)=b%L*0.1d0                               ! editable: geom of beam cross section
```

### Comparing `metalattice-0.0.28/src/metalattice/abaqus/fortran/code/kshape20h.f` & `metalattice-0.0.29/src/metalattice/abaqus/fortran/code/kshape20h.f`

 * *Files identical despite different names*

### Comparing `metalattice-0.0.28/src/metalattice/abaqus/fortran/code/kshape8h.f` & `metalattice-0.0.29/src/metalattice/abaqus/fortran/code/kshape8h.f`

 * *Files identical despite different names*

### Comparing `metalattice-0.0.28/src/metalattice/abaqus/fortran/code/lattice.f` & `metalattice-0.0.29/src/metalattice/abaqus/fortran/code/lattice.f`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
                                   !   Geometric input data: Radius
           enumerator S_HEX        ! for a hollow hexagonal section.
           enumerator S_I          ! for an I-beam section.
           enumerator S_L          ! for an L-beam section.
           enumerator S_PIPE       ! for a thin-walled circular section.
           enumerator S_RECT       ! for a solid, rectangular section.
                                   !   Geometric input data: a, b
-          enumerator S_THICK PIPE ! for a thick-walled circular section (Abaqus/Standard only).
+          enumerator S_THICK_PIPE ! for a thick-walled circular section (Abaqus/Standard only).
           enumerator S_TRAPEZOID  ! for a trapezoidal section.
         end enum
 
         enum, bind(c)           ! beam element type
           enumerator B31
           enumerator B33
         end enum
```

### Comparing `metalattice-0.0.28/src/metalattice/abaqus/fortran/code/mpc3d.f` & `metalattice-0.0.29/src/metalattice/abaqus/fortran/code/mpc3d.f`

 * *Files identical despite different names*

### Comparing `metalattice-0.0.28/src/metalattice/abaqus/scripts/generate_beam_inp.py` & `metalattice-0.0.29/src/metalattice/abaqus/scripts/generate_beam_inp.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # -*- coding: mbcs -*-
 # Do not delete the following import lines
 from abaqus import *
 from abaqusConstants import *
 import __main__
 
 from multiprocessing import cpu_count
-
+import numpy as np
 
 def generate_inp(
     job_name,
     model_name,
     geom_inp,
-    E = 200E3,
-    nu = 0.3,
-    rho = 7.7E-9,
+    E=200E3,
+    nu=0.3,
+    rho=7.7E-9,
+    step_name="static",
 ):
     import section
     import regionToolset
     import displayGroupMdbToolset as dgm
     import part
     import material
     import assembly
@@ -33,48 +34,56 @@
     import displayGroupOdbToolset as dgo
     import connectorBehavior
 
     model_obj = mdb.ModelFromInputFile(name=model_name, inputFileName=geom_inp)
     model_obj.setValues(noPartsInputFile=ON)
 
     part_obj = model_obj.parts.values()[-1]
-    instance_obj = model_obj.rootAssembly.Instance(
-        name=part_obj.name + "-1",
-        part=part_obj,
-        dependent=ON
-    )
 
     material_obj = model_obj.Material(name='Material-1')
     material_obj.Elastic(table=((E, nu), ))
     material_obj.Density(table=((rho, ), ))
 
-    profile_obj = model_obj.CircularProfile(name='Profile-1', r=0.1)
-    section_obj = model_obj.BeamSection(
-        name='Section-1',
-        integration=DURING_ANALYSIS,
-        profile=profile_obj.name,
-        material=material_obj.name,
-        consistentMassMatrix=False,
-    )
-
-    e = part_obj.elements
-    region = regionToolset.Region(elements=e)
-    part_obj.SectionAssignment(
-        region=region,
-        sectionName='Section-1',
-        offset=0.0,
-        offsetType=MIDDLE_SURFACE,
-        offsetField='',
-        thicknessAssignment=FROM_SECTION
-    )
-    part_obj.assignBeamSectionOrientation(
-        region=region,
-        method=N1_COSINES,
-        n1=(0.0, 0.0, 1.0)
-    )
+    for key, value in model_obj.rootAssembly.sets.items():
+        if "BEAM" not in key: continue
+        beam = value.elements[0]
+        coords = [
+            np.array(n.coordinates)
+            for n in beam.getNodes()
+        ]
+        e1 = coords[1] - coords[0]
+        L = np.linalg.norm(e1)
+        e1 = e1 / L
+        profile_obj = model_obj.CircularProfile(name='Profile'+key[4:], r=0.1*L)
+        section_obj = model_obj.BeamSection(
+            name='Section'+key[4:],
+            integration=DURING_ANALYSIS,
+            profile=profile_obj.name,
+            material=material_obj.name,
+            consistentMassMatrix=False,
+        )
+
+        region = regionToolset.Region(elements=part_obj.elements.sequenceFromLabels([beam.label]))
+        
+        part_obj.SectionAssignment(
+            region=region,
+            sectionName=section_obj.name,
+        )
+
+        part_obj.assignBeamSectionOrientation(
+            region=region,
+            method=N1_COSINES,
+            n1=(0.0, 0.0, 1.0)
+        )
+
+    if step_name == "static":
+        model_obj.StaticStep(
+            name='Step-1',
+            previous='Initial',
+        )
 
     if int(version)>2020:
         this_job = mdb.Job(
             name=job_name,
             model=model_name,
             numCpus=cpu_count()/2,
             numDomains=cpu_count()/2,
@@ -125,17 +134,22 @@
         type=float,
     )
     parser.add_argument(
         "rho",
         default=7.7e-9,
         type=float,
     )
-    args = parser.parse_args(sys.argv[-6:])
-    print(args)
+    parser.add_argument(
+        "step_name",
+        default="static",
+        type=str,
+    )
+    args = parser.parse_args(sys.argv[-(len(parser._actions) - 1):])
     generate_inp(
         job_name=args.job_name,
         model_name=args.model_name,
         geom_inp=args.geom_inp,
         E=args.E,
         nu=args.nu,
         rho=args.rho,
+        step_name=args.step_name
     )
```

### Comparing `metalattice-0.0.28/src/metalattice/lattice/lattice.py` & `metalattice-0.0.29/src/metalattice/lattice/lattice.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,28 @@
 from numpy.typing import ArrayLike
 from shutil import copyfile
 
 from metalattice.material import Material
 from metalattice.abaqus import fortran
 from metalattice.abaqus.fortran import compile_fortran
 from metalattice.abaqus.fortran import lib
-from metalattice.abaqus.scripts import run_abaqus_script
+from metalattice.abaqus.writer import AbaqusInpWriter
+
+cross_section = {
+    lib.lattice.s_arbitrary:"ARBITRARY",
+    lib.lattice.s_box:"BOX",
+    lib.lattice.s_circ:"CIRC",
+    lib.lattice.s_hex:"HEX",
+    lib.lattice.s_i:"I",
+    lib.lattice.s_l:"L",
+    lib.lattice.s_pipe:"PIPE",
+    lib.lattice.s_rect:"RECT",
+    lib.lattice.s_thick_pipe:"THICK PIPE",
+    lib.lattice.s_trapezoid:"TRAPEZOID",
+}
 
 
 class Lattice:
     def __init__(
         self,
         ns: list[int],
         strides: list[int] = [1, 1, 1],
@@ -89,18 +102,18 @@
             return
         self.beams = {}
         for i in range(cell_ns[0]):
             for j in range(cell_ns[1]):
                 for k in range(cell_ns[2]):
                     beams = self.beams_inside_cube(i, j, k)
                     for beam in beams:
-                        key = tuple([
+                        key = (
                             tuple(beam["indices"][:, 0].tolist()),
                             tuple(beam["indices"][:, 1].tolist()),
-                        ])
+                        )
                         if key not in self.beams:
                             self.beams[key] = beam
 
     def genertate_continuum_mesh(
         self,
         element_type: str = "MPC3D8",
         regenerate: bool = False,
@@ -307,15 +320,15 @@
 
         conn = []
         ijk_list = list(self.nodes.keys())
         for beam in self.beams.values():
             conn.append(
                 [
                     ijk_list.index(tuple([
-                        (ijk[d] - 1) % node_ns[d]
+                        ijk[d] % node_ns[d]
                         for d in range(3)
                     ]))
                     for ijk in beam["indices"].T
                 ]
             )
 
         element_type = beam["element"]
@@ -334,36 +347,79 @@
 
         point_sets: dict[str, ArrayLike] = {}
         sign = {0: "-", 1: "+"}
         for d in range(3):
             if not self.periodic[d]:
                 for pn in range(2):
                     indices = [
-                        [i for i in range(0, node_ns[j])]
-                        for j in range(3)
+                        np.arange(node_ns[i])
+                        for i in range(3)
                     ]
-                    indices[d] = [pn * node_ns[d]]
+                    indices[d] = [pn * (node_ns[d] - 1)]
                     point_sets[f"SURFACE-{d}{sign[pn]}"] = [
-                        ijk_list.index(tuple(i, j, k))
-                        for i in range(0, node_ns[0])
-                        for j in range(0, node_ns[1])
-                        for k in range(0, node_ns[2])
+                        ijk_list.index((i, j, k))
+                        for i in indices[0]
+                        for j in indices[1]
+                        for k in indices[2]
                     ]
+        
+        cell_sets: dict[str, ArrayLike] = {}
+        beam_keys = list(self.beams.keys())
+        for k in self.beams.keys():
+            kw = [
+                f"({k[i][0]}-{k[i][1]}-{k[i][2]})"
+                for i in range(2)
+            ]
+            cell_sets[f"BEAM-{kw[0]}-{kw[1]}"] = [np.array([beam_keys.index(k)])]
 
         meshio.write_points_cells(
             filename=inp_file_name,
             points=points,
             cells=cells,
             point_sets=point_sets,
+            cell_sets=cell_sets,
         )
 
-        run_abaqus_script(
-            script_file="generate_beam_inp",
-            option=f"main_{job_name} main_{job_name} {inp_file_name} {self.material.E} {self.material.nu} {self.material.rho}"
+        writer = AbaqusInpWriter(inp_file_name=inp_file_name)
+
+        for k, beam in self.beams.items():
+            kw = [
+                f"({k[i][0]}-{k[i][1]}-{k[i][2]})"
+                for i in range(2)
+            ]
+            writer.write_sections({
+                f"BEAM-{kw[0]}-{kw[1]}":{
+                    "elset": f"BEAM-{kw[0]}-{kw[1]}",
+                    "material": self.material.name,
+                    "section": cross_section[beam["section"]],
+                    "lumped": "YES" if beam["lumped"] else "NO",
+                    "geom": [str(g) for g in beam["geom"]],
+                    "n1": [str(n) for n in beam["t"][1,:]],
+                }
+            })
+
+        writer.write_material(self.material)
+        writer.write_step(
+            step={
+                "name": "Step-1",
+                "type": "Static",
+                "BCs": {
+                    "BC-1":{
+                        "type": "Boundary",
+                        "data": ["SURFACE-0-,1,6"],
+                    },
+                    "BC-2":{
+                        "type": "Boundary",
+                        "data": ["SURFACE-0+,2,2,1.0"],
+                    }
+                },
+                "loads": {},
+            },
         )
+        writer.close()
 
     def write_micropolar_job(
         self,
         job_name: str,
         element_type: str = "MPC3D8",
         regenerate: bool = False,
     ):
```

### Comparing `metalattice-0.0.28/src/metalattice.egg-info/PKG-INFO` & `metalattice-0.0.29/src/metalattice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalattice
-Version: 0.0.28
+Version: 0.0.29
 Summary: A Python package to model lattice metamaterials, using Abaqus.
 Author-email: Huang Lihao <huang-lihao@outlook.com>
 Maintainer-email: Huang Lihao <huang-lihao@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 HUANG Lihao (huang-lihao)
```

### Comparing `metalattice-0.0.28/src/metalattice.egg-info/SOURCES.txt` & `metalattice-0.0.29/src/metalattice.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 src/metalattice.egg-info/PKG-INFO
 src/metalattice.egg-info/SOURCES.txt
 src/metalattice.egg-info/dependency_links.txt
 src/metalattice.egg-info/requires.txt
 src/metalattice.egg-info/top_level.txt
 src/metalattice/abaqus/__init__.py
 src/metalattice/abaqus/step.py
+src/metalattice/abaqus/writer.py
 src/metalattice/abaqus/fortran/__init__.py
 src/metalattice/abaqus/fortran/lib.py
-src/metalattice/abaqus/fortran/code/custom_lattice.f
 src/metalattice/abaqus/fortran/code/cylin_lattice.f
 src/metalattice/abaqus/fortran/code/kshape20h.f
 src/metalattice/abaqus/fortran/code/kshape8h.f
 src/metalattice/abaqus/fortran/code/lattice.f
 src/metalattice/abaqus/fortran/code/mpc3d.f
 src/metalattice/abaqus/fortran/code/namelist_element.f
 src/metalattice/abaqus/fortran/code/namelist_info.f
```

### Comparing `metalattice-0.0.28/tests/test_lattice_defination.py` & `metalattice-0.0.29/tests/test_lattice_defination.py`

 * *Files identical despite different names*

### Comparing `metalattice-0.0.28/tests/test_math_constants.py` & `metalattice-0.0.29/tests/test_math_constants.py`

 * *Files identical despite different names*

### Comparing `metalattice-0.0.28/tests/test_output_to_abaqus.py` & `metalattice-0.0.29/tests/test_output_to_abaqus.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         )
         la.write_micropolar_job(
             job_name="test_rect__micropolar_mpc3d8",
             element_type="MPC3D8",
             regenerate=True,
         )
         la.write_micropolar_job(
-            job_name="testt_rect_micropolar_mpc3d20",
+            job_name="test_rect_micropolar_mpc3d20",
             element_type="MPC3D20",
             regenerate=True,
         )
 
     def test_cylin_lattice(self):
         from metalattice.lattice.lattice import Lattice
```

