# Comparing `tmp/atlas-splitter-0.1.1.dev1.tar.gz` & `tmp/atlas-splitter-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/atlas-splitter-0.1.1.dev1.tar", last modified: Tue Mar  1 08:39:52 2022, max compression
+gzip compressed data, was "atlas-splitter-0.1.2.tar", last modified: Tue May 23 11:40:46 2023, max compression
```

## Comparing `atlas-splitter-0.1.1.dev1.tar` & `atlas-splitter-0.1.2.tar`

### file list

```diff
@@ -1,48 +1,61 @@
-drwxr-xr-x   0 gevaert  (141395) bbp      (10067)        0 2022-03-01 08:39:52.315769 atlas-splitter-0.1.1.dev1/
-drwxr-xr-x   0 gevaert  (141395) bbp      (10067)        0 2022-03-01 08:39:52.297392 atlas-splitter-0.1.1.dev1/.github/
-drwxr-xr-x   0 gevaert  (141395) bbp      (10067)        0 2022-03-01 08:39:52.302598 atlas-splitter-0.1.1.dev1/.github/workflows/
--rw-r--r--   0 gevaert  (141395) bbp      (10067)      618 2022-02-25 12:34:02.000000 atlas-splitter-0.1.1.dev1/.github/workflows/publish-sdist.yml
--rw-r--r--   0 gevaert  (141395) bbp      (10067)     1553 2022-02-25 12:37:16.000000 atlas-splitter-0.1.1.dev1/.github/workflows/run-tox.yml
--rw-r--r--   0 gevaert  (141395) bbp      (10067)      119 2021-12-17 16:46:52.000000 atlas-splitter-0.1.1.dev1/.gitignore
--rw-r--r--   0 gevaert  (141395) bbp      (10067)      200 2022-02-28 12:27:13.000000 atlas-splitter-0.1.1.dev1/AUTHORS.txt
--rw-r--r--   0 gevaert  (141395) bbp      (10067)      233 2021-12-17 16:46:52.000000 atlas-splitter-0.1.1.dev1/CHANGELOG.rst
--rw-r--r--   0 gevaert  (141395) bbp      (10067)    11358 2022-02-28 08:46:58.000000 atlas-splitter-0.1.1.dev1/LICENSE.txt
--rw-r--r--   0 gevaert  (141395) bbp      (10067)      765 2022-03-01 08:39:52.315292 atlas-splitter-0.1.1.dev1/PKG-INFO
--rw-r--r--   0 gevaert  (141395) bbp      (10067)     1232 2022-02-28 10:36:21.000000 atlas-splitter-0.1.1.dev1/README.rst
--rw-r--r--   0 gevaert  (141395) bbp      (10067)   160273 2022-02-25 12:14:58.000000 atlas-splitter-0.1.1.dev1/atlas-splitter.jpg
-drwxr-xr-x   0 gevaert  (141395) bbp      (10067)        0 2022-03-01 08:39:52.303628 atlas-splitter-0.1.1.dev1/atlas_splitter/
--rw-r--r--   0 gevaert  (141395) bbp      (10067)       79 2022-02-28 10:13:46.000000 atlas-splitter-0.1.1.dev1/atlas_splitter/__init__.py
-drwxr-xr-x   0 gevaert  (141395) bbp      (10067)        0 2022-03-01 08:39:52.307015 atlas-splitter-0.1.1.dev1/atlas_splitter/app/
--rw-r--r--   0 gevaert  (141395) bbp      (10067)       33 2021-12-17 16:46:52.000000 atlas-splitter-0.1.1.dev1/atlas_splitter/app/__init__.py
--rw-r--r--   0 gevaert  (141395) bbp      (10067)      376 2021-12-17 16:46:52.000000 atlas-splitter-0.1.1.dev1/atlas_splitter/app/cli.py
--rw-r--r--   0 gevaert  (141395) bbp      (10067)     2641 2022-01-27 08:32:50.000000 atlas-splitter-0.1.1.dev1/atlas_splitter/app/layer_splitter.py
--rw-r--r--   0 gevaert  (141395) bbp      (10067)      152 2021-12-17 16:46:52.000000 atlas-splitter-0.1.1.dev1/atlas_splitter/exceptions.py
-drwxr-xr-x   0 gevaert  (141395) bbp      (10067)        0 2022-03-01 08:39:52.307960 atlas-splitter-0.1.1.dev1/atlas_splitter/layer_splitter/
--rw-r--r--   0 gevaert  (141395) bbp      (10067)        0 2021-12-17 16:46:52.000000 atlas-splitter-0.1.1.dev1/atlas_splitter/layer_splitter/__init__.py
--rw-r--r--   0 gevaert  (141395) bbp      (10067)    15077 2022-02-24 10:05:57.000000 atlas-splitter-0.1.1.dev1/atlas_splitter/layer_splitter/isocortex_layer_23.py
-drwxr-xr-x   0 gevaert  (141395) bbp      (10067)        0 2022-03-01 08:39:52.305816 atlas-splitter-0.1.1.dev1/atlas_splitter.egg-info/
--rw-r--r--   0 gevaert  (141395) bbp      (10067)      765 2022-03-01 08:39:52.304140 atlas-splitter-0.1.1.dev1/atlas_splitter.egg-info/PKG-INFO
--rw-r--r--   0 gevaert  (141395) bbp      (10067)      918 2022-03-01 08:39:52.304494 atlas-splitter-0.1.1.dev1/atlas_splitter.egg-info/SOURCES.txt
--rw-r--r--   0 gevaert  (141395) bbp      (10067)        1 2022-03-01 08:39:52.304971 atlas-splitter-0.1.1.dev1/atlas_splitter.egg-info/dependency_links.txt
--rw-r--r--   0 gevaert  (141395) bbp      (10067)      108 2022-03-01 08:39:52.305424 atlas-splitter-0.1.1.dev1/atlas_splitter.egg-info/requires.txt
--rw-r--r--   0 gevaert  (141395) bbp      (10067)       21 2022-03-01 08:39:52.305933 atlas-splitter-0.1.1.dev1/atlas_splitter.egg-info/top_level.txt
-drwxr-xr-x   0 gevaert  (141395) bbp      (10067)        0 2022-03-01 08:39:52.308682 atlas-splitter-0.1.1.dev1/doc/
--rw-r--r--   0 gevaert  (141395) bbp      (10067)     1490 2021-12-17 16:46:52.000000 atlas-splitter-0.1.1.dev1/doc/Makefile
-drwxr-xr-x   0 gevaert  (141395) bbp      (10067)        0 2022-03-01 08:39:52.311215 atlas-splitter-0.1.1.dev1/doc/source/
--rw-r--r--   0 gevaert  (141395) bbp      (10067)       33 2021-12-17 16:46:52.000000 atlas-splitter-0.1.1.dev1/doc/source/changelog.rst
--rw-r--r--   0 gevaert  (141395) bbp      (10067)      260 2021-12-17 16:46:52.000000 atlas-splitter-0.1.1.dev1/doc/source/cli.rst
--rw-r--r--   0 gevaert  (141395) bbp      (10067)     6665 2022-02-28 12:10:43.000000 atlas-splitter-0.1.1.dev1/doc/source/conf.py
--rw-r--r--   0 gevaert  (141395) bbp      (10067)      220 2022-02-28 12:08:16.000000 atlas-splitter-0.1.1.dev1/doc/source/index.rst
--rw-r--r--   0 gevaert  (141395) bbp      (10067)      165 2021-12-17 16:46:52.000000 atlas-splitter-0.1.1.dev1/doc/source/layer_splitter.rst
--rw-r--r--   0 gevaert  (141395) bbp      (10067)       50 2022-02-28 12:08:09.000000 atlas-splitter-0.1.1.dev1/doc/source/readme.rst
--rw-r--r--   0 gevaert  (141395) bbp      (10067)       38 2022-03-01 08:39:52.315900 atlas-splitter-0.1.1.dev1/setup.cfg
--rw-r--r--   0 gevaert  (141395) bbp      (10067)     1207 2022-03-01 08:39:10.000000 atlas-splitter-0.1.1.dev1/setup.py
-drwxr-xr-x   0 gevaert  (141395) bbp      (10067)        0 2022-03-01 08:39:52.313528 atlas-splitter-0.1.1.dev1/tests/
--rw-r--r--   0 gevaert  (141395) bbp      (10067)   637735 2021-12-17 16:46:52.000000 atlas-splitter-0.1.1.dev1/tests/1.json
--rw-r--r--   0 gevaert  (141395) bbp      (10067)        0 2021-12-17 16:46:52.000000 atlas-splitter-0.1.1.dev1/tests/__init__.py
-drwxr-xr-x   0 gevaert  (141395) bbp      (10067)        0 2022-03-01 08:39:52.314757 atlas-splitter-0.1.1.dev1/tests/layer_splitter/
--rw-r--r--   0 gevaert  (141395) bbp      (10067)        0 2021-12-17 16:46:52.000000 atlas-splitter-0.1.1.dev1/tests/layer_splitter/__init__.py
--rw-r--r--   0 gevaert  (141395) bbp      (10067)     9200 2021-12-17 16:46:52.000000 atlas-splitter-0.1.1.dev1/tests/layer_splitter/test_isocortex_layer_23.py
--rw-r--r--   0 gevaert  (141395) bbp      (10067)     1777 2021-12-17 16:46:52.000000 atlas-splitter-0.1.1.dev1/tests/layer_splitter/utils.py
--rw-r--r--   0 gevaert  (141395) bbp      (10067)     1977 2021-12-17 16:46:52.000000 atlas-splitter-0.1.1.dev1/tests/test_app_layer_splitter.py
--rw-r--r--   0 gevaert  (141395) bbp      (10067)     1641 2022-02-28 12:14:25.000000 atlas-splitter-0.1.1.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:40:46.285686 atlas-splitter-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:40:46.277686 atlas-splitter-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:40:46.281686 atlas-splitter-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/.github/workflows/publish-sdist.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/.github/workflows/run-tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-23 11:40:46.285686 atlas-splitter-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   160273 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/atlas-splitter.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:40:46.281686 atlas-splitter-0.1.2/atlas_splitter/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/atlas_splitter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:40:46.281686 atlas-splitter-0.1.2/atlas_splitter/app/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/atlas_splitter/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/atlas_splitter/app/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:40:46.281686 atlas-splitter-0.1.2/atlas_splitter/barrel_splitter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/atlas_splitter/barrel_splitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/atlas_splitter/barrel_splitter/somatosensory_barrels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/atlas_splitter/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:40:46.281686 atlas-splitter-0.1.2/atlas_splitter/layer_splitter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/atlas_splitter/layer_splitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/atlas_splitter/layer_splitter/isocortex_layer_23.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/atlas_splitter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/atlas_splitter/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:40:46.281686 atlas-splitter-0.1.2/atlas_splitter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-23 11:40:46.000000 atlas-splitter-0.1.2/atlas_splitter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-23 11:40:46.000000 atlas-splitter-0.1.2/atlas_splitter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 11:40:46.000000 atlas-splitter-0.1.2/atlas_splitter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-23 11:40:46.000000 atlas-splitter-0.1.2/atlas_splitter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-23 11:40:46.000000 atlas-splitter-0.1.2/atlas_splitter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-23 11:40:46.000000 atlas-splitter-0.1.2/atlas_splitter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:40:46.281686 atlas-splitter-0.1.2/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:40:46.281686 atlas-splitter-0.1.2/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/doc/source/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/doc/source/layer_splitter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/doc/source/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 11:40:46.285686 atlas-splitter-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:40:46.285686 atlas-splitter-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)   637735 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/tests/1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/tests/2.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:40:46.285686 atlas-splitter-0.1.2/tests/barrel_splitter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/tests/barrel_splitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/tests/barrel_splitter/test_somatosensory_barrels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20969 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/tests/barrel_splitter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:40:46.285686 atlas-splitter-0.1.2/tests/layer_splitter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/tests/layer_splitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/tests/layer_splitter/test_isocortex_layer_23.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/tests/layer_splitter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/tests/test_app_barrel_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/tests/test_app_layer_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-23 11:40:40.000000 atlas-splitter-0.1.2/tox.ini
```

### Comparing `atlas-splitter-0.1.1.dev1/.github/workflows/publish-sdist.yml` & `atlas-splitter-0.1.2/.github/workflows/publish-sdist.yml`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,17 @@
       - 'v[0-9]+.[0-9]+.[0-9]+'
 
 jobs:
   build-n-publish:
     name: Build and publish on PyPI
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@master
+      - uses: actions/checkout@v3
       - name: Set up Python 3.8
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: 3.8
 
       - name: Build a source tarball
         run:
             python setup.py sdist
```

