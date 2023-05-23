# Comparing `tmp/carpo_teacher-0.0.7.tar.gz` & `tmp/carpo_teacher-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carpo_teacher-0.0.7.tar", last modified: Wed Sep 21 16:51:52 2022, max compression
+gzip compressed data, was "carpo_teacher-0.0.9.tar", last modified: Tue May 23 14:23:28 2023, max compression
```

## Comparing `carpo_teacher-0.0.7.tar` & `carpo_teacher-0.0.9.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2022-09-21 16:51:52.803262 carpo_teacher-0.0.7/
--rw-rw-r--   0 kritish   (1000) kritish   (1000)       86 2022-04-22 15:03:31.000000 carpo_teacher-0.0.7/CHANGELOG.md
--rw-rw-r--   0 kritish   (1000) kritish   (1000)     1508 2022-04-22 15:03:31.000000 carpo_teacher-0.0.7/LICENSE
--rw-rw-r--   0 kritish   (1000) kritish   (1000)      447 2022-04-22 15:03:31.000000 carpo_teacher-0.0.7/MANIFEST.in
--rw-rw-r--   0 kritish   (1000) kritish   (1000)     4407 2022-09-21 16:51:52.803262 carpo_teacher-0.0.7/PKG-INFO
--rw-rw-r--   0 kritish   (1000) kritish   (1000)     3373 2022-07-01 16:27:22.000000 carpo_teacher-0.0.7/README.md
--rw-rw-r--   0 kritish   (1000) kritish   (1000)     1895 2022-04-22 15:03:31.000000 carpo_teacher-0.0.7/RELEASE.md
-drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2022-09-21 16:51:52.795262 carpo_teacher-0.0.7/carpo_teacher/
--rw-rw-r--   0 kritish   (1000) kritish   (1000)      976 2022-04-22 15:03:31.000000 carpo_teacher-0.0.7/carpo_teacher/__init__.py
--rw-rw-r--   0 kritish   (1000) kritish   (1000)      625 2022-04-22 15:03:31.000000 carpo_teacher-0.0.7/carpo_teacher/_version.py
--rw-rw-r--   0 kritish   (1000) kritish   (1000)    21705 2022-08-26 06:30:21.000000 carpo_teacher-0.0.7/carpo_teacher/handlers.py
-drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2022-09-21 16:51:52.795262 carpo_teacher-0.0.7/carpo_teacher/labextension/
--rw-rw-r--   0 kritish   (1000) kritish   (1000)    20784 2022-08-26 06:29:13.000000 carpo_teacher-0.0.7/carpo_teacher/labextension/build_log.json
--rw-rw-r--   0 kritish   (1000) kritish   (1000)     3747 2022-08-26 06:29:14.000000 carpo_teacher-0.0.7/carpo_teacher/labextension/package.json
-drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2022-09-21 16:51:52.799262 carpo_teacher-0.0.7/carpo_teacher/labextension/static/
--rw-rw-r--   0 kritish   (1000) kritish   (1000)    36383 2022-08-26 06:29:14.000000 carpo_teacher-0.0.7/carpo_teacher/labextension/static/lib_index_js.63bb1f0b3e113fb2d1b6.js
--rw-rw-r--   0 kritish   (1000) kritish   (1000)    32294 2022-08-26 06:29:14.000000 carpo_teacher-0.0.7/carpo_teacher/labextension/static/lib_index_js.63bb1f0b3e113fb2d1b6.js.map
--rw-rw-r--   0 kritish   (1000) kritish   (1000)    28925 2022-08-26 06:29:14.000000 carpo_teacher-0.0.7/carpo_teacher/labextension/static/remoteEntry.d6f902fe01b1dc4f6fba.js
--rw-rw-r--   0 kritish   (1000) kritish   (1000)    27698 2022-08-26 06:29:14.000000 carpo_teacher-0.0.7/carpo_teacher/labextension/static/remoteEntry.d6f902fe01b1dc4f6fba.js.map
--rw-rw-r--   0 kritish   (1000) kritish   (1000)      156 2022-08-26 06:29:13.000000 carpo_teacher-0.0.7/carpo_teacher/labextension/static/style.js
--rw-rw-r--   0 kritish   (1000) kritish   (1000)     7398 2022-08-26 06:29:14.000000 carpo_teacher-0.0.7/carpo_teacher/labextension/static/style_index_js.fc6324d8ef291b0fdd9a.js
--rw-rw-r--   0 kritish   (1000) kritish   (1000)     5848 2022-08-26 06:29:14.000000 carpo_teacher-0.0.7/carpo_teacher/labextension/static/style_index_js.fc6324d8ef291b0fdd9a.js.map
--rw-rw-r--   0 kritish   (1000) kritish   (1000)    12056 2022-08-26 06:29:14.000000 carpo_teacher-0.0.7/carpo_teacher/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.6760bbd0c725e3542c7a.js
--rw-rw-r--   0 kritish   (1000) kritish   (1000)    13787 2022-08-26 06:29:14.000000 carpo_teacher-0.0.7/carpo_teacher/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.6760bbd0c725e3542c7a.js.map
-drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2022-09-21 16:51:52.795262 carpo_teacher-0.0.7/carpo_teacher.egg-info/
--rw-rw-r--   0 kritish   (1000) kritish   (1000)     4407 2022-09-21 16:51:52.000000 carpo_teacher-0.0.7/carpo_teacher.egg-info/PKG-INFO
--rw-rw-r--   0 kritish   (1000) kritish   (1000)     1519 2022-09-21 16:51:52.000000 carpo_teacher-0.0.7/carpo_teacher.egg-info/SOURCES.txt
--rw-rw-r--   0 kritish   (1000) kritish   (1000)        1 2022-09-21 16:51:52.000000 carpo_teacher-0.0.7/carpo_teacher.egg-info/dependency_links.txt
--rw-rw-r--   0 kritish   (1000) kritish   (1000)        1 2022-04-08 22:47:07.000000 carpo_teacher-0.0.7/carpo_teacher.egg-info/not-zip-safe
--rw-rw-r--   0 kritish   (1000) kritish   (1000)       23 2022-09-21 16:51:52.000000 carpo_teacher-0.0.7/carpo_teacher.egg-info/requires.txt
--rw-rw-r--   0 kritish   (1000) kritish   (1000)       14 2022-09-21 16:51:52.000000 carpo_teacher-0.0.7/carpo_teacher.egg-info/top_level.txt
--rw-rw-r--   0 kritish   (1000) kritish   (1000)      187 2022-04-22 15:03:31.000000 carpo_teacher-0.0.7/install.json
-drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2022-09-21 16:51:52.791262 carpo_teacher-0.0.7/jupyter-config/
-drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2022-09-21 16:51:52.799262 carpo_teacher-0.0.7/jupyter-config/nb-config/
--rw-rw-r--   0 kritish   (1000) kritish   (1000)       90 2022-04-22 15:03:31.000000 carpo_teacher-0.0.7/jupyter-config/nb-config/carpo_teacher.json
-drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2022-09-21 16:51:52.799262 carpo_teacher-0.0.7/jupyter-config/server-config/
--rw-rw-r--   0 kritish   (1000) kritish   (1000)       88 2022-04-22 15:03:31.000000 carpo_teacher-0.0.7/jupyter-config/server-config/carpo_teacher.json
--rw-rw-r--   0 kritish   (1000) kritish   (1000)     3605 2022-09-21 16:51:29.000000 carpo_teacher-0.0.7/package.json
--rw-rw-r--   0 kritish   (1000) kritish   (1000)      587 2022-04-22 15:03:31.000000 carpo_teacher-0.0.7/pyproject.toml
--rw-rw-r--   0 kritish   (1000) kritish   (1000)       38 2022-09-21 16:51:52.803262 carpo_teacher-0.0.7/setup.cfg
--rw-rw-r--   0 kritish   (1000) kritish   (1000)     3181 2022-04-22 15:03:31.000000 carpo_teacher-0.0.7/setup.py
-drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2022-09-21 16:51:52.803262 carpo_teacher-0.0.7/src/
--rw-rw-r--   0 kritish   (1000) kritish   (1000)     1100 2022-05-14 23:57:30.000000 carpo_teacher-0.0.7/src/handler.ts
--rw-rw-r--   0 kritish   (1000) kritish   (1000)    15039 2022-08-26 06:31:10.000000 carpo_teacher-0.0.7/src/index.ts
--rw-rw-r--   0 kritish   (1000) kritish   (1000)      211 2022-04-22 15:03:31.000000 carpo_teacher-0.0.7/src/model.ts
--rw-rw-r--   0 kritish   (1000) kritish   (1000)     2550 2022-07-07 03:50:43.000000 carpo_teacher-0.0.7/src/upload-solution.ts
--rw-rw-r--   0 kritish   (1000) kritish   (1000)     7238 2022-08-26 05:49:15.000000 carpo_teacher-0.0.7/src/widget.tsx
-drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2022-09-21 16:51:52.803262 carpo_teacher-0.0.7/style/
--rw-rw-r--   0 kritish   (1000) kritish   (1000)     1153 2022-07-06 21:53:44.000000 carpo_teacher-0.0.7/style/base.css
--rw-rw-r--   0 kritish   (1000) kritish   (1000)       26 2022-04-22 15:03:31.000000 carpo_teacher-0.0.7/style/index.css
--rw-rw-r--   0 kritish   (1000) kritish   (1000)       21 2022-04-22 15:03:31.000000 carpo_teacher-0.0.7/style/index.js
--rw-rw-r--   0 kritish   (1000) kritish   (1000)      555 2022-04-22 15:03:31.000000 carpo_teacher-0.0.7/tsconfig.json
+drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2023-05-23 14:23:28.191575 carpo_teacher-0.0.9/
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)       86 2022-04-22 15:03:31.000000 carpo_teacher-0.0.9/CHANGELOG.md
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)     3373 2022-10-14 15:34:26.000000 carpo_teacher-0.0.9/DEV_INSTALL.md
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)     1508 2022-04-22 15:03:31.000000 carpo_teacher-0.0.9/LICENSE
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)      447 2022-04-22 15:03:31.000000 carpo_teacher-0.0.9/MANIFEST.in
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)     2755 2023-05-23 14:23:28.191575 carpo_teacher-0.0.9/PKG-INFO
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)     1721 2022-10-17 17:31:16.000000 carpo_teacher-0.0.9/README.md
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)     1895 2022-04-22 15:03:31.000000 carpo_teacher-0.0.9/RELEASE.md
+drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2023-05-23 14:23:28.187575 carpo_teacher-0.0.9/carpo_teacher/
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)      976 2022-04-22 15:03:31.000000 carpo_teacher-0.0.9/carpo_teacher/__init__.py
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)      625 2022-04-22 15:03:31.000000 carpo_teacher-0.0.9/carpo_teacher/_version.py
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)    22717 2023-05-23 14:01:44.000000 carpo_teacher-0.0.9/carpo_teacher/handlers.py
+drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2023-05-23 14:23:28.187575 carpo_teacher-0.0.9/carpo_teacher/labextension/
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)    20784 2023-05-23 13:47:21.000000 carpo_teacher-0.0.9/carpo_teacher/labextension/build_log.json
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)     3747 2023-05-23 13:47:22.000000 carpo_teacher-0.0.9/carpo_teacher/labextension/package.json
+drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2023-05-23 14:23:28.191575 carpo_teacher-0.0.9/carpo_teacher/labextension/static/
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)    36224 2023-05-23 13:47:22.000000 carpo_teacher-0.0.9/carpo_teacher/labextension/static/lib_index_js.26b2dac9fb26b92e5e77.js
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)    32296 2023-05-23 13:47:22.000000 carpo_teacher-0.0.9/carpo_teacher/labextension/static/lib_index_js.26b2dac9fb26b92e5e77.js.map
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)    28925 2023-05-23 13:47:22.000000 carpo_teacher-0.0.9/carpo_teacher/labextension/static/remoteEntry.991b8dc2b6efb319125a.js
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)    27698 2023-05-23 13:47:22.000000 carpo_teacher-0.0.9/carpo_teacher/labextension/static/remoteEntry.991b8dc2b6efb319125a.js.map
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)      156 2023-05-23 13:47:21.000000 carpo_teacher-0.0.9/carpo_teacher/labextension/static/style.js
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)     7398 2023-05-23 13:47:22.000000 carpo_teacher-0.0.9/carpo_teacher/labextension/static/style_index_js.fc6324d8ef291b0fdd9a.js
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)     5848 2023-05-23 13:47:22.000000 carpo_teacher-0.0.9/carpo_teacher/labextension/static/style_index_js.fc6324d8ef291b0fdd9a.js.map
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)    12056 2023-05-23 13:47:22.000000 carpo_teacher-0.0.9/carpo_teacher/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.6760bbd0c725e3542c7a.js
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)    13787 2023-05-23 13:47:22.000000 carpo_teacher-0.0.9/carpo_teacher/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.6760bbd0c725e3542c7a.js.map
+drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2023-05-23 14:23:28.187575 carpo_teacher-0.0.9/carpo_teacher.egg-info/
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)     2755 2023-05-23 14:23:27.000000 carpo_teacher-0.0.9/carpo_teacher.egg-info/PKG-INFO
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)     1534 2023-05-23 14:23:28.000000 carpo_teacher-0.0.9/carpo_teacher.egg-info/SOURCES.txt
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)        1 2023-05-23 14:23:27.000000 carpo_teacher-0.0.9/carpo_teacher.egg-info/dependency_links.txt
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)        1 2022-04-08 22:47:07.000000 carpo_teacher-0.0.9/carpo_teacher.egg-info/not-zip-safe
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)       23 2023-05-23 14:23:28.000000 carpo_teacher-0.0.9/carpo_teacher.egg-info/requires.txt
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)       14 2023-05-23 14:23:28.000000 carpo_teacher-0.0.9/carpo_teacher.egg-info/top_level.txt
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)      187 2022-04-22 15:03:31.000000 carpo_teacher-0.0.9/install.json
+drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2023-05-23 14:23:28.183575 carpo_teacher-0.0.9/jupyter-config/
+drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2023-05-23 14:23:28.191575 carpo_teacher-0.0.9/jupyter-config/nb-config/
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)       90 2022-04-22 15:03:31.000000 carpo_teacher-0.0.9/jupyter-config/nb-config/carpo_teacher.json
+drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2023-05-23 14:23:28.191575 carpo_teacher-0.0.9/jupyter-config/server-config/
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)       88 2022-04-22 15:03:31.000000 carpo_teacher-0.0.9/jupyter-config/server-config/carpo_teacher.json
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)     3605 2023-05-23 14:01:15.000000 carpo_teacher-0.0.9/package.json
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)      587 2022-04-22 15:03:31.000000 carpo_teacher-0.0.9/pyproject.toml
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)       38 2023-05-23 14:23:28.191575 carpo_teacher-0.0.9/setup.cfg
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)     3181 2022-04-22 15:03:31.000000 carpo_teacher-0.0.9/setup.py
+drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2023-05-23 14:23:28.191575 carpo_teacher-0.0.9/src/
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)     1100 2022-05-14 23:57:30.000000 carpo_teacher-0.0.9/src/handler.ts
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)    14556 2023-05-23 14:00:26.000000 carpo_teacher-0.0.9/src/index.ts
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)      211 2022-04-22 15:03:31.000000 carpo_teacher-0.0.9/src/model.ts
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)     2550 2023-03-16 21:41:54.000000 carpo_teacher-0.0.9/src/upload-solution.ts
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)     7238 2023-02-17 05:46:19.000000 carpo_teacher-0.0.9/src/widget.tsx
+drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2023-05-23 14:23:28.191575 carpo_teacher-0.0.9/style/
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)     1153 2022-10-14 15:34:26.000000 carpo_teacher-0.0.9/style/base.css
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)       26 2022-04-22 15:03:31.000000 carpo_teacher-0.0.9/style/index.css
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)       21 2022-04-22 15:03:31.000000 carpo_teacher-0.0.9/style/index.js
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)      555 2022-04-22 15:03:31.000000 carpo_teacher-0.0.9/tsconfig.json
```

### Comparing `carpo_teacher-0.0.7/LICENSE` & `carpo_teacher-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `carpo_teacher-0.0.7/README.md` & `carpo_teacher-0.0.9/DEV_INSTALL.md`

 * *Files identical despite different names*

