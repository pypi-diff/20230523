# Comparing `tmp/pysast-1.1.2a0.tar.gz` & `tmp/pysast-1.1.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysast-1.1.2a0.tar", max compression
+gzip compressed data, was "pysast-1.1.3a0.tar", max compression
```

## Comparing `pysast-1.1.2a0.tar` & `pysast-1.1.3a0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    35802 2023-05-18 12:47:39.295835 pysast-1.1.2a0/LICENSE
--rw-r--r--   0        0        0     1198 2023-05-21 07:01:09.081563 pysast-1.1.2a0/pyproject.toml
--rw-r--r--   0        0        0    41389 2023-05-21 07:01:09.111227 pysast-1.1.2a0/pysast.py
--rw-r--r--   0        0        0     4922 2023-05-21 07:01:09.042706 pysast-1.1.2a0/README.md
--rw-r--r--   0        0        0     5648 1970-01-01 00:00:00.000000 pysast-1.1.2a0/PKG-INFO
+-rw-r--r--   0        0        0    35802 2023-05-18 12:47:39.295835 pysast-1.1.3a0/LICENSE
+-rw-r--r--   0        0        0     1198 2023-05-23 13:03:57.934055 pysast-1.1.3a0/pyproject.toml
+-rw-r--r--   0        0        0    41676 2023-05-23 13:03:57.965057 pysast-1.1.3a0/pysast.py
+-rw-r--r--   0        0        0     4922 2023-05-23 13:03:57.832210 pysast-1.1.3a0/README.md
+-rw-r--r--   0        0        0     5648 1970-01-01 00:00:00.000000 pysast-1.1.3a0/PKG-INFO
```

### Comparing `pysast-1.1.2a0/LICENSE` & `pysast-1.1.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysast-1.1.2a0/pyproject.toml` & `pysast-1.1.3a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysast"
-version = "1.1.2-alpha"
+version = "1.1.3-alpha"
 description="SAST Code Scanner in Python"
 authors = ["MatrixEditor"]
 keywords = ["pysast"]
 readme = "README.md"
 license = "GNU GPLv3"
 classifiers = [
      # How mature is this project? Common values are
```

### Comparing `pysast-1.1.2a0/pysast.py` & `pysast-1.1.3a0/pysast.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from __future__ import annotations
 
 __doc__ = """Simple and small python module to perform SAST scans."""
 __version__ = "1.1"
-__sem_version__ = "1.1.2-alpha"
+__sem_version__ = "1.1.3-alpha"
 __authors__ = "MatrixEditor"
 
 import sys
 import os
 import re
 import logging
 import json
@@ -191,15 +191,15 @@
         matches = False
         for item in [x.strip() for x in value.strip().split(",")]:
             if self._use_re:
                 matches = matches or re.search(item, target, re.IGNORECASE)
             else:
                 matches = matches or item.lower() in target.lower()
 
-        return (self._inverted and matches) or (not self._inverted and not matches)
+        return (self._inverted and not matches) or (not self._inverted and matches)
 
 
 class SupportsFilter:
     """A mixin class for supporting filtering based on predefined criteria.
 
     The ``SupportsFilter`` class provides a method for applying filters to a file
     based on various criteria such as file extension, file name, full path, and MIME
@@ -252,15 +252,17 @@
 
             if value.startswith("re:"):
                 # Enable regular expression matching
                 file_filter.with_re()
                 value = value[3:]
 
             if key.lower() == FILTER_FILE_EXT:
-                target = "" if "." not in file_path else file_path.split(".")[-1]
+                target = (
+                    "" if "." not in file_path else pathlib.Path(file_path).suffix[1:]
+                )
             elif key.lower() == FILTER_FILE_NAME:
                 target = os.path.basename(file_path)  # Extract file name
             elif key.lower() == FILTER_FULL_PATH:
                 target = file_path
             elif key.lower() == FILTER_MIME_TYPE:
                 target = mime_type
             else:
@@ -381,14 +383,17 @@
         if not hasattr(mod, "compile"):
             mod = re
             logger.warning("Target module has not compile() function: %s", self.engine)
 
         # Compilation errors should be visible to the user
         self.re_pattern = mod.compile(self.text.encode(errors="replace"))
 
+    def __repr__(self) -> str:
+        return "<SastPattern re='%s'>" % self.text
+
 
 class SastRule(SupportsFilter):
     """A class to describe a single SAST rule.
 
     It extends the :class:`SupportsFilter` class. The purpose of this class is
     to encapsulate a rule with its associated content, filters, and patterns. It
     also provides methods to add patterns and reset its internal state.
@@ -406,15 +411,15 @@
     def __init__(self, rule_id: str, rule_content: dict) -> None:
         self.rule_id = rule_id
         self.rule_content = rule_content
         self.filters = {}
         self.patterns = []
 
         # Filters are optional so we don't have to use them
-        if "filter" in self.rule_content.get("meta", {}):
+        if "filters" in self.rule_content.get("meta", {}):
             self.filters = extract_filter_keys(self.rule_content["meta"], is_meta=True)
 
         # Patterns can be declared as pure string with default filter mode "and"
         # and can be defined in two ways:
         # 1. Single pattern: Use the "pattern" attribute to define a single pattern
         if "pattern" in self.rule_content:
             pattern = self.rule_content["pattern"]
@@ -547,14 +552,16 @@
 
         # If any of the required patterns don't have a match, it also indicates
         # that the rule does not have a match, and False is returned.
         for pattern in self.rule.required_patterns:
             if pattern not in self._pattern_matches:
                 return False
 
+        # If no required patterns are defined and only optional patterns (or),
+        # at least one has to be detected:
         return len(self._pattern_matches) > 0
 
     def search(self, line: bytes, line_index: int, abs_offset: int):
         """Search for matches of the rule's patterns in a given line.
 
         Before searching for matches, the method checks if a transformation is
         specified in the rule's content using the ``"input"``. If the transformation
@@ -584,15 +591,15 @@
         :type abs_offset: int
         """
         transform = self.rule.rule_content.get("input", "default")
         if transform != "default" and hasattr(line, transform):
             line = getattr(line, transform)()
 
         for pattern in self.rule.patterns:
-            result = re.search(pattern.re_pattern, line)
+            result = pattern.re_pattern.search(line)
 
             if result and len(self._matches) < DEFAULT_MAX_MATCHES:
                 self._lines.append(line_index)
                 start, _ = result.span()
                 self._positions.append(abs_offset + (start or 1))
                 if pattern not in self._pattern_matches:
                     self._pattern_matches.append(pattern)
@@ -656,14 +663,15 @@
 
         fp.close()
         for rule in self.sast_rules:
             rule_result = rule.create_result(file_path)
             if rule_result:
                 result.append(rule_result)
 
+        del self.sast_rules
         return result
 
 
 class SastScanner(SupportsFilter):
     """
     A class representing a static application security scanner.
 
@@ -761,15 +769,15 @@
     @property
     def has_matches(self) -> bool:
         """Check if there are any scan results.
 
         :return: True if there are scan results, False otherwise.
         :rtype: bool
         """
-        return len(self._scan_results) != 0
+        return len(self.scan_results) != 0
 
     @property
     def json(self) -> str:
         """Get the scan results in JSON format.
 
         :return: A string representing the scan results in JSON format.
         """
@@ -1090,15 +1098,15 @@
         )
         print(
             intent * 3,
             "Offsets:",
             pprint.pformat(match[RESULT_KEY_POSITIONS], compact=True),
         )
         print(intent * 3, "Meta:")
-        for key, value in match.get('meta', {}).items():
+        for key, value in match.get("meta", {}).items():
             print(intent * 6, f"{key}: {value}")
         print()
 
     def scan_file(file_path: str) -> bool:
         try:
             if scanner.scan(file_path):
                 if args.dump_json:
```

### Comparing `pysast-1.1.2a0/README.md` & `pysast-1.1.3a0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # PySAST
 
 [![python](https://img.shields.io/badge/python-3.8+-blue.svg?logo=python&labelColor=lightgrey)](https://www.python.org/downloads/)
 ![Status](https://img.shields.io:/static/v1?label=Status&message=Alpha-Release&color=lightgreen)
 ![Platform](https://img.shields.io:/static/v1?label=Platforms&message=All&color=yellowgreen)
-![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=1.1.2-alpha&color=lightblue)
+![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=1.1.3-alpha&color=lightblue)
 ![Codestyle](https://img.shields.io:/static/v1?label=Codestyle&message=black&color=black)
 
 Welcome to `pysast` - a powerful Python package designed for scanning one or multiple files using customizable rules written
 in JSON or YAML. This package allows you to automate the process of code analysis and identify potential issues or violations
 based on your specified criteria.
 
 By utilizing the rule-based system, you can define a set of rules that reflect your desired coding standards, best practices,
```

### Comparing `pysast-1.1.2a0/PKG-INFO` & `pysast-1.1.3a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysast
-Version: 1.1.2a0
+Version: 1.1.3a0
 Summary: SAST Code Scanner in Python
 License: GNU GPLv3
 Keywords: pysast
 Author: MatrixEditor
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -21,15 +21,15 @@
 Description-Content-Type: text/markdown
 
 # PySAST
 
 [![python](https://img.shields.io/badge/python-3.8+-blue.svg?logo=python&labelColor=lightgrey)](https://www.python.org/downloads/)
 ![Status](https://img.shields.io:/static/v1?label=Status&message=Alpha-Release&color=lightgreen)
 ![Platform](https://img.shields.io:/static/v1?label=Platforms&message=All&color=yellowgreen)
-![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=1.1.2-alpha&color=lightblue)
+![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=1.1.3-alpha&color=lightblue)
 ![Codestyle](https://img.shields.io:/static/v1?label=Codestyle&message=black&color=black)
 
 Welcome to `pysast` - a powerful Python package designed for scanning one or multiple files using customizable rules written
 in JSON or YAML. This package allows you to automate the process of code analysis and identify potential issues or violations
 based on your specified criteria.
 
 By utilizing the rule-based system, you can define a set of rules that reflect your desired coding standards, best practices,
```

