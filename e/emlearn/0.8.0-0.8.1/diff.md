# Comparing `tmp/emlearn-0.8.0.tar.gz` & `tmp/emlearn-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/emlearn-0.8.0.tar", last modified: Sat Mar  2 00:29:06 2019, max compression
+gzip compressed data, was "dist/emlearn-0.8.1.tar", last modified: Wed Mar  6 19:03:24 2019, max compression
```

## Comparing `emlearn-0.8.0.tar` & `emlearn-0.8.1.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-02 00:29:06.000000 emlearn-0.8.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)       65 2019-03-02 00:27:21.000000 emlearn-0.8.0/MANIFEST.in
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-02 00:29:06.000000 emlearn-0.8.0/examples/
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2319 2019-03-02 00:27:21.000000 emlearn-0.8.0/examples/window-function.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2149 2019-03-02 00:27:21.000000 emlearn-0.8.0/examples/mel-filterbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2019-03-02 00:27:21.000000 emlearn-0.8.0/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1050 2019-03-02 00:27:21.000000 emlearn-0.8.0/LICENSE.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     3055 2019-03-02 00:29:06.000000 emlearn-0.8.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2086 2019-03-02 00:27:21.000000 emlearn-0.8.0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-02 00:29:06.000000 emlearn-0.8.0/bindings/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5123 2019-03-02 00:27:21.000000 emlearn-0.8.0/bindings/eml_audio.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4580 2019-03-02 00:27:21.000000 emlearn-0.8.0/bindings/eml_net.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1345 2019-03-02 00:27:21.000000 emlearn-0.8.0/bindings/eml_signal.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2297 2019-03-02 00:27:21.000000 emlearn-0.8.0/bindings/eml_trees.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2697 2019-03-02 00:27:21.000000 emlearn-0.8.0/bindings/eml_bayes.cpp
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-02 00:29:06.000000 emlearn-0.8.0/emlearn.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3055 2019-03-02 00:29:06.000000 emlearn-0.8.0/emlearn.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-03-02 00:29:06.000000 emlearn-0.8.0/emlearn.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       57 2019-03-02 00:29:06.000000 emlearn-0.8.0/emlearn.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-03-02 00:29:06.000000 emlearn-0.8.0/emlearn.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      943 2019-03-02 00:29:06.000000 emlearn-0.8.0/emlearn.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2019-03-02 00:29:06.000000 emlearn-0.8.0/emlearn.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-03-02 00:29:06.000000 emlearn-0.8.0/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-02 00:29:06.000000 emlearn-0.8.0/emlearn/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6312 2019-03-02 00:27:21.000000 emlearn-0.8.0/emlearn/net.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      595 2019-03-02 00:27:21.000000 emlearn-0.8.0/emlearn/cgen.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6446 2019-03-02 00:27:21.000000 emlearn-0.8.0/emlearn/eml_audio.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1118 2019-03-02 00:27:21.000000 emlearn-0.8.0/emlearn/signal.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2366 2019-03-02 00:27:21.000000 emlearn-0.8.0/emlearn/common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1517 2019-03-02 00:27:21.000000 emlearn-0.8.0/emlearn/eml_test.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      864 2019-03-02 00:27:21.000000 emlearn-0.8.0/emlearn/eml_fixedpoint.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2640 2019-03-02 00:27:21.000000 emlearn-0.8.0/emlearn/eml_common.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2350 2019-03-02 00:27:21.000000 emlearn-0.8.0/emlearn/eml_vector.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1935 2019-03-02 00:27:21.000000 emlearn-0.8.0/emlearn/eml_iir.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2697 2019-03-02 00:27:21.000000 emlearn-0.8.0/emlearn/eml_trees.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    11792 2019-03-02 00:27:21.000000 emlearn-0.8.0/emlearn/trees.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3442 2019-03-02 00:27:21.000000 emlearn-0.8.0/emlearn/bayes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2215 2019-03-02 00:27:21.000000 emlearn-0.8.0/emlearn/eml_benchmark.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3309 2019-03-02 00:27:21.000000 emlearn-0.8.0/emlearn/eml_fft.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3518 2019-03-02 00:27:21.000000 emlearn-0.8.0/emlearn/eml_bayes.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      133 2019-03-02 00:27:21.000000 emlearn-0.8.0/emlearn/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      722 2019-03-02 00:27:21.000000 emlearn-0.8.0/emlearn/convert.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8772 2019-03-02 00:27:21.000000 emlearn-0.8.0/emlearn/eml_net.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-02 00:29:06.000000 emlearn-0.8.0/test/
--rw-rw-r--   0 travis    (2000) travis    (2000)      774 2019-03-02 00:27:21.000000 emlearn-0.8.0/test/test_benchmark.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2462 2019-03-02 00:27:21.000000 emlearn-0.8.0/test/test_window_function.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1786 2019-03-02 00:27:21.000000 emlearn-0.8.0/test/test_filters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1278 2019-03-02 00:27:21.000000 emlearn-0.8.0/test/test_bayes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2248 2019-03-02 00:27:21.000000 emlearn-0.8.0/test/test_trees.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9497 2019-03-02 00:27:21.000000 emlearn-0.8.0/test/test_audio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5772 2019-03-02 00:27:21.000000 emlearn-0.8.0/test/test_net.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      130 2019-03-02 00:27:21.000000 emlearn-0.8.0/requirements.dev.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     5015 2019-03-02 00:27:21.000000 emlearn-0.8.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-06 19:03:24.000000 emlearn-0.8.1/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       88 2019-03-06 19:01:31.000000 emlearn-0.8.1/MANIFEST.in
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-06 19:03:24.000000 emlearn-0.8.1/examples/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     2319 2019-03-06 19:01:31.000000 emlearn-0.8.1/examples/window-function.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2149 2019-03-06 19:01:31.000000 emlearn-0.8.1/examples/mel-filterbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       28 2019-03-06 19:01:31.000000 emlearn-0.8.1/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1050 2019-03-06 19:01:31.000000 emlearn-0.8.1/LICENSE.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3055 2019-03-06 19:03:24.000000 emlearn-0.8.1/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2086 2019-03-06 19:01:31.000000 emlearn-0.8.1/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-06 19:03:24.000000 emlearn-0.8.1/bindings/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5123 2019-03-06 19:01:31.000000 emlearn-0.8.1/bindings/eml_audio.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4580 2019-03-06 19:01:31.000000 emlearn-0.8.1/bindings/eml_net.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1345 2019-03-06 19:01:31.000000 emlearn-0.8.1/bindings/eml_signal.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2297 2019-03-06 19:01:31.000000 emlearn-0.8.1/bindings/eml_trees.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2697 2019-03-06 19:01:31.000000 emlearn-0.8.1/bindings/eml_bayes.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)      860 2019-03-06 19:01:31.000000 emlearn-0.8.1/bindings/emlpy_common.hpp
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-06 19:03:24.000000 emlearn-0.8.1/emlearn.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3055 2019-03-06 19:03:24.000000 emlearn-0.8.1/emlearn.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-03-06 19:03:24.000000 emlearn-0.8.1/emlearn.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       57 2019-03-06 19:03:24.000000 emlearn-0.8.1/emlearn.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-03-06 19:03:24.000000 emlearn-0.8.1/emlearn.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      969 2019-03-06 19:03:24.000000 emlearn-0.8.1/emlearn.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       28 2019-03-06 19:03:24.000000 emlearn-0.8.1/emlearn.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-03-06 19:03:24.000000 emlearn-0.8.1/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-06 19:03:24.000000 emlearn-0.8.1/emlearn/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6312 2019-03-06 19:01:31.000000 emlearn-0.8.1/emlearn/net.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      595 2019-03-06 19:01:31.000000 emlearn-0.8.1/emlearn/cgen.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6446 2019-03-06 19:01:31.000000 emlearn-0.8.1/emlearn/eml_audio.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1118 2019-03-06 19:01:31.000000 emlearn-0.8.1/emlearn/signal.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2366 2019-03-06 19:01:31.000000 emlearn-0.8.1/emlearn/common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1517 2019-03-06 19:01:31.000000 emlearn-0.8.1/emlearn/eml_test.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      864 2019-03-06 19:01:31.000000 emlearn-0.8.1/emlearn/eml_fixedpoint.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2640 2019-03-06 19:01:31.000000 emlearn-0.8.1/emlearn/eml_common.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2350 2019-03-06 19:01:31.000000 emlearn-0.8.1/emlearn/eml_vector.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1935 2019-03-06 19:01:31.000000 emlearn-0.8.1/emlearn/eml_iir.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2697 2019-03-06 19:01:31.000000 emlearn-0.8.1/emlearn/eml_trees.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11792 2019-03-06 19:01:31.000000 emlearn-0.8.1/emlearn/trees.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3442 2019-03-06 19:01:31.000000 emlearn-0.8.1/emlearn/bayes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2215 2019-03-06 19:01:31.000000 emlearn-0.8.1/emlearn/eml_benchmark.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3309 2019-03-06 19:01:31.000000 emlearn-0.8.1/emlearn/eml_fft.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3518 2019-03-06 19:01:31.000000 emlearn-0.8.1/emlearn/eml_bayes.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      133 2019-03-06 19:01:31.000000 emlearn-0.8.1/emlearn/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      722 2019-03-06 19:01:31.000000 emlearn-0.8.1/emlearn/convert.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8772 2019-03-06 19:01:31.000000 emlearn-0.8.1/emlearn/eml_net.h
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-06 19:03:24.000000 emlearn-0.8.1/test/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      774 2019-03-06 19:01:31.000000 emlearn-0.8.1/test/test_benchmark.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2511 2019-03-06 19:01:31.000000 emlearn-0.8.1/test/test_window_function.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1786 2019-03-06 19:01:31.000000 emlearn-0.8.1/test/test_filters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1278 2019-03-06 19:01:31.000000 emlearn-0.8.1/test/test_bayes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2248 2019-03-06 19:01:31.000000 emlearn-0.8.1/test/test_trees.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9497 2019-03-06 19:01:31.000000 emlearn-0.8.1/test/test_audio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5772 2019-03-06 19:01:31.000000 emlearn-0.8.1/test/test_net.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      130 2019-03-06 19:01:31.000000 emlearn-0.8.1/requirements.dev.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5015 2019-03-06 19:01:31.000000 emlearn-0.8.1/setup.py
```

### Comparing `emlearn-0.8.0/examples/window-function.py` & `emlearn-0.8.1/examples/window-function.py`

 * *Files identical despite different names*

### Comparing `emlearn-0.8.0/examples/mel-filterbank.py` & `emlearn-0.8.1/examples/mel-filterbank.py`

 * *Files identical despite different names*

### Comparing `emlearn-0.8.0/LICENSE.md` & `emlearn-0.8.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `emlearn-0.8.0/PKG-INFO` & `emlearn-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emlearn
-Version: 0.8.0
+Version: 0.8.1
 Summary: Machine learning for microcontrollers and embedded systems
 Home-page: https://github.com/emlearn/emlearn
 Author: Jon Nordby
 Author-email: jononor@gmail.com
 License: UNKNOWN
 Description: [![Travis CI Build Status](https://travis-ci.org/jonnor/emlearn.svg?branch=master)](https://travis-ci.org/jonnor/emlearn)
         [![Appveyor Build status](https://ci.appveyor.com/api/projects/status/myb325oc06w89flc?svg=true)](https://ci.appveyor.com/project/jonnor/emlearn)
```

