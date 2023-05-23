# Comparing `tmp/invenio-xrootd-1.0.0a6.tar.gz` & `tmp/invenio-xrootd-2.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-xrootd-1.0.0a6.tar", last modified: Thu Aug 31 11:34:25 2017, max compression
+gzip compressed data, was "invenio-xrootd-2.0.0a1.tar", last modified: Tue May 23 11:49:53 2023, max compression
```

## Comparing `invenio-xrootd-1.0.0a6.tar` & `invenio-xrootd-2.0.0a1.tar`

### file list

```diff
@@ -1,51 +1,50 @@
-drwxr-xr-x   0 simko     (1000) simko     (1000)        0 2017-08-31 11:34:25.000000 invenio-xrootd-1.0.0a6/
--rw-rw-r--   0 simko     (1000) simko     (1000)     1964 2016-09-29 12:47:57.000000 invenio-xrootd-1.0.0a6/README.rst
-drwxr-xr-x   0 simko     (1000) simko     (1000)        0 2017-08-31 11:34:25.000000 invenio-xrootd-1.0.0a6/tests/
--rw-rw-r--   0 simko     (1000) simko     (1000)     3860 2016-09-16 14:29:49.000000 invenio-xrootd-1.0.0a6/tests/conftest.py
--rw-r--r--   0 simko     (1000) simko     (1000)     4333 2017-08-31 10:05:12.000000 invenio-xrootd-1.0.0a6/tests/test_storage.py
--rw-rw-r--   0 simko     (1000) simko     (1000)     3466 2016-09-05 14:44:41.000000 invenio-xrootd-1.0.0a6/CONTRIBUTING.rst
--rw-r--r--   0 simko     (1000) simko     (1000)     4497 2017-08-31 11:34:25.000000 invenio-xrootd-1.0.0a6/PKG-INFO
--rw-rw-r--   0 simko     (1000) simko     (1000)    18092 2016-09-05 14:44:41.000000 invenio-xrootd-1.0.0a6/LICENSE
--rw-rw-r--   0 simko     (1000) simko     (1000)      629 2016-09-29 12:47:57.000000 invenio-xrootd-1.0.0a6/INSTALL.rst
--rw-r--r--   0 simko     (1000) simko     (1000)     1062 2017-08-31 10:05:12.000000 invenio-xrootd-1.0.0a6/CHANGES.rst
--rw-r--r--   0 simko     (1000) simko     (1000)      197 2017-08-31 11:34:25.000000 invenio-xrootd-1.0.0a6/setup.cfg
--rw-rw-r--   0 simko     (1000) simko     (1000)     1087 2016-09-05 14:44:41.000000 invenio-xrootd-1.0.0a6/AUTHORS.rst
-drwxr-xr-x   0 simko     (1000) simko     (1000)        0 2017-08-31 11:34:25.000000 invenio-xrootd-1.0.0a6/docs/
--rw-rw-r--   0 simko     (1000) simko     (1000)     6997 2016-09-05 14:44:41.000000 invenio-xrootd-1.0.0a6/docs/make.bat
--rw-rw-r--   0 simko     (1000) simko     (1000)     1051 2016-09-05 14:44:41.000000 invenio-xrootd-1.0.0a6/docs/api.rst
--rw-rw-r--   0 simko     (1000) simko     (1000)     1008 2016-09-05 14:44:41.000000 invenio-xrootd-1.0.0a6/docs/installation.rst
--rw-rw-r--   0 simko     (1000) simko     (1000)      867 2016-09-05 14:44:41.000000 invenio-xrootd-1.0.0a6/docs/license.rst
--rw-rw-r--   0 simko     (1000) simko     (1000)     1008 2016-09-05 14:44:41.000000 invenio-xrootd-1.0.0a6/docs/changes.rst
--rw-rw-r--   0 simko     (1000) simko     (1000)     7441 2016-09-05 14:44:41.000000 invenio-xrootd-1.0.0a6/docs/Makefile
--rw-rw-r--   0 simko     (1000) simko     (1000)     1024 2016-09-05 14:44:41.000000 invenio-xrootd-1.0.0a6/docs/usage.rst
--rw-rw-r--   0 simko     (1000) simko     (1000)     1571 2016-09-05 14:44:41.000000 invenio-xrootd-1.0.0a6/docs/index.rst
--rw-rw-r--   0 simko     (1000) simko     (1000)     1013 2016-09-05 14:44:41.000000 invenio-xrootd-1.0.0a6/docs/contributing.rst
--rw-rw-r--   0 simko     (1000) simko     (1000)     1008 2016-09-05 14:44:41.000000 invenio-xrootd-1.0.0a6/docs/authors.rst
--rw-rw-r--   0 simko     (1000) simko     (1000)       17 2016-09-29 12:47:57.000000 invenio-xrootd-1.0.0a6/docs/requirements.txt
--rw-r--r--   0 simko     (1000) simko     (1000)    10687 2017-08-31 10:05:12.000000 invenio-xrootd-1.0.0a6/docs/conf.py
--rw-rw-r--   0 simko     (1000) simko     (1000)     1132 2016-09-05 14:44:41.000000 invenio-xrootd-1.0.0a6/requirements-devel.txt
--rw-rw-r--   0 simko     (1000) simko     (1000)     1533 2016-09-05 14:44:41.000000 invenio-xrootd-1.0.0a6/.editorconfig
--rw-r--r--   0 simko     (1000) simko     (1000)     1479 2016-10-18 14:45:27.000000 invenio-xrootd-1.0.0a6/MANIFEST.in
--rw-r--r--   0 simko     (1000) simko     (1000)       58 2016-10-18 14:45:27.000000 invenio-xrootd-1.0.0a6/MAINTAINERS
--rwxrwxr-x   0 simko     (1000) simko     (1000)     1184 2016-09-05 14:44:41.000000 invenio-xrootd-1.0.0a6/run-tests.sh
--rw-rw-r--   0 simko     (1000) simko     (1000)     1059 2016-09-05 14:44:41.000000 invenio-xrootd-1.0.0a6/pytest.ini
--rw-r--r--   0 simko     (1000) simko     (1000)     3240 2017-08-31 10:05:12.000000 invenio-xrootd-1.0.0a6/setup.py
--rw-r--r--   0 simko     (1000) simko     (1000)     1025 2017-08-31 10:05:12.000000 invenio-xrootd-1.0.0a6/run-docker.sh
-drwxr-xr-x   0 simko     (1000) simko     (1000)        0 2017-08-31 11:34:25.000000 invenio-xrootd-1.0.0a6/invenio_xrootd/
--rw-rw-r--   0 simko     (1000) simko     (1000)     3096 2016-09-29 12:47:57.000000 invenio-xrootd-1.0.0a6/invenio_xrootd/__init__.py
--rw-rw-r--   0 simko     (1000) simko     (1000)     1276 2016-09-05 14:44:41.000000 invenio-xrootd-1.0.0a6/invenio_xrootd/errors.py
--rw-r--r--   0 simko     (1000) simko     (1000)     1912 2017-08-31 10:05:12.000000 invenio-xrootd-1.0.0a6/invenio_xrootd/ext.py
--rw-r--r--   0 simko     (1000) simko     (1000)     1183 2017-08-31 10:05:12.000000 invenio-xrootd-1.0.0a6/invenio_xrootd/version.py
--rw-r--r--   0 simko     (1000) simko     (1000)     6797 2017-08-31 10:05:12.000000 invenio-xrootd-1.0.0a6/invenio_xrootd/storage.py
--rw-r--r--   0 simko     (1000) simko     (1000)      735 2017-08-31 10:05:12.000000 invenio-xrootd-1.0.0a6/RELEASE-NOTES.rst
--rw-rw-r--   0 simko     (1000) simko     (1000)      124 2016-09-05 14:44:41.000000 invenio-xrootd-1.0.0a6/.dockerignore
-drwxr-xr-x   0 simko     (1000) simko     (1000)        0 2017-08-31 11:34:25.000000 invenio-xrootd-1.0.0a6/invenio_xrootd.egg-info/
--rw-rw-r--   0 simko     (1000) simko     (1000)     4497 2017-08-31 11:34:25.000000 invenio-xrootd-1.0.0a6/invenio_xrootd.egg-info/PKG-INFO
--rw-rw-r--   0 simko     (1000) simko     (1000)      493 2017-08-31 11:34:25.000000 invenio-xrootd-1.0.0a6/invenio_xrootd.egg-info/requires.txt
--rw-rw-r--   0 simko     (1000) simko     (1000)        1 2016-09-25 11:34:54.000000 invenio-xrootd-1.0.0a6/invenio_xrootd.egg-info/not-zip-safe
--rw-rw-r--   0 simko     (1000) simko     (1000)       15 2017-08-31 11:34:25.000000 invenio-xrootd-1.0.0a6/invenio_xrootd.egg-info/top_level.txt
--rw-rw-r--   0 simko     (1000) simko     (1000)      866 2017-08-31 11:34:25.000000 invenio-xrootd-1.0.0a6/invenio_xrootd.egg-info/SOURCES.txt
--rw-rw-r--   0 simko     (1000) simko     (1000)        1 2017-08-31 11:34:25.000000 invenio-xrootd-1.0.0a6/invenio_xrootd.egg-info/dependency_links.txt
--rw-r--r--   0 simko     (1000) simko     (1000)      146 2017-08-31 11:34:25.000000 invenio-xrootd-1.0.0a6/invenio_xrootd.egg-info/entry_points.txt
-drwxr-xr-x   0 simko     (1000) simko     (1000)        0 2017-08-31 11:34:25.000000 invenio-xrootd-1.0.0a6/.tx/
--rw-rw-r--   0 simko     (1000) simko     (1000)     1790 2016-09-05 14:44:41.000000 invenio-xrootd-1.0.0a6/.tx/config
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:49:53.691458 invenio-xrootd-2.0.0a1/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-05-23 11:49:49.000000 invenio-xrootd-2.0.0a1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)      821 2023-05-23 11:49:49.000000 invenio-xrootd-2.0.0a1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:49:53.687458 invenio-xrootd-2.0.0a1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:49:53.687458 invenio-xrootd-2.0.0a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      879 2023-05-23 11:49:49.000000 invenio-xrootd-2.0.0a1/.github/workflows/pypi-release.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1120 2023-05-23 11:49:49.000000 invenio-xrootd-2.0.0a1/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:49:53.687458 invenio-xrootd-2.0.0a1/.tx/
+-rw-r--r--   0 runner    (1001) docker     (122)     1053 2023-05-23 11:49:49.000000 invenio-xrootd-2.0.0a1/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (122)      342 2023-05-23 11:49:49.000000 invenio-xrootd-2.0.0a1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      375 2023-05-23 11:49:49.000000 invenio-xrootd-2.0.0a1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3698 2023-05-23 11:49:49.000000 invenio-xrootd-2.0.0a1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1270 2023-05-23 11:49:49.000000 invenio-xrootd-2.0.0a1/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-05-23 11:49:49.000000 invenio-xrootd-2.0.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      750 2023-05-23 11:49:49.000000 invenio-xrootd-2.0.0a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2154 2023-05-23 11:49:53.691458 invenio-xrootd-2.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      997 2023-05-23 11:49:49.000000 invenio-xrootd-2.0.0a1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:49:53.687458 invenio-xrootd-2.0.0a1/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7441 2023-05-23 11:49:49.000000 invenio-xrootd-2.0.0a1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      292 2023-05-23 11:49:49.000000 invenio-xrootd-2.0.0a1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      249 2023-05-23 11:49:49.000000 invenio-xrootd-2.0.0a1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      249 2023-05-23 11:49:49.000000 invenio-xrootd-2.0.0a1/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     9906 2023-05-23 11:49:49.000000 invenio-xrootd-2.0.0a1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      254 2023-05-23 11:49:49.000000 invenio-xrootd-2.0.0a1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      812 2023-05-23 11:49:49.000000 invenio-xrootd-2.0.0a1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      249 2023-05-23 11:49:49.000000 invenio-xrootd-2.0.0a1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-05-23 11:49:49.000000 invenio-xrootd-2.0.0a1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6997 2023-05-23 11:49:49.000000 invenio-xrootd-2.0.0a1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-23 11:49:49.000000 invenio-xrootd-2.0.0a1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      265 2023-05-23 11:49:49.000000 invenio-xrootd-2.0.0a1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:49:53.687458 invenio-xrootd-2.0.0a1/invenio_xrootd/
+-rw-r--r--   0 runner    (1001) docker     (122)     2310 2023-05-23 11:49:49.000000 invenio-xrootd-2.0.0a1/invenio_xrootd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      483 2023-05-23 11:49:49.000000 invenio-xrootd-2.0.0a1/invenio_xrootd/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1132 2023-05-23 11:49:49.000000 invenio-xrootd-2.0.0a1/invenio_xrootd/ext.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5674 2023-05-23 11:49:49.000000 invenio-xrootd-2.0.0a1/invenio_xrootd/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:49:53.687458 invenio-xrootd-2.0.0a1/invenio_xrootd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2154 2023-05-23 11:49:53.000000 invenio-xrootd-2.0.0a1/invenio_xrootd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-05-23 11:49:53.000000 invenio-xrootd-2.0.0a1/invenio_xrootd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 11:49:53.000000 invenio-xrootd-2.0.0a1/invenio_xrootd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      146 2023-05-23 11:49:53.000000 invenio-xrootd-2.0.0a1/invenio_xrootd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 11:49:53.000000 invenio-xrootd-2.0.0a1/invenio_xrootd.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      150 2023-05-23 11:49:53.000000 invenio-xrootd-2.0.0a1/invenio_xrootd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-23 11:49:53.000000 invenio-xrootd-2.0.0a1/invenio_xrootd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      281 2023-05-23 11:49:49.000000 invenio-xrootd-2.0.0a1/run-docker.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      428 2023-05-23 11:49:49.000000 invenio-xrootd-2.0.0a1/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     1540 2023-05-23 11:49:53.691458 invenio-xrootd-2.0.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      321 2023-05-23 11:49:49.000000 invenio-xrootd-2.0.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:49:53.691458 invenio-xrootd-2.0.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     3040 2023-05-23 11:49:49.000000 invenio-xrootd-2.0.0a1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3464 2023-05-23 11:49:49.000000 invenio-xrootd-2.0.0a1/tests/test_storage.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `invenio-xrootd-1.0.0a6/tests/conftest.py` & `invenio-xrootd-2.0.0a1/tests/conftest.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,18 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2016 CERN.
+# Copyright (C) 2016-2019 CERN.
 #
-# Invenio is free software; you can redistribute it
-# and/or modify it under the terms of the GNU General Public License as
-# published by the Free Software Foundation; either version 2 of the
-# License, or (at your option) any later version.
-#
-# Invenio is distributed in the hope that it will be
-# useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-# General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with Invenio; if not, write to the
-# Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston,
-# MA 02111-1307, USA.
-#
-# In applying this license, CERN does not
-# waive the privileges and immunities granted to it by virtue of its status
-# as an Intergovernmental Organization or submit itself to any jurisdiction.
+# Invenio is free software; you can redistribute it and/or modify it
+# under the terms of the MIT License; see LICENSE file for more details.
 
 
 """Pytest configuration."""
 
-from __future__ import absolute_import, print_function
-
 import hashlib
 import shutil
 import tempfile
 from functools import wraps
 from os import makedirs
 from os.path import dirname, join
 
@@ -41,29 +23,27 @@
 
 
 @pytest.fixture
 def BytesIO():
     """IO instance."""
     try:
         from io import BytesIO
+
         return BytesIO
     except ImportError:
         from StringIO import StringIO
+
         return StringIO
 
 
 @pytest.yield_fixture()
 def app():
     """Flask application fixture."""
-    app = Flask('testapp')
-    app.config.update(
-        TESTING=True,
-        MAX_CONTENT_LENGTH=10,
-        XROOTD_CHECKSUM_ALGO='md5'
-    )
+    app = Flask("testapp")
+    app.config.update(TESTING=True, MAX_CONTENT_LENGTH=10, XROOTD_CHECKSUM_ALGO="md5")
     with app.app_context():
         yield app
 
 
 @pytest.fixture
 def mkurl():
     """Generate test root URL."""
@@ -78,29 +58,29 @@
     yield path
     shutil.rmtree(path)
 
 
 @pytest.fixture
 def file_path(tmppath):
     """File path."""
-    return join(tmppath, 'a/b/testfile')
+    return join(tmppath, "a/b/testfile")
 
 
 @pytest.fixture
 def file_url(file_path, mkurl):
     """File URL."""
     return mkurl(file_path)
 
 
 @pytest.fixture
 def file_content(file_path):
     """File content."""
     makedirs(dirname(file_path))
-    data = b'test'
-    with open(file_path, 'wb') as fp:
+    data = b"test"
+    with open(file_path, "wb") as fp:
         fp.write(data)
     return data
 
 
 @pytest.fixture
 def file_md5(file_content):
     """Checksum of content."""
@@ -129,15 +109,15 @@
     f = xrd_storage._get_fs
 
     @wraps(f)
     def mock(*args, **kwargs):
         fs, filename = f(*args, **kwargs)
 
         def xrd_checksum(*args, **kwargs):
-            return 'adler32', file_md5
+            return "adler32", file_md5
 
         fs.xrd_checksum = xrd_checksum
         return fs, filename
 
     xrd_storage._get_fs = mock
 
     return xrd_storage
@@ -148,13 +128,14 @@
     """EOS storage instance."""
     return EOSFileStorage(file_url)
 
 
 @pytest.fixture
 def file_instance_mock(file_url):
     """Mock of a file instance."""
+
     class FileInstance(object):
         def __init__(self, **kwargs):
             for k, v in kwargs.items():
                 setattr(self, k, v)
 
     return FileInstance(uri=file_url, size=4, updated=None)
```

