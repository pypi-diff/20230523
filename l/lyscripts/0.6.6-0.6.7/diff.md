# Comparing `tmp/lyscripts-0.6.6.tar.gz` & `tmp/lyscripts-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyscripts-0.6.6.tar", last modified: Thu Dec  1 16:05:28 2022, max compression
+gzip compressed data, was "lyscripts-0.6.7.tar", last modified: Tue May 23 10:12:21 2023, max compression
```

## Comparing `lyscripts-0.6.6.tar` & `lyscripts-0.6.7.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 16:05:28.081687 lyscripts-0.6.6/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 16:05:28.073687 lyscripts-0.6.6/.chglog/
--rwxr-xr-x   0 runner    (1001) docker     (122)     1043 2022-12-01 16:05:08.000000 lyscripts-0.6.6/.chglog/CHANGELOG.tpl.md
--rwxr-xr-x   0 runner    (1001) docker     (122)      814 2022-12-01 16:05:08.000000 lyscripts-0.6.6/.chglog/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 16:05:28.069687 lyscripts-0.6.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 16:05:28.073687 lyscripts-0.6.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      664 2022-12-01 16:05:08.000000 lyscripts-0.6.6/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (122)      788 2022-12-01 16:05:08.000000 lyscripts-0.6.6/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1202 2022-12-01 16:05:08.000000 lyscripts-0.6.6/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1860 2022-12-01 16:05:08.000000 lyscripts-0.6.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1611 2022-12-01 16:05:08.000000 lyscripts-0.6.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     9766 2022-12-01 16:05:08.000000 lyscripts-0.6.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2022-12-01 16:05:08.000000 lyscripts-0.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     7732 2022-12-01 16:05:28.081687 lyscripts-0.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7178 2022-12-01 16:05:08.000000 lyscripts-0.6.6/README.md
--rw-r--r--   0 runner    (1001) docker     (122)    18415 2022-12-01 16:05:08.000000 lyscripts-0.6.6/favicon.png
--rw-r--r--   0 runner    (1001) docker     (122)   105407 2022-12-01 16:05:08.000000 lyscripts-0.6.6/github-social-card.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 16:05:28.073687 lyscripts-0.6.6/lyscripts/
--rw-r--r--   0 runner    (1001) docker     (122)     3319 2022-12-01 16:05:08.000000 lyscripts-0.6.6/lyscripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      268 2022-12-01 16:05:08.000000 lyscripts-0.6.6/lyscripts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      176 2022-12-01 16:05:27.000000 lyscripts-0.6.6/lyscripts/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 16:05:28.077687 lyscripts-0.6.6/lyscripts/app/
--rw-r--r--   0 runner    (1001) docker     (122)      617 2022-12-01 16:05:08.000000 lyscripts-0.6.6/lyscripts/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10498 2022-12-01 16:05:08.000000 lyscripts-0.6.6/lyscripts/app/prevalence.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 16:05:28.077687 lyscripts-0.6.6/lyscripts/data/
--rw-r--r--   0 runner    (1001) docker     (122)     1759 2022-12-01 16:05:08.000000 lyscripts-0.6.6/lyscripts/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1024 2022-12-01 16:05:08.000000 lyscripts-0.6.6/lyscripts/data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4665 2022-12-01 16:05:08.000000 lyscripts-0.6.6/lyscripts/data/clean.py
--rw-r--r--   0 runner    (1001) docker     (122)    13440 2022-12-01 16:05:08.000000 lyscripts-0.6.6/lyscripts/data/enhance.py
--rw-r--r--   0 runner    (1001) docker     (122)     5525 2022-12-01 16:05:08.000000 lyscripts-0.6.6/lyscripts/data/generate.py
--rw-r--r--   0 runner    (1001) docker     (122)     2808 2022-12-01 16:05:08.000000 lyscripts-0.6.6/lyscripts/data/join.py
--rw-r--r--   0 runner    (1001) docker     (122)    10538 2022-12-01 16:05:08.000000 lyscripts-0.6.6/lyscripts/data/lyproxify.py
--rw-r--r--   0 runner    (1001) docker     (122)     3802 2022-12-01 16:05:08.000000 lyscripts-0.6.6/lyscripts/data/split.py
--rw-r--r--   0 runner    (1001) docker     (122)     1124 2022-12-01 16:05:08.000000 lyscripts-0.6.6/lyscripts/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     8517 2022-12-01 16:05:08.000000 lyscripts-0.6.6/lyscripts/evaluate.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 16:05:28.077687 lyscripts-0.6.6/lyscripts/plot/
--rw-r--r--   0 runner    (1001) docker     (122)     1276 2022-12-01 16:05:08.000000 lyscripts-0.6.6/lyscripts/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      878 2022-12-01 16:05:08.000000 lyscripts-0.6.6/lyscripts/plot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5504 2022-12-01 16:05:08.000000 lyscripts-0.6.6/lyscripts/plot/corner.py
--rw-r--r--   0 runner    (1001) docker     (122)     4230 2022-12-01 16:05:08.000000 lyscripts-0.6.6/lyscripts/plot/histograms.py
--rw-r--r--   0 runner    (1001) docker     (122)     6241 2022-12-01 16:05:08.000000 lyscripts-0.6.6/lyscripts/plot/thermo_int.py
--rw-r--r--   0 runner    (1001) docker     (122)    10042 2022-12-01 16:05:08.000000 lyscripts-0.6.6/lyscripts/plot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 16:05:28.077687 lyscripts-0.6.6/lyscripts/predict/
--rw-r--r--   0 runner    (1001) docker     (122)     1132 2022-12-01 16:05:08.000000 lyscripts-0.6.6/lyscripts/predict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      794 2022-12-01 16:05:08.000000 lyscripts-0.6.6/lyscripts/predict/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14134 2022-12-01 16:05:08.000000 lyscripts-0.6.6/lyscripts/predict/prevalences.py
--rw-r--r--   0 runner    (1001) docker     (122)     6647 2022-12-01 16:05:08.000000 lyscripts-0.6.6/lyscripts/predict/risks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1956 2022-12-01 16:05:08.000000 lyscripts-0.6.6/lyscripts/predict/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    18888 2022-12-01 16:05:08.000000 lyscripts-0.6.6/lyscripts/sample.py
--rw-r--r--   0 runner    (1001) docker     (122)     4859 2022-12-01 16:05:08.000000 lyscripts-0.6.6/lyscripts/temp_schedule.py
--rw-r--r--   0 runner    (1001) docker     (122)    18711 2022-12-01 16:05:08.000000 lyscripts-0.6.6/lyscripts/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 16:05:28.073687 lyscripts-0.6.6/lyscripts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7732 2022-12-01 16:05:28.000000 lyscripts-0.6.6/lyscripts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1574 2022-12-01 16:05:28.000000 lyscripts-0.6.6/lyscripts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-01 16:05:28.000000 lyscripts-0.6.6/lyscripts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       45 2022-12-01 16:05:28.000000 lyscripts-0.6.6/lyscripts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      193 2022-12-01 16:05:28.000000 lyscripts-0.6.6/lyscripts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2022-12-01 16:05:28.000000 lyscripts-0.6.6/lyscripts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1472 2022-12-01 16:05:08.000000 lyscripts-0.6.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-01 16:05:28.081687 lyscripts-0.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-01 16:05:08.000000 lyscripts-0.6.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 16:05:28.077687 lyscripts-0.6.6/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     2433 2022-12-01 16:05:08.000000 lyscripts-0.6.6/tests/_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 16:05:28.077687 lyscripts-0.6.6/tests/plot/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 16:05:28.077687 lyscripts-0.6.6/tests/plot/baseline/
--rw-r--r--   0 runner    (1001) docker     (122)    12265 2022-12-01 16:05:08.000000 lyscripts-0.6.6/tests/plot/baseline/sine.png
--rw-r--r--   0 runner    (1001) docker     (122)    12916 2022-12-01 16:05:08.000000 lyscripts-0.6.6/tests/plot/baseline/sine.svg
--rw-r--r--   0 runner    (1001) docker     (122)    12629 2022-12-01 16:05:08.000000 lyscripts-0.6.6/tests/plot/baseline/sine_svg.png
--rw-r--r--   0 runner    (1001) docker     (122)    36976 2022-12-01 16:05:08.000000 lyscripts-0.6.6/tests/plot/baseline/test_draw.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 16:05:28.077687 lyscripts-0.6.6/tests/plot/data/
--rw-r--r--   0 runner    (1001) docker     (122)    86144 2022-12-01 16:05:08.000000 lyscripts-0.6.6/tests/plot/data/beta_samples.hdf5
--rw-r--r--   0 runner    (1001) docker     (122)     7882 2022-12-01 16:05:08.000000 lyscripts-0.6.6/tests/plot/plot_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 16:05:28.081687 lyscripts-0.6.6/tests/predict/
--rw-r--r--   0 runner    (1001) docker     (122)     1156 2022-12-01 16:05:08.000000 lyscripts-0.6.6/tests/predict/predict_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     3291 2022-12-01 16:05:08.000000 lyscripts-0.6.6/tests/predict/prevalences_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      504 2022-12-01 16:05:08.000000 lyscripts-0.6.6/tests/run_doctests.py
--rw-r--r--   0 runner    (1001) docker     (122)       31 2022-12-01 16:05:08.000000 lyscripts-0.6.6/tests/test.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      491 2022-12-01 16:05:08.000000 lyscripts-0.6.6/tests/test_data.csv
--rw-r--r--   0 runner    (1001) docker     (122)     2831 2022-12-01 16:05:08.000000 lyscripts-0.6.6/tests/test_params.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1161 2022-12-01 16:05:08.000000 lyscripts-0.6.6/tests/utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:12:21.935064 lyscripts-0.6.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:12:21.927064 lyscripts-0.6.7/.chglog/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1043 2023-05-23 10:12:04.000000 lyscripts-0.6.7/.chglog/CHANGELOG.tpl.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      814 2023-05-23 10:12:04.000000 lyscripts-0.6.7/.chglog/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:12:21.927064 lyscripts-0.6.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:12:21.927064 lyscripts-0.6.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-23 10:12:04.000000 lyscripts-0.6.7/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-23 10:12:04.000000 lyscripts-0.6.7/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-23 10:12:04.000000 lyscripts-0.6.7/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-23 10:12:04.000000 lyscripts-0.6.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-23 10:12:04.000000 lyscripts-0.6.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10068 2023-05-23 10:12:04.000000 lyscripts-0.6.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-23 10:12:04.000000 lyscripts-0.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-05-23 10:12:21.935064 lyscripts-0.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-05-23 10:12:04.000000 lyscripts-0.6.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18415 2023-05-23 10:12:04.000000 lyscripts-0.6.7/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)   105407 2023-05-23 10:12:04.000000 lyscripts-0.6.7/github-social-card.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:12:21.931064 lyscripts-0.6.7/lyscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-23 10:12:21.000000 lyscripts-0.6.7/lyscripts/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:12:21.931064 lyscripts-0.6.7/lyscripts/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/app/prevalence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:12:21.931064 lyscripts-0.6.7/lyscripts/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/data/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13440 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/data/enhance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/data/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/data/join.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10538 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/data/lyproxify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/data/split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/evaluate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:12:21.931064 lyscripts-0.6.7/lyscripts/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/plot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/plot/corner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/plot/histograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/plot/thermo_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/plot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:12:21.935064 lyscripts-0.6.7/lyscripts/predict/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/predict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/predict/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14134 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/predict/prevalences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/predict/risks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/predict/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/temp_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19744 2023-05-23 10:12:04.000000 lyscripts-0.6.7/lyscripts/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:12:21.931064 lyscripts-0.6.7/lyscripts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-05-23 10:12:21.000000 lyscripts-0.6.7/lyscripts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-23 10:12:21.000000 lyscripts-0.6.7/lyscripts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 10:12:21.000000 lyscripts-0.6.7/lyscripts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-23 10:12:21.000000 lyscripts-0.6.7/lyscripts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-23 10:12:21.000000 lyscripts-0.6.7/lyscripts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 10:12:21.000000 lyscripts-0.6.7/lyscripts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-23 10:12:04.000000 lyscripts-0.6.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 10:12:21.935064 lyscripts-0.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 10:12:04.000000 lyscripts-0.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:12:21.935064 lyscripts-0.6.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-23 10:12:04.000000 lyscripts-0.6.7/tests/_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:12:21.935064 lyscripts-0.6.7/tests/plot/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:12:21.935064 lyscripts-0.6.7/tests/plot/baseline/
+-rw-r--r--   0 runner    (1001) docker     (123)    12265 2023-05-23 10:12:04.000000 lyscripts-0.6.7/tests/plot/baseline/sine.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12916 2023-05-23 10:12:04.000000 lyscripts-0.6.7/tests/plot/baseline/sine.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-05-23 10:12:04.000000 lyscripts-0.6.7/tests/plot/baseline/sine_svg.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36976 2023-05-23 10:12:04.000000 lyscripts-0.6.7/tests/plot/baseline/test_draw.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:12:21.935064 lyscripts-0.6.7/tests/plot/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    86144 2023-05-23 10:12:04.000000 lyscripts-0.6.7/tests/plot/data/beta_samples.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)     8088 2023-05-23 10:12:04.000000 lyscripts-0.6.7/tests/plot/plot_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:12:21.935064 lyscripts-0.6.7/tests/predict/
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-23 10:12:04.000000 lyscripts-0.6.7/tests/predict/predict_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-05-23 10:12:04.000000 lyscripts-0.6.7/tests/predict/prevalences_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-23 10:12:04.000000 lyscripts-0.6.7/tests/run_doctests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-23 10:12:04.000000 lyscripts-0.6.7/tests/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-23 10:12:04.000000 lyscripts-0.6.7/tests/test_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-23 10:12:04.000000 lyscripts-0.6.7/tests/test_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-23 10:12:04.000000 lyscripts-0.6.7/tests/utils_test.py
```

### Comparing `lyscripts-0.6.6/.chglog/CHANGELOG.tpl.md` & `lyscripts-0.6.7/.chglog/CHANGELOG.tpl.md`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/.chglog/config.yml` & `lyscripts-0.6.7/.chglog/config.yml`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/.github/workflows/build.yml` & `lyscripts-0.6.7/.github/workflows/build.yml`

 * *Files 19% similar despite different names*

```diff
@@ -11,17 +11,17 @@
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v2
         with:
           fetch-depth: 0
       - name: Install python 3
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
-          python-version: 3.8
+          python-version: '3.10'
       - name: Install dependencies
         run: |
           python3 -m pip install -U pip setuptools setuptools-scm wheel twine build
       - name: Build and publish
         env:
           TWINE_USERNAME: __token__
           TWINE_PASSWORD: ${{ secrets.PYPI_TOKEN }}
