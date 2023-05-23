# Comparing `tmp/carpo_student-0.0.8.tar.gz` & `tmp/carpo_student-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carpo_student-0.0.8.tar", last modified: Wed Sep 21 16:50:24 2022, max compression
+gzip compressed data, was "carpo_student-0.0.9.tar", last modified: Tue May 23 14:21:37 2023, max compression
```

## Comparing `carpo_student-0.0.8.tar` & `carpo_student-0.0.9.tar`

### file list

```diff
@@ -1,54 +1,56 @@
-drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2022-09-21 16:50:24.950876 carpo_student-0.0.8/
--rw-rw-r--   0 kritish   (1000) kritish   (1000)       86 2022-04-22 15:03:31.000000 carpo_student-0.0.8/CHANGELOG.md
--rw-rw-r--   0 kritish   (1000) kritish   (1000)     1508 2022-04-22 15:03:31.000000 carpo_student-0.0.8/LICENSE
--rw-rw-r--   0 kritish   (1000) kritish   (1000)      447 2022-04-22 15:03:31.000000 carpo_student-0.0.8/MANIFEST.in
--rw-rw-r--   0 kritish   (1000) kritish   (1000)     4408 2022-09-21 16:50:24.950876 carpo_student-0.0.8/PKG-INFO
--rw-rw-r--   0 kritish   (1000) kritish   (1000)     3373 2022-07-01 16:27:38.000000 carpo_student-0.0.8/README.md
--rw-rw-r--   0 kritish   (1000) kritish   (1000)     1895 2022-04-22 15:03:31.000000 carpo_student-0.0.8/RELEASE.md
-drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2022-09-21 16:50:24.946876 carpo_student-0.0.8/carpo_student/
--rw-rw-r--   0 kritish   (1000) kritish   (1000)      976 2022-04-28 03:03:51.000000 carpo_student-0.0.8/carpo_student/__init__.py
--rw-rw-r--   0 kritish   (1000) kritish   (1000)      625 2022-04-28 03:03:51.000000 carpo_student-0.0.8/carpo_student/_version.py
--rw-rw-r--   0 kritish   (1000) kritish   (1000)    21238 2022-09-21 16:41:08.000000 carpo_student-0.0.8/carpo_student/handlers.py
-drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2022-09-21 16:50:24.946876 carpo_student-0.0.8/carpo_student/labextension/
--rw-rw-r--   0 kritish   (1000) kritish   (1000)    20809 2022-08-31 15:54:29.000000 carpo_student-0.0.8/carpo_student/labextension/build_log.json
--rw-rw-r--   0 kritish   (1000) kritish   (1000)     3748 2022-08-31 15:54:29.000000 carpo_student-0.0.8/carpo_student/labextension/package.json
-drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2022-09-21 16:50:24.946876 carpo_student-0.0.8/carpo_student/labextension/static/
--rw-rw-r--   0 kritish   (1000) kritish   (1000)    31147 2022-08-31 15:54:29.000000 carpo_student-0.0.8/carpo_student/labextension/static/lib_index_js.c3e6db586344d03a5551.js
--rw-rw-r--   0 kritish   (1000) kritish   (1000)    26184 2022-08-31 15:54:29.000000 carpo_student-0.0.8/carpo_student/labextension/static/lib_index_js.c3e6db586344d03a5551.js.map
--rw-rw-r--   0 kritish   (1000) kritish   (1000)    29068 2022-08-31 15:54:29.000000 carpo_student-0.0.8/carpo_student/labextension/static/remoteEntry.b940a131cff178ae61e8.js
--rw-rw-r--   0 kritish   (1000) kritish   (1000)    27805 2022-08-31 15:54:29.000000 carpo_student-0.0.8/carpo_student/labextension/static/remoteEntry.b940a131cff178ae61e8.js.map
--rw-rw-r--   0 kritish   (1000) kritish   (1000)      156 2022-08-31 15:54:29.000000 carpo_student-0.0.8/carpo_student/labextension/static/style.js
--rw-rw-r--   0 kritish   (1000) kritish   (1000)     6240 2022-08-31 15:54:29.000000 carpo_student-0.0.8/carpo_student/labextension/static/style_index_js.e596dd9ff10e476ac3a0.js
--rw-rw-r--   0 kritish   (1000) kritish   (1000)     4188 2022-08-31 15:54:29.000000 carpo_student-0.0.8/carpo_student/labextension/static/style_index_js.e596dd9ff10e476ac3a0.js.map
--rw-rw-r--   0 kritish   (1000) kritish   (1000)    12056 2022-08-31 15:54:29.000000 carpo_student-0.0.8/carpo_student/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.a80375a08cdf3b742d9b.js
--rw-rw-r--   0 kritish   (1000) kritish   (1000)    13787 2022-08-31 15:54:29.000000 carpo_student-0.0.8/carpo_student/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.a80375a08cdf3b742d9b.js.map
-drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2022-09-21 16:50:24.946876 carpo_student-0.0.8/carpo_student.egg-info/
--rw-rw-r--   0 kritish   (1000) kritish   (1000)     4408 2022-09-21 16:50:24.000000 carpo_student-0.0.8/carpo_student.egg-info/PKG-INFO
--rw-rw-r--   0 kritish   (1000) kritish   (1000)     1545 2022-09-21 16:50:24.000000 carpo_student-0.0.8/carpo_student.egg-info/SOURCES.txt
--rw-rw-r--   0 kritish   (1000) kritish   (1000)        1 2022-09-21 16:50:24.000000 carpo_student-0.0.8/carpo_student.egg-info/dependency_links.txt
--rw-rw-r--   0 kritish   (1000) kritish   (1000)        1 2022-04-08 22:56:48.000000 carpo_student-0.0.8/carpo_student.egg-info/not-zip-safe
--rw-rw-r--   0 kritish   (1000) kritish   (1000)       23 2022-09-21 16:50:24.000000 carpo_student-0.0.8/carpo_student.egg-info/requires.txt
--rw-rw-r--   0 kritish   (1000) kritish   (1000)       14 2022-09-21 16:50:24.000000 carpo_student-0.0.8/carpo_student.egg-info/top_level.txt
--rw-rw-r--   0 kritish   (1000) kritish   (1000)      187 2022-04-22 15:03:31.000000 carpo_student-0.0.8/install.json
-drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2022-09-21 16:50:24.942876 carpo_student-0.0.8/jupyter-config/
-drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2022-09-21 16:50:24.946876 carpo_student-0.0.8/jupyter-config/nb-config/
--rw-rw-r--   0 kritish   (1000) kritish   (1000)       90 2022-04-22 15:03:31.000000 carpo_student-0.0.8/jupyter-config/nb-config/carpo_student.json
-drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2022-09-21 16:50:24.946876 carpo_student-0.0.8/jupyter-config/server-config/
--rw-rw-r--   0 kritish   (1000) kritish   (1000)       88 2022-04-22 15:03:31.000000 carpo_student-0.0.8/jupyter-config/server-config/carpo_student.json
--rw-rw-r--   0 kritish   (1000) kritish   (1000)     3606 2022-09-21 16:40:43.000000 carpo_student-0.0.8/package.json
--rw-rw-r--   0 kritish   (1000) kritish   (1000)      587 2022-04-22 15:03:31.000000 carpo_student-0.0.8/pyproject.toml
--rw-rw-r--   0 kritish   (1000) kritish   (1000)       38 2022-09-21 16:50:24.950876 carpo_student-0.0.8/setup.cfg
--rw-rw-r--   0 kritish   (1000) kritish   (1000)     3181 2022-04-22 15:03:31.000000 carpo_student-0.0.8/setup.py
-drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2022-09-21 16:50:24.946876 carpo_student-0.0.8/src/
--rw-rw-r--   0 kritish   (1000) kritish   (1000)     1739 2022-07-07 03:40:34.000000 carpo_student-0.0.8/src/get-solutions.ts
--rw-rw-r--   0 kritish   (1000) kritish   (1000)     1100 2022-04-22 15:03:31.000000 carpo_student-0.0.8/src/handler.ts
--rw-rw-r--   0 kritish   (1000) kritish   (1000)    10685 2022-08-31 15:54:16.000000 carpo_student-0.0.8/src/index.ts
--rw-rw-r--   0 kritish   (1000) kritish   (1000)       89 2022-04-22 15:03:31.000000 carpo_student-0.0.8/src/model.ts
--rw-rw-r--   0 kritish   (1000) kritish   (1000)     4227 2022-08-26 06:09:54.000000 carpo_student-0.0.8/src/share-code.ts
--rw-rw-r--   0 kritish   (1000) kritish   (1000)     4296 2022-07-06 21:59:10.000000 carpo_student-0.0.8/src/widget.tsx
-drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2022-09-21 16:50:24.950876 carpo_student-0.0.8/style/
--rw-rw-r--   0 kritish   (1000) kritish   (1000)      722 2022-07-06 21:42:41.000000 carpo_student-0.0.8/style/base.css
--rw-rw-r--   0 kritish   (1000) kritish   (1000)       26 2022-04-22 15:03:31.000000 carpo_student-0.0.8/style/index.css
--rw-rw-r--   0 kritish   (1000) kritish   (1000)       21 2022-04-22 15:03:31.000000 carpo_student-0.0.8/style/index.js
--rw-rw-r--   0 kritish   (1000) kritish   (1000)      555 2022-04-22 15:03:31.000000 carpo_student-0.0.8/tsconfig.json
--rw-rw-r--   0 kritish   (1000) kritish   (1000)   297625 2022-07-18 18:36:51.000000 carpo_student-0.0.8/yarn.lock
+drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2023-05-23 14:21:37.283083 carpo_student-0.0.9/
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)       86 2022-04-22 15:03:31.000000 carpo_student-0.0.9/CHANGELOG.md
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)     3373 2022-10-14 15:34:26.000000 carpo_student-0.0.9/DEV_INSTALL.md
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)      833 2022-10-17 17:31:16.000000 carpo_student-0.0.9/INSTALL.md
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)     1508 2022-04-22 15:03:31.000000 carpo_student-0.0.9/LICENSE
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)      447 2022-04-22 15:03:31.000000 carpo_student-0.0.9/MANIFEST.in
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)     1962 2023-05-23 14:21:37.283083 carpo_student-0.0.9/PKG-INFO
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)      927 2022-10-14 15:34:26.000000 carpo_student-0.0.9/README.md
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)     1895 2022-04-22 15:03:31.000000 carpo_student-0.0.9/RELEASE.md
+drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2023-05-23 14:21:37.279083 carpo_student-0.0.9/carpo_student/
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)      976 2022-04-28 03:03:51.000000 carpo_student-0.0.9/carpo_student/__init__.py
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)      625 2022-04-28 03:03:51.000000 carpo_student-0.0.9/carpo_student/_version.py
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)    21276 2023-05-23 14:01:27.000000 carpo_student-0.0.9/carpo_student/handlers.py
+drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2023-05-23 14:21:37.279083 carpo_student-0.0.9/carpo_student/labextension/
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)    20809 2023-05-18 20:21:15.000000 carpo_student-0.0.9/carpo_student/labextension/build_log.json
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)     3748 2023-05-18 20:21:15.000000 carpo_student-0.0.9/carpo_student/labextension/package.json
+drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2023-05-23 14:21:37.283083 carpo_student-0.0.9/carpo_student/labextension/static/
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)    32796 2023-05-18 20:21:15.000000 carpo_student-0.0.9/carpo_student/labextension/static/lib_index_js.702cd083cba688e6ae07.js
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)    28366 2023-05-18 20:21:15.000000 carpo_student-0.0.9/carpo_student/labextension/static/lib_index_js.702cd083cba688e6ae07.js.map
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)    29068 2023-05-18 20:21:15.000000 carpo_student-0.0.9/carpo_student/labextension/static/remoteEntry.8056dafefbbffbedae97.js
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)    27805 2023-05-18 20:21:15.000000 carpo_student-0.0.9/carpo_student/labextension/static/remoteEntry.8056dafefbbffbedae97.js.map
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)      156 2023-05-18 20:21:15.000000 carpo_student-0.0.9/carpo_student/labextension/static/style.js
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)     6240 2023-05-18 20:21:15.000000 carpo_student-0.0.9/carpo_student/labextension/static/style_index_js.e596dd9ff10e476ac3a0.js
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)     4188 2023-05-18 20:21:15.000000 carpo_student-0.0.9/carpo_student/labextension/static/style_index_js.e596dd9ff10e476ac3a0.js.map
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)    12056 2023-05-18 20:21:15.000000 carpo_student-0.0.9/carpo_student/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.a80375a08cdf3b742d9b.js
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)    13787 2023-05-18 20:21:15.000000 carpo_student-0.0.9/carpo_student/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.a80375a08cdf3b742d9b.js.map
+drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2023-05-23 14:21:37.279083 carpo_student-0.0.9/carpo_student.egg-info/
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)     1962 2023-05-23 14:21:36.000000 carpo_student-0.0.9/carpo_student.egg-info/PKG-INFO
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)     1571 2023-05-23 14:21:37.000000 carpo_student-0.0.9/carpo_student.egg-info/SOURCES.txt
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)        1 2023-05-23 14:21:36.000000 carpo_student-0.0.9/carpo_student.egg-info/dependency_links.txt
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)        1 2022-04-08 22:56:48.000000 carpo_student-0.0.9/carpo_student.egg-info/not-zip-safe
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)       23 2023-05-23 14:21:37.000000 carpo_student-0.0.9/carpo_student.egg-info/requires.txt
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)       14 2023-05-23 14:21:37.000000 carpo_student-0.0.9/carpo_student.egg-info/top_level.txt
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)      187 2022-04-22 15:03:31.000000 carpo_student-0.0.9/install.json
+drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2023-05-23 14:21:37.275082 carpo_student-0.0.9/jupyter-config/
+drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2023-05-23 14:21:37.283083 carpo_student-0.0.9/jupyter-config/nb-config/
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)       90 2022-04-22 15:03:31.000000 carpo_student-0.0.9/jupyter-config/nb-config/carpo_student.json
+drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2023-05-23 14:21:37.283083 carpo_student-0.0.9/jupyter-config/server-config/
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)       88 2022-04-22 15:03:31.000000 carpo_student-0.0.9/jupyter-config/server-config/carpo_student.json
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)     3606 2023-05-23 14:01:04.000000 carpo_student-0.0.9/package.json
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)      587 2022-04-22 15:03:31.000000 carpo_student-0.0.9/pyproject.toml
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)       38 2023-05-23 14:21:37.283083 carpo_student-0.0.9/setup.cfg
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)     3181 2022-04-22 15:03:31.000000 carpo_student-0.0.9/setup.py
+drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2023-05-23 14:21:37.283083 carpo_student-0.0.9/src/
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)     1739 2022-10-14 15:34:26.000000 carpo_student-0.0.9/src/get-solutions.ts
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)     1100 2022-04-22 15:03:31.000000 carpo_student-0.0.9/src/handler.ts
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)    11773 2023-05-23 13:58:28.000000 carpo_student-0.0.9/src/index.ts
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)       89 2022-04-22 15:03:31.000000 carpo_student-0.0.9/src/model.ts
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)     4332 2022-12-20 04:38:25.000000 carpo_student-0.0.9/src/share-code.ts
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)     4511 2023-05-18 20:21:06.000000 carpo_student-0.0.9/src/widget.tsx
+drwxrwxr-x   0 kritish   (1000) kritish   (1000)        0 2023-05-23 14:21:37.283083 carpo_student-0.0.9/style/
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)      722 2022-10-14 15:34:26.000000 carpo_student-0.0.9/style/base.css
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)       26 2022-04-22 15:03:31.000000 carpo_student-0.0.9/style/index.css
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)       21 2022-04-22 15:03:31.000000 carpo_student-0.0.9/style/index.js
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)      555 2022-04-22 15:03:31.000000 carpo_student-0.0.9/tsconfig.json
+-rw-rw-r--   0 kritish   (1000) kritish   (1000)   297625 2022-07-18 18:36:51.000000 carpo_student-0.0.9/yarn.lock
```

### Comparing `carpo_student-0.0.8/LICENSE` & `carpo_student-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `carpo_student-0.0.8/PKG-INFO` & `carpo_student-0.0.9/DEV_INSTALL.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,7 @@
-Metadata-Version: 2.1
-Name: carpo_student
-Version: 0.0.8
-Summary: JupyterLab extension with backend and frontend parts for carpo student.
-Home-page: https://github.com/github_username/carpo-student
-Author: 
-Author-email: 
-License: BSD-3-Clause
-Keywords: Jupyter,JupyterLab,JupyterLab3
-Platform: Linux
-Platform: Mac OS X
-Platform: Windows
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Framework :: Jupyter
-Classifier: Framework :: Jupyter :: JupyterLab
-Classifier: Framework :: Jupyter :: JupyterLab :: 3
-Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
-Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # carpo_student
 
 [![Github Actions Status](https://github.com/github_username/carpo-student/workflows/Build/badge.svg)](https://github.com/github_username/carpo-student/actions/workflows/build.yml)[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/github_username/carpo-student/main?urlpath=lab)
 
 JupyterLab extension with backend and frontend parts for carpo student.
 
 
@@ -132,9 +104,7 @@
 In development mode, you will also need to remove the symlink created by `jupyter labextension develop`
 command. To find its location, you can run `jupyter labextension list` to figure out where the `labextensions`
 folder is located. Then you can remove the symlink named `carpo-student` within that folder.
 
 ### Packaging the extension
 
 See [RELEASE](RELEASE.md)
-
-
```

