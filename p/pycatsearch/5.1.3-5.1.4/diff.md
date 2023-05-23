# Comparing `tmp/pycatsearch-5.1.3.tar.gz` & `tmp/pycatsearch-5.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycatsearch-5.1.3.tar", last modified: Fri May 19 17:57:11 2023, max compression
+gzip compressed data, was "pycatsearch-5.1.4.tar", last modified: Tue May 23 06:51:47 2023, max compression
```

## Comparing `pycatsearch-5.1.3.tar` & `pycatsearch-5.1.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:57:11.452977 pycatsearch-5.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:57:11.444977 pycatsearch-5.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:57:11.444977 pycatsearch-5.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-05-19 17:57:11.448977 pycatsearch-5.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9070 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     1391 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 17:57:11.452977 pycatsearch-5.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:57:11.444977 pycatsearch-5.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:57:11.448977 pycatsearch-5.1.3/src/pycatsearch/
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      109 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-19 17:57:11.000000 pycatsearch-5.1.3/src/pycatsearch/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/async_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    18859 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/catalog_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10423 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:57:11.448977 pycatsearch-5.1.3/src/pycatsearch/gui/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/gui/catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/gui/download_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/gui/float_spinbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/gui/frequency_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/gui/menu_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/gui/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/gui/selectable_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     9654 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/gui/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/gui/substance_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/gui/substances_box.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/gui/titled_list_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    38950 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/gui/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/gui/waiting_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)    21042 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/src/pycatsearch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:57:11.448977 pycatsearch-5.1.3/src/pycatsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-05-19 17:57:11.000000 pycatsearch-5.1.3/src/pycatsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-19 17:57:11.000000 pycatsearch-5.1.3/src/pycatsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 17:57:11.000000 pycatsearch-5.1.3/src/pycatsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-19 17:57:11.000000 pycatsearch-5.1.3/src/pycatsearch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 17:57:11.000000 pycatsearch-5.1.3/src/pycatsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-19 17:57:11.000000 pycatsearch-5.1.3/src/pycatsearch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-05-19 17:56:58.000000 pycatsearch-5.1.3/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:51:47.988060 pycatsearch-5.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:51:47.984060 pycatsearch-5.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:51:47.984060 pycatsearch-5.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10610 2023-05-23 06:51:47.988060 pycatsearch-5.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9070 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1230 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 06:51:47.988060 pycatsearch-5.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:51:47.984060 pycatsearch-5.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:51:47.988060 pycatsearch-5.1.4/src/pycatsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      109 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-23 06:51:47.000000 pycatsearch-5.1.4/src/pycatsearch/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/async_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18859 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/catalog_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10423 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:51:47.988060 pycatsearch-5.1.4/src/pycatsearch/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/gui/catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/gui/download_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/gui/float_spinbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/gui/frequency_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/gui/menu_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/gui/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/gui/selectable_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/gui/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/gui/substance_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/gui/substances_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/gui/titled_list_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40971 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/gui/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/gui/waiting_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23913 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/src/pycatsearch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:51:47.988060 pycatsearch-5.1.4/src/pycatsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10610 2023-05-23 06:51:47.000000 pycatsearch-5.1.4/src/pycatsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-23 06:51:47.000000 pycatsearch-5.1.4/src/pycatsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 06:51:47.000000 pycatsearch-5.1.4/src/pycatsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-23 06:51:47.000000 pycatsearch-5.1.4/src/pycatsearch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 06:51:47.000000 pycatsearch-5.1.4/src/pycatsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 06:51:47.000000 pycatsearch-5.1.4/src/pycatsearch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-05-23 06:51:34.000000 pycatsearch-5.1.4/updater.py
```

### Comparing `pycatsearch-5.1.3/.github/workflows/publish-to-pypi.yml` & `pycatsearch-5.1.4/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.3/LICENSE.md` & `pycatsearch-5.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.3/PKG-INFO` & `pycatsearch-5.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycatsearch
-Version: 5.1.3
+Version: 5.1.4
 Summary: Yet another implementation of JPL and CDMS spectroscopy catalogs offline search
 Author-email: StSav012 <stsav012@gmail.com>
 License: LGPL-3.0-only
 Project-URL: Source Code, https://github.com/StSav012/pycatsearch
 Project-URL: Bug Tracker, https://github.com/StSav012/pycatsearch/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Win32 (MS Windows)
@@ -20,15 +20,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Chemistry
-Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # PyCatSearch
```

### Comparing `pycatsearch-5.1.3/README.md` & `pycatsearch-5.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.3/main.py` & `pycatsearch-5.1.4/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,27 +20,21 @@
         _root.withdraw()
         tkinter.messagebox.showerror(title='Outdated Python', message=message)
         _root.destroy()
 
     exit(1)
 
 if __name__ == '__main__':
-    from contextlib import suppress
-
-    __author__ = 'StSav012'
-    __original_name__ = 'py''cat''search'
 
     try:
-        with suppress(ImportError):
-            from updater import update_with_pip
-
-            update_with_pip(__original_name__)
-
         from pycatsearch import main
     except ImportError:
+        __author__ = 'StSav012'
+        __original_name__ = 'py''cat''search'
+
         try:
             from updater import update_with_pip
 
             update_with_pip(__original_name__)
 
             from pycatsearch import main
         except ImportError:
```

### Comparing `pycatsearch-5.1.3/pyproject.toml` & `pycatsearch-5.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Topic :: Scientific/Engineering',
     'Topic :: Scientific/Engineering :: Astronomy',
     'Topic :: Scientific/Engineering :: Atmospheric Science',
     'Topic :: Scientific/Engineering :: Chemistry',
-    'Topic :: Scientific/Engineering :: Medical Science Apps.',
     'Topic :: Scientific/Engineering :: Physics',
     'Typing :: Typed',
 ]
 dynamic = [
     'version',
     'dependencies',
 ]
