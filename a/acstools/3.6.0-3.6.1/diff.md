# Comparing `tmp/acstools-3.6.0.tar.gz` & `tmp/acstools-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acstools-3.6.0.tar", last modified: Mon May  8 21:39:46 2023, max compression
+gzip compressed data, was "acstools-3.6.1.tar", last modified: Tue May 23 16:28:10 2023, max compression
```

## Comparing `acstools-3.6.0.tar` & `acstools-3.6.1.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:46.274543 acstools-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-08 21:39:07.000000 acstools-3.6.0/.bandit.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:46.254543 acstools-3.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:46.254543 acstools-3.6.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-08 21:39:07.000000 acstools-3.6.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-08 21:39:07.000000 acstools-3.6.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-08 21:39:07.000000 acstools-3.6.0/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-08 21:39:07.000000 acstools-3.6.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-08 21:39:07.000000 acstools-3.6.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-08 21:39:07.000000 acstools-3.6.0/.github/labeler.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:46.254543 acstools-3.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-05-08 21:39:07.000000 acstools-3.6.0/.github/workflows/ci_workflows.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-08 21:39:07.000000 acstools-3.6.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-08 21:39:07.000000 acstools-3.6.0/.github/workflows/open_actions.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-08 21:39:07.000000 acstools-3.6.0/.github/workflows/predeps_workflows.yml
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-08 21:39:07.000000 acstools-3.6.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-08 21:39:07.000000 acstools-3.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-08 21:39:07.000000 acstools-3.6.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-08 21:39:07.000000 acstools-3.6.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-08 21:39:07.000000 acstools-3.6.0/CITATION.md
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-05-08 21:39:07.000000 acstools-3.6.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-08 21:39:07.000000 acstools-3.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-08 21:39:07.000000 acstools-3.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-08 21:39:46.274543 acstools-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-08 21:39:07.000000 acstools-3.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:46.262543 acstools-3.6.0/acstools/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/acs2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    38670 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/acs_destripe.py
--rw-r--r--   0 runner    (1001) docker     (123)    26899 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/acs_destripe_plus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/acsccd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/acscte.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/acscteforwardmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    10631 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/acsphotcte.py
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/acsrej.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/acssum.py
--rw-r--r--   0 runner    (1001) docker     (123)    13247 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/acszpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/calacs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:46.262543 acstools-3.6.0/acstools/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/data/polarizer_tables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/data/rt_line_kernel_width15.fits
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/data/rt_line_kernel_width3.fits
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/data/rt_line_kernel_width7.fits
--rw-r--r--   0 runner    (1001) docker     (123)    52685 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/findsat_mrt.py
--rw-r--r--   0 runner    (1001) docker     (123)    16594 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/polarization_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    35084 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/satdet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:46.266543 acstools-3.6.0/acstools/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:46.246543 acstools-3.6.0/acstools/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:46.266543 acstools-3.6.0/acstools/tests/data/input/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/data/input/ja0x03ojq_flt.fits
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/data/input/jb5g05ubq_flt.fits
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/data/input/jc2z03cvq_blv_tmp.fits
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/data/input/jc5001soq_flt.fits
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/data/input/jc8m10syq_flc.fits
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/data/input/jc8m32j5q_flc.fits
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/data/input/jc8o04ghq_flt.fits
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/data/input/jc8o04ghq_mask1.fits
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/data/input/jc8o04ghq_mask2.fits
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:46.270543 acstools-3.6.0/acstools/tests/data/truth/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/data/truth/ja0x03ojq_flt_ref.fits
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/data/truth/jb5g05ubq_flt_ref.fits
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/data/truth/jc2z03cvq_blv_tmp_ref.fits
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/data/truth/jc5001soq_flt_ref.fits
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/data/truth/jc8m10syq_flc_ref.fits
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/data/truth/jc8m32j5q_flc_mask_ref.fits
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/data/truth/jc8o04ghq_flt_ref.fits
--rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/test_polarization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/test_wfc_destripe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/test_wfc_findsat_mrt.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/test_wfc_satdet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16780 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/utils_calib.py
--rw-r--r--   0 runner    (1001) docker     (123)    48734 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/utils_findsat_mrt.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-08 21:39:17.000000 acstools-3.6.0/acstools/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:46.262543 acstools-3.6.0/acstools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-08 21:39:17.000000 acstools-3.6.0/acstools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-08 21:39:46.000000 acstools-3.6.0/acstools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 21:39:17.000000 acstools-3.6.0/acstools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-08 21:39:17.000000 acstools-3.6.0/acstools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 21:39:17.000000 acstools-3.6.0/acstools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-08 21:39:17.000000 acstools-3.6.0/acstools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 21:39:17.000000 acstools-3.6.0/acstools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-08 21:39:07.000000 acstools-3.6.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:46.270543 acstools-3.6.0/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-05-08 21:39:07.000000 acstools-3.6.0/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-05-08 21:39:07.000000 acstools-3.6.0/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:46.274543 acstools-3.6.0/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:46.274543 acstools-3.6.0/doc/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    65413 2023-05-08 21:39:07.000000 acstools-3.6.0/doc/source/_static/stsci_pri_combo_mark_white.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:46.274543 acstools-3.6.0/doc/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:07.000000 acstools-3.6.0/doc/source/_templates/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-08 21:39:07.000000 acstools-3.6.0/doc/source/acs_destripe.rst
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-08 21:39:07.000000 acstools-3.6.0/doc/source/acsphotcte.rst
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-08 21:39:07.000000 acstools-3.6.0/doc/source/acszpt.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-05-08 21:39:07.000000 acstools-3.6.0/doc/source/calacs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-05-08 21:39:07.000000 acstools-3.6.0/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-08 21:39:07.000000 acstools-3.6.0/doc/source/findsat_mrt.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-08 21:39:07.000000 acstools-3.6.0/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-08 21:39:07.000000 acstools-3.6.0/doc/source/polarization_tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-08 21:39:07.000000 acstools-3.6.0/doc/source/satdet.rst
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-08 21:39:07.000000 acstools-3.6.0/doc/source/utils_calib.rst
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-08 21:39:07.000000 acstools-3.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-08 21:39:46.274543 acstools-3.6.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-05-08 21:39:07.000000 acstools-3.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:28:10.656798 acstools-3.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-23 16:27:24.000000 acstools-3.6.1/.bandit.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:28:10.644797 acstools-3.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:28:10.648797 acstools-3.6.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-23 16:27:24.000000 acstools-3.6.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-23 16:27:24.000000 acstools-3.6.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-23 16:27:24.000000 acstools-3.6.1/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-23 16:27:24.000000 acstools-3.6.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-23 16:27:24.000000 acstools-3.6.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-23 16:27:24.000000 acstools-3.6.1/.github/labeler.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:28:10.648797 acstools-3.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-05-23 16:27:24.000000 acstools-3.6.1/.github/workflows/ci_workflows.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-23 16:27:24.000000 acstools-3.6.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-23 16:27:24.000000 acstools-3.6.1/.github/workflows/open_actions.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-23 16:27:24.000000 acstools-3.6.1/.github/workflows/predeps_workflows.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-23 16:27:24.000000 acstools-3.6.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-23 16:27:24.000000 acstools-3.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-23 16:27:24.000000 acstools-3.6.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-23 16:27:24.000000 acstools-3.6.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-23 16:27:24.000000 acstools-3.6.1/CITATION.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-05-23 16:27:24.000000 acstools-3.6.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-23 16:27:24.000000 acstools-3.6.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-23 16:27:24.000000 acstools-3.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-23 16:28:10.656798 acstools-3.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-23 16:27:24.000000 acstools-3.6.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:28:10.648797 acstools-3.6.1/acstools/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-23 16:27:24.000000 acstools-3.6.1/acstools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-23 16:27:24.000000 acstools-3.6.1/acstools/acs2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38670 2023-05-23 16:27:24.000000 acstools-3.6.1/acstools/acs_destripe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26899 2023-05-23 16:27:24.000000 acstools-3.6.1/acstools/acs_destripe_plus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-23 16:27:24.000000 acstools-3.6.1/acstools/acsccd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-05-23 16:27:24.000000 acstools-3.6.1/acstools/acscte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-05-23 16:27:24.000000 acstools-3.6.1/acstools/acscteforwardmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10537 2023-05-23 16:27:24.000000 acstools-3.6.1/acstools/acsphotcte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-05-23 16:27:24.000000 acstools-3.6.1/acstools/acsrej.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-23 16:27:24.000000 acstools-3.6.1/acstools/acssum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13238 2023-05-23 16:27:24.000000 acstools-3.6.1/acstools/acszpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-23 16:27:24.000000 acstools-3.6.1/acstools/calacs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:28:10.652797 acstools-3.6.1/acstools/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-23 16:27:24.000000 acstools-3.6.1/acstools/data/polarizer_tables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-05-23 16:27:24.000000 acstools-3.6.1/acstools/data/rt_line_kernel_width15.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-05-23 16:27:24.000000 acstools-3.6.1/acstools/data/rt_line_kernel_width3.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-05-23 16:27:24.000000 acstools-3.6.1/acstools/data/rt_line_kernel_width7.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    52685 2023-05-23 16:27:24.000000 acstools-3.6.1/acstools/findsat_mrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16594 2023-05-23 16:27:24.000000 acstools-3.6.1/acstools/polarization_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35081 2023-05-23 16:27:24.000000 acstools-3.6.1/acstools/satdet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:28:10.652797 acstools-3.6.1/acstools/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-23 16:27:24.000000 acstools-3.6.1/acstools/tests/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-23 16:27:24.000000 acstools-3.6.1/acstools/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:28:10.644797 acstools-3.6.1/acstools/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:28:10.652797 acstools-3.6.1/acstools/tests/data/input/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-23 16:27:24.000000 acstools-3.6.1/acstools/tests/data/input/ja0x03ojq_flt.fits
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-23 16:27:24.000000 acstools-3.6.1/acstools/tests/data/input/jb5g05ubq_flt.fits
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-23 16:27:24.000000 acstools-3.6.1/acstools/tests/data/input/jc2z03cvq_blv_tmp.fits
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-23 16:27:24.000000 acstools-3.6.1/acstools/tests/data/input/jc5001soq_flt.fits
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-23 16:27:24.000000 acstools-3.6.1/acstools/tests/data/input/jc8m10syq_flc.fits
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-23 16:27:24.000000 acstools-3.6.1/acstools/tests/data/input/jc8m32j5q_flc.fits
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-23 16:27:24.000000 acstools-3.6.1/acstools/tests/data/input/jc8o04ghq_flt.fits
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-23 16:27:24.000000 acstools-3.6.1/acstools/tests/data/input/jc8o04ghq_mask1.fits
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-23 16:27:24.000000 acstools-3.6.1/acstools/tests/data/input/jc8o04ghq_mask2.fits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:28:10.656798 acstools-3.6.1/acstools/tests/data/truth/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-23 16:27:24.000000 acstools-3.6.1/acstools/tests/data/truth/ja0x03ojq_flt_ref.fits
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-23 16:27:24.000000 acstools-3.6.1/acstools/tests/data/truth/jb5g05ubq_flt_ref.fits
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-23 16:27:24.000000 acstools-3.6.1/acstools/tests/data/truth/jc2z03cvq_blv_tmp_ref.fits
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-23 16:27:24.000000 acstools-3.6.1/acstools/tests/data/truth/jc5001soq_flt_ref.fits
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-23 16:27:25.000000 acstools-3.6.1/acstools/tests/data/truth/jc8m10syq_flc_ref.fits
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-23 16:27:25.000000 acstools-3.6.1/acstools/tests/data/truth/jc8m32j5q_flc_mask_ref.fits
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-23 16:27:25.000000 acstools-3.6.1/acstools/tests/data/truth/jc8o04ghq_flt_ref.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-05-23 16:27:25.000000 acstools-3.6.1/acstools/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-23 16:27:25.000000 acstools-3.6.1/acstools/tests/test_polarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-23 16:27:25.000000 acstools-3.6.1/acstools/tests/test_wfc_destripe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-23 16:27:25.000000 acstools-3.6.1/acstools/tests/test_wfc_findsat_mrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-23 16:27:25.000000 acstools-3.6.1/acstools/tests/test_wfc_satdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16780 2023-05-23 16:27:25.000000 acstools-3.6.1/acstools/utils_calib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48734 2023-05-23 16:27:25.000000 acstools-3.6.1/acstools/utils_findsat_mrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-23 16:27:37.000000 acstools-3.6.1/acstools/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:28:10.652797 acstools-3.6.1/acstools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-23 16:27:37.000000 acstools-3.6.1/acstools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-23 16:28:10.000000 acstools-3.6.1/acstools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 16:27:37.000000 acstools-3.6.1/acstools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-23 16:27:37.000000 acstools-3.6.1/acstools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 16:27:37.000000 acstools-3.6.1/acstools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-23 16:27:37.000000 acstools-3.6.1/acstools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 16:27:37.000000 acstools-3.6.1/acstools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-23 16:27:25.000000 acstools-3.6.1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:28:10.656798 acstools-3.6.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-05-23 16:27:25.000000 acstools-3.6.1/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-05-23 16:27:25.000000 acstools-3.6.1/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:28:10.656798 acstools-3.6.1/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:28:10.656798 acstools-3.6.1/doc/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    65413 2023-05-23 16:27:25.000000 acstools-3.6.1/doc/source/_static/stsci_pri_combo_mark_white.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:28:10.656798 acstools-3.6.1/doc/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:27:25.000000 acstools-3.6.1/doc/source/_templates/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-23 16:27:25.000000 acstools-3.6.1/doc/source/acs_destripe.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-23 16:27:25.000000 acstools-3.6.1/doc/source/acsphotcte.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-23 16:27:25.000000 acstools-3.6.1/doc/source/acszpt.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9851 2023-05-23 16:27:25.000000 acstools-3.6.1/doc/source/calacs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-05-23 16:27:25.000000 acstools-3.6.1/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-23 16:27:25.000000 acstools-3.6.1/doc/source/findsat_mrt.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-23 16:27:25.000000 acstools-3.6.1/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-23 16:27:25.000000 acstools-3.6.1/doc/source/polarization_tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-23 16:27:25.000000 acstools-3.6.1/doc/source/satdet.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-23 16:27:25.000000 acstools-3.6.1/doc/source/utils_calib.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-23 16:27:25.000000 acstools-3.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-23 16:28:10.656798 acstools-3.6.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-05-23 16:27:25.000000 acstools-3.6.1/setup.py
```

### Comparing `acstools-3.6.0/.github/ISSUE_TEMPLATE/bug_report.md` & `acstools-3.6.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/.github/ISSUE_TEMPLATE/feature_request.md` & `acstools-3.6.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/.github/ISSUE_TEMPLATE/question.md` & `acstools-3.6.1/.github/ISSUE_TEMPLATE/question.md`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/.github/PULL_REQUEST_TEMPLATE.md` & `acstools-3.6.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/.github/labeler.yml` & `acstools-3.6.1/.github/labeler.yml`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/.github/workflows/ci_workflows.yml` & `acstools-3.6.1/.github/workflows/ci_workflows.yml`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/.github/workflows/codeql-analysis.yml` & `acstools-3.6.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/.github/workflows/open_actions.yml` & `acstools-3.6.1/.github/workflows/open_actions.yml`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/.github/workflows/predeps_workflows.yml` & `acstools-3.6.1/.github/workflows/predeps_workflows.yml`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/.github/workflows/publish-to-pypi.yml` & `acstools-3.6.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/CODE_OF_CONDUCT.md` & `acstools-3.6.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/LICENSE.md` & `acstools-3.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/PKG-INFO` & `acstools-3.6.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acstools
-Version: 3.6.0
+Version: 3.6.1
 Summary: Python Tools for HST ACS
 Home-page: https://github.com/spacetelescope/acstools
 Author: Matt Davis, Warren Hack, Norman Grogin, Pey Lian Lim, Sara Ogaz, Leonardo Ubeda, Mihai Cara, David Borncamp, Nathan Miles, Tyler Desjardins, Jenna Ryon, David Stark
 Author-email: help@stsci.edu
 License: BSD
 Project-URL: Bug Reports, https://github.com/spacetelescope/acstools/issues/
 Project-URL: Source, https://github.com/spacetelescope/acstools/
```

