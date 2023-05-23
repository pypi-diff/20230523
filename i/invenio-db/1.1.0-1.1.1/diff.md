# Comparing `tmp/invenio-db-1.1.0.tar.gz` & `tmp/invenio-db-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-db-1.1.0.tar", last modified: Tue Apr 11 08:04:00 2023, max compression
+gzip compressed data, was "dist/invenio-db-1.1.1.tar", last modified: Tue May 23 13:03:13 2023, max compression
```

## Comparing `invenio-db-1.1.0.tar` & `invenio-db-1.1.1.tar`

### file list

```diff
@@ -1,69 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:04:00.000000 invenio-db-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)      124 2023-04-11 08:03:57.000000 invenio-db-1.1.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (122)      641 2023-04-11 08:03:57.000000 invenio-db-1.1.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-04-11 08:03:57.000000 invenio-db-1.1.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:04:00.000000 invenio-db-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:04:00.000000 invenio-db-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      661 2023-04-11 08:03:57.000000 invenio-db-1.1.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2834 2023-04-11 08:03:57.000000 invenio-db-1.1.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (122)      492 2023-04-11 08:03:57.000000 invenio-db-1.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2535 2023-04-11 08:03:57.000000 invenio-db-1.1.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3698 2023-04-11 08:03:57.000000 invenio-db-1.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)      589 2023-04-11 08:03:57.000000 invenio-db-1.1.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-04-11 08:03:57.000000 invenio-db-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      693 2023-04-11 08:03:57.000000 invenio-db-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4878 2023-04-11 08:04:00.000000 invenio-db-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      948 2023-04-11 08:03:57.000000 invenio-db-1.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-04-11 08:03:57.000000 invenio-db-1.1.0/constraints-pypi.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:04:00.000000 invenio-db-1.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     7425 2023-04-11 08:03:57.000000 invenio-db-1.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     6314 2023-04-11 08:03:57.000000 invenio-db-1.1.0/docs/alembic.rst
--rw-r--r--   0 runner    (1001) docker     (122)      375 2023-04-11 08:03:57.000000 invenio-db-1.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-04-11 08:03:57.000000 invenio-db-1.1.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-04-11 08:03:57.000000 invenio-db-1.1.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (122)     9968 2023-04-11 08:03:57.000000 invenio-db-1.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1775 2023-04-11 08:03:57.000000 invenio-db-1.1.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-04-11 08:03:57.000000 invenio-db-1.1.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)      856 2023-04-11 08:03:57.000000 invenio-db-1.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-04-11 08:03:57.000000 invenio-db-1.1.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)      253 2023-04-11 08:03:57.000000 invenio-db-1.1.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6989 2023-04-11 08:03:57.000000 invenio-db-1.1.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-11 08:03:57.000000 invenio-db-1.1.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4138 2023-04-11 08:03:57.000000 invenio-db-1.1.0/docs/session_management.rst
--rw-r--r--   0 runner    (1001) docker     (122)      259 2023-04-11 08:03:57.000000 invenio-db-1.1.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:04:00.000000 invenio-db-1.1.0/invenio_db/
--rw-r--r--   0 runner    (1001) docker     (122)     2651 2023-04-11 08:03:57.000000 invenio-db-1.1.0/invenio_db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:04:00.000000 invenio-db-1.1.0/invenio_db/alembic/
--rw-r--r--   0 runner    (1001) docker     (122)     4110 2023-04-11 08:03:57.000000 invenio-db-1.1.0/invenio_db/alembic/35c1075e6360_force_naming_convention.py
--rw-r--r--   0 runner    (1001) docker     (122)      546 2023-04-11 08:03:57.000000 invenio-db-1.1.0/invenio_db/alembic/96e796392533_create_database_migrations.py
--rw-r--r--   0 runner    (1001) docker     (122)     1212 2023-04-11 08:03:57.000000 invenio-db-1.1.0/invenio_db/alembic/dbdbc1b19cf2_create_transaction_table.py
--rw-r--r--   0 runner    (1001) docker     (122)      693 2023-04-11 08:03:57.000000 invenio-db-1.1.0/invenio_db/alembic/script.py.mako
--rw-r--r--   0 runner    (1001) docker     (122)     3329 2023-04-11 08:03:57.000000 invenio-db-1.1.0/invenio_db/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     5593 2023-04-11 08:03:57.000000 invenio-db-1.1.0/invenio_db/ext.py
--rw-r--r--   0 runner    (1001) docker     (122)      444 2023-04-11 08:03:57.000000 invenio-db-1.1.0/invenio_db/proxies.py
--rw-r--r--   0 runner    (1001) docker     (122)     4148 2023-04-11 08:03:57.000000 invenio-db-1.1.0/invenio_db/shared.py
--rw-r--r--   0 runner    (1001) docker     (122)     4315 2023-04-11 08:03:57.000000 invenio-db-1.1.0/invenio_db/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:04:00.000000 invenio-db-1.1.0/invenio_db.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4878 2023-04-11 08:04:00.000000 invenio-db-1.1.0/invenio_db.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1329 2023-04-11 08:04:00.000000 invenio-db-1.1.0/invenio_db.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 08:04:00.000000 invenio-db-1.1.0/invenio_db.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      114 2023-04-11 08:04:00.000000 invenio-db-1.1.0/invenio_db.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 08:04:00.000000 invenio-db-1.1.0/invenio_db.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      329 2023-04-11 08:04:00.000000 invenio-db-1.1.0/invenio_db.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-11 08:04:00.000000 invenio-db-1.1.0/invenio_db.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-04-11 08:03:57.000000 invenio-db-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      671 2023-04-11 08:03:57.000000 invenio-db-1.1.0/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)      708 2023-04-11 08:03:57.000000 invenio-db-1.1.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (122)     1464 2023-04-11 08:04:00.000000 invenio-db-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-04-11 08:03:57.000000 invenio-db-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:04:00.000000 invenio-db-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1026 2023-04-11 08:03:57.000000 invenio-db-1.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:04:00.000000 invenio-db-1.1.0/tests/demo/
--rw-r--r--   0 runner    (1001) docker     (122)      254 2023-04-11 08:03:57.000000 invenio-db-1.1.0/tests/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-04-11 08:03:57.000000 invenio-db-1.1.0/tests/demo/child.py
--rw-r--r--   0 runner    (1001) docker     (122)      416 2023-04-11 08:03:57.000000 invenio-db-1.1.0/tests/demo/parent.py
--rw-r--r--   0 runner    (1001) docker     (122)      736 2023-04-11 08:03:57.000000 invenio-db-1.1.0/tests/demo/versioned_a.py
--rw-r--r--   0 runner    (1001) docker     (122)      736 2023-04-11 08:03:57.000000 invenio-db-1.1.0/tests/demo/versioned_b.py
--rw-r--r--   0 runner    (1001) docker     (122)    12583 2023-04-11 08:03:57.000000 invenio-db-1.1.0/tests/test_db.py
--rw-r--r--   0 runner    (1001) docker     (122)     2575 2023-04-11 08:03:57.000000 invenio-db-1.1.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3702 2023-04-11 08:03:57.000000 invenio-db-1.1.0/tests/test_versioning.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 13:03:12.000000 invenio-db-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-05-23 13:03:08.000000 invenio-db-1.1.1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)      641 2023-05-23 13:03:08.000000 invenio-db-1.1.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-05-23 13:03:08.000000 invenio-db-1.1.1/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 13:03:12.000000 invenio-db-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 13:03:12.000000 invenio-db-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      661 2023-05-23 13:03:08.000000 invenio-db-1.1.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2810 2023-05-23 13:03:08.000000 invenio-db-1.1.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-05-23 13:03:08.000000 invenio-db-1.1.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2693 2023-05-23 13:03:08.000000 invenio-db-1.1.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3698 2023-05-23 13:03:08.000000 invenio-db-1.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      589 2023-05-23 13:03:08.000000 invenio-db-1.1.1/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-05-23 13:03:08.000000 invenio-db-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-05-23 13:03:08.000000 invenio-db-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5108 2023-05-23 13:03:12.000000 invenio-db-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      948 2023-05-23 13:03:08.000000 invenio-db-1.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-05-23 13:03:08.000000 invenio-db-1.1.1/constraints-pypi.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 13:03:12.000000 invenio-db-1.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7425 2023-05-23 13:03:08.000000 invenio-db-1.1.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     6314 2023-05-23 13:03:08.000000 invenio-db-1.1.1/docs/alembic.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      375 2023-05-23 13:03:08.000000 invenio-db-1.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-05-23 13:03:08.000000 invenio-db-1.1.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-05-23 13:03:08.000000 invenio-db-1.1.1/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     9981 2023-05-23 13:03:08.000000 invenio-db-1.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1775 2023-05-23 13:03:08.000000 invenio-db-1.1.1/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-05-23 13:03:08.000000 invenio-db-1.1.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      856 2023-05-23 13:03:08.000000 invenio-db-1.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-05-23 13:03:08.000000 invenio-db-1.1.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-05-23 13:03:08.000000 invenio-db-1.1.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6989 2023-05-23 13:03:08.000000 invenio-db-1.1.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-23 13:03:08.000000 invenio-db-1.1.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4138 2023-05-23 13:03:08.000000 invenio-db-1.1.1/docs/session_management.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      259 2023-05-23 13:03:08.000000 invenio-db-1.1.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 13:03:12.000000 invenio-db-1.1.1/invenio_db/
+-rw-r--r--   0 runner    (1001) docker     (122)     2651 2023-05-23 13:03:08.000000 invenio-db-1.1.1/invenio_db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 13:03:12.000000 invenio-db-1.1.1/invenio_db/alembic/
+-rw-r--r--   0 runner    (1001) docker     (122)     4110 2023-05-23 13:03:08.000000 invenio-db-1.1.1/invenio_db/alembic/35c1075e6360_force_naming_convention.py
+-rw-r--r--   0 runner    (1001) docker     (122)      546 2023-05-23 13:03:08.000000 invenio-db-1.1.1/invenio_db/alembic/96e796392533_create_database_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1212 2023-05-23 13:03:08.000000 invenio-db-1.1.1/invenio_db/alembic/dbdbc1b19cf2_create_transaction_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-05-23 13:03:08.000000 invenio-db-1.1.1/invenio_db/alembic/script.py.mako
+-rw-r--r--   0 runner    (1001) docker     (122)     3443 2023-05-23 13:03:08.000000 invenio-db-1.1.1/invenio_db/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5593 2023-05-23 13:03:08.000000 invenio-db-1.1.1/invenio_db/ext.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4148 2023-05-23 13:03:08.000000 invenio-db-1.1.1/invenio_db/shared.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4271 2023-05-23 13:03:08.000000 invenio-db-1.1.1/invenio_db/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 13:03:12.000000 invenio-db-1.1.1/invenio_db.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5108 2023-05-23 13:03:12.000000 invenio-db-1.1.1/invenio_db.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-05-23 13:03:12.000000 invenio-db-1.1.1/invenio_db.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 13:03:12.000000 invenio-db-1.1.1/invenio_db.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      114 2023-05-23 13:03:12.000000 invenio-db-1.1.1/invenio_db.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 13:03:12.000000 invenio-db-1.1.1/invenio_db.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-05-23 13:03:12.000000 invenio-db-1.1.1/invenio_db.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-23 13:03:12.000000 invenio-db-1.1.1/invenio_db.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-05-23 13:03:08.000000 invenio-db-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      671 2023-05-23 13:03:08.000000 invenio-db-1.1.1/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)      708 2023-05-23 13:03:08.000000 invenio-db-1.1.1/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     1488 2023-05-23 13:03:12.000000 invenio-db-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-05-23 13:03:08.000000 invenio-db-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 13:03:12.000000 invenio-db-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1026 2023-05-23 13:03:08.000000 invenio-db-1.1.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 13:03:12.000000 invenio-db-1.1.1/tests/demo/
+-rw-r--r--   0 runner    (1001) docker     (122)      254 2023-05-23 13:03:08.000000 invenio-db-1.1.1/tests/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-05-23 13:03:08.000000 invenio-db-1.1.1/tests/demo/child.py
+-rw-r--r--   0 runner    (1001) docker     (122)      416 2023-05-23 13:03:08.000000 invenio-db-1.1.1/tests/demo/parent.py
+-rw-r--r--   0 runner    (1001) docker     (122)      736 2023-05-23 13:03:08.000000 invenio-db-1.1.1/tests/demo/versioned_a.py
+-rw-r--r--   0 runner    (1001) docker     (122)      736 2023-05-23 13:03:08.000000 invenio-db-1.1.1/tests/demo/versioned_b.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12713 2023-05-23 13:03:08.000000 invenio-db-1.1.1/tests/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2530 2023-05-23 13:03:08.000000 invenio-db-1.1.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3702 2023-05-23 13:03:08.000000 invenio-db-1.1.1/tests/test_versioning.py
```

### Comparing `invenio-db-1.1.0/.editorconfig` & `invenio-db-1.1.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-db-1.1.0/.github/workflows/pypi-publish.yml` & `invenio-db-1.1.1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-db-1.1.0/.github/workflows/tests.yml` & `invenio-db-1.1.1/.github/workflows/tests.yml`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             DB_EXTRAS: "mysql"
 
           - db-service: mysql8
             DB_EXTRAS: "mysql"
 
     env:
       DB: ${{ matrix.db-service }}
-      EXTRAS: tests,${{ matrix.DB_EXTRAS }}
+      EXTRAS: tests
     steps:
       - name: Checkout
         uses: actions/checkout@v2
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
```

