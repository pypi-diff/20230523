# Comparing `tmp/pytest-relaxed-2.0.0.tar.gz` & `tmp/pytest-relaxed-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmprat8jmcq/dist/pytest-relaxed-2.0.0.tar", last modified: Sat Dec 31 22:16:47 2022, max compression
+gzip compressed data, was "/tmp/tmp7to219d5/dist/pytest-relaxed-2.0.1.tar", last modified: Tue May 23 03:21:56 2023, max compression
```

## Comparing `pytest-relaxed-2.0.0.tar` & `pytest-relaxed-2.0.1.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2022-12-31 22:16:47.000000 pytest-relaxed-2.0.0/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2022-12-31 22:16:47.000000 pytest-relaxed-2.0.0/docs/
--rw-r--r--   0 jforcier  (1000) users      (100)    20480 2022-12-31 22:16:15.000000 pytest-relaxed-2.0.0/docs/.changelog.rst.swp
--rw-r--r--   0 jforcier  (1000) users      (100)       72 2022-06-17 18:58:26.000000 pytest-relaxed-2.0.0/docs/index.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     4564 2022-12-31 22:16:07.000000 pytest-relaxed-2.0.0/docs/changelog.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      901 2022-12-19 03:37:32.000000 pytest-relaxed-2.0.0/docs/conf.py
--rw-r--r--   0 jforcier  (1000) users      (100)      363 2022-12-31 22:15:23.000000 pytest-relaxed-2.0.0/dev-requirements.txt
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2022-12-31 22:16:47.000000 pytest-relaxed-2.0.0/pytest_relaxed.egg-info/
--rw-r--r--   0 jforcier  (1000) users      (100)    10934 2022-12-31 22:16:47.000000 pytest-relaxed-2.0.0/pytest_relaxed.egg-info/PKG-INFO
--rw-r--r--   0 jforcier  (1000) users      (100)       20 2022-12-31 22:16:47.000000 pytest-relaxed-2.0.0/pytest_relaxed.egg-info/requires.txt
--rw-r--r--   0 jforcier  (1000) users      (100)       44 2022-12-31 22:16:47.000000 pytest-relaxed-2.0.0/pytest_relaxed.egg-info/entry_points.txt
--rw-r--r--   0 jforcier  (1000) users      (100)       15 2022-12-31 22:16:47.000000 pytest-relaxed-2.0.0/pytest_relaxed.egg-info/top_level.txt
--rw-r--r--   0 jforcier  (1000) users      (100)      645 2022-12-31 22:16:47.000000 pytest-relaxed-2.0.0/pytest_relaxed.egg-info/SOURCES.txt
--rw-r--r--   0 jforcier  (1000) users      (100)        1 2022-12-31 22:16:47.000000 pytest-relaxed-2.0.0/pytest_relaxed.egg-info/dependency_links.txt
--rw-r--r--   0 jforcier  (1000) users      (100)       38 2022-12-31 22:16:47.000000 pytest-relaxed-2.0.0/setup.cfg
--rw-r--r--   0 jforcier  (1000) users      (100)     9710 2022-12-19 03:34:43.000000 pytest-relaxed-2.0.0/README.rst
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2022-12-31 22:16:47.000000 pytest-relaxed-2.0.0/tests/
--rw-r--r--   0 jforcier  (1000) users      (100)     8769 2022-12-17 02:40:44.000000 pytest-relaxed-2.0.0/tests/test_display.py
--rw-r--r--   0 jforcier  (1000) users      (100)    14305 2022-12-18 05:17:47.000000 pytest-relaxed-2.0.0/tests/test_collection.py
--rw-r--r--   0 jforcier  (1000) users      (100)      970 2022-12-17 02:39:28.000000 pytest-relaxed-2.0.0/tests/test_raises.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2110 2022-12-19 03:31:02.000000 pytest-relaxed-2.0.0/tasks.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2168 2022-12-17 04:46:25.000000 pytest-relaxed-2.0.0/setup.py
--rw-r--r--   0 jforcier  (1000) users      (100)    10934 2022-12-31 22:16:47.000000 pytest-relaxed-2.0.0/PKG-INFO
--rw-r--r--   0 jforcier  (1000) users      (100)      200 2022-06-17 18:58:26.000000 pytest-relaxed-2.0.0/MANIFEST.in
--rw-r--r--   0 jforcier  (1000) users      (100)     1314 2022-06-17 18:58:26.000000 pytest-relaxed-2.0.0/LICENSE
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2022-12-31 22:16:47.000000 pytest-relaxed-2.0.0/pytest_relaxed/
--rw-r--r--   0 jforcier  (1000) users      (100)     6973 2022-12-17 02:39:28.000000 pytest-relaxed-2.0.0/pytest_relaxed/reporter.py
--rw-r--r--   0 jforcier  (1000) users      (100)      421 2022-12-17 02:39:28.000000 pytest-relaxed-2.0.0/pytest_relaxed/raises.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2260 2022-12-19 03:35:49.000000 pytest-relaxed-2.0.0/pytest_relaxed/trap.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2216 2022-12-17 02:40:01.000000 pytest-relaxed-2.0.0/pytest_relaxed/plugin.py
--rw-r--r--   0 jforcier  (1000) users      (100)      828 2022-06-17 18:58:26.000000 pytest-relaxed-2.0.0/pytest_relaxed/fixtures.py
--rw-r--r--   0 jforcier  (1000) users      (100)     6014 2022-12-18 06:12:03.000000 pytest-relaxed-2.0.0/pytest_relaxed/classes.py
--rw-r--r--   0 jforcier  (1000) users      (100)       80 2022-12-16 23:19:57.000000 pytest-relaxed-2.0.0/pytest_relaxed/_version.py
--rw-r--r--   0 jforcier  (1000) users      (100)       88 2022-06-17 18:58:26.000000 pytest-relaxed-2.0.0/pytest_relaxed/__init__.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-23 03:21:56.000000 pytest-relaxed-2.0.1/
+-rw-r--r--   0 jforcier  (1000) users      (100)      200 2022-06-17 18:58:26.000000 pytest-relaxed-2.0.1/MANIFEST.in
+-rw-r--r--   0 jforcier  (1000) users      (100)       38 2023-05-23 03:21:56.000000 pytest-relaxed-2.0.1/setup.cfg
+-rw-r--r--   0 jforcier  (1000) users      (100)      326 2023-05-23 03:19:08.000000 pytest-relaxed-2.0.1/dev-requirements.txt
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-23 03:21:56.000000 pytest-relaxed-2.0.1/pytest_relaxed.egg-info/
+-rw-r--r--   0 jforcier  (1000) users      (100)      621 2023-05-23 03:21:56.000000 pytest-relaxed-2.0.1/pytest_relaxed.egg-info/SOURCES.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)       15 2023-05-23 03:21:56.000000 pytest-relaxed-2.0.1/pytest_relaxed.egg-info/top_level.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)        1 2023-05-23 03:21:56.000000 pytest-relaxed-2.0.1/pytest_relaxed.egg-info/dependency_links.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)       44 2023-05-23 03:21:56.000000 pytest-relaxed-2.0.1/pytest_relaxed.egg-info/entry_points.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)       20 2023-05-23 03:21:56.000000 pytest-relaxed-2.0.1/pytest_relaxed.egg-info/requires.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)    10990 2023-05-23 03:21:56.000000 pytest-relaxed-2.0.1/pytest_relaxed.egg-info/PKG-INFO
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-23 03:21:56.000000 pytest-relaxed-2.0.1/pytest_relaxed/
+-rw-r--r--   0 jforcier  (1000) users      (100)      421 2022-12-17 02:39:28.000000 pytest-relaxed-2.0.1/pytest_relaxed/raises.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2260 2022-12-19 03:35:49.000000 pytest-relaxed-2.0.1/pytest_relaxed/trap.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2216 2022-12-17 02:40:01.000000 pytest-relaxed-2.0.1/pytest_relaxed/plugin.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     6973 2022-12-17 02:39:28.000000 pytest-relaxed-2.0.1/pytest_relaxed/reporter.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       88 2022-06-17 18:58:26.000000 pytest-relaxed-2.0.1/pytest_relaxed/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     6317 2023-05-23 03:19:08.000000 pytest-relaxed-2.0.1/pytest_relaxed/classes.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       80 2023-05-23 03:21:55.000000 pytest-relaxed-2.0.1/pytest_relaxed/_version.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      828 2022-06-17 18:58:26.000000 pytest-relaxed-2.0.1/pytest_relaxed/fixtures.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1314 2022-06-17 18:58:26.000000 pytest-relaxed-2.0.1/LICENSE
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-23 03:21:56.000000 pytest-relaxed-2.0.1/tests/
+-rw-r--r--   0 jforcier  (1000) users      (100)    14782 2023-05-23 03:19:08.000000 pytest-relaxed-2.0.1/tests/test_collection.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     8769 2022-12-17 02:40:44.000000 pytest-relaxed-2.0.1/tests/test_display.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      962 2023-02-16 20:05:36.000000 pytest-relaxed-2.0.1/tests/test_raises.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-23 03:21:56.000000 pytest-relaxed-2.0.1/docs/
+-rw-r--r--   0 jforcier  (1000) users      (100)      901 2022-12-19 03:37:32.000000 pytest-relaxed-2.0.1/docs/conf.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       72 2022-06-17 18:58:26.000000 pytest-relaxed-2.0.1/docs/index.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     4871 2023-05-23 03:21:53.000000 pytest-relaxed-2.0.1/docs/changelog.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     9710 2022-12-19 03:34:43.000000 pytest-relaxed-2.0.1/README.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)    10990 2023-05-23 03:21:56.000000 pytest-relaxed-2.0.1/PKG-INFO
+-rw-r--r--   0 jforcier  (1000) users      (100)     2223 2023-02-16 20:05:36.000000 pytest-relaxed-2.0.1/setup.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2101 2023-05-23 03:19:08.000000 pytest-relaxed-2.0.1/tasks.py
```

### Comparing `pytest-relaxed-2.0.0/docs/changelog.rst` & `pytest-relaxed-2.0.1/docs/changelog.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+- :release:`2.0.1 <2023-05-22>`
+- :bug:`9` Don't try loading Pytest fixture functions as if they were test
+  functions. Classifying this as a bug even though it's a moderately sized
+  change in behavior; it's vanishingly unlikely anybody was relying on this
+  somehow! Thanks to ``@cajopa`` for the report.
 - :release:`2.0.0 <2022-12-31>`
 - :bug:`- major` Prior to version 2, we failed to correctly support true Pytest
   setup/teardown methods (i.e. ``setup_method`` and ``teardown_method``) and
   these would not get copied to inner class scopes. This has been fixed. We
   still support old nose-style ``setup``/``teardown`` for now, despite them
   going away in Pytest 8.
 - :support:`-` Modernize codebase/project a bunch:
```

### Comparing `pytest-relaxed-2.0.0/docs/conf.py` & `pytest-relaxed-2.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytest-relaxed-2.0.0/pytest_relaxed.egg-info/PKG-INFO` & `pytest-relaxed-2.0.1/pytest_relaxed.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-relaxed
-Version: 2.0.0
+Version: 2.0.1
 Summary: Relaxed test discovery/organization for pytest
 Home-page: https://pytest-relaxed.readthedocs.io/
 Author: Jeff Forcier
 Author-email: jeff@bitprophet.org
 License: BSD
 Project-URL: Source, https://github.com/bitprophet/pytest-relaxed
 Project-URL: Changelog, https://github.com/bitprophet/pytest-relaxed/blob/main/docs/changelog.rst
@@ -13,14 +13,15 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Testing
```

### Comparing `pytest-relaxed-2.0.0/pytest_relaxed.egg-info/SOURCES.txt` & `pytest-relaxed-2.0.1/pytest_relaxed.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 LICENSE
 MANIFEST.in
 README.rst
 dev-requirements.txt
 setup.py
 tasks.py
-docs/.changelog.rst.swp
 docs/changelog.rst
 docs/conf.py
 docs/index.rst
 pytest_relaxed/__init__.py
 pytest_relaxed/_version.py
 pytest_relaxed/classes.py
 pytest_relaxed/fixtures.py
