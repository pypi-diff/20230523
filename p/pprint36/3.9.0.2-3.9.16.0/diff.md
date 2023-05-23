# Comparing `tmp/pprint36-3.9.0.2.tar.gz` & `tmp/pprint36-3.9.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pprint36-3.9.0.2.tar", last modified: Sun Sep 20 17:18:27 2020, max compression
+gzip compressed data, was "pprint36-3.9.16.0.tar", last modified: Tue May 23 13:35:33 2023, max compression
```

## Comparing `pprint36-3.9.0.2.tar` & `pprint36-3.9.16.0.tar`

### file list

```diff
@@ -1,22 +1,9 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-20 17:18:27.000000 pprint36-3.9.0.2/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-09-20 17:18:00.000000 pprint36-3.9.0.2/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1124 2020-09-20 17:18:27.000000 pprint36-3.9.0.2/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     4116 2020-09-20 17:18:00.000000 pprint36-3.9.0.2/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-20 17:18:27.000000 pprint36-3.9.0.2/pprint36.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2020-09-20 17:18:27.000000 pprint36-3.9.0.2/pprint36.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        7 2020-09-20 17:18:27.000000 pprint36-3.9.0.2/pprint36.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-09-20 17:18:27.000000 pprint36-3.9.0.2/pprint36.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      366 2020-09-20 17:18:27.000000 pprint36-3.9.0.2/pprint36.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-09-20 17:18:27.000000 pprint36-3.9.0.2/pprint36.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     6138 2020-09-20 17:18:27.000000 pprint36-3.9.0.2/pprint36.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      444 2020-09-20 17:18:00.000000 pprint36-3.9.0.2/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      106 2020-09-20 17:18:00.000000 pprint36-3.9.0.2/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)    13919 2020-09-20 17:18:00.000000 pprint36-3.9.0.2/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     1715 2020-09-20 17:18:00.000000 pprint36-3.9.0.2/__pkginfo__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6138 2020-09-20 17:18:27.000000 pprint36-3.9.0.2/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      144 2020-09-20 17:18:00.000000 pprint36-3.9.0.2/MANIFEST.in
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-20 17:18:27.000000 pprint36-3.9.0.2/pprint36/
--rw-rw-r--   0 travis    (2000) travis    (2000)    18657 2020-09-20 17:18:00.000000 pprint36-3.9.0.2/pprint36/_pprint.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-09-20 17:18:00.000000 pprint36-3.9.0.2/pprint36/py.typed
--rw-rw-r--   0 travis    (2000) travis    (2000)      884 2020-09-20 17:18:00.000000 pprint36-3.9.0.2/pprint36/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1547 2020-09-20 17:18:00.000000 pprint36-3.9.0.2/pprint36/_pprint.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     4515 2023-05-23 13:35:33.049271 pprint36-3.9.16.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    13919 2023-05-23 13:35:33.045271 pprint36-3.9.16.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 13:35:33.049271 pprint36-3.9.16.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     5683 2023-05-23 13:35:33.049271 pprint36-3.9.16.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2107 2023-05-23 13:35:33.049271 pprint36-3.9.16.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)    18657 2023-05-23 13:34:55.946906 pprint36-3.9.16.0/pprint36/_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1547 2023-05-23 13:34:55.946906 pprint36-3.9.16.0/pprint36/_pprint.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 13:34:55.946906 pprint36-3.9.16.0/pprint36/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      885 2023-05-23 13:34:55.946906 pprint36-3.9.16.0/pprint36/__init__.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pprint36-3.9.0.2/README.rst` & `pprint36-3.9.16.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -25,38 +25,46 @@
 .. start shields
 
 .. list-table::
 	:stub-columns: 1
 	:widths: 10 90
 
 	* - Tests
-	  - |travis| |actions_windows| |actions_macos| |coveralls| |codefactor|
+	  - |actions_linux| |actions_windows| |actions_macos| |coveralls|
 	* - PyPI
 	  - |pypi-version| |supported-versions| |supported-implementations| |wheel|
 	* - Activity
