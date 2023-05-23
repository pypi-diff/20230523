# Comparing `tmp/sphinx-proofscape-0.3.2.tar.gz` & `tmp/sphinx-proofscape-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-proofscape-0.3.2.tar", last modified: Tue May 23 14:55:20 2023, max compression
+gzip compressed data, was "sphinx-proofscape-0.4.0.tar", last modified: Tue May 23 15:56:46 2023, max compression
```

## Comparing `sphinx-proofscape-0.3.2.tar` & `sphinx-proofscape-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2023-05-23 14:55:20.544999 sphinx-proofscape-0.3.2/
--rw-r--r--   0 skieffer   (501) staff       (20)    11359 2022-08-23 20:24:57.000000 sphinx-proofscape-0.3.2/LICENSE
--rw-r--r--   0 skieffer   (501) staff       (20)       66 2023-01-01 18:47:48.000000 sphinx-proofscape-0.3.2/NOTICE
--rw-r--r--   0 skieffer   (501) staff       (20)      610 2023-05-23 14:55:20.545135 sphinx-proofscape-0.3.2/PKG-INFO
--rw-r--r--   0 skieffer   (501) staff       (20)      193 2022-08-23 21:45:08.000000 sphinx-proofscape-0.3.2/README.rst
--rw-r--r--   0 skieffer   (501) staff       (20)       81 2023-01-19 20:31:13.000000 sphinx-proofscape-0.3.2/pyproject.toml
--rw-r--r--   0 skieffer   (501) staff       (20)      671 2023-05-23 14:55:20.546101 sphinx-proofscape-0.3.2/setup.cfg
-drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2023-05-23 14:55:20.541116 sphinx-proofscape-0.3.2/sphinx_proofscape/
--rw-r--r--   0 skieffer   (501) staff       (20)     4154 2023-05-23 14:39:25.000000 sphinx-proofscape-0.3.2/sphinx_proofscape/__init__.py
--rw-r--r--   0 skieffer   (501) staff       (20)    11594 2023-01-01 18:47:48.000000 sphinx-proofscape-0.3.2/sphinx_proofscape/chart_widget.py
--rw-r--r--   0 skieffer   (501) staff       (20)    12128 2023-01-01 18:47:48.000000 sphinx-proofscape-0.3.2/sphinx_proofscape/lang_exts.py
--rw-r--r--   0 skieffer   (501) staff       (20)     7284 2023-01-01 18:47:48.000000 sphinx-proofscape-0.3.2/sphinx_proofscape/lexer.py
-drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2023-05-23 14:55:20.543937 sphinx-proofscape-0.3.2/sphinx_proofscape.egg-info/
--rw-r--r--   0 skieffer   (501) staff       (20)      610 2023-05-23 14:55:20.000000 sphinx-proofscape-0.3.2/sphinx_proofscape.egg-info/PKG-INFO
--rw-r--r--   0 skieffer   (501) staff       (20)      400 2023-05-23 14:55:20.000000 sphinx-proofscape-0.3.2/sphinx_proofscape.egg-info/SOURCES.txt
--rw-r--r--   0 skieffer   (501) staff       (20)        1 2023-05-23 14:55:20.000000 sphinx-proofscape-0.3.2/sphinx_proofscape.egg-info/dependency_links.txt
--rw-r--r--   0 skieffer   (501) staff       (20)       70 2023-05-23 14:55:20.000000 sphinx-proofscape-0.3.2/sphinx_proofscape.egg-info/requires.txt
--rw-r--r--   0 skieffer   (501) staff       (20)       18 2023-05-23 14:55:20.000000 sphinx-proofscape-0.3.2/sphinx_proofscape.egg-info/top_level.txt
-drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2023-05-23 14:55:20.544354 sphinx-proofscape-0.3.2/tests/
--rw-r--r--   0 skieffer   (501) staff       (20)    10198 2023-05-23 14:30:49.000000 sphinx-proofscape-0.3.2/tests/test_extension.py
+drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2023-05-23 15:56:46.967822 sphinx-proofscape-0.4.0/
+-rw-r--r--   0 skieffer   (501) staff       (20)    11359 2022-08-23 20:24:57.000000 sphinx-proofscape-0.4.0/LICENSE
+-rw-r--r--   0 skieffer   (501) staff       (20)       66 2023-01-01 18:47:48.000000 sphinx-proofscape-0.4.0/NOTICE
+-rw-r--r--   0 skieffer   (501) staff       (20)      815 2023-05-23 15:56:46.967975 sphinx-proofscape-0.4.0/PKG-INFO
+-rw-r--r--   0 skieffer   (501) staff       (20)      398 2023-05-23 15:55:50.000000 sphinx-proofscape-0.4.0/README.rst
+-rw-r--r--   0 skieffer   (501) staff       (20)       81 2023-05-23 15:00:45.000000 sphinx-proofscape-0.4.0/pyproject.toml
+-rw-r--r--   0 skieffer   (501) staff       (20)      671 2023-05-23 15:56:46.968808 sphinx-proofscape-0.4.0/setup.cfg
+drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2023-05-23 15:56:46.964818 sphinx-proofscape-0.4.0/sphinx_proofscape/
+-rw-r--r--   0 skieffer   (501) staff       (20)     3914 2023-05-23 15:55:50.000000 sphinx-proofscape-0.4.0/sphinx_proofscape/__init__.py
+-rw-r--r--   0 skieffer   (501) staff       (20)    11594 2023-01-01 18:47:48.000000 sphinx-proofscape-0.4.0/sphinx_proofscape/chart_widget.py
+-rw-r--r--   0 skieffer   (501) staff       (20)    12128 2023-01-01 18:47:48.000000 sphinx-proofscape-0.4.0/sphinx_proofscape/lang_exts.py
+-rw-r--r--   0 skieffer   (501) staff       (20)     7284 2023-01-01 18:47:48.000000 sphinx-proofscape-0.4.0/sphinx_proofscape/lexer.py
+drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2023-05-23 15:56:46.966735 sphinx-proofscape-0.4.0/sphinx_proofscape.egg-info/
+-rw-r--r--   0 skieffer   (501) staff       (20)      815 2023-05-23 15:56:46.000000 sphinx-proofscape-0.4.0/sphinx_proofscape.egg-info/PKG-INFO
+-rw-r--r--   0 skieffer   (501) staff       (20)      400 2023-05-23 15:56:46.000000 sphinx-proofscape-0.4.0/sphinx_proofscape.egg-info/SOURCES.txt
+-rw-r--r--   0 skieffer   (501) staff       (20)        1 2023-05-23 15:56:46.000000 sphinx-proofscape-0.4.0/sphinx_proofscape.egg-info/dependency_links.txt
+-rw-r--r--   0 skieffer   (501) staff       (20)       70 2023-05-23 15:56:46.000000 sphinx-proofscape-0.4.0/sphinx_proofscape.egg-info/requires.txt
+-rw-r--r--   0 skieffer   (501) staff       (20)       18 2023-05-23 15:56:46.000000 sphinx-proofscape-0.4.0/sphinx_proofscape.egg-info/top_level.txt
+drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2023-05-23 15:56:46.967201 sphinx-proofscape-0.4.0/tests/
+-rw-r--r--   0 skieffer   (501) staff       (20)     4539 2023-05-23 15:55:50.000000 sphinx-proofscape-0.4.0/tests/test_extension.py
```

### Comparing `sphinx-proofscape-0.3.2/LICENSE` & `sphinx-proofscape-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-proofscape-0.3.2/PKG-INFO` & `sphinx-proofscape-0.4.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: sphinx-proofscape
-Version: 0.3.2
+Version: 0.4.0
 Summary: Sphinx extension for Proofscape
 Home-page: https://github.com/proofscape/sphinx-proofscape/
 License: Apache 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 License-File: NOTICE
 
 sphinx-proofscape
 =================
 
