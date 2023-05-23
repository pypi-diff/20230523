# Comparing `tmp/hyperparameter-0.5.1.tar.gz` & `tmp/hyperparameter-0.5.2.tar.gz`

## Comparing `hyperparameter-0.5.1.tar` & `hyperparameter-0.5.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 hyperparameter-0.5.1/Cargo.toml
--rw-r--r--   0     1001      123      834 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0     1001      123      126 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/.github/ISSUE_TEMPLATE/custom.md
--rw-r--r--   0     1001      123      595 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0     1001      123      706 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/.github/workflows/codecov.yml
--rw-r--r--   0     1001      123      845 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/.github/workflows/mkdocs.yml
--rw-r--r--   0     1001      123     1202 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/.github/workflows/python-publish.yml
--rw-r--r--   0     1001      123     2001 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/.gitignore
--rw-r--r--   0     1001      123      356 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/.pre-commit-config.yaml
--rw-r--r--   0     1001      123     5202 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/CODE_OF_CONDUCT.md
--rw-r--r--   0     1001      123    22947 2023-05-16 03:06:41.000000 hyperparameter-0.5.1/Cargo.lock
--rw-r--r--   0     1001      123    11356 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/LICENSE
--rw-r--r--   0     1001      123     3861 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/README.md
--rw-r--r--   0     1001      123     3457 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/README.zh.md
--rw-r--r--   0     1001      123     2846 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/docs/examples/optimization.md
--rw-r--r--   0     1001      123     2868 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/docs/examples/optimization.zh.md
--rw-r--r--   0     1001      123     3861 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/docs/index.md
--rw-r--r--   0     1001      123     3457 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/docs/index.zh.md
--rw-r--r--   0     1001      123     3000 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/docs/quick_start.md
--rw-r--r--   0     1001      123     3000 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/docs/quick_start.zh.md
--rw-r--r--   0     1001      123       48 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/docs/reference.md
--rw-r--r--   0     1001      123      110 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/docs/requirements.txt
--rw-r--r--   0     1001      123     6738 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/docs/structured_parameter.md
--rw-r--r--   0     1001      123      337 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/application/README.md
--rw-r--r--   0     1001      123      789 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/application/app.py
--rw-r--r--   0     1001      123       46 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/application/cfg.json
--rw-r--r--   0     1001      123     4733 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/automl_optuna_mnist/automl_mnist.py
--rw-r--r--   0     1001      123     2047 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/cpp/cxx_test.cc
--rw-r--r--   0     1001      123      271 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/cpp/cxx_test.py
--rw-r--r--   0     1001      123      237 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/cpp/cxx_test.sh
--rw-r--r--   0     1001      123      152 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/mnist/README.md
--rw-r--r--   0     1001      123     5625 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/mnist/main.py
--rw-r--r--   0     1001      123     5899 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/mnist/main_with_hp.py
--rw-r--r--   0     1001      123     6202 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/mnist/main_with_hp_with_mlflow.py
--rw-r--r--   0     1001      123       18 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/mnist/requirements.txt
--rw-r--r--   0     1001      123     2846 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/optuna/README.md
--rw-r--r--   0     1001      123      230 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/optuna/example.py
--rw-r--r--   0     1001      123      527 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/optuna/example_hp.py
--rw-r--r--   0     1001      123      727 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/optuna/example_hp_nested.py
--rw-r--r--   0     1001      123     1650 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/sparse_lr/README.md
--rw-r--r--   0     1001      123      581 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/sparse_lr/example_1.py
--rw-r--r--   0     1001      123      934 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/sparse_lr/example_2.py
--rw-r--r--   0     1001      123     1059 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/sparse_lr/example_mlflow.py
--rw-r--r--   0     1001      123      867 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/sparse_lr/model.py
--rw-r--r--   0     1001      123     1631 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/storage.rs
--rw-r--r--   0     1001      123        0 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/hparam/__init__.py
--rw-r--r--   0     1001      123     3710 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/hparam/__main__.py
--rw-r--r--   0     1001      123      314 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/hyperparameter/__init__.py
--rw-r--r--   0     1001      123    17127 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/hyperparameter/api.py
--rw-r--r--   0     1001      123     7588 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/hyperparameter/hyperparameter.h
--rw-r--r--   0     1001      123      828 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/hyperparameter/loader.py
--rw-r--r--   0     1001      123     4196 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/hyperparameter/storage.py
--rw-r--r--   0     1001      123     2223 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/hyperparameter/tune.py
--rw-r--r--   0     1001      123     1249 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/mkdocs.yml
--rw-r--r--   0     1001      123      938 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/pyproject.toml
--rw-r--r--   0     1001      123     5571 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/src/entry.rs
--rw-r--r--   0     1001      123     6580 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/src/ext.rs
--rw-r--r--   0     1001      123     2038 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/src/ffi.rs
--rw-r--r--   0     1001      123      106 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/src/lib.rs
--rw-r--r--   0     1001      123     8129 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/src/storage.rs
--rw-r--r--   0     1001      123     4528 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/src/xxh.rs
--rwxr-xr-x   0     1001      123    40754 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/tests/a.out
--rw-r--r--   0     1001      123      912 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/tests/test_auto_param.py
--rw-r--r--   0     1001      123     3769 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/tests/test_param_scope.py
--rw-r--r--   0     1001      123      697 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/tests/test_param_scope_thread.py
--rw-r--r--   0     1001      123     2988 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/tests/test_rust_backend.py
--rw-r--r--   0        0        0     4210 1970-01-01 00:00:00.000000 hyperparameter-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      442 1970-01-01 00:00:00.000000 hyperparameter-0.5.2/Cargo.toml
+-rw-r--r--   0     1001      123      834 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0     1001      123      126 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0     1001      123      595 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0     1001      123      706 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/.github/workflows/codecov.yml
+-rw-r--r--   0     1001      123      845 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/.github/workflows/mkdocs.yml
+-rw-r--r--   0     1001      123     1202 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/.github/workflows/python-publish.yml
+-rw-r--r--   0     1001      123     2001 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/.gitignore
+-rw-r--r--   0     1001      123      356 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/.pre-commit-config.yaml
+-rw-r--r--   0     1001      123     5202 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0     1001      123    22513 2023-05-23 05:58:25.000000 hyperparameter-0.5.2/Cargo.lock
+-rw-r--r--   0     1001      123    11356 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/LICENSE
+-rw-r--r--   0     1001      123     3861 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/README.md
+-rw-r--r--   0     1001      123     3457 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/README.zh.md
+-rw-r--r--   0     1001      123     2846 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/docs/examples/optimization.md
+-rw-r--r--   0     1001      123     2868 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/docs/examples/optimization.zh.md
+-rw-r--r--   0     1001      123     3861 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/docs/index.md
+-rw-r--r--   0     1001      123     3457 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/docs/index.zh.md
+-rw-r--r--   0     1001      123     3000 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/docs/quick_start.md
+-rw-r--r--   0     1001      123     3000 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/docs/quick_start.zh.md
+-rw-r--r--   0     1001      123       48 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/docs/reference.md
+-rw-r--r--   0     1001      123      110 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/docs/requirements.txt
+-rw-r--r--   0     1001      123     6738 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/docs/structured_parameter.md
+-rw-r--r--   0     1001      123      337 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/application/README.md
+-rw-r--r--   0     1001      123      789 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/application/app.py
+-rw-r--r--   0     1001      123       46 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/application/cfg.json
+-rw-r--r--   0     1001      123     4733 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/automl_optuna_mnist/automl_mnist.py
+-rw-r--r--   0     1001      123     2047 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/cpp/cxx_test.cc
+-rw-r--r--   0     1001      123      271 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/cpp/cxx_test.py
+-rw-r--r--   0     1001      123      237 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/cpp/cxx_test.sh
+-rw-r--r--   0     1001      123      152 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/mnist/README.md
+-rw-r--r--   0     1001      123     5625 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/mnist/main.py
+-rw-r--r--   0     1001      123     5899 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/mnist/main_with_hp.py
+-rw-r--r--   0     1001      123     6202 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/mnist/main_with_hp_with_mlflow.py
+-rw-r--r--   0     1001      123       18 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/mnist/requirements.txt
+-rw-r--r--   0     1001      123     2846 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/optuna/README.md
+-rw-r--r--   0     1001      123      230 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/optuna/example.py
+-rw-r--r--   0     1001      123      527 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/optuna/example_hp.py
+-rw-r--r--   0     1001      123      727 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/optuna/example_hp_nested.py
+-rw-r--r--   0     1001      123     1650 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/sparse_lr/README.md
+-rw-r--r--   0     1001      123      581 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/sparse_lr/example_1.py
+-rw-r--r--   0     1001      123      934 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/sparse_lr/example_2.py
+-rw-r--r--   0     1001      123     1059 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/sparse_lr/example_mlflow.py
+-rw-r--r--   0     1001      123      867 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/sparse_lr/model.py
+-rw-r--r--   0     1001      123     1631 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/storage.rs
+-rw-r--r--   0     1001      123        0 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/hparam/__init__.py
+-rw-r--r--   0     1001      123     3710 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/hparam/__main__.py
+-rw-r--r--   0     1001      123      314 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/hyperparameter/__init__.py
+-rw-r--r--   0     1001      123    17127 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/hyperparameter/api.py
+-rw-r--r--   0     1001      123     7588 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/hyperparameter/hyperparameter.h
+-rw-r--r--   0     1001      123      828 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/hyperparameter/loader.py
+-rw-r--r--   0     1001      123     4196 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/hyperparameter/storage.py
+-rw-r--r--   0     1001      123     2223 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/hyperparameter/tune.py
+-rw-r--r--   0     1001      123     1249 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/mkdocs.yml
+-rw-r--r--   0     1001      123      938 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/pyproject.toml
+-rw-r--r--   0     1001      123     5460 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/src/entry.rs
+-rw-r--r--   0     1001      123     6580 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/src/ext.rs
+-rw-r--r--   0     1001      123     2038 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/src/ffi.rs
+-rw-r--r--   0     1001      123      106 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/src/lib.rs
+-rw-r--r--   0     1001      123     8129 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/src/storage.rs
+-rw-r--r--   0     1001      123     4528 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/src/xxh.rs
+-rwxr-xr-x   0     1001      123    40754 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/tests/a.out
+-rw-r--r--   0     1001      123      912 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/tests/test_auto_param.py
+-rw-r--r--   0     1001      123     3769 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/tests/test_param_scope.py
+-rw-r--r--   0     1001      123      697 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/tests/test_param_scope_thread.py
+-rw-r--r--   0     1001      123     2988 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/tests/test_rust_backend.py
+-rw-r--r--   0        0        0     4210 1970-01-01 00:00:00.000000 hyperparameter-0.5.2/PKG-INFO
```

### Comparing `hyperparameter-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md` & `hyperparameter-0.5.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/.github/ISSUE_TEMPLATE/feature_request.md` & `hyperparameter-0.5.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/.github/workflows/codecov.yml` & `hyperparameter-0.5.2/.github/workflows/codecov.yml`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/.github/workflows/mkdocs.yml` & `hyperparameter-0.5.2/.github/workflows/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/.github/workflows/python-publish.yml` & `hyperparameter-0.5.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/.gitignore` & `hyperparameter-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/CODE_OF_CONDUCT.md` & `hyperparameter-0.5.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/Cargo.lock` & `hyperparameter-0.5.2/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,12 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
-name = "arraystring"
-version = "0.3.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4d517c467117e1d8ca795bc8cc90857ff7f79790cca0e26f6e9462694ece0185"
-dependencies = [
- "typenum",
-]
-
-[[package]]
 name = "atty"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
 dependencies = [
  "hermit-abi 0.1.19",
  "libc",
@@ -38,17 +29,17 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bumpalo"
-version = "3.12.2"
+version = "3.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c6ed94e98ecff0c12dd1b04c15ec0d7d9458ca8fe806cea6f12954efe74c63b"
+checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
 
 [[package]]
 name = "cc"
 version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
 
@@ -252,17 +243,16 @@
 checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "hyperparameter"
-version = "0.1.0"
+version = "0.5.2"
 dependencies = [
- "arraystring",
  "cxx",
  "lazy_static",
  "pyo3",
  "rspec",
 ]
 
 [[package]]
@@ -375,17 +365,17 @@
 name = "proc-macro-hack"
 version = "0.5.20+deprecated"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.57"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c4ec6d5fe0b140acb27c9a0444118cf55bfbb4e0b259739429abb4521dd67c16"
+checksum = "fa1fb82fc0c281dd9671101b66b771ebbe1eaf967b96ac8740dcba4b70005ca8"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.18.3"
@@ -711,20 +701,14 @@
  "proc-macro2",
  "quote",
  "standback",
  "syn 1.0.109",
 ]
 
 [[package]]
-name = "typenum"
-version = "1.16.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
-
-[[package]]
 name = "unicode-ident"
 version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
 
 [[package]]
 name = "unindent"
```

