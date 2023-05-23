# Comparing `tmp/sqlalchemy-spanner-1.6.0.tar.gz` & `tmp/sqlalchemy-spanner-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-spanner-1.6.0.tar", last modified: Thu Apr 27 11:41:31 2023, max compression
+gzip compressed data, was "sqlalchemy-spanner-1.6.1.tar", last modified: Tue May 23 09:53:17 2023, max compression
```

## Comparing `sqlalchemy-spanner-1.6.0.tar` & `sqlalchemy-spanner-1.6.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-27 11:41:31.242700 sqlalchemy-spanner-1.6.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-04-27 11:39:23.000000 sqlalchemy-spanner-1.6.0/LICENSE
--rw-r--r--   0 root         (0)     1003    17665 2023-04-27 11:41:31.242700 sqlalchemy-spanner-1.6.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003    17292 2023-04-27 11:39:23.000000 sqlalchemy-spanner-1.6.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-27 11:41:31.238699 sqlalchemy-spanner-1.6.0/google/
--rw-rw-r--   0 root         (0)     1003      747 2023-04-27 11:39:23.000000 sqlalchemy-spanner-1.6.0/google/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-27 11:41:31.238699 sqlalchemy-spanner-1.6.0/google/cloud/
--rw-rw-r--   0 root         (0)     1003      747 2023-04-27 11:39:23.000000 sqlalchemy-spanner-1.6.0/google/cloud/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-27 11:41:31.238699 sqlalchemy-spanner-1.6.0/google/cloud/sqlalchemy_spanner/
--rw-rw-r--   0 root         (0)     1003      651 2023-04-27 11:39:23.000000 sqlalchemy-spanner-1.6.0/google/cloud/sqlalchemy_spanner/__init__.py
--rw-rw-r--   0 root         (0)     1003     1988 2023-04-27 11:39:23.000000 sqlalchemy-spanner-1.6.0/google/cloud/sqlalchemy_spanner/_opentelemetry_tracing.py
--rw-rw-r--   0 root         (0)     1003      792 2023-04-27 11:39:23.000000 sqlalchemy-spanner-1.6.0/google/cloud/sqlalchemy_spanner/provision.py
--rw-rw-r--   0 root         (0)     1003     3140 2023-04-27 11:39:23.000000 sqlalchemy-spanner-1.6.0/google/cloud/sqlalchemy_spanner/requirements.py
--rw-rw-r--   0 root         (0)     1003    50036 2023-04-27 11:39:23.000000 sqlalchemy-spanner-1.6.0/google/cloud/sqlalchemy_spanner/sqlalchemy_spanner.py
--rw-rw-r--   0 root         (0)     1003      261 2023-04-27 11:41:31.242700 sqlalchemy-spanner-1.6.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2431 2023-04-27 11:39:23.000000 sqlalchemy-spanner-1.6.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-27 11:41:31.242700 sqlalchemy-spanner-1.6.0/sqlalchemy_spanner.egg-info/
--rw-r--r--   0 root         (0)     1003    17665 2023-04-27 11:41:31.000000 sqlalchemy-spanner-1.6.0/sqlalchemy_spanner.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003      742 2023-04-27 11:41:31.000000 sqlalchemy-spanner-1.6.0/sqlalchemy_spanner.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-27 11:41:31.000000 sqlalchemy-spanner-1.6.0/sqlalchemy_spanner.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       87 2023-04-27 11:41:31.000000 sqlalchemy-spanner-1.6.0/sqlalchemy_spanner.egg-info/entry_points.txt
--rw-r--r--   0 root         (0)     1003       20 2023-04-27 11:41:31.000000 sqlalchemy-spanner-1.6.0/sqlalchemy_spanner.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-27 11:41:31.000000 sqlalchemy-spanner-1.6.0/sqlalchemy_spanner.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      155 2023-04-27 11:41:31.000000 sqlalchemy-spanner-1.6.0/sqlalchemy_spanner.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-04-27 11:41:31.000000 sqlalchemy-spanner-1.6.0/sqlalchemy_spanner.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-27 11:41:31.242700 sqlalchemy-spanner-1.6.0/test/
--rw-rw-r--   0 root         (0)     1003    69178 2023-04-27 11:39:23.000000 sqlalchemy-spanner-1.6.0/test/test_suite_13.py
--rw-rw-r--   0 root         (0)     1003    81649 2023-04-27 11:39:23.000000 sqlalchemy-spanner-1.6.0/test/test_suite_14.py
--rw-rw-r--   0 root         (0)     1003   103981 2023-04-27 11:39:23.000000 sqlalchemy-spanner-1.6.0/test/test_suite_20.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-23 09:53:17.154111 sqlalchemy-spanner-1.6.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-05-23 09:51:18.000000 sqlalchemy-spanner-1.6.1/LICENSE
+-rw-r--r--   0 root         (0)     1003    17665 2023-05-23 09:53:17.154111 sqlalchemy-spanner-1.6.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003    17292 2023-05-23 09:51:18.000000 sqlalchemy-spanner-1.6.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-23 09:53:17.150111 sqlalchemy-spanner-1.6.1/google/
+-rw-rw-r--   0 root         (0)     1003      747 2023-05-23 09:51:18.000000 sqlalchemy-spanner-1.6.1/google/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-23 09:53:17.150111 sqlalchemy-spanner-1.6.1/google/cloud/
+-rw-rw-r--   0 root         (0)     1003      747 2023-05-23 09:51:18.000000 sqlalchemy-spanner-1.6.1/google/cloud/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-23 09:53:17.150111 sqlalchemy-spanner-1.6.1/google/cloud/sqlalchemy_spanner/
+-rw-rw-r--   0 root         (0)     1003      651 2023-05-23 09:51:18.000000 sqlalchemy-spanner-1.6.1/google/cloud/sqlalchemy_spanner/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1988 2023-05-23 09:51:18.000000 sqlalchemy-spanner-1.6.1/google/cloud/sqlalchemy_spanner/_opentelemetry_tracing.py
+-rw-rw-r--   0 root         (0)     1003      792 2023-05-23 09:51:18.000000 sqlalchemy-spanner-1.6.1/google/cloud/sqlalchemy_spanner/provision.py
+-rw-rw-r--   0 root         (0)     1003     3140 2023-05-23 09:51:18.000000 sqlalchemy-spanner-1.6.1/google/cloud/sqlalchemy_spanner/requirements.py
+-rw-rw-r--   0 root         (0)     1003    50099 2023-05-23 09:51:18.000000 sqlalchemy-spanner-1.6.1/google/cloud/sqlalchemy_spanner/sqlalchemy_spanner.py
+-rw-rw-r--   0 root         (0)     1003      261 2023-05-23 09:53:17.154111 sqlalchemy-spanner-1.6.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2431 2023-05-23 09:51:18.000000 sqlalchemy-spanner-1.6.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-23 09:53:17.154111 sqlalchemy-spanner-1.6.1/sqlalchemy_spanner.egg-info/
+-rw-r--r--   0 root         (0)     1003    17665 2023-05-23 09:53:17.000000 sqlalchemy-spanner-1.6.1/sqlalchemy_spanner.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003      742 2023-05-23 09:53:17.000000 sqlalchemy-spanner-1.6.1/sqlalchemy_spanner.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-05-23 09:53:17.000000 sqlalchemy-spanner-1.6.1/sqlalchemy_spanner.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       87 2023-05-23 09:53:17.000000 sqlalchemy-spanner-1.6.1/sqlalchemy_spanner.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-05-23 09:53:17.000000 sqlalchemy-spanner-1.6.1/sqlalchemy_spanner.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-05-23 09:53:17.000000 sqlalchemy-spanner-1.6.1/sqlalchemy_spanner.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      155 2023-05-23 09:53:17.000000 sqlalchemy-spanner-1.6.1/sqlalchemy_spanner.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-05-23 09:53:17.000000 sqlalchemy-spanner-1.6.1/sqlalchemy_spanner.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-23 09:53:17.154111 sqlalchemy-spanner-1.6.1/test/
+-rw-rw-r--   0 root         (0)     1003    69178 2023-05-23 09:51:18.000000 sqlalchemy-spanner-1.6.1/test/test_suite_13.py
+-rw-rw-r--   0 root         (0)     1003    81649 2023-05-23 09:51:18.000000 sqlalchemy-spanner-1.6.1/test/test_suite_14.py
+-rw-rw-r--   0 root         (0)     1003   103981 2023-05-23 09:51:18.000000 sqlalchemy-spanner-1.6.1/test/test_suite_20.py
```

### Comparing `sqlalchemy-spanner-1.6.0/LICENSE` & `sqlalchemy-spanner-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.6.0/PKG-INFO` & `sqlalchemy-spanner-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-spanner
-Version: 1.6.0
+Version: 1.6.1
 Summary: SQLAlchemy dialect integrated into Cloud Spanner database
 Home-page: https://github.com/cloudspannerecosystem/python-spanner-sqlalchemy
 Author: Google LLC
 Author-email: cloud-spanner-developers@googlegroups.com
 Classifier: Intended Audience :: Developers
 Provides-Extra: tracing
 License-File: LICENSE
