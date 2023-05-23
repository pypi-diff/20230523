# Comparing `tmp/php2py-0.1.0.tar.gz` & `tmp/php2py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "php2py-0.1.0.tar", max compression
+gzip compressed data, was "php2py-0.1.1.tar", max compression
```

## Comparing `php2py-0.1.0.tar` & `php2py-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,20 @@
--rw-r--r--   0        0        0     1559 2023-05-23 06:09:52.949881 php2py-0.1.0/LICENSE
--rw-r--r--   0        0        0      987 2023-05-23 06:30:04.713529 php2py-0.1.0/README.md
--rw-r--r--   0        0        0     1195 2023-05-23 06:21:55.567751 php2py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-23 05:59:23.011645 php2py-0.1.0/src/php2py/__init__.py
--rw-r--r--   0        0        0     1818 2023-05-23 05:59:23.012047 php2py-0.1.0/src/php2py/parser.py
--rw-r--r--   0        0        0    14892 2023-05-23 05:59:23.012256 php2py-0.1.0/src/php2py/php_ast.py
--rw-r--r--   0        0        0    34971 2023-05-23 05:59:23.012650 php2py-0.1.0/src/php2py/translator.py
--rw-r--r--   0        0        0        0 2023-05-23 06:16:13.275175 php2py-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0       40 2023-05-23 05:59:23.013030 php2py-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0      930 2023-05-23 06:19:38.727957 php2py-0.1.0/tests/test_assignments.py
--rw-r--r--   0        0        0      968 2023-05-23 06:19:42.680915 php2py-0.1.0/tests/test_classes.py
--rw-r--r--   0        0        0     1986 2023-05-23 06:19:48.284916 php2py-0.1.0/tests/test_control_flow.py
--rw-r--r--   0        0        0     1412 2023-05-23 06:19:52.269569 php2py-0.1.0/tests/test_functions.py
--rw-r--r--   0        0        0     3095 2023-05-23 06:20:21.204035 php2py-0.1.0/tests/test_translator.py
--rw-r--r--   0        0        0      246 2023-05-23 06:20:10.095118 php2py-0.1.0/tests/test_whole_programs.py
--rw-r--r--   0        0        0     2226 2023-05-23 05:59:23.014795 php2py-0.1.0/tests/util.py
--rw-r--r--   0        0        0     1860 1970-01-01 00:00:00.000000 php2py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1559 2023-05-23 06:32:18.069556 php2py-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1898 2023-05-23 07:14:27.931239 php2py-0.1.1/README.md
+-rw-r--r--   0        0        0     1256 2023-05-23 07:14:50.964995 php2py-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-03-05 11:27:00.834601 php2py-0.1.1/src/php2py/__init__.py
+-rw-r--r--   0        0        0      216 2022-03-04 18:54:00.719295 php2py-0.1.1/src/php2py/etc/composer.json
+-rw-r--r--   0        0        0     2448 2023-05-23 06:32:18.070273 php2py-0.1.1/src/php2py/etc/composer.lock
+-rw-r--r--   0        0        0     1064 2023-05-23 07:09:01.029475 php2py-0.1.1/src/php2py/main.py
+-rw-r--r--   0        0        0     1990 2023-05-23 06:56:16.686004 php2py-0.1.1/src/php2py/parser.py
+-rw-r--r--   0        0        0    14892 2022-03-08 17:39:04.665953 php2py-0.1.1/src/php2py/php_ast.py
+-rw-r--r--   0        0        0    34971 2022-03-08 17:43:12.031753 php2py-0.1.1/src/php2py/translator.py
+-rw-r--r--   0        0        0        0 2023-05-23 06:32:18.074916 php2py-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0       40 2022-03-08 09:11:16.167491 php2py-0.1.1/tests/conftest.py
+-rw-r--r--   0        0        0      930 2023-05-23 06:32:18.076808 php2py-0.1.1/tests/test_assignments.py
+-rw-r--r--   0        0        0      968 2023-05-23 06:32:18.078753 php2py-0.1.1/tests/test_classes.py
+-rw-r--r--   0        0        0     2011 2023-05-23 06:35:52.574763 php2py-0.1.1/tests/test_control_flow.py
+-rw-r--r--   0        0        0     1412 2023-05-23 06:32:18.080739 php2py-0.1.1/tests/test_functions.py
+-rw-r--r--   0        0        0     3095 2023-05-23 06:32:18.081938 php2py-0.1.1/tests/test_translator.py
+-rw-r--r--   0        0        0      246 2023-05-23 06:32:18.082305 php2py-0.1.1/tests/test_whole_programs.py
+-rw-r--r--   0        0        0     2209 2023-05-23 07:01:27.241961 php2py-0.1.1/tests/util.py
+-rw-r--r--   0        0        0     2759 1970-01-01 00:00:00.000000 php2py-0.1.1/PKG-INFO
```

### Comparing `php2py-0.1.0/LICENSE` & `php2py-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `php2py-0.1.0/pyproject.toml` & `php2py-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,58 @@
-[tool]
 [tool.poetry]
 name = "php2py"
-version = "0.1.0"
+version = "0.1.1"
 homepage = "https://github.com/sfermigier/php2py"
 description = "PHP to Python transpiler."
 authors = ["Abilian SAS <sf@abilian.com>"]
 readme = "README.md"
-classifiers=[
+classifiers = [
     'Development Status :: 2 - Pre-Alpha',
     'Intended Audience :: Developers',
     'Natural Language :: English',
     'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.8',
-    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
 ]
 packages = [
     { include = "php2py", from = "src" },
     { include = "tests", format = "sdist" },
 ]
 
-
 [tool.poetry.dependencies]
 python = ">=3.9,<4"
 astor = "^0.8.1"
 attrs = "^23.1.0"
 
 # For debugging. Remove later.
 icecream = "^2.1.2"
 rich = "^11.2.0"
 devtools = "^0.8.0"
 astpretty = "^2.1.0"
-
+click = "^8.1.3"
 
 [tool.poetry.dev-dependencies]
 abilian-devtools = "*"
 
 restructuredtext_lint = "*"
 
+[tool.poetry.scripts]
+php2py = "php2py.main:main"
+
 
 [tool.ruff]
 extend-ignore = [
     "S101", # Use of 'assert'
     "E501", # Line too long
     # TODO: fix these
     "F841", # Local variable `key` is assigned to but never used
 ]
 extend-exclude = [
     ".nox"
 ]
 
-
 [tool.isort]
 profile = "black"
 
-
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `php2py-0.1.0/src/php2py/parser.py` & `php2py-0.1.1/src/php2py/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 import json
 import shlex
 import subprocess
 import tempfile
