# Comparing `tmp/collective.shariff-2.0.1.tar.gz` & `tmp/collective.shariff-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.shariff-2.0.1.tar", last modified: Mon Dec 20 09:17:16 2021, max compression
+gzip compressed data, was "collective.shariff-3.0.0.tar", last modified: Fri Oct  7 08:40:54 2022, max compression
```

## Comparing `collective.shariff-2.0.1.tar` & `collective.shariff-3.0.0.tar`

### file list

```diff
@@ -1,59 +1,65 @@
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2021-12-20 09:17:16.644193 collective.shariff-2.0.1/
--rw-r--r--   0 peterm     (501) staff       (20)      522 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/CHANGES.rst
--rw-r--r--   0 peterm     (501) staff       (20)    17987 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/LICENSE.GPL
--rw-r--r--   0 peterm     (501) staff       (20)      735 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/LICENSE.txt
--rw-r--r--   0 peterm     (501) staff       (20)      394 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/MANIFEST.in
--rw-r--r--   0 peterm     (501) staff       (20)     2424 2021-12-20 09:17:16.644341 collective.shariff-2.0.1/PKG-INFO
--rw-r--r--   0 peterm     (501) staff       (20)      598 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/README.rst
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2021-12-20 09:17:16.627407 collective.shariff-2.0.1/collective/
--rw-r--r--   0 peterm     (501) staff       (20)      244 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective/__init__.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2021-12-20 09:17:16.632376 collective.shariff-2.0.1/collective/shariff/
--rw-r--r--   0 peterm     (501) staff       (20)        0 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective/shariff/__init__.py
--rw-r--r--   0 peterm     (501) staff       (20)     1377 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective/shariff/browser.py
--rw-r--r--   0 peterm     (501) staff       (20)     1427 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective/shariff/configure.zcml
--rw-r--r--   0 peterm     (501) staff       (20)     1607 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective/shariff/decorator.py
--rw-r--r--   0 peterm     (501) staff       (20)      112 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective/shariff/interfaces.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2021-12-20 09:17:16.624816 collective.shariff-2.0.1/collective/shariff/profiles/
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2021-12-20 09:17:16.633340 collective.shariff-2.0.1/collective/shariff/profiles/default/
--rw-r--r--   0 peterm     (501) staff       (20)      282 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective/shariff/profiles/default/browserlayer.xml
--rw-r--r--   0 peterm     (501) staff       (20)       71 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective/shariff/profiles/default/metadata.xml
--rw-r--r--   0 peterm     (501) staff       (20)     2157 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective/shariff/profiles/default/registry.xml
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2021-12-20 09:17:16.634616 collective.shariff-2.0.1/collective/shariff/profiles/uninstall/
--rw-r--r--   0 peterm     (501) staff       (20)      187 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective/shariff/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 peterm     (501) staff       (20)      231 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective/shariff/profiles/uninstall/cssregistry.xml
--rw-r--r--   0 peterm     (501) staff       (20)      245 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective/shariff/profiles/uninstall/jsregistry.xml
--rw-r--r--   0 peterm     (501) staff       (20)      634 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective/shariff/profiles/uninstall/registry.xml
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2021-12-20 09:17:16.643807 collective.shariff-2.0.1/collective/shariff/resources/
--rwxr-xr-x   0 peterm     (501) staff       (20)   129648 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective/shariff/resources/fa-brands-400.eot
--rwxr-xr-x   0 peterm     (501) staff       (20)   691865 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective/shariff/resources/fa-brands-400.svg
--rwxr-xr-x   0 peterm     (501) staff       (20)   129344 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective/shariff/resources/fa-brands-400.ttf
--rwxr-xr-x   0 peterm     (501) staff       (20)    87544 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective/shariff/resources/fa-brands-400.woff
--rwxr-xr-x   0 peterm     (501) staff       (20)    74656 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective/shariff/resources/fa-brands-400.woff2
--rwxr-xr-x   0 peterm     (501) staff       (20)    34388 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective/shariff/resources/fa-regular-400.eot
--rwxr-xr-x   0 peterm     (501) staff       (20)   144451 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective/shariff/resources/fa-regular-400.svg
--rwxr-xr-x   0 peterm     (501) staff       (20)    34092 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective/shariff/resources/fa-regular-400.ttf
--rwxr-xr-x   0 peterm     (501) staff       (20)    16804 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective/shariff/resources/fa-regular-400.woff
--rwxr-xr-x   0 peterm     (501) staff       (20)    13584 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective/shariff/resources/fa-regular-400.woff2
--rwxr-xr-x   0 peterm     (501) staff       (20)   186708 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective/shariff/resources/fa-solid-900.eot
--rwxr-xr-x   0 peterm     (501) staff       (20)   816852 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective/shariff/resources/fa-solid-900.svg
--rwxr-xr-x   0 peterm     (501) staff       (20)   186424 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective/shariff/resources/fa-solid-900.ttf
--rwxr-xr-x   0 peterm     (501) staff       (20)    96256 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective/shariff/resources/fa-solid-900.woff
--rwxr-xr-x   0 peterm     (501) staff       (20)    74328 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective/shariff/resources/fa-solid-900.woff2
--rwxr-xr-x   0 peterm     (501) staff       (20)    69064 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective/shariff/resources/shariff.complete.css
--rwxr-xr-x   0 peterm     (501) staff       (20)    49865 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective/shariff/resources/shariff.complete.js
--rwxr-xr-x   0 peterm     (501) staff       (20)    12509 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective/shariff/resources/shariff.min.css
--rwxr-xr-x   0 peterm     (501) staff       (20)    46135 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective/shariff/resources/shariff.min.js
--rw-r--r--   0 peterm     (501) staff       (20)     1414 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective/shariff/setuphandlers.py
--rw-r--r--   0 peterm     (501) staff       (20)     1413 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective/shariff/tests.py
--rw-r--r--   0 peterm     (501) staff       (20)      559 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective/shariff/viewlet.pt
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2021-12-20 09:17:16.630074 collective.shariff-2.0.1/collective.shariff.egg-info/
--rw-r--r--   0 peterm     (501) staff       (20)     2424 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective.shariff.egg-info/PKG-INFO
--rw-r--r--   0 peterm     (501) staff       (20)     1966 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective.shariff.egg-info/SOURCES.txt
--rw-r--r--   0 peterm     (501) staff       (20)        1 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective.shariff.egg-info/dependency_links.txt
--rw-r--r--   0 peterm     (501) staff       (20)       59 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective.shariff.egg-info/entry_points.txt
--rw-r--r--   0 peterm     (501) staff       (20)       11 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective.shariff.egg-info/namespace_packages.txt
--rw-r--r--   0 peterm     (501) staff       (20)        1 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective.shariff.egg-info/not-zip-safe
--rw-r--r--   0 peterm     (501) staff       (20)       26 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective.shariff.egg-info/requires.txt
--rw-r--r--   0 peterm     (501) staff       (20)       11 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/collective.shariff.egg-info/top_level.txt
--rw-r--r--   0 peterm     (501) staff       (20)       67 2021-12-20 09:17:16.644830 collective.shariff-2.0.1/setup.cfg
--rw-r--r--   0 peterm     (501) staff       (20)     1419 2021-12-20 09:17:16.000000 collective.shariff-2.0.1/setup.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2022-10-07 08:40:54.264516 collective.shariff-3.0.0/
+-rw-r--r--   0 peterm     (501) staff       (20)      601 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/CHANGES.rst
+-rw-r--r--   0 peterm     (501) staff       (20)    17987 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/LICENSE.GPL
+-rw-r--r--   0 peterm     (501) staff       (20)      735 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/LICENSE.txt
+-rw-r--r--   0 peterm     (501) staff       (20)      426 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/MANIFEST.in
+-rw-r--r--   0 peterm     (501) staff       (20)    11790 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/Makefile
+-rw-r--r--   0 peterm     (501) staff       (20)     2218 2022-10-07 08:40:54.264578 collective.shariff-3.0.0/PKG-INFO
+-rw-r--r--   0 peterm     (501) staff       (20)      613 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/README.rst
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2022-10-07 08:40:54.255668 collective.shariff-3.0.0/collective/
+-rw-r--r--   0 peterm     (501) staff       (20)      245 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/collective/__init__.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2022-10-07 08:40:54.258014 collective.shariff-3.0.0/collective/shariff/
+-rw-r--r--   0 peterm     (501) staff       (20)        0 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/collective/shariff/__init__.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1387 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/collective/shariff/browser.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1599 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/collective/shariff/configure.zcml
+-rw-r--r--   0 peterm     (501) staff       (20)     1568 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/collective/shariff/decorator.py
+-rw-r--r--   0 peterm     (501) staff       (20)      110 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/collective/shariff/interfaces.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2022-10-07 08:40:54.254121 collective.shariff-3.0.0/collective/shariff/profiles/
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2022-10-07 08:40:54.258543 collective.shariff-3.0.0/collective/shariff/profiles/default/
+-rw-r--r--   0 peterm     (501) staff       (20)      282 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/collective/shariff/profiles/default/browserlayer.xml
+-rw-r--r--   0 peterm     (501) staff       (20)       71 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/collective/shariff/profiles/default/metadata.xml
+-rw-r--r--   0 peterm     (501) staff       (20)     2043 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/collective/shariff/profiles/default/registry.xml
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2022-10-07 08:40:54.258818 collective.shariff-3.0.0/collective/shariff/profiles/uninstall/
+-rw-r--r--   0 peterm     (501) staff       (20)      187 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/collective/shariff/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 peterm     (501) staff       (20)      516 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/collective/shariff/profiles/uninstall/registry.xml
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2022-10-07 08:40:54.264156 collective.shariff-3.0.0/collective/shariff/resources/
+-rwxr-xr-x   0 peterm     (501) staff       (20)   129648 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/collective/shariff/resources/fa-brands-400.eot
+-rwxr-xr-x   0 peterm     (501) staff       (20)   691865 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/collective/shariff/resources/fa-brands-400.svg
+-rwxr-xr-x   0 peterm     (501) staff       (20)   129344 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/collective/shariff/resources/fa-brands-400.ttf
+-rwxr-xr-x   0 peterm     (501) staff       (20)    87544 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/collective/shariff/resources/fa-brands-400.woff
+-rwxr-xr-x   0 peterm     (501) staff       (20)    74656 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/collective/shariff/resources/fa-brands-400.woff2
+-rwxr-xr-x   0 peterm     (501) staff       (20)    34388 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/collective/shariff/resources/fa-regular-400.eot
+-rwxr-xr-x   0 peterm     (501) staff       (20)   144451 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/collective/shariff/resources/fa-regular-400.svg
+-rwxr-xr-x   0 peterm     (501) staff       (20)    34092 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/collective/shariff/resources/fa-regular-400.ttf
+-rwxr-xr-x   0 peterm     (501) staff       (20)    16804 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/collective/shariff/resources/fa-regular-400.woff
+-rwxr-xr-x   0 peterm     (501) staff       (20)    13584 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/collective/shariff/resources/fa-regular-400.woff2
+-rwxr-xr-x   0 peterm     (501) staff       (20)   186708 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/collective/shariff/resources/fa-solid-900.eot
+-rwxr-xr-x   0 peterm     (501) staff       (20)   816852 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/collective/shariff/resources/fa-solid-900.svg
+-rwxr-xr-x   0 peterm     (501) staff       (20)   186424 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/collective/shariff/resources/fa-solid-900.ttf
+-rwxr-xr-x   0 peterm     (501) staff       (20)    96256 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/collective/shariff/resources/fa-solid-900.woff
+-rwxr-xr-x   0 peterm     (501) staff       (20)    74328 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/collective/shariff/resources/fa-solid-900.woff2
+-rwxr-xr-x   0 peterm     (501) staff       (20)    69064 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/collective/shariff/resources/shariff.complete.css
+-rwxr-xr-x   0 peterm     (501) staff       (20)    49865 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/collective/shariff/resources/shariff.complete.js
+-rwxr-xr-x   0 peterm     (501) staff       (20)    12509 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/collective/shariff/resources/shariff.min.css
+-rwxr-xr-x   0 peterm     (501) staff       (20)    46135 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/collective/shariff/resources/shariff.min.js
+-rw-r--r--   0 peterm     (501) staff       (20)      400 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/collective/shariff/setuphandlers.py
+-rw-r--r--   0 peterm     (501) staff       (20)      844 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/collective/shariff/testing.py
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2022-10-07 08:40:54.264418 collective.shariff-3.0.0/collective/shariff/tests/
+-rw-r--r--   0 peterm     (501) staff       (20)        0 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/collective/shariff/tests/__init__.py
+-rw-r--r--   0 peterm     (501) staff       (20)     1973 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/collective/shariff/tests/test_setup.py
+-rw-r--r--   0 peterm     (501) staff       (20)      427 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/collective/shariff/upgrades.zcml
+-rw-r--r--   0 peterm     (501) staff       (20)      559 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/collective/shariff/viewlet.pt
+drwxr-xr-x   0 peterm     (501) staff       (20)        0 2022-10-07 08:40:54.256588 collective.shariff-3.0.0/collective.shariff.egg-info/
+-rw-r--r--   0 peterm     (501) staff       (20)     2218 2022-10-07 08:40:54.000000 collective.shariff-3.0.0/collective.shariff.egg-info/PKG-INFO
+-rw-r--r--   0 peterm     (501) staff       (20)     2019 2022-10-07 08:40:54.000000 collective.shariff-3.0.0/collective.shariff.egg-info/SOURCES.txt
+-rw-r--r--   0 peterm     (501) staff       (20)        1 2022-10-07 08:40:54.000000 collective.shariff-3.0.0/collective.shariff.egg-info/dependency_links.txt
+-rw-r--r--   0 peterm     (501) staff       (20)       40 2022-10-07 08:40:54.000000 collective.shariff-3.0.0/collective.shariff.egg-info/entry_points.txt
+-rw-r--r--   0 peterm     (501) staff       (20)       11 2022-10-07 08:40:54.000000 collective.shariff-3.0.0/collective.shariff.egg-info/namespace_packages.txt
+-rw-r--r--   0 peterm     (501) staff       (20)        1 2022-10-07 08:40:54.000000 collective.shariff-3.0.0/collective.shariff.egg-info/not-zip-safe
+-rw-r--r--   0 peterm     (501) staff       (20)      132 2022-10-07 08:40:54.000000 collective.shariff-3.0.0/collective.shariff.egg-info/requires.txt
+-rw-r--r--   0 peterm     (501) staff       (20)       11 2022-10-07 08:40:54.000000 collective.shariff-3.0.0/collective.shariff.egg-info/top_level.txt
+-rw-r--r--   0 peterm     (501) staff       (20)       58 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/constraints.txt
+-rw-r--r--   0 peterm     (501) staff       (20)      631 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/mx.ini
+-rw-r--r--   0 peterm     (501) staff       (20)      153 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/requirements.txt
+-rw-r--r--   0 peterm     (501) staff       (20)      230 2022-10-07 08:40:54.264822 collective.shariff-3.0.0/setup.cfg
+-rw-r--r--   0 peterm     (501) staff       (20)     1853 2022-10-07 08:40:53.000000 collective.shariff-3.0.0/setup.py
```

### Comparing `collective.shariff-2.0.1/LICENSE.GPL` & `collective.shariff-3.0.0/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.shariff-2.0.1/LICENSE.txt` & `collective.shariff-3.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `collective.shariff-2.0.1/README.rst` & `collective.shariff-3.0.0/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 This package contains resources of https://github.com/heiseonline/shariff −
 a social media button package with focus on privacy.
 
 Versions:
 ---------
 
 - 1.x -> Plone 4.3
-- 2.x -> Plone 5.x/6.0
+- 2.x -> Plone 5.x
+- 3.x -> Plone 6.x
 
 
 TODO
 ====
 
 - Add tests
 - Create a ``shariff.json`` view
```

