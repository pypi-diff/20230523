# Comparing `tmp/unicode-name-inquiry-1.9.2.tar.gz` & `tmp/unicode-name-inquiry-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unicode-name-inquiry-1.9.2.tar", last modified: Mon May 22 16:57:55 2023, max compression
+gzip compressed data, was "unicode-name-inquiry-1.9.3.tar", last modified: Tue May 23 17:27:03 2023, max compression
```

## Comparing `unicode-name-inquiry-1.9.2.tar` & `unicode-name-inquiry-1.9.3.tar`

### file list

```diff
@@ -1,29 +1,33 @@
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-22 16:57:55.000000 unicode-name-inquiry-1.9.2/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1057 2023-05-10 23:37:19.000000 unicode-name-inquiry-1.9.2/LICENSE
--rw-rw-r--   0 kevin     (1001) dialout     (20)     5215 2023-05-22 16:57:55.000000 unicode-name-inquiry-1.9.2/PKG-INFO
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4405 2023-05-12 21:23:57.000000 unicode-name-inquiry-1.9.2/README.md
--rw-rw-r--   0 kevin     (1001) dialout     (20)     3817 2023-05-22 16:33:03.000000 unicode-name-inquiry-1.9.2/pyproject.toml
--rw-rw-r--   0 kevin     (1001) dialout     (20)       38 2023-05-22 16:57:55.000000 unicode-name-inquiry-1.9.2/setup.cfg
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-22 16:57:55.000000 unicode-name-inquiry-1.9.2/src/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2133 2023-05-21 14:51:20.000000 unicode-name-inquiry-1.9.2/src/test_uni.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-22 16:57:55.000000 unicode-name-inquiry-1.9.2/src/uc/
--rw-rw-r--   0 kevin     (1001) dialout     (20)       35 2023-05-22 16:32:11.000000 unicode-name-inquiry-1.9.2/src/uc/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1639 2023-05-22 16:30:42.000000 unicode-name-inquiry-1.9.2/src/uc/block.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-22 16:57:55.000000 unicode-name-inquiry-1.9.2/src/uc/data/
--rw-rw-r--   0 kevin     (1001) dialout     (20)       58 2023-05-22 16:32:46.000000 unicode-name-inquiry-1.9.2/src/uc/data/__init__.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)    18613 2023-05-21 14:25:06.000000 unicode-name-inquiry-1.9.2/src/uc/data/block.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1066 2023-05-12 21:23:57.000000 unicode-name-inquiry-1.9.2/src/uc/data/ccc.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1488 2023-05-22 16:31:01.000000 unicode-name-inquiry-1.9.2/src/uc/format.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     2263 2023-05-21 17:34:53.000000 unicode-name-inquiry-1.9.2/src/uc/search.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1426 2023-05-21 17:53:23.000000 unicode-name-inquiry-1.9.2/src/uc/test_block.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     3461 2023-05-21 17:50:43.000000 unicode-name-inquiry-1.9.2/src/uc/test_format.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     1448 2023-05-21 17:51:19.000000 unicode-name-inquiry-1.9.2/src/uc/test_search.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     5128 2023-05-22 15:28:23.000000 unicode-name-inquiry-1.9.2/src/uc/test_uni.py
--rw-rw-r--   0 kevin     (1001) dialout     (20)     4864 2023-05-22 16:31:27.000000 unicode-name-inquiry-1.9.2/src/uc/uni.py
--rwxrwxr-x   0 kevin     (1001) dialout     (20)     7043 2023-05-22 16:31:43.000000 unicode-name-inquiry-1.9.2/src/uni.py
-drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-22 16:57:55.000000 unicode-name-inquiry-1.9.2/src/unicode_name_inquiry.egg-info/
--rw-rw-r--   0 kevin     (1001) dialout     (20)     5215 2023-05-22 16:57:54.000000 unicode-name-inquiry-1.9.2/src/unicode_name_inquiry.egg-info/PKG-INFO
--rw-rw-r--   0 kevin     (1001) dialout     (20)      533 2023-05-22 16:57:54.000000 unicode-name-inquiry-1.9.2/src/unicode_name_inquiry.egg-info/SOURCES.txt
--rw-rw-r--   0 kevin     (1001) dialout     (20)        1 2023-05-22 16:57:54.000000 unicode-name-inquiry-1.9.2/src/unicode_name_inquiry.egg-info/dependency_links.txt
--rw-rw-r--   0 kevin     (1001) dialout     (20)       33 2023-05-22 16:57:54.000000 unicode-name-inquiry-1.9.2/src/unicode_name_inquiry.egg-info/entry_points.txt
--rw-rw-r--   0 kevin     (1001) dialout     (20)       16 2023-05-22 16:57:54.000000 unicode-name-inquiry-1.9.2/src/unicode_name_inquiry.egg-info/top_level.txt
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-23 17:27:03.000000 unicode-name-inquiry-1.9.3/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1057 2023-05-10 23:37:19.000000 unicode-name-inquiry-1.9.3/LICENSE
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     5641 2023-05-23 17:27:03.000000 unicode-name-inquiry-1.9.3/PKG-INFO
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4831 2023-05-23 17:22:46.000000 unicode-name-inquiry-1.9.3/README.md
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     3855 2023-05-23 17:24:33.000000 unicode-name-inquiry-1.9.3/pyproject.toml
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       38 2023-05-23 17:27:03.000000 unicode-name-inquiry-1.9.3/setup.cfg
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-23 17:27:03.000000 unicode-name-inquiry-1.9.3/src/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2610 2023-05-23 17:15:05.000000 unicode-name-inquiry-1.9.3/src/test_uni.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-23 17:27:03.000000 unicode-name-inquiry-1.9.3/src/uc/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       35 2023-05-22 16:32:11.000000 unicode-name-inquiry-1.9.3/src/uc/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1639 2023-05-22 16:30:42.000000 unicode-name-inquiry-1.9.3/src/uc/block.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-23 17:27:03.000000 unicode-name-inquiry-1.9.3/src/uc/data/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       58 2023-05-22 16:32:46.000000 unicode-name-inquiry-1.9.3/src/uc/data/__init__.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)    18613 2023-05-21 14:25:06.000000 unicode-name-inquiry-1.9.3/src/uc/data/block.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1066 2023-05-12 21:23:57.000000 unicode-name-inquiry-1.9.3/src/uc/data/ccc.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)    28591 2023-05-23 16:43:35.000000 unicode-name-inquiry-1.9.3/src/uc/data/html_entities.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2390 2023-05-23 16:46:43.000000 unicode-name-inquiry-1.9.3/src/uc/data/make_html_entities.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1488 2023-05-22 16:31:01.000000 unicode-name-inquiry-1.9.3/src/uc/format.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      672 2023-05-23 16:48:32.000000 unicode-name-inquiry-1.9.3/src/uc/html.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     2591 2023-05-23 16:53:21.000000 unicode-name-inquiry-1.9.3/src/uc/search.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1426 2023-05-21 17:53:23.000000 unicode-name-inquiry-1.9.3/src/uc/test_block.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     3563 2023-05-23 16:25:03.000000 unicode-name-inquiry-1.9.3/src/uc/test_format.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1159 2023-05-23 17:24:23.000000 unicode-name-inquiry-1.9.3/src/uc/test_html.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     1575 2023-05-23 16:55:13.000000 unicode-name-inquiry-1.9.3/src/uc/test_search.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     5233 2023-05-23 16:25:11.000000 unicode-name-inquiry-1.9.3/src/uc/test_uni.py
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     4977 2023-05-23 16:19:11.000000 unicode-name-inquiry-1.9.3/src/uc/uni.py
+-rwxrwxr-x   0 kevin     (1001) dialout     (20)     7705 2023-05-23 17:11:20.000000 unicode-name-inquiry-1.9.3/src/uni.py
+drwxrwxr-x   0 kevin     (1001) dialout     (20)        0 2023-05-23 17:27:03.000000 unicode-name-inquiry-1.9.3/src/unicode_name_inquiry.egg-info/
+-rw-rw-r--   0 kevin     (1001) dialout     (20)     5641 2023-05-23 17:27:03.000000 unicode-name-inquiry-1.9.3/src/unicode_name_inquiry.egg-info/PKG-INFO
+-rw-rw-r--   0 kevin     (1001) dialout     (20)      631 2023-05-23 17:27:03.000000 unicode-name-inquiry-1.9.3/src/unicode_name_inquiry.egg-info/SOURCES.txt
+-rw-rw-r--   0 kevin     (1001) dialout     (20)        1 2023-05-23 17:27:03.000000 unicode-name-inquiry-1.9.3/src/unicode_name_inquiry.egg-info/dependency_links.txt
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       33 2023-05-23 17:27:03.000000 unicode-name-inquiry-1.9.3/src/unicode_name_inquiry.egg-info/entry_points.txt
+-rw-rw-r--   0 kevin     (1001) dialout     (20)       16 2023-05-23 17:27:03.000000 unicode-name-inquiry-1.9.3/src/unicode_name_inquiry.egg-info/top_level.txt
```

### Comparing `unicode-name-inquiry-1.9.2/LICENSE` & `unicode-name-inquiry-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unicode-name-inquiry-1.9.2/PKG-INFO` & `unicode-name-inquiry-1.9.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicode-name-inquiry
-Version: 1.9.2
+Version: 1.9.3
 Summary: Command-line tool to display Unicode character information
 License: MIT License
 Project-URL: repository, https://codeberg.org/datatravelandexperiments/uni
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
@@ -49,19 +49,31 @@
 character names.
 
 #### `--glob`, `-g`
 
 The _character_ arguments are shell-style patterns, matched against character
 names.
 
