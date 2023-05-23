# Comparing `tmp/numpyro-ext-0.0.1.tar.gz` & `tmp/numpyro-ext-0.0.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numpyro-ext-0.0.1.tar", last modified: Mon Aug  1 19:05:42 2022, max compression
+gzip compressed data, was "numpyro-ext-0.0.2rc1.tar", last modified: Mon May 22 23:57:53 2023, max compression
```

## Comparing `numpyro-ext-0.0.1.tar` & `numpyro-ext-0.0.2rc1.tar`

### file list

```diff
@@ -1,33 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 19:05:42.195991 numpyro-ext-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)      867 2022-08-01 19:05:30.000000 numpyro-ext-0.0.1/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 19:05:42.195991 numpyro-ext-0.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-08-01 19:05:30.000000 numpyro-ext-0.0.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 19:05:42.195991 numpyro-ext-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2246 2022-08-01 19:05:30.000000 numpyro-ext-0.0.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-08-01 19:05:30.000000 numpyro-ext-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      785 2022-08-01 19:05:30.000000 numpyro-ext-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     5468 2022-08-01 19:05:30.000000 numpyro-ext-0.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1370 2022-08-01 19:05:30.000000 numpyro-ext-0.0.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-08-01 19:05:30.000000 numpyro-ext-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    13700 2022-08-01 19:05:42.195991 numpyro-ext-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-08-01 19:05:30.000000 numpyro-ext-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-08-01 19:05:30.000000 numpyro-ext-0.0.1/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (121)     1402 2022-08-01 19:05:30.000000 numpyro-ext-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-08-01 19:05:30.000000 numpyro-ext-0.0.1/readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-01 19:05:42.195991 numpyro-ext-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-01 19:05:30.000000 numpyro-ext-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 19:05:42.195991 numpyro-ext-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 19:05:42.195991 numpyro-ext-0.0.1/src/numpyro_ext/
--rw-r--r--   0 runner    (1001) docker     (121)      643 2022-08-01 19:05:30.000000 numpyro-ext-0.0.1/src/numpyro_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17387 2022-08-01 19:05:30.000000 numpyro-ext-0.0.1/src/numpyro_ext/distributions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1877 2022-08-01 19:05:30.000000 numpyro-ext-0.0.1/src/numpyro_ext/info.py
--rw-r--r--   0 runner    (1001) docker     (121)     4209 2022-08-01 19:05:30.000000 numpyro-ext-0.0.1/src/numpyro_ext/optim.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-08-01 19:05:42.000000 numpyro-ext-0.0.1/src/numpyro_ext/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 19:05:42.195991 numpyro-ext-0.0.1/src/numpyro_ext.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13700 2022-08-01 19:05:42.000000 numpyro-ext-0.0.1/src/numpyro_ext.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      567 2022-08-01 19:05:42.000000 numpyro-ext-0.0.1/src/numpyro_ext.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-01 19:05:42.000000 numpyro-ext-0.0.1/src/numpyro_ext.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-08-01 19:05:42.000000 numpyro-ext-0.0.1/src/numpyro_ext.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-08-01 19:05:42.000000 numpyro-ext-0.0.1/src/numpyro_ext.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 19:05:42.195991 numpyro-ext-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-08-01 19:05:30.000000 numpyro-ext-0.0.1/tests/test_numpyro_ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:57:53.994176 numpyro-ext-0.0.2rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-22 23:57:42.000000 numpyro-ext-0.0.2rc1/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:57:53.990176 numpyro-ext-0.0.2rc1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-22 23:57:42.000000 numpyro-ext-0.0.2rc1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:57:53.990176 numpyro-ext-0.0.2rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-22 23:57:42.000000 numpyro-ext-0.0.2rc1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-22 23:57:42.000000 numpyro-ext-0.0.2rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-22 23:57:42.000000 numpyro-ext-0.0.2rc1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-05-22 23:57:42.000000 numpyro-ext-0.0.2rc1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-22 23:57:42.000000 numpyro-ext-0.0.2rc1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-22 23:57:42.000000 numpyro-ext-0.0.2rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-05-22 23:57:53.994176 numpyro-ext-0.0.2rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-05-22 23:57:42.000000 numpyro-ext-0.0.2rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-22 23:57:42.000000 numpyro-ext-0.0.2rc1/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-22 23:57:42.000000 numpyro-ext-0.0.2rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-22 23:57:42.000000 numpyro-ext-0.0.2rc1/readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 23:57:53.994176 numpyro-ext-0.0.2rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-22 23:57:42.000000 numpyro-ext-0.0.2rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:57:53.990176 numpyro-ext-0.0.2rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:57:53.990176 numpyro-ext-0.0.2rc1/src/numpyro_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-22 23:57:42.000000 numpyro-ext-0.0.2rc1/src/numpyro_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17603 2023-05-22 23:57:42.000000 numpyro-ext-0.0.2rc1/src/numpyro_ext/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-22 23:57:42.000000 numpyro-ext-0.0.2rc1/src/numpyro_ext/infer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-05-22 23:57:42.000000 numpyro-ext-0.0.2rc1/src/numpyro_ext/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-05-22 23:57:42.000000 numpyro-ext-0.0.2rc1/src/numpyro_ext/linear_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-05-22 23:57:42.000000 numpyro-ext-0.0.2rc1/src/numpyro_ext/optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-22 23:57:53.000000 numpyro-ext-0.0.2rc1/src/numpyro_ext/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:57:53.990176 numpyro-ext-0.0.2rc1/src/numpyro_ext.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-05-22 23:57:53.000000 numpyro-ext-0.0.2rc1/src/numpyro_ext.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-22 23:57:53.000000 numpyro-ext-0.0.2rc1/src/numpyro_ext.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 23:57:53.000000 numpyro-ext-0.0.2rc1/src/numpyro_ext.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-22 23:57:53.000000 numpyro-ext-0.0.2rc1/src/numpyro_ext.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 23:57:53.000000 numpyro-ext-0.0.2rc1/src/numpyro_ext.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:57:53.990176 numpyro-ext-0.0.2rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-05-22 23:57:42.000000 numpyro-ext-0.0.2rc1/tests/test_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-22 23:57:42.000000 numpyro-ext-0.0.2rc1/tests/test_infer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-05-22 23:57:42.000000 numpyro-ext-0.0.2rc1/tests/test_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-22 23:57:42.000000 numpyro-ext-0.0.2rc1/tests/test_linear_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-22 23:57:42.000000 numpyro-ext-0.0.2rc1/tests/test_optim.py
```

### Comparing `numpyro-ext-0.0.1/.copier-answers.yml` & `numpyro-ext-0.0.2rc1/.copier-answers.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-_commit: v0.0.5
+_commit: v0.0.14
 _src_path: gh:dfm/copier-python
 author_email: foreman.mackey@gmail.com
 author_fullname: Dan Foreman-Mackey
 author_username: dfm
 code_of_conduct_email: foreman.mackey@gmail.com
 copyright_holder: Simons Foundation, Inc.
 copyright_license: Apache
