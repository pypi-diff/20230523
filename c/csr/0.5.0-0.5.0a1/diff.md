# Comparing `tmp/csr-0.5.0.tar.gz` & `tmp/csr-0.5.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csr-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "csr-0.5.0a1.tar", last modified: Tue Apr 18 22:24:18 2023, max compression
```

## Comparing `csr-0.5.0.tar` & `csr-0.5.0a1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0      164 2023-05-23 21:47:03.167024 csr-0.5.0/.editorconfig
--rw-r--r--   0        0        0      223 2023-05-23 21:47:03.167024 csr-0.5.0/.gitignore
--rw-r--r--   0        0        0      147 2023-05-23 21:47:03.167024 csr-0.5.0/.readthedocs.yml
--rw-r--r--   0        0        0     1089 2023-05-23 21:47:03.167024 csr-0.5.0/LICENSE
--rw-r--r--   0        0        0      834 2023-05-23 21:47:03.167024 csr-0.5.0/README.md
--rw-r--r--   0        0        0     3358 2023-05-23 21:47:03.167024 csr-0.5.0/Timings.py
--rw-r--r--   0        0        0       59 2023-05-23 21:47:03.167024 csr-0.5.0/codecov.yml
--rw-r--r--   0        0        0     1447 2023-05-23 21:47:03.167024 csr-0.5.0/conftest.py
--rw-r--r--   0        0        0      249 2023-05-23 21:47:03.167024 csr-0.5.0/csr/__init__.py
--rw-r--r--   0        0        0     2698 2023-05-23 21:47:03.167024 csr-0.5.0/csr/_rows.py
--rw-r--r--   0        0        0     1610 2023-05-23 21:47:03.167024 csr-0.5.0/csr/_struct.py
--rw-r--r--   0        0        0      519 2023-05-23 21:47:03.167024 csr-0.5.0/csr/_util.py
--rw-r--r--   0        0        0     3287 2023-05-23 21:47:03.167024 csr-0.5.0/csr/_wiring.py
--rw-r--r--   0        0        0     1778 2023-05-23 21:47:03.167024 csr-0.5.0/csr/constructors.py
--rw-r--r--   0        0        0    22794 2023-05-23 21:47:03.167024 csr-0.5.0/csr/csr.py
--rw-r--r--   0        0        0      363 2023-05-23 21:47:03.167024 csr-0.5.0/csr/kernel.py
--rw-r--r--   0        0        0     2887 2023-05-23 21:47:03.167024 csr-0.5.0/csr/kernels/__init__.py
--rw-r--r--   0        0        0      173 2023-05-23 21:47:03.167024 csr-0.5.0/csr/kernels/mkl/__init__.py
--rw-r--r--   0        0        0      497 2023-05-23 21:47:03.167024 csr-0.5.0/csr/kernels/mkl/_api.py
--rw-r--r--   0        0        0     3424 2023-05-23 21:47:03.167024 csr-0.5.0/csr/kernels/mkl/handle.py
--rw-r--r--   0        0        0     5567 2023-05-23 21:47:03.167024 csr-0.5.0/csr/kernels/mkl/mkl_ops.c
--rw-r--r--   0        0        0     1060 2023-05-23 21:47:03.167024 csr-0.5.0/csr/kernels/mkl/mkl_ops.h
--rw-r--r--   0        0        0      733 2023-05-23 21:47:03.167024 csr-0.5.0/csr/kernels/mkl/multiply.py
--rw-r--r--   0        0        0     1265 2023-05-23 21:47:03.167024 csr-0.5.0/csr/kernels/numba/__init__.py
--rw-r--r--   0        0        0     3235 2023-05-23 21:47:03.167024 csr-0.5.0/csr/kernels/numba/multiply.py
--rw-r--r--   0        0        0      804 2023-05-23 21:47:03.167024 csr-0.5.0/csr/kernels/scipy.py
--rw-r--r--   0        0        0     6566 2023-05-23 21:47:03.167024 csr-0.5.0/csr/structure.py
--rw-r--r--   0        0        0     3500 2023-05-23 21:47:03.167024 csr-0.5.0/csr/test_utils.py
--rw-r--r--   0        0        0     2077 2023-05-23 21:47:03.167024 csr-0.5.0/csr/transform.py
--rw-r--r--   0        0        0     1089 2023-05-23 21:47:03.167024 csr-0.5.0/docs/conf.py
--rw-r--r--   0        0        0     1644 2023-05-23 21:47:03.167024 csr-0.5.0/docs/csr.rst
--rw-r--r--   0        0        0     1170 2023-05-23 21:47:03.167024 csr-0.5.0/docs/index.rst
--rw-r--r--   0        0        0     3859 2023-05-23 21:47:03.167024 csr-0.5.0/docs/kernels.rst
--rw-r--r--   0        0        0       70 2023-05-23 21:47:03.167024 csr-0.5.0/jupytext.toml
--rw-r--r--   0        0        0      155 2023-05-23 21:47:03.167024 csr-0.5.0/min-constraints.txt
--rw-r--r--   0        0        0       68 2023-05-23 21:47:03.167024 csr-0.5.0/mkl-devel.yml
--rw-r--r--   0        0        0     1290 2023-05-23 21:47:03.167024 csr-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      541 2023-05-23 21:47:03.167024 csr-0.5.0/pytest.ini
--rw-r--r--   0        0        0      198 2023-05-23 21:47:03.167024 csr-0.5.0/setup.cfg
--rw-r--r--   0        0        0     1776 2023-05-23 21:47:03.167024 csr-0.5.0/tasks.py
--rw-r--r--   0        0        0     1020 2023-05-23 21:47:03.167024 csr-0.5.0/tests/test_active_kernel.py
--rw-r--r--   0        0        0     8841 2023-05-23 21:47:03.167024 csr-0.5.0/tests/test_attributes.py
--rw-r--r--   0        0        0      411 2023-05-23 21:47:03.167024 csr-0.5.0/tests/test_bench_mult_vec.py
--rw-r--r--   0        0        0     2105 2023-05-23 21:47:03.167024 csr-0.5.0/tests/test_bench_multiply.py
--rw-r--r--   0        0        0     4908 2023-05-23 21:47:03.167024 csr-0.5.0/tests/test_convert.py
--rw-r--r--   0        0        0      445 2023-05-23 21:47:03.167024 csr-0.5.0/tests/test_handles.py
--rw-r--r--   0        0        0     3045 2023-05-23 21:47:03.167024 csr-0.5.0/tests/test_initialize.py
--rw-r--r--   0        0        0      598 2023-05-23 21:47:03.167024 csr-0.5.0/tests/test_kernel_numba.py
--rw-r--r--   0        0        0     2856 2023-05-23 21:47:03.167024 csr-0.5.0/tests/test_mkl.py
--rw-r--r--   0        0        0      900 2023-05-23 21:47:03.167024 csr-0.5.0/tests/test_mult_vec.py
--rw-r--r--   0        0        0     1938 2023-05-23 21:47:03.167024 csr-0.5.0/tests/test_multiply.py
--rw-r--r--   0        0        0     5640 2023-05-23 21:47:03.167024 csr-0.5.0/tests/test_numba.py
--rw-r--r--   0        0        0     1178 2023-05-23 21:47:03.167024 csr-0.5.0/tests/test_pickle.py
--rw-r--r--   0        0        0     5878 2023-05-23 21:47:03.167024 csr-0.5.0/tests/test_transform.py
--rw-r--r--   0        0        0     2095 2023-05-23 21:47:03.167024 csr-0.5.0/tests/test_transpose.py
--rw-r--r--   0        0        0      509 2023-05-23 21:47:03.167024 csr-0.5.0/tox.ini
--rw-r--r--   0        0        0     2363 1970-01-01 00:00:00.000000 csr-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      164 2022-02-19 17:31:58.226879 csr-0.5.0a1/.editorconfig
+-rw-r--r--   0        0        0      223 2022-02-19 17:31:58.227901 csr-0.5.0a1/.gitignore
+-rw-r--r--   0        0        0      147 2022-02-19 17:31:58.227901 csr-0.5.0a1/.readthedocs.yml
+-rw-r--r--   0        0        0     1089 2022-02-19 17:31:58.236816 csr-0.5.0a1/LICENSE
+-rw-r--r--   0        0        0      834 2022-02-19 17:31:58.245368 csr-0.5.0a1/README.md
+-rw-r--r--   0        0        0     3358 2022-02-19 17:31:58.249963 csr-0.5.0a1/Timings.py
+-rw-r--r--   0        0        0       59 2022-07-30 21:03:37.175923 csr-0.5.0a1/codecov.yml
+-rw-r--r--   0        0        0     1447 2023-04-10 23:45:09.997691 csr-0.5.0a1/conftest.py
+-rw-r--r--   0        0        0      251 2023-04-18 22:23:58.557628 csr-0.5.0a1/csr/__init__.py
+-rw-r--r--   0        0        0     2698 2023-04-18 22:23:12.666863 csr-0.5.0a1/csr/_rows.py
+-rw-r--r--   0        0        0     1610 2022-07-30 21:03:37.178089 csr-0.5.0a1/csr/_struct.py
+-rw-r--r--   0        0        0      519 2022-02-19 17:31:58.229901 csr-0.5.0a1/csr/_util.py
+-rw-r--r--   0        0        0     3287 2023-04-18 22:23:12.666863 csr-0.5.0a1/csr/_wiring.py
+-rw-r--r--   0        0        0     1778 2022-02-19 17:31:58.228901 csr-0.5.0a1/csr/constructors.py
+-rw-r--r--   0        0        0    22794 2023-04-18 22:23:12.667863 csr-0.5.0a1/csr/csr.py
+-rw-r--r--   0        0        0      363 2022-02-19 17:31:58.230402 csr-0.5.0a1/csr/kernel.py
+-rw-r--r--   0        0        0     2887 2022-02-19 17:31:58.231902 csr-0.5.0a1/csr/kernels/__init__.py
+-rw-r--r--   0        0        0      173 2022-02-19 17:31:58.232401 csr-0.5.0a1/csr/kernels/mkl/__init__.py
+-rw-r--r--   0        0        0      497 2022-02-19 17:31:58.232401 csr-0.5.0a1/csr/kernels/mkl/_api.py
+-rw-r--r--   0        0        0     3424 2022-07-30 21:03:37.178089 csr-0.5.0a1/csr/kernels/mkl/handle.py
+-rw-r--r--   0        0        0     5567 2022-02-19 17:31:58.232919 csr-0.5.0a1/csr/kernels/mkl/mkl_ops.c
+-rw-r--r--   0        0        0     1060 2022-02-19 17:31:58.232401 csr-0.5.0a1/csr/kernels/mkl/mkl_ops.h
+-rw-r--r--   0        0        0      733 2022-02-19 17:31:58.232919 csr-0.5.0a1/csr/kernels/mkl/multiply.py
+-rw-r--r--   0        0        0     1265 2022-07-30 21:03:37.179972 csr-0.5.0a1/csr/kernels/numba/__init__.py
+-rw-r--r--   0        0        0     3235 2022-02-19 17:31:58.234175 csr-0.5.0a1/csr/kernels/numba/multiply.py
+-rw-r--r--   0        0        0      804 2022-02-19 17:31:58.234175 csr-0.5.0a1/csr/kernels/scipy.py
+-rw-r--r--   0        0        0     6566 2022-02-19 17:31:58.234110 csr-0.5.0a1/csr/structure.py
+-rw-r--r--   0        0        0     3500 2022-07-30 21:03:37.180469 csr-0.5.0a1/csr/test_utils.py
+-rw-r--r--   0        0        0     2077 2022-07-30 21:03:37.180469 csr-0.5.0a1/csr/transform.py
+-rw-r--r--   0        0        0     1089 2022-02-19 17:31:58.234677 csr-0.5.0a1/docs/conf.py
+-rw-r--r--   0        0        0     1644 2022-02-19 17:31:58.235177 csr-0.5.0a1/docs/csr.rst
+-rw-r--r--   0        0        0     1170 2022-02-19 17:31:58.236320 csr-0.5.0a1/docs/index.rst
+-rw-r--r--   0        0        0     3859 2022-02-19 17:31:58.235705 csr-0.5.0a1/docs/kernels.rst
+-rw-r--r--   0        0        0       70 2022-02-19 17:31:58.236816 csr-0.5.0a1/jupytext.toml
+-rw-r--r--   0        0        0      155 2022-10-25 18:41:00.310046 csr-0.5.0a1/min-constraints.txt
+-rw-r--r--   0        0        0       68 2022-07-30 21:03:37.183531 csr-0.5.0a1/mkl-devel.yml
+-rw-r--r--   0        0        0     1304 2022-10-25 18:44:18.722422 csr-0.5.0a1/pyproject.toml
+-rw-r--r--   0        0        0      541 2022-07-30 21:03:37.184709 csr-0.5.0a1/pytest.ini
+-rw-r--r--   0        0        0      198 2022-02-19 17:31:58.246419 csr-0.5.0a1/setup.cfg
+-rw-r--r--   0        0        0     1776 2022-07-30 21:02:36.314600 csr-0.5.0a1/tasks.py
+-rw-r--r--   0        0        0     1020 2022-02-19 17:31:58.245368 csr-0.5.0a1/tests/test_active_kernel.py
+-rw-r--r--   0        0        0     8841 2023-04-18 22:23:12.668866 csr-0.5.0a1/tests/test_attributes.py
+-rw-r--r--   0        0        0      411 2022-02-19 17:31:58.246419 csr-0.5.0a1/tests/test_bench_mult_vec.py
+-rw-r--r--   0        0        0     2105 2022-02-19 17:31:58.246962 csr-0.5.0a1/tests/test_bench_multiply.py
+-rw-r--r--   0        0        0     4908 2022-07-30 21:03:37.195086 csr-0.5.0a1/tests/test_convert.py
+-rw-r--r--   0        0        0      445 2022-07-30 21:03:37.193995 csr-0.5.0a1/tests/test_handles.py
+-rw-r--r--   0        0        0     3045 2022-02-19 17:31:58.247463 csr-0.5.0a1/tests/test_initialize.py
+-rw-r--r--   0        0        0      598 2022-07-30 21:03:37.199162 csr-0.5.0a1/tests/test_kernel_numba.py
+-rw-r--r--   0        0        0     2856 2022-07-30 21:03:37.197352 csr-0.5.0a1/tests/test_mkl.py
+-rw-r--r--   0        0        0      900 2022-07-30 21:03:37.184709 csr-0.5.0a1/tests/test_mult_vec.py
+-rw-r--r--   0        0        0     1938 2022-07-30 21:03:37.200327 csr-0.5.0a1/tests/test_multiply.py
+-rw-r--r--   0        0        0     5640 2023-04-18 22:23:12.668866 csr-0.5.0a1/tests/test_numba.py
+-rw-r--r--   0        0        0     1178 2022-02-19 17:31:58.248963 csr-0.5.0a1/tests/test_pickle.py
+-rw-r--r--   0        0        0     5878 2022-07-30 21:03:37.198164 csr-0.5.0a1/tests/test_transform.py
+-rw-r--r--   0        0        0     2095 2022-07-30 21:03:37.200828 csr-0.5.0a1/tests/test_transpose.py
+-rw-r--r--   0        0        0      509 2022-02-19 17:31:58.249462 csr-0.5.0a1/tox.ini
+-rw-r--r--   0        0        0     2404 1970-01-01 00:00:00.000000 csr-0.5.0a1/PKG-INFO
```

### Comparing `csr-0.5.0/LICENSE` & `csr-0.5.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/README.md` & `csr-0.5.0a1/README.md`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/Timings.py` & `csr-0.5.0a1/Timings.py`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/conftest.py` & `csr-0.5.0a1/conftest.py`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/csr/_rows.py` & `csr-0.5.0a1/csr/_rows.py`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/csr/_struct.py` & `csr-0.5.0a1/csr/_struct.py`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/csr/_util.py` & `csr-0.5.0a1/csr/_util.py`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/csr/_wiring.py` & `csr-0.5.0a1/csr/_wiring.py`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/csr/constructors.py` & `csr-0.5.0a1/csr/constructors.py`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/csr/csr.py` & `csr-0.5.0a1/csr/csr.py`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/csr/kernels/__init__.py` & `csr-0.5.0a1/csr/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/csr/kernels/mkl/handle.py` & `csr-0.5.0a1/csr/kernels/mkl/handle.py`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/csr/kernels/mkl/mkl_ops.c` & `csr-0.5.0a1/csr/kernels/mkl/mkl_ops.c`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/csr/kernels/mkl/mkl_ops.h` & `csr-0.5.0a1/csr/kernels/mkl/mkl_ops.h`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/csr/kernels/mkl/multiply.py` & `csr-0.5.0a1/csr/kernels/mkl/multiply.py`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/csr/kernels/numba/__init__.py` & `csr-0.5.0a1/csr/kernels/numba/__init__.py`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/csr/kernels/numba/multiply.py` & `csr-0.5.0a1/csr/kernels/numba/multiply.py`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/csr/kernels/scipy.py` & `csr-0.5.0a1/csr/kernels/scipy.py`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/csr/structure.py` & `csr-0.5.0a1/csr/structure.py`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/csr/test_utils.py` & `csr-0.5.0a1/csr/test_utils.py`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/csr/transform.py` & `csr-0.5.0a1/csr/transform.py`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/docs/conf.py` & `csr-0.5.0a1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/docs/csr.rst` & `csr-0.5.0a1/docs/csr.rst`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/docs/index.rst` & `csr-0.5.0a1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/docs/kernels.rst` & `csr-0.5.0a1/docs/kernels.rst`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/pyproject.toml` & `csr-0.5.0a1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -8,44 +8,45 @@
     "License :: OSI Approved :: MIT License",
     "Intended Audience :: Science/Research",
 ]
 description = "Compressed Sparse Row matrices for Python, with Numba API."
 readme = "README.md"
 license = { file = "LICENSE" }
 dynamic = ['version']
-requires-python = ">= 3.8"
+requires-python = ">= 3.7"
 dependencies = [
-    "numba >=0.51,<0.58",
-    "numpy >=1.21",
-    "scipy >=1.4,<2"
+    "numba >=0.51,<0.57",
+    "numpy >=1.17",
+    "scipy >=1.2,<2"
 ]
 
 [[project.authors]]
 name = "Michael Ekstrand"
 email = "michaelekstrand@boisestate.edu"
 
 [project.urls]
 home-page = "https://csr.lenskit.org"
 source = "https://github.com/lenskit/csr"
 
 [project.optional-dependencies]
 test = [
-    "pytest ==7.*",
+    "pytest ==6.*",
     "pytest-doctestplus >=0.9",
     "pytest-benchmark >=3",
     "pytest-cov >=2.12",
     "hypothesis ~=6.30",
     "psutil >=5"
 ]
 dev = [
     "flit >=3.2,<4",
-    "lenskit-build-helpers >=0.3",
     "keyring",
     "flake8",
     "rstcheck",
+    "invoke",
+    "lenskit-build-helpers >=0.1",
     "sphinx-autobuild >=2021",
 ]
 doc = [
     "sphinx >=4",
     "furo"
 ]
 profile = [
```

