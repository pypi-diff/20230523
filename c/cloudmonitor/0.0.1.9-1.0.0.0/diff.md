# Comparing `tmp/cloudmonitor-0.0.1.9.tar.gz` & `tmp/cloudmonitor-1.0.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cloudmonitor-0.0.1.9.tar", last modified: Tue Apr 25 05:53:24 2023, max compression
+gzip compressed data, was "cloudmonitor-1.0.0.0.tar", last modified: Tue May 23 15:38:30 2023, max compression
```

## Comparing `cloudmonitor-0.0.1.9.tar` & `cloudmonitor-1.0.0.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-25 05:53:24.000000 cloudmonitor-0.0.1.9/
-drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-25 05:53:24.000000 cloudmonitor-0.0.1.9/cloudmonitor.egg-info/
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       86 2023-04-25 05:53:24.000000 cloudmonitor-0.0.1.9/cloudmonitor.egg-info/entry_points.txt
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     1112 2023-04-25 05:53:24.000000 cloudmonitor-0.0.1.9/cloudmonitor.egg-info/PKG-INFO
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       41 2023-04-25 05:53:24.000000 cloudmonitor-0.0.1.9/cloudmonitor.egg-info/requires.txt
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)        1 2023-04-25 05:53:24.000000 cloudmonitor-0.0.1.9/cloudmonitor.egg-info/dependency_links.txt
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)      525 2023-04-25 05:53:24.000000 cloudmonitor-0.0.1.9/cloudmonitor.egg-info/SOURCES.txt
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       13 2023-04-25 05:53:24.000000 cloudmonitor-0.0.1.9/cloudmonitor.egg-info/top_level.txt
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       37 2023-04-25 05:53:10.000000 cloudmonitor-0.0.1.9/MANIFEST.in
-drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-25 05:53:24.000000 cloudmonitor-0.0.1.9/cloudmonitor/
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       49 2023-04-25 05:48:46.000000 cloudmonitor-0.0.1.9/cloudmonitor/__init__.py
-drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-25 05:53:24.000000 cloudmonitor-0.0.1.9/cloudmonitor/ssh/
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       22 2023-04-23 13:11:47.000000 cloudmonitor-0.0.1.9/cloudmonitor/ssh/__init__.py
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     1135 2023-04-23 14:10:51.000000 cloudmonitor-0.0.1.9/cloudmonitor/ssh/client.py
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     2786 2023-04-25 05:38:08.000000 cloudmonitor-0.0.1.9/cloudmonitor/config.py
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     2139 2023-04-24 14:48:11.000000 cloudmonitor-0.0.1.9/cloudmonitor/server.py
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       64 2023-04-23 13:11:47.000000 cloudmonitor-0.0.1.9/cloudmonitor/__main__.py
-drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-25 05:53:24.000000 cloudmonitor-0.0.1.9/cloudmonitor/templates/
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     9262 2023-04-24 14:09:06.000000 cloudmonitor-0.0.1.9/cloudmonitor/templates/index.html
-drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-25 05:53:24.000000 cloudmonitor-0.0.1.9/cloudmonitor/status/
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       21 2023-04-23 13:11:47.000000 cloudmonitor-0.0.1.9/cloudmonitor/status/__init__.py
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)      630 2023-04-23 13:11:47.000000 cloudmonitor-0.0.1.9/cloudmonitor/status/define.py
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     2327 2023-04-23 13:11:47.000000 cloudmonitor-0.0.1.9/cloudmonitor/status/query.py
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     1112 2023-04-25 05:53:24.000000 cloudmonitor-0.0.1.9/PKG-INFO
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     2714 2023-04-25 05:52:04.000000 cloudmonitor-0.0.1.9/setup.py
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)      284 2023-04-23 14:47:47.000000 cloudmonitor-0.0.1.9/README.md
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       38 2023-04-25 05:53:24.000000 cloudmonitor-0.0.1.9/setup.cfg
+drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-05-23 15:38:30.124479 cloudmonitor-1.0.0.0/
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       37 2023-04-25 05:53:10.000000 cloudmonitor-1.0.0.0/MANIFEST.in
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     3610 2023-05-23 15:38:30.124479 cloudmonitor-1.0.0.0/PKG-INFO
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     3032 2023-05-23 15:38:14.000000 cloudmonitor-1.0.0.0/README.md
+drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-05-23 15:38:30.124479 cloudmonitor-1.0.0.0/cloudmonitor/
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       49 2023-05-23 15:31:14.000000 cloudmonitor-1.0.0.0/cloudmonitor/__init__.py
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       64 2023-04-23 13:11:47.000000 cloudmonitor-1.0.0.0/cloudmonitor/__main__.py
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     2786 2023-04-25 05:38:08.000000 cloudmonitor-1.0.0.0/cloudmonitor/config.py
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     2157 2023-05-23 15:35:36.000000 cloudmonitor-1.0.0.0/cloudmonitor/server.py
+drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-05-23 15:38:30.124479 cloudmonitor-1.0.0.0/cloudmonitor/ssh/
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       22 2023-04-23 13:11:47.000000 cloudmonitor-1.0.0.0/cloudmonitor/ssh/__init__.py
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     1135 2023-04-23 14:10:51.000000 cloudmonitor-1.0.0.0/cloudmonitor/ssh/client.py
+drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-05-23 15:38:30.124479 cloudmonitor-1.0.0.0/cloudmonitor/status/
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       21 2023-04-23 13:11:47.000000 cloudmonitor-1.0.0.0/cloudmonitor/status/__init__.py
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)      630 2023-04-23 13:11:47.000000 cloudmonitor-1.0.0.0/cloudmonitor/status/define.py
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     2327 2023-04-23 13:11:47.000000 cloudmonitor-1.0.0.0/cloudmonitor/status/query.py
+drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-05-23 15:38:30.124479 cloudmonitor-1.0.0.0/cloudmonitor/templates/
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     9340 2023-05-23 15:21:45.000000 cloudmonitor-1.0.0.0/cloudmonitor/templates/index.html
+drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-05-23 15:38:30.124479 cloudmonitor-1.0.0.0/cloudmonitor.egg-info/
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     3610 2023-05-23 15:38:30.000000 cloudmonitor-1.0.0.0/cloudmonitor.egg-info/PKG-INFO
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)      525 2023-05-23 15:38:30.000000 cloudmonitor-1.0.0.0/cloudmonitor.egg-info/SOURCES.txt
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)        1 2023-05-23 15:38:30.000000 cloudmonitor-1.0.0.0/cloudmonitor.egg-info/dependency_links.txt
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       85 2023-05-23 15:38:30.000000 cloudmonitor-1.0.0.0/cloudmonitor.egg-info/entry_points.txt
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       57 2023-05-23 15:38:30.000000 cloudmonitor-1.0.0.0/cloudmonitor.egg-info/requires.txt
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       13 2023-05-23 15:38:30.000000 cloudmonitor-1.0.0.0/cloudmonitor.egg-info/top_level.txt
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       38 2023-05-23 15:38:30.124479 cloudmonitor-1.0.0.0/setup.cfg
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     2631 2023-05-23 15:37:38.000000 cloudmonitor-1.0.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cloudmonitor-0.0.1.9/cloudmonitor.egg-info/SOURCES.txt` & `cloudmonitor-1.0.0.0/cloudmonitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudmonitor-0.0.1.9/cloudmonitor/ssh/client.py` & `cloudmonitor-1.0.0.0/cloudmonitor/ssh/client.py`

 * *Files identical despite different names*

### Comparing `cloudmonitor-0.0.1.9/cloudmonitor/config.py` & `cloudmonitor-1.0.0.0/cloudmonitor/config.py`

 * *Files identical despite different names*

### Comparing `cloudmonitor-0.0.1.9/cloudmonitor/server.py` & `cloudmonitor-1.0.0.0/cloudmonitor/server.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import os
 import time
 import argparse, yaml
 import logging
 import functools
 from datetime import datetime, timedelta
 from flask import Flask, render_template, jsonify