### Comparing `collective.shariff-2.0.1/collective/shariff/browser.py` & `collective.shariff-3.0.0/collective/shariff/browser.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,37 +4,38 @@
 from Products.Five import BrowserView
 from Products.Five.browser.pagetemplatefile import ViewPageTemplateFile
 
 import json
 
 
 class Shariff(BrowserView):
-
     def __call__(self):
-        """ backend view to determine counters next to buttons """
+        """backend view to determine counters next to buttons"""
         # XXX: NOT INMPLEMENTED RIGHT NOW
         pass
 
 
 class ShariffViewlet(ViewletBase):
-    index = ViewPageTemplateFile('viewlet.pt')
+    index = ViewPageTemplateFile("viewlet.pt")
 
     def render(self):
         # hide on edit/add views
         if IViewView.providedBy(self.view):
             return self.index()
-        return u""
+        return ""
 
     def update(self):
         super(ShariffViewlet, self).update()
         b_url = api.portal.get_registry_record(
-            'collective.shariff.settings.backend_url')
+            "collective.shariff.settings.backend_url"
+        )
         if b_url:
             self.backend_url = "{}/{}".format(self.navigation_root_url, b_url)
-        self.theme = api.portal.get_registry_record(
-            'collective.shariff.settings.theme')
+        self.theme = api.portal.get_registry_record("collective.shariff.settings.theme")
         self.lang = api.portal.get_current_language()
         self.url = self.context.absolute_url()
         self.twitter_via = api.portal.get_registry_record(
-            'collective.shariff.settings.twitter_via')
-        self.services = json.dumps(api.portal.get_registry_record(
-            'collective.shariff.settings.services'))
+            "collective.shariff.settings.twitter_via"
+        )
+        self.services = json.dumps(
+            api.portal.get_registry_record("collective.shariff.settings.services")
+        )
```

### Comparing `collective.shariff-2.0.1/collective/shariff/configure.zcml` & `collective.shariff-3.0.0/collective/shariff/configure.zcml`

 * *Files 6% similar despite different names*

```diff
@@ -3,47 +3,48 @@
     xmlns:five="http://namespaces.zope.org/five"
     xmlns:i18n="http://namespaces.zope.org/i18n"
     xmlns:plone="http://namespaces.plone.org/plone"
     xmlns:browser="http://namespaces.zope.org/browser"
     xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
     i18n_domain="collective.shariff">
 
