# Comparing `tmp/prelude-cli-1.2.0.tar.gz` & `tmp/prelude-cli-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude-cli-1.2.0.tar", last modified: Tue May 23 20:19:01 2023, max compression
+gzip compressed data, was "prelude-cli-1.2.1.tar", last modified: Tue May 23 21:46:57 2023, max compression
```

## Comparing `prelude-cli-1.2.0.tar` & `prelude-cli-1.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-23 20:19:01.502207 prelude-cli-1.2.0/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-cli-1.2.0/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude-cli-1.2.0/MANIFEST.in
--rw-r--r--   0 pack       (501) staff       (20)      832 2023-05-23 20:19:01.502254 prelude-cli-1.2.0/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude-cli-1.2.0/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-23 20:19:01.499610 prelude-cli-1.2.0/prelude_cli/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.0/prelude_cli/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)      775 2023-05-02 14:19:17.000000 prelude-cli-1.2.0/prelude_cli/cli.py
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-05-03 13:30:52.000000 prelude-cli-1.2.0/prelude_cli/spinner.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-23 20:19:01.500500 prelude-cli-1.2.0/prelude_cli/templates/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.0/prelude_cli/templates/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)      241 2023-05-04 16:11:50.000000 prelude-cli-1.2.0/prelude_cli/templates/template.go
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-23 20:19:01.501992 prelude-cli-1.2.0/prelude_cli/views/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.0/prelude_cli/views/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     3241 2023-05-18 20:31:39.000000 prelude-cli-1.2.0/prelude_cli/views/build.py
--rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude-cli-1.2.0/prelude_cli/views/configure.py
--rw-r--r--   0 pack       (501) staff       (20)     7272 2023-05-23 15:18:07.000000 prelude-cli-1.2.0/prelude_cli/views/detect.py
--rw-r--r--   0 pack       (501) staff       (20)     3478 2023-05-18 20:31:39.000000 prelude-cli-1.2.0/prelude_cli/views/iam.py
--rw-r--r--   0 pack       (501) staff       (20)     2279 2023-05-18 19:30:30.000000 prelude-cli-1.2.0/prelude_cli/views/partner.py
--rw-r--r--   0 pack       (501) staff       (20)     1139 2023-05-03 13:30:52.000000 prelude-cli-1.2.0/prelude_cli/views/shared.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-23 20:19:01.500319 prelude-cli-1.2.0/prelude_cli.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)      832 2023-05-23 20:19:01.000000 prelude-cli-1.2.0/prelude_cli.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      598 2023-05-23 20:19:01.000000 prelude-cli-1.2.0/prelude_cli.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2023-05-23 20:19:01.000000 prelude-cli-1.2.0/prelude_cli.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)       48 2023-05-23 20:19:01.000000 prelude-cli-1.2.0/prelude_cli.egg-info/entry_points.txt
--rw-r--r--   0 pack       (501) staff       (20)       32 2023-05-23 20:19:01.000000 prelude-cli-1.2.0/prelude_cli.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       12 2023-05-23 20:19:01.000000 prelude-cli-1.2.0/prelude_cli.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-cli-1.2.0/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      663 2023-05-23 20:19:01.502457 prelude-cli-1.2.0/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-23 21:46:57.208481 prelude-cli-1.2.1/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-cli-1.2.1/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude-cli-1.2.1/MANIFEST.in
+-rw-r--r--   0 pack       (501) staff       (20)      832 2023-05-23 21:46:57.208529 prelude-cli-1.2.1/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude-cli-1.2.1/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-23 21:46:57.204897 prelude-cli-1.2.1/prelude_cli/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.1/prelude_cli/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)      775 2023-05-02 14:19:17.000000 prelude-cli-1.2.1/prelude_cli/cli.py
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-05-03 13:30:52.000000 prelude-cli-1.2.1/prelude_cli/spinner.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-23 21:46:57.205799 prelude-cli-1.2.1/prelude_cli/templates/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.1/prelude_cli/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)      241 2023-05-04 16:11:50.000000 prelude-cli-1.2.1/prelude_cli/templates/template.go
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-23 21:46:57.208132 prelude-cli-1.2.1/prelude_cli/views/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.1/prelude_cli/views/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     3241 2023-05-18 20:31:39.000000 prelude-cli-1.2.1/prelude_cli/views/build.py
+-rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude-cli-1.2.1/prelude_cli/views/configure.py
+-rw-r--r--   0 pack       (501) staff       (20)     7276 2023-05-23 21:42:11.000000 prelude-cli-1.2.1/prelude_cli/views/detect.py
+-rw-r--r--   0 pack       (501) staff       (20)     3478 2023-05-18 20:31:39.000000 prelude-cli-1.2.1/prelude_cli/views/iam.py
+-rw-r--r--   0 pack       (501) staff       (20)     2279 2023-05-18 19:30:30.000000 prelude-cli-1.2.1/prelude_cli/views/partner.py
+-rw-r--r--   0 pack       (501) staff       (20)     1139 2023-05-03 13:30:52.000000 prelude-cli-1.2.1/prelude_cli/views/shared.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-23 21:46:57.205618 prelude-cli-1.2.1/prelude_cli.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)      832 2023-05-23 21:46:57.000000 prelude-cli-1.2.1/prelude_cli.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      598 2023-05-23 21:46:57.000000 prelude-cli-1.2.1/prelude_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2023-05-23 21:46:57.000000 prelude-cli-1.2.1/prelude_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)       48 2023-05-23 21:46:57.000000 prelude-cli-1.2.1/prelude_cli.egg-info/entry_points.txt
+-rw-r--r--   0 pack       (501) staff       (20)       32 2023-05-23 21:46:57.000000 prelude-cli-1.2.1/prelude_cli.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       12 2023-05-23 21:46:57.000000 prelude-cli-1.2.1/prelude_cli.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-cli-1.2.1/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      663 2023-05-23 21:46:57.208742 prelude-cli-1.2.1/setup.cfg
```

### Comparing `prelude-cli-1.2.0/LICENSE` & `prelude-cli-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.0/PKG-INFO` & `prelude-cli-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 1.2.0
+Version: 1.2.1
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-cli-1.2.0/prelude_cli/cli.py` & `prelude-cli-1.2.1/prelude_cli/cli.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.0/prelude_cli/views/build.py` & `prelude-cli-1.2.1/prelude_cli/views/build.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.0/prelude_cli/views/configure.py` & `prelude-cli-1.2.1/prelude_cli/views/configure.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.0/prelude_cli/views/detect.py` & `prelude-cli-1.2.1/prelude_cli/views/detect.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
         for attach in controller.get_test(test_id=test['id']).get('attachments'):
             if Path(attach).suffix:
                 code = controller.download(test_id=test['id'], filename=attach)
                 with open(PurePath(test['id'], attach), 'wb') as f:
                     f.write(code)
 
     async def start_cloning():
