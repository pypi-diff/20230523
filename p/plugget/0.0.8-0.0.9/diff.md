# Comparing `tmp/plugget-0.0.8.tar.gz` & `tmp/plugget-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plugget-0.0.8.tar", last modified: Sun May 21 13:13:57 2023, max compression
+gzip compressed data, was "plugget-0.0.9.tar", last modified: Tue May 23 14:02:07 2023, max compression
```

## Comparing `plugget-0.0.8.tar` & `plugget-0.0.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:13:57.724173 plugget-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:13:57.720173 plugget-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:13:57.724173 plugget-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-21 13:13:46.000000 plugget-0.0.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-21 13:13:46.000000 plugget-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-21 13:13:57.724173 plugget-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-21 13:13:46.000000 plugget-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:13:57.724173 plugget-0.0.8/plugget/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-21 13:13:46.000000 plugget-0.0.8/plugget/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:13:57.724173 plugget-0.0.8/plugget/actions/
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-21 13:13:46.000000 plugget-0.0.8/plugget/actions/_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-21 13:13:46.000000 plugget-0.0.8/plugget/actions/blender_addon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-21 13:13:46.000000 plugget-0.0.8/plugget/actions/blender_pip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-05-21 13:13:46.000000 plugget-0.0.8/plugget/actions/krita_pip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-21 13:13:46.000000 plugget-0.0.8/plugget/actions/krita_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-21 13:13:46.000000 plugget-0.0.8/plugget/actions/max_macroscript.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-21 13:13:46.000000 plugget-0.0.8/plugget/actions/unreal_pip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-21 13:13:46.000000 plugget-0.0.8/plugget/actions/unreal_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:13:57.724173 plugget-0.0.8/plugget/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 13:13:46.000000 plugget-0.0.8/plugget/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-21 13:13:46.000000 plugget-0.0.8/plugget/apps/blender.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:13:57.724173 plugget-0.0.8/plugget/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     9754 2023-05-21 13:13:46.000000 plugget-0.0.8/plugget/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:13:57.724173 plugget-0.0.8/plugget/data/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-21 13:13:46.000000 plugget-0.0.8/plugget/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13655 2023-05-21 13:13:46.000000 plugget-0.0.8/plugget/data/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-21 13:13:46.000000 plugget-0.0.8/plugget/data/packages_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:13:57.724173 plugget-0.0.8/plugget/github/
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-21 13:13:46.000000 plugget-0.0.8/plugget/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-21 13:13:46.000000 plugget-0.0.8/plugget/github/async.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:13:57.724173 plugget-0.0.8/plugget/gumroad/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-21 13:13:46.000000 plugget-0.0.8/plugget/gumroad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-21 13:13:46.000000 plugget-0.0.8/plugget/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-21 13:13:46.000000 plugget-0.0.8/plugget/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:13:57.724173 plugget-0.0.8/plugget.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-21 13:13:57.000000 plugget-0.0.8/plugget.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-21 13:13:57.000000 plugget-0.0.8/plugget.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 13:13:57.000000 plugget-0.0.8/plugget.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-21 13:13:57.000000 plugget-0.0.8/plugget.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-21 13:13:57.000000 plugget-0.0.8/plugget.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-21 13:13:46.000000 plugget-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-21 13:13:46.000000 plugget-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 13:13:57.728173 plugget-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-21 13:13:46.000000 plugget-0.0.8/testcode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:02:07.679933 plugget-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:02:07.671933 plugget-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:02:07.675933 plugget-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-23 14:01:54.000000 plugget-0.0.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-23 14:01:54.000000 plugget-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-23 14:02:07.679933 plugget-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-23 14:01:54.000000 plugget-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:02:07.675933 plugget-0.0.9/plugget/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-23 14:01:54.000000 plugget-0.0.9/plugget/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:02:07.675933 plugget-0.0.9/plugget/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-23 14:01:54.000000 plugget-0.0.9/plugget/actions/_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-05-23 14:01:54.000000 plugget-0.0.9/plugget/actions/blender_addon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-05-23 14:01:54.000000 plugget-0.0.9/plugget/actions/blender_pip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-05-23 14:01:54.000000 plugget-0.0.9/plugget/actions/krita_pip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-23 14:01:54.000000 plugget-0.0.9/plugget/actions/krita_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-23 14:01:54.000000 plugget-0.0.9/plugget/actions/max_macroscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-05-23 14:01:54.000000 plugget-0.0.9/plugget/actions/unreal_pip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-23 14:01:54.000000 plugget-0.0.9/plugget/actions/unreal_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:02:07.679933 plugget-0.0.9/plugget/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:01:54.000000 plugget-0.0.9/plugget/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-23 14:01:54.000000 plugget-0.0.9/plugget/apps/blender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:02:07.679933 plugget-0.0.9/plugget/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     9754 2023-05-23 14:01:54.000000 plugget-0.0.9/plugget/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:02:07.679933 plugget-0.0.9/plugget/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-23 14:01:54.000000 plugget-0.0.9/plugget/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13655 2023-05-23 14:01:54.000000 plugget-0.0.9/plugget/data/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-23 14:01:54.000000 plugget-0.0.9/plugget/data/packages_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:02:07.679933 plugget-0.0.9/plugget/github/
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-23 14:01:54.000000 plugget-0.0.9/plugget/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-23 14:01:54.000000 plugget-0.0.9/plugget/github/async.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:02:07.679933 plugget-0.0.9/plugget/gumroad/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-23 14:01:54.000000 plugget-0.0.9/plugget/gumroad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-23 14:01:54.000000 plugget-0.0.9/plugget/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-23 14:01:54.000000 plugget-0.0.9/plugget/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:02:07.675933 plugget-0.0.9/plugget.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-23 14:02:07.000000 plugget-0.0.9/plugget.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-23 14:02:07.000000 plugget-0.0.9/plugget.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:02:07.000000 plugget-0.0.9/plugget.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-23 14:02:07.000000 plugget-0.0.9/plugget.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 14:02:07.000000 plugget-0.0.9/plugget.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-23 14:01:54.000000 plugget-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-23 14:01:54.000000 plugget-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 14:02:07.679933 plugget-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-23 14:01:54.000000 plugget-0.0.9/testcode.py
```

### Comparing `plugget-0.0.8/.github/workflows/python-publish.yml` & `plugget-0.0.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `plugget-0.0.8/.gitignore` & `plugget-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `plugget-0.0.8/PKG-INFO` & `plugget-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugget
-Version: 0.0.8
+Version: 0.0.9
 Summary: detect which app the python interpreter is running in
 Author: Hannes
 Project-URL: Homepage, https://github.com/hannesdelbeke/plugget
 Project-URL: Source, https://github.com/hannesdelbeke/plugget
 Keywords: plugin,addon,add-on,extension,package,manager,resource,studio,dcc,app,application,pipeline,blender,krita,max
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.4
```

### Comparing `plugget-0.0.8/README.md` & `plugget-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `plugget-0.0.8/plugget/actions/_template.py` & `plugget-0.0.9/plugget/actions/_template.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.8/plugget/actions/blender_addon.py` & `plugget-0.0.9/plugget/actions/blender_addon.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 def install(package: "plugget.data.Package", force=False, enable=True, **kwargs) -> bool:  # todo , force=False, enable=True):
     # If the “force” parameter is True, the add-on will be reinstalled, even if it has not been previously removed.
     addon_names_before = _get_all_addon_names()
     _install_addon(package)
     addon_names_after = _get_all_addon_names()
     new_addons = addon_names_after - addon_names_before
-    _enable_addons(new_addons, enable=enable)
+    _enable_addons(new_addons, enable=enable)  # don't run this before dependencies are installed
     return True
 
 
 def _install_addon(package):
 
     # if a repo has plugin in root. we get the repo files content
     # if the repo has plugin in subdir, that file lives in repo_paths
```

