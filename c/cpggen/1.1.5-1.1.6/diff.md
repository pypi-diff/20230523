# Comparing `tmp/cpggen-1.1.5.tar.gz` & `tmp/cpggen-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpggen-1.1.5.tar", max compression
+gzip compressed data, was "cpggen-1.1.6.tar", max compression
```

## Comparing `cpggen-1.1.5.tar` & `cpggen-1.1.6.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-05-15 09:59:59.282099 cpggen-1.1.5/LICENSE
--rw-r--r--   0        0        0    12219 2023-05-15 09:59:59.282099 cpggen-1.1.5/README.md
--rw-r--r--   0        0        0        0 2023-05-15 09:59:59.286099 cpggen-1.1.5/cpggen/__init__.py
--rw-r--r--   0        0        0    21377 2023-05-15 09:59:59.286099 cpggen-1.1.5/cpggen/cli.py
--rw-r--r--   0        0        0    39366 2023-05-15 09:59:59.286099 cpggen-1.1.5/cpggen/executor.py
--rw-r--r--   0        0        0     1078 2023-05-15 09:59:59.286099 cpggen-1.1.5/cpggen/logger.py
--rw-r--r--   0        0        0    14556 2023-05-15 09:59:59.286099 cpggen-1.1.5/cpggen/utils.py
--rw-r--r--   0        0        0     1326 2023-05-15 09:59:59.286099 cpggen-1.1.5/pyproject.toml
--rw-r--r--   0        0        0    13591 1970-01-01 00:00:00.000000 cpggen-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-23 16:49:47.838062 cpggen-1.1.6/LICENSE
+-rw-r--r--   0        0        0    12901 2023-05-23 16:49:47.842062 cpggen-1.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 16:49:47.842062 cpggen-1.1.6/cpggen/__init__.py
+-rw-r--r--   0        0        0    21252 2023-05-23 16:49:47.842062 cpggen-1.1.6/cpggen/cli.py
+-rw-r--r--   0        0        0    41249 2023-05-23 16:49:47.842062 cpggen-1.1.6/cpggen/executor.py
+-rw-r--r--   0        0        0     1079 2023-05-23 16:49:47.842062 cpggen-1.1.6/cpggen/logger.py
+-rw-r--r--   0        0        0        0 2023-05-23 16:49:47.842062 cpggen-1.1.6/cpggen/source/__init__.py
+-rw-r--r--   0        0        0     4001 2023-05-23 16:49:47.842062 cpggen-1.1.6/cpggen/source/ghsa.py
+-rw-r--r--   0        0        0    18139 2023-05-23 16:49:47.842062 cpggen-1.1.6/cpggen/utils.py
+-rw-r--r--   0        0        0     1363 2023-05-23 16:49:47.842062 cpggen-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0    14172 1970-01-01 00:00:00.000000 cpggen-1.1.6/PKG-INFO
```

### Comparing `cpggen-1.1.5/LICENSE` & `cpggen-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cpggen-1.1.5/README.md` & `cpggen-1.1.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 ██║     ██╔═══╝ ██║   ██║
 ╚██████╗██║     ╚██████╔╝
  ╚═════╝╚═╝      ╚═════╝
 ```
 
 CPG Generator is a python cli tool to generate [Code Property Graph](https://cpg.joern.io) for multiple languages. The generated CPG can be directly imported to [Joern](https://joern.io) or uploaded to [Qwiet.AI](https://docs.shiftleft.io/home) for analysis.
 
+[![release](https://github.com/appthreat/cpggen/actions/workflows/pythonpublish.yml/badge.svg)](https://github.com/appthreat/cpggen/actions/workflows/pythonpublish.yml)
+[![Downloads](https://static.pepy.tech/badge/cpggen)](https://pepy.tech/project/cpggen)
+[![Discord](https://img.shields.io/badge/-Discord-lime?style=for-the-badge&logo=discord&logoColor=white&color=black)](https://discord.gg/tmmtjCEHNV)
+
 ## Pre-requisites
 
 - JDK 11 or above
 - Python 3.10
 - Docker or podman (Windows, Linux or Mac) or
 - Joern [natively installed](https://docs.joern.io/installation) (Linux only)
 
@@ -27,23 +31,23 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
 - Joern with all the CPG frontends
 - cpggen with Python 3.10
 - cdxgen with Node.js 18 - Generates SBoM
 
 ```bash
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.1.5/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/latest/download/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v1.1.5/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/latest/download/cpggen.exe
 .\cpggen.exe --help
 ```
 
 NOTE: On Windows, antivirus and antimalware could prevent this single executable from functioning properly. Depending on the system, administrative privileges might also be required. Use container-based execution as a fallback.
 
 ### OCI Artifacts via ORAS cli
 
@@ -127,24 +131,31 @@
 
 To specify input and output directory.
 
 ```
 cpggen -i <src directory> -o <CPG directory or file name>
 ```
 
-You can even pass a git or a package url as source
+You can even pass a git or a package url or CVE id as source
 
 ```
 cpggen -i https://github.com/HooliCorp/vulnerable-aws-koa-app -o /tmp/cpg
 ```
 
 ```
 cpggen -i "pkg:maven/org.apache.commons/commons-io@1.3.2" -o /tmp/cpg
 ```
 
+```
+export GITHUB_TOKEN=<token with read:packages scope>
+cpggen -i CVE-2023-32681 -o /tmp/cpg
+
+cpggen -i GHSA-j8r2-6x86-q33q -o /tmp/cpg
+```
+
 To specify language type.
 
 ```
 cpggen -i <src directory> -o <CPG directory or file name> -l java
 
 # Comma separated values are accepted for multiple languages
 cpggen -i <src directory> -o <CPG directory or file name> -l java,js,python
@@ -248,15 +259,15 @@
 usage: cpggen [-h] [-i SRC] [-o CPG_OUT_DIR] [-l LANGUAGE] [--use-container] [--build] [--joern-home JOERN_HOME] [--server] [--server-host SERVER_HOST] [--server-port SERVER_PORT] [--export]
               [--export-repr {ast,cfg,cdg,ddg,pdg,cpg,cpg14,all}] [--export-format {neo4jcsv,graphml,graphson,dot}] [--export-out-dir EXPORT_OUT_DIR] [--verbose] [--skip-sbom] [--slice] [--slice-mode {Usages,DataFlow}] [--use-parse]
 
 CPG Generator
 
 optional arguments:
   -h, --help            show this help message and exit
-  -i SRC, --src SRC     Source directory or url
+  -i SRC, --src SRC     Source directory or url or CVE or GHSA id
   -o CPG_OUT_DIR, --out-dir CPG_OUT_DIR
                         CPG output directory
   -l LANGUAGE, --lang LANGUAGE
                         Optional. CPG language frontend to use. Auto-detects by default.
   --use-container       Use cpggen docker image
   --build               Attempt to build the project automatically
   --joern-home JOERN_HOME
@@ -299,14 +310,15 @@
 | CPG_SLICE               | Set to true to slice CPG                                                   |
 | CPG_SLICE_MODE          | Slice mode. Default Usages                                                 |
 | CPG_VECTORS             | Set to true to generate vector representations of code from CPG            |
 | SHIFTLEFT_ACCESS_TOKEN  | Set to automatically submit the CPG for analysis by Qwiet AI               |
 | CDXGEN_ARGS             | Extra arguments to pass to cdxgen                                          |
 | ENABLE_SBOM             | Enable SBoM generation using cdxgen                                        |
 | JIMPLE_ANDROID_JAR      | Path to android.jar for use with jimple for .apk or .dex to CPG conversion |