+#### `--html`, `-H`
+
+The _character_ arguments are HTML entity names.
+Surrounding the name with `&` and `;` is optional.
+
 #### `--match`, `-m`
 
 The _character_ arguments are text that can match anywhere in a character
 name.
 
+#### `--string`, `-S`
+
+The _character_ arguments are treated as sequences of individual characters.
+For example, if the argument is `tilde`, instead of reporting the single
+character `~`, the result will be the five characters `t`, `i`, `l`, `d`,
+and `e`.
+
 #### `--word`, `-w`
 
 The _character_ arguments are full words that must appear in a character name.
 
 ### BLOCK MATCH OPTION
 
 #### `--block=`_block_, `-b` _block_
@@ -112,15 +124,16 @@
 - `{category}` - the character's category.
 - `{char}` - the character.
 - `{combining}` - the character's combining value.
 - `{decimal}` - the character's decimal value.
 - `{decomposition}` - the character's decomposition.
 - `{digit}` - the character's digit value.
 - `{eol}` - the end-of-line character (newline unless changed by command-line options).
-- `{id}` - the character name with blanks and hyphends replaced by ‘`_`’.
+- `{html}` - the HTML entity name for the character.
+- `{id}` - the character name with blanks and hyphends replaced by `_`.
 - `{mirrored}` - whether the character is mirrored in bidirectional text.
 - `{name}` - the character's name.
 - `{nfc}` - the NFC normalization form, as character names.
 - `{NFC}` - the NFC normalization form.
 - `{nfd}` - the NFD normalization form, as character names.
 - `{NFD}` - the NFD normalization form.
 - `{nfkc}` - the NFKC normalization form, as character names.
