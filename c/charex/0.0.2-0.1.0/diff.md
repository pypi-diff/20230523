# Comparing `tmp/charex-0.0.2.tar.gz` & `tmp/charex-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charex-0.0.2.tar", last modified: Thu May 18 15:18:28 2023, max compression
+gzip compressed data, was "charex-0.1.0.tar", last modified: Tue May 23 13:08:01 2023, max compression
```

## Comparing `charex-0.0.2.tar` & `charex-0.1.0.tar`

### file list

```diff
@@ -1,53 +1,55 @@
-drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-18 15:18:28.977571 charex-0.0.2/
--rw-r--r--   0 pji        (501) staff       (20)     1069 2023-04-20 18:29:08.000000 charex-0.0.2/LICENSE
--rw-r--r--   0 pji        (501) staff       (20)       38 2023-05-17 17:45:10.000000 charex-0.0.2/MANIFEST.in
--rw-r--r--   0 pji        (501) staff       (20)     3113 2023-05-18 15:18:28.977714 charex-0.0.2/PKG-INFO
--rw-r--r--   0 pji        (501) staff       (20)     2536 2023-05-17 17:47:37.000000 charex-0.0.2/README.rst
-drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-18 15:18:28.948537 charex-0.0.2/charex/
--rw-r--r--   0 pji        (501) staff       (20)      371 2023-05-18 15:17:51.000000 charex-0.0.2/charex/__init__.py
--rw-r--r--   0 pji        (501) staff       (20)      402 2023-05-18 15:17:51.000000 charex-0.0.2/charex/__main__.py
--rw-r--r--   0 pji        (501) staff       (20)    10185 2023-05-18 15:17:51.000000 charex-0.0.2/charex/charex.py
--rw-r--r--   0 pji        (501) staff       (20)    15803 2023-05-18 15:17:51.000000 charex-0.0.2/charex/charsets.py
-drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-18 15:18:28.973271 charex-0.0.2/charex/data/
--rw-r--r--   0 pji        (501) staff       (20)    76759 2023-04-24 18:02:02.000000 charex-0.0.2/charex/data/PropertyValueAliases.txt
--rw-r--r--   0 pji        (501) staff       (20)  1897793 2023-04-28 15:11:52.000000 charex-0.0.2/charex/data/UnicodeData.txt
--rw-r--r--   0 pji        (501) staff       (20)        0 2023-04-21 22:16:00.000000 charex-0.0.2/charex/data/__init__.py
-drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-18 15:18:28.974026 charex-0.0.2/charex/data/__pycache__/
--rw-r--r--   0 pji        (501) staff       (20)      154 2023-04-25 11:55:58.000000 charex-0.0.2/charex/data/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 pji        (501) staff       (20)   145897 2023-05-11 13:10:11.000000 charex-0.0.2/charex/data/entities.json
--rw-r--r--   0 pji        (501) staff       (20)      126 2023-05-08 18:24:17.000000 charex-0.0.2/charex/data/help_xt.txt
--rw-r--r--   0 pji        (501) staff       (20)      574 2023-05-04 17:01:12.000000 charex-0.0.2/charex/data/quote.html
--rw-r--r--   0 pji        (501) staff       (20)      573 2023-05-05 11:29:50.000000 charex-0.0.2/charex/data/result.html
--rw-r--r--   0 pji        (501) staff       (20)    99273 2023-05-17 16:34:15.000000 charex-0.0.2/charex/data/rev_casefold.json
--rw-r--r--   0 pji        (501) staff       (20)   685484 2023-05-17 16:25:24.000000 charex-0.0.2/charex/data/rev_nfc.json
--rw-r--r--   0 pji        (501) staff       (20)   676626 2023-05-17 16:28:18.000000 charex-0.0.2/charex/data/rev_nfd.json
--rw-r--r--   0 pji        (501) staff       (20)   802292 2023-05-17 16:29:56.000000 charex-0.0.2/charex/data/rev_nfkc.json
--rw-r--r--   0 pji        (501) staff       (20)   793983 2023-05-17 16:28:34.000000 charex-0.0.2/charex/data/rev_nfkd.json
--rw-r--r--   0 pji        (501) staff       (20)      391 2023-05-11 13:19:35.000000 charex-0.0.2/charex/data/sources.json
--rw-r--r--   0 pji        (501) staff       (20)     5028 2023-05-18 15:17:51.000000 charex-0.0.2/charex/denormal.py
--rw-r--r--   0 pji        (501) staff       (20)    15455 2023-05-18 15:17:51.000000 charex-0.0.2/charex/escape.py
--rw-r--r--   0 pji        (501) staff       (20)     2883 2023-05-18 15:17:51.000000 charex-0.0.2/charex/http.py
--rw-r--r--   0 pji        (501) staff       (20)     5064 2023-05-18 15:17:51.000000 charex-0.0.2/charex/normal.py
--rw-r--r--   0 pji        (501) staff       (20)    23246 2023-05-18 15:17:51.000000 charex-0.0.2/charex/shell.py
-drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-18 15:18:28.944031 charex-0.0.2/charex/static/
-drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-18 15:18:28.974650 charex-0.0.2/charex/static/styles/
--rw-r--r--   0 pji        (501) staff       (20)      455 2023-05-05 11:30:23.000000 charex-0.0.2/charex/static/styles/styles.css
--rw-r--r--   0 pji        (501) staff       (20)     4561 2023-05-18 15:17:51.000000 charex-0.0.2/charex/util.py
-drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-18 15:18:28.950382 charex-0.0.2/charex.egg-info/
--rw-r--r--   0 pji        (501) staff       (20)     3113 2023-05-18 15:18:28.000000 charex-0.0.2/charex.egg-info/PKG-INFO
--rw-r--r--   0 pji        (501) staff       (20)     1003 2023-05-18 15:18:28.000000 charex-0.0.2/charex.egg-info/SOURCES.txt
--rw-r--r--   0 pji        (501) staff       (20)        1 2023-05-18 15:18:28.000000 charex-0.0.2/charex.egg-info/dependency_links.txt
--rw-r--r--   0 pji        (501) staff       (20)       48 2023-05-18 15:18:28.000000 charex-0.0.2/charex.egg-info/entry_points.txt
--rw-r--r--   0 pji        (501) staff       (20)        6 2023-05-18 15:18:28.000000 charex-0.0.2/charex.egg-info/requires.txt
--rw-r--r--   0 pji        (501) staff       (20)        7 2023-05-18 15:18:28.000000 charex-0.0.2/charex.egg-info/top_level.txt
--rw-r--r--   0 pji        (501) staff       (20)      895 2023-05-18 15:15:01.000000 charex-0.0.2/pyproject.toml
--rw-r--r--   0 pji        (501) staff       (20)      204 2023-05-18 15:18:28.978400 charex-0.0.2/setup.cfg
-drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-18 15:18:28.977321 charex-0.0.2/tests/
--rw-r--r--   0 pji        (501) staff       (20)     5956 2023-05-18 15:17:51.000000 charex-0.0.2/tests/test_charex.py
--rw-r--r--   0 pji        (501) staff       (20)     2489 2023-05-18 15:17:51.000000 charex-0.0.2/tests/test_charset.py
--rw-r--r--   0 pji        (501) staff       (20)     2783 2023-05-18 15:17:51.000000 charex-0.0.2/tests/test_denormal.py
--rw-r--r--   0 pji        (501) staff       (20)     8775 2023-05-18 15:17:51.000000 charex-0.0.2/tests/test_escape.py
--rw-r--r--   0 pji        (501) staff       (20)     8204 2023-05-18 15:17:51.000000 charex-0.0.2/tests/test_main.py
--rw-r--r--   0 pji        (501) staff       (20)     3274 2023-05-18 15:17:51.000000 charex-0.0.2/tests/test_normal.py
--rw-r--r--   0 pji        (501) staff       (20)     6079 2023-05-18 15:17:51.000000 charex-0.0.2/tests/test_shell.py
--rw-r--r--   0 pji        (501) staff       (20)     2377 2023-05-18 15:17:51.000000 charex-0.0.2/tests/test_utility.py
+drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-23 13:08:01.291814 charex-0.1.0/
+-rw-r--r--   0 pji        (501) staff       (20)     1069 2023-04-20 18:29:08.000000 charex-0.1.0/LICENSE
+-rw-r--r--   0 pji        (501) staff       (20)       38 2023-05-17 17:45:10.000000 charex-0.1.0/MANIFEST.in
+-rw-r--r--   0 pji        (501) staff       (20)     3814 2023-05-23 13:08:01.292041 charex-0.1.0/PKG-INFO
+-rw-r--r--   0 pji        (501) staff       (20)     3237 2023-05-23 13:06:42.000000 charex-0.1.0/README.rst
+drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-23 13:08:01.258610 charex-0.1.0/charex/
+-rw-r--r--   0 pji        (501) staff       (20)      439 2023-05-23 13:07:32.000000 charex-0.1.0/charex/__init__.py
+-rw-r--r--   0 pji        (501) staff       (20)      402 2023-05-23 13:07:32.000000 charex-0.1.0/charex/__main__.py
+-rw-r--r--   0 pji        (501) staff       (20)    10751 2023-05-23 13:07:32.000000 charex-0.1.0/charex/charex.py
+-rw-r--r--   0 pji        (501) staff       (20)    15753 2023-05-23 13:07:32.000000 charex-0.1.0/charex/charsets.py
+-rw-r--r--   0 pji        (501) staff       (20)     8926 2023-05-23 13:07:32.000000 charex-0.1.0/charex/cmds.py
+drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-23 13:08:01.285359 charex-0.1.0/charex/data/
+-rw-r--r--   0 pji        (501) staff       (20)    76759 2023-04-24 18:02:02.000000 charex-0.1.0/charex/data/PropertyValueAliases.txt
+-rw-r--r--   0 pji        (501) staff       (20)  1897793 2023-04-28 15:11:52.000000 charex-0.1.0/charex/data/UnicodeData.txt
+-rw-r--r--   0 pji        (501) staff       (20)        0 2023-04-21 22:16:00.000000 charex-0.1.0/charex/data/__init__.py
+drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-23 13:08:01.286667 charex-0.1.0/charex/data/__pycache__/
+-rw-r--r--   0 pji        (501) staff       (20)      154 2023-04-25 11:55:58.000000 charex-0.1.0/charex/data/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 pji        (501) staff       (20)   145897 2023-05-11 13:10:11.000000 charex-0.1.0/charex/data/entities.json
+-rw-r--r--   0 pji        (501) staff       (20)      126 2023-05-08 18:24:17.000000 charex-0.1.0/charex/data/help_xt.txt
+-rw-r--r--   0 pji        (501) staff       (20)      574 2023-05-04 17:01:12.000000 charex-0.1.0/charex/data/quote.html
+-rw-r--r--   0 pji        (501) staff       (20)      573 2023-05-05 11:29:50.000000 charex-0.1.0/charex/data/result.html
+-rw-r--r--   0 pji        (501) staff       (20)    99273 2023-05-17 16:34:15.000000 charex-0.1.0/charex/data/rev_casefold.json
+-rw-r--r--   0 pji        (501) staff       (20)   685484 2023-05-17 16:25:24.000000 charex-0.1.0/charex/data/rev_nfc.json
+-rw-r--r--   0 pji        (501) staff       (20)   676626 2023-05-17 16:28:18.000000 charex-0.1.0/charex/data/rev_nfd.json
+-rw-r--r--   0 pji        (501) staff       (20)   802292 2023-05-17 16:29:56.000000 charex-0.1.0/charex/data/rev_nfkc.json
+-rw-r--r--   0 pji        (501) staff       (20)   793983 2023-05-17 16:28:34.000000 charex-0.1.0/charex/data/rev_nfkd.json
+-rw-r--r--   0 pji        (501) staff       (20)      391 2023-05-11 13:19:35.000000 charex-0.1.0/charex/data/sources.json
+-rw-r--r--   0 pji        (501) staff       (20)     9341 2023-05-23 13:07:32.000000 charex-0.1.0/charex/denormal.py
+-rw-r--r--   0 pji        (501) staff       (20)    15455 2023-05-23 13:07:32.000000 charex-0.1.0/charex/escape.py
+-rw-r--r--   0 pji        (501) staff       (20)    14795 2023-05-23 13:07:32.000000 charex-0.1.0/charex/gui.py
+-rw-r--r--   0 pji        (501) staff       (20)     2883 2023-05-23 13:07:32.000000 charex-0.1.0/charex/http.py
+-rw-r--r--   0 pji        (501) staff       (20)     5064 2023-05-23 13:07:32.000000 charex-0.1.0/charex/normal.py
+-rw-r--r--   0 pji        (501) staff       (20)    20293 2023-05-23 13:07:32.000000 charex-0.1.0/charex/shell.py
+drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-23 13:08:01.253335 charex-0.1.0/charex/static/
+drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-23 13:08:01.287056 charex-0.1.0/charex/static/styles/
+-rw-r--r--   0 pji        (501) staff       (20)      455 2023-05-05 11:30:23.000000 charex-0.1.0/charex/static/styles/styles.css
+-rw-r--r--   0 pji        (501) staff       (20)     6431 2023-05-23 13:07:32.000000 charex-0.1.0/charex/util.py
+drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-23 13:08:01.260939 charex-0.1.0/charex.egg-info/
+-rw-r--r--   0 pji        (501) staff       (20)     3814 2023-05-23 13:08:01.000000 charex-0.1.0/charex.egg-info/PKG-INFO
+-rw-r--r--   0 pji        (501) staff       (20)     1032 2023-05-23 13:08:01.000000 charex-0.1.0/charex.egg-info/SOURCES.txt
+-rw-r--r--   0 pji        (501) staff       (20)        1 2023-05-23 13:08:01.000000 charex-0.1.0/charex.egg-info/dependency_links.txt
+-rw-r--r--   0 pji        (501) staff       (20)       48 2023-05-23 13:08:01.000000 charex-0.1.0/charex.egg-info/entry_points.txt
+-rw-r--r--   0 pji        (501) staff       (20)        6 2023-05-23 13:08:01.000000 charex-0.1.0/charex.egg-info/requires.txt
+-rw-r--r--   0 pji        (501) staff       (20)        7 2023-05-23 13:08:01.000000 charex-0.1.0/charex.egg-info/top_level.txt
+-rw-r--r--   0 pji        (501) staff       (20)      895 2023-05-23 12:57:29.000000 charex-0.1.0/pyproject.toml
+-rw-r--r--   0 pji        (501) staff       (20)      221 2023-05-23 13:08:01.292891 charex-0.1.0/setup.cfg
+drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-05-23 13:08:01.291193 charex-0.1.0/tests/
+-rw-r--r--   0 pji        (501) staff       (20)     6498 2023-05-23 13:07:32.000000 charex-0.1.0/tests/test_charex.py
+-rw-r--r--   0 pji        (501) staff       (20)     2909 2023-05-23 13:07:32.000000 charex-0.1.0/tests/test_charset.py
+-rw-r--r--   0 pji        (501) staff       (20)     2783 2023-05-23 13:07:32.000000 charex-0.1.0/tests/test_denormal.py
+-rw-r--r--   0 pji        (501) staff       (20)     8775 2023-05-23 13:07:32.000000 charex-0.1.0/tests/test_escape.py
+-rw-r--r--   0 pji        (501) staff       (20)     8113 2023-05-23 13:07:32.000000 charex-0.1.0/tests/test_main.py
+-rw-r--r--   0 pji        (501) staff       (20)     3274 2023-05-23 13:07:32.000000 charex-0.1.0/tests/test_normal.py
+-rw-r--r--   0 pji        (501) staff       (20)     5986 2023-05-23 13:07:32.000000 charex-0.1.0/tests/test_shell.py
+-rw-r--r--   0 pji        (501) staff       (20)     5410 2023-05-23 13:07:32.000000 charex-0.1.0/tests/test_utility.py
```

### Comparing `charex-0.0.2/LICENSE` & `charex-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `charex-0.0.2/PKG-INFO` & `charex-0.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: charex
-Version: 0.0.2
+Version: 0.1.0
 Summary: A unicode and character set explorer.
 Author-email: "Paul J. Iutzi" <pji@mac.com>
 Project-URL: Homepage, https://charex.readthedocs.io/en/latest/index.html#
 Project-URL: Documentation, https://charex.readthedocs.io/en/latest/index.html#
 Project-URL: Source, https://github.com/pji/charex
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -19,26 +19,47 @@
 
 `charex` is a Unicode and character set explorer for understanding
 issues with character set translation and Unicode normalization.
 
 
 Why Did I Make This?
 ====================
-I find the ambiguity of text data interesting. In memory its all ones
+I find the ambiguity of text data interesting. In memory it's all ones
 and zeros. There is nothing inherent to the data that makes `0x20` mean
 a space character, but we've mostly agreed that it does. That "mostly"
 part is what's interesting to me, and where a lot of fun problems lie.
 
 
 How Do I Use This?
 ==================
-Right now, the best way to use it is to clone the repository. Then in
-the root of the repository, run `charex` as a module.::
+It's in PyPI, so you can install it with `pip`, as long as you are
+using Python 3.11 or higher::
 
-    python -m charex
+    pip install charex
+
+`charex` has four modes of operation:
+
+*   Direct command line invocation,
+*   An interactive shell,
+*   A graphical user interface (GUI),
+*   An application programming interface (API).
+
+
+Command Line
+------------
+To get help for direct invocation from the command line::
+
+    $ charex -h
+
+
+Interactive Shell
+-----------------
+To launch the interactive shell::
+
+    $ charex
 
 That will bring you to the `charex` shell::
 
     Welcome to the charex shell.
     Press ? for a list of comands.
     
     charex>
@@ -47,50 +68,70 @@
 
     Welcome to the charex shell.
     Press ? for a list of comands.
     
     charex> ?
     The following commands are available:
 
-    * cd: Decode the given address in all codecs.
-    * ce: Encode the given character in all codecs.
-    * cl: List registered character sets.
-    * ct: Count denormalization results.
-    * dm: Build a denormalization map.
-    * dn: Perform denormalizations.
-    * dt: Display details for a code point.
-    * el: List the registered escape schemes.
-    * es: Escape a string using the given scheme.
-    * fl: List registered normalization forms.
-    * help: Display command list.
-    * nl: Perform normalizations.
-    * sh: Run in an interactive shell.
+      * cd: Decode the given address in all codecs.
+      * ce: Encode the given character in all codecs.
+      * cl: List registered character sets.
+      * clear: Clear the terminal.
+      * ct: Count denormalization results.
+      * dm: Build a denormalization map.
+      * dn: Perform denormalizations.
+      * dt: Display details for a code point.
+      * el: List the registered escape schemes.
+      * es: Escape a string using the given scheme.
+      * fl: List registered normalization forms.
+      * nl: Perform normalizations.
+      * sh: Run in an interactive shell.
 
     For help on individual commands, use "help {command}".
 
     charex>
 
 And then type `help` then a name of one of the commands to learn what
 it does::
 
     charex> help dn
-    usage: charex dn [-h] [-m MAXDEPTH] [-n NUMBER] [-r] [-s SEED]
-                     {nfc,nfd,nfkc,nfkd} base
+    usage: charex dn [-h] [-m MAXDEPTH] [-n NUMBER] [-r] [-s SEED] form base
 
     Denormalize a string.
 
     positional arguments:
-      {nfc,nfd,nfkc,nfkd}   The Unicode normalization form for the
-                            denormalization.
+      form                  The normalization form for the denormalization. Valid
+                            options are: casefold, nfc, nfd, nfkc, nfkd.
       base                  The base normalized string.
 
     options:
       -h, --help            show this help message and exit
       -m MAXDEPTH, --maxdepth MAXDEPTH
                             Maximum number of reverse normalizations to use for
                             each character.
       -n NUMBER, --number NUMBER
                             Maximum number of results to return.
       -r, --random          Randomize the denormalization.
       -s SEED, --seed SEED  Seed the randomized denormalization.
 
     charex>
+
+
+GUI
+---
+To launch the `charex` GUI::
+
+    $ charex gui
+
+
+API
+---
+To import `charex` into your Python script to get a summary of a
+Unicode character::
+
+    >>> import charex
+    >>>
+    >>>
+    >>> value = 'a'
+    >>> char = charex.Character(value)
+    >>> print(char.summarize())
+    a U+0061 (LATIN SMALL LETTER A)
```