```

### Comparing `pycatsearch-5.1.3/setup.py` & `pycatsearch-5.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.3/src/pycatsearch/__init__.py` & `pycatsearch-5.1.4/src/pycatsearch/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from .catalog import Catalog
 
 __author__ = 'StSav012'
 __original_name__ = 'py''cat''search'
 
 try:
-    from _version import __version__
+    from ._version import __version__
 except ImportError:
     __version__ = ''
 
 
 def _version_tuple(version_string: str) -> tuple[int | str, ...]:
     result: tuple[int | str, ...] = tuple()
     part: str
@@ -72,15 +72,15 @@
     if _version_tuple(__version__) < _version_tuple('2.4.0'):
         # 2.4.0 is not released yet, so no warning until there is the release time
         if not QT6:
             QLibraryInfo.path = lambda *args, **kwargs: QLibraryInfo.location(*args, **kwargs)
             QLibraryInfo.LibraryPath = QLibraryInfo.LibraryLocation
 
 
-def main() -> None:
+def main() -> int:
     ap: argparse.ArgumentParser = argparse.ArgumentParser(
         allow_abbrev=True,
         description='Yet another implementation of JPL and CDMS spectroscopy catalogs offline search.\n'
                     f'Find more at https://github.com/{__author__}/{__original_name__}.')
     ap.add_argument('catalog', type=str, help='the catalog location to load',
                     nargs=argparse.ZERO_OR_MORE)
     ap_group = ap.add_argument_group(title='Search options',
@@ -123,20 +123,20 @@
                             'inchi', 'trivial_name', 'structural_formula', 'name', 'stoichiometric_formula',
                             'isotopolog', 'state', 'degrees_of_freedom', 'timeout']
     search_args: dict[str, str | float | int] = dict((arg, getattr(args, arg)) for arg in arg_names
                                                      if getattr(args, arg) is not None)
     if search_args:
         c: Catalog = Catalog(*args.catalog)
         c.print(**search_args)
-        return
+        return 0
 
-    main_gui()
+    return main_gui()
 
 
-def main_gui() -> None:
+def main_gui() -> int:
     ap: argparse.ArgumentParser = argparse.ArgumentParser(
         description='Yet another implementation of JPL and CDMS spectroscopy catalogs offline search.\n'
                     f'Find more at https://github.com/{__author__}/{__original_name__}.')
     ap.add_argument('catalog', type=str, help='the catalog location to load',
                     nargs=argparse.ZERO_OR_MORE)
 
     try:
@@ -173,16 +173,17 @@
             if isinstance(ex, SyntaxError):
                 tkinter.messagebox.showerror(title='Syntax Error', message=error_message)
             elif isinstance(ex, ImportError):
                 tkinter.messagebox.showerror(title='Package Missing', message=error_message)
             else:
                 tkinter.messagebox.showerror(title='Error', message=error_message)
             root.destroy()
+        return 1
     else:
-        gui.run()
+        return gui.run()
 
 
 def download() -> None:
     from . import downloader
 
     downloader.download()
```

### Comparing `pycatsearch-5.1.3/src/pycatsearch/async_downloader.py` & `pycatsearch-5.1.4/src/pycatsearch/async_downloader.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.3/src/pycatsearch/catalog.py` & `pycatsearch-5.1.4/src/pycatsearch/catalog.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.3/src/pycatsearch/catalog_entry.py` & `pycatsearch-5.1.4/src/pycatsearch/catalog_entry.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.3/src/pycatsearch/downloader.py` & `pycatsearch-5.1.4/src/pycatsearch/downloader.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.3/src/pycatsearch/gui/catalog_info.py` & `pycatsearch-5.1.4/src/pycatsearch/gui/catalog_info.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.3/src/pycatsearch/gui/download_dialog.py` & `pycatsearch-5.1.4/src/pycatsearch/gui/download_dialog.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 from math import inf
 from queue import Queue
 from typing import cast
 
-from qtpy.QtCore import QTimer
+from qtpy.QtCore import QTimer, Slot
 from qtpy.QtWidgets import (QDialog, QDoubleSpinBox, QFormLayout, QLabel, QProgressBar, QVBoxLayout,
                             QWidget, QWizard, QWizardPage)
 from qtpy.compat import getsavefilename
 
 try:
     from ..async_downloader import Downloader
 except (SyntaxError, ImportError, ModuleNotFoundError):
@@ -105,29 +105,30 @@
         self.downloader: Downloader | None = None
         self.state_queue: Queue[tuple[int, int]] = Queue()
 
         self.progress_bar: QProgressBar = QProgressBar(self)
         layout.addWidget(self.progress_bar)
 
         self.timer: QTimer = QTimer(self)
-        self.timer.timeout.connect(self.on_timeout)
+        self.timer.timeout.connect(self._on_timeout)
 
     def initializePage(self) -> None:
         super(ProgressPage, self).initializePage()
         self.setButtonText(QWizard.WizardButton.CommitButton, self.buttonText(QWizard.WizardButton.NextButton))
 
         frequency_limits: tuple[float, float] = (
             self.field('min_frequency'),
             self.field('max_frequency'),
         )
         self.downloader = Downloader(frequency_limits=frequency_limits, state_queue=self.state_queue)
         self.downloader.start()
         self.timer.start(100)
 
-    def on_timeout(self) -> None:
+    @Slot()
+    def _on_timeout(self) -> None:
         while not self.state_queue.empty():
             cataloged_species: int
             not_yet_processed_species: int
             cataloged_species, not_yet_processed_species = self.state_queue.get(block=False)
             self.progress_bar.setValue(cataloged_species)
             self.progress_bar.setMaximum(cataloged_species + not_yet_processed_species)
         if self.isComplete():
```

### Comparing `pycatsearch-5.1.3/src/pycatsearch/gui/float_spinbox.py` & `pycatsearch-5.1.4/src/pycatsearch/gui/float_spinbox.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.3/src/pycatsearch/gui/frequency_box.py` & `pycatsearch-5.1.4/src/pycatsearch/gui/frequency_box.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 from math import inf
 