-  <genericsetup:registerProfile
-      name="default"
-      title="collective.shariff"
-      directory="profiles/default"
-      description="Installs the collective.shariff package"
-      provides="Products.GenericSetup.interfaces.EXTENSION"
-      />
-
-  <genericsetup:registerProfile
-      name="uninstall"
-      title="collective.shariff (uninstall)"
-      directory="profiles/uninstall"
-      description="Uninstalls the collective.shariff package"
-      provides="Products.GenericSetup.interfaces.EXTENSION"
-      />
+    <genericsetup:registerProfile
+        name="default"
+        title="collective.shariff"
+        directory="profiles/default"
+        description="Installs the collective.shariff package"
+        provides="Products.GenericSetup.interfaces.EXTENSION" />
+
+    <genericsetup:registerProfile
+        name="uninstall"
+        title="collective.shariff (uninstall)"
+        directory="profiles/uninstall"
+        description="Uninstalls the collective.shariff package"
+        provides="Products.GenericSetup.interfaces.EXTENSION" />
+
+    <utility
+        factory=".setuphandlers.HiddenProfiles"
+        name="collective.shariff-hiddenprofiles" />
 
-  <!-- -*- extra stuff goes here -*- -->
-  <plone:static
+    <include file="upgrades.zcml" />
+
+    <!-- -*- extra stuff goes here -*- -->
+    <plone:static
         directory="resources"
         type="plone"
