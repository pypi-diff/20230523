# Comparing `tmp/ghga_service_commons-0.3.0.tar.gz` & `tmp/ghga_service_commons-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghga_service_commons-0.3.0.tar", last modified: Tue May  2 10:52:30 2023, max compression
+gzip compressed data, was "ghga_service_commons-0.3.1.tar", last modified: Tue May 23 12:17:43 2023, max compression
```

## Comparing `ghga_service_commons-0.3.0.tar` & `ghga_service_commons-0.3.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:52:30.892847 ghga_service_commons-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-05-02 10:52:30.892847 ghga_service_commons-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:52:30.884847 ghga_service_commons-0.3.0/ghga_service_commons/
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/ghga_service_commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/ghga_service_commons/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:52:30.888847 ghga_service_commons-0.3.0/ghga_service_commons/api/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/ghga_service_commons/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/ghga_service_commons/api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/ghga_service_commons/api/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:52:30.888847 ghga_service_commons-0.3.0/ghga_service_commons/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/ghga_service_commons/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/ghga_service_commons/auth/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/ghga_service_commons/auth/ghga.py
--rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/ghga_service_commons/auth/jwt_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/ghga_service_commons/auth/policies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:52:30.888847 ghga_service_commons-0.3.0/ghga_service_commons/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/ghga_service_commons/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/ghga_service_commons/utils/crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/ghga_service_commons/utils/jwt_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/ghga_service_commons/utils/temp_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/ghga_service_commons/utils/utc_dates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:52:30.888847 ghga_service_commons-0.3.0/ghga_service_commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-05-02 10:52:30.000000 ghga_service_commons-0.3.0/ghga_service_commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-02 10:52:30.000000 ghga_service_commons-0.3.0/ghga_service_commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 10:52:30.000000 ghga_service_commons-0.3.0/ghga_service_commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-02 10:52:30.000000 ghga_service_commons-0.3.0/ghga_service_commons.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 10:52:30.000000 ghga_service_commons-0.3.0/ghga_service_commons.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-02 10:52:30.000000 ghga_service_commons-0.3.0/ghga_service_commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-02 10:52:30.000000 ghga_service_commons-0.3.0/ghga_service_commons.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-02 10:52:30.892847 ghga_service_commons-0.3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:52:30.884847 ghga_service_commons-0.3.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:52:30.888847 ghga_service_commons-0.3.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/tests/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:52:30.888847 ghga_service_commons-0.3.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:52:30.888847 ghga_service_commons-0.3.0/tests/integration/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/tests/integration/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/tests/integration/fixtures/hello_world_test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/tests/integration/fixtures/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/tests/integration/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:52:30.888847 ghga_service_commons-0.3.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:52:30.888847 ghga_service_commons-0.3.0/tests/unit/api/
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/tests/unit/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/tests/unit/api/test_testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:52:30.888847 ghga_service_commons-0.3.0/tests/unit/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/tests/unit/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/tests/unit/auth/test_ghga.py
--rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/tests/unit/auth/test_jwt_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/tests/unit/auth/test_policies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:52:30.888847 ghga_service_commons-0.3.0/tests/unit/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/tests/unit/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/tests/unit/fixtures/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:52:30.892847 ghga_service_commons-0.3.0/tests/unit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/tests/unit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/tests/unit/utils/test_crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/tests/unit/utils/test_jwt_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/tests/unit/utils/test_temp_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-05-02 10:52:19.000000 ghga_service_commons-0.3.0/tests/unit/utils/test_utc_dates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:17:43.579584 ghga_service_commons-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-05-23 12:17:43.579584 ghga_service_commons-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:17:43.563584 ghga_service_commons-0.3.1/ghga_service_commons/
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/ghga_service_commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/ghga_service_commons/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:17:43.567584 ghga_service_commons-0.3.1/ghga_service_commons/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/ghga_service_commons/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/ghga_service_commons/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/ghga_service_commons/api/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:17:43.571584 ghga_service_commons-0.3.1/ghga_service_commons/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/ghga_service_commons/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/ghga_service_commons/auth/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/ghga_service_commons/auth/ghga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/ghga_service_commons/auth/jwt_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/ghga_service_commons/auth/policies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:17:43.571584 ghga_service_commons-0.3.1/ghga_service_commons/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/ghga_service_commons/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/ghga_service_commons/utils/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/ghga_service_commons/utils/jwt_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/ghga_service_commons/utils/temp_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/ghga_service_commons/utils/utc_dates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:17:43.567584 ghga_service_commons-0.3.1/ghga_service_commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-05-23 12:17:43.000000 ghga_service_commons-0.3.1/ghga_service_commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-23 12:17:43.000000 ghga_service_commons-0.3.1/ghga_service_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 12:17:43.000000 ghga_service_commons-0.3.1/ghga_service_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-23 12:17:43.000000 ghga_service_commons-0.3.1/ghga_service_commons.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 12:17:43.000000 ghga_service_commons-0.3.1/ghga_service_commons.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-23 12:17:43.000000 ghga_service_commons-0.3.1/ghga_service_commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-23 12:17:43.000000 ghga_service_commons-0.3.1/ghga_service_commons.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-23 12:17:43.583584 ghga_service_commons-0.3.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:17:43.559584 ghga_service_commons-0.3.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:17:43.571584 ghga_service_commons-0.3.1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/tests/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:17:43.571584 ghga_service_commons-0.3.1/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:17:43.575584 ghga_service_commons-0.3.1/tests/integration/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/tests/integration/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/tests/integration/fixtures/hello_world_test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/tests/integration/fixtures/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/tests/integration/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:17:43.575584 ghga_service_commons-0.3.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:17:43.575584 ghga_service_commons-0.3.1/tests/unit/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/tests/unit/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/tests/unit/api/test_testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:17:43.575584 ghga_service_commons-0.3.1/tests/unit/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/tests/unit/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/tests/unit/auth/test_ghga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/tests/unit/auth/test_jwt_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/tests/unit/auth/test_policies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:17:43.579584 ghga_service_commons-0.3.1/tests/unit/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/tests/unit/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/tests/unit/fixtures/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:17:43.579584 ghga_service_commons-0.3.1/tests/unit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/tests/unit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/tests/unit/utils/test_crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/tests/unit/utils/test_jwt_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/tests/unit/utils/test_temp_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-05-23 12:17:28.000000 ghga_service_commons-0.3.1/tests/unit/utils/test_utc_dates.py
```

### Comparing `ghga_service_commons-0.3.0/LICENSE` & `ghga_service_commons-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-0.3.0/PKG-INFO` & `ghga_service_commons-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghga_service_commons
-Version: 0.3.0
+Version: 0.3.1
 Summary: A library that contains common functionality used in services of GHGA
 Home-page: https://github.com/ghga-de/ghga-service-commons
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ghga_service_commons-0.3.0/README.md` & `ghga_service_commons-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-0.3.0/ghga_service_commons/__init__.py` & `ghga_service_commons-0.3.1/ghga_service_commons/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """A library that contains the common functionality used in services of GHGA"""
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
```

### Comparing `ghga_service_commons-0.3.0/ghga_service_commons/__main__.py` & `ghga_service_commons-0.3.1/ghga_service_commons/__main__.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-0.3.0/ghga_service_commons/api/__init__.py` & `ghga_service_commons-0.3.1/ghga_service_commons/api/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-0.3.0/ghga_service_commons/api/api.py` & `ghga_service_commons-0.3.1/ghga_service_commons/api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,22 +12,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Functionality for initializing, configuring, and running RESTful
 webapps with FastAPI"""
 
-from typing import Dict, Literal, Optional, Sequence, Union
+from typing import Dict, Optional, Sequence, Union
 
 import uvicorn
 from fastapi import FastAPI
 from fastapi.middleware.cors import CORSMiddleware
 from httpyexpect.server.handlers.fastapi_ import configure_exception_handler
 from pydantic import BaseSettings, Field
 
+try:  # workaround for https://github.com/pydantic/pydantic/issues/5821
+    from typing_extensions import Literal
+except ImportError:
+    from typing import Literal  # type: ignore
+
 # type alias for log level parameter
 LogLevel = Literal["critical", "error", "warning", "info", "debug", "trace"]
 
 
 class ApiConfigBase(BaseSettings):
     """A base class with API-required config params.
     Inherit your config class from this class if you need
