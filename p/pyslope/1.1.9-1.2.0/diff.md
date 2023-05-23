# Comparing `tmp/pyslope-1.1.9.tar.gz` & `tmp/pyslope-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyslope-1.1.9.tar", last modified: Thu Jun  9 08:18:03 2022, max compression
+gzip compressed data, was "pyslope-1.2.0.tar", last modified: Tue May 23 12:52:54 2023, max compression
```

## Comparing `pyslope-1.1.9.tar` & `pyslope-1.2.0.tar`

### file list

```diff
@@ -1,71 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 08:18:03.684959 pyslope-1.1.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-06-09 08:17:57.000000 pyslope-1.1.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-06-09 08:17:57.000000 pyslope-1.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    13988 2022-06-09 08:18:03.684959 pyslope-1.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10838 2022-06-09 08:17:57.000000 pyslope-1.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 08:18:03.684959 pyslope-1.1.9/pyslope/
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      498 2022-06-09 08:18:03.684959 pyslope-1.1.9/pyslope/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     3176 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/data_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 08:18:03.668959 pyslope-1.1.9/pyslope/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 08:18:03.668959 pyslope-1.1.9/pyslope/examples/hyrcan/
--rw-r--r--   0 runner    (1001) docker     (121)     1488 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/hyrcan/a.hjs
--rw-r--r--   0 runner    (1001) docker     (121)     1488 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/hyrcan/b.hjs
--rw-r--r--   0 runner    (1001) docker     (121)     1529 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/hyrcan/c.hjs
--rw-r--r--   0 runner    (1001) docker     (121)     1780 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/hyrcan/d.hjs
--rw-r--r--   0 runner    (1001) docker     (121)     1699 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/hyrcan/e.hjs
--rw-r--r--   0 runner    (1001) docker     (121)    78940 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/hyrcan/hyrcan.png
--rw-r--r--   0 runner    (1001) docker     (121)    10593 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/readme_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   287714 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/readme_example_plot_all_maxfos2.png
--rw-r--r--   0 runner    (1001) docker     (121)    87260 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/readme_example_plot_boundary.png
--rw-r--r--   0 runner    (1001) docker     (121)   112604 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/readme_example_plot_critical.png
--rw-r--r--   0 runner    (1001) docker     (121)   106712 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/readme_example_plot_dynamic.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 08:18:03.672959 pyslope-1.1.9/pyslope/examples/readme_img/
--rw-r--r--   0 runner    (1001) docker     (121)    87260 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/readme_img/limits.png
--rw-r--r--   0 runner    (1001) docker     (121)    87092 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/readme_img/lls.png
--rw-r--r--   0 runner    (1001) docker     (121)    73458 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/readme_img/materials.png
--rw-r--r--   0 runner    (1001) docker     (121)   311831 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/readme_img/plot_all_planes2.png
--rw-r--r--   0 runner    (1001) docker     (121)    87260 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/readme_img/plot_boundary.png
--rw-r--r--   0 runner    (1001) docker     (121)   110295 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/readme_img/plot_critical.png
--rw-r--r--   0 runner    (1001) docker     (121)    78725 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/readme_img/slope.png
--rw-r--r--   0 runner    (1001) docker     (121)    84746 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/readme_img/udls.png
--rw-r--r--   0 runner    (1001) docker     (121)    87351 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/readme_img/water.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 08:18:03.672959 pyslope-1.1.9/pyslope/examples/search/
--rw-r--r--   0 runner    (1001) docker     (121)   239228 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/search/pySlope_1000.png
--rw-r--r--   0 runner    (1001) docker     (121)   284414 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/search/pySlope_2000.png
--rw-r--r--   0 runner    (1001) docker     (121)   295997 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/search/pySlope_5000.png
--rw-r--r--   0 runner    (1001) docker     (121)    46293 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/search/slide_1000.png
--rw-r--r--   0 runner    (1001) docker     (121)    59090 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/search/slide_2000.png
--rw-r--r--   0 runner    (1001) docker     (121)    75086 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/search/slide_5000.png
--rw-r--r--   0 runner    (1001) docker     (121)    10027 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/search.xlsx
--rw-r--r--   0 runner    (1001) docker     (121)    10955 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/slices.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 08:18:03.672959 pyslope-1.1.9/pyslope/examples/slide/
--rw-r--r--   0 runner    (1001) docker     (121)   217762 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/slide/a.slim
--rw-r--r--   0 runner    (1001) docker     (121)    89844 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/slide/a_2000.slim
--rw-r--r--   0 runner    (1001) docker     (121)   136002 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/slide/b.slim
--rw-r--r--   0 runner    (1001) docker     (121)   136540 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/slide/c.slim
--rw-r--r--   0 runner    (1001) docker     (121)    22851 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/slide/c2.slim
--rw-r--r--   0 runner    (1001) docker     (121)   136038 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/slide/d.slim
--rw-r--r--   0 runner    (1001) docker     (121)   146568 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/slide/e.slim
--rw-r--r--   0 runner    (1001) docker     (121)   109179 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/slide/f.slim
--rw-r--r--   0 runner    (1001) docker     (121)    38557 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/slide/slide.png
--rw-r--r--   0 runner    (1001) docker     (121)    12618 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/summary_results.xlsx
--rw-r--r--   0 runner    (1001) docker     (121)   896867 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/examples/validation.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 08:18:03.680959 pyslope-1.1.9/pyslope/graphs/
--rw-r--r--   0 runner    (1001) docker     (121)     6141 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/graphs/graphs.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)  3488504 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/graphs/sandstone_fill_5m_1_1.html
--rw-r--r--   0 runner    (1001) docker     (121)  3487188 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/graphs/sandstone_fill_FOS_1.25_for_loads_and_angles.html
--rw-r--r--   0 runner    (1001) docker     (121)    82744 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/pyslope.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 08:18:03.684959 pyslope-1.1.9/pyslope/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/tests/test_slope.py
--rw-r--r--   0 runner    (1001) docker     (121)    11039 2022-06-09 08:17:57.000000 pyslope-1.1.9/pyslope/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 08:18:03.664959 pyslope-1.1.9/pyslope.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13988 2022-06-09 08:18:03.000000 pyslope-1.1.9/pyslope.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1952 2022-06-09 08:18:03.000000 pyslope-1.1.9/pyslope.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-09 08:18:03.000000 pyslope-1.1.9/pyslope.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-06-09 08:18:03.000000 pyslope-1.1.9/pyslope.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-06-09 08:18:03.000000 pyslope-1.1.9/pyslope.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-06-09 08:17:57.000000 pyslope-1.1.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      377 2022-06-09 08:18:03.684959 pyslope-1.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2054 2022-06-09 08:17:57.000000 pyslope-1.1.9/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    81180 2022-06-09 08:17:57.000000 pyslope-1.1.9/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:52:54.005010 pyslope-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-23 12:52:47.000000 pyslope-1.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-23 12:52:47.000000 pyslope-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14216 2023-05-23 12:52:54.005010 pyslope-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11034 2023-05-23 12:52:47.000000 pyslope-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:52:54.005010 pyslope-1.2.0/pyslope/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-23 12:52:54.005010 pyslope-1.2.0/pyslope/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/data_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:52:53.989010 pyslope-1.2.0/pyslope/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/docs/docstrings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13786 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/docs/requirements_docs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:52:53.989010 pyslope-1.2.0/pyslope/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:52:53.989010 pyslope-1.2.0/pyslope/examples/hyrcan/
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/hyrcan/a.hjs
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/hyrcan/b.hjs
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/hyrcan/c.hjs
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/hyrcan/d.hjs
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/hyrcan/e.hjs
+-rw-r--r--   0 runner    (1001) docker     (123)    78940 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/hyrcan/hyrcan.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/readme_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   287714 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/readme_example_plot_all_maxfos2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    87260 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/readme_example_plot_boundary.png
+-rw-r--r--   0 runner    (1001) docker     (123)   112604 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/readme_example_plot_critical.png
+-rw-r--r--   0 runner    (1001) docker     (123)   106712 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/readme_example_plot_dynamic.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:52:53.993010 pyslope-1.2.0/pyslope/examples/readme_img/
+-rw-r--r--   0 runner    (1001) docker     (123)    87260 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/readme_img/limits.png
+-rw-r--r--   0 runner    (1001) docker     (123)    87092 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/readme_img/lls.png
+-rw-r--r--   0 runner    (1001) docker     (123)    73458 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/readme_img/materials.png
+-rw-r--r--   0 runner    (1001) docker     (123)   311831 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/readme_img/plot_all_planes2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    87260 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/readme_img/plot_boundary.png
+-rw-r--r--   0 runner    (1001) docker     (123)   110295 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/readme_img/plot_critical.png
+-rw-r--r--   0 runner    (1001) docker     (123)    78725 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/readme_img/slope.png
+-rw-r--r--   0 runner    (1001) docker     (123)    84746 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/readme_img/udls.png
+-rw-r--r--   0 runner    (1001) docker     (123)    87351 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/readme_img/water.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:52:53.993010 pyslope-1.2.0/pyslope/examples/search/
+-rw-r--r--   0 runner    (1001) docker     (123)   239228 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/search/pySlope_1000.png
+-rw-r--r--   0 runner    (1001) docker     (123)   284414 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/search/pySlope_2000.png
+-rw-r--r--   0 runner    (1001) docker     (123)   295997 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/search/pySlope_5000.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46293 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/search/slide_1000.png
+-rw-r--r--   0 runner    (1001) docker     (123)    59090 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/search/slide_2000.png
+-rw-r--r--   0 runner    (1001) docker     (123)    75086 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/search/slide_5000.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/search.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/slices.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:52:53.997010 pyslope-1.2.0/pyslope/examples/slide/
+-rw-r--r--   0 runner    (1001) docker     (123)   217762 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/slide/a.slim
+-rw-r--r--   0 runner    (1001) docker     (123)    89844 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/slide/a_2000.slim
+-rw-r--r--   0 runner    (1001) docker     (123)   136002 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/slide/b.slim
+-rw-r--r--   0 runner    (1001) docker     (123)   136540 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/slide/c.slim
+-rw-r--r--   0 runner    (1001) docker     (123)    22851 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/slide/c2.slim
+-rw-r--r--   0 runner    (1001) docker     (123)   136038 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/slide/d.slim
+-rw-r--r--   0 runner    (1001) docker     (123)   146568 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/slide/e.slim
+-rw-r--r--   0 runner    (1001) docker     (123)   109179 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/slide/f.slim
+-rw-r--r--   0 runner    (1001) docker     (123)    38557 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/slide/slide.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/summary_results.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    89313 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/examples/validation.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:52:54.001010 pyslope-1.2.0/pyslope/graphs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/graphs/graphs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  3488504 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/graphs/sandstone_fill_5m_1_1.html
+-rw-r--r--   0 runner    (1001) docker     (123)  3487188 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/graphs/sandstone_fill_FOS_1.25_for_loads_and_angles.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:52:54.005010 pyslope-1.2.0/pyslope/paper/
+-rw-r--r--   0 runner    (1001) docker     (123)    11968 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/paper/paper.md
+-rw-r--r--   0 runner    (1001) docker     (123)   398520 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/paper/pySlope_paper.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    87429 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/pyslope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:52:54.005010 pyslope-1.2.0/pyslope/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/tests/test_slope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/tests/test_validation_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-05-23 12:52:47.000000 pyslope-1.2.0/pyslope/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:52:53.985010 pyslope-1.2.0/pyslope.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14216 2023-05-23 12:52:53.000000 pyslope-1.2.0/pyslope.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-23 12:52:53.000000 pyslope-1.2.0/pyslope.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 12:52:53.000000 pyslope-1.2.0/pyslope.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-23 12:52:53.000000 pyslope-1.2.0/pyslope.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 12:52:53.000000 pyslope-1.2.0/pyslope.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-23 12:52:47.000000 pyslope-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-23 12:52:54.005010 pyslope-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-23 12:52:47.000000 pyslope-1.2.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-05-23 12:52:47.000000 pyslope-1.2.0/versioneer.py
```

### Comparing `pyslope-1.1.9/LICENSE.txt` & `pyslope-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/PKG-INFO` & `pyslope-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 Metadata-Version: 2.1
 Name: pyslope
-Version: 1.1.9
+Version: 1.2.0
 Summary: A 2D Slope Stability Software using bishops method
 Home-page: https://github.com/JesseBonanno/pyslope
 Author: Jesse Bonanno
 Author-email: jessebonanno@gmail.com
 License: MIT
-Download-URL: https://github.com/JesseBonanno/pyslope/archive/v1.1.9.tar.gz
+Download-URL: https://github.com/JesseBonanno/pyslope/archive/v1.2.0.tar.gz
 Description: # pySlope
         
         
         [![PyPi](https://img.shields.io/pypi/v/pyslope.svg)](https://pypi.org/project/pyslope/)
         [![License](https://img.shields.io/badge/license-MIT-lightgreen.svg)](https://github.com/JesseBonanno/pyslope/blob/main/LICENSE.txt)
         [![CodeFactor](https://www.codefactor.io/repository/github/jessebonanno/pyslope/badge?s=43db3d31fb1ca55747ede7e5205c7d9e0cf37ced)](https://www.codefactor.io/repository/github/jessebonanno/pyslope)
         [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JesseBonanno/pyslope/main?filepath=pyslope%2Fexamples%2Freadme_example.ipynb)
         [![Documentation Status](https://readthedocs.org/projects/pyslope/badge/?version=latest)](https://pyslope.readthedocs.io/en/latest)
         [![Code Style](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black)
         [![Downloads](https://pepy.tech/badge/pyslope)](https://pepy.tech/project/pyslope)
         [![codecov](https://codecov.io/gh/JesseBonanno/PySlope/branch/main/graph/badge.svg?token=ASUIW54CXV)](https://codecov.io/gh/JesseBonanno/PySlope)
         [![CI](https://github.com/JesseBonanno/PySlope/actions/workflows/ci.yaml/badge.svg)](https://github.com/JesseBonanno/PySlope/actions/workflows/ci.yaml)
         [![pre-commit](https://github.com/JesseBonanno/PySlope/actions/workflows/pre-commit.yaml/badge.svg)](https://github.com/JesseBonanno/PySlope/actions/workflows/pre-commit.yaml)
+        [![Website](https://img.shields.io/badge/website-up-brightgreen)](https://pyslope.herokuapp.com/)
+        
         
         pySlope is a 2D slope stability module based on bishops method of slices. This module allows for the following parameters:
            - unlimited horizontal geological units
            - water table
            - uniform loads
            - line loads
            - slope search limits
          
         This module can return plots for the critical failure slope or plots for all failure slopes below a certain factor of safety.
         
         ## Project Purpose
         
         The purpose of this project is two fold:
         
-           1. Create a free online slope stability software
+           1. Create a free online slope stability software [![Website](https://img.shields.io/badge/website-up-brightgreen)](https://pyslope.herokuapp.com/)
            2. Provide a pythonic solution to implementing Bishop's method based on object oriented coding principles
         
         Performing a slope stability calculation by hand is extremely uneconimical and time consuming. The problem involves a lot of geometrical mathematics which can make the calculation hard to achieve with only excel. Python packages exist for geometrical mathematics which makes Python well suited for implementing a slope stability analysis package. There is however, no well-documented open-source slope stability software that can currently be found online. This package aims to fill that gap.
         
         ## Functionality and usage
         
         A typical use case of the `pySlope` package involves the following steps:
@@ -280,28 +282,30 @@
         ```
         
         Releasing
         ---------
         
         Releases are published automatically when a tag is pushed to GitHub.
         
-        .. code-block:: bash
+        ```shell
+        # Set next version number
+        export RELEASE=vX.X.X
         
-           # Set next version number
-           export RELEASE=vX.X.X
+        # Create tags
+        git commit --allow-empty -m "Release $RELEASE"
+        git tag -a $RELEASE -m "Version $RELEASE"
         
-           # Create tags
-           git commit --allow-empty -m "Release $RELEASE"
-           git tag -a $RELEASE -m "Version $RELEASE"
+        # Push (for working from a fork)
+        git push upstream --tags
         
-           # Push (for working from a fork)
-           git push upstream --tags
+        # if not working from fork would instead be
+        # git push origin --tags
+        ```
         
-           # if not working from fork would instead be
-           # git push origin --tags
+        Or set a tag with Github Desktop.
         
         ## License
         
         [![License](https://img.shields.io/badge/license-MIT-lightgreen.svg)](https://github.com/JesseBonanno/pyslope/blob/main/LICENSE.txt)
         
 Keywords: geotechnical,slope,stability,civil,engineering,bishops
 Platform: UNKNOWN
```

### Comparing `pyslope-1.1.9/README.md` & `pyslope-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,29 +7,31 @@
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JesseBonanno/pyslope/main?filepath=pyslope%2Fexamples%2Freadme_example.ipynb)
 [![Documentation Status](https://readthedocs.org/projects/pyslope/badge/?version=latest)](https://pyslope.readthedocs.io/en/latest)
 [![Code Style](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black)
 [![Downloads](https://pepy.tech/badge/pyslope)](https://pepy.tech/project/pyslope)
 [![codecov](https://codecov.io/gh/JesseBonanno/PySlope/branch/main/graph/badge.svg?token=ASUIW54CXV)](https://codecov.io/gh/JesseBonanno/PySlope)
 [![CI](https://github.com/JesseBonanno/PySlope/actions/workflows/ci.yaml/badge.svg)](https://github.com/JesseBonanno/PySlope/actions/workflows/ci.yaml)
 [![pre-commit](https://github.com/JesseBonanno/PySlope/actions/workflows/pre-commit.yaml/badge.svg)](https://github.com/JesseBonanno/PySlope/actions/workflows/pre-commit.yaml)
+[![Website](https://img.shields.io/badge/website-up-brightgreen)](https://pyslope.herokuapp.com/)
+
 
 pySlope is a 2D slope stability module based on bishops method of slices. This module allows for the following parameters:
    - unlimited horizontal geological units
    - water table
    - uniform loads
    - line loads
    - slope search limits
  
 This module can return plots for the critical failure slope or plots for all failure slopes below a certain factor of safety.
 
 ## Project Purpose
 
 The purpose of this project is two fold:
 
-   1. Create a free online slope stability software
+   1. Create a free online slope stability software [![Website](https://img.shields.io/badge/website-up-brightgreen)](https://pyslope.herokuapp.com/)
    2. Provide a pythonic solution to implementing Bishop's method based on object oriented coding principles
 
 Performing a slope stability calculation by hand is extremely uneconimical and time consuming. The problem involves a lot of geometrical mathematics which can make the calculation hard to achieve with only excel. Python packages exist for geometrical mathematics which makes Python well suited for implementing a slope stability analysis package. There is however, no well-documented open-source slope stability software that can currently be found online. This package aims to fill that gap.
 
 ## Functionality and usage
 
 A typical use case of the `pySlope` package involves the following steps:
@@ -271,25 +273,27 @@
 ```
 
 Releasing
 ---------
 
 Releases are published automatically when a tag is pushed to GitHub.
 
-.. code-block:: bash
+```shell
+# Set next version number
+export RELEASE=vX.X.X
 
-   # Set next version number
-   export RELEASE=vX.X.X
+# Create tags
+git commit --allow-empty -m "Release $RELEASE"
+git tag -a $RELEASE -m "Version $RELEASE"
 
-   # Create tags
-   git commit --allow-empty -m "Release $RELEASE"
-   git tag -a $RELEASE -m "Version $RELEASE"
+# Push (for working from a fork)
+git push upstream --tags
 
-   # Push (for working from a fork)
-   git push upstream --tags
+# if not working from fork would instead be
+# git push origin --tags
+```
 
-   # if not working from fork would instead be
-   # git push origin --tags
+Or set a tag with Github Desktop.
 
 ## License
 
 [![License](https://img.shields.io/badge/license-MIT-lightgreen.svg)](https://github.com/JesseBonanno/pyslope/blob/main/LICENSE.txt)
```

### Comparing `pyslope-1.1.9/pyslope/data_validation.py` & `pyslope-1.2.0/pyslope/data_validation.py`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/examples/hyrcan/a.hjs` & `pyslope-1.2.0/pyslope/examples/hyrcan/a.hjs`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/examples/hyrcan/b.hjs` & `pyslope-1.2.0/pyslope/examples/hyrcan/b.hjs`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/examples/hyrcan/c.hjs` & `pyslope-1.2.0/pyslope/examples/hyrcan/c.hjs`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/examples/hyrcan/d.hjs` & `pyslope-1.2.0/pyslope/examples/hyrcan/d.hjs`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/examples/hyrcan/e.hjs` & `pyslope-1.2.0/pyslope/examples/hyrcan/e.hjs`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/examples/hyrcan/hyrcan.png` & `pyslope-1.2.0/pyslope/examples/hyrcan/hyrcan.png`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/examples/readme_example_plot_all_maxfos2.png` & `pyslope-1.2.0/pyslope/examples/readme_example_plot_all_maxfos2.png`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/examples/readme_example_plot_boundary.png` & `pyslope-1.2.0/pyslope/examples/readme_example_plot_boundary.png`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/examples/readme_example_plot_critical.png` & `pyslope-1.2.0/pyslope/examples/readme_example_plot_critical.png`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/examples/readme_example_plot_dynamic.png` & `pyslope-1.2.0/pyslope/examples/readme_example_plot_dynamic.png`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/examples/readme_img/limits.png` & `pyslope-1.2.0/pyslope/examples/readme_img/limits.png`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/examples/readme_img/lls.png` & `pyslope-1.2.0/pyslope/examples/readme_img/lls.png`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/examples/readme_img/materials.png` & `pyslope-1.2.0/pyslope/examples/readme_img/materials.png`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/examples/readme_img/plot_all_planes2.png` & `pyslope-1.2.0/pyslope/examples/readme_img/plot_all_planes2.png`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/examples/readme_img/plot_boundary.png` & `pyslope-1.2.0/pyslope/examples/readme_img/plot_boundary.png`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/examples/readme_img/plot_critical.png` & `pyslope-1.2.0/pyslope/examples/readme_img/plot_critical.png`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/examples/readme_img/slope.png` & `pyslope-1.2.0/pyslope/examples/readme_img/slope.png`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/examples/readme_img/udls.png` & `pyslope-1.2.0/pyslope/examples/readme_img/udls.png`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/examples/readme_img/water.png` & `pyslope-1.2.0/pyslope/examples/readme_img/water.png`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/examples/search/pySlope_1000.png` & `pyslope-1.2.0/pyslope/examples/search/pySlope_1000.png`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/examples/search/pySlope_2000.png` & `pyslope-1.2.0/pyslope/examples/search/pySlope_2000.png`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/examples/search/pySlope_5000.png` & `pyslope-1.2.0/pyslope/examples/search/pySlope_5000.png`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/examples/search/slide_1000.png` & `pyslope-1.2.0/pyslope/examples/search/slide_1000.png`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/examples/search/slide_2000.png` & `pyslope-1.2.0/pyslope/examples/search/slide_2000.png`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/examples/search/slide_5000.png` & `pyslope-1.2.0/pyslope/examples/search/slide_5000.png`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/examples/search.xlsx` & `pyslope-1.2.0/pyslope/examples/search.xlsx`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/examples/slices.xlsx` & `pyslope-1.2.0/pyslope/examples/slices.xlsx`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/examples/slide/a.slim` & `pyslope-1.2.0/pyslope/examples/slide/a.slim`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/examples/slide/a_2000.slim` & `pyslope-1.2.0/pyslope/examples/slide/a_2000.slim`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/examples/slide/b.slim` & `pyslope-1.2.0/pyslope/examples/slide/b.slim`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/examples/slide/c.slim` & `pyslope-1.2.0/pyslope/examples/slide/c.slim`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/examples/slide/c2.slim` & `pyslope-1.2.0/pyslope/examples/slide/c2.slim`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/examples/slide/d.slim` & `pyslope-1.2.0/pyslope/examples/slide/d.slim`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/examples/slide/e.slim` & `pyslope-1.2.0/pyslope/examples/slide/e.slim`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/examples/slide/f.slim` & `pyslope-1.2.0/pyslope/examples/slide/f.slim`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/examples/slide/slide.png` & `pyslope-1.2.0/pyslope/examples/slide/slide.png`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/examples/summary_results.xlsx` & `pyslope-1.2.0/pyslope/examples/summary_results.xlsx`

 * *Files 21% similar despite different names*

```diff
@@ -103,687 +103,708 @@
 00000660: f8ae 01d5 4253 edad 86b0 b737 a0ea 93cf  ....BS.....7....
 00000670: 9b7f d796 a6e9 0d3f 8839 4cec d299 15c8  .......?.9L.....
 00000680: 7362 67d9 ae7c c86c 21f5 f91a 5553 6839  sbg..|.l!...USh9
 00000690: 69b0 629e 723a 2279 5f64 6cc0 f344 9bbf  i.b.r:"y_dl..D..
 000006a0: 13fd 7c2d 4e9c c852 2234 12f8 32cf 47c7  ..|-N..R"4..2.G.
 000006b0: 25a0 f57f 5ab4 34f1 cb9d 79c4 3709 c3ab  %...Z.4...y.7...
 000006c0: c8f0 c982 8b1f a8de 0100 00ff ff03 0050  ...............P
-000006d0: 4b03 0414 0006 0008 0000 0021 0071 e87b  K..........!.q.{
-000006e0: 2fb3 0300 0064 0900 000f 0000 0078 6c2f  /....d.......xl/
+000006d0: 4b03 0414 0006 0008 0000 0021 000e 2db9  K..........!..-.
+000006e0: 62a1 0300 0051 0900 000f 0000 0078 6c2f  b....Q.......xl/
 000006f0: 776f 726b 626f 6f6b 2e78 6d6c ac55 5d6f  workbook.xml.U]o
-00000700: a338 147d 5f69 ff03 e29d 8209 1f01 3519  .8.}_i........5.
-00000710: 852f 6d57 eda8 6a33 ed4b a4ca 01a7 a002  ./mW..j3.K......
-00000720: 666d d310 55f3 dff7 9a84 94a6 ab55 b6b3  fm..U........U..
-00000730: 5162 c7f6 c9c9 b9d7 e75e 2ebf 7555 a9bc  Qb.......^..uU..
-00000740: 12c6 0b5a cf54 7461 a80a a953 9a15 f5f3  ...Z.Tta...S....
-00000750: 4cfd b14c b4a9 aa70 81eb 0c97 b426 3375  L..L...p.....&3u
-00000760: 47b8 fa6d fefb 6f97 5bca 5ed6 94be 2840  G..m..o.[.^...(@
-00000770: 50f3 999a 0bd1 f8ba ced3 9c54 985f d086  P..........T._..
-00000780: d470 b2a1 acc2 0296 ec59 e70d 2338 e339  .p.......Y..#8.9
-00000790: 21a2 2a75 d330 1cbd c245 adee 197c 760e  !.*u.0...E...|v.
-000007a0: 07dd 6c8a 9444 346d 2b52 8b3d 0923 2516  ..l..D4m+R.=.#%.
-000007b0: 209f e745 c307 b62a 3d87 aec2 eca5 6db4   ..E...*=.....m.
-000007c0: 9456 0d50 ac8b b210 bb9e 5455 aad4 bf7a  .V.P......TU...z
-000007d0: ae29 c3eb 12c2 ee90 ad74 0cde 0e7c 9001  .).......t...|..
-000007e0: 8339 fc13 1c7d faab aa48 19e5 7423 2e80  .9...}...H..t#..
-000007f0: 5adf 8bfe 143f 3274 843e a4a0 fb9c 83f3  Z....?2t.>......
-00000800: 982c 9d91 d742 dee1 5115 73be a8ca 3972  .,...B..Q.s...9r
-00000810: 39ef 64c8 f865 3604 d6ea bde2 43f2 bec8  9.d..e6.....C...
-00000820: 661f b599 eafc 7253 94e4 616f 5d05 37cd  f.....rS..ao].7.
-00000830: 775c c99b 2a55 a5c4 5cc4 5921 4836 535d  w\..*U..\.Y!H6S]
-00000840: 58d2 2df9 b0c1 da26 688b 124e 4ddb 346d  X.-....&h..NM.4m
-00000850: 559f 1fed 7ccb 948c 6c70 5b8a 2518 79a0  U...|...lp[.%.y.
-00000860: 87ca 701c 6f8f 0463 2c4a 4158 8d05 0969  ..p.o..c,JAX...i
-00000870: 2dc0 8787 b87e d573 f34b e00e 730a 0e57  -....~.s.K..s..W
-00000880: eec8 5f6d c108 1416 f80b 6285 11a7 3e5e  .._m......b...>^
-00000890: f35b 2c72 a565 e54c 0dfd d50f 0ee1 affe  .[,r.e.L........
-000008a0: 249c 9355 c468 b3a6 ddaa d989 9cd6 30dd  $..U.h........0.
-000008b0: 9750 84ab dbc3 dcec 78bf 261d ae9a 92f0  .P......x.&.....
-000008c0: d5c8 bff8 73b1 fc07 07e3 5426 503f 6adf  ....s.....T&P?j.
-000008d0: 7f3f cd11 84c0 fcc1 a5b7 8229 f0fd 2aba  .?.........)..*.
-000008e0: 869b bac7 af70 6fe0 8eec 50d6 5770 3168  .....po...P.Wp1h
-000008f0: f254 a7cc 474f 6fa1 113b 8e3b 35b4 d035  .T..GOo..;.;5..5
-00000900: 22cd 9a9a 0bcd 8b5c 5b0b 23d7 b50d 072d  "......\[.#....-
-00000910: 6237 f909 c130 c74f 296e 457e b084 a49e  b7...0.O)nE~....
-00000920: a916 dcff a7a3 1bdc 0d27 c8f0 db22 7b97  .........'..."{.
-00000930: f166 1c5e 9a9c 4f86 e1ec a70c 5836 bf87  .f.^..O.....X6..
-00000940: 826c f9bb 79e4 52e9 1e8b 3aa3 db99 aa21  .l..y.R...:....!
-00000950: 1382 da7d 5c6e fbc3 c722 1339 b8cf 332c  ...}\n...".9..3,
-00000960: 80ec f7fe 20c5 730e 8a91 3d95 9b38 15c5  .... .s...=..8..
-00000970: 2b59 e235 2895 2198 52e7 4c7d 43a6 0739  +Y.5(.!.R.L}C..9
-00000980: f05c 2d70 d144 b3ec e944 0bc2 c4d2 22db  .\-p.D...D....".
-00000990: 5924 8ebd 8817 91dd ebd3 4702 fba6 0b42  Y$........G....B
-000009a0: fb59 a9fb 42c1 d0d8 652f eeb3 ad2a cc97  .Y..B...e/...*..
-000009b0: f4ec 2a43 32b8 3170 3d02 42d7 3b02 cd53  ..*C2.1p=.B.;..S
-000009c0: 603a 024e 46c0 c929 301b 0121 b823 a375  `:.NF..)0..!.#.u
-000009d0: 0a24 23a0 3d02 f625 ab0f 51a5 b84c a16e  .$#.=..%..Q..L.n
-000009e0: e5d4 07e3 21c3 f424 15e9 c435 17fd 0c25  ....!..$...5...%
-000009f0: 53c8 ec59 c6c2 353c 4b33 e289 0d66 f24c  S..Y..5<K3...f.L
-00000a00: 6d6a 4d4c 2db4 2233 b6dd 388a 03c8 ded0  mjML-."3..8.....
-00000a10: a7fe 87ce de57 ae3f 3c2c a5ca 1c33 b164  .....W.?<,...3.d
-00000a20: 387d 8147 ec1d d904 9883 fbfb a4eb a077  8}.G...........w
-00000a30: 2c36 b0a7 8131 0189 5682 12cd 429e a105  ,6...1..V...B...
-00000a40: 8163 6976 944c 6c17 4561 6cf7 ce97 0f60  .civ.Ll.Eal....`
-00000a50: bf93 e16f bed8 57a7 7aff 6b82 450b 3d47  ...o..W.z.k.E.=G
-00000a60: b69b 7eed cb31 39ec 1e37 37fb 8d83 8d3e  ..~..19..77....>
-00000a70: 340a ff2e 9279 3ffc fadf 80f7 107d 49ce  4....y?......}I.
-00000a80: 0427 0f67 02c3 ef37 cb9b 33b1 d7f1 f2e9  .'.g...7..3.....
-00000a90: 3139 17bc b809 a2c5 01af ff63 76f6 b727  19.........cv..'
-00000aa0: c7de 73fa 70e7 f3bf 0100 00ff ff03 0050  ..s.p..........P
-00000ab0: 4b03 0414 0006 0008 0000 0021 003d 5880  K..........!.=X.
-00000ac0: 7a10 0100 00ee 0400 001a 0008 0178 6c2f  z............xl/
-00000ad0: 5f72 656c 732f 776f 726b 626f 6f6b 2e78  _rels/workbook.x
-00000ae0: 6d6c 2e72 656c 7320 a204 0128 a000 0100  ml.rels ...(....
+00000700: a338 147d 5f69 ff03 e29d 82f9 4a40 4d46  .8.}_i......J@MF
+00000710: 1040 5ba9 1d55 9d4c fb12 a972 c029 de02  .@[..U.L...r.)..
+00000720: 666d a749 55cd 7fdf 6b12 529a ac46 99ce  fm.IU...k.R..F..
+00000730: 4689 0df6 e1e4 dceb 732f 975f b675 a5bd  F.......s/._.u..
+00000740: 102e 286b 263a bab0 748d 3439 2b68 f334  ..(k&:..t.49+h.4
+00000750: d1bf cf33 63ac 6b42 e2a6 c015 6bc8 447f  ...3c.kB....k.D.
+00000760: 2542 ff32 fdf3 8fcb 0de3 cf4b c69e 3520  %B.2.......K..5 
+00000770: 68c4 442f a56c 43d3 1479 496a 2c2e 584b  h.D/.lC..yIj,.XK
+00000780: 1ad8 5931 5e63 09b7 fcc9 142d 27b8 1025  ..Y1^c.....-'..%
+00000790: 21b2 ae4c dbb2 7cb3 c6b4 d177 0c21 3f87  !..L..|....w.!?.
+000007a0: 83ad 5634 2709 cbd7 3569 e48e 8493 0a4b  ..V4'...5i.....K
+000007b0: 902f 4ada 8a9e adce cfa1 ab31 7f5e b746  ./J........1.^.F
+000007c0: ceea 1628 96b4 a2f2 b523 d5b5 3a0f af9e  ...(.....#..:...
+000007d0: 1ac6 f1b2 82b0 b7c8 d3b6 1cbe 3efc 9005  ............>...
+000007e0: 83dd ff13 6c9d fc55 4d73 ce04 5bc9 0ba0  ....l..UMs..[...
+000007f0: 3677 a24f e247 9689 d087 146c 4f73 701e  6w.O.G.....lOsp.
+00000800: 936b 72f2 42d5 191e 5471 ff93 aafc 0397  .kr.B...Tq......
+00000810: ff4e 86ac df66 4360 adce 2b21 24ef 936c  .N...fC`..+!$..l
+00000820: de41 9bad 4f2f 57b4 22f7 3beb 6ab8 6dbf  .A..O/W.".;.j.m.
+00000830: e25a 9d54 a56b 1516 322d a824 c544 1fc1  .Z.T.k..2-.$.D..
+00000840: 2ddb 900f 0b7c ddc6 6b5a c1ae edd9 b6a7  -....|..kZ......
+00000850: 9bd3 839d 6fb9 5690 155e 5772 0e46 eee9  ....o.V..^Wr.F..
+00000860: a132 7c3f d821 c118 5125 096f b024 33d6  .2|?.!..Q%.o.$3.
+00000870: 48f0 e13e aedf f5dc f412 b867 2503 876b  H..>.......g%..k
+00000880: 77e4 9f35 e504 0a0b fc05 b1c2 88f3 102f  w..5.........../
+00000890: c52d 96a5 b6e6 d544 9f85 8bef 02c2 5ffc  .-.....D......_.
+000008a0: 4d84 208b 8488 67c9 da45 fb2a 2aa8 bec3  M. ...g..E.**...
+000008b0: 4cb6 b86e 2b22 1603 c3e2 d3ea f805 cbe2  L..n+"..........
+000008c0: 5c65 cc3c 88dd 5d1f 2705 34f3 b0b7 e5ad  \e.<..].'.4.....
+000008d0: e41a 5c5f 25d7 7034 dff0 0b1c 14d8 a1d8  ..\_%.p4........
+000008e0: d7f1 159c 0472 1e9b 9c87 e8f1 6d14 2429  .....r......m.$)
+000008f0: 7293 c070 92c8 315c 0bc5 46e4 b989 1164  r..p..1\..F....d
+00000900: 599c 7ab6 1fa1 d4f9 01c1 703f cc19 5ecb  Y.z.......p?..^.
+00000910: 72ef 0145 3dd1 5d38 f093 ad1b bced 7790  r..E=.]8......w.
+00000920: 15ae 69f1 2ee3 cdda 7f0c 351f 0dfd de0f  ..i.......5.....
+00000930: 15b0 ea76 f794 6cc4 bb5b d4ad b67d a04d  ...v..l..[...}.M
+00000940: c136 5d44 affd b513 407c 9b6e e381 16b2  .6]D....@|.n....
+00000950: 04ab 8dc7 d661 ed2f 429f 4a50 8b3c 5bd5  .....a./B.JP.<[.
+00000960: 05ce 257d 2173 bc04 9892 6f2b 8d13 fd0d  ..%}!s....o+....
+00000970: d981 3bb6 8391 118f 10a4 c21b 3b46 3ccb  ..;.........;F<.
+00000980: 5c23 f1fc 28f3 bd28 8d12 afd3 660e c475  \#..(..(....f..u
+00000990: 1d16 4476 b3d6 7455 81a1 8bab c6db 655a  ..Dv..tU......eZ
+000009a0: d778 a8e8 f955 8154 6043 e072 0004 2907  .x...U.T`C.r..).
+000009b0: a07d 0ccc 0740 6700 748e 81c5 00e8 0e80  .}...@g.t.......
+000009c0: ee31 900c 80de 00d8 d5a7 d947 95e3 2a87  .1.........G..*.
+000009d0: 2255 5317 4c80 2c3b 5054 642b af85 ec66  "US.L.,;PTd+...f
+000009e0: a80f aab2 e75a d1c8 0a5c c34a 1dcf 70c7  .....Z...\.J..p.
+000009f0: 816d 8c5d c736 666e 62a7 de28 4dd2 18b2  .m.].6fnb..(M...
+00000a00: d737 a5ff a18d 7765 1af6 6f46 a5b2 c45c  .7....we..oF...\
+00000a10: ce39 ce9f e17d 7a47 5631 16e0 fc2e e926  .9...}zGV1.....&
+00000a20: e81d 8a8d bd71 6c39 20d1 cd50 66b8 28b0  .....ql9 ..Pf.(.
+00000a30: 8c38 f65d c34b 32c7 1ba1 6496 7ad9 bb58  .8.].K2...d.z..X
+00000a40: 15fe ea93 4d74 6c76 4f13 2cd7 d060 546f  ....MtlvO.,..`To
+00000a50: e9ee 4335 66fb d5c3 e26a b7b0 b7d1 8726  ..C5f....j.....&
+00000a60: 11de 252a effb a77f 06fc 06d1 57e4 4c70  ..%*........W.Lp
+00000a70: 767f 2670 f6f5 667e 7326 f63a 9d3f 3e64  v.&p..f~s&.:.?>d
+00000a80: e782 a39b 3889 f678 f33f b3b3 3b3d 3576  ....8..x.?..;=5v
+00000a90: 9e33 fb33 9ffe 0b00 00ff ff03 0050 4b03  .3.3.........PK.
+00000aa0: 0414 0006 0008 0000 0021 003d 5880 7a10  .........!.=X.z.
+00000ab0: 0100 00ee 0400 001a 0008 0178 6c2f 5f72  ...........xl/_r
+00000ac0: 656c 732f 776f 726b 626f 6f6b 2e78 6d6c  els/workbook.xml
+00000ad0: 2e72 656c 7320 a204 0128 a000 0100 0000  .rels ...(......
+00000ae0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000af0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ba0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000bb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000bc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000bd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000be0: 0000 0000 0000 0000 0000 0000 0000 00bc  ................
-00000bf0: 94dd 6a84 3010 85ef 0b7d 07c9 7d8d ba3f  ..j.0....}..}..?
-00000c00: 2d65 e3de 94c2 deb6 db07 083a 1a59 4d24  -e.........:.YM$
-00000c10: 33fd f1ed 3b08 ad15 96f4 46bc 094c 869c  3...;.....F..L..
-00000c20: f3e5 0cc9 e1f8 d5b5 d107 786c 9c55 228d  ..........xl.U".
-00000c30: 1311 812d 5cd9 d85a 89b7 f3f3 dd83 8890  ...-\..Z........
-00000c40: b42d 75eb 2c28 3100 8a63 7e7b 7378 8156  .-u.,(1..c~{sx.V
-00000c50: 131f 42d3 f418 b18a 4525 0c51 ff28 2516  ..B.....E%.Q.(%.
-00000c60: 063a 8db1 ebc1 72a7 72be d3c4 a5af 65af  .:....r.r.....e.
-00000c70: 8b8b ae41 6649 b297 feaf 86c8 679a d1a9  ...AfI......g...
-00000c80: 54c2 9f4a f63f 0f3d 3bff afed aaaa 29e0  T..J.?.=;.....).
-00000c90: c915 ef1d 58ba 6221 d168 0fe5 2b79 be1e  ....X.b!.h..+y..
-00000ca0: b2b0 f635 9012 b3ed 9889 85bc 0eb3 5912  ...5..........Y.
-00000cb0: e6d3 f90b 1a00 9a40 7eb7 9051 b9b3 09c1  .......@~..Q....
-00000cc0: dc2f 9a0c 0d2d 8f76 8a64 ac43 f6d9 ca59  ./...-.v.d.C...Y
-00000cd0: 6421 9874 6598 3404 b35f 1286 f829 c134  d!.te.4.._...).4
-00000ce0: 97b1 94e3 1a64 d8ad 1cc8 2e14 c876 6598  .....d.......ve.
-00000cf0: ed0f 8c9c fd52 f937 0000 00ff ff03 0050  .....R.7.......P
-00000d00: 4b03 0414 0006 0008 0000 0021 002d cb5c  K..........!.-.\
-00000d10: 0cf8 0200 0048 0700 0018 0000 0078 6c2f  .....H.......xl/
-00000d20: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
-00000d30: 312e 786d 6c9c d34b 6fa3 3010 00e0 fb4a  1.xml..Ko.0....J
-00000d40: fb1f 2cdf 8981 84b4 a090 2a2d 41db dbaa  ..,.......*-A...
-00000d50: eaee dd31 4362 c50f d676 5e5a ed7f df81  ...1Cb...v^Z....
-00000d60: 2869 a55c a24a 2006 2cbe 99c1 c3ec e9a8  (i.\.J .,.......
-00000d70: 15d9 83f3 d29a 9226 a398 1230 c236 d2ac  .......&...0.6..
-00000d80: 4bfa ebbd 8e1e 29f1 819b 862b 6ba0 a427  K.....)....+k..'
-00000d90: f0f4 69fe fddb ec60 ddd6 6f00 0241 c1f8  ..i....`..o..A..
-00000da0: 926e 42e8 0ac6 bcd8 80e6 7e64 3b30 b8d2  .nB.......~d;0..
-00000db0: 5aa7 79c0 5bb7 66be 73c0 9be1 25ad 581a  Z.y.[.f.s...%.X.
-00000dc0: c753 a6b9 34f4 2c14 ee1e c3b6 ad14 5059  .S..4.,.......PY
-00000dd0: b1d3 60c2 1971 a078 c0fa fd46 76fe a269  ..`..q.x...Fv..i
-00000de0: 710f a7b9 dbee ba48 58dd 21b1 924a 86d3  q......HX.!..J..
-00000df0: 8052 a245 f1ba 36d6 f195 c2be 8fc9 840b  .R.E..6.........
-00000e00: 7274 78a4 788e 2f69 86e7 3799 b414 ce7a  rtx.x./i..7....z
-00000e10: db86 11ca ec5c f36d fb39 cb19 1757 e9b6  .....\.m.9...W..
-00000e20: ffbb 9864 c21c ec65 bf81 1f54 fab5 9292  ...d...e...T....
-00000e30: ec6a a51f d8f8 8bd8 f48a f59f cb15 3bd9  .j............;.
-00000e40: 94f4 6f3e 7d9e 8cb3 c538 5a56 d534 9ad4  ..o>}....8ZV.4..
-00000e50: c963 9457 cb2c 7a58 bc3c c775 fe50 65cb  .c.W.,zX.<.u.Pe.
-00000e60: fa1f 9dcf 1a89 3bdc 7745 1cb4 255d 2445  ......;.wE..%]$E
-00000e70: 9551 369f 0df3 f35b c2c1 7f8a 493f 8e2b  .Q6....[....I?.+
-00000e80: 6bb7 fdc2 2ba6 8951 f0a0 40f4 8341 385e  k...+..Q..@..A8^
-00000e90: f6f0 024a 95f4 2dc9 71a4 ff0c 681f 23c9  ...J..-.q...h.#.
-00000ea0: aee6 e7f8 e2d7 c308 ff74 a481 96ef 5478  .........t....Tx
-00000eb0: b387 1f20 d79b 80ff 4b86 8df5 9351 34a7  ... ....K....Q4.
-00000ec0: 0abc c091 c4d4 a3b4 2ff4 3f00 0000 ffff  ......../.?.....
-00000ed0: 0000 00ff ff94 93dd 8e82 3010 855f 85f4  ..........0.._..
-00000ee0: 010a fddb aa29 4d16 7911 8224 5ea9 b184  .....)M.y..$^...
-00000ef0: dd7d fbed 3006 da51 13e9 05a1 9c93 33df  .}..0..Q......3.
-00000f00: 4c8b 0be7 6118 db6e ecbc bb5f 7f8a 7bcd  L...a..n..._..{.
-00000f10: 042b c2ad bb84 f876 d0ac f815 baeb 0fa7  .+.....v........
-00000f20: bf76 08fd 7019 6b56 7169 9877 3d78 bfa3  .v..p.kVqi.w=x..
-00000f30: 397e 0a71 3f79 e5ca c9bb b27f 684d aa55  9~.q?y......hM.U
-00000f40: b976 4c35 916b 6daa c945 2b23 dec2 28b7  .vL5.km..E+#..(.
-00000f50: 30ca 996e 4d9a c91b 88a8 597c 2efc 5f84  0..nM.....Y|.._.
-00000f60: f1d9 6108 2926 0b2e ed1b 4eb5 8553 bd9c  ..a.)&....N..S..
-00000f70: 2244 c0a1 c084 2517 d6ee d345 90d1 9c36  "D....%....E...6
-00000f80: a509 3216 8941 bb2a 5d6f f8e3 f97f 7e17  ..2..A.*]o....~.
-00000f90: f4cc 480a 3610 91cf d912 6874 6087 8aef  ..H.6.....ht`...
-00000fa0: 2b9d 36b8 23fc 5804 6c6b 4c76 35cc 1664  +.6.#.X.lkLv5..d
-00000fb0: b8c8 9327 c7da 4044 8e4c 288e e840 64c3  ...'..@D.L(..@d.
-00000fc0: ada2 537e e446 c5bc 6e06 91cb f5ef fb07  ..S~.F..n.......
-00000fd0: 0000 ffff 0000 00ff ffb2 2948 4c4f f54d  ..........)HLO.M
-00000fe0: 2c4a cfcc 2b56 c849 4d2b b155 32d0 3357  ,J..+V.IM+.U2.3W
-00000ff0: 5228 ca4c cf80 b14b f20b c0a2 a64a 0a49  R(.L...K.....J.I
-00001000: f925 25f9 b930 5e46 6a62 4a6a 1188 67ac  .%%..0^FjbJj..g.
-00001010: a490 969f 5f02 e3e8 dbd9 e897 e717 6517  ...._.........e.
-00001020: 67a4 a696 d801 0000 00ff ff03 0050 4b03  g............PK.
-00001030: 0414 0006 0008 0000 0021 0093 958a 80f4  .........!......
-00001040: 0200 0052 0700 0018 0000 0078 6c2f 776f  ...R.......xl/wo
-00001050: 726b 7368 6565 7473 2f73 6865 6574 322e  rksheets/sheet2.
-00001060: 786d 6c9c d351 6fb2 3014 06e0 fb2f d97f  xml..Qo.0..../..
-00001070: 687a 8f85 2a6e 1270 61a2 d9ee be2c dbee  hz..*n.pa....,..
-00001080: 6b39 4823 6d59 5ba7 66d9 7f5f c1a8 5bbc  k9H#mY[.f.._..[.
-00001090: 314b 2029 109e 730e 7d49 ef77 b241 1f60  1K )..s.}I.w.A.`
-000010a0: acd0 2ac3 d120 c408 14d7 a550 ab0c bfbe  ..*.. .....P....
-000010b0: 2c82 3b8c ac63 aa64 8d56 90e1 3d58 7c3f  ,.;..c.d.V..=X|?
-000010c0: bdf9 976e b559 db1a c021 2f28 9be1 dab9  ...n.Y...!/(....
-000010d0: 3621 c4f2 1a24 b303 dd82 f24f 2a6d 2473  6!...$.....O*m$s
-000010e0: fed2 ac88 6d0d b0b2 7f49 3684 86e1 9848  ....m....I6....H
-000010f0: 2614 3e08 89b9 c6d0 5525 3814 9a6f 2428  &.>.....U%8..o$(
-00001100: 7740 0c34 ccf9 fe6d 2d5a 7bd4 24bf 8693  w@.4...m-Z{.$...
-00001110: ccac 376d c0b5 6c3d b114 8d70 fb1e c548  ..7m..l=...p...H
-00001120: f2e4 69a5 b461 cbc6 cfbd 8b46 8ca3 9df1  ..i..a.....F....
-00001130: 07f5 e7f0 58a6 bf7f 5149 0a6e b4d5 951b  ....X...QI.n....
-00001140: 7899 1c7a be1c 7f42 2684 f193 7439 ff55  x..z...B&...t9.U
-00001150: 4c34 2206 3e44 b781 678a fead a528 3e59  L4".>D..g....(>Y
-00001160: f48c 0dff 888d 4f58 f7b9 4cb2 1165 863f  ......OX..L..e.?
-00001170: e734 9a47 743e 09e2 6248 8351 1cce 823c  .4.Gt>..bH.Q...<
-00001180: 5a8c 833c 7f28 66b7 e18c e693 db2f 3c4d  Z..<.(f....../<M
-00001190: 4be1 77b8 9b0a 19a8 329c 4749 1163 324d  K.w.....2.GI.c2M
-000011a0: fbfc bc09 d8da 1f6b d4c5 71a9 f5ba 7bf0  .......k..q...{.
-000011b0: e4cb 845e b0d0 00ef 8281 ecfb 6f83 9c90  ...^........o...
-000011c0: 697a 5e1f c145 9fd9 ff06 9550 b14d e39e  iz^..E.....P.M..
-000011d0: f5f6 11c4 aa76 fe07 89fd 245d 1492 725f  .....v....$]..r_
-000011e0: 80e5 3e83 bed6 8076 9d7d 0300 00ff ff00  ..>....v.}......
-000011f0: 0000 ffff 9493 5b6e 8330 1045 b782 bc00  ......[n.0.E....
-00001200: 835f 5047 c652 8937 8228 52bf 9228 46b4  ._PG.R.7.(R..(F.
-00001210: dd7d 67ec 041c 9746 810f 04dc abeb 330f  .}g....F......3.
-00001220: 8cff 1cc7 c9f5 536f cdf5 fc55 5c5b c248  ......So...U\[.H
-00001230: e12f fdc9 c3d3 4192 e29b c97e 387c fcb8  ./....A....~8|..
-00001240: d10f e369 6a49 45b9 22d6 0ce8 7d07 337c  ...ijIE."...}.3|
-00001250: f2f0 3e5b 61ca d99a 72b8 695d aa55 8fda  ..>[a...r.i].U..
-00001260: 31d5 d8a3 e652 8d2f 5a09 780b 23df c3c8  1....R./Z.x.#...
-00001270: 03dd 9a14 c83b 8c68 09dc 17fe 3a63 fceb  .....;.h....:c..
-00001280: 5019 694c 6694 37ff 708a 3d9c 62b3 8b18  P.iLf.7.p.=.b...
-00001290: 8143 c10e 73ca eb5a a757 861c cd69 513a  .C..s..Z.W...iQ:
-000012a0: 438e 8784 a0ed d6c2 c85f 1fbf 0c58 321b  C........_...X2.
-000012b0: 3c46 606b c352 50cd 9b67 c877 f33a 0796  <F`k.RP..g.w.:..
-000012c0: 2d8b 8ba7 08aa 6595 26bd 6d17 a0f6 1480  -.....e.&.m.....
-000012d0: 9b3c db6c ae1d 46dc 0b50 b411 aa4a ae6c  .<.l..F..P...J.l
-000012e0: cd8f d11c 0704 6655 a7e6 6ceb dced 3cb0  ......fU..l...<.
-000012f0: e9ed ccb8 e6e5 fa5b fe02 0000 ffff 0000  .......[........
-00001300: 00ff ffb2 2948 4c4f f54d 2c4a cfcc 2b56  ....)HLO.M,J..+V
-00001310: c849 4d2b b155 32d0 3357 5228 ca4c cf80  .IM+.U2.3WR(.L..
-00001320: b14b f20b c0a2 a64a 0a49 f925 25f9 b930  .K.....J.I.%%..0
-00001330: 5e46 6a62 4a6a 1188 67ac a490 969f 5f02  ^FjbJj..g....._.
-00001340: e3e8 dbd9 e897 e717 6517 67a4 a696 d801  ........e.g.....
-00001350: 0000 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
-00001360: 0000 0021 00fe acc9 e9d8 0200 0098 0600  ...!............
-00001370: 0018 0000 0078 6c2f 776f 726b 7368 6565  .....xl/workshee
-00001380: 7473 2f73 6865 6574 332e 786d 6c9c d3cb  ts/sheet3.xml...
-00001390: 8e9b 3014 06e0 7da5 7907 e43d 31b7 5c40  ..0...}.y..=1.\@
-000013a0: 21a3 4e48 d4d9 55a3 b67b c71c 8215 5f18  !.NH..U..{...._.
-000013b0: dbb9 a9ea bbf7 4094 cc48 d944 2381 3058  ......@..H.D#.0X
-000013c0: 7cc7 07ff cc9f 4f4a 0607 b04e 185d 9278  |.....OJ...N.].x
-000013d0: 1491 0034 37b5 d0db 92fc feb5 0e67 2470  ...47........g$p
-000013e0: 9ee9 9a49 a3a1 2467 70e4 79f1 f46d 7e34  ...I..$gp.y..m~4
-000013f0: 76e7 5a00 1fa0 a05d 495a efbb 8252 c75b  v.Z....]IZ...R.[
-00001400: 50cc 8d4c 071a 671a 6315 f378 6bb7 d475  P..L..g.c..xk..u
-00001410: 1658 3dbc a424 4da2 6842 1513 9a5c 84c2  .X=..$M.hB...\..
-00001420: 3e62 98a6 111c 2ac3 f70a b4bf 2016 24f3  >b....*..... .$.
-00001430: b87e d78a ce5d 35c5 1fe1 14b3 bb7d 1772  .~...]5......}.r
-00001440: a33a 2436 420a 7f1e 5012 285e bc6e b5b1  .:$6B...P.(^.n..
-00001450: 6c23 b1ef 539c 311e 9c2c 1e09 9ee9 b5cc  l#..S.1..,......
-00001460: f0fc ae92 12dc 1a67 1a3f 4299 5ed6 7cdf  .......g.?B.^.|.
-00001470: 7e4e 73ca f84d baef ff21 26ce a885 83e8  ~Ns..M...!&.....
-00001480: 37f0 834a beb6 a478 7cb3 920f 2cfd 2236  7..J...x|...,."6
-00001490: b961 fde7 b2c5 5ed4 25f9 9b4e abc9 729a  .a....^.%..N..r.
-000014a0: 4661 9ee6 b330 4bb2 2a9c add6 2f61 bc5e  Fa...0K.*.../a.^
-000014b0: 4d27 f9b8 5aae f2f8 1f59 cc6b 813b dc77  M'..Z....Y.k.;.w
-000014c0: 1558 684a f23d 2eaa 8cd0 c57c c8cf 1f01  .XhJ.=.....|....
-000014d0: 47f7 691c f471 dc18 b3eb 275e b14c 8482  G.i..q....'^.L..
-000014e0: 0309 bc0f 46c0 f072 8025 4859 9297 2926  ....F..r.%HY..)&
-000014f0: fa7d 3071 8820 bd89 9fc7 577d 3d04 f8a7  .}0q. ....W}=...
-00001500: 0d6a 68d8 5efa 3773 fc01 62db 7afc 5bc6  .jh.^.7s..b.z.[.
-00001510: d856 9f8b a23e 57e0 3806 120b 8f92 31aa  .V...>W.8.....1.
-00001520: ff01 0000 ffff 0000 00ff ff94 925b 0e83  .............[..
-00001530: 2010 45b7 6258 80f2 f219 3469 7123 849a   .E.bX....4iq#..
-00001540: f4cb 3662 6cbb fb0e d22a 129b 54be 807b  ..6bl....*..T..{
-00001550: 3373 e621 ccb5 ebc6 568d aa11 c3ed 110d  3s.!....V.......
-00001560: 3522 2832 77d5 1bb8 551c 454f c295 ae2e  5"(2w...U.EO....
-00001570: afb6 33ba ebc7 1ae1 98a6 a811 da7a 4f60  ..3..........zO`
-00001580: 862f 03ef a961 2299 1a91 e88f 76f6 35bc  ./...a".....v.5.
-00001590: d5a4 af91 add6 fa1a 5db4 04f0 1646 7a84  ........]....Fz.
-000015a0: 91ee d2d9 10b6 584b 4ee2 0c17 d83b 0192  ......XKN....;..
-000015b0: 7466 17c8 9a83 52db 55c9 f781 d911 6036  tf....R.U.....`6
-000015c0: 43f1 a09d 3644 8d5c 261a 3392 fbc0 6b9f  C...6D.\&.3...k.
-000015d0: e6b9 c8c0 ccc2 1ebb 1410 86fe 0086 c9ff  ................
-000015e0: bf05 7c06 4e03 601b e20b cc62 c203 5d3a  ..|.N.`....b..]:
-000015f0: dd4d 00f4 bc28 bd53 044b e152 80ad ccf6  .M...(.S.K.R....
-00001600: eb76 fb91 acfb fc06 0000 ffff 0000 00ff  .v..............
-00001610: ffb2 2948 4c4f f54d 2c4a cfcc 2b56 c849  ..)HLO.M,J..+V.I
-00001620: 4d2b b155 32d0 3357 5228 ca4c cf80 b14b  M+.U2.3WR(.L...K
-00001630: f20b c0a2 a64a 0a49 f925 25f9 b930 5e46  .....J.I.%%..0^F
-00001640: 6a62 4a6a 1188 67ac a490 969f 5f02 e3e8  jbJj..g....._...
-00001650: dbd9 e897 e717 6517 67a4 a696 d801 0000  ......e.g.......
-00001660: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
-00001670: 0021 008c 50f6 3fd7 0200 0098 0600 0018  .!..P.?.........
-00001680: 0000 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
-00001690: 2f73 6865 6574 342e 786d 6c9c d34b 6fa3  /sheet4.xml..Ko.
-000016a0: 3010 00e0 7ba5 fd0f 96ef c440 429a a090  0...{......@B...
-000016b0: 2a25 8db6 b76a b5bb 77c7 0cc1 8a1f aced  *%...j..w.......
-000016c0: bcb4 ea7f ef40 94b4 522e 5125 1003 16df  .....@..R.Q%....
-000016d0: cce0 61f6 74d4 8aec c179 694d 4193 414c  ..a.t....yiMA.AL
-000016e0: 0918 612b 6936 05fd f37b 154d 28f1 819b  ..a+i6...{.M(...
-000016f0: 8a2b 6ba0 a027 f0f4 69fe e361 76b0 6eeb  .+k..'..i..av.n.
-00001700: 1b80 4050 30be a04d 086d ce98 170d 68ee  ..@P0..M.m....h.
-00001710: 07b6 0583 2bb5 759a 07bc 751b e65b 07bc  ....+.u...u..[..
-00001720: ea5f d28a a571 3c66 9a4b 43cf 42ee ee31  ._...q<f.KC.B..1
-00001730: 6c5d 4b01 4b2b 761a 4c38 230e 140f 58bf  l]K.K+v.L8#...X.
-00001740: 6f64 eb2f 9a16 f770 9abb edae 8d84 d52d  od./...p.......-
-00001750: 126b a964 38f5 2825 5ae4 af1b 631d 5f2b  .k.d8.(%Z...c._+
-00001760: ecfb 988c b820 4787 478a e7f0 92a6 7f7e  ..... G.G......~
-00001770: 9349 4be1 acb7 7518 a0cc ce35 dfb6 3f65  .IK...u....5..?e
-00001780: 53c6 c555 baed ff2e 2619 3107 7bd9 6de0  S..U....&.1.{.m.
-00001790: 2795 7eaf a424 bb5a e927 36fc 2636 be62  '.~..$.Z.'6.&6.b
-000017a0: dde7 72f9 4e56 05fd 3f49 1e5f ca61 b98a  ..r.NV..?I._.a..
-000017b0: c6e3 9749 344a 978b e839 5b94 d173 3c7d  ...I4J...9[..s<}
-000017c0: 9c2e ca2c c9ca c93b 9dcf 2a89 3bdc 7545  ...,...;..*.;.uE
-000017d0: 1cd4 055d 24f9 7244 d97c d6cf cf5f 0907  ...]$.rD.|..._..
-000017e0: ff25 26dd 38ae addd 760b af98 2646 c183  .%&.8...v...&F..
-000017f0: 02d1 0d06 e178 d943 094a 15b4 cc70 a2ff  .....x.C.J...p..
-00001800: f526 8608 b2ab f835 bee8 ab7e 80df 1ca9  .&.....5...~....
-00001810: a0e6 3b15 7ed9 c34f 909b 26e0 df82 52bf  ..;.~..O..&...R.
-00001820: ff79 755a 8217 3890 9878 9076 ea07 0000  .yuZ..8..x.v....
-00001830: 00ff ff00 0000 ffff 9492 5b0e 8320 1045  ..........[.. .E
-00001840: b762 5880 08e2 3348 52eb 468c 35e9 976d  .bX...3HR.F.5..m
-00001850: c4d8 76f7 1d9c 5690 98a6 f285 9ef1 7a18  ..v...V.......z.
-00001860: 46ea 6bdf 4f4d 3bb5 4a8e b747 3056 8491  F.k.OM;.J..G0V..
-00001870: 40df db41 c3ae 1424 7832 d176 e5e5 d5f4  @..A...$x2.v....
-00001880: baeb 87a9 2251 c813 a264 676a 4f50 0caf  ...."Q...dgjOP..
-00001890: 343c cf2a 9674 5692 761f 56bb 2cda b2b3  4<.*.tV.v.V.,...
-000018a0: cbd8 9635 2ee3 2ba3 a0b7 3af2 238e 7cd7  ...5..+...:.#.|.
-000018b0: ce44 5444 2c8c 8549 9179 86c8 f15b c3d3  .DTD,..I.y...[..
-000018c0: c859 beb2 2db3 311b e1f8 8870 bc48 09af  .Y..-.1....p.H..
-000018d0: 9d26 a222 c878 9864 be30 7234 019e 8b5f  .&.".x.d.0r4..._
-000018e0: c26b 4c9e ec77 186e feff 29c0 2eda a465  .kL..w.n..)....e
-000018f0: 366a 13f1 1516 3034 71e1 acd4 6b37 1633  6j....04q...k7.3
-00001900: 3c79 c853 e116 7b47 6df0 7f90 99da 186c  <y.S..{Gm......l
-00001910: 37b5 f3fc 0600 00ff ff00 0000 ffff b229  7..............)
-00001920: 484c 4ff5 4d2c 4acf cc2b 56c8 494d 2bb1  HLO.M,J..+V.IM+.
-00001930: 5532 d033 5752 28ca 4ccf 80b1 4bf2 0bc0  U2.3WR(.L...K...
-00001940: a2a6 4a0a 49f9 2525 f9b9 305e 466a 624a  ..J.I.%%..0^FjbJ
-00001950: 6a11 8867 aca4 9096 9f5f 02e3 e8db d9e8  j..g....._......
-00001960: 97e7 1765 1767 a4a6 96d8 0100 0000 ffff  ...e.g..........
-00001970: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
-00001980: cb1d 3c24 de02 0000 a806 0000 1800 0000  ..<$............
-00001990: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
-000019a0: 6565 7435 2e78 6d6c 9c92 5b6f e230 1085  eet5.xml..[o.0..
-000019b0: df57 ea7f b0fc 1e9c 8400 4d44 a868 01b5  .W........MD.h..
-000019c0: 6fab eee5 dd38 1362 e14b d636 37ad f6bf  o....8.b.K.67...
-000019d0: ef24 085a 8917 5429 91c6 13fb 3b73 e233  .$.Z..T)....;s.3
-000019e0: 7d3a 6a45 f6e0 bcb4 a6a4 c920 a604 8cb0  }:jE....... ....
-000019f0: 9534 9b92 fefa b98a 1e29 f181 9b8a 2b6b  .4.......)....+k
-00001a00: a0a4 27f0 f469 f6f0 6d7a b06e eb1b 8040  ..'..i..mz.n...@
-00001a10: 9060 7c49 9b10 da82 312f 1ad0 dc0f 6c0b  .`|I....1/....l.
-00001a20: 06bf d4d6 691e 70e9 36cc b70e 78d5 1fd2  ....i.p.6...x...
-00001a30: 8aa5 713c 669a 4b43 cf84 c2dd c3b0 752d  ..q<f.KC......u-
-00001a40: 052c acd8 6930 e10c 71a0 78c0 f97d 235b  .,..i0..q.x..}#[
-00001a50: 7fa1 6971 0f4e 73b7 ddb5 91b0 ba45 c45a  ..iq.Ns......E.Z
-00001a60: 2a19 4e3d 9412 2d8a b78d b18e af15 fa3e  *.N=..-........>
-00001a70: 2619 17e4 e8f0 49f1 1d5e 64fa fe8d 9296  &.....I..^d.....
-00001a80: c259 6feb 3040 323b cf7c 6b3f 6739 e3e2  .Yo.0@2;.|k?g9..
-00001a90: 4aba f57f 1726 c998 83bd ec2e f003 957e  J....&.........~
-00001aa0: 6da4 6474 65a5 1fb0 e117 61e3 2bac fb5d  m.dte.....a.+..]
-00001ab0: aed8 c9aa a47f 47f3 799e 4d96 9368 98ae  ......G.y.M..h..
-00001ac0: 9ea3 2cce 9328 9f3f e6d1 643c 1e67 cb38  ..,..(.?..d<.g.8
-00001ad0: cee3 e5cb 3f3a 9b56 126f b873 451c d425  ....?:.V.o.sE..%
-00001ae0: 9d27 c522 a36c 36ed f3f3 5bc2 c17f aa49  .'.".l6...[....I
-00001af0: e0eb 1fa0 4004 408d 8492 2e9e 6b6b b7dd  ....@.@.....kk..
-00001b00: c637 6cc5 48f4 fd86 8ec8 4590 7b78 01a5  .7l.H.....E.{x..
-00001b10: 4afa 9a63 c2ff f41a 58a2 00bb 2a7c ae2f  J..c....X...*|./
-00001b20: 6aab 3ed0 df1d a9a0 e63b 15de ede1 15e4  j.>......;......
-00001b30: a609 283b 429b 5d4e 8aea b400 2f30 a028  ..(;B.]N..../0.(
-00001b40: 3c48 4748 fd0f 0000 ffff 0000 00ff ff94  <HGH............
-00001b50: 925b 0e82 3010 45b7 42ba 80be 2b42 0a89  .[..0.E.B...+B..
-00001b60: c246 0836 f10b 8d25 a8bb 774a 114a 438c  .F.6...%..wJ.JC.
-00001b70: f40b 3837 d333 c368 7b35 a6af 9bbe 29f5  ..87.3.h{5....).
-00001b80: e3f6 4c1e 0562 28b1 f7a6 b3f0 944b 94bc  ..L..b(......K..
-00001b90: 986c dafc f2ae 8d6d 4dd7 1788 62ae 50a9  .l.....mM...b.P.
-00001ba0: 5b97 3d41 183e 5978 1f4a a1c9 506a d24e  [.=A.>Yx.J..Pj.N
-00001bb0: ec1c 32ba 6655 c8d8 9ad5 21e3 3323 a037  ..2.fU....!.3#.7
-00001bc0: 3bf2 3d8e 7cd3 ce95 2890 1c19 c754 b22c  ;.=.|...(....T.,
-00001bd0: 38c7 48d7 877d 2108 8b43 a4bc 4556 c262  8.H..}!..C..EV.b
-00001be0: 8fb0 18a5 6434 4e57 a240 9e09 9cd2 c8a1  ....d4NW.@......
-00001bf0: f27c 6a16 a72c a5c1 8967 3c97 614b ab2b  .|j..,...g<.aK.+
-00001c00: 61f8 f3ff 6f81 9fa2 8a84 5d89 afb0 c24a  a...o.....]....J
-00001c10: 8a1f 4295 0fb3 b173 08ab 78c2 d315 40b2  ..B....s..x...@.
-00001c20: b04c bc1f 64d9 e70f 0000 00ff ff00 0000  .L..d...........
-00001c30: ffff b229 484c 4ff5 4d2c 4acf cc2b 56c8  ...)HLO.M,J..+V.
-00001c40: 494d 2bb1 5532 d033 5752 28ca 4ccf 80b1  IM+.U2.3WR(.L...
-00001c50: 4bf2 0bc0 a2a6 4a0a 49f9 2525 f9b9 305e  K.....J.I.%%..0^
-00001c60: 466a 624a 6a11 8867 aca4 9096 9f5f 02e3  FjbJj..g....._..
-00001c70: e8db d9e8 97e7 1765 1767 a4a6 96d8 0100  .......e.g......
-00001c80: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
-00001c90: 0000 2100 c117 10be 4e07 0000 c620 0000  ..!.....N.... ..
-00001ca0: 1300 0000 786c 2f74 6865 6d65 2f74 6865  ....xl/theme/the
-00001cb0: 6d65 312e 786d 6cec 59cd 8b1b 3714 bf17  me1.xml.Y...7...
-00001cc0: fa3f 0c73 77fc 35e3 8f25 dee0 cf6c 93dd  .?.sw.5..%...l..
-00001cd0: 2464 9d94 1cb5 b6ec 5156 3332 92bc 1b13  $d......QV32....
-00001ce0: 0225 39f5 5228 a4a5 9742 6f3d 94d2 4003  .%9.R(...Bo=..@.
-00001cf0: 0dbd f48f 0924 b4e9 1fd1 27cd d823 ade5  .....$....'..#..
-00001d00: 249b 6c4a 5a76 0d8b 47fe bda7 a7f7 9e7e  $.lJZv..G......~
-00001d10: 7af3 74f1 d2bd 987a 4798 0bc2 9296 5fbe  z.t....zG....._.
-00001d20: 50f2 3d9c 8cd8 9824 d396 7f6b 3828 347c  P.=....$...k8(4|
-00001d30: 4f48 948c 1165 096e f90b 2cfc 4bdb 9f7e  OH...e.n..,.K..~
-00001d40: 7211 6dc9 08c7 d803 f944 6ca1 961f 4939  r.m......Dl...I9
-00001d50: db2a 16c5 0886 91b8 c066 3881 df26 8cc7  .*.......f8..&..
-00001d60: 48c2 239f 16c7 1c1d 83de 9816 2ba5 52ad  H.#.........+.R.
-00001d70: 1823 92f8 5e82 6250 7b7d 3221 23ec 0d95  .#..^.bP{}2!#...
-00001d80: 4a7f 7ba9 bc4f e131 9142 0d8c 28df 57aa  J.{..O.1.B..(.W.
-00001d90: b125 a1b1 e3c3 b242 8885 e852 ee1d 21da  .%.....B...R..!.
-00001da0: f261 9e31 3b1e e27b d2f7 2812 127e 68f9  .a.1;..{..(..~h.
-00001db0: 25fd e717 b72f 16d1 5626 44e5 0659 436e  %..../..V&D..YCn
-00001dc0: a0ff 32b9 4c60 7c58 d173 f2e9 c16a d220  ..2.L`|X.s...j. 
-00001dd0: 0883 5a7b a55f 03a8 5cc7 f5eb fd5a bfb6  ..Z{._..\....Z..
-00001de0: d2a7 0168 3482 95a6 b6d8 3aeb 956e 9061  ...h4.....:..n.a
-00001df0: 0d50 fad5 a1bb 57ef 55cb 16de d05f 5db3  .P....W.U...._].
-00001e00: b91d aa8f 85d7 a054 7fb0 861f 0cba e045  .......T.......E
-00001e10: 0baf 4129 3e5c c387 9d66 a767 ebd7 a014  ..A)>\...f.g....
-00001e20: 5f5b c3d7 4bed 5e50 b7f4 6b50 4449 72b8  _[..K.^P..kPDIr.
-00001e30: 862e 85b5 6a77 b9da 1564 c2e8 8e13 de0c  ....jw...d......
-00001e40: 8341 bd92 29cf 5190 0dab ec52 534c 5822  .A..).Q....RSLX"
-00001e50: 37e5 5a8c ee32 3e00 8002 5224 49e2 c9c5  7.Z..2>...R$I...
-00001e60: 0c4f d008 b2b8 8b28 39e0 c4db 25d3 0812  .O.....(9...%...
-00001e70: 6f86 1226 60b8 5429 0d4a 55f8 af3e 81fe  o..&`.T).JU..>..
-00001e80: a623 8ab6 3032 a495 5d60 8958 1b52 f678  .#..02..]`.X.R.x
-00001e90: 62c4 c94c b6fc 2ba0 d537 202f 9e3d 7bfe  b..L..+..7 /.={.
-00001ea0: f0e9 f387 bf3d 7ff4 e8f9 c35f b2b9 b52a  .....=....._...*
-00001eb0: 4b6e 0725 5353 eed5 8f5f fffd fd17 de5f  Kn.%SS..._....._
-00001ec0: bffe f0ea f137 e9d4 27f1 c2c4 bffc f9cb  .....7..'.......
-00001ed0: 97bf fff1 3af5 b0e2 dc15 2fbe 7df2 f2e9  ....:...../.}...
-00001ee0: 9317 df7d f5e7 4f8f 1dda db1c 1d98 f021  ...}..O........!
-00001ef0: 89b1 f0ae e163 ef26 8b61 810e fbf1 013f  .....c.&.a.....?
-00001f00: 9dc4 3042 c492 4011 e876 a8ee cbc8 025e  ..0B..@..v.....^
-00001f10: 5b20 eac2 75b0 edc2 db1c 58c6 05bc 3cbf  [ ..u.....X...<.
-00001f20: 6bd9 ba1f f1b9 248e 99af 46b1 05dc 638c  k.....$...F...c.
-00001f30: 7618 773a e0aa 9acb f0f0 709e 4cdd 93f3  v.w:......p.L...
-00001f40: b989 bb89 d091 6bee 2e4a ac00 f7e7 33a0  ......k..J....3.
-00001f50: 57e2 52d9 8db0 65e6 0d8a 1289 a638 c1d2  W.R...e......8..
-00001f60: 53bf b143 8c1d abbb 4388 e5d7 3d32 e24c  S..C....C...=2.L
-00001f70: b089 f4ee 10af 8388 d325 4372 6025 522e  .........%Cr`%R.
-00001f80: b443 6288 cbc2 6520 84da f2cd de6d afc3  .Cb...e .....m..
-00001f90: a86b d53d 7c64 2361 5b20 ea30 7e88 a9e5  .k.=|d#a[ .0~...
-00001fa0: c6cb 682e 51ec 5239 4431 351d be8b 64e4  ..h.Q.R9D15...d.
-00001fb0: 3272 7fc1 4726 ae2f 2444 7a8a 29f3 fa63  2r..G&./$Dz.)..c
-00001fc0: 2c84 4be6 3a87 f51a 41bf 0a0c e30e fb1e  ,.K.:...A.......
-00001fd0: 5dc4 3692 4b72 e8d2 b98b 1833 913d 76d8  ].6.Kr.....3.=v.
-00001fe0: 8d50 3c73 da4c 92c8 c47e 260e 2145 9177  .P<s.L...~&.!E.w
-00001ff0: 8349 177c 8fd9 3b44 3d43 1c50 b231 dcb7  .I.|..;D=C.P.1..
-00002000: 09b6 c2fd 6622 b805 e46a 9a94 2788 fa65  ....f"...j..'..e
-00002010: ce1d b1bc 8c99 bd1f 1774 82b0 8b65 da3c  .........t...e.<
-00002020: b6d8 b5cd 8933 3b3a f3a9 95da bb18 5374  .....3;:......St
-00002030: 8cc6 187b b73e 7358 d061 33cb e7b9 d157  ...{.>sX.a3....W
-00002040: 2260 951d ec4a ac2b c8ce 55f5 9c60 0165  "`...J.+..U..`.e
-00002050: 92aa 6bd6 2972 9708 2b65 f7f1 946d b067  ..k.)r..+e...m.g
-00002060: 6f71 8278 1628 8911 dfa4 f91a 44dd 4a5d  oq.x.(......D.J]
-00002070: 38e5 9c54 7a9d 8e0e 4de0 3502 e51f e48b  8..Tz...M.5.....
-00002080: d329 d705 e830 92bb bf49 eb8d 0859 6797  .)...0...I...Yg.
-00002090: 7a16 ee7c 5d70 2b7e 6fb3 c760 5fde 3ded  z..|]p+~o..`_.=.
-000020a0: be04 197c 6a19 20f6 b7f6 cd10 516b 823c  ...|j. .....Qk.<
-000020b0: 6186 080a 0c17 dd82 8815 fe5c 449d ab5a  a..........\D..Z
-000020c0: 6cee 949b d89b 360f 0314 4656 bd13 93e4  l.....6...FV....
-000020d0: 8dc5 cf89 b227 fc77 ca1e 7701 7306 058f  .....'.w..w.s...
-000020e0: 5bf1 fb94 3a9b 2865 e744 81b3 09f7 1f2c  [...:.(e.D.....,
-000020f0: 6b7a 689e dcc0 7092 ac73 d679 5573 5ed5  kzh...p..s.yUs^.
-00002100: f8ff fbaa 66d3 5e3e af65 ce6b 99f3 5ac6  ....f.^>.e.k..Z.
-00002110: f5f6 f541 6a99 bc7c 81ca 26ef f2e8 9e4f  ...Aj..|..&....O
-00002120: bcb1 e533 2194 eecb 05c5 bb42 777d 04bc  ...3!......Bw}..
-00002130: d18c 0730 a8db 51ba 27b9 6a01 ce22 f89a  ...0..Q.'.j.."..
-00002140: 3598 2cdc 9423 2de3 7126 3f27 32da 8fd0  5.,..#-.q&?'2...
-00002150: 0c5a 4365 ddc0 9c8a 4cf5 5478 3326 a063  .ZCe....L.Tx3&.c
-00002160: a487 752b 159f d0ad fb4e f378 8f8d d34e  ..u+.....N.x...N
-00002170: 67b9 acba 9aa9 0b05 92f9 7829 5c8d 4397  g.........x)\.C.
-00002180: 4aa6 e85a 3def dead d4eb 7ee8 5477 5997  J..Z=.....~.TwY.
-00002190: 0628 d9d3 1861 4c66 1b51 7518 515f 0e42  .(...aLf.Qu.Q_.B
-000021a0: 145e 6784 5ed9 9958 d174 58d1 50ea 97a1  .^g.^..X.tX.P...
-000021b0: 5a46 71e5 0a30 6d15 1578 e5f6 e045 bde5  ZFq..0m..x...E..
-000021c0: 8741 da41 8666 1c94 e763 15a7 b499 bc8c  .A.A.f...c......
-000021d0: ae0a ce99 467a 9333 a999 0150 622f 3320  ....Fz.3...Pb/3 
-000021e0: 8f74 53d9 ba71 796a 7569 aabd 45a4 2d23  .tS..qyjui..E.-#
-000021f0: 8c74 b38d 30d2 3082 17e1 2c3b cd96 fb59  .t..0.0...,;...Y
-00002200: c6ba 9987 d432 4fb9 62b9 1b72 33ea 8d0f  .....2O.b..r3...
-00002210: 116b 4522 27b8 8126 2653 d0c4 3b6e f9b5  .kE"'..&&S..;n..
-00002220: 6a08 b72a 2334 6bf9 13e8 18c3 d778 06b9  j..*#4k......x..
-00002230: 23d4 5b17 a253 b876 1949 9e6e f877 6196  #.[..S.v.I.n.wa.
-00002240: 1917 b287 4494 3a5c 934e ca06 3191 987b  ....D.:\.N..1..{
-00002250: 94c4 2d5f 2d7f 950d 34d1 1ca2 6d2b 5780  ..-_-...4...m+W.
-00002260: 103e 5ae3 9a40 2b1f 9b71 1074 3bc8 7832  .>Z..@+..q.t;.x2
-00002270: c123 6986 dd18 519e 4e1f 81e1 53ae 70fe  .#i...Q.N...S.p.
-00002280: aac5 df1d ac24 d91c c2bd 1f8d 8fbd 033a  .....$.........:
-00002290: e737 11a4 5858 2f2b 078e 8980 8b83 72ea  .7..XX/+......r.
-000022a0: cd31 819b b015 91e5 f977 e260 ca68 d7bc  .1.......w.`.h..
-000022b0: 8ad2 3994 8e23 3a8b 5076 a298 649e c235  ..9..#:.Pv..d..5
-000022c0: 89ae ccd1 4f2b 1f18 4fd9 9ac1 a1eb 2e3c  ....O+..O......<
-000022d0: 98aa 03f6 bd4f dd37 1fd5 ca73 0669 e667  .....O.7...s.i.g
-000022e0: a6c5 2aea d474 93e9 873b e40d abf2 43d4  ..*..t...;....C.
-000022f0: b22a a56e fd4e 2d72 ae6b 2eb9 0e12 d579  .*.n.N-r.k.....y
-00002300: 4abc e1d4 7d8b 03c1 302d 9fcc 324d 59bc  J...}...0-..2MY.
-00002310: 4ec3 8ab3 b351 dbb4 332c 080c 4fd4 36f8  N....Q..3,..O.6.
-00002320: 6d75 4638 3df1 ae27 3fc8 9dcc 5a75 402c  muF8=..'?...Zu@,
-00002330: eb4a 9df8 faca dcbc d566 0777 813c 7a70  .J.......f.w.<zp
-00002340: 7f38 a752 e850 426f 9723 28fa d21b c894  .8.R.PBo.#(.....
-00002350: 3660 8bdc 9359 8d08 dfbc 3927 2dff 7e29  6`...Y....9'-.~)
-00002360: 6c07 dd4a d82d 941a 61bf 1054 8352 a111  l..J.-..a..T.R..
-00002370: b6ab 8576 1856 cbfd b05c ea75 2a0f e060  ...v.V...\.u*..`
-00002380: 9151 5c0e d3eb fa01 5c61 d045 7669 afc7  .Q\.....\a.Evi..
-00002390: d72e eee3 e52d cd85 118b 8b4c 5fcc 17b5  .....-.....L_...
-000023a0: e1fa e2be 5cd9 7c71 ef11 209d fbb5 caa0  ....\.|q.. .....
-000023b0: 596d 766a 8566 b53d 2804 bd4e a3d0 ecd6  Ymvj.f.=(..N....
-000023c0: 3a85 5ead 5bef 0d7a ddb0 d11c 3cf0 bd23  :.^.[..z....<..#
-000023d0: 0d0e dad5 6e50 eb37 0ab5 72b7 5b08 6a25  ....nP.7..r.[.j%
-000023e0: 657e a359 a807 954a 3ba8 b71b fda0 fd20  e~.Y...J;...... 
-000023f0: 2b63 60e5 297d 64be 00f7 6abb b6ff 0100  +c`.)}d...j.....
-00002400: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
-00002410: 0021 008c 0545 6718 0300 00ba 0800 000d  .!...Eg.........
-00002420: 0000 0078 6c2f 7374 796c 6573 2e78 6d6c  ...xl/styles.xml
-00002430: c456 db8e d330 107d 47e2 1f2c bf67 9d64  .V...0.}G..,.g.d
-00002440: 9bd2 5649 10dd 6e24 2458 21ed 22f1 ea26  ..VI..n$$X!."..&
-00002450: 4e6b e14b 709c 2505 f1ef 8c9d b4cd 0ac4  Nk.Kp.%.........
-00002460: 6517 8997 c61e 8f8f cfcc 9cb1 9bbe eca5  e...............
-00002470: 40f7 ccb4 5cab 0c47 1721 464c 95ba e26a  @...\..G.!FL...j
-00002480: 97e1 f777 45b0 c0a8 b554 5554 68c5 327c  ...wE....TUTh.2|
-00002490: 602d 7e99 3f7f 96b6 f620 d8ed 9e31 8b00  `-~.?.... ...1..
-000024a0: 42b5 19de 5bdb ac08 69cb 3d93 b4bd d00d  B...[...i.=.....
-000024b0: 53b0 526b 23a9 85a9 d991 b631 8c56 addb  S.Rk#......1.V..
-000024c0: 2405 89c3 704e 24e5 0a0f 082b 59fe 0988  $...pN$....+Y...
-000024d0: a4e6 63d7 04a5 960d b57c cb05 b707 8f85  ..c......|......
-000024e0: 912c 57af 774a 1bba 1540 b58f 66b4 447d  .,W.wJ...@..f.D}
-000024f0: 3437 31ea cdf1 106f fde1 1cc9 4ba3 5b5d  471....o....K.[]
-00002500: db0b c025 baae 79c9 7ea4 bb24 4b42 cb33  ...%..y.~..$KB.3
-00002510: 1220 3f0e 294a 4818 3f88 bd37 8f44 9a11  . ?.)JH.?..7.D..
-00002520: c3ee b92b 1fce 53d5 c942 da16 95ba 5316  ...+..S..B....S.
-00002530: ca79 32a1 61e5 7505 c6f9 0ca3 a12a 57ba  .y2.a.u......*W.
-00002540: 823c 8517 6118 6292 a764 dc9e a7b5 5653  .<..a.b..d....VS
-00002550: 1448 22a4 72f5 51e9 cfaa 704b 03b4 f3ca  .H".r.Q...pK....
-00002560: d3f6 0bba a702 2c91 c328 b5d0 0659 9000  ......,..(...Y..
-00002570: 207b 8ba2 920d 1e57 54f0 ade1 cead a692   {.....WT.......
-00002580: 8bc3 608e 9dc1 ab66 f493 1c6a e809 0d27  ..`....f...j...'
-00002590: 104f 0736 7121 4eb1 c510 9b33 e429 c8c0  .O.6q!N....3.)..
-000025a0: 32a3 0a98 a071 7c77 68e0 7805 8a1d 60bc  2....q|wh.x...`.
-000025b0: df6f bc77 861e a238 996c 20fe c03c dd6a  .o.w...8.l ..<.j
-000025c0: 5341 874c b33a 98f2 54b0 da02 7bc3 777b  SA.L.:..T...{.w{
-000025d0: f7b5 ba81 dfad b616 5494 a715 a73b ada8  ........T....;..
-000025e0: 70b9 3dee 1807 2da4 8a09 71eb bae8 43fd  p.=...-...q...C.
-000025f0: 00bb af27 d582 7e74 d1bb c2b9 2104 320e  ...'..~t....!.2.
-00002600: 07bc 61e2 f0a7 6803 f604 3681 64fd 3d2c  ..a...h...6.d.=,
-00002610: eaeb 13fe 1376 23da 34e2 f04a f09d 92ec  .....v#.4..J....
-00002620: 284b 90c2 3045 7b6d f817 08d1 69c8 e7d1  (K..0E{m....i...
-00002630: 57a0 af9f c418 7dea b465 ef0c ab79 ef74  W.....}..e...y.t
-00002640: f86f 388c adf3 bb72 9cf2 f673 1637 9ddc  .o8....r...s.7..
-00002650: 3253 f87b f13f 72f3 55f9 675c bcfe 4071  2S.{.?r.U.g\..@q
-00002660: 1359 3f10 f549 9ec8 dd07 19be 71e1 0bb8  .Y?..I......q...
-00002670: 4a47 89a1 6dc7 85e5 ea27 8206 ccaa 3fb7  JG..m....'....?.
-00002680: 88bf aaac bbe2 7df3 9c4e 81f6 a858 4d3b  ......}..N...XM;
-00002690: 61ef 4e8b 193e 8fdf b28a 7732 3e79 bde3  a.N..>....w2>y..
-000026a0: f7da 7a88 0c9f c76f 5c27 4773 a741 d6db  ..z....o\'Gs.A..
-000026b0: 372d 5c70 f045 9de1 19fe 7abd 7eb1 dc5c  7-\p.E....z.~..\
-000026c0: 1771 b008 d78b 6076 c992 6099 ac37 4132  .q....`v..`..7A2
-000026d0: bb5a 6f36 c532 8cc3 ab6f 9387 e609 cf8c  .Zo6.2...o......
-000026e0: 7f17 a105 a2d9 aa15 f018 9931 d831 c4db  ...........1.1..
-000026f0: b32d c393 c940 df77 10d0 9e72 5fc6 f3f0  .-...@.w...r_...
-00002700: 5512 8541 7119 46c1 6c4e 17c1 627e 9904  U..Aq.F.lN..b~..
-00002710: 4512 c59b f96c 7d9d 14c9 847b f2c8 e728  E....l}....{...(
-00002720: 2451 343c 6c8e 7cb2 b25c 32c1 d5b1 56c7  $Q4<l.|..\2...V.
-00002730: 0a4d ad50 2498 fe22 0872 ac04 39ff e9c8  .M.P$..".r..9...
-00002740: bf03 0000 ffff 0300 504b 0304 1400 0600  ........PK......
-00002750: 0800 0000 2100 2e8e 9c7c dc00 0000 8d01  ....!....|......
-00002760: 0000 1400 0000 786c 2f73 6861 7265 6453  ......xl/sharedS
-00002770: 7472 696e 6773 2e78 6d6c 6cd0 c16a c330  trings.xmll..j.0
-00002780: 0c06 e0fb 60ef 6074 9f1d bb2c 4d86 e31e  ....`.`t...,M...
-00002790: 0a63 f76e 0f60 62af 3124 726a 3963 79fb  .c.n.`b.1$rj9cy.
-000027a0: 79f4 3048 76d4 a75f 1248 9fbe a791 7df9  y.0Hv.._.H....}.
-000027b0: 4421 6207 9257 c03c f6d1 05bc 76f0 f1fe  D!b..W.<....v...
-000027c0: fad4 00a3 6cd1 d931 a2ef 60f5 0427 f3f8  ....l..1..`..'..
-000027d0: a089 322b b348 1d0c 39cf 2f42 503f f8c9  ..2+.H..9./BP?..
-000027e0: 128f b3c7 d2f9 8c69 b2b9 94e9 2a68 4ede  .......i....*hN.
-000027f0: 3a1a bccf d328 5455 d562 b201 81f5 71c1  :....(TU.b....q.
-00002800: dc81 6a81 2d18 6e8b 3fdf 414a 309a 82d1  ..j.-.n.?.AJ0...
-00002810: d9cc eb65 2c2b b5c8 468b 5fba f3db 9a7a  ...e,+..F._....z
-00002820: 8b5b bd8c c1ed a2c9 bab0 d036 aab8 6caa  .[.........6..l.
-00002830: 2d4a ae8e f23f dc25 0fbc ad76 f8cc 8fb2  -J...?.%...v....
-00002840: d91f 5275 bdc5 327e 68ff 5094 779a 1f00  ..Ru..2~h.P.w...
-00002850: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
-00002860: 0000 2100 ca5c a8f7 4401 0000 5b02 0000  ..!..\..D...[...
-00002870: 1100 0801 646f 6350 726f 7073 2f63 6f72  ....docProps/cor
-00002880: 652e 786d 6c20 a204 0128 a000 0100 0000  e.xml ...(......
-00002890: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000028a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000028b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000028c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000028d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000028e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000028f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002900: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002910: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002920: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002930: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002940: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002950: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002960: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002970: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002980: 0000 0000 0000 0000 0000 0000 008c 9251  ...............Q
-00002990: 4bc3 3014 85df 05ff 43c9 7b9b a6dd c60c  K.0.....C.{.....
-000029a0: 6d07 2a7b 1007 8215 c5b7 90dc 6dc5 260d  m.*{........m.&.
-000029b0: 49b4 dbbf 376d b75a 990f 3ee6 9e73 bf7b  I...7m.Z..>..s.{
-000029c0: ee25 d9ea 20eb e00b 8cad 1a95 2312 c528  .%.. .......#..(
-000029d0: 00c5 1b51 a95d 8e5e ca75 b844 8175 4c09  ...Q.].^.u.D.uL.
-000029e0: 5637 0a72 7404 8b56 c5f5 55c6 35e5 8d81  V7.rt..V..U.5...
-000029f0: 27d3 6830 ae02 1b78 92b2 94eb 1ced 9dd3  '.h0...x........
-00002a00: 1463 cbf7 2099 8dbc 4379 71db 18c9 9c7f  .c.. ...Cyq.....
-00002a10: 9a1d d68c 7fb0 1de0 248e 1758 8263 8239  ........$..X.c.9
-00002a20: 863b 60a8 4722 3a21 051f 91fa d3d4 3d40  .;`.G":!......=@
-00002a30: 700c 3548 50ce 6212 11fc e375 60a4 fdb3  p.5HP.b....u`...
-00002a40: a157 264e 59b9 a3f6 3b9d e24e d982 0fe2  .W&NY...;..N....
-00002a50: e83e d86a 34b6 6d1b b569 1fc3 e727 f86d  .>.j4.m..i...'.m
-00002a60: f3f8 dcaf 1a56 aabb 1507 5464 8253 6e80  .....V....Td.Sn.
-00002a70: b9c6 140f 602d 6478 52e9 ae57 33eb 36fe  ....`-dxR..W3.6.
-00002a80: d0db 0ac4 edf1 6cba 143c a90f 3ee0 4004  ......l..<..>.@.
-00002a90: 3e0a 1d82 9f95 d7f4 eebe 5ca3 2289 9324  >.........\."..$
-00002aa0: 8ce7 61b2 2c13 4267 0b9a debc 7773 7ff5  ..a.,.Bg....ws..
-00002ab0: 77d1 8682 3c4d ff07 318d 4b92 d059 4ae7  w...<M..1.K..YJ.
-00002ac0: 6442 3c03 8a0c 5f7c 87e2 1b00 00ff ff03  dB<..._|........
-00002ad0: 0050 4b03 0414 0006 0008 0000 0021 002a  .PK..........!.*
-00002ae0: d179 cb95 0100 0064 0300 0010 0008 0164  .y.....d.......d
-00002af0: 6f63 5072 6f70 732f 6170 702e 786d 6c20  ocProps/app.xml 
-00002b00: a204 0128 a000 0100 0000 0000 0000 0000  ...(............
-00002b10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002b20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002b30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002b40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002b50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002b60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002b70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002b80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002b90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002ba0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002bb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002bc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002bd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002be0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002bf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002c00: 0000 0000 0000 009c 9341 4fdc 3010 85ef  .........AO.0...
-00002c10: 95fa 1f22 df59 075a 50b5 728c aa05 c4a1  ...".Y.ZP.r.....
-00002c20: a82b ed42 cfc6 996c 2c12 dbf2 0cd1 2ebf  .+.B...l,.......
-00002c30: be93 4484 2cdd 536f e3f7 464f 9f67 6c75  ..D.,.So..FO.glu
-00002c40: bd6f 9bac 8384 2ef8 429c 2f72 9181 b7a1  .o......B./r....
-00002c50: 747e 5788 c7ed ddd9 0f91 2119 5f9a 2678  t~W.......!._.&x
-00002c60: 28c4 0150 5ceb af5f d43a 8508 891c 60c6  (..P\.._.:....`.
-00002c70: 111e 0b51 13c5 a594 686b 680d 2ed8 f6ec  ...Q....hkh.....
-00002c80: 5421 b586 f898 7632 5495 b370 13ec 6b0b  T!....v2T..p..k.
-00002c90: 9ee4 459e 5f49 d813 f812 cab3 3805 8a31  ..E._I......8..1
-00002ca0: 71d9 d1ff 8696 c1f6 7cf8 b43d 4406 d6ea  q.......|..=D...
-00002cb0: 678c 8db3 86f8 96fa c1d9 1430 5494 ddee  g..........0T...
-00002cc0: 2d34 4ace 4dc5 741b b0af c9d1 41e7 4ace  -4J.M.t.....A.J.
-00002cd0: 8f6a 634d 032b 0ed6 9569 1094 fc10 d43d  .jcM.+...i.....=
-00002ce0: 987e 686b e312 6ad5 d1b2 034b 2165 e8de  .~hk..j....K!e..
-00002cf0: 786c 1722 7b36 083d 4e21 3a93 9cf1 c458  xl."{6.=N!:....X
-00002d00: 7ddb 7818 ea26 2225 fd27 a417 ac01 0895  }.x..&"%.'......
-00002d10: e486 511c ca79 efbc 76df f5e5 d0c0 c571  ..Q..y..v......q
-00002d20: 631f 3082 b071 8cb8 75d4 00fe aed6 26d1  c.0..q..u.....&.
-00002d30: 09e2 cb39 f1c0 30f2 8e38 668e 3641 3e9f  ...9..0..8f.6A>.
-00002d40: 54ed 49b5 3ca9 f24c 3f5d 7998 22c3 7fc2  T.I.<..L?]y."...
-00002d50: 5d85 361a 7f60 63aa 7e39 ff82 8f71 1b6e  ].6..`c.~9...q.n
-00002d60: 0cc1 fb86 8e45 b5a9 4d82 9297 3a6d 7012  .....E..M...:mp.
-00002d70: d43d 2f27 357d c8aa 367e 07e5 7bcf bf46  .=/'5}..6~..{..F
-00002d80: ff9e 9ec6 4fa3 cfaf 16f9 b79c 9fca 4c53  ....O.........LS
-00002d90: f2e3 7be8 bf00 0000 ffff 0300 504b 0102  ..{.........PK..
-00002da0: 2d00 1400 0600 0800 0000 2100 4841 42ca  -.........!.HAB.
-00002db0: 7101 0000 b006 0000 1300 0000 0000 0000  q...............
-00002dc0: 0000 0000 0000 0000 0000 5b43 6f6e 7465  ..........[Conte
-00002dd0: 6e74 5f54 7970 6573 5d2e 786d 6c50 4b01  nt_Types].xmlPK.
-00002de0: 022d 0014 0006 0008 0000 0021 00b5 5530  .-.........!..U0
-00002df0: 23f4 0000 004c 0200 000b 0000 0000 0000  #....L..........
-00002e00: 0000 0000 0000 00aa 0300 005f 7265 6c73  ..........._rels
-00002e10: 2f2e 7265 6c73 504b 0102 2d00 1400 0600  /.relsPK..-.....
-00002e20: 0800 0000 2100 71e8 7b2f b303 0000 6409  ....!.q.{/....d.
-00002e30: 0000 0f00 0000 0000 0000 0000 0000 0000  ................
-00002e40: cf06 0000 786c 2f77 6f72 6b62 6f6f 6b2e  ....xl/workbook.
-00002e50: 786d 6c50 4b01 022d 0014 0006 0008 0000  xmlPK..-........
-00002e60: 0021 003d 5880 7a10 0100 00ee 0400 001a  .!.=X.z.........
-00002e70: 0000 0000 0000 0000 0000 0000 00af 0a00  ................
-00002e80: 0078 6c2f 5f72 656c 732f 776f 726b 626f  .xl/_rels/workbo
-00002e90: 6f6b 2e78 6d6c 2e72 656c 7350 4b01 022d  ok.xml.relsPK..-
-00002ea0: 0014 0006 0008 0000 0021 002d cb5c 0cf8  .........!.-.\..
-00002eb0: 0200 0048 0700 0018 0000 0000 0000 0000  ...H............
-00002ec0: 0000 0000 00ff 0c00 0078 6c2f 776f 726b  .........xl/work
-00002ed0: 7368 6565 7473 2f73 6865 6574 312e 786d  sheets/sheet1.xm
-00002ee0: 6c50 4b01 022d 0014 0006 0008 0000 0021  lPK..-.........!
-00002ef0: 0093 958a 80f4 0200 0052 0700 0018 0000  .........R......
-00002f00: 0000 0000 0000 0000 0000 002d 1000 0078  ...........-...x
-00002f10: 6c2f 776f 726b 7368 6565 7473 2f73 6865  l/worksheets/she
-00002f20: 6574 322e 786d 6c50 4b01 022d 0014 0006  et2.xmlPK..-....
-00002f30: 0008 0000 0021 00fe acc9 e9d8 0200 0098  .....!..........
-00002f40: 0600 0018 0000 0000 0000 0000 0000 0000  ................
-00002f50: 0057 1300 0078 6c2f 776f 726b 7368 6565  .W...xl/workshee
-00002f60: 7473 2f73 6865 6574 332e 786d 6c50 4b01  ts/sheet3.xmlPK.
-00002f70: 022d 0014 0006 0008 0000 0021 008c 50f6  .-.........!..P.
-00002f80: 3fd7 0200 0098 0600 0018 0000 0000 0000  ?...............
-00002f90: 0000 0000 0000 0065 1600 0078 6c2f 776f  .......e...xl/wo
-00002fa0: 726b 7368 6565 7473 2f73 6865 6574 342e  rksheets/sheet4.
-00002fb0: 786d 6c50 4b01 022d 0014 0006 0008 0000  xmlPK..-........
-00002fc0: 0021 00cb 1d3c 24de 0200 00a8 0600 0018  .!...<$.........
-00002fd0: 0000 0000 0000 0000 0000 0000 0072 1900  .............r..
-00002fe0: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
-00002ff0: 6865 6574 352e 786d 6c50 4b01 022d 0014  heet5.xmlPK..-..
-00003000: 0006 0008 0000 0021 00c1 1710 be4e 0700  .......!.....N..
-00003010: 00c6 2000 0013 0000 0000 0000 0000 0000  .. .............
-00003020: 0000 0086 1c00 0078 6c2f 7468 656d 652f  .......xl/theme/
-00003030: 7468 656d 6531 2e78 6d6c 504b 0102 2d00  theme1.xmlPK..-.
-00003040: 1400 0600 0800 0000 2100 8c05 4567 1803  ........!...Eg..
-00003050: 0000 ba08 0000 0d00 0000 0000 0000 0000  ................
-00003060: 0000 0000 0524 0000 786c 2f73 7479 6c65  .....$..xl/style
-00003070: 732e 786d 6c50 4b01 022d 0014 0006 0008  s.xmlPK..-......
-00003080: 0000 0021 002e 8e9c 7cdc 0000 008d 0100  ...!....|.......
-00003090: 0014 0000 0000 0000 0000 0000 0000 0048  ...............H
-000030a0: 2700 0078 6c2f 7368 6172 6564 5374 7269  '..xl/sharedStri
-000030b0: 6e67 732e 786d 6c50 4b01 022d 0014 0006  ngs.xmlPK..-....
-000030c0: 0008 0000 0021 00ca 5ca8 f744 0100 005b  .....!..\..D...[
-000030d0: 0200 0011 0000 0000 0000 0000 0000 0000  ................
-000030e0: 0056 2800 0064 6f63 5072 6f70 732f 636f  .V(..docProps/co
-000030f0: 7265 2e78 6d6c 504b 0102 2d00 1400 0600  re.xmlPK..-.....
-00003100: 0800 0000 2100 2ad1 79cb 9501 0000 6403  ....!.*.y.....d.
-00003110: 0000 1000 0000 0000 0000 0000 0000 0000  ................
-00003120: d12a 0000 646f 6350 726f 7073 2f61 7070  .*..docProps/app
-00003130: 2e78 6d6c 504b 0506 0000 0000 0e00 0e00  .xmlPK..........
-00003140: 9803 0000 9c2d 0000 0000                 .....-....
+00000bd0: 0000 0000 0000 0000 0000 0000 00bc 94dd  ................
+00000be0: 6a84 3010 85ef 0b7d 07c9 7d8d ba3f 2d65  j.0....}..}..?-e
+00000bf0: e3de 94c2 deb6 db07 083a 1a59 4d24 33fd  .........:.YM$3.
+00000c00: f1ed 3b08 ad15 96f4 46bc 094c 869c f3e5  ..;.....F..L....
+00000c10: 0cc9 e1f8 d5b5 d107 786c 9c55 228d 1311  ........xl.U"...
+00000c20: 812d 5cd9 d85a 89b7 f3f3 dd83 8890 b42d  .-\..Z.........-
+00000c30: 75eb 2c28 3100 8a63 7e7b 7378 8156 131f  u.,(1..c~{sx.V..
+00000c40: 42d3 f418 b18a 4525 0c51 ff28 2516 063a  B.....E%.Q.(%..:
+00000c50: 8db1 ebc1 72a7 72be d3c4 a5af 65af 8b8b  ....r.r.....e...
+00000c60: ae41 6649 b297 feaf 86c8 679a d1a9 54c2  .AfI......g...T.
+00000c70: 9f4a f63f 0f3d 3bff afed aaaa 29e0 c915  .J.?.=;.....)...
+00000c80: ef1d 58ba 6221 d168 0fe5 2b79 be1e b2b0  ..X.b!.h..+y....
+00000c90: f635 9012 b3ed 9889 85bc 0eb3 5912 e6d3  .5..........Y...
+00000ca0: f90b 1a00 9a40 7eb7 9051 b9b3 09c1 dc2f  .....@~..Q...../
+00000cb0: 9a0c 0d2d 8f76 8a64 ac43 f6d9 ca59 6421  ...-.v.d.C...Yd!
+00000cc0: 9874 6598 3404 b35f 1286 f829 c134 97b1  .te.4.._...).4..
+00000cd0: 94e3 1a64 d8ad 1cc8 2e14 c876 6598 ed0f  ...d.......ve...
+00000ce0: 8c9c fd52 f937 0000 00ff ff03 0050 4b03  ...R.7.......PK.
+00000cf0: 0414 0006 0008 0000 0021 004f 51ac 0514  .........!.OQ...
+00000d00: 0300 00d0 0700 0018 0000 0078 6c2f 776f  ...........xl/wo
+00000d10: 726b 7368 6565 7473 2f73 6865 6574 312e  rksheets/sheet1.
+00000d20: 786d 6c9c d34b 6fa3 3010 00e0 7ba5 fd0f  xml..Ko.0...{...
+00000d30: 96ef c440 425a 5048 9596 b0db 5b55 75f7  ...@BZPH....[Uu.
+00000d40: ee98 2158 f183 b59d 9756 fbdf 6b13 25ad  ..!X.....V..k.%.
+00000d50: 944b 5409 c480 c537 3378 983d 1ea4 403b  .KT....73x.=..@;
+00000d60: 3096 6b55 e264 1463 048a e986 ab75 897f  0.kU.d.c.....u..
+00000d70: bfd7 d103 46d6 51d5 50a1 1594 f808 163f  ....F.Q.P......?
+00000d80: ce7f dccd f6da 6c6c 07e0 9017 942d 71e7  ......ll.....-q.
+00000d90: 5c5f 1062 5907 92da 91ee 41f9 9556 1b49  \_.bY.....A..V.I
+00000da0: 9dbf 356b 627b 03b4 195e 9282 a471 3c25  ..5kb{...^...q<%
+00000db0: 9272 854f 4261 6e31 74db 7206 9566 5b09  .r.OBan1t.r..f[.
+00000dc0: ca9d 1003 823a 5fbf ed78 6fcf 9a64 b770  .....:_..xo..d.p
+00000dd0: 929a cdb6 8f98 96bd 2756 5c70 771c 508c  ........'V\pw.P.
+00000de0: 242b 5ed6 4a1b ba12 beef 4332 a10c 1d8c  $+^.J.....C2....
+00000df0: 3f52 7f8e cf69 86e7 5799 2467 465b ddba  ?R...i..W.$gF[..
+00000e00: 9197 c9a9 e6eb f673 9213 ca2e d275 ff37  .......s.....u.7
+00000e10: 31c9 8418 d8f1 b081 9f54 fabd 9292 ec62  1........T.....b
+00000e20: a59f d8f8 9bd8 f482 85cf 658a 2d6f 4afc  ..........e.-oJ.
+00000e30: 2f9f 3e4d c6d9 621c 2dab 6a1a 4dea e421  /.>M..b.-.j.M..!
+00000e40: caab 6516 dd2f 9e9f e23a bfaf b265 fd1f  ..e../...:...e..
+00000e50: cf67 0df7 3b1c ba42 06da 122f 92e2 6786  .g..;..B.../..g.
+00000e60: c97c 36cc cf1f 0e7b fb25 4661 1c57 5a6f  .|6....{.%Fa.WZo
+00000e70: c2c2 8b4f 137b c182 0016 0603 517f d9c1  ...O.{......Q...
+00000e80: 3308 51e2 2a0d 23fd 7740 43ec 4972 31bf  3.Q.*.#.w@C.Ir1.
+00000e90: c667 bf1e 46f8 d5a0 065a ba15 ee4d ef7f  .g..F....Z...M..
+00000ea0: 015f 77ce ff2f 996f 2c4c 46d1 1c2b b0cc  ._w../.o,LF..+..
+00000eb0: 8fa4 4f3d 4a43 a11f 0000 00ff ff00 0000  ..O=JC..........
+00000ec0: ffff 9494 dd6a 8430 1085 5f45 f200 89f9  .....j.0.._E....
+00000ed0: 6b76 9718 a82b f639 c40a bdda 968d d8f6  kv...+.9........
+00000ee0: ed9b 38e2 4ea6 a5a0 17a2 73c6 93f3 4d54  ..8.N.....s...MT
+00000ef0: 1fdf a669 ee86 7908 fefe fe59 dd1b 2659  ...i..y....Y..&Y
+00000f00: 153f 865b 4c57 17c7 aa2f 6986 f1f2 fadd  .?.[LW.../i.....
+00000f10: 4d71 9c6e 73c3 6aae 2c0b 7ecc bdcf a939  Mq.ns.j.,.~....9
+00000f20: 9562 ba5f 82f6 6209 5e8c 9bd6 62ad 2eb5  .b._..b.^...b...
+00000f30: 2bd6 64a9 7558 53bb 2652 bc3d a33a 9251  +.d.uXS.&R.=.:.Q
+00000f40: ade9 1e4e 6bf2 365b 342c 9df7 fc4f 24e3  ...Nk.6[4,...O$.
+00000f50: ef0e 4b92 82b3 e4ca 11f7 1e9e b54c 6cc3  ..K..........Ll.
+00000f60: 7841 8582 441f 21d1 7fce 395b e46d cb7b  xA..D.!...9[.m.{
+00000f70: a0b8 74ee 8c0f 0205 cd18 db10 2858 2419  ..t.........(X$.
+00000f80: 9d6a 7c50 4230 4284 a850 109a 2384 66a5  .j|PB0B..P..#.f.
+00000f90: 2091 da6c 51ee 9523 58d0 0133 d0fc 5c1b   ..lQ..#X..3..\.
+00000fa0: 3c82 1321 8445 721b b1e9 c106 41a1 4201  <..!.Er.....A.B.
+00000fb0: 658f 40e5 cf65 09e4 e569 b345 0945 725e  e.@..e...i.E.Er^
+00000fc0: a103 a02c 779a eed4 e69b 14fb 0f6e 0f36  ...,w........n.6
+00000fd0: 080a 1500 4a3c fe02 3f00 0000 ffff 0000  ....J<..?.......
+00000fe0: 00ff ffb2 2948 4c4f f54d 2c4a cfcc 2b56  ....)HLO.M,J..+V
+00000ff0: c849 4d2b b155 32d0 3357 5228 ca4c cf80  .IM+.U2.3WR(.L..
+00001000: b14b f20b c0a2 a64a 0a49 f925 25f9 b930  .K.....J.I.%%..0
+00001010: 5e46 6a62 4a6a 1188 67ac a490 969f 5f02  ^FjbJj..g....._.
+00001020: e3e8 dbd9 e897 e717 6517 67a4 a696 d801  ........e.g.....
+00001030: 0000 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
+00001040: 0000 0021 0031 a2f7 2822 0300 00ea 0700  ...!.1..("......
+00001050: 0018 0000 0078 6c2f 776f 726b 7368 6565  .....xl/workshee
+00001060: 7473 2f73 6865 6574 322e 786d 6c9c 934b  ts/sheet2.xml..K
+00001070: 8fda 3014 85f7 23f5 3f58 de07 c781 3025  ..0...#.?X....0%
+00001080: 4a18 a540 a6b3 abaa b67b e3dc 100b 3f52  J..@.....{....?R
+00001090: dbbc 34ea 7f1f 2708 a8c4 068d 142b d7b1  ..4...'......+..
+000010a0: fc9d 7be2 e3fc e5a8 24da 8375 c2e8 02d3  ..{.....$..u....
+000010b0: 518c 1168 6e6a a137 05fe fdab 8abe 62e4  Q..hnj.7......b.
+000010c0: 3cd3 3593 4643 814f e0f0 cbfc cb53 7e30  <.5.FC.O.....S~0
+000010d0: 76eb 5a00 8f02 41bb 02b7 de77 1921 8eb7  v.Z...A....w.!..
+000010e0: a098 1b99 0e74 5869 8c55 cc87 a9dd 10d7  .....tXi.U......
+000010f0: 5960 f5b0 4949 92c4 f194 2826 343e 1332  Y`..II....(&4>.2
+00001100: fb08 c334 8de0 b034 7ca7 40fb 33c4 8264  ...4...4|.@.3..d
+00001110: 3ef4 ef5a d1b9 0b4d f147 708a d9ed ae8b  >..Z...M.Gp.....
+00001120: b851 5d40 ac85 14fe 3440 3152 3c7b db68  .Q]@....4@1R<{.h
+00001130: 63d9 5a06 df47 3a61 1c1d 6d78 9230 c617  c.Z..G:a..mx.0..
+00001140: 99e1 fb9d 9212 dc1a 671a 3f0a 6472 eef9  ........g.?.dr..
+00001150: defe 8ccc 08e3 57d2 bdff 8730 7442 2cec  ......W....0tB,.
+00001160: 457f 8037 54f2 b996 687a 6525 37d8 f893  E..7T...hze%7...
+00001170: b0e9 15d6 ff2e 9bed 445d e0f7 5542 5734  ........D]..UBW4
+00001180: 59cd a274 394e a249 1a2f a292 56d3 a82c  Y..t9N.I./..V..,
+00001190: bf2d 17cf f122 2967 cfff f03c af45 38e1  .-...")g...<.E8.
+000011a0: de15 b2d0 14b8 a4d9 6b8a c93c 1ff2 f347  ........k..<...G
+000011b0: c0c1 fd57 a33e 8e6b 63b6 fdc2 5b90 8903  ...W.>.kc...[...
+000011c0: c181 04de 0703 b1f0 dac3 02a4 2c70 4543  ............,pEC
+000011d0: a2ff 0ecc eac2 2457 e83c bfd5 1781 6ac8  ......$W.<....j.
+000011e0: f00f 8b6a 68d8 4efa 9fe6 f01d c4a6 f5e1  ...jh.N.........
+000011f0: c2a4 c159 1f8d ac3e 2dc1 f190 c9a0 3d4a  ...Y...>-.....=J
+00001200: fa4e 3f00 0000 ffff 0000 00ff ff94 545b  .N?...........T[
+00001210: 6e83 3010 bc0a f201 0cf8 0125 024b 2188  n.0........%.K!.
+00001220: 9e03 51a4 7ea5 518c 6873 fbda 5e02 eb6d  ..Q.~.Q.hs..^..m
+00001230: 1509 7f20 d819 c633 de85 da7e 4ed3 dc0d  ... ...3...~N...
+00001240: f360 eafb d777 726f 58ce 127b 1bae d6dd  .`...wroX..{....
+00001250: 9d4a 96fc e46a 184f 1f8f 6eb2 e374 9d1b  .J...j.O..n..t..
+00001260: 9671 a199 a947 cf3d 3bb2 2b59 f7bc 1859  .q...G.=;.+Y...Y
+00001270: a78b a9d3 71c5 5a8c 6531 76c1 581e 631d  ....q.Z.e1v.X.c.
+00001280: c6c4 86a5 cede e651 1cf1 2882 bb5d 2938  .......Q..(..])8
+00001290: 6fbd 44c3 dc75 f35f 108f 7f19 9a38 05e5  o.D..u._.....8..
+000012a0: 9c8b 92a8 f7f0 ae66 e97a 18ef a810 2591  .......f.z....%.
+000012b0: 4792 c87f cfd9 4bf8 b6f9 1e08 2e8a a2c2  G.....K.........
+000012c0: 8b84 0232 8e5d 9150 b049 108a 911e de45  ...2.].P.I.....E
+000012d0: a150 210a a58e 8452 c1b8 22c3 e325 7c7b  .P!....R.."..%|{
+000012e0: c260 f14a 94af 423d c97b 2f73 3270 1dec  .`.J..B=.{/s2p..
+000012f0: 2279 a532 acf4 4622 8212 8a88 0a51 447d  "y.2..F".....QD}
+00001300: 24a2 ff5e 1643 a6a7 f512 cf88 9a97 5267  $..^.C........Rg
+00001310: 6891 8fe9 0264 68b2 23eb 0293 c9f4 75eb  h....dh.#.....u.
+00001320: 7e8e 56bd d0ec 4113 8545 0508 9bee bf87  ~.V...A..E......
+00001330: 5f00 0000 ffff 0000 00ff ffb2 2948 4c4f  _...........)HLO
+00001340: f54d 2c4a cfcc 2b56 c849 4d2b b155 32d0  .M,J..+V.IM+.U2.
+00001350: 3357 5228 ca4c cf80 b14b f20b c0a2 a64a  3WR(.L...K.....J
+00001360: 0a49 f925 25f9 b930 5e46 6a62 4a6a 1188  .I.%%..0^FjbJj..
+00001370: 67ac a490 969f 5f02 e3e8 dbd9 e897 e717  g....._.........
+00001380: 6517 67a4 a696 d801 0000 00ff ff03 0050  e.g............P
+00001390: 4b03 0414 0006 0008 0000 0021 00b3 1262  K..........!...b
+000013a0: 9247 0300 0038 0800 0018 0000 0078 6c2f  .G...8.......xl/
+000013b0: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
+000013c0: 332e 786d 6c9c 93db 8e9b 3010 86ef 2bf5  3.xml.....0...+.
+000013d0: 1d2c df13 73c8 0914 b26a 73e8 ee5d d5e3  .,..s....js..]..
+000013e0: b563 8660 c5c6 d436 39a8 eabb 7700 25bb  .c.`...69...w.%.
+000013f0: 526e a295 000f f6f0 fdff e0f1 e2e9 ac15  Rn..............
+00001400: 3982 75d2 d439 8d46 2125 500b 53c8 7a9f  9.u..9.F!%P.S.z.
+00001410: d39f 3fb6 c19c 12e7 795d 7065 6ac8 e905  ..?.....y]pej...
+00001420: 1c7d 5a7e fcb0 3819 7b70 1580 2748 a85d  .}Z~..8.{p..'H.]
+00001430: 4e2b ef9b 8c31 272a d0dc 8d4c 0335 ae94  N+...1'*...L.5..
+00001440: c66a eef1 d5ee 996b 2cf0 a2ff 482b 1687  .j.....k,...H+..
+00001450: e194 692e 6b3a 1032 fb08 c394 a514 b036  ..i.k:.2.......6
+00001460: a2d5 50fb 0162 4171 8ffe 5d25 1b77 a569  ..P..bAq..]%.w.i
+00001470: f108 4e73 7b68 9b40 18dd 2062 2795 f497  ..Ns{h.@.. b'...
+00001480: 1e4a 8916 d9cb be36 96ef 14d6 7d8e c65c  .J.....6....}..\
+00001490: 90b3 c52b c63b b9ca f4f3 774a 5a0a 6b9c  ...+.;....wJZ.k.
+000014a0: 29fd 08c9 6cf0 7c5f 7eca 52c6 c58d 745f  )...l.|_~.R...t_
+000014b0: ff43 9868 cc2c 1c65 b781 afa8 f87d 96a2  .C.h.,.e.....}..
+000014c0: c98d 15bf c292 77c2 a637 58f7 bb6c d6ca  ......w..7X..l..
+000014d0: 22a7 7f93 d97a ba9a 2561 9026 e93c 18c7  "....z..%a.&.<..
+000014e0: e375 30df 6c3f 07d1 7633 9ba6 93f5 6a93  .u0.l?..v3....j.
+000014f0: 46ff e872 5148 dce1 ae2a 62a1 cce9 a728  F..rQH...*b....(
+00001500: fb32 a16c b9e8 fbe7 9784 937b 1313 cf77  .2.l.......{...w
+00001510: df41 81f0 801a 1125 5d7b ee8c 3974 892f  .A.....%]{..9t./
+00001520: 3815 22d1 f509 1d91 0b2f 8fb0 02a5 72fa  8."....../....r.
+00001530: 1c61 bafb d38b 7431 4ab0 9bc6 dbf8 aab7  .a....t1J.......
+00001540: ed5b faab 2505 94bc 55fe 9b39 3d83 dc57  .[..%...U..9=..W
+00001550: 1e85 2758 68d7 2959 7159 8313 d8a2 283d  ..'Xh.)YqY....(=
+00001560: 8a7b e3c2 2844 e093 6889 670d 5335 3ff7  .{..(D..h.g.S5?.
+00001570: e349 16be ea3c 924a 1605 7407 9112 d13a  .I...<.J..t....:
+00001580: 6ff4 ef61 69b0 d513 fe03 0000 ffff 0000  o..ai...........
+00001590: 00ff ff94 545b 6e83 3010 bc0a f201 307e  ....T[n.0.....0~
+000015a0: f08a 0c52 0b21 e740 14a9 5f49 14a3 a4bd  ...R.!.@.._I....
+000015b0: 7dd7 d934 ac57 5124 fc65 76c6 b33b 630b  }..4.WQ$.ev..;c.
+000015c0: e7bf e779 e9c7 656c dde5 744b 2e8d 5022  ...y..el..tK..P"
+000015d0: f1e7 f1e8 61b7 2b45 f2a3 ec38 edbe 7efb  ....a.+E...8..~.
+000015e0: d94f f371 6944 96ea 5cb4 6e0a dc0f 2043  .O.qiD..\.n... C
+000015f0: c9c3 f7b5 354e 5e5b 27a7 07f6 49b1 2cc6  ....5N^['...I.,.
+00001600: 3a8a a918 eb29 a663 6c1f 9d5b 0f4a 98fd  :....).cl..[.J..
+00001610: 6940 6f31 a05f 8e1e 2442 12c1 964a 8bac  i@o1._..$B...J..
+00001620: cac8 62f3 7648 46a1 4066 39f4 2b52 3237  ..b.vHF.@f9.+R27
+00001630: 2ba2 df34 18b0 412e e423 d903 2944 cecd  +..4..A..#..)D..
+00001640: 16e7 e6ee ceb2 4b0b 128d c0c1 746a 5449  ......K.....tjTI
+00001650: 0763 b7d1 31b2 e137 892d 4046 73e7 4f84  .c..1..7.-@Fs.O.
+00001660: 8535 a024 f14a 0a91 57bb c5ab bd7b cd99  .5.$.J..W....{..
+00001670: d720 f1ef d5a4 ca32 bc43 1c5f 01e0 6555  . .....2.C._..eU
+00001680: 9355 b157 8b2d 8056 176f 22db a366 81af  .U.W.-.V.o"..f..
+00001690: 0e34 0dd5 ac63 cd01 c924 0c52 88c2 c837  .4...c...$.R...7
+000016a0: 8431 0472 2388 2a29 a0aa 5cff 0a7f 0000  .1.r#.*)..\.....
+000016b0: 00ff ff00 0000 ffff b229 484c 4ff5 4d2c  .........)HLO.M,
+000016c0: 4acf cc2b 56c8 494d 2bb1 5532 d033 5752  J..+V.IM+.U2.3WR
+000016d0: 28ca 4ccf 80b1 4bf2 0bc0 a2a6 4a0a 49f9  (.L...K.....J.I.
+000016e0: 2525 f9b9 305e 466a 624a 6a11 8867 aca4  %%..0^FjbJj..g..
+000016f0: 9096 9f5f 02e3 e8db d9e8 97e7 1765 1767  ..._.........e.g
+00001700: a4a6 96d8 0100 0000 ffff 0300 504b 0304  ............PK..
+00001710: 1400 0600 0800 0000 2100 0c86 c513 f102  ........!.......
+00001720: 0000 0007 0000 1800 0000 786c 2f77 6f72  ..........xl/wor
+00001730: 6b73 6865 6574 732f 7368 6565 7434 2e78  ksheets/sheet4.x
+00001740: 6d6c 9cd3 5d6f 9b30 1406 e0fb 49fd 0f96  ml..]o.0....I...
+00001750: ef89 8184 3441 2155 4a9a ae77 d3b4 f5de  ....4A!UJ..w....
+00001760: 3187 60c5 1fcc 76be 34ed bfef 4094 b452  1.`...v.4...@..R
+00001770: 6ea2 4a20 0c16 cff1 c12f b3a7 a356 640f  n.J ...../...Vd.
+00001780: ce4b 6b0a 9a0c 624a c008 5b49 b329 e8ef  .Kk...bJ..[I.)..
+00001790: 5fab 6842 890f dc54 5c59 0305 3d81 a74f  _.hB...T\Y..=..O
+000017a0: f387 6fb3 8375 5bdf 0004 8282 f105 6d42  ..o..u[.......mB
+000017b0: 6873 c6bc 6840 733f b02d 189c a9ad d33c  hs..h@s?.-.....<
+000017c0: e0ad db30 df3a e055 ff92 562c 8de3 31d3  ...0.:.U..V,..1.
+000017d0: 5c1a 7a16 7277 8f61 eb5a 0a58 5ab1 d360  \.z.rw.a.Z.XZ..`
+000017e0: c219 71a0 78c0 f5fb 46b6 fea2 6971 0fa7  ..q.x...F...iq..
+000017f0: b9db eeda 4858 dd22 b196 4a86 538f 52a2  ....HX."..J.S.R.
+00001800: 45fe b631 d6f1 b5c2 be8f c988 0b72 7478  E..1.........rtx
+00001810: a478 0e2f 65fa e737 95b4 14ce 7a5b 8701  .x./e..7....z[..
+00001820: caec bce6 dbf6 a76c cab8 b84a b7fd dfc5  .......l...J....
+00001830: 2423 e660 2fbb 0dfc a0d2 af2d 29c9 ae56  $#.`/......-)..V
+00001840: fa81 0dbf 888d af58 f7b9 5cbe 9355 41ff  .......X..\..UA.
+00001850: 4e92 c797 7258 aea2 f1f8 6512 8dd2 e522  N...rX....e...."
+00001860: 7ace 1665 f41c 4f1f a78b 324b b272 f28f  z..e..O...2K.r..
+00001870: ce67 95c4 1dee ba22 0eea 822e 92fc 7544  .g....."......uD
+00001880: d97c d6e7 e75d c2c1 7f1a 932e 8e6b 6bb7  .|...].......kk.
+00001890: ddc4 1b96 8951 f0a0 4074 c120 1c2f 7b28  .....Q..@t. ./{(
+000018a0: 41a9 82be 2698 71ff a747 bb31 92ec 6a7e  A...&.q..G.1..j~
+000018b0: 1e5f fc55 1fe1 1f8e 5450 f39d 0a3f ede1  ._.U....TP...?..
+000018c0: 3bc8 4d13 f07f c9b0 b12e 1979 755a 8217  ;.M........yuZ..
+000018d0: 1849 2c3d 4833 54ff 0300 00ff ff00 0000  .I,=H3T.........
+000018e0: ffff 9493 5d0e 8230 1084 af42 7a00 4a4b  ....]..0...Bz.JK
+000018f0: 0b6a 0a89 48f0 1c04 497c 5263 893f b7b7  .j..H...I|Rc.?..
+00001900: 6511 b61b 6342 9fca 7ecb 7466 0bc6 9efb  e...cB..~.tf....
+00001910: 7ea8 dba1 2dcd fdfa 8cee 0513 2cb2 b7f6  ~...-.......,...
+00001920: 62dd 6e97 b3e8 2554 dbed 4eef bab7 5d7f  b.n...%T..N...].
+00001930: 190a 96c4 52b3 d274 be77 ef9a 5dc9 bae7  ....R..t.w..]...
+00001940: 4799 1afe 280d ef26 5661 9684 ec80 9908  G...(..&Va......
+00001950: 598d 999c 1977 f666 8f72 8d47 f9d3 9d97  Y....w.f.r.G....
+00001960: 2898 1a99 88f5 3627 0e81 c3bb 9e67 095a  (.....6'.....g.Z
+00001970: d4f2 d246 641a 90d1 8c4f 5339 a242 1029  ...Fd....OS9.B.)
+00001980: 5d13 291d 6d2b 3270 2f51 3060 32d6 398d  ].).m+2p/Q0`2.9.
+00001990: 041c bc3a be51 ff22 cd32 1b1d 1ed3 800c  ...:.Q.".2......
+000019a0: 8a84 0a41 24b5 2612 dc04 39ab f212 df48  ...A$.&...9....H
+000019b0: ca7d 78e9 16ad 8c5c 1934 0b98 4d2c 3385  .}x....\.4..M,3.
+000019c0: 9bc9 306a 38cf 6966 44a6 0119 940f 1520  ..0j8.ifD...... 
+000019d0: 1f5f fe9a 0f00 0000 ffff 0000 00ff ffb2  ._..............
+000019e0: 2948 4c4f f54d 2c4a cfcc 2b56 c849 4d2b  )HLO.M,J..+V.IM+
+000019f0: b155 32d0 3357 5228 ca4c cf80 b14b f20b  .U2.3WR(.L...K..
+00001a00: c0a2 a64a 0a49 f925 25f9 b930 5e46 6a62  ...J.I.%%..0^Fjb
+00001a10: 4a6a 1188 67ac a490 969f 5f02 e3e8 dbd9  Jj..g....._.....
+00001a20: e897 e717 6517 67a4 a696 d801 0000 00ff  ....e.g.........
+00001a30: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
+00001a40: 0096 4071 3cf1 0200 0000 0700 0018 0000  ..@q<...........
+00001a50: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
+00001a60: 6865 6574 352e 786d 6c9c d35d 6f9b 3014  heet5.xml..]o.0.
+00001a70: 06e0 fb49 fb0f 96ef 8981 1052 5048 95b6  ...I.......RPH..
+00001a80: c9d6 bb69 da76 ef98 43b0 e20f 6a3b 5f9a  ...i.v..C...j;_.
+00001a90: f6df 7720 4a5a 2937 5125 1006 8be7 f8e0  ..w JZ)7Q%......
+00001aa0: 97d9 e351 2bb2 07e7 a535 154d 4631 2560  ...Q+....5.MF1%`
+00001ab0: 84ad a5d9 54f4 f7af 55f4 4089 0fdc d45c  ....T...U.@....\
+00001ac0: 5903 153d 81a7 8ff3 af5f 6607 ebb6 be05  Y..=....._f.....
+00001ad0: 0804 05e3 2bda 86d0 958c 79d1 82e6 7e64  ....+.....y...~d
+00001ae0: 3b30 38d3 58a7 79c0 5bb7 61be 73c0 ebe1  ;08.X.y.[.a.s...
+00001af0: 25ad 581a c739 d35c 1a7a 164a 778f 619b  %.X..9.\.z.Jw.a.
+00001b00: 460a 78b1 62a7 c184 33e2 40f1 80eb f7ad  F.x.b...3.@.....
+00001b10: ecfc 45d3 e21e 4e73 b7dd 7591 b0ba 4362  ..E...Ns..u...Cb
+00001b20: 2d95 0ca7 01a5 448b f275 63ac e36b 857d  -.....D..uc..k.}
+00001b30: 1f93 8c0b 7274 78a4 788e 2f65 86e7 3795  ....rtx.x./e..7.
+00001b40: b414 ce7a db84 11ca ecbc e6db f60b 5630  ...z..........V0
+00001b50: 2eae d26d ff77 3149 c61c ec65 bf81 ef54  ...m.w1I...e...T
+00001b60: fab9 2525 93ab 95be 63e3 4f62 f915 eb3f  ..%%....c.Ob...?
+00001b70: 972b 77b2 aee8 dfc9 6251 64d3 e534 1aa7  .+w.....bQd..4..
+00001b80: aba7 288b 8b24 2a16 0f45 34cd f33c 5bc6  ..(..$*..E4..<[.
+00001b90: 7111 2f9f ffd1 f9ac 96b8 c37d 57c4 4153  q./........}W.AS
+00001ba0: d145 527e cb28 9bcf 86fc fc91 70f0 1fc6  .ER~.(......p...
+00001bb0: a48f e3da da6d 3ff1 8a65 6214 3c28 107d  .....m?..eb.<(.}
+00001bc0: 3008 c7cb 1e9e 41a9 8a2e c798 71ff 36a0  0.....A.....q.6.
+00001bd0: fd18 4976 353f 8e2f fe6a 88f0 0f47 6a68  ..Iv5?./.j...Gjh
+00001be0: f84e 859f f6f0 1de4 a60d f8bf 4cb0 b13e  .N..........L..>
+00001bf0: 1965 7d7a 012f 3092 587a 944e 50fd 0f00  .e}z./0.Xz.NP...
+00001c00: 00ff ff00 0000 ffff 9493 5b0e 8230 1045  ..........[..0.E
+00001c10: b742 ba80 be2b 620a 8942 701d 0449 fc42  .B...+b..Bp..I.B
+00001c20: 4389 8fdd 5b18 c4a1 5113 fa05 7386 db7b  C...[...Q...s..{
+00001c30: a7c5 ba73 d3f4 45d5 5799 ed2e f7a8 4b89  ...s..E.W.....K.
+00001c40: 2091 bb56 adf3 4fbb 9844 0fa1 ab7a 777a   ..V..O..D...zwz
+00001c50: 168d ab9b b64f 09a7 d290 ccd6 43ef de37  .....O......C..7
+00001c60: fb92 f3ef b74c 5976 cb2c ab27 76c0 8c2f  .....LYv.,.'v../
+00001c70: 598e 9958 b202 3339 33e6 edcd 1ee5 1a8f  Y..X..393.......
+00001c80: f2ab bb41 2225 7a64 9272 2d12 b4b6 815d  ...A"%zd.r-....]
+00001c90: 6806 21df ac36 81e5 9fa4 842f 0d61 d354  h.!..6...../.a.T
+00001ca0: 8ea8 b088 a4d6 4452 a36d 1d0c 7c90 4809  ......DR.m..|.H.
+00001cb0: 3045 631e b8cc 814f e3a0 b188 395a e129  0Ec....O....9Z.)
+00001cc0: cc32 2218 4609 3228 122a 2c22 e935 91e0  .2".F.2(.*,".5..
+00001cd0: 244c 1069 9078 4732 d468 f5c7 720e cd62  $L.i.xG2.h..r..b
+00001ce0: 9c8d 6f36 e129 4d5b 7892 6099 cf1d 1bef  ..o6.)M[x.`.....
+00001cf0: 7409 3228 1f2a 403e f6f9 6b5e 0000 00ff  t.2(.*@>..k^....
+00001d00: ff00 0000 ffff b229 484c 4ff5 4d2c 4acf  .......)HLO.M,J.
+00001d10: cc2b 56c8 494d 2bb1 5532 d033 5752 28ca  .+V.IM+.U2.3WR(.
+00001d20: 4ccf 80b1 4bf2 0bc0 a2a6 4a0a 49f9 2525  L...K.....J.I.%%
+00001d30: f9b9 305e 466a 624a 6a11 8867 aca4 9096  ..0^FjbJj..g....
+00001d40: 9f5f 02e3 e8db d9e8 97e7 1765 1767 a4a6  ._.........e.g..
+00001d50: 96d8 0100 0000 ffff 0300 504b 0304 1400  ..........PK....
+00001d60: 0600 0800 0000 2100 c117 10be 4e07 0000  ......!.....N...
+00001d70: c620 0000 1300 0000 786c 2f74 6865 6d65  . ......xl/theme
+00001d80: 2f74 6865 6d65 312e 786d 6cec 59cd 8b1b  /theme1.xml.Y...
+00001d90: 3714 bf17 fa3f 0c73 77fc 35e3 8f25 dee0  7....?.sw.5..%..
+00001da0: cf6c 93dd 2464 9d94 1cb5 b6ec 5156 3332  .l..$d......QV32
+00001db0: 92bc 1b13 0225 39f5 5228 a4a5 9742 6f3d  .....%9.R(...Bo=
+00001dc0: 94d2 4003 0dbd f48f 0924 b4e9 1fd1 27cd  ..@......$....'.
+00001dd0: d823 ade5 249b 6c4a 5a76 0d8b 47fe bda7  .#..$.lJZv..G...
+00001de0: a7f7 9e7e 7af3 74f1 d2bd 987a 4798 0bc2  ...~z.t....zG...
+00001df0: 9296 5fbe 50f2 3d9c 8cd8 9824 d396 7f6b  .._.P.=....$...k
+00001e00: 3828 347c 4f48 948c 1165 096e f90b 2cfc  8(4|OH...e.n..,.
+00001e10: 4bdb 9f7e 7211 6dc9 08c7 d803 f944 6ca1  K..~r.m......Dl.
+00001e20: 961f 4939 db2a 16c5 0886 91b8 c066 3881  ..I9.*.......f8.
+00001e30: df26 8cc7 48c2 239f 16c7 1c1d 83de 9816  .&..H.#.........
+00001e40: 2ba5 52ad 1823 92f8 5e82 6250 7b7d 3221  +.R..#..^.bP{}2!
+00001e50: 23ec 0d95 4a7f 7ba9 bc4f e131 9142 0d8c  #...J.{..O.1.B..
+00001e60: 28df 57aa b125 a1b1 e3c3 b242 8885 e852  (.W..%.....B...R
+00001e70: ee1d 21da f261 9e31 3b1e e27b d2f7 2812  ..!..a.1;..{..(.
+00001e80: 127e 68f9 25fd e717 b72f 16d1 5626 44e5  .~h.%..../..V&D.
+00001e90: 0659 436e a0ff 32b9 4c60 7c58 d173 f2e9  .YCn..2.L`|X.s..
+00001ea0: c16a d220 0883 5a7b a55f 03a8 5cc7 f5eb  .j. ..Z{._..\...
+00001eb0: fd5a bfb6 d2a7 0168 3482 95a6 b6d8 3aeb  .Z.....h4.....:.
+00001ec0: 956e 9061 0d50 fad5 a1bb 57ef 55cb 16de  .n.a.P....W.U...
+00001ed0: d05f 5db3 b91d aa8f 85d7 a054 7fb0 861f  ._]........T....
+00001ee0: 0cba e045 0baf 4129 3e5c c387 9d66 a767  ...E..A)>\...f.g
+00001ef0: ebd7 a014 5f5b c3d7 4bed 5e50 b7f4 6b50  ...._[..K.^P..kP
+00001f00: 4449 72b8 862e 85b5 6a77 b9da 1564 c2e8  DIr.....jw...d..
+00001f10: 8e13 de0c 8341 bd92 29cf 5190 0dab ec52  .....A..).Q....R
+00001f20: 534c 5822 37e5 5a8c ee32 3e00 8002 5224  SLX"7.Z..2>...R$
+00001f30: 49e2 c9c5 0c4f d008 b2b8 8b28 39e0 c4db  I....O.....(9...
+00001f40: 25d3 0812 6f86 1226 60b8 5429 0d4a 55f8  %...o..&`.T).JU.
+00001f50: af3e 81fe a623 8ab6 3032 a495 5d60 8958  .>...#..02..]`.X
+00001f60: 1b52 f678 62c4 c94c b6fc 2ba0 d537 202f  .R.xb..L..+..7 /
+00001f70: 9e3d 7bfe f0e9 f387 bf3d 7ff4 e8f9 c35f  .={......=....._
+00001f80: b2b9 b52a 4b6e 0725 5353 eed5 8f5f fffd  ...*Kn.%SS..._..
+00001f90: fd17 de5f bffe f0ea f137 e9d4 27f1 c2c4  ..._.....7..'...
+00001fa0: bffc f9cb 97bf fff1 3af5 b0e2 dc15 2fbe  ........:...../.
+00001fb0: 7df2 f2e9 9317 df7d f5e7 4f8f 1dda db1c  }......}..O.....
+00001fc0: 1d98 f021 89b1 f0ae e163 ef26 8b61 810e  ...!.....c.&.a..
+00001fd0: fbf1 013f 9dc4 3042 c492 4011 e876 a8ee  ...?..0B..@..v..
+00001fe0: cbc8 025e 5b20 eac2 75b0 edc2 db1c 58c6  ...^[ ..u.....X.
+00001ff0: 05bc 3cbf 6bd9 ba1f f1b9 248e 99af 46b1  ..<.k.....$...F.
+00002000: 05dc 638c 7618 773a e0aa 9acb f0f0 709e  ..c.v.w:......p.
+00002010: 4cdd 93f3 b989 bb89 d091 6bee 2e4a ac00  L.........k..J..
+00002020: f7e7 33a0 57e2 52d9 8db0 65e6 0d8a 1289  ..3.W.R...e.....
+00002030: a638 c1d2 53bf b143 8c1d abbb 4388 e5d7  .8..S..C....C...
+00002040: 3d32 e24c b089 f4ee 10af 8388 d325 4372  =2.L.........%Cr
+00002050: 6025 522e b443 6288 cbc2 6520 84da f2cd  `%R..Cb...e ....
+00002060: de6d afc3 a86b d53d 7c64 2361 5b20 ea30  .m...k.=|d#a[ .0
+00002070: 7e88 a9e5 c6cb 682e 51ec 5239 4431 351d  ~.....h.Q.R9D15.
+00002080: be8b 64e4 3272 7fc1 4726 ae2f 2444 7a8a  ..d.2r..G&./$Dz.
+00002090: 29f3 fa63 2c84 4be6 3a87 f51a 41bf 0a0c  )..c,.K.:...A...
+000020a0: e30e fb1e 5dc4 3692 4b72 e8d2 b98b 1833  ....].6.Kr.....3
+000020b0: 913d 76d8 8d50 3c73 da4c 92c8 c47e 260e  .=v..P<s.L...~&.
+000020c0: 2145 9177 8349 177c 8fd9 3b44 3d43 1c50  !E.w.I.|..;D=C.P
+000020d0: b231 dcb7 09b6 c2fd 6622 b805 e46a 9a94  .1......f"...j..
+000020e0: 2788 fa65 ce1d b1bc 8c99 bd1f 1774 82b0  '..e.........t..
+000020f0: 8b65 da3c b6d8 b5cd 8933 3b3a f3a9 95da  .e.<.....3;:....
+00002100: bb18 5374 8cc6 187b b73e 7358 d061 33cb  ..St...{.>sX.a3.
+00002110: e7b9 d157 2260 951d ec4a ac2b c8ce 55f5  ...W"`...J.+..U.
+00002120: 9c60 0165 92aa 6bd6 2972 9708 2b65 f7f1  .`.e..k.)r..+e..
+00002130: 946d b067 6f71 8278 1628 8911 dfa4 f91a  .m.goq.x.(......
+00002140: 44dd 4a5d 38e5 9c54 7a9d 8e0e 4de0 3502  D.J]8..Tz...M.5.
+00002150: e51f e48b d329 d705 e830 92bb bf49 eb8d  .....)...0...I..
+00002160: 0859 6797 7a16 ee7c 5d70 2b7e 6fb3 c760  .Yg.z..|]p+~o..`
+00002170: 5fde 3ded be04 197c 6a19 20f6 b7f6 cd10  _.=....|j. .....
+00002180: 516b 823c 6186 080a 0c17 dd82 8815 fe5c  Qk.<a..........\
+00002190: 449d ab5a 6cee 949b d89b 360f 0314 4656  D..Zl.....6...FV
+000021a0: bd13 93e4 8dc5 cf89 b227 fc77 ca1e 7701  .........'.w..w.
+000021b0: 7306 058f 5bf1 fb94 3a9b 2865 e744 81b3  s...[...:.(e.D..
+000021c0: 09f7 1f2c 6b7a 689e dcc0 7092 ac73 d679  ...,kzh...p..s.y
+000021d0: 5573 5ed5 f8ff fbaa 66d3 5e3e af65 ce6b  Us^.....f.^>.e.k
+000021e0: 99f3 5ac6 f5f6 f541 6a99 bc7c 81ca 26ef  ..Z....Aj..|..&.
+000021f0: f2e8 9e4f bcb1 e533 2194 eecb 05c5 bb42  ...O...3!......B
+00002200: 777d 04bc d18c 0730 a8db 51ba 27b9 6a01  w}.....0..Q.'.j.
+00002210: ce22 f89a 3598 2cdc 9423 2de3 7126 3f27  ."..5.,..#-.q&?'
+00002220: 32da 8fd0 0c5a 4365 ddc0 9c8a 4cf5 5478  2....ZCe....L.Tx
+00002230: 3326 a063 a487 752b 159f d0ad fb4e f378  3&.c..u+.....N.x
+00002240: 8f8d d34e 67b9 acba 9aa9 0b05 92f9 7829  ...Ng.........x)
+00002250: 5c8d 4397 4aa6 e85a 3def dead d4eb 7ee8  \.C.J..Z=.....~.
+00002260: 5477 5997 0628 d9d3 1861 4c66 1b51 7518  TwY..(...aLf.Qu.
+00002270: 515f 0e42 145e 6784 5ed9 9958 d174 58d1  Q_.B.^g.^..X.tX.
+00002280: 50ea 97a1 5a46 71e5 0a30 6d15 1578 e5f6  P...ZFq..0m..x..
+00002290: e045 bde5 8741 da41 8666 1c94 e763 15a7  .E...A.A.f...c..
+000022a0: b499 bc8c ae0a ce99 467a 9333 a999 0150  ........Fz.3...P
+000022b0: 622f 3320 8f74 53d9 ba71 796a 7569 aabd  b/3 .tS..qyjui..
+000022c0: 45a4 2d23 8c74 b38d 30d2 3082 17e1 2c3b  E.-#.t..0.0...,;
+000022d0: cd96 fb59 c6ba 9987 d432 4fb9 62b9 1b72  ...Y.....2O.b..r
+000022e0: 33ea 8d0f 116b 4522 27b8 8126 2653 d0c4  3....kE"'..&&S..
+000022f0: 3b6e f9b5 6a08 b72a 2334 6bf9 13e8 18c3  ;n..j..*#4k.....
+00002300: d778 06b9 23d4 5b17 a253 b876 1949 9e6e  .x..#.[..S.v.I.n
+00002310: f877 6196 1917 b287 4494 3a5c 934e ca06  .wa.....D.:\.N..
+00002320: 3191 987b 94c4 2d5f 2d7f 950d 34d1 1ca2  1..{..-_-...4...
+00002330: 6d2b 5780 103e 5ae3 9a40 2b1f 9b71 1074  m+W..>Z..@+..q.t
+00002340: 3bc8 7832 c123 6986 dd18 519e 4e1f 81e1  ;.x2.#i...Q.N...
+00002350: 53ae 70fe aac5 df1d ac24 d91c c2bd 1f8d  S.p......$......
+00002360: 8fbd 033a e737 11a4 5858 2f2b 078e 8980  ...:.7..XX/+....
+00002370: 8b83 72ea cd31 819b b015 91e5 f977 e260  ..r..1.......w.`
+00002380: ca68 d7bc 8ad2 3994 8e23 3a8b 5076 a298  .h....9..#:.Pv..
+00002390: 649e c235 89ae ccd1 4f2b 1f18 4fd9 9ac1  d..5....O+..O...
+000023a0: a1eb 2e3c 98aa 03f6 bd4f dd37 1fd5 ca73  ...<.....O.7...s
+000023b0: 0669 e667 a6c5 2aea d474 93e9 873b e40d  .i.g..*..t...;..
+000023c0: abf2 43d4 b22a a56e fd4e 2d72 ae6b 2eb9  ..C..*.n.N-r.k..
+000023d0: 0e12 d579 4abc e1d4 7d8b 03c1 302d 9fcc  ...yJ...}...0-..
+000023e0: 324d 59bc 4ec3 8ab3 b351 dbb4 332c 080c  2MY.N....Q..3,..
+000023f0: 4fd4 36f8 6d75 4638 3df1 ae27 3fc8 9dcc  O.6.muF8=..'?...
+00002400: 5a75 402c eb4a 9df8 faca dcbc d566 0777  Zu@,.J.......f.w
+00002410: 813c 7a70 7f38 a752 e850 426f 9723 28fa  .<zp.8.R.PBo.#(.
+00002420: d21b c894 3660 8bdc 9359 8d08 dfbc 3927  ....6`...Y....9'
+00002430: 2dff 7e29 6c07 dd4a d82d 941a 61bf 1054  -.~)l..J.-..a..T
+00002440: 8352 a111 b6ab 8576 1856 cbfd b05c ea75  .R.....v.V...\.u
+00002450: 2a0f e060 9151 5c0e d3eb fa01 5c61 d045  *..`.Q\.....\a.E
+00002460: 7669 afc7 d72e eee3 e52d cd85 118b 8b4c  vi.......-.....L
+00002470: 5fcc 17b5 e1fa e2be 5cd9 7c71 ef11 209d  _.......\.|q.. .
+00002480: fbb5 caa0 596d 766a 8566 b53d 2804 bd4e  ....Ymvj.f.=(..N
+00002490: a3d0 ecd6 3a85 5ead 5bef 0d7a ddb0 d11c  ....:.^.[..z....
+000024a0: 3cf0 bd23 0d0e dad5 6e50 eb37 0ab5 72b7  <..#....nP.7..r.
+000024b0: 5b08 6a25 657e a359 a807 954a 3ba8 b71b  [.j%e~.Y...J;...
+000024c0: fda0 fd20 2b63 60e5 297d 64be 00f7 6abb  ... +c`.)}d...j.
+000024d0: b6ff 0100 00ff ff03 0050 4b03 0414 0006  .........PK.....
+000024e0: 0008 0000 0021 0083 b677 5c7b 0300 00ce  .....!...w\{....
+000024f0: 0a00 000d 0000 0078 6c2f 7374 796c 6573  .......xl/styles
+00002500: 2e78 6d6c c456 5b6f db36 147e 1fb0 ff40  .xml.V[o.6.~...@
+00002510: 10d8 a3a2 4b2c d736 2415 751c 0105 ba22  ....K,.6$.u...."
+00002520: 4032 a0af b444 d944 79d1 282a 935b ecbf  @2...D.Dy.(*.[..
+00002530: ef90 922c b9cd d62c dde5 c526 8fce 39fc  ...,...,...&..9.
+00002540: be73 2393 d79d e0e8 91ea 8629 99e2 f02a  .s#........)...*
+00002550: c088 ca42 954c 1e52 fccb 43ee ad30 6a0c  ...B.L.R..C..0j.
+00002560: 9125 e14a d214 9f68 835f 673f fe90 34e6  .%.J...h._g?..4.
+00002570: c4e9 fd91 5283 c085 6c52 7c34 a6de f87e  ....R...lR|4...~
+00002580: 531c a920 cd95 aaa9 842f 95d2 8218 d8ea  S.. ...../......
+00002590: 83df d49a 92b2 b146 82fb 5110 2c7d 4198  .......F..Q.,}A.
+000025a0: c4bd 878d 289e e344 10fd b1ad bd42 899a  ....(..D.....B..
+000025b0: 18b6 679c 9993 f385 9128 366f 0f52 69b2  ..g......(6o.Ri.
+000025c0: e700 b50b 17a4 405d b8d4 11ea f478 8893  ......@].....x..
+000025d0: 7e75 8e60 8556 8daa cc15 f8f5 5555 b182  ~u.`.V......UU..
+000025e0: 7e0d 77ed af7d 524c 9ec0 f3cb 3c85 b11f  ~.w..}RL....<...
+000025f0: 4417 dc3b fd42 4f0b 5fd3 4766 d387 b344  D..;.BO._.Gf...D
+00002600: b622 17a6 4185 6aa5 4971 7416 a1fe cbdb  ."..A.j.Iqt.....
+00002610: 1272 bc5c 60d4 67e5 4695 10a7 e02a 0802  .r.\`.g.F....*..
+00002620: ec8f d617 aacb 2754 7fb2 bafe 7054 9654  ......'T....pT.T
+00002630: 4ace 4f84 8043 d837 1fa5 fa4d e6f6 139c  J.O..C.7...M....
+00002640: 0830 ac56 9634 9fd0 23e1 2009 ad8f 4271  .0.V.4..#. ...Bq
+00002650: a591 8172 0114 4e22 89a0 bdc6 0de1 6caf  ...r..N"......l.
+00002660: 9955 ab88 60fc d48b 232b 7015 36e8 0906  .U..`...#+p.6...
+00002670: f976 80fa 13fe ab73 7c47 1bc0 31ce 2fe2  .v.....s|G..1./.
+00002680: 6d05 5902 a569 a896 396c d0b0 7e38 d540  m.Y..i..9l..~8.@
+00002690: 5342 17f5 709d de37 b40f 9a9c c228 9e19  SB..p..7.....(..
+000026a0: f8ee c02c d92b 5d42 d78e 99b6 21ee 4559  ...,.+]B....!.EY
+000026b0: c269 6520 4a9a 1d8e f6df a81a 7ef7 ca18  .ie J.......~...
+000026c0: a8ec 2c29 1939 2849 b8cd e168 312c 1a48  ..,).9(I...h1,.H
+000026d0: 09e5 fcde 76f6 87ea 8255 57cd ca02 6684  ....v....UW...f.
+000026e0: 656f 8bc9 2e81 c8b0 ecfd f51b f07f 61b4  eo............a.
+000026f0: 9e8c c23f 3542 a4ae f9c9 968d 73dd efc0  ...?5B......s...
+00002700: ffb4 db3a ded3 fe0d 6707 29e8 dce0 4e2b  ...:....g.)...N+
+00002710: 430b e306 9aab 6b7f ceaa e738 a3f7 0a42  C.....k....8...B
+00002720: f7f7 e9a1 ae7a 9ae7 b382 73b6 ee09 cf48  .....z....s....H
+00002730: d844 42e9 f79c d051 69f6 09a2 617b c6e5  .DB....Qi...a{..
+00002740: d355 4257 7d17 62f4 6b0b 01ba d3b4 629d  .UBW}.b.k.....b.
+00002750: edbb 7f06 c330 56be 5516 13f3 2751 bc6f  .....0V.U...'Q.o
+00002760: c59e eadc dd19 ff23 3657 78ff 1616 3753  .......#6Wx...7S
+00002770: 9f19 a731 3b4f 63e9 1bc5 4dce 1757 f0b3  ...1;Oc...M..W..
+00002780: 4f70 5d04 7d33 1b12 1723 e2dc 64c8 4ef1  Op].}3...#..d.N.
+00002790: 14bf b749 e470 590e 8d82 f62d e386 c973  ...I.pY....-...s
+000027a0: db7c 6970 4775 018d 3c5a 00b0 9945 3f03  .|ipGu..<Z...E?.
+000027b0: cf26 80a2 eca6 11e5 dadc d86b df0d af33  .&.........k...3
+000027c0: 2e68 c692 56a4 e5e6 e1fc 31c5 d3fa 675a  .h..V.....1...gZ
+000027d0: b256 4467 ad3b f6a8 8c73 91e2 69fd ce4e  .VDg.;...s..i..N
+000027e0: d270 697b 8f76 e65d 0317 19fc a356 b314  .pi{.v.].....V..
+000027f0: 7fbe ddbe 5aef 6ef3 c85b 05db 95b7 b8a6  ....Z.n..[......
+00002800: b1b7 8eb7 3b2f 5edc 6c77 bb7c 1d44 c1cd  ....;/^.lw.|.D..
+00002810: efb3 c7c7 773c 3ddc 5b09 5a3f 5c6c 1a0e  ....w<=.[.Z?\l..
+00002820: 0f14 3d90 1d28 de4f b214 cf36 3d7c 3739  ..=..(.O...6=|79
+00002830: 00f6 1cfb 3a5a 066f e230 f0f2 eb20 f416  ....:Z.o.0... ..
+00002840: 4bb2 f256 cbeb d8cb e330 da2d 17db db38  K..V.....0.-...8
+00002850: 8f67 d8e3 173e 5102 3f0c fbc7 8e05 1f6f  .g...>Q.?......o
+00002860: 0c13 9433 39e6 6acc d05c 0a49 82ed 5f90  ...39.j..\.I.._.
+00002870: f0c7 4cf8 d343 34fb 0300 00ff ff03 0050  ..L..C4........P
+00002880: 4b03 0414 0006 0008 0000 0021 00a6 7a14  K..........!..z.
+00002890: ebe1 0000 00a6 0100 0014 0000 0078 6c2f  .............xl/
+000028a0: 7368 6172 6564 5374 7269 6e67 732e 786d  sharedStrings.xm
+000028b0: 6c6c d0c1 4ec4 2010 06e0 bb89 ef40 b80b  ll..N. ......@..
+000028c0: 8566 bb5d 03ec c1c4 785f 7d00 d2e2 9684  .f.]....x_}.....
+000028d0: 0e95 a1c6 bebd 6cf6 62a8 c7f9 e69f 1982  ......l.b.......
+000028e0: 3aff cc81 7cbb 843e 82a6 8235 9438 18e2  :...|..>...5.8..
+000028f0: e8e1 aae9 c7fb eb53 4f09 660b a30d 119c  .......SO.f.....
+00002900: a69b 437a 368f 0f0a 3193 320b a8e9 94f3  ..Cz6...1.2.....
+00002910: f2cc 390e 939b 2db2 b838 289d cf98 669b  ..9...-..8(...f.
+00002920: 4b99 ae1c 97e4 ec88 9373 790e 5c36 4dc7  K........sy.\6M.
+00002930: 67eb 8192 21ae 9035 6dcb d915 fcd7 ea5e  g...!..5m......^
+00002940: ee20 2435 0abd 51d9 2cdb 2594 958a 67a3  . $5..Q.,.%...g.
+00002950: f88d eefc b6a5 c142 ad97 e0c7 5d34 d9d1  .......B....]4..
+00002960: af58 4725 137d 53a3 60f2 28fe c35d b265  .XG%.}S.`.(..].e
+00002970: a766 8707 7614 fdfe 90ec ba1a cb78 7baa  .f..v........x{.
+00002980: 116f af27 87bf 7b79 f967 f30b 0000 ffff  .o.'..{y.g......
+00002990: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
+000029a0: feec b726 4f01 0000 6302 0000 1100 0801  ...&O...c.......
+000029b0: 646f 6350 726f 7073 2f63 6f72 652e 786d  docProps/core.xm
+000029c0: 6c20 a204 0128 a000 0100 0000 0000 0000  l ...(..........
+000029d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000029e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000029f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002a00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002a10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002a20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002a30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002a40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002a50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002a60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002a70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002a80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002a90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002aa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002ab0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002ac0: 0000 0000 0000 0000 0084 9251 4bc3 3014  ...........QK.0.
+00002ad0: 85df 05ff 43c9 7b9b a69b 7386 b603 953d  ....C.{...s....=
+00002ae0: 8803 c18a e25b 4cee b66a 9394 24da eddf  .....[L..j..$...
+00002af0: 9bb6 5bed 50f0 31f7 9c7c 39e7 9274 b193  ..[.P.1..|9..t..
+00002b00: 55f0 05c6 965a 6588 4431 0a40 712d 4ab5  U....Ze.D1.@q-J.
+00002b10: c9d0 53b1 0ce7 28b0 8e29 c12a ad20 437b  ..S...(..).*. C{
+00002b20: b068 919f 9fa5 bca6 5c1b 7830 ba06 e34a  .h......\.x0...J
+00002b30: b081 2729 4b79 9da1 ad73 35c5 d8f2 2d48  ..')Ky...s5...-H
+00002b40: 6623 ef50 5e5c 6b23 99f3 47b3 c135 e31f  f#.P^\k#..G..5..
+00002b50: 6c03 3889 e319 96e0 9860 8ee1 1618 d603  l.8......`......
+00002b60: 111d 9082 0fc8 fad3 541d 4070 0c15 4850  ........T.@p..HP
+00002b70: ce62 1211 fce3 7560 a4fd f342 a78c 9cb2  .b....u`...B....
+00002b80: 74fb da77 3ac4 1db3 05ef c5c1 bdb3 e560  t..w:..........`
+00002b90: 6c9a 266a 265d 0c9f 9fe0 97d5 fd63 5735  l.&j&].......cW5
+00002ba0: 2c55 bb2b 0e28 4f05 a7dc 0073 dae4 7760  ,U.+.(O....s..w`
+00002bb0: 2da4 7834 69b7 5731 eb56 7ed1 eb12 c4f5  -.x4i.W1.V~.....
+00002bc0: 3e7f 6f4d c19b 564c 299d e2df 064f ec0a  >.oM..VL)....O..
+00002bd0: f458 1081 8f44 fb02 47e5 7972 735b 2c51  .X...D..G.yrs[,Q
+00002be0: 9ec4 4912 c617 6132 2f12 42a7 333a b97a  ..I...a2/.B.3:.z
+00002bf0: 6ddf 3fb9 df46 ec07 f290 e25f e22c 2497  m.?..F....._.,$.
+00002c00: 0589 e994 5092 8c88 4740 dee5 3efd 16f9  ....P...G@..>...
+00002c10: 3700 0000 ffff 0300 504b 0304 1400 0600  7.......PK......
+00002c20: 0800 0000 2100 2ad1 79cb 9501 0000 6403  ....!.*.y.....d.
+00002c30: 0000 1000 0801 646f 6350 726f 7073 2f61  ......docProps/a
+00002c40: 7070 2e78 6d6c 20a2 0401 28a0 0001 0000  pp.xml ...(.....
+00002c50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002c60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002c70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002c80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002c90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002ca0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002cb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002cc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002cd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002ce0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002cf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002d00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002d10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002d20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002d30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002d40: 0000 0000 0000 0000 0000 0000 0000 9c93  ................
+00002d50: 414f dc30 1085 ef95 fa1f 22df 5907 5a50  AO.0......".Y.ZP
+00002d60: b572 8caa 05c4 a1a8 2bed 42cf c699 6c2c  .r......+.B...l,
+00002d70: 12db f20c d12e bfbe 9344 842c dd53 6fe3  .........D.,.So.
+00002d80: f746 4f9f 676c 75bd 6f9b ac83 842e f842  .FO.glu.o......B
+00002d90: 9c2f 7291 81b7 a174 7e57 88c7 eddd d90f  ./r....t~W......
+00002da0: 9121 195f 9a26 7828 c401 505c ebaf 5fd4  .!._.&x(..P\.._.
+00002db0: 3a85 0889 1c60 c611 1e0b 5113 c5a5 9468  :....`....Q....h
+00002dc0: 6b68 0d2e d8f6 ec54 21b5 86f8 9876 3254  kh.....T!....v2T
+00002dd0: 95b3 7013 ec6b 0b9e e445 9e5f 49d8 13f8  ..p..k...E._I...
+00002de0: 12ca b338 058a 3171 d9d1 ff86 96c1 f67c  ...8..1q.......|
+00002df0: f8b4 3d44 06d6 ea67 8c8d b386 f896 fac1  ..=D...g........
+00002e00: d914 3054 94dd ee2d 344a ce4d c574 1bb0  ..0T...-4J.M.t..
+00002e10: afc9 d141 e74a ce8f 6a63 4d03 2b0e d695  ...A.J..jcM.+...
+00002e20: 6910 94fc 10d4 3d98 7e68 6be3 126a d5d1  i.....=.~hk..j..
+00002e30: b203 4b21 65e8 de78 6c17 227b 3608 3d4e  ..K!e..xl."{6.=N
+00002e40: 213a 939c f1c4 587d db78 18ea 2622 25fd  !:....X}.x..&"%.
+00002e50: 27a4 17ac 0108 95e4 8651 1cca 79ef bc76  '........Q..y..v
+00002e60: dff5 e5d0 c0c5 7163 1f30 82b0 718c b875  ......qc.0..q..u
+00002e70: d400 feae d626 d109 e2cb 39f1 c030 f28e  .....&....9..0..
+00002e80: 3866 8e36 413e 9f54 ed49 b53c a9f2 4c3f  8f.6A>.T.I.<..L?
+00002e90: 5d79 9822 c37f c25d 8536 1a7f 6063 aa7e  ]y."...].6..`c.~
+00002ea0: 39ff 828f 711b 6e0c c1fb 868e 45b5 a94d  9...q.n.....E..M
+00002eb0: 8292 973a 6d70 12d4 3d2f 2735 7dc8 aa36  ...:mp..=/'5}..6
+00002ec0: 7e07 e57b cfbf 46ff 9e9e c64f a3cf af16  ~..{..F....O....
+00002ed0: f9b7 9c9f ca4c 53f2 e37b e8bf 0000 00ff  .....LS..{......
+00002ee0: ff03 0050 4b01 022d 0014 0006 0008 0000  ...PK..-........
+00002ef0: 0021 0048 4142 ca71 0100 00b0 0600 0013  .!.HAB.q........
+00002f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002f10: 005b 436f 6e74 656e 745f 5479 7065 735d  .[Content_Types]
+00002f20: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
+00002f30: 0000 2100 b555 3023 f400 0000 4c02 0000  ..!..U0#....L...
+00002f40: 0b00 0000 0000 0000 0000 0000 0000 aa03  ................
+00002f50: 0000 5f72 656c 732f 2e72 656c 7350 4b01  .._rels/.relsPK.
+00002f60: 022d 0014 0006 0008 0000 0021 000e 2db9  .-.........!..-.
+00002f70: 62a1 0300 0051 0900 000f 0000 0000 0000  b....Q..........
+00002f80: 0000 0000 0000 00cf 0600 0078 6c2f 776f  ...........xl/wo
+00002f90: 726b 626f 6f6b 2e78 6d6c 504b 0102 2d00  rkbook.xmlPK..-.
+00002fa0: 1400 0600 0800 0000 2100 3d58 807a 1001  ........!.=X.z..
+00002fb0: 0000 ee04 0000 1a00 0000 0000 0000 0000  ................
+00002fc0: 0000 0000 9d0a 0000 786c 2f5f 7265 6c73  ........xl/_rels
+00002fd0: 2f77 6f72 6b62 6f6f 6b2e 786d 6c2e 7265  /workbook.xml.re
+00002fe0: 6c73 504b 0102 2d00 1400 0600 0800 0000  lsPK..-.........
+00002ff0: 2100 4f51 ac05 1403 0000 d007 0000 1800  !.OQ............
+00003000: 0000 0000 0000 0000 0000 0000 ed0c 0000  ................
+00003010: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
+00003020: 6565 7431 2e78 6d6c 504b 0102 2d00 1400  eet1.xmlPK..-...
+00003030: 0600 0800 0000 2100 31a2 f728 2203 0000  ......!.1..("...
+00003040: ea07 0000 1800 0000 0000 0000 0000 0000  ................
+00003050: 0000 3710 0000 786c 2f77 6f72 6b73 6865  ..7...xl/workshe
+00003060: 6574 732f 7368 6565 7432 2e78 6d6c 504b  ets/sheet2.xmlPK
+00003070: 0102 2d00 1400 0600 0800 0000 2100 b312  ..-.........!...
+00003080: 6292 4703 0000 3808 0000 1800 0000 0000  b.G...8.........
+00003090: 0000 0000 0000 0000 8f13 0000 786c 2f77  ............xl/w
+000030a0: 6f72 6b73 6865 6574 732f 7368 6565 7433  orksheets/sheet3
+000030b0: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
+000030c0: 0000 2100 0c86 c513 f102 0000 0007 0000  ..!.............
+000030d0: 1800 0000 0000 0000 0000 0000 0000 0c17  ................
+000030e0: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
+000030f0: 7368 6565 7434 2e78 6d6c 504b 0102 2d00  sheet4.xmlPK..-.
+00003100: 1400 0600 0800 0000 2100 9640 713c f102  ........!..@q<..
+00003110: 0000 0007 0000 1800 0000 0000 0000 0000  ................
+00003120: 0000 0000 331a 0000 786c 2f77 6f72 6b73  ....3...xl/works
+00003130: 6865 6574 732f 7368 6565 7435 2e78 6d6c  heets/sheet5.xml
+00003140: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
+00003150: c117 10be 4e07 0000 c620 0000 1300 0000  ....N.... ......
+00003160: 0000 0000 0000 0000 0000 5a1d 0000 786c  ..........Z...xl
+00003170: 2f74 6865 6d65 2f74 6865 6d65 312e 786d  /theme/theme1.xm
+00003180: 6c50 4b01 022d 0014 0006 0008 0000 0021  lPK..-.........!
+00003190: 0083 b677 5c7b 0300 00ce 0a00 000d 0000  ...w\{..........
+000031a0: 0000 0000 0000 0000 0000 00d9 2400 0078  ............$..x
+000031b0: 6c2f 7374 796c 6573 2e78 6d6c 504b 0102  l/styles.xmlPK..
+000031c0: 2d00 1400 0600 0800 0000 2100 a67a 14eb  -.........!..z..
+000031d0: e100 0000 a601 0000 1400 0000 0000 0000  ................
+000031e0: 0000 0000 0000 7f28 0000 786c 2f73 6861  .......(..xl/sha
+000031f0: 7265 6453 7472 696e 6773 2e78 6d6c 504b  redStrings.xmlPK
+00003200: 0102 2d00 1400 0600 0800 0000 2100 feec  ..-.........!...
+00003210: b726 4f01 0000 6302 0000 1100 0000 0000  .&O...c.........
+00003220: 0000 0000 0000 0000 9229 0000 646f 6350  .........)..docP
+00003230: 726f 7073 2f63 6f72 652e 786d 6c50 4b01  rops/core.xmlPK.
+00003240: 022d 0014 0006 0008 0000 0021 002a d179  .-.........!.*.y
+00003250: cb95 0100 0064 0300 0010 0000 0000 0000  .....d..........
+00003260: 0000 0000 0000 0018 2c00 0064 6f63 5072  ........,..docPr
+00003270: 6f70 732f 6170 702e 786d 6c50 4b05 0600  ops/app.xmlPK...
+00003280: 0000 000e 000e 0098 0300 00e3 2e00 0000  ................
+00003290: 00                                       .
```

### Comparing `pyslope-1.1.9/pyslope/graphs/graphs.ipynb` & `pyslope-1.2.0/pyslope/graphs/graphs.ipynb`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/graphs/sandstone_fill_5m_1_1.html` & `pyslope-1.2.0/pyslope/graphs/sandstone_fill_5m_1_1.html`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/graphs/sandstone_fill_FOS_1.25_for_loads_and_angles.html` & `pyslope-1.2.0/pyslope/graphs/sandstone_fill_FOS_1.25_for_loads_and_angles.html`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope/pyslope.py` & `pyslope-1.2.0/pyslope/pyslope.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,5172 +1,5465 @@
 00000000: 2320 7374 616e 6461 7264 206c 6962 7261  # standard libra
 00000010: 7279 2069 6d70 6f72 7473 0a66 726f 6d20  ry imports.from 
 00000020: 6d61 7468 2069 6d70 6f72 7420 7261 6469  math import radi
 00000030: 616e 732c 2074 616e 2c20 7371 7274 2c20  ans, tan, sqrt, 
 00000040: 6174 616e 2c20 636f 732c 2073 696e 0a66  atan, cos, sin.f
 00000050: 726f 6d20 6461 7461 636c 6173 7365 7320  rom dataclasses 
 00000060: 696d 706f 7274 2064 6174 6163 6c61 7373  import dataclass
-00000070: 0a69 6d70 6f72 7420 6f73 0a0a 2320 7468  .import os..# th
-00000080: 6972 6420 7061 7274 7920 696d 706f 7274  ird party import
-00000090: 730a 6672 6f6d 2070 6c6f 746c 7920 696d  s.from plotly im
-000000a0: 706f 7274 2067 7261 7068 5f6f 626a 6563  port graph_objec
-000000b0: 7473 2061 7320 676f 0a66 726f 6d20 7471  ts as go.from tq
-000000c0: 646d 2069 6d70 6f72 7420 7471 646d 0a0a  dm import tqdm..
-000000d0: 2320 6861 7665 2074 6f20 646f 2074 6869  # have to do thi
-000000e0: 7320 746f 2061 6c6c 6f77 2066 6f72 2072  s to allow for r
-000000f0: 656c 6174 6976 6520 696d 706f 7274 730a  elative imports.
-00000100: 2320 6861 7665 2074 6f20 616c 6c6f 7720  # have to allow 
-00000110: 666f 7220 7265 6c61 7469 7665 2069 6d70  for relative imp
-00000120: 6f72 7473 2073 6f20 616c 736f 2077 6f72  orts so also wor
-00000130: 6b73 2077 6974 6820 646a 616e 676f 0a0a  ks with django..
-00000140: 2320 6966 2075 7369 6e67 2074 6869 7320  # if using this 
-00000150: 6669 6c65 206f 7220 7370 6869 6e78 2c20  file or sphinx, 
-00000160: 6361 6e74 2062 6520 7265 6c61 7469 7665  cant be relative
-00000170: 0a69 6620 5f5f 6e61 6d65 5f5f 203d 3d20  .if __name__ == 
-00000180: 225f 5f6d 6169 6e5f 5f22 206f 7220 5f5f  "__main__" or __
-00000190: 6e61 6d65 5f5f 203d 3d20 2270 7973 6c6f  name__ == "pyslo
-000001a0: 7065 223a 0a20 2020 2069 6d70 6f72 7420  pe":.    import 
-000001b0: 6461 7461 5f76 616c 6964 6174 696f 6e0a  data_validation.
-000001c0: 2020 2020 696d 706f 7274 2075 7469 6c69      import utili
-000001d0: 7469 6573 0a23 2069 6620 7275 6e6e 696e  ties.# if runnin
-000001e0: 6720 6672 6f6d 2064 6a61 6e67 6f20 6e65  g from django ne
-000001f0: 6564 2074 6f20 7573 6520 7265 6c61 7469  ed to use relati
-00000200: 7665 0a65 6c73 653a 0a20 2020 2066 726f  ve.else:.    fro
-00000210: 6d20 2e20 696d 706f 7274 2064 6174 615f  m . import data_
-00000220: 7661 6c69 6461 7469 6f6e 0a20 2020 2066  validation.    f
-00000230: 726f 6d20 2e20 696d 706f 7274 2075 7469  rom . import uti
-00000240: 6c69 7469 6573 0a0a 434f 4c4f 5552 5f46  lities..COLOUR_F
-00000250: 4f53 5f44 4943 542c 204d 4154 4552 4941  OS_DICT, MATERIA
-00000260: 4c5f 434f 4c4f 5253 203d 2075 7469 6c69  L_COLORS = utili
-00000270: 7469 6573 2e43 4f4c 4f55 525f 464f 535f  ties.COLOUR_FOS_
-00000280: 4449 4354 2c20 7574 696c 6974 6965 732e  DICT, utilities.
-00000290: 4d41 5445 5249 414c 5f43 4f4c 4f52 530a  MATERIAL_COLORS.
-000002a0: 4d41 585f 434f 4c4f 5552 5f4b 4559 203d  MAX_COLOUR_KEY =
-000002b0: 206d 6178 2843 4f4c 4f55 525f 464f 535f   max(COLOUR_FOS_
-000002c0: 4449 4354 290a 0a0a 4064 6174 6163 6c61  DICT)...@datacla
-000002d0: 7373 0a63 6c61 7373 204d 6174 6572 6961  ss.class Materia
-000002e0: 6c3a 0a20 2020 2022 2222 436c 6173 7320  l:.    """Class 
-000002f0: 7265 7072 6573 656e 7469 6e67 2067 656f  representing geo
-00000300: 6c6f 6769 6361 6c20 6d61 7465 7269 616c  logical material
-00000310: 2075 6e69 742e 0a0a 2020 2020 5061 7261   unit...    Para
-00000320: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
-00000330: 2d2d 2d2d 2d0a 2020 2020 756e 6974 5f77  -----.    unit_w
-00000340: 6569 6768 7420 3a20 666c 6f61 740a 2020  eight : float.  
-00000350: 2020 2020 2020 6d61 7465 7269 616c 2075        material u
-00000360: 6e69 7420 7765 6967 6874 2069 6e20 6b4e  nit weight in kN
-00000370: 2f6d 332c 2062 7920 6465 6661 756c 7420  /m3, by default 
-00000380: 3230 0a20 2020 2066 7269 6374 696f 6e5f  20.    friction_
-00000390: 616e 676c 653a 2069 6e74 0a20 2020 2020  angle: int.     
-000003a0: 2020 206d 6174 6572 6961 6c20 6672 6963     material fric
-000003b0: 7469 6f6e 2061 6e67 6c65 2069 6e20 6465  tion angle in de
-000003c0: 6772 6565 732c 2062 7920 6465 6661 756c  grees, by defaul
-000003d0: 7420 3335 0a20 2020 2063 6f68 6573 696f  t 35.    cohesio
-000003e0: 6e20 3a20 696e 740a 2020 2020 2020 2020  n : int.        
-000003f0: 6d61 7465 7269 616c 2063 6f68 6573 696f  material cohesio
-00000400: 6e20 696e 206b 5061 2c20 6279 2064 6566  n in kPa, by def
-00000410: 6175 6c74 2032 0a20 2020 2064 6570 7468  ault 2.    depth
-00000420: 5f74 6f5f 626f 7474 6f6d 203a 2066 6c6f  _to_bottom : flo
-00000430: 6174 0a20 2020 2020 2020 2064 6570 7468  at.        depth
-00000440: 2074 6f20 7468 6520 626f 7474 6f6d 206f   to the bottom o
-00000450: 6620 7468 6520 6d61 7465 7269 616c 2073  f the material s
-00000460: 7472 6174 6120 6672 6f6d 2074 6865 2074  trata from the t
-00000470: 6f70 0a20 2020 2020 2020 206f 6620 7468  op.        of th
-00000480: 6520 736c 6f70 652c 2062 7920 6465 6661  e slope, by defa
-00000490: 756c 7420 352e 204e 6f74 652c 206d 6174  ult 5. Note, mat
-000004a0: 6572 6961 6c73 2061 7373 6967 6e65 6420  erials assigned 
-000004b0: 746f 0a20 2020 2020 2020 2061 2073 6c6f  to.        a slo
-000004c0: 7065 206d 7573 7420 6861 7665 2061 2075  pe must have a u
-000004d0: 6e69 7175 6520 6465 7074 685f 746f 5f62  nique depth_to_b
-000004e0: 6f74 746f 6d20 6f72 2061 6e20 6572 726f  ottom or an erro
-000004f0: 720a 2020 2020 2020 2020 7769 6c6c 2062  r.        will b
-00000500: 6520 7261 6973 6564 2e0a 2020 2020 6e61  e raised..    na
-00000510: 6d65 203a 2073 7472 2028 6f70 7469 6f6e  me : str (option
-00000520: 616c 290a 2020 2020 2020 2020 6e61 6d65  al).        name
-00000530: 206f 6620 7468 6520 7374 7261 7461 0a20   of the strata. 
-00000540: 2020 2063 6f6c 6f72 203a 2073 7472 2028     color : str (
-00000550: 6f70 7469 6f6e 616c 290a 2020 2020 2020  optional).      
-00000560: 2020 636f 6c6f 7220 746f 2062 6520 7573    color to be us
-00000570: 6564 2074 6f20 7265 7072 6573 656e 7420  ed to represent 
-00000580: 7468 6520 7374 7261 7461 2077 6865 6e20  the strata when 
-00000590: 706c 6f74 7469 6e67 2e20 436f 6c6f 720a  plotting. Color.
-000005a0: 2020 2020 2020 2020 6d61 7920 6265 2070          may be p
-000005b0: 726f 7669 6465 6420 6173 2061 2073 7472  rovided as a str
-000005c0: 696e 672c 2073 7461 6e64 6172 6420 3320  ing, standard 3 
-000005d0: 6865 7820 6469 6769 7420 6f72 2036 2068  hex digit or 6 h
-000005e0: 6578 2064 6967 6974 0a20 2020 2020 2020  ex digit.       
-000005f0: 2077 6562 2063 6f6d 7061 7469 626c 6520   web compatible 
-00000600: 7265 7072 6573 656e 7461 7469 6f6e 2e20  representation. 
-00000610: 4966 206e 6f74 2070 726f 7669 6465 6420  If not provided 
-00000620: 636f 6c6f 7220 6175 746f 6d61 7469 6361  color automatica
-00000630: 6c6c 790a 2020 2020 2020 2020 6173 7369  lly.        assi
-00000640: 676e 6564 2e0a 0a20 2020 2045 7861 6d70  gned...    Examp
-00000650: 6c65 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  les.    --------
-00000660: 2d2d 2d2d 0a20 2020 203e 3e3e 204d 6174  ----.    >>> Mat
-00000670: 6572 6961 6c28 3230 2c33 352c 322c 3529  erial(20,35,2,5)
-00000680: 0a20 2020 204d 6174 6572 6961 6c3a 2875  .    Material:(u
-00000690: 773d 3230 2c70 6869 3d33 352c 633d 322c  w=20,phi=35,c=2,
-000006a0: 645f 626f 743d 3529 0a20 2020 203e 3e3e  d_bot=5).    >>>
-000006b0: 204d 6174 6572 6961 6c28 290a 2020 2020   Material().    
-000006c0: 4d61 7465 7269 616c 3a28 7577 3d32 302c  Material:(uw=20,
-000006d0: 7068 693d 3335 2c63 3d32 2c64 5f62 6f74  phi=35,c=2,d_bot
-000006e0: 3d35 290a 2020 2020 3e3e 3e20 6120 3d20  =5).    >>> a = 
-000006f0: 4d61 7465 7269 616c 2829 0a20 2020 203e  Material().    >
-00000700: 3e3e 2061 2e63 6f68 6573 696f 6e20 3d3d  >> a.cohesion ==
-00000710: 2032 0a20 2020 2054 7275 650a 0a0a 2020   2.    True...  
-00000720: 2020 2222 220a 0a20 2020 2075 6e69 745f    """..    unit_
-00000730: 7765 6967 6874 3a20 666c 6f61 7420 3d20  weight: float = 
-00000740: 3230 0a20 2020 2066 7269 6374 696f 6e5f  20.    friction_
-00000750: 616e 676c 653a 2069 6e74 203d 2033 350a  angle: int = 35.
-00000760: 2020 2020 636f 6865 7369 6f6e 3a20 696e      cohesion: in
-00000770: 7420 3d20 320a 2020 2020 6465 7074 685f  t = 2.    depth_
-00000780: 746f 5f62 6f74 746f 6d3a 2066 6c6f 6174  to_bottom: float
-00000790: 203d 2035 0a20 2020 206e 616d 653a 2073   = 5.    name: s
-000007a0: 7472 203d 2022 220a 2020 2020 636f 6c6f  tr = "".    colo
-000007b0: 723a 2073 7472 203d 2022 220a 0a20 2020  r: str = ""..   
-000007c0: 2064 6566 205f 5f70 6f73 745f 696e 6974   def __post_init
-000007d0: 5f5f 2873 656c 6629 3a0a 2020 2020 2020  __(self):.      
-000007e0: 2020 6461 7461 5f76 616c 6964 6174 696f    data_validatio
-000007f0: 6e2e 6173 7365 7274 5f72 616e 6765 2873  n.assert_range(s
-00000800: 656c 662e 756e 6974 5f77 6569 6768 742c  elf.unit_weight,
-00000810: 2022 756e 6974 2077 6569 6768 7422 2c20   "unit weight", 
-00000820: 312c 2035 3029 0a20 2020 2020 2020 2064  1, 50).        d
-00000830: 6174 615f 7661 6c69 6461 7469 6f6e 2e61  ata_validation.a
-00000840: 7373 6572 745f 706f 7369 7469 7665 5f6e  ssert_positive_n
-00000850: 756d 6265 7228 7365 6c66 2e66 7269 6374  umber(self.frict
-00000860: 696f 6e5f 616e 676c 652c 2022 6672 6963  ion_angle, "fric
-00000870: 7469 6f6e 5f61 6e67 6c65 2229 0a20 2020  tion_angle").   
-00000880: 2020 2020 2064 6174 615f 7661 6c69 6461       data_valida
-00000890: 7469 6f6e 2e61 7373 6572 745f 6e75 6d62  tion.assert_numb
-000008a0: 6572 2873 656c 662e 636f 6865 7369 6f6e  er(self.cohesion
-000008b0: 2c20 2263 6f68 6573 696f 6e22 290a 2020  , "cohesion").  
-000008c0: 2020 2020 2020 6461 7461 5f76 616c 6964        data_valid
-000008d0: 6174 696f 6e2e 6173 7365 7274 5f6e 756d  ation.assert_num
-000008e0: 6265 7228 7365 6c66 2e64 6570 7468 5f74  ber(self.depth_t
-000008f0: 6f5f 626f 7474 6f6d 2c20 2264 6570 7468  o_bottom, "depth
-00000900: 2074 6f20 626f 7474 6f6d 2229 0a0a 2020   to bottom")..  
-00000910: 2020 2020 2020 2320 6966 2075 7365 7220        # if user 
-00000920: 6769 7665 7320 6120 6e65 6761 7469 7665  gives a negative
-00000930: 2076 616c 7565 206a 7573 7420 6d61 6b65   value just make
-00000940: 2069 7420 706f 7369 7469 7665 2069 6e73   it positive ins
-00000950: 7465 6164 2e0a 2020 2020 2020 2020 7365  tead..        se
-00000960: 6c66 2e63 6f68 6573 696f 6e20 3d20 6162  lf.cohesion = ab
-00000970: 7328 7365 6c66 2e63 6f68 6573 696f 6e29  s(self.cohesion)
-00000980: 0a20 2020 2020 2020 2073 656c 662e 6465  .        self.de
-00000990: 7074 685f 746f 5f62 6f74 746f 6d20 3d20  pth_to_bottom = 
-000009a0: 6162 7328 7365 6c66 2e64 6570 7468 5f74  abs(self.depth_t
-000009b0: 6f5f 626f 7474 6f6d 290a 0a20 2020 2020  o_bottom)..     
-000009c0: 2020 2069 6620 7365 6c66 2e6e 616d 6520     if self.name 
-000009d0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-000009e0: 2020 2020 2073 656c 662e 6e61 6d65 203d       self.name =
-000009f0: 2022 220a 2020 2020 2020 2020 6966 2073   "".        if s
-00000a00: 656c 662e 636f 6c6f 7220 6973 204e 6f6e  elf.color is Non
-00000a10: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00000a20: 656c 662e 636f 6c6f 7220 3d20 2222 0a0a  elf.color = ""..
-00000a30: 2020 2020 2020 2020 6173 7365 7274 2069          assert i
-00000a40: 7369 6e73 7461 6e63 6528 7365 6c66 2e6e  sinstance(self.n
-00000a50: 616d 652c 2073 7472 290a 2020 2020 2020  ame, str).      
-00000a60: 2020 6173 7365 7274 2069 7369 6e73 7461    assert isinsta
-00000a70: 6e63 6528 7365 6c66 2e63 6f6c 6f72 2c20  nce(self.color, 
-00000a80: 7374 7229 0a0a 2020 2020 2020 2020 2320  str)..        # 
-00000a90: 6e65 6564 2074 6f20 6465 6669 6e65 2073  need to define s
-00000aa0: 6570 6572 6174 6520 746f 2063 6f6c 6f72  eperate to color
-00000ab0: 2073 696e 6365 2063 6f6c 6f72 2070 726f   since color pro
-00000ac0: 7065 7274 7920 6973 2063 6861 6e67 6564  perty is changed
-00000ad0: 0a20 2020 2020 2020 2023 2077 6865 6e20  .        # when 
-00000ae0: 7573 6572 2064 6566 696e 6564 2063 6f6c  user defined col
-00000af0: 6f72 2064 6f65 736e 7420 6578 6973 742e  or doesnt exist.
-00000b00: 2054 6865 7265 2077 6173 2061 2064 6566   There was a def
-00000b10: 696e 6520 666c 6f6f 720a 2020 2020 2020  ine floor.      
-00000b20: 2020 2320 7072 6576 696f 7573 6c79 2073    # previously s
-00000b30: 696e 6365 2077 6865 6e20 7265 6d6f 7669  ince when removi
-00000b40: 6e67 206d 6174 6572 6961 6c73 2074 6865  ng materials the
-00000b50: 2063 6f6c 6f72 2066 6f72 2061 646a 6563   color for adjec
-00000b60: 656e 740a 2020 2020 2020 2020 2320 6d61  ent.        # ma
-00000b70: 7465 7269 616c 7320 636f 756c 6420 6265  terials could be
-00000b80: 636f 6d65 2074 6865 2073 616d 652e 0a20  come the same.. 
-00000b90: 2020 2020 2020 2023 2043 6f6d 6d65 6e74         # Comment
-00000ba0: 2066 726f 6d20 4a65 7373 6520 422c 2031   from Jesse B, 1
-00000bb0: 342e 3033 2e32 320a 2020 2020 2020 2020  4.03.22.        
-00000bc0: 7365 6c66 2e75 7365 725f 6465 6669 6e65  self.user_define
-00000bd0: 645f 636f 6c6f 7220 3d20 7365 6c66 2e63  d_color = self.c
-00000be0: 6f6c 6f72 0a0a 2020 2020 6465 6620 5f5f  olor..    def __
-00000bf0: 7265 7072 5f5f 2873 656c 6629 3a0a 2020  repr__(self):.  
-00000c00: 2020 2020 2020 7265 7475 726e 2028 0a20        return (. 
-00000c10: 2020 2020 2020 2020 2020 2066 224d 6174             f"Mat
-00000c20: 6572 6961 6c3a 7b73 656c 662e 6e61 6d65  erial:{self.name
-00000c30: 7d22 0a20 2020 2020 2020 2020 2020 2066  }".            f
-00000c40: 2228 7577 3d7b 7365 6c66 2e75 6e69 745f  "(uw={self.unit_
-00000c50: 7765 6967 6874 7d2c 220a 2020 2020 2020  weight},".      
-00000c60: 2020 2020 2020 6622 7068 693d 7b73 656c        f"phi={sel
-00000c70: 662e 6672 6963 7469 6f6e 5f61 6e67 6c65  f.friction_angle
-00000c80: 7d2c 220a 2020 2020 2020 2020 2020 2020  },".            
-00000c90: 6622 633d 7b73 656c 662e 636f 6865 7369  f"c={self.cohesi
-00000ca0: 6f6e 7d2c 220a 2020 2020 2020 2020 2020  on},".          
-00000cb0: 2020 6622 645f 626f 743d 7b73 656c 662e    f"d_bot={self.
-00000cc0: 6465 7074 685f 746f 5f62 6f74 746f 6d7d  depth_to_bottom}
-00000cd0: 2922 0a20 2020 2020 2020 2029 0a0a 0a40  )".        )...@
-00000ce0: 6461 7461 636c 6173 730a 636c 6173 7320  dataclass.class 
-00000cf0: 5564 6c3a 0a20 2020 2022 2222 436c 6173  Udl:.    """Clas
-00000d00: 7320 7265 7072 6573 656e 7469 6e67 2075  s representing u
-00000d10: 6e69 666f 726d 6c79 2064 6973 7472 6962  niformly distrib
-00000d20: 7574 6564 2073 7572 6661 6365 2070 7265  uted surface pre
-00000d30: 7373 7572 6520 696e 206b 5061 0a0a 2020  ssure in kPa..  
-00000d40: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-00000d50: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00000d60: 6d61 676e 6974 7564 6520 3a20 666c 6f61  magnitude : floa
-00000d70: 740a 2020 2020 2020 2020 6d61 676e 6974  t.        magnit
-00000d80: 7564 6520 6f66 2055 444c 2066 6f72 6365  ude of UDL force
-00000d90: 2069 6e20 6b50 610a 2020 2020 6f66 6673   in kPa.    offs
-00000da0: 6574 203a 2066 6c6f 6174 0a20 2020 2020  et : float.     
-00000db0: 2020 206f 6666 7365 7420 6f66 206c 6f61     offset of loa
-00000dc0: 6420 6672 6f6d 2073 6c6f 7065 2069 6e20  d from slope in 
-00000dd0: 6d0a 2020 2020 6c65 6e67 7468 203a 2066  m.    length : f
-00000de0: 6c6f 6174 0a20 2020 2020 2020 206c 656e  loat.        len
-00000df0: 6774 6820 6f66 206c 6f61 6420 696e 206d  gth of load in m
-00000e00: 2c20 6966 2030 206f 7220 4e6f 6e65 2074  , if 0 or None t
-00000e10: 6865 6e20 6173 7375 6d65 6420 636f 6e74  hen assumed cont
-00000e20: 696e 756f 7573 2e0a 2020 2020 2020 2020  inuous..        
-00000e30: 4279 2064 6566 6175 6c74 204e 6f6e 652e  By default None.
-00000e40: 0a20 2020 2063 6f6c 6f72 203a 2073 7472  .    color : str
-00000e50: 2028 6f70 7469 6f6e 616c 290a 2020 2020   (optional).    
-00000e60: 2020 2020 636f 6c6f 7220 746f 2062 6520      color to be 
-00000e70: 7573 6564 2074 6f20 7265 7072 6573 656e  used to represen
-00000e80: 7420 7468 6520 7374 7261 7461 2077 6865  t the strata whe
-00000e90: 6e20 706c 6f74 7469 6e67 2e20 436f 6c6f  n plotting. Colo
-00000ea0: 720a 2020 2020 2020 2020 6d61 7920 6265  r.        may be
-00000eb0: 2070 726f 7669 6465 6420 6173 2061 2073   provided as a s
-00000ec0: 7472 696e 672c 2073 7461 6e64 6172 6420  tring, standard 
-00000ed0: 3320 6865 7820 6469 6769 7420 6f72 2036  3 hex digit or 6
-00000ee0: 2068 6578 2064 6967 6974 0a20 2020 2020   hex digit.     
-00000ef0: 2020 2077 6562 2063 6f6d 7061 7469 626c     web compatibl
-00000f00: 6520 7265 7072 6573 656e 7461 7469 6f6e  e representation
-00000f10: 2e20 4966 206e 6f74 2070 726f 7669 6465  . If not provide
-00000f20: 6420 636f 6c6f 7220 6175 746f 6d61 7469  d color automati
-00000f30: 6361 6c6c 790a 2020 2020 2020 2020 6173  cally.        as
-00000f40: 7369 676e 6564 2e0a 2020 2020 6479 6e61  signed..    dyna
-00000f50: 6d69 635f 6f66 6673 6574 203a 2062 6f6f  mic_offset : boo
-00000f60: 6c0a 2020 2020 2020 2020 4966 2054 7275  l.        If Tru
-00000f70: 6520 7468 656e 2074 6865 206c 6f61 6420  e then the load 
-00000f80: 6f66 6673 6574 2077 696c 6c20 6265 2064  offset will be d
-00000f90: 796e 616d 6963 616c 6c79 206d 6f76 6564  ynamically moved
-00000fa0: 2069 6620 6120 2264 796e 616d 6963 0a20   if a "dynamic. 
-00000fb0: 2020 2020 2020 2061 6e61 6c79 7369 7322         analysis"
-00000fc0: 2069 7320 7275 6e2e 2028 466f 7220 6120   is run. (For a 
-00000fd0: 7374 616e 6461 7264 2061 6e61 6c79 7369  standard analysi
-00000fe0: 7320 7468 6520 6f66 6673 6574 2076 616c  s the offset val
-00000ff0: 7565 2069 7320 7374 696c 6c20 7573 6564  ue is still used
-00001000: 292e 0a20 2020 2020 2020 2042 7920 6465  )..        By de
-00001010: 6661 756c 7420 4661 6c73 652e 0a0a 2020  fault False...  
-00001020: 2020 4578 616d 706c 6573 0a20 2020 202d    Examples.    -
-00001030: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
-00001040: 3e3e 3e20 5564 6c28 6d61 676e 6974 7564  >>> Udl(magnitud
-00001050: 6520 3d20 3130 2c20 6f66 6673 6574 203d  e = 10, offset =
-00001060: 2031 2c20 6c65 6e67 7468 203d 2032 2c20   1, length = 2, 
-00001070: 636f 6c6f 7220 3d20 2270 696e 6b22 290a  color = "pink").
-00001080: 2020 2020 5544 4c3a 2031 3020 6b50 612c      UDL: 10 kPa,
-00001090: 206f 6666 7365 7420 3d20 3120 6d2c 206c   offset = 1 m, l
-000010a0: 6f61 6420 6c65 6e67 7468 203d 2032 206d  oad length = 2 m
-000010b0: 0a20 2020 203e 3e3e 2055 646c 2829 0a20  .    >>> Udl(). 
-000010c0: 2020 2055 444c 3a20 3020 6b50 612c 206f     UDL: 0 kPa, o
-000010d0: 6666 7365 7420 3d20 3020 6d2c 206c 6f61  ffset = 0 m, loa
-000010e0: 6420 6c65 6e67 7468 203d 204e 6f6e 6520  d length = None 
-000010f0: 6d0a 2020 2020 3e3e 3e20 6120 3d20 5564  m.    >>> a = Ud
-00001100: 6c28 290a 2020 2020 3e3e 3e20 612e 6d61  l().    >>> a.ma
-00001110: 676e 6974 7564 6520 3d3d 2030 0a20 2020  gnitude == 0.   
-00001120: 2054 7275 650a 0a20 2020 2022 2222 0a0a   True..    """..
-00001130: 2020 2020 6d61 676e 6974 7564 653a 2066      magnitude: f
-00001140: 6c6f 6174 203d 2030 0a20 2020 206f 6666  loat = 0.    off
-00001150: 7365 743a 2066 6c6f 6174 203d 2030 0a20  set: float = 0. 
-00001160: 2020 206c 656e 6774 683a 2066 6c6f 6174     length: float
-00001170: 203d 204e 6f6e 650a 2020 2020 636f 6c6f   = None.    colo
-00001180: 723a 2073 7472 203d 2022 7265 6422 0a20  r: str = "red". 
-00001190: 2020 2064 796e 616d 6963 5f6f 6666 7365     dynamic_offse
-000011a0: 743a 2062 6f6f 6c20 3d20 4661 6c73 650a  t: bool = False.
-000011b0: 0a20 2020 2064 6566 205f 5f70 6f73 745f  .    def __post_
-000011c0: 696e 6974 5f5f 2873 656c 6629 3a0a 2020  init__(self):.  
-000011d0: 2020 2020 2020 6461 7461 5f76 616c 6964        data_valid
-000011e0: 6174 696f 6e2e 6173 7365 7274 5f6e 756d  ation.assert_num
-000011f0: 6265 7228 7365 6c66 2e6d 6167 6e69 7475  ber(self.magnitu
-00001200: 6465 2c20 226c 6f61 6420 6d61 676e 6974  de, "load magnit
-00001210: 7564 6522 290a 2020 2020 2020 2020 6461  ude").        da
-00001220: 7461 5f76 616c 6964 6174 696f 6e2e 6173  ta_validation.as
-00001230: 7365 7274 5f6e 756d 6265 7228 7365 6c66  sert_number(self
-00001240: 2e6f 6666 7365 742c 2022 6c6f 6164 206f  .offset, "load o
-00001250: 6666 7365 7422 290a 0a20 2020 2020 2020  ffset")..       
-00001260: 2069 6620 7365 6c66 2e6c 656e 6774 683a   if self.length:
-00001270: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-00001280: 615f 7661 6c69 6461 7469 6f6e 2e61 7373  a_validation.ass
-00001290: 6572 745f 6e75 6d62 6572 2873 656c 662e  ert_number(self.
-000012a0: 6c65 6e67 7468 2c20 226c 6f61 6420 6c65  length, "load le
-000012b0: 6e67 7468 2229 0a20 2020 2020 2020 2020  ngth").         
-000012c0: 2020 2073 656c 662e 6c65 6e67 7468 203d     self.length =
-000012d0: 2061 6273 2873 656c 662e 6c65 6e67 7468   abs(self.length
-000012e0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-000012f0: 2020 2020 2020 2020 2020 2020 2320 6d61              # ma
-00001300: 6b65 206e 6f6e 6520 6966 206c 656e 6774  ke none if lengt
-00001310: 6820 3d20 303f 0a20 2020 2020 2020 2020  h = 0?.         
-00001320: 2020 2073 656c 662e 6c65 6e67 7468 203d     self.length =
-00001330: 204e 6f6e 650a 0a20 2020 2020 2020 2073   None..        s
-00001340: 656c 662e 6d61 676e 6974 7564 6520 3d20  elf.magnitude = 
-00001350: 6162 7328 7365 6c66 2e6d 6167 6e69 7475  abs(self.magnitu
-00001360: 6465 290a 2020 2020 2020 2020 7365 6c66  de).        self
-00001370: 2e6f 6666 7365 7420 3d20 6162 7328 7365  .offset = abs(se
-00001380: 6c66 2e6f 6666 7365 7429 0a0a 2020 2020  lf.offset)..    
-00001390: 2020 2020 7365 6c66 2e70 7265 6369 7369      self.precisi
-000013a0: 6f6e 203d 2075 7469 6c69 7469 6573 2e67  on = utilities.g
-000013b0: 6574 5f70 7265 6369 7369 6f6e 2873 656c  et_precision(sel
-000013c0: 662e 6d61 676e 6974 7564 6529 0a0a 2020  f.magnitude)..  
-000013d0: 2020 2020 2020 6966 206e 6f74 2075 7469        if not uti
-000013e0: 6c69 7469 6573 2e69 735f 636f 6c6f 7228  lities.is_color(
-000013f0: 7365 6c66 2e63 6f6c 6f72 293a 0a20 2020  self.color):.   
-00001400: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-00001410: 6c6f 7220 3d20 2272 6564 220a 0a20 2020  lor = "red"..   
-00001420: 2064 6566 205f 5f72 6570 725f 5f28 7365   def __repr__(se
-00001430: 6c66 293a 0a20 2020 2020 2020 2072 6574  lf):.        ret
-00001440: 7572 6e20 6622 5544 4c3a 207b 7365 6c66  urn f"UDL: {self
-00001450: 2e6d 6167 6e69 7475 6465 7d20 6b50 612c  .magnitude} kPa,
-00001460: 206f 6666 7365 7420 3d20 7b73 656c 662e   offset = {self.
-00001470: 6f66 6673 6574 7d20 6d2c 206c 6f61 6420  offset} m, load 
-00001480: 6c65 6e67 7468 203d 207b 7365 6c66 2e6c  length = {self.l
-00001490: 656e 6774 687d 206d 220a 0a0a 4064 6174  ength} m"...@dat
-000014a0: 6163 6c61 7373 0a63 6c61 7373 204c 696e  aclass.class Lin
-000014b0: 654c 6f61 643a 0a20 2020 2022 2222 436c  eLoad:.    """Cl
-000014c0: 6173 7320 7265 7072 6573 656e 7469 6e67  ass representing
-000014d0: 206c 696e 6520 6c6f 6164 2069 6e20 6b4e   line load in kN
-000014e0: 2f6d 0a0a 2020 2020 5061 7261 6d65 7465  /m..    Paramete
-000014f0: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
-00001500: 2d0a 2020 2020 6d61 676e 6974 7564 6520  -.    magnitude 
-00001510: 3a20 666c 6f61 740a 2020 2020 2020 2020  : float.        
-00001520: 6d61 676e 6974 7564 6520 6f66 2055 444c  magnitude of UDL
-00001530: 2066 6f72 6365 2069 6e20 6b50 610a 2020   force in kPa.  
-00001540: 2020 6f66 6673 6574 203a 2066 6c6f 6174    offset : float
-00001550: 0a20 2020 2020 2020 206f 6666 7365 7420  .        offset 
-00001560: 6f66 206c 6f61 6420 6672 6f6d 2073 6c6f  of load from slo
-00001570: 7065 2069 6e20 6d0a 2020 2020 6c65 6e67  pe in m.    leng
-00001580: 7468 203a 2066 6c6f 6174 0a20 2020 2020  th : float.     
-00001590: 2020 206c 656e 6774 6820 6f66 206c 6f61     length of loa
-000015a0: 6420 696e 206d 2c20 6966 2030 206f 7220  d in m, if 0 or 
-000015b0: 4e6f 6e65 2074 6865 6e20 6173 7375 6d65  None then assume
-000015c0: 6420 636f 6e74 696e 756f 7573 2e0a 2020  d continuous..  
-000015d0: 2020 2020 2020 4279 2064 6566 6175 6c74        By default
-000015e0: 204e 6f6e 652e 0a20 2020 2063 6f6c 6f72   None..    color
-000015f0: 203a 2073 7472 2028 6f70 7469 6f6e 616c   : str (optional
-00001600: 290a 2020 2020 2020 2020 636f 6c6f 7220  ).        color 
-00001610: 746f 2062 6520 7573 6564 2074 6f20 7265  to be used to re
-00001620: 7072 6573 656e 7420 7468 6520 7374 7261  present the stra
-00001630: 7461 2077 6865 6e20 706c 6f74 7469 6e67  ta when plotting
-00001640: 2e20 436f 6c6f 720a 2020 2020 2020 2020  . Color.        
-00001650: 6d61 7920 6265 2070 726f 7669 6465 6420  may be provided 
-00001660: 6173 2061 2073 7472 696e 672c 2073 7461  as a string, sta
-00001670: 6e64 6172 6420 3320 6865 7820 6469 6769  ndard 3 hex digi
-00001680: 7420 6f72 2036 2068 6578 2064 6967 6974  t or 6 hex digit
-00001690: 0a20 2020 2020 2020 2077 6562 2063 6f6d  .        web com
-000016a0: 7061 7469 626c 6520 7265 7072 6573 656e  patible represen
-000016b0: 7461 7469 6f6e 2e20 4966 206e 6f74 2070  tation. If not p
-000016c0: 726f 7669 6465 6420 636f 6c6f 7220 6175  rovided color au
-000016d0: 746f 6d61 7469 6361 6c6c 790a 2020 2020  tomatically.    
-000016e0: 2020 2020 6173 7369 676e 6564 2e0a 2020      assigned..  
-000016f0: 2020 6479 6e61 6d69 635f 6f66 6673 6574    dynamic_offset
-00001700: 203a 2062 6f6f 6c0a 2020 2020 2020 2020   : bool.        
-00001710: 4966 2054 7275 6520 7468 656e 2074 6865  If True then the
-00001720: 206c 6f61 6420 6f66 6673 6574 2077 696c   load offset wil
-00001730: 6c20 6265 2064 796e 616d 6963 616c 6c79  l be dynamically
-00001740: 206d 6f76 6564 2069 6620 6120 2264 796e   moved if a "dyn
-00001750: 616d 6963 0a20 2020 2020 2020 2061 6e61  amic.        ana
-00001760: 6c79 7369 7322 2069 7320 7275 6e2e 2028  lysis" is run. (
-00001770: 466f 7220 6120 7374 616e 6461 7264 2061  For a standard a
-00001780: 6e61 6c79 7369 7320 7468 6520 6f66 6673  nalysis the offs
-00001790: 6574 2076 616c 7565 2069 7320 7374 696c  et value is stil
-000017a0: 6c20 7573 6564 292e 0a20 2020 2020 2020  l used)..       
-000017b0: 2042 7920 6465 6661 756c 7420 4661 6c73   By default Fals
-000017c0: 652e 0a20 2020 2022 2222 0a0a 2020 2020  e..    """..    
-000017d0: 6d61 676e 6974 7564 653a 2066 6c6f 6174  magnitude: float
-000017e0: 203d 2030 0a20 2020 206f 6666 7365 743a   = 0.    offset:
-000017f0: 2066 6c6f 6174 203d 2030 0a20 2020 2063   float = 0.    c
-00001800: 6f6c 6f72 3a20 7374 7220 3d20 2262 6c75  olor: str = "blu
-00001810: 6522 0a20 2020 2064 796e 616d 6963 5f6f  e".    dynamic_o
-00001820: 6666 7365 743a 2062 6f6f 6c20 3d20 4661  ffset: bool = Fa
-00001830: 6c73 650a 0a20 2020 2064 6566 205f 5f70  lse..    def __p
-00001840: 6f73 745f 696e 6974 5f5f 2873 656c 6629  ost_init__(self)
-00001850: 3a0a 2020 2020 2020 2020 6461 7461 5f76  :.        data_v
-00001860: 616c 6964 6174 696f 6e2e 6173 7365 7274  alidation.assert
-00001870: 5f6e 756d 6265 7228 7365 6c66 2e6d 6167  _number(self.mag
-00001880: 6e69 7475 6465 2c20 226c 6f61 6420 6d61  nitude, "load ma
-00001890: 676e 6974 7564 6522 290a 2020 2020 2020  gnitude").      
-000018a0: 2020 6461 7461 5f76 616c 6964 6174 696f    data_validatio
-000018b0: 6e2e 6173 7365 7274 5f6e 756d 6265 7228  n.assert_number(
-000018c0: 7365 6c66 2e6f 6666 7365 742c 2022 6c6f  self.offset, "lo
-000018d0: 6164 206f 6666 7365 7422 290a 0a20 2020  ad offset")..   
-000018e0: 2020 2020 2073 656c 662e 7072 6563 6973       self.precis
-000018f0: 696f 6e20 3d20 7574 696c 6974 6965 732e  ion = utilities.
-00001900: 6765 745f 7072 6563 6973 696f 6e28 7365  get_precision(se
-00001910: 6c66 2e6d 6167 6e69 7475 6465 290a 0a20  lf.magnitude).. 
-00001920: 2020 2020 2020 2073 656c 662e 6d61 676e         self.magn
-00001930: 6974 7564 6520 3d20 6162 7328 7365 6c66  itude = abs(self
-00001940: 2e6d 6167 6e69 7475 6465 290a 2020 2020  .magnitude).    
-00001950: 2020 2020 7365 6c66 2e6f 6666 7365 7420      self.offset 
-00001960: 3d20 6162 7328 7365 6c66 2e6f 6666 7365  = abs(self.offse
-00001970: 7429 0a0a 2020 2020 2020 2020 6966 206e  t)..        if n
-00001980: 6f74 2075 7469 6c69 7469 6573 2e69 735f  ot utilities.is_
-00001990: 636f 6c6f 7228 7365 6c66 2e63 6f6c 6f72  color(self.color
-000019a0: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-000019b0: 656c 662e 636f 6c6f 7220 3d20 2262 6c75  elf.color = "blu
-000019c0: 6522 0a0a 2020 2020 6465 6620 5f5f 7265  e"..    def __re
-000019d0: 7072 5f5f 2873 656c 6629 3a0a 2020 2020  pr__(self):.    
-000019e0: 2020 2020 7265 7475 726e 2066 224c 696e      return f"Lin
-000019f0: 653a 207b 7365 6c66 2e6d 6167 6e69 7475  e: {self.magnitu
-00001a00: 6465 7d20 6b4e 2f6d 2c20 6f66 6673 6574  de} kN/m, offset
-00001a10: 203d 207b 7365 6c66 2e6f 6666 7365 747d   = {self.offset}
-00001a20: 206d 220a 0a0a 636c 6173 7320 536c 6f70   m"...class Slop
-00001a30: 653a 0a20 2020 2022 2222 536c 6f70 6520  e:.    """Slope 
-00001a40: 6f62 6a65 6374 2e0a 0a20 2020 2050 6172  object...    Par
-00001a50: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
-00001a60: 2d2d 2d2d 2d2d 0a20 2020 2068 6569 6768  ------.    heigh
-00001a70: 7420 3a20 666c 6f61 740a 2020 2020 2020  t : float.      
-00001a80: 2020 6865 6967 6874 206f 6620 736c 6f70    height of slop
-00001a90: 6520 696e 206d 6574 7265 732c 2062 7920  e in metres, by 
-00001aa0: 6465 6661 756c 7420 320a 2020 2020 616e  default 2.    an
-00001ab0: 676c 6520 3a20 696e 742c 206f 7074 696f  gle : int, optio
-00001ac0: 6e61 6c0a 2020 2020 2020 2020 616e 676c  nal.        angl
-00001ad0: 6520 6f66 2073 6c6f 7065 2028 6f6e 6c79  e of slope (only
-00001ae0: 2075 7365 6420 6966 206c 656e 6774 6820   used if length 
-00001af0: 4e6f 6e65 292c 2062 7920 6465 6661 756c  None), by defaul
-00001b00: 7420 3330 0a20 2020 206c 656e 6774 6820  t 30.    length 
-00001b10: 3a20 666c 6f61 742c 206f 7074 696f 6e61  : float, optiona
-00001b20: 6c0a 2020 2020 2020 2020 6c65 6e67 7468  l.        length
-00001b30: 206f 6620 736c 6f70 6520 696e 206d 6574   of slope in met
-00001b40: 7265 732c 2062 7920 6465 6661 756c 7420  res, by default 
-00001b50: 4e6f 6e65 0a20 2020 2022 2222 0a0a 2020  None.    """..  
-00001b60: 2020 6465 6620 5f5f 7265 7072 5f5f 2873    def __repr__(s
-00001b70: 656c 6629 3a0a 2020 2020 2020 2020 7265  elf):.        re
-00001b80: 7475 726e 2066 2253 6c6f 7065 3a20 7b72  turn f"Slope: {r
-00001b90: 6f75 6e64 2873 656c 662e 5f68 6569 6768  ound(self._heigh
-00001ba0: 742c 3329 7d56 203a 207b 726f 756e 6428  t,3)}V : {round(
-00001bb0: 7365 6c66 2e5f 6c65 6e67 7468 2c33 297d  self._length,3)}
-00001bc0: 4822 0a0a 2020 2020 6465 6620 5f5f 696e  H"..    def __in
-00001bd0: 6974 5f5f 2873 656c 662c 2068 6569 6768  it__(self, heigh
-00001be0: 743a 2066 6c6f 6174 203d 2031 2c20 616e  t: float = 1, an
-00001bf0: 676c 653a 2069 6e74 203d 2033 302c 206c  gle: int = 30, l
-00001c00: 656e 6774 683a 2066 6c6f 6174 203d 204e  ength: float = N
-00001c10: 6f6e 6529 3a0a 0a20 2020 2020 2020 2023  one):..        #
-00001c20: 2069 6e69 7469 616c 6973 6520 656d 7074   initialise empt
-00001c30: 7920 7072 6f70 6572 7469 6573 2075 7365  y properties use
-00001c40: 6420 696e 206f 7468 6572 2063 6f6d 706f  d in other compo
-00001c50: 6e65 6e74 7320 6f66 2063 6c61 7373 0a20  nents of class. 
-00001c60: 2020 2020 2020 2073 656c 662e 5f6d 6174         self._mat
-00001c70: 6572 6961 6c73 203d 205b 5d0a 2020 2020  erials = [].    
-00001c80: 2020 2020 7365 6c66 2e5f 7761 7465 725f      self._water_
-00001c90: 524c 203d 204e 6f6e 650a 2020 2020 2020  RL = None.      
-00001ca0: 2020 7365 6c66 2e5f 7564 6c73 203d 205b    self._udls = [
-00001cb0: 5d0a 2020 2020 2020 2020 7365 6c66 2e5f  ].        self._
-00001cc0: 6c6c 7320 3d20 5b5d 0a0a 2020 2020 2020  lls = []..      
-00001cd0: 2020 2320 4e4f 5445 3a20 646f 6e74 2077    # NOTE: dont w
-00001ce0: 616e 7420 746f 2072 6573 6574 2077 6974  ant to reset wit
-00001cf0: 6820 6368 616e 6765 7320 746f 2074 6865  h changes to the
-00001d00: 206d 6f64 656c 2c20 6a75 7374 206e 6565   model, just nee
-00001d10: 6420 746f 2069 6e69 7469 616c 6973 6520  d to initialise 
-00001d20: 6865 7265 0a20 2020 2020 2020 2073 656c  here.        sel
-00001d30: 662e 5f64 796e 616d 6963 5f72 6573 756c  f._dynamic_resul
-00001d40: 7473 203d 207b 7d0a 2020 2020 2020 2020  ts = {}.        
-00001d50: 7365 6c66 2e5f 696e 6469 7669 6475 616c  self._individual
-00001d60: 5f70 6c61 6e65 7320 3d20 5b5d 0a0a 2020  _planes = []..  
-00001d70: 2020 2020 2020 7365 6c66 2e5f 6578 7465        self._exte
-00001d80: 726e 616c 5f62 6f75 6e64 6172 7920 3d20  rnal_boundary = 
-00001d90: 4e6f 6e65 0a0a 2020 2020 2020 2020 2320  None..        # 
-00001da0: 696e 7469 616c 6973 6520 6f70 7469 6f6e  intialise option
-00001db0: 730a 2020 2020 2020 2020 7365 6c66 2e75  s.        self.u
-00001dc0: 7064 6174 655f 626f 756e 6461 7279 5f6f  pdate_boundary_o
-00001dd0: 7074 696f 6e73 284d 494e 5f45 5854 5f48  ptions(MIN_EXT_H
-00001de0: 3d36 2c20 4d49 4e5f 4558 545f 4c3d 3130  =6, MIN_EXT_L=10
-00001df0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-00001e00: 6574 5f65 7874 6572 6e61 6c5f 626f 756e  et_external_boun
-00001e10: 6461 7279 2868 6569 6768 743d 6865 6967  dary(height=heig
-00001e20: 6874 2c20 616e 676c 653d 616e 676c 652c  ht, angle=angle,
-00001e30: 206c 656e 6774 683d 6c65 6e67 7468 290a   length=length).
-00001e40: 2020 2020 2020 2020 7365 6c66 2e75 7064          self.upd
-00001e50: 6174 655f 616e 616c 7973 6973 5f6f 7074  ate_analysis_opt
-00001e60: 696f 6e73 280a 2020 2020 2020 2020 2020  ions(.          
-00001e70: 2020 736c 6963 6573 3d32 352c 0a20 2020    slices=25,.   
-00001e80: 2020 2020 2020 2020 2069 7465 7261 7469           iterati
-00001e90: 6f6e 733d 3130 3030 2c0a 2020 2020 2020  ons=1000,.      
-00001ea0: 2020 2020 2020 6d69 6e5f 6661 696c 7572        min_failur
-00001eb0: 655f 6469 7374 3d30 2c0a 2020 2020 2020  e_dist=0,.      
-00001ec0: 2020 2020 2020 746f 6c65 7261 6e63 653d        tolerance=
-00001ed0: 302e 3030 352c 0a20 2020 2020 2020 2020  0.005,.         
-00001ee0: 2020 206d 6178 5f69 7465 7261 7469 6f6e     max_iteration
-00001ef0: 733d 3135 2c0a 2020 2020 2020 2020 290a  s=15,.        ).
-00001f00: 0a20 2020 2020 2020 2073 656c 662e 7570  .        self.up
-00001f10: 6461 7465 5f77 6174 6572 5f61 6e61 6c79  date_water_analy
-00001f20: 7369 735f 6f70 7469 6f6e 7328 6175 746f  sis_options(auto
-00001f30: 3d54 7275 6529 0a0a 2020 2020 2020 2020  =True)..        
-00001f40: 2320 7365 7473 2064 6566 6175 6c74 2061  # sets default a
-00001f50: 6e61 6c79 7369 7320 6c69 6d69 7473 2028  nalysis limits (
-00001f60: 6965 206e 6f20 6c69 6d69 7429 0a20 2020  ie no limit).   
-00001f70: 2020 2020 2073 656c 662e 7265 6d6f 7665       self.remove
-00001f80: 5f61 6e61 6c79 7369 735f 6c69 6d69 7473  _analysis_limits
-00001f90: 2829 0a0a 2020 2020 2320 636c 6561 7273  ()..    # clears
-00001fa0: 2073 6561 7263 6820 7661 6c75 652c 2072   search value, r
-00001fb0: 756e 2077 6865 6e20 6d6f 6465 6c20 7265  un when model re
-00001fc0: 7375 6c74 7320 6e6f 206c 6f6e 6765 7220  sults no longer 
-00001fd0: 7661 6c69 642e 0a20 2020 2064 6566 205f  valid..    def _
-00001fe0: 7265 7365 745f 7265 7375 6c74 7328 7365  reset_results(se
-00001ff0: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
-00002000: 662e 5f73 6561 7263 6820 3d20 5b5d 0a20  f._search = []. 
-00002010: 2020 2020 2020 2073 656c 662e 5f6d 696e         self._min
-00002020: 5f46 4f53 203d 2030 0a20 2020 2020 2020  _FOS = 0.       
-00002030: 2073 656c 662e 5f6d 696e 5f46 4f53 5f6c   self._min_FOS_l
-00002040: 6f63 6174 696f 6e20 3d20 5b5d 0a20 2020  ocation = [].   
-00002050: 2020 2020 2073 656c 662e 5f6d 696e 5f46       self._min_F
-00002060: 4f53 5f64 6963 7420 3d20 7b0a 2020 2020  OS_dict = {.    
-00002070: 2020 2020 2020 2020 2246 4f53 223a 2030          "FOS": 0
-00002080: 2c0a 2020 2020 2020 2020 2020 2020 226c  ,.            "l
-00002090: 5f63 223a 2030 2c0a 2020 2020 2020 2020  _c": 0,.        
-000020a0: 2020 2020 2272 5f63 223a 2030 2c0a 2020      "r_c": 0,.  
-000020b0: 2020 2020 2020 2020 2020 2263 5f78 223a            "c_x":
-000020c0: 2030 2c0a 2020 2020 2020 2020 2020 2020   0,.            
-000020d0: 2263 5f79 223a 2030 2c0a 2020 2020 2020  "c_y": 0,.      
-000020e0: 2020 2020 2020 2272 6164 6975 7322 3a20        "radius": 
-000020f0: 302c 0a20 2020 2020 2020 207d 0a0a 2020  0,.        }..  
-00002100: 2020 6465 6620 7365 745f 6578 7465 726e    def set_extern
-00002110: 616c 5f62 6f75 6e64 6172 7928 0a20 2020  al_boundary(.   
-00002120: 2020 2020 2073 656c 662c 2068 6569 6768       self, heigh
-00002130: 743a 2066 6c6f 6174 203d 2032 2c20 616e  t: float = 2, an
-00002140: 676c 653a 2069 6e74 203d 2033 302c 206c  gle: int = 30, l
-00002150: 656e 6774 683a 2066 6c6f 6174 203d 204e  ength: float = N
-00002160: 6f6e 650a 2020 2020 293a 0a20 2020 2020  one.    ):.     
-00002170: 2020 2022 2222 5365 7420 6578 7465 726e     """Set extern
-00002180: 616c 2062 6f75 6e64 6172 7920 666f 7220  al boundary for 
-00002190: 6d6f 6465 6c2e 0a0a 2020 2020 2020 2020  model...        
-000021a0: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
-000021b0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-000021c0: 2020 2020 2020 6865 6967 6874 203a 2066        height : f
-000021d0: 6c6f 6174 2c20 6f70 7469 6f6e 616c 0a20  loat, optional. 
-000021e0: 2020 2020 2020 2020 2020 2068 6569 6768             heigh
-000021f0: 7420 6f66 2073 6c6f 7065 2069 6e20 6d65  t of slope in me
-00002200: 7472 6573 2c20 6279 2064 6566 6175 6c74  tres, by default
-00002210: 2032 0a20 2020 2020 2020 2061 6e67 6c65   2.        angle
-00002220: 203a 2069 6e74 2c20 6f70 7469 6f6e 616c   : int, optional
-00002230: 0a20 2020 2020 2020 2020 2020 2061 6e67  .            ang
-00002240: 6c65 206f 6620 736c 6f70 6520 696e 2064  le of slope in d
-00002250: 6567 7265 6573 2028 6d61 7920 6265 206c  egrees (may be l
-00002260: 6566 7420 6173 206e 6f6e 6520 6966 2073  eft as none if s
-00002270: 6c6f 7065 0a20 2020 2020 2020 2020 2020  lope.           
-00002280: 2069 7320 696e 7374 6561 6420 6578 7072   is instead expr
-00002290: 6573 7365 6420 6279 206c 656e 6774 6820  essed by length 
-000022a0: 6f66 2073 6c6f 7065 292c 2062 7920 6465  of slope), by de
-000022b0: 6661 756c 7420 3330 0a20 2020 2020 2020  fault 30.       
-000022c0: 206c 656e 6774 6820 3a20 666c 6f61 742c   length : float,
-000022d0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-000022e0: 2020 2020 2020 6c65 6e67 7468 206f 6620        length of 
-000022f0: 736c 6f70 6520 696e 206d 6574 7265 7320  slope in metres 
-00002300: 286d 6179 2062 6520 6c65 6674 2061 7320  (may be left as 
-00002310: 6e6f 6e65 2069 6620 736c 6f70 650a 2020  none if slope.  
-00002320: 2020 2020 2020 2020 2020 6973 2069 6e73            is ins
-00002330: 7465 6164 2065 7870 7265 7373 6564 2062  tead expressed b
-00002340: 7920 616e 676c 6520 6f66 2073 6c6f 7065  y angle of slope
-00002350: 292c 2062 7920 6465 6661 756c 7420 4e6f  ), by default No
-00002360: 6e65 0a0a 2020 2020 2020 2020 5261 6973  ne..        Rais
-00002370: 6573 0a20 2020 2020 2020 202d 2d2d 2d2d  es.        -----
-00002380: 2d0a 2020 2020 2020 2020 5661 6c75 6545  -.        ValueE
-00002390: 7272 6f72 0a20 2020 2020 2020 2020 2020  rror.           
-000023a0: 2049 6620 696e 7075 7420 6e6f 7420 696e   If input not in
-000023b0: 2072 6571 7569 7265 6420 7261 6e67 6520   required range 
-000023c0: 6f72 206f 6620 7265 7175 6972 6564 2074  or of required t
-000023d0: 7970 650a 2020 2020 2020 2020 2222 220a  ype.        """.
-000023e0: 2020 2020 2020 2020 2320 7661 6c69 6461          # valida
-000023f0: 7465 2069 6e70 7574 730a 2020 2020 2020  te inputs.      
-00002400: 2020 6461 7461 5f76 616c 6964 6174 696f    data_validatio
-00002410: 6e2e 6173 7365 7274 5f73 7472 6963 746c  n.assert_strictl
-00002420: 795f 706f 7369 7469 7665 5f6e 756d 6265  y_positive_numbe
-00002430: 7228 6865 6967 6874 2c20 2268 6569 6768  r(height, "heigh
-00002440: 7422 290a 2020 2020 2020 2020 6966 2061  t").        if a
-00002450: 6e67 6c65 2069 7320 6e6f 7420 4e6f 6e65  ngle is not None
-00002460: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-00002470: 6973 2061 6c6c 6f77 6564 2074 6f20 6265  is allowed to be
-00002480: 2039 3020 6275 7420 6e6f 7420 300a 2020   90 but not 0.  
-00002490: 2020 2020 2020 2020 2020 6461 7461 5f76            data_v
-000024a0: 616c 6964 6174 696f 6e2e 6173 7365 7274  alidation.assert
-000024b0: 5f72 616e 6765 2861 6e67 6c65 2c20 2261  _range(angle, "a
-000024c0: 6e67 6c65 222c 2030 2c20 3930 2c20 6e6f  ngle", 0, 90, no
-000024d0: 745f 6c6f 773d 5472 7565 290a 2020 2020  t_low=True).    
-000024e0: 2020 2020 6966 206c 656e 6774 6820 6973      if length is
-000024f0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00002500: 2020 2020 2020 2064 6174 615f 7661 6c69         data_vali
-00002510: 6461 7469 6f6e 2e61 7373 6572 745f 706f  dation.assert_po
-00002520: 7369 7469 7665 5f6e 756d 6265 7228 6c65  sitive_number(le
-00002530: 6e67 7468 2c20 226c 656e 6774 6822 290a  ngth, "length").
-00002540: 0a20 2020 2020 2020 2023 2069 6620 616e  .        # if an
-00002550: 676c 6520 6173 7369 676e 6564 2069 6e73  gle assigned ins
-00002560: 7465 6164 206f 6620 6c65 6e67 7468 2077  tead of length w
-00002570: 6f72 6b20 6f75 7420 7468 6520 6d6f 6465  ork out the mode
-00002580: 6c20 6c65 6e67 7468 0a20 2020 2020 2020  l length.       
-00002590: 2069 6620 6c65 6e67 7468 2069 7320 4e6f   if length is No
-000025a0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000025b0: 6966 206e 6f74 2061 6e67 6c65 3a0a 2020  if not angle:.  
-000025c0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-000025d0: 6973 6520 5661 6c75 6545 7272 6f72 280a  ise ValueError(.
-000025e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025f0: 2020 2020 2272 6571 7569 7265 2061 6e67      "require ang
-00002600: 6c65 206f 6620 736c 6f70 6520 6f72 206c  le of slope or l
-00002610: 656e 6774 6820 6f66 2073 6c6f 7065 2074  ength of slope t
-00002620: 6f20 696e 6974 6961 6c69 7365 220a 2020  o initialise".  
-00002630: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00002640: 2020 2020 2020 2020 2020 2020 6c65 6e67              leng
-00002650: 7468 203d 2068 6569 6768 7420 2f20 7461  th = height / ta
-00002660: 6e28 7261 6469 616e 7328 616e 676c 6529  n(radians(angle)
-00002670: 290a 0a20 2020 2020 2020 2023 2068 656c  )..        # hel
-00002680: 7020 7769 7468 2064 6976 6973 696f 6e20  p with division 
-00002690: 6279 207a 6572 6f20 6572 726f 7273 0a20  by zero errors. 
-000026a0: 2020 2020 2020 206c 656e 6774 6820 3d20         length = 
-000026b0: 6d61 7828 6c65 6e67 7468 2c20 302e 3030  max(length, 0.00
-000026c0: 3129 0a0a 2020 2020 2020 2020 4d49 4e5f  1)..        MIN_
-000026d0: 4558 545f 4820 3d20 7365 6c66 2e5f 4d49  EXT_H = self._MI
-000026e0: 4e5f 4558 545f 480a 2020 2020 2020 2020  N_EXT_H.        
-000026f0: 4d49 4e5f 4558 545f 4c20 3d20 7365 6c66  MIN_EXT_L = self
-00002700: 2e5f 4d49 4e5f 4558 545f 4c0a 0a20 2020  ._MIN_EXT_L..   
-00002710: 2020 2020 2074 6f74 5f68 203d 206d 6178       tot_h = max
-00002720: 2833 202a 2068 6569 6768 742c 204d 494e  (3 * height, MIN
-00002730: 5f45 5854 5f48 2c20 3520 2a20 6c65 6e67  _EXT_H, 5 * leng
-00002740: 7468 202f 2032 290a 2020 2020 2020 2020  th / 2).        
-00002750: 746f 745f 6c20 3d20 6d61 7828 3520 2a20  tot_l = max(5 * 
-00002760: 6c65 6e67 7468 2c20 4d49 4e5f 4558 545f  length, MIN_EXT_
-00002770: 4c2c 2034 202a 2068 6569 6768 7429 0a0a  L, 4 * height)..
-00002780: 2020 2020 2020 2020 2320 6465 7465 726d          # determ
-00002790: 696e 6520 636f 6f72 6469 6e61 7465 7320  ine coordinates 
-000027a0: 666f 7220 6564 6765 7320 6f66 2073 6c6f  for edges of slo
-000027b0: 7065 0a20 2020 2020 2020 2064 7820 3d20  pe.        dx = 
-000027c0: 2874 6f74 5f6c 202d 206c 656e 6774 6829  (tot_l - length)
-000027d0: 202f 2032 0a20 2020 2020 2020 2074 6f70   / 2.        top
-000027e0: 203d 2028 6478 2c20 746f 745f 6829 0a20   = (dx, tot_h). 
-000027f0: 2020 2020 2020 2062 6f74 203d 2028 6478         bot = (dx
-00002800: 202b 206c 656e 6774 682c 2074 6f74 5f68   + length, tot_h
-00002810: 202d 2068 6569 6768 7429 0a0a 2020 2020   - height)..    
-00002820: 2020 2020 2320 7365 7420 7570 2065 7874      # set up ext
-00002830: 6572 6e61 6c20 626f 756e 6461 7279 2061  ernal boundary a
-00002840: 7320 6c69 7374 206f 6620 636f 6f72 6469  s list of coordi
-00002850: 6e61 7465 730a 2020 2020 2020 2020 7365  nates.        se
-00002860: 6c66 2e5f 6578 7465 726e 616c 5f62 6f75  lf._external_bou
-00002870: 6e64 6172 7920 3d20 5b0a 2020 2020 2020  ndary = [.      
-00002880: 2020 2020 2020 2830 2c20 3029 2c0a 2020        (0, 0),.  
-00002890: 2020 2020 2020 2020 2020 2830 2c20 746f            (0, to
-000028a0: 705b 315d 292c 0a20 2020 2020 2020 2020  p[1]),.         
-000028b0: 2020 2074 6f70 2c0a 2020 2020 2020 2020     top,.        
-000028c0: 2020 2020 626f 742c 0a20 2020 2020 2020      bot,.       
-000028d0: 2020 2020 2028 746f 745f 6c2c 2062 6f74       (tot_l, bot
-000028e0: 5b31 5d29 2c0a 2020 2020 2020 2020 2020  [1]),.          
-000028f0: 2020 2874 6f74 5f6c 2c20 3029 2c0a 2020    (tot_l, 0),.  
-00002900: 2020 2020 2020 2020 2020 2830 2c20 3029            (0, 0)
-00002910: 2c0a 2020 2020 2020 2020 5d0a 0a20 2020  ,.        ]..   
-00002920: 2020 2020 2023 2073 6574 2072 656c 6576       # set relev
-00002930: 616e 7420 7661 7269 6162 6c65 7320 746f  ant variables to
-00002940: 2073 656c 660a 2020 2020 2020 2020 7365   self.        se
-00002950: 6c66 2e5f 6c65 6e67 7468 203d 206c 656e  lf._length = len
-00002960: 6774 680a 2020 2020 2020 2020 7365 6c66  gth.        self
-00002970: 2e5f 6865 6967 6874 203d 2068 6569 6768  ._height = heigh
-00002980: 740a 2020 2020 2020 2020 7365 6c66 2e5f  t.        self._
-00002990: 6772 6164 6965 6e74 203d 2068 6569 6768  gradient = heigh
-000029a0: 7420 2f20 6c65 6e67 7468 0a0a 2020 2020  t / length..    
-000029b0: 2020 2020 7365 6c66 2e5f 746f 705f 636f      self._top_co
-000029c0: 6f72 6420 3d20 746f 700a 2020 2020 2020  ord = top.      
-000029d0: 2020 7365 6c66 2e5f 626f 745f 636f 6f72    self._bot_coor
-000029e0: 6420 3d20 626f 740a 0a20 2020 2020 2020  d = bot..       
-000029f0: 2073 656c 662e 5f65 7874 6572 6e61 6c5f   self._external_
-00002a00: 6c65 6e67 7468 203d 2074 6f74 5f6c 0a20  length = tot_l. 
-00002a10: 2020 2020 2020 2073 656c 662e 5f65 7874         self._ext
-00002a20: 6572 6e61 6c5f 6865 6967 6874 203d 2074  ernal_height = t
-00002a30: 6f74 5f68 0a0a 2020 2020 2020 2020 2320  ot_h..        # 
-00002a40: 7564 6c20 636f 6f72 6469 6e61 7465 7320  udl coordinates 
-00002a50: 6361 6e20 6265 2065 6666 6563 7465 6420  can be effected 
-00002a60: 6279 2065 7874 6572 6e61 6c20 626f 756e  by external boun
-00002a70: 6461 7279 206d 6f64 6966 6963 6174 696f  dary modificatio
-00002a80: 6e0a 2020 2020 2020 2020 2320 6e65 6564  n.        # need
-00002a90: 2074 6f20 7570 6461 7465 2063 6f6f 7264   to update coord
-00002aa0: 696e 6174 6573 2e0a 2020 2020 2020 2020  inates..        
-00002ab0: 7365 6c66 2e5f 7570 6461 7465 5f75 646c  self._update_udl
-00002ac0: 5f63 6f6f 7264 696e 6174 6573 2829 0a20  _coordinates(). 
-00002ad0: 2020 2020 2020 2073 656c 662e 5f75 7064         self._upd
-00002ae0: 6174 655f 6c6c 5f63 6f6f 7264 696e 6174  ate_ll_coordinat
-00002af0: 6573 2829 0a0a 2020 2020 2020 2020 2320  es()..        # 
-00002b00: 7265 7365 7420 6c69 6d69 7473 0a20 2020  reset limits.   
-00002b10: 2020 2020 2073 656c 662e 7265 6d6f 7665       self.remove
-00002b20: 5f61 6e61 6c79 7369 735f 6c69 6d69 7473  _analysis_limits
-00002b30: 2829 0a0a 2020 2020 2020 2020 2320 7265  ()..        # re
-00002b40: 7365 7420 7265 7375 6c74 730a 2020 2020  set results.    
-00002b50: 2020 2020 7365 6c66 2e5f 7265 7365 745f      self._reset_
-00002b60: 7265 7375 6c74 7328 290a 0a20 2020 2064  results()..    d
-00002b70: 6566 2073 6574 5f77 6174 6572 5f74 6162  ef set_water_tab
-00002b80: 6c65 2873 656c 662c 2064 6570 7468 3a20  le(self, depth: 
-00002b90: 666c 6f61 7429 3a0a 2020 2020 2020 2020  float):.        
-00002ba0: 2222 2273 6574 2077 6174 6572 2074 6162  """set water tab
-00002bb0: 6c65 2076 616c 7565 2e0a 0a20 2020 2020  le value...     
-00002bc0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-00002bd0: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-00002be0: 0a20 2020 2020 2020 2064 6570 7468 203a  .        depth :
-00002bf0: 2066 6c6f 6174 0a20 2020 2020 2020 2020   float.         
-00002c00: 2020 2064 6570 7468 206f 6620 7761 7465     depth of wate
-00002c10: 7220 6672 6f6d 2074 6f70 206f 6620 736c  r from top of sl
-00002c20: 6f70 652e 0a20 2020 2020 2020 2022 2222  ope..        """
-00002c30: 0a0a 2020 2020 2020 2020 6966 2064 6570  ..        if dep
-00002c40: 7468 2069 7320 4e6f 6e65 3a0a 2020 2020  th is None:.    
-00002c50: 2020 2020 2020 2020 7365 6c66 2e72 656d          self.rem
-00002c60: 6f76 655f 7761 7465 725f 7461 626c 6528  ove_water_table(
-00002c70: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-00002c80: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00002c90: 5f76 616c 6964 6174 696f 6e2e 6173 7365  _validation.asse
-00002ca0: 7274 5f70 6f73 6974 6976 655f 6e75 6d62  rt_positive_numb
-00002cb0: 6572 2864 6570 7468 2c20 2277 6174 6572  er(depth, "water
-00002cc0: 2064 6570 7468 2229 0a20 2020 2020 2020   depth").       
-00002cd0: 2020 2020 2073 656c 662e 5f77 6174 6572       self._water
-00002ce0: 5f52 4c20 3d20 6d61 7828 302c 2073 656c  _RL = max(0, sel
-00002cf0: 662e 5f74 6f70 5f63 6f6f 7264 5b31 5d20  f._top_coord[1] 
-00002d00: 2d20 6465 7074 6829 0a0a 2020 2020 2020  - depth)..      
-00002d10: 2020 2320 7265 7365 7420 7265 7375 6c74    # reset result
-00002d20: 730a 2020 2020 2020 2020 7365 6c66 2e5f  s.        self._
-00002d30: 7265 7365 745f 7265 7375 6c74 7328 290a  reset_results().
-00002d40: 0a20 2020 2064 6566 2072 656d 6f76 655f  .    def remove_
-00002d50: 7761 7465 725f 7461 626c 6528 7365 6c66  water_table(self
-00002d60: 293a 0a20 2020 2020 2020 2022 2222 5265  ):.        """Re
-00002d70: 6d6f 7665 2077 6174 6572 2074 6162 6c65  move water table
-00002d80: 2066 726f 6d20 6d6f 6465 6c22 2222 0a20   from model""". 
-00002d90: 2020 2020 2020 2073 656c 662e 5f77 6174         self._wat
-00002da0: 6572 5f52 4c20 3d20 4e6f 6e65 0a0a 2020  er_RL = None..  
-00002db0: 2020 2020 2020 2320 7265 7365 7420 7265        # reset re
-00002dc0: 7375 6c74 730a 2020 2020 2020 2020 7365  sults.        se
-00002dd0: 6c66 2e5f 7265 7365 745f 7265 7375 6c74  lf._reset_result
-00002de0: 7328 290a 0a20 2020 2064 6566 2073 6574  s()..    def set
-00002df0: 5f75 646c 7328 7365 6c66 2c20 2a75 646c  _udls(self, *udl
-00002e00: 7329 3a0a 2020 2020 2020 2020 2222 2273  s):.        """s
-00002e10: 6574 2061 2073 7572 6661 6365 2073 7572  et a surface sur
-00002e20: 6368 6172 6765 206f 6e20 746f 7020 6f66  charge on top of
-00002e30: 2074 6865 2073 6c6f 7065 2e0a 0a20 2020   the slope...   
-00002e40: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-00002e50: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00002e60: 2d2d 0a20 2020 2020 2020 202a 7564 6c73  --.        *udls
-00002e70: 203a 2055 646c 206f 626a 6563 7473 0a20   : Udl objects. 
-00002e80: 2020 2020 2020 2020 2020 2055 646c 206f             Udl o
-00002e90: 626a 6563 7420 746f 2062 6520 6173 7369  bject to be assi
-00002ea0: 676e 6564 2074 6f20 7468 6520 736c 6f70  gned to the slop
-00002eb0: 6520 6f62 6a65 6374 2e0a 2020 2020 2020  e object..      
-00002ec0: 2020 2222 220a 0a20 2020 2020 2020 2066    """..        f
-00002ed0: 6f72 2075 646c 2069 6e20 7564 6c73 3a0a  or udl in udls:.
-00002ee0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00002ef0: 7369 6e73 7461 6e63 6528 7564 6c2c 2055  sinstance(udl, U
-00002f00: 646c 293a 0a20 2020 2020 2020 2020 2020  dl):.           
-00002f10: 2020 2020 2069 6620 7564 6c2e 6d61 676e       if udl.magn
-00002f20: 6974 7564 6520 3e20 303a 0a20 2020 2020  itude > 0:.     
-00002f30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00002f40: 656c 662e 5f75 646c 732e 6170 7065 6e64  elf._udls.append
-00002f50: 2875 646c 290a 0a20 2020 2020 2020 2020  (udl)..         
-00002f60: 2020 2020 2020 2020 2020 2023 2075 7064             # upd
-00002f70: 6174 6520 746f 206d 616b 6520 7375 7265  ate to make sure
-00002f80: 2066 756c 6c20 6c6f 6164 2069 7320 696e   full load is in
-00002f90: 636c 7564 6564 0a20 2020 2020 2020 2020  cluded.         
-00002fa0: 2020 2020 2020 2020 2020 206d 696e 5f6c             min_l
-00002fb0: 656e 6774 6820 3d20 2875 646c 2e6f 6666  ength = (udl.off
-00002fc0: 7365 7420 2b20 2875 646c 2e6c 656e 6774  set + (udl.lengt
-00002fd0: 6820 6f72 2033 2929 202a 2032 2e35 0a20  h or 3)) * 2.5. 
-00002fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ff0: 2020 2069 6620 7365 6c66 2e5f 4d49 4e5f     if self._MIN_
-00003000: 4558 545f 4c20 3c20 6d69 6e5f 6c65 6e67  EXT_L < min_leng
-00003010: 7468 3a0a 2020 2020 2020 2020 2020 2020  th:.            
-00003020: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00003030: 2e75 7064 6174 655f 626f 756e 6461 7279  .update_boundary
-00003040: 5f6f 7074 696f 6e73 284d 494e 5f45 5854  _options(MIN_EXT
-00003050: 5f4c 3d6d 696e 5f6c 656e 6774 6829 0a0a  _L=min_length)..
-00003060: 2020 2020 2020 2020 7365 6c66 2e5f 7570          self._up
-00003070: 6461 7465 5f75 646c 5f63 6f6f 7264 696e  date_udl_coordin
-00003080: 6174 6573 2829 0a0a 2020 2020 2020 2020  ates()..        
-00003090: 6966 2073 656c 662e 5f75 646c 733a 0a20  if self._udls:. 
-000030a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000030b0: 5f75 646c 5f6d 6178 203d 206d 6178 2875  _udl_max = max(u
-000030c0: 646c 2e6d 6167 6e69 7475 6465 2066 6f72  dl.magnitude for
-000030d0: 2075 646c 2069 6e20 7365 6c66 2e5f 7564   udl in self._ud
-000030e0: 6c73 290a 0a20 2020 2020 2020 2023 2072  ls)..        # r
-000030f0: 6573 6574 2072 6573 756c 7473 0a20 2020  eset results.   
-00003100: 2020 2020 2073 656c 662e 5f72 6573 6574       self._reset
-00003110: 5f72 6573 756c 7473 2829 0a0a 2020 2020  _results()..    
-00003120: 2320 646f 6e74 206e 6565 6420 746f 2072  # dont need to r
-00003130: 6573 6574 2072 6573 756c 7473 2073 696e  eset results sin
-00003140: 6365 2074 6869 7320 6f6e 6c79 2073 686f  ce this only sho
-00003150: 756c 6420 6265 2063 616c 6c65 640a 2020  uld be called.  
-00003160: 2020 2320 6173 2061 2070 6172 7420 6f66    # as a part of
-00003170: 2072 6573 6574 7469 6e67 0a20 2020 2064   resetting.    d
-00003180: 6566 205f 7570 6461 7465 5f75 646c 5f63  ef _update_udl_c
-00003190: 6f6f 7264 696e 6174 6573 2873 656c 6629  oordinates(self)
-000031a0: 3a0a 2020 2020 2020 2020 2255 7064 6174  :.        "Updat
-000031b0: 6520 636f 6f72 6469 6e61 7465 7320 666f  e coordinates fo
-000031c0: 7220 6c65 6674 2061 6e64 2072 6967 6874  r left and right
-000031d0: 206f 6620 7564 6c20 6261 7365 6420 6f6e   of udl based on
-000031e0: 2065 7874 6572 6e61 6c20 626f 756e 6461   external bounda
-000031f0: 7279 2061 6e64 2055 646c 206f 626a 6563  ry and Udl objec
-00003200: 7422 0a0a 2020 2020 2020 2020 666f 7220  t"..        for 
-00003210: 7564 6c20 696e 2073 656c 662e 5f75 646c  udl in self._udl
-00003220: 733a 0a0a 2020 2020 2020 2020 2020 2020  s:..            
-00003230: 7269 6768 745f 7820 3d20 7365 6c66 2e5f  right_x = self._
-00003240: 746f 705f 636f 6f72 645b 305d 202d 2075  top_coord[0] - u
-00003250: 646c 2e6f 6666 7365 740a 2020 2020 2020  dl.offset.      
-00003260: 2020 2020 2020 6966 2075 646c 2e6c 656e        if udl.len
-00003270: 6774 683a 0a20 2020 2020 2020 2020 2020  gth:.           
-00003280: 2020 2020 206c 6566 745f 7820 3d20 6d61       left_x = ma
-00003290: 7828 302c 2072 6967 6874 5f78 202d 2075  x(0, right_x - u
-000032a0: 646c 2e6c 656e 6774 6829 0a20 2020 2020  dl.length).     
-000032b0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000032c0: 2020 2020 2020 2020 2020 2020 206c 6566               lef
-000032d0: 745f 7820 3d20 300a 0a20 2020 2020 2020  t_x = 0..       
-000032e0: 2020 2020 2075 646c 2e6c 6566 7420 3d20       udl.left = 
-000032f0: 6c65 6674 5f78 0a20 2020 2020 2020 2020  left_x.         
-00003300: 2020 2075 646c 2e72 6967 6874 203d 2072     udl.right = r
-00003310: 6967 6874 5f78 0a0a 2020 2020 6465 6620  ight_x..    def 
-00003320: 7265 6d6f 7665 5f75 646c 7328 7365 6c66  remove_udls(self
-00003330: 2c20 2a75 646c 732c 2072 656d 6f76 655f  , *udls, remove_
-00003340: 616c 6c3d 4661 6c73 6529 3a0a 2020 2020  all=False):.    
-00003350: 2020 2020 2222 2252 656d 6f76 6520 7564      """Remove ud
-00003360: 6c20 6672 6f6d 206d 6f64 656c 2069 6620  l from model if 
-00003370: 6173 736f 6369 6174 6564 2077 6974 6820  associated with 
-00003380: 6d6f 6465 6c2e 0a0a 2020 2020 2020 2020  model...        
-00003390: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
-000033a0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-000033b0: 2020 2020 2020 2a75 646c 7320 3a20 5564        *udls : Ud
-000033c0: 6c20 6f62 6a65 6374 730a 2020 2020 2020  l objects.      
-000033d0: 2020 2020 2020 5564 6c20 6f62 6a65 6374        Udl object
-000033e0: 2074 6f20 6265 2072 656d 6f76 6564 2066   to be removed f
-000033f0: 726f 6d20 7468 6520 736c 6f70 6520 6f62  rom the slope ob
-00003400: 6a65 6374 2e0a 2020 2020 2020 2020 7265  ject..        re
-00003410: 6d6f 7665 5f61 6c6c 203a 2062 6f6f 6c2c  move_all : bool,
-00003420: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-00003430: 2020 2020 2020 4966 2074 7275 6520 7265        If true re
-00003440: 6d6f 7665 2061 6c6c 2075 646c 732c 2062  move all udls, b
-00003450: 7920 6465 6661 756c 7420 4661 6c73 650a  y default False.
-00003460: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
-00003470: 2020 2020 2066 6f72 2075 646c 2069 6e20       for udl in 
-00003480: 7564 6c73 3a0a 2020 2020 2020 2020 2020  udls:.          
-00003490: 2020 666f 7220 6368 6563 6b5f 7564 6c20    for check_udl 
-000034a0: 696e 2073 656c 662e 5f75 646c 733a 0a20  in self._udls:. 
-000034b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000034c0: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
-000034d0: 2020 2020 2020 2020 6368 6563 6b5f 7564          check_ud
-000034e0: 6c2e 6f66 6673 6574 203d 3d20 7564 6c2e  l.offset == udl.
-000034f0: 6f66 6673 6574 0a20 2020 2020 2020 2020  offset.         
-00003500: 2020 2020 2020 2020 2020 2061 6e64 2063             and c
-00003510: 6865 636b 5f75 646c 2e6d 6167 6e69 7475  heck_udl.magnitu
-00003520: 6465 203d 3d20 7564 6c2e 6d61 676e 6974  de == udl.magnit
-00003530: 7564 650a 2020 2020 2020 2020 2020 2020  ude.            
-00003540: 2020 2020 2020 2020 616e 6420 6368 6563          and chec
-00003550: 6b5f 7564 6c2e 6c65 6e67 7468 203d 3d20  k_udl.length == 
-00003560: 7564 6c2e 6c65 6e67 7468 0a20 2020 2020  udl.length.     
-00003570: 2020 2020 2020 2020 2020 2029 3a0a 2020             ):.  
-00003580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003590: 2020 7365 6c66 2e5f 7564 6c73 2e72 656d    self._udls.rem
-000035a0: 6f76 6528 6368 6563 6b5f 7564 6c29 0a0a  ove(check_udl)..
-000035b0: 2020 2020 2020 2020 7365 6c66 2e5f 7564          self._ud
-000035c0: 6c5f 6d61 7820 3d20 6d61 7828 7365 6c66  l_max = max(self
-000035d0: 2e5f 7564 6c73 2c20 6b65 793d 6c61 6d62  ._udls, key=lamb
-000035e0: 6461 2078 3a20 782e 6d61 676e 6974 7564  da x: x.magnitud
-000035f0: 6529 0a0a 2020 2020 2020 2020 6966 2072  e)..        if r
-00003600: 656d 6f76 655f 616c 6c3a 0a20 2020 2020  emove_all:.     
-00003610: 2020 2020 2020 2073 656c 662e 5f75 646c         self._udl
-00003620: 7320 3d20 5b5d 0a20 2020 2020 2020 2020  s = [].         
-00003630: 2020 2073 656c 662e 5f75 646c 5f6d 6178     self._udl_max
-00003640: 203d 2030 0a0a 2020 2020 2020 2020 2320   = 0..        # 
-00003650: 7265 7365 7420 7265 7375 6c74 730a 2020  reset results.  
-00003660: 2020 2020 2020 7365 6c66 2e5f 7265 7365        self._rese
-00003670: 745f 7265 7375 6c74 7328 290a 0a20 2020  t_results()..   
-00003680: 2064 6566 2073 6574 5f6c 6c73 2873 656c   def set_lls(sel
-00003690: 662c 202a 6c6c 7329 3a0a 2020 2020 2020  f, *lls):.      
-000036a0: 2020 2222 2273 6574 2061 2073 7572 6661    """set a surfa
-000036b0: 6365 2073 7572 6368 6172 6765 206f 6e20  ce surcharge on 
-000036c0: 746f 7020 6f66 2074 6865 2073 6c6f 7065  top of the slope
-000036d0: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-000036e0: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
-000036f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
-00003700: 2020 2020 2020 202a 6c6c 7320 3a20 4c69         *lls : Li
-00003710: 6e65 4c6f 6164 206f 626a 6563 7473 0a20  neLoad objects. 
-00003720: 2020 2020 2020 2020 2020 204c 696e 654c             LineL
-00003730: 6f61 6420 6f62 6a65 6374 2074 6f20 6265  oad object to be
-00003740: 2061 7373 6967 6e65 6420 746f 2074 6865   assigned to the
-00003750: 2073 6c6f 7065 206f 626a 6563 742e 0a20   slope object.. 
-00003760: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
-00003770: 2020 2020 666f 7220 6c6c 2069 6e20 6c6c      for ll in ll
-00003780: 733a 0a20 2020 2020 2020 2020 2020 2069  s:.            i
-00003790: 6620 6973 696e 7374 616e 6365 286c 6c2c  f isinstance(ll,
-000037a0: 204c 696e 654c 6f61 6429 3a0a 2020 2020   LineLoad):.    
-000037b0: 2020 2020 2020 2020 2020 2020 6966 206c              if l
-000037c0: 6c2e 6d61 676e 6974 7564 6520 3e20 303a  l.magnitude > 0:
-000037d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000037e0: 2020 2020 2073 656c 662e 5f6c 6c73 2e61       self._lls.a
-000037f0: 7070 656e 6428 6c6c 290a 0a20 2020 2020  ppend(ll)..     
-00003800: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00003810: 2075 7064 6174 6520 746f 206d 616b 6520   update to make 
-00003820: 7375 7265 2066 756c 6c20 6c6f 6164 2069  sure full load i
-00003830: 7320 696e 636c 7564 6564 0a20 2020 2020  s included.     
-00003840: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00003850: 696e 5f6c 656e 6774 6820 3d20 6c6c 2e6f  in_length = ll.o
-00003860: 6666 7365 7420 2a20 330a 2020 2020 2020  ffset * 3.      
-00003870: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00003880: 2073 656c 662e 5f4d 494e 5f45 5854 5f4c   self._MIN_EXT_L
-00003890: 203c 206d 696e 5f6c 656e 6774 683a 0a20   < min_length:. 
-000038a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038b0: 2020 2020 2020 2073 656c 662e 7570 6461         self.upda
-000038c0: 7465 5f62 6f75 6e64 6172 795f 6f70 7469  te_boundary_opti
-000038d0: 6f6e 7328 4d49 4e5f 4558 545f 4c3d 6d69  ons(MIN_EXT_L=mi
-000038e0: 6e5f 6c65 6e67 7468 290a 0a20 2020 2020  n_length)..     
-000038f0: 2020 2073 656c 662e 5f75 7064 6174 655f     self._update_
-00003900: 6c6c 5f63 6f6f 7264 696e 6174 6573 2829  ll_coordinates()
-00003910: 0a0a 2020 2020 2020 2020 2320 7265 7365  ..        # rese
-00003920: 7420 7265 7375 6c74 730a 2020 2020 2020  t results.      
-00003930: 2020 7365 6c66 2e5f 7265 7365 745f 7265    self._reset_re
-00003940: 7375 6c74 7328 290a 0a20 2020 2023 2064  sults()..    # d
-00003950: 6f6e 7420 6e65 6564 2074 6f20 7265 7365  ont need to rese
-00003960: 7420 7265 7375 6c74 7320 7369 6e63 6520  t results since 
-00003970: 7468 6973 206f 6e6c 7920 7368 6f75 6c64  this only should
-00003980: 2062 6520 6361 6c6c 6564 0a20 2020 2023   be called.    #
-00003990: 2061 7320 6120 7061 7274 206f 6620 7265   as a part of re
-000039a0: 7365 7474 696e 670a 2020 2020 6465 6620  setting.    def 
-000039b0: 5f75 7064 6174 655f 6c6c 5f63 6f6f 7264  _update_ll_coord
-000039c0: 696e 6174 6573 2873 656c 6629 3a0a 2020  inates(self):.  
-000039d0: 2020 2020 2020 2255 7064 6174 6520 636f        "Update co
-000039e0: 6f72 6469 6e61 7465 7320 666f 7220 706f  ordinates for po
-000039f0: 696e 7420 6c6f 6164 2062 6173 6564 206f  int load based o
-00003a00: 6e20 6578 7465 726e 616c 2062 6f75 6e64  n external bound
-00003a10: 6172 7920 616e 6420 4c69 6e65 4c6f 6164  ary and LineLoad
-00003a20: 206f 626a 6563 7422 0a0a 2020 2020 2020   object"..      
-00003a30: 2020 666f 7220 6c6c 2069 6e20 7365 6c66    for ll in self
-00003a40: 2e5f 6c6c 733a 0a20 2020 2020 2020 2020  ._lls:.         
-00003a50: 2020 2063 6f6f 7264 203d 206d 6178 2830     coord = max(0
-00003a60: 2c20 7365 6c66 2e5f 746f 705f 636f 6f72  , self._top_coor
-00003a70: 645b 305d 202d 206c 6c2e 6f66 6673 6574  d[0] - ll.offset
-00003a80: 290a 0a20 2020 2020 2020 2020 2020 206c  )..            l
-00003a90: 6c2e 636f 6f72 6420 3d20 636f 6f72 640a  l.coord = coord.
-00003aa0: 0a20 2020 2064 6566 2072 656d 6f76 655f  .    def remove_
-00003ab0: 6c6c 7328 7365 6c66 2c20 2a6c 6c73 2c20  lls(self, *lls, 
-00003ac0: 7265 6d6f 7665 5f61 6c6c 3d46 616c 7365  remove_all=False
-00003ad0: 293a 0a20 2020 2020 2020 2022 2222 5265  ):.        """Re
-00003ae0: 6d6f 7665 2075 646c 2066 726f 6d20 6d6f  move udl from mo
-00003af0: 6465 6c20 6966 2061 7373 6f63 6961 7465  del if associate
-00003b00: 6420 7769 7468 206d 6f64 656c 2e0a 0a20  d with model... 
-00003b10: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-00003b20: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-00003b30: 2d2d 2d2d 0a20 2020 2020 2020 202a 6c6c  ----.        *ll
-00003b40: 7320 3a20 4c69 6e65 4c6f 6164 206f 626a  s : LineLoad obj
-00003b50: 6563 7473 0a20 2020 2020 2020 2020 2020  ects.           
-00003b60: 204c 696e 654c 6f61 6420 6f62 6a65 6374   LineLoad object
-00003b70: 2074 6f20 6265 2072 656d 6f76 6564 2066   to be removed f
-00003b80: 726f 6d20 7468 6520 736c 6f70 6520 6f62  rom the slope ob
-00003b90: 6a65 6374 2e0a 2020 2020 2020 2020 7265  ject..        re
-00003ba0: 6d6f 7665 5f61 6c6c 203a 2062 6f6f 6c2c  move_all : bool,
-00003bb0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-00003bc0: 2020 2020 2020 6966 2074 7275 6520 7265        if true re
-00003bd0: 6d6f 7665 2061 6c6c 206c 6c73 2c20 6279  move all lls, by
-00003be0: 2064 6566 6175 6c74 2046 616c 7365 0a20   default False. 
-00003bf0: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
-00003c00: 2020 2020 2320 6361 6e20 7072 6f62 6162      # can probab
-00003c10: 6c79 2077 7269 7465 2074 6869 7320 6173  ly write this as
-00003c20: 204f 286e 2920 7261 7468 6572 2074 6861   O(n) rather tha
-00003c30: 6e20 4f28 6e5e 3229 0a20 2020 2020 2020  n O(n^2).       
-00003c40: 2066 6f72 206c 6c20 696e 206c 6c73 3a0a   for ll in lls:.
-00003c50: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00003c60: 6368 6563 6b5f 6c6c 2069 6e20 7365 6c66  check_ll in self
-00003c70: 2e5f 6c6c 733a 0a20 2020 2020 2020 2020  ._lls:.         
-00003c80: 2020 2020 2020 2069 6620 6368 6563 6b5f         if check_
-00003c90: 6c6c 2e6f 6666 7365 7420 3d3d 206c 6c2e  ll.offset == ll.
-00003ca0: 6f66 6673 6574 2061 6e64 2063 6865 636b  offset and check
-00003cb0: 5f6c 6c2e 6d61 676e 6974 7564 6520 3d3d  _ll.magnitude ==
-00003cc0: 206c 6c2e 6d61 676e 6974 7564 653a 0a20   ll.magnitude:. 
-00003cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ce0: 2020 2073 656c 662e 5f6c 6c73 2e72 656d     self._lls.rem
-00003cf0: 6f76 6528 6368 6563 6b5f 6c6c 290a 0a20  ove(check_ll).. 
-00003d00: 2020 2020 2020 2069 6620 7265 6d6f 7665         if remove
-00003d10: 5f61 6c6c 3a0a 2020 2020 2020 2020 2020  _all:.          
-00003d20: 2020 7365 6c66 2e5f 6c6c 7320 3d20 5b5d    self._lls = []
-00003d30: 0a0a 2020 2020 2020 2020 2320 7265 7365  ..        # rese
-00003d40: 7420 7265 7375 6c74 730a 2020 2020 2020  t results.      
-00003d50: 2020 7365 6c66 2e5f 7265 7365 745f 7265    self._reset_re
-00003d60: 7375 6c74 7328 290a 0a20 2020 2064 6566  sults()..    def
-00003d70: 2073 6574 5f6d 6174 6572 6961 6c73 2873   set_materials(s
-00003d80: 656c 662c 202a 6d61 7465 7269 616c 7329  elf, *materials)
-00003d90: 3a0a 2020 2020 2020 2020 2222 2241 7373  :.        """Ass
-00003da0: 6967 6e20 6d61 7465 7269 616c 2069 6e73  ign material ins
-00003db0: 7461 6e63 6573 2074 6f20 7468 6520 736c  tances to the sl
-00003dc0: 6f70 6520 696e 7374 616e 6365 2e0a 0a20  ope instance... 
-00003dd0: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-00003de0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-00003df0: 2d2d 2d2d 0a20 2020 2020 2020 202a 6d61  ----.        *ma
-00003e00: 7465 7269 616c 7320 3a20 4d61 7465 7269  terials : Materi
-00003e10: 616c 2028 6c69 7374 292c 206f 7074 696f  al (list), optio
-00003e20: 6e61 6c0a 2020 2020 2020 2020 2020 2020  nal.            
-00003e30: 4d61 7465 7269 616c 2069 6e73 7461 6e63  Material instanc
-00003e40: 6573 2074 6f20 6265 2061 7373 6f63 6961  es to be associa
-00003e50: 7465 6420 7769 7468 2073 6c6f 7065 2e0a  ted with slope..
-00003e60: 0a0a 2020 2020 2020 2020 5261 6973 6573  ..        Raises
-00003e70: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d0a  .        ------.
-00003e80: 2020 2020 2020 2020 5661 6c75 6545 7272          ValueErr
-00003e90: 6f72 0a20 2020 2020 2020 2020 2020 2049  or.            I
-00003ea0: 6620 6d61 7465 7269 616c 206e 6f74 2069  f material not i
-00003eb0: 6e73 7461 6e63 6520 6f66 204d 6174 6572  nstance of Mater
-00003ec0: 6961 6c20 636c 6173 7320 6572 726f 7220  ial class error 
-00003ed0: 6973 2072 6169 7365 642e 0a20 2020 2020  is raised..     
-00003ee0: 2020 2056 616c 7565 4572 726f 720a 2020     ValueError.  
-00003ef0: 2020 2020 2020 2020 2020 4966 206e 6f6e            If non
-00003f00: 2d75 6e69 7175 6520 6d61 7465 7269 616c  -unique material
-00003f10: 2064 6570 7468 7320 7468 656e 2065 7272   depths then err
-00003f20: 6f72 2069 7320 7261 6973 6564 2e0a 2020  or is raised..  
-00003f30: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-00003f40: 2020 2023 2063 6865 636b 206d 6174 6572     # check mater
-00003f50: 6961 6c20 6f62 6a65 6374 2065 6e74 6572  ial object enter
-00003f60: 6564 0a20 2020 2020 2020 2066 6f72 206d  ed.        for m
-00003f70: 6174 6572 6961 6c20 696e 206d 6174 6572  aterial in mater
-00003f80: 6961 6c73 3a0a 2020 2020 2020 2020 2020  ials:.          
-00003f90: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
-00003fa0: 6e63 6528 6d61 7465 7269 616c 2c20 4d61  nce(material, Ma
-00003fb0: 7465 7269 616c 293a 0a20 2020 2020 2020  terial):.       
-00003fc0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
-00003fd0: 616c 7565 4572 726f 7228 0a20 2020 2020  alueError(.     
-00003fe0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00003ff0: 5468 6520 6675 6e63 7469 6f6e 2061 6464  The function add
-00004000: 5f6d 6174 6572 6961 6c73 206f 6e6c 7920  _materials only 
-00004010: 6163 6365 7074 7320 696e 7374 616e 6365  accepts instance
-00004020: 7320 6f66 2074 6865 204d 6174 6572 6961  s of the Materia
-00004030: 6c20 436c 6173 7322 0a20 2020 2020 2020  l Class".       
-00004040: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-00004050: 2020 2020 2320 4e65 6564 2074 6f20 7661      # Need to va
-00004060: 6c69 6461 7465 206d 6174 6572 6961 6c20  lidate material 
-00004070: 7661 6c75 6573 2061 6c73 6f0a 0a20 2020  values also..   
-00004080: 2020 2020 2023 2073 6f72 7420 6d61 7465       # sort mate
-00004090: 7269 616c 7320 746f 2062 6520 696e 206f  rials to be in o
-000040a0: 7264 6572 2c20 696e 636c 7564 6520 6578  rder, include ex
-000040b0: 6973 7469 6e67 206d 6174 6572 6961 6c73  isting materials
-000040c0: 0a20 2020 2020 2020 206d 6174 6572 6961  .        materia
-000040d0: 6c73 203d 206c 6973 7428 6d61 7465 7269  ls = list(materi
-000040e0: 616c 7329 202b 2073 656c 662e 5f6d 6174  als) + self._mat
-000040f0: 6572 6961 6c73 0a20 2020 2020 2020 206d  erials.        m
-00004100: 6174 6572 6961 6c73 2e73 6f72 7428 6b65  aterials.sort(ke
-00004110: 793d 6c61 6d62 6461 2078 3a20 782e 6465  y=lambda x: x.de
-00004120: 7074 685f 746f 5f62 6f74 746f 6d29 0a0a  pth_to_bottom)..
-00004130: 2020 2020 2020 2020 6465 7074 6873 203d          depths =
-00004140: 205b 6d61 7465 7269 616c 2e64 6570 7468   [material.depth
-00004150: 5f74 6f5f 626f 7474 6f6d 2066 6f72 206d  _to_bottom for m
-00004160: 6174 6572 6961 6c20 696e 206d 6174 6572  aterial in mater
-00004170: 6961 6c73 5d0a 0a20 2020 2020 2020 2023  ials]..        #
-00004180: 2069 6620 6765 6f6c 6f67 6963 616c 2075   if geological u
-00004190: 6e69 7420 6465 6570 6572 2074 6861 6e20  nit deeper than 
-000041a0: 6d6f 6465 6c20 7468 616e 2065 7874 656e  model than exten
-000041b0: 6420 6d6f 6465 6c20 746f 2066 6974 206d  d model to fit m
-000041c0: 6174 6572 6961 6c73 0a20 2020 2020 2020  aterials.       
-000041d0: 2069 6620 6465 7074 6873 5b2d 315d 203e   if depths[-1] >
-000041e0: 2073 656c 662e 5f65 7874 6572 6e61 6c5f   self._external_
-000041f0: 6865 6967 6874 3a0a 2020 2020 2020 2020  height:.        
-00004200: 2020 2020 7365 6c66 2e75 7064 6174 655f      self.update_
-00004210: 626f 756e 6461 7279 5f6f 7074 696f 6e73  boundary_options
-00004220: 284d 494e 5f45 5854 5f48 3d64 6570 7468  (MIN_EXT_H=depth
-00004230: 735b 2d31 5d29 0a0a 2020 2020 2020 2020  s[-1])..        
-00004240: 2320 6368 6563 6b20 6d61 7465 7269 616c  # check material
-00004250: 2064 6570 7468 2075 6e69 7175 650a 2020   depth unique.  
-00004260: 2020 2020 2020 6966 206c 656e 2864 6570        if len(dep
-00004270: 7468 7329 203e 206c 656e 2873 6574 2864  ths) > len(set(d
-00004280: 6570 7468 7329 293a 0a20 2020 2020 2020  epths)):.       
-00004290: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-000042a0: 4572 726f 7228 2254 6865 2073 616d 6520  Error("The same 
-000042b0: 6d61 7465 7269 616c 2064 6570 7468 2068  material depth h
-000042c0: 6173 2062 6565 6e20 696e 7075 7420 7477  as been input tw
-000042d0: 6963 6522 290a 0a20 2020 2020 2020 206d  ice")..        m
-000042e0: 6174 6572 6961 6c5f 7265 6669 6e65 6420  aterial_refined 
-000042f0: 3d20 5b5d 0a20 2020 2020 2020 2023 2064  = [].        # d
-00004300: 6566 696e 6520 524c 2066 6f72 2065 6163  efine RL for eac
-00004310: 6820 6d61 7465 7269 616c 2061 6e64 2063  h material and c
-00004320: 6f6c 6f72 2066 6f72 2065 6163 6820 6d61  olor for each ma
-00004330: 7465 7269 616c 0a20 2020 2020 2020 2066  terial.        f
-00004340: 6f72 2069 2c20 6d61 7465 7269 616c 2069  or i, material i
-00004350: 6e20 656e 756d 6572 6174 6528 6d61 7465  n enumerate(mate
-00004360: 7269 616c 7329 3a0a 2020 2020 2020 2020  rials):.        
-00004370: 2020 2020 6d61 7465 7269 616c 2e52 4c20      material.RL 
-00004380: 3d20 7365 6c66 2e5f 6578 7465 726e 616c  = self._external
-00004390: 5f68 6569 6768 7420 2d20 6d61 7465 7269  _height - materi
-000043a0: 616c 2e64 6570 7468 5f74 6f5f 626f 7474  al.depth_to_bott
-000043b0: 6f6d 0a0a 2020 2020 2020 2020 2020 2020  om..            
-000043c0: 6966 2028 0a20 2020 2020 2020 2020 2020  if (.           
-000043d0: 2020 2020 2075 7469 6c69 7469 6573 2e69       utilities.i
-000043e0: 735f 636f 6c6f 7228 6d61 7465 7269 616c  s_color(material
-000043f0: 2e75 7365 725f 6465 6669 6e65 645f 636f  .user_defined_co
-00004400: 6c6f 7229 0a20 2020 2020 2020 2020 2020  lor).           
-00004410: 2020 2020 2061 6e64 206d 6174 6572 6961       and materia
-00004420: 6c2e 7573 6572 5f64 6566 696e 6564 5f63  l.user_defined_c
-00004430: 6f6c 6f72 2021 3d20 2222 0a20 2020 2020  olor != "".     
-00004440: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
-00004450: 2020 2020 2020 2020 2020 6d61 7465 7269            materi
-00004460: 616c 2e63 6f6c 6f72 203d 206d 6174 6572  al.color = mater
-00004470: 6961 6c2e 7573 6572 5f64 6566 696e 6564  ial.user_defined
-00004480: 5f63 6f6c 6f72 0a20 2020 2020 2020 2020  _color.         
-00004490: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000044a0: 2020 2020 2020 2020 206d 6174 6572 6961           materia
-000044b0: 6c2e 636f 6c6f 7220 3d20 4d41 5445 5249  l.color = MATERI
-000044c0: 414c 5f43 4f4c 4f52 535b 6920 2520 3130  AL_COLORS[i % 10
-000044d0: 5d0a 0a20 2020 2020 2020 2020 2020 206d  ]..            m
-000044e0: 6174 6572 6961 6c5f 7265 6669 6e65 642e  aterial_refined.
-000044f0: 6170 7065 6e64 286d 6174 6572 6961 6c29  append(material)
-00004500: 0a0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-00004510: 6d61 7465 7269 616c 7320 3d20 6d61 7465  materials = mate
-00004520: 7269 616c 5f72 6566 696e 6564 0a0a 2020  rial_refined..  
-00004530: 2020 2020 2020 2320 7265 7365 7420 7265        # reset re
-00004540: 7375 6c74 730a 2020 2020 2020 2020 7365  sults.        se
-00004550: 6c66 2e5f 7265 7365 745f 7265 7375 6c74  lf._reset_result
-00004560: 7328 290a 0a20 2020 2064 6566 2072 656d  s()..    def rem
-00004570: 6f76 655f 6d61 7465 7269 616c 280a 2020  ove_material(.  
-00004580: 2020 2020 2020 7365 6c66 2c20 6d61 7465        self, mate
-00004590: 7269 616c 3a20 4d61 7465 7269 616c 203d  rial: Material =
-000045a0: 204e 6f6e 652c 2064 6570 7468 3a20 666c   None, depth: fl
-000045b0: 6f61 7420 3d20 4e6f 6e65 2c20 7265 6d6f  oat = None, remo
-000045c0: 7665 5f61 6c6c 3d46 616c 7365 0a20 2020  ve_all=False.   
-000045d0: 2029 3a0a 2020 2020 2020 2020 2222 2252   ):.        """R
-000045e0: 656d 6f76 6520 6d61 7465 7269 616c 2066  emove material f
-000045f0: 726f 6d20 736c 6f70 652e 0a0a 2020 2020  rom slope...    
-00004600: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-00004610: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-00004620: 2d0a 2020 2020 2020 2020 6d61 7465 7269  -.        materi
-00004630: 616c 203a 204d 6174 6572 6961 6c2c 206f  al : Material, o
-00004640: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-00004650: 2020 2020 6d61 7465 7269 616c 206f 626a      material obj
-00004660: 6563 742e 2049 6620 7370 6563 6966 6965  ect. If specifie
-00004670: 6420 616e 6420 6578 6973 7473 2069 6e20  d and exists in 
-00004680: 6d61 7465 7269 616c 730a 2020 2020 2020  materials.      
-00004690: 2020 2020 2020 6173 736f 6369 6174 6564        associated
-000046a0: 2077 6974 6820 736c 6f70 6520 7468 656e   with slope then
-000046b0: 2077 696c 6c20 6265 2072 656d 6f76 6564   will be removed
-000046c0: 2c20 6279 2064 6566 6175 6c74 204e 6f6e  , by default Non
-000046d0: 650a 2020 2020 2020 2020 6465 7074 6820  e.        depth 
-000046e0: 3a20 666c 6f61 742c 206f 7074 696f 6e61  : float, optiona
-000046f0: 6c0a 2020 2020 2020 2020 2020 2020 6465  l.            de
-00004700: 7074 6820 696e 206d 6574 7265 7320 6f66  pth in metres of
-00004710: 206d 6174 6572 6961 6c20 6f62 6a65 6374   material object
-00004720: 2e20 4966 206e 6f74 204e 6f6e 6520 616e  . If not None an
-00004730: 6420 6d61 7465 7269 616c 2066 6f75 6e64  d material found
-00004740: 0a20 2020 2020 2020 2020 2020 2061 7420  .            at 
-00004750: 696e 6469 6361 7465 6420 6465 7074 6820  indicated depth 
-00004760: 7468 656e 2077 696c 6c20 7265 6d6f 7665  then will remove
-00004770: 2074 6865 206d 6174 6572 6961 6c2c 2062   the material, b
-00004780: 7920 6465 6661 756c 7420 4e6f 6e65 0a20  y default None. 
-00004790: 2020 2020 2020 2072 656d 6f76 655f 616c         remove_al
-000047a0: 6c20 3a20 426f 6f6c 6561 6e2c 206f 7074  l : Boolean, opt
-000047b0: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
-000047c0: 2020 6966 2074 7275 6520 616c 6c20 6d61    if true all ma
-000047d0: 7465 7269 616c 7320 7265 6d6f 7665 642c  terials removed,
-000047e0: 2064 6566 6175 6c74 2066 616c 7365 0a0a   default false..
-000047f0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00004800: 2020 2020 2320 6765 6e65 7261 6c20 6e6f      # general no
-00004810: 7465 3a20 6465 7074 6820 7573 6564 2074  te: depth used t
-00004820: 6f20 7265 6d6f 7665 206f 626a 6563 7420  o remove object 
-00004830: 7261 7468 6572 2074 6861 6e20 6469 7265  rather than dire
-00004840: 6374 6c79 2072 656d 6f76 696e 670a 2020  ctly removing.  
-00004850: 2020 2020 2020 2320 6576 656e 2077 6865        # even whe
-00004860: 6e20 6d61 7465 7269 616c 2063 6c61 7373  n material class
-00004870: 2070 726f 7669 6465 6420 6265 6361 7573   provided becaus
-00004880: 6520 6120 7573 6572 206d 6967 6874 2072  e a user might r
-00004890: 6569 6e69 7469 616c 6973 650a 2020 2020  einitialise.    
-000048a0: 2020 2020 2320 616e 206f 626a 6563 7420      # an object 
-000048b0: 7769 7468 2074 6865 2073 616d 6520 6465  with the same de
-000048c0: 7461 696c 7320 6275 7420 6966 2074 6865  tails but if the
-000048d0: 2070 6f69 6e74 6572 2069 7320 6368 616e   pointer is chan
-000048e0: 6765 6420 7468 616e 0a20 2020 2020 2020  ged than.       
-000048f0: 2023 2069 7420 6d69 6768 7420 6265 2063   # it might be c
-00004900: 6f6e 6675 7369 6e67 2066 6f72 2074 6865  onfusing for the
-00004910: 2075 7365 7220 6173 2074 6f20 7768 7920   user as to why 
-00004920: 7468 6579 2063 616e 7420 7265 6d6f 7665  they cant remove
-00004930: 2e0a 2020 2020 2020 2020 2320 436f 6d6d  ..        # Comm
-00004940: 656e 7420 6279 204a 6573 7365 2042 2c20  ent by Jesse B, 
-00004950: 3134 2e30 332e 3230 3232 2e0a 0a20 2020  14.03.2022...   
-00004960: 2020 2020 2023 2069 6620 6d61 7465 7269       # if materi
-00004970: 616c 2064 6566 696e 6564 2061 6e64 206d  al defined and m
-00004980: 6174 6572 6961 6c20 7479 7065 2069 7320  aterial type is 
-00004990: 4d61 7465 7269 616c 2073 6574 2064 6570  Material set dep
-000049a0: 7468 2074 6f20 6265 2064 6570 7468 206f  th to be depth o
-000049b0: 6620 6d61 7465 7269 616c 0a20 2020 2020  f material.     
-000049c0: 2020 2069 6620 6d61 7465 7269 616c 2061     if material a
-000049d0: 6e64 2069 7369 6e73 7461 6e63 6528 6d61  nd isinstance(ma
-000049e0: 7465 7269 616c 2c20 4d61 7465 7269 616c  terial, Material
-000049f0: 293a 0a20 2020 2020 2020 2020 2020 2064  ):.            d
-00004a00: 6570 7468 203d 206d 6174 6572 6961 6c2e  epth = material.
-00004a10: 6465 7074 685f 746f 5f62 6f74 746f 6d0a  depth_to_bottom.
-00004a20: 0a20 2020 2020 2020 2023 2069 6620 6465  .        # if de
-00004a30: 7074 6820 7370 6563 6966 6965 6420 6164  pth specified ad
-00004a40: 6f70 740a 2020 2020 2020 2020 6966 2064  opt.        if d
-00004a50: 6570 7468 3a0a 2020 2020 2020 2020 2020  epth:.          
-00004a60: 2020 666f 7220 6d20 696e 2073 656c 662e    for m in self.
-00004a70: 5f6d 6174 6572 6961 6c73 3a0a 2020 2020  _materials:.    
-00004a80: 2020 2020 2020 2020 2020 2020 6966 206d              if m
-00004a90: 2e64 6570 7468 5f74 6f5f 626f 7474 6f6d  .depth_to_bottom
-00004aa0: 203d 3d20 6465 7074 683a 0a20 2020 2020   == depth:.     
-00004ab0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00004ac0: 656c 662e 5f6d 6174 6572 6961 6c73 2e72  elf._materials.r
-00004ad0: 656d 6f76 6528 6d29 0a20 2020 2020 2020  emove(m).       
-00004ae0: 2020 2020 2020 2020 2020 2020 2062 7265               bre
-00004af0: 616b 0a0a 2020 2020 2020 2020 6966 2072  ak..        if r
-00004b00: 656d 6f76 655f 616c 6c3a 0a20 2020 2020  emove_all:.     
-00004b10: 2020 2020 2020 2073 656c 662e 5f6d 6174         self._mat
-00004b20: 6572 6961 6c73 203d 205b 5d0a 0a20 2020  erials = []..   
-00004b30: 2020 2020 2023 2072 6573 6574 2072 6573       # reset res
-00004b40: 756c 7473 0a20 2020 2020 2020 2073 656c  ults.        sel
-00004b50: 662e 5f72 6573 6574 5f72 6573 756c 7473  f._reset_results
-00004b60: 2829 0a0a 2020 2020 6465 6620 7570 6461  ()..    def upda
-00004b70: 7465 5f77 6174 6572 5f61 6e61 6c79 7369  te_water_analysi
-00004b80: 735f 6f70 7469 6f6e 7328 7365 6c66 2c20  s_options(self, 
-00004b90: 6175 746f 3a20 626f 6f6c 203d 2054 7275  auto: bool = Tru
-00004ba0: 652c 2048 3a20 696e 7420 3d20 3129 3a0a  e, H: int = 1):.
-00004bb0: 2020 2020 2020 2020 2222 2255 7064 6174          """Updat
-00004bc0: 6520 616e 616c 7973 6973 206f 7074 696f  e analysis optio
-00004bd0: 6e73 2072 6567 6172 6469 6e67 2068 6f77  ns regarding how
-00004be0: 2077 6174 6572 2069 7320 7472 6561 7465   water is treate
-00004bf0: 642e 0a0a 2020 2020 2020 2020 5061 7261  d...        Para
-00004c00: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
-00004c10: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-00004c20: 2020 6175 746f 203a 2062 6f6f 6c2c 206f    auto : bool, o
-00004c30: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-00004c40: 2020 2020 4966 2074 7275 6520 6361 6c63      If true calc
-00004c50: 756c 6174 6573 2070 7265 7373 7572 6520  ulates pressure 
-00004c60: 6865 6164 2061 7574 6f6d 6174 6963 616c  head automatical
-00004c70: 6c79 2028 6661 6374 6f72 2069 7320 636f  ly (factor is co
-00004c80: 7328 6129 2a2a 3220 7768 6572 6520 6120  s(a)**2 where a 
-00004c90: 6973 0a20 2020 2020 2020 2020 2020 2074  is.            t
-00004ca0: 6865 2061 6e67 6c65 206f 6620 736c 6f70  he angle of slop
-00004cb0: 6529 2e20 4966 2046 616c 7365 2074 616b  e). If False tak
-00004cc0: 6573 206d 616e 7561 6c20 6661 6374 6f72  es manual factor
-00004cd0: 2028 4829 2e20 6279 2064 6566 6175 6c74   (H). by default
-00004ce0: 2054 7275 650a 2020 2020 2020 2020 4820   True.        H 
-00004cf0: 3a20 696e 742c 206f 7074 696f 6e61 6c0a  : int, optional.
-00004d00: 2020 2020 2020 2020 2020 2020 6661 6374              fact
-00004d10: 6f72 206f 6e20 7761 7465 7220 7072 6573  or on water pres
-00004d20: 7375 7265 2e20 4966 2031 2077 6174 6572  sure. If 1 water
-00004d30: 2068 6561 6420 6571 7561 6c73 2064 6973   head equals dis
-00004d40: 7461 6e63 6520 6265 7477 6565 6e20 7761  tance between wa
-00004d50: 7465 720a 2020 2020 2020 2020 2020 2020  ter.            
-00004d60: 7461 626c 6520 616e 6420 626f 7474 6f6d  table and bottom
-00004d70: 206f 6620 736c 6963 652e 2049 6620 3020   of slice. If 0 
-00004d80: 6e6f 2077 6174 6572 2070 7265 7373 7572  no water pressur
-00004d90: 6520 6973 2063 6f6e 7369 6465 7265 642e  e is considered.
-00004da0: 2042 7920 6465 6661 756c 7420 312e 0a20   By default 1.. 
-00004db0: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
-00004dc0: 2020 2020 6966 2061 7574 6f3a 0a20 2020      if auto:.   
-00004dd0: 2020 2020 2020 2020 2061 203d 2061 7461           a = ata
-00004de0: 6e28 7365 6c66 2e5f 6772 6164 6965 6e74  n(self._gradient
-00004df0: 290a 2020 2020 2020 2020 2020 2020 4820  ).            H 
-00004e00: 3d20 636f 7328 6129 202a 2a20 320a 0a20  = cos(a) ** 2.. 
-00004e10: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00004e20: 2020 2020 2020 2020 2064 6174 615f 7661           data_va
-00004e30: 6c69 6461 7469 6f6e 2e61 7373 6572 745f  lidation.assert_
-00004e40: 6e75 6d62 6572 2848 2c20 2248 2229 0a20  number(H, "H"). 
-00004e50: 2020 2020 2020 2020 2020 2069 6620 4820             if H 
-00004e60: 3e20 313a 0a20 2020 2020 2020 2020 2020  > 1:.           
-00004e70: 2020 2020 2048 203d 2031 0a20 2020 2020       H = 1.     
-00004e80: 2020 2020 2020 2065 6c69 6620 4820 3c20         elif H < 
-00004e90: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
-00004ea0: 2020 2048 203d 2030 0a0a 2020 2020 2020     H = 0..      
-00004eb0: 2020 7365 6c66 2e5f 7761 7465 725f 616e    self._water_an
-00004ec0: 616c 7973 6973 5f48 203d 2048 0a0a 2020  alysis_H = H..  
-00004ed0: 2020 2020 2020 2320 7265 7365 7420 7265        # reset re
-00004ee0: 7375 6c74 730a 2020 2020 2020 2020 7365  sults.        se
-00004ef0: 6c66 2e5f 7265 7365 745f 7265 7375 6c74  lf._reset_result
-00004f00: 7328 290a 0a20 2020 2064 6566 2075 7064  s()..    def upd
-00004f10: 6174 655f 616e 616c 7973 6973 5f6f 7074  ate_analysis_opt
-00004f20: 696f 6e73 280a 2020 2020 2020 2020 7365  ions(.        se
-00004f30: 6c66 2c0a 2020 2020 2020 2020 736c 6963  lf,.        slic
-00004f40: 6573 3a20 696e 7420 3d20 4e6f 6e65 2c0a  es: int = None,.
-00004f50: 2020 2020 2020 2020 6974 6572 6174 696f          iteratio
-00004f60: 6e73 3a20 696e 7420 3d20 4e6f 6e65 2c0a  ns: int = None,.
-00004f70: 2020 2020 2020 2020 6d69 6e5f 6661 696c          min_fail
-00004f80: 7572 655f 6469 7374 3a20 696e 7420 3d20  ure_dist: int = 
-00004f90: 4e6f 6e65 2c0a 2020 2020 2020 2020 746f  None,.        to
-00004fa0: 6c65 7261 6e63 653a 2066 6c6f 6174 203d  lerance: float =
-00004fb0: 204e 6f6e 652c 0a20 2020 2020 2020 206d   None,.        m
-00004fc0: 6178 5f69 7465 7261 7469 6f6e 733a 2069  ax_iterations: i
-00004fd0: 6e74 203d 204e 6f6e 652c 0a20 2020 2029  nt = None,.    )
-00004fe0: 3a0a 2020 2020 2020 2020 2222 2246 756e  :.        """Fun
-00004ff0: 6374 696f 6e20 746f 2075 7064 6174 6520  ction to update 
-00005000: 616e 616c 7973 6973 206d 6f64 656c 6c69  analysis modelli
-00005010: 6e67 206f 7074 696f 6e73 2e0a 0a20 2020  ng options...   
-00005020: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-00005030: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00005040: 2d2d 0a20 2020 2020 2020 2073 6c69 6365  --.        slice
-00005050: 7320 3a20 696e 742c 206f 7074 696f 6e61  s : int, optiona
-00005060: 6c0a 2020 2020 2020 2020 2020 2020 536c  l.            Sl
-00005070: 6963 6573 2074 6f20 7461 6b65 2069 6e20  ices to take in 
-00005080: 6361 6c63 756c 6174 696f 6e20 666f 7220  calculation for 
-00005090: 6561 6368 2070 6f74 656e 7469 616c 0a20  each potential. 
-000050a0: 2020 2020 2020 2020 2020 2063 6972 6375             circu
-000050b0: 6c61 7220 6661 696c 7572 6520 2862 6574  lar failure (bet
-000050c0: 7765 656e 2031 3020 616e 6420 3530 3029  ween 10 and 500)
-000050d0: 2e20 4966 204e 6f6e 6520 646f 6573 6e74  . If None doesnt
-000050e0: 2075 7064 6174 6520 7468 6520 7061 7261   update the para
-000050f0: 6d65 7465 722c 2062 7920 6465 6661 756c  meter, by defaul
-00005100: 7420 4e6f 6e65 2e0a 2020 2020 2020 2020  t None..        
-00005110: 6974 6572 6174 696f 6e73 203a 2069 6e74  iterations : int
-00005120: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-00005130: 2020 2020 2020 2041 7070 726f 7869 6d61         Approxima
-00005140: 7465 206e 756d 6265 7220 6f66 2070 6f74  te number of pot
-00005150: 656e 7469 616c 2073 6c6f 7065 7320 746f  ential slopes to
-00005160: 2063 6865 636b 2028 6265 7477 6565 6e20   check (between 
-00005170: 3530 3020 616e 6420 3130 3030 3030 292e  500 and 100000).
-00005180: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
-00005190: 4e6f 6e65 2064 6f65 736e 7420 7570 6461  None doesnt upda
-000051a0: 7465 2074 6865 2070 6172 616d 6574 6572  te the parameter
-000051b0: 2c20 6279 2064 6566 6175 6c74 204e 6f6e  , by default Non
-000051c0: 652e 0a20 2020 2020 2020 206d 696e 5f66  e..        min_f
-000051d0: 6169 6c75 7265 5f64 6973 7461 6e63 6520  ailure_distance 
-000051e0: 3a20 696e 742c 206f 7074 696f 6e61 6c0a  : int, optional.
-000051f0: 2020 2020 2020 2020 2020 2020 4966 2073              If s
-00005200: 7065 6369 6669 6564 206f 6e6c 7920 6661  pecified only fa
-00005210: 696c 7572 6520 736c 6f70 6573 2077 6974  ilure slopes wit
-00005220: 6820 6120 6469 7374 616e 6365 2067 7265  h a distance gre
-00005230: 6174 6572 2074 6861 6e20 7468 650a 2020  ater than the.  
-00005240: 2020 2020 2020 2020 2020 6d69 6e20 6661            min fa
-00005250: 696c 7572 6520 6469 7374 616e 6365 2077  ilure distance w
-00005260: 696c 6c20 6265 2061 7373 6573 7365 642c  ill be assessed,
-00005270: 2062 7920 6465 6661 756c 7420 4e6f 6e65   by default None
-00005280: 2e0a 2020 2020 2020 2020 746f 6c65 7261  ..        tolera
-00005290: 6e63 6520 3a20 666c 6f61 742c 206f 7074  nce : float, opt
-000052a0: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
-000052b0: 2020 436f 6e76 6572 6761 6e63 6520 746f    Convergance to
-000052c0: 6c65 7261 6e63 6520 6f6e 2062 6973 686f  lerance on bisho
-000052d0: 7073 2e20 4361 6c63 756c 6174 696f 6e20  ps. Calculation 
-000052e0: 7769 6c6c 2073 746f 7020 7768 656e 2063  will stop when c
-000052f0: 6861 6e67 6520 696e 2066 6163 746f 720a  hange in factor.
-00005300: 2020 2020 2020 2020 2020 2020 6f66 2073              of s
-00005310: 6166 6574 7920 6973 206c 6573 7320 7468  afety is less th
-00005320: 616e 2074 6865 2074 6f6c 6572 616e 6365  an the tolerance
-00005330: 2073 7065 6369 6669 6564 2e20 4279 2064   specified. By d
-00005340: 6566 6175 6c74 204e 6f6e 652e 2049 6e69  efault None. Ini
-00005350: 616c 6973 6564 2061 7320 302e 3030 352e  alised as 0.005.
-00005360: 0a20 2020 2020 2020 206d 6178 5f69 7465  .        max_ite
-00005370: 7261 7469 6f6e 7320 3a20 696e 742c 206f  rations : int, o
-00005380: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-00005390: 2020 2020 4d61 7869 6d75 6d20 6e75 6d62      Maximum numb
-000053a0: 6572 206f 6620 6974 6572 6174 696f 6e73  er of iterations
-000053b0: 2066 6f72 2063 6f6e 7665 7267 656e 6365   for convergence
-000053c0: 206f 6e20 6269 7368 6f70 2066 6163 746f   on bishop facto
-000053d0: 7220 6f66 2073 6166 6574 792e 2042 7920  r of safety. By 
-000053e0: 6465 6661 756c 740a 2020 2020 2020 2020  default.        
-000053f0: 2020 2020 4e6f 6e65 2e20 496e 6974 6961      None. Initia
-00005400: 6c69 7365 6420 6173 2031 352e 0a20 2020  lised as 15..   
-00005410: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00005420: 2069 6620 736c 6963 6573 3a0a 2020 2020   if slices:.    
-00005430: 2020 2020 2020 2020 7365 6c66 2e5f 736c          self._sl
-00005440: 6963 6573 203d 206d 6178 286d 696e 2835  ices = max(min(5
-00005450: 3030 2c20 736c 6963 6573 292c 2031 3029  00, slices), 10)
-00005460: 0a0a 2020 2020 2020 2020 6966 2069 7465  ..        if ite
-00005470: 7261 7469 6f6e 733a 0a20 2020 2020 2020  rations:.       
-00005480: 2020 2020 2073 656c 662e 5f69 7465 7261       self._itera
-00005490: 7469 6f6e 7320 3d20 6d61 7828 6d69 6e28  tions = max(min(
-000054a0: 6974 6572 6174 696f 6e73 2c20 3130 3030  iterations, 1000
-000054b0: 3030 292c 2035 3030 290a 0a20 2020 2020  00), 500)..     
-000054c0: 2020 2069 6620 6d69 6e5f 6661 696c 7572     if min_failur
-000054d0: 655f 6469 7374 2069 7320 6e6f 7420 4e6f  e_dist is not No
-000054e0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000054f0: 7365 6c66 2e5f 6d69 6e5f 6661 696c 7572  self._min_failur
-00005500: 655f 6469 7374 616e 6365 203d 206d 696e  e_distance = min
-00005510: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00005520: 2020 6d69 6e5f 6661 696c 7572 655f 6469    min_failure_di
-00005530: 7374 2c20 7365 6c66 2e5f 6578 7465 726e  st, self._extern
-00005540: 616c 5f6c 656e 6774 6820 2a20 302e 390a  al_length * 0.9.
-00005550: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-00005560: 2020 2020 2020 2069 6620 746f 6c65 7261         if tolera
-00005570: 6e63 6520 6973 206e 6f74 204e 6f6e 653a  nce is not None:
-00005580: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00005590: 662e 5f74 6f6c 6572 616e 6365 203d 2074  f._tolerance = t
-000055a0: 6f6c 6572 616e 6365 0a0a 2020 2020 2020  olerance..      
-000055b0: 2020 6966 206d 6178 5f69 7465 7261 7469    if max_iterati
-000055c0: 6f6e 7320 6973 206e 6f74 204e 6f6e 653a  ons is not None:
-000055d0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000055e0: 662e 5f6d 6178 5f69 7465 7261 7469 6f6e  f._max_iteration
-000055f0: 7320 3d20 6d61 785f 6974 6572 6174 696f  s = max_iteratio
-00005600: 6e73 0a0a 2020 2020 2020 2020 2320 7265  ns..        # re
-00005610: 7365 7420 7265 7375 6c74 730a 2020 2020  set results.    
-00005620: 2020 2020 7365 6c66 2e5f 7265 7365 745f      self._reset_
-00005630: 7265 7375 6c74 7328 290a 0a20 2020 2064  results()..    d
-00005640: 6566 2075 7064 6174 655f 626f 756e 6461  ef update_bounda
-00005650: 7279 5f6f 7074 696f 6e73 280a 2020 2020  ry_options(.    
-00005660: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-00005670: 2020 4d49 4e5f 4558 545f 4c3a 2066 6c6f    MIN_EXT_L: flo
-00005680: 6174 203d 204e 6f6e 652c 0a20 2020 2020  at = None,.     
-00005690: 2020 204d 494e 5f45 5854 5f48 3a20 666c     MIN_EXT_H: fl
-000056a0: 6f61 7420 3d20 4e6f 6e65 2c0a 2020 2020  oat = None,.    
-000056b0: 293a 0a20 2020 2020 2020 2022 2222 4675  ):.        """Fu
-000056c0: 6e63 7469 6f6e 2074 6f20 7570 6461 7465  nction to update
-000056d0: 2065 7874 6572 6e61 6c20 626f 756e 6461   external bounda
-000056e0: 7279 206f 7074 696f 6e73 2e0a 0a20 2020  ry options...   
-000056f0: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-00005700: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00005710: 2d2d 0a20 2020 2020 2020 204d 494e 5f45  --.        MIN_E
-00005720: 5854 5f4c 203a 2066 6c6f 6174 2c20 6f70  XT_L : float, op
-00005730: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
-00005740: 2020 204d 696e 696d 756d 2065 7874 6572     Minimum exter
-00005750: 6e61 6c20 626f 756e 6461 7279 206c 656e  nal boundary len
-00005760: 6774 682e 2049 6620 4e6f 6e65 2064 6f65  gth. If None doe
-00005770: 736e 7420 7570 6461 7465 0a20 2020 2020  snt update.     
-00005780: 2020 2020 2020 2074 6865 2070 6172 616d         the param
-00005790: 6574 6572 2c20 6279 2064 6566 6175 6c74  eter, by default
-000057a0: 204e 6f6e 650a 2020 2020 2020 2020 4d49   None.        MI
-000057b0: 4e5f 4558 545f 4820 3a20 666c 6f61 742c  N_EXT_H : float,
-000057c0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-000057d0: 2020 2020 2020 4d69 6e69 6d75 6d20 6578        Minimum ex
-000057e0: 7465 726e 616c 2062 6f75 6e64 6172 7920  ternal boundary 
-000057f0: 6865 6967 6874 2e20 4966 204e 6f6e 6520  height. If None 
-00005800: 646f 6573 6e74 2075 7064 6174 650a 2020  doesnt update.  
-00005810: 2020 2020 2020 2020 2020 7468 6520 7061            the pa
-00005820: 7261 6d65 7465 722c 2062 7920 6465 6661  rameter, by defa
-00005830: 756c 7420 4e6f 6e65 2e0a 2020 2020 2020  ult None..      
-00005840: 2020 2222 220a 0a20 2020 2020 2020 2069    """..        i
-00005850: 6620 4d49 4e5f 4558 545f 483a 0a20 2020  f MIN_EXT_H:.   
-00005860: 2020 2020 2020 2020 2064 6174 615f 7661           data_va
-00005870: 6c69 6461 7469 6f6e 2e61 7373 6572 745f  lidation.assert_
-00005880: 7374 7269 6374 6c79 5f70 6f73 6974 6976  strictly_positiv
-00005890: 655f 6e75 6d62 6572 280a 2020 2020 2020  e_number(.      
-000058a0: 2020 2020 2020 2020 2020 4d49 4e5f 4558            MIN_EX
-000058b0: 545f 482c 2022 4d69 6e69 6d75 6d20 6578  T_H, "Minimum ex
-000058c0: 7465 726e 616c 206d 6f64 656c 2068 6569  ternal model hei
-000058d0: 6768 7420 284d 494e 5f45 5854 5f48 2922  ght (MIN_EXT_H)"
-000058e0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-000058f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00005900: 5f4d 494e 5f45 5854 5f48 203d 204d 494e  _MIN_EXT_H = MIN
-00005910: 5f45 5854 5f48 0a20 2020 2020 2020 2069  _EXT_H.        i
-00005920: 6620 4d49 4e5f 4558 545f 4c3a 0a20 2020  f MIN_EXT_L:.   
-00005930: 2020 2020 2020 2020 2064 6174 615f 7661           data_va
-00005940: 6c69 6461 7469 6f6e 2e61 7373 6572 745f  lidation.assert_
-00005950: 7374 7269 6374 6c79 5f70 6f73 6974 6976  strictly_positiv
-00005960: 655f 6e75 6d62 6572 280a 2020 2020 2020  e_number(.      
-00005970: 2020 2020 2020 2020 2020 4d49 4e5f 4558            MIN_EX
-00005980: 545f 4c2c 2022 4d69 6e69 6d75 6d20 6578  T_L, "Minimum ex
-00005990: 7465 726e 616c 206d 6f64 656c 206c 656e  ternal model len
-000059a0: 6774 6820 284d 494e 5f45 5854 5f48 2922  gth (MIN_EXT_H)"
-000059b0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-000059c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000059d0: 5f4d 494e 5f45 5854 5f4c 203d 204d 494e  _MIN_EXT_L = MIN
-000059e0: 5f45 5854 5f4c 0a0a 2020 2020 2020 2020  _EXT_L..        
-000059f0: 2320 6966 2074 6865 2065 7874 6572 6e61  # if the externa
-00005a00: 6c20 626f 756e 6461 7279 2068 6173 2062  l boundary has b
-00005a10: 6565 6e20 7365 7420 7468 6973 2063 616c  een set this cal
-00005a20: 6c20 6973 2061 6674 6572 2069 6e69 742e  l is after init.
-00005a30: 2043 616e 2075 7064 6174 6520 7468 6520   Can update the 
-00005a40: 626f 756e 6461 7279 2e0a 2020 2020 2020  boundary..      
-00005a50: 2020 2320 6f74 6865 7277 6973 6520 7769    # otherwise wi
-00005a60: 6c6c 2067 6574 2061 6e20 6572 726f 720a  ll get an error.
-00005a70: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00005a80: 5f65 7874 6572 6e61 6c5f 626f 756e 6461  _external_bounda
-00005a90: 7279 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ry is not None:.
-00005aa0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00005ab0: 2e73 6574 5f65 7874 6572 6e61 6c5f 626f  .set_external_bo
-00005ac0: 756e 6461 7279 2868 6569 6768 743d 7365  undary(height=se
-00005ad0: 6c66 2e5f 6865 6967 6874 2c20 6c65 6e67  lf._height, leng
-00005ae0: 7468 3d73 656c 662e 5f6c 656e 6774 6829  th=self._length)
-00005af0: 0a0a 2020 2020 2020 2020 2320 7265 7365  ..        # rese
-00005b00: 7420 7265 7375 6c74 730a 2020 2020 2020  t results.      
-00005b10: 2020 7365 6c66 2e5f 7265 7365 745f 7265    self._reset_re
-00005b20: 7375 6c74 7328 290a 0a20 2020 2064 6566  sults()..    def
-00005b30: 2072 656d 6f76 655f 616e 616c 7973 6973   remove_analysis
-00005b40: 5f6c 696d 6974 7328 7365 6c66 293a 0a20  _limits(self):. 
-00005b50: 2020 2020 2020 2022 2222 5265 7365 7420         """Reset 
-00005b60: 616e 616c 7973 6973 206c 696d 6974 7320  analysis limits 
-00005b70: 746f 2064 6566 6175 6c74 2028 6e6f 206c  to default (no l
-00005b80: 696d 6974 7329 2e22 2222 0a20 2020 2020  imits).""".     
-00005b90: 2020 2073 656c 662e 7365 745f 616e 616c     self.set_anal
-00005ba0: 7973 6973 5f6c 696d 6974 7328 0a20 2020  ysis_limits(.   
-00005bb0: 2020 2020 2020 2020 206c 6566 745f 783d           left_x=
-00005bc0: 302c 0a20 2020 2020 2020 2020 2020 2072  0,.            r
-00005bd0: 6967 6874 5f78 5f6c 6566 743d 7365 6c66  ight_x_left=self
-00005be0: 2e5f 746f 705f 636f 6f72 645b 305d 2c0a  ._top_coord[0],.
-00005bf0: 2020 2020 2020 2020 2020 2020 6c65 6674              left
-00005c00: 5f78 5f72 6967 6874 3d73 656c 662e 5f74  _x_right=self._t
-00005c10: 6f70 5f63 6f6f 7264 5b30 5d2c 0a20 2020  op_coord[0],.   
-00005c20: 2020 2020 2020 2020 2072 6967 6874 5f78           right_x
-00005c30: 3d73 656c 662e 5f65 7874 6572 6e61 6c5f  =self._external_
-00005c40: 6c65 6e67 7468 2c0a 2020 2020 2020 2020  length,.        
-00005c50: 290a 0a20 2020 2020 2020 2023 2072 6573  )..        # res
-00005c60: 6574 2072 6573 756c 7473 0a20 2020 2020  et results.     
-00005c70: 2020 2073 656c 662e 5f72 6573 6574 5f72     self._reset_r
-00005c80: 6573 756c 7473 2829 0a0a 2020 2020 6465  esults()..    de
-00005c90: 6620 7365 745f 616e 616c 7973 6973 5f6c  f set_analysis_l
-00005ca0: 696d 6974 7328 0a20 2020 2020 2020 2073  imits(.        s
-00005cb0: 656c 662c 0a20 2020 2020 2020 206c 6566  elf,.        lef
-00005cc0: 745f 783a 2066 6c6f 6174 203d 204e 6f6e  t_x: float = Non
-00005cd0: 652c 0a20 2020 2020 2020 2072 6967 6874  e,.        right
-00005ce0: 5f78 3a20 666c 6f61 7420 3d20 4e6f 6e65  _x: float = None
-00005cf0: 2c0a 2020 2020 2020 2020 6c65 6674 5f78  ,.        left_x
-00005d00: 5f72 6967 6874 3a20 666c 6f61 7420 3d20  _right: float = 
-00005d10: 4e6f 6e65 2c0a 2020 2020 2020 2020 7269  None,.        ri
-00005d20: 6768 745f 785f 6c65 6674 3a20 666c 6f61  ght_x_left: floa
-00005d30: 7420 3d20 4e6f 6e65 2c0a 2020 2020 293a  t = None,.    ):
-00005d40: 0a20 2020 2020 2020 2022 2222 7365 7420  .        """set 
-00005d50: 6c69 6d69 7473 206f 6e20 736c 6f70 6520  limits on slope 
-00005d60: 616e 616c 7973 6973 2073 6561 7263 682e  analysis search.
-00005d70: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-00005d80: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
-00005d90: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00005da0: 6c65 6674 5f78 203a 2066 6c6f 6174 0a20  left_x : float. 
-00005db0: 2020 2020 2020 2020 2020 206c 6566 7420             left 
-00005dc0: 7820 636f 6f72 6469 6e61 7465 206f 6620  x coordinate of 
-00005dd0: 7365 6172 6368 2c20 6465 6669 6e65 7320  search, defines 
-00005de0: 6f75 7465 7220 6564 6765 0a20 2020 2020  outer edge.     
-00005df0: 2020 2020 2020 206f 6620 746f 7020 6f66         of top of
-00005e00: 2073 6561 7263 680a 2020 2020 2020 2020   search.        
-00005e10: 7269 6768 745f 7820 3a20 666c 6f61 740a  right_x : float.
-00005e20: 2020 2020 2020 2020 2020 2020 7269 6768              righ
-00005e30: 7420 7820 636f 6f72 6469 6e61 7465 2073  t x coordinate s
-00005e40: 6561 7263 682c 2064 6566 696e 6573 206f  earch, defines o
-00005e50: 7574 6572 2065 6467 6520 6f66 0a20 2020  uter edge of.   
-00005e60: 2020 2020 2020 2020 2062 6f74 746f 6d20           bottom 
-00005e70: 6f66 2073 6561 7263 680a 2020 2020 2020  of search.      
-00005e80: 2020 6c65 6674 5f78 5f72 6967 6874 203a    left_x_right :
-00005e90: 2066 6c6f 6174 2c20 6f70 7469 6f6e 616c   float, optional
-00005ea0: 0a20 2020 2020 2020 2020 2020 206c 6566  .            lef
-00005eb0: 7420 7820 636f 6f72 6469 6e61 7465 2072  t x coordinate r
-00005ec0: 6967 6874 2068 616e 6420 6c69 6d69 7420  ight hand limit 
-00005ed0: 6f66 2073 6561 7263 682c 2064 6566 696e  of search, defin
-00005ee0: 6573 0a20 2020 2020 2020 2020 2020 2069  es.            i
-00005ef0: 6e6e 6572 2065 6467 6520 6f66 2074 6f70  nner edge of top
-00005f00: 206f 6620 7365 6172 6368 2e20 4966 206e   of search. If n
-00005f10: 6f6e 6520 6967 6e6f 7265 642c 2062 7920  one ignored, by 
-00005f20: 6465 6661 756c 7420 4e6f 6e65 0a20 2020  default None.   
-00005f30: 2020 2020 2072 6967 6874 5f78 5f6c 6566       right_x_lef
-00005f40: 7420 3a20 666c 6f61 742c 206f 7074 696f  t : float, optio
-00005f50: 6e61 6c0a 2020 2020 2020 2020 2020 2020  nal.            
-00005f60: 7269 6768 7420 7820 636f 6f72 6469 6e61  right x coordina
-00005f70: 7465 206c 6566 7420 6861 6e64 206c 696d  te left hand lim
-00005f80: 6974 206f 6620 7365 6172 6368 2c20 6465  it of search, de
-00005f90: 6669 6e65 730a 2020 2020 2020 2020 2020  fines.          
-00005fa0: 2020 696e 6e65 7220 6564 6765 206f 6620    inner edge of 
-00005fb0: 626f 7474 6f6d 206f 6620 7365 6172 6368  bottom of search
-00005fc0: 2e20 4966 206e 6f6e 6520 6967 6e6f 7265  . If none ignore
-00005fd0: 642c 2062 7920 6465 6661 756c 7420 4e6f  d, by default No
-00005fe0: 6e65 0a20 2020 2020 2020 2022 2222 0a20  ne.        """. 
-00005ff0: 2020 2020 2020 2023 2073 6574 2074 6f20         # set to 
-00006000: 6375 7272 656e 7420 6d6f 6465 6c20 7661  current model va
-00006010: 6c75 6573 2069 6620 6e6f 7420 7365 742c  lues if not set,
-00006020: 2065 6c73 6520 6368 6563 6b20 696e 7075   else check inpu
-00006030: 7420 6973 2076 616c 6964 0a20 2020 2020  t is valid.     
-00006040: 2020 2069 6620 6c65 6674 5f78 2069 7320     if left_x is 
-00006050: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00006060: 2020 6c65 6674 5f78 203d 2073 656c 662e    left_x = self.
-00006070: 5f6c 696d 6974 735b 305d 0a20 2020 2020  _limits[0].     
-00006080: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00006090: 2020 2020 2064 6174 615f 7661 6c69 6461       data_valida
-000060a0: 7469 6f6e 2e61 7373 6572 745f 706f 7369  tion.assert_posi
-000060b0: 7469 7665 5f6e 756d 6265 7228 6c65 6674  tive_number(left
-000060c0: 5f78 2c20 226c 6566 745f 7820 6c69 6d69  _x, "left_x limi
-000060d0: 7422 290a 0a20 2020 2020 2020 2069 6620  t")..        if 
-000060e0: 6c65 6674 5f78 5f72 6967 6874 2069 7320  left_x_right is 
-000060f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00006100: 2020 6c65 6674 5f78 5f72 6967 6874 203d    left_x_right =
-00006110: 2073 656c 662e 5f6c 696d 6974 735b 315d   self._limits[1]
-00006120: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00006130: 2020 2020 2020 2020 2020 2064 6174 615f             data_
-00006140: 7661 6c69 6461 7469 6f6e 2e61 7373 6572  validation.asser
-00006150: 745f 7374 7269 6374 6c79 5f70 6f73 6974  t_strictly_posit
-00006160: 6976 655f 6e75 6d62 6572 280a 2020 2020  ive_number(.    
-00006170: 2020 2020 2020 2020 2020 2020 6c65 6674              left
-00006180: 5f78 5f72 6967 6874 2c20 226c 6566 745f  _x_right, "left_
-00006190: 7820 7269 6768 7420 636f 6f72 6469 6e61  x right coordina
-000061a0: 7465 220a 2020 2020 2020 2020 2020 2020  te".            
-000061b0: 290a 0a20 2020 2020 2020 2069 6620 7269  )..        if ri
-000061c0: 6768 745f 785f 6c65 6674 2069 7320 4e6f  ght_x_left is No
-000061d0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000061e0: 7269 6768 745f 785f 6c65 6674 203d 2073  right_x_left = s
-000061f0: 656c 662e 5f6c 696d 6974 735b 325d 0a20  elf._limits[2]. 
-00006200: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00006210: 2020 2020 2020 2020 2064 6174 615f 7661           data_va
-00006220: 6c69 6461 7469 6f6e 2e61 7373 6572 745f  lidation.assert_
-00006230: 7374 7269 6374 6c79 5f70 6f73 6974 6976  strictly_positiv
-00006240: 655f 6e75 6d62 6572 2872 6967 6874 5f78  e_number(right_x
-00006250: 2c20 2272 6967 6874 5f78 5f6c 696d 6974  , "right_x_limit
-00006260: 2229 0a0a 2020 2020 2020 2020 6966 2072  ")..        if r
-00006270: 6967 6874 5f78 2069 7320 4e6f 6e65 3a0a  ight_x is None:.
-00006280: 2020 2020 2020 2020 2020 2020 7269 6768              righ
-00006290: 745f 7820 3d20 7365 6c66 2e5f 6c69 6d69  t_x = self._limi
-000062a0: 7473 5b33 5d0a 2020 2020 2020 2020 656c  ts[3].        el
-000062b0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-000062c0: 6461 7461 5f76 616c 6964 6174 696f 6e2e  data_validation.
-000062d0: 6173 7365 7274 5f73 7472 6963 746c 795f  assert_strictly_
-000062e0: 706f 7369 7469 7665 5f6e 756d 6265 7228  positive_number(
-000062f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006300: 2072 6967 6874 5f78 5f6c 6566 742c 2022   right_x_left, "
-00006310: 7269 6768 745f 7820 6c65 6674 2063 6f6f  right_x left coo
-00006320: 7264 696e 6174 6522 0a20 2020 2020 2020  rdinate".       
-00006330: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-00006340: 2320 6966 206f 6e6c 7920 6f6e 6520 6f66  # if only one of
-00006350: 2074 6865 2064 6f75 626c 6520 7061 7261   the double para
-00006360: 6d65 7465 7273 2069 7320 6465 6669 6e65  meters is define
-00006370: 640a 2020 2020 2020 2020 2320 7468 6520  d.        # the 
-00006380: 6f74 6865 7220 7368 6f75 6c64 2062 6520  other should be 
-00006390: 7365 7420 7570 2074 6f20 6571 7561 6c20  set up to equal 
-000063a0: 6974 0a20 2020 2020 2020 2023 206f 7220  it.        # or 
-000063b0: 7468 6520 6469 6167 7261 6d20 6973 2063  the diagram is c
-000063c0: 6f6e 6675 7369 6e67 0a20 2020 2020 2020  onfusing.       
-000063d0: 2069 6620 6c65 6674 5f78 5f72 6967 6874   if left_x_right
-000063e0: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
-000063f0: 2072 6967 6874 5f78 5f6c 6566 7420 6973   right_x_left is
-00006400: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00006410: 2020 2072 6967 6874 5f78 5f6c 6566 7420     right_x_left 
-00006420: 3d20 6c65 6674 5f78 5f72 6967 6874 0a0a  = left_x_right..
-00006430: 2020 2020 2020 2020 6966 2072 6967 6874          if right
-00006440: 5f78 5f6c 6566 7420 6973 206e 6f74 204e  _x_left is not N
-00006450: 6f6e 6520 616e 6420 6c65 6674 5f78 5f72  one and left_x_r
-00006460: 6967 6874 2069 7320 4e6f 6e65 3a0a 2020  ight is None:.  
-00006470: 2020 2020 2020 2020 2020 6c65 6674 5f78            left_x
-00006480: 5f72 6967 6874 203d 2072 6967 6874 5f78  _right = right_x
-00006490: 5f6c 6566 740a 0a20 2020 2020 2020 2023  _left..        #
-000064a0: 2065 6e66 6f72 6365 2068 6172 6420 626f   enforce hard bo
-000064b0: 756e 6461 7269 6573 2066 6f72 206c 696d  undaries for lim
-000064c0: 6974 730a 2020 2020 2020 2020 6c65 6674  its.        left
-000064d0: 5f78 203d 206d 6178 286c 6566 745f 782c  _x = max(left_x,
-000064e0: 2030 290a 2020 2020 2020 2020 6c65 6674   0).        left
-000064f0: 5f78 5f72 6967 6874 203d 206d 696e 286c  _x_right = min(l
-00006500: 6566 745f 785f 7269 6768 742c 2073 656c  eft_x_right, sel
-00006510: 662e 5f74 6f70 5f63 6f6f 7264 5b30 5d29  f._top_coord[0])
-00006520: 0a20 2020 2020 2020 2072 6967 6874 5f78  .        right_x
-00006530: 203d 206d 696e 2872 6967 6874 5f78 2c20   = min(right_x, 
-00006540: 7365 6c66 2e5f 6578 7465 726e 616c 5f6c  self._external_l
-00006550: 656e 6774 6829 0a20 2020 2020 2020 2072  ength).        r
-00006560: 6967 6874 5f78 5f6c 6566 7420 3d20 6d61  ight_x_left = ma
-00006570: 7828 7269 6768 745f 785f 6c65 6674 2c20  x(right_x_left, 
-00006580: 7365 6c66 2e5f 746f 705f 636f 6f72 645b  self._top_coord[
-00006590: 305d 290a 0a20 2020 2020 2020 2023 2063  0])..        # c
-000065a0: 6865 636b 206f 7264 6572 2069 7320 6f6b  heck order is ok
-000065b0: 6179 0a20 2020 2020 2020 2069 6620 6c65  ay.        if le
-000065c0: 6674 5f78 203e 3d20 6c65 6674 5f78 5f72  ft_x >= left_x_r
-000065d0: 6967 6874 206f 7220 7269 6768 745f 785f  ight or right_x_
-000065e0: 6c65 6674 203e 3d20 7269 6768 745f 783a  left >= right_x:
-000065f0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00006600: 7365 2056 616c 7565 4572 726f 7228 0a20  se ValueError(. 
-00006610: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00006620: 6c69 6d69 7473 206f 7574 206f 6620 6f72  limits out of or
-00006630: 6465 7220 6f72 2063 6f6e 666c 6963 7469  der or conflicti
-00006640: 6e67 2c20 6368 6563 6b20 696e 7075 7420  ng, check input 
-00006650: 666f 7220 616e 616c 7973 6973 206c 696d  for analysis lim
-00006660: 6974 7322 0a20 2020 2020 2020 2020 2020  its".           
-00006670: 2029 0a0a 2020 2020 2020 2020 7365 6c66   )..        self
-00006680: 2e5f 6c69 6d69 7473 203d 205b 6c65 6674  ._limits = [left
-00006690: 5f78 2c20 6c65 6674 5f78 5f72 6967 6874  _x, left_x_right
-000066a0: 2c20 7269 6768 745f 785f 6c65 6674 2c20  , right_x_left, 
-000066b0: 7269 6768 745f 785d 0a0a 2020 2020 2020  right_x]..      
-000066c0: 2020 2320 7265 7365 7420 7265 7375 6c74    # reset result
-000066d0: 730a 2020 2020 2020 2020 7365 6c66 2e5f  s.        self._
-000066e0: 7265 7365 745f 7265 7375 6c74 7328 290a  reset_results().
-000066f0: 0a20 2020 2064 6566 205f 7365 745f 656e  .    def _set_en
-00006700: 7472 795f 6578 6974 5f70 6c61 6e65 7328  try_exit_planes(
-00006710: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00006720: 2222 4675 6e63 7469 6f6e 2074 6f20 6765  ""Function to ge
-00006730: 6e65 7261 7465 2073 6561 7263 6820 706c  nerate search pl
-00006740: 616e 6573 2062 6173 6564 206f 6e20 6120  anes based on a 
-00006750: 6d65 7468 6f64 0a20 2020 2020 2020 206f  method.        o
-00006760: 6620 7072 6564 6574 6572 6d69 6e69 6e67  f predetermining
-00006770: 2077 6865 7265 2074 6865 2066 6169 6c75   where the failu
-00006780: 7265 2070 6c61 6e65 2077 696c 6c20 656e  re plane will en
-00006790: 7465 7220 616e 640a 2020 2020 2020 2020  ter and.        
-000067a0: 6578 6974 2074 6865 206d 6f64 656c 2e22  exit the model."
-000067b0: 2222 0a0a 2020 2020 2020 2020 2320 6e75  ""..        # nu
-000067c0: 6d62 6572 206f 6620 6469 6666 6572 656e  mber of differen
-000067d0: 7420 7261 6469 6920 746f 2063 6f6e 7369  t radii to consi
-000067e0: 6465 7220 666f 7220 7468 6520 7361 6d65  der for the same
-000067f0: 2065 6e64 2070 6f69 6e74 730a 2020 2020   end points.    
-00006800: 2020 2020 6e75 6d5f 6369 7263 6c65 7320      num_circles 
-00006810: 3d20 6d61 7828 352c 2069 6e74 2873 656c  = max(5, int(sel
-00006820: 662e 5f69 7465 7261 7469 6f6e 7320 2f20  f._iterations / 
-00006830: 3830 3029 290a 0a20 2020 2020 2020 2023  800))..        #
-00006840: 2067 656e 6572 6174 6520 636f 6f72 6469   generate coordi
-00006850: 6e61 7465 7320 666f 7220 6c65 6674 206f  nates for left o
-00006860: 6620 736c 6f70 650a 2020 2020 2020 2020  f slope.        
-00006870: 706f 696e 745f 636f 6d62 696e 6174 696f  point_combinatio
-00006880: 6e73 203d 2073 656c 662e 5f69 7465 7261  ns = self._itera
-00006890: 7469 6f6e 7320 2f20 6e75 6d5f 6369 7263  tions / num_circ
-000068a0: 6c65 730a 0a20 2020 2020 2020 2023 2073  les..        # s
-000068b0: 696d 706c 6966 6963 6174 696f 6e20 6765  implification ge
-000068c0: 6e65 7261 6c6c 7920 7769 6c6c 206d 6561  nerally will mea
-000068d0: 6e20 736c 6967 6874 6c79 206c 6573 7320  n slightly less 
-000068e0: 6974 6572 6174 696f 6e73 206f 6363 7572  iterations occur
-000068f0: 2e0a 2020 2020 2020 2020 2320 666f 7220  ..        # for 
-00006900: 7468 6520 6465 6661 756c 7420 7661 6c75  the default valu
-00006910: 6520 6f66 2032 3030 3020 7468 6973 2077  e of 2000 this w
-00006920: 696c 6c20 6265 2065 7861 6374 0a20 2020  ill be exact.   
-00006930: 2020 2020 2023 2028 3520 6369 7263 6c65       # (5 circle
-00006940: 7320 2a20 3230 2074 6f70 202a 2032 3020  s * 20 top * 20 
-00006950: 626f 7474 6f6d 203d 2032 3030 3020 6578  bottom = 2000 ex
-00006960: 6163 7420 636f 6d62 696e 6174 696f 6e73  act combinations
-00006970: 290a 2020 2020 2020 2020 6e75 6d5f 706f  ).        num_po
-00006980: 696e 7473 5f74 6f70 203d 2069 6e74 2873  ints_top = int(s
-00006990: 7172 7428 706f 696e 745f 636f 6d62 696e  qrt(point_combin
-000069a0: 6174 696f 6e73 2929 0a20 2020 2020 2020  ations)).       
-000069b0: 206e 756d 5f70 6f69 6e74 735f 626f 7420   num_points_bot 
-000069c0: 3d20 6e75 6d5f 706f 696e 7473 5f74 6f70  = num_points_top
-000069d0: 0a0a 2020 2020 2020 2020 7768 696c 6520  ..        while 
-000069e0: 6e75 6d5f 706f 696e 7473 5f74 6f70 202a  num_points_top *
-000069f0: 206e 756d 5f70 6f69 6e74 735f 626f 7420   num_points_bot 
-00006a00: 2a20 6e75 6d5f 6369 7263 6c65 7320 3c20  * num_circles < 
-00006a10: 7365 6c66 2e5f 6974 6572 6174 696f 6e73  self._iterations
-00006a20: 3a0a 2020 2020 2020 2020 2020 2020 6e75  :.            nu
-00006a30: 6d5f 706f 696e 7473 5f62 6f74 202b 3d20  m_points_bot += 
-00006a40: 310a 0a20 2020 2020 2020 2023 2072 656d  1..        # rem
-00006a50: 6f76 6520 6e75 6d62 6572 206f 6620 706f  ove number of po
-00006a60: 696e 7473 206f 6e20 746f 7020 746f 2062  ints on top to b
-00006a70: 6520 7370 7265 6164 2074 6f20 616c 6c6f  e spread to allo
-00006a80: 7720 666f 7220 7370 6563 6966 6963 0a20  w for specific. 
-00006a90: 2020 2020 2020 2023 2070 6f69 6e74 7320         # points 
-00006aa0: 6e65 7874 2074 6f20 7468 6520 6564 6765  next to the edge
-00006ab0: 206f 6620 6c6f 6164 730a 2020 2020 2020   of loads.      
-00006ac0: 2020 6e75 6d5f 706f 696e 7473 5f74 6f70    num_points_top
-00006ad0: 203d 206e 756d 5f70 6f69 6e74 735f 746f   = num_points_to
-00006ae0: 7020 2d20 6c65 6e28 7365 6c66 2e5f 6c6c  p - len(self._ll
-00006af0: 7329 202d 206c 656e 2873 656c 662e 5f75  s) - len(self._u
-00006b00: 646c 7329 0a0a 2020 2020 2020 2020 2320  dls)..        # 
-00006b10: 6765 7420 6c69 6d69 7473 206f 6e20 626f  get limits on bo
-00006b20: 756e 6473 206f 6620 736c 6f70 650a 2020  unds of slope.  
-00006b30: 2020 2020 2020 2320 6e6f 7420 736f 6d65        # not some
-00006b40: 206c 696d 6974 7320 6d69 6768 7420 7374   limits might st
-00006b50: 696c 6c20 7374 7265 7463 6820 6f66 6620  ill stretch off 
-00006b60: 736c 6f70 650a 2020 2020 2020 2020 2320  slope.        # 
-00006b70: 6275 7420 3c3d 2063 6865 636b 206c 6174  but <= check lat
-00006b80: 6572 2063 6f6e 7369 6465 7273 2074 6869  er considers thi
-00006b90: 732e 0a20 2020 2020 2020 2078 312c 2078  s..        x1, x
-00006ba0: 322c 2078 332c 2078 3420 3d20 7365 6c66  2, x3, x4 = self
-00006bb0: 2e5f 6c69 6d69 7473 0a0a 2020 2020 2020  ._limits..      
-00006bc0: 2020 2320 636f 6f72 6469 6e61 7465 7320    # coordinates 
-00006bd0: 666f 7220 6661 696c 7572 6520 706c 616e  for failure plan
-00006be0: 6573 2061 7420 746f 7020 6f66 2073 6c6f  es at top of slo
-00006bf0: 7065 0a20 2020 2020 2020 2023 2079 2063  pe.        # y c
-00006c00: 6f6f 7264 696e 6174 6520 6973 2061 6c77  oordinate is alw
-00006c10: 6179 7320 7468 6520 636f 6f72 6469 6e61  ays the coordina
-00006c20: 7465 206f 6620 7468 6520 746f 7020 6f66  te of the top of
-00006c30: 2074 6865 2073 6c6f 7065 0a20 2020 2020   the slope.     
-00006c40: 2020 206c 6566 745f 636f 6f72 6473 203d     left_coords =
-00006c50: 205b 0a20 2020 2020 2020 2020 2020 2028   [.            (
-00006c60: 7831 202b 2028 6e20 2f20 286e 756d 5f70  x1 + (n / (num_p
-00006c70: 6f69 6e74 735f 746f 7020 2d20 3129 2920  oints_top - 1)) 
-00006c80: 2a20 2878 3220 2d20 7831 292c 2073 656c  * (x2 - x1), sel
-00006c90: 662e 5f74 6f70 5f63 6f6f 7264 5b31 5d29  f._top_coord[1])
-00006ca0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00006cb0: 206e 2069 6e20 7261 6e67 6528 6e75 6d5f   n in range(num_
-00006cc0: 706f 696e 7473 5f74 6f70 290a 2020 2020  points_top).    
-00006cd0: 2020 2020 5d0a 0a20 2020 2020 2020 2023      ]..        #
-00006ce0: 2063 6f6f 6469 6e61 7465 7320 666f 7220   coodinates for 
-00006cf0: 7468 6520 626f 7474 6f6d 206f 6620 7468  the bottom of th
-00006d00: 6520 6661 696c 7572 6520 706c 616e 650a  e failure plane.
-00006d10: 2020 2020 2020 2020 2320 6361 6e20 6265          # can be
-00006d20: 2061 7420 626f 7474 6f6d 206f 7220 6f6e   at bottom or on
-00006d30: 2073 6c6f 7065 2c20 736f 2079 2069 7320   slope, so y is 
-00006d40: 6675 6e63 7469 6f6e 206f 6620 7820 616e  function of x an
-00006d50: 640a 2020 2020 2020 2020 2320 6e65 6564  d.        # need
-00006d60: 7320 746f 2062 6520 6465 7465 726d 696e  s to be determin
-00006d70: 6564 2066 6f72 2064 6966 6665 7265 6e74  ed for different
-00006d80: 2070 6f69 6e74 730a 2020 2020 2020 2020   points.        
-00006d90: 7269 6768 745f 636f 6f72 6473 5f78 203d  right_coords_x =
-00006da0: 205b 0a20 2020 2020 2020 2020 2020 2078   [.            x
-00006db0: 3320 2b20 286e 202f 2028 6e75 6d5f 706f  3 + (n / (num_po
-00006dc0: 696e 7473 5f62 6f74 2929 202a 2028 7834  ints_bot)) * (x4
-00006dd0: 202d 2078 3329 0a20 2020 2020 2020 2020   - x3).         
-00006de0: 2020 2066 6f72 206e 2069 6e20 7261 6e67     for n in rang
-00006df0: 6528 312c 206e 756d 5f70 6f69 6e74 735f  e(1, num_points_
-00006e00: 626f 7420 2b20 3129 0a20 2020 2020 2020  bot + 1).       
-00006e10: 205d 0a0a 2020 2020 2020 2020 7269 6768   ]..        righ
-00006e20: 745f 636f 6f72 6473 203d 205b 0a20 2020  t_coords = [.   
-00006e30: 2020 2020 2020 2020 2028 782c 2073 656c           (x, sel
-00006e40: 662e 6765 745f 6578 7465 726e 616c 5f79  f.get_external_y
-00006e50: 5f69 6e74 6572 7365 6374 696f 6e28 7829  _intersection(x)
-00006e60: 2920 666f 7220 7820 696e 2072 6967 6874  ) for x in right
-00006e70: 5f63 6f6f 7264 735f 780a 2020 2020 2020  _coords_x.      
-00006e80: 2020 5d0a 0a20 2020 2020 2020 2073 6561    ]..        sea
-00006e90: 7263 6820 3d20 5b5d 0a0a 2020 2020 2020  rch = []..      
-00006ea0: 2020 2320 6164 6420 696e 2063 6f6f 7264    # add in coord
-00006eb0: 696e 6174 6573 2064 6972 6563 746c 7920  inates directly 
-00006ec0: 6164 6a61 6365 6e74 2074 6f20 6c6f 6164  adjacent to load
-00006ed0: 730a 2020 2020 2020 2020 666f 7220 6c6c  s.        for ll
-00006ee0: 2069 6e20 7365 6c66 2e5f 6c6c 733a 0a20   in self._lls:. 
-00006ef0: 2020 2020 2020 2020 2020 206c 6566 745f             left_
-00006f00: 636f 6f72 6473 202b 3d20 5b28 6c6c 2e63  coords += [(ll.c
-00006f10: 6f6f 7264 202d 2030 2e30 3031 2c20 7365  oord - 0.001, se
-00006f20: 6c66 2e5f 746f 705f 636f 6f72 645b 315d  lf._top_coord[1]
-00006f30: 295d 0a0a 2020 2020 2020 2020 666f 7220  )]..        for 
-00006f40: 7564 6c20 696e 2073 656c 662e 5f75 646c  udl in self._udl
-00006f50: 733a 0a20 2020 2020 2020 2020 2020 206c  s:.            l
-00006f60: 6566 745f 636f 6f72 6473 202b 3d20 5b28  eft_coords += [(
-00006f70: 7564 6c2e 6c65 6674 202d 2030 2e30 3031  udl.left - 0.001
-00006f80: 2c20 7365 6c66 2e5f 746f 705f 636f 6f72  , self._top_coor
-00006f90: 645b 315d 295d 0a0a 2020 2020 2020 2020  d[1])]..        
-00006fa0: 2320 6c6f 6f70 2074 6872 6f75 6768 206c  # loop through l
-00006fb0: 6566 7420 616e 6420 7269 6768 7420 706f  eft and right po
-00006fc0: 696e 7473 2074 6f20 6765 6e65 7261 7465  ints to generate
-00006fd0: 2063 6f6f 7264 696e 6174 6573 0a20 2020   coordinates.   
-00006fe0: 2020 2020 2066 6f72 206c 5f63 2069 6e20       for l_c in 
-00006ff0: 7471 646d 286c 6566 745f 636f 6f72 6473  tqdm(left_coords
-00007000: 293a 0a20 2020 2020 2020 2020 2020 2066  ):.            f
-00007010: 6f72 2072 5f63 2069 6e20 7269 6768 745f  or r_c in right_
-00007020: 636f 6f72 6473 3a0a 2020 2020 2020 2020  coords:.        
-00007030: 2020 2020 2020 2020 6966 2075 7469 6c69          if utili
-00007040: 7469 6573 2e64 6973 745f 706f 696e 7473  ties.dist_points
-00007050: 286c 5f63 2c20 725f 6329 203e 2073 656c  (l_c, r_c) > sel
-00007060: 662e 5f6d 696e 5f66 6169 6c75 7265 5f64  f._min_failure_d
-00007070: 6973 7461 6e63 653a 0a20 2020 2020 2020  istance:.       
-00007080: 2020 2020 2020 2020 2020 2020 2073 6561               sea
-00007090: 7263 6820 2b3d 2073 656c 662e 5f67 656e  rch += self._gen
-000070a0: 6572 6174 655f 706c 616e 6573 286c 5f63  erate_planes(l_c
-000070b0: 2c20 725f 632c 206e 756d 5f63 6972 636c  , r_c, num_circl
-000070c0: 6573 290a 0a20 2020 2020 2020 2073 656c  es)..        sel
-000070d0: 662e 5f73 6561 7263 6820 3d20 7365 6172  f._search = sear
-000070e0: 6368 0a0a 2020 2020 6465 6620 5f67 656e  ch..    def _gen
-000070f0: 6572 6174 655f 706c 616e 6573 2873 656c  erate_planes(sel
-00007100: 662c 206c 5f63 2c20 725f 632c 206e 756d  f, l_c, r_c, num
-00007110: 5f63 6972 636c 6573 3d35 293a 0a20 2020  _circles=5):.   
-00007120: 2020 2020 2022 2222 4765 6e65 7261 7465       """Generate
-00007130: 2066 6169 6c75 7265 2070 6c61 6e65 2063   failure plane c
-00007140: 6972 636c 6520 636f 6f72 6469 6e61 7465  ircle coordinate
-00007150: 7320 7769 7468 2065 6e74 7279 2061 6e64  s with entry and
-00007160: 2065 7869 7420 706f 696e 742e 0a0a 2020   exit point...  
-00007170: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-00007180: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00007190: 2d2d 2d0a 2020 2020 2020 2020 6c5f 6320  ---.        l_c 
-000071a0: 3a20 666c 6f61 740a 2020 2020 2020 2020  : float.        
-000071b0: 2020 2020 4c65 6674 2078 2063 6f6f 7264      Left x coord
-000071c0: 696e 6174 6520 7768 6963 6820 7265 7072  inate which repr
-000071d0: 6573 656e 7473 2074 6865 2074 6f70 206f  esents the top o
-000071e0: 6620 7468 6520 6661 696c 7572 650a 2020  f the failure.  
-000071f0: 2020 2020 2020 2020 2020 706c 616e 652e            plane.
-00007200: 0a20 2020 2020 2020 2072 5f63 203a 2066  .        r_c : f
-00007210: 6c6f 6174 0a20 2020 2020 2020 2020 2020  loat.           
-00007220: 2052 6967 6874 2078 2063 6f6f 7264 696e   Right x coordin
-00007230: 6174 6520 7768 6963 6820 7265 7072 6573  ate which repres
-00007240: 656e 7473 2074 6865 2062 6f74 746f 6d20  ents the bottom 
-00007250: 6f66 2074 6865 2066 6169 6c75 7265 0a20  of the failure. 
-00007260: 2020 2020 2020 2020 2020 2070 6c61 6e65             plane
-00007270: 2e0a 2020 2020 2020 2020 6e75 6d5f 6369  ..        num_ci
-00007280: 7263 6c65 7320 3a20 696e 742c 206f 7074  rcles : int, opt
-00007290: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
-000072a0: 2020 6e75 6d62 6572 206f 6620 6469 6666    number of diff
-000072b0: 6572 656e 7420 6369 7263 6c65 2072 6164  erent circle rad
-000072c0: 6969 2074 6f20 6173 7365 7373 2070 6173  ii to assess pas
-000072d0: 7369 6e67 2074 6872 6f75 6768 0a20 2020  sing through.   
-000072e0: 2020 2020 2020 2020 2074 6865 2065 6e74           the ent
-000072f0: 7279 2061 6e64 2065 7869 7420 706f 696e  ry and exit poin
-00007300: 7473 2c20 6279 2064 6566 6175 6c74 2035  ts, by default 5
-00007310: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00007320: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-00007330: 2d0a 2020 2020 2020 2020 6c69 7374 206f  -.        list o
-00007340: 6620 6469 6374 696f 6e61 7269 6573 206f  f dictionaries o
-00007350: 6620 7468 6520 666f 726d 3a0a 2020 2020  f the form:.    
-00007360: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-00007370: 2020 226c 5f63 223a 206c 5f63 2c0a 2020    "l_c": l_c,.  
-00007380: 2020 2020 2020 2020 2020 2272 5f63 223a            "r_c":
-00007390: 2072 5f63 2c0a 2020 2020 2020 2020 2020   r_c,.          
-000073a0: 2020 2263 5f78 223a 2063 5f78 2c0a 2020    "c_x": c_x,.  
-000073b0: 2020 2020 2020 2020 2020 2263 5f79 223a            "c_y":
-000073c0: 2063 5f79 2c0a 2020 2020 2020 2020 2020   c_y,.          
-000073d0: 2020 2272 6164 6975 7322 3a20 7261 6469    "radius": radi
-000073e0: 7573 2c0a 2020 2020 2020 2020 7d0a 0a20  us,.        }.. 
-000073f0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00007400: 2020 2073 6561 7263 6820 3d20 5b5d 0a0a     search = []..
-00007410: 2020 2020 2020 2020 2320 6173 7375 6d65          # assume
-00007420: 2061 2073 7461 7274 696e 6720 6369 7263   a starting circ
-00007430: 6c65 2074 6861 7420 6861 7320 6120 7374  le that has a st
-00007440: 7261 6967 6874 2076 6572 7469 6361 6c20  raight vertical 
-00007450: 736c 6f70 6520 646f 776e 2061 7420 7468  slope down at th
-00007460: 6520 746f 7020 6f66 2074 6865 2073 6c6f  e top of the slo
-00007470: 7065 0a20 2020 2020 2020 2023 2074 6869  pe.        # thi
-00007480: 7320 6d65 616e 7320 7468 6520 6365 6e74  s means the cent
-00007490: 7265 206f 6620 7468 6520 6369 7263 6c65  re of the circle
-000074a0: 2069 7320 696e 206c 696e 6520 7769 7468   is in line with
-000074b0: 2074 6865 2074 6f70 206f 6620 7468 6520   the top of the 
-000074c0: 736c 6f70 650a 2020 2020 2020 2020 2320  slope.        # 
-000074d0: 7369 6e63 6520 7468 6520 7461 6e67 656e  since the tangen
-000074e0: 7420 6f66 2074 6865 2063 6972 636c 6520  t of the circle 
-000074f0: 6973 2070 6572 7065 6e64 6963 756c 6172  is perpendicular
-00007500: 2074 6f20 7468 6520 6365 6e74 7265 0a0a   to the centre..
-00007510: 2020 2020 2020 2020 2320 616e 676c 6520          # angle 
-00007520: 6f66 2073 6c6f 7065 206f 6620 6368 6f6f  of slope of choo
-00007530: 7264 2028 466f 7220 6369 7263 756c 6172  rd (For circular
-00007540: 2073 6c6f 7065 290a 2020 2020 2020 2020   slope).        
-00007550: 6265 7461 203d 2061 7461 6e28 286c 5f63  beta = atan((l_c
-00007560: 5b31 5d20 2d20 725f 635b 315d 2920 2f20  [1] - r_c[1]) / 
-00007570: 2872 5f63 5b30 5d20 2d20 6c5f 635b 305d  (r_c[0] - l_c[0]
-00007580: 2929 0a0a 2020 2020 2020 2020 2320 6861  ))..        # ha
-00007590: 6c66 206f 6620 7468 6520 6369 7263 6c65  lf of the circle
-000075a0: 2063 6f6f 7264 2074 6861 7420 7061 7373   coord that pass
-000075b0: 6573 7320 6672 6f6d 2074 6f70 206f 6620  ess from top of 
-000075c0: 706f 696e 7420 746f 2062 6f74 746f 6d20  point to bottom 
-000075d0: 6f66 2070 6f69 6e74 0a20 2020 2020 2020  of point.       
-000075e0: 2068 616c 665f 636f 6f72 645f 6469 7374   half_coord_dist
-000075f0: 616e 6365 203d 2073 7172 7428 286c 5f63  ance = sqrt((l_c
-00007600: 5b31 5d20 2d20 725f 635b 315d 2920 2a2a  [1] - r_c[1]) **
-00007610: 2032 202b 2028 725f 635b 305d 202d 206c   2 + (r_c[0] - l
-00007620: 5f63 5b30 5d29 202a 2a20 3229 202f 2032  _c[0]) ** 2) / 2
-00007630: 0a0a 2020 2020 2020 2020 2320 7374 6172  ..        # star
-00007640: 7469 6e67 2063 6972 636c 6520 6465 7461  ting circle deta
-00007650: 696c 732c 2069 6620 7261 6469 7573 2031  ils, if radius 1
-00007660: 2077 6f75 6c64 2062 6520 6120 7665 7274   would be a vert
-00007670: 6963 616c 2073 6c6f 7065 2e0a 2020 2020  ical slope..    
-00007680: 2020 2020 2320 696e 6372 6561 7365 2074      # increase t
-00007690: 6f20 312e 3120 746f 2070 7265 7665 6e74  o 1.1 to prevent
-000076a0: 206d 6120 6465 6e6f 6d69 6e61 746f 7220   ma denominator 
-000076b0: 6973 7375 6573 2066 6f72 2062 6973 686f  issues for bisho
-000076c0: 7073 206d 6574 686f 642e 0a20 2020 2020  ps method..     
-000076d0: 2020 2073 7461 7274 5f72 6164 6975 7320     start_radius 
-000076e0: 3d20 6861 6c66 5f63 6f6f 7264 5f64 6973  = half_coord_dis
-000076f0: 7461 6e63 6520 2f20 636f 7328 6265 7461  tance / cos(beta
-00007700: 2920 2a20 312e 310a 2020 2020 2020 2020  ) * 1.1.        
-00007710: 2320 7374 6172 745f 6365 6e74 7265 203d  # start_centre =
-00007720: 2028 6c5f 635b 305d 202b 2073 7461 7274   (l_c[0] + start
-00007730: 5f72 6164 6975 732c 206c 5f63 5b31 5d29  _radius, l_c[1])
-00007740: 0a20 2020 2020 2020 2073 7461 7274 5f63  .        start_c
-00007750: 686f 7264 5f74 6f5f 6365 6e74 7265 203d  hord_to_centre =
-00007760: 2073 7172 7428 7374 6172 745f 7261 6469   sqrt(start_radi
-00007770: 7573 2a2a 3220 2d20 6861 6c66 5f63 6f6f  us**2 - half_coo
-00007780: 7264 5f64 6973 7461 6e63 652a 2a32 290a  rd_distance**2).
-00007790: 2020 2020 2020 2020 7374 6172 745f 6368          start_ch
-000077a0: 6f72 645f 746f 5f65 6467 6520 3d20 7374  ord_to_edge = st
-000077b0: 6172 745f 7261 6469 7573 202d 2073 7461  art_radius - sta
-000077c0: 7274 5f63 686f 7264 5f74 6f5f 6365 6e74  rt_chord_to_cent
-000077d0: 7265 0a0a 2020 2020 2020 2020 2320 7477  re..        # tw
-000077e0: 6f20 696e 7465 7273 6563 7469 6e67 2063  o intersecting c
-000077f0: 686f 7264 7320 7468 726f 7567 6820 6369  hords through ci
-00007800: 7263 6c65 2068 6176 6520 7365 676d 656e  rcle have segmen
-00007810: 7473 206f 6620 6368 6f72 6473 2072 656c  ts of chords rel
-00007820: 6174 6564 0a20 2020 2020 2020 2023 2061  ated.        # a
-00007830: 7320 6120 2a20 6220 3d20 6320 2a20 6420  s a * b = c * d 
-00007840: 2c20 7768 6572 6520 6120 616e 6420 6220  , where a and b 
-00007850: 6172 6520 7468 6520 6c65 6e67 7468 7320  are the lengths 
-00007860: 6f66 2063 686f 7264 206f 6e20 6561 6368  of chord on each
-00007870: 2073 6964 6520 6f66 2069 6e74 6572 7365   side of interse
-00007880: 6374 696f 6e0a 2020 2020 2020 2020 2320  ction.        # 
-00007890: 6173 2073 7563 6820 7765 2068 6176 6520  as such we have 
-000078a0: 6861 6c66 5f63 6f6f 7264 5f64 6973 7461  half_coord_dista
-000078b0: 6e63 6520 2a2a 2032 203d 2063 686f 7264  nce ** 2 = chord
-000078c0: 5f74 6f5f 6564 6765 202a 2028 5220 2b20  _to_edge * (R + 
-000078d0: 2852 2d63 686f 7264 5f74 6f5f 6564 6765  (R-chord_to_edge
-000078e0: 2929 203d 2043 0a20 2020 2020 2020 2043  )) = C.        C
-000078f0: 203d 2068 616c 665f 636f 6f72 645f 6469   = half_coord_di
-00007900: 7374 616e 6365 2a2a 320a 0a20 2020 2020  stance**2..     
-00007910: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-00007920: 6528 302c 206e 756d 5f63 6972 636c 6573  e(0, num_circles
-00007930: 293a 0a0a 2020 2020 2020 2020 2020 2020  ):..            
-00007940: 2320 646f 6573 6e74 2069 6e63 6c75 6465  # doesnt include
-00007950: 2067 6f69 6e67 2061 6c6c 2074 6865 2077   going all the w
-00007960: 6179 2069 6e20 7768 6963 6820 7765 2064  ay in which we d
-00007970: 6f6e 7420 7761 6e74 2074 6f20 646f 2061  ont want to do a
-00007980: 6e79 7761 7973 0a20 2020 2020 2020 2020  nyways.         
-00007990: 2020 2063 686f 7264 5f74 6f5f 6564 6765     chord_to_edge
-000079a0: 203d 2073 7461 7274 5f63 686f 7264 5f74   = start_chord_t
-000079b0: 6f5f 6564 6765 202a 2028 6e75 6d5f 6369  o_edge * (num_ci
-000079c0: 7263 6c65 7320 2d20 6929 202f 206e 756d  rcles - i) / num
-000079d0: 5f63 6972 636c 6573 0a20 2020 2020 2020  _circles.       
-000079e0: 2020 2020 2072 6164 6975 7320 3d20 7574       radius = ut
-000079f0: 696c 6974 6965 732e 6369 7263 6c65 5f72  ilities.circle_r
-00007a00: 6164 6975 735f 6672 6f6d 5f61 6263 6428  adius_from_abcd(
-00007a10: 6368 6f72 645f 746f 5f65 6467 652c 2043  chord_to_edge, C
-00007a20: 290a 2020 2020 2020 2020 2020 2020 6365  ).            ce
-00007a30: 6e74 7265 203d 2075 7469 6c69 7469 6573  ntre = utilities
-00007a40: 2e63 6972 636c 655f 6365 6e74 7265 280a  .circle_centre(.
-00007a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a60: 6265 7461 3d62 6574 612c 0a20 2020 2020  beta=beta,.     
-00007a70: 2020 2020 2020 2020 2020 2063 686f 7264             chord
-00007a80: 5f69 6e74 6572 7365 6374 696f 6e3d 7574  _intersection=ut
-00007a90: 696c 6974 6965 732e 6d69 645f 636f 6f72  ilities.mid_coor
-00007aa0: 6428 6c5f 632c 2072 5f63 292c 0a20 2020  d(l_c, r_c),.   
-00007ab0: 2020 2020 2020 2020 2020 2020 2063 686f               cho
-00007ac0: 7264 5f74 6f5f 6365 6e74 7265 3d72 6164  rd_to_centre=rad
-00007ad0: 6975 7320 2d20 6368 6f72 645f 746f 5f65  ius - chord_to_e
-00007ae0: 6467 652c 0a20 2020 2020 2020 2020 2020  dge,.           
-00007af0: 2029 0a20 2020 2020 2020 2020 2020 2063   ).            c
-00007b00: 5f78 2c20 635f 7920 3d20 6365 6e74 7265  _x, c_y = centre
-00007b10: 0a0a 2020 2020 2020 2020 2020 2020 695f  ..            i_
-00007b20: 6c69 7374 203d 2073 656c 662e 5f67 6574  list = self._get
-00007b30: 5f63 6972 636c 655f 6578 7465 726e 616c  _circle_external
-00007b40: 5f69 6e74 6572 7365 6374 696f 6e28 635f  _intersection(c_
-00007b50: 782c 2063 5f79 2c20 7261 6469 7573 290a  x, c_y, radius).
-00007b60: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00007b70: 6c65 6e28 7365 7428 695f 6c69 7374 2929  len(set(i_list))
-00007b80: 203c 2032 3a0a 2020 2020 2020 2020 2020   < 2:.          
-00007b90: 2020 2020 2020 636f 6e74 696e 7565 0a0a        continue..
-00007ba0: 2020 2020 2020 2020 2020 2020 6c5f 6320              l_c 
-00007bb0: 3d20 695f 6c69 7374 5b30 5d0a 2020 2020  = i_list[0].    
-00007bc0: 2020 2020 2020 2020 725f 6320 3d20 695f          r_c = i_
-00007bd0: 6c69 7374 5b31 5d0a 0a20 2020 2020 2020  list[1]..       
-00007be0: 2020 2020 2073 6561 7263 6820 2b3d 205b       search += [
-00007bf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007c00: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00007c10: 2020 2020 2020 2022 6c5f 6322 3a20 6c5f         "l_c": l_
-00007c20: 632c 0a20 2020 2020 2020 2020 2020 2020  c,.             
-00007c30: 2020 2020 2020 2022 725f 6322 3a20 725f         "r_c": r_
-00007c40: 632c 0a20 2020 2020 2020 2020 2020 2020  c,.             
-00007c50: 2020 2020 2020 2022 635f 7822 3a20 635f         "c_x": c_
-00007c60: 782c 0a20 2020 2020 2020 2020 2020 2020  x,.             
-00007c70: 2020 2020 2020 2022 635f 7922 3a20 635f         "c_y": c_
-00007c80: 792c 0a20 2020 2020 2020 2020 2020 2020  y,.             
-00007c90: 2020 2020 2020 2022 7261 6469 7573 223a         "radius":
-00007ca0: 2072 6164 6975 732c 0a20 2020 2020 2020   radius,.       
-00007cb0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00007cc0: 2020 2020 2020 205d 0a0a 2020 2020 2020         ]..      
-00007cd0: 2020 7265 7475 726e 2073 6561 7263 680a    return search.
-00007ce0: 0a20 2020 2064 6566 2061 6464 5f73 696e  .    def add_sin
-00007cf0: 676c 655f 656e 7472 795f 6578 6974 5f70  gle_entry_exit_p
-00007d00: 6c61 6e65 2873 656c 662c 206c 5f63 782c  lane(self, l_cx,
-00007d10: 2072 5f63 782c 206e 756d 5f63 6972 636c   r_cx, num_circl
-00007d20: 6573 3d35 293a 0a20 2020 2020 2020 2022  es=5):.        "
-00007d30: 2222 4164 6420 6661 696c 7572 6520 706c  ""Add failure pl
-00007d40: 616e 6520 746f 2062 6520 616e 616c 7973  ane to be analys
-00007d50: 6564 2062 6520 7370 6563 6966 7969 6e67  ed be specifying
-00007d60: 2073 7461 7274 2061 6e64 2065 7869 7420   start and exit 
-00007d70: 706f 696e 742e 0a0a 2020 2020 2020 2020  point...        
-00007d80: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
-00007d90: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00007da0: 2020 2020 2020 6c5f 6320 3a20 666c 6f61        l_c : floa
-00007db0: 740a 2020 2020 2020 2020 2020 2020 4c65  t.            Le
-00007dc0: 6674 2078 2063 6f6f 7264 696e 6174 6520  ft x coordinate 
-00007dd0: 7768 6963 6820 7265 7072 6573 656e 7473  which represents
-00007de0: 2074 6865 2074 6f70 206f 6620 7468 6520   the top of the 
-00007df0: 6661 696c 7572 650a 2020 2020 2020 2020  failure.        
-00007e00: 2020 2020 706c 616e 652e 0a20 2020 2020      plane..     
-00007e10: 2020 2072 5f63 203a 2066 6c6f 6174 0a20     r_c : float. 
-00007e20: 2020 2020 2020 2020 2020 2052 6967 6874             Right
-00007e30: 2078 2063 6f6f 7264 696e 6174 6520 7768   x coordinate wh
-00007e40: 6963 6820 7265 7072 6573 656e 7473 2074  ich represents t
-00007e50: 6865 2062 6f74 746f 6d20 6f66 2074 6865  he bottom of the
-00007e60: 2066 6169 6c75 7265 0a20 2020 2020 2020   failure.       
-00007e70: 2020 2020 2070 6c61 6e65 2e0a 2020 2020       plane..    
-00007e80: 2020 2020 6e75 6d5f 6369 7263 6c65 7320      num_circles 
-00007e90: 3a20 696e 742c 206f 7074 696f 6e61 6c0a  : int, optional.
-00007ea0: 2020 2020 2020 2020 2020 2020 6e75 6d62              numb
-00007eb0: 6572 206f 6620 6469 6666 6572 656e 7420  er of different 
-00007ec0: 6369 7263 6c65 2072 6164 6969 2074 6f20  circle radii to 
-00007ed0: 6173 7365 7373 2070 6173 7369 6e67 2074  assess passing t
-00007ee0: 6872 6f75 6768 0a20 2020 2020 2020 2020  hrough.         
-00007ef0: 2020 2074 6865 2065 6e74 7279 2061 6e64     the entry and
-00007f00: 2065 7869 7420 706f 696e 7473 2c20 6279   exit points, by
-00007f10: 2064 6566 6175 6c74 2035 0a20 2020 2020   default 5.     
-00007f20: 2020 2022 2222 0a20 2020 2020 2020 2023     """.        #
-00007f30: 2061 6464 2062 7920 6164 6469 6e67 2069   add by adding i
-00007f40: 6e20 6c65 6674 2061 6e64 2072 6967 6874  n left and right
-00007f50: 2066 6169 6c75 7265 2063 6f6f 7264 696e   failure coordin
-00007f60: 6174 650a 2020 2020 2020 2020 7365 6c66  ate.        self
-00007f70: 2e5f 696e 6469 7669 6475 616c 5f70 6c61  ._individual_pla
-00007f80: 6e65 7320 2b3d 2073 656c 662e 5f67 656e  nes += self._gen
-00007f90: 6572 6174 655f 706c 616e 6573 280a 2020  erate_planes(.  
-00007fa0: 2020 2020 2020 2020 2020 286c 5f63 782c            (l_cx,
-00007fb0: 2073 656c 662e 6765 745f 6578 7465 726e   self.get_extern
-00007fc0: 616c 5f79 5f69 6e74 6572 7365 6374 696f  al_y_intersectio
-00007fd0: 6e28 6c5f 6378 2929 2c0a 2020 2020 2020  n(l_cx)),.      
-00007fe0: 2020 2020 2020 2872 5f63 782c 2073 656c        (r_cx, sel
-00007ff0: 662e 6765 745f 6578 7465 726e 616c 5f79  f.get_external_y
-00008000: 5f69 6e74 6572 7365 6374 696f 6e28 725f  _intersection(r_
-00008010: 6378 2929 2c0a 2020 2020 2020 2020 2020  cx)),.          
-00008020: 2020 6e75 6d5f 6369 7263 6c65 732c 0a20    num_circles,. 
-00008030: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-00008040: 2020 2320 7265 7365 7420 7265 7375 6c74    # reset result
-00008050: 730a 2020 2020 2020 2020 7365 6c66 2e5f  s.        self._
-00008060: 7265 7365 745f 7265 7375 6c74 7328 290a  reset_results().
-00008070: 0a20 2020 2064 6566 2061 6464 5f73 696e  .    def add_sin
-00008080: 676c 655f 6369 7263 756c 6172 5f70 6c61  gle_circular_pla
-00008090: 6e65 2873 656c 662c 2063 5f78 2c20 635f  ne(self, c_x, c_
-000080a0: 792c 2072 6164 6975 7329 3a0a 2020 2020  y, radius):.    
-000080b0: 2020 2020 2222 2241 6464 2066 6169 6c75      """Add failu
-000080c0: 7265 2070 6c61 6e65 2074 6f20 6265 2061  re plane to be a
-000080d0: 6e61 6c79 7365 6420 6279 2073 7065 6369  nalysed by speci
-000080e0: 6679 696e 6720 6369 7263 6c65 2070 726f  fying circle pro
-000080f0: 7065 7274 6965 732e 0a0a 2020 2020 2020  perties...      
-00008100: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-00008110: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
-00008120: 2020 2020 2020 2020 635f 7820 3a20 666c          c_x : fl
-00008130: 6f61 742c 0a20 2020 2020 2020 2020 2020  oat,.           
-00008140: 2063 656e 7472 6520 6f66 2063 6972 636c   centre of circl
-00008150: 6520 7820 636f 6f72 6469 6e61 7465 2e0a  e x coordinate..
-00008160: 2020 2020 2020 2020 635f 7920 3a20 666c          c_y : fl
-00008170: 6f61 742c 0a20 2020 2020 2020 2020 2020  oat,.           
-00008180: 2063 656e 7472 6520 6f66 2063 6972 636c   centre of circl
-00008190: 6520 7920 636f 6f72 6469 6e61 7465 2e0a  e y coordinate..
-000081a0: 2020 2020 2020 2020 7261 6469 7573 203a          radius :
-000081b0: 2066 6c6f 6174 0a20 2020 2020 2020 2020   float.         
-000081c0: 2020 2072 6164 6975 7320 6f66 2063 6972     radius of cir
-000081d0: 636c 650a 2020 2020 2020 2020 2222 220a  cle.        """.
-000081e0: 2020 2020 2020 2020 695f 6c69 7374 203d          i_list =
-000081f0: 2073 656c 662e 5f67 6574 5f63 6972 636c   self._get_circl
-00008200: 655f 6578 7465 726e 616c 5f69 6e74 6572  e_external_inter
-00008210: 7365 6374 696f 6e28 635f 782c 2063 5f79  section(c_x, c_y
-00008220: 2c20 7261 6469 7573 290a 2020 2020 2020  , radius).      
-00008230: 2020 6966 206c 656e 2873 6574 2869 5f6c    if len(set(i_l
-00008240: 6973 7429 2920 3c20 323a 0a20 2020 2020  ist)) < 2:.     
-00008250: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
-00008260: 6e65 0a20 2020 2020 2020 2065 6c73 653a  ne.        else:
-00008270: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00008280: 662e 5f69 6e64 6976 6964 7561 6c5f 706c  f._individual_pl
-00008290: 616e 6573 202b 3d20 5b0a 2020 2020 2020  anes += [.      
-000082a0: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
-000082b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082c0: 226c 5f63 223a 2069 5f6c 6973 745b 305d  "l_c": i_list[0]
-000082d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000082e0: 2020 2020 2020 2272 5f63 223a 2069 5f6c        "r_c": i_l
-000082f0: 6973 745b 315d 2c0a 2020 2020 2020 2020  ist[1],.        
-00008300: 2020 2020 2020 2020 2020 2020 2263 5f78              "c_x
-00008310: 223a 2063 5f78 2c0a 2020 2020 2020 2020  ": c_x,.        
-00008320: 2020 2020 2020 2020 2020 2020 2263 5f79              "c_y
-00008330: 223a 2063 5f79 2c0a 2020 2020 2020 2020  ": c_y,.        
-00008340: 2020 2020 2020 2020 2020 2020 2272 6164              "rad
-00008350: 6975 7322 3a20 7261 6469 7573 2c0a 2020  ius": radius,.  
-00008360: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
-00008370: 2020 2020 2020 2020 2020 2020 5d0a 0a20              ].. 
-00008380: 2020 2020 2020 2023 2072 6573 6574 2072         # reset r
-00008390: 6573 756c 7473 0a20 2020 2020 2020 2073  esults.        s
-000083a0: 656c 662e 5f72 6573 6574 5f72 6573 756c  elf._reset_resul
-000083b0: 7473 2829 0a0a 2020 2020 6465 6620 7265  ts()..    def re
-000083c0: 6d6f 7665 5f69 6e64 6976 6964 7561 6c5f  move_individual_
-000083d0: 706c 616e 6573 2873 656c 6629 3a0a 2020  planes(self):.  
-000083e0: 2020 2020 2020 2222 2252 656d 6f76 6520        """Remove 
-000083f0: 696e 6469 7669 6475 616c 6c79 2061 6464  individually add
-00008400: 6564 2066 6169 6c75 7265 2070 6c61 6e65  ed failure plane
-00008410: 732e 2222 220a 2020 2020 2020 2020 7365  s.""".        se
-00008420: 6c66 2e5f 696e 6469 7669 6475 616c 5f70  lf._individual_p
-00008430: 6c61 6e65 7320 3d20 5b5d 0a0a 2020 2020  lanes = []..    
-00008440: 2020 2020 2320 7265 7365 7420 7265 7375      # reset resu
-00008450: 6c74 730a 2020 2020 2020 2020 7365 6c66  lts.        self
-00008460: 2e5f 7265 7365 745f 7265 7375 6c74 7328  ._reset_results(
-00008470: 290a 0a20 2020 2064 6566 2061 6e61 6c79  )..    def analy
-00008480: 7365 5f73 6c6f 7065 2873 656c 662c 206d  se_slope(self, m
-00008490: 6178 5f66 6f73 3d4e 6f6e 6529 3a0a 2020  ax_fos=None):.  
-000084a0: 2020 2020 2020 2222 2241 6e61 6c79 7365        """Analyse
-000084b0: 206d 616e 7920 706f 7373 6962 6c65 2066   many possible f
-000084c0: 6169 6c75 7265 2070 6c61 6e65 7320 666f  ailure planes fo
-000084d0: 7220 6120 736c 6f70 6520 4f52 0a20 2020  r a slope OR.   
-000084e0: 2020 2020 2069 6e64 6976 7561 6c6c 7920       indivually 
-000084f0: 6164 6465 6420 6661 696c 7572 6520 706c  added failure pl
-00008500: 616e 6573 2069 6620 6164 6465 6420 746f  anes if added to
-00008510: 2073 6c6f 7065 2e22 2222 0a0a 2020 2020   slope."""..    
-00008520: 2020 2020 2320 6966 2069 6e64 6976 6964      # if individ
-00008530: 7561 6c20 6661 696c 7572 6520 706c 616e  ual failure plan
-00008540: 6573 2073 6574 206f 6e6c 7920 616e 616c  es set only anal
-00008550: 7973 6520 7468 656d 0a20 2020 2020 2020  yse them.       
-00008560: 2069 6620 7365 6c66 2e5f 696e 6469 7669   if self._indivi
-00008570: 6475 616c 5f70 6c61 6e65 7320 213d 205b  dual_planes != [
-00008580: 5d3a 0a20 2020 2020 2020 2020 2020 2073  ]:.            s
-00008590: 656c 662e 5f73 6561 7263 6820 3d20 7365  elf._search = se
-000085a0: 6c66 2e5f 696e 6469 7669 6475 616c 5f70  lf._individual_p
-000085b0: 6c61 6e65 730a 0a20 2020 2020 2020 2023  lanes..        #
-000085c0: 206f 7468 6572 7769 7365 2067 656e 6572   otherwise gener
-000085d0: 6174 6520 706c 616e 6573 2061 6372 6f73  ate planes acros
-000085e0: 7320 7468 6520 656e 7469 7265 2073 6c6f  s the entire slo
-000085f0: 7065 0a20 2020 2020 2020 2065 6c73 653a  pe.        else:
-00008600: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00008610: 662e 5f73 6574 5f65 6e74 7279 5f65 7869  f._set_entry_exi
-00008620: 745f 706c 616e 6573 2829 0a0a 2020 2020  t_planes()..    
-00008630: 2020 2020 2320 676f 2074 6872 6f75 6768      # go through
-00008640: 2065 6163 6820 6173 7375 6d65 6420 706c   each assumed pl
-00008650: 616e 6520 616e 6420 6361 6c63 756c 6174  ane and calculat
-00008660: 6520 7468 6520 464f 530a 2020 2020 2020  e the FOS.      
-00008670: 2020 666f 7220 692c 2073 6561 7263 6820    for i, search 
-00008680: 696e 2065 6e75 6d65 7261 7465 2874 7164  in enumerate(tqd
-00008690: 6d28 7365 6c66 2e5f 7365 6172 6368 2929  m(self._search))
-000086a0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000086b0: 6c66 2e5f 7365 6172 6368 5b69 5d5b 2246  lf._search[i]["F
-000086c0: 4f53 225d 203d 2073 656c 662e 5f61 6e61  OS"] = self._ana
-000086d0: 6c79 7365 5f63 6972 6375 6c61 725f 6661  lyse_circular_fa
-000086e0: 696c 7572 655f 6269 7368 6f70 280a 2020  ilure_bishop(.  
-000086f0: 2020 2020 2020 2020 2020 2020 2020 635f                c_
-00008700: 783d 7365 6172 6368 5b22 635f 7822 5d2c  x=search["c_x"],
-00008710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008720: 2063 5f79 3d73 6561 7263 685b 2263 5f79   c_y=search["c_y
-00008730: 225d 2c0a 2020 2020 2020 2020 2020 2020  "],.            
-00008740: 2020 2020 7261 6469 7573 3d73 6561 7263      radius=searc
-00008750: 685b 2272 6164 6975 7322 5d2c 0a20 2020  h["radius"],.   
-00008760: 2020 2020 2020 2020 2020 2020 206c 5f63               l_c
-00008770: 3d73 6561 7263 685b 226c 5f63 225d 2c0a  =search["l_c"],.
-00008780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008790: 725f 633d 7365 6172 6368 5b22 725f 6322  r_c=search["r_c"
-000087a0: 5d2c 0a20 2020 2020 2020 2020 2020 2029  ],.            )
-000087b0: 0a0a 2020 2020 2020 2020 6966 206f 732e  ..        if os.
-000087c0: 656e 7669 726f 6e2e 6765 7428 2244 4a41  environ.get("DJA
-000087d0: 4e47 4f5f 4445 4255 4722 2920 3d3d 2022  NGO_DEBUG") == "
-000087e0: 5452 5545 223a 0a20 2020 2020 2020 2020  TRUE":.         
-000087f0: 2020 2070 7269 6e74 2866 226c 656e 6774     print(f"lengt
-00008800: 6820 6f66 2073 6561 7263 6820 6973 207b  h of search is {
-00008810: 6c65 6e28 7365 6c66 2e5f 7365 6172 6368  len(self._search
-00008820: 297d 2229 0a0a 2020 2020 2020 2020 2320  )}")..        # 
-00008830: 7469 6479 2074 6865 2069 6e66 6f72 6d61  tidy the informa
-00008840: 7469 6f6e 2074 6f20 7265 6d6f 7665 2061  tion to remove a
-00008850: 6e79 7468 696e 6720 7468 6174 2064 6964  nything that did
-00008860: 6e74 2072 756e 2061 6e64 0a20 2020 2020  nt run and.     
-00008870: 2020 2023 2074 6f20 6265 2073 6f72 7465     # to be sorte
-00008880: 6420 6672 6f6d 206c 6f77 6573 7420 464f  d from lowest FO
-00008890: 5320 746f 2068 6967 6865 7374 2046 4f53  S to highest FOS
-000088a0: 0a20 2020 2020 2020 2073 6561 7263 6820  .        search 
-000088b0: 3d20 6c69 7374 2866 696c 7465 7228 286c  = list(filter((l
-000088c0: 616d 6264 6120 783a 2078 5b22 464f 5322  ambda x: x["FOS"
-000088d0: 5d20 6973 206e 6f74 204e 6f6e 6529 2c20  ] is not None), 
-000088e0: 7365 6c66 2e5f 7365 6172 6368 2929 0a20  self._search)). 
-000088f0: 2020 2020 2020 2073 6561 7263 682e 736f         search.so
-00008900: 7274 286b 6579 3d6c 616d 6264 6120 783a  rt(key=lambda x:
-00008910: 2078 5b22 464f 5322 5d29 0a20 2020 2020   x["FOS"]).     
-00008920: 2020 2069 6620 6d61 785f 666f 733a 0a20     if max_fos:. 
-00008930: 2020 2020 2020 2020 2020 2073 6561 7263             searc
-00008940: 6820 3d20 6c69 7374 2866 696c 7465 7228  h = list(filter(
-00008950: 6c61 6d62 6461 2078 3a20 2878 5b22 464f  lambda x: (x["FO
-00008960: 5322 5d20 3c3d 206d 6178 5f66 6f73 292c  S"] <= max_fos),
-00008970: 2073 6561 7263 6829 290a 0a20 2020 2020   search))..     
-00008980: 2020 2073 656c 662e 5f73 6561 7263 6820     self._search 
-00008990: 3d20 7365 6172 6368 0a0a 2020 2020 2020  = search..      
-000089a0: 2020 6966 206f 732e 656e 7669 726f 6e2e    if os.environ.
-000089b0: 6765 7428 2244 4a41 4e47 4f5f 4445 4255  get("DJANGO_DEBU
-000089c0: 4722 2920 3d3d 2022 5452 5545 223a 0a20  G") == "TRUE":. 
-000089d0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-000089e0: 2866 226c 656e 6774 6820 6f66 2073 6561  (f"length of sea
-000089f0: 7263 6820 6973 207b 6c65 6e28 7365 6c66  rch is {len(self
-00008a00: 2e5f 7365 6172 6368 297d 2229 0a0a 2020  ._search)}")..  
-00008a10: 2020 6465 6620 5f61 6e61 6c79 7365 5f63    def _analyse_c
-00008a20: 6972 6375 6c61 725f 6661 696c 7572 655f  ircular_failure_
-00008a30: 6f72 6469 6e61 7279 280a 2020 2020 2020  ordinary(.      
-00008a40: 2020 7365 6c66 2c20 635f 783a 2066 6c6f    self, c_x: flo
-00008a50: 6174 2c20 635f 793a 2066 6c6f 6174 2c20  at, c_y: float, 
-00008a60: 7261 6469 7573 3a20 666c 6f61 742c 206c  radius: float, l
-00008a70: 5f63 3d4e 6f6e 652c 2072 5f63 3d4e 6f6e  _c=None, r_c=Non
-00008a80: 650a 2020 2020 293a 0a20 2020 2020 2020  e.    ):.       
-00008a90: 2022 2222 4361 6c63 756c 6174 6520 6661   """Calculate fa
-00008aa0: 6374 6f72 206f 6620 7361 6665 7479 2066  ctor of safety f
-00008ab0: 6f72 2061 2063 6972 6375 6c61 7220 6661  or a circular fa
-00008ac0: 696c 7572 6520 706c 616e 6520 7468 726f  ilure plane thro
-00008ad0: 7567 6820 7468 6520 736c 6f70 650a 2020  ugh the slope.  
-00008ae0: 2020 2020 2020 7573 696e 6720 7468 6520        using the 
-00008af0: 6f72 6469 6e61 7279 206d 6574 686f 6420  ordinary method 
-00008b00: 2873 7765 6469 7368 206d 6574 686f 6420  (swedish method 
-00008b10: 6f66 2073 6c69 6365 7329 2e0a 0a20 2020  of slices)...   
-00008b20: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-00008b30: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00008b40: 2d2d 0a20 2020 2020 2020 2063 5f78 203a  --.        c_x :
-00008b50: 2066 6c6f 6174 0a20 2020 2020 2020 2020   float.         
-00008b60: 2020 2063 6972 636c 6520 6365 6e74 6572     circle center
-00008b70: 2078 2063 6f6f 7264 696e 6174 650a 2020   x coordinate.  
-00008b80: 2020 2020 2020 635f 7920 3a20 666c 6f61        c_y : floa
-00008b90: 740a 2020 2020 2020 2020 2020 2020 6369  t.            ci
-00008ba0: 7263 6c65 2063 656e 7465 7220 7920 636f  rcle center y co
-00008bb0: 6f72 6469 6e61 7465 0a20 2020 2020 2020  ordinate.       
-00008bc0: 2072 6164 6975 7320 3a20 666c 6f61 740a   radius : float.
-00008bd0: 2020 2020 2020 2020 2020 2020 6369 7263              circ
-00008be0: 6c65 2072 6164 6975 730a 2020 2020 2020  le radius.      
-00008bf0: 2020 6c5f 6320 3a20 7475 706c 652c 206f    l_c : tuple, o
-00008c00: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-00008c10: 2020 2020 636f 6f72 6469 6e61 7465 7320      coordinates 
-00008c20: 6f66 206c 6566 7420 696e 7465 7273 6563  of left intersec
-00008c30: 7469 6f6e 2062 6574 7765 656e 2062 6f75  tion between bou
-00008c40: 6e64 6172 7920 616e 640a 2020 2020 2020  ndary and.      
-00008c50: 2020 2020 2020 6661 696c 7572 6520 706c        failure pl
-00008c60: 616e 6520 6966 2061 6c72 6561 6479 206b  ane if already k
-00008c70: 6e6f 776e 2c20 6279 2064 6566 6175 6c74  nown, by default
-00008c80: 204e 6f6e 652e 0a20 2020 2020 2020 2072   None..        r
-00008c90: 5f63 203a 2074 7570 6c65 2c20 6f70 7469  _c : tuple, opti
-00008ca0: 6f6e 616c 0a20 2020 2020 2020 2020 2020  onal.           
-00008cb0: 2063 6f6f 7264 696e 6174 6573 206f 6620   coordinates of 
-00008cc0: 6c65 6674 2069 6e74 6572 7365 6374 696f  left intersectio
-00008cd0: 6e20 6265 7477 6565 6e20 626f 756e 6461  n between bounda
-00008ce0: 7279 2061 6e64 0a20 2020 2020 2020 2020  ry and.         
-00008cf0: 2020 2066 6169 6c75 7265 2070 6c61 6e65     failure plane
-00008d00: 2069 6620 616c 7265 6164 7920 6b6e 6f77   if already know
-00008d10: 6e2c 2062 7920 6465 6661 756c 7420 4e6f  n, by default No
-00008d20: 6e65 2e0a 0a0a 2020 2020 2020 2020 5265  ne....        Re
-00008d30: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
-00008d40: 2d2d 2d2d 2d0a 2020 2020 2020 2020 666c  -----.        fl
-00008d50: 6f61 740a 2020 2020 2020 2020 2020 2020  oat.            
-00008d60: 6661 6374 6f72 206f 6620 7361 6665 7479  factor of safety
-00008d70: 0a20 2020 2020 2020 204e 6f6e 650a 2020  .        None.  
-00008d80: 2020 2020 2020 2020 2020 6966 2063 616e            if can
-00008d90: 7420 6361 6c63 756c 6174 6520 7265 7475  t calculate retu
-00008da0: 726e 7320 4e6f 6e65 0a0a 2020 2020 2020  rns None..      
-00008db0: 2020 2222 220a 2020 2020 2020 2020 2320    """.        # 
-00008dc0: 6461 7461 2076 616c 6964 6174 696f 6e0a  data validation.
-00008dd0: 2020 2020 2020 2020 6461 7461 5f76 616c          data_val
-00008de0: 6964 6174 696f 6e2e 6173 7365 7274 5f73  idation.assert_s
-00008df0: 7472 6963 746c 795f 706f 7369 7469 7665  trictly_positive
-00008e00: 5f6e 756d 6265 7228 0a20 2020 2020 2020  _number(.       
-00008e10: 2020 2020 2063 5f78 2c20 2263 5f78 2028       c_x, "c_x (
-00008e20: 6369 7263 6c65 2078 2063 6f6f 7264 696e  circle x coordin
-00008e30: 6174 6529 220a 2020 2020 2020 2020 290a  ate)".        ).
-00008e40: 2020 2020 2020 2020 6461 7461 5f76 616c          data_val
-00008e50: 6964 6174 696f 6e2e 6173 7365 7274 5f73  idation.assert_s
-00008e60: 7472 6963 746c 795f 706f 7369 7469 7665  trictly_positive
-00008e70: 5f6e 756d 6265 7228 0a20 2020 2020 2020  _number(.       
-00008e80: 2020 2020 2063 5f79 2c20 2263 5f79 2028       c_y, "c_y (
-00008e90: 6369 7263 6c65 2079 2063 6f6f 7264 696e  circle y coordin
-00008ea0: 6174 6529 220a 2020 2020 2020 2020 290a  ate)".        ).
-00008eb0: 2020 2020 2020 2020 6461 7461 5f76 616c          data_val
-00008ec0: 6964 6174 696f 6e2e 6173 7365 7274 5f73  idation.assert_s
-00008ed0: 7472 6963 746c 795f 706f 7369 7469 7665  trictly_positive
-00008ee0: 5f6e 756d 6265 7228 7261 6469 7573 2c20  _number(radius, 
-00008ef0: 2272 6164 6975 7322 290a 0a20 2020 2020  "radius")..     
-00008f00: 2020 2023 2069 6620 6c5f 6320 616e 6420     # if l_c and 
-00008f10: 725f 6320 6e6f 7420 7365 7420 7468 656e  r_c not set then
-00008f20: 2075 7365 7220 6973 2070 726f 6261 626c   user is probabl
-00008f30: 7920 6368 6563 6b69 6e67 2061 6e20 696e  y checking an in
-00008f40: 6469 7669 6475 616c 2063 6972 6375 6c61  dividual circula
-00008f50: 7220 706c 616e 650a 2020 2020 2020 2020  r plane.        
-00008f60: 2320 6361 6e20 6765 7420 7468 6520 7269  # can get the ri
-00008f70: 6768 7420 616e 6420 6c65 6674 2063 6f6f  ght and left coo
-00008f80: 7264 696e 6174 6520 696e 7465 7273 6563  rdinate intersec
-00008f90: 7469 6f6e 2077 6974 6820 7468 6520 6d6f  tion with the mo
-00008fa0: 6465 6c20 666f 7220 7468 6973 2063 6173  del for this cas
-00008fb0: 652e 0a20 2020 2020 2020 2069 6620 6c5f  e..        if l_
-00008fc0: 6320 6973 204e 6f6e 6520 6f72 2072 5f63  c is None or r_c
-00008fd0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00008fe0: 2020 2020 2020 695f 6c69 7374 203d 2073        i_list = s
-00008ff0: 656c 662e 5f67 6574 5f63 6972 636c 655f  elf._get_circle_
-00009000: 6578 7465 726e 616c 5f69 6e74 6572 7365  external_interse
-00009010: 6374 696f 6e28 635f 782c 2063 5f79 2c20  ction(c_x, c_y, 
-00009020: 7261 6469 7573 290a 2020 2020 2020 2020  radius).        
-00009030: 2020 2020 6966 206c 656e 2873 6574 2869      if len(set(i
-00009040: 5f6c 6973 7429 2920 213d 2032 3a0a 2020  _list)) != 2:.  
-00009050: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00009060: 7475 726e 204e 6f6e 650a 2020 2020 2020  turn None.      
-00009070: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00009080: 2020 2020 695f 6c69 7374 203d 205b 6c5f      i_list = [l_
-00009090: 632c 2072 5f63 5d0a 0a20 2020 2020 2020  c, r_c]..       
-000090a0: 2023 2074 6f74 616c 206e 756d 6265 7220   # total number 
-000090b0: 6f66 2073 6c69 6365 730a 2020 2020 2020  of slices.      
-000090c0: 2020 534c 4943 4553 203d 2073 656c 662e    SLICES = self.
-000090d0: 5f73 6c69 6365 730a 0a20 2020 2020 2020  _slices..       
-000090e0: 2023 2068 6f72 697a 6f6e 7461 6c20 6469   # horizontal di
-000090f0: 7374 616e 6365 2062 6574 7765 656e 206c  stance between l
-00009100: 6566 7420 616e 6420 7269 6768 7420 736c  eft and right sl
-00009110: 6963 650a 2020 2020 2020 2020 6469 7374  ice.        dist
-00009120: 203d 2069 5f6c 6973 745b 315d 5b30 5d20   = i_list[1][0] 
-00009130: 2d20 695f 6c69 7374 5b30 5d5b 305d 0a0a  - i_list[0][0]..
-00009140: 2020 2020 2020 2020 2320 7769 6474 6820          # width 
-00009150: 6f66 2061 2073 6c69 6365 0a20 2020 2020  of a slice.     
-00009160: 2020 2062 203d 2064 6973 7420 2f20 534c     b = dist / SL
-00009170: 4943 4553 0a0a 2020 2020 2020 2020 6966  ICES..        if
-00009180: 2062 203c 3d20 302e 3030 3030 3031 3a0a   b <= 0.000001:.
-00009190: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000091a0: 726e 204e 6f6e 650a 0a20 2020 2020 2020  rn None..       
-000091b0: 2023 2069 6e69 7469 616c 6973 6520 6365   # initialise ce
-000091c0: 6e74 7265 2070 6f69 6e74 206f 6620 6669  ntre point of fi
-000091d0: 7273 7420 736c 6963 650a 2020 2020 2020  rst slice.      
-000091e0: 2020 735f 7820 3d20 695f 6c69 7374 5b30    s_x = i_list[0
-000091f0: 5d5b 305d 202b 2062 202f 2032 0a0a 2020  ][0] + b / 2..  
-00009200: 2020 2020 2020 2320 696e 7469 616c 6973        # intialis
-00009210: 6520 7468 6520 7075 7368 2061 6e64 2072  e the push and r
-00009220: 6573 6973 7461 6e63 6520 636f 6d70 6f6e  esistance compon
-00009230: 656e 7473 2066 6f72 2046 4f53 2062 6566  ents for FOS bef
-00009240: 6f72 6520 6c6f 6f70 696e 670a 2020 2020  ore looping.    
-00009250: 2020 2020 7075 7368 696e 6720 3d20 302e      pushing = 0.
-00009260: 300a 2020 2020 2020 2020 7265 7369 7374  0.        resist
-00009270: 696e 6720 3d20 302e 300a 0a20 2020 2020  ing = 0.0..     
-00009280: 2020 2023 206c 6f6f 7020 7468 726f 7567     # loop throug
-00009290: 6820 736c 6963 6573 0a20 2020 2020 2020  h slices.       
-000092a0: 2066 6f72 205f 2069 6e20 7261 6e67 6528   for _ in range(
-000092b0: 302c 2053 4c49 4345 5329 3a0a 2020 2020  0, SLICES):.    
-000092c0: 2020 2020 2020 2020 2320 6465 6669 6e65          # define
-000092d0: 2079 2063 6f6f 7264 696e 6174 6573 2066   y coordinates f
-000092e0: 6f72 2073 6c69 6365 2062 6f74 746f 6d0a  or slice bottom.
-000092f0: 2020 2020 2020 2020 2020 2020 2320 4841              # HA
-00009300: 5320 4552 524f 520a 2020 2020 2020 2020  S ERROR.        
-00009310: 2020 2020 2320 2863 7920 2d20 735f 7962      # (cy - s_yb
-00009320: 2920 2a2a 2032 202b 2061 6273 2873 5f78  ) ** 2 + abs(s_x
-00009330: 2d63 5f78 292a 2a32 203d 2052 202a 2a20  -c_x)**2 = R ** 
-00009340: 320a 2020 2020 2020 2020 2020 2020 2320  2.            # 
-00009350: 7371 7274 2852 2a2a 3220 2d20 6162 7328  sqrt(R**2 - abs(
-00009360: 735f 782d 635f 7829 2a2a 3229 203d 2063  s_x-c_x)**2) = c
-00009370: 5f79 202d 2073 5f79 620a 2020 2020 2020  _y - s_yb.      
-00009380: 2020 2020 2020 735f 7962 203d 2063 5f79        s_yb = c_y
-00009390: 202d 2073 7172 7428 7261 6469 7573 2a2a   - sqrt(radius**
-000093a0: 3220 2d20 6162 7328 735f 7820 2d20 635f  2 - abs(s_x - c_
-000093b0: 7829 202a 2a20 3229 0a0a 2020 2020 2020  x) ** 2)..      
-000093c0: 2020 2020 2020 2320 6765 7420 7920 636f        # get y co
-000093d0: 6f72 6469 6e61 7465 2061 7420 736c 6963  ordinate at slic
-000093e0: 6520 746f 700a 2020 2020 2020 2020 2020  e top.          
-000093f0: 2020 735f 7974 203d 2073 656c 662e 6765    s_yt = self.ge
-00009400: 745f 6578 7465 726e 616c 5f79 5f69 6e74  t_external_y_int
-00009410: 6572 7365 6374 696f 6e28 735f 7829 0a0a  ersection(s_x)..
-00009420: 2020 2020 2020 2020 2020 2020 2320 6f75              # ou
-00009430: 7420 6f66 2062 6f75 6e64 730a 2020 2020  t of bounds.    
-00009440: 2020 2020 2020 2020 6966 2073 5f79 7420          if s_yt 
-00009450: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00009460: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00009470: 4e6f 6e65 0a0a 2020 2020 2020 2020 2020  None..          
-00009480: 2020 6966 2073 5f79 7420 3c20 735f 7962    if s_yt < s_yb
-00009490: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000094a0: 2020 735f 7974 203d 2073 5f79 620a 0a20    s_yt = s_yb.. 
-000094b0: 2020 2020 2020 2020 2020 2023 2067 6574             # get
-000094c0: 2061 6c70 6861 2c20 6479 2061 6c77 6179   alpha, dy alway
-000094d0: 7320 706f 7369 7469 7665 2c20 6478 206e  s positive, dx n
-000094e0: 6567 6174 6976 6520 746f 2072 6967 6874  egative to right
-000094f0: 2028 7570 6869 6c6c 292c 2064 7820 706f   (uphill), dx po
-00009500: 7369 7469 7665 2074 6f20 6c65 6674 0a20  sitive to left. 
-00009510: 2020 2020 2020 2020 2020 2023 206e 6f74             # not
-00009520: 6520 616c 7068 6120 696e 2072 6164 6961  e alpha in radia
-00009530: 6e73 2062 7920 6465 6661 756c 740a 2020  ns by default.  
-00009540: 2020 2020 2020 2020 2020 6479 203d 2063            dy = c
-00009550: 5f79 202d 2073 5f79 620a 2020 2020 2020  _y - s_yb.      
-00009560: 2020 2020 2020 6478 203d 2063 5f78 202d        dx = c_x -
-00009570: 2073 5f78 0a20 2020 2020 2020 2020 2020   s_x.           
-00009580: 2061 6c70 6861 203d 2061 7461 6e28 6478   alpha = atan(dx
-00009590: 202f 2064 7929 0a0a 2020 2020 2020 2020   / dy)..        
-000095a0: 2020 2020 2320 6765 7420 6c65 6e67 7468      # get length
-000095b0: 0a20 2020 2020 2020 2020 2020 2069 6e63  .            inc
-000095c0: 6c69 6e65 645f 6c65 6e67 7468 203d 2062  lined_length = b
-000095d0: 202f 2063 6f73 2861 6c70 6861 290a 0a20   / cos(alpha).. 
-000095e0: 2020 2020 2020 2020 2020 2023 2063 616c             # cal
-000095f0: 6375 6c61 7465 2073 7472 6970 2077 6569  culate strip wei
-00009600: 6768 740a 2020 2020 2020 2020 2020 2020  ght.            
-00009610: 5720 3d20 7365 6c66 2e5f 6361 6c63 756c  W = self._calcul
-00009620: 6174 655f 7374 7269 705f 7765 6967 6874  ate_strip_weight
-00009630: 2862 2c20 735f 7974 2c20 735f 7962 290a  (b, s_yt, s_yb).
-00009640: 0a20 2020 2020 2020 2020 2020 2023 2067  .            # g
-00009650: 6574 206d 6174 6572 6961 6c20 7072 6f70  et material prop
-00009660: 6572 7469 6573 2061 7420 7468 6520 626f  erties at the bo
-00009670: 7474 6f6d 206f 6620 7468 6520 736c 6963  ttom of the slic
-00009680: 650a 2020 2020 2020 2020 2020 2020 626f  e.            bo
-00009690: 7474 6f6d 5f6d 6174 6572 6961 6c20 3d20  ttom_material = 
-000096a0: 7365 6c66 2e5f 6765 745f 6d61 7465 7269  self._get_materi
-000096b0: 616c 5f61 745f 6465 7074 6828 735f 7962  al_at_depth(s_yb
-000096c0: 290a 0a20 2020 2020 2020 2020 2020 2063  )..            c
-000096d0: 6f68 6573 696f 6e20 3d20 626f 7474 6f6d  ohesion = bottom
-000096e0: 5f6d 6174 6572 6961 6c2e 636f 6865 7369  _material.cohesi
-000096f0: 6f6e 0a20 2020 2020 2020 2020 2020 2066  on.            f
-00009700: 7269 6374 696f 6e5f 616e 676c 6520 3d20  riction_angle = 
-00009710: 626f 7474 6f6d 5f6d 6174 6572 6961 6c2e  bottom_material.
-00009720: 6672 6963 7469 6f6e 5f61 6e67 6c65 0a0a  friction_angle..
-00009730: 2020 2020 2020 2020 2020 2020 2320 6966              # if
-00009740: 2074 6865 7265 2069 7320 6120 7564 6c20   there is a udl 
-00009750: 6c6f 6164 206f 6e20 7468 6520 7374 7269  load on the stri
-00009760: 7020 6170 706c 7920 6974 2e0a 2020 2020  p apply it..    
-00009770: 2020 2020 2020 2020 666f 7220 7564 6c20          for udl 
-00009780: 696e 2073 656c 662e 5f75 646c 733a 0a20  in self._udls:. 
-00009790: 2020 2020 2020 2020 2020 2020 2020 2057                 W
-000097a0: 202b 3d20 7365 6c66 2e5f 6361 6c63 756c   += self._calcul
-000097b0: 6174 655f 7374 7269 705f 7564 6c5f 666f  ate_strip_udl_fo
-000097c0: 7263 6528 622c 2073 5f78 2c20 7564 6c29  rce(b, s_x, udl)
-000097d0: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-000097e0: 6966 2074 6865 7265 2069 7320 6120 706f  if there is a po
-000097f0: 696e 7420 6c6f 6164 206f 6e20 7468 6520  int load on the 
-00009800: 7374 7269 7020 6170 706c 7920 6974 2e0a  strip apply it..
-00009810: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00009820: 6c6c 2069 6e20 7365 6c66 2e5f 6c6c 733a  ll in self._lls:
-00009830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009840: 2057 202b 3d20 7365 6c66 2e5f 6361 6c63   W += self._calc
-00009850: 756c 6174 655f 7374 7269 705f 6c6c 2862  ulate_strip_ll(b
-00009860: 2c20 735f 782c 206c 6c29 0a0a 2020 2020  , s_x, ll)..    
-00009870: 2020 2020 2020 2020 2320 636f 6e73 6964          # consid
-00009880: 6572 6174 696f 6e20 666f 7220 7761 7465  eration for wate
-00009890: 720a 2020 2020 2020 2020 2020 2020 6966  r.            if
-000098a0: 2073 656c 662e 5f77 6174 6572 5f52 4c3a   self._water_RL:
-000098b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000098c0: 2023 2064 6574 6572 6d69 6e65 2048 2066   # determine H f
-000098d0: 6163 746f 7220 6261 7365 6420 6f6e 2073  actor based on s
-000098e0: 6574 7469 6e67 0a20 2020 2020 2020 2020  etting.         
-000098f0: 2020 2020 2020 2023 2068 7474 7073 3a2f         # https:/
-00009900: 2f77 7777 2e72 6f63 7363 6965 6e63 652e  /www.rocscience.
-00009910: 636f 6d2f 6865 6c70 2f73 6c69 6465 322f  com/help/slide2/
-00009920: 646f 6375 6d65 6e74 6174 696f 6e2f 736c  documentation/sl
-00009930: 6964 652d 6d6f 6465 6c2f 6d61 7465 7269  ide-model/materi
-00009940: 616c 2d70 726f 7065 7274 6965 732f 6465  al-properties/de
-00009950: 6669 6e65 2d6d 6174 6572 6961 6c2d 7072  fine-material-pr
-00009960: 6f70 6572 7469 6573 2f77 6174 6572 2d70  operties/water-p
-00009970: 6172 616d 6574 6572 730a 0a20 2020 2020  arameters..     
-00009980: 2020 2020 2020 2020 2020 2023 206f 6e6c             # onl
-00009990: 7920 7573 6520 4820 6661 6374 6f72 2069  y use H factor i
-000099a0: 6620 7761 7465 7220 736c 6f70 696e 670a  f water sloping.
-000099b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099c0: 6966 2028 0a20 2020 2020 2020 2020 2020  if (.           
-000099d0: 2020 2020 2020 2020 2073 656c 662e 6765           self.ge
-000099e0: 745f 6578 7465 726e 616c 5f78 5f69 6e74  t_external_x_int
-000099f0: 6572 7365 6374 696f 6e28 7365 6c66 2e5f  ersection(self._
-00009a00: 7761 7465 725f 524c 290a 2020 2020 2020  water_RL).      
-00009a10: 2020 2020 2020 2020 2020 2020 2020 3c20                < 
-00009a20: 735f 780a 2020 2020 2020 2020 2020 2020  s_x.            
-00009a30: 2020 2020 2020 2020 3c20 7365 6c66 2e5f          < self._
-00009a40: 626f 745f 636f 6f72 645b 305d 0a20 2020  bot_coord[0].   
-00009a50: 2020 2020 2020 2020 2020 2020 2029 3a0a               ):.
-00009a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a70: 2020 2020 5520 3d20 280a 2020 2020 2020      U = (.      
-00009a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a90: 2020 6d61 7828 6d69 6e28 7365 6c66 2e5f    max(min(self._
-00009aa0: 7761 7465 725f 524c 2c20 735f 7974 2920  water_RL, s_yt) 
-00009ab0: 2d20 735f 7962 2c20 3029 0a20 2020 2020  - s_yb, 0).     
-00009ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ad0: 2020 202a 2039 2e38 310a 2020 2020 2020     * 9.81.      
-00009ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009af0: 2020 2a20 696e 636c 696e 6564 5f6c 656e    * inclined_len
-00009b00: 6774 680a 2020 2020 2020 2020 2020 2020  gth.            
-00009b10: 2020 2020 2020 2020 2020 2020 2a20 7365              * se
-00009b20: 6c66 2e5f 7761 7465 725f 616e 616c 7973  lf._water_analys
-00009b30: 6973 5f48 0a20 2020 2020 2020 2020 2020  is_H.           
-00009b40: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00009b50: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00009b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009b70: 2020 2020 2055 203d 2028 0a20 2020 2020       U = (.     
-00009b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b90: 2020 206d 6178 286d 696e 2873 656c 662e     max(min(self.
-00009ba0: 5f77 6174 6572 5f52 4c2c 2073 5f79 7429  _water_RL, s_yt)
-00009bb0: 202d 2073 5f79 622c 2030 290a 2020 2020   - s_yb, 0).    
-00009bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009bd0: 2020 2020 2a20 392e 3831 0a20 2020 2020      * 9.81.     
-00009be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009bf0: 2020 202a 2069 6e63 6c69 6e65 645f 6c65     * inclined_le
-00009c00: 6e67 7468 0a20 2020 2020 2020 2020 2020  ngth.           
-00009c10: 2020 2020 2020 2020 2020 2020 202a 2031               * 1
-00009c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009c30: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00009c40: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00009c50: 2020 2020 2020 2020 2055 203d 2030 0a0a           U = 0..
-00009c60: 2020 2020 2020 2020 2020 2020 2320 6361              # ca
-00009c70: 6c63 756c 6174 6520 7265 7369 7374 696e  lculate resistin
-00009c80: 670a 2020 2020 2020 2020 2020 2020 7265  g.            re
-00009c90: 7369 7374 696e 6720 2b3d 2063 6f68 6573  sisting += cohes
-00009ca0: 696f 6e20 2a20 696e 636c 696e 6564 5f6c  ion * inclined_l
-00009cb0: 656e 6774 6820 2b20 6d61 7828 0a20 2020  ength + max(.   
-00009cc0: 2020 2020 2020 2020 2020 2020 2030 2c20               0, 
-00009cd0: 2857 202a 2063 6f73 2861 6c70 6861 2920  (W * cos(alpha) 
-00009ce0: 2d20 5529 0a20 2020 2020 2020 2020 2020  - U).           
-00009cf0: 2029 202a 2074 616e 2872 6164 6961 6e73   ) * tan(radians
-00009d00: 2866 7269 6374 696f 6e5f 616e 676c 6529  (friction_angle)
-00009d10: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
-00009d20: 2063 616c 6375 6c61 7465 2070 7573 6869   calculate pushi
-00009d30: 6e67 0a20 2020 2020 2020 2020 2020 2070  ng.            p
-00009d40: 7573 6869 6e67 202b 3d20 5720 2a20 7369  ushing += W * si
-00009d50: 6e28 616c 7068 6129 0a0a 2020 2020 2020  n(alpha)..      
-00009d60: 2020 2020 2020 2320 696e 6974 6961 6c69        # initiali
-00009d70: 7365 2073 6c69 6365 2078 2063 6f6f 7264  se slice x coord
-00009d80: 696e 6174 6520 666f 7220 6e65 7874 206c  inate for next l
-00009d90: 6f6f 700a 2020 2020 2020 2020 2020 2020  oop.            
-00009da0: 735f 7820 3d20 735f 7820 2b20 620a 0a20  s_x = s_x + b.. 
-00009db0: 2020 2020 2020 2069 6620 7075 7368 696e         if pushin
-00009dc0: 6720 3c3d 2030 3a0a 2020 2020 2020 2020  g <= 0:.        
-00009dd0: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
-00009de0: 0a20 2020 2020 2020 2046 4f53 203d 2072  .        FOS = r
-00009df0: 6573 6973 7469 6e67 202f 2070 7573 6869  esisting / pushi
-00009e00: 6e67 0a0a 2020 2020 2020 2020 7265 7475  ng..        retu
-00009e10: 726e 2046 4f53 0a0a 2020 2020 2320 6269  rn FOS..    # bi
-00009e20: 7368 6f70 0a0a 2020 2020 6465 6620 5f61  shop..    def _a
-00009e30: 6e61 6c79 7365 5f63 6972 6375 6c61 725f  nalyse_circular_
-00009e40: 6661 696c 7572 655f 6269 7368 6f70 280a  failure_bishop(.
-00009e50: 2020 2020 2020 2020 7365 6c66 2c20 635f          self, c_
-00009e60: 783a 2066 6c6f 6174 2c20 635f 793a 2066  x: float, c_y: f
-00009e70: 6c6f 6174 2c20 7261 6469 7573 3a20 666c  loat, radius: fl
-00009e80: 6f61 742c 206c 5f63 3d4e 6f6e 652c 2072  oat, l_c=None, r
-00009e90: 5f63 3d4e 6f6e 650a 2020 2020 293a 0a20  _c=None.    ):. 
-00009ea0: 2020 2020 2020 2022 2222 4361 6c63 756c         """Calcul
-00009eb0: 6174 6520 6661 6374 6f72 206f 6620 7361  ate factor of sa
-00009ec0: 6665 7479 2066 6f72 2061 2063 6972 6375  fety for a circu
-00009ed0: 6c61 7220 6661 696c 7572 6520 706c 616e  lar failure plan
-00009ee0: 6520 7468 726f 7567 6820 7468 6520 736c  e through the sl
-00009ef0: 6f70 650a 2020 2020 2020 2020 7573 696e  ope.        usin
-00009f00: 6720 6269 7368 6f70 7320 6d65 7468 6f64  g bishops method
-00009f10: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-00009f20: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
-00009f30: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-00009f40: 2063 5f78 203a 2066 6c6f 6174 0a20 2020   c_x : float.   
-00009f50: 2020 2020 2020 2020 2063 6972 636c 6520           circle 
-00009f60: 6365 6e74 6572 2078 2063 6f6f 7264 696e  center x coordin
-00009f70: 6174 650a 2020 2020 2020 2020 635f 7920  ate.        c_y 
-00009f80: 3a20 666c 6f61 740a 2020 2020 2020 2020  : float.        
-00009f90: 2020 2020 6369 7263 6c65 2063 656e 7465      circle cente
-00009fa0: 7220 7920 636f 6f72 6469 6e61 7465 0a20  r y coordinate. 
-00009fb0: 2020 2020 2020 2072 6164 6975 7320 3a20         radius : 
-00009fc0: 666c 6f61 740a 2020 2020 2020 2020 2020  float.          
-00009fd0: 2020 6369 7263 6c65 2072 6164 6975 730a    circle radius.
-00009fe0: 2020 2020 2020 2020 6c5f 6320 3a20 7475          l_c : tu
-00009ff0: 706c 652c 206f 7074 696f 6e61 6c0a 2020  ple, optional.  
-0000a000: 2020 2020 2020 2020 2020 636f 6f72 6469            coordi
-0000a010: 6e61 7465 7320 6f66 206c 6566 7420 696e  nates of left in
-0000a020: 7465 7273 6563 7469 6f6e 2062 6574 7765  tersection betwe
-0000a030: 656e 2062 6f75 6e64 6172 7920 616e 640a  en boundary and.
-0000a040: 2020 2020 2020 2020 2020 2020 6661 696c              fail
-0000a050: 7572 6520 706c 616e 6520 6966 2061 6c72  ure plane if alr
-0000a060: 6561 6479 206b 6e6f 776e 2c20 6279 2064  eady known, by d
-0000a070: 6566 6175 6c74 204e 6f6e 652e 0a20 2020  efault None..   
-0000a080: 2020 2020 2072 5f63 203a 2074 7570 6c65       r_c : tuple
-0000a090: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-0000a0a0: 2020 2020 2020 2063 6f6f 7264 696e 6174         coordinat
-0000a0b0: 6573 206f 6620 6c65 6674 2069 6e74 6572  es of left inter
-0000a0c0: 7365 6374 696f 6e20 6265 7477 6565 6e20  section between 
-0000a0d0: 626f 756e 6461 7279 2061 6e64 0a20 2020  boundary and.   
-0000a0e0: 2020 2020 2020 2020 2066 6169 6c75 7265           failure
-0000a0f0: 2070 6c61 6e65 2069 6620 616c 7265 6164   plane if alread
-0000a100: 7920 6b6e 6f77 6e2c 2062 7920 6465 6661  y known, by defa
-0000a110: 756c 7420 4e6f 6e65 2e0a 0a0a 2020 2020  ult None....    
-0000a120: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-0000a130: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-0000a140: 2020 2020 666c 6f61 740a 2020 2020 2020      float.      
-0000a150: 2020 2020 2020 6661 6374 6f72 206f 6620        factor of 
-0000a160: 7361 6665 7479 0a20 2020 2020 2020 204e  safety.        N
-0000a170: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-0000a180: 6966 2063 616e 7420 6361 6c63 756c 6174  if cant calculat
-0000a190: 6520 7265 7475 726e 7320 4e6f 6e65 0a0a  e returns None..
-0000a1a0: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
-0000a1b0: 2020 2020 2023 2069 6620 6c5f 6320 616e       # if l_c an
-0000a1c0: 6420 725f 6320 6e6f 7420 7365 7420 7468  d r_c not set th
-0000a1d0: 656e 2075 7365 7220 6973 2070 726f 6261  en user is proba
-0000a1e0: 626c 7920 6368 6563 6b69 6e67 2061 6e20  bly checking an 
-0000a1f0: 696e 6469 7669 6475 616c 2063 6972 6375  individual circu
-0000a200: 6c61 7220 706c 616e 650a 2020 2020 2020  lar plane.      
-0000a210: 2020 2320 6361 6e20 6765 7420 7468 6520    # can get the 
-0000a220: 7269 6768 7420 616e 6420 6c65 6674 2063  right and left c
-0000a230: 6f6f 7264 696e 6174 6520 696e 7465 7273  oordinate inters
-0000a240: 6563 7469 6f6e 2077 6974 6820 7468 6520  ection with the 
-0000a250: 6d6f 6465 6c20 666f 7220 7468 6973 2063  model for this c
-0000a260: 6173 652e 0a20 2020 2020 2020 2069 6620  ase..        if 
-0000a270: 6c5f 6320 6973 204e 6f6e 6520 6f72 2072  l_c is None or r
-0000a280: 5f63 2069 7320 4e6f 6e65 3a0a 2020 2020  _c is None:.    
-0000a290: 2020 2020 2020 2020 695f 6c69 7374 203d          i_list =
-0000a2a0: 2073 656c 662e 5f67 6574 5f63 6972 636c   self._get_circl
-0000a2b0: 655f 6578 7465 726e 616c 5f69 6e74 6572  e_external_inter
-0000a2c0: 7365 6374 696f 6e28 635f 782c 2063 5f79  section(c_x, c_y
-0000a2d0: 2c20 7261 6469 7573 290a 2020 2020 2020  , radius).      
-0000a2e0: 2020 2020 2020 6966 206c 656e 2873 6574        if len(set
-0000a2f0: 2869 5f6c 6973 7429 2920 3c20 323a 0a20  (i_list)) < 2:. 
-0000a300: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000a310: 6574 7572 6e20 4e6f 6e65 0a20 2020 2020  eturn None.     
-0000a320: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000a330: 2020 2020 2020 2020 2020 2020 206c 5f63               l_c
-0000a340: 2c20 725f 6320 3d20 695f 6c69 7374 5b30  , r_c = i_list[0
-0000a350: 5d2c 2069 5f6c 6973 745b 315d 0a20 2020  ], i_list[1].   
-0000a360: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000a370: 2020 2020 2020 2069 5f6c 6973 7420 3d20         i_list = 
-0000a380: 5b6c 5f63 2c20 725f 635d 0a0a 2020 2020  [l_c, r_c]..    
-0000a390: 2020 2020 4653 203d 2073 656c 662e 5f61      FS = self._a
-0000a3a0: 6e61 6c79 7365 5f63 6972 6375 6c61 725f  nalyse_circular_
-0000a3b0: 6661 696c 7572 655f 6f72 6469 6e61 7279  failure_ordinary
-0000a3c0: 2863 5f78 2c20 635f 792c 2072 6164 6975  (c_x, c_y, radiu
-0000a3d0: 732c 206c 5f63 2c20 725f 6329 0a0a 2020  s, l_c, r_c)..  
-0000a3e0: 2020 2020 2020 6966 2046 5320 6973 204e        if FS is N
-0000a3f0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000a400: 2072 6574 7572 6e20 4e6f 6e65 0a0a 2020   return None..  
-0000a410: 2020 2020 2020 7072 6576 5f46 5320 3d20        prev_FS = 
-0000a420: 4653 0a0a 2020 2020 2020 2020 2320 746f  FS..        # to
-0000a430: 7461 6c20 6e75 6d62 6572 206f 6620 736c  tal number of sl
-0000a440: 6963 6573 0a20 2020 2020 2020 2053 4c49  ices.        SLI
-0000a450: 4345 5320 3d20 7365 6c66 2e5f 736c 6963  CES = self._slic
-0000a460: 6573 0a0a 2020 2020 2020 2020 2320 686f  es..        # ho
-0000a470: 7269 7a6f 6e74 616c 2064 6973 7461 6e63  rizontal distanc
-0000a480: 6520 6265 7477 6565 6e20 6c65 6674 2061  e between left a
-0000a490: 6e64 2072 6967 6874 2073 6c69 6365 0a20  nd right slice. 
-0000a4a0: 2020 2020 2020 2064 6973 7420 3d20 695f         dist = i_
-0000a4b0: 6c69 7374 5b31 5d5b 305d 202d 2069 5f6c  list[1][0] - i_l
-0000a4c0: 6973 745b 305d 5b30 5d0a 0a20 2020 2020  ist[0][0]..     
-0000a4d0: 2020 2023 2077 6964 7468 206f 6620 6120     # width of a 
-0000a4e0: 736c 6963 650a 2020 2020 2020 2020 6220  slice.        b 
-0000a4f0: 3d20 6469 7374 202f 2053 4c49 4345 530a  = dist / SLICES.
-0000a500: 0a20 2020 2020 2020 2066 6f72 205f 2069  .        for _ i
-0000a510: 6e20 7261 6e67 6528 7365 6c66 2e5f 6d61  n range(self._ma
-0000a520: 785f 6974 6572 6174 696f 6e73 293a 0a20  x_iterations):. 
-0000a530: 2020 2020 2020 2020 2020 2023 2069 6e69             # ini
-0000a540: 7469 616c 6973 6520 6365 6e74 7265 2070  tialise centre p
-0000a550: 6f69 6e74 206f 6620 6669 7273 7420 736c  oint of first sl
-0000a560: 6963 650a 2020 2020 2020 2020 2020 2020  ice.            
-0000a570: 735f 7820 3d20 695f 6c69 7374 5b30 5d5b  s_x = i_list[0][
-0000a580: 305d 202b 2062 202f 2032 0a0a 2020 2020  0] + b / 2..    
-0000a590: 2020 2020 2020 2020 6966 2070 7265 765f          if prev_
-0000a5a0: 4653 2069 7320 4e6f 6e65 3a0a 2020 2020  FS is None:.    
-0000a5b0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000a5c0: 726e 204e 6f6e 650a 0a20 2020 2020 2020  rn None..       
-0000a5d0: 2020 2020 2023 2069 6e74 6961 6c69 7365       # intialise
-0000a5e0: 2074 6865 2070 7573 6820 616e 6420 7265   the push and re
-0000a5f0: 7369 7374 616e 6365 2063 6f6d 706f 6e65  sistance compone
-0000a600: 6e74 7320 666f 7220 464f 5320 6265 666f  nts for FOS befo
-0000a610: 7265 206c 6f6f 7069 6e67 0a20 2020 2020  re looping.     
-0000a620: 2020 2020 2020 2070 7573 6869 6e67 203d         pushing =
-0000a630: 2030 2e30 0a20 2020 2020 2020 2020 2020   0.0.           
-0000a640: 2072 6573 6973 7469 6e67 203d 2030 2e30   resisting = 0.0
-0000a650: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-0000a660: 6c6f 6f70 2074 6872 6f75 6768 2073 6c69  loop through sli
-0000a670: 6365 730a 2020 2020 2020 2020 2020 2020  ces.            
-0000a680: 666f 7220 5f20 696e 2072 616e 6765 2830  for _ in range(0
-0000a690: 2c20 534c 4943 4553 293a 0a20 2020 2020  , SLICES):.     
-0000a6a0: 2020 2020 2020 2020 2020 2023 2064 6566             # def
-0000a6b0: 696e 6520 7920 636f 6f72 6469 6e61 7465  ine y coordinate
-0000a6c0: 7320 666f 7220 736c 6963 6520 626f 7474  s for slice bott
-0000a6d0: 6f6d 0a0a 2020 2020 2020 2020 2020 2020  om..            
-0000a6e0: 2020 2020 2320 6966 2072 6164 6975 7320      # if radius 
-0000a6f0: 3c20 6162 7328 735f 7820 2d20 635f 7829  < abs(s_x - c_x)
-0000a700: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000a710: 2020 2320 2020 2020 7265 7475 726e 204e    #     return N
-0000a720: 6f6e 650a 0a20 2020 2020 2020 2020 2020  one..           
-0000a730: 2020 2020 2073 5f79 6220 3d20 635f 7920       s_yb = c_y 
-0000a740: 2d20 7371 7274 2872 6164 6975 732a 2a32  - sqrt(radius**2
-0000a750: 202d 2061 6273 2873 5f78 202d 2063 5f78   - abs(s_x - c_x
-0000a760: 2920 2a2a 2032 290a 0a20 2020 2020 2020  ) ** 2)..       
-0000a770: 2020 2020 2020 2020 2023 2067 6574 2079           # get y
-0000a780: 2063 6f6f 7264 696e 6174 6520 6174 2073   coordinate at s
-0000a790: 6c69 6365 2074 6f70 0a20 2020 2020 2020  lice top.       
-0000a7a0: 2020 2020 2020 2020 2073 5f79 7420 3d20           s_yt = 
-0000a7b0: 7365 6c66 2e67 6574 5f65 7874 6572 6e61  self.get_externa
-0000a7c0: 6c5f 795f 696e 7465 7273 6563 7469 6f6e  l_y_intersection
-0000a7d0: 2873 5f78 290a 0a20 2020 2020 2020 2020  (s_x)..         
-0000a7e0: 2020 2020 2020 2023 206f 7574 206f 6620         # out of 
-0000a7f0: 626f 756e 6473 0a20 2020 2020 2020 2020  bounds.         
-0000a800: 2020 2020 2020 2069 6620 735f 7974 2069         if s_yt i
-0000a810: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-0000a820: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000a830: 726e 204e 6f6e 650a 0a20 2020 2020 2020  rn None..       
-0000a840: 2020 2020 2020 2020 2023 2067 6574 2061           # get a
-0000a850: 6c70 6861 2c20 6479 2061 6c77 6179 7320  lpha, dy always 
-0000a860: 706f 7369 7469 7665 2c20 6478 206e 6567  positive, dx neg
-0000a870: 6174 6976 6520 746f 2072 6967 6874 2028  ative to right (
-0000a880: 7570 6869 6c6c 292c 2064 7820 706f 7369  uphill), dx posi
-0000a890: 7469 7665 2074 6f20 6c65 6674 0a20 2020  tive to left.   
-0000a8a0: 2020 2020 2020 2020 2020 2020 2023 206e               # n
-0000a8b0: 6f74 6520 616c 7068 6120 696e 2072 6164  ote alpha in rad
-0000a8c0: 6961 6e73 2062 7920 6465 6661 756c 740a  ians by default.
-0000a8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8e0: 6479 203d 2063 5f79 202d 2073 5f79 620a  dy = c_y - s_yb.
-0000a8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a900: 6478 203d 2063 5f78 202d 2073 5f78 0a20  dx = c_x - s_x. 
-0000a910: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0000a920: 6c70 6861 203d 2061 7461 6e28 6478 202f  lpha = atan(dx /
-0000a930: 2064 7929 0a0a 2020 2020 2020 2020 2020   dy)..          
-0000a940: 2020 2020 2020 2320 6765 7420 6c65 6e67        # get leng
-0000a950: 7468 0a20 2020 2020 2020 2020 2020 2020  th.             
-0000a960: 2020 2023 206c 203d 2062 202f 2063 6f73     # l = b / cos
-0000a970: 2861 6c70 6861 290a 0a20 2020 2020 2020  (alpha)..       
-0000a980: 2020 2020 2020 2020 2023 2063 616c 6375           # calcu
-0000a990: 6c61 7465 2073 7472 6970 2077 6569 6768  late strip weigh
-0000a9a0: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
-0000a9b0: 2020 5720 3d20 7365 6c66 2e5f 6361 6c63    W = self._calc
-0000a9c0: 756c 6174 655f 7374 7269 705f 7765 6967  ulate_strip_weig
-0000a9d0: 6874 2862 2c20 735f 7974 2c20 735f 7962  ht(b, s_yt, s_yb
-0000a9e0: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000a9f0: 2020 2023 2067 6574 206d 6174 6572 6961     # get materia
-0000aa00: 6c20 7072 6f70 6572 7469 6573 2061 7420  l properties at 
-0000aa10: 7468 6520 626f 7474 6f6d 206f 6620 7468  the bottom of th
-0000aa20: 6520 736c 6963 650a 2020 2020 2020 2020  e slice.        
-0000aa30: 2020 2020 2020 2020 626f 7474 6f6d 5f6d          bottom_m
-0000aa40: 6174 6572 6961 6c20 3d20 7365 6c66 2e5f  aterial = self._
-0000aa50: 6765 745f 6d61 7465 7269 616c 5f61 745f  get_material_at_
-0000aa60: 6465 7074 6828 735f 7962 290a 0a20 2020  depth(s_yb)..   
-0000aa70: 2020 2020 2020 2020 2020 2020 2063 6f68               coh
-0000aa80: 6573 696f 6e20 3d20 626f 7474 6f6d 5f6d  esion = bottom_m
-0000aa90: 6174 6572 6961 6c2e 636f 6865 7369 6f6e  aterial.cohesion
-0000aaa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000aab0: 2066 7269 6374 696f 6e5f 616e 676c 6520   friction_angle 
-0000aac0: 3d20 626f 7474 6f6d 5f6d 6174 6572 6961  = bottom_materia
-0000aad0: 6c2e 6672 6963 7469 6f6e 5f61 6e67 6c65  l.friction_angle
-0000aae0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000aaf0: 2020 2320 4143 434f 5244 494e 4720 544f    # ACCORDING TO
-0000ab00: 2047 454f 534c 4f50 4520 5348 4f55 4c44   GEOSLOPE SHOULD
-0000ab10: 2044 4f20 5448 4520 4348 4543 4b20 4245   DO THE CHECK BE
-0000ab20: 4c4f 572e 0a20 2020 2020 2020 2020 2020  LOW..           
-0000ab30: 2020 2020 2023 2054 4849 5320 484f 5745       # THIS HOWE
-0000ab40: 5645 5220 454c 494d 494e 4154 4553 2041  VER ELIMINATES A
-0000ab50: 4c4d 4f53 5420 414c 4c20 4f46 2054 4845  LMOST ALL OF THE
-0000ab60: 2050 524f 504f 5345 4420 534c 4f50 4553   PROPOSED SLOPES
-0000ab70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ab80: 2023 2053 4c49 4445 2044 4f45 534e 5420   # SLIDE DOESNT 
-0000ab90: 434f 4e53 4944 4552 2054 4849 532e 0a0a  CONSIDER THIS...
-0000aba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000abb0: 2320 6966 205f 203d 3d20 303a 0a20 2020  # if _ == 0:.   
-0000abc0: 2020 2020 2020 2020 2020 2020 2023 2020               #  
-0000abd0: 2020 2069 6620 616c 7068 6120 2a20 3138     if alpha * 18
-0000abe0: 3020 2f20 332e 3134 203e 2034 3520 2b20  0 / 3.14 > 45 + 
-0000abf0: 6672 6963 7469 6f6e 5f61 6e67 6c65 202f  friction_angle /
-0000ac00: 2032 3a0a 2020 2020 2020 2020 2020 2020   2:.            
-0000ac10: 2020 2020 2320 2020 2020 2020 2020 7265      #         re
-0000ac20: 7475 726e 204e 6f6e 650a 0a20 2020 2020  turn None..     
-0000ac30: 2020 2020 2020 2020 2020 2023 2069 6620             # if 
-0000ac40: 5f20 3d3d 2053 4c49 4345 5320 2d20 313a  _ == SLICES - 1:
-0000ac50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ac60: 2023 2020 2020 2069 6620 616c 7068 6120   #     if alpha 
-0000ac70: 2a20 3138 3020 2f20 332e 3134 203c 2034  * 180 / 3.14 < 4
-0000ac80: 3520 2d20 6672 6963 7469 6f6e 5f61 6e67  5 - friction_ang
-0000ac90: 6c65 2f32 3a0a 2020 2020 2020 2020 2020  le/2:.          
-0000aca0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-0000acb0: 7265 7475 726e 204e 6f6e 650a 0a20 2020  return None..   
-0000acc0: 2020 2020 2020 2020 2020 2020 2023 2069               # i
-0000acd0: 6620 7468 6572 6520 6973 2061 2075 646c  f there is a udl
-0000ace0: 206c 6f61 6420 6f6e 2074 6865 2073 7472   load on the str
-0000acf0: 6970 2061 7070 6c79 2069 742e 0a20 2020  ip apply it..   
-0000ad00: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000ad10: 2075 646c 2069 6e20 7365 6c66 2e5f 7564   udl in self._ud
-0000ad20: 6c73 3a0a 2020 2020 2020 2020 2020 2020  ls:.            
-0000ad30: 2020 2020 2020 2020 5720 2b3d 2073 656c          W += sel
-0000ad40: 662e 5f63 616c 6375 6c61 7465 5f73 7472  f._calculate_str
-0000ad50: 6970 5f75 646c 5f66 6f72 6365 2862 2c20  ip_udl_force(b, 
-0000ad60: 735f 782c 2075 646c 290a 0a20 2020 2020  s_x, udl)..     
-0000ad70: 2020 2020 2020 2020 2020 2023 2069 6620             # if 
-0000ad80: 7468 6572 6520 6973 2061 2070 6f69 6e74  there is a point
-0000ad90: 206c 6f61 6420 6f6e 2074 6865 2073 7472   load on the str
-0000ada0: 6970 2061 7070 6c79 2069 742e 0a20 2020  ip apply it..   
-0000adb0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000adc0: 206c 6c20 696e 2073 656c 662e 5f6c 6c73   ll in self._lls
-0000add0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000ade0: 2020 2020 2020 5720 2b3d 2073 656c 662e        W += self.
-0000adf0: 5f63 616c 6375 6c61 7465 5f73 7472 6970  _calculate_strip
-0000ae00: 5f6c 6c28 622c 2073 5f78 2c20 6c6c 290a  _ll(b, s_x, ll).
-0000ae10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ae20: 2023 2063 6f6e 7369 6465 7261 7469 6f6e   # consideration
-0000ae30: 2066 6f72 2077 6174 6572 0a20 2020 2020   for water.     
-0000ae40: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000ae50: 6c66 2e5f 7761 7465 725f 524c 3a0a 2020  lf._water_RL:.  
-0000ae60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae70: 2020 2320 6465 7465 726d 696e 6520 4820    # determine H 
-0000ae80: 6661 6374 6f72 2062 6173 6564 206f 6e20  factor based on 
-0000ae90: 7365 7474 696e 670a 2020 2020 2020 2020  setting.        
-0000aea0: 2020 2020 2020 2020 2020 2020 2320 6874              # ht
-0000aeb0: 7470 733a 2f2f 7777 772e 726f 6373 6369  tps://www.rocsci
-0000aec0: 656e 6365 2e63 6f6d 2f68 656c 702f 736c  ence.com/help/sl
-0000aed0: 6964 6532 2f64 6f63 756d 656e 7461 7469  ide2/documentati
-0000aee0: 6f6e 2f73 6c69 6465 2d6d 6f64 656c 2f6d  on/slide-model/m
-0000aef0: 6174 6572 6961 6c2d 7072 6f70 6572 7469  aterial-properti
-0000af00: 6573 2f64 6566 696e 652d 6d61 7465 7269  es/define-materi
-0000af10: 616c 2d70 726f 7065 7274 6965 732f 7761  al-properties/wa
-0000af20: 7465 722d 7061 7261 6d65 7465 7273 0a0a  ter-parameters..
-0000af30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af40: 2020 2020 2320 6f6e 6c79 2075 7365 2048      # only use H
-0000af50: 2066 6163 746f 7220 6966 206f 6e20 7468   factor if on th
-0000af60: 6520 736c 6f70 652c 206f 7468 6572 7769  e slope, otherwi
-0000af70: 7365 2075 7365 2031 0a20 2020 2020 2020  se use 1.       
-0000af80: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000af90: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000afa0: 2020 2020 2020 2020 2020 7365 6c66 2e67            self.g
-0000afb0: 6574 5f65 7874 6572 6e61 6c5f 785f 696e  et_external_x_in
-0000afc0: 7465 7273 6563 7469 6f6e 2873 656c 662e  tersection(self.
-0000afd0: 5f77 6174 6572 5f52 4c29 0a20 2020 2020  _water_RL).     
-0000afe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aff0: 2020 203c 2073 5f78 0a20 2020 2020 2020     < s_x.       
-0000b000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b010: 203c 2073 656c 662e 5f62 6f74 5f63 6f6f   < self._bot_coo
-0000b020: 7264 5b30 5d0a 2020 2020 2020 2020 2020  rd[0].          
-0000b030: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
-0000b040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b050: 2020 2020 2055 203d 2028 0a20 2020 2020       U = (.     
-0000b060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b070: 2020 2020 2020 206d 6178 286d 696e 2873         max(min(s
-0000b080: 656c 662e 5f77 6174 6572 5f52 4c2c 2073  elf._water_RL, s
-0000b090: 5f79 7429 202d 2073 5f79 622c 2030 290a  _yt) - s_yb, 0).
-0000b0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b0b0: 2020 2020 2020 2020 2020 2020 2a20 392e              * 9.
-0000b0c0: 3831 0a20 2020 2020 2020 2020 2020 2020  81.             
-0000b0d0: 2020 2020 2020 2020 2020 2020 2020 202a                 *
-0000b0e0: 2062 0a20 2020 2020 2020 2020 2020 2020   b.             
-0000b0f0: 2020 2020 2020 2020 2020 2020 2020 202a                 *
-0000b100: 2073 656c 662e 5f77 6174 6572 5f61 6e61   self._water_ana
-0000b110: 6c79 7369 735f 480a 2020 2020 2020 2020  lysis_H.        
-0000b120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b130: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000b140: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000b150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b160: 2020 2020 5520 3d20 6d61 7828 6d69 6e28      U = max(min(
-0000b170: 7365 6c66 2e5f 7761 7465 725f 524c 2c20  self._water_RL, 
-0000b180: 735f 7974 2920 2d20 735f 7962 2c20 3029  s_yt) - s_yb, 0)
-0000b190: 202a 2039 2e38 3120 2a20 6220 2a20 310a   * 9.81 * b * 1.
-0000b1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1b0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000b1c0: 2020 2020 2020 2020 2020 5520 3d20 300a            U = 0.
-0000b1d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b1e0: 2023 2063 616c 6375 6c61 7465 206d 610a   # calculate ma.
-0000b1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b200: 6d61 203d 2063 6f73 2861 6c70 6861 2920  ma = cos(alpha) 
-0000b210: 2b20 7369 6e28 616c 7068 6129 202a 2074  + sin(alpha) * t
-0000b220: 616e 2872 6164 6961 6e73 2866 7269 6374  an(radians(frict
-0000b230: 696f 6e5f 616e 676c 6529 2920 2f20 7072  ion_angle)) / pr
-0000b240: 6576 5f46 530a 0a20 2020 2020 2020 2020  ev_FS..         
-0000b250: 2020 2020 2020 2023 2063 616c 6375 6c61         # calcula
-0000b260: 7465 2072 6573 6973 7469 6e67 0a20 2020  te resisting.   
-0000b270: 2020 2020 2020 2020 2020 2020 2072 6573               res
-0000b280: 6973 7469 6e67 202b 3d20 280a 2020 2020  isting += (.    
-0000b290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b2a0: 636f 6865 7369 6f6e 202a 2062 202b 2028  cohesion * b + (
-0000b2b0: 5720 2d20 5529 202a 2074 616e 2872 6164  W - U) * tan(rad
-0000b2c0: 6961 6e73 2866 7269 6374 696f 6e5f 616e  ians(friction_an
-0000b2d0: 676c 6529 290a 2020 2020 2020 2020 2020  gle)).          
-0000b2e0: 2020 2020 2020 2920 2f20 6d61 0a0a 2020        ) / ma..  
-0000b2f0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000b300: 6361 6c63 756c 6174 6520 7075 7368 696e  calculate pushin
-0000b310: 670a 2020 2020 2020 2020 2020 2020 2020  g.              
-0000b320: 2020 7075 7368 696e 6720 2b3d 2057 202a    pushing += W *
-0000b330: 2073 696e 2861 6c70 6861 290a 0a20 2020   sin(alpha)..   
-0000b340: 2020 2020 2020 2020 2020 2020 2023 2069               # i
-0000b350: 6e69 7469 616c 6973 6520 736c 6963 6520  nitialise slice 
-0000b360: 7820 636f 6f72 6469 6e61 7465 2066 6f72  x coordinate for
-0000b370: 206e 6578 7420 6c6f 6f70 0a20 2020 2020   next loop.     
-0000b380: 2020 2020 2020 2020 2020 2073 5f78 203d             s_x =
-0000b390: 2073 5f78 202b 2062 0a0a 2020 2020 2020   s_x + b..      
-0000b3a0: 2020 2020 2020 6966 2070 7573 6869 6e67        if pushing
-0000b3b0: 203c 3d20 303a 0a20 2020 2020 2020 2020   <= 0:.         
-0000b3c0: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
-0000b3d0: 6e65 0a20 2020 2020 2020 2020 2020 2069  ne.            i
-0000b3e0: 6620 7265 7369 7374 696e 6720 3c20 3020  f resisting < 0 
-0000b3f0: 6f72 2070 7573 6869 6e67 203c 2030 3a0a  or pushing < 0:.
-0000b400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b410: 7265 7475 726e 204e 6f6e 650a 0a20 2020  return None..   
-0000b420: 2020 2020 2020 2020 2046 5320 3d20 7265           FS = re
-0000b430: 7369 7374 696e 6720 2f20 7075 7368 696e  sisting / pushin
-0000b440: 670a 2020 2020 2020 2020 2020 2020 6966  g.            if
-0000b450: 2061 6273 2870 7265 765f 4653 202d 2046   abs(prev_FS - F
-0000b460: 5329 203c 2073 656c 662e 5f74 6f6c 6572  S) < self._toler
-0000b470: 616e 6365 3a0a 2020 2020 2020 2020 2020  ance:.          
-0000b480: 2020 2020 2020 7265 7475 726e 2046 530a        return FS.
-0000b490: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0000b4a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000b4b0: 2020 7072 6576 5f46 5320 3d20 4653 0a0a    prev_FS = FS..
-0000b4c0: 2020 2020 2020 2020 7265 7475 726e 2070          return p
-0000b4d0: 7265 765f 4653 0a0a 2020 2020 6465 6620  rev_FS..    def 
-0000b4e0: 616e 616c 7973 655f 6479 6e61 6d69 6328  analyse_dynamic(
-0000b4f0: 7365 6c66 2c20 6372 6974 6963 616c 5f66  self, critical_f
-0000b500: 6f73 3d31 2e33 293a 0a20 2020 2020 2020  os=1.3):.       
-0000b510: 2022 2222 416e 616c 7973 6520 736c 6f70   """Analyse slop
-0000b520: 6520 616e 6420 6f66 6673 6574 2064 796e  e and offset dyn
-0000b530: 616d 6963 206c 6f61 6473 2075 6e74 696c  amic loads until
-0000b540: 2063 7269 7469 6361 6c20 464f 5320 6973   critical FOS is
-0000b550: 2061 6368 6965 7665 640a 0a20 2020 2020   achieved..     
-0000b560: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-0000b570: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-0000b580: 0a20 2020 2020 2020 2063 7269 7469 6361  .        critica
-0000b590: 6c5f 666f 7320 3a20 666c 6f61 742c 206f  l_fos : float, o
-0000b5a0: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-0000b5b0: 2020 2020 6d69 6e69 6d75 6d20 7265 7175      minimum requ
-0000b5c0: 6972 6564 2066 6163 746f 7220 6f66 2073  ired factor of s
-0000b5d0: 6166 6574 792c 2062 7920 6465 6661 756c  afety, by defaul
-0000b5e0: 7420 312e 330a 2020 2020 2020 2020 2222  t 1.3.        ""
-0000b5f0: 220a 2020 2020 2020 2020 7365 6c66 2e5f  ".        self._
-0000b600: 6479 6e61 6d69 635f 7265 7375 6c74 7320  dynamic_results 
-0000b610: 3d20 7b7d 0a0a 2020 2020 2020 2020 2320  = {}..        # 
-0000b620: 6368 6563 6b20 6361 7365 2066 6f72 206c  check case for l
-0000b630: 6f61 6420 6174 2072 6967 6874 2061 6e64  oad at right and
-0000b640: 206c 6f61 6420 6174 206c 6566 7420 6265   load at left be
-0000b650: 666f 7265 0a20 2020 2020 2020 2023 2074  fore.        # t
-0000b660: 7279 696e 6720 746f 2063 6f6e 7665 7267  rying to converg
-0000b670: 6520 6f6e 2070 6f73 6974 696f 6e0a 2020  e on position.  
-0000b680: 2020 2020 2020 7269 6768 7420 3d20 302e        right = 0.
-0000b690: 300a 2020 2020 2020 2020 6c65 6674 203d  0.        left =
-0000b6a0: 2073 656c 662e 5f6c 656e 6774 6820 2d20   self._length - 
-0000b6b0: 302e 3031 0a0a 2020 2020 2020 2020 2320  0.01..        # 
-0000b6c0: 6368 6563 6b20 666f 7220 6578 7472 656d  check for extrem
-0000b6d0: 6520 6361 7365 2077 6974 6820 6c6f 6164  e case with load
-0000b6e0: 7320 6174 2063 7265 7374 2028 7269 6768  s at crest (righ
-0000b6f0: 7429 0a20 2020 2020 2020 2023 2069 6620  t).        # if 
-0000b700: 736c 6f70 6520 6973 2073 6166 6520 2846  slope is safe (F
-0000b710: 4f53 2068 6967 6829 2074 6865 6e20 7265  OS high) then re
-0000b720: 7475 726e 0a20 2020 2020 2020 2073 656c  turn.        sel
-0000b730: 662e 5f73 6574 5f64 796e 616d 6963 5f6f  f._set_dynamic_o
-0000b740: 6666 7365 7428 7269 6768 7429 0a20 2020  ffset(right).   
-0000b750: 2020 2020 2073 656c 662e 616e 616c 7973       self.analys
-0000b760: 655f 736c 6f70 6528 290a 2020 2020 2020  e_slope().      
-0000b770: 2020 666f 7320 3d20 7365 6c66 2e67 6574    fos = self.get
-0000b780: 5f6d 696e 5f46 4f53 2829 0a20 2020 2020  _min_FOS().     
-0000b790: 2020 2073 656c 662e 5f64 796e 616d 6963     self._dynamic
-0000b7a0: 5f72 6573 756c 7473 5b72 6967 6874 5d20  _results[right] 
-0000b7b0: 3d20 666f 730a 2020 2020 2020 2020 6966  = fos.        if
-0000b7c0: 2066 6f73 203e 2063 7269 7469 6361 6c5f   fos > critical_
-0000b7d0: 666f 733a 0a20 2020 2020 2020 2020 2020  fos:.           
-0000b7e0: 2072 6574 7572 6e20 300a 0a20 2020 2020   return 0..     
-0000b7f0: 2020 2023 2063 6865 636b 2066 6f72 2065     # check for e
-0000b800: 7874 7265 6d65 2063 6173 6520 7769 7468  xtreme case with
-0000b810: 206c 6f61 6473 2061 7420 656e 6420 6f66   loads at end of
-0000b820: 2073 6c6f 7065 2061 7320 6661 7220 6177   slope as far aw
-0000b830: 6179 2066 726f 6d20 6372 6573 7420 286c  ay from crest (l
-0000b840: 6566 7429 0a20 2020 2020 2020 2023 2049  eft).        # I
-0000b850: 6620 736c 6f70 6520 6973 2075 6e73 6166  f slope is unsaf
-0000b860: 6520 2846 4f53 2073 7469 6c6c 206c 6f77  e (FOS still low
-0000b870: 2920 7468 656e 2072 6574 7572 6e0a 2020  ) then return.  
-0000b880: 2020 2020 2020 7365 6c66 2e5f 7365 745f        self._set_
-0000b890: 6479 6e61 6d69 635f 6f66 6673 6574 286c  dynamic_offset(l
-0000b8a0: 6566 7429 0a20 2020 2020 2020 2073 656c  eft).        sel
-0000b8b0: 662e 616e 616c 7973 655f 736c 6f70 6528  f.analyse_slope(
-0000b8c0: 290a 2020 2020 2020 2020 666f 7320 3d20  ).        fos = 
-0000b8d0: 7365 6c66 2e67 6574 5f6d 696e 5f46 4f53  self.get_min_FOS
-0000b8e0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-0000b8f0: 5f64 796e 616d 6963 5f72 6573 756c 7473  _dynamic_results
-0000b900: 5b6c 6566 745d 203d 2066 6f73 0a20 2020  [left] = fos.   
-0000b910: 2020 2020 2069 6620 666f 7320 3c20 6372       if fos < cr
-0000b920: 6974 6963 616c 5f66 6f73 3a0a 2020 2020  itical_fos:.    
-0000b930: 2020 2020 2020 2020 7265 7475 726e 2031          return 1
-0000b940: 0a0a 2020 2020 2020 2020 2320 4966 206e  ..        # If n
-0000b950: 6569 7468 6572 206f 6620 7468 6520 7072  either of the pr
-0000b960: 6576 696f 7573 2072 6573 756c 7473 2077  evious results w
-0000b970: 6173 2074 7275 6520 6669 6e64 2074 6865  as true find the
-0000b980: 2069 6e74 6572 6d65 6469 6174 6520 706f   intermediate po
-0000b990: 696e 740a 2020 2020 2020 2020 2320 7768  int.        # wh
-0000b9a0: 6572 6520 7468 6520 6372 6974 6963 616c  ere the critical
-0000b9b0: 2046 4f53 2069 7320 7265 6163 6865 640a   FOS is reached.
-0000b9c0: 2020 2020 2020 2020 2320 6f66 6673 6574          # offset
-0000b9d0: 2066 6f72 206c 6566 7420 7368 6f75 6c64   for left should
-0000b9e0: 6e74 2062 6520 6d6f 7265 2074 6865 6e20  nt be more then 
-0000b9f0: 7468 6520 706f 696e 7420 7468 6174 2074  the point that t
-0000ba00: 6865 2073 6c6f 7065 2073 7461 7274 6564  he slope started
-0000ba10: 2066 6169 6c69 6e67 2066 726f 6d0a 2020   failing from.  
-0000ba20: 2020 2020 2020 2320 696e 2074 6865 2077        # in the w
-0000ba30: 6f72 7365 2063 6173 650a 2020 2020 2020  orse case.      
-0000ba40: 2020 2320 6c65 6674 203d 2073 656c 662e    # left = self.
-0000ba50: 6765 745f 6d69 6e5f 464f 535f 656e 645f  get_min_FOS_end_
-0000ba60: 706f 696e 7473 2829 5b30 5d5b 305d 0a0a  points()[0][0]..
-0000ba70: 2020 2020 2020 2020 7072 6576 696f 7573          previous
-0000ba80: 5f66 6f73 203d 2030 0a0a 2020 2020 2020  _fos = 0..      
-0000ba90: 2020 2320 636f 6e76 6572 6765 0a20 2020    # converge.   
-0000baa0: 2020 2020 2066 6f72 205f 2069 6e20 7261       for _ in ra
-0000bab0: 6e67 6528 3130 293a 0a20 2020 2020 2020  nge(10):.       
-0000bac0: 2020 2020 2023 2023 2063 6865 636b 206d       # # check m
-0000bad0: 6964 706f 696e 7420 666f 7220 464f 530a  idpoint for FOS.
-0000bae0: 2020 2020 2020 2020 2020 2020 2320 6d69              # mi
-0000baf0: 6470 6f69 6e74 203d 2028 6c65 6674 202b  dpoint = (left +
-0000bb00: 2072 6967 6874 2920 2f20 320a 0a20 2020   right) / 2..   
-0000bb10: 2020 2020 2020 2020 2023 206c 6574 206d           # let m
-0000bb20: 6964 706f 696e 7420 6265 2077 6569 6768  idpoint be weigh
-0000bb30: 7465 6420 7661 6c75 6520 6261 7365 6420  ted value based 
-0000bb40: 6f6e 2046 4f53 0a20 2020 2020 2020 2020  on FOS.         
-0000bb50: 2020 206c 6566 745f 666f 7320 3d20 7365     left_fos = se
-0000bb60: 6c66 2e5f 6479 6e61 6d69 635f 7265 7375  lf._dynamic_resu
-0000bb70: 6c74 735b 6c65 6674 5d0a 2020 2020 2020  lts[left].      
-0000bb80: 2020 2020 2020 7269 6768 745f 666f 7320        right_fos 
-0000bb90: 3d20 7365 6c66 2e5f 6479 6e61 6d69 635f  = self._dynamic_
-0000bba0: 7265 7375 6c74 735b 7269 6768 745d 0a0a  results[right]..
-0000bbb0: 2020 2020 2020 2020 2020 2020 6d20 3d20              m = 
-0000bbc0: 286c 6566 745f 666f 7320 2d20 7269 6768  (left_fos - righ
-0000bbd0: 745f 666f 7329 202f 2028 6c65 6674 202d  t_fos) / (left -
-0000bbe0: 2072 6967 6874 290a 2020 2020 2020 2020   right).        
-0000bbf0: 2020 2020 6d69 6470 6f69 6e74 203d 2072      midpoint = r
-0000bc00: 6967 6874 202b 2028 6372 6974 6963 616c  ight + (critical
-0000bc10: 5f66 6f73 202d 2072 6967 6874 5f66 6f73  _fos - right_fos
-0000bc20: 2920 2f20 6d0a 0a20 2020 2020 2020 2020  ) / m..         
-0000bc30: 2020 2073 656c 662e 5f73 6574 5f64 796e     self._set_dyn
-0000bc40: 616d 6963 5f6f 6666 7365 7428 6d69 6470  amic_offset(midp
-0000bc50: 6f69 6e74 290a 2020 2020 2020 2020 2020  oint).          
-0000bc60: 2020 7365 6c66 2e61 6e61 6c79 7365 5f73    self.analyse_s
-0000bc70: 6c6f 7065 2829 0a20 2020 2020 2020 2020  lope().         
-0000bc80: 2020 2066 6f73 203d 2073 656c 662e 6765     fos = self.ge
-0000bc90: 745f 6d69 6e5f 464f 5328 290a 2020 2020  t_min_FOS().    
-0000bca0: 2020 2020 2020 2020 7365 6c66 2e5f 6479          self._dy
-0000bcb0: 6e61 6d69 635f 7265 7375 6c74 735b 6d69  namic_results[mi
-0000bcc0: 6470 6f69 6e74 5d20 3d20 666f 730a 0a20  dpoint] = fos.. 
-0000bcd0: 2020 2020 2020 2020 2020 2023 2063 6865             # che
-0000bce0: 636b 2069 6620 6c6f 6164 2069 7320 7769  ck if load is wi
-0000bcf0: 7468 696e 2074 6865 207a 6f6e 6520 6f66  thin the zone of
-0000bd00: 2069 6e66 6c75 656e 6365 2c20 6966 206c   influence, if l
-0000bd10: 6173 7420 7477 6f20 464f 5320 6172 6520  ast two FOS are 
-0000bd20: 6964 656e 7469 6361 6c0a 2020 2020 2020  identical.      
-0000bd30: 2020 2020 2020 2320 7468 656e 2070 726f        # then pro
-0000bd40: 6261 626c 7920 6e6f 740a 2020 2020 2020  bably not.      
-0000bd50: 2020 2020 2020 6966 2070 7265 7669 6f75        if previou
-0000bd60: 735f 666f 7320 213d 2066 6f73 3a0a 2020  s_fos != fos:.  
-0000bd70: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000bd80: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
-0000bd90: 2020 2020 2020 2061 6273 2870 7265 7669         abs(previ
-0000bda0: 6f75 735f 666f 7320 2d20 666f 7329 203c  ous_fos - fos) <
-0000bdb0: 3d20 302e 3031 206f 7220 6162 7328 666f  = 0.01 or abs(fo
-0000bdc0: 7320 2d20 6372 6974 6963 616c 5f66 6f73  s - critical_fos
-0000bdd0: 2920 3c3d 2030 2e30 310a 2020 2020 2020  ) <= 0.01.      
-0000bde0: 2020 2020 2020 2020 2020 2920 616e 6420            ) and 
-0000bdf0: 726f 756e 6428 666f 732c 2033 2920 3e3d  round(fos, 3) >=
-0000be00: 2063 7269 7469 6361 6c5f 666f 733a 0a20   critical_fos:. 
-0000be10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be20: 2020 2062 7265 616b 0a0a 2020 2020 2020     break..      
-0000be30: 2020 2020 2020 2320 4966 2046 4f53 2068        # If FOS h
-0000be40: 6967 6820 7468 656e 206d 6f76 6520 636c  igh then move cl
-0000be50: 6f73 6572 2074 6f20 636c 6966 660a 2020  oser to cliff.  
-0000be60: 2020 2020 2020 2020 2020 6966 2066 6f73            if fos
-0000be70: 203c 2063 7269 7469 6361 6c5f 666f 733a   < critical_fos:
-0000be80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000be90: 2072 6967 6874 203d 206d 6964 706f 696e   right = midpoin
-0000bea0: 740a 2020 2020 2020 2020 2020 2020 656c  t.            el
-0000beb0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000bec0: 2020 2020 6c65 6674 203d 206d 6964 706f      left = midpo
-0000bed0: 696e 740a 0a20 2020 2020 2020 2020 2020  int..           
-0000bee0: 2070 7265 7669 6f75 735f 666f 7320 3d20   previous_fos = 
-0000bef0: 666f 730a 0a20 2020 2020 2020 2073 656c  fos..        sel
-0000bf00: 662e 5f64 796e 616d 6963 5f72 6573 756c  f._dynamic_resul
-0000bf10: 7473 203d 2064 6963 7428 0a20 2020 2020  ts = dict(.     
-0000bf20: 2020 2020 2020 2073 6f72 7465 6428 7365         sorted(se
-0000bf30: 6c66 2e5f 6479 6e61 6d69 635f 7265 7375  lf._dynamic_resu
-0000bf40: 6c74 732e 6974 656d 7328 292c 206b 6579  lts.items(), key
-0000bf50: 3d6c 616d 6264 6120 6974 656d 3a20 6974  =lambda item: it
-0000bf60: 656d 5b31 5d29 0a20 2020 2020 2020 2029  em[1]).        )
-0000bf70: 0a0a 2020 2020 6465 6620 5f73 6574 5f64  ..    def _set_d
-0000bf80: 796e 616d 6963 5f6f 6666 7365 7428 7365  ynamic_offset(se
-0000bf90: 6c66 2c20 6f66 6673 6574 293a 0a20 2020  lf, offset):.   
-0000bfa0: 2020 2020 2023 2072 656d 656d 6265 7220       # remember 
-0000bfb0: 6465 6661 756c 7420 7661 6c75 6573 3f0a  default values?.
-0000bfc0: 2020 2020 2020 2020 7564 6c73 203d 2073          udls = s
-0000bfd0: 656c 662e 5f75 646c 730a 2020 2020 2020  elf._udls.      
-0000bfe0: 2020 6c6c 7320 3d20 7365 6c66 2e5f 6c6c    lls = self._ll
-0000bff0: 730a 0a20 2020 2020 2020 2023 2072 656d  s..        # rem
-0000c000: 6f76 6520 6c6f 6164 730a 2020 2020 2020  ove loads.      
-0000c010: 2020 7365 6c66 2e72 656d 6f76 655f 7564    self.remove_ud
-0000c020: 6c73 2872 656d 6f76 655f 616c 6c3d 5472  ls(remove_all=Tr
-0000c030: 7565 290a 2020 2020 2020 2020 7365 6c66  ue).        self
-0000c040: 2e72 656d 6f76 655f 6c6c 7328 7265 6d6f  .remove_lls(remo
-0000c050: 7665 5f61 6c6c 3d54 7275 6529 0a0a 2020  ve_all=True)..  
-0000c060: 2020 2020 2020 2320 7570 6461 7465 206c        # update l
-0000c070: 6f61 6473 0a20 2020 2020 2020 2066 6f72  oads.        for
-0000c080: 2075 646c 2069 6e20 7564 6c73 3a0a 2020   udl in udls:.  
-0000c090: 2020 2020 2020 2020 2020 6966 2075 646c            if udl
-0000c0a0: 2e64 796e 616d 6963 5f6f 6666 7365 743a  .dynamic_offset:
-0000c0b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c0c0: 2075 646c 2e6f 6666 7365 7420 3d20 6f66   udl.offset = of
-0000c0d0: 6673 6574 0a20 2020 2020 2020 2020 2020  fset.           
-0000c0e0: 2073 656c 662e 7365 745f 7564 6c73 2875   self.set_udls(u
-0000c0f0: 646c 290a 0a20 2020 2020 2020 2066 6f72  dl)..        for
-0000c100: 206c 6c20 696e 206c 6c73 3a0a 2020 2020   ll in lls:.    
-0000c110: 2020 2020 2020 2020 6966 206c 6c2e 6479          if ll.dy
-0000c120: 6e61 6d69 635f 6f66 6673 6574 3a0a 2020  namic_offset:.  
-0000c130: 2020 2020 2020 2020 2020 2020 2020 6c6c                ll
-0000c140: 2e6f 6666 7365 7420 3d20 6f66 6673 6574  .offset = offset
-0000c150: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000c160: 662e 7365 745f 6c6c 7328 6c6c 290a 0a20  f.set_lls(ll).. 
-0000c170: 2020 2064 6566 205f 6765 745f 6369 7263     def _get_circ
-0000c180: 6c65 5f65 7874 6572 6e61 6c5f 696e 7465  le_external_inte
-0000c190: 7273 6563 7469 6f6e 2873 656c 662c 2063  rsection(self, c
-0000c1a0: 5f78 3a20 666c 6f61 742c 2063 5f79 3a20  _x: float, c_y: 
-0000c1b0: 666c 6f61 742c 2072 6164 6975 733a 2066  float, radius: f
-0000c1c0: 6c6f 6174 293a 0a20 2020 2020 2020 2022  loat):.        "
-0000c1d0: 2222 4765 7420 696e 7465 7273 6563 7469  ""Get intersecti
-0000c1e0: 6f6e 2070 6f69 6e74 7320 6f66 2061 2063  on points of a c
-0000c1f0: 6972 636c 6520 7769 7468 2065 7874 6572  ircle with exter
-0000c200: 6e61 6c20 626f 756e 6461 7279 0a0a 2020  nal boundary..  
-0000c210: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-0000c220: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-0000c230: 2d2d 2d0a 2020 2020 2020 2020 635f 7820  ---.        c_x 
-0000c240: 3a20 666c 6f61 740a 2020 2020 2020 2020  : float.        
-0000c250: 2020 2020 6369 7263 6c65 2078 2063 6f6f      circle x coo
-0000c260: 6469 6e61 7465 0a20 2020 2020 2020 2063  dinate.        c
-0000c270: 5f79 203a 2066 6c6f 6174 0a20 2020 2020  _y : float.     
-0000c280: 2020 2020 2020 2063 6972 636c 6520 7920         circle y 
-0000c290: 636f 6f72 6469 6e61 7465 0a20 2020 2020  coordinate.     
-0000c2a0: 2020 2072 6164 6975 7320 3a20 666c 6f61     radius : floa
-0000c2b0: 740a 2020 2020 2020 2020 2020 2020 6369  t.            ci
-0000c2c0: 7263 6c65 2072 6164 6975 730a 0a20 2020  rcle radius..   
-0000c2d0: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
-0000c2e0: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
-0000c2f0: 2020 2020 2074 7570 6c65 0a20 2020 2020       tuple.     
-0000c300: 2020 2020 2020 2074 7570 6c65 206f 6620         tuple of 
-0000c310: 7477 6f20 636f 6f72 6469 6e61 7465 7320  two coordinates 
-0000c320: 286c 6566 7420 636f 6f72 6469 6e61 7465  (left coordinate
-0000c330: 2c20 7269 6768 7420 636f 6f72 6469 6e61  , right coordina
-0000c340: 7465 290a 2020 2020 2020 2020 2222 220a  te).        """.
-0000c350: 0a20 2020 2020 2020 2069 5f6c 6973 7420  .        i_list 
-0000c360: 3d20 5b5d 0a0a 2020 2020 2020 2020 746f  = []..        to
-0000c370: 705f 696e 7465 7273 6563 7469 6f6e 203d  p_intersection =
-0000c380: 2075 7469 6c69 7469 6573 2e63 6972 6c65   utilities.cirle
-0000c390: 5f6c 696e 655f 696e 7465 7273 6563 7469  _line_intersecti
-0000c3a0: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
-0000c3b0: 2830 2c20 7365 6c66 2e5f 746f 705f 636f  (0, self._top_co
-0000c3c0: 6f72 645b 315d 292c 2073 656c 662e 5f74  ord[1]), self._t
-0000c3d0: 6f70 5f63 6f6f 7264 2c20 635f 782c 2063  op_coord, c_x, c
-0000c3e0: 5f79 2c20 7261 6469 7573 0a20 2020 2020  _y, radius.     
-0000c3f0: 2020 2029 0a0a 2020 2020 2020 2020 2320     )..        # 
-0000c400: 6f6e 6c79 2063 6172 6520 6162 6f75 7420  only care about 
-0000c410: 6c65 6674 206f 6620 6369 7263 6c65 2066  left of circle f
-0000c420: 6f72 2074 6f70 2069 6e74 6572 7365 6374  or top intersect
-0000c430: 696f 6e0a 2020 2020 2020 2020 2320 7369  ion.        # si
-0000c440: 6e63 6520 6661 696c 7572 6520 6672 6f6d  nce failure from
-0000c450: 206c 6566 7420 746f 2072 6967 6874 2061   left to right a
-0000c460: 6c77 6179 730a 2020 2020 2020 2020 6966  lways.        if
-0000c470: 2074 6f70 5f69 6e74 6572 7365 6374 696f   top_intersectio
-0000c480: 6e3a 0a20 2020 2020 2020 2020 2020 2074  n:.            t
-0000c490: 6f70 5f69 6e74 6572 7365 6374 696f 6e2e  op_intersection.
-0000c4a0: 736f 7274 2829 0a20 2020 2020 2020 2020  sort().         
-0000c4b0: 2020 2074 6f70 5f69 6e74 6572 7365 6374     top_intersect
-0000c4c0: 696f 6e20 3d20 746f 705f 696e 7465 7273  ion = top_inters
-0000c4d0: 6563 7469 6f6e 5b30 5d0a 2020 2020 2020  ection[0].      
-0000c4e0: 2020 2020 2020 6966 2074 6f70 5f69 6e74        if top_int
-0000c4f0: 6572 7365 6374 696f 6e5b 305d 203e 3d20  ersection[0] >= 
-0000c500: 3020 616e 6420 746f 705f 696e 7465 7273  0 and top_inters
-0000c510: 6563 7469 6f6e 5b30 5d20 3c3d 2073 656c  ection[0] <= sel
-0000c520: 662e 5f74 6f70 5f63 6f6f 7264 5b30 5d3a  f._top_coord[0]:
-0000c530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c540: 2069 5f6c 6973 742e 6170 7065 6e64 2874   i_list.append(t
-0000c550: 6f70 5f69 6e74 6572 7365 6374 696f 6e29  op_intersection)
-0000c560: 0a0a 2020 2020 2020 2020 626f 745f 696e  ..        bot_in
-0000c570: 7465 7273 6563 7469 6f6e 203d 2075 7469  tersection = uti
-0000c580: 6c69 7469 6573 2e63 6972 6c65 5f6c 696e  lities.cirle_lin
-0000c590: 655f 696e 7465 7273 6563 7469 6f6e 280a  e_intersection(.
-0000c5a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000c5b0: 2e5f 626f 745f 636f 6f72 642c 0a20 2020  ._bot_coord,.   
-0000c5c0: 2020 2020 2020 2020 2028 7365 6c66 2e5f           (self._
-0000c5d0: 6578 7465 726e 616c 5f6c 656e 6774 682c  external_length,
-0000c5e0: 2073 656c 662e 5f62 6f74 5f63 6f6f 7264   self._bot_coord
-0000c5f0: 5b31 5d29 2c0a 2020 2020 2020 2020 2020  [1]),.          
-0000c600: 2020 635f 782c 0a20 2020 2020 2020 2020    c_x,.         
-0000c610: 2020 2063 5f79 2c0a 2020 2020 2020 2020     c_y,.        
-0000c620: 2020 2020 7261 6469 7573 2c0a 2020 2020      radius,.    
-0000c630: 2020 2020 290a 0a20 2020 2020 2020 2023      )..        #
-0000c640: 206f 6e6c 7920 6361 7265 2061 626f 7574   only care about
-0000c650: 2072 6967 6874 206f 6620 6369 7263 6c65   right of circle
-0000c660: 2066 6f72 2062 6f74 746f 6d20 696e 7465   for bottom inte
-0000c670: 7273 6563 7469 6f6e 0a20 2020 2020 2020  rsection.       
-0000c680: 2023 2073 696e 6365 2066 6169 6c75 7265   # since failure
-0000c690: 2077 696c 6c20 616c 7761 7973 2062 6520   will always be 
-0000c6a0: 746f 2072 6967 6874 206f 6620 6369 726c  to right of cirl
-0000c6b0: 6520 6f6e 2062 6f74 746f 6d0a 2020 2020  e on bottom.    
-0000c6c0: 2020 2020 2320 756e 6c65 7373 2066 6169      # unless fai
-0000c6d0: 6c75 7265 2063 7574 7320 7468 726f 7567  lure cuts throug
-0000c6e0: 6820 736c 6f70 6520 2869 6e20 7768 6963  h slope (in whic
-0000c6f0: 6820 6361 7365 2076 616c 7565 206f 6620  h case value of 
-0000c700: 746f 650a 2020 2020 2020 2020 2320 7769  toe.        # wi
-0000c710: 6c6c 2062 6520 7069 636b 6564 2075 7020  ll be picked up 
-0000c720: 666f 7220 6d69 6420 696e 7465 7273 6563  for mid intersec
-0000c730: 7469 6f6e 2061 6e79 7761 7973 290a 2020  tion anyways).  
-0000c740: 2020 2020 2020 6966 2062 6f74 5f69 6e74        if bot_int
-0000c750: 6572 7365 6374 696f 6e3a 0a20 2020 2020  ersection:.     
-0000c760: 2020 2020 2020 2062 6f74 5f69 6e74 6572         bot_inter
-0000c770: 7365 6374 696f 6e2e 736f 7274 2829 0a20  section.sort(). 
-0000c780: 2020 2020 2020 2020 2020 2062 6f74 5f69             bot_i
-0000c790: 6e74 6572 7365 6374 696f 6e20 3d20 626f  ntersection = bo
-0000c7a0: 745f 696e 7465 7273 6563 7469 6f6e 5b2d  t_intersection[-
-0000c7b0: 315d 0a20 2020 2020 2020 2020 2020 2069  1].            i
-0000c7c0: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
-0000c7d0: 2020 2020 626f 745f 696e 7465 7273 6563      bot_intersec
-0000c7e0: 7469 6f6e 5b30 5d20 3e3d 2073 656c 662e  tion[0] >= self.
-0000c7f0: 5f62 6f74 5f63 6f6f 7264 5b30 5d0a 2020  _bot_coord[0].  
-0000c800: 2020 2020 2020 2020 2020 2020 2020 616e                an
-0000c810: 6420 626f 745f 696e 7465 7273 6563 7469  d bot_intersecti
-0000c820: 6f6e 5b30 5d20 3c3d 2073 656c 662e 5f65  on[0] <= self._e
-0000c830: 7874 6572 6e61 6c5f 6c65 6e67 7468 0a20  xternal_length. 
-0000c840: 2020 2020 2020 2020 2020 2029 3a0a 2020             ):.  
-0000c850: 2020 2020 2020 2020 2020 2020 2020 695f                i_
-0000c860: 6c69 7374 2e61 7070 656e 6428 626f 745f  list.append(bot_
-0000c870: 696e 7465 7273 6563 7469 6f6e 290a 0a20  intersection).. 
-0000c880: 2020 2020 2020 206d 6964 5f69 6e74 6572         mid_inter
-0000c890: 7365 6374 696f 6e20 3d20 7574 696c 6974  section = utilit
-0000c8a0: 6965 732e 6369 726c 655f 6c69 6e65 5f69  ies.cirle_line_i
-0000c8b0: 6e74 6572 7365 6374 696f 6e28 0a20 2020  ntersection(.   
-0000c8c0: 2020 2020 2020 2020 2073 656c 662e 5f74           self._t
-0000c8d0: 6f70 5f63 6f6f 7264 2c20 7365 6c66 2e5f  op_coord, self._
-0000c8e0: 626f 745f 636f 6f72 642c 2063 5f78 2c20  bot_coord, c_x, 
-0000c8f0: 635f 792c 2072 6164 6975 730a 2020 2020  c_y, radius.    
-0000c900: 2020 2020 290a 0a20 2020 2020 2020 2066      )..        f
-0000c910: 6f72 2061 2069 6e20 6d69 645f 696e 7465  or a in mid_inte
-0000c920: 7273 6563 7469 6f6e 3a0a 2020 2020 2020  rsection:.      
-0000c930: 2020 2020 2020 6966 2061 5b30 5d20 3e3d        if a[0] >=
-0000c940: 2073 656c 662e 5f74 6f70 5f63 6f6f 7264   self._top_coord
-0000c950: 5b30 5d20 616e 6420 615b 305d 203c 3d20  [0] and a[0] <= 
-0000c960: 7365 6c66 2e5f 626f 745f 636f 6f72 645b  self._bot_coord[
-0000c970: 305d 3a0a 2020 2020 2020 2020 2020 2020  0]:.            
-0000c980: 2020 2020 695f 6c69 7374 2e61 7070 656e      i_list.appen
-0000c990: 6428 6129 0a0a 2020 2020 2020 2020 2320  d(a)..        # 
-0000c9a0: 7265 6d6f 7665 2061 6e79 2063 6c6f 7365  remove any close
-0000c9b0: 2070 6f69 6e74 730a 2020 2020 2020 2020   points.        
-0000c9c0: 695f 6c69 7374 2e73 6f72 7428 6b65 793d  i_list.sort(key=
-0000c9d0: 6c61 6d62 6461 2078 3a20 785b 305d 290a  lambda x: x[0]).
-0000c9e0: 2020 2020 2020 2020 756e 6971 7565 5f6c          unique_l
-0000c9f0: 6973 7420 3d20 5b5d 0a20 2020 2020 2020  ist = [].       
-0000ca00: 2078 203d 202d 310a 2020 2020 2020 2020   x = -1.        
-0000ca10: 666f 7220 6920 696e 2069 5f6c 6973 743a  for i in i_list:
-0000ca20: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000ca30: 6162 7328 695b 305d 202d 2078 2920 3e20  abs(i[0] - x) > 
-0000ca40: 302e 3031 3a0a 2020 2020 2020 2020 2020  0.01:.          
-0000ca50: 2020 2020 2020 756e 6971 7565 5f6c 6973        unique_lis
-0000ca60: 742e 6170 7065 6e64 2869 290a 2020 2020  t.append(i).    
-0000ca70: 2020 2020 2020 2020 7820 3d20 695b 305d          x = i[0]
-0000ca80: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0000ca90: 2075 6e69 7175 655f 6c69 7374 0a0a 2020   unique_list..  
-0000caa0: 2020 6465 6620 5f63 616c 6375 6c61 7465    def _calculate
-0000cab0: 5f73 7472 6970 5f77 6569 6768 7428 7365  _strip_weight(se
-0000cac0: 6c66 2c20 623a 2066 6c6f 6174 2c20 735f  lf, b: float, s_
-0000cad0: 7974 3a20 666c 6f61 742c 2073 5f79 623a  yt: float, s_yb:
-0000cae0: 2066 6c6f 6174 293a 0a20 2020 2020 2020   float):.       
-0000caf0: 2022 2222 6361 6c63 756c 6174 6573 2074   """calculates t
-0000cb00: 6865 2077 6569 6768 7420 6f66 2061 2073  he weight of a s
-0000cb10: 7472 6970 2e0a 0a20 2020 2020 2020 2050  trip...        P
-0000cb20: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-0000cb30: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-0000cb40: 2020 2020 2062 203a 2066 6c6f 6174 0a20       b : float. 
-0000cb50: 2020 2020 2020 2020 2020 2073 7472 6970             strip
-0000cb60: 2077 6964 7468 2069 6e20 6d65 7472 6573   width in metres
-0000cb70: 0a20 2020 2020 2020 2073 5f79 7420 3a20  .        s_yt : 
-0000cb80: 666c 6f61 740a 2020 2020 2020 2020 2020  float.          
-0000cb90: 2020 7374 7269 7020 7920 636f 6f72 6469    strip y coordi
-0000cba0: 6e61 7465 2061 7420 746f 7020 6f66 2073  nate at top of s
-0000cbb0: 7472 6970 0a20 2020 2020 2020 2073 5f79  trip.        s_y
-0000cbc0: 6220 3a20 666c 6f61 740a 2020 2020 2020  b : float.      
-0000cbd0: 2020 2020 2020 7374 7269 7020 7920 636f        strip y co
-0000cbe0: 6f72 6469 6e61 7465 2061 7420 626f 7474  ordinate at bott
-0000cbf0: 6f6d 206f 6620 7374 7269 700a 0a20 2020  om of strip..   
-0000cc00: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
-0000cc10: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
-0000cc20: 2020 2020 2066 6c6f 6174 0a20 2020 2020       float.     
-0000cc30: 2020 2020 2020 2057 6569 6768 7420 6f66         Weight of
-0000cc40: 2073 7472 6970 2069 6e20 6b4e 2e0a 2020   strip in kN..  
-0000cc50: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-0000cc60: 2020 2023 2069 6e74 6961 6c69 7a65 2070     # intialize p
-0000cc70: 726f 7065 7274 6965 730a 2020 2020 2020  roperties.      
-0000cc80: 2020 5720 3d20 302e 3020 2023 206b 4e0a    W = 0.0  # kN.
-0000cc90: 2020 2020 2020 2020 746f 7020 3d20 735f          top = s_
-0000cca0: 7974 0a0a 2020 2020 2020 2020 2320 6c6f  yt..        # lo
-0000ccb0: 6f70 2074 6872 6f75 6768 206d 6174 6572  op through mater
-0000ccc0: 6961 6c73 206e 6f74 696e 6720 7468 6174  ials noting that
-0000ccd0: 2074 6865 7920 6172 6520 616c 7265 6164   they are alread
-0000cce0: 7920 736f 7274 6564 2062 7920 6465 7074  y sorted by dept
-0000ccf0: 680a 2020 2020 2020 2020 666f 7220 6d20  h.        for m 
-0000cd00: 696e 2073 656c 662e 5f6d 6174 6572 6961  in self._materia
-0000cd10: 6c73 3a0a 2020 2020 2020 2020 2020 2020  ls:.            
-0000cd20: 2320 7768 696c 6520 6c61 7965 7273 2061  # while layers a
-0000cd30: 7265 2068 6967 6865 7220 7468 616e 2074  re higher than t
-0000cd40: 6865 2074 6f70 206f 6620 7468 6520 736c  he top of the sl
-0000cd50: 6963 6520 6967 6e6f 7265 2074 6865 206d  ice ignore the m
-0000cd60: 6174 6572 6961 6c0a 2020 2020 2020 2020  aterial.        
-0000cd70: 2020 2020 6966 206d 2e52 4c20 3e3d 2073      if m.RL >= s
-0000cd80: 5f79 743a 0a20 2020 2020 2020 2020 2020  _yt:.           
-0000cd90: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
-0000cda0: 2020 2020 2020 2020 2020 2320 7768 696c            # whil
-0000cdb0: 6520 7468 6520 626f 7474 6f6d 206f 6620  e the bottom of 
-0000cdc0: 6c61 7965 7220 6973 2069 6e20 7468 6520  layer is in the 
-0000cdd0: 736c 6963 6520 636f 6e73 6964 6572 2c20  slice consider, 
-0000cde0: 676f 2066 726f 6d20 7468 650a 2020 2020  go from the.    
-0000cdf0: 2020 2020 2020 2020 2320 6375 7272 656e          # curren
-0000ce00: 7420 746f 7020 746f 2074 6865 2062 6f74  t top to the bot
-0000ce10: 746f 6d20 6f66 2074 6865 206c 6179 6572  tom of the layer
-0000ce20: 0a20 2020 2020 2020 2020 2020 2023 2074  .            # t
-0000ce30: 6869 7320 6361 7074 7572 6573 2074 6865  his captures the
-0000ce40: 2063 6173 6520 6f66 2074 6865 2074 6f70   case of the top
-0000ce50: 206f 6620 7468 6520 7374 7269 7020 6265   of the strip be
-0000ce60: 696e 6720 7061 7274 6961 6c6c 7920 696e  ing partially in
-0000ce70: 2061 206c 6179 6572 0a20 2020 2020 2020   a layer.       
-0000ce80: 2020 2020 2065 6c69 6620 6d2e 524c 203c       elif m.RL <
-0000ce90: 2073 5f79 7420 616e 6420 6d2e 524c 203e   s_yt and m.RL >
-0000cea0: 2073 5f79 623a 0a20 2020 2020 2020 2020   s_yb:.         
-0000ceb0: 2020 2020 2020 2057 202b 3d20 6220 2a20         W += b * 
-0000cec0: 6d2e 756e 6974 5f77 6569 6768 7420 2a20  m.unit_weight * 
-0000ced0: 2874 6f70 202d 206d 2e52 4c29 0a20 2020  (top - m.RL).   
-0000cee0: 2020 2020 2020 2020 2020 2020 2074 6f70               top
-0000cef0: 203d 206d 2e52 4c0a 2020 2020 2020 2020   = m.RL.        
-0000cf00: 2020 2020 2320 696e 2074 6865 2063 6173      # in the cas
-0000cf10: 6520 7468 6174 2074 6865 2062 6f74 746f  e that the botto
-0000cf20: 6d20 6f66 2074 6865 2073 7472 6970 2069  m of the strip i
-0000cf30: 7320 6e6f 7720 6f75 7473 6964 6520 7468  s now outside th
-0000cf40: 6520 7261 6e67 650a 2020 2020 2020 2020  e range.        
-0000cf50: 2020 2020 2320 7765 2073 7469 6c6c 2068      # we still h
-0000cf60: 6176 6520 6d61 7465 7269 616c 2062 6574  ave material bet
-0000cf70: 7765 656e 2074 6865 2063 7572 7265 6e74  ween the current
-0000cf80: 2074 6f70 2061 6e64 2074 6865 2062 6f74   top and the bot
-0000cf90: 746f 6d20 6f66 2074 6865 2073 7472 6970  tom of the strip
-0000cfa0: 0a20 2020 2020 2020 2020 2020 2023 2077  .            # w
-0000cfb0: 6520 6361 7074 7572 6520 6974 2069 6e20  e capture it in 
-0000cfc0: 7468 6973 2065 6467 6520 6361 7365 2061  this edge case a
-0000cfd0: 6e64 2074 6865 6e20 6272 6561 6b20 7369  nd then break si
-0000cfe0: 6e63 6520 6576 6572 7974 6869 6e67 2062  nce everything b
-0000cff0: 656c 6f77 2063 616e 2062 6520 6967 6e6f  elow can be igno
-0000d000: 7265 640a 2020 2020 2020 2020 2020 2020  red.            
-0000d010: 2320 7765 2061 6c73 6f20 6772 6162 2074  # we also grab t
-0000d020: 6865 206d 6174 6572 6961 6c20 7072 6f70  he material prop
-0000d030: 6572 7469 6573 2061 7420 7468 6520 6261  erties at the ba
-0000d040: 7365 0a20 2020 2020 2020 2020 2020 2065  se.            e
-0000d050: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000d060: 2020 2020 2057 202b 3d20 6220 2a20 6d2e       W += b * m.
-0000d070: 756e 6974 5f77 6569 6768 7420 2a20 2874  unit_weight * (t
-0000d080: 6f70 202d 2073 5f79 6229 0a20 2020 2020  op - s_yb).     
-0000d090: 2020 2020 2020 2020 2020 2074 6f70 203d             top =
-0000d0a0: 206d 2e52 4c0a 2020 2020 2020 2020 2020   m.RL.          
-0000d0b0: 2020 2020 2020 6272 6561 6b0a 0a20 2020        break..   
-0000d0c0: 2020 2020 2023 2063 6865 636b 2063 6173       # check cas
-0000d0d0: 6520 7468 6174 2072 616e 206f 7574 206f  e that ran out o
-0000d0e0: 6620 6c61 7965 7273 2028 6c6f 6f70 2074  f layers (loop t
-0000d0f0: 6572 6d69 6e61 7465 6420 6561 726c 6965  erminated earlie
-0000d100: 7220 7468 616e 2065 7870 6563 7465 6429  r than expected)
-0000d110: 0a20 2020 2020 2020 2069 6620 746f 7020  .        if top 
-0000d120: 3e20 735f 7962 3a0a 2020 2020 2020 2020  > s_yb:.        
-0000d130: 2020 2020 6d20 3d20 7365 6c66 2e5f 6d61      m = self._ma
-0000d140: 7465 7269 616c 735b 2d31 5d0a 2020 2020  terials[-1].    
-0000d150: 2020 2020 2020 2020 5720 2b3d 2062 202a          W += b *
-0000d160: 206d 2e75 6e69 745f 7765 6967 6874 202a   m.unit_weight *
-0000d170: 2028 746f 7020 2d20 735f 7962 290a 0a20   (top - s_yb).. 
-0000d180: 2020 2020 2020 2072 6574 7572 6e20 570a         return W.
-0000d190: 0a20 2020 2064 6566 205f 6765 745f 6d61  .    def _get_ma
-0000d1a0: 7465 7269 616c 5f61 745f 6465 7074 6828  terial_at_depth(
-0000d1b0: 7365 6c66 2c20 735f 7962 293a 0a20 2020  self, s_yb):.   
-0000d1c0: 2020 2020 2022 2222 5265 7475 726e 2074       """Return t
-0000d1d0: 6865 206d 6174 6572 6961 6c20 636c 6173  he material clas
-0000d1e0: 7320 6174 2061 2073 7065 6369 6669 6564  s at a specified
-0000d1f0: 2064 6570 7468 2e0a 0a20 2020 2020 2020   depth...       
-0000d200: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-0000d210: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-0000d220: 2020 2020 2020 2073 5f79 6220 3a20 666c         s_yb : fl
-0000d230: 6f61 740a 2020 2020 2020 2020 2020 2020  oat.            
-0000d240: 7374 7269 7020 7920 636f 6f72 6469 6e61  strip y coordina
-0000d250: 7465 2061 7420 626f 7474 6f6d 206f 6620  te at bottom of 
-0000d260: 7374 7269 700a 0a20 2020 2020 2020 2052  strip..        R
-0000d270: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
-0000d280: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 204d  ------.        M
-0000d290: 6174 6572 6961 6c0a 2020 2020 2020 2020  aterial.        
-0000d2a0: 2020 2020 6d61 7465 7269 616c 206f 626a      material obj
-0000d2b0: 6563 7420 6174 2074 6865 2073 7065 6369  ect at the speci
-0000d2c0: 6669 6564 2064 6570 7468 2e0a 2020 2020  fied depth..    
-0000d2d0: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
-0000d2e0: 2023 206c 6f6f 7020 7468 726f 7567 6820   # loop through 
-0000d2f0: 616c 6c20 6d61 7465 7269 616c 732c 2069  all materials, i
-0000d300: 6620 7765 2068 6176 6520 7061 7373 6564  f we have passed
-0000d310: 2074 6865 2062 6f74 746f 6d20 7461 6b65   the bottom take
-0000d320: 2074 6865 2070 7265 7669 6f75 730a 2020   the previous.  
-0000d330: 2020 2020 2020 666f 7220 6d20 696e 2073        for m in s
-0000d340: 656c 662e 5f6d 6174 6572 6961 6c73 3a0a  elf._materials:.
-0000d350: 2020 2020 2020 2020 2020 2020 6966 206d              if m
-0000d360: 2e52 4c20 3c20 735f 7962 3a0a 2020 2020  .RL < s_yb:.    
-0000d370: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000d380: 726e 206d 0a0a 2020 2020 2020 2020 7265  rn m..        re
-0000d390: 7475 726e 2073 656c 662e 5f6d 6174 6572  turn self._mater
-0000d3a0: 6961 6c73 5b2d 315d 0a0a 2020 2020 6465  ials[-1]..    de
-0000d3b0: 6620 5f63 616c 6375 6c61 7465 5f73 7472  f _calculate_str
-0000d3c0: 6970 5f75 646c 5f66 6f72 6365 2873 656c  ip_udl_force(sel
-0000d3d0: 662c 2062 2c20 735f 782c 2075 646c 293a  f, b, s_x, udl):
-0000d3e0: 0a20 2020 2020 2020 2022 2222 4361 6c63  .        """Calc
-0000d3f0: 756c 6174 6573 2074 6865 2075 646c 2066  ulates the udl f
-0000d400: 6f72 6365 206f 7665 7220 7374 7269 702e  orce over strip.
-0000d410: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-0000d420: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
-0000d430: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-0000d440: 6220 3a20 666c 6f61 742c 0a20 2020 2020  b : float,.     
-0000d450: 2020 2020 2020 2073 7472 6970 2077 6964         strip wid
-0000d460: 7468 2069 6e20 6d0a 2020 2020 2020 2020  th in m.        
-0000d470: 735f 7820 3a20 666c 6f61 742c 0a20 2020  s_x : float,.   
-0000d480: 2020 2020 2020 2020 2073 7472 6970 2078           strip x
-0000d490: 2063 6f6f 7264 696e 6174 6520 2866 6f72   coordinate (for
-0000d4a0: 2063 656e 7465 7220 6f66 2073 7472 6970   center of strip
-0000d4b0: 290a 2020 2020 2020 2020 7564 6c20 3a20  ).        udl : 
-0000d4c0: 5564 6c20 6f62 6a65 6374 2c0a 2020 2020  Udl object,.    
-0000d4d0: 2020 2020 2020 2020 7564 6c20 6f62 6a65          udl obje
-0000d4e0: 6374 0a0a 2020 2020 2020 2020 5265 7475  ct..        Retu
-0000d4f0: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
-0000d500: 2d2d 2d0a 2020 2020 2020 2020 666c 6f61  ---.        floa
-0000d510: 740a 2020 2020 2020 2020 2020 2020 7564  t.            ud
-0000d520: 6c20 666f 7263 6520 6f6e 2073 7472 6970  l force on strip
-0000d530: 2069 6e20 6b4e 0a20 2020 2020 2020 2022   in kN.        "
-0000d540: 2222 0a20 2020 2020 2020 2057 203d 2030  "".        W = 0
-0000d550: 0a0a 2020 2020 2020 2020 6c6f 6164 5f78  ..        load_x
-0000d560: 6c2c 206c 6f61 645f 7872 203d 2075 646c  l, load_xr = udl
-0000d570: 2e6c 6566 742c 2075 646c 2e72 6967 6874  .left, udl.right
-0000d580: 0a20 2020 2020 2020 2073 7472 6970 5f78  .        strip_x
-0000d590: 6c20 3d20 735f 7820 2d20 2862 202f 2032  l = s_x - (b / 2
-0000d5a0: 290a 2020 2020 2020 2020 7374 7269 705f  ).        strip_
-0000d5b0: 7872 203d 2073 5f78 202b 2028 6220 2f20  xr = s_x + (b / 
-0000d5c0: 3229 0a0a 2020 2020 2020 2020 2320 6361  2)..        # ca
-0000d5d0: 7365 2031 2063 6c65 6172 6c79 206c 6f61  se 1 clearly loa
-0000d5e0: 6420 6973 2063 6f6d 706c 6574 656c 7920  d is completely 
-0000d5f0: 696e 7369 6465 0a20 2020 2020 2020 2069  inside.        i
-0000d600: 6620 6c6f 6164 5f78 6c20 3c3d 2073 7472  f load_xl <= str
-0000d610: 6970 5f78 6c20 616e 6420 6c6f 6164 5f78  ip_xl and load_x
-0000d620: 7220 3e3d 2073 7472 6970 5f78 723a 0a20  r >= strip_xr:. 
-0000d630: 2020 2020 2020 2020 2020 2057 202b 3d20             W += 
-0000d640: 6220 2a20 7564 6c2e 6d61 676e 6974 7564  b * udl.magnitud
-0000d650: 650a 2020 2020 2020 2020 2320 6361 7365  e.        # case
-0000d660: 2032 206f 6e20 7468 6520 6c65 6674 2069   2 on the left i
-0000d670: 6e73 6964 6520 7468 6520 6c6f 6164 0a20  nside the load. 
-0000d680: 2020 2020 2020 2065 6c69 6620 7374 7269         elif stri
-0000d690: 705f 786c 203c 3d20 6c6f 6164 5f78 6c20  p_xl <= load_xl 
-0000d6a0: 616e 6420 7374 7269 705f 7872 203e 3d20  and strip_xr >= 
-0000d6b0: 6c6f 6164 5f78 6c3a 0a20 2020 2020 2020  load_xl:.       
-0000d6c0: 2020 2020 2057 202b 3d20 2873 7472 6970       W += (strip
-0000d6d0: 5f78 7220 2d20 6c6f 6164 5f78 6c29 202a  _xr - load_xl) *
-0000d6e0: 2075 646c 2e6d 6167 6e69 7475 6465 0a0a   udl.magnitude..
-0000d6f0: 2020 2020 2020 2020 2320 6361 7365 2033          # case 3
-0000d700: 206f 6e20 7468 6520 7269 6768 7420 7369   on the right si
-0000d710: 6465 206f 6620 7468 6520 6c6f 6164 0a20  de of the load. 
-0000d720: 2020 2020 2020 2065 6c69 6620 7374 7269         elif stri
-0000d730: 705f 786c 203c 3d20 6c6f 6164 5f78 7220  p_xl <= load_xr 
-0000d740: 616e 6420 7374 7269 705f 7872 203e 3d20  and strip_xr >= 
-0000d750: 6c6f 6164 5f78 723a 0a20 2020 2020 2020  load_xr:.       
-0000d760: 2020 2020 2057 202b 3d20 286c 6f61 645f       W += (load_
-0000d770: 7872 202d 2073 7472 6970 5f78 6c29 202a  xr - strip_xl) *
-0000d780: 2075 646c 2e6d 6167 6e69 7475 6465 0a0a   udl.magnitude..
-0000d790: 2020 2020 2020 2020 7265 7475 726e 2057          return W
-0000d7a0: 0a0a 2020 2020 6465 6620 5f63 616c 6375  ..    def _calcu
-0000d7b0: 6c61 7465 5f73 7472 6970 5f6c 6c28 7365  late_strip_ll(se
-0000d7c0: 6c66 2c20 622c 2073 5f78 2c20 6c6c 293a  lf, b, s_x, ll):
-0000d7d0: 0a20 2020 2020 2020 2022 2222 4361 6c63  .        """Calc
-0000d7e0: 756c 6174 6573 2074 6865 206c 6c20 666f  ulates the ll fo
-0000d7f0: 7263 6520 6f76 6572 2073 7472 6970 2e0a  rce over strip..
-0000d800: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-0000d810: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
-0000d820: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2062  ------.        b
-0000d830: 203a 2066 6c6f 6174 2c0a 2020 2020 2020   : float,.      
-0000d840: 2020 2020 2020 7374 7269 7020 7769 6474        strip widt
-0000d850: 6820 696e 206d 0a20 2020 2020 2020 2073  h in m.        s
-0000d860: 5f78 203a 2066 6c6f 6174 2c0a 2020 2020  _x : float,.    
-0000d870: 2020 2020 2020 2020 7374 7269 7020 7820          strip x 
-0000d880: 636f 6f72 6469 6e61 7465 2028 666f 7220  coordinate (for 
-0000d890: 6365 6e74 6572 206f 6620 7374 7269 7029  center of strip)
-0000d8a0: 0a20 2020 2020 2020 206c 6c20 3a20 4c69  .        ll : Li
-0000d8b0: 6e65 4c6f 6164 206f 626a 6563 742c 0a20  neLoad object,. 
-0000d8c0: 2020 2020 2020 2020 2020 204c 696e 654c             LineL
-0000d8d0: 6f61 6420 6f62 6a65 6374 0a0a 2020 2020  oad object..    
-0000d8e0: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-0000d8f0: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-0000d900: 2020 2020 666c 6f61 740a 2020 2020 2020      float.      
-0000d910: 2020 2020 2020 7564 6c20 666f 7263 6520        udl force 
-0000d920: 6f6e 2073 7472 6970 2069 6e20 6b4e 0a20  on strip in kN. 
-0000d930: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
-0000d940: 2020 2020 7374 7269 705f 786c 203d 2073      strip_xl = s
-0000d950: 5f78 202d 2028 6220 2f20 3229 0a20 2020  _x - (b / 2).   
-0000d960: 2020 2020 2073 7472 6970 5f78 7220 3d20       strip_xr = 
-0000d970: 735f 7820 2b20 2862 202f 2032 290a 0a20  s_x + (b / 2).. 
-0000d980: 2020 2020 2020 2023 204e 6565 6420 6a75         # Need ju
-0000d990: 7374 206f 6e65 2063 6f6d 7061 7269 736f  st one compariso
-0000d9a0: 6e20 746f 2062 6520 6571 7561 6c20 746f  n to be equal to
-0000d9b0: 206f 7220 6772 6561 7465 7220 7468 616e   or greater than
-0000d9c0: 2073 6f20 7468 6174 0a20 2020 2020 2020   so that.       
-0000d9d0: 2023 2069 6e20 7468 6520 6361 7365 2074   # in the case t
-0000d9e0: 6865 2070 6f69 6e74 206c 6f61 6420 6973  he point load is
-0000d9f0: 2065 7863 6174 6c79 2061 7420 7468 6520   excatly at the 
-0000da00: 626f 756e 6461 7279 0a20 2020 2020 2020  boundary.       
-0000da10: 2023 2074 776f 2061 646a 6365 6e74 2073   # two adjcent s
-0000da20: 7472 6970 7320 776f 6e74 2064 6f75 626c  trips wont doubl
-0000da30: 6520 7570 206f 7220 6967 6e6f 7265 2063  e up or ignore c
-0000da40: 6f6d 706c 6574 656c 792e 0a20 2020 2020  ompletely..     
-0000da50: 2020 2069 6620 7374 7269 705f 786c 203c     if strip_xl <
-0000da60: 3d20 6c6c 2e63 6f6f 7264 203c 2073 7472  = ll.coord < str
-0000da70: 6970 5f78 723a 0a20 2020 2020 2020 2020  ip_xr:.         
-0000da80: 2020 2072 6574 7572 6e20 6c6c 2e6d 6167     return ll.mag
-0000da90: 6e69 7475 6465 0a20 2020 2020 2020 2065  nitude.        e
-0000daa0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000dab0: 2072 6574 7572 6e20 300a 0a20 2020 2064   return 0..    d
-0000dac0: 6566 2067 6574 5f64 796e 616d 6963 5f72  ef get_dynamic_r
-0000dad0: 6573 756c 7473 2873 656c 6629 3a0a 2020  esults(self):.  
-0000dae0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000daf0: 662e 5f64 796e 616d 6963 5f72 6573 756c  f._dynamic_resul
-0000db00: 7473 0a0a 2020 2020 6465 6620 7072 696e  ts..    def prin
-0000db10: 745f 6479 6e61 6d69 635f 7265 7375 6c74  t_dynamic_result
-0000db20: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
-0000db30: 2066 6f72 206b 2c20 7620 696e 2073 656c   for k, v in sel
-0000db40: 662e 6765 745f 6479 6e61 6d69 635f 7265  f.get_dynamic_re
-0000db50: 7375 6c74 7328 292e 6974 656d 7328 293a  sults().items():
-0000db60: 0a20 2020 2020 2020 2020 2020 206f 6666  .            off
-0000db70: 7365 7420 3d20 7374 7228 726f 756e 6428  set = str(round(
-0000db80: 6b2c 2033 2929 0a20 2020 2020 2020 2020  k, 3)).         
-0000db90: 2020 206f 6666 7365 7420 3d20 6f66 6673     offset = offs
-0000dba0: 6574 202b 2022 3022 202a 2028 3520 2d20  et + "0" * (5 - 
-0000dbb0: 6c65 6e28 6f66 6673 6574 2929 0a0a 2020  len(offset))..  
-0000dbc0: 2020 2020 2020 2020 2020 666f 7320 3d20            fos = 
-0000dbd0: 7374 7228 726f 756e 6428 762c 2033 2929  str(round(v, 3))
-0000dbe0: 0a20 2020 2020 2020 2020 2020 2066 6f73  .            fos
-0000dbf0: 203d 2066 6f73 202b 2022 3022 202a 2028   = fos + "0" * (
-0000dc00: 3520 2d20 6c65 6e28 666f 7329 290a 0a20  5 - len(fos)).. 
-0000dc10: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-0000dc20: 2866 224f 6666 7365 743a 207b 6f66 6673  (f"Offset: {offs
-0000dc30: 6574 7d20 6d2c 2046 4f53 3a20 7b66 6f73  et} m, FOS: {fos
-0000dc40: 7d22 290a 0a20 2020 2064 6566 2067 6574  }")..    def get
-0000dc50: 5f6d 696e 5f46 4f53 2873 656c 6629 3a0a  _min_FOS(self):.
-0000dc60: 2020 2020 2020 2020 2222 2247 6574 206d          """Get m
-0000dc70: 696e 2066 6163 746f 7220 6f66 2073 6166  in factor of saf
-0000dc80: 6574 7920 666f 7220 736c 6f70 6520 6d6f  ety for slope mo
-0000dc90: 6465 6c2e 0a0a 2020 2020 2020 2020 5265  del...        Re
-0000dca0: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
-0000dcb0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 666c  -----.        fl
-0000dcc0: 6f61 740a 2020 2020 2020 2020 2020 2020  oat.            
-0000dcd0: 6372 6974 6963 616c 2066 6163 746f 7220  critical factor 
-0000dce0: 6f66 2073 6166 6574 790a 2020 2020 2020  of safety.      
-0000dcf0: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
-0000dd00: 7475 726e 2073 656c 662e 5f73 6561 7263  turn self._searc
-0000dd10: 685b 305d 5b22 464f 5322 5d0a 0a20 2020  h[0]["FOS"]..   
-0000dd20: 2064 6566 2067 6574 5f6d 696e 5f46 4f53   def get_min_FOS
-0000dd30: 5f63 6972 636c 6528 7365 6c66 293a 0a20  _circle(self):. 
-0000dd40: 2020 2020 2020 2022 2222 4765 7420 7468         """Get th
-0000dd50: 6520 7072 6f70 6572 7469 6573 206f 6620  e properties of 
-0000dd60: 7468 6520 6369 7263 6c65 2074 6861 7420  the circle that 
-0000dd70: 6761 7665 2074 6865 2063 7269 7469 6361  gave the critica
-0000dd80: 6c20 6661 6374 6f72 206f 6620 7361 6665  l factor of safe
-0000dd90: 7479 2e0a 0a20 2020 2020 2020 2052 6574  ty...        Ret
-0000dda0: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
-0000ddb0: 2d2d 2d2d 0a20 2020 2020 2020 2074 7570  ----.        tup
-0000ddc0: 6c65 0a20 2020 2020 2020 2020 2020 2074  le.            t
-0000ddd0: 7570 6c65 2063 6f6e 7461 696e 696e 6720  uple containing 
-0000dde0: 2863 6972 636c 6520 7820 636f 6f72 6469  (circle x coordi
-0000ddf0: 6e61 7465 2c20 6369 7263 6c65 2079 2063  nate, circle y c
-0000de00: 6f6f 7264 696e 6174 652c 2063 6972 636c  oordinate, circl
-0000de10: 6520 7261 6469 7573 290a 2020 2020 2020  e radius).      
-0000de20: 2020 2222 220a 2020 2020 2020 2020 635f    """.        c_
-0000de30: 7820 3d20 7365 6c66 2e5f 7365 6172 6368  x = self._search
-0000de40: 5b30 5d5b 2263 5f78 225d 0a20 2020 2020  [0]["c_x"].     
-0000de50: 2020 2063 5f79 203d 2073 656c 662e 5f73     c_y = self._s
-0000de60: 6561 7263 685b 305d 5b22 635f 7922 5d0a  earch[0]["c_y"].
-0000de70: 2020 2020 2020 2020 7261 6469 7573 203d          radius =
-0000de80: 2073 656c 662e 5f73 6561 7263 685b 305d   self._search[0]
-0000de90: 5b22 7261 6469 7573 225d 0a20 2020 2020  ["radius"].     
-0000dea0: 2020 2072 6574 7572 6e20 2863 5f78 2c20     return (c_x, 
-0000deb0: 635f 792c 2072 6164 6975 7329 0a0a 2020  c_y, radius)..  
-0000dec0: 2020 6465 6620 6765 745f 6d69 6e5f 464f    def get_min_FO
-0000ded0: 535f 656e 645f 706f 696e 7473 2873 656c  S_end_points(sel
-0000dee0: 6629 3a0a 2020 2020 2020 2020 2222 2247  f):.        """G
-0000def0: 6574 2074 6865 2065 7874 6572 6e61 6c20  et the external 
-0000df00: 626f 756e 6461 7279 2069 6e74 6572 7365  boundary interse
-0000df10: 6374 696f 6e20 666f 7220 7468 6520 736c  ction for the sl
-0000df20: 6f70 6520 7468 6174 2067 6176 6520 7468  ope that gave th
-0000df30: 6520 6372 6974 6963 616c 2066 6163 746f  e critical facto
-0000df40: 7220 6f66 2073 6166 6574 792e 0a0a 2020  r of safety...  
-0000df50: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
-0000df60: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
-0000df70: 2020 2020 2020 7475 706c 650a 2020 2020        tuple.    
-0000df80: 2020 2020 2020 2020 7475 706c 6520 636f          tuple co
-0000df90: 6e74 6169 6e69 6e67 2028 6c65 6674 2063  ntaining (left c
-0000dfa0: 6f6f 7264 696e 6174 652c 2072 6967 6874  oordinate, right
-0000dfb0: 2063 6f6f 7264 696e 6174 6529 0a20 2020   coordinate).   
-0000dfc0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000dfd0: 206c 5f63 203d 2073 656c 662e 5f73 6561   l_c = self._sea
-0000dfe0: 7263 685b 305d 5b22 6c5f 6322 5d0a 2020  rch[0]["l_c"].  
-0000dff0: 2020 2020 2020 725f 6320 3d20 7365 6c66        r_c = self
-0000e000: 2e5f 7365 6172 6368 5b30 5d5b 2272 5f63  ._search[0]["r_c
-0000e010: 225d 0a20 2020 2020 2020 2072 6574 7572  "].        retur
-0000e020: 6e20 286c 5f63 2c20 725f 6329 0a0a 2020  n (l_c, r_c)..  
-0000e030: 2020 6465 6620 6765 745f 6578 7465 726e    def get_extern
-0000e040: 616c 5f79 5f69 6e74 6572 7365 6374 696f  al_y_intersectio
-0000e050: 6e28 7365 6c66 2c20 7829 3a0a 2020 2020  n(self, x):.    
-0000e060: 2020 2020 2222 2272 6574 7572 6e20 7920      """return y 
-0000e070: 636f 6f72 6469 6e61 7465 206f 6620 696e  coordinate of in
-0000e080: 7465 7273 6563 7469 6f6e 2077 6974 6820  tersection with 
-0000e090: 626f 756e 6461 7279 2066 6f72 2061 2067  boundary for a g
-0000e0a0: 6976 656e 2078 2222 220a 2020 2020 2020  iven x""".      
-0000e0b0: 2020 6966 2078 203c 2030 206f 7220 7820    if x < 0 or x 
-0000e0c0: 3e20 7365 6c66 2e5f 6578 7465 726e 616c  > self._external
-0000e0d0: 5f6c 656e 6774 683a 0a20 2020 2020 2020  _length:.       
-0000e0e0: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
-0000e0f0: 0a20 2020 2020 2020 2023 2079 2069 7320  .        # y is 
-0000e100: 6265 6c6f 7720 7468 6520 626f 7474 6f6d  below the bottom
-0000e110: 206f 6620 7468 6520 736c 6f70 650a 2020   of the slope.  
-0000e120: 2020 2020 2020 656c 6966 2078 203c 3d20        elif x <= 
-0000e130: 7365 6c66 2e5f 746f 705f 636f 6f72 645b  self._top_coord[
-0000e140: 305d 3a0a 2020 2020 2020 2020 2020 2020  0]:.            
-0000e150: 7265 7475 726e 2073 656c 662e 5f74 6f70  return self._top
-0000e160: 5f63 6f6f 7264 5b31 5d0a 2020 2020 2020  _coord[1].      
-0000e170: 2020 656c 6966 2078 203e 3d20 7365 6c66    elif x >= self
-0000e180: 2e5f 626f 745f 636f 6f72 645b 305d 3a0a  ._bot_coord[0]:.
-0000e190: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000e1a0: 726e 2073 656c 662e 5f62 6f74 5f63 6f6f  rn self._bot_coo
-0000e1b0: 7264 5b31 5d0a 2020 2020 2020 2020 2320  rd[1].        # 
-0000e1c0: 7920 6973 2061 626f 7665 2074 6865 2062  y is above the b
-0000e1d0: 6f74 746f 6d20 6f66 2074 6865 2073 6c6f  ottom of the slo
-0000e1e0: 7065 0a20 2020 2020 2020 2065 6c73 653a  pe.        else:
-0000e1f0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000e200: 7572 6e20 7365 6c66 2e5f 746f 705f 636f  urn self._top_co
-0000e210: 6f72 645b 315d 202d 2028 7820 2d20 7365  ord[1] - (x - se
-0000e220: 6c66 2e5f 746f 705f 636f 6f72 645b 305d  lf._top_coord[0]
-0000e230: 2920 2a20 7365 6c66 2e5f 6772 6164 6965  ) * self._gradie
-0000e240: 6e74 0a0a 2020 2020 6465 6620 6765 745f  nt..    def get_
-0000e250: 6578 7465 726e 616c 5f78 5f69 6e74 6572  external_x_inter
-0000e260: 7365 6374 696f 6e28 7365 6c66 2c20 7929  section(self, y)
-0000e270: 3a0a 2020 2020 2020 2020 2222 2272 6574  :.        """ret
-0000e280: 7572 6e20 7820 636f 6f72 6469 6e61 7465  urn x coordinate
-0000e290: 206f 6620 696e 7465 7273 6563 7469 6f6e   of intersection
-0000e2a0: 2077 6974 6820 626f 756e 6461 7279 2066   with boundary f
-0000e2b0: 6f72 2061 2067 6976 656e 2079 2222 220a  or a given y""".
-0000e2c0: 2020 2020 2020 2020 2320 7920 6973 2062          # y is b
-0000e2d0: 656c 6f77 2074 6865 2062 6f74 746f 6d20  elow the bottom 
-0000e2e0: 6f66 2074 6865 2073 6c6f 7065 0a20 2020  of the slope.   
-0000e2f0: 2020 2020 2069 6620 7920 3c20 7365 6c66       if y < self
-0000e300: 2e5f 626f 745f 636f 6f72 645b 315d 3a0a  ._bot_coord[1]:.
-0000e310: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000e320: 726e 2073 656c 662e 5f65 7874 6572 6e61  rn self._externa
-0000e330: 6c5f 6c65 6e67 7468 0a0a 2020 2020 2020  l_length..      
-0000e340: 2020 2320 7920 6973 2061 626f 7665 2074    # y is above t
-0000e350: 6865 2062 6f74 746f 6d20 6f66 2074 6865  he bottom of the
-0000e360: 2073 6c6f 7065 0a20 2020 2020 2020 2065   slope.        e
-0000e370: 6c69 6620 7920 3c20 7365 6c66 2e5f 6578  lif y < self._ex
-0000e380: 7465 726e 616c 5f68 6569 6768 743a 0a20  ternal_height:. 
-0000e390: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000e3a0: 6e20 7365 6c66 2e5f 746f 705f 636f 6f72  n self._top_coor
-0000e3b0: 645b 305d 202b 2028 7365 6c66 2e5f 746f  d[0] + (self._to
-0000e3c0: 705f 636f 6f72 645b 315d 202d 2079 2920  p_coord[1] - y) 
-0000e3d0: 2f20 7365 6c66 2e5f 6772 6164 6965 6e74  / self._gradient
-0000e3e0: 0a0a 2020 2020 2020 2020 656c 6966 2079  ..        elif y
-0000e3f0: 203d 3d20 7365 6c66 2e5f 626f 745f 636f   == self._bot_co
-0000e400: 6f72 645b 315d 3a0a 2020 2020 2020 2020  ord[1]:.        
-0000e410: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0000e420: 5f62 6f74 5f63 6f6f 7264 5b30 5d0a 0a20  _bot_coord[0].. 
-0000e430: 2020 2020 2020 2065 6c69 6620 7920 3d3d         elif y ==
-0000e440: 2073 656c 662e 5f74 6f70 5f63 6f6f 7264   self._top_coord
-0000e450: 5b31 5d3a 0a20 2020 2020 2020 2020 2020  [1]:.           
-0000e460: 2072 6574 7572 6e20 7365 6c66 2e5f 746f   return self._to
-0000e470: 705f 636f 6f72 645b 305d 0a0a 2020 2020  p_coord[0]..    
-0000e480: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000e490: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
-0000e4a0: 650a 0a20 2020 2064 6566 2067 6574 5f74  e..    def get_t
-0000e4b0: 6f70 5f63 6f6f 7264 696e 6174 6573 2873  op_coordinates(s
-0000e4c0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-0000e4d0: 2252 6574 7572 6e73 2074 6865 2074 6f70  "Returns the top
-0000e4e0: 2063 6f6f 7264 696e 6174 6520 6f66 2074   coordinate of t
-0000e4f0: 6865 2073 6c6f 7065 2e0a 0a20 2020 2020  he slope...     
-0000e500: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
-0000e510: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-0000e520: 2020 2074 7570 6c65 0a20 2020 2020 2020     tuple.       
-0000e530: 2020 2020 2028 782c 7929 2063 6f6f 7264       (x,y) coord
-0000e540: 696e 6174 6520 6f66 2074 6865 2074 6f70  inate of the top
-0000e550: 206f 6620 7468 6520 736c 6f70 652e 0a20   of the slope.. 
-0000e560: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000e570: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-0000e580: 746f 705f 636f 6f72 640a 0a20 2020 2064  top_coord..    d
-0000e590: 6566 2067 6574 5f62 6f74 746f 6d5f 636f  ef get_bottom_co
-0000e5a0: 6f72 6469 6e61 7465 7328 7365 6c66 293a  ordinates(self):
-0000e5b0: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
-0000e5c0: 726e 7320 7468 6520 626f 7474 6f6d 2063  rns the bottom c
-0000e5d0: 6f6f 7264 696e 6174 6520 6f66 2074 6865  oordinate of the
-0000e5e0: 2073 6c6f 7065 2e0a 0a20 2020 2020 2020   slope...       
-0000e5f0: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
-0000e600: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
-0000e610: 2074 7570 6c65 0a20 2020 2020 2020 2020   tuple.         
-0000e620: 2020 2028 782c 7929 2063 6f6f 7264 696e     (x,y) coordin
-0000e630: 6174 6520 6f66 2074 6865 2062 6f74 746f  ate of the botto
-0000e640: 6d20 6f66 2074 6865 2073 6c6f 7065 2e0a  m of the slope..
-0000e650: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000e660: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0000e670: 5f62 6f74 5f63 6f6f 7264 0a0a 2020 2020  _bot_coord..    
-0000e680: 6465 6620 706c 6f74 5f62 6f75 6e64 6172  def plot_boundar
-0000e690: 7928 7365 6c66 2c20 6d61 7465 7269 616c  y(self, material
-0000e6a0: 5f74 6162 6c65 3d54 7275 652c 206c 6567  _table=True, leg
-0000e6b0: 656e 643d 4661 6c73 6529 3a0a 2020 2020  end=False):.    
-0000e6c0: 2020 2020 2222 2250 6c6f 7420 6578 7465      """Plot exte
-0000e6d0: 726e 616c 2062 6f75 6e64 6172 792c 206d  rnal boundary, m
-0000e6e0: 6174 6572 6961 6c73 2c20 6c69 6d69 7473  aterials, limits
-0000e6f0: 2c20 6c6f 6164 696e 6720 616e 6420 7761  , loading and wa
-0000e700: 7465 7220 666f 7220 6d6f 6465 6c2e 0a0a  ter for model...
-0000e710: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
-0000e720: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
-0000e730: 2020 2020 2020 2020 706c 6f74 6c79 2066          plotly f
-0000e740: 6967 7572 650a 0a20 2020 2020 2020 2022  igure..        "
-0000e750: 2222 0a20 2020 2020 2020 2023 2064 7261  "".        # dra
-0000e760: 7720 7468 6520 6578 7465 726e 616c 2062  w the external b
-0000e770: 6f75 6e64 6172 790a 2020 2020 2020 2020  oundary.        
-0000e780: 785f 203d 205b 7820 666f 7220 782c 2079  x_ = [x for x, y
-0000e790: 2069 6e20 7365 6c66 2e5f 6578 7465 726e   in self._extern
-0000e7a0: 616c 5f62 6f75 6e64 6172 795d 0a20 2020  al_boundary].   
-0000e7b0: 2020 2020 2079 5f20 3d20 5b79 2066 6f72       y_ = [y for
-0000e7c0: 2078 2c20 7920 696e 2073 656c 662e 5f65   x, y in self._e
-0000e7d0: 7874 6572 6e61 6c5f 626f 756e 6461 7279  xternal_boundary
-0000e7e0: 5d0a 2020 2020 2020 2020 6669 6720 3d20  ].        fig = 
-0000e7f0: 676f 2e46 6967 7572 6528 676f 2e53 6361  go.Figure(go.Sca
-0000e800: 7474 6572 2878 3d6c 6973 7428 785f 292c  tter(x=list(x_),
-0000e810: 2079 3d6c 6973 7428 795f 292c 206d 6f64   y=list(y_), mod
-0000e820: 653d 226c 696e 6573 222c 206e 616d 653d  e="lines", name=
-0000e830: 2222 2929 0a0a 2020 2020 2020 2020 6669  ""))..        fi
-0000e840: 672e 7570 6461 7465 5f6c 6179 6f75 7428  g.update_layout(
-0000e850: 7769 6474 683d 3230 3030 2c20 6865 6967  width=2000, heig
-0000e860: 6874 3d31 3230 3029 0a0a 2020 2020 2020  ht=1200)..      
-0000e870: 2020 2320 666f 6c6c 6f77 696e 6720 6d61    # following ma
-0000e880: 6b65 7320 7375 7265 2078 2061 6e64 2079  kes sure x and y
-0000e890: 2061 7265 2073 6361 6c65 6420 7468 6520   are scaled the 
-0000e8a0: 7361 6d65 2c20 736f 2074 6861 740a 2020  same, so that.  
-0000e8b0: 2020 2020 2020 2320 6d6f 6465 6c20 6361        # model ca
-0000e8c0: 6e20 6265 2069 6e74 6572 7072 6574 7465  n be interprette
-0000e8d0: 6420 7072 6f70 6572 6c79 0a20 2020 2020  d properly.     
-0000e8e0: 2020 2066 6967 2e75 7064 6174 655f 7961     fig.update_ya
-0000e8f0: 7865 7328 0a20 2020 2020 2020 2020 2020  xes(.           
-0000e900: 2073 6361 6c65 616e 6368 6f72 3d22 7822   scaleanchor="x"
-0000e910: 2c0a 2020 2020 2020 2020 2020 2020 7363  ,.            sc
-0000e920: 616c 6572 6174 696f 3d31 2c0a 2020 2020  aleratio=1,.    
-0000e930: 2020 2020 290a 0a20 2020 2020 2020 2023      )..        #
-0000e940: 2064 6f6e 7420 7368 6f77 206c 6567 656e   dont show legen
-0000e950: 640a 2020 2020 2020 2020 6669 672e 7570  d.        fig.up
-0000e960: 6461 7465 5f6c 6179 6f75 7428 0a20 2020  date_layout(.   
-0000e970: 2020 2020 2020 2020 2073 686f 776c 6567           showleg
-0000e980: 656e 643d 4661 6c73 652c 0a20 2020 2020  end=False,.     
-0000e990: 2020 2029 0a0a 2020 2020 2020 2020 2320     )..        # 
-0000e9a0: 6966 2074 6865 7265 2061 7265 206e 6f20  if there are no 
-0000e9b0: 6d61 7465 7269 616c 7320 6a75 7374 2072  materials just r
-0000e9c0: 6574 7572 6e20 616e 2065 6d70 7479 2073  eturn an empty s
-0000e9d0: 6865 6c6c 0a20 2020 2020 2020 2069 6620  hell.        if 
-0000e9e0: 6e6f 7420 7365 6c66 2e5f 6d61 7465 7269  not self._materi
-0000e9f0: 616c 733a 0a20 2020 2020 2020 2020 2020  als:.           
-0000ea00: 2072 6574 7572 6e20 6669 670a 0a20 2020   return fig..   
-0000ea10: 2020 2020 2023 2067 6574 2074 6865 2070       # get the p
-0000ea20: 6f69 6e74 7320 7265 7072 6573 656e 7469  oints representi
-0000ea30: 6e67 2074 6865 2074 6f70 206c 696e 6520  ng the top line 
-0000ea40: 6f66 2074 6865 206d 6f64 656c 0a20 2020  of the model.   
-0000ea50: 2020 2020 2023 2074 6f20 6865 6c70 2077       # to help w
-0000ea60: 6974 6820 6472 6177 696e 6720 6d61 7465  ith drawing mate
-0000ea70: 7269 616c 730a 2020 2020 2020 2020 746f  rials.        to
-0000ea80: 7020 3d20 7365 6c66 2e5f 6578 7465 726e  p = self._extern
-0000ea90: 616c 5f62 6f75 6e64 6172 795b 313a 335d  al_boundary[1:3]
-0000eaa0: 0a0a 2020 2020 2020 2020 2320 6c65 6e67  ..        # leng
-0000eab0: 7468 206f 6620 6d6f 6465 6c20 286d 6178  th of model (max
-0000eac0: 2078 2063 6f6f 7264 696e 6174 6529 0a20   x coordinate). 
-0000ead0: 2020 2020 2020 2074 6f74 5f6c 203d 2073         tot_l = s
-0000eae0: 656c 662e 5f65 7874 6572 6e61 6c5f 6c65  elf._external_le
-0000eaf0: 6e67 7468 0a20 2020 2020 2020 206e 756d  ngth.        num
-0000eb00: 5f6d 6174 6572 6961 6c73 203d 206c 656e  _materials = len
-0000eb10: 2873 656c 662e 5f6d 6174 6572 6961 6c73  (self._materials
-0000eb20: 290a 0a20 2020 2020 2020 2023 206c 6f6f  )..        # loo
-0000eb30: 7020 7468 726f 7567 6820 6d61 7465 7269  p through materi
-0000eb40: 616c 730a 2020 2020 2020 2020 666f 7220  als.        for 
-0000eb50: 692c 206d 2069 6e20 656e 756d 6572 6174  i, m in enumerat
-0000eb60: 6528 7365 6c66 2e5f 6d61 7465 7269 616c  e(self._material
-0000eb70: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-0000eb80: 2320 6765 7420 7265 6665 7265 6e63 6520  # get reference 
-0000eb90: 6c65 7665 6c20 2879 2063 6f6f 7264 696e  level (y coordin
-0000eba0: 6174 6529 2066 6f72 206d 6174 6572 6961  ate) for materia
-0000ebb0: 6c0a 2020 2020 2020 2020 2020 2020 7920  l.            y 
-0000ebc0: 3d20 6d2e 524c 0a20 2020 2020 2020 2020  = m.RL.         
-0000ebd0: 2020 2078 203d 2073 656c 662e 6765 745f     x = self.get_
-0000ebe0: 6578 7465 726e 616c 5f78 5f69 6e74 6572  external_x_inter
-0000ebf0: 7365 6374 696f 6e28 7929 0a0a 2020 2020  section(y)..    
-0000ec00: 2020 2020 2020 2020 6c69 6e65 203d 205b          line = [
-0000ec10: 2830 2c20 7929 2c20 2878 2c20 7929 5d0a  (0, y), (x, y)].
-0000ec20: 0a20 2020 2020 2020 2020 2020 2023 2069  .            # i
-0000ec30: 6620 7468 6520 626f 7420 736c 6f70 6520  f the bot slope 
-0000ec40: 636f 6f72 6469 6e61 7465 2069 7320 6265  coordinate is be
-0000ec50: 7477 6565 6e20 7468 6520 626f 756e 6473  tween the bounds
-0000ec60: 206f 6620 7468 6520 6d61 7465 7269 616c   of the material
-0000ec70: 0a20 2020 2020 2020 2020 2020 2023 204f  .            # O
-0000ec80: 5220 4c41 5354 206d 6174 6572 6961 6c20  R LAST material 
-0000ec90: 616e 6420 6162 6f76 6520 6e65 6564 2074  and above need t
-0000eca0: 6f20 6472 6177 2061 2062 6974 2064 6966  o draw a bit dif
-0000ecb0: 6665 7265 6e74 6c79 0a0a 2020 2020 2020  ferently..      
-0000ecc0: 2020 2020 2020 6973 5f6c 6173 7420 3d20        is_last = 
-0000ecd0: 6920 3d3d 206e 756d 5f6d 6174 6572 6961  i == num_materia
-0000ece0: 6c73 202d 2031 0a0a 2020 2020 2020 2020  ls - 1..        
-0000ecf0: 2020 2020 6966 2028 0a20 2020 2020 2020      if (.       
-0000ed00: 2020 2020 2020 2020 2074 6f70 5b31 5d5b           top[1][
-0000ed10: 315d 203e 3d20 7365 6c66 2e5f 626f 745f  1] >= self._bot_
-0000ed20: 636f 6f72 645b 315d 2061 6e64 206c 696e  coord[1] and lin
-0000ed30: 655b 315d 5b31 5d20 3c20 7365 6c66 2e5f  e[1][1] < self._
-0000ed40: 626f 745f 636f 6f72 645b 315d 0a20 2020  bot_coord[1].   
-0000ed50: 2020 2020 2020 2020 2029 206f 7220 2869           ) or (i
-0000ed60: 735f 6c61 7374 2061 6e64 2074 6f70 5b31  s_last and top[1
-0000ed70: 5d5b 315d 203e 2073 656c 662e 5f62 6f74  ][1] > self._bot
-0000ed80: 5f63 6f6f 7264 5b31 5d29 3a0a 2020 2020  _coord[1]):.    
-0000ed90: 2020 2020 2020 2020 2020 2020 746f 702e              top.
-0000eda0: 6170 7065 6e64 2873 656c 662e 5f62 6f74  append(self._bot
-0000edb0: 5f63 6f6f 7264 290a 2020 2020 2020 2020  _coord).        
-0000edc0: 2020 2020 2020 2020 746f 702e 6170 7065          top.appe
-0000edd0: 6e64 2828 746f 745f 6c2c 2073 656c 662e  nd((tot_l, self.
-0000ede0: 5f62 6f74 5f63 6f6f 7264 5b31 5d29 290a  _bot_coord[1])).
-0000edf0: 0a20 2020 2020 2020 2020 2020 2023 2069  .            # i
-0000ee00: 6620 7765 2061 7265 2061 7420 7468 6520  f we are at the 
-0000ee10: 6c61 7374 206d 6174 6572 6961 6c20 6d61  last material ma
-0000ee20: 6b65 2074 6865 2062 6f74 746f 6d20 7468  ke the bottom th
-0000ee30: 6520 626f 7474 6f6d 206f 6620 7468 6520  e bottom of the 
-0000ee40: 6d6f 6465 6c0a 2020 2020 2020 2020 2020  model.          
-0000ee50: 2020 6966 2069 203d 3d20 6e75 6d5f 6d61    if i == num_ma
-0000ee60: 7465 7269 616c 7320 2d20 313a 0a20 2020  terials - 1:.   
-0000ee70: 2020 2020 2020 2020 2020 2020 2062 6f74               bot
-0000ee80: 203d 2073 656c 662e 5f65 7874 6572 6e61   = self._externa
-0000ee90: 6c5f 626f 756e 6461 7279 5b2d 323a 5d0a  l_boundary[-2:].
-0000eea0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0000eeb0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000eec0: 2020 626f 7420 3d20 6c69 6e65 0a0a 2020    bot = line..  
-0000eed0: 2020 2020 2020 2020 2020 2320 6368 616e            # chan
-0000eee0: 6765 2062 6f74 746f 6d20 636f 6f72 6469  ge bottom coordi
-0000eef0: 6e61 7465 7320 746f 2062 6520 7269 6768  nates to be righ
-0000ef00: 7420 746f 206c 6566 740a 2020 2020 2020  t to left.      
-0000ef10: 2020 2020 2020 2320 736f 2070 6f69 6e74        # so point
-0000ef20: 7320 6172 6520 6172 7261 6e67 6564 2063  s are arranged c
-0000ef30: 6c6f 636b 7769 7365 2069 6e20 6120 6369  lockwise in a ci
-0000ef40: 7263 6c65 0a20 2020 2020 2020 2020 2020  rcle.           
-0000ef50: 2062 6f74 203d 2073 6f72 7465 6428 626f   bot = sorted(bo
-0000ef60: 742c 2072 6576 6572 7365 3d54 7275 6529  t, reverse=True)
-0000ef70: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-0000ef80: 6765 7420 636f 6f72 6469 6e61 7465 730a  get coordinates.
-0000ef90: 2020 2020 2020 2020 2020 2020 636f 6f72              coor
-0000efa0: 6473 203d 2074 6f70 202b 2062 6f74 0a20  ds = top + bot. 
-0000efb0: 2020 2020 2020 2020 2020 2078 5f20 3d20             x_ = 
-0000efc0: 5b61 5b30 5d20 666f 7220 6120 696e 2063  [a[0] for a in c
-0000efd0: 6f6f 7264 735d 0a20 2020 2020 2020 2020  oords].         
-0000efe0: 2020 2079 5f20 3d20 5b61 5b31 5d20 666f     y_ = [a[1] fo
-0000eff0: 7220 6120 696e 2063 6f6f 7264 735d 0a0a  r a in coords]..
-0000f000: 2020 2020 2020 2020 2020 2020 6669 672e              fig.
-0000f010: 6164 645f 7472 6163 6528 0a20 2020 2020  add_trace(.     
-0000f020: 2020 2020 2020 2020 2020 2067 6f2e 5363             go.Sc
-0000f030: 6174 7465 7228 0a20 2020 2020 2020 2020  atter(.         
-0000f040: 2020 2020 2020 2020 2020 2078 3d6c 6973             x=lis
-0000f050: 7428 785f 292c 0a20 2020 2020 2020 2020  t(x_),.         
-0000f060: 2020 2020 2020 2020 2020 2079 3d6c 6973             y=lis
-0000f070: 7428 795f 292c 0a20 2020 2020 2020 2020  t(y_),.         
-0000f080: 2020 2020 2020 2020 2020 206d 6f64 653d             mode=
-0000f090: 226c 696e 6573 222c 0a20 2020 2020 2020  "lines",.       
-0000f0a0: 2020 2020 2020 2020 2020 2020 206d 6574               met
-0000f0b0: 613d 5b6d 2e75 6e69 745f 7765 6967 6874  a=[m.unit_weight
-0000f0c0: 2c20 6d2e 636f 6865 7369 6f6e 2c20 6d2e  , m.cohesion, m.
-0000f0d0: 6672 6963 7469 6f6e 5f61 6e67 6c65 2c20  friction_angle, 
-0000f0e0: 6d2e 6e61 6d65 5d2c 0a20 2020 2020 2020  m.name],.       
-0000f0f0: 2020 2020 2020 2020 2020 2020 2066 696c               fil
-0000f100: 6c3d 2274 6f73 656c 6622 2c0a 2020 2020  l="toself",.    
-0000f110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f120: 6e61 6d65 3d28 0a20 2020 2020 2020 2020  name=(.         
-0000f130: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000f140: 227b 6d2e 6e61 6d65 7d3c 6272 3e22 0a20  "{m.name}<br>". 
-0000f150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f160: 2020 2020 2020 2066 22ce b33a 207b 6d2e         f"..: {m.
-0000f170: 756e 6974 5f77 6569 6768 747d 206b 4e2f  unit_weight} kN/
-0000f180: 6d33 3c62 723e 220a 2020 2020 2020 2020  m3<br>".        
-0000f190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f1a0: 6622 633a 207b 6d2e 636f 6865 7369 6f6e  f"c: {m.cohesion
-0000f1b0: 7d20 6b50 613c 6272 3e22 0a20 2020 2020  } kPa<br>".     
-0000f1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f1d0: 2020 2066 22cf 953a 207b 6d2e 6672 6963     f"..: {m.fric
-0000f1e0: 7469 6f6e 5f61 6e67 6c65 7d20 6465 6772  tion_angle} degr
-0000f1f0: 6565 7322 0a20 2020 2020 2020 2020 2020  ees".           
-0000f200: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
-0000f210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f220: 686f 7665 7274 656d 706c 6174 653d 2222  hovertemplate=""
-0000f230: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000f240: 2020 2020 2020 6669 6c6c 636f 6c6f 723d        fillcolor=
-0000f250: 6d2e 636f 6c6f 722c 0a20 2020 2020 2020  m.color,.       
-0000f260: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000f270: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-0000f280: 2020 2020 2020 2320 7365 7420 7468 6520        # set the 
-0000f290: 6e65 7720 746f 7020 6173 2074 6865 2062  new top as the b
-0000f2a0: 6f74 746f 6d2c 2073 6f72 7420 746f 2070  ottom, sort to p
-0000f2b0: 7574 2069 7420 6261 636b 0a20 2020 2020  ut it back.     
-0000f2c0: 2020 2020 2020 2023 2074 6f20 6c65 6674         # to left
-0000f2d0: 2074 6f20 7269 6768 7420 6f72 6465 720a   to right order.
-0000f2e0: 2020 2020 2020 2020 2020 2020 626f 742e              bot.
-0000f2f0: 736f 7274 2829 0a20 2020 2020 2020 2020  sort().         
-0000f300: 2020 2074 6f70 203d 2062 6f74 0a0a 2020     top = bot..  
-0000f310: 2020 2020 2020 6966 206d 6174 6572 6961        if materia
-0000f320: 6c5f 7461 626c 653a 0a20 2020 2020 2020  l_table:.       
-0000f330: 2020 2020 2066 6967 203d 2073 656c 662e       fig = self.
-0000f340: 5f70 6c6f 745f 6d61 7465 7269 616c 5f74  _plot_material_t
-0000f350: 6162 6c65 2866 6967 290a 0a20 2020 2020  able(fig)..     
-0000f360: 2020 2069 6620 6c65 6765 6e64 3a0a 2020     if legend:.  
-0000f370: 2020 2020 2020 2020 2020 6669 6720 3d20            fig = 
-0000f380: 7365 6c66 2e5f 706c 6f74 5f46 4f53 5f6c  self._plot_FOS_l
-0000f390: 6567 656e 6428 6669 6729 0a0a 2020 2020  egend(fig)..    
-0000f3a0: 2020 2020 666f 7220 7564 6c20 696e 2073      for udl in s
-0000f3b0: 656c 662e 5f75 646c 733a 0a20 2020 2020  elf._udls:.     
-0000f3c0: 2020 2020 2020 2066 6967 203d 2073 656c         fig = sel
-0000f3d0: 662e 5f70 6c6f 745f 7564 6c28 6669 672c  f._plot_udl(fig,
-0000f3e0: 2075 646c 290a 0a20 2020 2020 2020 2066   udl)..        f
-0000f3f0: 6f72 206c 6c20 696e 2073 656c 662e 5f6c  or ll in self._l
-0000f400: 6c73 3a0a 2020 2020 2020 2020 2020 2020  ls:.            
-0000f410: 6669 6720 3d20 7365 6c66 2e5f 706c 6f74  fig = self._plot
-0000f420: 5f6c 6c28 6669 672c 206c 6c29 0a0a 2020  _ll(fig, ll)..  
-0000f430: 2020 2020 2020 6966 2073 656c 662e 5f77        if self._w
-0000f440: 6174 6572 5f52 4c3a 0a20 2020 2020 2020  ater_RL:.       
-0000f450: 2020 2020 2066 6967 203d 2073 656c 662e       fig = self.
-0000f460: 5f70 6c6f 745f 7761 7465 7228 6669 6729  _plot_water(fig)
-0000f470: 0a0a 2020 2020 2020 2020 6669 6720 3d20  ..        fig = 
-0000f480: 7365 6c66 2e5f 706c 6f74 5f6c 696d 6974  self._plot_limit
-0000f490: 7328 6669 6729 0a0a 2020 2020 2020 2020  s(fig)..        
-0000f4a0: 7265 7475 726e 2066 6967 0a0a 2020 2020  return fig..    
-0000f4b0: 6465 6620 706c 6f74 5f63 7269 7469 6361  def plot_critica
-0000f4c0: 6c28 7365 6c66 2c20 6d61 7465 7269 616c  l(self, material
-0000f4d0: 5f74 6162 6c65 3d54 7275 652c 206c 6567  _table=True, leg
-0000f4e0: 656e 643d 4661 6c73 6529 3a0a 2020 2020  end=False):.    
-0000f4f0: 2020 2020 2222 2250 6c6f 7420 6372 6974      """Plot crit
-0000f500: 6963 616c 2073 6c6f 7065 2028 692e 652e  ical slope (i.e.
-0000f510: 2073 6c6f 7065 2077 6974 6820 6c6f 7765   slope with lowe
-0000f520: 7374 2046 4f53 290a 0a20 2020 2020 2020  st FOS)..       
-0000f530: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
-0000f540: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
-0000f550: 2050 6c6f 746c 7920 6669 6775 7265 0a20   Plotly figure. 
-0000f560: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000f570: 2020 2066 6967 203d 2073 656c 662e 706c     fig = self.pl
-0000f580: 6f74 5f62 6f75 6e64 6172 7928 6d61 7465  ot_boundary(mate
-0000f590: 7269 616c 5f74 6162 6c65 3d6d 6174 6572  rial_table=mater
-0000f5a0: 6961 6c5f 7461 626c 652c 206c 6567 656e  ial_table, legen
-0000f5b0: 643d 6c65 6765 6e64 290a 0a20 2020 2020  d=legend)..     
-0000f5c0: 2020 2046 4f53 203d 2073 656c 662e 5f73     FOS = self._s
-0000f5d0: 6561 7263 685b 305d 5b22 464f 5322 5d0a  earch[0]["FOS"].
-0000f5e0: 2020 2020 2020 2020 635f 7820 3d20 7365          c_x = se
-0000f5f0: 6c66 2e5f 7365 6172 6368 5b30 5d5b 2263  lf._search[0]["c
-0000f600: 5f78 225d 0a20 2020 2020 2020 2063 5f79  _x"].        c_y
-0000f610: 203d 2073 656c 662e 5f73 6561 7263 685b   = self._search[
-0000f620: 305d 5b22 635f 7922 5d0a 2020 2020 2020  0]["c_y"].      
-0000f630: 2020 7261 6469 7573 203d 2073 656c 662e    radius = self.
-0000f640: 5f73 6561 7263 685b 305d 5b22 7261 6469  _search[0]["radi
-0000f650: 7573 225d 0a20 2020 2020 2020 206c 5f63  us"].        l_c
-0000f660: 203d 2073 656c 662e 5f73 6561 7263 685b   = self._search[
-0000f670: 305d 5b22 6c5f 6322 5d0a 2020 2020 2020  0]["l_c"].      
-0000f680: 2020 725f 6320 3d20 7365 6c66 2e5f 7365    r_c = self._se
-0000f690: 6172 6368 5b30 5d5b 2272 5f63 225d 0a0a  arch[0]["r_c"]..
-0000f6a0: 2020 2020 2020 2020 6669 6720 3d20 7365          fig = se
-0000f6b0: 6c66 2e5f 706c 6f74 5f66 6169 6c75 7265  lf._plot_failure
-0000f6c0: 5f70 6c61 6e65 280a 2020 2020 2020 2020  _plane(.        
-0000f6d0: 2020 2020 6669 672c 2063 5f78 2c20 635f      fig, c_x, c_
-0000f6e0: 792c 2072 6164 6975 732c 206c 5f63 2c20  y, radius, l_c, 
-0000f6f0: 725f 632c 2046 4f53 3d46 4f53 2c20 7368  r_c, FOS=FOS, sh
-0000f700: 6f77 5f63 656e 7465 723d 5472 7565 0a20  ow_center=True. 
-0000f710: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000f720: 2072 6574 7572 6e20 6669 670a 0a20 2020   return fig..   
-0000f730: 2064 6566 2070 6c6f 745f 616c 6c5f 706c   def plot_all_pl
-0000f740: 616e 6573 2873 656c 662c 206d 6178 5f66  anes(self, max_f
-0000f750: 6f73 3a20 666c 6f61 7420 3d20 352c 206d  os: float = 5, m
-0000f760: 6174 6572 6961 6c5f 7461 626c 653d 5472  aterial_table=Tr
-0000f770: 7565 2c20 6c65 6765 6e64 3d54 7275 6529  ue, legend=True)
-0000f780: 3a0a 2020 2020 2020 2020 2222 2270 6c6f  :.        """plo
-0000f790: 7420 6d75 6c74 6970 6c65 2066 6169 6c75  t multiple failu
-0000f7a0: 7265 2070 6c61 6e65 7320 696e 2074 6865  re planes in the
-0000f7b0: 2073 616d 6520 706c 6f74 0a0a 2020 2020   same plot..    
-0000f7c0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-0000f7d0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-0000f7e0: 2d0a 2020 2020 2020 2020 6d61 785f 666f  -.        max_fo
-0000f7f0: 7320 3a20 666c 6f61 742c 206f 7074 696f  s : float, optio
-0000f800: 6e61 6c0a 2020 2020 2020 2020 2020 2020  nal.            
-0000f810: 6d61 7869 6d75 6d20 6661 6374 6f72 206f  maximum factor o
-0000f820: 6620 7361 6665 7479 2074 6f20 6469 7370  f safety to disp
-0000f830: 6c61 7920 666f 7220 706c 616e 6573 2c0a  lay for planes,.
-0000f840: 2020 2020 2020 2020 2020 2020 6279 2064              by d
-0000f850: 6566 6175 6c74 2035 2e0a 0a20 2020 2020  efault 5...     
-0000f860: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
-0000f870: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-0000f880: 2020 2070 6c6f 746c 7920 6669 6775 7265     plotly figure
-0000f890: 0a0a 2020 2020 2020 2020 2222 220a 0a20  ..        """.. 
-0000f8a0: 2020 2020 2020 2066 6967 203d 2073 656c         fig = sel
-0000f8b0: 662e 706c 6f74 5f63 7269 7469 6361 6c28  f.plot_critical(
-0000f8c0: 6d61 7465 7269 616c 5f74 6162 6c65 3d6d  material_table=m
-0000f8d0: 6174 6572 6961 6c5f 7461 626c 652c 206c  aterial_table, l
-0000f8e0: 6567 656e 643d 6c65 6765 6e64 290a 0a20  egend=legend).. 
-0000f8f0: 2020 2020 2020 2066 6967 203d 2073 656c         fig = sel
-0000f900: 662e 5f70 6c6f 745f 464f 535f 6c65 6765  f._plot_FOS_lege
-0000f910: 6e64 2866 6967 290a 0a20 2020 2020 2020  nd(fig)..       
-0000f920: 2023 204a 4220 3230 2e30 342e 3232 202d   # JB 20.04.22 -
-0000f930: 2027 6861 636b 6564 2720 696e 746f 2068   'hacked' into h
-0000f940: 6f77 2070 6c6f 746c 7920 776f 726b 7320  ow plotly works 
-0000f950: 746f 206d 616b 6520 6661 7374 6572 0a20  to make faster. 
-0000f960: 2020 2020 2020 2023 2075 6c74 696d 6174         # ultimat
-0000f970: 656c 7920 6e6f 7420 7665 7279 2072 6561  ely not very rea
-0000f980: 6469 626c 6520 6170 7072 6f61 6368 2063  dible approach c
-0000f990: 6f6d 7061 7265 6420 746f 2074 6865 206f  ompared to the o
-0000f9a0: 6c64 2061 7070 726f 6163 680a 2020 2020  ld approach.    
-0000f9b0: 2020 2020 2320 686f 7765 7665 7220 6f6c      # however ol
-0000f9c0: 6420 6170 7072 6f61 6368 2077 6173 2074  d approach was t
-0000f9d0: 6f6f 2073 6c6f 770a 2020 2020 2020 2020  oo slow.        
-0000f9e0: 7472 6163 6573 203d 205b 5d0a 0a20 2020  traces = []..   
-0000f9f0: 2020 2020 2066 6f72 2069 2069 6e20 7471       for i in tq
-0000fa00: 646d 2873 656c 662e 5f73 6561 7263 6829  dm(self._search)
-0000fa10: 3a0a 0a20 2020 2020 2020 2020 2020 2046  :..            F
-0000fa20: 4f53 203d 2069 5b22 464f 5322 5d0a 2020  OS = i["FOS"].  
-0000fa30: 2020 2020 2020 2020 2020 6966 206d 6178            if max
-0000fa40: 5f66 6f73 2069 7320 4e6f 6e65 206f 7220  _fos is None or 
-0000fa50: 464f 5320 3c20 6d61 785f 666f 733a 0a0a  FOS < max_fos:..
-0000fa60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa70: 635f 7820 3d20 695b 2263 5f78 225d 0a20  c_x = i["c_x"]. 
-0000fa80: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000fa90: 5f79 203d 2069 5b22 635f 7922 5d0a 2020  _y = i["c_y"].  
-0000faa0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-0000fab0: 6469 7573 203d 2069 5b22 7261 6469 7573  dius = i["radius
-0000fac0: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
-0000fad0: 2020 206c 5f63 203d 2069 5b22 6c5f 6322     l_c = i["l_c"
-0000fae0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0000faf0: 2020 725f 6320 3d20 695b 2272 5f63 225d    r_c = i["r_c"]
-0000fb00: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000fb10: 2020 636f 6c6f 7220 3d20 434f 4c4f 5552    color = COLOUR
-0000fb20: 5f46 4f53 5f44 4943 545b 6d69 6e28 726f  _FOS_DICT[min(ro
-0000fb30: 756e 6428 464f 532c 2031 292c 204d 4158  und(FOS, 1), MAX
-0000fb40: 5f43 4f4c 4f55 525f 4b45 5929 5d0a 0a20  _COLOUR_KEY)].. 
-0000fb50: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000fb60: 2067 656e 6572 6174 6520 706f 696e 7473   generate points
-0000fb70: 2066 6f72 2063 6972 636c 652c 2067 656e   for circle, gen
-0000fb80: 6572 6174 6573 2070 6f69 6e74 7320 6f6e  erates points on
-0000fb90: 6c79 2061 6c6f 6e67 2062 6f74 746f 6d20  ly along bottom 
-0000fba0: 6861 6c66 206f 6620 6369 7263 6c65 0a20  half of circle. 
-0000fbb0: 2020 2020 2020 2020 2020 2020 2020 2078                 x
-0000fbc0: 2c20 7920 3d20 7574 696c 6974 6965 732e  , y = utilities.
-0000fbd0: 6765 6e65 7261 7465 5f63 6972 636c 655f  generate_circle_
-0000fbe0: 636f 6f72 6469 6e61 7465 7328 635f 782c  coordinates(c_x,
-0000fbf0: 2063 5f79 2c20 7261 6469 7573 290a 0a20   c_y, radius).. 
-0000fc00: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000fc10: 2065 6d70 7479 2076 6563 746f 7273 2066   empty vectors f
-0000fc20: 6f72 2063 6972 636c 6520 706f 696e 7473  or circle points
-0000fc30: 2074 6861 7420 7765 2077 696c 6c20 6163   that we will ac
-0000fc40: 7475 616c 6c79 2069 6e63 6c75 6465 0a20  tually include. 
-0000fc50: 2020 2020 2020 2020 2020 2020 2020 2078                 x
-0000fc60: 5f20 3d20 5b5d 0a20 2020 2020 2020 2020  _ = [].         
-0000fc70: 2020 2020 2020 2079 5f20 3d20 5b5d 0a0a         y_ = []..
-0000fc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc90: 2320 3635 206c 6f6e 6720 6c69 7374 2062  # 65 long list b
-0000fca0: 7574 2074 6865 206c 6173 7420 6861 6c66  ut the last half
-0000fcb0: 206f 6620 706f 696e 7473 2061 7265 2066   of points are f
-0000fcc0: 6f72 2074 6865 2074 6f70 2068 616c 6620  or the top half 
-0000fcd0: 6f66 0a20 2020 2020 2020 2020 2020 2020  of.             
-0000fce0: 2020 2023 2063 6972 636c 6520 616e 6420     # circle and 
-0000fcf0: 736f 2077 696c 6c20 6e65 7665 7220 6163  so will never ac
-0000fd00: 7475 616c 6c79 2062 6520 7265 7175 6972  tually be requir
-0000fd10: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
-0000fd20: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-0000fd30: 6765 286c 656e 2878 2929 3a0a 2020 2020  ge(len(x)):.    
-0000fd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd50: 2320 7820 636f 6f72 6469 6e61 7465 2073  # x coordinate s
-0000fd60: 686f 756c 6420 6265 2062 6574 7765 656e  hould be between
-0000fd70: 206c 6566 7420 616e 6420 7269 6768 740a   left and right.
-0000fd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd90: 2020 2020 2320 6e6f 7465 2066 6f72 2079      # note for y
-0000fda0: 2c20 7368 6f75 6c64 2062 6520 6c65 7373  , should be less
-0000fdb0: 2074 6861 6e20 6c65 6674 2079 2062 7574   than left y but
-0000fdc0: 2063 616e 2073 746f 6f70 0a20 2020 2020   can stoop.     
-0000fdd0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000fde0: 2062 656c 6f77 2072 6967 6874 2069 0a20   below right i. 
-0000fdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe00: 2020 2069 6620 785b 695d 203c 3d20 725f     if x[i] <= r_
-0000fe10: 635b 305d 2061 6e64 2078 5b69 5d20 3e3d  c[0] and x[i] >=
-0000fe20: 206c 5f63 5b30 5d20 616e 6420 795b 695d   l_c[0] and y[i]
-0000fe30: 203c 3d20 6c5f 635b 315d 3a0a 2020 2020   <= l_c[1]:.    
-0000fe40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe50: 2020 2020 785f 2e61 7070 656e 6428 785b      x_.append(x[
-0000fe60: 695d 290a 2020 2020 2020 2020 2020 2020  i]).            
-0000fe70: 2020 2020 2020 2020 2020 2020 795f 2e61              y_.a
-0000fe80: 7070 656e 6428 795b 695d 290a 0a20 2020  ppend(y[i])..   
-0000fe90: 2020 2020 2020 2020 2020 2020 2078 5f20               x_ 
-0000fea0: 3d20 5b6c 5f63 5b30 5d5d 202b 2078 5f20  = [l_c[0]] + x_ 
-0000feb0: 2b20 5b72 5f63 5b30 5d5d 0a20 2020 2020  + [r_c[0]].     
-0000fec0: 2020 2020 2020 2020 2020 2079 5f20 3d20             y_ = 
-0000fed0: 5b6c 5f63 5b31 5d5d 202b 2079 5f20 2b20  [l_c[1]] + y_ + 
-0000fee0: 5b72 5f63 5b31 5d5d 0a0a 2020 2020 2020  [r_c[1]]..      
-0000fef0: 2020 2020 2020 2020 2020 7472 6163 6573            traces
-0000ff00: 2e61 7070 656e 6428 0a20 2020 2020 2020  .append(.       
-0000ff10: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
-0000ff20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff30: 2020 2020 2020 2022 686f 7665 7274 656d         "hovertem
-0000ff40: 706c 6174 6522 3a20 2225 7b6d 6574 615b  plate": "%{meta[
-0000ff50: 305d 7d22 2c0a 2020 2020 2020 2020 2020  0]}",.          
-0000ff60: 2020 2020 2020 2020 2020 2020 2020 226c                "l
-0000ff70: 696e 6522 3a20 7b22 636f 6c6f 7222 3a20  ine": {"color": 
-0000ff80: 636f 6c6f 727d 2c0a 2020 2020 2020 2020  color},.        
-0000ff90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ffa0: 226d 6574 6122 3a20 5b72 6f75 6e64 2846  "meta": [round(F
-0000ffb0: 4f53 2c20 3329 5d2c 0a20 2020 2020 2020  OS, 3)],.       
-0000ffc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ffd0: 2022 6d6f 6465 223a 2022 6c69 6e65 7322   "mode": "lines"
-0000ffe0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000fff0: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
-00010000: 3a20 2222 2c0a 2020 2020 2020 2020 2020  : "",.          
-00010010: 2020 2020 2020 2020 2020 2020 2020 2278                "x
-00010020: 223a 2078 5f2c 0a20 2020 2020 2020 2020  ": x_,.         
-00010030: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00010040: 7922 3a20 795f 2c0a 2020 2020 2020 2020  y": y_,.        
-00010050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010060: 2274 7970 6522 3a20 2273 6361 7474 6572  "type": "scatter
-00010070: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00010080: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-00010090: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-000100a0: 2020 2020 7472 6163 6573 2e72 6576 6572      traces.rever
-000100b0: 7365 2829 0a0a 2020 2020 2020 2020 7465  se()..        te
-000100c0: 6d70 203d 2066 6967 2e74 6f5f 6469 6374  mp = fig.to_dict
-000100d0: 2829 0a20 2020 2020 2020 2074 656d 705b  ().        temp[
-000100e0: 2264 6174 6122 5d20 3d20 7475 706c 6528  "data"] = tuple(
-000100f0: 6c69 7374 2874 656d 705b 2264 6174 6122  list(temp["data"
-00010100: 5d29 202b 2074 7261 6365 7329 0a0a 2020  ]) + traces)..  
-00010110: 2020 2020 2020 7265 7475 726e 2067 6f2e        return go.
-00010120: 4669 6775 7265 2874 656d 7029 0a0a 2020  Figure(temp)..  
-00010130: 2020 6465 6620 5f70 6c6f 745f 616e 6e6f    def _plot_anno
-00010140: 7461 7465 5f46 4f53 280a 2020 2020 2020  tate_FOS(.      
-00010150: 2020 7365 6c66 2c20 6669 672c 2063 5f78    self, fig, c_x
-00010160: 3a20 666c 6f61 742c 2063 5f79 3a20 666c  : float, c_y: fl
-00010170: 6f61 742c 2072 6164 6975 733a 2066 6c6f  oat, radius: flo
-00010180: 6174 2c20 464f 533a 2066 6c6f 6174 0a20  at, FOS: float. 
-00010190: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
-000101a0: 2241 6e6e 6f74 6174 6520 464f 5320 6f6e  "Annotate FOS on
-000101b0: 2066 6967 7572 652e 0a0a 2020 2020 2020   figure...      
-000101c0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-000101d0: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
-000101e0: 2020 2020 2020 2020 6669 6720 3a20 706c          fig : pl
-000101f0: 6f74 6c79 2066 6967 7572 650a 2020 2020  otly figure.    
-00010200: 2020 2020 635f 7820 3a20 666c 6f61 740a      c_x : float.
-00010210: 2020 2020 2020 2020 2020 2020 6369 7263              circ
-00010220: 6c65 2063 656e 7465 7220 7820 636f 6f72  le center x coor
-00010230: 6469 6e61 7465 2e0a 2020 2020 2020 2020  dinate..        
-00010240: 635f 7920 3a20 666c 6f61 740a 2020 2020  c_y : float.    
-00010250: 2020 2020 2020 2020 6369 7263 6c65 2063          circle c
-00010260: 656e 7465 7220 7920 636f 6f72 6469 6e61  enter y coordina
-00010270: 7465 2e0a 2020 2020 2020 2020 464f 5320  te..        FOS 
-00010280: 3a20 666c 6f61 740a 2020 2020 2020 2020  : float.        
-00010290: 2020 2020 6369 7263 6c65 2066 6163 746f      circle facto
-000102a0: 7220 6f66 2073 6166 6574 7920 746f 2062  r of safety to b
-000102b0: 6520 616e 6e6f 7461 7465 6420 746f 2066  e annotated to f
-000102c0: 6967 7572 652e 0a0a 2020 2020 2020 2020  igure...        
-000102d0: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
-000102e0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-000102f0: 506c 6f74 6c79 2066 6967 7572 652e 0a20  Plotly figure.. 
-00010300: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
-00010310: 2020 2020 636f 6c6f 7220 3d20 434f 4c4f      color = COLO
-00010320: 5552 5f46 4f53 5f44 4943 545b 6d69 6e28  UR_FOS_DICT[min(
-00010330: 726f 756e 6428 464f 532c 2031 292c 204d  round(FOS, 1), M
-00010340: 4158 5f43 4f4c 4f55 525f 4b45 5929 5d0a  AX_COLOUR_KEY)].
-00010350: 0a20 2020 2020 2020 2066 6967 2e61 6464  .        fig.add
-00010360: 5f74 7261 6365 280a 2020 2020 2020 2020  _trace(.        
-00010370: 2020 2020 676f 2e53 6361 7474 6572 280a      go.Scatter(.
-00010380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010390: 783d 5b63 5f78 5d2c 0a20 2020 2020 2020  x=[c_x],.       
-000103a0: 2020 2020 2020 2020 2079 3d5b 635f 795d           y=[c_y]
-000103b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000103c0: 2020 6d6f 6465 3d22 6c69 6e65 732b 7465    mode="lines+te
-000103d0: 7874 222c 0a20 2020 2020 2020 2020 2020  xt",.           
-000103e0: 2020 2020 2074 6578 743d 5b66 227b 464f       text=[f"{FO
-000103f0: 533a 2e33 667d 225d 2c0a 2020 2020 2020  S:.3f}"],.      
-00010400: 2020 2020 2020 2020 2020 7465 7874 706f            textpo
-00010410: 7369 7469 6f6e 3d22 746f 7020 7269 6768  sition="top righ
-00010420: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
-00010430: 2020 2020 7465 7874 666f 6e74 3d64 6963      textfont=dic
-00010440: 7428 6661 6d69 6c79 3d22 7361 6e73 2073  t(family="sans s
-00010450: 6572 6966 222c 2073 697a 653d 3230 2c20  erif", size=20, 
-00010460: 636f 6c6f 723d 636f 6c6f 7229 2c0a 2020  color=color),.  
-00010470: 2020 2020 2020 2020 2020 2020 2020 6e61                na
-00010480: 6d65 3d22 222c 0a20 2020 2020 2020 2020  me="",.         
-00010490: 2020 2020 2020 2074 6578 7474 656d 706c         texttempl
-000104a0: 6174 653d 2225 7b74 6578 747d 222c 0a20  ate="%{text}",. 
-000104b0: 2020 2020 2020 2020 2020 2020 2020 2068                 h
-000104c0: 6f76 6572 7465 6d70 6c61 7465 3d66 2243  overtemplate=f"C
-000104d0: 656e 7472 653a 2028 7b63 5f78 3a2e 3366  entre: ({c_x:.3f
-000104e0: 7d2c 207b 635f 793a 2e33 667d 293c 6272  }, {c_y:.3f})<br
-000104f0: 3e52 6164 6975 733a 207b 7261 6469 7573  >Radius: {radius
-00010500: 3a2e 3366 7d3c 6272 3e46 4f53 3a20 7b46  :.3f}<br>FOS: {F
-00010510: 4f53 3a2e 3366 7d22 2c0a 2020 2020 2020  OS:.3f}",.      
-00010520: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00010530: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00010540: 6e20 6669 670a 0a20 2020 2064 6566 205f  n fig..    def _
-00010550: 706c 6f74 5f77 6174 6572 2873 656c 662c  plot_water(self,
-00010560: 2066 6967 293a 0a20 2020 2020 2020 2022   fig):.        "
-00010570: 2222 4164 6420 7761 7465 7220 7461 626c  ""Add water tabl
-00010580: 6520 746f 2070 6c6f 7422 2222 0a0a 2020  e to plot"""..  
-00010590: 2020 2020 2020 6966 2073 656c 662e 5f77        if self._w
-000105a0: 6174 6572 5f52 4c20 6973 204e 6f6e 653a  ater_RL is None:
-000105b0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000105c0: 7572 6e20 6669 670a 0a20 2020 2020 2020  urn fig..       
-000105d0: 2079 203d 2073 656c 662e 5f77 6174 6572   y = self._water
-000105e0: 5f52 4c0a 2020 2020 2020 2020 7820 3d20  _RL.        x = 
-000105f0: 7365 6c66 2e67 6574 5f65 7874 6572 6e61  self.get_externa
-00010600: 6c5f 785f 696e 7465 7273 6563 7469 6f6e  l_x_intersection
-00010610: 2879 290a 0a20 2020 2020 2020 2078 5f6c  (y)..        x_l
-00010620: 696e 6520 3d20 5b30 2c20 785d 0a20 2020  ine = [0, x].   
-00010630: 2020 2020 2079 5f6c 696e 6520 3d20 5b79       y_line = [y
-00010640: 2c20 795d 0a0a 2020 2020 2020 2020 2320  , y]..        # 
-00010650: 6966 2078 2069 7320 6c65 7373 2074 6861  if x is less tha
-00010660: 6e20 626f 7420 736c 6f70 6520 7468 656e  n bot slope then
-00010670: 2069 7320 616c 736f 2073 616d 6520 6173   is also same as
-00010680: 2073 6179 696e 6720 7820 6973 206c 6573   saying x is les
-00010690: 7320 7468 616e 2074 6865 2065 6467 6520  s than the edge 
-000106a0: 6f66 2074 6865 206d 6f64 656c 2e0a 2020  of the model..  
-000106b0: 2020 2020 2020 2320 6261 7369 6361 6c6c        # basicall
-000106c0: 7920 6e65 6564 2074 6f20 6d61 6b65 2073  y need to make s
-000106d0: 7572 6520 7468 6520 7761 7465 7220 7461  ure the water ta
-000106e0: 626c 6520 636f 6e74 696e 7565 7320 616c  ble continues al
-000106f0: 6f6e 6720 7468 6520 7375 7266 6163 650a  ong the surface.
-00010700: 2020 2020 2020 2020 2320 6173 2069 7320          # as is 
-00010710: 636f 6e73 6572 7661 7469 7665 6c79 2063  conservatively c
-00010720: 6f6e 7369 6465 7265 6420 696e 2074 6865  onsidered in the
-00010730: 206d 6f64 656c 0a20 2020 2020 2020 2069   model.        i
-00010740: 6620 7820 3c3d 2073 656c 662e 5f62 6f74  f x <= self._bot
-00010750: 5f63 6f6f 7264 5b30 5d3a 0a20 2020 2020  _coord[0]:.     
-00010760: 2020 2020 2020 2078 5f6c 696e 6520 2b3d         x_line +=
-00010770: 205b 7365 6c66 2e5f 626f 745f 636f 6f72   [self._bot_coor
-00010780: 645b 305d 2c20 7365 6c66 2e5f 6578 7465  d[0], self._exte
-00010790: 726e 616c 5f6c 656e 6774 685d 0a20 2020  rnal_length].   
-000107a0: 2020 2020 2020 2020 2079 5f6c 696e 6520           y_line 
-000107b0: 2b3d 205b 7365 6c66 2e5f 626f 745f 636f  += [self._bot_co
-000107c0: 6f72 645b 315d 2c20 7365 6c66 2e5f 626f  ord[1], self._bo
-000107d0: 745f 636f 6f72 645b 315d 5d0a 0a20 2020  t_coord[1]]..   
-000107e0: 2020 2020 2066 6967 2e61 6464 5f74 7261       fig.add_tra
-000107f0: 6365 280a 2020 2020 2020 2020 2020 2020  ce(.            
-00010800: 676f 2e53 6361 7474 6572 280a 2020 2020  go.Scatter(.    
-00010810: 2020 2020 2020 2020 2020 2020 783d 785f              x=x_
-00010820: 6c69 6e65 2c0a 2020 2020 2020 2020 2020  line,.          
-00010830: 2020 2020 2020 793d 795f 6c69 6e65 2c0a        y=y_line,.
-00010840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010850: 6d6f 6465 3d22 6c69 6e65 7322 2c0a 2020  mode="lines",.  
-00010860: 2020 2020 2020 2020 2020 2020 2020 6c69                li
-00010870: 6e65 5f63 6f6c 6f72 3d22 626c 7565 222c  ne_color="blue",
-00010880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010890: 206c 696e 655f 7769 6474 683d 342c 0a20   line_width=4,. 
-000108a0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-000108b0: 616d 653d 2222 2c0a 2020 2020 2020 2020  ame="",.        
-000108c0: 2020 2020 290a 2020 2020 2020 2020 290a      ).        ).
-000108d0: 0a20 2020 2020 2020 2066 6967 2e61 6464  .        fig.add
-000108e0: 5f61 6e6e 6f74 6174 696f 6e28 0a20 2020  _annotation(.   
-000108f0: 2020 2020 2020 2020 2078 3d73 656c 662e           x=self.
-00010900: 5f74 6f70 5f63 6f6f 7264 5b30 5d20 2f20  _top_coord[0] / 
-00010910: 342c 0a20 2020 2020 2020 2020 2020 2079  4,.            y
-00010920: 3d79 2c0a 2020 2020 2020 2020 2020 2020  =y,.            
-00010930: 7465 7874 3d22 e296 bc22 2c0a 2020 2020  text="...",.    
-00010940: 2020 2020 2020 2020 7368 6f77 6172 726f          showarro
-00010950: 773d 4661 6c73 652c 0a20 2020 2020 2020  w=False,.       
-00010960: 2020 2020 2079 7368 6966 743d 3130 2c0a       yshift=10,.
-00010970: 2020 2020 2020 2020 2020 2020 666f 6e74              font
-00010980: 5f73 697a 653d 3235 2c0a 2020 2020 2020  _size=25,.      
-00010990: 2020 2020 2020 666f 6e74 5f63 6f6c 6f72        font_color
-000109a0: 3d22 626c 7565 222c 0a20 2020 2020 2020  ="blue",.       
-000109b0: 2029 0a0a 2020 2020 2020 2020 6669 672e   )..        fig.
-000109c0: 6164 645f 616e 6e6f 7461 7469 6f6e 280a  add_annotation(.
-000109d0: 2020 2020 2020 2020 2020 2020 783d 7365              x=se
-000109e0: 6c66 2e5f 746f 705f 636f 6f72 645b 305d  lf._top_coord[0]
-000109f0: 202f 2034 2c0a 2020 2020 2020 2020 2020   / 4,.          
-00010a00: 2020 793d 792c 0a20 2020 2020 2020 2020    y=y,.         
-00010a10: 2020 2074 6578 743d 225f 222c 0a20 2020     text="_",.   
-00010a20: 2020 2020 2020 2020 2073 686f 7761 7272           showarr
-00010a30: 6f77 3d46 616c 7365 2c0a 2020 2020 2020  ow=False,.      
-00010a40: 2020 2020 2020 7973 6869 6674 3d32 2c0a        yshift=2,.
-00010a50: 2020 2020 2020 2020 2020 2020 666f 6e74              font
-00010a60: 5f73 697a 653d 3235 2c0a 2020 2020 2020  _size=25,.      
-00010a70: 2020 2020 2020 666f 6e74 5f63 6f6c 6f72        font_color
-00010a80: 3d22 626c 7565 222c 0a20 2020 2020 2020  ="blue",.       
-00010a90: 2029 0a0a 2020 2020 2020 2020 7265 7475   )..        retu
-00010aa0: 726e 2066 6967 0a0a 2020 2020 6465 6620  rn fig..    def 
-00010ab0: 5f70 6c6f 745f 6c69 6d69 7473 2873 656c  _plot_limits(sel
-00010ac0: 662c 2066 6967 293a 0a20 2020 2020 2020  f, fig):.       
-00010ad0: 2022 2222 4164 6420 616e 616c 7973 6973   """Add analysis
-00010ae0: 206c 696d 6974 7320 746f 2070 6c6f 7422   limits to plot"
-00010af0: 2222 0a0a 2020 2020 2020 2020 6c31 5f78  ""..        l1_x
-00010b00: 2c20 6c32 5f78 203d 2073 656c 662e 5f6c  , l2_x = self._l
-00010b10: 696d 6974 735b 305d 2c20 7365 6c66 2e5f  imits[0], self._
-00010b20: 6c69 6d69 7473 5b31 5d0a 2020 2020 2020  limits[1].      
-00010b30: 2020 7231 5f78 2c20 7232 5f78 203d 2073    r1_x, r2_x = s
-00010b40: 656c 662e 5f6c 696d 6974 735b 325d 2c20  elf._limits[2], 
-00010b50: 7365 6c66 2e5f 6c69 6d69 7473 5b33 5d0a  self._limits[3].
-00010b60: 0a20 2020 2020 2020 206c 315f 7920 3d20  .        l1_y = 
-00010b70: 7365 6c66 2e67 6574 5f65 7874 6572 6e61  self.get_externa
-00010b80: 6c5f 795f 696e 7465 7273 6563 7469 6f6e  l_y_intersection
-00010b90: 286c 315f 7829 0a20 2020 2020 2020 206c  (l1_x).        l
-00010ba0: 325f 7920 3d20 7365 6c66 2e67 6574 5f65  2_y = self.get_e
-00010bb0: 7874 6572 6e61 6c5f 795f 696e 7465 7273  xternal_y_inters
-00010bc0: 6563 7469 6f6e 286c 325f 7829 0a20 2020  ection(l2_x).   
-00010bd0: 2020 2020 2072 315f 7920 3d20 7365 6c66       r1_y = self
-00010be0: 2e67 6574 5f65 7874 6572 6e61 6c5f 795f  .get_external_y_
-00010bf0: 696e 7465 7273 6563 7469 6f6e 2872 315f  intersection(r1_
-00010c00: 7829 0a20 2020 2020 2020 2072 325f 7920  x).        r2_y 
-00010c10: 3d20 7365 6c66 2e67 6574 5f65 7874 6572  = self.get_exter
-00010c20: 6e61 6c5f 795f 696e 7465 7273 6563 7469  nal_y_intersecti
-00010c30: 6f6e 2872 325f 7829 0a0a 2020 2020 2020  on(r2_x)..      
-00010c40: 2020 706f 696e 7473 5f72 6967 6874 203d    points_right =
-00010c50: 205b 286c 315f 782c 206c 315f 7929 5d0a   [(l1_x, l1_y)].
-00010c60: 2020 2020 2020 2020 706f 696e 7473 5f6c          points_l
-00010c70: 6566 7420 3d20 5b28 7232 5f78 2c20 7232  eft = [(r2_x, r2
-00010c80: 5f79 295d 0a0a 2020 2020 2020 2020 6966  _y)]..        if
-00010c90: 2073 656c 662e 5f6c 696d 6974 735b 315d   self._limits[1]
-00010ca0: 2021 3d20 7365 6c66 2e5f 6c69 6d69 7473   != self._limits
-00010cb0: 5b32 5d3a 0a20 2020 2020 2020 2020 2020  [2]:.           
-00010cc0: 2070 6f69 6e74 735f 7269 6768 7420 2b3d   points_right +=
-00010cd0: 205b 2872 315f 782c 2072 315f 7929 5d0a   [(r1_x, r1_y)].
-00010ce0: 2020 2020 2020 2020 2020 2020 706f 696e              poin
-00010cf0: 7473 5f6c 6566 7420 2b3d 205b 286c 325f  ts_left += [(l2_
-00010d00: 782c 206c 325f 7929 5d0a 0a20 2020 2020  x, l2_y)]..     
-00010d10: 2020 2023 2061 6464 206f 7574 6572 206c     # add outer l
-00010d20: 696d 6974 730a 2020 2020 2020 2020 666f  imits.        fo
-00010d30: 7220 7020 696e 2070 6f69 6e74 735f 7269  r p in points_ri
-00010d40: 6768 743a 0a20 2020 2020 2020 2020 2020  ght:.           
-00010d50: 2066 6967 2e61 6464 5f61 6e6e 6f74 6174   fig.add_annotat
-00010d60: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
-00010d70: 2020 2020 2078 3d70 5b30 5d2c 0a20 2020       x=p[0],.   
-00010d80: 2020 2020 2020 2020 2020 2020 2079 3d70               y=p
-00010d90: 5b31 5d2c 0a20 2020 2020 2020 2020 2020  [1],.           
-00010da0: 2020 2020 2074 6578 743d 22e2 96b6 222c       text="...",
-00010db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010dc0: 2073 686f 7761 7272 6f77 3d46 616c 7365   showarrow=False
-00010dd0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00010de0: 2020 7973 6869 6674 3d31 352c 0a20 2020    yshift=15,.   
-00010df0: 2020 2020 2020 2020 2020 2020 2078 7368               xsh
-00010e00: 6966 743d 2d31 302c 0a20 2020 2020 2020  ift=-10,.       
-00010e10: 2020 2020 2020 2020 2066 6f6e 745f 7369           font_si
-00010e20: 7a65 3d32 352c 0a20 2020 2020 2020 2020  ze=25,.         
-00010e30: 2020 2020 2020 2066 6f6e 745f 636f 6c6f         font_colo
-00010e40: 723d 2262 6c61 636b 222c 0a20 2020 2020  r="black",.     
-00010e50: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-00010e60: 2020 666f 7220 7020 696e 2070 6f69 6e74    for p in point
-00010e70: 735f 6c65 6674 3a0a 2020 2020 2020 2020  s_left:.        
-00010e80: 2020 2020 6669 672e 6164 645f 616e 6e6f      fig.add_anno
-00010e90: 7461 7469 6f6e 280a 2020 2020 2020 2020  tation(.        
-00010ea0: 2020 2020 2020 2020 783d 705b 305d 2c0a          x=p[0],.
-00010eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ec0: 793d 705b 315d 2c0a 2020 2020 2020 2020  y=p[1],.        
-00010ed0: 2020 2020 2020 2020 7465 7874 3d22 e297          text="..
-00010ee0: 8022 2c0a 2020 2020 2020 2020 2020 2020  .",.            
-00010ef0: 2020 2020 7368 6f77 6172 726f 773d 4661      showarrow=Fa
-00010f00: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
-00010f10: 2020 2020 2079 7368 6966 743d 3135 2c0a       yshift=15,.
-00010f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f30: 7873 6869 6674 3d31 302c 0a20 2020 2020  xshift=10,.     
-00010f40: 2020 2020 2020 2020 2020 2066 6f6e 745f             font_
-00010f50: 7369 7a65 3d32 352c 0a20 2020 2020 2020  size=25,.       
-00010f60: 2020 2020 2020 2020 2066 6f6e 745f 636f           font_co
-00010f70: 6c6f 723d 2262 6c61 636b 222c 0a20 2020  lor="black",.   
-00010f80: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-00010f90: 2020 2020 666f 7220 7020 696e 2070 6f69      for p in poi
-00010fa0: 6e74 735f 6c65 6674 202b 2070 6f69 6e74  nts_left + point
-00010fb0: 735f 7269 6768 743a 0a20 2020 2020 2020  s_right:.       
-00010fc0: 2020 2020 2066 6967 2e61 6464 5f61 6e6e       fig.add_ann
-00010fd0: 6f74 6174 696f 6e28 0a20 2020 2020 2020  otation(.       
-00010fe0: 2020 2020 2020 2020 2078 3d70 5b30 5d2c           x=p[0],
-00010ff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011000: 2079 3d70 5b31 5d2c 0a20 2020 2020 2020   y=p[1],.       
-00011010: 2020 2020 2020 2020 2074 6578 743d 227c           text="|
-00011020: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00011030: 2020 2073 686f 7761 7272 6f77 3d46 616c     showarrow=Fal
-00011040: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
-00011050: 2020 2020 7973 6869 6674 3d31 352c 0a20      yshift=15,. 
-00011060: 2020 2020 2020 2020 2020 2020 2020 2078                 x
-00011070: 7368 6966 743d 302c 0a20 2020 2020 2020  shift=0,.       
-00011080: 2020 2020 2020 2020 2066 6f6e 745f 7369           font_si
-00011090: 7a65 3d32 352c 0a20 2020 2020 2020 2020  ze=25,.         
-000110a0: 2020 2020 2020 2066 6f6e 745f 636f 6c6f         font_colo
-000110b0: 723d 2262 6c61 636b 222c 0a20 2020 2020  r="black",.     
-000110c0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-000110d0: 2020 7265 7475 726e 2066 6967 0a0a 2020    return fig..  
-000110e0: 2020 6465 6620 5f70 6c6f 745f 6c6c 2873    def _plot_ll(s
-000110f0: 656c 662c 2066 6967 2c20 6c6c 293a 0a20  elf, fig, ll):. 
-00011100: 2020 2020 2020 2022 2222 4164 6420 706f         """Add po
-00011110: 696e 746c 6f61 6420 746f 2070 6c6f 7422  intload to plot"
-00011120: 2222 0a0a 2020 2020 2020 2020 6669 6720  ""..        fig 
-00011130: 3d20 7574 696c 6974 6965 732e 6472 6177  = utilities.draw
-00011140: 5f61 7272 6f77 280a 2020 2020 2020 2020  _arrow(.        
-00011150: 2020 2020 6669 672c 0a20 2020 2020 2020      fig,.       
-00011160: 2020 2020 2061 6e67 6c65 3d2d 3930 2c0a       angle=-90,.
-00011170: 2020 2020 2020 2020 2020 2020 666f 7263              forc
-00011180: 653d 6c6c 2e6d 6167 6e69 7475 6465 2c0a  e=ll.magnitude,.
-00011190: 2020 2020 2020 2020 2020 2020 785f 7375              x_su
-000111a0: 703d 6c6c 2e63 6f6f 7264 2c0a 2020 2020  p=ll.coord,.    
-000111b0: 2020 2020 2020 2020 795f 7375 703d 7365          y_sup=se
-000111c0: 6c66 2e5f 746f 705f 636f 6f72 645b 315d  lf._top_coord[1]
-000111d0: 2c0a 2020 2020 2020 2020 2020 2020 636f  ,.            co
-000111e0: 6c6f 723d 2262 6c61 636b 222c 0a20 2020  lor="black",.   
-000111f0: 2020 2020 2020 2020 2061 7272 6f77 6c65           arrowle
-00011200: 6e67 7468 3d31 3530 2c0a 2020 2020 2020  ngth=150,.      
-00011210: 2020 2020 2020 7368 6f77 5f76 616c 7565        show_value
-00011220: 733d 5472 7565 2c0a 2020 2020 2020 2020  s=True,.        
-00011230: 2020 2020 7072 6563 6973 696f 6e3d 6c6c      precision=ll
-00011240: 2e70 7265 6369 7369 6f6e 2c0a 2020 2020  .precision,.    
-00011250: 2020 2020 2020 2020 756e 6974 733d 226b          units="k
-00011260: 4e2f 6d22 2c0a 2020 2020 2020 2020 2020  N/m",.          
-00011270: 2020 6172 726f 7768 6561 643d 3130 2c0a    arrowhead=10,.
-00011280: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-00011290: 2020 2066 6967 203d 2075 7469 6c69 7469     fig = utiliti
-000112a0: 6573 2e64 7261 775f 6172 726f 7728 0a20  es.draw_arrow(. 
-000112b0: 2020 2020 2020 2020 2020 2066 6967 2c0a             fig,.
-000112c0: 2020 2020 2020 2020 2020 2020 616e 676c              angl
-000112d0: 653d 2d39 302c 0a20 2020 2020 2020 2020  e=-90,.         
-000112e0: 2020 2066 6f72 6365 3d6c 6c2e 6d61 676e     force=ll.magn
-000112f0: 6974 7564 652c 0a20 2020 2020 2020 2020  itude,.         
-00011300: 2020 2078 5f73 7570 3d6c 6c2e 636f 6f72     x_sup=ll.coor
-00011310: 642c 0a20 2020 2020 2020 2020 2020 2079  d,.            y
-00011320: 5f73 7570 3d73 656c 662e 5f74 6f70 5f63  _sup=self._top_c
-00011330: 6f6f 7264 5b31 5d2c 0a20 2020 2020 2020  oord[1],.       
-00011340: 2020 2020 2063 6f6c 6f72 3d6c 6c2e 636f       color=ll.co
-00011350: 6c6f 722c 0a20 2020 2020 2020 2020 2020  lor,.           
-00011360: 2061 7272 6f77 6c65 6e67 7468 3d31 3530   arrowlength=150
-00011370: 2c0a 2020 2020 2020 2020 2020 2020 7368  ,.            sh
-00011380: 6f77 5f76 616c 7565 733d 4661 6c73 652c  ow_values=False,
-00011390: 0a20 2020 2020 2020 2020 2020 2075 6e69  .            uni
-000113a0: 7473 3d22 6b4e 2f6d 222c 0a20 2020 2020  ts="kN/m",.     
-000113b0: 2020 2020 2020 2061 7272 6f77 6865 6164         arrowhead
-000113c0: 3d31 302c 0a20 2020 2020 2020 2029 0a0a  =10,.        )..
-000113d0: 2020 2020 2020 2020 7265 7475 726e 2066          return f
-000113e0: 6967 0a0a 2020 2020 6465 6620 5f70 6c6f  ig..    def _plo
-000113f0: 745f 7564 6c28 7365 6c66 2c20 6669 672c  t_udl(self, fig,
-00011400: 2075 646c 293a 0a20 2020 2020 2020 2022   udl):.        "
-00011410: 2222 4164 6420 556e 6966 6f72 6d20 6c6f  ""Add Uniform lo
-00011420: 6164 2074 6f20 706c 6f74 2222 220a 0a20  ad to plot""".. 
-00011430: 2020 2020 2020 2066 6967 203d 2075 7469         fig = uti
-00011440: 6c69 7469 6573 2e64 7261 775f 6172 726f  lities.draw_arro
-00011450: 7728 0a20 2020 2020 2020 2020 2020 2066  w(.            f
-00011460: 6967 2c0a 2020 2020 2020 2020 2020 2020  ig,.            
-00011470: 616e 676c 653d 2d39 302c 0a20 2020 2020  angle=-90,.     
-00011480: 2020 2020 2020 2066 6f72 6365 3d75 646c         force=udl
-00011490: 2e6d 6167 6e69 7475 6465 2c0a 2020 2020  .magnitude,.    
-000114a0: 2020 2020 2020 2020 785f 7375 703d 7564          x_sup=ud
-000114b0: 6c2e 6c65 6674 2c0a 2020 2020 2020 2020  l.left,.        
-000114c0: 2020 2020 795f 7375 703d 7365 6c66 2e5f      y_sup=self._
-000114d0: 746f 705f 636f 6f72 645b 315d 2c0a 2020  top_coord[1],.  
-000114e0: 2020 2020 2020 2020 2020 636f 6c6f 723d            color=
-000114f0: 7564 6c2e 636f 6c6f 722c 0a20 2020 2020  udl.color,.     
-00011500: 2020 2020 2020 2061 7272 6f77 6c65 6e67         arrowleng
-00011510: 7468 3d31 3030 202a 2028 7564 6c2e 6d61  th=100 * (udl.ma
-00011520: 676e 6974 7564 6520 2f20 7365 6c66 2e5f  gnitude / self._
-00011530: 7564 6c5f 6d61 7829 2c0a 2020 2020 2020  udl_max),.      
-00011540: 2020 2020 2020 7368 6f77 5f76 616c 7565        show_value
-00011550: 733d 4661 6c73 652c 0a20 2020 2020 2020  s=False,.       
-00011560: 2020 2020 2075 6e69 7473 3d22 6b4e 222c       units="kN",
-00011570: 0a20 2020 2020 2020 2020 2020 2061 7272  .            arr
-00011580: 6f77 6865 6164 3d31 302c 0a20 2020 2020  owhead=10,.     
-00011590: 2020 2020 2020 2070 7265 6369 7369 6f6e         precision
-000115a0: 3d75 646c 2e70 7265 6369 7369 6f6e 2c0a  =udl.precision,.
-000115b0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-000115c0: 2020 2066 6967 203d 2075 7469 6c69 7469     fig = utiliti
-000115d0: 6573 2e64 7261 775f 6172 726f 7728 0a20  es.draw_arrow(. 
-000115e0: 2020 2020 2020 2020 2020 2066 6967 2c0a             fig,.
-000115f0: 2020 2020 2020 2020 2020 2020 616e 676c              angl
-00011600: 653d 2d39 302c 0a20 2020 2020 2020 2020  e=-90,.         
-00011610: 2020 2066 6f72 6365 3d75 646c 2e6d 6167     force=udl.mag
-00011620: 6e69 7475 6465 2c0a 2020 2020 2020 2020  nitude,.        
-00011630: 2020 2020 785f 7375 703d 2875 646c 2e6c      x_sup=(udl.l
-00011640: 6566 7420 2b20 7564 6c2e 7269 6768 7429  eft + udl.right)
-00011650: 202f 2032 2c0a 2020 2020 2020 2020 2020   / 2,.          
-00011660: 2020 795f 7375 703d 7365 6c66 2e5f 746f    y_sup=self._to
-00011670: 705f 636f 6f72 645b 315d 2c0a 2020 2020  p_coord[1],.    
-00011680: 2020 2020 2020 2020 636f 6c6f 723d 2262          color="b
-00011690: 6c61 636b 222c 0a20 2020 2020 2020 2020  lack",.         
-000116a0: 2020 2061 7272 6f77 6c65 6e67 7468 3d31     arrowlength=1
-000116b0: 3030 202a 2028 7564 6c2e 6d61 676e 6974  00 * (udl.magnit
-000116c0: 7564 6520 2f20 7365 6c66 2e5f 7564 6c5f  ude / self._udl_
-000116d0: 6d61 7829 202b 2031 302c 0a20 2020 2020  max) + 10,.     
-000116e0: 2020 2020 2020 2073 686f 775f 7661 6c75         show_valu
-000116f0: 6573 3d54 7275 652c 0a20 2020 2020 2020  es=True,.       
-00011700: 2020 2020 2070 7265 6369 7369 6f6e 3d75       precision=u
-00011710: 646c 2e70 7265 6369 7369 6f6e 2c0a 2020  dl.precision,.  
-00011720: 2020 2020 2020 2020 2020 756e 6974 733d            units=
-00011730: 226b 5061 222c 0a20 2020 2020 2020 2020  "kPa",.         
-00011740: 2020 2061 7272 6f77 6865 6164 3d30 2c0a     arrowhead=0,.
-00011750: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
-00011760: 5f77 6964 7468 3d30 2c0a 2020 2020 2020  _width=0,.      
-00011770: 2020 290a 0a20 2020 2020 2020 2066 6967    )..        fig
-00011780: 203d 2075 7469 6c69 7469 6573 2e64 7261   = utilities.dra
-00011790: 775f 6172 726f 7728 0a20 2020 2020 2020  w_arrow(.       
-000117a0: 2020 2020 2066 6967 2c0a 2020 2020 2020       fig,.      
-000117b0: 2020 2020 2020 616e 676c 653d 2d39 302c        angle=-90,
-000117c0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-000117d0: 6365 3d75 646c 2e6d 6167 6e69 7475 6465  ce=udl.magnitude
-000117e0: 2c0a 2020 2020 2020 2020 2020 2020 785f  ,.            x_
-000117f0: 7375 703d 7564 6c2e 7269 6768 742c 0a20  sup=udl.right,. 
-00011800: 2020 2020 2020 2020 2020 2079 5f73 7570             y_sup
-00011810: 3d73 656c 662e 5f74 6f70 5f63 6f6f 7264  =self._top_coord
-00011820: 5b31 5d2c 0a20 2020 2020 2020 2020 2020  [1],.           
-00011830: 2063 6f6c 6f72 3d75 646c 2e63 6f6c 6f72   color=udl.color
-00011840: 2c0a 2020 2020 2020 2020 2020 2020 6172  ,.            ar
-00011850: 726f 776c 656e 6774 683d 3130 3020 2a20  rowlength=100 * 
-00011860: 2875 646c 2e6d 6167 6e69 7475 6465 202f  (udl.magnitude /
-00011870: 2073 656c 662e 5f75 646c 5f6d 6178 292c   self._udl_max),
-00011880: 0a20 2020 2020 2020 2020 2020 2073 686f  .            sho
-00011890: 775f 7661 6c75 6573 3d46 616c 7365 2c0a  w_values=False,.
-000118a0: 2020 2020 2020 2020 2020 2020 756e 6974              unit
-000118b0: 733d 226b 4e22 2c0a 2020 2020 2020 2020  s="kN",.        
-000118c0: 2020 2020 6172 726f 7768 6561 643d 3130      arrowhead=10
-000118d0: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-000118e0: 2020 2020 2023 2044 7261 7720 696e 206c       # Draw in l
-000118f0: 696e 6520 6162 6f76 6520 6172 726f 7773  ine above arrows
-00011900: 0a20 2020 2020 2020 2079 3020 3d20 3130  .        y0 = 10
-00011910: 3020 2a20 2875 646c 2e6d 6167 6e69 7475  0 * (udl.magnitu
-00011920: 6465 202f 2073 656c 662e 5f75 646c 5f6d  de / self._udl_m
-00011930: 6178 290a 0a20 2020 2020 2020 2073 6861  ax)..        sha
-00011940: 7065 203d 2064 6963 7428 0a20 2020 2020  pe = dict(.     
-00011950: 2020 2020 2020 2074 7970 653d 226c 696e         type="lin
-00011960: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
-00011970: 7872 6566 3d22 7822 2c0a 2020 2020 2020  xref="x",.      
-00011980: 2020 2020 2020 7972 6566 3d22 7922 2c0a        yref="y",.
-00011990: 2020 2020 2020 2020 2020 2020 7830 3d75              x0=u
-000119a0: 646c 2e6c 6566 742c 0a20 2020 2020 2020  dl.left,.       
-000119b0: 2020 2020 2079 303d 7930 2c0a 2020 2020       y0=y0,.    
-000119c0: 2020 2020 2020 2020 7831 3d75 646c 2e72          x1=udl.r
-000119d0: 6967 6874 2c0a 2020 2020 2020 2020 2020  ight,.          
-000119e0: 2020 7931 3d79 302c 0a20 2020 2020 2020    y1=y0,.       
-000119f0: 2020 2020 206c 696e 655f 636f 6c6f 723d       line_color=
-00011a00: 7564 6c2e 636f 6c6f 722c 0a20 2020 2020  udl.color,.     
-00011a10: 2020 2020 2020 206c 696e 655f 7769 6474         line_widt
-00011a20: 683d 322c 0a20 2020 2020 2020 2020 2020  h=2,.           
-00011a30: 2079 7369 7a65 6d6f 6465 3d22 7069 7865   ysizemode="pixe
-00011a40: 6c22 2c0a 2020 2020 2020 2020 2020 2020  l",.            
-00011a50: 7861 6e63 686f 723d 7564 6c2e 6c65 6674  xanchor=udl.left
-00011a60: 2c0a 2020 2020 2020 2020 2020 2020 7961  ,.            ya
-00011a70: 6e63 686f 723d 7365 6c66 2e5f 746f 705f  nchor=self._top_
-00011a80: 636f 6f72 645b 315d 2c0a 2020 2020 2020  coord[1],.      
-00011a90: 2020 290a 0a20 2020 2020 2020 2066 6967    )..        fig
-00011aa0: 2e61 6464 5f73 6861 7065 2873 6861 7065  .add_shape(shape
-00011ab0: 290a 0a20 2020 2020 2020 2023 2064 7261  )..        # dra
-00011ac0: 7720 696e 2072 6563 7461 6e67 756c 6172  w in rectangular
-00011ad0: 2061 7265 610a 2020 2020 2020 2020 7368   area.        sh
-00011ae0: 6170 6520 3d20 6469 6374 280a 2020 2020  ape = dict(.    
-00011af0: 2020 2020 2020 2020 7479 7065 3d22 7265          type="re
-00011b00: 6374 222c 0a20 2020 2020 2020 2020 2020  ct",.           
-00011b10: 2078 7265 663d 2278 222c 0a20 2020 2020   xref="x",.     
-00011b20: 2020 2020 2020 2079 7265 663d 2279 222c         yref="y",
-00011b30: 0a20 2020 2020 2020 2020 2020 2078 303d  .            x0=
-00011b40: 7564 6c2e 6c65 6674 2c0a 2020 2020 2020  udl.left,.      
-00011b50: 2020 2020 2020 7930 3d30 2c0a 2020 2020        y0=0,.    
-00011b60: 2020 2020 2020 2020 7831 3d75 646c 2e72          x1=udl.r
-00011b70: 6967 6874 2c0a 2020 2020 2020 2020 2020  ight,.          
-00011b80: 2020 7931 3d79 302c 0a20 2020 2020 2020    y1=y0,.       
-00011b90: 2020 2020 2066 696c 6c63 6f6c 6f72 3d75       fillcolor=u
-00011ba0: 646c 2e63 6f6c 6f72 2c0a 2020 2020 2020  dl.color,.      
-00011bb0: 2020 2020 2020 6f70 6163 6974 793d 302e        opacity=0.
-00011bc0: 322c 0a20 2020 2020 2020 2020 2020 206c  2,.            l
-00011bd0: 696e 655f 7769 6474 683d 322c 0a20 2020  ine_width=2,.   
-00011be0: 2020 2020 2020 2020 2079 7369 7a65 6d6f           ysizemo
-00011bf0: 6465 3d22 7069 7865 6c22 2c0a 2020 2020  de="pixel",.    
-00011c00: 2020 2020 2020 2020 7861 6e63 686f 723d          xanchor=
-00011c10: 7564 6c2e 6c65 6674 2c0a 2020 2020 2020  udl.left,.      
-00011c20: 2020 2020 2020 7961 6e63 686f 723d 7365        yanchor=se
-00011c30: 6c66 2e5f 746f 705f 636f 6f72 645b 315d  lf._top_coord[1]
-00011c40: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-00011c50: 2020 2020 2066 6967 2e61 6464 5f73 6861       fig.add_sha
-00011c60: 7065 2873 6861 7065 290a 0a20 2020 2020  pe(shape)..     
-00011c70: 2020 2072 6574 7572 6e20 6669 670a 0a20     return fig.. 
-00011c80: 2020 2064 6566 205f 706c 6f74 5f6d 6174     def _plot_mat
-00011c90: 6572 6961 6c5f 7461 626c 6528 7365 6c66  erial_table(self
-00011ca0: 2c20 6669 6729 3a0a 2020 2020 2020 2020  , fig):.        
-00011cb0: 2222 2250 6c6f 7420 7461 626c 6520 6f66  """Plot table of
-00011cc0: 206d 6174 6572 6961 6c20 7072 6f70 6572   material proper
-00011cd0: 7469 6573 2222 220a 0a20 2020 2020 2020  ties"""..       
-00011ce0: 2072 6f77 5f68 203d 2030 2e30 350a 2020   row_h = 0.05.  
-00011cf0: 2020 2020 2020 7461 626c 655f 7769 6474        table_widt
-00011d00: 6820 3d20 302e 340a 2020 2020 2020 2020  h = 0.4.        
-00011d10: 7461 626c 655f 6865 6967 6874 203d 2072  table_height = r
-00011d20: 6f77 5f68 202a 2028 6c65 6e28 7365 6c66  ow_h * (len(self
-00011d30: 2e5f 6d61 7465 7269 616c 7329 202b 2031  ._materials) + 1
-00011d40: 290a 0a20 2020 2020 2020 2023 2070 6f69  )..        # poi
-00011d50: 6e74 7320 6174 2074 6865 2062 6f74 746f  nts at the botto
-00011d60: 6d20 6c65 6674 0a20 2020 2020 2020 2078  m left.        x
-00011d70: 302c 2079 3020 3d20 302e 312c 2030 2e31  0, y0 = 0.1, 0.1
-00011d80: 0a0a 2020 2020 2020 2020 2320 706f 696e  ..        # poin
-00011d90: 7473 2061 7420 7468 6520 746f 7020 7269  ts at the top ri
-00011da0: 6768 740a 2020 2020 2020 2020 7831 203d  ght.        x1 =
-00011db0: 2078 3020 2b20 7461 626c 655f 7769 6474   x0 + table_widt
-00011dc0: 680a 2020 2020 2020 2020 7931 203d 2079  h.        y1 = y
-00011dd0: 3020 2b20 7461 626c 655f 6865 6967 6874  0 + table_height
-00011de0: 0a0a 2020 2020 2020 2020 2320 6164 6420  ..        # add 
-00011df0: 6865 6164 6572 2062 6163 6b67 726f 756e  header backgroun
-00011e00: 640a 2020 2020 2020 2020 6669 672e 6164  d.        fig.ad
-00011e10: 645f 7368 6170 6528 0a20 2020 2020 2020  d_shape(.       
-00011e20: 2020 2020 2074 7970 653d 2272 6563 7422       type="rect"
-00011e30: 2c0a 2020 2020 2020 2020 2020 2020 7872  ,.            xr
-00011e40: 6566 3d22 7820 646f 6d61 696e 222c 0a20  ef="x domain",. 
-00011e50: 2020 2020 2020 2020 2020 2079 7265 663d             yref=
-00011e60: 2279 2064 6f6d 6169 6e22 2c0a 2020 2020  "y domain",.    
-00011e70: 2020 2020 2020 2020 7830 3d78 302c 0a20          x0=x0,. 
-00011e80: 2020 2020 2020 2020 2020 2078 313d 7831             x1=x1
-00011e90: 2c0a 2020 2020 2020 2020 2020 2020 7930  ,.            y0
-00011ea0: 3d79 3120 2d20 726f 775f 682c 0a20 2020  =y1 - row_h,.   
-00011eb0: 2020 2020 2020 2020 2079 313d 7931 2c0a           y1=y1,.
-00011ec0: 2020 2020 2020 2020 2020 2020 6669 6c6c              fill
-00011ed0: 636f 6c6f 723d 226c 6967 6874 6772 6579  color="lightgrey
-00011ee0: 222c 0a20 2020 2020 2020 2029 0a0a 2020  ",.        )..  
-00011ef0: 2020 2020 2020 2320 6164 6420 6261 636b        # add back
-00011f00: 6772 6f75 6e64 0a20 2020 2020 2020 2066  ground.        f
-00011f10: 6967 2e61 6464 5f73 6861 7065 280a 2020  ig.add_shape(.  
-00011f20: 2020 2020 2020 2020 2020 7479 7065 3d22            type="
-00011f30: 7265 6374 222c 0a20 2020 2020 2020 2020  rect",.         
-00011f40: 2020 2078 7265 663d 2278 2064 6f6d 6169     xref="x domai
-00011f50: 6e22 2c0a 2020 2020 2020 2020 2020 2020  n",.            
-00011f60: 7972 6566 3d22 7920 646f 6d61 696e 222c  yref="y domain",
-00011f70: 0a20 2020 2020 2020 2020 2020 2078 303d  .            x0=
-00011f80: 7830 2c0a 2020 2020 2020 2020 2020 2020  x0,.            
-00011f90: 7831 3d78 312c 0a20 2020 2020 2020 2020  x1=x1,.         
-00011fa0: 2020 2079 303d 7930 2c0a 2020 2020 2020     y0=y0,.      
-00011fb0: 2020 2020 2020 7931 3d79 3120 2d20 726f        y1=y1 - ro
-00011fc0: 775f 682c 0a20 2020 2020 2020 2020 2020  w_h,.           
-00011fd0: 2066 696c 6c63 6f6c 6f72 3d22 7768 6974   fillcolor="whit
-00011fe0: 6522 2c0a 2020 2020 2020 2020 290a 0a20  e",.        ).. 
-00011ff0: 2020 2020 2020 2023 2061 6464 2063 6f6c         # add col
-00012000: 756d 6e73 2069 6e0a 2020 2020 2020 2020  umns in.        
-00012010: 636f 6c75 6d6e 5f75 6e69 745f 706f 7369  column_unit_posi
-00012020: 7469 6f6e 7320 3d20 5b32 302c 2031 352c  tions = [20, 15,
-00012030: 2031 302c 2031 302c 2031 305d 0a20 2020   10, 10, 10].   
-00012040: 2020 2020 2063 6f6c 756d 6e5f 7265 6c5f       column_rel_
-00012050: 706f 7369 7469 6f6e 7320 3d20 5b5d 0a0a  positions = []..
-00012060: 2020 2020 2020 2020 746f 7461 6c5f 7769          total_wi
-00012070: 6474 6820 3d20 7375 6d28 636f 6c75 6d6e  dth = sum(column
-00012080: 5f75 6e69 745f 706f 7369 7469 6f6e 7329  _unit_positions)
-00012090: 0a0a 2020 2020 2020 2020 636f 6c75 6d6e  ..        column
-000120a0: 5f74 6578 745f 756e 6974 5f78 7368 6966  _text_unit_xshif
-000120b0: 7420 3d20 5b31 2c20 312c 2034 2c20 342c  t = [1, 1, 4, 4,
-000120c0: 2034 5d0a 2020 2020 2020 2020 6173 7375   4].        assu
-000120d0: 6d65 645f 6772 6170 685f 7769 6474 6820  med_graph_width 
-000120e0: 3d20 3130 3030 0a20 2020 2020 2020 2063  = 1000.        c
-000120f0: 6f6c 756d 6e5f 7265 6c5f 7873 6869 6674  olumn_rel_xshift
-00012100: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
-00012110: 2061 202f 2074 6f74 616c 5f77 6964 7468   a / total_width
-00012120: 202a 2061 7373 756d 6564 5f67 7261 7068   * assumed_graph
-00012130: 5f77 6964 7468 202a 2074 6162 6c65 5f77  _width * table_w
-00012140: 6964 7468 0a20 2020 2020 2020 2020 2020  idth.           
-00012150: 2066 6f72 2061 2069 6e20 636f 6c75 6d6e   for a in column
-00012160: 5f74 6578 745f 756e 6974 5f78 7368 6966  _text_unit_xshif
-00012170: 740a 2020 2020 2020 2020 5d0a 0a20 2020  t.        ]..   
-00012180: 2020 2020 2063 756d 5f77 6964 7468 203d       cum_width =
-00012190: 2030 0a20 2020 2020 2020 2066 6f72 2063   0.        for c
-000121a0: 6f6c 5f77 6964 7468 2069 6e20 636f 6c75  ol_width in colu
-000121b0: 6d6e 5f75 6e69 745f 706f 7369 7469 6f6e  mn_unit_position
-000121c0: 733a 0a20 2020 2020 2020 2020 2020 2023  s:.            #
-000121d0: 2067 6574 2075 6e69 7420 706f 7369 7469   get unit positi
-000121e0: 6f6e 2028 6965 2070 6f73 6974 696f 6e20  on (ie position 
-000121f0: 6173 2070 6572 6365 6e74 6167 6520 6f66  as percentage of
-00012200: 2074 6f74 616c 2077 6964 7468 290a 2020   total width).  
-00012210: 2020 2020 2020 2020 2020 636f 6c75 6d6e            column
-00012220: 5f72 656c 5f70 6f73 6974 696f 6e20 3d20  _rel_position = 
-00012230: 2863 756d 5f77 6964 7468 202b 2063 6f6c  (cum_width + col
-00012240: 5f77 6964 7468 2920 2f20 746f 7461 6c5f  _width) / total_
-00012250: 7769 6474 680a 2020 2020 2020 2020 2020  width.          
-00012260: 2020 636f 6c75 6d6e 5f72 656c 5f70 6f73    column_rel_pos
-00012270: 6974 696f 6e73 2e61 7070 656e 6428 636f  itions.append(co
-00012280: 6c75 6d6e 5f72 656c 5f70 6f73 6974 696f  lumn_rel_positio
-00012290: 6e29 0a0a 2020 2020 2020 2020 2020 2020  n)..            
-000122a0: 6375 6d5f 7769 6474 6820 2b3d 2063 6f6c  cum_width += col
-000122b0: 5f77 6964 7468 0a0a 2020 2020 2020 2020  _width..        
-000122c0: 2020 2020 2320 6164 6420 696e 2063 6f6c      # add in col
-000122d0: 756d 6e20 6261 7365 6420 6f6e 2075 6e69  umn based on uni
-000122e0: 7420 706f 7369 7469 6f6e 0a20 2020 2020  t position.     
-000122f0: 2020 2020 2020 2078 203d 2078 3020 2b20         x = x0 + 
-00012300: 636f 6c75 6d6e 5f72 656c 5f70 6f73 6974  column_rel_posit
-00012310: 696f 6e20 2a20 2874 6162 6c65 5f77 6964  ion * (table_wid
-00012320: 7468 290a 0a20 2020 2020 2020 2020 2020  th)..           
-00012330: 2066 6967 2e61 6464 5f73 6861 7065 280a   fig.add_shape(.
-00012340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012350: 7479 7065 3d22 7265 6374 222c 0a20 2020  type="rect",.   
-00012360: 2020 2020 2020 2020 2020 2020 2078 7265               xre
-00012370: 663d 2278 2064 6f6d 6169 6e22 2c0a 2020  f="x domain",.  
-00012380: 2020 2020 2020 2020 2020 2020 2020 7972                yr
-00012390: 6566 3d22 7920 646f 6d61 696e 222c 0a20  ef="y domain",. 
-000123a0: 2020 2020 2020 2020 2020 2020 2020 2078                 x
-000123b0: 303d 782c 0a20 2020 2020 2020 2020 2020  0=x,.           
-000123c0: 2020 2020 2078 313d 782c 0a20 2020 2020       x1=x,.     
-000123d0: 2020 2020 2020 2020 2020 2079 303d 7930             y0=y0
-000123e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000123f0: 2020 7931 3d79 312c 0a20 2020 2020 2020    y1=y1,.       
-00012400: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-00012410: 2320 6164 6420 696e 2068 6561 6465 7220  # add in header 
-00012420: 7465 7874 0a20 2020 2020 2020 2074 6162  text.        tab
-00012430: 6c65 5f68 6561 6465 7220 3d20 5b22 4d41  le_header = ["MA
-00012440: 5445 5249 414c 222c 2022 434f 4c4f 5222  TERIAL", "COLOR"
-00012450: 2c20 22ce b322 2c20 2263 222c 2022 cf95  , "..", "c", "..
-00012460: 225d 0a20 2020 2020 2020 2074 6162 6c65  "].        table
-00012470: 5f68 6561 6465 7220 3d20 5b22 3c62 3e22  _header = ["<b>"
-00012480: 202b 2061 202b 2022 3c2f 623e 2220 666f   + a + "</b>" fo
-00012490: 7220 6120 696e 2074 6162 6c65 5f68 6561  r a in table_hea
-000124a0: 6465 725d 0a0a 2020 2020 2020 2020 7820  der]..        x 
-000124b0: 3d20 7830 0a20 2020 2020 2020 2066 6f72  = x0.        for
-000124c0: 2069 2c20 6320 696e 2065 6e75 6d65 7261   i, c in enumera
-000124d0: 7465 2863 6f6c 756d 6e5f 7265 6c5f 706f  te(column_rel_po
-000124e0: 7369 7469 6f6e 7329 3a0a 2020 2020 2020  sitions):.      
-000124f0: 2020 2020 2020 6669 672e 6164 645f 616e        fig.add_an
-00012500: 6e6f 7461 7469 6f6e 280a 2020 2020 2020  notation(.      
-00012510: 2020 2020 2020 2020 2020 7872 6566 3d22            xref="
-00012520: 7820 646f 6d61 696e 222c 0a20 2020 2020  x domain",.     
-00012530: 2020 2020 2020 2020 2020 2079 7265 663d             yref=
-00012540: 2279 2064 6f6d 6169 6e22 2c0a 2020 2020  "y domain",.    
-00012550: 2020 2020 2020 2020 2020 2020 783d 782c              x=x,
-00012560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012570: 2079 3d79 3120 2d20 726f 775f 6820 2f20   y=y1 - row_h / 
-00012580: 322c 0a20 2020 2020 2020 2020 2020 2020  2,.             
-00012590: 2020 2074 6578 743d 7461 626c 655f 6865     text=table_he
-000125a0: 6164 6572 5b69 5d2c 0a20 2020 2020 2020  ader[i],.       
-000125b0: 2020 2020 2020 2020 2073 686f 7761 7272           showarr
-000125c0: 6f77 3d46 616c 7365 2c0a 2020 2020 2020  ow=False,.      
-000125d0: 2020 2020 2020 2020 2020 7973 6869 6674            yshift
-000125e0: 3d2d 3133 2c0a 2020 2020 2020 2020 2020  =-13,.          
-000125f0: 2020 2020 2020 7873 6869 6674 3d63 6f6c        xshift=col
-00012600: 756d 6e5f 7265 6c5f 7873 6869 6674 5b69  umn_rel_xshift[i
-00012610: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-00012620: 2020 2066 6f6e 745f 7369 7a65 3d31 332c     font_size=13,
-00012630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012640: 2066 6f6e 745f 636f 6c6f 723d 2262 6c61   font_color="bla
-00012650: 636b 222c 0a20 2020 2020 2020 2020 2020  ck",.           
-00012660: 2029 0a20 2020 2020 2020 2020 2020 2078   ).            x
-00012670: 203d 2078 3020 2b20 6320 2a20 2874 6162   = x0 + c * (tab
-00012680: 6c65 5f77 6964 7468 290a 0a20 2020 2020  le_width)..     
-00012690: 2020 2023 2061 6464 2072 6f77 730a 2020     # add rows.  
-000126a0: 2020 2020 2020 666f 7220 7220 696e 2072        for r in r
-000126b0: 616e 6765 286c 656e 2873 656c 662e 5f6d  ange(len(self._m
-000126c0: 6174 6572 6961 6c73 2929 3a0a 2020 2020  aterials)):.    
-000126d0: 2020 2020 2020 2020 7920 3d20 7931 202d          y = y1 -
-000126e0: 2072 6f77 5f68 202d 2072 202a 2072 6f77   row_h - r * row
-000126f0: 5f68 0a0a 2020 2020 2020 2020 2020 2020  _h..            
-00012700: 6669 672e 6164 645f 7368 6170 6528 0a20  fig.add_shape(. 
-00012710: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00012720: 7970 653d 2272 6563 7422 2c0a 2020 2020  ype="rect",.    
-00012730: 2020 2020 2020 2020 2020 2020 7872 6566              xref
-00012740: 3d22 7820 646f 6d61 696e 222c 0a20 2020  ="x domain",.   
-00012750: 2020 2020 2020 2020 2020 2020 2079 7265               yre
-00012760: 663d 2279 2064 6f6d 6169 6e22 2c0a 2020  f="y domain",.  
-00012770: 2020 2020 2020 2020 2020 2020 2020 7830                x0
-00012780: 3d78 302c 0a20 2020 2020 2020 2020 2020  =x0,.           
-00012790: 2020 2020 2078 313d 7831 2c0a 2020 2020       x1=x1,.    
-000127a0: 2020 2020 2020 2020 2020 2020 7930 3d79              y0=y
-000127b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000127c0: 2020 7931 3d79 2c0a 2020 2020 2020 2020    y1=y,.        
-000127d0: 2020 2020 290a 0a20 2020 2020 2020 2023      )..        #
-000127e0: 2061 6464 206d 6174 6572 6961 6c20 696e   add material in
-000127f0: 666f 0a0a 2020 2020 2020 2020 7920 3d20  fo..        y = 
-00012800: 7931 202d 2072 6f77 5f68 202f 2032 0a0a  y1 - row_h / 2..
-00012810: 2020 2020 2020 2020 666f 7220 702c 206d          for p, m
-00012820: 2069 6e20 656e 756d 6572 6174 6528 7365   in enumerate(se
-00012830: 6c66 2e5f 6d61 7465 7269 616c 7329 3a0a  lf._materials):.
-00012840: 2020 2020 2020 2020 2020 2020 7820 3d20              x = 
-00012850: 7830 0a20 2020 2020 2020 2020 2020 2079  x0.            y
-00012860: 202d 3d20 726f 775f 680a 2020 2020 2020   -= row_h.      
-00012870: 2020 2020 2020 6461 7461 203d 205b 6d2e        data = [m.
-00012880: 6e61 6d65 2c20 2272 6564 222c 206d 2e75  name, "red", m.u
-00012890: 6e69 745f 7765 6967 6874 2c20 6d2e 636f  nit_weight, m.co
-000128a0: 6865 7369 6f6e 2c20 6d2e 6672 6963 7469  hesion, m.fricti
-000128b0: 6f6e 5f61 6e67 6c65 5d0a 0a20 2020 2020  on_angle]..     
-000128c0: 2020 2020 2020 2066 6f72 2069 2c20 6320         for i, c 
-000128d0: 696e 2065 6e75 6d65 7261 7465 2863 6f6c  in enumerate(col
-000128e0: 756d 6e5f 7265 6c5f 706f 7369 7469 6f6e  umn_rel_position
-000128f0: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-00012900: 2020 2020 6966 2069 203d 3d20 313a 0a20      if i == 1:. 
-00012910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012920: 2020 2066 6967 2e61 6464 5f73 6861 7065     fig.add_shape
-00012930: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00012940: 2020 2020 2020 2020 2020 7479 7065 3d22            type="
-00012950: 7265 6374 222c 0a20 2020 2020 2020 2020  rect",.         
-00012960: 2020 2020 2020 2020 2020 2020 2020 2078                 x
-00012970: 7265 663d 2270 6170 6572 222c 0a20 2020  ref="paper",.   
-00012980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012990: 2020 2020 2079 7265 663d 2270 6170 6572       yref="paper
-000129a0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-000129b0: 2020 2020 2020 2020 2020 2078 303d 782c             x0=x,
-000129c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000129d0: 2020 2020 2020 2020 2078 313d 7830 202b           x1=x0 +
-000129e0: 2063 6f6c 756d 6e5f 7265 6c5f 706f 7369   column_rel_posi
-000129f0: 7469 6f6e 735b 315d 202a 2028 7461 626c  tions[1] * (tabl
-00012a00: 655f 7769 6474 6829 2c0a 2020 2020 2020  e_width),.      
-00012a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a20: 2020 7930 3d79 202d 2072 6f77 5f68 202f    y0=y - row_h /
-00012a30: 2032 2c0a 2020 2020 2020 2020 2020 2020   2,.            
-00012a40: 2020 2020 2020 2020 2020 2020 7931 3d79              y1=y
-00012a50: 202b 2072 6f77 5f68 202f 2032 2c0a 2020   + row_h / 2,.  
-00012a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a70: 2020 2020 2020 6669 6c6c 636f 6c6f 723d        fillcolor=
-00012a80: 6d2e 636f 6c6f 722c 0a20 2020 2020 2020  m.color,.       
-00012a90: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00012aa0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00012ab0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00012ac0: 2020 2020 2020 2020 2066 6967 2e61 6464           fig.add
-00012ad0: 5f61 6e6e 6f74 6174 696f 6e28 0a20 2020  _annotation(.   
-00012ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012af0: 2020 2020 2078 7265 663d 2278 2064 6f6d       xref="x dom
-00012b00: 6169 6e22 2c0a 2020 2020 2020 2020 2020  ain",.          
-00012b10: 2020 2020 2020 2020 2020 2020 2020 7972                yr
-00012b20: 6566 3d22 7920 646f 6d61 696e 222c 0a20  ef="y domain",. 
-00012b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b40: 2020 2020 2020 2078 3d78 2c0a 2020 2020         x=x,.    
-00012b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b60: 2020 2020 793d 792c 0a20 2020 2020 2020      y=y,.       
-00012b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b80: 2074 6578 743d 6461 7461 5b69 5d2c 0a20   text=data[i],. 
-00012b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ba0: 2020 2020 2020 2073 686f 7761 7272 6f77         showarrow
-00012bb0: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
-00012bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012bd0: 7973 6869 6674 3d2d 3133 2c0a 2020 2020  yshift=-13,.    
-00012be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012bf0: 2020 2020 7873 6869 6674 3d63 6f6c 756d      xshift=colum
-00012c00: 6e5f 7265 6c5f 7873 6869 6674 5b69 5d2c  n_rel_xshift[i],
-00012c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012c20: 2020 2020 2020 2020 2066 6f6e 745f 7369           font_si
-00012c30: 7a65 3d31 332c 0a20 2020 2020 2020 2020  ze=13,.         
-00012c40: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00012c50: 6f6e 745f 636f 6c6f 723d 2262 6c61 636b  ont_color="black
-00012c60: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00012c70: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00012c80: 2020 2020 2020 2020 2078 203d 2078 3020           x = x0 
-00012c90: 2b20 6320 2a20 2874 6162 6c65 5f77 6964  + c * (table_wid
-00012ca0: 7468 290a 0a20 2020 2020 2020 2072 6574  th)..        ret
-00012cb0: 7572 6e20 6669 670a 0a20 2020 2064 6566  urn fig..    def
-00012cc0: 205f 706c 6f74 5f46 4f53 5f6c 6567 656e   _plot_FOS_legen
-00012cd0: 6428 7365 6c66 2c20 6669 6729 3a0a 2020  d(self, fig):.  
-00012ce0: 2020 2020 2020 2222 2250 6c6f 7420 636f        """Plot co
-00012cf0: 6c6f 7220 6c65 6765 6e64 2066 6f72 2066  lor legend for f
-00012d00: 6163 746f 7220 6f66 2073 6166 6574 7920  actor of safety 
-00012d10: 636f 6c6f 7273 2222 220a 0a20 2020 2020  colors"""..     
-00012d20: 2020 2079 6920 3d20 302e 390a 2020 2020     yi = 0.9.    
-00012d30: 2020 2020 7966 203d 2030 2e35 0a0a 2020      yf = 0.5..  
-00012d40: 2020 2020 2020 7830 203d 2030 2e39 0a20        x0 = 0.9. 
-00012d50: 2020 2020 2020 2078 3120 3d20 302e 3935         x1 = 0.95
-00012d60: 0a0a 2020 2020 2020 2020 6669 672e 6164  ..        fig.ad
-00012d70: 645f 7368 6170 6528 0a20 2020 2020 2020  d_shape(.       
-00012d80: 2020 2020 2074 7970 653d 2272 6563 7422       type="rect"
-00012d90: 2c0a 2020 2020 2020 2020 2020 2020 7872  ,.            xr
-00012da0: 6566 3d22 7061 7065 7222 2c0a 2020 2020  ef="paper",.    
-00012db0: 2020 2020 2020 2020 7972 6566 3d22 7061          yref="pa
-00012dc0: 7065 7222 2c0a 2020 2020 2020 2020 2020  per",.          
-00012dd0: 2020 7830 3d78 3020 2d20 302e 3032 2c0a    x0=x0 - 0.02,.
-00012de0: 2020 2020 2020 2020 2020 2020 7831 3d78              x1=x
-00012df0: 3120 2b20 302e 3035 2c0a 2020 2020 2020  1 + 0.05,.      
-00012e00: 2020 2020 2020 7930 3d79 6920 2b20 302e        y0=yi + 0.
-00012e10: 3035 2c0a 2020 2020 2020 2020 2020 2020  05,.            
-00012e20: 7931 3d79 6620 2d20 302e 3033 2c0a 2020  y1=yf - 0.03,.  
-00012e30: 2020 2020 2020 2020 2020 6669 6c6c 636f            fillco
-00012e40: 6c6f 723d 2277 6869 7465 222c 0a20 2020  lor="white",.   
-00012e50: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-00012e60: 666f 7220 6b2c 2076 2069 6e20 434f 4c4f  for k, v in COLO
-00012e70: 5552 5f46 4f53 5f44 4943 542e 6974 656d  UR_FOS_DICT.item
-00012e80: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
-00012e90: 2066 6967 2e61 6464 5f73 6861 7065 280a   fig.add_shape(.
-00012ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012eb0: 7479 7065 3d22 7265 6374 222c 0a20 2020  type="rect",.   
-00012ec0: 2020 2020 2020 2020 2020 2020 2078 7265               xre
-00012ed0: 663d 2270 6170 6572 222c 0a20 2020 2020  f="paper",.     
-00012ee0: 2020 2020 2020 2020 2020 2079 7265 663d             yref=
-00012ef0: 2270 6170 6572 222c 0a20 2020 2020 2020  "paper",.       
-00012f00: 2020 2020 2020 2020 2078 303d 7830 2c0a           x0=x0,.
-00012f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f20: 7831 3d78 312c 0a20 2020 2020 2020 2020  x1=x1,.         
-00012f30: 2020 2020 2020 2079 303d 7969 202b 206b         y0=yi + k
-00012f40: 202a 2028 7966 202d 2079 6929 202f 204d   * (yf - yi) / M
-00012f50: 4158 5f43 4f4c 4f55 525f 4b45 592c 0a20  AX_COLOUR_KEY,. 
-00012f60: 2020 2020 2020 2020 2020 2020 2020 2079                 y
-00012f70: 313d 7969 202b 2028 6b20 2b20 302e 3129  1=yi + (k + 0.1)
-00012f80: 202a 2028 7966 202d 2079 6929 202f 204d   * (yf - yi) / M
-00012f90: 4158 5f43 4f4c 4f55 525f 4b45 592c 0a20  AX_COLOUR_KEY,. 
-00012fa0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00012fb0: 696c 6c63 6f6c 6f72 3d76 2c0a 2020 2020  illcolor=v,.    
-00012fc0: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
-00012fd0: 3d64 6963 7428 0a20 2020 2020 2020 2020  =dict(.         
-00012fe0: 2020 2020 2020 2020 2020 2063 6f6c 6f72             color
-00012ff0: 3d22 626c 6163 6b22 2c0a 2020 2020 2020  ="black",.      
-00013000: 2020 2020 2020 2020 2020 2020 2020 7769                wi
-00013010: 6474 683d 302e 322c 0a20 2020 2020 2020  dth=0.2,.       
-00013020: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
-00013030: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-00013040: 2020 2020 2020 2069 6620 726f 756e 6428         if round(
-00013050: 6b2c 2031 2920 2520 3120 3d3d 2030 3a0a  k, 1) % 1 == 0:.
-00013060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013070: 2023 2062 616e 6461 6964 2066 6978 2062   # bandaid fix b
-00013080: 6563 6175 7365 2069 2063 616e 7420 6669  ecause i cant fi
-00013090: 6775 7265 206f 7574 2077 6879 2074 6865  gure out why the
-000130a0: 2073 6361 6c65 2073 686f 7773 2077 726f   scale shows wro
-000130b0: 6e67 0a20 2020 2020 2020 2020 2020 2020  ng.             
-000130c0: 2020 2069 6620 6b20 3c20 322e 353a 0a20     if k < 2.5:. 
-000130d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000130e0: 2020 2079 203d 2066 6c6f 6174 2879 6929     y = float(yi)
-000130f0: 202b 2066 6c6f 6174 286b 202d 2030 2e31   + float(k - 0.1
-00013100: 3529 202a 2066 6c6f 6174 2879 6620 2d20  5) * float(yf - 
-00013110: 7969 2920 2f20 666c 6f61 7428 0a20 2020  yi) / float(.   
-00013120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013130: 2020 2020 204d 4158 5f43 4f4c 4f55 525f       MAX_COLOUR_
-00013140: 4b45 590a 2020 2020 2020 2020 2020 2020  KEY.            
-00013150: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00013160: 2020 2020 2020 2020 2020 656c 6966 206b            elif k
-00013170: 203e 2034 2e35 3a0a 2020 2020 2020 2020   > 4.5:.        
-00013180: 2020 2020 2020 2020 2020 2020 7920 3d20              y = 
-00013190: 666c 6f61 7428 7969 2920 2b20 666c 6f61  float(yi) + floa
-000131a0: 7428 6b29 202a 2066 6c6f 6174 2879 6620  t(k) * float(yf 
-000131b0: 2d20 7969 2920 2f20 666c 6f61 7428 4d41  - yi) / float(MA
-000131c0: 585f 434f 4c4f 5552 5f4b 4559 290a 2020  X_COLOUR_KEY).  
-000131d0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-000131e0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-000131f0: 2020 2020 2020 2020 7920 3d20 666c 6f61          y = floa
-00013200: 7428 7969 2920 2b20 666c 6f61 7428 6b20  t(yi) + float(k 
-00013210: 2b20 302e 3129 202a 2066 6c6f 6174 2879  + 0.1) * float(y
-00013220: 6620 2d20 7969 2920 2f20 666c 6f61 7428  f - yi) / float(
-00013230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013240: 2020 2020 2020 2020 204d 4158 5f43 4f4c           MAX_COL
-00013250: 4f55 525f 4b45 590a 2020 2020 2020 2020  OUR_KEY.        
-00013260: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-00013270: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00013280: 6967 2e61 6464 5f61 6e6e 6f74 6174 696f  ig.add_annotatio
-00013290: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
-000132a0: 2020 2020 2020 2078 7265 663d 2270 6170         xref="pap
-000132b0: 6572 222c 0a20 2020 2020 2020 2020 2020  er",.           
-000132c0: 2020 2020 2020 2020 2079 7265 663d 2270           yref="p
-000132d0: 6170 6572 222c 0a20 2020 2020 2020 2020  aper",.         
-000132e0: 2020 2020 2020 2020 2020 2078 3d78 312c             x=x1,
-000132f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013300: 2020 2020 2079 3d79 2c0a 2020 2020 2020       y=y,.      
-00013310: 2020 2020 2020 2020 2020 2020 2020 7465                te
-00013320: 7874 3d66 227b 6b7d 222c 0a20 2020 2020  xt=f"{k}",.     
-00013330: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00013340: 686f 7761 7272 6f77 3d46 616c 7365 2c0a  howarrow=False,.
-00013350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013360: 2020 2020 7973 6869 6674 3d30 2c0a 2020      yshift=0,.  
-00013370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013380: 2020 7873 6869 6674 3d33 372c 0a20 2020    xshift=37,.   
-00013390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000133a0: 2066 6f6e 745f 7369 7a65 3d31 362c 0a20   font_size=16,. 
-000133b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000133c0: 2020 2066 6f6e 745f 636f 6c6f 723d 2262     font_color="b
-000133d0: 6c61 636b 222c 0a20 2020 2020 2020 2020  lack",.         
-000133e0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-000133f0: 2020 2320 6164 6420 746f 7020 6465 7363    # add top desc
-00013400: 7269 7074 696f 6e0a 2020 2020 2020 2020  ription.        
-00013410: 6669 672e 6164 645f 616e 6e6f 7461 7469  fig.add_annotati
-00013420: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
-00013430: 7872 6566 3d22 7061 7065 7222 2c0a 2020  xref="paper",.  
-00013440: 2020 2020 2020 2020 2020 7972 6566 3d22            yref="
-00013450: 7061 7065 7222 2c0a 2020 2020 2020 2020  paper",.        
-00013460: 2020 2020 783d 2878 3020 2b20 7831 2920      x=(x0 + x1) 
-00013470: 2f20 322c 0a20 2020 2020 2020 2020 2020  / 2,.           
-00013480: 2079 3d79 692c 0a20 2020 2020 2020 2020   y=yi,.         
-00013490: 2020 2074 6578 743d 223c 623e 4c65 6765     text="<b>Lege
-000134a0: 6e64 3c2f 623e 222c 0a20 2020 2020 2020  nd</b>",.       
-000134b0: 2020 2020 2061 6c69 676e 3d22 6365 6e74       align="cent
-000134c0: 6572 222c 0a20 2020 2020 2020 2020 2020  er",.           
-000134d0: 2073 686f 7761 7272 6f77 3d46 616c 7365   showarrow=False
-000134e0: 2c0a 2020 2020 2020 2020 2020 2020 7973  ,.            ys
-000134f0: 6869 6674 3d33 332c 0a20 2020 2020 2020  hift=33,.       
-00013500: 2020 2020 2078 7368 6966 743d 3630 2c0a       xshift=60,.
-00013510: 2020 2020 2020 2020 2020 2020 666f 6e74              font
-00013520: 5f73 697a 653d 3230 2c0a 2020 2020 2020  _size=20,.      
-00013530: 2020 2020 2020 666f 6e74 5f63 6f6c 6f72        font_color
-00013540: 3d22 626c 6163 6b22 2c0a 2020 2020 2020  ="black",.      
-00013550: 2020 290a 0a20 2020 2020 2020 2072 6574    )..        ret
-00013560: 7572 6e20 6669 670a 0a20 2020 2064 6566  urn fig..    def
-00013570: 205f 706c 6f74 5f66 6169 6c75 7265 5f70   _plot_failure_p
-00013580: 6c61 6e65 280a 2020 2020 2020 2020 7365  lane(.        se
-00013590: 6c66 2c0a 2020 2020 2020 2020 6669 672c  lf,.        fig,
-000135a0: 0a20 2020 2020 2020 2063 5f78 3a20 666c  .        c_x: fl
-000135b0: 6f61 742c 0a20 2020 2020 2020 2063 5f79  oat,.        c_y
-000135c0: 3a20 666c 6f61 742c 0a20 2020 2020 2020  : float,.       
-000135d0: 2072 6164 6975 733a 2066 6c6f 6174 2c0a   radius: float,.
-000135e0: 2020 2020 2020 2020 6c5f 633a 2074 7570          l_c: tup
-000135f0: 6c65 2c0a 2020 2020 2020 2020 725f 633a  le,.        r_c:
-00013600: 2074 7570 6c65 2c0a 2020 2020 2020 2020   tuple,.        
-00013610: 464f 533a 2066 6c6f 6174 2c0a 2020 2020  FOS: float,.    
-00013620: 2020 2020 7368 6f77 5f63 656e 7465 723d      show_center=
-00013630: 4661 6c73 652c 0a20 2020 2029 3a0a 2020  False,.    ):.  
-00013640: 2020 2020 2020 2222 2241 6464 2066 6169        """Add fai
-00013650: 6c75 7265 2070 6c61 6e65 2074 6f20 706c  lure plane to pl
-00013660: 6f74 2e0a 0a20 2020 2020 2020 2050 6172  ot...        Par
-00013670: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
-00013680: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-00013690: 2020 2066 6967 203a 2070 6c6f 746c 7920     fig : plotly 
-000136a0: 6669 6775 7265 0a20 2020 2020 2020 2020  figure.         
-000136b0: 2020 2070 6c6f 746c 7920 6669 6775 7265     plotly figure
-000136c0: 2074 6f20 6861 7665 2069 6e66 6f72 6d61   to have informa
-000136d0: 7469 6f6e 2061 6464 6564 2074 6f2e 0a20  tion added to.. 
-000136e0: 2020 2020 2020 2063 5f78 203a 2066 6c6f         c_x : flo
-000136f0: 6174 0a20 2020 2020 2020 2020 2020 2066  at.            f
-00013700: 6169 6c75 7265 2070 6c61 6e65 2063 6972  ailure plane cir
-00013710: 636c 6520 6365 6e74 6572 2078 2063 6f6f  cle center x coo
-00013720: 7264 696e 6174 652e 0a20 2020 2020 2020  rdinate..       
-00013730: 2063 5f79 203a 2066 6c6f 6174 0a20 2020   c_y : float.   
-00013740: 2020 2020 2020 2020 2066 6169 6c75 7265           failure
-00013750: 2070 6c61 6e65 2063 6972 636c 6520 6365   plane circle ce
-00013760: 6e74 6572 2079 2063 6f6f 7264 696e 6174  nter y coordinat
-00013770: 652e 0a20 2020 2020 2020 2072 6164 6975  e..        radiu
-00013780: 7320 3a20 666c 6f61 740a 2020 2020 2020  s : float.      
-00013790: 2020 2020 2020 6661 696c 7572 6520 706c        failure pl
-000137a0: 616e 6520 6369 7263 6c65 2072 6164 6975  ane circle radiu
-000137b0: 730a 2020 2020 2020 2020 6c5f 6320 3a20  s.        l_c : 
-000137c0: 7475 706c 650a 2020 2020 2020 2020 2020  tuple.          
-000137d0: 2020 6c65 6674 2069 6e74 6572 7365 6374    left intersect
-000137e0: 696f 6e20 706f 696e 7420 6265 7477 6565  ion point betwee
-000137f0: 6e20 6661 696c 7572 6520 706c 616e 6520  n failure plane 
-00013800: 616e 6420 6578 7465 726e 616c 2062 6f75  and external bou
-00013810: 6e64 6172 792e 0a20 2020 2020 2020 2072  ndary..        r
-00013820: 5f63 203a 2074 7570 6c65 0a20 2020 2020  _c : tuple.     
-00013830: 2020 2020 2020 2072 6967 6874 2069 6e74         right int
-00013840: 6572 7365 6374 696f 6e20 706f 696e 7420  ersection point 
-00013850: 6265 7477 6565 6e20 6661 696c 7572 6520  between failure 
-00013860: 706c 616e 6520 616e 6420 6578 7465 726e  plane and extern
-00013870: 616c 2062 6f75 6e64 6172 792e 0a20 2020  al boundary..   
-00013880: 2020 2020 2046 4f53 203a 2066 6c6f 6174       FOS : float
-00013890: 0a20 2020 2020 2020 2020 2020 2046 6163  .            Fac
-000138a0: 746f 7220 6f66 2073 6166 6574 7920 6f66  tor of safety of
-000138b0: 2073 6c6f 7065 2028 7573 6564 2069 6e20   slope (used in 
-000138c0: 636f 6c6f 7269 6e67 2064 7261 776e 2066  coloring drawn f
-000138d0: 6169 6c75 7265 2070 6c61 6e65 290a 2020  ailure plane).  
-000138e0: 2020 2020 2020 7368 6f77 5f63 656e 7465        show_cente
-000138f0: 7220 3a20 626f 6f6c 2c20 6f70 7469 6f6e  r : bool, option
-00013900: 616c 0a20 2020 2020 2020 2020 2020 2049  al.            I
-00013910: 6620 7472 7565 2077 696c 6c20 7072 6f6a  f true will proj
-00013920: 6563 7420 746f 2074 6865 2063 656e 7465  ect to the cente
-00013930: 7220 6f66 2063 6972 636c 6520 616e 6420  r of circle and 
-00013940: 7368 6f77 2c20 6279 2064 6566 6175 6c74  show, by default
-00013950: 2066 616c 7365 2e0a 0a20 2020 2020 2020   false...       
-00013960: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
-00013970: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
-00013980: 2070 6c6f 746c 7920 6669 6775 7265 0a20   plotly figure. 
-00013990: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
-000139a0: 2020 2020 635f 7820 3d20 726f 756e 6428      c_x = round(
-000139b0: 635f 782c 2033 290a 2020 2020 2020 2020  c_x, 3).        
-000139c0: 635f 7920 3d20 726f 756e 6428 635f 792c  c_y = round(c_y,
-000139d0: 2033 290a 2020 2020 2020 2020 7261 6469   3).        radi
-000139e0: 7573 203d 2072 6f75 6e64 2872 6164 6975  us = round(radiu
-000139f0: 732c 2033 290a 2020 2020 2020 2020 464f  s, 3).        FO
-00013a00: 5320 3d20 726f 756e 6428 464f 532c 2033  S = round(FOS, 3
-00013a10: 290a 0a20 2020 2020 2020 2069 6620 464f  )..        if FO
-00013a20: 5320 3e20 353a 0a20 2020 2020 2020 2020  S > 5:.         
-00013a30: 2020 2063 6f6c 6f72 203d 2043 4f4c 4f55     color = COLOU
-00013a40: 525f 464f 535f 4449 4354 5b35 2e30 5d0a  R_FOS_DICT[5.0].
-00013a50: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00013a60: 2020 2020 2020 2020 2020 636f 6c6f 7220            color 
-00013a70: 3d20 434f 4c4f 5552 5f46 4f53 5f44 4943  = COLOUR_FOS_DIC
-00013a80: 545b 726f 756e 6428 464f 532c 2031 295d  T[round(FOS, 1)]
-00013a90: 0a0a 2020 2020 2020 2020 2320 6765 6e65  ..        # gene
-00013aa0: 7261 7465 2070 6f69 6e74 7320 666f 7220  rate points for 
-00013ab0: 6369 7263 6c65 0a20 2020 2020 2020 2078  circle.        x
-00013ac0: 2c20 7920 3d20 7574 696c 6974 6965 732e  , y = utilities.
-00013ad0: 6765 6e65 7261 7465 5f63 6972 636c 655f  generate_circle_
-00013ae0: 636f 6f72 6469 6e61 7465 7328 635f 782c  coordinates(c_x,
-00013af0: 2063 5f79 2c20 7261 6469 7573 290a 0a20   c_y, radius).. 
-00013b00: 2020 2020 2020 2023 2065 6d70 7479 2076         # empty v
-00013b10: 6563 746f 7273 2066 6f72 2063 6972 636c  ectors for circl
-00013b20: 6520 706f 696e 7473 2074 6861 7420 7765  e points that we
-00013b30: 2077 696c 6c20 6163 7475 616c 6c79 2069   will actually i
-00013b40: 6e63 6c75 6465 0a20 2020 2020 2020 2078  nclude.        x
-00013b50: 5f20 3d20 5b5d 0a20 2020 2020 2020 2079  _ = [].        y
-00013b60: 5f20 3d20 5b5d 0a0a 2020 2020 2020 2020  _ = []..        
-00013b70: 2320 3635 206c 6f6e 6720 6c69 7374 2062  # 65 long list b
-00013b80: 7574 2074 6865 206c 6173 7420 6861 6c66  ut the last half
-00013b90: 206f 6620 706f 696e 7473 2061 7265 2066   of points are f
-00013ba0: 6f72 2074 6865 2074 6f70 2068 616c 6620  or the top half 
-00013bb0: 6f66 0a20 2020 2020 2020 2023 2063 6972  of.        # cir
-00013bc0: 636c 6520 616e 6420 736f 2077 696c 6c20  cle and so will 
-00013bd0: 6e65 7665 7220 6163 7475 616c 6c79 2062  never actually b
-00013be0: 6520 7265 7175 6972 6564 2e0a 2020 2020  e required..    
-00013bf0: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-00013c00: 6765 286c 656e 2878 2929 3a0a 2020 2020  ge(len(x)):.    
-00013c10: 2020 2020 2020 2020 2320 7820 636f 6f72          # x coor
-00013c20: 6469 6e61 7465 2073 686f 756c 6420 6265  dinate should be
-00013c30: 2062 6574 7765 656e 206c 6566 7420 616e   between left an
-00013c40: 6420 7269 6768 740a 2020 2020 2020 2020  d right.        
-00013c50: 2020 2020 2320 6e6f 7465 2066 6f72 2079      # note for y
-00013c60: 2c20 7368 6f75 6c64 2062 6520 6c65 7373  , should be less
-00013c70: 2074 6861 6e20 6c65 6674 2079 2062 7574   than left y but
-00013c80: 2063 616e 2073 746f 6f70 0a20 2020 2020   can stoop.     
-00013c90: 2020 2020 2020 2023 2062 656c 6f77 2072         # below r
-00013ca0: 6967 6874 2069 0a20 2020 2020 2020 2020  ight i.         
-00013cb0: 2020 2069 6620 785b 695d 203c 3d20 725f     if x[i] <= r_
-00013cc0: 635b 305d 2061 6e64 2078 5b69 5d20 3e3d  c[0] and x[i] >=
-00013cd0: 206c 5f63 5b30 5d20 616e 6420 795b 695d   l_c[0] and y[i]
-00013ce0: 203c 3d20 6c5f 635b 315d 3a0a 2020 2020   <= l_c[1]:.    
-00013cf0: 2020 2020 2020 2020 2020 2020 785f 2e61              x_.a
-00013d00: 7070 656e 6428 785b 695d 290a 2020 2020  ppend(x[i]).    
-00013d10: 2020 2020 2020 2020 2020 2020 795f 2e61              y_.a
-00013d20: 7070 656e 6428 795b 695d 290a 0a20 2020  ppend(y[i])..   
-00013d30: 2020 2020 2069 6620 7368 6f77 5f63 656e       if show_cen
-00013d40: 7465 723a 0a20 2020 2020 2020 2020 2020  ter:.           
-00013d50: 2078 5f20 2b3d 205b 725f 635b 305d 2c20   x_ += [r_c[0], 
-00013d60: 635f 782c 206c 5f63 5b30 5d2c 2078 5f5b  c_x, l_c[0], x_[
-00013d70: 305d 5d0a 2020 2020 2020 2020 2020 2020  0]].            
-00013d80: 795f 202b 3d20 5b72 5f63 5b31 5d2c 2063  y_ += [r_c[1], c
-00013d90: 5f79 2c20 6c5f 635b 315d 2c20 795f 5b30  _y, l_c[1], y_[0
-00013da0: 5d5d 0a20 2020 2020 2020 2065 6c73 653a  ]].        else:
-00013db0: 0a20 2020 2020 2020 2020 2020 2078 5f20  .            x_ 
-00013dc0: 3d20 5b6c 5f63 5b30 5d5d 202b 2078 5f20  = [l_c[0]] + x_ 
-00013dd0: 2b20 5b72 5f63 5b30 5d5d 0a20 2020 2020  + [r_c[0]].     
-00013de0: 2020 2020 2020 2079 5f20 3d20 5b6c 5f63         y_ = [l_c
-00013df0: 5b31 5d5d 202b 2079 5f20 2b20 5b72 5f63  [1]] + y_ + [r_c
-00013e00: 5b31 5d5d 0a0a 2020 2020 2020 2020 2320  [1]]..        # 
-00013e10: 5448 4953 2049 5320 544f 4f20 534c 4f57  THIS IS TOO SLOW
-00013e20: 2028 696e 2065 7870 6572 696d 656e 7461   (in experimenta
-00013e30: 7469 6f6e 2074 6865 2072 6561 6c0a 2020  tion the real.  
-00013e40: 2020 2020 2020 2320 7072 6f62 6c65 6d20        # problem 
-00013e50: 6973 2077 6974 6820 706c 6f74 6c79 2c20  is with plotly, 
-00013e60: 6576 656e 2077 6974 6820 6d69 6e69 6d61  even with minima
-00013e70: 6c20 6461 7461 0a20 2020 2020 2020 2023  l data.        #
-00013e80: 2061 6464 696e 6720 6576 6572 7974 6869   adding everythi
-00013e90: 6e67 2069 6e20 6973 2073 6c6f 7729 0a20  ng in is slow). 
-00013ea0: 2020 2020 2020 2066 6967 2e61 6464 5f74         fig.add_t
-00013eb0: 7261 6365 280a 2020 2020 2020 2020 2020  race(.          
-00013ec0: 2020 676f 2e53 6361 7474 6572 280a 2020    go.Scatter(.  
-00013ed0: 2020 2020 2020 2020 2020 2020 2020 783d                x=
-00013ee0: 785f 2c0a 2020 2020 2020 2020 2020 2020  x_,.            
-00013ef0: 2020 2020 793d 795f 2c0a 2020 2020 2020      y=y_,.      
-00013f00: 2020 2020 2020 2020 2020 6d6f 6465 3d22            mode="
-00013f10: 6c69 6e65 7322 2c0a 2020 2020 2020 2020  lines",.        
-00013f20: 2020 2020 2020 2020 6c69 6e65 5f63 6f6c          line_col
-00013f30: 6f72 3d63 6f6c 6f72 2c0a 2020 2020 2020  or=color,.      
-00013f40: 2020 2020 2020 2020 2020 686f 7665 7274            hovert
-00013f50: 656d 706c 6174 653d 2222 2c0a 2020 2020  emplate="",.    
-00013f60: 2020 2020 2020 2020 2020 2020 7465 7874              text
-00013f70: 7465 6d70 6c61 7465 3d22 222c 0a20 2020  template="",.   
-00013f80: 2020 2020 2020 2020 2020 2020 206e 616d               nam
-00013f90: 653d 2222 2c0a 2020 2020 2020 2020 2020  e="",.          
-00013fa0: 2020 290a 2020 2020 2020 2020 290a 0a20    ).        ).. 
-00013fb0: 2020 2020 2020 2023 2069 6620 7368 6f77         # if show
-00013fc0: 2063 656e 7465 7220 6164 6420 616e 6e6f   center add anno
-00013fd0: 7461 7469 6f6e 2077 6974 6820 686f 7665  tation with hove
-00013fe0: 726c 6162 656c 2061 6e64 2074 6578 740a  rlabel and text.
-00013ff0: 2020 2020 2020 2020 6966 2073 686f 775f          if show_
-00014000: 6365 6e74 6572 3a0a 2020 2020 2020 2020  center:.        
-00014010: 2020 2020 6669 6720 3d20 7365 6c66 2e5f      fig = self._
-00014020: 706c 6f74 5f61 6e6e 6f74 6174 655f 464f  plot_annotate_FO
-00014030: 5328 6669 672c 2063 5f78 2c20 635f 792c  S(fig, c_x, c_y,
-00014040: 2072 6164 6975 732c 2046 4f53 290a 0a20   radius, FOS).. 
-00014050: 2020 2020 2020 2072 6574 7572 6e20 6669         return fi
-00014060: 670a 0a0a 6966 205f 5f6e 616d 655f 5f20  g...if __name__ 
-00014070: 3d3d 2022 5f5f 6d61 696e 5f5f 223a 0a0a  == "__main__":..
-00014080: 2020 2020 7320 3d20 536c 6f70 6528 6865      s = Slope(he
-00014090: 6967 6874 3d31 2c20 616e 676c 653d 4e6f  ight=1, angle=No
-000140a0: 6e65 2c20 6c65 6e67 7468 3d31 290a 0a20  ne, length=1).. 
-000140b0: 2020 206d 3120 3d20 4d61 7465 7269 616c     m1 = Material
-000140c0: 2832 302c 2033 352c 2030 2c20 302e 3529  (20, 35, 0, 0.5)
-000140d0: 0a20 2020 206d 3220 3d20 4d61 7465 7269  .    m2 = Materi
-000140e0: 616c 2832 302c 2033 352c 2032 2c20 3129  al(20, 35, 2, 1)
-000140f0: 0a20 2020 206d 3320 3d20 4d61 7465 7269  .    m3 = Materi
-00014100: 616c 2831 382c 2033 302c 2030 2c20 3529  al(18, 30, 0, 5)
-00014110: 0a0a 2020 2020 732e 7365 745f 6d61 7465  ..    s.set_mate
-00014120: 7269 616c 7328 6d31 2c20 6d32 2c20 6d33  rials(m1, m2, m3
-00014130: 290a 0a20 2020 2066 6f72 2072 2069 6e20  )..    for r in 
-00014140: 7261 6e67 6528 322c 2036 293a 0a20 2020  range(2, 6):.   
-00014150: 2020 2020 2073 2e61 6464 5f73 696e 676c       s.add_singl
-00014160: 655f 6369 7263 756c 6172 5f70 6c61 6e65  e_circular_plane
-00014170: 280a 2020 2020 2020 2020 2020 2020 635f  (.            c_
-00014180: 783d 732e 6765 745f 626f 7474 6f6d 5f63  x=s.get_bottom_c
-00014190: 6f6f 7264 696e 6174 6573 2829 5b30 5d2c  oordinates()[0],
-000141a0: 0a20 2020 2020 2020 2020 2020 2063 5f79  .            c_y
-000141b0: 3d73 2e67 6574 5f62 6f74 746f 6d5f 636f  =s.get_bottom_co
-000141c0: 6f72 6469 6e61 7465 7328 295b 315d 202b  ordinates()[1] +
-000141d0: 2032 2e35 2c0a 2020 2020 2020 2020 2020   2.5,.          
-000141e0: 2020 7261 6469 7573 3d72 2c0a 2020 2020    radius=r,.    
-000141f0: 2020 2020 290a 0a20 2020 2073 2e75 7064      )..    s.upd
-00014200: 6174 655f 616e 616c 7973 6973 5f6f 7074  ate_analysis_opt
-00014210: 696f 6e73 2873 6c69 6365 733d 3530 290a  ions(slices=50).
-00014220: 0a20 2020 2073 2e73 6574 5f77 6174 6572  .    s.set_water
-00014230: 5f74 6162 6c65 2830 2e37 290a 0a20 2020  _table(0.7)..   
-00014240: 2073 2e61 6e61 6c79 7365 5f73 6c6f 7065   s.analyse_slope
-00014250: 2829 0a0a 2020 2020 2320 7072 696e 7420  ()..    # print 
-00014260: 7468 6520 6372 6974 6963 616c 2046 4f53  the critical FOS
-00014270: 2066 6f72 2074 6865 2073 6c6f 7065 0a20   for the slope. 
-00014280: 2020 2070 7269 6e74 2822 666f 733a 222c     print("fos:",
-00014290: 2073 2e67 6574 5f6d 696e 5f46 4f53 2829   s.get_min_FOS()
-000142a0: 290a 0a20 2020 2023 2070 6c6f 7420 7468  )..    # plot th
-000142b0: 6520 6372 6974 6963 616c 2066 6169 6c75  e critical failu
-000142c0: 7265 2073 7572 6661 6365 0a20 2020 2066  re surface.    f
-000142d0: 6967 5f31 203d 2073 2e70 6c6f 745f 616c  ig_1 = s.plot_al
-000142e0: 6c5f 706c 616e 6573 286d 6178 5f66 6f73  l_planes(max_fos
-000142f0: 3d4e 6f6e 6529 0a20 2020 2066 6967 5f31  =None).    fig_1
-00014300: 2e75 7064 6174 655f 6c61 796f 7574 2877  .update_layout(w
-00014310: 6964 7468 3d31 3230 302c 2068 6569 6768  idth=1200, heigh
-00014320: 743d 3730 3029 0a20 2020 2066 6967 5f31  t=700).    fig_1
-00014330: 2e73 686f 7728 290a                      .show().
+00000070: 0a69 6d70 6f72 7420 6d75 6c74 6970 726f  .import multipro
+00000080: 6365 7373 696e 670a 0a23 2074 6869 7264  cessing..# third
+00000090: 2070 6172 7479 2069 6d70 6f72 7473 0a66   party imports.f
+000000a0: 726f 6d20 706c 6f74 6c79 2069 6d70 6f72  rom plotly impor
+000000b0: 7420 6772 6170 685f 6f62 6a65 6374 7320  t graph_objects 
+000000c0: 6173 2067 6f0a 6672 6f6d 2074 7164 6d20  as go.from tqdm 
+000000d0: 696d 706f 7274 2074 7164 6d0a 0a23 2068  import tqdm..# h
+000000e0: 6176 6520 746f 2064 6f20 7468 6973 2074  ave to do this t
+000000f0: 6f20 616c 6c6f 7720 666f 7220 7265 6c61  o allow for rela
+00000100: 7469 7665 2069 6d70 6f72 7473 0a23 2068  tive imports.# h
+00000110: 6176 6520 746f 2061 6c6c 6f77 2066 6f72  ave to allow for
+00000120: 2072 656c 6174 6976 6520 696d 706f 7274   relative import
+00000130: 7320 736f 2061 6c73 6f20 776f 726b 7320  s so also works 
+00000140: 7769 7468 2064 6a61 6e67 6f0a 0a23 2069  with django..# i
+00000150: 6620 7573 696e 6720 7468 6973 2066 696c  f using this fil
+00000160: 6520 6f72 2073 7068 696e 782c 2063 616e  e or sphinx, can
+00000170: 7420 6265 2072 656c 6174 6976 650a 6966  t be relative.if
+00000180: 205f 5f6e 616d 655f 5f20 696e 2028 225f   __name__ in ("_
+00000190: 5f6d 6169 6e5f 5f22 2c20 2270 7973 6c6f  _main__", "pyslo
+000001a0: 7065 222c 2022 5f5f 6d70 5f6d 6169 6e5f  pe", "__mp_main_
+000001b0: 5f22 293a 0a20 2020 2069 6d70 6f72 7420  _"):.    import 
+000001c0: 6461 7461 5f76 616c 6964 6174 696f 6e0a  data_validation.
+000001d0: 2020 2020 696d 706f 7274 2075 7469 6c69      import utili
+000001e0: 7469 6573 0a23 2069 6620 7275 6e6e 696e  ties.# if runnin
+000001f0: 6720 6672 6f6d 2064 6a61 6e67 6f20 6e65  g from django ne
+00000200: 6564 2074 6f20 7573 6520 7265 6c61 7469  ed to use relati
+00000210: 7665 0a65 6c73 653a 0a20 2020 2066 726f  ve.else:.    fro
+00000220: 6d20 2e20 696d 706f 7274 2064 6174 615f  m . import data_
+00000230: 7661 6c69 6461 7469 6f6e 0a20 2020 2066  validation.    f
+00000240: 726f 6d20 2e20 696d 706f 7274 2075 7469  rom . import uti
+00000250: 6c69 7469 6573 0a0a 434f 4c4f 5552 5f46  lities..COLOUR_F
+00000260: 4f53 5f44 4943 542c 204d 4154 4552 4941  OS_DICT, MATERIA
+00000270: 4c5f 434f 4c4f 5253 203d 2075 7469 6c69  L_COLORS = utili
+00000280: 7469 6573 2e43 4f4c 4f55 525f 464f 535f  ties.COLOUR_FOS_
+00000290: 4449 4354 2c20 7574 696c 6974 6965 732e  DICT, utilities.
+000002a0: 4d41 5445 5249 414c 5f43 4f4c 4f52 530a  MATERIAL_COLORS.
+000002b0: 4d41 585f 434f 4c4f 5552 5f4b 4559 203d  MAX_COLOUR_KEY =
+000002c0: 206d 6178 2843 4f4c 4f55 525f 464f 535f   max(COLOUR_FOS_
+000002d0: 4449 4354 290a 0a0a 4064 6174 6163 6c61  DICT)...@datacla
+000002e0: 7373 0a63 6c61 7373 204d 6174 6572 6961  ss.class Materia
+000002f0: 6c3a 0a20 2020 2022 2222 436c 6173 7320  l:.    """Class 
+00000300: 7265 7072 6573 656e 7469 6e67 2067 656f  representing geo
+00000310: 6c6f 6769 6361 6c20 6d61 7465 7269 616c  logical material
+00000320: 2075 6e69 742e 0a0a 2020 2020 5061 7261   unit...    Para
+00000330: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
+00000340: 2d2d 2d2d 2d0a 2020 2020 756e 6974 5f77  -----.    unit_w
+00000350: 6569 6768 7420 3a20 666c 6f61 740a 2020  eight : float.  
+00000360: 2020 2020 2020 6d61 7465 7269 616c 2075        material u
+00000370: 6e69 7420 7765 6967 6874 2069 6e20 6b4e  nit weight in kN
+00000380: 2f6d 332c 2062 7920 6465 6661 756c 7420  /m3, by default 
+00000390: 3230 0a20 2020 2066 7269 6374 696f 6e5f  20.    friction_
+000003a0: 616e 676c 653a 2069 6e74 0a20 2020 2020  angle: int.     
+000003b0: 2020 206d 6174 6572 6961 6c20 6672 6963     material fric
+000003c0: 7469 6f6e 2061 6e67 6c65 2069 6e20 6465  tion angle in de
+000003d0: 6772 6565 732c 2062 7920 6465 6661 756c  grees, by defaul
+000003e0: 7420 3335 0a20 2020 2063 6f68 6573 696f  t 35.    cohesio
+000003f0: 6e20 3a20 696e 740a 2020 2020 2020 2020  n : int.        
+00000400: 6d61 7465 7269 616c 2063 6f68 6573 696f  material cohesio
+00000410: 6e20 696e 206b 5061 2c20 6279 2064 6566  n in kPa, by def
+00000420: 6175 6c74 2032 0a20 2020 2064 6570 7468  ault 2.    depth
+00000430: 5f74 6f5f 626f 7474 6f6d 203a 2066 6c6f  _to_bottom : flo
+00000440: 6174 0a20 2020 2020 2020 2064 6570 7468  at.        depth
+00000450: 2074 6f20 7468 6520 626f 7474 6f6d 206f   to the bottom o
+00000460: 6620 7468 6520 6d61 7465 7269 616c 2073  f the material s
+00000470: 7472 6174 6120 6672 6f6d 2074 6865 2074  trata from the t
+00000480: 6f70 0a20 2020 2020 2020 206f 6620 7468  op.        of th
+00000490: 6520 736c 6f70 652c 2062 7920 6465 6661  e slope, by defa
+000004a0: 756c 7420 352e 204e 6f74 652c 206d 6174  ult 5. Note, mat
+000004b0: 6572 6961 6c73 2061 7373 6967 6e65 6420  erials assigned 
+000004c0: 746f 0a20 2020 2020 2020 2061 2073 6c6f  to.        a slo
+000004d0: 7065 206d 7573 7420 6861 7665 2061 2075  pe must have a u
+000004e0: 6e69 7175 6520 6465 7074 685f 746f 5f62  nique depth_to_b
+000004f0: 6f74 746f 6d20 6f72 2061 6e20 6572 726f  ottom or an erro
+00000500: 720a 2020 2020 2020 2020 7769 6c6c 2062  r.        will b
+00000510: 6520 7261 6973 6564 2e0a 2020 2020 6e61  e raised..    na
+00000520: 6d65 203a 2073 7472 2028 6f70 7469 6f6e  me : str (option
+00000530: 616c 290a 2020 2020 2020 2020 6e61 6d65  al).        name
+00000540: 206f 6620 7468 6520 7374 7261 7461 0a20   of the strata. 
+00000550: 2020 2063 6f6c 6f72 203a 2073 7472 2028     color : str (
+00000560: 6f70 7469 6f6e 616c 290a 2020 2020 2020  optional).      
+00000570: 2020 636f 6c6f 7220 746f 2062 6520 7573    color to be us
+00000580: 6564 2074 6f20 7265 7072 6573 656e 7420  ed to represent 
+00000590: 7468 6520 7374 7261 7461 2077 6865 6e20  the strata when 
+000005a0: 706c 6f74 7469 6e67 2e20 436f 6c6f 720a  plotting. Color.
+000005b0: 2020 2020 2020 2020 6d61 7920 6265 2070          may be p
+000005c0: 726f 7669 6465 6420 6173 2061 2073 7472  rovided as a str
+000005d0: 696e 672c 2073 7461 6e64 6172 6420 3320  ing, standard 3 
+000005e0: 6865 7820 6469 6769 7420 6f72 2036 2068  hex digit or 6 h
+000005f0: 6578 2064 6967 6974 0a20 2020 2020 2020  ex digit.       
+00000600: 2077 6562 2063 6f6d 7061 7469 626c 6520   web compatible 
+00000610: 7265 7072 6573 656e 7461 7469 6f6e 2e20  representation. 
+00000620: 4966 206e 6f74 2070 726f 7669 6465 6420  If not provided 
+00000630: 636f 6c6f 7220 6175 746f 6d61 7469 6361  color automatica
+00000640: 6c6c 790a 2020 2020 2020 2020 6173 7369  lly.        assi
+00000650: 676e 6564 2e0a 0a20 2020 2045 7861 6d70  gned...    Examp
+00000660: 6c65 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  les.    --------
+00000670: 2d2d 2d2d 0a20 2020 203e 3e3e 204d 6174  ----.    >>> Mat
+00000680: 6572 6961 6c28 3230 2c33 352c 322c 3529  erial(20,35,2,5)
+00000690: 0a20 2020 204d 6174 6572 6961 6c3a 2875  .    Material:(u
+000006a0: 773d 3230 2c70 6869 3d33 352c 633d 322c  w=20,phi=35,c=2,
+000006b0: 645f 626f 743d 3529 0a20 2020 203e 3e3e  d_bot=5).    >>>
+000006c0: 204d 6174 6572 6961 6c28 290a 2020 2020   Material().    
+000006d0: 4d61 7465 7269 616c 3a28 7577 3d32 302c  Material:(uw=20,
+000006e0: 7068 693d 3335 2c63 3d32 2c64 5f62 6f74  phi=35,c=2,d_bot
+000006f0: 3d35 290a 2020 2020 3e3e 3e20 6120 3d20  =5).    >>> a = 
+00000700: 4d61 7465 7269 616c 2829 0a20 2020 203e  Material().    >
+00000710: 3e3e 2061 2e63 6f68 6573 696f 6e20 3d3d  >> a.cohesion ==
+00000720: 2032 0a20 2020 2054 7275 650a 0a0a 2020   2.    True...  
+00000730: 2020 2222 220a 0a20 2020 2075 6e69 745f    """..    unit_
+00000740: 7765 6967 6874 3a20 666c 6f61 7420 3d20  weight: float = 
+00000750: 3230 0a20 2020 2066 7269 6374 696f 6e5f  20.    friction_
+00000760: 616e 676c 653a 2069 6e74 203d 2033 350a  angle: int = 35.
+00000770: 2020 2020 636f 6865 7369 6f6e 3a20 696e      cohesion: in
+00000780: 7420 3d20 320a 2020 2020 6465 7074 685f  t = 2.    depth_
+00000790: 746f 5f62 6f74 746f 6d3a 2066 6c6f 6174  to_bottom: float
+000007a0: 203d 2035 0a20 2020 206e 616d 653a 2073   = 5.    name: s
+000007b0: 7472 203d 2022 220a 2020 2020 636f 6c6f  tr = "".    colo
+000007c0: 723a 2073 7472 203d 2022 220a 0a20 2020  r: str = ""..   
+000007d0: 2064 6566 205f 5f70 6f73 745f 696e 6974   def __post_init
+000007e0: 5f5f 2873 656c 6629 3a0a 2020 2020 2020  __(self):.      
+000007f0: 2020 6461 7461 5f76 616c 6964 6174 696f    data_validatio
+00000800: 6e2e 6173 7365 7274 5f72 616e 6765 2873  n.assert_range(s
+00000810: 656c 662e 756e 6974 5f77 6569 6768 742c  elf.unit_weight,
+00000820: 2022 756e 6974 2077 6569 6768 7422 2c20   "unit weight", 
+00000830: 312c 2035 3029 0a20 2020 2020 2020 2064  1, 50).        d
+00000840: 6174 615f 7661 6c69 6461 7469 6f6e 2e61  ata_validation.a
+00000850: 7373 6572 745f 706f 7369 7469 7665 5f6e  ssert_positive_n
+00000860: 756d 6265 7228 7365 6c66 2e66 7269 6374  umber(self.frict
+00000870: 696f 6e5f 616e 676c 652c 2022 6672 6963  ion_angle, "fric
+00000880: 7469 6f6e 5f61 6e67 6c65 2229 0a20 2020  tion_angle").   
+00000890: 2020 2020 2064 6174 615f 7661 6c69 6461       data_valida
+000008a0: 7469 6f6e 2e61 7373 6572 745f 6e75 6d62  tion.assert_numb
+000008b0: 6572 2873 656c 662e 636f 6865 7369 6f6e  er(self.cohesion
+000008c0: 2c20 2263 6f68 6573 696f 6e22 290a 2020  , "cohesion").  
+000008d0: 2020 2020 2020 6461 7461 5f76 616c 6964        data_valid
+000008e0: 6174 696f 6e2e 6173 7365 7274 5f6e 756d  ation.assert_num
+000008f0: 6265 7228 7365 6c66 2e64 6570 7468 5f74  ber(self.depth_t
+00000900: 6f5f 626f 7474 6f6d 2c20 2264 6570 7468  o_bottom, "depth
+00000910: 2074 6f20 626f 7474 6f6d 2229 0a0a 2020   to bottom")..  
+00000920: 2020 2020 2020 2320 6966 2075 7365 7220        # if user 
+00000930: 6769 7665 7320 6120 6e65 6761 7469 7665  gives a negative
+00000940: 2076 616c 7565 206a 7573 7420 6d61 6b65   value just make
+00000950: 2069 7420 706f 7369 7469 7665 2069 6e73   it positive ins
+00000960: 7465 6164 2e0a 2020 2020 2020 2020 7365  tead..        se
+00000970: 6c66 2e63 6f68 6573 696f 6e20 3d20 6162  lf.cohesion = ab
+00000980: 7328 7365 6c66 2e63 6f68 6573 696f 6e29  s(self.cohesion)
+00000990: 0a20 2020 2020 2020 2073 656c 662e 6465  .        self.de
+000009a0: 7074 685f 746f 5f62 6f74 746f 6d20 3d20  pth_to_bottom = 
+000009b0: 6162 7328 7365 6c66 2e64 6570 7468 5f74  abs(self.depth_t
+000009c0: 6f5f 626f 7474 6f6d 290a 0a20 2020 2020  o_bottom)..     
+000009d0: 2020 2069 6620 7365 6c66 2e6e 616d 6520     if self.name 
+000009e0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+000009f0: 2020 2020 2073 656c 662e 6e61 6d65 203d       self.name =
+00000a00: 2022 220a 2020 2020 2020 2020 6966 2073   "".        if s
+00000a10: 656c 662e 636f 6c6f 7220 6973 204e 6f6e  elf.color is Non
+00000a20: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00000a30: 656c 662e 636f 6c6f 7220 3d20 2222 0a0a  elf.color = ""..
+00000a40: 2020 2020 2020 2020 6173 7365 7274 2069          assert i
+00000a50: 7369 6e73 7461 6e63 6528 7365 6c66 2e6e  sinstance(self.n
+00000a60: 616d 652c 2073 7472 290a 2020 2020 2020  ame, str).      
+00000a70: 2020 6173 7365 7274 2069 7369 6e73 7461    assert isinsta
+00000a80: 6e63 6528 7365 6c66 2e63 6f6c 6f72 2c20  nce(self.color, 
+00000a90: 7374 7229 0a0a 2020 2020 2020 2020 2320  str)..        # 
+00000aa0: 6e65 6564 2074 6f20 6465 6669 6e65 2073  need to define s
+00000ab0: 6570 6572 6174 6520 746f 2063 6f6c 6f72  eperate to color
+00000ac0: 2073 696e 6365 2063 6f6c 6f72 2070 726f   since color pro
+00000ad0: 7065 7274 7920 6973 2063 6861 6e67 6564  perty is changed
+00000ae0: 0a20 2020 2020 2020 2023 2077 6865 6e20  .        # when 
+00000af0: 7573 6572 2064 6566 696e 6564 2063 6f6c  user defined col
+00000b00: 6f72 2064 6f65 736e 7420 6578 6973 742e  or doesnt exist.
+00000b10: 2054 6865 7265 2077 6173 2061 2064 6566   There was a def
+00000b20: 696e 6520 666c 6f6f 720a 2020 2020 2020  ine floor.      
+00000b30: 2020 2320 7072 6576 696f 7573 6c79 2073    # previously s
+00000b40: 696e 6365 2077 6865 6e20 7265 6d6f 7669  ince when removi
+00000b50: 6e67 206d 6174 6572 6961 6c73 2074 6865  ng materials the
+00000b60: 2063 6f6c 6f72 2066 6f72 2061 646a 6563   color for adjec
+00000b70: 656e 740a 2020 2020 2020 2020 2320 6d61  ent.        # ma
+00000b80: 7465 7269 616c 7320 636f 756c 6420 6265  terials could be
+00000b90: 636f 6d65 2074 6865 2073 616d 652e 0a20  come the same.. 
+00000ba0: 2020 2020 2020 2023 2043 6f6d 6d65 6e74         # Comment
+00000bb0: 2066 726f 6d20 4a65 7373 6520 422c 2031   from Jesse B, 1
+00000bc0: 342e 3033 2e32 320a 2020 2020 2020 2020  4.03.22.        
+00000bd0: 7365 6c66 2e75 7365 725f 6465 6669 6e65  self.user_define
+00000be0: 645f 636f 6c6f 7220 3d20 7365 6c66 2e63  d_color = self.c
+00000bf0: 6f6c 6f72 0a0a 2020 2020 6465 6620 5f5f  olor..    def __
+00000c00: 7265 7072 5f5f 2873 656c 6629 3a0a 2020  repr__(self):.  
+00000c10: 2020 2020 2020 7265 7475 726e 2028 0a20        return (. 
+00000c20: 2020 2020 2020 2020 2020 2066 224d 6174             f"Mat
+00000c30: 6572 6961 6c3a 7b73 656c 662e 6e61 6d65  erial:{self.name
+00000c40: 7d22 0a20 2020 2020 2020 2020 2020 2066  }".            f
+00000c50: 2228 7577 3d7b 7365 6c66 2e75 6e69 745f  "(uw={self.unit_
+00000c60: 7765 6967 6874 7d2c 220a 2020 2020 2020  weight},".      
+00000c70: 2020 2020 2020 6622 7068 693d 7b73 656c        f"phi={sel
+00000c80: 662e 6672 6963 7469 6f6e 5f61 6e67 6c65  f.friction_angle
+00000c90: 7d2c 220a 2020 2020 2020 2020 2020 2020  },".            
+00000ca0: 6622 633d 7b73 656c 662e 636f 6865 7369  f"c={self.cohesi
+00000cb0: 6f6e 7d2c 220a 2020 2020 2020 2020 2020  on},".          
+00000cc0: 2020 6622 645f 626f 743d 7b73 656c 662e    f"d_bot={self.
+00000cd0: 6465 7074 685f 746f 5f62 6f74 746f 6d7d  depth_to_bottom}
+00000ce0: 2922 0a20 2020 2020 2020 2029 0a0a 0a40  )".        )...@
+00000cf0: 6461 7461 636c 6173 730a 636c 6173 7320  dataclass.class 
+00000d00: 5564 6c3a 0a20 2020 2022 2222 436c 6173  Udl:.    """Clas
+00000d10: 7320 7265 7072 6573 656e 7469 6e67 2075  s representing u
+00000d20: 6e69 666f 726d 6c79 2064 6973 7472 6962  niformly distrib
+00000d30: 7574 6564 2073 7572 6661 6365 2070 7265  uted surface pre
+00000d40: 7373 7572 6520 696e 206b 5061 0a0a 2020  ssure in kPa..  
+00000d50: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+00000d60: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+00000d70: 6d61 676e 6974 7564 6520 3a20 666c 6f61  magnitude : floa
+00000d80: 740a 2020 2020 2020 2020 6d61 676e 6974  t.        magnit
+00000d90: 7564 6520 6f66 2055 444c 2066 6f72 6365  ude of UDL force
+00000da0: 2069 6e20 6b50 610a 2020 2020 6f66 6673   in kPa.    offs
+00000db0: 6574 203a 2066 6c6f 6174 0a20 2020 2020  et : float.     
+00000dc0: 2020 206f 6666 7365 7420 6f66 206c 6f61     offset of loa
+00000dd0: 6420 6672 6f6d 2073 6c6f 7065 2069 6e20  d from slope in 
+00000de0: 6d0a 2020 2020 6c65 6e67 7468 203a 2066  m.    length : f
+00000df0: 6c6f 6174 0a20 2020 2020 2020 206c 656e  loat.        len
+00000e00: 6774 6820 6f66 206c 6f61 6420 696e 206d  gth of load in m
+00000e10: 2c20 6966 2030 206f 7220 4e6f 6e65 2074  , if 0 or None t
+00000e20: 6865 6e20 6173 7375 6d65 6420 636f 6e74  hen assumed cont
+00000e30: 696e 756f 7573 2e0a 2020 2020 2020 2020  inuous..        
+00000e40: 4279 2064 6566 6175 6c74 204e 6f6e 652e  By default None.
+00000e50: 0a20 2020 2063 6f6c 6f72 203a 2073 7472  .    color : str
+00000e60: 2028 6f70 7469 6f6e 616c 290a 2020 2020   (optional).    
+00000e70: 2020 2020 636f 6c6f 7220 746f 2062 6520      color to be 
+00000e80: 7573 6564 2074 6f20 7265 7072 6573 656e  used to represen
+00000e90: 7420 7468 6520 7374 7261 7461 2077 6865  t the strata whe
+00000ea0: 6e20 706c 6f74 7469 6e67 2e20 436f 6c6f  n plotting. Colo
+00000eb0: 720a 2020 2020 2020 2020 6d61 7920 6265  r.        may be
+00000ec0: 2070 726f 7669 6465 6420 6173 2061 2073   provided as a s
+00000ed0: 7472 696e 672c 2073 7461 6e64 6172 6420  tring, standard 
+00000ee0: 3320 6865 7820 6469 6769 7420 6f72 2036  3 hex digit or 6
+00000ef0: 2068 6578 2064 6967 6974 0a20 2020 2020   hex digit.     
+00000f00: 2020 2077 6562 2063 6f6d 7061 7469 626c     web compatibl
+00000f10: 6520 7265 7072 6573 656e 7461 7469 6f6e  e representation
+00000f20: 2e20 4966 206e 6f74 2070 726f 7669 6465  . If not provide
+00000f30: 6420 636f 6c6f 7220 6175 746f 6d61 7469  d color automati
+00000f40: 6361 6c6c 790a 2020 2020 2020 2020 6173  cally.        as
+00000f50: 7369 676e 6564 2e0a 2020 2020 6479 6e61  signed..    dyna
+00000f60: 6d69 635f 6f66 6673 6574 203a 2062 6f6f  mic_offset : boo
+00000f70: 6c0a 2020 2020 2020 2020 4966 2054 7275  l.        If Tru
+00000f80: 6520 7468 656e 2074 6865 206c 6f61 6420  e then the load 
+00000f90: 6f66 6673 6574 2077 696c 6c20 6265 2064  offset will be d
+00000fa0: 796e 616d 6963 616c 6c79 206d 6f76 6564  ynamically moved
+00000fb0: 2069 6620 6120 2264 796e 616d 6963 0a20   if a "dynamic. 
+00000fc0: 2020 2020 2020 2061 6e61 6c79 7369 7322         analysis"
+00000fd0: 2069 7320 7275 6e2e 2028 466f 7220 6120   is run. (For a 
+00000fe0: 7374 616e 6461 7264 2061 6e61 6c79 7369  standard analysi
+00000ff0: 7320 7468 6520 6f66 6673 6574 2076 616c  s the offset val
+00001000: 7565 2069 7320 7374 696c 6c20 7573 6564  ue is still used
+00001010: 292e 0a20 2020 2020 2020 2042 7920 6465  )..        By de
+00001020: 6661 756c 7420 4661 6c73 652e 0a0a 2020  fault False...  
+00001030: 2020 4578 616d 706c 6573 0a20 2020 202d    Examples.    -
+00001040: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
+00001050: 3e3e 3e20 5564 6c28 6d61 676e 6974 7564  >>> Udl(magnitud
+00001060: 6520 3d20 3130 2c20 6f66 6673 6574 203d  e = 10, offset =
+00001070: 2031 2c20 6c65 6e67 7468 203d 2032 2c20   1, length = 2, 
+00001080: 636f 6c6f 7220 3d20 2270 696e 6b22 290a  color = "pink").
+00001090: 2020 2020 5544 4c3a 2031 3020 6b50 612c      UDL: 10 kPa,
+000010a0: 206f 6666 7365 7420 3d20 3120 6d2c 206c   offset = 1 m, l
+000010b0: 6f61 6420 6c65 6e67 7468 203d 2032 206d  oad length = 2 m
+000010c0: 0a20 2020 203e 3e3e 2055 646c 2829 0a20  .    >>> Udl(). 
+000010d0: 2020 2055 444c 3a20 3020 6b50 612c 206f     UDL: 0 kPa, o
+000010e0: 6666 7365 7420 3d20 3020 6d2c 206c 6f61  ffset = 0 m, loa
+000010f0: 6420 6c65 6e67 7468 2063 6f6e 7469 6e75  d length continu
+00001100: 6f75 730a 2020 2020 3e3e 3e20 6120 3d20  ous.    >>> a = 
+00001110: 5564 6c28 290a 2020 2020 3e3e 3e20 612e  Udl().    >>> a.
+00001120: 6d61 676e 6974 7564 6520 3d3d 2030 0a20  magnitude == 0. 
+00001130: 2020 2054 7275 650a 0a20 2020 2022 2222     True..    """
+00001140: 0a0a 2020 2020 6d61 676e 6974 7564 653a  ..    magnitude:
+00001150: 2066 6c6f 6174 203d 2030 0a20 2020 206f   float = 0.    o
+00001160: 6666 7365 743a 2066 6c6f 6174 203d 2030  ffset: float = 0
+00001170: 0a20 2020 206c 656e 6774 683a 2066 6c6f  .    length: flo
+00001180: 6174 203d 204e 6f6e 650a 2020 2020 636f  at = None.    co
+00001190: 6c6f 723a 2073 7472 203d 2022 7265 6422  lor: str = "red"
+000011a0: 0a20 2020 2064 796e 616d 6963 5f6f 6666  .    dynamic_off
+000011b0: 7365 743a 2062 6f6f 6c20 3d20 4661 6c73  set: bool = Fals
+000011c0: 650a 0a20 2020 2064 6566 205f 5f70 6f73  e..    def __pos
+000011d0: 745f 696e 6974 5f5f 2873 656c 6629 3a0a  t_init__(self):.
+000011e0: 2020 2020 2020 2020 6461 7461 5f76 616c          data_val
+000011f0: 6964 6174 696f 6e2e 6173 7365 7274 5f6e  idation.assert_n
+00001200: 756d 6265 7228 7365 6c66 2e6d 6167 6e69  umber(self.magni
+00001210: 7475 6465 2c20 226c 6f61 6420 6d61 676e  tude, "load magn
+00001220: 6974 7564 6522 290a 2020 2020 2020 2020  itude").        
+00001230: 6461 7461 5f76 616c 6964 6174 696f 6e2e  data_validation.
+00001240: 6173 7365 7274 5f6e 756d 6265 7228 7365  assert_number(se
+00001250: 6c66 2e6f 6666 7365 742c 2022 6c6f 6164  lf.offset, "load
+00001260: 206f 6666 7365 7422 290a 0a20 2020 2020   offset")..     
+00001270: 2020 2069 6620 7365 6c66 2e6c 656e 6774     if self.lengt
+00001280: 683a 0a20 2020 2020 2020 2020 2020 2064  h:.            d
+00001290: 6174 615f 7661 6c69 6461 7469 6f6e 2e61  ata_validation.a
+000012a0: 7373 6572 745f 6e75 6d62 6572 2873 656c  ssert_number(sel
+000012b0: 662e 6c65 6e67 7468 2c20 226c 6f61 6420  f.length, "load 
+000012c0: 6c65 6e67 7468 2229 0a20 2020 2020 2020  length").       
+000012d0: 2020 2020 2073 656c 662e 6c65 6e67 7468       self.length
+000012e0: 203d 2061 6273 2873 656c 662e 6c65 6e67   = abs(self.leng
+000012f0: 7468 290a 2020 2020 2020 2020 656c 7365  th).        else
+00001300: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+00001310: 6d61 6b65 206e 6f6e 6520 6966 206c 656e  make none if len
+00001320: 6774 6820 3d20 303f 0a20 2020 2020 2020  gth = 0?.       
+00001330: 2020 2020 2073 656c 662e 6c65 6e67 7468       self.length
+00001340: 203d 204e 6f6e 650a 0a20 2020 2020 2020   = None..       
+00001350: 2073 656c 662e 6d61 676e 6974 7564 6520   self.magnitude 
+00001360: 3d20 6162 7328 7365 6c66 2e6d 6167 6e69  = abs(self.magni
+00001370: 7475 6465 290a 2020 2020 2020 2020 7365  tude).        se
+00001380: 6c66 2e6f 6666 7365 7420 3d20 6162 7328  lf.offset = abs(
+00001390: 7365 6c66 2e6f 6666 7365 7429 0a0a 2020  self.offset)..  
+000013a0: 2020 2020 2020 7365 6c66 2e70 7265 6369        self.preci
+000013b0: 7369 6f6e 203d 2075 7469 6c69 7469 6573  sion = utilities
+000013c0: 2e67 6574 5f70 7265 6369 7369 6f6e 2873  .get_precision(s
+000013d0: 656c 662e 6d61 676e 6974 7564 6529 0a0a  elf.magnitude)..
+000013e0: 2020 2020 2020 2020 6966 206e 6f74 2075          if not u
+000013f0: 7469 6c69 7469 6573 2e69 735f 636f 6c6f  tilities.is_colo
+00001400: 7228 7365 6c66 2e63 6f6c 6f72 293a 0a20  r(self.color):. 
+00001410: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00001420: 636f 6c6f 7220 3d20 2272 6564 220a 0a20  color = "red".. 
+00001430: 2020 2064 6566 205f 5f72 6570 725f 5f28     def __repr__(
+00001440: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
+00001450: 6620 7365 6c66 2e6c 656e 6774 6820 6973  f self.length is
+00001460: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00001470: 2020 2072 6574 7572 6e20 6622 5544 4c3a     return f"UDL:
+00001480: 207b 7365 6c66 2e6d 6167 6e69 7475 6465   {self.magnitude
+00001490: 7d20 6b50 612c 206f 6666 7365 7420 3d20  } kPa, offset = 
+000014a0: 7b73 656c 662e 6f66 6673 6574 7d20 6d2c  {self.offset} m,
+000014b0: 206c 6f61 6420 6c65 6e67 7468 2063 6f6e   load length con
+000014c0: 7469 6e75 6f75 7322 0a20 2020 2020 2020  tinuous".       
+000014d0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000014e0: 2020 2072 6574 7572 6e20 6622 5544 4c3a     return f"UDL:
+000014f0: 207b 7365 6c66 2e6d 6167 6e69 7475 6465   {self.magnitude
+00001500: 7d20 6b50 612c 206f 6666 7365 7420 3d20  } kPa, offset = 
+00001510: 7b73 656c 662e 6f66 6673 6574 7d20 6d2c  {self.offset} m,
+00001520: 206c 6f61 6420 6c65 6e67 7468 203d 207b   load length = {
+00001530: 7365 6c66 2e6c 656e 6774 687d 206d 220a  self.length} m".
+00001540: 0a0a 4064 6174 6163 6c61 7373 0a63 6c61  ..@dataclass.cla
+00001550: 7373 204c 696e 654c 6f61 643a 0a20 2020  ss LineLoad:.   
+00001560: 2022 2222 436c 6173 7320 7265 7072 6573   """Class repres
+00001570: 656e 7469 6e67 206c 696e 6520 6c6f 6164  enting line load
+00001580: 2069 6e20 6b4e 2f6d 0a0a 2020 2020 5061   in kN/m..    Pa
+00001590: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
+000015a0: 2d2d 2d2d 2d2d 2d0a 2020 2020 6d61 676e  -------.    magn
+000015b0: 6974 7564 6520 3a20 666c 6f61 740a 2020  itude : float.  
+000015c0: 2020 2020 2020 6d61 676e 6974 7564 6520        magnitude 
+000015d0: 6f66 2055 444c 2066 6f72 6365 2069 6e20  of UDL force in 
+000015e0: 6b50 610a 2020 2020 6f66 6673 6574 203a  kPa.    offset :
+000015f0: 2066 6c6f 6174 0a20 2020 2020 2020 206f   float.        o
+00001600: 6666 7365 7420 6f66 206c 6f61 6420 6672  ffset of load fr
+00001610: 6f6d 2073 6c6f 7065 2069 6e20 6d0a 2020  om slope in m.  
+00001620: 2020 6c65 6e67 7468 203a 2066 6c6f 6174    length : float
+00001630: 0a20 2020 2020 2020 206c 656e 6774 6820  .        length 
+00001640: 6f66 206c 6f61 6420 696e 206d 2c20 6966  of load in m, if
+00001650: 2030 206f 7220 4e6f 6e65 2074 6865 6e20   0 or None then 
+00001660: 6173 7375 6d65 6420 636f 6e74 696e 756f  assumed continuo
+00001670: 7573 2e0a 2020 2020 2020 2020 4279 2064  us..        By d
+00001680: 6566 6175 6c74 204e 6f6e 652e 0a20 2020  efault None..   
+00001690: 2063 6f6c 6f72 203a 2073 7472 2028 6f70   color : str (op
+000016a0: 7469 6f6e 616c 290a 2020 2020 2020 2020  tional).        
+000016b0: 636f 6c6f 7220 746f 2062 6520 7573 6564  color to be used
+000016c0: 2074 6f20 7265 7072 6573 656e 7420 7468   to represent th
+000016d0: 6520 7374 7261 7461 2077 6865 6e20 706c  e strata when pl
+000016e0: 6f74 7469 6e67 2e20 436f 6c6f 720a 2020  otting. Color.  
+000016f0: 2020 2020 2020 6d61 7920 6265 2070 726f        may be pro
+00001700: 7669 6465 6420 6173 2061 2073 7472 696e  vided as a strin
+00001710: 672c 2073 7461 6e64 6172 6420 3320 6865  g, standard 3 he
+00001720: 7820 6469 6769 7420 6f72 2036 2068 6578  x digit or 6 hex
+00001730: 2064 6967 6974 0a20 2020 2020 2020 2077   digit.        w
+00001740: 6562 2063 6f6d 7061 7469 626c 6520 7265  eb compatible re
+00001750: 7072 6573 656e 7461 7469 6f6e 2e20 4966  presentation. If
+00001760: 206e 6f74 2070 726f 7669 6465 6420 636f   not provided co
+00001770: 6c6f 7220 6175 746f 6d61 7469 6361 6c6c  lor automaticall
+00001780: 790a 2020 2020 2020 2020 6173 7369 676e  y.        assign
+00001790: 6564 2e0a 2020 2020 6479 6e61 6d69 635f  ed..    dynamic_
+000017a0: 6f66 6673 6574 203a 2062 6f6f 6c0a 2020  offset : bool.  
+000017b0: 2020 2020 2020 4966 2054 7275 6520 7468        If True th
+000017c0: 656e 2074 6865 206c 6f61 6420 6f66 6673  en the load offs
+000017d0: 6574 2077 696c 6c20 6265 2064 796e 616d  et will be dynam
+000017e0: 6963 616c 6c79 206d 6f76 6564 2069 6620  ically moved if 
+000017f0: 6120 2264 796e 616d 6963 0a20 2020 2020  a "dynamic.     
+00001800: 2020 2061 6e61 6c79 7369 7322 2069 7320     analysis" is 
+00001810: 7275 6e2e 2028 466f 7220 6120 7374 616e  run. (For a stan
+00001820: 6461 7264 2061 6e61 6c79 7369 7320 7468  dard analysis th
+00001830: 6520 6f66 6673 6574 2076 616c 7565 2069  e offset value i
+00001840: 7320 7374 696c 6c20 7573 6564 292e 0a20  s still used).. 
+00001850: 2020 2020 2020 2042 7920 6465 6661 756c         By defaul
+00001860: 7420 4661 6c73 652e 0a0a 2020 2020 4578  t False...    Ex
+00001870: 616d 706c 6573 0a20 2020 202d 2d2d 2d2d  amples.    -----
+00001880: 2d2d 2d2d 2d2d 2d0a 2020 2020 3e3e 3e20  -------.    >>> 
+00001890: 4c69 6e65 4c6f 6164 286d 6167 6e69 7475  LineLoad(magnitu
+000018a0: 6465 203d 2031 302c 206f 6666 7365 7420  de = 10, offset 
+000018b0: 3d20 312c 2063 6f6c 6f72 203d 2022 7069  = 1, color = "pi
+000018c0: 6e6b 2229 0a20 2020 204c 696e 654c 6f61  nk").    LineLoa
+000018d0: 643a 2031 3020 6b4e 2f6d 2c20 6f66 6673  d: 10 kN/m, offs
+000018e0: 6574 203d 2031 206d 0a20 2020 203e 3e3e  et = 1 m.    >>>
+000018f0: 204c 696e 654c 6f61 6428 290a 2020 2020   LineLoad().    
+00001900: 4c69 6e65 4c6f 6164 3a20 3020 6b4e 2f6d  LineLoad: 0 kN/m
+00001910: 2c20 6f66 6673 6574 203d 2030 206d 0a20  , offset = 0 m. 
+00001920: 2020 203e 3e3e 2061 203d 204c 696e 654c     >>> a = LineL
+00001930: 6f61 6428 290a 2020 2020 3e3e 3e20 612e  oad().    >>> a.
+00001940: 6d61 676e 6974 7564 6520 3d3d 2030 0a20  magnitude == 0. 
+00001950: 2020 2054 7275 650a 2020 2020 2222 220a     True.    """.
+00001960: 0a20 2020 206d 6167 6e69 7475 6465 3a20  .    magnitude: 
+00001970: 666c 6f61 7420 3d20 300a 2020 2020 6f66  float = 0.    of
+00001980: 6673 6574 3a20 666c 6f61 7420 3d20 300a  fset: float = 0.
+00001990: 2020 2020 636f 6c6f 723a 2073 7472 203d      color: str =
+000019a0: 2022 626c 7565 220a 2020 2020 6479 6e61   "blue".    dyna
+000019b0: 6d69 635f 6f66 6673 6574 3a20 626f 6f6c  mic_offset: bool
+000019c0: 203d 2046 616c 7365 0a0a 2020 2020 6465   = False..    de
+000019d0: 6620 5f5f 706f 7374 5f69 6e69 745f 5f28  f __post_init__(
+000019e0: 7365 6c66 293a 0a20 2020 2020 2020 2064  self):.        d
+000019f0: 6174 615f 7661 6c69 6461 7469 6f6e 2e61  ata_validation.a
+00001a00: 7373 6572 745f 6e75 6d62 6572 2873 656c  ssert_number(sel
+00001a10: 662e 6d61 676e 6974 7564 652c 2022 6c6f  f.magnitude, "lo
+00001a20: 6164 206d 6167 6e69 7475 6465 2229 0a20  ad magnitude"). 
+00001a30: 2020 2020 2020 2064 6174 615f 7661 6c69         data_vali
+00001a40: 6461 7469 6f6e 2e61 7373 6572 745f 6e75  dation.assert_nu
+00001a50: 6d62 6572 2873 656c 662e 6f66 6673 6574  mber(self.offset
+00001a60: 2c20 226c 6f61 6420 6f66 6673 6574 2229  , "load offset")
+00001a70: 0a0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
+00001a80: 7265 6369 7369 6f6e 203d 2075 7469 6c69  recision = utili
+00001a90: 7469 6573 2e67 6574 5f70 7265 6369 7369  ties.get_precisi
+00001aa0: 6f6e 2873 656c 662e 6d61 676e 6974 7564  on(self.magnitud
+00001ab0: 6529 0a0a 2020 2020 2020 2020 7365 6c66  e)..        self
+00001ac0: 2e6d 6167 6e69 7475 6465 203d 2061 6273  .magnitude = abs
+00001ad0: 2873 656c 662e 6d61 676e 6974 7564 6529  (self.magnitude)
+00001ae0: 0a20 2020 2020 2020 2073 656c 662e 6f66  .        self.of
+00001af0: 6673 6574 203d 2061 6273 2873 656c 662e  fset = abs(self.
+00001b00: 6f66 6673 6574 290a 0a20 2020 2020 2020  offset)..       
+00001b10: 2069 6620 6e6f 7420 7574 696c 6974 6965   if not utilitie
+00001b20: 732e 6973 5f63 6f6c 6f72 2873 656c 662e  s.is_color(self.
+00001b30: 636f 6c6f 7229 3a0a 2020 2020 2020 2020  color):.        
+00001b40: 2020 2020 7365 6c66 2e63 6f6c 6f72 203d      self.color =
+00001b50: 2022 626c 7565 220a 0a20 2020 2064 6566   "blue"..    def
+00001b60: 205f 5f72 6570 725f 5f28 7365 6c66 293a   __repr__(self):
+00001b70: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00001b80: 6622 4c69 6e65 4c6f 6164 3a20 7b73 656c  f"LineLoad: {sel
+00001b90: 662e 6d61 676e 6974 7564 657d 206b 4e2f  f.magnitude} kN/
+00001ba0: 6d2c 206f 6666 7365 7420 3d20 7b73 656c  m, offset = {sel
+00001bb0: 662e 6f66 6673 6574 7d20 6d22 0a0a 0a63  f.offset} m"...c
+00001bc0: 6c61 7373 2053 6c6f 7065 3a0a 2020 2020  lass Slope:.    
+00001bd0: 2222 2253 6c6f 7065 206f 626a 6563 742e  """Slope object.
+00001be0: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
+00001bf0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+00001c00: 2020 2020 6865 6967 6874 203a 2066 6c6f      height : flo
+00001c10: 6174 0a20 2020 2020 2020 2068 6569 6768  at.        heigh
+00001c20: 7420 6f66 2073 6c6f 7065 2069 6e20 6d65  t of slope in me
+00001c30: 7472 6573 2c20 6279 2064 6566 6175 6c74  tres, by default
+00001c40: 2032 0a20 2020 2061 6e67 6c65 203a 2069   2.    angle : i
+00001c50: 6e74 2c20 6f70 7469 6f6e 616c 0a20 2020  nt, optional.   
+00001c60: 2020 2020 2061 6e67 6c65 206f 6620 736c       angle of sl
+00001c70: 6f70 6520 286f 6e6c 7920 7573 6564 2069  ope (only used i
+00001c80: 6620 6c65 6e67 7468 204e 6f6e 6529 2c20  f length None), 
+00001c90: 6279 2064 6566 6175 6c74 2033 300a 2020  by default 30.  
+00001ca0: 2020 6c65 6e67 7468 203a 2066 6c6f 6174    length : float
+00001cb0: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+00001cc0: 2020 206c 656e 6774 6820 6f66 2073 6c6f     length of slo
+00001cd0: 7065 2069 6e20 6d65 7472 6573 2c20 6279  pe in metres, by
+00001ce0: 2064 6566 6175 6c74 204e 6f6e 650a 0a20   default None.. 
+00001cf0: 2020 2045 7861 6d70 6c65 730a 2020 2020     Examples.    
+00001d00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
+00001d10: 203e 3e3e 2053 6c6f 7065 2868 6569 6768   >>> Slope(heigh
+00001d20: 7420 3d20 312c 2061 6e67 6c65 203d 2035  t = 1, angle = 5
+00001d30: 302c 206c 656e 6774 6820 3d20 4e6f 6e65  0, length = None
+00001d40: 290a 2020 2020 536c 6f70 653a 2031 5620  ).    Slope: 1V 
+00001d50: 3a20 302e 3833 3948 0a20 2020 203e 3e3e  : 0.839H.    >>>
+00001d60: 2053 6c6f 7065 2868 6569 6768 7420 3d20   Slope(height = 
+00001d70: 312c 2061 6e67 6c65 203d 2035 302c 206c  1, angle = 50, l
+00001d80: 656e 6774 6820 3d20 3229 0a20 2020 2053  ength = 2).    S
+00001d90: 6c6f 7065 3a20 3156 203a 2032 480a 2020  lope: 1V : 2H.  
+00001da0: 2020 3e3e 3e20 536c 6f70 6528 6865 6967    >>> Slope(heig
+00001db0: 6874 203d 2031 2c20 616e 676c 6520 3d20  ht = 1, angle = 
+00001dc0: 4e6f 6e65 2c20 6c65 6e67 7468 203d 2032  None, length = 2
+00001dd0: 290a 2020 2020 536c 6f70 653a 2031 5620  ).    Slope: 1V 
+00001de0: 3a20 3248 0a20 2020 203e 3e3e 2053 6c6f  : 2H.    >>> Slo
+00001df0: 7065 2829 0a20 2020 2053 6c6f 7065 3a20  pe().    Slope: 
+00001e00: 3156 203a 2031 2e37 3332 480a 2020 2020  1V : 1.732H.    
+00001e10: 2222 220a 0a20 2020 2064 6566 205f 5f72  """..    def __r
+00001e20: 6570 725f 5f28 7365 6c66 293a 0a20 2020  epr__(self):.   
+00001e30: 2020 2020 2072 6574 7572 6e20 6622 536c       return f"Sl
+00001e40: 6f70 653a 207b 726f 756e 6428 7365 6c66  ope: {round(self
+00001e50: 2e5f 6865 6967 6874 2c33 297d 5620 3a20  ._height,3)}V : 
+00001e60: 7b72 6f75 6e64 2873 656c 662e 5f6c 656e  {round(self._len
+00001e70: 6774 682c 3329 7d48 220a 0a20 2020 2064  gth,3)}H"..    d
+00001e80: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00001e90: 2c20 6865 6967 6874 3a20 666c 6f61 7420  , height: float 
+00001ea0: 3d20 312c 2061 6e67 6c65 3a20 696e 7420  = 1, angle: int 
+00001eb0: 3d20 3330 2c20 6c65 6e67 7468 3a20 666c  = 30, length: fl
+00001ec0: 6f61 7420 3d20 4e6f 6e65 293a 0a20 2020  oat = None):.   
+00001ed0: 2020 2020 2023 2069 6e69 7469 616c 6973       # initialis
+00001ee0: 6520 656d 7074 7920 7072 6f70 6572 7469  e empty properti
+00001ef0: 6573 2075 7365 6420 696e 206f 7468 6572  es used in other
+00001f00: 2063 6f6d 706f 6e65 6e74 7320 6f66 2063   components of c
+00001f10: 6c61 7373 0a20 2020 2020 2020 2073 656c  lass.        sel
+00001f20: 662e 5f6d 6174 6572 6961 6c73 203d 205b  f._materials = [
+00001f30: 5d0a 2020 2020 2020 2020 7365 6c66 2e5f  ].        self._
+00001f40: 7761 7465 725f 524c 203d 204e 6f6e 650a  water_RL = None.
+00001f50: 2020 2020 2020 2020 7365 6c66 2e5f 7564          self._ud
+00001f60: 6c73 203d 205b 5d0a 2020 2020 2020 2020  ls = [].        
+00001f70: 7365 6c66 2e5f 6c6c 7320 3d20 5b5d 0a0a  self._lls = []..
+00001f80: 2020 2020 2020 2020 2320 4e4f 5445 3a20          # NOTE: 
+00001f90: 646f 6e74 2077 616e 7420 746f 2072 6573  dont want to res
+00001fa0: 6574 2077 6974 6820 6368 616e 6765 7320  et with changes 
+00001fb0: 746f 2074 6865 206d 6f64 656c 2c20 6a75  to the model, ju
+00001fc0: 7374 206e 6565 6420 746f 2069 6e69 7469  st need to initi
+00001fd0: 616c 6973 6520 6865 7265 0a20 2020 2020  alise here.     
+00001fe0: 2020 2073 656c 662e 5f64 796e 616d 6963     self._dynamic
+00001ff0: 5f72 6573 756c 7473 203d 207b 7d0a 2020  _results = {}.  
+00002000: 2020 2020 2020 7365 6c66 2e5f 696e 6469        self._indi
+00002010: 7669 6475 616c 5f70 6c61 6e65 7320 3d20  vidual_planes = 
+00002020: 5b5d 0a0a 2020 2020 2020 2020 7365 6c66  []..        self
+00002030: 2e5f 6578 7465 726e 616c 5f62 6f75 6e64  ._external_bound
+00002040: 6172 7920 3d20 4e6f 6e65 0a0a 2020 2020  ary = None..    
+00002050: 2020 2020 2320 696e 7469 616c 6973 6520      # intialise 
+00002060: 6f70 7469 6f6e 730a 2020 2020 2020 2020  options.        
+00002070: 7365 6c66 2e75 7064 6174 655f 626f 756e  self.update_boun
+00002080: 6461 7279 5f6f 7074 696f 6e73 284d 494e  dary_options(MIN
+00002090: 5f45 5854 5f48 3d36 2c20 4d49 4e5f 4558  _EXT_H=6, MIN_EX
+000020a0: 545f 4c3d 3130 290a 2020 2020 2020 2020  T_L=10).        
+000020b0: 7365 6c66 2e73 6574 5f65 7874 6572 6e61  self.set_externa
+000020c0: 6c5f 626f 756e 6461 7279 2868 6569 6768  l_boundary(heigh
+000020d0: 743d 6865 6967 6874 2c20 616e 676c 653d  t=height, angle=
+000020e0: 616e 676c 652c 206c 656e 6774 683d 6c65  angle, length=le
+000020f0: 6e67 7468 290a 2020 2020 2020 2020 7365  ngth).        se
+00002100: 6c66 2e75 7064 6174 655f 616e 616c 7973  lf.update_analys
+00002110: 6973 5f6f 7074 696f 6e73 280a 2020 2020  is_options(.    
+00002120: 2020 2020 2020 2020 736c 6963 6573 3d32          slices=2
+00002130: 352c 0a20 2020 2020 2020 2020 2020 2069  5,.            i
+00002140: 7465 7261 7469 6f6e 733d 3130 3030 2c0a  terations=1000,.
+00002150: 2020 2020 2020 2020 2020 2020 6d69 6e5f              min_
+00002160: 6661 696c 7572 655f 6469 7374 3d30 2c0a  failure_dist=0,.
+00002170: 2020 2020 2020 2020 2020 2020 746f 6c65              tole
+00002180: 7261 6e63 653d 302e 3030 352c 0a20 2020  rance=0.005,.   
+00002190: 2020 2020 2020 2020 206d 6178 5f69 7465           max_ite
+000021a0: 7261 7469 6f6e 733d 3135 2c0a 2020 2020  rations=15,.    
+000021b0: 2020 2020 290a 0a20 2020 2020 2020 2073      )..        s
+000021c0: 656c 662e 7570 6461 7465 5f77 6174 6572  elf.update_water
+000021d0: 5f61 6e61 6c79 7369 735f 6f70 7469 6f6e  _analysis_option
+000021e0: 7328 6175 746f 3d54 7275 6529 0a0a 2020  s(auto=True)..  
+000021f0: 2020 2020 2020 2320 7365 7473 2064 6566        # sets def
+00002200: 6175 6c74 2061 6e61 6c79 7369 7320 6c69  ault analysis li
+00002210: 6d69 7473 2028 6965 206e 6f20 6c69 6d69  mits (ie no limi
+00002220: 7429 0a20 2020 2020 2020 2073 656c 662e  t).        self.
+00002230: 7265 6d6f 7665 5f61 6e61 6c79 7369 735f  remove_analysis_
+00002240: 6c69 6d69 7473 2829 0a0a 2020 2020 6465  limits()..    de
+00002250: 6620 5f72 6573 6574 5f72 6573 756c 7473  f _reset_results
+00002260: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00002270: 2222 2263 6c65 6172 7320 7365 6172 6368  """clears search
+00002280: 2076 616c 7565 2c20 7275 6e20 7768 656e   value, run when
+00002290: 206d 6f64 656c 2072 6573 756c 7473 206e   model results n
+000022a0: 6f20 6c6f 6e67 6572 2076 616c 6964 2e22  o longer valid."
+000022b0: 2222 0a0a 2020 2020 2020 2020 7365 6c66  ""..        self
+000022c0: 2e5f 7365 6172 6368 203d 205b 5d0a 2020  ._search = [].  
+000022d0: 2020 2020 2020 7365 6c66 2e5f 6d69 6e5f        self._min_
+000022e0: 464f 5320 3d20 300a 2020 2020 2020 2020  FOS = 0.        
+000022f0: 7365 6c66 2e5f 6d69 6e5f 464f 535f 6c6f  self._min_FOS_lo
+00002300: 6361 7469 6f6e 203d 205b 5d0a 2020 2020  cation = [].    
+00002310: 2020 2020 7365 6c66 2e5f 6d69 6e5f 464f      self._min_FO
+00002320: 535f 6469 6374 203d 207b 0a20 2020 2020  S_dict = {.     
+00002330: 2020 2020 2020 2022 464f 5322 3a20 302c         "FOS": 0,
+00002340: 0a20 2020 2020 2020 2020 2020 2022 6c5f  .            "l_
+00002350: 6322 3a20 302c 0a20 2020 2020 2020 2020  c": 0,.         
+00002360: 2020 2022 725f 6322 3a20 302c 0a20 2020     "r_c": 0,.   
+00002370: 2020 2020 2020 2020 2022 635f 7822 3a20           "c_x": 
+00002380: 302c 0a20 2020 2020 2020 2020 2020 2022  0,.            "
+00002390: 635f 7922 3a20 302c 0a20 2020 2020 2020  c_y": 0,.       
+000023a0: 2020 2020 2022 7261 6469 7573 223a 2030       "radius": 0
+000023b0: 2c0a 2020 2020 2020 2020 7d0a 0a20 2020  ,.        }..   
+000023c0: 2064 6566 2073 6574 5f65 7874 6572 6e61   def set_externa
+000023d0: 6c5f 626f 756e 6461 7279 280a 2020 2020  l_boundary(.    
+000023e0: 2020 2020 7365 6c66 2c20 6865 6967 6874      self, height
+000023f0: 3a20 666c 6f61 7420 3d20 312c 2061 6e67  : float = 1, ang
+00002400: 6c65 3a20 696e 7420 3d20 3330 2c20 6c65  le: int = 30, le
+00002410: 6e67 7468 3a20 666c 6f61 7420 3d20 4e6f  ngth: float = No
+00002420: 6e65 0a20 2020 2029 3a0a 2020 2020 2020  ne.    ):.      
+00002430: 2020 2222 2253 6574 2065 7874 6572 6e61    """Set externa
+00002440: 6c20 626f 756e 6461 7279 2066 6f72 206d  l boundary for m
+00002450: 6f64 656c 2e0a 0a20 2020 2020 2020 2050  odel...        P
+00002460: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+00002470: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00002480: 2020 2020 2068 6569 6768 7420 3a20 666c       height : fl
+00002490: 6f61 742c 206f 7074 696f 6e61 6c0a 2020  oat, optional.  
+000024a0: 2020 2020 2020 2020 2020 6865 6967 6874            height
+000024b0: 206f 6620 736c 6f70 6520 696e 206d 6574   of slope in met
+000024c0: 7265 732c 2062 7920 6465 6661 756c 7420  res, by default 
+000024d0: 310a 2020 2020 2020 2020 616e 676c 6520  1.        angle 
+000024e0: 3a20 696e 742c 206f 7074 696f 6e61 6c0a  : int, optional.
+000024f0: 2020 2020 2020 2020 2020 2020 616e 676c              angl
+00002500: 6520 6f66 2073 6c6f 7065 2069 6e20 6465  e of slope in de
+00002510: 6772 6565 7320 286d 6179 2062 6520 6c65  grees (may be le
+00002520: 6674 2061 7320 6e6f 6e65 2069 6620 736c  ft as none if sl
+00002530: 6f70 650a 2020 2020 2020 2020 2020 2020  ope.            
+00002540: 6973 2069 6e73 7465 6164 2065 7870 7265  is instead expre
+00002550: 7373 6564 2062 7920 6c65 6e67 7468 206f  ssed by length o
+00002560: 6620 736c 6f70 6529 2c20 6279 2064 6566  f slope), by def
+00002570: 6175 6c74 2033 300a 2020 2020 2020 2020  ault 30.        
+00002580: 6c65 6e67 7468 203a 2066 6c6f 6174 2c20  length : float, 
+00002590: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
+000025a0: 2020 2020 206c 656e 6774 6820 6f66 2073       length of s
+000025b0: 6c6f 7065 2069 6e20 6d65 7472 6573 2028  lope in metres (
+000025c0: 6d61 7920 6265 206c 6566 7420 6173 206e  may be left as n
+000025d0: 6f6e 6520 6966 2073 6c6f 7065 0a20 2020  one if slope.   
+000025e0: 2020 2020 2020 2020 2069 7320 696e 7374           is inst
+000025f0: 6561 6420 6578 7072 6573 7365 6420 6279  ead expressed by
+00002600: 2061 6e67 6c65 206f 6620 736c 6f70 6529   angle of slope)
+00002610: 2c20 6279 2064 6566 6175 6c74 204e 6f6e  , by default Non
+00002620: 650a 0a20 2020 2020 2020 2052 6169 7365  e..        Raise
+00002630: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+00002640: 0a20 2020 2020 2020 2056 616c 7565 4572  .        ValueEr
+00002650: 726f 720a 2020 2020 2020 2020 2020 2020  ror.            
+00002660: 4966 2069 6e70 7574 206e 6f74 2069 6e20  If input not in 
+00002670: 7265 7175 6972 6564 2072 616e 6765 206f  required range o
+00002680: 7220 6f66 2072 6571 7569 7265 6420 7479  r of required ty
+00002690: 7065 0a0a 2020 2020 2020 2020 4578 616d  pe..        Exam
+000026a0: 706c 6573 0a20 2020 2020 2020 202d 2d2d  ples.        ---
+000026b0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+000026c0: 2020 3e3e 3e20 6120 3d20 536c 6f70 6528    >>> a = Slope(
+000026d0: 6865 6967 6874 203d 2031 2c20 616e 676c  height = 1, angl
+000026e0: 6520 3d20 3435 2c20 6c65 6e67 7468 203d  e = 45, length =
+000026f0: 204e 6f6e 6529 0a20 2020 2020 2020 203e   None).        >
+00002700: 3e3e 2061 0a20 2020 2020 2020 2053 6c6f  >> a.        Slo
+00002710: 7065 3a20 3156 203a 2031 2e30 480a 2020  pe: 1V : 1.0H.  
+00002720: 2020 2020 2020 3e3e 3e20 612e 7365 745f        >>> a.set_
+00002730: 6578 7465 726e 616c 5f62 6f75 6e64 6172  external_boundar
+00002740: 7928 6865 6967 6874 203d 2032 2c20 6c65  y(height = 2, le
+00002750: 6e67 7468 203d 2030 2e35 290a 2020 2020  ngth = 0.5).    
+00002760: 2020 2020 3e3e 3e20 610a 2020 2020 2020      >>> a.      
+00002770: 2020 536c 6f70 653a 2032 5620 3a20 302e    Slope: 2V : 0.
+00002780: 3548 0a20 2020 2020 2020 2022 2222 0a20  5H.        """. 
+00002790: 2020 2020 2020 2023 2076 616c 6964 6174         # validat
+000027a0: 6520 696e 7075 7473 0a20 2020 2020 2020  e inputs.       
+000027b0: 2069 6620 6865 6967 6874 2069 7320 6e6f   if height is no
+000027c0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000027d0: 2020 2020 6461 7461 5f76 616c 6964 6174      data_validat
+000027e0: 696f 6e2e 6173 7365 7274 5f73 7472 6963  ion.assert_stric
+000027f0: 746c 795f 706f 7369 7469 7665 5f6e 756d  tly_positive_num
+00002800: 6265 7228 6865 6967 6874 2c20 2268 6569  ber(height, "hei
+00002810: 6768 7422 290a 2020 2020 2020 2020 6966  ght").        if
+00002820: 2061 6e67 6c65 2069 7320 6e6f 7420 4e6f   angle is not No
+00002830: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00002840: 2320 6973 2061 6c6c 6f77 6564 2074 6f20  # is allowed to 
+00002850: 6265 2039 3020 6275 7420 6e6f 7420 300a  be 90 but not 0.
+00002860: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00002870: 5f76 616c 6964 6174 696f 6e2e 6173 7365  _validation.asse
+00002880: 7274 5f72 616e 6765 2861 6e67 6c65 2c20  rt_range(angle, 
+00002890: 2261 6e67 6c65 222c 2030 2c20 3930 2c20  "angle", 0, 90, 
+000028a0: 6e6f 745f 6c6f 773d 5472 7565 290a 2020  not_low=True).  
+000028b0: 2020 2020 2020 6966 206c 656e 6774 6820        if length 
+000028c0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000028d0: 2020 2020 2020 2020 2064 6174 615f 7661           data_va
+000028e0: 6c69 6461 7469 6f6e 2e61 7373 6572 745f  lidation.assert_
+000028f0: 706f 7369 7469 7665 5f6e 756d 6265 7228  positive_number(
+00002900: 6c65 6e67 7468 2c20 226c 656e 6774 6822  length, "length"
+00002910: 290a 0a20 2020 2020 2020 2023 2069 6620  )..        # if 
+00002920: 616e 676c 6520 6173 7369 676e 6564 2069  angle assigned i
+00002930: 6e73 7465 6164 206f 6620 6c65 6e67 7468  nstead of length
+00002940: 2077 6f72 6b20 6f75 7420 7468 6520 6d6f   work out the mo
+00002950: 6465 6c20 6c65 6e67 7468 0a20 2020 2020  del length.     
+00002960: 2020 2069 6620 6c65 6e67 7468 2069 7320     if length is 
+00002970: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00002980: 2020 6966 206e 6f74 2061 6e67 6c65 3a0a    if not angle:.
+00002990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029a0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+000029b0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000029c0: 2020 2020 2020 2272 6571 7569 7265 2061        "require a
+000029d0: 6e67 6c65 206f 6620 736c 6f70 6520 6f72  ngle of slope or
+000029e0: 206c 656e 6774 6820 6f66 2073 6c6f 7065   length of slope
+000029f0: 2074 6f20 696e 6974 6961 6c69 7365 220a   to initialise".
+00002a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a10: 290a 2020 2020 2020 2020 2020 2020 6c65  ).            le
+00002a20: 6e67 7468 203d 2068 6569 6768 7420 2f20  ngth = height / 
+00002a30: 7461 6e28 7261 6469 616e 7328 616e 676c  tan(radians(angl
+00002a40: 6529 290a 0a20 2020 2020 2020 2023 2068  e))..        # h
+00002a50: 656c 7020 7769 7468 2064 6976 6973 696f  elp with divisio
+00002a60: 6e20 6279 207a 6572 6f20 6572 726f 7273  n by zero errors
+00002a70: 0a20 2020 2020 2020 206c 656e 6774 6820  .        length 
+00002a80: 3d20 6d61 7828 6c65 6e67 7468 2c20 302e  = max(length, 0.
+00002a90: 3030 3129 0a0a 2020 2020 2020 2020 4d49  001)..        MI
+00002aa0: 4e5f 4558 545f 4820 3d20 7365 6c66 2e5f  N_EXT_H = self._
+00002ab0: 4d49 4e5f 4558 545f 480a 2020 2020 2020  MIN_EXT_H.      
+00002ac0: 2020 4d49 4e5f 4558 545f 4c20 3d20 7365    MIN_EXT_L = se
+00002ad0: 6c66 2e5f 4d49 4e5f 4558 545f 4c0a 0a20  lf._MIN_EXT_L.. 
+00002ae0: 2020 2020 2020 2074 6f74 5f68 203d 206d         tot_h = m
+00002af0: 6178 2833 202a 2068 6569 6768 742c 204d  ax(3 * height, M
+00002b00: 494e 5f45 5854 5f48 2c20 3520 2a20 6c65  IN_EXT_H, 5 * le
+00002b10: 6e67 7468 202f 2032 290a 2020 2020 2020  ngth / 2).      
+00002b20: 2020 746f 745f 6c20 3d20 6d61 7828 3520    tot_l = max(5 
+00002b30: 2a20 6c65 6e67 7468 2c20 4d49 4e5f 4558  * length, MIN_EX
+00002b40: 545f 4c2c 2034 202a 2068 6569 6768 7429  T_L, 4 * height)
+00002b50: 0a0a 2020 2020 2020 2020 2320 6465 7465  ..        # dete
+00002b60: 726d 696e 6520 636f 6f72 6469 6e61 7465  rmine coordinate
+00002b70: 7320 666f 7220 6564 6765 7320 6f66 2073  s for edges of s
+00002b80: 6c6f 7065 0a20 2020 2020 2020 2064 7820  lope.        dx 
+00002b90: 3d20 2874 6f74 5f6c 202d 206c 656e 6774  = (tot_l - lengt
+00002ba0: 6829 202f 2032 0a20 2020 2020 2020 2074  h) / 2.        t
+00002bb0: 6f70 203d 2028 6478 2c20 746f 745f 6829  op = (dx, tot_h)
+00002bc0: 0a20 2020 2020 2020 2062 6f74 203d 2028  .        bot = (
+00002bd0: 6478 202b 206c 656e 6774 682c 2074 6f74  dx + length, tot
+00002be0: 5f68 202d 2068 6569 6768 7429 0a0a 2020  _h - height)..  
+00002bf0: 2020 2020 2020 2320 7365 7420 7570 2065        # set up e
+00002c00: 7874 6572 6e61 6c20 626f 756e 6461 7279  xternal boundary
+00002c10: 2061 7320 6c69 7374 206f 6620 636f 6f72   as list of coor
+00002c20: 6469 6e61 7465 730a 2020 2020 2020 2020  dinates.        
+00002c30: 7365 6c66 2e5f 6578 7465 726e 616c 5f62  self._external_b
+00002c40: 6f75 6e64 6172 7920 3d20 5b0a 2020 2020  oundary = [.    
+00002c50: 2020 2020 2020 2020 2830 2c20 3029 2c0a          (0, 0),.
+00002c60: 2020 2020 2020 2020 2020 2020 2830 2c20              (0, 
+00002c70: 746f 705b 315d 292c 0a20 2020 2020 2020  top[1]),.       
+00002c80: 2020 2020 2074 6f70 2c0a 2020 2020 2020       top,.      
+00002c90: 2020 2020 2020 626f 742c 0a20 2020 2020        bot,.     
+00002ca0: 2020 2020 2020 2028 746f 745f 6c2c 2062         (tot_l, b
+00002cb0: 6f74 5b31 5d29 2c0a 2020 2020 2020 2020  ot[1]),.        
+00002cc0: 2020 2020 2874 6f74 5f6c 2c20 3029 2c0a      (tot_l, 0),.
+00002cd0: 2020 2020 2020 2020 2020 2020 2830 2c20              (0, 
+00002ce0: 3029 2c0a 2020 2020 2020 2020 5d0a 0a20  0),.        ].. 
+00002cf0: 2020 2020 2020 2023 2073 6574 2072 656c         # set rel
+00002d00: 6576 616e 7420 7661 7269 6162 6c65 7320  evant variables 
+00002d10: 746f 2073 656c 660a 2020 2020 2020 2020  to self.        
+00002d20: 7365 6c66 2e5f 6c65 6e67 7468 203d 206c  self._length = l
+00002d30: 656e 6774 680a 2020 2020 2020 2020 7365  ength.        se
+00002d40: 6c66 2e5f 6865 6967 6874 203d 2068 6569  lf._height = hei
+00002d50: 6768 740a 2020 2020 2020 2020 7365 6c66  ght.        self
+00002d60: 2e5f 6772 6164 6965 6e74 203d 2068 6569  ._gradient = hei
+00002d70: 6768 7420 2f20 6c65 6e67 7468 0a0a 2020  ght / length..  
+00002d80: 2020 2020 2020 7365 6c66 2e5f 746f 705f        self._top_
+00002d90: 636f 6f72 6420 3d20 746f 700a 2020 2020  coord = top.    
+00002da0: 2020 2020 7365 6c66 2e5f 626f 745f 636f      self._bot_co
+00002db0: 6f72 6420 3d20 626f 740a 0a20 2020 2020  ord = bot..     
+00002dc0: 2020 2073 656c 662e 5f65 7874 6572 6e61     self._externa
+00002dd0: 6c5f 6c65 6e67 7468 203d 2074 6f74 5f6c  l_length = tot_l
+00002de0: 0a20 2020 2020 2020 2073 656c 662e 5f65  .        self._e
+00002df0: 7874 6572 6e61 6c5f 6865 6967 6874 203d  xternal_height =
+00002e00: 2074 6f74 5f68 0a0a 2020 2020 2020 2020   tot_h..        
+00002e10: 2320 7564 6c20 636f 6f72 6469 6e61 7465  # udl coordinate
+00002e20: 7320 6361 6e20 6265 2065 6666 6563 7465  s can be effecte
+00002e30: 6420 6279 2065 7874 6572 6e61 6c20 626f  d by external bo
+00002e40: 756e 6461 7279 206d 6f64 6966 6963 6174  undary modificat
+00002e50: 696f 6e0a 2020 2020 2020 2020 2320 6e65  ion.        # ne
+00002e60: 6564 2074 6f20 7570 6461 7465 2063 6f6f  ed to update coo
+00002e70: 7264 696e 6174 6573 2e0a 2020 2020 2020  rdinates..      
+00002e80: 2020 7365 6c66 2e5f 7570 6461 7465 5f75    self._update_u
+00002e90: 646c 5f63 6f6f 7264 696e 6174 6573 2829  dl_coordinates()
+00002ea0: 0a20 2020 2020 2020 2073 656c 662e 5f75  .        self._u
+00002eb0: 7064 6174 655f 6c6c 5f63 6f6f 7264 696e  pdate_ll_coordin
+00002ec0: 6174 6573 2829 0a0a 2020 2020 2020 2020  ates()..        
+00002ed0: 2320 7265 7365 7420 6c69 6d69 7473 0a20  # reset limits. 
+00002ee0: 2020 2020 2020 2073 656c 662e 7265 6d6f         self.remo
+00002ef0: 7665 5f61 6e61 6c79 7369 735f 6c69 6d69  ve_analysis_limi
+00002f00: 7473 2829 0a0a 2020 2020 2020 2020 2320  ts()..        # 
+00002f10: 7265 7365 7420 7265 7375 6c74 730a 2020  reset results.  
+00002f20: 2020 2020 2020 7365 6c66 2e5f 7265 7365        self._rese
+00002f30: 745f 7265 7375 6c74 7328 290a 0a20 2020  t_results()..   
+00002f40: 2064 6566 2073 6574 5f77 6174 6572 5f74   def set_water_t
+00002f50: 6162 6c65 2873 656c 662c 2064 6570 7468  able(self, depth
+00002f60: 3a20 666c 6f61 7429 3a0a 2020 2020 2020  : float):.      
+00002f70: 2020 2222 2273 6574 2077 6174 6572 2074    """set water t
+00002f80: 6162 6c65 2076 616c 7565 2e0a 0a20 2020  able value...   
+00002f90: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
+00002fa0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+00002fb0: 2d2d 0a20 2020 2020 2020 2064 6570 7468  --.        depth
+00002fc0: 203a 2066 6c6f 6174 0a20 2020 2020 2020   : float.       
+00002fd0: 2020 2020 2064 6570 7468 206f 6620 7761       depth of wa
+00002fe0: 7465 7220 6672 6f6d 2074 6f70 206f 6620  ter from top of 
+00002ff0: 736c 6f70 652e 0a0a 2020 2020 2020 2020  slope...        
+00003000: 4578 616d 706c 6573 0a20 2020 2020 2020  Examples.       
+00003010: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020   ------------.  
+00003020: 2020 2020 2020 3e3e 3e20 7320 3d20 536c        >>> s = Sl
+00003030: 6f70 6528 290a 2020 2020 2020 2020 3e3e  ope().        >>
+00003040: 3e20 732e 7365 745f 7761 7465 725f 7461  > s.set_water_ta
+00003050: 626c 6528 312e 3229 0a20 2020 2020 2020  ble(1.2).       
+00003060: 203e 3e3e 2073 2e5f 7761 7465 725f 6465   >>> s._water_de
+00003070: 7074 680a 2020 2020 2020 2020 312e 320a  pth.        1.2.
+00003080: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
+00003090: 2020 2020 2069 6620 6465 7074 6820 6973       if depth is
+000030a0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000030b0: 2020 2073 656c 662e 7265 6d6f 7665 5f77     self.remove_w
+000030c0: 6174 6572 5f74 6162 6c65 2829 0a20 2020  ater_table().   
+000030d0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+000030e0: 2020 2020 2020 2064 6174 615f 7661 6c69         data_vali
+000030f0: 6461 7469 6f6e 2e61 7373 6572 745f 706f  dation.assert_po
+00003100: 7369 7469 7665 5f6e 756d 6265 7228 6465  sitive_number(de
+00003110: 7074 682c 2022 7761 7465 7220 6465 7074  pth, "water dept
+00003120: 6822 290a 2020 2020 2020 2020 2020 2020  h").            
+00003130: 7365 6c66 2e5f 7761 7465 725f 524c 203d  self._water_RL =
+00003140: 206d 6178 2830 2c20 7365 6c66 2e5f 746f   max(0, self._to
+00003150: 705f 636f 6f72 645b 315d 202d 2064 6570  p_coord[1] - dep
+00003160: 7468 290a 2020 2020 2020 2020 2020 2020  th).            
+00003170: 7365 6c66 2e5f 7761 7465 725f 6465 7074  self._water_dept
+00003180: 6820 3d20 6465 7074 680a 0a20 2020 2020  h = depth..     
+00003190: 2020 2023 2072 6573 6574 2072 6573 756c     # reset resul
+000031a0: 7473 0a20 2020 2020 2020 2073 656c 662e  ts.        self.
+000031b0: 5f72 6573 6574 5f72 6573 756c 7473 2829  _reset_results()
+000031c0: 0a0a 2020 2020 6465 6620 7265 6d6f 7665  ..    def remove
+000031d0: 5f77 6174 6572 5f74 6162 6c65 2873 656c  _water_table(sel
+000031e0: 6629 3a0a 2020 2020 2020 2020 2222 2252  f):.        """R
+000031f0: 656d 6f76 6520 7761 7465 7220 7461 626c  emove water tabl
+00003200: 6520 6672 6f6d 206d 6f64 656c 2e0a 0a20  e from model... 
+00003210: 2020 2020 2020 2045 7861 6d70 6c65 730a         Examples.
+00003220: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+00003230: 2d2d 2d2d 0a20 2020 2020 2020 203e 3e3e  ----.        >>>
+00003240: 2073 203d 2053 6c6f 7065 2829 0a20 2020   s = Slope().   
+00003250: 2020 2020 203e 3e3e 2073 2e73 6574 5f77       >>> s.set_w
+00003260: 6174 6572 5f74 6162 6c65 2831 2e32 290a  ater_table(1.2).
+00003270: 2020 2020 2020 2020 3e3e 3e20 732e 7265          >>> s.re
+00003280: 6d6f 7665 5f77 6174 6572 5f74 6162 6c65  move_water_table
+00003290: 2829 0a20 2020 2020 2020 203e 3e3e 2073  ().        >>> s
+000032a0: 2e5f 7761 7465 725f 524c 203d 3d20 732e  ._water_RL == s.
+000032b0: 5f77 6174 6572 5f64 6570 7468 203d 3d20  _water_depth == 
+000032c0: 4e6f 6e65 0a20 2020 2020 2020 2054 7275  None.        Tru
+000032d0: 650a 2020 2020 2020 2020 2222 220a 2020  e.        """.  
+000032e0: 2020 2020 2020 7365 6c66 2e5f 7761 7465        self._wate
+000032f0: 725f 524c 203d 204e 6f6e 650a 2020 2020  r_RL = None.    
+00003300: 2020 2020 7365 6c66 2e5f 7761 7465 725f      self._water_
+00003310: 6465 7074 6820 3d20 4e6f 6e65 0a0a 2020  depth = None..  
+00003320: 2020 2020 2020 2320 7265 7365 7420 7265        # reset re
+00003330: 7375 6c74 730a 2020 2020 2020 2020 7365  sults.        se
+00003340: 6c66 2e5f 7265 7365 745f 7265 7375 6c74  lf._reset_result
+00003350: 7328 290a 0a20 2020 2064 6566 2073 6574  s()..    def set
+00003360: 5f75 646c 7328 7365 6c66 2c20 2a75 646c  _udls(self, *udl
+00003370: 7329 3a0a 2020 2020 2020 2020 2222 2273  s):.        """s
+00003380: 6574 2061 2073 7572 6661 6365 2073 7572  et a surface sur
+00003390: 6368 6172 6765 206f 6e20 746f 7020 6f66  charge on top of
+000033a0: 2074 6865 2073 6c6f 7065 2e0a 0a20 2020   the slope...   
+000033b0: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
+000033c0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+000033d0: 2d2d 0a20 2020 2020 2020 202a 7564 6c73  --.        *udls
+000033e0: 203a 2055 646c 206f 626a 6563 7473 0a20   : Udl objects. 
+000033f0: 2020 2020 2020 2020 2020 2055 646c 206f             Udl o
+00003400: 626a 6563 7420 746f 2062 6520 6173 7369  bject to be assi
+00003410: 676e 6564 2074 6f20 7468 6520 736c 6f70  gned to the slop
+00003420: 6520 6f62 6a65 6374 2e0a 0a20 2020 2020  e object...     
+00003430: 2020 2045 7861 6d70 6c65 730a 2020 2020     Examples.    
+00003440: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
+00003450: 0a20 2020 2020 2020 203e 3e3e 2073 203d  .        >>> s =
+00003460: 2053 6c6f 7065 2829 0a20 2020 2020 2020   Slope().       
+00003470: 203e 3e3e 2075 3120 3d20 5564 6c28 3529   >>> u1 = Udl(5)
+00003480: 0a20 2020 2020 2020 203e 3e3e 2075 3220  .        >>> u2 
+00003490: 3d20 5564 6c28 3130 290a 2020 2020 2020  = Udl(10).      
+000034a0: 2020 3e3e 3e20 732e 7365 745f 7564 6c73    >>> s.set_udls
+000034b0: 2875 312c 2075 3229 0a20 2020 2020 2020  (u1, u2).       
+000034c0: 203e 3e3e 206c 656e 2873 2e5f 7564 6c73   >>> len(s._udls
+000034d0: 2920 3d3d 2032 0a20 2020 2020 2020 2054  ) == 2.        T
+000034e0: 7275 650a 0a20 2020 2020 2020 2022 2222  rue..        """
+000034f0: 0a0a 2020 2020 2020 2020 666f 7220 7564  ..        for ud
+00003500: 6c20 696e 2075 646c 733a 0a20 2020 2020  l in udls:.     
+00003510: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+00003520: 616e 6365 2875 646c 2c20 5564 6c29 3a0a  ance(udl, Udl):.
+00003530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003540: 6966 2075 646c 2e6d 6167 6e69 7475 6465  if udl.magnitude
+00003550: 203e 2030 3a0a 2020 2020 2020 2020 2020   > 0:.          
+00003560: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00003570: 7564 6c73 2e61 7070 656e 6428 7564 6c29  udls.append(udl)
+00003580: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003590: 2020 2020 2020 2320 7570 6461 7465 2074        # update t
+000035a0: 6f20 6d61 6b65 2073 7572 6520 6675 6c6c  o make sure full
+000035b0: 206c 6f61 6420 6973 2069 6e63 6c75 6465   load is include
+000035c0: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
+000035d0: 2020 2020 2020 6d69 6e5f 6c65 6e67 7468        min_length
+000035e0: 203d 2028 7564 6c2e 6f66 6673 6574 202b   = (udl.offset +
+000035f0: 2028 7564 6c2e 6c65 6e67 7468 206f 7220   (udl.length or 
+00003600: 3329 2920 2a20 322e 350a 2020 2020 2020  3)) * 2.5.      
+00003610: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00003620: 2073 656c 662e 5f4d 494e 5f45 5854 5f4c   self._MIN_EXT_L
+00003630: 203c 206d 696e 5f6c 656e 6774 683a 0a20   < min_length:. 
+00003640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003650: 2020 2020 2020 2073 656c 662e 7570 6461         self.upda
+00003660: 7465 5f62 6f75 6e64 6172 795f 6f70 7469  te_boundary_opti
+00003670: 6f6e 7328 4d49 4e5f 4558 545f 4c3d 6d69  ons(MIN_EXT_L=mi
+00003680: 6e5f 6c65 6e67 7468 290a 0a20 2020 2020  n_length)..     
+00003690: 2020 2073 656c 662e 5f75 7064 6174 655f     self._update_
+000036a0: 7564 6c5f 636f 6f72 6469 6e61 7465 7328  udl_coordinates(
+000036b0: 290a 0a20 2020 2020 2020 2069 6620 7365  )..        if se
+000036c0: 6c66 2e5f 7564 6c73 3a0a 2020 2020 2020  lf._udls:.      
+000036d0: 2020 2020 2020 7365 6c66 2e5f 7564 6c5f        self._udl_
+000036e0: 6d61 7820 3d20 6d61 7828 7564 6c2e 6d61  max = max(udl.ma
+000036f0: 676e 6974 7564 6520 666f 7220 7564 6c20  gnitude for udl 
+00003700: 696e 2073 656c 662e 5f75 646c 7329 0a0a  in self._udls)..
+00003710: 2020 2020 2020 2020 2320 7265 7365 7420          # reset 
+00003720: 7265 7375 6c74 730a 2020 2020 2020 2020  results.        
+00003730: 7365 6c66 2e5f 7265 7365 745f 7265 7375  self._reset_resu
+00003740: 6c74 7328 290a 0a20 2020 2023 2064 6f6e  lts()..    # don
+00003750: 7420 6e65 6564 2074 6f20 7265 7365 7420  t need to reset 
+00003760: 7265 7375 6c74 7320 7369 6e63 6520 7468  results since th
+00003770: 6973 206f 6e6c 7920 7368 6f75 6c64 2062  is only should b
+00003780: 6520 6361 6c6c 6564 0a20 2020 2023 2061  e called.    # a
+00003790: 7320 6120 7061 7274 206f 6620 7265 7365  s a part of rese
+000037a0: 7474 696e 670a 2020 2020 6465 6620 5f75  tting.    def _u
+000037b0: 7064 6174 655f 7564 6c5f 636f 6f72 6469  pdate_udl_coordi
+000037c0: 6e61 7465 7328 7365 6c66 293a 0a20 2020  nates(self):.   
+000037d0: 2020 2020 2022 5570 6461 7465 2063 6f6f       "Update coo
+000037e0: 7264 696e 6174 6573 2066 6f72 206c 6566  rdinates for lef
+000037f0: 7420 616e 6420 7269 6768 7420 6f66 2075  t and right of u
+00003800: 646c 2062 6173 6564 206f 6e20 6578 7465  dl based on exte
+00003810: 726e 616c 2062 6f75 6e64 6172 7920 616e  rnal boundary an
+00003820: 6420 5564 6c20 6f62 6a65 6374 220a 0a20  d Udl object".. 
+00003830: 2020 2020 2020 2066 6f72 2075 646c 2069         for udl i
+00003840: 6e20 7365 6c66 2e5f 7564 6c73 3a0a 2020  n self._udls:.  
+00003850: 2020 2020 2020 2020 2020 7269 6768 745f            right_
+00003860: 7820 3d20 7365 6c66 2e5f 746f 705f 636f  x = self._top_co
+00003870: 6f72 645b 305d 202d 2075 646c 2e6f 6666  ord[0] - udl.off
+00003880: 7365 740a 2020 2020 2020 2020 2020 2020  set.            
+00003890: 6966 2075 646c 2e6c 656e 6774 683a 0a20  if udl.length:. 
+000038a0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+000038b0: 6566 745f 7820 3d20 6d61 7828 302c 2072  eft_x = max(0, r
+000038c0: 6967 6874 5f78 202d 2075 646c 2e6c 656e  ight_x - udl.len
+000038d0: 6774 6829 0a20 2020 2020 2020 2020 2020  gth).           
+000038e0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000038f0: 2020 2020 2020 206c 6566 745f 7820 3d20         left_x = 
+00003900: 300a 0a20 2020 2020 2020 2020 2020 2075  0..            u
+00003910: 646c 2e6c 6566 7420 3d20 6c65 6674 5f78  dl.left = left_x
+00003920: 0a20 2020 2020 2020 2020 2020 2075 646c  .            udl
+00003930: 2e72 6967 6874 203d 2072 6967 6874 5f78  .right = right_x
+00003940: 0a0a 2020 2020 6465 6620 7265 6d6f 7665  ..    def remove
+00003950: 5f75 646c 7328 7365 6c66 2c20 2a75 646c  _udls(self, *udl
+00003960: 732c 2072 656d 6f76 655f 616c 6c3d 4661  s, remove_all=Fa
+00003970: 6c73 6529 3a0a 2020 2020 2020 2020 2222  lse):.        ""
+00003980: 2252 656d 6f76 6520 7564 6c20 6672 6f6d  "Remove udl from
+00003990: 206d 6f64 656c 2069 6620 6173 736f 6369   model if associ
+000039a0: 6174 6564 2077 6974 6820 6d6f 6465 6c2e  ated with model.
+000039b0: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+000039c0: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
+000039d0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+000039e0: 2a75 646c 7320 3a20 5564 6c20 6f62 6a65  *udls : Udl obje
+000039f0: 6374 730a 2020 2020 2020 2020 2020 2020  cts.            
+00003a00: 5564 6c20 6f62 6a65 6374 2074 6f20 6265  Udl object to be
+00003a10: 2072 656d 6f76 6564 2066 726f 6d20 7468   removed from th
+00003a20: 6520 736c 6f70 6520 6f62 6a65 6374 2e0a  e slope object..
+00003a30: 2020 2020 2020 2020 7265 6d6f 7665 5f61          remove_a
+00003a40: 6c6c 203a 2062 6f6f 6c2c 206f 7074 696f  ll : bool, optio
+00003a50: 6e61 6c0a 2020 2020 2020 2020 2020 2020  nal.            
+00003a60: 4966 2074 7275 6520 7265 6d6f 7665 2061  If true remove a
+00003a70: 6c6c 2075 646c 732c 2062 7920 6465 6661  ll udls, by defa
+00003a80: 756c 7420 4661 6c73 650a 0a20 2020 2020  ult False..     
+00003a90: 2020 2045 7861 6d70 6c65 730a 2020 2020     Examples.    
+00003aa0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
+00003ab0: 0a20 2020 2020 2020 203e 3e3e 2073 203d  .        >>> s =
+00003ac0: 2053 6c6f 7065 2829 0a20 2020 2020 2020   Slope().       
+00003ad0: 203e 3e3e 2075 312c 2075 3220 3d20 5564   >>> u1, u2 = Ud
+00003ae0: 6c28 3529 2c20 5564 6c28 3130 290a 2020  l(5), Udl(10).  
+00003af0: 2020 2020 2020 3e3e 3e20 732e 7365 745f        >>> s.set_
+00003b00: 7564 6c73 2875 312c 2075 3229 0a20 2020  udls(u1, u2).   
+00003b10: 2020 2020 203e 3e3e 2073 2e72 656d 6f76       >>> s.remov
+00003b20: 655f 7564 6c73 2875 3129 0a20 2020 2020  e_udls(u1).     
+00003b30: 2020 203e 3e3e 206c 656e 2873 2e5f 7564     >>> len(s._ud
+00003b40: 6c73 2920 3d3d 2031 0a20 2020 2020 2020  ls) == 1.       
+00003b50: 2054 7275 650a 2020 2020 2020 2020 3e3e   True.        >>
+00003b60: 3e20 732e 7265 6d6f 7665 5f75 646c 7328  > s.remove_udls(
+00003b70: 7265 6d6f 7665 5f61 6c6c 3d54 7275 6529  remove_all=True)
+00003b80: 0a20 2020 2020 2020 203e 3e3e 206c 656e  .        >>> len
+00003b90: 2873 2e5f 7564 6c73 2920 3d3d 2030 0a20  (s._udls) == 0. 
+00003ba0: 2020 2020 2020 2054 7275 650a 2020 2020         True.    
+00003bb0: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+00003bc0: 2066 6f72 2075 646c 2069 6e20 7564 6c73   for udl in udls
+00003bd0: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
+00003be0: 7220 6368 6563 6b5f 7564 6c20 696e 2073  r check_udl in s
+00003bf0: 656c 662e 5f75 646c 733a 0a20 2020 2020  elf._udls:.     
+00003c00: 2020 2020 2020 2020 2020 2069 6620 280a             if (.
+00003c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c20: 2020 2020 6368 6563 6b5f 7564 6c2e 6f66      check_udl.of
+00003c30: 6673 6574 203d 3d20 7564 6c2e 6f66 6673  fset == udl.offs
+00003c40: 6574 0a20 2020 2020 2020 2020 2020 2020  et.             
+00003c50: 2020 2020 2020 2061 6e64 2063 6865 636b         and check
+00003c60: 5f75 646c 2e6d 6167 6e69 7475 6465 203d  _udl.magnitude =
+00003c70: 3d20 7564 6c2e 6d61 676e 6974 7564 650a  = udl.magnitude.
+00003c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c90: 2020 2020 616e 6420 6368 6563 6b5f 7564      and check_ud
+00003ca0: 6c2e 6c65 6e67 7468 203d 3d20 7564 6c2e  l.length == udl.
+00003cb0: 6c65 6e67 7468 0a20 2020 2020 2020 2020  length.         
+00003cc0: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
+00003cd0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00003ce0: 6c66 2e5f 7564 6c73 2e72 656d 6f76 6528  lf._udls.remove(
+00003cf0: 6368 6563 6b5f 7564 6c29 0a0a 2020 2020  check_udl)..    
+00003d00: 2020 2020 6966 2072 656d 6f76 655f 616c      if remove_al
+00003d10: 6c3a 0a20 2020 2020 2020 2020 2020 2073  l:.            s
+00003d20: 656c 662e 5f75 646c 7320 3d20 5b5d 0a20  elf._udls = []. 
+00003d30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00003d40: 5f75 646c 5f6d 6178 203d 2030 0a0a 2020  _udl_max = 0..  
+00003d50: 2020 2020 2020 6966 2073 656c 662e 5f75        if self._u
+00003d60: 646c 733a 0a20 2020 2020 2020 2020 2020  dls:.           
+00003d70: 2073 656c 662e 5f75 646c 5f6d 6178 203d   self._udl_max =
+00003d80: 206d 6178 2873 656c 662e 5f75 646c 732c   max(self._udls,
+00003d90: 206b 6579 3d6c 616d 6264 6120 783a 2078   key=lambda x: x
+00003da0: 2e6d 6167 6e69 7475 6465 290a 0a20 2020  .magnitude)..   
+00003db0: 2020 2020 2023 2072 6573 6574 2072 6573       # reset res
+00003dc0: 756c 7473 0a20 2020 2020 2020 2073 656c  ults.        sel
+00003dd0: 662e 5f72 6573 6574 5f72 6573 756c 7473  f._reset_results
+00003de0: 2829 0a0a 2020 2020 6465 6620 7365 745f  ()..    def set_
+00003df0: 6c6c 7328 7365 6c66 2c20 2a6c 6c73 293a  lls(self, *lls):
+00003e00: 0a20 2020 2020 2020 2022 2222 7365 7420  .        """set 
+00003e10: 6120 7375 7266 6163 6520 7375 7263 6861  a surface surcha
+00003e20: 7267 6520 6f6e 2074 6f70 206f 6620 7468  rge on top of th
+00003e30: 6520 736c 6f70 650a 0a20 2020 2020 2020  e slope..       
+00003e40: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00003e50: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
+00003e60: 2d2d 2d2d 2d0a 2020 2020 2020 2020 2a6c  -----.        *l
+00003e70: 6c73 203a 204c 696e 654c 6f61 6420 6f62  ls : LineLoad ob
+00003e80: 6a65 6374 730a 2020 2020 2020 2020 2020  jects.          
+00003e90: 2020 4c69 6e65 4c6f 6164 206f 626a 6563    LineLoad objec
+00003ea0: 7420 746f 2062 6520 6173 7369 676e 6564  t to be assigned
+00003eb0: 2074 6f20 7468 6520 736c 6f70 6520 6f62   to the slope ob
+00003ec0: 6a65 6374 2e0a 0a20 2020 2020 2020 2045  ject...        E
+00003ed0: 7861 6d70 6c65 730a 2020 2020 2020 2020  xamples.        
+00003ee0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
+00003ef0: 2020 2020 203e 3e3e 2073 203d 2053 6c6f       >>> s = Slo
+00003f00: 7065 2829 0a20 2020 2020 2020 203e 3e3e  pe().        >>>
+00003f10: 206c 6c31 203d 204c 696e 654c 6f61 6428   ll1 = LineLoad(
+00003f20: 3529 0a20 2020 2020 2020 203e 3e3e 206c  5).        >>> l
+00003f30: 6c32 203d 204c 696e 654c 6f61 6428 3130  l2 = LineLoad(10
+00003f40: 290a 2020 2020 2020 2020 3e3e 3e20 732e  ).        >>> s.
+00003f50: 7365 745f 6c6c 7328 6c6c 312c 206c 6c32  set_lls(ll1, ll2
+00003f60: 290a 2020 2020 2020 2020 3e3e 3e20 6c65  ).        >>> le
+00003f70: 6e28 732e 5f6c 6c73 2920 3d3d 2032 0a20  n(s._lls) == 2. 
+00003f80: 2020 2020 2020 2054 7275 650a 0a20 2020         True..   
+00003f90: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+00003fa0: 2020 666f 7220 6c6c 2069 6e20 6c6c 733a    for ll in lls:
+00003fb0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00003fc0: 6973 696e 7374 616e 6365 286c 6c2c 204c  isinstance(ll, L
+00003fd0: 696e 654c 6f61 6429 3a0a 2020 2020 2020  ineLoad):.      
+00003fe0: 2020 2020 2020 2020 2020 6966 206c 6c2e            if ll.
+00003ff0: 6d61 676e 6974 7564 6520 3e20 303a 0a20  magnitude > 0:. 
+00004000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004010: 2020 2073 656c 662e 5f6c 6c73 2e61 7070     self._lls.app
+00004020: 656e 6428 6c6c 290a 0a20 2020 2020 2020  end(ll)..       
+00004030: 2020 2020 2020 2020 2020 2020 2023 2075               # u
+00004040: 7064 6174 6520 746f 206d 616b 6520 7375  pdate to make su
+00004050: 7265 2066 756c 6c20 6c6f 6164 2069 7320  re full load is 
+00004060: 696e 636c 7564 6564 0a20 2020 2020 2020  included.       
+00004070: 2020 2020 2020 2020 2020 2020 206d 696e               min
+00004080: 5f6c 656e 6774 6820 3d20 6c6c 2e6f 6666  _length = ll.off
+00004090: 7365 7420 2a20 330a 2020 2020 2020 2020  set * 3.        
+000040a0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+000040b0: 656c 662e 5f4d 494e 5f45 5854 5f4c 203c  elf._MIN_EXT_L <
+000040c0: 206d 696e 5f6c 656e 6774 683a 0a20 2020   min_length:.   
+000040d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000040e0: 2020 2020 2073 656c 662e 7570 6461 7465       self.update
+000040f0: 5f62 6f75 6e64 6172 795f 6f70 7469 6f6e  _boundary_option
+00004100: 7328 4d49 4e5f 4558 545f 4c3d 6d69 6e5f  s(MIN_EXT_L=min_
+00004110: 6c65 6e67 7468 290a 0a20 2020 2020 2020  length)..       
+00004120: 2073 656c 662e 5f75 7064 6174 655f 6c6c   self._update_ll
+00004130: 5f63 6f6f 7264 696e 6174 6573 2829 0a0a  _coordinates()..
+00004140: 2020 2020 2020 2020 2320 7265 7365 7420          # reset 
+00004150: 7265 7375 6c74 730a 2020 2020 2020 2020  results.        
+00004160: 7365 6c66 2e5f 7265 7365 745f 7265 7375  self._reset_resu
+00004170: 6c74 7328 290a 0a20 2020 2023 2064 6f6e  lts()..    # don
+00004180: 7420 6e65 6564 2074 6f20 7265 7365 7420  t need to reset 
+00004190: 7265 7375 6c74 7320 7369 6e63 6520 7468  results since th
+000041a0: 6973 206f 6e6c 7920 7368 6f75 6c64 2062  is only should b
+000041b0: 6520 6361 6c6c 6564 0a20 2020 2023 2061  e called.    # a
+000041c0: 7320 6120 7061 7274 206f 6620 7265 7365  s a part of rese
+000041d0: 7474 696e 670a 2020 2020 6465 6620 5f75  tting.    def _u
+000041e0: 7064 6174 655f 6c6c 5f63 6f6f 7264 696e  pdate_ll_coordin
+000041f0: 6174 6573 2873 656c 6629 3a0a 2020 2020  ates(self):.    
+00004200: 2020 2020 2255 7064 6174 6520 636f 6f72      "Update coor
+00004210: 6469 6e61 7465 7320 666f 7220 706f 696e  dinates for poin
+00004220: 7420 6c6f 6164 2062 6173 6564 206f 6e20  t load based on 
+00004230: 6578 7465 726e 616c 2062 6f75 6e64 6172  external boundar
+00004240: 7920 616e 6420 4c69 6e65 4c6f 6164 206f  y and LineLoad o
+00004250: 626a 6563 7422 0a0a 2020 2020 2020 2020  bject"..        
+00004260: 666f 7220 6c6c 2069 6e20 7365 6c66 2e5f  for ll in self._
+00004270: 6c6c 733a 0a20 2020 2020 2020 2020 2020  lls:.           
+00004280: 2063 6f6f 7264 203d 206d 6178 2830 2c20   coord = max(0, 
+00004290: 7365 6c66 2e5f 746f 705f 636f 6f72 645b  self._top_coord[
+000042a0: 305d 202d 206c 6c2e 6f66 6673 6574 290a  0] - ll.offset).
+000042b0: 0a20 2020 2020 2020 2020 2020 206c 6c2e  .            ll.
+000042c0: 636f 6f72 6420 3d20 636f 6f72 640a 0a20  coord = coord.. 
+000042d0: 2020 2064 6566 2072 656d 6f76 655f 6c6c     def remove_ll
+000042e0: 7328 7365 6c66 2c20 2a6c 6c73 2c20 7265  s(self, *lls, re
+000042f0: 6d6f 7665 5f61 6c6c 3d46 616c 7365 293a  move_all=False):
+00004300: 0a20 2020 2020 2020 2022 2222 5265 6d6f  .        """Remo
+00004310: 7665 2075 646c 2066 726f 6d20 6d6f 6465  ve udl from mode
+00004320: 6c20 6966 2061 7373 6f63 6961 7465 6420  l if associated 
+00004330: 7769 7468 206d 6f64 656c 2e0a 0a20 2020  with model...   
+00004340: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
+00004350: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+00004360: 2d2d 0a20 2020 2020 2020 202a 6c6c 7320  --.        *lls 
+00004370: 3a20 4c69 6e65 4c6f 6164 206f 626a 6563  : LineLoad objec
+00004380: 7473 0a20 2020 2020 2020 2020 2020 204c  ts.            L
+00004390: 696e 654c 6f61 6420 6f62 6a65 6374 2074  ineLoad object t
+000043a0: 6f20 6265 2072 656d 6f76 6564 2066 726f  o be removed fro
+000043b0: 6d20 7468 6520 736c 6f70 6520 6f62 6a65  m the slope obje
+000043c0: 6374 2e0a 2020 2020 2020 2020 7265 6d6f  ct..        remo
+000043d0: 7665 5f61 6c6c 203a 2062 6f6f 6c2c 206f  ve_all : bool, o
+000043e0: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+000043f0: 2020 2020 6966 2074 7275 6520 7265 6d6f      if true remo
+00004400: 7665 2061 6c6c 206c 6c73 2c20 6279 2064  ve all lls, by d
+00004410: 6566 6175 6c74 2046 616c 7365 0a0a 2020  efault False..  
+00004420: 2020 2020 2020 4578 616d 706c 6573 0a20        Examples. 
+00004430: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+00004440: 2d2d 2d0a 2020 2020 2020 2020 3e3e 3e20  ---.        >>> 
+00004450: 7320 3d20 536c 6f70 6528 290a 2020 2020  s = Slope().    
+00004460: 2020 2020 3e3e 3e20 6c6c 3120 3d20 4c69      >>> ll1 = Li
+00004470: 6e65 4c6f 6164 2835 290a 2020 2020 2020  neLoad(5).      
+00004480: 2020 3e3e 3e20 6c6c 3220 3d20 4c69 6e65    >>> ll2 = Line
+00004490: 4c6f 6164 2831 3029 0a20 2020 2020 2020  Load(10).       
+000044a0: 203e 3e3e 2073 2e73 6574 5f6c 6c73 286c   >>> s.set_lls(l
+000044b0: 6c31 2c20 6c6c 3229 0a20 2020 2020 2020  l1, ll2).       
+000044c0: 203e 3e3e 2073 2e72 656d 6f76 655f 6c6c   >>> s.remove_ll
+000044d0: 7328 6c6c 3129 0a20 2020 2020 2020 203e  s(ll1).        >
+000044e0: 3e3e 206c 656e 2873 2e5f 6c6c 7329 203d  >> len(s._lls) =
+000044f0: 3d20 310a 2020 2020 2020 2020 5472 7565  = 1.        True
+00004500: 0a20 2020 2020 2020 203e 3e3e 2073 2e72  .        >>> s.r
+00004510: 656d 6f76 655f 6c6c 7328 7265 6d6f 7665  emove_lls(remove
+00004520: 5f61 6c6c 3d54 7275 6529 0a20 2020 2020  _all=True).     
+00004530: 2020 203e 3e3e 206c 656e 2873 2e5f 6c6c     >>> len(s._ll
+00004540: 7329 203d 3d20 300a 2020 2020 2020 2020  s) == 0.        
+00004550: 5472 7565 0a20 2020 2020 2020 2022 2222  True.        """
+00004560: 0a0a 2020 2020 2020 2020 2320 6361 6e20  ..        # can 
+00004570: 7072 6f62 6162 6c79 2077 7269 7465 2074  probably write t
+00004580: 6869 7320 6173 204f 286e 2920 7261 7468  his as O(n) rath
+00004590: 6572 2074 6861 6e20 4f28 6e5e 3229 0a20  er than O(n^2). 
+000045a0: 2020 2020 2020 2066 6f72 206c 6c20 696e         for ll in
+000045b0: 206c 6c73 3a0a 2020 2020 2020 2020 2020   lls:.          
+000045c0: 2020 666f 7220 6368 6563 6b5f 6c6c 2069    for check_ll i
+000045d0: 6e20 7365 6c66 2e5f 6c6c 733a 0a20 2020  n self._lls:.   
+000045e0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000045f0: 6368 6563 6b5f 6c6c 2e6f 6666 7365 7420  check_ll.offset 
+00004600: 3d3d 206c 6c2e 6f66 6673 6574 2061 6e64  == ll.offset and
+00004610: 2063 6865 636b 5f6c 6c2e 6d61 676e 6974   check_ll.magnit
+00004620: 7564 6520 3d3d 206c 6c2e 6d61 676e 6974  ude == ll.magnit
+00004630: 7564 653a 0a20 2020 2020 2020 2020 2020  ude:.           
+00004640: 2020 2020 2020 2020 2073 656c 662e 5f6c           self._l
+00004650: 6c73 2e72 656d 6f76 6528 6368 6563 6b5f  ls.remove(check_
+00004660: 6c6c 290a 0a20 2020 2020 2020 2069 6620  ll)..        if 
+00004670: 7265 6d6f 7665 5f61 6c6c 3a0a 2020 2020  remove_all:.    
+00004680: 2020 2020 2020 2020 7365 6c66 2e5f 6c6c          self._ll
+00004690: 7320 3d20 5b5d 0a0a 2020 2020 2020 2020  s = []..        
+000046a0: 2320 7265 7365 7420 7265 7375 6c74 730a  # reset results.
+000046b0: 2020 2020 2020 2020 7365 6c66 2e5f 7265          self._re
+000046c0: 7365 745f 7265 7375 6c74 7328 290a 0a20  set_results().. 
+000046d0: 2020 2064 6566 2073 6574 5f6d 6174 6572     def set_mater
+000046e0: 6961 6c73 2873 656c 662c 202a 6d61 7465  ials(self, *mate
+000046f0: 7269 616c 7329 3a0a 2020 2020 2020 2020  rials):.        
+00004700: 2222 2241 7373 6967 6e20 6d61 7465 7269  """Assign materi
+00004710: 616c 2069 6e73 7461 6e63 6573 2074 6f20  al instances to 
+00004720: 7468 6520 736c 6f70 6520 696e 7374 616e  the slope instan
+00004730: 6365 2e0a 0a20 2020 2020 2020 2050 6172  ce...        Par
+00004740: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+00004750: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+00004760: 2020 202a 6d61 7465 7269 616c 7320 3a20     *materials : 
+00004770: 4d61 7465 7269 616c 2028 6c69 7374 292c  Material (list),
+00004780: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+00004790: 2020 2020 2020 4d61 7465 7269 616c 2069        Material i
+000047a0: 6e73 7461 6e63 6573 2074 6f20 6265 2061  nstances to be a
+000047b0: 7373 6f63 6961 7465 6420 7769 7468 2073  ssociated with s
+000047c0: 6c6f 7065 2e0a 0a20 2020 2020 2020 2052  lope...        R
+000047d0: 6169 7365 730a 2020 2020 2020 2020 2d2d  aises.        --
+000047e0: 2d2d 2d2d 0a20 2020 2020 2020 2056 616c  ----.        Val
+000047f0: 7565 4572 726f 720a 2020 2020 2020 2020  ueError.        
+00004800: 2020 2020 4966 206d 6174 6572 6961 6c20      If material 
+00004810: 6e6f 7420 696e 7374 616e 6365 206f 6620  not instance of 
+00004820: 4d61 7465 7269 616c 2063 6c61 7373 2065  Material class e
+00004830: 7272 6f72 2069 7320 7261 6973 6564 2e0a  rror is raised..
+00004840: 2020 2020 2020 2020 5661 6c75 6545 7272          ValueErr
+00004850: 6f72 0a20 2020 2020 2020 2020 2020 2049  or.            I
+00004860: 6620 6e6f 6e2d 756e 6971 7565 206d 6174  f non-unique mat
+00004870: 6572 6961 6c20 6465 7074 6873 2074 6865  erial depths the
+00004880: 6e20 6572 726f 7220 6973 2072 6169 7365  n error is raise
+00004890: 642e 0a0a 2020 2020 2020 2020 4578 616d  d...        Exam
+000048a0: 706c 6573 0a20 2020 2020 2020 202d 2d2d  ples.        ---
+000048b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
+000048c0: 2020 2020 2020 203e 3e3e 2073 203d 2053         >>> s = S
+000048d0: 6c6f 7065 2829 0a20 2020 2020 2020 203e  lope().        >
+000048e0: 3e3e 206d 3120 3d20 4d61 7465 7269 616c  >> m1 = Material
+000048f0: 2829 0a20 2020 2020 2020 203e 3e3e 206d  ().        >>> m
+00004900: 3220 3d20 4d61 7465 7269 616c 2875 6e69  2 = Material(uni
+00004910: 745f 7765 6967 6874 203d 2031 382c 636f  t_weight = 18,co
+00004920: 6865 7369 6f6e 3d32 2c20 6672 6963 7469  hesion=2, fricti
+00004930: 6f6e 5f61 6e67 6c65 203d 2033 302c 6465  on_angle = 30,de
+00004940: 7074 685f 746f 5f62 6f74 746f 6d20 3d20  pth_to_bottom = 
+00004950: 312e 3332 290a 2020 2020 2020 2020 3e3e  1.32).        >>
+00004960: 3e20 732e 7365 745f 6d61 7465 7269 616c  > s.set_material
+00004970: 7328 6d31 2c20 6d32 290a 2020 2020 2020  s(m1, m2).      
+00004980: 2020 3e3e 3e20 6c65 6e28 732e 5f6d 6174    >>> len(s._mat
+00004990: 6572 6961 6c73 2920 3d3d 2032 0a20 2020  erials) == 2.   
+000049a0: 2020 2020 2054 7275 650a 2020 2020 2020       True.      
+000049b0: 2020 3e3e 3e20 732e 7265 6d6f 7665 5f6d    >>> s.remove_m
+000049c0: 6174 6572 6961 6c28 6d31 290a 2020 2020  aterial(m1).    
+000049d0: 2020 2020 3e3e 3e20 6c65 6e28 732e 5f6d      >>> len(s._m
+000049e0: 6174 6572 6961 6c73 2920 3d3d 2031 0a20  aterials) == 1. 
+000049f0: 2020 2020 2020 2054 7275 650a 2020 2020         True.    
+00004a00: 2020 2020 3e3e 3e20 732e 7265 6d6f 7665      >>> s.remove
+00004a10: 5f6d 6174 6572 6961 6c28 7265 6d6f 7665  _material(remove
+00004a20: 5f61 6c6c 3d54 7275 6529 0a20 2020 2020  _all=True).     
+00004a30: 2020 203e 3e3e 206c 656e 2873 2e5f 6d61     >>> len(s._ma
+00004a40: 7465 7269 616c 7329 203d 3d20 300a 2020  terials) == 0.  
+00004a50: 2020 2020 2020 5472 7565 0a0a 2020 2020        True..    
+00004a60: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+00004a70: 2023 2063 6865 636b 206d 6174 6572 6961   # check materia
+00004a80: 6c20 6f62 6a65 6374 2065 6e74 6572 6564  l object entered
+00004a90: 0a20 2020 2020 2020 2066 6f72 206d 6174  .        for mat
+00004aa0: 6572 6961 6c20 696e 206d 6174 6572 6961  erial in materia
+00004ab0: 6c73 3a0a 2020 2020 2020 2020 2020 2020  ls:.            
+00004ac0: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
+00004ad0: 6528 6d61 7465 7269 616c 2c20 4d61 7465  e(material, Mate
+00004ae0: 7269 616c 293a 0a20 2020 2020 2020 2020  rial):.         
+00004af0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00004b00: 7565 4572 726f 7228 0a20 2020 2020 2020  ueError(.       
+00004b10: 2020 2020 2020 2020 2020 2020 2022 5468               "Th
+00004b20: 6520 6675 6e63 7469 6f6e 2061 6464 5f6d  e function add_m
+00004b30: 6174 6572 6961 6c73 206f 6e6c 7920 6163  aterials only ac
+00004b40: 6365 7074 7320 696e 7374 616e 6365 7320  cepts instances 
+00004b50: 6f66 2074 6865 204d 6174 6572 6961 6c20  of the Material 
+00004b60: 436c 6173 7322 0a20 2020 2020 2020 2020  Class".         
+00004b70: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00004b80: 2020 2320 4e65 6564 2074 6f20 7661 6c69    # Need to vali
+00004b90: 6461 7465 206d 6174 6572 6961 6c20 7661  date material va
+00004ba0: 6c75 6573 2061 6c73 6f0a 0a20 2020 2020  lues also..     
+00004bb0: 2020 2023 2073 6f72 7420 6d61 7465 7269     # sort materi
+00004bc0: 616c 7320 746f 2062 6520 696e 206f 7264  als to be in ord
+00004bd0: 6572 2c20 696e 636c 7564 6520 6578 6973  er, include exis
+00004be0: 7469 6e67 206d 6174 6572 6961 6c73 0a20  ting materials. 
+00004bf0: 2020 2020 2020 206d 6174 6572 6961 6c73         materials
+00004c00: 203d 206c 6973 7428 6d61 7465 7269 616c   = list(material
+00004c10: 7329 202b 2073 656c 662e 5f6d 6174 6572  s) + self._mater
+00004c20: 6961 6c73 0a20 2020 2020 2020 206d 6174  ials.        mat
+00004c30: 6572 6961 6c73 2e73 6f72 7428 6b65 793d  erials.sort(key=
+00004c40: 6c61 6d62 6461 2078 3a20 782e 6465 7074  lambda x: x.dept
+00004c50: 685f 746f 5f62 6f74 746f 6d29 0a0a 2020  h_to_bottom)..  
+00004c60: 2020 2020 2020 6465 7074 6873 203d 205b        depths = [
+00004c70: 6d61 7465 7269 616c 2e64 6570 7468 5f74  material.depth_t
+00004c80: 6f5f 626f 7474 6f6d 2066 6f72 206d 6174  o_bottom for mat
+00004c90: 6572 6961 6c20 696e 206d 6174 6572 6961  erial in materia
+00004ca0: 6c73 5d0a 0a20 2020 2020 2020 2023 2069  ls]..        # i
+00004cb0: 6620 6765 6f6c 6f67 6963 616c 2075 6e69  f geological uni
+00004cc0: 7420 6465 6570 6572 2074 6861 6e20 6d6f  t deeper than mo
+00004cd0: 6465 6c20 7468 616e 2065 7874 656e 6420  del than extend 
+00004ce0: 6d6f 6465 6c20 746f 2066 6974 206d 6174  model to fit mat
+00004cf0: 6572 6961 6c73 0a20 2020 2020 2020 2069  erials.        i
+00004d00: 6620 6465 7074 6873 5b2d 315d 203e 2073  f depths[-1] > s
+00004d10: 656c 662e 5f65 7874 6572 6e61 6c5f 6865  elf._external_he
+00004d20: 6967 6874 3a0a 2020 2020 2020 2020 2020  ight:.          
+00004d30: 2020 7365 6c66 2e75 7064 6174 655f 626f    self.update_bo
+00004d40: 756e 6461 7279 5f6f 7074 696f 6e73 284d  undary_options(M
+00004d50: 494e 5f45 5854 5f48 3d64 6570 7468 735b  IN_EXT_H=depths[
+00004d60: 2d31 5d29 0a0a 2020 2020 2020 2020 2320  -1])..        # 
+00004d70: 6368 6563 6b20 6d61 7465 7269 616c 2064  check material d
+00004d80: 6570 7468 2075 6e69 7175 650a 2020 2020  epth unique.    
+00004d90: 2020 2020 6966 206c 656e 2864 6570 7468      if len(depth
+00004da0: 7329 203e 206c 656e 2873 6574 2864 6570  s) > len(set(dep
+00004db0: 7468 7329 293a 0a20 2020 2020 2020 2020  ths)):.         
+00004dc0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+00004dd0: 726f 7228 2254 6865 2073 616d 6520 6d61  ror("The same ma
+00004de0: 7465 7269 616c 2064 6570 7468 2068 6173  terial depth has
+00004df0: 2062 6565 6e20 696e 7075 7420 7477 6963   been input twic
+00004e00: 6522 290a 0a20 2020 2020 2020 206d 6174  e")..        mat
+00004e10: 6572 6961 6c5f 7265 6669 6e65 6420 3d20  erial_refined = 
+00004e20: 5b5d 0a20 2020 2020 2020 2023 2064 6566  [].        # def
+00004e30: 696e 6520 524c 2066 6f72 2065 6163 6820  ine RL for each 
+00004e40: 6d61 7465 7269 616c 2061 6e64 2063 6f6c  material and col
+00004e50: 6f72 2066 6f72 2065 6163 6820 6d61 7465  or for each mate
+00004e60: 7269 616c 0a20 2020 2020 2020 2066 6f72  rial.        for
+00004e70: 2069 2c20 6d61 7465 7269 616c 2069 6e20   i, material in 
+00004e80: 656e 756d 6572 6174 6528 6d61 7465 7269  enumerate(materi
+00004e90: 616c 7329 3a0a 2020 2020 2020 2020 2020  als):.          
+00004ea0: 2020 6d61 7465 7269 616c 2e52 4c20 3d20    material.RL = 
+00004eb0: 7365 6c66 2e5f 6578 7465 726e 616c 5f68  self._external_h
+00004ec0: 6569 6768 7420 2d20 6d61 7465 7269 616c  eight - material
+00004ed0: 2e64 6570 7468 5f74 6f5f 626f 7474 6f6d  .depth_to_bottom
+00004ee0: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00004ef0: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+00004f00: 2020 2075 7469 6c69 7469 6573 2e69 735f     utilities.is_
+00004f10: 636f 6c6f 7228 6d61 7465 7269 616c 2e75  color(material.u
+00004f20: 7365 725f 6465 6669 6e65 645f 636f 6c6f  ser_defined_colo
+00004f30: 7229 0a20 2020 2020 2020 2020 2020 2020  r).             
+00004f40: 2020 2061 6e64 206d 6174 6572 6961 6c2e     and material.
+00004f50: 7573 6572 5f64 6566 696e 6564 5f63 6f6c  user_defined_col
+00004f60: 6f72 2021 3d20 2222 0a20 2020 2020 2020  or != "".       
+00004f70: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
+00004f80: 2020 2020 2020 2020 6d61 7465 7269 616c          material
+00004f90: 2e63 6f6c 6f72 203d 206d 6174 6572 6961  .color = materia
+00004fa0: 6c2e 7573 6572 5f64 6566 696e 6564 5f63  l.user_defined_c
+00004fb0: 6f6c 6f72 0a20 2020 2020 2020 2020 2020  olor.           
+00004fc0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00004fd0: 2020 2020 2020 206d 6174 6572 6961 6c2e         material.
+00004fe0: 636f 6c6f 7220 3d20 4d41 5445 5249 414c  color = MATERIAL
+00004ff0: 5f43 4f4c 4f52 535b 6920 2520 3130 5d0a  _COLORS[i % 10].
+00005000: 0a20 2020 2020 2020 2020 2020 206d 6174  .            mat
+00005010: 6572 6961 6c5f 7265 6669 6e65 642e 6170  erial_refined.ap
+00005020: 7065 6e64 286d 6174 6572 6961 6c29 0a0a  pend(material)..
+00005030: 2020 2020 2020 2020 7365 6c66 2e5f 6d61          self._ma
+00005040: 7465 7269 616c 7320 3d20 6d61 7465 7269  terials = materi
+00005050: 616c 5f72 6566 696e 6564 0a0a 2020 2020  al_refined..    
+00005060: 2020 2020 2320 7265 7365 7420 7265 7375      # reset resu
+00005070: 6c74 730a 2020 2020 2020 2020 7365 6c66  lts.        self
+00005080: 2e5f 7265 7365 745f 7265 7375 6c74 7328  ._reset_results(
+00005090: 290a 0a20 2020 2064 6566 2072 656d 6f76  )..    def remov
+000050a0: 655f 6d61 7465 7269 616c 280a 2020 2020  e_material(.    
+000050b0: 2020 2020 7365 6c66 2c20 6d61 7465 7269      self, materi
+000050c0: 616c 3a20 4d61 7465 7269 616c 203d 204e  al: Material = N
+000050d0: 6f6e 652c 2064 6570 7468 3a20 666c 6f61  one, depth: floa
+000050e0: 7420 3d20 4e6f 6e65 2c20 7265 6d6f 7665  t = None, remove
+000050f0: 5f61 6c6c 3d46 616c 7365 0a20 2020 2029  _all=False.    )
+00005100: 3a0a 2020 2020 2020 2020 2222 2252 656d  :.        """Rem
+00005110: 6f76 6520 6d61 7465 7269 616c 2066 726f  ove material fro
+00005120: 6d20 736c 6f70 652e 0a0a 2020 2020 2020  m slope...      
+00005130: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+00005140: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
+00005150: 2020 2020 2020 2020 6d61 7465 7269 616c          material
+00005160: 203a 204d 6174 6572 6961 6c2c 206f 7074   : Material, opt
+00005170: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
+00005180: 2020 6d61 7465 7269 616c 206f 626a 6563    material objec
+00005190: 742e 2049 6620 7370 6563 6966 6965 6420  t. If specified 
+000051a0: 616e 6420 6578 6973 7473 2069 6e20 6d61  and exists in ma
+000051b0: 7465 7269 616c 730a 2020 2020 2020 2020  terials.        
+000051c0: 2020 2020 6173 736f 6369 6174 6564 2077      associated w
+000051d0: 6974 6820 736c 6f70 6520 7468 656e 2077  ith slope then w
+000051e0: 696c 6c20 6265 2072 656d 6f76 6564 2c20  ill be removed, 
+000051f0: 6279 2064 6566 6175 6c74 204e 6f6e 650a  by default None.
+00005200: 2020 2020 2020 2020 6465 7074 6820 3a20          depth : 
+00005210: 666c 6f61 742c 206f 7074 696f 6e61 6c0a  float, optional.
+00005220: 2020 2020 2020 2020 2020 2020 6465 7074              dept
+00005230: 6820 696e 206d 6574 7265 7320 6f66 206d  h in metres of m
+00005240: 6174 6572 6961 6c20 6f62 6a65 6374 2e20  aterial object. 
+00005250: 4966 206e 6f74 204e 6f6e 6520 616e 6420  If not None and 
+00005260: 6d61 7465 7269 616c 2066 6f75 6e64 0a20  material found. 
+00005270: 2020 2020 2020 2020 2020 2061 7420 696e             at in
+00005280: 6469 6361 7465 6420 6465 7074 6820 7468  dicated depth th
+00005290: 656e 2077 696c 6c20 7265 6d6f 7665 2074  en will remove t
+000052a0: 6865 206d 6174 6572 6961 6c2c 2062 7920  he material, by 
+000052b0: 6465 6661 756c 7420 4e6f 6e65 0a20 2020  default None.   
+000052c0: 2020 2020 2072 656d 6f76 655f 616c 6c20       remove_all 
+000052d0: 3a20 426f 6f6c 6561 6e2c 206f 7074 696f  : Boolean, optio
+000052e0: 6e61 6c0a 2020 2020 2020 2020 2020 2020  nal.            
+000052f0: 6966 2074 7275 6520 616c 6c20 6d61 7465  if true all mate
+00005300: 7269 616c 7320 7265 6d6f 7665 642c 2064  rials removed, d
+00005310: 6566 6175 6c74 2066 616c 7365 0a0a 0a20  efault false... 
+00005320: 2020 2020 2020 2045 7861 6d70 6c65 730a         Examples.
+00005330: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+00005340: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+00005350: 2020 3e3e 3e20 7320 3d20 536c 6f70 6528    >>> s = Slope(
+00005360: 290a 2020 2020 2020 2020 3e3e 3e20 6d31  ).        >>> m1
+00005370: 203d 204d 6174 6572 6961 6c28 290a 2020   = Material().  
+00005380: 2020 2020 2020 3e3e 3e20 6d32 203d 204d        >>> m2 = M
+00005390: 6174 6572 6961 6c28 756e 6974 5f77 6569  aterial(unit_wei
+000053a0: 6768 7420 3d20 3138 2c63 6f68 6573 696f  ght = 18,cohesio
+000053b0: 6e3d 322c 6672 6963 7469 6f6e 5f61 6e67  n=2,friction_ang
+000053c0: 6c65 203d 2033 302c 6465 7074 685f 746f  le = 30,depth_to
+000053d0: 5f62 6f74 746f 6d20 3d20 312e 3332 290a  _bottom = 1.32).
+000053e0: 2020 2020 2020 2020 3e3e 3e20 732e 7365          >>> s.se
+000053f0: 745f 6d61 7465 7269 616c 7328 6d31 2c20  t_materials(m1, 
+00005400: 6d32 290a 2020 2020 2020 2020 3e3e 3e20  m2).        >>> 
+00005410: 6c65 6e28 732e 5f6d 6174 6572 6961 6c73  len(s._materials
+00005420: 2920 3d3d 2032 0a20 2020 2020 2020 2054  ) == 2.        T
+00005430: 7275 650a 2020 2020 2020 2020 3e3e 3e20  rue.        >>> 
+00005440: 732e 7265 6d6f 7665 5f6d 6174 6572 6961  s.remove_materia
+00005450: 6c28 6d31 290a 2020 2020 2020 2020 3e3e  l(m1).        >>
+00005460: 3e20 6c65 6e28 732e 5f6d 6174 6572 6961  > len(s._materia
+00005470: 6c73 2920 3d3d 2031 0a20 2020 2020 2020  ls) == 1.       
+00005480: 2054 7275 650a 2020 2020 2020 2020 3e3e   True.        >>
+00005490: 3e20 732e 7265 6d6f 7665 5f6d 6174 6572  > s.remove_mater
+000054a0: 6961 6c28 7265 6d6f 7665 5f61 6c6c 3d54  ial(remove_all=T
+000054b0: 7275 6529 0a20 2020 2020 2020 203e 3e3e  rue).        >>>
+000054c0: 206c 656e 2873 2e5f 6d61 7465 7269 616c   len(s._material
+000054d0: 7329 203d 3d20 300a 2020 2020 2020 2020  s) == 0.        
+000054e0: 5472 7565 0a0a 2020 2020 2020 2020 2222  True..        ""
+000054f0: 220a 2020 2020 2020 2020 2320 6765 6e65  ".        # gene
+00005500: 7261 6c20 6e6f 7465 3a20 6465 7074 6820  ral note: depth 
+00005510: 7573 6564 2074 6f20 7265 6d6f 7665 206f  used to remove o
+00005520: 626a 6563 7420 7261 7468 6572 2074 6861  bject rather tha
+00005530: 6e20 6469 7265 6374 6c79 2072 656d 6f76  n directly remov
+00005540: 696e 670a 2020 2020 2020 2020 2320 6576  ing.        # ev
+00005550: 656e 2077 6865 6e20 6d61 7465 7269 616c  en when material
+00005560: 2063 6c61 7373 2070 726f 7669 6465 6420   class provided 
+00005570: 6265 6361 7573 6520 6120 7573 6572 206d  because a user m
+00005580: 6967 6874 2072 6569 6e69 7469 616c 6973  ight reinitialis
+00005590: 650a 2020 2020 2020 2020 2320 616e 206f  e.        # an o
+000055a0: 626a 6563 7420 7769 7468 2074 6865 2073  bject with the s
+000055b0: 616d 6520 6465 7461 696c 7320 6275 7420  ame details but 
+000055c0: 6966 2074 6865 2070 6f69 6e74 6572 2069  if the pointer i
+000055d0: 7320 6368 616e 6765 6420 7468 616e 0a20  s changed than. 
+000055e0: 2020 2020 2020 2023 2069 7420 6d69 6768         # it migh
+000055f0: 7420 6265 2063 6f6e 6675 7369 6e67 2066  t be confusing f
+00005600: 6f72 2074 6865 2075 7365 7220 6173 2074  or the user as t
+00005610: 6f20 7768 7920 7468 6579 2063 616e 7420  o why they cant 
+00005620: 7265 6d6f 7665 2e0a 2020 2020 2020 2020  remove..        
+00005630: 2320 436f 6d6d 656e 7420 6279 204a 6573  # Comment by Jes
+00005640: 7365 2042 2c20 3134 2e30 332e 3230 3232  se B, 14.03.2022
+00005650: 2e0a 0a20 2020 2020 2020 2023 2069 6620  ...        # if 
+00005660: 6d61 7465 7269 616c 2064 6566 696e 6564  material defined
+00005670: 2061 6e64 206d 6174 6572 6961 6c20 7479   and material ty
+00005680: 7065 2069 7320 4d61 7465 7269 616c 2073  pe is Material s
+00005690: 6574 2064 6570 7468 2074 6f20 6265 2064  et depth to be d
+000056a0: 6570 7468 206f 6620 6d61 7465 7269 616c  epth of material
+000056b0: 0a20 2020 2020 2020 2069 6620 6d61 7465  .        if mate
+000056c0: 7269 616c 2061 6e64 2069 7369 6e73 7461  rial and isinsta
+000056d0: 6e63 6528 6d61 7465 7269 616c 2c20 4d61  nce(material, Ma
+000056e0: 7465 7269 616c 293a 0a20 2020 2020 2020  terial):.       
+000056f0: 2020 2020 2064 6570 7468 203d 206d 6174       depth = mat
+00005700: 6572 6961 6c2e 6465 7074 685f 746f 5f62  erial.depth_to_b
+00005710: 6f74 746f 6d0a 0a20 2020 2020 2020 2023  ottom..        #
+00005720: 2069 6620 6465 7074 6820 7370 6563 6966   if depth specif
+00005730: 6965 6420 6164 6f70 740a 2020 2020 2020  ied adopt.      
+00005740: 2020 6966 2064 6570 7468 3a0a 2020 2020    if depth:.    
+00005750: 2020 2020 2020 2020 666f 7220 6d20 696e          for m in
+00005760: 2073 656c 662e 5f6d 6174 6572 6961 6c73   self._materials
+00005770: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00005780: 2020 6966 206d 2e64 6570 7468 5f74 6f5f    if m.depth_to_
+00005790: 626f 7474 6f6d 203d 3d20 6465 7074 683a  bottom == depth:
+000057a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000057b0: 2020 2020 2073 656c 662e 5f6d 6174 6572       self._mater
+000057c0: 6961 6c73 2e72 656d 6f76 6528 6d29 0a20  ials.remove(m). 
+000057d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000057e0: 2020 2062 7265 616b 0a0a 2020 2020 2020     break..      
+000057f0: 2020 6966 2072 656d 6f76 655f 616c 6c3a    if remove_all:
+00005800: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00005810: 662e 5f6d 6174 6572 6961 6c73 203d 205b  f._materials = [
+00005820: 5d0a 0a20 2020 2020 2020 2023 2072 6573  ]..        # res
+00005830: 6574 2072 6573 756c 7473 0a20 2020 2020  et results.     
+00005840: 2020 2073 656c 662e 5f72 6573 6574 5f72     self._reset_r
+00005850: 6573 756c 7473 2829 0a0a 2020 2020 6465  esults()..    de
+00005860: 6620 7570 6461 7465 5f77 6174 6572 5f61  f update_water_a
+00005870: 6e61 6c79 7369 735f 6f70 7469 6f6e 7328  nalysis_options(
+00005880: 7365 6c66 2c20 6175 746f 3a20 626f 6f6c  self, auto: bool
+00005890: 203d 2054 7275 652c 2048 3a20 696e 7420   = True, H: int 
+000058a0: 3d20 3129 3a0a 2020 2020 2020 2020 2222  = 1):.        ""
+000058b0: 2255 7064 6174 6520 616e 616c 7973 6973  "Update analysis
+000058c0: 206f 7074 696f 6e73 2072 6567 6172 6469   options regardi
+000058d0: 6e67 2068 6f77 2077 6174 6572 2069 7320  ng how water is 
+000058e0: 7472 6561 7465 642e 0a0a 2020 2020 2020  treated...      
+000058f0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+00005900: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
+00005910: 2020 2020 2020 2020 6175 746f 203a 2062          auto : b
+00005920: 6f6f 6c2c 206f 7074 696f 6e61 6c0a 2020  ool, optional.  
+00005930: 2020 2020 2020 2020 2020 4966 2074 7275            If tru
+00005940: 6520 6361 6c63 756c 6174 6573 2070 7265  e calculates pre
+00005950: 7373 7572 6520 6865 6164 2061 7574 6f6d  ssure head autom
+00005960: 6174 6963 616c 6c79 2028 6661 6374 6f72  atically (factor
+00005970: 2069 7320 636f 7328 6129 2a2a 3220 7768   is cos(a)**2 wh
+00005980: 6572 6520 6120 6973 0a20 2020 2020 2020  ere a is.       
+00005990: 2020 2020 2074 6865 2061 6e67 6c65 206f       the angle o
+000059a0: 6620 736c 6f70 6529 2e20 4966 2046 616c  f slope). If Fal
+000059b0: 7365 2074 616b 6573 206d 616e 7561 6c20  se takes manual 
+000059c0: 6661 6374 6f72 2028 4829 2e20 6279 2064  factor (H). by d
+000059d0: 6566 6175 6c74 2054 7275 650a 2020 2020  efault True.    
+000059e0: 2020 2020 4820 3a20 696e 742c 206f 7074      H : int, opt
+000059f0: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
+00005a00: 2020 6661 6374 6f72 206f 6e20 7761 7465    factor on wate
+00005a10: 7220 7072 6573 7375 7265 2e20 4966 2031  r pressure. If 1
+00005a20: 2077 6174 6572 2068 6561 6420 6571 7561   water head equa
+00005a30: 6c73 2064 6973 7461 6e63 6520 6265 7477  ls distance betw
+00005a40: 6565 6e20 7761 7465 720a 2020 2020 2020  een water.      
+00005a50: 2020 2020 2020 7461 626c 6520 616e 6420        table and 
+00005a60: 626f 7474 6f6d 206f 6620 736c 6963 652e  bottom of slice.
+00005a70: 2049 6620 3020 6e6f 2077 6174 6572 2070   If 0 no water p
+00005a80: 7265 7373 7572 6520 6973 2063 6f6e 7369  ressure is consi
+00005a90: 6465 7265 642e 2042 7920 6465 6661 756c  dered. By defaul
+00005aa0: 7420 312e 0a0a 0a20 2020 2020 2020 2045  t 1....        E
+00005ab0: 7861 6d70 6c65 730a 2020 2020 2020 2020  xamples.        
+00005ac0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005ad0: 2d0a 2020 2020 2020 2020 3e3e 3e20 7320  -.        >>> s 
+00005ae0: 3d20 536c 6f70 6528 290a 2020 2020 2020  = Slope().      
+00005af0: 2020 3e3e 3e20 732e 7570 6461 7465 5f77    >>> s.update_w
+00005b00: 6174 6572 5f61 6e61 6c79 7369 735f 6f70  ater_analysis_op
+00005b10: 7469 6f6e 7328 6175 746f 3d54 7275 6529  tions(auto=True)
+00005b20: 0a20 2020 2020 2020 203e 3e3e 2073 2e75  .        >>> s.u
+00005b30: 7064 6174 655f 7761 7465 725f 616e 616c  pdate_water_anal
+00005b40: 7973 6973 5f6f 7074 696f 6e73 2861 7574  ysis_options(aut
+00005b50: 6f3d 4661 6c73 652c 2048 203d 2030 2e37  o=False, H = 0.7
+00005b60: 3229 0a20 2020 2020 2020 2022 2222 0a0a  2).        """..
+00005b70: 2020 2020 2020 2020 6966 2061 7574 6f3a          if auto:
+00005b80: 0a20 2020 2020 2020 2020 2020 2061 203d  .            a =
+00005b90: 2061 7461 6e28 7365 6c66 2e5f 6772 6164   atan(self._grad
+00005ba0: 6965 6e74 290a 2020 2020 2020 2020 2020  ient).          
+00005bb0: 2020 4820 3d20 636f 7328 6129 202a 2a20    H = cos(a) ** 
+00005bc0: 320a 0a20 2020 2020 2020 2065 6c73 653a  2..        else:
+00005bd0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+00005be0: 615f 7661 6c69 6461 7469 6f6e 2e61 7373  a_validation.ass
+00005bf0: 6572 745f 6e75 6d62 6572 2848 2c20 2248  ert_number(H, "H
+00005c00: 2229 0a20 2020 2020 2020 2020 2020 2069  ").            i
+00005c10: 6620 4820 3e20 313a 0a20 2020 2020 2020  f H > 1:.       
+00005c20: 2020 2020 2020 2020 2048 203d 2031 0a20           H = 1. 
+00005c30: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00005c40: 4820 3c20 303a 0a20 2020 2020 2020 2020  H < 0:.         
+00005c50: 2020 2020 2020 2048 203d 2030 0a0a 2020         H = 0..  
+00005c60: 2020 2020 2020 7365 6c66 2e5f 7761 7465        self._wate
+00005c70: 725f 616e 616c 7973 6973 5f48 203d 2048  r_analysis_H = H
+00005c80: 0a0a 2020 2020 2020 2020 2320 7265 7365  ..        # rese
+00005c90: 7420 7265 7375 6c74 730a 2020 2020 2020  t results.      
+00005ca0: 2020 7365 6c66 2e5f 7265 7365 745f 7265    self._reset_re
+00005cb0: 7375 6c74 7328 290a 0a20 2020 2064 6566  sults()..    def
+00005cc0: 2075 7064 6174 655f 616e 616c 7973 6973   update_analysis
+00005cd0: 5f6f 7074 696f 6e73 280a 2020 2020 2020  _options(.      
+00005ce0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+00005cf0: 736c 6963 6573 3a20 696e 7420 3d20 4e6f  slices: int = No
+00005d00: 6e65 2c0a 2020 2020 2020 2020 6974 6572  ne,.        iter
+00005d10: 6174 696f 6e73 3a20 696e 7420 3d20 4e6f  ations: int = No
+00005d20: 6e65 2c0a 2020 2020 2020 2020 6d69 6e5f  ne,.        min_
+00005d30: 6661 696c 7572 655f 6469 7374 3a20 696e  failure_dist: in
+00005d40: 7420 3d20 4e6f 6e65 2c0a 2020 2020 2020  t = None,.      
+00005d50: 2020 746f 6c65 7261 6e63 653a 2066 6c6f    tolerance: flo
+00005d60: 6174 203d 204e 6f6e 652c 0a20 2020 2020  at = None,.     
+00005d70: 2020 206d 6178 5f69 7465 7261 7469 6f6e     max_iteration
+00005d80: 733a 2069 6e74 203d 204e 6f6e 652c 0a20  s: int = None,. 
+00005d90: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
+00005da0: 2246 756e 6374 696f 6e20 746f 2075 7064  "Function to upd
+00005db0: 6174 6520 616e 616c 7973 6973 206d 6f64  ate analysis mod
+00005dc0: 656c 6c69 6e67 206f 7074 696f 6e73 2e0a  elling options..
+00005dd0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00005de0: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+00005df0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2073  ------.        s
+00005e00: 6c69 6365 7320 3a20 696e 742c 206f 7074  lices : int, opt
+00005e10: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
+00005e20: 2020 536c 6963 6573 2074 6f20 7461 6b65    Slices to take
+00005e30: 2069 6e20 6361 6c63 756c 6174 696f 6e20   in calculation 
+00005e40: 666f 7220 6561 6368 2070 6f74 656e 7469  for each potenti
+00005e50: 616c 0a20 2020 2020 2020 2020 2020 2063  al.            c
+00005e60: 6972 6375 6c61 7220 6661 696c 7572 6520  ircular failure 
+00005e70: 2862 6574 7765 656e 2031 3020 616e 6420  (between 10 and 
+00005e80: 3530 3029 2e20 4966 204e 6f6e 6520 646f  500). If None do
+00005e90: 6573 6e74 2075 7064 6174 6520 7468 6520  esnt update the 
+00005ea0: 7061 7261 6d65 7465 722c 2062 7920 6465  parameter, by de
+00005eb0: 6661 756c 7420 4e6f 6e65 2e0a 2020 2020  fault None..    
+00005ec0: 2020 2020 6974 6572 6174 696f 6e73 203a      iterations :
+00005ed0: 2069 6e74 2c20 6f70 7469 6f6e 616c 0a20   int, optional. 
+00005ee0: 2020 2020 2020 2020 2020 2041 7070 726f             Appro
+00005ef0: 7869 6d61 7465 206e 756d 6265 7220 6f66  ximate number of
+00005f00: 2070 6f74 656e 7469 616c 2073 6c6f 7065   potential slope
+00005f10: 7320 746f 2063 6865 636b 2028 6265 7477  s to check (betw
+00005f20: 6565 6e20 3530 3020 616e 6420 3130 3030  een 500 and 1000
+00005f30: 3030 292e 0a20 2020 2020 2020 2020 2020  00)..           
+00005f40: 2049 6620 4e6f 6e65 2064 6f65 736e 7420   If None doesnt 
+00005f50: 7570 6461 7465 2074 6865 2070 6172 616d  update the param
+00005f60: 6574 6572 2c20 6279 2064 6566 6175 6c74  eter, by default
+00005f70: 204e 6f6e 652e 0a20 2020 2020 2020 206d   None..        m
+00005f80: 696e 5f66 6169 6c75 7265 5f64 6973 7420  in_failure_dist 
+00005f90: 3a20 696e 742c 206f 7074 696f 6e61 6c0a  : int, optional.
+00005fa0: 2020 2020 2020 2020 2020 2020 4966 2073              If s
+00005fb0: 7065 6369 6669 6564 206f 6e6c 7920 6661  pecified only fa
+00005fc0: 696c 7572 6520 736c 6f70 6573 2077 6974  ilure slopes wit
+00005fd0: 6820 6120 6469 7374 616e 6365 2067 7265  h a distance gre
+00005fe0: 6174 6572 2074 6861 6e20 7468 650a 2020  ater than the.  
+00005ff0: 2020 2020 2020 2020 2020 6d69 6e20 6661            min fa
+00006000: 696c 7572 6520 6469 7374 616e 6365 2077  ilure distance w
+00006010: 696c 6c20 6265 2061 7373 6573 7365 642c  ill be assessed,
+00006020: 2062 7920 6465 6661 756c 7420 4e6f 6e65   by default None
+00006030: 2e0a 2020 2020 2020 2020 746f 6c65 7261  ..        tolera
+00006040: 6e63 6520 3a20 666c 6f61 742c 206f 7074  nce : float, opt
+00006050: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
+00006060: 2020 436f 6e76 6572 6761 6e63 6520 746f    Convergance to
+00006070: 6c65 7261 6e63 6520 6f6e 2062 6973 686f  lerance on bisho
+00006080: 7073 2e20 4361 6c63 756c 6174 696f 6e20  ps. Calculation 
+00006090: 7769 6c6c 2073 746f 7020 7768 656e 2063  will stop when c
+000060a0: 6861 6e67 6520 696e 2066 6163 746f 720a  hange in factor.
+000060b0: 2020 2020 2020 2020 2020 2020 6f66 2073              of s
+000060c0: 6166 6574 7920 6973 206c 6573 7320 7468  afety is less th
+000060d0: 616e 2074 6865 2074 6f6c 6572 616e 6365  an the tolerance
+000060e0: 2073 7065 6369 6669 6564 2e20 4279 2064   specified. By d
+000060f0: 6566 6175 6c74 204e 6f6e 652e 2049 6e69  efault None. Ini
+00006100: 616c 6973 6564 2061 7320 302e 3030 352e  alised as 0.005.
+00006110: 0a20 2020 2020 2020 206d 6178 5f69 7465  .        max_ite
+00006120: 7261 7469 6f6e 7320 3a20 696e 742c 206f  rations : int, o
+00006130: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+00006140: 2020 2020 4d61 7869 6d75 6d20 6e75 6d62      Maximum numb
+00006150: 6572 206f 6620 6974 6572 6174 696f 6e73  er of iterations
+00006160: 2066 6f72 2063 6f6e 7665 7267 656e 6365   for convergence
+00006170: 206f 6e20 6269 7368 6f70 2066 6163 746f   on bishop facto
+00006180: 7220 6f66 2073 6166 6574 792e 2042 7920  r of safety. By 
+00006190: 6465 6661 756c 740a 2020 2020 2020 2020  default.        
+000061a0: 2020 2020 4e6f 6e65 2e20 496e 6974 6961      None. Initia
+000061b0: 6c69 7365 6420 6173 2031 352e 0a0a 2020  lised as 15...  
+000061c0: 2020 2020 2020 4578 616d 706c 6573 0a20        Examples. 
+000061d0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+000061e0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+000061f0: 203e 3e3e 2073 203d 2053 6c6f 7065 2829   >>> s = Slope()
+00006200: 0a20 2020 2020 2020 203e 3e3e 2073 2e75  .        >>> s.u
+00006210: 7064 6174 655f 616e 616c 7973 6973 5f6f  pdate_analysis_o
+00006220: 7074 696f 6e73 2873 6c69 6365 7320 3d20  ptions(slices = 
+00006230: 3235 2c69 7465 7261 7469 6f6e 7320 3d20  25,iterations = 
+00006240: 3235 3030 2c6d 696e 5f66 6169 6c75 7265  2500,min_failure
+00006250: 5f64 6973 7420 3d20 302e 3229 0a20 2020  _dist = 0.2).   
+00006260: 2020 2020 203e 3e3e 2073 2e75 7064 6174       >>> s.updat
+00006270: 655f 616e 616c 7973 6973 5f6f 7074 696f  e_analysis_optio
+00006280: 6e73 2874 6f6c 6572 616e 6365 203d 2030  ns(tolerance = 0
+00006290: 2e30 3035 2c6d 6178 5f69 7465 7261 7469  .005,max_iterati
+000062a0: 6f6e 7320 3d20 3530 290a 2020 2020 2020  ons = 50).      
+000062b0: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
+000062c0: 2073 6c69 6365 733a 0a20 2020 2020 2020   slices:.       
+000062d0: 2020 2020 2073 656c 662e 5f73 6c69 6365       self._slice
+000062e0: 7320 3d20 6d61 7828 6d69 6e28 3530 302c  s = max(min(500,
+000062f0: 2073 6c69 6365 7329 2c20 3130 290a 0a20   slices), 10).. 
+00006300: 2020 2020 2020 2069 6620 6974 6572 6174         if iterat
+00006310: 696f 6e73 3a0a 2020 2020 2020 2020 2020  ions:.          
+00006320: 2020 7365 6c66 2e5f 6974 6572 6174 696f    self._iteratio
+00006330: 6e73 203d 206d 6178 286d 696e 2869 7465  ns = max(min(ite
+00006340: 7261 7469 6f6e 732c 2031 3030 3030 3029  rations, 100000)
+00006350: 2c20 3530 3029 0a0a 2020 2020 2020 2020  , 500)..        
+00006360: 6966 206d 696e 5f66 6169 6c75 7265 5f64  if min_failure_d
+00006370: 6973 7420 6973 206e 6f74 204e 6f6e 653a  ist is not None:
+00006380: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00006390: 662e 5f6d 696e 5f66 6169 6c75 7265 5f64  f._min_failure_d
+000063a0: 6973 7461 6e63 6520 3d20 6d69 6e28 0a20  istance = min(. 
+000063b0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+000063c0: 696e 5f66 6169 6c75 7265 5f64 6973 742c  in_failure_dist,
+000063d0: 2073 656c 662e 5f65 7874 6572 6e61 6c5f   self._external_
+000063e0: 6c65 6e67 7468 202a 2030 2e39 0a20 2020  length * 0.9.   
+000063f0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+00006400: 2020 2020 6966 2074 6f6c 6572 616e 6365      if tolerance
+00006410: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00006420: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00006430: 746f 6c65 7261 6e63 6520 3d20 746f 6c65  tolerance = tole
+00006440: 7261 6e63 650a 0a20 2020 2020 2020 2069  rance..        i
+00006450: 6620 6d61 785f 6974 6572 6174 696f 6e73  f max_iterations
+00006460: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00006470: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00006480: 6d61 785f 6974 6572 6174 696f 6e73 203d  max_iterations =
+00006490: 206d 6178 5f69 7465 7261 7469 6f6e 730a   max_iterations.
+000064a0: 0a20 2020 2020 2020 2023 2072 6573 6574  .        # reset
+000064b0: 2072 6573 756c 7473 0a20 2020 2020 2020   results.       
+000064c0: 2073 656c 662e 5f72 6573 6574 5f72 6573   self._reset_res
+000064d0: 756c 7473 2829 0a0a 2020 2020 6465 6620  ults()..    def 
+000064e0: 7570 6461 7465 5f62 6f75 6e64 6172 795f  update_boundary_
+000064f0: 6f70 7469 6f6e 7328 0a20 2020 2020 2020  options(.       
+00006500: 2073 656c 662c 0a20 2020 2020 2020 204d   self,.        M
+00006510: 494e 5f45 5854 5f4c 3a20 666c 6f61 7420  IN_EXT_L: float 
+00006520: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00006530: 4d49 4e5f 4558 545f 483a 2066 6c6f 6174  MIN_EXT_H: float
+00006540: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
+00006550: 2020 2020 2020 2020 2222 2246 756e 6374          """Funct
+00006560: 696f 6e20 746f 2075 7064 6174 6520 6578  ion to update ex
+00006570: 7465 726e 616c 2062 6f75 6e64 6172 7920  ternal boundary 
+00006580: 6f70 7469 6f6e 732e 0a0a 2020 2020 2020  options...      
+00006590: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+000065a0: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
+000065b0: 2020 2020 2020 2020 4d49 4e5f 4558 545f          MIN_EXT_
+000065c0: 4c20 3a20 666c 6f61 742c 206f 7074 696f  L : float, optio
+000065d0: 6e61 6c0a 2020 2020 2020 2020 2020 2020  nal.            
+000065e0: 4d69 6e69 6d75 6d20 6578 7465 726e 616c  Minimum external
+000065f0: 2062 6f75 6e64 6172 7920 6c65 6e67 7468   boundary length
+00006600: 2e20 4966 204e 6f6e 6520 646f 6573 6e74  . If None doesnt
+00006610: 2075 7064 6174 650a 2020 2020 2020 2020   update.        
+00006620: 2020 2020 7468 6520 7061 7261 6d65 7465      the paramete
+00006630: 722c 2062 7920 6465 6661 756c 7420 4e6f  r, by default No
+00006640: 6e65 0a20 2020 2020 2020 204d 494e 5f45  ne.        MIN_E
+00006650: 5854 5f48 203a 2066 6c6f 6174 2c20 6f70  XT_H : float, op
+00006660: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
+00006670: 2020 204d 696e 696d 756d 2065 7874 6572     Minimum exter
+00006680: 6e61 6c20 626f 756e 6461 7279 2068 6569  nal boundary hei
+00006690: 6768 742e 2049 6620 4e6f 6e65 2064 6f65  ght. If None doe
+000066a0: 736e 7420 7570 6461 7465 0a20 2020 2020  snt update.     
+000066b0: 2020 2020 2020 2074 6865 2070 6172 616d         the param
+000066c0: 6574 6572 2c20 6279 2064 6566 6175 6c74  eter, by default
+000066d0: 204e 6f6e 652e 0a0a 2020 2020 2020 2020   None...        
+000066e0: 4578 616d 706c 6573 0a20 2020 2020 2020  Examples.       
+000066f0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+00006700: 2d2d 0a20 2020 2020 2020 203e 3e3e 2073  --.        >>> s
+00006710: 203d 2053 6c6f 7065 2829 0a20 2020 2020   = Slope().     
+00006720: 2020 203e 3e3e 2073 2e75 7064 6174 655f     >>> s.update_
+00006730: 626f 756e 6461 7279 5f6f 7074 696f 6e73  boundary_options
+00006740: 284d 494e 5f45 5854 5f4c 203d 2031 3030  (MIN_EXT_L = 100
+00006750: 290a 2020 2020 2020 2020 3e3e 3e20 732e  ).        >>> s.
+00006760: 5f65 7874 6572 6e61 6c5f 6c65 6e67 7468  _external_length
+00006770: 203d 3d20 3130 300a 2020 2020 2020 2020   == 100.        
+00006780: 5472 7565 0a20 2020 2020 2020 203e 3e3e  True.        >>>
+00006790: 2073 2e75 7064 6174 655f 626f 756e 6461   s.update_bounda
+000067a0: 7279 5f6f 7074 696f 6e73 284d 494e 5f45  ry_options(MIN_E
+000067b0: 5854 5f48 203d 2032 3030 290a 2020 2020  XT_H = 200).    
+000067c0: 2020 2020 3e3e 3e20 732e 5f65 7874 6572      >>> s._exter
+000067d0: 6e61 6c5f 6865 6967 6874 203d 3d20 3230  nal_height == 20
+000067e0: 300a 2020 2020 2020 2020 5472 7565 0a20  0.        True. 
+000067f0: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
+00006800: 2020 2020 6966 204d 494e 5f45 5854 5f48      if MIN_EXT_H
+00006810: 3a0a 2020 2020 2020 2020 2020 2020 6461  :.            da
+00006820: 7461 5f76 616c 6964 6174 696f 6e2e 6173  ta_validation.as
+00006830: 7365 7274 5f73 7472 6963 746c 795f 706f  sert_strictly_po
+00006840: 7369 7469 7665 5f6e 756d 6265 7228 0a20  sitive_number(. 
+00006850: 2020 2020 2020 2020 2020 2020 2020 204d                 M
+00006860: 494e 5f45 5854 5f48 2c20 224d 696e 696d  IN_EXT_H, "Minim
+00006870: 756d 2065 7874 6572 6e61 6c20 6d6f 6465  um external mode
+00006880: 6c20 6865 6967 6874 2028 4d49 4e5f 4558  l height (MIN_EX
+00006890: 545f 4829 220a 2020 2020 2020 2020 2020  T_H)".          
+000068a0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+000068b0: 7365 6c66 2e5f 4d49 4e5f 4558 545f 4820  self._MIN_EXT_H 
+000068c0: 3d20 4d49 4e5f 4558 545f 480a 2020 2020  = MIN_EXT_H.    
+000068d0: 2020 2020 6966 204d 494e 5f45 5854 5f4c      if MIN_EXT_L
+000068e0: 3a0a 2020 2020 2020 2020 2020 2020 6461  :.            da
+000068f0: 7461 5f76 616c 6964 6174 696f 6e2e 6173  ta_validation.as
+00006900: 7365 7274 5f73 7472 6963 746c 795f 706f  sert_strictly_po
+00006910: 7369 7469 7665 5f6e 756d 6265 7228 0a20  sitive_number(. 
+00006920: 2020 2020 2020 2020 2020 2020 2020 204d                 M
+00006930: 494e 5f45 5854 5f4c 2c20 224d 696e 696d  IN_EXT_L, "Minim
+00006940: 756d 2065 7874 6572 6e61 6c20 6d6f 6465  um external mode
+00006950: 6c20 6c65 6e67 7468 2028 4d49 4e5f 4558  l length (MIN_EX
+00006960: 545f 4829 220a 2020 2020 2020 2020 2020  T_H)".          
+00006970: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00006980: 7365 6c66 2e5f 4d49 4e5f 4558 545f 4c20  self._MIN_EXT_L 
+00006990: 3d20 4d49 4e5f 4558 545f 4c0a 0a20 2020  = MIN_EXT_L..   
+000069a0: 2020 2020 2023 2069 6620 7468 6520 6578       # if the ex
+000069b0: 7465 726e 616c 2062 6f75 6e64 6172 7920  ternal boundary 
+000069c0: 6861 7320 6265 656e 2073 6574 2074 6869  has been set thi
+000069d0: 7320 6361 6c6c 2069 7320 6166 7465 7220  s call is after 
+000069e0: 696e 6974 2e20 4361 6e20 7570 6461 7465  init. Can update
+000069f0: 2074 6865 2062 6f75 6e64 6172 792e 0a20   the boundary.. 
+00006a00: 2020 2020 2020 2023 206f 7468 6572 7769         # otherwi
+00006a10: 7365 2077 696c 6c20 6765 7420 616e 2065  se will get an e
+00006a20: 7272 6f72 0a20 2020 2020 2020 2069 6620  rror.        if 
+00006a30: 7365 6c66 2e5f 6578 7465 726e 616c 5f62  self._external_b
+00006a40: 6f75 6e64 6172 7920 6973 206e 6f74 204e  oundary is not N
+00006a50: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00006a60: 2073 656c 662e 7365 745f 6578 7465 726e   self.set_extern
+00006a70: 616c 5f62 6f75 6e64 6172 7928 6865 6967  al_boundary(heig
+00006a80: 6874 3d73 656c 662e 5f68 6569 6768 742c  ht=self._height,
+00006a90: 206c 656e 6774 683d 7365 6c66 2e5f 6c65   length=self._le
+00006aa0: 6e67 7468 290a 0a20 2020 2020 2020 2023  ngth)..        #
+00006ab0: 2072 6573 6574 2072 6573 756c 7473 0a20   reset results. 
+00006ac0: 2020 2020 2020 2073 656c 662e 5f72 6573         self._res
+00006ad0: 6574 5f72 6573 756c 7473 2829 0a0a 2020  et_results()..  
+00006ae0: 2020 6465 6620 7265 6d6f 7665 5f61 6e61    def remove_ana
+00006af0: 6c79 7369 735f 6c69 6d69 7473 2873 656c  lysis_limits(sel
+00006b00: 6629 3a0a 2020 2020 2020 2020 2222 2252  f):.        """R
+00006b10: 6573 6574 2061 6e61 6c79 7369 7320 6c69  eset analysis li
+00006b20: 6d69 7473 2074 6f20 6465 6661 756c 7420  mits to default 
+00006b30: 286e 6f20 6c69 6d69 7473 292e 2222 220a  (no limits).""".
+00006b40: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+00006b50: 5f61 6e61 6c79 7369 735f 6c69 6d69 7473  _analysis_limits
+00006b60: 280a 2020 2020 2020 2020 2020 2020 6c65  (.            le
+00006b70: 6674 5f78 3d30 2c0a 2020 2020 2020 2020  ft_x=0,.        
+00006b80: 2020 2020 7269 6768 745f 785f 6c65 6674      right_x_left
+00006b90: 3d73 656c 662e 5f74 6f70 5f63 6f6f 7264  =self._top_coord
+00006ba0: 5b30 5d2c 0a20 2020 2020 2020 2020 2020  [0],.           
+00006bb0: 206c 6566 745f 785f 7269 6768 743d 7365   left_x_right=se
+00006bc0: 6c66 2e5f 746f 705f 636f 6f72 645b 305d  lf._top_coord[0]
+00006bd0: 2c0a 2020 2020 2020 2020 2020 2020 7269  ,.            ri
+00006be0: 6768 745f 783d 7365 6c66 2e5f 6578 7465  ght_x=self._exte
+00006bf0: 726e 616c 5f6c 656e 6774 682c 0a20 2020  rnal_length,.   
+00006c00: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00006c10: 2320 7265 7365 7420 7265 7375 6c74 730a  # reset results.
+00006c20: 2020 2020 2020 2020 7365 6c66 2e5f 7265          self._re
+00006c30: 7365 745f 7265 7375 6c74 7328 290a 0a20  set_results().. 
+00006c40: 2020 2064 6566 2073 6574 5f61 6e61 6c79     def set_analy
+00006c50: 7369 735f 6c69 6d69 7473 280a 2020 2020  sis_limits(.    
+00006c60: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00006c70: 2020 6c65 6674 5f78 3a20 666c 6f61 7420    left_x: float 
+00006c80: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00006c90: 7269 6768 745f 783a 2066 6c6f 6174 203d  right_x: float =
+00006ca0: 204e 6f6e 652c 0a20 2020 2020 2020 206c   None,.        l
+00006cb0: 6566 745f 785f 7269 6768 743a 2066 6c6f  eft_x_right: flo
+00006cc0: 6174 203d 204e 6f6e 652c 0a20 2020 2020  at = None,.     
+00006cd0: 2020 2072 6967 6874 5f78 5f6c 6566 743a     right_x_left:
+00006ce0: 2066 6c6f 6174 203d 204e 6f6e 652c 0a20   float = None,. 
+00006cf0: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
+00006d00: 2273 6574 206c 696d 6974 7320 6f6e 2073  "set limits on s
+00006d10: 6c6f 7065 2061 6e61 6c79 7369 7320 7365  lope analysis se
+00006d20: 6172 6368 2e0a 0a20 2020 2020 2020 2050  arch...        P
+00006d30: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+00006d40: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00006d50: 2020 2020 206c 6566 745f 7820 3a20 666c       left_x : fl
+00006d60: 6f61 740a 2020 2020 2020 2020 2020 2020  oat.            
+00006d70: 6c65 6674 2078 2063 6f6f 7264 696e 6174  left x coordinat
+00006d80: 6520 6f66 2073 6561 7263 682c 2064 6566  e of search, def
+00006d90: 696e 6573 206f 7574 6572 2065 6467 650a  ines outer edge.
+00006da0: 2020 2020 2020 2020 2020 2020 6f66 2074              of t
+00006db0: 6f70 206f 6620 7365 6172 6368 0a20 2020  op of search.   
+00006dc0: 2020 2020 2072 6967 6874 5f78 203a 2066       right_x : f
+00006dd0: 6c6f 6174 0a20 2020 2020 2020 2020 2020  loat.           
+00006de0: 2072 6967 6874 2078 2063 6f6f 7264 696e   right x coordin
+00006df0: 6174 6520 7365 6172 6368 2c20 6465 6669  ate search, defi
+00006e00: 6e65 7320 6f75 7465 7220 6564 6765 206f  nes outer edge o
+00006e10: 660a 2020 2020 2020 2020 2020 2020 626f  f.            bo
+00006e20: 7474 6f6d 206f 6620 7365 6172 6368 0a20  ttom of search. 
+00006e30: 2020 2020 2020 206c 6566 745f 785f 7269         left_x_ri
+00006e40: 6768 7420 3a20 666c 6f61 742c 206f 7074  ght : float, opt
+00006e50: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
+00006e60: 2020 6c65 6674 2078 2063 6f6f 7264 696e    left x coordin
+00006e70: 6174 6520 7269 6768 7420 6861 6e64 206c  ate right hand l
+00006e80: 696d 6974 206f 6620 7365 6172 6368 2c20  imit of search, 
+00006e90: 6465 6669 6e65 730a 2020 2020 2020 2020  defines.        
+00006ea0: 2020 2020 696e 6e65 7220 6564 6765 206f      inner edge o
+00006eb0: 6620 746f 7020 6f66 2073 6561 7263 682e  f top of search.
+00006ec0: 2049 6620 6e6f 6e65 2069 676e 6f72 6564   If none ignored
+00006ed0: 2c20 6279 2064 6566 6175 6c74 204e 6f6e  , by default Non
+00006ee0: 650a 2020 2020 2020 2020 7269 6768 745f  e.        right_
+00006ef0: 785f 6c65 6674 203a 2066 6c6f 6174 2c20  x_left : float, 
+00006f00: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
+00006f10: 2020 2020 2072 6967 6874 2078 2063 6f6f       right x coo
+00006f20: 7264 696e 6174 6520 6c65 6674 2068 616e  rdinate left han
+00006f30: 6420 6c69 6d69 7420 6f66 2073 6561 7263  d limit of searc
+00006f40: 682c 2064 6566 696e 6573 0a20 2020 2020  h, defines.     
+00006f50: 2020 2020 2020 2069 6e6e 6572 2065 6467         inner edg
+00006f60: 6520 6f66 2062 6f74 746f 6d20 6f66 2073  e of bottom of s
+00006f70: 6561 7263 682e 2049 6620 6e6f 6e65 2069  earch. If none i
+00006f80: 676e 6f72 6564 2c20 6279 2064 6566 6175  gnored, by defau
+00006f90: 6c74 204e 6f6e 650a 2020 2020 2020 2020  lt None.        
+00006fa0: 2222 220a 2020 2020 2020 2020 2320 7365  """.        # se
+00006fb0: 7420 746f 2063 7572 7265 6e74 206d 6f64  t to current mod
+00006fc0: 656c 2076 616c 7565 7320 6966 206e 6f74  el values if not
+00006fd0: 2073 6574 2c20 656c 7365 2063 6865 636b   set, else check
+00006fe0: 2069 6e70 7574 2069 7320 7661 6c69 640a   input is valid.
+00006ff0: 2020 2020 2020 2020 6966 206c 6566 745f          if left_
+00007000: 7820 6973 204e 6f6e 653a 0a20 2020 2020  x is None:.     
+00007010: 2020 2020 2020 206c 6566 745f 7820 3d20         left_x = 
+00007020: 7365 6c66 2e5f 6c69 6d69 7473 5b30 5d0a  self._limits[0].
+00007030: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00007040: 2020 2020 2020 2020 2020 6461 7461 5f76            data_v
+00007050: 616c 6964 6174 696f 6e2e 6173 7365 7274  alidation.assert
+00007060: 5f70 6f73 6974 6976 655f 6e75 6d62 6572  _positive_number
+00007070: 286c 6566 745f 782c 2022 6c65 6674 5f78  (left_x, "left_x
+00007080: 206c 696d 6974 2229 0a0a 2020 2020 2020   limit")..      
+00007090: 2020 6966 206c 6566 745f 785f 7269 6768    if left_x_righ
+000070a0: 7420 6973 204e 6f6e 653a 0a20 2020 2020  t is None:.     
+000070b0: 2020 2020 2020 206c 6566 745f 785f 7269         left_x_ri
+000070c0: 6768 7420 3d20 7365 6c66 2e5f 6c69 6d69  ght = self._limi
+000070d0: 7473 5b31 5d0a 2020 2020 2020 2020 656c  ts[1].        el
+000070e0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000070f0: 6461 7461 5f76 616c 6964 6174 696f 6e2e  data_validation.
+00007100: 6173 7365 7274 5f73 7472 6963 746c 795f  assert_strictly_
+00007110: 706f 7369 7469 7665 5f6e 756d 6265 7228  positive_number(
+00007120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007130: 206c 6566 745f 785f 7269 6768 742c 2022   left_x_right, "
+00007140: 6c65 6674 5f78 2072 6967 6874 2063 6f6f  left_x right coo
+00007150: 7264 696e 6174 6522 0a20 2020 2020 2020  rdinate".       
+00007160: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00007170: 6966 2072 6967 6874 5f78 5f6c 6566 7420  if right_x_left 
+00007180: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00007190: 2020 2020 2072 6967 6874 5f78 5f6c 6566       right_x_lef
+000071a0: 7420 3d20 7365 6c66 2e5f 6c69 6d69 7473  t = self._limits
+000071b0: 5b32 5d0a 2020 2020 2020 2020 656c 7365  [2].        else
+000071c0: 3a0a 2020 2020 2020 2020 2020 2020 6461  :.            da
+000071d0: 7461 5f76 616c 6964 6174 696f 6e2e 6173  ta_validation.as
+000071e0: 7365 7274 5f73 7472 6963 746c 795f 706f  sert_strictly_po
+000071f0: 7369 7469 7665 5f6e 756d 6265 7228 7269  sitive_number(ri
+00007200: 6768 745f 782c 2022 7269 6768 745f 785f  ght_x, "right_x_
+00007210: 6c69 6d69 7422 290a 0a20 2020 2020 2020  limit")..       
+00007220: 2069 6620 7269 6768 745f 7820 6973 204e   if right_x is N
+00007230: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00007240: 2072 6967 6874 5f78 203d 2073 656c 662e   right_x = self.
+00007250: 5f6c 696d 6974 735b 335d 0a20 2020 2020  _limits[3].     
+00007260: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00007270: 2020 2020 2064 6174 615f 7661 6c69 6461       data_valida
+00007280: 7469 6f6e 2e61 7373 6572 745f 7374 7269  tion.assert_stri
+00007290: 6374 6c79 5f70 6f73 6974 6976 655f 6e75  ctly_positive_nu
+000072a0: 6d62 6572 280a 2020 2020 2020 2020 2020  mber(.          
+000072b0: 2020 2020 2020 7269 6768 745f 785f 6c65        right_x_le
+000072c0: 6674 2c20 2272 6967 6874 5f78 206c 6566  ft, "right_x lef
+000072d0: 7420 636f 6f72 6469 6e61 7465 220a 2020  t coordinate".  
+000072e0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+000072f0: 2020 2020 2023 2069 6620 6f6e 6c79 206f       # if only o
+00007300: 6e65 206f 6620 7468 6520 646f 7562 6c65  ne of the double
+00007310: 2070 6172 616d 6574 6572 7320 6973 2064   parameters is d
+00007320: 6566 696e 6564 0a20 2020 2020 2020 2023  efined.        #
+00007330: 2074 6865 206f 7468 6572 2073 686f 756c   the other shoul
+00007340: 6420 6265 2073 6574 2075 7020 746f 2065  d be set up to e
+00007350: 7175 616c 2069 740a 2020 2020 2020 2020  qual it.        
+00007360: 2320 6f72 2074 6865 2064 6961 6772 616d  # or the diagram
+00007370: 2069 7320 636f 6e66 7573 696e 670a 2020   is confusing.  
+00007380: 2020 2020 2020 6966 206c 6566 745f 785f        if left_x_
+00007390: 7269 6768 7420 6973 206e 6f74 204e 6f6e  right is not Non
+000073a0: 6520 616e 6420 7269 6768 745f 785f 6c65  e and right_x_le
+000073b0: 6674 2069 7320 4e6f 6e65 3a0a 2020 2020  ft is None:.    
+000073c0: 2020 2020 2020 2020 7269 6768 745f 785f          right_x_
+000073d0: 6c65 6674 203d 206c 6566 745f 785f 7269  left = left_x_ri
+000073e0: 6768 740a 0a20 2020 2020 2020 2069 6620  ght..        if 
+000073f0: 7269 6768 745f 785f 6c65 6674 2069 7320  right_x_left is 
+00007400: 6e6f 7420 4e6f 6e65 2061 6e64 206c 6566  not None and lef
+00007410: 745f 785f 7269 6768 7420 6973 204e 6f6e  t_x_right is Non
+00007420: 653a 0a20 2020 2020 2020 2020 2020 206c  e:.            l
+00007430: 6566 745f 785f 7269 6768 7420 3d20 7269  eft_x_right = ri
+00007440: 6768 745f 785f 6c65 6674 0a0a 2020 2020  ght_x_left..    
+00007450: 2020 2020 2320 656e 666f 7263 6520 6861      # enforce ha
+00007460: 7264 2062 6f75 6e64 6172 6965 7320 666f  rd boundaries fo
+00007470: 7220 6c69 6d69 7473 0a20 2020 2020 2020  r limits.       
+00007480: 206c 6566 745f 7820 3d20 6d61 7828 6c65   left_x = max(le
+00007490: 6674 5f78 2c20 3029 0a20 2020 2020 2020  ft_x, 0).       
+000074a0: 206c 6566 745f 785f 7269 6768 7420 3d20   left_x_right = 
+000074b0: 6d69 6e28 6c65 6674 5f78 5f72 6967 6874  min(left_x_right
+000074c0: 2c20 7365 6c66 2e5f 746f 705f 636f 6f72  , self._top_coor
+000074d0: 645b 305d 290a 2020 2020 2020 2020 7269  d[0]).        ri
+000074e0: 6768 745f 7820 3d20 6d69 6e28 7269 6768  ght_x = min(righ
+000074f0: 745f 782c 2073 656c 662e 5f65 7874 6572  t_x, self._exter
+00007500: 6e61 6c5f 6c65 6e67 7468 290a 2020 2020  nal_length).    
+00007510: 2020 2020 7269 6768 745f 785f 6c65 6674      right_x_left
+00007520: 203d 206d 6178 2872 6967 6874 5f78 5f6c   = max(right_x_l
+00007530: 6566 742c 2073 656c 662e 5f74 6f70 5f63  eft, self._top_c
+00007540: 6f6f 7264 5b30 5d29 0a0a 2020 2020 2020  oord[0])..      
+00007550: 2020 2320 6368 6563 6b20 6f72 6465 7220    # check order 
+00007560: 6973 206f 6b61 790a 2020 2020 2020 2020  is okay.        
+00007570: 6966 206c 6566 745f 7820 3e3d 206c 6566  if left_x >= lef
+00007580: 745f 785f 7269 6768 7420 6f72 2072 6967  t_x_right or rig
+00007590: 6874 5f78 5f6c 6566 7420 3e3d 2072 6967  ht_x_left >= rig
+000075a0: 6874 5f78 3a0a 2020 2020 2020 2020 2020  ht_x:.          
+000075b0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+000075c0: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
+000075d0: 2020 2020 226c 696d 6974 7320 6f75 7420      "limits out 
+000075e0: 6f66 206f 7264 6572 206f 7220 636f 6e66  of order or conf
+000075f0: 6c69 6374 696e 672c 2063 6865 636b 2069  licting, check i
+00007600: 6e70 7574 2066 6f72 2061 6e61 6c79 7369  nput for analysi
+00007610: 7320 6c69 6d69 7473 220a 2020 2020 2020  s limits".      
+00007620: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00007630: 2073 656c 662e 5f6c 696d 6974 7320 3d20   self._limits = 
+00007640: 5b6c 6566 745f 782c 206c 6566 745f 785f  [left_x, left_x_
+00007650: 7269 6768 742c 2072 6967 6874 5f78 5f6c  right, right_x_l
+00007660: 6566 742c 2072 6967 6874 5f78 5d0a 0a20  eft, right_x].. 
+00007670: 2020 2020 2020 2023 2072 6573 6574 2072         # reset r
+00007680: 6573 756c 7473 0a20 2020 2020 2020 2073  esults.        s
+00007690: 656c 662e 5f72 6573 6574 5f72 6573 756c  elf._reset_resul
+000076a0: 7473 2829 0a0a 2020 2020 6465 6620 5f73  ts()..    def _s
+000076b0: 6574 5f65 6e74 7279 5f65 7869 745f 706c  et_entry_exit_pl
+000076c0: 616e 6573 2873 656c 6629 3a0a 2020 2020  anes(self):.    
+000076d0: 2020 2020 2222 2246 756e 6374 696f 6e20      """Function 
+000076e0: 746f 2067 656e 6572 6174 6520 7365 6172  to generate sear
+000076f0: 6368 2070 6c61 6e65 7320 6261 7365 6420  ch planes based 
+00007700: 6f6e 2061 206d 6574 686f 640a 2020 2020  on a method.    
+00007710: 2020 2020 6f66 2070 7265 6465 7465 726d      of predeterm
+00007720: 696e 696e 6720 7768 6572 6520 7468 6520  ining where the 
+00007730: 6661 696c 7572 6520 706c 616e 6520 7769  failure plane wi
+00007740: 6c6c 2065 6e74 6572 2061 6e64 0a20 2020  ll enter and.   
+00007750: 2020 2020 2065 7869 7420 7468 6520 6d6f       exit the mo
+00007760: 6465 6c2e 2222 220a 0a20 2020 2020 2020  del."""..       
+00007770: 2023 206e 756d 6265 7220 6f66 2064 6966   # number of dif
+00007780: 6665 7265 6e74 2072 6164 6969 2074 6f20  ferent radii to 
+00007790: 636f 6e73 6964 6572 2066 6f72 2074 6865  consider for the
+000077a0: 2073 616d 6520 656e 6420 706f 696e 7473   same end points
+000077b0: 0a20 2020 2020 2020 206e 756d 5f63 6972  .        num_cir
+000077c0: 636c 6573 203d 206d 6178 2835 2c20 696e  cles = max(5, in
+000077d0: 7428 7365 6c66 2e5f 6974 6572 6174 696f  t(self._iteratio
+000077e0: 6e73 202f 2038 3030 2929 0a0a 2020 2020  ns / 800))..    
+000077f0: 2020 2020 2320 6765 6e65 7261 7465 2063      # generate c
+00007800: 6f6f 7264 696e 6174 6573 2066 6f72 206c  oordinates for l
+00007810: 6566 7420 6f66 2073 6c6f 7065 0a20 2020  eft of slope.   
+00007820: 2020 2020 2070 6f69 6e74 5f63 6f6d 6269       point_combi
+00007830: 6e61 7469 6f6e 7320 3d20 7365 6c66 2e5f  nations = self._
+00007840: 6974 6572 6174 696f 6e73 202f 206e 756d  iterations / num
+00007850: 5f63 6972 636c 6573 0a0a 2020 2020 2020  _circles..      
+00007860: 2020 2320 7369 6d70 6c69 6669 6361 7469    # simplificati
+00007870: 6f6e 2067 656e 6572 616c 6c79 2077 696c  on generally wil
+00007880: 6c20 6d65 616e 2073 6c69 6768 746c 7920  l mean slightly 
+00007890: 6c65 7373 2069 7465 7261 7469 6f6e 7320  less iterations 
+000078a0: 6f63 6375 722e 0a20 2020 2020 2020 2023  occur..        #
+000078b0: 2066 6f72 2074 6865 2064 6566 6175 6c74   for the default
+000078c0: 2076 616c 7565 206f 6620 3230 3030 2074   value of 2000 t
+000078d0: 6869 7320 7769 6c6c 2062 6520 6578 6163  his will be exac
+000078e0: 740a 2020 2020 2020 2020 2320 2835 2063  t.        # (5 c
+000078f0: 6972 636c 6573 202a 2032 3020 746f 7020  ircles * 20 top 
+00007900: 2a20 3230 2062 6f74 746f 6d20 3d20 3230  * 20 bottom = 20
+00007910: 3030 2065 7861 6374 2063 6f6d 6269 6e61  00 exact combina
+00007920: 7469 6f6e 7329 0a20 2020 2020 2020 206e  tions).        n
+00007930: 756d 5f70 6f69 6e74 735f 746f 7020 3d20  um_points_top = 
+00007940: 696e 7428 7371 7274 2870 6f69 6e74 5f63  int(sqrt(point_c
+00007950: 6f6d 6269 6e61 7469 6f6e 7329 290a 2020  ombinations)).  
+00007960: 2020 2020 2020 6e75 6d5f 706f 696e 7473        num_points
+00007970: 5f62 6f74 203d 206e 756d 5f70 6f69 6e74  _bot = num_point
+00007980: 735f 746f 700a 0a20 2020 2020 2020 2077  s_top..        w
+00007990: 6869 6c65 206e 756d 5f70 6f69 6e74 735f  hile num_points_
+000079a0: 746f 7020 2a20 6e75 6d5f 706f 696e 7473  top * num_points
+000079b0: 5f62 6f74 202a 206e 756d 5f63 6972 636c  _bot * num_circl
+000079c0: 6573 203c 2073 656c 662e 5f69 7465 7261  es < self._itera
+000079d0: 7469 6f6e 733a 0a20 2020 2020 2020 2020  tions:.         
+000079e0: 2020 206e 756d 5f70 6f69 6e74 735f 626f     num_points_bo
+000079f0: 7420 2b3d 2031 0a0a 2020 2020 2020 2020  t += 1..        
+00007a00: 2320 7265 6d6f 7665 206e 756d 6265 7220  # remove number 
+00007a10: 6f66 2070 6f69 6e74 7320 6f6e 2074 6f70  of points on top
+00007a20: 2074 6f20 6265 2073 7072 6561 6420 746f   to be spread to
+00007a30: 2061 6c6c 6f77 2066 6f72 2073 7065 6369   allow for speci
+00007a40: 6669 630a 2020 2020 2020 2020 2320 706f  fic.        # po
+00007a50: 696e 7473 206e 6578 7420 746f 2074 6865  ints next to the
+00007a60: 2065 6467 6520 6f66 206c 6f61 6473 0a20   edge of loads. 
+00007a70: 2020 2020 2020 206e 756d 5f70 6f69 6e74         num_point
+00007a80: 735f 746f 7020 3d20 6e75 6d5f 706f 696e  s_top = num_poin
+00007a90: 7473 5f74 6f70 202d 206c 656e 2873 656c  ts_top - len(sel
+00007aa0: 662e 5f6c 6c73 2920 2d20 6c65 6e28 7365  f._lls) - len(se
+00007ab0: 6c66 2e5f 7564 6c73 290a 0a20 2020 2020  lf._udls)..     
+00007ac0: 2020 2023 2067 6574 206c 696d 6974 7320     # get limits 
+00007ad0: 6f6e 2062 6f75 6e64 7320 6f66 2073 6c6f  on bounds of slo
+00007ae0: 7065 0a20 2020 2020 2020 2023 206e 6f74  pe.        # not
+00007af0: 2073 6f6d 6520 6c69 6d69 7473 206d 6967   some limits mig
+00007b00: 6874 2073 7469 6c6c 2073 7472 6574 6368  ht still stretch
+00007b10: 206f 6666 2073 6c6f 7065 0a20 2020 2020   off slope.     
+00007b20: 2020 2023 2062 7574 203c 3d20 6368 6563     # but <= chec
+00007b30: 6b20 6c61 7465 7220 636f 6e73 6964 6572  k later consider
+00007b40: 7320 7468 6973 2e0a 2020 2020 2020 2020  s this..        
+00007b50: 7831 2c20 7832 2c20 7833 2c20 7834 203d  x1, x2, x3, x4 =
+00007b60: 2073 656c 662e 5f6c 696d 6974 730a 0a20   self._limits.. 
+00007b70: 2020 2020 2020 2023 2063 6f6f 7264 696e         # coordin
+00007b80: 6174 6573 2066 6f72 2066 6169 6c75 7265  ates for failure
+00007b90: 2070 6c61 6e65 7320 6174 2074 6f70 206f   planes at top o
+00007ba0: 6620 736c 6f70 650a 2020 2020 2020 2020  f slope.        
+00007bb0: 2320 7920 636f 6f72 6469 6e61 7465 2069  # y coordinate i
+00007bc0: 7320 616c 7761 7973 2074 6865 2063 6f6f  s always the coo
+00007bd0: 7264 696e 6174 6520 6f66 2074 6865 2074  rdinate of the t
+00007be0: 6f70 206f 6620 7468 6520 736c 6f70 650a  op of the slope.
+00007bf0: 2020 2020 2020 2020 6c65 6674 5f63 6f6f          left_coo
+00007c00: 7264 7320 3d20 5b0a 2020 2020 2020 2020  rds = [.        
+00007c10: 2020 2020 2878 3120 2b20 286e 202f 2028      (x1 + (n / (
+00007c20: 6e75 6d5f 706f 696e 7473 5f74 6f70 202d  num_points_top -
+00007c30: 2031 2929 202a 2028 7832 202d 2078 3129   1)) * (x2 - x1)
+00007c40: 2c20 7365 6c66 2e5f 746f 705f 636f 6f72  , self._top_coor
+00007c50: 645b 315d 290a 2020 2020 2020 2020 2020  d[1]).          
+00007c60: 2020 666f 7220 6e20 696e 2072 616e 6765    for n in range
+00007c70: 286e 756d 5f70 6f69 6e74 735f 746f 7029  (num_points_top)
+00007c80: 0a20 2020 2020 2020 205d 0a0a 2020 2020  .        ]..    
+00007c90: 2020 2020 2320 636f 6f64 696e 6174 6573      # coodinates
+00007ca0: 2066 6f72 2074 6865 2062 6f74 746f 6d20   for the bottom 
+00007cb0: 6f66 2074 6865 2066 6169 6c75 7265 2070  of the failure p
+00007cc0: 6c61 6e65 0a20 2020 2020 2020 2023 2063  lane.        # c
+00007cd0: 616e 2062 6520 6174 2062 6f74 746f 6d20  an be at bottom 
+00007ce0: 6f72 206f 6e20 736c 6f70 652c 2073 6f20  or on slope, so 
+00007cf0: 7920 6973 2066 756e 6374 696f 6e20 6f66  y is function of
+00007d00: 2078 2061 6e64 0a20 2020 2020 2020 2023   x and.        #
+00007d10: 206e 6565 6473 2074 6f20 6265 2064 6574   needs to be det
+00007d20: 6572 6d69 6e65 6420 666f 7220 6469 6666  ermined for diff
+00007d30: 6572 656e 7420 706f 696e 7473 0a20 2020  erent points.   
+00007d40: 2020 2020 2072 6967 6874 5f63 6f6f 7264       right_coord
+00007d50: 735f 7820 3d20 5b0a 2020 2020 2020 2020  s_x = [.        
+00007d60: 2020 2020 7833 202b 2028 6e20 2f20 286e      x3 + (n / (n
+00007d70: 756d 5f70 6f69 6e74 735f 626f 7429 2920  um_points_bot)) 
+00007d80: 2a20 2878 3420 2d20 7833 290a 2020 2020  * (x4 - x3).    
+00007d90: 2020 2020 2020 2020 666f 7220 6e20 696e          for n in
+00007da0: 2072 616e 6765 2831 2c20 6e75 6d5f 706f   range(1, num_po
+00007db0: 696e 7473 5f62 6f74 202b 2031 290a 2020  ints_bot + 1).  
+00007dc0: 2020 2020 2020 5d0a 0a20 2020 2020 2020        ]..       
+00007dd0: 2072 6967 6874 5f63 6f6f 7264 7320 3d20   right_coords = 
+00007de0: 5b0a 2020 2020 2020 2020 2020 2020 2878  [.            (x
+00007df0: 2c20 7365 6c66 2e67 6574 5f65 7874 6572  , self.get_exter
+00007e00: 6e61 6c5f 795f 696e 7465 7273 6563 7469  nal_y_intersecti
+00007e10: 6f6e 2878 2929 2066 6f72 2078 2069 6e20  on(x)) for x in 
+00007e20: 7269 6768 745f 636f 6f72 6473 5f78 0a20  right_coords_x. 
+00007e30: 2020 2020 2020 205d 0a0a 2020 2020 2020         ]..      
+00007e40: 2020 7365 6172 6368 203d 205b 5d0a 0a20    search = [].. 
+00007e50: 2020 2020 2020 2023 2061 6464 2069 6e20         # add in 
+00007e60: 636f 6f72 6469 6e61 7465 7320 6469 7265  coordinates dire
+00007e70: 6374 6c79 2061 646a 6163 656e 7420 746f  ctly adjacent to
+00007e80: 206c 6f61 6473 0a20 2020 2020 2020 2066   loads.        f
+00007e90: 6f72 206c 6c20 696e 2073 656c 662e 5f6c  or ll in self._l
+00007ea0: 6c73 3a0a 2020 2020 2020 2020 2020 2020  ls:.            
+00007eb0: 6c65 6674 5f63 6f6f 7264 7320 2b3d 205b  left_coords += [
+00007ec0: 286c 6c2e 636f 6f72 6420 2d20 302e 3030  (ll.coord - 0.00
+00007ed0: 312c 2073 656c 662e 5f74 6f70 5f63 6f6f  1, self._top_coo
+00007ee0: 7264 5b31 5d29 5d0a 0a20 2020 2020 2020  rd[1])]..       
+00007ef0: 2066 6f72 2075 646c 2069 6e20 7365 6c66   for udl in self
+00007f00: 2e5f 7564 6c73 3a0a 2020 2020 2020 2020  ._udls:.        
+00007f10: 2020 2020 6c65 6674 5f63 6f6f 7264 7320      left_coords 
+00007f20: 2b3d 205b 2875 646c 2e6c 6566 7420 2d20  += [(udl.left - 
+00007f30: 302e 3030 312c 2073 656c 662e 5f74 6f70  0.001, self._top
+00007f40: 5f63 6f6f 7264 5b31 5d29 5d0a 0a20 2020  _coord[1])]..   
+00007f50: 2020 2020 2023 206c 6f6f 7020 7468 726f       # loop thro
+00007f60: 7567 6820 6c65 6674 2061 6e64 2072 6967  ugh left and rig
+00007f70: 6874 2070 6f69 6e74 7320 746f 2067 656e  ht points to gen
+00007f80: 6572 6174 6520 636f 6f72 6469 6e61 7465  erate coordinate
+00007f90: 730a 2020 2020 2020 2020 666f 7220 6c5f  s.        for l_
+00007fa0: 6320 696e 206c 6566 745f 636f 6f72 6473  c in left_coords
+00007fb0: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
+00007fc0: 7220 725f 6320 696e 2072 6967 6874 5f63  r r_c in right_c
+00007fd0: 6f6f 7264 733a 0a20 2020 2020 2020 2020  oords:.         
+00007fe0: 2020 2020 2020 2069 6620 7574 696c 6974         if utilit
+00007ff0: 6965 732e 6469 7374 5f70 6f69 6e74 7328  ies.dist_points(
+00008000: 6c5f 632c 2072 5f63 2920 3e20 7365 6c66  l_c, r_c) > self
+00008010: 2e5f 6d69 6e5f 6661 696c 7572 655f 6469  ._min_failure_di
+00008020: 7374 616e 6365 3a0a 2020 2020 2020 2020  stance:.        
+00008030: 2020 2020 2020 2020 2020 2020 7365 6172              sear
+00008040: 6368 202b 3d20 7365 6c66 2e5f 6765 6e65  ch += self._gene
+00008050: 7261 7465 5f70 6c61 6e65 7328 6c5f 632c  rate_planes(l_c,
+00008060: 2072 5f63 2c20 6e75 6d5f 6369 7263 6c65   r_c, num_circle
+00008070: 7329 0a0a 2020 2020 2020 2020 7365 6c66  s)..        self
+00008080: 2e5f 7365 6172 6368 203d 2073 6561 7263  ._search = searc
+00008090: 680a 0a20 2020 2064 6566 205f 6765 6e65  h..    def _gene
+000080a0: 7261 7465 5f70 6c61 6e65 7328 7365 6c66  rate_planes(self
+000080b0: 2c20 6c5f 632c 2072 5f63 2c20 6e75 6d5f  , l_c, r_c, num_
+000080c0: 6369 7263 6c65 733d 3529 3a0a 2020 2020  circles=5):.    
+000080d0: 2020 2020 2222 2247 656e 6572 6174 6520      """Generate 
+000080e0: 6661 696c 7572 6520 706c 616e 6520 6369  failure plane ci
+000080f0: 7263 6c65 2063 6f6f 7264 696e 6174 6573  rcle coordinates
+00008100: 2077 6974 6820 656e 7472 7920 616e 6420   with entry and 
+00008110: 6578 6974 2070 6f69 6e74 2e0a 0a20 2020  exit point...   
+00008120: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
+00008130: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+00008140: 2d2d 0a20 2020 2020 2020 206c 5f63 203a  --.        l_c :
+00008150: 2066 6c6f 6174 0a20 2020 2020 2020 2020   float.         
+00008160: 2020 204c 6566 7420 7820 636f 6f72 6469     Left x coordi
+00008170: 6e61 7465 2077 6869 6368 2072 6570 7265  nate which repre
+00008180: 7365 6e74 7320 7468 6520 746f 7020 6f66  sents the top of
+00008190: 2074 6865 2066 6169 6c75 7265 0a20 2020   the failure.   
+000081a0: 2020 2020 2020 2020 2070 6c61 6e65 2e0a           plane..
+000081b0: 2020 2020 2020 2020 725f 6320 3a20 666c          r_c : fl
+000081c0: 6f61 740a 2020 2020 2020 2020 2020 2020  oat.            
+000081d0: 5269 6768 7420 7820 636f 6f72 6469 6e61  Right x coordina
+000081e0: 7465 2077 6869 6368 2072 6570 7265 7365  te which represe
+000081f0: 6e74 7320 7468 6520 626f 7474 6f6d 206f  nts the bottom o
+00008200: 6620 7468 6520 6661 696c 7572 650a 2020  f the failure.  
+00008210: 2020 2020 2020 2020 2020 706c 616e 652e            plane.
+00008220: 0a20 2020 2020 2020 206e 756d 5f63 6972  .        num_cir
+00008230: 636c 6573 203a 2069 6e74 2c20 6f70 7469  cles : int, opti
+00008240: 6f6e 616c 0a20 2020 2020 2020 2020 2020  onal.           
+00008250: 206e 756d 6265 7220 6f66 2064 6966 6665   number of diffe
+00008260: 7265 6e74 2063 6972 636c 6520 7261 6469  rent circle radi
+00008270: 6920 746f 2061 7373 6573 7320 7061 7373  i to assess pass
+00008280: 696e 6720 7468 726f 7567 680a 2020 2020  ing through.    
+00008290: 2020 2020 2020 2020 7468 6520 656e 7472          the entr
+000082a0: 7920 616e 6420 6578 6974 2070 6f69 6e74  y and exit point
+000082b0: 732c 2062 7920 6465 6661 756c 7420 350a  s, by default 5.
+000082c0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+000082d0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+000082e0: 0a20 2020 2020 2020 206c 6973 7420 6f66  .        list of
+000082f0: 2064 6963 7469 6f6e 6172 6965 7320 6f66   dictionaries of
+00008300: 2074 6865 2066 6f72 6d3a 0a20 2020 2020   the form:.     
+00008310: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
+00008320: 2022 6c5f 6322 3a20 6c5f 632c 0a20 2020   "l_c": l_c,.   
+00008330: 2020 2020 2020 2020 2022 725f 6322 3a20           "r_c": 
+00008340: 725f 632c 0a20 2020 2020 2020 2020 2020  r_c,.           
+00008350: 2022 635f 7822 3a20 635f 782c 0a20 2020   "c_x": c_x,.   
+00008360: 2020 2020 2020 2020 2022 635f 7922 3a20           "c_y": 
+00008370: 635f 792c 0a20 2020 2020 2020 2020 2020  c_y,.           
+00008380: 2022 7261 6469 7573 223a 2072 6164 6975   "radius": radiu
+00008390: 732c 0a20 2020 2020 2020 207d 0a0a 2020  s,.        }..  
+000083a0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000083b0: 2020 7365 6172 6368 203d 205b 5d0a 0a20    search = [].. 
+000083c0: 2020 2020 2020 2023 2061 7373 756d 6520         # assume 
+000083d0: 6120 7374 6172 7469 6e67 2063 6972 636c  a starting circl
+000083e0: 6520 7468 6174 2068 6173 2061 2073 7472  e that has a str
+000083f0: 6169 6768 7420 7665 7274 6963 616c 2073  aight vertical s
+00008400: 6c6f 7065 2064 6f77 6e20 6174 2074 6865  lope down at the
+00008410: 2074 6f70 206f 6620 7468 6520 736c 6f70   top of the slop
+00008420: 650a 2020 2020 2020 2020 2320 7468 6973  e.        # this
+00008430: 206d 6561 6e73 2074 6865 2063 656e 7472   means the centr
+00008440: 6520 6f66 2074 6865 2063 6972 636c 6520  e of the circle 
+00008450: 6973 2069 6e20 6c69 6e65 2077 6974 6820  is in line with 
+00008460: 7468 6520 746f 7020 6f66 2074 6865 2073  the top of the s
+00008470: 6c6f 7065 0a20 2020 2020 2020 2023 2073  lope.        # s
+00008480: 696e 6365 2074 6865 2074 616e 6765 6e74  ince the tangent
+00008490: 206f 6620 7468 6520 6369 7263 6c65 2069   of the circle i
+000084a0: 7320 7065 7270 656e 6469 6375 6c61 7220  s perpendicular 
+000084b0: 746f 2074 6865 2063 656e 7472 650a 0a20  to the centre.. 
+000084c0: 2020 2020 2020 2023 2061 6e67 6c65 206f         # angle o
+000084d0: 6620 736c 6f70 6520 6f66 2063 686f 6f72  f slope of choor
+000084e0: 6420 2846 6f72 2063 6972 6375 6c61 7220  d (For circular 
+000084f0: 736c 6f70 6529 0a20 2020 2020 2020 2062  slope).        b
+00008500: 6574 6120 3d20 6174 616e 2828 6c5f 635b  eta = atan((l_c[
+00008510: 315d 202d 2072 5f63 5b31 5d29 202f 2028  1] - r_c[1]) / (
+00008520: 725f 635b 305d 202d 206c 5f63 5b30 5d29  r_c[0] - l_c[0])
+00008530: 290a 0a20 2020 2020 2020 2023 2068 616c  )..        # hal
+00008540: 6620 6f66 2074 6865 2063 6972 636c 6520  f of the circle 
+00008550: 636f 6f72 6420 7468 6174 2070 6173 7365  coord that passe
+00008560: 7373 2066 726f 6d20 746f 7020 6f66 2070  ss from top of p
+00008570: 6f69 6e74 2074 6f20 626f 7474 6f6d 206f  oint to bottom o
+00008580: 6620 706f 696e 740a 2020 2020 2020 2020  f point.        
+00008590: 6861 6c66 5f63 6f6f 7264 5f64 6973 7461  half_coord_dista
+000085a0: 6e63 6520 3d20 7371 7274 2828 6c5f 635b  nce = sqrt((l_c[
+000085b0: 315d 202d 2072 5f63 5b31 5d29 202a 2a20  1] - r_c[1]) ** 
+000085c0: 3220 2b20 2872 5f63 5b30 5d20 2d20 6c5f  2 + (r_c[0] - l_
+000085d0: 635b 305d 2920 2a2a 2032 2920 2f20 320a  c[0]) ** 2) / 2.
+000085e0: 0a20 2020 2020 2020 2023 2073 7461 7274  .        # start
+000085f0: 696e 6720 6369 7263 6c65 2064 6574 6169  ing circle detai
+00008600: 6c73 2c20 6966 2072 6164 6975 7320 3120  ls, if radius 1 
+00008610: 776f 756c 6420 6265 2061 2076 6572 7469  would be a verti
+00008620: 6361 6c20 736c 6f70 652e 0a20 2020 2020  cal slope..     
+00008630: 2020 2023 2069 6e63 7265 6173 6520 746f     # increase to
+00008640: 2031 2e31 2074 6f20 7072 6576 656e 7420   1.1 to prevent 
+00008650: 6d61 2064 656e 6f6d 696e 6174 6f72 2069  ma denominator i
+00008660: 7373 7565 7320 666f 7220 6269 7368 6f70  ssues for bishop
+00008670: 7320 6d65 7468 6f64 2e0a 2020 2020 2020  s method..      
+00008680: 2020 7374 6172 745f 7261 6469 7573 203d    start_radius =
+00008690: 2068 616c 665f 636f 6f72 645f 6469 7374   half_coord_dist
+000086a0: 616e 6365 202f 2063 6f73 2862 6574 6129  ance / cos(beta)
+000086b0: 202a 2031 2e31 0a20 2020 2020 2020 2023   * 1.1.        #
+000086c0: 2073 7461 7274 5f63 656e 7472 6520 3d20   start_centre = 
+000086d0: 286c 5f63 5b30 5d20 2b20 7374 6172 745f  (l_c[0] + start_
+000086e0: 7261 6469 7573 2c20 6c5f 635b 315d 290a  radius, l_c[1]).
+000086f0: 2020 2020 2020 2020 7374 6172 745f 6368          start_ch
+00008700: 6f72 645f 746f 5f63 656e 7472 6520 3d20  ord_to_centre = 
+00008710: 7371 7274 2873 7461 7274 5f72 6164 6975  sqrt(start_radiu
+00008720: 732a 2a32 202d 2068 616c 665f 636f 6f72  s**2 - half_coor
+00008730: 645f 6469 7374 616e 6365 2a2a 3229 0a20  d_distance**2). 
+00008740: 2020 2020 2020 2073 7461 7274 5f63 686f         start_cho
+00008750: 7264 5f74 6f5f 6564 6765 203d 2073 7461  rd_to_edge = sta
+00008760: 7274 5f72 6164 6975 7320 2d20 7374 6172  rt_radius - star
+00008770: 745f 6368 6f72 645f 746f 5f63 656e 7472  t_chord_to_centr
+00008780: 650a 0a20 2020 2020 2020 2023 2074 776f  e..        # two
+00008790: 2069 6e74 6572 7365 6374 696e 6720 6368   intersecting ch
+000087a0: 6f72 6473 2074 6872 6f75 6768 2063 6972  ords through cir
+000087b0: 636c 6520 6861 7665 2073 6567 6d65 6e74  cle have segment
+000087c0: 7320 6f66 2063 686f 7264 7320 7265 6c61  s of chords rela
+000087d0: 7465 640a 2020 2020 2020 2020 2320 6173  ted.        # as
+000087e0: 2061 202a 2062 203d 2063 202a 2064 202c   a * b = c * d ,
+000087f0: 2077 6865 7265 2061 2061 6e64 2062 2061   where a and b a
+00008800: 7265 2074 6865 206c 656e 6774 6873 206f  re the lengths o
+00008810: 6620 6368 6f72 6420 6f6e 2065 6163 6820  f chord on each 
+00008820: 7369 6465 206f 6620 696e 7465 7273 6563  side of intersec
+00008830: 7469 6f6e 0a20 2020 2020 2020 2023 2061  tion.        # a
+00008840: 7320 7375 6368 2077 6520 6861 7665 2068  s such we have h
+00008850: 616c 665f 636f 6f72 645f 6469 7374 616e  alf_coord_distan
+00008860: 6365 202a 2a20 3220 3d20 6368 6f72 645f  ce ** 2 = chord_
+00008870: 746f 5f65 6467 6520 2a20 2852 202b 2028  to_edge * (R + (
+00008880: 522d 6368 6f72 645f 746f 5f65 6467 6529  R-chord_to_edge)
+00008890: 2920 3d20 430a 2020 2020 2020 2020 4320  ) = C.        C 
+000088a0: 3d20 6861 6c66 5f63 6f6f 7264 5f64 6973  = half_coord_dis
+000088b0: 7461 6e63 652a 2a32 0a0a 2020 2020 2020  tance**2..      
+000088c0: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+000088d0: 2830 2c20 6e75 6d5f 6369 7263 6c65 7329  (0, num_circles)
+000088e0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+000088f0: 646f 6573 6e74 2069 6e63 6c75 6465 2067  doesnt include g
+00008900: 6f69 6e67 2061 6c6c 2074 6865 2077 6179  oing all the way
+00008910: 2069 6e20 7768 6963 6820 7765 2064 6f6e   in which we don
+00008920: 7420 7761 6e74 2074 6f20 646f 2061 6e79  t want to do any
+00008930: 7761 7973 0a20 2020 2020 2020 2020 2020  ways.           
+00008940: 2063 686f 7264 5f74 6f5f 6564 6765 203d   chord_to_edge =
+00008950: 2073 7461 7274 5f63 686f 7264 5f74 6f5f   start_chord_to_
+00008960: 6564 6765 202a 2028 6e75 6d5f 6369 7263  edge * (num_circ
+00008970: 6c65 7320 2d20 6929 202f 206e 756d 5f63  les - i) / num_c
+00008980: 6972 636c 6573 0a20 2020 2020 2020 2020  ircles.         
+00008990: 2020 2072 6164 6975 7320 3d20 7574 696c     radius = util
+000089a0: 6974 6965 732e 6369 7263 6c65 5f72 6164  ities.circle_rad
+000089b0: 6975 735f 6672 6f6d 5f61 6263 6428 6368  ius_from_abcd(ch
+000089c0: 6f72 645f 746f 5f65 6467 652c 2043 290a  ord_to_edge, C).
+000089d0: 2020 2020 2020 2020 2020 2020 6365 6e74              cent
+000089e0: 7265 203d 2075 7469 6c69 7469 6573 2e63  re = utilities.c
+000089f0: 6972 636c 655f 6365 6e74 7265 280a 2020  ircle_centre(.  
+00008a00: 2020 2020 2020 2020 2020 2020 2020 6265                be
+00008a10: 7461 3d62 6574 612c 0a20 2020 2020 2020  ta=beta,.       
+00008a20: 2020 2020 2020 2020 2063 686f 7264 5f69           chord_i
+00008a30: 6e74 6572 7365 6374 696f 6e3d 7574 696c  ntersection=util
+00008a40: 6974 6965 732e 6d69 645f 636f 6f72 6428  ities.mid_coord(
+00008a50: 6c5f 632c 2072 5f63 292c 0a20 2020 2020  l_c, r_c),.     
+00008a60: 2020 2020 2020 2020 2020 2063 686f 7264             chord
+00008a70: 5f74 6f5f 6365 6e74 7265 3d72 6164 6975  _to_centre=radiu
+00008a80: 7320 2d20 6368 6f72 645f 746f 5f65 6467  s - chord_to_edg
+00008a90: 652c 0a20 2020 2020 2020 2020 2020 2029  e,.            )
+00008aa0: 0a20 2020 2020 2020 2020 2020 2063 5f78  .            c_x
+00008ab0: 2c20 635f 7920 3d20 6365 6e74 7265 0a0a  , c_y = centre..
+00008ac0: 2020 2020 2020 2020 2020 2020 695f 6c69              i_li
+00008ad0: 7374 203d 2073 656c 662e 5f67 6574 5f63  st = self._get_c
+00008ae0: 6972 636c 655f 6578 7465 726e 616c 5f69  ircle_external_i
+00008af0: 6e74 6572 7365 6374 696f 6e28 635f 782c  ntersection(c_x,
+00008b00: 2063 5f79 2c20 7261 6469 7573 290a 0a20   c_y, radius).. 
+00008b10: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+00008b20: 6e28 7365 7428 695f 6c69 7374 2929 203c  n(set(i_list)) <
+00008b30: 2032 3a0a 2020 2020 2020 2020 2020 2020   2:.            
+00008b40: 2020 2020 636f 6e74 696e 7565 0a0a 2020      continue..  
+00008b50: 2020 2020 2020 2020 2020 6c5f 6320 3d20            l_c = 
+00008b60: 695f 6c69 7374 5b30 5d0a 2020 2020 2020  i_list[0].      
+00008b70: 2020 2020 2020 725f 6320 3d20 695f 6c69        r_c = i_li
+00008b80: 7374 5b31 5d0a 0a20 2020 2020 2020 2020  st[1]..         
+00008b90: 2020 2073 6561 7263 6820 2b3d 205b 0a20     search += [. 
+00008ba0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00008bb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008bc0: 2020 2020 2022 6c5f 6322 3a20 6c5f 632c       "l_c": l_c,
+00008bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008be0: 2020 2020 2022 725f 6322 3a20 725f 632c       "r_c": r_c,
+00008bf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008c00: 2020 2020 2022 635f 7822 3a20 635f 782c       "c_x": c_x,
+00008c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008c20: 2020 2020 2022 635f 7922 3a20 635f 792c       "c_y": c_y,
+00008c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008c40: 2020 2020 2022 7261 6469 7573 223a 2072       "radius": r
+00008c50: 6164 6975 732c 0a20 2020 2020 2020 2020  adius,.         
+00008c60: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00008c70: 2020 2020 205d 0a0a 2020 2020 2020 2020       ]..        
+00008c80: 7265 7475 726e 2073 6561 7263 680a 0a20  return search.. 
+00008c90: 2020 2064 6566 2061 6464 5f73 696e 676c     def add_singl
+00008ca0: 655f 656e 7472 795f 6578 6974 5f70 6c61  e_entry_exit_pla
+00008cb0: 6e65 2873 656c 662c 206c 5f63 782c 2072  ne(self, l_cx, r
+00008cc0: 5f63 782c 206e 756d 5f63 6972 636c 6573  _cx, num_circles
+00008cd0: 3d35 293a 0a20 2020 2020 2020 2022 2222  =5):.        """
+00008ce0: 4164 6420 6661 696c 7572 6520 706c 616e  Add failure plan
+00008cf0: 6520 746f 2062 6520 616e 616c 7973 6564  e to be analysed
+00008d00: 2062 6520 7370 6563 6966 7969 6e67 2073   be specifying s
+00008d10: 7461 7274 2061 6e64 2065 7869 7420 706f  tart and exit po
+00008d20: 696e 742e 0a0a 2020 2020 2020 2020 5061  int...        Pa
+00008d30: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+00008d40: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+00008d50: 2020 2020 6c5f 6320 3a20 666c 6f61 740a      l_c : float.
+00008d60: 2020 2020 2020 2020 2020 2020 4c65 6674              Left
+00008d70: 2078 2063 6f6f 7264 696e 6174 6520 7768   x coordinate wh
+00008d80: 6963 6820 7265 7072 6573 656e 7473 2074  ich represents t
+00008d90: 6865 2074 6f70 206f 6620 7468 6520 6661  he top of the fa
+00008da0: 696c 7572 650a 2020 2020 2020 2020 2020  ilure.          
+00008db0: 2020 706c 616e 652e 0a20 2020 2020 2020    plane..       
+00008dc0: 2072 5f63 203a 2066 6c6f 6174 0a20 2020   r_c : float.   
+00008dd0: 2020 2020 2020 2020 2052 6967 6874 2078           Right x
+00008de0: 2063 6f6f 7264 696e 6174 6520 7768 6963   coordinate whic
+00008df0: 6820 7265 7072 6573 656e 7473 2074 6865  h represents the
+00008e00: 2062 6f74 746f 6d20 6f66 2074 6865 2066   bottom of the f
+00008e10: 6169 6c75 7265 0a20 2020 2020 2020 2020  ailure.         
+00008e20: 2020 2070 6c61 6e65 2e0a 2020 2020 2020     plane..      
+00008e30: 2020 6e75 6d5f 6369 7263 6c65 7320 3a20    num_circles : 
+00008e40: 696e 742c 206f 7074 696f 6e61 6c0a 2020  int, optional.  
+00008e50: 2020 2020 2020 2020 2020 6e75 6d62 6572            number
+00008e60: 206f 6620 6469 6666 6572 656e 7420 6369   of different ci
+00008e70: 7263 6c65 2072 6164 6969 2074 6f20 6173  rcle radii to as
+00008e80: 7365 7373 2070 6173 7369 6e67 2074 6872  sess passing thr
+00008e90: 6f75 6768 0a20 2020 2020 2020 2020 2020  ough.           
+00008ea0: 2074 6865 2065 6e74 7279 2061 6e64 2065   the entry and e
+00008eb0: 7869 7420 706f 696e 7473 2c20 6279 2064  xit points, by d
+00008ec0: 6566 6175 6c74 2035 0a20 2020 2020 2020  efault 5.       
+00008ed0: 2022 2222 0a20 2020 2020 2020 2023 2061   """.        # a
+00008ee0: 6464 2062 7920 6164 6469 6e67 2069 6e20  dd by adding in 
+00008ef0: 6c65 6674 2061 6e64 2072 6967 6874 2066  left and right f
+00008f00: 6169 6c75 7265 2063 6f6f 7264 696e 6174  ailure coordinat
+00008f10: 650a 2020 2020 2020 2020 7365 6c66 2e5f  e.        self._
+00008f20: 696e 6469 7669 6475 616c 5f70 6c61 6e65  individual_plane
+00008f30: 7320 2b3d 2073 656c 662e 5f67 656e 6572  s += self._gener
+00008f40: 6174 655f 706c 616e 6573 280a 2020 2020  ate_planes(.    
+00008f50: 2020 2020 2020 2020 286c 5f63 782c 2073          (l_cx, s
+00008f60: 656c 662e 6765 745f 6578 7465 726e 616c  elf.get_external
+00008f70: 5f79 5f69 6e74 6572 7365 6374 696f 6e28  _y_intersection(
+00008f80: 6c5f 6378 2929 2c0a 2020 2020 2020 2020  l_cx)),.        
+00008f90: 2020 2020 2872 5f63 782c 2073 656c 662e      (r_cx, self.
+00008fa0: 6765 745f 6578 7465 726e 616c 5f79 5f69  get_external_y_i
+00008fb0: 6e74 6572 7365 6374 696f 6e28 725f 6378  ntersection(r_cx
+00008fc0: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
+00008fd0: 6e75 6d5f 6369 7263 6c65 732c 0a20 2020  num_circles,.   
+00008fe0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00008ff0: 2320 7265 7365 7420 7265 7375 6c74 730a  # reset results.
+00009000: 2020 2020 2020 2020 7365 6c66 2e5f 7265          self._re
+00009010: 7365 745f 7265 7375 6c74 7328 290a 0a20  set_results().. 
+00009020: 2020 2064 6566 2061 6464 5f73 696e 676c     def add_singl
+00009030: 655f 6369 7263 756c 6172 5f70 6c61 6e65  e_circular_plane
+00009040: 2873 656c 662c 2063 5f78 2c20 635f 792c  (self, c_x, c_y,
+00009050: 2072 6164 6975 7329 3a0a 2020 2020 2020   radius):.      
+00009060: 2020 2222 2241 6464 2066 6169 6c75 7265    """Add failure
+00009070: 2070 6c61 6e65 2074 6f20 6265 2061 6e61   plane to be ana
+00009080: 6c79 7365 6420 6279 2073 7065 6369 6679  lysed by specify
+00009090: 696e 6720 6369 7263 6c65 2070 726f 7065  ing circle prope
+000090a0: 7274 6965 732e 0a0a 2020 2020 2020 2020  rties...        
+000090b0: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+000090c0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+000090d0: 2020 2020 2020 635f 7820 3a20 666c 6f61        c_x : floa
+000090e0: 742c 0a20 2020 2020 2020 2020 2020 2063  t,.            c
+000090f0: 656e 7472 6520 6f66 2063 6972 636c 6520  entre of circle 
+00009100: 7820 636f 6f72 6469 6e61 7465 2e0a 2020  x coordinate..  
+00009110: 2020 2020 2020 635f 7920 3a20 666c 6f61        c_y : floa
+00009120: 742c 0a20 2020 2020 2020 2020 2020 2063  t,.            c
+00009130: 656e 7472 6520 6f66 2063 6972 636c 6520  entre of circle 
+00009140: 7920 636f 6f72 6469 6e61 7465 2e0a 2020  y coordinate..  
+00009150: 2020 2020 2020 7261 6469 7573 203a 2066        radius : f
+00009160: 6c6f 6174 0a20 2020 2020 2020 2020 2020  loat.           
+00009170: 2072 6164 6975 7320 6f66 2063 6972 636c   radius of circl
+00009180: 650a 2020 2020 2020 2020 2222 220a 2020  e.        """.  
+00009190: 2020 2020 2020 695f 6c69 7374 203d 2073        i_list = s
+000091a0: 656c 662e 5f67 6574 5f63 6972 636c 655f  elf._get_circle_
+000091b0: 6578 7465 726e 616c 5f69 6e74 6572 7365  external_interse
+000091c0: 6374 696f 6e28 635f 782c 2063 5f79 2c20  ction(c_x, c_y, 
+000091d0: 7261 6469 7573 290a 2020 2020 2020 2020  radius).        
+000091e0: 6966 206c 656e 2873 6574 2869 5f6c 6973  if len(set(i_lis
+000091f0: 7429 2920 3c20 323a 0a20 2020 2020 2020  t)) < 2:.       
+00009200: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+00009210: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00009220: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00009230: 5f69 6e64 6976 6964 7561 6c5f 706c 616e  _individual_plan
+00009240: 6573 202b 3d20 5b0a 2020 2020 2020 2020  es += [.        
+00009250: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+00009260: 2020 2020 2020 2020 2020 2020 2020 226c                "l
+00009270: 5f63 223a 2069 5f6c 6973 745b 305d 2c0a  _c": i_list[0],.
+00009280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009290: 2020 2020 2272 5f63 223a 2069 5f6c 6973      "r_c": i_lis
+000092a0: 745b 315d 2c0a 2020 2020 2020 2020 2020  t[1],.          
+000092b0: 2020 2020 2020 2020 2020 2263 5f78 223a            "c_x":
+000092c0: 2063 5f78 2c0a 2020 2020 2020 2020 2020   c_x,.          
+000092d0: 2020 2020 2020 2020 2020 2263 5f79 223a            "c_y":
+000092e0: 2063 5f79 2c0a 2020 2020 2020 2020 2020   c_y,.          
+000092f0: 2020 2020 2020 2020 2020 2272 6164 6975            "radiu
+00009300: 7322 3a20 7261 6469 7573 2c0a 2020 2020  s": radius,.    
+00009310: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00009320: 2020 2020 2020 2020 2020 5d0a 0a20 2020            ]..   
+00009330: 2020 2020 2023 2072 6573 6574 2072 6573       # reset res
+00009340: 756c 7473 0a20 2020 2020 2020 2073 656c  ults.        sel
+00009350: 662e 5f72 6573 6574 5f72 6573 756c 7473  f._reset_results
+00009360: 2829 0a0a 2020 2020 6465 6620 7265 6d6f  ()..    def remo
+00009370: 7665 5f69 6e64 6976 6964 7561 6c5f 706c  ve_individual_pl
+00009380: 616e 6573 2873 656c 6629 3a0a 2020 2020  anes(self):.    
+00009390: 2020 2020 2222 2252 656d 6f76 6520 696e      """Remove in
+000093a0: 6469 7669 6475 616c 6c79 2061 6464 6564  dividually added
+000093b0: 2066 6169 6c75 7265 2070 6c61 6e65 732e   failure planes.
+000093c0: 2222 220a 2020 2020 2020 2020 7365 6c66  """.        self
+000093d0: 2e5f 696e 6469 7669 6475 616c 5f70 6c61  ._individual_pla
+000093e0: 6e65 7320 3d20 5b5d 0a0a 2020 2020 2020  nes = []..      
+000093f0: 2020 2320 7265 7365 7420 7265 7375 6c74    # reset result
+00009400: 730a 2020 2020 2020 2020 7365 6c66 2e5f  s.        self._
+00009410: 7265 7365 745f 7265 7375 6c74 7328 290a  reset_results().
+00009420: 0a20 2020 2064 6566 2061 6e61 6c79 7365  .    def analyse
+00009430: 5f73 6c6f 7065 2873 656c 662c 206d 6178  _slope(self, max
+00009440: 5f66 6f73 3d4e 6f6e 6529 3a0a 2020 2020  _fos=None):.    
+00009450: 2020 2020 2222 2241 6e61 6c79 7365 206d      """Analyse m
+00009460: 616e 7920 706f 7373 6962 6c65 2066 6169  any possible fai
+00009470: 6c75 7265 2070 6c61 6e65 7320 666f 7220  lure planes for 
+00009480: 6120 736c 6f70 6520 4f52 0a20 2020 2020  a slope OR.     
+00009490: 2020 2069 6e64 6976 7561 6c6c 7920 6164     indivually ad
+000094a0: 6465 6420 6661 696c 7572 6520 706c 616e  ded failure plan
+000094b0: 6573 2069 6620 6164 6465 6420 746f 2073  es if added to s
+000094c0: 6c6f 7065 2e22 2222 0a0a 2020 2020 2020  lope."""..      
+000094d0: 2020 2320 6966 2069 6e64 6976 6964 7561    # if individua
+000094e0: 6c20 6661 696c 7572 6520 706c 616e 6573  l failure planes
+000094f0: 2073 6574 206f 6e6c 7920 616e 616c 7973   set only analys
+00009500: 6520 7468 656d 0a20 2020 2020 2020 2069  e them.        i
+00009510: 6620 7365 6c66 2e5f 696e 6469 7669 6475  f self._individu
+00009520: 616c 5f70 6c61 6e65 7320 213d 205b 5d3a  al_planes != []:
+00009530: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00009540: 662e 5f73 6561 7263 6820 3d20 7365 6c66  f._search = self
+00009550: 2e5f 696e 6469 7669 6475 616c 5f70 6c61  ._individual_pla
+00009560: 6e65 730a 0a20 2020 2020 2020 2023 206f  nes..        # o
+00009570: 7468 6572 7769 7365 2067 656e 6572 6174  therwise generat
+00009580: 6520 706c 616e 6573 2061 6372 6f73 7320  e planes across 
+00009590: 7468 6520 656e 7469 7265 2073 6c6f 7065  the entire slope
+000095a0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+000095b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000095c0: 5f73 6574 5f65 6e74 7279 5f65 7869 745f  _set_entry_exit_
+000095d0: 706c 616e 6573 2829 0a0a 2020 2020 2020  planes()..      
+000095e0: 2020 2320 676f 2074 6872 6f75 6768 2065    # go through e
+000095f0: 6163 6820 6173 7375 6d65 6420 706c 616e  ach assumed plan
+00009600: 6520 616e 6420 6361 6c63 756c 6174 6520  e and calculate 
+00009610: 7468 6520 464f 530a 2020 2020 2020 2020  the FOS.        
+00009620: 2320 6966 206e 6f74 206d 7563 6820 746f  # if not much to
+00009630: 2064 6f20 7468 656e 2064 6f6e 7420 7573   do then dont us
+00009640: 6520 6d75 6c74 6970 726f 6365 7373 696e  e multiprocessin
+00009650: 672c 206f 7468 6572 7769 7365 2075 7365  g, otherwise use
+00009660: 206d 756c 7469 7072 6f63 6573 7369 6e67   multiprocessing
+00009670: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00009680: 2e5f 736c 6963 6573 202a 2073 656c 662e  ._slices * self.
+00009690: 5f69 7465 7261 7469 6f6e 7320 3c20 3235  _iterations < 25
+000096a0: 3030 303a 0a20 2020 2020 2020 2020 2020  000:.           
+000096b0: 2066 6f72 2069 2c20 7365 6172 6368 2069   for i, search i
+000096c0: 6e20 656e 756d 6572 6174 6528 7471 646d  n enumerate(tqdm
+000096d0: 2873 656c 662e 5f73 6561 7263 6829 293a  (self._search)):
+000096e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000096f0: 2073 656c 662e 5f73 6561 7263 685b 695d   self._search[i]
+00009700: 5b22 464f 5322 5d20 3d20 7365 6c66 2e5f  ["FOS"] = self._
+00009710: 616e 616c 7973 655f 6369 7263 756c 6172  analyse_circular
+00009720: 5f66 6169 6c75 7265 5f62 6973 686f 7028  _failure_bishop(
+00009730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009740: 2020 2020 2063 5f78 3d73 6561 7263 685b       c_x=search[
+00009750: 2263 5f78 225d 2c0a 2020 2020 2020 2020  "c_x"],.        
+00009760: 2020 2020 2020 2020 2020 2020 635f 793d              c_y=
+00009770: 7365 6172 6368 5b22 635f 7922 5d2c 0a20  search["c_y"],. 
+00009780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009790: 2020 2072 6164 6975 733d 7365 6172 6368     radius=search
+000097a0: 5b22 7261 6469 7573 225d 2c0a 2020 2020  ["radius"],.    
+000097b0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+000097c0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+000097d0: 2020 2020 2020 2020 2320 7573 6520 6d75          # use mu
+000097e0: 6c74 6970 726f 6365 7373 696e 6720 746f  ltiprocessing to
+000097f0: 2067 6574 2072 6573 756c 7473 0a20 2020   get results.   
+00009800: 2020 2020 2020 2020 2077 6974 6820 6d75           with mu
+00009810: 6c74 6970 726f 6365 7373 696e 672e 4d61  ltiprocessing.Ma
+00009820: 6e61 6765 7228 2920 6173 206d 616e 6167  nager() as manag
+00009830: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
+00009840: 2020 2020 7769 7468 206d 616e 6167 6572      with manager
+00009850: 2e50 6f6f 6c28 2920 6173 2070 6f6f 6c3a  .Pool() as pool:
+00009860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009870: 2020 2020 2072 6573 756c 7473 203d 2070       results = p
+00009880: 6f6f 6c2e 7374 6172 6d61 7028 0a20 2020  ool.starmap(.   
+00009890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000098a0: 2020 2020 2073 656c 662e 5f61 6e61 6c79       self._analy
+000098b0: 7365 5f63 6972 6375 6c61 725f 6661 696c  se_circular_fail
+000098c0: 7572 655f 6269 7368 6f70 2c0a 2020 2020  ure_bishop,.    
+000098d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000098e0: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
+000098f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009900: 2020 280a 2020 2020 2020 2020 2020 2020    (.            
+00009910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009920: 2020 2020 7365 6172 6368 5b22 635f 7822      search["c_x"
+00009930: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00009940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009950: 2020 2073 6561 7263 685b 2263 5f79 225d     search["c_y"]
+00009960: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00009970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009980: 2020 7365 6172 6368 5b22 7261 6469 7573    search["radius
+00009990: 225d 2c0a 2020 2020 2020 2020 2020 2020  "],.            
+000099a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000099b0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000099c0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+000099d0: 7220 7365 6172 6368 2069 6e20 7365 6c66  r search in self
+000099e0: 2e5f 7365 6172 6368 0a20 2020 2020 2020  ._search.       
+000099f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a00: 205d 2c0a 2020 2020 2020 2020 2020 2020   ],.            
+00009a10: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00009a20: 2020 2020 2020 2023 2061 6464 2072 6573         # add res
+00009a30: 756c 7473 2074 6f20 6469 6374 696f 6e61  ults to dictiona
+00009a40: 7279 0a20 2020 2020 2020 2020 2020 2066  ry.            f
+00009a50: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
+00009a60: 6e28 7365 6c66 2e5f 7365 6172 6368 2929  n(self._search))
+00009a70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00009a80: 2020 7365 6c66 2e5f 7365 6172 6368 5b69    self._search[i
+00009a90: 5d5b 2246 4f53 225d 203d 2072 6573 756c  ]["FOS"] = resul
+00009aa0: 7473 5b69 5d0a 0a20 2020 2020 2020 2023  ts[i]..        #
+00009ab0: 2074 6964 7920 7468 6520 696e 666f 726d   tidy the inform
+00009ac0: 6174 696f 6e20 746f 2072 656d 6f76 6520  ation to remove 
+00009ad0: 616e 7974 6869 6e67 2074 6861 7420 6469  anything that di
+00009ae0: 646e 7420 7275 6e20 616e 640a 2020 2020  dnt run and.    
+00009af0: 2020 2020 2320 746f 2062 6520 736f 7274      # to be sort
+00009b00: 6564 2066 726f 6d20 6c6f 7765 7374 2046  ed from lowest F
+00009b10: 4f53 2074 6f20 6869 6768 6573 7420 464f  OS to highest FO
+00009b20: 530a 2020 2020 2020 2020 7365 6172 6368  S.        search
+00009b30: 203d 206c 6973 7428 6669 6c74 6572 2828   = list(filter((
+00009b40: 6c61 6d62 6461 2078 3a20 785b 2246 4f53  lambda x: x["FOS
+00009b50: 225d 2069 7320 6e6f 7420 4e6f 6e65 292c  "] is not None),
+00009b60: 2073 656c 662e 5f73 6561 7263 6829 290a   self._search)).
+00009b70: 2020 2020 2020 2020 7365 6172 6368 2e73          search.s
+00009b80: 6f72 7428 6b65 793d 6c61 6d62 6461 2078  ort(key=lambda x
+00009b90: 3a20 785b 2246 4f53 225d 290a 2020 2020  : x["FOS"]).    
+00009ba0: 2020 2020 6966 206d 6178 5f66 6f73 3a0a      if max_fos:.
+00009bb0: 2020 2020 2020 2020 2020 2020 7365 6172              sear
+00009bc0: 6368 203d 206c 6973 7428 6669 6c74 6572  ch = list(filter
+00009bd0: 286c 616d 6264 6120 783a 2028 785b 2246  (lambda x: (x["F
+00009be0: 4f53 225d 203c 3d20 6d61 785f 666f 7329  OS"] <= max_fos)
+00009bf0: 2c20 7365 6172 6368 2929 0a0a 2020 2020  , search))..    
+00009c00: 2020 2020 7365 6c66 2e5f 7365 6172 6368      self._search
+00009c10: 203d 2073 6561 7263 680a 0a20 2020 2064   = search..    d
+00009c20: 6566 205f 616e 616c 7973 655f 6369 7263  ef _analyse_circ
+00009c30: 756c 6172 5f66 6169 6c75 7265 5f6f 7264  ular_failure_ord
+00009c40: 696e 6172 7928 0a20 2020 2020 2020 2073  inary(.        s
+00009c50: 656c 662c 2063 5f78 3a20 666c 6f61 742c  elf, c_x: float,
+00009c60: 2063 5f79 3a20 666c 6f61 742c 2072 6164   c_y: float, rad
+00009c70: 6975 733a 2066 6c6f 6174 2c20 6c5f 633d  ius: float, l_c=
+00009c80: 4e6f 6e65 2c20 725f 633d 4e6f 6e65 0a20  None, r_c=None. 
+00009c90: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
+00009ca0: 2243 616c 6375 6c61 7465 2066 6163 746f  "Calculate facto
+00009cb0: 7220 6f66 2073 6166 6574 7920 666f 7220  r of safety for 
+00009cc0: 6120 6369 7263 756c 6172 2066 6169 6c75  a circular failu
+00009cd0: 7265 2070 6c61 6e65 2074 6872 6f75 6768  re plane through
+00009ce0: 2074 6865 2073 6c6f 7065 0a20 2020 2020   the slope.     
+00009cf0: 2020 2075 7369 6e67 2074 6865 206f 7264     using the ord
+00009d00: 696e 6172 7920 6d65 7468 6f64 2028 7377  inary method (sw
+00009d10: 6564 6973 6820 6d65 7468 6f64 206f 6620  edish method of 
+00009d20: 736c 6963 6573 292e 0a0a 2020 2020 2020  slices)...      
+00009d30: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+00009d40: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
+00009d50: 2020 2020 2020 2020 635f 7820 3a20 666c          c_x : fl
+00009d60: 6f61 740a 2020 2020 2020 2020 2020 2020  oat.            
+00009d70: 6369 7263 6c65 2063 656e 7465 7220 7820  circle center x 
+00009d80: 636f 6f72 6469 6e61 7465 0a20 2020 2020  coordinate.     
+00009d90: 2020 2063 5f79 203a 2066 6c6f 6174 0a20     c_y : float. 
+00009da0: 2020 2020 2020 2020 2020 2063 6972 636c             circl
+00009db0: 6520 6365 6e74 6572 2079 2063 6f6f 7264  e center y coord
+00009dc0: 696e 6174 650a 2020 2020 2020 2020 7261  inate.        ra
+00009dd0: 6469 7573 203a 2066 6c6f 6174 0a20 2020  dius : float.   
+00009de0: 2020 2020 2020 2020 2063 6972 636c 6520           circle 
+00009df0: 7261 6469 7573 0a20 2020 2020 2020 206c  radius.        l
+00009e00: 5f63 203a 2074 7570 6c65 2c20 6f70 7469  _c : tuple, opti
+00009e10: 6f6e 616c 0a20 2020 2020 2020 2020 2020  onal.           
+00009e20: 2063 6f6f 7264 696e 6174 6573 206f 6620   coordinates of 
+00009e30: 6c65 6674 2069 6e74 6572 7365 6374 696f  left intersectio
+00009e40: 6e20 6265 7477 6565 6e20 626f 756e 6461  n between bounda
+00009e50: 7279 2061 6e64 0a20 2020 2020 2020 2020  ry and.         
+00009e60: 2020 2066 6169 6c75 7265 2070 6c61 6e65     failure plane
+00009e70: 2069 6620 616c 7265 6164 7920 6b6e 6f77   if already know
+00009e80: 6e2c 2062 7920 6465 6661 756c 7420 4e6f  n, by default No
+00009e90: 6e65 2e0a 2020 2020 2020 2020 725f 6320  ne..        r_c 
+00009ea0: 3a20 7475 706c 652c 206f 7074 696f 6e61  : tuple, optiona
+00009eb0: 6c0a 2020 2020 2020 2020 2020 2020 636f  l.            co
+00009ec0: 6f72 6469 6e61 7465 7320 6f66 206c 6566  ordinates of lef
+00009ed0: 7420 696e 7465 7273 6563 7469 6f6e 2062  t intersection b
+00009ee0: 6574 7765 656e 2062 6f75 6e64 6172 7920  etween boundary 
+00009ef0: 616e 640a 2020 2020 2020 2020 2020 2020  and.            
+00009f00: 6661 696c 7572 6520 706c 616e 6520 6966  failure plane if
+00009f10: 2061 6c72 6561 6479 206b 6e6f 776e 2c20   already known, 
+00009f20: 6279 2064 6566 6175 6c74 204e 6f6e 652e  by default None.
+00009f30: 0a0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00009f40: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
+00009f50: 2d2d 0a20 2020 2020 2020 2066 6c6f 6174  --.        float
+00009f60: 0a20 2020 2020 2020 2020 2020 2066 6163  .            fac
+00009f70: 746f 7220 6f66 2073 6166 6574 790a 2020  tor of safety.  
+00009f80: 2020 2020 2020 4e6f 6e65 0a20 2020 2020        None.     
+00009f90: 2020 2020 2020 2069 6620 6361 6e74 2063         if cant c
+00009fa0: 616c 6375 6c61 7465 2072 6574 7572 6e73  alculate returns
+00009fb0: 204e 6f6e 650a 0a20 2020 2020 2020 2022   None..        "
+00009fc0: 2222 0a20 2020 2020 2020 2023 2064 6174  "".        # dat
+00009fd0: 6120 7661 6c69 6461 7469 6f6e 0a20 2020  a validation.   
+00009fe0: 2020 2020 2064 6174 615f 7661 6c69 6461       data_valida
+00009ff0: 7469 6f6e 2e61 7373 6572 745f 7374 7269  tion.assert_stri
+0000a000: 6374 6c79 5f70 6f73 6974 6976 655f 6e75  ctly_positive_nu
+0000a010: 6d62 6572 280a 2020 2020 2020 2020 2020  mber(.          
+0000a020: 2020 635f 782c 2022 635f 7820 2863 6972    c_x, "c_x (cir
+0000a030: 636c 6520 7820 636f 6f72 6469 6e61 7465  cle x coordinate
+0000a040: 2922 0a20 2020 2020 2020 2029 0a20 2020  )".        ).   
+0000a050: 2020 2020 2064 6174 615f 7661 6c69 6461       data_valida
+0000a060: 7469 6f6e 2e61 7373 6572 745f 7374 7269  tion.assert_stri
+0000a070: 6374 6c79 5f70 6f73 6974 6976 655f 6e75  ctly_positive_nu
+0000a080: 6d62 6572 280a 2020 2020 2020 2020 2020  mber(.          
+0000a090: 2020 635f 792c 2022 635f 7920 2863 6972    c_y, "c_y (cir
+0000a0a0: 636c 6520 7920 636f 6f72 6469 6e61 7465  cle y coordinate
+0000a0b0: 2922 0a20 2020 2020 2020 2029 0a20 2020  )".        ).   
+0000a0c0: 2020 2020 2064 6174 615f 7661 6c69 6461       data_valida
+0000a0d0: 7469 6f6e 2e61 7373 6572 745f 7374 7269  tion.assert_stri
+0000a0e0: 6374 6c79 5f70 6f73 6974 6976 655f 6e75  ctly_positive_nu
+0000a0f0: 6d62 6572 2872 6164 6975 732c 2022 7261  mber(radius, "ra
+0000a100: 6469 7573 2229 0a0a 2020 2020 2020 2020  dius")..        
+0000a110: 2320 6966 206c 5f63 2061 6e64 2072 5f63  # if l_c and r_c
+0000a120: 206e 6f74 2073 6574 2074 6865 6e20 7573   not set then us
+0000a130: 6572 2069 7320 7072 6f62 6162 6c79 2063  er is probably c
+0000a140: 6865 636b 696e 6720 616e 2069 6e64 6976  hecking an indiv
+0000a150: 6964 7561 6c20 6369 7263 756c 6172 2070  idual circular p
+0000a160: 6c61 6e65 0a20 2020 2020 2020 2023 2063  lane.        # c
+0000a170: 616e 2067 6574 2074 6865 2072 6967 6874  an get the right
+0000a180: 2061 6e64 206c 6566 7420 636f 6f72 6469   and left coordi
+0000a190: 6e61 7465 2069 6e74 6572 7365 6374 696f  nate intersectio
+0000a1a0: 6e20 7769 7468 2074 6865 206d 6f64 656c  n with the model
+0000a1b0: 2066 6f72 2074 6869 7320 6361 7365 2e0a   for this case..
+0000a1c0: 2020 2020 2020 2020 6966 206c 5f63 2069          if l_c i
+0000a1d0: 7320 4e6f 6e65 206f 7220 725f 6320 6973  s None or r_c is
+0000a1e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000a1f0: 2020 2069 5f6c 6973 7420 3d20 7365 6c66     i_list = self
+0000a200: 2e5f 6765 745f 6369 7263 6c65 5f65 7874  ._get_circle_ext
+0000a210: 6572 6e61 6c5f 696e 7465 7273 6563 7469  ernal_intersecti
+0000a220: 6f6e 2863 5f78 2c20 635f 792c 2072 6164  on(c_x, c_y, rad
+0000a230: 6975 7329 0a20 2020 2020 2020 2020 2020  ius).           
+0000a240: 2069 6620 6c65 6e28 7365 7428 695f 6c69   if len(set(i_li
+0000a250: 7374 2929 2021 3d20 323a 0a20 2020 2020  st)) != 2:.     
+0000a260: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000a270: 6e20 4e6f 6e65 0a20 2020 2020 2020 2065  n None.        e
+0000a280: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000a290: 2069 5f6c 6973 7420 3d20 5b6c 5f63 2c20   i_list = [l_c, 
+0000a2a0: 725f 635d 0a0a 2020 2020 2020 2020 2320  r_c]..        # 
+0000a2b0: 746f 7461 6c20 6e75 6d62 6572 206f 6620  total number of 
+0000a2c0: 736c 6963 6573 0a20 2020 2020 2020 2053  slices.        S
+0000a2d0: 4c49 4345 5320 3d20 7365 6c66 2e5f 736c  LICES = self._sl
+0000a2e0: 6963 6573 0a0a 2020 2020 2020 2020 2320  ices..        # 
+0000a2f0: 686f 7269 7a6f 6e74 616c 2064 6973 7461  horizontal dista
+0000a300: 6e63 6520 6265 7477 6565 6e20 6c65 6674  nce between left
+0000a310: 2061 6e64 2072 6967 6874 2073 6c69 6365   and right slice
+0000a320: 0a20 2020 2020 2020 2064 6973 7420 3d20  .        dist = 
+0000a330: 695f 6c69 7374 5b31 5d5b 305d 202d 2069  i_list[1][0] - i
+0000a340: 5f6c 6973 745b 305d 5b30 5d0a 0a20 2020  _list[0][0]..   
+0000a350: 2020 2020 2023 2077 6964 7468 206f 6620       # width of 
+0000a360: 6120 736c 6963 650a 2020 2020 2020 2020  a slice.        
+0000a370: 6220 3d20 6469 7374 202f 2053 4c49 4345  b = dist / SLICE
+0000a380: 530a 0a20 2020 2020 2020 2069 6620 6220  S..        if b 
+0000a390: 3c3d 2030 2e30 3030 3030 313a 0a20 2020  <= 0.000001:.   
+0000a3a0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000a3b0: 4e6f 6e65 0a0a 2020 2020 2020 2020 2320  None..        # 
+0000a3c0: 696e 6974 6961 6c69 7365 2063 656e 7472  initialise centr
+0000a3d0: 6520 706f 696e 7420 6f66 2066 6972 7374  e point of first
+0000a3e0: 2073 6c69 6365 0a20 2020 2020 2020 2073   slice.        s
+0000a3f0: 5f78 203d 2069 5f6c 6973 745b 305d 5b30  _x = i_list[0][0
+0000a400: 5d20 2b20 6220 2f20 320a 0a20 2020 2020  ] + b / 2..     
+0000a410: 2020 2023 2069 6e74 6961 6c69 7365 2074     # intialise t
+0000a420: 6865 2070 7573 6820 616e 6420 7265 7369  he push and resi
+0000a430: 7374 616e 6365 2063 6f6d 706f 6e65 6e74  stance component
+0000a440: 7320 666f 7220 464f 5320 6265 666f 7265  s for FOS before
+0000a450: 206c 6f6f 7069 6e67 0a20 2020 2020 2020   looping.       
+0000a460: 2070 7573 6869 6e67 203d 2030 2e30 0a20   pushing = 0.0. 
+0000a470: 2020 2020 2020 2072 6573 6973 7469 6e67         resisting
+0000a480: 203d 2030 2e30 0a0a 2020 2020 2020 2020   = 0.0..        
+0000a490: 2320 6c6f 6f70 2074 6872 6f75 6768 2073  # loop through s
+0000a4a0: 6c69 6365 730a 2020 2020 2020 2020 666f  lices.        fo
+0000a4b0: 7220 5f20 696e 2072 616e 6765 2830 2c20  r _ in range(0, 
+0000a4c0: 534c 4943 4553 293a 0a20 2020 2020 2020  SLICES):.       
+0000a4d0: 2020 2020 2023 2064 6566 696e 6520 7920       # define y 
+0000a4e0: 636f 6f72 6469 6e61 7465 7320 666f 7220  coordinates for 
+0000a4f0: 736c 6963 6520 626f 7474 6f6d 0a20 2020  slice bottom.   
+0000a500: 2020 2020 2020 2020 2023 2048 4153 2045           # HAS E
+0000a510: 5252 4f52 0a20 2020 2020 2020 2020 2020  RROR.           
+0000a520: 2023 2028 6379 202d 2073 5f79 6229 202a   # (cy - s_yb) *
+0000a530: 2a20 3220 2b20 6162 7328 735f 782d 635f  * 2 + abs(s_x-c_
+0000a540: 7829 2a2a 3220 3d20 5220 2a2a 2032 0a20  x)**2 = R ** 2. 
+0000a550: 2020 2020 2020 2020 2020 2023 2073 7172             # sqr
+0000a560: 7428 522a 2a32 202d 2061 6273 2873 5f78  t(R**2 - abs(s_x
+0000a570: 2d63 5f78 292a 2a32 2920 3d20 635f 7920  -c_x)**2) = c_y 
+0000a580: 2d20 735f 7962 0a20 2020 2020 2020 2020  - s_yb.         
+0000a590: 2020 2073 5f79 6220 3d20 635f 7920 2d20     s_yb = c_y - 
+0000a5a0: 7371 7274 2872 6164 6975 732a 2a32 202d  sqrt(radius**2 -
+0000a5b0: 2061 6273 2873 5f78 202d 2063 5f78 2920   abs(s_x - c_x) 
+0000a5c0: 2a2a 2032 290a 0a20 2020 2020 2020 2020  ** 2)..         
+0000a5d0: 2020 2023 2067 6574 2079 2063 6f6f 7264     # get y coord
+0000a5e0: 696e 6174 6520 6174 2073 6c69 6365 2074  inate at slice t
+0000a5f0: 6f70 0a20 2020 2020 2020 2020 2020 2073  op.            s
+0000a600: 5f79 7420 3d20 7365 6c66 2e67 6574 5f65  _yt = self.get_e
+0000a610: 7874 6572 6e61 6c5f 795f 696e 7465 7273  xternal_y_inters
+0000a620: 6563 7469 6f6e 2873 5f78 290a 0a20 2020  ection(s_x)..   
+0000a630: 2020 2020 2020 2020 2023 206f 7574 206f           # out o
+0000a640: 6620 626f 756e 6473 0a20 2020 2020 2020  f bounds.       
+0000a650: 2020 2020 2069 6620 735f 7974 2069 7320       if s_yt is 
+0000a660: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000a670: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
+0000a680: 650a 0a20 2020 2020 2020 2020 2020 2069  e..            i
+0000a690: 6620 735f 7974 203c 2073 5f79 623a 0a20  f s_yt < s_yb:. 
+0000a6a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000a6b0: 5f79 7420 3d20 735f 7962 0a0a 2020 2020  _yt = s_yb..    
+0000a6c0: 2020 2020 2020 2020 2320 6765 7420 616c          # get al
+0000a6d0: 7068 612c 2064 7920 616c 7761 7973 2070  pha, dy always p
+0000a6e0: 6f73 6974 6976 652c 2064 7820 6e65 6761  ositive, dx nega
+0000a6f0: 7469 7665 2074 6f20 7269 6768 7420 2875  tive to right (u
+0000a700: 7068 696c 6c29 2c20 6478 2070 6f73 6974  phill), dx posit
+0000a710: 6976 6520 746f 206c 6566 740a 2020 2020  ive to left.    
+0000a720: 2020 2020 2020 2020 2320 6e6f 7465 2061          # note a
+0000a730: 6c70 6861 2069 6e20 7261 6469 616e 7320  lpha in radians 
+0000a740: 6279 2064 6566 6175 6c74 0a20 2020 2020  by default.     
+0000a750: 2020 2020 2020 2064 7920 3d20 635f 7920         dy = c_y 
+0000a760: 2d20 735f 7962 0a20 2020 2020 2020 2020  - s_yb.         
+0000a770: 2020 2064 7820 3d20 635f 7820 2d20 735f     dx = c_x - s_
+0000a780: 780a 2020 2020 2020 2020 2020 2020 616c  x.            al
+0000a790: 7068 6120 3d20 6174 616e 2864 7820 2f20  pha = atan(dx / 
+0000a7a0: 6479 290a 0a20 2020 2020 2020 2020 2020  dy)..           
+0000a7b0: 2023 2067 6574 206c 656e 6774 680a 2020   # get length.  
+0000a7c0: 2020 2020 2020 2020 2020 696e 636c 696e            inclin
+0000a7d0: 6564 5f6c 656e 6774 6820 3d20 6220 2f20  ed_length = b / 
+0000a7e0: 636f 7328 616c 7068 6129 0a0a 2020 2020  cos(alpha)..    
+0000a7f0: 2020 2020 2020 2020 2320 6361 6c63 756c          # calcul
+0000a800: 6174 6520 7374 7269 7020 7765 6967 6874  ate strip weight
+0000a810: 0a20 2020 2020 2020 2020 2020 2057 203d  .            W =
+0000a820: 2073 656c 662e 5f63 616c 6375 6c61 7465   self._calculate
+0000a830: 5f73 7472 6970 5f77 6569 6768 7428 622c  _strip_weight(b,
+0000a840: 2073 5f79 742c 2073 5f79 6229 0a0a 2020   s_yt, s_yb)..  
+0000a850: 2020 2020 2020 2020 2020 2320 6765 7420            # get 
+0000a860: 6d61 7465 7269 616c 2070 726f 7065 7274  material propert
+0000a870: 6965 7320 6174 2074 6865 2062 6f74 746f  ies at the botto
+0000a880: 6d20 6f66 2074 6865 2073 6c69 6365 0a20  m of the slice. 
+0000a890: 2020 2020 2020 2020 2020 2062 6f74 746f             botto
+0000a8a0: 6d5f 6d61 7465 7269 616c 203d 2073 656c  m_material = sel
+0000a8b0: 662e 5f67 6574 5f6d 6174 6572 6961 6c5f  f._get_material_
+0000a8c0: 6174 5f64 6570 7468 2873 5f79 6229 0a0a  at_depth(s_yb)..
+0000a8d0: 2020 2020 2020 2020 2020 2020 636f 6865              cohe
+0000a8e0: 7369 6f6e 203d 2062 6f74 746f 6d5f 6d61  sion = bottom_ma
+0000a8f0: 7465 7269 616c 2e63 6f68 6573 696f 6e0a  terial.cohesion.
+0000a900: 2020 2020 2020 2020 2020 2020 6672 6963              fric
+0000a910: 7469 6f6e 5f61 6e67 6c65 203d 2062 6f74  tion_angle = bot
+0000a920: 746f 6d5f 6d61 7465 7269 616c 2e66 7269  tom_material.fri
+0000a930: 6374 696f 6e5f 616e 676c 650a 0a20 2020  ction_angle..   
+0000a940: 2020 2020 2020 2020 2023 2069 6620 7468           # if th
+0000a950: 6572 6520 6973 2061 2075 646c 206c 6f61  ere is a udl loa
+0000a960: 6420 6f6e 2074 6865 2073 7472 6970 2061  d on the strip a
+0000a970: 7070 6c79 2069 742e 0a20 2020 2020 2020  pply it..       
+0000a980: 2020 2020 2066 6f72 2075 646c 2069 6e20       for udl in 
+0000a990: 7365 6c66 2e5f 7564 6c73 3a0a 2020 2020  self._udls:.    
+0000a9a0: 2020 2020 2020 2020 2020 2020 5720 2b3d              W +=
+0000a9b0: 2073 656c 662e 5f63 616c 6375 6c61 7465   self._calculate
+0000a9c0: 5f73 7472 6970 5f75 646c 5f66 6f72 6365  _strip_udl_force
+0000a9d0: 2862 2c20 735f 782c 2075 646c 290a 0a20  (b, s_x, udl).. 
+0000a9e0: 2020 2020 2020 2020 2020 2023 2069 6620             # if 
+0000a9f0: 7468 6572 6520 6973 2061 2070 6f69 6e74  there is a point
+0000aa00: 206c 6f61 6420 6f6e 2074 6865 2073 7472   load on the str
+0000aa10: 6970 2061 7070 6c79 2069 742e 0a20 2020  ip apply it..   
+0000aa20: 2020 2020 2020 2020 2066 6f72 206c 6c20           for ll 
+0000aa30: 696e 2073 656c 662e 5f6c 6c73 3a0a 2020  in self._lls:.  
+0000aa40: 2020 2020 2020 2020 2020 2020 2020 5720                W 
+0000aa50: 2b3d 2073 656c 662e 5f63 616c 6375 6c61  += self._calcula
+0000aa60: 7465 5f73 7472 6970 5f6c 6c28 622c 2073  te_strip_ll(b, s
+0000aa70: 5f78 2c20 6c6c 290a 0a20 2020 2020 2020  _x, ll)..       
+0000aa80: 2020 2020 2023 2063 6f6e 7369 6465 7261       # considera
+0000aa90: 7469 6f6e 2066 6f72 2077 6174 6572 0a20  tion for water. 
+0000aaa0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000aab0: 6c66 2e5f 7761 7465 725f 524c 3a0a 2020  lf._water_RL:.  
+0000aac0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000aad0: 6465 7465 726d 696e 6520 4820 6661 6374  determine H fact
+0000aae0: 6f72 2062 6173 6564 206f 6e20 7365 7474  or based on sett
+0000aaf0: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
+0000ab00: 2020 2020 2320 6874 7470 733a 2f2f 7777      # https://ww
+0000ab10: 772e 726f 6373 6369 656e 6365 2e63 6f6d  w.rocscience.com
+0000ab20: 2f68 656c 702f 736c 6964 6532 2f64 6f63  /help/slide2/doc
+0000ab30: 756d 656e 7461 7469 6f6e 2f73 6c69 6465  umentation/slide
+0000ab40: 2d6d 6f64 656c 2f6d 6174 6572 6961 6c2d  -model/material-
+0000ab50: 7072 6f70 6572 7469 6573 2f64 6566 696e  properties/defin
+0000ab60: 652d 6d61 7465 7269 616c 2d70 726f 7065  e-material-prope
+0000ab70: 7274 6965 732f 7761 7465 722d 7061 7261  rties/water-para
+0000ab80: 6d65 7465 7273 0a0a 2020 2020 2020 2020  meters..        
+0000ab90: 2020 2020 2020 2020 2320 6f6e 6c79 2075          # only u
+0000aba0: 7365 2048 2066 6163 746f 7220 6966 2077  se H factor if w
+0000abb0: 6174 6572 2073 6c6f 7069 6e67 0a20 2020  ater sloping.   
+0000abc0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000abd0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000abe0: 2020 2020 2020 7365 6c66 2e67 6574 5f65        self.get_e
+0000abf0: 7874 6572 6e61 6c5f 785f 696e 7465 7273  xternal_x_inters
+0000ac00: 6563 7469 6f6e 2873 656c 662e 5f77 6174  ection(self._wat
+0000ac10: 6572 5f52 4c29 0a20 2020 2020 2020 2020  er_RL).         
+0000ac20: 2020 2020 2020 2020 2020 203c 2073 5f78             < s_x
+0000ac30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ac40: 2020 2020 203c 2073 656c 662e 5f62 6f74       < self._bot
+0000ac50: 5f63 6f6f 7264 5b30 5d0a 2020 2020 2020  _coord[0].      
+0000ac60: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
+0000ac70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac80: 2055 203d 2028 0a20 2020 2020 2020 2020   U = (.         
+0000ac90: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0000aca0: 6178 286d 696e 2873 656c 662e 5f77 6174  ax(min(self._wat
+0000acb0: 6572 5f52 4c2c 2073 5f79 7429 202d 2073  er_RL, s_yt) - s
+0000acc0: 5f79 622c 2030 290a 2020 2020 2020 2020  _yb, 0).        
+0000acd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ace0: 2a20 392e 3831 0a20 2020 2020 2020 2020  * 9.81.         
+0000acf0: 2020 2020 2020 2020 2020 2020 2020 202a                 *
+0000ad00: 2069 6e63 6c69 6e65 645f 6c65 6e67 7468   inclined_length
+0000ad10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ad20: 2020 2020 2020 2020 202a 2073 656c 662e           * self.
+0000ad30: 5f77 6174 6572 5f61 6e61 6c79 7369 735f  _water_analysis_
+0000ad40: 480a 2020 2020 2020 2020 2020 2020 2020  H.              
+0000ad50: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000ad60: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000ad70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad80: 2020 5520 3d20 280a 2020 2020 2020 2020    U = (.        
+0000ad90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ada0: 6d61 7828 6d69 6e28 7365 6c66 2e5f 7761  max(min(self._wa
+0000adb0: 7465 725f 524c 2c20 735f 7974 2920 2d20  ter_RL, s_yt) - 
+0000adc0: 735f 7962 2c20 3029 0a20 2020 2020 2020  s_yb, 0).       
+0000add0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ade0: 202a 2039 2e38 310a 2020 2020 2020 2020   * 9.81.        
+0000adf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae00: 2a20 696e 636c 696e 6564 5f6c 656e 6774  * inclined_lengt
+0000ae10: 680a 2020 2020 2020 2020 2020 2020 2020  h.              
+0000ae20: 2020 2020 2020 2020 2020 2a20 310a 2020            * 1.  
+0000ae30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae40: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0000ae50: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000ae60: 2020 2020 2020 5520 3d20 300a 0a20 2020        U = 0..   
+0000ae70: 2020 2020 2020 2020 2023 2063 616c 6375           # calcu
+0000ae80: 6c61 7465 2072 6573 6973 7469 6e67 0a20  late resisting. 
+0000ae90: 2020 2020 2020 2020 2020 2072 6573 6973             resis
+0000aea0: 7469 6e67 202b 3d20 636f 6865 7369 6f6e  ting += cohesion
+0000aeb0: 202a 2069 6e63 6c69 6e65 645f 6c65 6e67   * inclined_leng
+0000aec0: 7468 202b 206d 6178 280a 2020 2020 2020  th + max(.      
+0000aed0: 2020 2020 2020 2020 2020 302c 2028 5720            0, (W 
+0000aee0: 2a20 636f 7328 616c 7068 6129 202d 2055  * cos(alpha) - U
+0000aef0: 290a 2020 2020 2020 2020 2020 2020 2920  ).            ) 
+0000af00: 2a20 7461 6e28 7261 6469 616e 7328 6672  * tan(radians(fr
+0000af10: 6963 7469 6f6e 5f61 6e67 6c65 2929 0a0a  iction_angle))..
+0000af20: 2020 2020 2020 2020 2020 2020 2320 6361              # ca
+0000af30: 6c63 756c 6174 6520 7075 7368 696e 670a  lculate pushing.
+0000af40: 2020 2020 2020 2020 2020 2020 7075 7368              push
+0000af50: 696e 6720 2b3d 2057 202a 2073 696e 2861  ing += W * sin(a
+0000af60: 6c70 6861 290a 0a20 2020 2020 2020 2020  lpha)..         
+0000af70: 2020 2023 2069 6e69 7469 616c 6973 6520     # initialise 
+0000af80: 736c 6963 6520 7820 636f 6f72 6469 6e61  slice x coordina
+0000af90: 7465 2066 6f72 206e 6578 7420 6c6f 6f70  te for next loop
+0000afa0: 0a20 2020 2020 2020 2020 2020 2073 5f78  .            s_x
+0000afb0: 203d 2073 5f78 202b 2062 0a0a 2020 2020   = s_x + b..    
+0000afc0: 2020 2020 6966 2070 7573 6869 6e67 203c      if pushing <
+0000afd0: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
+0000afe0: 2072 6574 7572 6e20 4e6f 6e65 0a0a 2020   return None..  
+0000aff0: 2020 2020 2020 464f 5320 3d20 7265 7369        FOS = resi
+0000b000: 7374 696e 6720 2f20 7075 7368 696e 670a  sting / pushing.
+0000b010: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000b020: 464f 530a 0a20 2020 2023 2062 6973 686f  FOS..    # bisho
+0000b030: 700a 0a20 2020 2064 6566 205f 616e 616c  p..    def _anal
+0000b040: 7973 655f 6369 7263 756c 6172 5f66 6169  yse_circular_fai
+0000b050: 6c75 7265 5f62 6973 686f 7028 0a20 2020  lure_bishop(.   
+0000b060: 2020 2020 2073 656c 662c 2063 5f78 3a20       self, c_x: 
+0000b070: 666c 6f61 742c 2063 5f79 3a20 666c 6f61  float, c_y: floa
+0000b080: 742c 2072 6164 6975 733a 2066 6c6f 6174  t, radius: float
+0000b090: 2c20 6c5f 633d 4e6f 6e65 2c20 725f 633d  , l_c=None, r_c=
+0000b0a0: 4e6f 6e65 0a20 2020 2029 3a0a 2020 2020  None.    ):.    
+0000b0b0: 2020 2020 2222 2243 616c 6375 6c61 7465      """Calculate
+0000b0c0: 2066 6163 746f 7220 6f66 2073 6166 6574   factor of safet
+0000b0d0: 7920 666f 7220 6120 6369 7263 756c 6172  y for a circular
+0000b0e0: 2066 6169 6c75 7265 2070 6c61 6e65 2074   failure plane t
+0000b0f0: 6872 6f75 6768 2074 6865 2073 6c6f 7065  hrough the slope
+0000b100: 0a20 2020 2020 2020 2075 7369 6e67 2062  .        using b
+0000b110: 6973 686f 7073 206d 6574 686f 642e 0a0a  ishops method...
+0000b120: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+0000b130: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
+0000b140: 2d2d 2d2d 2d0a 2020 2020 2020 2020 635f  -----.        c_
+0000b150: 7820 3a20 666c 6f61 740a 2020 2020 2020  x : float.      
+0000b160: 2020 2020 2020 6369 7263 6c65 2063 656e        circle cen
+0000b170: 7465 7220 7820 636f 6f72 6469 6e61 7465  ter x coordinate
+0000b180: 0a20 2020 2020 2020 2063 5f79 203a 2066  .        c_y : f
+0000b190: 6c6f 6174 0a20 2020 2020 2020 2020 2020  loat.           
+0000b1a0: 2063 6972 636c 6520 6365 6e74 6572 2079   circle center y
+0000b1b0: 2063 6f6f 7264 696e 6174 650a 2020 2020   coordinate.    
+0000b1c0: 2020 2020 7261 6469 7573 203a 2066 6c6f      radius : flo
+0000b1d0: 6174 0a20 2020 2020 2020 2020 2020 2063  at.            c
+0000b1e0: 6972 636c 6520 7261 6469 7573 0a20 2020  ircle radius.   
+0000b1f0: 2020 2020 206c 5f63 203a 2074 7570 6c65       l_c : tuple
+0000b200: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+0000b210: 2020 2020 2020 2063 6f6f 7264 696e 6174         coordinat
+0000b220: 6573 206f 6620 6c65 6674 2069 6e74 6572  es of left inter
+0000b230: 7365 6374 696f 6e20 6265 7477 6565 6e20  section between 
+0000b240: 626f 756e 6461 7279 2061 6e64 0a20 2020  boundary and.   
+0000b250: 2020 2020 2020 2020 2066 6169 6c75 7265           failure
+0000b260: 2070 6c61 6e65 2069 6620 616c 7265 6164   plane if alread
+0000b270: 7920 6b6e 6f77 6e2c 2062 7920 6465 6661  y known, by defa
+0000b280: 756c 7420 4e6f 6e65 2e0a 2020 2020 2020  ult None..      
+0000b290: 2020 725f 6320 3a20 7475 706c 652c 206f    r_c : tuple, o
+0000b2a0: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+0000b2b0: 2020 2020 636f 6f72 6469 6e61 7465 7320      coordinates 
+0000b2c0: 6f66 206c 6566 7420 696e 7465 7273 6563  of left intersec
+0000b2d0: 7469 6f6e 2062 6574 7765 656e 2062 6f75  tion between bou
+0000b2e0: 6e64 6172 7920 616e 640a 2020 2020 2020  ndary and.      
+0000b2f0: 2020 2020 2020 6661 696c 7572 6520 706c        failure pl
+0000b300: 616e 6520 6966 2061 6c72 6561 6479 206b  ane if already k
+0000b310: 6e6f 776e 2c20 6279 2064 6566 6175 6c74  nown, by default
+0000b320: 204e 6f6e 652e 0a0a 0a20 2020 2020 2020   None....       
+0000b330: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
+0000b340: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
+0000b350: 2066 6c6f 6174 0a20 2020 2020 2020 2020   float.         
+0000b360: 2020 2066 6163 746f 7220 6f66 2073 6166     factor of saf
+0000b370: 6574 790a 2020 2020 2020 2020 4e6f 6e65  ety.        None
+0000b380: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000b390: 6361 6e74 2063 616c 6375 6c61 7465 2072  cant calculate r
+0000b3a0: 6574 7572 6e73 204e 6f6e 650a 0a20 2020  eturns None..   
+0000b3b0: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+0000b3c0: 2020 2320 6966 206c 5f63 2061 6e64 2072    # if l_c and r
+0000b3d0: 5f63 206e 6f74 2073 6574 2074 6865 6e20  _c not set then 
+0000b3e0: 7573 6572 2069 7320 7072 6f62 6162 6c79  user is probably
+0000b3f0: 2063 6865 636b 696e 6720 616e 2069 6e64   checking an ind
+0000b400: 6976 6964 7561 6c20 6369 7263 756c 6172  ividual circular
+0000b410: 2070 6c61 6e65 0a20 2020 2020 2020 2023   plane.        #
+0000b420: 2063 616e 2067 6574 2074 6865 2072 6967   can get the rig
+0000b430: 6874 2061 6e64 206c 6566 7420 636f 6f72  ht and left coor
+0000b440: 6469 6e61 7465 2069 6e74 6572 7365 6374  dinate intersect
+0000b450: 696f 6e20 7769 7468 2074 6865 206d 6f64  ion with the mod
+0000b460: 656c 2066 6f72 2074 6869 7320 6361 7365  el for this case
+0000b470: 2e0a 2020 2020 2020 2020 6966 206c 5f63  ..        if l_c
+0000b480: 2069 7320 4e6f 6e65 206f 7220 725f 6320   is None or r_c 
+0000b490: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+0000b4a0: 2020 2020 2069 5f6c 6973 7420 3d20 7365       i_list = se
+0000b4b0: 6c66 2e5f 6765 745f 6369 7263 6c65 5f65  lf._get_circle_e
+0000b4c0: 7874 6572 6e61 6c5f 696e 7465 7273 6563  xternal_intersec
+0000b4d0: 7469 6f6e 2863 5f78 2c20 635f 792c 2072  tion(c_x, c_y, r
+0000b4e0: 6164 6975 7329 0a20 2020 2020 2020 2020  adius).         
+0000b4f0: 2020 2069 6620 6c65 6e28 7365 7428 695f     if len(set(i_
+0000b500: 6c69 7374 2929 203c 2032 3a0a 2020 2020  list)) < 2:.    
+0000b510: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000b520: 726e 204e 6f6e 650a 2020 2020 2020 2020  rn None.        
+0000b530: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000b540: 2020 2020 2020 2020 2020 6c5f 632c 2072            l_c, r
+0000b550: 5f63 203d 2069 5f6c 6973 745b 305d 2c20  _c = i_list[0], 
+0000b560: 695f 6c69 7374 5b31 5d0a 2020 2020 2020  i_list[1].      
+0000b570: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000b580: 2020 2020 695f 6c69 7374 203d 205b 6c5f      i_list = [l_
+0000b590: 632c 2072 5f63 5d0a 0a20 2020 2020 2020  c, r_c]..       
+0000b5a0: 2046 5320 3d20 7365 6c66 2e5f 616e 616c   FS = self._anal
+0000b5b0: 7973 655f 6369 7263 756c 6172 5f66 6169  yse_circular_fai
+0000b5c0: 6c75 7265 5f6f 7264 696e 6172 7928 635f  lure_ordinary(c_
+0000b5d0: 782c 2063 5f79 2c20 7261 6469 7573 2c20  x, c_y, radius, 
+0000b5e0: 6c5f 632c 2072 5f63 290a 0a20 2020 2020  l_c, r_c)..     
+0000b5f0: 2020 2069 6620 4653 2069 7320 4e6f 6e65     if FS is None
+0000b600: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0000b610: 7475 726e 204e 6f6e 650a 0a20 2020 2020  turn None..     
+0000b620: 2020 2070 7265 765f 4653 203d 2046 530a     prev_FS = FS.
+0000b630: 0a20 2020 2020 2020 2023 2074 6f74 616c  .        # total
+0000b640: 206e 756d 6265 7220 6f66 2073 6c69 6365   number of slice
+0000b650: 730a 2020 2020 2020 2020 534c 4943 4553  s.        SLICES
+0000b660: 203d 2073 656c 662e 5f73 6c69 6365 730a   = self._slices.
+0000b670: 0a20 2020 2020 2020 2023 2068 6f72 697a  .        # horiz
+0000b680: 6f6e 7461 6c20 6469 7374 616e 6365 2062  ontal distance b
+0000b690: 6574 7765 656e 206c 6566 7420 616e 6420  etween left and 
+0000b6a0: 7269 6768 7420 736c 6963 650a 2020 2020  right slice.    
+0000b6b0: 2020 2020 6469 7374 203d 2069 5f6c 6973      dist = i_lis
+0000b6c0: 745b 315d 5b30 5d20 2d20 695f 6c69 7374  t[1][0] - i_list
+0000b6d0: 5b30 5d5b 305d 0a0a 2020 2020 2020 2020  [0][0]..        
+0000b6e0: 2320 7769 6474 6820 6f66 2061 2073 6c69  # width of a sli
+0000b6f0: 6365 0a20 2020 2020 2020 2062 203d 2064  ce.        b = d
+0000b700: 6973 7420 2f20 534c 4943 4553 0a0a 2020  ist / SLICES..  
+0000b710: 2020 2020 2020 666f 7220 5f20 696e 2072        for _ in r
+0000b720: 616e 6765 2873 656c 662e 5f6d 6178 5f69  ange(self._max_i
+0000b730: 7465 7261 7469 6f6e 7329 3a0a 2020 2020  terations):.    
+0000b740: 2020 2020 2020 2020 2320 696e 6974 6961          # initia
+0000b750: 6c69 7365 2063 656e 7472 6520 706f 696e  lise centre poin
+0000b760: 7420 6f66 2066 6972 7374 2073 6c69 6365  t of first slice
+0000b770: 0a20 2020 2020 2020 2020 2020 2073 5f78  .            s_x
+0000b780: 203d 2069 5f6c 6973 745b 305d 5b30 5d20   = i_list[0][0] 
+0000b790: 2b20 6220 2f20 320a 0a20 2020 2020 2020  + b / 2..       
+0000b7a0: 2020 2020 2069 6620 7072 6576 5f46 5320       if prev_FS 
+0000b7b0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+0000b7c0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000b7d0: 4e6f 6e65 0a0a 2020 2020 2020 2020 2020  None..          
+0000b7e0: 2020 2320 696e 7469 616c 6973 6520 7468    # intialise th
+0000b7f0: 6520 7075 7368 2061 6e64 2072 6573 6973  e push and resis
+0000b800: 7461 6e63 6520 636f 6d70 6f6e 656e 7473  tance components
+0000b810: 2066 6f72 2046 4f53 2062 6566 6f72 6520   for FOS before 
+0000b820: 6c6f 6f70 696e 670a 2020 2020 2020 2020  looping.        
+0000b830: 2020 2020 7075 7368 696e 6720 3d20 302e      pushing = 0.
+0000b840: 300a 2020 2020 2020 2020 2020 2020 7265  0.            re
+0000b850: 7369 7374 696e 6720 3d20 302e 300a 0a20  sisting = 0.0.. 
+0000b860: 2020 2020 2020 2020 2020 2023 206c 6f6f             # loo
+0000b870: 7020 7468 726f 7567 6820 736c 6963 6573  p through slices
+0000b880: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0000b890: 205f 2069 6e20 7261 6e67 6528 302c 2053   _ in range(0, S
+0000b8a0: 4c49 4345 5329 3a0a 2020 2020 2020 2020  LICES):.        
+0000b8b0: 2020 2020 2020 2020 2320 6465 6669 6e65          # define
+0000b8c0: 2079 2063 6f6f 7264 696e 6174 6573 2066   y coordinates f
+0000b8d0: 6f72 2073 6c69 6365 2062 6f74 746f 6d0a  or slice bottom.
+0000b8e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b8f0: 2023 2069 6620 7261 6469 7573 203c 2061   # if radius < a
+0000b900: 6273 2873 5f78 202d 2063 5f78 293a 0a20  bs(s_x - c_x):. 
+0000b910: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000b920: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+0000b930: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000b940: 2020 735f 7962 203d 2063 5f79 202d 2073    s_yb = c_y - s
+0000b950: 7172 7428 7261 6469 7573 2a2a 3220 2d20  qrt(radius**2 - 
+0000b960: 6162 7328 735f 7820 2d20 635f 7829 202a  abs(s_x - c_x) *
+0000b970: 2a20 3229 0a0a 2020 2020 2020 2020 2020  * 2)..          
+0000b980: 2020 2020 2020 2320 6765 7420 7920 636f        # get y co
+0000b990: 6f72 6469 6e61 7465 2061 7420 736c 6963  ordinate at slic
+0000b9a0: 6520 746f 700a 2020 2020 2020 2020 2020  e top.          
+0000b9b0: 2020 2020 2020 735f 7974 203d 2073 656c        s_yt = sel
+0000b9c0: 662e 6765 745f 6578 7465 726e 616c 5f79  f.get_external_y
+0000b9d0: 5f69 6e74 6572 7365 6374 696f 6e28 735f  _intersection(s_
+0000b9e0: 7829 0a0a 2020 2020 2020 2020 2020 2020  x)..            
+0000b9f0: 2020 2020 2320 6f75 7420 6f66 2062 6f75      # out of bou
+0000ba00: 6e64 730a 2020 2020 2020 2020 2020 2020  nds.            
+0000ba10: 2020 2020 6966 2073 5f79 7420 6973 204e      if s_yt is N
+0000ba20: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000ba30: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000ba40: 4e6f 6e65 0a0a 2020 2020 2020 2020 2020  None..          
+0000ba50: 2020 2020 2020 2320 6765 7420 616c 7068        # get alph
+0000ba60: 612c 2064 7920 616c 7761 7973 2070 6f73  a, dy always pos
+0000ba70: 6974 6976 652c 2064 7820 6e65 6761 7469  itive, dx negati
+0000ba80: 7665 2074 6f20 7269 6768 7420 2875 7068  ve to right (uph
+0000ba90: 696c 6c29 2c20 6478 2070 6f73 6974 6976  ill), dx positiv
+0000baa0: 6520 746f 206c 6566 740a 2020 2020 2020  e to left.      
+0000bab0: 2020 2020 2020 2020 2020 2320 6e6f 7465            # note
+0000bac0: 2061 6c70 6861 2069 6e20 7261 6469 616e   alpha in radian
+0000bad0: 7320 6279 2064 6566 6175 6c74 0a20 2020  s by default.   
+0000bae0: 2020 2020 2020 2020 2020 2020 2064 7920               dy 
+0000baf0: 3d20 635f 7920 2d20 735f 7962 0a20 2020  = c_y - s_yb.   
+0000bb00: 2020 2020 2020 2020 2020 2020 2064 7820               dx 
+0000bb10: 3d20 635f 7820 2d20 735f 780a 2020 2020  = c_x - s_x.    
+0000bb20: 2020 2020 2020 2020 2020 2020 616c 7068              alph
+0000bb30: 6120 3d20 6174 616e 2864 7820 2f20 6479  a = atan(dx / dy
+0000bb40: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000bb50: 2020 2023 2067 6574 206c 656e 6774 680a     # get length.
+0000bb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb70: 2320 6c20 3d20 6220 2f20 636f 7328 616c  # l = b / cos(al
+0000bb80: 7068 6129 0a0a 2020 2020 2020 2020 2020  pha)..          
+0000bb90: 2020 2020 2020 2320 6361 6c63 756c 6174        # calculat
+0000bba0: 6520 7374 7269 7020 7765 6967 6874 0a20  e strip weight. 
+0000bbb0: 2020 2020 2020 2020 2020 2020 2020 2057                 W
+0000bbc0: 203d 2073 656c 662e 5f63 616c 6375 6c61   = self._calcula
+0000bbd0: 7465 5f73 7472 6970 5f77 6569 6768 7428  te_strip_weight(
+0000bbe0: 622c 2073 5f79 742c 2073 5f79 6229 0a0a  b, s_yt, s_yb)..
+0000bbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc00: 2320 6765 7420 6d61 7465 7269 616c 2070  # get material p
+0000bc10: 726f 7065 7274 6965 7320 6174 2074 6865  roperties at the
+0000bc20: 2062 6f74 746f 6d20 6f66 2074 6865 2073   bottom of the s
+0000bc30: 6c69 6365 0a20 2020 2020 2020 2020 2020  lice.           
+0000bc40: 2020 2020 2062 6f74 746f 6d5f 6d61 7465       bottom_mate
+0000bc50: 7269 616c 203d 2073 656c 662e 5f67 6574  rial = self._get
+0000bc60: 5f6d 6174 6572 6961 6c5f 6174 5f64 6570  _material_at_dep
+0000bc70: 7468 2873 5f79 6229 0a0a 2020 2020 2020  th(s_yb)..      
+0000bc80: 2020 2020 2020 2020 2020 636f 6865 7369            cohesi
+0000bc90: 6f6e 203d 2062 6f74 746f 6d5f 6d61 7465  on = bottom_mate
+0000bca0: 7269 616c 2e63 6f68 6573 696f 6e0a 2020  rial.cohesion.  
+0000bcb0: 2020 2020 2020 2020 2020 2020 2020 6672                fr
+0000bcc0: 6963 7469 6f6e 5f61 6e67 6c65 203d 2062  iction_angle = b
+0000bcd0: 6f74 746f 6d5f 6d61 7465 7269 616c 2e66  ottom_material.f
+0000bce0: 7269 6374 696f 6e5f 616e 676c 650a 0a20  riction_angle.. 
+0000bcf0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000bd00: 2041 4343 4f52 4449 4e47 2054 4f20 4745   ACCORDING TO GE
+0000bd10: 4f53 4c4f 5045 2053 484f 554c 4420 444f  OSLOPE SHOULD DO
+0000bd20: 2054 4845 2043 4845 434b 2042 454c 4f57   THE CHECK BELOW
+0000bd30: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000bd40: 2020 2320 5448 4953 2048 4f57 4556 4552    # THIS HOWEVER
+0000bd50: 2045 4c49 4d49 4e41 5445 5320 414c 4d4f   ELIMINATES ALMO
+0000bd60: 5354 2041 4c4c 204f 4620 5448 4520 5052  ST ALL OF THE PR
+0000bd70: 4f50 4f53 4544 2053 4c4f 5045 530a 2020  OPOSED SLOPES.  
+0000bd80: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000bd90: 534c 4944 4520 444f 4553 4e54 2043 4f4e  SLIDE DOESNT CON
+0000bda0: 5349 4445 5220 5448 4953 2e0a 0a20 2020  SIDER THIS...   
+0000bdb0: 2020 2020 2020 2020 2020 2020 2023 2069               # i
+0000bdc0: 6620 5f20 3d3d 2030 3a0a 2020 2020 2020  f _ == 0:.      
+0000bdd0: 2020 2020 2020 2020 2020 2320 2020 2020            #     
+0000bde0: 6966 2061 6c70 6861 202a 2031 3830 202f  if alpha * 180 /
+0000bdf0: 2033 2e31 3420 3e20 3435 202b 2066 7269   3.14 > 45 + fri
+0000be00: 6374 696f 6e5f 616e 676c 6520 2f20 323a  ction_angle / 2:
+0000be10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000be20: 2023 2020 2020 2020 2020 2072 6574 7572   #         retur
+0000be30: 6e20 4e6f 6e65 0a0a 2020 2020 2020 2020  n None..        
+0000be40: 2020 2020 2020 2020 2320 6966 205f 203d          # if _ =
+0000be50: 3d20 534c 4943 4553 202d 2031 3a0a 2020  = SLICES - 1:.  
+0000be60: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000be70: 2020 2020 6966 2061 6c70 6861 202a 2031      if alpha * 1
+0000be80: 3830 202f 2033 2e31 3420 3c20 3435 202d  80 / 3.14 < 45 -
+0000be90: 2066 7269 6374 696f 6e5f 616e 676c 652f   friction_angle/
+0000bea0: 323a 0a20 2020 2020 2020 2020 2020 2020  2:.             
+0000beb0: 2020 2023 2020 2020 2020 2020 2072 6574     #         ret
+0000bec0: 7572 6e20 4e6f 6e65 0a0a 2020 2020 2020  urn None..      
+0000bed0: 2020 2020 2020 2020 2020 2320 6966 2074            # if t
+0000bee0: 6865 7265 2069 7320 6120 7564 6c20 6c6f  here is a udl lo
+0000bef0: 6164 206f 6e20 7468 6520 7374 7269 7020  ad on the strip 
+0000bf00: 6170 706c 7920 6974 2e0a 2020 2020 2020  apply it..      
+0000bf10: 2020 2020 2020 2020 2020 666f 7220 7564            for ud
+0000bf20: 6c20 696e 2073 656c 662e 5f75 646c 733a  l in self._udls:
+0000bf30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bf40: 2020 2020 2057 202b 3d20 7365 6c66 2e5f       W += self._
+0000bf50: 6361 6c63 756c 6174 655f 7374 7269 705f  calculate_strip_
+0000bf60: 7564 6c5f 666f 7263 6528 622c 2073 5f78  udl_force(b, s_x
+0000bf70: 2c20 7564 6c29 0a0a 2020 2020 2020 2020  , udl)..        
+0000bf80: 2020 2020 2020 2020 2320 6966 2074 6865          # if the
+0000bf90: 7265 2069 7320 6120 706f 696e 7420 6c6f  re is a point lo
+0000bfa0: 6164 206f 6e20 7468 6520 7374 7269 7020  ad on the strip 
+0000bfb0: 6170 706c 7920 6974 2e0a 2020 2020 2020  apply it..      
+0000bfc0: 2020 2020 2020 2020 2020 666f 7220 6c6c            for ll
+0000bfd0: 2069 6e20 7365 6c66 2e5f 6c6c 733a 0a20   in self._lls:. 
+0000bfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bff0: 2020 2057 202b 3d20 7365 6c66 2e5f 6361     W += self._ca
+0000c000: 6c63 756c 6174 655f 7374 7269 705f 6c6c  lculate_strip_ll
+0000c010: 2862 2c20 735f 782c 206c 6c29 0a0a 2020  (b, s_x, ll)..  
+0000c020: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000c030: 636f 6e73 6964 6572 6174 696f 6e20 666f  consideration fo
+0000c040: 7220 7761 7465 720a 2020 2020 2020 2020  r water.        
+0000c050: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000c060: 5f77 6174 6572 5f52 4c3a 0a20 2020 2020  _water_RL:.     
+0000c070: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000c080: 2064 6574 6572 6d69 6e65 2048 2066 6163   determine H fac
+0000c090: 746f 7220 6261 7365 6420 6f6e 2073 6574  tor based on set
+0000c0a0: 7469 6e67 0a20 2020 2020 2020 2020 2020  ting.           
+0000c0b0: 2020 2020 2020 2020 2023 2068 7474 7073           # https
+0000c0c0: 3a2f 2f77 7777 2e72 6f63 7363 6965 6e63  ://www.rocscienc
+0000c0d0: 652e 636f 6d2f 6865 6c70 2f73 6c69 6465  e.com/help/slide
+0000c0e0: 322f 646f 6375 6d65 6e74 6174 696f 6e2f  2/documentation/
+0000c0f0: 736c 6964 652d 6d6f 6465 6c2f 6d61 7465  slide-model/mate
+0000c100: 7269 616c 2d70 726f 7065 7274 6965 732f  rial-properties/
+0000c110: 6465 6669 6e65 2d6d 6174 6572 6961 6c2d  define-material-
+0000c120: 7072 6f70 6572 7469 6573 2f77 6174 6572  properties/water
+0000c130: 2d70 6172 616d 6574 6572 730a 0a20 2020  -parameters..   
+0000c140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c150: 2023 206f 6e6c 7920 7573 6520 4820 6661   # only use H fa
+0000c160: 6374 6f72 2069 6620 6f6e 2074 6865 2073  ctor if on the s
+0000c170: 6c6f 7065 2c20 6f74 6865 7277 6973 6520  lope, otherwise 
+0000c180: 7573 6520 310a 2020 2020 2020 2020 2020  use 1.          
+0000c190: 2020 2020 2020 2020 2020 6966 2028 0a20            if (. 
+0000c1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c1b0: 2020 2020 2020 2073 656c 662e 6765 745f         self.get_
+0000c1c0: 6578 7465 726e 616c 5f78 5f69 6e74 6572  external_x_inter
+0000c1d0: 7365 6374 696f 6e28 7365 6c66 2e5f 7761  section(self._wa
+0000c1e0: 7465 725f 524c 290a 2020 2020 2020 2020  ter_RL).        
+0000c1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c200: 3c20 735f 780a 2020 2020 2020 2020 2020  < s_x.          
+0000c210: 2020 2020 2020 2020 2020 2020 2020 3c20                < 
+0000c220: 7365 6c66 2e5f 626f 745f 636f 6f72 645b  self._bot_coord[
+0000c230: 305d 0a20 2020 2020 2020 2020 2020 2020  0].             
+0000c240: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
+0000c250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c260: 2020 5520 3d20 280a 2020 2020 2020 2020    U = (.        
+0000c270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c280: 2020 2020 6d61 7828 6d69 6e28 7365 6c66      max(min(self
+0000c290: 2e5f 7761 7465 725f 524c 2c20 735f 7974  ._water_RL, s_yt
+0000c2a0: 2920 2d20 735f 7962 2c20 3029 0a20 2020  ) - s_yb, 0).   
+0000c2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c2c0: 2020 2020 2020 2020 202a 2039 2e38 310a           * 9.81.
+0000c2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c2e0: 2020 2020 2020 2020 2020 2020 2a20 620a              * b.
+0000c2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c300: 2020 2020 2020 2020 2020 2020 2a20 7365              * se
+0000c310: 6c66 2e5f 7761 7465 725f 616e 616c 7973  lf._water_analys
+0000c320: 6973 5f48 0a20 2020 2020 2020 2020 2020  is_H.           
+0000c330: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+0000c340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c350: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000c360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c370: 2055 203d 206d 6178 286d 696e 2873 656c   U = max(min(sel
+0000c380: 662e 5f77 6174 6572 5f52 4c2c 2073 5f79  f._water_RL, s_y
+0000c390: 7429 202d 2073 5f79 622c 2030 2920 2a20  t) - s_yb, 0) * 
+0000c3a0: 392e 3831 202a 2062 202a 2031 0a20 2020  9.81 * b * 1.   
+0000c3b0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+0000c3c0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000c3d0: 2020 2020 2020 2055 203d 2030 0a0a 2020         U = 0..  
+0000c3e0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000c3f0: 6361 6c63 756c 6174 6520 6d61 0a20 2020  calculate ma.   
+0000c400: 2020 2020 2020 2020 2020 2020 206d 6120               ma 
+0000c410: 3d20 636f 7328 616c 7068 6129 202b 2073  = cos(alpha) + s
+0000c420: 696e 2861 6c70 6861 2920 2a20 7461 6e28  in(alpha) * tan(
+0000c430: 7261 6469 616e 7328 6672 6963 7469 6f6e  radians(friction
+0000c440: 5f61 6e67 6c65 2929 202f 2070 7265 765f  _angle)) / prev_
+0000c450: 4653 0a0a 2020 2020 2020 2020 2020 2020  FS..            
+0000c460: 2020 2020 2320 6361 6c63 756c 6174 6520      # calculate 
+0000c470: 7265 7369 7374 696e 670a 2020 2020 2020  resisting.      
+0000c480: 2020 2020 2020 2020 2020 7265 7369 7374            resist
+0000c490: 696e 6720 2b3d 2028 0a20 2020 2020 2020  ing += (.       
+0000c4a0: 2020 2020 2020 2020 2020 2020 2063 6f68               coh
+0000c4b0: 6573 696f 6e20 2a20 6220 2b20 2857 202d  esion * b + (W -
+0000c4c0: 2055 2920 2a20 7461 6e28 7261 6469 616e   U) * tan(radian
+0000c4d0: 7328 6672 6963 7469 6f6e 5f61 6e67 6c65  s(friction_angle
+0000c4e0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+0000c4f0: 2020 2029 202f 206d 610a 0a20 2020 2020     ) / ma..     
+0000c500: 2020 2020 2020 2020 2020 2023 2063 616c             # cal
+0000c510: 6375 6c61 7465 2070 7573 6869 6e67 0a20  culate pushing. 
+0000c520: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000c530: 7573 6869 6e67 202b 3d20 5720 2a20 7369  ushing += W * si
+0000c540: 6e28 616c 7068 6129 0a0a 2020 2020 2020  n(alpha)..      
+0000c550: 2020 2020 2020 2020 2020 2320 696e 6974            # init
+0000c560: 6961 6c69 7365 2073 6c69 6365 2078 2063  ialise slice x c
+0000c570: 6f6f 7264 696e 6174 6520 666f 7220 6e65  oordinate for ne
+0000c580: 7874 206c 6f6f 700a 2020 2020 2020 2020  xt loop.        
+0000c590: 2020 2020 2020 2020 735f 7820 3d20 735f          s_x = s_
+0000c5a0: 7820 2b20 620a 0a20 2020 2020 2020 2020  x + b..         
+0000c5b0: 2020 2069 6620 7075 7368 696e 6720 3c3d     if pushing <=
+0000c5c0: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+0000c5d0: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
+0000c5e0: 2020 2020 2020 2020 2020 2020 6966 2072              if r
+0000c5f0: 6573 6973 7469 6e67 203c 2030 206f 7220  esisting < 0 or 
+0000c600: 7075 7368 696e 6720 3c20 303a 0a20 2020  pushing < 0:.   
+0000c610: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+0000c620: 7572 6e20 4e6f 6e65 0a0a 2020 2020 2020  urn None..      
+0000c630: 2020 2020 2020 4653 203d 2072 6573 6973        FS = resis
+0000c640: 7469 6e67 202f 2070 7573 6869 6e67 0a20  ting / pushing. 
+0000c650: 2020 2020 2020 2020 2020 2069 6620 6162             if ab
+0000c660: 7328 7072 6576 5f46 5320 2d20 4653 2920  s(prev_FS - FS) 
+0000c670: 3c20 7365 6c66 2e5f 746f 6c65 7261 6e63  < self._toleranc
+0000c680: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000c690: 2020 2072 6574 7572 6e20 4653 0a20 2020     return FS.   
+0000c6a0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0000c6b0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000c6c0: 7265 765f 4653 203d 2046 530a 0a20 2020  rev_FS = FS..   
+0000c6d0: 2020 2020 2072 6574 7572 6e20 7072 6576       return prev
+0000c6e0: 5f46 530a 0a20 2020 2064 6566 2061 6e61  _FS..    def ana
+0000c6f0: 6c79 7365 5f64 796e 616d 6963 2873 656c  lyse_dynamic(sel
+0000c700: 662c 2063 7269 7469 6361 6c5f 666f 733d  f, critical_fos=
+0000c710: 312e 3329 3a0a 2020 2020 2020 2020 2222  1.3):.        ""
+0000c720: 2241 6e61 6c79 7365 2073 6c6f 7065 2061  "Analyse slope a
+0000c730: 6e64 206f 6666 7365 7420 6479 6e61 6d69  nd offset dynami
+0000c740: 6320 6c6f 6164 7320 756e 7469 6c20 6372  c loads until cr
+0000c750: 6974 6963 616c 2046 4f53 2069 7320 6163  itical FOS is ac
+0000c760: 6869 6576 6564 0a0a 2020 2020 2020 2020  hieved..        
+0000c770: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+0000c780: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+0000c790: 2020 2020 2020 6372 6974 6963 616c 5f66        critical_f
+0000c7a0: 6f73 203a 2066 6c6f 6174 2c20 6f70 7469  os : float, opti
+0000c7b0: 6f6e 616c 0a20 2020 2020 2020 2020 2020  onal.           
+0000c7c0: 206d 696e 696d 756d 2072 6571 7569 7265   minimum require
+0000c7d0: 6420 6661 6374 6f72 206f 6620 7361 6665  d factor of safe
+0000c7e0: 7479 2c20 6279 2064 6566 6175 6c74 2031  ty, by default 1
+0000c7f0: 2e33 0a20 2020 2020 2020 2022 2222 0a20  .3.        """. 
+0000c800: 2020 2020 2020 2073 656c 662e 5f64 796e         self._dyn
+0000c810: 616d 6963 5f72 6573 756c 7473 203d 207b  amic_results = {
+0000c820: 7d0a 0a20 2020 2020 2020 2023 2063 6865  }..        # che
+0000c830: 636b 2063 6173 6520 666f 7220 6c6f 6164  ck case for load
+0000c840: 2061 7420 7269 6768 7420 616e 6420 6c6f   at right and lo
+0000c850: 6164 2061 7420 6c65 6674 2062 6566 6f72  ad at left befor
+0000c860: 650a 2020 2020 2020 2020 2320 7472 7969  e.        # tryi
+0000c870: 6e67 2074 6f20 636f 6e76 6572 6765 206f  ng to converge o
+0000c880: 6e20 706f 7369 7469 6f6e 0a20 2020 2020  n position.     
+0000c890: 2020 2072 6967 6874 203d 2030 2e30 0a0a     right = 0.0..
+0000c8a0: 2020 2020 2020 2020 2320 6765 7420 7468          # get th
+0000c8b0: 6520 6c65 6e67 7468 206f 6620 7468 6520  e length of the 
+0000c8c0: 746f 7020 616e 6420 7375 6274 7261 6374  top and subtract
+0000c8d0: 2074 6865 206c 6172 6765 7374 2064 796e   the largest dyn
+0000c8e0: 616d 6963 206c 6f61 6420 6c65 6e67 7468  amic load length
+0000c8f0: 0a20 2020 2020 2020 206c 6566 7420 3d20  .        left = 
+0000c900: 7365 6c66 2e5f 6c65 6e67 7468 0a20 2020  self._length.   
+0000c910: 2020 2020 2066 6f72 2075 646c 2069 6e20       for udl in 
+0000c920: 7365 6c66 2e5f 7564 6c73 3a0a 2020 2020  self._udls:.    
+0000c930: 2020 2020 2020 2020 6966 2075 646c 2e64          if udl.d
+0000c940: 796e 616d 6963 5f6f 6666 7365 743a 0a20  ynamic_offset:. 
+0000c950: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0000c960: 6566 7420 3d20 6d61 7828 6c65 6674 2c20  eft = max(left, 
+0000c970: 7365 6c66 2e5f 746f 705f 636f 6f72 645b  self._top_coord[
+0000c980: 305d 202d 2075 646c 2e6c 656e 6774 6829  0] - udl.length)
+0000c990: 0a0a 2020 2020 2020 2020 6c65 6674 202d  ..        left -
+0000c9a0: 3d20 302e 3031 0a0a 2020 2020 2020 2020  = 0.01..        
+0000c9b0: 2320 6368 6563 6b20 666f 7220 6578 7472  # check for extr
+0000c9c0: 656d 6520 6361 7365 2077 6974 6820 6c6f  eme case with lo
+0000c9d0: 6164 7320 6174 2063 7265 7374 2028 7269  ads at crest (ri
+0000c9e0: 6768 7429 0a20 2020 2020 2020 2023 2069  ght).        # i
+0000c9f0: 6620 736c 6f70 6520 6973 2073 6166 6520  f slope is safe 
+0000ca00: 2846 4f53 2068 6967 6829 2074 6865 6e20  (FOS high) then 
+0000ca10: 7265 7475 726e 0a20 2020 2020 2020 2073  return.        s
+0000ca20: 656c 662e 5f73 6574 5f64 796e 616d 6963  elf._set_dynamic
+0000ca30: 5f6f 6666 7365 7428 7269 6768 7429 0a20  _offset(right). 
+0000ca40: 2020 2020 2020 2073 656c 662e 616e 616c         self.anal
+0000ca50: 7973 655f 736c 6f70 6528 290a 2020 2020  yse_slope().    
+0000ca60: 2020 2020 666f 7320 3d20 7365 6c66 2e67      fos = self.g
+0000ca70: 6574 5f6d 696e 5f46 4f53 2829 0a20 2020  et_min_FOS().   
+0000ca80: 2020 2020 2073 656c 662e 5f64 796e 616d       self._dynam
+0000ca90: 6963 5f72 6573 756c 7473 5b72 6967 6874  ic_results[right
+0000caa0: 5d20 3d20 666f 730a 2020 2020 2020 2020  ] = fos.        
+0000cab0: 6966 2066 6f73 203e 2063 7269 7469 6361  if fos > critica
+0000cac0: 6c5f 666f 733a 0a20 2020 2020 2020 2020  l_fos:.         
+0000cad0: 2020 2072 6574 7572 6e20 300a 0a20 2020     return 0..   
+0000cae0: 2020 2020 2023 2063 6865 636b 2066 6f72       # check for
+0000caf0: 2065 7874 7265 6d65 2063 6173 6520 7769   extreme case wi
+0000cb00: 7468 206c 6f61 6473 2061 7420 656e 6420  th loads at end 
+0000cb10: 6f66 2073 6c6f 7065 2061 7320 6661 7220  of slope as far 
+0000cb20: 6177 6179 2066 726f 6d20 6372 6573 7420  away from crest 
+0000cb30: 286c 6566 7429 0a20 2020 2020 2020 2023  (left).        #
+0000cb40: 2049 6620 736c 6f70 6520 6973 2075 6e73   If slope is uns
+0000cb50: 6166 6520 2846 4f53 2073 7469 6c6c 206c  afe (FOS still l
+0000cb60: 6f77 2920 7468 656e 2072 6574 7572 6e0a  ow) then return.
+0000cb70: 2020 2020 2020 2020 7365 6c66 2e5f 7365          self._se
+0000cb80: 745f 6479 6e61 6d69 635f 6f66 6673 6574  t_dynamic_offset
+0000cb90: 286c 6566 7429 0a20 2020 2020 2020 2073  (left).        s
+0000cba0: 656c 662e 616e 616c 7973 655f 736c 6f70  elf.analyse_slop
+0000cbb0: 6528 290a 2020 2020 2020 2020 666f 7320  e().        fos 
+0000cbc0: 3d20 7365 6c66 2e67 6574 5f6d 696e 5f46  = self.get_min_F
+0000cbd0: 4f53 2829 0a20 2020 2020 2020 2073 656c  OS().        sel
+0000cbe0: 662e 5f64 796e 616d 6963 5f72 6573 756c  f._dynamic_resul
+0000cbf0: 7473 5b6c 6566 745d 203d 2066 6f73 0a20  ts[left] = fos. 
+0000cc00: 2020 2020 2020 2069 6620 666f 7320 3c20         if fos < 
+0000cc10: 6372 6974 6963 616c 5f66 6f73 3a0a 2020  critical_fos:.  
+0000cc20: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000cc30: 2031 0a0a 2020 2020 2020 2020 2320 4966   1..        # If
+0000cc40: 206e 6569 7468 6572 206f 6620 7468 6520   neither of the 
+0000cc50: 7072 6576 696f 7573 2072 6573 756c 7473  previous results
+0000cc60: 2077 6173 2074 7275 6520 6669 6e64 2074   was true find t
+0000cc70: 6865 2069 6e74 6572 6d65 6469 6174 6520  he intermediate 
+0000cc80: 706f 696e 740a 2020 2020 2020 2020 2320  point.        # 
+0000cc90: 7768 6572 6520 7468 6520 6372 6974 6963  where the critic
+0000cca0: 616c 2046 4f53 2069 7320 7265 6163 6865  al FOS is reache
+0000ccb0: 640a 2020 2020 2020 2020 2320 6f66 6673  d.        # offs
+0000ccc0: 6574 2066 6f72 206c 6566 7420 7368 6f75  et for left shou
+0000ccd0: 6c64 6e74 2062 6520 6d6f 7265 2074 6865  ldnt be more the
+0000cce0: 6e20 7468 6520 706f 696e 7420 7468 6174  n the point that
+0000ccf0: 2074 6865 2073 6c6f 7065 2073 7461 7274   the slope start
+0000cd00: 6564 2066 6169 6c69 6e67 2066 726f 6d0a  ed failing from.
+0000cd10: 2020 2020 2020 2020 2320 696e 2074 6865          # in the
+0000cd20: 2077 6f72 7365 2063 6173 650a 2020 2020   worse case.    
+0000cd30: 2020 2020 2320 6c65 6674 203d 2073 656c      # left = sel
+0000cd40: 662e 6765 745f 6d69 6e5f 464f 535f 656e  f.get_min_FOS_en
+0000cd50: 645f 706f 696e 7473 2829 5b30 5d5b 305d  d_points()[0][0]
+0000cd60: 0a0a 2020 2020 2020 2020 7072 6576 696f  ..        previo
+0000cd70: 7573 5f66 6f73 203d 2030 0a0a 2020 2020  us_fos = 0..    
+0000cd80: 2020 2020 2320 636f 6e76 6572 6765 0a20      # converge. 
+0000cd90: 2020 2020 2020 2066 6f72 205f 2069 6e20         for _ in 
+0000cda0: 7261 6e67 6528 3130 293a 0a20 2020 2020  range(10):.     
+0000cdb0: 2020 2020 2020 2023 2023 2063 6865 636b         # # check
+0000cdc0: 206d 6964 706f 696e 7420 666f 7220 464f   midpoint for FO
+0000cdd0: 530a 2020 2020 2020 2020 2020 2020 2320  S.            # 
+0000cde0: 6d69 6470 6f69 6e74 203d 2028 6c65 6674  midpoint = (left
+0000cdf0: 202b 2072 6967 6874 2920 2f20 320a 0a20   + right) / 2.. 
+0000ce00: 2020 2020 2020 2020 2020 2023 206c 6574             # let
+0000ce10: 206d 6964 706f 696e 7420 6265 2077 6569   midpoint be wei
+0000ce20: 6768 7465 6420 7661 6c75 6520 6261 7365  ghted value base
+0000ce30: 6420 6f6e 2046 4f53 0a20 2020 2020 2020  d on FOS.       
+0000ce40: 2020 2020 206c 6566 745f 666f 7320 3d20       left_fos = 
+0000ce50: 7365 6c66 2e5f 6479 6e61 6d69 635f 7265  self._dynamic_re
+0000ce60: 7375 6c74 735b 6c65 6674 5d0a 2020 2020  sults[left].    
+0000ce70: 2020 2020 2020 2020 7269 6768 745f 666f          right_fo
+0000ce80: 7320 3d20 7365 6c66 2e5f 6479 6e61 6d69  s = self._dynami
+0000ce90: 635f 7265 7375 6c74 735b 7269 6768 745d  c_results[right]
+0000cea0: 0a0a 2020 2020 2020 2020 2020 2020 6d20  ..            m 
+0000ceb0: 3d20 286c 6566 745f 666f 7320 2d20 7269  = (left_fos - ri
+0000cec0: 6768 745f 666f 7329 202f 2028 6c65 6674  ght_fos) / (left
+0000ced0: 202d 2072 6967 6874 290a 2020 2020 2020   - right).      
+0000cee0: 2020 2020 2020 6d69 6470 6f69 6e74 203d        midpoint =
+0000cef0: 2072 6967 6874 202b 2028 6372 6974 6963   right + (critic
+0000cf00: 616c 5f66 6f73 202d 2072 6967 6874 5f66  al_fos - right_f
+0000cf10: 6f73 2920 2f20 6d0a 0a20 2020 2020 2020  os) / m..       
+0000cf20: 2020 2020 2073 656c 662e 5f73 6574 5f64       self._set_d
+0000cf30: 796e 616d 6963 5f6f 6666 7365 7428 6d69  ynamic_offset(mi
+0000cf40: 6470 6f69 6e74 290a 2020 2020 2020 2020  dpoint).        
+0000cf50: 2020 2020 7365 6c66 2e61 6e61 6c79 7365      self.analyse
+0000cf60: 5f73 6c6f 7065 2829 0a20 2020 2020 2020  _slope().       
+0000cf70: 2020 2020 2066 6f73 203d 2073 656c 662e       fos = self.
+0000cf80: 6765 745f 6d69 6e5f 464f 5328 290a 2020  get_min_FOS().  
+0000cf90: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000cfa0: 6479 6e61 6d69 635f 7265 7375 6c74 735b  dynamic_results[
+0000cfb0: 6d69 6470 6f69 6e74 5d20 3d20 666f 730a  midpoint] = fos.
+0000cfc0: 0a20 2020 2020 2020 2020 2020 2023 2063  .            # c
+0000cfd0: 6865 636b 2069 6620 6c6f 6164 2069 7320  heck if load is 
+0000cfe0: 7769 7468 696e 2074 6865 207a 6f6e 6520  within the zone 
+0000cff0: 6f66 2069 6e66 6c75 656e 6365 2c20 6966  of influence, if
+0000d000: 206c 6173 7420 7477 6f20 464f 5320 6172   last two FOS ar
+0000d010: 6520 6964 656e 7469 6361 6c0a 2020 2020  e identical.    
+0000d020: 2020 2020 2020 2020 2320 7468 656e 2070          # then p
+0000d030: 726f 6261 626c 7920 6e6f 740a 2020 2020  robably not.    
+0000d040: 2020 2020 2020 2020 6966 2070 7265 7669          if previ
+0000d050: 6f75 735f 666f 7320 213d 2066 6f73 3a0a  ous_fos != fos:.
+0000d060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d070: 6966 2028 0a20 2020 2020 2020 2020 2020  if (.           
+0000d080: 2020 2020 2020 2020 2061 6273 2870 7265           abs(pre
+0000d090: 7669 6f75 735f 666f 7320 2d20 666f 7329  vious_fos - fos)
+0000d0a0: 203c 3d20 302e 3031 206f 7220 6162 7328   <= 0.01 or abs(
+0000d0b0: 666f 7320 2d20 6372 6974 6963 616c 5f66  fos - critical_f
+0000d0c0: 6f73 2920 3c3d 2030 2e30 310a 2020 2020  os) <= 0.01.    
+0000d0d0: 2020 2020 2020 2020 2020 2020 2920 616e              ) an
+0000d0e0: 6420 726f 756e 6428 666f 732c 2033 2920  d round(fos, 3) 
+0000d0f0: 3e3d 2063 7269 7469 6361 6c5f 666f 733a  >= critical_fos:
+0000d100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d110: 2020 2020 2062 7265 616b 0a0a 2020 2020       break..    
+0000d120: 2020 2020 2020 2020 2320 4966 2046 4f53          # If FOS
+0000d130: 2068 6967 6820 7468 656e 206d 6f76 6520   high then move 
+0000d140: 636c 6f73 6572 2074 6f20 636c 6966 660a  closer to cliff.
+0000d150: 2020 2020 2020 2020 2020 2020 6966 2066              if f
+0000d160: 6f73 203c 2063 7269 7469 6361 6c5f 666f  os < critical_fo
+0000d170: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+0000d180: 2020 2072 6967 6874 203d 206d 6964 706f     right = midpo
+0000d190: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
+0000d1a0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000d1b0: 2020 2020 2020 6c65 6674 203d 206d 6964        left = mid
+0000d1c0: 706f 696e 740a 0a20 2020 2020 2020 2020  point..         
+0000d1d0: 2020 2070 7265 7669 6f75 735f 666f 7320     previous_fos 
+0000d1e0: 3d20 666f 730a 0a20 2020 2020 2020 2073  = fos..        s
+0000d1f0: 656c 662e 5f64 796e 616d 6963 5f72 6573  elf._dynamic_res
+0000d200: 756c 7473 203d 2064 6963 7428 0a20 2020  ults = dict(.   
+0000d210: 2020 2020 2020 2020 2073 6f72 7465 6428           sorted(
+0000d220: 7365 6c66 2e5f 6479 6e61 6d69 635f 7265  self._dynamic_re
+0000d230: 7375 6c74 732e 6974 656d 7328 292c 206b  sults.items(), k
+0000d240: 6579 3d6c 616d 6264 6120 6974 656d 3a20  ey=lambda item: 
+0000d250: 6974 656d 5b31 5d29 0a20 2020 2020 2020  item[1]).       
+0000d260: 2029 0a0a 2020 2020 6465 6620 5f73 6574   )..    def _set
+0000d270: 5f64 796e 616d 6963 5f6f 6666 7365 7428  _dynamic_offset(
+0000d280: 7365 6c66 2c20 6f66 6673 6574 293a 0a20  self, offset):. 
+0000d290: 2020 2020 2020 2023 2072 656d 656d 6265         # remembe
+0000d2a0: 7220 6465 6661 756c 7420 7661 6c75 6573  r default values
+0000d2b0: 3f0a 2020 2020 2020 2020 7564 6c73 203d  ?.        udls =
+0000d2c0: 2073 656c 662e 5f75 646c 730a 2020 2020   self._udls.    
+0000d2d0: 2020 2020 6c6c 7320 3d20 7365 6c66 2e5f      lls = self._
+0000d2e0: 6c6c 730a 0a20 2020 2020 2020 2023 2072  lls..        # r
+0000d2f0: 656d 6f76 6520 6c6f 6164 730a 2020 2020  emove loads.    
+0000d300: 2020 2020 7365 6c66 2e72 656d 6f76 655f      self.remove_
+0000d310: 7564 6c73 2872 656d 6f76 655f 616c 6c3d  udls(remove_all=
+0000d320: 5472 7565 290a 2020 2020 2020 2020 7365  True).        se
+0000d330: 6c66 2e72 656d 6f76 655f 6c6c 7328 7265  lf.remove_lls(re
+0000d340: 6d6f 7665 5f61 6c6c 3d54 7275 6529 0a0a  move_all=True)..
+0000d350: 2020 2020 2020 2020 2320 7570 6461 7465          # update
+0000d360: 206c 6f61 6473 0a20 2020 2020 2020 2066   loads.        f
+0000d370: 6f72 2075 646c 2069 6e20 7564 6c73 3a0a  or udl in udls:.
+0000d380: 2020 2020 2020 2020 2020 2020 6966 2075              if u
+0000d390: 646c 2e64 796e 616d 6963 5f6f 6666 7365  dl.dynamic_offse
+0000d3a0: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+0000d3b0: 2020 2075 646c 2e6f 6666 7365 7420 3d20     udl.offset = 
+0000d3c0: 6f66 6673 6574 0a20 2020 2020 2020 2020  offset.         
+0000d3d0: 2020 2073 656c 662e 7365 745f 7564 6c73     self.set_udls
+0000d3e0: 2875 646c 290a 0a20 2020 2020 2020 2066  (udl)..        f
+0000d3f0: 6f72 206c 6c20 696e 206c 6c73 3a0a 2020  or ll in lls:.  
+0000d400: 2020 2020 2020 2020 2020 6966 206c 6c2e            if ll.
+0000d410: 6479 6e61 6d69 635f 6f66 6673 6574 3a0a  dynamic_offset:.
+0000d420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d430: 6c6c 2e6f 6666 7365 7420 3d20 6f66 6673  ll.offset = offs
+0000d440: 6574 0a20 2020 2020 2020 2020 2020 2073  et.            s
+0000d450: 656c 662e 7365 745f 6c6c 7328 6c6c 290a  elf.set_lls(ll).
+0000d460: 0a20 2020 2064 6566 205f 6765 745f 6369  .    def _get_ci
+0000d470: 7263 6c65 5f65 7874 6572 6e61 6c5f 696e  rcle_external_in
+0000d480: 7465 7273 6563 7469 6f6e 2873 656c 662c  tersection(self,
+0000d490: 2063 5f78 3a20 666c 6f61 742c 2063 5f79   c_x: float, c_y
+0000d4a0: 3a20 666c 6f61 742c 2072 6164 6975 733a  : float, radius:
+0000d4b0: 2066 6c6f 6174 293a 0a20 2020 2020 2020   float):.       
+0000d4c0: 2022 2222 4765 7420 696e 7465 7273 6563   """Get intersec
+0000d4d0: 7469 6f6e 2070 6f69 6e74 7320 6f66 2061  tion points of a
+0000d4e0: 2063 6972 636c 6520 7769 7468 2065 7874   circle with ext
+0000d4f0: 6572 6e61 6c20 626f 756e 6461 7279 0a0a  ernal boundary..
+0000d500: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+0000d510: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
+0000d520: 2d2d 2d2d 2d0a 2020 2020 2020 2020 635f  -----.        c_
+0000d530: 7820 3a20 666c 6f61 740a 2020 2020 2020  x : float.      
+0000d540: 2020 2020 2020 6369 7263 6c65 2078 2063        circle x c
+0000d550: 6f6f 6469 6e61 7465 0a20 2020 2020 2020  oodinate.       
+0000d560: 2063 5f79 203a 2066 6c6f 6174 0a20 2020   c_y : float.   
+0000d570: 2020 2020 2020 2020 2063 6972 636c 6520           circle 
+0000d580: 7920 636f 6f72 6469 6e61 7465 0a20 2020  y coordinate.   
+0000d590: 2020 2020 2072 6164 6975 7320 3a20 666c       radius : fl
+0000d5a0: 6f61 740a 2020 2020 2020 2020 2020 2020  oat.            
+0000d5b0: 6369 7263 6c65 2072 6164 6975 730a 0a20  circle radius.. 
+0000d5c0: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
+0000d5d0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
+0000d5e0: 2020 2020 2020 2074 7570 6c65 0a20 2020         tuple.   
+0000d5f0: 2020 2020 2020 2020 2074 7570 6c65 206f           tuple o
+0000d600: 6620 7477 6f20 636f 6f72 6469 6e61 7465  f two coordinate
+0000d610: 7320 286c 6566 7420 636f 6f72 6469 6e61  s (left coordina
+0000d620: 7465 2c20 7269 6768 7420 636f 6f72 6469  te, right coordi
+0000d630: 6e61 7465 290a 2020 2020 2020 2020 2222  nate).        ""
+0000d640: 220a 0a20 2020 2020 2020 2069 5f6c 6973  "..        i_lis
+0000d650: 7420 3d20 5b5d 0a0a 2020 2020 2020 2020  t = []..        
+0000d660: 746f 705f 696e 7465 7273 6563 7469 6f6e  top_intersection
+0000d670: 203d 2075 7469 6c69 7469 6573 2e63 6972   = utilities.cir
+0000d680: 6c65 5f6c 696e 655f 696e 7465 7273 6563  le_line_intersec
+0000d690: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
+0000d6a0: 2020 2830 2c20 7365 6c66 2e5f 746f 705f    (0, self._top_
+0000d6b0: 636f 6f72 645b 315d 292c 2073 656c 662e  coord[1]), self.
+0000d6c0: 5f74 6f70 5f63 6f6f 7264 2c20 635f 782c  _top_coord, c_x,
+0000d6d0: 2063 5f79 2c20 7261 6469 7573 0a20 2020   c_y, radius.   
+0000d6e0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+0000d6f0: 2320 6f6e 6c79 2063 6172 6520 6162 6f75  # only care abou
+0000d700: 7420 6c65 6674 206f 6620 6369 7263 6c65  t left of circle
+0000d710: 2066 6f72 2074 6f70 2069 6e74 6572 7365   for top interse
+0000d720: 6374 696f 6e0a 2020 2020 2020 2020 2320  ction.        # 
+0000d730: 7369 6e63 6520 6661 696c 7572 6520 6672  since failure fr
+0000d740: 6f6d 206c 6566 7420 746f 2072 6967 6874  om left to right
+0000d750: 2061 6c77 6179 730a 2020 2020 2020 2020   always.        
+0000d760: 6966 2074 6f70 5f69 6e74 6572 7365 6374  if top_intersect
+0000d770: 696f 6e3a 0a20 2020 2020 2020 2020 2020  ion:.           
+0000d780: 2074 6f70 5f69 6e74 6572 7365 6374 696f   top_intersectio
+0000d790: 6e2e 736f 7274 2829 0a20 2020 2020 2020  n.sort().       
+0000d7a0: 2020 2020 2074 6f70 5f69 6e74 6572 7365       top_interse
+0000d7b0: 6374 696f 6e20 3d20 746f 705f 696e 7465  ction = top_inte
+0000d7c0: 7273 6563 7469 6f6e 5b30 5d0a 2020 2020  rsection[0].    
+0000d7d0: 2020 2020 2020 2020 6966 2074 6f70 5f69          if top_i
+0000d7e0: 6e74 6572 7365 6374 696f 6e5b 305d 203e  ntersection[0] >
+0000d7f0: 3d20 3020 616e 6420 746f 705f 696e 7465  = 0 and top_inte
+0000d800: 7273 6563 7469 6f6e 5b30 5d20 3c3d 2073  rsection[0] <= s
+0000d810: 656c 662e 5f74 6f70 5f63 6f6f 7264 5b30  elf._top_coord[0
+0000d820: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+0000d830: 2020 2069 5f6c 6973 742e 6170 7065 6e64     i_list.append
+0000d840: 2874 6f70 5f69 6e74 6572 7365 6374 696f  (top_intersectio
+0000d850: 6e29 0a0a 2020 2020 2020 2020 626f 745f  n)..        bot_
+0000d860: 696e 7465 7273 6563 7469 6f6e 203d 2075  intersection = u
+0000d870: 7469 6c69 7469 6573 2e63 6972 6c65 5f6c  tilities.cirle_l
+0000d880: 696e 655f 696e 7465 7273 6563 7469 6f6e  ine_intersection
+0000d890: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
+0000d8a0: 6c66 2e5f 626f 745f 636f 6f72 642c 0a20  lf._bot_coord,. 
+0000d8b0: 2020 2020 2020 2020 2020 2028 7365 6c66             (self
+0000d8c0: 2e5f 6578 7465 726e 616c 5f6c 656e 6774  ._external_lengt
+0000d8d0: 682c 2073 656c 662e 5f62 6f74 5f63 6f6f  h, self._bot_coo
+0000d8e0: 7264 5b31 5d29 2c0a 2020 2020 2020 2020  rd[1]),.        
+0000d8f0: 2020 2020 635f 782c 0a20 2020 2020 2020      c_x,.       
+0000d900: 2020 2020 2063 5f79 2c0a 2020 2020 2020       c_y,.      
+0000d910: 2020 2020 2020 7261 6469 7573 2c0a 2020        radius,.  
+0000d920: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0000d930: 2023 206f 6e6c 7920 6361 7265 2061 626f   # only care abo
+0000d940: 7574 2072 6967 6874 206f 6620 6369 7263  ut right of circ
+0000d950: 6c65 2066 6f72 2062 6f74 746f 6d20 696e  le for bottom in
+0000d960: 7465 7273 6563 7469 6f6e 0a20 2020 2020  tersection.     
+0000d970: 2020 2023 2073 696e 6365 2066 6169 6c75     # since failu
+0000d980: 7265 2077 696c 6c20 616c 7761 7973 2062  re will always b
+0000d990: 6520 746f 2072 6967 6874 206f 6620 6369  e to right of ci
+0000d9a0: 726c 6520 6f6e 2062 6f74 746f 6d0a 2020  rle on bottom.  
+0000d9b0: 2020 2020 2020 2320 756e 6c65 7373 2066        # unless f
+0000d9c0: 6169 6c75 7265 2063 7574 7320 7468 726f  ailure cuts thro
+0000d9d0: 7567 6820 736c 6f70 6520 2869 6e20 7768  ugh slope (in wh
+0000d9e0: 6963 6820 6361 7365 2076 616c 7565 206f  ich case value o
+0000d9f0: 6620 746f 650a 2020 2020 2020 2020 2320  f toe.        # 
+0000da00: 7769 6c6c 2062 6520 7069 636b 6564 2075  will be picked u
+0000da10: 7020 666f 7220 6d69 6420 696e 7465 7273  p for mid inters
+0000da20: 6563 7469 6f6e 2061 6e79 7761 7973 290a  ection anyways).
+0000da30: 2020 2020 2020 2020 6966 2062 6f74 5f69          if bot_i
+0000da40: 6e74 6572 7365 6374 696f 6e3a 0a20 2020  ntersection:.   
+0000da50: 2020 2020 2020 2020 2062 6f74 5f69 6e74           bot_int
+0000da60: 6572 7365 6374 696f 6e2e 736f 7274 2829  ersection.sort()
+0000da70: 0a20 2020 2020 2020 2020 2020 2062 6f74  .            bot
+0000da80: 5f69 6e74 6572 7365 6374 696f 6e20 3d20  _intersection = 
+0000da90: 626f 745f 696e 7465 7273 6563 7469 6f6e  bot_intersection
+0000daa0: 5b2d 315d 0a20 2020 2020 2020 2020 2020  [-1].           
+0000dab0: 2069 6620 280a 2020 2020 2020 2020 2020   if (.          
+0000dac0: 2020 2020 2020 626f 745f 696e 7465 7273        bot_inters
+0000dad0: 6563 7469 6f6e 5b30 5d20 3e3d 2073 656c  ection[0] >= sel
+0000dae0: 662e 5f62 6f74 5f63 6f6f 7264 5b30 5d0a  f._bot_coord[0].
+0000daf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db00: 616e 6420 626f 745f 696e 7465 7273 6563  and bot_intersec
+0000db10: 7469 6f6e 5b30 5d20 3c3d 2073 656c 662e  tion[0] <= self.
+0000db20: 5f65 7874 6572 6e61 6c5f 6c65 6e67 7468  _external_length
+0000db30: 0a20 2020 2020 2020 2020 2020 2029 3a0a  .            ):.
+0000db40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db50: 695f 6c69 7374 2e61 7070 656e 6428 626f  i_list.append(bo
+0000db60: 745f 696e 7465 7273 6563 7469 6f6e 290a  t_intersection).
+0000db70: 0a20 2020 2020 2020 206d 6964 5f69 6e74  .        mid_int
+0000db80: 6572 7365 6374 696f 6e20 3d20 7574 696c  ersection = util
+0000db90: 6974 6965 732e 6369 726c 655f 6c69 6e65  ities.cirle_line
+0000dba0: 5f69 6e74 6572 7365 6374 696f 6e28 0a20  _intersection(. 
+0000dbb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000dbc0: 5f74 6f70 5f63 6f6f 7264 2c20 7365 6c66  _top_coord, self
+0000dbd0: 2e5f 626f 745f 636f 6f72 642c 2063 5f78  ._bot_coord, c_x
+0000dbe0: 2c20 635f 792c 2072 6164 6975 730a 2020  , c_y, radius.  
+0000dbf0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0000dc00: 2066 6f72 2061 2069 6e20 6d69 645f 696e   for a in mid_in
+0000dc10: 7465 7273 6563 7469 6f6e 3a0a 2020 2020  tersection:.    
+0000dc20: 2020 2020 2020 2020 6966 2061 5b30 5d20          if a[0] 
+0000dc30: 3e3d 2073 656c 662e 5f74 6f70 5f63 6f6f  >= self._top_coo
+0000dc40: 7264 5b30 5d20 616e 6420 615b 305d 203c  rd[0] and a[0] <
+0000dc50: 3d20 7365 6c66 2e5f 626f 745f 636f 6f72  = self._bot_coor
+0000dc60: 645b 305d 3a0a 2020 2020 2020 2020 2020  d[0]:.          
+0000dc70: 2020 2020 2020 695f 6c69 7374 2e61 7070        i_list.app
+0000dc80: 656e 6428 6129 0a0a 2020 2020 2020 2020  end(a)..        
+0000dc90: 2320 7265 6d6f 7665 2061 6e79 2063 6c6f  # remove any clo
+0000dca0: 7365 2070 6f69 6e74 730a 2020 2020 2020  se points.      
+0000dcb0: 2020 695f 6c69 7374 2e73 6f72 7428 6b65    i_list.sort(ke
+0000dcc0: 793d 6c61 6d62 6461 2078 3a20 785b 305d  y=lambda x: x[0]
+0000dcd0: 290a 2020 2020 2020 2020 756e 6971 7565  ).        unique
+0000dce0: 5f6c 6973 7420 3d20 5b5d 0a20 2020 2020  _list = [].     
+0000dcf0: 2020 2078 203d 202d 310a 2020 2020 2020     x = -1.      
+0000dd00: 2020 666f 7220 6920 696e 2069 5f6c 6973    for i in i_lis
+0000dd10: 743a 0a20 2020 2020 2020 2020 2020 2069  t:.            i
+0000dd20: 6620 6162 7328 695b 305d 202d 2078 2920  f abs(i[0] - x) 
+0000dd30: 3e20 302e 3031 3a0a 2020 2020 2020 2020  > 0.01:.        
+0000dd40: 2020 2020 2020 2020 756e 6971 7565 5f6c          unique_l
+0000dd50: 6973 742e 6170 7065 6e64 2869 290a 2020  ist.append(i).  
+0000dd60: 2020 2020 2020 2020 2020 7820 3d20 695b            x = i[
+0000dd70: 305d 0a0a 2020 2020 2020 2020 7265 7475  0]..        retu
+0000dd80: 726e 2075 6e69 7175 655f 6c69 7374 0a0a  rn unique_list..
+0000dd90: 2020 2020 6465 6620 5f63 616c 6375 6c61      def _calcula
+0000dda0: 7465 5f73 7472 6970 5f77 6569 6768 7428  te_strip_weight(
+0000ddb0: 7365 6c66 2c20 623a 2066 6c6f 6174 2c20  self, b: float, 
+0000ddc0: 735f 7974 3a20 666c 6f61 742c 2073 5f79  s_yt: float, s_y
+0000ddd0: 623a 2066 6c6f 6174 293a 0a20 2020 2020  b: float):.     
+0000dde0: 2020 2022 2222 6361 6c63 756c 6174 6573     """calculates
+0000ddf0: 2074 6865 2077 6569 6768 7420 6f66 2061   the weight of a
+0000de00: 2073 7472 6970 2e0a 0a20 2020 2020 2020   strip...       
+0000de10: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+0000de20: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+0000de30: 2020 2020 2020 2062 203a 2066 6c6f 6174         b : float
+0000de40: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
+0000de50: 6970 2077 6964 7468 2069 6e20 6d65 7472  ip width in metr
+0000de60: 6573 0a20 2020 2020 2020 2073 5f79 7420  es.        s_yt 
+0000de70: 3a20 666c 6f61 740a 2020 2020 2020 2020  : float.        
+0000de80: 2020 2020 7374 7269 7020 7920 636f 6f72      strip y coor
+0000de90: 6469 6e61 7465 2061 7420 746f 7020 6f66  dinate at top of
+0000dea0: 2073 7472 6970 0a20 2020 2020 2020 2073   strip.        s
+0000deb0: 5f79 6220 3a20 666c 6f61 740a 2020 2020  _yb : float.    
+0000dec0: 2020 2020 2020 2020 7374 7269 7020 7920          strip y 
+0000ded0: 636f 6f72 6469 6e61 7465 2061 7420 626f  coordinate at bo
+0000dee0: 7474 6f6d 206f 6620 7374 7269 700a 0a20  ttom of strip.. 
+0000def0: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
+0000df00: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
+0000df10: 2020 2020 2020 2066 6c6f 6174 0a20 2020         float.   
+0000df20: 2020 2020 2020 2020 2057 6569 6768 7420           Weight 
+0000df30: 6f66 2073 7472 6970 2069 6e20 6b4e 2e0a  of strip in kN..
+0000df40: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
+0000df50: 2020 2020 2023 2069 6e74 6961 6c69 7a65       # intialize
+0000df60: 2070 726f 7065 7274 6965 730a 2020 2020   properties.    
+0000df70: 2020 2020 5720 3d20 302e 3020 2023 206b      W = 0.0  # k
+0000df80: 4e0a 2020 2020 2020 2020 746f 7020 3d20  N.        top = 
+0000df90: 735f 7974 0a0a 2020 2020 2020 2020 2320  s_yt..        # 
+0000dfa0: 6c6f 6f70 2074 6872 6f75 6768 206d 6174  loop through mat
+0000dfb0: 6572 6961 6c73 206e 6f74 696e 6720 7468  erials noting th
+0000dfc0: 6174 2074 6865 7920 6172 6520 616c 7265  at they are alre
+0000dfd0: 6164 7920 736f 7274 6564 2062 7920 6465  ady sorted by de
+0000dfe0: 7074 680a 2020 2020 2020 2020 666f 7220  pth.        for 
+0000dff0: 6d20 696e 2073 656c 662e 5f6d 6174 6572  m in self._mater
+0000e000: 6961 6c73 3a0a 2020 2020 2020 2020 2020  ials:.          
+0000e010: 2020 2320 7768 696c 6520 6c61 7965 7273    # while layers
+0000e020: 2061 7265 2068 6967 6865 7220 7468 616e   are higher than
+0000e030: 2074 6865 2074 6f70 206f 6620 7468 6520   the top of the 
+0000e040: 736c 6963 6520 6967 6e6f 7265 2074 6865  slice ignore the
+0000e050: 206d 6174 6572 6961 6c0a 2020 2020 2020   material.      
+0000e060: 2020 2020 2020 6966 206d 2e52 4c20 3e3d        if m.RL >=
+0000e070: 2073 5f79 743a 0a20 2020 2020 2020 2020   s_yt:.         
+0000e080: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
+0000e090: 2020 2020 2020 2020 2020 2020 2320 7768              # wh
+0000e0a0: 696c 6520 7468 6520 626f 7474 6f6d 206f  ile the bottom o
+0000e0b0: 6620 6c61 7965 7220 6973 2069 6e20 7468  f layer is in th
+0000e0c0: 6520 736c 6963 6520 636f 6e73 6964 6572  e slice consider
+0000e0d0: 2c20 676f 2066 726f 6d20 7468 650a 2020  , go from the.  
+0000e0e0: 2020 2020 2020 2020 2020 2320 6375 7272            # curr
+0000e0f0: 656e 7420 746f 7020 746f 2074 6865 2062  ent top to the b
+0000e100: 6f74 746f 6d20 6f66 2074 6865 206c 6179  ottom of the lay
+0000e110: 6572 0a20 2020 2020 2020 2020 2020 2023  er.            #
+0000e120: 2074 6869 7320 6361 7074 7572 6573 2074   this captures t
+0000e130: 6865 2063 6173 6520 6f66 2074 6865 2074  he case of the t
+0000e140: 6f70 206f 6620 7468 6520 7374 7269 7020  op of the strip 
+0000e150: 6265 696e 6720 7061 7274 6961 6c6c 7920  being partially 
+0000e160: 696e 2061 206c 6179 6572 0a20 2020 2020  in a layer.     
+0000e170: 2020 2020 2020 2065 6c69 6620 6d2e 524c         elif m.RL
+0000e180: 203c 2073 5f79 7420 616e 6420 6d2e 524c   < s_yt and m.RL
+0000e190: 203e 2073 5f79 623a 0a20 2020 2020 2020   > s_yb:.       
+0000e1a0: 2020 2020 2020 2020 2057 202b 3d20 6220           W += b 
+0000e1b0: 2a20 6d2e 756e 6974 5f77 6569 6768 7420  * m.unit_weight 
+0000e1c0: 2a20 2874 6f70 202d 206d 2e52 4c29 0a20  * (top - m.RL). 
+0000e1d0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000e1e0: 6f70 203d 206d 2e52 4c0a 2020 2020 2020  op = m.RL.      
+0000e1f0: 2020 2020 2020 2320 696e 2074 6865 2063        # in the c
+0000e200: 6173 6520 7468 6174 2074 6865 2062 6f74  ase that the bot
+0000e210: 746f 6d20 6f66 2074 6865 2073 7472 6970  tom of the strip
+0000e220: 2069 7320 6e6f 7720 6f75 7473 6964 6520   is now outside 
+0000e230: 7468 6520 7261 6e67 650a 2020 2020 2020  the range.      
+0000e240: 2020 2020 2020 2320 7765 2073 7469 6c6c        # we still
+0000e250: 2068 6176 6520 6d61 7465 7269 616c 2062   have material b
+0000e260: 6574 7765 656e 2074 6865 2063 7572 7265  etween the curre
+0000e270: 6e74 2074 6f70 2061 6e64 2074 6865 2062  nt top and the b
+0000e280: 6f74 746f 6d20 6f66 2074 6865 2073 7472  ottom of the str
+0000e290: 6970 0a20 2020 2020 2020 2020 2020 2023  ip.            #
+0000e2a0: 2077 6520 6361 7074 7572 6520 6974 2069   we capture it i
+0000e2b0: 6e20 7468 6973 2065 6467 6520 6361 7365  n this edge case
+0000e2c0: 2061 6e64 2074 6865 6e20 6272 6561 6b20   and then break 
+0000e2d0: 7369 6e63 6520 6576 6572 7974 6869 6e67  since everything
+0000e2e0: 2062 656c 6f77 2063 616e 2062 6520 6967   below can be ig
+0000e2f0: 6e6f 7265 640a 2020 2020 2020 2020 2020  nored.          
+0000e300: 2020 2320 7765 2061 6c73 6f20 6772 6162    # we also grab
+0000e310: 2074 6865 206d 6174 6572 6961 6c20 7072   the material pr
+0000e320: 6f70 6572 7469 6573 2061 7420 7468 6520  operties at the 
+0000e330: 6261 7365 0a20 2020 2020 2020 2020 2020  base.           
+0000e340: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000e350: 2020 2020 2020 2057 202b 3d20 6220 2a20         W += b * 
+0000e360: 6d2e 756e 6974 5f77 6569 6768 7420 2a20  m.unit_weight * 
+0000e370: 2874 6f70 202d 2073 5f79 6229 0a20 2020  (top - s_yb).   
+0000e380: 2020 2020 2020 2020 2020 2020 2074 6f70               top
+0000e390: 203d 206d 2e52 4c0a 2020 2020 2020 2020   = m.RL.        
+0000e3a0: 2020 2020 2020 2020 6272 6561 6b0a 0a20          break.. 
+0000e3b0: 2020 2020 2020 2023 2063 6865 636b 2063         # check c
+0000e3c0: 6173 6520 7468 6174 2072 616e 206f 7574  ase that ran out
+0000e3d0: 206f 6620 6c61 7965 7273 2028 6c6f 6f70   of layers (loop
+0000e3e0: 2074 6572 6d69 6e61 7465 6420 6561 726c   terminated earl
+0000e3f0: 6965 7220 7468 616e 2065 7870 6563 7465  ier than expecte
+0000e400: 6429 0a20 2020 2020 2020 2069 6620 746f  d).        if to
+0000e410: 7020 3e20 735f 7962 3a0a 2020 2020 2020  p > s_yb:.      
+0000e420: 2020 2020 2020 6d20 3d20 7365 6c66 2e5f        m = self._
+0000e430: 6d61 7465 7269 616c 735b 2d31 5d0a 2020  materials[-1].  
+0000e440: 2020 2020 2020 2020 2020 5720 2b3d 2062            W += b
+0000e450: 202a 206d 2e75 6e69 745f 7765 6967 6874   * m.unit_weight
+0000e460: 202a 2028 746f 7020 2d20 735f 7962 290a   * (top - s_yb).
+0000e470: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000e480: 570a 0a20 2020 2064 6566 205f 6765 745f  W..    def _get_
+0000e490: 6d61 7465 7269 616c 5f61 745f 6465 7074  material_at_dept
+0000e4a0: 6828 7365 6c66 2c20 735f 7962 293a 0a20  h(self, s_yb):. 
+0000e4b0: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
+0000e4c0: 2074 6865 206d 6174 6572 6961 6c20 636c   the material cl
+0000e4d0: 6173 7320 6174 2061 2073 7065 6369 6669  ass at a specifi
+0000e4e0: 6564 2064 6570 7468 2e0a 0a20 2020 2020  ed depth...     
+0000e4f0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+0000e500: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+0000e510: 0a20 2020 2020 2020 2073 5f79 6220 3a20  .        s_yb : 
+0000e520: 666c 6f61 740a 2020 2020 2020 2020 2020  float.          
+0000e530: 2020 7374 7269 7020 7920 636f 6f72 6469    strip y coordi
+0000e540: 6e61 7465 2061 7420 626f 7474 6f6d 206f  nate at bottom o
+0000e550: 6620 7374 7269 700a 0a20 2020 2020 2020  f strip..       
+0000e560: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
+0000e570: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
+0000e580: 204d 6174 6572 6961 6c0a 2020 2020 2020   Material.      
+0000e590: 2020 2020 2020 6d61 7465 7269 616c 206f        material o
+0000e5a0: 626a 6563 7420 6174 2074 6865 2073 7065  bject at the spe
+0000e5b0: 6369 6669 6564 2064 6570 7468 2e0a 2020  cified depth..  
+0000e5c0: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+0000e5d0: 2020 2023 206c 6f6f 7020 7468 726f 7567     # loop throug
+0000e5e0: 6820 616c 6c20 6d61 7465 7269 616c 732c  h all materials,
+0000e5f0: 2069 6620 7765 2068 6176 6520 7061 7373   if we have pass
+0000e600: 6564 2074 6865 2062 6f74 746f 6d20 7461  ed the bottom ta
+0000e610: 6b65 2074 6865 2070 7265 7669 6f75 730a  ke the previous.
+0000e620: 2020 2020 2020 2020 666f 7220 6d20 696e          for m in
+0000e630: 2073 656c 662e 5f6d 6174 6572 6961 6c73   self._materials
+0000e640: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+0000e650: 206d 2e52 4c20 3c20 735f 7962 3a0a 2020   m.RL < s_yb:.  
+0000e660: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000e670: 7475 726e 206d 0a0a 2020 2020 2020 2020  turn m..        
+0000e680: 7265 7475 726e 2073 656c 662e 5f6d 6174  return self._mat
+0000e690: 6572 6961 6c73 5b2d 315d 0a0a 2020 2020  erials[-1]..    
+0000e6a0: 6465 6620 5f63 616c 6375 6c61 7465 5f73  def _calculate_s
+0000e6b0: 7472 6970 5f75 646c 5f66 6f72 6365 2873  trip_udl_force(s
+0000e6c0: 656c 662c 2062 2c20 735f 782c 2075 646c  elf, b, s_x, udl
+0000e6d0: 293a 0a20 2020 2020 2020 2022 2222 4361  ):.        """Ca
+0000e6e0: 6c63 756c 6174 6573 2074 6865 2075 646c  lculates the udl
+0000e6f0: 2066 6f72 6365 206f 7665 7220 7374 7269   force over stri
+0000e700: 702e 0a0a 2020 2020 2020 2020 5061 7261  p...        Para
+0000e710: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
+0000e720: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+0000e730: 2020 6220 3a20 666c 6f61 742c 0a20 2020    b : float,.   
+0000e740: 2020 2020 2020 2020 2073 7472 6970 2077           strip w
+0000e750: 6964 7468 2069 6e20 6d0a 2020 2020 2020  idth in m.      
+0000e760: 2020 735f 7820 3a20 666c 6f61 742c 0a20    s_x : float,. 
+0000e770: 2020 2020 2020 2020 2020 2073 7472 6970             strip
+0000e780: 2078 2063 6f6f 7264 696e 6174 6520 2866   x coordinate (f
+0000e790: 6f72 2063 656e 7465 7220 6f66 2073 7472  or center of str
+0000e7a0: 6970 290a 2020 2020 2020 2020 7564 6c20  ip).        udl 
+0000e7b0: 3a20 5564 6c20 6f62 6a65 6374 2c0a 2020  : Udl object,.  
+0000e7c0: 2020 2020 2020 2020 2020 7564 6c20 6f62            udl ob
+0000e7d0: 6a65 6374 0a0a 2020 2020 2020 2020 5265  ject..        Re
+0000e7e0: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
+0000e7f0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 666c  -----.        fl
+0000e800: 6f61 740a 2020 2020 2020 2020 2020 2020  oat.            
+0000e810: 7564 6c20 666f 7263 6520 6f6e 2073 7472  udl force on str
+0000e820: 6970 2069 6e20 6b4e 0a20 2020 2020 2020  ip in kN.       
+0000e830: 2022 2222 0a20 2020 2020 2020 2057 203d   """.        W =
+0000e840: 2030 0a0a 2020 2020 2020 2020 6c6f 6164   0..        load
+0000e850: 5f78 6c2c 206c 6f61 645f 7872 203d 2075  _xl, load_xr = u
+0000e860: 646c 2e6c 6566 742c 2075 646c 2e72 6967  dl.left, udl.rig
+0000e870: 6874 0a20 2020 2020 2020 2073 7472 6970  ht.        strip
+0000e880: 5f78 6c20 3d20 735f 7820 2d20 2862 202f  _xl = s_x - (b /
+0000e890: 2032 290a 2020 2020 2020 2020 7374 7269   2).        stri
+0000e8a0: 705f 7872 203d 2073 5f78 202b 2028 6220  p_xr = s_x + (b 
+0000e8b0: 2f20 3229 0a0a 2020 2020 2020 2020 2320  / 2)..        # 
+0000e8c0: 6361 7365 2031 2063 6c65 6172 6c79 206c  case 1 clearly l
+0000e8d0: 6f61 6420 6973 2063 6f6d 706c 6574 656c  oad is completel
+0000e8e0: 7920 696e 7369 6465 0a20 2020 2020 2020  y inside.       
+0000e8f0: 2069 6620 6c6f 6164 5f78 6c20 3c3d 2073   if load_xl <= s
+0000e900: 7472 6970 5f78 6c20 616e 6420 6c6f 6164  trip_xl and load
+0000e910: 5f78 7220 3e3d 2073 7472 6970 5f78 723a  _xr >= strip_xr:
+0000e920: 0a20 2020 2020 2020 2020 2020 2057 202b  .            W +
+0000e930: 3d20 6220 2a20 7564 6c2e 6d61 676e 6974  = b * udl.magnit
+0000e940: 7564 650a 2020 2020 2020 2020 2320 6361  ude.        # ca
+0000e950: 7365 2032 206f 6e20 7468 6520 6c65 6674  se 2 on the left
+0000e960: 2069 6e73 6964 6520 7468 6520 6c6f 6164   inside the load
+0000e970: 0a20 2020 2020 2020 2065 6c69 6620 7374  .        elif st
+0000e980: 7269 705f 786c 203c 3d20 6c6f 6164 5f78  rip_xl <= load_x
+0000e990: 6c20 616e 6420 7374 7269 705f 7872 203e  l and strip_xr >
+0000e9a0: 3d20 6c6f 6164 5f78 6c3a 0a20 2020 2020  = load_xl:.     
+0000e9b0: 2020 2020 2020 2057 202b 3d20 2873 7472         W += (str
+0000e9c0: 6970 5f78 7220 2d20 6c6f 6164 5f78 6c29  ip_xr - load_xl)
+0000e9d0: 202a 2075 646c 2e6d 6167 6e69 7475 6465   * udl.magnitude
+0000e9e0: 0a0a 2020 2020 2020 2020 2320 6361 7365  ..        # case
+0000e9f0: 2033 206f 6e20 7468 6520 7269 6768 7420   3 on the right 
+0000ea00: 7369 6465 206f 6620 7468 6520 6c6f 6164  side of the load
+0000ea10: 0a20 2020 2020 2020 2065 6c69 6620 7374  .        elif st
+0000ea20: 7269 705f 786c 203c 3d20 6c6f 6164 5f78  rip_xl <= load_x
+0000ea30: 7220 616e 6420 7374 7269 705f 7872 203e  r and strip_xr >
+0000ea40: 3d20 6c6f 6164 5f78 723a 0a20 2020 2020  = load_xr:.     
+0000ea50: 2020 2020 2020 2057 202b 3d20 286c 6f61         W += (loa
+0000ea60: 645f 7872 202d 2073 7472 6970 5f78 6c29  d_xr - strip_xl)
+0000ea70: 202a 2075 646c 2e6d 6167 6e69 7475 6465   * udl.magnitude
+0000ea80: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0000ea90: 2057 0a0a 2020 2020 6465 6620 5f63 616c   W..    def _cal
+0000eaa0: 6375 6c61 7465 5f73 7472 6970 5f6c 6c28  culate_strip_ll(
+0000eab0: 7365 6c66 2c20 622c 2073 5f78 2c20 6c6c  self, b, s_x, ll
+0000eac0: 293a 0a20 2020 2020 2020 2022 2222 4361  ):.        """Ca
+0000ead0: 6c63 756c 6174 6573 2074 6865 206c 6c20  lculates the ll 
+0000eae0: 666f 7263 6520 6f76 6572 2073 7472 6970  force over strip
+0000eaf0: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+0000eb00: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+0000eb10: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+0000eb20: 2062 203a 2066 6c6f 6174 2c0a 2020 2020   b : float,.    
+0000eb30: 2020 2020 2020 2020 7374 7269 7020 7769          strip wi
+0000eb40: 6474 6820 696e 206d 0a20 2020 2020 2020  dth in m.       
+0000eb50: 2073 5f78 203a 2066 6c6f 6174 2c0a 2020   s_x : float,.  
+0000eb60: 2020 2020 2020 2020 2020 7374 7269 7020            strip 
+0000eb70: 7820 636f 6f72 6469 6e61 7465 2028 666f  x coordinate (fo
+0000eb80: 7220 6365 6e74 6572 206f 6620 7374 7269  r center of stri
+0000eb90: 7029 0a20 2020 2020 2020 206c 6c20 3a20  p).        ll : 
+0000eba0: 4c69 6e65 4c6f 6164 206f 626a 6563 742c  LineLoad object,
+0000ebb0: 0a20 2020 2020 2020 2020 2020 204c 696e  .            Lin
+0000ebc0: 654c 6f61 6420 6f62 6a65 6374 0a0a 2020  eLoad object..  
+0000ebd0: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
+0000ebe0: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
+0000ebf0: 2020 2020 2020 666c 6f61 740a 2020 2020        float.    
+0000ec00: 2020 2020 2020 2020 7564 6c20 666f 7263          udl forc
+0000ec10: 6520 6f6e 2073 7472 6970 2069 6e20 6b4e  e on strip in kN
+0000ec20: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
+0000ec30: 2020 2020 2020 7374 7269 705f 786c 203d        strip_xl =
+0000ec40: 2073 5f78 202d 2028 6220 2f20 3229 0a20   s_x - (b / 2). 
+0000ec50: 2020 2020 2020 2073 7472 6970 5f78 7220         strip_xr 
+0000ec60: 3d20 735f 7820 2b20 2862 202f 2032 290a  = s_x + (b / 2).
+0000ec70: 0a20 2020 2020 2020 2023 204e 6565 6420  .        # Need 
+0000ec80: 6a75 7374 206f 6e65 2063 6f6d 7061 7269  just one compari
+0000ec90: 736f 6e20 746f 2062 6520 6571 7561 6c20  son to be equal 
+0000eca0: 746f 206f 7220 6772 6561 7465 7220 7468  to or greater th
+0000ecb0: 616e 2073 6f20 7468 6174 0a20 2020 2020  an so that.     
+0000ecc0: 2020 2023 2069 6e20 7468 6520 6361 7365     # in the case
+0000ecd0: 2074 6865 2070 6f69 6e74 206c 6f61 6420   the point load 
+0000ece0: 6973 2065 7863 6174 6c79 2061 7420 7468  is excatly at th
+0000ecf0: 6520 626f 756e 6461 7279 0a20 2020 2020  e boundary.     
+0000ed00: 2020 2023 2074 776f 2061 646a 6365 6e74     # two adjcent
+0000ed10: 2073 7472 6970 7320 776f 6e74 2064 6f75   strips wont dou
+0000ed20: 626c 6520 7570 206f 7220 6967 6e6f 7265  ble up or ignore
+0000ed30: 2063 6f6d 706c 6574 656c 792e 0a20 2020   completely..   
+0000ed40: 2020 2020 2069 6620 7374 7269 705f 786c       if strip_xl
+0000ed50: 203c 3d20 6c6c 2e63 6f6f 7264 203c 2073   <= ll.coord < s
+0000ed60: 7472 6970 5f78 723a 0a20 2020 2020 2020  trip_xr:.       
+0000ed70: 2020 2020 2072 6574 7572 6e20 6c6c 2e6d       return ll.m
+0000ed80: 6167 6e69 7475 6465 0a20 2020 2020 2020  agnitude.       
+0000ed90: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000eda0: 2020 2072 6574 7572 6e20 300a 0a20 2020     return 0..   
+0000edb0: 2064 6566 2067 6574 5f64 796e 616d 6963   def get_dynamic
+0000edc0: 5f72 6573 756c 7473 2873 656c 6629 3a0a  _results(self):.
+0000edd0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000ede0: 656c 662e 5f64 796e 616d 6963 5f72 6573  elf._dynamic_res
+0000edf0: 756c 7473 0a0a 2020 2020 6465 6620 7072  ults..    def pr
+0000ee00: 696e 745f 6479 6e61 6d69 635f 7265 7375  int_dynamic_resu
+0000ee10: 6c74 7328 7365 6c66 293a 0a20 2020 2020  lts(self):.     
+0000ee20: 2020 2066 6f72 206b 2c20 7620 696e 2073     for k, v in s
+0000ee30: 656c 662e 6765 745f 6479 6e61 6d69 635f  elf.get_dynamic_
+0000ee40: 7265 7375 6c74 7328 292e 6974 656d 7328  results().items(
+0000ee50: 293a 0a20 2020 2020 2020 2020 2020 206f  ):.            o
+0000ee60: 6666 7365 7420 3d20 7374 7228 726f 756e  ffset = str(roun
+0000ee70: 6428 6b2c 2033 2929 0a20 2020 2020 2020  d(k, 3)).       
+0000ee80: 2020 2020 206f 6666 7365 7420 3d20 6f66       offset = of
+0000ee90: 6673 6574 202b 2022 3022 202a 2028 3520  fset + "0" * (5 
+0000eea0: 2d20 6c65 6e28 6f66 6673 6574 2929 0a0a  - len(offset))..
+0000eeb0: 2020 2020 2020 2020 2020 2020 666f 7320              fos 
+0000eec0: 3d20 7374 7228 726f 756e 6428 762c 2033  = str(round(v, 3
+0000eed0: 2929 0a20 2020 2020 2020 2020 2020 2066  )).            f
+0000eee0: 6f73 203d 2066 6f73 202b 2022 3022 202a  os = fos + "0" *
+0000eef0: 2028 3520 2d20 6c65 6e28 666f 7329 290a   (5 - len(fos)).
+0000ef00: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+0000ef10: 6e74 2866 224f 6666 7365 743a 207b 6f66  nt(f"Offset: {of
+0000ef20: 6673 6574 7d20 6d2c 2046 4f53 3a20 7b66  fset} m, FOS: {f
+0000ef30: 6f73 7d22 290a 0a20 2020 2064 6566 2067  os}")..    def g
+0000ef40: 6574 5f6d 696e 5f46 4f53 2873 656c 6629  et_min_FOS(self)
+0000ef50: 3a0a 2020 2020 2020 2020 2222 2247 6574  :.        """Get
+0000ef60: 206d 696e 2066 6163 746f 7220 6f66 2073   min factor of s
+0000ef70: 6166 6574 7920 666f 7220 736c 6f70 6520  afety for slope 
+0000ef80: 6d6f 6465 6c2e 0a0a 2020 2020 2020 2020  model...        
+0000ef90: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
+0000efa0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+0000efb0: 666c 6f61 740a 2020 2020 2020 2020 2020  float.          
+0000efc0: 2020 6372 6974 6963 616c 2066 6163 746f    critical facto
+0000efd0: 7220 6f66 2073 6166 6574 790a 2020 2020  r of safety.    
+0000efe0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000eff0: 7265 7475 726e 2073 656c 662e 5f73 6561  return self._sea
+0000f000: 7263 685b 305d 5b22 464f 5322 5d0a 0a20  rch[0]["FOS"].. 
+0000f010: 2020 2064 6566 2067 6574 5f6d 696e 5f46     def get_min_F
+0000f020: 4f53 5f63 6972 636c 6528 7365 6c66 293a  OS_circle(self):
+0000f030: 0a20 2020 2020 2020 2022 2222 4765 7420  .        """Get 
+0000f040: 7468 6520 7072 6f70 6572 7469 6573 206f  the properties o
+0000f050: 6620 7468 6520 6369 7263 6c65 2074 6861  f the circle tha
+0000f060: 7420 6761 7665 2074 6865 2063 7269 7469  t gave the criti
+0000f070: 6361 6c20 6661 6374 6f72 206f 6620 7361  cal factor of sa
+0000f080: 6665 7479 2e0a 0a20 2020 2020 2020 2052  fety...        R
+0000f090: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
+0000f0a0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2074  ------.        t
+0000f0b0: 7570 6c65 0a20 2020 2020 2020 2020 2020  uple.           
+0000f0c0: 2074 7570 6c65 2063 6f6e 7461 696e 696e   tuple containin
+0000f0d0: 6720 2863 6972 636c 6520 7820 636f 6f72  g (circle x coor
+0000f0e0: 6469 6e61 7465 2c20 6369 7263 6c65 2079  dinate, circle y
+0000f0f0: 2063 6f6f 7264 696e 6174 652c 2063 6972   coordinate, cir
+0000f100: 636c 6520 7261 6469 7573 290a 2020 2020  cle radius).    
+0000f110: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000f120: 635f 7820 3d20 7365 6c66 2e5f 7365 6172  c_x = self._sear
+0000f130: 6368 5b30 5d5b 2263 5f78 225d 0a20 2020  ch[0]["c_x"].   
+0000f140: 2020 2020 2063 5f79 203d 2073 656c 662e       c_y = self.
+0000f150: 5f73 6561 7263 685b 305d 5b22 635f 7922  _search[0]["c_y"
+0000f160: 5d0a 2020 2020 2020 2020 7261 6469 7573  ].        radius
+0000f170: 203d 2073 656c 662e 5f73 6561 7263 685b   = self._search[
+0000f180: 305d 5b22 7261 6469 7573 225d 0a20 2020  0]["radius"].   
+0000f190: 2020 2020 2072 6574 7572 6e20 2863 5f78       return (c_x
+0000f1a0: 2c20 635f 792c 2072 6164 6975 7329 0a0a  , c_y, radius)..
+0000f1b0: 2020 2020 6465 6620 6765 745f 6d69 6e5f      def get_min_
+0000f1c0: 464f 535f 656e 645f 706f 696e 7473 2873  FOS_end_points(s
+0000f1d0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+0000f1e0: 2247 6574 2074 6865 2065 7874 6572 6e61  "Get the externa
+0000f1f0: 6c20 626f 756e 6461 7279 2069 6e74 6572  l boundary inter
+0000f200: 7365 6374 696f 6e20 666f 7220 7468 6520  section for the 
+0000f210: 736c 6f70 6520 7468 6174 2067 6176 6520  slope that gave 
+0000f220: 7468 6520 6372 6974 6963 616c 2066 6163  the critical fac
+0000f230: 746f 7220 6f66 2073 6166 6574 792e 0a0a  tor of safety...
+0000f240: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
+0000f250: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
+0000f260: 2020 2020 2020 2020 7475 706c 650a 2020          tuple.  
+0000f270: 2020 2020 2020 2020 2020 7475 706c 6520            tuple 
+0000f280: 636f 6e74 6169 6e69 6e67 2028 6c65 6674  containing (left
+0000f290: 2063 6f6f 7264 696e 6174 652c 2072 6967   coordinate, rig
+0000f2a0: 6874 2063 6f6f 7264 696e 6174 6529 0a20  ht coordinate). 
+0000f2b0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000f2c0: 2020 206c 5f63 203d 2073 656c 662e 5f73     l_c = self._s
+0000f2d0: 6561 7263 685b 305d 5b22 6c5f 6322 5d0a  earch[0]["l_c"].
+0000f2e0: 2020 2020 2020 2020 725f 6320 3d20 7365          r_c = se
+0000f2f0: 6c66 2e5f 7365 6172 6368 5b30 5d5b 2272  lf._search[0]["r
+0000f300: 5f63 225d 0a20 2020 2020 2020 2072 6574  _c"].        ret
+0000f310: 7572 6e20 286c 5f63 2c20 725f 6329 0a0a  urn (l_c, r_c)..
+0000f320: 2020 2020 6465 6620 6765 745f 6578 7465      def get_exte
+0000f330: 726e 616c 5f79 5f69 6e74 6572 7365 6374  rnal_y_intersect
+0000f340: 696f 6e28 7365 6c66 2c20 7829 3a0a 2020  ion(self, x):.  
+0000f350: 2020 2020 2020 2222 2272 6574 7572 6e20        """return 
+0000f360: 7920 636f 6f72 6469 6e61 7465 206f 6620  y coordinate of 
+0000f370: 696e 7465 7273 6563 7469 6f6e 2077 6974  intersection wit
+0000f380: 6820 626f 756e 6461 7279 2066 6f72 2061  h boundary for a
+0000f390: 2067 6976 656e 2078 2222 220a 2020 2020   given x""".    
+0000f3a0: 2020 2020 6966 2078 203c 2030 206f 7220      if x < 0 or 
+0000f3b0: 7820 3e20 7365 6c66 2e5f 6578 7465 726e  x > self._extern
+0000f3c0: 616c 5f6c 656e 6774 683a 0a20 2020 2020  al_length:.     
+0000f3d0: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+0000f3e0: 6e65 0a20 2020 2020 2020 2023 2079 2069  ne.        # y i
+0000f3f0: 7320 6265 6c6f 7720 7468 6520 626f 7474  s below the bott
+0000f400: 6f6d 206f 6620 7468 6520 736c 6f70 650a  om of the slope.
+0000f410: 2020 2020 2020 2020 656c 6966 2078 203c          elif x <
+0000f420: 3d20 7365 6c66 2e5f 746f 705f 636f 6f72  = self._top_coor
+0000f430: 645b 305d 3a0a 2020 2020 2020 2020 2020  d[0]:.          
+0000f440: 2020 7265 7475 726e 2073 656c 662e 5f74    return self._t
+0000f450: 6f70 5f63 6f6f 7264 5b31 5d0a 2020 2020  op_coord[1].    
+0000f460: 2020 2020 656c 6966 2078 203e 3d20 7365      elif x >= se
+0000f470: 6c66 2e5f 626f 745f 636f 6f72 645b 305d  lf._bot_coord[0]
+0000f480: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0000f490: 7475 726e 2073 656c 662e 5f62 6f74 5f63  turn self._bot_c
+0000f4a0: 6f6f 7264 5b31 5d0a 2020 2020 2020 2020  oord[1].        
+0000f4b0: 2320 7920 6973 2061 626f 7665 2074 6865  # y is above the
+0000f4c0: 2062 6f74 746f 6d20 6f66 2074 6865 2073   bottom of the s
+0000f4d0: 6c6f 7065 0a20 2020 2020 2020 2065 6c73  lope.        els
+0000f4e0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0000f4f0: 6574 7572 6e20 7365 6c66 2e5f 746f 705f  eturn self._top_
+0000f500: 636f 6f72 645b 315d 202d 2028 7820 2d20  coord[1] - (x - 
+0000f510: 7365 6c66 2e5f 746f 705f 636f 6f72 645b  self._top_coord[
+0000f520: 305d 2920 2a20 7365 6c66 2e5f 6772 6164  0]) * self._grad
+0000f530: 6965 6e74 0a0a 2020 2020 6465 6620 6765  ient..    def ge
+0000f540: 745f 6578 7465 726e 616c 5f78 5f69 6e74  t_external_x_int
+0000f550: 6572 7365 6374 696f 6e28 7365 6c66 2c20  ersection(self, 
+0000f560: 7929 3a0a 2020 2020 2020 2020 2222 2272  y):.        """r
+0000f570: 6574 7572 6e20 7820 636f 6f72 6469 6e61  eturn x coordina
+0000f580: 7465 206f 6620 696e 7465 7273 6563 7469  te of intersecti
+0000f590: 6f6e 2077 6974 6820 626f 756e 6461 7279  on with boundary
+0000f5a0: 2066 6f72 2061 2067 6976 656e 2079 2222   for a given y""
+0000f5b0: 220a 2020 2020 2020 2020 2320 7920 6973  ".        # y is
+0000f5c0: 2062 656c 6f77 2074 6865 2062 6f74 746f   below the botto
+0000f5d0: 6d20 6f66 2074 6865 2073 6c6f 7065 0a20  m of the slope. 
+0000f5e0: 2020 2020 2020 2069 6620 7920 3c20 7365         if y < se
+0000f5f0: 6c66 2e5f 626f 745f 636f 6f72 645b 315d  lf._bot_coord[1]
+0000f600: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0000f610: 7475 726e 2073 656c 662e 5f65 7874 6572  turn self._exter
+0000f620: 6e61 6c5f 6c65 6e67 7468 0a0a 2020 2020  nal_length..    
+0000f630: 2020 2020 2320 7920 6973 2061 626f 7665      # y is above
+0000f640: 2074 6865 2062 6f74 746f 6d20 6f66 2074   the bottom of t
+0000f650: 6865 2073 6c6f 7065 0a20 2020 2020 2020  he slope.       
+0000f660: 2065 6c69 6620 7920 3c20 7365 6c66 2e5f   elif y < self._
+0000f670: 6578 7465 726e 616c 5f68 6569 6768 743a  external_height:
+0000f680: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000f690: 7572 6e20 7365 6c66 2e5f 746f 705f 636f  urn self._top_co
+0000f6a0: 6f72 645b 305d 202b 2028 7365 6c66 2e5f  ord[0] + (self._
+0000f6b0: 746f 705f 636f 6f72 645b 315d 202d 2079  top_coord[1] - y
+0000f6c0: 2920 2f20 7365 6c66 2e5f 6772 6164 6965  ) / self._gradie
+0000f6d0: 6e74 0a0a 2020 2020 2020 2020 656c 6966  nt..        elif
+0000f6e0: 2079 203d 3d20 7365 6c66 2e5f 626f 745f   y == self._bot_
+0000f6f0: 636f 6f72 645b 315d 3a0a 2020 2020 2020  coord[1]:.      
+0000f700: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000f710: 662e 5f62 6f74 5f63 6f6f 7264 5b30 5d0a  f._bot_coord[0].
+0000f720: 0a20 2020 2020 2020 2065 6c69 6620 7920  .        elif y 
+0000f730: 3d3d 2073 656c 662e 5f74 6f70 5f63 6f6f  == self._top_coo
+0000f740: 7264 5b31 5d3a 0a20 2020 2020 2020 2020  rd[1]:.         
+0000f750: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+0000f760: 746f 705f 636f 6f72 645b 305d 0a0a 2020  top_coord[0]..  
+0000f770: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000f780: 2020 2020 2020 2020 7265 7475 726e 204e          return N
+0000f790: 6f6e 650a 0a20 2020 2064 6566 2067 6574  one..    def get
+0000f7a0: 5f74 6f70 5f63 6f6f 7264 696e 6174 6573  _top_coordinates
+0000f7b0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000f7c0: 2222 2252 6574 7572 6e73 2074 6865 2074  """Returns the t
+0000f7d0: 6f70 2063 6f6f 7264 696e 6174 6520 6f66  op coordinate of
+0000f7e0: 2074 6865 2073 6c6f 7065 2e0a 0a20 2020   the slope...   
+0000f7f0: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
+0000f800: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
+0000f810: 2020 2020 2074 7570 6c65 0a20 2020 2020       tuple.     
+0000f820: 2020 2020 2020 2028 782c 7929 2063 6f6f         (x,y) coo
+0000f830: 7264 696e 6174 6520 6f66 2074 6865 2074  rdinate of the t
+0000f840: 6f70 206f 6620 7468 6520 736c 6f70 652e  op of the slope.
+0000f850: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000f860: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0000f870: 2e5f 746f 705f 636f 6f72 640a 0a20 2020  ._top_coord..   
+0000f880: 2064 6566 2067 6574 5f62 6f74 746f 6d5f   def get_bottom_
+0000f890: 636f 6f72 6469 6e61 7465 7328 7365 6c66  coordinates(self
+0000f8a0: 293a 0a20 2020 2020 2020 2022 2222 5265  ):.        """Re
+0000f8b0: 7475 726e 7320 7468 6520 626f 7474 6f6d  turns the bottom
+0000f8c0: 2063 6f6f 7264 696e 6174 6520 6f66 2074   coordinate of t
+0000f8d0: 6865 2073 6c6f 7065 2e0a 0a20 2020 2020  he slope...     
+0000f8e0: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
+0000f8f0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+0000f900: 2020 2074 7570 6c65 0a20 2020 2020 2020     tuple.       
+0000f910: 2020 2020 2028 782c 7929 2063 6f6f 7264       (x,y) coord
+0000f920: 696e 6174 6520 6f66 2074 6865 2062 6f74  inate of the bot
+0000f930: 746f 6d20 6f66 2074 6865 2073 6c6f 7065  tom of the slope
+0000f940: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+0000f950: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000f960: 662e 5f62 6f74 5f63 6f6f 7264 0a0a 2020  f._bot_coord..  
+0000f970: 2020 6465 6620 706c 6f74 5f62 6f75 6e64    def plot_bound
+0000f980: 6172 7928 7365 6c66 2c20 6d61 7465 7269  ary(self, materi
+0000f990: 616c 5f74 6162 6c65 3d54 7275 652c 206c  al_table=True, l
+0000f9a0: 6567 656e 643d 4661 6c73 6529 3a0a 2020  egend=False):.  
+0000f9b0: 2020 2020 2020 2222 2250 6c6f 7420 6578        """Plot ex
+0000f9c0: 7465 726e 616c 2062 6f75 6e64 6172 792c  ternal boundary,
+0000f9d0: 206d 6174 6572 6961 6c73 2c20 6c69 6d69   materials, limi
+0000f9e0: 7473 2c20 6c6f 6164 696e 6720 616e 6420  ts, loading and 
+0000f9f0: 7761 7465 7220 666f 7220 6d6f 6465 6c2e  water for model.
+0000fa00: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+0000fa10: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+0000fa20: 2d0a 2020 2020 2020 2020 706c 6f74 6c79  -.        plotly
+0000fa30: 2066 6967 7572 650a 0a20 2020 2020 2020   figure..       
+0000fa40: 2022 2222 0a20 2020 2020 2020 2023 2064   """.        # d
+0000fa50: 7261 7720 7468 6520 6578 7465 726e 616c  raw the external
+0000fa60: 2062 6f75 6e64 6172 790a 2020 2020 2020   boundary.      
+0000fa70: 2020 785f 203d 205b 7820 666f 7220 782c    x_ = [x for x,
+0000fa80: 2079 2069 6e20 7365 6c66 2e5f 6578 7465   y in self._exte
+0000fa90: 726e 616c 5f62 6f75 6e64 6172 795d 0a20  rnal_boundary]. 
+0000faa0: 2020 2020 2020 2079 5f20 3d20 5b79 2066         y_ = [y f
+0000fab0: 6f72 2078 2c20 7920 696e 2073 656c 662e  or x, y in self.
+0000fac0: 5f65 7874 6572 6e61 6c5f 626f 756e 6461  _external_bounda
+0000fad0: 7279 5d0a 2020 2020 2020 2020 6669 6720  ry].        fig 
+0000fae0: 3d20 676f 2e46 6967 7572 6528 676f 2e53  = go.Figure(go.S
+0000faf0: 6361 7474 6572 2878 3d6c 6973 7428 785f  catter(x=list(x_
+0000fb00: 292c 2079 3d6c 6973 7428 795f 292c 206d  ), y=list(y_), m
+0000fb10: 6f64 653d 226c 696e 6573 222c 206e 616d  ode="lines", nam
+0000fb20: 653d 2222 2929 0a0a 2020 2020 2020 2020  e=""))..        
+0000fb30: 6669 672e 7570 6461 7465 5f6c 6179 6f75  fig.update_layou
+0000fb40: 7428 7769 6474 683d 3230 3030 2c20 6865  t(width=2000, he
+0000fb50: 6967 6874 3d31 3230 3029 0a0a 2020 2020  ight=1200)..    
+0000fb60: 2020 2020 2320 666f 6c6c 6f77 696e 6720      # following 
+0000fb70: 6d61 6b65 7320 7375 7265 2078 2061 6e64  makes sure x and
+0000fb80: 2079 2061 7265 2073 6361 6c65 6420 7468   y are scaled th
+0000fb90: 6520 7361 6d65 2c20 736f 2074 6861 740a  e same, so that.
+0000fba0: 2020 2020 2020 2020 2320 6d6f 6465 6c20          # model 
+0000fbb0: 6361 6e20 6265 2069 6e74 6572 7072 6574  can be interpret
+0000fbc0: 7465 6420 7072 6f70 6572 6c79 0a20 2020  ted properly.   
+0000fbd0: 2020 2020 2066 6967 2e75 7064 6174 655f       fig.update_
+0000fbe0: 7961 7865 7328 0a20 2020 2020 2020 2020  yaxes(.         
+0000fbf0: 2020 2073 6361 6c65 616e 6368 6f72 3d22     scaleanchor="
+0000fc00: 7822 2c0a 2020 2020 2020 2020 2020 2020  x",.            
+0000fc10: 7363 616c 6572 6174 696f 3d31 2c0a 2020  scaleratio=1,.  
+0000fc20: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0000fc30: 2023 2064 6f6e 7420 7368 6f77 206c 6567   # dont show leg
+0000fc40: 656e 640a 2020 2020 2020 2020 6669 672e  end.        fig.
+0000fc50: 7570 6461 7465 5f6c 6179 6f75 7428 0a20  update_layout(. 
+0000fc60: 2020 2020 2020 2020 2020 2073 686f 776c             showl
+0000fc70: 6567 656e 643d 4661 6c73 652c 0a20 2020  egend=False,.   
+0000fc80: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+0000fc90: 2320 6966 2074 6865 7265 2061 7265 206e  # if there are n
+0000fca0: 6f20 6d61 7465 7269 616c 7320 6a75 7374  o materials just
+0000fcb0: 2072 6574 7572 6e20 616e 2065 6d70 7479   return an empty
+0000fcc0: 2073 6865 6c6c 0a20 2020 2020 2020 2069   shell.        i
+0000fcd0: 6620 6e6f 7420 7365 6c66 2e5f 6d61 7465  f not self._mate
+0000fce0: 7269 616c 733a 0a20 2020 2020 2020 2020  rials:.         
+0000fcf0: 2020 2072 6574 7572 6e20 6669 670a 0a20     return fig.. 
+0000fd00: 2020 2020 2020 2023 2067 6574 2074 6865         # get the
+0000fd10: 2070 6f69 6e74 7320 7265 7072 6573 656e   points represen
+0000fd20: 7469 6e67 2074 6865 2074 6f70 206c 696e  ting the top lin
+0000fd30: 6520 6f66 2074 6865 206d 6f64 656c 0a20  e of the model. 
+0000fd40: 2020 2020 2020 2023 2074 6f20 6865 6c70         # to help
+0000fd50: 2077 6974 6820 6472 6177 696e 6720 6d61   with drawing ma
+0000fd60: 7465 7269 616c 730a 2020 2020 2020 2020  terials.        
+0000fd70: 746f 7020 3d20 7365 6c66 2e5f 6578 7465  top = self._exte
+0000fd80: 726e 616c 5f62 6f75 6e64 6172 795b 313a  rnal_boundary[1:
+0000fd90: 335d 0a0a 2020 2020 2020 2020 2320 6c65  3]..        # le
+0000fda0: 6e67 7468 206f 6620 6d6f 6465 6c20 286d  ngth of model (m
+0000fdb0: 6178 2078 2063 6f6f 7264 696e 6174 6529  ax x coordinate)
+0000fdc0: 0a20 2020 2020 2020 2074 6f74 5f6c 203d  .        tot_l =
+0000fdd0: 2073 656c 662e 5f65 7874 6572 6e61 6c5f   self._external_
+0000fde0: 6c65 6e67 7468 0a20 2020 2020 2020 206e  length.        n
+0000fdf0: 756d 5f6d 6174 6572 6961 6c73 203d 206c  um_materials = l
+0000fe00: 656e 2873 656c 662e 5f6d 6174 6572 6961  en(self._materia
+0000fe10: 6c73 290a 0a20 2020 2020 2020 2023 206c  ls)..        # l
+0000fe20: 6f6f 7020 7468 726f 7567 6820 6d61 7465  oop through mate
+0000fe30: 7269 616c 730a 2020 2020 2020 2020 666f  rials.        fo
+0000fe40: 7220 692c 206d 2069 6e20 656e 756d 6572  r i, m in enumer
+0000fe50: 6174 6528 7365 6c66 2e5f 6d61 7465 7269  ate(self._materi
+0000fe60: 616c 7329 3a0a 2020 2020 2020 2020 2020  als):.          
+0000fe70: 2020 2320 6765 7420 7265 6665 7265 6e63    # get referenc
+0000fe80: 6520 6c65 7665 6c20 2879 2063 6f6f 7264  e level (y coord
+0000fe90: 696e 6174 6529 2066 6f72 206d 6174 6572  inate) for mater
+0000fea0: 6961 6c0a 2020 2020 2020 2020 2020 2020  ial.            
+0000feb0: 7920 3d20 6d2e 524c 0a20 2020 2020 2020  y = m.RL.       
+0000fec0: 2020 2020 2078 203d 2073 656c 662e 6765       x = self.ge
+0000fed0: 745f 6578 7465 726e 616c 5f78 5f69 6e74  t_external_x_int
+0000fee0: 6572 7365 6374 696f 6e28 7929 0a0a 2020  ersection(y)..  
+0000fef0: 2020 2020 2020 2020 2020 6c69 6e65 203d            line =
+0000ff00: 205b 2830 2c20 7929 2c20 2878 2c20 7929   [(0, y), (x, y)
+0000ff10: 5d0a 0a20 2020 2020 2020 2020 2020 2023  ]..            #
+0000ff20: 2069 6620 7468 6520 626f 7420 736c 6f70   if the bot slop
+0000ff30: 6520 636f 6f72 6469 6e61 7465 2069 7320  e coordinate is 
+0000ff40: 6265 7477 6565 6e20 7468 6520 626f 756e  between the boun
+0000ff50: 6473 206f 6620 7468 6520 6d61 7465 7269  ds of the materi
+0000ff60: 616c 0a20 2020 2020 2020 2020 2020 2023  al.            #
+0000ff70: 204f 5220 4c41 5354 206d 6174 6572 6961   OR LAST materia
+0000ff80: 6c20 616e 6420 6162 6f76 6520 6e65 6564  l and above need
+0000ff90: 2074 6f20 6472 6177 2061 2062 6974 2064   to draw a bit d
+0000ffa0: 6966 6665 7265 6e74 6c79 0a0a 2020 2020  ifferently..    
+0000ffb0: 2020 2020 2020 2020 6973 5f6c 6173 7420          is_last 
+0000ffc0: 3d20 6920 3d3d 206e 756d 5f6d 6174 6572  = i == num_mater
+0000ffd0: 6961 6c73 202d 2031 0a0a 2020 2020 2020  ials - 1..      
+0000ffe0: 2020 2020 2020 6966 2028 0a20 2020 2020        if (.     
+0000fff0: 2020 2020 2020 2020 2020 2074 6f70 5b31             top[1
+00010000: 5d5b 315d 203e 3d20 7365 6c66 2e5f 626f  ][1] >= self._bo
+00010010: 745f 636f 6f72 645b 315d 2061 6e64 206c  t_coord[1] and l
+00010020: 696e 655b 315d 5b31 5d20 3c20 7365 6c66  ine[1][1] < self
+00010030: 2e5f 626f 745f 636f 6f72 645b 315d 0a20  ._bot_coord[1]. 
+00010040: 2020 2020 2020 2020 2020 2029 206f 7220             ) or 
+00010050: 2869 735f 6c61 7374 2061 6e64 2074 6f70  (is_last and top
+00010060: 5b31 5d5b 315d 203e 2073 656c 662e 5f62  [1][1] > self._b
+00010070: 6f74 5f63 6f6f 7264 5b31 5d29 3a0a 2020  ot_coord[1]):.  
+00010080: 2020 2020 2020 2020 2020 2020 2020 746f                to
+00010090: 702e 6170 7065 6e64 2873 656c 662e 5f62  p.append(self._b
+000100a0: 6f74 5f63 6f6f 7264 290a 2020 2020 2020  ot_coord).      
+000100b0: 2020 2020 2020 2020 2020 746f 702e 6170            top.ap
+000100c0: 7065 6e64 2828 746f 745f 6c2c 2073 656c  pend((tot_l, sel
+000100d0: 662e 5f62 6f74 5f63 6f6f 7264 5b31 5d29  f._bot_coord[1])
+000100e0: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
+000100f0: 2069 6620 7765 2061 7265 2061 7420 7468   if we are at th
+00010100: 6520 6c61 7374 206d 6174 6572 6961 6c20  e last material 
+00010110: 6d61 6b65 2074 6865 2062 6f74 746f 6d20  make the bottom 
+00010120: 7468 6520 626f 7474 6f6d 206f 6620 7468  the bottom of th
+00010130: 6520 6d6f 6465 6c0a 2020 2020 2020 2020  e model.        
+00010140: 2020 2020 6966 2069 203d 3d20 6e75 6d5f      if i == num_
+00010150: 6d61 7465 7269 616c 7320 2d20 313a 0a20  materials - 1:. 
+00010160: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+00010170: 6f74 203d 2073 656c 662e 5f65 7874 6572  ot = self._exter
+00010180: 6e61 6c5f 626f 756e 6461 7279 5b2d 323a  nal_boundary[-2:
+00010190: 5d0a 2020 2020 2020 2020 2020 2020 656c  ].            el
+000101a0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000101b0: 2020 2020 626f 7420 3d20 6c69 6e65 0a0a      bot = line..
+000101c0: 2020 2020 2020 2020 2020 2020 2320 6368              # ch
+000101d0: 616e 6765 2062 6f74 746f 6d20 636f 6f72  ange bottom coor
+000101e0: 6469 6e61 7465 7320 746f 2062 6520 7269  dinates to be ri
+000101f0: 6768 7420 746f 206c 6566 740a 2020 2020  ght to left.    
+00010200: 2020 2020 2020 2020 2320 736f 2070 6f69          # so poi
+00010210: 6e74 7320 6172 6520 6172 7261 6e67 6564  nts are arranged
+00010220: 2063 6c6f 636b 7769 7365 2069 6e20 6120   clockwise in a 
+00010230: 6369 7263 6c65 0a20 2020 2020 2020 2020  circle.         
+00010240: 2020 2062 6f74 203d 2073 6f72 7465 6428     bot = sorted(
+00010250: 626f 742c 2072 6576 6572 7365 3d54 7275  bot, reverse=Tru
+00010260: 6529 0a0a 2020 2020 2020 2020 2020 2020  e)..            
+00010270: 2320 6765 7420 636f 6f72 6469 6e61 7465  # get coordinate
+00010280: 730a 2020 2020 2020 2020 2020 2020 636f  s.            co
+00010290: 6f72 6473 203d 2074 6f70 202b 2062 6f74  ords = top + bot
+000102a0: 0a20 2020 2020 2020 2020 2020 2078 5f20  .            x_ 
+000102b0: 3d20 5b61 5b30 5d20 666f 7220 6120 696e  = [a[0] for a in
+000102c0: 2063 6f6f 7264 735d 0a20 2020 2020 2020   coords].       
+000102d0: 2020 2020 2079 5f20 3d20 5b61 5b31 5d20       y_ = [a[1] 
+000102e0: 666f 7220 6120 696e 2063 6f6f 7264 735d  for a in coords]
+000102f0: 0a0a 2020 2020 2020 2020 2020 2020 6669  ..            fi
+00010300: 672e 6164 645f 7472 6163 6528 0a20 2020  g.add_trace(.   
+00010310: 2020 2020 2020 2020 2020 2020 2067 6f2e               go.
+00010320: 5363 6174 7465 7228 0a20 2020 2020 2020  Scatter(.       
+00010330: 2020 2020 2020 2020 2020 2020 2078 3d6c               x=l
+00010340: 6973 7428 785f 292c 0a20 2020 2020 2020  ist(x_),.       
+00010350: 2020 2020 2020 2020 2020 2020 2079 3d6c               y=l
+00010360: 6973 7428 795f 292c 0a20 2020 2020 2020  ist(y_),.       
+00010370: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
+00010380: 653d 226c 696e 6573 222c 0a20 2020 2020  e="lines",.     
+00010390: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+000103a0: 6574 613d 5b6d 2e75 6e69 745f 7765 6967  eta=[m.unit_weig
+000103b0: 6874 2c20 6d2e 636f 6865 7369 6f6e 2c20  ht, m.cohesion, 
+000103c0: 6d2e 6672 6963 7469 6f6e 5f61 6e67 6c65  m.friction_angle
+000103d0: 2c20 6d2e 6e61 6d65 5d2c 0a20 2020 2020  , m.name],.     
+000103e0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000103f0: 696c 6c3d 2274 6f73 656c 6622 2c0a 2020  ill="toself",.  
+00010400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010410: 2020 6e61 6d65 3d28 0a20 2020 2020 2020    name=(.       
+00010420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010430: 2066 227b 6d2e 6e61 6d65 7d3c 6272 3e22   f"{m.name}<br>"
+00010440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010450: 2020 2020 2020 2020 2066 22ce b33a 207b           f"..: {
+00010460: 6d2e 756e 6974 5f77 6569 6768 747d 206b  m.unit_weight} k
+00010470: 4e2f 6d33 3c62 723e 220a 2020 2020 2020  N/m3<br>".      
+00010480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010490: 2020 6622 633a 207b 6d2e 636f 6865 7369    f"c: {m.cohesi
+000104a0: 6f6e 7d20 6b50 613c 6272 3e22 0a20 2020  on} kPa<br>".   
+000104b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000104c0: 2020 2020 2066 22cf 953a 207b 6d2e 6672       f"..: {m.fr
+000104d0: 6963 7469 6f6e 5f61 6e67 6c65 7d20 6465  iction_angle} de
+000104e0: 6772 6565 7322 0a20 2020 2020 2020 2020  grees".         
+000104f0: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
+00010500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010510: 2020 686f 7665 7274 656d 706c 6174 653d    hovertemplate=
+00010520: 2222 2c0a 2020 2020 2020 2020 2020 2020  "",.            
+00010530: 2020 2020 2020 2020 6669 6c6c 636f 6c6f          fillcolo
+00010540: 723d 6d2e 636f 6c6f 722c 0a20 2020 2020  r=m.color,.     
+00010550: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00010560: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+00010570: 2020 2020 2020 2020 2320 7365 7420 7468          # set th
+00010580: 6520 6e65 7720 746f 7020 6173 2074 6865  e new top as the
+00010590: 2062 6f74 746f 6d2c 2073 6f72 7420 746f   bottom, sort to
+000105a0: 2070 7574 2069 7420 6261 636b 0a20 2020   put it back.   
+000105b0: 2020 2020 2020 2020 2023 2074 6f20 6c65           # to le
+000105c0: 6674 2074 6f20 7269 6768 7420 6f72 6465  ft to right orde
+000105d0: 720a 2020 2020 2020 2020 2020 2020 626f  r.            bo
+000105e0: 742e 736f 7274 2829 0a20 2020 2020 2020  t.sort().       
+000105f0: 2020 2020 2074 6f70 203d 2062 6f74 0a0a       top = bot..
+00010600: 2020 2020 2020 2020 6966 206d 6174 6572          if mater
+00010610: 6961 6c5f 7461 626c 653a 0a20 2020 2020  ial_table:.     
+00010620: 2020 2020 2020 2066 6967 203d 2073 656c         fig = sel
+00010630: 662e 5f70 6c6f 745f 6d61 7465 7269 616c  f._plot_material
+00010640: 5f74 6162 6c65 2866 6967 290a 0a20 2020  _table(fig)..   
+00010650: 2020 2020 2069 6620 6c65 6765 6e64 3a0a       if legend:.
+00010660: 2020 2020 2020 2020 2020 2020 6669 6720              fig 
+00010670: 3d20 7365 6c66 2e5f 706c 6f74 5f46 4f53  = self._plot_FOS
+00010680: 5f6c 6567 656e 6428 6669 6729 0a0a 2020  _legend(fig)..  
+00010690: 2020 2020 2020 666f 7220 7564 6c20 696e        for udl in
+000106a0: 2073 656c 662e 5f75 646c 733a 0a20 2020   self._udls:.   
+000106b0: 2020 2020 2020 2020 2066 6967 203d 2073           fig = s
+000106c0: 656c 662e 5f70 6c6f 745f 7564 6c28 6669  elf._plot_udl(fi
+000106d0: 672c 2075 646c 290a 0a20 2020 2020 2020  g, udl)..       
+000106e0: 2066 6f72 206c 6c20 696e 2073 656c 662e   for ll in self.
+000106f0: 5f6c 6c73 3a0a 2020 2020 2020 2020 2020  _lls:.          
+00010700: 2020 6669 6720 3d20 7365 6c66 2e5f 706c    fig = self._pl
+00010710: 6f74 5f6c 6c28 6669 672c 206c 6c29 0a0a  ot_ll(fig, ll)..
+00010720: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00010730: 5f77 6174 6572 5f52 4c3a 0a20 2020 2020  _water_RL:.     
+00010740: 2020 2020 2020 2066 6967 203d 2073 656c         fig = sel
+00010750: 662e 5f70 6c6f 745f 7761 7465 7228 6669  f._plot_water(fi
+00010760: 6729 0a0a 2020 2020 2020 2020 6669 6720  g)..        fig 
+00010770: 3d20 7365 6c66 2e5f 706c 6f74 5f6c 696d  = self._plot_lim
+00010780: 6974 7328 6669 6729 0a0a 2020 2020 2020  its(fig)..      
+00010790: 2020 7265 7475 726e 2066 6967 0a0a 2020    return fig..  
+000107a0: 2020 6465 6620 706c 6f74 5f63 7269 7469    def plot_criti
+000107b0: 6361 6c28 7365 6c66 2c20 6d61 7465 7269  cal(self, materi
+000107c0: 616c 5f74 6162 6c65 3d54 7275 652c 206c  al_table=True, l
+000107d0: 6567 656e 643d 4661 6c73 6529 3a0a 2020  egend=False):.  
+000107e0: 2020 2020 2020 2222 2250 6c6f 7420 6372        """Plot cr
+000107f0: 6974 6963 616c 2073 6c6f 7065 2028 692e  itical slope (i.
+00010800: 652e 2073 6c6f 7065 2077 6974 6820 6c6f  e. slope with lo
+00010810: 7765 7374 2046 4f53 290a 0a20 2020 2020  west FOS)..     
+00010820: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
+00010830: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+00010840: 2020 2050 6c6f 746c 7920 6669 6775 7265     Plotly figure
+00010850: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00010860: 2020 2020 2066 6967 203d 2073 656c 662e       fig = self.
+00010870: 706c 6f74 5f62 6f75 6e64 6172 7928 6d61  plot_boundary(ma
+00010880: 7465 7269 616c 5f74 6162 6c65 3d6d 6174  terial_table=mat
+00010890: 6572 6961 6c5f 7461 626c 652c 206c 6567  erial_table, leg
+000108a0: 656e 643d 6c65 6765 6e64 290a 0a20 2020  end=legend)..   
+000108b0: 2020 2020 2046 4f53 203d 2073 656c 662e       FOS = self.
+000108c0: 5f73 6561 7263 685b 305d 5b22 464f 5322  _search[0]["FOS"
+000108d0: 5d0a 2020 2020 2020 2020 635f 7820 3d20  ].        c_x = 
+000108e0: 7365 6c66 2e5f 7365 6172 6368 5b30 5d5b  self._search[0][
+000108f0: 2263 5f78 225d 0a20 2020 2020 2020 2063  "c_x"].        c
+00010900: 5f79 203d 2073 656c 662e 5f73 6561 7263  _y = self._searc
+00010910: 685b 305d 5b22 635f 7922 5d0a 2020 2020  h[0]["c_y"].    
+00010920: 2020 2020 7261 6469 7573 203d 2073 656c      radius = sel
+00010930: 662e 5f73 6561 7263 685b 305d 5b22 7261  f._search[0]["ra
+00010940: 6469 7573 225d 0a20 2020 2020 2020 206c  dius"].        l
+00010950: 5f63 203d 2073 656c 662e 5f73 6561 7263  _c = self._searc
+00010960: 685b 305d 5b22 6c5f 6322 5d0a 2020 2020  h[0]["l_c"].    
+00010970: 2020 2020 725f 6320 3d20 7365 6c66 2e5f      r_c = self._
+00010980: 7365 6172 6368 5b30 5d5b 2272 5f63 225d  search[0]["r_c"]
+00010990: 0a0a 2020 2020 2020 2020 6669 6720 3d20  ..        fig = 
+000109a0: 7365 6c66 2e5f 706c 6f74 5f66 6169 6c75  self._plot_failu
+000109b0: 7265 5f70 6c61 6e65 280a 2020 2020 2020  re_plane(.      
+000109c0: 2020 2020 2020 6669 672c 2063 5f78 2c20        fig, c_x, 
+000109d0: 635f 792c 2072 6164 6975 732c 206c 5f63  c_y, radius, l_c
+000109e0: 2c20 725f 632c 2046 4f53 3d46 4f53 2c20  , r_c, FOS=FOS, 
+000109f0: 7368 6f77 5f63 656e 7465 723d 5472 7565  show_center=True
+00010a00: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+00010a10: 2020 2072 6574 7572 6e20 6669 670a 0a20     return fig.. 
+00010a20: 2020 2064 6566 2070 6c6f 745f 616c 6c5f     def plot_all_
+00010a30: 706c 616e 6573 2873 656c 662c 206d 6178  planes(self, max
+00010a40: 5f66 6f73 3a20 666c 6f61 7420 3d20 352c  _fos: float = 5,
+00010a50: 206d 6174 6572 6961 6c5f 7461 626c 653d   material_table=
+00010a60: 5472 7565 2c20 6c65 6765 6e64 3d54 7275  True, legend=Tru
+00010a70: 6529 3a0a 2020 2020 2020 2020 2222 2270  e):.        """p
+00010a80: 6c6f 7420 6d75 6c74 6970 6c65 2066 6169  lot multiple fai
+00010a90: 6c75 7265 2070 6c61 6e65 7320 696e 2074  lure planes in t
+00010aa0: 6865 2073 616d 6520 706c 6f74 0a0a 2020  he same plot..  
+00010ab0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+00010ac0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00010ad0: 2d2d 2d0a 2020 2020 2020 2020 6d61 785f  ---.        max_
+00010ae0: 666f 7320 3a20 666c 6f61 742c 206f 7074  fos : float, opt
+00010af0: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
+00010b00: 2020 6d61 7869 6d75 6d20 6661 6374 6f72    maximum factor
+00010b10: 206f 6620 7361 6665 7479 2074 6f20 6469   of safety to di
+00010b20: 7370 6c61 7920 666f 7220 706c 616e 6573  splay for planes
+00010b30: 2c0a 2020 2020 2020 2020 2020 2020 6279  ,.            by
+00010b40: 2064 6566 6175 6c74 2035 2e0a 0a20 2020   default 5...   
+00010b50: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
+00010b60: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
+00010b70: 2020 2020 2070 6c6f 746c 7920 6669 6775       plotly figu
+00010b80: 7265 0a0a 2020 2020 2020 2020 2222 220a  re..        """.
+00010b90: 0a20 2020 2020 2020 2066 6967 203d 2073  .        fig = s
+00010ba0: 656c 662e 706c 6f74 5f63 7269 7469 6361  elf.plot_critica
+00010bb0: 6c28 6d61 7465 7269 616c 5f74 6162 6c65  l(material_table
+00010bc0: 3d6d 6174 6572 6961 6c5f 7461 626c 652c  =material_table,
+00010bd0: 206c 6567 656e 643d 6c65 6765 6e64 290a   legend=legend).
+00010be0: 0a20 2020 2020 2020 2066 6967 203d 2073  .        fig = s
+00010bf0: 656c 662e 5f70 6c6f 745f 464f 535f 6c65  elf._plot_FOS_le
+00010c00: 6765 6e64 2866 6967 290a 0a20 2020 2020  gend(fig)..     
+00010c10: 2020 2023 204a 4220 3230 2e30 342e 3232     # JB 20.04.22
+00010c20: 202d 2027 6861 636b 6564 2720 696e 746f   - 'hacked' into
+00010c30: 2068 6f77 2070 6c6f 746c 7920 776f 726b   how plotly work
+00010c40: 7320 746f 206d 616b 6520 6661 7374 6572  s to make faster
+00010c50: 0a20 2020 2020 2020 2023 2075 6c74 696d  .        # ultim
+00010c60: 6174 656c 7920 6e6f 7420 7665 7279 2072  ately not very r
+00010c70: 6561 6469 626c 6520 6170 7072 6f61 6368  eadible approach
+00010c80: 2063 6f6d 7061 7265 6420 746f 2074 6865   compared to the
+00010c90: 206f 6c64 2061 7070 726f 6163 680a 2020   old approach.  
+00010ca0: 2020 2020 2020 2320 686f 7765 7665 7220        # however 
+00010cb0: 6f6c 6420 6170 7072 6f61 6368 2077 6173  old approach was
+00010cc0: 2074 6f6f 2073 6c6f 770a 2020 2020 2020   too slow.      
+00010cd0: 2020 7472 6163 6573 203d 205b 5d0a 0a20    traces = [].. 
+00010ce0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+00010cf0: 7471 646d 2873 656c 662e 5f73 6561 7263  tqdm(self._searc
+00010d00: 6829 3a0a 2020 2020 2020 2020 2020 2020  h):.            
+00010d10: 464f 5320 3d20 695b 2246 4f53 225d 0a20  FOS = i["FOS"]. 
+00010d20: 2020 2020 2020 2020 2020 2069 6620 6d61             if ma
+00010d30: 785f 666f 7320 6973 204e 6f6e 6520 6f72  x_fos is None or
+00010d40: 2046 4f53 203c 206d 6178 5f66 6f73 3a0a   FOS < max_fos:.
+00010d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d60: 635f 7820 3d20 695b 2263 5f78 225d 0a20  c_x = i["c_x"]. 
+00010d70: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00010d80: 5f79 203d 2069 5b22 635f 7922 5d0a 2020  _y = i["c_y"].  
+00010d90: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+00010da0: 6469 7573 203d 2069 5b22 7261 6469 7573  dius = i["radius
+00010db0: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+00010dc0: 2020 206c 5f63 203d 2069 5b22 6c5f 6322     l_c = i["l_c"
+00010dd0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00010de0: 2020 725f 6320 3d20 695b 2272 5f63 225d    r_c = i["r_c"]
+00010df0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010e00: 2020 636f 6c6f 7220 3d20 434f 4c4f 5552    color = COLOUR
+00010e10: 5f46 4f53 5f44 4943 545b 6d69 6e28 726f  _FOS_DICT[min(ro
+00010e20: 756e 6428 464f 532c 2031 292c 204d 4158  und(FOS, 1), MAX
+00010e30: 5f43 4f4c 4f55 525f 4b45 5929 5d0a 0a20  _COLOUR_KEY)].. 
+00010e40: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00010e50: 2067 656e 6572 6174 6520 706f 696e 7473   generate points
+00010e60: 2066 6f72 2063 6972 636c 652c 2067 656e   for circle, gen
+00010e70: 6572 6174 6573 2070 6f69 6e74 7320 6f6e  erates points on
+00010e80: 6c79 2061 6c6f 6e67 2062 6f74 746f 6d20  ly along bottom 
+00010e90: 6861 6c66 206f 6620 6369 7263 6c65 0a20  half of circle. 
+00010ea0: 2020 2020 2020 2020 2020 2020 2020 2078                 x
+00010eb0: 2c20 7920 3d20 7574 696c 6974 6965 732e  , y = utilities.
+00010ec0: 6765 6e65 7261 7465 5f63 6972 636c 655f  generate_circle_
+00010ed0: 636f 6f72 6469 6e61 7465 7328 635f 782c  coordinates(c_x,
+00010ee0: 2063 5f79 2c20 7261 6469 7573 290a 0a20   c_y, radius).. 
+00010ef0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00010f00: 2065 6d70 7479 2076 6563 746f 7273 2066   empty vectors f
+00010f10: 6f72 2063 6972 636c 6520 706f 696e 7473  or circle points
+00010f20: 2074 6861 7420 7765 2077 696c 6c20 6163   that we will ac
+00010f30: 7475 616c 6c79 2069 6e63 6c75 6465 0a20  tually include. 
+00010f40: 2020 2020 2020 2020 2020 2020 2020 2078                 x
+00010f50: 5f20 3d20 5b5d 0a20 2020 2020 2020 2020  _ = [].         
+00010f60: 2020 2020 2020 2079 5f20 3d20 5b5d 0a0a         y_ = []..
+00010f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f80: 2320 3635 206c 6f6e 6720 6c69 7374 2062  # 65 long list b
+00010f90: 7574 2074 6865 206c 6173 7420 6861 6c66  ut the last half
+00010fa0: 206f 6620 706f 696e 7473 2061 7265 2066   of points are f
+00010fb0: 6f72 2074 6865 2074 6f70 2068 616c 6620  or the top half 
+00010fc0: 6f66 0a20 2020 2020 2020 2020 2020 2020  of.             
+00010fd0: 2020 2023 2063 6972 636c 6520 616e 6420     # circle and 
+00010fe0: 736f 2077 696c 6c20 6e65 7665 7220 6163  so will never ac
+00010ff0: 7475 616c 6c79 2062 6520 7265 7175 6972  tually be requir
+00011000: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
+00011010: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+00011020: 6765 286c 656e 2878 2929 3a0a 2020 2020  ge(len(x)):.    
+00011030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011040: 2320 7820 636f 6f72 6469 6e61 7465 2073  # x coordinate s
+00011050: 686f 756c 6420 6265 2062 6574 7765 656e  hould be between
+00011060: 206c 6566 7420 616e 6420 7269 6768 740a   left and right.
+00011070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011080: 2020 2020 2320 6e6f 7465 2066 6f72 2079      # note for y
+00011090: 2c20 7368 6f75 6c64 2062 6520 6c65 7373  , should be less
+000110a0: 2074 6861 6e20 6c65 6674 2079 2062 7574   than left y but
+000110b0: 2063 616e 2073 746f 6f70 0a20 2020 2020   can stoop.     
+000110c0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+000110d0: 2062 656c 6f77 2072 6967 6874 2069 0a20   below right i. 
+000110e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000110f0: 2020 2069 6620 785b 695d 203c 3d20 725f     if x[i] <= r_
+00011100: 635b 305d 2061 6e64 2078 5b69 5d20 3e3d  c[0] and x[i] >=
+00011110: 206c 5f63 5b30 5d20 616e 6420 795b 695d   l_c[0] and y[i]
+00011120: 203c 3d20 6c5f 635b 315d 3a0a 2020 2020   <= l_c[1]:.    
+00011130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011140: 2020 2020 785f 2e61 7070 656e 6428 785b      x_.append(x[
+00011150: 695d 290a 2020 2020 2020 2020 2020 2020  i]).            
+00011160: 2020 2020 2020 2020 2020 2020 795f 2e61              y_.a
+00011170: 7070 656e 6428 795b 695d 290a 0a20 2020  ppend(y[i])..   
+00011180: 2020 2020 2020 2020 2020 2020 2078 5f20               x_ 
+00011190: 3d20 5b6c 5f63 5b30 5d5d 202b 2078 5f20  = [l_c[0]] + x_ 
+000111a0: 2b20 5b72 5f63 5b30 5d5d 0a20 2020 2020  + [r_c[0]].     
+000111b0: 2020 2020 2020 2020 2020 2079 5f20 3d20             y_ = 
+000111c0: 5b6c 5f63 5b31 5d5d 202b 2079 5f20 2b20  [l_c[1]] + y_ + 
+000111d0: 5b72 5f63 5b31 5d5d 0a0a 2020 2020 2020  [r_c[1]]..      
+000111e0: 2020 2020 2020 2020 2020 7472 6163 6573            traces
+000111f0: 2e61 7070 656e 6428 0a20 2020 2020 2020  .append(.       
+00011200: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
+00011210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011220: 2020 2020 2020 2022 686f 7665 7274 656d         "hovertem
+00011230: 706c 6174 6522 3a20 2225 7b6d 6574 615b  plate": "%{meta[
+00011240: 305d 7d22 2c0a 2020 2020 2020 2020 2020  0]}",.          
+00011250: 2020 2020 2020 2020 2020 2020 2020 226c                "l
+00011260: 696e 6522 3a20 7b22 636f 6c6f 7222 3a20  ine": {"color": 
+00011270: 636f 6c6f 727d 2c0a 2020 2020 2020 2020  color},.        
+00011280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011290: 226d 6574 6122 3a20 5b72 6f75 6e64 2846  "meta": [round(F
+000112a0: 4f53 2c20 3329 5d2c 0a20 2020 2020 2020  OS, 3)],.       
+000112b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112c0: 2022 6d6f 6465 223a 2022 6c69 6e65 7322   "mode": "lines"
+000112d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000112e0: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
+000112f0: 3a20 2222 2c0a 2020 2020 2020 2020 2020  : "",.          
+00011300: 2020 2020 2020 2020 2020 2020 2020 2278                "x
+00011310: 223a 2078 5f2c 0a20 2020 2020 2020 2020  ": x_,.         
+00011320: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00011330: 7922 3a20 795f 2c0a 2020 2020 2020 2020  y": y_,.        
+00011340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011350: 2274 7970 6522 3a20 2273 6361 7474 6572  "type": "scatter
+00011360: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00011370: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00011380: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+00011390: 2020 2020 7472 6163 6573 2e72 6576 6572      traces.rever
+000113a0: 7365 2829 0a0a 2020 2020 2020 2020 7465  se()..        te
+000113b0: 6d70 203d 2066 6967 2e74 6f5f 6469 6374  mp = fig.to_dict
+000113c0: 2829 0a20 2020 2020 2020 2074 656d 705b  ().        temp[
+000113d0: 2264 6174 6122 5d20 3d20 7475 706c 6528  "data"] = tuple(
+000113e0: 6c69 7374 2874 656d 705b 2264 6174 6122  list(temp["data"
+000113f0: 5d29 202b 2074 7261 6365 7329 0a0a 2020  ]) + traces)..  
+00011400: 2020 2020 2020 7265 7475 726e 2067 6f2e        return go.
+00011410: 4669 6775 7265 2874 656d 7029 0a0a 2020  Figure(temp)..  
+00011420: 2020 6465 6620 5f70 6c6f 745f 616e 6e6f    def _plot_anno
+00011430: 7461 7465 5f46 4f53 280a 2020 2020 2020  tate_FOS(.      
+00011440: 2020 7365 6c66 2c20 6669 672c 2063 5f78    self, fig, c_x
+00011450: 3a20 666c 6f61 742c 2063 5f79 3a20 666c  : float, c_y: fl
+00011460: 6f61 742c 2072 6164 6975 733a 2066 6c6f  oat, radius: flo
+00011470: 6174 2c20 464f 533a 2066 6c6f 6174 0a20  at, FOS: float. 
+00011480: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
+00011490: 2241 6e6e 6f74 6174 6520 464f 5320 6f6e  "Annotate FOS on
+000114a0: 2066 6967 7572 652e 0a0a 2020 2020 2020   figure...      
+000114b0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+000114c0: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
+000114d0: 2020 2020 2020 2020 6669 6720 3a20 706c          fig : pl
+000114e0: 6f74 6c79 2066 6967 7572 650a 2020 2020  otly figure.    
+000114f0: 2020 2020 635f 7820 3a20 666c 6f61 740a      c_x : float.
+00011500: 2020 2020 2020 2020 2020 2020 6369 7263              circ
+00011510: 6c65 2063 656e 7465 7220 7820 636f 6f72  le center x coor
+00011520: 6469 6e61 7465 2e0a 2020 2020 2020 2020  dinate..        
+00011530: 635f 7920 3a20 666c 6f61 740a 2020 2020  c_y : float.    
+00011540: 2020 2020 2020 2020 6369 7263 6c65 2063          circle c
+00011550: 656e 7465 7220 7920 636f 6f72 6469 6e61  enter y coordina
+00011560: 7465 2e0a 2020 2020 2020 2020 464f 5320  te..        FOS 
+00011570: 3a20 666c 6f61 740a 2020 2020 2020 2020  : float.        
+00011580: 2020 2020 6369 7263 6c65 2066 6163 746f      circle facto
+00011590: 7220 6f66 2073 6166 6574 7920 746f 2062  r of safety to b
+000115a0: 6520 616e 6e6f 7461 7465 6420 746f 2066  e annotated to f
+000115b0: 6967 7572 652e 0a0a 2020 2020 2020 2020  igure...        
+000115c0: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
+000115d0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+000115e0: 506c 6f74 6c79 2066 6967 7572 652e 0a20  Plotly figure.. 
+000115f0: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
+00011600: 2020 2020 636f 6c6f 7220 3d20 434f 4c4f      color = COLO
+00011610: 5552 5f46 4f53 5f44 4943 545b 6d69 6e28  UR_FOS_DICT[min(
+00011620: 726f 756e 6428 464f 532c 2031 292c 204d  round(FOS, 1), M
+00011630: 4158 5f43 4f4c 4f55 525f 4b45 5929 5d0a  AX_COLOUR_KEY)].
+00011640: 0a20 2020 2020 2020 2066 6967 2e61 6464  .        fig.add
+00011650: 5f74 7261 6365 280a 2020 2020 2020 2020  _trace(.        
+00011660: 2020 2020 676f 2e53 6361 7474 6572 280a      go.Scatter(.
+00011670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011680: 783d 5b63 5f78 5d2c 0a20 2020 2020 2020  x=[c_x],.       
+00011690: 2020 2020 2020 2020 2079 3d5b 635f 795d           y=[c_y]
+000116a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000116b0: 2020 6d6f 6465 3d22 6c69 6e65 732b 7465    mode="lines+te
+000116c0: 7874 222c 0a20 2020 2020 2020 2020 2020  xt",.           
+000116d0: 2020 2020 2074 6578 743d 5b66 227b 464f       text=[f"{FO
+000116e0: 533a 2e33 667d 225d 2c0a 2020 2020 2020  S:.3f}"],.      
+000116f0: 2020 2020 2020 2020 2020 7465 7874 706f            textpo
+00011700: 7369 7469 6f6e 3d22 746f 7020 7269 6768  sition="top righ
+00011710: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
+00011720: 2020 2020 7465 7874 666f 6e74 3d64 6963      textfont=dic
+00011730: 7428 6661 6d69 6c79 3d22 7361 6e73 2073  t(family="sans s
+00011740: 6572 6966 222c 2073 697a 653d 3230 2c20  erif", size=20, 
+00011750: 636f 6c6f 723d 636f 6c6f 7229 2c0a 2020  color=color),.  
+00011760: 2020 2020 2020 2020 2020 2020 2020 6e61                na
+00011770: 6d65 3d22 222c 0a20 2020 2020 2020 2020  me="",.         
+00011780: 2020 2020 2020 2074 6578 7474 656d 706c         texttempl
+00011790: 6174 653d 2225 7b74 6578 747d 222c 0a20  ate="%{text}",. 
+000117a0: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+000117b0: 6f76 6572 7465 6d70 6c61 7465 3d66 2243  overtemplate=f"C
+000117c0: 656e 7472 653a 2028 7b63 5f78 3a2e 3366  entre: ({c_x:.3f
+000117d0: 7d2c 207b 635f 793a 2e33 667d 293c 6272  }, {c_y:.3f})<br
+000117e0: 3e52 6164 6975 733a 207b 7261 6469 7573  >Radius: {radius
+000117f0: 3a2e 3366 7d3c 6272 3e46 4f53 3a20 7b46  :.3f}<br>FOS: {F
+00011800: 4f53 3a2e 3366 7d22 2c0a 2020 2020 2020  OS:.3f}",.      
+00011810: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00011820: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00011830: 6e20 6669 670a 0a20 2020 2064 6566 205f  n fig..    def _
+00011840: 706c 6f74 5f77 6174 6572 2873 656c 662c  plot_water(self,
+00011850: 2066 6967 293a 0a20 2020 2020 2020 2022   fig):.        "
+00011860: 2222 4164 6420 7761 7465 7220 7461 626c  ""Add water tabl
+00011870: 6520 746f 2070 6c6f 7422 2222 0a0a 2020  e to plot"""..  
+00011880: 2020 2020 2020 6966 2073 656c 662e 5f77        if self._w
+00011890: 6174 6572 5f52 4c20 6973 204e 6f6e 653a  ater_RL is None:
+000118a0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000118b0: 7572 6e20 6669 670a 0a20 2020 2020 2020  urn fig..       
+000118c0: 2079 203d 2073 656c 662e 5f77 6174 6572   y = self._water
+000118d0: 5f52 4c0a 2020 2020 2020 2020 7820 3d20  _RL.        x = 
+000118e0: 7365 6c66 2e67 6574 5f65 7874 6572 6e61  self.get_externa
+000118f0: 6c5f 785f 696e 7465 7273 6563 7469 6f6e  l_x_intersection
+00011900: 2879 290a 0a20 2020 2020 2020 2078 5f6c  (y)..        x_l
+00011910: 696e 6520 3d20 5b30 2c20 785d 0a20 2020  ine = [0, x].   
+00011920: 2020 2020 2079 5f6c 696e 6520 3d20 5b79       y_line = [y
+00011930: 2c20 795d 0a0a 2020 2020 2020 2020 2320  , y]..        # 
+00011940: 6966 2078 2069 7320 6c65 7373 2074 6861  if x is less tha
+00011950: 6e20 626f 7420 736c 6f70 6520 7468 656e  n bot slope then
+00011960: 2069 7320 616c 736f 2073 616d 6520 6173   is also same as
+00011970: 2073 6179 696e 6720 7820 6973 206c 6573   saying x is les
+00011980: 7320 7468 616e 2074 6865 2065 6467 6520  s than the edge 
+00011990: 6f66 2074 6865 206d 6f64 656c 2e0a 2020  of the model..  
+000119a0: 2020 2020 2020 2320 6261 7369 6361 6c6c        # basicall
+000119b0: 7920 6e65 6564 2074 6f20 6d61 6b65 2073  y need to make s
+000119c0: 7572 6520 7468 6520 7761 7465 7220 7461  ure the water ta
+000119d0: 626c 6520 636f 6e74 696e 7565 7320 616c  ble continues al
+000119e0: 6f6e 6720 7468 6520 7375 7266 6163 650a  ong the surface.
+000119f0: 2020 2020 2020 2020 2320 6173 2069 7320          # as is 
+00011a00: 636f 6e73 6572 7661 7469 7665 6c79 2063  conservatively c
+00011a10: 6f6e 7369 6465 7265 6420 696e 2074 6865  onsidered in the
+00011a20: 206d 6f64 656c 0a20 2020 2020 2020 2069   model.        i
+00011a30: 6620 7820 3c3d 2073 656c 662e 5f62 6f74  f x <= self._bot
+00011a40: 5f63 6f6f 7264 5b30 5d3a 0a20 2020 2020  _coord[0]:.     
+00011a50: 2020 2020 2020 2078 5f6c 696e 6520 2b3d         x_line +=
+00011a60: 205b 7365 6c66 2e5f 626f 745f 636f 6f72   [self._bot_coor
+00011a70: 645b 305d 2c20 7365 6c66 2e5f 6578 7465  d[0], self._exte
+00011a80: 726e 616c 5f6c 656e 6774 685d 0a20 2020  rnal_length].   
+00011a90: 2020 2020 2020 2020 2079 5f6c 696e 6520           y_line 
+00011aa0: 2b3d 205b 7365 6c66 2e5f 626f 745f 636f  += [self._bot_co
+00011ab0: 6f72 645b 315d 2c20 7365 6c66 2e5f 626f  ord[1], self._bo
+00011ac0: 745f 636f 6f72 645b 315d 5d0a 0a20 2020  t_coord[1]]..   
+00011ad0: 2020 2020 2066 6967 2e61 6464 5f74 7261       fig.add_tra
+00011ae0: 6365 280a 2020 2020 2020 2020 2020 2020  ce(.            
+00011af0: 676f 2e53 6361 7474 6572 280a 2020 2020  go.Scatter(.    
+00011b00: 2020 2020 2020 2020 2020 2020 783d 785f              x=x_
+00011b10: 6c69 6e65 2c0a 2020 2020 2020 2020 2020  line,.          
+00011b20: 2020 2020 2020 793d 795f 6c69 6e65 2c0a        y=y_line,.
+00011b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b40: 6d6f 6465 3d22 6c69 6e65 7322 2c0a 2020  mode="lines",.  
+00011b50: 2020 2020 2020 2020 2020 2020 2020 6c69                li
+00011b60: 6e65 5f63 6f6c 6f72 3d22 626c 7565 222c  ne_color="blue",
+00011b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011b80: 206c 696e 655f 7769 6474 683d 342c 0a20   line_width=4,. 
+00011b90: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00011ba0: 616d 653d 2222 2c0a 2020 2020 2020 2020  ame="",.        
+00011bb0: 2020 2020 290a 2020 2020 2020 2020 290a      ).        ).
+00011bc0: 0a20 2020 2020 2020 2066 6967 2e61 6464  .        fig.add
+00011bd0: 5f61 6e6e 6f74 6174 696f 6e28 0a20 2020  _annotation(.   
+00011be0: 2020 2020 2020 2020 2078 3d73 656c 662e           x=self.
+00011bf0: 5f74 6f70 5f63 6f6f 7264 5b30 5d20 2f20  _top_coord[0] / 
+00011c00: 342c 0a20 2020 2020 2020 2020 2020 2079  4,.            y
+00011c10: 3d79 2c0a 2020 2020 2020 2020 2020 2020  =y,.            
+00011c20: 7465 7874 3d22 e296 bc22 2c0a 2020 2020  text="...",.    
+00011c30: 2020 2020 2020 2020 7368 6f77 6172 726f          showarro
+00011c40: 773d 4661 6c73 652c 0a20 2020 2020 2020  w=False,.       
+00011c50: 2020 2020 2079 7368 6966 743d 3130 2c0a       yshift=10,.
+00011c60: 2020 2020 2020 2020 2020 2020 666f 6e74              font
+00011c70: 5f73 697a 653d 3235 2c0a 2020 2020 2020  _size=25,.      
+00011c80: 2020 2020 2020 666f 6e74 5f63 6f6c 6f72        font_color
+00011c90: 3d22 626c 7565 222c 0a20 2020 2020 2020  ="blue",.       
+00011ca0: 2029 0a0a 2020 2020 2020 2020 6669 672e   )..        fig.
+00011cb0: 6164 645f 616e 6e6f 7461 7469 6f6e 280a  add_annotation(.
+00011cc0: 2020 2020 2020 2020 2020 2020 783d 7365              x=se
+00011cd0: 6c66 2e5f 746f 705f 636f 6f72 645b 305d  lf._top_coord[0]
+00011ce0: 202f 2034 2c0a 2020 2020 2020 2020 2020   / 4,.          
+00011cf0: 2020 793d 792c 0a20 2020 2020 2020 2020    y=y,.         
+00011d00: 2020 2074 6578 743d 225f 222c 0a20 2020     text="_",.   
+00011d10: 2020 2020 2020 2020 2073 686f 7761 7272           showarr
+00011d20: 6f77 3d46 616c 7365 2c0a 2020 2020 2020  ow=False,.      
+00011d30: 2020 2020 2020 7973 6869 6674 3d32 2c0a        yshift=2,.
+00011d40: 2020 2020 2020 2020 2020 2020 666f 6e74              font
+00011d50: 5f73 697a 653d 3235 2c0a 2020 2020 2020  _size=25,.      
+00011d60: 2020 2020 2020 666f 6e74 5f63 6f6c 6f72        font_color
+00011d70: 3d22 626c 7565 222c 0a20 2020 2020 2020  ="blue",.       
+00011d80: 2029 0a0a 2020 2020 2020 2020 7265 7475   )..        retu
+00011d90: 726e 2066 6967 0a0a 2020 2020 6465 6620  rn fig..    def 
+00011da0: 5f70 6c6f 745f 6c69 6d69 7473 2873 656c  _plot_limits(sel
+00011db0: 662c 2066 6967 293a 0a20 2020 2020 2020  f, fig):.       
+00011dc0: 2022 2222 4164 6420 616e 616c 7973 6973   """Add analysis
+00011dd0: 206c 696d 6974 7320 746f 2070 6c6f 7422   limits to plot"
+00011de0: 2222 0a0a 2020 2020 2020 2020 6c31 5f78  ""..        l1_x
+00011df0: 2c20 6c32 5f78 203d 2073 656c 662e 5f6c  , l2_x = self._l
+00011e00: 696d 6974 735b 305d 2c20 7365 6c66 2e5f  imits[0], self._
+00011e10: 6c69 6d69 7473 5b31 5d0a 2020 2020 2020  limits[1].      
+00011e20: 2020 7231 5f78 2c20 7232 5f78 203d 2073    r1_x, r2_x = s
+00011e30: 656c 662e 5f6c 696d 6974 735b 325d 2c20  elf._limits[2], 
+00011e40: 7365 6c66 2e5f 6c69 6d69 7473 5b33 5d0a  self._limits[3].
+00011e50: 0a20 2020 2020 2020 206c 315f 7920 3d20  .        l1_y = 
+00011e60: 7365 6c66 2e67 6574 5f65 7874 6572 6e61  self.get_externa
+00011e70: 6c5f 795f 696e 7465 7273 6563 7469 6f6e  l_y_intersection
+00011e80: 286c 315f 7829 0a20 2020 2020 2020 206c  (l1_x).        l
+00011e90: 325f 7920 3d20 7365 6c66 2e67 6574 5f65  2_y = self.get_e
+00011ea0: 7874 6572 6e61 6c5f 795f 696e 7465 7273  xternal_y_inters
+00011eb0: 6563 7469 6f6e 286c 325f 7829 0a20 2020  ection(l2_x).   
+00011ec0: 2020 2020 2072 315f 7920 3d20 7365 6c66       r1_y = self
+00011ed0: 2e67 6574 5f65 7874 6572 6e61 6c5f 795f  .get_external_y_
+00011ee0: 696e 7465 7273 6563 7469 6f6e 2872 315f  intersection(r1_
+00011ef0: 7829 0a20 2020 2020 2020 2072 325f 7920  x).        r2_y 
+00011f00: 3d20 7365 6c66 2e67 6574 5f65 7874 6572  = self.get_exter
+00011f10: 6e61 6c5f 795f 696e 7465 7273 6563 7469  nal_y_intersecti
+00011f20: 6f6e 2872 325f 7829 0a0a 2020 2020 2020  on(r2_x)..      
+00011f30: 2020 706f 696e 7473 5f72 6967 6874 203d    points_right =
+00011f40: 205b 286c 315f 782c 206c 315f 7929 5d0a   [(l1_x, l1_y)].
+00011f50: 2020 2020 2020 2020 706f 696e 7473 5f6c          points_l
+00011f60: 6566 7420 3d20 5b28 7232 5f78 2c20 7232  eft = [(r2_x, r2
+00011f70: 5f79 295d 0a0a 2020 2020 2020 2020 6966  _y)]..        if
+00011f80: 2073 656c 662e 5f6c 696d 6974 735b 315d   self._limits[1]
+00011f90: 2021 3d20 7365 6c66 2e5f 6c69 6d69 7473   != self._limits
+00011fa0: 5b32 5d3a 0a20 2020 2020 2020 2020 2020  [2]:.           
+00011fb0: 2070 6f69 6e74 735f 7269 6768 7420 2b3d   points_right +=
+00011fc0: 205b 2872 315f 782c 2072 315f 7929 5d0a   [(r1_x, r1_y)].
+00011fd0: 2020 2020 2020 2020 2020 2020 706f 696e              poin
+00011fe0: 7473 5f6c 6566 7420 2b3d 205b 286c 325f  ts_left += [(l2_
+00011ff0: 782c 206c 325f 7929 5d0a 0a20 2020 2020  x, l2_y)]..     
+00012000: 2020 2023 2061 6464 206f 7574 6572 206c     # add outer l
+00012010: 696d 6974 730a 2020 2020 2020 2020 666f  imits.        fo
+00012020: 7220 7020 696e 2070 6f69 6e74 735f 7269  r p in points_ri
+00012030: 6768 743a 0a20 2020 2020 2020 2020 2020  ght:.           
+00012040: 2066 6967 2e61 6464 5f61 6e6e 6f74 6174   fig.add_annotat
+00012050: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
+00012060: 2020 2020 2078 3d70 5b30 5d2c 0a20 2020       x=p[0],.   
+00012070: 2020 2020 2020 2020 2020 2020 2079 3d70               y=p
+00012080: 5b31 5d2c 0a20 2020 2020 2020 2020 2020  [1],.           
+00012090: 2020 2020 2074 6578 743d 22e2 96b6 222c       text="...",
+000120a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000120b0: 2073 686f 7761 7272 6f77 3d46 616c 7365   showarrow=False
+000120c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000120d0: 2020 7973 6869 6674 3d31 352c 0a20 2020    yshift=15,.   
+000120e0: 2020 2020 2020 2020 2020 2020 2078 7368               xsh
+000120f0: 6966 743d 2d31 302c 0a20 2020 2020 2020  ift=-10,.       
+00012100: 2020 2020 2020 2020 2066 6f6e 745f 7369           font_si
+00012110: 7a65 3d32 352c 0a20 2020 2020 2020 2020  ze=25,.         
+00012120: 2020 2020 2020 2066 6f6e 745f 636f 6c6f         font_colo
+00012130: 723d 2262 6c61 636b 222c 0a20 2020 2020  r="black",.     
+00012140: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00012150: 2020 666f 7220 7020 696e 2070 6f69 6e74    for p in point
+00012160: 735f 6c65 6674 3a0a 2020 2020 2020 2020  s_left:.        
+00012170: 2020 2020 6669 672e 6164 645f 616e 6e6f      fig.add_anno
+00012180: 7461 7469 6f6e 280a 2020 2020 2020 2020  tation(.        
+00012190: 2020 2020 2020 2020 783d 705b 305d 2c0a          x=p[0],.
+000121a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000121b0: 793d 705b 315d 2c0a 2020 2020 2020 2020  y=p[1],.        
+000121c0: 2020 2020 2020 2020 7465 7874 3d22 e297          text="..
+000121d0: 8022 2c0a 2020 2020 2020 2020 2020 2020  .",.            
+000121e0: 2020 2020 7368 6f77 6172 726f 773d 4661      showarrow=Fa
+000121f0: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
+00012200: 2020 2020 2079 7368 6966 743d 3135 2c0a       yshift=15,.
+00012210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012220: 7873 6869 6674 3d31 302c 0a20 2020 2020  xshift=10,.     
+00012230: 2020 2020 2020 2020 2020 2066 6f6e 745f             font_
+00012240: 7369 7a65 3d32 352c 0a20 2020 2020 2020  size=25,.       
+00012250: 2020 2020 2020 2020 2066 6f6e 745f 636f           font_co
+00012260: 6c6f 723d 2262 6c61 636b 222c 0a20 2020  lor="black",.   
+00012270: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+00012280: 2020 2020 666f 7220 7020 696e 2070 6f69      for p in poi
+00012290: 6e74 735f 6c65 6674 202b 2070 6f69 6e74  nts_left + point
+000122a0: 735f 7269 6768 743a 0a20 2020 2020 2020  s_right:.       
+000122b0: 2020 2020 2066 6967 2e61 6464 5f61 6e6e       fig.add_ann
+000122c0: 6f74 6174 696f 6e28 0a20 2020 2020 2020  otation(.       
+000122d0: 2020 2020 2020 2020 2078 3d70 5b30 5d2c           x=p[0],
+000122e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000122f0: 2079 3d70 5b31 5d2c 0a20 2020 2020 2020   y=p[1],.       
+00012300: 2020 2020 2020 2020 2074 6578 743d 227c           text="|
+00012310: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00012320: 2020 2073 686f 7761 7272 6f77 3d46 616c     showarrow=Fal
+00012330: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
+00012340: 2020 2020 7973 6869 6674 3d31 352c 0a20      yshift=15,. 
+00012350: 2020 2020 2020 2020 2020 2020 2020 2078                 x
+00012360: 7368 6966 743d 302c 0a20 2020 2020 2020  shift=0,.       
+00012370: 2020 2020 2020 2020 2066 6f6e 745f 7369           font_si
+00012380: 7a65 3d32 352c 0a20 2020 2020 2020 2020  ze=25,.         
+00012390: 2020 2020 2020 2066 6f6e 745f 636f 6c6f         font_colo
+000123a0: 723d 2262 6c61 636b 222c 0a20 2020 2020  r="black",.     
+000123b0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+000123c0: 2020 7265 7475 726e 2066 6967 0a0a 2020    return fig..  
+000123d0: 2020 6465 6620 5f70 6c6f 745f 6c6c 2873    def _plot_ll(s
+000123e0: 656c 662c 2066 6967 2c20 6c6c 293a 0a20  elf, fig, ll):. 
+000123f0: 2020 2020 2020 2022 2222 4164 6420 706f         """Add po
+00012400: 696e 746c 6f61 6420 746f 2070 6c6f 7422  intload to plot"
+00012410: 2222 0a0a 2020 2020 2020 2020 6669 6720  ""..        fig 
+00012420: 3d20 7574 696c 6974 6965 732e 6472 6177  = utilities.draw
+00012430: 5f61 7272 6f77 280a 2020 2020 2020 2020  _arrow(.        
+00012440: 2020 2020 6669 672c 0a20 2020 2020 2020      fig,.       
+00012450: 2020 2020 2061 6e67 6c65 3d2d 3930 2c0a       angle=-90,.
+00012460: 2020 2020 2020 2020 2020 2020 666f 7263              forc
+00012470: 653d 6c6c 2e6d 6167 6e69 7475 6465 2c0a  e=ll.magnitude,.
+00012480: 2020 2020 2020 2020 2020 2020 785f 7375              x_su
+00012490: 703d 6c6c 2e63 6f6f 7264 2c0a 2020 2020  p=ll.coord,.    
+000124a0: 2020 2020 2020 2020 795f 7375 703d 7365          y_sup=se
+000124b0: 6c66 2e5f 746f 705f 636f 6f72 645b 315d  lf._top_coord[1]
+000124c0: 2c0a 2020 2020 2020 2020 2020 2020 636f  ,.            co
+000124d0: 6c6f 723d 2262 6c61 636b 222c 0a20 2020  lor="black",.   
+000124e0: 2020 2020 2020 2020 2061 7272 6f77 6c65           arrowle
+000124f0: 6e67 7468 3d31 3530 2c0a 2020 2020 2020  ngth=150,.      
+00012500: 2020 2020 2020 7368 6f77 5f76 616c 7565        show_value
+00012510: 733d 5472 7565 2c0a 2020 2020 2020 2020  s=True,.        
+00012520: 2020 2020 7072 6563 6973 696f 6e3d 6c6c      precision=ll
+00012530: 2e70 7265 6369 7369 6f6e 2c0a 2020 2020  .precision,.    
+00012540: 2020 2020 2020 2020 756e 6974 733d 226b          units="k
+00012550: 4e2f 6d22 2c0a 2020 2020 2020 2020 2020  N/m",.          
+00012560: 2020 6172 726f 7768 6561 643d 3130 2c0a    arrowhead=10,.
+00012570: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00012580: 2020 2066 6967 203d 2075 7469 6c69 7469     fig = utiliti
+00012590: 6573 2e64 7261 775f 6172 726f 7728 0a20  es.draw_arrow(. 
+000125a0: 2020 2020 2020 2020 2020 2066 6967 2c0a             fig,.
+000125b0: 2020 2020 2020 2020 2020 2020 616e 676c              angl
+000125c0: 653d 2d39 302c 0a20 2020 2020 2020 2020  e=-90,.         
+000125d0: 2020 2066 6f72 6365 3d6c 6c2e 6d61 676e     force=ll.magn
+000125e0: 6974 7564 652c 0a20 2020 2020 2020 2020  itude,.         
+000125f0: 2020 2078 5f73 7570 3d6c 6c2e 636f 6f72     x_sup=ll.coor
+00012600: 642c 0a20 2020 2020 2020 2020 2020 2079  d,.            y
+00012610: 5f73 7570 3d73 656c 662e 5f74 6f70 5f63  _sup=self._top_c
+00012620: 6f6f 7264 5b31 5d2c 0a20 2020 2020 2020  oord[1],.       
+00012630: 2020 2020 2063 6f6c 6f72 3d6c 6c2e 636f       color=ll.co
+00012640: 6c6f 722c 0a20 2020 2020 2020 2020 2020  lor,.           
+00012650: 2061 7272 6f77 6c65 6e67 7468 3d31 3530   arrowlength=150
+00012660: 2c0a 2020 2020 2020 2020 2020 2020 7368  ,.            sh
+00012670: 6f77 5f76 616c 7565 733d 4661 6c73 652c  ow_values=False,
+00012680: 0a20 2020 2020 2020 2020 2020 2075 6e69  .            uni
+00012690: 7473 3d22 6b4e 2f6d 222c 0a20 2020 2020  ts="kN/m",.     
+000126a0: 2020 2020 2020 2061 7272 6f77 6865 6164         arrowhead
+000126b0: 3d31 302c 0a20 2020 2020 2020 2029 0a0a  =10,.        )..
+000126c0: 2020 2020 2020 2020 7265 7475 726e 2066          return f
+000126d0: 6967 0a0a 2020 2020 6465 6620 5f70 6c6f  ig..    def _plo
+000126e0: 745f 7564 6c28 7365 6c66 2c20 6669 672c  t_udl(self, fig,
+000126f0: 2075 646c 293a 0a20 2020 2020 2020 2022   udl):.        "
+00012700: 2222 4164 6420 556e 6966 6f72 6d20 6c6f  ""Add Uniform lo
+00012710: 6164 2074 6f20 706c 6f74 2222 220a 0a20  ad to plot""".. 
+00012720: 2020 2020 2020 2066 6967 203d 2075 7469         fig = uti
+00012730: 6c69 7469 6573 2e64 7261 775f 6172 726f  lities.draw_arro
+00012740: 7728 0a20 2020 2020 2020 2020 2020 2066  w(.            f
+00012750: 6967 2c0a 2020 2020 2020 2020 2020 2020  ig,.            
+00012760: 616e 676c 653d 2d39 302c 0a20 2020 2020  angle=-90,.     
+00012770: 2020 2020 2020 2066 6f72 6365 3d75 646c         force=udl
+00012780: 2e6d 6167 6e69 7475 6465 2c0a 2020 2020  .magnitude,.    
+00012790: 2020 2020 2020 2020 785f 7375 703d 7564          x_sup=ud
+000127a0: 6c2e 6c65 6674 2c0a 2020 2020 2020 2020  l.left,.        
+000127b0: 2020 2020 795f 7375 703d 7365 6c66 2e5f      y_sup=self._
+000127c0: 746f 705f 636f 6f72 645b 315d 2c0a 2020  top_coord[1],.  
+000127d0: 2020 2020 2020 2020 2020 636f 6c6f 723d            color=
+000127e0: 7564 6c2e 636f 6c6f 722c 0a20 2020 2020  udl.color,.     
+000127f0: 2020 2020 2020 2061 7272 6f77 6c65 6e67         arrowleng
+00012800: 7468 3d31 3030 202a 2028 7564 6c2e 6d61  th=100 * (udl.ma
+00012810: 676e 6974 7564 6520 2f20 7365 6c66 2e5f  gnitude / self._
+00012820: 7564 6c5f 6d61 7829 2c0a 2020 2020 2020  udl_max),.      
+00012830: 2020 2020 2020 7368 6f77 5f76 616c 7565        show_value
+00012840: 733d 4661 6c73 652c 0a20 2020 2020 2020  s=False,.       
+00012850: 2020 2020 2075 6e69 7473 3d22 6b4e 222c       units="kN",
+00012860: 0a20 2020 2020 2020 2020 2020 2061 7272  .            arr
+00012870: 6f77 6865 6164 3d31 302c 0a20 2020 2020  owhead=10,.     
+00012880: 2020 2020 2020 2070 7265 6369 7369 6f6e         precision
+00012890: 3d75 646c 2e70 7265 6369 7369 6f6e 2c0a  =udl.precision,.
+000128a0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+000128b0: 2020 2066 6967 203d 2075 7469 6c69 7469     fig = utiliti
+000128c0: 6573 2e64 7261 775f 6172 726f 7728 0a20  es.draw_arrow(. 
+000128d0: 2020 2020 2020 2020 2020 2066 6967 2c0a             fig,.
+000128e0: 2020 2020 2020 2020 2020 2020 616e 676c              angl
+000128f0: 653d 2d39 302c 0a20 2020 2020 2020 2020  e=-90,.         
+00012900: 2020 2066 6f72 6365 3d75 646c 2e6d 6167     force=udl.mag
+00012910: 6e69 7475 6465 2c0a 2020 2020 2020 2020  nitude,.        
+00012920: 2020 2020 785f 7375 703d 2875 646c 2e6c      x_sup=(udl.l
+00012930: 6566 7420 2b20 7564 6c2e 7269 6768 7429  eft + udl.right)
+00012940: 202f 2032 2c0a 2020 2020 2020 2020 2020   / 2,.          
+00012950: 2020 795f 7375 703d 7365 6c66 2e5f 746f    y_sup=self._to
+00012960: 705f 636f 6f72 645b 315d 2c0a 2020 2020  p_coord[1],.    
+00012970: 2020 2020 2020 2020 636f 6c6f 723d 2262          color="b
+00012980: 6c61 636b 222c 0a20 2020 2020 2020 2020  lack",.         
+00012990: 2020 2061 7272 6f77 6c65 6e67 7468 3d31     arrowlength=1
+000129a0: 3030 202a 2028 7564 6c2e 6d61 676e 6974  00 * (udl.magnit
+000129b0: 7564 6520 2f20 7365 6c66 2e5f 7564 6c5f  ude / self._udl_
+000129c0: 6d61 7829 202b 2031 302c 0a20 2020 2020  max) + 10,.     
+000129d0: 2020 2020 2020 2073 686f 775f 7661 6c75         show_valu
+000129e0: 6573 3d54 7275 652c 0a20 2020 2020 2020  es=True,.       
+000129f0: 2020 2020 2070 7265 6369 7369 6f6e 3d75       precision=u
+00012a00: 646c 2e70 7265 6369 7369 6f6e 2c0a 2020  dl.precision,.  
+00012a10: 2020 2020 2020 2020 2020 756e 6974 733d            units=
+00012a20: 226b 5061 222c 0a20 2020 2020 2020 2020  "kPa",.         
+00012a30: 2020 2061 7272 6f77 6865 6164 3d30 2c0a     arrowhead=0,.
+00012a40: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
+00012a50: 5f77 6964 7468 3d30 2c0a 2020 2020 2020  _width=0,.      
+00012a60: 2020 290a 0a20 2020 2020 2020 2066 6967    )..        fig
+00012a70: 203d 2075 7469 6c69 7469 6573 2e64 7261   = utilities.dra
+00012a80: 775f 6172 726f 7728 0a20 2020 2020 2020  w_arrow(.       
+00012a90: 2020 2020 2066 6967 2c0a 2020 2020 2020       fig,.      
+00012aa0: 2020 2020 2020 616e 676c 653d 2d39 302c        angle=-90,
+00012ab0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00012ac0: 6365 3d75 646c 2e6d 6167 6e69 7475 6465  ce=udl.magnitude
+00012ad0: 2c0a 2020 2020 2020 2020 2020 2020 785f  ,.            x_
+00012ae0: 7375 703d 7564 6c2e 7269 6768 742c 0a20  sup=udl.right,. 
+00012af0: 2020 2020 2020 2020 2020 2079 5f73 7570             y_sup
+00012b00: 3d73 656c 662e 5f74 6f70 5f63 6f6f 7264  =self._top_coord
+00012b10: 5b31 5d2c 0a20 2020 2020 2020 2020 2020  [1],.           
+00012b20: 2063 6f6c 6f72 3d75 646c 2e63 6f6c 6f72   color=udl.color
+00012b30: 2c0a 2020 2020 2020 2020 2020 2020 6172  ,.            ar
+00012b40: 726f 776c 656e 6774 683d 3130 3020 2a20  rowlength=100 * 
+00012b50: 2875 646c 2e6d 6167 6e69 7475 6465 202f  (udl.magnitude /
+00012b60: 2073 656c 662e 5f75 646c 5f6d 6178 292c   self._udl_max),
+00012b70: 0a20 2020 2020 2020 2020 2020 2073 686f  .            sho
+00012b80: 775f 7661 6c75 6573 3d46 616c 7365 2c0a  w_values=False,.
+00012b90: 2020 2020 2020 2020 2020 2020 756e 6974              unit
+00012ba0: 733d 226b 4e22 2c0a 2020 2020 2020 2020  s="kN",.        
+00012bb0: 2020 2020 6172 726f 7768 6561 643d 3130      arrowhead=10
+00012bc0: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
+00012bd0: 2020 2020 2023 2044 7261 7720 696e 206c       # Draw in l
+00012be0: 696e 6520 6162 6f76 6520 6172 726f 7773  ine above arrows
+00012bf0: 0a20 2020 2020 2020 2079 3020 3d20 3130  .        y0 = 10
+00012c00: 3020 2a20 2875 646c 2e6d 6167 6e69 7475  0 * (udl.magnitu
+00012c10: 6465 202f 2073 656c 662e 5f75 646c 5f6d  de / self._udl_m
+00012c20: 6178 290a 0a20 2020 2020 2020 2073 6861  ax)..        sha
+00012c30: 7065 203d 2064 6963 7428 0a20 2020 2020  pe = dict(.     
+00012c40: 2020 2020 2020 2074 7970 653d 226c 696e         type="lin
+00012c50: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+00012c60: 7872 6566 3d22 7822 2c0a 2020 2020 2020  xref="x",.      
+00012c70: 2020 2020 2020 7972 6566 3d22 7922 2c0a        yref="y",.
+00012c80: 2020 2020 2020 2020 2020 2020 7830 3d75              x0=u
+00012c90: 646c 2e6c 6566 742c 0a20 2020 2020 2020  dl.left,.       
+00012ca0: 2020 2020 2079 303d 7930 2c0a 2020 2020       y0=y0,.    
+00012cb0: 2020 2020 2020 2020 7831 3d75 646c 2e72          x1=udl.r
+00012cc0: 6967 6874 2c0a 2020 2020 2020 2020 2020  ight,.          
+00012cd0: 2020 7931 3d79 302c 0a20 2020 2020 2020    y1=y0,.       
+00012ce0: 2020 2020 206c 696e 655f 636f 6c6f 723d       line_color=
+00012cf0: 7564 6c2e 636f 6c6f 722c 0a20 2020 2020  udl.color,.     
+00012d00: 2020 2020 2020 206c 696e 655f 7769 6474         line_widt
+00012d10: 683d 322c 0a20 2020 2020 2020 2020 2020  h=2,.           
+00012d20: 2079 7369 7a65 6d6f 6465 3d22 7069 7865   ysizemode="pixe
+00012d30: 6c22 2c0a 2020 2020 2020 2020 2020 2020  l",.            
+00012d40: 7861 6e63 686f 723d 7564 6c2e 6c65 6674  xanchor=udl.left
+00012d50: 2c0a 2020 2020 2020 2020 2020 2020 7961  ,.            ya
+00012d60: 6e63 686f 723d 7365 6c66 2e5f 746f 705f  nchor=self._top_
+00012d70: 636f 6f72 645b 315d 2c0a 2020 2020 2020  coord[1],.      
+00012d80: 2020 290a 0a20 2020 2020 2020 2066 6967    )..        fig
+00012d90: 2e61 6464 5f73 6861 7065 2873 6861 7065  .add_shape(shape
+00012da0: 290a 0a20 2020 2020 2020 2023 2064 7261  )..        # dra
+00012db0: 7720 696e 2072 6563 7461 6e67 756c 6172  w in rectangular
+00012dc0: 2061 7265 610a 2020 2020 2020 2020 7368   area.        sh
+00012dd0: 6170 6520 3d20 6469 6374 280a 2020 2020  ape = dict(.    
+00012de0: 2020 2020 2020 2020 7479 7065 3d22 7265          type="re
+00012df0: 6374 222c 0a20 2020 2020 2020 2020 2020  ct",.           
+00012e00: 2078 7265 663d 2278 222c 0a20 2020 2020   xref="x",.     
+00012e10: 2020 2020 2020 2079 7265 663d 2279 222c         yref="y",
+00012e20: 0a20 2020 2020 2020 2020 2020 2078 303d  .            x0=
+00012e30: 7564 6c2e 6c65 6674 2c0a 2020 2020 2020  udl.left,.      
+00012e40: 2020 2020 2020 7930 3d30 2c0a 2020 2020        y0=0,.    
+00012e50: 2020 2020 2020 2020 7831 3d75 646c 2e72          x1=udl.r
+00012e60: 6967 6874 2c0a 2020 2020 2020 2020 2020  ight,.          
+00012e70: 2020 7931 3d79 302c 0a20 2020 2020 2020    y1=y0,.       
+00012e80: 2020 2020 2066 696c 6c63 6f6c 6f72 3d75       fillcolor=u
+00012e90: 646c 2e63 6f6c 6f72 2c0a 2020 2020 2020  dl.color,.      
+00012ea0: 2020 2020 2020 6f70 6163 6974 793d 302e        opacity=0.
+00012eb0: 322c 0a20 2020 2020 2020 2020 2020 206c  2,.            l
+00012ec0: 696e 655f 7769 6474 683d 322c 0a20 2020  ine_width=2,.   
+00012ed0: 2020 2020 2020 2020 2079 7369 7a65 6d6f           ysizemo
+00012ee0: 6465 3d22 7069 7865 6c22 2c0a 2020 2020  de="pixel",.    
+00012ef0: 2020 2020 2020 2020 7861 6e63 686f 723d          xanchor=
+00012f00: 7564 6c2e 6c65 6674 2c0a 2020 2020 2020  udl.left,.      
+00012f10: 2020 2020 2020 7961 6e63 686f 723d 7365        yanchor=se
+00012f20: 6c66 2e5f 746f 705f 636f 6f72 645b 315d  lf._top_coord[1]
+00012f30: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
+00012f40: 2020 2020 2066 6967 2e61 6464 5f73 6861       fig.add_sha
+00012f50: 7065 2873 6861 7065 290a 0a20 2020 2020  pe(shape)..     
+00012f60: 2020 2072 6574 7572 6e20 6669 670a 0a20     return fig.. 
+00012f70: 2020 2064 6566 205f 706c 6f74 5f6d 6174     def _plot_mat
+00012f80: 6572 6961 6c5f 7461 626c 6528 7365 6c66  erial_table(self
+00012f90: 2c20 6669 6729 3a0a 2020 2020 2020 2020  , fig):.        
+00012fa0: 2222 2250 6c6f 7420 7461 626c 6520 6f66  """Plot table of
+00012fb0: 206d 6174 6572 6961 6c20 7072 6f70 6572   material proper
+00012fc0: 7469 6573 2222 220a 0a20 2020 2020 2020  ties"""..       
+00012fd0: 2072 6f77 5f68 203d 2030 2e30 350a 2020   row_h = 0.05.  
+00012fe0: 2020 2020 2020 7461 626c 655f 7769 6474        table_widt
+00012ff0: 6820 3d20 302e 340a 2020 2020 2020 2020  h = 0.4.        
+00013000: 7461 626c 655f 6865 6967 6874 203d 2072  table_height = r
+00013010: 6f77 5f68 202a 2028 6c65 6e28 7365 6c66  ow_h * (len(self
+00013020: 2e5f 6d61 7465 7269 616c 7329 202b 2031  ._materials) + 1
+00013030: 290a 0a20 2020 2020 2020 2023 2070 6f69  )..        # poi
+00013040: 6e74 7320 6174 2074 6865 2062 6f74 746f  nts at the botto
+00013050: 6d20 6c65 6674 0a20 2020 2020 2020 2078  m left.        x
+00013060: 302c 2079 3020 3d20 302e 312c 2030 2e31  0, y0 = 0.1, 0.1
+00013070: 0a0a 2020 2020 2020 2020 2320 706f 696e  ..        # poin
+00013080: 7473 2061 7420 7468 6520 746f 7020 7269  ts at the top ri
+00013090: 6768 740a 2020 2020 2020 2020 7831 203d  ght.        x1 =
+000130a0: 2078 3020 2b20 7461 626c 655f 7769 6474   x0 + table_widt
+000130b0: 680a 2020 2020 2020 2020 7931 203d 2079  h.        y1 = y
+000130c0: 3020 2b20 7461 626c 655f 6865 6967 6874  0 + table_height
+000130d0: 0a0a 2020 2020 2020 2020 2320 6164 6420  ..        # add 
+000130e0: 6865 6164 6572 2062 6163 6b67 726f 756e  header backgroun
+000130f0: 640a 2020 2020 2020 2020 6669 672e 6164  d.        fig.ad
+00013100: 645f 7368 6170 6528 0a20 2020 2020 2020  d_shape(.       
+00013110: 2020 2020 2074 7970 653d 2272 6563 7422       type="rect"
+00013120: 2c0a 2020 2020 2020 2020 2020 2020 7872  ,.            xr
+00013130: 6566 3d22 7820 646f 6d61 696e 222c 0a20  ef="x domain",. 
+00013140: 2020 2020 2020 2020 2020 2079 7265 663d             yref=
+00013150: 2279 2064 6f6d 6169 6e22 2c0a 2020 2020  "y domain",.    
+00013160: 2020 2020 2020 2020 7830 3d78 302c 0a20          x0=x0,. 
+00013170: 2020 2020 2020 2020 2020 2078 313d 7831             x1=x1
+00013180: 2c0a 2020 2020 2020 2020 2020 2020 7930  ,.            y0
+00013190: 3d79 3120 2d20 726f 775f 682c 0a20 2020  =y1 - row_h,.   
+000131a0: 2020 2020 2020 2020 2079 313d 7931 2c0a           y1=y1,.
+000131b0: 2020 2020 2020 2020 2020 2020 6669 6c6c              fill
+000131c0: 636f 6c6f 723d 226c 6967 6874 6772 6579  color="lightgrey
+000131d0: 222c 0a20 2020 2020 2020 2029 0a0a 2020  ",.        )..  
+000131e0: 2020 2020 2020 2320 6164 6420 6261 636b        # add back
+000131f0: 6772 6f75 6e64 0a20 2020 2020 2020 2066  ground.        f
+00013200: 6967 2e61 6464 5f73 6861 7065 280a 2020  ig.add_shape(.  
+00013210: 2020 2020 2020 2020 2020 7479 7065 3d22            type="
+00013220: 7265 6374 222c 0a20 2020 2020 2020 2020  rect",.         
+00013230: 2020 2078 7265 663d 2278 2064 6f6d 6169     xref="x domai
+00013240: 6e22 2c0a 2020 2020 2020 2020 2020 2020  n",.            
+00013250: 7972 6566 3d22 7920 646f 6d61 696e 222c  yref="y domain",
+00013260: 0a20 2020 2020 2020 2020 2020 2078 303d  .            x0=
+00013270: 7830 2c0a 2020 2020 2020 2020 2020 2020  x0,.            
+00013280: 7831 3d78 312c 0a20 2020 2020 2020 2020  x1=x1,.         
+00013290: 2020 2079 303d 7930 2c0a 2020 2020 2020     y0=y0,.      
+000132a0: 2020 2020 2020 7931 3d79 3120 2d20 726f        y1=y1 - ro
+000132b0: 775f 682c 0a20 2020 2020 2020 2020 2020  w_h,.           
+000132c0: 2066 696c 6c63 6f6c 6f72 3d22 7768 6974   fillcolor="whit
+000132d0: 6522 2c0a 2020 2020 2020 2020 290a 0a20  e",.        ).. 
+000132e0: 2020 2020 2020 2023 2061 6464 2063 6f6c         # add col
+000132f0: 756d 6e73 2069 6e0a 2020 2020 2020 2020  umns in.        
+00013300: 636f 6c75 6d6e 5f75 6e69 745f 706f 7369  column_unit_posi
+00013310: 7469 6f6e 7320 3d20 5b32 302c 2031 322c  tions = [20, 12,
+00013320: 2031 352c 2031 322c 2031 325d 0a20 2020   15, 12, 12].   
+00013330: 2020 2020 2063 6f6c 756d 6e5f 7265 6c5f       column_rel_
+00013340: 706f 7369 7469 6f6e 7320 3d20 5b5d 0a0a  positions = []..
+00013350: 2020 2020 2020 2020 746f 7461 6c5f 7769          total_wi
+00013360: 6474 6820 3d20 7375 6d28 636f 6c75 6d6e  dth = sum(column
+00013370: 5f75 6e69 745f 706f 7369 7469 6f6e 7329  _unit_positions)
+00013380: 0a0a 2020 2020 2020 2020 636f 6c75 6d6e  ..        column
+00013390: 5f74 6578 745f 756e 6974 5f78 7368 6966  _text_unit_xshif
+000133a0: 7420 3d20 5b31 2c20 312c 2031 2c20 352c  t = [1, 1, 1, 5,
+000133b0: 2035 5d0a 2020 2020 2020 2020 6173 7375   5].        assu
+000133c0: 6d65 645f 6772 6170 685f 7769 6474 6820  med_graph_width 
+000133d0: 3d20 3130 3030 0a20 2020 2020 2020 2063  = 1000.        c
+000133e0: 6f6c 756d 6e5f 7265 6c5f 7873 6869 6674  olumn_rel_xshift
+000133f0: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
+00013400: 2061 202f 2074 6f74 616c 5f77 6964 7468   a / total_width
+00013410: 202a 2061 7373 756d 6564 5f67 7261 7068   * assumed_graph
+00013420: 5f77 6964 7468 202a 2074 6162 6c65 5f77  _width * table_w
+00013430: 6964 7468 0a20 2020 2020 2020 2020 2020  idth.           
+00013440: 2066 6f72 2061 2069 6e20 636f 6c75 6d6e   for a in column
+00013450: 5f74 6578 745f 756e 6974 5f78 7368 6966  _text_unit_xshif
+00013460: 740a 2020 2020 2020 2020 5d0a 0a20 2020  t.        ]..   
+00013470: 2020 2020 2063 756d 5f77 6964 7468 203d       cum_width =
+00013480: 2030 0a20 2020 2020 2020 2066 6f72 2063   0.        for c
+00013490: 6f6c 5f77 6964 7468 2069 6e20 636f 6c75  ol_width in colu
+000134a0: 6d6e 5f75 6e69 745f 706f 7369 7469 6f6e  mn_unit_position
+000134b0: 733a 0a20 2020 2020 2020 2020 2020 2023  s:.            #
+000134c0: 2067 6574 2075 6e69 7420 706f 7369 7469   get unit positi
+000134d0: 6f6e 2028 6965 2070 6f73 6974 696f 6e20  on (ie position 
+000134e0: 6173 2070 6572 6365 6e74 6167 6520 6f66  as percentage of
+000134f0: 2074 6f74 616c 2077 6964 7468 290a 2020   total width).  
+00013500: 2020 2020 2020 2020 2020 636f 6c75 6d6e            column
+00013510: 5f72 656c 5f70 6f73 6974 696f 6e20 3d20  _rel_position = 
+00013520: 2863 756d 5f77 6964 7468 202b 2063 6f6c  (cum_width + col
+00013530: 5f77 6964 7468 2920 2f20 746f 7461 6c5f  _width) / total_
+00013540: 7769 6474 680a 2020 2020 2020 2020 2020  width.          
+00013550: 2020 636f 6c75 6d6e 5f72 656c 5f70 6f73    column_rel_pos
+00013560: 6974 696f 6e73 2e61 7070 656e 6428 636f  itions.append(co
+00013570: 6c75 6d6e 5f72 656c 5f70 6f73 6974 696f  lumn_rel_positio
+00013580: 6e29 0a0a 2020 2020 2020 2020 2020 2020  n)..            
+00013590: 6375 6d5f 7769 6474 6820 2b3d 2063 6f6c  cum_width += col
+000135a0: 5f77 6964 7468 0a0a 2020 2020 2020 2020  _width..        
+000135b0: 2020 2020 2320 6164 6420 696e 2063 6f6c      # add in col
+000135c0: 756d 6e20 6261 7365 6420 6f6e 2075 6e69  umn based on uni
+000135d0: 7420 706f 7369 7469 6f6e 0a20 2020 2020  t position.     
+000135e0: 2020 2020 2020 2078 203d 2078 3020 2b20         x = x0 + 
+000135f0: 636f 6c75 6d6e 5f72 656c 5f70 6f73 6974  column_rel_posit
+00013600: 696f 6e20 2a20 2874 6162 6c65 5f77 6964  ion * (table_wid
+00013610: 7468 290a 0a20 2020 2020 2020 2020 2020  th)..           
+00013620: 2066 6967 2e61 6464 5f73 6861 7065 280a   fig.add_shape(.
+00013630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013640: 7479 7065 3d22 7265 6374 222c 0a20 2020  type="rect",.   
+00013650: 2020 2020 2020 2020 2020 2020 2078 7265               xre
+00013660: 663d 2278 2064 6f6d 6169 6e22 2c0a 2020  f="x domain",.  
+00013670: 2020 2020 2020 2020 2020 2020 2020 7972                yr
+00013680: 6566 3d22 7920 646f 6d61 696e 222c 0a20  ef="y domain",. 
+00013690: 2020 2020 2020 2020 2020 2020 2020 2078                 x
+000136a0: 303d 782c 0a20 2020 2020 2020 2020 2020  0=x,.           
+000136b0: 2020 2020 2078 313d 782c 0a20 2020 2020       x1=x,.     
+000136c0: 2020 2020 2020 2020 2020 2079 303d 7930             y0=y0
+000136d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000136e0: 2020 7931 3d79 312c 0a20 2020 2020 2020    y1=y1,.       
+000136f0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00013700: 2320 6164 6420 696e 2068 6561 6465 7220  # add in header 
+00013710: 7465 7874 0a20 2020 2020 2020 2074 6162  text.        tab
+00013720: 6c65 5f68 6561 6465 7220 3d20 5b22 4d41  le_header = ["MA
+00013730: 5445 5249 414c 222c 2022 434f 4c4f 5222  TERIAL", "COLOR"
+00013740: 2c20 22ce b320 286b 4e2f 6d33 2922 2c20  , ".. (kN/m3)", 
+00013750: 2263 2028 6b50 6129 222c 2022 cf95 2028  "c (kPa)", ".. (
+00013760: 6465 6729 225d 0a20 2020 2020 2020 2074  deg)"].        t
+00013770: 6162 6c65 5f68 6561 6465 7220 3d20 5b22  able_header = ["
+00013780: 3c62 3e22 202b 2061 202b 2022 3c2f 623e  <b>" + a + "</b>
+00013790: 2220 666f 7220 6120 696e 2074 6162 6c65  " for a in table
+000137a0: 5f68 6561 6465 725d 0a0a 2020 2020 2020  _header]..      
+000137b0: 2020 7820 3d20 7830 0a20 2020 2020 2020    x = x0.       
+000137c0: 2066 6f72 2069 2c20 6320 696e 2065 6e75   for i, c in enu
+000137d0: 6d65 7261 7465 2863 6f6c 756d 6e5f 7265  merate(column_re
+000137e0: 6c5f 706f 7369 7469 6f6e 7329 3a0a 2020  l_positions):.  
+000137f0: 2020 2020 2020 2020 2020 6669 672e 6164            fig.ad
+00013800: 645f 616e 6e6f 7461 7469 6f6e 280a 2020  d_annotation(.  
+00013810: 2020 2020 2020 2020 2020 2020 2020 7872                xr
+00013820: 6566 3d22 7820 646f 6d61 696e 222c 0a20  ef="x domain",. 
+00013830: 2020 2020 2020 2020 2020 2020 2020 2079                 y
+00013840: 7265 663d 2279 2064 6f6d 6169 6e22 2c0a  ref="y domain",.
+00013850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013860: 783d 782c 0a20 2020 2020 2020 2020 2020  x=x,.           
+00013870: 2020 2020 2079 3d79 3120 2d20 726f 775f       y=y1 - row_
+00013880: 6820 2f20 322c 0a20 2020 2020 2020 2020  h / 2,.         
+00013890: 2020 2020 2020 2074 6578 743d 7461 626c         text=tabl
+000138a0: 655f 6865 6164 6572 5b69 5d2c 0a20 2020  e_header[i],.   
+000138b0: 2020 2020 2020 2020 2020 2020 2073 686f               sho
+000138c0: 7761 7272 6f77 3d46 616c 7365 2c0a 2020  warrow=False,.  
+000138d0: 2020 2020 2020 2020 2020 2020 2020 7973                ys
+000138e0: 6869 6674 3d2d 3133 2c0a 2020 2020 2020  hift=-13,.      
+000138f0: 2020 2020 2020 2020 2020 7873 6869 6674            xshift
+00013900: 3d63 6f6c 756d 6e5f 7265 6c5f 7873 6869  =column_rel_xshi
+00013910: 6674 5b69 5d2c 0a20 2020 2020 2020 2020  ft[i],.         
+00013920: 2020 2020 2020 2066 6f6e 745f 7369 7a65         font_size
+00013930: 3d31 332c 0a20 2020 2020 2020 2020 2020  =13,.           
+00013940: 2020 2020 2066 6f6e 745f 636f 6c6f 723d       font_color=
+00013950: 2262 6c61 636b 222c 0a20 2020 2020 2020  "black",.       
+00013960: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00013970: 2020 2078 203d 2078 3020 2b20 6320 2a20     x = x0 + c * 
+00013980: 2874 6162 6c65 5f77 6964 7468 290a 0a20  (table_width).. 
+00013990: 2020 2020 2020 2023 2061 6464 2072 6f77         # add row
+000139a0: 730a 2020 2020 2020 2020 666f 7220 7220  s.        for r 
+000139b0: 696e 2072 616e 6765 286c 656e 2873 656c  in range(len(sel
+000139c0: 662e 5f6d 6174 6572 6961 6c73 2929 3a0a  f._materials)):.
+000139d0: 2020 2020 2020 2020 2020 2020 7920 3d20              y = 
+000139e0: 7931 202d 2072 6f77 5f68 202d 2072 202a  y1 - row_h - r *
+000139f0: 2072 6f77 5f68 0a0a 2020 2020 2020 2020   row_h..        
+00013a00: 2020 2020 6669 672e 6164 645f 7368 6170      fig.add_shap
+00013a10: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
+00013a20: 2020 2074 7970 653d 2272 6563 7422 2c0a     type="rect",.
+00013a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a40: 7872 6566 3d22 7820 646f 6d61 696e 222c  xref="x domain",
+00013a50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013a60: 2079 7265 663d 2279 2064 6f6d 6169 6e22   yref="y domain"
+00013a70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00013a80: 2020 7830 3d78 302c 0a20 2020 2020 2020    x0=x0,.       
+00013a90: 2020 2020 2020 2020 2078 313d 7831 2c0a           x1=x1,.
+00013aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ab0: 7930 3d79 2c0a 2020 2020 2020 2020 2020  y0=y,.          
+00013ac0: 2020 2020 2020 7931 3d79 2c0a 2020 2020        y1=y,.    
+00013ad0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00013ae0: 2020 2023 2061 6464 206d 6174 6572 6961     # add materia
+00013af0: 6c20 696e 666f 0a0a 2020 2020 2020 2020  l info..        
+00013b00: 7920 3d20 7931 202d 2072 6f77 5f68 202f  y = y1 - row_h /
+00013b10: 2032 0a0a 2020 2020 2020 2020 666f 7220   2..        for 
+00013b20: 702c 206d 2069 6e20 656e 756d 6572 6174  p, m in enumerat
+00013b30: 6528 7365 6c66 2e5f 6d61 7465 7269 616c  e(self._material
+00013b40: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+00013b50: 7820 3d20 7830 0a20 2020 2020 2020 2020  x = x0.         
+00013b60: 2020 2079 202d 3d20 726f 775f 680a 2020     y -= row_h.  
+00013b70: 2020 2020 2020 2020 2020 6461 7461 203d            data =
+00013b80: 205b 6d2e 6e61 6d65 2c20 2272 6564 222c   [m.name, "red",
+00013b90: 206d 2e75 6e69 745f 7765 6967 6874 2c20   m.unit_weight, 
+00013ba0: 6d2e 636f 6865 7369 6f6e 2c20 6d2e 6672  m.cohesion, m.fr
+00013bb0: 6963 7469 6f6e 5f61 6e67 6c65 5d0a 0a20  iction_angle].. 
+00013bc0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+00013bd0: 2c20 6320 696e 2065 6e75 6d65 7261 7465  , c in enumerate
+00013be0: 2863 6f6c 756d 6e5f 7265 6c5f 706f 7369  (column_rel_posi
+00013bf0: 7469 6f6e 7329 3a0a 2020 2020 2020 2020  tions):.        
+00013c00: 2020 2020 2020 2020 6966 2069 203d 3d20          if i == 
+00013c10: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
+00013c20: 2020 2020 2020 2066 6967 2e61 6464 5f73         fig.add_s
+00013c30: 6861 7065 280a 2020 2020 2020 2020 2020  hape(.          
+00013c40: 2020 2020 2020 2020 2020 2020 2020 7479                ty
+00013c50: 7065 3d22 7265 6374 222c 0a20 2020 2020  pe="rect",.     
+00013c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c70: 2020 2078 7265 663d 2270 6170 6572 222c     xref="paper",
+00013c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013c90: 2020 2020 2020 2020 2079 7265 663d 2270           yref="p
+00013ca0: 6170 6572 222c 0a20 2020 2020 2020 2020  aper",.         
+00013cb0: 2020 2020 2020 2020 2020 2020 2020 2078                 x
+00013cc0: 303d 782c 0a20 2020 2020 2020 2020 2020  0=x,.           
+00013cd0: 2020 2020 2020 2020 2020 2020 2078 313d               x1=
+00013ce0: 7830 202b 2063 6f6c 756d 6e5f 7265 6c5f  x0 + column_rel_
+00013cf0: 706f 7369 7469 6f6e 735b 315d 202a 2028  positions[1] * (
+00013d00: 7461 626c 655f 7769 6474 6829 2c0a 2020  table_width),.  
+00013d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d20: 2020 2020 2020 7930 3d79 202d 2072 6f77        y0=y - row
+00013d30: 5f68 202f 2032 2c0a 2020 2020 2020 2020  _h / 2,.        
+00013d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d50: 7931 3d79 202b 2072 6f77 5f68 202f 2032  y1=y + row_h / 2
+00013d60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00013d70: 2020 2020 2020 2020 2020 6669 6c6c 636f            fillco
+00013d80: 6c6f 723d 6d2e 636f 6c6f 722c 0a20 2020  lor=m.color,.   
+00013d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013da0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00013db0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00013dc0: 2020 2020 2020 2020 2020 2020 2066 6967               fig
+00013dd0: 2e61 6464 5f61 6e6e 6f74 6174 696f 6e28  .add_annotation(
+00013de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013df0: 2020 2020 2020 2020 2078 7265 663d 2278           xref="x
+00013e00: 2064 6f6d 6169 6e22 2c0a 2020 2020 2020   domain",.      
+00013e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013e20: 2020 7972 6566 3d22 7920 646f 6d61 696e    yref="y domain
+00013e30: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00013e40: 2020 2020 2020 2020 2020 2078 3d78 2c0a             x=x,.
+00013e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013e60: 2020 2020 2020 2020 793d 792c 0a20 2020          y=y,.   
+00013e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013e80: 2020 2020 2074 6578 743d 6461 7461 5b69       text=data[i
+00013e90: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00013ea0: 2020 2020 2020 2020 2020 2073 686f 7761             showa
+00013eb0: 7272 6f77 3d46 616c 7365 2c0a 2020 2020  rrow=False,.    
+00013ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ed0: 2020 2020 7973 6869 6674 3d2d 3133 2c0a      yshift=-13,.
+00013ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ef0: 2020 2020 2020 2020 7873 6869 6674 3d63          xshift=c
+00013f00: 6f6c 756d 6e5f 7265 6c5f 7873 6869 6674  olumn_rel_xshift
+00013f10: 5b69 5d2c 0a20 2020 2020 2020 2020 2020  [i],.           
+00013f20: 2020 2020 2020 2020 2020 2020 2066 6f6e               fon
+00013f30: 745f 7369 7a65 3d31 332c 0a20 2020 2020  t_size=13,.     
+00013f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f50: 2020 2066 6f6e 745f 636f 6c6f 723d 2262     font_color="b
+00013f60: 6c61 636b 222c 0a20 2020 2020 2020 2020  lack",.         
+00013f70: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00013f80: 2020 2020 2020 2020 2020 2020 2078 203d               x =
+00013f90: 2078 3020 2b20 6320 2a20 2874 6162 6c65   x0 + c * (table
+00013fa0: 5f77 6964 7468 290a 0a20 2020 2020 2020  _width)..       
+00013fb0: 2072 6574 7572 6e20 6669 670a 0a20 2020   return fig..   
+00013fc0: 2064 6566 205f 706c 6f74 5f46 4f53 5f6c   def _plot_FOS_l
+00013fd0: 6567 656e 6428 7365 6c66 2c20 6669 6729  egend(self, fig)
+00013fe0: 3a0a 2020 2020 2020 2020 2222 2250 6c6f  :.        """Plo
+00013ff0: 7420 636f 6c6f 7220 6c65 6765 6e64 2066  t color legend f
+00014000: 6f72 2066 6163 746f 7220 6f66 2073 6166  or factor of saf
+00014010: 6574 7920 636f 6c6f 7273 2222 220a 0a20  ety colors""".. 
+00014020: 2020 2020 2020 2079 6920 3d20 302e 390a         yi = 0.9.
+00014030: 2020 2020 2020 2020 7966 203d 2030 2e35          yf = 0.5
+00014040: 0a0a 2020 2020 2020 2020 7830 203d 2030  ..        x0 = 0
+00014050: 2e39 0a20 2020 2020 2020 2078 3120 3d20  .9.        x1 = 
+00014060: 302e 3935 0a0a 2020 2020 2020 2020 6669  0.95..        fi
+00014070: 672e 6164 645f 7368 6170 6528 0a20 2020  g.add_shape(.   
+00014080: 2020 2020 2020 2020 2074 7970 653d 2272           type="r
+00014090: 6563 7422 2c0a 2020 2020 2020 2020 2020  ect",.          
+000140a0: 2020 7872 6566 3d22 7061 7065 7222 2c0a    xref="paper",.
+000140b0: 2020 2020 2020 2020 2020 2020 7972 6566              yref
+000140c0: 3d22 7061 7065 7222 2c0a 2020 2020 2020  ="paper",.      
+000140d0: 2020 2020 2020 7830 3d78 3020 2d20 302e        x0=x0 - 0.
+000140e0: 3032 2c0a 2020 2020 2020 2020 2020 2020  02,.            
+000140f0: 7831 3d78 3120 2b20 302e 3035 2c0a 2020  x1=x1 + 0.05,.  
+00014100: 2020 2020 2020 2020 2020 7930 3d79 6920            y0=yi 
+00014110: 2b20 302e 3035 2c0a 2020 2020 2020 2020  + 0.05,.        
+00014120: 2020 2020 7931 3d79 6620 2d20 302e 3033      y1=yf - 0.03
+00014130: 2c0a 2020 2020 2020 2020 2020 2020 6669  ,.            fi
+00014140: 6c6c 636f 6c6f 723d 2277 6869 7465 222c  llcolor="white",
+00014150: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00014160: 2020 2020 666f 7220 6b2c 2076 2069 6e20      for k, v in 
+00014170: 434f 4c4f 5552 5f46 4f53 5f44 4943 542e  COLOUR_FOS_DICT.
+00014180: 6974 656d 7328 293a 0a20 2020 2020 2020  items():.       
+00014190: 2020 2020 2066 6967 2e61 6464 5f73 6861       fig.add_sha
+000141a0: 7065 280a 2020 2020 2020 2020 2020 2020  pe(.            
+000141b0: 2020 2020 7479 7065 3d22 7265 6374 222c      type="rect",
+000141c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000141d0: 2078 7265 663d 2270 6170 6572 222c 0a20   xref="paper",. 
+000141e0: 2020 2020 2020 2020 2020 2020 2020 2079                 y
+000141f0: 7265 663d 2270 6170 6572 222c 0a20 2020  ref="paper",.   
+00014200: 2020 2020 2020 2020 2020 2020 2078 303d               x0=
+00014210: 7830 2c0a 2020 2020 2020 2020 2020 2020  x0,.            
+00014220: 2020 2020 7831 3d78 312c 0a20 2020 2020      x1=x1,.     
+00014230: 2020 2020 2020 2020 2020 2079 303d 7969             y0=yi
+00014240: 202b 206b 202a 2028 7966 202d 2079 6929   + k * (yf - yi)
+00014250: 202f 204d 4158 5f43 4f4c 4f55 525f 4b45   / MAX_COLOUR_KE
+00014260: 592c 0a20 2020 2020 2020 2020 2020 2020  Y,.             
+00014270: 2020 2079 313d 7969 202b 2028 6b20 2b20     y1=yi + (k + 
+00014280: 302e 3129 202a 2028 7966 202d 2079 6929  0.1) * (yf - yi)
+00014290: 202f 204d 4158 5f43 4f4c 4f55 525f 4b45   / MAX_COLOUR_KE
+000142a0: 592c 0a20 2020 2020 2020 2020 2020 2020  Y,.             
+000142b0: 2020 2066 696c 6c63 6f6c 6f72 3d76 2c0a     fillcolor=v,.
+000142c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000142d0: 6c69 6e65 3d64 6963 7428 0a20 2020 2020  line=dict(.     
+000142e0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000142f0: 6f6c 6f72 3d22 626c 6163 6b22 2c0a 2020  olor="black",.  
+00014300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014310: 2020 7769 6474 683d 302e 322c 0a20 2020    width=0.2,.   
+00014320: 2020 2020 2020 2020 2020 2020 2029 2c0a               ),.
+00014330: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+00014340: 2020 2020 2020 2020 2020 2069 6620 726f             if ro
+00014350: 756e 6428 6b2c 2031 2920 2520 3120 3d3d  und(k, 1) % 1 ==
+00014360: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+00014370: 2020 2020 2320 6261 6e64 6169 6420 6669      # bandaid fi
+00014380: 7820 6265 6361 7573 6520 6920 6361 6e74  x because i cant
+00014390: 2066 6967 7572 6520 6f75 7420 7768 7920   figure out why 
+000143a0: 7468 6520 7363 616c 6520 7368 6f77 7320  the scale shows 
+000143b0: 7772 6f6e 670a 2020 2020 2020 2020 2020  wrong.          
+000143c0: 2020 2020 2020 6966 206b 203c 2032 2e35        if k < 2.5
+000143d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000143e0: 2020 2020 2020 7920 3d20 666c 6f61 7428        y = float(
+000143f0: 7969 2920 2b20 666c 6f61 7428 6b20 2d20  yi) + float(k - 
+00014400: 302e 3135 2920 2a20 666c 6f61 7428 7966  0.15) * float(yf
+00014410: 202d 2079 6929 202f 2066 6c6f 6174 280a   - yi) / float(.
+00014420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014430: 2020 2020 2020 2020 4d41 585f 434f 4c4f          MAX_COLO
+00014440: 5552 5f4b 4559 0a20 2020 2020 2020 2020  UR_KEY.         
+00014450: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00014460: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+00014470: 6620 6b20 3e20 342e 353a 0a20 2020 2020  f k > 4.5:.     
+00014480: 2020 2020 2020 2020 2020 2020 2020 2079                 y
+00014490: 203d 2066 6c6f 6174 2879 6929 202b 2066   = float(yi) + f
+000144a0: 6c6f 6174 286b 2920 2a20 666c 6f61 7428  loat(k) * float(
+000144b0: 7966 202d 2079 6929 202f 2066 6c6f 6174  yf - yi) / float
+000144c0: 284d 4158 5f43 4f4c 4f55 525f 4b45 5929  (MAX_COLOUR_KEY)
+000144d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000144e0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000144f0: 2020 2020 2020 2020 2020 2079 203d 2066             y = f
+00014500: 6c6f 6174 2879 6929 202b 2066 6c6f 6174  loat(yi) + float
+00014510: 286b 202b 2030 2e31 2920 2a20 666c 6f61  (k + 0.1) * floa
+00014520: 7428 7966 202d 2079 6929 202f 2066 6c6f  t(yf - yi) / flo
+00014530: 6174 280a 2020 2020 2020 2020 2020 2020  at(.            
+00014540: 2020 2020 2020 2020 2020 2020 4d41 585f              MAX_
+00014550: 434f 4c4f 5552 5f4b 4559 0a20 2020 2020  COLOUR_KEY.     
+00014560: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00014570: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014580: 2020 6669 672e 6164 645f 616e 6e6f 7461    fig.add_annota
+00014590: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
+000145a0: 2020 2020 2020 2020 2020 7872 6566 3d22            xref="
+000145b0: 7061 7065 7222 2c0a 2020 2020 2020 2020  paper",.        
+000145c0: 2020 2020 2020 2020 2020 2020 7972 6566              yref
+000145d0: 3d22 7061 7065 7222 2c0a 2020 2020 2020  ="paper",.      
+000145e0: 2020 2020 2020 2020 2020 2020 2020 783d                x=
+000145f0: 7831 2c0a 2020 2020 2020 2020 2020 2020  x1,.            
+00014600: 2020 2020 2020 2020 793d 792c 0a20 2020          y=y,.   
+00014610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014620: 2074 6578 743d 6622 7b6b 7d22 2c0a 2020   text=f"{k}",.  
+00014630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014640: 2020 7368 6f77 6172 726f 773d 4661 6c73    showarrow=Fals
+00014650: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00014660: 2020 2020 2020 2079 7368 6966 743d 302c         yshift=0,
+00014670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014680: 2020 2020 2078 7368 6966 743d 3337 2c0a       xshift=37,.
+00014690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000146a0: 2020 2020 666f 6e74 5f73 697a 653d 3136      font_size=16
+000146b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000146c0: 2020 2020 2020 666f 6e74 5f63 6f6c 6f72        font_color
+000146d0: 3d22 626c 6163 6b22 2c0a 2020 2020 2020  ="black",.      
+000146e0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+000146f0: 2020 2020 2023 2061 6464 2074 6f70 2064       # add top d
+00014700: 6573 6372 6970 7469 6f6e 0a20 2020 2020  escription.     
+00014710: 2020 2066 6967 2e61 6464 5f61 6e6e 6f74     fig.add_annot
+00014720: 6174 696f 6e28 0a20 2020 2020 2020 2020  ation(.         
+00014730: 2020 2078 7265 663d 2270 6170 6572 222c     xref="paper",
+00014740: 0a20 2020 2020 2020 2020 2020 2079 7265  .            yre
+00014750: 663d 2270 6170 6572 222c 0a20 2020 2020  f="paper",.     
+00014760: 2020 2020 2020 2078 3d28 7830 202b 2078         x=(x0 + x
+00014770: 3129 202f 2032 2c0a 2020 2020 2020 2020  1) / 2,.        
+00014780: 2020 2020 793d 7969 2c0a 2020 2020 2020      y=yi,.      
+00014790: 2020 2020 2020 7465 7874 3d22 3c62 3e4c        text="<b>L
+000147a0: 6567 656e 643c 2f62 3e22 2c0a 2020 2020  egend</b>",.    
+000147b0: 2020 2020 2020 2020 616c 6967 6e3d 2263          align="c
+000147c0: 656e 7465 7222 2c0a 2020 2020 2020 2020  enter",.        
+000147d0: 2020 2020 7368 6f77 6172 726f 773d 4661      showarrow=Fa
+000147e0: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
+000147f0: 2079 7368 6966 743d 3333 2c0a 2020 2020   yshift=33,.    
+00014800: 2020 2020 2020 2020 7873 6869 6674 3d36          xshift=6
+00014810: 302c 0a20 2020 2020 2020 2020 2020 2066  0,.            f
+00014820: 6f6e 745f 7369 7a65 3d32 302c 0a20 2020  ont_size=20,.   
+00014830: 2020 2020 2020 2020 2066 6f6e 745f 636f           font_co
+00014840: 6c6f 723d 2262 6c61 636b 222c 0a20 2020  lor="black",.   
+00014850: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00014860: 7265 7475 726e 2066 6967 0a0a 2020 2020  return fig..    
+00014870: 6465 6620 5f70 6c6f 745f 6661 696c 7572  def _plot_failur
+00014880: 655f 706c 616e 6528 0a20 2020 2020 2020  e_plane(.       
+00014890: 2073 656c 662c 0a20 2020 2020 2020 2066   self,.        f
+000148a0: 6967 2c0a 2020 2020 2020 2020 635f 783a  ig,.        c_x:
+000148b0: 2066 6c6f 6174 2c0a 2020 2020 2020 2020   float,.        
+000148c0: 635f 793a 2066 6c6f 6174 2c0a 2020 2020  c_y: float,.    
+000148d0: 2020 2020 7261 6469 7573 3a20 666c 6f61      radius: floa
+000148e0: 742c 0a20 2020 2020 2020 206c 5f63 3a20  t,.        l_c: 
+000148f0: 7475 706c 652c 0a20 2020 2020 2020 2072  tuple,.        r
+00014900: 5f63 3a20 7475 706c 652c 0a20 2020 2020  _c: tuple,.     
+00014910: 2020 2046 4f53 3a20 666c 6f61 742c 0a20     FOS: float,. 
+00014920: 2020 2020 2020 2073 686f 775f 6365 6e74         show_cent
+00014930: 6572 3d46 616c 7365 2c0a 2020 2020 293a  er=False,.    ):
+00014940: 0a20 2020 2020 2020 2022 2222 4164 6420  .        """Add 
+00014950: 6661 696c 7572 6520 706c 616e 6520 746f  failure plane to
+00014960: 2070 6c6f 742e 0a0a 2020 2020 2020 2020   plot...        
+00014970: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+00014980: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00014990: 2020 2020 2020 6669 6720 3a20 706c 6f74        fig : plot
+000149a0: 6c79 2066 6967 7572 650a 2020 2020 2020  ly figure.      
+000149b0: 2020 2020 2020 706c 6f74 6c79 2066 6967        plotly fig
+000149c0: 7572 6520 746f 2068 6176 6520 696e 666f  ure to have info
+000149d0: 726d 6174 696f 6e20 6164 6465 6420 746f  rmation added to
+000149e0: 2e0a 2020 2020 2020 2020 635f 7820 3a20  ..        c_x : 
+000149f0: 666c 6f61 740a 2020 2020 2020 2020 2020  float.          
+00014a00: 2020 6661 696c 7572 6520 706c 616e 6520    failure plane 
+00014a10: 6369 7263 6c65 2063 656e 7465 7220 7820  circle center x 
+00014a20: 636f 6f72 6469 6e61 7465 2e0a 2020 2020  coordinate..    
+00014a30: 2020 2020 635f 7920 3a20 666c 6f61 740a      c_y : float.
+00014a40: 2020 2020 2020 2020 2020 2020 6661 696c              fail
+00014a50: 7572 6520 706c 616e 6520 6369 7263 6c65  ure plane circle
+00014a60: 2063 656e 7465 7220 7920 636f 6f72 6469   center y coordi
+00014a70: 6e61 7465 2e0a 2020 2020 2020 2020 7261  nate..        ra
+00014a80: 6469 7573 203a 2066 6c6f 6174 0a20 2020  dius : float.   
+00014a90: 2020 2020 2020 2020 2066 6169 6c75 7265           failure
+00014aa0: 2070 6c61 6e65 2063 6972 636c 6520 7261   plane circle ra
+00014ab0: 6469 7573 0a20 2020 2020 2020 206c 5f63  dius.        l_c
+00014ac0: 203a 2074 7570 6c65 0a20 2020 2020 2020   : tuple.       
+00014ad0: 2020 2020 206c 6566 7420 696e 7465 7273       left inters
+00014ae0: 6563 7469 6f6e 2070 6f69 6e74 2062 6574  ection point bet
+00014af0: 7765 656e 2066 6169 6c75 7265 2070 6c61  ween failure pla
+00014b00: 6e65 2061 6e64 2065 7874 6572 6e61 6c20  ne and external 
+00014b10: 626f 756e 6461 7279 2e0a 2020 2020 2020  boundary..      
+00014b20: 2020 725f 6320 3a20 7475 706c 650a 2020    r_c : tuple.  
+00014b30: 2020 2020 2020 2020 2020 7269 6768 7420            right 
+00014b40: 696e 7465 7273 6563 7469 6f6e 2070 6f69  intersection poi
+00014b50: 6e74 2062 6574 7765 656e 2066 6169 6c75  nt between failu
+00014b60: 7265 2070 6c61 6e65 2061 6e64 2065 7874  re plane and ext
+00014b70: 6572 6e61 6c20 626f 756e 6461 7279 2e0a  ernal boundary..
+00014b80: 2020 2020 2020 2020 464f 5320 3a20 666c          FOS : fl
+00014b90: 6f61 740a 2020 2020 2020 2020 2020 2020  oat.            
+00014ba0: 4661 6374 6f72 206f 6620 7361 6665 7479  Factor of safety
+00014bb0: 206f 6620 736c 6f70 6520 2875 7365 6420   of slope (used 
+00014bc0: 696e 2063 6f6c 6f72 696e 6720 6472 6177  in coloring draw
+00014bd0: 6e20 6661 696c 7572 6520 706c 616e 6529  n failure plane)
+00014be0: 0a20 2020 2020 2020 2073 686f 775f 6365  .        show_ce
+00014bf0: 6e74 6572 203a 2062 6f6f 6c2c 206f 7074  nter : bool, opt
+00014c00: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
+00014c10: 2020 4966 2074 7275 6520 7769 6c6c 2070    If true will p
+00014c20: 726f 6a65 6374 2074 6f20 7468 6520 6365  roject to the ce
+00014c30: 6e74 6572 206f 6620 6369 7263 6c65 2061  nter of circle a
+00014c40: 6e64 2073 686f 772c 2062 7920 6465 6661  nd show, by defa
+00014c50: 756c 7420 6661 6c73 652e 0a0a 2020 2020  ult false...    
+00014c60: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
+00014c70: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+00014c80: 2020 2020 706c 6f74 6c79 2066 6967 7572      plotly figur
+00014c90: 650a 2020 2020 2020 2020 2222 220a 0a20  e.        """.. 
+00014ca0: 2020 2020 2020 2063 5f78 203d 2072 6f75         c_x = rou
+00014cb0: 6e64 2863 5f78 2c20 3329 0a20 2020 2020  nd(c_x, 3).     
+00014cc0: 2020 2063 5f79 203d 2072 6f75 6e64 2863     c_y = round(c
+00014cd0: 5f79 2c20 3329 0a20 2020 2020 2020 2072  _y, 3).        r
+00014ce0: 6164 6975 7320 3d20 726f 756e 6428 7261  adius = round(ra
+00014cf0: 6469 7573 2c20 3329 0a20 2020 2020 2020  dius, 3).       
+00014d00: 2046 4f53 203d 2072 6f75 6e64 2846 4f53   FOS = round(FOS
+00014d10: 2c20 3329 0a0a 2020 2020 2020 2020 6966  , 3)..        if
+00014d20: 2046 4f53 203e 2035 3a0a 2020 2020 2020   FOS > 5:.      
+00014d30: 2020 2020 2020 636f 6c6f 7220 3d20 434f        color = CO
+00014d40: 4c4f 5552 5f46 4f53 5f44 4943 545b 352e  LOUR_FOS_DICT[5.
+00014d50: 305d 0a20 2020 2020 2020 2065 6c73 653a  0].        else:
+00014d60: 0a20 2020 2020 2020 2020 2020 2063 6f6c  .            col
+00014d70: 6f72 203d 2043 4f4c 4f55 525f 464f 535f  or = COLOUR_FOS_
+00014d80: 4449 4354 5b72 6f75 6e64 2846 4f53 2c20  DICT[round(FOS, 
+00014d90: 3129 5d0a 0a20 2020 2020 2020 2023 2067  1)]..        # g
+00014da0: 656e 6572 6174 6520 706f 696e 7473 2066  enerate points f
+00014db0: 6f72 2063 6972 636c 650a 2020 2020 2020  or circle.      
+00014dc0: 2020 782c 2079 203d 2075 7469 6c69 7469    x, y = utiliti
+00014dd0: 6573 2e67 656e 6572 6174 655f 6369 7263  es.generate_circ
+00014de0: 6c65 5f63 6f6f 7264 696e 6174 6573 2863  le_coordinates(c
+00014df0: 5f78 2c20 635f 792c 2072 6164 6975 7329  _x, c_y, radius)
+00014e00: 0a0a 2020 2020 2020 2020 2320 656d 7074  ..        # empt
+00014e10: 7920 7665 6374 6f72 7320 666f 7220 6369  y vectors for ci
+00014e20: 7263 6c65 2070 6f69 6e74 7320 7468 6174  rcle points that
+00014e30: 2077 6520 7769 6c6c 2061 6374 7561 6c6c   we will actuall
+00014e40: 7920 696e 636c 7564 650a 2020 2020 2020  y include.      
+00014e50: 2020 785f 203d 205b 5d0a 2020 2020 2020    x_ = [].      
+00014e60: 2020 795f 203d 205b 5d0a 0a20 2020 2020    y_ = []..     
+00014e70: 2020 2023 2036 3520 6c6f 6e67 206c 6973     # 65 long lis
+00014e80: 7420 6275 7420 7468 6520 6c61 7374 2068  t but the last h
+00014e90: 616c 6620 6f66 2070 6f69 6e74 7320 6172  alf of points ar
+00014ea0: 6520 666f 7220 7468 6520 746f 7020 6861  e for the top ha
+00014eb0: 6c66 206f 660a 2020 2020 2020 2020 2320  lf of.        # 
+00014ec0: 6369 7263 6c65 2061 6e64 2073 6f20 7769  circle and so wi
+00014ed0: 6c6c 206e 6576 6572 2061 6374 7561 6c6c  ll never actuall
+00014ee0: 7920 6265 2072 6571 7569 7265 642e 0a20  y be required.. 
+00014ef0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+00014f00: 7261 6e67 6528 6c65 6e28 7829 293a 0a20  range(len(x)):. 
+00014f10: 2020 2020 2020 2020 2020 2023 2078 2063             # x c
+00014f20: 6f6f 7264 696e 6174 6520 7368 6f75 6c64  oordinate should
+00014f30: 2062 6520 6265 7477 6565 6e20 6c65 6674   be between left
+00014f40: 2061 6e64 2072 6967 6874 0a20 2020 2020   and right.     
+00014f50: 2020 2020 2020 2023 206e 6f74 6520 666f         # note fo
+00014f60: 7220 792c 2073 686f 756c 6420 6265 206c  r y, should be l
+00014f70: 6573 7320 7468 616e 206c 6566 7420 7920  ess than left y 
+00014f80: 6275 7420 6361 6e20 7374 6f6f 700a 2020  but can stoop.  
+00014f90: 2020 2020 2020 2020 2020 2320 6265 6c6f            # belo
+00014fa0: 7720 7269 6768 7420 690a 2020 2020 2020  w right i.      
+00014fb0: 2020 2020 2020 6966 2078 5b69 5d20 3c3d        if x[i] <=
+00014fc0: 2072 5f63 5b30 5d20 616e 6420 785b 695d   r_c[0] and x[i]
+00014fd0: 203e 3d20 6c5f 635b 305d 2061 6e64 2079   >= l_c[0] and y
+00014fe0: 5b69 5d20 3c3d 206c 5f63 5b31 5d3a 0a20  [i] <= l_c[1]:. 
+00014ff0: 2020 2020 2020 2020 2020 2020 2020 2078                 x
+00015000: 5f2e 6170 7065 6e64 2878 5b69 5d29 0a20  _.append(x[i]). 
+00015010: 2020 2020 2020 2020 2020 2020 2020 2079                 y
+00015020: 5f2e 6170 7065 6e64 2879 5b69 5d29 0a0a  _.append(y[i])..
+00015030: 2020 2020 2020 2020 6966 2073 686f 775f          if show_
+00015040: 6365 6e74 6572 3a0a 2020 2020 2020 2020  center:.        
+00015050: 2020 2020 785f 202b 3d20 5b72 5f63 5b30      x_ += [r_c[0
+00015060: 5d2c 2063 5f78 2c20 6c5f 635b 305d 2c20  ], c_x, l_c[0], 
+00015070: 785f 5b30 5d5d 0a20 2020 2020 2020 2020  x_[0]].         
+00015080: 2020 2079 5f20 2b3d 205b 725f 635b 315d     y_ += [r_c[1]
+00015090: 2c20 635f 792c 206c 5f63 5b31 5d2c 2079  , c_y, l_c[1], y
+000150a0: 5f5b 305d 5d0a 2020 2020 2020 2020 656c  _[0]].        el
+000150b0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000150c0: 785f 203d 205b 6c5f 635b 305d 5d20 2b20  x_ = [l_c[0]] + 
+000150d0: 785f 202b 205b 725f 635b 305d 5d0a 2020  x_ + [r_c[0]].  
+000150e0: 2020 2020 2020 2020 2020 795f 203d 205b            y_ = [
+000150f0: 6c5f 635b 315d 5d20 2b20 795f 202b 205b  l_c[1]] + y_ + [
+00015100: 725f 635b 315d 5d0a 0a20 2020 2020 2020  r_c[1]]..       
+00015110: 2023 2054 4849 5320 4953 2054 4f4f 2053   # THIS IS TOO S
+00015120: 4c4f 5720 2869 6e20 6578 7065 7269 6d65  LOW (in experime
+00015130: 6e74 6174 696f 6e20 7468 6520 7265 616c  ntation the real
+00015140: 0a20 2020 2020 2020 2023 2070 726f 626c  .        # probl
+00015150: 656d 2069 7320 7769 7468 2070 6c6f 746c  em is with plotl
+00015160: 792c 2065 7665 6e20 7769 7468 206d 696e  y, even with min
+00015170: 696d 616c 2064 6174 610a 2020 2020 2020  imal data.      
+00015180: 2020 2320 6164 6469 6e67 2065 7665 7279    # adding every
+00015190: 7468 696e 6720 696e 2069 7320 736c 6f77  thing in is slow
+000151a0: 290a 2020 2020 2020 2020 6669 672e 6164  ).        fig.ad
+000151b0: 645f 7472 6163 6528 0a20 2020 2020 2020  d_trace(.       
+000151c0: 2020 2020 2067 6f2e 5363 6174 7465 7228       go.Scatter(
+000151d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000151e0: 2078 3d78 5f2c 0a20 2020 2020 2020 2020   x=x_,.         
+000151f0: 2020 2020 2020 2079 3d79 5f2c 0a20 2020         y=y_,.   
+00015200: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
+00015210: 653d 226c 696e 6573 222c 0a20 2020 2020  e="lines",.     
+00015220: 2020 2020 2020 2020 2020 206c 696e 655f             line_
+00015230: 636f 6c6f 723d 636f 6c6f 722c 0a20 2020  color=color,.   
+00015240: 2020 2020 2020 2020 2020 2020 2068 6f76               hov
+00015250: 6572 7465 6d70 6c61 7465 3d22 222c 0a20  ertemplate="",. 
+00015260: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00015270: 6578 7474 656d 706c 6174 653d 2222 2c0a  exttemplate="",.
+00015280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015290: 6e61 6d65 3d22 222c 0a20 2020 2020 2020  name="",.       
+000152a0: 2020 2020 2029 0a20 2020 2020 2020 2029       ).        )
+000152b0: 0a0a 2020 2020 2020 2020 2320 6966 2073  ..        # if s
+000152c0: 686f 7720 6365 6e74 6572 2061 6464 2061  how center add a
+000152d0: 6e6e 6f74 6174 696f 6e20 7769 7468 2068  nnotation with h
+000152e0: 6f76 6572 6c61 6265 6c20 616e 6420 7465  overlabel and te
+000152f0: 7874 0a20 2020 2020 2020 2069 6620 7368  xt.        if sh
+00015300: 6f77 5f63 656e 7465 723a 0a20 2020 2020  ow_center:.     
+00015310: 2020 2020 2020 2066 6967 203d 2073 656c         fig = sel
+00015320: 662e 5f70 6c6f 745f 616e 6e6f 7461 7465  f._plot_annotate
+00015330: 5f46 4f53 2866 6967 2c20 635f 782c 2063  _FOS(fig, c_x, c
+00015340: 5f79 2c20 7261 6469 7573 2c20 464f 5329  _y, radius, FOS)
+00015350: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00015360: 2066 6967 0a0a 0a69 6620 5f5f 6e61 6d65   fig...if __name
+00015370: 5f5f 203d 3d20 225f 5f6d 6169 6e5f 5f22  __ == "__main__"
+00015380: 3a0a 2020 2020 7320 3d20 536c 6f70 6528  :.    s = Slope(
+00015390: 6865 6967 6874 3d31 2c20 616e 676c 653d  height=1, angle=
+000153a0: 4e6f 6e65 2c20 6c65 6e67 7468 3d31 290a  None, length=1).
+000153b0: 0a20 2020 206d 3120 3d20 4d61 7465 7269  .    m1 = Materi
+000153c0: 616c 2832 302c 2033 352c 2030 2c20 302e  al(20, 35, 0, 0.
+000153d0: 3529 0a20 2020 206d 3220 3d20 4d61 7465  5).    m2 = Mate
+000153e0: 7269 616c 2832 302c 2033 352c 2032 2c20  rial(20, 35, 2, 
+000153f0: 3129 0a20 2020 206d 3320 3d20 4d61 7465  1).    m3 = Mate
+00015400: 7269 616c 2831 382c 2033 302c 2030 2c20  rial(18, 30, 0, 
+00015410: 3529 0a0a 2020 2020 732e 7365 745f 6d61  5)..    s.set_ma
+00015420: 7465 7269 616c 7328 6d31 2c20 6d32 2c20  terials(m1, m2, 
+00015430: 6d33 290a 0a20 2020 2073 2e75 7064 6174  m3)..    s.updat
+00015440: 655f 616e 616c 7973 6973 5f6f 7074 696f  e_analysis_optio
+00015450: 6e73 2873 6c69 6365 733d 3130 2c20 6974  ns(slices=10, it
+00015460: 6572 6174 696f 6e73 3d35 3030 290a 0a20  erations=500).. 
+00015470: 2020 2073 2e73 6574 5f77 6174 6572 5f74     s.set_water_t
+00015480: 6162 6c65 2830 2e37 290a 2020 2020 732e  able(0.7).    s.
+00015490: 616e 616c 7973 655f 736c 6f70 6528 290a  analyse_slope().
+000154a0: 0a20 2020 2023 2070 7269 6e74 2074 6865  .    # print the
+000154b0: 2063 7269 7469 6361 6c20 464f 5320 666f   critical FOS fo
+000154c0: 7220 7468 6520 736c 6f70 650a 2020 2020  r the slope.    
+000154d0: 7072 696e 7428 2266 6f73 3a22 2c20 732e  print("fos:", s.
+000154e0: 6765 745f 6d69 6e5f 464f 5328 2929 0a0a  get_min_FOS())..
+000154f0: 2020 2020 2320 706c 6f74 2074 6865 2063      # plot the c
+00015500: 7269 7469 6361 6c20 6661 696c 7572 6520  ritical failure 
+00015510: 7375 7266 6163 650a 2020 2020 6669 675f  surface.    fig_
+00015520: 3120 3d20 732e 706c 6f74 5f61 6c6c 5f70  1 = s.plot_all_p
+00015530: 6c61 6e65 7328 6d61 785f 666f 733d 4e6f  lanes(max_fos=No
+00015540: 6e65 290a 2020 2020 6669 675f 312e 7570  ne).    fig_1.up
+00015550: 6461 7465 5f6c 6179 6f75 7428 7769 6474  date_layout(widt
+00015560: 683d 3132 3030 2c20 6865 6967 6874 3d37  h=1200, height=7
+00015570: 3030 290a 2020 2020 6669 675f 312e 7368  00).    fig_1.sh
+00015580: 6f77 2829 0a                             ow().
```

### Comparing `pyslope-1.1.9/pyslope/utilities.py` & `pyslope-1.2.0/pyslope/utilities.py`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/pyslope.egg-info/PKG-INFO` & `pyslope-1.2.0/pyslope.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 Metadata-Version: 2.1
 Name: pyslope
-Version: 1.1.9
+Version: 1.2.0
 Summary: A 2D Slope Stability Software using bishops method
 Home-page: https://github.com/JesseBonanno/pyslope
 Author: Jesse Bonanno
 Author-email: jessebonanno@gmail.com
 License: MIT
-Download-URL: https://github.com/JesseBonanno/pyslope/archive/v1.1.9.tar.gz
+Download-URL: https://github.com/JesseBonanno/pyslope/archive/v1.2.0.tar.gz
 Description: # pySlope
         
         
         [![PyPi](https://img.shields.io/pypi/v/pyslope.svg)](https://pypi.org/project/pyslope/)
         [![License](https://img.shields.io/badge/license-MIT-lightgreen.svg)](https://github.com/JesseBonanno/pyslope/blob/main/LICENSE.txt)
         [![CodeFactor](https://www.codefactor.io/repository/github/jessebonanno/pyslope/badge?s=43db3d31fb1ca55747ede7e5205c7d9e0cf37ced)](https://www.codefactor.io/repository/github/jessebonanno/pyslope)
         [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JesseBonanno/pyslope/main?filepath=pyslope%2Fexamples%2Freadme_example.ipynb)
         [![Documentation Status](https://readthedocs.org/projects/pyslope/badge/?version=latest)](https://pyslope.readthedocs.io/en/latest)
         [![Code Style](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black)
         [![Downloads](https://pepy.tech/badge/pyslope)](https://pepy.tech/project/pyslope)
         [![codecov](https://codecov.io/gh/JesseBonanno/PySlope/branch/main/graph/badge.svg?token=ASUIW54CXV)](https://codecov.io/gh/JesseBonanno/PySlope)
         [![CI](https://github.com/JesseBonanno/PySlope/actions/workflows/ci.yaml/badge.svg)](https://github.com/JesseBonanno/PySlope/actions/workflows/ci.yaml)
         [![pre-commit](https://github.com/JesseBonanno/PySlope/actions/workflows/pre-commit.yaml/badge.svg)](https://github.com/JesseBonanno/PySlope/actions/workflows/pre-commit.yaml)
+        [![Website](https://img.shields.io/badge/website-up-brightgreen)](https://pyslope.herokuapp.com/)
+        
         
         pySlope is a 2D slope stability module based on bishops method of slices. This module allows for the following parameters:
            - unlimited horizontal geological units
            - water table
            - uniform loads
            - line loads
            - slope search limits
          
         This module can return plots for the critical failure slope or plots for all failure slopes below a certain factor of safety.
         
         ## Project Purpose
         
         The purpose of this project is two fold:
         
-           1. Create a free online slope stability software
+           1. Create a free online slope stability software [![Website](https://img.shields.io/badge/website-up-brightgreen)](https://pyslope.herokuapp.com/)
            2. Provide a pythonic solution to implementing Bishop's method based on object oriented coding principles
         
         Performing a slope stability calculation by hand is extremely uneconimical and time consuming. The problem involves a lot of geometrical mathematics which can make the calculation hard to achieve with only excel. Python packages exist for geometrical mathematics which makes Python well suited for implementing a slope stability analysis package. There is however, no well-documented open-source slope stability software that can currently be found online. This package aims to fill that gap.
         
         ## Functionality and usage
         
         A typical use case of the `pySlope` package involves the following steps:
@@ -280,28 +282,30 @@
         ```
         
         Releasing
         ---------
         
         Releases are published automatically when a tag is pushed to GitHub.
         
-        .. code-block:: bash
+        ```shell
+        # Set next version number
+        export RELEASE=vX.X.X
         
-           # Set next version number
-           export RELEASE=vX.X.X
+        # Create tags
+        git commit --allow-empty -m "Release $RELEASE"
+        git tag -a $RELEASE -m "Version $RELEASE"
         
-           # Create tags
-           git commit --allow-empty -m "Release $RELEASE"
-           git tag -a $RELEASE -m "Version $RELEASE"
+        # Push (for working from a fork)
+        git push upstream --tags
         
-           # Push (for working from a fork)
-           git push upstream --tags
+        # if not working from fork would instead be
+        # git push origin --tags
+        ```
         
-           # if not working from fork would instead be
-           # git push origin --tags
+        Or set a tag with Github Desktop.
         
         ## License
         
         [![License](https://img.shields.io/badge/license-MIT-lightgreen.svg)](https://github.com/JesseBonanno/pyslope/blob/main/LICENSE.txt)
         
 Keywords: geotechnical,slope,stability,civil,engineering,bishops
 Platform: UNKNOWN
```

### Comparing `pyslope-1.1.9/pyslope.egg-info/SOURCES.txt` & `pyslope-1.2.0/pyslope.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,22 @@
 pyslope/pyslope.py
 pyslope/utilities.py
 pyslope.egg-info/PKG-INFO
 pyslope.egg-info/SOURCES.txt
 pyslope.egg-info/dependency_links.txt
 pyslope.egg-info/requires.txt
 pyslope.egg-info/top_level.txt
+pyslope/docs/Makefile
+pyslope/docs/conf.py
+pyslope/docs/docstrings.rst
+pyslope/docs/examples.rst
+pyslope/docs/index.rst
+pyslope/docs/installation.rst
+pyslope/docs/make.bat
+pyslope/docs/requirements_docs.txt
 pyslope/examples/readme_example.ipynb
 pyslope/examples/readme_example_plot_all_maxfos2.png
 pyslope/examples/readme_example_plot_boundary.png
 pyslope/examples/readme_example_plot_critical.png
 pyslope/examples/readme_example_plot_dynamic.png
 pyslope/examples/search.xlsx
 pyslope/examples/slices.xlsx
@@ -53,8 +61,11 @@
 pyslope/examples/slide/d.slim
 pyslope/examples/slide/e.slim
 pyslope/examples/slide/f.slim
 pyslope/examples/slide/slide.png
 pyslope/graphs/graphs.ipynb
 pyslope/graphs/sandstone_fill_5m_1_1.html
 pyslope/graphs/sandstone_fill_FOS_1.25_for_loads_and_angles.html
-pyslope/tests/test_slope.py
+pyslope/paper/paper.md
+pyslope/paper/pySlope_paper.pdf
+pyslope/tests/test_slope.py
+pyslope/tests/test_validation_examples.py
```

### Comparing `pyslope-1.1.9/setup.py` & `pyslope-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `pyslope-1.1.9/versioneer.py` & `pyslope-1.2.0/versioneer.py`

 * *Files identical despite different names*

