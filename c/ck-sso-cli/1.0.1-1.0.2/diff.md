# Comparing `tmp/ck-sso-cli-1.0.1.tar.gz` & `tmp/ck-sso-cli-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ck-sso-cli-1.0.1.tar", last modified: Tue May 23 04:50:24 2023, max compression
+gzip compressed data, was "ck-sso-cli-1.0.2.tar", last modified: Tue May 23 07:56:18 2023, max compression
```

## Comparing `ck-sso-cli-1.0.1.tar` & `ck-sso-cli-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 aditya     (501) staff       (20)        0 2023-05-23 04:50:24.809671 ck-sso-cli-1.0.1/
--rw-r--r--   0 aditya     (501) staff       (20)    11353 2023-05-23 04:44:11.000000 ck-sso-cli-1.0.1/LICENSE
--rw-r--r--   0 aditya     (501) staff       (20)      343 2023-05-23 04:50:24.809528 ck-sso-cli-1.0.1/PKG-INFO
--rw-r--r--   0 aditya     (501) staff       (20)     4602 2023-05-23 04:44:11.000000 ck-sso-cli-1.0.1/README.md
-drwxr-xr-x   0 aditya     (501) staff       (20)        0 2023-05-23 04:50:24.808144 ck-sso-cli-1.0.1/ck_sso_cli.egg-info/
--rw-r--r--   0 aditya     (501) staff       (20)      343 2023-05-23 04:50:24.000000 ck-sso-cli-1.0.1/ck_sso_cli.egg-info/PKG-INFO
--rw-r--r--   0 aditya     (501) staff       (20)      366 2023-05-23 04:50:24.000000 ck-sso-cli-1.0.1/ck_sso_cli.egg-info/SOURCES.txt
--rw-r--r--   0 aditya     (501) staff       (20)        1 2023-05-23 04:50:24.000000 ck-sso-cli-1.0.1/ck_sso_cli.egg-info/dependency_links.txt
--rw-r--r--   0 aditya     (501) staff       (20)       57 2023-05-23 04:50:24.000000 ck-sso-cli-1.0.1/ck_sso_cli.egg-info/entry_points.txt
--rw-r--r--   0 aditya     (501) staff       (20)        6 2023-05-23 04:50:24.000000 ck-sso-cli-1.0.1/ck_sso_cli.egg-info/requires.txt
--rw-r--r--   0 aditya     (501) staff       (20)        9 2023-05-23 04:50:24.000000 ck-sso-cli-1.0.1/ck_sso_cli.egg-info/top_level.txt
-drwxr-xr-x   0 aditya     (501) staff       (20)        0 2023-05-23 04:50:24.809284 ck-sso-cli-1.0.1/ckssocli/
--rw-r--r--   0 aditya     (501) staff       (20)       45 2023-05-23 04:44:11.000000 ck-sso-cli-1.0.1/ckssocli/__init__.py
--rw-r--r--   0 aditya     (501) staff       (20)     2312 2023-05-23 04:49:10.000000 ck-sso-cli-1.0.1/ckssocli/ck_configuration.py
--rw-r--r--   0 aditya     (501) staff       (20)      496 2023-05-23 04:44:11.000000 ck-sso-cli-1.0.1/ckssocli/ck_help.py
--rw-r--r--   0 aditya     (501) staff       (20)     3842 2023-05-23 04:46:21.000000 ck-sso-cli-1.0.1/ckssocli/ck_login.py
--rw-r--r--   0 aditya     (501) staff       (20)      796 2023-05-23 04:44:11.000000 ck-sso-cli-1.0.1/ckssocli/ck_sso_cli.py
--rw-r--r--   0 aditya     (501) staff       (20)       44 2023-05-23 04:48:49.000000 ck-sso-cli-1.0.1/ckssocli/version.py
--rw-r--r--   0 aditya     (501) staff       (20)       38 2023-05-23 04:50:24.809734 ck-sso-cli-1.0.1/setup.cfg
--rw-r--r--   0 aditya     (501) staff       (20)      728 2023-05-23 04:44:11.000000 ck-sso-cli-1.0.1/setup.py
+drwxr-xr-x   0 aditya     (501) staff       (20)        0 2023-05-23 07:56:18.614595 ck-sso-cli-1.0.2/
+-rw-r--r--   0 aditya     (501) staff       (20)    11353 2023-05-23 04:44:11.000000 ck-sso-cli-1.0.2/LICENSE
+-rw-r--r--   0 aditya     (501) staff       (20)      328 2023-05-23 07:56:18.614468 ck-sso-cli-1.0.2/PKG-INFO
+-rw-r--r--   0 aditya     (501) staff       (20)     4602 2023-05-23 04:44:11.000000 ck-sso-cli-1.0.2/README.md
+drwxr-xr-x   0 aditya     (501) staff       (20)        0 2023-05-23 07:56:18.613145 ck-sso-cli-1.0.2/ck_sso_cli.egg-info/
+-rw-r--r--   0 aditya     (501) staff       (20)      328 2023-05-23 07:56:18.000000 ck-sso-cli-1.0.2/ck_sso_cli.egg-info/PKG-INFO
+-rw-r--r--   0 aditya     (501) staff       (20)      366 2023-05-23 07:56:18.000000 ck-sso-cli-1.0.2/ck_sso_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 aditya     (501) staff       (20)        1 2023-05-23 07:56:18.000000 ck-sso-cli-1.0.2/ck_sso_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 aditya     (501) staff       (20)       57 2023-05-23 07:56:18.000000 ck-sso-cli-1.0.2/ck_sso_cli.egg-info/entry_points.txt
+-rw-r--r--   0 aditya     (501) staff       (20)        6 2023-05-23 07:56:18.000000 ck-sso-cli-1.0.2/ck_sso_cli.egg-info/requires.txt
+-rw-r--r--   0 aditya     (501) staff       (20)        9 2023-05-23 07:56:18.000000 ck-sso-cli-1.0.2/ck_sso_cli.egg-info/top_level.txt
+drwxr-xr-x   0 aditya     (501) staff       (20)        0 2023-05-23 07:56:18.614263 ck-sso-cli-1.0.2/ckssocli/
+-rw-r--r--   0 aditya     (501) staff       (20)       45 2023-05-23 04:44:11.000000 ck-sso-cli-1.0.2/ckssocli/__init__.py
+-rw-r--r--   0 aditya     (501) staff       (20)     2312 2023-05-23 04:49:10.000000 ck-sso-cli-1.0.2/ckssocli/ck_configuration.py
+-rw-r--r--   0 aditya     (501) staff       (20)      496 2023-05-23 04:44:11.000000 ck-sso-cli-1.0.2/ckssocli/ck_help.py
+-rw-r--r--   0 aditya     (501) staff       (20)     4998 2023-05-23 07:55:42.000000 ck-sso-cli-1.0.2/ckssocli/ck_login.py
+-rw-r--r--   0 aditya     (501) staff       (20)      796 2023-05-23 04:44:11.000000 ck-sso-cli-1.0.2/ckssocli/ck_sso_cli.py
+-rw-r--r--   0 aditya     (501) staff       (20)       44 2023-05-23 07:54:28.000000 ck-sso-cli-1.0.2/ckssocli/version.py
+-rw-r--r--   0 aditya     (501) staff       (20)       38 2023-05-23 07:56:18.614647 ck-sso-cli-1.0.2/setup.cfg
+-rw-r--r--   0 aditya     (501) staff       (20)      713 2023-05-23 04:59:14.000000 ck-sso-cli-1.0.2/setup.py
```

### Comparing `ck-sso-cli-1.0.1/LICENSE` & `ck-sso-cli-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ck-sso-cli-1.0.1/README.md` & `ck-sso-cli-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ck-sso-cli-1.0.1/ckssocli/ck_configuration.py` & `ck-sso-cli-1.0.2/ckssocli/ck_configuration.py`

 * *Files identical despite different names*

### Comparing `ck-sso-cli-1.0.1/ckssocli/ck_sso_cli.py` & `ck-sso-cli-1.0.2/ckssocli/ck_sso_cli.py`

 * *Files identical despite different names*

### Comparing `ck-sso-cli-1.0.1/setup.py` & `ck-sso-cli-1.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     name='ck-sso-cli',
     version=__version__,
     description='Provides a wrapper for AWS IAM Identity Center authentication to an External AWS Account',
     packages=find_packages(),
     license='Apache License 2.0',
     author='Aditya Ajay',
     author_email='aditya.ajay@tothenew.com',
-    url='https://github.com/okta-awscli/okta-awscli',
+    url='https://www.cloudkeeper.ai/',
     entry_points={
         'console_scripts': [
             'ck-sso-cli=ckssocli.ck_sso_cli:main',
         ],
     },
     install_requires=[
         'boto3'
```

