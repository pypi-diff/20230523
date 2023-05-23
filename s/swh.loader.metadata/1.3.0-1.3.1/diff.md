# Comparing `tmp/swh.loader.metadata-1.3.0.tar.gz` & `tmp/swh.loader.metadata-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swh.loader.metadata-1.3.0.tar", last modified: Wed May 17 13:27:00 2023, max compression
+gzip compressed data, was "dist/swh.loader.metadata-1.3.1.tar", last modified: Tue May 23 12:57:47 2023, max compression
```

## Comparing `swh.loader.metadata-1.3.0.tar` & `swh.loader.metadata-1.3.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-17 13:27:00.000000 swh.loader.metadata-1.3.0/
--rw-r--r--   0 jenkins    (115) docker     (999)       83 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      943 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     1148 2023-05-17 13:27:00.000000 swh.loader.metadata-1.3.0/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)      190 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/README.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      373 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-17 13:27:00.000000 swh.loader.metadata-1.3.0/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/docs/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)      190 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/docs/README.rst
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-17 13:27:00.000000 swh.loader.metadata-1.3.0/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-17 13:27:00.000000 swh.loader.metadata-1.3.0/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/docs/conf.py
--rw-r--r--   0 jenkins    (115) docker     (999)      245 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/docs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      371 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      136 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      100 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      226 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/requirements.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-05-17 13:27:00.000000 swh.loader.metadata-1.3.0/setup.cfg
--rwxr-xr-x   0 jenkins    (115) docker     (999)     2632 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/setup.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-17 13:27:00.000000 swh.loader.metadata-1.3.0/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-17 13:27:00.000000 swh.loader.metadata-1.3.0/swh/loader/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/swh/loader/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-17 13:27:00.000000 swh.loader.metadata-1.3.0/swh/loader/metadata/
--rw-r--r--   0 jenkins    (115) docker     (999)      540 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/swh/loader/metadata/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7105 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/swh/loader/metadata/base.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3287 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/swh/loader/metadata/cli.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4501 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/swh/loader/metadata/gitea.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3280 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/swh/loader/metadata/github.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6226 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/swh/loader/metadata/journal_client.py
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/swh/loader/metadata/py.typed
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-17 13:27:00.000000 swh.loader.metadata-1.3.0/swh/loader/metadata/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/swh/loader/metadata/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-17 13:27:00.000000 swh.loader.metadata-1.3.0/swh/loader/metadata/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-17 13:27:00.000000 swh.loader.metadata-1.3.0/swh/loader/metadata/tests/data/https_api.github.com/
--rw-r--r--   0 jenkins    (115) docker     (999)    16850 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/swh/loader/metadata/tests/data/https_api.github.com/repos_jmarlena_linguist
--rw-r--r--   0 jenkins    (115) docker     (999)     5393 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/swh/loader/metadata/tests/data/https_api.github.com/repos_octocat_Hello-World
--rw-r--r--   0 jenkins    (115) docker     (999)    16869 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/swh/loader/metadata/tests/data/https_api.github.com/repos_octocat_linguist
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-17 13:27:00.000000 swh.loader.metadata-1.3.0/swh/loader/metadata/tests/data/https_codeberg.org/
--rw-r--r--   0 jenkins    (115) docker     (999)     1845 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/swh/loader/metadata/tests/data/https_codeberg.org/api_v1_repos_ForgeFed_ForgeFed
--rw-r--r--   0 jenkins    (115) docker     (999)     3632 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/swh/loader/metadata/tests/data/https_codeberg.org/api_v1_repos__ZN3val_ForgeFed
--rw-r--r--   0 jenkins    (115) docker     (999)     2873 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/swh/loader/metadata/tests/test_base.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3567 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/swh/loader/metadata/tests/test_cli.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3875 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/swh/loader/metadata/tests/test_gitea.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4058 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/swh/loader/metadata/tests/test_github.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8371 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/swh/loader/metadata/tests/test_journal_client.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-17 13:27:00.000000 swh.loader.metadata-1.3.0/swh.loader.metadata.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     1148 2023-05-17 13:27:00.000000 swh.loader.metadata-1.3.0/swh.loader.metadata.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     1547 2023-05-17 13:27:00.000000 swh.loader.metadata-1.3.0/swh.loader.metadata.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-05-17 13:27:00.000000 swh.loader.metadata-1.3.0/swh.loader.metadata.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      200 2023-05-17 13:27:00.000000 swh.loader.metadata-1.3.0/swh.loader.metadata.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      189 2023-05-17 13:27:00.000000 swh.loader.metadata-1.3.0/swh.loader.metadata.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-05-17 13:27:00.000000 swh.loader.metadata-1.3.0/swh.loader.metadata.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1551 2023-05-17 13:26:58.000000 swh.loader.metadata-1.3.0/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-23 12:57:47.000000 swh.loader.metadata-1.3.1/
+-rw-r--r--   0 jenkins    (115) docker     (999)       83 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      943 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     1148 2023-05-23 12:57:47.000000 swh.loader.metadata-1.3.1/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)      190 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/README.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      373 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-23 12:57:47.000000 swh.loader.metadata-1.3.1/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/docs/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)      190 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/docs/README.rst
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-23 12:57:47.000000 swh.loader.metadata-1.3.1/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-23 12:57:47.000000 swh.loader.metadata-1.3.1/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/docs/conf.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      245 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/docs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      371 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      136 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      100 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      226 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/requirements.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-05-23 12:57:47.000000 swh.loader.metadata-1.3.1/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     2632 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/setup.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-23 12:57:47.000000 swh.loader.metadata-1.3.1/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-23 12:57:47.000000 swh.loader.metadata-1.3.1/swh/loader/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/swh/loader/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-23 12:57:47.000000 swh.loader.metadata-1.3.1/swh/loader/metadata/
+-rw-r--r--   0 jenkins    (115) docker     (999)      540 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/swh/loader/metadata/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7105 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/swh/loader/metadata/base.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3287 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/swh/loader/metadata/cli.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4501 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/swh/loader/metadata/gitea.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3280 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/swh/loader/metadata/github.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6358 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/swh/loader/metadata/journal_client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/swh/loader/metadata/py.typed
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-23 12:57:47.000000 swh.loader.metadata-1.3.1/swh/loader/metadata/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/swh/loader/metadata/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-23 12:57:47.000000 swh.loader.metadata-1.3.1/swh/loader/metadata/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-23 12:57:47.000000 swh.loader.metadata-1.3.1/swh/loader/metadata/tests/data/https_api.github.com/
+-rw-r--r--   0 jenkins    (115) docker     (999)    16850 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/swh/loader/metadata/tests/data/https_api.github.com/repos_jmarlena_linguist
+-rw-r--r--   0 jenkins    (115) docker     (999)     5393 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/swh/loader/metadata/tests/data/https_api.github.com/repos_octocat_Hello-World
+-rw-r--r--   0 jenkins    (115) docker     (999)    16869 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/swh/loader/metadata/tests/data/https_api.github.com/repos_octocat_linguist
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-23 12:57:47.000000 swh.loader.metadata-1.3.1/swh/loader/metadata/tests/data/https_codeberg.org/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1845 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/swh/loader/metadata/tests/data/https_codeberg.org/api_v1_repos_ForgeFed_ForgeFed
+-rw-r--r--   0 jenkins    (115) docker     (999)     3632 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/swh/loader/metadata/tests/data/https_codeberg.org/api_v1_repos__ZN3val_ForgeFed
+-rw-r--r--   0 jenkins    (115) docker     (999)     2873 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/swh/loader/metadata/tests/test_base.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3567 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/swh/loader/metadata/tests/test_cli.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3875 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/swh/loader/metadata/tests/test_gitea.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4058 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/swh/loader/metadata/tests/test_github.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8371 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/swh/loader/metadata/tests/test_journal_client.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-23 12:57:47.000000 swh.loader.metadata-1.3.1/swh.loader.metadata.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1148 2023-05-23 12:57:47.000000 swh.loader.metadata-1.3.1/swh.loader.metadata.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     1547 2023-05-23 12:57:47.000000 swh.loader.metadata-1.3.1/swh.loader.metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-05-23 12:57:47.000000 swh.loader.metadata-1.3.1/swh.loader.metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      200 2023-05-23 12:57:47.000000 swh.loader.metadata-1.3.1/swh.loader.metadata.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      189 2023-05-23 12:57:47.000000 swh.loader.metadata-1.3.1/swh.loader.metadata.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-05-23 12:57:47.000000 swh.loader.metadata-1.3.1/swh.loader.metadata.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1551 2023-05-23 12:57:45.000000 swh.loader.metadata-1.3.1/tox.ini
```

### Comparing `swh.loader.metadata-1.3.0/.pre-commit-config.yaml` & `swh.loader.metadata-1.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.3.0/CODE_OF_CONDUCT.md` & `swh.loader.metadata-1.3.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.3.0/LICENSE` & `swh.loader.metadata-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.3.0/PKG-INFO` & `swh.loader.metadata-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.loader.metadata
-Version: 1.3.0
+Version: 1.3.1
 Summary: Software Heritage Extrinsic Metadata Fetchers
 Home-page: https://forge.softwareheritage.org/diffusion/swh-loader-metadata
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-loader-metadata
```

### Comparing `swh.loader.metadata-1.3.0/setup.py` & `swh.loader.metadata-1.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.3.0/swh/loader/metadata/__init__.py` & `swh.loader.metadata-1.3.1/swh/loader/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.3.0/swh/loader/metadata/base.py` & `swh.loader.metadata-1.3.1/swh/loader/metadata/base.py`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.3.0/swh/loader/metadata/cli.py` & `swh.loader.metadata-1.3.1/swh/loader/metadata/cli.py`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.3.0/swh/loader/metadata/gitea.py` & `swh.loader.metadata-1.3.1/swh/loader/metadata/gitea.py`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.3.0/swh/loader/metadata/github.py` & `swh.loader.metadata-1.3.1/swh/loader/metadata/github.py`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.3.0/swh/loader/metadata/journal_client.py` & `swh.loader.metadata-1.3.1/swh/loader/metadata/journal_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,16 @@
                 self.statsd_timed("get_listed_origins")(
                     self.scheduler.get_listed_origins
                 ),
                 url=origin["url"],
             ):
                 self._process_listed_origin(listed_origin)
 