-        name="collective.shariff"
-        />
+        name="collective.shariff" />
 
-  <browser:page
-      name="shariff"
-      class=".browser.Shariff"
-      for="*"
-      permission="zope2.View"
-      />
-
-  <browser:viewlet
-      name="collective.shariff"
-      for="*"
-      class=".browser.ShariffViewlet"
-      manager="plone.app.layout.viewlets.interfaces.IBelowContent"
-      permission="zope2.View"
-      layer=".interfaces.IShariffInstalled"
-      />
+    <browser:page
+        name="shariff"
+        class=".browser.Shariff"
+        for="*"
+        permission="zope2.View" />
+
+    <browser:viewlet
+        name="collective.shariff"
+        for="*"
+        class=".browser.ShariffViewlet"
+        manager="plone.app.layout.viewlets.interfaces.IBelowContent"
+        permission="zope2.View"
+        layer=".interfaces.IShariffInstalled" />
 
 </configure>
```

### Comparing `collective.shariff-2.0.1/collective/shariff/decorator.py` & `collective.shariff-3.0.0/collective/shariff/decorator.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 """
 Decorator for upgrade steps
 """
 
 # Python compatibility:
 from __future__ import absolute_import
 
-# Standard library:
-import logging
 from functools import wraps
 from time import time
 
