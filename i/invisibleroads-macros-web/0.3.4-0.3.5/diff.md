# Comparing `tmp/invisibleroads-macros-web-0.3.4.tar.gz` & `tmp/invisibleroads-macros-web-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invisibleroads-macros-web-0.3.4.tar", last modified: Sat May 20 03:33:33 2023, max compression
+gzip compressed data, was "invisibleroads-macros-web-0.3.5.tar", last modified: Tue May 23 18:26:10 2023, max compression
```

## Comparing `invisibleroads-macros-web-0.3.4.tar` & `invisibleroads-macros-web-0.3.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-20 03:33:33.077991 invisibleroads-macros-web-0.3.4/
--rw-r--r--   0 rhh       (1000) rhh       (1000)      288 2023-05-18 17:00:41.000000 invisibleroads-macros-web-0.3.4/CHANGES.md
--rw-r--r--   0 rhh       (1000) rhh       (1000)       13 2023-05-18 17:00:41.000000 invisibleroads-macros-web-0.3.4/MANIFEST.in
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1875 2023-05-20 03:33:33.076991 invisibleroads-macros-web-0.3.4/PKG-INFO
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1086 2023-05-18 17:00:41.000000 invisibleroads-macros-web-0.3.4/README.md
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-20 03:33:33.074991 invisibleroads-macros-web-0.3.4/invisibleroads_macros_web/
--rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2023-05-18 17:00:41.000000 invisibleroads-macros-web-0.3.4/invisibleroads_macros_web/__init__.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      846 2023-05-18 17:00:41.000000 invisibleroads-macros-web-0.3.4/invisibleroads_macros_web/browser.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      290 2023-05-18 17:00:41.000000 invisibleroads-macros-web-0.3.4/invisibleroads_macros_web/escape.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1263 2023-05-18 17:00:41.000000 invisibleroads-macros-web-0.3.4/invisibleroads_macros_web/jinja.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      864 2023-05-20 01:27:51.000000 invisibleroads-macros-web-0.3.4/invisibleroads_macros_web/markdown.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      882 2023-05-18 17:00:41.000000 invisibleroads-macros-web-0.3.4/invisibleroads_macros_web/port.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1117 2023-05-18 17:00:41.000000 invisibleroads-macros-web-0.3.4/invisibleroads_macros_web/starlette.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-20 03:33:33.075991 invisibleroads-macros-web-0.3.4/invisibleroads_macros_web.egg-info/
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1875 2023-05-20 03:33:33.000000 invisibleroads-macros-web-0.3.4/invisibleroads_macros_web.egg-info/PKG-INFO
--rw-r--r--   0 rhh       (1000) rhh       (1000)      667 2023-05-20 03:33:33.000000 invisibleroads-macros-web-0.3.4/invisibleroads_macros_web.egg-info/SOURCES.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-05-20 03:33:33.000000 invisibleroads-macros-web-0.3.4/invisibleroads_macros_web.egg-info/dependency_links.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)      163 2023-05-20 03:33:33.000000 invisibleroads-macros-web-0.3.4/invisibleroads_macros_web.egg-info/requires.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)       32 2023-05-20 03:33:33.000000 invisibleroads-macros-web-0.3.4/invisibleroads_macros_web.egg-info/top_level.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-05-18 17:01:44.000000 invisibleroads-macros-web-0.3.4/invisibleroads_macros_web.egg-info/zip-safe
--rw-r--r--   0 rhh       (1000) rhh       (1000)       38 2023-05-20 03:33:33.077991 invisibleroads-macros-web-0.3.4/setup.cfg
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1374 2023-05-20 01:27:51.000000 invisibleroads-macros-web-0.3.4/setup.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-20 03:33:33.076991 invisibleroads-macros-web-0.3.4/tests/
--rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2023-05-18 17:00:41.000000 invisibleroads-macros-web-0.3.4/tests/__init__.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      344 2023-05-18 17:00:41.000000 invisibleroads-macros-web-0.3.4/tests/test_escape.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      904 2023-05-20 01:27:51.000000 invisibleroads-macros-web-0.3.4/tests/test_markdown.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      882 2023-05-18 17:00:41.000000 invisibleroads-macros-web-0.3.4/tests/test_port.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-23 18:26:10.289443 invisibleroads-macros-web-0.3.5/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      288 2022-12-14 19:46:41.000000 invisibleroads-macros-web-0.3.5/CHANGES.md
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       13 2022-10-28 18:39:04.000000 invisibleroads-macros-web-0.3.5/MANIFEST.in
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1875 2023-05-23 18:26:10.289443 invisibleroads-macros-web-0.3.5/PKG-INFO
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1086 2023-02-06 17:49:03.000000 invisibleroads-macros-web-0.3.5/README.md
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-23 18:26:10.288443 invisibleroads-macros-web-0.3.5/invisibleroads_macros_web/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2022-10-28 18:39:04.000000 invisibleroads-macros-web-0.3.5/invisibleroads_macros_web/__init__.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      846 2022-10-28 18:39:04.000000 invisibleroads-macros-web-0.3.5/invisibleroads_macros_web/browser.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      290 2022-10-28 18:39:04.000000 invisibleroads-macros-web-0.3.5/invisibleroads_macros_web/escape.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1263 2023-02-06 20:19:53.000000 invisibleroads-macros-web-0.3.5/invisibleroads_macros_web/jinja.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      845 2023-05-23 18:25:26.000000 invisibleroads-macros-web-0.3.5/invisibleroads_macros_web/markdown.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      882 2022-10-28 18:39:04.000000 invisibleroads-macros-web-0.3.5/invisibleroads_macros_web/port.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1117 2023-03-31 18:25:46.000000 invisibleroads-macros-web-0.3.5/invisibleroads_macros_web/starlette.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-23 18:26:10.288443 invisibleroads-macros-web-0.3.5/invisibleroads_macros_web.egg-info/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1875 2023-05-23 18:26:10.000000 invisibleroads-macros-web-0.3.5/invisibleroads_macros_web.egg-info/PKG-INFO
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      667 2023-05-23 18:26:10.000000 invisibleroads-macros-web-0.3.5/invisibleroads_macros_web.egg-info/SOURCES.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-05-23 18:26:10.000000 invisibleroads-macros-web-0.3.5/invisibleroads_macros_web.egg-info/dependency_links.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      163 2023-05-23 18:26:10.000000 invisibleroads-macros-web-0.3.5/invisibleroads_macros_web.egg-info/requires.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       32 2023-05-23 18:26:10.000000 invisibleroads-macros-web-0.3.5/invisibleroads_macros_web.egg-info/top_level.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2022-10-28 18:53:12.000000 invisibleroads-macros-web-0.3.5/invisibleroads_macros_web.egg-info/zip-safe
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       38 2023-05-23 18:26:10.289443 invisibleroads-macros-web-0.3.5/setup.cfg
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1374 2023-05-23 18:21:56.000000 invisibleroads-macros-web-0.3.5/setup.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-23 18:26:10.289443 invisibleroads-macros-web-0.3.5/tests/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2023-05-02 16:01:35.000000 invisibleroads-macros-web-0.3.5/tests/__init__.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      344 2022-10-28 18:39:04.000000 invisibleroads-macros-web-0.3.5/tests/test_escape.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      865 2023-05-23 18:24:12.000000 invisibleroads-macros-web-0.3.5/tests/test_markdown.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      882 2023-05-02 16:01:35.000000 invisibleroads-macros-web-0.3.5/tests/test_port.py
```

### Comparing `invisibleroads-macros-web-0.3.4/PKG-INFO` & `invisibleroads-macros-web-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invisibleroads-macros-web
-Version: 0.3.4
+Version: 0.3.5
 Summary: Shortcut functions for web operations
 Home-page: https://github.com/invisibleroads/invisibleroads-macros-web
 Author: Roy Hyunjin Han
 Author-email: rhh@crosscompute.com
 Keywords: invisibleroads
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `invisibleroads-macros-web-0.3.4/README.md` & `invisibleroads-macros-web-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `invisibleroads-macros-web-0.3.4/invisibleroads_macros_web/browser.py` & `invisibleroads-macros-web-0.3.5/invisibleroads_macros_web/browser.py`

 * *Files identical despite different names*

### Comparing `invisibleroads-macros-web-0.3.4/invisibleroads_macros_web/jinja.py` & `invisibleroads-macros-web-0.3.5/invisibleroads_macros_web/jinja.py`

 * *Files identical despite different names*

### Comparing `invisibleroads-macros-web-0.3.4/invisibleroads_macros_web/port.py` & `invisibleroads-macros-web-0.3.5/invisibleroads_macros_web/port.py`

 * *Files identical despite different names*

### Comparing `invisibleroads-macros-web-0.3.4/invisibleroads_macros_web/starlette.py` & `invisibleroads-macros-web-0.3.5/invisibleroads_macros_web/starlette.py`

 * *Files identical despite different names*

### Comparing `invisibleroads-macros-web-0.3.4/invisibleroads_macros_web.egg-info/PKG-INFO` & `invisibleroads-macros-web-0.3.5/invisibleroads_macros_web.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invisibleroads-macros-web
-Version: 0.3.4
+Version: 0.3.5
 Summary: Shortcut functions for web operations
 Home-page: https://github.com/invisibleroads/invisibleroads-macros-web
 Author: Roy Hyunjin Han
 Author-email: rhh@crosscompute.com
 Keywords: invisibleroads
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `invisibleroads-macros-web-0.3.4/invisibleroads_macros_web.egg-info/SOURCES.txt` & `invisibleroads-macros-web-0.3.5/invisibleroads_macros_web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invisibleroads-macros-web-0.3.4/setup.py` & `invisibleroads-macros-web-0.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 FOLDER = dirname(abspath(__file__))
 DESCRIPTION = '\n\n'.join(open(join(FOLDER, _)).read().strip() for _ in [
     'README.md', 'CHANGES.md'])
 
 
 setup(
     name='invisibleroads-macros-web',
-    version='0.3.4',
+    version='0.3.5',
     description='Shortcut functions for web operations',
     long_description=DESCRIPTION,
     long_description_content_type='text/markdown',
     classifiers=[
         'Programming Language :: Python',
         'License :: OSI Approved :: MIT License',
     ],
```

