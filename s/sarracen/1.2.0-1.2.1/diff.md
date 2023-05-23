# Comparing `tmp/sarracen-1.2.0.tar.gz` & `tmp/sarracen-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarracen-1.2.0.tar", last modified: Mon Apr 17 00:51:45 2023, max compression
+gzip compressed data, was "sarracen-1.2.1.tar", last modified: Tue May 23 17:30:14 2023, max compression
```

## Comparing `sarracen-1.2.0.tar` & `sarracen-1.2.1.tar`

### file list

```diff
@@ -1,59 +1,61 @@
--rw-r--r--   0        0        0      679 2023-04-17 00:51:11.188684 sarracen-1.2.0/.github/workflows/joss_paper.yml
--rw-r--r--   0        0        0       76 2023-04-17 00:51:11.188880 sarracen-1.2.0/.gitignore
--rw-r--r--   0        0        0      125 2023-04-17 00:51:11.189036 sarracen-1.2.0/.readthedocs.yaml
--rw-r--r--   0        0        0    35149 2023-04-17 00:51:11.189358 sarracen-1.2.0/LICENCE
--rw-r--r--   0        0        0     1445 2023-04-17 00:51:11.189538 sarracen-1.2.0/README.md
--rw-r--r--   0        0        0      634 2023-04-17 00:51:11.189715 sarracen-1.2.0/docs/Makefile
--rw-r--r--   0        0        0     1712 2023-04-17 00:51:11.189922 sarracen-1.2.0/docs/api.rst
--rw-r--r--   0        0        0     2153 2023-04-17 00:51:11.190043 sarracen-1.2.0/docs/conf.py
--rw-r--r--   0        0        0      133 2023-04-17 00:51:11.190144 sarracen-1.2.0/docs/examples.rst
--rw-r--r--   0        0        0     2310 2023-04-17 00:51:11.190323 sarracen-1.2.0/docs/examples/dustydisc.rst
--rw-r--r--   0        0        0   300231 2023-04-17 00:51:11.191988 sarracen-1.2.0/docs/examples/dustydisc/dustydisc-describe.png
--rw-r--r--   0        0        0   577154 2023-04-17 00:51:11.195266 sarracen-1.2.0/docs/examples/dustydisc/dustydisc-dust.png
--rw-r--r--   0        0        0   296363 2023-04-17 00:51:11.197124 sarracen-1.2.0/docs/examples/dustydisc/dustydisc-gas-sinks.png
--rw-r--r--   0        0        0   296269 2023-04-17 00:51:11.198908 sarracen-1.2.0/docs/examples/dustydisc/dustydisc-gas.png
--rw-r--r--   0        0        0   152484 2023-04-17 00:51:11.199956 sarracen-1.2.0/docs/examples/dustydisc/dustydisc-sdf-sinks.png
--rw-r--r--   0        0        0   506967 2023-04-17 00:51:11.202675 sarracen-1.2.0/docs/examples/dustydisc/dustydisc-sdf.png
--rw-r--r--   0        0        0    17275 2023-04-17 00:51:11.202921 sarracen-1.2.0/docs/examples/dustydisc/dustydisc-value-counts.png
--rw-r--r--   0        0        0     1121 2023-04-17 00:51:11.203063 sarracen-1.2.0/docs/examples/ot.rst
--rw-r--r--   0        0        0    18453 2023-04-17 00:51:11.203305 sarracen-1.2.0/docs/examples/ot/ot-1d.png
--rw-r--r--   0        0        0   145467 2023-04-17 00:51:11.204116 sarracen-1.2.0/docs/examples/ot/ot-describe.png
--rw-r--r--   0        0        0   178608 2023-04-17 00:51:11.205112 sarracen-1.2.0/docs/examples/ot/ot-sdf.png
--rw-r--r--   0        0        0    70378 2023-04-17 00:51:11.205587 sarracen-1.2.0/docs/examples/ot/ot-streamlines.png
--rw-r--r--   0        0        0    48370 2023-04-17 00:51:11.206005 sarracen-1.2.0/docs/examples/ot/ot.png
--rw-r--r--   0        0        0     1138 2023-04-17 00:51:11.206139 sarracen-1.2.0/docs/index.rst
--rw-r--r--   0        0        0     1648 2023-04-17 00:51:11.206243 sarracen-1.2.0/docs/installation.rst
--rw-r--r--   0        0        0      800 2023-04-17 00:51:11.206354 sarracen-1.2.0/docs/make.bat
--rw-r--r--   0        0        0    95948 2023-04-17 00:51:11.207023 sarracen-1.2.0/docs/paper/main_image.png
--rw-r--r--   0        0        0    14031 2023-04-17 00:51:11.207197 sarracen-1.2.0/docs/paper/paper.bib
--rw-r--r--   0        0        0     5953 2023-04-17 00:51:11.207327 sarracen-1.2.0/docs/paper/paper.md
--rw-r--r--   0        0        0     3484 2023-04-17 00:51:11.207450 sarracen-1.2.0/docs/quick-start.rst
--rw-r--r--   0        0        0     4814 2023-04-17 00:51:11.207605 sarracen-1.2.0/docs/render.rst
--rw-r--r--   0        0        0      527 2023-04-17 00:51:11.207721 sarracen-1.2.0/pyproject.toml
--rw-r--r--   0        0        0       75 2023-04-17 00:51:11.207809 sarracen-1.2.0/requirements.txt
--rw-r--r--   0        0        0      363 2023-04-17 00:51:11.207950 sarracen-1.2.0/sarracen/__init__.py
--rw-r--r--   0        0        0      385 2023-04-17 00:51:11.208083 sarracen-1.2.0/sarracen/interpolate/__init__.py
--rw-r--r--   0        0        0     4766 2023-04-17 00:51:11.208403 sarracen-1.2.0/sarracen/interpolate/base_backend.py
--rw-r--r--   0        0        0    24755 2023-04-17 00:51:11.208617 sarracen-1.2.0/sarracen/interpolate/cpu_backend.py
--rw-r--r--   0        0        0    27110 2023-04-17 00:51:11.208770 sarracen-1.2.0/sarracen/interpolate/gpu_backend.py
--rw-r--r--   0        0        0    55074 2023-04-17 00:51:11.209147 sarracen-1.2.0/sarracen/interpolate/interpolate.py
--rw-r--r--   0        0        0      212 2023-04-17 00:51:11.209355 sarracen-1.2.0/sarracen/kernels/__init__.py
--rw-r--r--   0        0        0     3467 2023-04-17 00:51:11.209488 sarracen-1.2.0/sarracen/kernels/base_kernel.py
--rw-r--r--   0        0        0      562 2023-04-17 00:51:11.209590 sarracen-1.2.0/sarracen/kernels/cubic_spline.py
--rw-r--r--   0        0        0    13535 2023-04-17 00:51:11.209724 sarracen-1.2.0/sarracen/kernels/cubic_spline_exact.py
--rw-r--r--   0        0        0      634 2023-04-17 00:51:11.209820 sarracen-1.2.0/sarracen/kernels/quartic_spline.py
--rw-r--r--   0        0        0      607 2023-04-17 00:51:11.209913 sarracen-1.2.0/sarracen/kernels/quintic_spline.py
--rw-r--r--   0        0        0        1 2023-04-17 00:51:11.210036 sarracen-1.2.0/sarracen/readers/__init__.py
--rw-r--r--   0        0        0      678 2023-04-17 00:51:11.210127 sarracen-1.2.0/sarracen/readers/read_csv.py
--rw-r--r--   0        0        0     8959 2023-04-17 00:51:11.210252 sarracen-1.2.0/sarracen/readers/read_marisa.py
--rw-r--r--   0        0        0     9017 2023-04-17 00:51:11.210386 sarracen-1.2.0/sarracen/readers/read_phantom.py
--rw-r--r--   0        0        0    29829 2023-04-17 00:51:11.210506 sarracen-1.2.0/sarracen/render.py
--rw-r--r--   0        0        0    19956 2023-04-17 00:51:11.210693 sarracen-1.2.0/sarracen/sarracen_dataframe.py
--rw-r--r--   0        0        0        0 2023-04-17 00:51:11.210799 sarracen-1.2.0/sarracen/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 00:51:11.210889 sarracen-1.2.0/sarracen/tests/readers/__init__.py
--rw-r--r--   0        0        0      969 2023-04-17 00:51:11.210978 sarracen-1.2.0/sarracen/tests/readers/test_read_csv.py
--rw-r--r--   0        0        0    84917 2023-04-17 00:51:11.211350 sarracen-1.2.0/sarracen/tests/test_interpolate.py
--rw-r--r--   0        0        0     8159 2023-04-17 00:51:11.211500 sarracen-1.2.0/sarracen/tests/test_kernels.py
--rw-r--r--   0        0        0    11302 2023-04-17 00:51:11.211642 sarracen-1.2.0/sarracen/tests/test_render.py
--rw-r--r--   0        0        0     5514 2023-04-17 00:51:11.211798 sarracen-1.2.0/sarracen/tests/test_sarracen_dataframe.py
--rw-r--r--   0        0        0     1907 1970-01-01 00:00:00.000000 sarracen-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      679 2023-05-23 17:25:45.049573 sarracen-1.2.1/.github/workflows/joss_paper.yml
+-rw-r--r--   0        0        0       76 2023-05-23 17:25:45.049661 sarracen-1.2.1/.gitignore
+-rw-r--r--   0        0        0      125 2023-05-23 17:25:45.049741 sarracen-1.2.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     5493 2023-05-23 17:25:45.049850 sarracen-1.2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0    35149 2023-05-23 17:25:45.050092 sarracen-1.2.1/LICENCE
+-rw-r--r--   0        0        0     2264 2023-05-23 17:25:45.050225 sarracen-1.2.1/README.md
+-rw-r--r--   0        0        0      634 2023-05-23 17:25:45.050343 sarracen-1.2.1/docs/Makefile
+-rw-r--r--   0        0        0     1712 2023-05-23 17:25:45.050440 sarracen-1.2.1/docs/api.rst
+-rw-r--r--   0        0        0     2153 2023-05-23 17:25:45.050526 sarracen-1.2.1/docs/conf.py
+-rw-r--r--   0        0        0     1173 2023-05-23 17:25:45.050624 sarracen-1.2.1/docs/contributing.rst
+-rw-r--r--   0        0        0      133 2023-05-23 17:25:45.050699 sarracen-1.2.1/docs/examples.rst
+-rw-r--r--   0        0        0     2310 2023-05-23 17:25:45.050830 sarracen-1.2.1/docs/examples/dustydisc.rst
+-rw-r--r--   0        0        0   300231 2023-05-23 17:25:45.052392 sarracen-1.2.1/docs/examples/dustydisc/dustydisc-describe.png
+-rw-r--r--   0        0        0   577154 2023-05-23 17:25:45.055494 sarracen-1.2.1/docs/examples/dustydisc/dustydisc-dust.png
+-rw-r--r--   0        0        0   296363 2023-05-23 17:25:45.057079 sarracen-1.2.1/docs/examples/dustydisc/dustydisc-gas-sinks.png
+-rw-r--r--   0        0        0   296269 2023-05-23 17:25:45.058636 sarracen-1.2.1/docs/examples/dustydisc/dustydisc-gas.png
+-rw-r--r--   0        0        0   152484 2023-05-23 17:25:45.059480 sarracen-1.2.1/docs/examples/dustydisc/dustydisc-sdf-sinks.png
+-rw-r--r--   0        0        0   506967 2023-05-23 17:25:45.062017 sarracen-1.2.1/docs/examples/dustydisc/dustydisc-sdf.png
+-rw-r--r--   0        0        0    17275 2023-05-23 17:25:45.062189 sarracen-1.2.1/docs/examples/dustydisc/dustydisc-value-counts.png
+-rw-r--r--   0        0        0     1121 2023-05-23 17:25:45.062281 sarracen-1.2.1/docs/examples/ot.rst
+-rw-r--r--   0        0        0    18453 2023-05-23 17:25:45.062464 sarracen-1.2.1/docs/examples/ot/ot-1d.png
+-rw-r--r--   0        0        0   145467 2023-05-23 17:25:45.063212 sarracen-1.2.1/docs/examples/ot/ot-describe.png
+-rw-r--r--   0        0        0   178608 2023-05-23 17:25:45.064211 sarracen-1.2.1/docs/examples/ot/ot-sdf.png
+-rw-r--r--   0        0        0    70378 2023-05-23 17:25:45.064684 sarracen-1.2.1/docs/examples/ot/ot-streamlines.png
+-rw-r--r--   0        0        0    48370 2023-05-23 17:25:45.065025 sarracen-1.2.1/docs/examples/ot/ot.png
+-rw-r--r--   0        0        0     1154 2023-05-23 17:25:45.065141 sarracen-1.2.1/docs/index.rst
+-rw-r--r--   0        0        0     1648 2023-05-23 17:25:45.065228 sarracen-1.2.1/docs/installation.rst
+-rw-r--r--   0        0        0      800 2023-05-23 17:25:45.065311 sarracen-1.2.1/docs/make.bat
+-rw-r--r--   0        0        0    95948 2023-05-23 17:25:45.065895 sarracen-1.2.1/docs/paper/main_image.png
+-rw-r--r--   0        0        0    14031 2023-05-23 17:25:45.066035 sarracen-1.2.1/docs/paper/paper.bib
+-rw-r--r--   0        0        0     5953 2023-05-23 17:25:45.066145 sarracen-1.2.1/docs/paper/paper.md
+-rw-r--r--   0        0        0     3484 2023-05-23 17:25:45.066247 sarracen-1.2.1/docs/quick-start.rst
+-rw-r--r--   0        0        0     4814 2023-05-23 17:25:45.066335 sarracen-1.2.1/docs/render.rst
+-rw-r--r--   0        0        0      527 2023-05-23 17:25:45.066403 sarracen-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0       75 2023-05-23 17:25:45.066468 sarracen-1.2.1/requirements.txt
+-rw-r--r--   0        0        0      363 2023-05-23 17:29:44.559778 sarracen-1.2.1/sarracen/__init__.py
+-rw-r--r--   0        0        0      385 2023-05-23 17:25:45.066665 sarracen-1.2.1/sarracen/interpolate/__init__.py
+-rw-r--r--   0        0        0     4766 2023-05-23 17:25:45.066922 sarracen-1.2.1/sarracen/interpolate/base_backend.py
+-rw-r--r--   0        0        0    24755 2023-05-23 17:25:45.067067 sarracen-1.2.1/sarracen/interpolate/cpu_backend.py
+-rw-r--r--   0        0        0    27110 2023-05-23 17:25:45.067164 sarracen-1.2.1/sarracen/interpolate/gpu_backend.py
+-rw-r--r--   0        0        0    55074 2023-05-23 17:25:45.067472 sarracen-1.2.1/sarracen/interpolate/interpolate.py
+-rw-r--r--   0        0        0      212 2023-05-23 17:25:45.067578 sarracen-1.2.1/sarracen/kernels/__init__.py
+-rw-r--r--   0        0        0     3467 2023-05-23 17:25:45.067665 sarracen-1.2.1/sarracen/kernels/base_kernel.py
+-rw-r--r--   0        0        0      562 2023-05-23 17:25:45.067732 sarracen-1.2.1/sarracen/kernels/cubic_spline.py
+-rw-r--r--   0        0        0    13535 2023-05-23 17:25:45.067832 sarracen-1.2.1/sarracen/kernels/cubic_spline_exact.py
+-rw-r--r--   0        0        0      634 2023-05-23 17:25:45.067901 sarracen-1.2.1/sarracen/kernels/quartic_spline.py
+-rw-r--r--   0        0        0      607 2023-05-23 17:25:45.067968 sarracen-1.2.1/sarracen/kernels/quintic_spline.py
+-rw-r--r--   0        0        0        1 2023-05-23 17:25:45.068062 sarracen-1.2.1/sarracen/readers/__init__.py
+-rw-r--r--   0        0        0      678 2023-05-23 17:25:45.068203 sarracen-1.2.1/sarracen/readers/read_csv.py
+-rw-r--r--   0        0        0     8959 2023-05-23 17:25:45.068313 sarracen-1.2.1/sarracen/readers/read_marisa.py
+-rw-r--r--   0        0        0     9017 2023-05-23 17:25:45.068426 sarracen-1.2.1/sarracen/readers/read_phantom.py
+-rw-r--r--   0        0        0    30051 2023-05-23 17:25:45.068505 sarracen-1.2.1/sarracen/render.py
+-rw-r--r--   0        0        0    19956 2023-05-23 17:25:45.068655 sarracen-1.2.1/sarracen/sarracen_dataframe.py
+-rw-r--r--   0        0        0        0 2023-05-23 17:25:45.068730 sarracen-1.2.1/sarracen/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 17:25:45.068798 sarracen-1.2.1/sarracen/tests/readers/__init__.py
+-rw-r--r--   0        0        0      969 2023-05-23 17:25:45.068868 sarracen-1.2.1/sarracen/tests/readers/test_read_csv.py
+-rw-r--r--   0        0        0    84917 2023-05-23 17:25:45.069147 sarracen-1.2.1/sarracen/tests/test_interpolate.py
+-rw-r--r--   0        0        0     8159 2023-05-23 17:25:45.069267 sarracen-1.2.1/sarracen/tests/test_kernels.py
+-rw-r--r--   0        0        0    11302 2023-05-23 17:25:45.069355 sarracen-1.2.1/sarracen/tests/test_render.py
+-rw-r--r--   0        0        0     5514 2023-05-23 17:25:45.069431 sarracen-1.2.1/sarracen/tests/test_sarracen_dataframe.py
+-rw-r--r--   0        0        0     2726 1970-01-01 00:00:00.000000 sarracen-1.2.1/PKG-INFO
```

### Comparing `sarracen-1.2.0/.github/workflows/joss_paper.yml` & `sarracen-1.2.1/.github/workflows/joss_paper.yml`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/LICENCE` & `sarracen-1.2.1/LICENCE`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/README.md` & `sarracen-1.2.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -22,11 +22,27 @@
     pip install git+https://github.com/ttricco/sarracen.git
 
 Documentation
 -------------
 
 Sarracen's documentation is hosted online at [https://sarracen.readthedocs.io](https://sarracen.readthedocs.io).
 
