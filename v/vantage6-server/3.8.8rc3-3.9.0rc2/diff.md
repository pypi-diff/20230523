# Comparing `tmp/vantage6-server-3.8.8rc3.tar.gz` & `tmp/vantage6-server-3.9.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-server-3.8.8rc3.tar", last modified: Mon May 22 13:38:30 2023, max compression
+gzip compressed data, was "vantage6-server-3.9.0rc2.tar", last modified: Tue May  9 13:37:06 2023, max compression
```

## Comparing `vantage6-server-3.8.8rc3.tar` & `vantage6-server-3.9.0rc2.tar`

### file list

```diff
@@ -1,93 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:30.056137 vantage6-server-3.8.8rc3/
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-22 13:38:30.056137 vantage6-server-3.8.8rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 13:38:30.056137 vantage6-server-3.8.8rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:30.048138 vantage6-server-3.8.8rc3/tests_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/tests_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11685 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/tests_server/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)   100968 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/tests_server/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:30.044138 vantage6-server-3.8.8rc3/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:30.048138 vantage6-server-3.8.8rc3/vantage6/server/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/__build__
--rw-r--r--   0 runner    (1001) docker     (123)    22901 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:30.048138 vantage6-server-3.8.8rc3/vantage6/server/_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:30.048138 vantage6-server-3.8.8rc3/vantage6/server/_data/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/_data/dev/fixtures.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/_data/dev/node_a.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/_data/dev/node_b.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/_data/dev/server.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/_data/example_fixtures.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/_data/node_config_skeleton.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/_data/server_config_skeleton.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/_data/testnodeconfiguration.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/_data/unittest_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/_data/unittest_fixtures.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:30.048138 vantage6-server-3.8.8rc3/vantage6/server/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/cli/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:30.048138 vantage6-server-3.8.8rc3/vantage6/server/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/configuration/configuration_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/configuration/configuration_wizard.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:30.048138 vantage6-server-3.8.8rc3/vantage6/server/controller/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/controller/fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/controller/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/default_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/mail_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:30.052137 vantage6-server-3.8.8rc3/vantage6/server/model/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/model/algorithm_port.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/model/authenticatable.py
--rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/model/collaboration.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/model/member.py
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/model/node.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/model/node_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/model/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/model/permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/model/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/model/role.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/model/role_rule_association.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/model/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/model/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     9799 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/model/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    10485 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:30.052137 vantage6-server-3.8.8rc3/vantage6/server/resource/
--rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32446 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/resource/collaboration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:30.052137 vantage6-server-3.8.8rc3/vantage6/server/resource/common/
--rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/resource/common/_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/resource/common/auth_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/resource/common/swagger_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/resource/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/resource/health.py
--rw-r--r--   0 runner    (1001) docker     (123)    19180 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/resource/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    17265 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/resource/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/resource/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)    14322 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/resource/port.py
--rw-r--r--   0 runner    (1001) docker     (123)    18466 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/resource/recover.py
--rw-r--r--   0 runner    (1001) docker     (123)    12589 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/resource/result.py
--rw-r--r--   0 runner    (1001) docker     (123)    26264 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/resource/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/resource/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/resource/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    27653 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/resource/task.py
--rw-r--r--   0 runner    (1001) docker     (123)    12439 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/resource/token.py
--rw-r--r--   0 runner    (1001) docker     (123)    26416 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/resource/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/resource/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    19136 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/resource/vpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/resource/websocket_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/session.py
--rw-r--r--   0 runner    (1001) docker     (123)    13600 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/websockets.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-22 13:38:16.000000 vantage6-server-3.8.8rc3/vantage6/server/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:38:30.052137 vantage6-server-3.8.8rc3/vantage6_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-22 13:38:30.000000 vantage6-server-3.8.8rc3/vantage6_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-22 13:38:30.000000 vantage6-server-3.8.8rc3/vantage6_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 13:38:30.000000 vantage6-server-3.8.8rc3/vantage6_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-22 13:38:30.000000 vantage6-server-3.8.8rc3/vantage6_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-22 13:38:30.000000 vantage6-server-3.8.8rc3/vantage6_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-22 13:38:30.000000 vantage6-server-3.8.8rc3/vantage6_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:06.434940 vantage6-server-3.9.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-09 13:37:06.434940 vantage6-server-3.9.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 13:37:06.438941 vantage6-server-3.9.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:06.426940 vantage6-server-3.9.0rc2/tests_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/tests_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11685 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/tests_server/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100933 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/tests_server/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:06.426940 vantage6-server-3.9.0rc2/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:06.430940 vantage6-server-3.9.0rc2/vantage6/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/__build__
+-rw-r--r--   0 runner    (1001) docker     (123)    25332 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:06.430940 vantage6-server-3.9.0rc2/vantage6/server/_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:06.430940 vantage6-server-3.9.0rc2/vantage6/server/_data/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/_data/dev/fixtures.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/_data/dev/node_a.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/_data/dev/node_b.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/_data/dev/server.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/_data/example_fixtures.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/_data/node_config_skeleton.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/_data/server_config_skeleton.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/_data/testnodeconfiguration.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/_data/unittest_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/_data/unittest_fixtures.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:06.430940 vantage6-server-3.9.0rc2/vantage6/server/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10395 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/cli/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:06.430940 vantage6-server-3.9.0rc2/vantage6/server/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/controller/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/default_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/mail_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:06.434940 vantage6-server-3.9.0rc2/vantage6/server/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/model/algorithm_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/model/authenticatable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13359 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/model/collaboration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/model/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/model/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/model/node_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/model/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/model/permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/model/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/model/role_rule_association.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/model/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/model/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:06.434940 vantage6-server-3.9.0rc2/vantage6/server/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)     7543 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32446 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/collaboration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:06.434940 vantage6-server-3.9.0rc2/vantage6/server/resource/common/
+-rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/common/_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/common/auth_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/common/swagger_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/health.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19180 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17265 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16376 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18466 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/recover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12589 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26260 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27653 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12439 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26410 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19105 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/vpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/websocket_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14088 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/websockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:06.434940 vantage6-server-3.9.0rc2/vantage6_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-09 13:37:06.000000 vantage6-server-3.9.0rc2/vantage6_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-09 13:37:06.000000 vantage6-server-3.9.0rc2/vantage6_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:37:06.000000 vantage6-server-3.9.0rc2/vantage6_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-09 13:37:06.000000 vantage6-server-3.9.0rc2/vantage6_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-09 13:37:06.000000 vantage6-server-3.9.0rc2/vantage6_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-09 13:37:06.000000 vantage6-server-3.9.0rc2/vantage6_server.egg-info/top_level.txt
```

### Comparing `vantage6-server-3.8.8rc3/PKG-INFO` & `vantage6-server-3.9.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-server
-Version: 3.8.8rc3
+Version: 3.9.0rc2
 Summary: Vantage6 server
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-server Version: 3.8.8rc3 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-server Version: 3.9.0rc2 Summary: Vantage6
 server Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-server-3.8.8rc3/setup.py` & `vantage6-server-3.9.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.8rc3/tests_server/test_models.py` & `vantage6-server-3.9.0rc2/tests_server/test_models.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.8rc3/tests_server/test_resources.py` & `vantage6-server-3.9.0rc2/tests_server/test_resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,16 +48,15 @@
 class TestResources(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls):
         """Called immediately before running a test method."""
         Database().connect("sqlite://", allow_drop_all=True)
 
-        ctx = context.TestContext.from_external_config_file(
-            "unittest_config.yaml")
+        ctx = context.TestContext.from_external_config_file()
 
         # create server instance. Patch the start_background_task method
         # to prevent the server from starting a ping/pong thread that will
         # prevent the tests from starting
         with patch.object(SocketIO, 'start_background_task'):
             server = ServerApp(ctx)
         cls.server = server
