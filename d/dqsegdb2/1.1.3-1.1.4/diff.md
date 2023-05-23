# Comparing `tmp/dqsegdb2-1.1.3.tar.gz` & `tmp/dqsegdb2-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dqsegdb2-1.1.3.tar", last modified: Mon Sep 26 16:38:07 2022, max compression
+gzip compressed data, was "dqsegdb2-1.1.4.tar", last modified: Tue May 23 14:44:21 2023, max compression
```

## Comparing `dqsegdb2-1.1.3.tar` & `dqsegdb2-1.1.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-09-26 16:38:07.534064 dqsegdb2-1.1.3/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1129 2022-05-05 08:49:55.000000 dqsegdb2-1.1.3/.appveyor.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)      229 2022-01-31 17:11:59.000000 dqsegdb2-1.1.3/.codeclimate.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)      387 2022-05-04 14:08:06.000000 dqsegdb2-1.1.3/.flake8
--rw-r--r--   0 duncan    (1000) duncan    (1000)      190 2022-06-30 15:59:05.000000 dqsegdb2-1.1.3/.gitignore
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-09-26 16:38:07.514064 dqsegdb2-1.1.3/.gitlab/
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-09-26 16:38:07.524064 dqsegdb2-1.1.3/.gitlab/ci/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2200 2022-05-04 14:08:06.000000 dqsegdb2-1.1.3/.gitlab/ci/analysis.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)      579 2022-05-04 14:08:06.000000 dqsegdb2-1.1.3/.gitlab/ci/coverage.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3800 2022-06-30 15:59:05.000000 dqsegdb2-1.1.3/.gitlab/ci/debian.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)      627 2022-06-30 15:59:05.000000 dqsegdb2-1.1.3/.gitlab/ci/dist.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)      766 2022-09-26 16:28:58.000000 dqsegdb2-1.1.3/.gitlab/ci/docs.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1327 2022-05-04 14:08:06.000000 dqsegdb2-1.1.3/.gitlab/ci/python.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4000 2022-06-30 15:59:05.000000 dqsegdb2-1.1.3/.gitlab/ci/rhel.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)      953 2022-05-04 14:08:06.000000 dqsegdb2-1.1.3/.gitlab/ci/test.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)      519 2022-06-30 15:59:05.000000 dqsegdb2-1.1.3/.gitlab-ci.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)      291 2022-09-26 16:28:58.000000 dqsegdb2-1.1.3/.readthedocs.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)    33095 2020-11-12 14:45:19.000000 dqsegdb2-1.1.3/LICENSE
--rw-r--r--   0 duncan    (1000) duncan    (1000)      101 2022-06-30 15:59:05.000000 dqsegdb2-1.1.3/MANIFEST.in
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3078 2022-09-26 16:38:07.534064 dqsegdb2-1.1.3/PKG-INFO
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1621 2022-05-04 14:08:06.000000 dqsegdb2-1.1.3/README.md
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1734 2022-09-26 15:44:33.000000 dqsegdb2-1.1.3/RELEASE.md
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-09-26 16:38:07.534064 dqsegdb2-1.1.3/debian/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      577 2022-09-26 15:44:33.000000 dqsegdb2-1.1.3/debian/changelog
--rw-r--r--   0 duncan    (1000) duncan    (1000)        3 2022-06-30 15:59:05.000000 dqsegdb2-1.1.3/debian/compat
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1097 2022-09-26 15:44:33.000000 dqsegdb2-1.1.3/debian/control
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1033 2022-06-30 15:59:05.000000 dqsegdb2-1.1.3/debian/copyright
--rwxr-xr-x   0 duncan    (1000) duncan    (1000)      111 2022-06-30 15:59:05.000000 dqsegdb2-1.1.3/debian/rules
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-09-26 16:38:07.534064 dqsegdb2-1.1.3/debian/source/
--rw-r--r--   0 duncan    (1000) duncan    (1000)       12 2022-06-30 15:59:05.000000 dqsegdb2-1.1.3/debian/source/format
--rw-r--r--   0 duncan    (1000) duncan    (1000)      167 2022-06-30 15:59:05.000000 dqsegdb2-1.1.3/debian/watch
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-09-26 16:38:07.534064 dqsegdb2-1.1.3/docs/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1984 2022-09-26 15:44:51.000000 dqsegdb2-1.1.3/docs/conf.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2433 2022-09-26 15:44:33.000000 dqsegdb2-1.1.3/docs/index.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-09-26 16:38:07.534064 dqsegdb2-1.1.3/dqsegdb2/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1002 2022-05-05 08:58:10.000000 dqsegdb2-1.1.3/dqsegdb2/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)      176 2022-09-26 16:38:07.000000 dqsegdb2-1.1.3/dqsegdb2/_version.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3482 2022-09-23 09:33:33.000000 dqsegdb2-1.1.3/dqsegdb2/api.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5704 2022-09-26 14:44:46.000000 dqsegdb2-1.1.3/dqsegdb2/query.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-09-26 16:38:07.534064 dqsegdb2-1.1.3/dqsegdb2/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      768 2022-05-05 08:58:10.000000 dqsegdb2-1.1.3/dqsegdb2/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1261 2022-05-05 08:58:10.000000 dqsegdb2-1.1.3/dqsegdb2/tests/test_api.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2782 2022-05-05 08:58:10.000000 dqsegdb2-1.1.3/dqsegdb2/tests/test_query.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2022-09-26 16:38:07.534064 dqsegdb2-1.1.3/dqsegdb2.egg-info/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3078 2022-09-26 16:38:07.000000 dqsegdb2-1.1.3/dqsegdb2.egg-info/PKG-INFO
--rw-r--r--   0 duncan    (1000) duncan    (1000)      822 2022-09-26 16:38:07.000000 dqsegdb2-1.1.3/dqsegdb2.egg-info/SOURCES.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)        1 2022-09-26 16:38:07.000000 dqsegdb2-1.1.3/dqsegdb2.egg-info/dependency_links.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)      192 2022-09-26 16:38:07.000000 dqsegdb2-1.1.3/dqsegdb2.egg-info/requires.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)        9 2022-09-26 16:38:07.000000 dqsegdb2-1.1.3/dqsegdb2.egg-info/top_level.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)      801 2022-06-30 15:59:05.000000 dqsegdb2-1.1.3/pyproject.toml
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2659 2022-09-26 15:44:33.000000 dqsegdb2-1.1.3/python-dqsegdb2.spec
--rw-r--r--   0 duncan    (1000) duncan    (1000)       72 2022-01-31 17:11:59.000000 dqsegdb2-1.1.3/requirements.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1547 2022-09-26 16:38:07.534064 dqsegdb2-1.1.3/setup.cfg
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1058 2022-06-30 15:59:05.000000 dqsegdb2-1.1.3/setup.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-05-23 14:44:21.356606 dqsegdb2-1.1.4/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1129 2023-05-23 13:02:46.000000 dqsegdb2-1.1.4/.appveyor.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      229 2022-01-31 17:11:59.000000 dqsegdb2-1.1.4/.codeclimate.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      387 2023-05-23 13:02:46.000000 dqsegdb2-1.1.4/.flake8
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      190 2023-05-23 13:02:46.000000 dqsegdb2-1.1.4/.gitignore
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-05-23 14:44:21.336606 dqsegdb2-1.1.4/.gitlab/
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-05-23 14:44:21.346606 dqsegdb2-1.1.4/.gitlab/ci/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2384 2023-05-23 13:03:07.000000 dqsegdb2-1.1.4/.gitlab/ci/analysis.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      579 2022-05-04 14:08:06.000000 dqsegdb2-1.1.4/.gitlab/ci/coverage.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3800 2022-06-30 15:59:05.000000 dqsegdb2-1.1.4/.gitlab/ci/debian.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      627 2022-06-30 15:59:05.000000 dqsegdb2-1.1.4/.gitlab/ci/dist.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      766 2022-09-26 16:28:58.000000 dqsegdb2-1.1.4/.gitlab/ci/docs.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1327 2023-05-23 13:02:46.000000 dqsegdb2-1.1.4/.gitlab/ci/python.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4000 2022-06-30 15:59:05.000000 dqsegdb2-1.1.4/.gitlab/ci/rhel.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      953 2022-05-04 14:08:06.000000 dqsegdb2-1.1.4/.gitlab/ci/test.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      519 2022-06-30 15:59:05.000000 dqsegdb2-1.1.4/.gitlab-ci.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      291 2023-05-23 13:02:46.000000 dqsegdb2-1.1.4/.readthedocs.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    33095 2020-11-12 14:45:19.000000 dqsegdb2-1.1.4/LICENSE
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      101 2022-06-30 15:59:05.000000 dqsegdb2-1.1.4/MANIFEST.in
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3078 2023-05-23 14:44:21.356606 dqsegdb2-1.1.4/PKG-INFO
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1621 2022-05-04 14:08:06.000000 dqsegdb2-1.1.4/README.md
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1734 2022-09-26 15:44:33.000000 dqsegdb2-1.1.4/RELEASE.md
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-05-23 14:44:21.346606 dqsegdb2-1.1.4/debian/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      720 2023-05-23 14:40:58.000000 dqsegdb2-1.1.4/debian/changelog
+-rw-r--r--   0 duncan    (1000) duncan    (1000)        3 2022-06-30 15:59:05.000000 dqsegdb2-1.1.4/debian/compat
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1097 2022-09-26 15:44:33.000000 dqsegdb2-1.1.4/debian/control
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1033 2022-06-30 15:59:05.000000 dqsegdb2-1.1.4/debian/copyright
+-rwxr-xr-x   0 duncan    (1000) duncan    (1000)      111 2022-06-30 15:59:05.000000 dqsegdb2-1.1.4/debian/rules
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-05-23 14:44:21.346606 dqsegdb2-1.1.4/debian/source/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       12 2022-06-30 15:59:05.000000 dqsegdb2-1.1.4/debian/source/format
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      167 2022-06-30 15:59:05.000000 dqsegdb2-1.1.4/debian/watch
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-05-23 14:44:21.346606 dqsegdb2-1.1.4/docs/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1984 2023-05-23 13:02:46.000000 dqsegdb2-1.1.4/docs/conf.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2433 2023-05-23 13:02:46.000000 dqsegdb2-1.1.4/docs/index.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-05-23 14:44:21.346606 dqsegdb2-1.1.4/dqsegdb2/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1002 2023-05-23 13:02:46.000000 dqsegdb2-1.1.4/dqsegdb2/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      160 2023-05-23 14:44:21.000000 dqsegdb2-1.1.4/dqsegdb2/_version.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3482 2023-05-23 13:02:46.000000 dqsegdb2-1.1.4/dqsegdb2/api.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5932 2023-05-23 13:03:07.000000 dqsegdb2-1.1.4/dqsegdb2/query.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-05-23 14:44:21.356606 dqsegdb2-1.1.4/dqsegdb2/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      768 2022-05-05 08:58:10.000000 dqsegdb2-1.1.4/dqsegdb2/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1261 2023-05-23 13:02:46.000000 dqsegdb2-1.1.4/dqsegdb2/tests/test_api.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2782 2023-05-23 13:02:46.000000 dqsegdb2-1.1.4/dqsegdb2/tests/test_query.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-05-23 14:44:21.356606 dqsegdb2-1.1.4/dqsegdb2.egg-info/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3078 2023-05-23 14:44:21.000000 dqsegdb2-1.1.4/dqsegdb2.egg-info/PKG-INFO
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      822 2023-05-23 14:44:21.000000 dqsegdb2-1.1.4/dqsegdb2.egg-info/SOURCES.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)        1 2023-05-23 14:44:21.000000 dqsegdb2-1.1.4/dqsegdb2.egg-info/dependency_links.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      192 2023-05-23 14:44:21.000000 dqsegdb2-1.1.4/dqsegdb2.egg-info/requires.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)        9 2023-05-23 14:44:21.000000 dqsegdb2-1.1.4/dqsegdb2.egg-info/top_level.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      830 2023-05-23 13:03:07.000000 dqsegdb2-1.1.4/pyproject.toml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2748 2023-05-23 14:40:58.000000 dqsegdb2-1.1.4/python-dqsegdb2.spec
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       72 2022-01-31 17:11:59.000000 dqsegdb2-1.1.4/requirements.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1547 2023-05-23 14:44:21.356606 dqsegdb2-1.1.4/setup.cfg
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1058 2022-06-30 15:59:05.000000 dqsegdb2-1.1.4/setup.py
```

### Comparing `dqsegdb2-1.1.3/.appveyor.yml` & `dqsegdb2-1.1.4/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `dqsegdb2-1.1.3/.gitlab/ci/analysis.yml` & `dqsegdb2-1.1.4/.gitlab/ci/analysis.yml`

 * *Files 14% similar despite different names*