### Comparing `plugget-0.0.8/plugget/actions/blender_pip.py` & `plugget-0.0.9/plugget/actions/blender_pip.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,24 @@
 import logging
 import subprocess
 from pathlib import Path
 import bpy
 import importlib
+import os
+import sys
+
+
+def prep_pythonpath():
+    # copy the sys.paths to PYTHONPATH to pass to subprocess, for pip to use
+    paths = os.environ.get("PYTHONPATH", "").split(os.pathsep)
+    new_paths = [p for p in sys.path if p not in paths]
+    paths += new_paths
+    joined_paths = os.pathsep.join(paths)
+    if joined_paths:
+        os.environ["PYTHONPATH"] = joined_paths
 
 
 def get_requirements(package: "plugget.data.Package", **kwargs) -> list[Path]:
     # if requirements.txt exists in self.repo_paths, install requirements
     requirements_paths = []
     if (package.clone_dir / "requirements.txt").exists():
         requirements_paths.append(package.clone_dir / "requirements.txt")
@@ -15,37 +27,43 @@
             if p.endswith("requirements.txt"):
                 requirements_paths.append(package.clone_dir / p)
     return requirements_paths
 
 
 # todo share pip functions
 def install(package: "plugget.data.Package", **kwargs):
+    prep_pythonpath()
+
     blender_user_site_packages = Path(str(bpy.utils.script_path_user())) / "modules"  # appdata
 
     for p in get_requirements(package):
         if p.exists():
             print("requirements.txt found, installing requirements")
             # todo blender pip
             try:
                 # todo python -m pip
