# Comparing `tmp/pyloobins-0.1.8.tar.gz` & `tmp/pyloobins-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyloobins-0.1.8.tar", max compression
+gzip compressed data, was "pyloobins-0.1.9.tar", max compression
```

## Comparing `pyloobins-0.1.8.tar` & `pyloobins-0.1.9.tar`

### file list

```diff
@@ -1,34 +1,38 @@
--rw-r--r--   0        0        0    35149 2023-04-11 23:56:04.085551 pyloobins-0.1.8/LICENSE
--rw-r--r--   0        0        0      885 2023-05-01 23:30:07.408912 pyloobins-0.1.8/LOOBins/GetFileInfo.yml
--rw-r--r--   0        0        0     1412 2023-05-01 23:30:07.409275 pyloobins-0.1.8/LOOBins/SetFile.yml
--rw-r--r--   0        0        0     1410 2023-05-17 23:34:53.847985 pyloobins-0.1.8/LOOBins/csrutil.yml
--rw-r--r--   0        0        0     2449 2023-05-08 00:30:49.737329 pyloobins-0.1.8/LOOBins/ditto.yml
--rw-r--r--   0        0        0     1644 2023-05-20 14:12:36.410173 pyloobins-0.1.8/LOOBins/dns-sd.yml
--rw-r--r--   0        0        0     3545 2023-05-01 23:30:07.409751 pyloobins-0.1.8/LOOBins/dscl.yml
--rw-r--r--   0        0        0     2138 2023-05-01 23:30:07.409978 pyloobins-0.1.8/LOOBins/ioreg.yml
--rw-r--r--   0        0        0     1538 2023-05-01 01:46:27.775139 pyloobins-0.1.8/LOOBins/last.yml
--rw-r--r--   0        0        0     1869 2023-05-17 23:34:53.848702 pyloobins-0.1.8/LOOBins/lsregister.yml
--rw-r--r--   0        0        0     1763 2023-05-14 23:57:44.222650 pyloobins-0.1.8/LOOBins/mdfind.yml
--rw-r--r--   0        0        0     4420 2023-05-01 23:30:07.410858 pyloobins-0.1.8/LOOBins/networksetup.yml
--rw-r--r--   0        0        0      868 2023-05-15 00:11:31.657614 pyloobins-0.1.8/LOOBins/open.yml
--rw-r--r--   0        0        0     1229 2023-05-15 23:03:47.041630 pyloobins-0.1.8/LOOBins/osacompile.yml
--rw-r--r--   0        0        0     3237 2023-05-01 23:30:07.411097 pyloobins-0.1.8/LOOBins/osascript.yml
--rw-r--r--   0        0        0     1263 2023-05-01 23:30:07.411462 pyloobins-0.1.8/LOOBins/pbpaste.yml
--rw-r--r--   0        0        0     1259 2023-05-11 01:22:04.795362 pyloobins-0.1.8/LOOBins/plutil.yml
--rw-r--r--   0        0        0     1249 2023-05-17 23:34:53.848926 pyloobins-0.1.8/LOOBins/profiles.yml
--rw-r--r--   0        0        0     1051 2023-05-01 01:46:27.801548 pyloobins-0.1.8/LOOBins/screencapture.yml
--rw-r--r--   0        0        0     2458 2023-05-01 01:46:27.474479 pyloobins-0.1.8/LOOBins/security.yml
--rw-r--r--   0        0        0      840 2023-05-01 23:30:07.411670 pyloobins-0.1.8/LOOBins/softwareupdate.yml
--rw-r--r--   0        0        0      790 2023-05-01 23:30:07.411980 pyloobins-0.1.8/LOOBins/sysctl.yml
--rw-r--r--   0        0        0     1158 2023-05-18 14:49:43.472269 pyloobins-0.1.8/LOOBins/tclsh.yml
--rw-r--r--   0        0        0     1993 2023-05-11 01:17:33.005665 pyloobins-0.1.8/LOOBins/textutil.yml
--rw-r--r--   0        0        0     2034 2023-05-06 18:13:38.210711 pyloobins-0.1.8/LOOBins/tmutil.yml
--rw-r--r--   0        0        0     1636 2023-04-23 17:34:43.219172 pyloobins-0.1.8/LOOBins/xattr.yml
--rw-r--r--   0        0        0     1011 2023-05-21 12:12:36.819967 pyloobins-0.1.8/docs/pyloobins/README.md
--rw-r--r--   0        0        0     1227 2023-05-21 12:37:41.843961 pyloobins-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-07 02:06:55.452190 pyloobins-0.1.8/src/pyloobins/__init__.py
--rw-r--r--   0        0        0     2182 2023-05-21 12:27:21.858770 pyloobins-0.1.8/src/pyloobins/cli.py
--rw-r--r--   0        0        0     4015 2023-05-15 23:42:52.127853 pyloobins-0.1.8/src/pyloobins/models.py
--rw-r--r--   0        0        0     1311 2023-05-01 23:30:07.412430 pyloobins-0.1.8/src/pyloobins/templates/loobin.md.j2
--rw-r--r--   0        0        0     2761 2023-05-21 12:27:14.980058 pyloobins-0.1.8/src/pyloobins/util.py
--rw-r--r--   0        0        0     1894 1970-01-01 00:00:00.000000 pyloobins-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-11 23:56:04.085551 pyloobins-0.1.9/LICENSE
+-rw-r--r--   0        0        0      885 2023-05-01 23:30:07.408912 pyloobins-0.1.9/LOOBins/GetFileInfo.yml
+-rw-r--r--   0        0        0     1412 2023-05-01 23:30:07.409275 pyloobins-0.1.9/LOOBins/SetFile.yml
+-rw-r--r--   0        0        0     1410 2023-05-17 23:34:53.847985 pyloobins-0.1.9/LOOBins/csrutil.yml
+-rw-r--r--   0        0        0     2449 2023-05-08 00:30:49.737329 pyloobins-0.1.9/LOOBins/ditto.yml
+-rw-r--r--   0        0        0     1644 2023-05-20 14:12:36.410173 pyloobins-0.1.9/LOOBins/dns-sd.yml
+-rw-r--r--   0        0        0     3545 2023-05-01 23:30:07.409751 pyloobins-0.1.9/LOOBins/dscl.yml
+-rw-r--r--   0        0        0     2046 2023-05-23 12:32:36.331097 pyloobins-0.1.9/LOOBins/hdiutil.yml
+-rw-r--r--   0        0        0     2138 2023-05-01 23:30:07.409978 pyloobins-0.1.9/LOOBins/ioreg.yml
+-rw-r--r--   0        0        0     1538 2023-05-01 01:46:27.775139 pyloobins-0.1.9/LOOBins/last.yml
+-rw-r--r--   0        0        0     1869 2023-05-17 23:34:53.848702 pyloobins-0.1.9/LOOBins/lsregister.yml
+-rw-r--r--   0        0        0     1763 2023-05-14 23:57:44.222650 pyloobins-0.1.9/LOOBins/mdfind.yml
+-rw-r--r--   0        0        0     4420 2023-05-01 23:30:07.410858 pyloobins-0.1.9/LOOBins/networksetup.yml
+-rw-r--r--   0        0        0      753 2023-05-23 12:32:36.331361 pyloobins-0.1.9/LOOBins/nscurl.yml
+-rw-r--r--   0        0        0      868 2023-05-15 00:11:31.657614 pyloobins-0.1.9/LOOBins/open.yml
+-rw-r--r--   0        0        0     1229 2023-05-15 23:03:47.041630 pyloobins-0.1.9/LOOBins/osacompile.yml
+-rw-r--r--   0        0        0     3237 2023-05-01 23:30:07.411097 pyloobins-0.1.9/LOOBins/osascript.yml
+-rw-r--r--   0        0        0     1263 2023-05-01 23:30:07.411462 pyloobins-0.1.9/LOOBins/pbpaste.yml
+-rw-r--r--   0        0        0     1259 2023-05-11 01:22:04.795362 pyloobins-0.1.9/LOOBins/plutil.yml
+-rw-r--r--   0        0        0     1249 2023-05-17 23:34:53.848926 pyloobins-0.1.9/LOOBins/profiles.yml
+-rw-r--r--   0        0        0     1206 2023-05-21 12:51:13.791530 pyloobins-0.1.9/LOOBins/safaridriver.yml
+-rw-r--r--   0        0        0     1051 2023-05-01 01:46:27.801548 pyloobins-0.1.9/LOOBins/screencapture.yml
+-rw-r--r--   0        0        0     2458 2023-05-01 01:46:27.474479 pyloobins-0.1.9/LOOBins/security.yml
+-rw-r--r--   0        0        0      840 2023-05-01 23:30:07.411670 pyloobins-0.1.9/LOOBins/softwareupdate.yml
+-rw-r--r--   0        0        0     1118 2023-05-23 12:32:36.331549 pyloobins-0.1.9/LOOBins/ssh-keygen.yml
+-rw-r--r--   0        0        0      790 2023-05-01 23:30:07.411980 pyloobins-0.1.9/LOOBins/sysctl.yml
+-rw-r--r--   0        0        0     1158 2023-05-18 14:49:43.472269 pyloobins-0.1.9/LOOBins/tclsh.yml
+-rw-r--r--   0        0        0     1993 2023-05-11 01:17:33.005665 pyloobins-0.1.9/LOOBins/textutil.yml
+-rw-r--r--   0        0        0     2034 2023-05-06 18:13:38.210711 pyloobins-0.1.9/LOOBins/tmutil.yml
+-rw-r--r--   0        0        0     1636 2023-04-23 17:34:43.219172 pyloobins-0.1.9/LOOBins/xattr.yml
+-rw-r--r--   0        0        0     1011 2023-05-21 12:12:36.819967 pyloobins-0.1.9/docs/pyloobins/README.md
+-rw-r--r--   0        0        0     1227 2023-05-23 12:32:36.331803 pyloobins-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-07 02:06:55.452190 pyloobins-0.1.9/src/pyloobins/__init__.py
+-rw-r--r--   0        0        0     2182 2023-05-21 12:27:21.858770 pyloobins-0.1.9/src/pyloobins/cli.py
+-rw-r--r--   0        0        0     4015 2023-05-15 23:42:52.127853 pyloobins-0.1.9/src/pyloobins/models.py
+-rw-r--r--   0        0        0     1311 2023-05-01 23:30:07.412430 pyloobins-0.1.9/src/pyloobins/templates/loobin.md.j2
+-rw-r--r--   0        0        0     2768 2023-05-23 12:32:36.332053 pyloobins-0.1.9/src/pyloobins/util.py
+-rw-r--r--   0        0        0     1894 1970-01-01 00:00:00.000000 pyloobins-0.1.9/PKG-INFO
```

### Comparing `pyloobins-0.1.8/LICENSE` & `pyloobins-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.8/LOOBins/GetFileInfo.yml` & `pyloobins-0.1.9/LOOBins/GetFileInfo.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.8/LOOBins/SetFile.yml` & `pyloobins-0.1.9/LOOBins/SetFile.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.8/LOOBins/csrutil.yml` & `pyloobins-0.1.9/LOOBins/csrutil.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.8/LOOBins/ditto.yml` & `pyloobins-0.1.9/LOOBins/ditto.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.8/LOOBins/dns-sd.yml` & `pyloobins-0.1.9/LOOBins/dns-sd.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.8/LOOBins/dscl.yml` & `pyloobins-0.1.9/LOOBins/dscl.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.8/LOOBins/ioreg.yml` & `pyloobins-0.1.9/LOOBins/ioreg.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.8/LOOBins/last.yml` & `pyloobins-0.1.9/LOOBins/last.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.8/LOOBins/lsregister.yml` & `pyloobins-0.1.9/LOOBins/lsregister.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.8/LOOBins/mdfind.yml` & `pyloobins-0.1.9/LOOBins/mdfind.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.8/LOOBins/networksetup.yml` & `pyloobins-0.1.9/LOOBins/networksetup.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.8/LOOBins/open.yml` & `pyloobins-0.1.9/LOOBins/open.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.8/LOOBins/osacompile.yml` & `pyloobins-0.1.9/LOOBins/osacompile.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.8/LOOBins/osascript.yml` & `pyloobins-0.1.9/LOOBins/osascript.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.8/LOOBins/pbpaste.yml` & `pyloobins-0.1.9/LOOBins/pbpaste.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.8/LOOBins/plutil.yml` & `pyloobins-0.1.9/LOOBins/plutil.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.8/LOOBins/profiles.yml` & `pyloobins-0.1.9/LOOBins/profiles.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.8/LOOBins/screencapture.yml` & `pyloobins-0.1.9/LOOBins/screencapture.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.8/LOOBins/security.yml` & `pyloobins-0.1.9/LOOBins/security.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.8/LOOBins/softwareupdate.yml` & `pyloobins-0.1.9/LOOBins/softwareupdate.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.8/LOOBins/sysctl.yml` & `pyloobins-0.1.9/LOOBins/sysctl.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.8/LOOBins/tclsh.yml` & `pyloobins-0.1.9/LOOBins/tclsh.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.8/LOOBins/textutil.yml` & `pyloobins-0.1.9/LOOBins/textutil.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.8/LOOBins/tmutil.yml` & `pyloobins-0.1.9/LOOBins/tmutil.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.8/LOOBins/xattr.yml` & `pyloobins-0.1.9/LOOBins/xattr.yml`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.8/docs/pyloobins/README.md` & `pyloobins-0.1.9/docs/pyloobins/README.md`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.8/pyproject.toml` & `pyloobins-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PyLOOBins"
-version = "0.1.8"
+version = "0.1.9"
 description = "Python package for managing the LOOBins model and schema."
 authors = ["infosecB <brendan@infosecb.com>"]
 readme = "docs/pyloobins/README.md"
 packages = [{include = "pyloobins", from = "src"}]
 include = ["LOOBins/*.yml"]
 homepage = "https://loobins.io/"
 repository = "https://github.com/infosecB/LOOBins"