+# Standard library:
+import logging
+
+
 __all__ = [
-        # decorators:
-        'step',
-        # exceptions:
-        'StepAborted',
-        ]
+    # decorators:
+    "step",
+    # exceptions:
+    "StepAborted",
+]
 
 
 class StepAborted(Exception):
     """
     Raised by the @step decorator if keyboard-interrupted
     """
 
@@ -28,33 +30,34 @@
 def step(func):
     """
     Decorate a migration step:
     - amend the logger argument, if missing
     - log the execution time
     - catch keyboard interrupts to allow the Zope instance to keep on running
     """
+
     @wraps(func)
     def wrapper(context, logger=None):
         funcname = func.__name__
         if logger is None:
-            logger = logging.getLogger('setup:'+funcname)
+            logger = logging.getLogger("setup:" + funcname)
         _started = time()
         try:
             res = func(context, logger)
         except Exception as e:
             delta = time() - _started
             if isinstance(e, KeyboardInterrupt):
-                logger.error('%(funcname)s aborted after %(delta)5.2f seconds',
-                             locals())
+                logger.error(
+                    "%(funcname)s aborted after %(delta)5.2f seconds", locals()
+                )
                 logger.exception(e)
                 raise StepAborted
             else:
-                logger.error('%(funcname)s: %(e)r after %(delta)5.2f seconds',
-                             locals())
+                logger.error("%(funcname)s: %(e)r after %(delta)5.2f seconds", locals())
                 logger.exception(e)
                 raise
         else:
             delta = time() - _started