```diff
@@ -20,14 +20,19 @@
 
 flake8:
   stage: code quality
   extends:
     # https://computing.docs.ligo.org/gitlab-ci-templates/python/#.python:flake8
     - .python:flake8
   needs: []
+  variables:
+    # don't fail the pipeline because of linting issues,
+    # these are presented in the code-quality box in the
+    # merge_request UI
+    FLAKE8_OPTIONS: "--exit-zero"
   before_script:
     # pick requirements out of the setup.cfg
     - ${PYTHON} -m pip install setuptools --upgrade-strategy=only-if-needed
     - |
       REQUIREMENTS=$(${PYTHON} -c "
       from setuptools import Distribution
       dist = Distribution()
```

### Comparing `dqsegdb2-1.1.3/.gitlab/ci/coverage.yml` & `dqsegdb2-1.1.4/.gitlab/ci/coverage.yml`

 * *Files identical despite different names*

### Comparing `dqsegdb2-1.1.3/.gitlab/ci/debian.yml` & `dqsegdb2-1.1.4/.gitlab/ci/debian.yml`

 * *Files identical despite different names*

### Comparing `dqsegdb2-1.1.3/.gitlab/ci/dist.yml` & `dqsegdb2-1.1.4/.gitlab/ci/dist.yml`

 * *Files identical despite different names*