### Comparing `invenio-db-1.1.0/CHANGES.rst` & `invenio-db-1.1.1/CHANGES.rst`

 * *Files 14% similar despite different names*

```diff
@@ -4,19 +4,28 @@
 
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 1.1.1 (released 2023-05-22)
+
+- upgrade minimal python version
+- code formatting
+- force installing greenlet dependency
+- upper pin alembic dependency version
+
+Version 1.0.15 (released 2023-05-17)
+
+- yanked due to mixed commits in the release
+
 Version 1.1.0 (released 2023-04-06)
 
-- Increase minimum version of Python to 3.7
-- Upgrades flask-sqlalchemy
-- Fixes deprecation warnings for flask-sqlalchemy, EncryptedType and WeakKeyDictionary
+- yanked, because of an incompatibility with Flask-SQLAlchemy v3.
 
 Version 1.0.14 (released 2022-03-30)
 
 - Adds support for SQLAlchemy 1.4 and Flask v2.1.
 
 Version 1.0.13 (released 2022-02-21)
```

### Comparing `invenio-db-1.1.0/CONTRIBUTING.rst` & `invenio-db-1.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-db-1.1.0/INSTALL.rst` & `invenio-db-1.1.1/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `invenio-db-1.1.0/LICENSE` & `invenio-db-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-db-1.1.0/MANIFEST.in` & `invenio-db-1.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-db-1.1.0/PKG-INFO` & `invenio-db-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-db
-Version: 1.1.0
+Version: 1.1.1
 Summary: Database management for Invenio.
 Home-page: https://github.com/inveniosoftware/invenio-db
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -39,19 +39,28 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 1.1.1 (released 2023-05-22)
+        
+        - upgrade minimal python version
+        - code formatting
+        - force installing greenlet dependency
+        - upper pin alembic dependency version
+        
+        Version 1.0.15 (released 2023-05-17)
+        
+        - yanked due to mixed commits in the release
+        
         Version 1.1.0 (released 2023-04-06)
         
