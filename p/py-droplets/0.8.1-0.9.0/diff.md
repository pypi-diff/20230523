# Comparing `tmp/py-droplets-0.8.1.tar.gz` & `tmp/py-droplets-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-droplets-0.8.1.tar", last modified: Thu Dec  9 07:32:01 2021, max compression
+gzip compressed data, was "py-droplets-0.9.0.tar", last modified: Tue Mar 15 16:48:38 2022, max compression
```

## Comparing `py-droplets-0.8.1.tar` & `py-droplets-0.9.0.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2021-12-09 07:32:01.934465 py-droplets-0.8.1/
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2021-12-09 07:32:01.909858 py-droplets-0.8.1/.github/
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2021-12-09 07:32:01.915924 py-droplets-0.8.1/.github/workflows/
--rw-r--r--   0 dzwicker   (501) staff       (20)     2001 2020-09-09 13:47:51.000000 py-droplets-0.8.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 dzwicker   (501) staff       (20)      938 2021-06-14 11:19:48.000000 py-droplets-0.8.1/.github/workflows/coverage_report.yml
--rw-r--r--   0 dzwicker   (501) staff       (20)      947 2021-06-14 11:19:48.000000 py-droplets-0.8.1/.github/workflows/python_tests.yml
--rw-r--r--   0 dzwicker   (501) staff       (20)     1466 2020-04-01 09:17:02.000000 py-droplets-0.8.1/.gitignore
--rw-r--r--   0 dzwicker   (501) staff       (20)      157 2021-01-06 14:08:16.000000 py-droplets-0.8.1/.isort.cfg
--rw-r--r--   0 dzwicker   (501) staff       (20)      264 2020-03-02 19:32:27.000000 py-droplets-0.8.1/.travis.yml
--rw-r--r--   0 dzwicker   (501) staff       (20)     1070 2020-03-02 18:37:51.000000 py-droplets-0.8.1/LICENSE
--rw-r--r--   0 dzwicker   (501) staff       (20)     2979 2021-12-09 07:32:01.934612 py-droplets-0.8.1/PKG-INFO
--rw-r--r--   0 dzwicker   (501) staff       (20)     2030 2020-07-24 10:01:57.000000 py-droplets-0.8.1/README.md
--rw-r--r--   0 dzwicker   (501) staff       (20)       51 2021-02-16 14:31:27.000000 py-droplets-0.8.1/TODO.md
--rw-r--r--   0 dzwicker   (501) staff       (20)      165 2020-03-30 19:10:19.000000 py-droplets-0.8.1/codecov.yml
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2021-12-09 07:32:01.916758 py-droplets-0.8.1/docs/
--rw-r--r--   0 dzwicker   (501) staff       (20)      584 2020-03-02 18:37:51.000000 py-droplets-0.8.1/docs/Makefile
--rwxr-xr-x   0 dzwicker   (501) staff       (20)       49 2020-03-02 18:37:51.000000 py-droplets-0.8.1/docs/build_all.sh
--rw-r--r--   0 dzwicker   (501) staff       (20)      117 2021-11-10 17:00:52.000000 py-droplets-0.8.1/docs/requirements.txt
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2021-12-09 07:32:01.918480 py-droplets-0.8.1/docs/source/
--rw-r--r--   0 dzwicker   (501) staff       (20)     7429 2021-10-21 06:55:24.000000 py-droplets-0.8.1/docs/source/conf.py
--rw-r--r--   0 dzwicker   (501) staff       (20)      409 2021-01-06 14:07:39.000000 py-droplets-0.8.1/docs/source/index.rst
--rw-r--r--   0 dzwicker   (501) staff       (20)     2779 2021-06-14 11:19:48.000000 py-droplets-0.8.1/docs/source/installation.rst
--rwxr-xr-x   0 dzwicker   (501) staff       (20)     1397 2020-07-24 10:01:57.000000 py-droplets-0.8.1/docs/source/parse_examples.py
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2021-12-09 07:32:01.919315 py-droplets-0.8.1/docs/source/quickstart/
--rw-r--r--   0 dzwicker   (501) staff       (20)     3076 2020-07-24 10:01:57.000000 py-droplets-0.8.1/docs/source/quickstart/contributing.rst
--rw-r--r--   0 dzwicker   (501) staff       (20)     1790 2020-04-17 07:57:33.000000 py-droplets-0.8.1/docs/source/quickstart/examples.rst
--rw-r--r--   0 dzwicker   (501) staff       (20)       99 2020-03-02 18:37:51.000000 py-droplets-0.8.1/docs/source/quickstart/quickstart.rst
--rwxr-xr-x   0 dzwicker   (501) staff       (20)     1729 2020-08-19 10:59:01.000000 py-droplets-0.8.1/docs/source/run_autodoc.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     3885 2020-08-19 10:59:01.000000 py-droplets-0.8.1/docs/source/sphinx_simplify_typehints.py
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2021-12-09 07:32:01.922100 py-droplets-0.8.1/droplets/
--rw-r--r--   0 dzwicker   (501) staff       (20)      465 2020-07-24 10:01:57.000000 py-droplets-0.8.1/droplets/__init__.py
--rw-r--r--   0 dzwicker   (501) staff       (20)      530 2021-06-17 13:35:53.000000 py-droplets-0.8.1/droplets/conftest.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    25790 2021-11-01 18:35:43.000000 py-droplets-0.8.1/droplets/droplet_tracks.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    42293 2021-11-26 16:19:54.000000 py-droplets-0.8.1/droplets/droplets.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    31088 2021-11-20 09:39:29.000000 py-droplets-0.8.1/droplets/emulsions.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    23385 2021-11-20 09:40:02.000000 py-droplets-0.8.1/droplets/image_analysis.py
--rw-r--r--   0 dzwicker   (501) staff       (20)       85 2020-11-23 18:28:49.000000 py-droplets-0.8.1/droplets/py.typed
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2021-12-09 07:32:01.923007 py-droplets-0.8.1/droplets/resources/
--rwxr--r--   0 dzwicker   (501) staff       (20)     1902 2020-09-16 12:39:15.000000 py-droplets-0.8.1/droplets/resources/make_spheres_3d.py
--rw-r--r--   0 dzwicker   (501) staff       (20)       32 2020-09-16 11:00:51.000000 py-droplets-0.8.1/droplets/resources/requirements.txt
--rw-r--r--   0 dzwicker   (501) staff       (20)   228936 2020-09-16 11:35:31.000000 py-droplets-0.8.1/droplets/resources/spheres_3d.hdf5
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2021-12-09 07:32:01.925167 py-droplets-0.8.1/droplets/tests/
--rw-r--r--   0 dzwicker   (501) staff       (20)     3962 2021-09-22 18:30:06.000000 py-droplets-0.8.1/droplets/tests/test_droplet_tracks.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     7257 2021-06-17 13:35:53.000000 py-droplets-0.8.1/droplets/tests/test_droplets.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     6217 2021-09-22 18:30:06.000000 py-droplets-0.8.1/droplets/tests/test_emulsion.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     1450 2021-06-17 13:35:53.000000 py-droplets-0.8.1/droplets/tests/test_examples.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     9791 2021-06-17 13:35:53.000000 py-droplets-0.8.1/droplets/tests/test_image_analysis.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     1517 2021-06-17 13:35:53.000000 py-droplets-0.8.1/droplets/tests/test_trackers.py
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2021-12-09 07:32:01.925689 py-droplets-0.8.1/droplets/tools/
--rw-r--r--   0 dzwicker   (501) staff       (20)        0 2021-11-26 16:19:54.000000 py-droplets-0.8.1/droplets/tools/__init__.py
--rw-r--r--   0 dzwicker   (501) staff       (20)    13249 2021-11-26 16:19:54.000000 py-droplets-0.8.1/droplets/tools/spherical.py
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2021-12-09 07:32:01.926192 py-droplets-0.8.1/droplets/tools/tests/
--rw-r--r--   0 dzwicker   (501) staff       (20)        0 2021-11-26 16:19:54.000000 py-droplets-0.8.1/droplets/tools/tests/__init__.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     4137 2021-11-26 16:19:54.000000 py-droplets-0.8.1/droplets/tools/tests/test_spherical.py
--rw-r--r--   0 dzwicker   (501) staff       (20)     8644 2021-11-20 09:40:14.000000 py-droplets-0.8.1/droplets/trackers.py
--rw-r--r--   0 dzwicker   (501) staff       (20)      136 2021-12-09 07:30:12.000000 py-droplets-0.8.1/droplets/version.py
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2021-12-09 07:32:01.927653 py-droplets-0.8.1/examples/
--rw-r--r--   0 dzwicker   (501) staff       (20)      352 2021-09-22 18:30:06.000000 py-droplets-0.8.1/examples/analyze_image.py
--rw-r--r--   0 dzwicker   (501) staff       (20)      352 2021-01-06 14:08:41.000000 py-droplets-0.8.1/examples/analyze_simulation.py
--rw-r--r--   0 dzwicker   (501) staff       (20)      401 2020-07-24 10:01:57.000000 py-droplets-0.8.1/examples/define_droplets.py
--rw-r--r--   0 dzwicker   (501) staff       (20)      429 2020-08-19 10:59:01.000000 py-droplets-0.8.1/examples/plot_emulsion.py
--rw-r--r--   0 dzwicker   (501) staff       (20)      498 2021-09-22 18:30:06.000000 py-droplets-0.8.1/examples/plot_emulsion_properties.py
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2021-12-09 07:32:01.927930 py-droplets-0.8.1/examples/resources/
--rw-r--r--   0 dzwicker   (501) staff       (20)    12396 2021-09-22 18:30:06.000000 py-droplets-0.8.1/examples/resources/emulsion.png
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2021-12-09 07:32:01.928214 py-droplets-0.8.1/examples/tutorial/
--rw-r--r--   0 dzwicker   (501) staff       (20)   488989 2020-04-15 12:36:25.000000 py-droplets-0.8.1/examples/tutorial/Using the py-droplets package.ipynb
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2021-12-09 07:32:01.930641 py-droplets-0.8.1/py_droplets.egg-info/
--rw-r--r--   0 dzwicker   (501) staff       (20)     2979 2021-12-09 07:32:01.000000 py-droplets-0.8.1/py_droplets.egg-info/PKG-INFO
--rw-r--r--   0 dzwicker   (501) staff       (20)     1908 2021-12-09 07:32:01.000000 py-droplets-0.8.1/py_droplets.egg-info/SOURCES.txt
--rw-r--r--   0 dzwicker   (501) staff       (20)        1 2021-12-09 07:32:01.000000 py-droplets-0.8.1/py_droplets.egg-info/dependency_links.txt
--rw-r--r--   0 dzwicker   (501) staff       (20)        1 2021-12-09 07:32:01.000000 py-droplets-0.8.1/py_droplets.egg-info/not-zip-safe
--rw-r--r--   0 dzwicker   (501) staff       (20)       57 2021-12-09 07:32:01.000000 py-droplets-0.8.1/py_droplets.egg-info/requires.txt
--rw-r--r--   0 dzwicker   (501) staff       (20)        9 2021-12-09 07:32:01.000000 py-droplets-0.8.1/py_droplets.egg-info/top_level.txt
--rw-r--r--   0 dzwicker   (501) staff       (20)       86 2021-09-22 18:30:06.000000 py-droplets-0.8.1/requirements.txt
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2021-12-09 07:32:01.931215 py-droplets-0.8.1/scripts/
--rwxr-xr-x   0 dzwicker   (501) staff       (20)      269 2021-09-17 09:53:59.000000 py-droplets-0.8.1/scripts/format_code.sh
--rwxr--r--   0 dzwicker   (501) staff       (20)      274 2021-12-09 07:31:51.000000 py-droplets-0.8.1/scripts/upload_to_pypi.sh
--rw-r--r--   0 dzwicker   (501) staff       (20)       79 2021-12-09 07:32:01.935091 py-droplets-0.8.1/setup.cfg
--rw-r--r--   0 dzwicker   (501) staff       (20)     1679 2021-06-14 11:19:48.000000 py-droplets-0.8.1/setup.py
-drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2021-12-09 07:32:01.934226 py-droplets-0.8.1/tests/
--rw-r--r--   0 dzwicker   (501) staff       (20)       24 2020-04-01 09:15:56.000000 py-droplets-0.8.1/tests/.coveragerc
--rw-r--r--   0 dzwicker   (501) staff       (20)      830 2020-09-16 12:36:10.000000 py-droplets-0.8.1/tests/mypy.ini
--rw-r--r--   0 dzwicker   (501) staff       (20)      237 2020-11-23 19:11:44.000000 py-droplets-0.8.1/tests/pytest.ini
--rw-r--r--   0 dzwicker   (501) staff       (20)      104 2020-08-19 10:58:02.000000 py-droplets-0.8.1/tests/requirements.txt
--rwxr-xr-x   0 dzwicker   (501) staff       (20)     7221 2021-06-14 11:19:48.000000 py-droplets-0.8.1/tests/run_tests.py
--rwxr-xr-x   0 dzwicker   (501) staff       (20)      197 2020-07-24 10:01:57.000000 py-droplets-0.8.1/tests/tests_all.sh
--rwxr-xr-x   0 dzwicker   (501) staff       (20)      123 2020-11-25 12:17:54.000000 py-droplets-0.8.1/tests/tests_codestyle.sh
--rwxr-xr-x   0 dzwicker   (501) staff       (20)      191 2020-11-25 12:17:54.000000 py-droplets-0.8.1/tests/tests_coverage.sh
--rwxr-xr-x   0 dzwicker   (501) staff       (20)      354 2020-11-25 12:17:54.000000 py-droplets-0.8.1/tests/tests_parallel.sh
--rwxr-xr-x   0 dzwicker   (501) staff       (20)      332 2020-11-25 12:17:54.000000 py-droplets-0.8.1/tests/tests_run.sh
--rwxr-xr-x   0 dzwicker   (501) staff       (20)      161 2021-01-25 08:02:13.000000 py-droplets-0.8.1/tests/tests_types.sh
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2022-03-15 16:48:38.092008 py-droplets-0.9.0/
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2022-03-15 16:48:38.061989 py-droplets-0.9.0/.github/
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2022-03-15 16:48:38.070011 py-droplets-0.9.0/.github/workflows/
+-rw-r--r--   0 dzwicker   (501) staff       (20)     2001 2020-09-09 13:47:51.000000 py-droplets-0.9.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 dzwicker   (501) staff       (20)      938 2021-06-14 11:19:48.000000 py-droplets-0.9.0/.github/workflows/coverage_report.yml
+-rw-r--r--   0 dzwicker   (501) staff       (20)      952 2022-03-15 16:43:52.000000 py-droplets-0.9.0/.github/workflows/python_tests.yml
+-rw-r--r--   0 dzwicker   (501) staff       (20)     1466 2020-04-01 09:17:02.000000 py-droplets-0.9.0/.gitignore
+-rw-r--r--   0 dzwicker   (501) staff       (20)      157 2021-01-06 14:08:16.000000 py-droplets-0.9.0/.isort.cfg
+-rw-r--r--   0 dzwicker   (501) staff       (20)      264 2020-03-02 19:32:27.000000 py-droplets-0.9.0/.travis.yml
+-rw-r--r--   0 dzwicker   (501) staff       (20)     1070 2020-03-02 18:37:51.000000 py-droplets-0.9.0/LICENSE
+-rw-r--r--   0 dzwicker   (501) staff       (20)     3030 2022-03-15 16:48:38.092158 py-droplets-0.9.0/PKG-INFO
+-rw-r--r--   0 dzwicker   (501) staff       (20)     2030 2020-07-24 10:01:57.000000 py-droplets-0.9.0/README.md
+-rw-r--r--   0 dzwicker   (501) staff       (20)       51 2021-02-16 14:31:27.000000 py-droplets-0.9.0/TODO.md
+-rw-r--r--   0 dzwicker   (501) staff       (20)      165 2020-03-30 19:10:19.000000 py-droplets-0.9.0/codecov.yml
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2022-03-15 16:48:38.071153 py-droplets-0.9.0/docs/
+-rw-r--r--   0 dzwicker   (501) staff       (20)      584 2020-03-02 18:37:51.000000 py-droplets-0.9.0/docs/Makefile
+-rwxr-xr-x   0 dzwicker   (501) staff       (20)       49 2020-03-02 18:37:51.000000 py-droplets-0.9.0/docs/build_all.sh
+-rw-r--r--   0 dzwicker   (501) staff       (20)      117 2021-11-10 17:00:52.000000 py-droplets-0.9.0/docs/requirements.txt
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2022-03-15 16:48:38.073474 py-droplets-0.9.0/docs/source/
+-rw-r--r--   0 dzwicker   (501) staff       (20)     7429 2021-10-21 06:55:24.000000 py-droplets-0.9.0/docs/source/conf.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)      409 2021-01-06 14:07:39.000000 py-droplets-0.9.0/docs/source/index.rst
+-rw-r--r--   0 dzwicker   (501) staff       (20)     2779 2021-06-14 11:19:48.000000 py-droplets-0.9.0/docs/source/installation.rst
+-rwxr-xr-x   0 dzwicker   (501) staff       (20)     1397 2020-07-24 10:01:57.000000 py-droplets-0.9.0/docs/source/parse_examples.py
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2022-03-15 16:48:38.074656 py-droplets-0.9.0/docs/source/quickstart/
+-rw-r--r--   0 dzwicker   (501) staff       (20)     3076 2020-07-24 10:01:57.000000 py-droplets-0.9.0/docs/source/quickstart/contributing.rst
+-rw-r--r--   0 dzwicker   (501) staff       (20)     1790 2020-04-17 07:57:33.000000 py-droplets-0.9.0/docs/source/quickstart/examples.rst
+-rw-r--r--   0 dzwicker   (501) staff       (20)       99 2020-03-02 18:37:51.000000 py-droplets-0.9.0/docs/source/quickstart/quickstart.rst
+-rwxr-xr-x   0 dzwicker   (501) staff       (20)     1729 2020-08-19 10:59:01.000000 py-droplets-0.9.0/docs/source/run_autodoc.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     3885 2020-08-19 10:59:01.000000 py-droplets-0.9.0/docs/source/sphinx_simplify_typehints.py
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2022-03-15 16:48:38.078145 py-droplets-0.9.0/droplets/
+-rw-r--r--   0 dzwicker   (501) staff       (20)      465 2020-07-24 10:01:57.000000 py-droplets-0.9.0/droplets/__init__.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)      530 2021-06-17 13:35:53.000000 py-droplets-0.9.0/droplets/conftest.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    25790 2021-11-01 18:35:43.000000 py-droplets-0.9.0/droplets/droplet_tracks.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    42239 2022-03-15 16:43:52.000000 py-droplets-0.9.0/droplets/droplets.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    31104 2022-03-15 16:43:52.000000 py-droplets-0.9.0/droplets/emulsions.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    23475 2022-03-15 16:43:52.000000 py-droplets-0.9.0/droplets/image_analysis.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)       85 2020-11-23 18:28:49.000000 py-droplets-0.9.0/droplets/py.typed
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2022-03-15 16:48:38.079273 py-droplets-0.9.0/droplets/resources/
+-rwxr--r--   0 dzwicker   (501) staff       (20)     1902 2020-09-16 12:39:15.000000 py-droplets-0.9.0/droplets/resources/make_spheres_3d.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)       32 2020-09-16 11:00:51.000000 py-droplets-0.9.0/droplets/resources/requirements.txt
+-rw-r--r--   0 dzwicker   (501) staff       (20)   228936 2020-09-16 11:35:31.000000 py-droplets-0.9.0/droplets/resources/spheres_3d.hdf5
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2022-03-15 16:48:38.081419 py-droplets-0.9.0/droplets/tests/
+-rw-r--r--   0 dzwicker   (501) staff       (20)     3962 2021-09-22 18:30:06.000000 py-droplets-0.9.0/droplets/tests/test_droplet_tracks.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     7249 2022-03-15 16:43:52.000000 py-droplets-0.9.0/droplets/tests/test_droplets.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     6217 2021-09-22 18:30:06.000000 py-droplets-0.9.0/droplets/tests/test_emulsion.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     1450 2021-06-17 13:35:53.000000 py-droplets-0.9.0/droplets/tests/test_examples.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     9791 2021-06-17 13:35:53.000000 py-droplets-0.9.0/droplets/tests/test_image_analysis.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     1517 2021-06-17 13:35:53.000000 py-droplets-0.9.0/droplets/tests/test_trackers.py
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2022-03-15 16:48:38.081933 py-droplets-0.9.0/droplets/tools/
+-rw-r--r--   0 dzwicker   (501) staff       (20)        0 2021-11-26 16:19:54.000000 py-droplets-0.9.0/droplets/tools/__init__.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)    13097 2022-03-15 16:43:52.000000 py-droplets-0.9.0/droplets/tools/spherical.py
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2022-03-15 16:48:38.082490 py-droplets-0.9.0/droplets/tools/tests/
+-rw-r--r--   0 dzwicker   (501) staff       (20)        0 2021-11-26 16:19:54.000000 py-droplets-0.9.0/droplets/tools/tests/__init__.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     4137 2021-11-26 16:19:54.000000 py-droplets-0.9.0/droplets/tools/tests/test_spherical.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)     8644 2021-11-20 09:40:14.000000 py-droplets-0.9.0/droplets/trackers.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)      136 2022-03-15 16:43:35.000000 py-droplets-0.9.0/droplets/version.py
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2022-03-15 16:48:38.084107 py-droplets-0.9.0/examples/
+-rw-r--r--   0 dzwicker   (501) staff       (20)      352 2021-09-22 18:30:06.000000 py-droplets-0.9.0/examples/analyze_image.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)      352 2021-01-06 14:08:41.000000 py-droplets-0.9.0/examples/analyze_simulation.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)      401 2020-07-24 10:01:57.000000 py-droplets-0.9.0/examples/define_droplets.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)      429 2020-08-19 10:59:01.000000 py-droplets-0.9.0/examples/plot_emulsion.py
+-rw-r--r--   0 dzwicker   (501) staff       (20)      498 2021-09-22 18:30:06.000000 py-droplets-0.9.0/examples/plot_emulsion_properties.py
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2022-03-15 16:48:38.084425 py-droplets-0.9.0/examples/resources/
+-rw-r--r--   0 dzwicker   (501) staff       (20)    12396 2021-09-22 18:30:06.000000 py-droplets-0.9.0/examples/resources/emulsion.png
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2022-03-15 16:48:38.084752 py-droplets-0.9.0/examples/tutorial/
+-rw-r--r--   0 dzwicker   (501) staff       (20)   488989 2020-04-15 12:36:25.000000 py-droplets-0.9.0/examples/tutorial/Using the py-droplets package.ipynb
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2022-03-15 16:48:38.087350 py-droplets-0.9.0/py_droplets.egg-info/
+-rw-r--r--   0 dzwicker   (501) staff       (20)     3030 2022-03-15 16:48:37.000000 py-droplets-0.9.0/py_droplets.egg-info/PKG-INFO
+-rw-r--r--   0 dzwicker   (501) staff       (20)     1908 2022-03-15 16:48:37.000000 py-droplets-0.9.0/py_droplets.egg-info/SOURCES.txt
+-rw-r--r--   0 dzwicker   (501) staff       (20)        1 2022-03-15 16:48:37.000000 py-droplets-0.9.0/py_droplets.egg-info/dependency_links.txt
+-rw-r--r--   0 dzwicker   (501) staff       (20)        1 2022-03-15 16:48:37.000000 py-droplets-0.9.0/py_droplets.egg-info/not-zip-safe
+-rw-r--r--   0 dzwicker   (501) staff       (20)       57 2022-03-15 16:48:37.000000 py-droplets-0.9.0/py_droplets.egg-info/requires.txt
+-rw-r--r--   0 dzwicker   (501) staff       (20)        9 2022-03-15 16:48:37.000000 py-droplets-0.9.0/py_droplets.egg-info/top_level.txt
+-rw-r--r--   0 dzwicker   (501) staff       (20)       86 2022-03-15 16:43:52.000000 py-droplets-0.9.0/requirements.txt
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2022-03-15 16:48:38.087982 py-droplets-0.9.0/scripts/
+-rwxr-xr-x   0 dzwicker   (501) staff       (20)      269 2021-09-17 09:53:59.000000 py-droplets-0.9.0/scripts/format_code.sh
+-rwxr--r--   0 dzwicker   (501) staff       (20)      274 2022-03-15 16:48:33.000000 py-droplets-0.9.0/scripts/upload_to_pypi.sh
+-rw-r--r--   0 dzwicker   (501) staff       (20)       79 2022-03-15 16:48:38.092754 py-droplets-0.9.0/setup.cfg
+-rw-r--r--   0 dzwicker   (501) staff       (20)     1729 2022-03-15 16:43:52.000000 py-droplets-0.9.0/setup.py
+drwxr-xr-x   0 dzwicker   (501) staff       (20)        0 2022-03-15 16:48:38.091748 py-droplets-0.9.0/tests/
+-rw-r--r--   0 dzwicker   (501) staff       (20)       24 2020-04-01 09:15:56.000000 py-droplets-0.9.0/tests/.coveragerc
+-rw-r--r--   0 dzwicker   (501) staff       (20)      902 2022-03-15 16:43:52.000000 py-droplets-0.9.0/tests/mypy.ini
+-rw-r--r--   0 dzwicker   (501) staff       (20)      237 2020-11-23 19:11:44.000000 py-droplets-0.9.0/tests/pytest.ini
+-rw-r--r--   0 dzwicker   (501) staff       (20)      104 2020-08-19 10:58:02.000000 py-droplets-0.9.0/tests/requirements.txt
+-rwxr-xr-x   0 dzwicker   (501) staff       (20)     7221 2021-06-14 11:19:48.000000 py-droplets-0.9.0/tests/run_tests.py
+-rwxr-xr-x   0 dzwicker   (501) staff       (20)      197 2020-07-24 10:01:57.000000 py-droplets-0.9.0/tests/tests_all.sh
+-rwxr-xr-x   0 dzwicker   (501) staff       (20)      123 2020-11-25 12:17:54.000000 py-droplets-0.9.0/tests/tests_codestyle.sh
+-rwxr-xr-x   0 dzwicker   (501) staff       (20)      191 2020-11-25 12:17:54.000000 py-droplets-0.9.0/tests/tests_coverage.sh
+-rwxr-xr-x   0 dzwicker   (501) staff       (20)      354 2020-11-25 12:17:54.000000 py-droplets-0.9.0/tests/tests_parallel.sh
+-rwxr-xr-x   0 dzwicker   (501) staff       (20)      332 2020-11-25 12:17:54.000000 py-droplets-0.9.0/tests/tests_run.sh
+-rwxr-xr-x   0 dzwicker   (501) staff       (20)      161 2021-01-25 08:02:13.000000 py-droplets-0.9.0/tests/tests_types.sh
```

### Comparing `py-droplets-0.8.1/.github/workflows/codeql-analysis.yml` & `py-droplets-0.9.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `py-droplets-0.8.1/.github/workflows/coverage_report.yml` & `py-droplets-0.9.0/.github/workflows/coverage_report.yml`

 * *Files identical despite different names*

