# Comparing `tmp/ck-sso-cli-1.0.0.tar.gz` & `tmp/ck-sso-cli-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ck-sso-cli-1.0.0.tar", last modified: Tue Nov  8 06:24:03 2022, max compression
+gzip compressed data, was "ck-sso-cli-1.0.1.tar", last modified: Tue May 23 04:50:24 2023, max compression
```

## Comparing `ck-sso-cli-1.0.0.tar` & `ck-sso-cli-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 aditya    (1000) aditya    (1000)        0 2022-11-08 06:24:03.295432 ck-sso-cli-1.0.0/
--rw-rw-r--   0 aditya    (1000) aditya    (1000)    11353 2022-11-07 09:14:00.000000 ck-sso-cli-1.0.0/LICENSE
--rw-rw-r--   0 aditya    (1000) aditya    (1000)      315 2022-11-08 06:24:03.295432 ck-sso-cli-1.0.0/PKG-INFO
--rw-rw-r--   0 aditya    (1000) aditya    (1000)     4602 2022-11-08 06:22:45.000000 ck-sso-cli-1.0.0/README.md
-drwxrwxr-x   0 aditya    (1000) aditya    (1000)        0 2022-11-08 06:24:03.295432 ck-sso-cli-1.0.0/ck_sso_cli.egg-info/
--rw-rw-r--   0 aditya    (1000) aditya    (1000)      315 2022-11-08 06:24:03.000000 ck-sso-cli-1.0.0/ck_sso_cli.egg-info/PKG-INFO
--rw-rw-r--   0 aditya    (1000) aditya    (1000)      366 2022-11-08 06:24:03.000000 ck-sso-cli-1.0.0/ck_sso_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 aditya    (1000) aditya    (1000)        1 2022-11-08 06:24:03.000000 ck-sso-cli-1.0.0/ck_sso_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 aditya    (1000) aditya    (1000)       56 2022-11-08 06:24:03.000000 ck-sso-cli-1.0.0/ck_sso_cli.egg-info/entry_points.txt
--rw-rw-r--   0 aditya    (1000) aditya    (1000)        6 2022-11-08 06:24:03.000000 ck-sso-cli-1.0.0/ck_sso_cli.egg-info/requires.txt
--rw-rw-r--   0 aditya    (1000) aditya    (1000)        9 2022-11-08 06:24:03.000000 ck-sso-cli-1.0.0/ck_sso_cli.egg-info/top_level.txt
-drwxrwxr-x   0 aditya    (1000) aditya    (1000)        0 2022-11-08 06:24:03.295432 ck-sso-cli-1.0.0/ckssocli/
--rw-rw-r--   0 aditya    (1000) aditya    (1000)       45 2022-11-07 09:32:13.000000 ck-sso-cli-1.0.0/ckssocli/__init__.py
--rw-rw-r--   0 aditya    (1000) aditya    (1000)     2281 2022-11-07 18:18:09.000000 ck-sso-cli-1.0.0/ckssocli/ck_configuration.py
--rw-rw-r--   0 aditya    (1000) aditya    (1000)      496 2022-11-07 15:24:56.000000 ck-sso-cli-1.0.0/ckssocli/ck_help.py
--rw-rw-r--   0 aditya    (1000) aditya    (1000)     3811 2022-11-07 18:34:14.000000 ck-sso-cli-1.0.0/ckssocli/ck_login.py
--rw-rw-r--   0 aditya    (1000) aditya    (1000)      796 2022-11-07 14:22:53.000000 ck-sso-cli-1.0.0/ckssocli/ck_sso_cli.py
--rw-rw-r--   0 aditya    (1000) aditya    (1000)       44 2022-11-08 06:23:54.000000 ck-sso-cli-1.0.0/ckssocli/version.py
--rw-rw-r--   0 aditya    (1000) aditya    (1000)       38 2022-11-08 06:24:03.295432 ck-sso-cli-1.0.0/setup.cfg
--rw-rw-r--   0 aditya    (1000) aditya    (1000)      728 2022-11-07 15:49:38.000000 ck-sso-cli-1.0.0/setup.py
+drwxr-xr-x   0 aditya     (501) staff       (20)        0 2023-05-23 04:50:24.809671 ck-sso-cli-1.0.1/
+-rw-r--r--   0 aditya     (501) staff       (20)    11353 2023-05-23 04:44:11.000000 ck-sso-cli-1.0.1/LICENSE
+-rw-r--r--   0 aditya     (501) staff       (20)      343 2023-05-23 04:50:24.809528 ck-sso-cli-1.0.1/PKG-INFO
+-rw-r--r--   0 aditya     (501) staff       (20)     4602 2023-05-23 04:44:11.000000 ck-sso-cli-1.0.1/README.md
+drwxr-xr-x   0 aditya     (501) staff       (20)        0 2023-05-23 04:50:24.808144 ck-sso-cli-1.0.1/ck_sso_cli.egg-info/
+-rw-r--r--   0 aditya     (501) staff       (20)      343 2023-05-23 04:50:24.000000 ck-sso-cli-1.0.1/ck_sso_cli.egg-info/PKG-INFO
+-rw-r--r--   0 aditya     (501) staff       (20)      366 2023-05-23 04:50:24.000000 ck-sso-cli-1.0.1/ck_sso_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 aditya     (501) staff       (20)        1 2023-05-23 04:50:24.000000 ck-sso-cli-1.0.1/ck_sso_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 aditya     (501) staff       (20)       57 2023-05-23 04:50:24.000000 ck-sso-cli-1.0.1/ck_sso_cli.egg-info/entry_points.txt
+-rw-r--r--   0 aditya     (501) staff       (20)        6 2023-05-23 04:50:24.000000 ck-sso-cli-1.0.1/ck_sso_cli.egg-info/requires.txt
+-rw-r--r--   0 aditya     (501) staff       (20)        9 2023-05-23 04:50:24.000000 ck-sso-cli-1.0.1/ck_sso_cli.egg-info/top_level.txt
+drwxr-xr-x   0 aditya     (501) staff       (20)        0 2023-05-23 04:50:24.809284 ck-sso-cli-1.0.1/ckssocli/
+-rw-r--r--   0 aditya     (501) staff       (20)       45 2023-05-23 04:44:11.000000 ck-sso-cli-1.0.1/ckssocli/__init__.py
+-rw-r--r--   0 aditya     (501) staff       (20)     2312 2023-05-23 04:49:10.000000 ck-sso-cli-1.0.1/ckssocli/ck_configuration.py
+-rw-r--r--   0 aditya     (501) staff       (20)      496 2023-05-23 04:44:11.000000 ck-sso-cli-1.0.1/ckssocli/ck_help.py
+-rw-r--r--   0 aditya     (501) staff       (20)     3842 2023-05-23 04:46:21.000000 ck-sso-cli-1.0.1/ckssocli/ck_login.py
+-rw-r--r--   0 aditya     (501) staff       (20)      796 2023-05-23 04:44:11.000000 ck-sso-cli-1.0.1/ckssocli/ck_sso_cli.py
+-rw-r--r--   0 aditya     (501) staff       (20)       44 2023-05-23 04:48:49.000000 ck-sso-cli-1.0.1/ckssocli/version.py
+-rw-r--r--   0 aditya     (501) staff       (20)       38 2023-05-23 04:50:24.809734 ck-sso-cli-1.0.1/setup.cfg
+-rw-r--r--   0 aditya     (501) staff       (20)      728 2023-05-23 04:44:11.000000 ck-sso-cli-1.0.1/setup.py
```

### Comparing `ck-sso-cli-1.0.0/LICENSE` & `ck-sso-cli-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ck-sso-cli-1.0.0/README.md` & `ck-sso-cli-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ck-sso-cli-1.0.0/ckssocli/ck_configuration.py` & `ck-sso-cli-1.0.1/ckssocli/ck_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import json
 import subprocess
 import os
 
 
 def configure_utility():
     # Retrieving the directory where .ck-sso-cli/ folder is present
