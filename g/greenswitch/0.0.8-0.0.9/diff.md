# Comparing `tmp/greenswitch-0.0.8.tar.gz` & `tmp/greenswitch-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/greenswitch-0.0.8.tar", last modified: Thu Dec 29 13:17:51 2016, max compression
+gzip compressed data, was "dist/greenswitch-0.0.9.tar", last modified: Tue Dec 18 13:38:12 2018, max compression
```

## Comparing `greenswitch-0.0.8.tar` & `greenswitch-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 italorossi   (503) staff       (20)        0 2016-12-29 13:17:51.000000 greenswitch-0.0.8/
-drwxr-xr-x   0 italorossi   (503) staff       (20)        0 2016-12-29 13:17:51.000000 greenswitch-0.0.8/greenswitch/
--rw-r--r--   0 italorossi   (503) staff       (20)      223 2016-04-11 18:55:59.000000 greenswitch-0.0.8/greenswitch/__init__.py
--rw-r--r--   0 italorossi   (503) staff       (20)     7219 2016-12-29 13:14:51.000000 greenswitch-0.0.8/greenswitch/esl.py
-drwxr-xr-x   0 italorossi   (503) staff       (20)        0 2016-12-29 13:17:51.000000 greenswitch-0.0.8/greenswitch.egg-info/
--rw-r--r--   0 italorossi   (503) staff       (20)        1 2016-12-29 13:17:51.000000 greenswitch-0.0.8/greenswitch.egg-info/dependency_links.txt
--rw-r--r--   0 italorossi   (503) staff       (20)     1965 2016-12-29 13:17:51.000000 greenswitch-0.0.8/greenswitch.egg-info/PKG-INFO
--rw-r--r--   0 italorossi   (503) staff       (20)       11 2016-12-29 13:17:51.000000 greenswitch-0.0.8/greenswitch.egg-info/requires.txt
--rw-r--r--   0 italorossi   (503) staff       (20)      273 2016-12-29 13:17:51.000000 greenswitch-0.0.8/greenswitch.egg-info/SOURCES.txt
--rw-r--r--   0 italorossi   (503) staff       (20)       12 2016-12-29 13:17:51.000000 greenswitch-0.0.8/greenswitch.egg-info/top_level.txt
--rw-r--r--   0 italorossi   (503) staff       (20)     1074 2016-02-28 22:36:29.000000 greenswitch-0.0.8/LICENSE
--rw-r--r--   0 italorossi   (503) staff       (20)       44 2016-02-28 23:55:48.000000 greenswitch-0.0.8/MANIFEST.in
--rw-r--r--   0 italorossi   (503) staff       (20)     1965 2016-12-29 13:17:51.000000 greenswitch-0.0.8/PKG-INFO
--rw-r--r--   0 italorossi   (503) staff       (20)     1000 2016-04-08 21:33:08.000000 greenswitch-0.0.8/README.rst
--rw-r--r--   0 italorossi   (503) staff       (20)       11 2016-11-05 23:25:40.000000 greenswitch-0.0.8/requirements.txt
--rw-r--r--   0 italorossi   (503) staff       (20)       59 2016-12-29 13:17:51.000000 greenswitch-0.0.8/setup.cfg
--rw-r--r--   0 italorossi   (503) staff       (20)     1084 2016-12-29 13:15:01.000000 greenswitch-0.0.8/setup.py
+drwxr-xr-x   0 italorossi   (503) staff       (20)        0 2018-12-18 13:38:12.000000 greenswitch-0.0.9/
+-rw-r--r--   0 italorossi   (503) staff       (20)     7730 2018-12-18 13:38:12.000000 greenswitch-0.0.9/PKG-INFO
+drwxr-xr-x   0 italorossi   (503) staff       (20)        0 2018-12-18 13:38:12.000000 greenswitch-0.0.9/greenswitch/
+-rw-r--r--   0 italorossi   (503) staff       (20)    20681 2018-12-18 12:45:28.000000 greenswitch-0.0.9/greenswitch/esl.py
+-rw-r--r--   0 italorossi   (503) staff       (20)      258 2018-08-29 19:13:33.000000 greenswitch-0.0.9/greenswitch/__init__.py
+-rw-r--r--   0 italorossi   (503) staff       (20)     1152 2018-08-29 19:13:33.000000 greenswitch-0.0.9/LICENSE
+-rw-r--r--   0 italorossi   (503) staff       (20)       11 2016-11-05 23:25:40.000000 greenswitch-0.0.9/requirements.txt
+-rw-r--r--   0 italorossi   (503) staff       (20)       44 2016-02-28 23:55:48.000000 greenswitch-0.0.9/MANIFEST.in
+drwxr-xr-x   0 italorossi   (503) staff       (20)        0 2018-12-18 13:38:12.000000 greenswitch-0.0.9/greenswitch.egg-info/
+-rw-r--r--   0 italorossi   (503) staff       (20)     7730 2018-12-18 13:38:12.000000 greenswitch-0.0.9/greenswitch.egg-info/PKG-INFO
+-rw-r--r--   0 italorossi   (503) staff       (20)      273 2018-12-18 13:38:12.000000 greenswitch-0.0.9/greenswitch.egg-info/SOURCES.txt
+-rw-r--r--   0 italorossi   (503) staff       (20)       11 2018-12-18 13:38:12.000000 greenswitch-0.0.9/greenswitch.egg-info/requires.txt
+-rw-r--r--   0 italorossi   (503) staff       (20)       12 2018-12-18 13:38:12.000000 greenswitch-0.0.9/greenswitch.egg-info/top_level.txt
+-rw-r--r--   0 italorossi   (503) staff       (20)        1 2018-12-18 13:38:12.000000 greenswitch-0.0.9/greenswitch.egg-info/dependency_links.txt
+-rw-r--r--   0 italorossi   (503) staff       (20)     1084 2018-12-18 13:35:02.000000 greenswitch-0.0.9/setup.py
+-rw-r--r--   0 italorossi   (503) staff       (20)       38 2018-12-18 13:38:12.000000 greenswitch-0.0.9/setup.cfg
+-rw-r--r--   0 italorossi   (503) staff       (20)     5765 2018-08-29 19:13:33.000000 greenswitch-0.0.9/README.rst
```

### Comparing `greenswitch-0.0.8/LICENSE` & `greenswitch-0.0.9/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 The MIT License
 
-Copyright (c) 2016 Ítalo Rossi.
+Copyright (c) 2016, Evolux Sistemas Ltda.
+
+This project was originally created and maintained by Ítalo Rossi.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `greenswitch-0.0.8/setup.py` & `greenswitch-0.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     readme = f.read()
 
 with open('requirements.txt') as f:
     requires = f.readlines()
 
 setup(
     name='greenswitch',
-    version='0.0.8',
+    version='0.0.9',
     description=u'Battle proven FreeSWITCH Event Socket Protocol client implementation with Gevent.',
     long_description=readme,
     author=u'Ítalo Rossi',
     author_email=u'italorossib@gmail.com',
     url=u'https://github.com/evoluxbr/greenswitch',
     license=u'MIT',
     packages=find_packages(exclude=('tests', 'docs')),
```