-        self.storage.flush()
+        with self.statsd_timed("flush_storage"):
+            self.storage.flush()
 
     def _process_listed_origin(
         self,
         listed_origin: ListedOrigin,
     ) -> List[RawExtrinsicMetadata]:
         origin = Origin(url=listed_origin.url)
 
@@ -146,23 +147,27 @@
                     after=now - datetime.timedelta(days=self.reload_after_days),
                     limit=1,
                 )
 
             if last_metadata.results:
                 # We already have recent metadata; don't load it again.
                 self.statsd.increment(
-                    "metadata_items_fetched_total", len(last_metadata.results), tags=tags
+                    "metadata_items_fetched_total",
+                    len(last_metadata.results),
+                    tags=tags,
                 )
 
                 continue
 
             with self.statsd_timed("get_origin_metadata", tags=tags):
                 metadata = list(metadata_fetcher.get_origin_metadata())
 
-            self.statsd.increment("new_metadata_items", len(metadata), tags=tags)
+            self.statsd.increment(
+                "metadata_items_added_total", len(metadata), tags=tags
+            )
 
             with self.statsd_timed("metadata_fetcher_add"):
                 self._add_metadata_fetchers({m.fetcher for m in metadata})
 
             with self.statsd_timed("metadata_authority_add"):
                 self._add_metadata_authorities({m.authority for m in metadata})