-        - Increase minimum version of Python to 3.7
-        - Upgrades flask-sqlalchemy
-        - Fixes deprecation warnings for flask-sqlalchemy, EncryptedType and WeakKeyDictionary
+        - yanked, because of an incompatibility with Flask-SQLAlchemy v3.
         
         Version 1.0.14 (released 2022-03-30)
         
         - Adds support for SQLAlchemy 1.4 and Flask v2.1.
         
         Version 1.0.13 (released 2022-02-21)
```

### Comparing `invenio-db-1.1.0/README.rst` & `invenio-db-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-db-1.1.0/docs/Makefile` & `invenio-db-1.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-db-1.1.0/docs/alembic.rst` & `invenio-db-1.1.1/docs/alembic.rst`

 * *Files identical despite different names*

### Comparing `invenio-db-1.1.0/docs/conf.py` & `invenio-db-1.1.1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,11 +308,11 @@
 # texinfo_show_urls = 'footnote'
 
 # If true, do not generate a @detailmenu in the "Top" node's menu.
 # texinfo_no_detailmenu = False
 
 
 # Example configuration for intersphinx: refer to the Python standard library.
-intersphinx_mapping = {"https://docs.python.org/": None}
+intersphinx_mapping = {"python": ("https://docs.python.org/3", None)}
 
 # Autodoc configuraton.
 autoclass_content = "both"
