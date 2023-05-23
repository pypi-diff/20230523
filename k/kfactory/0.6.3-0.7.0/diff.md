# Comparing `tmp/kfactory-0.6.3.tar.gz` & `tmp/kfactory-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfactory-0.6.3.tar", last modified: Fri Apr 21 19:57:59 2023, max compression
+gzip compressed data, was "kfactory-0.7.0.tar", last modified: Tue May 23 05:30:28 2023, max compression
```

## Comparing `kfactory-0.6.3.tar` & `kfactory-0.7.0.tar`

### file list

```diff
@@ -1,93 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:57:59.395300 kfactory-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-21 19:57:41.000000 kfactory-0.6.3/.bumpversion.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:57:59.387300 kfactory-0.6.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-21 19:57:41.000000 kfactory-0.6.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:57:59.387300 kfactory-0.6.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-21 19:57:41.000000 kfactory-0.6.3/.github/workflows/pages.yml
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-21 19:57:41.000000 kfactory-0.6.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-21 19:57:41.000000 kfactory-0.6.3/.github/workflows/test_code.yml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-21 19:57:41.000000 kfactory-0.6.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-04-21 19:57:41.000000 kfactory-0.6.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-21 19:57:41.000000 kfactory-0.6.3/.sourcery.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-21 19:57:41.000000 kfactory-0.6.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-21 19:57:41.000000 kfactory-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-21 19:57:41.000000 kfactory-0.6.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-21 19:57:59.395300 kfactory-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-21 19:57:41.000000 kfactory-0.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:57:59.387300 kfactory-0.6.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:57:59.391300 kfactory-0.6.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   138035 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/_static/complex.png
--rw-r--r--   0 runner    (1001) docker     (123)   985194 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/_static/klive.webm
--rw-r--r--   0 runner    (1001) docker     (123)   129785 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/_static/waveguide.png
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/complex_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/klive.rst
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:57:59.391300 kfactory-0.6.3/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    11525 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/notebooks/00_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13535 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/notebooks/01_references.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/notebooks/02_DRC.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/notebooks/03_Enclosures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/star.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-21 19:57:41.000000 kfactory-0.6.3/docs/waveguide.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-21 19:57:41.000000 kfactory-0.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 19:57:59.395300 kfactory-0.6.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:57:59.387300 kfactory-0.6.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:57:59.391300 kfactory-0.6.3/src/kfactory/
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/generic_tech.py
--rw-r--r--   0 runner    (1001) docker     (123)    81247 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/kcell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:57:59.391300 kfactory-0.6.3/src/kfactory/pcells/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/pcells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/pcells/bezier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/pcells/circular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:57:59.391300 kfactory-0.6.3/src/kfactory/pcells/dbu/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/pcells/dbu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/pcells/dbu/taper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/pcells/dbu/waveguide.py
--rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/pcells/euler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/pcells/taper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/pcells/waveguide.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/placer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/port.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:57:59.395300 kfactory-0.6.3/src/kfactory/routing/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9993 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/routing/electrical.py
--rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/routing/manhattan.py
--rw-r--r--   0 runner    (1001) docker     (123)    20349 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/routing/optical.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:57:59.395300 kfactory-0.6.3/src/kfactory/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35789 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/utils/enclosure.py
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/utils/fill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/utils/simplify.py
--rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/utils/violations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:57:59.395300 kfactory-0.6.3/src/kfactory/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12502 2023-04-21 19:57:41.000000 kfactory-0.6.3/src/kfactory/widgets/interactive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:57:59.391300 kfactory-0.6.3/src/kfactory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-21 19:57:59.000000 kfactory-0.6.3/src/kfactory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-21 19:57:59.000000 kfactory-0.6.3/src/kfactory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 19:57:59.000000 kfactory-0.6.3/src/kfactory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-21 19:57:59.000000 kfactory-0.6.3/src/kfactory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-21 19:57:59.000000 kfactory-0.6.3/src/kfactory.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:57:59.395300 kfactory-0.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-21 19:57:41.000000 kfactory-0.6.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-21 19:57:41.000000 kfactory-0.6.3/tests/test_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-21 19:57:41.000000 kfactory-0.6.3/tests/test_cplxcells.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-21 19:57:41.000000 kfactory-0.6.3/tests/test_enclosure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-21 19:57:41.000000 kfactory-0.6.3/tests/test_extrude.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-21 19:57:41.000000 kfactory-0.6.3/tests/test_ports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-21 19:57:41.000000 kfactory-0.6.3/tests/test_rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-21 19:57:41.000000 kfactory-0.6.3/tests/test_routing.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-21 19:57:41.000000 kfactory-0.6.3/tests/test_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-04-21 19:57:41.000000 kfactory-0.6.3/tests/test_spiral.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:28.466122 kfactory-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-23 05:30:10.000000 kfactory-0.7.0/.bumpversion.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:28.454122 kfactory-0.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:28.454122 kfactory-0.7.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-23 05:30:10.000000 kfactory-0.7.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-23 05:30:10.000000 kfactory-0.7.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-23 05:30:10.000000 kfactory-0.7.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:28.454122 kfactory-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-23 05:30:10.000000 kfactory-0.7.0/.github/workflows/pages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-23 05:30:10.000000 kfactory-0.7.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-23 05:30:10.000000 kfactory-0.7.0/.github/workflows/test_code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-23 05:30:10.000000 kfactory-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-23 05:30:10.000000 kfactory-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-23 05:30:10.000000 kfactory-0.7.0/.sourcery.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-23 05:30:10.000000 kfactory-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-23 05:30:10.000000 kfactory-0.7.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-23 05:30:28.466122 kfactory-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-23 05:30:10.000000 kfactory-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:28.458122 kfactory-0.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:28.458122 kfactory-0.7.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   138035 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/_static/complex.png
+-rw-r--r--   0 runner    (1001) docker     (123)   985194 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/_static/klive.webm
+-rw-r--r--   0 runner    (1001) docker     (123)   129785 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/_static/waveguide.png
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/_toc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/complex_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/config.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/intro.md
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/klive.md
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:28.458122 kfactory-0.7.0/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    10750 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/notebooks/00_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13152 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/notebooks/01_references.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/notebooks/02_DRC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/notebooks/03_Enclosures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/star.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-23 05:30:10.000000 kfactory-0.7.0/docs/waveguide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-23 05:30:10.000000 kfactory-0.7.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-05-23 05:30:10.000000 kfactory-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 05:30:28.466122 kfactory-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:28.454122 kfactory-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:28.462122 kfactory-0.7.0/src/kfactory/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:28.462122 kfactory-0.7.0/src/kfactory/cells/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/cells/bezier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/cells/circular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:28.462122 kfactory-0.7.0/src/kfactory/cells/dbu/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/cells/dbu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/cells/dbu/taper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/cells/dbu/waveguide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/cells/euler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/cells/taper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/cells/waveguide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90612 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/kcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/pdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/placer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:28.462122 kfactory-0.7.0/src/kfactory/routing/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/routing/electrical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12507 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/routing/manhattan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20414 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/routing/optical.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:28.462122 kfactory-0.7.0/src/kfactory/technology/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/technology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/technology/color_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/technology/klayout_tech.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/technology/layer_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14087 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/technology/layer_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41776 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/technology/layer_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/technology/xml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/technology/yaml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/typings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:28.466122 kfactory-0.7.0/src/kfactory/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55837 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/utils/enclosure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/utils/fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/utils/simplify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9316 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/utils/violations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:28.466122 kfactory-0.7.0/src/kfactory/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14853 2023-05-23 05:30:10.000000 kfactory-0.7.0/src/kfactory/widgets/interactive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:28.462122 kfactory-0.7.0/src/kfactory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-23 05:30:28.000000 kfactory-0.7.0/src/kfactory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-23 05:30:28.000000 kfactory-0.7.0/src/kfactory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 05:30:28.000000 kfactory-0.7.0/src/kfactory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-23 05:30:28.000000 kfactory-0.7.0/src/kfactory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 05:30:28.000000 kfactory-0.7.0/src/kfactory.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 05:30:28.466122 kfactory-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-23 05:30:10.000000 kfactory-0.7.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-23 05:30:10.000000 kfactory-0.7.0/tests/test_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-05-23 05:30:10.000000 kfactory-0.7.0/tests/test_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-23 05:30:10.000000 kfactory-0.7.0/tests/test_cplxcells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-23 05:30:10.000000 kfactory-0.7.0/tests/test_enclosure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-23 05:30:10.000000 kfactory-0.7.0/tests/test_extrude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-23 05:30:10.000000 kfactory-0.7.0/tests/test_pdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-05-23 05:30:10.000000 kfactory-0.7.0/tests/test_ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-23 05:30:10.000000 kfactory-0.7.0/tests/test_rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-23 05:30:10.000000 kfactory-0.7.0/tests/test_routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-23 05:30:10.000000 kfactory-0.7.0/tests/test_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-23 05:30:10.000000 kfactory-0.7.0/tests/test_spiral.py
```

### Comparing `kfactory-0.6.3/.github/workflows/pages.yml` & `kfactory-0.7.0/.github/workflows/pages.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 name: Sphinx docs to gh-pages
 
 on:
   push:
     branches:
       - main
+    # tags:
+    #   v[0-9]+.[0-9]+.[0-9]+
   workflow_dispatch:
 
 jobs:
-  sphinx_docs_to_gh-pages:
+  build-docs:
     runs-on: ubuntu-latest
     name: Sphinx docs to gh-pages
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: "3.10"
           cache: "pip"
           cache-dependency-path: pyproject.toml
       - name: Installing the library
         shell: bash -l {0}
         run: |
           pip install -e .[ci,docs]
-          sudo apt install pandoc
-      - name: Clean docs and create notebooks
-        shell: bash -l {0}
-        run: |
-          cd docs
-          make clean
-          make convert
-          cd -
-      - name: Running the Sphinx to gh-pages Action
-        uses: uibcdf/action-sphinx-docs-to-gh-pages@v1.1.0-beta
-        with:
-          branch: main
-          dir_docs: docs
-          sphinxopts: ""
+          export KFACTORY_DISPLAY_TYPE="image"
+          mkdocs gh-deploy --force
+  deploy-docs:
+    needs: build-docs
+    permissions:
+      pages: write
+      id-token: write
+
+    environment:
+      name: github-pages
+      url: ${{ steps.deployment.outputs.page_url }}
+
+    runs-on: ubuntu-latest
+    steps:
+      - name: Deploy to GitHub Pages
+        id: deployment
+        uses: actions/deploy-pages@v2
```

### Comparing `kfactory-0.6.3/.github/workflows/release.yml` & `kfactory-0.7.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.3/.github/workflows/test_code.yml` & `kfactory-0.7.0/.github/workflows/test_code.yml`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,14 @@
       - uses: actions/setup-python@v4
       - name: Install ci dependencies
         run: |
           python -m pip install -U pip
           python -m pip install -e .[ci]
       - uses: pre-commit/action@v3.0.0
   test_code:
-    needs: [pre-commit]
     runs-on: ${{ matrix.os }}
     strategy:
       max-parallel: 12
       matrix:
         python-version: ["3.10"]
         os: [ubuntu-latest, windows-latest, macos-latest]
     steps:
@@ -30,20 +29,24 @@
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
           cache: "pip"
           cache-dependency-path: pyproject.toml
       - name: Install dependencies
+        env:
+          GH_TOKEN: ${{ github.token }}
         run: |
           pip install -e .[ci]
+          make gds-download
       - name: Test with pytest
-        run: pytest -vv
+        env:
+          KFACTORY_LOGFILTER__LEVEL: "ERROR"
+        run: pytest -vv -s
   test_docs:
-    needs: [pre-commit]
     runs-on: ${{ matrix.os }}
     strategy:
       max-parallel: 12
       matrix:
         python-version: ["3.10"]
         os: [ubuntu-latest]
 
@@ -57,15 +60,11 @@
           channel-priority: true
           activate-environment: anaconda-client-env
       - name: Install dependencies
         run: |
           python -m pip install --user -U pip
           python -m pip install --user -e .[docs,ci]
           python -m ipykernel install --user --name python3
-          sudo apt install pandoc
           make install
       - name: Test documentation
         run: |
-          cd docs
-          make clean
-          make convert
-          make html
+          make docs
```

### Comparing `kfactory-0.6.3/.pre-commit-config.yaml` & `kfactory-0.7.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,28 @@
     rev: "v4.4.0"
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-symlinks
       - id: check-yaml
+        args: []
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
       - id: name-tests-test
         args: ["--pytest-test-first"]
       - id: requirements-txt-fixer
       - id: trailing-whitespace
 
+  - repo: https://github.com/asottile/pyupgrade
+    rev: v3.4.0
+    hooks:
+      - id: pyupgrade
+
   # - repo: https://github.com/pre-commit/pre-commit-hooks
   #   rev: a41c4b94b220171e928ff3e6c9bef34e71267f46
   #   hooks:
   #     - id: check-yaml
   #       exclude: ^(conda\.recipe/meta\.yaml|conda_build/templates/.*\.yaml|docs/click/meta\.yaml|conda/meta\.yaml|construct.yaml)
   #     - id: end-of-file-fixer
   #     - id: trailing-whitespace
@@ -56,15 +62,15 @@
   - repo: https://github.com/kynan/nbstripout
     rev: 0.6.1
     hooks:
       - id: nbstripout
         files: .ipynb
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+    rev: v3.4.0
     hooks:
       - id: pyupgrade
         args: [--py37-plus, --keep-runtime-typing]
 
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.4
     hooks:
```

### Comparing `kfactory-0.6.3/LICENSE` & `kfactory-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.3/Makefile` & `kfactory-0.7.0/Makefile`

 * *Files 20% similar despite different names*

```diff
@@ -7,16 +7,19 @@
 	pip install -e .[docs,dev]
 	pre-commit install
 
 docs-clean:
 	rm -rf docs/_autosummary/
 	rm -rf docs/build
 
+docs:
+	mkdocs build
+
 test:
-	pytest
+	pytest -s
 
 cov:
 	pytest --cov=kfactory
 
 venv:
 	python3 -m venv env
 
@@ -44,8 +47,14 @@
 update-pre:
 	pre-commit autoupdate --bleeding-edge
 
 release:
 	git push
 	git push origin --tags
 