### Comparing `carpo_teacher-0.0.7/RELEASE.md` & `carpo_teacher-0.0.9/RELEASE.md`

 * *Files identical despite different names*

### Comparing `carpo_teacher-0.0.7/carpo_teacher/__init__.py` & `carpo_teacher-0.0.9/carpo_teacher/__init__.py`

 * *Files identical despite different names*

### Comparing `carpo_teacher-0.0.7/carpo_teacher/_version.py` & `carpo_teacher-0.0.9/carpo_teacher/_version.py`

 * *Files identical despite different names*

### Comparing `carpo_teacher-0.0.7/carpo_teacher/handlers.py` & `carpo_teacher-0.0.9/carpo_teacher/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
    
     # Create config.json file
     config_path = os.path.join(current_dir,"Exercises","config.json")
     if not os.path.isfile(config_path):
         config_data = {}
         config_data['name'] = "John Smith"
         config_data['server'] = "http://delphinus.cs.memphis.edu:XXXX"
-        config_data['carpo_version'] = "0.0.1"
+        config_data['carpo_version'] = "0.0.9"
         # Write default config
         with open(config_path, "w") as config_file:
             config_file.write(json.dumps(config_data, indent=4))
     
     # Create blank notebook
     notebook_path = os.path.join(current_dir,"Exercises","Readme.ipynb")
     if not os.path.isfile(notebook_path):
@@ -122,14 +122,15 @@
             print(response)
         except requests.exceptions.RequestException as e:
             self.set_status(500)
             self.finish(json.dumps({'message': "Carpo Server Error. {}".format(e)}))
             return
 
         config_data['id'] = response['id']
+        config_data['uuid'] = response['uuid']
         # Write id to the json file.
         with open(os.path.join(os.getcwd(),"Exercises",'config.json'), "w") as config_file:
             config_file.write(json.dumps(config_data, indent=4))
         print(response)
         self.finish(response)
         
 class SubmissionHandler(APIHandler):
@@ -480,27 +481,48 @@
     # The following decorator should be present on all verb methods (head, get, post,
     # patch, put, delete, options) to ensure only authorized user can request the
     # Jupyter server
 
     @tornado.web.authenticated
     def get(self):
         # input_data is a dictionary with a key "name"
-        input_data = self.get_json_body()
+        # input_data = self.get_json_body()
 
         config_data = read_config_file()
 
         if not {'id', 'name', 'server'}.issubset(config_data):
             self.set_status(500)
             self.finish(json.dumps({'message': "User is not registered. Please Register User."}))
             return
 
         problems_status_url = config_data['server'] + "/problems/status"
 
         self.finish({"url":problems_status_url })
     
+class GoWebAppRouteHandler(APIHandler):
+    @tornado.web.authenticated
+    def get(self):
+        # input_data is a dictionary with a key "name"
+        # input_data = self.get_json_body()
+        config_data = read_config_file()
+
+        if not {'id', 'name', 'server'}.issubset(config_data):
+            self.set_status(500)
+            self.finish(json.dumps({'message': "User is not registered. Please Register User."}))
+            return
+
+        if not {'app_url'}.issubset(config_data):
+            self.set_status(500)
+            self.finish(json.dumps({'message': "app_url not found in config."}))
+            return
+
+        web_page_url = config_data['app_url'] +"/#/?token="+ config_data['uuid']
+
+        self.finish({"url":web_page_url })
+
 def setup_handlers(web_app):
     host_pattern = ".*$"
 
     base_url = web_app.settings["base_url"]
     route_pattern_code = url_path_join(base_url, "carpo-teacher", "submissions")
     handlers = [(route_pattern_code, SubmissionHandler)]
     web_app.add_handlers(host_pattern, handlers)
@@ -521,7 +543,11 @@
     web_app.add_handlers(host_pattern, [(route_pattern_register, RegistrationHandler, dict(config_files = create_initial_files()))])
 
     route_pattern_problems_status =  url_path_join(web_app.settings['base_url'], "carpo-teacher", "view_problem_list")
     web_app.add_handlers(host_pattern, [(route_pattern_problems_status, ViewProblemStatusRouteHandler)])
 
     route_pattern_problems_status =  url_path_join(web_app.settings['base_url'], "carpo-teacher", "solution")
     web_app.add_handlers(host_pattern, [(route_pattern_problems_status, SolutionHandler)])
+
+    route_pattern_problems_status =  url_path_join(web_app.settings['base_url'], "carpo-teacher", "view_app")
+    web_app.add_handlers(host_pattern, [(route_pattern_problems_status, GoWebAppRouteHandler)])
+
```

### Comparing `carpo_teacher-0.0.7/carpo_teacher/labextension/build_log.json` & `carpo_teacher-0.0.9/carpo_teacher/labextension/build_log.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999992921055613%*

 * *Differences: {'0': "{'plugins': {1: {'_options': {'shared': {'carpo-teacher': {'version': '0.0.7'}}}}}}"}*

```diff
@@ -580,15 +580,15 @@
                             "import": false,
                             "requiredVersion": "^1.30.0",
                             "singleton": true
                         },
                         "carpo-teacher": {
                             "import": "/home/kritish/Projects/carpo/carpo_teacher/lib/index.js",
                             "singleton": true,
-                            "version": "0.0.6"
+                            "version": "0.0.7"
                         },
                         "react": {
                             "import": false,
                             "requiredVersion": "^17.0.1",
                             "singleton": true
                         },
                         "react-dom": {
```

### Comparing `carpo_teacher-0.0.7/carpo_teacher/labextension/package.json` & `carpo_teacher-0.0.9/carpo_teacher/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9756944444444444%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.991b8dc2b6efb319125a.js'}}",*

 * * "'version'": "'0.0.7'"}*

```diff
@@ -48,15 +48,15 @@
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.d6f902fe01b1dc4f6fba.js",
+            "load": "static/remoteEntry.991b8dc2b6efb319125a.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "carpo_teacher"
                 },
@@ -111,9 +111,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.0.6"
+    "version": "0.0.7"
 }
```

### Comparing `carpo_teacher-0.0.7/carpo_teacher/labextension/static/lib_index_js.63bb1f0b3e113fb2d1b6.js` & `carpo_teacher-0.0.9/carpo_teacher/labextension/static/lib_index_js.26b2dac9fb26b92e5e77.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -75,23 +75,23 @@
                 /* harmony export */
                 __webpack_require__.d(__webpack_exports__, {
                     /* harmony export */
                     "AllSubmissionButtonExtension": () => ( /* binding */ AllSubmissionButtonExtension),
                     /* harmony export */
                     "ArchiveProblemButtonExtension": () => ( /* binding */ ArchiveProblemButtonExtension),
                     /* harmony export */
+                    "GoToApp": () => ( /* binding */ GoToApp),
+                    /* harmony export */
                     "NewSubmissionButtonExtension": () => ( /* binding */ NewSubmissionButtonExtension),
                     /* harmony export */
                     "PublishProblemButtonExtension": () => ( /* binding */ PublishProblemButtonExtension),
                     /* harmony export */
                     "RegisterButton": () => ( /* binding */ RegisterButton),
                     /* harmony export */
-                    "default": () => (__WEBPACK_DEFAULT_EXPORT__),
-                    /* harmony export */
-                    "viewProblemStatusExtension": () => ( /* binding */ viewProblemStatusExtension)
+                    "default": () => (__WEBPACK_DEFAULT_EXPORT__)
                     /* harmony export */
                 });
                 /* harmony import */
                 var _handler__WEBPACK_IMPORTED_MODULE_6__ = __webpack_require__( /*! ./handler */ "./lib/handler.js");
                 /* harmony import */
                 var _jupyterlab_notebook__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__( /*! @jupyterlab/notebook */ "webpack/sharing/consume/default/@jupyterlab/notebook");
                 /* harmony import */
@@ -152,15 +152,14 @@
                                                 });
                                             }
                                         });
                                     }
                                     const cell = notebook.activeCell;
                                     var sCell;
                                     const activeIndex = notebook.activeCellIndex;
-                                    console.log("Active cell index: ", activeIndex);
                                     // const heading = cell.model.value.text.split("\n")[0].split(" ")
                                     const submission_id = function(text) {
                                         return Number(text.split("\n")[0].split(" ")[2]);
                                     };
                                     const problem_id = function(text) {
                                         return Number(text.split("\n")[0].split(" ")[1]);
                                     };
@@ -170,27 +169,14 @@
                                     var info = {
                                         id: submission_id(cell.model.value.text),
                                         problem_id: problem_id(cell.model.value.text),
                                         student_id: student_id(cell.model.value.text),
                                         code: cell.model.value.text
                                     };
                                     var header;
-                                    // For feedback case: cell is markdown so loop over the notebook widgets to get code cell before the active cell index
-                                    // if (cell.model.type == 'markdown' ){
-                                    //   notebook.widgets.map((c,index) =>{
-                                    //     // activeIndex-1 could be the top cell (when the question type is markdown)
-                                    //     if(index == activeIndex-1 && !c.model.value.text.startsWith("## Submission")) {
-                                    //       const code = c.model.value.text
-                                    //       info.code = code  
-                                    //       info.id = submission_id(code)
-                                    //       info.student_id = student_id(code)
-                                    //       info.problem_id = problem_id(code)
-                                    //     }
-                                    //   })
-                                    // }
                                     // Get the status cell:
                                     notebook.widgets.map((c, index) => {
                                         if (index == activeIndex + 1) {
                                             sCell = c;
                                         }
                                     });
                                     header = cell.model.value.text.split("\n")[0];
@@ -202,31 +188,26 @@
                                         currentCellCheckButton = newCheckButton;
                                     } else {
                                         const newFeedbackButton = new _widget__WEBPACK_IMPORTED_MODULE_4__.FeedbackButton(cell, info);
                                         cell.layout.addWidget(newFeedbackButton);
                                         currentCell = cell;
                                         currentCellCheckButton = newFeedbackButton;
                                     }
-                                    // if (question.includes("## PID ")){
-                                    //   (cell.layout as PanelLayout).addWidget(newCheckButton);
-                                    //   currentCellCheckButton = newCheckButton;
-                                    // }
-                                    // Set the current cell and button for future
-                                    // reference
                                 });
                             });
                         });
                         //  tell the document registry about your widget extension:
                         app.docRegistry.addWidgetExtension('Notebook', new RegisterButton());
-                        app.docRegistry.addWidgetExtension('Notebook', new NewSubmissionButtonExtension());
-                        app.docRegistry.addWidgetExtension('Notebook', new AllSubmissionButtonExtension());
+                        app.docRegistry.addWidgetExtension('Notebook', new GoToApp());
+                        // app.docRegistry.addWidgetExtension('Notebook', new NewSubmissionButtonExtension());
+                        // app.docRegistry.addWidgetExtension('Notebook', new AllSubmissionButtonExtension());
                         app.docRegistry.addWidgetExtension('Notebook', new PublishProblemButtonExtension());
                         app.docRegistry.addWidgetExtension('Notebook', new ArchiveProblemButtonExtension());
                         app.docRegistry.addWidgetExtension('Notebook', new _upload_solution__WEBPACK_IMPORTED_MODULE_5__.GetSolutionButton());
