# Comparing `tmp/venv-modulefile-0.0.8.tar.gz` & `tmp/venv-modulefile-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/volatile/catA/rl222169/softs/custom_venv/extend_python_venv_with_environment_modules/dist/tmp3w1inqb9/venv-modulefile-0.0.8.ta", last modified: Fri May  5 07:36:30 2023, max compression
+gzip compressed data, was "/volatile/catA/rl222169/softs/custom_venv/extend_python_venv_with_environment_modules/dist/tmpzq18jqg9/venv-modulefile-0.0.9.ta", last modified: Fri May  5 09:18:23 2023, max compression
```

## Comparing `venv-modulefile-0.0.8.tar` & `venv-modulefile-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-05 07:36:30.000000 venv-modulefile-0.0.8/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2042 2023-05-05 07:36:30.000000 venv-modulefile-0.0.8/PKG-INFO
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       81 2023-05-04 08:19:39.000000 venv-modulefile-0.0.8/pyproject.toml
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       38 2023-05-05 07:36:30.000000 venv-modulefile-0.0.8/setup.cfg
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       22 2023-04-19 16:42:18.000000 venv-modulefile-0.0.8/MANIFEST.in
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      898 2023-05-04 08:19:39.000000 venv-modulefile-0.0.8/README.md
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     9593 2023-05-04 08:46:54.000000 venv-modulefile-0.0.8/setup.py
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-05 07:36:30.000000 venv-modulefile-0.0.8/src/
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-05 07:36:30.000000 venv-modulefile-0.0.8/src/venvmod/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        6 2023-05-05 07:35:53.000000 venv-modulefile-0.0.8/src/venvmod/VERSION
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      232 2023-05-04 08:26:00.000000 venv-modulefile-0.0.8/src/venvmod/__init__.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2840 2023-05-04 10:36:26.000000 venv-modulefile-0.0.8/src/venvmod/tools.py
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-05 07:36:30.000000 venv-modulefile-0.0.8/src/venvmod/commands/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1539 2023-05-04 09:25:04.000000 venv-modulefile-0.0.8/src/venvmod/commands/test_imports.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2098 2023-05-04 09:28:22.000000 venv-modulefile-0.0.8/src/venvmod/commands/__init__.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     3897 2023-05-04 10:38:57.000000 venv-modulefile-0.0.8/src/venvmod/commands/create_module.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     8304 2023-05-04 10:38:37.000000 venv-modulefile-0.0.8/src/venvmod/commands/append_module.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    12262 2023-05-04 09:42:38.000000 venv-modulefile-0.0.8/src/venvmod/modulefile.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      898 2023-05-04 08:19:39.000000 venv-modulefile-0.0.8/src/README.md
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-05 07:36:30.000000 venv-modulefile-0.0.8/src/venv_modulefile.egg-info/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      809 2023-05-05 07:36:30.000000 venv-modulefile-0.0.8/src/venv_modulefile.egg-info/entry_points.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        8 2023-05-05 07:36:30.000000 venv-modulefile-0.0.8/src/venv_modulefile.egg-info/top_level.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      567 2023-05-05 07:36:30.000000 venv-modulefile-0.0.8/src/venv_modulefile.egg-info/SOURCES.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2042 2023-05-05 07:36:30.000000 venv-modulefile-0.0.8/src/venv_modulefile.egg-info/PKG-INFO
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        1 2023-05-05 07:36:30.000000 venv-modulefile-0.0.8/src/venv_modulefile.egg-info/dependency_links.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      229 2023-05-05 07:36:30.000000 venv-modulefile-0.0.8/src/venv_modulefile.egg-info/requires.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1302 2023-05-04 08:19:39.000000 venv-modulefile-0.0.8/LICENSE.md
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-05 09:18:23.000000 venv-modulefile-0.0.9/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2042 2023-05-05 09:18:23.000000 venv-modulefile-0.0.9/PKG-INFO
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       81 2023-05-04 08:19:39.000000 venv-modulefile-0.0.9/pyproject.toml
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       38 2023-05-05 09:18:23.000000 venv-modulefile-0.0.9/setup.cfg
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       22 2023-04-19 16:42:18.000000 venv-modulefile-0.0.9/MANIFEST.in
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      898 2023-05-04 08:19:39.000000 venv-modulefile-0.0.9/README.md
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     9593 2023-05-04 08:46:54.000000 venv-modulefile-0.0.9/setup.py
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-05 09:18:23.000000 venv-modulefile-0.0.9/src/
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-05 09:18:23.000000 venv-modulefile-0.0.9/src/venvmod/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        6 2023-05-05 09:17:55.000000 venv-modulefile-0.0.9/src/venvmod/VERSION
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      232 2023-05-04 08:26:00.000000 venv-modulefile-0.0.9/src/venvmod/__init__.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2840 2023-05-04 10:36:26.000000 venv-modulefile-0.0.9/src/venvmod/tools.py
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-05 09:18:23.000000 venv-modulefile-0.0.9/src/venvmod/commands/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1539 2023-05-04 09:25:04.000000 venv-modulefile-0.0.9/src/venvmod/commands/test_imports.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2571 2023-05-05 09:11:43.000000 venv-modulefile-0.0.9/src/venvmod/commands/__init__.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     4197 2023-05-05 09:14:33.000000 venv-modulefile-0.0.9/src/venvmod/commands/create_module.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     8304 2023-05-04 10:38:37.000000 venv-modulefile-0.0.9/src/venvmod/commands/append_module.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    12262 2023-05-04 09:42:38.000000 venv-modulefile-0.0.9/src/venvmod/modulefile.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      898 2023-05-04 08:19:39.000000 venv-modulefile-0.0.9/src/README.md
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-05 09:18:23.000000 venv-modulefile-0.0.9/src/venv_modulefile.egg-info/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      809 2023-05-05 09:18:23.000000 venv-modulefile-0.0.9/src/venv_modulefile.egg-info/entry_points.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        8 2023-05-05 09:18:23.000000 venv-modulefile-0.0.9/src/venv_modulefile.egg-info/top_level.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      567 2023-05-05 09:18:23.000000 venv-modulefile-0.0.9/src/venv_modulefile.egg-info/SOURCES.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2042 2023-05-05 09:18:23.000000 venv-modulefile-0.0.9/src/venv_modulefile.egg-info/PKG-INFO
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        1 2023-05-05 09:18:23.000000 venv-modulefile-0.0.9/src/venv_modulefile.egg-info/dependency_links.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      229 2023-05-05 09:18:23.000000 venv-modulefile-0.0.9/src/venv_modulefile.egg-info/requires.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1302 2023-05-04 08:19:39.000000 venv-modulefile-0.0.9/LICENSE.md
```

### Comparing `venv-modulefile-0.0.8/PKG-INFO` & `venv-modulefile-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: venv-modulefile
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python venv extension using Modulefile
 Home-page: https://github.com/roland-lenain/venv-modulefile
 Author: R. Lenain
 Author-email: roland.lenain@cea.fr
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/roland-lenain/venv-modulefile/issues
 Project-URL: Doc, https://venv-modulefile.readthedocs.io/en/latest/index.html