```

### Comparing `pytest-relaxed-2.0.0/README.rst` & `pytest-relaxed-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-relaxed-2.0.0/tests/test_display.py` & `pytest-relaxed-2.0.1/tests/test_display.py`

 * *Files identical despite different names*

### Comparing `pytest-relaxed-2.0.0/tests/test_collection.py` & `pytest-relaxed-2.0.1/tests/test_collection.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pytest import ExitCode, mark
 
 
 # For 'testdir' fixture, mostly
 pytest_plugins = "pytester"
 
 
-class Test_pytest_collect_file(object):
+class Test_pytest_collect_file:
     def test_only_loads_dot_py_files(self, testdir):
         testdir.makepyfile(
             somefile="""
             def hello_how_are_you():
                 pass
         """
         )
@@ -175,14 +175,32 @@
         assert not re.match(r"^teardown$", stdout)
         assert not re.match(r"^setup_method$", stdout)
         assert not re.match(r"^teardown_method$", stdout)
         # Real tests not skipped
         assert "actual test here" in stdout
         assert "actual nested test here" in stdout
 
+    def test_skips_pytest_fixtures(self, testdir):
+        testdir.makepyfile(
+            foo="""
+            from pytest import fixture
+
+            @fixture
+            def pls_noload():
+                yield
+
+            def actual_test_here():
+                pass
+        """
+        )
+        stdout = testdir.runpytest("-v").stdout.str()
+        assert "actual test here" in stdout
+        # will be in stdout as a failure and warning if bug present
+        assert "pls_noload" not in stdout
+
     def test_setup_given_inner_class_instances_when_inherited(self, testdir):
         # NOTE: without this functionality in place, we still see setup()
         # called on a per-test-method basis, but where 'self' is the outer
         # class, not the inner class! so anything actually touching 'self'
         # breaks.
         # TODO: should this pattern change to be something like a pytest
         # per-class autouse fixture method?
