# Comparing `tmp/lazyparser-0.2.0.tar.gz` & `tmp/lazyparser-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lazyparser-0.2.0.tar", last modified: Wed Oct  9 07:40:19 2019, max compression
+gzip compressed data, was "lazyparser-0.2.1.tar", last modified: Tue May 23 14:14:31 2023, max compression
```

## Comparing `lazyparser-0.2.0.tar` & `lazyparser-0.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2019-10-09 07:40:19.000000 lazyparser-0.2.0/
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    19467 2019-10-09 07:28:24.000000 lazyparser-0.2.0/test.py
-drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2019-10-09 07:40:19.000000 lazyparser-0.2.0/doc/
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      818 2019-10-09 07:28:24.000000 lazyparser-0.2.0/doc/make.bat
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      611 2019-10-09 07:28:24.000000 lazyparser-0.2.0/doc/Makefile
-drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2019-10-09 07:40:19.000000 lazyparser-0.2.0/doc/source/
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    13416 2019-10-09 07:28:24.000000 lazyparser-0.2.0/doc/source/lazyparser.rst
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     4905 2019-10-09 07:28:24.000000 lazyparser-0.2.0/doc/source/conf.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      470 2019-10-09 07:28:24.000000 lazyparser-0.2.0/doc/source/index.rst
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      156 2019-10-09 07:28:24.000000 lazyparser-0.2.0/doc/source/license.rst
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    11299 2019-10-09 07:28:24.000000 lazyparser-0.2.0/doc/source/License.txt
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    35305 2019-10-09 07:28:24.000000 lazyparser-0.2.0/lazyparser.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)       45 2019-10-09 07:28:24.000000 lazyparser-0.2.0/.gitignore
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)       38 2019-10-09 07:40:19.000000 lazyparser-0.2.0/setup.cfg
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      325 2019-10-09 07:33:53.000000 lazyparser-0.2.0/update_notes.md
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)       22 2019-10-09 07:28:24.000000 lazyparser-0.2.0/.coveragerc
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)       77 2019-10-09 07:28:24.000000 lazyparser-0.2.0/MANIFEST.in
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     1395 2019-10-09 07:35:30.000000 lazyparser-0.2.0/README.md
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      286 2019-10-09 07:28:24.000000 lazyparser-0.2.0/LICENSE.txt
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      210 2019-10-09 07:28:24.000000 lazyparser-0.2.0/.travis.yml
-drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2019-10-09 07:40:19.000000 lazyparser-0.2.0/lazyparser.egg-info/
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      422 2019-10-09 07:40:19.000000 lazyparser-0.2.0/lazyparser.egg-info/SOURCES.txt
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)        1 2019-10-09 07:40:19.000000 lazyparser-0.2.0/lazyparser.egg-info/dependency_links.txt
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)       16 2019-10-09 07:40:19.000000 lazyparser-0.2.0/lazyparser.egg-info/requires.txt
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)       11 2019-10-09 07:40:19.000000 lazyparser-0.2.0/lazyparser.egg-info/top_level.txt
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     2333 2019-10-09 07:40:19.000000 lazyparser-0.2.0/lazyparser.egg-info/PKG-INFO
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     1016 2019-10-09 07:28:24.000000 lazyparser-0.2.0/setup.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     2333 2019-10-09 07:40:19.000000 lazyparser-0.2.0/PKG-INFO
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-05-23 14:14:31.608485 lazyparser-0.2.1/
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)       22 2019-12-12 08:26:25.000000 lazyparser-0.2.1/.coveragerc
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)       45 2019-12-12 08:26:25.000000 lazyparser-0.2.1/.gitignore
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      209 2022-04-28 15:47:22.000000 lazyparser-0.2.1/.travis.yml
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)      286 2019-12-12 08:26:25.000000 lazyparser-0.2.1/LICENSE.txt
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)       77 2019-12-12 08:26:25.000000 lazyparser-0.2.1/MANIFEST.in
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2169 2023-05-23 14:14:31.608485 lazyparser-0.2.1/PKG-INFO
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     1395 2019-12-12 08:26:25.000000 lazyparser-0.2.1/README.md
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-05-23 14:14:31.604485 lazyparser-0.2.1/doc/
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)      611 2019-12-12 08:26:25.000000 lazyparser-0.2.1/doc/Makefile
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)      818 2019-12-12 08:26:25.000000 lazyparser-0.2.1/doc/make.bat
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-05-23 14:14:31.608485 lazyparser-0.2.1/doc/source/
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)    11299 2019-12-12 08:26:25.000000 lazyparser-0.2.1/doc/source/License.txt
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     4905 2019-12-12 08:26:25.000000 lazyparser-0.2.1/doc/source/conf.py
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)      470 2019-12-12 08:26:25.000000 lazyparser-0.2.1/doc/source/index.rst
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)    13416 2019-12-12 08:26:25.000000 lazyparser-0.2.1/doc/source/lazyparser.rst
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)      156 2019-12-12 08:26:25.000000 lazyparser-0.2.1/doc/source/license.rst
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-05-23 14:14:31.608485 lazyparser-0.2.1/lazyparser.egg-info/
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     2169 2023-05-23 14:14:31.000000 lazyparser-0.2.1/lazyparser.egg-info/PKG-INFO
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)      422 2023-05-23 14:14:31.000000 lazyparser-0.2.1/lazyparser.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)        1 2023-05-23 14:14:31.000000 lazyparser-0.2.1/lazyparser.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)       16 2023-05-23 14:14:31.000000 lazyparser-0.2.1/lazyparser.egg-info/requires.txt
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)       11 2023-05-23 14:14:31.000000 lazyparser-0.2.1/lazyparser.egg-info/top_level.txt
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    35317 2022-04-28 15:50:12.000000 lazyparser-0.2.1/lazyparser.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       38 2023-05-23 14:14:31.608485 lazyparser-0.2.1/setup.cfg
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1115 2022-04-28 15:43:49.000000 lazyparser-0.2.1/setup.py
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)    19467 2019-12-12 08:26:25.000000 lazyparser-0.2.1/test.py
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)      390 2022-04-28 15:51:34.000000 lazyparser-0.2.1/update_notes.md
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `lazyparser-0.2.0/test.py` & `lazyparser-0.2.1/test.py`

 * *Files identical despite different names*