```

### Comparing `unicode-name-inquiry-1.9.2/README.md` & `unicode-name-inquiry-1.9.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -28,19 +28,31 @@
 character names.
 
 #### `--glob`, `-g`
 
 The _character_ arguments are shell-style patterns, matched against character
 names.
 
+#### `--html`, `-H`
+
+The _character_ arguments are HTML entity names.
+Surrounding the name with `&` and `;` is optional.
+
 #### `--match`, `-m`
 
 The _character_ arguments are text that can match anywhere in a character
 name.
 
+#### `--string`, `-S`
+
+The _character_ arguments are treated as sequences of individual characters.
+For example, if the argument is `tilde`, instead of reporting the single
+character `~`, the result will be the five characters `t`, `i`, `l`, `d`,
+and `e`.
+
 #### `--word`, `-w`
 
 The _character_ arguments are full words that must appear in a character name.
 
 ### BLOCK MATCH OPTION
 
 #### `--block=`_block_, `-b` _block_
@@ -91,15 +103,16 @@
 - `{category}` - the character's category.
 - `{char}` - the character.
 - `{combining}` - the character's combining value.
 - `{decimal}` - the character's decimal value.
 - `{decomposition}` - the character's decomposition.
 - `{digit}` - the character's digit value.
 - `{eol}` - the end-of-line character (newline unless changed by command-line options).