+| GITHUB_TOKEN            | Token with read:packages scope to analyze CVE or GitHub Advisory           |
 
 ## GitHub actions
 
 Use the marketplace [action](https://github.com/marketplace/actions/cpggen) to generate CPGs using GitHub actions. Optionally, the upload the generated CPGs as build artifacts use the below step.
 
 ```
 - name: Upload cpg
```

### Comparing `cpggen-1.1.5/cpggen/cli.py` & `cpggen-1.1.6/cpggen/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import argparse
-import json
 import os
 import shutil
 import signal
 import sys
 import tempfile
 from multiprocessing import Pool, freeze_support
 from pathlib import Path, PurePath
 
 from quart import Quart, request
 
 from cpggen import executor, utils
 from cpggen.logger import LOG, console, enable_debug
 
-try:
-    os.environ["PYTHONIOENCODING"] = "utf-8"
-    os.environ["PYTHONUTF8"] = 1
-except Exception:
-    pass
+os.environ["PYTHONIOENCODING"] = "utf-8"
+os.environ["PYTHONUTF8"] = "1"
 
-product_logo = """
+PRODUCT_LOGO = """
  ██████╗██████╗  ██████╗
 ██╔════╝██╔══██╗██╔════╝
 ██║     ██████╔╝██║  ███╗
 ██║     ██╔═══╝ ██║   ██║
 ╚██████╗██║     ╚██████╔╝
  ╚═════╝╚═╝      ╚═════╝
 """
@@ -37,15 +33,15 @@
 
 def build_args():
     """
     Constructs command line arguments for the scanner
     """
     parser = argparse.ArgumentParser(description="CPG Generator")
     parser.add_argument(
-        "-i", "--src", dest="src", help="Source directory or url", default=os.getcwd()
+        "-i", "--src", dest="src", help="Source directory or url or CVE or GHSA id", default=os.getcwd()
     )
     parser.add_argument(
         "-o", "--out-dir", dest="cpg_out_dir", help="CPG output directory"
     )
     parser.add_argument(
         "-l",
         "--lang",
@@ -154,15 +150,16 @@
         dest="slice_mode",
         choices=["Usages", "DataFlow"],
         help="Mode used for CPG slicing",
     )
     parser.add_argument(
         "--use-parse",
         dest="use_parse",
-        help="Use joern-parse command instead of invoking the language frontends. Useful when default overlays are important",
+        help="Use joern-parse command instead of invoking the language frontends. Useful when default overlays are "
+        "important",
         action="store_true",
         default=False,
     )
     parser.add_argument(
         "--vectors",
         action="store_true",
         default=True if os.getenv("CPG_VECTORS") in ("true", "1") else False,
@@ -170,42 +167,44 @@
         help="Extract vector representations of code from CPG",
     )
     return parser.parse_args()
 
 
 @app.get("/")
 async def index():
+    """Index route"""
     return {}
 
 
 def run_server(args):
-    console.print(product_logo, style="info")
+    """Run cpggen as a server"""
+    console.print(PRODUCT_LOGO, style="info")
     console.print(f"cpggen server running on {args.server_host}:{args.server_port}")
     app.run(
         host=args.server_host,
         port=args.server_port,
         debug=True if os.getenv("AT_DEBUG_MODE") in ("debug", "true", "1") else False,
         use_reloader=False,
     )
 
 
 @app.route("/cpg", methods=["GET", "POST"])
 async def generate_cpg():
+    """Method to generate CPG via the http route"""
     q = request.args
     params = await request.get_json()
     url = ""
     src = ""
     languages = ""
     cpg_out_dir = None
-    export_out_dir = None
     is_temp_dir = False
     auto_build = True
     skip_sbom = True
     export = False
-    slice = False
+    should_slice = False
     use_parse = False
     slice_mode = "Usages"
     app_manifest_list = []
     errors_warnings = []
     vectors = False
     if not params:
         params = {}
@@ -216,15 +215,15 @@
     if q.get("out_dir"):
         cpg_out_dir = q.get("out_dir")
     if q.get("lang"):
         languages = q.get("lang")
     if q.get("export", "") in ("True", "true", "1"):
         export = True
     if q.get("slice", "") in ("True", "true", "1"):
-        slice = True
+        should_slice = True
     if q.get("vectors", "") in ("True", "true", "1"):
         vectors = True
     if q.get("slice_mode"):
         slice_mode = q.get("slice_mode")
     if q.get("auto_build", "") in ("False", "false", "0"):
         auto_build = False
     if q.get("skip_sbom", "") in ("False", "false", "0"):
@@ -240,39 +239,33 @@
     if params.get("auto_build", "") in ("False", "false", "0"):
         auto_build = False
     if params.get("skip_sbom", "") in ("False", "false", "0"):
         skip_sbom = False
     if params.get("export", "") in ("True", "true", "1"):
         export = True
     if params.get("slice", "") in ("True", "true", "1"):
-        slice = True
+        should_slice = True
     if params.get("vectors", "") in ("True", "true", "1"):
         vectors = True
     if params.get("slice_mode"):
         slice_mode = params.get("slice_mode")
     if not src and not url:
         return {"error": "true", "message": "path or url is required"}, 500
     # If src contains url, then reassign
-    if not url and (
-        src.startswith("http") or src.startswith("git://") or src.startswith("pkg:")
-    ):
+    if not os.path.isdir(src) and not os.path.isfile(src):
         url = src
-    if url:
         clone_dir = tempfile.mkdtemp(prefix="cpggen")
-        if url.startswith("pkg:"):
-            download_file = utils.download_package(url, clone_dir)
-            if download_file and os.path.exists(download_file):
-                src = clone_dir
+        if src.startswith("http") or src.startswith("git://"):
+            utils.clone_repo(url, clone_dir)
         else:
-            src = utils.clone_repo(url, clone_dir)
+            utils.download_package_unsafe(url, clone_dir)
+        src = clone_dir
         is_temp_dir = True
     if not cpg_out_dir:
         cpg_out_dir = tempfile.mkdtemp(prefix="cpggen_cpg_out")
-    if not export_out_dir:
-        export_out_dir = tempfile.mkdtemp(prefix="cpggen_export_out")
     if cpg_out_dir and not os.path.exists(cpg_out_dir):
         os.makedirs(cpg_out_dir, exist_ok=True)
     if not languages or languages == "autodetect":
         languages = utils.detect_project_type(src)
     else:
         languages = languages.split(",")
     for lang in languages:
@@ -290,22 +283,22 @@
             use_container=False,
             use_parse=use_parse,
             auto_build=auto_build,
             extra_args={
                 "skip_sbom": skip_sbom,
                 "slice_mode": slice_mode,
                 "for_export": export,
-                "for_slice": slice,
+                "for_slice": should_slice,
                 "for_vectors": vectors,
                 "url": url,
             },
         )
         if mlist:
             app_manifest_list += mlist
-        if slice and mlist:
+        if should_slice and mlist:
             for ml in mlist:
                 if not os.path.exists(ml.get("cpg")):
                     errors_warnings.append(
                         f"""CPG file was not found at {ml.get("cpg")}"""
                     )
                     continue
                 executor.exec_tool(
@@ -324,20 +317,16 @@
                         "slice_out": ml.get("slice_out"),
                     },
                 )
                 if not os.path.exists(ml.get("slice_out")):
                     errors_warnings.append(
                         f"""CPG slice file was not found at {ml.get("slice_out")}"""
                     )
-    if is_temp_dir:
-        try:
-            os.remove(src)
-        except Exception:
-            # Ignore cleanup errors
-            pass
+    if is_temp_dir and src.startswith(tempfile.gettempdir()):
+        shutil.rmtree(src, ignore_errors=True)
     return {
         "success": False if errors_warnings else True,
         "message": "\n".join(errors_warnings)
         if errors_warnings
         else f"CPG generated successfully at {cpg_out_dir}",
         "out_dir": cpg_out_dir,
         "app_manifests": app_manifest_list,
@@ -347,36 +336,77 @@
 def init_worker():
     """
     Handler for worker processes to let their parent handle interruptions
     """
     signal.signal(signal.SIGINT, signal.SIG_IGN)
 
 
+def get_output_dir(src, cpg_out_dir=None, export_out_dir=None):
+    """Method to determine and create the cpg and export output directories"""
+    if not src:
+        return None, None, False
+    is_temp_dir = False
+    # purl, http url or CVE id
+    if not os.path.isdir(src) and not os.path.isfile(src):
+        if not cpg_out_dir:
+            cpg_out_dir = tempfile.mkdtemp(prefix="cpggen_cpg_out")
+            is_temp_dir = True
+        if not export_out_dir:
+            export_out_dir = tempfile.mkdtemp(prefix="cpggen_export_out")
+            is_temp_dir = True
+    if not cpg_out_dir:
+        if os.path.isfile(src):
+            cpg_out_dir = os.path.join(os.path.dirname(src), "cpg_out")
+        else:
+            cpg_out_dir = os.path.join(src, "cpg_out")
+    if not export_out_dir:
+        export_out_dir = os.path.join(src, "cpg_export")
+    cpg_out_dir = str(PurePath(cpg_out_dir))
+    export_out_dir = str(PurePath(export_out_dir))
+    if cpg_out_dir and not os.path.exists(cpg_out_dir):
+        os.makedirs(cpg_out_dir, exist_ok=True)
+    return cpg_out_dir, export_out_dir, is_temp_dir
+
+
 def cpg(
     src,
     cpg_out_dir,
     languages,
     joern_home,
     use_container=False,
     use_parse=False,
     auto_build=False,
     skip_sbom=False,
     export=False,
-    slice=False,
+    should_slice=False,
     slice_mode=None,
-    url=None,
     vectors=False,
 ):
+    """Method to generate cpg using multiple processes"""
     if __name__ in ("__main__", "cpggen.cli"):
         with Pool(processes=os.cpu_count(), initializer=init_worker) as pool:
             try:
                 ret = []
                 exec_results = []
+                url = ""
+                # Where the source is a url or a CVE id download it
+                if not os.path.isdir(src) and not os.path.isfile(src):
+                    url = src
+                    clone_dir = tempfile.mkdtemp(prefix="cpggen")
+                    if src.startswith("http") or src.startswith("git://"):
+                        utils.clone_repo(src, clone_dir)
+                    else:
+                        utils.download_package_unsafe(src, clone_dir)
+                    src = clone_dir
+                    if not languages or languages == "autodetect":
+                        languages = utils.detect_project_type(src)
+                    else:
+                        languages = languages.split(",")
                 for lang in languages:
-                    LOG.debug(f"Generating CPG for the language {lang} at {src}")
+                    LOG.debug("Generating CPG for the language %s at %s", lang, src)
                     exec_results.append(
                         pool.apply_async(
                             executor.exec_tool,
                             (
                                 lang,
                                 src,
                                 cpg_out_dir,
@@ -385,15 +415,15 @@
                                 use_container,
                                 use_parse,
                                 auto_build,
                                 {
                                     "skip_sbom": skip_sbom,
                                     "slice_mode": slice_mode,
                                     "for_export": export,
-                                    "for_slice": slice,
+                                    "for_slice": should_slice,
                                     "for_vectors": vectors,
                                     "url": url,
                                 },
                             ),
                         )
                     )
                 for res in exec_results:
@@ -404,92 +434,76 @@
                 return ret
             except KeyboardInterrupt:
                 pool.terminate()
             pool.join()
     return None
 
 
-def collect_cpg_manifests(cpg_out_dir):
-    cpg_manifests = []
-    if os.path.isfile(cpg_out_dir):
-        cpg_out_dir = os.path.dirname(cpg_out_dir)
-    mfiles = utils.find_files(cpg_out_dir, ".manifest.json") if cpg_out_dir else []
-    for amanifest in mfiles:
-        with open(amanifest) as mfp:
-            manifest_obj = json.load(mfp)
-            cpg_manifests.append(manifest_obj)
-    return cpg_manifests
-
-
 def fix_export_repr(export_repr, export_format):
+    """Method to validate and fix the export representation based on the format"""
     if export_format == "neo4jcsv":
         if export_repr != "cpg":
-            LOG.warn(
+            LOG.warning(
                 "cpg is the only supported export representation for neo4jcsv format"
             )
         return "cpg"
     return export_repr
 
 
 def export_slice_cpg(
-    src,
     cpg_out_dir,
     joern_home,
     use_container,
     use_parse,
     export,
     export_repr,
     export_format,
     export_out_dir,
-    slice,
-    slice_mode,
-    vectors,
+    should_slice=False,
+    slice_mode=None,
+    vectors=False,
     cpg_manifests=None,
 ):
+    """Method to export or slice cpg"""
     if __name__ in ("__main__", "cpggen.cli"):
         with Pool(processes=os.cpu_count(), initializer=init_worker) as pool:
             try:
                 export_tool = "export"
-                if slice:
+                if should_slice:
                     export_tool = "slice"
                 elif vectors:
                     export_tool = "vectors"
                 # Collect the CPG manifests if none was provided.
                 # This could result in duplicate executions
                 if not cpg_manifests:
-                    cpg_manifests = collect_cpg_manifests(cpg_out_dir)
+                    cpg_manifests = utils.collect_cpg_manifests(cpg_out_dir)
                 for manifest_obj in cpg_manifests:
                     if not manifest_obj or not manifest_obj.get("cpg"):
                         continue
                     app_export_out_dir = os.path.join(
                         export_out_dir, manifest_obj["app"]
                     )
-                    try:
-                        # joern-export annoyingly will not overwrite directories
-                        # but would expect first level directories to exist
-                        if os.path.exists(app_export_out_dir):
-                            try:
-                                shutil.rmtree(app_export_out_dir)
-                            except Exception:
-                                # Ignore remove errors
-                                pass
-                        os.makedirs(export_out_dir, exist_ok=True)
-                    except Exception:
-                        # Ignore errors
-                        pass
+                    # joern-export annoyingly will not overwrite directories
+                    # but would expect first level directories to exist
+                    if os.path.exists(app_export_out_dir):
+                        shutil.rmtree(app_export_out_dir, ignore_errors=True)
+                    os.makedirs(export_out_dir, exist_ok=True)
                     cpg_path = manifest_obj["cpg"]
                     # In case of GitHub action we need to fix the cpg_path to prefix GITHUB_WORKSPACE
                     # since the manifest would only have relative path
                     if os.getenv("GITHUB_WORKSPACE") and not cpg_path.startswith(
                         os.getenv("GITHUB_WORKSPACE")
                     ):
                         cpg_path = os.path.join(os.getenv("GITHUB_WORKSPACE"), cpg_path)
                     if export:
                         LOG.debug(
-                            f"""Exporting CPG for the app {manifest_obj["app"]} from {cpg_path} to {app_export_out_dir}"""
+                            """Exporting CPG for the app %s from %s to %s""",
+                            manifest_obj["app"],
+                            cpg_path,
+                            app_export_out_dir,
                         )
                     pool.apply_async(
                         executor.exec_tool,
                         (
                             export_tool,
                             cpg_path,
                             app_export_out_dir,
@@ -501,136 +515,97 @@
                             {
                                 "export_repr": fix_export_repr(
                                     export_repr, export_format
                                 )
                                 if export
                                 else None,
                                 "export_format": export_format if export else None,
-                                "slice_mode": slice_mode if slice else None,
+                                "slice_mode": slice_mode if should_slice else None,
                                 "slice_out": manifest_obj.get("slice_out"),
                             },
                         ),
                     )
                 pool.close()
             except KeyboardInterrupt:
                 pool.terminate()
             pool.join()
 
 
 def main():
-    print(product_logo)
+    """Main method"""
+    print(PRODUCT_LOGO)
     args = build_args()
     # Turn on verbose mode
     if args.verbose_mode:
         enable_debug()
     if args.server_mode:
         return run_server(args)
     src = args.src
-    cpg_out_dir = args.cpg_out_dir
-    export_out_dir = args.export_out_dir
-    if (
-        not src.startswith("http")
-        and not src.startswith("git://")
-        and not src.startswith("pkg:")
-    ):
-        src = str(PurePath(args.src))
-        if not cpg_out_dir and src:
-            if os.path.isfile(src):
-                cpg_out_dir = os.path.join(os.path.dirname(src), "cpg_out")
-            else:
-                cpg_out_dir = os.path.join(src, "cpg_out")
-        if not export_out_dir and src:
-            export_out_dir = os.path.join(src, "cpg_export")
-    if cpg_out_dir:
-        cpg_out_dir = str(PurePath(cpg_out_dir))
-    if export_out_dir:
-        export_out_dir = str(PurePath(export_out_dir))
-    languages = args.language
+    cpg_out_dir, export_out_dir, is_temp_dir = get_output_dir(
+        src, args.cpg_out_dir, args.export_out_dir
+    )
+    if os.path.exists(src):
+        src = str(PurePath(src))
     joern_home = args.joern_home
     use_container = args.use_container
     use_parse = args.use_parse
     is_bundled_exe = False
     try:
         if getattr(sys, "_MEIPASS"):
             is_bundled_exe = True
             # Reset joern_home for bundled exe
             if not os.path.exists(joern_home):
                 joern_home = ""
-    except Exception:
+    except AttributeError:
         pass
     if joern_home and not os.path.exists(joern_home) and not is_bundled_exe:
         if utils.check_command("docker") or utils.check_command("podman"):
             use_container = True
         else:
             console.print(
-                "Joern installation was not found. Please install joern by following the instructions at https://joern.io and set the environment variable JOERN_HOME to the directory containing the cli tools"
+                "Joern installation was not found. Please install joern by following the instructions at "
+                "https://joern.io and set the environment variable JOERN_HOME to the directory containing the cli tools"
             )
             console.print(
                 "Alternatively, ensure docker or podman is available to use cpggen container image"
             )
     # GitHub action is very weird
     if os.getenv("GITHUB_PATH") and utils.check_command("joern"):
         joern_home = ""
-    is_temp_dir = False
-    url = ""
-    if src.startswith("http") or src.startswith("git://") or src.startswith("pkg:"):
-        url = src
-        clone_dir = tempfile.mkdtemp(prefix="cpggen")
-        if src.startswith("pkg:"):
-            download_file = utils.download_package(src, clone_dir)
-            if download_file and os.path.exists(download_file):
-                src = clone_dir
-        else:
-            src = utils.clone_repo(src, clone_dir)
-        is_temp_dir = True
-        if not cpg_out_dir:
-            cpg_out_dir = tempfile.mkdtemp(prefix="cpggen_cpg_out")
-        if not export_out_dir:
-            export_out_dir = tempfile.mkdtemp(prefix="cpggen_export_out")
-    if not languages or languages == "autodetect":
-        languages = utils.detect_project_type(src)
-    else:
-        languages = languages.split(",")
-    if cpg_out_dir and not os.path.exists(cpg_out_dir):
-        os.makedirs(cpg_out_dir, exist_ok=True)
     cpg_manifests = cpg(
         src,
         cpg_out_dir,
-        languages,
+        args.language,
         joern_home=joern_home,
         use_container=use_container,
         use_parse=use_parse,
         auto_build=args.auto_build,
         skip_sbom=args.skip_sbom,
         export=args.export,
-        slice=args.slice,
+        should_slice=args.slice,
         slice_mode=args.slice_mode,
-        url=url,
         vectors=args.vectors,
     )
     if args.export or args.slice or args.vectors:
         export_slice_cpg(
-            src,
             cpg_out_dir,
             joern_home=joern_home,
             use_container=use_container,
             use_parse=use_parse,
             export=args.export,
             export_repr=args.export_repr,
             export_format=args.export_format,
             export_out_dir=export_out_dir,
-            slice=args.slice,
+            should_slice=args.slice,
             slice_mode=args.slice_mode,
             vectors=args.vectors,
             cpg_manifests=cpg_manifests,
         )
-    if is_temp_dir:
-        try:
-            shutil.rmtree(src)
-        except Exception:
-            # Ignore cleanup errors
-            pass
+    # We can remove the src but not the cpg_out and cpg_export which might get used
+    # by downstream tools
+    if is_temp_dir and src.startswith(tempfile.gettempdir()):
+        shutil.rmtree(src, ignore_errors=True)
 
 
 if __name__ == "__main__":
     freeze_support()
     main()
```

### Comparing `cpggen-1.1.5/cpggen/executor.py` & `cpggen-1.1.6/cpggen/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,26 +18,26 @@
     find_files,
     find_go_mods,
     find_gradle_files,
     find_java_artifacts,
     find_makefiles,
     find_pom_files,
     find_sbt_files,
-    to_friendly_name,
+    purl_to_friendly_name,
 )
 
 runtimeValues = {}
 svmem = psutil.virtual_memory()
 max_memory = bytes2human(getattr(svmem, "available"), format="%(value).0f%(symbol)s")
-cpu_count = str(psutil.cpu_count())
+CPU_COUNT = str(psutil.cpu_count())
 
 only_bat_ext = ".bat" if sys.platform == "win32" else ""
 bin_ext = ".bat" if sys.platform == "win32" else ".sh"
 exe_ext = ".exe" if sys.platform == "win32" else ""
-use_shell = True if sys.platform == "win32" else False
+USE_SHELL = True if sys.platform == "win32" else False
 
 
 def resource_path(relative_path):
     try:
         base_path = sys._MEIPASS
     except Exception:
         base_path = os.path.dirname(__file__)
@@ -50,19 +50,24 @@
 local_bin_dir = resource_path("local_bin")
 if os.path.exists(local_bin_dir):
     csharp2cpg_bundled = resource_path(
         os.path.join("local_bin", "joern-cli", "csharp2cpg.zip")
     )
     joern_bundled = resource_path(os.path.join("local_bin", "joern-cli.zip"))
     if os.path.exists(csharp2cpg_bundled) and not os.path.exists(
-        os.path.join(local_bin_dir, "bin", "csharp2cpg")
+        os.path.join(local_bin_dir, "joern-cli", "bin", "csharp2cpg")
     ):
         try:
             with zipfile.ZipFile(csharp2cpg_bundled, "r") as zip_ref:
-                zip_ref.extractall(local_bin_dir)
+                zip_ref.extractall(os.path.join(local_bin_dir, "joern-cli"))
+                LOG.debug("Extracted %s", csharp2cpg_bundled)
+                if not os.path.exists(
+                    os.path.join(local_bin_dir, "joern-cli", "bin", "csharp2cpg")
+                ):
+                    LOG.debug("csharp2cpg could not be found after extraction")
         except Exception as e:
             LOG.info(
                 "cpggen was prevented from extracting the csharp2cpg frontend.\nPlease check if your terminal has administrative privileges or if the antivirus is preventing this process.\nAlternatively, use container-based execution."
             )
             LOG.error(e)
     if os.path.exists(joern_bundled) and not os.path.exists(
         os.path.join(local_bin_dir, "joern-cli", "c2cpg.sh")
@@ -75,15 +80,15 @@
                     for filename in files:
                         if not filename.endswith(".jar") and (
                             filename.endswith("%(bin_ext)s")
                             or "2cpg" in filename
                             or "joern-" in filename
                         ):
                             os.chmod(os.path.join(dirname, filename), 0o755)
-                LOG.debug(f"Extracted {joern_bundled}")
+                LOG.debug("Extracted %s", joern_bundled)
                 os.environ["JOERN_HOME"] = os.path.join(local_bin_dir, "joern-cli")
                 os.environ["CPGGEN_BIN_DIR"] = local_bin_dir
                 os.environ["PATH"] += os.sep + os.environ["JOERN_HOME"] + os.sep
         except Exception as e:
             LOG.info(
                 "cpggen was prevented from extracting the joern library.\nPlease check if your terminal has administrative privileges or if the antivirus is preventing this process.\nAlternatively, use container-based execution."
             )
@@ -96,29 +101,26 @@
         )
         if os.path.exists(local_cdxgen_cmd):
             cdxgen_cmd = local_cdxgen_cmd
             # Set the plugins directory as an environment variable
             os.environ["CDXGEN_PLUGINS_DIR"] = local_bin_dir
 
 
-def get(configName, default_value=None):
+def get(config_name, default_value=None):
     """Method to retrieve a config given a name. This method lazy loads configuration
     values and helps with overriding using a local config
-    :param configName: Name of the config
+    :param config_name: Name of the config
     :return Config value
     """
-    try:
-        value = runtimeValues.get(configName)
-        if value is None:
-            value = os.environ.get(configName.replace("-", "_").upper())
-        if value is None:
-            value = default_value
-        return value
-    except Exception:
-        return default_value
+    value = runtimeValues.get(config_name)
+    if value is None:
+        value = os.environ.get(config_name.replace("-", "_").upper())
+    if value is None:
+        value = default_value
+    return value
 
 
 cpg_tools_map = {
     "c": "%(joern_home)sc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "cpp": "%(joern_home)sc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "c-with-deps": "%(joern_home)sc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --with-include-auto-discovery",
     "cpp-with-deps": "%(joern_home)sc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --with-include-auto-discovery",
@@ -230,20 +232,21 @@
     "binary": "ghidra",
     "ruby": "rubysrc",
     "jimple": "java",
 }
 
 
 def qwiet_analysis(app_manifest, src, cwd, env):
+    """Method to submit the cpg to Qwiet.AI"""
     try:
         relative_path = os.path.relpath(cwd, src)
         if relative_path and not relative_path.startswith(".."):
             os.environ["SL_VCS_RELATIVE_PATH"] = relative_path
             env["SL_VCS_RELATIVE_PATH"] = relative_path
-        LOG.info(f"Submitting {app_manifest['app']} for Qwiet.AI analysis")
+        LOG.info("Submitting %s for Qwiet.AI analysis", app_manifest["app"])
         build_args = cpg_tools_map["qwiet"]
         policy = ""
         vcs_correction = ""
         if os.getenv("SHIFTLEFT_POLICY"):
             policy = f"""--policy {os.getenv("SHIFTLEFT_POLICY")} """
         elif os.getenv("ENABLE_BEST_PRACTICES") in ("true", "1"):
             policy = """--policy io.shiftleft/defaultWithDictAndBestPractices """
@@ -254,81 +257,83 @@
             ):
                 vcs_correction = '--vcs-prefix-correction "*=src/main/java" '
             if "scala" in app_manifest.get("tool_lang"):
                 vcs_correction = '--vcs-prefix-correction "*=src/main/scala" '
         build_args = build_args % dict(
             **app_manifest, policy=policy, vcs_correction=vcs_correction
         )
-        LOG.debug(f"Executing {build_args}")
+        LOG.debug("Executing %s", build_args)
         cp = subprocess.run(
             build_args.split(" "),
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             cwd=cwd,
             env=env,
             check=False,
-            shell=use_shell,
+            shell=USE_SHELL,
             encoding="utf-8",
         )
         if cp:
             if cp.stdout:
                 LOG.info(cp.stdout)
             if cp.returncode and cp.stderr:
-                LOG.warn(cp.stderr)
+                LOG.warning(cp.stderr)
             else:
-                LOG.info(f"{app_manifest['app']} uploaded successfully")
-    except Exception as e:
+                LOG.info("%s uploaded successfully", app_manifest["app"])
+    except subprocess.SubprocessError as e:
         LOG.error(e)
 
 
 def dot_convert(export_out_dir, env):
     if check_command("dot"):
         dot_files = find_files(export_out_dir, ".dot", False, False)
         if len(dot_files) > 5:
             LOG.info(
-                f"{len(dot_files)} dot files generated after export. Skipping dot2png conversion ..."
+                "%d dot files generated after export. Skipping dot2png conversion ...",
+                len(dot_files),
             )
             return
         for df in dot_files:
             convert_cmd_with_args = cpg_tools_map["dot2png"] % dict(
                 dot_file=df, png_out=df.replace(".dot", ".png")
             )
             try:
                 subprocess.run(
                     convert_cmd_with_args.split(" "),
                     stdout=subprocess.PIPE,
                     stderr=subprocess.PIPE,
                     cwd=export_out_dir,
                     env=env,
                     check=False,
-                    shell=use_shell,
+                    shell=USE_SHELL,
                     encoding="utf-8",
                 )
             except Exception as e:
                 LOG.debug(e)
     else:
         LOG.debug(
             "Install graphviz package and ensure the command `dot` is available in the PATH to convert to png automatically"
         )
 
 
 def do_x_build(src, env, build_artefacts, tool_lang):
+    """Method to guess and build applications"""
     tool_lang = tool_lang.split("-")[0]
     build_crashes = {}
     for k, v in build_artefacts.items():
         failed_modules = 0
         crashed_modules = 0
         build_sets = build_tools_map.get(tool_lang)
         if isinstance(build_sets, dict):
             build_args = build_tools_map[tool_lang][k]
         else:
             build_args = build_sets
         if len(v) > 5:
             LOG.debug(
-                f"This project has {len(v)} modules. Build might take a while ..."
+                "This project has %d modules. Build might take a while ...", len(v)
             )
         for afile in v:
             base_dir = os.path.dirname(afile)
             build_args_str = " ".join(build_args)
             if "%(" in build_args_str:
                 gradle_cmd = "gradle"
                 maven_cmd = "mvn"
@@ -346,46 +351,47 @@
                     except Exception:
                         # Ignore errors
                         pass
                 build_args_str = build_args_str % dict(
                     gradle_cmd=gradle_cmd, maven_cmd=maven_cmd
                 )
             try:
-                LOG.debug(f"Executing build command: {build_args_str} in {base_dir}")
+                LOG.debug("Executing build command: %s in %s", build_args_str, base_dir)
                 cp = subprocess.run(
                     build_args_str.split(" "),
                     stdout=subprocess.PIPE,
                     stderr=subprocess.PIPE,
                     cwd=base_dir,
                     env=env,
                     check=False,
-                    shell=use_shell,
+                    shell=USE_SHELL,
                     encoding="utf-8",
                 )
                 if cp:
                     # These languages always need troubleshooting
                     if tool_lang in ("csharp", "dotnet", "go"):
                         if cp.stderr:
                             LOG.info(cp.stderr)
                         if cp.stdout:
                             LOG.info(cp.stdout)
                     elif LOG.isEnabledFor(DEBUG) and cp.returncode and cp.stderr:
                         LOG.debug(cp.stderr)
                     failed_modules = failed_modules + 1
-            except Exception as e:
-                LOG.info(e)
+            except subprocess.SubprocessError:
+                LOG.info(exc_info=True)
                 crashed_modules = crashed_modules + 1
         build_crashes[k] = {
             "failed_modules": failed_modules,
             "crashed_modules": crashed_modules,
         }
     return build_crashes
 
 
 def do_jar_build(tool_lang, src, env):
+    """Method to build java apps"""
     build_artefacts = {
         "gradle": find_gradle_files(src),
         "maven": find_pom_files(src),
         "sbt": find_sbt_files(src),
     }
     settings_xmls = find_files(src, "settings.xml", False, False)
     if settings_xmls:
@@ -396,23 +402,25 @@
             LOG.info(
                 "Set the environment variable AT_DEBUG_MODE to debug and look for any build errors"
             )
     return do_x_build(src, env, build_artefacts, tool_lang)
 
 
 def do_go_build(src, env):
+    """Method to build go apps"""
     build_artefacts = {
         "mage": find_files(src, "magefile.go", False, False),
         "go": find_go_mods(src),
         "make": find_makefiles(src),
     }
     return do_x_build(src, env, build_artefacts, "go")
 
 
 def do_build(tool_lang, src, cwd, env):
+    """Method to build various apps"""
     if tool_lang in ("csharp",):
         if os.path.exists(os.path.join(src, "global.json")):
             LOG.debug(
                 "global.json is found in the root directory. Ensure the correct version of dotnet sdk is installed.\nAlternatively, set the rollForward property to latestMajor to use the bundled .Net 7 SDK from the cpggen container image."
             )
         return do_x_build(src, env, {"csharp": find_csharp_artifacts(src)}, "csharp")
     elif (
@@ -422,30 +430,36 @@
     ):
         return do_jar_build(tool_lang, src, env)
     elif tool_lang == "go":
         return do_go_build(src, env)
 
 
 def troubleshoot_app(lang_build_crashes, tool_lang):
+    """Not implemented yet"""
     pass
 
 
 def exec_tool(
     tool_lang,
     src,
     cpg_out_dir,
     cwd=None,
     joern_home=None,
     use_container=False,
     use_parse=False,
     auto_build=False,
-    extra_args={},
-    env=os.environ.copy(),
+    extra_args=None,
+    env=None,
     stdout=subprocess.DEVNULL,
 ):
+    """Method to execute tools to generate cpg or perform exports"""
+    if env is None:
+        env = os.environ.copy()
+    if extra_args is None:
+        extra_args = {}
     with Progress(
         console=console,
         transient=True,
         redirect_stderr=False,
         redirect_stdout=False,
         refresh_per_second=1,
     ) as progress:
@@ -495,32 +509,38 @@
             cmd_with_args = cpg_tools_map.get(cpg_cmd_lang)
             if not cmd_with_args:
                 return
             # Perform build first
             if build_tools_map.get(tool_lang):
                 if os.getenv("CI"):
                     LOG.debug(
-                        f"Automatically building {src} for {tool_lang}. To speed up this step, cache the build dependencies using the CI cache settings."
+                        "Automatically building %s for %s. To speed up this step, cache the build dependencies using the CI cache settings.",
+                        src,
+                        tool_lang,
                     )
                 elif use_container:
                     LOG.debug(
-                        f"Attempting to build {src} for {tool_lang} using the bundled build tools from the container image."
+                        "Attempting to build %s for %s using the bundled build tools from the container image.",
+                        src,
+                        tool_lang,
                     )
                 else:
                     LOG.debug(
-                        f"Attempting to build {src} for {tool_lang} using the locally available build tools.\nFor better results, please ensure the correct version of these tools are installed for your application.\nAlternatively, use container image based execution."
+                        "Attempting to build %s for %s using the locally available build tools.\nFor better results, please ensure the correct version of these tools are installed for your application.\nAlternatively, use container image based execution.",
+                        src,
+                        tool_lang,
                     )
                 lang_build_crashes[tool_lang] = do_build(tool_lang, src, cwd, env)
             uber_jar = ""
             csharp_artifacts = ""
             # For languages like scala, jsp or jar we need to create a uber jar containing all jar, war files from the source directory
             if "uber_jar" in cmd_with_args:
                 stdout = subprocess.PIPE
                 java_artifacts = find_java_artifacts(src)
-                if len(java_artifacts):
+                if len(java_artifacts) > 0:
                     uber_jar = java_artifacts[0]
             if "csharp_artifacts" in cmd_with_args:
                 stdout = subprocess.PIPE
                 csharp_artifacts = find_csharp_artifacts(src)
                 if len(csharp_artifacts):
                     csharp_artifacts = csharp_artifacts[0]
             modules = [src]
@@ -567,15 +587,15 @@
                         else f"{cpg_out}.bom.xml"
                     )
                     manifest_out = (
                         cpg_out.replace(".bin.zip", ".manifest.json")
                         if cpg_out.endswith(".bin.zip")
                         else f"{cpg_out}.manifest.json"
                     )
-                    LOG.debug(f"CPG file for {tool_lang} is {cpg_out}")
+                    LOG.debug("CPG file for %s is %s", tool_lang, cpg_out)
                 if not slice_out:
                     slice_out = cpg_out.replace(".bin.zip", ".slices")
                     slice_out = slice_out + (
                         ".json" if extra_args.get("slice_mode") == "Usages" else ".cpg"
                     )
                     extra_args["slice_out"] = slice_out
                 cmd_with_args = cmd_with_args % dict(
@@ -625,24 +645,26 @@
                     **extra_args,
                 )
                 cmd_list_with_args = cmd_with_args.split(" ")
                 sbom_cmd_list_with_args = sbom_cmd_with_args.split(" ")
                 lang_cmd = cmd_list_with_args[0]
                 if not check_command(lang_cmd) and not os.path.exists(lang_cmd):
                     if not use_container:
-                        LOG.warn(
-                            f"{lang_cmd} is not found. Try running cpggen with --use-container argument."
+                        LOG.warning(
+                            "%s is not found. Try running cpggen with --use-container argument.",
+                            lang_cmd,
                         )
                     elif not use_parse:
-                        LOG.warn(
+                        LOG.warning(
                             "Try running cpggen with --use-parse argument to use joern-parse command instead of language frontends."
                         )
                     else:
-                        LOG.warn(
-                            f"{lang_cmd} is not found. Ensure the PATH variable in your container image is set to the bin directory of Joern."
+                        LOG.warning(
+                            "%s is not found. Ensure the PATH variable in your container image is set to the bin directory of Joern.",
+                            lang_cmd,
                         )
                     return
                 # Is this an Export or Slice task?
                 if tool_lang in ("export", "slice", "vectors"):
                     try:
                         progress.update(
                             task,
@@ -653,76 +675,96 @@
                         cp = subprocess.run(
                             cmd_list_with_args,
                             stdout=stdout,
                             stderr=stderr,
                             cwd=cwd,
                             env=env,
                             check=False,
-                            shell=use_shell,
+                            shell=USE_SHELL,
                             encoding="utf-8",
                         )
                         # Bug. joern-vectors doesn't create json
                         if tool_lang == "vectors" and cp and cp.stdout:
                             os.makedirs(cpg_out_dir, exist_ok=True)
                             with open(
-                                os.path.join(cpg_out_dir, "vectors.json"), mode="w"
+                                os.path.join(cpg_out_dir, "vectors.json"),
+                                mode="w",
+                                encoding="utf-8",
                             ) as fp:
                                 fp.write(cp.stdout)
                         if cp and cp.returncode and cp.stderr:
-                            LOG.warn(
-                                f"{tool_lang.capitalize()} operation has failed for {src}"
+                            LOG.warning(
+                                "%s operation has failed for %s",
+                                tool_lang.capitalize(),
+                                src,
                             )
                             if not os.getenv("AT_DEBUG_MODE"):
                                 LOG.info(
                                     "Set the environment variable AT_DEBUG_MODE to debug to see the debug logs"
                                 )
                             if cp.stdout:
                                 LOG.info(cp.stdout)
                             if cp.stderr:
                                 LOG.info("------------------------------")
                                 LOG.info(cp.stderr)
                                 LOG.info("------------------------------")
                                 LOG.info(
-                                    f"Command used {' '.join(cmd_list_with_args)}\nPlease report the above error to https://github.com/joernio/joern/issues"
+                                    "Command used %s\nPlease report the above error to https://github.com/joernio/joern/issues",
+                                    " ".join(cmd_list_with_args),
                                 )
                         else:
                             check_dir = (
                                 cpg_out_dir
-                                if tool_lang in ("export")
+                                if tool_lang == "export"
                                 else (
                                     os.path.join(cpg_out_dir, "vectors.json")
                                     if tool_lang == "vectors"
                                     else slice_out
                                 )
                             )
                             if os.path.exists(check_dir):
                                 if tool_lang == "vectors":
                                     LOG.info(
-                                        f"CPG {src} successfully vectorized to {check_dir}"
+                                        "CPG %s successfully vectorized to %s",
+                                        src,
+                                        check_dir,
                                     )
                                 else:
                                     LOG.info(
-                                        f"CPG {src} successfully {tool_lang + ('d' if tool_lang.endswith('e') else 'ed')} to {check_dir}"
+                                        "CPG %s successfully %s to {check_dir}",
+                                        src,
+                                        tool_lang
+                                        + ("d" if tool_lang.endswith("e") else "ed"),
                                     )
                                 # Convert dot files to png
                                 if tool_lang == "export":
                                     progress.update(
                                         task,
                                         description="Convert exported graph to png",
                                         completed=95,
                                         total=100,
                                     )
                                     dot_convert(cpg_out_dir, env)
                             else:
-                                LOG.warn(
-                                    f"Unable to {tool_lang} {src} to {check_dir}. Try running joern-{tool_lang} manually using the command {' '.join(cmd_list_with_args)}"
+                                LOG.warning(
+                                    "Unable to %s %s to %s. Try running joern-%s manually using the command %s",
+                                    tool_lang,
+                                    src,
+                                    check_dir,
+                                    tool_lang,
+                                    " ".join(cmd_list_with_args),
                                 )
                     except Exception as e:
-                        LOG.warn(f"Unable to {tool_lang} {src} to {cpg_out_dir}")
-                        LOG.error(e)
+                        LOG.warning(
+                            "Unable to %s %s to %s",
+                            tool_lang,
+                            src,
+                            cpg_out_dir,
+                            exc_info=True,
+                        )
                     progress.update(task, completed=100, total=100)
                     continue
                 LOG.debug(
                     '⚡︎ Generating CPG for the {} app "{}" - "{}"'.format(
                         tool_lang,
                         os.path.basename(amodule),
                         " ".join(cmd_list_with_args),
@@ -739,32 +781,32 @@
                             description="Generating SBoM using cdxgen",
                             completed=10,
                             total=100,
                         )
                         # Enable debug for sbom tool
                         if LOG.isEnabledFor(DEBUG):
                             env["SCAN_DEBUG_MODE"] = "debug"
-                        LOG.debug(f"Executing {' '.join(sbom_cmd_list_with_args)}")
+                        LOG.debug("Executing %s", " ".join(sbom_cmd_list_with_args))
 
                         cp = subprocess.run(
                             sbom_cmd_list_with_args,
                             stdout=stdout,
                             stderr=stderr,
                             cwd=cwd,
                             env=env,
                             check=False,
-                            shell=use_shell,
+                            shell=USE_SHELL,
                             encoding="utf-8",
                         )
                         if cp and LOG.isEnabledFor(DEBUG):
                             if cp.stdout:
                                 LOG.debug(cp.stdout)
                             if cp.stderr:
                                 LOG.debug(cp.stderr)
-                    except Exception:
+                    except subprocess.SubprocessError:
                         # Ignore SBoM errors
                         pass
                 progress.update(
                     task,
                     description=f"Generating {tool_lang_simple} CPG",
                     completed=20,
                     total=100,
@@ -772,41 +814,46 @@
                 cp = subprocess.run(
                     cmd_list_with_args,
                     stdout=stdout,
                     stderr=stderr,
                     cwd=cwd,
                     env=env,
                     check=False,
-                    shell=use_shell,
+                    shell=USE_SHELL,
                     encoding="utf-8",
                 )
                 if cp and stdout == subprocess.PIPE:
                     for line in cp.stdout:
                         progress.update(task, completed=5)
                 if cp and cp.returncode:
                     if cp.stdout:
                         LOG.info(cp.stdout)
                     if cp.stderr:
                         LOG.info(cp.stderr)
                 if os.path.exists(cpg_out):
                     # go2cpg seems to produce a cpg without read permissions
                     try:
                         os.chmod(cpg_out, 0o644)
-                    except Exception:
+                    except OSError:
                         # Ignore errors
                         pass
                     if os.getenv("CI"):
                         LOG.info(
-                            f"""CPG {cpg_out} generated successfully for {tool_lang}."""
+                            """CPG %s generated successfully for %s.""",
+                            cpg_out,
+                            tool_lang,
                         )
                     else:
                         LOG.info(
-                            f"""CPG for {tool_lang} is {cpg_out}. You can import this in joern using importCpg("{cpg_out}")"""
+                            """CPG for %s is %s. You can import this in joern using importCpg("%s")""",
+                            tool_lang,
+                            cpg_out,
+                            cpg_out,
                         )
-                    with open(manifest_out, mode="w") as mfp:
+                    with open(manifest_out, mode="w", encoding="utf-8") as mfp:
                         # In case of github action, we need to convert this to relative path
                         if os.getenv("GITHUB_PATH"):
                             cpg_out = cpg_out.replace("/github/workspace/", "")
                             sbom_out = sbom_out.replace("/github/workspace/", "")
                             amodule = amodule.replace("/github/workspace/", "")
                         language = tool_lang_simple
                         # Override the language for jvm
@@ -822,15 +869,15 @@
                             ]
                         full_app_name = extra_args.get(
                             "full_app_name", f"{app_base_name}-{language}"
                         )
                         if extra_args.get("url") and extra_args.get("url").startswith(
                             "pkg:"
                         ):
-                            full_app_name = to_friendly_name(extra_args.get("url"))
+                            full_app_name = purl_to_friendly_name(extra_args.get("url"))
                         app_manifest = {
                             "src": amodule,
                             "group": app_base_name,
                             "app": full_app_name,
                             "cpg": cpg_out,
                             "sbom": sbom_out,
                             "slice_out": slice_out,
@@ -846,15 +893,15 @@
                                 description="Uploading to Qwiet AI for analysis",
                                 completed=90,
                                 total=100,
                             )
                             qwiet_analysis(app_manifest, src, cwd, env)
                         json.dump(app_manifest, mfp)
                 else:
-                    LOG.info(f"CPG {cpg_out} was not generated for {tool_lang}")
+                    LOG.info("CPG %s was not generated for %s", cpg_out, tool_lang)
                     if not os.getenv("AT_DEBUG_MODE"):
                         LOG.info(
                             "Set the environment variable AT_DEBUG_MODE to debug to see the debug logs"
                         )
                     if cp.stdout:
                         LOG.info(cp.stdout)
                     if cp.stderr:
@@ -862,9 +909,9 @@
                     troubleshoot_app(lang_build_crashes, tool_lang)
                 progress.update(task, completed=100, total=100)
         except Exception as e:
             if not os.getenv("AT_DEBUG_MODE"):
                 LOG.info(
                     "Set the environment variable AT_DEBUG_MODE to debug to see the debug logs"
                 )
-            LOG.error(e)
+            LOG.warning(e)
     return app_manifest_list
```

### Comparing `cpggen-1.1.5/cpggen/logger.py` & `cpggen-1.1.6/cpggen/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 logging.basicConfig(
     level=logging.INFO,
     format="%(message)s",
     datefmt="[%X]",
     handlers=[
         RichHandler(
-            console=console, markup=True, show_path=False, enable_link_path=False
+            console=console, markup=False, show_path=False, enable_link_path=False
         )
     ],
 )
 LOG = logging.getLogger(__name__)
 USE_DEBUG = False
 
 # Set logging level
```

### Comparing `cpggen-1.1.5/cpggen/utils.py` & `cpggen-1.1.6/cpggen/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,36 @@
+import json
 import os
 import re
 import shutil
 import tempfile
+import tarfile
 import zipfile
 from pathlib import Path
 from sys import platform
 
 import httpx
 import rich.progress
 from packageurl import PackageURL
 from packageurl.contrib import purl2url
 from rich.progress import Progress
 
+from cpggen.source import ghsa
+
 GIT_AVAILABLE = False
 try:
     import git
 
     GIT_AVAILABLE = True
-except Exception:
+except ImportError:
     pass
 
+MAVEN_CENTRAL_URL = "https://repo1.maven.org/maven2/"
+ANDROID_MAVEN = "https://maven.google.com/"
+
 # Default ignore list
 ignore_directories = [
     ".git",
     ".svn",
     ".mvn",
     ".idea",
     "backup",
@@ -159,14 +166,15 @@
 
 def find_files(src, src_ext_name, use_start=False, quick=False):
     """
     Method to find files with given extension
     :param src: Source directory
     :param src_ext_name: Extension
     :param use_start: Boolean to check for file prefix
+    :param quick: Quick search mode to return after a single hit
     :return: List of files with full path
     """
     result = []
     for root, dirs, files in os.walk(src):
         filter_ignored_dirs(dirs)
         if not is_ignored_dir(src, root):
             for file in files:
@@ -180,15 +188,15 @@
                     return result
     return result
 
 
 def find_java_artifacts(search_dir):
     """
     Method to find java artifacts in the given directory
-    :param src: Directory to search
+    :param search_dir: Directory to search
     :return: List of war or ear or jar files
     """
     jlist = []
     with tempfile.NamedTemporaryFile(
         mode="w", suffix=".jar", encoding="utf-8", delete=False
     ) as zfile:
         with zipfile.ZipFile(zfile.name, "w") as zf:
@@ -207,16 +215,16 @@
                             zf.write(os.path.join(dirname, filename))
     return jlist if len(jlist) == 1 else [os.path.abspath(zfile.name)]
 
 
 def find_csharp_artifacts(search_dir):
     """
     Method to find .Net solution and csproj files in the given directory
-    :param src: Directory to search
-    :return: List of war or ear or jar files
+    :param search_dir: Directory to search
+    :return: List of .sln or .csharp files
     """
     result = [p.as_posix() for p in Path(search_dir).absolute().rglob("*.sln")]
     if not result:
         result = [p.as_posix() for p in Path(search_dir).absolute().rglob("*.csproj")]
     return result
 
 
@@ -241,19 +249,16 @@
 
 
 def check_command(cmd):
     """
     Method to check if command is available
     :return True if command is available in PATH. False otherwise
     """
-    try:
-        cpath = shutil.which(cmd, mode=os.F_OK | os.X_OK)
-        return cpath is not None
-    except Exception:
-        return False
+    cpath = shutil.which(cmd, mode=os.F_OK | os.X_OK)
+    return cpath is not None
 
 
 def is_binary_string(content):
     """
     Method to check if the given content is a binary string
     """
     textchars = bytearray({7, 8, 9, 10, 12, 13, 27} | set(range(0x20, 0x100)) - {0x7F})
@@ -264,32 +269,32 @@
     """Detect if the source is a binary file
     :param src: Source path
     :return True if binary file. False otherwise.
     """
     if os.path.isfile(src):
         try:
             return is_binary_string(open(src, "rb").read(1024))
-        except Exception:
+        except OSError:
             return False
     return False
 
 
 def find_exe_files(src):
     """
     Method to find files with given extenstion
     """
     result = []
     for root, dirs, files in os.walk(src):
         filter_ignored_dirs(dirs)
         for file in files:
             if is_ignored_file(file):
                 continue
-            fullPath = os.path.join(root, file)
-            if is_exe(fullPath):
-                result.append(fullPath)
+            full_path = os.path.join(root, file)
+            if is_exe(full_path):
+                result.append(full_path)
     return result
 
 
 def bomstrip(manifest):
     """
     Function to delete UTF-8 BOM character in "string"
     """
@@ -423,71 +428,162 @@
             or find_files(src_dir, ".jimple", False, True)
         ):
             project_types.append("jimple")
     return project_types
 
 
 def clone_repo(repo_url, clone_dir, depth=1):
+    """Method to clone a git repo"""
     if not GIT_AVAILABLE:
         return None
     git.Repo.clone_from(repo_url, clone_dir, depth=depth)
     return clone_dir
 
 
 def build_maven_download_url(purl):
     """
     Return a maven download URL from the `purl` string.
     """
-    MAVEN_CENTRAL_URL = "https://repo1.maven.org/maven2/"
-    ANDROID_MAVEN = "https://maven.google.com/"
     url_prefix = MAVEN_CENTRAL_URL
 
     purl_data = PackageURL.from_string(purl)
     group = purl_data.namespace.replace(".", "/")
     name = purl_data.name
     version = purl_data.version
 
     if "android" in group:
         url_prefix = ANDROID_MAVEN
 
     if name and version:
         return f"{url_prefix}{group}/{name}/{version}/{name}-{version}.jar"
 
 
+def build_pypi_download_url(purl):
+    """
+    Return a PyPI download URL from the `purl` string.
+    """
+    url_prefix = "https://pypi.io/packages/source/"
+    purl_data = PackageURL.from_string(purl)
+    name = purl_data.name
+    version = purl_data.version
+    if name and version:
+        return f"{url_prefix}{name[0]}/{name}/{name}-{version}.tar.gz"
+
+
+def build_golang_download_url(purl):
+    """
+    Return a golang download URL from the `purl` string.
+    """
+    purl_data = PackageURL.from_string(purl)
+    namespace = purl_data.namespace
+    name = purl_data.name
+    version = purl_data.version
+    qualifiers = purl_data.qualifiers
+    download_url = qualifiers.get("download_url")
+    if download_url:
+        return download_url
+    if not (namespace and name and version):
+        return
+    version_prefix = qualifiers.get("version_prefix", "v")
+    version = f"{version_prefix}{version}"
+    return f"https://{namespace}/{name}/archive/refs/tags/{version}.zip"
+
+
+def build_ghsa_download_url(cve_or_ghsa):
+    """Method to get download urls for the packages belonging to the CVE"""
+    return ghsa.get_download_urls(cve_or_ghsa=cve_or_ghsa)
+
+
 def get_download_url(purl_str):
+    """Build download urls from a purl or CVE or GHSA id"""
+    if purl_str.startswith("GHSA") or purl_str.startswith("CVE"):
+        return build_ghsa_download_url(purl_str)
     if purl_str.startswith("pkg:maven"):
         return build_maven_download_url(purl_str)
+    if purl_str.startswith("pkg:pypi"):
+        return build_pypi_download_url(purl_str)
+    if purl_str.startswith("pkg:golang"):
+        return build_golang_download_url(purl_str)
     return purl2url.get_download_url(purl_str)
 
 
-def download_package(purl_str, download_dir):
+def unzip_unsafe(zf, to_dir):
+    """Method to unzip the file in an unsafe manne"""
+    with zipfile.ZipFile(zf, "r") as zip_ref:
+        zip_ref.extractall(to_dir)
+    shutil.rmtree(zf, ignore_errors=True)
+
+
+def untar_unsafe(tf, to_dir):
+    """Method to untar .tar or .tar.gz files in an unsafe manner"""
+    if tf.endswith("tar.gz") or tf.endswith(".tgz"):
+        tar = tarfile.open(tf, "r:gz")
+        tar.extractall(to_dir)
+        tar.close()
+    elif tf.endswith(".tar"):
+        tar = tarfile.open(tf, "r:")
+        tar.extractall(to_dir)
+        tar.close()
+    shutil.rmtree(tf, ignore_errors=True)
+
+
+def download_package_unsafe(purl_str, download_dir, expand_archive=True):
+    """Method to download the package from the given purl or CVE id"""
     if not purl_str:
         return
     durl = get_download_url(purl_str)
     if not durl:
         return
-    with open(
-        os.path.join(download_dir, os.path.basename(durl)), mode="wb"
-    ) as download_file:
-        with httpx.stream("GET", durl) as response:
-            total = int(response.headers["Content-Length"])
-            with Progress(
-                "[progress.percentage]{task.percentage:>3.0f}%",
-                rich.progress.BarColumn(bar_width=None),
-                rich.progress.DownloadColumn(),
-                rich.progress.TransferSpeedColumn(),
-            ) as progress:
-                download_task = progress.add_task("Download", total=total)
-                for chunk in response.iter_bytes():
-                    download_file.write(chunk)
-                    progress.update(
-                        download_task, completed=response.num_bytes_downloaded
-                    )
-                return download_file.name
+    if isinstance(durl, str):
+        durl = [durl]
+    for aurl in durl:
+        if isinstance(aurl, dict) and aurl.get("purl"):
+            aurl = get_download_url(aurl.get("purl"))
+        with open(
+            os.path.join(download_dir, os.path.basename(aurl)), mode="wb"
+        ) as download_file:
+            with httpx.stream("GET", aurl, follow_redirects=True) as response:
+                total = int(response.headers["Content-Length"])
+                with Progress(
+                    "[progress.percentage]{task.percentage:>3.0f}%",
+                    rich.progress.BarColumn(bar_width=None),
+                    rich.progress.DownloadColumn(),
+                    rich.progress.TransferSpeedColumn(),
+                ) as progress:
+                    download_task = progress.add_task("Download", total=total)
+                    for chunk in response.iter_bytes():
+                        download_file.write(chunk)
+                        progress.update(
+                            download_task, completed=response.num_bytes_downloaded
+                        )
+            download_file.close()
+            if expand_archive:
+                if download_file.name.endswith(".zip"):
+                    unzip_unsafe(download_file.name, download_dir)
+                elif (
+                    download_file.name.endswith(".tar")
+                    or download_file.name.endswith(".tar.gz")
+                    or download_file.name.endswith(".tgz")
+                ):
+                    untar_unsafe(download_file.name, download_dir)
+    return download_dir
 
 
-def to_friendly_name(purl_str):
+def purl_to_friendly_name(purl_str):
     """Convert package url to a friendly name"""
     purl_data = PackageURL.from_string(purl_str)
     name = purl_data.name
     version = purl_data.version
     return f"{name}-{version}"
+
+
+def collect_cpg_manifests(cpg_out_dir):
+    """Utility method to collect all the CPG manifests created in a directory"""
+    cpg_manifests = []
+    if os.path.isfile(cpg_out_dir):
+        cpg_out_dir = os.path.dirname(cpg_out_dir)
+    mfiles = find_files(cpg_out_dir, ".manifest.json") if cpg_out_dir else []
+    for amanifest in mfiles:
+        with open(amanifest, encoding="utf-8") as mfp:
+            manifest_obj = json.load(mfp)
+            cpg_manifests.append(manifest_obj)
+    return cpg_manifests
```

### Comparing `cpggen-1.1.5/pyproject.toml` & `cpggen-1.1.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cpggen"
-version = "1.1.5"
+version = "1.1.6"
 description = "Generate CPG for multiple languages for use with joern"
 authors = ["Team AppThreat <cloud@appthreat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "cpggen"}]
 homepage = "https://github.com/AppThreat/cpggen"
 repository = "https://github.com/AppThreat/cpggen"
@@ -37,11 +37,13 @@
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 black = "^23.3.0"
 flake8 = "^6.0.0"
 pytest-cov = "^4.0.0"
 pyinstaller = "^5.10.1"
+bandit = "^1.7.5"
+pylint = "^2.17.4"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cpggen-1.1.5/PKG-INFO` & `cpggen-1.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpggen
-Version: 1.1.5
+Version: 1.1.6
 Summary: Generate CPG for multiple languages for use with joern
 Home-page: https://github.com/AppThreat/cpggen
 License: Apache-2.0
 Keywords: joern,code analysis,static analysis,cpg,code property graph
 Author: Team AppThreat
 Author-email: cloud@appthreat.com
 Requires-Python: >=3.8.1,<3.12
@@ -13,17 +13,15 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Dist: gitpython (>=3.1.31,<4.0.0)
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: packageurl-python (>=0.11.1,<0.12.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: quart (>=0.18.4,<0.19.0)
@@ -40,14 +38,18 @@
 ██║     ██╔═══╝ ██║   ██║
 ╚██████╗██║     ╚██████╔╝
  ╚═════╝╚═╝      ╚═════╝
 ```
 
 CPG Generator is a python cli tool to generate [Code Property Graph](https://cpg.joern.io) for multiple languages. The generated CPG can be directly imported to [Joern](https://joern.io) or uploaded to [Qwiet.AI](https://docs.shiftleft.io/home) for analysis.
 
+[![release](https://github.com/appthreat/cpggen/actions/workflows/pythonpublish.yml/badge.svg)](https://github.com/appthreat/cpggen/actions/workflows/pythonpublish.yml)
+[![Downloads](https://static.pepy.tech/badge/cpggen)](https://pepy.tech/project/cpggen)
+[![Discord](https://img.shields.io/badge/-Discord-lime?style=for-the-badge&logo=discord&logoColor=white&color=black)](https://discord.gg/tmmtjCEHNV)
+
 ## Pre-requisites
 
 - JDK 11 or above
 - Python 3.10
 - Docker or podman (Windows, Linux or Mac) or
 - Joern [natively installed](https://docs.joern.io/installation) (Linux only)
 
@@ -60,23 +62,23 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
 - Joern with all the CPG frontends
 - cpggen with Python 3.10
 - cdxgen with Node.js 18 - Generates SBoM
 
 ```bash
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.1.5/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/latest/download/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v1.1.5/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/latest/download/cpggen.exe
 .\cpggen.exe --help
 ```
 
 NOTE: On Windows, antivirus and antimalware could prevent this single executable from functioning properly. Depending on the system, administrative privileges might also be required. Use container-based execution as a fallback.
 
 ### OCI Artifacts via ORAS cli
 
@@ -160,24 +162,31 @@
 
 To specify input and output directory.
 
 ```
 cpggen -i <src directory> -o <CPG directory or file name>
 ```
 
-You can even pass a git or a package url as source
+You can even pass a git or a package url or CVE id as source
 
 ```
 cpggen -i https://github.com/HooliCorp/vulnerable-aws-koa-app -o /tmp/cpg
 ```
 
 ```
 cpggen -i "pkg:maven/org.apache.commons/commons-io@1.3.2" -o /tmp/cpg
 ```
 
+```
+export GITHUB_TOKEN=<token with read:packages scope>
+cpggen -i CVE-2023-32681 -o /tmp/cpg
+
+cpggen -i GHSA-j8r2-6x86-q33q -o /tmp/cpg
+```
+
 To specify language type.
 
 ```
 cpggen -i <src directory> -o <CPG directory or file name> -l java
 
 # Comma separated values are accepted for multiple languages
 cpggen -i <src directory> -o <CPG directory or file name> -l java,js,python
@@ -281,15 +290,15 @@
 usage: cpggen [-h] [-i SRC] [-o CPG_OUT_DIR] [-l LANGUAGE] [--use-container] [--build] [--joern-home JOERN_HOME] [--server] [--server-host SERVER_HOST] [--server-port SERVER_PORT] [--export]
               [--export-repr {ast,cfg,cdg,ddg,pdg,cpg,cpg14,all}] [--export-format {neo4jcsv,graphml,graphson,dot}] [--export-out-dir EXPORT_OUT_DIR] [--verbose] [--skip-sbom] [--slice] [--slice-mode {Usages,DataFlow}] [--use-parse]
 
 CPG Generator
 
 optional arguments:
   -h, --help            show this help message and exit
-  -i SRC, --src SRC     Source directory or url
+  -i SRC, --src SRC     Source directory or url or CVE or GHSA id
   -o CPG_OUT_DIR, --out-dir CPG_OUT_DIR
                         CPG output directory
   -l LANGUAGE, --lang LANGUAGE
                         Optional. CPG language frontend to use. Auto-detects by default.
   --use-container       Use cpggen docker image
   --build               Attempt to build the project automatically
   --joern-home JOERN_HOME
@@ -332,14 +341,15 @@
 | CPG_SLICE               | Set to true to slice CPG                                                   |
 | CPG_SLICE_MODE          | Slice mode. Default Usages                                                 |
 | CPG_VECTORS             | Set to true to generate vector representations of code from CPG            |
 | SHIFTLEFT_ACCESS_TOKEN  | Set to automatically submit the CPG for analysis by Qwiet AI               |
 | CDXGEN_ARGS             | Extra arguments to pass to cdxgen                                          |
 | ENABLE_SBOM             | Enable SBoM generation using cdxgen                                        |
 | JIMPLE_ANDROID_JAR      | Path to android.jar for use with jimple for .apk or .dex to CPG conversion |
+| GITHUB_TOKEN            | Token with read:packages scope to analyze CVE or GitHub Advisory           |
 
 ## GitHub actions
 
 Use the marketplace [action](https://github.com/marketplace/actions/cpggen) to generate CPGs using GitHub actions. Optionally, the upload the generated CPGs as build artifacts use the below step.
 
 ```
 - name: Upload cpg
```

