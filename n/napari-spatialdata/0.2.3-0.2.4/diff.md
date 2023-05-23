# Comparing `tmp/napari-spatialdata-0.2.3.tar.gz` & `tmp/napari-spatialdata-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-spatialdata-0.2.3.tar", last modified: Thu May 11 11:24:02 2023, max compression
+gzip compressed data, was "napari-spatialdata-0.2.4.tar", last modified: Tue May 23 16:22:43 2023, max compression
```

## Comparing `napari-spatialdata-0.2.3.tar` & `napari-spatialdata-0.2.4.tar`

### file list

```diff
@@ -1,77 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:24:02.256269 napari-spatialdata-0.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:24:02.212270 napari-spatialdata-0.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:24:02.224270 napari-spatialdata-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/.mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:24:02.224270 napari-spatialdata-0.2.3/.napari/
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/.napari/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-05-11 11:24:02.256269 napari-spatialdata-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:24:02.228270 napari-spatialdata-0.2.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:24:02.228270 napari-spatialdata-0.2.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/docs/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:24:02.228270 napari-spatialdata-0.2.3/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/docs/_templates/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:24:02.228270 napari-spatialdata-0.2.3/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/docs/api.md
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:24:02.232270 napari-spatialdata-0.2.3/docs/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/docs/extensions/typed_returns.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:24:02.240270 napari-spatialdata-0.2.3/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)  2807648 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/docs/notebooks/mibitof_analysis.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  3449197 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/docs/notebooks/nanostring_analysis.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  5522494 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/docs/notebooks/spatialdata.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/docs/references.bib
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/docs/references.md
--rw-r--r--   0 runner    (1001) docker     (123)    16428 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/docs/template_usage.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:24:02.248269 napari-spatialdata-0.2.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/examples/spatialdata_mibitof.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/examples/spatialdata_nanostring.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/examples/spatialdata_visium.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-11 11:24:02.260269 napari-spatialdata-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:24:02.216270 napari-spatialdata-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:24:02.252269 napari-spatialdata-0.2.3/src/napari_spatialdata/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/src/napari_spatialdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/src/napari_spatialdata/_categoricals_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:24:02.256269 napari-spatialdata-0.2.3/src/napari_spatialdata/_constants/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/src/napari_spatialdata/_constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/src/napari_spatialdata/_constants/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/src/napari_spatialdata/_constants/_pkg_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/src/napari_spatialdata/_constants/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/src/napari_spatialdata/_interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     9962 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/src/napari_spatialdata/_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/src/napari_spatialdata/_scatterwidgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/src/napari_spatialdata/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-11 11:24:02.000000 napari-spatialdata-0.2.3/src/napari_spatialdata/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/src/napari_spatialdata/_view.py
--rw-r--r--   0 runner    (1001) docker     (123)    17675 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/src/napari_spatialdata/_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/src/napari_spatialdata/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:24:02.256269 napari-spatialdata-0.2.3/src/napari_spatialdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-05-11 11:24:02.000000 napari-spatialdata-0.2.3/src/napari_spatialdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-11 11:24:02.000000 napari-spatialdata-0.2.3/src/napari_spatialdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 11:24:02.000000 napari-spatialdata-0.2.3/src/napari_spatialdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-11 11:24:02.000000 napari-spatialdata-0.2.3/src/napari_spatialdata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-11 11:24:02.000000 napari-spatialdata-0.2.3/src/napari_spatialdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 11:24:02.000000 napari-spatialdata-0.2.3/src/napari_spatialdata.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 11:24:02.256269 napari-spatialdata-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/tests/test_interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/tests/test_scatterwidgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/tests/test_spatialdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-11 11:23:34.000000 napari-spatialdata-0.2.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:43.373450 napari-spatialdata-0.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:43.345449 napari-spatialdata-0.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:43.349449 napari-spatialdata-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/.mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:43.349449 napari-spatialdata-0.2.4/.napari/
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/.napari/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-05-23 16:22:43.373450 napari-spatialdata-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:43.353449 napari-spatialdata-0.2.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:43.353449 napari-spatialdata-0.2.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/docs/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:43.353449 napari-spatialdata-0.2.4/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/docs/_templates/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:43.353449 napari-spatialdata-0.2.4/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/docs/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/docs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:43.353449 napari-spatialdata-0.2.4/docs/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/docs/extensions/typed_returns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:43.361449 napari-spatialdata-0.2.4/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)  2807648 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/docs/notebooks/mibitof_analysis.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  3449197 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/docs/notebooks/nanostring_analysis.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   250844 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/docs/notebooks/scatterwidget.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  5522494 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/docs/notebooks/spatialdata.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/docs/references.bib
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/docs/references.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16450 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/docs/template_usage.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:43.369449 napari-spatialdata-0.2.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/examples/spatialdata_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/examples/spatialdata_visium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-23 16:22:43.373450 napari-spatialdata-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:43.345449 napari-spatialdata-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:43.369449 napari-spatialdata-0.2.4/src/napari_spatialdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/src/napari_spatialdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/src/napari_spatialdata/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/src/napari_spatialdata/_categoricals_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:43.373450 napari-spatialdata-0.2.4/src/napari_spatialdata/_constants/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/src/napari_spatialdata/_constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/src/napari_spatialdata/_constants/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/src/napari_spatialdata/_constants/_pkg_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/src/napari_spatialdata/_constants/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8506 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/src/napari_spatialdata/_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/src/napari_spatialdata/_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/src/napari_spatialdata/_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11817 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/src/napari_spatialdata/_scatterwidgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/src/napari_spatialdata/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-23 16:22:43.000000 napari-spatialdata-0.2.4/src/napari_spatialdata/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12679 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/src/napari_spatialdata/_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18152 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/src/napari_spatialdata/_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/src/napari_spatialdata/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:43.373450 napari-spatialdata-0.2.4/src/napari_spatialdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-05-23 16:22:43.000000 napari-spatialdata-0.2.4/src/napari_spatialdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-23 16:22:43.000000 napari-spatialdata-0.2.4/src/napari_spatialdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 16:22:43.000000 napari-spatialdata-0.2.4/src/napari_spatialdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-23 16:22:43.000000 napari-spatialdata-0.2.4/src/napari_spatialdata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-23 16:22:43.000000 napari-spatialdata-0.2.4/src/napari_spatialdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-23 16:22:43.000000 napari-spatialdata-0.2.4/src/napari_spatialdata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:43.373450 napari-spatialdata-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/tests/test_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/tests/test_scatterwidgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/tests/test_spatialdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/tox.ini
```

### Comparing `napari-spatialdata-0.2.3/.github/workflows/test_and_deploy.yml` & `napari-spatialdata-0.2.4/.github/workflows/test_and_deploy.yml`

 * *Files 8% similar despite different names*

```diff
@@ -50,15 +50,15 @@
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install setuptools tox tox-gh-actions
 
       # this runs the platform-specific tests declared in tox.ini
       - name: Test with tox
-        uses: GabrielBB/xvfb-action@v1
+        uses: coactions/setup-xvfb@v1
         with:
           run: python -m tox
         env:
           PLATFORM: ${{ matrix.platform }}
 
       - name: Coverage
         uses: codecov/codecov-action@v3
```

### Comparing `napari-spatialdata-0.2.3/.gitignore` & `napari-spatialdata-0.2.4/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+data/
+
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
```

### Comparing `napari-spatialdata-0.2.3/.mypy.ini` & `napari-spatialdata-0.2.4/.mypy.ini`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.3/.napari/DESCRIPTION.md` & `napari-spatialdata-0.2.4/.napari/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.3/.pre-commit-config.yaml` & `napari-spatialdata-0.2.4/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   python: python3
 default_stages:
   - commit
   - push
 minimum_pre_commit_version: 2.9.3
 repos:
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.2.0
+    rev: v1.3.0
     hooks:
       - id: mypy
         additional_dependencies: [numpy>=1.23]
         exclude: docs
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
@@ -45,11 +45,11 @@
       - id: check-toml
       - id: requirements-txt-fixer
   - repo: https://github.com/asottile/blacken-docs
     rev: 1.13.0
     hooks:
       - id: blacken-docs
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.263
+    rev: v0.0.269
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
```

### Comparing `napari-spatialdata-0.2.3/LICENSE` & `napari-spatialdata-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.3/PKG-INFO` & `napari-spatialdata-0.2.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-spatialdata
-Version: 0.2.3
+Version: 0.2.4
 Summary: Interactive visualization of spatial omics data with napari
 Home-page: https://github.com/scverse/napari-spatialdata.git
 Author: giovanni palla
 Author-email: giov.pll@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/scverse/napari-spatialdata/issues
 Project-URL: Documentation, https://github.com/scverse/napari-spatialdata#README.md
@@ -20,39 +20,30 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: doc
+Provides-Extra: all
 License-File: LICENSE
 