### Comparing `py-droplets-0.8.1/.gitignore` & `py-droplets-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `py-droplets-0.8.1/LICENSE` & `py-droplets-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-droplets-0.8.1/PKG-INFO` & `py-droplets-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: py-droplets
-Version: 0.8.1
+Version: 0.9.0
 Summary: Python package for describing and analyzing droplets in experiments and simulations
 Home-page: https://github.com/zwicker-group/py-droplets
 Author: David Zwicker
 Author-email: david.zwicker@ds.mpg.de
 License: MIT
-Download-URL: https://github.com/zwicker-group/py-droplets/archive/v0.8.1.tar.gz
+Download-URL: https://github.com/zwicker-group/py-droplets/archive/v0.9.0.tar.gz
 Keywords: emulsions,image-analysis
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: hdf
 License-File: LICENSE
 
 # py-droplets
```

### Comparing `py-droplets-0.8.1/README.md` & `py-droplets-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `py-droplets-0.8.1/docs/Makefile` & `py-droplets-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `py-droplets-0.8.1/docs/source/conf.py` & `py-droplets-0.9.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `py-droplets-0.8.1/docs/source/installation.rst` & `py-droplets-0.9.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `py-droplets-0.8.1/docs/source/parse_examples.py` & `py-droplets-0.9.0/docs/source/parse_examples.py`

 * *Files identical despite different names*

### Comparing `py-droplets-0.8.1/docs/source/quickstart/contributing.rst` & `py-droplets-0.9.0/docs/source/quickstart/contributing.rst`

 * *Files identical despite different names*

### Comparing `py-droplets-0.8.1/docs/source/quickstart/examples.rst` & `py-droplets-0.9.0/docs/source/quickstart/examples.rst`

 * *Files identical despite different names*

### Comparing `py-droplets-0.8.1/docs/source/run_autodoc.py` & `py-droplets-0.9.0/docs/source/run_autodoc.py`

 * *Files identical despite different names*

### Comparing `py-droplets-0.8.1/docs/source/sphinx_simplify_typehints.py` & `py-droplets-0.9.0/docs/source/sphinx_simplify_typehints.py`

 * *Files identical despite different names*

### Comparing `py-droplets-0.8.1/droplets/conftest.py` & `py-droplets-0.9.0/droplets/conftest.py`

 * *Files identical despite different names*

### Comparing `py-droplets-0.8.1/droplets/droplet_tracks.py` & `py-droplets-0.9.0/droplets/droplet_tracks.py`

 * *Files identical despite different names*

### Comparing `py-droplets-0.8.1/droplets/droplets.py` & `py-droplets-0.9.0/droplets/droplets.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
                 The data array used to initialize the droplet
         """
         # note that we do not call the __init__ method of the class, since we do
         # not need to invent the dtype and set all the attributes. We here
         # simply assume that the given data is sane
         obj = cls.__new__(cls)
         obj.data = data
-        return obj  # type: ignore
+        return obj
 
     @classmethod
     def from_droplet(cls, droplet: DropletBase, **kwargs) -> DropletBase:
         r"""return a droplet with data taken from `droplet`
 
         Args:
             droplet (:class:`DropletBase`):