### Comparing `acstools-3.6.0/README.rst` & `acstools-3.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/acstools/__init__.py` & `acstools-3.6.1/acstools/__init__.py`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/acstools/acs2d.py` & `acstools-3.6.1/acstools/acs2d.py`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/acstools/acs_destripe.py` & `acstools-3.6.1/acstools/acs_destripe.py`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/acstools/acs_destripe_plus.py` & `acstools-3.6.1/acstools/acs_destripe_plus.py`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/acstools/acsccd.py` & `acstools-3.6.1/acstools/acsccd.py`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/acstools/acscte.py` & `acstools-3.6.1/acstools/acscte.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 The acscte module contains a function `acscte` that calls the ACSCTE executable.
 Use this function to facilitate batch runs of ACSCTE.
 
 Only WFC full-frame and some 2K subarrays are currently supported. See
-`ACS Data Handbook <https://hst-docs.stsci.edu/acsdhb>`_
+`Table 7.6 in the ACS Instrument Handbook <https://hst-docs.stsci.edu/acsihb/chapter-7-observing-techniques/7-3-operating-modes#id-7.3OperatingModes-table7.6>`_
 for more details.
 
 .. note:: Calibration flags are controlled by primary header.
 
 Examples
 --------
```

### Comparing `acstools-3.6.0/acstools/acscteforwardmodel.py` & `acstools-3.6.1/acstools/acscteforwardmodel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 The acscteforwardmodel module contains a function `acscteforwardmodel`
 that calls the ACSCTE forward model executable.
 Use this function to facilitate batch runs of the forward model.
 
 Only WFC full-frame and some 2K subarrays are currently supported. See
