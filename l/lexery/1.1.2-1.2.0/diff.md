# Comparing `tmp/lexery-1.1.2.tar.gz` & `tmp/lexery-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexery-1.1.2.tar", last modified: Sun Apr  3 08:13:30 2022, max compression
+gzip compressed data, was "lexery-1.2.0.tar", last modified: Tue May 23 21:27:42 2023, max compression
```

## Comparing `lexery-1.1.2.tar` & `lexery-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-03 08:13:30.682217 lexery-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)     6047 2022-04-03 08:13:30.682217 lexery-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5264 2022-04-03 08:13:19.000000 lexery-1.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-03 08:13:30.678217 lexery-1.1.2/lexery/
--rw-r--r--   0 runner    (1001) docker     (121)     7477 2022-04-03 08:13:19.000000 lexery-1.1.2/lexery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-04-03 08:13:19.000000 lexery-1.1.2/lexery/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-03 08:13:30.682217 lexery-1.1.2/lexery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6047 2022-04-03 08:13:30.000000 lexery-1.1.2/lexery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      203 2022-04-03 08:13:30.000000 lexery-1.1.2/lexery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-03 08:13:30.000000 lexery-1.1.2/lexery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-04-03 08:13:30.000000 lexery-1.1.2/lexery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-04-03 08:13:30.000000 lexery-1.1.2/lexery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-03 08:13:30.682217 lexery-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1637 2022-04-03 08:13:19.000000 lexery-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:27:42.814240 lexery-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-05-23 21:27:42.814240 lexery-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-05-23 21:27:31.000000 lexery-1.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:27:42.814240 lexery-1.2.0/lexery/
+-rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-05-23 21:27:31.000000 lexery-1.2.0/lexery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-23 21:27:31.000000 lexery-1.2.0/lexery/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:27:42.814240 lexery-1.2.0/lexery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-05-23 21:27:42.000000 lexery-1.2.0/lexery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-23 21:27:42.000000 lexery-1.2.0/lexery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 21:27:42.000000 lexery-1.2.0/lexery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-23 21:27:42.000000 lexery-1.2.0/lexery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 21:27:42.000000 lexery-1.2.0/lexery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 21:27:42.814240 lexery-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-23 21:27:31.000000 lexery-1.2.0/setup.py
```

### Comparing `lexery-1.1.2/PKG-INFO` & `lexery-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: lexery
-Version: 1.1.2
+Version: 1.2.0
 Summary: A simple lexer based on regular expressions
 Home-page: https://github.com/Parquery/lexery
 Author: Marko Ristin
 Author-email: marko@ristin.ch
 License: License :: OSI Approved :: MIT License
 Keywords: lexer regexp regular expression
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: dev
 
 Lexery
 ======
 
 .. image:: https://github.com/Parquery/lexery/actions/workflows/ci.yml/badge.svg
     :target: https://github.com/Parquery/lexery/actions/workflows/ci.yml
@@ -182,9 +180,7 @@
 Versioning
 ==========
 We follow `Semantic Versioning <http://semver.org/spec/v1.0.0.html>`_. The version X.Y.Z indicates:
 
 * X is the major version (backward-incompatible),
 * Y is the minor version (backward-compatible), and
 * Z is the patch version (backward-compatible bug fix).