```

### Comparing `venv-modulefile-0.0.8/README.md` & `venv-modulefile-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.0.8/setup.py` & `venv-modulefile-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.0.8/src/venvmod/tools.py` & `venv-modulefile-0.0.9/src/venvmod/tools.py`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.0.8/src/venvmod/commands/test_imports.py` & `venv-modulefile-0.0.9/src/venvmod/commands/test_imports.py`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.0.8/src/venvmod/commands/__init__.py` & `venv-modulefile-0.0.9/src/venvmod/commands/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 import argparse
 from pathlib import Path
-from typing import List
+from typing import Any, List, Tuple
 
 from ..modulefile import get_module_file_directory
 
 def get_parser(description: str,
                help_arguments: str = None,
                with_appli: bool = False,
                with_verbose: bool = False,
+               options: List[Tuple[str, Any, str]] = None,
                args: List = None) -> argparse.Namespace:
     """Create a parser for entry-points.
 
     Parameters
     ----------
     description : str
         Description of the command
     help_arguments : str, optional
         Help for the arguments, by default None
     with_appli : bool, optional
         True to enable '--appli' option, by default False
     with_verbose : bool, optional
         True to enable '--verbise' option, by default False
+    options: List[Tuple[str, Any, str]], optional
+        list of options defined as ('--option-name', default, 'help'), by default None
     args : List, optional
         list of arguments if not given throug cli, by default None
 
     Returns
     -------
     argparse.Namespace
         parsed arguments
@@ -39,14 +42,21 @@
 
     if with_appli:
         parser.add_argument('--appli', metavar='appli', default="",
                         help='Name of the appli modulefile (case insensitive)')
     if help_arguments:
         parser.add_argument('arguments', nargs='+', default=[], help=help_arguments)
 
+    if options:
+        for option in options:
+            parser.add_argument(f"--{option[0]}",
+                                metavar=option[0].replace("-","_"),
+                                default=option[1],
+                                help=option[2])
+
     return parser.parse_args(args)
 
 def get_module_filename(virtual_env_name: str, appli_name: str = None) -> str:
     """_summary_
 
     Parameters
     ----------
