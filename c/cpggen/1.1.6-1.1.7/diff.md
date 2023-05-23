# Comparing `tmp/cpggen-1.1.6.tar.gz` & `tmp/cpggen-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpggen-1.1.6.tar", max compression
+gzip compressed data, was "cpggen-1.1.7.tar", max compression
```

## Comparing `cpggen-1.1.6.tar` & `cpggen-1.1.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-05-23 16:49:47.838062 cpggen-1.1.6/LICENSE
--rw-r--r--   0        0        0    12901 2023-05-23 16:49:47.842062 cpggen-1.1.6/README.md
--rw-r--r--   0        0        0        0 2023-05-23 16:49:47.842062 cpggen-1.1.6/cpggen/__init__.py
--rw-r--r--   0        0        0    21252 2023-05-23 16:49:47.842062 cpggen-1.1.6/cpggen/cli.py
--rw-r--r--   0        0        0    41249 2023-05-23 16:49:47.842062 cpggen-1.1.6/cpggen/executor.py
--rw-r--r--   0        0        0     1079 2023-05-23 16:49:47.842062 cpggen-1.1.6/cpggen/logger.py
--rw-r--r--   0        0        0        0 2023-05-23 16:49:47.842062 cpggen-1.1.6/cpggen/source/__init__.py
--rw-r--r--   0        0        0     4001 2023-05-23 16:49:47.842062 cpggen-1.1.6/cpggen/source/ghsa.py
--rw-r--r--   0        0        0    18139 2023-05-23 16:49:47.842062 cpggen-1.1.6/cpggen/utils.py
--rw-r--r--   0        0        0     1363 2023-05-23 16:49:47.842062 cpggen-1.1.6/pyproject.toml
--rw-r--r--   0        0        0    14172 1970-01-01 00:00:00.000000 cpggen-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-23 19:15:31.782543 cpggen-1.1.7/LICENSE
+-rw-r--r--   0        0        0    12901 2023-05-23 19:15:31.782543 cpggen-1.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 19:15:31.782543 cpggen-1.1.7/cpggen/__init__.py
+-rw-r--r--   0        0        0    21095 2023-05-23 19:15:31.782543 cpggen-1.1.7/cpggen/cli.py
+-rw-r--r--   0        0        0    41249 2023-05-23 19:15:31.782543 cpggen-1.1.7/cpggen/executor.py
+-rw-r--r--   0        0        0     1079 2023-05-23 19:15:31.782543 cpggen-1.1.7/cpggen/logger.py
+-rw-r--r--   0        0        0        0 2023-05-23 19:15:31.782543 cpggen-1.1.7/cpggen/source/__init__.py
+-rw-r--r--   0        0        0     4001 2023-05-23 19:15:31.782543 cpggen-1.1.7/cpggen/source/ghsa.py
+-rw-r--r--   0        0        0    18139 2023-05-23 19:15:31.782543 cpggen-1.1.7/cpggen/utils.py
+-rw-r--r--   0        0        0     1363 2023-05-23 19:15:31.786543 cpggen-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0    14172 1970-01-01 00:00:00.000000 cpggen-1.1.7/PKG-INFO
```

### Comparing `cpggen-1.1.6/LICENSE` & `cpggen-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cpggen-1.1.6/README.md` & `cpggen-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `cpggen-1.1.6/cpggen/cli.py` & `cpggen-1.1.7/cpggen/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,19 @@
 
 def build_args():
     """
     Constructs command line arguments for the scanner
     """
     parser = argparse.ArgumentParser(description="CPG Generator")
     parser.add_argument(
-        "-i", "--src", dest="src", help="Source directory or url or CVE or GHSA id", default=os.getcwd()
+        "-i",
+        "--src",
+        dest="src",
+        help="Source directory or url or CVE or GHSA id",
+        default=os.getcwd(),
     )
     parser.add_argument(
         "-o", "--out-dir", dest="cpg_out_dir", help="CPG output directory"
     )
     parser.add_argument(
         "-l",
         "--lang",
@@ -192,15 +196,14 @@
     """Method to generate CPG via the http route"""
     q = request.args
     params = await request.get_json()
     url = ""
     src = ""
     languages = ""
     cpg_out_dir = None
-    is_temp_dir = False
     auto_build = True
     skip_sbom = True
     export = False
     should_slice = False
     use_parse = False
     slice_mode = "Usages"
     app_manifest_list = []
@@ -247,23 +250,23 @@
     if params.get("vectors", "") in ("True", "true", "1"):
         vectors = True
     if params.get("slice_mode"):
         slice_mode = params.get("slice_mode")
     if not src and not url:
         return {"error": "true", "message": "path or url is required"}, 500
     # If src contains url, then reassign
-    if not os.path.isdir(src) and not os.path.isfile(src):
-        url = src
+    if not src and url:
+        src = url
+    if not os.path.exists(src):
         clone_dir = tempfile.mkdtemp(prefix="cpggen")
         if src.startswith("http") or src.startswith("git://"):
             utils.clone_repo(url, clone_dir)
         else:
             utils.download_package_unsafe(url, clone_dir)
         src = clone_dir
-        is_temp_dir = True
     if not cpg_out_dir:
         cpg_out_dir = tempfile.mkdtemp(prefix="cpggen_cpg_out")
     if cpg_out_dir and not os.path.exists(cpg_out_dir):
         os.makedirs(cpg_out_dir, exist_ok=True)
     if not languages or languages == "autodetect":
         languages = utils.detect_project_type(src)
     else:
@@ -317,16 +320,14 @@
                         "slice_out": ml.get("slice_out"),
                     },
                 )
                 if not os.path.exists(ml.get("slice_out")):
                     errors_warnings.append(
                         f"""CPG slice file was not found at {ml.get("slice_out")}"""
                     )
-    if is_temp_dir and src.startswith(tempfile.gettempdir()):
-        shutil.rmtree(src, ignore_errors=True)
     return {
         "success": False if errors_warnings else True,
         "message": "\n".join(errors_warnings)
         if errors_warnings
         else f"CPG generated successfully at {cpg_out_dir}",
         "out_dir": cpg_out_dir,
         "app_manifests": app_manifest_list,
@@ -342,15 +343,15 @@
 
 def get_output_dir(src, cpg_out_dir=None, export_out_dir=None):
     """Method to determine and create the cpg and export output directories"""
     if not src:
         return None, None, False
     is_temp_dir = False
     # purl, http url or CVE id
-    if not os.path.isdir(src) and not os.path.isfile(src):
+    if not os.path.exists(src):
         if not cpg_out_dir:
             cpg_out_dir = tempfile.mkdtemp(prefix="cpggen_cpg_out")
             is_temp_dir = True
         if not export_out_dir:
             export_out_dir = tempfile.mkdtemp(prefix="cpggen_export_out")
             is_temp_dir = True
     if not cpg_out_dir:
```

