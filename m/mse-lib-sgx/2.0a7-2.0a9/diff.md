# Comparing `tmp/mse_lib_sgx-2.0a7.tar.gz` & `tmp/mse_lib_sgx-2.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mse_lib_sgx-2.0a7.tar", last modified: Mon May 22 08:21:45 2023, max compression
+gzip compressed data, was "mse_lib_sgx-2.0a9.tar", last modified: Mon May 22 09:01:46 2023, max compression
```

## Comparing `mse_lib_sgx-2.0a7.tar` & `mse_lib_sgx-2.0a9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:21:45.803617 mse_lib_sgx-2.0a7/
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-22 08:21:45.803617 mse_lib_sgx-2.0a7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-22 08:20:52.000000 mse_lib_sgx-2.0a7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-22 08:21:45.803617 mse_lib_sgx-2.0a7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-22 08:20:52.000000 mse_lib_sgx-2.0a7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:21:45.799617 mse_lib_sgx-2.0a7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:21:45.799617 mse_lib_sgx-2.0a7/src/mse_lib_sgx/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-22 08:20:52.000000 mse_lib_sgx-2.0a7/src/mse_lib_sgx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-22 08:20:52.000000 mse_lib_sgx-2.0a7/src/mse_lib_sgx/base64url.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-05-22 08:20:52.000000 mse_lib_sgx-2.0a7/src/mse_lib_sgx/certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8533 2023-05-22 08:20:52.000000 mse_lib_sgx-2.0a7/src/mse_lib_sgx/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-22 08:20:52.000000 mse_lib_sgx-2.0a7/src/mse_lib_sgx/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-22 08:20:52.000000 mse_lib_sgx-2.0a7/src/mse_lib_sgx/globs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-05-22 08:20:52.000000 mse_lib_sgx-2.0a7/src/mse_lib_sgx/http_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-22 08:20:52.000000 mse_lib_sgx-2.0a7/src/mse_lib_sgx/import_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:21:45.803617 mse_lib_sgx-2.0a7/src/mse_lib_sgx/sgx/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-22 08:20:52.000000 mse_lib_sgx-2.0a7/src/mse_lib_sgx/sgx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-22 08:20:52.000000 mse_lib_sgx-2.0a7/src/mse_lib_sgx/sgx/key.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-22 08:20:52.000000 mse_lib_sgx-2.0a7/src/mse_lib_sgx/sgx/quote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:21:45.803617 mse_lib_sgx-2.0a7/src/mse_lib_sgx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-22 08:21:45.000000 mse_lib_sgx-2.0a7/src/mse_lib_sgx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-22 08:21:45.000000 mse_lib_sgx-2.0a7/src/mse_lib_sgx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 08:21:45.000000 mse_lib_sgx-2.0a7/src/mse_lib_sgx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-22 08:21:45.000000 mse_lib_sgx-2.0a7/src/mse_lib_sgx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 08:21:45.000000 mse_lib_sgx-2.0a7/src/mse_lib_sgx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-22 08:21:45.000000 mse_lib_sgx-2.0a7/src/mse_lib_sgx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 08:21:45.000000 mse_lib_sgx-2.0a7/src/mse_lib_sgx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:21:45.803617 mse_lib_sgx-2.0a7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-22 08:20:52.000000 mse_lib_sgx-2.0a7/tests/test_cert_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-22 08:20:52.000000 mse_lib_sgx-2.0a7/tests/test_conf_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:01:46.084179 mse_lib_sgx-2.0a9/
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-22 09:01:46.084179 mse_lib_sgx-2.0a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-22 09:00:53.000000 mse_lib_sgx-2.0a9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-22 09:01:46.084179 mse_lib_sgx-2.0a9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-22 09:00:53.000000 mse_lib_sgx-2.0a9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:01:46.080179 mse_lib_sgx-2.0a9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:01:46.080179 mse_lib_sgx-2.0a9/src/mse_lib_sgx/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-22 09:00:53.000000 mse_lib_sgx-2.0a9/src/mse_lib_sgx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-22 09:00:53.000000 mse_lib_sgx-2.0a9/src/mse_lib_sgx/base64url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-05-22 09:00:53.000000 mse_lib_sgx-2.0a9/src/mse_lib_sgx/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-05-22 09:00:53.000000 mse_lib_sgx-2.0a9/src/mse_lib_sgx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-22 09:00:53.000000 mse_lib_sgx-2.0a9/src/mse_lib_sgx/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-22 09:00:53.000000 mse_lib_sgx-2.0a9/src/mse_lib_sgx/globs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-05-22 09:00:53.000000 mse_lib_sgx-2.0a9/src/mse_lib_sgx/http_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-22 09:00:53.000000 mse_lib_sgx-2.0a9/src/mse_lib_sgx/import_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:01:46.080179 mse_lib_sgx-2.0a9/src/mse_lib_sgx/sgx/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-22 09:00:53.000000 mse_lib_sgx-2.0a9/src/mse_lib_sgx/sgx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-22 09:00:53.000000 mse_lib_sgx-2.0a9/src/mse_lib_sgx/sgx/key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-22 09:00:53.000000 mse_lib_sgx-2.0a9/src/mse_lib_sgx/sgx/quote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:01:46.080179 mse_lib_sgx-2.0a9/src/mse_lib_sgx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-22 09:01:46.000000 mse_lib_sgx-2.0a9/src/mse_lib_sgx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-22 09:01:46.000000 mse_lib_sgx-2.0a9/src/mse_lib_sgx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 09:01:46.000000 mse_lib_sgx-2.0a9/src/mse_lib_sgx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-22 09:01:46.000000 mse_lib_sgx-2.0a9/src/mse_lib_sgx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 09:01:45.000000 mse_lib_sgx-2.0a9/src/mse_lib_sgx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-22 09:01:46.000000 mse_lib_sgx-2.0a9/src/mse_lib_sgx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 09:01:46.000000 mse_lib_sgx-2.0a9/src/mse_lib_sgx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:01:46.084179 mse_lib_sgx-2.0a9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-22 09:00:53.000000 mse_lib_sgx-2.0a9/tests/test_cert_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-22 09:00:53.000000 mse_lib_sgx-2.0a9/tests/test_conf_server.py
```

### Comparing `mse_lib_sgx-2.0a7/PKG-INFO` & `mse_lib_sgx-2.0a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mse_lib_sgx
-Version: 2.0a7
+Version: 2.0a9
 Summary: Library for Cosmian MSE to bootstrap Flask application
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mse_lib_sgx-2.0a7/README.md` & `mse_lib_sgx-2.0a9/README.md`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a7/setup.py` & `mse_lib_sgx-2.0a9/setup.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a7/src/mse_lib_sgx/base64url.py` & `mse_lib_sgx-2.0a9/src/mse_lib_sgx/base64url.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a7/src/mse_lib_sgx/certificate.py` & `mse_lib_sgx-2.0a9/src/mse_lib_sgx/certificate.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a7/src/mse_lib_sgx/cli.py` & `mse_lib_sgx-2.0a9/src/mse_lib_sgx/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,15 +209,20 @@
             ssl_app_mode == SslAppMode.CUSTOM_CERTIFICATE
             and globs.SSL_PRIVATE_KEY
             and ssl_private_key_path is not None
         ):
             ssl_private_key_path.write_text(globs.SSL_PRIVATE_KEY)
 
     if globs.PLAINCODE:
-        shutil.copytree(args.app_dir, globs.MODULE_DIR_PATH, dirs_exist_ok=True)
+        shutil.copytree(
+            src=args.app_dir,
+            dst=globs.MODULE_DIR_PATH,
+            copy_function=shutil.copy,
+            dirs_exist_ok=True,
+        )
     else:
         decrypt_directory(
             dir_path=args.app_dir,
             key=globs.CODE_KEY_PATH.read_bytes(),
             ext=".enc",
             out_dir_path=globs.MODULE_DIR_PATH,
         )
```