-                        app.docRegistry.addWidgetExtension('Notebook', new viewProblemStatusExtension());
+                        // app.docRegistry.addWidgetExtension('Notebook', new viewProblemStatusExtension());
                     }
                 };
                 class RegisterButton {
                     /**
                      * Create a new extension for the notebook panel widget.
                      *
                      * @param panel Notebook panel
@@ -261,14 +242,41 @@
                         });
                         panel.toolbar.insertItem(10, 'register', button);
                         return new _lumino_disposable__WEBPACK_IMPORTED_MODULE_2__.DisposableDelegate(() => {
                             button.dispose();
                         });
                     }
                 }
+                class GoToApp {
+                    createNew(panel, context) {
+                        const viewWebApp = () => {
+                            (0, _handler__WEBPACK_IMPORTED_MODULE_6__.requestAPI)('view_app', {
+                                method: 'GET'
+                            })
+                            .then(data => {
+                                    // console.log(data);
+                                    window.open(data.url, "_blank");
+                                })
+                                .catch(reason => {
+                                    (0, _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_3__.showErrorMessage)('View App Status Error', reason);
+                                    console.error(`Failed to view app status.\n${reason}`);
+                                });
+                        };
+                        const button = new _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_3__.ToolbarButton({
+                            className: 'get-app-button',
+                            label: 'App',
+                            onClick: viewWebApp,
+                            tooltip: 'Go to the web app',
+                        });
+                        panel.toolbar.insertItem(11, 'viewWebApp', button);
+                        return new _lumino_disposable__WEBPACK_IMPORTED_MODULE_2__.DisposableDelegate(() => {
+                            button.dispose();
+                        });
+                    }
+                }
                 class NewSubmissionButtonExtension {
                     /**
                      * Create a new extension for the notebook panel widget.
                      *
                      * @param panel Notebook panel
                      * @param context Notebook context
                      * @returns Disposable on the added button
@@ -418,15 +426,15 @@
                         };
                         const button = new _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_3__.ToolbarButton({
                             className: 'publish-problem-button',
                             label: 'Publish',
                             onClick: publishProblem,
                             tooltip: 'Publish New Problem.',
                         });
-                        panel.toolbar.insertItem(13, 'publishNewProblem', button);
+                        panel.toolbar.insertItem(12, 'publishNewProblem', button);
                         return new _lumino_disposable__WEBPACK_IMPORTED_MODULE_2__.DisposableDelegate(() => {
                             button.dispose();
                         });
                     }
                 }
                 class ArchiveProblemButtonExtension {
                     /**
@@ -476,54 +484,62 @@
                         };
                         const button = new _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_3__.ToolbarButton({
                             className: 'archive-problem-button',
                             label: 'Unpublish',
                             onClick: archiveProblem,
                             tooltip: 'Unpublish the problem.',
                         });
-                        panel.toolbar.insertItem(14, 'archivesProblem', button);
-                        return new _lumino_disposable__WEBPACK_IMPORTED_MODULE_2__.DisposableDelegate(() => {
-                            button.dispose();
-                        });
-                    }
-                }
-                class viewProblemStatusExtension {
-                    /**
-                     * Create a new extension for the notebook panel widget.
-                     *
-                     * @param panel Notebook panel
-                     * @param context Notebook context
-                     * @returns Disposable on the added button
-                     */
-                    createNew(panel, context) {
-                        const viewProblemStatus = () => {
-                            (0, _handler__WEBPACK_IMPORTED_MODULE_6__.requestAPI)('view_problem_list', {
-                                method: 'GET'
-                            })
-                            .then(data => {
-                                    console.log(data);
-                                    window.open(data.url, "_blank");
-                                })
-                                .catch(reason => {
-                                    (0, _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_3__.showErrorMessage)('View Problem Status Error', reason);
-                                    console.error(`Failed to view problem status.\n${reason}`);
-                                });
-                        };
-                        const button = new _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_3__.ToolbarButton({
-                            className: 'get-status-button',
-                            label: 'Problems',
-                            onClick: viewProblemStatus,
-                            tooltip: 'View all problem status',
-                        });
-                        panel.toolbar.insertItem(16, 'viewProblemStatus', button);
+                        panel.toolbar.insertItem(13, 'archivesProblem', button);
                         return new _lumino_disposable__WEBPACK_IMPORTED_MODULE_2__.DisposableDelegate(() => {
                             button.dispose();
                         });
                     }
                 }
+                // export class viewProblemStatusExtension
+                //   implements DocumentRegistry.IWidgetExtension<NotebookPanel, INotebookModel>
+                // {
+                //   /**
+                //    * Create a new extension for the notebook panel widget.
+                //    *
+                //    * @param panel Notebook panel
+                //    * @param context Notebook context
+                //    * @returns Disposable on the added button
+                //    */
+                //   createNew(
+                //     panel: NotebookPanel,
+                //     context: DocumentRegistry.IContext<INotebookModel>
+                //   ): IDisposable {
+                //     const viewProblemStatus = () => {
+                //       requestAPI<any>('view_problem_list',{
+                //         method: 'GET'
+                //       })
+                //         .then(data => {
+                //           console.log(data);
+                //           window.open(
+                //             data.url, "_blank");
+                //         })
+                //         .catch(reason => {
+                //           showErrorMessage('View Problem Status Error', reason);
+                //           console.error(
+                //             `Failed to view problem status.\n${reason}`
+                //           );
+                //         });
+                //     };
+                //     const button = new ToolbarButton({
+                //       className: 'get-status-button',
+                //       label: 'Problems',
+                //       onClick: viewProblemStatus,
+                //       tooltip: 'View all problem status',
+                //     });
+                //     panel.toolbar.insertItem(15, 'viewProblemStatus', button);
+                //     return new DisposableDelegate(() => {
+                //       button.dispose();
+                //     });
+                //   }
+                // }
                 /* harmony default export */
                 const __WEBPACK_DEFAULT_EXPORT__ = (plugin);
 
 
                 /***/
             }),
 
@@ -603,15 +619,15 @@
                         };
                         const button = new _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_1__.ToolbarButton({
                             className: 'upload-solution-button',
                             label: 'UploadSolution',
                             onClick: uploadSolution,
                             tooltip: 'Upload solutions to the problem.',
                         });
-                        panel.toolbar.insertItem(15, 'getSolutions', button);
+                        panel.toolbar.insertItem(14, 'getSolutions', button);
                         return new _lumino_disposable__WEBPACK_IMPORTED_MODULE_0__.DisposableDelegate(() => {
                             button.dispose();
                         });
                     }
                 }
 
 