-`ACS Data Handbook <https://hst-docs.stsci.edu/acsdhb>`_ for more details.
+`Table 7.6 in the ACS Instrument Handbook <https://hst-docs.stsci.edu/acsihb/chapter-7-observing-techniques/7-3-operating-modes#id-7.3OperatingModes-table7.6>`_
+for more details.
 
 For guidance on running the CTE forward model, see the Jupyter notebook
 `ACS CTE Forward Model Example <https://github.com/spacetelescope/acs-notebook/blob/master/acs_cte_forward_model/acs_cte_forward_model_example.ipynb>`_.
 
 .. note:: Calibration flags are controlled by primary header.
 
 Examples
```

### Comparing `acstools-3.6.0/acstools/acsphotcte.py` & `acstools-3.6.1/acstools/acsphotcte.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,25 +17,24 @@
 ----------------
 As this service is hosted on AWS, there are some guidelines that should be
 followed when utilizing this tool. For each call to
 :py:meth:`~acstools.acsphotcte.PhotCTEAPI.correct_photometry`, AWS will assemble the compute resources,
 install the software, compute the CTE corrections, send the result back,
 and then terminate all resources. Hence, users should try to process as many
 sources as they can in a single function call. Testing has shown that the
-optimal number is < 25000, but the service can handle as many as 150,000
+optimal number is < 25,000, but the service can handle as many as 150,000
 sources in a single request.
 
 Examples
 --------