### Comparing `hyperparameter-0.5.1/LICENSE` & `hyperparameter-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/README.md` & `hyperparameter-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/README.zh.md` & `hyperparameter-0.5.2/README.zh.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/docs/examples/optimization.md` & `hyperparameter-0.5.2/docs/examples/optimization.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/docs/examples/optimization.zh.md` & `hyperparameter-0.5.2/docs/examples/optimization.zh.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/docs/index.md` & `hyperparameter-0.5.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/docs/index.zh.md` & `hyperparameter-0.5.2/docs/index.zh.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/docs/quick_start.md` & `hyperparameter-0.5.2/docs/quick_start.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/docs/quick_start.zh.md` & `hyperparameter-0.5.2/docs/quick_start.zh.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/docs/structured_parameter.md` & `hyperparameter-0.5.2/docs/structured_parameter.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/examples/application/app.py` & `hyperparameter-0.5.2/examples/application/app.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/examples/automl_optuna_mnist/automl_mnist.py` & `hyperparameter-0.5.2/examples/automl_optuna_mnist/automl_mnist.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/examples/cpp/cxx_test.cc` & `hyperparameter-0.5.2/examples/cpp/cxx_test.cc`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/examples/mnist/main.py` & `hyperparameter-0.5.2/examples/mnist/main.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/examples/mnist/main_with_hp.py` & `hyperparameter-0.5.2/examples/mnist/main_with_hp.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/examples/mnist/main_with_hp_with_mlflow.py` & `hyperparameter-0.5.2/examples/mnist/main_with_hp_with_mlflow.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/examples/optuna/README.md` & `hyperparameter-0.5.2/examples/optuna/README.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/examples/optuna/example_hp.py` & `hyperparameter-0.5.2/examples/optuna/example_hp.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/examples/optuna/example_hp_nested.py` & `hyperparameter-0.5.2/examples/optuna/example_hp_nested.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/examples/sparse_lr/README.md` & `hyperparameter-0.5.2/examples/sparse_lr/README.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/examples/sparse_lr/example_1.py` & `hyperparameter-0.5.2/examples/sparse_lr/example_1.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/examples/sparse_lr/example_2.py` & `hyperparameter-0.5.2/examples/sparse_lr/example_2.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/examples/sparse_lr/example_mlflow.py` & `hyperparameter-0.5.2/examples/sparse_lr/example_mlflow.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/examples/sparse_lr/model.py` & `hyperparameter-0.5.2/examples/sparse_lr/model.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/examples/storage.rs` & `hyperparameter-0.5.2/examples/storage.rs`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/hparam/__main__.py` & `hyperparameter-0.5.2/hparam/__main__.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/hyperparameter/api.py` & `hyperparameter-0.5.2/hyperparameter/api.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/hyperparameter/hyperparameter.h` & `hyperparameter-0.5.2/hyperparameter/hyperparameter.h`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/hyperparameter/loader.py` & `hyperparameter-0.5.2/hyperparameter/loader.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/hyperparameter/storage.py` & `hyperparameter-0.5.2/hyperparameter/storage.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/hyperparameter/tune.py` & `hyperparameter-0.5.2/hyperparameter/tune.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/mkdocs.yml` & `hyperparameter-0.5.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/pyproject.toml` & `hyperparameter-0.5.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "hyperparameter"
-version = "0.5.1"
+version = "0.5.2"
 authors = [{ name = "Reiase", email = "reiase@gmail.com" }]
 description = "A hyper-parameter library for researchers, data scientists and machine learning engineers."
 requires-python = ">=3.7"
 readme = "README.md"
 license = { text = "Apache License Version 2.0" }
 
 [tool.maturin]