```

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/__init__.py` & `vantage6-server-3.9.0rc2/vantage6/server/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,19 +16,21 @@
 import os
 import uuid
 import json
 import time
 import datetime as dt
 import traceback
 
+from typing import Any
 from http import HTTPStatus
 from werkzeug.exceptions import HTTPException
 from flasgger import Swagger
 from flask import (
-    Flask, make_response, current_app, request, send_from_directory, Request
+    Flask, make_response, current_app, request, send_from_directory, Request,
+    Response
 )
 from flask_cors import CORS
 from flask_jwt_extended import JWTManager
 from flask_marshmallow import Marshmallow
 from flask_restful import Api
 from flask_mail import Mail
 from flask_principal import Principal, Identity, identity_changed
@@ -71,15 +73,15 @@
 
     Attributes
     ----------
     ctx : ServerContext
         Context object that contains the configuration of the server.
     """
 
-    def __init__(self, ctx: ServerContext):
+    def __init__(self, ctx: ServerContext) -> None:
         """Create a vantage6-server application."""
 
         self.ctx = ctx
 
         # initialize, configure Flask
         self.app = Flask(APPNAME, root_path=os.path.dirname(__file__))
         self.configure_flask()
@@ -123,15 +125,25 @@
         # set up socket ping/pong
         log.debug("Starting thread to set node status")
         t = Thread(target=self.__node_status_worker, daemon=True)
         t.start()
 
         log.info("Initialization done")
 
-    def setup_socket_connection(self):
+    def setup_socket_connection(self) -> SocketIO:
+        """
+        Setup a socket connection. If a message queue is defined, connect the
+        socket to the message queue. Otherwise, use the default socketio
+        settings.
+
+        Returns
+        -------
+        SocketIO
+            SocketIO object
+        """
 
         msg_queue = self.ctx.config.get('rabbitmq_uri')
         if msg_queue:
             log.debug(f'Connecting to msg queue: {msg_queue}')
 
         try:
             socketio = SocketIO(
@@ -157,27 +169,27 @@
         # FIXME: temporary fix to get socket object into the namespace class
         DefaultSocketNamespace.socketio = socketio
         socketio.on_namespace(DefaultSocketNamespace("/tasks"))
 
         return socketio
 
     @staticmethod
-    def configure_logging():
+    def configure_logging() -> None:
         """Set third party loggers to a warning level"""
 
         # Prevent logging from urllib3
         logging.getLogger("urllib3").setLevel(logging.WARNING)
         logging.getLogger("socketIO-client").setLevel(logging.WARNING)
         logging.getLogger("engineio.server").setLevel(logging.WARNING)
         logging.getLogger("socketio.server").setLevel(logging.WARNING)
         logging.getLogger('sqlalchemy.engine').setLevel(logging.WARNING)
         logging.getLogger('requests_oauthlib.oauth2_session')\
             .setLevel(logging.WARNING)
 
-    def configure_flask(self):
+    def configure_flask(self) -> None:
         """Configure the Flask settings of the vantage6 server."""
 
         # let us handle exceptions
         self.app.config['PROPAGATE_EXCEPTIONS'] = True
 
         # patch where to obtain token
         self.app.config['JWT_AUTH_URL_RULE'] = '/api/token'
@@ -307,15 +319,14 @@
                 HTTPStatus.INTERNAL_SERVER_ERROR
 
         @self.app.route('/robots.txt')
         def static_from_root():
             return send_from_directory(self.app.static_folder,
                                        request.path[1:])
 
-
     def _get_jwt_expiration_seconds(
         self, config_key: str, default_hours: int,
         longer_than: int = MIN_TOKEN_VALIDITY_SECONDS,
         is_refresh: bool = False
     ) -> int:
         """
         Return the expiration time for JWT tokens.
@@ -363,24 +374,38 @@
             # default
             log.error(f"Invalid value for '{config_key}': {hours_expire}. "
                       f"Using default value: {default_hours} hours")
             seconds_expire = int(float(default_hours) * 3600)
 
         return seconds_expire
 
-
-    def configure_api(self):
+    def configure_api(self) -> None:
         """Define global API output and its structure."""
 
         # helper to create HATEOAS schemas
         HATEOASModelSchema.api = self.api
 
         # whatever you get try to json it
         @self.api.representation('application/json')
-        def output_json(data, code, headers=None):
+        # pylint: disable=unused-argument
+        def output_json(
+            data: Any, code: HTTPStatus, headers: dict = None
+        ) -> Response:
+            """
+            Return jsonified data for request responses.
+
+            Parameters
+            ----------
+            data: Any
+                The data to be jsonified
+            code: HTTPStatus
+                The HTTP status code of the response
+            headers: dict
+                Additional headers to be added to the response
+            """
 
             if isinstance(data, db.Base):
                 data = db.jsonable(data)
             elif isinstance(data, list) and len(data) and \
                     isinstance(data[0], db.Base):
                 data = db.jsonable(data)
 
@@ -388,15 +413,31 @@
             resp.headers.extend(headers or {})
             return resp
 
     def configure_jwt(self):
         """Configure JWT authentication."""
 
         @self.jwt.additional_claims_loader
-        def additional_claims_loader(identity):
+        # pylint: disable=unused-argument
+        def additional_claims_loader(
+                identity: db.Authenticatable | dict) -> dict:
+            """
+            Create additional claims for JWT tokens: set user type and for
+            users, set their roles.
+
+            Parameters
+            ----------
+            identity: db.Authenticatable | dict
+                The identity for which to create the claims
+
+            Returns
+            -------
+            dict:
+                The claims to be added to the JWT token
+            """
             roles = []
             if isinstance(identity, db.User):
                 type_ = 'user'
                 roles = [role.name for role in identity.roles]
 
             elif isinstance(identity, db.Node):
                 type_ = 'node'
@@ -410,26 +451,60 @@
                 'client_type': type_,
                 'roles': roles,
             }
 
             return claims
 
         @self.jwt.user_identity_loader
-        def user_identity_loader(identity):
-            """"JSON serializing identity to be used by create_access_token."""
+        # pylint: disable=unused-argument
+        def user_identity_loader(
+                identity: db.Authenticatable | dict) -> str | dict:
+            """"
+            JSON serializing identity to be used by create_access_token.
+
+            Parameters
+            ----------
+            identity: db.Authenticatable | dict
+                The identity to be serialized
+
+            Returns
+            -------
+            str | dict:
+                The serialized identity. For a node or user, this is the id;
+                for a container, it is a dict.
+            """
             if isinstance(identity, db.Authenticatable):
                 return identity.id
             if isinstance(identity, dict):
                 return identity
 
             log.error(f"Could not create a JSON serializable identity \
                         from '{str(identity)}'")
 
         @self.jwt.user_lookup_loader
-        def user_lookup_loader(jwt_payload, jwt_headers):
+        # pylint: disable=unused-argument
+        def user_lookup_loader(
+            jwt_payload: dict, jwt_headers: dict
+        ) -> db.Authenticatable | dict:
+            """
+            Load the user, node or container instance from the JWT payload.
+
+            Parameters
+            ----------
+            jwt_payload: dict
+                The JWT payload
+            jwt_headers: dict
+                The JWT headers
+
+            Returns
+            -------
+            db.Authenticatable | dict:
+                The user, node or container identity. If the identity is a
+                container, a dict is returned.
+            """
             identity = jwt_headers['sub']
             auth_identity = Identity(identity)
 
             # in case of a user or node an auth id is shared as identity
             if isinstance(identity, int):
 
                 # auth_identity = Identity(identity)
@@ -471,29 +546,30 @@
                         )
 
                 identity_changed.send(current_app._get_current_object(),
                                       identity=auth_identity)
 
                 return auth
             else:
+                # container identity
 
                 for rule in db.Role.get_by_name(DefaultRole.CONTAINER).rules:
                     auth_identity.provides.add(
                         RuleNeed(
                             name=rule.name,
                             scope=rule.scope,
                             operation=rule.operation
                         )
                     )
                 identity_changed.send(current_app._get_current_object(),
                                       identity=auth_identity)
                 log.debug(identity)
                 return identity
 
-    def load_resources(self):
+    def load_resources(self) -> None:
         """Import the modules containing API resources."""
 
         # make services available to the endpoints, this way each endpoint can
         # make use of 'em.
         services = {
             "socketio": self.socketio,
             "mail": self.mail,
@@ -506,26 +582,26 @@
             module = importlib.import_module('vantage6.server.resource.' + res)
             module.setup(self.api, self.ctx.config['api_path'], services)
 
     # TODO consider moving this method elsewhere. This is not trivial at the
     # moment because of the circular import issue with `db`, see
     # https://github.com/vantage6/vantage6/issues/53
     @staticmethod
-    def _add_default_roles():
+    def _add_default_roles() -> None:
         for role in get_default_roles(db):
             if not db.Role.get_by_name(role['name']):
                 log.warn(f"Creating new default role {role['name']}...")
                 new_role = db.Role(
                     name=role['name'],
                     description=role['description'],
                     rules=role['rules']
                 )
                 new_role.save()
 
-    def start(self):
+    def start(self) -> None:
         """
         Start the server.
 
         Before server is really started, some database settings are checked and
         (re)set where appropriate.
         """
         # add default roles (if they don't exist yet)
```

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/_data/dev/fixtures.yaml` & `vantage6-server-3.9.0rc2/vantage6/server/_data/dev/fixtures.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/_data/dev/node_a.yaml` & `vantage6-server-3.9.0rc2/vantage6/server/_data/dev/node_a.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/_data/dev/node_b.yaml` & `vantage6-server-3.9.0rc2/vantage6/server/_data/dev/node_b.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/_data/dev/server.yaml` & `vantage6-server-3.9.0rc2/vantage6/server/_data/dev/server.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/_data/example_fixtures.yaml` & `vantage6-server-3.9.0rc2/vantage6/server/_data/example_fixtures.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/_data/node_config_skeleton.yaml` & `vantage6-server-3.9.0rc2/vantage6/server/_data/node_config_skeleton.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/_data/server_config_skeleton.yaml` & `vantage6-server-3.9.0rc2/vantage6/server/_data/server_config_skeleton.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/_data/unittest_config.yaml` & `vantage6-server-3.9.0rc2/vantage6/server/_data/unittest_config.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/_data/unittest_fixtures.yaml` & `vantage6-server-3.9.0rc2/vantage6/server/_data/unittest_fixtures.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/_version.py` & `vantage6-server-3.9.0rc2/vantage6/server/_version.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, '__build__')) as fp:
     __build__ = json.load(fp)
 
 # Module version