-In this example, we get the CTE corrected FLT photometry for a list of 1000
-sources. For each parameter, we generate 1000 random values in the interval [0, 1) and
-then scale each value to be in the typical range. We use arbitrary values for
-the fluxes, local sky backgrounds, and MJD. We assume a radius of 3 pixels was
-used to compute the aperture photometry. For the ACS/WFC CCD chips, the maximum
-number of Y transfers is 2048 and so we scale by 2048.
+In this example, we obtain the CTE-corrected FLT photometry for a list of 1000
+artificial sources. For each parameter, we generate 1000 random values in the interval [0, 1) and
+then scale the random data by a realistic value for stellar fluxes,
+y-transfers, and local sky backgrounds. An arbitrary MJD is defined, and
+we assume an aperture radius of 3 pixels.
 
 >>> import numpy as np
 >>> from acstools import acsphotcte
 >>> n_sample = 1000
 >>> ytransfers = 2048 * np.random.random(size=n_sample)
 >>> fluxes = 20000*np.random.random(size=n_sample)
 >>> magnitudes = -2.5 * np.log10(fluxes)
```

### Comparing `acstools-3.6.0/acstools/acsrej.py` & `acstools-3.6.1/acstools/acsrej.py`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/acstools/acssum.py` & `acstools-3.6.1/acstools/acssum.py`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/acstools/acszpt.py` & `acstools-3.6.1/acstools/acszpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 information for all the filters for the desired detector at the specified date.
 In either case, the result will be an ``astropy.table.QTable`` where each column
 is an ``astropy.units.quantity.Quantity`` object with the appropriate units attached.
 
 Examples
 --------
 
