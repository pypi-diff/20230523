# Comparing `tmp/mathsym_adasneves-1.1.3.tar.gz` & `tmp/mathsym_adasneves-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathsym_adasneves-1.1.3.tar", last modified: Sat May 20 22:13:33 2023, max compression
+gzip compressed data, was "mathsym_adasneves-1.1.4.tar", last modified: Mon May 22 22:53:24 2023, max compression
```

## Comparing `mathsym_adasneves-1.1.3.tar` & `mathsym_adasneves-1.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-20 22:13:33.617088 mathsym_adasneves-1.1.3/
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1073 2023-05-13 19:33:38.000000 mathsym_adasneves-1.1.3/LICENSE
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1744 2023-05-20 22:13:33.617088 mathsym_adasneves-1.1.3/PKG-INFO
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1226 2023-05-19 00:28:33.000000 mathsym_adasneves-1.1.3/README.md
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      591 2023-05-20 22:13:15.000000 mathsym_adasneves-1.1.3/pyproject.toml
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)       38 2023-05-20 22:13:33.617088 mathsym_adasneves-1.1.3/setup.cfg
-drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-20 22:13:33.613089 mathsym_adasneves-1.1.3/src/
-drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-20 22:13:33.613089 mathsym_adasneves-1.1.3/src/mathsym_adasneves.egg-info/
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1744 2023-05-20 22:13:33.000000 mathsym_adasneves-1.1.3/src/mathsym_adasneves.egg-info/PKG-INFO
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      437 2023-05-20 22:13:33.000000 mathsym_adasneves-1.1.3/src/mathsym_adasneves.egg-info/SOURCES.txt
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)        1 2023-05-20 22:13:33.000000 mathsym_adasneves-1.1.3/src/mathsym_adasneves.egg-info/dependency_links.txt
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)       21 2023-05-20 22:13:33.000000 mathsym_adasneves-1.1.3/src/mathsym_adasneves.egg-info/top_level.txt
-drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-20 22:13:33.617088 mathsym_adasneves-1.1.3/src/symMath_adasneves127/
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)        0 2023-05-19 00:08:33.000000 mathsym_adasneves-1.1.3/src/symMath_adasneves127/__init__.py
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1073 2023-05-19 00:54:00.000000 mathsym_adasneves-1.1.3/src/symMath_adasneves127/equation.py
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      101 2023-05-19 00:13:51.000000 mathsym_adasneves-1.1.3/src/symMath_adasneves127/token.py
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     2084 2023-05-19 00:57:25.000000 mathsym_adasneves-1.1.3/src/symMath_adasneves127/token_maker.py
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     3438 2023-05-19 00:09:20.000000 mathsym_adasneves-1.1.3/src/symMath_adasneves127/tree_maker.py
--rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     2621 2023-05-20 22:13:21.000000 mathsym_adasneves-1.1.3/src/symMath_adasneves127/tree_node.py
+drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-22 22:53:24.626060 mathsym_adasneves-1.1.4/
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1073 2023-05-13 19:33:38.000000 mathsym_adasneves-1.1.4/LICENSE
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1744 2023-05-22 22:53:24.626060 mathsym_adasneves-1.1.4/PKG-INFO
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1226 2023-05-19 00:28:33.000000 mathsym_adasneves-1.1.4/README.md
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      591 2023-05-22 22:53:13.000000 mathsym_adasneves-1.1.4/pyproject.toml
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)       38 2023-05-22 22:53:24.626060 mathsym_adasneves-1.1.4/setup.cfg
+drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-22 22:53:24.622060 mathsym_adasneves-1.1.4/src/
+drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-22 22:53:24.626060 mathsym_adasneves-1.1.4/src/mathsym_adasneves.egg-info/
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1744 2023-05-22 22:53:24.000000 mathsym_adasneves-1.1.4/src/mathsym_adasneves.egg-info/PKG-INFO
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      437 2023-05-22 22:53:24.000000 mathsym_adasneves-1.1.4/src/mathsym_adasneves.egg-info/SOURCES.txt
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)        1 2023-05-22 22:53:24.000000 mathsym_adasneves-1.1.4/src/mathsym_adasneves.egg-info/dependency_links.txt
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)       21 2023-05-22 22:53:24.000000 mathsym_adasneves-1.1.4/src/mathsym_adasneves.egg-info/top_level.txt
+drwxrwxr-x   0 adasneves  (1000) adasneves  (1000)        0 2023-05-22 22:53:24.626060 mathsym_adasneves-1.1.4/src/symMath_adasneves127/
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)        0 2023-05-19 00:08:33.000000 mathsym_adasneves-1.1.4/src/symMath_adasneves127/__init__.py
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     1073 2023-05-19 00:54:00.000000 mathsym_adasneves-1.1.4/src/symMath_adasneves127/equation.py
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)      101 2023-05-19 00:13:51.000000 mathsym_adasneves-1.1.4/src/symMath_adasneves127/token.py
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     2222 2023-05-20 23:49:20.000000 mathsym_adasneves-1.1.4/src/symMath_adasneves127/token_maker.py
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     3438 2023-05-19 00:09:20.000000 mathsym_adasneves-1.1.4/src/symMath_adasneves127/tree_maker.py
+-rw-rw-r--   0 adasneves  (1000) adasneves  (1000)     3642 2023-05-22 22:47:50.000000 mathsym_adasneves-1.1.4/src/symMath_adasneves127/tree_node.py
```

### Comparing `mathsym_adasneves-1.1.3/LICENSE` & `mathsym_adasneves-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mathsym_adasneves-1.1.3/PKG-INFO` & `mathsym_adasneves-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathsym_adasneves
-Version: 1.1.3
+Version: 1.1.4
 Summary: A small example package
 Author-email: Alex Dasneves <adasneves@adasneves.info>
 Project-URL: Homepage, https://github.com/adasneves127/Symmath
 Project-URL: Bug Tracker, https://github.com/adasneves127/Symmath/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mathsym_adasneves-1.1.3/README.md` & `mathsym_adasneves-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `mathsym_adasneves-1.1.3/pyproject.toml` & `mathsym_adasneves-1.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mathsym_adasneves"