-            logger.info('%(res)r <-- %(funcname)s (%(delta)5.2f seconds)', locals())
+            logger.info("%(res)r <-- %(funcname)s (%(delta)5.2f seconds)", locals())
         return res
 
     return wrapper
```

### Comparing `collective.shariff-2.0.1/collective/shariff/profiles/default/registry.xml` & `collective.shariff-3.0.0/collective/shariff/profiles/default/registry.xml`

 * *Files 15% similar despite different names*

#### Comparing `collective.shariff-2.0.1/collective/shariff/profiles/default/registry.xml` & `collective.shariff-3.0.0/collective/shariff/profiles/default/registry.xml`

```diff
@@ -30,17 +30,15 @@
     <field type="plone.registry.field.TextLine">
       <title>Shariff Twitter account</title>
       <description/>
     </field>
     <value/>
   </record>
   <records prefix="plone.bundles/shariff-complete" interface="Products.CMFPlone.interfaces.IBundleRegistry">
-    <value key="depends">plone-base</value>
-    <value key="load_async">True</value>
-    <value key="merge_with">default</value>
-    <value key="compile">True</value>
+    <value key="depends">plone</value>
+    <value key="load_async">False</value>
+    <value key="load_defer">False</value>
     <value key="enabled">True</value>
     <value key="jscompilation">/++plone++collective.shariff/shariff.complete.js</value>
     <value key="csscompilation">/++plone++collective.shariff/shariff.complete.css</value>
-    <value key="last_compilation">2021-12-20 10:00:00</value>
   </records>
 </registry>