@@ -871,8 +887,8 @@
 
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=lib_index_js.63bb1f0b3e113fb2d1b6.js.map
+//# sourceMappingURL=lib_index_js.26b2dac9fb26b92e5e77.js.map
```

### Comparing `carpo_teacher-0.0.7/carpo_teacher/labextension/static/lib_index_js.63bb1f0b3e113fb2d1b6.js.map` & `carpo_teacher-0.0.9/carpo_teacher/labextension/static/lib_index_js.26b2dac9fb26b92e5e77.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8095238095238094%*

 * *Differences: {"'file'": "'lib_index_js.26b2dac9fb26b92e5e77.js'",*

 * * "'mappings'": "';;;;;;;;;;;;;;;;;AAA+C;AACS;AACxD;AACA;AACA;AACA;AACA;AACA;AACA;AACO,kDAAkD;AACzD;AACA,qBAAqB,+EAA6B;AAClD,uBAAuB,8DAAW;AAClC;AACA;AACA;AACA,yBAAyB,8EAA4B;AACrD;AACA;AACA,kBAAkB,+EAA6B;AAC/C;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,kBAAkB,gFAA8B;AAChD;AACA;AACA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AClCuC;AACkC;AACd;AACG;AAC9D,YAAY,OAAO;AACqC;AACmC;AACrC;AACtD;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,kEAAgB;AAC/B,eAAe,wEAAmB;AAClC;AACA;A […]*

```diff
@@ -1,19 +1,19 @@
 {
-    "file": "lib_index_js.63bb1f0b3e113fb2d1b6.js",
-    "mappings": ";;;;;;;;;;;;;;;;;AAA+C;AACS;AACxD;AACA;AACA;AACA;AACA;AACA;AACA;AACO,kDAAkD;AACzD;AACA,qBAAqB,+EAA6B;AAClD,uBAAuB,8DAAW;AAClC;AACA;AACA;AACA,yBAAyB,8EAA4B;AACrD;AACA;AACA,kBAAkB,+EAA6B;AAC/C;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,kBAAkB,gFAA8B;AAChD;AACA;AACA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AClCuC;AACkC;AACd;AACG;AAC9D,YAAY,OAAO;AACqC;AACmC;AACrC;AACtD;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,kEAAgB;AAC/B,eAAe,wEAAmB;AAClC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iCAAiC;AACjC;AACA,yBAAyB;AACzB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,0BAA0B;AAC1B;AACA;AACA;AACA;AACA;AACA;AACA,qBAAqB;AACrB;AACA;AACA;AACA,mDAAmD,oDAAe;AAClE;AACA;AACA;AACA;AACA;AACA,sDAAsD,mDAAc;AACpE;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iBAAiB;AACjB,aAAa;AACb,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA,2DAA2D,+DAAiB;AAC5E;AACA;AACA;AACO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,oDAAU;AACtB;AACA,aAAa;AACb;AACA;AACA,gBAAgB,gEAAU;AAC1B;AACA;AACA,8BAA8B,iEAAe,GAAG,aAAa;AAC7D,iBAAiB;AACjB,aAAa;AACb;AACA,gBAAgB,sEAAgB;AAChC,sEAAsE,OAAO;AAC7E,aAAa;AACb;AACA,2BAA2B,+DAAa;AACxC;AACA;AACA;AACA;AACA,SAAS;AACT;AACA,mBAAmB,kEAAkB;AACrC;AACA,SAAS;AACT;AACA;AACO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,iFAA+B;AAC3C,YAAY,oDAAU;AACtB;AACA,aAAa;AACb;AACA;AACA;AACA;AACA;AACA;AACA;AACA,gBAAgB,gEAAU;AAC1B;AACA;AACA,8BAA8B,iEAAe,GAAG,aAAa;AAC7D,iBAAiB;AACjB;AACA,aAAa;AACb;AACA,gBAAgB,sEAAgB;AAChC,8GAA8G,OAAO;AACrH,aAAa;AACb;AACA,2BAA2B,+DAAa;AACxC;AACA;AACA;AACA;AACA,SAAS;AACT;AACA,mBAAmB,kEAAkB;AACrC;AACA,SAAS;AACT;AACA;AACO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,iFAA+B;AAC3C,YAAY,oDAAU;AACtB;AACA,aAAa;AACb;AACA,gBAAgB,gEAAU;AAC1B;AACA;AACA,8BAA8B,iEAAe,GAAG,aAAa;AAC7D,iBAAiB;AACjB;AACA,aAAa;AACb;AACA,gBAAgB,sEAAgB;AAChC,8GAA8G,OAAO;AACrH,aAAa;AACb;AACA,2BAA2B,+DAAa;AACxC;AACA;AACA;AACA;AACA,SAAS;AACT;AACA,mBAAmB,kEAAkB;AACrC;AACA,SAAS;AACT;AACA;AACO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,iFAA+B;AAC3C;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACA,gBAAgB,sEAAgB;AAChC;AACA;AACA;AACA,gBAAgB,sEAAgB;AAChC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,oDAAU;AACtB;AACA;AACA,aAAa;AACb;AACA;AACA;AACA;AACA;AACA;AACA,iBAAiB;AACjB,gBAAgB,gEAAU;AAC1B;AACA;AACA,8BAA8B,iEAAe,GAAG,aAAa;AAC7D,iBAAiB;AACjB,aAAa;AACb;AACA,gBAAgB,sEAAgB;AAChC,4EAA4E,OAAO;AACnF,aAAa;AACb;AACA,2BAA2B,+DAAa;AACxC;AACA;AACA;AACA;AACA,SAAS;AACT;AACA,mBAAmB,kEAAkB;AACrC;AACA,SAAS;AACT;AACA;AACO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,iFAA+B;AAC3C;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACA,gBAAgB,sEAAgB;AAChC;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,oDAAU;AACtB;AACA;AACA,aAAa;AACb;AACA;AACA,gBAAgB,gEAAU;AAC1B;AACA;AACA,8BAA8B,iEAAe,GAAG,aAAa;AAC7D,iBAAiB;AACjB,aAAa;AACb;AACA,gBAAgB,sEAAgB;AAChC,gEAAgE,OAAO;AACvE,aAAa;AACb;AACA,2BAA2B,+DAAa;AACxC;AACA;AACA;AACA;AACA,SAAS;AACT;AACA,mBAAmB,kEAAkB;AACrC;AACA,SAAS;AACT;AACA;AACO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,oDAAU;AACtB;AACA,aAAa;AACb;AACA;AACA;AACA,aAAa;AACb;AACA,gBAAgB,sEAAgB;AAChC,iEAAiE,OAAO;AACxE,aAAa;AACb;AACA,2BAA2B,+DAAa;AACxC;AACA;AACA;AACA;AACA,SAAS;AACT;AACA,mBAAmB,kEAAkB;AACrC;AACA,SAAS;AACT;AACA;AACA,iEAAe,MAAM,EAAC;;;;;;;;;;;;;;;;;;;;AChZkC;AACmC;AACpD;AAChC;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACA,gBAAgB,sEAAgB;AAChC;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,oDAAU;AACtB;AACA;AACA,aAAa;AACb;AACA;AACA,gBAAgB,gEAAU;AAC1B;AACA;AACA,8BAA8B,iEAAe,GAAG,aAAa;AAC7D,iBAAiB;AACjB,aAAa;AACb;AACA,gBAAgB,sEAAgB;AAChC,wEAAwE,OAAO;AAC/E,aAAa;AACb;AACA,2BAA2B,+DAAa;AACxC;AACA;AACA;AACA;AACA,SAAS;AACT;AACA,mBAAmB,kEAAkB;AACrC;AACA,SAAS;AACT;AACA;;;;;;;;;;;;;;;;;;;;;;;AC1DmD;AAC2C;AACpE;AACa;AACqC;AAC5E,uBAAuB,eAAe,MAAM,0DAAmB,aAAa,mEAAmE;AAC/I,IAAI,0DAAmB,CAAC,2EAAoB,IAAI,sFAAsF;AACtI,uBAAuB,eAAe,MAAM,0DAAmB,aAAa,mEAAmE;AAC/I,IAAI,0DAAmB,CAAC,2EAAoB,IAAI,sFAAsF;AACtI,sBAAsB,eAAe,MAAM,0DAAmB,aAAa,mEAAmE;AAC9I,IAAI,0DAAmB,CAAC,2EAAoB,IAAI,sFAAsF;AACtI,mCAAmC,yBAAyB;AAC5D;AACA;AACA,YAAY,gEAAU;AACtB;AACA;AACA,0BAA0B,iEAAe,GAAG,aAAa;AACzD,aAAa;AACb;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,QAAQ,oDAAU;AAClB;AACA;AACA,SAAS;AACT;AACA,YAAY,gEAAU;AACtB;AACA;AACA,0BAA0B,iEAAe,GAAG,aAAa;AACzD,aAAa;AACb;AACA,SAAS;AACT;AACA,YAAY,sEAAgB;AAC5B,+DAA+D,OAAO;AACtE,SAAS;AACT;AACA;AACA;AACA,YAAY,gEAAU;AACtB;AACA;AACA,0BAA0B,iEAAe,GAAG,aAAa;AACzD,aAAa;AACb;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,QAAQ,oDAAU;AAClB;AACA;AACA,SAAS;AACT,YAAY,gEAAU;AACtB;AACA;AACA,0BAA0B,iEAAe,GAAG,aAAa;AACzD,aAAa;AACb;AACA,SAAS;AACT;AACA,YAAY,sEAAgB;AAC5B,wDAAwD,OAAO;AAC/D,SAAS;AACT;AACA,YAAY,0DAAmB,UAAU,kBAAkB;AAC3D,QAAQ,0DAAmB,gBAAgB,MAAM,gEAAS,sCAAsC;AAChG,QAAQ,0DAAmB,gBAAgB,MAAM,gEAAS,uCAAuC;AACjG,QAAQ,0DAAmB,gBAAgB,MAAM,+DAAQ,mCAAmC;AAC5F;AACA,uCAAuC,yBAAyB;AAChE;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,QAAQ,oDAAU;AAClB;AACA;AACA,SAAS;AACT,YAAY,gEAAU;AACtB;AACA;AACA,0BAA0B,iEAAe,GAAG,aAAa;AACzD,aAAa;AACb,SAAS;AACT;AACA,YAAY,sEAAgB;AAC5B,wDAAwD,OAAO;AAC/D,SAAS;AACT;AACA,YAAY,0DAAmB,eAAe,MAAM,+DAAQ,mCAAmC;AAC/F;AACO,8BAA8B,6DAAW;AAChD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,0DAAmB,4BAA4B,+DAA+D;AAC7H;AACA;AACO,6BAA6B,6DAAW;AAC/C;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,0DAAmB,gCAAgC,yDAAyD;AAC3H;AACA",
+    "file": "lib_index_js.26b2dac9fb26b92e5e77.js",
+    "mappings": ";;;;;;;;;;;;;;;;;AAA+C;AACS;AACxD;AACA;AACA;AACA;AACA;AACA;AACA;AACO,kDAAkD;AACzD;AACA,qBAAqB,+EAA6B;AAClD,uBAAuB,8DAAW;AAClC;AACA;AACA;AACA,yBAAyB,8EAA4B;AACrD;AACA;AACA,kBAAkB,+EAA6B;AAC/C;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,kBAAkB,gFAA8B;AAChD;AACA;AACA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AClCuC;AACkC;AACd;AACG;AAC9D,YAAY,OAAO;AACqC;AACmC;AACrC;AACtD;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,kEAAgB;AAC/B,eAAe,wEAAmB;AAClC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iCAAiC;AACjC;AACA,yBAAyB;AACzB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,qBAAqB;AACrB;AACA;AACA;AACA,mDAAmD,oDAAe;AAClE;AACA;AACA;AACA;AACA;AACA,sDAAsD,mDAAc;AACpE;AACA;AACA;AACA;AACA,iBAAiB;AACjB,aAAa;AACb,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA,2DAA2D,+DAAiB;AAC5E;AACA;AACA;AACO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,oDAAU;AACtB;AACA,aAAa;AACb;AACA;AACA,gBAAgB,gEAAU;AAC1B;AACA;AACA,8BAA8B,iEAAe,GAAG,aAAa;AAC7D,iBAAiB;AACjB,aAAa;AACb;AACA,gBAAgB,sEAAgB;AAChC,sEAAsE,OAAO;AAC7E,aAAa;AACb;AACA,2BAA2B,+DAAa;AACxC;AACA;AACA;AACA;AACA,SAAS;AACT;AACA,mBAAmB,kEAAkB;AACrC;AACA,SAAS;AACT;AACA;AACO;AACP;AACA;AACA,YAAY,oDAAU;AACtB;AACA,aAAa;AACb;AACA;AACA;AACA,aAAa;AACb;AACA,gBAAgB,sEAAgB;AAChC,6DAA6D,OAAO;AACpE,aAAa;AACb;AACA,2BAA2B,+DAAa;AACxC;AACA;AACA;AACA;AACA,SAAS;AACT;AACA,mBAAmB,kEAAkB;AACrC;AACA,SAAS;AACT;AACA;AACO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,iFAA+B;AAC3C,YAAY,oDAAU;AACtB;AACA,aAAa;AACb;AACA;AACA;AACA;AACA;AACA;AACA;AACA,gBAAgB,gEAAU;AAC1B;AACA;AACA,8BAA8B,iEAAe,GAAG,aAAa;AAC7D,iBAAiB;AACjB;AACA,aAAa;AACb;AACA,gBAAgB,sEAAgB;AAChC,8GAA8G,OAAO;AACrH,aAAa;AACb;AACA,2BAA2B,+DAAa;AACxC;AACA;AACA;AACA;AACA,SAAS;AACT;AACA,mBAAmB,kEAAkB;AACrC;AACA,SAAS;AACT;AACA;AACO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,iFAA+B;AAC3C,YAAY,oDAAU;AACtB;AACA,aAAa;AACb;AACA,gBAAgB,gEAAU;AAC1B;AACA;AACA,8BAA8B,iEAAe,GAAG,aAAa;AAC7D,iBAAiB;AACjB;AACA,aAAa;AACb;AACA,gBAAgB,sEAAgB;AAChC,8GAA8G,OAAO;AACrH,aAAa;AACb;AACA,2BAA2B,+DAAa;AACxC;AACA;AACA;AACA;AACA,SAAS;AACT;AACA,mBAAmB,kEAAkB;AACrC;AACA,SAAS;AACT;AACA;AACO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,iFAA+B;AAC3C;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACA,gBAAgB,sEAAgB;AAChC;AACA;AACA;AACA,gBAAgB,sEAAgB;AAChC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,oDAAU;AACtB;AACA;AACA,aAAa;AACb;AACA;AACA;AACA;AACA;AACA;AACA,iBAAiB;AACjB,gBAAgB,gEAAU;AAC1B;AACA;AACA,8BAA8B,iEAAe,GAAG,aAAa;AAC7D,iBAAiB;AACjB,aAAa;AACb;AACA,gBAAgB,sEAAgB;AAChC,4EAA4E,OAAO;AACnF,aAAa;AACb;AACA,2BAA2B,+DAAa;AACxC;AACA;AACA;AACA;AACA,SAAS;AACT;AACA,mBAAmB,kEAAkB;AACrC;AACA,SAAS;AACT;AACA;AACO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,iFAA+B;AAC3C;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACA,gBAAgB,sEAAgB;AAChC;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,oDAAU;AACtB;AACA;AACA,aAAa;AACb;AACA;AACA,gBAAgB,gEAAU;AAC1B;AACA;AACA,8BAA8B,iEAAe,GAAG,aAAa;AAC7D,iBAAiB;AACjB,aAAa;AACb;AACA,gBAAgB,sEAAgB;AAChC,gEAAgE,OAAO;AACvE,aAAa;AACb;AACA,2BAA2B,+DAAa;AACxC;AACA;AACA;AACA;AACA,SAAS;AACT;AACA,mBAAmB,kEAAkB;AACrC;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,UAAU;AACV;AACA;AACA;AACA;AACA,YAAY;AACZ;AACA;AACA;AACA,kDAAkD,OAAO;AACzD;AACA,YAAY;AACZ;AACA;AACA;AACA;AACA;AACA;AACA,QAAQ;AACR;AACA;AACA;AACA,QAAQ;AACR;AACA;AACA,iEAAe,MAAM,EAAC;;;;;;;;;;;;;;;;;;;;AChakC;AACmC;AACpD;AAChC;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACA,gBAAgB,sEAAgB;AAChC;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,oDAAU;AACtB;AACA;AACA,aAAa;AACb;AACA;AACA,gBAAgB,gEAAU;AAC1B;AACA;AACA,8BAA8B,iEAAe,GAAG,aAAa;AAC7D,iBAAiB;AACjB,aAAa;AACb;AACA,gBAAgB,sEAAgB;AAChC,wEAAwE,OAAO;AAC/E,aAAa;AACb;AACA,2BAA2B,+DAAa;AACxC;AACA;AACA;AACA;AACA,SAAS;AACT;AACA,mBAAmB,kEAAkB;AACrC;AACA,SAAS;AACT;AACA;;;;;;;;;;;;;;;;;;;;;;;AC1DmD;AAC2C;AACpE;AACa;AACqC;AAC5E,uBAAuB,eAAe,MAAM,0DAAmB,aAAa,mEAAmE;AAC/I,IAAI,0DAAmB,CAAC,2EAAoB,IAAI,sFAAsF;AACtI,uBAAuB,eAAe,MAAM,0DAAmB,aAAa,mEAAmE;AAC/I,IAAI,0DAAmB,CAAC,2EAAoB,IAAI,sFAAsF;AACtI,sBAAsB,eAAe,MAAM,0DAAmB,aAAa,mEAAmE;AAC9I,IAAI,0DAAmB,CAAC,2EAAoB,IAAI,sFAAsF;AACtI,mCAAmC,yBAAyB;AAC5D;AACA;AACA,YAAY,gEAAU;AACtB;AACA;AACA,0BAA0B,iEAAe,GAAG,aAAa;AACzD,aAAa;AACb;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,QAAQ,oDAAU;AAClB;AACA;AACA,SAAS;AACT;AACA,YAAY,gEAAU;AACtB;AACA;AACA,0BAA0B,iEAAe,GAAG,aAAa;AACzD,aAAa;AACb;AACA,SAAS;AACT;AACA,YAAY,sEAAgB;AAC5B,+DAA+D,OAAO;AACtE,SAAS;AACT;AACA;AACA;AACA,YAAY,gEAAU;AACtB;AACA;AACA,0BAA0B,iEAAe,GAAG,aAAa;AACzD,aAAa;AACb;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,QAAQ,oDAAU;AAClB;AACA;AACA,SAAS;AACT,YAAY,gEAAU;AACtB;AACA;AACA,0BAA0B,iEAAe,GAAG,aAAa;AACzD,aAAa;AACb;AACA,SAAS;AACT;AACA,YAAY,sEAAgB;AAC5B,wDAAwD,OAAO;AAC/D,SAAS;AACT;AACA,YAAY,0DAAmB,UAAU,kBAAkB;AAC3D,QAAQ,0DAAmB,gBAAgB,MAAM,gEAAS,sCAAsC;AAChG,QAAQ,0DAAmB,gBAAgB,MAAM,gEAAS,uCAAuC;AACjG,QAAQ,0DAAmB,gBAAgB,MAAM,+DAAQ,mCAAmC;AAC5F;AACA,uCAAuC,yBAAyB;AAChE;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,QAAQ,oDAAU;AAClB;AACA;AACA,SAAS;AACT,YAAY,gEAAU;AACtB;AACA;AACA,0BAA0B,iEAAe,GAAG,aAAa;AACzD,aAAa;AACb,SAAS;AACT;AACA,YAAY,sEAAgB;AAC5B,wDAAwD,OAAO;AAC/D,SAAS;AACT;AACA,YAAY,0DAAmB,eAAe,MAAM,+DAAQ,mCAAmC;AAC/F;AACO,8BAA8B,6DAAW;AAChD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,0DAAmB,4BAA4B,+DAA+D;AAC7H;AACA;AACO,6BAA6B,6DAAW;AAC/C;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,0DAAmB,gCAAgC,yDAAyD;AAC3H;AACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://carpo-teacher/./lib/handler.js",
         "webpack://carpo-teacher/./lib/index.js",
         "webpack://carpo-teacher/./lib/upload-solution.js",
         "webpack://carpo-teacher/./lib/widget.js"
     ],
     "sourcesContent": [
         "import { URLExt } from '@jupyterlab/coreutils';\nimport { ServerConnection } from '@jupyterlab/services';\n/**\n * Call the API extension\n *\n * @param endPoint API REST end point for the extension\n * @param init Initial values for the request\n * @returns The response body interpreted as JSON\n */\nexport async function requestAPI(endPoint = '', init = {}) {\n    // Make request to Jupyter API\n    const settings = ServerConnection.makeSettings();\n    const requestUrl = URLExt.join(settings.baseUrl, 'carpo-teacher', // API Namespace\n    endPoint);\n    let response;\n    try {\n        response = await ServerConnection.makeRequest(requestUrl, init, settings);\n    }\n    catch (error) {\n        throw new ServerConnection.NetworkError(error);\n    }\n    let data = await response.text();\n    if (data.length > 0) {\n        try {\n            data = JSON.parse(data);\n        }\n        catch (error) {\n            console.log('Not a JSON response body.', response);\n        }\n    }\n    if (!response.ok) {\n        throw new ServerConnection.ResponseError(response, data.message || data);\n    }\n    return data;\n}\n",
-        "import { requestAPI } from './handler';\nimport { NotebookActions, INotebookTracker } from '@jupyterlab/notebook';\nimport { CellCheckButton, FeedbackButton } from './widget';\nimport { IFileBrowserFactory } from '@jupyterlab/filebrowser';\n// import { Cell } from '@jupyterlab/cells';\nimport { DisposableDelegate } from '@lumino/disposable';\nimport { ToolbarButton, Dialog, showDialog, showErrorMessage } from '@jupyterlab/apputils';\nimport { GetSolutionButton } from './upload-solution';\n/**\n * Initialization data for the carpo-teacher extension.\n */\nconst plugin = {\n    id: 'carpo-teacher:plugin',\n    autoStart: true,\n    requires: [INotebookTracker],\n    optional: [IFileBrowserFactory],\n    activate: (app, nbTrack, browserFactory, docManager) => {\n        console.log('JupyterLab extension carpo-teacher is activated!');\n        nbTrack.currentChanged.connect(() => {\n            const notebookPanel = nbTrack.currentWidget;\n            const notebook = nbTrack.currentWidget.content;\n            // If current Notebook is not inside Exercises/problem_ directory, disable all functionality.\n            if (!nbTrack.currentWidget.context.path.includes(\"problem_\")) {\n                return;\n            }\n            notebookPanel.context.ready.then(async () => {\n                let currentCell = null;\n                let currentCellCheckButton = null;\n                nbTrack.activeCellChanged.connect(() => {\n                    if (currentCell) {\n                        notebook.widgets.map((c) => {\n                            if (c.model.type == 'code' || c.model.type == 'markdown') {\n                                const currentLayout = c.layout;\n                                currentLayout.widgets.map(w => {\n                                    if (w === currentCellCheckButton) {\n                                        currentLayout.removeWidget(w);\n                                    }\n                                });\n                            }\n                        });\n                    }\n                    const cell = notebook.activeCell;\n                    var sCell;\n                    const activeIndex = notebook.activeCellIndex;\n                    console.log(\"Active cell index: \", activeIndex);\n                    // const heading = cell.model.value.text.split(\"\\n\")[0].split(\" \")\n                    const submission_id = function (text) {\n                        return Number(text.split(\"\\n\")[0].split(\" \")[2]);\n                    };\n                    const problem_id = function (text) {\n                        return Number(text.split(\"\\n\")[0].split(\" \")[1]);\n                    };\n                    const student_id = function (text) {\n                        return Number((text.split(\"\\n\")[0].split(\" \")[0]).replace(\"#\", \"\"));\n                    };\n                    var info = {\n                        id: submission_id(cell.model.value.text),\n                        problem_id: problem_id(cell.model.value.text),\n                        student_id: student_id(cell.model.value.text),\n                        code: cell.model.value.text\n                    };\n                    var header;\n                    // For feedback case: cell is markdown so loop over the notebook widgets to get code cell before the active cell index\n                    // if (cell.model.type == 'markdown' ){\n                    //   notebook.widgets.map((c,index) =>{\n                    //     // activeIndex-1 could be the top cell (when the question type is markdown)\n                    //     if(index == activeIndex-1 && !c.model.value.text.startsWith(\"## Submission\")) {\n                    //       const code = c.model.value.text\n                    //       info.code = code  \n                    //       info.id = submission_id(code)\n                    //       info.student_id = student_id(code)\n                    //       info.problem_id = problem_id(code)\n                    //     }\n                    //   })\n                    // }\n                    // Get the status cell:\n                    notebook.widgets.map((c, index) => {\n                        if (index == activeIndex + 1) {\n                            sCell = c;\n                        }\n                    });\n                    header = cell.model.value.text.split(\"\\n\")[0];\n                    if (header.match(/^#[0-9]+ [0-9]+ [0-9]+$/)) {\n                        console.log(\"Submission Grading block.........\");\n                        const newCheckButton = new CellCheckButton(cell, sCell, info);\n                        cell.layout.addWidget(newCheckButton);\n                        currentCell = cell;\n                        currentCellCheckButton = newCheckButton;\n                    }\n                    else {\n                        const newFeedbackButton = new FeedbackButton(cell, info);\n                        cell.layout.addWidget(newFeedbackButton);\n                        currentCell = cell;\n                        currentCellCheckButton = newFeedbackButton;\n                    }\n                    // if (question.includes(\"## PID \")){\n                    //   (cell.layout as PanelLayout).addWidget(newCheckButton);\n                    //   currentCellCheckButton = newCheckButton;\n                    // }\n                    // Set the current cell and button for future\n                    // reference\n                });\n            });\n        });\n        //  tell the document registry about your widget extension:\n        app.docRegistry.addWidgetExtension('Notebook', new RegisterButton());\n        app.docRegistry.addWidgetExtension('Notebook', new NewSubmissionButtonExtension());\n        app.docRegistry.addWidgetExtension('Notebook', new AllSubmissionButtonExtension());\n        app.docRegistry.addWidgetExtension('Notebook', new PublishProblemButtonExtension());\n        app.docRegistry.addWidgetExtension('Notebook', new ArchiveProblemButtonExtension());\n        app.docRegistry.addWidgetExtension('Notebook', new GetSolutionButton());\n        app.docRegistry.addWidgetExtension('Notebook', new viewProblemStatusExtension());\n    }\n};\nexport class RegisterButton {\n    /**\n     * Create a new extension for the notebook panel widget.\n     *\n     * @param panel Notebook panel\n     * @param context Notebook context\n     * @returns Disposable on the added button\n     */\n    createNew(panel, context) {\n        const register = () => {\n            requestAPI('register', {\n                method: 'GET'\n            })\n                .then(data => {\n                console.log(data);\n                showDialog({\n                    title: '',\n                    body: \"Teacher \" + data.name + \" has been registered.\",\n                    buttons: [Dialog.okButton({ label: 'Ok' })]\n                });\n            })\n                .catch(reason => {\n                showErrorMessage('Registration Error', reason);\n                console.error(`Failed to register user as Teacher.\\n${reason}`);\n            });\n        };\n        const button = new ToolbarButton({\n            className: 'register-button',\n            label: 'Register',\n            onClick: register,\n            tooltip: 'Register as a Teacher',\n        });\n        panel.toolbar.insertItem(10, 'register', button);\n        return new DisposableDelegate(() => {\n            button.dispose();\n        });\n    }\n}\nexport class NewSubmissionButtonExtension {\n    /**\n     * Create a new extension for the notebook panel widget.\n     *\n     * @param panel Notebook panel\n     * @param context Notebook context\n     * @returns Disposable on the added button\n     */\n    createNew(panel, context) {\n        const getSubmissions = () => {\n            NotebookActions.clearAllOutputs(panel.content);\n            requestAPI('submissions', {\n                method: 'GET'\n            })\n                .then(data => {\n                if (data.Remaining != 0) {\n                    var msg = \"Notebook \" + data.sub_file + \" is placed in folder Problem_\" + data.question + \". There are \" + data.remaining + \" submissions in the queue.\";\n                }\n                else {\n                    var msg = \"You have got 0 submissions. Please check again later.\\n\";\n                }\n                showDialog({\n                    title: 'Submission Status',\n                    body: msg,\n                    buttons: [Dialog.okButton({ label: 'Ok' })]\n                });\n                console.log(data);\n            })\n                .catch(reason => {\n                showErrorMessage('Get Student Code Error', reason);\n                console.error(`Failed to get student's code from the server. Please check your connection.\\n${reason}`);\n            });\n        };\n        const button = new ToolbarButton({\n            className: 'sync-code-button',\n            label: 'GetSubs',\n            onClick: getSubmissions,\n            tooltip: 'Download new submissions from students.',\n        });\n        panel.toolbar.insertItem(11, 'getStudentsCode', button);\n        return new DisposableDelegate(() => {\n            button.dispose();\n        });\n    }\n}\nexport class AllSubmissionButtonExtension {\n    /**\n     * Create a new extension for the notebook panel widget.\n     *\n     * @param panel Notebook panel\n     * @param context Notebook context\n     * @returns Disposable on the added button\n     */\n    createNew(panel, context) {\n        const getGradedSubmissions = () => {\n            NotebookActions.clearAllOutputs(panel.content);\n            requestAPI('graded_submissions', {\n                method: 'GET'\n            })\n                .then(data => {\n                showDialog({\n                    title: '',\n                    body: data.msg,\n                    buttons: [Dialog.okButton({ label: 'Ok' })]\n                });\n                console.log(data);\n            })\n                .catch(reason => {\n                showErrorMessage('Get Graded Submissions Error', reason);\n                console.error(`Failed to get student's code from the server. Please check your connection.\\n${reason}`);\n            });\n        };\n        const button = new ToolbarButton({\n            className: 'sync-code-button',\n            label: 'Graded',\n            onClick: getGradedSubmissions,\n            tooltip: 'Get all graded submissions.',\n        });\n        panel.toolbar.insertItem(12, 'getAllGradedSubmissions', button);\n        return new DisposableDelegate(() => {\n            button.dispose();\n        });\n    }\n}\nexport class PublishProblemButtonExtension {\n    /**\n     * Create a new extension for the notebook panel widget.\n     *\n     * @param panel Notebook panel\n     * @param context Notebook context\n     * @returns Disposable on the added button\n     */\n    createNew(panel, context) {\n        const publishProblem = () => {\n            NotebookActions.clearAllOutputs(panel.content);\n            const notebook = panel.content;\n            const activeIndex = notebook.activeCellIndex;\n            var problem;\n            var format;\n            var header;\n            var time_limit;\n            notebook.widgets.map((c, index) => {\n                if (index === activeIndex) {\n                    problem = c.model.value.text;\n                    format = c.model.type;\n                }\n            });\n            if (problem.includes(\"#PID:\")) {\n                showErrorMessage('Publish Question Error', \"Problem already published.\");\n                return;\n            }\n            if (!problem) {\n                showErrorMessage('Publish Question Error', \"Problem is empty.\");\n                return;\n            }\n            header = problem.split('\\n')[0];\n            if (header.match(/[0-9]+[a-zA-Z]/)) {\n                time_limit = header.match(/[0-9]+[a-zA-Z]/)[0];\n            }\n            let postBody = {\n                \"question\": problem,\n                \"format\": format,\n                \"time_limit\": time_limit\n            };\n            requestAPI('problem', {\n                method: 'POST',\n                body: JSON.stringify(postBody)\n            })\n                .then(data => {\n                console.log(data);\n                notebook.widgets.map((c, index) => {\n                    if (index === activeIndex) {\n                        c.model.value.text = \"#PID:\" + data.id + \"\\n\" + problem;\n                    }\n                });\n                showDialog({\n                    title: 'New Questions Published',\n                    body: 'Problem ' + data.id + \" is published.\",\n                    buttons: [Dialog.okButton({ label: 'Ok' })]\n                });\n            })\n                .catch(reason => {\n                showErrorMessage('Publish Question Error', reason);\n                console.error(`Failed to publish question to the server.\\n${reason}`);\n            });\n        };\n        const button = new ToolbarButton({\n            className: 'publish-problem-button',\n            label: 'Publish',\n            onClick: publishProblem,\n            tooltip: 'Publish New Problem.',\n        });\n        panel.toolbar.insertItem(13, 'publishNewProblem', button);\n        return new DisposableDelegate(() => {\n            button.dispose();\n        });\n    }\n}\nexport class ArchiveProblemButtonExtension {\n    /**\n     * Create a new extension for the notebook panel widget.\n     *\n     * @param panel Notebook panel\n     * @param context Notebook context\n     * @returns Disposable on the added button\n     */\n    createNew(panel, context) {\n        const archiveProblem = () => {\n            NotebookActions.clearAllOutputs(panel.content);\n            const notebook = panel.content;\n            const activeIndex = notebook.activeCellIndex;\n            var problem;\n            notebook.widgets.map((c, index) => {\n                if (index === activeIndex) {\n                    problem = c.model.value.text;\n                }\n            });\n            if (!problem.includes(\"#PID:\")) {\n                showErrorMessage('Unpublish Question Error', \"Active problem not found.\");\n                return;\n            }\n            var problem_id = parseInt((problem.split(\"\\n\")[0]).split(\"#PID:\")[1]);\n            let body = {\n                \"problem_id\": problem_id\n            };\n            requestAPI('problem', {\n                method: 'DELETE',\n                body: JSON.stringify(body)\n            })\n                .then(data => {\n                console.log(data);\n                showDialog({\n                    title: 'Question Unpublished',\n                    body: 'Problem id ' + problem_id + ' is  unpublished.',\n                    buttons: [Dialog.okButton({ label: 'Ok' })]\n                });\n            })\n                .catch(reason => {\n                showErrorMessage('Unpublish Question Error', reason);\n                console.error(`Failed to unpublish question.\\n${reason}`);\n            });\n        };\n        const button = new ToolbarButton({\n            className: 'archive-problem-button',\n            label: 'Unpublish',\n            onClick: archiveProblem,\n            tooltip: 'Unpublish the problem.',\n        });\n        panel.toolbar.insertItem(14, 'archivesProblem', button);\n        return new DisposableDelegate(() => {\n            button.dispose();\n        });\n    }\n}\nexport class viewProblemStatusExtension {\n    /**\n     * Create a new extension for the notebook panel widget.\n     *\n     * @param panel Notebook panel\n     * @param context Notebook context\n     * @returns Disposable on the added button\n     */\n    createNew(panel, context) {\n        const viewProblemStatus = () => {\n            requestAPI('view_problem_list', {\n                method: 'GET'\n            })\n                .then(data => {\n                console.log(data);\n                window.open(data.url, \"_blank\");\n            })\n                .catch(reason => {\n                showErrorMessage('View Problem Status Error', reason);\n                console.error(`Failed to view problem status.\\n${reason}`);\n            });\n        };\n        const button = new ToolbarButton({\n            className: 'get-status-button',\n            label: 'Problems',\n            onClick: viewProblemStatus,\n            tooltip: 'View all problem status',\n        });\n        panel.toolbar.insertItem(16, 'viewProblemStatus', button);\n        return new DisposableDelegate(() => {\n            button.dispose();\n        });\n    }\n}\nexport default plugin;\n",
-        "import { DisposableDelegate } from '@lumino/disposable';\nimport { ToolbarButton, Dialog, showDialog, showErrorMessage } from '@jupyterlab/apputils';\nimport { requestAPI } from './handler';\nexport class GetSolutionButton {\n    /**\n     * Create a new extension for the notebook panel widget.\n     *\n     * @param panel Notebook panel\n     * @param context Notebook context\n     * @returns Disposable on the added button\n     */\n    createNew(panel, context) {\n        const uploadSolution = () => {\n            const notebook = panel.content;\n            const activeIndex = notebook.activeCellIndex;\n            var code_block;\n            notebook.widgets.map((c, index) => {\n                if (index === activeIndex) {\n                    code_block = c.model.value.text;\n                }\n            });\n            if (!code_block.includes(\"#PID:\")) {\n                showErrorMessage('Upload Solution Error', \"Active problem not found.\");\n                return;\n            }\n            var problem_id = parseInt((code_block.split(\"\\n\")[0]).split(\"#PID:\")[1]);\n            let body = {\n                \"problem_id\": problem_id,\n                \"code\": code_block\n            };\n            requestAPI('solution', {\n                method: 'POST',\n                body: JSON.stringify(body)\n            })\n                .then(data => {\n                console.log(data);\n                showDialog({\n                    title: 'Solution Uploaded',\n                    body: 'Solution uploaded for ProblemID ' + problem_id + '.',\n                    buttons: [Dialog.okButton({ label: 'Ok' })]\n                });\n            })\n                .catch(reason => {\n                showErrorMessage('Upload Solution Error', reason);\n                console.error(`Failed to upload solution to problem.\\n${reason}`);\n            });\n        };\n        const button = new ToolbarButton({\n            className: 'upload-solution-button',\n            label: 'UploadSolution',\n            onClick: uploadSolution,\n            tooltip: 'Upload solutions to the problem.',\n        });\n        panel.toolbar.insertItem(15, 'getSolutions', button);\n        return new DisposableDelegate(() => {\n            button.dispose();\n        });\n    }\n}\n",
+        "import { requestAPI } from './handler';\nimport { NotebookActions, INotebookTracker } from '@jupyterlab/notebook';\nimport { CellCheckButton, FeedbackButton } from './widget';\nimport { IFileBrowserFactory } from '@jupyterlab/filebrowser';\n// import { Cell } from '@jupyterlab/cells';\nimport { DisposableDelegate } from '@lumino/disposable';\nimport { ToolbarButton, Dialog, showDialog, showErrorMessage } from '@jupyterlab/apputils';\nimport { GetSolutionButton } from './upload-solution';\n/**\n * Initialization data for the carpo-teacher extension.\n */\nconst plugin = {\n    id: 'carpo-teacher:plugin',\n    autoStart: true,\n    requires: [INotebookTracker],\n    optional: [IFileBrowserFactory],\n    activate: (app, nbTrack, browserFactory, docManager) => {\n        console.log('JupyterLab extension carpo-teacher is activated!');\n        nbTrack.currentChanged.connect(() => {\n            const notebookPanel = nbTrack.currentWidget;\n            const notebook = nbTrack.currentWidget.content;\n            // If current Notebook is not inside Exercises/problem_ directory, disable all functionality.\n            if (!nbTrack.currentWidget.context.path.includes(\"problem_\")) {\n                return;\n            }\n            notebookPanel.context.ready.then(async () => {\n                let currentCell = null;\n                let currentCellCheckButton = null;\n                nbTrack.activeCellChanged.connect(() => {\n                    if (currentCell) {\n                        notebook.widgets.map((c) => {\n                            if (c.model.type == 'code' || c.model.type == 'markdown') {\n                                const currentLayout = c.layout;\n                                currentLayout.widgets.map(w => {\n                                    if (w === currentCellCheckButton) {\n                                        currentLayout.removeWidget(w);\n                                    }\n                                });\n                            }\n                        });\n                    }\n                    const cell = notebook.activeCell;\n                    var sCell;\n                    const activeIndex = notebook.activeCellIndex;\n                    // const heading = cell.model.value.text.split(\"\\n\")[0].split(\" \")\n                    const submission_id = function (text) {\n                        return Number(text.split(\"\\n\")[0].split(\" \")[2]);\n                    };\n                    const problem_id = function (text) {\n                        return Number(text.split(\"\\n\")[0].split(\" \")[1]);\n                    };\n                    const student_id = function (text) {\n                        return Number((text.split(\"\\n\")[0].split(\" \")[0]).replace(\"#\", \"\"));\n                    };\n                    var info = {\n                        id: submission_id(cell.model.value.text),\n                        problem_id: problem_id(cell.model.value.text),\n                        student_id: student_id(cell.model.value.text),\n                        code: cell.model.value.text\n                    };\n                    var header;\n                    // Get the status cell:\n                    notebook.widgets.map((c, index) => {\n                        if (index == activeIndex + 1) {\n                            sCell = c;\n                        }\n                    });\n                    header = cell.model.value.text.split(\"\\n\")[0];\n                    if (header.match(/^#[0-9]+ [0-9]+ [0-9]+$/)) {\n                        console.log(\"Submission Grading block.........\");\n                        const newCheckButton = new CellCheckButton(cell, sCell, info);\n                        cell.layout.addWidget(newCheckButton);\n                        currentCell = cell;\n                        currentCellCheckButton = newCheckButton;\n                    }\n                    else {\n                        const newFeedbackButton = new FeedbackButton(cell, info);\n                        cell.layout.addWidget(newFeedbackButton);\n                        currentCell = cell;\n                        currentCellCheckButton = newFeedbackButton;\n                    }\n                });\n            });\n        });\n        //  tell the document registry about your widget extension:\n        app.docRegistry.addWidgetExtension('Notebook', new RegisterButton());\n        app.docRegistry.addWidgetExtension('Notebook', new GoToApp());\n        // app.docRegistry.addWidgetExtension('Notebook', new NewSubmissionButtonExtension());\n        // app.docRegistry.addWidgetExtension('Notebook', new AllSubmissionButtonExtension());\n        app.docRegistry.addWidgetExtension('Notebook', new PublishProblemButtonExtension());\n        app.docRegistry.addWidgetExtension('Notebook', new ArchiveProblemButtonExtension());\n        app.docRegistry.addWidgetExtension('Notebook', new GetSolutionButton());\n        // app.docRegistry.addWidgetExtension('Notebook', new viewProblemStatusExtension());\n    }\n};\nexport class RegisterButton {\n    /**\n     * Create a new extension for the notebook panel widget.\n     *\n     * @param panel Notebook panel\n     * @param context Notebook context\n     * @returns Disposable on the added button\n     */\n    createNew(panel, context) {\n        const register = () => {\n            requestAPI('register', {\n                method: 'GET'\n            })\n                .then(data => {\n                console.log(data);\n                showDialog({\n                    title: '',\n                    body: \"Teacher \" + data.name + \" has been registered.\",\n                    buttons: [Dialog.okButton({ label: 'Ok' })]\n                });\n            })\n                .catch(reason => {\n                showErrorMessage('Registration Error', reason);\n                console.error(`Failed to register user as Teacher.\\n${reason}`);\n            });\n        };\n        const button = new ToolbarButton({\n            className: 'register-button',\n            label: 'Register',\n            onClick: register,\n            tooltip: 'Register as a Teacher',\n        });\n        panel.toolbar.insertItem(10, 'register', button);\n        return new DisposableDelegate(() => {\n            button.dispose();\n        });\n    }\n}\nexport class GoToApp {\n    createNew(panel, context) {\n        const viewWebApp = () => {\n            requestAPI('view_app', {\n                method: 'GET'\n            })\n                .then(data => {\n                // console.log(data);\n                window.open(data.url, \"_blank\");\n            })\n                .catch(reason => {\n                showErrorMessage('View App Status Error', reason);\n                console.error(`Failed to view app status.\\n${reason}`);\n            });\n        };\n        const button = new ToolbarButton({\n            className: 'get-app-button',\n            label: 'App',\n            onClick: viewWebApp,\n            tooltip: 'Go to the web app',\n        });\n        panel.toolbar.insertItem(11, 'viewWebApp', button);\n        return new DisposableDelegate(() => {\n            button.dispose();\n        });\n    }\n}\nexport class NewSubmissionButtonExtension {\n    /**\n     * Create a new extension for the notebook panel widget.\n     *\n     * @param panel Notebook panel\n     * @param context Notebook context\n     * @returns Disposable on the added button\n     */\n    createNew(panel, context) {\n        const getSubmissions = () => {\n            NotebookActions.clearAllOutputs(panel.content);\n            requestAPI('submissions', {\n                method: 'GET'\n            })\n                .then(data => {\n                if (data.Remaining != 0) {\n                    var msg = \"Notebook \" + data.sub_file + \" is placed in folder Problem_\" + data.question + \". There are \" + data.remaining + \" submissions in the queue.\";\n                }\n                else {\n                    var msg = \"You have got 0 submissions. Please check again later.\\n\";\n                }\n                showDialog({\n                    title: 'Submission Status',\n                    body: msg,\n                    buttons: [Dialog.okButton({ label: 'Ok' })]\n                });\n                console.log(data);\n            })\n                .catch(reason => {\n                showErrorMessage('Get Student Code Error', reason);\n                console.error(`Failed to get student's code from the server. Please check your connection.\\n${reason}`);\n            });\n        };\n        const button = new ToolbarButton({\n            className: 'sync-code-button',\n            label: 'GetSubs',\n            onClick: getSubmissions,\n            tooltip: 'Download new submissions from students.',\n        });\n        panel.toolbar.insertItem(11, 'getStudentsCode', button);\n        return new DisposableDelegate(() => {\n            button.dispose();\n        });\n    }\n}\nexport class AllSubmissionButtonExtension {\n    /**\n     * Create a new extension for the notebook panel widget.\n     *\n     * @param panel Notebook panel\n     * @param context Notebook context\n     * @returns Disposable on the added button\n     */\n    createNew(panel, context) {\n        const getGradedSubmissions = () => {\n            NotebookActions.clearAllOutputs(panel.content);\n            requestAPI('graded_submissions', {\n                method: 'GET'\n            })\n                .then(data => {\n                showDialog({\n                    title: '',\n                    body: data.msg,\n                    buttons: [Dialog.okButton({ label: 'Ok' })]\n                });\n                console.log(data);\n            })\n                .catch(reason => {\n                showErrorMessage('Get Graded Submissions Error', reason);\n                console.error(`Failed to get student's code from the server. Please check your connection.\\n${reason}`);\n            });\n        };\n        const button = new ToolbarButton({\n            className: 'sync-code-button',\n            label: 'Graded',\n            onClick: getGradedSubmissions,\n            tooltip: 'Get all graded submissions.',\n        });\n        panel.toolbar.insertItem(12, 'getAllGradedSubmissions', button);\n        return new DisposableDelegate(() => {\n            button.dispose();\n        });\n    }\n}\nexport class PublishProblemButtonExtension {\n    /**\n     * Create a new extension for the notebook panel widget.\n     *\n     * @param panel Notebook panel\n     * @param context Notebook context\n     * @returns Disposable on the added button\n     */\n    createNew(panel, context) {\n        const publishProblem = () => {\n            NotebookActions.clearAllOutputs(panel.content);\n            const notebook = panel.content;\n            const activeIndex = notebook.activeCellIndex;\n            var problem;\n            var format;\n            var header;\n            var time_limit;\n            notebook.widgets.map((c, index) => {\n                if (index === activeIndex) {\n                    problem = c.model.value.text;\n                    format = c.model.type;\n                }\n            });\n            if (problem.includes(\"#PID:\")) {\n                showErrorMessage('Publish Question Error', \"Problem already published.\");\n                return;\n            }\n            if (!problem) {\n                showErrorMessage('Publish Question Error', \"Problem is empty.\");\n                return;\n            }\n            header = problem.split('\\n')[0];\n            if (header.match(/[0-9]+[a-zA-Z]/)) {\n                time_limit = header.match(/[0-9]+[a-zA-Z]/)[0];\n            }\n            let postBody = {\n                \"question\": problem,\n                \"format\": format,\n                \"time_limit\": time_limit\n            };\n            requestAPI('problem', {\n                method: 'POST',\n                body: JSON.stringify(postBody)\n            })\n                .then(data => {\n                console.log(data);\n                notebook.widgets.map((c, index) => {\n                    if (index === activeIndex) {\n                        c.model.value.text = \"#PID:\" + data.id + \"\\n\" + problem;\n                    }\n                });\n                showDialog({\n                    title: 'New Questions Published',\n                    body: 'Problem ' + data.id + \" is published.\",\n                    buttons: [Dialog.okButton({ label: 'Ok' })]\n                });\n            })\n                .catch(reason => {\n                showErrorMessage('Publish Question Error', reason);\n                console.error(`Failed to publish question to the server.\\n${reason}`);\n            });\n        };\n        const button = new ToolbarButton({\n            className: 'publish-problem-button',\n            label: 'Publish',\n            onClick: publishProblem,\n            tooltip: 'Publish New Problem.',\n        });\n        panel.toolbar.insertItem(12, 'publishNewProblem', button);\n        return new DisposableDelegate(() => {\n            button.dispose();\n        });\n    }\n}\nexport class ArchiveProblemButtonExtension {\n    /**\n     * Create a new extension for the notebook panel widget.\n     *\n     * @param panel Notebook panel\n     * @param context Notebook context\n     * @returns Disposable on the added button\n     */\n    createNew(panel, context) {\n        const archiveProblem = () => {\n            NotebookActions.clearAllOutputs(panel.content);\n            const notebook = panel.content;\n            const activeIndex = notebook.activeCellIndex;\n            var problem;\n            notebook.widgets.map((c, index) => {\n                if (index === activeIndex) {\n                    problem = c.model.value.text;\n                }\n            });\n            if (!problem.includes(\"#PID:\")) {\n                showErrorMessage('Unpublish Question Error', \"Active problem not found.\");\n                return;\n            }\n            var problem_id = parseInt((problem.split(\"\\n\")[0]).split(\"#PID:\")[1]);\n            let body = {\n                \"problem_id\": problem_id\n            };\n            requestAPI('problem', {\n                method: 'DELETE',\n                body: JSON.stringify(body)\n            })\n                .then(data => {\n                console.log(data);\n                showDialog({\n                    title: 'Question Unpublished',\n                    body: 'Problem id ' + problem_id + ' is  unpublished.',\n                    buttons: [Dialog.okButton({ label: 'Ok' })]\n                });\n            })\n                .catch(reason => {\n                showErrorMessage('Unpublish Question Error', reason);\n                console.error(`Failed to unpublish question.\\n${reason}`);\n            });\n        };\n        const button = new ToolbarButton({\n            className: 'archive-problem-button',\n            label: 'Unpublish',\n            onClick: archiveProblem,\n            tooltip: 'Unpublish the problem.',\n        });\n        panel.toolbar.insertItem(13, 'archivesProblem', button);\n        return new DisposableDelegate(() => {\n            button.dispose();\n        });\n    }\n}\n// export class viewProblemStatusExtension\n//   implements DocumentRegistry.IWidgetExtension<NotebookPanel, INotebookModel>\n// {\n//   /**\n//    * Create a new extension for the notebook panel widget.\n//    *\n//    * @param panel Notebook panel\n//    * @param context Notebook context\n//    * @returns Disposable on the added button\n//    */\n//   createNew(\n//     panel: NotebookPanel,\n//     context: DocumentRegistry.IContext<INotebookModel>\n//   ): IDisposable {\n//     const viewProblemStatus = () => {\n//       requestAPI<any>('view_problem_list',{\n//         method: 'GET'\n//       })\n//         .then(data => {\n//           console.log(data);\n//           window.open(\n//             data.url, \"_blank\");\n//         })\n//         .catch(reason => {\n//           showErrorMessage('View Problem Status Error', reason);\n//           console.error(\n//             `Failed to view problem status.\\n${reason}`\n//           );\n//         });\n//     };\n//     const button = new ToolbarButton({\n//       className: 'get-status-button',\n//       label: 'Problems',\n//       onClick: viewProblemStatus,\n//       tooltip: 'View all problem status',\n//     });\n//     panel.toolbar.insertItem(15, 'viewProblemStatus', button);\n//     return new DisposableDelegate(() => {\n//       button.dispose();\n//     });\n//   }\n// }\nexport default plugin;\n",
+        "import { DisposableDelegate } from '@lumino/disposable';\nimport { ToolbarButton, Dialog, showDialog, showErrorMessage } from '@jupyterlab/apputils';\nimport { requestAPI } from './handler';\nexport class GetSolutionButton {\n    /**\n     * Create a new extension for the notebook panel widget.\n     *\n     * @param panel Notebook panel\n     * @param context Notebook context\n     * @returns Disposable on the added button\n     */\n    createNew(panel, context) {\n        const uploadSolution = () => {\n            const notebook = panel.content;\n            const activeIndex = notebook.activeCellIndex;\n            var code_block;\n            notebook.widgets.map((c, index) => {\n                if (index === activeIndex) {\n                    code_block = c.model.value.text;\n                }\n            });\n            if (!code_block.includes(\"#PID:\")) {\n                showErrorMessage('Upload Solution Error', \"Active problem not found.\");\n                return;\n            }\n            var problem_id = parseInt((code_block.split(\"\\n\")[0]).split(\"#PID:\")[1]);\n            let body = {\n                \"problem_id\": problem_id,\n                \"code\": code_block\n            };\n            requestAPI('solution', {\n                method: 'POST',\n                body: JSON.stringify(body)\n            })\n                .then(data => {\n                console.log(data);\n                showDialog({\n                    title: 'Solution Uploaded',\n                    body: 'Solution uploaded for ProblemID ' + problem_id + '.',\n                    buttons: [Dialog.okButton({ label: 'Ok' })]\n                });\n            })\n                .catch(reason => {\n                showErrorMessage('Upload Solution Error', reason);\n                console.error(`Failed to upload solution to problem.\\n${reason}`);\n            });\n        };\n        const button = new ToolbarButton({\n            className: 'upload-solution-button',\n            label: 'UploadSolution',\n            onClick: uploadSolution,\n            tooltip: 'Upload solutions to the problem.',\n        });\n        panel.toolbar.insertItem(14, 'getSolutions', button);\n        return new DisposableDelegate(() => {\n            button.dispose();\n        });\n    }\n}\n",
         "import { ReactWidget } from '@jupyterlab/apputils';\nimport { checkIcon, closeIcon, LabIcon, saveIcon, redoIcon } from '@jupyterlab/ui-components';\nimport React from 'react';\nimport { requestAPI } from './handler';\nimport { Dialog, showDialog, showErrorMessage } from '@jupyterlab/apputils';\nconst GradeButton = ({ icon, onClick }) => (React.createElement(\"button\", { type: \"button\", onClick: () => onClick(), className: \"cellButton\" },\n    React.createElement(LabIcon.resolveReact, { icon: icon, className: \"cellButton-icon\", tag: \"span\", width: \"15px\", height: \"15px\" })));\nconst ResetButton = ({ icon, onClick }) => (React.createElement(\"button\", { type: \"button\", onClick: () => onClick(), className: \"cellButton\" },\n    React.createElement(LabIcon.resolveReact, { icon: icon, className: \"cellButton-icon\", tag: \"span\", width: \"15px\", height: \"15px\" })));\nconst SendButton = ({ icon, onClick }) => (React.createElement(\"button\", { type: \"button\", onClick: () => onClick(), className: \"cellButton\" },\n    React.createElement(LabIcon.resolveReact, { icon: icon, className: \"cellButton-icon\", tag: \"span\", width: \"15px\", height: \"15px\" })));\nconst CodeCellButtonComponent = ({ cell, statusCell, info, }) => {\n    const submitGrade = async (val) => {\n        if (info.id == NaN) {\n            showDialog({\n                title: 'Grading Error',\n                body: \"Invalid Cell for grading.\",\n                buttons: [Dialog.okButton({ label: 'Ok' })]\n            });\n            return;\n        }\n        let postBody = {\n            \"student_id\": info.student_id,\n            \"submission_id\": info.id,\n            \"problem_id\": info.problem_id,\n            \"score\": val ? 1 : 2,\n            \"code\": cell.model.value.text\n        };\n        var status = val ? \"Correct.\" : \"Incorrect.\";\n        // console.log(\"Grade: \", postBody)\n        requestAPI('submissions/grade', {\n            method: 'POST',\n            body: JSON.stringify(postBody)\n        }).then(data => {\n            var msg = \"This submission is now graded as \" + status;\n            showDialog({\n                title: 'Grading Status',\n                body: msg,\n                buttons: [Dialog.okButton({ label: 'Ok' })]\n            });\n            statusCell.model.value.text = \"### Status: \" + status;\n        })\n            .catch(reason => {\n            showErrorMessage('Submission Grade Error', reason);\n            console.error(`Failed to grade the submission. \\n${reason}`);\n        });\n    };\n    const sendFeedback = async () => {\n        if (info.id == NaN) {\n            showDialog({\n                title: 'Feedback Error',\n                body: \"Invalid Cell for feedback.\",\n                buttons: [Dialog.okButton({ label: 'Ok' })]\n            });\n            return;\n        }\n        let postBody = {\n            \"student_id\": info.student_id,\n            \"submission_id\": info.id,\n            \"problem_id\": info.problem_id,\n            \"code\": cell.model.value.text\n        };\n        requestAPI('submissions/feedbacks', {\n            method: 'POST',\n            body: JSON.stringify(postBody)\n        }).then(data => {\n            showDialog({\n                title: 'Feedback Status',\n                body: data.msg,\n                buttons: [Dialog.okButton({ label: 'Ok' })]\n            });\n            statusCell.model.value.text = \"### Status: Try Again\";\n        })\n            .catch(reason => {\n            showErrorMessage('Feedback Send Error', reason);\n            console.error(`Failed to save feedback. \\n${reason}`);\n        });\n    };\n    return (React.createElement(\"div\", { className: 'grp' },\n        React.createElement(GradeButton, { icon: checkIcon, onClick: () => (submitGrade)(true) }),\n        React.createElement(GradeButton, { icon: closeIcon, onClick: () => (submitGrade)(false) }),\n        React.createElement(ResetButton, { icon: redoIcon, onClick: () => (sendFeedback)() })));\n};\nconst MarkdownCellButtonComponent = ({ cell, statusCell, info, }) => {\n    const sendFeedback = async () => {\n        let postBody = {\n            \"student_id\": info.student_id,\n            \"submission_id\": info.id,\n            \"problem_id\": info.problem_id,\n            \"code\": info.code,\n            \"message\": info.message,\n            \"comment\": cell.model.value.text\n        };\n        // console.log(\"Feedback: \", postBody)\n        requestAPI('submissions/feedbacks', {\n            method: 'POST',\n            body: JSON.stringify(postBody)\n        }).then(data => {\n            showDialog({\n                title: 'Feedback Status',\n                body: \"Feedback is sent to the student.\",\n                buttons: [Dialog.okButton({ label: 'Ok' })]\n            });\n        })\n            .catch(reason => {\n            showErrorMessage('Feedback Send Error', reason);\n            console.error(`Failed to save feedback. \\n${reason}`);\n        });\n    };\n    return (React.createElement(SendButton, { icon: saveIcon, onClick: () => (sendFeedback)() }));\n};\nexport class CellCheckButton extends ReactWidget {\n    constructor(cell, statusCell, info) {\n        super();\n        this.cell = null;\n        this.statusCell = null;\n        this.info = null;\n        this.cell = cell;\n        this.statusCell = statusCell;\n        this.info = info;\n        this.addClass('jp-grpCellButton');\n    }\n    render() {\n        return React.createElement(CodeCellButtonComponent, { cell: this.cell, statusCell: this.statusCell, info: this.info });\n    }\n}\nexport class FeedbackButton extends ReactWidget {\n    constructor(cell, info) {\n        super();\n        this.cell = null;\n        this.statusCell = null;\n        this.info = null;\n        this.cell = cell;\n        this.info = info;\n        this.addClass('jp-CellButton');\n    }\n    render() {\n        return React.createElement(MarkdownCellButtonComponent, { cell: this.cell, statusCell: this.cell, info: this.info });\n    }\n}\n"
     ],
     "version": 3
 }
```

### Comparing `carpo_teacher-0.0.7/carpo_teacher/labextension/static/remoteEntry.d6f902fe01b1dc4f6fba.js` & `carpo_teacher-0.0.9/carpo_teacher/labextension/static/remoteEntry.991b8dc2b6efb319125a.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -182,15 +182,15 @@
     (() => {
         /******/ // This function allow to reference async chunks
         /******/
         __webpack_require__.u = (chunkId) => {
             /******/ // return url for filenames based on template
             /******/
             return "" + chunkId + "." + {
-                "lib_index_js": "63bb1f0b3e113fb2d1b6",
+                "lib_index_js": "26b2dac9fb26b92e5e77",
                 "vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1": "6760bbd0c725e3542c7a",
                 "style_index_js": "fc6324d8ef291b0fdd9a"
             } [chunkId] + ".js";
             /******/
         };
         /******/
     })();
@@ -425,15 +425,15 @@
             /******/
             var promises = [];
             /******/
             switch (name) {
                 /******/
                 case "default": {
                     /******/
-                    register("carpo-teacher", "0.0.6", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
+                    register("carpo-teacher", "0.0.7", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
                     /******/
                 }
                 /******/
                 break;
                 /******/
             }
             /******/
@@ -1077,8 +1077,8 @@
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/carpo-teacher");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB)["carpo-teacher"] = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.d6f902fe01b1dc4f6fba.js.map
+//# sourceMappingURL=remoteEntry.991b8dc2b6efb319125a.js.map
```

### Comparing `carpo_teacher-0.0.7/carpo_teacher/labextension/static/remoteEntry.d6f902fe01b1dc4f6fba.js.map` & `carpo_teacher-0.0.9/carpo_teacher/labextension/static/remoteEntry.991b8dc2b6efb319125a.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9135338345864661%*

 * *Differences: {"'file'": "'remoteEntry.991b8dc2b6efb319125a.js'",*

 * * "'sourcesContent'": "{insert: [(5, '// This function allow to reference async "*

 * *                     'chunks\\n__webpack_require__.u = (chunkId) => {\\n\\t// return url for '*

 * *                     'filenames based on template\\n\\treturn "" + chunkId + "." + '*

 * *                     '{"lib_index_js":"26b2dac9fb26b92e5e77","vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1":"6760bbd0c725e3542c7a","style_index […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "remoteEntry.d6f902fe01b1dc4f6fba.js",
+    "file": "remoteEntry.991b8dc2b6efb319125a.js",
     "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,4MAA4M;WAC1O;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC3CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WCfA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WCrLA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;UErFA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://carpo-teacher/webpack/container-entry",
         "webpack://carpo-teacher/webpack/bootstrap",
         "webpack://carpo-teacher/webpack/runtime/compat get default export",
@@ -24,20 +24,20 @@
     ],
     "sourcesContent": [
         "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./style\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"style_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./style/index.js */ \"./style/index.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId](module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"63bb1f0b3e113fb2d1b6\",\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\":\"6760bbd0c725e3542c7a\",\"style_index_js\":\"fc6324d8ef291b0fdd9a\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"26b2dac9fb26b92e5e77\",\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\":\"6760bbd0c725e3542c7a\",\"style_index_js\":\"fc6324d8ef291b0fdd9a\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"carpo-teacher:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\t;\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"carpo-teacher\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"carpo-teacher\", \"0.0.6\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"carpo-teacher\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"carpo-teacher\", \"0.0.7\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) scriptUrl = scripts[scripts.length - 1].src\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
         "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) typeof console !== \"undefined\" && console.warn && console.warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\ttypeof console !== \"undefined\" && console.warn && console.warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/notebook\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/notebook\", [1,3,4,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/filebrowser\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/filebrowser\", [1,3,4,3])),\n\t\"webpack/sharing/consume/default/@lumino/disposable\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/disposable\", [1,1,10,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,3,4,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/ui-components\", [1,3,4,3])),\n\t\"webpack/sharing/consume/default/react\": () => (loadSingletonVersionCheck(\"default\", \"react\", [1,17,0,1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/coreutils\", [1,5,4,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/services\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/services\", [1,6,4,3]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/notebook\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/filebrowser\",\n\t\t\"webpack/sharing/consume/default/@lumino/disposable\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\",\n\t\t\"webpack/sharing/consume/default/react\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/services\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
         "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"carpo-teacher\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t} else installedChunks[chunkId] = 0;\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkcarpo_teacher\"] = self[\"webpackChunkcarpo_teacher\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/carpo-teacher\");\n",
         ""
     ],
```

### Comparing `carpo_teacher-0.0.7/carpo_teacher/labextension/static/style_index_js.fc6324d8ef291b0fdd9a.js` & `carpo_teacher-0.0.9/carpo_teacher/labextension/static/style_index_js.fc6324d8ef291b0fdd9a.js`

 * *Files identical despite different names*

### Comparing `carpo_teacher-0.0.7/carpo_teacher/labextension/static/style_index_js.fc6324d8ef291b0fdd9a.js.map` & `carpo_teacher-0.0.9/carpo_teacher/labextension/static/style_index_js.fc6324d8ef291b0fdd9a.js.map`

 * *Files identical despite different names*

### Comparing `carpo_teacher-0.0.7/carpo_teacher/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.6760bbd0c725e3542c7a.js` & `carpo_teacher-0.0.9/carpo_teacher/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.6760bbd0c725e3542c7a.js`

 * *Files identical despite different names*

### Comparing `carpo_teacher-0.0.7/carpo_teacher/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.6760bbd0c725e3542c7a.js.map` & `carpo_teacher-0.0.9/carpo_teacher/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.6760bbd0c725e3542c7a.js.map`

 * *Files identical despite different names*

### Comparing `carpo_teacher-0.0.7/carpo_teacher.egg-info/SOURCES.txt` & `carpo_teacher-0.0.9/carpo_teacher.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 CHANGELOG.md
+DEV_INSTALL.md
 LICENSE
 MANIFEST.in
 README.md
 RELEASE.md
 install.json
 package.json
 pyproject.toml
@@ -15,18 +16,18 @@
 carpo_teacher.egg-info/SOURCES.txt
 carpo_teacher.egg-info/dependency_links.txt
 carpo_teacher.egg-info/not-zip-safe
 carpo_teacher.egg-info/requires.txt
 carpo_teacher.egg-info/top_level.txt
 carpo_teacher/labextension/build_log.json
 carpo_teacher/labextension/package.json
-carpo_teacher/labextension/static/lib_index_js.63bb1f0b3e113fb2d1b6.js
-carpo_teacher/labextension/static/lib_index_js.63bb1f0b3e113fb2d1b6.js.map
-carpo_teacher/labextension/static/remoteEntry.d6f902fe01b1dc4f6fba.js
-carpo_teacher/labextension/static/remoteEntry.d6f902fe01b1dc4f6fba.js.map
+carpo_teacher/labextension/static/lib_index_js.26b2dac9fb26b92e5e77.js
+carpo_teacher/labextension/static/lib_index_js.26b2dac9fb26b92e5e77.js.map
+carpo_teacher/labextension/static/remoteEntry.991b8dc2b6efb319125a.js
+carpo_teacher/labextension/static/remoteEntry.991b8dc2b6efb319125a.js.map
 carpo_teacher/labextension/static/style.js
 carpo_teacher/labextension/static/style_index_js.fc6324d8ef291b0fdd9a.js
 carpo_teacher/labextension/static/style_index_js.fc6324d8ef291b0fdd9a.js.map
 carpo_teacher/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.6760bbd0c725e3542c7a.js
 carpo_teacher/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.6760bbd0c725e3542c7a.js.map
 jupyter-config/nb-config/carpo_teacher.json
 jupyter-config/server-config/carpo_teacher.json
```

### Comparing `carpo_teacher-0.0.7/package.json` & `carpo_teacher-0.0.9/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'0.0.9'"}*

```diff
@@ -106,9 +106,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.0.7"
+    "version": "0.0.9"
 }
```

### Comparing `carpo_teacher-0.0.7/pyproject.toml` & `carpo_teacher-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `carpo_teacher-0.0.7/setup.py` & `carpo_teacher-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `carpo_teacher-0.0.7/src/handler.ts` & `carpo_teacher-0.0.9/src/handler.ts`

 * *Files identical despite different names*

### Comparing `carpo_teacher-0.0.7/src/index.ts` & `carpo_teacher-0.0.9/src/index.ts`

 * *Files 6% similar despite different names*

```diff
@@ -140,20 +140,18 @@
         });
 
       });
     });
     
     //  tell the document registry about your widget extension:
     app.docRegistry.addWidgetExtension('Notebook', new RegisterButton());
-    app.docRegistry.addWidgetExtension('Notebook', new NewSubmissionButtonExtension());
-    app.docRegistry.addWidgetExtension('Notebook', new AllSubmissionButtonExtension());
+    app.docRegistry.addWidgetExtension('Notebook', new GoToApp());
     app.docRegistry.addWidgetExtension('Notebook', new PublishProblemButtonExtension());
     app.docRegistry.addWidgetExtension('Notebook', new ArchiveProblemButtonExtension());
     app.docRegistry.addWidgetExtension('Notebook', new GetSolutionButton());
-    app.docRegistry.addWidgetExtension('Notebook', new viewProblemStatusExtension());
     
   }
 };
 
 export class RegisterButton
   implements DocumentRegistry.IWidgetExtension<NotebookPanel, INotebookModel>
 {
@@ -202,14 +200,54 @@
     panel.toolbar.insertItem(10, 'register', button);
     return new DisposableDelegate(() => {
       button.dispose();
     });
   }
 }
 
+export class GoToApp implements DocumentRegistry.IWidgetExtension<NotebookPanel, INotebookModel>
+{
+  createNew(
+    panel: NotebookPanel,
+    context: DocumentRegistry.IContext<INotebookModel>
+  ): IDisposable {
+    const viewWebApp = () => {
+
+    requestAPI<any>('view_app',{
+      method: 'GET'
+    })
+      .then(data => {
+        // console.log(data);
+        window.open(
+          data.url, "_blank");
+      })
+      .catch(reason => {
+        showErrorMessage('View App Status Error', reason);
+        console.error(
+          `Failed to view app status.\n${reason}`
+        );
+      });
+
+    };
+
+    const button = new ToolbarButton({
+      className: 'get-app-button',
+      label: 'App',
+      onClick: viewWebApp,
+      tooltip: 'Go to the web app',
+    });
+
+    panel.toolbar.insertItem(11, 'viewWebApp', button);
+
+    return new DisposableDelegate(() => {
+      button.dispose();
+    });
+  }
+}
+
 
 export class NewSubmissionButtonExtension
   implements DocumentRegistry.IWidgetExtension<NotebookPanel, INotebookModel>
 {
   /**
    * Create a new extension for the notebook panel widget.
    *
@@ -411,15 +449,15 @@
     const button = new ToolbarButton({
       className: 'publish-problem-button',
       label: 'Publish',
       onClick: publishProblem,
       tooltip: 'Publish New Problem.',
     });
 
-    panel.toolbar.insertItem(13, 'publishNewProblem', button);
+    panel.toolbar.insertItem(12, 'publishNewProblem', button);
     return new DisposableDelegate(() => {
       button.dispose();
     });
   }
 }
 
 export class ArchiveProblemButtonExtension
@@ -487,62 +525,15 @@
     const button = new ToolbarButton({
       className: 'archive-problem-button',
       label: 'Unpublish',
       onClick: archiveProblem,
       tooltip: 'Unpublish the problem.',
     });
 
-    panel.toolbar.insertItem(14, 'archivesProblem', button);
-    return new DisposableDelegate(() => {
-      button.dispose();
-    });
-  }
-}
-
-export class viewProblemStatusExtension
-  implements DocumentRegistry.IWidgetExtension<NotebookPanel, INotebookModel>
-{
-  /**
-   * Create a new extension for the notebook panel widget.
-   *
-   * @param panel Notebook panel
-   * @param context Notebook context
-   * @returns Disposable on the added button
-   */
-  createNew(
-    panel: NotebookPanel,
-    context: DocumentRegistry.IContext<INotebookModel>
-  ): IDisposable {
-    const viewProblemStatus = () => {
-
-      requestAPI<any>('view_problem_list',{
-        method: 'GET'
-      })
-        .then(data => {
-          console.log(data);
-          window.open(
-            data.url, "_blank");
-        })
-        .catch(reason => {
-          showErrorMessage('View Problem Status Error', reason);
-          console.error(
-            `Failed to view problem status.\n${reason}`
-          );
-        });
-
-    };
-
-    const button = new ToolbarButton({
-      className: 'get-status-button',
-      label: 'Problems',
-      onClick: viewProblemStatus,
-      tooltip: 'View all problem status',
-    });
-
-    panel.toolbar.insertItem(16, 'viewProblemStatus', button);
+    panel.toolbar.insertItem(13, 'archivesProblem', button);
     return new DisposableDelegate(() => {
       button.dispose();
     });
   }
 }
 
 export default plugin;
```

### Comparing `carpo_teacher-0.0.7/src/upload-solution.ts` & `carpo_teacher-0.0.9/src/upload-solution.ts`

 * *Files 0% similar despite different names*

```diff
@@ -77,13 +77,13 @@
     const button = new ToolbarButton({
       className: 'upload-solution-button',
       label: 'UploadSolution',
       onClick: uploadSolution,
       tooltip: 'Upload solutions to the problem.',
     });
 
-    panel.toolbar.insertItem(15, 'getSolutions', button);
+    panel.toolbar.insertItem(14, 'getSolutions', button);
     return new DisposableDelegate(() => {
       button.dispose();
     });
   }
 }
```

### Comparing `carpo_teacher-0.0.7/src/widget.tsx` & `carpo_teacher-0.0.9/src/widget.tsx`

 * *Files identical despite different names*

### Comparing `carpo_teacher-0.0.7/style/base.css` & `carpo_teacher-0.0.9/style/base.css`

 * *Files identical despite different names*

### Comparing `carpo_teacher-0.0.7/tsconfig.json` & `carpo_teacher-0.0.9/tsconfig.json`

 * *Files identical despite different names*