-version = "1.1.3"
+version = "1.1.4"
 authors = [
   { name="Alex Dasneves", email="adasneves@adasneves.info" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `mathsym_adasneves-1.1.3/src/mathsym_adasneves.egg-info/PKG-INFO` & `mathsym_adasneves-1.1.4/src/mathsym_adasneves.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathsym-adasneves
-Version: 1.1.3
+Version: 1.1.4
 Summary: A small example package
 Author-email: Alex Dasneves <adasneves@adasneves.info>
 Project-URL: Homepage, https://github.com/adasneves127/Symmath
 Project-URL: Bug Tracker, https://github.com/adasneves127/Symmath/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mathsym_adasneves-1.1.3/src/symMath_adasneves127/equation.py` & `mathsym_adasneves-1.1.4/src/symMath_adasneves127/equation.py`

 * *Files identical despite different names*

### Comparing `mathsym_adasneves-1.1.3/src/symMath_adasneves127/token_maker.py` & `mathsym_adasneves-1.1.4/src/symMath_adasneves127/token_maker.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,18 +23,21 @@
             case "^":
                 token_list.append(token("EXPONENT", "^"))
             case "x":
                 token_list.append(token("VARIABLE", "x"))
         
         if equation_code.startswith("sin"):
             token_list.append(token("TRIG.SIN", "sin"))
+            equation_code = equation_code[2:]
         elif equation_code.startswith("cos"):
             token_list.append(token("TRIG.COS", "cos"))
+            equation_code = equation_code[2:]
         elif equation_code.startswith("tan"):
             token_list.append(token("TRIG.TAN", "tan"))
+            equation_code = equation_code[2:]
         
         if char.isdigit() or char == ".":
             numbStr = "" if char != "." else "0"
             while char.isdigit() or char == ".":
                 numbStr += char
                 if len(equation_code) > 1 and (equation_code[1].isdigit() or \
                                                equation_code[1] == "."):
```

### Comparing `mathsym_adasneves-1.1.3/src/symMath_adasneves127/tree_maker.py` & `mathsym_adasneves-1.1.4/src/symMath_adasneves127/tree_maker.py`

 * *Files identical despite different names*