```

### Comparing `invenio-db-1.1.0/docs/configuration.rst` & `invenio-db-1.1.1/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `invenio-db-1.1.0/docs/index.rst` & `invenio-db-1.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-db-1.1.0/docs/make.bat` & `invenio-db-1.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-db-1.1.0/docs/session_management.rst` & `invenio-db-1.1.1/docs/session_management.rst`

 * *Files identical despite different names*

### Comparing `invenio-db-1.1.0/invenio_db/__init__.py` & `invenio-db-1.1.1/invenio_db/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,14 +87,14 @@
    )
 
 """
 
 from .ext import InvenioDB
 from .shared import db
 
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 
 __all__ = (
     "__version__",
     "db",
     "InvenioDB",
 )
```

### Comparing `invenio-db-1.1.0/invenio_db/alembic/35c1075e6360_force_naming_convention.py` & `invenio-db-1.1.1/invenio_db/alembic/35c1075e6360_force_naming_convention.py`

 * *Files identical despite different names*

### Comparing `invenio-db-1.1.0/invenio_db/alembic/96e796392533_create_database_migrations.py` & `invenio-db-1.1.1/invenio_db/alembic/96e796392533_create_database_migrations.py`

 * *Files identical despite different names*

### Comparing `invenio-db-1.1.0/invenio_db/alembic/dbdbc1b19cf2_create_transaction_table.py` & `invenio-db-1.1.1/invenio_db/alembic/dbdbc1b19cf2_create_transaction_table.py`

 * *Files identical despite different names*

### Comparing `invenio-db-1.1.0/invenio_db/alembic/script.py.mako` & `invenio-db-1.1.1/invenio_db/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `invenio-db-1.1.0/invenio_db/cli.py` & `invenio-db-1.1.1/invenio_db/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,21 +4,31 @@
 # Copyright (C) 2015-2018 CERN.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Click command-line interface for database management."""
 