### Comparing `csr-0.5.0/pytest.ini` & `csr-0.5.0a1/pytest.ini`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/tasks.py` & `csr-0.5.0a1/tasks.py`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/tests/test_active_kernel.py` & `csr-0.5.0a1/tests/test_active_kernel.py`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/tests/test_attributes.py` & `csr-0.5.0a1/tests/test_attributes.py`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/tests/test_bench_multiply.py` & `csr-0.5.0a1/tests/test_bench_multiply.py`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/tests/test_convert.py` & `csr-0.5.0a1/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/tests/test_initialize.py` & `csr-0.5.0a1/tests/test_initialize.py`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/tests/test_kernel_numba.py` & `csr-0.5.0a1/tests/test_kernel_numba.py`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/tests/test_mkl.py` & `csr-0.5.0a1/tests/test_mkl.py`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/tests/test_mult_vec.py` & `csr-0.5.0a1/tests/test_mult_vec.py`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/tests/test_multiply.py` & `csr-0.5.0a1/tests/test_multiply.py`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/tests/test_numba.py` & `csr-0.5.0a1/tests/test_numba.py`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/tests/test_pickle.py` & `csr-0.5.0a1/tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/tests/test_transform.py` & `csr-0.5.0a1/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/tests/test_transpose.py` & `csr-0.5.0a1/tests/test_transpose.py`

 * *Files identical despite different names*

