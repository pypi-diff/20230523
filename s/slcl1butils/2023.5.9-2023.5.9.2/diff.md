# Comparing `tmp/slcl1butils-2023.5.9.tar.gz` & `tmp/slcl1butils-2023.5.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slcl1butils-2023.5.9.tar", last modified: Tue May  9 10:09:37 2023, max compression
+gzip compressed data, was "slcl1butils-2023.5.9.2.tar", last modified: Tue May  9 14:55:01 2023, max compression
```

## Comparing `slcl1butils-2023.5.9.tar` & `slcl1butils-2023.5.9.2.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:37.044831 slcl1butils-2023.5.9/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:37.032831 slcl1butils-2023.5.9/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:37.032831 slcl1butils-2023.5.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-09 10:09:37.044831 slcl1butils-2023.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:37.028831 slcl1butils-2023.5.9/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:37.032831 slcl1butils-2023.5.9/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/ci/requirements/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/ci/requirements/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:37.036831 slcl1butils-2023.5.9/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:37.028831 slcl1butils-2023.5.9/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:37.036831 slcl1butils-2023.5.9/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/docs/_static/css/slcl1butils.css
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/docs/basic_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:37.036831 slcl1butils-2023.5.9/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/docs/examples/display_a_IW_L1B_xspectra.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/docs/examples/do_L1C_SAFE_from_L1B_SAFE_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/docs/examples/intro.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/docs/examples/plotting_L1B_geometry_with_holoview_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/docs/examples/plotting_L1B_variables_with_holoview_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)    59687 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/docs/oceanspectrumSAR.png
--rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/get_polygons_from_l1b.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/requirements_doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 10:09:37.044831 slcl1butils-2023.5.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:37.036831 slcl1butils-2023.5.9/slcl1butils/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:37.040831 slcl1butils-2023.5.9/slcl1butils/coloc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/coloc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/coloc/coloc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:37.040831 slcl1butils-2023.5.9/slcl1butils/compute/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/compute/compute_from_l1b.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/compute/cwave.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/compute/macs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/compute/stack_iw_l1b.py
--rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/compute/stack_wv_l1c_monthly.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/conversion_polar_cartesian.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/cwave_parameters_computation_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/get_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/get_polygons_from_l1b.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:37.040831 slcl1butils-2023.5.9/slcl1butils/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/plotting/add_azimuth_cutoff_lines_on_polar_spec_fig.py
--rw-r--r--   0 runner    (1001) docker     (123)    20411 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/plotting/display_one_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)    12819 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/plotting/display_xspectra_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/plotting/plotting_L1B_geometry_with_holoview_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/plotting/plotting_L1B_variables_with_holoview_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/plotting/spectra_plot_circles_wavenumbers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/raster_readers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:37.044831 slcl1butils-2023.5.9/slcl1butils/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      563 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.pbs
--rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1858 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE_prun.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.pbs
--rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/spectrum_clockwise_to_trigo.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/spectrum_rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/symmetrize_l1b_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-09 10:09:19.000000 slcl1butils-2023.5.9/slcl1butils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:09:37.040831 slcl1butils-2023.5.9/slcl1butils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-09 10:09:37.000000 slcl1butils-2023.5.9/slcl1butils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-09 10:09:37.000000 slcl1butils-2023.5.9/slcl1butils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 10:09:37.000000 slcl1butils-2023.5.9/slcl1butils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-09 10:09:37.000000 slcl1butils-2023.5.9/slcl1butils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-09 10:09:37.000000 slcl1butils-2023.5.9/slcl1butils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 10:09:37.000000 slcl1butils-2023.5.9/slcl1butils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:55:01.796081 slcl1butils-2023.5.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:55:01.792081 slcl1butils-2023.5.9.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:55:01.792081 slcl1butils-2023.5.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-09 14:55:01.796081 slcl1butils-2023.5.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:55:01.792081 slcl1butils-2023.5.9.2/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:55:01.792081 slcl1butils-2023.5.9.2/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/ci/requirements/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/ci/requirements/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:55:01.792081 slcl1butils-2023.5.9.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:55:01.792081 slcl1butils-2023.5.9.2/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:55:01.792081 slcl1butils-2023.5.9.2/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/docs/_static/css/slcl1butils.css
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/docs/basic_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:55:01.792081 slcl1butils-2023.5.9.2/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/docs/examples/display_a_IW_L1B_xspectra.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/docs/examples/do_L1C_SAFE_from_L1B_SAFE_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/docs/examples/intro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/docs/examples/plotting_L1B_geometry_with_holoview_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/docs/examples/plotting_L1B_variables_with_holoview_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    59687 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/docs/oceanspectrumSAR.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/get_polygons_from_l1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/requirements_doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 14:55:01.796081 slcl1butils-2023.5.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:55:01.796081 slcl1butils-2023.5.9.2/slcl1butils/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:55:01.796081 slcl1butils-2023.5.9.2/slcl1butils/coloc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/coloc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/coloc/coloc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:55:01.796081 slcl1butils-2023.5.9.2/slcl1butils/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/compute/compute_from_l1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/compute/cwave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/compute/macs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/compute/stack_iw_l1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/compute/stack_wv_l1c_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/conversion_polar_cartesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/cwave_parameters_computation_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/get_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/get_polygons_from_l1b.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:55:01.796081 slcl1butils-2023.5.9.2/slcl1butils/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/plotting/add_azimuth_cutoff_lines_on_polar_spec_fig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20411 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/plotting/display_one_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12819 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/plotting/display_xspectra_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/plotting/plotting_L1B_geometry_with_holoview_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/plotting/plotting_L1B_variables_with_holoview_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/plotting/spectra_plot_circles_wavenumbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/raster_readers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:55:01.796081 slcl1butils-2023.5.9.2/slcl1butils/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      563 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.pbs
+-rw-r--r--   0 runner    (1001) docker     (123)    13011 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1858 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE_prun.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.pbs
+-rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/spectrum_clockwise_to_trigo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/spectrum_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/symmetrize_l1b_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-09 14:54:41.000000 slcl1butils-2023.5.9.2/slcl1butils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:55:01.796081 slcl1butils-2023.5.9.2/slcl1butils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-09 14:55:01.000000 slcl1butils-2023.5.9.2/slcl1butils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-09 14:55:01.000000 slcl1butils-2023.5.9.2/slcl1butils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 14:55:01.000000 slcl1butils-2023.5.9.2/slcl1butils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-09 14:55:01.000000 slcl1butils-2023.5.9.2/slcl1butils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-09 14:55:01.000000 slcl1butils-2023.5.9.2/slcl1butils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 14:55:01.000000 slcl1butils-2023.5.9.2/slcl1butils.egg-info/top_level.txt
```

### Comparing `slcl1butils-2023.5.9/.github/workflows/publish.yml` & `slcl1butils-2023.5.9.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/.gitignore` & `slcl1butils-2023.5.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/.pre-commit-config.yaml` & `slcl1butils-2023.5.9.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/LICENSE` & `slcl1butils-2023.5.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/PKG-INFO` & `slcl1butils-2023.5.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slcl1butils
-Version: 2023.5.9
+Version: 2023.5.9.2
 Summary: Python library to exploit SAR IFREMER L1B products
 Author: Alexis Mouche
 License: GPL-3.0
 Keywords: SAR,wave,reseach,cross-spectra
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `slcl1butils-2023.5.9/docs/Makefile` & `slcl1butils-2023.5.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/docs/conf.py` & `slcl1butils-2023.5.9.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/docs/examples/display_a_IW_L1B_xspectra.ipynb` & `slcl1butils-2023.5.9.2/docs/examples/display_a_IW_L1B_xspectra.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/docs/examples/do_L1C_SAFE_from_L1B_SAFE_example.ipynb` & `slcl1butils-2023.5.9.2/docs/examples/do_L1C_SAFE_from_L1B_SAFE_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/docs/examples/plotting_L1B_geometry_with_holoview_example.ipynb` & `slcl1butils-2023.5.9.2/docs/examples/plotting_L1B_geometry_with_holoview_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/docs/examples/plotting_L1B_variables_with_holoview_example.ipynb` & `slcl1butils-2023.5.9.2/docs/examples/plotting_L1B_variables_with_holoview_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/docs/index.rst` & `slcl1butils-2023.5.9.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/docs/installing.rst` & `slcl1butils-2023.5.9.2/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/docs/oceanspectrumSAR.png` & `slcl1butils-2023.5.9.2/docs/oceanspectrumSAR.png`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/get_polygons_from_l1b.py` & `slcl1butils-2023.5.9.2/get_polygons_from_l1b.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/pyproject.toml` & `slcl1butils-2023.5.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/slcl1butils/coloc/coloc.py` & `slcl1butils-2023.5.9.2/slcl1butils/coloc/coloc.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/slcl1butils/compute/compute_from_l1b.py` & `slcl1butils-2023.5.9.2/slcl1butils/compute/compute_from_l1b.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/slcl1butils/compute/cwave.py` & `slcl1butils-2023.5.9.2/slcl1butils/compute/cwave.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/slcl1butils/compute/macs.py` & `slcl1butils-2023.5.9.2/slcl1butils/compute/macs.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/slcl1butils/compute/stack_iw_l1b.py` & `slcl1butils-2023.5.9.2/slcl1butils/compute/stack_iw_l1b.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/slcl1butils/compute/stack_wv_l1c_monthly.py` & `slcl1butils-2023.5.9.2/slcl1butils/compute/stack_wv_l1c_monthly.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/slcl1butils/conversion_polar_cartesian.py` & `slcl1butils-2023.5.9.2/slcl1butils/conversion_polar_cartesian.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/slcl1butils/cwave_parameters_computation_example.ipynb` & `slcl1butils-2023.5.9.2/slcl1butils/cwave_parameters_computation_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/slcl1butils/get_config.py` & `slcl1butils-2023.5.9.2/slcl1butils/get_config.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/slcl1butils/get_polygons_from_l1b.py` & `slcl1butils-2023.5.9.2/slcl1butils/get_polygons_from_l1b.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/slcl1butils/plotting/add_azimuth_cutoff_lines_on_polar_spec_fig.py` & `slcl1butils-2023.5.9.2/slcl1butils/plotting/add_azimuth_cutoff_lines_on_polar_spec_fig.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/slcl1butils/plotting/display_one_spectra.py` & `slcl1butils-2023.5.9.2/slcl1butils/plotting/display_one_spectra.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/slcl1butils/plotting/display_xspectra_grid.py` & `slcl1butils-2023.5.9.2/slcl1butils/plotting/display_xspectra_grid.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/slcl1butils/plotting/plotting_L1B_geometry_with_holoview_example.ipynb` & `slcl1butils-2023.5.9.2/slcl1butils/plotting/plotting_L1B_geometry_with_holoview_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/slcl1butils/plotting/plotting_L1B_variables_with_holoview_example.ipynb` & `slcl1butils-2023.5.9.2/slcl1butils/plotting/plotting_L1B_variables_with_holoview_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/slcl1butils/plotting/spectra_plot_circles_wavenumbers.py` & `slcl1butils-2023.5.9.2/slcl1butils/plotting/spectra_plot_circles_wavenumbers.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/slcl1butils/raster_readers.py` & `slcl1butils-2023.5.9.2/slcl1butils/raster_readers.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.pbs` & `slcl1butils-2023.5.9.2/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.pbs`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.py` & `slcl1butils-2023.5.9.2/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         l1c_full_path = get_l1c_filepath(l1b_fullpath,version=version, outputdir=outputdir)
         if os.path.exists(l1c_full_path) and overwrite is False:
             logging.info('%s already exists', l1c_full_path)
         else:
             ds_intra, ds_inter = enrich_onesubswath_l1b(l1b_fullpath, ancillary_list=None, cwave=cwave, macs=macs,
                                                         colocat=colocat,
                                                         time_separation=time_separation)
-            if 'xspectra' in ds_inter:
+            if 'macs_Im' in ds_inter: # if macs is not computed -> XS not available -> no need to create L1C
                 save_l1c_to_netcdf(l1c_full_path, ds_intra, ds_inter,version=version)
                 cpt['saved_in_nc'] += 1
             else:
                 logging.info('there is no xspectra in this subswath -> the L1C will not be saved')
                 cpt['L1B_without_spectra'] += 1
     logging.info('cpt: %s',cpt)
     return 0
```