-.PHONY: build
+gds-upload:
+	gh release upload v0.6.0 gds/gds_ref/*.gds --clobber
+
+gds-download:
+	gh release download v0.6.0 -D gds/gds_ref/ --clobber
+
+.PHONY: build docs
```

### Comparing `kfactory-0.6.3/PKG-INFO` & `kfactory-0.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: kfactory
-Version: 0.6.3
+Version: 0.7.0
 Summary: KLayout API implementation of gdsfactory
 Author-email: gdsfactory community <contact@gdsfactory.com>
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Provides-Extra: git
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: ci
 Provides-Extra: ipy
 License-File: LICENSE
 
-# KFactory 0.6.3
+# KFactory 0.7.0
 
 Kfactory is a [gdsfactory](https://github.com/gdsfactory/gdsfactory)-like tool. It is built with [KLayout](https://klayout.de) as a backend instead of gdstk, but aims to offer the similar featuers.
 
 Features similar to gdsfactory:
 
 - [x] Cells & decorator for caching & storing cells
 - [x] Simple routing (point to point and simpl bundle routes for electrical routes)
```

### Comparing `kfactory-0.6.3/README.md` & `kfactory-0.7.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.3/docs/README.md` & `kfactory-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# KFactory 0.6.3
+# KFactory 0.7.0
 
 Kfactory is a [gdsfactory](https://github.com/gdsfactory/gdsfactory)-like tool. It is built with [KLayout](https://klayout.de) as a backend instead of gdstk, but aims to offer the similar featuers.
 
 Features similar to gdsfactory:
 
 - [x] Cells & decorator for caching & storing cells
 - [x] Simple routing (point to point and simpl bundle routes for electrical routes)
```

### Comparing `kfactory-0.6.3/docs/_static/complex.png` & `kfactory-0.7.0/docs/_static/complex.png`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.3/docs/_static/klive.webm` & `kfactory-0.7.0/docs/_static/klive.webm`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.3/docs/_static/waveguide.png` & `kfactory-0.7.0/docs/_static/waveguide.png`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.3/docs/complex_cell.py` & `kfactory-0.7.0/docs/complex_cell.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,40 @@
+# ---
+# jupyter:
+#   jupytext:
+#     cell_metadata_filter: -all
+#     text_representation:
+#       extension: .py
+#       format_name: light
+#       format_version: '1.5'
+#       jupytext_version: 1.14.5
+#   kernelspec:
+#     display_name: kernel_name
+#     language: python
+#     name: kernel_name
+# ---
+
 from layers import LAYER, si_enc
 from waveguide import waveguide
 
 import kfactory as kf
 
 
-@kf.autocell
+@kf.cell
 def composite_cell() -> kf.KCell:
     c = kf.KCell()
 
     bend = c.create_inst(
-        kf.pcells.circular.bend_circular(
-            1000 * c.klib.dbu, 20000 * c.klib.dbu, LAYER.SI, enclosure=si_enc
-        )  # the standard kf.pcells are in um, so we need to convert to dbu
+        kf.cells.circular.bend_circular(
+            1000 * c.kcl.dbu, 20000 * c.kcl.dbu, LAYER.SI, enclosure=si_enc
+        )  # the standard kf.cells are in um, so we need to convert to dbu
     )
     wg = c << waveguide(1000, 5000, 5000)
 
-    wg.connect("o1", bend, "o2")
+    wg.align("o1", bend, "o2")
 
     c.add_port(name="1", port=bend.ports["o1"])
     c.add_port(name="2", port=wg.ports["o2"])
 
     c.autorename_ports()
 
     c.draw_ports()
```

### Comparing `kfactory-0.6.3/docs/notebooks/00_geometry.py` & `kfactory-0.7.0/docs/notebooks/00_geometry.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # ---
 # jupyter:
 #   jupytext:
 #     custom_cell_magics: kql
-#     formats: ipynb,py
+#     formats: ipynb,py:light
 #     text_representation:
 #       extension: .py
 #       format_name: light
 #       format_version: '1.5'
 #       jupytext_version: 1.14.5
 #   kernelspec:
 #     display_name: Python 3 (ipykernel)
@@ -22,118 +22,116 @@
 #
 # Most Shape types are available as microns and dbu parts. They can be converted with <ShapeTypeDBU>.to_dtype(dbu) to microns and with <ShapeTypeMicrons>.to_itype(dbu) where dbu is the the conversion of one database unit to microns
 #
 # Lets add a polygon
 # # KCell
 #
 #
-# A `Cell` is like an empty canvas, where you can add polygons, references to other Components and ports (to connect to other components)
+# A `Cell` is like an empty canvas, where you can add polygons, references to other Cells and ports (to connect to other cells)
 #
 # In KLayout geometries are in datatabase units (dbu) or microns. GDS uses an integer grid as a basis for geometries. The default is `0.001`, i.e. 1nm grid size (0.001 microns)
 #
 # `Point`, `Box`, `Polygon`, `Edge`, `Region` are in dbu
 # `DPoint`, `DBox`, `DPolygon`, `DEdge` are in microns
 #
 # Most Shape types are available as microns and dbu parts. They can be converted with `<ShapeTypeDBU>.to_dtype(dbu)` to microns and with `<ShapeTypeMicrons>.to_itype(dbu)` where `dbu` is the the conversion of one database unit to microns
 
-# + vscode={"languageId": "python"}
+
 import kfactory as kf
 
-# Create a blank component (essentially an empty GDS cell with some special features)
+# Create a blank cell (essentially an empty GDS cell with some special features)
 c = kf.KCell()
 
 # Create and add a polygon from separate lists of x points and y points
 # (Can also be added like [(x1,y1), (x2,y2), (x3,y3), ... ]
 poly1 = kf.kdb.DPolygon(
     [
         kf.kdb.DPoint(-8, -6),
         kf.kdb.DPoint(6, 8),
         kf.kdb.DPoint(7, 17),
         kf.kdb.DPoint(9, 5),
     ]
 )
 
 
-c.shapes(c.klib.layer(1, 0)).insert(poly1)
+c.shapes(c.kcl.layer(1, 0)).insert(poly1)
 # show it in matplotlib and KLayout (you need to have KLayout open and install gdsfactory from the git repo with make install)
 
 c
 
 # -
 
 
 # **Exercise** :
 #
-# Make a component similar to the one above that has a second polygon in layer (1, 1)
+# Make a cell similar to the one above that has a second polygon in layer (1, 1)
 
-# + vscode={"languageId": "python"}
 import kfactory as kf
 
 c = kf.KCell()
 
 # Create some new geometry from the functions available in the geometry library
 textgenerator = kf.kdb.TextGenerator.default_generator()
-t = textgenerator.text("Hello!", c.klib.dbu)
-# t = gf.components.text("Hello!")
+t = textgenerator.text("Hello!", c.kcl.dbu)
+# t = gf.cells.text("Hello!")
 
 r = kf.kdb.DBox(-2.5, -5, 2.5, 5)
-# r = gf.components.rectangle(size=[5, 10], layer=(2, 0))
+# r = gf.cells.rectangle(size=[5, 10], layer=(2, 0))
 
-# Add references to the new geometry to c, our blank component
+# Add references to the new geometry to c, our blank cell
 
 # c.shapes(layer(1,0)).insert(t)
 # text1 = c.add_ref(t)  # Add the text we created as a reference
 # Using the << operator (identical to add_ref()), add the same geometry a second time
 # text2 = c << t
 # r = c << r  # Add the rectangle we created
 
 # Now that the geometry has been added to "c", we can move everything around:
 text1 = t.transformed(
-    kf.kdb.DTrans(0.0, 10.0).to_itype(c.klib.dbu)
+    kf.kdb.DTrans(0.0, 10.0).to_itype(c.kcl.dbu)
 )  # DTrans is a transformation in microns with arguments (<rotation in 90° increments>, <mirror boolean>, <x in microns>, <y in microns>)
 ### complex transformation example:ce
 #     magnification(float): magnification, DO NOT USE on cells or references, only shapes, most foundries will not allow magnifications on actual cell references or cells
 #     rotation(float): rotation in degrees
 #     mirror(bool): boolean to mirror at x axis and then rotate if true
 #     x(float): x coordinate
 #     y(float): y coordinate
 #
 text2 = t.transformed(
-    kf.kdb.DCplxTrans(2.0, 45.0, False, 5.0, 30.0).to_itrans(c.klib.dbu)
+    kf.kdb.DCplxTrans(2.0, 45.0, False, 5.0, 30.0).to_itrans(c.kcl.dbu)
 )
 # text1.movey(25)
 # text2.move([5, 30])
 # text2.rotate(45)
 r.move(
     -5, 0
 )  # boxes can be moved like this, other shapes and cellss/refs need to be moved with .transform
 r.move(-5, 0)
 
 
-c.shapes(c.klib.layer(1, 0)).insert(text1)
-c.shapes(c.klib.layer(2, 0)).insert(text2)
-c.shapes(c.klib.layer(2, 0)).insert(r)
+c.shapes(c.kcl.layer(1, 0)).insert(text1)
+c.shapes(c.kcl.layer(2, 0)).insert(text2)
+c.shapes(c.kcl.layer(2, 0)).insert(r)
 
 c
 # -
 
-# ## Connect **ports**
+# ## connect **ports**
 #
-# Components can have a "Port" that allows you to connect ComponentReferences together like legos.
+# Cells can have a "Port" that allows you to connect Instances together like legos.
 #
 # You can write a simple function to make a rectangular straight, assign ports to the ends, and then connect those rectangles together.
 
 
-# + vscode={"languageId": "python"}
-@kf.autocell
+@kf.cell
 def straight(length=10, width=1, layer=(1, 0)):
     wg = kf.KCell()
     box = kf.kdb.DBox(length, width)
-    int_box = box.to_itype(wg.klib.dbu)
-    _layer = kf.klib.layer(*layer)
+    int_box = box.to_itype(wg.kcl.dbu)
+    _layer = kf.kcl.layer(*layer)
     wg.shapes(_layer).insert(box)
     wg.add_port(
         kf.Port(
             name="o1",
             dwidth=width,
             dcplx_trans=kf.kdb.DCplxTrans(1, 180, False, box.left, box.center().y),
             layer=_layer,
@@ -158,111 +156,110 @@
 # wg2.transform(kf.kdb.DCplxTrans(1, 10, False, 10, 0))
 # wg3.transform(kf.kdb.DCplxTrans(1, 15, False, 20, 0))
 # wg2.movey(10).rotate(10)
 # wg3.movey(20).rotate(15)
 print(c.name)
 c
 
-# + vscode={"languageId": "python"}
-# Now we can connect everything together using the ports:
+# Now we can align everything together using the ports:
 
 # Each straight has two ports: 'W0' and 'E0'.  These are arbitrary
 # names defined in our straight() function above
 
 # Let's keep wg1 in place on the bottom, and connect the other straights to it.
 # To do that, on wg2 we'll grab the "W0" port and connect it to the "E0" on wg1:
 wg2.connect("o1", wg1.ports["o2"])
 # Next, on wg3 let's grab the "W0" port and connect it to the "E0" on wg2:
 wg3.connect("o1", wg2.ports["o2"])
 
 c
 
-# + vscode={"languageId": "python"}
+
 c.add_port(name="o1", port=wg1.ports["o1"])
 c.add_port(name="o2", port=wg3.ports["o2"])
 c
 # -
 
-# As you can see the `red` labels are for the component ports while
+# As you can see the `red` labels are for the cell ports while
 # `blue` labels are for the sub-ports (children ports)
 
 # ## Move and rotate references
 #
-# You can move, rotate, and reflect references to Components.
+# You can move, rotate, and reflect references to Cells.
+
 
-# + vscode={"languageId": "python"}
 c = kf.KCell()
 
 
 # Create and add a polygon from separate lists of x points and y points
 # e.g. [(x1, x2, x3, ...), (y1, y2, y3, ...)]
-c.shapes(c.klib.layer(4, 0)).insert(
+c.shapes(c.kcl.layer(4, 0)).insert(
     kf.kdb.DPolygon([kf.kdb.DPoint(x, y) for x, y in zip((8, 6, 7, 9), (6, 8, 9, 5))])
 )
 
 # Alternatively, create and add a polygon from a list of points
 # e.g. [(x1,y1), (x2,y2), (x3,y3), ...] using the same function
-c.shapes(c.klib.layer(4, 0)).insert(
+c.shapes(c.kcl.layer(4, 0)).insert(
     kf.kdb.DPolygon(
         [kf.kdb.DPoint(x, y) for (x, y) in ((0, 0), (1, 1), (1, 3), (-3, 3))]
     )
 )
 
 
 c
 # -
 
 # ## Ports
 #
-# Your straights wg1/wg2/wg3 are references to other waveguide components.
+# Your straights wg1/wg2/wg3 are references to other waveguide cells.
 #
-# If you want to add ports to the new Component `c` you can use `add_port`, where you can create a new port or use an reference an existing port from the underlying reference.
+# If you want to add ports to the new Cell `c` you can use `add_port`, where you can create a new port or use an reference an existing port from the underlying reference.
+
+# You can access the ports of a Cell or Instance
 
-# You can access the ports of a Component or ComponentReference
 
-# + vscode={"languageId": "python"}
 wg2.ports
 # -
 
 # ## References
 #
-# Now that we have your component `c` is a multi-straight component, you can add references to that component in a new blank Component `c2`, then add two references and shift one to see the movement.
+# Now that we have your cell `c` is a multi-straight cell, you can add references to that cell in a new blank Cell `c2`, then add two references and shift one to see the movement.
+
 
-# + vscode={"languageId": "python"}
 c2 = kf.KCell(name="MultiMultiWaveguide")
 wg1 = straight(layer=(2, 0))
 wg2 = straight(layer=(2, 0))
 mwg1_ref = c2.create_inst(wg1)
 mwg2_ref = c2.create_inst(wg2)
 mwg2_ref.transform(kf.kdb.DTrans(10, 10))
 c2
 
-# + vscode={"languageId": "python"}
 # Like before, let's connect mwg1 and mwg2 together
 mwg1_ref.connect("o2", mwg2_ref.ports["o1"])
+
 c2
 # -
 
 #
 #             self.layout_view.active_cellview().layout().cell(event["owner"].name)
 # ## Labels
 #
-# You can add abstract GDS labels (annotate) to your Components, in order to record information
+# You can add abstract GDS labels (annotate) to your Cells, in order to record information
 # directly into the final GDS file without putting any extra geometry onto any layer
 # This label will display in a GDS viewer, but will not be rendered or printed
-# like the polygons created by gf.components.text().
+# like the polygons created by gf.cells.text().
+
 
-# + vscode={"languageId": "python"}
-c2.shapes(c2.klib.layer(1, 0)).insert(kf.kdb.Text("First label", mwg1_ref.trans))
-# c2.shapes(c2.klib.layer(1,0).insert(kf.kdb.Text("First label", position=mwg1_ref.center)
-c2.shapes(c2.klib.layer(1, 0)).insert(kf.kdb.Text("Second label", mwg2_ref.trans))
+c2.shapes(c2.kcl.layer(1, 0)).insert(kf.kdb.Text("First label", mwg1_ref.trans))
+# c2.shapes(c2.kcl.layer(1,0).insert(kf.kdb.Text("First label", position=mwg1_ref.center)
+c2.shapes(c2.kcl.layer(1, 0)).insert(kf.kdb.Text("Second label", mwg2_ref.trans))
 # c2.add_label(text="Second label", position=mwg2_ref.center)
 
 # It's very useful for recording information about the devices or layout
-c2.shapes(c2.klib.layer(10, 0)).insert(
+c2.shapes(c2.kcl.layer(10, 0)).insert(
     kf.kdb.Text(
         f"The x size of this\nlayout is {c2.dbbox().width()}",
         kf.kdb.Trans(c2.bbox().right, c2.bbox().top),
     )
 )
 
 c2
@@ -274,97 +271,97 @@
 # perform an XOR on them, you can do that with the `boolean()` function.
 #
 #
 # The ``operation`` argument should be {not, and, or, xor, 'A-B', 'B-A', 'A+B'}.
 # Note that 'A+B' is equivalent to 'or', 'A-B' is equivalent to 'not', and
 # 'B-A' is equivalent to 'not' with the operands switched
 
-# + vscode={"languageId": "python"}
+
 e1 = kf.kdb.DPolygon.ellipse(kf.kdb.DBox(10, 8), 64)
 e2 = kf.kdb.DPolygon.ellipse(kf.kdb.DBox(10, 6), 64).transformed(
     kf.kdb.DTrans(2.0, 0.0)
 )
 # -
 
 c = kf.KCell()
-c.shapes(c.klib.layer(2, 0)).insert(e1)
-c.shapes(c.klib.layer(3, 0)).insert(e2)
+c.shapes(c.kcl.layer(2, 0)).insert(e1)
+c.shapes(c.kcl.layer(3, 0)).insert(e2)
 c
 
 # e1 NOT e2
 c = kf.KCell()
-e3 = kf.kdb.Region(e1.to_itype(c.klib.dbu)) - kf.kdb.Region(e2.to_itype(c.klib.dbu))
-c.shapes(c.klib.layer(1, 0)).insert(e3)
+e3 = kf.kdb.Region(e1.to_itype(c.kcl.dbu)) - kf.kdb.Region(e2.to_itype(c.kcl.dbu))
+c.shapes(c.kcl.layer(1, 0)).insert(e3)
 c
 
 # e1 AND e2
 c = kf.KCell()
-e3 = kf.kdb.Region(e1.to_itype(c.klib.dbu)) & kf.kdb.Region(e2.to_itype(c.klib.dbu))
-c.shapes(c.klib.layer(1, 0)).insert(e3)
+e3 = kf.kdb.Region(e1.to_itype(c.kcl.dbu)) & kf.kdb.Region(e2.to_itype(c.kcl.dbu))
+c.shapes(c.kcl.layer(1, 0)).insert(e3)
 c
 
 # e1 OR e2
 c = kf.KCell()
-e3 = kf.kdb.Region(e1.to_itype(c.klib.dbu)) + kf.kdb.Region(e2.to_itype(c.klib.dbu))
-c.shapes(c.klib.layer(1, 0)).insert(e3)
+e3 = kf.kdb.Region(e1.to_itype(c.kcl.dbu)) + kf.kdb.Region(e2.to_itype(c.kcl.dbu))
+c.shapes(c.kcl.layer(1, 0)).insert(e3)
 c
 
 # e1 OR e2 (merged)
 c = kf.KCell()
 e3 = (
-    kf.kdb.Region(e1.to_itype(c.klib.dbu)) + kf.kdb.Region(e2.to_itype(c.klib.dbu))
+    kf.kdb.Region(e1.to_itype(c.kcl.dbu)) + kf.kdb.Region(e2.to_itype(c.kcl.dbu))
 ).merge()
-c.shapes(c.klib.layer(1, 0)).insert(e3)
+c.shapes(c.kcl.layer(1, 0)).insert(e3)
 c
 
 # e1 XOR e2
 c = kf.KCell()
-e3 = kf.kdb.Region(e1.to_itype(c.klib.dbu)) ^ kf.kdb.Region(e2.to_itype(c.klib.dbu))
-c.shapes(c.klib.layer(1, 0)).insert(e3)
+e3 = kf.kdb.Region(e1.to_itype(c.kcl.dbu)) ^ kf.kdb.Region(e2.to_itype(c.kcl.dbu))
+c.shapes(c.kcl.layer(1, 0)).insert(e3)
 c
 
 # ## Move Reference by port
 
-# + vscode={"languageId": "python"}
+
 # MMI not implemented yet
 
 # c = kf.KCell()
-# mmi = c.add_ref(gf.components.mmi1x2())
-# bend = c.add_ref(gf.components.bend_circular(layer=(2, 0)))
+# mmi = c.add_ref(gf.cells.mmi1x2())
+# bend = c.add_ref(gf.cells.bend_circular(layer=(2, 0)))
 # c
 
-# + vscode={"languageId": "python"}
 # bend.connect("o1", mmi.ports["o2"])  # connects follow Source, destination syntax
+
 # c
 # -
 
 # ## Mirror reference
 #
 # By default the mirror works along the x=0 axis.
 
-# + vscode={"languageId": "python"}
-# c = gf.Component("ref_mirror")
-# mmi = c.add_ref(gf.components.mmi1x2())
-# bend = c.add_ref(gf.components.bend_circular(layer=(2, 0)))
+
+# c = gf.Cell("ref_mirror")
+# mmi = c.add_ref(gf.cells.mmi1x2())
+# bend = c.add_ref(gf.cells.bend_circular(layer=(2, 0)))
 # c
 
-# + vscode={"languageId": "python"}
+
 # mmi.mirror()
 # c
 # -
 
 # ## Write GDS
 #
 # [GDSII](https://en.wikipedia.org/wiki/GDSII) is the Standard format for exchanging CMOS and Photonic circuits.
 #
-# You can write your Component to GDS file.
+# You can write your Cell to GDS file.
+
 
-# + vscode={"languageId": "python"}
 c.write("demo.gds")
 # -
 
 # You can see the GDS file in Klayout viewer.
 #
 # Sometimes you also want to save the GDS together with metadata (settings, port names, widths, locations ...) in YAML
 
-# + vscode={"languageId": "python"}
+
 # c.write_gds_with_metadata("demo.gds") # not implemented, normal write writes metadata already
```

### Comparing `kfactory-0.6.3/docs/notebooks/01_references.py` & `kfactory-0.7.0/docs/notebooks/01_references.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 #     display_name: Python 3 (ipykernel)
 #     language: python
 #     name: python3
 # ---
 
 # # References and ports
 #
-# GDS allows your the component once in memory and Reference or Instance the component multiple times.
+# GDS allows your the cell once in memory and Reference or Instance the cell multiple times.
 #
 # `gdstk` and `gdspy` calls it `Reference` and `klayout` calls it `Instance`
 
-# As you build components you can include references to other components. Adding a reference is like having a pointer to a component.
+# As you build cells you can include references to other cells. Adding a reference is like having a pointer to a cell.
 #
 # The GDSII specification allows the use of references, and similarly kfactory uses them (with the `create_inst()` function).
 # what is an instance? Simply put:  **A reference does not contain any geometry. It only *points* to an existing geometry**.
 #
 # Say you have a ridiculously large polygon with 100 billion vertices that you call BigPolygon. It's huge, and you need to use it in your design 250 times.
 # Well, a single copy of BigPolygon takes up 1MB of memory, so you don't want to make 250 copies of it
 # You can instead *references* the polygon 250 times.
@@ -31,44 +31,44 @@
 # This way, you can keep one copy of BigPolygon and use it again and again.
 #
 # You can start by making a blank `KFactory` and add a single polygon to it.
 
 # +
 import kfactory as kf
 
-# Create a blank Component
+# Create a blank Cell
 p = kf.KCell()
 
 # Add a polygon
 xpts = [0, 0, 5, 6, 9, 12]
 ypts = [0, 1, 1, 2, 2, 0]
-p.shapes(p.klib.layer(2, 0)).insert(
+p.shapes(p.kcl.layer(2, 0)).insert(
     kf.kdb.DPolygon([kf.kdb.DPoint(x, y) for x, y in zip(xpts, ypts)])
 )
 
-# plot the Component with the polygon in it
+# plot the Cell with the polygon in it
 p
 # -
 
 # Now, you want to reuse this polygon repeatedly without creating multiple copies of it.
 #
-# To do so, you need to make a second blank `Component`, this time called `c`.
+# To do so, you need to make a second blank `Cell`, this time called `c`.
 #
-# In this new Component you *reference* our Component `p` which contains our polygon.
+# In this new Cell you *reference* our Cell `p` which contains our polygon.
 
-c = kf.KCell(name="Component_with_references")  # Create a new blank Component
-poly_ref = c.create_inst(p)  # Reference the Component "p" that has the polygon in it
+c = kf.KCell(name="Cell_with_references")  # Create a new blank Cell
+poly_ref = c.create_inst(p)  # Reference the Cell "p" that has the polygon in it
 c
 
 # you just made a copy of your polygon -- but remember, you didn't actually
 # make a second polygon, you just made a reference (aka pointer) to the original
 # polygon.  Let's add two more references to `c`:
 
-poly_ref2 = c.create_inst(p)  # Reference the Component "p" that has the polygon in it
-poly_ref3 = c.create_inst(p)  # Reference the Component "p" that has the polygon in it
+poly_ref2 = c.create_inst(p)  # Reference the Cell "p" that has the polygon in it
+poly_ref3 = c.create_inst(p)  # Reference the Cell "p" that has the polygon in it
 c
 
 # Now you have 3x polygons all on top of each other.  Again, this would appear
 # useless, except that you can manipulate each reference independently. Notice that
 # when you called `c.add_ref(p)` above, we saved the result to a new variable each
 # time (`poly_ref`, `poly_ref2`, and `poly_ref3`)?  You can use those variables to
 # reposition the references.
@@ -83,23 +83,23 @@
 
 # Now you're getting somewhere! You've only had to make the polygon once, but you're
 # able to reuse it as many times as you want.
 #
 # ## Modifying the referenced geometry
 #
 # What happens when you change the original geometry that the reference points to?  In your case, your references in
-# `c` all point to the Component `p` that with the original polygon.  Let's try
+# `c` all point to the Cell `p` that with the original polygon.  Let's try
 # adding a second polygon to `p`.
 #
 # First you add the second polygon and make sure `P` looks like you expect:
 
 # Add a 2nd polygon to "p"
 xpts = [14, 14, 16, 16]
 ypts = [0, 2, 2, 0]
-p.shapes(p.klib.layer(1, 0)).insert(
+p.shapes(p.kcl.layer(1, 0)).insert(
     kf.kdb.DPolygon([kf.kdb.DPoint(x, y) for x, y in zip(xpts, ypts)])
 )
 p
 
 # That looks good.  Now let's find out what happened to `c` that contains the
 # three references.  Keep in mind that you have not modified `c` or executed any
 # functions/operations on `c` -- all you have done is modify `p`.
@@ -112,46 +112,46 @@
 # elements in a computation- and memory-efficient way.
 #
 # Let's try making references a level deeper by referencing `c`.  Note here we use
 # the `<<` operator to add the references -- this is just shorthand, and is
 # exactly equivalent to using `add_ref()`
 
 # +
-c2 = kf.KCell(name="array_sample")  # Create a new blank Component
-d_ref1 = c2.create_inst(c)  # Reference the Component "c" that 3 references in it
+c2 = kf.KCell(name="array_sample")  # Create a new blank Cell
+d_ref1 = c2.create_inst(c)  # Reference the Cell "c" that 3 references in it
 d_ref2 = c2 << c  # Use the "<<" operator to create a 2nd reference to c
 d_ref3 = c2 << c  # Use the "<<" operator to create a 3rd reference to c
 
 d_ref1.transform(kf.kdb.DTrans(20.0, 0.0))
 d_ref2.transform(kf.kdb.DTrans(40.0, 0.0))
 
 c2
 # -
 
-# As you've seen you have two ways to add a reference to our component:
+# As you've seen you have two ways to add a reference to our cell:
 #
-# 1. create the reference and add it to the component
+# 1. create the reference and add it to the cell
 
 c = kf.KCell(name="reference_sample")
-w = kf.pcells.waveguide.waveguide(length=10, width=0.6, layer=c.klib.layer(1, 0))
+w = kf.cells.waveguide.waveguide(length=10, width=0.6, layer=c.kcl.layer(1, 0))
 wr = kf.kdb.CellInstArray(w._kdb_cell, kf.kdb.Trans.R0)
 c.insert(wr)
 c
 
 # 2. or do it in a single line
 
 c = kf.KCell(name="reference_sample_shorter_syntax")
-wr = c << kf.pcells.waveguide.waveguide(length=10, width=0.6, layer=c.klib.layer(1, 0))
+wr = c << kf.cells.waveguide.waveguide(length=10, width=0.6, layer=c.kcl.layer(1, 0))
 c
 
 # in both cases you can move the reference `wr` after created
 
 c = kf.KCell(name="two_references")
-wr1 = c << kf.pcells.waveguide.waveguide(length=10, width=0.6, layer=c.klib.layer(1, 0))
-wr2 = c << kf.pcells.waveguide.waveguide(length=10, width=0.6, layer=c.klib.layer(1, 0))
+wr1 = c << kf.cells.waveguide.waveguide(length=10, width=0.6, layer=c.kcl.layer(1, 0))
+wr2 = c << kf.cells.waveguide.waveguide(length=10, width=0.6, layer=c.kcl.layer(1, 0))
 wr2.transform(kf.kdb.DTrans(0.0, 10.0))
 c.add_ports(wr1.ports, prefix="top_")
 c.add_ports(wr2.ports, prefix="bot_")
 
 c.ports
 
 # You can also auto_rename ports using gdsfactory default convention, where ports are numbered clockwise starting from the bottom left
@@ -160,56 +160,56 @@
 
 c.ports
 
 c
 
 # ## Arrays of references
 #
-# In GDS, there's a type of structure called a "ComponentReference" which takes a cell and repeats it NxM times on a fixed grid spacing. For convenience, `Component` includes this functionality with the add_array() function.
+# In GDS, there's a type of structure called a "Instance" which takes a cell and repeats it NxM times on a fixed grid spacing. For convenience, `Cell` includes this functionality with the add_array() function.
 # Note that CellArrays are not compatible with ports (since there is no way to access/modify individual elements in a GDS cellarray)
 #
 # gdsfactory also provides with more flexible arrangement options if desired, see for example `grid()` and `packer()`.
 #
-# As well as `gf.components.array`
+# As well as `gf.cells.array`
 #
-# Let's make a new Component and put a big array of our Component `c` in it:
+# Let's make a new Cell and put a big array of our Cell `c` in it:
 
 # +
 # not converted yet
 
-c3 = kf.KCell("array_of_references")  # Create a new blank Component
+c3 = kf.KCell("array_of_references")  # Create a new blank Cell
 aref = c3.create_inst(
     c, na=6, nb=3, a=kf.kdb.Vector(20000, 0), b=kf.kdb.Vector(0, 15000)
-)  # Reference the Component "c" 3 references in it with a 3 rows, 6 columns array
+)  # Reference the Cell "c" 3 references in it with a 3 rows, 6 columns array
 c3
 # -
 
 # CellArrays don't have ports and there is no way to access/modify individual elements in a GDS cellarray.
 #
-# gdsfactory provides you with similar functions in `gf.components.array` and `gf.components.array_2d`
+# gdsfactory provides you with similar functions in `gf.cells.array` and `gf.cells.array_2d`
 
 # +
-# c4 = gf.Component("demo_array")  # Create a new blank Component
-# aref = c4 << gf.components.array(component=c, columns=3, rows=2)
+# c4 = gf.Cell("demo_array")  # Create a new blank Cell
+# aref = c4 << gf.cells.array(cell=c, columns=3, rows=2)
 # c4.add_ports(aref.get_ports_list())
 # c4
 
 
 # +
-# # gf.components.array?
+# # gf.cells.array?
 # -
 
-# You can also create an array of references for periodic structures. Lets create a [Distributed Bragg Reflector](https://picwriter.readthedocs.io/en/latest/components/dbr.html)
+# You can also create an array of references for periodic structures. Lets create a [Distributed Bragg Reflector](https://picwriter.readthedocs.io/en/latest/cells/dbr.html)
 
 
 # +
 # @gf.cell
-# def dbr_period(w1=0.5, w2=0.6, l1=0.2, l2=0.4, straight=gf.components.straight):
+# def dbr_period(w1=0.5, w2=0.6, l1=0.2, l2=0.4, straight=gf.cells.straight):
 #     """Return one DBR period."""
-#     c = gf.Component()
+#     c = gf.Cell()
 #     r1 = c << straight(length=l1, width=w1)
 #     r2 = c << straight(length=l2, width=w2)
 #     r2.connect(port="o1", destination=r1.ports["o2"])
 #     c.add_port("o1", port=r1.ports["o1"])
 #     c.add_port("o2", port=r2.ports["o2"])
 #     return c
 
@@ -217,57 +217,57 @@
 # l1 = 0.2
 # l2 = 0.4
 # n = 3
 # period = dbr_period(l1=l1, l2=l2)
 # period
 
 # +
-# dbr = gf.Component("DBR")
+# dbr = gf.Cell("DBR")
 # dbr.add_array(period, columns=n, rows=1, spacing=(l1 + l2, 100))
 # dbr
 # -
 
-# Finally we need to add ports to the new component
+# Finally we need to add ports to the new cell
 
 # +
 # p0 = dbr.add_port("o1", port=period.ports["o1"])
 # p1 = dbr.add_port("o2", port=period.ports["o2"])
 
 # p1.center = [(l1 + l2) * n, 0]
 # dbr
 # -
 
-# ## Connect references
+# ## connect references
 #
 # We have seen that once you create a reference you can manipulate the reference to move it to a location. Here we are going to connect that reference to a port. Remember that we follow that a certain reference `source` connects to a `destination` port
 
 # +
-# bend = gf.components.bend_circular()
+# bend = gf.cells.bend_circular()
 # bend
 
 # +
-# c = gf.Component("sample_reference_connect")
+# c = gf.Cell("sample_reference_connect")
 
-# mmi = c << gf.components.mmi1x2()
-# b = c << gf.components.bend_circular()
+# mmi = c << gf.cells.mmi1x2()
+# b = c << gf.cells.bend_circular()
 # b.connect("o1", destination=mmi.ports["o2"])
 
 # c.add_port("o1", port=mmi.ports["o1"])
 # c.add_port("o2", port=b.ports["o2"])
 # c.add_port("o3", port=mmi.ports["o3"])
 # c
 # -
 
 # You can also access the ports directly from the references
 
 # +
-# c = gf.Component("sample_reference_connect_simpler")
+# c = gf.Cell("sample_reference_connect_simpler")
 
-# mmi = c << gf.components.mmi1x2()
-# b = c << gf.components.bend_circular()
+# mmi = c << gf.cells.mmi1x2()
+# b = c << gf.cells.bend_circular()
 # b.connect("o1", destination=mmi["o2"])
 
 # c.add_port("o1", port=mmi["o1"])
 # c.add_port("o2", port=b["o2"])
 # c.add_port("o3", port=mmi["o3"])
 # c
 # -
@@ -285,19 +285,19 @@
 # The port naming comes in most cases from the `gdsfactory.cross_section`. For example
 #
 # - `gdsfactory.cross_section.strip`  has ports `o1` for input and `o2` for output
 # - `gdsfactory.cross_section.metal1` has ports `e1` for input and `e2` for output
 
 # +
 # size = 4
-# c = gf.components.nxn(west=2, south=2, north=2, east=2, xsize=size, ysize=size)
+# c = gf.cells.nxn(west=2, south=2, north=2, east=2, xsize=size, ysize=size)
 # c
 
 # +
-# c = gf.components.straight_heater_metal(length=30)
+# c = gf.cells.straight_heater_metal(length=30)
 # c
 
 # +
 # c.ports
 # -
 
 # You can get the optical ports by `layer`
@@ -308,15 +308,15 @@
 
 # or by `width`
 
 # +
 # c.get_ports_dict(width=0.5)
 
 # +
-# c0 = gf.components.straight_heater_metal()
+# c0 = gf.cells.straight_heater_metal()
 # c0.ports
 
 # +
 # c1 = c0.copy()
 # c1.auto_rename_ports_layer_orientation()
 # c1.ports
 
@@ -344,16 +344,16 @@
 #          1 -|______|- 6
 #              |   |
 #              8   7
 #
 # ```
 
 # +
-# c = gf.Component("demo_ports")
-# nxn = gf.components.nxn(west=2, north=2, east=2, south=2, xsize=4, ysize=4)
+# c = gf.Cell("demo_ports")
+# nxn = gf.cells.nxn(west=2, north=2, east=2, south=2, xsize=4, ysize=4)
 # ref = c.add_ref(nxn)
 # c.add_ports(ref.ports)
 # c
 
 # +
 # ref.get_ports_list()  # by default returns ports clockwise starting from bottom left west facing port
 
@@ -393,18 +393,18 @@
 # -
 
 # Lets extend the East facing ports (orientation = 0 deg)
 
 # +
 # cross_section = gf.cross_section.strip()
 
-# nxn = gf.components.nxn(
+# nxn = gf.cells.nxn(
 #     west=2, north=2, east=2, south=2, xsize=4, ysize=4, cross_section=cross_section
 # )
-# c = gf.components.extension.extend_ports(component=nxn, orientation=0)
+# c = gf.cells.extension.extend_ports(cell=nxn, orientation=0)
 # c
 
 # +
 # c.ports
 
 # +
 # df = c.get_ports_pandas()
@@ -414,52 +414,52 @@
 # df[df.port_type == "optical"]
 # -
 
 # ## pins
 #
 # You can add pins (port markers) to each port. Each foundry PDK does this differently, so gdsfactory supports all of them.
 #
-# - square with port inside the component
-# - square centered (half inside, half outside component)
+# - square with port inside the cell
+# - square centered (half inside, half outside cell)
 # - triangular
 # - path (SiEPIC)
 #
 #
-# by default Component.show() will add triangular pins, so you can see the direction of the port in Klayout.
+# by default Cell.show() will add triangular pins, so you can see the direction of the port in Klayout.
 
 # +
-# gf.components.mmi1x2(decorator=gf.add_pins.add_pins)
+# gf.cells.mmi1x2(decorator=gf.add_pins.add_pins)
 
 # +
-# gf.components.mmi1x2(decorator=gf.add_pins.add_pins_triangle)
+# gf.cells.mmi1x2(decorator=gf.add_pins.add_pins_triangle)
 # -
 
-# ## component_sequence
+# ## cell_sequence
 #
 # When you have repetitive connections you can describe the connectivity as an ASCII map
 
 # +
-# bend180 = gf.components.bend_circular180()
-# wg_pin = gf.components.straight_pin(length=40)
-# wg = gf.components.straight()
+# bend180 = gf.cells.bend_circular180()
+# wg_pin = gf.cells.straight_pin(length=40)
+# wg = gf.cells.straight()
 
-# # Define a map between symbols and (component, input port, output port)
-# symbol_to_component = {
+# # Define a map between symbols and (cell, input port, output port)
+# symbol_to_cell = {
 #     "D": (bend180, "o1", "o2"),
 #     "C": (bend180, "o2", "o1"),
 #     "P": (wg_pin, "o1", "o2"),
 #     "-": (wg, "o1", "o2"),
 # }
 
 # # Generate a sequence
-# # This is simply a chain of characters. Each of them represents a component
+# # This is simply a connect of characters. Each of them represents a cell
 # # with a given input and and a given output
 
 # sequence = "DC-P-P-P-P-CD"
-# component = gf.components.component_sequence(
-#     sequence=sequence, symbol_to_component=symbol_to_component
+# cell = gf.cells.cell_sequence(
+#     sequence=sequence, symbol_to_cell=symbol_to_cell
 # )
-# component.name = "component_sequence"
-# component
+# cell.name = "cell_sequence"
+# cell
 # -
 
 # As the sequence is defined as a string you can use the string operations to easily build complex sequences
```

### Comparing `kfactory-0.6.3/docs/notebooks/02_DRC.py` & `kfactory-0.7.0/docs/notebooks/02_DRC.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     [kf.kdb.DPoint(0, 10), kf.kdb.DPoint(30, 10), kf.kdb.DPoint(30, 0)]
 )
 triangle.shapes(triangle.layer(1, 0)).insert(triangle_poly)
 triangle
 
 box = kf.KCell("Box")
 box_rect = kf.kdb.DBox(0, 0, 20, 5)
-box.shapes(box.klib.layer(1, 0)).insert(box_rect)
+box.shapes(box.kcl.layer(1, 0)).insert(box_rect)
 box
 
 c = kf.KCell("fix_accute_angle")
 c << triangle
 c << box
 c
 
@@ -33,30 +33,30 @@
 d1 = datetime.now()
 
 for i in range(50):
     ellipse = kf.kdb.Polygon.ellipse(kf.kdb.Box(10000, 20000), i * 2)
 
     x0 = 0
     for j in range(5000, 30000, 500):
-        c.shapes(c.klib.layer(1, 0)).insert(
+        c.shapes(c.kcl.layer(1, 0)).insert(
             ellipse.transformed(kf.kdb.Trans(x0, i * 30000))
         )
-        c.shapes(c.klib.layer(1, 0)).insert(
+        c.shapes(c.kcl.layer(1, 0)).insert(
             ellipse.transformed(kf.kdb.Trans(x0 + j, i * 30000))
         )
 
         x0 += 15000
 
 d2 = datetime.now()
 
-c.shapes(c.klib.layer(2, 0)).insert(
+c.shapes(c.kcl.layer(2, 0)).insert(
     kf.utils.fix_spacing_tiled(
         c,
         1000,
-        c.klib.layer(1, 0),
+        c.kcl.layer(1, 0),
         metrics=kf.kdb.Metrics.Euclidian,
         n_threads=32,
         tile_size=(250, 250),
     )
 )
 
 d3 = datetime.now()
@@ -74,30 +74,30 @@
 d1 = datetime.now()
 
 for i in range(50):
     ellipse = kf.kdb.Polygon.ellipse(kf.kdb.Box(10000, 20000), i * 2)
 
     x0 = 0
     for j in range(5000, 30000, 500):
-        c.shapes(c.klib.layer(1, 0)).insert(
+        c.shapes(c.kcl.layer(1, 0)).insert(
             ellipse.transformed(kf.kdb.Trans(x0, i * 30000))
         )
-        c.shapes(c.klib.layer(1, 0)).insert(
+        c.shapes(c.kcl.layer(1, 0)).insert(
             ellipse.transformed(kf.kdb.Trans(x0 + j, i * 30000))
         )
 
         x0 += 15000
 
 d2 = datetime.now()
 
-c.shapes(c.klib.layer(2, 0)).insert(
+c.shapes(c.kcl.layer(2, 0)).insert(
     kf.utils.fix_spacing_minkowski_tiled(
         c,
         1000,
-        c.klib.layer(1, 0),
+        c.kcl.layer(1, 0),
         n_threads=32,
         tile_size=(250, 250),
         smooth=5,
     )
 )
 
 d3 = datetime.now()
@@ -106,39 +106,39 @@
 print(f"time to clean: {d3-d2}")
 print(f"total time: {d3-d1}")
 
 c
 # -
 
 c = kf.KCell("ToFill")
-c.shapes(kf.klib.layer(1, 0)).insert(
+c.shapes(kf.kcl.layer(1, 0)).insert(
     kf.kdb.DPolygon.ellipse(kf.kdb.DBox(5000, 3000), 512)
 )
-c.shapes(kf.klib.layer(10, 0)).insert(
+c.shapes(kf.kcl.layer(10, 0)).insert(
     kf.kdb.DPolygon(
         [kf.kdb.DPoint(0, 0), kf.kdb.DPoint(5000, 0), kf.kdb.DPoint(5000, 3000)]
     )
 )
 c
 
 fc = kf.KCell("fill")
-fc.shapes(fc.klib.layer(2, 0)).insert(kf.kdb.DBox(20, 40))
-fc.shapes(fc.klib.layer(3, 0)).insert(kf.kdb.DBox(30, 15))
+fc.shapes(fc.kcl.layer(2, 0)).insert(kf.kdb.DBox(20, 40))
+fc.shapes(fc.kcl.layer(3, 0)).insert(kf.kdb.DBox(30, 15))
 fc
 
 import kfactory.utils.fill as fill
 
-# fill.fill_tiled(c, fc, [(kf.klib.layer(1,0), 0)], exclude_layers = [(kf.klib.layer(10,0), 100), (kf.klib.layer(2,0), 0), (kf.klib.layer(3,0),0)], x_space=5, y_space=5)
+# fill.fill_tiled(c, fc, [(kf.kcl.layer(1,0), 0)], exclude_layers = [(kf.kcl.layer(10,0), 100), (kf.kcl.layer(2,0), 0), (kf.kcl.layer(3,0),0)], x_space=5, y_space=5)
 fill.fill_tiled(
     c,
     fc,
-    [(kf.klib.layer(1, 0), 0)],
+    [(kf.kcl.layer(1, 0), 0)],
     exclude_layers=[
-        (kf.klib.layer(10, 0), 100),
-        (kf.klib.layer(2, 0), 0),
-        (kf.klib.layer(3, 0), 0),
+        (kf.kcl.layer(10, 0), 100),
+        (kf.kcl.layer(2, 0), 0),
+        (kf.kcl.layer(3, 0), 0),
     ],
     x_space=5,
     y_space=5,
 )
 
 c
```

### Comparing `kfactory-0.6.3/docs/notebooks/03_Enclosures.py` & `kfactory-0.7.0/docs/notebooks/03_Enclosures.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,133 +4,129 @@
 class LAYER(kf.LayerEnum):
     WG = (1, 0)
     WGEX = (2, 0)
     SLAB = (3, 0)
     SLABEX = (4, 0)
 
 
-enc = kf.utils.Enclosure(
+enc = kf.utils.LayerEnclosure(
     [
         (LAYER.WGEX, 5000),
         (LAYER.SLAB, 5000, 50000),
         (LAYER.SLAB, 55000, 95000),
         (LAYER.SLABEX, 110000),
     ],
     name="WGSLAB",
     main_layer=LAYER.WG,
 )
 
 
-@kf.autocell
+@kf.cell
 def rectangles(
     radius: int,
     width: int,
     pitch: int,
     n: int,
     l_straight: int,
     layer: kf.LayerEnum,
-    enclosure: kf.utils.Enclosure,
+    enclosure: kf.utils.LayerEnclosure,
 ) -> kf.KCell:
     """Rectangles with eulerbends as corners."""
     c = kf.KCell()
-    bend = kf.pcells.euler.bend_euler(
-        width=int(width * c.klib.dbu), radius=int(c.klib.dbu * radius), layer=layer
+    bend = kf.cells.euler.bend_euler(
+        width=int(width * c.kcl.dbu), radius=int(c.kcl.dbu * radius), layer=layer
     )
 
     def wg_f(length: int) -> kf.KCell:
-        return kf.pcells.waveguide.waveguide_dbu(
-            width=width, length=length, layer=layer
-        )
+        return kf.cells.waveguide.waveguide_dbu(width=width, length=length, layer=layer)
 
     for i in range(n):
         b1, b2, b3, b4 = (c << bend for _ in range(4))
         b1.transform(kf.kdb.Trans(i * pitch, -i * pitch))
         v = 2 * i * pitch
         if v:
             wg_v = wg_f(v)
             wg1 = c << wg_v
-            wg1.align("o1", b1, "o2")
-            b2.align("o1", wg1, "o2")
+            wg1.connect("o1", b1, "o2")
+            b2.connect("o1", wg1, "o2")
         else:
-            b2.align("o1", b1, "o2")
+            b2.connect("o1", b1, "o2")
         _l_straight = l_straight + 2 * i * pitch
         if _l_straight:
             wg_h = wg_f(_l_straight)
             wg2 = c << wg_h
-            wg2.align("o1", b2, "o2")
-            b3.align("o1", wg2, "o2")
+            wg2.connect("o1", b2, "o2")
+            b3.connect("o1", wg2, "o2")
         else:
-            b3.align("o1", b2, "o2")
+            b3.connect("o1", b2, "o2")
         if v:
             wg3 = c << wg_v
-            wg3.align("o1", b3, "o2")
-            b4.align("o1", wg3, "o2")
+            wg3.connect("o1", b3, "o2")
+            b4.connect("o1", wg3, "o2")
         else:
-            b4.align("o1", b3, "o2")
+            b4.connect("o1", b3, "o2")
         if _l_straight:
             wg4 = c << wg_h
-            wg4.align("o1", b4, "o2")
+            wg4.connect("o1", b4, "o2")
 
     def shape(d: int) -> kf.kdb.Polygon:
         return kf.kdb.Polygon.ellipse(kf.kdb.Box(2 * d, 2 * d), 64)
 
     enclosure.apply_minkowski_custom(c=c, shape=shape, ref=layer)
 
     return c
 
 
-@kf.autocell
+@kf.cell
 def rectangles_tiled(
     radius: int,
     width: int,
     pitch: int,
     n: int,
     l_straight: int,
     layer: kf.LayerEnum,
-    enclosure: kf.utils.Enclosure,
+    enclosure: kf.utils.LayerEnclosure,
 ) -> kf.KCell:
     """Rectangles with eulerbends as corners."""
     c = kf.KCell()
-    bend = kf.pcells.euler.bend_euler(
-        width=int(width * c.klib.dbu), radius=int(c.klib.dbu * radius), layer=layer
+    bend = kf.cells.euler.bend_euler(
+        width=int(width * c.kcl.dbu), radius=int(c.kcl.dbu * radius), layer=layer
     )
 
     def wg_f(length: int) -> kf.KCell:
-        return kf.pcells.waveguide.waveguide_dbu(
-            width=width, length=length, layer=layer
-        )
+        return kf.cells.waveguide.waveguide_dbu(width=width, length=length, layer=layer)
 
     for i in range(n):
         b1, b2, b3, b4 = (c << bend for _ in range(4))
         b1.transform(kf.kdb.Trans(i * pitch, -i * pitch))
         v = 2 * i * pitch
         if v:
             wg_v = wg_f(v)
             wg1 = c << wg_v
-            wg1.align("o1", b1, "o2")
-            b2.align("o1", wg1, "o2")
+            wg1.connect("o1", b1, "o2")
+            b2.connect("o1", wg1, "o2")
         else:
-            b2.align("o1", b1, "o2")
+            b2.connect("o1", b1, "o2")
         _l_straight = l_straight + 2 * i * pitch
         if _l_straight:
             wg_h = wg_f(_l_straight)
             wg2 = c << wg_h
-            wg2.align("o1", b2, "o2")
-            b3.align("o1", wg2, "o2")
+            wg2.connect("o1", b2, "o2")
+            b3.connect("o1", wg2, "o2")
         else:
-            b3.align("o1", b2, "o2")
+            b3.connect("o1", b2, "o2")
         if v:
             wg3 = c << wg_v
-            wg3.align("o1", b3, "o2")
-            b4.align("o1", wg3, "o2")
+            wg3.connect("o1", b3, "o2")
+            b4.connect("o1", wg3, "o2")
         else:
-            b4.align("o1", b3, "o2")
+            b4.connect("o1", b3, "o2")
         if _l_straight:
             wg4 = c << wg_h
-            wg4.align("o1", b4, "o2")
+            wg4.connect("o1", b4, "o2")
 
     def shape(d: int) -> kf.kdb.Polygon:
         return kf.kdb.Polygon.ellipse(kf.kdb.Box(2 * d, 2 * d), 64)
 
     enclosure.apply_minkowski_tiled(c=c, ref=layer, n_pts=64)
 
     return c
```

### Comparing `kfactory-0.6.3/docs/star.py` & `kfactory-0.7.0/docs/star.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import kfactory as kf
 import numpy as np
 from layers import LAYER
 import random
 
 
-@kf.autocell
+@kf.cell
 def star(
     size: float, proportion: float, n_diamonds: int = 3, layer: kf.LayerEnum = LAYER.SI
 ) -> kf.KCell:
     """Create a diamond star cell
 
     Args:
         size: size in um
@@ -40,15 +40,15 @@
         c.shapes(layer).insert(
             diamond.transformed(kf.kdb.DCplxTrans(1, angle, False, 0, 0))
         )
 
     return c
 
 
-@kf.autocell
+@kf.cell
 def merged_star(
     size: float, proportion: float, n_diamonds: int = 3, layer: kf.LayerEnum = LAYER.SI
 ) -> kf.KCell:
     """Same as star but use the star shapes and merge them to one polygon"""
 
     c = kf.KCell()
 
@@ -59,15 +59,15 @@
     # Insert the region
 
     c.shapes(layer).insert(reg)
 
     return c
 
 
-@kf.autocell
+@kf.cell
 def sky_with_stars() -> kf.KCell:
     c = kf.KCell()
 
     box = kf.kdb.Box(0, 0, 400000, 400000)  # 400umx400um sky (default dbu)
     sky = kf.kdb.Region(box)
 
     # set a custom seed for random
@@ -83,15 +83,15 @@
         angle = random.uniform(0, 360)
         _star = c << merged_star(
             size=random.uniform(5, 25),
             proportion=random.uniform(0.2, 0.3),
             n_diamonds=random.randint(2, 5),
             layer=star_layer,
         )
-        _star.transform(kf.kdb.DCplxTrans(1, angle, False, x, y))
+        _star.transform(kf.kdb.DTrans(angle, False, x, y))
 
     # remove the stars from the sky
 
     sky -= kf.kdb.Region(c.begin_shapes_rec(star_layer))
 
     c.shapes(LAYER.SIEXCLUDE).insert(sky)
```

### Comparing `kfactory-0.6.3/docs/waveguide.py` & `kfactory-0.7.0/docs/waveguide.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from layers import LAYER
 
 import kfactory as kf
 
 
-@kf.autocell
+@kf.cell
 def waveguide(width: int, length: int, width_exclude: int) -> kf.KCell:
     """Waveguide: Silicon on 1/0, Silicon exclude on 1/1"""
     c = kf.KCell()
     c.shapes(LAYER.SI).insert(kf.kdb.Box(0, -width // 2, length, width // 2))
     c.shapes(LAYER.SIEXCLUDE).insert(
         kf.kdb.Box(0, -width_exclude // 2, length, width_exclude // 2)
     )
```

### Comparing `kfactory-0.6.3/pyproject.toml` & `kfactory-0.7.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -9,65 +9,63 @@
 classifiers = [
 	"Programming Language :: Python :: 3.10",
 	"Operating System :: OS Independent",
 ]
 requires-python = ">=3.10"
 
 
-version = "0.6.3"
+version = "0.7.0"
 authors = [
     {name = "gdsfactory community", email = "contact@gdsfactory.com"},
 ]
 dependencies = [
 	"klayout >= 0.28.3",
 	"scipy",
 	"ruamel.yaml",
 	"cachetools >= 5.2.0",
   "pydantic",
 	"loguru",
 	"tomli",
 ]
 
 [project.optional-dependencies]
+git = [
+	"gitpython",
+]
 dev = [
 	"black>=23",
 	"mypy",
 	"pre-commit",
 	"gitpython",
 	"pylsp-mypy",
 	"python-lsp-server[all]",
 	"python-lsp-ruff",
 	"types-cachetools",
 	"python-lsp-black",
+	"kfactory[git]",
 ]
 docs = [
-	"sphinx",
-	"docutils==0.17.1",
-	"sphinx_rtd_theme",
-	"sphinxcontrib-video",
-	"sphinx-autodoc-typehints",
-	"sphinx-book-theme>=0.3.3",
-	"sphinx-click",
-	"sphinx-copybutton",
-	"sphinx-markdown-tables",
-	"myst-parser",
-	"matplotlib",
-	"nbsphinx",
-	"autodoc_pydantic",
-	"jupytext",
-	"jupyter",
 	"kfactory[ipy]",
+  "mkdocs",
+	"mkdocs-jupyter>=0.24",
+  "mkdocstrings[python]",
+  "mkdocs-material",
+  "mkdocs_gen_files",
+	"mkdocs-literate-nav",
+	"mkdocs-section-index",
+	"mkdocs-video",
 ]
 ci = [
 	"flake8",
 	"flake8-pyproject",
 	"pytest",
 	"pytest_regressions",
 	"mypy",
 	"types-cachetools",
+	"kfactory[git]",
 ]
 ipy = [
 	"ipython",
 	"ipywidgets",
 	"ipytree",
 	"ipyevents",
 ]
@@ -97,16 +95,19 @@
 '''
 
 [tool.mypy]
 python_version = "3.10"
 strict = true
 exclude = [
 	"tests",
-	"src/kfactory/widgets",
+	"src/kfactory/widgets/interactive.py",
+	"src/kfactory/technology",
+	"src/kfactory/pdk.py",
 ]
+plugins = "pydantic.mypy"
 
 [tool.pylsp-mypy]
 enabled = true
 live_mode = true
 strict = true
 
 [[tool.mypy.overrides]]
```

### Comparing `kfactory-0.6.3/src/kfactory/__init__.py` & `kfactory-0.7.0/src/kfactory/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,44 +10,44 @@
 import klayout.dbcore as kdb
 import klayout.lay as lay
 from .kcell import (
     KCell,
     Instance,
     Port,
     Ports,
-    autocell,
     cell,
-    klib,
-    KLib,
+    kcl,
+    KCLayout,
     default_save,
     LayerEnum,
     show,
 )
-from . import pcells, placer, routing, utils, port
-from .config import logger
+from . import cells, placer, routing, utils, port, pdk
+from .conf import config
+from .pdk import Pdk
 
+__version__ = "0.7.0"
 
-__version__ = "0.6.3"
-
+logger = config.logger
 
 __all__ = [
     "KCell",
     "Instance",
     "Port",
     "Ports",
-    "autocell",
     "cell",
-    "klib",
-    "KLib",
+    "kcl",
+    "KCLayout",
     "default_save",
     "kdb",
     "lay",
     "port",
-    "pcells",
+    "cells",
     "placer",
     "routing",
     "utils",
     "show",
-    "klay",
-    "logger",
+    "config",
     "LayerEnum",
+    "logger",
+    "pdk",
 ]
```

### Comparing `kfactory-0.6.3/src/kfactory/config.py` & `kfactory-0.7.0/src/kfactory/conf.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 """Kfactory configuration."""
 
 from __future__ import annotations
 
+import os
 import re
 import sys
 import traceback
 from itertools import takewhile
+from typing import TYPE_CHECKING, Any, ClassVar, Literal
 
 import loguru
 from loguru import logger as logger
+from pydantic import BaseModel, BaseSettings, Field
+
+if TYPE_CHECKING:
+    from loguru import Logger
 
 
 def add_traceback(record: loguru.Record) -> None:
     """Add a traceback to the logger."""
     extra = record["extra"]
     if extra.get("with_traceback", False):
         extra["traceback"] = "\n" + "".join(traceback.format_stack())
@@ -41,40 +47,74 @@
         return (
             "<green>{time:YYYY-MM-DD HH:mm:ss.SSS}</green> | <level>{level: <8}"
             "</level> | <cyan>{name}</cyan>:<cyan>{function}</cyan>:<cyan>{line}</cyan>"
             " - <level>{message}</level>\n{exception}"
         )
 
 
-class LogFilter:
+class LogFilter(BaseModel):
     """Filter certain messages by log level or regex.
 
     Filtered messages are not evaluated and discarded.
     """
 
-    def __init__(self, level: str, regex: str | None = None) -> None:
-        """Create new filter.
-
-        Args:
-            level: Minimum log level to print to log. Options:
-                ["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"]
-            regex: Discard messages matching the regex string. Set to `None` to disable.
-        """
-        self.level = level
-        self.regex = regex
+    level: Literal[
+        "TRACE", "DEBUG", "INFO", "SUCCESS", "WARNING", "ERROR", "CRITICAL"
+    ] = "INFO"
+    regex: str | None = None
 
     def __call__(self, record: loguru.Record) -> bool:
         """Loguru needs the filter to be callable."""
         levelno = logger.level(self.level).no
         if self.regex is None:
             return record["level"].no >= levelno
         else:
             return record["level"].no >= levelno and not bool(
                 re.search(self.regex, record["message"])
             )
 
 
-filter = LogFilter("DEBUG")
-logger.remove()
-logger.add(sys.stdout, format=tracing_formatter, filter=filter)
+def get_affinity() -> int:
+    """Get number of cores/threads available.
+
+    On (most) linux we can get it through the scheduling affinity. Otherwise,
+    fall back to the multiprocessing cpu count.
+    """
+    try:
+        threads = len(os.sched_getaffinity(0))
+    except AttributeError:
+        import multiprocessing
+
+        threads = multiprocessing.cpu_count()
+    finally:
+        return threads
+
+
+class Settings(BaseSettings):
+    """KFactory settings object."""
+
+    n_threads: int = get_affinity()
+    logger: ClassVar[Logger] = logger
+    logfilter: LogFilter = Field(default_factory=LogFilter)
+    display_type: Literal["widget", "image", "docs"] = "widget"
+
+    def __init__(self, **data: Any):
+        """Set log filter and run pydantic."""
+        super().__init__(**data)
+        self.logger.remove()
+        self.logger.add(sys.stdout, format=tracing_formatter, filter=self.logfilter)
+        self.logger.info("LogLevel: {}", self.logfilter.level)
+
+    class Config:
+        """Pydantic settings."""
+
+        validation = False
+        arbitrary_types_allowed = True
+        fields = {"logger": {"exclude": True}}
+        env_prefix = "kfactory_"
+        env_nested_delimiter = "_"
+
+
+config = Settings()
+
 
-__all__ = ["logger", "filter"]
+__all__ = ["config"]
```

### Comparing `kfactory-0.6.3/src/kfactory/kcell.py` & `kfactory-0.7.0/src/kfactory/kcell.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,64 +1,86 @@
 """Core module of kfactory.
 
-Defines the :py:class:`KCell` providing klayout Cells with Ports
+Defines the [KCell][kfactory.kcell.KCell] providing klayout Cells with Ports
 and other convenience functions.
 
-:py:class:`Instance` are the kfactory instances used to also acquire
-ports etc from instances.
+[Instance][kfactory.kcell.Instance] are the kfactory instances used to also acquire
+ports and other inf from instances.
 
 """
 
 import functools
 import importlib
+import importlib.util
 import json
 import socket
 from collections.abc import Callable, Hashable, Iterable, Iterator
 
 # from enum import IntEnum
 from enum import Enum, IntEnum
 from hashlib import sha3_512
-from inspect import signature
+from inspect import Parameter, signature
 from pathlib import Path
 from tempfile import gettempdir
-from typing import Any, Literal, cast, overload  # ParamSpec, # >= python 3.10
+from typing import (  # ParamSpec, # >= python 3.10
+    TYPE_CHECKING,
+    Any,
+    Literal,
+    TypeVar,
+    cast,
+    overload,
+)
 
 # from cachetools import Cache, cached
 import cachetools.func
 import numpy as np
 import ruamel.yaml
 from typing_extensions import ParamSpec
 
 from . import kdb
-from .config import logger
+from .conf import config
 from .port import rename_clockwise
 
 # import struct
 # from abc import abstractmethod
 
-
-try:
-    from __main__ import __file__ as mf
-except ImportError:
-    mf = "shell"
+if TYPE_CHECKING:
+    from .pdk import Pdk
 
 
 KCellParams = ParamSpec("KCellParams")
 
+AnyTrans = TypeVar(
+    "AnyTrans", bound=kdb.Trans | kdb.DTrans | kdb.ICplxTrans | kdb.DCplxTrans
+)
+
 
 class PROPID(IntEnum):
     """Mapping for GDS properties."""
 
     NAME = 0
 
 
+class LockedError(AttributeError):
+    """Raised when a locked cell is being modified."""
+
+    @config.logger.catch
+    def __init__(self, kcell: "KCell"):
+        """Throw _locked error."""
+        super().__init__(
+            f"KCell {kcell.name} has been locked already."
+            " Modification has been disabled. "
+            "Modify the KCell in its autocell function or make a copy."
+        )
+
+
 class PortWidthMismatch(ValueError):
     """Error thrown when two ports don't have a matching `width`."""
 
-    @logger.catch
+    @config.logger.catch
     def __init__(
         self,
         inst: "Instance",
         other_inst: "Instance | Port",
         p1: "Port",
         p2: "Port",
         *args: Any,
@@ -77,18 +99,18 @@
                 *args,
             )
 
 
 class PortLayerMismatch(ValueError):
     """Error thrown when two ports don't have a matching `layer`."""
 
-    @logger.catch
+    @config.logger.catch
     def __init__(
         self,
-        lib: "KLib",
+        lib: "KCLayout",
         inst: "Instance",
         other_inst: "Instance | Port",
         p1: "Port",
         p2: "Port",
         *args: Any,
     ):
         """Throw error for the two ports `p1`/`p1`."""
@@ -115,15 +137,15 @@
                 *args,
             )
 
 
 class PortTypeMismatch(ValueError):
     """Error thrown when two ports don't have a matching `port_type`."""
 
-    @logger.catch
+    @config.logger.catch
     def __init__(
         self,
         inst: "Instance",
         other_inst: "Instance | Port",
         p1: "Port",
         p2: "Port",
         *args: Any,
@@ -156,81 +178,81 @@
     save.gds2_write_cell_properties = True
     save.gds2_write_file_properties = True
     save.gds2_write_timestamps = False
 
     return save
 
 
-class KLib(kdb.Layout):
-    """Small extension to the ``klayout.db.Layout``.
+class KCLayout(kdb.Layout):
+    """Small extension to the klayout.db.Layout.
 
-    It adds tracking for the :py:class:`~kfactory.kcell.KCell` objects
-    instead of only the :py:class:`klayout.db.Cell` objects.
-    Additionally it allows creation and registration through :py:func:`~create_cell`
+    It adds tracking for the [KCell][kfactory.kcell.KCell] objects
+    instead of only the `klayout.db.Cell` objects.
+    Additionally it allows creation and registration through `create_cell`
 
-    All attributes of ``klayout.db.Layout`` are transparently accessible
+    All attributes of `klayout.db.Layout` are transparently accessible
 
     Attributes:
         editable: Whether the layout should be opened in editable mode (default: True)
-        rename_function: function that takes an Iterable[Port] and renames them
+        rename_function: function that takes an iterable object of ports and renames them
     """
 
-    def __init__(self, editable: bool = True) -> None:
-        """Crete a library of cells.
+    def __init__(self, editable: bool = True, pdk: "Pdk | None" = None) -> None:
+        """Create a library of cells.
 
         Args:
             editable: Open the KLayout Layout in editable mode if `True`.
+            pdk: Pdk associated with the layout.
         """
         self.kcells: dict[int, "KCell"] = {}
         kdb.Layout.__init__(self, editable)
         self.rename_function: Callable[..., None] = rename_clockwise
+        self.pdk = pdk
 
-    def dup(self, init_cells: bool = True) -> "KLib":
-        """Create a duplication of the `~KLib` object.
+    def dup(self, init_cells: bool = True) -> "KCLayout":
+        """Create a duplication of the `~KCLayout` object.
 
         Args:
-            init_cells: initialize the all cells in the new KLib object
+            init_cells: initialize the all cells in the new KCLayout object
 
         Returns:
             Copy of itself
         """
-        klib = KLib()
-        klib.assign(super().dup())
+        kcl = KCLayout()
+        kcl.assign(super().dup())
         if init_cells:
             for i, kc in self.kcells.items():
-                klib.kcells[i] = KCell(
+                kcl.kcells[i] = KCell(
                     name=kc.name,
-                    klib=klib,
-                    kdb_cell=klib.cell(kc.name),
+                    kcl=kcl,
+                    kdb_cell=kcl.cell(kc.name),
                     ports=kc.ports,
                 )
-        klib.rename_function = self.rename_function
-        return klib
+        kcl.rename_function = self.rename_function
+        return kcl
 
     def create_cell(  # type: ignore[override]
         self,
         name: str,
         *args: str,
         allow_duplicate: bool = False,
     ) -> kdb.Cell:
         """Create a new cell in the library.
 
         This shouldn't be called manually.
         The constructor of KCell will call this method.
 
         Args:
-            kcell: The KCell to be registered in the Layout.
-            name: The (initial) name of the cell. Can be changed through
-                :py:func:`~update_cell_name`
+            name: The (initial) name of the cell.
             allow_duplicate: Allow the creation of a cell with the same name which
                 already is registered in the Layout.
-                This will create a cell with the name :py:attr:`name` + `$1` or `2..n`
+                This will create a cell with the name `name` + `$1` or `2..n`
                 increasing by the number of existing duplicates
             args: additional arguments passed to
-                :py:func:`~klayout.db.Layout.create_cell`
+                `klayout.db.Layout.create_cell`
 
         Returns:
             klayout.db.Cell: klayout.db.Cell object created in the Layout
 
         """
         if allow_duplicate or (self.cell(name) is None):
             # self.kcells[name] = kcell
@@ -238,28 +260,28 @@
         else:
             raise ValueError(
                 f"Cellname {name} already exists. Please make sure the cellname is"
                 " unique or pass `allow_duplicate` when creating the library"
             )
 
     def delete_cell(self, cell: "KCell | int") -> None:
-        """Delete a cell in the klib object."""
+        """Delete a cell in the kcl object."""
         if isinstance(cell, int):
             super().delete_cell(cell)
             del self.kcells[cell]
         else:
             ci = cell.cell_index()
             super().delete_cell(ci)
             del self.kcells[ci]
 
     def register_cell(self, kcell: "KCell", allow_reregister: bool = False) -> None:
-        """Register an existing cell in the KLib object.
+        """Register an existing cell in the KCLayout object.
 
         Args:
-            kcell: KCell to be registered in the KLib
+            kcell: KCell to be registered in the KCLayout
             allow_reregister: Overwrite the existing KCell registration with this one.
                 Doesn't allow name duplication.
         """
 
         def check_name(other: "KCell") -> bool:
             return other._kdb_cell.name == kcell._kdb_cell.name
 
@@ -281,22 +303,22 @@
             try:
                 return self.kcells[obj]
             except KeyError:
                 if self.cell(obj) is None:
                     raise
 
                 c = self.cell(obj)
-                return KCell(name=c.name, klib=self, kdb_cell=self.cell(obj))
+                return KCell(name=c.name, kcl=self, kdb_cell=self.cell(obj))
         else:
             if self.cell(obj) is not None:
                 try:
                     return self.kcells[self.cell(obj).cell_index()]
                 except KeyError:
                     c = self.cell(obj)
-                    return KCell(name=c.name, klib=self, kdb_cell=self.cell(obj))
+                    return KCell(name=c.name, kcl=self, kdb_cell=self.cell(obj))
             from pprint import pformat
 
             raise ValueError(
                 f"Library doesn't have a KCell named {obj},"
                 " available KCells are"
                 f"{pformat(sorted([cell.name for cell in self.kcells.values()]))}"
             )
@@ -323,15 +345,15 @@
             lm = kdb.Layout.read(self, fn)
         else:
             lm = kdb.Layout.read(self, fn, options)
 
         if register_cells:
             new_cells = set(self.cells("*")) - cells
             for c in new_cells:
-                KCell(kdb_cell=c, klib=self)
+                KCell(kdb_cell=c, kcl=self)
 
         return lm
 
     def write(  # type: ignore[override]
         self,
         filename: str | Path,
         gzip: bool = False,
@@ -345,50 +367,51 @@
             options: KLayout options to load from the GDS. Can determine how merge
                 conflicts are handled for example. See
                 https://www.klayout.de/doc-qt5/code/class_LoadLayoutOptions.html
         """
         return kdb.Layout.write(self, str(filename), options)
 
 
-klib = KLib()
+kcl = KCLayout()
 """Default library object.
 
-:py:class:`~kfactory.kcell.KCell` uses this object unless another one is
+Any [KCell][kfactory.kcell.KCell] uses this object unless another one is
 specified in the constructor."""
 
 
 class LayerEnum(int, Enum):
     """Class for having the layers stored and a mapping int <-> layer,datatype.
 
-    This Enum can also be treated as a tuple, i.e. it implements __getitem__ and __len__
+    This Enum can also be treated as a tuple, i.e. it implements `__getitem__`
+    and `__len__`.
 
     Attributes:
         layer: layer number
         datatype: layer datatype
     """
 
     layer: int
     datatype: int
 
     def __new__(  # type: ignore[misc]
         cls: "LayerEnum",
         layer: int,
         datatype: int,
-        lib: KLib = klib,
+        kcl: KCLayout = kcl,
     ) -> "LayerEnum":
         """Create a new Enum.
 
         Because it needs to act like an integer an enum is created and expanded.
 
         Args:
             layer: Layer number of the layer.
             datatype: Datatype of the layer.
-            lib: :py:class:~`KLib` to register the layer to.
+            kcl: Base Layout object to register the layer to.
         """
-        value = lib.layer(layer, datatype)
+        value = kcl.layer(layer, datatype)
         obj: int = int.__new__(cls, value)  # type: ignore[call-overload]
         obj._value_ = value  # type: ignore[attr-defined]
         obj.layer = layer  # type: ignore[attr-defined]
         obj.datatype = datatype  # type: ignore[attr-defined]
         return obj  # type: ignore[return-value]
 
     def __getitem__(self, key: int) -> int:
@@ -433,47 +456,51 @@
         dcplx_trans: Transformation in micrometer. The port will autoconvert between
             trans and dcplx_trans on demand.
         port_type: A string defining the type of the port
         layer: Index of the layer or a LayerEnum that acts like an integer, but can
             contain layer number and datatype
         info: A dictionary with additional info. Not reflected in GDS. Copy will make a
             (shallow) copy of it.
+        d: Access port info in micrometer basis such as width and position / angle.
+        kcl: Link to the layout this port resides in.
     """
 
     yaml_tag = "!Port"
     name: str | None
+    kcl: KCLayout
     width: int
-    layer: int
+    layer: int | LayerEnum
     _trans: kdb.Trans | None
     _dcplx_trans: kdb.DCplxTrans | None
     port_type: str
+    d: "UMPort"
 
     @overload
     def __init__(
         self,
         *,
         name: str | None = None,
         width: int,
         layer: LayerEnum | int,
         trans: kdb.Trans,
-        klib: KLib = klib,
+        kcl: KCLayout = kcl,
         port_type: str = "optical",
         info: dict[str, Any] = {},
     ):
         ...
 
     @overload
     def __init__(
         self,
         *,
         name: str | None = None,
         dwidth: float,
         layer: LayerEnum | int,
         dcplx_trans: kdb.DCplxTrans,
-        klib: KLib = klib,
+        kcl: KCLayout = kcl,
         port_type: str = "optical",
         info: dict[str, Any] = {},
     ):
         ...
 
     @overload
     def __init__(
@@ -482,15 +509,15 @@
         name: str | None = None,
         width: int,
         layer: LayerEnum | int,
         port_type: str = "optical",
         angle: int,
         position: tuple[int, int],
         mirror_x: bool = False,
-        klib: KLib = klib,
+        kcl: KCLayout = kcl,
         info: dict[str, Any] = {},
     ):
         ...
 
     @overload
     def __init__(
         self,
@@ -498,15 +525,15 @@
         name: str | None = None,
         dwidth: float,
         layer: LayerEnum | int,
         port_type: str = "optical",
         dangle: float,
         dposition: tuple[float, float],
         mirror_x: bool = False,
-        klib: KLib = klib,
+        kcl: KCLayout = kcl,
         info: dict[str, Any] = {},
     ):
         ...
 
     def __init__(
         self,
         *,
@@ -519,20 +546,20 @@
         dcplx_trans: kdb.DCplxTrans | str | None = None,
         angle: int | None = None,
         dangle: float | None = None,
         position: tuple[int, int] | None = None,
         dposition: tuple[float, float] | None = None,
         mirror_x: bool = False,
         port: "Port | None" = None,
-        klib: KLib = klib,
+        kcl: KCLayout = kcl,
         info: dict[str, Any] = {},
     ):
         """Create a port from dbu or um based units."""
-        self.klib = klib
-        self.d = DPart(self)
+        self.kcl = kcl
+        self.d = UMPort(self)
         self.info = info.copy()
         if port is not None:
             self.name = port.name if name is None else name
 
             if port.dcplx_trans.is_complex():
                 self.dcplx_trans = port.dcplx_trans
             else:
@@ -556,15 +583,15 @@
             elif dcplx_trans is not None:
                 if isinstance(dcplx_trans, str):
                     self.dcplx_trans = kdb.DCplxTrans.from_s(dcplx_trans)
                 else:
                     self.dcplx_trans = dcplx_trans.dup()
                 assert dwidth is not None
                 self.d.width = dwidth
-                assert self.width * self.klib.dbu == float(
+                assert self.width * self.kcl.dbu == float(
                     dwidth
                 ), "When converting to dbu the width does not match the desired width!"
             elif width is not None:
                 assert angle is not None
                 assert position is not None
                 self.trans = kdb.Trans(angle, mirror_x, *position)
                 self.width = width
@@ -588,48 +615,48 @@
     def copy(self, trans: kdb.Trans | kdb.DCplxTrans = kdb.Trans.R0) -> "Port":
         """Get a copy of a port.
 
         Args:
             trans: an optional transformation applied to the port to be copied
 
         Returns:
-            port (:py:class:`Port`): a copy of the port
+            port: a copy of the port
         """
         if self._trans:
             if isinstance(trans, kdb.Trans):
                 _trans = trans * self.trans
                 return Port(
                     name=self.name,
                     trans=_trans,
                     layer=self.layer,
                     port_type=self.port_type,
                     width=self.width,
-                    klib=self.klib,
+                    kcl=self.kcl,
                 )
             elif not trans.is_complex():
-                _trans = trans.s_trans().to_itype(self.klib.dbu) * self.trans
+                _trans = trans.s_trans().to_itype(self.kcl.dbu) * self.trans
                 return Port(
                     name=self.name,
                     trans=_trans,
                     layer=self.layer,
                     port_type=self.port_type,
                     width=self.width,
-                    klib=self.klib,
+                    kcl=self.kcl,
                 )
         if isinstance(trans, kdb.Trans):
-            dtrans = kdb.DCplxTrans(trans.to_dtype(self.klib.dbu))
+            dtrans = kdb.DCplxTrans(trans.to_dtype(self.kcl.dbu))
             _dtrans = dtrans * self.dcplx_trans
         else:
             _dtrans = trans * self.dcplx_trans
         return Port(
             name=self.name,
             dcplx_trans=_dtrans,
             dwidth=self.d.width,
             layer=self.layer,
-            klib=self.klib,
+            kcl=self.kcl,
             port_type=self.port_type,
             info=self.info,
         )
 
     @property
     def x(self) -> int:
         """X coordinate of the port in dbu."""
@@ -640,15 +667,15 @@
         if self._trans:
             vec = self._trans.disp
             vec.x = value
             self._trans.disp = vec
         elif self._dcplx_trans:
             vec = self.trans.disp
             vec.x = value
-            self._dcplx_trans.disp = vec.to_dtype(self.klib.dbu)
+            self._dcplx_trans.disp = vec.to_dtype(self.kcl.dbu)
 
     @property
     def y(self) -> int:
         """Y coordinate of the port in dbu."""
         return self.trans.disp.y
 
     @y.setter
@@ -656,24 +683,24 @@
         if self._trans:
             vec = self._trans.disp
             vec.y = value
             self._trans.disp = vec
         elif self._dcplx_trans:
             vec = self.trans.disp
             vec.y = value
-            self._dcplx_trans.disp = vec.to_dtype(self.klib.dbu)
+            self._dcplx_trans.disp = vec.to_dtype(self.kcl.dbu)
 
     @property
     def trans(self) -> kdb.Trans:
         """Simple Transformation of the Port.
 
         If this is set with the setter, it will overwrite any transformation or
         dcplx transformation
         """
-        return self._trans or self.dcplx_trans.s_trans().to_itype(self.klib.dbu)
+        return self._trans or self.dcplx_trans.s_trans().to_itype(self.kcl.dbu)
 
     @trans.setter
     def trans(self, value: kdb.Trans) -> None:
         self._trans = value.dup()
         self._dcplx_trans = None
 
     @property
@@ -681,26 +708,26 @@
         """Complex transformation (µm based).
 
         If the internal transformation is simple, return a complex copy.
 
         The setter will set a complex transformation and overwrite the internal
         transformation (set simple to `None` and the complex to the provided value.
         """
-        return self._dcplx_trans or kdb.DCplxTrans(self.trans.to_dtype(self.klib.dbu))
+        return self._dcplx_trans or kdb.DCplxTrans(self.trans.to_dtype(self.kcl.dbu))
 
     @dcplx_trans.setter
     def dcplx_trans(self, value: kdb.DCplxTrans) -> None:
         self._dcplx_trans = value.dup()
         self._trans = None
 
     @property
     def angle(self) -> int:
         """Angle of the transformation.
 
-        In the range of [0,1,2,3] which are increments in 90°. Not to be confused
+        In the range of `[0,1,2,3]` which are increments in 90°. Not to be confused
         with `rot` of the transformation which keeps additional info about the
         mirror flag.
         """
         return self.trans.angle
 
     @angle.setter
     def angle(self, value: int) -> None:
@@ -722,14 +749,21 @@
             self.dcplx_trans.angle = value
 
     @property
     def mirror(self) -> bool:
         """Returns `True`/`False` depending on the mirror flag on the transformation."""
         return self.trans.is_mirror()
 
+    @mirror.setter
+    def mirror(self, value: bool) -> None:
+        """Setter for mirror flag on trans."""
+        self._trans = self.trans.dup()
+        self._dcplx_trans = None
+        self._trans.mirror = value
+
     def hash(self) -> bytes:
         """Hash of Port."""
         h = sha3_512()
         name = self.name if self.name else ""
         h.update(name.encode("UTF-8"))
         h.update(self.trans.hash().to_bytes(8, "big"))
         h.update(self.width.to_bytes(8, "big"))
@@ -750,15 +784,15 @@
             return (
                 f"Port({'name: ' + self.name if self.name else ''}"
                 f", dwidth: {self.d.width}, trans: {self.dcplx_trans.to_s()}, layer: "
                 f"{ln}, port_type: {self.port_type})"
             )
 
 
-class DPart:
+class UMPort:
     """Make the port able to dynamically give um based info."""
 
     def __init__(self, parent: Port):
         """Constructor, just needs a pointer to the port.
 
         Args:
             parent: port that this should be attached to
@@ -771,42 +805,42 @@
         return self.parent.dcplx_trans.disp.x
 
     @x.setter
     def x(self, value: float) -> None:
         vec = self.parent.dcplx_trans.disp
         vec.x = value
         if self.parent._trans:
-            self.parent._trans.disp = vec.to_itype(self.parent.klib.dbu)
+            self.parent._trans.disp = vec.to_itype(self.parent.kcl.dbu)
         elif self.parent._dcplx_trans:
             self.parent._dcplx_trans.disp = vec
 
     @property
     def y(self) -> float:
         """Y coordinate of the port in um."""
         return self.parent.dcplx_trans.disp.y
 
     @y.setter
     def y(self, value: float) -> None:
         vec = self.parent.dcplx_trans.disp
         vec.y = value
         if self.parent._trans:
-            self.parent._trans.disp = vec.to_itype(self.parent.klib.dbu)
+            self.parent._trans.disp = vec.to_itype(self.parent.kcl.dbu)
         elif self.parent._dcplx_trans:
             self.parent._dcplx_trans.disp = vec
 
     @property
     def position(self) -> tuple[float, float]:
         """Coordinate of the port in um."""
         vec = self.parent.dcplx_trans.disp
         return (vec.x, vec.y)
 
     @position.setter
     def position(self, pos: tuple[float, float]) -> None:
         if self.parent._trans:
-            self.parent._trans.disp = kdb.DVector(*pos).to_itype(self.parent.klib.dbu)
+            self.parent._trans.disp = kdb.DVector(*pos).to_itype(self.parent.kcl.dbu)
         elif self.parent._dcplx_trans:
             self.parent._dcplx_trans.disp = kdb.DVector(*pos)
 
     @property
     def angle(self) -> float:
         """Angle of the port in degrees."""
         return self.parent.dcplx_trans.angle
@@ -821,154 +855,161 @@
         trans = self.parent.dcplx_trans
         trans.angle = value
         self.parent.dcplx_trans = trans
 
     @property
     def width(self) -> float:
         """Width of the port in um."""
-        return self.parent.width * self.parent.klib.dbu
+        return self.parent.width * self.parent.kcl.dbu
 
     @width.setter
     def width(self, value: float) -> None:
-        self.parent.width = int(value / self.parent.klib.dbu)
-        assert self.parent.width * self.parent.klib.dbu == float(value), (
+        self.parent.width = int(value / self.parent.kcl.dbu)
+        assert self.parent.width * self.parent.kcl.dbu == float(value), (
             "When converting to dbu the width does not match the desired width"
             f"({self.width} / {value})!"
         )
 
 
 class KCell:
     """KLayout cell and change its class to KCell.
 
-    A KCell is a dynamic proxy for :py:class:~`kdb.Cell`. It has all the
+    A KCell is a dynamic proxy for kdb.Cell. It has all the
     attributes of the official KLayout class. Some attributes have been adjusted
     to return KCell specific sub classes. If the function is listed here in the
     docs, they have been adjusted for KFactory specifically. This object will
-    transparently proxy to :py:class:`kdb.Cell`. Meaning any attribute not directly
+    transparently proxy to kdb.Cell. Meaning any attribute not directly
     defined in this class that are available from the KLayout counter part can
     still be accessed. The pure KLayout object can be accessed with
-    :py:attr:`KCell._kdb_cell`.
+    `_kdb_cell`.
 
     Attributes:
-        klib: Library object that is the manager of the KLayout
-            :py:class:`kdb.Layout`
-        settings: A dictionary containing settings populated by:py:func:`autocell`
+        kcl: Library object that is the manager of the KLayout
+        settings: A dictionary containing settings populated by the
+            [cell][kfactory.kcell.cell] decorator.
         info: Dictionary for storing additional info if necessary. This is not
             passed to the GDS and therefore not reversible.
         _kdb_cell: Pure KLayout cell object.
         _locked: If set the cell shouldn't be modified anymore.
         ports: Manages the ports of the cell.
     """
 
     yaml_tag = "!KCell"
     _ports: "Ports"
 
     def __init__(
         self,
         name: str | None = None,
-        klib: KLib = klib,
+        kcl: KCLayout = kcl,
         kdb_cell: kdb.Cell | None = None,
         ports: "Ports | None" = None,
     ):
         """Constructor of KCell.
 
         Args:
             name: Name of the cell, if None will autogenerate name to
                 "Unnamed_<cell_index>".
-            klib: KLib the cell should be attached to.
+            kcl: KCLayout the cell should be attached to.
             kdb_cell: If not `None`, a KCell will be created from and existing
                 KLayout Cell
-            ports: Attach an existing :py:class:`~Ports` object to the KCell,
+            ports: Attach an existing [Ports][kfactory.kcell.Ports] object to the KCell,
                 if `None` create an empty one.
         """
-        self.klib = klib
+        self.kcl = kcl
         self.insts: Instances = Instances()
         self.settings: dict[str, Any] = {}
         self.info: dict[str, Any] = {}
         self._locked = False
         if name is None:
             _name = "Unnamed_!"
         else:
             _name = name
-        self._kdb_cell = kdb_cell or klib.create_cell(_name)
+        self._kdb_cell = kdb_cell or kcl.create_cell(_name)
         if _name == "Unnamed_!":
             self._kdb_cell.name = f"Unnamed_{self.cell_index()}"
-        self.klib.register_cell(self, allow_reregister=True)
-        self.ports: Ports = ports or Ports(self.klib)
+        self.kcl.register_cell(self, allow_reregister=True)
+        self.ports: Ports = ports or Ports(self.kcl)
         self.complex = False
 
         if kdb_cell is not None:
             for inst in kdb_cell.each_inst():
-                self.insts.append(Instance(self.klib, inst))
+                self.insts.append(Instance(self.kcl, inst))
 
     @property
     def name(self) -> str:
         """Name of the KCell."""
         return self._kdb_cell.name
 
     @name.setter
     def name(self, value: str) -> None:
+        if self._locked:
+            raise LockedError(self)
         self._kdb_cell.name = value
 
     @property
     def prop_id(self) -> int:
         """Gets the properties ID associated with the cell."""
         return self._kdb_cell.prop_id
 
     @prop_id.setter
     def prop_id(self, value: int) -> None:
+        if self._locked:
+            raise LockedError(self)
         self._kdb_cell.prop_id = value
 
     @property
     def ghost_cell(self) -> bool:
         """Returns a value indicating whether the cell is a "ghost cell"."""
         return self._kdb_cell.ghost_cell
 
     @ghost_cell.setter
     def ghost_cell(self, value: bool) -> None:
+        if self._locked:
+            raise LockedError(self)
         self._kdb_cell.ghost_cell = value
 
     def __getattr__(self, name):  # type: ignore[no-untyped-def]
         """If KCell doesn't have an attribute, look in the KLayout Cell."""
         return getattr(self._kdb_cell, name)
 
     def dup(self) -> "KCell":
         """Copy the full cell.
 
-        Sets :py:attr:_locked to `False`
+        Sets `_locked` to `False`
 
         Returns:
             cell: Exact copy of the current cell.
                 The name will have `$1` as duplicate names are not allowed
         """
         kdb_copy = self._kdb_copy()
 
-        c = KCell(klib=self.klib, kdb_cell=kdb_copy)
+        c = KCell(kcl=self.kcl, kdb_cell=kdb_copy)
         c.ports = self.ports.copy()
         for inst in kdb_copy.each_inst():
-            c.insts.append(Instance(self.klib, instance=inst))
-        c._locked = False
+            c.insts.append(Instance(self.kcl, instance=inst))
+        # c._locked = False
         return c
 
     def __copy__(self) -> "KCell":
-        """Enables use of :py:func:`copy.copy` and :py:func:`copy.deep_copy`."""
+        """Enables use of `copy.copy` and `copy.deep_copy`."""
         return self.dup()
 
     def add_port(
         self, port: Port, name: str | None = None, keep_mirror: bool = False
     ) -> None:
         """Add an existing port. E.g. from an instance to propagate the port.
 
         Args:
-            port: The port to add. Port should either be a :py:class:`~Port`,
-                or will be converted to an integer based port with 90° increment
+            port: The port to add.
             name: Overwrite the name of the port
             keep_mirror: Keep the mirror part of the transformation of a port if
                 `True`, else set the mirror flag to `False`.
         """
+        if self._locked:
+            raise LockedError(self)
         self.ports.add_port(port=port, name=name)
 
     def add_ports(
         self, ports: Iterable[Port], prefix: str = "", keep_mirror: bool = False
     ) -> None:
         """Add a sequence of ports to the cells.
 
@@ -976,14 +1017,16 @@
 
         Args:
             ports: list/tuple (anything iterable) of ports.
             prefix: string to add in front of all the port names
             keep_mirror: Keep the mirror part of the transformation of a port if
                 `True`, else set the mirror flag to `False`.
         """
+        if self._locked:
+            raise LockedError(self)
         self.ports.add_ports(ports=ports, prefix=prefix, keep_mirror=keep_mirror)
 
     @classmethod
     def from_yaml(
         cls: "Callable[..., KCell]",
         constructor: Any,
         node: Any,
@@ -994,19 +1037,19 @@
             constructor,
             node,
             deep=True,
         )
         cell = cls(d["name"])
         if verbose:
             print(f"Building {d['name']}")
-        cell.ports = d.get("ports", Ports(ports=[], klib=cell.klib))
+        cell.ports = d.get("ports", Ports(ports=[], kcl=cell.kcl))
         cell.settings = d.get("settings", {})
         for inst in d.get("insts", []):
             if "cellname" in inst:
-                _cell = cell.klib[inst["cellname"]]
+                _cell = cell.kcl[inst["cellname"]]
             elif "cellfunction" in inst:
                 module_name, fname = inst["cellfunction"].rsplit(".", 1)
                 module = importlib.import_module(module_name)
                 cellf = getattr(module, fname)
                 _cell = cellf(**inst["settings"])
                 del module
             else:
@@ -1162,30 +1205,44 @@
     def show(self) -> None:
         """Stream the gds to klive.
 
         Will create a temporary file of the gds and load it in KLayout via klive
         """
         show(self)
 
-    def _ipython_display_(self) -> None:
-        """Display a cell in a Jupyter Cell.
+    def plot(self) -> None:
+        """Display cell.
 
         Usage: Pass the kcell variable as an argument in the cell at the end
         """
         from .widgets.interactive import display_kcell
 
         display_kcell(self)
 
+    def _ipython_display_(self) -> None:
+        """Display a cell in a Jupyter Cell.
+
+        Usage: Pass the kcell variable as an argument in the cell at the end
+        """
+        self.plot()
+
+    def __repr__(self) -> str:
+        """Return a string representation of the Cell."""
+        port_names = [p.name for p in self.ports]
+        return f"{self.name}: ports {port_names}, {len(self.insts)} instances"
+
     @property
     def ports(self) -> "Ports":
         """Ports associated with the cell."""
         return self._ports
 
     @ports.setter
     def ports(self, new_ports: "InstancePorts | Ports") -> None:
+        if self._locked:
+            raise LockedError(self)
         self._ports = new_ports.copy()
 
     @overload
     def create_port(
         self,
         *,
         name: str | None = None,
@@ -1228,15 +1285,17 @@
         layer: LayerEnum | int,
         port_type: str = "optical",
         mirror_x: bool = False,
     ) -> None:
         ...
 
     def create_port(self, **kwargs: Any) -> None:
-        """Proxy for :py:func:`Ports.create_port`."""
+        """Proxy for [Ports.create_port][kfactory.kcell.Ports.create_port]."""
+        if self._locked:
+            raise LockedError(self)
         self.ports.create_port(**kwargs)
 
     @overload
     def create_inst(
         self,
         cell: "KCell | int",
         trans: kdb.Trans | kdb.ICplxTrans | kdb.Vector = kdb.Trans(),
@@ -1290,25 +1349,29 @@
     ) -> "Instance":
         """Add an instance of another KCell.
 
         Args:
             cell: The cell to be added
             trans: The integer transformation applied to the reference
             dtrans: um transformation of the reference. If not `None`,
-                will overwrite :py:attr:`trans`
+                will overwrite trans`
             a: Vector (DVector if trans is um based) for the array.
-                Needs to be in positive X-direction
-            b: Vector (DVector if trans is um based) for the array.
-                Needs to be in positive Y-direction
-            na: Number of elements in direction of :py:attr:`a`
-            nb: Number of elements in direction of :py:attr:`b`
+                Needs to be in positive X-direction. Usually this is only a
+                Vector in x-direction. Some foundries won't allow other Vectors.
+            b: Vector (DVector if transs is um based) for the array.
+                Needs to be in positive Y-direction. Usually this is only a
+                Vector in x-direction. Some foundries won't allow other Vectors.
+            na: Number of elements in direction of `a`
+            nb: Number of elements in direction of `b`
 
         Returns:
-            :py:class:`~Instance`: The created instance
+            The created instance
         """
+        if self._locked:
+            raise LockedError(self)
         if isinstance(cell, int):
             ci = cell
         else:
             ci = cell.cell_index()
 
         if dtrans is None:
             if a is None:
@@ -1330,27 +1393,27 @@
                 cast(kdb.DVector, a)
                 cast(kdb.DVector, b)
                 ca = self._kdb_cell.insert(
                     kdb.DCellInstArray(
                         ci, dtrans, a, b, na, nb  # type: ignore[arg-type]
                     )
                 )
-        inst = Instance(self.klib, ca)
+        inst = Instance(self.kcl, ca)
         self.insts.append(inst)
         return inst
 
     def _kdb_copy(self) -> kdb.Cell:
         return self._kdb_cell.dup()
 
     def layer(self, *args: Any, **kwargs: Any) -> int:
-        """Get the layer info, convenience for klayout.db.Layout.layer."""
-        return self.klib.layer(*args, **kwargs)
+        """Get the layer info, convenience for `klayout.db.Layout.layer`."""
+        return self.kcl.layer(*args, **kwargs)
 
     def __lshift__(self, cell: "KCell") -> "Instance":
-        """Convenience function for :py:attr:"~create_inst(cell)`.
+        """Convenience function for [create_inst][kfactory.kcell.KCell.create_inst].
 
         Args:
             cell: The cell to be added as an instance
         """
         return self.create_inst(cell)
 
     def hash(self) -> bytes:
@@ -1373,43 +1436,47 @@
         return h.digest()
 
     def autorename_ports(self, rename_func: Callable[..., None] | None = None) -> None:
         """Rename the ports with the schema angle -> "NSWE" and sort by x and y.
 
         Args:
             rename_func: Function that takes Iterable[Port] and renames them.
-            This can of course contain a filter and only rename some of the ports
+                This can of course contain a filter and only rename some of the ports
         """
+        if self._locked:
+            raise LockedError(self)
         if rename_func is None:
-            self.klib.rename_function(self.ports._ports)
+            self.kcl.rename_function(self.ports._ports)
         else:
             rename_func(self.ports._ports)
 
     def flatten(self, prune: bool = True, merge: bool = True) -> None:
         """Flatten the cell.
 
         Pruning will delete the klayout.db.Cell if unused,
         but might cause artifacts at the moment.
 
         Args:
             prune: Delete unused child cells if they aren't used in any other KCell
             merge: Merge the shapes on all layers
         """
+        if self._locked:
+            raise LockedError(self)
         self._kdb_cell.flatten(False)  # prune)
         self.insts = Instances()
 
         if merge:
             for layer in self.layout().layer_indexes():
                 reg = kdb.Region(self.begin_shapes_rec(layer))
                 reg.merge()
                 self.clear(layer)
                 self.shapes(layer).insert(reg)
 
     def draw_ports(self) -> None:
-        """Draw all the ports on their respective :py:attr:`Port.layer`:."""
+        """Draw all the ports on their respective layer."""
         polys: dict[int, kdb.Region] = {}
 
         for port in self.ports:
             w = port.width
 
             if w in polys:
                 poly = polys[w]
@@ -1445,15 +1512,18 @@
                 self.shapes(port.layer).insert(
                     kdb.Text(port.name if port.name else "", port.trans)
                 )
 
     def write(
         self, filename: str | Path, save_options: kdb.SaveLayoutOptions = default_save()
     ) -> None:
-        """Write a KCell to a GDS. See :py:func:`KLib.write` for more info."""
+        """Write a KCell to a GDS.
+
+        See [KCLayout.write][kfactory.kcell.KCLayout.write] for more info.
+        """
         return self._kdb_cell.write(str(filename), save_options)
 
     @classmethod
     def to_yaml(cls, representer, node):  # type: ignore
         """Internal function to convert the cell to yaml."""
         d = {
             "name": node.name,
@@ -1478,27 +1548,26 @@
             d["shapes"] = shapes
         if len(node.settings) > 0:
             d["settings"] = node.settings
         return representer.represent_mapping(cls.yaml_tag, d)
 
     def each_inst(self) -> Iterator["Instance"]:
         """Iterates over all child instances (which may actually be instance arrays)."""
-        yield from (Instance(self.klib, inst) for inst in self._kdb_cell.each_inst())
+        yield from (Instance(self.kcl, inst) for inst in self._kdb_cell.each_inst())
 
     def each_overlapping_inst(self, b: kdb.Box | kdb.DBox) -> Iterator["Instance"]:
         """Gets the instances overlapping the given rectangle."""
         yield from (
-            Instance(self.klib, inst)
-            for inst in self._kdb_cell.each_overlapping_inst(b)
+            Instance(self.kcl, inst) for inst in self._kdb_cell.each_overlapping_inst(b)
         )
 
     def each_touching_inst(self, b: kdb.Box | kdb.DBox) -> Iterator["Instance"]:
         """Gets the instances overlapping the given rectangle."""
         yield from (
-            Instance(self.klib, inst) for inst in self._kdb_cell.each_touching_inst(b)
+            Instance(self.kcl, inst) for inst in self._kdb_cell.each_touching_inst(b)
         )
 
     @overload
     def insert(
         self, inst: "Instance | kdb.CellInstArray | kdb.DCellInstArray"
     ) -> "Instance":
         ...
@@ -1511,41 +1580,96 @@
 
     def insert(
         self,
         inst: "Instance | kdb.CellInstArray | kdb.DCellInstArray",
         property_id: int | None = None,
     ) -> "Instance":
         """Inserts a cell instance given by another reference."""
+        if self._locked:
+            raise LockedError(self)
         if isinstance(inst, Instance):
-            return Instance(self.klib, self._kdb_cell.insert(inst._instance))
+            return Instance(self.kcl, self._kdb_cell.insert(inst._instance))
         else:
             if not property_id:
-                return Instance(self.klib, self._kdb_cell.insert(inst))
+                return Instance(self.kcl, self._kdb_cell.insert(inst))
             else:
                 assert isinstance(inst, kdb.CellInstArray | kdb.DCellInstArray)
-                return Instance(self.klib, self._kdb_cell.insert(inst, property_id))
+                return Instance(self.kcl, self._kdb_cell.insert(inst, property_id))
+
+    @overload
+    def transform(
+        self,
+        inst: kdb.Instance,
+        trans: kdb.Trans | kdb.DTrans | kdb.ICplxTrans | kdb.DCplxTrans,
+        /,
+        *,
+        no_warn: bool = False,
+    ) -> "Instance":
+        ...
+
+    @overload
+    def transform(
+        self,
+        trans: kdb.Trans | kdb.DTrans | kdb.ICplxTrans | kdb.DCplxTrans,
+        /,
+        *,
+        no_warn: bool = False,
+    ) -> None:
+        ...
+
+    def transform(
+        self,
+        inst_or_trans: kdb.Instance
+        | kdb.Trans
+        | kdb.DTrans
+        | kdb.ICplxTrans
+        | kdb.DCplxTrans,
+        trans: kdb.Trans | kdb.DTrans | kdb.ICplxTrans | kdb.DCplxTrans | None = None,
+        /,
+        *,
+        no_warn: bool = False,
+    ) -> "Instance | None":
+        """Transforms the instance or cell with the transformation given."""
+        if self._locked:
+            raise LockedError(self)
+        if trans:
+            return Instance(
+                self.kcl,
+                self._kdb_cell.transform(
+                    inst_or_trans, trans  # type: ignore[arg-type]
+                ),
+            )
+        else:
+            return self._kdb_cell.transform(inst_or_trans)  # type:ignore[arg-type]
 
 
 class Instance:
     """An Instance of a KCell.
 
     An Instance is a reference to a KCell with a transformation.
 
     Attributes:
-        _instance: The internal :py:class:~`kdb.Instance` reference
+        _instance: The internal `kdb.Instance` reference
         ports: Transformed ports of the KCell
+        kcl: Pointer to the layout object holding the instance
+        d: Helper that allows retrieval of instance information in um
     """
 
     yaml_tag = "!Instance"
+    _instance: kdb.Instance
+    kcl: KCLayout
+    ports: "InstancePorts"
+    d: "UMInstance"
 
-    def __init__(self, klib: KLib, instance: kdb.Instance) -> None:
+    def __init__(self, kcl: KCLayout, instance: kdb.Instance) -> None:
         """Create an instance from a KLayout Instance."""
         self._instance = instance
-        self.klib = klib
+        self.kcl = kcl
         self.ports = InstancePorts(self)
+        self.d = UMInstance(self)
 
     def __getattr__(self, name):  # type: ignore[no-untyped-def]
         """If we don't have an attribute, get it from the instance."""
         return getattr(self._instance, name)
 
     @property
     def name(self) -> str | None:
@@ -1565,15 +1689,15 @@
     @cell_index.setter
     def cell_index(self, value: int) -> None:
         self._instance_.cell_index = value
 
     @property
     def cell(self) -> KCell:
         """Parent KCell  of the Instance."""
-        return self.klib[self.cell_index]
+        return self.kcl[self.cell_index]
 
     @cell.setter
     def cell(self, value: KCell) -> None:
         self.cell_index = value.cell_index()
 
     @property
     def a(self) -> kdb.Vector:
@@ -1667,15 +1791,15 @@
     @nb.setter
     def nb(self, value: int) -> None:
         self._instance.nb = value
 
     @property
     def parent_cell(self) -> KCell:
         """Gets the cell this instance is contained in."""
-        return self.klib[self._instance.parent_cell.cell_index()]
+        return self.kcl[self._instance.parent_cell.cell_index()]
 
     @parent_cell.setter
     def parent_cell(self, cell: KCell | kdb.Cell) -> None:
         if isinstance(cell, KCell):
             self._instance.parent_cell = cell._kdb_cell
         else:
             self._instance.parent_cell = cell
@@ -1724,101 +1848,38 @@
         other_port_name: str | None = None,
         *,
         mirror: bool = False,
         allow_width_mismatch: bool = False,
         allow_layer_mismatch: bool = False,
         allow_type_mismatch: bool = False,
     ) -> None:
-        """Align port with name ``portname`` to a port.
-
-        .. deprecated:: 0.6.0
-            Use :py:func:`align` instead.
-            :py:func:`connect` will be removed in 0.7.0
-
-        Function to allow to transform this instance so that a port of this instance is
-        aligned (same position with 180° turn) to another instance.
-
-        Args:
-            port: The name of the port of this instance to be connected, or directly an
-                instance port. Can be `None` because port names can be `None`.
-            other: The other instance or a port. Skip `other_port_name` if it's a port.
-            other_port_name: The name of the other port. Ignored if
-                :py:attr:`~other_instance` is a port.
-            mirror: Instead of applying klayout.db.Trans.R180 as a connection
-                transformation, use klayout.db.Trans.M90, which effectively means this
-                instance will be mirrored and connected.
-            allow_width_mismatch: Skip width check between the ports if set.
-            allow_layer_mismatch: Skip layer check between the ports if set.
-            allow_type_mismatch: Skip port_type check between the ports if set.
-        """
-        logger.warning(
-            "Instance.connect will be removed in 0.7.0, please use Instance.align"
-        )
-        self.align(  # type: ignore[call-overload]
-            port=port,
-            other=other,
-            other_port_name=other_port_name,
-            mirror=mirror,
-            allow_width_mismatch=allow_layer_mismatch,
-            allow_layer_mismatch=allow_layer_mismatch,
-            allow_type_mismatch=allow_type_mismatch,
-        )
-
-    @overload
-    def align(
-        self, port: str | Port | None, other: Port, *, mirror: bool = False
-    ) -> None:
-        ...
-
-    @overload
-    def align(
-        self,
-        port: str | Port | None,
-        other: "Instance",
-        other_port_name: str | None,
-        *,
-        mirror: bool = False,
-    ) -> None:
-        ...
-
-    def align(
-        self,
-        port: str | Port | None,
-        other: "Instance | Port",
-        other_port_name: str | None = None,
-        *,
-        mirror: bool = False,
-        allow_width_mismatch: bool = False,
-        allow_layer_mismatch: bool = False,
-        allow_type_mismatch: bool = False,
-    ) -> None:
-        """Align port with name ``portname`` to a port.
+        """Align port with name `portname` to a port.
 
         Function to allow to transform this instance so that a port of this instance is
-        aligned (same position with 180° turn) to another instance.
+        connected (same position with 180° turn) to another instance.
 
         Args:
             port: The name of the port of this instance to be connected, or directly an
                 instance port. Can be `None` because port names can be `None`.
             other: The other instance or a port. Skip `other_port_name` if it's a port.
             other_port_name: The name of the other port. Ignored if
-                :py:attr:`~other_instance` is a port.
+                `other` is a port.
             mirror: Instead of applying klayout.db.Trans.R180 as a connection
                 transformation, use klayout.db.Trans.M90, which effectively means this
                 instance will be mirrored and connected.
             allow_width_mismatch: Skip width check between the ports if set.
             allow_layer_mismatch: Skip layer check between the ports if set.
             allow_type_mismatch: Skip port_type check between the ports if set.
         """
         if isinstance(other, Instance):
             if other_port_name is None:
                 raise ValueError(
                     "portname cannot be None if an Instance Object is given. For"
                     "complex connections (non-90 degree and floating point ports) use"
-                    "connect_cplx instead"
+                    "route_cplx instead"
                 )
             op = other.ports[other_port_name]
         elif isinstance(other, Port):
             op = other
         else:
             raise ValueError("other_instance must be of type Instance or Port")
         if isinstance(port, Port):
@@ -1829,37 +1890,198 @@
             raise PortWidthMismatch(
                 self,
                 other,
                 p,
                 op,
             )
         elif int(p.layer) != int(op.layer) and not allow_layer_mismatch:
-            raise PortLayerMismatch(self.cell.klib, self, other, p, op)
+            raise PortLayerMismatch(self.cell.kcl, self, other, p, op)
         elif p.port_type != op.port_type and not allow_type_mismatch:
             raise PortTypeMismatch(self, other, p, op)
         else:
             if p._dcplx_trans or op._dcplx_trans:
                 dconn_trans = kdb.DCplxTrans.M90 if mirror else kdb.DCplxTrans.R180
-                self.dcplx_trans = (
+                self._instance.dcplx_trans = (
                     op.dcplx_trans * dconn_trans * p.dcplx_trans.inverted()
                 )
             else:
                 conn_trans = kdb.Trans.M90 if mirror else kdb.Trans.R180
-                self.trans = op.trans * conn_trans * p.trans.inverted()
+                self._instance.trans = op.trans * conn_trans * p.trans.inverted()
 
     @classmethod
     def to_yaml(cls, representer, node):  # type: ignore[no-untyped-def]
         """Convert the instance to a yaml representation."""
         d = {
             "cellname": node.cell.name,
             "trans": node._trans,
             "dcplx_trans": node._dcplx_trans,
         }
         return representer.represent_mapping(cls.yaml_tag, d)
 
+    @overload
+    def movex(self, destination: int, /) -> None:
+        ...
+
+    @overload
+    def movex(self, origin: int, destination: int) -> None:
+        ...
+
+    def movex(self, origin: int, destination: int | None = None) -> None:
+        """Move the instance in x-direction in dbu.
+
+        Args:
+            origin: reference point to move [dbu]
+            destination: move origin so that it will land on this coordinate [dbu]
+        """
+        if destination is None:
+            self.transform(kdb.Trans(origin, 0))
+        else:
+            self.transform(kdb.Trans(destination - origin, 0))
+
+    @overload
+    def movey(self, destination: int, /) -> None:
+        ...
+
+    @overload
+    def movey(self, origin: int, destination: int) -> None:
+        ...
+
+    def movey(self, origin: int, destination: int | None = None) -> None:
+        """Move the instance in y-direction in dbu.
+
+        Args:
+            origin: reference point to move [dbu]
+            destination: move origin so that it will land on this coordinate [dbu]
+        """
+        if destination is None:
+            self.transform(kdb.Trans(0, origin))
+        else:
+            self.transform(kdb.Trans(0, destination - origin))
+
+    @overload
+    def move(self, destination: tuple[int, int], /) -> None:
+        ...
+
+    @overload
+    def move(self, origin: tuple[int, int], destination: tuple[int, int]) -> None:
+        ...
+
+    def move(
+        self, origin: tuple[int, int], destination: tuple[int, int] | None = None
+    ) -> None:
+        """Move the instance in dbu.
+
+        Args:
+            origin: reference point to move [dbu]
+            destination: move origin so that it will land on this coordinate [dbu]
+        """
+        if destination is None:
+            self.transform(kdb.Trans(*origin))
+        else:
+            self.transform(
+                kdb.Trans(destination[0] - origin[0], destination[1] - origin[1])
+            )
+
+    def rotate(self, angle: Literal[0, 1, 2, 3]) -> None:
+        """Rotate instance in increments of 90°."""
+        self.transform(kdb.Trans(angle, False, 0, 0))
+
+    def __repr__(self) -> str:
+        """Return a string representation of the instance."""
+        port_names = [p.name for p in self.ports]
+        return (
+            f"{self.parent_cell.name}: ports {port_names}, {self.kcl[self.cell_index]}"
+        )
+
+
+class UMInstance:
+    """Make the port able to dynamically give um based info."""
+
+    def __init__(self, parent: Instance):
+        """Constructor, just needs a pointer to the port.
+
+        Args:
+            parent: port that this should be attached to
+        """
+        self.parent = parent
+
+    @overload
+    def movex(self, destination: float, /) -> None:
+        ...
+
+    @overload
+    def movex(self, origin: float, destination: float) -> None:
+        ...
+
+    def movex(self, origin: float, destination: float | None = None) -> None:
+        """Move the instance in x-direction in um.
+
+        Args:
+            origin: reference point to move
+            destination: move origin so that it will land on this coordinate
+        """
+        if destination is None:
+            self.parent.transform(kdb.DTrans(float(origin), 0.0))
+        else:
+            self.parent.transform(kdb.DTrans(float(destination - origin), 0.0))
+
+    @overload
+    def movey(self, destination: float, /) -> None:
+        ...
+
+    @overload
+    def movey(self, origin: float, destination: float) -> None:
+        ...
+
+    def movey(self, origin: float, destination: float | None = None) -> None:
+        """Move the instance in y-direction in um.
+
+        Args:
+            origin: reference point to move
+            destination: move origin so that it will land on this coordinate
+        """
+        if destination is None:
+            self.parent.transform(kdb.DTrans(0.0, float(origin)))
+        else:
+            self.parent.transform(kdb.DTrans(0.0, float(destination - origin)))
+
+    def rotate(self, angle: float) -> None:
+        """Rotate instance in degrees."""
+        self.parent.transform(kdb.DCplxTrans(1, angle, False, 0, 0))
+
+    @overload
+    def move(self, destination: tuple[float, float], /) -> None:
+        ...
+
+    @overload
+    def move(
+        self, origin: tuple[float, float], destination: tuple[float, float]
+    ) -> None:
+        ...
+
+    def move(
+        self,
+        origin: tuple[float, float],
+        destination: tuple[float, float] | None = None,
+    ) -> None:
+        """Move the instance in dbu.
+
+        Args:
+            origin: reference point to move [dbu]
+            destination: move origin so that it will land on this coordinate [dbu]
+        """
+        if destination is None:
+            self.parent.transform(kdb.DTrans(float(origin[0]), float(origin[1])))
+        else:
+            self.parent.transform(
+                kdb.DTrans(
+                    float(destination[0] - origin[0]), float(destination[1] - origin[1])
+                )
+            )
+
 
 class Instances:
     """Holder for instances.
 
     Allows retrieval by name or index
     """
 
@@ -1905,27 +2127,30 @@
     """A collection of ports.
 
     It is not a traditional dictionary. Elements can be retrieved as in a tradional
     dictionary. But to keep tabs on names etc, the ports are stored as a list
 
     Attributes:
         _ports: Internal storage of the ports. Normally ports should be retrieved with
-            :py:func:`__getitem__` or with :py:func:`~get_all`
+            [__getitem__][kfactory.kcell.Ports.__getitem__] or with
+            [get_all_named][kfactory.kcell.Ports.get_all_named]
     """
 
     yaml_tag = "!Ports"
+    kcl: KCLayout
+    _locked: bool
 
-    def __init__(self, klib: KLib, ports: Iterable[Port] = []) -> None:
+    def __init__(self, kcl: KCLayout, ports: Iterable[Port] = []) -> None:
         """Constructor."""
         self._ports: list[Port] = list(ports)
-        self.klib = klib
+        self.kcl = kcl
 
     def copy(self) -> "Ports":
         """Get a copy of each port."""
-        return Ports(ports=[p.copy() for p in self._ports], klib=self.klib)
+        return Ports(ports=[p.copy() for p in self._ports], kcl=self.kcl)
 
     def contains(self, port: Port) -> bool:
         """Check whether a port is already in the list."""
         return port.hash() in [v.hash() for v in self._ports]
 
     def __iter__(self) -> Iterator[Port]:
         """Iterator, that allows for loops etc to directly access the object."""
@@ -1936,16 +2161,16 @@
     ) -> None:
         """Add a port object.
 
         Args:
             port: The port to add
             name: Overwrite the name of the port
             keep_mirror: Keep the mirror flag from the original port if `True`,
-                else set :py:attr:~`Port.trans.mirror` (or the complex equivalent)
-                to `False`.
+                else set [Port.trans.mirror][kfactory.kcell.Port.trans] (or the complex
+                equivalent) to `False`.
         """
         _port = port.copy()
         if not keep_mirror:
             if port._trans:
                 port._trans.mirror = False
             elif port._dcplx_trans:
                 port._dcplx_trans.mirror = False
@@ -2033,37 +2258,37 @@
             assert width is not None
             port = Port(
                 name=name,
                 trans=trans,
                 width=width,
                 layer=layer,
                 port_type=port_type,
-                klib=self.klib,
+                kcl=self.kcl,
             )
         elif dcplx_trans is not None:
             assert dwidth is not None
             port = Port(
                 name=name,
                 dwidth=dwidth,
                 dcplx_trans=dcplx_trans,
                 layer=layer,
                 port_type=port_type,
-                klib=self.klib,
+                kcl=self.kcl,
             )
         elif angle is not None and position is not None:
             assert width is not None
             port = Port(
                 name=name,
                 width=width,
                 layer=layer,
                 port_type=port_type,
                 angle=angle,
                 position=position,
                 mirror_x=mirror_x,
-                klib=self.klib,
+                kcl=self.kcl,
             )
         else:
             raise ValueError(
                 f"You need to define width {width} and trans {trans} or angle {angle}"
                 f" and position {position} or dcplx_trans {dcplx_trans}"
                 f" and dwidth {dwidth}"
             )
@@ -2122,19 +2347,23 @@
     """Ports of an instance.
 
     These act as virtual ports as the positions needs to change if the
     instance changes etc.
 
 
     Attributes:
-        cell_ports: A pointer to the :py:class:~`Ports` of the cell
-        instance: A pointer to the :py:class:~`Instance` related to this.
+        cell_ports: A pointer to the [`KCell.ports`][kfactory.kcell.KCell.ports]
+            of the cell
+        instance: A pointer to the Instance related to this.
             This provides a way to dynamically calculate the ports.
     """
 
+    cell_ports: Ports
+    instance: Instance
+
     def __init__(self, instance: Instance) -> None:
         """Creates the virtual ports object.
 
         Args:
             instance: The related instance
         """
         self.cell_ports = instance.cell.ports
@@ -2155,28 +2384,28 @@
         else:
             yield from (p.copy(self.instance.dcplx_trans) for p in self.cell_ports)
 
     def __repr__(self) -> str:
         """String representation.
 
         Creates a copy and uses the `__repr__` of
-        :py:class:~`Ports`.
+        [Ports][kfactory.kcell.Ports.__repr__].
         """
         return repr(self.copy())
 
     def copy(self) -> Ports:
-        """Creates a copy in the form of :py:class:~`Ports`."""
+        """Creates a copy in the form of [Ports][kfactory.kcell.Ports]."""
         if not self.instance.is_complex():
             return Ports(
-                klib=self.instance.klib,
+                kcl=self.instance.kcl,
                 ports=[p.copy(self.instance.trans) for p in self.cell_ports._ports],
             )
         else:
             return Ports(
-                klib=self.instance.klib,
+                kcl=self.instance.kcl,
                 ports=[
                     p.copy(self.instance.dcplx_trans) for p in self.cell_ports._ports
                 ],
             )
 
 
 @overload
@@ -2189,32 +2418,76 @@
     *,
     set_settings: bool = True,
     set_name: bool = True,
 ) -> Callable[[Callable[KCellParams, KCell]], Callable[KCellParams, KCell]]:
     ...
 
 
-@logger.catch
+@config.logger.catch
 def autocell(
     _func: Callable[KCellParams, KCell] | None = None,
     /,
     *,
     set_settings: bool = True,
     set_name: bool = True,
     check_ports: bool = True,
     check_instances: bool = True,
 ) -> (
     Callable[KCellParams, KCell]
     | Callable[[Callable[KCellParams, KCell]], Callable[KCellParams, KCell]]
 ):
+    """Autoname and validate cells.
+
+    .. deprecated:: 0.7.0
+        Use [cell][kfactory.kcell.cell] instead.
+        `connect` will be removed in 0.8.0
+    """
+    config.logger.warning("autocell is deprecated, use cell instead")
+    return cell(  # type: ignore[no-any-return, call-overload]
+        _func,
+        set_settings=set_settings,
+        set_name=set_name,
+        check_ports=check_ports,
+        check_instances=check_instances,
+    )
+
+
+@overload
+def cell(_func: Callable[KCellParams, KCell], /) -> Callable[KCellParams, KCell]:
+    ...
+
+
+@overload
+def cell(
+    *,
+    set_settings: bool = True,
+    set_name: bool = True,
+) -> Callable[[Callable[KCellParams, KCell]], Callable[KCellParams, KCell]]:
+    ...
+
+
+@config.logger.catch
+def cell(
+    _func: Callable[KCellParams, KCell] | None = None,
+    /,
+    *,
+    set_settings: bool = True,
+    set_name: bool = True,
+    check_ports: bool = True,
+    check_instances: bool = True,
+) -> (
+    Callable[KCellParams, KCell]
+    | Callable[[Callable[KCellParams, KCell]], Callable[KCellParams, KCell]]
+):
     """Decorator to cache and auto name the celll.
 
-    This will use :py:func:`functools.cache` to cache the function call.
+    This will use `functools.cache` to cache the function call.
     Additionally, if enabled this will set the name and from the args/kwargs of the
-    function and also paste them into a settings dictionary of the :py:class:`~KCell`.
+    function and also paste them into a settings dictionary of the
+    [KCell][kfactory.kcell.KCell].
 
     Args:
         set_settings: Copy the args & kwargs into the settings dictionary
         set_name: Auto create the name of the cell to the functionname plus a
             string created from the args/kwargs
         check_ports: Check whether there are any non-90° ports in the cell and throw a
             warning if there are
@@ -2238,34 +2511,49 @@
                 p.name: p.default for k, p in sig.parameters.items()
             }
             arg_par = list(sig.parameters.items())[: len(args)]
             for i, (k, v) in enumerate(arg_par):
                 params[k] = args[i]
             params.update(kwargs)
 
+            del_parameters: list[str] = []
+
             for key, value in params.items():
                 if isinstance(value, dict):
                     params[key] = dict_to_frozen_set(value)
+                if value == Parameter.empty:
+                    del_parameters.append(key)
+
+            for param in del_parameters:
+                del params[param]
 
             @cachetools.cached(cache=cache)
             @functools.wraps(f)
             def wrapped_cell(
                 **params: KCellParams.args,
             ) -> KCell:
                 for key, value in params.items():
                     if isinstance(value, frozenset):
                         params[key] = frozenset_to_dict(value)
                 cell = f(**params)
                 if cell._locked:
+                    # If the cell is locked, it comes from a cache (most likely)
+                    # and should be copied first
                     cell = cell.dup()
                 if set_name:
-                    name = get_component_name(f.__name__, **params)
+                    name = get_cell_name(f.__name__, **params)
                     cell.name = name
                 if set_settings:
                     cell.settings.update(params)
+                if check_instances:
+                    if any(inst.is_complex() for inst in cell.each_inst()):
+                        raise ValueError(
+                            "Most foundries will not allow off-grid instances. Please "
+                            "flatten them or add check_instances=False to the decorator"
+                        )
 
                 i = 0
                 for name, setting in cell.settings.items():
                     while cell.property(i) is not None:
                         i += 1
                     if isinstance(setting, KCell):
                         cell.set_property(i, f"{name}: {setting.name}")
@@ -2288,43 +2576,27 @@
 
 
 def frozenset_to_dict(fs: frozenset[tuple[str, Hashable]]) -> dict[str, Hashable]:
     """Convert `frozenset` to `dict`."""
     return dict(fs)
 
 
-def cell(
-    _func: Callable[..., KCell] | None = None,
-    *,
-    set_settings: bool = True,
-    maxsize: int = 512,
-) -> (
-    Callable[KCellParams, KCell]
-    | Callable[[Callable[KCellParams, KCell]], Callable[KCellParams, KCell]]
-):
-    """Convenience alias for :py:func:`~autocell` with `(set_name=False)`."""
-    if _func is None:
-        return autocell(set_settings=set_settings, set_name=False)
-    else:
-        return autocell(_func)
-
-
 def dict2name(prefix: str | None = None, **kwargs: dict[str, Any]) -> str:
     """Returns name from a dict."""
     label = [prefix] if prefix else []
     for key, value in kwargs.items():
         key = join_first_letters(key)
         label += [f"{key.upper()}{clean_value(value)}"]
     _label = "_".join(label)
     return clean_name(_label)
 
 
-def get_component_name(component_type: str, **kwargs: dict[str, Any]) -> str:
-    """Convert a component to a string."""
-    name = component_type
+def get_cell_name(cell_type: str, **kwargs: dict[str, Any]) -> str:
+    """Convert a cell to a string."""
+    name = cell_type
 
     if kwargs:
         name += f"_{dict2name(None, **kwargs)}"
 
     return name
 
 
@@ -2410,62 +2682,113 @@
 
 def show(
     gds: str | KCell | Path,
     keep_position: bool = True,
     save_options: kdb.SaveLayoutOptions = default_save(),
 ) -> None:
     """Show GDS in klayout."""
+    import inspect
+
     delete = False
 
+    # Find the file that calls stack
+    # stk = inspect.stack()[-1]
+
+    try:
+        stk = inspect.getouterframes(inspect.currentframe())
+        frame = stk[2]
+        name = (
+            Path(frame.filename).stem + "_" + frame.function
+            if frame.function != "<module>"
+            else Path(frame.filename).stem
+        )
+    except Exception:
+        try:
+            from __main__ import __file__ as mf
+
+            name = mf
+        except ImportError:
+            name = "shell"
+
     if isinstance(gds, KCell):
-        _mf = "stdin" if mf == "<stdin>" else mf
-        tf = Path(gettempdir()) / Path(_mf).with_suffix(".gds")
-        tf.parent.mkdir(parents=True, exist_ok=True)
-        gds.write(str(tf), save_options)
-        gds_file = tf
-        delete = True
+        gds_file: Path | None = None
+        spec = importlib.util.find_spec("git")
+        if spec is not None:
+            import git
+
+            try:
+                repo = git.repo.Repo(".", search_parent_directories=True)
+            except git.InvalidGitRepositoryError:
+                pass
+            else:
+                wtd = repo.working_tree_dir
+                if wtd is not None:
+                    root = Path(wtd) / "build/gds"
+                    root.mkdir(parents=True, exist_ok=True)
+                    tf = root / Path(name).with_suffix(".gds")
+                    tf.parent.mkdir(parents=True, exist_ok=True)
+                    gds.write(str(tf), save_options)
+                    gds_file = tf
+                    delete = False
+        else:
+            config.logger.info(
+                "git isn't installed. For better file storage, "
+                "please install kfactory[git] or gitpython."
+            )
+        if not gds_file:
+            try:
+                from __main__ import __file__ as mf
+            except ImportError:
+                mf = "shell"
+            _mf = "stdin" if mf == "<stdin>" else mf
+            tf = Path(gettempdir()) / (name + ".gds")
+            tf.parent.mkdir(parents=True, exist_ok=True)
+            gds.write(str(tf), save_options)
+            gds_file = tf
+            delete = True
+
     elif isinstance(gds, str | Path):
         gds_file = Path(gds)
     else:
         raise NotImplementedError(f"unknown type {type(gds)} for streaming to KLayout")
-
     if not gds_file.is_file():
         raise ValueError(f"{gds_file} is not a File")
+    config.logger.debug("klive file: {}", gds_file)
     data_dict = {
         "gds": str(gds_file),
         "keep_position": keep_position,
     }
     data = json.dumps(data_dict)
     try:
         conn = socket.create_connection(("127.0.0.1", 8082), timeout=0.5)
         data = data + "\n"
         enc_data = data.encode()
         conn.sendall(enc_data)
         conn.settimeout(5)
     except OSError:
-        logger.warning("Could not connect to klive server")
+        config.logger.warning("Could not connect to klive server")
     else:
         msg = ""
         try:
             msg = conn.recv(1024).decode("utf-8")
-            logger.info(f"Message from klive: {msg}")
+            config.logger.info(f"Message from klive: {msg}")
         except OSError:
-            logger.warning("klive didn't send data, closing")
+            config.logger.warning("klive didn't send data, closing")
         finally:
             conn.close()
 
     if delete:
         Path(gds_file).unlink()
 
 
 __all__ = [
     "KCell",
     "Instance",
     "Port",
     "Ports",
     "autocell",
     "cell",
-    "klib",
-    "KLib",
+    "kcl",
+    "KCLayout",
     "default_save",
     "LayerEnum",
 ]
```

### Comparing `kfactory-0.6.3/src/kfactory/pcells/bezier.py` & `kfactory-0.7.0/src/kfactory/cells/bezier.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from collections.abc import Sequence
 
 import numpy as np
 import numpy.typing as nty
 from scipy.special import binom  # type: ignore[import]
 
-from .. import KCell, LayerEnum, autocell, kdb
-from ..utils import Enclosure
+from .. import KCell, LayerEnum, cell, kdb
+from ..utils import LayerEnclosure
 
 __all__ = ["bend_s"]
 
 
 def bezier_curve(
     t: nty.NDArray[np.float64],
     control_points: Sequence[tuple[np.float64 | float, np.float64 | float]],
@@ -24,24 +24,24 @@
         ank = binom(n, k) * (1 - t) ** (n - k) * t**k
         xs += ank * control_points[k][0]
         ys += ank * control_points[k][1]
 
     return [kdb.DPoint(float(x), float(y)) for x, y in zip(xs, ys)]
 
 
-@autocell
+@cell
 def bend_s(
     width: float,
     height: float,
     length: float,
     layer: int | LayerEnum,
     nb_points: int = 99,
     t_start: float = 0,
     t_stop: float = 1,
-    enclosure: Enclosure | None = None,
+    enclosure: LayerEnclosure | None = None,
 ) -> KCell:
     """Creat a bezier bend.
 
     Args:
         width: Width of the core. [um]
         height: height difference of left/right. [um]
         length: Length of the bend. [um]
@@ -60,29 +60,31 @@
             (_length / 2, _height),
             (_length, _height),
         ],
         t=np.linspace(t_start, t_stop, nb_points),
     )
 
     if enclosure is None:
-        enclosure = Enclosure()
+        enclosure = LayerEnclosure()
 
-    enclosure.extrude_path(c, path=pts, main_layer=layer, width=width)
+    enclosure.extrude_path(
+        c, path=pts, main_layer=layer, width=width, start_angle=0, end_angle=0
+    )
 
     c.create_port(
-        name="W0",
-        width=int(width / c.klib.dbu),
-        trans=kdb.Trans(0, False, 0, 0),
+        width=int(width / c.kcl.dbu),
+        trans=kdb.Trans(2, False, 0, 0),
         layer=layer,
         port_type="optical",
     )
     c.create_port(
-        name="E0",
-        width=int(width / c.klib.dbu),
+        width=int(width / c.kcl.dbu),
         trans=kdb.Trans(
-            0, False, c.bbox().right, c.bbox().top - int(width / c.klib.dbu) // 2
+            0, False, c.bbox().right, c.bbox().top - int(width / c.kcl.dbu) // 2
         ),
         layer=layer,
         port_type="optical",
     )
 
+    c.autorename_ports()
+
     return c
```

### Comparing `kfactory-0.6.3/src/kfactory/pcells/circular.py` & `kfactory-0.7.0/src/kfactory/cells/circular.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,37 +2,36 @@
 
 A circular bend has a constant radius.
 """
 
 import numpy as np
 
 from .. import kdb
-from ..kcell import KCell, LayerEnum, autocell
-from ..utils import Enclosure, extrude_path
+from ..kcell import KCell, LayerEnum, cell
+from ..utils import LayerEnclosure, extrude_path
 
 __all__ = ["bend_circular"]
 
 
-@autocell
+@cell
 def bend_circular(
     width: float,
     radius: float,
     layer: int | LayerEnum,
-    enclosure: Enclosure | None = None,
+    enclosure: LayerEnclosure | None = None,
     theta: float = 90,
     theta_step: float = 1,
 ) -> KCell:
     """Circular radius bend [um].
 
     Args:
         width: Width of the core. [um]
         radius: Radius of the backbone. [um]
         layer: Layer index of the target layer.
-        enclosure: :py:class:`kfactory.utils.Enclosure` object to describe the
-            claddings.
+        enclosure: Optional enclosure.
         theta: Angle amount of the bend.
         theta_step: Angle amount per backbone point of the bend.
     """
     c = KCell()
     r = radius
     backbone = [
         kdb.DPoint(x, y)
@@ -53,28 +52,28 @@
         start_angle=0,
         end_angle=theta,
     )
 
     c.create_port(
         name="o1",
         trans=kdb.Trans(2, False, 0, 0),
-        width=int(width / c.klib.dbu),
+        width=int(width / c.kcl.dbu),
         layer=layer,
     )
 
     match theta:
         case 90:
             c.create_port(
                 name="o2",
-                trans=kdb.DTrans(1, False, radius, radius).to_itype(c.klib.dbu),
-                width=int(width / c.klib.dbu),
+                trans=kdb.DTrans(1, False, radius, radius).to_itype(c.kcl.dbu),
+                width=int(width / c.kcl.dbu),
                 layer=layer,
             )
         case 180:
             c.create_port(
                 name="o2",
-                trans=kdb.DTrans(0, False, 0, 2 * radius).to_itype(c.klib.dbu),
-                width=int(width / c.klib.dbu),
+                trans=kdb.DTrans(0, False, 0, 2 * radius).to_itype(c.kcl.dbu),
+                width=int(width / c.kcl.dbu),
                 layer=layer,
             )
 
     return c
```

### Comparing `kfactory-0.6.3/src/kfactory/pcells/dbu/taper.py` & `kfactory-0.7.0/src/kfactory/cells/dbu/taper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 """Taper definitions [dbu].
 
 TODO: Non-linear tapers
 """
 
-from ... import KCell, autocell, kdb
-from ...utils import Enclosure
+from ... import KCell, cell, kdb
+from ...utils import LayerEnclosure
 
 __all__ = ["taper"]
 
 
-@autocell
+@cell
 def taper(
     width1: int,
     width2: int,
     length: int,
     layer: int,
-    enclosure: Enclosure | None = None,
+    enclosure: LayerEnclosure | None = None,
 ) -> KCell:
     r"""Linear Taper [um].
 
-    Visualization::
-
                __
              _/  │ Slab/Exclude
            _/  __│
          _/  _/  │
         │  _/    │
         │_/      │
         │_       │ Core
@@ -34,15 +32,15 @@
             \_   │
               \__│ Slab/Exclude
 
     Args:
         width1: Width of the core on the left side. [dbu]
         width2: Width of the core on the right side. [dbu]
         length: Length of the taper. [dbu]
-        layer: Layer index / :py:class:~`LayerEnum` of the core.
+        layer: Main layer of the taper.
         enclosure: Definition of the slab/exclude.
     """
     c = KCell()
 
     c.shapes(layer).insert(
         kdb.Polygon(
             [
@@ -57,12 +55,12 @@
     c.create_port(name="o1", trans=kdb.Trans(2, False, 0, 0), width=width1, layer=layer)
     c.create_port(
         name="o2", trans=kdb.Trans(0, False, length, 0), width=width2, layer=layer
     )
 
     if enclosure is not None:
         enclosure.apply_minkowski_y(c, kdb.Region(c.bbox()))
-    c.settings["width1_um"] = width1 * c.klib.dbu
-    c.settings["width2_um"] = width2 * c.klib.dbu
-    c.settings["length_um"] = length * c.klib.dbu
+    c.settings["width1_um"] = width1 * c.kcl.dbu
+    c.settings["width2_um"] = width2 * c.kcl.dbu
+    c.settings["length_um"] = length * c.kcl.dbu
 
     return c
```

### Comparing `kfactory-0.6.3/src/kfactory/pcells/dbu/waveguide.py` & `kfactory-0.7.0/src/kfactory/cells/dbu/waveguide.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,47 +8,46 @@
     │                              │
     │             Core             │
     │                              │
     ├──────────────────────────────┤
     │         Slab/Exclude         │
     └──────────────────────────────┘
 
-The slabs and excludes can be given in the form of an :py:class:~`Enclosure`.
+The slabs and excludes can be given in the form of an
+[Enclosure][kfactory.utils.LayerEnclosure].
 """
 
-from ... import KCell, LayerEnum, autocell, kdb
-from ...utils import Enclosure
+from ... import KCell, LayerEnum, cell, kdb
+from ...utils import LayerEnclosure
 
 __all__ = ["waveguide"]
 
 
-@autocell
+@cell
 def waveguide(
     width: int,
     length: int,
     layer: int | LayerEnum,
-    enclosure: Enclosure | None = None,
+    enclosure: LayerEnclosure | None = None,
 ) -> KCell:
     """Waveguide defined in dbu.
 
-    Visualization::
-
         ┌──────────────────────────────┐
         │         Slab/Exclude         │
         ├──────────────────────────────┤
         │                              │
         │             Core             │
         │                              │
         ├──────────────────────────────┤
         │         Slab/Exclude         │
         └──────────────────────────────┘
     Args:
         width: Waveguide width. [dbu]
         length: Waveguide length. [dbu]
-        layer: Layer index / :py:class:~`LayerEnum`.
+        layer: Main layer of the waveguide.
         enclosure: Definition of slab/excludes. [dbu]
     """
     c = KCell()
 
     if width // 2 * 2 != width:
         raise ValueError("The width (w) must be a multiple of 2 database units")
 
@@ -57,13 +56,13 @@
     c.create_port(
         name="o2", trans=kdb.Trans(0, False, length, 0), layer=layer, width=width
     )
 
     if enclosure is not None:
         enclosure.apply_minkowski_y(c, layer)
     c.settings = {
-        "width_um": width * c.klib.dbu,
-        "length_um": length * c.klib.dbu,
+        "width_um": width * c.kcl.dbu,
+        "length_um": length * c.kcl.dbu,
         "layer": layer,
     }
     c.autorename_ports()
     return c
```

### Comparing `kfactory-0.6.3/src/kfactory/pcells/euler.py` & `kfactory-0.7.0/src/kfactory/cells/euler.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 """
 
 import numpy as np
 from scipy.optimize import brentq  # type: ignore[import]
 from scipy.special import fresnel  # type: ignore[import]
 
 from .. import kdb
-from ..kcell import KCell, LayerEnum, autocell
-from ..utils import Enclosure, extrude_path
+from ..kcell import KCell, LayerEnum, cell
+from ..utils import LayerEnclosure, extrude_path
 
 __all__ = [
     "euler_bend_points",
     "euler_sbend_points",
     "bend_euler",
     "bend_s_euler",
 ]
@@ -154,20 +154,20 @@
         spoints.append(pts)
         right_point.append(kdb.DPoint(r_pt_x, r_pt_y))
     spoints += right_point[::-1]
 
     return spoints
 
 
-@autocell
+@cell
 def bend_euler(
     width: float,
     radius: float,
     layer: int | LayerEnum,
-    enclosure: Enclosure | None = None,
+    enclosure: LayerEnclosure | None = None,
     theta: float = 90,
     resolution: float = 150,
 ) -> KCell:
     """Create a euler bend.
 
     Args:
         width: Width of the core. [um]
@@ -190,44 +190,44 @@
         start_angle=0,
         end_angle=theta,
     )
 
     if theta == 90:
         c.create_port(
             layer=layer,
-            width=int(width / c.klib.dbu),
+            width=int(width / c.kcl.dbu),
             trans=kdb.Trans(2, False, backbone[0].to_itype(dbu).to_v()),
         )
         c.create_port(
             layer=layer,
-            width=int(width / c.klib.dbu),
+            width=int(width / c.kcl.dbu),
             trans=kdb.Trans(1, False, backbone[-1].to_itype(dbu).to_v()),
         )
     elif theta == 180:
         c.create_port(
             layer=layer,
-            width=int(width / c.klib.dbu),
+            width=int(width / c.kcl.dbu),
             trans=kdb.Trans(2, False, backbone[0].to_itype(dbu).to_v()),
         )
         c.create_port(
             layer=layer,
-            width=int(width / c.klib.dbu),
+            width=int(width / c.kcl.dbu),
             trans=kdb.Trans(2, False, backbone[-1].to_itype(dbu).to_v()),
         )
     c.autorename_ports()
     return c
 
 
-@autocell
+@cell
 def bend_s_euler(
     offset: float,
     width: float,
     radius: float,
     layer: LayerEnum | int,
-    enclosure: Enclosure | None = None,
+    enclosure: LayerEnclosure | None = None,
     resolution: float = 150,
 ) -> KCell:
     """Create a euler s-bend.
 
     Args:
         offset: Offset between left/right. [um]
         width: Width of the core. [um]
@@ -259,19 +259,19 @@
         p2 = backbone[0].to_itype(dbu)
     else:
         p1 = backbone[0].to_itype(dbu)
         p2 = backbone[-1].to_itype(dbu)
     c.create_port(
         name="W0",
         trans=kdb.Trans(2, False, p1.to_v()),
-        width=int(width / c.klib.dbu),
+        width=int(width / c.kcl.dbu),
         port_type="optical",
         layer=layer,
     )
     c.create_port(
         name="E0",
         trans=kdb.Trans(0, False, p2.to_v()),
-        width=int(width / c.klib.dbu),
+        width=int(width / c.kcl.dbu),
         port_type="optical",
         layer=layer,
     )
     return c
```

### Comparing `kfactory-0.6.3/src/kfactory/pcells/taper.py` & `kfactory-0.7.0/src/kfactory/cells/taper.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 r"""Tapers, linear only.
 
 TODO: Non-linear tapers.
 
 """
 
 
-from .. import KCell, LayerEnum, klib
-from ..utils import Enclosure
+from .. import KCell, LayerEnum, kcl
+from ..utils import LayerEnclosure
 from .dbu.taper import taper as taper_dbu
 
 __all__ = ["taper", "taper_dbu"]
 
 
 def taper(
     width1: float,
     width2: float,
     length: float,
     layer: int | LayerEnum,
-    enclosure: Enclosure | None = None,
+    enclosure: LayerEnclosure | None = None,
 ) -> KCell:
     r"""Linear Taper [um].
 
     Visualization::
 
                __
              _/  │ Slab/Exclude
@@ -36,17 +36,17 @@
             \_   │
               \__│ Slab/Exclude
 
     Args:
         width1: Width of the core on the left side. [um]
         width2: Width of the core on the right side. [um]
         length: Length of the taper. [um]
-        layer: Layer index / :py:class:~`LayerEnum` of the core.
+        layer: Main layer of the taper.
         enclosure: Definition of the slab/exclude.
     """
     return taper_dbu(
-        width1=int(width1 / klib.dbu),
-        width2=int(width2 / klib.dbu),
-        length=int(length / klib.dbu),
+        width1=int(width1 / kcl.dbu),
+        width2=int(width2 / kcl.dbu),
+        length=int(length / kcl.dbu),
         layer=layer,
         enclosure=enclosure,
     )
```

### Comparing `kfactory-0.6.3/src/kfactory/pcells/waveguide.py` & `kfactory-0.7.0/src/kfactory/cells/waveguide.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,26 +12,26 @@
     │        Slab/Exclude         │
     └─────────────────────────────┘
 
 The slabs and excludes can be given in the form of an :py:class:~`Enclosure`.
 """
 
 
-from .. import KCell, LayerEnum, klib
-from ..utils import Enclosure
+from .. import KCell, LayerEnum, kcl
+from ..utils import LayerEnclosure
 from .dbu.waveguide import waveguide as waveguide_dbu
 
 __all__ = ["waveguide", "waveguide_dbu"]
 
 
 def waveguide(
     width: float,
     length: float,
     layer: int | LayerEnum,
-    enclosure: Enclosure | None = None,
+    enclosure: LayerEnclosure | None = None,
 ) -> KCell:
     """Straight waveguide in um.
 
     Visualization::
 
         ┌─────────────────────────────┐
         │        Slab/Exclude         │
@@ -42,13 +42,13 @@
         ├─────────────────────────────┤
         │        Slab/Exclude         │
         └─────────────────────────────┘
 
     Args:
         width: Width of the waveguide. [um]
         length: Length of the waveguide. [um]
-        layer: Layer index / :py:class:~`LayerEnum`
+        layer: Main layer of the waveguide.
         enclosure: Definition of slabs/excludes. [um]
     """
     return waveguide_dbu(
-        int(width / klib.dbu), int(length / klib.dbu), layer, enclosure=enclosure
+        int(width / kcl.dbu), int(length / kcl.dbu), layer, enclosure=enclosure
     )
```

### Comparing `kfactory-0.6.3/src/kfactory/placer.py` & `kfactory-0.7.0/src/kfactory/placer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,34 @@
+"""Placer of bends/straights from a route."""
+
 import os
 import sys
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any, TypeVar
 
 from ruamel.yaml import YAML
 from ruamel.yaml.constructor import SafeConstructor
 
-from .kcell import KCell, KLib, Port, Ports
-from .kcell import klib as stdlib
-from .utils import Enclosure
+from .kcell import KCell, KCLayout, Port, Ports
+from .kcell import kcl as stdkcl
+from .utils import LayerEnclosure
 
 __all__ = ["cells_to_yaml", "cells_from_yaml"]
 
 PathLike = TypeVar("PathLike", str, Path, None)
 
 
-def cells_to_yaml(
-    output: PathLike, cells: list[KCell] | KCell
-) -> None:  # , library: KLib=library):
+def cells_to_yaml(output: PathLike, cells: list[KCell] | KCell) -> None:
     """Convert cell(s) to a yaml representations.
 
     Args:
-        output: A stream or string of a path where to dump the yaml. Can also be set to sys.stdout
-        cells: A single :py:class:`~kfactory.kcell.KCell` or a list of them.
+        output: A stream or string of a path where to dump the yaml. Can also be
+            set to sys.stdout
+        cells: A single [KCell][kfactory.kcell.KCell] or a list of them.
 
 
     Returns:
         yaml dump
     """
     yaml = YAML()
     yaml.register_class(KCell)
@@ -40,93 +41,93 @@
 def get_yaml_obj() -> YAML:
     """New global yaml object."""
     return YAML()
 
 
 def register_classes(
     yaml: YAML,
-    library: KLib = stdlib,
+    kcl: KCLayout = stdkcl,
     additional_classes: list[object] | None = None,
     verbose: bool = False,
 ) -> None:
     """Register a new KCell class compatible with ruamel yaml."""
 
     class ModKCell(KCell):
-        def __init__(self, name: str | None = None, library: KLib = library):
+        def __init__(self, name: str | None = None, library: KCLayout = kcl):
             KCell.__init__(self, name, library)
 
         @classmethod
         def from_yaml(cls, constructor, node):  # type: ignore[no-untyped-def]
             return super().from_yaml(constructor, node, verbose=verbose)
 
     yaml.register_class(ModKCell)
     yaml.register_class(Port)
     yaml.register_class(Ports)
-    yaml.register_class(Enclosure)
+    yaml.register_class(LayerEnclosure)
 
     if additional_classes is not None:
         for c in additional_classes:
             yaml.register_class(c)
 
 
 def cells_from_yaml(
     inp: Path,
-    klib: KLib = stdlib,
+    kcl: KCLayout = stdkcl,
     additional_classes: list[object] | None = None,
     verbose: bool = False,
 ) -> None:
     """Recreate cells from a yaml file.
 
     Args:
         inp: Input file path.
-        klib: KLib to load the cells into.
+        kcl: KCLayout to load the cells into.
         additional_classes: Additional yaml classes that should be registered.
             This is used for example to enable loading additional yaml files etc.
         verbose: Print more verbose errors etc.
     """
     yaml = get_yaml_obj()
     yaml.register_class(
-        include_from_loader(inp.parent, klib, additional_classes, verbose)
+        include_from_loader(inp.parent, kcl, additional_classes, verbose)
     )
 
     register_classes(
         yaml,
-        klib,
+        kcl,
         additional_classes,
         verbose,
     )
     yaml.load(inp)
 
 
 def exploded_yaml(
     inp: os.PathLike[Any],
-    library: KLib = stdlib,
+    library: KCLayout = stdkcl,
     additional_classes: list[object] | None = None,
     verbose: bool = False,
 ) -> Any:
     """Expanded yaml.
 
     Expand cross-references. Same syntax as :py:func:~`cells_from_yaml`
     """
     yaml = YAML(pure=True)
 
     class ModKCell(KCell):
-        def __init__(self, name: str | None = None, library: KLib = library):
+        def __init__(self, name: str | None = None, library: KCLayout = library):
             KCell.__init__(self, name, library)
 
         @classmethod
         def from_yaml(cls, constructor, node):  # type: ignore[no-untyped-def]
             super().from_yaml(constructor, node, verbose=verbose)
 
     return yaml.dump(yaml.load(inp), sys.stdout)
 
 
 def include_from_loader(
     folder: Path,
-    library: KLib,
+    library: KCLayout,
     additional_classes: list[object] | None,
     verbose: bool,
 ) -> Any:
     """Expand ruamel to support the `!include` keyword."""
 
     @dataclass
     class Include:
```

### Comparing `kfactory-0.6.3/src/kfactory/port.py` & `kfactory-0.7.0/src/kfactory/port.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,30 +90,29 @@
     port_type: str | None = None,
     regex: str | None = None,
     dir_names: tuple[str, str, str, str] = ("E", "N", "W", "S"),
     prefix: str = "",
 ) -> None:
     """Rename ports by angle of their transformation.
 
-    Visualization::
              N0  N1
              |___|_
         W1 -|      |- E1
             |      |
         W0 -|______|- E0
              |   |
             S0   S1
 
     Args:
         ports: list of ports to be renamed
         layer: A layer index to filter by
         port_type: port_type string to filter by
         regex: Regex string to use to filter the ports to be renamed.
         dir_names: Prefixes for the directions (east, north, west, south).
-        prefix: Prefix to add before :py:attr:~`dir_names`
+        prefix: Prefix to add before `dir_names`
     """
     _ports = filter_layer_pt_reg(ports, layer, port_type, regex)
 
     for dir in DIRECTION:
         dir_2 = -1 if dir < 2 else 1
         if dir % 2:
```

### Comparing `kfactory-0.6.3/src/kfactory/routing/electrical.py` & `kfactory-0.7.0/src/kfactory/routing/electrical.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from collections.abc import Callable
 
 from .. import kdb
 from ..kcell import Instance, KCell, Port
 from .manhattan import route_manhattan
 
 
-def connect_elec(
+def route_elec(
     c: KCell,
     start_port: Port,
     end_port: Port,
     start_straight: int | None = None,
     end_straight: int | None = None,
     route_path_function: Callable[..., list[kdb.Point]] = route_manhattan,
     width: int | None = None,
@@ -46,22 +46,21 @@
 
     pts = route_path_function(
         start_port.copy(),
         end_port.copy(),
         bend90_radius=0,
         start_straight=start_straight,
         end_straight=end_straight,
-        in_dbu=True,
     )
 
     path = kdb.Path(pts, width)
     c.shapes(layer).insert(path.polygon())
 
 
-def connect_L_route(
+def route_L(
     c: KCell,
     input_ports: list[Port],
     output_orientation: int = 1,
     wire_spacing: int = 10000,
 ) -> list[Port]:
     """Route ports towards a bundle in an L shape.
 
@@ -80,34 +79,34 @@
     if output_orientation == 1:
         for i, p in enumerate(input_ports[::-1]):
             temp_port = p.copy()
             temp_port.trans = kdb.Trans(
                 3, False, x_max - wire_spacing * (i + 1), y_max + wire_spacing
             )
 
-            connect_elec(c, p, temp_port)
+            route_elec(c, p, temp_port)
             temp_port.trans.angle = 1
             output_ports.append(temp_port)
     elif output_orientation == 3:
         for i, p in enumerate(input_ports):
             temp_port = p.copy()
             temp_port.trans = kdb.Trans(
                 1, False, x_max - wire_spacing * (i + 1), y_min - wire_spacing
             )
-            connect_elec(c, p, temp_port)
+            route_elec(c, p, temp_port)
             temp_port.trans.angle = 3
             output_ports.append(temp_port)
     else:
         raise ValueError(
             "Invalid L-shape routing. Please change output_orientaion to 1 or 3."
         )
     return output_ports
 
 
-def connect_bundle(
+def route_bundle(
     c: KCell,
     input_ports: list[Port],
     target_ports: list[Port],
     wire_spacing: int = 10000,
 ) -> None:
     """Connect multiple input ports to output ports.
 
@@ -115,15 +114,15 @@
     same direction (could be any of W, S, E, N). The target ports have the opposite
     orientation, i.e. if input ports are oriented to north, and target ports should
     be oriented to south. The function will produce a routing to connect input ports
     to output ports without any crossings.
 
     Args:
         c: KCell to place the routes in.
-        input_ports; List of start ports.
+        input_ports: List of start ports.
         target_ports: List of end ports.
         wire_spacing: Minimum space between wires. [dbu]
     """
     input_ports.sort(key=lambda p: p.y)
 
     x_max = max(p.x for p in input_ports)
     x_min = min(p.x for p in input_ports)
@@ -133,69 +132,69 @@
     if input_orientation in [1, 3]:
         y_max = input_ports[-1].y
         y_min = input_ports[0].y
         for p in input_ports:
             temp_port = p.copy()
             y_shift = y_max if input_orientation == 1 else y_min
             temp_port.trans = kdb.Trans(4 - input_orientation, False, p.x, y_shift)
-            connect_elec(c, p, temp_port)
+            route_elec(c, p, temp_port)
             temp_port.trans.angle = input_orientation
             output_ports.append(temp_port)
         output_ports.sort(key=lambda p: p.x)
         L_count = 0
         R_count = 0
         for i in range(len(output_ports)):
             if target_ports[i].x > output_ports[i].x:
                 L_count += 1
-                connect_elec(
+                route_elec(
                     c,
                     output_ports[i],
                     target_ports[i],
                     start_straight=abs(target_ports[i].y - output_ports[i].y)
                     - L_count * wire_spacing,
                     end_straight=L_count * wire_spacing,
                 )
                 R_count = 0
             else:
                 R_count += 1
-                connect_elec(
+                route_elec(
                     c,
                     output_ports[i],
                     target_ports[i],
                     start_straight=R_count * wire_spacing,
                     end_straight=abs(target_ports[i].y - output_ports[i].y)
                     - R_count * wire_spacing,
                 )
                 L_count = 0
     else:
         for p in input_ports:
             temp_port = p.copy()
             x_shift = x_max if input_orientation == 0 else x_min
             temp_port.trans = kdb.Trans(2 - input_orientation, False, x_shift, p.y)
-            connect_elec(c, p, temp_port)
+            route_elec(c, p, temp_port)
             temp_port.trans.angle = input_orientation
             output_ports.append(temp_port)
         output_ports.sort(key=lambda p: p.y)
         T_count = 0
         B_count = 0
         for i in range(len(output_ports)):
             if target_ports[i].y > output_ports[i].y:
                 B_count += 1
-                connect_elec(
+                route_elec(
                     c,
                     output_ports[i],
                     target_ports[i],
                     start_straight=abs(target_ports[i].x - output_ports[i].x)
                     - B_count * wire_spacing,
                     end_straight=B_count * wire_spacing,
                 )
                 T_count = 0
             else:
                 T_count += 1
-                connect_elec(
+                route_elec(
                     c,
                     output_ports[i],
                     target_ports[i],
                     start_straight=T_count * wire_spacing,
                     end_straight=abs(target_ports[i].y - output_ports[i].y)
                     - T_count * wire_spacing,
                 )
@@ -203,15 +202,15 @@
 
 
 def get_electrical_ports(c: Instance, port_type: str = "electrical") -> list[Port]:
     """Filter list of an instance by electrical ports."""
     return [p for p in c.ports if p.port_type == port_type]
 
 
-def connect_wire(c: KCell, input_port: Port, output_port: Port) -> None:
+def route_wire(c: KCell, input_port: Port, output_port: Port) -> None:
     """Connection between two electrical ports *DO NOT USE*.
 
     This function mainly implements a connection between two electrical ports.
     Not finished yet. Don't use.
 
     Args:
         c: KCell to place connection in.
@@ -237,15 +236,15 @@
         (
             kdb.Point(output_port.x, output_port.y + input_port.width // 2)
             if input_port.angle % 2 == 0
             else kdb.Point(output_port.x + input_port.width // 2, output_port.y)
         )
 
 
-def connect_dual_rails(
+def route_dual_rails(
     c: KCell,
     start_port: Port,
     end_port: Port,
     start_straight: int | None = None,
     end_straight: int | None = None,
     route_path_function: Callable[..., list[kdb.Point]] = route_manhattan,
     width: int | None = None,
```

### Comparing `kfactory-0.6.3/src/kfactory/routing/manhattan.py` & `kfactory-0.7.0/src/kfactory/routing/manhattan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 """Can calculate manhattan routes based on ports/transformations."""
 
 import numpy as np
 
 from .. import kdb
-from ..config import logger
-from ..kcell import KLib, Port
+from ..conf import config
+from ..kcell import KCLayout, Port
 from ..utils import clean_points
 
 __all__ = ["route_manhattan", "route_manhattan_180"]
 
 
 def droute_manhattan_180(
     port1: kdb.DTrans,
     port2: kdb.DTrans,
     bend90_radius: float,
     bend180_radius: float,
     start_straight: float,
     end_straight: float,
-    layout: KLib | kdb.Layout,
+    layout: KCLayout | kdb.Layout,
 ) -> list[kdb.Point]:
     """Calculate manhattan route using um based points.
 
     Args:
         port1: Transformation of start port.
         port2: Transformation of end port.
         bend90_radius: The radius or (symmetrical) dimension of 90° bend. [um]
         bend180_radius: The distance between the two ports of the 180° bend. [um]
         start_straight: Minimum straight after the starting port. [um]
         end_straight: Minimum straight before the end port. [um]
-        layout: Layout/KLib object where to get the dbu info from.
+        layout: Layout/KCLayout object where to get the dbu info from.
 
     Returns:
         route: Calculated route in points in dbu.
     """
     return route_manhattan_180(
         port1.to_itype(layout.dbu),
         port2.to_itype(layout.dbu),
@@ -138,27 +138,27 @@
 
 def droute_manhattan(
     port1: kdb.DTrans,
     port2: kdb.DTrans,
     bend90_radius: int,
     start_straight: int,
     end_straight: int,
-    layout: KLib | kdb.Layout,
+    layout: KCLayout | kdb.Layout,
 ) -> list[kdb.Point]:
     """Calculate manhattan route using um based points.
 
     Doesn't use any non-90° bends.
 
     Args:
         port1: Transformation of start port.
         port2: Transformation of end port.
         bend90_radius: The radius or (symmetrical) dimension of 90° bend. [um]
         start_straight: Minimum straight after the starting port. [um]
         end_straight: Minimum straight before the end port. [um]
-        layout: Layout/KLib object where to get the dbu info from.
+        layout: Layout/KCLayout object where to get the dbu info from.
 
     Returns:
         route: Calculated route in points in dbu.
     """
     return route_manhattan(
         port1.to_itype(layout.dbu),
         port2.to_itype(layout.dbu),
@@ -221,15 +221,15 @@
         (t1 * kdb.Trans(0, False, start_straight, 0)).disp.to_p(),
         (t2 * kdb.Trans(0, False, end_straight, 0)).disp.to_p(),
     )
     match (box.width(), box.height()):
         case (x, y) if (x < bend90_radius and y <= 2 * bend90_radius) or (
             x <= 2 * bend90_radius and y < bend90_radius
         ):
-            logger.warning(
+            config.logger.warning(
                 "Potential collision in routing due to small distance between the port "
                 f"in relation to bend radius {x=}/{bend90_radius}, {y=}/{bend90_radius}"
             )
 
     # we want a straight start and have to add a bend radius if
     t1 *= kdb.Trans(start_straight + bend90_radius, 0)
     tv = t1.inverted() * (t2.disp - t1.disp)
```

### Comparing `kfactory-0.6.3/src/kfactory/routing/optical.py` & `kfactory-0.7.0/src/kfactory/routing/optical.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Optical routing allows the creation of photonic (or any route using bends)."""
 
 from collections.abc import Callable, Sequence
 
 from .. import kdb
-from ..config import logger
+from ..conf import config
 from ..kcell import KCell, Port
 from .manhattan import route_manhattan
 
 
 def vec_angle(v: kdb.Vector) -> int:
     """Determine vector angle in increments of 90°."""
     if v.x != 0 and v.y != 0:
@@ -19,15 +19,15 @@
         case (x, 0) if x < 0:
             return 2
         case (0, y) if y > 0:
             return 1
         case (0, y) if y < 0:
             return 3
         case _:
-            logger.warning(f"{v} is not a manhattan, cannot determine direction")
+            config.logger.warning(f"{v} is not a manhattan, cannot determine direction")
     return -1
 
 
 def route_loopback(
     p1: Port | kdb.Trans,
     p2: Port | kdb.Trans,
     bend90_radius: int,
@@ -116,31 +116,31 @@
             start_straight=start_straight + d_loop,
             end_straight=0,
         )
         + pts_end
     )  # end_straight=end_straight# + d_loop,
 
 
-@logger.catch
-def connect(
+@config.logger.catch
+def route(
     c: KCell,
     p1: Port,
     p2: Port,
     straight_factory: Callable[[int, int], KCell],
     bend90_cell: KCell,
     bend180_cell: KCell | None = None,
     taper_cell: KCell | None = None,
     start_straight: int = 0,
     end_straight: int = 0,
     route_path_function: Callable[
         ...,
         list[kdb.Point],
     ] = route_manhattan,
     port_type: str = "optical",
-    allow_small_routes: int = False,
+    allow_small_routes: bool = False,
     different_port_width: int = False,
 ) -> None:
     """Bend 90 part."""
     if p1.width != p2.width and not different_port_width:
         raise ValueError(
             f"The ports have different widths {p1.width=} {p2.width=}. If this is"
             "intentional, add `different_port_width=True` to override this."
@@ -214,33 +214,33 @@
         )
 
         if len(pts) > 2:
             if (vec := pts[1] - pts[0]).abs() == b180r:
                 match (p1.trans.angle - vec_angle(vec)) % 4:
                     case 1:
                         bend180 = c << bend180_cell
-                        bend180.align(b180p1.name, p1)
+                        bend180.connect(b180p1.name, p1)
                         start_port = bend180.ports[b180p2.name]
                         pts = pts[1:]
                     case 3:
                         bend180 = c << bend180_cell
-                        bend180.align(b180p2.name, p1)
+                        bend180.connect(b180p2.name, p1)
                         start_port = bend180.ports[b180p1.name]
                         pts = pts[1:]
             if (vec := pts[-1] - pts[-2]).abs() == b180r:
                 match ((vec_angle(vec) - p2.trans.angle) % 4):
                     case 1:
                         bend180 = c << bend180_cell
-                        bend180.align(b180p1.name, p2)
+                        bend180.connect(b180p1.name, p2)
                         end_port = bend180.ports[b180p2.name]
                         pts = pts[:-1]
                     case 3:
                         bend180 = c << bend180_cell
                         # bend180.mirror = True
-                        bend180.align(b180p2.name, p2)
+                        bend180.connect(b180p2.name, p2)
                         end_port = bend180.ports[b180p1.name]
                         pts = pts[:-1]
 
             if len(pts) > 3:
                 # TODO 180 stuff
                 pt1, pt2, pt3 = pts[:3]
                 j = 0
@@ -253,18 +253,18 @@
                     ang1 = vec_angle(vecp)
                     ang2 = vec_angle(vec)
                     ang3 = vec_angle(vecn)
 
                     if vecp == vec and ang2 - ang1 == 0:
                         bend180 = c << bend180_cell
                         if start_port.name == b180p2.name:
-                            bend180.align(b180p1.name, start_port)
+                            bend180.connect(b180p1.name, start_port)
                             start_port = bend180.ports[b180p2.name]
                         else:
-                            bend180.align(b180p2.name, start_port)
+                            bend180.connect(b180p2.name, start_port)
                             start_port = bend180.ports[b180p1.name]
                         j = i - 1
                     elif (
                         vec.abs() == b180r
                         and (ang2 - ang1) % 4 == 1
                         and (ang3 - ang2) % 4 == 1
                     ):
@@ -396,18 +396,18 @@
 
     if (bend90_ports[1].trans.angle - bend90_ports[0].trans.angle) % 4 == 3:
         b90p1 = bend90_ports[1]
         b90p2 = bend90_ports[0]
     else:
         b90p1 = bend90_ports[0]
         b90p2 = bend90_ports[1]
-    assert b90p1.name is not None, logger.error(
+    assert b90p1.name is not None, config.logger.error(
         "bend90_cell needs named ports, {}", b90p1
     )
-    assert b90p2.name is not None, logger.error(
+    assert b90p2.name is not None, config.logger.error(
         "bend90_cell needs named ports, {}", b90p2
     )
     b90c = kdb.Trans(
         b90p1.trans.rot,
         b90p1.trans.is_mirror(),
         b90p1.trans.disp.x if b90p1.trans.angle % 2 else b90p2.trans.disp.x,
         b90p2.trans.disp.y if b90p1.trans.angle % 2 else b90p1.trans.disp.y,
@@ -440,30 +440,30 @@
         if (
             taper_cell is None
             or length
             < (taperp1.trans.disp - taperp2.trans.disp).abs() * 2 + min_straight_taper
         ):
             wg = c << straight_factory(width=w, length=(pts[1] - pts[0]).abs())
             wg_p1, wg_p2 = (v for v in wg.ports if v.port_type == port_type)
-            wg.align(wg_p1, p1)
+            wg.connect(wg_p1, p1)
         else:
             t1 = c << taper_cell
-            t1.align(taperp1.name, p1)
+            t1.connect(taperp1.name, p1)
             if length - (taperp1.trans.disp - taperp2.trans.disp).abs() * 2 != 0:
                 wg = c << straight_factory(
                     width=taperp2.width,
                     length=length - (taperp1.trans.disp - taperp2.trans.disp).abs() * 2,
                 )
                 wg_p1, wg_p2 = (v for v in wg.ports if v.port_type == port_type)
-                wg.align(wg_p1, t1, taperp2.name)
+                wg.connect(wg_p1, t1, taperp2.name)
                 t2 = c << taper_cell
-                t2.align(taperp2.name, wg_p2)
+                t2.connect(taperp2.name, wg_p2)
             else:
                 t2 = c << taper_cell
-                t2.align(taperp2.name, t1, taperp2.name)
+                t2.connect(taperp2.name, t1, taperp2.name)
         return
     for i in range(1, len(pts) - 1):
         pt = pts[i]
         new_pt = pts[i + 1]
 
         if (pt.distance(old_pt) < b90r) and not allow_small_routes:
             raise ValueError(
@@ -503,48 +503,48 @@
                 taper_cell is None
                 or length
                 < (taperp1.trans.disp - taperp2.trans.disp).abs() * 2
                 + min_straight_taper
             ):
                 wg = c << straight_factory(width=w, length=length)
                 wg_p1, wg_p2 = (v for v in wg.ports if v.port_type == port_type)
-                wg.align(wg_p1, bend90, b90p1.name)
+                wg.connect(wg_p1, bend90, b90p1.name)
             else:
                 t1 = c << taper_cell
-                t1.align(taperp1.name, bend90, b90p1.name)
+                t1.connect(taperp1.name, bend90, b90p1.name)
                 if length - (taperp1.trans.disp - taperp2.trans.disp).abs() * 2 != 0:
                     wg = c << straight_factory(
                         width=taperp2.width,
                         length=length
                         - (taperp1.trans.disp - taperp2.trans.disp).abs() * 2,
                     )
                     wg_p1, wg_p2 = (v for v in wg.ports if v.port_type == port_type)
-                    wg.align(wg_p1.name, t1, taperp2.name)
+                    wg.connect(wg_p1.name, t1, taperp2.name)
                     t2 = c << taper_cell
-                    t2.align(taperp2.name, wg, wg_p2.name)
+                    t2.connect(taperp2.name, wg, wg_p2.name)
                 else:
                     t2 = c << taper_cell
-                    t2.align(taperp2.name, t1, taperp2.name)
+                    t2.connect(taperp2.name, t1, taperp2.name)
         old_pt = pt
         old_bend_port = bend90.ports[b90p2.name]
     length = (bend90.ports[b90p2.name].trans.disp - p2.trans.disp).abs()
     if length > 0:
         if (
             taper_cell is None
             or length
             < (taperp1.trans.disp - taperp2.trans.disp).abs() * 2 + min_straight_taper
         ):
             wg = c << straight_factory(width=w, length=length)
             wg_p1, wg_p2 = (v for v in wg.ports if v.port_type == port_type)
-            wg.align(wg_p1.name, bend90, b90p2.name)
+            wg.connect(wg_p1.name, bend90, b90p2.name)
         else:
             t1 = c << taper_cell
-            t1.align(taperp1.name, bend90, b90p2.name)
+            t1.connect(taperp1.name, bend90, b90p2.name)
             if length - (taperp1.trans.disp - taperp2.trans.disp).abs() * 2 != 0:
                 wg = c << straight_factory(
                     width=taperp2.width,
                     length=length - (taperp1.trans.disp - taperp2.trans.disp).abs() * 2,
                 )
                 wg_p1, wg_p2 = (v for v in wg.ports if v.port_type == port_type)
-                wg.align(wg_p1.name, t1, taperp2.name)
+                wg.connect(wg_p1.name, t1, taperp2.name)
                 t2 = c << taper_cell
-                t2.align(taperp2.name, wg, wg_p2.name)
+                t2.connect(taperp2.name, wg, wg_p2.name)
```

### Comparing `kfactory-0.6.3/src/kfactory/utils/__init__.py` & `kfactory-0.7.0/src/kfactory/utils/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 """Utilities to provide geometrical, fill and DRC violation help.
 
-:py:class:~`Enclosures can automatically generate slab and excludes based on minkowski
-sums instead of only vector based sizing.
+[Enclosures][kfactory.utils.enclosure.LayerEnclosure] can automatically generate slab
+and excludes based on minkowski sums instead of only vector based sizing.
 
-:py:func:~`fill_tiled` provides a filling algorithm that can use the
-:py:class:~`klayout.db.TilingProcessor` to calculate the regions to fill.
+[fill_tiled][kfactory.utils.fill_tiled] provides a filling algorithm that can use
+the `klayout.db.TilingProcessor` to calculate the regions to fill.
 
-:py:func:~`fix_spacing` uses a region space check to calculate areas that violate
-min space violations. :py:func:~`fix_spacing_tiled` to fix it using a TilingProcessor.
+[fix_spacing][kfactory.utils.violations.fix_spacing_tiled] uses a region space check to
+calculate areas that violate min space violations.
 """
 
 from .enclosure import (
     Direction,
-    Enclosure,
+    KCellEnclosure,
+    LayerEnclosure,
     clean_points,
     extrude_path,
     extrude_path_dynamic,
 )
 from .fill import fill_tiled
 from .violations import fix_spacing_minkowski_tiled, fix_spacing_tiled
 
 __all__ = [
-    "Enclosure",
+    "LayerEnclosure",
+    "KCellEnclosure",
     "violations",
     "Direction",
     "geo",
     "extrude_path",
     "extrude_path_dynamic",
     "fill_tiled",
     "fix_spacing_tiled",
```

### Comparing `kfactory-0.6.3/src/kfactory/utils/enclosure.py` & `kfactory-0.7.0/src/kfactory/utils/enclosure.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """Enclosure module.
 
 Enclosures allow to calculate slab/excludes and similar concepts to an arbitrary
 shape located on a main_layer or reference layer or region.
 """
 
-import os
-from collections.abc import Callable, Sequence
+from collections.abc import Callable, Iterable, Iterator, Sequence
 from enum import IntEnum
 from hashlib import sha1
-from typing import Any, Optional, TypeGuard
+from typing import Any, Optional, TypeGuard, overload
 
 import numpy as np
-from pydantic import BaseModel, Field, PrivateAttr
+from pydantic import BaseModel, Field, PrivateAttr, validator
 
 from .. import kdb
-from ..config import logger
-from ..kcell import KCell, LayerEnum
+from ..conf import config
+from ..kcell import KCell, LayerEnum, Port
+from ..port import filter_layer
 
 __all__ = [
-    "Enclosure",
+    "LayerEnclosure",
+    "KCellEnclosure",
     "extrude_path",
     "extrude_path_points",
     "extrude_path_dynamic",
     "extrude_path_dynamic_points",
 ]
 
 
@@ -150,15 +151,15 @@
 
 
 def extrude_path(
     target: KCell,
     layer: LayerEnum | int,
     path: list[kdb.DPoint],
     width: float,
-    enclosure: Optional["Enclosure"] = None,
+    enclosure: Optional["LayerEnclosure"] = None,
     start_angle: float | None = None,
     end_angle: float | None = None,
 ) -> None:
     """Extrude a path from a list of points and a static width.
 
     Args:
         target: the cell where to insert the shapes to (and get the database unit from)
@@ -185,30 +186,30 @@
     for layer, layer_sec in layer_list.items():
         reg = kdb.Region()
         for section in layer_sec.sections:
             _r = kdb.Region(
                 path_pts_to_polygon(
                     *extrude_path_points(
                         path,
-                        width + 2 * section.d_max * target.klib.dbu,
+                        width + 2 * section.d_max * target.kcl.dbu,
                         start_angle,
                         end_angle,
                     )
-                ).to_itype(target.klib.dbu)
+                ).to_itype(target.kcl.dbu)
             )
             if section.d_min is not None:
                 _r -= kdb.Region(
                     path_pts_to_polygon(
                         *extrude_path_points(
                             path,
-                            width + 2 * section.d_min * target.klib.dbu,
+                            width + 2 * section.d_min * target.kcl.dbu,
                             start_angle,
                             end_angle,
                         )
-                    ).to_itype(target.klib.dbu)
+                    ).to_itype(target.kcl.dbu)
                 )
             reg.insert(_r)
         target.shapes(layer).insert(reg.merge())
 
 
 def extrude_path_dynamic_points(
     path: list[kdb.DPoint],
@@ -285,15 +286,15 @@
 
 
 def extrude_path_dynamic(
     target: KCell,
     layer: LayerEnum | int,
     path: list[kdb.DPoint],
     widths: Callable[[float], float] | list[float],
-    enclosure: Optional["Enclosure"] = None,
+    enclosure: Optional["LayerEnclosure"] = None,
     start_angle: float | None = None,
     end_angle: float | None = None,
 ) -> None:
     """Extrude a path with dynamic width.
 
     Extrude from a list of points and a list of widths and add an enclosure if
         specified.
@@ -324,92 +325,90 @@
         for layer, layer_sec in layer_list.items():
             reg = kdb.Region()
             for section in layer_sec.sections:
 
                 def w_max(x: float) -> float:
                     return (
                         widths(x)  # type: ignore[operator]
-                        + 2 * section.d_max * target.klib.dbu
+                        + 2 * section.d_max * target.kcl.dbu
                     )
 
                 _r = kdb.Region(
                     path_pts_to_polygon(
                         *extrude_path_dynamic_points(
                             path,
                             w_max,
                             start_angle,
                             end_angle,
                         )
-                    ).to_itype(target.klib.dbu)
+                    ).to_itype(target.kcl.dbu)
                 )
                 if section.d_min is not None:
 
                     def w_min(x: float) -> float:
                         return (
                             widths(x)  # type: ignore[operator]
                             + 2  # type: ignore[operator]
                             * section.d_min
-                            * target.klib.dbu
+                            * target.kcl.dbu
                         )
 
                     _r -= kdb.Region(
                         path_pts_to_polygon(
                             *extrude_path_dynamic_points(
                                 path,
                                 w_min,
                                 start_angle,
                                 end_angle,
                             )
-                        ).to_itype(target.klib.dbu)
+                        ).to_itype(target.kcl.dbu)
                     )
                 reg.insert(_r)
             target.shapes(layer).insert(reg.merge())
 
     else:
         for layer, layer_sec in layer_list.items():
             reg = kdb.Region()
             for section in layer_sec.sections:
                 max_widths = [
-                    w + 2 * section.d_max * target.klib.dbu
+                    w + 2 * section.d_max * target.kcl.dbu
                     for w in widths  # type: ignore[union-attr]
                 ]
                 _r = kdb.Region(
                     path_pts_to_polygon(
                         *extrude_path_dynamic_points(
                             path,
                             max_widths,
                             start_angle,
                             end_angle,
                         )
-                    ).to_itype(target.klib.dbu)
+                    ).to_itype(target.kcl.dbu)
                 )
                 if section.d_min is not None:
                     min_widths = [
-                        w + 2 * section.d_min * target.klib.dbu
+                        w + 2 * section.d_min * target.kcl.dbu
                         for w in widths  # type: ignore[union-attr]
                     ]
                     _r -= kdb.Region(
                         path_pts_to_polygon(
                             *extrude_path_dynamic_points(
                                 path,
                                 min_widths,
                                 start_angle,
                                 end_angle,
                             )
-                        ).to_itype(target.klib.dbu)
+                        ).to_itype(target.kcl.dbu)
                     )
                 reg.insert(_r)
             target.shapes(layer).insert(reg.merge())
 
 
 class Section(BaseModel):
     """Section of an Enclosure.
 
-    Visualization::
-
         Maximum only Section:
             ┌────────────────────────┐  ▲
             │                        │  │
             │  ┌──────────────────┐  │  │
             │  │                  │  │  │
             │  │    Reference     │  │  │ Section
             │  │                  │  │  │ (d_max only)
@@ -475,60 +474,91 @@
                         self.sections[i].d_min, sec.d_min  # type: ignore[type-var]
                     )
                     self.sections.pop(i)
                     if i == len(self.sections):
                         break
             self.sections.insert(i, sec)
 
+    def max_size(self) -> int:
+        """Maximum size of the sections in this layer section."""
+        return self.sections[-1].d_max
+
     def __hash__(self) -> int:
         """Unique hash of LayerSection."""
         return hash(tuple((s.d_min, s.d_max) for s in self.sections))
 
 
-class Enclosure(BaseModel):
+class LayerEnclosure(BaseModel):
     """Definitions for calculation of enclosing (or smaller) shapes of a reference.
 
     Attributes:
-        layer_sections: Mapping of layers to their :py:class;`LayerSection`
-
+        layer_sections: Mapping of layers to their layer sections.
+        main_layer: Layer which to use unless specified otherwise.
     """
 
     layer_sections: dict[LayerEnum | int, LayerSection]
-    _name: str | None = PrivateAttr(default=None)
-    warn: bool = True
-
+    _name: str | None = PrivateAttr()
     main_layer: LayerEnum | int | None
-
     yaml_tag: str = "!Enclosure"
 
     class Config:
         """pydantic config."""
 
         validate_assignment = True
 
     def __init__(
         self,
         sections: Sequence[
             tuple[LayerEnum | int, int] | tuple[LayerEnum | int, int, int]
         ] = [],
         name: str | None = None,
-        warn: bool = True,
         main_layer: LayerEnum | int | None = None,
+        dsections: Sequence[
+            tuple[LayerEnum | int, float] | tuple[LayerEnum | int, float, float]
+        ]
+        | None = None,
+        dbu: float | None = None,
     ):
-        """Constructor of new enclosure."""
+        """Constructor of new enclosure.
+
+        Args:
+            sections: tuples containing info for the enclosure.
+                Elements must be of the form (layer, max) or (layer, min, max)
+            name: Optional name of the enclosure. If a name is given in the
+                cell name this name will be used for enclosure arguments.
+            main_layer: Main layer used if the functions don't get an explicit layer.
+            dsections: Same as sections but min/max defined in um
+            dbu: `KCLayout.dbu` (conversion dbu -> um). Must be specified if
+                `desections` is not `None`.
+        """
         super().__init__(
-            warn=warn,
             layer_sections={},
+            _name=name,
             main_layer=main_layer,
         )
-
         self._name = name
 
         self.layer_sections = {}
 
+        if dsections is not None:
+            assert dbu is not None, "If sections in um are defined, dbu must be set"
+            sections = list(sections)
+            for section in dsections:
+                if len(section) == 2:
+                    sections.append((section[0], round(section[1] / dbu)))
+
+                elif len(section) == 3:
+                    sections.append(
+                        (
+                            section[0],
+                            round(section[1] / dbu),
+                            round(section[2] / dbu),  # type: ignore[misc]
+                        )
+                    )
+
         for sec in sorted(sections, key=lambda sec: (sec[0], sec[1])):
             if sec[0] in self.layer_sections:
                 ls = self.layer_sections[sec[0]]
             else:
                 ls = LayerSection()
                 self.layer_sections[sec[0]] = ls
             ls.add_section(Section(d_max=sec[1])) if len(sec) < 3 else ls.add_section(
@@ -537,29 +567,29 @@
 
     def __hash__(self) -> int:  # make hashable BaseModel subclass
         """Calculate a unique hash of the enclosure."""
         return hash(
             (str(self), self.main_layer, tuple(list(self.layer_sections.items())))
         )
 
-    def __add__(self, other: "Enclosure") -> "Enclosure":
+    def __add__(self, other: "LayerEnclosure") -> "LayerEnclosure":
         """Returns the merged enclosure of two enclosures."""
-        enc = Enclosure()
+        enc = LayerEnclosure()
 
         for layer, secs in self.layer_sections.items():
             for sec in secs.sections:
                 enc.add_section(layer, sec)
 
         for layer, secs in other.layer_sections.items():
             for sec in secs.sections:
                 enc.add_section(layer, sec)
 
         return enc
 
-    def __iadd__(self, other: "Enclosure") -> "Enclosure":
+    def __iadd__(self, other: "LayerEnclosure") -> "LayerEnclosure":
         """Allows merging another enclosure into this one."""
         for layer, secs in other.layer_sections.items():
             for sec in secs.sections:
                 self.add_section(layer, sec)
         return self
 
     def add_section(self, layer: LayerEnum | int, sec: Section) -> None:
@@ -574,14 +604,19 @@
         if layer in self.layer_sections:
             d[layer].add_section(sec)
         else:
             d[layer] = LayerSection(sections=[sec])
 
         self.layer_sections = d  # trick pydantic to validate
 
+    @property
+    def name(self) -> str:
+        """Get name of the Enclosure."""
+        return self.__str__()
+
     def minkowski_region(
         self,
         r: kdb.Region,
         d: int | None,
         shape: Callable[[int], list[kdb.Point] | kdb.Box | kdb.Edge | kdb.Polygon],
     ) -> kdb.Region:
         """Calculaste a region from a minkowski sum.
@@ -626,15 +661,15 @@
 
         This can be used for tapers/
         waveguides or similar that are straight.
 
         Args:
             c: Cell to apply the enclosure to.
             ref: Reference to use as a base for the enclosure.
-            direction: X/Y or both directions, see :py:class:~`DIRECTION`.
+            direction: X/Y or both directions.
                 Uses a box if both directions are selected.
         """
         match direction:
             case Direction.BOTH:
 
                 def box(d: int) -> kdb.Box:
                     return kdb.Box(-d, -d, d, d)
@@ -730,16 +765,17 @@
         Useful if the target is a big or complicated enclosure. Will split target ref
         into tiles and calculate them in parallel. Uses a circle as a shape for the
         minkowski sum.
 
         Args:
             c: Target KCell to apply the enclosures into.
             ref: The reference shapes to apply the enclosures to.
-                Can be a layer or a region. If `None`, it will trey to use the
-                :py:attr:`main_layer`
+                Can be a layer or a region. If `None`, it will try to use the
+                `main_layer` of the
+                [enclosure][kfactory.utils.enclosure.LayerEnclosure].
             tile_size: Tile size. This should be in the order off 10+ maximum size
                 of the maximum size of sections.
             n_pts: Number of points in the circle. < 3 will create a triangle. 4 a
                 diamond, etc.
             n_threads: Number o threads to use. By default (`None`) it will use as many
                 threads as are set to the process (usually all cores of the machine).
         """
@@ -749,40 +785,40 @@
             if ref is None:
                 raise ValueError(
                     "The enclosure doesn't have  a reference `main_layer` defined."
                     " Therefore the layer must be defined in calls"
                 )
         tp = kdb.TilingProcessor()
         tp.frame = c.dbbox()  # type: ignore[misc]
-        tp.dbu = c.klib.dbu
-        tp.threads = n_threads or len(os.sched_getaffinity(0))
+        tp.dbu = c.kcl.dbu
+        tp.threads = n_threads or config.n_threads
         maxsize = 0
         for layersection in self.layer_sections.values():
             maxsize = max(
                 maxsize, *[section.d_max for section in layersection.sections]
             )
 
         min_tile_size_rec = 10 * maxsize * tp.dbu
 
         if tile_size is None:
             tile_size = min_tile_size_rec * 2
 
         if float(tile_size) <= min_tile_size_rec:
-            logger.warning(
+            config.logger.warning(
                 "Tile size should be larger than the maximum of "
                 "the enclosures (recommendation: {} / {})",
                 tile_size,
                 min_tile_size_rec,
             )
 
         tp.tile_border(maxsize * tp.dbu, maxsize * tp.dbu)
 
         tp.tile_size(tile_size, tile_size)
         if isinstance(ref, int):
-            tp.input("main_layer", c.klib, c.cell_index(), ref)
+            tp.input("main_layer", c.kcl, c.cell_index(), ref)
         else:
             tp.input("main_layer", ref)
 
         operators = []
 
         for layer, sections in self.layer_sections.items():
             operator = RegionOperator(cell=c, layer=layer)
@@ -827,24 +863,24 @@
                     queue_str += (
                         f"_output(target_{layer}," "(max_reg - min_reg)& _tile, true);"
                     )
                 else:
                     queue_str += f"_output(target_{layer},max_reg & _tile, true);"
 
                 tp.queue(queue_str)
-                logger.debug(
+                config.logger.debug(
                     "String queued for {} on layer {}: {}", c.name, layer, queue_str
                 )
 
             operators.append((layer, operator))
 
-        c.klib.start_changes()
-        logger.info("Starting minkowski on {}", c.name)
+        c.kcl.start_changes()
+        config.logger.info("Starting minkowski on {}", c.name)
         tp.execute(f"Minkowski {c.name}")
-        c.klib.end_changes()
+        c.kcl.end_changes()
 
         for layer, operator in operators:
             operator.insert()
 
     def apply_custom(
         self,
         c: KCell,
@@ -865,15 +901,17 @@
 
     def apply_bbox(self, c: KCell, ref: int | kdb.Region | None = None) -> None:
         """Apply an enclosure based on a bounding box.
 
         Args:
             c: Target cell.
             ref: Reference layer or region (the bounding box). If `None` use
-                :py:attr:~`main_layer` if defined, else throw an error.
+                the `main_layer` of  the
+                [enclosure][kfactory.utils.enclosure.LayerEnclosure] if defined,
+                else throw an error.
         """
         if ref is None:
             ref = self.main_layer
 
             if ref is None:
                 raise ValueError(
                     "The enclosure doesn't have  a reference `main_layer` defined."
@@ -899,17 +937,18 @@
     @classmethod
     def to_yaml(cls, representer, node):  # type: ignore[no-untyped-def]
         """Get YAML representation of the enclosure."""
         d = dict(node.enclosures)
         return representer.represent_mapping(cls.yaml_tag, d)
 
     def __str__(self) -> str:
-        """String of enclosure. Use :py:attr:~`name`.
+        """String representation of an enclosure.
 
-        Use a hash of the sections and main_layer if the name is `None`.
+        Use [name][kfactory.utils.enclosure.LayerEnclosure.name]
+        if available. Use a hash of the sections and main_layer if the name is `None`.
         """
         if self._name is not None:
             return self._name
         list_to_hash: Any = [
             self.main_layer,
         ]
         for layer, layer_section in self.layer_sections.items():
@@ -918,29 +957,46 @@
 
     def extrude_path(
         self,
         c: KCell,
         path: list[kdb.DPoint],
         main_layer: int | LayerEnum | None,
         width: float,
+        start_angle: float | None = None,
+        end_angle: float | None = None,
     ) -> None:
         """Extrude a path and add it to a main layer.
 
+        Start and end angle should be set in relation to the orientation of the path.
+        If the path for example is starting E->W, the start angle should be 0 (if that
+        that is the desired angle). End angle is the same if the end
+        piece is stopping 2nd-last -> last in E->W.
+
         Args:
             c: The cell where to insert the path to
             path: Backbone of the path. [um]
             main_layer: Layer index where to put the main part of the path.
             width: Width of the core of the path
+            start_angle: angle of the start piece
+            end_angle: angle of the end piece
         """
         if main_layer is None:
             raise ValueError(
                 "The enclosure doesn't have  a reference `main_layer` defined."
                 " Therefore the layer must be defined in calls"
             )
-        extrude_path(target=c, layer=main_layer, path=path, width=width, enclosure=self)
+        extrude_path(
+            target=c,
+            layer=main_layer,
+            path=path,
+            width=width,
+            enclosure=self,
+            start_angle=start_angle,
+            end_angle=end_angle,
+        )
 
     def extrude_path_dynamic(
         self,
         c: KCell,
         path: list[kdb.DPoint],
         main_layer: int | LayerEnum | None,
         widths: Callable[[float], float] | list[float],
@@ -963,14 +1019,46 @@
                 " Therefore the layer must be defined in calls"
             )
         extrude_path_dynamic(
             target=c, layer=main_layer, path=path, widths=widths, enclosure=self
         )
 
 
+class LayerEnclosureCollection(BaseModel):
+    """Collection of LayerEnclosures."""
+
+    enclosures: list[LayerEnclosure]
+
+    @validator("enclosures", each_item=True)
+    def enclosures_must_have_main_layer(cls, v: LayerEnclosure) -> LayerEnclosure:
+        """The PDK Enclosure must have main layers defined for each Enclosure.
+
+        The PDK Enclosure uses this to automatically apply enclosures.
+        """
+        assert (
+            v.main_layer is not None
+        ), "Enclosure for PDKEnclosure must have a main layer defined"
+        return v
+
+    def __get_item__(self, key: str | int) -> LayerEnclosure:
+        """Retrieve enclosure by main layer."""
+        try:
+            return next(filter(lambda enc: enc.main_layer == key, self.enclosures))
+        except StopIteration:
+            raise KeyError(f"Unknown key {key}")
+
+    def __iter__(self) -> Iterator[LayerEnclosure]:  # type: ignore[override]
+        """Iterator over the LayerEnclosures."""
+        yield from self.enclosures
+
+    def __len__(self) -> int:
+        """Length of the LayerEnclosure list."""
+        return len(self.enclosures)
+
+
 class RegionOperator(kdb.TileOutputReceiver):
     """Region collector. Just getst the tile and inserts it into the target cell."""
 
     def __init__(self, cell: KCell, layer: LayerEnum | int) -> None:
         """Initialization.
 
         Args:
@@ -992,16 +1080,454 @@
     ) -> None:
         """Tiling Processor output call.
 
         Args:
             ix: x-axis index of tile.
             iy: y_axis index of tile.
             tile: The bounding box of the tile.
-            region: The target object of the :py:class:~`klayout.db.TilingProcessor`
+            region: The target object of the `klayout.db.TilingProcessor`
             dbu: dbu used by the processor.
             clip: Whether the target was clipped to the tile or not.
         """
         self.region.insert(region)
 
     def insert(self) -> None:
         """Insert the finished region into the cell."""
         self.kcell.shapes(self.layer).insert(self.region)
+
+
+class PortHoles(BaseModel):
+    """Calculates a region for holes from sizing and a list of ports."""
+
+    region: kdb.Region = Field(default_factory=kdb.Region)
+
+    def insert_ports(self, oversize: int, ports: Iterable[Port]) -> None:
+        """Add ports to carve out."""
+        for port in ports:
+            half_width = port.width // 2 + oversize
+            if port._trans:
+                self.region.insert(
+                    kdb.Polygon(
+                        kdb.Box(0, -half_width, half_width, half_width)
+                    ).transformed(port.trans)
+                )
+            else:
+                self.region.insert(
+                    kdb.Polygon(
+                        kdb.Box(0, -half_width, half_width, half_width)
+                    ).transformed(port.dcplx_trans.to_itrans(port.kcl.dbu))
+                )
+
+    # def calculate(self) -> None:
+    # """Calculate Region."""
+    # for port in self.ports:
+    #     half_width = port.width // 2 + self.oversize
+    #     if port._trans:
+    #         self.region.insert(
+    #             kdb.Polygon(
+    #                 kdb.Box(0, -half_width, half_width, half_width)
+    #             ).transformed(port.trans)
+    #         )
+    #     else:
+    #         self.region.insert(
+    #             kdb.Polygon(
+    #                 kdb.Box(0, -half_width, half_width, half_width)
+    #             ).transformed(port.dcplx_trans.to_itrans(port.kcl.dbu))
+    #         )
+
+    class Config:
+        """pydantic config."""
+
+        allow_mutation = False
+        arbitrary_types_allowed = True
+
+
+class RegionTilesOperator(kdb.TileOutputReceiver):
+    """Region collector. Just getst the tile and inserts it into the target cell.
+
+    As it can be used multiple times for the same tile, it needs to merge when
+    inserting.
+    """
+
+    def __init__(
+        self,
+        cell: KCell,
+        layers: list[LayerEnum | int],
+    ) -> None:
+        """Initialization.
+
+        Args:
+            cell: Target cell.
+            layers: Target layers.
+        """
+        self.kcell = cell
+        self.layers = layers
+        self.regions: dict[int, dict[int, kdb.Region]] = {}
+        self.merged_region: kdb.Region = kdb.Region()
+        self.merged = False
+
+    def put(
+        self,
+        ix: int,
+        iy: int,
+        tile: kdb.Box,
+        region: kdb.Region,
+        dbu: float,
+        clip: bool,
+    ) -> None:
+        """Tiling Processor output call.
+
+        Args:
+            ix: x-axis index of tile.
+            iy: y_axis index of tile.
+            tile: The bounding box of the tile.
+            region: The target object of the `klayout.db.TilingProcessor`
+            dbu: dbu used by the processor.
+            clip: Whether the target was clipped to the tile or not.
+        """
+        if ix not in self.regions:
+            self.regions[ix] = {}
+        if iy not in self.regions[ix]:
+            self.regions[ix][iy] = kdb.Region()
+        reg = self.regions[ix][iy]
+        reg.insert(region)
+        reg.merge()
+
+    def merge_region(self) -> None:
+        """Create one region from the individual tiles."""
+        for dicts in self.regions.values():
+            for reg in dicts.values():
+                self.merged_region += reg
+
+    @overload
+    def insert(self) -> None:
+        ...
+
+    @overload
+    def insert(self, port_hole_map: dict[int, PortHoles]) -> None:
+        ...
+
+    def insert(
+        self,
+        port_hole_map: dict[int, PortHoles] | None = None,
+    ) -> None:
+        """Insert the finished region into the cell.
+
+        Args:
+            port_hole_map: Carve out holes around the ports.
+        """
+        if not self.merged:
+            self.merge_region()
+
+        if port_hole_map:
+            for layer in self.layers:
+                carved_region = self.merged_region - port_hole_map[layer].region
+                self.kcell.shapes(layer).insert(carved_region)
+        else:
+            for layer in self.layers:
+                self.kcell.shapes(layer).insert(self.merged_region)
+
+
+class KCellEnclosure(BaseModel):
+    """Collection of [enclosures][kfactory.utils.enclosure.LayerEnclosure] for cells."""
+
+    enclosures: LayerEnclosureCollection
+
+    def __init__(self, enclosures: Iterable[LayerEnclosure]):
+        """Init. Allow usage of an iterable object instead of a collection."""
+        super().__init__(enclosures=LayerEnclosureCollection(enclosures=enclosures))
+
+    def minkowski_region(
+        self,
+        r: kdb.Region,
+        d: int | None,
+        shape: Callable[[int], list[kdb.Point] | kdb.Box | kdb.Edge | kdb.Polygon],
+    ) -> kdb.Region:
+        """Calculaste a region from a minkowski sum.
+
+        If the distance is negative, the function will take the inverse region and apply
+        the minkowski and take the inverse again.
+
+        Args:
+            r: Target region.
+            d: Distance to pass to the shape. Can be any integer. [dbu]
+            shape: Function returning a shape for the minkowski region.
+        """
+        if d is None:
+            return kdb.Region()
+        elif d == 0:
+            return r.dup()
+        elif d > 0:
+            return r.minkowski_sum(shape(d))
+        else:
+            _shape = shape(abs(d))
+            if isinstance(_shape, list):
+                box_shape = kdb.Polygon(_shape)
+                bbox_maxsize = max(
+                    box_shape.bbox().width(),
+                    box_shape.bbox().height(),
+                )
+            else:
+                bbox_maxsize = max(
+                    _shape.bbox().width(),
+                    _shape.bbox().height(),
+                )
+            bbox_r = kdb.Region(r.bbox().enlarged(bbox_maxsize))
+            return r - (bbox_r - r).minkowski_sum(_shape)
+
+    def apply_minkowski_enc(
+        self,
+        c: KCell,
+        direction: Direction = Direction.BOTH,
+    ) -> None:
+        """Apply an enclosure with a vector in y-direction.
+
+        This can be used for tapers/
+        waveguides or similar that are straight.
+
+        Args:
+            c: Cell to apply the enclosure to.
+            direction: X/Y or both directions, see [kfactory.utils.enclosure.DIRECTION].
+                Uses a box if both directions are selected.
+        """
+        match direction:
+            case Direction.BOTH:
+
+                def box(d: int) -> kdb.Box:
+                    return kdb.Box(-d, -d, d, d)
+
+                self.apply_minkowski_custom(c, shape=box)
+
+            case Direction.Y:
+
+                def edge(d: int) -> kdb.Edge:
+                    return kdb.Edge(0, -d, 0, d)
+
+                self.apply_minkowski_custom(c, shape=edge)
+
+            case Direction.X:
+
+                def edge(d: int) -> kdb.Edge:
+                    return kdb.Edge(-d, 0, d, 0)
+
+                self.apply_minkowski_custom(c, shape=edge)
+
+            case _:
+                raise ValueError("Undefined direction")
+
+    def apply_minkowski_y(self, c: KCell) -> None:
+        """Apply an enclosure with a vector in y-direction.
+
+        This can be used for tapers/
+        waveguides or similar that are straight.
+
+        Args:
+            c: Cell to apply the enclosure to.
+        """
+        return self.apply_minkowski_enc(c, direction=Direction.Y)
+
+    def apply_minkowski_x(self, c: KCell) -> None:
+        """Apply an enclosure with a vector in x-direction.
+
+        This can be used for tapers/
+        waveguides or similar that are straight.
+
+        Args:
+            c: Cell to apply the enclosure to.
+        """
+        return self.apply_minkowski_enc(c, direction=Direction.X)
+
+    def apply_minkowski_custom(
+        self,
+        c: KCell,
+        shape: Callable[[int], kdb.Edge | kdb.Polygon | kdb.Box],
+    ) -> None:
+        """Apply an enclosure with a custom shape.
+
+        This can be used for tapers/
+        waveguides or similar that are straight.
+
+        Args:
+            c: Cell to apply the enclosure to.
+            shape: A function that will return a shape which takes one argument
+                the size of the section in dbu.
+            shape: Reference to use as a base for the enclosure.
+        """
+        regions = {}
+
+        for enc in self.enclosures:
+            if not c.bbox_per_layer(enc.main_layer).empty():
+                rsi = c.begin_shapes_rec(enc.main_layer)
+                for layer, layersec in enc.layer_sections.items():
+                    if layer not in regions:
+                        reg = kdb.Region()
+                        regions[layer] = reg
+                    else:
+                        reg = regions[layer]
+                    for section in layersec.sections:
+                        reg += self.minkowski_region(
+                            rsi, section.d_max, shape
+                        ) - self.minkowski_region(rsi, section.d_min, shape)
+
+                        reg.merge()
+
+        for layer, region in regions.items():
+            c.shapes(layer).insert(region)
+
+    def apply_minkowski_tiled(
+        self,
+        c: KCell,
+        tile_size: float | None = None,
+        n_pts: int = 64,
+        n_threads: int | None = None,
+        carve_out_ports: bool = True,
+    ) -> None:
+        """Minkowski regions with tiling processor.
+
+        Useful if the target is a big or complicated enclosure. Will split target ref
+        into tiles and calculate them in parallel. Uses a circle as a shape for the
+        minkowski sum.
+
+        Args:
+            c: Target KCell to apply the enclosures into.
+            tile_size: Tile size. This should be in the order off 10+ maximum size
+                of the maximum size of sections.
+            n_pts: Number of points in the circle. < 3 will create a triangle. 4 a
+                diamond, etc.
+            n_threads: Number o threads to use. By default (`None`) it will use as many
+                threads as are set to the process (usually all cores of the machine).
+            carve_out_ports: Carves out a box of port_width +
+        """
+        tp = kdb.TilingProcessor()
+        tp.frame = c.dbbox()  # type: ignore[misc]
+        tp.dbu = c.kcl.dbu
+        tp.threads = n_threads or config.n_threads
+        inputs: set[int] = set()
+        port_hole_map: dict[int, PortHoles] = {}
+
+        for enc in self.enclosures:
+            maxsize = 0
+            assert enc.main_layer is not None
+            for layer, layersection in enc.layer_sections.items():
+                size = layersection.sections[-1].d_max
+                maxsize = max(maxsize, size)
+
+                if layer in port_hole_map:
+                    port_hole_map[layer].insert_ports(
+                        size, filter_layer(c.ports, enc.main_layer)
+                    )
+                else:
+                    _port_holes = PortHoles()
+                    _port_holes.insert_ports(
+                        size, filter_layer(c.ports, enc.main_layer)
+                    )
+                    port_hole_map[layer] = _port_holes
+
+        min_tile_size_rec = 10 * maxsize * tp.dbu
+
+        if tile_size is None:
+            tile_size = min_tile_size_rec * 2
+
+        if float(tile_size) <= min_tile_size_rec:
+            config.logger.warning(
+                "Tile size should be larger than the maximum of "
+                "the enclosures (recommendation: {} / {})",
+                tile_size,
+                min_tile_size_rec,
+            )
+        tp.tile_border(maxsize * tp.dbu, maxsize * tp.dbu)
+        tp.tile_size(tile_size, tile_size)
+
+        for i, enc in enumerate(self.enclosures):
+            assert enc.main_layer is not None
+            if not c.bbox_per_layer(enc.main_layer).empty():
+                _inp = f"main_layer_{enc.main_layer}"
+                if enc.main_layer not in inputs:
+                    tp.input(f"{_inp}", c.kcl, c.cell_index(), enc.main_layer)
+                    inputs.add(enc.main_layer)
+                    config.logger.debug("Created input {}", _inp)
+
+                layer_regiontilesoperators: dict[LayerSection, RegionTilesOperator] = {}
+
+                for layer, layer_section in enc.layer_sections.items():
+                    if layer_section in layer_regiontilesoperators:
+                        layer_regiontilesoperators[layer_section].layers.append(layer)
+                    else:
+                        _out = f"target_{layer}"
+                        operator = RegionTilesOperator(cell=c, layers=[layer])
+                        layer_regiontilesoperators[layer_section] = operator
+                        tp.output(_out, operator)
+                        config.logger.debug("Created output {}", _out)
+
+                        for i, section in enumerate(reversed(layer_section.sections)):
+                            queue_str = (
+                                "var max_shape = Polygon.ellipse("
+                                f"Box.new({section.d_max*2},{section.d_max*2}),"
+                                f" {n_pts});"
+                            )
+                            match section.d_max:
+                                case d if d > 0:
+                                    max_region = (
+                                        "var max_reg = "
+                                        f"{_inp}.minkowski_sum(max_shape).merged();"
+                                    )
+                                case d if d < 0:
+                                    max_region = (
+                                        f"var tile_reg = _tile &"
+                                        f" _frame.sized({maxsize});"
+                                        "var max_reg = tile_reg - "
+                                        f"(tile_reg - {_inp});"
+                                    )
+                                case 0:
+                                    max_region = (
+                                        "var tile_reg = _tile & "
+                                        f"_frame.sized({maxsize});"
+                                        f"var max_reg = {_inp} & tile_reg;"
+                                    )
+                            queue_str += max_region
+                            if section.d_min:
+                                queue_str += (
+                                    "var min_shape = Polygon.ellipse("
+                                    f"Box.new({section.d_min*2},{section.d_min*2}),"
+                                    " 64);"
+                                )
+                                match section.d_min:
+                                    case d if d > 0:
+                                        min_region = (
+                                            "var min_reg = "
+                                            f"{_inp}.minkowski_sum(min_shape);"
+                                        )
+                                    case d if d < 0:
+                                        min_region = (
+                                            "var min_reg = tile_reg - (tile_reg - "
+                                            f"{_inp}).minkowski_sum(min_shape);"
+                                        )
+                                    case 0:
+                                        min_region = f"var min_reg = {_inp} & tile_reg;"
+                                queue_str += min_region
+                                queue_str += (
+                                    f"_output({_out},"
+                                    "(max_reg - min_reg) & _tile, true);"
+                                )
+                            else:
+                                queue_str += f"_output({_out}, max_reg & _tile, true);"
+
+                            tp.queue(queue_str)
+                            config.logger.debug(
+                                "String queued for {} on layer {}: '{}'",
+                                c.name,
+                                layer,
+                                queue_str,
+                            )
+
+        c.kcl.start_changes()
+        config.logger.info("Starting minkowski on {}", c.name)
+        tp.execute(f"Minkowski {c.name}")
+        c.kcl.end_changes()
+
+        if carve_out_ports:
+            for operator in layer_regiontilesoperators.values():
+                for layer in operator.layers:
+                    operator.insert(port_hole_map=port_hole_map)
+        else:
+            for operator in layer_regiontilesoperators.values():
+                operator.insert()
```

### Comparing `kfactory-0.6.3/src/kfactory/utils/simplify.py` & `kfactory-0.7.0/src/kfactory/utils/simplify.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.3/src/kfactory/utils/violations.py` & `kfactory-0.7.0/src/kfactory/utils/violations.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 minimum space violations and then applies a fix.
 """
 
 import os
 from typing import overload
 
 from .. import KCell, LayerEnum, kdb
-from ..config import logger
+from ..conf import logger
 
 __all__ = [
     "fix_spacing_tiled",
     "fix_spacing_sizing_tiled",
     "fix_spacing_minkowski_tiled",
 ]
 
@@ -89,22 +89,22 @@
 
     Returns:
         fix: Region containing the fixes for the violations
 
     """
     if tile_size is None:
         min(25 * min_space, 250)
-        tile_size = (30 * min_space * c.klib.dbu, 30 * min_space * c.klib.dbu)
+        tile_size = (30 * min_space * c.kcl.dbu, 30 * min_space * c.kcl.dbu)
 
     tp = kdb.TilingProcessor()
-    tp.frame = c.bbox_per_layer(layer).to_dtype(c.klib.dbu)  # type: ignore[misc]
-    tp.dbu = c.klib.dbu
+    tp.frame = c.bbox_per_layer(layer).to_dtype(c.kcl.dbu)  # type: ignore[misc]
+    tp.dbu = c.kcl.dbu
     tp.tile_size(*tile_size)  # tile size in um
     tp.tile_border(min_space * overlap * tp.dbu, min_space * overlap * tp.dbu)
-    tp.input("reg", c.klib, c.cell_index(), layer)
+    tp.input("reg", c.kcl, c.cell_index(), layer)
     tp.threads = n_threads or len(os.sched_getaffinity(0))
 
     fix_reg = RegionOperator()
     tp.output("fix_reg", fix_reg)
 
     if smooth_factor != 0 or smooth_absolute:
         keep = "true" if smooth_keep_hv else "false"
@@ -134,17 +134,17 @@
             " + sc.polygons()); r_int.merge();"
             " r_int.insert(reg.interacting(sc.polygons()));"
             "r_int.merge(); _output(fix_reg, r_int)"
         )
 
     tp.queue(queue_str)
 
-    c.klib.start_changes()
+    c.kcl.start_changes()
     tp.execute("Min Space Fix")
-    c.klib.end_changes()
+    c.kcl.end_changes()
 
     return fix_reg.region
 
 
 def fix_spacing_sizing_tiled(
     c: KCell,
     min_space: int,
@@ -155,51 +155,50 @@
 ) -> kdb.Region:
     """Fix min space issues by using a dilation & erosion.
 
     Args:
         c: Input cell
         min_space: Minimum space rule [dbu]
         layer: Input layer index
-        metrics: The metrics to use to determine the violation edges
         n_threads: on how many threads to run the check simultaneously
         tile_size: tuple determining the size of each sub tile (in um), should be big
             compared to the violation size
         overlap: how many times bigger to make the tile border in relation to the
             violation size. Smaller than 1 can lead to errors
 
     Returns:
         kdb.Region: Region containing the fixes for the violations
 
     """
     tp = kdb.TilingProcessor()
     if tile_size is None:
-        size = min_space * 20 * c.klib.dbu
+        size = min_space * 20 * c.kcl.dbu
         tile_size = (size, size)
-    tp.frame = c.bbox_per_layer(layer).to_dtype(c.klib.dbu)  # type: ignore[misc]
-    tp.dbu = c.klib.dbu
+    tp.frame = c.bbox_per_layer(layer).to_dtype(c.kcl.dbu)  # type: ignore[misc]
+    tp.dbu = c.kcl.dbu
     tp.tile_size(*tile_size)  # tile size in um
     tp.tile_border(min_space * overlap * tp.dbu, min_space * overlap * tp.dbu)
-    tp.input("reg", c.klib, c.cell_index(), layer)
+    tp.input("reg", c.kcl, c.cell_index(), layer)
     tp.threads = n_threads or len(os.sched_getaffinity(0))
 
     fix_reg = kdb.Region()
 
     tp.output("fix_reg", fix_reg)
 
     queue_str = (
         "var tile_reg= reg & (_tile & _frame);"
         + f"reg = tile_reg.sized({min_space}).sized({-min_space});"
         + "_output(fix_reg, reg)"
     )
 
     tp.queue(queue_str)
 
-    c.klib.start_changes()
+    c.kcl.start_changes()
     tp.execute("Min Space Fix")
-    c.klib.end_changes()
+    c.kcl.end_changes()
 
     return fix_reg
 
 
 def fix_spacing_minkowski_tiled(
     c: KCell,
     min_space: int,
@@ -211,40 +210,39 @@
 ) -> kdb.Region:
     """Fix min space issues by using a dilation & erosion with a box.
 
     Args:
         c: Input cell
         min_space: Minimum space rule [dbu]
         ref: Input layer index or region
-        metrics: The metrics to use to determine the violation edges
         n_threads: on how many threads to run the check simultaneously
         tile_size: tuple determining the size of each sub tile (in um), should be big
             compared to the violation size
         overlap: how many times bigger to make the tile border in relation to the
             violation size. Smaller than 1 can lead to errors
         smooth: Apply smoothening (simplifying) at the end if > 0
 
     Returns:
         kdb.Region: Region containing the fixes for the violations
     """
     tp = kdb.TilingProcessor()
     tp.frame = c.dbbox()  # type: ignore[misc]
-    tp.dbu = c.klib.dbu
+    tp.dbu = c.kcl.dbu
     tp.threads = n_threads or len(os.sched_getaffinity(0))
 
     min_tile_size_rec = 10 * min_space * tp.dbu
 
     if tile_size is None:
         tile_size = (min_tile_size_rec * 2, min_tile_size_rec * 2)
 
     tp.tile_border(min_space * tp.dbu, min_space * tp.dbu)
 
     tp.tile_size(*tile_size)
     if isinstance(ref, int):
-        tp.input("main_layer", c.klib, c.cell_index(), ref)
+        tp.input("main_layer", c.kcl, c.cell_index(), ref)
     else:
         tp.input("main_layer", ref)
 
     operator = RegionOperator()
     tp.output("target", operator)
     queue_str = (
         f"var tile_reg = (_tile & _frame).sized({min_space});"
@@ -253,18 +251,18 @@
         "reg = tile_reg - (tile_reg - reg).minkowski_sum(shape);"
         "_output(target, reg & _tile, true);"
     )
 
     tp.queue(queue_str)
     logger.debug("String queued for {}:  {}", c.name, queue_str)
 
-    c.klib.start_changes()
+    c.kcl.start_changes()
     logger.info("Starting minkowski on {}", c.name)
     tp.execute(f"Minkowski {c.name}")
-    c.klib.end_changes()
+    c.kcl.end_changes()
 
     return operator.region
 
 
 class RegionOperator(kdb.TileOutputReceiver):
     """Region collector. Just getst the tile and inserts it into the target cell."""
```

### Comparing `kfactory-0.6.3/src/kfactory/widgets/interactive.py` & `kfactory-0.7.0/src/kfactory/widgets/interactive.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Interactivate jupyter widget."""
 
 try:
     from pathlib import Path
     from typing import Any
 
     from ipyevents import Event  # type: ignore[import]
-    from IPython.display import display  # type: ignore[import]
+    from IPython.display import Image as IPImage  # type: ignore[import]
+    from IPython.display import display
     from ipytree import Node, Tree  # type: ignore[import]
     from ipywidgets import (  # type: ignore[import]
         Accordion,
         AppLayout,
         Box,
         Button,
         HBox,
@@ -20,28 +21,88 @@
         RadioButtons,
         Tab,
         ToggleButtons,
         VBox,
     )
 
     from .. import kdb, lay
-    from ..config import logger
+    from ..conf import config
     from ..kcell import KCell
 
 except ImportError as e:
     print("You need install jupyter notebook plugin with `pip install kfactory[ipy]`")
     raise e
 
 
 def display_kcell(kc: KCell) -> None:
-    cell_dup = kc.klib.dup()[kc.name]
+    cell_dup = kc.kcl.dup()[kc.name]
     cell_dup.draw_ports()
 
-    lw = LayoutWidget(cell=cell_dup)
-    display(lw.widget)
+    match config.display_type:
+        case "widget":
+            lw = LayoutWidget(cell=cell_dup)
+            display(lw.widget)
+        case "image":
+            lipi = LayoutIPImage(cell=cell_dup)
+            display(lipi.image)
+
+
+class LayoutImage:
+    def __init__(
+        self,
+        cell: KCell,
+        layer_properties: str | None = None,
+    ):
+        self.layout_view = lay.LayoutView()
+        self.layout_view.show_layout(cell.kcl, False)
+        self.layer_properties: Path | None = None
+        if layer_properties is not None:
+            self.layer_properties = Path(layer_properties)
+            if self.layer_properties.exists() and self.layer_properties.is_file():
+                self.layer_properties = self.layer_properties
+                self.layout_view.load_layer_props(str(self.layer_properties))
+        self.show_cell(cell._kdb_cell)
+        png_data = self.layout_view.get_screenshot_pixels().to_png_data()
+
+        self.image = Image(value=png_data, format="png")
+
+    def show_cell(self, cell: kdb.Cell) -> None:
+        self.layout_view.active_cellview().cell = cell
+        self.layout_view.max_hier()
+        self.layout_view.resize(800, 600)
+        self.layout_view.add_missing_layers()
+        self.layout_view.zoom_fit()
+
+
+class LayoutIPImage:
+    def __init__(
+        self,
+        cell: KCell,
+        layer_properties: str | None = None,
+    ):
+        self.layout_view = lay.LayoutView()
+        self.layout_view.show_layout(cell.kcl, False)
+        self.layer_properties: Path | None = None
+        if layer_properties is not None:
+            self.layer_properties = Path(layer_properties)
+            if self.layer_properties.exists() and self.layer_properties.is_file():
+                self.layer_properties = self.layer_properties
+                self.layout_view.load_layer_props(str(self.layer_properties))
+        self.show_cell(cell._kdb_cell)
+        png_data = self.layout_view.get_screenshot_pixels().to_png_data()
+        self.image = IPImage(
+            data=png_data, format="png", embed=True, width=800, height=600
+        )
+
+    def show_cell(self, cell: kdb.Cell) -> None:
+        self.layout_view.active_cellview().cell = cell
+        self.layout_view.max_hier()
+        self.layout_view.resize(800, 600)
+        self.layout_view.add_missing_layers()
+        self.layout_view.zoom_fit()
 
 
 class LayoutWidget:
     def __init__(
         self,
         cell: KCell,
         layer_properties: str | None = None,
@@ -49,15 +110,15 @@
         with_layer_selector: bool = True,
     ):
         self.debug = Output()
 
         self.hide_unused_layers = hide_unused_layers
 
         self.layout_view = lay.LayoutView()
-        self.layout_view.show_layout(cell.klib, False)
+        self.layout_view.show_layout(cell.kcl, False)
         self.layer_properties: Path | None = None
         if layer_properties is not None:
             self.layer_properties = Path(layer_properties)
             if self.layer_properties.exists() and self.layer_properties.is_file():
                 self.layer_properties = self.layer_properties
                 self.layout_view.load_layer_props(str(self.layer_properties))
         self.show_cell(cell._kdb_cell)
@@ -101,15 +162,15 @@
             self.layout_view.switch_mode(buttons.value)
             self.refresh()
 
         self.widget = AppLayout(
             left_sidebar=mode_selector,
             center=self.image,
             right_sidebar=selector_tabs,
-            align_items="top",
+            connect_items="top",
             justify_items="center",
             footer=self.debug,
             # footer=mode_selector,
             pane_weights=[1, 3, 1],
         )
 
     def show_cell(self, cell: kdb.Cell) -> None:
@@ -122,15 +183,15 @@
     def button_toggle(self, button: Button) -> None:
         button.style.button_color = (
             "transparent"
             if (button.style.button_color == button.default_color)
             else button.default_color
         )
 
-        logger.info("button toggle")
+        config.logger.info("button toggle")
         for props in self.layout_view.each_layer():
             if props == button.layer_props:
                 props.visible = not props.visible
                 props.name = button.name
                 button.layer_props = props
                 break
         self.refresh()
```

### Comparing `kfactory-0.6.3/src/kfactory.egg-info/PKG-INFO` & `kfactory-0.7.0/src/kfactory.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: kfactory
-Version: 0.6.3
+Version: 0.7.0
 Summary: KLayout API implementation of gdsfactory
 Author-email: gdsfactory community <contact@gdsfactory.com>
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Provides-Extra: git
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: ci
 Provides-Extra: ipy
 License-File: LICENSE
 
-# KFactory 0.6.3
+# KFactory 0.7.0
 
 Kfactory is a [gdsfactory](https://github.com/gdsfactory/gdsfactory)-like tool. It is built with [KLayout](https://klayout.de) as a backend instead of gdstk, but aims to offer the similar featuers.
 
 Features similar to gdsfactory:
 
 - [x] Cells & decorator for caching & storing cells
 - [x] Simple routing (point to point and simpl bundle routes for electrical routes)
```

### Comparing `kfactory-0.6.3/tests/test_cplxcells.py` & `kfactory-0.7.0/tests/test_cplxcells.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import kfactory as kf
 
 
-@kf.autocell
+@kf.cell
 def simple_cplx_cell(layer: kf.LayerEnum) -> kf.KCell:
     c = kf.KCell()
 
     hh = 2.5
 
     dct = kf.kdb.DCplxTrans(1, 30, False, 2.5, 2.5)
     dbox = kf.kdb.DPolygon(kf.kdb.DBox(0, -hh, 10, hh)).transformed(dct)
@@ -29,16 +29,18 @@
     c.shapes(layer).insert(dbox)
 
     c.draw_ports()
     return c
 
 
 def test_cell(LAYER: kf.LayerEnum):
-    simple_cplx_cell(LAYER.WG)
+    c = simple_cplx_cell(LAYER.WG)
+    c.show()
 
 
 def test_connected_cell(LAYER: kf.LayerEnum):
     c = kf.KCell()
     layer = LAYER.WG
     sckc1 = c << simple_cplx_cell(layer)
     sckc2 = c << simple_cplx_cell(layer)
-    sckc2.align("o1", sckc1, "o1")
+    sckc2.connect("o1", sckc1, "o1")
+    c.show()
```

### Comparing `kfactory-0.6.3/tests/test_extrude.py` & `kfactory-0.7.0/tests/test_extrude.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 import kfactory as kf
 from kfactory.utils import extrude_path, extrude_path_dynamic
 import numpy as np
 
 
-@kf.autocell
+@kf.cell
 def taper_dyn(
-    length: float, width: float, layer: kf.LayerEnum, enclosure: kf.utils.Enclosure
+    length: float, width: float, layer: kf.LayerEnum, enclosure: kf.utils.LayerEnclosure
 ) -> kf.KCell:
     c = kf.KCell()
 
     path = [kf.kdb.DPoint(x, 0) for x in range(21)]
     _width = lambda x: width + width * np.sin(x * np.pi / 2)
 
     extrude_path_dynamic(c, layer, path, _width, enclosure)
 
+    c.show()
+
     return c
 
 
-@kf.autocell
+@kf.cell
 def taper_static(
-    length: float, width: float, layer: kf.LayerEnum, enclosure: kf.utils.Enclosure
+    length: float, width: float, layer: kf.LayerEnum, enclosure: kf.utils.LayerEnclosure
 ) -> kf.KCell:
     c = kf.KCell()
 
     path = [kf.kdb.DPoint(x, 0) for x in range(21)]
 
     _width = [width + np.sin(x * np.pi / 2) for x in [_x / 20 for _x in range(21)]]
     extrude_path_dynamic(c, layer, path, _width, enclosure)
+    c.show()
 
     return c
 
 
 def test_dynamic_sine_taper(LAYER, wg_enc):
     _taper = taper_dyn(10, 1, LAYER.WG, wg_enc)
 
@@ -45,19 +48,21 @@
     enclosure = wg_enc
     c = kf.KCell()
 
     path = [kf.kdb.DPoint(x, 0) for x in range(21)]
     _width = lambda x: width + width * np.sin(x * np.pi / 2)
 
     enclosure.extrude_path_dynamic(c, path, layer, _width)
+    c.show()
 
 
 def test_enc_extrude_static(LAYER, wg_enc):
     width = 10
     layer = LAYER.WG
     enclosure = wg_enc
     c = kf.KCell()
 
     path = [kf.kdb.DPoint(x, 0) for x in range(21)]
     _width = [width + np.sin(x * np.pi / 2) for x in [_x / 20 for _x in range(21)]]
 
     enclosure.extrude_path_dynamic(c, path, layer, _width)
+    c.show()
```

### Comparing `kfactory-0.6.3/tests/test_ports.py` & `kfactory-0.7.0/tests/test_ports.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import kfactory as kf
 import pytest
 import re
 
 
-@kf.autocell
+@kf.cell
 def waveguide(width: int, length: int, layer: int) -> kf.KCell:
     c = kf.KCell()
 
     c.shapes(layer).insert(kf.kdb.Box(0, -width // 2, length, width // 2))
 
     c.create_port(
         name="o1", trans=kf.kdb.Trans(2, False, 0, 0), width=width, layer=layer
@@ -20,19 +20,19 @@
 
 @pytest.fixture()
 def wg(LAYER):
     return waveguide(1000, 20000, LAYER.WG)
 
 
 @pytest.fixture()
-@kf.autocell
+@kf.cell
 def wg_floating_off_grid(LAYER):
     with pytest.raises(AssertionError):
         c = kf.KCell()
-        dbu = c.klib.dbu
+        dbu = c.kcl.dbu
 
         p1 = kf.kcell.Port(
             dwidth=10 + dbu / 2,
             name="o1",
             dcplx_trans=kf.kdb.DCplxTrans(1, 180, False, dbu / 2, 0),
             layer=LAYER.WG,
         )
@@ -43,15 +43,15 @@
             layer=LAYER.WG,
         )
         c.shapes(LAYER.WG).insert(kf.kdb.DBox(p1.x, -p1.width / 2, p2.x, p1.width / 2))
 
         c.add_port(p1)
         c.add_port(p2)
 
-        kf.config.filter.regex = None
+        kf.config.logfilter.regex = None
 
     return c
 
 
 def test_waveguide(LAYER):
     waveguide(1000, 20000, LAYER.WG)
 
@@ -69,46 +69,46 @@
     wg1 = c << waveguide(1000, 20000, LAYER.WG)
     port = kf.kcell.Port(
         dwidth=1,
         layer=LAYER.WG,
         name="cplxp1",
         dcplx_trans=kf.kdb.DCplxTrans(1, 30, False, 5, 10),
     )
-    wg1.align("o1", port)
+    wg1.connect("o1", port)
 
 
 def test_connect_cplx_inst(LAYER):
     c = kf.KCell()
 
     wg1 = c << waveguide(1000, 20000, LAYER.WG)
     wg2 = c << waveguide(1000, 20000, LAYER.WG)
     wg1.transform(kf.kdb.DCplxTrans(1, 30, False, 5, 10))
-    wg2.align("o1", wg1, "o2")
-    kf.config.filter.regex = f"Port ({re.escape(str(wg1.ports['o1']))}|{re.escape(str(wg2.ports['o2']))}) is not an integer based port, converting to integer based"
+    wg2.connect("o1", wg1, "o2")
+    kf.config.logfilter.regex = f"Port ({re.escape(str(wg1.ports['o1']))}|{re.escape(str(wg2.ports['o2']))}) is not an integer based port, converting to integer based"
 
     c.add_port(wg1.ports["o1"])
     c.add_port(wg2.ports["o2"])
 
-    kf.config.filter.regex = None
+    kf.config.logfilter.regex = None
     c.flatten()
 
 
 # def test_floating(wg_floating_off_grid):
 #     c = kf.KCell()
 
 #     wg1 = c << wg_floating_off_grid
 #     wg2 = c << wg_floating_off_grid
-#     wg2.align("o2", wg1, "o1")
+#     wg2.connect("o2", wg1, "o1")
 
 
 def test_connect_integer(wg):
     c = kf.KCell()
 
     wg1 = c << wg
     wg2 = c << wg
-    wg2.align("o1", wg1, "o1")
+    wg2.connect("o1", wg1, "o1")
 
     assert wg2.ports["o1"].trans == kf.kdb.Trans(0, False, 0, 0)
 
 
 # if __name__ == "__main__":
 #     test_waveguide()
```

### Comparing `kfactory-0.6.3/tests/test_rename.py` & `kfactory-0.7.0/tests/test_rename.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 port_x_coords = [-10000, 0, 0, 0, 10000]
 port_y_coords = [0, -10000, 0, 10000, 0]
 offset = 50000
 
 
-@kf.autocell
+@kf.cell
 def port_tests(rename_f: Optional[Callable[..., None]] = None) -> kf.KCell:
     c = kf.KCell()
 
     i = 0
     for angle in range(4):
         for x, y in zip(port_x_coords, port_y_coords):
             point = (
@@ -24,16 +24,16 @@
             c.create_port(
                 name=f"{i}",
                 trans=kf.kdb.Trans(
                     angle,
                     False,
                     point.to_v(),
                 ),
-                layer=c.klib.layer(1, 0),
-                width=1 / c.klib.dbu,
+                layer=c.kcl.layer(1, 0),
+                width=1 / c.kcl.dbu,
             )
     if rename_f is None:
         c.autorename_ports()
     else:
         c.autorename_ports(rename_f)
     c.draw_ports()
     return c
```

### Comparing `kfactory-0.6.3/tests/test_routing.py` & `kfactory-0.7.0/tests/test_routing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 import kfactory as kf
 import pytest
-import warnings
 from random import randint
 
-from typing import Callable
+from collections.abc import Callable
 
 
 @pytest.mark.parametrize(
     "x",
     [
         5000,
         0,
     ],
 )
-def test_connect_straight(
+def test_route_straight(
     x: int,
     bend90: kf.KCell,
     waveguide_factory: Callable[..., kf.KCell],
     LAYER: kf.LayerEnum,
     optical_port: kf.Port,
 ) -> None:
     c = kf.KCell()
     p1 = optical_port.copy()
     p2 = optical_port.copy()
     p2.trans = kf.kdb.Trans(2, False, x, 0)
-    kf.routing.optical.connect(
+    kf.routing.optical.route(
         c,
         p1,
         p2,
         straight_factory=waveguide_factory,
         bend90_cell=bend90,
     )
 
@@ -44,67 +43,66 @@
         (500, 500, 3),
         (-500, 30000, 3),
         (500, 30000, 3),
         (-10000, 30000, 3),
         (0, 0, 2),
     ],
 )
-def test_connect_bend90(
+def test_route_bend90(
     bend90: kf.KCell,
     waveguide_factory: Callable[..., kf.KCell],
     LAYER: kf.LayerEnum,
     optical_port: kf.Port,
     x: int,
     y: int,
     angle2: int,
 ) -> None:
     c = kf.KCell()
     p1 = optical_port.copy()
     p2 = optical_port.copy()
     p2.trans = kf.kdb.Trans(angle2, False, x, y)
     b90r = abs(bend90.ports._ports[0].x - bend90.ports._ports[1].x)
     if abs(x) < b90r or abs(y) < b90r:
-        kf.config.filter.regex = f"Potential collision in routing due to small distance between the port in relation to bend radius x={x}/{b90r}, y={y}/{b90r}"
-    kf.routing.optical.connect(
+        kf.config.logfilter.regex = f"Potential collision in routing due to small distance between the port in relation to bend radius x={x}/{b90r}, y={y}/{b90r}"
+    kf.routing.optical.route(
         c,
         p1,
         p2,
         straight_factory=waveguide_factory,
         bend90_cell=bend90,
     )
 
-    kf.config.filter.regex = None
+    kf.config.logfilter.regex = None
 
 
 @pytest.mark.parametrize(
     "x,y,angle2",
     [
         (40000, 40000, 2),
         (20000, 20000, 3),
         (10000, 10000, 3),
     ],
 )
-def test_connect_bend90_euler(
+def test_route_bend90_euler(
     bend90_euler: kf.KCell,
     waveguide_factory: Callable[..., kf.KCell],
     LAYER: kf.LayerEnum,
     optical_port: kf.Port,
     x: int,
     y: int,
     angle2: int,
 ) -> None:
     c = kf.KCell()
     p1 = optical_port.copy()
     p2 = optical_port.copy()
     p2.trans = kf.kdb.Trans(angle2, False, x, y)
     b90r = abs(bend90_euler.ports._ports[0].x - bend90_euler.ports._ports[1].x)
-    warnings.filterwarnings("error")
     if abs(x) < b90r or abs(y) < b90r:
-        kf.config.filter.regex = f"Potential collision in routing due to small distance between the port in relation to bend radius x={x}/{b90r}, y={y}/{b90r}"
-    kf.routing.optical.connect(
+        kf.config.logfilter.regex = f"Potential collision in routing due to small distance between the port in relation to bend radius x={x}/{b90r}, y={y}/{b90r}"
+    kf.routing.optical.route(
         c,
         p1,
         p2,
         straight_factory=waveguide_factory,
         bend90_cell=bend90_euler,
     )
-    kf.config.filter.regex = None
+    kf.config.logfilter.regex = None
```

### Comparing `kfactory-0.6.3/tests/test_spiral.py` & `kfactory-0.7.0/tests/test_spiral.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import warnings
 
 
 def bend_circular(
     width: int,
     radius: int,
     layer: int,
-    enclosure: Optional[kf.utils.Enclosure] = None,
+    enclosure: Optional[kf.utils.LayerEnclosure] = None,
     theta: int = 90,
     theta_step: float = 1,
 ) -> kf.KCell:
     """Circular radius bend
 
     Args:
         width: Width in database units
@@ -21,15 +21,15 @@
         layer: Layer index of the target layer
         enclosure: :py:class:`kfactory.utils.Enclosure` object to describe the claddings
     Returns:
         cell (KCell): Circular Bend KCell
     """
 
     c = kf.KCell()
-    r = radius * c.klib.dbu
+    r = radius * c.kcl.dbu
     backbone = [
         kf.kdb.DPoint(x, y)
         for x, y in [
             [np.sin(_theta / 180 * np.pi) * r, (-np.cos(_theta / 180 * np.pi) + 1) * r]
             for _theta in np.linspace(
                 0, theta, int(theta // theta_step + 0.5), endpoint=True
             )
@@ -61,15 +61,15 @@
     return c
 
 
 def dbend_circular(
     width: float,
     radius: float,
     layer: kf.kcell.LayerEnum,
-    enclosure: Optional[kf.utils.Enclosure] = None,
+    enclosure: Optional[kf.utils.LayerEnclosure] = None,
     theta: float = 90,
     theta_step: float = 1,
 ) -> kf.KCell:
     """Circular radius bend
 
     Args:
         width: Width in database units
@@ -129,32 +129,30 @@
     p = kf.Port(name="start", trans=kf.kdb.Trans.R0, width=1000, layer=LAYER.WG)
 
     for _ in range(10):
         r = r1 + r2
         r2 = r1
         r1 = r
         b = c << bend_circular(width=1000, radius=r2, layer=LAYER.WG)
-        b.align("W0", p)
+        b.connect("W0", p)
         p = b.ports["N0"]
 
 
 def test_dspiral(LAYER):
     c = kf.KCell()
 
     r1 = 1
     r2 = 0
 
     p = kf.Port(
         name="start", dcplx_trans=kf.kdb.DCplxTrans.R0, dwidth=1, layer=LAYER.WG
     )
 
-    kf.config.filter.level = "ERROR"
+    kf.config.logfilter.level = "ERROR"
 
     for _ in range(10):
         r = r1 + r2
         r2 = r1
         r1 = r
         b = c << dbend_circular(width=1, radius=r2, layer=LAYER.WG)
-        b.align("W0", p)
+        b.connect("W0", p)
         p = b.ports["N0"]
-
-    kf.config.filter.level = "DEBUG"
```