@@ -233,15 +251,15 @@
             _util="""
             def helper():
                 pass
 
             class Helper:
                 pass
 
-            class NewHelper(object):
+            class NewHelper:
                 pass
         """
         )
         testdir.makepyfile(
             foo="""
             from _util import helper, Helper, NewHelper
 
@@ -259,15 +277,15 @@
         # Trigger is something that appears callable but isn't a real function;
         # almost any callable class seems to suffice. (Real world triggers are
         # things like invoke/fabric Task objects.)
         # Can also be triggered if our collection is buggy and does not
         # explicitly reject imported classes (i.e. if we only reject funcs).
         testdir.makepyfile(
             _util="""
-            class Callable(object):
+            class Callable:
                 def __call__(self):
                     pass
 
             helper = Callable()
 
             class HelperClass:
                 def __init__(self):
```

### Comparing `pytest-relaxed-2.0.0/tests/test_raises.py` & `pytest-relaxed-2.0.1/tests/test_raises.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     pass
 
 
 class OtherBoom(Exception):
     pass
 
 
-class Test_raises(object):
+class Test_raises:
     def test_when_given_exception_raised_no_problem(self):
         @raises(Boom)
         def kaboom():
             raise Boom
 
         kaboom()
         # If we got here, we're good...
```

### Comparing `pytest-relaxed-2.0.0/tasks.py` & `pytest-relaxed-2.0.1/tasks.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from invoke import task, Collection
-from invocations.checks import blacken
+from invocations import checks
 from invocations.packaging import release
 from invocations import docs, pytest as pytests
 
 
 @task
 def coverage(c, html=True, codecov=False):
     """
@@ -60,9 +60,9 @@
         opts=opts,
         x=x,
         k=k,
         module=module,
     )
 
 
-ns = Collection(blacken, coverage, docs, test, release)
+ns = Collection(checks, coverage, docs, test, release)
 ns.configure({"blacken": {"find_opts": "-and -not -path './build*'"}})
```

### Comparing `pytest-relaxed-2.0.0/setup.py` & `pytest-relaxed-2.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         "Development Status :: 5 - Production/Stable",
         "Framework :: Pytest",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Testing",
```

### Comparing `pytest-relaxed-2.0.0/PKG-INFO` & `pytest-relaxed-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-relaxed
-Version: 2.0.0
+Version: 2.0.1
 Summary: Relaxed test discovery/organization for pytest
 Home-page: https://pytest-relaxed.readthedocs.io/
 Author: Jeff Forcier
 Author-email: jeff@bitprophet.org
 License: BSD
 Project-URL: Source, https://github.com/bitprophet/pytest-relaxed
 Project-URL: Changelog, https://github.com/bitprophet/pytest-relaxed/blob/main/docs/changelog.rst
@@ -13,14 +13,15 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Testing
```

### Comparing `pytest-relaxed-2.0.0/LICENSE` & `pytest-relaxed-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-relaxed-2.0.0/pytest_relaxed/reporter.py` & `pytest-relaxed-2.0.1/pytest_relaxed/reporter.py`

 * *Files identical despite different names*

### Comparing `pytest-relaxed-2.0.0/pytest_relaxed/trap.py` & `pytest-relaxed-2.0.1/pytest_relaxed/trap.py`

 * *Files identical despite different names*

### Comparing `pytest-relaxed-2.0.0/pytest_relaxed/plugin.py` & `pytest-relaxed-2.0.1/pytest_relaxed/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-relaxed-2.0.0/pytest_relaxed/fixtures.py` & `pytest-relaxed-2.0.1/pytest_relaxed/fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest-relaxed-2.0.0/pytest_relaxed/classes.py` & `pytest-relaxed-2.0.1/pytest_relaxed/classes.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,19 +14,26 @@
 
 # NOTE: these are defined here for reuse by both pytest's own machinery and our
 # internal bits.
 def istestclass(name):
     return not name.startswith("_")
 
 
-def istestfunction(name):
-    return not (
-        name.startswith("_")
-        or name in ("setup", "setup_method", "teardown", "teardown_method")
+# NOTE: this is defined at top level due to a couple spots of reuse outside of
+# the mixin class itself.
+def istestfunction(obj, name):
+    is_hidden_name = name.startswith("_") or name in (
+        "setup",
+        "setup_method",
+        "teardown",
+        "teardown_method",
     )
+    # TODO: is this reliable? how about __pytest_wrapped__?
+    is_fixture = hasattr(obj, "_pytestfixturefunction")
+    return not (is_hidden_name or is_fixture)
 
 
 # All other classes in here currently inherit from PyCollector, and it is what
 # defines the default istestfunction/istestclass, so makes sense to inherit
 # from it for our mixin. (PyobjMixin, another commonly found class, offers
 # nothing of interest to us however.)
 class RelaxedMixin(PyCollector):
@@ -41,15 +48,15 @@
     # we test 'obj' for is its membership in a module, which must happen inside
     # SpecModule's override.
 
     def istestclass(self, obj, name):
         return istestclass(name)
 
     def istestfunction(self, obj, name):
-        return istestfunction(name)
+        return istestfunction(obj, name)
 
 
 class SpecModule(RelaxedMixin, Module):
     def _is_test_obj(self, test_func, obj, name):
         # First run our super() test, which should be RelaxedMixin's.
         good_name = getattr(super(), test_func)(obj, name)
         # If RelaxedMixin said no, we can't really say yes, as the name itself
@@ -116,15 +123,15 @@
                 continue
             # Functions (methods) may get skipped, or not, depending:
             # NOTE: as of pytest 7, for some reason the value appears as a
             # function and not a method (???) so covering both bases...
             if isinstance(value, (types.MethodType, types.FunctionType)):
                 # If they look like tests, they get skipped; don't want to copy
                 # tests around!
-                if istestfunction(name):
+                if istestfunction(obj, name):
                     continue
                 # Non-test == they're probably lifecycle methods
                 # (setup/teardown) or helpers (_do_thing). Rebind them to the
                 # target instance, otherwise the 'self' in the setup/helper is
                 # not the same 'self' as that in the actual test method it runs
                 # around or within!
                 setattr(obj, name, value)
```