-version_info = ((( 3, 8, 8, 'candidate', __build__, 0)))
+version_info = (3, 9, 0, 'candidate', __build__, 0)
 
 # Module version stage suffix map
 _specifier_ = {'alpha': 'a', 'beta': 'b', 'candidate': 'rc', 'final': ''}
 version = f'{version_info[0]}.{version_info[1]}.{version_info[2]}'
-pre_release = f'' if version_info[3] == 'final' else \
+pre_release = '' if version_info[3] == 'final' else \
   '.'+_specifier_[version_info[3]]+str(version_info[4])
-post_release = f'' if not version_info[5] else f'.post{version_info[5]}'
+post_release = '' if not version_info[5] else f'.post{version_info[5]}'
 
 # Module version accessible using thomas.__version__
 __version__ = f'{version}{pre_release}{post_release}'
```

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/cli/server.py` & `vantage6-server-3.9.0rc2/vantage6/server/cli/server.py`

 * *Files 20% similar despite different names*

```diff
@@ -31,25 +31,45 @@
 help_ = {
     "name": "name of the configutation you want to use.",
     "config": "absolute path to configuration-file; overrides NAME",
     "env": "configuration environment to use"
 }
 
 
-def click_insert_context(func):
+def click_insert_context(func: callable) -> callable:
+    """
+    Decorator to insert a ServerContext object into the function.
+
+    This decorator will insert a ServerContext object into the function. The
+    ServerContext object is created based on the configuration file that is
+    selected by the user. The user can select the configuration file by
+    supplying the name of the configuration file, or by supplying the path to
+    the configuration file. The decorator will also initialize the database
+    connection.
+
+    Parameters
+    ----------
+    func : callable
+        The function to decorate.
+
+    Returns
+    -------
+    callable
+        The decorated function.
+    """
 
     # add option decorators
     @click.option('-n', '--name', default=None, help=help_["name"])
     @click.option('-c', '--config', default=None, help=help_["config"])
     @click.option('-e', '--environment', default=S_ENV, help=help_["env"])
     @click.option('--system', 'system_folders', flag_value=True)
     @click.option('--user', 'system_folders', flag_value=False, default=S_FOL)
     @wraps(func)
-    def func_with_context(name, config, environment, system_folders,
-                          *args, **kwargs):
+    def func_with_context(name: str, config: str, environment: str,
+                          system_folders: bool, *args, **kwargs) -> callable:
 
         # select configuration if none supplied
         if config:
             ctx = ServerContext.from_external_config_file(
                 config,
                 environment,
                 system_folders
@@ -94,47 +114,60 @@
 
         return func(ctx, *args, **kwargs)
 
     return func_with_context
 
 
 @click.group(name='server')
-def cli_server():
+def cli_server() -> None:
     """Subcommand `vserver`."""
     pass
 
 
 #
 #   start
 #
 @cli_server.command(name='start')
 @click.option('--ip', default=None, help='ip address to listen on')
 @click.option('-p', '--port', type=int, help='port to listen on')
 @click.option('--debug', is_flag=True,
               help='run server in debug mode (auto-restart)')
 @click_insert_context
-def cli_server_start(ctx, ip, port, debug):
-    """Start the server."""
+def cli_server_start(ctx: ServerContext, ip: str, port: str,
+                     debug: bool) -> None:
+    """
+    Start the server.
 
+    Parameters
+    ----------
+    ctx : ServerContext
+        The server context.
+    ip : str
+        The ip address to listen on.
+    port : str
+        The port to listen on.
+    debug : bool
+        Run server in debug mode (auto-restart).
+    """
     info("Starting server.")
 
     # Run the server
     ip = ip or ctx.config['ip'] or '127.0.0.1'
     port = port or int(ctx.config['port']) or 5000
     info(f"ip: {ip}, port: {port}")
     app = ServerApp(ctx).start()
     run_dev_server(app, ip, port, debug=debug)
 
 
 #
 #   list
 #
 @cli_server.command(name='list')
-def cli_server_configuration_list():
-    """Print the available configurations."""
+def cli_server_configuration_list() -> None:
+    """Print the available servers."""
 
     click.echo("\nName"+(21*" ")+"Environments"+(21*" ")+"System/User")
     click.echo("-"*70)
 
     sys_configs, f1 = ServerContext.available_configurations(
         system_folders=True)
     for config in sys_configs:
@@ -159,16 +192,23 @@
 
 
 #
 #   files
 #
 @cli_server.command(name='files')
 @click_insert_context
-def cli_server_files(ctx):
-    """List files locations of a server instance."""
+def cli_server_files(ctx: ServerContext) -> None:
+    """
+    List files locations of a server instance.
+
+    Parameters
+    ----------
+    ctx : ServerContext
+        The context of the server instance.
+    """
     info(f"Configuration file = {ctx.config_file}")
     info(f"Log file           = {ctx.log_file}")
     info(f"Database           = {ctx.get_database_uri()}")
 
 
 #
 #   new
@@ -176,17 +216,27 @@
 @cli_server.command(name='new')
 @click.option('-n', '--name', default=None,
               help="name of the configutation you want to use.")
 @click.option('-e', '--environment', default=S_ENV,
               help='configuration environment to use')
 @click.option('--system', 'system_folders', flag_value=True)
 @click.option('--user', 'system_folders', flag_value=False, default=S_FOL)
-def cli_server_new(name, environment, system_folders):
-    """Create new configuration."""
+def cli_server_new(name: str, environment: str, system_folders: bool) -> None:
+    """
+    Create new server configuration.
 
+    Parameters
+    ----------
+    name : str
+        The name of the configuration.
+    environment : str
+        The environment of the configuration.
+    system_folders : bool
+        Whether to use system folders or not.
+    """
     if not name:
         name = q.text("Please enter a configuration-name:").ask()
         name_new = name.replace(" ", "-")
         if name != name_new:
             info(f"Replaced spaces from configuration name: {name}")
             name = name_new
 
@@ -224,35 +274,58 @@
 #
 #   import
 #
 @cli_server.command(name='import')
 @click.argument('file_', type=click.Path(exists=True))
 @click.option('--drop-all', is_flag=True, default=False)
 @click_insert_context
-def cli_server_import(ctx, file_, drop_all):
-    """ Import organizations/collaborations/users and tasks.
+def cli_server_import(ctx: ServerContext, file_: str, drop_all: bool) -> None:
+    """
+    Import organizations/collaborations/users and tasks. Mainly useful for
+    testing purposes.
 
-        Especially usefull for testing purposes.
+    Parameters
+    ----------
+    ctx : ServerContext
+        The context of the server instance.
+    file_ : str
+        The YAML file with resources to import.
+    drop_all : bool
+        Whether to drop all tables before importing.
     """
+    # Note: ctx appears to be unused but is needed for the click_insert_context
+    # to select the server in which to import the data.
     info("Reading yaml file.")
     with open(file_) as f:
         entities = yaml.safe_load(f.read())
 
     info("Adding entities to database.")
     fixture.load(entities, drop_all=drop_all)
 
 
 #
 #   shell
 #
 @cli_server.command(name='shell')
 @click_insert_context
-def cli_server_shell(ctx):
-    """ Run a iPython shell. """
-    # shell.init(ctx.environment)
+def cli_server_shell(ctx: ServerContext) -> None:
+    """
+    Run an iPython shell.
+
+    Note that using the shell is not recommended, as there are no checks on
+    the validity of the data you are entering. It is better to use the UI,
+    Python client, or the API.
+
+    Parameters
+    ----------
+    ctx : ServerContext
+        The context of the server instance.
+    """
+    # Note: ctx appears to be unused but is needed for the click_insert_context
+    # to select the server and start the database connection.
     c = get_config()
     c.InteractiveShellEmbed.colors = "Linux"
 
     # Suppress logging (e.g. on tab-completion)
     import logging
     logging.getLogger('parso.cache').setLevel(logging.WARNING)
     logging.getLogger('parso.python.diff').setLevel(logging.WARNING)
@@ -265,10 +338,10 @@
     IPython.embed(config=c)
 
 
 #
 #   version
 #
 @cli_server.command(name='version')
-def cli_server_version():
-    """Returns current version of vantage6 services installed."""
+def cli_server_version() -> None:
+    """ Prints current version of vantage6 services installed. """
     click.echo(__version__)
```

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/controller/fixture.py` & `vantage6-server-3.9.0rc2/vantage6/server/controller/fixture.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import uuid
 import logging
 
 import vantage6.server.model as db
