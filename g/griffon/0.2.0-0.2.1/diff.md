# Comparing `tmp/griffon-0.2.0.tar.gz` & `tmp/griffon-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griffon-0.2.0.tar", last modified: Wed May 10 08:52:14 2023, max compression
+gzip compressed data, was "griffon-0.2.1.tar", last modified: Tue May 23 07:05:16 2023, max compression
```

## Comparing `griffon-0.2.0.tar` & `griffon-0.2.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:52:14.970026 griffon-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-10 08:51:59.000000 griffon-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-10 08:52:14.970026 griffon-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-10 08:51:59.000000 griffon-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:52:14.966026 griffon-0.2.0/griffon/
--rw-r--r--   0 runner    (1001) docker     (123)    10988 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:52:14.966026 griffon-0.2.0/griffon/autocomplete/
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/autocomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:52:14.970026 griffon-0.2.0/griffon/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/commands/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/commands/docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:52:14.970026 griffon-0.2.0/griffon/commands/entities/
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/commands/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26909 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/commands/entities/community_component_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    27264 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/commands/entities/corgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/commands/entities/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14400 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/commands/entities/osidb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/commands/plugin_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:52:14.970026 griffon-0.2.0/griffon/commands/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/commands/plugins/cve_mitre.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/commands/plugins/cvelib.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/commands/plugins/fcc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/commands/plugins/go_vuln.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/commands/plugins/osv.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/commands/plugins/semgrep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/commands/process.py
--rw-r--r--   0 runner    (1001) docker     (123)    24015 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/commands/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/commands/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    38678 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:52:14.970026 griffon-0.2.0/griffon/services/
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/services/core_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    38394 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/services/core_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)    20730 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/services/core_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:52:14.970026 griffon-0.2.0/griffon/static/
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/static/default_griffonrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:52:14.966026 griffon-0.2.0/griffon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-10 08:52:14.000000 griffon-0.2.0/griffon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-10 08:52:14.000000 griffon-0.2.0/griffon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 08:52:14.000000 griffon-0.2.0/griffon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-10 08:52:14.000000 griffon-0.2.0/griffon.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-10 08:52:14.000000 griffon-0.2.0/griffon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-10 08:52:14.000000 griffon-0.2.0/griffon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-10 08:51:59.000000 griffon-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 08:52:14.970026 griffon-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-10 08:51:59.000000 griffon-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:52:14.970026 griffon-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-10 08:51:59.000000 griffon-0.2.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-10 08:51:59.000000 griffon-0.2.0/tests/test_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-10 08:51:59.000000 griffon-0.2.0/tests/test_manage.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-10 08:51:59.000000 griffon-0.2.0/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-10 08:51:59.000000 griffon-0.2.0/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-10 08:51:59.000000 griffon-0.2.0/tests/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-10 08:51:59.000000 griffon-0.2.0/tests/test_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-10 08:51:59.000000 griffon-0.2.0/tests/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:05:16.290184 griffon-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-23 07:04:57.000000 griffon-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-23 07:05:16.290184 griffon-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-23 07:04:57.000000 griffon-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:05:16.282184 griffon-0.2.1/griffon/
+-rw-r--r--   0 runner    (1001) docker     (123)    10988 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:05:16.282184 griffon-0.2.1/griffon/autocomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/autocomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:05:16.282184 griffon-0.2.1/griffon/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/commands/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/commands/docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:05:16.286184 griffon-0.2.1/griffon/commands/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/commands/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26909 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/commands/entities/community_component_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27264 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/commands/entities/corgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/commands/entities/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14400 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/commands/entities/osidb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/commands/plugin_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:05:16.286184 griffon-0.2.1/griffon/commands/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/commands/plugins/cve_mitre.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/commands/plugins/cvelib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/commands/plugins/fcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/commands/plugins/go_vuln.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/commands/plugins/osv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/commands/plugins/semgrep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/commands/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24381 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/commands/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/commands/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41808 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:05:16.286184 griffon-0.2.1/griffon/services/
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/services/core_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36478 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/services/core_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20730 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/services/core_reports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:05:16.286184 griffon-0.2.1/griffon/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-23 07:04:57.000000 griffon-0.2.1/griffon/static/default_griffonrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:05:16.282184 griffon-0.2.1/griffon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-23 07:05:16.000000 griffon-0.2.1/griffon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-23 07:05:16.000000 griffon-0.2.1/griffon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 07:05:16.000000 griffon-0.2.1/griffon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-23 07:05:16.000000 griffon-0.2.1/griffon.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-23 07:05:16.000000 griffon-0.2.1/griffon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-23 07:05:16.000000 griffon-0.2.1/griffon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-23 07:04:57.000000 griffon-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 07:05:16.290184 griffon-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-23 07:04:57.000000 griffon-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:05:16.290184 griffon-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-23 07:04:57.000000 griffon-0.2.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-23 07:04:57.000000 griffon-0.2.1/tests/test_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-23 07:04:57.000000 griffon-0.2.1/tests/test_manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-23 07:04:57.000000 griffon-0.2.1/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-23 07:04:57.000000 griffon-0.2.1/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-23 07:04:57.000000 griffon-0.2.1/tests/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-23 07:04:57.000000 griffon-0.2.1/tests/test_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-23 07:04:57.000000 griffon-0.2.1/tests/test_unit.py
```

### Comparing `griffon-0.2.0/LICENSE` & `griffon-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `griffon-0.2.0/PKG-INFO` & `griffon-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: griffon
-Version: 0.2.0
+Version: 0.2.1
 Summary: Red Hat Product Security CLI
 Home-page: https://github.com/RedHatProductSecurity/griffon
 Author: James Fuller, Red Hat Product Security
 License: MIT
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `griffon-0.2.0/README.md` & `griffon-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `griffon-0.2.0/griffon/__init__.py` & `griffon-0.2.1/griffon/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import osidb_bindings
 from osidb_bindings.bindings.python_client.models import Affect, Flaw, Tracker
 from pkg_resources import resource_filename  # type: ignore
 from rich.logging import RichHandler
 
 from griffon.output import console
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 
 if "CORGI_API_URL" not in os.environ:
     print("Must set CORGI_API_URL environment variable.")
     exit(1)
 CORGI_API_URL = os.environ["CORGI_API_URL"]
 
 if "OSIDB_API_URL" not in os.environ:
```