-    directory = subprocess.run(['pwd'], capture_output=True)
+    cmd = 'echo $HOME'
+    directory = subprocess.run(cmd, shell=True, capture_output=True)
     directory = directory.stdout.decode('utf-8')
     directory = directory.split('\n')
     directory = directory[0]
 
     # Setting the profile
 
     profile = 'default'
```

### Comparing `ck-sso-cli-1.0.0/ckssocli/ck_login.py` & `ck-sso-cli-1.0.1/ckssocli/ck_login.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import sys 
 import subprocess
 import json
 import boto3
 import os 
 
 def login_utility():
-    directory = subprocess.run(['pwd'], capture_output=True)
+    cmd = 'echo $HOME'
+    directory = subprocess.run(cmd, shell=True, capture_output=True)
     directory = directory.stdout.decode('utf-8')
     directory = directory.split('\n')
     directory = directory[0]
 
     profile = 'default'
 
     if len(sys.argv) == 2:
```

### Comparing `ck-sso-cli-1.0.0/ckssocli/ck_sso_cli.py` & `ck-sso-cli-1.0.1/ckssocli/ck_sso_cli.py`

 * *Files identical despite different names*

### Comparing `ck-sso-cli-1.0.0/setup.py` & `ck-sso-cli-1.0.1/setup.py`

 * *Files identical despite different names*