-Retrieve the zeropoint information for all the filters on 2016-04-01 for WFC:
+Retrieve the zeropoint information for all of the WFC filters on 2016-04-01:
 
 >>> from acstools import acszpt
 >>> q = acszpt.Query(date="2016-04-01", detector="WFC")
 >>> zpt_table = q.fetch()
 >>> print(zpt_table)
 Filter PHOTLAM             PHOTFLAM            STmag  VEGAmag  ABmag
        Angstrom erg / (Angstrom cm2 electron) mag(ST)   mag   mag(AB)
@@ -37,26 +37,26 @@
  F658N   6584.0                    1.9976e-18  23.149  22.378  22.748
  F660N   6599.4                    5.2219e-18  22.105  21.414    21.7
  F775W   7693.5                    1.0033e-19  26.396   25.26  25.658
  F814W   8045.5                     7.092e-20  26.773  25.506  25.937
 F850LP   9031.5                    1.5313e-19  25.937  24.323  24.851
  F892N   8914.8                    1.5105e-18  23.452  21.892  22.394
 
-Retrieve the zeropoint information for the F435W filter on 2016-04-01 for WFC:
+Retrieve the zeropoint information for the WFC/F435W filter on 2016-04-01:
 
 >>> from acstools import acszpt
 >>> q = acszpt.Query(date="2016-04-01", detector="WFC", filt="F435W")
 >>> zpt_table = q.fetch()
 >>> print(zpt_table)
 Filter PHOTLAM             PHOTFLAM            STmag  VEGAmag  ABmag
        Angstrom erg / (Angstrom cm2 electron) mag(ST)   mag   mag(AB)
 ------ -------- ----------------------------- ------- ------- -------
  F435W   4329.9                    3.1858e-19  25.142  25.767  25.652
 