-Bugs / Missing Features
------------------------
+Contributing
+------------
 
-Please raise any bugs [as an issue](https://github.com/ttricco/sarracen/issues). If something does not work as you might expect, please let us know. If there are features that you feel are missing, please let us know.
+Contributions are welcomed and appreciated. Here are some ways to get involved:
+- Submitting bug reports.
+- Feature requests or suggestions.
+- Improving the documentation or providing examples.
+- Writing code to add optimizations or new features.
+
+Please use the [GitHub issue tracker](https://github.com/ttricco/sarracen/issues) to raise any bugs or to submit feature
+requests. If something does not work as you might expect, please let us know. If there are features that you feel are
+missing, please let us know.
+
+Code submissions should be submitted as a pull request. Make sure that all existing unit tests successfully pass, and 
+please add any new unit tests that are relevant. Documentation changes should also be submitted as a pull request.
+
+If you are stuck or need help, [raising an issue](https://github.com/ttricco/sarracen/issues) is a good place to start. 
+This helps us keep common issues in public view. Feel free to also [email](mailto:tstricco@mun.ca) with questions.
+
+Please note that we adhere to a [code of conduct](CODE_OF_CONDUCT.md).
```

### Comparing `sarracen-1.2.0/docs/Makefile` & `sarracen-1.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/docs/api.rst` & `sarracen-1.2.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/docs/conf.py` & `sarracen-1.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/docs/examples/dustydisc.rst` & `sarracen-1.2.1/docs/examples/dustydisc.rst`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/docs/examples/dustydisc/dustydisc-describe.png` & `sarracen-1.2.1/docs/examples/dustydisc/dustydisc-describe.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/docs/examples/dustydisc/dustydisc-dust.png` & `sarracen-1.2.1/docs/examples/dustydisc/dustydisc-dust.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/docs/examples/dustydisc/dustydisc-gas-sinks.png` & `sarracen-1.2.1/docs/examples/dustydisc/dustydisc-gas-sinks.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/docs/examples/dustydisc/dustydisc-gas.png` & `sarracen-1.2.1/docs/examples/dustydisc/dustydisc-gas.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/docs/examples/dustydisc/dustydisc-sdf-sinks.png` & `sarracen-1.2.1/docs/examples/dustydisc/dustydisc-sdf-sinks.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/docs/examples/dustydisc/dustydisc-sdf.png` & `sarracen-1.2.1/docs/examples/dustydisc/dustydisc-sdf.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/docs/examples/dustydisc/dustydisc-value-counts.png` & `sarracen-1.2.1/docs/examples/dustydisc/dustydisc-value-counts.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/docs/examples/ot.rst` & `sarracen-1.2.1/docs/examples/ot.rst`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/docs/examples/ot/ot-1d.png` & `sarracen-1.2.1/docs/examples/ot/ot-1d.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/docs/examples/ot/ot-describe.png` & `sarracen-1.2.1/docs/examples/ot/ot-describe.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/docs/examples/ot/ot-sdf.png` & `sarracen-1.2.1/docs/examples/ot/ot-sdf.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/docs/examples/ot/ot-streamlines.png` & `sarracen-1.2.1/docs/examples/ot/ot-streamlines.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/docs/examples/ot/ot.png` & `sarracen-1.2.1/docs/examples/ot/ot.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/docs/index.rst` & `sarracen-1.2.1/docs/index.rst`

 * *Files 14% similar despite different names*

```diff
@@ -21,14 +21,15 @@
    :caption: Contents:
 
    installation
    quick-start
    render
    examples
    api
+   contributing
 
 
 Indices and tables
 ==================
 
 * :ref:`genindex`
 * :ref:`modindex`
```

### Comparing `sarracen-1.2.0/docs/installation.rst` & `sarracen-1.2.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/docs/make.bat` & `sarracen-1.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/docs/paper/main_image.png` & `sarracen-1.2.1/docs/paper/main_image.png`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/docs/paper/paper.bib` & `sarracen-1.2.1/docs/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/docs/paper/paper.md` & `sarracen-1.2.1/docs/paper/paper.md`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/docs/quick-start.rst` & `sarracen-1.2.1/docs/quick-start.rst`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/docs/render.rst` & `sarracen-1.2.1/docs/render.rst`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/pyproject.toml` & `sarracen-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/sarracen/interpolate/base_backend.py` & `sarracen-1.2.1/sarracen/interpolate/base_backend.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/sarracen/interpolate/cpu_backend.py` & `sarracen-1.2.1/sarracen/interpolate/cpu_backend.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/sarracen/interpolate/gpu_backend.py` & `sarracen-1.2.1/sarracen/interpolate/gpu_backend.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/sarracen/interpolate/interpolate.py` & `sarracen-1.2.1/sarracen/interpolate/interpolate.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/sarracen/kernels/base_kernel.py` & `sarracen-1.2.1/sarracen/kernels/base_kernel.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/sarracen/kernels/cubic_spline.py` & `sarracen-1.2.1/sarracen/kernels/cubic_spline.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/sarracen/kernels/cubic_spline_exact.py` & `sarracen-1.2.1/sarracen/kernels/cubic_spline_exact.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/sarracen/kernels/quartic_spline.py` & `sarracen-1.2.1/sarracen/kernels/quartic_spline.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/sarracen/kernels/quintic_spline.py` & `sarracen-1.2.1/sarracen/kernels/quintic_spline.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/sarracen/readers/read_csv.py` & `sarracen-1.2.1/sarracen/readers/read_csv.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/sarracen/readers/read_marisa.py` & `sarracen-1.2.1/sarracen/readers/read_marisa.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/sarracen/readers/read_phantom.py` & `sarracen-1.2.1/sarracen/readers/read_phantom.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/sarracen/render.py` & `sarracen-1.2.1/sarracen/render.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,14 +148,16 @@
         For a 3D dataset, the z value to take a cross-section at. If none, column interpolation is performed.
     kernel: BaseKernel, optional
         Kernel to use for smoothing the target data. Defaults to the kernel specified in `data`.
     x_pixels, y_pixels: int, optional
         Number of pixels present in the final image.
     xlim, ylim: tuple of float, optional
         The starting and ending corners of the final 2D image.
+    vmin, vmax: float, optional
+        Lower and upper limits of the range of values for the colour bar.
     cmap: str or Colormap, optional
         The color map to use when plotting a 2D image.
     cbar: bool, optional
         True if a colorbar should be drawn.
     cbar_kws: dict, optional
         Keyword arguments to pass to matplotlib.figure.Figure.colorbar().
     cbar_ax: Axes
@@ -269,15 +271,17 @@
 
     x, y = _default_axes(data, x, y)
     xlim, ylim = _default_bounds(data, x, y, xlim, ylim)
 
     kwargs.setdefault("origin", 'lower')
     kwargs.setdefault("extent", [xlim[0], xlim[1], ylim[0], ylim[1]])
     if log_scale:
-        kwargs.setdefault("norm", LogNorm(clip=True))
+        kwargs.setdefault("norm", LogNorm(clip=True, vmin=kwargs.get('vmin'), vmax=kwargs.get('vmax')))
+        kwargs.pop("vmin", None)
+        kwargs.pop("vmax", None)
 
     graphic = ax.imshow(img, cmap=cmap, **kwargs)
     if rotation is not None and data.get_dim() == 3:
         ax.set_xticks([])
         ax.set_yticks([])
     else:
         ax.set_xlabel(x)
```

### Comparing `sarracen-1.2.0/sarracen/sarracen_dataframe.py` & `sarracen-1.2.1/sarracen/sarracen_dataframe.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/sarracen/tests/readers/test_read_csv.py` & `sarracen-1.2.1/sarracen/tests/readers/test_read_csv.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/sarracen/tests/test_interpolate.py` & `sarracen-1.2.1/sarracen/tests/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/sarracen/tests/test_kernels.py` & `sarracen-1.2.1/sarracen/tests/test_kernels.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/sarracen/tests/test_render.py` & `sarracen-1.2.1/sarracen/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/sarracen/tests/test_sarracen_dataframe.py` & `sarracen-1.2.1/sarracen/tests/test_sarracen_dataframe.py`

 * *Files identical despite different names*

### Comparing `sarracen-1.2.0/PKG-INFO` & `sarracen-1.2.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarracen
-Version: 1.2.0
+Version: 1.2.1
 Summary: SPH analysis and visualization
 Author-email: "Terrence S. Tricco" <tstricco@mun.ca>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: matplotlib>=3.6
 Requires-Dist: numba>=0.55.1
 Requires-Dist: pandas>=1.4
@@ -37,12 +37,27 @@
     pip install git+https://github.com/ttricco/sarracen.git
 
 Documentation
 -------------
 
 Sarracen's documentation is hosted online at [https://sarracen.readthedocs.io](https://sarracen.readthedocs.io).
 
-Bugs / Missing Features
------------------------
+Contributing
+------------
+
+Contributions are welcomed and appreciated. Here are some ways to get involved:
+- Submitting bug reports.
+- Feature requests or suggestions.
+- Improving the documentation or providing examples.
+- Writing code to add optimizations or new features.
+
+Please use the [GitHub issue tracker](https://github.com/ttricco/sarracen/issues) to raise any bugs or to submit feature
+requests. If something does not work as you might expect, please let us know. If there are features that you feel are
+missing, please let us know.
+
+Code submissions should be submitted as a pull request. Make sure that all existing unit tests successfully pass, and 
+please add any new unit tests that are relevant. Documentation changes should also be submitted as a pull request.
 
-Please raise any bugs [as an issue](https://github.com/ttricco/sarracen/issues). If something does not work as you might expect, please let us know. If there are features that you feel are missing, please let us know.
+If you are stuck or need help, [raising an issue](https://github.com/ttricco/sarracen/issues) is a good place to start. 
+This helps us keep common issues in public view. Feel free to also [email](mailto:tstricco@mun.ca) with questions.
 
+Please note that we adhere to a [code of conduct](CODE_OF_CONDUCT.md).
```

