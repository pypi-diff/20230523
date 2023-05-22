# Comparing `tmp/tgbox-cli-0.1.1.tar.gz` & `tmp/tgbox-cli-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgbox-cli-0.1.1.tar", last modified: Fri Apr 28 21:09:14 2023, max compression
+gzip compressed data, was "tgbox-cli-1.0.tar", last modified: Mon May 22 21:59:56 2023, max compression
```

## Comparing `tgbox-cli-0.1.1.tar` & `tgbox-cli-1.0.tar`

### file list

```diff
@@ -1,15 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:09:14.032647 tgbox-cli-0.1.1/
--rw-r--r--   0 root         (0) root         (0)      845 2023-04-28 21:09:14.028647 tgbox-cli-0.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 21:09:14.032647 tgbox-cli-0.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1480 2023-04-28 21:08:38.000000 tgbox-cli-0.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:09:14.024647 tgbox-cli-0.1.1/tgbox_cli/
--rwxr-xr-x   0 root         (0) root         (0)    41172 2023-04-28 21:08:38.000000 tgbox-cli-0.1.1/tgbox_cli/tgbox_cli.py
--rw-r--r--   0 root         (0) root         (0)     3677 2023-04-28 21:08:38.000000 tgbox-cli-0.1.1/tgbox_cli/tools.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-28 21:08:38.000000 tgbox-cli-0.1.1/tgbox_cli/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:09:14.028647 tgbox-cli-0.1.1/tgbox_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      845 2023-04-28 21:09:13.000000 tgbox-cli-0.1.1/tgbox_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      271 2023-04-28 21:09:13.000000 tgbox-cli-0.1.1/tgbox_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 21:09:13.000000 tgbox-cli-0.1.1/tgbox_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       92 2023-04-28 21:09:13.000000 tgbox-cli-0.1.1/tgbox_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-04-28 21:09:13.000000 tgbox-cli-0.1.1/tgbox_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-28 21:09:13.000000 tgbox-cli-0.1.1/tgbox_cli.egg-info/top_level.txt
+drwxr-xr-x   0 non       (1000) non       (1000)        0 2023-05-22 21:59:56.004062 tgbox-cli-1.0/
+-rw-r--r--   0 non       (1000) non       (1000)       35 2023-04-28 22:25:05.000000 tgbox-cli-1.0/MANIFEST.in
+-rw-r--r--   0 non       (1000) non       (1000)     4542 2023-05-22 21:59:56.000062 tgbox-cli-1.0/PKG-INFO
+-rw-r--r--   0 non       (1000) non       (1000)     3015 2023-05-21 21:01:51.000000 tgbox-cli-1.0/README.md
+-rw-r--r--   0 non       (1000) non       (1000)       38 2023-05-22 21:59:56.004062 tgbox-cli-1.0/setup.cfg
+-rw-r--r--   0 non       (1000) non       (1000)     1713 2023-05-22 21:59:39.000000 tgbox-cli-1.0/setup.py
+drwxr-xr-x   0 non       (1000) non       (1000)        0 2023-05-22 21:59:55.968061 tgbox-cli-1.0/tgbox_cli/
+-rw-r--r--   0 non       (1000) non       (1000)        0 2023-04-28 22:25:05.000000 tgbox-cli-1.0/tgbox_cli/__init__.py
+drwxr-xr-x   0 non       (1000) non       (1000)        0 2023-05-22 21:59:55.992062 tgbox-cli-1.0/tgbox_cli/data/
+-rw-r--r--   0 non       (1000) non       (1000)    35898 2023-05-21 01:12:54.000000 tgbox-cli-1.0/tgbox_cli/data/help.txt
+-rw-r--r--   0 non       (1000) non       (1000)   105651 2023-04-28 22:25:05.000000 tgbox-cli-1.0/tgbox_cli/data/logo.ico
+-rw-r--r--   0 non       (1000) non       (1000)     1685 2023-05-22 21:12:40.000000 tgbox-cli-1.0/tgbox_cli/session.py
+-rwxr-xr-x   0 non       (1000) non       (1000)    95907 2023-05-22 21:12:29.000000 tgbox-cli-1.0/tgbox_cli/tgbox_cli.py
+-rw-r--r--   0 non       (1000) non       (1000)     9495 2023-05-13 23:05:14.000000 tgbox-cli-1.0/tgbox_cli/tools.py
+-rw-r--r--   0 non       (1000) non       (1000)       16 2023-05-22 21:59:39.000000 tgbox-cli-1.0/tgbox_cli/version.py
+drwxr-xr-x   0 non       (1000) non       (1000)        0 2023-05-22 21:59:55.972061 tgbox-cli-1.0/tgbox_cli.egg-info/
+-rw-r--r--   0 non       (1000) non       (1000)     4542 2023-05-22 21:59:55.000000 tgbox-cli-1.0/tgbox_cli.egg-info/PKG-INFO
+-rw-r--r--   0 non       (1000) non       (1000)      384 2023-05-22 21:59:55.000000 tgbox-cli-1.0/tgbox_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 non       (1000) non       (1000)        1 2023-05-22 21:59:55.000000 tgbox-cli-1.0/tgbox_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 non       (1000) non       (1000)       92 2023-05-22 21:59:55.000000 tgbox-cli-1.0/tgbox_cli.egg-info/entry_points.txt
+-rw-r--r--   0 non       (1000) non       (1000)       69 2023-05-22 21:59:55.000000 tgbox-cli-1.0/tgbox_cli.egg-info/requires.txt
+-rw-r--r--   0 non       (1000) non       (1000)       10 2023-05-22 21:59:55.000000 tgbox-cli-1.0/tgbox_cli.egg-info/top_level.txt
```

### Comparing `tgbox-cli-0.1.1/setup.py` & `tgbox-cli-1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,47 @@
 from setuptools import setup
 from ast import literal_eval
 
 with open('tgbox_cli/version.py', encoding='utf-8') as f:
-    version = literal_eval(f.read().split('=',1)[1].strip())
+    version = literal_eval(f.read().split('=')[1].strip())
 
 setup(
     name             = "tgbox-cli",
     version          = version,
     packages         = ['tgbox_cli'],
     license          = 'MIT',
     description      = 'A Command Line Interface to the TGBOX',
+    long_description = open('README.md', encoding='utf-8').read(),
     author           = 'NotStatilko',
     author_email     = 'thenonproton@pm.me',
     url              = 'https://github.com/NotStatilko/tgbox-cli',
     download_url     = f'https://github.com/NotStatilko/tgbox-cli/archive/refs/tags/v{version}.tar.gz',
 
+    long_description_content_type='text/markdown',
+
+    package_data = {
+        'tgbox_cli': ['tgbox_cli/data'],
+    },
+    include_package_data = True,
+
     install_requires=[
         'urllib3',
-        'tgbox<1',
+        'tgbox<2',
         'click==8.1.3',
         'enlighten==1.10.2'
     ],
     extras_require={
-        'fast': ['tgbox[fast]<1']
+        'fast': ['tgbox[fast]<2']
     },
     keywords = [
         'Telegram', 'Cloud-Storage',
         'Cloud', 'Non-official'
     ],
     classifiers = [
-        'Development Status :: 4 - Beta',
+        'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Intended Audience :: End Users/Desktop',
         'Topic :: Security :: Cryptography',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
```