+from vantage6.server.model.base import Database
 
 module_name = __name__.split('.')[-1]
 log = logging.getLogger(module_name)
 
 
 # TODO maybe move this function to a more general location (utils?)
 def _is_valid_uuid(uuid_to_test):
@@ -23,19 +24,30 @@
     try:
         uuid_obj = uuid.UUID(uuid_to_test)
     except ValueError:
         return False
     return str(uuid_obj) == uuid_to_test
 
 
-def load(fixtures, drop_all=False):
+def load(fixtures: dict, drop_all: bool = False) -> None:
+    """
+    Load fixtures (i.e. fixed resources to test functionality) into the
+    database.
+
+    Parameters
+    ----------
+    fixtures : dict
+        Dictionary containing the fixtures to load into the database.
+    drop_all : bool
+        If `True` all tables in the database will be dropped before loading
+    """
     # TODO we are not sure the DB is connected here....
 
-    # if drop_all:
-    #     Database().drop_all()
+    if drop_all:
+        Database().drop_all()
 
     log.info("Create Organizations and Users")
     for org in fixtures.get("organizations", {}):
         # print(org)
 
         # create organization
         organization = db.Organization(**{k: org[k] for k in [
```

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/db.py` & `vantage6-server-3.9.0rc2/vantage6/server/db.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,16 +29,33 @@
 from vantage6.common.globals import STRING_ENCODING
 
 
 module_name = logger_name(__name__)
 log = logging.getLogger(module_name)
 
 
-def jsonable(value):
-    """Convert a (list of) SQLAlchemy instance(s) to native Python objects."""
+def jsonable(value: list[Base] | Base) -> list | dict:
+    """
+    Convert a (list of) SQLAlchemy instance(s) to native Python objects.
+
+    Parameters
+    ----------
+    value : list[Base] | Base
+        A single SQLAlchemy instance or a list of SQLAlchemy instances
+
+    Returns
+    -------
+    list | dict
+        A single Python object or a list of Python objects
+
+    Raises
+    ------
+    Exception
+        If the value is not an instance of db.Base or a list of db.Base
+    """
     if isinstance(value, list):
         return [jsonable(i) for i in value]
 
     elif isinstance(value, Base):
         log.debug(f"preparing={value}")
         retval = dict()
         mapper = sql.inspect(value.__class__)
@@ -61,12 +78,7 @@
             retval[column] = column_value
 
         return retval
 
     # FIXME: does it make sense to raise an exception or should base types
     #        (or other JSON-serializable types) just be returned as-is?
     raise Exception('value should be instance of db.Base or list!')
-
-
-def jsonify(value):
-    """Convert a (list of) SQLAlchemy instance(s) to a JSON (string)."""
-    return json.dumps(jsonable(value))
```

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/default_roles.py` & `vantage6-server-3.9.0rc2/vantage6/server/default_roles.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-from typing import List
 from enum import Enum
 
 from vantage6.server.model.rule import Operation, Scope
 
 
-# Name of the default roles
 class DefaultRole(str, Enum):
+    """ Enum containing the names of the default roles """
     ROOT = "Root"
     CONTAINER = "container"
     NODE = "node"
     VIEWER = "Viewer"
     RESEARCHER = "Researcher"
     ORG_ADMIN = "Organization Admin"
     COL_ADMIN = "Collaboration Admin"
 
 
 # TODO BvB 22-06-07: we now have to pass this 'db' module as argument to a
 # function because that module has a connection to the database. This should
 # not be necessary. Fix that after fixing the circular imports described in
 # https://github.com/vantage6/vantage6/issues/53
-def get_default_roles(db) -> List[dict]:
+def get_default_roles(db) -> list[dict]:
     """
     Get a list containing the default roles and their rules, so that they may
     be created in the database
 
     Parameters
     ----------
     db
```

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/globals.py` & `vantage6-server-3.9.0rc2/vantage6/server/globals.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/mail_service.py` & `vantage6-server-3.9.0rc2/vantage6/server/mail_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 
 from threading import Thread
-from typing import List
 from flask_mail import Message, Mail
 from flask import Flask
 
 from vantage6.common import logger_name
 
 module_name = logger_name(__name__)
 log = logging.getLogger(module_name)
@@ -41,15 +40,15 @@
         with app.app_context():
             try:
                 self.mail.send(msg)
             except Exception as e:
                 log.error("Mailserver error!")
                 log.debug(e)
 
-    def send_email(self, subject: str, sender: str, recipients: List[str],
+    def send_email(self, subject: str, sender: str, recipients: list[str],
                    text_body: str, html_body: str) -> None:
         """
         Send an email.
 
         This is used for service emails, e.g. to help users reset their
         password.
```

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/model/__init__.py` & `vantage6-server-3.9.0rc2/vantage6/server/model/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/model/algorithm_port.py` & `vantage6-server-3.9.0rc2/vantage6/server/model/algorithm_port.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/model/authenticatable.py` & `vantage6-server-3.9.0rc2/vantage6/server/model/authenticatable.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/model/base.py` & `vantage6-server-3.9.0rc2/vantage6/server/model/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 import os
 import inspect as class_inspect
-from typing import List
 from flask.globals import g
 
 from sqlalchemy import Column, Integer, inspect, Table
 from sqlalchemy.orm.session import Session
 from sqlalchemy.ext.declarative import declarative_base, declared_attr
 from sqlalchemy.orm.clsregistry import _ModuleMarker
 from sqlalchemy import create_engine
@@ -150,29 +149,29 @@
             else:
                 log.error(
                     f"Model {table_cls} declares table {table_name} which does"
                     " not exist in the database."
                 )
 
     def get_non_existing_columns(self, table_cls: Table,
-                                 table_name: str) -> List[Column]:
+                                 table_name: str) -> list[Column]:
         """
         Return a list of columns that are defined in the SQLAlchemy model, but
         are not present in the database
 
         Parameters
         ----------
         table_cls: Table
             The table that is evaluated
         table_name: str
             The name of the table
 
         Returns
         -------
-        List[Column]
+        list[Column]
             List of SQLAlchemy Column objects that are present in the model,
             but not in the database
         """
         column_names = [
             c["name"] for c in self.__iengine.get_columns(table_name)
         ]
         mapper = inspect(table_cls)
@@ -205,15 +204,15 @@
                  "exist yet")
         self.engine.execute(
             'ALTER TABLE "%s" ADD COLUMN %s %s' % (tab_name, col_name,
                                                    col_type)
         )
 
     @staticmethod
-    def is_column_missing(column: Column, column_names: List[str],
+    def is_column_missing(column: Column, column_names: list[str],
                           table_name: str) -> bool:
         """ Check if column is missing in the table
 
         Parameters
         ----------
         column: Column
             The column that is evaluated
```

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/model/collaboration.py` & `vantage6-server-3.9.0rc2/vantage6/server/model/collaboration.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from __future__ import annotations
-from typing import List, Union
 from sqlalchemy import Column, String, Boolean, exists
 from sqlalchemy.orm import relationship
 from sqlalchemy.orm.exc import NoResultFound
 
 from vantage6.server.model.base import Base, DatabaseSessionManager
 from vantage6.server.model.node import Node
 from vantage6.server.model.organization import Organization
@@ -39,37 +38,37 @@
 
     # relationships
     organizations = relationship("Organization", secondary="Member",
                                  back_populates='collaborations')
     nodes = relationship("Node", back_populates="collaboration")
     tasks = relationship("Task", back_populates="collaboration")
 
-    def get_organization_ids(self) -> List[int]:
+    def get_organization_ids(self) -> list[int]:
         """
         Returns a list of organization ids that are part of this collaboration.
 
         Returns
         -------
         list[int]
             List of organization ids
         """
         return [organization.id for organization in self.organizations]
 
-    def get_task_ids(self) -> List[int]:
+    def get_task_ids(self) -> list[int]:
         """
         Returns a list of task ids that are part of this collaboration.
 
         Returns
         -------
         list[int]
             List of task ids
         """
         return [task.id for task in self.tasks]
 
-    def get_nodes_from_organizations(self, ids: List[int]) -> List[Node]:
+    def get_nodes_from_organizations(self, ids: list[int]) -> list[Node]:
         """
         Returns a subset of nodes that are part of the given organizations.
 
         Parameters
         ----------
         ids : list[int]
             List of organization ids
@@ -78,15 +77,15 @@
         -------
         list[:class:`~vantage6.server.model.node.Node`]
             List of nodes that are part of the given organizations
         """
         return [n for n in self.nodes if n.organization.id in ids]
 
     def get_node_from_organization(
-            self, organization: Organization) -> Union[Node, None]:
+            self, organization: Organization) -> Node | None:
         """
         Returns the node that is part of the given :class:`.Organization`.
 
         Parameters
         ----------
         organization: Organization
             Organization
@@ -99,15 +98,15 @@
         """
         for node in self.nodes:
             if node.organization.id == organization.id:
                 return node
         return None
 
     @classmethod
-    def find_by_name(cls, name: str) -> Union[Collaboration, None]:
+    def find_by_name(cls, name: str) -> Collaboration | None:
         """
         Find :class:`.Collaboration` by its name.
 
         Note
         ----
         If multiple collaborations share the same name, the first
         collaboration found is returned.
```

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/model/member.py` & `vantage6-server-3.9.0rc2/vantage6/server/model/member.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/model/node.py` & `vantage6-server-3.9.0rc2/vantage6/server/model/node.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/model/node_config.py` & `vantage6-server-3.9.0rc2/vantage6/server/model/node_config.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/model/organization.py` & `vantage6-server-3.9.0rc2/vantage6/server/model/organization.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/model/permission.py` & `vantage6-server-3.9.0rc2/vantage6/server/model/permission.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/model/result.py` & `vantage6-server-3.9.0rc2/vantage6/server/model/result.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/model/role.py` & `vantage6-server-3.9.0rc2/vantage6/server/model/role.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from __future__ import annotations
-from typing import Union
 from sqlalchemy import Column, Text, Integer, ForeignKey
 from sqlalchemy.orm import relationship
 from sqlalchemy.orm.exc import NoResultFound
 
 from vantage6.server.model.base import Base, DatabaseSessionManager
 
 
@@ -14,19 +13,19 @@
     ----------
     name : str
         Name of the role
     description : str
         Description of the role
     organization_id : int
         Id of the organization this role belongs to
-    rules : List[Rule]
+    rules : list[Rule]
         List of rules that belong to this role
     organization : Organization
         Organization this role belongs to
-    users : List[User]
+    users : list[User]
         List of users that belong to this role
     """
 
     # fields
     name = Column(Text)
     description = Column(Text)
     organization_id = Column(Integer, ForeignKey("organization.id"))
@@ -35,15 +34,15 @@
     rules = relationship("Rule", back_populates="roles",
                          secondary="role_rule_association")
     organization = relationship("Organization", back_populates="roles")
     users = relationship("User", back_populates="roles",
                          secondary="Permission")
 
     @classmethod
-    def get_by_name(cls, name: str) -> Union[Role, None]:
+    def get_by_name(cls, name: str) -> Role | None:
         """
         Get a role by its name.
 
         Parameters
         ----------
         name : str
             Name of the role
```

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/model/rule.py` & `vantage6-server-3.9.0rc2/vantage6/server/model/rule.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 from enum import Enum as Enumerate
-from typing import Union
 
 from sqlalchemy import Column, Text, String, Enum
 from sqlalchemy.orm import relationship
 from sqlalchemy.orm.exc import NoResultFound
 from vantage6.server.model.base import Base, DatabaseSessionManager
 
 
@@ -57,16 +56,15 @@
     # relationships
     roles = relationship("Role", back_populates="rules",
                          secondary="role_rule_association")
     users = relationship("User", back_populates="rules",
                          secondary="UserPermission")
 
     @classmethod
-    def get_by_(cls, name: str, scope: str, operation: str
-                ) -> Union[Rule, None]:
+    def get_by_(cls, name: str, scope: str, operation: str) -> Rule | None:
         """
         Get a rule by its name, scope and operation.
 
         Parameters
         ----------
         name : str
             Name of the resource on which the rule acts, e.g. 'node'
```

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/model/task.py` & `vantage6-server-3.9.0rc2/vantage6/server/model/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from typing import List
 from sqlalchemy import Column, String, ForeignKey, Integer, sql
 from sqlalchemy.orm import relationship
 from sqlalchemy.ext.hybrid import hybrid_property
 
 from vantage6.common.task_status import TaskStatus, has_task_failed
 from vantage6.server.model.node import Node
 from vantage6.server.model.base import Base, DatabaseSessionManager
@@ -110,15 +109,15 @@
         elif TaskStatus.INITIALIZING in result_statuses:
             return TaskStatus.INITIALIZING.value
         elif TaskStatus.PENDING in result_statuses:
             return TaskStatus.PENDING.value
         else:
             return TaskStatus.COMPLETED.value
 
-    def results_for_node(self, node: Node) -> List:
+    def results_for_node(self, node: Node) -> list:
         """
         Get all results for a given node.
 
         Parameters
         ----------
         node: model.node.Node
             Node for which to get the results
```

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/model/user.py` & `vantage6-server-3.9.0rc2/vantage6/server/model/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 import bcrypt
 import re
 import datetime as dt
 
-from typing import Tuple, Union
 from sqlalchemy import Column, String, Integer, ForeignKey, exists, DateTime
 from sqlalchemy.orm import relationship, validates
 
 from vantage6.server.model.base import DatabaseSessionManager
 from vantage6.server.model.authenticatable import Authenticatable
 from vantage6.server.model.rule import Operation, Rule, Scope
 
@@ -108,15 +107,15 @@
         Returns
         -------
         str
             Hashed password
         """
         return self.hash(password)
 
-    def set_password(self, pw: str) -> Union[str, None]:
+    def set_password(self, pw: str) -> str | None:
         """
         Set the password of the current user. This function doesn't save the
         new password to the database
 
         Parameters
         ----------
         pw: str
@@ -165,15 +164,15 @@
         """
         if self.password is not None:
             expected_hash = self.password.encode('utf8')
             return bcrypt.checkpw(pw.encode('utf8'), expected_hash)
         return False
 
     def is_blocked(self, max_failed_attempts: int,
-                   inactivation_in_minutes: int) -> Tuple[bool, str | None]:
+                   inactivation_in_minutes: int) -> tuple[bool, str | None]:
         """
         Check if user can login or if they are temporarily blocked because they
         entered a wrong password too often
 
         Parameters
         ----------
         max_failed_attempts: int
```

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/permission.py` & `vantage6-server-3.9.0rc2/vantage6/server/permission.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
 import importlib
 
 from collections import namedtuple
-from typing import Callable, List, Union
 from flask_principal import Permission, PermissionDenied
 
 from vantage6.server.globals import RESOURCES
 from vantage6.server.default_roles import DefaultRole
 from vantage6.server.model.role import Role
 from vantage6.server.model.rule import Rule, Operation, Scope
 from vantage6.server.model.base import DatabaseSessionManager
@@ -195,15 +194,15 @@
             self.assign_rule_to_node(resource, scope, operation)
 
         # assign all new rules to root user
         self.assign_rule_to_root(resource, scope, operation)
 
         self.collection(resource).add(rule.scope, rule.operation)
 
-    def appender(self, name: str) -> Callable:
+    def appender(self, name: str) -> callable:
         """
         Add a module's rules to the rule collection
 
         Parameters
         ----------
         name: str
             The name of the module whose rules are to be registered
@@ -292,29 +291,29 @@
             operation=operation,
             scope=scope
         ).scalar()
         session.commit()
         return result
 
     @staticmethod
-    def verify_user_rules(rules: List[Rule]) -> Union[dict, bool]:
+    def check_user_rules(rules: list[Rule]) -> dict | bool:
         """
-        Check if an user, node or container has all the `rules`
+        Check if a user, node or container has all the `rules` in a list
 
         Parameters
         ----------
         rules: List[Rule]
             List of rules that user is checked to have
 
         Returns
         -------
         Union[dict, bool]
-            False if user has all rules, else a dict with a message
+            Dict with a message which rule is missing, else None
         """
         for rule in rules:
             requires = RuleNeed(rule.name, rule.scope, rule.operation)
             try:
                 Permission(requires).test()
             except PermissionDenied:
                 return {"msg": f"You don't have the rule ({rule.name}, "
                         f"{rule.scope}, {rule.operation})"}
-        return False
+        return None
```

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/resource/__init__.py` & `vantage6-server-3.9.0rc2/vantage6/server/resource/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # -*- coding: utf-8 -*-
 import datetime
 from http import HTTPStatus
 import logging
 
 from functools import wraps
-from typing import Union
 
 from flask import g, request
 from flask_restful import Resource, Api
 from flask_mail import Mail
 from flask_jwt_extended import (
     get_jwt, get_jwt_identity, jwt_required
 )
@@ -105,15 +104,15 @@
         -------
         tuple
             Tuple of (dumped page, HTTPStatus.OK, headers of the page)
         """
         return self.dump(page, schema), HTTPStatus.OK, page.headers
 
     @staticmethod
-    def obtain_auth() -> Union[db.Authenticatable, dict]:
+    def obtain_auth() -> db.Authenticatable | dict:
         """
         Read authenticatable object or dict from the flask global context.
 
         Returns
         -------
         Union[db.Authenticatable, dict]
             Authenticatable object or dict. Authenticatable object is either a
```

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/resource/collaboration.py` & `vantage6-server-3.9.0rc2/vantage6/server/resource/collaboration.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/resource/common/_schema.py` & `vantage6-server-3.9.0rc2/vantage6/server/resource/common/_schema.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/resource/common/auth_helper.py` & `vantage6-server-3.9.0rc2/vantage6/server/resource/common/auth_helper.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/resource/common/swagger_templates.py` & `vantage6-server-3.9.0rc2/vantage6/server/resource/common/swagger_templates.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/resource/event.py` & `vantage6-server-3.9.0rc2/vantage6/server/resource/event.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/resource/health.py` & `vantage6-server-3.9.0rc2/vantage6/server/resource/health.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # -*- coding: utf-8 -*-
 import logging
 
 from http import HTTPStatus
-from sqlalchemy.exc import InvalidRequestError
 from flask.globals import g
 from flask_restful import Api
 
 from vantage6.server.resource import ServicesResources
 from vantage6.common import logger_name
 
 
@@ -34,21 +33,14 @@
         Health,
         path,
         endpoint='health',
         methods=('GET',),
         resource_class_kwargs=services
     )
 
-    api.add_resource(
-        Fix,
-        path + "/fix",
-        methods=('GET',),
-        resource_class_kwargs=services
-    )
-
 
 # ------------------------------------------------------------------------------
 # Resources / API's
 # ------------------------------------------------------------------------------
 class Health(ServicesResources):
 
     def get(self):
@@ -74,25 +66,7 @@
             g.session.execute('SELECT 1')
             db_ok = True
         except Exception as e:
             log.error("DB not responding")
             log.debug(e)
 
         return {'database': db_ok}, HTTPStatus.OK
-
-
-class Fix(ServicesResources):
-
-    def get(self):
-        """Experimental switch to fix db errors"""
-
-        try:
-            g.session.execute('SELECT 1')
-
-        except (InvalidRequestError, Exception) as e:
-            log.error("DB nudge... Does this work?")
-            log.debug(e)
-            # session.invalidate()
-            # session.rollback()
-
-        # finally:
-        #     session.close()
```

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/resource/node.py` & `vantage6-server-3.9.0rc2/vantage6/server/resource/node.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/resource/organization.py` & `vantage6-server-3.9.0rc2/vantage6/server/resource/organization.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/resource/port.py` & `vantage6-server-3.9.0rc2/vantage6/server/resource/port.py`

 * *Files 13% similar despite different names*

```diff
@@ -410,52 +410,97 @@
         parameters:
           - in: path
             name: label
             schema:
               type: string
             description: Algorithm port label to filter by
           - in: path
+            name: only_children
+            schema:
+              type: boolean
+            description: Only include the addresses of subtasks, not those at
+              the same level. Incompatible with 'only_parent'.
+          - in: path
+            name: only_parent
+            schema:
+              type: boolean
+            description: Only send the address of the parent task, not those at
+              the same level. Incompatible with 'only_children'.
+          - in: path
             name: include_children
             schema:
               type: boolean
-            description: Include the addresses of subtasks
+            description: Include the addresses of subtasks. Ignored if
+              'only_children' is True. Incompatible with 'only_parent',
+              superseded by 'only_children'.
           - in: path
             name: include_parent
             schema:
               type: boolean
-            description: Include the addresses of parent tasks
+            description: Include the addresses of parent tasks. Ignored if
+              'only_parent' is True. Incopatible with 'only_children',
+              superseded by 'only_parent'.
 
         responses:
           200:
             description: Ok
+          400:
+            description: Incompatible arguments specified
 
         security:
         - bearerAuth: []
 
         tags: ["VPN"]
         """
         task_id = g.container['task_id']
         task_ids = [task_id]
 
         task = db.Task.get(task_id)
 
+        include_children = request.args.get('include_children', False)
+        include_parent = request.args.get('include_parent', False)
+        only_children = request.args.get('only_children', False)
+        only_parent = request.args.get('only_parent', False)
+
+        if only_children and only_parent:
+            return {
+                'msg': 'Using only_children and only_parent simultaneously is '
+                'not possible! Specify one or the other.'
+            }, HTTPStatus.BAD_REQUEST
+        elif only_children and include_parent:
+            return {
+                'msg': 'Using only_children and include_parent simultaneously '
+                'is not possible! Specify one or the other.'
+            }, HTTPStatus.BAD_REQUEST
+        elif only_parent and include_children:
+            return {
+                'msg': 'Using only_parent and include_children simultaneously '
+                'is not possible! Specify one or the other.'
+            }, HTTPStatus.BAD_REQUEST
+
         # include child tasks if requested
-        if request.args.get('include_children', False):
+        if include_children or only_children:
             subtasks = g.session.query(db.Task).filter(
                 db.Task.parent_id == task_id
             ).all()
-            task_ids.extend([t.id for t in subtasks])
+            if only_children:
+                task_ids = [t.id for t in subtasks]
+            else:
+                task_ids.extend([t.id for t in subtasks])
 
         # include parent task if requested
-        if request.args.get('include_parent', False):
+        if include_parent or only_parent:
             parent = g.session.query(db.Task).filter(
                 db.Task.id == task.parent_id
             ).one_or_none()
             if parent:
-                task_ids.append(parent.id)
+                if only_parent:
+                    task_ids = [parent.id]
+                else:
+                    task_ids.append(parent.id)
 
         # get all ports for the tasks requested
         q = g.session.query(AlgorithmPort)\
                      .join(Result)\
                      .filter(Result.task_id.in_(task_ids))\
 
         # filter by label if requested
@@ -469,12 +514,13 @@
         addresses = []
         for port in ports:
             d = {
                 'port': port.port,
                 'label': port.label,
                 'ip': port.result.node.ip,
                 'organization_id': port.result.organization_id,
-                'task_id': port.result.task_id
+                'task_id': port.result.task_id,
+                'parent_id': port.result.task.parent_id,
             }
             addresses.append(d)
 
         return {'addresses': addresses}, HTTPStatus.OK
```

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/resource/recover.py` & `vantage6-server-3.9.0rc2/vantage6/server/resource/recover.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/resource/result.py` & `vantage6-server-3.9.0rc2/vantage6/server/resource/result.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/resource/role.py` & `vantage6-server-3.9.0rc2/vantage6/server/resource/role.py`

 * *Files 0% similar despite different names*

```diff
@@ -335,15 +335,15 @@
                 rule = db.Rule.get(rule_id)
                 if not rule:
                     return {"msg": f"Rule id={rule_id} not found."}, \
                         HTTPStatus.NOT_FOUND
                 rules.append(rule)
 
         # And check that this used has the rules he is trying to assign
-        denied = self.permissions.verify_user_rules(rules)
+        denied = self.permissions.check_user_rules(rules)
         if denied:
             return denied, HTTPStatus.UNAUTHORIZED
 
         # set the organization id
         organization_id = (
             data['organization_id']
             if data['organization_id'] else g.user.organization_id
@@ -519,15 +519,15 @@
             rules = []
             for rule_id in data['rules']:
                 rule = db.Rule.get(rule_id)
                 if not rule:
                     return {'msg': f'rule with id={rule_id} not found!'}, \
                         HTTPStatus.NOT_FOUND
                 rules.append(rule)
-            denied = self.permissions.verify_user_rules(rules)
+            denied = self.permissions.check_user_rules(rules)
             if denied:
                 return denied, HTTPStatus.UNAUTHORIZED
             role.rules = rules
         role.save()
 
         return role_schema.dump(role, many=False).data, HTTPStatus.OK
 
@@ -720,15 +720,15 @@
         if not self.r.e_glo.can():
             if not (self.r.e_org.can() and
                     g.user.organization == role.organization):
                 return {'msg': 'You lack permissions to do that'}, \
                     HTTPStatus.UNAUTHORIZED
 
         # user needs to role to assign it
-        denied = self.permissions.verify_user_rules([rule])
+        denied = self.permissions.check_user_rules([rule])
         if denied:
             return denied, HTTPStatus.UNAUTHORIZED
 
         # We're good, lets add the rule
         role.rules.append(rule)
         role.save()
 
@@ -787,15 +787,15 @@
         if not self.r.d_glo.can():
             if not (self.r.d_org.can() and
                     g.user.organization == role.organization):
                 return {'msg': 'You lack permissions to do that'}, \
                     HTTPStatus.UNAUTHORIZED
 
         # user needs to role to remove it
-        denied = self.permissions.verify_user_rules([rule])
+        denied = self.permissions.check_user_rules([rule])
         if denied:
             return denied, HTTPStatus.UNAUTHORIZED
 
         if not (rule in role.rules):
             return {'msg': f'Rule id={rule_id} not found in Role={id}!'}, \
                 HTTPStatus.NOT_FOUND
```

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/resource/rule.py` & `vantage6-server-3.9.0rc2/vantage6/server/resource/rule.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/resource/stats.py` & `vantage6-server-3.9.0rc2/vantage6/server/resource/stats.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/resource/task.py` & `vantage6-server-3.9.0rc2/vantage6/server/resource/task.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/resource/token.py` & `vantage6-server-3.9.0rc2/vantage6/server/resource/token.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/resource/user.py` & `vantage6-server-3.9.0rc2/vantage6/server/resource/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -361,15 +361,15 @@
         # never extend your power on your own.
         potential_roles = data.get("roles")
         roles = []
         if potential_roles:
             for role in potential_roles:
                 role_ = db.Role.get(role)
                 if role_:
-                    denied = self.permissions.verify_user_rules(role_.rules)
+                    denied = self.permissions.check_user_rules(role_.rules)
                     if denied:
                         return denied, HTTPStatus.UNAUTHORIZED
                     roles.append(role_)
 
                     # validate that the assigned role is either a general role
                     # or a role pertaining to that organization
                     if (role_.organization and
@@ -381,15 +381,15 @@
 
         # You can only assign rules that you already have to others.
         potential_rules = data["rules"]
         rules = []
         if potential_rules:
             rules = [db.Rule.get(rule) for rule in potential_rules
                      if db.Rule.get(rule)]
-            denied = self.permissions.verify_user_rules(rules)
+            denied = self.permissions.check_user_rules(rules)
             if denied:
                 return denied, HTTPStatus.UNAUTHORIZED
 
         # Ok, looks like we got most of the security hazards out of the way
         user = db.User(
             username=data["username"],
             firstname=data["firstname"],
@@ -617,15 +617,15 @@
             # validate that user is not changing their own roles
             if user == g.user:
                 return {'msg': "You can't changes your own roles!"}, \
                     HTTPStatus.UNAUTHORIZED
 
             # validate that user can assign these
             for role in roles:
-                denied = self.permissions.verify_user_rules(role.rules)
+                denied = self.permissions.check_user_rules(role.rules)
                 if denied:
                     return denied, HTTPStatus.UNAUTHORIZED
 
                 # validate that the assigned role is either a general role or a
                 # role pertaining to that organization
                 if (role.organization and
                         role.organization.id != user.organization_id):
@@ -634,15 +634,15 @@
                         "belongs to a different organization than the user "
                     )}, HTTPStatus.UNAUTHORIZED
 
             # validate that user is not deleting roles they cannot assign
             # e.g. an organization admin is not allowed to delete a root role
             deleted_roles = [r for r in user.roles if r not in roles]
             for role in deleted_roles:
-                denied = self.permissions.verify_user_rules(role.rules)
+                denied = self.permissions.check_user_rules(role.rules)
                 if denied:
                     return {"msg": (
                         f"You are trying to delete the role {role.name} from "
                         "this user but that is not allowed because they have "
                         f"permissions you don't have: {denied['msg']} (and "
                         "they do!)"
                     )}, HTTPStatus.UNAUTHORIZED
@@ -661,22 +661,22 @@
 
             # validate that user is not changing their own rules
             if user == g.user:
                 return {'msg': "You can't changes your own rules!"}, \
                     HTTPStatus.UNAUTHORIZED
 
             # validate that user can assign these
-            denied = self.permissions.verify_user_rules(rules)
+            denied = self.permissions.check_user_rules(rules)
             if denied:
                 return denied, HTTPStatus.UNAUTHORIZED
 
             # validate that user is not deleting rules they do not have
             # themselves
             deleted_rules = [r for r in user.rules if r not in rules]
-            denied = self.permissions.verify_user_rules(deleted_rules)
+            denied = self.permissions.check_user_rules(deleted_rules)
             if denied:
                 return {"msg": (
                     f"{denied['msg']}. You can't delete permissions for "
                     "another user that you don't have yourself!"
                 )}, HTTPStatus.UNAUTHORIZED
 
             user.rules = rules
```

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/resource/version.py` & `vantage6-server-3.9.0rc2/vantage6/server/resource/version.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/resource/vpn.py` & `vantage6-server-3.9.0rc2/vantage6/server/resource/vpn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # -*- coding: utf-8 -*-
 import logging
 import os
 import json
 import base64
 import hashlib
 import re
-from typing import Dict, Tuple
 import urllib.parse as urlparse
 
 from http import HTTPStatus
 from flask.globals import g
 from flask import request
 from flask_restful import Api
 import requests
@@ -416,15 +415,15 @@
             )
 
         # get the authorization token from the request headers
         redirected_uri = response.headers['Location']
         parsed_url = urlparse.urlparse(redirected_uri)
         self.code = urlparse.parse_qs(parsed_url.query)['code']
 
-    def _get_token(self) -> Dict:
+    def _get_token(self) -> dict:
         """
         Use authorization code to obtain a token from the EduVPN portal
 
         Returns
         -------
         Dict:
             EduVPN portal token
@@ -497,15 +496,15 @@
         end_key = '</key>\n'
         end_remove_pos = ovpn_config.find(end_key)
         return (
             ovpn_config[0:start_remove_pos] +
             ovpn_config[end_remove_pos+len(end_key):]
         )
 
-    def get_profile(self) -> Dict:
+    def get_profile(self) -> dict:
         """
         Call the profile_list route of EduVPN API
 
         Returns
         -------
         Dict
             Response content of the EduVPN /profile_list route
@@ -530,15 +529,15 @@
             'profile_id': profile_id
         }
         response_config = self.session.get(
             f'{self.API_URL}/profile_config', params=params
         )
         return response_config.content.decode('utf-8')
 
-    def get_key_pair(self) -> Tuple[str, str]:
+    def get_key_pair(self) -> tuple[str, str]:
         """
         Call the create_keypair route of EduVPN API
 
         Returns
         -------
         Tuple(str, str):
             The certificate and the private key that together form the key pair
```

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/resource/websocket_test.py` & `vantage6-server-3.9.0rc2/vantage6/server/resource/websocket_test.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.8.8rc3/vantage6/server/websockets.py` & `vantage6-server-3.9.0rc2/vantage6/server/websockets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-from typing import Dict
 import jwt
 import datetime as dt
 
 from flask import request, session
 from flask_jwt_extended import get_jwt_identity, verify_jwt_in_request
 from flask_socketio import Namespace, emit, join_room, leave_room
 
@@ -201,15 +200,15 @@
         Parameters
         ----------
         e: str
             Error message that is being displayed in the server log
         """
         self.log.error(e)
 
-    def on_algorithm_status_change(self, data: Dict) -> None:
+    def on_algorithm_status_change(self, data: dict) -> None:
         """
         An algorithm container has changed its status. This status change may
         be that the algorithm has finished, crashed, etc. Here we notify the
         collaboration of the change.
 
         Parameters
         ----------
@@ -224,14 +223,20 @@
                 "status": "active",
                 # result_id for which the algorithm was running
                 "result_id": 1,
                 # collaboration_id for which the algorithm was running
                 "collaboration_id": 1
             }
         """
+        # only allow nodes to send this event
+        if session.type != 'node':
+            self.log.warn('Only nodes can send algorithm status changes! '
+                          f'{session.type} {session.auth_id} is not allowed.')
+            return
+
         result_id = data.get('result_id')
         task_id = data.get('task_id')
         collaboration_id = data.get('collaboration_id')
         status = data.get('status')
         node_id = data.get('node_id')
         organization_id = data.get('organization_id')
         parent_id = data.get('parent_id')
@@ -269,14 +274,20 @@
         Store this in the database for the duration of the node's session.
 
         Parameters
         ----------
         node_config: dict
             Dictionary containing the node's configuration.
         """
+        # only allow nodes to send this event
+        if session.type != 'node':
+            self.log.warn('Only nodes can send node configuration updates! '
+                          f'{session.type} {session.auth_id} is not allowed.')
+            return
+
         node = db.Node.get(session.auth_id)
 
         # delete any old data that may be present (if cleanup on disconnect
         # failed)
         self.__clean_node_data(node=node)
 
         # store (new) node config
```

### Comparing `vantage6-server-3.8.8rc3/vantage6_server.egg-info/PKG-INFO` & `vantage6-server-3.9.0rc2/vantage6_server.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-server
-Version: 3.8.8rc3
+Version: 3.9.0rc2
 Summary: Vantage6 server
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-server Version: 3.8.8rc3 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-server Version: 3.9.0rc2 Summary: Vantage6
 server Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-server-3.8.8rc3/vantage6_server.egg-info/SOURCES.txt` & `vantage6-server-3.9.0rc2/vantage6_server.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -23,19 +23,16 @@
 vantage6/server/_data/unittest_fixtures.yaml
 vantage6/server/_data/dev/fixtures.yaml
 vantage6/server/_data/dev/node_a.yaml
 vantage6/server/_data/dev/node_b.yaml
 vantage6/server/_data/dev/server.yaml
 vantage6/server/cli/__init__.py
 vantage6/server/cli/server.py
-vantage6/server/configuration/configuration_manager.py
-vantage6/server/configuration/configuration_wizard.py
 vantage6/server/controller/__init__.py
 vantage6/server/controller/fixture.py
-vantage6/server/controller/query.py
 vantage6/server/model/__init__.py
 vantage6/server/model/algorithm_port.py
 vantage6/server/model/authenticatable.py
 vantage6/server/model/base.py
 vantage6/server/model/collaboration.py
 vantage6/server/model/member.py
 vantage6/server/model/node.py
```