@@ -131,15 +131,15 @@
                 same type of droplet
             \**kwargs:
                 Additional arguments that can overwrite data in `droplet` or
                 set additional arguments for the current class
         """
         args = droplet._args
         args.update(kwargs)
-        return cls(**args)  # type: ignore
+        return cls(**args)
 
     @classmethod
     @abstractmethod
     def get_dtype(cls, **kwargs):
         """determine the dtype representing this droplet class
 
         Returns:
@@ -460,15 +460,15 @@
         elif self.dim == 3:
             # estimate the number of triangles covering the surface
             try:
                 surface_area = self.surface_area
             except (NotImplementedError, AttributeError):
                 # estimate surface area from 3d spherical droplet
                 surface_area = spherical.surface_from_radius(self.radius, dim=3)
-            num_est = (4 * surface_area) / (np.sqrt(3) * resolution ** 2)
+            num_est = (4 * surface_area) / (np.sqrt(3) * resolution**2)
             tri = triangulated_spheres.get_triangulation(num_est)
 
             φ, θ = tri["angles"][:, 0], tri["angles"][:, 1]
             return {
                 "vertices": self.interface_position(θ, φ),
                 "triangles": tri["cells"],
             }
@@ -622,17 +622,17 @@
         # calculate distances from droplet center
         dist: np.ndarray = grid.polar_coordinates_real(self.position, ret_angle=False)  # type: ignore
 
         # make the image
         if interface_width == 0 or dtype == np.bool_:
             result = dist < self.radius
         else:
-            result = 0.5 + 0.5 * np.tanh((self.radius - dist) / interface_width)
+            result = 0.5 + 0.5 * np.tanh((self.radius - dist) / interface_width)  # type: ignore
 
-        return result.astype(dtype)  # type: ignore
+        return result.astype(dtype)
 
 
 class PerturbedDropletBase(DiffuseDroplet, metaclass=ABCMeta):
     """represents a single droplet with a perturbed shape.
 
     This acts as an abstract class for which member functions need to specified
     depending on dimensionality.
@@ -889,21 +889,21 @@
             if b != 0:
                 curv_radius -= b * factor * np.cos(n * φ)
         return 1 / (self.radius * curv_radius)
 
     @property
     def volume(self) -> float:
         """float: volume of the droplet"""
-        term = 1 + np.sum(self.amplitudes ** 2) / 2
-        return np.pi * self.radius ** 2 * term  # type: ignore
+        term = 1 + np.sum(self.amplitudes**2) / 2
+        return np.pi * self.radius**2 * term  # type: ignore
 
     @volume.setter
     def volume(self, volume: float):
         """set volume keeping relative perturbations"""
-        term = 1 + np.sum(self.amplitudes ** 2) / 2
+        term = 1 + np.sum(self.amplitudes**2) / 2
         self.radius = np.sqrt(volume / (np.pi * term))
 
     @property
     def surface_area(self) -> float:
         """float: surface area of the droplet"""
         # discretize surface for simple approximation to integral
         φs, dφ = np.linspace(0, 2 * np.pi, 256, endpoint=False, retstep=True)
@@ -925,15 +925,15 @@
         return self.radius * line_element.sum() * dφ  # type: ignore
 
     @property
     def surface_area_approx(self) -> float:
         """float: surface area of the droplet (quadratic in amplitudes)"""
         length = 4
         for n, (a, b) in enumerate(iterate_in_pairs(self.amplitudes), 1):  # no 0th mode
-            length += n ** 2 * (a ** 2 + b ** 2)
+            length += n**2 * (a**2 + b**2)
         return np.pi * self.radius * length / 2
 
     def _get_mpl_patch(self, dim=2, **kwargs):
         """return the patch representing the droplet for plotting
 
         Args:
             dim (int, optional):
