# Comparing `tmp/pcrunner-1.0.2.tar.gz` & `tmp/pcrunner-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcrunner-1.0.2.tar", last modified: Sat Apr  1 17:45:01 2023, max compression
+gzip compressed data, was "pcrunner-1.0.3.tar", last modified: Tue May 23 14:18:42 2023, max compression
```

## Comparing `pcrunner-1.0.2.tar` & `pcrunner-1.0.3.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-04-01 17:45:01.193294 pcrunner-1.0.2/
--rw-r--r--   0 maarten    (501) staff       (20)      216 2021-10-21 13:00:44.000000 pcrunner-1.0.2/.flake8
-drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-04-01 17:45:01.175914 pcrunner-1.0.2/.github/
-drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-04-01 17:45:01.181384 pcrunner-1.0.2/.github/workflows/
--rw-r--r--   0 maarten    (501) staff       (20)     1471 2023-04-01 17:33:35.000000 pcrunner-1.0.2/.github/workflows/ci.yml
--rw-r--r--   0 maarten    (501) staff       (20)     2480 2021-10-21 13:00:44.000000 pcrunner-1.0.2/.gitignore
--rw-r--r--   0 maarten    (501) staff       (20)      954 2023-04-01 17:16:32.000000 pcrunner-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0 maarten    (501) staff       (20)      499 2021-10-21 13:00:44.000000 pcrunner-1.0.2/.readthedocs.yaml
--rw-r--r--   0 maarten    (501) staff       (20)     3557 2021-10-21 18:48:37.000000 pcrunner-1.0.2/HISTORY.rst
--rw-r--r--   0 maarten    (501) staff       (20)      762 2021-10-21 18:48:37.000000 pcrunner-1.0.2/LICENSE.txt
--rw-r--r--   0 maarten    (501) staff       (20)     2699 2021-10-21 14:15:58.000000 pcrunner-1.0.2/Makefile
--rw-r--r--   0 maarten    (501) staff       (20)     2982 2023-04-01 17:45:01.193513 pcrunner-1.0.2/PKG-INFO
--rw-r--r--   0 maarten    (501) staff       (20)     1861 2021-10-21 13:00:44.000000 pcrunner-1.0.2/README.rst
-drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-04-01 17:45:01.184081 pcrunner-1.0.2/docs/
--rw-r--r--   0 maarten    (501) staff       (20)      634 2021-10-21 13:00:44.000000 pcrunner-1.0.2/docs/Makefile
-drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-04-01 17:45:01.184363 pcrunner-1.0.2/docs/_static/
--rw-r--r--   0 maarten    (501) staff       (20)       14 2020-03-20 14:50:09.000000 pcrunner-1.0.2/docs/_static/.gitignore
--rw-r--r--   0 maarten    (501) staff       (20)     2196 2023-04-01 17:13:39.000000 pcrunner-1.0.2/docs/conf.py
--rw-r--r--   0 maarten    (501) staff       (20)       28 2021-10-21 13:00:44.000000 pcrunner-1.0.2/docs/history.rst
--rw-r--r--   0 maarten    (501) staff       (20)      529 2021-10-21 18:48:37.000000 pcrunner-1.0.2/docs/index.rst
--rw-r--r--   0 maarten    (501) staff       (20)      250 2021-10-21 13:00:44.000000 pcrunner-1.0.2/docs/installation.rst
--rw-r--r--   0 maarten    (501) staff       (20)       61 2021-10-21 13:00:44.000000 pcrunner-1.0.2/docs/modules.rst
--rw-r--r--   0 maarten    (501) staff       (20)     1030 2021-10-21 14:15:58.000000 pcrunner-1.0.2/docs/pcrunner.rst
--rw-r--r--   0 maarten    (501) staff       (20)       52 2021-10-21 13:00:44.000000 pcrunner-1.0.2/docs/requirements.txt
--rw-r--r--   0 maarten    (501) staff       (20)     4798 2021-10-21 13:00:44.000000 pcrunner-1.0.2/docs/usage.rst
--rw-r--r--   0 maarten    (501) staff       (20)     1025 2023-04-01 17:16:50.000000 pcrunner-1.0.2/pyproject.toml
--rw-r--r--   0 maarten    (501) staff       (20)     1620 2023-04-01 17:45:01.194280 pcrunner-1.0.2/setup.cfg
--rw-r--r--   0 maarten    (501) staff       (20)      100 2023-04-01 16:56:53.000000 pcrunner-1.0.2/setup.py
-drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-04-01 17:45:01.176571 pcrunner-1.0.2/src/
-drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-04-01 17:45:01.186365 pcrunner-1.0.2/src/pcrunner/
--rw-r--r--   0 maarten    (501) staff       (20)      403 2023-04-01 16:56:53.000000 pcrunner-1.0.2/src/pcrunner/__init__.py
--rw-r--r--   0 maarten    (501) staff       (20)     5182 2023-04-01 16:56:53.000000 pcrunner-1.0.2/src/pcrunner/configuration.py
--rw-r--r--   0 maarten    (501) staff       (20)     3457 2023-04-01 16:56:53.000000 pcrunner-1.0.2/src/pcrunner/daemon.py
-drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-04-01 17:45:01.189317 pcrunner-1.0.2/src/pcrunner/data/
--rw-r--r--   0 maarten    (501) staff       (20)        0 2021-10-21 13:00:44.000000 pcrunner-1.0.2/src/pcrunner/data/empty
-drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-04-01 17:45:01.190201 pcrunner-1.0.2/src/pcrunner/etc/
--rw-r--r--   0 maarten    (501) staff       (20)      740 2021-10-21 13:00:44.000000 pcrunner-1.0.2/src/pcrunner/etc/commands.txt
--rw-r--r--   0 maarten    (501) staff       (20)     1792 2021-10-21 13:00:44.000000 pcrunner-1.0.2/src/pcrunner/etc/commands.yml
--rw-r--r--   0 maarten    (501) staff       (20)     1820 2021-10-21 13:00:44.000000 pcrunner-1.0.2/src/pcrunner/etc/pcrunner.yml
--rw-r--r--   0 maarten    (501) staff       (20)      648 2023-04-01 16:56:53.000000 pcrunner-1.0.2/src/pcrunner/exception.py
-drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-04-01 17:45:01.190671 pcrunner-1.0.2/src/pcrunner/init/
--rwxr-xr-x   0 maarten    (501) staff       (20)     1171 2021-10-21 13:00:44.000000 pcrunner-1.0.2/src/pcrunner/init/pcrunner
--rw-r--r--   0 maarten    (501) staff       (20)    32066 2023-04-01 17:13:39.000000 pcrunner-1.0.2/src/pcrunner/main.py
-drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-04-01 17:45:01.191851 pcrunner-1.0.2/src/pcrunner/scripts/
--rwxr-xr-x   0 maarten    (501) staff       (20)     1217 2023-04-01 17:10:55.000000 pcrunner-1.0.2/src/pcrunner/scripts/check_dummy.py
--rwxr-xr-x   0 maarten    (501) staff       (20)       64 2021-10-21 18:48:37.000000 pcrunner-1.0.2/src/pcrunner/scripts/pcr.py
--rwxr-xr-x   0 maarten    (501) staff       (20)     4416 2023-04-01 17:13:39.000000 pcrunner-1.0.2/src/pcrunner/scripts/run_check.py
-drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-04-01 17:45:01.192284 pcrunner-1.0.2/src/pcrunner/systemd/
--rw-r--r--   0 maarten    (501) staff       (20)      231 2021-10-21 13:00:44.000000 pcrunner-1.0.2/src/pcrunner/systemd/pcrunner.service
--rw-r--r--   0 maarten    (501) staff       (20)     3026 2023-04-01 16:56:53.000000 pcrunner-1.0.2/src/pcrunner/windows_service.py
-drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-04-01 17:45:01.188879 pcrunner-1.0.2/src/pcrunner.egg-info/
--rw-r--r--   0 maarten    (501) staff       (20)     2982 2023-04-01 17:45:01.000000 pcrunner-1.0.2/src/pcrunner.egg-info/PKG-INFO
--rw-r--r--   0 maarten    (501) staff       (20)     1100 2023-04-01 17:45:01.000000 pcrunner-1.0.2/src/pcrunner.egg-info/SOURCES.txt
--rw-r--r--   0 maarten    (501) staff       (20)        1 2023-04-01 17:45:01.000000 pcrunner-1.0.2/src/pcrunner.egg-info/dependency_links.txt
--rw-r--r--   0 maarten    (501) staff       (20)       48 2023-04-01 17:45:01.000000 pcrunner-1.0.2/src/pcrunner.egg-info/entry_points.txt
--rw-r--r--   0 maarten    (501) staff       (20)        1 2023-04-01 17:43:42.000000 pcrunner-1.0.2/src/pcrunner.egg-info/not-zip-safe
--rw-r--r--   0 maarten    (501) staff       (20)      166 2023-04-01 17:45:01.000000 pcrunner-1.0.2/src/pcrunner.egg-info/requires.txt
--rw-r--r--   0 maarten    (501) staff       (20)        9 2023-04-01 17:45:01.000000 pcrunner-1.0.2/src/pcrunner.egg-info/top_level.txt
-drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-04-01 17:45:01.193077 pcrunner-1.0.2/tests/
--rw-r--r--   0 maarten    (501) staff       (20)        0 2020-03-20 14:50:09.000000 pcrunner-1.0.2/tests/__init__.py
--rw-r--r--   0 maarten    (501) staff       (20)     1534 2023-04-01 16:56:53.000000 pcrunner-1.0.2/tests/test_configuration.py
--rw-r--r--   0 maarten    (501) staff       (20)     7598 2023-04-01 17:14:48.000000 pcrunner-1.0.2/tests/test_main.py
--rw-r--r--   0 maarten    (501) staff       (20)      587 2023-04-01 17:34:19.000000 pcrunner-1.0.2/tox.ini
+drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-05-23 14:18:42.251278 pcrunner-1.0.3/
+-rw-r--r--   0 maarten    (501) staff       (20)      216 2021-10-21 13:00:44.000000 pcrunner-1.0.3/.flake8
+drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-05-23 14:18:42.233197 pcrunner-1.0.3/.github/
+drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-05-23 14:18:42.239734 pcrunner-1.0.3/.github/workflows/
+-rw-r--r--   0 maarten    (501) staff       (20)     1471 2023-04-01 17:33:35.000000 pcrunner-1.0.3/.github/workflows/ci.yml
+-rw-r--r--   0 maarten    (501) staff       (20)     2482 2023-05-23 14:13:55.000000 pcrunner-1.0.3/.gitignore
+-rw-r--r--   0 maarten    (501) staff       (20)      954 2023-04-01 17:16:32.000000 pcrunner-1.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 maarten    (501) staff       (20)        9 2023-05-23 14:13:59.000000 pcrunner-1.0.3/.python-version
+-rw-r--r--   0 maarten    (501) staff       (20)      499 2021-10-21 13:00:44.000000 pcrunner-1.0.3/.readthedocs.yaml
+-rw-r--r--   0 maarten    (501) staff       (20)     3557 2021-10-21 18:48:37.000000 pcrunner-1.0.3/HISTORY.rst
+-rw-r--r--   0 maarten    (501) staff       (20)      762 2021-10-21 18:48:37.000000 pcrunner-1.0.3/LICENSE.txt
+-rw-r--r--   0 maarten    (501) staff       (20)     2699 2021-10-21 14:15:58.000000 pcrunner-1.0.3/Makefile
+-rw-r--r--   0 maarten    (501) staff       (20)     2982 2023-05-23 14:18:42.251477 pcrunner-1.0.3/PKG-INFO
+-rw-r--r--   0 maarten    (501) staff       (20)     1861 2021-10-21 13:00:44.000000 pcrunner-1.0.3/README.rst
+drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-05-23 14:18:42.243223 pcrunner-1.0.3/docs/
+-rw-r--r--   0 maarten    (501) staff       (20)      634 2021-10-21 13:00:44.000000 pcrunner-1.0.3/docs/Makefile
+drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-05-23 14:18:42.243588 pcrunner-1.0.3/docs/_static/
+-rw-r--r--   0 maarten    (501) staff       (20)       14 2020-03-20 14:50:09.000000 pcrunner-1.0.3/docs/_static/.gitignore
+-rw-r--r--   0 maarten    (501) staff       (20)     2196 2023-04-01 17:13:39.000000 pcrunner-1.0.3/docs/conf.py
+-rw-r--r--   0 maarten    (501) staff       (20)       28 2021-10-21 13:00:44.000000 pcrunner-1.0.3/docs/history.rst
+-rw-r--r--   0 maarten    (501) staff       (20)      529 2021-10-21 18:48:37.000000 pcrunner-1.0.3/docs/index.rst
+-rw-r--r--   0 maarten    (501) staff       (20)      250 2021-10-21 13:00:44.000000 pcrunner-1.0.3/docs/installation.rst
+-rw-r--r--   0 maarten    (501) staff       (20)       61 2021-10-21 13:00:44.000000 pcrunner-1.0.3/docs/modules.rst
+-rw-r--r--   0 maarten    (501) staff       (20)     1030 2021-10-21 14:15:58.000000 pcrunner-1.0.3/docs/pcrunner.rst
+-rw-r--r--   0 maarten    (501) staff       (20)       52 2021-10-21 13:00:44.000000 pcrunner-1.0.3/docs/requirements.txt
+-rw-r--r--   0 maarten    (501) staff       (20)     4798 2021-10-21 13:00:44.000000 pcrunner-1.0.3/docs/usage.rst
+-rw-r--r--   0 maarten    (501) staff       (20)     1025 2023-04-01 17:16:50.000000 pcrunner-1.0.3/pyproject.toml
+-rw-r--r--   0 maarten    (501) staff       (20)     1620 2023-05-23 14:18:42.252371 pcrunner-1.0.3/setup.cfg
+-rw-r--r--   0 maarten    (501) staff       (20)      100 2023-04-01 16:56:53.000000 pcrunner-1.0.3/setup.py
+drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-05-23 14:18:42.233892 pcrunner-1.0.3/src/
+drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-05-23 14:18:42.245769 pcrunner-1.0.3/src/pcrunner/
+-rw-r--r--   0 maarten    (501) staff       (20)      403 2023-04-01 16:56:53.000000 pcrunner-1.0.3/src/pcrunner/__init__.py
+-rw-r--r--   0 maarten    (501) staff       (20)     5182 2023-04-01 16:56:53.000000 pcrunner-1.0.3/src/pcrunner/configuration.py
+-rw-r--r--   0 maarten    (501) staff       (20)     3457 2023-04-01 16:56:53.000000 pcrunner-1.0.3/src/pcrunner/daemon.py
+drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-05-23 14:18:42.248069 pcrunner-1.0.3/src/pcrunner/data/
+-rw-r--r--   0 maarten    (501) staff       (20)        0 2021-10-21 13:00:44.000000 pcrunner-1.0.3/src/pcrunner/data/empty
+drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-05-23 14:18:42.248856 pcrunner-1.0.3/src/pcrunner/etc/
+-rw-r--r--   0 maarten    (501) staff       (20)      740 2021-10-21 13:00:44.000000 pcrunner-1.0.3/src/pcrunner/etc/commands.txt
+-rw-r--r--   0 maarten    (501) staff       (20)     1792 2021-10-21 13:00:44.000000 pcrunner-1.0.3/src/pcrunner/etc/commands.yml
+-rw-r--r--   0 maarten    (501) staff       (20)     1820 2021-10-21 13:00:44.000000 pcrunner-1.0.3/src/pcrunner/etc/pcrunner.yml
+-rw-r--r--   0 maarten    (501) staff       (20)      648 2023-04-01 16:56:53.000000 pcrunner-1.0.3/src/pcrunner/exception.py
+drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-05-23 14:18:42.249138 pcrunner-1.0.3/src/pcrunner/init/
+-rwxr-xr-x   0 maarten    (501) staff       (20)     1171 2021-10-21 13:00:44.000000 pcrunner-1.0.3/src/pcrunner/init/pcrunner
+-rw-r--r--   0 maarten    (501) staff       (20)    32074 2023-05-23 14:02:10.000000 pcrunner-1.0.3/src/pcrunner/main.py
+drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-05-23 14:18:42.249980 pcrunner-1.0.3/src/pcrunner/scripts/
+-rwxr-xr-x   0 maarten    (501) staff       (20)     1217 2023-04-01 17:10:55.000000 pcrunner-1.0.3/src/pcrunner/scripts/check_dummy.py
+-rwxr-xr-x   0 maarten    (501) staff       (20)       64 2021-10-21 18:48:37.000000 pcrunner-1.0.3/src/pcrunner/scripts/pcr.py
+-rwxr-xr-x   0 maarten    (501) staff       (20)     4416 2023-04-01 17:13:39.000000 pcrunner-1.0.3/src/pcrunner/scripts/run_check.py
+drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-05-23 14:18:42.250262 pcrunner-1.0.3/src/pcrunner/systemd/
+-rw-r--r--   0 maarten    (501) staff       (20)      231 2021-10-21 13:00:44.000000 pcrunner-1.0.3/src/pcrunner/systemd/pcrunner.service
+-rw-r--r--   0 maarten    (501) staff       (20)     3026 2023-04-01 16:56:53.000000 pcrunner-1.0.3/src/pcrunner/windows_service.py
+drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-05-23 14:18:42.247791 pcrunner-1.0.3/src/pcrunner.egg-info/
+-rw-r--r--   0 maarten    (501) staff       (20)     2982 2023-05-23 14:18:42.000000 pcrunner-1.0.3/src/pcrunner.egg-info/PKG-INFO
+-rw-r--r--   0 maarten    (501) staff       (20)     1116 2023-05-23 14:18:42.000000 pcrunner-1.0.3/src/pcrunner.egg-info/SOURCES.txt
+-rw-r--r--   0 maarten    (501) staff       (20)        1 2023-05-23 14:18:42.000000 pcrunner-1.0.3/src/pcrunner.egg-info/dependency_links.txt
+-rw-r--r--   0 maarten    (501) staff       (20)       48 2023-05-23 14:18:42.000000 pcrunner-1.0.3/src/pcrunner.egg-info/entry_points.txt
+-rw-r--r--   0 maarten    (501) staff       (20)        1 2023-05-23 14:17:23.000000 pcrunner-1.0.3/src/pcrunner.egg-info/not-zip-safe
+-rw-r--r--   0 maarten    (501) staff       (20)      166 2023-05-23 14:18:42.000000 pcrunner-1.0.3/src/pcrunner.egg-info/requires.txt
+-rw-r--r--   0 maarten    (501) staff       (20)        9 2023-05-23 14:18:42.000000 pcrunner-1.0.3/src/pcrunner.egg-info/top_level.txt
+drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-05-23 14:18:42.251033 pcrunner-1.0.3/tests/
+-rw-r--r--   0 maarten    (501) staff       (20)        0 2020-03-20 14:50:09.000000 pcrunner-1.0.3/tests/__init__.py
+-rw-r--r--   0 maarten    (501) staff       (20)     1534 2023-04-01 16:56:53.000000 pcrunner-1.0.3/tests/test_configuration.py
+-rw-r--r--   0 maarten    (501) staff       (20)     7598 2023-04-01 17:14:48.000000 pcrunner-1.0.3/tests/test_main.py
+-rw-r--r--   0 maarten    (501) staff       (20)      587 2023-04-01 17:34:19.000000 pcrunner-1.0.3/tox.ini
```

### Comparing `pcrunner-1.0.2/.github/workflows/ci.yml` & `pcrunner-1.0.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pcrunner-1.0.2/.gitignore` & `pcrunner-1.0.3/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 # IPython
 profile_default/
 ipython_config.py
 
 # pyenv
 #   For a library or package, you might want to ignore these files since the code is
 #   intended to run in multiple environments; otherwise, check them in:
-.python-version
+# .python-version
 
 # pipenv
 #   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
 #   However, in case of collaboration, if having platform-specific dependencies or dependencies
 #   having no cross-platform support, pipenv may install dependencies that don't work, or not
 #   install all needed dependencies.
 Pipfile.lock
```

### Comparing `pcrunner-1.0.2/.pre-commit-config.yaml` & `pcrunner-1.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pcrunner-1.0.2/HISTORY.rst` & `pcrunner-1.0.3/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `pcrunner-1.0.2/LICENSE.txt` & `pcrunner-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pcrunner-1.0.2/Makefile` & `pcrunner-1.0.3/Makefile`

 * *Files identical despite different names*

### Comparing `pcrunner-1.0.2/PKG-INFO` & `pcrunner-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcrunner
-Version: 1.0.2
+Version: 1.0.3
 Summary: A module for running Passive Nagios/Icinga Checks
 Home-page: https://github.com/maartenq/pcrunner
 Author: Maarten
 Author-email: ikmaarten@gmail.com
 License: ISC
 Project-URL: Bug Tracker, https://github.com/maartenq/pcrunner/issues
 Project-URL: Changelog, https://github.com/maartenq/pcrunner/blob/main/HISTORY.rst
```

### Comparing `pcrunner-1.0.2/README.rst` & `pcrunner-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `pcrunner-1.0.2/docs/Makefile` & `pcrunner-1.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pcrunner-1.0.2/docs/conf.py` & `pcrunner-1.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pcrunner-1.0.2/docs/index.rst` & `pcrunner-1.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pcrunner-1.0.2/docs/pcrunner.rst` & `pcrunner-1.0.3/docs/pcrunner.rst`

 * *Files identical despite different names*