-	  - |commits-latest| |commits-since| |maintained|
+	  - |commits-latest| |commits-since| |maintained| |pypi-downloads|
+	* - QA
+	  - |codefactor| |actions_flake8| |actions_mypy|
 	* - Other
-	  - |license| |language| |requires| |pre_commit|
+	  - |license| |language| |requires|
 
+.. |actions_linux| image:: https://github.com/domdfcoding/pprint36/workflows/Linux/badge.svg
+	:target: https://github.com/domdfcoding/pprint36/actions?query=workflow%3A%22Linux%22
+	:alt: Linux Test Status
+
+.. |actions_windows| image:: https://github.com/domdfcoding/pprint36/workflows/Windows/badge.svg
+	:target: https://github.com/domdfcoding/pprint36/actions?query=workflow%3A%22Windows%22
+	:alt: Windows Test Status
+
+.. |actions_macos| image:: https://github.com/domdfcoding/pprint36/workflows/macOS/badge.svg
+	:target: https://github.com/domdfcoding/pprint36/actions?query=workflow%3A%22macOS%22
+	:alt: macOS Test Status
+
+.. |actions_flake8| image:: https://github.com/domdfcoding/pprint36/workflows/Flake8/badge.svg
+	:target: https://github.com/domdfcoding/pprint36/actions?query=workflow%3A%22Flake8%22
+	:alt: Flake8 Status
+
+.. |actions_mypy| image:: https://github.com/domdfcoding/pprint36/workflows/mypy/badge.svg
+	:target: https://github.com/domdfcoding/pprint36/actions?query=workflow%3A%22mypy%22
+	:alt: mypy status
 
-
-.. |travis| image:: https://img.shields.io/travis/com/domdfcoding/pprint36/master?logo=travis
-	:target: https://travis-ci.com/domdfcoding/pprint36
-	:alt: Travis Build Status
-
-.. |actions_windows| image:: https://github.com/domdfcoding/pprint36/workflows/Windows%20Tests/badge.svg
-	:target: https://github.com/domdfcoding/pprint36/actions?query=workflow%3A%22Windows+Tests%22
-	:alt: Windows Tests Status
-
-.. |actions_macos| image:: https://github.com/domdfcoding/pprint36/workflows/macOS%20Tests/badge.svg
-	:target: https://github.com/domdfcoding/pprint36/actions?query=workflow%3A%22macOS+Tests%22
-	:alt: macOS Tests Status
-
-.. |requires| image:: https://requires.io/github/domdfcoding/pprint36/requirements.svg?branch=master
-	:target: https://requires.io/github/domdfcoding/pprint36/requirements/?branch=master
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/domdfcoding/pprint36/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/domdfcoding/pprint36/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/domdfcoding/pprint36/master?logo=coveralls
 	:target: https://coveralls.io/github/domdfcoding/pprint36?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/domdfcoding/pprint36?logo=codefactor
@@ -82,28 +90,28 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/pprint36
 	:target: https://github.com/domdfcoding/pprint36/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/pprint36
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/pprint36/v3.9.0.2
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/pprint36/v3.9.16.0
 	:target: https://github.com/domdfcoding/pprint36/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/pprint36
 	:target: https://github.com/domdfcoding/pprint36/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2020
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
-.. |pre_commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
-	:target: https://github.com/pre-commit/pre-commit
-	:alt: pre-commit
+.. |pypi-downloads| image:: https://img.shields.io/pypi/dm/pprint36
+	:target: https://pypi.org/project/pprint36/
+	:alt: PyPI - Downloads
 
 .. end shields
 
 |
 
 Installation
 --------------
