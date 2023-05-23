# Comparing `tmp/deadnews_template_python-1.0.2a6.tar.gz` & `tmp/deadnews_template_python-1.0.3a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deadnews_template_python-1.0.2a6.tar", max compression
+gzip compressed data, was "deadnews_template_python-1.0.3a2.tar", max compression
```

## Comparing `deadnews_template_python-1.0.2a6.tar` & `deadnews_template_python-1.0.3a2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1065 2023-05-04 01:39:34.631887 deadnews_template_python-1.0.2a6/LICENSE
--rw-r--r--   0        0        0      845 2023-05-04 01:39:34.631887 deadnews_template_python-1.0.2a6/README.md
--rw-r--r--   0        0        0     2363 2023-05-04 01:39:51.584123 deadnews_template_python-1.0.2a6/pyproject.toml
--rw-r--r--   0        0        0      160 2023-05-04 01:39:34.631887 deadnews_template_python-1.0.2a6/src/deadnews_template_python/__init__.py
--rw-r--r--   0        0        0     1508 1970-01-01 00:00:00.000000 deadnews_template_python-1.0.2a6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-23 16:01:52.937966 deadnews_template_python-1.0.3a2/LICENSE
+-rw-r--r--   0        0        0      845 2023-05-23 16:01:52.937966 deadnews_template_python-1.0.3a2/README.md
+-rw-r--r--   0        0        0     2176 2023-05-23 16:02:08.950144 deadnews_template_python-1.0.3a2/pyproject.toml
+-rw-r--r--   0        0        0      160 2023-05-23 16:01:52.937966 deadnews_template_python-1.0.3a2/src/deadnews_template_python/__init__.py
+-rw-r--r--   0        0        0     1508 1970-01-01 00:00:00.000000 deadnews_template_python-1.0.3a2/PKG-INFO
```

### Comparing `deadnews_template_python-1.0.2a6/LICENSE` & `deadnews_template_python-1.0.3a2/LICENSE`

 * *Files identical despite different names*

### Comparing `deadnews_template_python-1.0.2a6/README.md` & `deadnews_template_python-1.0.3a2/README.md`

 * *Files identical despite different names*

### Comparing `deadnews_template_python-1.0.2a6/pyproject.toml` & `deadnews_template_python-1.0.3a2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "deadnews-template-python"
-version = "1.0.2-alpha.6"
+version = "1.0.3-alpha.2"
 description = "Python Project Template"
 authors = ["DeadNews <aurczpbgr@mozmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/DeadNews/deadnews-template-python"
 repository = "https://github.com/DeadNews/deadnews-template-python"
 keywords = ["python", "template", "layout"]
@@ -17,23 +17,23 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 
 [tool.poetry.group.ci.dependencies]
 black = "^23.3.0"
 mypy = "^1.2.0"
 poethepoet = "^0.20.0"
-ruff = "^0.0.264"
+ruff = "^0.0.267"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 
 [tool.poe.tasks]
-ruff = "ruff check . --diff --format github"
-black = "black . --check --diff"
+ruff = "ruff check ."
+black = "black --check ."
 mypy = "mypy ."
 ci.sequence = ["ruff", "black", "mypy"]
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
@@ -52,45 +52,34 @@
 [[tool.mypy.overrides]]
 module = ["tests.*"]
 allow_untyped_defs = true
 
 [tool.pytest.ini_options]
 addopts = "--verbose --cov=./src"
 testpaths = ["tests"]
-markers = ["docker", "slow"]
+markers = ["docker", "key_required"]
 
 [tool.coverage.report]
-exclude_lines = ["if __name__ == .__main__.:"]
+exclude_lines = ["if TYPE_CHECKING:", "if __name__ == .__main__.:"]
 
 [tool.ruff]
 line-length = 99
 select = ["ALL"]
 ignore = [
-  "D203",    # 1 blank line required before class docstring
-  "D212",    # Multi-line docstring summary should start at the first line
-  "E501",    # Line too long
-  "EXE001",  # Shebang is present but file is not executable
-  "FBT001",  # Boolean positional arg in function definition
-  "PLR2004", # Magic value used in comparison
-  "S113",    # Missing requests timeout
-  "S603",    # Calling subprocess.Popen with shell=False
+  "COM812", # Trailing comma missing
+  "D203",   # 1 blank line required before class docstring
+  "D212",   # Multi-line docstring summary should start at the first line
+  "E501",   # Line too long
+  "EXE001", # Shebang is present but file is not executable
+  "FBT001", # Boolean positional arg in function definition
+  "FBT002", # Boolean default value in function definition
 ]
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
-"tests/*" = ["ANN", "D", "S"]
+"tests/*" = ["ANN", "D", "PLC1901", "PLR2004", "S"]
 
 [tool.ruff.flake8-comprehensions]
 allow-dict-calls-with-keyword-arguments = false
 
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "all"
-
-[tool.ruff.mccabe]
-max-complexity = 10
-
-[tool.ruff.pylint]
-max-args = 5
-
-# [tool.ruff.pydocstyle]
-# # Use Google-style docstrings.
-# convention = "pep257"
```

### Comparing `deadnews_template_python-1.0.2a6/PKG-INFO` & `deadnews_template_python-1.0.3a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deadnews-template-python
-Version: 1.0.2a6
+Version: 1.0.3a2
 Summary: Python Project Template
 Home-page: https://github.com/DeadNews/deadnews-template-python
 License: MIT
 Keywords: python,template,layout
 Author: DeadNews
 Author-email: aurczpbgr@mozmail.com
 Requires-Python: >=3.10,<4.0
```