### Comparing `atlas-splitter-0.1.1.dev1/.github/workflows/run-tox.yml` & `atlas-splitter-0.1.2/.github/workflows/run-tox.yml`

 * *Files 19% similar despite different names*

```diff
@@ -7,20 +7,20 @@
         - master
 
 jobs:
   tests:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.7, 3.8, 3.9, 3.10]
+        python-version: ['3.7', '3.8', '3.9', '3.10']
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip setuptools
         pip install tox-gh-actions
@@ -29,17 +29,17 @@
       run: |
         tox -etests
 
   lint:
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python 3.8
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: 3.8
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip setuptools
         pip install tox
@@ -48,17 +48,17 @@
       run: |
         tox -elint
 
   coverage:
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python 3.8
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: 3.8
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip setuptools
         pip install tox
```

### Comparing `atlas-splitter-0.1.1.dev1/LICENSE.txt` & `atlas-splitter-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `atlas-splitter-0.1.1.dev1/PKG-INFO` & `atlas-splitter-0.1.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 Metadata-Version: 2.1
 Name: atlas-splitter
-Version: 0.1.1.dev1
+Version: 0.1.2
 Summary: CLI to split atlas regions and modify annotations accordingly
 Home-page: https://github.com/BlueBrain/atlas-splitter
 Author: Blue Brain Project, EPFL
 License: Apache-2
 Download-URL: https://github.com/BlueBrain/atlas-splitter
+Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7.0
 Provides-Extra: tests
-License-File: LICENSE.txt
-License-File: AUTHORS.txt
-
-UNKNOWN
-
```

### Comparing `atlas-splitter-0.1.1.dev1/atlas-splitter.jpg` & `atlas-splitter-0.1.2/atlas-splitter.jpg`

 * *Files identical despite different names*

### Comparing `atlas-splitter-0.1.1.dev1/atlas_splitter/app/layer_splitter.py` & `atlas-splitter-0.1.2/atlas_splitter/app/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,94 @@
-"""Refine annotations by splitting layers of a brain region"""
+"""The atlas-splitter command line launcher"""
+
 import json
 import logging
 
 import click
-import voxcell  # type: ignore
+import pandas as pd
 from atlas_commons.app_utils import (
     EXISTING_FILE_PATH,
     common_atlas_options,
     log_args,
     set_verbose,
     verbose_option,
 )
+from voxcell import VoxelData
 
+from atlas_splitter.barrel_splitter import somatosensory_barrels
 from atlas_splitter.layer_splitter import isocortex_layer_23
+from atlas_splitter.version import VERSION as __version__
 
 L = logging.getLogger(__name__)
 logging.basicConfig(level=logging.INFO)
 
 
-@click.group()
-def app():
-    """Run the splitter CLI"""
+class NaturalOrderGroup(click.Group):
+    """Click group preserving the order of commands."""
+
+    def list_commands(self, ctx: click.Context):
+        """Return the list of possible commands."""
+        return list(self.commands)
+
+
+@click.group(cls=NaturalOrderGroup)
+@click.version_option(__version__)
+def cli():
+    """The CLI entry point."""
+
+
+@cli.command()
+@verbose_option
+@common_atlas_options
+@click.option(
+    "--barrels-path",
+    type=EXISTING_FILE_PATH,
+    required=True,
+    help=("Path to the DataFrame with barrel positions and labels."),
+)
+@click.option("--output-hierarchy-path", required=True, help="Path of the json file to write")
+@click.option("--output-annotation-path", required=True, help="Path of the nrrd file to write")
+@log_args(L)
+def split_barrel_columns(  # pylint: disable=too-many-arguments
+    verbose,
+    annotation_path,
+    hierarchy_path,
+    barrels_path,
+    output_hierarchy_path,
+    output_annotation_path,
+):
+    """Introduce the barrel columns to SSp-bfd (primary somatosensory barrel cortex)
+    in the mouse annotations in place. Positions of the voxels need to be specified by a DataFrame.
+
+    The `hierarchy` dict and the `annotation` are modified in-place.
+    All of the barrels present in the DF are introduced based on their
+    x, y, z voxel positions.
+
+    New children are added to the layer 4 of Somatosensory barrel cortex
+    in Isocortex.
+    """
+    set_verbose(L, verbose)
+
+    L.info("Loading files ...")
+    barrel_positions = pd.read_feather(barrels_path)
+    annotation = VoxelData.load_nrrd(annotation_path)
+
+    with open(hierarchy_path, "r", encoding="utf-8") as h_file:
+        hierarchy = json.load(h_file)
+
+    L.info("Introduce the barrel columns to SSp-bfd...")
+    somatosensory_barrels.split_barrels(hierarchy, annotation, barrel_positions)
+
+    L.info("Saving modified hierarchy and annotation files ...")
+    with open(output_hierarchy_path, "w", encoding="utf-8") as out:
+        json.dump(hierarchy, out, indent=1, separators=(",", ": "))
+    annotation.save_nrrd(output_annotation_path)
 
 
-@app.command()
+@cli.command()
 @verbose_option
 @common_atlas_options
 @click.option(
     "--direction-vectors-path",
     type=EXISTING_FILE_PATH,
     required=True,
     help=(
@@ -56,18 +117,18 @@
 
     Note: The modification of the hierarchy file is independent of the input annotated volume.
     The direction vectors should not be (NaN, NaN, NaN) on any voxel of the layer 2/3 volume.
     """
     set_verbose(L, verbose)
 
     L.info("Loading files ...")
-    annotation = voxcell.VoxelData.load_nrrd(annotation_path)
+    annotation = VoxelData.load_nrrd(annotation_path)
     with open(hierarchy_path, "r", encoding="utf-8") as h_file:
         hierarchy = json.load(h_file)
-    direction_vectors = voxcell.VoxelData.load_nrrd(direction_vectors_path)
+    direction_vectors = VoxelData.load_nrrd(direction_vectors_path)
 
     # Splits and updates in place hierarchy and annotations
     L.info("Splitting layer 2/3 in layer 2 and layer 3 ...")
     isocortex_layer_23.split(hierarchy, annotation, direction_vectors.raw)
 
     L.info("Saving modified hierarchy and annotation files ...")
     with open(output_hierarchy_path, "w", encoding="utf-8") as out:
```

### Comparing `atlas-splitter-0.1.1.dev1/atlas_splitter/layer_splitter/isocortex_layer_23.py` & `atlas-splitter-0.1.2/atlas_splitter/layer_splitter/isocortex_layer_23.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,105 +19,35 @@
 decide whether a voxel belongs either to layer 2 or layer 3.
 """
 from __future__ import annotations
 
 import copy
 import logging
 from collections import defaultdict
-from itertools import count
 from typing import Any, Dict, Iterator, Set
 
 import numpy as np
 from atlas_commons.typing import BoolArray, FloatArray, NDArray
 from cgal_pybind import slice_volume
 from voxcell import RegionMap, VoxelData
 
 from atlas_splitter.exceptions import AtlasSplitterError
+from atlas_splitter.utils import _assert_is_leaf_node, create_id_generator, get_isocortex_hierarchy
 
 L = logging.getLogger(__name__)
 
 # The following constants are documented in Section 5.1.1.4 of the release report of the
 # Neocortex Tissue Reconstruction.
 DEFAULT_L2_THICKNESS = 95.10
 DEFAULT_L3_THICKNESS = 225.3199
 DEFAULT_RATIO = DEFAULT_L2_THICKNESS / (DEFAULT_L2_THICKNESS + DEFAULT_L3_THICKNESS)
 
 HierarchyDict = Dict[str, Any]
 
 
-def get_isocortex_hierarchy(allen_hierachy: HierarchyDict):
-    """
-    Extract the hierarchy dict of the iscortex from AIBS hierarchy dict.
-    Args:
-        allen_hierarchy: AIBS hierarchy dict instantiated from
-            http://api.brain-map.org/api/v2/structure_graph_download/1.json.
-    """
-    error_msg = "Wrong input. The AIBS 1.json file is expected."
-    if "msg" not in allen_hierachy:
-        raise AtlasSplitterError(error_msg)
-
-    hierarchy = allen_hierachy["msg"][0]
-    try:
-        while hierarchy["acronym"] != "Isocortex":
-            hierarchy = hierarchy["children"][0]
-    except KeyError as error:
-        raise AtlasSplitterError(error_msg) from error
-
-    return hierarchy
-
-
-def create_id_generator(region_map: RegionMap) -> Iterator[int]:
-    """Create an identifiers generator.
-
-    The generator produces an identifier which is different from all
-    the previous ones and from the identifiers in use in `self.region_map`.
-
-    Args:
-        region_map: map to navigate the brain region hierarchy.
-
-    Return:
-        iterator providing the next id.
-    """
-    last = max(region_map.find("root", attr="acronym", with_descendants=True))
-    return count(start=last + 1)
-
-
-def _assert_is_leaf_node(node) -> None:
-    """
-    Raises an AtalasSplitterError if `node` is not a leaf node.
-
-    Args:
-        node: node of the hierarchy tree. Dict of the form
-        {
-            "id": 195,
-                   "atlas_id": 1014,
-                   "ontology_id": 1,
-                   "acronym": "PL2",
-                   "name": "Prelimbic area, layer 2",
-                   "color_hex_triplet": "2FA850",
-                   "graph_order": 240,
-                   "st_level": 11,
-                   "hemisphere_id": 3,
-                   "parent_structure_id": 972,
-                   "children": []
-                  },
-
-        }
-    Raises:
-        AtlasSplitterError if `node` is a not a leaf `node`.
-    """
-    if "children" not in node:
-        raise AtlasSplitterError(f'Missing "children" key for region {node["name"]}.')
-    if node["children"] != []:
-        raise AtlasSplitterError(
-            f'Region {node["name"]} has an unexpected "children" value: '
-            f'{node["children"]}. Expected: [].'
-        )
-
-
 def edit_hierarchy(
     hierarchy: HierarchyDict,
     new_layer_ids: Dict[int, Dict[str, int]],
     ids_to_reuse: Dict[int, Dict[str, int]],
     region_map: RegionMap,
     id_generator: Iterator[int],
 ) -> None:
@@ -335,15 +265,18 @@
     if np.any(np.isnan(direction_vectors[volume])):
         raise AtlasSplitterError(
             "The 3D region to split, that is layer 2/3, contains [NaN, NaN, NaN] "
             "direction vectors. Consider interpolating these vectors by valid ones. "
             "See, e.g., ``atlas-direction-vectors`` documentation and"
             "``atlas-direction-vectors interpolation --help`` in particular."
         )
-    L.info("Splitting the layer 2/3 volume using a thickness ratio of %f ...", thickness_ratio)
+    L.info(
+        "Splitting the layer 2/3 volume using a thickness ratio of %f ...",
+        thickness_ratio,
+    )
     # The voxels labeled with 1 (resp. 2) are the voxels whose cortical depth is at most
     # (resp. greater than) `thickness_ratio` times the full thickness of layer 2/3.
     # Note: direction vectors flow from the deepest layer to the shallowest layer.
     splitting = slice_volume(
         volume=volume,
         # Default offset can be of type float if voxcell<=3.0.1
         offset=np.array(annotation.offset, dtype=np.float32),
```

### Comparing `atlas-splitter-0.1.1.dev1/atlas_splitter.egg-info/PKG-INFO` & `atlas-splitter-0.1.2/atlas_splitter.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 Metadata-Version: 2.1
 Name: atlas-splitter
-Version: 0.1.1.dev1
+Version: 0.1.2
 Summary: CLI to split atlas regions and modify annotations accordingly
 Home-page: https://github.com/BlueBrain/atlas-splitter
 Author: Blue Brain Project, EPFL
 License: Apache-2
 Download-URL: https://github.com/BlueBrain/atlas-splitter
+Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7.0
 Provides-Extra: tests
-License-File: LICENSE.txt
-License-File: AUTHORS.txt
-
-UNKNOWN
-
```

### Comparing `atlas-splitter-0.1.1.dev1/atlas_splitter.egg-info/SOURCES.txt` & `atlas-splitter-0.1.2/atlas_splitter.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,46 @@
 .gitignore
 AUTHORS.txt
 CHANGELOG.rst
+CONTRIBUTING.rst
 LICENSE.txt
 README.rst
 atlas-splitter.jpg
 setup.py
 tox.ini
 .github/workflows/publish-sdist.yml
 .github/workflows/run-tox.yml
 atlas_splitter/__init__.py
 atlas_splitter/exceptions.py
+atlas_splitter/utils.py
+atlas_splitter/version.py
 atlas_splitter.egg-info/PKG-INFO
 atlas_splitter.egg-info/SOURCES.txt
 atlas_splitter.egg-info/dependency_links.txt
+atlas_splitter.egg-info/entry_points.txt
 atlas_splitter.egg-info/requires.txt
 atlas_splitter.egg-info/top_level.txt
 atlas_splitter/app/__init__.py
 atlas_splitter/app/cli.py
-atlas_splitter/app/layer_splitter.py
+atlas_splitter/barrel_splitter/__init__.py
+atlas_splitter/barrel_splitter/somatosensory_barrels.py
 atlas_splitter/layer_splitter/__init__.py
 atlas_splitter/layer_splitter/isocortex_layer_23.py
 doc/Makefile
 doc/source/changelog.rst
 doc/source/cli.rst
 doc/source/conf.py
 doc/source/index.rst
 doc/source/layer_splitter.rst
 doc/source/readme.rst
 tests/1.json
+tests/2.json
 tests/__init__.py
+tests/test_app_barrel_splitter.py
 tests/test_app_layer_splitter.py
+tests/test_utils.py
+tests/barrel_splitter/__init__.py
+tests/barrel_splitter/test_somatosensory_barrels.py
+tests/barrel_splitter/utils.py
 tests/layer_splitter/__init__.py
 tests/layer_splitter/test_isocortex_layer_23.py
 tests/layer_splitter/utils.py
```

### Comparing `atlas-splitter-0.1.1.dev1/doc/Makefile` & `atlas-splitter-0.1.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `atlas-splitter-0.1.1.dev1/doc/source/conf.py` & `atlas-splitter-0.1.2/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `atlas-splitter-0.1.1.dev1/setup.py` & `atlas-splitter-0.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,38 +4,38 @@
 
 setup(
     name="atlas-splitter",
     author="Blue Brain Project, EPFL",
     description="CLI to split atlas regions and modify annotations accordingly",
     url="https://github.com/BlueBrain/atlas-splitter",
     download_url="https://github.com/BlueBrain/atlas-splitter",
-    license='Apache-2',
+    license="Apache-2",
     python_requires=">=3.7.0",
     install_requires=[
-        "atlas-commons>=0.1.3.dev0",
+        "atlas-commons>=0.1.4",
         "click>=7.0",
         "cgal-pybind>=0.1.3",
         "numpy>=1.15.0",
         "voxcell>=3.0.0",
+        "pyarrow>=8.0.0",
     ],
     extras_require={
         "tests": [
             "pytest>=4.4.0",
         ],
     },
     packages=find_packages(),
     include_package_data=True,
-
+    entry_points={"console_scripts": ["atlas-splitter=atlas_splitter.app.cli:cli"]},
     use_scm_version={
         "local_scheme": "no-local-version",
-        },
+    },
     setup_requires=[
-        'setuptools_scm',
+        "setuptools_scm",
     ],
-
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

### Comparing `atlas-splitter-0.1.1.dev1/tests/1.json` & `atlas-splitter-0.1.2/tests/1.json`

 * *Files identical despite different names*

### Comparing `atlas-splitter-0.1.1.dev1/tests/layer_splitter/test_isocortex_layer_23.py` & `atlas-splitter-0.1.2/tests/layer_splitter/test_isocortex_layer_23.py`

 * *Files 14% similar despite different names*

```diff
@@ -71,70 +71,14 @@
                 ],
                 "parent_structure_id": 315,
             }
         ],
     }
 
 
-def test_get_isocortex_hierarchy():
-    with pytest.raises(AtlasSplitterError):
-        allen_hierarchy = {
-            "root": [
-                {
-                    "id": 998,
-                    "children": [
-                        {
-                            "id": 0,
-                            "acronym": "grey matter",
-                            "children": [{"id": 1, "acronym": "End of the world"}],
-                        }
-                    ],
-                }
-            ]
-        }
-        tested.get_isocortex_hierarchy(allen_hierarchy)
-    with pytest.raises(AtlasSplitterError):
-        allen_hierarchy = {
-            "msg": [
-                {
-                    "id": 998,
-                    "children": [
-                        {
-                            "id": 0,
-                            "acronym": "root",
-                            "children": [{"id": 1, "acronym": "End of the world"}],
-                        }
-                    ],
-                }
-            ]
-        }
-        tested.get_isocortex_hierarchy(allen_hierarchy)
-
-
-def test_get_isocortex_hierarchy_exception():
-    with open(str(Path(TEST_PATH, "1.json", encoding="utf-8"))) as h_file:
-        allen_hierarchy = json.load(h_file)
-        isocortex_hierarchy = tested.get_isocortex_hierarchy(allen_hierarchy)
-        assert isocortex_hierarchy["acronym"] == "Isocortex"
-
-
-def test_create_id_generator():
-    region_map = RegionMap.load_json(str(Path(TEST_PATH, "1.json", encoding="utf-8")))
-    id_generator = tested.create_id_generator(region_map)
-
-    npt.assert_array_equal(
-        (
-            next(id_generator),
-            next(id_generator),
-            next(id_generator),
-        ),
-        (614454278, 614454279, 614454280),
-    )
-
-
 def test_edit_hierarchy():
     isocortex_hierarchy = get_isocortex_hierarchy_excerpt()
     expected_hierarchy = get_isocortex_hierarchy_excerpt()
     # Removes "Somatomotor areas, Layer 2"
     # The corresponding identifier should be reused
     del expected_hierarchy["children"][0]["children"][1]
 
@@ -242,8 +186,13 @@
     with open(str(Path(TEST_PATH, "1.json")), encoding="utf-8") as h_file:
         allen_hierarchy = json.load(h_file)
 
     data = get_splitting_input_data()
     data["direction_vectors"][1, 25, 25] = [np.nan] * 3
 
     with pytest.raises(AtlasSplitterError, match=".*\\[NaN, NaN, NaN\\] direction vector.*"):
-        tested.split(allen_hierarchy, data["annotation"], data["direction_vectors"], data["ratio"])
+        tested.split(
+            allen_hierarchy,
+            data["annotation"],
+            data["direction_vectors"],
+            data["ratio"],
+        )
```

### Comparing `atlas-splitter-0.1.1.dev1/tests/layer_splitter/utils.py` & `atlas-splitter-0.1.2/tests/layer_splitter/utils.py`

 * *Files identical despite different names*

### Comparing `atlas-splitter-0.1.1.dev1/tests/test_app_layer_splitter.py` & `atlas-splitter-0.1.2/tests/test_app_layer_splitter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """test app.layer_splitter"""
 from pathlib import Path
 
 from atlas_commons.app_utils import assert_properties
 from click.testing import CliRunner
 from voxcell import RegionMap, VoxelData  # type: ignore
 
-import atlas_splitter.app.layer_splitter as tested
+import atlas_splitter.app.cli as tested
 from tests.layer_splitter.utils import LAYER_23_IDS, get_splitting_input_data
 
 TEST_PATH = Path(__file__).parent
 
 
 def _get_result(runner):
     return runner.invoke(
-        tested.app,
+        tested.cli,
         [
             "split-isocortex-layer-23",
             "--annotation-path",
             "annotation.nrrd",
             "--hierarchy-path",
             str(Path(TEST_PATH, "1.json")),
             "--direction-vectors-path",
```

### Comparing `atlas-splitter-0.1.1.dev1/tox.ini` & `atlas-splitter-0.1.2/tox.ini`

 * *Files 19% similar despite different names*

```diff
@@ -2,19 +2,16 @@
 name = atlas_splitter
 black_version = 22.0
 
 [tox]
 envlist =
     check-version
     lint
-    py38
     docs
-
-indexserver =
-    default = https://bbpteam.epfl.ch/repository/devpi/simple
+    tests
 
 [testenv]
 extras = tests
 passenv = PYTHONPATH
 commands = pytest tests
 
 [testenv:lint]
```