### Comparing `carpo_student-0.0.8/RELEASE.md` & `carpo_student-0.0.9/RELEASE.md`

 * *Files identical despite different names*

### Comparing `carpo_student-0.0.8/carpo_student/__init__.py` & `carpo_student-0.0.9/carpo_student/__init__.py`

 * *Files identical despite different names*

### Comparing `carpo_student-0.0.8/carpo_student/_version.py` & `carpo_student-0.0.9/carpo_student/_version.py`

 * *Files identical despite different names*

### Comparing `carpo_student-0.0.8/carpo_student/handlers.py` & `carpo_student-0.0.9/carpo_student/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from jupyter_server.base.handlers import APIHandler
 from jupyter_server.utils import url_path_join
 import tornado
 import requests
 import os
 import uuid
 
+from jupyter_server import serverapp
+
 
 def read_config_file():
     """
     reads config.json file
     :return: dict
     """
     config_file = os.path.join(os.getcwd() ,"Exercises",'config.json')
@@ -31,15 +33,15 @@
    
     # Create config.json file
     config_path = os.path.join(current_dir,"Exercises","config.json")
     if not os.path.isfile(config_path):
         config_data = {}
         config_data['name'] = "John Smith"
         config_data['server'] = "http://delphinus.cs.memphis.edu:XXXX"
-        config_data['carpo_version'] = "0.0.8"
+        config_data['carpo_version'] = "0.0.9"
         # Write default config
         with open(config_path, "w") as config_file:
             config_file.write(json.dumps(config_data, indent=4))
     
     # Create blank notebook
     notebook_path = os.path.join(current_dir,"Exercises","Readme.ipynb")
     if not os.path.isfile(notebook_path):
```

### Comparing `carpo_student-0.0.8/carpo_student/labextension/build_log.json` & `carpo_student-0.0.9/carpo_student/labextension/build_log.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999992921055613%*

 * *Differences: {'0': "{'plugins': {1: {'_options': {'shared': {'carpo-student': {'version': '0.0.8'}}}}}}"}*

```diff
@@ -580,15 +580,15 @@
                             "import": false,
                             "requiredVersion": "^1.30.0",
                             "singleton": true
                         },
                         "carpo-student": {
                             "import": "/home/kritish/Projects/carpo/carpo_student/lib/index.js",
                             "singleton": true,
-                            "version": "0.0.7"
+                            "version": "0.0.8"
                         },
                         "react": {
                             "import": false,
                             "requiredVersion": "^17.0.1",
                             "singleton": true
                         },
                         "react-dom": {
```

### Comparing `carpo_student-0.0.8/carpo_student/labextension/package.json` & `carpo_student-0.0.9/carpo_student/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9756944444444444%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.8056dafefbbffbedae97.js'}}",*

 * * "'version'": "'0.0.8'"}*

```diff
@@ -48,15 +48,15 @@
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.b940a131cff178ae61e8.js",
+            "load": "static/remoteEntry.8056dafefbbffbedae97.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "carpo_student"
                 },
@@ -111,9 +111,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.0.7"
+    "version": "0.0.8"
 }
```

### Comparing `carpo_student-0.0.8/carpo_student/labextension/static/lib_index_js.c3e6db586344d03a5551.js` & `carpo_student-0.0.9/carpo_student/labextension/static/lib_index_js.702cd083cba688e6ae07.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -168,27 +168,27 @@
                 /* harmony import */
                 var _widget__WEBPACK_IMPORTED_MODULE_4__ = __webpack_require__( /*! ./widget */ "./lib/widget.js");
                 /* harmony import */
                 var _jupyterlab_settingregistry__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__( /*! @jupyterlab/settingregistry */ "webpack/sharing/consume/default/@jupyterlab/settingregistry");
                 /* harmony import */
                 var _jupyterlab_settingregistry__WEBPACK_IMPORTED_MODULE_1___default = /*#__PURE__*/ __webpack_require__.n(_jupyterlab_settingregistry__WEBPACK_IMPORTED_MODULE_1__);
                 /* harmony import */
-                var _handler__WEBPACK_IMPORTED_MODULE_7__ = __webpack_require__( /*! ./handler */ "./lib/handler.js");
+                var _handler__WEBPACK_IMPORTED_MODULE_5__ = __webpack_require__( /*! ./handler */ "./lib/handler.js");
                 /* harmony import */
                 var _lumino_disposable__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__( /*! @lumino/disposable */ "webpack/sharing/consume/default/@lumino/disposable");
                 /* harmony import */
                 var _lumino_disposable__WEBPACK_IMPORTED_MODULE_2___default = /*#__PURE__*/ __webpack_require__.n(_lumino_disposable__WEBPACK_IMPORTED_MODULE_2__);
                 /* harmony import */
                 var _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__( /*! @jupyterlab/apputils */ "webpack/sharing/consume/default/@jupyterlab/apputils");
                 /* harmony import */
                 var _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_3___default = /*#__PURE__*/ __webpack_require__.n(_jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_3__);
                 /* harmony import */
-                var _share_code__WEBPACK_IMPORTED_MODULE_5__ = __webpack_require__( /*! ./share-code */ "./lib/share-code.js");
+                var _share_code__WEBPACK_IMPORTED_MODULE_6__ = __webpack_require__( /*! ./share-code */ "./lib/share-code.js");
                 /* harmony import */
-                var _get_solutions__WEBPACK_IMPORTED_MODULE_6__ = __webpack_require__( /*! ./get-solutions */ "./lib/get-solutions.js");
+                var _get_solutions__WEBPACK_IMPORTED_MODULE_7__ = __webpack_require__( /*! ./get-solutions */ "./lib/get-solutions.js");
 
 
 
 
 
 
 
@@ -199,16 +199,18 @@
                 const plugin = {
                     id: 'carpo-student:plugin',
                     autoStart: true,
                     requires: [_jupyterlab_notebook__WEBPACK_IMPORTED_MODULE_0__.INotebookTracker],
                     optional: [_jupyterlab_settingregistry__WEBPACK_IMPORTED_MODULE_1__.ISettingRegistry],
                     activate: (app, nbTrack, settingRegistry) => {
                         console.log('JupyterLab extension carpo-student is activated!');
+                        // var interval => (); 
+                        var counter = 0;
                         nbTrack.currentChanged.connect(() => {
-                            console.log("->: ", nbTrack.currentWidget.context.path);
+                            console.log("my counter: ", counter);
                             const notebookPanel = nbTrack.currentWidget;
                             const notebook = nbTrack.currentWidget.content;
                             const filename = notebookPanel.context.path;
                             // Disable Code Share functionality if inside Feedback directory
                             if (filename.includes("Feedback")) {
                                 return;
                             }
@@ -241,33 +243,59 @@
                                     // Get the message block referencing the active cell.
                                     notebook.widgets.map((c, index) => {
                                         if (c.model.value.text.startsWith("## Message to instructor:")) {
                                             info.message = c.model.value.text;
                                         }
                                         if (index == activeIndex) {
                                             question = c.model.value.text;
+                                            if (question.includes("## PID ")) {
+                                                const newCheckButton = new _widget__WEBPACK_IMPORTED_MODULE_4__.CellCheckButton(cell, info);
+                                                cell.layout.addWidget(newCheckButton);
+                                                currentCellCheckButton = newCheckButton;
+                                                // Send code snapshot to the server:
+                                                if (counter == 0) {
+                                                    setInterval(function() {
+                                                        // console.log("Update: ", c.model.value.text)
+                                                        let postBody = {
+                                                            "message": "",
+                                                            "code": c.model.value.text,
+                                                            "problem_id": info.problem_id,
+                                                            "snapshot": 1
+                                                        };
+                                                        // console.log("From widget: ", postBody)
+                                                        (0, _handler__WEBPACK_IMPORTED_MODULE_5__.requestAPI)('submissions', {
+                                                            method: 'POST',
+                                                            body: JSON.stringify(postBody)
+                                                        })
+                                                        .then(data => {
+                                                            console.log("Snapshot sent.", data);
+                                                        });
+                                                    }, 10000);
+                                                    counter++;
+                                                }
+                                            }
                                         }
                                     });
-                                    const newCheckButton = new _widget__WEBPACK_IMPORTED_MODULE_4__.CellCheckButton(cell, info);
-                                    if (question.includes("## PID ")) {
-                                        cell.layout.addWidget(newCheckButton);
-                                        currentCellCheckButton = newCheckButton;
-                                    }
+                                    // const newCheckButton: CellCheckButton = new CellCheckButton(cell,info);
+                                    // if (question.includes("## PID ")){
+                                    //   (cell.layout as PanelLayout).addWidget(newCheckButton);
+                                    //   currentCellCheckButton = newCheckButton;
+                                    // }
                                     // Set the current cell and button for future
                                     // reference
                                     currentCell = cell;
                                 });
                             });
                         });
                         //  tell the document registry about your widget extension:
                         app.docRegistry.addWidgetExtension('Notebook', new RegisterButton());
                         app.docRegistry.addWidgetExtension('Notebook', new GetQuestionButton());