+import sys
+
 import click
+from click import _termui_impl
+from flask import current_app
 from flask.cli import with_appcontext
 from sqlalchemy_utils.functions import create_database, database_exists, drop_database
+from werkzeug.local import LocalProxy
 
-from .proxies import current_sqlalchemy
 from .utils import create_alembic_version_table, drop_alembic_version_table
 
+_db = LocalProxy(lambda: current_app.extensions["sqlalchemy"].db)
+
+# Fix Python 3 compatibility issue in click
+if sys.version_info > (3,):
+    _termui_impl.long = int  # pragma: no cover
+
 
 def abort_if_false(ctx, param, value):
     """Abort command is value is False."""
     if not value:
         ctx.abort()
 
 
@@ -41,19 +51,19 @@
 
 @db.command()
 @click.option("-v", "--verbose", is_flag=True, default=False)
 @with_appcontext
 def create(verbose):
     """Create tables."""
     click.secho("Creating all tables!", fg="yellow", bold=True)
-    with click.progressbar(current_sqlalchemy.metadata.sorted_tables) as bar:
+    with click.progressbar(_db.metadata.sorted_tables) as bar:
         for table in bar:
             if verbose:
                 click.echo(" Creating table {0}".format(table))
-            table.create(bind=current_sqlalchemy.engine, checkfirst=True)
+            table.create(bind=_db.engine, checkfirst=True)
     create_alembic_version_table()
     click.secho("Created all tables!", fg="green")
 
 
 @db.command()
 @click.option("-v", "--verbose", is_flag=True, default=False)
 @click.option(
@@ -63,30 +73,30 @@
     expose_value=False,
     prompt="Do you know that you are going to drop the db?",
 )
 @with_appcontext
 def drop(verbose):
     """Drop tables."""
     click.secho("Dropping all tables!", fg="red", bold=True)
-    with click.progressbar(reversed(current_sqlalchemy.metadata.sorted_tables)) as bar:
+    with click.progressbar(reversed(_db.metadata.sorted_tables)) as bar:
         for table in bar:
             if verbose:
                 click.echo(" Dropping table {0}".format(table))
-            table.drop(bind=current_sqlalchemy.engine, checkfirst=True)
+            table.drop(bind=_db.engine, checkfirst=True)
         drop_alembic_version_table()
     click.secho("Dropped all tables!", fg="green")
 
 
 @db.command()
 @with_appcontext
 def init():
     """Create database."""