+from gevent import pywsgi
 from .config import C, load_config, load_args
 from .status import update_servers
 
+
 __all__ = ["main"]
 
 app = Flask(
     __name__,
     template_folder=os.path.join(C.root_path, "templates")
 )
+
 parser = argparse.ArgumentParser(
     prog="Cloud Monitor",
-    description="A Web-GUI for monitoring servers",
-    # epilog='Text at the bottom of help'
+    description='''A Web-GUI for monitoring servers''',
+    epilog='''Pypi Homepage: https://pypi.org/project/cloudmonitor/'''
 )
 parser.add_argument("-c", "--config", dest="config", required=True, type=str, help="path of YAML config file")
 parser.add_argument("-p", "--port", dest="port", required=False, default=8899, type=int, help="port for Web GUI")
 parser.add_argument(
     "-w", "--workers", dest="workers", required=False, default=4, type=int, help="number of multi-process workers"
 )
 args = parser.parse_args()
@@ -45,17 +48,16 @@
 
         return wrapped_func
 
     return wrapper_cache
 
 
 @app.route("/")
-def hello_world():
+def index():
     status()
-    print(app.template_folder)
     return render_template("index.html", servers=C.status, refresh=C.refresh)
 
 
 @app.route("/reload")
 def reload():
     if not load_config(args.config):
         return "Error! Please see logs."