```

### Comparing `collective.shariff-2.0.1/collective/shariff/resources/fa-brands-400.eot` & `collective.shariff-3.0.0/collective/shariff/resources/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `collective.shariff-2.0.1/collective/shariff/resources/fa-brands-400.svg` & `collective.shariff-3.0.0/collective/shariff/resources/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `collective.shariff-2.0.1/collective/shariff/resources/fa-brands-400.ttf` & `collective.shariff-3.0.0/collective/shariff/resources/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `collective.shariff-2.0.1/collective/shariff/resources/fa-brands-400.woff` & `collective.shariff-3.0.0/collective/shariff/resources/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `collective.shariff-2.0.1/collective/shariff/resources/fa-brands-400.woff2` & `collective.shariff-3.0.0/collective/shariff/resources/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `collective.shariff-2.0.1/collective/shariff/resources/fa-regular-400.eot` & `collective.shariff-3.0.0/collective/shariff/resources/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `collective.shariff-2.0.1/collective/shariff/resources/fa-regular-400.svg` & `collective.shariff-3.0.0/collective/shariff/resources/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `collective.shariff-2.0.1/collective/shariff/resources/fa-regular-400.ttf` & `collective.shariff-3.0.0/collective/shariff/resources/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `collective.shariff-2.0.1/collective/shariff/resources/fa-regular-400.woff` & `collective.shariff-3.0.0/collective/shariff/resources/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `collective.shariff-2.0.1/collective/shariff/resources/fa-regular-400.woff2` & `collective.shariff-3.0.0/collective/shariff/resources/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `collective.shariff-2.0.1/collective/shariff/resources/fa-solid-900.eot` & `collective.shariff-3.0.0/collective/shariff/resources/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `collective.shariff-2.0.1/collective/shariff/resources/fa-solid-900.svg` & `collective.shariff-3.0.0/collective/shariff/resources/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `collective.shariff-2.0.1/collective/shariff/resources/fa-solid-900.ttf` & `collective.shariff-3.0.0/collective/shariff/resources/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `collective.shariff-2.0.1/collective/shariff/resources/fa-solid-900.woff` & `collective.shariff-3.0.0/collective/shariff/resources/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `collective.shariff-2.0.1/collective/shariff/resources/fa-solid-900.woff2` & `collective.shariff-3.0.0/collective/shariff/resources/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `collective.shariff-2.0.1/collective/shariff/resources/shariff.complete.css` & `collective.shariff-3.0.0/collective/shariff/resources/shariff.complete.css`

 * *Files identical despite different names*

### Comparing `collective.shariff-2.0.1/collective/shariff/resources/shariff.complete.js` & `collective.shariff-3.0.0/collective/shariff/resources/shariff.complete.js`

 * *Files identical despite different names*

### Comparing `collective.shariff-2.0.1/collective/shariff/resources/shariff.min.css` & `collective.shariff-3.0.0/collective/shariff/resources/shariff.min.css`

 * *Files identical despite different names*

### Comparing `collective.shariff-2.0.1/collective/shariff/resources/shariff.min.js` & `collective.shariff-3.0.0/collective/shariff/resources/shariff.min.js`

 * *Files identical despite different names*

### Comparing `collective.shariff-2.0.1/collective/shariff/viewlet.pt` & `collective.shariff-3.0.0/collective/shariff/viewlet.pt`

 * *Files identical despite different names*

### Comparing `collective.shariff-2.0.1/collective.shariff.egg-info/SOURCES.txt` & `collective.shariff-3.0.0/collective.shariff.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 CHANGES.rst
 LICENSE.GPL
 LICENSE.txt
 MANIFEST.in
+Makefile
 README.rst
+constraints.txt
+mx.ini
+requirements.txt
 setup.cfg
 setup.py
 collective/__init__.py
 collective.shariff.egg-info/PKG-INFO
 collective.shariff.egg-info/SOURCES.txt
 collective.shariff.egg-info/dependency_links.txt
 collective.shariff.egg-info/entry_points.txt
@@ -16,22 +20,21 @@
 collective.shariff.egg-info/top_level.txt
 collective/shariff/__init__.py
 collective/shariff/browser.py
 collective/shariff/configure.zcml
 collective/shariff/decorator.py
 collective/shariff/interfaces.py
 collective/shariff/setuphandlers.py
-collective/shariff/tests.py
+collective/shariff/testing.py
+collective/shariff/upgrades.zcml
 collective/shariff/viewlet.pt
 collective/shariff/profiles/default/browserlayer.xml
 collective/shariff/profiles/default/metadata.xml
 collective/shariff/profiles/default/registry.xml
 collective/shariff/profiles/uninstall/browserlayer.xml