```

### Comparing `sqlalchemy-spanner-1.6.0/README.rst` & `sqlalchemy-spanner-1.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.6.0/google/__init__.py` & `sqlalchemy-spanner-1.6.1/google/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.6.0/google/cloud/__init__.py` & `sqlalchemy-spanner-1.6.1/google/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.6.0/google/cloud/sqlalchemy_spanner/__init__.py` & `sqlalchemy-spanner-1.6.1/google/cloud/sqlalchemy_spanner/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.6.0/google/cloud/sqlalchemy_spanner/_opentelemetry_tracing.py` & `sqlalchemy-spanner-1.6.1/google/cloud/sqlalchemy_spanner/_opentelemetry_tracing.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.6.0/google/cloud/sqlalchemy_spanner/provision.py` & `sqlalchemy-spanner-1.6.1/google/cloud/sqlalchemy_spanner/provision.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.6.0/google/cloud/sqlalchemy_spanner/requirements.py` & `sqlalchemy-spanner-1.6.1/google/cloud/sqlalchemy_spanner/requirements.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.6.0/google/cloud/sqlalchemy_spanner/sqlalchemy_spanner.py` & `sqlalchemy-spanner-1.6.1/google/cloud/sqlalchemy_spanner/sqlalchemy_spanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,28 +178,29 @@
     """Identifiers compiler.
 
     In Cloud Spanner backticks "`" are used for keywords escaping.
     """
 
     reserved_words = RESERVED_WORDS.copy()
     reserved_words.update(spanner_dbapi.parse_utils.SPANNER_RESERVED_KEYWORDS)