-Retrieve the zeropoint information for the F435W filter for WFC at multiple dates:
+Retrieve the zeropoint information for the WFC/F435W filter on multiple dates:
 
 >>> from acstools import acszpt
 >>> dates = ['2004-10-13', '2011-04-01', '2014-01-17', '2018-05-23']
 >>> queries = []
 
 >>> for date in dates:
 ...     q = acszpt.Query(date=date, detector='WFC', filt='F435W')
```

### Comparing `acstools-3.6.0/acstools/calacs.py` & `acstools-3.6.1/acstools/calacs.py`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/acstools/data/polarizer_tables.yaml` & `acstools-3.6.1/acstools/data/polarizer_tables.yaml`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/acstools/data/rt_line_kernel_width15.fits` & `acstools-3.6.1/acstools/data/rt_line_kernel_width15.fits`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/acstools/data/rt_line_kernel_width3.fits` & `acstools-3.6.1/acstools/data/rt_line_kernel_width3.fits`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/acstools/data/rt_line_kernel_width7.fits` & `acstools-3.6.1/acstools/data/rt_line_kernel_width7.fits`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/acstools/findsat_mrt.py` & `acstools-3.6.1/acstools/findsat_mrt.py`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/acstools/polarization_tools.py` & `acstools-3.6.1/acstools/polarization_tools.py`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/acstools/satdet.py` & `acstools-3.6.1/acstools/satdet.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     Only tested for ACS/WFC FLT and FLC images, but it should
     theoretically work for any instrument.
 
     Requires skimage version 0.11.x or later.
 
     :func:`skimage.transform.probabilistic_hough_line` gives
     slightly different results from run to run, but this should
-    not matter since :func:`detsat` only provides crude
+    not matter since :func:`detsat` only provides a crude
     approximation of the actual trail(s).
 
     Performance is faster when ``plot=False``, where applicable.
 
 Examples
 --------
 >>> from acstools.satdet import detsat, make_mask
@@ -211,15 +211,15 @@
     immax = np.max(image)
     edge = canny(image, sigma=sigma,
                  low_threshold=immax * low_thresh,
                  high_threshold=immax * h_thresh)
 
     # clean up the small objects, will make less noise
     morph.remove_small_objects(edge, min_size=small_edge, connectivity=8,
-                               in_place=True)
+                               out=edge)
 
     # create an array of angles from 0 to 180, exactly 0 will get bad columns
     # but it is unlikely that a satellite will be exactly at 0 degrees, so
     # don't bother checking.
     # then, convert to radians.
     angle = np.radians(np.arange(2, 178, 0.5, dtype=float))
```

### Comparing `acstools-3.6.0/acstools/tests/helpers.py` & `acstools-3.6.1/acstools/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/acstools/tests/test_polarization.py` & `acstools-3.6.1/acstools/tests/test_polarization.py`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/acstools/tests/test_wfc_destripe.py` & `acstools-3.6.1/acstools/tests/test_wfc_destripe.py`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/acstools/tests/test_wfc_findsat_mrt.py` & `acstools-3.6.1/acstools/tests/test_wfc_findsat_mrt.py`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/acstools/tests/test_wfc_satdet.py` & `acstools-3.6.1/acstools/tests/test_wfc_satdet.py`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/acstools/utils_calib.py` & `acstools-3.6.1/acstools/utils_calib.py`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/acstools/utils_findsat_mrt.py` & `acstools-3.6.1/acstools/utils_findsat_mrt.py`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/acstools.egg-info/PKG-INFO` & `acstools-3.6.1/acstools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acstools
-Version: 3.6.0
+Version: 3.6.1
 Summary: Python Tools for HST ACS
 Home-page: https://github.com/spacetelescope/acstools
 Author: Matt Davis, Warren Hack, Norman Grogin, Pey Lian Lim, Sara Ogaz, Leonardo Ubeda, Mihai Cara, David Borncamp, Nathan Miles, Tyler Desjardins, Jenna Ryon, David Stark
 Author-email: help@stsci.edu
 License: BSD
 Project-URL: Bug Reports, https://github.com/spacetelescope/acstools/issues/
 Project-URL: Source, https://github.com/spacetelescope/acstools/