### Comparing `invenio-xrootd-1.0.0a6/CONTRIBUTING.rst` & `invenio-xrootd-2.0.0a1/CONTRIBUTING.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+..
+    This file is part of Invenio.
+    Copyright (C) 2016-2019 CERN.
+
+    Invenio is free software; you can redistribute it and/or modify it
+    under the terms of the MIT License; see LICENSE file for more details.
+
 Contributing
 ============
 
 Contributions are welcome, and they are greatly appreciated! Every
 little bit helps, and credit will always be given.
 
 Types of Contributions
@@ -109,10 +116,10 @@
 -----------------------
 
 Before you submit a pull request, check that it meets these guidelines:
 
 1. The pull request should include tests and must not decrease test coverage.
 2. If the pull request adds functionality, the docs should be updated. Put
    your new functionality into a function with a docstring.
-3. The pull request should work for Python 2.7, 3.3, 3.4 and 3.5. Check
-   https://travis-ci.org/inveniosoftware/invenio-xrootd/pull_requests
+3. The pull request should work for Python 3.6, 3.7 and 3.8. Check
+   https://github.com/inveniosoftware/invenio-xrootd/actions?query=event%3Apull_request
    and make sure that the tests pass for all supported Python versions.
```

### Comparing `invenio-xrootd-1.0.0a6/docs/make.bat` & `invenio-xrootd-2.0.0a1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-xrootd-1.0.0a6/docs/Makefile` & `invenio-xrootd-2.0.0a1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-xrootd-1.0.0a6/docs/conf.py` & `invenio-xrootd-2.0.0a1/docs/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,334 +1,316 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2016 CERN.
+# Copyright (C) 2016-2019 CERN.
 #