-from qtpy.QtCore import Qt
+from qtpy.QtCore import Qt, Slot
 from qtpy.QtWidgets import QAbstractSpinBox, QDoubleSpinBox, QFormLayout, QTabWidget, QWidget
 
 from .settings import Settings
 from ..utils import *
 
 __all__ = ['FrequencyBox']
 
@@ -60,18 +60,18 @@
         self._spin_frequency_deviation.setSingleStep(0.1)
         self._spin_frequency_deviation.setValue(0.4)
         self._layout_by_center.addRow(self._layout_by_center.tr('Deviation:'), self._spin_frequency_deviation)
         self.addTab(self._page_by_center, self.tr('Center'))
 
         self.load_settings()
 
-        self._spin_frequency_from.editingFinished.connect(self.on_spin_frequency_from_edited)
-        self._spin_frequency_to.editingFinished.connect(self.on_spin_frequency_to_edited)
-        self._spin_frequency_center.editingFinished.connect(self.on_spin_frequency_center_edited)
-        self._spin_frequency_deviation.editingFinished.connect(self.on_spin_frequency_deviation_edited)
+        self._spin_frequency_from.editingFinished.connect(self._on_spin_frequency_from_edited)
+        self._spin_frequency_to.editingFinished.connect(self._on_spin_frequency_to_edited)
+        self._spin_frequency_center.editingFinished.connect(self._on_spin_frequency_center_edited)
+        self._spin_frequency_deviation.editingFinished.connect(self._on_spin_frequency_deviation_edited)
 
     def load_settings(self) -> None:
         self._settings.beginGroup('search')
         self._settings.beginGroup('frequency')
         self._frequency_from = self._settings.value('from', self._spin_frequency_from.value(), float)
         self._frequency_to = self._settings.value('to', self._spin_frequency_to.value(), float)
         self._frequency_center = self._settings.value('center', self._spin_frequency_center.value(), float)
@@ -109,24 +109,28 @@
         min_value = self._settings.from_mhz(min_value)
         max_value = self._settings.from_mhz(max_value)
         spin: QDoubleSpinBox
         for spin in frequency_spins:
             spin.setMinimum(min_value)
             spin.setMaximum(max_value)
 
-    def on_spin_frequency_from_edited(self) -> None:
+    @Slot()
+    def _on_spin_frequency_from_edited(self) -> None:
         self._frequency_from = self._settings.to_mhz(self._spin_frequency_from.value())
 
-    def on_spin_frequency_to_edited(self) -> None:
+    @Slot()
+    def _on_spin_frequency_to_edited(self) -> None:
         self._frequency_to = self._settings.to_mhz(self._spin_frequency_to.value())
 
-    def on_spin_frequency_center_edited(self) -> None:
+    @Slot()
+    def _on_spin_frequency_center_edited(self) -> None:
         self._frequency_center = self._settings.to_mhz(self._spin_frequency_center.value())
 
-    def on_spin_frequency_deviation_edited(self) -> None:
+    @Slot()
+    def _on_spin_frequency_deviation_edited(self) -> None:
         self._frequency_deviation = self._settings.to_mhz(self._spin_frequency_deviation.value())
 
     def fill_parameters(self) -> None:
         frequency_suffix: int = self._settings.frequency_unit
         frequency_suffix_str: str = ' ' + self._settings.FREQUENCY_UNITS[frequency_suffix]
         if frequency_suffix in (0, 1, 2):  # MHz, GHz, cm⁻¹
             self._spin_frequency_from.setValue(self._settings.from_mhz(self._frequency_from))
```

### Comparing `pycatsearch-5.1.3/src/pycatsearch/gui/menu_bar.py` & `pycatsearch-5.1.4/src/pycatsearch/gui/menu_bar.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
             QIcon.fromTheme('document-revert', self.style().standardIcon(QStyle.StandardPixmap.SP_BrowserReload)),
             self.tr('&Reload Catalogs'),
             self.menu_file)
         self.action_download_catalog: QAction = QAction(self.tr('&Download Catalog...'), self.menu_file)
         self.action_preferences: QAction = QAction(self.tr('&Preferences...'), self.menu_file)
         self.action_quit: QAction = QAction(QIcon.fromTheme('application-exit'), self.tr('&Quit'),
                                             self.menu_file)