+from pathlib import Path
 
 from . import php_ast
 
 
-def parse(source_code: str):
+def parse(source_code: str, php_parse: str | Path = ""):
+    if not php_parse:
+        php_parse = "vendor/nikic/php-parser/bin/php-parse"
+    php_parse = Path(php_parse)
+    assert php_parse.exists()
+
     with tempfile.NamedTemporaryFile("w", suffix=".php", delete=False) as source_file:
         source_file.write(source_code)
         source_file.flush()
 
-        cmd_line = f"vendor/nikic/php-parser/bin/php-parse -j {source_file.name}"
+        cmd_line = f"{php_parse} -j {source_file.name}"
         args = shlex.split(cmd_line)
         with subprocess.Popen(
             args, stdout=subprocess.PIPE, stderr=subprocess.DEVNULL
         ) as p:
             json_ast = json.load(p.stdout)
             result = make_ast(json_ast)
```

### Comparing `php2py-0.1.0/src/php2py/php_ast.py` & `php2py-0.1.1/src/php2py/php_ast.py`

 * *Files identical despite different names*

### Comparing `php2py-0.1.0/src/php2py/translator.py` & `php2py-0.1.1/src/php2py/translator.py`

 * *Files identical despite different names*

### Comparing `php2py-0.1.0/tests/test_assignments.py` & `php2py-0.1.1/tests/test_assignments.py`

 * *Files identical despite different names*

### Comparing `php2py-0.1.0/tests/test_classes.py` & `php2py-0.1.1/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `php2py-0.1.0/tests/test_control_flow.py` & `php2py-0.1.1/tests/test_control_flow.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from unittest import skip
+
 from .util import check_compiles
 
 
 def test_while():
     input = r"""<?php
         while (true) {
             echo $bar;
@@ -84,15 +86,16 @@
         # endforeach;
         # foreach ($foo as $bar[0]) {}
     ?>"""
     expected = "for bar in foo:\n" "    echo(bar)\n" "pass"
     check_compiles(input, expected)
 
 
-# def test_for():
-#     input = r"""<?php
-#         for ($i = 0; $i < 10; $i++) {
-#             echo $i;
-#         }
-#     ?>"""
-#     expected = ""
-#     check_compiles(input, expected)
+@skip("TODO")
+def test_for():
+    input = r"""<?php
+        for ($i = 0; $i < 10; $i++) {
+            echo $i;
+        }
+    ?>"""
+    expected = ""
+    check_compiles(input, expected)
```

### Comparing `php2py-0.1.0/tests/test_functions.py` & `php2py-0.1.1/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `php2py-0.1.0/tests/test_translator.py` & `php2py-0.1.1/tests/test_translator.py`

 * *Files identical despite different names*

### Comparing `php2py-0.1.0/tests/util.py` & `php2py-0.1.1/tests/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import ast
 import shlex
 import subprocess
 import tempfile
 from ast import unparse
 
-import astpretty
 import rich
 from devtools import debug
 
 from php2py.parser import parse
 from php2py.translator import Translator
```