-- `{id}` - the character name with blanks and hyphends replaced by ‘`_`’.
+- `{html}` - the HTML entity name for the character.
+- `{id}` - the character name with blanks and hyphends replaced by `_`.
 - `{mirrored}` - whether the character is mirrored in bidirectional text.
 - `{name}` - the character's name.
 - `{nfc}` - the NFC normalization form, as character names.
 - `{NFC}` - the NFC normalization form.
 - `{nfd}` - the NFD normalization form, as character names.
 - `{NFD}` - the NFD normalization form.
 - `{nfkc}` - the NFKC normalization form, as character names.
```

### Comparing `unicode-name-inquiry-1.9.2/pyproject.toml` & `unicode-name-inquiry-1.9.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "unicode-name-inquiry"
-version = "1.9.2"
+version = "1.9.3"
 description = "Command-line tool to display Unicode character information"
 license.text = "MIT License"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
@@ -120,14 +120,17 @@
 lines-between-types = 1
 
 [tool.ruff.per-file-ignores]
 "test_*.py" = [
     "ANN001", "ANN201",  # test typing tbd
     "S101",     # assert
 ]
+"html_entities.py" = [
+    "RUF001"
+]
 
 [tool.yapf]
 based_on_style = "pep8"
 allow_multiline_lambdas = true
 allow_multiline_dictionary_keys = true
 blank_lines_around_top_level_definition = 1
 blank_lines_between_top_level_imports_and_variables = 1
```

### Comparing `unicode-name-inquiry-1.9.2/src/uc/block.py` & `unicode-name-inquiry-1.9.3/src/uc/block.py`

 * *Files identical despite different names*

### Comparing `unicode-name-inquiry-1.9.2/src/uc/data/block.py` & `unicode-name-inquiry-1.9.3/src/uc/data/block.py`

 * *Files identical despite different names*

### Comparing `unicode-name-inquiry-1.9.2/src/uc/data/ccc.py` & `unicode-name-inquiry-1.9.3/src/uc/data/ccc.py`

 * *Files identical despite different names*

### Comparing `unicode-name-inquiry-1.9.2/src/uc/format.py` & `unicode-name-inquiry-1.9.3/src/uc/format.py`

 * *Files identical despite different names*

### Comparing `unicode-name-inquiry-1.9.2/src/uc/search.py` & `unicode-name-inquiry-1.9.3/src/uc/search.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import fnmatch
 import re
 import unicodedata
 
 from collections.abc import Callable, Iterable
 from typing import Any
 
+import uc.html
 import uc.uni
 
 # Name searches.
 
 NameSearch = Callable[
     [Iterable[str], Iterable[str], Callable[[Iterable], bool]], Iterable[str]]
 
@@ -55,20 +56,30 @@
         x.search(unicodedata.name(c, '')) for x in search))
 
 def search_glob(select: Iterable[str],
                 source: Iterable[str],
                 fold: Fold = all) -> Iterable[str]:
     return search_egrep((fnmatch.translate(x) for x in select), source, fold)
 