```

### Comparing `acstools-3.6.0/acstools.egg-info/SOURCES.txt` & `acstools-3.6.1/acstools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/conftest.py` & `acstools-3.6.1/conftest.py`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/doc/Makefile` & `acstools-3.6.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/doc/make.bat` & `acstools-3.6.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/doc/source/_static/stsci_pri_combo_mark_white.png` & `acstools-3.6.1/doc/source/_static/stsci_pri_combo_mark_white.png`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/doc/source/calacs.rst` & `acstools-3.6.1/doc/source/calacs.rst`

 * *Files 2% similar despite different names*

```diff
@@ -52,39 +52,41 @@
     :headings: =-
     :no-inheritance-diagram:
 
 CTE Forward Model
 =================
 
 This functionality is provided to simulate the CTE effects associated with
-readout of the WFC detectors. It is not part of the standard CALACS pipeline.
+readout of the WFC detectors. It is not involved in standard data calibration with the CALACS pipeline.
 
 .. automodapi:: acstools.acscteforwardmodel
     :no-heading:
     :headings: =-
     :no-inheritance-diagram:
 
 PIXVALUE in FITS File
 =====================
 
-CALACS uses HSTIO that utilizes ``PIXVALUE`` keyword to represent a data
-extension with constant value. However, this is not a standard FITS behavior
-and is not recognized by ``astropy.io.fits``. While you should not encounter errors or warnings, constant value data extensions may exhibit unexpected behavior when reading, writing, or manipulating them with ``astropy.io.fits``. Therefore, if issues such as these arise, we recommend use of
+CALACS uses HSTIO, which utilizes the ``PIXVALUE`` keyword to represent a data
+extension with a constant value. However, this is not a standard FITS behavior
+and is not recognized by ``astropy.io.fits``. While you should not encounter errors or warnings, 
+constant value data extensions may exhibit unexpected behavior when reading, writing, or 
+manipulating them with ``astropy.io.fits``. Therefore, if issues such as these arise, we recommend use of
 ``stsci.tools.stpyfits``, which is distributed as part of ``stsci_python``,
 instead of `astropy.io.fits` when working with CALACS products.
 To use ``stpyfits`` in Python::
 
     from stsci.tools import stpyfits as fits
 
 calacs.e (C Program)
 ====================
 
 A detailed description of CALACS is available in the
 `ACS Data Handbook <https://hst-docs.stsci.edu/acsdhb>`_.
-If you have questions not answered in the documentation, please contact
+If you have questions not answered in the documentation, please contact the
 `STScI Help Desk <https://hsthelp.stsci.edu>`_.
 
 Where to Find CALACS
 --------------------
 
 CALACS is part of the
 `HSTCAL package <https://github.com/spacetelescope/hstcal>`_.
@@ -131,16 +133,17 @@
     * Specify the number of threads used for PCTECORR.
       The default is 'greedy' and will use that specified by the system environment variable OMP_NUM_THREADS.
       If N > ``OMP_NUM_THREADS``, ``OMP_NUM_THREADS`` will be used instead. The option -1 takes precedence.
 
 * --ctegen <1|2>
 
     * Specify which generation CTE correction to use, the default is 2. Gen 1 (officially deprecated) refers to
-      the correction algorithm used in calacs version pre 9.2.0 in relation to
-      `ACS ISR 2010-03 <https://ui.adsabs.harvard.edu/abs/2010PASP..122.1035A/abstract>`_. Gen 2 refers to the new CTE correction algorithm implemented in calacs version 9.2.0 (HSTCAL 1.3.0) in relation to `ACS ISR 2018-04 <https://ui.adsabs.harvard.edu/abs/2018acs..rept....4A/abstract>`_.
+      the correction algorithm used in calacs version pre 9.2.0, described in
+      `ACS ISR 2010-03 <https://ui.adsabs.harvard.edu/abs/2010PASP..122.1035A/abstract>`_. Gen 2 refers to the 
+      new CTE correction algorithm implemented in calacs version 9.2.0 (HSTCAL 1.3.0) described in `ACS ISR 2018-04 <https://ui.adsabs.harvard.edu/abs/2018acs..rept....4A/abstract>`_.
 
 * --pctetab <filename>
 
     * Override the PCTETAB reference file specified in the image header.
 
 Parallel Processing with OpenMP
 -------------------------------