### Comparing `pcrunner-1.0.2/docs/usage.rst` & `pcrunner-1.0.3/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `pcrunner-1.0.2/pyproject.toml` & `pcrunner-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pcrunner-1.0.2/setup.cfg` & `pcrunner-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `pcrunner-1.0.2/src/pcrunner/configuration.py` & `pcrunner-1.0.3/src/pcrunner/configuration.py`

 * *Files identical despite different names*

### Comparing `pcrunner-1.0.2/src/pcrunner/daemon.py` & `pcrunner-1.0.3/src/pcrunner/daemon.py`

 * *Files identical despite different names*

### Comparing `pcrunner-1.0.2/src/pcrunner/etc/commands.txt` & `pcrunner-1.0.3/src/pcrunner/etc/commands.txt`

 * *Files identical despite different names*

### Comparing `pcrunner-1.0.2/src/pcrunner/etc/commands.yml` & `pcrunner-1.0.3/src/pcrunner/etc/commands.yml`

 * *Files identical despite different names*

### Comparing `pcrunner-1.0.2/src/pcrunner/etc/pcrunner.yml` & `pcrunner-1.0.3/src/pcrunner/etc/pcrunner.yml`

 * *Files identical despite different names*

### Comparing `pcrunner-1.0.2/src/pcrunner/exception.py` & `pcrunner-1.0.3/src/pcrunner/exception.py`

 * *Files identical despite different names*

