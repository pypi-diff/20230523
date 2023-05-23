# Comparing `tmp/tryceratops-2.3.1.tar.gz` & `tmp/tryceratops-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tryceratops-2.3.1.tar", max compression
+gzip compressed data, was "tryceratops-2.3.2.tar", max compression
```

## Comparing `tryceratops-2.3.1.tar` & `tryceratops-2.3.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1084 2023-05-20 14:58:46.889732 tryceratops-2.3.1/LICENSE
--rw-r--r--   0        0        0     6243 2023-05-20 14:59:24.646022 tryceratops-2.3.1/README.md
--rw-r--r--   0        0        0     2243 2023-05-20 14:59:24.714022 tryceratops-2.3.1/pyproject.toml
--rw-r--r--   0        0        0       69 2023-05-20 14:59:24.642022 tryceratops-2.3.1/src/tryceratops/__init__.py
--rw-r--r--   0        0        0     2227 2023-05-20 14:58:46.893733 tryceratops-2.3.1/src/tryceratops/__main__.py
--rw-r--r--   0        0        0     1185 2023-05-20 14:58:46.893733 tryceratops-2.3.1/src/tryceratops/analyzers/__init__.py
--rw-r--r--   0        0        0     1865 2023-05-20 14:58:46.893733 tryceratops-2.3.1/src/tryceratops/analyzers/base.py
--rw-r--r--   0        0        0     5624 2023-05-20 14:58:46.893733 tryceratops-2.3.1/src/tryceratops/analyzers/call.py
--rw-r--r--   0        0        0     2492 2023-05-20 14:58:46.893733 tryceratops-2.3.1/src/tryceratops/analyzers/classdefs.py
--rw-r--r--   0        0        0     2154 2023-05-20 14:58:46.893733 tryceratops-2.3.1/src/tryceratops/analyzers/conditional.py
--rw-r--r--   0        0        0     6385 2023-05-20 14:58:46.893733 tryceratops-2.3.1/src/tryceratops/analyzers/exception_block.py
--rw-r--r--   0        0        0      350 2023-05-20 14:58:46.893733 tryceratops-2.3.1/src/tryceratops/analyzers/exceptions.py
--rw-r--r--   0        0        0     1192 2023-05-20 14:58:46.893733 tryceratops-2.3.1/src/tryceratops/analyzers/try_block.py
--rw-r--r--   0        0        0       50 2023-05-20 14:58:46.893733 tryceratops-2.3.1/src/tryceratops/files/__init__.py
--rw-r--r--   0        0        0     3618 2023-05-20 14:58:46.893733 tryceratops-2.3.1/src/tryceratops/files/discovery.py
--rw-r--r--   0        0        0     1455 2023-05-20 14:58:46.893733 tryceratops-2.3.1/src/tryceratops/files/parser.py
--rw-r--r--   0        0        0      602 2023-05-20 14:58:46.893733 tryceratops-2.3.1/src/tryceratops/fixers/__init__.py
--rw-r--r--   0        0        0     2713 2023-05-20 14:58:46.893733 tryceratops-2.3.1/src/tryceratops/fixers/base.py
--rw-r--r--   0        0        0     2772 2023-05-20 14:58:46.893733 tryceratops-2.3.1/src/tryceratops/fixers/exception_block.py
--rw-r--r--   0        0        0      361 2023-05-20 14:58:46.893733 tryceratops-2.3.1/src/tryceratops/fixers/exceptions.py
--rw-r--r--   0        0        0     2130 2023-05-20 14:58:46.893733 tryceratops-2.3.1/src/tryceratops/flake_plugin.py
--rw-r--r--   0        0        0     2729 2023-05-20 14:58:46.897733 tryceratops-2.3.1/src/tryceratops/interfaces.py
--rw-r--r--   0        0        0     1065 2023-05-20 14:58:46.897733 tryceratops-2.3.1/src/tryceratops/logging_config.py
--rw-r--r--   0        0        0      165 2023-05-20 14:58:46.897733 tryceratops-2.3.1/src/tryceratops/processors.py
--rw-r--r--   0        0        0     3039 2023-05-20 14:58:46.897733 tryceratops-2.3.1/src/tryceratops/runners.py
--rw-r--r--   0        0        0     3629 2023-05-20 14:58:46.897733 tryceratops-2.3.1/src/tryceratops/settings.py
--rw-r--r--   0        0        0      791 2023-05-20 14:58:46.897733 tryceratops-2.3.1/src/tryceratops/types.py
--rw-r--r--   0        0        0      108 2023-05-20 14:58:46.897733 tryceratops-2.3.1/src/tryceratops/violations/__init__.py
--rw-r--r--   0        0        0     1745 2023-05-20 14:58:46.897733 tryceratops-2.3.1/src/tryceratops/violations/codes.py
--rw-r--r--   0        0        0     2403 2023-05-20 14:58:46.897733 tryceratops-2.3.1/src/tryceratops/violations/violations.py
--rw-r--r--   0        0        0     7443 1970-01-01 00:00:00.000000 tryceratops-2.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-05-23 11:13:05.464490 tryceratops-2.3.2/LICENSE
+-rw-r--r--   0        0        0     6243 2023-05-23 11:13:34.356360 tryceratops-2.3.2/README.md
+-rw-r--r--   0        0        0     2243 2023-05-23 11:13:34.412360 tryceratops-2.3.2/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-05-23 11:13:34.356360 tryceratops-2.3.2/src/tryceratops/__init__.py
+-rw-r--r--   0        0        0     2227 2023-05-23 11:13:05.468490 tryceratops-2.3.2/src/tryceratops/__main__.py
+-rw-r--r--   0        0        0     1185 2023-05-23 11:13:05.468490 tryceratops-2.3.2/src/tryceratops/analyzers/__init__.py
+-rw-r--r--   0        0        0     1865 2023-05-23 11:13:05.468490 tryceratops-2.3.2/src/tryceratops/analyzers/base.py
+-rw-r--r--   0        0        0     5624 2023-05-23 11:13:05.468490 tryceratops-2.3.2/src/tryceratops/analyzers/call.py
+-rw-r--r--   0        0        0     2492 2023-05-23 11:13:05.468490 tryceratops-2.3.2/src/tryceratops/analyzers/classdefs.py
+-rw-r--r--   0        0        0     2154 2023-05-23 11:13:05.468490 tryceratops-2.3.2/src/tryceratops/analyzers/conditional.py
+-rw-r--r--   0        0        0     6385 2023-05-23 11:13:05.468490 tryceratops-2.3.2/src/tryceratops/analyzers/exception_block.py
+-rw-r--r--   0        0        0      350 2023-05-23 11:13:05.468490 tryceratops-2.3.2/src/tryceratops/analyzers/exceptions.py
+-rw-r--r--   0        0        0     1192 2023-05-23 11:13:05.468490 tryceratops-2.3.2/src/tryceratops/analyzers/try_block.py
+-rw-r--r--   0        0        0       50 2023-05-23 11:13:05.468490 tryceratops-2.3.2/src/tryceratops/files/__init__.py
+-rw-r--r--   0        0        0     3626 2023-05-23 11:13:05.468490 tryceratops-2.3.2/src/tryceratops/files/discovery.py
+-rw-r--r--   0        0        0     1455 2023-05-23 11:13:05.468490 tryceratops-2.3.2/src/tryceratops/files/parser.py
+-rw-r--r--   0        0        0      602 2023-05-23 11:13:05.468490 tryceratops-2.3.2/src/tryceratops/fixers/__init__.py
+-rw-r--r--   0        0        0     2713 2023-05-23 11:13:05.468490 tryceratops-2.3.2/src/tryceratops/fixers/base.py
+-rw-r--r--   0        0        0     2772 2023-05-23 11:13:05.468490 tryceratops-2.3.2/src/tryceratops/fixers/exception_block.py
+-rw-r--r--   0        0        0      361 2023-05-23 11:13:05.468490 tryceratops-2.3.2/src/tryceratops/fixers/exceptions.py
+-rw-r--r--   0        0        0     2178 2023-05-23 11:13:05.468490 tryceratops-2.3.2/src/tryceratops/flake_plugin.py
+-rw-r--r--   0        0        0     2729 2023-05-23 11:13:05.468490 tryceratops-2.3.2/src/tryceratops/interfaces.py
+-rw-r--r--   0        0        0     1065 2023-05-23 11:13:05.468490 tryceratops-2.3.2/src/tryceratops/logging_config.py
+-rw-r--r--   0        0        0      869 2023-05-23 11:13:05.468490 tryceratops-2.3.2/src/tryceratops/parsing_types.py
+-rw-r--r--   0        0        0      165 2023-05-23 11:13:05.468490 tryceratops-2.3.2/src/tryceratops/processors.py
+-rw-r--r--   0        0        0     3047 2023-05-23 11:13:05.468490 tryceratops-2.3.2/src/tryceratops/runners.py
+-rw-r--r--   0        0        0     3637 2023-05-23 11:13:05.468490 tryceratops-2.3.2/src/tryceratops/settings.py
+-rw-r--r--   0        0        0      108 2023-05-23 11:13:05.468490 tryceratops-2.3.2/src/tryceratops/violations/__init__.py
+-rw-r--r--   0        0        0     1745 2023-05-23 11:13:05.468490 tryceratops-2.3.2/src/tryceratops/violations/codes.py
+-rw-r--r--   0        0        0     2403 2023-05-23 11:13:05.468490 tryceratops-2.3.2/src/tryceratops/violations/violations.py
+-rw-r--r--   0        0        0     7443 1970-01-01 00:00:00.000000 tryceratops-2.3.2/PKG-INFO
```

### Comparing `tryceratops-2.3.1/LICENSE` & `tryceratops-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.1/README.md` & `tryceratops-2.3.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 
 ## Pre-commit
 
 If you wish to use pre-commit, add this:
 
 ```yaml
   - repo: https://github.com/guilatrova/tryceratops
-    rev: v2.3.1
+    rev: v2.3.2
     hooks:
       - id: tryceratops
 ```
 
 ## Show your style
 
 [![try/except style: tryceratops](https://img.shields.io/badge/try%2Fexcept%20style-tryceratops%20%F0%9F%A6%96%E2%9C%A8-black)](https://github.com/guilatrova/tryceratops)
```

### Comparing `tryceratops-2.3.1/pyproject.toml` & `tryceratops-2.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tryceratops"
-version = "2.3.1"
+version = "2.3.2"
 description = "Prevent Exception Handling AntiPatterns"
 authors = ["Guilherme Latrova <hello@guilatrova.dev>"]
 license = "MIT"
 keywords = ["lint", "try", "except"]
 readme = "README.md"
 homepage = "https://github.com/guilatrova/tryceratops"
 repository = "https://github.com/guilatrova/tryceratops"
@@ -50,15 +50,15 @@
 build_command = "pip install poetry && poetry build"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 click = ">=7"
 toml = ">=0.10.2"
 rich = ">=10.14.0"
-typing-extensions = { version = ">=4.5.0", python = "<3.10" }
+typing-extensions = { version = ">=4.5.0", python = "<3.11" }
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^2.12.1"
 flake8 = "^6.0.0"
 flake8-annotations = "^3.0.1"
 black = "^23.3.0"
```

### Comparing `tryceratops-2.3.1/src/tryceratops/__main__.py` & `tryceratops-2.3.2/src/tryceratops/__main__.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.1/src/tryceratops/analyzers/__init__.py` & `tryceratops-2.3.2/src/tryceratops/analyzers/__init__.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.1/src/tryceratops/analyzers/base.py` & `tryceratops-2.3.2/src/tryceratops/analyzers/base.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.1/src/tryceratops/analyzers/call.py` & `tryceratops-2.3.2/src/tryceratops/analyzers/call.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.1/src/tryceratops/analyzers/classdefs.py` & `tryceratops-2.3.2/src/tryceratops/analyzers/classdefs.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.1/src/tryceratops/analyzers/conditional.py` & `tryceratops-2.3.2/src/tryceratops/analyzers/conditional.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.1/src/tryceratops/analyzers/exception_block.py` & `tryceratops-2.3.2/src/tryceratops/analyzers/exception_block.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.1/src/tryceratops/analyzers/try_block.py` & `tryceratops-2.3.2/src/tryceratops/analyzers/try_block.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.1/src/tryceratops/files/discovery.py` & `tryceratops-2.3.2/src/tryceratops/files/discovery.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import toml
 from dataclasses import dataclass
 from os import listdir
 from os.path import isdir, isfile, join
 from pathlib import Path
 from typing import Generator, Iterable, List, Optional, Sequence
 
-from tryceratops.types import ParsedFileType, PyprojectConfig
+from tryceratops.parsing_types import ParsedFileType, PyprojectConfig
 
 from .parser import parse_file
 
 logger = logging.getLogger(__name__)
 
 
 def is_python_file(filename: str) -> bool:
```

### Comparing `tryceratops-2.3.1/src/tryceratops/files/parser.py` & `tryceratops-2.3.2/src/tryceratops/files/parser.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.1/src/tryceratops/fixers/__init__.py` & `tryceratops-2.3.2/src/tryceratops/fixers/__init__.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.1/src/tryceratops/fixers/base.py` & `tryceratops-2.3.2/src/tryceratops/fixers/base.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.1/src/tryceratops/fixers/exception_block.py` & `tryceratops-2.3.2/src/tryceratops/fixers/exception_block.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.1/src/tryceratops/flake_plugin.py` & `tryceratops-2.3.2/src/tryceratops/flake_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,19 @@
 from tryceratops.files.parser import parse_ignore_tokens
 from tryceratops.runners import Runner
 from tryceratops.settings import FileFilter, GlobalSettings
 from tryceratops.violations.violations import Violation
 
 PACKAGE_NAME = "tryceratops"
 GLOBAL_DUMMY_FILTER = GlobalSettings(
-    include_experimental=False, ignore_violations=[], exclude_dirs=[], autofix=False
+    include_experimental=False,
+    ignore_violations=[],
+    exclude_dirs=[],
+    autofix=False,
+    allowed_base_exceptions=set(),
 )
 FLAKE8_VIOLATION_TYPE = Tuple[int, int, str, Type[Any]]
 # line, offset, message, class
 
 
 class TryceratopsAdapterPlugin:
     name = PACKAGE_NAME
```

### Comparing `tryceratops-2.3.1/src/tryceratops/interfaces.py` & `tryceratops-2.3.2/src/tryceratops/interfaces.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.1/src/tryceratops/logging_config.py` & `tryceratops-2.3.2/src/tryceratops/logging_config.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.1/src/tryceratops/runners.py` & `tryceratops-2.3.2/src/tryceratops/runners.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import ast
 import logging
 from dataclasses import dataclass
 from typing import List, Set, Type
 
 from tryceratops.analyzers import BaseAnalyzer, get_analyzer_chain
 from tryceratops.fixers import BaseFixer, get_fixers_chain
+from tryceratops.parsing_types import ParsedFilesType
 from tryceratops.processors import Processor
 from tryceratops.settings import FileFilter, GlobalSettings
-from tryceratops.types import ParsedFilesType
 from tryceratops.violations import Violation
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class RuntimeError:
```

### Comparing `tryceratops-2.3.1/src/tryceratops/settings.py` & `tryceratops-2.3.2/src/tryceratops/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import TYPE_CHECKING, Iterable, Optional, Set, Type
 
 from tryceratops.processors import Processor
 from tryceratops.violations import Violation
 from tryceratops.violations.codes import NON_PICKABLE_CLASS
 
 if TYPE_CHECKING:
-    from tryceratops.types import PyprojectConfig
+    from tryceratops.parsing_types import PyprojectConfig
 
 
 @dataclass
 class IgnoreViolation:
     line: int
     code: Optional[Iterable[str]] = None
```

### Comparing `tryceratops-2.3.1/src/tryceratops/types.py` & `tryceratops-2.3.2/src/tryceratops/parsing_types.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 import ast
+import sys
 import typing as t
-import typing_extensions as te
+
+if sys.version_info >= (3, 11):
+    import typing as te
+else:
+    import typing_extensions as te
 
 from tryceratops.settings import FileFilter
 
 ParsedFileType = t.Tuple[str, ast.AST, FileFilter]
 ParsedFilesType = t.Collection[ParsedFileType]
```

### Comparing `tryceratops-2.3.1/src/tryceratops/violations/codes.py` & `tryceratops-2.3.2/src/tryceratops/violations/codes.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.1/src/tryceratops/violations/violations.py` & `tryceratops-2.3.2/src/tryceratops/violations/violations.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.1/PKG-INFO` & `tryceratops-2.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tryceratops
-Version: 2.3.1
+Version: 2.3.2
 Summary: Prevent Exception Handling AntiPatterns
 Home-page: https://github.com/guilatrova/tryceratops
 License: MIT
 Keywords: lint,try,except
 Author: Guilherme Latrova
 Author-email: hello@guilatrova.dev
 Requires-Python: >=3.8.1,<4.0
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Dist: click (>=7)
 Requires-Dist: rich (>=10.14.0)
 Requires-Dist: toml (>=0.10.2)
-Requires-Dist: typing-extensions (>=4.5.0) ; python_version < "3.10"
+Requires-Dist: typing-extensions (>=4.5.0) ; python_version < "3.11"
 Project-URL: Changelog, https://github.com/guilatrova/tryceratops/blob/main/CHANGELOG.md
 Project-URL: Repository, https://github.com/guilatrova/tryceratops
 Description-Content-Type: text/markdown
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/guilatrova/tryceratops/main/img/logo.png">
 </p>
@@ -171,15 +171,15 @@
 
 ## Pre-commit
 
 If you wish to use pre-commit, add this:
 
 ```yaml
   - repo: https://github.com/guilatrova/tryceratops
-    rev: v2.3.1
+    rev: v2.3.2
     hooks:
       - id: tryceratops
 ```
 
 ## Show your style
 
 [![try/except style: tryceratops](https://img.shields.io/badge/try%2Fexcept%20style-tryceratops%20%F0%9F%A6%96%E2%9C%A8-black)](https://github.com/guilatrova/tryceratops)
```