### Comparing `griffon-0.2.0/griffon/autocomplete/__init__.py` & `griffon-0.2.1/griffon/autocomplete/__init__.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.0/griffon/cli.py` & `griffon-0.2.1/griffon/cli.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.0/griffon/commands/configure.py` & `griffon-0.2.1/griffon/commands/configure.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.0/griffon/commands/docs.py` & `griffon-0.2.1/griffon/commands/docs.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.0/griffon/commands/entities/__init__.py` & `griffon-0.2.1/griffon/commands/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.0/griffon/commands/entities/community_component_registry.py` & `griffon-0.2.1/griffon/commands/entities/community_component_registry.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.0/griffon/commands/entities/corgi.py` & `griffon-0.2.1/griffon/commands/entities/corgi.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.0/griffon/commands/entities/helpers.py` & `griffon-0.2.1/griffon/commands/entities/helpers.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.0/griffon/commands/entities/osidb.py` & `griffon-0.2.1/griffon/commands/entities/osidb.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.0/griffon/commands/plugin_commands.py` & `griffon-0.2.1/griffon/commands/plugin_commands.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.0/griffon/commands/plugins/cve_mitre.py` & `griffon-0.2.1/griffon/commands/plugins/cve_mitre.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.0/griffon/commands/plugins/go_vuln.py` & `griffon-0.2.1/griffon/commands/plugins/go_vuln.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.0/griffon/commands/plugins/osv.py` & `griffon-0.2.1/griffon/commands/plugins/osv.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.0/griffon/commands/plugins/semgrep.py` & `griffon-0.2.1/griffon/commands/plugins/semgrep.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.0/griffon/commands/process.py` & `griffon-0.2.1/griffon/commands/process.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.0/griffon/commands/queries.py` & `griffon-0.2.1/griffon/commands/queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,22 @@
     help="Filter rh naming.",
 )
 @click.option(
     "--search-all",
     "search_all",
     is_flag=True,
     default=False,
-    help="Search all root Components and dependencies.",
+    help="Search all Components and dependencies.",
+)
+@click.option(
+    "--search-all-roots",
+    "search_all_roots",
+    is_flag=True,
+    default=False,
+    help="Search all ROOT Components and dependencies.",
 )
 @click.option(
     "--search-redhat",
     "search_redhat",
     is_flag=True,
     default=False,
     help="Search all Red Hat root Components and dependencies.",
@@ -228,14 +235,21 @@
     "--search-upstreams",
     "search_upstreams",
     is_flag=True,
     default=False,
     help="Search for Components by upstream.",
 )
 @click.option(
+    "--no-community",
+    "no_community",
+    is_flag=True,
+    default=False,
+    help="Do not search community.",
+)
+@click.option(
     "-v",
     "verbose",
     count=True,
     default=get_config_option("default", "verbosity", 0),
     help="Verbose output, more detailed search results, can be used multiple times (e.g. -vvv).",
 )  # noqa
 @click.pass_context
@@ -250,17 +264,19 @@
     affect_mode,
     sfm2_flaw_id,
     flaw_mode,
     search_latest,
     search_related_url,
     filter_rh_naming,
     search_all,
+    search_all_roots,
     search_redhat,
     search_community,
     search_upstreams,
+    no_community,
     verbose,
 ):
     with console.status("griffoning", spinner="line") as operation_status:
         """List products of a latest component."""
         if verbose:
             ctx.obj["VERBOSE"] = verbose
         if not purl and not component_name:
@@ -268,14 +284,15 @@
             click.echo("")
             click.echo("\033[1mMust supply Component name or --purl.\033[0m")
             exit(0)
 
         if (
             not search_latest
             and not search_all
+            and not search_all_roots
             and not search_related_url
             and not search_community
             and not search_upstreams
             and not search_redhat
         ):
             ctx.params["search_latest"] = True
```

### Comparing `griffon-0.2.0/griffon/commands/reports.py` & `griffon-0.2.1/griffon/commands/reports.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.0/griffon/output.py` & `griffon-0.2.1/griffon/output.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import enum
 import json
 import logging
+import re
 
 import click
 from packageurl import PackageURL
 from rich.console import Console
 from rich.text import Text
 from rich.tree import Tree
 
@@ -150,251 +151,297 @@
                 item["ofuri"],
                 item["manifest_link"],
                 no_wrap=False,
             )
     ctx.exit()
 
 