+def search_html(select: Iterable[str],
+                source: Iterable[str],
+                _fold: Fold = all) -> Iterable[str]:
+    r: list[str] = []
+    for s in select:
+        if (ec := uc.html.entity_to_characters(s)):
+            r += ec
+    return (c for c in source if c in r)
+
 __NAME_SEARCH = {
     'exact': search_exact,
     'match': search_match,
     'word': search_word,
     'egrep': search_egrep,
     'glob': search_glob,
+    'html': search_html,
 }
 
 def search_name(mode: str,
                 select: Iterable[str],
                 source: Iterable[str],
                 fold: Fold = all) -> Iterable[str]:
     if mode in __NAME_SEARCH:
```

### Comparing `unicode-name-inquiry-1.9.2/src/uc/test_block.py` & `unicode-name-inquiry-1.9.3/src/uc/test_block.py`

 * *Files identical despite different names*

### Comparing `unicode-name-inquiry-1.9.2/src/uc/test_format.py` & `unicode-name-inquiry-1.9.3/src/uc/test_format.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: MIT
-"""Test code.format."""
+"""Test uc.format."""
 
 import pytest
 
 from uc.format import UniFormat
 
 # yapf: disable
 FORMAT_CASES: list[tuple[str, str, str]] = [
@@ -59,14 +59,16 @@
      'LATIN CAPITAL LETTER D, LATIN CAPITAL LETTER Z WITH CARON'),
     ('\u00C0',      'NFD',              'A\u0300'),
     ('\u00C0',      'nfd',
      'LATIN CAPITAL LETTER A, COMBINING GRAVE ACCENT'),
     ('\u01C4',      'NFKD',             'DZ\u030C'),
     ('\u01C4',      'nfkd',
      'LATIN CAPITAL LETTER D, LATIN CAPITAL LETTER Z, COMBINING CARON'),
+    ('B',           'html',             '&#0042;'),
+    ('\u00FE',      'html',             '&thorn;'),
 ]
 # yapf: enable
 
 @pytest.mark.parametrize(('character', 'key', 'result'), FORMAT_CASES)
 def test_uni_format_init(character, key, result):
     u = UniFormat(character)
     assert u[key] == result
```

### Comparing `unicode-name-inquiry-1.9.2/src/uc/test_search.py` & `unicode-name-inquiry-1.9.3/src/uc/test_search.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: MIT
-"""Test code.search."""
+"""Test uc.search."""
 
 import sys
 
 from collections.abc import Generator
 
 import pytest
 
@@ -15,32 +15,36 @@
 def chars(lo: int = 0,
           hi: int = sys.maxunicode + 1) -> Generator[str, None, None]:
     return (chr(i) for i in range(lo, hi))
 
 def test_search_name_exact():
     r = search_name('exact', ['8', 'Digit nine', '\uABCD', 'fail'],
                     chars(0, 0x7F))
-    assert list(r) == list('89')
+    assert set(r) == set('89')
 
 def test_search_name_match():
     r = search_name('match', ['it ni', 'dig'], chars(0, 0x7F))
     s = search_name('match', ['it ni', 'dig'], chars(0, 0x7F), any)
-    assert list(r) == list('9')
-    assert list(s) == list('0123456789')
+    assert set(r) == set('9')
+    assert set(s) == set('0123456789')
 
 def test_search_name_word():
     r = search_name('word', ['nine', 'digit'], chars(0, 0x7F))
     s = search_name('word', ['nine', 'digit'], chars(0, 0x7F), any)
-    assert list(r) == list('9')
-    assert list(s) == list('0123456789')
+    assert set(r) == set('9')
+    assert set(s) == set('0123456789')
 
 def test_search_name_egrep():
     r = search_name('egrep', ['c[eio][lmn]'], chars(0, 0x7F))
-    assert list(r) == list('%,:;@^`')
+    assert set(r) == set('%,:;@^`')
 
 def test_search_name_glob():
     r = search_name('glob', ['c[eo]*n'], chars(0, 0x7F))
