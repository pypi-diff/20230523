# Comparing `tmp/pyextrasafe-0.0.0a0.tar.gz` & `tmp/pyextrasafe-0.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyextrasafe-0.0.0a0.tar", last modified: Tue May 23 00:24:22 2023, max compression
+gzip compressed data, was "pyextrasafe-0.0.0a1.tar", last modified: Tue May 23 19:39:09 2023, max compression
```

## Comparing `pyextrasafe-0.0.0a0.tar` & `pyextrasafe-0.0.0a1.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2023-05-23 00:24:22.098880 pyextrasafe-0.0.0a0/
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)      306 2023-05-22 20:44:19.000000 pyextrasafe-0.0.0a0/CHANGELOG.md
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1063 2023-05-22 19:03:28.000000 pyextrasafe-0.0.0a0/Cargo.toml
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)    10494 2023-05-22 09:25:15.000000 pyextrasafe-0.0.0a0/LICENSE.md
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)      145 2023-05-22 20:44:44.000000 pyextrasafe-0.0.0a0/MANIFEST.in
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1290 2023-05-22 19:21:25.000000 pyextrasafe-0.0.0a0/Makefile
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     3233 2023-05-23 00:24:22.098880 pyextrasafe-0.0.0a0/PKG-INFO
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1929 2023-05-22 23:52:37.000000 pyextrasafe-0.0.0a0/README.md
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)      668 2023-05-22 08:46:08.000000 pyextrasafe-0.0.0a0/build.rs
-drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2023-05-23 00:24:22.098880 pyextrasafe-0.0.0a0/docs/
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)      947 2023-05-22 23:43:14.000000 pyextrasafe-0.0.0a0/docs/conf.py
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)       28 2023-05-22 23:57:55.000000 pyextrasafe-0.0.0a0/docs/index.rst
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)      204 2023-05-22 22:45:05.000000 pyextrasafe-0.0.0a0/pyproject.toml
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)      228 2023-05-22 23:44:25.000000 pyextrasafe-0.0.0a0/requirements-dev.txt
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)      164 2023-05-22 23:44:30.000000 pyextrasafe-0.0.0a0/requirements-readthedocs.txt
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)      385 2023-05-22 10:16:45.000000 pyextrasafe-0.0.0a0/rustfmt.toml
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1368 2023-05-23 00:24:22.098880 pyextrasafe-0.0.0a0/setup.cfg
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)      479 2023-05-22 20:46:15.000000 pyextrasafe-0.0.0a0/setup.py
-drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2023-05-23 00:24:22.098880 pyextrasafe-0.0.0a0/src/
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     2775 2023-05-22 18:22:30.000000 pyextrasafe-0.0.0a0/src/lib.rs
-drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2023-05-23 00:24:22.098880 pyextrasafe-0.0.0a0/src/pyextrasafe/
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     3853 2023-05-22 23:58:05.000000 pyextrasafe-0.0.0a0/src/pyextrasafe/__init__.py
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)      296 2023-05-22 19:07:07.000000 pyextrasafe-0.0.0a0/src/pyextrasafe/__init__.pyi
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     3684 2023-05-22 23:13:25.000000 pyextrasafe-0.0.0a0/src/pyextrasafe/_pyextrasafe.pyi
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)        0 2023-05-22 09:17:19.000000 pyextrasafe-0.0.0a0/src/pyextrasafe/py.typed
-drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2023-05-23 00:24:22.098880 pyextrasafe-0.0.0a0/src/pyextrasafe.egg-info/
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     3233 2023-05-23 00:24:22.000000 pyextrasafe-0.0.0a0/src/pyextrasafe.egg-info/PKG-INFO
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)      554 2023-05-23 00:24:22.000000 pyextrasafe-0.0.0a0/src/pyextrasafe.egg-info/SOURCES.txt
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)        1 2023-05-23 00:24:22.000000 pyextrasafe-0.0.0a0/src/pyextrasafe.egg-info/dependency_links.txt
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)        1 2023-05-22 23:43:44.000000 pyextrasafe-0.0.0a0/src/pyextrasafe.egg-info/not-zip-safe
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)       12 2023-05-23 00:24:22.000000 pyextrasafe-0.0.0a0/src/pyextrasafe.egg-info/top_level.txt
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)    10266 2023-05-22 18:01:01.000000 pyextrasafe-0.0.0a0/src/rule_sets.rs
--rw-r--r--   0 kijewski  (1000) kijewski  (1000)     2979 2023-05-22 18:02:03.000000 pyextrasafe-0.0.0a0/src/safety_ctx.rs
+drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2023-05-23 19:39:09.032528 pyextrasafe-0.0.0a1/
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)      306 2023-05-22 20:44:19.000000 pyextrasafe-0.0.0a1/CHANGELOG.md
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1082 2023-05-23 19:29:49.000000 pyextrasafe-0.0.0a1/Cargo.toml
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)    10494 2023-05-22 09:25:15.000000 pyextrasafe-0.0.0a1/LICENSE.md
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)      145 2023-05-22 20:44:44.000000 pyextrasafe-0.0.0a1/MANIFEST.in
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1398 2023-05-23 16:08:52.000000 pyextrasafe-0.0.0a1/Makefile
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     3286 2023-05-23 19:39:09.032528 pyextrasafe-0.0.0a1/PKG-INFO
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1982 2023-05-23 19:27:31.000000 pyextrasafe-0.0.0a1/README.md
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)      668 2023-05-22 08:46:08.000000 pyextrasafe-0.0.0a1/build.rs
+drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2023-05-23 19:39:09.030528 pyextrasafe-0.0.0a1/docs/
+drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2023-05-23 19:39:09.030528 pyextrasafe-0.0.0a1/docs/_static/
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)      280 2023-05-23 19:11:41.000000 pyextrasafe-0.0.0a1/docs/_static/custom.css
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1010 2023-05-23 19:09:14.000000 pyextrasafe-0.0.0a1/docs/conf.py
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)       42 2023-05-23 19:07:25.000000 pyextrasafe-0.0.0a1/docs/index.rst
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)      204 2023-05-22 22:45:05.000000 pyextrasafe-0.0.0a1/pyproject.toml
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)      228 2023-05-22 23:44:25.000000 pyextrasafe-0.0.0a1/requirements-dev.txt
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)      164 2023-05-23 19:29:53.000000 pyextrasafe-0.0.0a1/requirements-readthedocs.txt
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)      385 2023-05-22 10:16:45.000000 pyextrasafe-0.0.0a1/rustfmt.toml
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     1368 2023-05-23 19:39:09.032528 pyextrasafe-0.0.0a1/setup.cfg
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)      479 2023-05-22 20:46:15.000000 pyextrasafe-0.0.0a1/setup.py
+drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2023-05-23 19:39:09.030528 pyextrasafe-0.0.0a1/src/
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     2775 2023-05-23 16:04:22.000000 pyextrasafe-0.0.0a1/src/lib.rs
+drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2023-05-23 19:39:09.030528 pyextrasafe-0.0.0a1/src/pyextrasafe/
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     4020 2023-05-23 19:27:10.000000 pyextrasafe-0.0.0a1/src/pyextrasafe/__init__.py
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)      296 2023-05-22 19:07:07.000000 pyextrasafe-0.0.0a1/src/pyextrasafe/__init__.pyi
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     5850 2023-05-23 18:29:04.000000 pyextrasafe-0.0.0a1/src/pyextrasafe/_pyextrasafe.pyi
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)        0 2023-05-22 09:17:19.000000 pyextrasafe-0.0.0a1/src/pyextrasafe/py.typed
+drwxr-xr-x   0 kijewski  (1000) kijewski  (1000)        0 2023-05-23 19:39:09.032528 pyextrasafe-0.0.0a1/src/pyextrasafe.egg-info/
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     3286 2023-05-23 19:39:09.000000 pyextrasafe-0.0.0a1/src/pyextrasafe.egg-info/PKG-INFO
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)      578 2023-05-23 19:39:09.000000 pyextrasafe-0.0.0a1/src/pyextrasafe.egg-info/SOURCES.txt
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)        1 2023-05-23 19:39:09.000000 pyextrasafe-0.0.0a1/src/pyextrasafe.egg-info/dependency_links.txt
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)        1 2023-05-22 23:43:44.000000 pyextrasafe-0.0.0a1/src/pyextrasafe.egg-info/not-zip-safe
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)       12 2023-05-23 19:39:09.000000 pyextrasafe-0.0.0a1/src/pyextrasafe.egg-info/top_level.txt
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)    17180 2023-05-23 18:29:01.000000 pyextrasafe-0.0.0a1/src/rule_sets.rs
+-rw-r--r--   0 kijewski  (1000) kijewski  (1000)     4247 2023-05-23 17:02:52.000000 pyextrasafe-0.0.0a1/src/safety_ctx.rs
```

### Comparing `pyextrasafe-0.0.0a0/Cargo.toml` & `pyextrasafe-0.0.0a1/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -10,21 +10,22 @@
 # KEEP SYNCHRONOUS TO REQUIREMENTS-READTHEDOCS.TXT (pyextrasafe)
 # KEEP SYNCHRONOUS TO LINKS IN README.MD (raw.githubusercontent.com)
 # Rust uses semver (https://semver.org/).
 # Python uses PEP 440 (https://www.python.org/dev/peps/pep-0440/).
 # Normal releases are exactly the same.
 # Pre-releases are X.Y.Z-aN in semver, and X.Y.ZaN in PEP 440.
 # Post-releases are X.Y.Z+N in semver, and X.Y.Z.postN in PEP 440.