-# Invenio is free software; you can redistribute it
-# and/or modify it under the terms of the GNU General Public License as
-# published by the Free Software Foundation; either version 2 of the
-# License, or (at your option) any later version.
-#
-# Invenio is distributed in the hope that it will be
-# useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-# General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with Invenio; if not, write to the
-# Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston,
-# MA 02111-1307, USA.
-#
-# In applying this license, CERN does not
-# waive the privileges and immunities granted to it by virtue of its status
-# as an Intergovernmental Organization or submit itself to any jurisdiction.
-
-from __future__ import print_function
-
-import os
+# Invenio is free software; you can redistribute it and/or modify it
+# under the terms of the MIT License; see LICENSE file for more details.
 
-import sphinx.environment
+from xrootdpyfs import __version__
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
-#needs_sphinx = '1.0'
+# needs_sphinx = '1.0'
 
 # Do not warn on external images.
-suppress_warnings = ['image.nonlocal_uri']
+suppress_warnings = ["image.nonlocal_uri"]
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    'sphinx.ext.autodoc',
-    'sphinx.ext.coverage',
-    'sphinx.ext.doctest',
-    'sphinx.ext.intersphinx',
-    'sphinx.ext.viewcode',
+    "sphinx.ext.autodoc",
+    "sphinx.ext.coverage",
+    "sphinx.ext.doctest",
+    "sphinx.ext.intersphinx",
+    "sphinx.ext.viewcode",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 # source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The encoding of source files.
-#source_encoding = 'utf-8-sig'
+# source_encoding = 'utf-8-sig'
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
-project = u'Invenio-XRootD'
-copyright = u'2016, CERN'
-author = u'CERN'
+project = "Invenio-XRootD"
+copyright = "2016, CERN"
+author = "CERN"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-
-# Get the version string. Cannot be done with import!
-g = {}
-with open(os.path.join('..', 'invenio_xrootd', 'version.py'), 'rt') as fp:
-    exec(fp.read(), g)
-    version = g['__version__']
+version = __version__
 
 # The full version, including alpha/beta/rc tags.
 release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