```

### Comparing `numpyro-ext-0.0.1/.github/workflows/tests.yml` & `numpyro-ext-0.0.2rc1/.github/workflows/tests.yml`

 * *Files 16% similar despite different names*

```diff
@@ -6,76 +6,105 @@
       - main
     tags:
       - "*"
   pull_request:
   workflow_dispatch:
     inputs:
       prerelease:
-        description: 'Run a pre-release, testing the build'
+        description: "Run a pre-release, testing the build"
         required: false
         type: boolean
         default: false
 
 jobs:
   tests:
     runs-on: ${{ matrix.os }}
     strategy:
+      fail-fast: false
       matrix:
         os: ["ubuntu-latest"]
-        python-version: ["3.7", "3.8", "3.9", "3.10"]
+        python-version: ["3.8", "3.9", "3.10"]
         nox-session: ["tests"]
         include:
           - os: macos-latest
             python-version: "3.10"
             nox-session: "tests"
           - os: ubuntu-latest
             python-version: "3.10"
+            nox-session: "doctest"
+          - os: ubuntu-latest
+            python-version: "3.10"
             nox-session: "lint"
 
     steps:
       - name: Checkout
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
         with:
           submodules: true
           fetch-depth: 0
       - name: Configure Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Cache pip packages
         uses: actions/cache@v3
         with:
           path: ~/.cache/pip
-          key: pip-${{ matrix.nox-session }}-${{ hashFiles('**/noxfile.py') }}
+          key: ${{ runner.os }}-pip-${{ matrix.nox-session }}-${{ hashFiles('**/noxfile.py') }}
           restore-keys: |