-    displayed_database = render_url(current_sqlalchemy.engine.url)
+    displayed_database = render_url(_db.engine.url)
     click.secho(f"Creating database {displayed_database}", fg="green")
-    database_url = str(current_sqlalchemy.engine.url)
+    database_url = str(_db.engine.url)
     if not database_exists(database_url):
         create_database(database_url)
 
 
 @db.command()
 @click.option(
     "--yes-i-know",
@@ -94,16 +104,16 @@
     callback=abort_if_false,
     expose_value=False,
     prompt="Do you know that you are going to destroy the db?",
 )
 @with_appcontext
 def destroy():
     """Drop database."""
-    displayed_database = render_url(current_sqlalchemy.engine.url)
+    displayed_database = render_url(_db.engine.url)
     click.secho(f"Destroying database {displayed_database}", fg="red", bold=True)
-    if current_sqlalchemy.engine.name == "sqlite":
+    if _db.engine.name == "sqlite":
         try:
-            drop_database(current_sqlalchemy.engine.url)
-        except FileNotFoundError:
+            drop_database(_db.engine.url)
+        except FileNotFoundError as e:
             click.secho("Sqlite database has not been initialised", fg="red", bold=True)
     else:
-        drop_database(current_sqlalchemy.engine.url)
+        drop_database(_db.engine.url)
```

### Comparing `invenio-db-1.1.0/invenio_db/ext.py` & `invenio-db-1.1.1/invenio_db/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-db-1.1.0/invenio_db/shared.py` & `invenio-db-1.1.1/invenio_db/shared.py`

 * *Files identical despite different names*

### Comparing `invenio-db-1.1.0/invenio_db/utils.py` & `invenio-db-1.1.1/invenio_db/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,20 +7,22 @@
 # under the terms of the MIT License; see LICENSE file for more details.
 # from .signals import secret_key_changed
 
 """Invenio-DB utility functions."""
 
 from flask import current_app
 from sqlalchemy import inspect
+from werkzeug.local import LocalProxy
 
-from .proxies import current_sqlalchemy
-from .shared import db as _db
+from .shared import db
 
+_db = LocalProxy(lambda: current_app.extensions["sqlalchemy"].db)
 
-def rebuild_encrypted_properties(old_key, model, properties, db=_db):
+
+def rebuild_encrypted_properties(old_key, model, properties):
     """Rebuild model's EncryptedType properties when the SECRET_KEY is changed.
 
     :param old_key: old SECRET_KEY.
     :param model: the affected db model.
     :param properties: list of properties to rebuild.
     """
     inspector = inspect(db.engine)
@@ -67,21 +69,19 @@
         alembic.migration_context._ensure_version_table()
         for head in alembic.script_directory.revision_map._real_heads:
             alembic.migration_context.stamp(alembic.script_directory, head)
 
 
 def drop_alembic_version_table():
     """Drop alembic_version table."""