```

### Comparing `lyscripts-0.6.6/.github/workflows/docs.yml` & `lyscripts-0.6.7/.github/workflows/docs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 jobs:
   build:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v2
       - name: Install Python
-        uses: actions/setup-python@v3
+        uses: actions/setup-python@v4
         with:
-          python-version: 3.8
+          python-version: '3.10'
       - name: Install deps & package
         run: |
           python -m pip install --upgrade pip
           python -m pip install .[docs]
       - name: Build docs
         run: >
           python -m pdoc
```

### Comparing `lyscripts-0.6.6/.github/workflows/tests.yml` & `lyscripts-0.6.7/.github/workflows/tests.yml`

 * *Files 8% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     # Steps represent a sequence of tasks that will be executed as part of the job
     steps:
       # Checks-out your repository under $GITHUB_WORKSPACE, so your job can access it
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: Install python 3
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
-          python-version: 3.8
+          python-version: '3.10'
       - name: install dependencies
         run: |
           python3 -m pip install -U pip setuptools setuptools-scm wheel
           python3 -m pip install .[tests]
       - name: Run tests
         run: |
           python3 -m pytest --doctest-modules
```

### Comparing `lyscripts-0.6.6/.gitignore` & `lyscripts-0.6.7/.gitignore`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/.pre-commit-config.yaml` & `lyscripts-0.6.7/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   - id: trailing-whitespace
 - repo: https://github.com/hadialqattan/pycln
   rev: v1.1.0
   hooks:
   - id: pycln
     args: [--config=pyproject.toml]
 - repo: https://github.com/PyCQA/isort
