# Comparing `tmp/pinstall-1.2.tar.gz` & `tmp/pinstall-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinstall-1.2.tar", last modified: Tue May 23 01:22:58 2023, max compression
+gzip compressed data, was "pinstall-1.3.tar", last modified: Tue May 23 04:05:38 2023, max compression
```

## Comparing `pinstall-1.2.tar` & `pinstall-1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-05-23 01:22:58.068758 pinstall-1.2/
--rw-r--r--   0 mark      (1000) mark      (1000)     7077 2023-05-23 01:22:58.068758 pinstall-1.2/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)     6695 2023-04-27 00:00:18.000000 pinstall-1.2/README.md
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-05-23 01:22:58.068758 pinstall-1.2/pinstall/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2021-01-27 04:55:01.000000 pinstall-1.2/pinstall/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)       97 2023-04-26 03:19:54.000000 pinstall-1.2/pinstall/__main__.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-05-23 01:22:58.068758 pinstall-1.2/pinstall/commands/
--rw-r--r--   0 mark      (1000) mark      (1000)     6047 2023-04-24 03:05:44.000000 pinstall-1.2/pinstall/commands/service.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1257 2023-04-21 01:09:48.000000 pinstall-1.2/pinstall/commands/status.py
--rw-r--r--   0 mark      (1000) mark      (1000)     4056 2023-05-23 01:19:49.000000 pinstall-1.2/pinstall/commands/venv.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1385 2023-04-16 04:09:21.000000 pinstall-1.2/pinstall/pinstall.py
--rw-r--r--   0 mark      (1000) mark      (1000)      775 2023-04-13 07:15:57.000000 pinstall-1.2/pinstall/run.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-05-23 01:22:58.068758 pinstall-1.2/pinstall.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     7077 2023-05-23 01:22:58.000000 pinstall-1.2/pinstall.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      374 2023-05-23 01:22:58.000000 pinstall-1.2/pinstall.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-05-23 01:22:58.000000 pinstall-1.2/pinstall.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       52 2023-05-23 01:22:58.000000 pinstall-1.2/pinstall.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       13 2023-05-23 01:22:58.000000 pinstall-1.2/pinstall.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       27 2023-05-23 01:22:58.000000 pinstall-1.2/pinstall.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       38 2023-05-23 01:22:58.068758 pinstall-1.2/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1062 2023-05-23 01:20:30.000000 pinstall-1.2/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-05-23 04:05:38.380892 pinstall-1.3/
+-rw-r--r--   0 mark      (1000) mark      (1000)     7077 2023-05-23 04:05:38.377558 pinstall-1.3/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)     6695 2023-04-27 00:00:18.000000 pinstall-1.3/README.md
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-05-23 04:05:38.377558 pinstall-1.3/pinstall/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2021-01-27 04:55:01.000000 pinstall-1.3/pinstall/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)       97 2023-04-26 03:19:54.000000 pinstall-1.3/pinstall/__main__.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-05-23 04:05:38.377558 pinstall-1.3/pinstall/commands/
+-rw-r--r--   0 mark      (1000) mark      (1000)     6047 2023-04-24 03:05:44.000000 pinstall-1.3/pinstall/commands/service.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1257 2023-04-21 01:09:48.000000 pinstall-1.3/pinstall/commands/status.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     4067 2023-05-23 04:05:00.000000 pinstall-1.3/pinstall/commands/venv.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1385 2023-04-16 04:09:21.000000 pinstall-1.3/pinstall/pinstall.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      775 2023-04-13 07:15:57.000000 pinstall-1.3/pinstall/run.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-05-23 04:05:38.377558 pinstall-1.3/pinstall.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     7077 2023-05-23 04:05:38.000000 pinstall-1.3/pinstall.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      374 2023-05-23 04:05:38.000000 pinstall-1.3/pinstall.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-05-23 04:05:38.000000 pinstall-1.3/pinstall.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       52 2023-05-23 04:05:38.000000 pinstall-1.3/pinstall.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       13 2023-05-23 04:05:38.000000 pinstall-1.3/pinstall.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       27 2023-05-23 04:05:38.000000 pinstall-1.3/pinstall.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       38 2023-05-23 04:05:38.380892 pinstall-1.3/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1062 2023-05-23 04:02:34.000000 pinstall-1.3/setup.py
```

### Comparing `pinstall-1.2/PKG-INFO` & `pinstall-1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinstall
-Version: 1.2
+Version: 1.3
 Summary: Installer Tool for Python Programs
 Home-page: https://github.com/bulletmark/pinstall
 Author: Mark Blakeney
 Author-email: mark.blakeney@bullet-systems.net
 License: GPLv3
 Keywords: venv virtualenv systemd service
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pinstall-1.2/README.md` & `pinstall-1.3/README.md`

 * *Files identical despite different names*

### Comparing `pinstall-1.2/pinstall/commands/service.py` & `pinstall-1.3/pinstall/commands/service.py`

 * *Files identical despite different names*

### Comparing `pinstall-1.2/pinstall/commands/status.py` & `pinstall-1.3/pinstall/commands/status.py`

 * *Files identical despite different names*

### Comparing `pinstall-1.2/pinstall/commands/venv.py` & `pinstall-1.3/pinstall/commands/venv.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     parser.add_argument('-r', '--no-require', action='store_true',
                         help='don\'t pip install packages from '
                         'requirements.txt')
     parser.add_argument('-u', '--no-upgrade', action='store_true',
                         help='don\'t upgrade pip/setuptools in venv')
     parser.add_argument('-w', '--no-wheel', action='store_true',
                         help='don\'t install wheel in venv')
-    parser.add_argument('-v', '--verbose', action='count',
+    parser.add_argument('-v', '--verbose', action='count', default=0,
                         help='verbose pip install (can add multiple times to '
                         'increase verbosity)')
     parser.add_argument('args', nargs='*',
                         help='optional arguments to python -m venv '
                         '(add by starting with "--"). See options in '
                         '`python -m venv -h`')
```

### Comparing `pinstall-1.2/pinstall/pinstall.py` & `pinstall-1.3/pinstall/pinstall.py`

 * *Files identical despite different names*

### Comparing `pinstall-1.2/pinstall/run.py` & `pinstall-1.3/pinstall/run.py`

 * *Files identical despite different names*

### Comparing `pinstall-1.2/pinstall.egg-info/PKG-INFO` & `pinstall-1.3/pinstall.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinstall
-Version: 1.2
+Version: 1.3
 Summary: Installer Tool for Python Programs
 Home-page: https://github.com/bulletmark/pinstall
 Author: Mark Blakeney
 Author-email: mark.blakeney@bullet-systems.net
 License: GPLv3
 Keywords: venv virtualenv systemd service
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pinstall-1.2/setup.py` & `pinstall-1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 name = 'pinstall'
 module = name.replace('-', '_')
 here = Path(__file__).resolve().parent
 
 setup(
     name=name,
-    version='1.2',
+    version='1.3',
     description='Installer Tool for Python Programs',
     long_description=here.joinpath('README.md').read_text(),
     long_description_content_type='text/markdown',
     url=f'https://github.com/bulletmark/{name}',
     author='Mark Blakeney',
     author_email='mark.blakeney@bullet-systems.net',
     keywords='venv virtualenv systemd service',
```

