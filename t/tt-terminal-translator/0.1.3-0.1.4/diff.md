# Comparing `tmp/tt_terminal_translator-0.1.3.tar.gz` & `tmp/tt_terminal_translator-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tt_terminal_translator-0.1.3.tar", max compression
+gzip compressed data, was "tt_terminal_translator-0.1.4.tar", max compression
```

## Comparing `tt_terminal_translator-0.1.3.tar` & `tt_terminal_translator-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1073 2023-05-06 02:57:49.810774 tt_terminal_translator-0.1.3/LICENSE
--rw-r--r--   0        0        0     1895 2023-05-06 02:57:49.810774 tt_terminal_translator-0.1.3/README.md
--rw-r--r--   0        0        0     1725 2023-05-06 03:29:50.160326 tt_terminal_translator-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2439 2023-05-06 03:14:32.129998 tt_terminal_translator-0.1.3/src/terminal_translator/config.py
--rw-r--r--   0        0        0     2517 2023-05-06 03:14:41.539958 tt_terminal_translator-0.1.3/src/terminal_translator/main.py
--rw-r--r--   0        0        0      359 2023-05-06 03:29:43.733677 tt_terminal_translator-0.1.3/src/terminal_translator/version.py
--rw-r--r--   0        0        0     2870 1970-01-01 00:00:00.000000 tt_terminal_translator-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-06 02:57:49.810774 tt_terminal_translator-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1895 2023-05-06 02:57:49.810774 tt_terminal_translator-0.1.4/README.md
+-rw-r--r--   0        0        0     1777 2023-05-22 23:04:34.025626 tt_terminal_translator-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2439 2023-05-06 03:14:32.129998 tt_terminal_translator-0.1.4/src/terminal_translator/config.py
+-rw-r--r--   0        0        0     2517 2023-05-06 03:14:41.539958 tt_terminal_translator-0.1.4/src/terminal_translator/main.py
+-rw-r--r--   0        0        0      359 2023-05-06 03:29:43.733677 tt_terminal_translator-0.1.4/src/terminal_translator/version.py
+-rw-r--r--   0        0        0     2965 1970-01-01 00:00:00.000000 tt_terminal_translator-0.1.4/PKG-INFO
```

### Comparing `tt_terminal_translator-0.1.3/LICENSE` & `tt_terminal_translator-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tt_terminal_translator-0.1.3/README.md` & `tt_terminal_translator-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `tt_terminal_translator-0.1.3/pyproject.toml` & `tt_terminal_translator-0.1.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tt-terminal-translator"
-version = "0.1.3"
+version = "0.1.4"
 description = "Terminal Translator is a translation CLI that uses the Google Cloud API. "
 authors = ["gbPagano <guilhermebpagano@gmail.com>"]
 readme = "README.md"
 packages = [{include = "terminal_translator", from = "src"}]
 classifiers = [  
     "Environment :: Console",
     "Development Status :: 5 - Production/Stable",
@@ -24,14 +24,16 @@
 python = "^3.10"
 google-cloud-translate = "^3.11.0"
 dynaconf = "^3.1.12"
 toml = "^0.10.2"
 typer = "^0.7.0"
 rich = "^13.3.2"
 pyperclip = "^1.8.2"
+requests = "^2.31.0"
+pymdown-extensions = "^10.0.1"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 isort = "^5.12.0"
 ruff = "^0.0.259"
 pip-audit = "^2.5.3"
```

### Comparing `tt_terminal_translator-0.1.3/src/terminal_translator/config.py` & `tt_terminal_translator-0.1.4/src/terminal_translator/config.py`

 * *Files identical despite different names*

### Comparing `tt_terminal_translator-0.1.3/src/terminal_translator/main.py` & `tt_terminal_translator-0.1.4/src/terminal_translator/main.py`

 * *Files identical despite different names*

### Comparing `tt_terminal_translator-0.1.3/PKG-INFO` & `tt_terminal_translator-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: tt-terminal-translator
-Version: 0.1.3
+Version: 0.1.4
 Summary: Terminal Translator is a translation CLI that uses the Google Cloud API. 
 Author: gbPagano
 Author-email: guilhermebpagano@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
 Requires-Dist: google-cloud-translate (>=3.11.0,<4.0.0)
+Requires-Dist: pymdown-extensions (>=10.0.1,<11.0.0)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.3.2,<14.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Project-URL: Code, https://github.com/gbPagano/terminal-translator
 Project-URL: Documentation, https://terminal-translator.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
```

