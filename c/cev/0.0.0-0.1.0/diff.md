# Comparing `tmp/cev-0.0.0.tar.gz` & `tmp/cev-0.1.0.tar.gz`

## Comparing `cev-0.0.0.tar` & `cev-0.1.0.tar`

### file list

```diff
@@ -1,47 +1,30 @@
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 cev-0.0.0/.editorconfig
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cev-0.0.0/.gitattributes
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 cev-0.0.0/Snakefile
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 cev-0.0.0/environment.yml
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 cev-0.0.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cev-0.0.0/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 cev-0.0.0/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 cev-0.0.0/.pytest_cache/README.md
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cev-0.0.0/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 cev-0.0.0/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 cev-0.0.0/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 cev-0.0.0/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 cev-0.0.0/.ruff_cache/content/22fc9873323ca5fb
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 cev-0.0.0/.ruff_cache/content/5fca4e6fae68281d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 cev-0.0.0/.ruff_cache/content/6ff3cc7bd6f76b7f
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 cev-0.0.0/.ruff_cache/content/7266c22be038003b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 cev-0.0.0/.ruff_cache/content/7afd9612cc372dfb
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 cev-0.0.0/.ruff_cache/content/84e2d55fa4e07966
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 cev-0.0.0/.ruff_cache/content/afbeedc9f84810d
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 cev-0.0.0/.ruff_cache/content/b096359e551b34e5
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 cev-0.0.0/.ruff_cache/content/b17caf624ac3ccb
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 cev-0.0.0/.ruff_cache/content/bca656cf5da14b26
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 cev-0.0.0/.ruff_cache/content/cf0d0ef95eec8610
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 cev-0.0.0/.ruff_cache/content/d9b05658f593cf2b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 cev-0.0.0/.ruff_cache/content/e24b578ba96cdbd6
--rw-r--r--   0        0        0   423026 2020-02-02 00:00:00.000000 cev-0.0.0/notebooks/neighborhood-analysis.ipynb
--rw-r--r--   0        0        0     8001 2020-02-02 00:00:00.000000 cev-0.0.0/notebooks/prototype.ipynb
--rw-r--r--   0        0        0   535212 2020-02-02 00:00:00.000000 cev-0.0.0/notebooks/test_cases/confusion.ipynb
--rw-r--r--   0        0        0  6642577 2020-02-02 00:00:00.000000 cev-0.0.0/notebooks/test_cases/neighborhood.ipynb
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 cev-0.0.0/cev/__init__.py
--rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 cev-0.0.0/cev/_widget_utils.py
--rw-r--r--   0        0        0    13559 2020-02-02 00:00:00.000000 cev-0.0.0/cev/logo.py
--rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 cev-0.0.0/cev/metrics.py
--rw-r--r--   0        0        0     4724 2020-02-02 00:00:00.000000 cev-0.0.0/cev/transformation.py
--rw-r--r--   0        0        0    18612 2020-02-02 00:00:00.000000 cev-0.0.0/cev/widgets.py
--rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 cev-0.0.0/cev/static/AnnotationLogo.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cev-0.0.0/cev/test_cases/__init__.py
--rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 cev-0.0.0/cev/test_cases/confusion.py
--rw-r--r--   0        0        0     7818 2020-02-02 00:00:00.000000 cev-0.0.0/cev/test_cases/metrics.py
--rw-r--r--   0        0        0     7130 2020-02-02 00:00:00.000000 cev-0.0.0/cev/test_cases/neighborhood.py
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 cev-0.0.0/cev/test_cases/utils.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 cev-0.0.0/tests/test_cev.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 cev-0.0.0/.gitignore
--rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 cev-0.0.0/LICENSE
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 cev-0.0.0/README.md
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 cev-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 cev-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 cev-0.1.0/.editorconfig
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cev-0.1.0/.gitattributes
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 cev-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 cev-0.1.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     9760 2020-02-02 00:00:00.000000 cev-0.1.0/notebooks/abundance-analysis.ipynb
+-rw-r--r--   0        0        0     9044 2020-02-02 00:00:00.000000 cev-0.1.0/notebooks/getting-started.ipynb
+-rw-r--r--   0        0        0     9042 2020-02-02 00:00:00.000000 cev-0.1.0/notebooks/lui-2021.ipynb
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 cev-0.1.0/cev/__init__.py
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 cev-0.1.0/cev/_compare.py
+-rw-r--r--   0        0        0     5962 2020-02-02 00:00:00.000000 cev-0.1.0/cev/_compare_metric_dropdown.py
+-rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 cev-0.1.0/cev/_compare_selection_type_dropdown.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 cev-0.1.0/cev/_compare_zoom_toggle.py
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 cev-0.1.0/cev/_embedding.py
+-rw-r--r--   0        0        0     7069 2020-02-02 00:00:00.000000 cev-0.1.0/cev/_embedding_comparison_widget.py
+-rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 cev-0.1.0/cev/_embedding_widget.py
+-rw-r--r--   0        0        0     8661 2020-02-02 00:00:00.000000 cev-0.1.0/cev/_widget_utils.py
+-rw-r--r--   0        0        0     9051 2020-02-02 00:00:00.000000 cev-0.1.0/cev/metrics.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 cev-0.1.0/cev/widgets.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 cev-0.1.0/cev/components/__init__.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 cev-0.1.0/cev/components/_html_widget.py
+-rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 cev-0.1.0/cev/components/_marker_composition_logo.py
+-rw-r--r--   0        0        0     7725 2020-02-02 00:00:00.000000 cev-0.1.0/cev/components/_marker_selection_indicator.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 cev-0.1.0/cev/components/_width_optimizer.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 cev-0.1.0/tests/test_cev.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 cev-0.1.0/tests/test_widget_utils.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 cev-0.1.0/.gitignore
+-rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 cev-0.1.0/LICENSE
+-rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 cev-0.1.0/README.md
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 cev-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 cev-0.1.0/PKG-INFO
```

### Comparing `cev-0.0.0/.github/workflows/ci.yml` & `cev-0.1.0/.github/workflows/ci.yml`

 * *Files 22% similar despite different names*

```diff
@@ -2,62 +2,50 @@
 
 on:
   push:
     branches:
       - main
     tags:
       - "v*"
-  pull_request: {}
+  pull_request:
+  workflow_dispatch:
 
 jobs:
 
   Lint:
     runs-on: ubuntu-latest
     steps:
       - name: Checkout
         uses: actions/checkout@v3
 
-      - uses: actions/setup-python@v4
-        with:
-          python-version: "3.x"
-          cache: "pip"
-          cache-dependency-path: "**/pyproject.toml"
-
-      - name: Install dependencies
-        run: |
-          python -m pip install --upgrade pip
-          pip install black[jupyter] ruff
-
-      - name: Check formatting and linting
-        run: black --check . && ruff .
+      # this could be replaced with pre-commit.ci
+      - run: pipx run pre-commit run --all-files
 
   Test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.9", "3.10"]
+        python-version: ["3.8", "3.9", "3.10", "3.11"]
 
     steps:
       - name: Checkout
         uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
-          cache: "pip"
-          cache-dependency-path: "**/pyproject.toml"
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -e .[test,dev]
 
       - name: Run tests
-        run: pytest ./tests --color=yes
+        run: pytest --color=yes
 
   Release:
     if: startsWith(github.ref, 'refs/tags/')
     needs: [Lint, Test]
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
```

### Comparing `cev-0.0.0/LICENSE` & `cev-0.1.0/LICENSE`

 * *Files identical despite different names*