-    assert list(r) == list('%:;')
+    assert set(r) == set('%:;')
+
+def test_search_name_html():
+    r = search_name('html', ['&thorn;', 'THORN', '¬anentity'], chars(0, 0xFF))
+    assert set(r) == set('þÞ')
 
 def test_search_name_bad():
     with pytest.raises(ValueError, match='Unknown'):
         _ = search_name('bad', ['c[eo]*n'], chars(0, 0x7F))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `unicode-name-inquiry-1.9.2/src/uc/test_uni.py` & `unicode-name-inquiry-1.9.3/src/uc/test_uni.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: MIT
-"""Test code.block."""
+"""Test uc.uni."""
 
 from typing import Any
 
 import pytest
 
 import uc.data.ccc
 import uc.uni
@@ -61,14 +61,18 @@
     assert uc.uni.digit('\U0001D7DB') == 3
     assert uc.uni.digit('\U00002464') == 5  # CIRCLED DIGIT FIVE
 
 def test_uni_hexadecimal():
     assert uc.uni.hexadecimal('\u00E2') == '00E2'
     assert uc.uni.hexadecimal('\U0001D53B') == '1D53B'
 
+def test_uni_html():
+    assert uc.uni.html('B') == '&#0042;'
+    assert uc.uni.html('\u00FE') == '&thorn;'
+
 def test_uni_identifier():
     assert (uc.uni.identifier('\U0001D53C') ==
             'MATHEMATICAL_DOUBLE_STRUCK_CAPITAL_E')
     assert uc.uni.identifier('\U00101234', 'Default') == 'Default'
 
 def test_uni_east_asian_width():
     assert uc.uni.east_asian_width('B') == 'Na'
```

### Comparing `unicode-name-inquiry-1.9.2/src/uc/uni.py` & `unicode-name-inquiry-1.9.3/src/uc/uni.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import unicodedata
 
 from collections.abc import Callable, Sequence
 from typing import Any, TypeVar
 
 import uc.block
+import uc.html
 
 T = TypeVar('T')
 
 # Conversion
 
 def unichr(value: int | str) -> str:
     """Convert an integer, character, or Unicode name to character."""
@@ -131,14 +132,18 @@
     return width(c)
 
 @register(PROPERTIES)
 def hexadecimal(c: str, _=None, digits: int = 4) -> str:
     return f'{ord(c):0{digits}X}'
 
 @register(PROPERTIES)
+def html(c: str, _=None) -> str:
+    return uc.html.character_to_entity(c)
+
+@register(PROPERTIES)
 def identifier(c: str, default: T | None = None) -> str | T | None:
     try:
         return unicodedata.name(c).replace(' ', '_').replace('-', '_')
     except ValueError:
         return default
 
 @register(PROPERTIES)
```

### Comparing `unicode-name-inquiry-1.9.2/src/uni.py` & `unicode-name-inquiry-1.9.3/src/uni.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,17 +59,20 @@
               'Mirrored   {mirrored}{eol}'
               'Decomp     {DECOMPOSITION!s:16} {decomposition}{eol}'
               'NFC        {NFC:16} {nfc}{eol}'
               'NFKC       {NFKC:16} {nfkc}{eol}'
               'NFD        {NFD:16} {nfd}{eol}'
               'NFKD       {NFKD:16} {nfkd}{eol}'
               'UTF-8      {UTF8!s:16} {utf8}{eol}'
-              'UTF-16     {UTF16!s:16} {utf16}{eol}')),
+              'UTF-16     {UTF16!s:16} {utf16}{eol}'
+              'HTML       {html}'
+              )),
     'compose': ('print for XCompose', ': "{char}"   U{x} # {name}'),
 }