-#today = ''
+# today = ''
 # Else, today_fmt is used as the format for a strftime call.
-#today_fmt = '%B %d, %Y'
+# today_fmt = '%B %d, %Y'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 exclude_patterns = []
 
 # The reST default role (used for this markup: `text`) to use for all
 # documents.
-#default_role = None
+# default_role = None
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
-#add_function_parentheses = True
+# add_function_parentheses = True
 
 # If true, the current module name will be prepended to all description
 # unit titles (such as .. function::).
-#add_module_names = True
+# add_module_names = True
 
 # If true, sectionauthor and moduleauthor directives will be shown in the
 # output. They are ignored by default.
-#show_authors = False
+# show_authors = False
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # A list of ignored prefixes for module index sorting.
-#modindex_common_prefix = []
+# modindex_common_prefix = []
 
 # If true, keep warnings as "system message" paragraphs in the built documents.
-#keep_warnings = False
+# keep_warnings = False
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = False
 
 
 # -- Options for HTML output ----------------------------------------------
-html_theme = 'alabaster'
+html_theme = "alabaster"
 
 html_theme_options = {
-    'description': 'XRootD file storage support for Invenio.',
-    'github_user': 'inveniosoftware',
-    'github_repo': 'invenio-xrootd',
-    'github_button': False,
-    'github_banner': True,
-    'show_powered_by': False,
-    'extra_nav_links': {
-        'invenio-xrootd@GitHub': 'http://github.com/inveniosoftware/invenio-xrootd',
-        'invenio-xrootd@PyPI': 'http://pypi.python.org/pypi/invenio-xrootd/',
-    }
+    "description": "XRootD file storage support for Invenio.",
+    "github_user": "inveniosoftware",
+    "github_repo": "invenio-xrootd",
+    "github_button": False,
+    "github_banner": True,
+    "show_powered_by": False,
+    "extra_nav_links": {
+        "invenio-xrootd@GitHub": "http://github.com/inveniosoftware/invenio-xrootd",
+        "invenio-xrootd@PyPI": "http://pypi.python.org/pypi/invenio-xrootd/",
+    },
 }
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
-#html_theme_options = {}
+# html_theme_options = {}
 
 # Add any paths that contain custom themes here, relative to this directory.
