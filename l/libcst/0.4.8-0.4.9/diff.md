# Comparing `tmp/libcst-0.4.8.tar.gz` & `tmp/libcst-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libcst-0.4.8.tar", last modified: Thu Nov 10 10:06:26 2022, max compression
+gzip compressed data, was "libcst-0.4.9.tar", last modified: Thu Nov 10 21:32:33 2022, max compression
```

## Comparing `libcst-0.4.8.tar` & `libcst-0.4.9.tar`

### file list

```diff
@@ -1,489 +1,489 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.279847 libcst-0.4.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.231846 libcst-0.4.8/.cargo/
--rw-r--r--   0 runner    (1001) docker     (121)      223 2022-11-10 10:06:10.000000 libcst-0.4.8/.cargo/config.toml
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-11-10 10:06:10.000000 libcst-0.4.8/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-11-10 10:06:10.000000 libcst-0.4.8/.fixit.config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     5318 2022-11-10 10:06:10.000000 libcst-0.4.8/.flake8
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-11-10 10:06:10.000000 libcst-0.4.8/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.231846 libcst-0.4.8/.github/
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-11-10 10:06:10.000000 libcst-0.4.8/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (121)      526 2022-11-10 10:06:10.000000 libcst-0.4.8/.github/build-matrix.json
--rw-r--r--   0 runner    (1001) docker     (121)      327 2022-11-10 10:06:10.000000 libcst-0.4.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.231846 libcst-0.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2911 2022-11-10 10:06:10.000000 libcst-0.4.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)     6542 2022-11-10 10:06:10.000000 libcst-0.4.8/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1962 2022-11-10 10:06:10.000000 libcst-0.4.8/.github/workflows/pypi_upload.yml
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-11-10 10:06:10.000000 libcst-0.4.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-11-10 10:06:10.000000 libcst-0.4.8/.pyre_configuration
--rw-r--r--   0 runner    (1001) docker     (121)      311 2022-11-10 10:06:10.000000 libcst-0.4.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-11-10 10:06:10.000000 libcst-0.4.8/.watchmanconfig
--rw-r--r--   0 runner    (1001) docker     (121)    32176 2022-11-10 10:06:10.000000 libcst-0.4.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     3535 2022-11-10 10:06:10.000000 libcst-0.4.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1462 2022-11-10 10:06:10.000000 libcst-0.4.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     4698 2022-11-10 10:06:10.000000 libcst-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-11-10 10:06:10.000000 libcst-0.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    11081 2022-11-10 10:06:26.279847 libcst-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10297 2022-11-10 10:06:10.000000 libcst-0.4.8/README.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)      992 2022-11-10 10:06:10.000000 libcst-0.4.8/check_copyright.sh
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-11-10 10:06:10.000000 libcst-0.4.8/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.211845 libcst-0.4.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.231846 libcst-0.4.8/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.231846 libcst-0.4.8/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (121)      385 2022-11-10 10:06:10.000000 libcst-0.4.8/docs/source/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.235846 libcst-0.4.8/docs/source/_static/img/
--rw-r--r--   0 runner    (1001) docker     (121)   108465 2022-11-10 10:06:10.000000 libcst-0.4.8/docs/source/_static/img/python_scopes.png
--rw-r--r--   0 runner    (1001) docker     (121)    30400 2022-11-10 10:06:10.000000 libcst-0.4.8/docs/source/_static/img/python_scopes.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.235846 libcst-0.4.8/docs/source/_static/logo/
--rw-r--r--   0 runner    (1001) docker     (121)     3638 2022-11-10 10:06:10.000000 libcst-0.4.8/docs/source/_static/logo/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)     3629 2022-11-10 10:06:10.000000 libcst-0.4.8/docs/source/_static/logo/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (121)      676 2022-11-10 10:06:10.000000 libcst-0.4.8/docs/source/_static/logo/favicon_16px.png
--rw-r--r--   0 runner    (1001) docker     (121)     1515 2022-11-10 10:06:10.000000 libcst-0.4.8/docs/source/_static/logo/favicon_32px.png
--rw-r--r--   0 runner    (1001) docker     (121)     4899 2022-11-10 10:06:10.000000 libcst-0.4.8/docs/source/_static/logo/horizontal.svg
--rw-r--r--   0 runner    (1001) docker     (121)     4884 2022-11-10 10:06:10.000000 libcst-0.4.8/docs/source/_static/logo/horizontal_white.svg
--rw-r--r--   0 runner    (1001) docker     (121)     8823 2022-11-10 10:06:10.000000 libcst-0.4.8/docs/source/_static/logo/horizontal_white_sidebar.png
--rw-r--r--   0 runner    (1001) docker     (121)     3336 2022-11-10 10:06:10.000000 libcst-0.4.8/docs/source/_static/logo/icon.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3339 2022-11-10 10:06:10.000000 libcst-0.4.8/docs/source/_static/logo/icon_white.svg
--rw-r--r--   0 runner    (1001) docker     (121)     4791 2022-11-10 10:06:10.000000 libcst-0.4.8/docs/source/_static/logo/vertical.svg
--rw-r--r--   0 runner    (1001) docker     (121)     4776 2022-11-10 10:06:10.000000 libcst-0.4.8/docs/source/_static/logo/vertical_white.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.235846 libcst-0.4.8/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-11-10 10:06:10.000000 libcst-0.4.8/docs/source/_templates/page.html
--rw-r--r--   0 runner    (1001) docker     (121)     8658 2022-11-10 10:06:10.000000 libcst-0.4.8/docs/source/best_practices.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8085 2022-11-10 10:06:10.000000 libcst-0.4.8/docs/source/codemods.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8644 2022-11-10 10:06:10.000000 libcst-0.4.8/docs/source/codemods_tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9553 2022-11-10 10:06:10.000000 libcst-0.4.8/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-11-10 10:06:10.000000 libcst-0.4.8/docs/source/experimental.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-11-10 10:06:10.000000 libcst-0.4.8/docs/source/helpers.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1008 2022-11-10 10:06:10.000000 libcst-0.4.8/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8876 2022-11-10 10:06:10.000000 libcst-0.4.8/docs/source/matchers.rst
--rw-r--r--   0 runner    (1001) docker     (121)    13597 2022-11-10 10:06:10.000000 libcst-0.4.8/docs/source/matchers_tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     9920 2022-11-10 10:06:10.000000 libcst-0.4.8/docs/source/metadata.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5347 2022-11-10 10:06:10.000000 libcst-0.4.8/docs/source/metadata_tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     3979 2022-11-10 10:06:10.000000 libcst-0.4.8/docs/source/motivation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9632 2022-11-10 10:06:10.000000 libcst-0.4.8/docs/source/nodes.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1252 2022-11-10 10:06:10.000000 libcst-0.4.8/docs/source/parser.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10261 2022-11-10 10:06:10.000000 libcst-0.4.8/docs/source/scope_tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     9873 2022-11-10 10:06:10.000000 libcst-0.4.8/docs/source/tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     5369 2022-11-10 10:06:10.000000 libcst-0.4.8/docs/source/visitors.rst
--rw-r--r--   0 runner    (1001) docker     (121)    15454 2022-11-10 10:06:10.000000 libcst-0.4.8/docs/source/why_libcst.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.235846 libcst-0.4.8/libcst/
--rw-r--r--   0 runner    (1001) docker     (121)     8492 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2911 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_add_slots.py
--rw-r--r--   0 runner    (1001) docker     (121)     5666 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_batched_visitor.py
--rw-r--r--   0 runner    (1001) docker     (121)     8017 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1618 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_flatten_sentinel.py
--rw-r--r--   0 runner    (1001) docker     (121)     2443 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_maybe_sentinel.py
--rw-r--r--   0 runner    (1001) docker     (121)     4832 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_metadata_dependent.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.239846 libcst-0.4.8/libcst/_nodes/
--rw-r--r--   0 runner    (1001) docker     (121)      360 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19439 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1719 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/deep_equals.py
--rw-r--r--   0 runner    (1001) docker     (121)   140076 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/expression.py
--rw-r--r--   0 runner    (1001) docker     (121)     7662 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/internal.py
--rw-r--r--   0 runner    (1001) docker     (121)     6619 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/module.py
--rw-r--r--   0 runner    (1001) docker     (121)    31193 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/op.py
--rw-r--r--   0 runner    (1001) docker     (121)   131699 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/statement.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.247846 libcst-0.4.8/libcst/_nodes/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10350 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     5132 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_assert.py
--rw-r--r--   0 runner    (1001) docker     (121)    16051 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_assign.py
--rw-r--r--   0 runner    (1001) docker     (121)    45724 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_atom.py
--rw-r--r--   0 runner    (1001) docker     (121)     2750 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_attribute.py
--rw-r--r--   0 runner    (1001) docker     (121)     7138 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_await.py
--rw-r--r--   0 runner    (1001) docker     (121)     6644 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_binary_op.py
--rw-r--r--   0 runner    (1001) docker     (121)     4286 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_boolean_op.py
--rw-r--r--   0 runner    (1001) docker     (121)    22698 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_call.py
--rw-r--r--   0 runner    (1001) docker     (121)    12963 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_classdef.py
--rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_comment.py
--rw-r--r--   0 runner    (1001) docker     (121)    13640 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_comparison.py
--rw-r--r--   0 runner    (1001) docker     (121)     7323 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_cst_node.py
--rw-r--r--   0 runner    (1001) docker     (121)     2555 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_del.py
--rw-r--r--   0 runner    (1001) docker     (121)     7133 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)     6013 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_dict_comp.py
--rw-r--r--   0 runner    (1001) docker     (121)     4077 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_docstring.py
--rw-r--r--   0 runner    (1001) docker     (121)     1053 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_else.py
--rw-r--r--   0 runner    (1001) docker     (121)     1286 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_empty_line.py
--rw-r--r--   0 runner    (1001) docker     (121)     2736 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_flatten_behavior.py
--rw-r--r--   0 runner    (1001) docker     (121)     7665 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_for.py
--rw-r--r--   0 runner    (1001) docker     (121)    93215 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_funcdef.py
--rw-r--r--   0 runner    (1001) docker     (121)     4780 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_global.py
--rw-r--r--   0 runner    (1001) docker     (121)     5299 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_if.py
--rw-r--r--   0 runner    (1001) docker     (121)     3727 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_ifexp.py
--rw-r--r--   0 runner    (1001) docker     (121)    29777 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (121)     5432 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_indented_block.py
--rw-r--r--   0 runner    (1001) docker     (121)    40077 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_lambda.py
--rw-r--r--   0 runner    (1001) docker     (121)      557 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_leaf_small_statements.py
--rw-r--r--   0 runner    (1001) docker     (121)     4695 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_list.py
--rw-r--r--   0 runner    (1001) docker     (121)    22302 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_match.py
--rw-r--r--   0 runner    (1001) docker     (121)     2366 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_matrix_multiply.py
--rw-r--r--   0 runner    (1001) docker     (121)     8290 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_module.py
--rw-r--r--   0 runner    (1001) docker     (121)     7750 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_namedexpr.py
--rw-r--r--   0 runner    (1001) docker     (121)     1027 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_newline.py
--rw-r--r--   0 runner    (1001) docker     (121)     4995 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_nonlocal.py
--rw-r--r--   0 runner    (1001) docker     (121)     4330 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_number.py
--rw-r--r--   0 runner    (1001) docker     (121)     7645 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_raise.py
--rw-r--r--   0 runner    (1001) docker     (121)     4031 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_removal_behavior.py
--rw-r--r--   0 runner    (1001) docker     (121)     3610 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_return.py
--rw-r--r--   0 runner    (1001) docker     (121)     4868 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_set.py
--rw-r--r--   0 runner    (1001) docker     (121)    20094 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_simple_comp.py
--rw-r--r--   0 runner    (1001) docker     (121)    13989 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_simple_statement.py
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_simple_string.py
--rw-r--r--   0 runner    (1001) docker     (121)     3827 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_simple_whitespace.py
--rw-r--r--   0 runner    (1001) docker     (121)     3037 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_small_statement.py
--rw-r--r--   0 runner    (1001) docker     (121)    16758 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_subscript.py
--rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_trailing_whitespace.py
--rw-r--r--   0 runner    (1001) docker     (121)    25792 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_try.py
--rw-r--r--   0 runner    (1001) docker     (121)    11237 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_tuple.py
--rw-r--r--   0 runner    (1001) docker     (121)     3210 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_unary_op.py
--rw-r--r--   0 runner    (1001) docker     (121)     5261 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_while.py
--rw-r--r--   0 runner    (1001) docker     (121)    13158 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_with.py
--rw-r--r--   0 runner    (1001) docker     (121)     8794 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/tests/test_yield.py
--rw-r--r--   0 runner    (1001) docker     (121)    11240 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_nodes/whitespace.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.247846 libcst-0.4.8/libcst/_parser/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8658 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/base_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.247846 libcst-0.4.8/libcst/_parser/conversions/
--rw-r--r--   0 runner    (1001) docker     (121)     8301 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/conversions/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/conversions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    53078 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/conversions/expression.py
--rw-r--r--   0 runner    (1001) docker     (121)     1726 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/conversions/module.py
--rw-r--r--   0 runner    (1001) docker     (121)    13365 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/conversions/params.py
--rw-r--r--   0 runner    (1001) docker     (121)    47301 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/conversions/statement.py
--rw-r--r--   0 runner    (1001) docker     (121)     2722 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/conversions/terminals.py
--rw-r--r--   0 runner    (1001) docker     (121)      622 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/custom_itertools.py
--rw-r--r--   0 runner    (1001) docker     (121)     7270 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/detect_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     5956 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/entrypoints.py
--rw-r--r--   0 runner    (1001) docker     (121)    12408 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/grammar.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.247846 libcst-0.4.8/libcst/_parser/parso/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/parso/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.247846 libcst-0.4.8/libcst/_parser/parso/pgen2/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/parso/pgen2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13727 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/parso/pgen2/generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     5887 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/parso/pgen2/grammar_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.247846 libcst-0.4.8/libcst/_parser/parso/python/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/parso/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1641 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/parso/python/py_token.py
--rw-r--r--   0 runner    (1001) docker     (121)     1384 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/parso/python/token.py
--rw-r--r--   0 runner    (1001) docker     (121)    44145 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/parso/python/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.247846 libcst-0.4.8/libcst/_parser/parso/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/parso/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1606 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/parso/tests/test_fstring.py
--rw-r--r--   0 runner    (1001) docker     (121)    14001 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/parso/tests/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (121)     2059 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/parso/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     7565 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/parso/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2083 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/production_decorator.py
--rw-r--r--   0 runner    (1001) docker     (121)     9370 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/py_whitespace_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     1807 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/python_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.251846 libcst-0.4.8/libcst/_parser/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1285 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (121)    14086 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/tests/test_detect_config.py
--rw-r--r--   0 runner    (1001) docker     (121)    10662 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/tests/test_footer_behavior.py
--rw-r--r--   0 runner    (1001) docker     (121)     1365 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/tests/test_node_identity.py
--rw-r--r--   0 runner    (1001) docker     (121)     6660 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/tests/test_parse_errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     1745 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/tests/test_version_compare.py
--rw-r--r--   0 runner    (1001) docker     (121)     9447 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/tests/test_whitespace_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    83462 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/tests/test_wrapped_tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.251846 libcst-0.4.8/libcst/_parser/types/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7020 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/types/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      568 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/types/conversions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3280 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/types/partials.py
--rw-r--r--   0 runner    (1001) docker     (121)      450 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/types/production.py
--rw-r--r--   0 runner    (1001) docker     (121)     1475 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/types/py_config.py
--rw-r--r--   0 runner    (1001) docker     (121)      885 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/types/py_token.py
--rw-r--r--   0 runner    (1001) docker     (121)     1396 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/types/py_whitespace_state.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.251846 libcst-0.4.8/libcst/_parser/types/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/types/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2212 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/types/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (121)      338 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/types/token.py
--rw-r--r--   0 runner    (1001) docker     (121)      427 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/types/whitespace_state.py
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/whitespace_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     8319 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_parser/wrapped_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (121)     1778 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_position.py
--rw-r--r--   0 runner    (1001) docker     (121)     1930 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_removal_sentinel.py
--rw-r--r--   0 runner    (1001) docker     (121)      794 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_tabs.py
--rw-r--r--   0 runner    (1001) docker     (121)     5975 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_type_enforce.py
--rw-r--r--   0 runner    (1001) docker     (121)   179734 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_typed_visitor.py
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_typed_visitor_base.py
--rw-r--r--   0 runner    (1001) docker     (121)      419 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_types.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-11-10 10:06:26.000000 libcst-0.4.8/libcst/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     6835 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/_visitors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.251846 libcst-0.4.8/libcst/codegen/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4714 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codegen/gather.py
--rw-r--r--   0 runner    (1001) docker     (121)    20436 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codegen/gen_matcher_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2332 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codegen/gen_type_mapping.py
--rw-r--r--   0 runner    (1001) docker     (121)     4459 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codegen/gen_visitor_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5810 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codegen/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.251846 libcst-0.4.8/libcst/codegen/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codegen/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4804 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codegen/tests/test_codegen_clean.py
--rw-r--r--   0 runner    (1001) docker     (121)     1887 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codegen/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.255846 libcst-0.4.8/libcst/codemod/
--rw-r--r--   0 runner    (1001) docker     (121)     1443 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24234 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     4916 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/_codemod.py
--rw-r--r--   0 runner    (1001) docker     (121)     8529 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/_command.py
--rw-r--r--   0 runner    (1001) docker     (121)     3167 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/_context.py
--rw-r--r--   0 runner    (1001) docker     (121)      989 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/_dummy_pool.py
--rw-r--r--   0 runner    (1001) docker     (121)     5467 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/_runner.py
--rw-r--r--   0 runner    (1001) docker     (121)     5850 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/_testing.py
--rw-r--r--   0 runner    (1001) docker     (121)     4958 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/_visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.259847 libcst-0.4.8/libcst/codemod/commands/
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1681 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/commands/add_pyre_directive.py
--rw-r--r--   0 runner    (1001) docker     (121)     4025 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/commands/add_trailing_commas.py
--rw-r--r--   0 runner    (1001) docker     (121)    16030 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/commands/convert_format_to_fstring.py
--rw-r--r--   0 runner    (1001) docker     (121)     2792 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/commands/convert_namedtuple_to_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (121)     5289 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/commands/convert_percent_format_to_fstring.py
--rw-r--r--   0 runner    (1001) docker     (121)    32682 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/commands/convert_type_comments.py
--rw-r--r--   0 runner    (1001) docker     (121)     1871 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/commands/ensure_import_present.py
--rw-r--r--   0 runner    (1001) docker     (121)     4133 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/commands/fix_pyre_directives.py
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/commands/noop.py
--rw-r--r--   0 runner    (1001) docker     (121)     1706 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/commands/remove_pyre_directive.py
--rw-r--r--   0 runner    (1001) docker     (121)     3404 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/commands/remove_unused_imports.py
--rw-r--r--   0 runner    (1001) docker     (121)    16562 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/commands/rename.py
--rw-r--r--   0 runner    (1001) docker     (121)     1966 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/commands/strip_strings_from_types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.259847 libcst-0.4.8/libcst/codemod/commands/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/commands/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3246 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/commands/tests/test_add_pyre_directive.py
--rw-r--r--   0 runner    (1001) docker     (121)     2102 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/commands/tests/test_add_trailing_commas.py
--rw-r--r--   0 runner    (1001) docker     (121)    11173 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/commands/tests/test_convert_format_to_fstring.py
--rw-r--r--   0 runner    (1001) docker     (121)     4504 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/commands/tests/test_convert_namedtuple_to_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (121)     2166 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/commands/tests/test_convert_percent_format_to_fstring.py
--rw-r--r--   0 runner    (1001) docker     (121)    13942 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/commands/tests/test_convert_type_comments.py
--rw-r--r--   0 runner    (1001) docker     (121)     1305 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/commands/tests/test_ensure_import_present.py
--rw-r--r--   0 runner    (1001) docker     (121)     5802 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/commands/tests/test_fix_pyre_directives.py
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/commands/tests/test_noop.py
--rw-r--r--   0 runner    (1001) docker     (121)     4650 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/commands/tests/test_remove_pyre_directive.py
--rw-r--r--   0 runner    (1001) docker     (121)     3271 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/commands/tests/test_remove_unused_imports.py
--rw-r--r--   0 runner    (1001) docker     (121)    15194 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/commands/tests/test_rename.py
--rw-r--r--   0 runner    (1001) docker     (121)     5813 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/commands/tests/test_strip_strings_from_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     1450 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/commands/tests/test_unnecessary_format_string.py
--rw-r--r--   0 runner    (1001) docker     (121)     1810 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/commands/unnecessary_format_string.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.259847 libcst-0.4.8/libcst/codemod/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/tests/codemod_formatter_error_input.py.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2553 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/tests/test_codemod.py
--rw-r--r--   0 runner    (1001) docker     (121)     1419 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/tests/test_codemod_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1629 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     3391 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/tests/test_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.263846 libcst-0.4.8/libcst/codemod/visitors/
--rw-r--r--   0 runner    (1001) docker     (121)     1290 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/visitors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17416 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/visitors/_add_imports.py
--rw-r--r--   0 runner    (1001) docker     (121)    53287 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/visitors/_apply_type_annotations.py
--rw-r--r--   0 runner    (1001) docker     (121)     2142 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/visitors/_gather_comments.py
--rw-r--r--   0 runner    (1001) docker     (121)     5821 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/visitors/_gather_exports.py
--rw-r--r--   0 runner    (1001) docker     (121)     2836 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/visitors/_gather_global_names.py
--rw-r--r--   0 runner    (1001) docker     (121)     6121 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/visitors/_gather_imports.py
--rw-r--r--   0 runner    (1001) docker     (121)     3574 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/visitors/_gather_string_annotation_names.py
--rw-r--r--   0 runner    (1001) docker     (121)     5642 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/visitors/_gather_unused_imports.py
--rw-r--r--   0 runner    (1001) docker     (121)     1630 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/visitors/_imports.py
--rw-r--r--   0 runner    (1001) docker     (121)    20494 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/visitors/_remove_imports.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.263846 libcst-0.4.8/libcst/codemod/visitors/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/visitors/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20692 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/visitors/tests/test_add_imports.py
--rw-r--r--   0 runner    (1001) docker     (121)    50145 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/visitors/tests/test_apply_type_annotations.py
--rw-r--r--   0 runner    (1001) docker     (121)     1625 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/visitors/tests/test_gather_comments.py
--rw-r--r--   0 runner    (1001) docker     (121)     4417 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/visitors/tests/test_gather_exports.py
--rw-r--r--   0 runner    (1001) docker     (121)     1886 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/visitors/tests/test_gather_global_names.py
--rw-r--r--   0 runner    (1001) docker     (121)     6031 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/visitors/tests/test_gather_imports.py
--rw-r--r--   0 runner    (1001) docker     (121)     2708 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/visitors/tests/test_gather_string_annotation_names.py
--rw-r--r--   0 runner    (1001) docker     (121)     3583 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/visitors/tests/test_gather_unused_imports.py
--rw-r--r--   0 runner    (1001) docker     (121)    23821 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/codemod/visitors/tests/test_remove_imports.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.263846 libcst-0.4.8/libcst/helpers/
--rw-r--r--   0 runner    (1001) docker     (121)     1395 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19403 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/helpers/_template.py
--rw-r--r--   0 runner    (1001) docker     (121)      956 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/helpers/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     1746 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/helpers/expression.py
--rw-r--r--   0 runner    (1001) docker     (121)     6029 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/helpers/module.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.263846 libcst-0.4.8/libcst/helpers/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/helpers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3507 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/helpers/tests/test_expression.py
--rw-r--r--   0 runner    (1001) docker     (121)    10497 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/helpers/tests/test_module.py
--rw-r--r--   0 runner    (1001) docker     (121)    11776 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/helpers/tests/test_template.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.263846 libcst-0.4.8/libcst/matchers/
--rw-r--r--   0 runner    (1001) docker     (121)   535179 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/matchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5130 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/matchers/_decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)    81853 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/matchers/_matcher_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     9718 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/matchers/_return_types.py
--rw-r--r--   0 runner    (1001) docker     (121)    35199 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/matchers/_visitors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.267847 libcst-0.4.8/libcst/matchers/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/matchers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    35418 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/matchers/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)    15761 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/matchers/tests/test_extract.py
--rw-r--r--   0 runner    (1001) docker     (121)     6721 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/matchers/tests/test_findall.py
--rw-r--r--   0 runner    (1001) docker     (121)    53908 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/matchers/tests/test_matchers.py
--rw-r--r--   0 runner    (1001) docker     (121)    23189 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/matchers/tests/test_matchers_with_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)    10927 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/matchers/tests/test_replace.py
--rw-r--r--   0 runner    (1001) docker     (121)    20190 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/matchers/tests/test_visitors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.267847 libcst-0.4.8/libcst/metadata/
--rw-r--r--   0 runner    (1001) docker     (121)     2497 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      546 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/metadata/accessor_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     5475 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/metadata/base_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     7825 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/metadata/expression_context_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     4733 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/metadata/full_repo_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     7363 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/metadata/name_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)      869 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/metadata/parent_node_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     4761 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/metadata/position_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     8391 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/metadata/reentrant_codegen.py
--rw-r--r--   0 runner    (1001) docker     (121)    46368 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/metadata/scope_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     3606 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/metadata/span_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.271847 libcst-0.4.8/libcst/metadata/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/metadata/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2018 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/metadata/tests/test_accessor_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     5639 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/metadata/tests/test_base_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)    14931 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/metadata/tests/test_expression_context_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     2783 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/metadata/tests/test_full_repo_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)    12198 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/metadata/tests/test_metadata_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     4160 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/metadata/tests/test_metadata_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)    19874 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/metadata/tests/test_name_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     1903 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/metadata/tests/test_parent_node_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     5923 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/metadata/tests/test_position_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     3852 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/metadata/tests/test_reentrant_codegen.py
--rw-r--r--   0 runner    (1001) docker     (121)    75819 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/metadata/tests/test_scope_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     3353 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/metadata/tests/test_span_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     3564 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/metadata/tests/test_type_inference_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     4633 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/metadata/type_inference_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     7575 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/metadata/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.271847 libcst-0.4.8/libcst/testing/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6107 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.271847 libcst-0.4.8/libcst/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.271847 libcst-0.4.8/libcst/tests/pyre/
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/tests/pyre/.pyre_configuration
--rw-r--r--   0 runner    (1001) docker     (121)     9703 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/tests/pyre/simple_class.json
--rw-r--r--   0 runner    (1001) docker     (121)      531 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/tests/pyre/simple_class.py
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/tests/test_add_slots.py
--rw-r--r--   0 runner    (1001) docker     (121)     2830 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/tests/test_batched_visitor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1646 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/tests/test_deep_clone.py
--rw-r--r--   0 runner    (1001) docker     (121)     4535 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/tests/test_deep_replace.py
--rw-r--r--   0 runner    (1001) docker     (121)     2524 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/tests/test_e2e.py
--rw-r--r--   0 runner    (1001) docker     (121)     2931 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     8102 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/tests/test_fuzz.py
--rw-r--r--   0 runner    (1001) docker     (121)     5193 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/tests/test_pyre_integration.py
--rw-r--r--   0 runner    (1001) docker     (121)      767 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/tests/test_tabs.py
--rw-r--r--   0 runner    (1001) docker     (121)    25336 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/tests/test_tool.py
--rw-r--r--   0 runner    (1001) docker     (121)     8028 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/tests/test_type_enforce.py
--rw-r--r--   0 runner    (1001) docker     (121)     3206 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/tests/test_visitor.py
--rw-r--r--   0 runner    (1001) docker     (121)    30607 2022-11-10 10:06:10.000000 libcst-0.4.8/libcst/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.235846 libcst-0.4.8/libcst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    11081 2022-11-10 10:06:26.000000 libcst-0.4.8/libcst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    15607 2022-11-10 10:06:26.000000 libcst-0.4.8/libcst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 10:06:26.000000 libcst-0.4.8/libcst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 10:06:26.000000 libcst-0.4.8/libcst.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-11-10 10:06:26.000000 libcst-0.4.8/libcst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-10 10:06:26.000000 libcst-0.4.8/libcst.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.271847 libcst-0.4.8/native/
--rw-r--r--   0 runner    (1001) docker     (121)    25856 2022-11-10 10:06:10.000000 libcst-0.4.8/native/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-11-10 10:06:10.000000 libcst-0.4.8/native/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.271847 libcst-0.4.8/native/libcst/
--rw-r--r--   0 runner    (1001) docker     (121)     1170 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (121)    32411 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/Grammar
--rw-r--r--   0 runner    (1001) docker     (121)     6453 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.271847 libcst-0.4.8/native/libcst/benches/
--rw-r--r--   0 runner    (1001) docker     (121)     3946 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/benches/parser_benchmark.rs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.271847 libcst-0.4.8/native/libcst/src/
--rw-r--r--   0 runner    (1001) docker     (121)      932 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/src/bin.rs
--rw-r--r--   0 runner    (1001) docker     (121)     5217 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.275847 libcst-0.4.8/native/libcst/src/nodes/
--rw-r--r--   0 runner    (1001) docker     (121)     1562 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/src/nodes/codegen.rs
--rw-r--r--   0 runner    (1001) docker     (121)    80125 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/src/nodes/expression.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/src/nodes/inflate_helpers.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1448 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/src/nodes/macros.rs
--rw-r--r--   0 runner    (1001) docker     (121)     7608 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/src/nodes/mod.rs
--rw-r--r--   0 runner    (1001) docker     (121)     2986 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/src/nodes/module.rs
--rw-r--r--   0 runner    (1001) docker     (121)    50731 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/src/nodes/op.rs
--rw-r--r--   0 runner    (1001) docker     (121)     4527 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/src/nodes/parser_config.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1588 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/src/nodes/py_cached.rs
--rw-r--r--   0 runner    (1001) docker     (121)   104571 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/src/nodes/statement.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/src/nodes/test_utils.rs
--rw-r--r--   0 runner    (1001) docker     (121)     5535 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/src/nodes/traits.rs
--rw-r--r--   0 runner    (1001) docker     (121)     4511 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/src/nodes/whitespace.rs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.275847 libcst-0.4.8/native/libcst/src/parser/
--rw-r--r--   0 runner    (1001) docker     (121)     3070 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/src/parser/errors.rs
--rw-r--r--   0 runner    (1001) docker     (121)   109918 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/src/parser/grammar.rs
--rw-r--r--   0 runner    (1001) docker     (121)      318 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/src/parser/mod.rs
--rw-r--r--   0 runner    (1001) docker     (121)     2232 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/src/parser/numbers.rs
--rw-r--r--   0 runner    (1001) docker     (121)      979 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/src/py.rs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.275847 libcst-0.4.8/native/libcst/src/tokenizer/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.275847 libcst-0.4.8/native/libcst/src/tokenizer/core/
--rw-r--r--   0 runner    (1001) docker     (121)     2403 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/src/tokenizer/core/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/src/tokenizer/core/README.md
--rw-r--r--   0 runner    (1001) docker     (121)    49640 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/src/tokenizer/core/mod.rs
--rw-r--r--   0 runner    (1001) docker     (121)     3179 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/src/tokenizer/core/string_types.rs
--rw-r--r--   0 runner    (1001) docker     (121)      502 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/src/tokenizer/debug_utils.rs
--rw-r--r--   0 runner    (1001) docker     (121)      321 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/src/tokenizer/mod.rs
--rw-r--r--   0 runner    (1001) docker     (121)     2607 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/src/tokenizer/operators.rs
--rw-r--r--   0 runner    (1001) docker     (121)    22036 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/src/tokenizer/tests.rs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.275847 libcst-0.4.8/native/libcst/src/tokenizer/text_position/
--rw-r--r--   0 runner    (1001) docker     (121)     9230 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/src/tokenizer/text_position/char_width.rs
--rw-r--r--   0 runner    (1001) docker     (121)    11761 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/src/tokenizer/text_position/mod.rs
--rw-r--r--   0 runner    (1001) docker     (121)    12813 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/src/tokenizer/whitespace_parser.rs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.275847 libcst-0.4.8/native/libcst/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.279847 libcst-0.4.8/native/libcst/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)     1059 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/tests/fixtures/big_binary_operator.py
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/tests/fixtures/class_craziness.py
--rw-r--r--   0 runner    (1001) docker     (121)     1991 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/tests/fixtures/comments.py
--rw-r--r--   0 runner    (1001) docker     (121)      471 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/tests/fixtures/comparisons.py
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/tests/fixtures/dangling_indent.py
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/tests/fixtures/decorated_function_without_body.py
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/tests/fixtures/dysfunctional_del.py
--rw-r--r--   0 runner    (1001) docker     (121)     9983 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/tests/fixtures/expr.py
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/tests/fixtures/expr_statement.py
--rw-r--r--   0 runner    (1001) docker     (121)     2000 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/tests/fixtures/fun_with_func_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/tests/fixtures/global_nonlocal.py
--rw-r--r--   0 runner    (1001) docker     (121)      416 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/tests/fixtures/import.py
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/tests/fixtures/indents_but_no_eol_before_eof.py
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/tests/fixtures/just_a_comment_without_nl.py
--rw-r--r--   0 runner    (1001) docker     (121)      896 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/tests/fixtures/malicious_match.py
--rw-r--r--   0 runner    (1001) docker     (121)      677 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/tests/fixtures/pep646.py
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/tests/fixtures/raise.py
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/tests/fixtures/smol_statements.py
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/tests/fixtures/spacious_spaces.py
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/tests/fixtures/starry_tries.py
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/tests/fixtures/suicidal_slices.py
--rw-r--r--   0 runner    (1001) docker     (121)      659 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/tests/fixtures/super_strings.py
--rw-r--r--   0 runner    (1001) docker     (121)      417 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/tests/fixtures/terrible_tries.py
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/tests/fixtures/trailing_comment_without_nl.py
--rw-r--r--   0 runner    (1001) docker     (121)      391 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/tests/fixtures/tuple_shenanigans.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/tests/fixtures/vast_emptiness.py
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/tests/fixtures/with_wickedness.py
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/tests/fixtures/wonky_walrus.py
--rw-r--r--   0 runner    (1001) docker     (121)     1641 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst/tests/parser_roundtrip.rs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.279847 libcst-0.4.8/native/libcst_derive/
--rw-r--r--   0 runner    (1001) docker     (121)      172 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst_derive/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.279847 libcst-0.4.8/native/libcst_derive/src/
--rw-r--r--   0 runner    (1001) docker     (121)     2196 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst_derive/src/codegen.rs
--rw-r--r--   0 runner    (1001) docker     (121)    13599 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst_derive/src/cstnode.rs
--rw-r--r--   0 runner    (1001) docker     (121)     2666 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst_derive/src/inflate.rs
--rw-r--r--   0 runner    (1001) docker     (121)     6748 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst_derive/src/into_py.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1564 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst_derive/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (121)     4174 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst_derive/src/parenthesized_node.rs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.223846 libcst-0.4.8/native/libcst_derive/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.279847 libcst-0.4.8/native/libcst_derive/tests/pass/
--rw-r--r--   0 runner    (1001) docker     (121)     3021 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst_derive/tests/pass/minimal_cst.rs
--rw-r--r--   0 runner    (1001) docker     (121)      907 2022-11-10 10:06:10.000000 libcst-0.4.8/native/libcst_derive/tests/pass/simple.rs
--rwxr-xr-x   0 runner    (1001) docker     (121)      270 2022-11-10 10:06:10.000000 libcst-0.4.8/native/roundtrip.sh
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-11-10 10:06:10.000000 libcst-0.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-11-10 10:06:10.000000 libcst-0.4.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-11-10 10:06:10.000000 libcst-0.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-10 10:06:26.279847 libcst-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2406 2022-11-10 10:06:10.000000 libcst-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.279847 libcst-0.4.8/stubs/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-11-10 10:06:10.000000 libcst-0.4.8/stubs/hypothesis.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-11-10 10:06:10.000000 libcst-0.4.8/stubs/hypothesmith.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.279847 libcst-0.4.8/stubs/libcst/
--rw-r--r--   0 runner    (1001) docker     (121)      426 2022-11-10 10:06:10.000000 libcst-0.4.8/stubs/libcst/native.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 10:06:26.279847 libcst-0.4.8/stubs/libcst_native/
--rw-r--r--   0 runner    (1001) docker     (121)     1146 2022-11-10 10:06:10.000000 libcst-0.4.8/stubs/libcst_native/parser_config.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      692 2022-11-10 10:06:10.000000 libcst-0.4.8/stubs/libcst_native/token_type.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      935 2022-11-10 10:06:10.000000 libcst-0.4.8/stubs/libcst_native/tokenize.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      973 2022-11-10 10:06:10.000000 libcst-0.4.8/stubs/libcst_native/whitespace_parser.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      556 2022-11-10 10:06:10.000000 libcst-0.4.8/stubs/libcst_native/whitespace_state.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-11-10 10:06:10.000000 libcst-0.4.8/stubs/setuptools.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1693 2022-11-10 10:06:10.000000 libcst-0.4.8/stubs/tokenize.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-11-10 10:06:10.000000 libcst-0.4.8/stubs/typing_inspect.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.894809 libcst-0.4.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.842809 libcst-0.4.9/.cargo/
+-rw-r--r--   0 runner    (1001) docker     (121)      223 2022-11-10 21:32:16.000000 libcst-0.4.9/.cargo/config.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      292 2022-11-10 21:32:16.000000 libcst-0.4.9/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (121)      231 2022-11-10 21:32:16.000000 libcst-0.4.9/.fixit.config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     5318 2022-11-10 21:32:16.000000 libcst-0.4.9/.flake8
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-11-10 21:32:16.000000 libcst-0.4.9/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.842809 libcst-0.4.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-11-10 21:32:16.000000 libcst-0.4.9/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (121)      526 2022-11-10 21:32:16.000000 libcst-0.4.9/.github/build-matrix.json
+-rw-r--r--   0 runner    (1001) docker     (121)      428 2022-11-10 21:32:16.000000 libcst-0.4.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.842809 libcst-0.4.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2910 2022-11-10 21:32:16.000000 libcst-0.4.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     6542 2022-11-10 21:32:16.000000 libcst-0.4.9/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1962 2022-11-10 21:32:16.000000 libcst-0.4.9/.github/workflows/pypi_upload.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      197 2022-11-10 21:32:16.000000 libcst-0.4.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      218 2022-11-10 21:32:16.000000 libcst-0.4.9/.pyre_configuration
+-rw-r--r--   0 runner    (1001) docker     (121)      311 2022-11-10 21:32:16.000000 libcst-0.4.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2022-11-10 21:32:16.000000 libcst-0.4.9/.watchmanconfig
+-rw-r--r--   0 runner    (1001) docker     (121)    32176 2022-11-10 21:32:16.000000 libcst-0.4.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)     3535 2022-11-10 21:32:16.000000 libcst-0.4.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1462 2022-11-10 21:32:16.000000 libcst-0.4.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)     4698 2022-11-10 21:32:16.000000 libcst-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2022-11-10 21:32:16.000000 libcst-0.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    11081 2022-11-10 21:32:33.894809 libcst-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    10297 2022-11-10 21:32:16.000000 libcst-0.4.9/README.rst
+-rwxr-xr-x   0 runner    (1001) docker     (121)      992 2022-11-10 21:32:16.000000 libcst-0.4.9/check_copyright.sh
+-rw-r--r--   0 runner    (1001) docker     (121)       51 2022-11-10 21:32:16.000000 libcst-0.4.9/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.834809 libcst-0.4.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.846809 libcst-0.4.9/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.846809 libcst-0.4.9/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)      385 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.850809 libcst-0.4.9/docs/source/_static/img/
+-rw-r--r--   0 runner    (1001) docker     (121)   108465 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/_static/img/python_scopes.png
+-rw-r--r--   0 runner    (1001) docker     (121)    30400 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/_static/img/python_scopes.svg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.850809 libcst-0.4.9/docs/source/_static/logo/
+-rw-r--r--   0 runner    (1001) docker     (121)     3638 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/_static/logo/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)     3629 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/_static/logo/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      676 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/_static/logo/favicon_16px.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1515 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/_static/logo/favicon_32px.png
+-rw-r--r--   0 runner    (1001) docker     (121)     4899 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/_static/logo/horizontal.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     4884 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/_static/logo/horizontal_white.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     8823 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/_static/logo/horizontal_white_sidebar.png
+-rw-r--r--   0 runner    (1001) docker     (121)     3336 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/_static/logo/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     3339 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/_static/logo/icon_white.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     4791 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/_static/logo/vertical.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     4776 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/_static/logo/vertical_white.svg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.850809 libcst-0.4.9/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (121)      346 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/_templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (121)     8658 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/best_practices.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     8085 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/codemods.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     8644 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/codemods_tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     9553 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      460 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/experimental.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/helpers.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1008 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     8876 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/matchers.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    13597 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/matchers_tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)     9920 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5347 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/metadata_tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)     3979 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/motivation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     9632 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/nodes.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1252 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/parser.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    10261 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/scope_tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)     9873 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)     5369 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/visitors.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    15454 2022-11-10 21:32:16.000000 libcst-0.4.9/docs/source/why_libcst.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.854809 libcst-0.4.9/libcst/
+-rw-r--r--   0 runner    (1001) docker     (121)     8492 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2911 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_add_slots.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5666 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_batched_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8017 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1618 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_flatten_sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2443 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_maybe_sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4832 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_metadata_dependent.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.858809 libcst-0.4.9/libcst/_nodes/
+-rw-r--r--   0 runner    (1001) docker     (121)      360 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19439 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1719 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/deep_equals.py
+-rw-r--r--   0 runner    (1001) docker     (121)   140076 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/expression.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7662 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/internal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6619 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/module.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31193 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/op.py
+-rw-r--r--   0 runner    (1001) docker     (121)   131699 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/statement.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.866809 libcst-0.4.9/libcst/_nodes/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10350 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5132 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_assert.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16051 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_assign.py
+-rw-r--r--   0 runner    (1001) docker     (121)    45724 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_atom.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2750 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7138 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_await.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6644 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_binary_op.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4286 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_boolean_op.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22698 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_call.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12963 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_classdef.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_comment.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13640 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7323 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_cst_node.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2555 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_del.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7133 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6013 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_dict_comp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4077 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1053 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_else.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1286 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_empty_line.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2736 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_flatten_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7665 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_for.py
+-rw-r--r--   0 runner    (1001) docker     (121)    93215 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_funcdef.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4780 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_global.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5299 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_if.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3727 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_ifexp.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29777 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5432 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_indented_block.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40077 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (121)      557 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_leaf_small_statements.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4695 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22302 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_match.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2366 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_matrix_multiply.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8290 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7750 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_namedexpr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1027 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_newline.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4995 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_nonlocal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4330 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_number.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7645 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_raise.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4031 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_removal_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3610 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_return.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4868 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_set.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20094 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_simple_comp.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13989 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_simple_statement.py
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_simple_string.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3827 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_simple_whitespace.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3037 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_small_statement.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16758 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_subscript.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_trailing_whitespace.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25792 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_try.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11237 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3210 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_unary_op.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5261 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_while.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13158 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_with.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8794 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/tests/test_yield.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11240 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_nodes/whitespace.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.866809 libcst-0.4.9/libcst/_parser/
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8658 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/base_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.870809 libcst-0.4.9/libcst/_parser/conversions/
+-rw-r--r--   0 runner    (1001) docker     (121)     8301 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/conversions/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/conversions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    53078 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/conversions/expression.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1726 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/conversions/module.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13365 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/conversions/params.py
+-rw-r--r--   0 runner    (1001) docker     (121)    47301 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/conversions/statement.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2722 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/conversions/terminals.py
+-rw-r--r--   0 runner    (1001) docker     (121)      622 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/custom_itertools.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7270 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/detect_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5956 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/entrypoints.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12408 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/grammar.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.870809 libcst-0.4.9/libcst/_parser/parso/
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/parso/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.870809 libcst-0.4.9/libcst/_parser/parso/pgen2/
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/parso/pgen2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13727 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/parso/pgen2/generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5887 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/parso/pgen2/grammar_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.870809 libcst-0.4.9/libcst/_parser/parso/python/
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/parso/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1641 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/parso/python/py_token.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1384 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/parso/python/token.py
+-rw-r--r--   0 runner    (1001) docker     (121)    44145 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/parso/python/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.870809 libcst-0.4.9/libcst/_parser/parso/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/parso/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1606 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/parso/tests/test_fstring.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14001 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/parso/tests/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2059 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/parso/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7565 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/parso/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2083 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/production_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9370 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/py_whitespace_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1807 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/python_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.870809 libcst-0.4.9/libcst/_parser/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1285 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14086 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/tests/test_detect_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10662 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/tests/test_footer_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1365 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/tests/test_node_identity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6660 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/tests/test_parse_errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1745 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/tests/test_version_compare.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9447 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/tests/test_whitespace_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)    83462 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/tests/test_wrapped_tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.870809 libcst-0.4.9/libcst/_parser/types/
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7020 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/types/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      568 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/types/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3280 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/types/partials.py
+-rw-r--r--   0 runner    (1001) docker     (121)      450 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/types/production.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1475 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/types/py_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      885 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/types/py_token.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1396 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/types/py_whitespace_state.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.870809 libcst-0.4.9/libcst/_parser/types/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/types/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2212 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/types/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      338 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/types/token.py
+-rw-r--r--   0 runner    (1001) docker     (121)      427 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/types/whitespace_state.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/whitespace_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8319 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_parser/wrapped_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1778 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_position.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1930 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_removal_sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (121)      794 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5975 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_type_enforce.py
+-rw-r--r--   0 runner    (1001) docker     (121)   179734 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_typed_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (121)      615 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_typed_visitor_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      419 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)      176 2022-11-10 21:32:33.000000 libcst-0.4.9/libcst/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6835 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/_visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.870809 libcst-0.4.9/libcst/codegen/
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4714 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codegen/gather.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20436 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codegen/gen_matcher_classes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2332 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codegen/gen_type_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4459 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codegen/gen_visitor_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5810 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codegen/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.874809 libcst-0.4.9/libcst/codegen/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codegen/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4804 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codegen/tests/test_codegen_clean.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1887 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codegen/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.874809 libcst-0.4.9/libcst/codemod/
+-rw-r--r--   0 runner    (1001) docker     (121)     1443 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24234 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4916 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/_codemod.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8529 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/_command.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3167 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/_context.py
+-rw-r--r--   0 runner    (1001) docker     (121)      989 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/_dummy_pool.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5467 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/_runner.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5850 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/_testing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4958 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/_visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.874809 libcst-0.4.9/libcst/codemod/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)      181 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1681 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/add_pyre_directive.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4025 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/add_trailing_commas.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16030 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/convert_format_to_fstring.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2792 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/convert_namedtuple_to_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5289 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/convert_percent_format_to_fstring.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32682 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/convert_type_comments.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1871 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/ensure_import_present.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4133 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/fix_pyre_directives.py
+-rw-r--r--   0 runner    (1001) docker     (121)      483 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/noop.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1706 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/remove_pyre_directive.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3404 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/remove_unused_imports.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16562 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/rename.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1966 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/strip_strings_from_types.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.878809 libcst-0.4.9/libcst/codemod/commands/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      181 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3246 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/tests/test_add_pyre_directive.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2102 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/tests/test_add_trailing_commas.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11173 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/tests/test_convert_format_to_fstring.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4504 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/tests/test_convert_namedtuple_to_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2166 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/tests/test_convert_percent_format_to_fstring.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13942 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/tests/test_convert_type_comments.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1305 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/tests/test_ensure_import_present.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5802 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/tests/test_fix_pyre_directives.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/tests/test_noop.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4650 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/tests/test_remove_pyre_directive.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3271 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/tests/test_remove_unused_imports.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15194 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/tests/test_rename.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5813 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/tests/test_strip_strings_from_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1450 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/tests/test_unnecessary_format_string.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1810 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/commands/unnecessary_format_string.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.878809 libcst-0.4.9/libcst/codemod/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      181 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      393 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/tests/codemod_formatter_error_input.py.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2553 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/tests/test_codemod.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1419 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/tests/test_codemod_cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1629 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3391 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/tests/test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.878809 libcst-0.4.9/libcst/codemod/visitors/
+-rw-r--r--   0 runner    (1001) docker     (121)     1290 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17416 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/_add_imports.py
+-rw-r--r--   0 runner    (1001) docker     (121)    53287 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/_apply_type_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2142 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/_gather_comments.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5821 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/_gather_exports.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2836 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/_gather_global_names.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6121 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/_gather_imports.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3574 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/_gather_string_annotation_names.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5642 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/_gather_unused_imports.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1630 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/_imports.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20494 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/_remove_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.878809 libcst-0.4.9/libcst/codemod/visitors/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      181 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20692 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/tests/test_add_imports.py
+-rw-r--r--   0 runner    (1001) docker     (121)    50145 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/tests/test_apply_type_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1625 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/tests/test_gather_comments.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4417 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/tests/test_gather_exports.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1886 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/tests/test_gather_global_names.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6031 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/tests/test_gather_imports.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2708 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/tests/test_gather_string_annotation_names.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3583 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/tests/test_gather_unused_imports.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23821 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/codemod/visitors/tests/test_remove_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.878809 libcst-0.4.9/libcst/helpers/
+-rw-r--r--   0 runner    (1001) docker     (121)     1395 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19403 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/helpers/_template.py
+-rw-r--r--   0 runner    (1001) docker     (121)      956 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/helpers/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1746 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/helpers/expression.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6029 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/helpers/module.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.878809 libcst-0.4.9/libcst/helpers/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/helpers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3507 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/helpers/tests/test_expression.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10497 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/helpers/tests/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11776 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/helpers/tests/test_template.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.882809 libcst-0.4.9/libcst/matchers/
+-rw-r--r--   0 runner    (1001) docker     (121)   535179 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/matchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5130 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/matchers/_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)    81853 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/matchers/_matcher_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9718 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/matchers/_return_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35199 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/matchers/_visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.882809 libcst-0.4.9/libcst/matchers/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/matchers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35418 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/matchers/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15761 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/matchers/tests/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6721 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/matchers/tests/test_findall.py
+-rw-r--r--   0 runner    (1001) docker     (121)    53908 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/matchers/tests/test_matchers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23189 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/matchers/tests/test_matchers_with_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10927 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/matchers/tests/test_replace.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20190 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/matchers/tests/test_visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.882809 libcst-0.4.9/libcst/metadata/
+-rw-r--r--   0 runner    (1001) docker     (121)     2497 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      546 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/accessor_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5475 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/base_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7825 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/expression_context_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4733 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/full_repo_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7363 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/name_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)      869 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/parent_node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4761 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/position_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8391 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/reentrant_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (121)    46368 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/scope_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3606 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/span_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.886809 libcst-0.4.9/libcst/metadata/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2018 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/tests/test_accessor_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5639 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/tests/test_base_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14931 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/tests/test_expression_context_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2783 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/tests/test_full_repo_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12198 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/tests/test_metadata_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4160 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/tests/test_metadata_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19874 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/tests/test_name_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1903 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/tests/test_parent_node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5923 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/tests/test_position_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3852 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/tests/test_reentrant_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (121)    75819 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/tests/test_scope_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3353 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/tests/test_span_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3564 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/tests/test_type_inference_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4633 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/type_inference_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7575 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/metadata/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.886809 libcst-0.4.9/libcst/testing/
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6107 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.886809 libcst-0.4.9/libcst/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.886809 libcst-0.4.9/libcst/tests/pyre/
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/tests/pyre/.pyre_configuration
+-rw-r--r--   0 runner    (1001) docker     (121)     9703 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/tests/pyre/simple_class.json
+-rw-r--r--   0 runner    (1001) docker     (121)      531 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/tests/pyre/simple_class.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/tests/test_add_slots.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2830 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/tests/test_batched_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1646 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/tests/test_deep_clone.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4535 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/tests/test_deep_replace.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2524 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/tests/test_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2931 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8102 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/tests/test_fuzz.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5193 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/tests/test_pyre_integration.py
+-rw-r--r--   0 runner    (1001) docker     (121)      767 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/tests/test_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25336 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/tests/test_tool.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8028 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/tests/test_type_enforce.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3206 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/tests/test_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30607 2022-11-10 21:32:16.000000 libcst-0.4.9/libcst/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.854809 libcst-0.4.9/libcst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    11081 2022-11-10 21:32:33.000000 libcst-0.4.9/libcst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    15607 2022-11-10 21:32:33.000000 libcst-0.4.9/libcst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 21:32:33.000000 libcst-0.4.9/libcst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 21:32:33.000000 libcst-0.4.9/libcst.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      482 2022-11-10 21:32:33.000000 libcst-0.4.9/libcst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-10 21:32:33.000000 libcst-0.4.9/libcst.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.886809 libcst-0.4.9/native/
+-rw-r--r--   0 runner    (1001) docker     (121)    25856 2022-11-10 21:32:16.000000 libcst-0.4.9/native/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2022-11-10 21:32:16.000000 libcst-0.4.9/native/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.886809 libcst-0.4.9/native/libcst/
+-rw-r--r--   0 runner    (1001) docker     (121)     1170 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (121)    32411 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/Grammar
+-rw-r--r--   0 runner    (1001) docker     (121)     6453 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.886809 libcst-0.4.9/native/libcst/benches/
+-rw-r--r--   0 runner    (1001) docker     (121)     3946 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/benches/parser_benchmark.rs
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.886809 libcst-0.4.9/native/libcst/src/
+-rw-r--r--   0 runner    (1001) docker     (121)      932 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/bin.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     5217 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.890809 libcst-0.4.9/native/libcst/src/nodes/
+-rw-r--r--   0 runner    (1001) docker     (121)     1562 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/nodes/codegen.rs
+-rw-r--r--   0 runner    (1001) docker     (121)    80125 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/nodes/expression.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/nodes/inflate_helpers.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1448 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/nodes/macros.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     7608 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/nodes/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     2986 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/nodes/module.rs
+-rw-r--r--   0 runner    (1001) docker     (121)    50731 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/nodes/op.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     4527 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/nodes/parser_config.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1588 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/nodes/py_cached.rs
+-rw-r--r--   0 runner    (1001) docker     (121)   104571 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/nodes/statement.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/nodes/test_utils.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     5535 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/nodes/traits.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     4511 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/nodes/whitespace.rs
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.890809 libcst-0.4.9/native/libcst/src/parser/
+-rw-r--r--   0 runner    (1001) docker     (121)     3070 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/parser/errors.rs
+-rw-r--r--   0 runner    (1001) docker     (121)   109918 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/parser/grammar.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      318 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/parser/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     2232 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/parser/numbers.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      979 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/py.rs
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.890809 libcst-0.4.9/native/libcst/src/tokenizer/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.890809 libcst-0.4.9/native/libcst/src/tokenizer/core/
+-rw-r--r--   0 runner    (1001) docker     (121)     2403 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/tokenizer/core/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/tokenizer/core/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)    49640 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/tokenizer/core/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     3179 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/tokenizer/core/string_types.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      502 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/tokenizer/debug_utils.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      321 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/tokenizer/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     2607 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/tokenizer/operators.rs
+-rw-r--r--   0 runner    (1001) docker     (121)    22036 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/tokenizer/tests.rs
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.890809 libcst-0.4.9/native/libcst/src/tokenizer/text_position/
+-rw-r--r--   0 runner    (1001) docker     (121)     9230 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/tokenizer/text_position/char_width.rs
+-rw-r--r--   0 runner    (1001) docker     (121)    11761 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/tokenizer/text_position/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (121)    12813 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/src/tokenizer/whitespace_parser.rs
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.890809 libcst-0.4.9/native/libcst/tests/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.894809 libcst-0.4.9/native/libcst/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (121)     1059 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/big_binary_operator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      376 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/class_craziness.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1991 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/comments.py
+-rw-r--r--   0 runner    (1001) docker     (121)      471 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/dangling_indent.py
+-rw-r--r--   0 runner    (1001) docker     (121)       36 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/decorated_function_without_body.py
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/dysfunctional_del.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9983 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/expr.py
+-rw-r--r--   0 runner    (1001) docker     (121)      145 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/expr_statement.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2000 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/fun_with_func_defs.py
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/global_nonlocal.py
+-rw-r--r--   0 runner    (1001) docker     (121)      416 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/import.py
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/indents_but_no_eol_before_eof.py
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/just_a_comment_without_nl.py
+-rw-r--r--   0 runner    (1001) docker     (121)      896 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/malicious_match.py
+-rw-r--r--   0 runner    (1001) docker     (121)      677 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/pep646.py
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/raise.py
+-rw-r--r--   0 runner    (1001) docker     (121)      110 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/smol_statements.py
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/spacious_spaces.py
+-rw-r--r--   0 runner    (1001) docker     (121)      386 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/starry_tries.py
+-rw-r--r--   0 runner    (1001) docker     (121)      424 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/suicidal_slices.py
+-rw-r--r--   0 runner    (1001) docker     (121)      659 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/super_strings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      417 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/terrible_tries.py
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/trailing_comment_without_nl.py
+-rw-r--r--   0 runner    (1001) docker     (121)      391 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/tuple_shenanigans.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/vast_emptiness.py
+-rw-r--r--   0 runner    (1001) docker     (121)      210 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/with_wickedness.py
+-rw-r--r--   0 runner    (1001) docker     (121)      192 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/fixtures/wonky_walrus.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1641 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst/tests/parser_roundtrip.rs
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.894809 libcst-0.4.9/native/libcst_derive/
+-rw-r--r--   0 runner    (1001) docker     (121)      172 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst_derive/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.894809 libcst-0.4.9/native/libcst_derive/src/
+-rw-r--r--   0 runner    (1001) docker     (121)     2196 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst_derive/src/codegen.rs
+-rw-r--r--   0 runner    (1001) docker     (121)    13599 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst_derive/src/cstnode.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     2666 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst_derive/src/inflate.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     6748 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst_derive/src/into_py.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1564 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst_derive/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     4174 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst_derive/src/parenthesized_node.rs
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.838809 libcst-0.4.9/native/libcst_derive/tests/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.894809 libcst-0.4.9/native/libcst_derive/tests/pass/
+-rw-r--r--   0 runner    (1001) docker     (121)     3021 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst_derive/tests/pass/minimal_cst.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      907 2022-11-10 21:32:16.000000 libcst-0.4.9/native/libcst_derive/tests/pass/simple.rs
+-rwxr-xr-x   0 runner    (1001) docker     (121)      270 2022-11-10 21:32:16.000000 libcst-0.4.9/native/roundtrip.sh
+-rw-r--r--   0 runner    (1001) docker     (121)      397 2022-11-10 21:32:16.000000 libcst-0.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      362 2022-11-10 21:32:16.000000 libcst-0.4.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-11-10 21:32:16.000000 libcst-0.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-10 21:32:33.894809 libcst-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2406 2022-11-10 21:32:16.000000 libcst-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.894809 libcst-0.4.9/stubs/
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-11-10 21:32:16.000000 libcst-0.4.9/stubs/hypothesis.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-11-10 21:32:16.000000 libcst-0.4.9/stubs/hypothesmith.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.894809 libcst-0.4.9/stubs/libcst/
+-rw-r--r--   0 runner    (1001) docker     (121)      426 2022-11-10 21:32:16.000000 libcst-0.4.9/stubs/libcst/native.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 21:32:33.894809 libcst-0.4.9/stubs/libcst_native/
+-rw-r--r--   0 runner    (1001) docker     (121)     1146 2022-11-10 21:32:16.000000 libcst-0.4.9/stubs/libcst_native/parser_config.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      692 2022-11-10 21:32:16.000000 libcst-0.4.9/stubs/libcst_native/token_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      935 2022-11-10 21:32:16.000000 libcst-0.4.9/stubs/libcst_native/tokenize.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      973 2022-11-10 21:32:16.000000 libcst-0.4.9/stubs/libcst_native/whitespace_parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      556 2022-11-10 21:32:16.000000 libcst-0.4.9/stubs/libcst_native/whitespace_state.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-11-10 21:32:16.000000 libcst-0.4.9/stubs/setuptools.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1693 2022-11-10 21:32:16.000000 libcst-0.4.9/stubs/tokenize.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-11-10 21:32:16.000000 libcst-0.4.9/stubs/typing_inspect.pyi
```

### Comparing `libcst-0.4.8/.flake8` & `libcst-0.4.9/.flake8`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/.github/build-matrix.json` & `libcst-0.4.9/.github/build-matrix.json`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/.github/workflows/build.yml` & `libcst-0.4.9/.github/workflows/build.yml`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
       - id: set-matrix
         # match github.ref to the on_ref_regex field in the json
         # to skip running linux/aarch64 builds on PRs
         run: |
           matrix=$(jq --arg ref "${{ github.ref }}" \
             'map(select(.on_ref_regex as $pat | $pat == null or ($ref | test($pat))) | del(.on_ref_regex))' \
             .github/build-matrix.json)
-          echo ::set-output name=matrix::{\"include\":$(echo $matrix)}\"
+          echo matrix={\"include\":$(echo $matrix)}\" >> $GITHUB_OUTPUT
 
   build:
     name: Build wheels on ${{ join(matrix.os, '/') }}/${{ matrix.vers }}
     needs: build_matrix
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
@@ -57,11 +57,11 @@
           working-directory: native
       - name: Disable scmtools local scheme
         if: ${{ github.event_name == 'push' && github.ref == 'refs/heads/main' }}
         run: >-
           echo LIBCST_NO_LOCAL_SCHEME=1 >> $GITHUB_ENV
       - name: Build wheels
         uses: pypa/cibuildwheel@v2.11.2
-      - uses: actions/upload-artifact@v2
+      - uses: actions/upload-artifact@v3
         with:
           path: wheelhouse/*.whl
           name: wheels
```