+        self.action_check_updates: QAction = QAction(self.tr('Check for Updates...'), self.menu_help)
         self.action_about_catalogs: QAction = QAction(
             QIcon.fromTheme('help-about', self.style().standardIcon(QStyle.StandardPixmap.SP_FileDialogInfoView)),
             self.tr('About Catalogs...'),
             self.menu_help)
         self.action_about: QAction = QAction(
             QIcon.fromTheme('help-about', self.style().standardIcon(QStyle.StandardPixmap.SP_FileDialogInfoView)),
             self.tr('&About...'),
@@ -64,14 +65,16 @@
         self.menu_file.addAction(self.action_reload)
         self.menu_file.addSeparator()
         self.menu_file.addAction(self.action_download_catalog)
         self.menu_file.addSeparator()
         self.menu_file.addAction(self.action_preferences)
         self.menu_file.addSeparator()
         self.menu_file.addAction(self.action_quit)
+        self.menu_help.addAction(self.action_check_updates)
+        self.menu_help.addSeparator()
         self.menu_help.addAction(self.action_about_catalogs)
         self.menu_help.addAction(self.action_about)
         self.menu_help.addAction(self.action_about_qt)
         self.menu_copy_only.addAction(self.action_copy_name)
         self.menu_copy_only.addAction(self.action_copy_frequency)
         self.menu_copy_only.addAction(self.action_copy_intensity)
         self.menu_copy_only.addAction(self.action_copy_lower_state_energy)
```

### Comparing `pycatsearch-5.1.3/src/pycatsearch/gui/preferences.py` & `pycatsearch-5.1.4/src/pycatsearch/gui/preferences.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.3/src/pycatsearch/gui/settings.py` & `pycatsearch-5.1.4/src/pycatsearch/gui/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,17 @@
     TEMPERATURE_UNITS: Final[list[str]] = ['K', '°C']
     LINE_ENDS: Final[list[str]] = [r'Line Feed (\n)', r'Carriage Return (\r)', r'CR+LF (\r\n)', r'LF+CR (\n\r)']
     _LINE_ENDS: Final[list[str]] = ['\n', '\r', '\r\n', '\n\r']
     CSV_SEPARATORS: Final[list[str]] = [r'comma (,)', r'tab (\t)', r'semicolon (;)', r'space ( )']
     _CSV_SEPARATORS: Final[list[str]] = [',', '\t', ';', ' ']
 
     DIALOG: dict[str, dict[str, tuple[Any, ...]]] = {
-        'Start': {
-            'Load catalogs when the program starts': ('load_last_catalogs',),
+        'When the program starts': {
+            'Load catalogs': ('load_last_catalogs',),
+            'Check for update': ('check_updates',),
         },
         'Display': {
             'Allow rich text in formulas': ('rich_text_in_formulas',),
         },
         'Search': {
             'Timeout:': (slice(1, 99), (' sec',), 'timeout',),
         },
@@ -232,14 +233,27 @@
     @load_last_catalogs.setter
     def load_last_catalogs(self, new_value: bool) -> None:
         self.beginGroup('start')
         self.setValue('loadLastCatalogs', new_value)
         self.endGroup()
 
     @property
+    def check_updates(self) -> bool:
+        self.beginGroup('start')
+        v: bool = self.value('checkUpdates', True, bool)
+        self.endGroup()
+        return v
+
+    @check_updates.setter
+    def check_updates(self, new_value: bool) -> None:
+        self.beginGroup('start')
+        self.setValue('checkUpdates', new_value)
+        self.endGroup()
+
+    @property
     def rich_text_in_formulas(self) -> bool:
         self.beginGroup('display')
         v: bool = self.value('richTextInFormulas', True, bool)
         self.endGroup()
         return v
 
     @rich_text_in_formulas.setter
```

### Comparing `pycatsearch-5.1.3/src/pycatsearch/gui/substance_info.py` & `pycatsearch-5.1.4/src/pycatsearch/gui/substance_info.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.3/src/pycatsearch/gui/substances_box.py` & `pycatsearch-5.1.4/src/pycatsearch/gui/substances_box.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
-from qtpy.QtCore import QModelIndex, Qt
+from qtpy.QtCore import QModelIndex, Qt, Slot
 from qtpy.QtWidgets import (QAbstractItemView, QCheckBox, QGroupBox, QLineEdit, QListWidget,
                             QListWidgetItem, QPushButton, QVBoxLayout, QWidget)
 
 from .settings import Settings
 from .substance_info import SubstanceInfo, SubstanceInfoSelector
 from ..catalog import Catalog
 from ..utils import *
@@ -43,18 +43,18 @@
             self._check_keep_selection.tr('Keep substances list selection through filter changes'))
         self._check_keep_selection.setText(self._check_keep_selection.tr('Persistent Selection'))
         self._layout_substance.addWidget(self._check_keep_selection)
         self._button_select_none.setStatusTip(self._button_select_none.tr('Clear substances list selection'))
         self._button_select_none.setText(self._button_select_none.tr('Select None'))
         self._layout_substance.addWidget(self._button_select_none)
 
-        self._text_substance.textChanged.connect(self.on_text_changed)
-        self._check_keep_selection.toggled.connect(self.on_check_save_selection_toggled)
-        self._button_select_none.clicked.connect(self.on_button_select_none_clicked)
-        self._list_substance.doubleClicked.connect(self.on_list_substance_double_clicked)
+        self._text_substance.textChanged.connect(self._on_text_changed)
+        self._check_keep_selection.toggled.connect(self._on_check_save_selection_toggled)
+        self._button_select_none.clicked.connect(self._on_button_select_none_clicked)
+        self._list_substance.doubleClicked.connect(self._on_list_substance_double_clicked)
 
         self.load_settings()
 
     def update_selected_substances(self) -> None:
         if self.isChecked():
             for i in range(self._list_substance.count()):
                 item: QListWidgetItem = self._list_substance.item(i)
@@ -124,28 +124,32 @@
             new_item.setData(Qt.ItemDataRole.UserRole, ids)
             new_item.setFlags(new_item.flags() | Qt.ItemFlag.ItemIsUserCheckable)
             new_item.setCheckState(Qt.CheckState.Checked
                                    if text in self._selected_substances
                                    else Qt.CheckState.Unchecked)
             self._list_substance.addItem(new_item)
 
-    def on_text_changed(self, current_text: str) -> None:
+    @Slot(str)
+    def _on_text_changed(self, current_text: str) -> None:
         self.fill_substances_list(current_text)
 
-    def on_check_save_selection_toggled(self, new_state: bool) -> None:
+    @Slot(bool)
+    def _on_check_save_selection_toggled(self, new_state: bool) -> None:
         if not new_state:
             self._selected_substances.clear()
             self.update_selected_substances()
 
-    def on_button_select_none_clicked(self) -> None:
+    @Slot()
+    def _on_button_select_none_clicked(self) -> None:
         for i in range(self._list_substance.count()):
             self._list_substance.item(i).setCheckState(Qt.CheckState.Unchecked)
         self._selected_substances.clear()
 
-    def on_list_substance_double_clicked(self, index: QModelIndex) -> None:
+    @Slot(QModelIndex)
+    def _on_list_substance_double_clicked(self, index: QModelIndex) -> None:
         item: QListWidgetItem = self._list_substance.item(index.row())
         ids: set[int] = item.data(Qt.ItemDataRole.UserRole)
         if len(ids) > 1:
             sis: SubstanceInfoSelector = SubstanceInfoSelector(self.catalog, ids, parent=self)
             sis.exec()
         elif ids:  # if not empty
             syn: SubstanceInfo = SubstanceInfo(self.catalog, ids.pop(), parent=self)
```

### Comparing `pycatsearch-5.1.3/src/pycatsearch/gui/titled_list_widget.py` & `pycatsearch-5.1.4/src/pycatsearch/gui/titled_list_widget.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.3/src/pycatsearch/gui/ui.py` & `pycatsearch-5.1.4/src/pycatsearch/gui/ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import math
 from typing import Any, Callable, Final
 
-from qtpy.QtCore import QAbstractTableModel, QMimeData, QModelIndex, QPoint, QPointF, QRect, QSize, Qt
+from qtpy.QtCore import QAbstractTableModel, QMimeData, QModelIndex, QPoint, QPointF, QRect, QSize, Qt, Slot
 from qtpy.QtGui import (QAbstractTextDocumentLayout, QClipboard, QCloseEvent, QCursor, QIcon, QPainter, QPixmap,
                         QScreen, QTextDocument)
 from qtpy.QtWidgets import (QAbstractItemView, QAbstractSpinBox, QApplication, QDoubleSpinBox, QFormLayout, QGridLayout,
                             QHeaderView, QMainWindow, QMessageBox, QPushButton, QStatusBar, QStyle,
                             QStyleOptionViewItem, QStyledItemDelegate, QTableView, QTableWidgetSelectionRange, QWidget)
 from qtpy.compat import getopenfilenames
 
@@ -386,43 +386,56 @@
 
         self.results_shown: bool = False
 
         self.preset_table()
 
         self.load_settings()
 
-        self.results_table.customContextMenuRequested.connect(self.on_table_context_menu_requested)
-        self.results_table.selectionModel().selectionChanged.connect(self.on_table_item_selection_changed)
-        self.results_table.doubleClicked.connect(self.on_action_substance_info_triggered)
-        self.spin_intensity.valueChanged.connect(self.on_spin_intensity_changed)
-        self.spin_temperature.valueChanged.connect(self.on_spin_temperature_changed)
-        self.button_search.clicked.connect(self.on_button_search_clicked)
-        self.menu_bar.action_load.triggered.connect(self.on_action_load_triggered)
-        self.menu_bar.action_quit.triggered.connect(self.on_action_quit_triggered)
-        self.menu_bar.action_about_catalogs.triggered.connect(self.on_action_about_catalogs_triggered)
-        self.menu_bar.action_about.triggered.connect(self.on_action_about_triggered)
-        self.menu_bar.action_about_qt.triggered.connect(self.on_action_about_qt_triggered)
-        self.menu_bar.action_download_catalog.triggered.connect(self.on_action_download_catalog_triggered)
-        self.menu_bar.action_preferences.triggered.connect(self.on_action_preferences_triggered)
-        self.menu_bar.action_copy.triggered.connect(self.on_action_copy_triggered)
-        self.menu_bar.action_select_all.triggered.connect(self.on_action_select_all_triggered)
-        self.menu_bar.action_reload.triggered.connect(self.on_action_reload_triggered)
-        self.menu_bar.action_copy_name.triggered.connect(self.on_action_copy_name_triggered)
-        self.menu_bar.action_copy_frequency.triggered.connect(self.on_action_copy_frequency_triggered)
-        self.menu_bar.action_copy_intensity.triggered.connect(self.on_action_copy_intensity_triggered)
-        self.menu_bar.action_copy_lower_state_energy.triggered.connect(self.on_action_copy_lower_state_energy_triggered)
-        self.menu_bar.action_show_frequency.toggled.connect(self.on_action_show_frequency_toggled)
-        self.menu_bar.action_show_intensity.toggled.connect(self.on_action_show_intensity_toggled)
-        self.menu_bar.action_show_lower_state_energy.toggled.connect(self.on_action_show_lower_state_energy_toggled)
-        self.menu_bar.action_substance_info.triggered.connect(self.on_action_substance_info_triggered)
-        self.menu_bar.action_clear.triggered.connect(self.on_action_clear_triggered)
+        self.results_table.customContextMenuRequested.connect(self._on_table_context_menu_requested)
+        self.results_table.selectionModel().selectionChanged.connect(self._on_table_item_selection_changed)
+        self.results_table.doubleClicked.connect(self._on_action_substance_info_triggered)
+        self.spin_intensity.valueChanged.connect(self._on_spin_intensity_changed)
+        self.spin_temperature.valueChanged.connect(self._on_spin_temperature_changed)
+        self.button_search.clicked.connect(self._on_button_search_clicked)
+        self.menu_bar.action_load.triggered.connect(self._on_action_load_triggered)
+        self.menu_bar.action_quit.triggered.connect(self._on_action_quit_triggered)
+        self.menu_bar.action_check_updates.triggered.connect(self._on_action_check_updates_triggered)
+        self.menu_bar.action_about_catalogs.triggered.connect(self._on_action_about_catalogs_triggered)
+        self.menu_bar.action_about.triggered.connect(self._on_action_about_triggered)
+        self.menu_bar.action_about_qt.triggered.connect(self._on_action_about_qt_triggered)
+        self.menu_bar.action_download_catalog.triggered.connect(self._on_action_download_catalog_triggered)
+        self.menu_bar.action_preferences.triggered.connect(self._on_action_preferences_triggered)
+        self.menu_bar.action_copy.triggered.connect(self._on_action_copy_triggered)
+        self.menu_bar.action_select_all.triggered.connect(self._on_action_select_all_triggered)
+        self.menu_bar.action_reload.triggered.connect(self._on_action_reload_triggered)
+        self.menu_bar.action_copy_name.triggered.connect(self._on_action_copy_name_triggered)
+        self.menu_bar.action_copy_frequency.triggered.connect(self._on_action_copy_frequency_triggered)
+        self.menu_bar.action_copy_intensity.triggered.connect(self._on_action_copy_intensity_triggered)
+        self.menu_bar.action_copy_lower_state_energy.triggered.connect(
+            self._on_action_copy_lower_state_energy_triggered)
+        self.menu_bar.action_show_frequency.toggled.connect(self._on_action_show_frequency_toggled)
+        self.menu_bar.action_show_intensity.toggled.connect(self._on_action_show_intensity_toggled)
+        self.menu_bar.action_show_lower_state_energy.toggled.connect(self._on_action_show_lower_state_energy_toggled)
+        self.menu_bar.action_substance_info.triggered.connect(self._on_action_substance_info_triggered)
+        self.menu_bar.action_clear.triggered.connect(self._on_action_clear_triggered)
 
         if not self.catalog.is_empty:
             self.box_frequency.set_frequency_limits(self.catalog.min_frequency, self.catalog.max_frequency)
 
+        if self.settings.check_updates:
+            _latest_release: ReleaseInfo = latest_release()
+            if _latest_release and _latest_release.version > __version__:
+                res: QMessageBox.StandardButton = QMessageBox.question(
+                    self, self.tr('Release Info'),
+                    self.tr('Version {release.version} published {release.pub_date} is available. '
+                            'Would you like to get the update? '
+                            'The app will try to restart.').format(release=_latest_release))
+                if res == QMessageBox.StandardButton.Yes:
+                    update_with_pip()
+
     def closeEvent(self, event: QCloseEvent) -> None:
         self.save_settings()
         event.accept()
 
     def load_catalog(self, *catalog_file_names: str) -> bool:
         self.setDisabled(True)
         last_cursor: QCursor = self.cursor()
@@ -433,27 +446,31 @@
         self.setCursor(last_cursor)
         self.setEnabled(True)
         self.button_search.setDisabled(self.catalog.is_empty)
         if not self.catalog.is_empty:
             self.box_frequency.set_frequency_limits(self.catalog.min_frequency, self.catalog.max_frequency)
         return not self.catalog.is_empty
 
-    def on_spin_temperature_changed(self, arg1: float) -> None:
+    @Slot(float)
+    def _on_spin_temperature_changed(self, arg1: float) -> None:
         self.temperature = self.settings.to_k(arg1)
         self.fill_table()
 
-    def on_spin_intensity_changed(self, arg1: float) -> None:
+    @Slot(float)
+    def _on_spin_intensity_changed(self, arg1: float) -> None:
         self.minimal_intensity = self.settings.to_log10_sq_nm_mhz(arg1)
         if self.results_shown:
             self.fill_table()
 
-    def on_table_context_menu_requested(self, pos: QPoint) -> None:
+    @Slot(QPoint)
+    def _on_table_context_menu_requested(self, pos: QPoint) -> None:
         self.menu_bar.menu_edit.popup(self.results_table.viewport().mapToGlobal(pos))
 
-    def on_table_item_selection_changed(self) -> None:
+    @Slot()
+    def _on_table_item_selection_changed(self) -> None:
         self.menu_bar.action_copy.setEnabled(bool(self.results_table.selectionModel().selectedRows()))
         self.menu_bar.action_substance_info.setEnabled(bool(self.results_table.selectionModel().selectedRows()))
 
     def get_open_file_names(self, formats: dict[tuple[str, ...], str],
                             caption: str = '', directory: str = '') -> tuple[list[str], str]:
 
         def join_file_dialog_formats(_formats: dict[tuple[str, ...], str]) -> str:
@@ -476,15 +493,16 @@
         _filter: str
         filename, _filter = getopenfilenames(self,
                                              caption=caption,
                                              filters=join_file_dialog_formats(formats),
                                              basedir=directory)
         return filename, _filter
 
-    def on_action_load_triggered(self) -> None:
+    @Slot()
+    def _on_action_load_triggered(self) -> None:
         self.status_bar.showMessage(self.tr('Select a catalog file to load.'))
         new_catalog_file_names: list[str]
         _formats: dict[tuple[str, ...], str] = {
             tuple(*all_cases('.json.gz'), *all_cases('.json.bz2'),
                   *all_cases('.json.xz'), *all_cases('.json.lzma')): self.tr('Compressed JSON', 'file type'),
             tuple(all_cases('.json')): self.tr('JSON', 'file type'),
         }
@@ -498,15 +516,16 @@
                 self.status_bar.showMessage(self.tr('Catalogs loaded.'))
             else:
                 self.status_bar.showMessage(self.tr('Failed to load a catalog.'))
 
         else:
             self.status_bar.clearMessage()
 
-    def on_action_reload_triggered(self) -> None:
+    @Slot()
+    def _on_action_reload_triggered(self) -> None:
         if self.catalog.sources:
             self.status_bar.showMessage(self.tr('Loading...'))
             if self.load_catalog(*self.catalog.sources):
                 self.status_bar.showMessage(self.tr('Catalogs loaded.'))
             else:
                 self.status_bar.showMessage(self.tr('Failed to load a catalog.'))
         else:
@@ -535,33 +554,37 @@
                                                        self.menu_bar.menu_columns.actions()))
                      if _a.isChecked()]
                 ) +
                 '</td></tr>' + self.settings.line_end
             )
         return '<table>' + self.settings.line_end + ''.join(text) + '</table>'
 