+CANNED_FORMATS['full'] = CANNED_FORMATS['long']
 
 PROPS = (
     'bidi',
     'category',
     'combining',
     'decimal',
     'decomposition',
@@ -85,15 +88,15 @@
 
     global SELF  # noqa: PLW0603
     SELF = pathlib.Path(argv[0]).stem
     global error_count  # noqa: PLW0603
     error_count = 0
 
     parser = argparse.ArgumentParser(prog=SELF)
-    search_group = parser.add_argument_group('search options')
+    search_group = parser.add_argument_group('lookup options')
     anyall = search_group.add_mutually_exclusive_group()
     anyall.add_argument(
         '--all',
         help='require all conditions',
         action='store_const',
         dest='fold',
         const=all,
@@ -118,27 +121,41 @@
         '--glob',
         '-g',
         help='search names using shell glob patterns',
         action='store_const',
         dest='search',
         const='glob')
     search.add_argument(
+        '--html',
+        '-H',
+        help='look up HTML entities',
+        action='store_const',
+        dest='search',
+        const='html')
+    search.add_argument(
         '--match',
         '-m',
         help='search names using text anywhere',
         action='store_const',
         dest='search',
         const='match')
     search.add_argument(
         '--word',
         '-w',
         help='search names using full words',
         action='store_const',
         dest='search',
         const='word')
+    search.add_argument(
+        '--string',
+        '-S',
+        help='treat arguments as sequences of individual characters',
+        action='store_const',
+        dest='search',
+        const='string')
 
     prop_group = parser.add_argument_group('property match options')
     prop_group.add_argument(
         '--block',
         '-b',
         action='append',
         help='limit to the given Unicode block')
@@ -194,19 +211,24 @@
             except ValueError as e:
                 error(e)
                 return error_count
 
     # Find matching characters.
     chrs: Iterable[str]
     if args.character:
-        if args.search:
+        if args.search and args.search != 'string':
             chrs = uc.search.search_name(args.search, args.character,
                                          unicode_chars(blocks), args.fold)
         else:
-            cc = (unichr_e(name) for name in args.character)
+            if args.search == 'string':
+                cc = []
+                for name in args.character:
+                    cc += name
+            else:
+                cc = (unichr_e(name) for name in args.character)
             chrs = (
                 c for c in cc
                 if c and (any(c in b for b in blocks) if blocks else True))
     elif blocks:
         chrs = unicode_chars(blocks)
     elif props:
         chrs = unicode_chars()
```

### Comparing `unicode-name-inquiry-1.9.2/src/unicode_name_inquiry.egg-info/PKG-INFO` & `unicode-name-inquiry-1.9.3/src/unicode_name_inquiry.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicode-name-inquiry
-Version: 1.9.2
+Version: 1.9.3
 Summary: Command-line tool to display Unicode character information
 License: MIT License
 Project-URL: repository, https://codeberg.org/datatravelandexperiments/uni
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
@@ -49,19 +49,31 @@
 character names.
 
 #### `--glob`, `-g`
 
 The _character_ arguments are shell-style patterns, matched against character
 names.
 
+#### `--html`, `-H`
+
+The _character_ arguments are HTML entity names.
+Surrounding the name with `&` and `;` is optional.
+
 #### `--match`, `-m`
 
 The _character_ arguments are text that can match anywhere in a character
 name.
 
+#### `--string`, `-S`
+
+The _character_ arguments are treated as sequences of individual characters.
+For example, if the argument is `tilde`, instead of reporting the single
+character `~`, the result will be the five characters `t`, `i`, `l`, `d`,
+and `e`.
+
 #### `--word`, `-w`
 
 The _character_ arguments are full words that must appear in a character name.
 
 ### BLOCK MATCH OPTION
 
 #### `--block=`_block_, `-b` _block_
@@ -112,15 +124,16 @@
 - `{category}` - the character's category.
 - `{char}` - the character.
 - `{combining}` - the character's combining value.
 - `{decimal}` - the character's decimal value.
 - `{decomposition}` - the character's decomposition.
 - `{digit}` - the character's digit value.
 - `{eol}` - the end-of-line character (newline unless changed by command-line options).
-- `{id}` - the character name with blanks and hyphends replaced by ‘`_`’.
+- `{html}` - the HTML entity name for the character.
+- `{id}` - the character name with blanks and hyphends replaced by `_`.
 - `{mirrored}` - whether the character is mirrored in bidirectional text.
 - `{name}` - the character's name.
 - `{nfc}` - the NFC normalization form, as character names.
 - `{NFC}` - the NFC normalization form.
 - `{nfd}` - the NFD normalization form, as character names.
 - `{NFD}` - the NFD normalization form.
 - `{nfkc}` - the NFKC normalization form, as character names.
```