```

### Comparing `pyloobins-0.1.8/src/pyloobins/cli.py` & `pyloobins-0.1.9/src/pyloobins/cli.py`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.8/src/pyloobins/models.py` & `pyloobins-0.1.9/src/pyloobins/models.py`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.8/src/pyloobins/templates/loobin.md.j2` & `pyloobins-0.1.9/src/pyloobins/templates/loobin.md.j2`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.8/src/pyloobins/util.py` & `pyloobins-0.1.9/src/pyloobins/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Utility functions that support the CLI and library"""
 import pathlib
-import site
 from datetime import date
 
 import yaml
 
+import pyloobins
 from .models import Detection, ExampleUseCase, LOOBin, Resource
 
 
 def get_loobins(path: str = "") -> list:
     """Returns a list of LOOBin objects"""
     loobins = []
     if path:
         yml_files = pathlib.Path(path).glob("**/*.yml")
     else:
-        yml_files = (pathlib.Path(site.getsitepackages()[0]) / "LOOBins").glob(
+        yml_files = (pathlib.Path(pyloobins.__file__).parents[1]/"LOOBins").glob(
             "**/*.yml"
         )
     for yml_file in yml_files:
         with open(yml_file, "r", encoding="utf-8") as stream:
             try:
                 yml_content = yaml.safe_load(stream)
             except yaml.YAMLError as exc:
```

### Comparing `pyloobins-0.1.8/PKG-INFO` & `pyloobins-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyloobins
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python package for managing the LOOBins model and schema.
 Home-page: https://loobins.io/
 License: GPL-3.0-or-later
 Keywords: cybersecurity,cli,lol
 Author: infosecB
 Author-email: brendan@infosecb.com
 Requires-Python: >=3.8,<4.0
```