-    def on_action_download_catalog_triggered(self) -> None:
+    @Slot()
+    def _on_action_download_catalog_triggered(self) -> None:
         downloader: DownloadDialog = DownloadDialog(
             frequency_limits=(self.catalog.min_frequency, self.catalog.max_frequency),
             parent=self)
         downloader.exec()
 
-    def on_action_preferences_triggered(self) -> None:
+    @Slot()
+    def _on_action_preferences_triggered(self) -> None:
         self.preferences_dialog.exec()
         self.fill_parameters()
         if self.results_model.rowCount():
             self.preset_table()
             self.fill_table()
         else:
             self.preset_table()
 
-    def on_action_quit_triggered(self) -> None:
+    @Slot()
+    def _on_action_quit_triggered(self) -> None:
         self.close()
 
-    def on_action_clear_triggered(self) -> None:
+    @Slot()
+    def _on_action_clear_triggered(self) -> None:
         self.results_model.clear()
         self.preset_table()
 
     def copy_selected_items(self, col: int) -> None:
         if col >= self.results_model.columnCount():
             return
 
@@ -573,63 +596,91 @@
         for row in self.results_table.selectionModel().selectedRows(col):
             text_to_copy.append(self.results_model.data(row))
         if col == 0:
             copy_to_clipboard(html_list(text_to_copy), Qt.TextFormat.RichText)
         else:
             copy_to_clipboard(self.settings.line_end.join(text_to_copy), Qt.TextFormat.PlainText)
 
