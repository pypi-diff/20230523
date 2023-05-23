# Comparing `tmp/mkdocs-simple-tags-plugin-0.8.tar.gz` & `tmp/mkdocs-simple-tags-plugin-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-simple-tags-plugin-0.8.tar", last modified: Mon May 15 18:44:20 2023, max compression
+gzip compressed data, was "mkdocs-simple-tags-plugin-0.9.tar", last modified: Mon May 15 19:10:37 2023, max compression
```

## Comparing `mkdocs-simple-tags-plugin-0.8.tar` & `mkdocs-simple-tags-plugin-0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-15 18:44:20.141341 mkdocs-simple-tags-plugin-0.8/
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)     5188 2023-05-15 18:44:20.141341 mkdocs-simple-tags-plugin-0.8/PKG-INFO
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)     3429 2023-05-15 16:23:29.000000 mkdocs-simple-tags-plugin-0.8/README.md
-drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-15 18:44:20.141341 mkdocs-simple-tags-plugin-0.8/mkdocs_simple_tags_plugin.egg-info/
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)     5188 2023-05-15 18:44:20.000000 mkdocs-simple-tags-plugin-0.8/mkdocs_simple_tags_plugin.egg-info/PKG-INFO
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)      388 2023-05-15 18:44:20.000000 mkdocs-simple-tags-plugin-0.8/mkdocs_simple_tags_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)        1 2023-05-15 18:44:20.000000 mkdocs-simple-tags-plugin-0.8/mkdocs_simple_tags_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)       55 2023-05-15 18:44:20.000000 mkdocs-simple-tags-plugin-0.8/mkdocs_simple_tags_plugin.egg-info/entry_points.txt
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)       14 2023-05-15 18:44:20.000000 mkdocs-simple-tags-plugin-0.8/mkdocs_simple_tags_plugin.egg-info/requires.txt
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)        5 2023-05-15 18:44:20.000000 mkdocs-simple-tags-plugin-0.8/mkdocs_simple_tags_plugin.egg-info/top_level.txt
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)      692 2023-05-15 18:44:20.141341 mkdocs-simple-tags-plugin-0.8/setup.cfg
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)      439 2023-05-15 18:44:06.000000 mkdocs-simple-tags-plugin-0.8/setup.py
-drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-15 18:44:20.141341 mkdocs-simple-tags-plugin-0.8/tags/
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)        1 2023-05-15 16:23:29.000000 mkdocs-simple-tags-plugin-0.8/tags/__init__.py
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)     4950 2023-05-15 18:37:29.000000 mkdocs-simple-tags-plugin-0.8/tags/plugin.py
-drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-15 18:44:20.141341 mkdocs-simple-tags-plugin-0.8/tags/templates/
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)      178 2023-05-15 17:59:27.000000 mkdocs-simple-tags-plugin-0.8/tags/templates/tags.md.template
+drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-15 19:10:37.583041 mkdocs-simple-tags-plugin-0.9/
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)     5188 2023-05-15 19:10:37.583041 mkdocs-simple-tags-plugin-0.9/PKG-INFO
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)     3429 2023-05-15 16:23:29.000000 mkdocs-simple-tags-plugin-0.9/README.md
+drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-15 19:10:37.583041 mkdocs-simple-tags-plugin-0.9/mkdocs_simple_tags_plugin.egg-info/
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)     5188 2023-05-15 19:10:37.000000 mkdocs-simple-tags-plugin-0.9/mkdocs_simple_tags_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)      388 2023-05-15 19:10:37.000000 mkdocs-simple-tags-plugin-0.9/mkdocs_simple_tags_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)        1 2023-05-15 19:10:37.000000 mkdocs-simple-tags-plugin-0.9/mkdocs_simple_tags_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)       55 2023-05-15 19:10:37.000000 mkdocs-simple-tags-plugin-0.9/mkdocs_simple_tags_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)       14 2023-05-15 19:10:37.000000 mkdocs-simple-tags-plugin-0.9/mkdocs_simple_tags_plugin.egg-info/requires.txt
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)        5 2023-05-15 19:10:37.000000 mkdocs-simple-tags-plugin-0.9/mkdocs_simple_tags_plugin.egg-info/top_level.txt
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)      692 2023-05-15 19:10:37.583041 mkdocs-simple-tags-plugin-0.9/setup.cfg
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)      439 2023-05-15 19:10:26.000000 mkdocs-simple-tags-plugin-0.9/setup.py
+drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-15 19:10:37.583041 mkdocs-simple-tags-plugin-0.9/tags/
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)        1 2023-05-15 16:23:29.000000 mkdocs-simple-tags-plugin-0.9/tags/__init__.py
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)     5020 2023-05-15 19:10:12.000000 mkdocs-simple-tags-plugin-0.9/tags/plugin.py
+drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-15 19:10:37.583041 mkdocs-simple-tags-plugin-0.9/tags/templates/
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)      178 2023-05-15 17:59:27.000000 mkdocs-simple-tags-plugin-0.9/tags/templates/tags.md.template
```

### Comparing `mkdocs-simple-tags-plugin-0.8/PKG-INFO` & `mkdocs-simple-tags-plugin-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-simple-tags-plugin
-Version: 0.8
+Version: 0.9
 Summary: "Create tags in mkdocs"
 Home-page: https://github.com/BeyondIM/mkdocs-simple-tags-plugin
 Author: BeyondIM
 Author-email: lypdarling@gmail.com
 License: MIT
 Description: # Tags
```

### Comparing `mkdocs-simple-tags-plugin-0.8/README.md` & `mkdocs-simple-tags-plugin-0.9/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-simple-tags-plugin-0.8/mkdocs_simple_tags_plugin.egg-info/PKG-INFO` & `mkdocs-simple-tags-plugin-0.9/mkdocs_simple_tags_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-simple-tags-plugin
-Version: 0.8
+Version: 0.9
 Summary: "Create tags in mkdocs"
 Home-page: https://github.com/BeyondIM/mkdocs-simple-tags-plugin
 Author: BeyondIM
 Author-email: lypdarling@gmail.com
 License: MIT
 Description: # Tags
```

### Comparing `mkdocs-simple-tags-plugin-0.8/setup.cfg` & `mkdocs-simple-tags-plugin-0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `mkdocs-simple-tags-plugin-0.8/tags/plugin.py` & `mkdocs-simple-tags-plugin-0.9/tags/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,16 @@
         takes markdown, page, config, and files
         currently modifies the markdown to add a button to click to get related tag info
         tag is customizeable by adding css that keys off the `self.css_name`
         """
         if 'tags' in page.meta:
             swap_mark = [f"[{x}](/{str(self.filename).strip('.md')}.html#{x}){{{self.css_name}}}"
                          for x in page.meta['tags']]
-            swap_mark.append('\n')
+            # swap_mark.append('\n')
+            swap_mark.prepend("<div class='tags'>").append("</div")
             return f'{" ".join(swap_mark)}{markdown}'
         return markdown
 
     def on_config(self, config):
         """Load config options"""
         self.filename = Path(self.config.get("filename") or self.filename)
         self.folder = Path(self.config.get("folder") or self.folder)
```