```

### Comparing `venv-modulefile-0.0.8/src/venvmod/commands/create_module.py` & `venv-modulefile-0.0.9/src/venvmod/commands/create_module.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,19 +29,26 @@
     Returns
     -------
     int
         return code
     """
 
     if virtual_env is None:
-        options = get_parser(description="Initialize Modulefile in venv.",
-                             help_arguments="Log message when the module is loaded.",
-                             with_appli=False,
-                             with_verbose=True)
+        options = get_parser(
+            description="Initialize Modulefile in venv.",
+            help_arguments="Log message when the module is loaded.",
+            with_appli=False,
+            with_verbose=True,
+            options=[("modulefile-version",
+                      version_or_path,
+                      "Modulefile version to use if not found or version < 4.6."
+                      " It can be a source directory to avoid downloading")])
         virtual_env = Path(options.virtual_env).absolute()
+        if options.modulefile_version:
+            version_or_path = options.modulefile_version
 
     if version.parse(get_version()) < version.parse("14.6"):
 
         install_prefix=virtual_env / "opt" / "modulefiles"
         if not install_prefix.exists():
             code = ModuleInstaller(install_prefix=install_prefix,
                                 version_or_path=version_or_path,
```

### Comparing `venv-modulefile-0.0.8/src/venvmod/commands/append_module.py` & `venv-modulefile-0.0.9/src/venvmod/commands/append_module.py`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.0.8/src/venvmod/modulefile.py` & `venv-modulefile-0.0.9/src/venvmod/modulefile.py`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.0.8/src/README.md` & `venv-modulefile-0.0.9/src/README.md`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.0.8/src/venv_modulefile.egg-info/entry_points.txt` & `venv-modulefile-0.0.9/src/venv_modulefile.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.0.8/src/venv_modulefile.egg-info/SOURCES.txt` & `venv-modulefile-0.0.9/src/venv_modulefile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.0.8/src/venv_modulefile.egg-info/PKG-INFO` & `venv-modulefile-0.0.9/src/venv_modulefile.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: venv-modulefile
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python venv extension using Modulefile
 Home-page: https://github.com/roland-lenain/venv-modulefile
 Author: R. Lenain
 Author-email: roland.lenain@cea.fr
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/roland-lenain/venv-modulefile/issues
 Project-URL: Doc, https://venv-modulefile.readthedocs.io/en/latest/index.html
```

### Comparing `venv-modulefile-0.0.8/LICENSE.md` & `venv-modulefile-0.0.9/LICENSE.md`

 * *Files identical despite different names*