@@ -1066,26 +1066,26 @@
             with the angles
         """
         Yk = spherical.spherical_harmonic_real_k
         correction = 0
         for k, a in enumerate(self.amplitudes, 1):  # skip zero-th mode!
             if a != 0:
                 l, _ = spherical.spherical_index_lm(k)
-                hk = (l ** 2 + l - 2) / 2
+                hk = (l**2 + l - 2) / 2
                 correction = a * hk * Yk(k, θ, φ)
-        return 1 / self.radius + correction / self.radius ** 2
+        return 1 / self.radius + correction / self.radius**2
 
     @property
     def volume(self) -> float:
         """float: volume of the droplet (determined numerically)"""
 
         def integrand(θ, φ):
             """helper function calculating the integrand"""
             r = self.interface_distance(θ, φ)
-            return r ** 3 * np.sin(θ) / 3
+            return r**3 * np.sin(θ) / 3
 
         volume = integrate.dblquad(
             integrand, 0, 2 * np.pi, lambda _: 0, lambda _: np.pi
         )[0]
         return volume  # type: ignore
 
     @volume.setter
@@ -1094,15 +1094,15 @@
         raise NotImplementedError("Cannot set volume")
 
     @property
     def volume_approx(self) -> float:
         """float: approximate volume to linear order in the perturbation"""
         volume = spherical.volume_from_radius(self.radius, 3)
         if len(self.amplitudes) > 0:
-            volume += self.amplitudes[0] * 2 * np.sqrt(np.pi) * self.radius ** 2
+            volume += self.amplitudes[0] * 2 * np.sqrt(np.pi) * self.radius**2
         return volume
 
     def _get_mpl_patch(self, dim=None, *, color=None, **kwargs):
         """return the patch representing the droplet for plotting
 
         Args:
             dim (int, optional): The dimension in which the data is plotted. If omitted,