```

### Comparing `pprint36-3.9.0.2/LICENSE` & `pprint36-3.9.16.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pprint36-3.9.0.2/pprint36/_pprint.py` & `pprint36-3.9.16.0/pprint36/_pprint.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     The wrapped-object will fallback to a Py2.x style comparison for
     unorderable types (sorting first comparing the type name and then by
     the obj ids).  Does not work recursively, so dict.items() must have
     _safe_key applied to both the key and the value.
 
     """
 
-	__slots__ = ['obj']
+	__slots__ = ["obj"]
 
 	def __init__(self, obj):
 		self.obj = obj
 
 	def __lt__(self, other):
 		try:
 			return self.obj < other.obj
@@ -131,32 +131,32 @@
         sort_dicts
             If true, dict keys are sorted.
 
         """
 		indent = int(indent)
 		width = int(width)
 		if indent < 0:
-			raise ValueError('indent must be >= 0')
+			raise ValueError("indent must be >= 0")
 		if depth is not None and depth <= 0:
-			raise ValueError('depth must be > 0')
+			raise ValueError("depth must be > 0")
 		if not width:
-			raise ValueError('width must be != 0')
+			raise ValueError("width must be != 0")
 		self._depth = depth
 		self._indent_per_level = indent
 		self._width = width
 		if stream is not None:
 			self._stream = stream
 		else:
 			self._stream = _sys.stdout
 		self._compact = bool(compact)
 		self._sort_dicts = sort_dicts
 
 	def pprint(self, object):
 		self._format(object, self._stream, 0, 0, {}, 0)
-		self._stream.write("\n")
+		self._stream.write('\n')
 
 	def pformat(self, object):
 		sio = _StringIO()
 		self._format(object, sio, 0, 0, {}, 0)
 		return sio.getvalue()
 
 	def isrecursive(self, object):
@@ -223,31 +223,31 @@
 		self._format_items(object, stream, indent, allowance + 1, context, level)
 		stream.write(']')
 
 	_dispatch[list.__repr__] = _pprint_list
 
 	def _pprint_tuple(self, object, stream, indent, allowance, context, level):
 		stream.write('(')
-		endchar = ',)' if len(object) == 1 else ')'
+		endchar = ",)" if len(object) == 1 else ')'
 		self._format_items(object, stream, indent, allowance + len(endchar), context, level)
 		stream.write(endchar)
 
 	_dispatch[tuple.__repr__] = _pprint_tuple
 
 	def _pprint_set(self, object, stream, indent, allowance, context, level):
 		if not len(object):
 			stream.write(repr(object))
 			return
 		typ = object.__class__
 		if typ is set:
 			stream.write('{')
 			endchar = '}'
 		else:
-			stream.write(typ.__name__ + '({')
-			endchar = '})'
+			stream.write(typ.__name__ + "({")
+			endchar = "})"
 			indent += len(typ.__name__) + 1
 		object = sorted(object, key=_safe_key)
 		self._format_items(object, stream, indent, allowance + len(endchar), context, level)
 		stream.write(endchar)
 
 	_dispatch[set.__repr__] = _pprint_set
 	_dispatch[frozenset.__repr__] = _pprint_set
@@ -322,32 +322,32 @@
 		if parens:
 			write(')')
 
 	_dispatch[bytes.__repr__] = _pprint_bytes
 
 	def _pprint_bytearray(self, object, stream, indent, allowance, context, level):
 		write = stream.write
-		write('bytearray(')
+		write("bytearray(")
 		self._pprint_bytes(bytes(object), stream, indent + 10, allowance + 1, context, level + 1)
 		write(')')
 
 	_dispatch[bytearray.__repr__] = _pprint_bytearray
 
 	def _pprint_mappingproxy(self, object, stream, indent, allowance, context, level):
-		stream.write('mappingproxy(')
+		stream.write("mappingproxy(")
 		self._format(object.copy(), stream, indent + 13, allowance + 1, context, level)
 		stream.write(')')
 
 	_dispatch[_types.MappingProxyType.__repr__] = _pprint_mappingproxy
 
 	def _pprint_simplenamespace(self, object, stream, indent, allowance, context, level):
 		if type(object) is _types.SimpleNamespace:
 			# The SimpleNamespace repr is "namespace" instead of the class
 			# name, so we do the same here. For subclasses; use the class name.