### Comparing `lazyparser-0.2.0/doc/make.bat` & `lazyparser-0.2.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `lazyparser-0.2.0/doc/Makefile` & `lazyparser-0.2.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `lazyparser-0.2.0/doc/source/lazyparser.rst` & `lazyparser-0.2.1/doc/source/lazyparser.rst`

 * *Files identical despite different names*

### Comparing `lazyparser-0.2.0/doc/source/conf.py` & `lazyparser-0.2.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `lazyparser-0.2.0/doc/source/License.txt` & `lazyparser-0.2.1/doc/source/License.txt`

 * *Files identical despite different names*

### Comparing `lazyparser-0.2.0/lazyparser.py` & `lazyparser-0.2.1/lazyparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 import sys
 import os
 import io
 import argparse
 import typing
 
 
-__version__ = '0.2.0'
+__version__ = '0.2.1'
 __all__ = ('List', 'set_env', 'set_epilog', 'set_groups', 'parse', 'flag')
 
 
 #####################################
 # sets the docstring environment
 pd1 = ":param"  # param delimiter 1
 pd2 = ":"  # param delimiter 2
@@ -673,15 +673,15 @@
 def handle_list_typing_type(arg_type):
     """
     Turn a list from the typing module into a lazyparser list.
 
     :param arg_type: (type or class instance) a type
     :return:
     """
-    if isinstance(arg_type, type(typing.List)):
+    if isinstance(arg_type, type(typing.List[typing.Any])):
         try:
             if arg_type.__name__ == 'List':  # for python 3.5
                 arg_type = List(vtype=arg_type.__args__[0])
         except AttributeError:
             if arg_type._name == "List":  # for python 3.7
                 arg_type = List(vtype=arg_type.__args__[0])
         return arg_type
```

### Comparing `lazyparser-0.2.0/README.md` & `lazyparser-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `lazyparser-0.2.0/lazyparser.egg-info/PKG-INFO` & `lazyparser-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,58 @@
 Metadata-Version: 2.1
 Name: lazyparser
-Version: 0.2.0
+Version: 0.2.1
 Summary: Lazyparser automates the parsing of arguments
 Home-page: https://github.com/NFontrodona/Lazyparser
 Author: Nicolas Fontrodona
 Author-email: nfontrodona@orange.fr
 License: Apache License 2.0
-Description: [![Build Status](https://travis-ci.com/NFontrodona/Lazyparser.svg?token=kVsLPqgGYaJqBE1Jazyp&branch=master)](https://travis-ci.com/NFontrodona/Lazyparser)
-        [![Coverage Status](https://coveralls.io/repos/github/NFontrodona/Lazyparser/badge.svg?branch=master)](https://coveralls.io/github/NFontrodona/Lazyparser?branch=master)
-        [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-        ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/lazyparser.svg)
-        
-        # Lazyparser README
-        
-        ## Description
-        
-        The lazyparser module automates the parsing of arguments. 
-        This module is based on [argparse](https://docs.python.org/3.5/library/argparse.html) developped by Steven J. Bethard.
-        
-        The lazyparser was written in ``python 3.5 `` with the version 1.4.0 of argparse.
-        It is compatible with ``python 3.5`` or higher.
-        
-        ## Documentation
-        
-        The documentation is available on <https://nfontrodona.github.io/Lazyparser/lazyparser.html>.
-        The documentation was created with sphinx (v 1.7).
-        To build the documentation, clone the project repository, go in the `doc` folder and type :
-        
-        ```sh
-        make html
-        ```
-        
-        This will create a folder `doc/build/html`. This folder will contain a file named ``index.html``. Double click on it to open the documentation with your web browser. 
-        
-        
-        ## Installation
-        
-        To install lazyparser, run :
-        
-        ```sh
-        pip install lazyparser
-        ```
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License  
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+[![Build Status](https://travis-ci.com/NFontrodona/Lazyparser.svg?token=kVsLPqgGYaJqBE1Jazyp&branch=master)](https://travis-ci.com/NFontrodona/Lazyparser)
+[![Coverage Status](https://coveralls.io/repos/github/NFontrodona/Lazyparser/badge.svg?branch=master)](https://coveralls.io/github/NFontrodona/Lazyparser?branch=master)
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/lazyparser.svg)
+
+# Lazyparser README
+
+## Description
+
+The lazyparser module automates the parsing of arguments. 
+This module is based on [argparse](https://docs.python.org/3.5/library/argparse.html) developped by Steven J. Bethard.
+
+The lazyparser was written in ``python 3.5 `` with the version 1.4.0 of argparse.
+It is compatible with ``python 3.5`` or higher.
+
+## Documentation
+
+The documentation is available on <https://nfontrodona.github.io/Lazyparser/lazyparser.html>.
+The documentation was created with sphinx (v 1.7).
+To build the documentation, clone the project repository, go in the `doc` folder and type :
+
+```sh
+make html
+```
+
+This will create a folder `doc/build/html`. This folder will contain a file named ``index.html``. Double click on it to open the documentation with your web browser. 
+
+
+## Installation
+
+To install lazyparser, run :
+
+```sh
+pip install lazyparser
+```
+
+
```