-    def on_action_copy_name_triggered(self) -> None:
+    @Slot()
+    def _on_action_copy_name_triggered(self) -> None:
         self.copy_selected_items(0)
 
-    def on_action_copy_frequency_triggered(self) -> None:
+    @Slot()
+    def _on_action_copy_frequency_triggered(self) -> None:
         self.copy_selected_items(1)
 
-    def on_action_copy_intensity_triggered(self) -> None:
+    @Slot()
+    def _on_action_copy_intensity_triggered(self) -> None:
         self.copy_selected_items(2)
 
-    def on_action_copy_lower_state_energy_triggered(self) -> None:
+    @Slot()
+    def _on_action_copy_lower_state_energy_triggered(self) -> None:
         self.copy_selected_items(3)
 
-    def on_action_copy_triggered(self) -> None:
+    @Slot()
+    def _on_action_copy_triggered(self) -> None:
         copy_to_clipboard(self.stringify_selection_html(), Qt.TextFormat.RichText)
 
-    def on_action_select_all_triggered(self) -> None:
+    @Slot()
+    def _on_action_select_all_triggered(self) -> None:
         self.results_table.selectAll()
 
-    def on_action_substance_info_triggered(self) -> None:
+    @Slot()
+    def _on_action_substance_info_triggered(self) -> None:
         if self.results_table.selectionModel().selectedRows():
             syn: SubstanceInfo = SubstanceInfo(
                 self.catalog,
                 self.results_model.row(self.results_table.selectionModel().selectedRows()[0].row()).id,
                 self)
             syn.exec()
 
     def toggle_results_table_column_visibility(self, column: int, is_visible: bool) -> None:
         if is_visible:
             self.results_table.showColumn(column)
         else:
             self.results_table.hideColumn(column)
 