@@ -191,36 +194,37 @@
 The image is multiplied by the gain, converting it to ELECTRONS.
 
 Bias Level Correction (BLEVCORR)
 --------------------------------
 
 BLEVCORR is performed after BIASCORR. Calculations are done in ELECTRONS.
 
-For post-SM4 full-frame WFC exposures, it also includes:
+For post-SM4 full-frame WFC exposures, this also includes:
 
 * de-striping to remove stripes introduced by new hardware installed during
   SM-4 (`ACS ISR 2011-05 <https://ui.adsabs.harvard.edu/abs/2011acs..rept....5G/abstract>`_)
 * if JWROTYPE=DS_int and CCDGAIN=2, also correct for bias shift
   (`ACS ISR 2012-02 <https://ui.adsabs.harvard.edu/abs/2012acs..rept....2G/abstract>`_) and cross-talk (`ACS ISR 2010-02 <https://ui.adsabs.harvard.edu/abs/2010acs..rept....2S/abstract>`_).
 
 Sink Pixel Flagging (SINKCORR)
 ------------------------------
 
-SINKCORR flags sink pixels and the adjacent affected pixels with the value
-1024 in the DQ array of WFC images using the SNKCFILE. Only performed on images
+SINKCORR flags sink pixels and adjacent affected pixels with the value
+1024 in the DQ array of WFC images using the SNKCFILE. It is only performed on images
 taken after January 2015.
 
 Pixel-Based CTE Correction (PCTECORR)
 -------------------------------------
 
-For all full-frame WFC exposures, pixel-based CTE correction (`ACS ISR 2018-04 <https://ui.adsabs.harvard.edu/abs/2018acs..rept....4A/abstract>`_)
-is applied during ACSCTE that occurs after ACSCCD, specifically, after BLEVCORR.
+For all full-frame WFC exposures, pixel-based CTE correction 
+(`ACS ISR 2018-04 <https://ui.adsabs.harvard.edu/abs/2018acs..rept....4A/abstract>`_)
+is applied during ACSCTE, which runs after BLEVCORR in ACSCCD.
 
 Because the CTE correction is applied before DARKCORR and FLSHCORR, it is
-necessary to use a CTE-corrected dark (DRKCFILE) if the PCTECORR step is enabled.
+necessary to use a CTE-corrected dark reference file (DRKCFILE) if the PCTECORR step is enabled.
 
 Parameters characterizing the CTE correction are stored in a reference table,
 PCTETAB.
 
 .. note::
 
     CALACS 8.2 and later uses a slightly different PCTETAB format, where
@@ -280,15 +284,15 @@
 
 * PCTETLEN
 
     * Maximum length of CTE trail.
 
 * PCTENFOR
 
-    * Number of iterations used for forward CTE model.
+    * Number of iterations used for the CTE forward model.
 
 Dark Current Subtraction (DARKCORR)
 -----------------------------------
 
 Dark correction uses DARKFILE if PCTECORR=OMIT, otherwise it uses DRKCFILE (CTE-corrected
 dark reference file).
 
@@ -303,15 +307,15 @@
 When FLSHCORR=PERFORM, it scales FLSHFILE by FLASHDUR for correction.
 
 Flat-Field Correction (FLATCORR)
 --------------------------------
 
 PFLTFILE is used for flat-field correction, which is a combination of the
 pixel-to-pixel flats and low-order flats. This corrects for pixel-to-pixel and
-large-scale sensitivity gradients across the detector by dividing the data with
+large-scale sensitivity gradients across the detector by dividing the data by
 the flat-field image.
 
 Photometry Keywords (PHOTCORR)
 ------------------------------
 
 The PHOTCORR step is performed using tables of precomputed values (IMPHTTAB).
 The correct table for a given image must be specified
```

### Comparing `acstools-3.6.0/doc/source/conf.py` & `acstools-3.6.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/doc/source/index.rst` & `acstools-3.6.1/doc/source/index.rst`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 To install the development version of this package::
 
     pip install git+https://github.com/spacetelescope/acstools
 
 .. note::
 
-    The information here reflect the *latest* software info and might not
+    The information here reflects the *latest* software and might not
     be in-sync with the
     `ACS Data Handbook <https://hst-docs.stsci.edu/acsdhb>`_.
 
 .. note::
 
     Standalone CTE correction (``PixCteCorr``) is no longer supported.
     Please use `acstools.acscte`.
```

### Comparing `acstools-3.6.0/setup.cfg` & `acstools-3.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `acstools-3.6.0/setup.py` & `acstools-3.6.1/setup.py`

 * *Files identical despite different names*