-def text_output_products_contain_component(
-    ctx, output, format, exclude_products, exclude_components
-):
-    component_name = ctx.params["component_name"]
+def text_output_products_contain_component(ctx, output, exclude_products, exclude_components):
+    search_component_name = ctx.params["component_name"]
 
     # handle single component
     if ctx.params["purl"]:
         ordered_results = sorted(output["results"], key=lambda d: d["ofuri"])
         for item in ordered_results:
             console.print(
                 Text(item["ofuri"], style="bold magenta u"),
                 no_wrap=False,
             )
         ctx.exit()
 
     # handle multiple components
     if "results" in output and output["count"] > 0:
-        ordered_results = sorted(output["results"], key=lambda d: d["product_stream"])
+        console.highlighter = None
+
+        # order at the end
+        # ordered_results = sorted(output["results"], key=lambda d: d["product_stream"])
+
+        # first flatten the tree
+        normalised_results = list()
+        if "results" in output:
+            for item in output["results"]:
+                for ps in item["product_streams"]:
+                    if ps["product_versions"][0]["name"] not in exclude_products:
+                        if not any([match in item["name"] for match in exclude_components]):
+                            c = {
+                                "product_version": ps["product_versions"][0]["name"],
+                                "product_stream": ps.get("name"),
+                                "namespace": item.get("namespace"),
+                                "name": item.get("name"),
+                                "nvr": item.get("nvr"),
+                                "type": item.get("type"),
+                                "arch": item.get("arch"),
+                                "related_url": item.get("related_url"),
+                                "purl": item.get("purl"),
+                                "sources": item.get("sources"),
+                            }
+                            if "software_build" in item:
+                                c["build_source_url"] = item["software_build"].get("source")
+                            normalised_results.append(c)
+        product_versions = sorted(
+            list(set([item["product_version"] for item in normalised_results]))
+        )
+        result_tree = {}
+        for pv in product_versions:
+            result_tree[pv] = {}
+            product_streams = sorted(
+                list(
+                    set(
+                        [
+                            item["product_stream"]
+                            for item in normalised_results
+                            if item["product_version"] == pv
+                        ]
+                    )
+                )
+            )
+            for ps in product_streams:
+                result_tree[pv][ps] = {}
+                component_names = sorted(
+                    list(
+                        set(
+                            [
+                                item["name"]
+                                for item in normalised_results
+                                if item["product_stream"] == ps
+                            ]
+                        )
+                    )
+                )
+                for cn in component_names:
+                    result_tree[pv][ps][cn] = {}
+                    nvrs = [
+                        item
+                        for item in normalised_results
+                        if item["product_stream"] == ps and item["name"] == cn
+                    ]
 
-        if exclude_products:
-            exclude_products_results = []
-            for result in ordered_results:
-                if result["product_version"] not in exclude_products:
-                    exclude_products_results.append(result)
-            ordered_results = exclude_products_results
+                    for nvr in nvrs:
+                        result_tree[pv][ps][cn][nvr["nvr"]] = nvr
 
         # TODO - MAVEN component type will require special handling
         if ctx.params["affect_mode"]:
             console.no_color = True
             console.highlighter = None
 
             flaw_mode = ctx.params["flaw_mode"]
             flaw_operation = "dry_run"
             if flaw_mode == "add":
                 flaw_operation = "new"
             if flaw_mode == "update":
                 flaw_operation = "update"
-            product_versions = sorted(
-                list(set([item["product_version"] for item in ordered_results]))
-            )
-            for pv in product_versions:
-                names = [item["name"] for item in ordered_results if pv == item["product_version"]]
-                names = list(set(names))
-                if component_name in names and f"{component_name}-container" in names:
-                    names.remove(f"{component_name}-container")
-                for name in names:
-                    if not any([match in name for match in exclude_components]):
-                        dep_name = name
+
+            for pv in result_tree.keys():
+                component_names = set()
+                for ps in result_tree[pv].keys():
+                    component_names.update(result_tree[pv][ps].keys())
+                # we should only show component name if both {component name} and {component name-container} exists # noqa
+                if (
+                    search_component_name in component_names
+                    and f"{search_component_name}-container" in component_names
+                ):
+                    component_names.remove(f"{search_component_name}-container")
+                for cn in component_names:
+                    # ensure {component name} is not in profile exclude components enum
+                    if not any([match in cn for match in exclude_components]):
                         console.print(
-                            f"{pv}/{name}={flaw_operation}",
+                            f"{pv}/{cn}={flaw_operation}",
                             no_wrap=False,
                         )
         else:
-            if ctx.obj["VERBOSE"] == 0:  # product_version X source component
-                product_versions = sorted(
-                    list(set([item["product_version"] for item in ordered_results]))
-                )
-                for pv in product_versions:
-                    names = [
-                        item["name"] for item in ordered_results if pv == item["product_version"]
-                    ]
-                    names = list(set(names))
-                    if component_name in names and f"{component_name}-container" in names:
-                        names.remove(f"{component_name}-container")
-                    for name in names:
-                        if not any([match in name for match in exclude_components]):
-                            dep_name = name.replace(component_name, f"[b]{component_name}[/b]")
-                            dep = f"[white]({dep_name})[/white]"
-                            console.print(
-                                Text(pv, style="magenta b u"),
-                                dep,
-                                no_wrap=False,
-                            )
 