-version = "0.0.0-a0"
+version = "0.0.0-a1"
 
 [lib]
 name = "_pyextrasafe"
 crate-type = ["cdylib"]
 
 [dependencies]
+bitflags = "2.3.1"
 extrasafe = "0.1.2"
 pyo3 = { version = "0.18.3", default-features = false, features = ["extension-module", "macros", "multiple-pymethods"] }
 
 [build-dependencies]
 pyo3-build-config = "0.18.3"
 
 [profile.release]
```

### Comparing `pyextrasafe-0.0.0a0/LICENSE.md` & `pyextrasafe-0.0.0a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyextrasafe-0.0.0a0/Makefile` & `pyextrasafe-0.0.0a1/Makefile`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-all: build docs
+all: build docs test
 
 
 .DELETE_ON_ERROR:
 .ONESHELL:
-.PHONY: all build clean dists docs install sdist
+.PHONY: all build clean dists docs install sdist test
 
 
 export ENV_DIR ?= env
 export PYTHON ?= python3.11
 
 
 clean:
@@ -51,15 +51,21 @@
 docs: install | ${ENV_DIR}/
 	set -eu
 
 	rm -r -- "./dist/doctrees/" || true
 	rm -r -- "./dist/html/" || true
 
 	. "./$${ENV_DIR}/bin/activate"
-	python3 -m sphinx -M html ./docs/ ./dist/
+	python3 -m sphinx -M html ./docs/ ./dist/ -W
+
+
+test: install | ${ENV_DIR}/
+	set -eu
+	. "./$${ENV_DIR}/bin/activate"
+	python3 hello-world.py
 
 
 dists:
 	${MAKE} PYTHON=python3.8 ENV_DIR=env3.8 build || true
 	${MAKE} PYTHON=python3.9 ENV_DIR=env3.9 build || true
 	${MAKE} PYTHON=python3.10 ENV_DIR=env3.10 build || true
 	${MAKE} PYTHON=python3.11 ENV_DIR=env3.11 build || true
```