### Comparing `dqsegdb2-1.1.3/.gitlab/ci/docs.yml` & `dqsegdb2-1.1.4/.gitlab/ci/docs.yml`

 * *Files identical despite different names*

### Comparing `dqsegdb2-1.1.3/.gitlab/ci/python.yml` & `dqsegdb2-1.1.4/.gitlab/ci/python.yml`

 * *Files identical despite different names*

### Comparing `dqsegdb2-1.1.3/.gitlab/ci/rhel.yml` & `dqsegdb2-1.1.4/.gitlab/ci/rhel.yml`

 * *Files identical despite different names*

### Comparing `dqsegdb2-1.1.3/.gitlab/ci/test.yml` & `dqsegdb2-1.1.4/.gitlab/ci/test.yml`

 * *Files identical despite different names*

### Comparing `dqsegdb2-1.1.3/.gitlab-ci.yml` & `dqsegdb2-1.1.4/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dqsegdb2-1.1.3/LICENSE` & `dqsegdb2-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dqsegdb2-1.1.3/PKG-INFO` & `dqsegdb2-1.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dqsegdb2
-Version: 1.1.3
+Version: 1.1.4
 Summary: Simplified python interface to DQSEGDB
 Home-page: https://pypi.org/project/dqsegdb2/
 Author: Duncan Macleod
 Author-email: duncan.macleod@ligo.org
 License: GPL-3.0-or-later
 Project-URL: Bug Tracker, https://git.ligo.org/duncanmmacleod/dqsegdb2/-/issues
 Project-URL: Documentation, https://dqsegdb2.readthedocs.io