### Comparing `invisibleroads-macros-web-0.3.4/tests/test_markdown.py` & `invisibleroads-macros-web-0.3.5/tests/test_markdown.py`

 * *Files 27% similar despite different names*

```diff
@@ -16,12 +16,11 @@
     assert html == '<p>x</p><p>y</p>'
 
 
 def test_remove_parent_paragraphs():
     html = remove_parent_paragraphs(
         '<p>x</p><p><button>\n</button></p><p>x</p>')
     assert html == '<p>x</p><button>\n</button><p>x</p>'
-    html = remove_parent_paragraphs(
-        '<p>x</p><p><div>\n<a></a>\n</div></p><p>x</p>')
-    assert html == '<p>x</p><div>\n<a></a>\n</div><p>x</p>'
-    html = remove_parent_paragraphs('<p><strong>\n</strong></p>')
-    assert html == '<p><strong>\n</strong></p>'
+    html = remove_parent_paragraphs('<p><span>\n</span></p>', tags=[])
+    assert html == '<p><span>\n</span></p>'
+    html = remove_parent_paragraphs('<p><span>\n</span></p>', tags=['span'])
+    assert html == '<span>\n</span>'
```

### Comparing `invisibleroads-macros-web-0.3.4/tests/test_port.py` & `invisibleroads-macros-web-0.3.5/tests/test_port.py`

 * *Files identical despite different names*