### Comparing `charex-0.0.2/README.rst` & `charex-0.1.0/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -4,26 +4,47 @@
 
 `charex` is a Unicode and character set explorer for understanding
 issues with character set translation and Unicode normalization.
 
 
 Why Did I Make This?
 ====================
-I find the ambiguity of text data interesting. In memory its all ones
+I find the ambiguity of text data interesting. In memory it's all ones
 and zeros. There is nothing inherent to the data that makes `0x20` mean
 a space character, but we've mostly agreed that it does. That "mostly"
 part is what's interesting to me, and where a lot of fun problems lie.
 
 
 How Do I Use This?
 ==================
-Right now, the best way to use it is to clone the repository. Then in
-the root of the repository, run `charex` as a module.::
+It's in PyPI, so you can install it with `pip`, as long as you are
+using Python 3.11 or higher::
 
-    python -m charex
+    pip install charex
+
+`charex` has four modes of operation:
+
+*   Direct command line invocation,
+*   An interactive shell,
+*   A graphical user interface (GUI),
+*   An application programming interface (API).
+
+
+Command Line
+------------
+To get help for direct invocation from the command line::
+
+    $ charex -h
+
+
+Interactive Shell
+-----------------
+To launch the interactive shell::
+
+    $ charex
 
 That will bring you to the `charex` shell::
 
     Welcome to the charex shell.
     Press ? for a list of comands.
     
     charex>
