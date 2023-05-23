# Comparing `tmp/sphinx-proofscape-0.3.1.tar.gz` & `tmp/sphinx-proofscape-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-proofscape-0.3.1.tar", last modified: Wed Sep 21 20:55:27 2022, max compression
+gzip compressed data, was "sphinx-proofscape-0.3.2.tar", last modified: Tue May 23 14:55:20 2023, max compression
```

## Comparing `sphinx-proofscape-0.3.1.tar` & `sphinx-proofscape-0.3.2.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2022-09-21 20:55:27.419887 sphinx-proofscape-0.3.1/
--rw-r--r--   0 skieffer   (501) staff       (20)    11359 2022-08-23 20:24:57.000000 sphinx-proofscape-0.3.1/LICENSE
--rw-r--r--   0 skieffer   (501) staff       (20)       61 2022-08-23 21:25:18.000000 sphinx-proofscape-0.3.1/NOTICE
--rw-r--r--   0 skieffer   (501) staff       (20)      632 2022-09-21 20:55:27.419375 sphinx-proofscape-0.3.1/PKG-INFO
--rw-r--r--   0 skieffer   (501) staff       (20)      193 2022-08-23 21:45:08.000000 sphinx-proofscape-0.3.1/README.rst
--rw-r--r--   0 skieffer   (501) staff       (20)       38 2022-09-21 20:55:27.420043 sphinx-proofscape-0.3.1/setup.cfg
--rw-r--r--   0 skieffer   (501) staff       (20)      760 2022-08-27 17:30:01.000000 sphinx-proofscape-0.3.1/setup.py
-drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2022-09-21 20:55:27.415540 sphinx-proofscape-0.3.1/sphinx_proofscape/
--rw-r--r--   0 skieffer   (501) staff       (20)     4154 2022-09-21 20:55:10.000000 sphinx-proofscape-0.3.1/sphinx_proofscape/__init__.py
--rw-r--r--   0 skieffer   (501) staff       (20)    11594 2022-08-23 21:30:08.000000 sphinx-proofscape-0.3.1/sphinx_proofscape/chart_widget.py
--rw-r--r--   0 skieffer   (501) staff       (20)    12030 2022-08-29 17:38:00.000000 sphinx-proofscape-0.3.1/sphinx_proofscape/lang_exts.py
--rw-r--r--   0 skieffer   (501) staff       (20)     7284 2022-09-21 20:24:19.000000 sphinx-proofscape-0.3.1/sphinx_proofscape/lexer.py
-drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2022-09-21 20:55:27.417965 sphinx-proofscape-0.3.1/sphinx_proofscape.egg-info/
--rw-r--r--   0 skieffer   (501) staff       (20)      632 2022-09-21 20:55:27.000000 sphinx-proofscape-0.3.1/sphinx_proofscape.egg-info/PKG-INFO
--rw-r--r--   0 skieffer   (501) staff       (20)      360 2022-09-21 20:55:27.000000 sphinx-proofscape-0.3.1/sphinx_proofscape.egg-info/SOURCES.txt
--rw-r--r--   0 skieffer   (501) staff       (20)        1 2022-09-21 20:55:27.000000 sphinx-proofscape-0.3.1/sphinx_proofscape.egg-info/dependency_links.txt
--rw-r--r--   0 skieffer   (501) staff       (20)       16 2022-09-21 20:55:27.000000 sphinx-proofscape-0.3.1/sphinx_proofscape.egg-info/requires.txt
--rw-r--r--   0 skieffer   (501) staff       (20)       18 2022-09-21 20:55:27.000000 sphinx-proofscape-0.3.1/sphinx_proofscape.egg-info/top_level.txt
+drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2023-05-23 14:55:20.544999 sphinx-proofscape-0.3.2/
+-rw-r--r--   0 skieffer   (501) staff       (20)    11359 2022-08-23 20:24:57.000000 sphinx-proofscape-0.3.2/LICENSE
+-rw-r--r--   0 skieffer   (501) staff       (20)       66 2023-01-01 18:47:48.000000 sphinx-proofscape-0.3.2/NOTICE
+-rw-r--r--   0 skieffer   (501) staff       (20)      610 2023-05-23 14:55:20.545135 sphinx-proofscape-0.3.2/PKG-INFO
+-rw-r--r--   0 skieffer   (501) staff       (20)      193 2022-08-23 21:45:08.000000 sphinx-proofscape-0.3.2/README.rst
+-rw-r--r--   0 skieffer   (501) staff       (20)       81 2023-01-19 20:31:13.000000 sphinx-proofscape-0.3.2/pyproject.toml
+-rw-r--r--   0 skieffer   (501) staff       (20)      671 2023-05-23 14:55:20.546101 sphinx-proofscape-0.3.2/setup.cfg
+drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2023-05-23 14:55:20.541116 sphinx-proofscape-0.3.2/sphinx_proofscape/
+-rw-r--r--   0 skieffer   (501) staff       (20)     4154 2023-05-23 14:39:25.000000 sphinx-proofscape-0.3.2/sphinx_proofscape/__init__.py
+-rw-r--r--   0 skieffer   (501) staff       (20)    11594 2023-01-01 18:47:48.000000 sphinx-proofscape-0.3.2/sphinx_proofscape/chart_widget.py
+-rw-r--r--   0 skieffer   (501) staff       (20)    12128 2023-01-01 18:47:48.000000 sphinx-proofscape-0.3.2/sphinx_proofscape/lang_exts.py
+-rw-r--r--   0 skieffer   (501) staff       (20)     7284 2023-01-01 18:47:48.000000 sphinx-proofscape-0.3.2/sphinx_proofscape/lexer.py
+drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2023-05-23 14:55:20.543937 sphinx-proofscape-0.3.2/sphinx_proofscape.egg-info/
+-rw-r--r--   0 skieffer   (501) staff       (20)      610 2023-05-23 14:55:20.000000 sphinx-proofscape-0.3.2/sphinx_proofscape.egg-info/PKG-INFO
+-rw-r--r--   0 skieffer   (501) staff       (20)      400 2023-05-23 14:55:20.000000 sphinx-proofscape-0.3.2/sphinx_proofscape.egg-info/SOURCES.txt
+-rw-r--r--   0 skieffer   (501) staff       (20)        1 2023-05-23 14:55:20.000000 sphinx-proofscape-0.3.2/sphinx_proofscape.egg-info/dependency_links.txt
+-rw-r--r--   0 skieffer   (501) staff       (20)       70 2023-05-23 14:55:20.000000 sphinx-proofscape-0.3.2/sphinx_proofscape.egg-info/requires.txt
+-rw-r--r--   0 skieffer   (501) staff       (20)       18 2023-05-23 14:55:20.000000 sphinx-proofscape-0.3.2/sphinx_proofscape.egg-info/top_level.txt
+drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2023-05-23 14:55:20.544354 sphinx-proofscape-0.3.2/tests/
+-rw-r--r--   0 skieffer   (501) staff       (20)    10198 2023-05-23 14:30:49.000000 sphinx-proofscape-0.3.2/tests/test_extension.py
```

### Comparing `sphinx-proofscape-0.3.1/LICENSE` & `sphinx-proofscape-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-proofscape-0.3.1/PKG-INFO` & `sphinx-proofscape-0.3.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: sphinx-proofscape
-Version: 0.3.1
+Version: 0.3.2
 Summary: Sphinx extension for Proofscape
 Home-page: https://github.com/proofscape/sphinx-proofscape/