-# napari-spatialdata
+![SpatialData banner](https://github.com/scverse/spatialdata/blob/main/docs/_static/img/spatialdata_horizontal.png?raw=true)
+
+# napari-spatialdata: interactive exploration and annotation of spatial omics data
 
 [![License](https://img.shields.io/pypi/l/napari-spatialdata.svg?color=green)](https://github.com/scverse/napari-spatialdata/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-spatialdata.svg?color=green)](https://pypi.org/project/napari-spatialdata)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-spatialdata.svg?color=green)](https://python.org)
 [![tests](https://github.com/scverse/napari-spatialdata/workflows/tests/badge.svg)](https://github.com/scverse/napari-spatialdata/actions)
 [![codecov](https://codecov.io/gh/scverse/napari-spatialdata/branch/main/graph/badge.svg?token=ASqlOKnOj7)](https://codecov.io/gh/scverse/napari-spatialdata)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/scverse/napari-spatialdata/main.svg)](https://results.pre-commit.ci/latest/github/scverse/napari-spatialdata/main)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-spatialdata)](https://napari-hub.org/plugins/napari-spatialdata)
 
-Interactive visualization of spatial omics data with napari
-
----
-
-This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
-
-<!--
-Don't miss the full getting started guide to set up your new package:
-https://github.com/napari/cookiecutter-napari-plugin#getting-started
-
-and review the napari docs for plugin developers:
-https://napari.org/plugins/stable/index.html
--->
+This repository contains a napari plugin for interactively exploring and annotating SpatialData objects. `napari-spatialdata` is part of the `SpatialData` ecosystem. To learn more about SpatialData, please see the [documentation](https://spatialdata.scverse.org/).
 
 ## Installation
 
 You can install `napari-spatialdata` via [pip]:
 
     pip install napari-spatialdata
 
@@ -64,14 +55,21 @@
 
 Or, you can also install in editable mode after cloning the repo by:
 
     git clone https://github.com/scverse/napari-spatialdata
     cd napari-spatialdata
     pip install -e .
 
+## Getting started
+
+To learn how to use the `napari-spatialdata` plugin, please see the [documentation](https://spatialdata.scverse.org/projects/napari/en/latest/notebooks/spatialdata.html). To learn how to integrate napari-spatialdata into your analysis workflows, please see the [SpatialData tutorials](https://spatialdata.scverse.org/en/latest/tutorials/notebooks/notebooks.html). In particular:
+
+- [Annotating regions of interest with napari](https://spatialdata.scverse.org/en/latest/tutorials/notebooks/notebooks/examples/napari_rois.html)
+- [Use landmark annotations to align multiple -omics layers](https://spatialdata.scverse.org/en/latest/tutorials/notebooks/notebooks/examples/alignment_using_landmarks.html)
+
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
```

### Comparing `napari-spatialdata-0.2.3/README.md` & `napari-spatialdata-0.2.4/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,20 @@
-# napari-spatialdata
+![SpatialData banner](https://github.com/scverse/spatialdata/blob/main/docs/_static/img/spatialdata_horizontal.png?raw=true)
+
+# napari-spatialdata: interactive exploration and annotation of spatial omics data
 
 [![License](https://img.shields.io/pypi/l/napari-spatialdata.svg?color=green)](https://github.com/scverse/napari-spatialdata/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-spatialdata.svg?color=green)](https://pypi.org/project/napari-spatialdata)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-spatialdata.svg?color=green)](https://python.org)
 [![tests](https://github.com/scverse/napari-spatialdata/workflows/tests/badge.svg)](https://github.com/scverse/napari-spatialdata/actions)
 [![codecov](https://codecov.io/gh/scverse/napari-spatialdata/branch/main/graph/badge.svg?token=ASqlOKnOj7)](https://codecov.io/gh/scverse/napari-spatialdata)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/scverse/napari-spatialdata/main.svg)](https://results.pre-commit.ci/latest/github/scverse/napari-spatialdata/main)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-spatialdata)](https://napari-hub.org/plugins/napari-spatialdata)
 
-Interactive visualization of spatial omics data with napari
-
----
-
-This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
-
-<!--
-Don't miss the full getting started guide to set up your new package:
-https://github.com/napari/cookiecutter-napari-plugin#getting-started
-
-and review the napari docs for plugin developers:
-https://napari.org/plugins/stable/index.html
--->
+This repository contains a napari plugin for interactively exploring and annotating SpatialData objects. `napari-spatialdata` is part of the `SpatialData` ecosystem. To learn more about SpatialData, please see the [documentation](https://spatialdata.scverse.org/).
 
 ## Installation
 
 You can install `napari-spatialdata` via [pip]:
 
     pip install napari-spatialdata
 
@@ -36,14 +26,21 @@
 
 Or, you can also install in editable mode after cloning the repo by:
 
     git clone https://github.com/scverse/napari-spatialdata
     cd napari-spatialdata
     pip install -e .
 
+## Getting started
+
+To learn how to use the `napari-spatialdata` plugin, please see the [documentation](https://spatialdata.scverse.org/projects/napari/en/latest/notebooks/spatialdata.html). To learn how to integrate napari-spatialdata into your analysis workflows, please see the [SpatialData tutorials](https://spatialdata.scverse.org/en/latest/tutorials/notebooks/notebooks.html). In particular:
+
+- [Annotating regions of interest with napari](https://spatialdata.scverse.org/en/latest/tutorials/notebooks/notebooks/examples/napari_rois.html)
+- [Use landmark annotations to align multiple -omics layers](https://spatialdata.scverse.org/en/latest/tutorials/notebooks/notebooks/examples/alignment_using_landmarks.html)
+
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
```

### Comparing `napari-spatialdata-0.2.3/docs/Makefile` & `napari-spatialdata-0.2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.3/docs/_templates/autosummary/class.rst` & `napari-spatialdata-0.2.4/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.3/docs/conf.py` & `napari-spatialdata-0.2.4/docs/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     "sphinx.ext.intersphinx",
     "sphinx.ext.autosummary",
     "sphinx.ext.napoleon",
     "sphinxcontrib.bibtex",
     "sphinx.ext.mathjax",
     "sphinx_autodoc_typehints",
     "sphinx_qt_documentation",
+    "scanpydoc",
     "IPython.sphinxext.ipython_console_highlighting",
     *[p.stem for p in (HERE / "extensions").glob("*.py")],
 ]
 
 autosummary_generate = True
 autodoc_member_order = "groupwise"
 autodoc_show_inheritance = False
@@ -86,14 +87,18 @@
     ".ipynb": "myst-nb",
     ".myst": "myst-nb",
 }
 
 intersphinx_mapping = {
     "anndata": ("https://anndata.readthedocs.io/en/stable/", None),
     "numpy": ("https://numpy.org/doc/stable/", None),
+    "geopandas": ("https://geopandas.org/en/stable/", None),
+    "xarray": ("https://docs.xarray.dev/en/stable/", None),
+    "datatree": ("https://datatree.readthedocs.io/en/latest/", None),
+    "dask": ("https://docs.dask.org/en/latest/", None),
     "napari": ("https://napari.org/stable/", None),
     "spatialdata": ("https://scverse-spatialdata.readthedocs.io/en/latest/", None),
 }
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
@@ -113,29 +118,35 @@
     "repository_url": repository_url,
     "use_repository_button": True,
 }
 
 pygments_style = "default"
 
 nitpick_ignore = [
-    # ("py:class", "destroyed"),
+    ("py:data", "typing.Any"),
+    ("py:data", "typing.Union"),
+    ("py:class", "NDArrayA"),
     # ("py:class", "self"),
     # ("py:obj", "napari_spatialdata.QtAdataScatterWidget.setTabOrder"),
     # ("py:obj", "napari_spatialdata.QtAdataViewWidget.insertAction"),
     # ("py:obj", "napari_spatialdata.QtAdataViewWidget.scroll"),
     # ("py:obj", "napari_spatialdata.QtAdataViewWidget.setTabOrder"),
     # ("py:class", "napari_spatialdata._model.ImageModel"),
     # ("py:obj", "napari_spatialdata.QtAdataScatterWidget.scroll"),
     # ("py:obj", "napari_spatialdata.QtAdataScatterWidget.insertAction"),
     # If building the documentation fails because of a missing link that is outside your control,
     # you can add an exception to this list.
     # ("py:class", "igraph.Graph"),
 ]
 
-qt_documentation = "PyQt5"
+qt_documentation = "PyQt6"
+
+suppress_warnings = [
+    "myst.header",  # https://github.com/executablebooks/MyST-Parser/issues/262
+]
 
 
 def setup(app):
     """App setup hook."""
     app.add_config_value(
         "recommonmark_config",
         {
```

### Comparing `napari-spatialdata-0.2.3/docs/contributing.md` & `napari-spatialdata-0.2.4/docs/contributing.md`

 * *Files 4% similar despite different names*

```diff
@@ -167,14 +167,20 @@
 
 ```bash
 cd docs
 make html
 open _build/html/index.html
 ```
 
+or use [sphinx-autobuild](https://sphinx-extensions.readthedocs.io/en/latest/sphinx-autobuild.html)
+
+```bash
+sphinx-autobuild docs docs/_build/html
+```
+
 <!-- Links -->
 
 [scanpy developer guide]: https://scanpy.readthedocs.io/en/latest/dev/index.html
 [cookiecutter-scverse-instance]: https://cookiecutter-scverse-instance.readthedocs.io/en/latest/template_usage.html
 [github quickstart guide]: https://docs.github.com/en/get-started/quickstart/create-a-repo?tool=webui
 [codecov]: https://about.codecov.io/sign-up/
 [codecov docs]: https://docs.codecov.com/docs
```

### Comparing `napari-spatialdata-0.2.3/docs/extensions/typed_returns.py` & `napari-spatialdata-0.2.4/docs/extensions/typed_returns.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.3/docs/make.bat` & `napari-spatialdata-0.2.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.3/docs/notebooks/mibitof_analysis.ipynb` & `napari-spatialdata-0.2.4/docs/notebooks/mibitof_analysis.ipynb`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.3/docs/notebooks/nanostring_analysis.ipynb` & `napari-spatialdata-0.2.4/docs/notebooks/nanostring_analysis.ipynb`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.3/docs/notebooks/spatialdata.ipynb` & `napari-spatialdata-0.2.4/docs/notebooks/spatialdata.ipynb`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.3/docs/references.bib` & `napari-spatialdata-0.2.4/docs/references.bib`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.3/docs/template_usage.md` & `napari-spatialdata-0.2.4/docs/template_usage.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+---
+orphan: true
+---
+
 # Using this template
 
 Welcome to the developer guidelines! This document is split into two parts:
 
 1.  The [repository setup](#setting-up-the-repository). This section is relevant primarily for the repository maintainer and shows how to connect
     continuous integration services and documents initial set-up of the repository.
 2.  The [contributor guide](contributing.md#contributing-guide). It contains information relevant to all developers who want to make a contribution.
```

### Comparing `napari-spatialdata-0.2.3/pyproject.toml` & `napari-spatialdata-0.2.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -84,10 +84,7 @@
     "src/napari_spatialdata/_constants/_pkg_constants.py" = ["D101","D102", "D106", "B024"]
     "src/napari_spatialdata/_constants/_constants.py" = ["D101","D102", "B024"]
     "src/napari_spatialdata/_constants/_utils.py" = ["D101","D102", "B024"]
     "src/napari_spatialdata/_widgets.py" = ["D"]
     "src/napari_spatialdata/_scatterwidgets.py" = ["D"]
 [tool.ruff.pydocstyle]
 convention = "numpy"
-[tool.ruff.pyupgrade]
-# Preserve types, even if a file imports `from __future__ import annotations`.
-keep-runtime-typing = true
```

### Comparing `napari-spatialdata-0.2.3/setup.cfg` & `napari-spatialdata-0.2.4/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -32,16 +32,17 @@
 install_requires = 
 	numpy
 	magicgui
 	qtpy
 	numba
 	anndata
 	scikit-image
-	napari[all]
+	napari
 	loguru
+	typing_extensions<=4.5
 	napari-matplotlib
 	scikit-learn
 	spatialdata
 package_dir = 
 	=src
 
 [options.extras_require]
@@ -49,37 +50,44 @@
 	tox
 	pytest  # https://docs.pytest.org/en/latest/contents.html
 	pytest-cov  # https://pytest-cov.readthedocs.io/en/latest/
 	pytest-qt  # https://pytest-qt.readthedocs.io/en/latest/
 	pre-commit>=2.9.0
 	towncrier>=21.3.0
 doc = 
-	sphinx>=4
-	sphinx-book-theme>=0.3.3
-	myst-nb
+	sphinx>=4.5
+	sphinx-book-theme>=1.0.0
+	myst-parser
 	sphinxcontrib-bibtex>=1.0.0
-	sphinx-autodoc-typehints
+	sphinx-autodoc-typehints>=1.11.0
+	sphinx-autobuild
+	scanpydoc
 	ipykernel
 	ipython
 	sphinx-copybutton
 	sphinx-qt-documentation
+	myst-nb
+all = 
+	PyQt6
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 napari_spatiadata = napari.yaml
 
 [options.entry_points]
 napari.manifest = 
 	napari-spatialdata = napari_spatialdata:napari.yaml
+console_scripts = 
+	spatialdata = napari_spatialdata.__main__:main
 
 [tool:pytest]
 python_files = test_*.py
 testpaths = tests/
 xfail_strict = true
-qt_api = pyqt5
+qt_api = pyqt6
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `napari-spatialdata-0.2.3/src/napari_spatialdata/__init__.py` & `napari-spatialdata-0.2.4/src/napari_spatialdata/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-__version__ = "0.1.0"
-
 from importlib.metadata import version  # Python = 3.9
 
+__version__ = version("napari-spatialdata")
+
 from packaging.version import parse
 
 try:
     __full_version__ = parse(version(__name__))
     __full_version__ = f"{__version__}+{__full_version__.local}" if __full_version__.local else __version__
 except ImportError:
     __full_version__ = __version__
 
 del version, parse
 
 from napari_spatialdata._interactive import Interactive as Interactive  # noqa: E402
+from napari_spatialdata._reader import get_reader  # noqa: E402
 from napari_spatialdata._view import (  # noqa: E402
     QtAdataScatterWidget,
     QtAdataViewWidget,
 )
```

### Comparing `napari-spatialdata-0.2.3/src/napari_spatialdata/_categoricals_utils.py` & `napari-spatialdata-0.2.4/src/napari_spatialdata/_categoricals_utils.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.3/src/napari_spatialdata/_constants/_pkg_constants.py` & `napari-spatialdata-0.2.4/src/napari_spatialdata/_constants/_pkg_constants.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.3/src/napari_spatialdata/_constants/_utils.py` & `napari-spatialdata-0.2.4/src/napari_spatialdata/_constants/_utils.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.3/src/napari_spatialdata/_interactive.py` & `napari-spatialdata-0.2.4/src/napari_spatialdata/_interactive.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import Any, Iterable, Union
+from __future__ import annotations
+
+from typing import Any, Iterable
 
 import napari
 import numpy as np
 import shapely
 from anndata import AnnData
 from loguru import logger
 from multiscale_spatial_image import MultiscaleSpatialImage
@@ -14,15 +16,15 @@
 
 
 class ElementWidget(QListWidget):
     def __init__(self, sdata: SpatialData):
         super().__init__()
         self._sdata = sdata
 
-    def _onClickChange(self, selected_coordinate_system: Union[QListWidgetItem, int, Iterable[str]]) -> None:
+    def _onClickChange(self, selected_coordinate_system: QListWidgetItem | int | Iterable[str]) -> None:
         self.clear()
 
         elements = {}
         for element_type, element_name, _ in self._sdata.filter_by_coordinate_system(
             selected_coordinate_system
         )._gen_elements():
             elements[element_name] = element_type
@@ -35,15 +37,15 @@
     def __init__(self, sdata: SpatialData):
         super().__init__()
 
         self._sdata = sdata
 
         self.addItems(self._sdata.coordinate_systems)
 
-    def _select_coord_sys(self, selected_coordinate_system: Union[QListWidgetItem, int, Iterable[str]]) -> None:
+    def _select_coord_sys(self, selected_coordinate_system: QListWidgetItem | int | Iterable[str]) -> None:
         self._system = str(selected_coordinate_system)
 
 
 class SdataWidget(QWidget):
     def __init__(self, viewer: Viewer, sdata: SpatialData):
         super().__init__()
         self._sdata = sdata
@@ -91,47 +93,67 @@
             affine=affine,
             shape_type="ellipse",
             metadata={
                 "adata": self._sdata.table[
                     self._sdata.table.obs[self._sdata.table.uns["spatialdata_attrs"]["region_key"]] == key
                 ],
                 "shapes_key": self._sdata.table.uns["spatialdata_attrs"]["region_key"],
+                "shapes_type": "circles",
             },
         )
 
     def _add_polygons(self, key: str) -> None:
         polygons = []
         df = self._sdata.shapes[key]
         affine = _get_transform(self._sdata.shapes[key], self.coordinate_system_widget._system)
 
-        for i in range(0, len(df)):
-            polygons.append(list(df.geometry[i].exterior.coords))
-
+        # when mulitpolygons are present, we select the largest ones
+        if "MultiPolygon" in np.unique(df.geometry.type):
+            logger.info("Multipolygons are present in the data. Only the largest polygon per cell is retained.")
+            df = df.explode(index_parts=False)
+            df["area"] = df.area
+            df = df.sort_values(by="area", ascending=False)  # sort by area
+            df = df[~df.index.duplicated(keep="first")]  # only keep the largest area
+            df = df.sort_index()  # reset the index to the first order
+        if len(df) < 100:
+            for i in range(0, len(df)):
+                polygons.append(list(df.geometry.iloc[i].exterior.coords))
+        else:
+            for i in range(
+                0, len(df)
+            ):  # This can be removed once napari is sped up in the plotting. It changes the shapes only very slightly
+                polygons.append(list(df.geometry.iloc[i].exterior.simplify(tolerance=2).coords))
+        # this will only work for polygons and not for multipolygons
         polygons = _swap_coordinates(polygons)
 
         self._viewer.add_shapes(
             polygons,
             name=key,
             affine=affine,
             shape_type="polygon",
             metadata={
                 "adata": self._sdata.table[
                     self._sdata.table.obs[self._sdata.table.uns["spatialdata_attrs"]["region_key"]] == key
                 ],
                 "shapes_key": self._sdata.table.uns["spatialdata_attrs"]["region_key"],
+                "shapes_type": "polygons",
             },
         )
 
     def _add_shapes(self, key: str) -> None:
         if type(self._sdata.shapes[key].iloc[0][0]) == shapely.geometry.point.Point:
             self._add_circles(key)
-        elif type(self._sdata.shapes[key].iloc[0][0]) == shapely.geometry.polygon.Polygon:
+        elif (type(self._sdata.shapes[key].iloc[0][0]) == shapely.geometry.polygon.Polygon) or (
+            type(self._sdata.shapes[key].iloc[0][0]) == shapely.geometry.multipolygon.MultiPolygon
+        ):
             self._add_polygons(key)
         else:
-            raise TypeError("Incorrect data type passed for shapes (should be Shapely Point or Polygon).")
+            raise TypeError(
+                "Incorrect data type passed for shapes (should be Shapely Point or Polygon or MultiPolygon)."
+            )
 
     def _add_label(self, key: str) -> None:
         affine = _get_transform(self._sdata.labels[key], self.coordinate_system_widget._system)
 
         self._viewer.add_labels(
             self._sdata.labels[key],
             name=key,
@@ -151,46 +173,57 @@
         if isinstance(img, MultiscaleSpatialImage):
             img = img["scale0"][key]
         # TODO: type check
         self._viewer.add_image(
             img,
             name=key,
             affine=affine,
-            metadata={
-                "adata": AnnData(),
-            },
         )
 
     def _add_points(self, key: str) -> None:
         points = self._sdata.points[key].compute()
         affine = _get_transform(self._sdata.points[key], self.coordinate_system_widget._system)
         if len(points) < 100000:
             subsample = np.arange(len(points))
         else:
             logger.info("Subsampling points because the number of points exceeds the currently supported 100 000.")
             gen = np.random.default_rng()
             subsample = gen.choice(len(points), size=100000, replace=False)
+
         self._viewer.add_points(
             points[["y", "x"]].values[subsample],
             name=key,
             size=20,
             affine=affine,
             metadata={
                 "adata": AnnData(obs=points.loc[subsample, :], obsm={"spatial": points[["x", "y"]].values[subsample]}),
             },
         )
 
 
 class Interactive:
+    """
+    Interactive visualization of spatial data.
+
+    Parameters
+    ----------
+    sdata
+        SpatialData object.
+
+    Returns
+    -------
+    None
+    """
+
     def __init__(self, sdata: SpatialData):
         self._viewer = napari.Viewer()
         self._sdata = sdata
         self._sdata_widget = SdataWidget(self._viewer, sdata)
         self._list_widget = self._viewer.window.add_dock_widget(
             self._sdata_widget, name="SpatialData", area="left", menu=self._viewer.window.window_menu
         )
 
     def run(self) -> None:
         napari.run()
 
-    def screenshot(self) -> Union[NDArrayA, Any]:
+    def screenshot(self) -> NDArrayA | Any:
         return self._viewer.screenshot(canvas_only=False)
```

### Comparing `napari-spatialdata-0.2.3/src/napari_spatialdata/_model.py` & `napari-spatialdata-0.2.4/src/napari_spatialdata/_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,22 +16,23 @@
 
 @dataclass
 class ImageModel:
     """Model which holds the data for interactive visualization."""
 
     events: EmitterGroup = field(init=False, default=None, repr=True)
     _layer: Layer = field(init=False, default=None, repr=True)
-    _adata: AnnData = field(init=False, default=None, repr=True)
+    _adata: Optional[AnnData] = field(init=False, default=None, repr=True)
     _spatial_key: str = field(default=Key.obsm.spatial, repr=False)
     _adata_layer: Optional[str] = field(init=False, default=None, repr=False)
     _label_key: Optional[str] = field(default=None, repr=True)
     _coordinates: Optional[NDArrayA] = field(init=False, default=None, repr=True)
     _points_coordinates: Optional[NDArrayA] = field(init=False, default=None, repr=True)
     _points_var: Optional[pd.Series] = field(init=False, default=None, repr=True)
     _scale: Optional[float] = field(init=False, default=None)
+    _system_name: Optional[str] = field(default=None, repr=True)
 
     _spot_diameter: Union[NDArrayA, float] = field(init=False, default=1)
     _point_diameter: Union[NDArrayA, float] = field(init=False, default=1)
     _scale_key: Optional[str] = field(init=False, default="tissue_hires_scalef")  # TODO(giovp): use constants for these
 
     _palette: Optional[str] = field(init=False, default=None, repr=False)
     _cmap: str = field(init=False, default="viridis", repr=False)
@@ -298,7 +299,15 @@
     @property
     def scale_key(self) -> Optional[str]:  # noqa: D102
         return self._scale_key
 
     @scale_key.setter
     def scale_key(self, scale_key: str) -> None:
         self._scale_key = scale_key
+
+    @property
+    def system_name(self) -> Optional[str]:  # noqa: D102
+        return self._system_name
+
+    @system_name.setter
+    def system_name(self, system_name: str) -> None:
+        self._system_name = system_name
```

### Comparing `napari-spatialdata-0.2.3/src/napari_spatialdata/_scatterwidgets.py` & `napari-spatialdata-0.2.4/src/napari_spatialdata/_scatterwidgets.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Dict, Iterable, List, Optional, Union
+from typing import TYPE_CHECKING, Any, Iterable
 
 import matplotlib as plt
-import napari
 import numpy as np
 import pandas as pd
 from anndata import AnnData
 from loguru import logger
 from matplotlib.axes import Axes
 from matplotlib.collections import Collection
 from matplotlib.path import Path
@@ -54,22 +53,20 @@
     alpha_other
         To highlight a selection, this tool sets all selected points to an
         alpha value of 1 and non-selected points to *alpha_other*.
     """
 
     def __init__(
         self,
-        viewer: Viewer,
         model: ImageModel,
         ax: Axes,
         collection: Collection,
-        data: List[NDArrayA],
+        data: list[NDArrayA],
         alpha_other: float = 0.3,
     ):
-        self.viewer = viewer
         self.model = model
         self.canvas = ax.figure.canvas
         self.collection = collection
         self.alpha_other = alpha_other
         self.exported_data = None
         self.data = data
         self.axes = ax
@@ -83,24 +80,24 @@
         if len(self.fc) == 0:
             raise ValueError("Collection must have a facecolor")
         elif len(self.fc) == 1:  # noqa: RET506
             self.fc = np.tile(self.fc, (self.Npts, 1))
 
         self.selector = LassoSelector(ax, onselect=self.onselect)
 
-        self.ind: Optional[NDArrayA] = None
+        self.ind: NDArrayA | None = None
 
     def export(self, adata: AnnData) -> None:
         model_layer: Layer = self.model.layer
         obs_name = model_layer.name + "_LASSO_SELECTED"
 
         adata.obs[obs_name] = self.exported_data
         logger.info("Exported selected coordinates to obs in AnnData as: {}", obs_name)  # noqa: P103
 
-    def onselect(self, verts: List[NDArrayA]) -> None:
+    def onselect(self, verts: list[NDArrayA]) -> None:
         self.path = Path(verts)
         self.ind = np.nonzero(self.path.contains_points(self.xys))[0]
 
         self.fc[:, -1] = self.alpha_other  # Set alpha of unselected coordinates
         self.fc[self.ind, -1] = 1  # Set alpha of selected coordinates
 
         self.collection.set_facecolors(self.fc)
@@ -112,19 +109,19 @@
 
 
 class ScatterListWidget(AListWidget):
     attrChanged = Signal()
     _text = None
     _chosen = None
 
-    def __init__(self, viewer: Viewer, model: ImageModel, attr: str, color: bool, **kwargs: Any):
-        AListWidget.__init__(self, viewer, model, attr, **kwargs)
+    def __init__(self, model: ImageModel, attr: str, color: bool, **kwargs: Any):
+        AListWidget.__init__(self, None, model, attr, **kwargs)
         self.attrChanged.connect(self._onChange)
         self._color = color
-        self._data: Optional[Union[NDArrayA, Dict[str, Any]]] = None
+        self._data: NDArrayA | dict[str, Any] | None = None
         self.itemClicked.connect(lambda item: self._onOneClick((item.text(),)))
 
     def _onChange(self) -> None:
         AListWidget._onChange(self)
         self.data = None
         self.text = None
         self.chosen = None
@@ -156,83 +153,91 @@
 
     def _onOneClick(self, items: Iterable[str]) -> None:
         if self.getAttribute() == "obsm":
             return
         self._onAction(items)
         return
 
-    def setAttribute(self, field: Optional[str]) -> None:
+    def setAttribute(self, field: str | None) -> None:
         if field == self.getAttribute():
             return
         if field not in ("var", "obs", "obsm"):
             raise ValueError(f"{field} is not a valid adata field.")
         self._attr = field
         self._getter = getattr(self.model, f"get_{field}")
         self.attrChanged.emit()
 
-    def getAttribute(self) -> Optional[str]:
+    def getAttribute(self) -> str | None:
         if TYPE_CHECKING:
             assert isinstance(self._attr, str)
         return self._attr
 
-    def setComponent(self, text: Optional[Union[int, str]]) -> None:
+    def setComponent(self, text: int | str | None) -> None:
         if self.getAttribute() == "var":
             if TYPE_CHECKING:
                 assert isinstance(text, str)
             self.text = text
             super().setAdataLayer(text)
         elif self.getAttribute() == "obsm":
             if TYPE_CHECKING:
                 assert isinstance(text, (int, str))
             self.text = text  # type: ignore[assignment]
             super().setIndex(text)
 
     @property
-    def text(self) -> Optional[str]:
+    def text(self) -> str | None:
         return self._text
 
     @text.setter
-    def text(self, text: Optional[Union[str, int]]) -> None:
+    def text(self, text: str | int | None) -> None:
         self._text = text if text is not None else None
 
     @property
-    def chosen(self) -> Optional[str]:
+    def chosen(self) -> str | None:
         return self._chosen
 
     @chosen.setter
-    def chosen(self, chosen: Optional[str]) -> None:
+    def chosen(self, chosen: str | None) -> None:
         self._chosen = chosen if chosen is not None else None
 
     @property
-    def data(self) -> Optional[Union[NDArrayA, Dict[str, Any]]]:
+    def data(self) -> NDArrayA | dict[str, Any] | None:
         return self._data
 
     @data.setter
-    def data(self, data: Union[NDArrayA, Dict[str, Any]]) -> None:
+    def data(self, data: NDArrayA | dict[str, Any]) -> None:
         self._data = data
 
 
 class MatplotlibWidget(NapariMPLWidget):
-    def __init__(self, viewer: Viewer, model: ImageModel):
+    def __init__(self, viewer: Viewer | None, model: ImageModel):
+        self.is_widget = False
+        if viewer is None:
+            viewer = Viewer()
+            self.is_widget = True
+
         super().__init__(viewer)
 
         self._viewer = viewer
         self._model = model
         self.axes = self.canvas.figure.subplots()
         self.colorbar = None
         self.selector = None
 
+        if self.is_widget:
+            self._viewer.close()
+
     def _onClick(
         self,
-        x_data: Union[NDArrayA, pd.Series],
-        y_data: Union[NDArrayA, pd.Series],
-        color_data: Union[NDArrayA, dict[str, Union[NDArrayA, pd.Series, dict[str, str]]]],
-        x_label: Optional[str],
-        y_label: Optional[str],
-        color_label: Optional[str],
+        x_data: NDArrayA | pd.Series,
+        y_data: NDArrayA | pd.Series,
+        color_data: NDArrayA | dict[str, NDArrayA | pd.Series | dict[str, str]],
+        x_label: str | None,
+        y_label: str | None,
+        color_label: str | None,
     ) -> None:
         self.cat = None
         self.palette = None
 
         if isinstance(color_data, dict):
             self.data = [x_data, y_data, color_data["vec"]]
             self.cat = color_data["cat"]
@@ -270,30 +275,29 @@
             if self.colorbar is None:
                 raise ValueError("Colorbar hasn't been created.")
             self.colorbar.set_label(self.color_label)
 
         self.canvas.draw()
 
         self.selector = SelectFromCollection(
-            self._viewer, self._model, self.axes, self.scatterplot, self.data
+            self._model, self.axes, self.scatterplot, self.data
         )  # type:ignore[assignment]
 
     def clear(self) -> None:
         if self.colorbar:
             self.colorbar.remove()
             self.colorbar = None
 
         self.axes.clear()
 
 
 class AxisWidgets(QtWidgets.QWidget):
-    def __init__(self, viewer: Viewer, model: ImageModel, name: str, color: bool = False):
+    def __init__(self, model: ImageModel, name: str, color: bool = False):
         super().__init__()
 
-        self._viewer = viewer
         self._model = model
 
         selection_label = QtWidgets.QLabel(f"{name} type:")
         selection_label.setToolTip("Select between obs, obsm and var.")
         self.selection_widget = QtWidgets.QComboBox()
         self.selection_widget.addItem("obsm", None)
         self.selection_widget.addItem("obs", None)
@@ -302,15 +306,15 @@
         self.setLayout(QtWidgets.QVBoxLayout())
         self.layout().addWidget(selection_label)
         self.layout().addWidget(self.selection_widget)
 
         label = QtWidgets.QLabel(f"Select for {name}:")
         label.setToolTip(f"Select {name}.")
 
-        self.widget = ScatterListWidget(self.viewer, self.model, attr="obsm", color=color)
+        self.widget = ScatterListWidget(self.model, attr="obsm", color=color)
         self.widget.setAttribute("obsm")
 
         self.component_widget = ComponentWidget(self.model, attr="obsm")
         self.component_widget.setToolTip("obsm")
         self.component_widget.currentTextChanged.connect(self.widget.setComponent)
         self.widget.itemClicked.connect(self.component_widget._onClickChange)
 
@@ -318,31 +322,30 @@
         self.layout().addWidget(self.widget)
         self.layout().addWidget(self.component_widget)
 
         self.selection_widget.currentTextChanged.connect(self.widget.setAttribute)
         self.selection_widget.currentTextChanged.connect(self.component_widget.setAttribute)
         self.selection_widget.currentTextChanged.connect(self.component_widget.setToolTip)
 
-    def getFormattedLabel(self) -> Optional[str]:
+    def getFormattedLabel(self) -> str | None:
         return (
             str(self.widget.getAttribute()) + ": " + str(self.widget.chosen)
             if self.widget.text is None
             else (
                 str(self.widget.getAttribute()) + ": " + str(self.widget.chosen) + "[" + str(self.widget.text) + "]"
                 if self.widget.getAttribute() == "obsm"
                 else str(self.widget.getAttribute())
                 + ": "
                 + str(self.widget.chosen)
                 + " on layer "
                 + str(self.widget.text)
             )
         )
 
-    @property
-    def viewer(self) -> napari.Viewer:
-        """:mod:`napari` viewer."""
-        return self._viewer
+    def clear(self) -> None:
+        self.widget.clear()
+        self.component_widget.clear()
 
     @property
     def model(self) -> ImageModel:
         """:mod:`napari` viewer."""
         return self._model
```

### Comparing `napari-spatialdata-0.2.3/src/napari_spatialdata/_utils.py` & `napari-spatialdata-0.2.4/src/napari_spatialdata/_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from functools import wraps
-from typing import TYPE_CHECKING, Any, Callable, List, Optional, Sequence, Tuple, Union
+from typing import TYPE_CHECKING, Any, Callable, Optional, Sequence, Union
 
 import numpy as np
 import pandas as pd
 from anndata import AnnData
 from dask.dataframe.core import DataFrame as DaskDataFrame
 from geopandas import GeoDataFrame
 from loguru import logger
@@ -36,15 +36,15 @@
 
     NDArrayA = NDArray[Any]
 except (ImportError, TypeError):
     NDArray = np.ndarray  # type: ignore[misc]
     NDArrayA = np.ndarray  # type: ignore[misc]
 
 
-Vector_name_t = Tuple[Optional[Union[pd.Series, NDArrayA]], Optional[str]]
+Vector_name_t = tuple[Optional[Union[pd.Series, NDArrayA]], Optional[str]]
 
 
 def _ensure_dense_vector(fn: Callable[..., Vector_name_t]) -> Callable[..., Vector_name_t]:
     @wraps(fn)
     def decorator(self: Any, *args: Any, **kwargs: Any) -> Vector_name_t:
         normalize = kwargs.pop("normalize", False)
         res, fmt = fn(self, *args, **kwargs)
@@ -81,28 +81,28 @@
 
     return decorator
 
 
 def _get_palette(
     adata: AnnData,
     key: str,
-    palette: Optional[str] = None,
-    vec: Optional[pd.Series] = None,
+    palette: str | None = None,
+    vec: pd.Series | None = None,
 ) -> dict[Any, Any]:
     if key not in adata.obs:
         raise KeyError("Missing key!")  # TODO: Improve error message
 
     return dict(zip(adata.obs[key].cat.categories, [to_rgb(i) for i in adata.uns[Key.uns.colors(key)]]))
 
 
 def _set_palette(
     adata: AnnData,
     key: str,
-    palette: Optional[str] = None,
-    vec: Optional[pd.Series] = None,
+    palette: str | None = None,
+    vec: pd.Series | None = None,
 ) -> dict[Any, Any]:
     if vec is not None and not is_categorical_dtype(vec):
         raise TypeError(f"Expected a `categorical` type, found `{infer_dtype(vec)}`.")
 
     add_colors_for_categorical_sample_annotation(
         adata,
         key=key,
@@ -114,17 +114,17 @@
     #
     return dict(zip(vec.cat.categories, [to_rgb(i) for i in adata.uns[Key.uns.colors(key)]]))
 
 
 def _get_categorical(
     adata: AnnData,
     key: str,
-    vec: Optional[pd.Series] = None,
-    palette: Optional[str] = None,
-    colordict: Union[pd.Series, dict[Any, Any], None] = None,
+    vec: pd.Series | None = None,
+    palette: str | None = None,
+    colordict: pd.Series | dict[Any, Any] | None = None,
 ) -> NDArrayA:
     categorical = vec if vec is not None else adata.obs[key]
     if not isinstance(colordict, dict):
         col_dict = _set_palette(adata, key, palette, colordict)
     else:
         col_dict = colordict
         for cat in colordict:
@@ -150,15 +150,15 @@
     kdtree = KDTree(coords)
     clusters = np.full(len(coords), fill_value="", dtype=object)
     # index consists of the categories that need not be string
     clusters[kdtree.query(df.values)[1]] = df.index.astype(str)
     return {"clusters": clusters}
 
 
-def _min_max_norm(vec: Union[spmatrix, NDArrayA]) -> NDArrayA:
+def _min_max_norm(vec: spmatrix | NDArrayA) -> NDArrayA:
     if issparse(vec):
         if TYPE_CHECKING:
             assert isinstance(vec, spmatrix)
         vec = vec.toarray().squeeze()
     vec = np.asarray(vec, dtype=np.float64)
     if vec.ndim != 1:
         raise ValueError(f"Expected `1` dimension, found `{vec.ndim}`.")
@@ -166,19 +166,19 @@
     maxx, minn = np.nanmax(vec), np.nanmin(vec)
 
     return (  # type: ignore[no-any-return]
         np.ones_like(vec) if np.isclose(minn, maxx) else ((vec - minn) / (maxx - minn))
     )
 
 
-def _swap_coordinates(data: List[Any]) -> List[Any]:
+def _swap_coordinates(data: list[Any]) -> list[Any]:
     return [[(y, x) for x, y in sublist] for sublist in data]
 
 
-def _get_transform(element: SpatialElement, coordinate_system_name: Optional[str] = None) -> NDArrayA:
+def _get_transform(element: SpatialElement, coordinate_system_name: str | None = None) -> NDArrayA:
     affine: NDArrayA
     transformations = get_transformation(element, get_all=True)
     cs = transformations.keys().__iter__().__next__() if coordinate_system_name is None else coordinate_system_name
     ct = transformations[cs]
     affine = ct.to_affine_matrix(input_axes=("y", "x"), output_axes=("y", "x"))
 
     if not isinstance(element, (SpatialImage, MultiscaleSpatialImage, AnnData, DaskDataFrame, GeoDataFrame)):
```

### Comparing `napari-spatialdata-0.2.3/src/napari_spatialdata/_view.py` & `napari-spatialdata-0.2.4/src/napari_spatialdata/_view.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from typing import Any, FrozenSet, Optional, Sequence
 
 import napari
 import numpy as np
 import pandas as pd
 from anndata import AnnData
 from loguru import logger
+from napari._qt.qt_resources import get_stylesheet
+from napari._qt.utils import QImg2array
 from napari.layers import Labels
 from napari.viewer import Viewer
+from qtpy.QtCore import QSize, Qt
 from qtpy.QtWidgets import (
     QComboBox,
     QGridLayout,
     QLabel,
     QPushButton,
     QVBoxLayout,
     QWidget,
@@ -33,38 +36,49 @@
 
 __all__ = ["QtAdataViewWidget", "QtAdataScatterWidget"]
 
 
 class QtAdataScatterWidget(QWidget):
     """Adata viewer widget."""
 
-    def __init__(self, viewer: Viewer):
+    def __init__(self, input: Viewer):
         super().__init__()
 
-        self._viewer = viewer
         self._model = ImageModel()
 
-        self._select_layer()
-        self._viewer.layers.selection.events.changed.connect(self._select_layer)
-        self._viewer.layers.selection.events.changed.connect(self._on_selection)
-
         self.setLayout(QGridLayout())
 
+        if isinstance(input, Viewer):
+            self._viewer = input
+            self._select_layer()
+            self._viewer.layers.selection.events.changed.connect(self._select_layer)
+            self._viewer.layers.selection.events.changed.connect(self._on_selection)
+
+        elif isinstance(input, AnnData):
+            self._viewer = None
+            self.model.adata = input
+            self.setStyleSheet(get_stylesheet("dark"))
+            self.quit_button_widget = QPushButton("Close")
+            self.quit_button_widget.clicked.connect(self.close)
+            self.quit_button_widget.setStyleSheet("background-color: red")
+            self.quit_button_widget.setFixedSize(QSize(100, 25))
+            self.layout().addWidget(self.quit_button_widget, 0, 2, 1, 1, Qt.AlignRight)
+
         # Matplotlib
 
         self.matplotlib_widget = MatplotlibWidget(self.viewer, self.model)
         self.layout().addWidget(self.matplotlib_widget, 1, 0, 1, 3)
 
-        self.x_widget = AxisWidgets(self.viewer, self.model, "X-axis")
+        self.x_widget = AxisWidgets(self.model, "X-axis")
         self.layout().addWidget(self.x_widget, 2, 0, 6, 1)
 
-        self.y_widget = AxisWidgets(self.viewer, self.model, "Y-axis")
+        self.y_widget = AxisWidgets(self.model, "Y-axis")
         self.layout().addWidget(self.y_widget, 2, 1, 6, 1)
 
-        self.color_widget = AxisWidgets(self.viewer, self.model, "Color", True)
+        self.color_widget = AxisWidgets(self.model, "Color", True)
         self.layout().addWidget(self.color_widget, 2, 2, 6, 1)
 
         self.plot_button_widget = QPushButton("Plot")
         self.plot_button_widget.clicked.connect(
             lambda: self.matplotlib_widget._onClick(
                 self.x_widget.widget.data,
                 self.y_widget.widget.data,
@@ -101,49 +115,50 @@
         self.y_widget.component_widget._onChange()
         self.color_widget.widget._onChange()
         self.color_widget.component_widget._onChange()
 
     def _select_layer(self) -> None:
         """Napari layers."""
         layer = self._viewer.layers.selection._current
-        if not isinstance(layer.metadata.get("adata", None), AnnData):
-            raise NotImplementedError(":class:`anndata.AnnData` not found in any `layer.metadata`.")
-
         self.model.layer = layer
+        if not hasattr(layer, "metadata") or not isinstance(layer.metadata.get("adata", None), AnnData):
+            if hasattr(self, "x_widget"):
+                self.x_widget.clear()
+                self.y_widget.clear()
+                self.color_widget.clear()
+            return
+
         # if layer is not None and "adata" in layer.metadata:
         self.model.adata = layer.metadata["adata"]
 
+    def screenshot(self) -> Any:
+        return QImg2array(self.grab().toImage())
+
     @property
     def viewer(self) -> napari.Viewer:
         """:mod:`napari` viewer."""
         return self._viewer
 
     @property
     def model(self) -> ImageModel:
         """:mod:`napari` viewer."""
         return self._model
 
-    @property
-    def layernames(self) -> FrozenSet[str]:
-        """Names of :class:`napari.layers.Layer`."""
-        return frozenset(layer.name for layer in self.viewer.layers)
-
 
 class QtAdataViewWidget(QWidget):
     """Adata viewer widget."""
 
     def __init__(self, viewer: Viewer):
         super().__init__()
 
         self._viewer = viewer
         self._model = ImageModel()
 
         self._select_layer()
         self._viewer.layers.selection.events.changed.connect(self._select_layer)
-        self._viewer.layers.selection.events.changed.connect(self._on_layer_update)
 
         self.setLayout(QVBoxLayout())
 
         # obs
         obs_label = QLabel("Observations:")
         obs_label.setToolTip("Keys in `adata.obs` containing cell observations.")
         self.obs_widget = AListWidget(self.viewer, self.model, attr="obs")
@@ -156,16 +171,18 @@
         self.var_widget = AListWidget(self.viewer, self.model, attr="var")
         self.var_widget.setAdataLayer("X")
 
         # layers
         adata_layer_label = QLabel("Layers:")
         adata_layer_label.setToolTip("Keys in `adata.layers` used when visualizing gene expression.")
         self.adata_layer_widget = QComboBox()
-        self.adata_layer_widget.addItem("X", None)
-        self.adata_layer_widget.addItems(self._get_adata_layer())
+        if self.model.adata is not None:
+            self.adata_layer_widget.addItem("X", None)
+            self.adata_layer_widget.addItems(self._get_adata_layer())
+
         self.adata_layer_widget.currentTextChanged.connect(self.var_widget.setAdataLayer)
 
         self.layout().addWidget(self.adata_layer_widget)
         self.layout().addWidget(var_label)
         self.layout().addWidget(self.var_widget)
 
         # obsm
@@ -210,33 +227,53 @@
         self.var_widget._onChange()
         self.obsm_widget._onChange()
         self.var_points_widget._onChange()
 
     def _select_layer(self) -> None:
         """Napari layers."""
         layer = self._viewer.layers.selection._current
-        if not isinstance(layer.metadata.get("adata", None), AnnData):
-            raise NotImplementedError(":class:`anndata.AnnData` not found in any `layer.metadata`.")
-
         self.model.layer = layer
+        if not hasattr(layer, "metadata") or not isinstance(layer.metadata.get("adata", None), AnnData):
+            if hasattr(self, "obs_widget"):
+                self.adata_layer_widget.clear()
+                self.obs_widget.clear()
+                self.var_widget.clear()
+                self.obsm_widget.clear()
+                self.var_points_widget.clear()
+            return
+
         # if layer is not None and "adata" in layer.metadata:
         self.model.adata = layer.metadata["adata"]
 
         if self.model.adata.shape == (0, 0):
             return
 
-        self.model.coordinates = np.insert(self.model.adata.obsm[Key.obsm.spatial][:, ::-1][:, :2], 0, values=0, axis=1)
+        if "spatial" in self.model.adata.obsm:
+            self.model.coordinates = np.insert(
+                self.model.adata.obsm[Key.obsm.spatial][:, ::-1][:, :2], 0, values=0, axis=1
+            )
+
         if "points" in layer.metadata:
+            # TODO: Check if this can be removed
             self.model.points_coordinates = layer.metadata["points"].X
             self.model.points_var = layer.metadata["points"].obs["gene"]
             self.model.point_diameter = np.array([0.0] + [layer.metadata["point_diameter"]] * 2) * self.model.scale
+
         self.model.spot_diameter = np.array([0.0, 10.0, 10.0])
         self.model.labels_key = layer.metadata["labels_key"] if isinstance(layer, Labels) else None
+        self.model.system_name = self.model.layer.name
+
         if "colormap" in layer.metadata:
             self.model.cmap = layer.metadata["colormap"]
+        if hasattr(
+            self, "obs_widget"
+        ):  # to check if the widget has been already initialized, layer update should only be called on layer change
+            self._on_layer_update()
+        else:
+            return
 
     def _get_adata_layer(self) -> Sequence[Optional[str]]:
         adata_layers = list(self.model.adata.layers.keys())
         if len(adata_layers):
             return adata_layers
         return [None]
 
@@ -258,18 +295,19 @@
     def _save_shapes(self, layer: napari.layers.Shapes, key: str) -> None:
         shape_list = layer._data_view
         triangles = shape_list._mesh.vertices[shape_list._mesh.displayed_triangles]
 
         # TODO(giovp): check if view and save accordingly
         points_mask: NDArrayA = _points_inside_triangles(self.model.coordinates[:, 1:], triangles)
 
-        logger.info("Saving layer shapes.")
+        if self._model._adata is not None:
+            logger.info("Saving layer shapes.")
 
-        self._model._adata.obs[key] = pd.Categorical(points_mask)
-        self._model._adata.uns[key] = {"meshes": layer.data.copy()}
+            self._model._adata.obs[key] = pd.Categorical(points_mask)
+            self._model._adata.uns[key] = {"meshes": layer.data.copy()}
 
     def _update_obs_items(self, key: str) -> None:
         self.obs_widget.addItems(key)
         if key in self.layernames:
             # update already present layer
             layer = self.viewer.layers[key]
             layer.face_color = _get_categorical(self.model.adata, key)
```

### Comparing `napari-spatialdata-0.2.3/src/napari_spatialdata/_widgets.py` & `napari-spatialdata-0.2.4/src/napari_spatialdata/_widgets.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 
 from abc import abstractmethod
 from functools import singledispatchmethod
-from typing import TYPE_CHECKING, Any, Iterable, Optional, Sequence, Union
+from typing import TYPE_CHECKING, Any, Iterable, Sequence
 
 import matplotlib.pyplot as plt
 import napari
 import numpy as np
 import pandas as pd
 from loguru import logger
-from napari.layers import Image, Labels, Layer, Points
+from napari.layers import Labels, Layer, Points, Shapes
 from napari.viewer import Viewer
 from qtpy import QtCore, QtWidgets
 from qtpy.QtCore import Qt, Signal
 from sklearn.preprocessing import MinMaxScaler
 from superqt import QRangeSlider
 from vispy import scene
 from vispy.color.colormap import Colormap, MatplotlibColormap
@@ -46,41 +46,41 @@
 }
 
 
 class ListWidget(QtWidgets.QListWidget):
     indexChanged = Signal(object)
     enterPressed = Signal(object)
 
-    def __init__(self, viewer: napari.Viewer, unique: bool = True, multiselect: bool = True, **kwargs: Any):
+    def __init__(self, viewer: napari.Viewer | None, unique: bool = True, multiselect: bool = True, **kwargs: Any):
         super().__init__(**kwargs)
         if multiselect:
             self.setSelectionMode(QtWidgets.QAbstractItemView.ExtendedSelection)
         else:
             self.setSelectionMode(QtWidgets.QAbstractItemView.SingleSelection)
 
-        self._index: Union[int, str] = 0
+        self._index: int | str = 0
         self._unique = unique
         self._viewer = viewer
 
         self.itemDoubleClicked.connect(lambda item: self._onAction((item.text(),)))
         self.enterPressed.connect(self._onAction)
         self.indexChanged.connect(self._onAction)
 
     @abstractmethod
-    def setIndex(self, index: Union[int, str]) -> None:
+    def setIndex(self, index: int | str) -> None:
         pass
 
-    def getIndex(self) -> Union[int, str]:
+    def getIndex(self) -> int | str:
         return self._index
 
     @abstractmethod
     def _onAction(self, items: Iterable[str]) -> None:
         pass
 
-    def addItems(self, labels: Union[str, Iterable[str]]) -> None:
+    def addItems(self, labels: str | Iterable[str]) -> None:
         if isinstance(labels, str):
             labels = (labels,)
         labels = tuple(labels)
 
         if self._unique:
             labels = tuple(label for label in labels if self.findItems(label, QtCore.Qt.MatchExactly) is not None)
 
@@ -95,150 +95,166 @@
         else:
             super().keyPressEvent(event)
 
 
 class AListWidget(ListWidget):
     layerChanged = Signal()
 
-    def __init__(self, viewer: Viewer, model: ImageModel, attr: str, **kwargs: Any):
+    def __init__(self, viewer: Viewer | None, model: ImageModel, attr: str, **kwargs: Any):
         if attr not in ImageModel.VALID_ATTRIBUTES:
             raise ValueError(f"Invalid attribute `{attr}`. Valid options are `{sorted(ImageModel.VALID_ATTRIBUTES)}`.")
         super().__init__(viewer, **kwargs)
 
         self._viewer = viewer
         self._model = model
 
         self._attr = attr
-        self._getter = getattr(self.model, f"get_{attr}")
 
+        self._getter = getattr(self.model, f"get_{attr}")
         self.layerChanged.connect(self._onChange)
         self._onChange()
 
     def _onChange(self) -> None:
         self.clear()
-        self.addItems(self.model.get_items(self._attr))
+        if self._model.adata is not None:
+            self.addItems(self.model.get_items(self._attr))
 
     def _onAction(self, items: Iterable[str]) -> None:
         for item in sorted(set(items)):
             try:
                 vec, name = self._getter(item, index=self.getIndex())
             except Exception as e:  # noqa: BLE001
                 logger.error(e)
                 continue
+
             if vec.ndim == 2:
                 self.viewer.add_points(
                     vec,
                     name=name,
                     edge_color="white",
                     face_color="white",
                     size=self.model.point_diameter,
                     symbol=self.model.symbol,
                 )
             else:
                 properties = self._get_points_properties(vec, key=item, layer=self.model.layer)
-                if isinstance(self.model.layer, (Image, Points)):
-                    self.viewer.add_points(
-                        self.model.coordinates,
-                        name=name,
-                        size=self.model.spot_diameter,
-                        opacity=1,
-                        face_colormap=self.model.cmap,
-                        edge_colormap=self.model.cmap,
-                        symbol=self.model.symbol,
-                        **properties,
-                    )
+
+                if isinstance(self.model.layer, (Points, Shapes)):
+                    self.model.layer.name = (
+                        "" if self.model.system_name is None else self.model.system_name + ":"
+                    ) + item
+                    self.model.layer.text = None  # needed because of the text-feature order of updates
+                    self.model.layer.features = properties.get("features", None)
+                    self.model.layer.face_color = properties["face_color"]
+                    self.model.layer.text = properties["text"]
                 elif isinstance(self.model.layer, Labels):
-                    self.viewer.add_labels(
-                        self.model.layer.data.copy(),
-                        name=name,
-                        **properties,
-                    )
+                    self.model.layer.name = (
+                        "" if self.model.system_name is None else self.model.system_name + ":"
+                    ) + item
+                    self.model.layer.color = properties["color"]
+                    self.model.layer.properties = properties.get("properties", None)
                 else:
                     raise ValueError("TODO")
                 # TODO(michalk8): add contrasting fg/bg color once https://github.com/napari/napari/issues/2019 is done
                 # TODO(giovp): make layer editable?
                 # self.viewer.layers[layer_name].editable = False
 
-    def setAdataLayer(self, layer: Optional[str]) -> None:
+    def setAdataLayer(self, layer: str | None) -> None:
         if layer in ("default", "None", "X"):
             layer = None
         if layer == self.getAdataLayer():
             return
         self.model.adata_layer = layer
         self.layerChanged.emit()
 
-    def getAdataLayer(self) -> Optional[str]:
+    def getAdataLayer(self) -> str | None:
         if TYPE_CHECKING:
             assert isinstance(self.model.adata_layer, str)
         return self.model.adata_layer
 
-    def setIndex(self, index: Union[int, str]) -> None:
+    def setIndex(self, index: int | str) -> None:
         if isinstance(index, str):
             if index == "":
                 index = 0
             elif self._attr != "obsm":
                 index = int(index, base=10)
             # for obsm, we convert index to int if needed (if not a DataFrame)
         if index == self._index:
             return
 
         self._index = index
         if self._attr == "obsm":
             self.indexChanged.emit(tuple(s.text() for s in self.selectedItems()))
 
-    def getIndex(self) -> Union[int, str]:
+    def getIndex(self) -> int | str:
         return self._index
 
     def _handle_already_present(self, layer_name: str) -> None:
         logger.debug(f"Layer `{layer_name}` is already loaded")
         self.viewer.layers.selection.select_only(self.viewer.layers[layer_name])
 
     @singledispatchmethod
-    def _get_points_properties(self, vec: Union[NDArrayA, pd.Series], **kwargs: Any) -> dict[str, Any]:
+    def _get_points_properties(self, vec: NDArrayA | pd.Series, **kwargs: Any) -> dict[str, Any]:
         raise NotImplementedError(type(vec))
 
     @_get_points_properties.register(np.ndarray)
     def _(self, vec: NDArrayA, **kwargs: Any) -> dict[str, Any]:
         layer = kwargs.pop("layer", None)
+        cmap = plt.get_cmap(self.model.cmap)
+        norm_vec = _min_max_norm(vec)
+        color_vec = cmap(norm_vec)
         if layer is not None and isinstance(layer, Labels):
             cmap = plt.get_cmap(self.model.cmap)
             norm_vec = _min_max_norm(vec)
             color_vec = cmap(norm_vec)
+
             return {
                 "color": dict(zip(self.model.adata.obs[self.model.labels_key].values, color_vec)),
                 "properties": {"value": vec},
-                "metadata": {"perc": (0, 100), "data": vec, "minmax": (np.nanmin(vec), np.nanmax(vec))},
+                "text": None,
             }
+
+        if layer is not None and isinstance(layer, Shapes):
+            cmap = plt.get_cmap(self.model.cmap)
+            norm_vec = _min_max_norm(vec)
+            color_vec = cmap(norm_vec)
+
+            return {
+                "text": None,
+                "face_color": color_vec,
+            }
+
         return {
             "text": None,
-            "face_color": "value",
-            "properties": {"value": vec},
-            "metadata": {"perc": (0, 100), "data": vec, "minmax": (np.nanmin(vec), np.nanmax(vec))},
+            "face_color": color_vec,
         }
 
     @_get_points_properties.register(pd.Series)
     def _(self, vec: pd.Series, key: str, layer: Layer) -> dict[str, Any]:
         colortypes = _set_palette(self.model.adata, key=key, palette=self.model.palette, vec=vec)
         face_color = _get_categorical(
             self.model.adata, key=key, palette=self.model.palette, colordict=colortypes, vec=vec
         )
+
         if layer is not None and isinstance(layer, Labels):
-            return {"color": dict(zip(self.model.adata.obs[self.model.labels_key].values, face_color))}
+            return {"color": dict(zip(self.model.adata.obs[self.model.labels_key].values, face_color)), "text": None}
+
+        if layer is not None and isinstance(layer, Shapes):
+            return {"face_color": face_color, "metadata": None, "text": None}
 
         cluster_labels = _position_cluster_labels(self.model.coordinates, vec)
         return {
             "text": {
                 "string": "{clusters}",
                 "size": 24,
                 "color": {"feature": "clusters", "colormap": colortypes},
                 "anchor": "center",
             },
             "face_color": face_color,
             "features": cluster_labels,
-            "metadata": None,
         }
 
     @property
     def viewer(self) -> napari.Viewer:
         """:mod:`napari` viewer."""
         return self._viewer
 
@@ -254,15 +270,15 @@
 
         self._model = model
         self.view().setVerticalScrollBarPolicy(QtCore.Qt.ScrollBarAsNeeded)
         self.setMaxVisibleItems(max_visible)
         self.setStyleSheet("combobox-popup: 0;")
         self._attr = attr
 
-    def addItems(self, texts: Union[QtWidgets.QListWidgetItem, int, Iterable[str]]) -> None:
+    def addItems(self, texts: QtWidgets.QListWidgetItem | int | Iterable[str]) -> None:
         if isinstance(texts, QtWidgets.QListWidgetItem):
             try:
                 key = texts.text()
                 if isinstance(self._model.adata.obsm[key], pd.DataFrame):
                     texts = sorted(self._model.adata.obsm[key].select_dtypes(include=[np.number, "category"]).columns)
                 elif hasattr(self._model.adata.obsm[key], "shape"):
                     texts = self._model.adata.obsm[key].shape[1]
@@ -281,47 +297,47 @@
             super().setToolTip("Indices for current key in `adata.obsm`. Choose by clicking on item from obsm list.")
         elif click == "var":
             super().setToolTip("Keys in `adata.layers`.")
         else:
             super().setToolTip("")
         return
 
-    def setAttribute(self, field: Optional[str]) -> None:
+    def setAttribute(self, field: str | None) -> None:
         if field == self.attr:
             return
         self.attr = field
         self._onChange()
 
     def _onChange(self) -> None:
         if self.attr == "var":
             self.clear()
             super().addItems(self._getAllLayers())
         else:
             self.clear()
 
-    def _onClickChange(self, clicked: Union[QtWidgets.QListWidgetItem, int, Iterable[str]]) -> None:
+    def _onClickChange(self, clicked: QtWidgets.QListWidgetItem | int | Iterable[str]) -> None:
         if self.attr == "obsm":
             self.clear()
             self.addItems(clicked)
 
-    def _getAllLayers(self) -> Sequence[Optional[str]]:
+    def _getAllLayers(self) -> Sequence[str | None]:
         adata_layers = list(self._model.adata.layers.keys())
         if len(adata_layers):
             adata_layers.insert(0, "X")
             return adata_layers
         return ["X"]
 
     @property
-    def attr(self) -> Optional[str]:
+    def attr(self) -> str | None:
         if TYPE_CHECKING:
             assert isinstance(self._attr, str)
         return self._attr
 
     @attr.setter
-    def attr(self, field: Optional[str]) -> None:
+    def attr(self, field: str | None) -> None:
         if field not in ("var", "obs", "obsm"):
             raise ValueError(f"{field} is not a valid adata field.")
         self._attr = field
 
 
 class CBarWidget(QtWidgets.QWidget):
     FORMAT = "{0:0.2f}"
@@ -329,17 +345,17 @@
     cmapChanged = Signal(str)
     climChanged = Signal((float, float))
 
     def __init__(
         self,
         model: ImageModel,
         cmap: str = "viridis",
-        label: Optional[str] = None,
-        width: Optional[int] = 250,
-        height: Optional[int] = 50,
+        label: str | None = None,
+        width: int | None = 250,
+        height: int | None = 50,
         **kwargs: Any,
     ):
         super().__init__(**kwargs)
 
         self._model = model
 
         self._clim = (0.0, 1.0)
```

### Comparing `napari-spatialdata-0.2.3/src/napari_spatialdata/napari.yaml` & `napari-spatialdata-0.2.4/src/napari_spatialdata/napari.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -4,12 +4,19 @@
   commands:
     - id: napari-spatialdata.QtAdataScatterWidget
       python_name: napari_spatialdata._view:QtAdataScatterWidget
       title: Visualize spatial omics data in napari
     - id: napari-spatialdata.QtAdataViewWidget
       python_name: napari_spatialdata._view:QtAdataViewWidget
       title: Visualize spatial omics data in napari
+    - id: napari-spatialdata.get_reader
+      python_name: napari_spatialdata:get_reader
+      title: Get napari Reader for spatialdata
   widgets:
     - command: napari-spatialdata.QtAdataScatterWidget
       display_name: Scatter
     - command: napari-spatialdata.QtAdataViewWidget
       display_name: View
+  readers:
+    - command: napari-spatialdata.get_reader
+      accepts_directories: true
+      filename_patterns: ["*.zarr"]
```

### Comparing `napari-spatialdata-0.2.3/src/napari_spatialdata.egg-info/PKG-INFO` & `napari-spatialdata-0.2.4/src/napari_spatialdata.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-spatialdata
-Version: 0.2.3
+Version: 0.2.4
 Summary: Interactive visualization of spatial omics data with napari
 Home-page: https://github.com/scverse/napari-spatialdata.git
 Author: giovanni palla
 Author-email: giov.pll@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/scverse/napari-spatialdata/issues
 Project-URL: Documentation, https://github.com/scverse/napari-spatialdata#README.md
@@ -20,39 +20,30 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: doc
+Provides-Extra: all
 License-File: LICENSE
 
-# napari-spatialdata
+![SpatialData banner](https://github.com/scverse/spatialdata/blob/main/docs/_static/img/spatialdata_horizontal.png?raw=true)
+
+# napari-spatialdata: interactive exploration and annotation of spatial omics data
 
 [![License](https://img.shields.io/pypi/l/napari-spatialdata.svg?color=green)](https://github.com/scverse/napari-spatialdata/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-spatialdata.svg?color=green)](https://pypi.org/project/napari-spatialdata)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-spatialdata.svg?color=green)](https://python.org)
 [![tests](https://github.com/scverse/napari-spatialdata/workflows/tests/badge.svg)](https://github.com/scverse/napari-spatialdata/actions)
 [![codecov](https://codecov.io/gh/scverse/napari-spatialdata/branch/main/graph/badge.svg?token=ASqlOKnOj7)](https://codecov.io/gh/scverse/napari-spatialdata)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/scverse/napari-spatialdata/main.svg)](https://results.pre-commit.ci/latest/github/scverse/napari-spatialdata/main)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-spatialdata)](https://napari-hub.org/plugins/napari-spatialdata)
 
-Interactive visualization of spatial omics data with napari
-
----
-
-This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
-
-<!--
-Don't miss the full getting started guide to set up your new package:
-https://github.com/napari/cookiecutter-napari-plugin#getting-started
-
-and review the napari docs for plugin developers:
-https://napari.org/plugins/stable/index.html
--->
+This repository contains a napari plugin for interactively exploring and annotating SpatialData objects. `napari-spatialdata` is part of the `SpatialData` ecosystem. To learn more about SpatialData, please see the [documentation](https://spatialdata.scverse.org/).
 
 ## Installation
 
 You can install `napari-spatialdata` via [pip]:
 
     pip install napari-spatialdata
 
@@ -64,14 +55,21 @@
 
 Or, you can also install in editable mode after cloning the repo by:
 
     git clone https://github.com/scverse/napari-spatialdata
     cd napari-spatialdata
     pip install -e .
 
+## Getting started
+
+To learn how to use the `napari-spatialdata` plugin, please see the [documentation](https://spatialdata.scverse.org/projects/napari/en/latest/notebooks/spatialdata.html). To learn how to integrate napari-spatialdata into your analysis workflows, please see the [SpatialData tutorials](https://spatialdata.scverse.org/en/latest/tutorials/notebooks/notebooks.html). In particular:
+
+- [Annotating regions of interest with napari](https://spatialdata.scverse.org/en/latest/tutorials/notebooks/notebooks/examples/napari_rois.html)
+- [Use landmark annotations to align multiple -omics layers](https://spatialdata.scverse.org/en/latest/tutorials/notebooks/notebooks/examples/alignment_using_landmarks.html)
+
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
```

### Comparing `napari-spatialdata-0.2.3/src/napari_spatialdata.egg-info/SOURCES.txt` & `napari-spatialdata-0.2.4/src/napari_spatialdata.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -9,37 +9,38 @@
 pyproject.toml
 setup.cfg
 tox.ini
 .github/workflows/test_and_deploy.yml
 .napari/DESCRIPTION.md
 docs/Makefile
 docs/api.md
-docs/changelog.md
+docs/cli.md
 docs/conf.py
 docs/contributing.md
 docs/index.md
 docs/make.bat
 docs/references.bib
 docs/references.md
 docs/template_usage.md
 docs/_static/.gitkeep
 docs/_templates/.gitkeep
 docs/_templates/autosummary/class.rst
 docs/extensions/typed_returns.py
 docs/notebooks/mibitof_analysis.ipynb
 docs/notebooks/nanostring_analysis.ipynb
+docs/notebooks/scatterwidget.ipynb
 docs/notebooks/spatialdata.ipynb
-examples/README.md
-examples/spatialdata_mibitof.py
-examples/spatialdata_nanostring.py
+examples/spatialdata_empty.py
 examples/spatialdata_visium.py
 src/napari_spatialdata/__init__.py
+src/napari_spatialdata/__main__.py
 src/napari_spatialdata/_categoricals_utils.py
 src/napari_spatialdata/_interactive.py
 src/napari_spatialdata/_model.py
+src/napari_spatialdata/_reader.py
 src/napari_spatialdata/_scatterwidgets.py
 src/napari_spatialdata/_utils.py
 src/napari_spatialdata/_version.py
 src/napari_spatialdata/_view.py
 src/napari_spatialdata/_widgets.py
 src/napari_spatialdata/napari.yaml
 src/napari_spatialdata.egg-info/PKG-INFO
```

### Comparing `napari-spatialdata-0.2.3/tests/conftest.py` & `napari-spatialdata-0.2.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.3/tests/test_interactive.py` & `napari-spatialdata-0.2.4/tests/test_interactive.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import platform
 from typing import Any, Union
 
 import numpy as np
 import pandas as pd
 import pytest
 from anndata import AnnData
 from napari.layers import Image, Labels
@@ -29,25 +28,21 @@
     )
 
     # create our widget, passing in the viewer
     _ = widget(viewer)
     viewer.layers.selection.events.changed.disconnect()
 
 
-@pytest.mark.skipif(platform.system() == "Linux", reason="Fails on ubuntu CI")
-@pytest.mark.skipif(platform.system() == "Darwin", reason="Fails on macos CI, but locally it is fine")
 @pytest.mark.parametrize("widget", [QtAdataViewWidget, QtAdataScatterWidget])
 def test_creating_widget_with_no_adata(make_napari_viewer: Any, widget: Any) -> None:
     # make viewer and add an image layer using our fixture
     viewer = make_napari_viewer()
 
     # create our widget, passing in the viewer
-    # with pytest.raises(NotImplementedError, match=r":class:`anndata.AnnData` not found in any `layer.metadata`."):
-    with pytest.raises(AttributeError, match=r"'NoneType' object has no attribute 'metadata'"):
-        _ = widget(viewer)
+    _ = widget(viewer)
     viewer.layers.selection.events.changed.disconnect()
 
 
 @pytest.mark.parametrize("widget", [QtAdataViewWidget])
 def test_model(
     make_napari_viewer: Any,
     widget: Any,
```

### Comparing `napari-spatialdata-0.2.3/tests/test_scatterwidgets.py` & `napari-spatialdata-0.2.4/tests/test_scatterwidgets.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.3/tests/test_spatialdata.py` & `napari-spatialdata-0.2.4/tests/test_spatialdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,16 +47,14 @@
     assert len(widget._viewer.layers) == 0
     widget.coordinate_system_widget._select_coord_sys("global")
     widget.elements_widget._onClickChange("global")
     widget._onClick(list(sdata.images.keys())[0])
     assert len(widget._viewer.layers) == 1
     assert isinstance(widget._viewer.layers[0], Image)
     assert widget._viewer.layers[0].name == list(sdata.images.keys())[0]
-    assert isinstance(widget._viewer.layers[0].metadata.get("adata"), AnnData)
-    assert widget._viewer.layers[0].metadata.get("adata").shape == (0, 0)
     sdata.images["image"] = to_multiscale(sdata.images["blobs_image"], [2, 4])
     widget.elements_widget._onClickChange("global")
     widget._onClick("image")
     assert len(widget._viewer.layers) == 2
     assert (widget._viewer.layers[0].data == widget._viewer.layers[1].data).all()
     del sdata.images["image"]
```

### Comparing `napari-spatialdata-0.2.3/tests/test_utils.py` & `napari-spatialdata-0.2.4/tests/test_utils.py`

 * *Files identical despite different names*

