# Comparing `tmp/mkdocs-simple-tags-plugin-1.2.tar.gz` & `tmp/mkdocs-simple-tags-plugin-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-simple-tags-plugin-1.2.tar", last modified: Mon May 15 19:30:11 2023, max compression
+gzip compressed data, was "mkdocs-simple-tags-plugin-1.3.tar", last modified: Mon May 15 19:39:52 2023, max compression
```

## Comparing `mkdocs-simple-tags-plugin-1.2.tar` & `mkdocs-simple-tags-plugin-1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-15 19:30:11.071401 mkdocs-simple-tags-plugin-1.2/
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)     5188 2023-05-15 19:30:11.071401 mkdocs-simple-tags-plugin-1.2/PKG-INFO
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)     3429 2023-05-15 16:23:29.000000 mkdocs-simple-tags-plugin-1.2/README.md
-drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-15 19:30:11.071401 mkdocs-simple-tags-plugin-1.2/mkdocs_simple_tags_plugin.egg-info/
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)     5188 2023-05-15 19:30:11.000000 mkdocs-simple-tags-plugin-1.2/mkdocs_simple_tags_plugin.egg-info/PKG-INFO
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)      388 2023-05-15 19:30:11.000000 mkdocs-simple-tags-plugin-1.2/mkdocs_simple_tags_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)        1 2023-05-15 19:30:11.000000 mkdocs-simple-tags-plugin-1.2/mkdocs_simple_tags_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)       55 2023-05-15 19:30:11.000000 mkdocs-simple-tags-plugin-1.2/mkdocs_simple_tags_plugin.egg-info/entry_points.txt
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)       14 2023-05-15 19:30:11.000000 mkdocs-simple-tags-plugin-1.2/mkdocs_simple_tags_plugin.egg-info/requires.txt
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)        5 2023-05-15 19:30:11.000000 mkdocs-simple-tags-plugin-1.2/mkdocs_simple_tags_plugin.egg-info/top_level.txt
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)      692 2023-05-15 19:30:11.071401 mkdocs-simple-tags-plugin-1.2/setup.cfg
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)      439 2023-05-15 19:30:01.000000 mkdocs-simple-tags-plugin-1.2/setup.py
-drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-15 19:30:11.071401 mkdocs-simple-tags-plugin-1.2/tags/
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)        1 2023-05-15 16:23:29.000000 mkdocs-simple-tags-plugin-1.2/tags/__init__.py
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)     4990 2023-05-15 19:29:39.000000 mkdocs-simple-tags-plugin-1.2/tags/plugin.py
-drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-15 19:30:11.071401 mkdocs-simple-tags-plugin-1.2/tags/templates/
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)      178 2023-05-15 17:59:27.000000 mkdocs-simple-tags-plugin-1.2/tags/templates/tags.md.template
+drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-15 19:39:52.951390 mkdocs-simple-tags-plugin-1.3/
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)     5188 2023-05-15 19:39:52.951390 mkdocs-simple-tags-plugin-1.3/PKG-INFO
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)     3429 2023-05-15 16:23:29.000000 mkdocs-simple-tags-plugin-1.3/README.md
+drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-15 19:39:52.951390 mkdocs-simple-tags-plugin-1.3/mkdocs_simple_tags_plugin.egg-info/
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)     5188 2023-05-15 19:39:52.000000 mkdocs-simple-tags-plugin-1.3/mkdocs_simple_tags_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)      388 2023-05-15 19:39:52.000000 mkdocs-simple-tags-plugin-1.3/mkdocs_simple_tags_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)        1 2023-05-15 19:39:52.000000 mkdocs-simple-tags-plugin-1.3/mkdocs_simple_tags_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)       55 2023-05-15 19:39:52.000000 mkdocs-simple-tags-plugin-1.3/mkdocs_simple_tags_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)       14 2023-05-15 19:39:52.000000 mkdocs-simple-tags-plugin-1.3/mkdocs_simple_tags_plugin.egg-info/requires.txt
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)        5 2023-05-15 19:39:52.000000 mkdocs-simple-tags-plugin-1.3/mkdocs_simple_tags_plugin.egg-info/top_level.txt
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)      692 2023-05-15 19:39:52.951390 mkdocs-simple-tags-plugin-1.3/setup.cfg
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)      439 2023-05-15 19:39:42.000000 mkdocs-simple-tags-plugin-1.3/setup.py
+drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-15 19:39:52.951390 mkdocs-simple-tags-plugin-1.3/tags/
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)        1 2023-05-15 16:23:29.000000 mkdocs-simple-tags-plugin-1.3/tags/__init__.py
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)     5163 2023-05-15 19:39:31.000000 mkdocs-simple-tags-plugin-1.3/tags/plugin.py
+drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-15 19:39:52.951390 mkdocs-simple-tags-plugin-1.3/tags/templates/
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)      178 2023-05-15 17:59:27.000000 mkdocs-simple-tags-plugin-1.3/tags/templates/tags.md.template
```

### Comparing `mkdocs-simple-tags-plugin-1.2/PKG-INFO` & `mkdocs-simple-tags-plugin-1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-simple-tags-plugin
-Version: 1.2
+Version: 1.3
 Summary: "Create tags in mkdocs"
 Home-page: https://github.com/BeyondIM/mkdocs-simple-tags-plugin
 Author: BeyondIM
 Author-email: lypdarling@gmail.com
 License: MIT
 Description: # Tags
```

### Comparing `mkdocs-simple-tags-plugin-1.2/README.md` & `mkdocs-simple-tags-plugin-1.3/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-simple-tags-plugin-1.2/mkdocs_simple_tags_plugin.egg-info/PKG-INFO` & `mkdocs-simple-tags-plugin-1.3/mkdocs_simple_tags_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-simple-tags-plugin
-Version: 1.2
+Version: 1.3
 Summary: "Create tags in mkdocs"
 Home-page: https://github.com/BeyondIM/mkdocs-simple-tags-plugin
 Author: BeyondIM
 Author-email: lypdarling@gmail.com
 License: MIT
 Description: # Tags
```

### Comparing `mkdocs-simple-tags-plugin-1.2/setup.cfg` & `mkdocs-simple-tags-plugin-1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `mkdocs-simple-tags-plugin-1.2/tags/plugin.py` & `mkdocs-simple-tags-plugin-1.3/tags/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,17 +44,19 @@
     def on_page_markdown(self, markdown, page, config, files):
         """
         takes markdown, page, config, and files
         currently modifies the markdown to add a button to click to get related tag info
         tag is customizeable by adding css that keys off the `self.css_name`
         """
         if 'tags' in page.meta:
-            swap_mark = [f"[{x}](/{str(self.filename).strip('.md')}.html#{x}){{{self.css_name}}}"
+            # swap_mark = [f"[{x}](/{str(self.filename).strip('.md')}.html#{x}){{{self.css_name}}}"
+            #              for x in page.meta['tags']]
+            swap_mark = [f"<a herf='/{str(self.filename).strip('.md')}.html#{x}' class='{self.css_name}'>{x}</a>"
                          for x in page.meta['tags']]
-            swap_mark.append('\n')
+            # swap_mark.append('\n')
             return "<div class='tags'>" + f'{" ".join(swap_mark)}' + "</div>" + f'{markdown}'
         return markdown
 
     def on_config(self, config):
         """Load config options"""
         self.filename = Path(self.config.get("filename") or self.filename)
         self.folder = Path(self.config.get("folder") or self.folder)
```