```

### Comparing `dqsegdb2-1.1.3/README.md` & `dqsegdb2-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `dqsegdb2-1.1.3/RELEASE.md` & `dqsegdb2-1.1.4/RELEASE.md`

 * *Files identical despite different names*

### Comparing `dqsegdb2-1.1.3/debian/control` & `dqsegdb2-1.1.4/debian/control`

 * *Files identical despite different names*

### Comparing `dqsegdb2-1.1.3/debian/copyright` & `dqsegdb2-1.1.4/debian/copyright`

 * *Files identical despite different names*

### Comparing `dqsegdb2-1.1.3/docs/conf.py` & `dqsegdb2-1.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dqsegdb2-1.1.3/docs/index.rst` & `dqsegdb2-1.1.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dqsegdb2-1.1.3/dqsegdb2/__init__.py` & `dqsegdb2-1.1.4/dqsegdb2/__init__.py`

 * *Files identical despite different names*

### Comparing `dqsegdb2-1.1.3/dqsegdb2/api.py` & `dqsegdb2-1.1.4/dqsegdb2/api.py`

 * *Files identical despite different names*

### Comparing `dqsegdb2-1.1.3/dqsegdb2/query.py` & `dqsegdb2-1.1.4/dqsegdb2/query.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 """
 
 import os
 
 from ligo import segments
 
 from igwn_auth_utils import requests as igwn_requests