-#html_theme_path = []
+# html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
-#html_title = None
+# html_title = None
 
 # A shorter title for the navigation bar.  Default is the same as html_title.
-#html_short_title = None
+# html_short_title = None
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
-#html_logo = None
+# html_logo = None
 
 # The name of an image file (within the static path) to use as favicon of the
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
-#html_favicon = None
+# html_favicon = None
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-#html_static_path = ['_static']
+# html_static_path = ['_static']
 
 # Add any extra paths that contain custom files (such as robots.txt or
 # .htaccess) here, relative to this directory. These files are copied
 # directly to the root of the documentation.
-#html_extra_path = []
+# html_extra_path = []
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
 # using the given strftime format.
-#html_last_updated_fmt = '%b %d, %Y'
+# html_last_updated_fmt = '%b %d, %Y'
 
 # If true, SmartyPants will be used to convert quotes and dashes to
 # typographically correct entities.
-#html_use_smartypants = True
+# html_use_smartypants = True
 
 # Custom sidebar templates, maps document names to template names.
 html_sidebars = {
-    '**': [
-        'about.html',
-        'navigation.html',
-        'relations.html',
-        'searchbox.html',
-        'donate.html',
+    "**": [
+        "about.html",
+        "navigation.html",
+        "relations.html",
+        "searchbox.html",
+        "donate.html",
     ]
 }
 
 # Additional templates that should be rendered to pages, maps page names to
 # template names.
-#html_additional_pages = {}
+# html_additional_pages = {}
 
 # If false, no module index is generated.
-#html_domain_indices = True
+# html_domain_indices = True
 
 # If false, no index is generated.
-#html_use_index = True
+# html_use_index = True
 
 # If true, the index is split into individual pages for each letter.
-#html_split_index = False
+# html_split_index = False
 
 # If true, links to the reST sources are added to the pages.
-#html_show_sourcelink = True
+# html_show_sourcelink = True
 
 # If true, "Created using Sphinx" is shown in the HTML footer. Default is True.
-#html_show_sphinx = True
+# html_show_sphinx = True
 
 # If true, "(C) Copyright ..." is shown in the HTML footer. Default is True.
-#html_show_copyright = True
+# html_show_copyright = True
 
 # If true, an OpenSearch description file will be output, and all pages will
 # contain a <link> tag referring to it.  The value of this option must be the
 # base URL from which the finished HTML is served.
-#html_use_opensearch = ''
+# html_use_opensearch = ''
 
 # This is the file name suffix for HTML files (e.g. ".xhtml").
-#html_file_suffix = None
+# html_file_suffix = None
 
 # Language to be used for generating the HTML full-text search index.
 # Sphinx supports the following languages:
 #   'da', 'de', 'en', 'es', 'fi', 'fr', 'hu', 'it', 'ja'
 #   'nl', 'no', 'pt', 'ro', 'ru', 'sv', 'tr'
-#html_search_language = 'en'
+# html_search_language = 'en'
 
 # A dictionary with options for the search language support, empty by default.
 # Now only 'ja' uses this config value
-#html_search_options = {'type': 'default'}
+# html_search_options = {'type': 'default'}
 
 # The name of a javascript file (relative to the configuration directory) that
 # implements a search results scorer. If empty, the default will be used.
-#html_search_scorer = 'scorer.js'
+# html_search_scorer = 'scorer.js'
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'invenio-xrootd_namedoc'
+htmlhelp_basename = "invenio-xrootd_namedoc"
 
 # -- Options for LaTeX output ---------------------------------------------
 
 latex_elements = {
-# The paper size ('letterpaper' or 'a4paper').
-#'papersize': 'letterpaper',
-
-# The font size ('10pt', '11pt' or '12pt').
-#'pointsize': '10pt',
-
-# Additional stuff for the LaTeX preamble.
-#'preamble': '',
-
-# Latex figure (float) alignment
-#'figure_align': 'htbp',
+    # The paper size ('letterpaper' or 'a4paper').
+    #'papersize': 'letterpaper',
+    # The font size ('10pt', '11pt' or '12pt').
+    #'pointsize': '10pt',
+    # Additional stuff for the LaTeX preamble.
+    #'preamble': '',
+    # Latex figure (float) alignment
+    #'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
-  (master_doc, 'invenio-xrootd.tex', u'invenio-xrootd Documentation',
-   u'CERN', 'manual'),
+    (
+        master_doc,
+        "invenio-xrootd.tex",
+        "invenio-xrootd Documentation",
+        "CERN",
+        "manual",
+    ),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
-#latex_logo = None
+# latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
 # not chapters.
-#latex_use_parts = False
+# latex_use_parts = False
 
 # If true, show page references after internal links.
-#latex_show_pagerefs = False
+# latex_show_pagerefs = False
 
 # If true, show URL addresses after external links.
-#latex_show_urls = False
+# latex_show_urls = False
 
 # Documents to append as an appendix to all manuals.
-#latex_appendices = []
+# latex_appendices = []
 
 # If false, no module index is generated.
-#latex_domain_indices = True
+# latex_domain_indices = True
 
 
 # -- Options for manual page output ---------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
-    (master_doc, 'invenio-xrootd', u'invenio-xrootd Documentation',
-     [author], 1)
+    (master_doc, "invenio-xrootd", "invenio-xrootd Documentation", [author], 1)
 ]
 
 # If true, show URL addresses after external links.
-#man_show_urls = False
+# man_show_urls = False
 
 
 # -- Options for Texinfo output -------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-  (master_doc, 'invenio-xrootd', u'Invenio-XRootD Documentation',
-   author, 'invenio-xrootd', 'XRootD file storage support for Invenio.',
-   'Miscellaneous'),
+    (
+        master_doc,
+        "invenio-xrootd",
+        "Invenio-XRootD Documentation",
+        author,
+        "invenio-xrootd",
+        "XRootD file storage support for Invenio.",
+        "Miscellaneous",
+    ),
 ]
 
 # Documents to append as an appendix to all manuals.