-Author: Proofscape contributors
 License: Apache 2.0
-Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
 License-File: LICENSE
 License-File: NOTICE
 
 sphinx-proofscape
 =================
 
 Sphinx extension for adding Proofscape widgets to your documents.
```

### Comparing `sphinx-proofscape-0.3.1/sphinx_proofscape/__init__.py` & `sphinx-proofscape-0.3.2/sphinx_proofscape/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   Sphinx-Proofscape                                                         #
 #                                                                             #
-#   Copyright (c) 2022 Proofscape contributors                                #
+#   Copyright (c) 2022-2023 Proofscape contributors                           #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
@@ -26,15 +26,15 @@
     PfscDefnsDirective,
 )
 from sphinx_proofscape.lexer import (
     MesonLexer, ProofscapeLexer, MesonBnfGrammarLexer,
 )
 
 
-__version__ = '0.3.1'
+__version__ = '0.3.2'
 
 
 ###############################################################################
 # Standard purge & merge
 # See e.g. https://www.sphinx-doc.org/en/master/development/tutorials/todo.html
```

### Comparing `sphinx-proofscape-0.3.1/sphinx_proofscape/chart_widget.py` & `sphinx-proofscape-0.3.2/sphinx_proofscape/chart_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   Sphinx-Proofscape                                                         #
 #                                                                             #