### Comparing `libcst-0.4.8/.github/workflows/ci.yml` & `libcst-0.4.9/.github/workflows/ci.yml`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
           coverage xml -i
       - uses: codecov/codecov-action@v2
         with:
           files: coverage.xml
           fail_ci_if_error: true
           verbose: true
       - name: Archive Coverage
-        uses: actions/upload-artifact@v2
+        uses: actions/upload-artifact@v3
         with:
           name: coverage
           path: coverage.xml
 
   # Build the docs
   docs:
     runs-on: ubuntu-latest
@@ -143,15 +143,15 @@
       - name: Install Dependencies
         if: steps.cache.outputs.cache-hit != 'true'
         run: |
           pip install --upgrade --upgrade-strategy eager build -r requirements.txt -r requirements-dev.txt
       - uses: ts-graphviz/setup-graphviz@v1
       - run: sphinx-build docs/source/ docs/build/
       - name: Archive Docs
-        uses: actions/upload-artifact@v2
+        uses: actions/upload-artifact@v3
         with:
           name: sphinx-docs
           path: docs/build
 
   # Test rust parts
   native:
     name: Rust unit tests
```

### Comparing `libcst-0.4.8/.github/workflows/pypi_upload.yml` & `libcst-0.4.9/.github/workflows/pypi_upload.yml`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/CHANGELOG.md` & `libcst-0.4.9/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/CODE_OF_CONDUCT.md` & `libcst-0.4.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/CONTRIBUTING.md` & `libcst-0.4.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/LICENSE` & `libcst-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/PKG-INFO` & `libcst-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libcst
-Version: 0.4.8
+Version: 0.4.9
 Summary: A concrete syntax tree with AST-like properties for Python 3.5, 3.6, 3.7, 3.8, 3.9, and 3.10 programs.
 Home-page: https://github.com/Instagram/LibCST
 License: MIT
 Project-URL: Changelog, https://github.com/Instagram/LibCST/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://libcst.readthedocs.io/en/latest/
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `libcst-0.4.8/README.rst` & `libcst-0.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/check_copyright.sh` & `libcst-0.4.9/check_copyright.sh`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/docs/source/_static/img/python_scopes.png` & `libcst-0.4.9/docs/source/_static/img/python_scopes.png`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/docs/source/_static/img/python_scopes.svg` & `libcst-0.4.9/docs/source/_static/img/python_scopes.svg`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/docs/source/_static/logo/favicon.ico` & `libcst-0.4.9/docs/source/_static/logo/favicon.ico`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/docs/source/_static/logo/favicon.svg` & `libcst-0.4.9/docs/source/_static/logo/favicon.svg`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/docs/source/_static/logo/favicon_16px.png` & `libcst-0.4.9/docs/source/_static/logo/favicon_16px.png`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/docs/source/_static/logo/favicon_32px.png` & `libcst-0.4.9/docs/source/_static/logo/favicon_32px.png`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/docs/source/_static/logo/horizontal.svg` & `libcst-0.4.9/docs/source/_static/logo/horizontal.svg`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/docs/source/_static/logo/horizontal_white.svg` & `libcst-0.4.9/docs/source/_static/logo/horizontal_white.svg`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/docs/source/_static/logo/horizontal_white_sidebar.png` & `libcst-0.4.9/docs/source/_static/logo/horizontal_white_sidebar.png`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/docs/source/_static/logo/icon.svg` & `libcst-0.4.9/docs/source/_static/logo/icon.svg`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/docs/source/_static/logo/icon_white.svg` & `libcst-0.4.9/docs/source/_static/logo/icon_white.svg`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/docs/source/_static/logo/vertical.svg` & `libcst-0.4.9/docs/source/_static/logo/vertical.svg`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/docs/source/_static/logo/vertical_white.svg` & `libcst-0.4.9/docs/source/_static/logo/vertical_white.svg`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/docs/source/best_practices.rst` & `libcst-0.4.9/docs/source/best_practices.rst`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/docs/source/codemods.rst` & `libcst-0.4.9/docs/source/codemods.rst`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/docs/source/codemods_tutorial.rst` & `libcst-0.4.9/docs/source/codemods_tutorial.rst`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/docs/source/conf.py` & `libcst-0.4.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/docs/source/helpers.rst` & `libcst-0.4.9/docs/source/helpers.rst`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/docs/source/index.rst` & `libcst-0.4.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/docs/source/matchers.rst` & `libcst-0.4.9/docs/source/matchers.rst`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/docs/source/matchers_tutorial.ipynb` & `libcst-0.4.9/docs/source/matchers_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/docs/source/metadata.rst` & `libcst-0.4.9/docs/source/metadata.rst`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/docs/source/metadata_tutorial.ipynb` & `libcst-0.4.9/docs/source/metadata_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/docs/source/motivation.rst` & `libcst-0.4.9/docs/source/motivation.rst`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/docs/source/nodes.rst` & `libcst-0.4.9/docs/source/nodes.rst`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/docs/source/parser.rst` & `libcst-0.4.9/docs/source/parser.rst`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/docs/source/scope_tutorial.ipynb` & `libcst-0.4.9/docs/source/scope_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/docs/source/tutorial.ipynb` & `libcst-0.4.9/docs/source/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/docs/source/visitors.rst` & `libcst-0.4.9/docs/source/visitors.rst`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/docs/source/why_libcst.rst` & `libcst-0.4.9/docs/source/why_libcst.rst`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/__init__.py` & `libcst-0.4.9/libcst/__init__.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_add_slots.py` & `libcst-0.4.9/libcst/_add_slots.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_batched_visitor.py` & `libcst-0.4.9/libcst/_batched_visitor.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_exceptions.py` & `libcst-0.4.9/libcst/_exceptions.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_flatten_sentinel.py` & `libcst-0.4.9/libcst/_flatten_sentinel.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_maybe_sentinel.py` & `libcst-0.4.9/libcst/_maybe_sentinel.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_metadata_dependent.py` & `libcst-0.4.9/libcst/_metadata_dependent.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/base.py` & `libcst-0.4.9/libcst/_nodes/base.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/deep_equals.py` & `libcst-0.4.9/libcst/_nodes/deep_equals.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/expression.py` & `libcst-0.4.9/libcst/_nodes/expression.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/internal.py` & `libcst-0.4.9/libcst/_nodes/internal.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/module.py` & `libcst-0.4.9/libcst/_nodes/module.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/op.py` & `libcst-0.4.9/libcst/_nodes/op.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/statement.py` & `libcst-0.4.9/libcst/_nodes/statement.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/base.py` & `libcst-0.4.9/libcst/_nodes/tests/base.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_assert.py` & `libcst-0.4.9/libcst/_nodes/tests/test_assert.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_assign.py` & `libcst-0.4.9/libcst/_nodes/tests/test_assign.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_atom.py` & `libcst-0.4.9/libcst/_nodes/tests/test_atom.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_attribute.py` & `libcst-0.4.9/libcst/_nodes/tests/test_attribute.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_await.py` & `libcst-0.4.9/libcst/_nodes/tests/test_await.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_binary_op.py` & `libcst-0.4.9/libcst/_nodes/tests/test_binary_op.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_boolean_op.py` & `libcst-0.4.9/libcst/_nodes/tests/test_boolean_op.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_call.py` & `libcst-0.4.9/libcst/_nodes/tests/test_call.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_classdef.py` & `libcst-0.4.9/libcst/_nodes/tests/test_classdef.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_comment.py` & `libcst-0.4.9/libcst/_nodes/tests/test_comment.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_comparison.py` & `libcst-0.4.9/libcst/_nodes/tests/test_comparison.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_cst_node.py` & `libcst-0.4.9/libcst/_nodes/tests/test_cst_node.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_del.py` & `libcst-0.4.9/libcst/_nodes/tests/test_del.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_dict.py` & `libcst-0.4.9/libcst/_nodes/tests/test_dict.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_dict_comp.py` & `libcst-0.4.9/libcst/_nodes/tests/test_dict_comp.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_docstring.py` & `libcst-0.4.9/libcst/_nodes/tests/test_docstring.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_else.py` & `libcst-0.4.9/libcst/_nodes/tests/test_else.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_empty_line.py` & `libcst-0.4.9/libcst/_nodes/tests/test_empty_line.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_flatten_behavior.py` & `libcst-0.4.9/libcst/_nodes/tests/test_flatten_behavior.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_for.py` & `libcst-0.4.9/libcst/_nodes/tests/test_for.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_funcdef.py` & `libcst-0.4.9/libcst/_nodes/tests/test_funcdef.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_global.py` & `libcst-0.4.9/libcst/_nodes/tests/test_global.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_if.py` & `libcst-0.4.9/libcst/_nodes/tests/test_if.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_ifexp.py` & `libcst-0.4.9/libcst/_nodes/tests/test_ifexp.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_import.py` & `libcst-0.4.9/libcst/_nodes/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_indented_block.py` & `libcst-0.4.9/libcst/_nodes/tests/test_indented_block.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_lambda.py` & `libcst-0.4.9/libcst/_nodes/tests/test_lambda.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_leaf_small_statements.py` & `libcst-0.4.9/libcst/_nodes/tests/test_leaf_small_statements.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_list.py` & `libcst-0.4.9/libcst/_nodes/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_match.py` & `libcst-0.4.9/libcst/_nodes/tests/test_match.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_matrix_multiply.py` & `libcst-0.4.9/libcst/_nodes/tests/test_matrix_multiply.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_module.py` & `libcst-0.4.9/libcst/_nodes/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_namedexpr.py` & `libcst-0.4.9/libcst/_nodes/tests/test_namedexpr.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_newline.py` & `libcst-0.4.9/libcst/_nodes/tests/test_newline.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_nonlocal.py` & `libcst-0.4.9/libcst/_nodes/tests/test_nonlocal.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_number.py` & `libcst-0.4.9/libcst/_nodes/tests/test_number.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_raise.py` & `libcst-0.4.9/libcst/_nodes/tests/test_raise.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_removal_behavior.py` & `libcst-0.4.9/libcst/_nodes/tests/test_removal_behavior.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_return.py` & `libcst-0.4.9/libcst/_nodes/tests/test_return.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_set.py` & `libcst-0.4.9/libcst/_nodes/tests/test_set.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_simple_comp.py` & `libcst-0.4.9/libcst/_nodes/tests/test_simple_comp.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_simple_statement.py` & `libcst-0.4.9/libcst/_nodes/tests/test_simple_statement.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_simple_string.py` & `libcst-0.4.9/libcst/_nodes/tests/test_simple_string.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_simple_whitespace.py` & `libcst-0.4.9/libcst/_nodes/tests/test_simple_whitespace.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_small_statement.py` & `libcst-0.4.9/libcst/_nodes/tests/test_small_statement.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_subscript.py` & `libcst-0.4.9/libcst/_nodes/tests/test_subscript.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_trailing_whitespace.py` & `libcst-0.4.9/libcst/_nodes/tests/test_trailing_whitespace.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_try.py` & `libcst-0.4.9/libcst/_nodes/tests/test_try.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_tuple.py` & `libcst-0.4.9/libcst/_nodes/tests/test_tuple.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_unary_op.py` & `libcst-0.4.9/libcst/_nodes/tests/test_unary_op.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_while.py` & `libcst-0.4.9/libcst/_nodes/tests/test_while.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_with.py` & `libcst-0.4.9/libcst/_nodes/tests/test_with.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/tests/test_yield.py` & `libcst-0.4.9/libcst/_nodes/tests/test_yield.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_nodes/whitespace.py` & `libcst-0.4.9/libcst/_nodes/whitespace.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/base_parser.py` & `libcst-0.4.9/libcst/_parser/base_parser.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/conversions/README.md` & `libcst-0.4.9/libcst/_parser/conversions/README.md`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/conversions/expression.py` & `libcst-0.4.9/libcst/_parser/conversions/expression.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/conversions/module.py` & `libcst-0.4.9/libcst/_parser/conversions/module.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/conversions/params.py` & `libcst-0.4.9/libcst/_parser/conversions/params.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/conversions/statement.py` & `libcst-0.4.9/libcst/_parser/conversions/statement.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/conversions/terminals.py` & `libcst-0.4.9/libcst/_parser/conversions/terminals.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/custom_itertools.py` & `libcst-0.4.9/libcst/_parser/custom_itertools.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/detect_config.py` & `libcst-0.4.9/libcst/_parser/detect_config.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/entrypoints.py` & `libcst-0.4.9/libcst/_parser/entrypoints.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/grammar.py` & `libcst-0.4.9/libcst/_parser/grammar.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/parso/pgen2/generator.py` & `libcst-0.4.9/libcst/_parser/parso/pgen2/generator.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/parso/pgen2/grammar_parser.py` & `libcst-0.4.9/libcst/_parser/parso/pgen2/grammar_parser.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/parso/python/py_token.py` & `libcst-0.4.9/libcst/_parser/parso/python/py_token.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/parso/python/token.py` & `libcst-0.4.9/libcst/_parser/parso/python/token.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/parso/python/tokenize.py` & `libcst-0.4.9/libcst/_parser/parso/python/tokenize.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/parso/tests/test_fstring.py` & `libcst-0.4.9/libcst/_parser/parso/tests/test_fstring.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/parso/tests/test_tokenize.py` & `libcst-0.4.9/libcst/_parser/parso/tests/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/parso/tests/test_utils.py` & `libcst-0.4.9/libcst/_parser/parso/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/parso/utils.py` & `libcst-0.4.9/libcst/_parser/parso/utils.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/production_decorator.py` & `libcst-0.4.9/libcst/_parser/production_decorator.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/py_whitespace_parser.py` & `libcst-0.4.9/libcst/_parser/py_whitespace_parser.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/python_parser.py` & `libcst-0.4.9/libcst/_parser/python_parser.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/tests/test_config.py` & `libcst-0.4.9/libcst/_parser/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/tests/test_detect_config.py` & `libcst-0.4.9/libcst/_parser/tests/test_detect_config.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/tests/test_footer_behavior.py` & `libcst-0.4.9/libcst/_parser/tests/test_footer_behavior.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/tests/test_node_identity.py` & `libcst-0.4.9/libcst/_parser/tests/test_node_identity.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/tests/test_parse_errors.py` & `libcst-0.4.9/libcst/_parser/tests/test_parse_errors.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/tests/test_version_compare.py` & `libcst-0.4.9/libcst/_parser/tests/test_version_compare.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/tests/test_whitespace_parser.py` & `libcst-0.4.9/libcst/_parser/tests/test_whitespace_parser.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/tests/test_wrapped_tokenize.py` & `libcst-0.4.9/libcst/_parser/tests/test_wrapped_tokenize.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/types/config.py` & `libcst-0.4.9/libcst/_parser/types/config.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/types/conversions.py` & `libcst-0.4.9/libcst/_parser/types/conversions.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/types/partials.py` & `libcst-0.4.9/libcst/_parser/types/partials.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/types/py_config.py` & `libcst-0.4.9/libcst/_parser/types/py_config.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/types/py_token.py` & `libcst-0.4.9/libcst/_parser/types/py_token.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/types/py_whitespace_state.py` & `libcst-0.4.9/libcst/_parser/types/py_whitespace_state.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/types/tests/test_config.py` & `libcst-0.4.9/libcst/_parser/types/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/whitespace_parser.py` & `libcst-0.4.9/libcst/_parser/whitespace_parser.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_parser/wrapped_tokenize.py` & `libcst-0.4.9/libcst/_parser/wrapped_tokenize.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_position.py` & `libcst-0.4.9/libcst/_position.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_removal_sentinel.py` & `libcst-0.4.9/libcst/_removal_sentinel.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_tabs.py` & `libcst-0.4.9/libcst/_tabs.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_type_enforce.py` & `libcst-0.4.9/libcst/_type_enforce.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_typed_visitor.py` & `libcst-0.4.9/libcst/_typed_visitor.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_typed_visitor_base.py` & `libcst-0.4.9/libcst/_typed_visitor_base.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/_visitors.py` & `libcst-0.4.9/libcst/_visitors.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codegen/gather.py` & `libcst-0.4.9/libcst/codegen/gather.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codegen/gen_matcher_classes.py` & `libcst-0.4.9/libcst/codegen/gen_matcher_classes.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codegen/gen_type_mapping.py` & `libcst-0.4.9/libcst/codegen/gen_type_mapping.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codegen/gen_visitor_functions.py` & `libcst-0.4.9/libcst/codegen/gen_visitor_functions.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codegen/generate.py` & `libcst-0.4.9/libcst/codegen/generate.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codegen/tests/test_codegen_clean.py` & `libcst-0.4.9/libcst/codegen/tests/test_codegen_clean.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codegen/transforms.py` & `libcst-0.4.9/libcst/codegen/transforms.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/__init__.py` & `libcst-0.4.9/libcst/codemod/__init__.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/_cli.py` & `libcst-0.4.9/libcst/codemod/_cli.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/_codemod.py` & `libcst-0.4.9/libcst/codemod/_codemod.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/_command.py` & `libcst-0.4.9/libcst/codemod/_command.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/_context.py` & `libcst-0.4.9/libcst/codemod/_context.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/_dummy_pool.py` & `libcst-0.4.9/libcst/codemod/_dummy_pool.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/_runner.py` & `libcst-0.4.9/libcst/codemod/_runner.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/_testing.py` & `libcst-0.4.9/libcst/codemod/_testing.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/_visitor.py` & `libcst-0.4.9/libcst/codemod/_visitor.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/commands/add_pyre_directive.py` & `libcst-0.4.9/libcst/codemod/commands/add_pyre_directive.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/commands/add_trailing_commas.py` & `libcst-0.4.9/libcst/codemod/commands/add_trailing_commas.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/commands/convert_format_to_fstring.py` & `libcst-0.4.9/libcst/codemod/commands/convert_format_to_fstring.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/commands/convert_namedtuple_to_dataclass.py` & `libcst-0.4.9/libcst/codemod/commands/convert_namedtuple_to_dataclass.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/commands/convert_percent_format_to_fstring.py` & `libcst-0.4.9/libcst/codemod/commands/convert_percent_format_to_fstring.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/commands/convert_type_comments.py` & `libcst-0.4.9/libcst/codemod/commands/convert_type_comments.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/commands/ensure_import_present.py` & `libcst-0.4.9/libcst/codemod/commands/ensure_import_present.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/commands/fix_pyre_directives.py` & `libcst-0.4.9/libcst/codemod/commands/fix_pyre_directives.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/commands/remove_pyre_directive.py` & `libcst-0.4.9/libcst/codemod/commands/remove_pyre_directive.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/commands/remove_unused_imports.py` & `libcst-0.4.9/libcst/codemod/commands/remove_unused_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/commands/rename.py` & `libcst-0.4.9/libcst/codemod/commands/rename.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/commands/strip_strings_from_types.py` & `libcst-0.4.9/libcst/codemod/commands/strip_strings_from_types.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/commands/tests/test_add_pyre_directive.py` & `libcst-0.4.9/libcst/codemod/commands/tests/test_add_pyre_directive.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/commands/tests/test_add_trailing_commas.py` & `libcst-0.4.9/libcst/codemod/commands/tests/test_add_trailing_commas.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/commands/tests/test_convert_format_to_fstring.py` & `libcst-0.4.9/libcst/codemod/commands/tests/test_convert_format_to_fstring.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/commands/tests/test_convert_namedtuple_to_dataclass.py` & `libcst-0.4.9/libcst/codemod/commands/tests/test_convert_namedtuple_to_dataclass.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/commands/tests/test_convert_percent_format_to_fstring.py` & `libcst-0.4.9/libcst/codemod/commands/tests/test_convert_percent_format_to_fstring.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/commands/tests/test_convert_type_comments.py` & `libcst-0.4.9/libcst/codemod/commands/tests/test_convert_type_comments.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/commands/tests/test_ensure_import_present.py` & `libcst-0.4.9/libcst/codemod/commands/tests/test_ensure_import_present.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/commands/tests/test_fix_pyre_directives.py` & `libcst-0.4.9/libcst/codemod/commands/tests/test_fix_pyre_directives.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/commands/tests/test_noop.py` & `libcst-0.4.9/libcst/codemod/commands/tests/test_noop.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/commands/tests/test_remove_pyre_directive.py` & `libcst-0.4.9/libcst/codemod/commands/tests/test_remove_pyre_directive.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/commands/tests/test_remove_unused_imports.py` & `libcst-0.4.9/libcst/codemod/commands/tests/test_remove_unused_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/commands/tests/test_rename.py` & `libcst-0.4.9/libcst/codemod/commands/tests/test_rename.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/commands/tests/test_strip_strings_from_types.py` & `libcst-0.4.9/libcst/codemod/commands/tests/test_strip_strings_from_types.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/commands/tests/test_unnecessary_format_string.py` & `libcst-0.4.9/libcst/codemod/commands/tests/test_unnecessary_format_string.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/commands/unnecessary_format_string.py` & `libcst-0.4.9/libcst/codemod/commands/unnecessary_format_string.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/tests/test_codemod.py` & `libcst-0.4.9/libcst/codemod/tests/test_codemod.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/tests/test_codemod_cli.py` & `libcst-0.4.9/libcst/codemod/tests/test_codemod_cli.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/tests/test_metadata.py` & `libcst-0.4.9/libcst/codemod/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/tests/test_runner.py` & `libcst-0.4.9/libcst/codemod/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/visitors/__init__.py` & `libcst-0.4.9/libcst/codemod/visitors/__init__.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/visitors/_add_imports.py` & `libcst-0.4.9/libcst/codemod/visitors/_add_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/visitors/_apply_type_annotations.py` & `libcst-0.4.9/libcst/codemod/visitors/_apply_type_annotations.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/visitors/_gather_comments.py` & `libcst-0.4.9/libcst/codemod/visitors/_gather_comments.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/visitors/_gather_exports.py` & `libcst-0.4.9/libcst/codemod/visitors/_gather_exports.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/visitors/_gather_global_names.py` & `libcst-0.4.9/libcst/codemod/visitors/_gather_global_names.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/visitors/_gather_imports.py` & `libcst-0.4.9/libcst/codemod/visitors/_gather_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/visitors/_gather_string_annotation_names.py` & `libcst-0.4.9/libcst/codemod/visitors/_gather_string_annotation_names.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/visitors/_gather_unused_imports.py` & `libcst-0.4.9/libcst/codemod/visitors/_gather_unused_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/visitors/_imports.py` & `libcst-0.4.9/libcst/codemod/visitors/_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/visitors/_remove_imports.py` & `libcst-0.4.9/libcst/codemod/visitors/_remove_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/visitors/tests/test_add_imports.py` & `libcst-0.4.9/libcst/codemod/visitors/tests/test_add_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/visitors/tests/test_apply_type_annotations.py` & `libcst-0.4.9/libcst/codemod/visitors/tests/test_apply_type_annotations.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/visitors/tests/test_gather_comments.py` & `libcst-0.4.9/libcst/codemod/visitors/tests/test_gather_comments.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/visitors/tests/test_gather_exports.py` & `libcst-0.4.9/libcst/codemod/visitors/tests/test_gather_exports.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/visitors/tests/test_gather_global_names.py` & `libcst-0.4.9/libcst/codemod/visitors/tests/test_gather_global_names.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/visitors/tests/test_gather_imports.py` & `libcst-0.4.9/libcst/codemod/visitors/tests/test_gather_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/visitors/tests/test_gather_string_annotation_names.py` & `libcst-0.4.9/libcst/codemod/visitors/tests/test_gather_string_annotation_names.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/visitors/tests/test_gather_unused_imports.py` & `libcst-0.4.9/libcst/codemod/visitors/tests/test_gather_unused_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/codemod/visitors/tests/test_remove_imports.py` & `libcst-0.4.9/libcst/codemod/visitors/tests/test_remove_imports.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/helpers/__init__.py` & `libcst-0.4.9/libcst/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/helpers/_template.py` & `libcst-0.4.9/libcst/helpers/_template.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/helpers/common.py` & `libcst-0.4.9/libcst/helpers/common.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/helpers/expression.py` & `libcst-0.4.9/libcst/helpers/expression.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/helpers/module.py` & `libcst-0.4.9/libcst/helpers/module.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/helpers/tests/test_expression.py` & `libcst-0.4.9/libcst/helpers/tests/test_expression.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/helpers/tests/test_module.py` & `libcst-0.4.9/libcst/helpers/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/helpers/tests/test_template.py` & `libcst-0.4.9/libcst/helpers/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/matchers/__init__.py` & `libcst-0.4.9/libcst/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/matchers/_decorators.py` & `libcst-0.4.9/libcst/matchers/_decorators.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/matchers/_matcher_base.py` & `libcst-0.4.9/libcst/matchers/_matcher_base.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/matchers/_return_types.py` & `libcst-0.4.9/libcst/matchers/_return_types.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/matchers/_visitors.py` & `libcst-0.4.9/libcst/matchers/_visitors.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/matchers/tests/test_decorators.py` & `libcst-0.4.9/libcst/matchers/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/matchers/tests/test_extract.py` & `libcst-0.4.9/libcst/matchers/tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/matchers/tests/test_findall.py` & `libcst-0.4.9/libcst/matchers/tests/test_findall.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/matchers/tests/test_matchers.py` & `libcst-0.4.9/libcst/matchers/tests/test_matchers.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/matchers/tests/test_matchers_with_metadata.py` & `libcst-0.4.9/libcst/matchers/tests/test_matchers_with_metadata.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/matchers/tests/test_replace.py` & `libcst-0.4.9/libcst/matchers/tests/test_replace.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/matchers/tests/test_visitors.py` & `libcst-0.4.9/libcst/matchers/tests/test_visitors.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/metadata/__init__.py` & `libcst-0.4.9/libcst/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/metadata/accessor_provider.py` & `libcst-0.4.9/libcst/metadata/accessor_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/metadata/base_provider.py` & `libcst-0.4.9/libcst/metadata/base_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/metadata/expression_context_provider.py` & `libcst-0.4.9/libcst/metadata/expression_context_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/metadata/full_repo_manager.py` & `libcst-0.4.9/libcst/metadata/full_repo_manager.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/metadata/name_provider.py` & `libcst-0.4.9/libcst/metadata/name_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/metadata/parent_node_provider.py` & `libcst-0.4.9/libcst/metadata/parent_node_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/metadata/position_provider.py` & `libcst-0.4.9/libcst/metadata/position_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/metadata/reentrant_codegen.py` & `libcst-0.4.9/libcst/metadata/reentrant_codegen.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/metadata/scope_provider.py` & `libcst-0.4.9/libcst/metadata/scope_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/metadata/span_provider.py` & `libcst-0.4.9/libcst/metadata/span_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/metadata/tests/test_accessor_provider.py` & `libcst-0.4.9/libcst/metadata/tests/test_accessor_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/metadata/tests/test_base_provider.py` & `libcst-0.4.9/libcst/metadata/tests/test_base_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/metadata/tests/test_expression_context_provider.py` & `libcst-0.4.9/libcst/metadata/tests/test_expression_context_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/metadata/tests/test_full_repo_manager.py` & `libcst-0.4.9/libcst/metadata/tests/test_full_repo_manager.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/metadata/tests/test_metadata_provider.py` & `libcst-0.4.9/libcst/metadata/tests/test_metadata_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/metadata/tests/test_metadata_wrapper.py` & `libcst-0.4.9/libcst/metadata/tests/test_metadata_wrapper.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/metadata/tests/test_name_provider.py` & `libcst-0.4.9/libcst/metadata/tests/test_name_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/metadata/tests/test_parent_node_provider.py` & `libcst-0.4.9/libcst/metadata/tests/test_parent_node_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/metadata/tests/test_position_provider.py` & `libcst-0.4.9/libcst/metadata/tests/test_position_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/metadata/tests/test_reentrant_codegen.py` & `libcst-0.4.9/libcst/metadata/tests/test_reentrant_codegen.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/metadata/tests/test_scope_provider.py` & `libcst-0.4.9/libcst/metadata/tests/test_scope_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/metadata/tests/test_span_provider.py` & `libcst-0.4.9/libcst/metadata/tests/test_span_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/metadata/tests/test_type_inference_provider.py` & `libcst-0.4.9/libcst/metadata/tests/test_type_inference_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/metadata/type_inference_provider.py` & `libcst-0.4.9/libcst/metadata/type_inference_provider.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/metadata/wrapper.py` & `libcst-0.4.9/libcst/metadata/wrapper.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/testing/utils.py` & `libcst-0.4.9/libcst/testing/utils.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/tests/pyre/simple_class.json` & `libcst-0.4.9/libcst/tests/pyre/simple_class.json`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/tests/pyre/simple_class.py` & `libcst-0.4.9/libcst/tests/pyre/simple_class.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/tests/test_add_slots.py` & `libcst-0.4.9/libcst/tests/test_add_slots.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/tests/test_batched_visitor.py` & `libcst-0.4.9/libcst/tests/test_batched_visitor.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/tests/test_deep_clone.py` & `libcst-0.4.9/libcst/tests/test_deep_clone.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/tests/test_deep_replace.py` & `libcst-0.4.9/libcst/tests/test_deep_replace.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/tests/test_e2e.py` & `libcst-0.4.9/libcst/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/tests/test_exceptions.py` & `libcst-0.4.9/libcst/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/tests/test_fuzz.py` & `libcst-0.4.9/libcst/tests/test_fuzz.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/tests/test_pyre_integration.py` & `libcst-0.4.9/libcst/tests/test_pyre_integration.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/tests/test_tabs.py` & `libcst-0.4.9/libcst/tests/test_tabs.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/tests/test_tool.py` & `libcst-0.4.9/libcst/tests/test_tool.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/tests/test_type_enforce.py` & `libcst-0.4.9/libcst/tests/test_type_enforce.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/tests/test_visitor.py` & `libcst-0.4.9/libcst/tests/test_visitor.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst/tool.py` & `libcst-0.4.9/libcst/tool.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/libcst.egg-info/PKG-INFO` & `libcst-0.4.9/libcst.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libcst
-Version: 0.4.8
+Version: 0.4.9
 Summary: A concrete syntax tree with AST-like properties for Python 3.5, 3.6, 3.7, 3.8, 3.9, and 3.10 programs.
 Home-page: https://github.com/Instagram/LibCST
 License: MIT
 Project-URL: Changelog, https://github.com/Instagram/LibCST/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://libcst.readthedocs.io/en/latest/
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `libcst-0.4.8/libcst.egg-info/SOURCES.txt` & `libcst-0.4.9/libcst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/Cargo.lock` & `libcst-0.4.9/native/Cargo.lock`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/Cargo.toml` & `libcst-0.4.9/native/libcst/Cargo.toml`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/Grammar` & `libcst-0.4.9/native/libcst/Grammar`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/README.md` & `libcst-0.4.9/native/libcst/README.md`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/benches/parser_benchmark.rs` & `libcst-0.4.9/native/libcst/benches/parser_benchmark.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/src/bin.rs` & `libcst-0.4.9/native/libcst/src/bin.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/src/lib.rs` & `libcst-0.4.9/native/libcst/src/lib.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/src/nodes/codegen.rs` & `libcst-0.4.9/native/libcst/src/nodes/codegen.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/src/nodes/expression.rs` & `libcst-0.4.9/native/libcst/src/nodes/expression.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/src/nodes/inflate_helpers.rs` & `libcst-0.4.9/native/libcst/src/nodes/inflate_helpers.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/src/nodes/macros.rs` & `libcst-0.4.9/native/libcst/src/nodes/macros.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/src/nodes/mod.rs` & `libcst-0.4.9/native/libcst/src/nodes/mod.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/src/nodes/module.rs` & `libcst-0.4.9/native/libcst/src/nodes/module.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/src/nodes/op.rs` & `libcst-0.4.9/native/libcst/src/nodes/op.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/src/nodes/parser_config.rs` & `libcst-0.4.9/native/libcst/src/nodes/parser_config.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/src/nodes/py_cached.rs` & `libcst-0.4.9/native/libcst/src/nodes/py_cached.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/src/nodes/statement.rs` & `libcst-0.4.9/native/libcst/src/nodes/statement.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/src/nodes/test_utils.rs` & `libcst-0.4.9/native/libcst/src/nodes/test_utils.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/src/nodes/traits.rs` & `libcst-0.4.9/native/libcst/src/nodes/traits.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/src/nodes/whitespace.rs` & `libcst-0.4.9/native/libcst/src/nodes/whitespace.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/src/parser/errors.rs` & `libcst-0.4.9/native/libcst/src/parser/errors.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/src/parser/grammar.rs` & `libcst-0.4.9/native/libcst/src/parser/grammar.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/src/parser/numbers.rs` & `libcst-0.4.9/native/libcst/src/parser/numbers.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/src/py.rs` & `libcst-0.4.9/native/libcst/src/py.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/src/tokenizer/core/LICENSE` & `libcst-0.4.9/native/libcst/src/tokenizer/core/LICENSE`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/src/tokenizer/core/mod.rs` & `libcst-0.4.9/native/libcst/src/tokenizer/core/mod.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/src/tokenizer/core/string_types.rs` & `libcst-0.4.9/native/libcst/src/tokenizer/core/string_types.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/src/tokenizer/operators.rs` & `libcst-0.4.9/native/libcst/src/tokenizer/operators.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/src/tokenizer/tests.rs` & `libcst-0.4.9/native/libcst/src/tokenizer/tests.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/src/tokenizer/text_position/char_width.rs` & `libcst-0.4.9/native/libcst/src/tokenizer/text_position/char_width.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/src/tokenizer/text_position/mod.rs` & `libcst-0.4.9/native/libcst/src/tokenizer/text_position/mod.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/src/tokenizer/whitespace_parser.rs` & `libcst-0.4.9/native/libcst/src/tokenizer/whitespace_parser.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/tests/fixtures/big_binary_operator.py` & `libcst-0.4.9/native/libcst/tests/fixtures/big_binary_operator.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/tests/fixtures/comments.py` & `libcst-0.4.9/native/libcst/tests/fixtures/comments.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/tests/fixtures/expr.py` & `libcst-0.4.9/native/libcst/tests/fixtures/expr.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/tests/fixtures/fun_with_func_defs.py` & `libcst-0.4.9/native/libcst/tests/fixtures/fun_with_func_defs.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/tests/fixtures/malicious_match.py` & `libcst-0.4.9/native/libcst/tests/fixtures/malicious_match.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/tests/fixtures/pep646.py` & `libcst-0.4.9/native/libcst/tests/fixtures/pep646.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/tests/fixtures/super_strings.py` & `libcst-0.4.9/native/libcst/tests/fixtures/super_strings.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst/tests/parser_roundtrip.rs` & `libcst-0.4.9/native/libcst/tests/parser_roundtrip.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst_derive/src/codegen.rs` & `libcst-0.4.9/native/libcst_derive/src/codegen.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst_derive/src/cstnode.rs` & `libcst-0.4.9/native/libcst_derive/src/cstnode.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst_derive/src/inflate.rs` & `libcst-0.4.9/native/libcst_derive/src/inflate.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst_derive/src/into_py.rs` & `libcst-0.4.9/native/libcst_derive/src/into_py.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst_derive/src/lib.rs` & `libcst-0.4.9/native/libcst_derive/src/lib.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst_derive/src/parenthesized_node.rs` & `libcst-0.4.9/native/libcst_derive/src/parenthesized_node.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst_derive/tests/pass/minimal_cst.rs` & `libcst-0.4.9/native/libcst_derive/tests/pass/minimal_cst.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/native/libcst_derive/tests/pass/simple.rs` & `libcst-0.4.9/native/libcst_derive/tests/pass/simple.rs`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/setup.py` & `libcst-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/stubs/libcst_native/parser_config.pyi` & `libcst-0.4.9/stubs/libcst_native/parser_config.pyi`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/stubs/libcst_native/token_type.pyi` & `libcst-0.4.9/stubs/libcst_native/token_type.pyi`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/stubs/libcst_native/tokenize.pyi` & `libcst-0.4.9/stubs/libcst_native/tokenize.pyi`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/stubs/libcst_native/whitespace_parser.pyi` & `libcst-0.4.9/stubs/libcst_native/whitespace_parser.pyi`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/stubs/libcst_native/whitespace_state.pyi` & `libcst-0.4.9/stubs/libcst_native/whitespace_state.pyi`

 * *Files identical despite different names*

### Comparing `libcst-0.4.8/stubs/tokenize.pyi` & `libcst-0.4.9/stubs/tokenize.pyi`

 * *Files identical despite different names*