-#texinfo_appendices = []
+# texinfo_appendices = []
 
 # If false, no module index is generated.
-#texinfo_domain_indices = True
+# texinfo_domain_indices = True
 
 # How to display URL addresses: 'footnote', 'no', or 'inline'.
-#texinfo_show_urls = 'footnote'
+# texinfo_show_urls = 'footnote'
 
 # If true, do not generate a @detailmenu in the "Top" node's menu.
-#texinfo_no_detailmenu = False
+# texinfo_no_detailmenu = False
 
 
 # Example configuration for intersphinx: refer to the Python standard library.
-intersphinx_mapping = {'https://docs.python.org/': None}
+intersphinx_mapping = {"https://docs.python.org/": None}
 
 # Autodoc configuraton.
-autoclass_content = 'both'
+autoclass_content = "both"
```

### Comparing `invenio-xrootd-1.0.0a6/invenio_xrootd/__init__.py` & `invenio-xrootd-2.0.0a1/invenio_xrootd/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,14 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2016 CERN.
+# Copyright (C) 2016-2019 CERN.
 #
-# Invenio is free software; you can redistribute it
-# and/or modify it under the terms of the GNU General Public License as
-# published by the Free Software Foundation; either version 2 of the
-# License, or (at your option) any later version.
-#
-# Invenio is distributed in the hope that it will be
-# useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-# General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with Invenio; if not, write to the
-# Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston,
-# MA 02111-1307, USA.
-#
-# In applying this license, CERN does not
-# waive the privileges and immunities granted to it by virtue of its status
-# as an Intergovernmental Organization or submit itself to any jurisdiction.
+# Invenio is free software; you can redistribute it and/or modify it
+# under the terms of the MIT License; see LICENSE file for more details.
 
 r"""XRootD file storage support for Invenio.
 
 This modules provide an Invenio file storage interface for XRootD. By default
 Invenio already has support for XRootD via
 `PyFilesytem <http://docs.pyfilesystem.org/en/latest/>`_  and the
 `XRootDPyFS <http://xrootdpyfs.readthedocs.io/>`_ package. This module
@@ -69,22 +53,25 @@
 you can run a tool such as
 `k5start <https://www.eyrie.org/~eagle/software/kstart/k5start.html>`_ on each
 client node in order to obtain a Kerberos ticket and continue keeping the
 ticket valid. The XRootD python bindings will transparently use this Kerberos
 ticket to authenticate against your server.
 """
 