-
-
```

### Comparing `lexery-1.1.2/README.rst` & `lexery-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `lexery-1.1.2/lexery/__init__.py` & `lexery-1.2.0/lexery/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 """Provide a simple lexer based on regular expressions."""
 import re
 from typing import List, Pattern, Optional
 
 # Don't forget to update the version in setup.py and CHANGELOG.rst!
-__version__ = '1.1.2'
+__version__ = '1.2.0'
 __author__ = 'Marko Ristin'
 __license__ = 'MIT'
 __status__ = 'Production'
 
 
 class Token:
     """Represent a token of a text."""
@@ -39,23 +39,48 @@
         return self.identifier == other.identifier and self.lineno == other.lineno and \
                self.position == other.position and self.content == other.content
 
 
 class Rule:
     """Define a lexing rule."""
 
-    def __init__(self, identifier: str, pattern: Pattern) -> None:
+    def __init__(self, identifier: str, pattern: Pattern, next_rule=None) -> None:
         """
         Initialize.
 
         :param identifier: of the rule
         :param pattern: regular expression defining the rule
         """
         self.identifier = identifier
         self.pattern = pattern
+        self.next_rule = next_rule
+
+    def match(self, text, pos, lno):
+        """
+        Match the rules with given text and position.
+
+        :param text: the given texte to match
+        :param pos: position of the text
+        :param lno: line number of the text
+        """
+        mtch = self.pattern.match(text, pos)
+        ret = []
+        if self.next_rule is not None and mtch is not None:
+            pos = 0
+            for rule in self.next_rule:
+                another_mtch, another_t = rule.match(mtch.group(), pos, 0)
+                if another_mtch:
+                    ret.append(another_t)
+                    pos += len(another_mtch.group())
+        else:
+            if mtch:
+                ret = mtch.group()
+            else:
+                ret = ''
+        return mtch, Token(self.identifier, content=ret, position=pos, lineno=lno)
 
 
 NONTAB_RE = re.compile(r'[^\t]')
 
 
 class Error(Exception):
     """Is raised when no token rule applies."""
@@ -73,15 +98,15 @@
         self.lineno = lineno
 
         super().__init__()
 
     def __str__(self) -> str:
         """Represent the error with a nice pointer as a multi-line message."""
         pointer = re.sub(NONTAB_RE, ' ', self.line[:self.position]) + '^'
-        txt = (f'Unmatched text at line {self.lineno} and position {self.position}:\n' f'{self.line}\n' f'{pointer}')
+        txt = f'Unmatched text at line {self.lineno} and position {self.position}:\n{self.line}\n{pointer}'
         return txt
 
 
 WHITESPACE_RE = re.compile(r'\s')
 
 
 class _Lexing:
@@ -186,19 +211,18 @@
         lexing = _Lexing(unmatched_identifier=self.unmatched_identifier)
 
         for lineno, line in enumerate(lines):
             position = 0
             while position < len(line):
                 mtched = False
                 for rule in self.rules:
-                    mtch = rule.pattern.match(line, position)
+                    another_line = line
+                    mtch, another_token = rule.match(another_line, position, lineno)
                     if mtch:
-                        token = Token(
-                            identifier=rule.identifier, content=mtch.group(), position=position, lineno=lineno)
-
+                        token = another_token
                         lexing.emit_matched_token(token=token)
 
                         position = mtch.end()
                         mtched = True
                         break
 
                 if not mtched:
```

### Comparing `lexery-1.1.2/lexery.egg-info/PKG-INFO` & `lexery-1.2.0/lexery.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: lexery
-Version: 1.1.2
+Version: 1.2.0
 Summary: A simple lexer based on regular expressions
 Home-page: https://github.com/Parquery/lexery
 Author: Marko Ristin
 Author-email: marko@ristin.ch
 License: License :: OSI Approved :: MIT License
 Keywords: lexer regexp regular expression
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: dev
 
 Lexery
 ======
 
 .. image:: https://github.com/Parquery/lexery/actions/workflows/ci.yml/badge.svg
     :target: https://github.com/Parquery/lexery/actions/workflows/ci.yml
@@ -182,9 +180,7 @@
 Versioning
 ==========
 We follow `Semantic Versioning <http://semver.org/spec/v1.0.0.html>`_. The version X.Y.Z indicates:
 
 * X is the major version (backward-incompatible),
 * Y is the minor version (backward-compatible), and
 * Z is the patch version (backward-compatible bug fix).
-
-
```

### Comparing `lexery-1.1.2/setup.py` & `lexery-1.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,31 +11,34 @@
 # pylint: disable=redefined-builtin
 here = os.path.abspath(os.path.dirname(__file__))  # pylint: disable=invalid-name
 with open(os.path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()  # pylint: disable=invalid-name
 
 setup(
     name='lexery',
-    version='1.1.2',  # Don't forget to update the changelog and __init__.py!
+    version='1.2.0',  # Don't forget to update the changelog and __init__.py!
     description='A simple lexer based on regular expressions',
     long_description=long_description,
     url='https://github.com/Parquery/lexery',
     author='Marko Ristin',
     author_email='marko@ristin.ch',
     # yapf: disable
     classifiers=[
-        'Development Status :: 5 - Production/Stable', 'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License', 'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6', 'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8', 'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10'
+        'Development Status :: 5 - Production/Stable',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     # yapf: enable
     keywords='lexer regexp regular expression',
     license='License :: OSI Approved :: MIT License',
     packages=find_packages(exclude=['contrib', 'docs', 'tests*']),
     install_requires=[],
     extras_require={
-        'dev': ['mypy==0.942', 'pylint==2.13.4', 'yapf==0.20.2', 'coverage>=4.5.1,<5', 'pydocstyle==6.1.1']
+        'dev': ['mypy==1.2.0', 'pylint==2.17.2', 'yapf==0.20.2', 'coverage>=4.5.1,<5', 'pydocstyle==6.1.1']
     },
     py_modules=['lexery'],
     package_data={"lexery": ["py.typed"]})
```