-            if ctx.obj["VERBOSE"] == 1:  # product_stream X source component
-                product_streams = sorted(
-                    list(set([item["product_stream"] for item in ordered_results]))
-                )
-                for ps in product_streams:
-                    ps_components = [
-                        item for item in ordered_results if item["product_stream"] == ps
-                    ]
-                    names = sorted(list(set([item["name"] for item in ps_components])))
-                    if component_name in names and f"{component_name}-container" in names:
-                        names.remove(f"{component_name}-container")
-
-                    for name in names:
-                        if not any([match in name for match in exclude_components]):
-                            sources = []
-                            nvr = ""
-                            for item in ps_components:
-                                if item["name"] == name and "sources" in item:
-                                    sources.extend(item["sources"])
-                                if item["nvr"]:
-                                    nvr = item["nvr"]
-
-                            root_component = "root component"
-                            if sources:
-                                source_purl = PackageURL.from_string(sources[0]["purl"])
-                                root_component = sources[0]["name"]
-
-                            dep_name = nvr.replace(component_name, f"[b]{component_name}[/b]")
-                            dep = f"[white]({dep_name}, {item['type'].lower()})[/white]"
-                            console.print(
-                                Text(ps, style="magenta b u"),
-                                root_component,
-                                dep,
-                                no_wrap=False,
-                            )
-
-            if ctx.obj["VERBOSE"] == 2:  # product_stream X nvr
-                product_streams = sorted(
-                    list(set([item["product_stream"] for item in ordered_results]))
-                )
-                for ps in product_streams:
-                    ps_components = [
-                        item for item in ordered_results if item["product_stream"] == ps
-                    ]
-                    names = sorted(list(set([item["name"] for item in ps_components])))
-                    if component_name in names and f"{component_name}-container" in names:
-                        names.remove(f"{component_name}-container")
-
-                    for name in names:
-                        if not any([match in name for match in exclude_components]):
-                            sources = []
-                            nvr = ""
-                            for item in ps_components:
-                                if item["name"] == name and "sources" in item:
-                                    sources.extend(item["sources"])
-                                if item["nvr"]:
-                                    nvr = item["nvr"]
-
-                            root_component = "root component"
-                            if sources:
-                                source_purl = PackageURL.from_string(sources[0]["purl"])
-                                root_component = f"{sources[0]['purl']}-{output_version(ctx,source_purl.version)}"  # noqa
-
-                            dep_name = nvr.replace(component_name, f"[b]{component_name}[/b]")
-                            dep = f"[white]({dep_name}, {item['type'].lower()})[/white]"
-                            console.print(
-                                Text(ps, style="magenta b u"),
-                                root_component,
-                                dep,
-                                no_wrap=False,
-                            )
-
-            if ctx.obj["VERBOSE"] == 3:  # source url, upstream
-                product_streams = sorted(
-                    list(set([item["product_stream"] for item in ordered_results]))
-                )
-                for ps in product_streams:
-                    ps_components = [
-                        item for item in ordered_results if item["product_stream"] == ps
-                    ]
-                    names = sorted(list(set([item["name"] for item in ps_components])))
-                    if component_name in names and f"{component_name}-container" in names:
-                        names.remove(f"{component_name}-container")
-                    for name in names:
-                        if not any([match in name for match in exclude_components]):
-                            sources = []
-                            related_url = ""
-                            build_source_url = ""
-                            nvr = ""
-                            for item in ps_components:
-                                if item["name"] == name:
-                                    if item["nvr"]:
-                                        nvr = item["nvr"]
-                                    if "sources" in item:
-                                        sources.extend(item["sources"])
-                                    if item["related_url"]:
-                                        related_url = item["related_url"]
-                                    if item["build_source_url"]:
-                                        build_source_url = item["build_source_url"]
-                            root_component = "root component"
-                            if sources:
-                                source_purl = PackageURL.from_string(sources[0]["purl"])
-                                root_component = f"{sources[0]['purl']}-{output_version(ctx,source_purl.version)}"  # noqa
-                            dep_name = nvr.replace(component_name, f"[b]{component_name}[/b]")
-                            dep = f"[white]({dep_name}, {item['type'].lower()})[/white]"
-                            related_url = related_url.replace(
-                                component_name, f"[b]{component_name}[/b]"
+            if ctx.obj["VERBOSE"] == 0:  # product_version X component_name
+                for pv in result_tree.keys():
+                    component_names = set()
+                    for ps in result_tree[pv].keys():
+                        component_names.update(result_tree[pv][ps].keys())
+                    # we should only show component name if both {component name} and {component name-container} exists # noqa
+                    if (
+                        search_component_name in component_names
+                        and f"{search_component_name}-container" in component_names
+                    ):
+                        component_names.remove(f"{search_component_name}-container")
+                    for cn in component_names:
+                        # ensure {component name} is not in profile exclude components enum
+                        if not any([match in cn for match in exclude_components]):
+                            # highlight search term
+                            dep_name = re.sub(
+                                search_component_name, f"[b]{search_component_name}[/b]", cn
                             )
+                            dep = f"[grey93]{dep_name}[/grey93]"
                             console.print(
-                                Text(ps, style="magenta b u"),
-                                root_component,
-                                dep,
-                                related_url,
-                                no_wrap=False,
-                            )
-            if ctx.obj["VERBOSE"] > 3:  # source url, upstream
-                product_streams = sorted(
-                    list(set([item["product_stream"] for item in ordered_results]))
-                )
-                for ps in product_streams:
-                    ps_components = [
-                        item for item in ordered_results if item["product_stream"] == ps
-                    ]
-                    names = sorted(list(set([item["name"] for item in ps_components])))
-                    if component_name in names and f"{component_name}-container" in names:
-                        names.remove(f"{component_name}-container")
-                    for name in names:
-                        if not any([match in name for match in exclude_components]):
-                            sources = []
-                            related_url = ""
-                            build_source_url = ""
-                            nvr = ""
-                            for item in ps_components:
-                                if item["name"] == name:
-                                    if item["nvr"]:
-                                        nvr = item["nvr"]
-                                    if "sources" in item:
-                                        sources.extend(item["sources"])
-                                    if item["related_url"]:
-                                        related_url = item["related_url"]
-                                    if item["build_source_url"]:
-                                        build_source_url = item["build_source_url"]
-                            root_component = "root component"
-                            if sources:
-                                source_purl = PackageURL.from_string(sources[0]["purl"])
-                                root_component = f"{sources[0]['purl']}-{output_version(ctx,source_purl.version)}"  # noqa
-                            upstream = ""
-                            if item["upstream_purl"]:
-                                upstream = f"[cyan]{item['upstream_purl']}[/cyan]"
-                            dep_name = nvr.replace(component_name, f"[b]{component_name}[/b]")
-                            dep = f"[white]({dep_name}, {item['type'].lower()})[/white]"
-                            related_url = related_url.replace(
-                                component_name, f"[b]{component_name}[/b]"
-                            )
-                            console.print(
-                                Text(ps, style="magenta b u"),
-                                root_component,
+                                Text(pv, style="magenta b u"),
                                 dep,
-                                related_url,
-                                build_source_url,
-                                upstream,
                                 no_wrap=False,
                             )
+            if ctx.obj["VERBOSE"] == 1:  # product_stream X nvr x related_url
+                for pv in result_tree.keys():
+                    for ps in result_tree[pv].keys():
+                        for cn in result_tree[pv][ps].keys():
+                            # ensure {component name} is not in profile exclude components enum
+                            if not any([match in cn for match in exclude_components]):
+                                for nvr in result_tree[pv][ps][cn].keys():
+                                    # highlight search term
+                                    dep_name = re.sub(
+                                        search_component_name,
+                                        f"[b]{search_component_name}[/b]",
+                                        nvr,
+                                    )
+                                    dep = f"[grey93]{dep_name}[/grey93]"
+                                    related_url = ""
+                                    if result_tree[pv][ps][cn][nvr]["related_url"]:
+                                        related_url = re.sub(
+                                            search_component_name,
+                                            f"[b]{search_component_name}[/b]",
+                                            result_tree[pv][ps][cn][nvr]["related_url"],
+                                        )
+                                    if result_tree[pv][ps][cn][nvr]["sources"]:
+                                        source_component_names = list(
+                                            set(
+                                                [
+                                                    source["name"]
+                                                    for source in result_tree[pv][ps][cn][nvr][
+                                                        "sources"
+                                                    ]
+                                                ]
+                                            )
+                                        )
+                                        for source_name in source_component_names:
+                                            console.print(
+                                                Text(ps, style="magenta b u"),
+                                                source_name,
+                                                dep,
+                                                f"([grey]{related_url}[/grey])",
+                                                no_wrap=False,
+                                            )
+                                    else:
+                                        console.print(
+                                            Text(ps, style="magenta b u"),
+                                            dep,
+                                            f"([grey]{related_url}[/grey])",
+                                            no_wrap=False,
+                                        )
+            if ctx.obj["VERBOSE"] == 2:  # product_stream X nvr x related_url x build_source_url
+                for pv in result_tree.keys():
+                    for ps in result_tree[pv].keys():
+                        for cn in result_tree[pv][ps].keys():
+                            if not any([match in cn for match in exclude_components]):
+                                for nvr in result_tree[pv][ps][cn].keys():
+                                    dep_name = re.sub(
+                                        search_component_name,
+                                        f"[b]{search_component_name}[/b]",
+                                        nvr,
+                                    )
+                                    dep = f"[grey93]{dep_name}[/grey93]"
+                                    related_url = ""
+                                    if result_tree[pv][ps][cn][nvr]["related_url"]:
+                                        related_url = re.sub(
+                                            search_component_name,
+                                            f"[b]{search_component_name}[/b]",
+                                            result_tree[pv][ps][cn][nvr]["related_url"],
+                                        )
+                                    build_source_url = ""
+                                    if result_tree[pv][ps][cn][nvr]["build_source_url"]:
+                                        build_source_url = result_tree[pv][ps][cn][nvr][
+                                            "build_source_url"
+                                        ]
+                                    if result_tree[pv][ps][cn][nvr]["sources"]:
+                                        source_component_names = list(
+                                            set(
+                                                [
+                                                    source["name"]
+                                                    for source in result_tree[pv][ps][cn][nvr][
+                                                        "sources"
+                                                    ]
+                                                ]
+                                            )
+                                        )
+                                        for source_name in source_component_names:
+                                            console.print(
+                                                Text(ps, style="magenta b u"),
+                                                source_name,
+                                                dep,
+                                                f"([grey]{related_url}[/grey])",
+                                                no_wrap=False,
+                                            )
+                                    else:
+                                        console.print(
+                                            Text(ps, style="magenta b u"),
+                                            dep,
+                                            f"([grey]{related_url}[/grey])",
+                                            f"([grey]{build_source_url}[/grey])",
+                                            no_wrap=False,
+                                        )
+            if ctx.obj["VERBOSE"] > 2:  # product_stream X purl x related_url x build_source_url
+                for pv in result_tree.keys():
+                    for ps in result_tree[pv].keys():
+                        for cn in result_tree[pv][ps].keys():
+                            if not any([match in cn for match in exclude_components]):
+                                for nvr in result_tree[pv][ps][cn].keys():
+                                    purl = result_tree[pv][ps][cn][nvr]["purl"]
+                                    dep = f"[grey93]{purl}[/grey93]"
+                                    related_url = ""
+                                    if result_tree[pv][ps][cn][nvr]["related_url"]:
+                                        related_url = re.sub(
+                                            search_component_name,
+                                            f"[b]{search_component_name}[/b]",
+                                            result_tree[pv][ps][cn][nvr]["related_url"],
+                                        )
+                                    build_source_url = ""
+                                    if result_tree[pv][ps][cn][nvr]["build_source_url"]:
+                                        build_source_url = result_tree[pv][ps][cn][nvr][
+                                            "build_source_url"
+                                        ]
+                                    if result_tree[pv][ps][cn][nvr]["sources"]:
+                                        source_component_names = list(
+                                            set(
+                                                [
+                                                    source["name"]
+                                                    for source in result_tree[pv][ps][cn][nvr][
+                                                        "sources"
+                                                    ]
+                                                ]
+                                            )
+                                        )
+                                        for source_name in source_component_names:
+                                            console.print(
+                                                Text(ps, style="magenta b u"),
+                                                source_name,
+                                                dep,
+                                                f"([grey]{related_url}[/grey])",
+                                                no_wrap=False,
+                                            )
+                                    else:
+                                        console.print(
+                                            Text(ps, style="magenta b u"),
+                                            f"[white]{purl}[/white]",
+                                            f"([grey]{related_url}[/grey])",
+                                            f"([grey]{build_source_url}[/grey])",
+                                            no_wrap=False,
+                                        )
 
         ctx.exit()
 
 
 def text_output_components_contain_component(ctx, output, format, exclude_components):
     if "results" in output:
         for item in output["results"]:
@@ -826,15 +873,15 @@
     if ctx and "FORMAT" in ctx.obj:
         format = OUTPUT_FORMAT(ctx.obj["FORMAT"])
     if format is OUTPUT_FORMAT.TEXT:
         if ctx.info_name == "product-summary":
             text_output_product_summary(ctx, output, format, exclude_products)
         if ctx.info_name == "products-contain-component":
             text_output_products_contain_component(
-                ctx, output, format, exclude_products, exclude_components
+                ctx, output, exclude_products, exclude_components
             )
         if ctx.info_name == "components-contain-component":
             text_output_components_contain_component(ctx, output, format, exclude_components)
         if ctx.info_name == "components-affected-by-flaw":
             text_output_components_affected_by_cve(ctx, output, format)
         if ctx.info_name == "products-affected-by-flaw":
             text_output_products_affected_by_cve(ctx, output, format, exclude_products)
```

### Comparing `griffon-0.2.0/griffon/services/__init__.py` & `griffon-0.2.1/griffon/services/__init__.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.0/griffon/services/core_process.py` & `griffon-0.2.1/griffon/services/core_process.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.0/griffon/services/core_queries.py` & `griffon-0.2.1/griffon/services/core_queries.py`

 * *Files 3% similar despite different names*

```diff
@@ -195,15 +195,15 @@
         return c["product_streams"]
 
 
 def output_component(pv, ps, c):
     is_root = False
     if (c.arch == "src" and c.type == "RPM") or (c.arch == "noarch" and c.type == "OCI"):
         is_root = True
-    sources = [{"purl": source["purl"]} for source in c.sources]
+    sources = [source for source in c.sources]
     component = {
         "is_root": is_root,
         "product_version": pv["name"],
         "product_version_ofuri": pv["ofuri"],
         "product_stream": ps["name"],
         "product_stream_ofuri": ps["ofuri"],
         "product_active": True,
@@ -212,19 +212,19 @@
         "namespace": str(c.namespace),
         "name": c.name,
         "arch": c.arch,
         "release": c.release,
         "version": c.version,
         "sources": sources,
         "nvr": c.nvr,
-        "build_id": None,
-        "build_type": None,
-        "build_source_url": None,
-        "related_url": None,
-        "upstream_purl": None,
+        # "build_id": None,
+        # "build_type": None,
+        # "build_source_url": None,
+        # "related_url": None,
+        # "upstream_purl": None,
     }
     if c.software_build:
         component["build_id"] = str(c.software_build.build_id)
         component["build_type"] = str(c.software_build.build_type)
         component["build_name"] = str(c.software_build.name)
         component["build_source_url"] = str(c.software_build.source)
     if c.upstreams:
@@ -236,15 +236,15 @@
     components = list()
     if component_cnt < 120:
         components.extend(components_initial.results)
     elif component_cnt > 120:
         components.extend(components_initial.results)
         with concurrent.futures.ThreadPoolExecutor() as executor:
             futures = []
-            for batch in range(120, component_cnt, 120):
+            for batch in range(120, 600, 120):
                 futures.append(
                     executor.submit(
                         corgi_session.components.retrieve_list,
                         **params,
                         offset=batch,
                         limit=120,  # noqa
                     )
@@ -267,101 +267,101 @@
         "purl",
         "arch",
         "namespace",
         "component_type",
         "strict_name_search",
         "search_latest",
         "search_all",
+        "search_all_roots",
         "search_related_url",
         "search_redhat",
         "search_community",
         "search_upstreams",
         "filter_rh_naming",
+        "no_community",
     ]
 
     def __init__(self, params: dict) -> None:
         self.corgi_session = CorgiService.create_session()
         self.params = params
-        self.component_name = self.params.get("component_name")
-        self.component_type = self.params.get("component_type")
+        self.component_name = self.params.get("component_name", "")
+        self.component_type = self.params.get("component_type", "")
         self.strict_name_search = self.params.get("strict_name_search")
         self.search_deps = self.params.get("search_deps")
         self.ns = self.params.get("namespace")
         self.search_latest = self.params.get("search_latest")
         self.search_all = self.params.get("search_all")
+        self.search_all_roots = self.params.get("search_all_roots")
         self.search_related_url = self.params.get("search_related_url")
         self.search_redhat = self.params.get("search_redhat")
         self.search_community = self.params.get("search_community")
         self.search_upstreams = self.params.get("search_upstreams")
         self.filter_rh_naming = self.params.get("filter_rh_naming")
+        self.no_community = self.params.get("no_community")
 
     def execute(self) -> List[Dict[str, Any]]:
         results = []
+        params = {
+            "include_fields": "link,purl,type,name,related_url,namespace,software_build,nvr,sources.purl,sources.name,upstreams.purl,upstreams.name,release,version,arch,product_streams.product_versions,product_streams.name,product_streams.ofuri",  # noqa
+        }
 
         if self.search_latest:
-            params = {
-                "latest_components_by_streams": True,
-                "include_fields": "link,purl,type,name,related_url,namespace,software_build,nvr,upstreams.purl,upstreams.name,release,version,arch,sources.name,sources.purl,sources.name,product_versions.name,product_versions.ofuri,product_streams.name,product_streams.ofuri",  # noqa
-            }
+            params["latest_components_by_streams"] = "True"
             if not self.strict_name_search:
                 params["re_name"] = self.component_name
             else:
                 params["name"] = self.component_name
             if self.ns:
                 params["namespace"] = self.ns
 
             component_initial = self.corgi_session.components.retrieve_list(limit=120, **params)
             latest_components: list = async_retrieve_components(
                 self.corgi_session, params, component_initial, component_initial.count
             )
-            for c in latest_components:
-                if self.strict_name_search:
-                    if c.name != self.component_name:
-                        continue
-                for pv in c.product_versions:
-                    for ps in c.product_streams:
-                        component = output_component(pv, ps, c)
-                        results.append(component)
+            results.extend(latest_components)
 
         if self.search_related_url:
             # Note: related_url filter has no concept of strict
-            params = {
-                "include_fields": "link,purl,type,name,related_url,namespace,software_build,nvr,upstreams.purl,upstreams.name,release,version,arch,sources.name,sources.purl,sources.name,product_versions.name,product_versions.ofuri,product_streams.name,product_streams.ofuri",  # noqa
-                "related_url": self.component_name,
-            }
+            params["related_url"] = self.component_name
             params["namespace"] = "REDHAT"
             if self.component_type:
                 params["type"] = self.component_type
 
             component_initial = self.corgi_session.components.retrieve_list(limit=120, **params)
             related_url_components: list = async_retrieve_components(
                 self.corgi_session, params, component_initial, component_initial.count
             )
-            for c in related_url_components:
-                if self.strict_name_search:
-                    if c.name != self.component_name:
-                        continue
-                for pv in c.product_versions:
-                    for ps in c.product_streams:
-                        results.append(output_component(pv, ps, c))
+            results.extend(related_url_components)
 
         if self.search_all:
-            params = {
-                "type": "RPM",
-                "arch": "src",
-                "include_fields": "link,purl,type,name,related_url,namespace,software_build,nvr,upstreams.purl,upstreams.name,release,version,arch,sources.name,sources.purl,sources.name,product_versions.name,product_versions.ofuri,product_streams.name,product_streams.ofuri",  # noqa
-            }
+            # params["type"] ="RPM"
             if not self.strict_name_search:
                 params["re_name"] = self.component_name
             else:
                 params["name"] = self.component_name
-
             if self.component_type:
                 params["type"] = self.component_type
 
+            all_component_initial = self.corgi_session.components.retrieve_list(limit=120, **params)
+            all_components: list = async_retrieve_components(
+                self.corgi_session,
+                params,
+                all_component_initial,
+                all_component_initial.count,
+            )
+            results.extend(all_components)
+
+        if self.search_all_roots:
+            params["type"] = "RPM"
+            params["arch"] = "src"
+            if not self.strict_name_search:
+                params["re_name"] = self.component_name
+            else:
+                params["name"] = self.component_name
+
             all_src_component_initial = self.corgi_session.components.retrieve_list(
                 limit=120, **params
             )
             all_src_components: list = async_retrieve_components(
                 self.corgi_session,
                 params,
                 all_src_component_initial,
@@ -374,50 +374,33 @@
             )
             all_noarch_components: list = async_retrieve_components(
                 self.corgi_session,
                 params,
                 all_noarch_component_initial,
                 all_noarch_component_initial.count,
             )
-            all_components = all_src_components + all_noarch_components
-
-            for c in all_components:
-                if self.strict_name_search:
-                    if c.name != self.component_name:
-                        continue
-                for pv in c.product_versions:
-                    for ps in c.product_streams:
-                        results.append(output_component(pv, ps, c))
+            all_root_components = all_src_components + all_noarch_components
+            results.extend(all_root_components)
 
         if self.search_upstreams:
             # Note: upstreams only takes a purl ... so we must use re_upstreams for
             # both strict and not strict search
-            params = params = {
-                "include_fields": "link,purl,type,name,namespace,software_build,nvr,related_url,upstreams.purl,upstreams.name,release,version,arch,sources.name,sources.purl,sources.name,product_versions.name,product_versions.ofuri,product_streams.name,product_streams.ofuri",  # noqa
-                "namespace": "UPSTREAM",
-            }
-
+            params["namespace"] = "UPSTREAM"
             if not self.strict_name_search:
                 params["re_name"] = self.component_name
             else:
                 params["name"] = self.component_name
             if self.component_type:
                 params["type"] = self.component_type
 
             component_initial = self.corgi_session.components.retrieve_list(limit=120, **params)
             upstream_components: list = async_retrieve_components(
                 self.corgi_session, params, component_initial, component_initial.count
             )
-            for c in upstream_components:
-                if self.strict_name_search:
-                    if c.name != self.component_name:
-                        continue
-                for pv in c.product_versions:
-                    for ps in c.product_streams:
-                        results.append(output_component(pv, ps, c))
+            results.extend(upstream_components)
 
         if self.filter_rh_naming:
             flags = re.IGNORECASE
             patterns = [
                 # binutils
                 re.compile(
                     f"(devtoolset\\-[0-9]+\\-|mingw\\-|gcc\\-toolset\\-[0-9]+\\-)?{self.component_name}[0-9\\.]*$",  # noqa
@@ -450,22 +433,20 @@
                         if m:
                             filtered_results.append(result)
                             is_matched = True
                             break
 
             results = filtered_results
 
-        if self.search_community or self.search_all:
+        if not self.no_community and (
+            self.search_community or self.search_all or self.search_all_roots
+        ):
             self.community_session = CommunityComponentService.create_session()
-
-            params = {
-                "include_fields": "link,purl,type,name,namespace,software_build,nvr,upstreams.purl,upstreams.name,release,version,arch,sources.name,sources.purl,sources.name,product_versions.name,product_versions.ofuri,product_streams.name,product_streams.ofuri",  # noqa
-                "type": "RPM",
-                "arch": "src",
-            }
+            params["type"] = "RPM"
+            params["arch"] = "src"
             if not self.strict_name_search:
                 params["re_name"] = self.component_name
             else:
                 params["name"] = self.component_name
 
             if self.component_type:
                 params["type"] = self.component_type
@@ -482,21 +463,15 @@
             commmunity_noarch_components: list = async_retrieve_components(
                 self.community_session,
                 params,
                 component_initial_noarch,
                 component_initial_noarch.count,
             )
             community_components = commmunity_src_components + commmunity_noarch_components
-            for c in community_components:
-                if self.strict_name_search:
-                    if c.name != self.component_name:
-                        continue
-                for pv in c.product_versions:
-                    for ps in c.product_streams:
-                        results.append(output_component(pv, ps, c))
+            results.extend(community_components)
 
         return results
 
 
 class components_containing_specific_component_query:
     """What components contain a specific component?"""
```

### Comparing `griffon-0.2.0/griffon/services/core_reports.py` & `griffon-0.2.1/griffon/services/core_reports.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.0/griffon/static/default_griffonrc` & `griffon-0.2.1/griffon/static/default_griffonrc`

 * *Files identical despite different names*

### Comparing `griffon-0.2.0/griffon.egg-info/PKG-INFO` & `griffon-0.2.1/griffon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: griffon
-Version: 0.2.0
+Version: 0.2.1
 Summary: Red Hat Product Security CLI
 Home-page: https://github.com/RedHatProductSecurity/griffon
 Author: James Fuller, Red Hat Product Security
 License: MIT
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `griffon-0.2.0/griffon.egg-info/SOURCES.txt` & `griffon-0.2.1/griffon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `griffon-0.2.0/pyproject.toml` & `griffon-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `griffon-0.2.0/setup.py` & `griffon-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.0/tests/test_cli.py` & `griffon-0.2.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.0/tests/test_entities.py` & `griffon-0.2.1/tests/test_entities.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.0/tests/test_manage.py` & `griffon-0.2.1/tests/test_manage.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.0/tests/test_plugins.py` & `griffon-0.2.1/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.0/tests/test_process.py` & `griffon-0.2.1/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.0/tests/test_queries.py` & `griffon-0.2.1/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.0/tests/test_reports.py` & `griffon-0.2.1/tests/test_reports.py`

 * *Files identical despite different names*

### Comparing `griffon-0.2.0/tests/test_unit.py` & `griffon-0.2.1/tests/test_unit.py`

 * *Files identical despite different names*