@@ -32,50 +53,70 @@
 
     Welcome to the charex shell.
     Press ? for a list of comands.
     
     charex> ?
     The following commands are available:
 
-    * cd: Decode the given address in all codecs.
-    * ce: Encode the given character in all codecs.
-    * cl: List registered character sets.
-    * ct: Count denormalization results.
-    * dm: Build a denormalization map.
-    * dn: Perform denormalizations.
-    * dt: Display details for a code point.
-    * el: List the registered escape schemes.
-    * es: Escape a string using the given scheme.
-    * fl: List registered normalization forms.
-    * help: Display command list.
-    * nl: Perform normalizations.
-    * sh: Run in an interactive shell.
+      * cd: Decode the given address in all codecs.
+      * ce: Encode the given character in all codecs.
+      * cl: List registered character sets.
+      * clear: Clear the terminal.
+      * ct: Count denormalization results.
+      * dm: Build a denormalization map.
+      * dn: Perform denormalizations.
+      * dt: Display details for a code point.
+      * el: List the registered escape schemes.
+      * es: Escape a string using the given scheme.
+      * fl: List registered normalization forms.
+      * nl: Perform normalizations.
+      * sh: Run in an interactive shell.
 
     For help on individual commands, use "help {command}".
 
     charex>
 
 And then type `help` then a name of one of the commands to learn what
 it does::
 
     charex> help dn