-            pip-${{ matrix.nox-session }}-
+            ${{ runner.os }}-pip-${{ matrix.nox-session }}-
       - name: Cache nox session files
         uses: actions/cache@v3
         with:
           path: .nox
-          key: nox-${{ matrix.nox-session }}-${{ hashFiles('**/noxfile.py') }}
+          key: ${{ runner.os }}-nox-${{ matrix.nox-session }}-${{ hashFiles('**/noxfile.py') }}
           restore-keys: |
-            nox-${{ matrix.nox-session }}-
+            ${{ runner.os }}-nox-${{ matrix.nox-session }}-
       - name: Cache pre-commit environments
         if: ${{ matrix.nox-session == 'lint' }}
         uses: actions/cache@v3
         with:
           path: ~/.cache/pre-commit
-          key: pre-commit-${{ hashFiles('.pre-commit-config.yaml') }}
+          key: ${{ runner.os }}-pre-commit-${{ hashFiles('.pre-commit-config.yaml') }}
           restore-keys: |
-            pre-commit-
+            ${{ runner.os }}-pre-commit-
       - name: Install nox
         run: |
           python -m pip install -U pip
           python -m pip install -U nox
       - name: Run tests
         run: python -m nox --non-interactive -s ${{ matrix.nox-session }}
 