### Comparing `pcrunner-1.0.2/src/pcrunner/init/pcrunner` & `pcrunner-1.0.3/src/pcrunner/init/pcrunner`

 * *Files identical despite different names*

### Comparing `pcrunner-1.0.2/src/pcrunner/main.py` & `pcrunner-1.0.3/src/pcrunner/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,16 +117,16 @@
                 # check got terminated
                 self.status_code = 3
                 self.stdout = ''
                 self.stderr = 'terminated, max time reached'
                 logger.error('check %s: %s ', self.name, self.stderr)
             else:
                 self.status_code = self.process.returncode
-                self.stdout = ' '.join(str(stdout).splitlines())
-                self.stderr = ' '.join(str(stderr).splitlines())
+                self.stdout = ' '.join(stdout.decode().splitlines())
+                self.stderr = ' '.join(stderr.decode().splitlines())
 
                 logger.debug(
                     'check %s: finished: PID: %d  return code %d',
                     self.name,
                     self.pid,
                     self.status_code,
                 )
```

### Comparing `pcrunner-1.0.2/src/pcrunner/scripts/check_dummy.py` & `pcrunner-1.0.3/src/pcrunner/scripts/check_dummy.py`

 * *Files identical despite different names*

### Comparing `pcrunner-1.0.2/src/pcrunner/scripts/run_check.py` & `pcrunner-1.0.3/src/pcrunner/scripts/run_check.py`

 * *Files identical despite different names*

### Comparing `pcrunner-1.0.2/src/pcrunner/windows_service.py` & `pcrunner-1.0.3/src/pcrunner/windows_service.py`

 * *Files identical despite different names*

### Comparing `pcrunner-1.0.2/src/pcrunner.egg-info/PKG-INFO` & `pcrunner-1.0.3/src/pcrunner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcrunner
-Version: 1.0.2
+Version: 1.0.3
 Summary: A module for running Passive Nagios/Icinga Checks
 Home-page: https://github.com/maartenq/pcrunner
 Author: Maarten
 Author-email: ikmaarten@gmail.com
 License: ISC
 Project-URL: Bug Tracker, https://github.com/maartenq/pcrunner/issues
 Project-URL: Changelog, https://github.com/maartenq/pcrunner/blob/main/HISTORY.rst
```

### Comparing `pcrunner-1.0.2/src/pcrunner.egg-info/SOURCES.txt` & `pcrunner-1.0.3/src/pcrunner.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 .flake8
 .gitignore
 .pre-commit-config.yaml
+.python-version
 .readthedocs.yaml
 HISTORY.rst
 LICENSE.txt
 Makefile
 README.rst
 pyproject.toml
 setup.cfg
```

### Comparing `pcrunner-1.0.2/tests/test_configuration.py` & `pcrunner-1.0.3/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `pcrunner-1.0.2/tests/test_main.py` & `pcrunner-1.0.3/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pcrunner-1.0.2/tox.ini` & `pcrunner-1.0.3/tox.ini`

 * *Files identical despite different names*