-    usage: charex dn [-h] [-m MAXDEPTH] [-n NUMBER] [-r] [-s SEED]
-                     {nfc,nfd,nfkc,nfkd} base
+    usage: charex dn [-h] [-m MAXDEPTH] [-n NUMBER] [-r] [-s SEED] form base
 
     Denormalize a string.
 
     positional arguments:
-      {nfc,nfd,nfkc,nfkd}   The Unicode normalization form for the
-                            denormalization.
+      form                  The normalization form for the denormalization. Valid
+                            options are: casefold, nfc, nfd, nfkc, nfkd.
       base                  The base normalized string.
 
     options:
       -h, --help            show this help message and exit
       -m MAXDEPTH, --maxdepth MAXDEPTH
                             Maximum number of reverse normalizations to use for
                             each character.
       -n NUMBER, --number NUMBER
                             Maximum number of results to return.
       -r, --random          Randomize the denormalization.
       -s SEED, --seed SEED  Seed the randomized denormalization.
 
     charex>
+
+
+GUI
+---
+To launch the `charex` GUI::
+
+    $ charex gui
+
+
+API
+---
+To import `charex` into your Python script to get a summary of a
+Unicode character::
+
+    >>> import charex
+    >>>
+    >>>
+    >>> value = 'a'
+    >>> char = charex.Character(value)
+    >>> print(char.summarize())
+    a U+0061 (LATIN SMALL LETTER A)
```

### Comparing `charex-0.0.2/charex/charex.py` & `charex-0.1.0/charex/charex.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,19 +133,32 @@
     return unicodedata_cache
 
 
 # Classes.
 class Character:
     """One or more code points representing a character.
 
-    :param value: The character to gather data for.
+    :param value: The character to gather data for. See below for the
+        formats the value can be passed in.
     :return: None.
     :rtype: NoneType
+
+    Character Formats
+    =================
+    The value can be passed in a couple of different formats:
+
+    *   *Single-Character string*: The value is a :class:`str` of
+        length one.
+    *   *Hex string*: The value is a hexadecimal number between 0x00
+        and 0x10FFFF passed as a :class:`str` prefixed with "0x".
+    *   *Address string*: The value is a hexadecimal number between
+        0x00 and 0x10FFFF passed as a :class:`str` prefixed with "U+".
     """
     def __init__(self, value: str) -> None:
+        value = util.to_char(value)
         self.__value = value
         self._rev_normal_cache: dict[str, tuple[str, ...]] = {}
 
     def __repr__(self) -> str:
         return f'{self.code_point} ({self.name})'
 
     @property
```

### Comparing `charex-0.0.2/charex/charsets.py` & `charex-0.1.0/charex/charsets.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 Data and functions for working with character sets.
 """
 from collections.abc import Iterator
 from dataclasses import dataclass
 from sys import byteorder
 
+from charex import util
+
 
 # Data classes.
 @dataclass
 class CodecDetails:
     """Information for working with the specific codec.
 
     :param size: (Optional.) The number of bytes used to address
@@ -550,25 +552,26 @@
 def get_codec_description(codec: str) -> str:
     """Provide the description for the given codec."""
     info = codecs[codec]
     return info.description
 
 
 def multiencode(
-    value: str,
+    value: bytes | int | str,
     codecs_: Iterator[str]
 ) -> dict[str, bytes]:
     """Provide the address for the given character for each of the
     given character sets.
 
     :param value: The character to encode.
     :param codecs_: The codecs to encode to.
     :return: The encoded value for each character set as a :class:`dict`.
     :rtype: dict
     """
+    value = util.to_char(value)
     results = {}
     for codec in codecs_:
         try:
             results[codec] = value.encode(codec)
         except UnicodeEncodeError:
             results[codec] = b''
     return results