-#   Copyright (c) 2022 Proofscape contributors                                #
+#   Copyright (c) 2022-2023 Proofscape contributors                           #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
```

### Comparing `sphinx-proofscape-0.3.1/sphinx_proofscape/lang_exts.py` & `sphinx-proofscape-0.3.2/sphinx_proofscape/lang_exts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   Sphinx-Proofscape                                                         #
 #                                                                             #
-#   Copyright (c) 2022 Proofscape contributors                                #
+#   Copyright (c) 2022-2023 Proofscape contributors                           #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
@@ -143,14 +143,16 @@
     """
 
     def finish_run(self, rawtext, label, widget_fields):
         repopath = self.config.pfsc_repopath
         repovers = self.config.pfsc_repovers
 
         vers_defns = self.config.pfsc_import_repos or {}
+        # FIXME:
+        #  Couldn't this be done just once? Maybe on an early sphinx build hook?
         vers_defns = regularize_version_dict(vers_defns)
 
         docname = self.env.docname
         wnum = self.env.new_serialno('widget')
 
         lp_defns = getattr(self.env, 'pfsc_lp_defns_by_docname', {})
 
@@ -234,15 +236,15 @@
     ===============
 
     * Each of the `on_board`, `off_board`, `view`, and `select` fields
       can receive only a boxlisting. This means:
         - None of these fields can yet receive any keywords (e.g. "all" for `off_board`).
         - The `view` option cannot yet receive its more advanced format, where
           a whole dictionary is passed.
-    * The `color` and `hovorcolor` fields are fully supported.
+    * The `color` and `hovercolor` fields are fully supported.
 
     Syntax
     ======
 
     Generally, the goal is to take advantage of the possibilities of rST, to make
     a nicer, easier syntax than is available in annotations. In the latter, we
     are constrained by JSON format; here we are not.
```

### Comparing `sphinx-proofscape-0.3.1/sphinx_proofscape/lexer.py` & `sphinx-proofscape-0.3.2/sphinx_proofscape/lexer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   Sphinx-Proofscape                                                         #
 #                                                                             #
-#   Copyright (c) 2022 Proofscape contributors                                #
+#   Copyright (c) 2022-2023 Proofscape contributors                           #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
```

### Comparing `sphinx-proofscape-0.3.1/sphinx_proofscape.egg-info/PKG-INFO` & `sphinx-proofscape-0.3.2/sphinx_proofscape.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: sphinx-proofscape
-Version: 0.3.1
+Version: 0.3.2
 Summary: Sphinx extension for Proofscape
 Home-page: https://github.com/proofscape/sphinx-proofscape/
-Author: Proofscape contributors
 License: Apache 2.0
-Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
 License-File: LICENSE
 License-File: NOTICE
 
 sphinx-proofscape
 =================
 
 Sphinx extension for adding Proofscape widgets to your documents.
```