### Comparing `lazyparser-0.2.0/setup.py` & `lazyparser-0.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,12 +22,14 @@
         "argparse>=1.4.0"
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License  ",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.5",
 )
```

### Comparing `lazyparser-0.2.0/PKG-INFO` & `lazyparser-0.2.1/lazyparser.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,58 @@
 Metadata-Version: 2.1
 Name: lazyparser
-Version: 0.2.0
+Version: 0.2.1
 Summary: Lazyparser automates the parsing of arguments
 Home-page: https://github.com/NFontrodona/Lazyparser
 Author: Nicolas Fontrodona
 Author-email: nfontrodona@orange.fr
 License: Apache License 2.0
-Description: [![Build Status](https://travis-ci.com/NFontrodona/Lazyparser.svg?token=kVsLPqgGYaJqBE1Jazyp&branch=master)](https://travis-ci.com/NFontrodona/Lazyparser)
-        [![Coverage Status](https://coveralls.io/repos/github/NFontrodona/Lazyparser/badge.svg?branch=master)](https://coveralls.io/github/NFontrodona/Lazyparser?branch=master)
-        [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-        ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/lazyparser.svg)
-        
-        # Lazyparser README
-        
-        ## Description
-        
-        The lazyparser module automates the parsing of arguments. 
-        This module is based on [argparse](https://docs.python.org/3.5/library/argparse.html) developped by Steven J. Bethard.
-        
-        The lazyparser was written in ``python 3.5 `` with the version 1.4.0 of argparse.
-        It is compatible with ``python 3.5`` or higher.
-        
-        ## Documentation
-        
-        The documentation is available on <https://nfontrodona.github.io/Lazyparser/lazyparser.html>.
-        The documentation was created with sphinx (v 1.7).
-        To build the documentation, clone the project repository, go in the `doc` folder and type :
-        
-        ```sh
-        make html
-        ```
-        
-        This will create a folder `doc/build/html`. This folder will contain a file named ``index.html``. Double click on it to open the documentation with your web browser. 
-        
-        
-        ## Installation
-        
-        To install lazyparser, run :
-        
-        ```sh
-        pip install lazyparser
-        ```
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License  
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+[![Build Status](https://travis-ci.com/NFontrodona/Lazyparser.svg?token=kVsLPqgGYaJqBE1Jazyp&branch=master)](https://travis-ci.com/NFontrodona/Lazyparser)
+[![Coverage Status](https://coveralls.io/repos/github/NFontrodona/Lazyparser/badge.svg?branch=master)](https://coveralls.io/github/NFontrodona/Lazyparser?branch=master)
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/lazyparser.svg)
+
+# Lazyparser README
+
+## Description
+
+The lazyparser module automates the parsing of arguments. 
+This module is based on [argparse](https://docs.python.org/3.5/library/argparse.html) developped by Steven J. Bethard.
+
+The lazyparser was written in ``python 3.5 `` with the version 1.4.0 of argparse.
+It is compatible with ``python 3.5`` or higher.
+
+## Documentation
+
+The documentation is available on <https://nfontrodona.github.io/Lazyparser/lazyparser.html>.
+The documentation was created with sphinx (v 1.7).
+To build the documentation, clone the project repository, go in the `doc` folder and type :
+
+```sh
+make html
+```
+
+This will create a folder `doc/build/html`. This folder will contain a file named ``index.html``. Double click on it to open the documentation with your web browser. 
+
+
+## Installation
+
+To install lazyparser, run :
+
+```sh
+pip install lazyparser
+```
+
+
```