@@ -583,19 +586,16 @@
 
     :param value: The address to decode. This can be passed as either
         an :class:`int`, :class:`str`, or :class:`bytes`.
     :param codec_: The codecs to decode to.
     :return: The decoded value for each character set as a :class:`dict`.
     :rtype: dict
     """
-    # Coerce the given value into ints.
-    if isinstance(value, str):
-        value = int(value, 16)
-    if isinstance(value, int):
-        value = value.to_bytes((value.bit_length() + 7) // 8)
+    # Coerce the given value into bytes.
+    value = util.to_bytes(value)
 
     # Decode the value into the character sets.
     results = {}
     for codec in codecs_:
         b = value
 
         # Pad for 2 or 4 byte codecs.
```

### Comparing `charex-0.0.2/charex/data/PropertyValueAliases.txt` & `charex-0.1.0/charex/data/PropertyValueAliases.txt`

 * *Files identical despite different names*

### Comparing `charex-0.0.2/charex/data/UnicodeData.txt` & `charex-0.1.0/charex/data/UnicodeData.txt`

 * *Files identical despite different names*

### Comparing `charex-0.0.2/charex/data/entities.json` & `charex-0.1.0/charex/data/entities.json`

 * *Files identical despite different names*

### Comparing `charex-0.0.2/charex/data/quote.html` & `charex-0.1.0/charex/data/quote.html`

 * *Files identical despite different names*

### Comparing `charex-0.0.2/charex/data/result.html` & `charex-0.1.0/charex/data/result.html`

 * *Files identical despite different names*

### Comparing `charex-0.0.2/charex/data/rev_casefold.json` & `charex-0.1.0/charex/data/rev_casefold.json`

 * *Files identical despite different names*

### Comparing `charex-0.0.2/charex/data/rev_nfc.json` & `charex-0.1.0/charex/data/rev_nfc.json`

 * *Files identical despite different names*

### Comparing `charex-0.0.2/charex/data/rev_nfd.json` & `charex-0.1.0/charex/data/rev_nfd.json`

 * *Files identical despite different names*

### Comparing `charex-0.0.2/charex/data/rev_nfkc.json` & `charex-0.1.0/charex/data/rev_nfkc.json`

 * *Files identical despite different names*

### Comparing `charex-0.0.2/charex/data/rev_nfkd.json` & `charex-0.1.0/charex/data/rev_nfkd.json`

 * *Files identical despite different names*

### Comparing `charex-0.0.2/charex/escape.py` & `charex-0.1.0/charex/escape.py`

 * *Files identical despite different names*

### Comparing `charex-0.0.2/charex/http.py` & `charex-0.1.0/charex/http.py`

 * *Files identical despite different names*

### Comparing `charex-0.0.2/charex/normal.py` & `charex-0.1.0/charex/normal.py`

 * *Files identical despite different names*

### Comparing `charex-0.0.2/charex/shell.py` & `charex-0.1.0/charex/shell.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,151 +8,85 @@
 from argparse import (
     ArgumentParser,
     Namespace,
     _SubParsersAction,
     RawDescriptionHelpFormatter
 )
 from cmd import Cmd
-from itertools import zip_longest
 import readline
 from shlex import split
 from shutil import get_terminal_size
 from textwrap import wrap
 
-from charex import charex as ch
+from charex import cmds
 from charex import charsets as cset
-from charex import denormal as dn
 from charex import escape as esc
+from charex import gui
 from charex import normal as nl
-from charex import util
-
-
-# Utility functions.
-def make_description_row(name: str, namewidth: int, descr: str) -> str:
-    """Create a two column row with a name and description.
-
-    :param name: The content for the first column.
-    :param namewidth: The width of the first column.
-    :param descr: The content for the second column.
-    :return: The row as a :class:`str`.
-    :rtype: str
-    """
-    name_lines = wrap(name, namewidth)
-    descr_lines = wrap(descr, 77 - namewidth)
-    lines = (
-        f'{n:<{namewidth}}  {d}'
-        for n, d in zip_longest(name_lines, descr_lines, fillvalue='')
-    )
-    return '\n'.join(lines)
-
-
-def write_list(
-    items: Sequence[str],
-    get_descr: Callable[[str], str],
-    show_descr: bool
-) -> None:
-    """Output the given list.
-
-    :param items: The items to list.
-    :param get_descr: The function used to look up the discription
-        of each item.
-    :param show_descr: Whether include the descriptions of each item
-        in the output.
-    :return: None.
-    :rtype: NoneType
-    """
-    width = max(len(item) for item in items)
-    for item in items:
-        if show_descr:
-            descr = get_descr(item)
-            row = make_description_row(item, width, descr)
-            print(row)
-            print()
-        else:
-            print(item)
 
 
 # Running modes.
 def mode_cd(args: Namespace) -> None:
     """Decode the given address in all codecs.
 
     :param args: The arguments used when the script was invoked.
     :return: None.
     :rtype: NoneType
     """
-    # Normalize the data.
-    if args.base.startswith('0b'):
-        b = util.bin2bytes(args.base[2:])
-    elif args.base.startswith('0x'):
-        b = util.hex2bytes(args.base[2:])
-    else:
-        b = args.base.encode('utf8')
-
-    # Get the data.
-    codecs = cset.get_codecs()
-    results = cset.multidecode(b, (codec for codec in codecs))
-
-    # Write the output.
-    width = max(len(codec) for codec in codecs)
-    for key in results:
-        c = results[key]
-        details = ''
-        if len(c) < 1:
-            details = '*** no character ***'
-        elif len(c) > 1:
-            details = '*** multiple characters ***'
-        else:
-            char = ch.Character(c)
-            details = f'{char.code_point} {char.name}'
-        c = util.neutralize_control_characters(c)
-        print(f'{key:>{width}}: {c} {details}')
+    for line in cmds.cd(args.base):
+        print(line)
     print()
 
 
 def mode_ce(args: Namespace) -> None:
     """Encode the given character in all codecs.
 
     :param args: The arguments used when the script was invoked.
     :return: None.
     :rtype: NoneType
     """
-    # Get the data.
-    codecs = cset.get_codecs()
-    results = cset.multiencode(args.base, (codec for codec in codecs))
-
-    # Write the output.
-    width = max(len(codec) for codec in codecs)
-    for key in results:
-        if b := results[key]:
-            c = ''.join(f'{n:>02x}'.upper() for n in b)
-            print(f'{key:>{width}}: {c}')
+    for line in cmds.ce(args.base):
+        print(line)
     print()
 
 
 def mode_cl(args: Namespace) -> None:
     """List registered character sets.
 
     :param args: The arguments used when the script was invoked.
     :return: None.
     :rtype: NoneType
     """
-    codecs = cset.get_codecs()
-    write_list(codecs, cset.get_codec_description, args.description)
+    for line in cmds.cl(args.description):
+        print(line)
+        if args.description:
+            print()
     print()
 
 
+def mode_clear(args: Namespace) -> None:
+    """Clear the terminal.
+
+    :param args: The arguments used when the script was invoked.
+    :return: None.
+    :rtype: NoneType
+    """
+    print('\x1b[2J')
+    print('\x1b[1;1H', end='')
+
+
 def mode_ct(args: Namespace) -> None:
     """Count denormalization results.
 
     :param args: The arguments used when the script was invoked.
     :return: None.
     :rtype: NoneType
     """
-    count = dn.count_denormalizations(args.base, args.form, args.maxdepth)
-    print(f'{count:,}')
+    count = cmds.ct(args.base, args.form, args.maxdepth)
+    print(count)
     print()
 
 
 def mode_dm(args: Namespace) -> None:
     """Build a denormalization map.
 
     :param args: The arguments used when the script was invoked.
@@ -168,138 +102,98 @@
 def mode_dn(args: Namespace) -> None:
     """Perform denormalizations.
 
     :param args: The arguments used when the script was invoked.
     :return: None.
     :rtype: NoneType
     """
-    results = dn.denormalize(
+    for result in cmds.dn(
         args.base,
         args.form,
         args.maxdepth,
-        args.number,
         args.random,
         args.seed
-    )
-    for result in results:
+    ):
         print(result)
     print()
 
 
 def mode_dt(args: Namespace) -> None:
     """Display details for a code point.
 
     :param args: The arguments used when the script was invoked.
     :return: None.
     :rtype: NoneType
     """