-                        app.docRegistry.addWidgetExtension('Notebook', new _share_code__WEBPACK_IMPORTED_MODULE_5__.ShareCodeButton());
+                        app.docRegistry.addWidgetExtension('Notebook', new _share_code__WEBPACK_IMPORTED_MODULE_6__.ShareCodeButton());
                         app.docRegistry.addWidgetExtension('Notebook', new GetFeedbackButton());
-                        app.docRegistry.addWidgetExtension('Notebook', new _get_solutions__WEBPACK_IMPORTED_MODULE_6__.GetSolutionButton());
+                        app.docRegistry.addWidgetExtension('Notebook', new _get_solutions__WEBPACK_IMPORTED_MODULE_7__.GetSolutionButton());
                         app.docRegistry.addWidgetExtension('Notebook', new ViewSubmissionStatusButton());
                         // app.docRegistry.addWidgetExtension('Notebook', new viewProblemStatusExtension());
                     }
                 };
                 class RegisterButton {
                     /**
                      * Create a new extension for the notebook panel widget.
@@ -276,15 +304,15 @@
                      * @param context Notebook context
                      * @returns Disposable on the added button
                      */
                     createNew(panel, context) {
                         const register = () => {
                             // NotebookActions.clearAllOutputs(panel.content);
                             // const notebook = panel.content;
-                            (0, _handler__WEBPACK_IMPORTED_MODULE_7__.requestAPI)('register', {
+                            (0, _handler__WEBPACK_IMPORTED_MODULE_5__.requestAPI)('register', {
                                 method: 'GET'
                             })
                             .then(data => {
                                     console.log(data);
                                     (0, _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_3__.showDialog)({
                                         title: '',
                                         body: "Student " + data.name + " has been registered.",
@@ -318,15 +346,15 @@
                      * @param context Notebook context
                      * @returns Disposable on the added button
                      */
                     createNew(panel, context) {
                         const getQuestion = () => {
                             // NotebookActions.clearAllOutputs(panel.content);
                             // const notebook = panel.content;
-                            (0, _handler__WEBPACK_IMPORTED_MODULE_7__.requestAPI)('question', {
+                            (0, _handler__WEBPACK_IMPORTED_MODULE_5__.requestAPI)('question', {
                                 method: 'GET'
                             })
                             .then(data => {
                                     console.log(data);
                                     (0, _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_3__.showDialog)({
                                         title: '',
                                         body: data.msg,
@@ -358,15 +386,15 @@
                      *
                      * @param panel Notebook panel
                      * @param context Notebook context
                      * @returns Disposable on the added button
                      */
                     createNew(panel, context) {
                         const getFeedback = () => {
-                            (0, _handler__WEBPACK_IMPORTED_MODULE_7__.requestAPI)('feedback', {
+                            (0, _handler__WEBPACK_IMPORTED_MODULE_5__.requestAPI)('feedback', {
                                 method: 'GET'
                             })
                             .then(data => {
                                     console.log(data);
                                     (0, _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_3__.showDialog)({
                                         title: '',
                                         body: data.msg,
@@ -402,15 +430,15 @@
                      *
                      * @param panel Notebook panel
                      * @param context Notebook context
                      * @returns Disposable on the added button
                      */
                     createNew(panel, context) {
                         const viewStatus = () => {
-                            (0, _handler__WEBPACK_IMPORTED_MODULE_7__.requestAPI)('view_student_status', {
+                            (0, _handler__WEBPACK_IMPORTED_MODULE_5__.requestAPI)('view_student_status', {
                                 method: 'GET'
                             })
                             .then(data => {
                                     console.log(data);
                                     window.open(data.url, "_blank");
                                 })
                                 .catch(reason => {
@@ -437,15 +465,15 @@
                      *
                      * @param panel Notebook panel
                      * @param context Notebook context
                      * @returns Disposable on the added button
                      */
                     createNew(panel, context) {
                         const viewProblemStatus = () => {
-                            (0, _handler__WEBPACK_IMPORTED_MODULE_7__.requestAPI)('view_problem_list', {
+                            (0, _handler__WEBPACK_IMPORTED_MODULE_5__.requestAPI)('view_problem_list', {
                                 method: 'GET'
                             })
                             .then(data => {
                                     console.log(data);
                                     window.open(data.url, "_blank");
                                 })
                                 .catch(reason => {
@@ -528,15 +556,16 @@
                             if (!codeBlock.startsWith("## PID ")) {
                                 (0, _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_1__.showErrorMessage)('Code Share Error', "Invalid cell selected. Use a specific problem cell block.");
                                 return;
                             }
                             let postBody = {
                                 "message": info.message,
                                 "code": codeBlock,
-                                "problem_id": info.problem_id
+                                "problem_id": info.problem_id,
+                                "snapshot": 2
                             };
                             console.log("Req body: ", postBody);
                             (0, _handler__WEBPACK_IMPORTED_MODULE_2__.requestAPI)('submissions', {
                                 method: 'POST',
                                 body: JSON.stringify(postBody)
                             })
                             .then(data => {
@@ -552,40 +581,40 @@
                                         body: data.msg,
                                         buttons: [_jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_1__.Dialog.okButton({
                                             label: 'Ok'
                                         })]
                                     });
                                     // Keep checking for new feedback.
                                     // This setInterval will be cleared once the feedback is downloaded (after reload())
-                                    setInterval(function() {
-                                        // console.log("Checking for feedback...")
-                                        (0, _handler__WEBPACK_IMPORTED_MODULE_2__.requestAPI)('feedback', {
-                                            method: 'GET'
-                                        })
-                                        .then(data => {
-                                                // console.log(data);
-                                                if (data['hard-reload'] != -1) {
-                                                    (0, _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_1__.showDialog)({
-                                                        title: '',
-                                                        body: data.msg,
-                                                        buttons: [_jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_1__.Dialog.okButton({
-                                                            label: 'Ok'
-                                                        })]
-                                                    }).then(result => {
-                                                        if (result.button.accept) {
-                                                            window.location.reload();
-                                                        }
-                                                    });
-                                                }
-                                            })
-                                            .catch(reason => {
-                                                (0, _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_1__.showErrorMessage)('Get Feedback Error', reason);
-                                                console.error(`Failed to fetch recent feedbacks.\n${reason}`);
-                                            });
-                                    }, 60000);
+                                    // setInterval(function(){
+                                    //     // console.log("Checking for feedback...")
+                                    //     requestAPI<any>('feedback',{
+                                    //     method: 'GET'
+                                    //     })
+                                    //     .then(data => {
+                                    //         // console.log(data);
+                                    //         if (data['hard-reload'] != -1) {
+                                    //         showDialog({
+                                    //             title:'',
+                                    //             body: data.msg,
+                                    //             buttons: [Dialog.okButton({ label: 'Ok' })]
+                                    //         }).then( result => {
+                                    //             if (result.button.accept ) {
+                                    //                 window.location.reload();
+                                    //             }
+                                    //         })
+                                    //         }
+                                    //     })
+                                    //     .catch(reason => {
+                                    //         showErrorMessage('Get Feedback Error', reason);
+                                    //         console.error(
+                                    //         `Failed to fetch recent feedbacks.\n${reason}`
+                                    //         );
+                                    //     });
+                                    // }, 60000);
                                 })
                                 .catch(reason => {
                                     (0, _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_1__.showErrorMessage)('Code Share Error', reason);
                                     console.error(`Failed to share code to server.\n${reason}`);
                                 });
                         };
                         const button = new _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_1__.ToolbarButton({
@@ -659,20 +688,23 @@
                     info,
                 }) => {
                     const shareCode = async () => {
                         if (isNaN(info.problem_id)) {
                             (0, _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_0__.showErrorMessage)('Code Share Error', "Invalid code block. Use specific problem notebook.");
                             return;
                         }
+                        // clear message skeleton
+                        info.message = info.message.replace("## Message to instructor: ", "");
                         let postBody = {
                             "message": info.message,
                             "code": cell.model.value.text,
-                            "problem_id": info.problem_id
+                            "problem_id": info.problem_id,
+                            "snapshot": 2
                         };
-                        // console.log("From widget: ", postBody)
+                        console.log("From widget: ", postBody);
                         (0, _handler__WEBPACK_IMPORTED_MODULE_3__.requestAPI)('submissions', {
                             method: 'POST',
                             body: JSON.stringify(postBody)
                         })
                         .then(data => {
                                 if (data.msg === "Submission saved successfully.") {
                                     if (info.message.length > 27) {
@@ -686,40 +718,40 @@
                                     body: data.msg,
                                     buttons: [_jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_0__.Dialog.okButton({
                                         label: 'Ok'
                                     })]
                                 });
                                 // Keep checking for new feedback.
                                 // This setInterval will be cleared once the feedback is downloaded (after reload())
-                                setInterval(function() {
-                                    // console.log("Checking for feedback...")
-                                    (0, _handler__WEBPACK_IMPORTED_MODULE_3__.requestAPI)('feedback', {
-                                        method: 'GET'
-                                    })
-                                    .then(data => {
-                                            // console.log(data);
-                                            if (data['hard-reload'] != -1) {
-                                                (0, _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_0__.showDialog)({
-                                                    title: '',
-                                                    body: data.msg,
-                                                    buttons: [_jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_0__.Dialog.okButton({
-                                                        label: 'Ok'
-                                                    })]
-                                                }).then(result => {
-                                                    if (result.button.accept) {
-                                                        window.location.reload();
-                                                    }
-                                                });
-                                            }
-                                        })
-                                        .catch(reason => {
-                                            (0, _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_0__.showErrorMessage)('Get Feedback Error', reason);
-                                            console.error(`Failed to fetch recent feedbacks.\n${reason}`);
-                                        });
-                                }, 60000);
+                                // setInterval(function(){
+                                //     // console.log("Checking for feedback...")
+                                //     requestAPI<any>('feedback',{
+                                //     method: 'GET'
+                                //     })
+                                //     .then(data => {
+                                //         // console.log(data);
+                                //         if (data['hard-reload'] != -1) {
+                                //         showDialog({
+                                //             title:'',
+                                //             body: data.msg,
+                                //             buttons: [Dialog.okButton({ label: 'Ok' })]
+                                //         }).then( result => {
+                                //             if (result.button.accept ) {
+                                //                 window.location.reload();
+                                //             }
+                                //         })
+                                //         }
+                                //     })
+                                //     .catch(reason => {
+                                //         showErrorMessage('Get Feedback Error', reason);
+                                //         console.error(
+                                //         `Failed to fetch recent feedbacks.\n${reason}`
+                                //         );
+                                //     });
+                                // }, 60000);
                             })
                             .catch(reason => {
                                 (0, _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_0__.showErrorMessage)('Code Share Error', reason);
                                 console.error(`Failed to share code to server.\n${reason}`);
                             });
                     };
                     return (react__WEBPACK_IMPORTED_MODULE_2___default().createElement("div", null,
@@ -747,8 +779,8 @@
 
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=lib_index_js.c3e6db586344d03a5551.js.map
+//# sourceMappingURL=lib_index_js.702cd083cba688e6ae07.js.map
```

### Comparing `carpo_student-0.0.8/carpo_student/labextension/static/lib_index_js.c3e6db586344d03a5551.js.map` & `carpo_student-0.0.9/carpo_student/labextension/static/lib_index_js.702cd083cba688e6ae07.js.map`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8035714285714286%*

 * *Differences: {"'file'": "'lib_index_js.702cd083cba688e6ae07.js'",*

 * * "'mappings'": "';;;;;;;;;;;;;;;;;;AAAwD;AACmC;AACpD;AAChC;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,oDAAU;AACtB;AACA,aAAa;AACb;AACA;AACA,gBAAgB,gEAAU;AAC1B;AACA;AACA,8BAA8B,iEAAe,GAAG,aAAa;AAC7D,iBAAiB;AACjB,aAAa;AACb;AACA,gBAAgB,sEAAgB;AAChC,mEAAmE,OAAO;AAC1E,aAAa;AACb;AACA,2BAA2B,+DAAa;AACxC;AACA;AACA;AACA;AACA,SAAS;AACT;AACA,mBAAmB,kEAAkB;AACrC;AACA,SAAS;AACT;AACA;;;;;;;;;;;;;;;;;;;ACxC+C;AACS;AACxD;AACA;AACA;AACA;AACA;AACA;AACA;AACO,kDAA […]*

```diff
@@ -1,21 +1,21 @@
 {
-    "file": "lib_index_js.c3e6db586344d03a5551.js",
-    "mappings": ";;;;;;;;;;;;;;;;;;AAAwD;AACmC;AACpD;AAChC;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,oDAAU;AACtB;AACA,aAAa;AACb;AACA;AACA,gBAAgB,gEAAU;AAC1B;AACA;AACA,8BAA8B,iEAAe,GAAG,aAAa;AAC7D,iBAAiB;AACjB,aAAa;AACb;AACA,gBAAgB,sEAAgB;AAChC,mEAAmE,OAAO;AAC1E,aAAa;AACb;AACA,2BAA2B,+DAAa;AACxC;AACA;AACA;AACA;AACA,SAAS;AACT;AACA,mBAAmB,kEAAkB;AACrC;AACA,SAAS;AACT;AACA;;;;;;;;;;;;;;;;;;;ACxC+C;AACS;AACxD;AACA;AACA;AACA;AACA;AACA;AACA;AACO,kDAAkD;AACzD;AACA,qBAAqB,+EAA6B;AAClD,uBAAuB,8DAAW;AAClC;AACA;AACA;AACA,yBAAyB,8EAA4B;AACrD;AACA;AACA,kBAAkB,+EAA6B;AAC/C;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,kBAAkB,gFAA8B;AAChD;AACA;AACA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AClCyD;AACd;AACoB;AACxB;AACiB;AACmC;AAC5C;AACK;AACpD;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,kEAAgB;AAC/B,eAAe,yEAAgB;AAC/B;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iCAAiC;AACjC;AACA,yBAAyB;AACzB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,qBAAqB;AACrB,+CAA+C,oDAAe;AAC9D;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iBAAiB;AACjB,aAAa;AACb,SAAS;AACT;AACA;AACA;AACA,2DAA2D,wDAAe;AAC1E;AACA,2DAA2D,6DAAiB;AAC5E;AACA;AACA;AACA;AACO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,oDAAU;AACtB;AACA,aAAa;AACb;AACA;AACA,gBAAgB,gEAAU;AAC1B;AACA;AACA,8BAA8B,iEAAe,GAAG,aAAa;AAC7D,iBAAiB;AACjB,aAAa;AACb;AACA,gBAAgB,sEAAgB;AAChC,sEAAsE,OAAO;AAC7E,aAAa;AACb;AACA,2BAA2B,+DAAa;AACxC;AACA;AACA;AACA;AACA,SAAS;AACT;AACA,mBAAmB,kEAAkB;AACrC;AACA,SAAS;AACT;AACA;AACO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,oDAAU;AACtB;AACA,aAAa;AACb;AACA;AACA,gBAAgB,gEAAU;AAC1B;AACA;AACA,8BAA8B,iEAAe,GAAG,aAAa;AAC7D,iBAAiB;AACjB,aAAa;AACb;AACA,gBAAgB,sEAAgB;AAChC,kEAAkE,OAAO;AACzE,aAAa;AACb;AACA,2BAA2B,+DAAa;AACxC;AACA;AACA;AACA;AACA,SAAS;AACT;AACA,mBAAmB,kEAAkB;AACrC;AACA,SAAS;AACT;AACA;AACO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,oDAAU;AACtB;AACA,aAAa;AACb;AACA;AACA,gBAAgB,gEAAU;AAC1B;AACA;AACA,8BAA8B,iEAAe,GAAG,aAAa;AAC7D,iBAAiB;AACjB;AACA;AACA;AACA,iBAAiB;AACjB,aAAa;AACb;AACA,gBAAgB,sEAAgB;AAChC,oEAAoE,OAAO;AAC3E,aAAa;AACb;AACA,2BAA2B,+DAAa;AACxC;AACA;AACA;AACA;AACA,SAAS;AACT;AACA,mBAAmB,kEAAkB;AACrC;AACA,SAAS;AACT;AACA;AACO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,oDAAU;AACtB;AACA,aAAa;AACb;AACA;AACA;AACA,aAAa;AACb;AACA,gBAAgB,sEAAgB;AAChC,4EAA4E,OAAO;AACnF,aAAa;AACb;AACA,2BAA2B,+DAAa;AACxC;AACA;AACA;AACA;AACA,SAAS;AACT;AACA,mBAAmB,kEAAkB;AACrC;AACA,SAAS;AACT;AACA;AACA;AACO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,oDAAU;AACtB;AACA,aAAa;AACb;AACA;AACA;AACA,aAAa;AACb;AACA,gBAAgB,sEAAgB;AAChC,iEAAiE,OAAO;AACxE,aAAa;AACb;AACA,2BAA2B,+DAAa;AACxC;AACA;AACA;AACA;AACA,SAAS;AACT;AACA,mBAAmB,kEAAkB;AACrC;AACA,SAAS;AACT;AACA;AACA,iEAAe,MAAM,EAAC;;;;;;;;;;;;;;;;;;;;AClRkC;AACmC;AACpD;AAChC;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACA,gBAAgB,sEAAgB;AAChC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,oDAAU;AACtB;AACA;AACA,aAAa;AACb;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,gBAAgB,gEAAU;AAC1B;AACA;AACA,8BAA8B,iEAAe,GAAG,aAAa;AAC7D,iBAAiB;AACjB;AACA;AACA;AACA;AACA,oBAAoB,oDAAU;AAC9B;AACA,qBAAqB;AACrB;AACA;AACA;AACA,4BAA4B,gEAAU;AACtC;AACA;AACA,0CAA0C,iEAAe,GAAG,aAAa;AACzE,6BAA6B;AAC7B;AACA;AACA;AACA,6BAA6B;AAC7B;AACA,qBAAqB;AACrB;AACA,wBAAwB,sEAAgB;AACxC,4EAA4E,OAAO;AACnF,qBAAqB;AACrB,iBAAiB;AACjB,aAAa;AACb;AACA,gBAAgB,sEAAgB;AAChC,kEAAkE,OAAO;AACzE,aAAa;AACb;AACA,2BAA2B,+DAAa;AACxC;AACA;AACA;AACA;AACA,SAAS;AACT;AACA,mBAAmB,kEAAkB;AACrC;AACA,SAAS;AACT;AACA;;;;;;;;;;;;;;;;;;;;;;ACnGmD;AACiB;AAC1C;AACa;AACqC;AAC5E,uBAAuB,eAAe,MAAM,0DAAmB,aAAa,mEAAmE;AAC/I,IAAI,0DAAmB,CAAC,2EAAoB,IAAI,sFAAsF;AACtI,mCAAmC,aAAa;AAChD;AACA;AACA,YAAY,sEAAgB;AAC5B;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,QAAQ,oDAAU;AAClB;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,gEAAU;AACtB;AACA;AACA,0BAA0B,iEAAe,GAAG,aAAa;AACzD,aAAa;AACb;AACA;AACA;AACA;AACA,gBAAgB,oDAAU;AAC1B;AACA,iBAAiB;AACjB;AACA;AACA;AACA,wBAAwB,gEAAU;AAClC;AACA;AACA,sCAAsC,iEAAe,GAAG,aAAa;AACrE,yBAAyB;AACzB;AACA;AACA;AACA,yBAAyB;AACzB;AACA,iBAAiB;AACjB;AACA,oBAAoB,sEAAgB;AACpC,wEAAwE,OAAO;AAC/E,iBAAiB;AACjB,aAAa;AACb,SAAS;AACT;AACA,YAAY,sEAAgB;AAC5B,8DAA8D,OAAO;AACrE,SAAS;AACT;AACA,YAAY,0DAAmB;AAC/B,QAAQ,0DAAmB,gBAAgB,MAAM,qEAAc,gCAAgC;AAC/F;AACO,8BAA8B,6DAAW;AAChD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,0DAAmB,4BAA4B,kCAAkC;AAChG;AACA",
+    "file": "lib_index_js.702cd083cba688e6ae07.js",
+    "mappings": ";;;;;;;;;;;;;;;;;;AAAwD;AACmC;AACpD;AAChC;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,oDAAU;AACtB;AACA,aAAa;AACb;AACA;AACA,gBAAgB,gEAAU;AAC1B;AACA;AACA,8BAA8B,iEAAe,GAAG,aAAa;AAC7D,iBAAiB;AACjB,aAAa;AACb;AACA,gBAAgB,sEAAgB;AAChC,mEAAmE,OAAO;AAC1E,aAAa;AACb;AACA,2BAA2B,+DAAa;AACxC;AACA;AACA;AACA;AACA,SAAS;AACT;AACA,mBAAmB,kEAAkB;AACrC;AACA,SAAS;AACT;AACA;;;;;;;;;;;;;;;;;;;ACxC+C;AACS;AACxD;AACA;AACA;AACA;AACA;AACA;AACA;AACO,kDAAkD;AACzD;AACA,qBAAqB,+EAA6B;AAClD,uBAAuB,8DAAW;AAClC;AACA;AACA;AACA,yBAAyB,8EAA4B;AACrD;AACA;AACA,kBAAkB,+EAA6B;AAC/C;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,kBAAkB,gFAA8B;AAChD;AACA;AACA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AClCyD;AACd;AACoB;AACxB;AACiB;AACmC;AAC5C;AACK;AACpD;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,kEAAgB;AAC/B,eAAe,yEAAgB;AAC/B;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iCAAiC;AACjC;AACA,yBAAyB;AACzB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,2DAA2D,oDAAe;AAC1E;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,wCAAwC,oDAAU;AAClD;AACA;AACA,yCAAyC;AACzC;AACA;AACA,yCAAyC;AACzC,qCAAqC;AACrC;AACA;AACA;AACA;AACA,qBAAqB;AACrB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iBAAiB;AACjB,aAAa;AACb,SAAS;AACT;AACA;AACA;AACA,2DAA2D,wDAAe;AAC1E;AACA,2DAA2D,6DAAiB;AAC5E;AACA;AACA;AACA;AACO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,oDAAU;AACtB;AACA,aAAa;AACb;AACA;AACA,gBAAgB,gEAAU;AAC1B;AACA;AACA,8BAA8B,iEAAe,GAAG,aAAa;AAC7D,iBAAiB;AACjB,aAAa;AACb;AACA,gBAAgB,sEAAgB;AAChC,sEAAsE,OAAO;AAC7E,aAAa;AACb;AACA,2BAA2B,+DAAa;AACxC;AACA;AACA;AACA;AACA,SAAS;AACT;AACA,mBAAmB,kEAAkB;AACrC;AACA,SAAS;AACT;AACA;AACO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,oDAAU;AACtB;AACA,aAAa;AACb;AACA;AACA,gBAAgB,gEAAU;AAC1B;AACA;AACA,8BAA8B,iEAAe,GAAG,aAAa;AAC7D,iBAAiB;AACjB,aAAa;AACb;AACA,gBAAgB,sEAAgB;AAChC,kEAAkE,OAAO;AACzE,aAAa;AACb;AACA,2BAA2B,+DAAa;AACxC;AACA;AACA;AACA;AACA,SAAS;AACT;AACA,mBAAmB,kEAAkB;AACrC;AACA,SAAS;AACT;AACA;AACO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,oDAAU;AACtB;AACA,aAAa;AACb;AACA;AACA,gBAAgB,gEAAU;AAC1B;AACA;AACA,8BAA8B,iEAAe,GAAG,aAAa;AAC7D,iBAAiB;AACjB;AACA;AACA;AACA,iBAAiB;AACjB,aAAa;AACb;AACA,gBAAgB,sEAAgB;AAChC,oEAAoE,OAAO;AAC3E,aAAa;AACb;AACA,2BAA2B,+DAAa;AACxC;AACA;AACA;AACA;AACA,SAAS;AACT;AACA,mBAAmB,kEAAkB;AACrC;AACA,SAAS;AACT;AACA;AACO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,oDAAU;AACtB;AACA,aAAa;AACb;AACA;AACA;AACA,aAAa;AACb;AACA,gBAAgB,sEAAgB;AAChC,4EAA4E,OAAO;AACnF,aAAa;AACb;AACA,2BAA2B,+DAAa;AACxC;AACA;AACA;AACA;AACA,SAAS;AACT;AACA,mBAAmB,kEAAkB;AACrC;AACA,SAAS;AACT;AACA;AACA;AACO;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,oDAAU;AACtB;AACA,aAAa;AACb;AACA;AACA;AACA,aAAa;AACb;AACA,gBAAgB,sEAAgB;AAChC,iEAAiE,OAAO;AACxE,aAAa;AACb;AACA,2BAA2B,+DAAa;AACxC;AACA;AACA;AACA;AACA,SAAS;AACT;AACA,mBAAmB,kEAAkB;AACrC;AACA,SAAS;AACT;AACA;AACA,iEAAe,MAAM,EAAC;;;;;;;;;;;;;;;;;;;;AC9SkC;AACmC;AACpD;AAChC;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACA,gBAAgB,sEAAgB;AAChC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,oDAAU;AACtB;AACA;AACA,aAAa;AACb;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,gBAAgB,gEAAU;AAC1B;AACA;AACA,8BAA8B,iEAAe,GAAG,aAAa;AAC7D,iBAAiB;AACjB;AACA;AACA;AACA;AACA;AACA;AACA,wBAAwB;AACxB;AACA;AACA;AACA;AACA;AACA;AACA,2DAA2D,aAAa;AACxE,4BAA4B;AAC5B;AACA;AACA;AACA,4BAA4B;AAC5B;AACA,wBAAwB;AACxB;AACA;AACA;AACA,iEAAiE,OAAO;AACxE;AACA,wBAAwB;AACxB,oBAAoB;AACpB,aAAa;AACb;AACA,gBAAgB,sEAAgB;AAChC,kEAAkE,OAAO;AACzE,aAAa;AACb;AACA,2BAA2B,+DAAa;AACxC;AACA;AACA;AACA;AACA,SAAS;AACT;AACA,mBAAmB,kEAAkB;AACrC;AACA,SAAS;AACT;AACA;;;;;;;;;;;;;;;;;;;;;;ACtGmD;AACiB;AAC1C;AACa;AACqC;AAC5E,uBAAuB,eAAe,MAAM,0DAAmB,aAAa,mEAAmE;AAC/I,IAAI,0DAAmB,CAAC,2EAAoB,IAAI,sFAAsF;AACtI,mCAAmC,aAAa;AAChD;AACA;AACA,YAAY,sEAAgB;AAC5B;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,QAAQ,oDAAU;AAClB;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,gEAAU;AACtB;AACA;AACA,0BAA0B,iEAAe,GAAG,aAAa;AACzD,aAAa;AACb;AACA;AACA;AACA;AACA;AACA;AACA,oBAAoB;AACpB;AACA;AACA;AACA;AACA;AACA;AACA,uDAAuD,aAAa;AACpE,wBAAwB;AACxB;AACA;AACA;AACA,wBAAwB;AACxB;AACA,oBAAoB;AACpB;AACA;AACA;AACA,6DAA6D,OAAO;AACpE;AACA,oBAAoB;AACpB,gBAAgB;AAChB,SAAS;AACT;AACA,YAAY,sEAAgB;AAC5B,8DAA8D,OAAO;AACrE,SAAS;AACT;AACA,YAAY,0DAAmB;AAC/B,QAAQ,0DAAmB,gBAAgB,MAAM,qEAAc,gCAAgC;AAC/F;AACO,8BAA8B,6DAAW;AAChD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,0DAAmB,4BAA4B,kCAAkC;AAChG;AACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://carpo-student/./lib/get-solutions.js",
         "webpack://carpo-student/./lib/handler.js",
         "webpack://carpo-student/./lib/index.js",
         "webpack://carpo-student/./lib/share-code.js",
         "webpack://carpo-student/./lib/widget.js"
     ],
     "sourcesContent": [
         "import { DisposableDelegate } from '@lumino/disposable';\nimport { ToolbarButton, Dialog, showDialog, showErrorMessage } from '@jupyterlab/apputils';\nimport { requestAPI } from './handler';\nexport class GetSolutionButton {\n    /**\n     * Create a new extension for the notebook panel widget.\n     *\n     * @param panel Notebook panel\n     * @param context Notebook context\n     * @returns Disposable on the added button\n     */\n    createNew(panel, context) {\n        const getSolutions = () => {\n            requestAPI('solution', {\n                method: 'GET'\n            })\n                .then(data => {\n                console.log(data);\n                showDialog({\n                    title: '',\n                    body: data.msg,\n                    buttons: [Dialog.okButton({ label: 'Ok' })]\n                });\n            })\n                .catch(reason => {\n                showErrorMessage('Get Solution Error', reason);\n                console.error(`Failed to get problem solutions.\\n${reason}`);\n            });\n        };\n        const button = new ToolbarButton({\n            className: 'get-solution-button',\n            label: 'GetSolutions',\n            onClick: getSolutions,\n            tooltip: 'Download solutions to problems.',\n        });\n        panel.toolbar.insertItem(14, 'getSolutions', button);\n        return new DisposableDelegate(() => {\n            button.dispose();\n        });\n    }\n}\n",
         "import { URLExt } from '@jupyterlab/coreutils';\nimport { ServerConnection } from '@jupyterlab/services';\n/**\n * Call the API extension\n *\n * @param endPoint API REST end point for the extension\n * @param init Initial values for the request\n * @returns The response body interpreted as JSON\n */\nexport async function requestAPI(endPoint = '', init = {}) {\n    // Make request to Jupyter API\n    const settings = ServerConnection.makeSettings();\n    const requestUrl = URLExt.join(settings.baseUrl, 'carpo-student', // API Namespace\n    endPoint);\n    let response;\n    try {\n        response = await ServerConnection.makeRequest(requestUrl, init, settings);\n    }\n    catch (error) {\n        throw new ServerConnection.NetworkError(error);\n    }\n    let data = await response.text();\n    if (data.length > 0) {\n        try {\n            data = JSON.parse(data);\n        }\n        catch (error) {\n            console.log('Not a JSON response body.', response);\n        }\n    }\n    if (!response.ok) {\n        throw new ServerConnection.ResponseError(response, data.message || data);\n    }\n    return data;\n}\n",
-        "import { INotebookTracker, } from '@jupyterlab/notebook';\nimport { CellCheckButton } from './widget';\nimport { ISettingRegistry } from '@jupyterlab/settingregistry';\nimport { requestAPI } from './handler';\nimport { DisposableDelegate } from '@lumino/disposable';\nimport { ToolbarButton, Dialog, showDialog, showErrorMessage } from '@jupyterlab/apputils';\nimport { ShareCodeButton } from './share-code';\nimport { GetSolutionButton } from './get-solutions';\n/**\n * Initialization data for the carpo-student extension.\n */\nconst plugin = {\n    id: 'carpo-student:plugin',\n    autoStart: true,\n    requires: [INotebookTracker],\n    optional: [ISettingRegistry],\n    activate: (app, nbTrack, settingRegistry) => {\n        console.log('JupyterLab extension carpo-student is activated!');\n        nbTrack.currentChanged.connect(() => {\n            console.log(\"->: \", nbTrack.currentWidget.context.path);\n            const notebookPanel = nbTrack.currentWidget;\n            const notebook = nbTrack.currentWidget.content;\n            const filename = notebookPanel.context.path;\n            // Disable Code Share functionality if inside Feedback directory\n            if (filename.includes(\"Feedback\")) {\n                return;\n            }\n            // Disable if not inside Exercises directory\n            if (!filename.includes(\"Exercises\")) {\n                return;\n            }\n            notebookPanel.context.ready.then(async () => {\n                let currentCell = null;\n                let currentCellCheckButton = null;\n                nbTrack.activeCellChanged.connect(() => {\n                    var question;\n                    if (currentCell) {\n                        notebook.widgets.map((c) => {\n                            if (c.model.type == 'code' || c.model.type == 'markdown') {\n                                const currentLayout = c.layout;\n                                currentLayout.widgets.map(w => {\n                                    if (w === currentCellCheckButton) {\n                                        currentLayout.removeWidget(w);\n                                    }\n                                });\n                            }\n                        });\n                    }\n                    const cell = notebook.activeCell;\n                    const activeIndex = notebook.activeCellIndex;\n                    var info = {\n                        problem_id: parseInt((filename.split(\"/\").pop()).replace(\"ex\", \"\").replace(\".ipynb\", \"\"))\n                    };\n                    // Get the message block referencing the active cell.\n                    notebook.widgets.map((c, index) => {\n                        if (c.model.value.text.startsWith(\"## Message to instructor:\")) {\n                            info.message = c.model.value.text;\n                        }\n                        if (index == activeIndex) {\n                            question = c.model.value.text;\n                        }\n                    });\n                    const newCheckButton = new CellCheckButton(cell, info);\n                    if (question.includes(\"## PID \")) {\n                        cell.layout.addWidget(newCheckButton);\n                        currentCellCheckButton = newCheckButton;\n                    }\n                    // Set the current cell and button for future\n                    // reference\n                    currentCell = cell;\n                });\n            });\n        });\n        //  tell the document registry about your widget extension:\n        app.docRegistry.addWidgetExtension('Notebook', new RegisterButton());\n        app.docRegistry.addWidgetExtension('Notebook', new GetQuestionButton());\n        app.docRegistry.addWidgetExtension('Notebook', new ShareCodeButton());\n        app.docRegistry.addWidgetExtension('Notebook', new GetFeedbackButton());\n        app.docRegistry.addWidgetExtension('Notebook', new GetSolutionButton());\n        app.docRegistry.addWidgetExtension('Notebook', new ViewSubmissionStatusButton());\n        // app.docRegistry.addWidgetExtension('Notebook', new viewProblemStatusExtension());\n    }\n};\nexport class RegisterButton {\n    /**\n     * Create a new extension for the notebook panel widget.\n     *\n     * @param panel Notebook panel\n     * @param context Notebook context\n     * @returns Disposable on the added button\n     */\n    createNew(panel, context) {\n        const register = () => {\n            // NotebookActions.clearAllOutputs(panel.content);\n            // const notebook = panel.content;\n            requestAPI('register', {\n                method: 'GET'\n            })\n                .then(data => {\n                console.log(data);\n                showDialog({\n                    title: '',\n                    body: \"Student \" + data.name + \" has been registered.\",\n                    buttons: [Dialog.okButton({ label: 'Ok' })]\n                });\n            })\n                .catch(reason => {\n                showErrorMessage('Registration Error', reason);\n                console.error(`Failed to register user as Student.\\n${reason}`);\n            });\n        };\n        const button = new ToolbarButton({\n            className: 'register-button',\n            label: 'Register',\n            onClick: register,\n            tooltip: 'Register as a Student',\n        });\n        panel.toolbar.insertItem(10, 'register', button);\n        return new DisposableDelegate(() => {\n            button.dispose();\n        });\n    }\n}\nexport class GetQuestionButton {\n    /**\n     * Create a new extension for the notebook panel widget.\n     *\n     * @param panel Notebook panel\n     * @param context Notebook context\n     * @returns Disposable on the added button\n     */\n    createNew(panel, context) {\n        const getQuestion = () => {\n            // NotebookActions.clearAllOutputs(panel.content);\n            // const notebook = panel.content;\n            requestAPI('question', {\n                method: 'GET'\n            })\n                .then(data => {\n                console.log(data);\n                showDialog({\n                    title: '',\n                    body: data.msg,\n                    buttons: [Dialog.okButton({ label: 'Ok' })]\n                });\n            })\n                .catch(reason => {\n                showErrorMessage('Get Problem Error', reason);\n                console.error(`Failed to get active questions.\\n${reason}`);\n            });\n        };\n        const button = new ToolbarButton({\n            className: 'get-question-button',\n            label: 'GetProblem',\n            onClick: getQuestion,\n            tooltip: 'Get Latest Problem From Server',\n        });\n        panel.toolbar.insertItem(11, 'getQuestion', button);\n        return new DisposableDelegate(() => {\n            button.dispose();\n        });\n    }\n}\nexport class GetFeedbackButton {\n    /**\n     * Create a new extension for the notebook panel widget.\n     *\n     * @param panel Notebook panel\n     * @param context Notebook context\n     * @returns Disposable on the added button\n     */\n    createNew(panel, context) {\n        const getFeedback = () => {\n            requestAPI('feedback', {\n                method: 'GET'\n            })\n                .then(data => {\n                console.log(data);\n                showDialog({\n                    title: '',\n                    body: data.msg,\n                    buttons: [Dialog.okButton({ label: 'Ok' })]\n                }).then(result => {\n                    if (result.button.accept && data['hard-reload'] == 1) {\n                        window.location.reload();\n                    }\n                });\n            })\n                .catch(reason => {\n                showErrorMessage('Get Feedback Error', reason);\n                console.error(`Failed to fetch recent feedbacks.\\n${reason}`);\n            });\n        };\n        const button = new ToolbarButton({\n            className: 'get-feedback-button',\n            label: 'GetFeedback',\n            onClick: getFeedback,\n            tooltip: 'Get Feedback to your Submission',\n        });\n        panel.toolbar.insertItem(13, 'getFeedback', button);\n        return new DisposableDelegate(() => {\n            button.dispose();\n        });\n    }\n}\nexport class ViewSubmissionStatusButton {\n    /**\n     * Create a new extension for the notebook panel widget.\n     *\n     * @param panel Notebook panel\n     * @param context Notebook context\n     * @returns Disposable on the added button\n     */\n    createNew(panel, context) {\n        const viewStatus = () => {\n            requestAPI('view_student_status', {\n                method: 'GET'\n            })\n                .then(data => {\n                console.log(data);\n                window.open(data.url, \"_blank\");\n            })\n                .catch(reason => {\n                showErrorMessage('View Status Error', reason);\n                console.error(`Failed to view student submission status.\\n${reason}`);\n            });\n        };\n        const button = new ToolbarButton({\n            className: 'get-status-button',\n            label: 'Status',\n            onClick: viewStatus,\n            tooltip: 'View your submissions status',\n        });\n        panel.toolbar.insertItem(14, 'viewStatus', button);\n        return new DisposableDelegate(() => {\n            button.dispose();\n        });\n    }\n}\n// Currently disabled\nexport class viewProblemStatusExtension {\n    /**\n     * Create a new extension for the notebook panel widget.\n     *\n     * @param panel Notebook panel\n     * @param context Notebook context\n     * @returns Disposable on the added button\n     */\n    createNew(panel, context) {\n        const viewProblemStatus = () => {\n            requestAPI('view_problem_list', {\n                method: 'GET'\n            })\n                .then(data => {\n                console.log(data);\n                window.open(data.url, \"_blank\");\n            })\n                .catch(reason => {\n                showErrorMessage('View Problem Status Error', reason);\n                console.error(`Failed to view problem status.\\n${reason}`);\n            });\n        };\n        const button = new ToolbarButton({\n            className: 'get-status-button',\n            label: 'Problems',\n            onClick: viewProblemStatus,\n            tooltip: 'View all problem status',\n        });\n        panel.toolbar.insertItem(15, 'viewProblemStatus', button);\n        return new DisposableDelegate(() => {\n            button.dispose();\n        });\n    }\n}\nexport default plugin;\n",
-        "import { DisposableDelegate } from '@lumino/disposable';\nimport { ToolbarButton, Dialog, showDialog, showErrorMessage } from '@jupyterlab/apputils';\nimport { requestAPI } from './handler';\nexport class ShareCodeButton {\n    /**\n     * Create a new extension for the notebook panel widget.\n     *\n     * @param panel Notebook panel\n     * @param context Notebook context\n     * @returns Disposable on the added button\n     */\n    createNew(panel, context) {\n        const shareCode = () => {\n            const notebook = panel.content;\n            const filename = panel.context.path;\n            const activeIndex = notebook.activeCellIndex;\n            var codeBlock;\n            var info = {\n                problem_id: parseInt((filename.split(\"/\").pop()).replace(\"ex\", \"\").replace(\".ipynb\", \"\"))\n            };\n            notebook.widgets.map((c, index) => {\n                if (c.model.value.text.startsWith(\"## Message to instructor:\")) {\n                    info.message = c.model.value.text;\n                }\n                if (index == activeIndex) {\n                    codeBlock = c.model.value.text;\n                }\n            });\n            if (!codeBlock.startsWith(\"## PID \")) {\n                showErrorMessage('Code Share Error', \"Invalid cell selected. Use a specific problem cell block.\");\n                return;\n            }\n            let postBody = {\n                \"message\": info.message,\n                \"code\": codeBlock,\n                \"problem_id\": info.problem_id\n            };\n            console.log(\"Req body: \", postBody);\n            requestAPI('submissions', {\n                method: 'POST',\n                body: JSON.stringify(postBody)\n            })\n                .then(data => {\n                if (data.msg === \"Submission saved successfully.\") {\n                    if (info.message.length > 27) {\n                        data.msg = 'Code & message is sent to the instructor.';\n                    }\n                    else {\n                        data.msg = 'Code is sent to the instructor.';\n                    }\n                }\n                showDialog({\n                    title: '',\n                    body: data.msg,\n                    buttons: [Dialog.okButton({ label: 'Ok' })]\n                });\n                // Keep checking for new feedback.\n                // This setInterval will be cleared once the feedback is downloaded (after reload())\n                setInterval(function () {\n                    // console.log(\"Checking for feedback...\")\n                    requestAPI('feedback', {\n                        method: 'GET'\n                    })\n                        .then(data => {\n                        // console.log(data);\n                        if (data['hard-reload'] != -1) {\n                            showDialog({\n                                title: '',\n                                body: data.msg,\n                                buttons: [Dialog.okButton({ label: 'Ok' })]\n                            }).then(result => {\n                                if (result.button.accept) {\n                                    window.location.reload();\n                                }\n                            });\n                        }\n                    })\n                        .catch(reason => {\n                        showErrorMessage('Get Feedback Error', reason);\n                        console.error(`Failed to fetch recent feedbacks.\\n${reason}`);\n                    });\n                }, 60000);\n            })\n                .catch(reason => {\n                showErrorMessage('Code Share Error', reason);\n                console.error(`Failed to share code to server.\\n${reason}`);\n            });\n        };\n        const button = new ToolbarButton({\n            className: 'share-code-button',\n            label: 'ShareCode',\n            onClick: shareCode,\n            tooltip: 'Share your code to the instructor.',\n        });\n        panel.toolbar.insertItem(12, 'shareCode', button);\n        return new DisposableDelegate(() => {\n            button.dispose();\n        });\n    }\n}\n",
-        "import { ReactWidget } from '@jupyterlab/apputils';\nimport { fileUploadIcon, LabIcon } from '@jupyterlab/ui-components';\nimport React from 'react';\nimport { requestAPI } from './handler';\nimport { Dialog, showDialog, showErrorMessage } from '@jupyterlab/apputils';\nconst ShareButton = ({ icon, onClick }) => (React.createElement(\"button\", { type: \"button\", onClick: () => onClick(), className: \"cellButton\" },\n    React.createElement(LabIcon.resolveReact, { icon: icon, className: \"cellButton-icon\", tag: \"span\", width: \"15px\", height: \"15px\" })));\nconst CodeCellButtonComponent = ({ cell, info, }) => {\n    const shareCode = async () => {\n        if (isNaN(info.problem_id)) {\n            showErrorMessage('Code Share Error', \"Invalid code block. Use specific problem notebook.\");\n            return;\n        }\n        let postBody = {\n            \"message\": info.message,\n            \"code\": cell.model.value.text,\n            \"problem_id\": info.problem_id\n        };\n        // console.log(\"From widget: \", postBody)\n        requestAPI('submissions', {\n            method: 'POST',\n            body: JSON.stringify(postBody)\n        })\n            .then(data => {\n            if (data.msg === \"Submission saved successfully.\") {\n                if (info.message.length > 27) {\n                    data.msg = 'Code & message is sent to the instructor.';\n                }\n                else {\n                    data.msg = 'Code is sent to the instructor.';\n                }\n            }\n            showDialog({\n                title: '',\n                body: data.msg,\n                buttons: [Dialog.okButton({ label: 'Ok' })]\n            });\n            // Keep checking for new feedback.\n            // This setInterval will be cleared once the feedback is downloaded (after reload())\n            setInterval(function () {\n                // console.log(\"Checking for feedback...\")\n                requestAPI('feedback', {\n                    method: 'GET'\n                })\n                    .then(data => {\n                    // console.log(data);\n                    if (data['hard-reload'] != -1) {\n                        showDialog({\n                            title: '',\n                            body: data.msg,\n                            buttons: [Dialog.okButton({ label: 'Ok' })]\n                        }).then(result => {\n                            if (result.button.accept) {\n                                window.location.reload();\n                            }\n                        });\n                    }\n                })\n                    .catch(reason => {\n                    showErrorMessage('Get Feedback Error', reason);\n                    console.error(`Failed to fetch recent feedbacks.\\n${reason}`);\n                });\n            }, 60000);\n        })\n            .catch(reason => {\n            showErrorMessage('Code Share Error', reason);\n            console.error(`Failed to share code to server.\\n${reason}`);\n        });\n    };\n    return (React.createElement(\"div\", null,\n        React.createElement(ShareButton, { icon: fileUploadIcon, onClick: () => (shareCode)() })));\n};\nexport class CellCheckButton extends ReactWidget {\n    constructor(cell, info) {\n        super();\n        this.cell = null;\n        this.info = null;\n        this.cell = cell;\n        this.info = info;\n        this.addClass('jp-CellButton');\n    }\n    render() {\n        return React.createElement(CodeCellButtonComponent, { cell: this.cell, info: this.info });\n    }\n}\n"
+        "import { INotebookTracker, } from '@jupyterlab/notebook';\nimport { CellCheckButton } from './widget';\nimport { ISettingRegistry } from '@jupyterlab/settingregistry';\nimport { requestAPI } from './handler';\nimport { DisposableDelegate } from '@lumino/disposable';\nimport { ToolbarButton, Dialog, showDialog, showErrorMessage } from '@jupyterlab/apputils';\nimport { ShareCodeButton } from './share-code';\nimport { GetSolutionButton } from './get-solutions';\n/**\n * Initialization data for the carpo-student extension.\n */\nconst plugin = {\n    id: 'carpo-student:plugin',\n    autoStart: true,\n    requires: [INotebookTracker],\n    optional: [ISettingRegistry],\n    activate: (app, nbTrack, settingRegistry) => {\n        console.log('JupyterLab extension carpo-student is activated!');\n        // var interval => (); \n        var counter = 0;\n        nbTrack.currentChanged.connect(() => {\n            console.log(\"my counter: \", counter);\n            const notebookPanel = nbTrack.currentWidget;\n            const notebook = nbTrack.currentWidget.content;\n            const filename = notebookPanel.context.path;\n            // Disable Code Share functionality if inside Feedback directory\n            if (filename.includes(\"Feedback\")) {\n                return;\n            }\n            // Disable if not inside Exercises directory\n            if (!filename.includes(\"Exercises\")) {\n                return;\n            }\n            notebookPanel.context.ready.then(async () => {\n                let currentCell = null;\n                let currentCellCheckButton = null;\n                nbTrack.activeCellChanged.connect(() => {\n                    var question;\n                    if (currentCell) {\n                        notebook.widgets.map((c) => {\n                            if (c.model.type == 'code' || c.model.type == 'markdown') {\n                                const currentLayout = c.layout;\n                                currentLayout.widgets.map(w => {\n                                    if (w === currentCellCheckButton) {\n                                        currentLayout.removeWidget(w);\n                                    }\n                                });\n                            }\n                        });\n                    }\n                    const cell = notebook.activeCell;\n                    const activeIndex = notebook.activeCellIndex;\n                    var info = {\n                        problem_id: parseInt((filename.split(\"/\").pop()).replace(\"ex\", \"\").replace(\".ipynb\", \"\"))\n                    };\n                    // Get the message block referencing the active cell.\n                    notebook.widgets.map((c, index) => {\n                        if (c.model.value.text.startsWith(\"## Message to instructor:\")) {\n                            info.message = c.model.value.text;\n                        }\n                        if (index == activeIndex) {\n                            question = c.model.value.text;\n                            if (question.includes(\"## PID \")) {\n                                const newCheckButton = new CellCheckButton(cell, info);\n                                cell.layout.addWidget(newCheckButton);\n                                currentCellCheckButton = newCheckButton;\n                                // Send code snapshot to the server:\n                                if (counter == 0) {\n                                    setInterval(function () {\n                                        // console.log(\"Update: \", c.model.value.text)\n                                        let postBody = {\n                                            \"message\": \"\",\n                                            \"code\": c.model.value.text,\n                                            \"problem_id\": info.problem_id,\n                                            \"snapshot\": 1\n                                        };\n                                        // console.log(\"From widget: \", postBody)\n                                        requestAPI('submissions', {\n                                            method: 'POST',\n                                            body: JSON.stringify(postBody)\n                                        })\n                                            .then(data => {\n                                            console.log(\"Snapshot sent.\", data);\n                                        });\n                                    }, 10000);\n                                    counter++;\n                                }\n                            }\n                        }\n                    });\n                    // const newCheckButton: CellCheckButton = new CellCheckButton(cell,info);\n                    // if (question.includes(\"## PID \")){\n                    //   (cell.layout as PanelLayout).addWidget(newCheckButton);\n                    //   currentCellCheckButton = newCheckButton;\n                    // }\n                    // Set the current cell and button for future\n                    // reference\n                    currentCell = cell;\n                });\n            });\n        });\n        //  tell the document registry about your widget extension:\n        app.docRegistry.addWidgetExtension('Notebook', new RegisterButton());\n        app.docRegistry.addWidgetExtension('Notebook', new GetQuestionButton());\n        app.docRegistry.addWidgetExtension('Notebook', new ShareCodeButton());\n        app.docRegistry.addWidgetExtension('Notebook', new GetFeedbackButton());\n        app.docRegistry.addWidgetExtension('Notebook', new GetSolutionButton());\n        app.docRegistry.addWidgetExtension('Notebook', new ViewSubmissionStatusButton());\n        // app.docRegistry.addWidgetExtension('Notebook', new viewProblemStatusExtension());\n    }\n};\nexport class RegisterButton {\n    /**\n     * Create a new extension for the notebook panel widget.\n     *\n     * @param panel Notebook panel\n     * @param context Notebook context\n     * @returns Disposable on the added button\n     */\n    createNew(panel, context) {\n        const register = () => {\n            // NotebookActions.clearAllOutputs(panel.content);\n            // const notebook = panel.content;\n            requestAPI('register', {\n                method: 'GET'\n            })\n                .then(data => {\n                console.log(data);\n                showDialog({\n                    title: '',\n                    body: \"Student \" + data.name + \" has been registered.\",\n                    buttons: [Dialog.okButton({ label: 'Ok' })]\n                });\n            })\n                .catch(reason => {\n                showErrorMessage('Registration Error', reason);\n                console.error(`Failed to register user as Student.\\n${reason}`);\n            });\n        };\n        const button = new ToolbarButton({\n            className: 'register-button',\n            label: 'Register',\n            onClick: register,\n            tooltip: 'Register as a Student',\n        });\n        panel.toolbar.insertItem(10, 'register', button);\n        return new DisposableDelegate(() => {\n            button.dispose();\n        });\n    }\n}\nexport class GetQuestionButton {\n    /**\n     * Create a new extension for the notebook panel widget.\n     *\n     * @param panel Notebook panel\n     * @param context Notebook context\n     * @returns Disposable on the added button\n     */\n    createNew(panel, context) {\n        const getQuestion = () => {\n            // NotebookActions.clearAllOutputs(panel.content);\n            // const notebook = panel.content;\n            requestAPI('question', {\n                method: 'GET'\n            })\n                .then(data => {\n                console.log(data);\n                showDialog({\n                    title: '',\n                    body: data.msg,\n                    buttons: [Dialog.okButton({ label: 'Ok' })]\n                });\n            })\n                .catch(reason => {\n                showErrorMessage('Get Problem Error', reason);\n                console.error(`Failed to get active questions.\\n${reason}`);\n            });\n        };\n        const button = new ToolbarButton({\n            className: 'get-question-button',\n            label: 'GetProblem',\n            onClick: getQuestion,\n            tooltip: 'Get Latest Problem From Server',\n        });\n        panel.toolbar.insertItem(11, 'getQuestion', button);\n        return new DisposableDelegate(() => {\n            button.dispose();\n        });\n    }\n}\nexport class GetFeedbackButton {\n    /**\n     * Create a new extension for the notebook panel widget.\n     *\n     * @param panel Notebook panel\n     * @param context Notebook context\n     * @returns Disposable on the added button\n     */\n    createNew(panel, context) {\n        const getFeedback = () => {\n            requestAPI('feedback', {\n                method: 'GET'\n            })\n                .then(data => {\n                console.log(data);\n                showDialog({\n                    title: '',\n                    body: data.msg,\n                    buttons: [Dialog.okButton({ label: 'Ok' })]\n                }).then(result => {\n                    if (result.button.accept && data['hard-reload'] == 1) {\n                        window.location.reload();\n                    }\n                });\n            })\n                .catch(reason => {\n                showErrorMessage('Get Feedback Error', reason);\n                console.error(`Failed to fetch recent feedbacks.\\n${reason}`);\n            });\n        };\n        const button = new ToolbarButton({\n            className: 'get-feedback-button',\n            label: 'GetFeedback',\n            onClick: getFeedback,\n            tooltip: 'Get Feedback to your Submission',\n        });\n        panel.toolbar.insertItem(13, 'getFeedback', button);\n        return new DisposableDelegate(() => {\n            button.dispose();\n        });\n    }\n}\nexport class ViewSubmissionStatusButton {\n    /**\n     * Create a new extension for the notebook panel widget.\n     *\n     * @param panel Notebook panel\n     * @param context Notebook context\n     * @returns Disposable on the added button\n     */\n    createNew(panel, context) {\n        const viewStatus = () => {\n            requestAPI('view_student_status', {\n                method: 'GET'\n            })\n                .then(data => {\n                console.log(data);\n                window.open(data.url, \"_blank\");\n            })\n                .catch(reason => {\n                showErrorMessage('View Status Error', reason);\n                console.error(`Failed to view student submission status.\\n${reason}`);\n            });\n        };\n        const button = new ToolbarButton({\n            className: 'get-status-button',\n            label: 'Status',\n            onClick: viewStatus,\n            tooltip: 'View your submissions status',\n        });\n        panel.toolbar.insertItem(14, 'viewStatus', button);\n        return new DisposableDelegate(() => {\n            button.dispose();\n        });\n    }\n}\n// Currently disabled\nexport class viewProblemStatusExtension {\n    /**\n     * Create a new extension for the notebook panel widget.\n     *\n     * @param panel Notebook panel\n     * @param context Notebook context\n     * @returns Disposable on the added button\n     */\n    createNew(panel, context) {\n        const viewProblemStatus = () => {\n            requestAPI('view_problem_list', {\n                method: 'GET'\n            })\n                .then(data => {\n                console.log(data);\n                window.open(data.url, \"_blank\");\n            })\n                .catch(reason => {\n                showErrorMessage('View Problem Status Error', reason);\n                console.error(`Failed to view problem status.\\n${reason}`);\n            });\n        };\n        const button = new ToolbarButton({\n            className: 'get-status-button',\n            label: 'Problems',\n            onClick: viewProblemStatus,\n            tooltip: 'View all problem status',\n        });\n        panel.toolbar.insertItem(15, 'viewProblemStatus', button);\n        return new DisposableDelegate(() => {\n            button.dispose();\n        });\n    }\n}\nexport default plugin;\n",
+        "import { DisposableDelegate } from '@lumino/disposable';\nimport { ToolbarButton, Dialog, showDialog, showErrorMessage } from '@jupyterlab/apputils';\nimport { requestAPI } from './handler';\nexport class ShareCodeButton {\n    /**\n     * Create a new extension for the notebook panel widget.\n     *\n     * @param panel Notebook panel\n     * @param context Notebook context\n     * @returns Disposable on the added button\n     */\n    createNew(panel, context) {\n        const shareCode = () => {\n            const notebook = panel.content;\n            const filename = panel.context.path;\n            const activeIndex = notebook.activeCellIndex;\n            var codeBlock;\n            var info = {\n                problem_id: parseInt((filename.split(\"/\").pop()).replace(\"ex\", \"\").replace(\".ipynb\", \"\"))\n            };\n            notebook.widgets.map((c, index) => {\n                if (c.model.value.text.startsWith(\"## Message to instructor:\")) {\n                    info.message = c.model.value.text;\n                }\n                if (index == activeIndex) {\n                    codeBlock = c.model.value.text;\n                }\n            });\n            if (!codeBlock.startsWith(\"## PID \")) {\n                showErrorMessage('Code Share Error', \"Invalid cell selected. Use a specific problem cell block.\");\n                return;\n            }\n            let postBody = {\n                \"message\": info.message,\n                \"code\": codeBlock,\n                \"problem_id\": info.problem_id,\n                \"snapshot\": 2\n            };\n            console.log(\"Req body: \", postBody);\n            requestAPI('submissions', {\n                method: 'POST',\n                body: JSON.stringify(postBody)\n            })\n                .then(data => {\n                if (data.msg === \"Submission saved successfully.\") {\n                    if (info.message.length > 27) {\n                        data.msg = 'Code & message is sent to the instructor.';\n                    }\n                    else {\n                        data.msg = 'Code is sent to the instructor.';\n                    }\n                }\n                showDialog({\n                    title: '',\n                    body: data.msg,\n                    buttons: [Dialog.okButton({ label: 'Ok' })]\n                });\n                // Keep checking for new feedback.\n                // This setInterval will be cleared once the feedback is downloaded (after reload())\n                // setInterval(function(){\n                //     // console.log(\"Checking for feedback...\")\n                //     requestAPI<any>('feedback',{\n                //     method: 'GET'\n                //     })\n                //     .then(data => {\n                //         // console.log(data);\n                //         if (data['hard-reload'] != -1) {\n                //         showDialog({\n                //             title:'',\n                //             body: data.msg,\n                //             buttons: [Dialog.okButton({ label: 'Ok' })]\n                //         }).then( result => {\n                //             if (result.button.accept ) {\n                //                 window.location.reload();\n                //             }\n                //         })\n                //         }\n                //     })\n                //     .catch(reason => {\n                //         showErrorMessage('Get Feedback Error', reason);\n                //         console.error(\n                //         `Failed to fetch recent feedbacks.\\n${reason}`\n                //         );\n                //     });\n                // }, 60000);\n            })\n                .catch(reason => {\n                showErrorMessage('Code Share Error', reason);\n                console.error(`Failed to share code to server.\\n${reason}`);\n            });\n        };\n        const button = new ToolbarButton({\n            className: 'share-code-button',\n            label: 'ShareCode',\n            onClick: shareCode,\n            tooltip: 'Share your code to the instructor.',\n        });\n        panel.toolbar.insertItem(12, 'shareCode', button);\n        return new DisposableDelegate(() => {\n            button.dispose();\n        });\n    }\n}\n",
+        "import { ReactWidget } from '@jupyterlab/apputils';\nimport { fileUploadIcon, LabIcon } from '@jupyterlab/ui-components';\nimport React from 'react';\nimport { requestAPI } from './handler';\nimport { Dialog, showDialog, showErrorMessage } from '@jupyterlab/apputils';\nconst ShareButton = ({ icon, onClick }) => (React.createElement(\"button\", { type: \"button\", onClick: () => onClick(), className: \"cellButton\" },\n    React.createElement(LabIcon.resolveReact, { icon: icon, className: \"cellButton-icon\", tag: \"span\", width: \"15px\", height: \"15px\" })));\nconst CodeCellButtonComponent = ({ cell, info, }) => {\n    const shareCode = async () => {\n        if (isNaN(info.problem_id)) {\n            showErrorMessage('Code Share Error', \"Invalid code block. Use specific problem notebook.\");\n            return;\n        }\n        // clear message skeleton\n        info.message = info.message.replace(\"## Message to instructor: \", \"\");\n        let postBody = {\n            \"message\": info.message,\n            \"code\": cell.model.value.text,\n            \"problem_id\": info.problem_id,\n            \"snapshot\": 2\n        };\n        console.log(\"From widget: \", postBody);\n        requestAPI('submissions', {\n            method: 'POST',\n            body: JSON.stringify(postBody)\n        })\n            .then(data => {\n            if (data.msg === \"Submission saved successfully.\") {\n                if (info.message.length > 27) {\n                    data.msg = 'Code & message is sent to the instructor.';\n                }\n                else {\n                    data.msg = 'Code is sent to the instructor.';\n                }\n            }\n            showDialog({\n                title: '',\n                body: data.msg,\n                buttons: [Dialog.okButton({ label: 'Ok' })]\n            });\n            // Keep checking for new feedback.\n            // This setInterval will be cleared once the feedback is downloaded (after reload())\n            // setInterval(function(){\n            //     // console.log(\"Checking for feedback...\")\n            //     requestAPI<any>('feedback',{\n            //     method: 'GET'\n            //     })\n            //     .then(data => {\n            //         // console.log(data);\n            //         if (data['hard-reload'] != -1) {\n            //         showDialog({\n            //             title:'',\n            //             body: data.msg,\n            //             buttons: [Dialog.okButton({ label: 'Ok' })]\n            //         }).then( result => {\n            //             if (result.button.accept ) {\n            //                 window.location.reload();\n            //             }\n            //         })\n            //         }\n            //     })\n            //     .catch(reason => {\n            //         showErrorMessage('Get Feedback Error', reason);\n            //         console.error(\n            //         `Failed to fetch recent feedbacks.\\n${reason}`\n            //         );\n            //     });\n            // }, 60000);\n        })\n            .catch(reason => {\n            showErrorMessage('Code Share Error', reason);\n            console.error(`Failed to share code to server.\\n${reason}`);\n        });\n    };\n    return (React.createElement(\"div\", null,\n        React.createElement(ShareButton, { icon: fileUploadIcon, onClick: () => (shareCode)() })));\n};\nexport class CellCheckButton extends ReactWidget {\n    constructor(cell, info) {\n        super();\n        this.cell = null;\n        this.info = null;\n        this.cell = cell;\n        this.info = info;\n        this.addClass('jp-CellButton');\n    }\n    render() {\n        return React.createElement(CodeCellButtonComponent, { cell: this.cell, info: this.info });\n    }\n}\n"
     ],
     "version": 3
 }
```

### Comparing `carpo_student-0.0.8/carpo_student/labextension/static/remoteEntry.b940a131cff178ae61e8.js` & `carpo_student-0.0.9/carpo_student/labextension/static/remoteEntry.8056dafefbbffbedae97.js`

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
-                "lib_index_js": "c3e6db586344d03a5551",
+                "lib_index_js": "702cd083cba688e6ae07",
                 "vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1": "a80375a08cdf3b742d9b",
                 "style_index_js": "e596dd9ff10e476ac3a0"
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
-                    register("carpo-student", "0.0.7", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
+                    register("carpo-student", "0.0.8", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
                     /******/
                 }
                 /******/
                 break;
                 /******/
             }
             /******/
@@ -1086,8 +1086,8 @@
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/carpo-student");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB)["carpo-student"] = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.b940a131cff178ae61e8.js.map
+//# sourceMappingURL=remoteEntry.8056dafefbbffbedae97.js.map
```

### Comparing `carpo_student-0.0.8/carpo_student/labextension/static/remoteEntry.b940a131cff178ae61e8.js.map` & `carpo_student-0.0.9/carpo_student/labextension/static/remoteEntry.8056dafefbbffbedae97.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9142857142857144%*

 * *Differences: {"'file'": "'remoteEntry.8056dafefbbffbedae97.js'",*

 * * "'sourcesContent'": "{insert: [(5, '// This function allow to reference async "*

 * *                     'chunks\\n__webpack_require__.u = (chunkId) => {\\n\\t// return url for '*

 * *                     'filenames based on template\\n\\treturn "" + chunkId + "." + '*

 * *                     '{"lib_index_js":"702cd083cba688e6ae07","vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1":"a80375a08cdf3b742d9b","style_index […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "remoteEntry.b940a131cff178ae61e8.js",
+    "file": "remoteEntry.8056dafefbbffbedae97.js",
     "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,4MAA4M;WAC1O;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC3CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WCfA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WCrLA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://carpo-student/webpack/container-entry",
         "webpack://carpo-student/webpack/bootstrap",
         "webpack://carpo-student/webpack/runtime/compat get default export",
@@ -25,20 +25,20 @@
     ],
     "sourcesContent": [
         "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./style\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"style_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./style/index.js */ \"./style/index.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId](module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"c3e6db586344d03a5551\",\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\":\"a80375a08cdf3b742d9b\",\"style_index_js\":\"e596dd9ff10e476ac3a0\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"702cd083cba688e6ae07\",\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\":\"a80375a08cdf3b742d9b\",\"style_index_js\":\"e596dd9ff10e476ac3a0\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"carpo-student:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\t;\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"carpo-student\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"carpo-student\", \"0.0.7\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"carpo-student\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"carpo-student\", \"0.0.8\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) scriptUrl = scripts[scripts.length - 1].src\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
         "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) typeof console !== \"undefined\" && console.warn && console.warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\ttypeof console !== \"undefined\" && console.warn && console.warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/notebook\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/notebook\", [1,3,4,2])),\n\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/settingregistry\", [1,3,4,2])),\n\t\"webpack/sharing/consume/default/@lumino/disposable\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/disposable\", [1,1,10,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,3,4,2])),\n\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/ui-components\", [1,3,4,2])),\n\t\"webpack/sharing/consume/default/react\": () => (loadSingletonVersionCheck(\"default\", \"react\", [1,17,0,1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/coreutils\", [1,5,4,2])),\n\t\"webpack/sharing/consume/default/@jupyterlab/services\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/services\", [1,6,4,2]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/notebook\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/settingregistry\",\n\t\t\"webpack/sharing/consume/default/@lumino/disposable\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\",\n\t\t\"webpack/sharing/consume/default/react\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/services\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
         "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"carpo-student\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t} else installedChunks[chunkId] = 0;\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkcarpo_student\"] = self[\"webpackChunkcarpo_student\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "__webpack_require__.nc = undefined;",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/carpo-student\");\n",
         ""
```

### Comparing `carpo_student-0.0.8/carpo_student/labextension/static/style_index_js.e596dd9ff10e476ac3a0.js` & `carpo_student-0.0.9/carpo_student/labextension/static/style_index_js.e596dd9ff10e476ac3a0.js`

 * *Files identical despite different names*

### Comparing `carpo_student-0.0.8/carpo_student/labextension/static/style_index_js.e596dd9ff10e476ac3a0.js.map` & `carpo_student-0.0.9/carpo_student/labextension/static/style_index_js.e596dd9ff10e476ac3a0.js.map`

 * *Files identical despite different names*

### Comparing `carpo_student-0.0.8/carpo_student/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.a80375a08cdf3b742d9b.js` & `carpo_student-0.0.9/carpo_student/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.a80375a08cdf3b742d9b.js`

 * *Files identical despite different names*

### Comparing `carpo_student-0.0.8/carpo_student/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.a80375a08cdf3b742d9b.js.map` & `carpo_student-0.0.9/carpo_student/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.a80375a08cdf3b742d9b.js.map`

 * *Files identical despite different names*

### Comparing `carpo_student-0.0.8/carpo_student.egg-info/SOURCES.txt` & `carpo_student-0.0.9/carpo_student.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 CHANGELOG.md
+DEV_INSTALL.md
+INSTALL.md
 LICENSE
 MANIFEST.in
 README.md
 RELEASE.md
 install.json
 package.json
 pyproject.toml
@@ -16,18 +18,18 @@
 carpo_student.egg-info/SOURCES.txt
 carpo_student.egg-info/dependency_links.txt
 carpo_student.egg-info/not-zip-safe
 carpo_student.egg-info/requires.txt
 carpo_student.egg-info/top_level.txt
 carpo_student/labextension/build_log.json
 carpo_student/labextension/package.json
-carpo_student/labextension/static/lib_index_js.c3e6db586344d03a5551.js
-carpo_student/labextension/static/lib_index_js.c3e6db586344d03a5551.js.map
-carpo_student/labextension/static/remoteEntry.b940a131cff178ae61e8.js
-carpo_student/labextension/static/remoteEntry.b940a131cff178ae61e8.js.map
+carpo_student/labextension/static/lib_index_js.702cd083cba688e6ae07.js
+carpo_student/labextension/static/lib_index_js.702cd083cba688e6ae07.js.map
+carpo_student/labextension/static/remoteEntry.8056dafefbbffbedae97.js
+carpo_student/labextension/static/remoteEntry.8056dafefbbffbedae97.js.map
 carpo_student/labextension/static/style.js
 carpo_student/labextension/static/style_index_js.e596dd9ff10e476ac3a0.js
 carpo_student/labextension/static/style_index_js.e596dd9ff10e476ac3a0.js.map
 carpo_student/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.a80375a08cdf3b742d9b.js
 carpo_student/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.a80375a08cdf3b742d9b.js.map
 jupyter-config/nb-config/carpo_student.json
 jupyter-config/server-config/carpo_student.json
```

### Comparing `carpo_student-0.0.8/package.json` & `carpo_student-0.0.9/package.json`

 * *Files 1% similar despite different names*

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
-    "version": "0.0.8"
+    "version": "0.0.9"
 }
```

### Comparing `carpo_student-0.0.8/pyproject.toml` & `carpo_student-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `carpo_student-0.0.8/setup.py` & `carpo_student-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `carpo_student-0.0.8/src/get-solutions.ts` & `carpo_student-0.0.9/src/get-solutions.ts`

 * *Files identical despite different names*

### Comparing `carpo_student-0.0.8/src/handler.ts` & `carpo_student-0.0.9/src/handler.ts`

 * *Files identical despite different names*

### Comparing `carpo_student-0.0.8/src/index.ts` & `carpo_student-0.0.9/src/index.ts`

 * *Files 3% similar despite different names*

```diff
@@ -45,18 +45,18 @@
   optional: [ISettingRegistry],
   activate: (
       app: JupyterFrontEnd, 
       nbTrack: INotebookTracker,
       settingRegistry: ISettingRegistry | null
     ) => {
     console.log('JupyterLab extension carpo-student is activated!');
-
+    // var interval => (); 
+    var counter: number = 0;
     nbTrack.currentChanged.connect(() => {
-      console.log("->: ", nbTrack.currentWidget.context.path);
-
+      console.log("my counter: ", counter);
       const notebookPanel = nbTrack.currentWidget;
       const notebook = nbTrack.currentWidget.content;
       const filename = notebookPanel.context.path
 
       // Disable Code Share functionality if inside Feedback directory
       if (filename.includes("Feedback")){
         return 
@@ -99,24 +99,51 @@
           // Get the message block referencing the active cell.
           notebook.widgets.map((c,index) =>{
             if (c.model.value.text.startsWith("## Message to instructor:")){
               info.message = c.model.value.text
             }
             if (index == activeIndex) {
               question = c.model.value.text
+              if (question.includes("## PID ")){
+
+                const newCheckButton: CellCheckButton = new CellCheckButton(cell,info);
+
+                (cell.layout as PanelLayout).addWidget(newCheckButton);
+                currentCellCheckButton = newCheckButton;
+
+                // Send code snapshot to the server:
+                if (counter == 0 ){
+                  setInterval(function () {
+                    let postBody = {
+                      "message": "",
+                      "code": c.model.value.text,
+                      "problem_id":info.problem_id,
+                      "snapshot": 1
+                      }
+                      requestAPI<any>('submissions',{
+                          method: 'POST',
+                          body: JSON.stringify(postBody)
+                      })
+                      .then(data => {
+                          console.log("Snapshot sent.", data)
+                        });
+                  }, 20000);
+                  counter ++;
+                }
+              }
             }
           })
        
 
-          const newCheckButton: CellCheckButton = new CellCheckButton(cell,info);
+          // const newCheckButton: CellCheckButton = new CellCheckButton(cell,info);
           
-          if (question.includes("## PID ")){
-            (cell.layout as PanelLayout).addWidget(newCheckButton);
-            currentCellCheckButton = newCheckButton;
-          }
+          // if (question.includes("## PID ")){
+          //   (cell.layout as PanelLayout).addWidget(newCheckButton);
+          //   currentCellCheckButton = newCheckButton;
+          // }
 
           // Set the current cell and button for future
           // reference
           currentCell = cell;
 
         });
```

### Comparing `carpo_student-0.0.8/style/base.css` & `carpo_student-0.0.9/style/base.css`

 * *Files identical despite different names*

### Comparing `carpo_student-0.0.8/tsconfig.json` & `carpo_student-0.0.9/tsconfig.json`

 * *Files identical despite different names*

### Comparing `carpo_student-0.0.8/yarn.lock` & `carpo_student-0.0.9/yarn.lock`

 * *Files identical despite different names*