-Sphinx extension for adding Proofscape widgets to your documents.
+Sphinx extension for use with Proofscape.
 
-Currently, only *chart widgets* are supported.
+In versions ``0.3.x``, this package provided both syntax highlighting (for the
+Proofscape module language and Meson language), and roles and directives for
+chart widgets.
 
-Support for all widget types is planned.
+In versions ``0.4.x``, only syntax highlighting is provided. Development of
+widget roles and directives has moved to the ``pise/server`` project.
```

### Comparing `sphinx-proofscape-0.3.2/setup.cfg` & `sphinx-proofscape-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `sphinx-proofscape-0.3.2/sphinx_proofscape/__init__.py` & `sphinx-proofscape-0.4.0/sphinx_proofscape/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     PfscDefnsDirective,
 )
 from sphinx_proofscape.lexer import (
     MesonLexer, ProofscapeLexer, MesonBnfGrammarLexer,
 )
 
 
-__version__ = '0.3.2'
+__version__ = '0.4.0'
 
 
 ###############################################################################
 # Standard purge & merge
 # See e.g. https://www.sphinx-doc.org/en/master/development/tutorials/todo.html
 
 
@@ -74,33 +74,24 @@
         app.add_js_file(None, body=body)
 
 
 ###############################################################################
 
 
 def setup(app):
-
-    app.add_config_value('pfsc_repopath', None, 'html')
-    app.add_config_value('pfsc_repovers', None, 'html')
-    app.add_config_value('pfsc_import_repos', None, 'html')
-
-    app.add_node(chartwidget,
-                 html=(visit_chartwidget_html, depart_chartwidget_html))
-
-    app.add_role('pfsc-chart', PfscChartRole())
-    app.add_directive('pfsc-chart', PfscChartDirective)
-    app.add_directive('pfsc-defns', PfscDefnsDirective)
+    # In version 0.3.x, we defined more than just the lexers, including roles,
+    # directives, etc.
+    # In version 0.4.x, we define only the lexers, while everything else has
+    # moved into `pise/server`.
+    # In future versions, we may move everything back into this package, which
+    # would then depend on a refactored `pfsc-core` package, yet to come.
 
     app.add_lexer('meson-grammar', MesonBnfGrammarLexer)
     app.add_lexer('meson', MesonLexer)
     app.add_lexer('proofscape', ProofscapeLexer)
     app.add_lexer('pfsc', ProofscapeLexer)
 
-    app.connect('env-purge-doc', purge_chart_widgets)
-    app.connect('env-merge-info', merge_chart_widgets)
-    app.connect('html-page-context', write_widget_data)
-
     return {
         'version': __version__,
         'parallel_read_safe': True,
         'parallel_write_safe': True,
     }
```