-    def rev_normalize(char: ch.Character, form: str) -> str:
-        points = char.denormalize(form)
-        values = []
-        for point in points:
-            if len(point) == 1:
-                c = ch.Character(point)
-                values.append(c.summarize())
-            elif len(point) > 1:
-                values.append(f'{point} *** multiple characters ***')
-                for item in point:
-                    char = ch.Character(item)
-                    values.append('  ' + char.summarize())
-        if not values:
-            return ''
-        return ('\n' + ' ' * 22).join(v for v in values)
-
-    # Gather the details for display.
-    cp = args.codepoint
-    if cp.startswith('U+'):
-        cp = '0x' + cp[2:]
-    if cp.startswith('0x'):
-        n = int(cp, 16)
-        cp = chr(n)
-    char = ch.Character(cp)
-    details = (
-        ('Display', char.value),
-        ('Name', char.name),
-        ('Code Point', char.code_point),
-        ('Category', char.category),
-        ('UTF-8', char.encode('utf8')),
-        ('UTF-16', char.encode('utf_16_be')),
-        ('UTF-32', char.encode('utf_32_be')),
-        ('Decomposition', char.decomposition),
-        ('C encoded', char.escape('c')),
-        ('URL encoded', char.escape('url')),
-        ('HTML encoded', char.escape('html')),
-        ('Reverse Cfold', rev_normalize(char, 'casefold')),
-        ('Reverse NFC', rev_normalize(char, 'nfc')),
-        ('Reverse NFD', rev_normalize(char, 'nfd')),
-        ('Reverse NFKC', rev_normalize(char, 'nfkc')),
-        ('Reverse NFKD', rev_normalize(char, 'nfkd')),
-    )
-
-    # Display the details.
-    width = 20
-    for detail in details:
-        label, value = detail
-        if value:
-            print(f'{label:>{width}}: {value}')
+    for line in cmds.dt(args.codepoint):
+        print(line)
     print()
 
 
 def mode_el(args: Namespace) -> None:
     """List the registered escape schemes.
 
     :param args: The arguments used when the script was invoked.
     :return: None.
     :rtype: NoneType
     """
-    schemes = esc.get_schemes()
-    write_list(schemes, esc.get_description, args.description)
+    for line in cmds.el(args.description):
+        print(line)
+        if args.description:
+            print()
     print()
 
 
 def mode_es(args: Namespace) -> None:
     """Escape a string using the given scheme.
 
     :param args: The arguments used when the script was invoked.
     :return: None.
     :rtype: NoneType
     """
-    result = esc.escape(args.base, args.scheme, 'utf8')
+    result = cmds.es(args.base, args.scheme, 'utf8')
     print(result)
     print()
 
 
 def mode_fl(args: Namespace) -> None:
     """List registered normalization forms.
 
     :param args: The arguments used when the script was invoked.
     :return: None.
     :rtype: NoneType
     """
-    forms = nl.get_forms()
-    write_list(forms, nl.get_description, args.description)
+    for line in cmds.fl(args.description):
+        print(line)
+        if args.description:
+            print()
     print()
 
 
+def mode_gui(args: Namespace) -> None:
+    """Start the GUI.
+
+    :param args: The arguments used when the script was invoked.
+    :return: None.
+    :rtype: NoneType
+    """
+    print('Running charex GUI....')
+    gui.main()
+    print('charex GUI stopped.')
+
+
 def mode_nl(args: Namespace) -> None:
     """Perform normalizations.
 
     :param args: The arguments used when the script was invoked.
     :return: None.
     :rtype: NoneType
     """
-    result = nl.normalize(args.form, args.base)
+    result = cmds.nl(args.form, args.base, args.expand)
     print(result)
-    if args.expand:
-        for item in result:
-            char = ch.Character(item)
-            indent = '  '
-            if 'mark' in char.category.casefold():
-                indent += ' '
-            print(f'  {char.summarize()}')
     print()
 
 
 def mode_sh(args: Namespace | None) -> None:
     """Run in an interactive shell.
 
     :param args: The arguments used when the script was invoked.
@@ -329,21 +223,23 @@
         help=list_modes(),
         metavar='mode',
         required=True
     )
     parse_cd(spa)
     parse_ce(spa)
     parse_cl(spa)
+    parse_clear(spa)
     parse_ct(spa)
     parse_dm(spa)
     parse_dn(spa)
     parse_dt(spa)
     parse_el(spa)
     parse_es(spa)
     parse_fl(spa)
+    parse_gui(spa)
     parse_nl(spa)
     parse_sh(spa)
 
     return p
 
 
 def parse_cd(spa: _SubParsersAction) -> None:
@@ -358,16 +254,16 @@
         'cd',
         description='Decode the given address in all codecs.'
     )
     sp.add_argument(
         'base',
         help=(
             'The base integer. Prefix the integer with "0x" for hex '
-            'or "0b" for binary. No prefix will be interpreted as the'
-            'UTF-8 address of the character.'
+            'or "0b" for binary. No prefix or a Unicode code point '
+            'will be interpreted as the UTF-8 address of the character.'
         ),
         action='store',
         type=str
     )
     sp.set_defaults(func=mode_cd)
 
 
@@ -409,14 +305,30 @@
         '-d', '--description',
         help='Show the description for the character sets.',
         action='store_true'
     )
     sp.set_defaults(func=mode_cl)
 
 
+def parse_clear(spa: _SubParsersAction) -> None:
+    """Clear the terminal.
+
+    :param spa: The subparser action used to add a new subparser to
+        the main parser.
+    :return: None.
+    :rtype: NoneType
+    """
+    sp = spa.add_parser(
+        'clear',
+        aliases=['clr',],
+        description='Clear the terminal.'
+    )
+    sp.set_defaults(func=mode_clear)
+
+
 def parse_ct(spa: _SubParsersAction) -> None:
     """Add the ct mode subparser.
 
     :param spa: The subparser action used to add a new subparser to
         the main parser.
     :return: None.
     :rtype: NoneType
@@ -506,29 +418,23 @@
         help='The base normalized string.',
         action='store',
         type=str
     )
     sp.add_argument(
         '-m', '--maxdepth',
         help=(
-            'Maximum number of reverse normalizations to use '
-            'for each character.'
+            'If not random, sets the maximum number of denormalizations '
+            'to use for each character. If random, sets the number of '
+            'random denormalizations to return.'
         ),
         default=0,
         action='store',
         type=int
     )
     sp.add_argument(
-        '-n', '--number',
-        help='Maximum number of results to return.',
-        default=0,
-        action='store',
-        type=int
-    )
-    sp.add_argument(
         '-r', '--random',
         help='Randomize the denormalization.',
         action='store_true'
     )
     sp.add_argument(
         '-s', '--seed',
         help='Seed the randomized denormalization.',
@@ -633,14 +539,30 @@
         '-d', '--description',
         help='Show the description for the character sets.',
         action='store_true'
     )
     sp.set_defaults(func=mode_fl)
 
 