### Comparing `emlearn-0.8.0/README.md` & `emlearn-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `emlearn-0.8.0/bindings/eml_audio.cpp` & `emlearn-0.8.1/bindings/eml_audio.cpp`

 * *Files identical despite different names*

### Comparing `emlearn-0.8.0/bindings/eml_net.cpp` & `emlearn-0.8.1/bindings/eml_net.cpp`

 * *Files identical despite different names*

### Comparing `emlearn-0.8.0/bindings/eml_signal.cpp` & `emlearn-0.8.1/bindings/eml_signal.cpp`

 * *Files identical despite different names*

### Comparing `emlearn-0.8.0/bindings/eml_trees.cpp` & `emlearn-0.8.1/bindings/eml_trees.cpp`

 * *Files identical despite different names*

### Comparing `emlearn-0.8.0/bindings/eml_bayes.cpp` & `emlearn-0.8.1/bindings/eml_bayes.cpp`

 * *Files identical despite different names*

### Comparing `emlearn-0.8.0/emlearn.egg-info/PKG-INFO` & `emlearn-0.8.1/emlearn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emlearn
-Version: 0.8.0
+Version: 0.8.1
 Summary: Machine learning for microcontrollers and embedded systems
 Home-page: https://github.com/emlearn/emlearn
 Author: Jon Nordby
 Author-email: jononor@gmail.com
 License: UNKNOWN
 Description: [![Travis CI Build Status](https://travis-ci.org/jonnor/emlearn.svg?branch=master)](https://travis-ci.org/jonnor/emlearn)
         [![Appveyor Build status](https://ci.appveyor.com/api/projects/status/myb325oc06w89flc?svg=true)](https://ci.appveyor.com/project/jonnor/emlearn)
```

### Comparing `emlearn-0.8.0/emlearn.egg-info/SOURCES.txt` & `emlearn-0.8.1/emlearn.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 requirements.txt
 setup.py
 bindings/eml_audio.cpp
 bindings/eml_bayes.cpp
 bindings/eml_net.cpp
 bindings/eml_signal.cpp
 bindings/eml_trees.cpp
+bindings/emlpy_common.hpp
 emlearn/__init__.py
 emlearn/bayes.py
 emlearn/cgen.py
 emlearn/common.py
 emlearn/convert.py
 emlearn/eml_audio.h
 emlearn/eml_bayes.h
```

### Comparing `emlearn-0.8.0/emlearn/net.py` & `emlearn-0.8.1/emlearn/net.py`

 * *Files identical despite different names*

### Comparing `emlearn-0.8.0/emlearn/cgen.py` & `emlearn-0.8.1/emlearn/cgen.py`

 * *Files identical despite different names*

### Comparing `emlearn-0.8.0/emlearn/eml_audio.h` & `emlearn-0.8.1/emlearn/eml_audio.h`

 * *Files identical despite different names*

### Comparing `emlearn-0.8.0/emlearn/signal.py` & `emlearn-0.8.1/emlearn/signal.py`

 * *Files identical despite different names*

### Comparing `emlearn-0.8.0/emlearn/common.py` & `emlearn-0.8.1/emlearn/common.py`

 * *Files identical despite different names*

### Comparing `emlearn-0.8.0/emlearn/eml_test.h` & `emlearn-0.8.1/emlearn/eml_test.h`

 * *Files identical despite different names*

### Comparing `emlearn-0.8.0/emlearn/eml_fixedpoint.h` & `emlearn-0.8.1/emlearn/eml_fixedpoint.h`

 * *Files identical despite different names*

### Comparing `emlearn-0.8.0/emlearn/eml_common.h` & `emlearn-0.8.1/emlearn/eml_common.h`

 * *Files identical despite different names*

### Comparing `emlearn-0.8.0/emlearn/eml_vector.h` & `emlearn-0.8.1/emlearn/eml_vector.h`

 * *Files identical despite different names*

### Comparing `emlearn-0.8.0/emlearn/eml_iir.h` & `emlearn-0.8.1/emlearn/eml_iir.h`

 * *Files identical despite different names*

### Comparing `emlearn-0.8.0/emlearn/eml_trees.h` & `emlearn-0.8.1/emlearn/eml_trees.h`

 * *Files identical despite different names*

### Comparing `emlearn-0.8.0/emlearn/trees.py` & `emlearn-0.8.1/emlearn/trees.py`

 * *Files identical despite different names*

### Comparing `emlearn-0.8.0/emlearn/bayes.py` & `emlearn-0.8.1/emlearn/bayes.py`

 * *Files identical despite different names*

### Comparing `emlearn-0.8.0/emlearn/eml_benchmark.h` & `emlearn-0.8.1/emlearn/eml_benchmark.h`

 * *Files identical despite different names*

### Comparing `emlearn-0.8.0/emlearn/eml_fft.h` & `emlearn-0.8.1/emlearn/eml_fft.h`

 * *Files identical despite different names*

### Comparing `emlearn-0.8.0/emlearn/eml_bayes.h` & `emlearn-0.8.1/emlearn/eml_bayes.h`

 * *Files identical despite different names*

### Comparing `emlearn-0.8.0/emlearn/convert.py` & `emlearn-0.8.1/emlearn/convert.py`

 * *Files identical despite different names*

### Comparing `emlearn-0.8.0/emlearn/eml_net.h` & `emlearn-0.8.1/emlearn/eml_net.h`

 * *Files identical despite different names*

### Comparing `emlearn-0.8.0/test/test_benchmark.py` & `emlearn-0.8.1/test/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `emlearn-0.8.0/test/test_window_function.py` & `emlearn-0.8.1/test/test_window_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import numpy
 
 examples_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), '../examples'))
 
 
 def run_window_function(options):
     path = os.path.join(examples_dir, 'window-function.py')
-    args = ['python3', path]
+    args = ['python', path]
 
     for key, value in options.items():
         args.append('--{}={}'.format(key, value))
 
     stdout = subprocess.check_output(' '.join(args), shell=True)
     return stdout.decode('utf-8')
 
@@ -48,15 +48,16 @@
 
     params = dict(include=include, name=name, length=length)
     prog = template_prog.format(**params)
     with open(code_path, 'w') as f:
         f.write(prog)
 
     # compile
-    subprocess.check_call(['gcc', code_path, '-o', prog_path])
+    args = ['gcc', '-std=c99', code_path, '-o', prog_path]
+    subprocess.check_call(' '.join(args), shell=True)
 
     stdout = subprocess.check_output([prog_path])
     arr = json.loads(stdout)
     return arr
 
 
 def window_function_test(file_path, args):
```

### Comparing `emlearn-0.8.0/test/test_filters.py` & `emlearn-0.8.1/test/test_filters.py`

 * *Files identical despite different names*

### Comparing `emlearn-0.8.0/test/test_bayes.py` & `emlearn-0.8.1/test/test_bayes.py`

 * *Files identical despite different names*

### Comparing `emlearn-0.8.0/test/test_trees.py` & `emlearn-0.8.1/test/test_trees.py`

 * *Files identical despite different names*

### Comparing `emlearn-0.8.0/test/test_audio.py` & `emlearn-0.8.1/test/test_audio.py`

 * *Files identical despite different names*

### Comparing `emlearn-0.8.0/test/test_net.py` & `emlearn-0.8.1/test/test_net.py`

 * *Files identical despite different names*

### Comparing `emlearn-0.8.0/setup.py` & `emlearn-0.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, Extension
 from setuptools.command.build_ext import build_ext
 import sys
 import os.path
 import setuptools
 
-__version__ = '0.8.0'
+__version__ = '0.8.1'
 
 project_dir = os.path.abspath(os.path.dirname(__file__))
 
 class get_pybind_include(object):
     """Helper class to determine the pybind11 include path
     The purpose of this class is to postpone importing pybind11
     until it is actually installed, so that the ``get_include()``
```