-    def on_action_show_frequency_toggled(self, is_checked: bool) -> None:
+    @Slot(bool)
+    def _on_action_show_frequency_toggled(self, is_checked: bool) -> None:
         self.toggle_results_table_column_visibility(1, is_checked)
 
-    def on_action_show_intensity_toggled(self, is_checked: bool) -> None:
+    @Slot(bool)
+    def _on_action_show_intensity_toggled(self, is_checked: bool) -> None:
         self.toggle_results_table_column_visibility(2, is_checked)
 
-    def on_action_show_lower_state_energy_toggled(self, is_checked: bool) -> None:
+    @Slot(bool)
+    def _on_action_show_lower_state_energy_toggled(self, is_checked: bool) -> None:
         self.toggle_results_table_column_visibility(3, is_checked)
 
-    def on_action_about_catalogs_triggered(self) -> None:
+    @Slot()
+    def _on_action_check_updates_triggered(self) -> None:
+        _latest_release: ReleaseInfo = latest_release()
+        if not _latest_release:
+            QMessageBox.warning(self, self.tr('Release Info'), self.tr('Update check failed.'))
+        elif _latest_release.version > __version__:
+            res: QMessageBox.StandardButton = QMessageBox.question(
+                self, self.tr('Release Info'),
+                self.tr('Version {release.version} published {release.pub_date} is available. '
+                        'Would you like to get the update? '
+                        'The app will try to restart.').format(release=_latest_release))
+            if res == QMessageBox.StandardButton.Yes:
+                update_with_pip()
+        else:
+            QMessageBox.information(self, self.tr('Release Info'), self.tr('You are using the latest version.'))
+
+    @Slot()
+    def _on_action_about_catalogs_triggered(self) -> None:
         if self.catalog:
             ci: CatalogInfo = CatalogInfo(self.catalog, self)
             ci.exec()
         else:
             QMessageBox.information(self, self.tr('Catalog Info'), self.tr('No catalogs loaded'))
 
-    def on_action_about_triggered(self) -> None:
+    @Slot()
+    def _on_action_about_triggered(self) -> None:
         QMessageBox.about(self,
                           self.tr("About CatSearch"),
                           "<html><p>"
                           + self.tr("CatSearch is a means of searching through spectroscopy lines catalogs. "
                                     "It's an offline application.")
                           + "</p><p>"
                           + self.tr("It relies on the data stored in JSON files.")
@@ -649,15 +700,16 @@
                           .format("<a href='https://www.gnu.org/copyleft/lesser.html'>{0}</a>"
                                   .format(self.tr("GNU LGPL version 3")))
                           + "</p><p>"
                           + self.tr("The source code is available on {0}.").format(
                               "<a href='https://github.com/StSav012/pycatsearch'>GitHub</a>")
                           + "</p></html>")
 
-    def on_action_about_qt_triggered(self) -> None:
+    @Slot()
+    def _on_action_about_qt_triggered(self) -> None:
         QMessageBox.aboutQt(self)
 
     def load_settings(self) -> None:
         self.settings.beginGroup('search')
         catalog_file_names: list[str] = []
         for i in range(self.settings.beginReadArray('catalogFiles')):
             self.settings.setArrayIndex(i)
@@ -777,15 +829,16 @@
 
         self.results_table.setSortingEnabled(True)
         self.menu_bar.action_select_all.setEnabled(bool(entries))
         self.menu_bar.action_clear.setEnabled(bool(entries))
         self.menu_bar.menu_copy_only.setEnabled(bool(entries))
         self.results_shown = True
 
-    def on_button_search_clicked(self) -> None:
+    @Slot()
+    def _on_button_search_clicked(self) -> None:
         self.status_bar.showMessage(self.tr('Searching...'))
         self.setDisabled(True)
         last_cursor: QCursor = self.cursor()
         self.setCursor(Qt.CursorShape.WaitCursor)
         self.repaint()
         self.box_substance.update_selected_substances()
         self.fill_table()