```

### Comparing `swh.loader.metadata-1.3.0/swh/loader/metadata/tests/data/https_api.github.com/repos_jmarlena_linguist` & `swh.loader.metadata-1.3.1/swh/loader/metadata/tests/data/https_api.github.com/repos_jmarlena_linguist`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.3.0/swh/loader/metadata/tests/data/https_api.github.com/repos_octocat_Hello-World` & `swh.loader.metadata-1.3.1/swh/loader/metadata/tests/data/https_api.github.com/repos_octocat_Hello-World`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.3.0/swh/loader/metadata/tests/data/https_api.github.com/repos_octocat_linguist` & `swh.loader.metadata-1.3.1/swh/loader/metadata/tests/data/https_api.github.com/repos_octocat_linguist`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.3.0/swh/loader/metadata/tests/data/https_codeberg.org/api_v1_repos_ForgeFed_ForgeFed` & `swh.loader.metadata-1.3.1/swh/loader/metadata/tests/data/https_codeberg.org/api_v1_repos_ForgeFed_ForgeFed`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.3.0/swh/loader/metadata/tests/data/https_codeberg.org/api_v1_repos__ZN3val_ForgeFed` & `swh.loader.metadata-1.3.1/swh/loader/metadata/tests/data/https_codeberg.org/api_v1_repos__ZN3val_ForgeFed`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.3.0/swh/loader/metadata/tests/test_base.py` & `swh.loader.metadata-1.3.1/swh/loader/metadata/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.3.0/swh/loader/metadata/tests/test_cli.py` & `swh.loader.metadata-1.3.1/swh/loader/metadata/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.3.0/swh/loader/metadata/tests/test_gitea.py` & `swh.loader.metadata-1.3.1/swh/loader/metadata/tests/test_gitea.py`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.3.0/swh/loader/metadata/tests/test_github.py` & `swh.loader.metadata-1.3.1/swh/loader/metadata/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.3.0/swh/loader/metadata/tests/test_journal_client.py` & `swh.loader.metadata-1.3.1/swh/loader/metadata/tests/test_journal_client.py`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.3.0/swh.loader.metadata.egg-info/PKG-INFO` & `swh.loader.metadata-1.3.1/swh.loader.metadata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.loader.metadata
-Version: 1.3.0
+Version: 1.3.1
 Summary: Software Heritage Extrinsic Metadata Fetchers
 Home-page: https://forge.softwareheritage.org/diffusion/swh-loader-metadata
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-loader-metadata
```

### Comparing `swh.loader.metadata-1.3.0/swh.loader.metadata.egg-info/SOURCES.txt` & `swh.loader.metadata-1.3.1/swh.loader.metadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh.loader.metadata-1.3.0/tox.ini` & `swh.loader.metadata-1.3.1/tox.ini`

 * *Files identical despite different names*