+def parse_gui(spa: _SubParsersAction) -> None:
+    """Run the GUI.
+
+    :param spa: The subparser action used to add a new subparser to
+        the main parser.
+    :return: None.
+    :rtype: NoneType
+    """
+    sp = spa.add_parser(
+        'gui',
+        aliases=[],
+        description='Run the charex GUI.'
+    )
+    sp.set_defaults(func=mode_gui)
+
+
 def parse_nl(spa: _SubParsersAction) -> None:
     """Add the nl mode subparser.
 
     :param spa: The subparser action used to add a new subparser to
         the main parser.
     :return: None.
     :rtype: NoneType
@@ -733,14 +655,19 @@
         self._run_cmd(cmd)
 
     def do_cl(self, arg):
         """List the registered character sets."""
         cmd = f'cl {arg}'
         self._run_cmd(cmd)
 
+    def do_clear(self, arg):
+        """Clear the terminal."""
+        cmd = f'clear {arg}'
+        self._run_cmd(cmd)
+
     def do_ct(self, arg):
         """Count denormalization results."""
         cmd = f'ct {arg}'
         self._run_cmd(cmd)
 
     def do_dm(self, arg):
         """Build a denormalization map."""
@@ -821,14 +748,18 @@
         cmd = f'ce -h'
         self._run_cmd(cmd)
 
     def help_cl(self):
         cmd = f'cl -h'
         self._run_cmd(cmd)
 
+    def help_clear(self):
+        cmd = f'clear -h'
+        self._run_cmd(cmd)
+
     def help_ct(self):
         """Help for the ct command."""
         cmd = f'ct -h'
         self._run_cmd(cmd)
 
     def help_dn(self):
         """Help for the dn command."""
```

### Comparing `charex-0.0.2/charex.egg-info/PKG-INFO` & `charex-0.1.0/charex.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: charex
-Version: 0.0.2
+Version: 0.1.0
 Summary: A unicode and character set explorer.
 Author-email: "Paul J. Iutzi" <pji@mac.com>
 Project-URL: Homepage, https://charex.readthedocs.io/en/latest/index.html#
 Project-URL: Documentation, https://charex.readthedocs.io/en/latest/index.html#
 Project-URL: Source, https://github.com/pji/charex
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -19,26 +19,47 @@
 
 `charex` is a Unicode and character set explorer for understanding
 issues with character set translation and Unicode normalization.
 
 
 Why Did I Make This?
 ====================
-I find the ambiguity of text data interesting. In memory its all ones
+I find the ambiguity of text data interesting. In memory it's all ones
 and zeros. There is nothing inherent to the data that makes `0x20` mean
 a space character, but we've mostly agreed that it does. That "mostly"
 part is what's interesting to me, and where a lot of fun problems lie.
 
 
 How Do I Use This?
 ==================
-Right now, the best way to use it is to clone the repository. Then in
-the root of the repository, run `charex` as a module.::
+It's in PyPI, so you can install it with `pip`, as long as you are
+using Python 3.11 or higher::
 
-    python -m charex
+    pip install charex
+
+`charex` has four modes of operation:
+
+*   Direct command line invocation,
+*   An interactive shell,
+*   A graphical user interface (GUI),
+*   An application programming interface (API).
+
+
+Command Line
+------------
+To get help for direct invocation from the command line::
+
+    $ charex -h
+
+
+Interactive Shell
+-----------------
+To launch the interactive shell::
+
+    $ charex
 
 That will bring you to the `charex` shell::
 
     Welcome to the charex shell.
     Press ? for a list of comands.
     
     charex>
@@ -47,50 +68,70 @@
 
     Welcome to the charex shell.
     Press ? for a list of comands.
     
     charex> ?
     The following commands are available:
 
-    * cd: Decode the given address in all codecs.
-    * ce: Encode the given character in all codecs.
-    * cl: List registered character sets.
-    * ct: Count denormalization results.
-    * dm: Build a denormalization map.
-    * dn: Perform denormalizations.
-    * dt: Display details for a code point.
-    * el: List the registered escape schemes.
-    * es: Escape a string using the given scheme.
-    * fl: List registered normalization forms.
-    * help: Display command list.
-    * nl: Perform normalizations.
-    * sh: Run in an interactive shell.
+      * cd: Decode the given address in all codecs.
+      * ce: Encode the given character in all codecs.
+      * cl: List registered character sets.
+      * clear: Clear the terminal.
+      * ct: Count denormalization results.
+      * dm: Build a denormalization map.
+      * dn: Perform denormalizations.
+      * dt: Display details for a code point.
+      * el: List the registered escape schemes.
+      * es: Escape a string using the given scheme.
+      * fl: List registered normalization forms.
+      * nl: Perform normalizations.
+      * sh: Run in an interactive shell.
 
     For help on individual commands, use "help {command}".
 
     charex>
 
 And then type `help` then a name of one of the commands to learn what
 it does::
 
     charex> help dn
-    usage: charex dn [-h] [-m MAXDEPTH] [-n NUMBER] [-r] [-s SEED]
-                     {nfc,nfd,nfkc,nfkd} base
+    usage: charex dn [-h] [-m MAXDEPTH] [-n NUMBER] [-r] [-s SEED] form base
 
     Denormalize a string.
 
     positional arguments:
-      {nfc,nfd,nfkc,nfkd}   The Unicode normalization form for the
-                            denormalization.
+      form                  The normalization form for the denormalization. Valid
+                            options are: casefold, nfc, nfd, nfkc, nfkd.
       base                  The base normalized string.
 
     options:
       -h, --help            show this help message and exit
       -m MAXDEPTH, --maxdepth MAXDEPTH
                             Maximum number of reverse normalizations to use for
                             each character.
       -n NUMBER, --number NUMBER
                             Maximum number of results to return.
       -r, --random          Randomize the denormalization.
       -s SEED, --seed SEED  Seed the randomized denormalization.
 
     charex>
+
+
+GUI
+---
+To launch the `charex` GUI::
+
+    $ charex gui
+
+
+API
+---
+To import `charex` into your Python script to get a summary of a
+Unicode character::
+
+    >>> import charex
+    >>>
+    >>>
+    >>> value = 'a'
+    >>> char = charex.Character(value)
+    >>> print(char.summarize())
+    a U+0061 (LATIN SMALL LETTER A)
```

### Comparing `charex-0.0.2/charex.egg-info/SOURCES.txt` & `charex-0.1.0/charex.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 README.rst
 pyproject.toml
 setup.cfg
 charex/__init__.py
 charex/__main__.py
 charex/charex.py
 charex/charsets.py
+charex/cmds.py
 charex/denormal.py
 charex/escape.py
+charex/gui.py
 charex/http.py
 charex/normal.py
 charex/shell.py
 charex/util.py
 charex.egg-info/PKG-INFO
 charex.egg-info/SOURCES.txt
 charex.egg-info/dependency_links.txt
```

### Comparing `charex-0.0.2/pyproject.toml` & `charex-0.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
 ]
 
 [project]
 name = "charex"
-version = "0.0.2"
+version = "0.1.0"
 authors = [
     {name="Paul J. Iutzi", email="pji@mac.com"},
 ]
 description = "A unicode and character set explorer."
 readme = "README.rst"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `charex-0.0.2/tests/test_charex.py` & `charex-0.1.0/tests/test_charex.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,46 @@
 """
 test_charex
 ~~~~~~~~~~~
 """
 import json
 
-import pytest
-
 from charex import charex as c
 
 
 # Test Character.
 def test_character_init():
-    """Given a string containing one or more codepoints representing
-    a character, a :class:`Character` object is initialized.
+    """Given a string containing a character, a :class:`Character`
+    object is initialized.
     """
     exp_value = 'a'
     act = c.Character(exp_value)
     assert act.value == exp_value
 
 
