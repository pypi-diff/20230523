# Comparing `tmp/force-relative-import-0.0.1.post1.tar.gz` & `tmp/force-relative-import-0.0.2.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "force-relative-import-0.0.1.post1.tar", last modified: Sun Apr 30 10:50:10 2023, max compression
+gzip compressed data, was "force-relative-import-0.0.2.post0.tar", last modified: Tue May 23 09:03:23 2023, max compression
```

## Comparing `force-relative-import-0.0.1.post1.tar` & `force-relative-import-0.0.2.post0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 10:50:05.175541 force-relative-import-0.0.1.post1/
--rw-rw-rw-   0        0        0     1066 2019-06-16 06:53:07.000000 force-relative-import-0.0.1.post1/LICENSE
--rw-rw-rw-   0        0        0     2406 2023-04-30 10:50:10.608086 force-relative-import-0.0.1.post1/PKG-INFO
--rw-rw-rw-   0        0        0     1891 2023-04-30 10:19:10.000000 force-relative-import-0.0.1.post1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 10:50:05.169662 force-relative-import-0.0.1.post1/force_relative_import/
--rw-rw-rw-   0        0        0     2542 2023-04-30 10:26:53.000000 force-relative-import-0.0.1.post1/force_relative_import/__init__.py
--rw-rw-rw-   0        0        0      183 2023-04-30 05:25:44.000000 force-relative-import-0.0.1.post1/force_relative_import/enable_now.py
-drwxrwxrwx   0        0        0        0 2023-04-30 10:50:10.607088 force-relative-import-0.0.1.post1/force_relative_import.egg-info/
--rw-rw-rw-   0        0        0     2406 2023-04-30 10:50:10.000000 force-relative-import-0.0.1.post1/force_relative_import.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-04-30 10:50:10.000000 force-relative-import-0.0.1.post1/force_relative_import.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 10:50:10.000000 force-relative-import-0.0.1.post1/force_relative_import.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-04-30 10:50:10.000000 force-relative-import-0.0.1.post1/force_relative_import.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-30 10:50:10.609084 force-relative-import-0.0.1.post1/setup.cfg
--rw-rw-rw-   0        0        0      733 2023-04-30 10:48:34.000000 force-relative-import-0.0.1.post1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:03:23.398161 force-relative-import-0.0.2.post0/
+-rw-rw-rw-   0        0        0     1066 2019-06-16 06:53:07.000000 force-relative-import-0.0.2.post0/LICENSE
+-rw-rw-rw-   0        0        0     2406 2023-05-23 09:03:23.396169 force-relative-import-0.0.2.post0/PKG-INFO
+-rw-rw-rw-   0        0        0     1891 2023-04-30 10:19:10.000000 force-relative-import-0.0.2.post0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 09:03:23.374573 force-relative-import-0.0.2.post0/force_relative_import/
+-rw-rw-rw-   0        0        0     2569 2023-05-23 08:58:50.000000 force-relative-import-0.0.2.post0/force_relative_import/__init__.py
+-rw-rw-rw-   0        0        0      183 2023-04-30 05:25:44.000000 force-relative-import-0.0.2.post0/force_relative_import/enable_now.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:03:23.390164 force-relative-import-0.0.2.post0/force_relative_import.egg-info/
+-rw-rw-rw-   0        0        0     2406 2023-05-23 09:03:22.000000 force-relative-import-0.0.2.post0/force_relative_import.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-05-23 09:03:23.000000 force-relative-import-0.0.2.post0/force_relative_import.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 09:03:22.000000 force-relative-import-0.0.2.post0/force_relative_import.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-23 09:03:22.000000 force-relative-import-0.0.2.post0/force_relative_import.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 09:03:23.398161 force-relative-import-0.0.2.post0/setup.cfg
+-rw-rw-rw-   0        0        0      733 2023-05-23 09:00:51.000000 force-relative-import-0.0.2.post0/setup.py
```

### Comparing `force-relative-import-0.0.1.post1/LICENSE` & `force-relative-import-0.0.2.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `force-relative-import-0.0.1.post1/PKG-INFO` & `force-relative-import-0.0.2.post0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: force-relative-import
-Version: 0.0.1.post1
+Version: 0.0.2.post0
 Summary: Allow users to bypass Python relative import restrictions.
 Home-page: https://github.com/One-sixth/force-relative-import
 Author: onesixth
 Author-email: noexist@noexist.noexist
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `force-relative-import-0.0.1.post1/README.md` & `force-relative-import-0.0.2.post0/README.md`

 * *Files identical despite different names*

### Comparing `force-relative-import-0.0.1.post1/force_relative_import/__init__.py` & `force-relative-import-0.0.2.post0/force_relative_import/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             # 不是目标异常，继续抛出
             raise e
 
         # 强制导入目标包
         require_module_file = globals['__file__']
         new_import_path = os.path.dirname(require_module_file) + _make_parent_str(level)
         sys.path.insert(0, new_import_path)
-        m = ori_import(name)
+        m = ori_import(name, globals, locals, fromlist)
         del sys.path[0]
         if info:
             print(f'Info! Force load relative module: {name} . Required by {require_module_file}', flush=True)
 
     return m
```

### Comparing `force-relative-import-0.0.1.post1/force_relative_import.egg-info/PKG-INFO` & `force-relative-import-0.0.2.post0/force_relative_import.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: force-relative-import
-Version: 0.0.1.post1
+Version: 0.0.2.post0
 Summary: Allow users to bypass Python relative import restrictions.
 Home-page: https://github.com/One-sixth/force-relative-import
 Author: onesixth
 Author-email: noexist@noexist.noexist
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `force-relative-import-0.0.1.post1/setup.py` & `force-relative-import-0.0.2.post0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-ver_str = '0.0.1.post1'
+ver_str = '0.0.2.post0'
 
 long_description = open('README.md', 'r', encoding='utf8').read()
 
 setup(
     name='force-relative-import',
     version=ver_str,
     description='Allow users to bypass Python relative import restrictions.',
```