```

### Comparing `ghga_service_commons-0.3.0/ghga_service_commons/api/testing.py` & `ghga_service_commons-0.3.1/ghga_service_commons/api/testing.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-0.3.0/ghga_service_commons/auth/__init__.py` & `ghga_service_commons-0.3.1/ghga_service_commons/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-0.3.0/ghga_service_commons/auth/context.py` & `ghga_service_commons-0.3.1/ghga_service_commons/auth/context.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-0.3.0/ghga_service_commons/auth/ghga.py` & `ghga_service_commons-0.3.1/ghga_service_commons/auth/ghga.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-0.3.0/ghga_service_commons/auth/jwt_auth.py` & `ghga_service_commons-0.3.1/ghga_service_commons/auth/jwt_auth.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-0.3.0/ghga_service_commons/auth/policies.py` & `ghga_service_commons-0.3.1/ghga_service_commons/auth/policies.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-0.3.0/ghga_service_commons/utils/__init__.py` & `ghga_service_commons-0.3.1/ghga_service_commons/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-0.3.0/ghga_service_commons/utils/crypt.py` & `ghga_service_commons-0.3.1/ghga_service_commons/utils/crypt.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-0.3.0/ghga_service_commons/utils/jwt_helpers.py` & `ghga_service_commons-0.3.1/ghga_service_commons/utils/jwt_helpers.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-0.3.0/ghga_service_commons/utils/temp_files.py` & `ghga_service_commons-0.3.1/ghga_service_commons/utils/temp_files.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-0.3.0/ghga_service_commons/utils/utc_dates.py` & `ghga_service_commons-0.3.1/ghga_service_commons/utils/utc_dates.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-0.3.0/ghga_service_commons.egg-info/PKG-INFO` & `ghga_service_commons-0.3.1/ghga_service_commons.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghga-service-commons
-Version: 0.3.0
+Version: 0.3.1
 Summary: A library that contains common functionality used in services of GHGA
 Home-page: https://github.com/ghga-de/ghga-service-commons
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ghga_service_commons-0.3.0/ghga_service_commons.egg-info/SOURCES.txt` & `ghga_service_commons-0.3.1/ghga_service_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-0.3.0/setup.cfg` & `ghga_service_commons-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-0.3.0/setup.py` & `ghga_service_commons-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-0.3.0/tests/fixtures/__init__.py` & `ghga_service_commons-0.3.1/tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-0.3.0/tests/integration/__init__.py` & `ghga_service_commons-0.3.1/tests/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-0.3.0/tests/integration/fixtures/__init__.py` & `ghga_service_commons-0.3.1/tests/integration/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-0.3.0/tests/integration/fixtures/hello_world_test_app.py` & `ghga_service_commons-0.3.1/tests/integration/fixtures/hello_world_test_app.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-0.3.0/tests/integration/fixtures/utils.py` & `ghga_service_commons-0.3.1/tests/integration/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-0.3.0/tests/integration/test_api.py` & `ghga_service_commons-0.3.1/tests/integration/test_api.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-0.3.0/tests/unit/__init__.py` & `ghga_service_commons-0.3.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-0.3.0/tests/unit/api/__init__.py` & `ghga_service_commons-0.3.1/tests/unit/api/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-0.3.0/tests/unit/api/test_testing.py` & `ghga_service_commons-0.3.1/tests/unit/api/test_testing.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-0.3.0/tests/unit/auth/__init__.py` & `ghga_service_commons-0.3.1/tests/unit/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-0.3.0/tests/unit/auth/test_ghga.py` & `ghga_service_commons-0.3.1/tests/unit/auth/test_ghga.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-0.3.0/tests/unit/auth/test_jwt_auth.py` & `ghga_service_commons-0.3.1/tests/unit/auth/test_jwt_auth.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-0.3.0/tests/unit/auth/test_policies.py` & `ghga_service_commons-0.3.1/tests/unit/auth/test_policies.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-0.3.0/tests/unit/fixtures/__init__.py` & `ghga_service_commons-0.3.1/tests/unit/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-0.3.0/tests/unit/fixtures/utils.py` & `ghga_service_commons-0.3.1/tests/unit/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-0.3.0/tests/unit/utils/__init__.py` & `ghga_service_commons-0.3.1/tests/unit/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-0.3.0/tests/unit/utils/test_crypt.py` & `ghga_service_commons-0.3.1/tests/unit/utils/test_crypt.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-0.3.0/tests/unit/utils/test_jwt_helpers.py` & `ghga_service_commons-0.3.1/tests/unit/utils/test_jwt_helpers.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-0.3.0/tests/unit/utils/test_temp_files.py` & `ghga_service_commons-0.3.1/tests/unit/utils/test_temp_files.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-0.3.0/tests/unit/utils/test_utc_dates.py` & `ghga_service_commons-0.3.1/tests/unit/utils/test_utc_dates.py`

 * *Files identical despite different names*