-			cls_name = 'namespace'
+			cls_name = "namespace"
 		else:
 			cls_name = object.__class__.__name__
 		indent += len(cls_name) + 1
 		delimnl = ',\n' + ' ' * indent
 		items = object.__dict__.items()
 		last_index = len(items) - 1
 
@@ -369,15 +369,15 @@
 		indent += self._indent_per_level
 		delimnl = ',\n' + ' ' * indent
 		last_index = len(items) - 1
 		for i, (key, ent) in enumerate(items):
 			last = i == last_index
 			rep = self._repr(key, context, level)
 			write(rep)
-			write(': ')
+			write(": ")
 			self._format(ent, stream, indent + len(rep) + 2, allowance if last else 1, context, level)
 			if not last:
 				write(delimnl)
 
 	def _format_items(self, items, stream, indent, allowance, context, level):
 		write = stream.write
 		indent += self._indent_per_level
@@ -406,15 +406,15 @@
 				if width < w:
 					width = max_width
 					if delim:
 						delim = delimnl
 				if width >= w:
 					width -= w
 					write(delim)
-					delim = ', '
+					delim = ", "
 					write(rep)
 					continue
 			write(delim)
 			delim = delimnl
 			self._format(ent, stream, indent, allowance if last else 1, context, level)
 
 	def _repr(self, object, context, level):
@@ -446,20 +446,20 @@
 	_dispatch[_collections.defaultdict.__repr__] = _pprint_default_dict
 
 	def _pprint_counter(self, object, stream, indent, allowance, context, level):
 		if not len(object):
 			stream.write(repr(object))
 			return
 		cls = object.__class__
-		stream.write(cls.__name__ + '({')
+		stream.write(cls.__name__ + "({")
 		if self._indent_per_level > 1:
 			stream.write((self._indent_per_level - 1) * ' ')
 		items = object.most_common()
 		self._format_dict_items(items, stream, indent + len(cls.__name__) + 1, allowance + 2, context, level)
-		stream.write('})')
+		stream.write("})")
 
 	_dispatch[_collections.Counter.__repr__] = _pprint_counter
 
 	def _pprint_chain_map(self, object, stream, indent, allowance, context, level):
 		if not len(object.maps):
 			stream.write(repr(object))
 			return
@@ -482,15 +482,15 @@
 			return
 		cls = object.__class__
 		stream.write(cls.__name__ + '(')
 		indent += len(cls.__name__) + 1
 		stream.write('[')
 		if object.maxlen is None:
 			self._format_items(object, stream, indent, allowance + 2, context, level)
-			stream.write('])')
+			stream.write("])")
 		else:
 			self._format_items(object, stream, indent, 2, context, level)
 			rml = self._repr(object.maxlen, context, level)
 			stream.write('],\n%smaxlen=%s)' % (' ' * indent, rml))
 
 	_dispatch[_collections.deque.__repr__] = _pprint_deque
```

### Comparing `pprint36-3.9.0.2/pprint36/__init__.py` & `pprint36-3.9.16.0/pprint36/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,11 +20,11 @@
 	from pprint import *
 else:
 	from ._pprint import *
 
 __author__: str = "Python Software Foundation"
 __copyright__: str = "2001-2020 Python Software Foundation"
 __license__: str = "PSF License"
-__version__: str = "3.9.0.2"
+__version__: str = "3.9.16.0"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = ["pprint", "pformat", "isreadable", "isrecursive", "saferepr", "PrettyPrinter", "pp"]
```

### Comparing `pprint36-3.9.0.2/pprint36/_pprint.pyi` & `pprint36-3.9.16.0/pprint36/_pprint.pyi`

 * *Files identical despite different names*