### Comparing `csr-0.5.0/PKG-INFO` & `csr-0.5.0a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: csr
-Version: 0.5.0
+Version: 0.5.0a1
 Summary: Compressed Sparse Row matrices for Python, with Numba API.
 Author-email: Michael Ekstrand <michaelekstrand@boisestate.edu>
-Requires-Python: >= 3.8
+Requires-Python: >= 3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
-Requires-Dist: numba >=0.51,<0.58
-Requires-Dist: numpy >=1.21
-Requires-Dist: scipy >=1.4,<2
+Requires-Dist: numba >=0.51,<0.57
+Requires-Dist: numpy >=1.17
+Requires-Dist: scipy >=1.2,<2
 Requires-Dist: flit >=3.2,<4 ; extra == "dev"
-Requires-Dist: lenskit-build-helpers >=0.3 ; extra == "dev"
 Requires-Dist: keyring ; extra == "dev"
 Requires-Dist: flake8 ; extra == "dev"
 Requires-Dist: rstcheck ; extra == "dev"
+Requires-Dist: invoke ; extra == "dev"
+Requires-Dist: lenskit-build-helpers >=0.1 ; extra == "dev"
 Requires-Dist: sphinx-autobuild >=2021 ; extra == "dev"
 Requires-Dist: sphinx >=4 ; extra == "doc"
 Requires-Dist: furo ; extra == "doc"
 Requires-Dist: cffi ; extra == "mkl"
 Requires-Dist: notebook ; extra == "profile"
 Requires-Dist: seaborn ; extra == "profile"
 Requires-Dist: jupytext ; extra == "profile"
 Requires-Dist: pandas >=1.0 ; extra == "profile"
-Requires-Dist: pytest ==7.* ; extra == "test"
+Requires-Dist: pytest ==6.* ; extra == "test"
 Requires-Dist: pytest-doctestplus >=0.9 ; extra == "test"
 Requires-Dist: pytest-benchmark >=3 ; extra == "test"
 Requires-Dist: pytest-cov >=2.12 ; extra == "test"
 Requires-Dist: hypothesis ~=6.30 ; extra == "test"
 Requires-Dist: psutil >=5 ; extra == "test"
 Project-URL: home-page, https://csr.lenskit.org
 Project-URL: source, https://github.com/lenskit/csr
```