```

### Comparing `pycatsearch-5.1.3/src/pycatsearch/gui/waiting_screen.py` & `pycatsearch-5.1.4/src/pycatsearch/gui/waiting_screen.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.3/src/pycatsearch/utils.py` & `pycatsearch-5.1.4/src/pycatsearch/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,15 +26,16 @@
            'log10_sq_nm_mhz_to_cm_per_molecule',
            'sq_nm_mhz_to_log10_sq_nm_mhz',
            'log10_cm_per_molecule_to_log10_sq_nm_mhz',
            'cm_per_molecule_to_log10_sq_nm_mhz',
            'sort_unique', 'merge_sorted', 'search_sorted',
            'within', 'chem_html', 'best_name', 'remove_html', 'wrap_in_html',
            'ensure_prefix', 'all_cases',
-           'save_catalog_to_file']
+           'save_catalog_to_file',
+           'ReleaseInfo', 'latest_release', 'update_with_pip']
 
 M_LOG10E: Final[float] = math.log10(math.e)
 
 T0: Final[float] = 300.00
 k: Final[float] = 1.380649000e-23  # https://physics.nist.gov/cgi-bin/cuu/Value?k
 h: Final[float] = 6.626070150e-34  # https://physics.nist.gov/cgi-bin/cuu/Value?h
 e: Final[float] = 1.602176634e-19  # https://physics.nist.gov/cgi-bin/cuu/Value?e
@@ -584,7 +585,78 @@
                          frequency_limits: tuple[float, float]) -> bool:
     from catalog import Catalog
 
     if not catalog:
         return False
     Catalog.save(filename=filename, catalog=catalog, frequency_limits=frequency_limits)
     return True
+
+
+class ReleaseInfo:
+    def __init__(self, version: str = '', pub_date: str = '') -> None:
+        self.version: str = version
+        self.pub_date: str = pub_date
+
+    def __bool__(self) -> bool:
+        return bool(self.version) and bool(self.pub_date)
+
+    def __gt__(self, other: str) -> bool:
+        self_as_tuple: tuple[int | str, ...] = tuple(int(i) if i.isdigit() else i for i in self.version.split('.'))
+        other_as_tuple: tuple[int | str, ...] = tuple(int(i) if i.isdigit() else i for i in other.split('.'))
+        return self_as_tuple > other_as_tuple
+
+
+def latest_release() -> ReleaseInfo:
+    import urllib.request
+    import xml.dom.minidom as dom
+    from http.client import HTTPResponse
+    from xml.dom.minicompat import NodeList
+    from urllib.error import URLError
+
+    from . import __original_name__
+
+    try:
+        r: HTTPResponse = urllib.request.urlopen(f'https://pypi.org/rss/project/{__original_name__}/releases.xml',
+                                                 timeout=1)
+    except URLError:
+        return ReleaseInfo()
+    if r.getcode() != 200 or not r.readable():
+        return ReleaseInfo()
+    rss: dom.Node | None = dom.parseString(r.read().decode(encoding='ascii')).documentElement
+    if not isinstance(rss, dom.Element) or rss.tagName != 'rss':
+        return ReleaseInfo()
+    channels: NodeList = rss.getElementsByTagName('channel')
+    if not channels or channels[0].nodeType != dom.Node.ELEMENT_NODE:
+        return ReleaseInfo()
+    channel: dom.Element = channels[0]
+    items: NodeList = channel.getElementsByTagName('item')
+    if not items or items[0].nodeType != dom.Node.ELEMENT_NODE:
+        return ReleaseInfo()
+    item: dom.Element = items[0]
+    titles: NodeList = item.getElementsByTagName('title')
+    if not titles or titles[0].nodeType != dom.Node.ELEMENT_NODE:
+        return ReleaseInfo()
+    title: dom.Element = titles[0]
+    pub_dates: NodeList = item.getElementsByTagName('pubDate')
+    if not pub_dates or pub_dates[0].nodeType != dom.Node.ELEMENT_NODE:
+        return ReleaseInfo()
+    pub_date: dom.Element = pub_dates[0]
+    title_value: dom.Node = title.firstChild
+    pub_date_value: dom.Node = pub_date.firstChild
+    if not isinstance(title_value, dom.Text) or not isinstance(pub_date_value, dom.Text):
+        return ReleaseInfo()
+
+    return ReleaseInfo(title_value.data, pub_date_value.data)
+
+
+def update_with_pip() -> None:
+    import subprocess
+    import sys
+
+    from . import __original_name__
+
+    subprocess.Popen(args=[
+        sys.executable, '-c',
+        f'''import sys, subprocess, time; time.sleep(2);\
+        subprocess.run(args=[sys.executable, '-m', 'pip', 'install', '-U', {__original_name__!r}]);\
+        subprocess.Popen(args=[sys.executable, '-m', {__original_name__!r}])'''])
+    sys.exit(0)
```

### Comparing `pycatsearch-5.1.3/src/pycatsearch.egg-info/PKG-INFO` & `pycatsearch-5.1.4/src/pycatsearch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycatsearch
-Version: 5.1.3
+Version: 5.1.4
 Summary: Yet another implementation of JPL and CDMS spectroscopy catalogs offline search
 Author-email: StSav012 <stsav012@gmail.com>
 License: LGPL-3.0-only
 Project-URL: Source Code, https://github.com/StSav012/pycatsearch
 Project-URL: Bug Tracker, https://github.com/StSav012/pycatsearch/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Win32 (MS Windows)
@@ -20,15 +20,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Chemistry
-Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # PyCatSearch
```

### Comparing `pycatsearch-5.1.3/src/pycatsearch.egg-info/SOURCES.txt` & `pycatsearch-5.1.4/src/pycatsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.3/updater.py` & `pycatsearch-5.1.4/updater.py`

 * *Files identical despite different names*