-    if has_table(current_sqlalchemy.engine, "alembic_version"):
-        alembic_version = current_sqlalchemy.Table(
-            "alembic_version",
-            current_sqlalchemy.metadata,
-            autoload_with=current_sqlalchemy.engine,
+    if has_table(_db.engine, "alembic_version"):
+        alembic_version = _db.Table(
+            "alembic_version", _db.metadata, autoload_with=_db.engine
         )
-        alembic_version.drop(bind=current_sqlalchemy.engine)
+        alembic_version.drop(bind=_db.engine)
 
 
 def versioning_model_classname(manager, model):
     """Get the name of the versioned model class."""
     if manager.options.get("use_module_name", True):
         return "%s%sVersion" % (
             model.__module__.title().replace(".", ""),
@@ -101,18 +101,20 @@
     return all(
         versioning_model_classname(manager, c) in declared_models
         for c in manager.pending_classes
     )
 
 
 def alembic_test_context():
-    """Alembic test context."""
+    """Alembic test context.
 
     # skip index from alembic migrations until sqlalchemy 2.0
     # https://github.com/sqlalchemy/sqlalchemy/discussions/7597
+    """
+
     def include_object(object, name, type_, reflected, compare_to):
         if name == "ix_uq_partial_files_object_is_head":
             return False
         return True
 
     return {
         "transaction_per_migration": True,
```

### Comparing `invenio-db-1.1.0/invenio_db.egg-info/PKG-INFO` & `invenio-db-1.1.1/invenio_db.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-db
-Version: 1.1.0
+Version: 1.1.1
 Summary: Database management for Invenio.
 Home-page: https://github.com/inveniosoftware/invenio-db
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -39,19 +39,28 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 1.1.1 (released 2023-05-22)
+        
+        - upgrade minimal python version
+        - code formatting
+        - force installing greenlet dependency
+        - upper pin alembic dependency version
+        
+        Version 1.0.15 (released 2023-05-17)
+        
+        - yanked due to mixed commits in the release
+        
         Version 1.1.0 (released 2023-04-06)
         
-        - Increase minimum version of Python to 3.7
-        - Upgrades flask-sqlalchemy
-        - Fixes deprecation warnings for flask-sqlalchemy, EncryptedType and WeakKeyDictionary
+        - yanked, because of an incompatibility with Flask-SQLAlchemy v3.
         
         Version 1.0.14 (released 2022-03-30)
         
         - Adds support for SQLAlchemy 1.4 and Flask v2.1.
         
         Version 1.0.13 (released 2022-02-21)
```

### Comparing `invenio-db-1.1.0/invenio_db.egg-info/SOURCES.txt` & `invenio-db-1.1.1/invenio_db.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 docs/make.bat
 docs/requirements.txt
 docs/session_management.rst
 docs/usage.rst
 invenio_db/__init__.py
 invenio_db/cli.py
 invenio_db/ext.py
-invenio_db/proxies.py
 invenio_db/shared.py
 invenio_db/utils.py
 invenio_db.egg-info/PKG-INFO
 invenio_db.egg-info/SOURCES.txt
 invenio_db.egg-info/dependency_links.txt
 invenio_db.egg-info/entry_points.txt
 invenio_db.egg-info/not-zip-safe
```

### Comparing `invenio-db-1.1.0/requirements-devel.txt` & `invenio-db-1.1.1/requirements-devel.txt`

 * *Files identical despite different names*

### Comparing `invenio-db-1.1.0/run-tests.sh` & `invenio-db-1.1.1/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-db-1.1.0/setup.cfg` & `invenio-db-1.1.1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -14,32 +14,32 @@
 
 [options]
 include_package_data = True
 packages = find:
 python_requires = >=3.7
 zip_safe = False
 install_requires = 
+	alembic>=1.10.0,<1.11.0
 	Flask-Alembic>=2.0.1
-	Flask-SQLAlchemy>=3.0,<4.0.0
+	Flask-SQLAlchemy>=2.1,<3.0.0
 	invenio-base>=1.2.10
 	SQLAlchemy-Continuum>=1.3.12
 	SQLAlchemy-Utils>=0.33.1,<0.39
-	SQLAlchemy>=1.2.18,<1.5.0
+	SQLAlchemy[asyncio]>=1.2.18,<1.5.0
 
 [options.extras_require]
 tests = 
-	six>=1.0.0
-	pytest-black>=0.3.0
+	pytest-black>=0.3.0,<0.3.10
 	cryptography>=2.1.4
 	pytest-invenio>=1.4.5
 	Sphinx>=4.5.0
-mysql = 
 	pymysql>=0.10.1
-postgresql = 
 	psycopg2-binary>=2.8.6
+mysql = 
+postgresql = 
 versioning = 
 
 [options.entry_points]
 invenio_base.api_apps = 
 	invenio_db = invenio_db:InvenioDB
 invenio_base.apps = 
 	invenio_db = invenio_db:InvenioDB
@@ -52,15 +52,15 @@
 build-dir = docs/_build
 all_files = 1
 
 [bdist_wheel]
 universal = 1
 
 [pydocstyle]
-add_ignore = D401, D202
+add_ignore = D401
 
 [isort]
 profile = black
 
 [check-manifest]
 ignore = 
 	*-requirements.txt
```

### Comparing `invenio-db-1.1.0/tests/conftest.py` & `invenio-db-1.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-db-1.1.0/tests/demo/versioned_a.py` & `invenio-db-1.1.1/tests/demo/versioned_a.py`

 * *Files identical despite different names*

### Comparing `invenio-db-1.1.0/tests/demo/versioned_b.py` & `invenio-db-1.1.1/tests/demo/versioned_b.py`

 * *Files identical despite different names*

### Comparing `invenio-db-1.1.0/tests/test_db.py` & `invenio-db-1.1.1/tests/test_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -331,31 +331,33 @@
 
         result = runner.invoke(db_cmd, ["init"])
         assert result.exit_code == 0
 
 
 def test_local_proxy(app, db):
     """Test local proxy filter."""
+    from werkzeug.local import LocalProxy
+
     InvenioDB(app, db=db)
 
     with app.app_context():
         query = db.select(
             [
                 db.literal("hello") != db.bindparam("a"),
                 db.literal(0) <= db.bindparam("x"),
                 db.literal("2") == db.bindparam("y"),
                 db.literal(None).is_(db.bindparam("z")),
             ]
         )
         result = db.engine.execute(
             query,
-            a="world",
-            x=1,
-            y="2",
-            z=None,
+            a=LocalProxy(lambda: "world"),
+            x=LocalProxy(lambda: 1),
+            y=LocalProxy(lambda: "2"),
+            z=LocalProxy(lambda: None),
         ).fetchone()
         assert result == (True, True, True, True)
 
 
 def test_db_create_alembic_upgrade(app, db):
     """Test that 'db create/drop' and 'alembic create' are compatible.
 
@@ -376,16 +378,17 @@
             # 'alembic upgrade'.
             result = runner.invoke(db_cmd, ["create", "-v"])
             assert result.exit_code == 0
             assert has_table(db.engine, "transaction")
             assert ext.alembic.migration_context._has_version_table()
             # Note that compare_metadata does not detect additional sequences
             # and constraints.
-            # Note: this compare_metadata leads on mysql8 to a not finishing test
-            # assert not ext.alembic.compare_metadata()
+            # TODO fix failing test on mysql
+            if db.engine.name != "mysql":
+                assert not ext.alembic.compare_metadata()
             ext.alembic.upgrade()
             assert has_table(db.engine, "transaction")
 
             ext.alembic.downgrade(target="96e796392533")
             assert inspect(db.engine).get_table_names() == ["alembic_version"]
 
             # Check that 'db drop' removes all tables, including
```

### Comparing `invenio-db-1.1.0/tests/test_utils.py` & `invenio-db-1.1.1/tests/test_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Test DB utilities."""
 
 import pytest
 import sqlalchemy as sa
 from sqlalchemy_continuum import remove_versioning
-from sqlalchemy_utils.types import StringEncryptedType
+from sqlalchemy_utils.types import EncryptedType
 
 from invenio_db import InvenioDB
 from invenio_db.utils import (
     rebuild_encrypted_properties,
     versioning_model_classname,
     versioning_models_registered,
 )
@@ -29,16 +29,15 @@
     def _secret_key():
         return app.config.get("SECRET_KEY").encode("utf-8")
 
     class Demo(db.Model):
         __tablename__ = "demo"
         pk = db.Column(sa.Integer, primary_key=True)
         et = db.Column(
-            StringEncryptedType(length=255, type_in=db.Unicode, key=_secret_key),
-            nullable=False,
+            EncryptedType(type_in=db.Unicode, key=_secret_key), nullable=False
         )
 
     InvenioDB(app, entry_point_group=False, db=db)
 
     with app.app_context():
         db.create_all()
         d1 = Demo(et="something")
@@ -47,21 +46,21 @@
 
     app.secret_key = new_secret_key
 
     with app.app_context():
         with pytest.raises(ValueError):
             db.session.query(Demo).all()
         with pytest.raises(AttributeError):
-            rebuild_encrypted_properties(old_secret_key, Demo, ["nonexistent"], db)
+            rebuild_encrypted_properties(old_secret_key, Demo, ["nonexistent"])
         assert app.secret_key == new_secret_key
 
     with app.app_context():
         with pytest.raises(ValueError):
             db.session.query(Demo).all()
-        rebuild_encrypted_properties(old_secret_key, Demo, ["et"], db)
+        rebuild_encrypted_properties(old_secret_key, Demo, ["et"])
         d1_after = db.session.query(Demo).first()
         assert d1_after.et == "something"
 
     with app.app_context():
         db.drop_all()
```

### Comparing `invenio-db-1.1.0/tests/test_versioning.py` & `invenio-db-1.1.1/tests/test_versioning.py`

 * *Files identical despite different names*