### Comparing `mse_lib_sgx-2.0a7/src/mse_lib_sgx/globs.py` & `mse_lib_sgx-2.0a9/src/mse_lib_sgx/globs.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a7/src/mse_lib_sgx/http_server.py` & `mse_lib_sgx-2.0a9/src/mse_lib_sgx/http_server.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a7/src/mse_lib_sgx/import_hook.py` & `mse_lib_sgx-2.0a9/src/mse_lib_sgx/import_hook.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a7/src/mse_lib_sgx/sgx/key.py` & `mse_lib_sgx-2.0a9/src/mse_lib_sgx/sgx/key.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a7/src/mse_lib_sgx/sgx/quote.py` & `mse_lib_sgx-2.0a9/src/mse_lib_sgx/sgx/quote.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a7/src/mse_lib_sgx.egg-info/PKG-INFO` & `mse_lib_sgx-2.0a9/src/mse_lib_sgx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mse-lib-sgx
-Version: 2.0a7
+Version: 2.0a9
 Summary: Library for Cosmian MSE to bootstrap Flask application
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mse_lib_sgx-2.0a7/src/mse_lib_sgx.egg-info/SOURCES.txt` & `mse_lib_sgx-2.0a9/src/mse_lib_sgx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a7/tests/test_cert_utils.py` & `mse_lib_sgx-2.0a9/tests/test_cert_utils.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.0a7/tests/test_conf_server.py` & `mse_lib_sgx-2.0a9/tests/test_conf_server.py`

 * *Files identical despite different names*