```

### Comparing `hyperparameter-0.5.1/src/entry.rs` & `hyperparameter-0.5.2/src/entry.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-use arraystring::CacheString;
 use std::{ffi::c_void, sync::Arc};
 
 #[derive(Debug, Clone, PartialEq)]
 pub struct DeferUnsafe(pub *mut c_void, pub unsafe fn(*mut c_void));
 
 impl Drop for DeferUnsafe {
     fn drop(&mut self) {
@@ -11,15 +10,15 @@
 }
 
 #[derive(Debug, Clone, PartialEq)]
 pub enum Value {
     Empty,
     Int(i64),
     Float(f64),
-    Text(CacheString),
+    Text(String),
     Boolen(bool),
     UserDefined(
         *mut c_void,              //data
         i32,                      //kind
         Option<Arc<DeferUnsafe>>, // de-allocator
     ),
 }
@@ -34,27 +33,27 @@
     fn from(value: f64) -> Self {
         Value::Float(value)
     }
 }
 
 impl From<String> for Value {
     fn from(value: String) -> Self {
-        Value::Text(CacheString::from_str_truncate(value))
+        Value::Text(value)
     }
 }
 
 impl From<&String> for Value {
     fn from(value: &String) -> Self {
-        Value::Text(CacheString::from_str_truncate(value))
+        Value::Text(value.clone())
     }
 }
 
 impl From<&str> for Value {
     fn from(value: &str) -> Self {
-        Value::Text(CacheString::from_str_truncate(value))
+        Value::Text(value.to_string())
     }
 }
 
 impl From<bool> for Value {
     fn from(value: bool) -> Self {
         Value::Boolen(value)
     }
```

### Comparing `hyperparameter-0.5.1/src/ext.rs` & `hyperparameter-0.5.2/src/ext.rs`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/src/ffi.rs` & `hyperparameter-0.5.2/src/ffi.rs`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/src/storage.rs` & `hyperparameter-0.5.2/src/storage.rs`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/src/xxh.rs` & `hyperparameter-0.5.2/src/xxh.rs`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/tests/a.out` & `hyperparameter-0.5.2/tests/a.out`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/tests/test_auto_param.py` & `hyperparameter-0.5.2/tests/test_auto_param.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/tests/test_param_scope.py` & `hyperparameter-0.5.2/tests/test_param_scope.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/tests/test_param_scope_thread.py` & `hyperparameter-0.5.2/tests/test_param_scope_thread.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/tests/test_rust_backend.py` & `hyperparameter-0.5.2/tests/test_rust_backend.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.1/PKG-INFO` & `hyperparameter-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperparameter
-Version: 0.5.1
+Version: 0.5.2
 License-File: LICENSE
 Summary: A hyper-parameter library for researchers, data scientists and machine learning engineers.
 Author-email: Reiase <reiase@gmail.com>
 License: Apache License Version 2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