### Comparing `slcl1butils-2023.5.9/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE_prun.py` & `slcl1butils-2023.5.9.2/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE_prun.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.pbs` & `slcl1butils-2023.5.9.2/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.pbs`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.py` & `slcl1butils-2023.5.9.2/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/slcl1butils/spectrum_clockwise_to_trigo.py` & `slcl1butils-2023.5.9.2/slcl1butils/spectrum_clockwise_to_trigo.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/slcl1butils/spectrum_rotation.py` & `slcl1butils-2023.5.9.2/slcl1butils/spectrum_rotation.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/slcl1butils/symmetrize_l1b_spectra.py` & `slcl1butils-2023.5.9.2/slcl1butils/symmetrize_l1b_spectra.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/slcl1butils/utils.py` & `slcl1butils-2023.5.9.2/slcl1butils/utils.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.9/slcl1butils.egg-info/PKG-INFO` & `slcl1butils-2023.5.9.2/slcl1butils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slcl1butils
-Version: 2023.5.9
+Version: 2023.5.9.2
 Summary: Python library to exploit SAR IFREMER L1B products
 Author: Alexis Mouche
 License: GPL-3.0
 Keywords: SAR,wave,reseach,cross-spectra
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `slcl1butils-2023.5.9/slcl1butils.egg-info/SOURCES.txt` & `slcl1butils-2023.5.9.2/slcl1butils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