+    reserved_words_lc = set(map(str.lower, reserved_words))
 
     def __init__(self, dialect):
         super(SpannerIdentifierPreparer, self).__init__(
             dialect, initial_quote="`", final_quote="`"
         )
 
     def _requires_quotes(self, value):
         """Return True if the given identifier requires quoting."""
         lc_value = value.lower()
         if lc_value == '"unicode"':  # don't escape default Spanner colation
             return False
 
         return (
-            lc_value in self.reserved_words
+            lc_value in self.reserved_words_lc
             or value[0] in self.illegal_initial_characters
             or not self.legal_characters.match(str(value))
             or (lc_value != value)
         )
 
 
 class SpannerSQLCompiler(SQLCompiler):
```

### Comparing `sqlalchemy-spanner-1.6.0/setup.py` & `sqlalchemy-spanner-1.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.6.0/sqlalchemy_spanner.egg-info/PKG-INFO` & `sqlalchemy-spanner-1.6.1/sqlalchemy_spanner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-spanner
-Version: 1.6.0
+Version: 1.6.1
 Summary: SQLAlchemy dialect integrated into Cloud Spanner database
 Home-page: https://github.com/cloudspannerecosystem/python-spanner-sqlalchemy
 Author: Google LLC
 Author-email: cloud-spanner-developers@googlegroups.com
 Classifier: Intended Audience :: Developers
 Provides-Extra: tracing
 License-File: LICENSE
```

### Comparing `sqlalchemy-spanner-1.6.0/sqlalchemy_spanner.egg-info/SOURCES.txt` & `sqlalchemy-spanner-1.6.1/sqlalchemy_spanner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.6.0/test/test_suite_13.py` & `sqlalchemy-spanner-1.6.1/test/test_suite_13.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.6.0/test/test_suite_14.py` & `sqlalchemy-spanner-1.6.1/test/test_suite_14.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-spanner-1.6.0/test/test_suite_20.py` & `sqlalchemy-spanner-1.6.1/test/test_suite_20.py`

 * *Files identical despite different names*

