# Comparing `tmp/mkdocs-simple-tags-plugin-1.0.tar.gz` & `tmp/mkdocs-simple-tags-plugin-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-simple-tags-plugin-1.0.tar", last modified: Mon May 15 19:16:05 2023, max compression
+gzip compressed data, was "mkdocs-simple-tags-plugin-1.1.tar", last modified: Mon May 15 19:20:32 2023, max compression
```

## Comparing `mkdocs-simple-tags-plugin-1.0.tar` & `mkdocs-simple-tags-plugin-1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-15 19:16:05.757217 mkdocs-simple-tags-plugin-1.0/
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)     5188 2023-05-15 19:16:05.757217 mkdocs-simple-tags-plugin-1.0/PKG-INFO
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)     3429 2023-05-15 16:23:29.000000 mkdocs-simple-tags-plugin-1.0/README.md
-drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-15 19:16:05.757217 mkdocs-simple-tags-plugin-1.0/mkdocs_simple_tags_plugin.egg-info/
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)     5188 2023-05-15 19:16:05.000000 mkdocs-simple-tags-plugin-1.0/mkdocs_simple_tags_plugin.egg-info/PKG-INFO
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)      388 2023-05-15 19:16:05.000000 mkdocs-simple-tags-plugin-1.0/mkdocs_simple_tags_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)        1 2023-05-15 19:16:05.000000 mkdocs-simple-tags-plugin-1.0/mkdocs_simple_tags_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)       55 2023-05-15 19:16:05.000000 mkdocs-simple-tags-plugin-1.0/mkdocs_simple_tags_plugin.egg-info/entry_points.txt
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)       14 2023-05-15 19:16:05.000000 mkdocs-simple-tags-plugin-1.0/mkdocs_simple_tags_plugin.egg-info/requires.txt
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)        5 2023-05-15 19:16:05.000000 mkdocs-simple-tags-plugin-1.0/mkdocs_simple_tags_plugin.egg-info/top_level.txt
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)      692 2023-05-15 19:16:05.757217 mkdocs-simple-tags-plugin-1.0/setup.cfg
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)      439 2023-05-15 19:15:52.000000 mkdocs-simple-tags-plugin-1.0/setup.py
-drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-15 19:16:05.757217 mkdocs-simple-tags-plugin-1.0/tags/
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)        1 2023-05-15 16:23:29.000000 mkdocs-simple-tags-plugin-1.0/tags/__init__.py
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)     5022 2023-05-15 19:15:35.000000 mkdocs-simple-tags-plugin-1.0/tags/plugin.py
-drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-15 19:16:05.757217 mkdocs-simple-tags-plugin-1.0/tags/templates/
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)      178 2023-05-15 17:59:27.000000 mkdocs-simple-tags-plugin-1.0/tags/templates/tags.md.template
+drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-15 19:20:32.300557 mkdocs-simple-tags-plugin-1.1/
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)     5188 2023-05-15 19:20:32.300557 mkdocs-simple-tags-plugin-1.1/PKG-INFO
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)     3429 2023-05-15 16:23:29.000000 mkdocs-simple-tags-plugin-1.1/README.md
+drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-15 19:20:32.300557 mkdocs-simple-tags-plugin-1.1/mkdocs_simple_tags_plugin.egg-info/
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)     5188 2023-05-15 19:20:32.000000 mkdocs-simple-tags-plugin-1.1/mkdocs_simple_tags_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)      388 2023-05-15 19:20:32.000000 mkdocs-simple-tags-plugin-1.1/mkdocs_simple_tags_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)        1 2023-05-15 19:20:32.000000 mkdocs-simple-tags-plugin-1.1/mkdocs_simple_tags_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)       55 2023-05-15 19:20:32.000000 mkdocs-simple-tags-plugin-1.1/mkdocs_simple_tags_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)       14 2023-05-15 19:20:32.000000 mkdocs-simple-tags-plugin-1.1/mkdocs_simple_tags_plugin.egg-info/requires.txt
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)        5 2023-05-15 19:20:32.000000 mkdocs-simple-tags-plugin-1.1/mkdocs_simple_tags_plugin.egg-info/top_level.txt
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)      692 2023-05-15 19:20:32.300557 mkdocs-simple-tags-plugin-1.1/setup.cfg
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)      439 2023-05-15 19:20:21.000000 mkdocs-simple-tags-plugin-1.1/setup.py
+drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-15 19:20:32.300557 mkdocs-simple-tags-plugin-1.1/tags/
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)        1 2023-05-15 16:23:29.000000 mkdocs-simple-tags-plugin-1.1/tags/__init__.py
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)     5044 2023-05-15 19:20:07.000000 mkdocs-simple-tags-plugin-1.1/tags/plugin.py
+drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-15 19:20:32.300557 mkdocs-simple-tags-plugin-1.1/tags/templates/
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)      178 2023-05-15 17:59:27.000000 mkdocs-simple-tags-plugin-1.1/tags/templates/tags.md.template
```

### Comparing `mkdocs-simple-tags-plugin-1.0/PKG-INFO` & `mkdocs-simple-tags-plugin-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-simple-tags-plugin
-Version: 1.0
+Version: 1.1
 Summary: "Create tags in mkdocs"
 Home-page: https://github.com/BeyondIM/mkdocs-simple-tags-plugin
 Author: BeyondIM
 Author-email: lypdarling@gmail.com
 License: MIT
 Description: # Tags
```

### Comparing `mkdocs-simple-tags-plugin-1.0/README.md` & `mkdocs-simple-tags-plugin-1.1/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-simple-tags-plugin-1.0/mkdocs_simple_tags_plugin.egg-info/PKG-INFO` & `mkdocs-simple-tags-plugin-1.1/mkdocs_simple_tags_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-simple-tags-plugin
-Version: 1.0
+Version: 1.1
 Summary: "Create tags in mkdocs"
 Home-page: https://github.com/BeyondIM/mkdocs-simple-tags-plugin
 Author: BeyondIM
 Author-email: lypdarling@gmail.com
 License: MIT
 Description: # Tags
```

### Comparing `mkdocs-simple-tags-plugin-1.0/setup.cfg` & `mkdocs-simple-tags-plugin-1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `mkdocs-simple-tags-plugin-1.0/tags/plugin.py` & `mkdocs-simple-tags-plugin-1.1/tags/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,16 @@
         currently modifies the markdown to add a button to click to get related tag info
         tag is customizeable by adding css that keys off the `self.css_name`
         """
         if 'tags' in page.meta:
             swap_mark = [f"[{x}](/{str(self.filename).strip('.md')}.html#{x}){{{self.css_name}}}"
                          for x in page.meta['tags']]
             # swap_mark.append('\n')
-            swap_mark.insert(0, "<div class='tags'>").append("</div")
+            swap_mark.insert(0, "<div class='tags'>")
+            swap_mark.append("</div")
             return f'{" ".join(swap_mark)}{markdown}'
         return markdown
 
     def on_config(self, config):
         """Load config options"""
         self.filename = Path(self.config.get("filename") or self.filename)
         self.folder = Path(self.config.get("folder") or self.folder)
```