-collective/shariff/profiles/uninstall/cssregistry.xml
-collective/shariff/profiles/uninstall/jsregistry.xml
 collective/shariff/profiles/uninstall/registry.xml
 collective/shariff/resources/fa-brands-400.eot
 collective/shariff/resources/fa-brands-400.svg
 collective/shariff/resources/fa-brands-400.ttf
 collective/shariff/resources/fa-brands-400.woff
 collective/shariff/resources/fa-brands-400.woff2
 collective/shariff/resources/fa-regular-400.eot
@@ -43,8 +46,10 @@
 collective/shariff/resources/fa-solid-900.svg
 collective/shariff/resources/fa-solid-900.ttf
 collective/shariff/resources/fa-solid-900.woff
 collective/shariff/resources/fa-solid-900.woff2
 collective/shariff/resources/shariff.complete.css
 collective/shariff/resources/shariff.complete.js
 collective/shariff/resources/shariff.min.css
-collective/shariff/resources/shariff.min.js
+collective/shariff/resources/shariff.min.js
+collective/shariff/tests/__init__.py
+collective/shariff/tests/test_setup.py
```

### Comparing `collective.shariff-2.0.1/setup.py` & `collective.shariff-3.0.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,44 +1,60 @@
-from setuptools import setup, find_packages
+from setuptools import find_packages
+from setuptools import setup
 
-version = '2.0.1'
 
-setup(name='collective.shariff',
-      version=version,
-      description="Implement shariff - social media buttons with privacy",
-      long_description='\n\n'.join([
+version = "3.0.0"
+
+setup(
+    name="collective.shariff",
+    version=version,
+    description="Implement shariff - social media buttons with privacy",
+    long_description="\n\n".join(
+        [
             open("README.rst").read(),
             open("CHANGES.rst").read(),
-            ]),
-      long_description_content_type='text/x-rst',
-      # Get more strings from
-      # http://pypi.python.org/pypi?:action=list_classifiers
-      classifiers=[
-        "Framework :: Plone",
-        "Framework :: Plone :: 5.1",
-        "Framework :: Plone :: 5.2",
-        "Framework :: Plone :: 6.0",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 2.7",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        ],
-      keywords='',
-      author='petschki',
-      author_email='peter.mathis@kominat.at',
-      url='https://github.com/collective/collective.shariff',
-      license='GPL',
-      packages=find_packages(exclude=['ez_setup']),
-      namespace_packages=['collective'],
-      include_package_data=True,
-      zip_safe=False,
-      install_requires=[
-          'setuptools',
-          # -*- Extra requirements: -*-
-          'plone.api>=1.5',
-      ],
-      entry_points="""
+        ]
+    ),
+    long_description_content_type="text/x-rst",
+    # Get more strings from
+    # http://pypi.python.org/pypi?:action=list_classifiers
+    classifiers=[
+        'Development Status :: 5 - Production/Stable',
+        'Environment :: Web Environment',
+        'Framework :: Plone',
+        'Framework :: Plone :: Addon',
+        'Framework :: Plone :: 6.0',
+        'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
+        'Operating System :: OS Independent',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Topic :: Software Development :: Libraries :: Python Modules',
+    ],
+    keywords='plone social sharing shariff',
+    author="petschki",
+    author_email="peter.mathis@kominat.at",
+    url="https://github.com/collective/collective.shariff",
+    license="GPL",
+    packages=find_packages(exclude=["ez_setup"]),
+    namespace_packages=["collective"],
+    include_package_data=True,
+    zip_safe=False,
+    install_requires=[
+        "setuptools",
+        # -*- Extra requirements: -*-
+        "plone.api>=1.5",
+    ],
+    extras_require={
+        "test": [
+            "plone.app.testing",
+            "plone.app.contenttypes",
+            "plone.app.robotframework",
+            "robotframework-selenium2library",
+        ]
+    },
+    entry_points="""
       [z3c.autoinclude.plugin]
       target = plone
       """,
-      )
+)
```