### Comparing `pyextrasafe-0.0.0a0/PKG-INFO` & `pyextrasafe-0.0.0a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyextrasafe
-Version: 0.0.0a0
+Version: 0.0.0a1
 Summary: Make your code extrasafe by preventing it from calling unneeded syscalls
 Home-page: https://github.com/Kijewski/pyextrasafe
 Author: René Kijewski
 Author-email: pypi.org@k6i.de
 License: MIT License
 Project-URL: Changelog, https://github.com/Kijewski/pyextrasafe/blob/main/CHANGELOG.md
 Project-URL: Code, https://github.com/Kijewski/pyextrasafe
@@ -30,37 +30,38 @@
 # PyExtraSafe
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/Kijewski/pyextrasafe/ci.yml?branch=main&logo=github&logoColor=efefef&style=flat-square)](https://github.com/Kijewski/pyextrasafe/actions/workflows/ci.yml)
 [![Documentation Status](https://img.shields.io/readthedocs/pyextrasafe?logo=readthedocs&logoColor=efefef&style=flat-square)](https://pyextrasafe.readthedocs.io/)
 [![PyPI](https://img.shields.io/pypi/v/pyextrasafe?logo=pypi&logoColor=efefef&style=flat-square)](https://pypi.org/project/pyextrasafe/)
 [![Python >= 3.8](https://img.shields.io/badge/python-%E2%89%A5%203.8-informational?logo=python&logoColor=efefef&style=flat-square)](https://www.python.org/)
 [![OS: Linux](https://img.shields.io/badge/os-linux-informational?logo=linux&logoColor=efefef&style=flat-square)](https://www.kernel.org/)
-[![License](https://img.shields.io/badge/license-Apache--2.0-informational?logo=apache&logoColor=efefef&style=flat-square)](/LICENSE.md)
+[![License](https://img.shields.io/badge/license-Apache--2.0-informational?logo=apache&logoColor=efefef&style=flat-square)](https://github.com/Kijewski/pyextrasafe/blob/main/LICENSE.md)
 
 PyExtraSafe is a library that makes it easy to improve your program’s security by selectively
 allowing the syscalls it can perform via the Linux kernel’s seccomp facilities.
 
 The python library is a shallow wrapper around [extrasafe](https://docs.rs/extrasafe/0.1.2/extrasafe/index.html).
 
+### Quick Example
+
 ```python
 from threading import Thread
 import pyextrasafe
 
-
 try:
     thread = Thread(target=print, args=["Hello, world!"])
     thread.start()
     thread.join()
 except Exception:
     print("Could not run Thread (should have been able!)")
 
-ctx = pyextrasafe.SafetyContext()
-ctx.enable(pyextrasafe.BasicCapabilities())
-ctx.enable(pyextrasafe.SystemIO().allow_stdout().allow_stderr())
-ctx.apply_to_all_threads()
+pyextrasafe.SafetyContext().enable(
+    pyextrasafe.BasicCapabilities(),
+    pyextrasafe.SystemIO().allow_stdout().allow_stderr(),
+).apply_to_all_threads()
 
 try:
     thread = Thread(target=print, args=["Hello, world!"])
     thread.start()
     thread.join()
 except Exception:
     print("Could not run Thread (that's good!)")
```

### Comparing `pyextrasafe-0.0.0a0/README.md` & `pyextrasafe-0.0.0a1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 # PyExtraSafe
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/Kijewski/pyextrasafe/ci.yml?branch=main&logo=github&logoColor=efefef&style=flat-square)](https://github.com/Kijewski/pyextrasafe/actions/workflows/ci.yml)
 [![Documentation Status](https://img.shields.io/readthedocs/pyextrasafe?logo=readthedocs&logoColor=efefef&style=flat-square)](https://pyextrasafe.readthedocs.io/)
 [![PyPI](https://img.shields.io/pypi/v/pyextrasafe?logo=pypi&logoColor=efefef&style=flat-square)](https://pypi.org/project/pyextrasafe/)
 [![Python >= 3.8](https://img.shields.io/badge/python-%E2%89%A5%203.8-informational?logo=python&logoColor=efefef&style=flat-square)](https://www.python.org/)
 [![OS: Linux](https://img.shields.io/badge/os-linux-informational?logo=linux&logoColor=efefef&style=flat-square)](https://www.kernel.org/)
-[![License](https://img.shields.io/badge/license-Apache--2.0-informational?logo=apache&logoColor=efefef&style=flat-square)](/LICENSE.md)
+[![License](https://img.shields.io/badge/license-Apache--2.0-informational?logo=apache&logoColor=efefef&style=flat-square)](https://github.com/Kijewski/pyextrasafe/blob/main/LICENSE.md)
 
 PyExtraSafe is a library that makes it easy to improve your program’s security by selectively
 allowing the syscalls it can perform via the Linux kernel’s seccomp facilities.
 
 The python library is a shallow wrapper around [extrasafe](https://docs.rs/extrasafe/0.1.2/extrasafe/index.html).
 
+### Quick Example
+
 ```python
 from threading import Thread
 import pyextrasafe
 
-
 try:
     thread = Thread(target=print, args=["Hello, world!"])
     thread.start()
     thread.join()
 except Exception:
     print("Could not run Thread (should have been able!)")
 
-ctx = pyextrasafe.SafetyContext()
-ctx.enable(pyextrasafe.BasicCapabilities())
-ctx.enable(pyextrasafe.SystemIO().allow_stdout().allow_stderr())
-ctx.apply_to_all_threads()
+pyextrasafe.SafetyContext().enable(
+    pyextrasafe.BasicCapabilities(),
+    pyextrasafe.SystemIO().allow_stdout().allow_stderr(),
+).apply_to_all_threads()
 
 try:
     thread = Thread(target=print, args=["Hello, world!"])
     thread.start()
     thread.join()
 except Exception:
     print("Could not run Thread (that's good!)")
```

### Comparing `pyextrasafe-0.0.0a0/build.rs` & `pyextrasafe-0.0.0a1/build.rs`

 * *Files identical despite different names*

### Comparing `pyextrasafe-0.0.0a0/docs/conf.py` & `pyextrasafe-0.0.0a1/docs/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 language = "en"
 exclude_patterns = []
 pygments_style = "sphinx"
 todo_include_todos = False
 autoclass_content = "both"
 
 html_theme = "furo"
+html_static_path = ["_static"]
+html_css_files = ["custom.css"]
 
 project = "PyExtraSafe"
 copyright = "2023, René Kijewski"
 author = "René Kijewski"
 
 release = pyextrasafe.__version__
 version = re.match(r"\A\d+\.\d+\.\d+", release).group(0)
```

### Comparing `pyextrasafe-0.0.0a0/setup.cfg` & `pyextrasafe-0.0.0a1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 0.0.0a0
+version = 0.0.0a1
 name = pyextrasafe
 description = Make your code extrasafe by preventing it from calling unneeded syscalls
 author = René Kijewski
 author_email = pypi.org@k6i.de
 license = MIT License
 license_files = LICENSE.md
 long_description = file: README.md
```

### Comparing `pyextrasafe-0.0.0a0/src/lib.rs` & `pyextrasafe-0.0.0a1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pyextrasafe-0.0.0a0/src/pyextrasafe/__init__.py` & `pyextrasafe-0.0.0a1/src/pyextrasafe/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,26 +45,25 @@
 -------------
 
 .. code-block:: python
 
     from threading import Thread
     import pyextrasafe
 
-
     try:
         thread = Thread(target=print, args=["Hello, world!"])
         thread.start()
         thread.join()
     except Exception:
         print("Could not run Thread (should have been able!)")
 
-    ctx = pyextrasafe.SafetyContext()
-    ctx.enable(pyextrasafe.BasicCapabilities())
-    ctx.enable(pyextrasafe.SystemIO().allow_stdout().allow_stderr())
-    ctx.apply_to_all_threads()
+    pyextrasafe.SafetyContext().enable(
+        pyextrasafe.BasicCapabilities(),
+        pyextrasafe.SystemIO().allow_stdout().allow_stderr(),
+    ).apply_to_all_threads()
 
     try:
         thread = Thread(target=print, args=["Hello, world!"])
         thread.start()
         thread.join()
     except Exception:
         print("Could not run Thread (that's good!)")
@@ -81,14 +80,19 @@
     :members:
 
 .. autoexception:: pyextrasafe.ExtraSafeError
 
 Built-in profiles
 -----------------
 
+All built-in profiles inherit from :class:`~pyextrasafe.RuleSet`.
+Adding custom profiles is not implemented, yet.
+
+All methods return :code:`self`\, so method calls can be chained.
+
 .. autoclass:: pyextrasafe.BasicCapabilities
     :members:
 
 .. autoclass:: pyextrasafe.ForkAndExec
     :members:
 
 .. autoclass:: pyextrasafe.Threads
```

### Comparing `pyextrasafe-0.0.0a0/src/pyextrasafe.egg-info/PKG-INFO` & `pyextrasafe-0.0.0a1/src/pyextrasafe.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyextrasafe
-Version: 0.0.0a0
+Version: 0.0.0a1
 Summary: Make your code extrasafe by preventing it from calling unneeded syscalls
 Home-page: https://github.com/Kijewski/pyextrasafe
 Author: René Kijewski
 Author-email: pypi.org@k6i.de
 License: MIT License
 Project-URL: Changelog, https://github.com/Kijewski/pyextrasafe/blob/main/CHANGELOG.md
 Project-URL: Code, https://github.com/Kijewski/pyextrasafe
@@ -30,37 +30,38 @@
 # PyExtraSafe
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/Kijewski/pyextrasafe/ci.yml?branch=main&logo=github&logoColor=efefef&style=flat-square)](https://github.com/Kijewski/pyextrasafe/actions/workflows/ci.yml)
 [![Documentation Status](https://img.shields.io/readthedocs/pyextrasafe?logo=readthedocs&logoColor=efefef&style=flat-square)](https://pyextrasafe.readthedocs.io/)
 [![PyPI](https://img.shields.io/pypi/v/pyextrasafe?logo=pypi&logoColor=efefef&style=flat-square)](https://pypi.org/project/pyextrasafe/)
 [![Python >= 3.8](https://img.shields.io/badge/python-%E2%89%A5%203.8-informational?logo=python&logoColor=efefef&style=flat-square)](https://www.python.org/)
 [![OS: Linux](https://img.shields.io/badge/os-linux-informational?logo=linux&logoColor=efefef&style=flat-square)](https://www.kernel.org/)
-[![License](https://img.shields.io/badge/license-Apache--2.0-informational?logo=apache&logoColor=efefef&style=flat-square)](/LICENSE.md)
+[![License](https://img.shields.io/badge/license-Apache--2.0-informational?logo=apache&logoColor=efefef&style=flat-square)](https://github.com/Kijewski/pyextrasafe/blob/main/LICENSE.md)
 
 PyExtraSafe is a library that makes it easy to improve your program’s security by selectively
 allowing the syscalls it can perform via the Linux kernel’s seccomp facilities.
 
 The python library is a shallow wrapper around [extrasafe](https://docs.rs/extrasafe/0.1.2/extrasafe/index.html).
 
+### Quick Example
+
 ```python
 from threading import Thread
 import pyextrasafe
 
-
 try:
     thread = Thread(target=print, args=["Hello, world!"])
     thread.start()
     thread.join()
 except Exception:
     print("Could not run Thread (should have been able!)")
 
-ctx = pyextrasafe.SafetyContext()
-ctx.enable(pyextrasafe.BasicCapabilities())
-ctx.enable(pyextrasafe.SystemIO().allow_stdout().allow_stderr())
-ctx.apply_to_all_threads()
+pyextrasafe.SafetyContext().enable(
+    pyextrasafe.BasicCapabilities(),
+    pyextrasafe.SystemIO().allow_stdout().allow_stderr(),
+).apply_to_all_threads()
 
 try:
     thread = Thread(target=print, args=["Hello, world!"])
     thread.start()
     thread.join()
 except Exception:
     print("Could not run Thread (that's good!)")
```

### Comparing `pyextrasafe-0.0.0a0/src/pyextrasafe.egg-info/SOURCES.txt` & `pyextrasafe-0.0.0a1/src/pyextrasafe.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 requirements-dev.txt
 requirements-readthedocs.txt
 rustfmt.toml
 setup.cfg
 setup.py
 docs/conf.py
 docs/index.rst
+docs/_static/custom.css
 src/lib.rs
 src/rule_sets.rs
 src/safety_ctx.rs
 src/pyextrasafe/__init__.py
 src/pyextrasafe/__init__.pyi
 src/pyextrasafe/_pyextrasafe.pyi
 src/pyextrasafe/py.typed
```