### Comparing `cpggen-1.1.6/cpggen/executor.py` & `cpggen-1.1.7/cpggen/executor.py`

 * *Files identical despite different names*

### Comparing `cpggen-1.1.6/cpggen/logger.py` & `cpggen-1.1.7/cpggen/logger.py`

 * *Files identical despite different names*

### Comparing `cpggen-1.1.6/cpggen/source/ghsa.py` & `cpggen-1.1.7/cpggen/source/ghsa.py`

 * *Files identical despite different names*

### Comparing `cpggen-1.1.6/cpggen/utils.py` & `cpggen-1.1.7/cpggen/utils.py`

 * *Files identical despite different names*

### Comparing `cpggen-1.1.6/pyproject.toml` & `cpggen-1.1.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cpggen"
-version = "1.1.6"
+version = "1.1.7"
 description = "Generate CPG for multiple languages for use with joern"
 authors = ["Team AppThreat <cloud@appthreat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "cpggen"}]
 homepage = "https://github.com/AppThreat/cpggen"
 repository = "https://github.com/AppThreat/cpggen"
```

### Comparing `cpggen-1.1.6/PKG-INFO` & `cpggen-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpggen
-Version: 1.1.6
+Version: 1.1.7
 Summary: Generate CPG for multiple languages for use with joern
 Home-page: https://github.com/AppThreat/cpggen
 License: Apache-2.0
 Keywords: joern,code analysis,static analysis,cpg,code property graph
 Author: Team AppThreat
 Author-email: cloud@appthreat.com
 Requires-Python: >=3.8.1,<3.12
```