```

### Comparing `py-droplets-0.8.1/droplets/emulsions.py` & `py-droplets-0.9.0/droplets/emulsions.py`

 * *Files 1% similar despite different names*

```diff
@@ -452,15 +452,15 @@
         np.fill_diagonal(dists, np.inf)
 
         while len(dists) > 1:
             # find minimal distance
             x, y = np.unravel_index(np.argmin(dists), dists.shape)
             if dists[x, y] < min_distance:
                 # droplets overlap -> remove the smaller one
-                if self[x].radius > self[y].radius:
+                if self[x].radius > self[y].radius:  # type: ignore
                     self.pop(y)
                     dists = np.delete(np.delete(dists, y, 0), y, 1)
                 else:
                     self.pop(x)
                     dists = np.delete(np.delete(dists, x, 0), x, 1)
             else:
                 break
```

### Comparing `py-droplets-0.8.1/droplets/image_analysis.py` & `py-droplets-0.9.0/droplets/image_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
     # create and emulsion from this of droplets
     grid._logger.info(f"Found {num_labels} droplet candidate(s)")
 
     # determine position from binary image and scale it to real space
     positions = ndimage.measurements.center_of_mass(mask_padded, labels, index=indices)
     # correct for the additional padding of the array
-    positions = grid.cell_to_point(positions - offset)
+    positions = grid.transform(positions - offset, "cell", "grid")
 
     # determine volume from binary image and scale it to real space
     volumes = ndimage.measurements.sum(mask_padded, labels, index=indices)
     volumes = np.asanyarray(volumes) * np.prod(grid.discretization)
 
     # only retain droplets that are inside the central area
     droplets = (
@@ -131,15 +131,15 @@
         return Emulsion([], grid=grid)
 
     # locate clusters around origin
     object_slices = ndimage.measurements.find_objects(labels)
     droplet = None
     for slices in object_slices:
         if slices[0].start == 0:  # contains point around origin
-            radius = float(grid.cell_to_point(slices[0].stop).flat[-1])  # type: ignore
+            radius = float(grid.transform(slices[0].stop, "cell", "grid").flat[-1])
             droplet = SphericalDroplet(np.zeros(grid.dim), radius=radius)
         else:
             logger = logging.getLogger(grid.__class__.__module__)
             logger.warning("Found object not located at origin")
 
     # return an emulsion of droplets
     if droplet:
@@ -173,15 +173,15 @@
             indices.append(index)
         else:
             logger = logging.getLogger(grid.__class__.__module__)
             logger.warning("Found object not located on symmetry axis")
 
     # determine position from binary image and scale it to real space
     pos = ndimage.measurements.center_of_mass(mask, labels, index=indices)
-    pos = grid.cell_to_point(pos)
+    pos = grid.transform(pos, "cell", "cartesian")
 
     # determine volume from binary image and scale it to real space
     vol_r, dz = grid.cell_volume_data
     cell_volumes = vol_r * dz
     vol = ndimage.measurements.sum(cell_volumes, labels, index=indices)
 
     # return an emulsion of droplets
@@ -209,28 +209,29 @@
     assert np.all(mask.shape == grid.shape)
 
     if grid.periodic[1]:
         # locate droplets respecting periodic boundary conditions in z-direction
 
         # pad the array to simulate periodic boundary conditions
         dim_r, dim_z = grid.shape
+        z_min, z_max = grid.axes_bounds[1]
         mask_padded = np.pad(mask, [[0, 0], [dim_z, dim_z]], mode="wrap")
         assert mask_padded.shape == (dim_r, 3 * dim_z)
 
         # locate droplets in the extended image
         candidates = _locate_droplets_in_mask_cylindrical_single(grid, mask_padded)
         grid._logger.info(f"Found {len(candidates)} droplet candidates.")
 
         # keep droplets that are inside the central area
         droplets = Emulsion(grid=grid)
         for droplet in candidates:
             # correct for the additional padding of the array
             droplet.position[2] -= grid.length
             # check whether the droplet lies in the original box
-            if grid.contains_point(droplet.position):
+            if z_min <= droplet.position[2] <= z_max:
                 droplets.append(droplet)
 
         grid._logger.info(f"Kept {len(droplets)} central droplets.")
 
         # filter overlapping droplets (e.g. due to duplicates)
         droplets.remove_overlapping()
 
@@ -429,16 +430,16 @@
         _image_deviation, data_flat[free], bounds=bounds, **least_squares_params
     )
     data_flat[free] = result.x
     droplet.data = unstructured_to_structured(data_flat, dtype=dtype)
 
     # normalize the droplet position
     grid = phase_field.grid