### Comparing `sphinx-proofscape-0.3.2/sphinx_proofscape/chart_widget.py` & `sphinx-proofscape-0.4.0/sphinx_proofscape/chart_widget.py`

 * *Files identical despite different names*

### Comparing `sphinx-proofscape-0.3.2/sphinx_proofscape/lang_exts.py` & `sphinx-proofscape-0.4.0/sphinx_proofscape/lang_exts.py`

 * *Files identical despite different names*

### Comparing `sphinx-proofscape-0.3.2/sphinx_proofscape/lexer.py` & `sphinx-proofscape-0.4.0/sphinx_proofscape/lexer.py`

 * *Files identical despite different names*

### Comparing `sphinx-proofscape-0.3.2/sphinx_proofscape.egg-info/PKG-INFO` & `sphinx-proofscape-0.4.0/sphinx_proofscape.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: sphinx-proofscape
-Version: 0.3.2
+Version: 0.4.0
 Summary: Sphinx extension for Proofscape
 Home-page: https://github.com/proofscape/sphinx-proofscape/
 License: Apache 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 License-File: NOTICE
 
 sphinx-proofscape
 =================
 
-Sphinx extension for adding Proofscape widgets to your documents.
+Sphinx extension for use with Proofscape.
 
-Currently, only *chart widgets* are supported.
+In versions ``0.3.x``, this package provided both syntax highlighting (for the
+Proofscape module language and Meson language), and roles and directives for
+chart widgets.
 
-Support for all widget types is planned.
+In versions ``0.4.x``, only syntax highlighting is provided. Development of
+widget roles and directives has moved to the ``pise/server`` project.
```

