# Comparing `tmp/venv-modulefile-0.1.0.tar.gz` & `tmp/venv-modulefile-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/volatile/catA/rl222169/softs/custom_venv/venv-modulefile/dist/tmpp6eu4o7a/venv-modulefile-0.1.0.tar", last modified: Tue May 23 14:27:08 2023, max compression
+gzip compressed data, was "/volatile/catA/rl222169/softs/custom_venv/venv-modulefile/dist/tmpf2iq8d1m/venv-modulefile-0.1.1.tar", last modified: Tue May 23 15:19:45 2023, max compression
```

## Comparing `venv-modulefile-0.1.0.tar` & `venv-modulefile-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-23 14:27:08.000000 venv-modulefile-0.1.0/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2942 2023-05-23 14:27:08.000000 venv-modulefile-0.1.0/PKG-INFO
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       81 2023-05-04 08:19:39.000000 venv-modulefile-0.1.0/pyproject.toml
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       38 2023-05-23 14:27:08.000000 venv-modulefile-0.1.0/setup.cfg
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       22 2023-04-19 16:42:18.000000 venv-modulefile-0.1.0/MANIFEST.in
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      959 2023-05-22 14:55:50.000000 venv-modulefile-0.1.0/README.md
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     9608 2023-05-22 10:27:41.000000 venv-modulefile-0.1.0/setup.py
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-23 14:27:08.000000 venv-modulefile-0.1.0/src/
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-23 14:27:08.000000 venv-modulefile-0.1.0/src/venvmod/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        6 2023-05-23 14:25:55.000000 venv-modulefile-0.1.0/src/venvmod/VERSION
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      247 2023-05-23 10:47:49.000000 venv-modulefile-0.1.0/src/venvmod/__init__.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2984 2023-05-23 12:42:56.000000 venv-modulefile-0.1.0/src/venvmod/tools.py
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-23 14:27:08.000000 venv-modulefile-0.1.0/src/venvmod/commands/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1713 2023-05-23 14:21:45.000000 venv-modulefile-0.1.0/src/venvmod/commands/test_imports.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     3522 2023-05-23 14:02:10.000000 venv-modulefile-0.1.0/src/venvmod/commands/__init__.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     5185 2023-05-23 14:00:38.000000 venv-modulefile-0.1.0/src/venvmod/commands/create_module.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    10169 2023-05-23 13:58:47.000000 venv-modulefile-0.1.0/src/venvmod/commands/append_module.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    13105 2023-05-23 14:13:14.000000 venv-modulefile-0.1.0/src/venvmod/modulefile.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1798 2023-05-22 15:00:27.000000 venv-modulefile-0.1.0/src/README.md
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-23 14:27:08.000000 venv-modulefile-0.1.0/src/venv_modulefile.egg-info/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      809 2023-05-23 14:27:08.000000 venv-modulefile-0.1.0/src/venv_modulefile.egg-info/entry_points.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        8 2023-05-23 14:27:08.000000 venv-modulefile-0.1.0/src/venv_modulefile.egg-info/top_level.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      567 2023-05-23 14:27:08.000000 venv-modulefile-0.1.0/src/venv_modulefile.egg-info/SOURCES.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2942 2023-05-23 14:27:08.000000 venv-modulefile-0.1.0/src/venv_modulefile.egg-info/PKG-INFO
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        1 2023-05-23 14:27:08.000000 venv-modulefile-0.1.0/src/venv_modulefile.egg-info/dependency_links.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      241 2023-05-23 14:27:08.000000 venv-modulefile-0.1.0/src/venv_modulefile.egg-info/requires.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1302 2023-05-04 08:19:39.000000 venv-modulefile-0.1.0/LICENSE.md
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-23 15:19:45.000000 venv-modulefile-0.1.1/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     4047 2023-05-23 15:19:45.000000 venv-modulefile-0.1.1/PKG-INFO
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       81 2023-05-04 08:19:39.000000 venv-modulefile-0.1.1/pyproject.toml
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       38 2023-05-23 15:19:45.000000 venv-modulefile-0.1.1/setup.cfg
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       22 2023-04-19 16:42:18.000000 venv-modulefile-0.1.1/MANIFEST.in
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      959 2023-05-22 14:55:50.000000 venv-modulefile-0.1.1/README.md
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     9608 2023-05-22 10:27:41.000000 venv-modulefile-0.1.1/setup.py
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-23 15:19:45.000000 venv-modulefile-0.1.1/src/
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-23 15:19:45.000000 venv-modulefile-0.1.1/src/venvmod/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        6 2023-05-23 15:19:14.000000 venv-modulefile-0.1.1/src/venvmod/VERSION
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      247 2023-05-23 10:47:49.000000 venv-modulefile-0.1.1/src/venvmod/__init__.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2984 2023-05-23 12:42:56.000000 venv-modulefile-0.1.1/src/venvmod/tools.py
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-23 15:19:45.000000 venv-modulefile-0.1.1/src/venvmod/commands/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1713 2023-05-23 14:21:45.000000 venv-modulefile-0.1.1/src/venvmod/commands/test_imports.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     3467 2023-05-23 14:58:07.000000 venv-modulefile-0.1.1/src/venvmod/commands/__init__.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     5185 2023-05-23 14:00:38.000000 venv-modulefile-0.1.1/src/venvmod/commands/create_module.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    10056 2023-05-23 14:58:12.000000 venv-modulefile-0.1.1/src/venvmod/commands/append_module.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    12965 2023-05-23 14:57:37.000000 venv-modulefile-0.1.1/src/venvmod/modulefile.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2903 2023-05-23 15:18:04.000000 venv-modulefile-0.1.1/src/README.md
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-23 15:19:45.000000 venv-modulefile-0.1.1/src/venv_modulefile.egg-info/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      809 2023-05-23 15:19:45.000000 venv-modulefile-0.1.1/src/venv_modulefile.egg-info/entry_points.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        8 2023-05-23 15:19:45.000000 venv-modulefile-0.1.1/src/venv_modulefile.egg-info/top_level.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      567 2023-05-23 15:19:45.000000 venv-modulefile-0.1.1/src/venv_modulefile.egg-info/SOURCES.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     4047 2023-05-23 15:19:45.000000 venv-modulefile-0.1.1/src/venv_modulefile.egg-info/PKG-INFO
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        1 2023-05-23 15:19:45.000000 venv-modulefile-0.1.1/src/venv_modulefile.egg-info/dependency_links.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      241 2023-05-23 15:19:45.000000 venv-modulefile-0.1.1/src/venv_modulefile.egg-info/requires.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1302 2023-05-04 08:19:39.000000 venv-modulefile-0.1.1/LICENSE.md
```

### Comparing `venv-modulefile-0.1.0/README.md` & `venv-modulefile-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.0/setup.py` & `venv-modulefile-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.0/src/venvmod/tools.py` & `venv-modulefile-0.1.1/src/venvmod/tools.py`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.0/src/venvmod/commands/test_imports.py` & `venv-modulefile-0.1.1/src/venvmod/commands/test_imports.py`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.0/src/venvmod/commands/__init__.py` & `venv-modulefile-0.1.1/src/venvmod/commands/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,15 +44,14 @@
     parser.add_argument('--verbose', action='store_true', help='To display the result.')
 
     if with_appli:
         parser.add_argument('--appli', metavar='appli', default="",
                             help='Name of the appli modulefile (case insensitive)')
     if positionals:
         for positional in positionals:
-            print("get_parser positional", positional)
             parser.add_argument(positional[0],
                                 metavar=positional[0].replace("-", "_"),
                                 default=positional[1],
                                 help=positional[2],
                                 nargs=positional[3])
 
     if options:
```

### Comparing `venv-modulefile-0.1.0/src/venvmod/commands/create_module.py` & `venv-modulefile-0.1.1/src/venvmod/commands/create_module.py`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.0/src/venvmod/commands/append_module.py` & `venv-modulefile-0.1.1/src/venvmod/commands/append_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,17 +223,14 @@
     else:
         virtual_env, appli = arguments
 
     # List env vars
     appli_env_vars = {envvar: value for envvar, value in os.environ.items()
                       if get_std_name(envvar).startswith(appli.replace('.', '_'))}
 
-    print(f"read_env: os.environ = '{os.environ}'")
-    print(f"read_env: appli_env_vars = '{appli_env_vars}'")
-
     logger.debug("read_env: os.environ = '%s'", os.environ)
     logger.debug("read_env: appli_env_vars = '%s'", appli_env_vars)
 
     # Source file in first
     for envvar, value in appli_env_vars.items():
         if envvar.endswith("SOURCEFILES"):
             for var in value.split(";"):
```

### Comparing `venv-modulefile-0.1.0/src/venvmod/modulefile.py` & `venv-modulefile-0.1.1/src/venvmod/modulefile.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,17 +56,14 @@
 
     Returns
     -------
     str
         version as 'x.y.z', '0.0.0' if not found
     """
     result = get_process_result(command="module --version", capture_output=True)
-    print(f"get_version: {result}")
-    print(f"get_version: {result.stderr.decode()}")
-    print(f"get_version: {result.stdout.decode()}")
     logger.debug(f"get_version: {result}")
     logger.debug(f"get_version: {result.stderr.decode()}")
     logger.debug(f"get_version: {result.stdout.decode()}")
     if 'VERSION=' in result.stderr.decode().split()[0]: # version < 4.0
         return result.stderr.decode().split()[0].split("=")[1]
     if 'Modules' == result.stderr.decode().split()[0]:
         return result.stderr.decode().split()[2]
```

### Comparing `venv-modulefile-0.1.0/src/venv_modulefile.egg-info/entry_points.txt` & `venv-modulefile-0.1.1/src/venv_modulefile.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.0/src/venv_modulefile.egg-info/SOURCES.txt` & `venv-modulefile-0.1.1/src/venv_modulefile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.0/LICENSE.md` & `venv-modulefile-0.1.1/LICENSE.md`

 * *Files identical despite different names*