@@ -66,16 +68,11 @@
 @cache(seconds=C.refresh)
 def status():
     C.status = update_servers(C.servers)
     return jsonify(C.status)
 
 
 def main():
-    app.run(
-        host="0.0.0.0", 
-        port=C.port, 
-        debug=True
-    )
-
+    server = pywsgi.WSGIServer(('0.0.0.0', C.port), app)
+    server.serve_forever()
 
-if __name__ == "__main__":
-    main()
+if __name__ == "__main__": main()
```

### Comparing `cloudmonitor-0.0.1.9/cloudmonitor/templates/index.html` & `cloudmonitor-1.0.0.0/cloudmonitor/templates/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -154,21 +154,24 @@
             function refresh(){
                 $("#refresh").removeClass("btn-outline-success");
                 $("#refresh").addClass("btn-warning");
                 $("#refresh").attr("disabled", true);
                 $("#refresh").html("Processing");
                 $.getJSON("./status", function(result){
                     $.each(result, function(i, field){
-                        render_server_data(field);
-                        $("#refresh").addClass("btn-outline-success");
-                        $("#refresh").removeClass("btn-warning");
-                        $("#refresh").removeAttr("disabled");
-                        $("#refresh").html("Refresh (" + TOTAL_COUNT + "S)");
-                        CURRE_COUNT = 0;
+                        try {
+                           render_server_data(field);
+                        }
+                        catch(err) { }
                     });
+                    $("#refresh").addClass("btn-outline-success");
+                    $("#refresh").removeClass("btn-warning");
+                    $("#refresh").removeAttr("disabled");
+                    $("#refresh").html("Refresh (" + TOTAL_COUNT + "S)");
+                    CURRE_COUNT = 0;
                 });
             }
             
             $(refresh);
             $("#refresh").click(refresh);
             setInterval(function(){
                 if (CURRE_COUNT < TOTAL_COUNT){
```

### Comparing `cloudmonitor-0.0.1.9/cloudmonitor/status/define.py` & `cloudmonitor-1.0.0.0/cloudmonitor/status/define.py`

 * *Files identical despite different names*

### Comparing `cloudmonitor-0.0.1.9/cloudmonitor/status/query.py` & `cloudmonitor-1.0.0.0/cloudmonitor/status/query.py`

 * *Files identical despite different names*

### Comparing `cloudmonitor-0.0.1.9/setup.py` & `cloudmonitor-1.0.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,31 +31,30 @@
 
 # What packages are required for this module to be executed?
 # `estimator` may depend on other packages. In order to reduce dependencies, it is not written here.
 REQUIRED = [
     "flask>=2.0.0",
     "paramiko>=3.0.0",
     "pyyaml>=6.0",
+    "gevent>=22.10.2",
 ]
 
 here = os.path.abspath(os.path.dirname(__file__))
-with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
+with open(os.path.join(here, "PACKAGE.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 if __name__ == "__main__":
     setup(
         name=NAME,
         version=VERSION,
         license="MIT Licence",
         url="https://github.com/WNJXYK/cloudmonitor",
         packages=find_packages(),
         include_package_data=True,
-        # package_dir={"": "cloudmonitor"},
-        # package_data={"cloudmonitor.templates": ["*.html"]},
         author="Zhi Zhou",
         author_email="wnjxyk@gmail.com",
         description=DESCRIPTION,
         long_description=long_description,
         long_description_content_type="text/markdown",
         python_requires=REQUIRES_PYTHON,
         install_requires=REQUIRED,
```