+def test_character_init_with_hex():
+    """Given a string containing a hexadecimal number starting with
+    "0x", a :class:`Character` object is initialized with the character
+    at that address.
+    """
+    exp_value = 'a'
+    act = c.Character('0x0061')
+    assert act.value == exp_value
+
+
+def test_character_init_with_code_point():
+    """Given a string containing a unicode code point starting with
+    "U+", a :class:`Character` object is initialized with the character
+    at that address.
+    """
+    exp_value = 'a'
+    act = c.Character('U+0061')
+    assert act.value == exp_value
+
+
 def test_character_category():
     """When called, :attr:`Character.category` returns the Unicode
     category for the character.
     """
     char = c.Character('a')
     assert char.category == 'Lowercase Letter'
```

### Comparing `charex-0.0.2/tests/test_charset.py` & `charex-0.1.0/tests/test_charset.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,65 +21,48 @@
     """
     codec = 'ascii'
     info = cs.codecs[codec]
     exp = info.description
     assert cs.get_codec_description(codec) == exp
 
 
-# Tests for multiencode.
-def test_multiencode():
-    """Given a code point and a list of character sets, return the
-    :class:`bytes` for that code point in each character set as a
-    :class:`dict`.
-    """
-    exp = {
-        'ascii': b'',
-        'cp1252': b'\x93',
-        'mac_roman': b'\xd2',
-        'utf_8': b'\xe2\x80\x9c',
-    }
-    codecs = exp.keys()
-    act = cs.multiencode('“', codecs)
-    assert exp == act
-
-
-def test_multiencode():
-    """Given an integer and a sequence of strings that reference
+# Tests for multidecode.
+def test_multidecode_bytes():
+    """Given bytes and a sequence of strings that reference
     decoding codecs, :func:`charex.charsets.multiencode` returns
     the code point for each given codec as a :class:`dict`.
     """
     exp = {
         'ascii': '',
         'cp1252': 'é',
         'iso8859_7': 'ι',
         'utf_16_be': 'é',
         'utf_16_le': 'é',
         'utf_16': 'é',
     }
     codecs = exp.keys()
-    act = cs.multidecode(0xe9, codecs)
+    act = cs.multidecode(b'\xe9', codecs)
     assert exp == act
 
 
-# Tests for multidecode.
-def test_multidecode_bytes():
-    """Given bytes and a sequence of strings that reference
+def test_multidecode_int():
+    """Given an integer and a sequence of strings that reference
     decoding codecs, :func:`charex.charsets.multiencode` returns
     the code point for each given codec as a :class:`dict`.
     """
     exp = {
         'ascii': '',
         'cp1252': 'é',
         'iso8859_7': 'ι',
         'utf_16_be': 'é',
         'utf_16_le': 'é',
         'utf_16': 'é',
     }
     codecs = exp.keys()
-    act = cs.multidecode(b'\xe9', codecs)
+    act = cs.multidecode(0xe9, codecs)
     assert exp == act
 
 
 def test_multidecode_str():
     """Given a hex string and a sequence of strings that reference
     decoding codecs, :func:`charex.charsets.multiencode` returns
     the code point for each given codec as a :class:`dict`.
@@ -89,9 +72,42 @@
         'cp1252': 'é',
         'iso8859_7': 'ι',
         'utf_16_be': 'é',
         'utf_16_le': 'é',
         'utf_16': 'é',
     }
     codecs = exp.keys()
-    act = cs.multidecode('e9', codecs)
+    act = cs.multidecode('0xe9', codecs)
+    assert exp == act
+
+
+# Tests for multiencode.
+def test_multiencode():
+    """Given a code point and a list of character sets, return the
+    :class:`bytes` for that code point in each character set as a
+    :class:`dict`.
+    """
+    exp = {
+        'ascii': b'',
+        'cp1252': b'\x93',
+        'mac_roman': b'\xd2',
+        'utf_8': b'\xe2\x80\x9c',
+    }
+    codecs = exp.keys()
+    act = cs.multiencode('“', codecs)
+    assert exp == act
+
+
+def test_multiencode_unicode():
+    """Given a code point and a list of character sets, return the
+    :class:`bytes` for that code point in each character set as a
+    :class:`dict`.
+    """
+    exp = {
+        'ascii': b'',
+        'cp1252': b'\x93',
+        'mac_roman': b'\xd2',
+        'utf_8': b'\xe2\x80\x9c',
+    }
+    codecs = exp.keys()
+    act = cs.multiencode('U+201c', codecs)
     assert exp == act
```

### Comparing `charex-0.0.2/tests/test_denormal.py` & `charex-0.1.0/tests/test_denormal.py`

 * *Files identical despite different names*

### Comparing `charex-0.0.2/tests/test_escape.py` & `charex-0.1.0/tests/test_escape.py`

 * *Files identical despite different names*

### Comparing `charex-0.0.2/tests/test_main.py` & `charex-0.1.0/tests/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,31 +187,28 @@
         'dn',
         'nfkd',
         '<->'
     )
     cli_test(exp, cmd, capsys)
 
 
-def test_dn_number(capsys):
+def test_dn_maxdepth(capsys):
     """Invoked with -n and an integer, dn mode should return no
     more than that number of results.
     """
     exp = (
         '\ufe64\ufe63\ufe65\n'
-        '\ufe64\ufe63\uff1e\n'
-        '\ufe64\uff0d\ufe65\n'
-        '\ufe64\uff0d\uff1e\n'
         '\n'
     )
     cmd = (
         'python -m charex',
         'dn',
         'nfkd',
         '<->',
-        '-n', '4'
+        '-m', '1'
     )
     cli_test(exp, cmd, capsys)
 
 
 def test_dn_random(capsys):
     """Called with -r, dn mode should return a randomly
     denormalize the string.
```

### Comparing `charex-0.0.2/tests/test_normal.py` & `charex-0.1.0/tests/test_normal.py`

 * *Files identical despite different names*

### Comparing `charex-0.0.2/tests/test_shell.py` & `charex-0.1.0/tests/test_shell.py`

 * *Files 3% similar despite different names*

```diff
@@ -120,24 +120,21 @@
 
 def test_dn_number(capsys):
     """Invoked with -n and an integer, dn mode should return no
     more than that number of results.
     """
     exp = (
         '\ufe64\ufe63\ufe65\n'
-        '\ufe64\ufe63\uff1e\n'
-        '\ufe64\uff0d\ufe65\n'
-        '\ufe64\uff0d\uff1e\n'
         '\n'
     )
     cmd = (
         'dn '
         'nfkd '
         '<-> '
-        '-n 4'
+        '-m 1'
     )
     shell_test(exp, cmd, capsys)
 
 
 def test_dn_random(capsys):
     """Called with -r, dn mode should return a randomly
     denormalize the string.
```