-        await asyncio.gather(*[fetch(test) for test in detect.list_tests()])
+        await asyncio.gather(*[fetch(test) for test in controller.list_tests()])
 
     with Spinner():
         asyncio.run(start_cloning())
         click.secho('Project cloned successfully', fg='green')
 
 
 @detect.command('activity')
```

### Comparing `prelude-cli-1.2.0/prelude_cli/views/iam.py` & `prelude-cli-1.2.1/prelude_cli/views/iam.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.0/prelude_cli/views/partner.py` & `prelude-cli-1.2.1/prelude_cli/views/partner.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.0/prelude_cli/views/shared.py` & `prelude-cli-1.2.1/prelude_cli/views/shared.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.0/prelude_cli.egg-info/PKG-INFO` & `prelude-cli-1.2.1/prelude_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 1.2.0
+Version: 1.2.1
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-cli-1.2.0/prelude_cli.egg-info/SOURCES.txt` & `prelude-cli-1.2.1/prelude_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.0/setup.cfg` & `prelude-cli-1.2.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prelude-cli
-version = 1.2.0
+version = 1.2.1
 author = Prelude Research
 author_email = support@preludesecurity.com
 description = For interacting with the Prelude SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/preludeorg
 classifiers = 
@@ -13,15 +13,15 @@
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=3.8
 install_requires = 
-	prelude-sdk == 1.2.0
+	prelude-sdk == 1.2.1
 	click > 8
 	rich
 
 [options.entry_points]
 console_scripts = 
 	prelude = prelude_cli.cli:cli
```