-                subprocess.run(["pip", "install", "-r", package.clone_dir / p, '-t', blender_user_site_packages, "--no-user"])
+                subprocess.run(
+                    ["pip", "install", "--upgrade", "-r", package.clone_dir / p, '-t', blender_user_site_packages,
+                     "--no-user"])
             except subprocess.CalledProcessError as e:
                 logging.error(e.output)
         else:
             logging.warning(f"expected requirements.txt not found: '{p}'")
     importlib.invalidate_caches()
 
 
 def uninstall(package: "plugget.data.Package", dependencies=False, **kwargs):
     # this method runs on uninstall, then the manifest is removed from installed packages
     # ideally uninstall removes files from a folder,
 
     if not dependencies:
         return
 
+    prep_pythonpath()
+
     blender_user_site_packages = Path(str(bpy.utils.script_path_user())) / "modules"  # appdata
 
     for p in get_requirements(package):
         if p.exists():
             print("requirements.txt found, uninstalling requirements")
             print("package.clone_dir / p", package.clone_dir / p)
             subprocess.run(["pip", "uninstall", "-r", package.clone_dir / p, "-y"])
```

### Comparing `plugget-0.0.8/plugget/actions/krita_pip.py` & `plugget-0.0.9/plugget/actions/krita_pip.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 
 def install(package: "plugget.data.Package", **kwargs):
     print("check for requirements")
 
     for p in get_requirements(package):
         if p.exists():
             print("requirements.txt found, installing requirements")
+            # todo python -m pip with krita py interpreter
             subprocess.run(["pip", "install", "-r", package.clone_dir / p, '-t', path, "--no-user"])
         else:
             logging.warning(f"expected requirements.txt not found: '{p}'")
     importlib.invalidate_caches()
 
 
 # def install(package: "plugget.data.Package", **kwargs):
```

### Comparing `plugget-0.0.8/plugget/actions/krita_plugin.py` & `plugget-0.0.9/plugget/actions/krita_plugin.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.8/plugget/actions/max_macroscript.py` & `plugget-0.0.9/plugget/actions/max_macroscript.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.8/plugget/actions/unreal_pip.py` & `plugget-0.0.9/plugget/actions/unreal_pip.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 
 def install(package: "plugget.data.Package", **kwargs):
     print("check for requirements")
 
     for p in get_requirements(package):
         if p.exists():
             print("requirements.txt found, installing requirements")
+            # todo python -m pip with unreal py interpreter
             subprocess.run(["pip", "install", "-r", package.clone_dir / p, '-t', project_site_dir, "--no-user"])
         else:
             logging.warning(f"expected requirements.txt not found: '{p}'")
     importlib.invalidate_caches()
 
     # # check if files were copied: package.clone_dir / p
     # if not (package.clone_dir / p).exists():
```

### Comparing `plugget-0.0.8/plugget/actions/unreal_plugin.py` & `plugget-0.0.9/plugget/actions/unreal_plugin.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.8/plugget/apps/blender.py` & `plugget-0.0.9/plugget/apps/blender.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.8/plugget/commands/__init__.py` & `plugget-0.0.9/plugget/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.8/plugget/data/package.py` & `plugget-0.0.9/plugget/data/package.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.8/plugget/data/packages_meta.py` & `plugget-0.0.9/plugget/data/packages_meta.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.8/plugget/github/__init__.py` & `plugget-0.0.9/plugget/github/__init__.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.8/plugget/github/async.py` & `plugget-0.0.9/plugget/github/async.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.8/plugget/gumroad/__init__.py` & `plugget-0.0.9/plugget/gumroad/__init__.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.8/plugget/settings.py` & `plugget-0.0.9/plugget/settings.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.8/plugget.egg-info/PKG-INFO` & `plugget-0.0.9/plugget.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugget
-Version: 0.0.8
+Version: 0.0.9
 Summary: detect which app the python interpreter is running in
 Author: Hannes
 Project-URL: Homepage, https://github.com/hannesdelbeke/plugget
 Project-URL: Source, https://github.com/hannesdelbeke/plugget
 Keywords: plugin,addon,add-on,extension,package,manager,resource,studio,dcc,app,application,pipeline,blender,krita,max
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.4
```

### Comparing `plugget-0.0.8/plugget.egg-info/SOURCES.txt` & `plugget-0.0.9/plugget.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plugget-0.0.8/pyproject.toml` & `plugget-0.0.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3.7",
 ]
 #dynamic = ["dependencies"]
 dependencies = ['importlib-metadata; python_version<"3.7"', "detect-app"]
 #dynamic = ["version"]
-version = "0.0.8"
+version = "0.0.9"
 
 #[project.optional-dependencies]
 #yaml = ["pyyaml"]
 
 #[project.scripts]
 #my-script = "my_package.module:function"
```

### Comparing `plugget-0.0.8/testcode.py` & `plugget-0.0.9/testcode.py`

 * *Files identical despite different names*