-    coords = grid.point_from_cartesian(droplet.position)
-    droplet.position = grid.point_to_cartesian(grid.normalize_point(coords))
+    coords = grid.transform(droplet.position, "cartesian", "grid")
+    droplet.position = grid.transform(grid.normalize_point(coords), "grid", "cartesian")
 
     return droplet
 
 
 def get_structure_factor(
     scalar_field: ScalarField,
     smoothing: Union[None, float, str] = "auto",
```

### Comparing `py-droplets-0.8.1/droplets/resources/make_spheres_3d.py` & `py-droplets-0.9.0/droplets/resources/make_spheres_3d.py`

 * *Files identical despite different names*

### Comparing `py-droplets-0.8.1/droplets/resources/spheres_3d.hdf5` & `py-droplets-0.9.0/droplets/resources/spheres_3d.hdf5`

 * *Files identical despite different names*

### Comparing `py-droplets-0.8.1/droplets/tests/test_droplet_tracks.py` & `py-droplets-0.9.0/droplets/tests/test_droplet_tracks.py`

 * *Files identical despite different names*

### Comparing `py-droplets-0.8.1/droplets/tests/test_droplets.py` & `py-droplets-0.9.0/droplets/tests/test_droplets.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,27 +76,27 @@
     pos = np.random.randn(2)
     radius = 1 + np.random.random()
     amplitudes = np.random.uniform(-0.2, 0.2, 6)
     d = droplets.PerturbedDroplet2D(pos, radius, 0, amplitudes)
 
     def integrand(φ):
         r = d.interface_distance(φ)
-        return 0.5 * r ** 2
+        return 0.5 * r**2
 
     vol = integrate.quad(integrand, 0, 2 * np.pi)[0]
     assert vol == pytest.approx(d.volume)
 
     vol = np.random.uniform(1, 2)
     d.volume = vol
     assert vol == pytest.approx(d.volume)
 
     pos = np.random.randn(3)
     radius = 1 + np.random.random()
     d = droplets.PerturbedDroplet3D(pos, radius, 0, np.zeros(7))
-    assert d.volume == pytest.approx(4 * np.pi / 3 * radius ** 3)
+    assert d.volume == pytest.approx(4 * np.pi / 3 * radius**3)
 
 
 def test_surface_area():
     """test surface area calculation of droplets"""
     # perturbed 2d droplet
     R0 = 3
     amplitudes = np.random.uniform(-1e-2, 1e-2, 6)
@@ -127,15 +127,15 @@
     amplitudes = epsilon * np.array([0.1, 0.2, 0.3, 0.4])
 
     def curvature_analytical(φ):
         """analytical expression for curvature"""
         radius = (
             3.0
             * (
-                5.0 * (40.0 + 27.0 * epsilon ** 2.0)
+                5.0 * (40.0 + 27.0 * epsilon**2.0)
                 + epsilon
                 * (
                     40.0 * (4.0 * np.cos(2.0 * φ) + np.sin(φ))
                     + np.cos(φ) * (80.0 + 66.0 * epsilon + 240.0 * np.sin(φ))
                     - epsilon
                     * (
                         10.0 * np.cos(3.0 * φ)
@@ -156,15 +156,15 @@
                     * epsilon
                     * (
                         2.0 * np.cos(φ)
                         + 8.0 * np.cos(2.0 * φ)
                         + np.sin(φ)
                         + 6.0 * np.sin(2.0 * φ)
                     )
-                    + epsilon ** 2.0
+                    + epsilon**2.0
                     * (
                         345.0
                         + 165.0 * np.cos(φ)
                         - 5.0 * np.cos(3.0 * φ)
                         - 21.0 * np.cos(4.0 * φ)
                         + 30.0 * np.sin(φ)
                         - 10.0 * np.sin(3.0 * φ)
```

### Comparing `py-droplets-0.8.1/droplets/tests/test_emulsion.py` & `py-droplets-0.9.0/droplets/tests/test_emulsion.py`

 * *Files identical despite different names*

### Comparing `py-droplets-0.8.1/droplets/tests/test_examples.py` & `py-droplets-0.9.0/droplets/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `py-droplets-0.8.1/droplets/tests/test_image_analysis.py` & `py-droplets-0.9.0/droplets/tests/test_image_analysis.py`

 * *Files identical despite different names*

### Comparing `py-droplets-0.8.1/droplets/tests/test_trackers.py` & `py-droplets-0.9.0/droplets/tests/test_trackers.py`

 * *Files identical despite different names*

### Comparing `py-droplets-0.8.1/droplets/tools/spherical.py` & `py-droplets-0.9.0/droplets/tools/spherical.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         volume (float or :class:`~numpy.ndarray`): Volume of the sphere
         dim (int): Dimension of the space
 
     Returns:
         float or :class:`~numpy.ndarray`: Radius of the sphere
     """
     if dim == 1:
-        return volume / 2  # type: ignore
+        return volume / 2
     elif dim == 2:
         return np.sqrt(volume / π)  # type: ignore
     elif dim == 3:
         return (3 * volume / (4 * π)) ** (1 / 3)  # type: ignore
     else:
         raise NotImplementedError(f"Cannot calculate the radius in {dim} dimensions")
 
@@ -142,25 +142,25 @@
 
     Returns:
         function: A function that takes a radius and returns the volume
     """
     if dim == 1:
 
         def volume_from_radius(radius: TNumArr) -> TNumArr:
-            return 2 * radius  # type: ignore
+            return 2 * radius
 
     elif dim == 2:
 
         def volume_from_radius(radius: TNumArr) -> TNumArr:
-            return π * radius ** 2  # type: ignore
+            return π * radius**2
 
     elif dim == 3:
 
         def volume_from_radius(radius: TNumArr) -> TNumArr:
-            return 4 * π / 3 * radius ** 3  # type: ignore
+            return 4 * π / 3 * radius**3
 
     else:
         raise NotImplementedError(f"Cannot calculate the volume in {dim} dimensions")
     return jit(volume_from_radius)  # type: ignore
 
 
 def surface_from_radius(radius: TNumArr, dim: int) -> TNumArr:
@@ -175,17 +175,17 @@
     """
     if dim == 1:
         if isinstance(radius, np.ndarray):
             return np.broadcast_to(2, radius.shape)  # type: ignore
         else:
             return 2
     elif dim == 2:
-        return 2 * π * radius  # type: ignore
+        return 2 * π * radius
     elif dim == 3:
-        return 4 * π * radius ** 2  # type: ignore
+        return 4 * π * radius**2
     else:
         raise NotImplementedError(
             f"Cannot calculate the surface area in {dim} dimensions"
         )
 
 
 def radius_from_surface(surface: TNumArr, dim: int) -> TNumArr:
@@ -197,15 +197,15 @@
 
     Returns:
         float or :class:`~numpy.ndarray`: Radius of the sphere
     """
     if dim == 1:
         raise RuntimeError("Cannot calculate radius of 1-d sphere from surface")
     elif dim == 2:
-        return surface / (2 * π)  # type: ignore
+        return surface / (2 * π)
     elif dim == 3:
         return np.sqrt(surface / (4 * π))  # type: ignore
     else:
         raise NotImplementedError(f"Cannot calculate the radius in {dim} dimensions")
 
 
 def make_surface_from_radius_compiled(dim: int) -> Callable[[TNumArr], TNumArr]:
@@ -238,21 +238,21 @@
                 else:
                     return lambda radius: np.full(radius.shape, 2)  # type: ignore
 
     elif dim == 2:
 
         @jit
         def surface_from_radius(radius: TNumArr) -> TNumArr:
-            return 2 * π * radius  # type: ignore
+            return 2 * π * radius
 
     elif dim == 3:
 
         @jit
         def surface_from_radius(radius: TNumArr) -> TNumArr:
-            return 4 * π * radius ** 2  # type: ignore
+            return 4 * π * radius**2
 
     else:
         raise NotImplementedError(
             f"Cannot calculate the surface area in {dim} dimensions"
         )
     return surface_from_radius
```

### Comparing `py-droplets-0.8.1/droplets/tools/tests/test_spherical.py` & `py-droplets-0.9.0/droplets/tools/tests/test_spherical.py`

 * *Files identical despite different names*

### Comparing `py-droplets-0.8.1/droplets/trackers.py` & `py-droplets-0.9.0/droplets/trackers.py`

 * *Files identical despite different names*

### Comparing `py-droplets-0.8.1/examples/resources/emulsion.png` & `py-droplets-0.9.0/examples/resources/emulsion.png`

 * *Files identical despite different names*

### Comparing `py-droplets-0.8.1/examples/tutorial/Using the py-droplets package.ipynb` & `py-droplets-0.9.0/examples/tutorial/Using the py-droplets package.ipynb`

 * *Files identical despite different names*

### Comparing `py-droplets-0.8.1/py_droplets.egg-info/PKG-INFO` & `py-droplets-0.9.0/py_droplets.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: py-droplets
-Version: 0.8.1
+Version: 0.9.0
 Summary: Python package for describing and analyzing droplets in experiments and simulations
 Home-page: https://github.com/zwicker-group/py-droplets
 Author: David Zwicker
 Author-email: david.zwicker@ds.mpg.de
 License: MIT
-Download-URL: https://github.com/zwicker-group/py-droplets/archive/v0.8.1.tar.gz
+Download-URL: https://github.com/zwicker-group/py-droplets/archive/v0.9.0.tar.gz
 Keywords: emulsions,image-analysis
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: hdf
 License-File: LICENSE
 
 # py-droplets
```

### Comparing `py-droplets-0.8.1/py_droplets.egg-info/SOURCES.txt` & `py-droplets-0.9.0/py_droplets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-droplets-0.8.1/setup.py` & `py-droplets-0.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,10 +45,11 @@
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
     ],
 )
```

### Comparing `py-droplets-0.8.1/tests/mypy.ini` & `py-droplets-0.9.0/tests/mypy.ini`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 ignore_missing_imports = True
 
 [mypy-napari.*]
 ignore_missing_imports = True
 
 [mypy-numba.*]
 ignore_missing_imports = True
+ignore_errors = False
+follow_imports=skip
+follow_imports_for_stubs=True
 
 [mypy-numpy.*]
 ignore_missing_imports = True
 
 [mypy-pandas.*]
 ignore_missing_imports = True
```

### Comparing `py-droplets-0.8.1/tests/run_tests.py` & `py-droplets-0.9.0/tests/run_tests.py`

 * *Files identical despite different names*