-  rev: 5.10.1
+  rev: 5.12.0
   hooks:
   - id: isort
     files: "\\.(py)$"
     args: [--settings-path=pyproject.toml]
 - repo: https://github.com/compilerla/conventional-pre-commit
   rev: v2.0.0
   hooks:
```

### Comparing `lyscripts-0.6.6/CHANGELOG.md` & `lyscripts-0.6.7/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+<a name="0.6.7"></a>
+## [0.6.7] - 2023-05-23
+
+### Bug Fixes
+- make flatten/unflatten funcs more consistent
+- add `max_depth` option for `flatten` function
+- bump isort version to avoid error
+
+### Features
+- add `unflatten` function
+
+
 <a name="0.6.6"></a>
 ## [0.6.6] - 2022-12-01
 
 ### Bug Fixes
 - pull another function out of a `rich` context, this time in the `join` command. Related to [#33].
 
 
@@ -226,15 +238,16 @@
 - set up git-chglog for creating changelogs
 - add pre-commit hook to check commit msg
 
 
 <a name="0.5.3"></a>
 ## [0.5.3] - 2022-08-22
 
-[Unreleased]: https://github.com/rmnldwg/lyscripts/compare/0.6.6...HEAD
+[Unreleased]: https://github.com/rmnldwg/lyscripts/compare/0.6.7...HEAD
+[0.6.7]: https://github.com/rmnldwg/lyscripts/compare/0.6.6...0.6.7
 [0.6.6]: https://github.com/rmnldwg/lyscripts/compare/0.6.5...0.6.6
 [0.6.5]: https://github.com/rmnldwg/lyscripts/compare/0.6.4...0.6.5
 [0.6.4]: https://github.com/rmnldwg/lyscripts/compare/0.6.3...0.6.4
 [0.6.3]: https://github.com/rmnldwg/lyscripts/compare/0.6.2...0.6.3
 [0.6.2]: https://github.com/rmnldwg/lyscripts/compare/0.6.1...0.6.2
 [0.6.1]: https://github.com/rmnldwg/lyscripts/compare/0.6.0...0.6.1
 [0.6.0]: https://github.com/rmnldwg/lyscripts/compare/0.5.11...0.6.0
```

### Comparing `lyscripts-0.6.6/LICENSE` & `lyscripts-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/PKG-INFO` & `lyscripts-0.6.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyscripts
-Version: 0.6.6
+Version: 0.6.7
 Summary: Package containing scripts used in lynference pipelines
 Author-email: Roman Ludwig <roman.ludwig@usz.ch>
 License: MIT
 Project-URL: source, https://github.com/rmnldwg/lyscripts
 Project-URL: documentation, https://rmnldwg.github.io/lyscripts
 Keywords: scripts,lymph,inference
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: apps
 License-File: LICENSE
 
-![social card](https://raw.githubusercontent.com/rmnldwg/lyscripts/main/github-social-card.png)
+<img src="https://raw.githubusercontent.com/rmnldwg/lyscripts/main/github-social-card.png" alt="social card" style="width:830px;"/>
 
 [![MIT license](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/rmnldwg/lyscripts/blob/main/LICENSE)
 [![GitHub repo](https://img.shields.io/badge/rmnldwg%2Flymph-grey.svg?style=flat&logo=github)](https://github.com/rmnldwg/lyscripts)
 [![build badge](https://github.com/rmnldwg/lyscripts/actions/workflows/build.yml/badge.svg?style=flat)](https://pypi.org/project/lyscripts/)
 [![docs badge](https://github.com/rmnldwg/lyscripts/actions/workflows/docs.yml/badge.svg?style=flat)](https://rmnldwg.github.io/lyscripts/)
 [![tests badge](https://github.com/rmnldwg/lyscripts/actions/workflows/tests.yml/badge.svg?style=flat)](https://rmnldwg.github.io/lyscripts/)
```

### Comparing `lyscripts-0.6.6/README.md` & `lyscripts-0.6.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![social card](https://raw.githubusercontent.com/rmnldwg/lyscripts/main/github-social-card.png)
+<img src="https://raw.githubusercontent.com/rmnldwg/lyscripts/main/github-social-card.png" alt="social card" style="width:830px;"/>
 
 [![MIT license](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/rmnldwg/lyscripts/blob/main/LICENSE)
 [![GitHub repo](https://img.shields.io/badge/rmnldwg%2Flymph-grey.svg?style=flat&logo=github)](https://github.com/rmnldwg/lyscripts)
 [![build badge](https://github.com/rmnldwg/lyscripts/actions/workflows/build.yml/badge.svg?style=flat)](https://pypi.org/project/lyscripts/)
 [![docs badge](https://github.com/rmnldwg/lyscripts/actions/workflows/docs.yml/badge.svg?style=flat)](https://rmnldwg.github.io/lyscripts/)
 [![tests badge](https://github.com/rmnldwg/lyscripts/actions/workflows/tests.yml/badge.svg?style=flat)](https://rmnldwg.github.io/lyscripts/)
```

### Comparing `lyscripts-0.6.6/favicon.png` & `lyscripts-0.6.7/favicon.png`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/github-social-card.png` & `lyscripts-0.6.7/github-social-card.png`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/lyscripts/__init__.py` & `lyscripts-0.6.7/lyscripts/__init__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/lyscripts/app/__init__.py` & `lyscripts-0.6.7/lyscripts/app/__init__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/lyscripts/app/prevalence.py` & `lyscripts-0.6.7/lyscripts/app/prevalence.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/lyscripts/data/__init__.py` & `lyscripts-0.6.7/lyscripts/data/__init__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/lyscripts/data/__main__.py` & `lyscripts-0.6.7/lyscripts/data/__main__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/lyscripts/data/clean.py` & `lyscripts-0.6.7/lyscripts/data/clean.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/lyscripts/data/enhance.py` & `lyscripts-0.6.7/lyscripts/data/enhance.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/lyscripts/data/generate.py` & `lyscripts-0.6.7/lyscripts/data/generate.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/lyscripts/data/join.py` & `lyscripts-0.6.7/lyscripts/data/join.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/lyscripts/data/lyproxify.py` & `lyscripts-0.6.7/lyscripts/data/lyproxify.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/lyscripts/data/split.py` & `lyscripts-0.6.7/lyscripts/data/split.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/lyscripts/data/utils.py` & `lyscripts-0.6.7/lyscripts/data/utils.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/lyscripts/evaluate.py` & `lyscripts-0.6.7/lyscripts/evaluate.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/lyscripts/plot/__init__.py` & `lyscripts-0.6.7/lyscripts/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/lyscripts/plot/__main__.py` & `lyscripts-0.6.7/lyscripts/plot/__main__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/lyscripts/plot/corner.py` & `lyscripts-0.6.7/lyscripts/plot/corner.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/lyscripts/plot/histograms.py` & `lyscripts-0.6.7/lyscripts/plot/histograms.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/lyscripts/plot/thermo_int.py` & `lyscripts-0.6.7/lyscripts/plot/thermo_int.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/lyscripts/plot/utils.py` & `lyscripts-0.6.7/lyscripts/plot/utils.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/lyscripts/predict/__init__.py` & `lyscripts-0.6.7/lyscripts/predict/__init__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/lyscripts/predict/__main__.py` & `lyscripts-0.6.7/lyscripts/predict/__main__.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/lyscripts/predict/prevalences.py` & `lyscripts-0.6.7/lyscripts/predict/prevalences.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/lyscripts/predict/risks.py` & `lyscripts-0.6.7/lyscripts/predict/risks.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/lyscripts/predict/utils.py` & `lyscripts-0.6.7/lyscripts/predict/utils.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/lyscripts/sample.py` & `lyscripts-0.6.7/lyscripts/sample.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/lyscripts/temp_schedule.py` & `lyscripts-0.6.7/lyscripts/temp_schedule.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/lyscripts/utils.py` & `lyscripts-0.6.7/lyscripts/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -453,42 +453,73 @@
 
     raise TypeError(f"Model cannot be of type {type(model)}")
 
 
 def flatten(
     nested: dict,
     prev_key: tuple = (),
-    flattened: Optional[dict] = None,
+    max_depth: Optional[int] = None,
 ) -> dict:
     """
-    Flatten a `nested` dictionary recursivel by extending the `prev_key` tuple. For
-    example:
-    >>> nested = {"hi": {"there": "buddy"}, "how": {"are": "you?"}}
+    Flatten a `nested` dictionary by creating key tuples for each value at `max_depth`.
+
+    For example:
+    >>> nested = {"tumor": {"1": {"t_stage": 1, "size": 12.3}}}
     >>> flatten(nested)
-    {('hi', 'there'): 'buddy', ('how', 'are'): 'you?'}
+    {('tumor', '1', 't_stage'): 1, ('tumor', '1', 'size'): 12.3}
+    >>> mapping = {"patient": {"#": {"age": {"func": int, "columns": ["age"]}}}}
+    >>> flatten(mapping, max_depth=3)
+    {('patient', '#', 'age'): {'func': <class 'int'>, 'columns': ['age']}}
     """
-    if flattened is None:
-        flattened = {}
+    result = {}
+
+    for key, value in nested.items():
+        is_dict = isinstance(value, dict)
+        has_reached_max_depth = max_depth is not None and len(prev_key) >= max_depth - 1
 
-    for key,val in nested.items():
-        if isinstance(val, dict):
-            flatten(val, (*prev_key, key), flattened)
+        if is_dict and not has_reached_max_depth:
+            result.update(flatten(value, (*prev_key, key), max_depth))
         else:
-            flattened[(*prev_key, key)] = val
+            result[(*prev_key, key)] = value
+
+    return result
 
-    return flattened
+
+def unflatten(flat: dict) -> dict:
+    """
+    Take a flat dictionary with tuples of keys and create nested dict from it.
+
+    Like so:
+    >>> flat = {('tumor', '1', 't_stage'): 1, ('tumor', '1', 'size'): 12.3}
+    >>> unflatten(flat)
+    {'tumor': {'1': {'t_stage': 1, 'size': 12.3}}}
+    >>> mapping = {('patient', '#', 'age'): {'func': int, 'columns': ['age']}}
+    >>> unflatten(mapping)
+    {'patient': {'#': {'age': {'func': <class 'int'>, 'columns': ['age']}}}}
+    """
+    result = {}
+
+    for keys, value in flat.items():
+        current = result
+        for key in keys[:-1]:
+            current = current.setdefault(key, {})
+
+        current[keys[-1]] = value
+
+    return result
 
 
 def get_modalities_subset(
     defined_modalities: Dict[str, List[float]],
     selection: List[str],
 ) -> Dict[str, List[float]]:
     """
-    Of the `defined_modalities` return only those mentioned in the `selection`. For
-    instance:
+    Of the `defined_modalities` return only those mentioned in the `selection`.
+
+    For instance:
     >>> modalities = {"CT": [0.76, 0.81], "MRI": [0.63, 0.86]}
     >>> get_modalities_subset(modalities, ["CT"])
     {'CT': [0.76, 0.81]}
     """
     selected_modalities = {}
     for mod in selection:
         try:
```

### Comparing `lyscripts-0.6.6/lyscripts.egg-info/PKG-INFO` & `lyscripts-0.6.7/lyscripts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyscripts
-Version: 0.6.6
+Version: 0.6.7
 Summary: Package containing scripts used in lynference pipelines
 Author-email: Roman Ludwig <roman.ludwig@usz.ch>
 License: MIT
 Project-URL: source, https://github.com/rmnldwg/lyscripts
 Project-URL: documentation, https://rmnldwg.github.io/lyscripts
 Keywords: scripts,lymph,inference
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: apps
 License-File: LICENSE
 
-![social card](https://raw.githubusercontent.com/rmnldwg/lyscripts/main/github-social-card.png)
+<img src="https://raw.githubusercontent.com/rmnldwg/lyscripts/main/github-social-card.png" alt="social card" style="width:830px;"/>
 
 [![MIT license](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/rmnldwg/lyscripts/blob/main/LICENSE)
 [![GitHub repo](https://img.shields.io/badge/rmnldwg%2Flymph-grey.svg?style=flat&logo=github)](https://github.com/rmnldwg/lyscripts)
 [![build badge](https://github.com/rmnldwg/lyscripts/actions/workflows/build.yml/badge.svg?style=flat)](https://pypi.org/project/lyscripts/)
 [![docs badge](https://github.com/rmnldwg/lyscripts/actions/workflows/docs.yml/badge.svg?style=flat)](https://rmnldwg.github.io/lyscripts/)
 [![tests badge](https://github.com/rmnldwg/lyscripts/actions/workflows/tests.yml/badge.svg?style=flat)](https://rmnldwg.github.io/lyscripts/)
```

### Comparing `lyscripts-0.6.6/lyscripts.egg-info/SOURCES.txt` & `lyscripts-0.6.7/lyscripts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/pyproject.toml` & `lyscripts-0.6.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/tests/_sample.py` & `lyscripts-0.6.7/tests/_sample.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/tests/plot/baseline/sine.png` & `lyscripts-0.6.7/tests/plot/baseline/sine.png`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/tests/plot/baseline/sine.svg` & `lyscripts-0.6.7/tests/plot/baseline/sine.svg`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/tests/plot/baseline/sine_svg.png` & `lyscripts-0.6.7/tests/plot/baseline/sine_svg.png`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/tests/plot/baseline/test_draw.png` & `lyscripts-0.6.7/tests/plot/baseline/test_draw.png`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/tests/plot/data/beta_samples.hdf5` & `lyscripts-0.6.7/tests/plot/data/beta_samples.hdf5`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/tests/plot/plot_utils_test.py` & `lyscripts-0.6.7/tests/plot/plot_utils_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -208,16 +208,21 @@
     save_figure_capture = capsys.readouterr()
 
     assert mpl_comp.compare_images(
         expected="./tests/plot/baseline/sine.png",
         actual="./tests/plot/results/sine.png",
         tol=0.,
     ) is None, "PNG of figure was not stored correctly."
-    assert mpl_comp.compare_images(
-        expected="./tests/plot/baseline/sine.svg",
-        actual="./tests/plot/results/sine.svg",
-        tol=0.,
-    ) is None, "SVG of figure was not stored correctly."
+
+    # Commented out, because I recently got the following message from matplotlib:
+    # `SKIPPED (Don't know how to convert .svg files to png)`
+    # So, I am commenting out this test for now.
+
+    # assert mpl_comp.compare_images(
+    #     expected="./tests/plot/baseline/sine.svg",
+    #     actual="./tests/plot/results/sine.svg",
+    #     tol=0.,
+    # ) is None, "SVG of figure was not stored correctly."
+
     assert save_figure_capture.out == expected_output, (
         "The output during the save figure procedure was wrong."
     )
-
```

### Comparing `lyscripts-0.6.6/tests/predict/predict_utils_test.py` & `lyscripts-0.6.7/tests/predict/predict_utils_test.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/tests/predict/prevalences_test.py` & `lyscripts-0.6.7/tests/predict/prevalences_test.py`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/tests/test_params.yaml` & `lyscripts-0.6.7/tests/test_params.yaml`

 * *Files identical despite different names*

### Comparing `lyscripts-0.6.6/tests/utils_test.py` & `lyscripts-0.6.7/tests/utils_test.py`

 * *Files identical despite different names*