+from igwn_auth_utils.scitokens import target_audience as scitoken_audience
 
 from . import api
 
 DEFAULT_SEGMENT_SERVER = os.environ.setdefault(
     'DEFAULT_SEGMENT_SERVER', 'https://segments.ligo.org')
 
 
@@ -164,14 +165,21 @@
         known=segments.segmentlist(),
         active=segments.segmentlist(),
         ifo=ifo,
         name=name,
         version=versions[0],
     )
 
+    # set default audience
+    if host:
+        request_kwargs.setdefault(
+            "token_audience",
+            scitoken_audience(host),
+        )
+
     with igwn_requests.Session(**request_kwargs) as sess:
         for i, version in enumerate(sorted(versions)):
             url = api.segment_query_url(host, ifo, name, version,
                                         start=start, end=end)
             result = _get_json(url, session=sess)
             for key in ('active', 'known'):
                 out[key].extend(segments.segmentlist(map(
```

### Comparing `dqsegdb2-1.1.3/dqsegdb2/tests/__init__.py` & `dqsegdb2-1.1.4/dqsegdb2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `dqsegdb2-1.1.3/dqsegdb2/tests/test_api.py` & `dqsegdb2-1.1.4/dqsegdb2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `dqsegdb2-1.1.3/dqsegdb2/tests/test_query.py` & `dqsegdb2-1.1.4/dqsegdb2/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `dqsegdb2-1.1.3/dqsegdb2.egg-info/PKG-INFO` & `dqsegdb2-1.1.4/dqsegdb2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dqsegdb2
-Version: 1.1.3
+Version: 1.1.4
 Summary: Simplified python interface to DQSEGDB
 Home-page: https://pypi.org/project/dqsegdb2/
 Author: Duncan Macleod
 Author-email: duncan.macleod@ligo.org
 License: GPL-3.0-or-later
 Project-URL: Bug Tracker, https://git.ligo.org/duncanmmacleod/dqsegdb2/-/issues
 Project-URL: Documentation, https://dqsegdb2.readthedocs.io
```

### Comparing `dqsegdb2-1.1.3/dqsegdb2.egg-info/SOURCES.txt` & `dqsegdb2-1.1.4/dqsegdb2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dqsegdb2-1.1.3/pyproject.toml` & `dqsegdb2-1.1.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -31,11 +31,12 @@
 # print report with one decimal point
 precision = 1
 
 [tool.pytest.ini_options]
 addopts = "-r a"
 filterwarnings = [
 	"error",
+	"ignore:.*pkg_resources.*",
 ]
 
 [tool.setuptools_scm]
 write_to = "dqsegdb2/_version.py"
```

### Comparing `dqsegdb2-1.1.3/python-dqsegdb2.spec` & `dqsegdb2-1.1.4/python-dqsegdb2.spec`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 %define srcname dqsegdb2
-%define version 1.1.3
+%define version 1.1.4
 %define release 1
 
 Name:     python-%{srcname}
 Version:  %{version}
 Release:  %{release}%{?dist}
 Summary:  Simplified python interface to DQSEGDB
 
@@ -73,14 +73,17 @@
 %license LICENSE
 %doc README.md
 %{python3_sitelib}/*
 
 # -- changelog
 
 %changelog
+* Tue May 23 2023 Duncan Macleod <duncan.macleod@ligo.org> - 1.1.4-1
+- update for 1.1.4
+
 * Mon Sep 26 2022 Duncan Macleod <duncan.macleod@ligo.org> - 1.1.3-1
 - update for 1.1.3
 - update igwn-auth-utils requirement
 - remove extra Requires for igwn-auth-utils[requests]
 
 * Thu May 05 2022 Duncan Macleod <duncan.macleod@ligo.org> - 1.1.2-1
 - update packaging for 1.1.2, reinstates RPM packages
```

### Comparing `dqsegdb2-1.1.3/setup.cfg` & `dqsegdb2-1.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `dqsegdb2-1.1.3/setup.py` & `dqsegdb2-1.1.4/setup.py`

 * *Files identical despite different names*