-  release:
-    if: ${{ inputs.prerelease || startsWith(github.ref, 'refs/tags/') }}
-    needs: tests
-    uses: dfm/workflows/.github/workflows/python-release.yml@main
-    with:
-      wheels: false
-      enable-windows: false
-    secrets:
-      pypi-token: ${{ secrets.pypi_password }}
+  build:
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v3
+        with:
+          fetch-depth: 0
+      - uses: actions/setup-python@v4
+        name: Install Python
+        with:
+          python-version: "3.9"
+      - name: Build sdist and wheel
+        run: |
+          python -m pip install -U pip
+          python -m pip install -U build
+          python -m build .
+      - uses: actions/upload-artifact@v3
+        with:
+          path: dist/*
+
+  upload_pypi:
+    environment:
+      name: pypi
+      url: https://pypi.org/p/snakemake-staging
+    permissions:
+      id-token: write
+    needs: [tests, build]
+    runs-on: ubuntu-latest
+    if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags/')
+    steps:
+      - uses: actions/download-artifact@v3
+        with:
+          name: artifact
+          path: dist
+      - uses: pypa/gh-action-pypi-publish@v1.8.6
```

### Comparing `numpyro-ext-0.0.1/.pre-commit-config.yaml` & `numpyro-ext-0.0.2rc1/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -3,27 +3,28 @@
     hooks:
       - id: forbidden-files
         name: forbidden files
         entry: found copier update rejection files; review them and remove them
         language: fail
         files: "\\.rej$"
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
         exclude_types: [json, binary]
         exclude: ".copier-answers.yml"
       - id: check-yaml
-  - repo: https://github.com/PyCQA/isort
-    rev: "5.10.1"
+  - repo: https://github.com/charliermarsh/ruff-pre-commit
+    rev: "v0.0.265"
     hooks:
-      - id: isort
-        additional_dependencies: [toml]
+      - id: ruff
+        exclude: "^docs/"
+        args: [--fix, --exit-non-zero-on-fix]
   - repo: https://github.com/psf/black
-    rev: "22.6.0"
+    rev: "23.3.0"
     hooks:
       - id: black-jupyter
   - repo: https://github.com/kynan/nbstripout
-    rev: "0.5.0"
+    rev: "0.6.1"
     hooks:
       - id: nbstripout
```

### Comparing `numpyro-ext-0.0.1/CODE_OF_CONDUCT.md` & `numpyro-ext-0.0.2rc1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `numpyro-ext-0.0.1/CONTRIBUTING.md` & `numpyro-ext-0.0.2rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `numpyro-ext-0.0.1/LICENSE` & `numpyro-ext-0.0.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `numpyro-ext-0.0.1/src/numpyro_ext/__init__.py` & `numpyro-ext-0.0.2rc1/src/numpyro_ext/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,8 +8,11 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from numpyro_ext.version import version as __version__
+from numpyro_ext import distributions as distributions
+from numpyro_ext import infer as infer
+from numpyro_ext import optim as optim
+from numpyro_ext.info import information as information
```

### Comparing `numpyro-ext-0.0.1/src/numpyro_ext/distributions.py` & `numpyro-ext-0.0.2rc1/src/numpyro_ext/distributions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 __all__ = [
     "QuadLDParams",
     "UnitDisk",
     "Angle",
     "MixtureGeneral",
     "NoncentralChi2",
+    "MarginalizedLinear",
 ]
 
 import jax
 import jax.numpy as jnp
 import jax.scipy as jsp
 import numpyro.distributions as dist
 from jax import lax
+from jax.scipy.linalg import cho_factor, cho_solve
+from numpyro.distributions import MixtureGeneral as MixtureGeneral
 from numpyro.distributions import constraints, transforms
-from numpyro.distributions.util import (
-    is_prng_key,
-    promote_shapes,
-    validate_sample,
-)
+from numpyro.distributions.util import is_prng_key, promote_shapes, validate_sample
+
+from numpyro_ext.linear_op import to_linear_op
 
 # ---------------
 # - Constraints -
 # ---------------
 
 
 class _QuadLDConstraint(constraints.Constraint):
@@ -159,17 +160,15 @@
 
 @transforms.biject_to.register(unit_disk)
 def _(constraint):
     del constraint
     return transforms.ComposeTransform(
         [
             transforms.SigmoidTransform(),
-            transforms.AffineTransform(
-                -1.0, 2.0, domain=constraints.unit_interval
-            ),
+            transforms.AffineTransform(-1.0, 2.0, domain=constraints.unit_interval),
             UnitDiskTransform(),
         ]
     )
 
 
 @transforms.biject_to.register(angle)
 def _(constraint):
@@ -178,26 +177,29 @@
 
 # -----------------
 # - Distributions -
 # -----------------
 
 
 class QuadLDParams(dist.Distribution):
+    """An uninformative prior for quadratic limb darkening parameters
+
+    This is an implementation of the `Kipping (2013)
+    <https://arxiv.org/abs/1308.0009>`_ re-parameterization of the two-parameter
+    limb darkening model to allow for efficient and uninformative sampling.
+    """
+
     support = quad_ld
 
     def __init__(self, *, validate_args=None):
-        super().__init__(
-            batch_shape=(), event_shape=(2,), validate_args=validate_args
-        )
+        super().__init__(batch_shape=(), event_shape=(2,), validate_args=validate_args)
 
     def sample(self, key, sample_shape=()):
         assert is_prng_key(key)
-        q = jax.random.uniform(
-            key, shape=sample_shape + (2,), minval=0, maxval=1
-        )
+        q = jax.random.uniform(key, shape=sample_shape + (2,), minval=0, maxval=1)
         return QuadLDParams.q2u(q)
 
     @validate_sample
     def log_prob(self, value):
         return jnp.zeros_like(value[..., 0])
 
     @property
@@ -224,31 +226,29 @@
         u2 = u1 + u[..., 1]
         q1 = jnp.square(u2)
         q2 = 0.5 * u1 / u2
         return jnp.stack((q1, q2), axis=-1)
 
 
 class UnitDisk(dist.Distribution):
+    """Two dimensional parameters constrained to live within the unit disk"""
+
     support = unit_disk
 
     def __init__(self, *, validate_args=None):
-        super().__init__(
-            batch_shape=(), event_shape=(2,), validate_args=validate_args
-        )
+        super().__init__(batch_shape=(), event_shape=(2,), validate_args=validate_args)
 
     def sample(self, key, sample_shape=()):
         assert is_prng_key(key)
         key1, key2 = jax.random.split(key)
         theta = jax.random.uniform(
             key1, shape=sample_shape, minval=-jnp.pi, maxval=jnp.pi
         )
         r = jnp.sqrt(
-            jax.random.uniform(
-                key2, shape=sample_shape, minval=0.0, maxval=1.0
-            )
+            jax.random.uniform(key2, shape=sample_shape, minval=0.0, maxval=1.0)
         )
         return jnp.stack((r * jnp.cos(theta), r * jnp.sin(theta)), axis=-1)
 
     @validate_sample
     def log_prob(self, value):
         del value
         return -jnp.log(jnp.pi)
@@ -259,19 +259,30 @@
 
     @property
     def variance(self):
         return jnp.array([0.25, 0.25])
 
 
 class Angle(dist.Distribution):
+    """An angle constrained to be in the range -pi to pi
+
+    The actual sampling is performed in the two dimensional vector space
+    proportional to ``(sin(theta), cos(theta))`` so that the sampler doesn't see
+    a discontinuity at pi.
+
+    The ``regularized`` parameter can be used to improve sampling performance
+    when the value of the angle is well constrained. It removes prior mass near
+    the origin in the sampling space, which can lead to bad geometry when the
+    angle is poorly constrained, but better performance when it is. The default
+    value of ``10.0`` is a good starting point.
+    """
+
     def __init__(self, *, regularized=10.0, validate_args=None):
         self.regularized = regularized
-        super().__init__(
-            batch_shape=(), event_shape=(), validate_args=validate_args
-        )
+        super().__init__(batch_shape=(), event_shape=(), validate_args=validate_args)
 
     @constraints.dependent_property
     def support(self):
         return _AngleConstraint(self.regularized)
 
     def sample(self, key, sample_shape=()):
         assert is_prng_key(key)
@@ -296,229 +307,14 @@
         cdf = (value + 0.5 * jnp.pi) / jnp.pi
         return jnp.clip(cdf, a_min=0.0, a_max=1.0)
 
     def icdf(self, value):
         return (value - 0.5) * jnp.pi
 
 
-class MixtureGeneral(dist.Distribution):
-    def __init__(
-        self, mixing_distribution, distributions, *, validate_args=None
-    ):
-        _check_mixing_distribution(mixing_distribution)
-
-        self._mixture_size = jnp.shape(mixing_distribution.probs)[-1]
-        if isinstance(distributions, dist.Distribution):
-            distributions = [distributions] * self.mixture_size
-        try:
-            distributions = list(distributions)
-        except TypeError:
-            raise ValueError(
-                "The 'distributions' argument must be a list of Distribution objects"
-            )
-        for d in distributions:
-            if not isinstance(d, dist.Distribution):
-                raise ValueError(
-                    "All elements of 'distributions' must be instaces of "
-                    "numpyro.distributions.Distribution subclasses"
-                )
-        if len(distributions) != self.mixture_size:
-            raise ValueError(
-                "The number of elements in 'distributions' must match the mixture size; "
-                f"expected {self._mixture_size}, got {len(distributions)}"
-            )
-
-        # FIXME: It would be good to check the support, but __eq__ isn't implemented
-        #        properly for most constraints...
-        # if any(
-        #     d.support != distributions[0].support for d in distributions[1:]
-        # ):
-        #     raise ValueError("All distributions must have the same support.")
-
-        self._mixing_distribution = mixing_distribution
-        self._distributions = distributions
-
-        batch_shape = lax.broadcast_shapes(
-            mixing_distribution.batch_shape,
-            *(d.batch_shape for d in distributions),
-        )
-        event_shape = lax.broadcast_shapes(
-            mixing_distribution.event_shape,
-            *(d.event_shape for d in distributions),
-        )
-
-        super().__init__(
-            batch_shape=batch_shape,
-            event_shape=event_shape,
-            validate_args=validate_args,
-        )
-
-    @property
-    def mixture_size(self):
-        """
-        The number of distributions in the mixture
-
-        :return: number of mixtures.
-        :rtype: int
-        """
-        return self._mixture_size
-
-    @property
-    def mixing_distribution(self):
-        """
-        The mixing distribution
-
-        :return: Categorical distribution
-        :rtype: Categorical
-        """
-        return self._mixing_distribution
-
-    @property
-    def distributions(self):
-        """
-        The list of component distributions being mixed
-
-        :return: The list of component distributions
-        :rtype: List[Distribution]
-        """
-        return self._distributions
-
-    @property
-    def mixture_dim(self):
-        return -self.event_dim - 1
-
-    @constraints.dependent_property
-    def support(self):
-        return self.distributions[0].support
-
-    @property
-    def is_discrete(self):
-        return self.distributions[0].is_discrete
-
-    def tree_flatten(self):
-        mixing_flat, mixing_aux = self.mixing_distribution.tree_flatten()
-        dists_flat, dists_aux = zip(
-            *(d.tree_flatten() for d in self.distributions)
-        )
-        params = (mixing_flat, dists_flat)
-        aux_data = (
-            (
-                type(self.mixing_distribution),
-                tuple(type(d) for d in self.distributions),
-            ),
-            (mixing_aux, dists_aux),
-        )
-        return params, aux_data
-
-    @classmethod
-    def tree_unflatten(cls, aux_data, params):
-        params_mix, params_dists = params
-        (cls_mix, cls_dists), (mixing_aux, dists_aux) = aux_data
-        mixing_dist = cls_mix.tree_unflatten(mixing_aux, params_mix)
-        distributions = [
-            c.tree_unflatten(a, p)
-            for c, a, p in zip(cls_dists, dists_aux, params_dists)
-        ]
-        return cls(
-            mixing_distribution=mixing_dist, distributions=distributions
-        )
-
-    @property
-    def mean(self):
-        probs = self.mixing_distribution.probs
-        probs = probs.reshape(probs.shape + (1,) * self.event_dim)
-        means = jnp.stack(
-            [d.mean for d in self.distributions], axis=self.mixture_dim
-        )
-        return jnp.sum(probs * means, axis=self.mixture_dim)
-
-    @property
-    def variance(self):
-        probs = self.mixing_distribution.probs
-        probs = probs.reshape(probs.shape + (1,) * self.event_dim)
-
-        means = jnp.stack(
-            [d.mean for d in self.distributions], axis=self.mixture_dim
-        )
-        variances = jnp.stack(
-            [d.variance for d in self.distributions], axis=self.mixture_dim
-        )
-
-        mean_cond_var = jnp.sum(probs * variances, axis=self.mixture_dim)
-        sq_deviation = (
-            means - jnp.expand_dims(self.mean, axis=self.mixture_dim)
-        ) ** 2
-        var_cond_mean = jnp.sum(probs * sq_deviation, axis=self.mixture_dim)
-        return mean_cond_var + var_cond_mean
-
-    def cdf(self, samples):
-        """
-        The cumulative distribution function of this mixture distribution.
-
-        :param value: samples from this distribution.
-        :return: output of the cummulative distribution function evaluated at `value`.
-        :raises: NotImplementedError if the component distribution does not implement the cdf method.
-        """
-        cdfs = jnp.stack(
-            [d.cdf(samples) for d in self.distributions], axis=self.mixture_dim
-        )
-        return jnp.sum(cdfs * self.mixing_distribution.probs, axis=-1)
-
-    def sample_with_intermediates(self, key, sample_shape=()):
-        assert is_prng_key(key)
-
-        key_ind, *key_comp = jax.random.split(key, 1 + len(self.distributions))
-
-        samples = []
-        for k, d in zip(key_comp, self.distributions):
-            samples.append(d.expand(sample_shape + self.batch_shape).sample(k))
-        samples = jnp.stack(samples, axis=self.mixture_dim)
-
-        indices = self.mixing_distribution.expand(
-            sample_shape + self.batch_shape
-        ).sample(key_ind)
-        n_expand = self.event_dim + 1
-        indices_expanded = indices.reshape(indices.shape + (1,) * n_expand)
-
-        samples_selected = jnp.take_along_axis(
-            samples, indices=indices_expanded, axis=self.mixture_dim
-        )
-
-        return jnp.squeeze(samples_selected, axis=self.mixture_dim), indices
-
-    def sample(self, key, sample_shape=()):
-        return self.sample_with_intermediates(
-            key=key, sample_shape=sample_shape
-        )[0]
-
-    @validate_sample
-    def component_log_probs(self, value):
-        component_log_probs = jnp.stack(
-            [d.log_prob(value) for d in self.distributions],
-            axis=self.mixture_dim,
-        )
-        return self.mixing_distribution.logits + component_log_probs
-
-    @validate_sample
-    def log_prob(self, value, intermediates=None):
-        del intermediates
-        log_probs = self.component_log_probs(value)
-        return jax.nn.logsumexp(log_probs, axis=self.mixture_dim)
-
-
-def _check_mixing_distribution(mixing_distribution):
-    if not isinstance(
-        mixing_distribution, (dist.CategoricalLogits, dist.CategoricalProbs)
-    ):
-        raise ValueError(
-            "The mixing distribution must be a numpyro.distributions.Categorical. "
-            f"However, it is of type {type(mixing_distribution)}"
-        )
-
-
 class NoncentralChi2(dist.Distribution):
     arg_constraints = {
         "df": constraints.positive,
         "nc": constraints.positive,
     }
     support = constraints.positive
     reparametrized_params = ["df", "nc"]
@@ -532,17 +328,15 @@
 
     def sample(self, key, sample_shape=()):
         # Ref: https://github.com/numpy/numpy/blob/
         # 89c80ba606f4346f8df2a31cfcc0e967045a68ed/numpy/
         # random/src/distributions/distributions.c#L797-L813
 
         def _random_chi2(key, df, shape=(), dtype=jnp.float_):
-            return 2.0 * jax.random.gamma(
-                key, 0.5 * df, shape=shape, dtype=dtype
-            )
+            return 2.0 * jax.random.gamma(key, 0.5 * df, shape=shape, dtype=dtype)
 
         assert is_prng_key(key)
         shape = sample_shape + self.batch_shape + self.event_shape
 
         key1, key2, key3 = jax.random.split(key, 3)
         i = jax.random.poisson(key1, 0.5 * self.nc, shape=shape)
         n = jax.random.normal(key2, shape=shape) + jnp.sqrt(self.nc)
@@ -554,36 +348,200 @@
         )
         return jnp.where(cond, chi2 + n * n, chi2)
 
     @validate_sample
     def log_prob(self, value):
         try:
             import tensorflow_probability.substrates.jax as tfp
-        except ImportError:
+        except ImportError as e:
             raise ImportError(
                 "tensorflow-probability is must be installed to use the "
                 "NoncentralChi2 distribution."
-            )
+            ) from e
 
         # Ref: https://github.com/scipy/scipy/blob/
         # 500878e88eacddc7edba93dda7d9ee5f784e50e6/scipy/
         # stats/_distn_infrastructure.py#L597-L610
         df2 = self.df / 2.0 - 1.0
         xs, ns = jnp.sqrt(value), jnp.sqrt(self.nc)
-        res = (
-            jsp.special.xlogy(df2 / 2.0, value / self.nc)
-            - 0.5 * (xs - ns) ** 2
-        )
+        res = jsp.special.xlogy(df2 / 2.0, value / self.nc) - 0.5 * (xs - ns) ** 2
         corr = tfp.math.bessel_ive(df2, xs * ns) / 2.0
         return jnp.where(
             jnp.greater(corr, 0.0),
             res + jnp.log(corr),
             -jnp.inf,
         )
 
     @property
     def mean(self):
         return self.df + self.nc
 
     @property
     def variance(self):
         return 2.0 * (self.df + 2.0 * self.nc)
+
+
+class MarginalizedLinear(dist.Distribution):
+    arg_constraints = {"design_matrix": constraints.real}
+    support = constraints.real_vector
+    reparametrized_params = ["design_matrix"]
+
+    def __init__(
+        self,
+        design_matrix,
+        prior_distribution,
+        data_distribution,
+        *,
+        validate_args=None,
+    ):
+        # We treat the trailing dimensions of the design matrix as "ground
+        # truth" for the dimensions of the problem.
+        if jnp.ndim(design_matrix) < 2:
+            raise ValueError("The design matrix must have at least 2 dimensions")
+        data_size, latent_size = jnp.shape(design_matrix)[-2:]
+
+        # We don't really care about the batch vs. event shapes of the input
+        # distributions, so instead we just check that the trailing dimensions
+        # are correct.
+        prior_dist_shape = tuple(prior_distribution.batch_shape) + tuple(
+            prior_distribution.event_shape
+        )
+        if len(prior_dist_shape) != 0 and prior_dist_shape[-1] != latent_size:
+            raise ValueError(
+                "The trailing dimensions of the prior distribution must match "
+                "the latent dimension defined by the design matrix; expected "
+                f"(..., {latent_size}), got {prior_dist_shape}"
+            )
+
+        data_dist_shape = tuple(data_distribution.batch_shape) + tuple(
+            data_distribution.event_shape
+        )
+        if len(data_dist_shape) != 0 and data_dist_shape[-1] != data_size:
+            raise ValueError(
+                "The trailing dimensions of the data distribution must match "
+                "the data dimension defined by the design matrix; expected "
+                f"(..., {data_size}), got {data_dist_shape}"
+            )
+
+        # We broadcast the relevant batch shapes to find the batch shape of this
+        # distribution, and expand or reshape all the members to match.
+        batch_shape = lax.broadcast_shapes(
+            design_matrix.shape[:-2],
+            prior_dist_shape[:-1],
+            data_dist_shape[:-1],
+        )
+        event_shape = (data_size,)
+        self.design_matrix = jnp.broadcast_to(
+            design_matrix, batch_shape + (data_size, latent_size)
+        )
+
+        if prior_distribution.event_shape == ():
+            self.prior_distribution = prior_distribution.expand(
+                batch_shape + (latent_size,)
+            )
+        else:
+            self.prior_distribution = prior_distribution.expand(batch_shape)
+
+        if data_distribution.event_shape == ():
+            self.data_distribution = data_distribution.expand(
+                batch_shape + (data_size,)
+            )
+        else:
+            self.data_distribution = data_distribution.expand(batch_shape)
+
+        super().__init__(
+            batch_shape=batch_shape,
+            event_shape=event_shape,
+            validate_args=validate_args,
+        )
+
+    def sample_with_intermediates(self, key, sample_shape=()):
+        assert is_prng_key(key)
+        prior_key, data_key = jax.random.split(key)
+        prior_sample = self.prior_distribution.sample(
+            prior_key, sample_shape=sample_shape
+        )
+        data_sample = self.data_distribution.sample(data_key, sample_shape=sample_shape)
+        delta = jnp.einsum("...ij,...j->...i", self.design_matrix, prior_sample)
+        return data_sample + delta, [prior_sample]
+
+    def sample(self, key, sample_shape=()):
+        return self.sample_with_intermediates(key, sample_shape)[0]
+
+    def log_prob_and_conditional(self, value):
+        data_size, _ = jnp.shape(self.design_matrix)[-2:]
+        assert jnp.shape(value)[-1] == data_size
+        prior = to_linear_op(self.prior_distribution)
+        data = to_linear_op(self.data_distribution)
+
+        def inner(a, b):
+            aT = jnp.swapaxes(a, -2, -1)
+            return aT @ b
+
+        # This inner matrix is used for both the matrix determinant and inverse
+        data_tril = data.solve_tril(self.design_matrix, False)
+        sigma = prior.inverse() + inner(data_tril, data_tril)
+        factor, lower = cho_factor(sigma, lower=True)
+
+        # Use the matrix determinant lemma to compute the full determinant
+        hld = jnp.sum(jnp.log(jnp.diagonal(factor, axis1=-2, axis2=-1)), -1)
+        norm = hld + prior.half_log_det() + data.half_log_det()
+
+        # Use the Woodbury matrix identity to solve the linear system
+        resid = (value - self.mean)[..., None]
+        alpha = data.solve_tril(resid, False)
+        result = inner(alpha, alpha)
+        alpha = inner(data_tril, alpha)
+        result -= inner(alpha, cho_solve((factor, lower), alpha))
+        log_prob = (
+            -0.5 * result[..., 0, 0] - norm - 0.5 * data_size * jnp.log(2 * jnp.pi)
+        )
+
+        # Evaluate the conditional mean
+        a = prior.solve_tril(prior.solve_tril(prior.loc()[..., None], False), True)
+        a = cho_solve((factor, lower), (a + alpha)[..., 0])
+
+        return log_prob, dist.MultivariateNormal(loc=a, precision_matrix=sigma)
+
+    @validate_sample
+    def log_prob(self, value):
+        return self.log_prob_and_conditional(value)[0]
+
+    def conditional(self, value=None):
+        if value is None:
+            return self.prior_distribution
+        return self.log_prob_and_conditional(value)[1]
+
+    def tree_flatten(self):
+        prior_flat, prior_aux = self.prior_distribution.tree_flatten()
+        data_flat, data_aux = self.data_distribution.tree_flatten()
+        return (self.design_matrix, prior_flat, data_flat), (
+            type(self.prior_distribution),
+            prior_aux,
+            type(self.data_distribution),
+            data_aux,
+        )
+
+    @classmethod
+    def tree_unflatten(cls, aux_data, params):
+        design_matrix, prior_flat, data_flat = params
+        prior_dist = aux_data[0].tree_unflatten(aux_data[1], prior_flat)
+        data_dist = aux_data[2].tree_unflatten(aux_data[3], data_flat)
+        return cls(
+            design_matrix=design_matrix,
+            prior_distribution=prior_dist,
+            data_distribution=data_dist,
+        )
+
+    @property
+    def mean(self):
+        mu = self.prior_distribution.mean[..., None]
+        mu = jnp.broadcast_to(mu, self.batch_shape + mu.shape[-2:])
+        return self.data_distribution.mean + (self.design_matrix @ mu)[..., 0]
+
+    @property
+    def covariance_matrix(self):
+        prior = to_linear_op(self.prior_distribution)
+        data = to_linear_op(self.data_distribution)
+        return data.cov() + self.design_matrix @ prior.cov() @ jnp.swapaxes(
+            self.design_matrix, -2, -1
+        )
```