-from __future__ import absolute_import, print_function
-
 from .errors import SizeRequiredError
-from .storage import EOSFileStorage, XRootDFileStorage, eos_storage_factory, \
-    xrootd_storage_factory
-from .version import __version__
+from .storage import (
+    EOSFileStorage,
+    XRootDFileStorage,
+    eos_storage_factory,
+    xrootd_storage_factory,
+)
+
+__version__ = "2.0.0a1"
 
 __all__ = (
-    '__version__',
-    'eos_storage_factory',
-    'EOSFileStorage',
-    'SizeRequiredError',
-    'xrootd_storage_factory',
-    'XRootDFileStorage',
+    "__version__",
+    "eos_storage_factory",
+    "EOSFileStorage",
+    "SizeRequiredError",
+    "xrootd_storage_factory",
+    "XRootDFileStorage",
 )
```

### Comparing `invenio-xrootd-1.0.0a6/invenio_xrootd.egg-info/SOURCES.txt` & `invenio-xrootd-2.0.0a1/invenio_xrootd.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 .dockerignore
 .editorconfig
 AUTHORS.rst
 CHANGES.rst
 CONTRIBUTING.rst
 INSTALL.rst
 LICENSE
-MAINTAINERS
 MANIFEST.in
 README.rst
-RELEASE-NOTES.rst
-pytest.ini
-requirements-devel.txt
 run-docker.sh
 run-tests.sh
 setup.cfg
 setup.py
+.github/workflows/pypi-release.yml
+.github/workflows/tests.yml
 .tx/config
 docs/Makefile
 docs/api.rst
 docs/authors.rst
 docs/changes.rst
 docs/conf.py
 docs/contributing.rst
@@ -28,15 +26,14 @@
 docs/make.bat
 docs/requirements.txt
 docs/usage.rst
 invenio_xrootd/__init__.py
 invenio_xrootd/errors.py
 invenio_xrootd/ext.py
 invenio_xrootd/storage.py
-invenio_xrootd/version.py
 invenio_xrootd.egg-info/PKG-INFO
 invenio_xrootd.egg-info/SOURCES.txt
 invenio_xrootd.egg-info/dependency_links.txt
 invenio_xrootd.egg-info/entry_points.txt
 invenio_xrootd.egg-info/not-zip-safe
 invenio_xrootd.egg-info/requires.txt
 invenio_xrootd.egg-info/top_level.txt
```

