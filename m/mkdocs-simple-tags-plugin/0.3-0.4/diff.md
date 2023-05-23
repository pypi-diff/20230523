# Comparing `tmp/mkdocs-simple-tags-plugin-0.3.tar.gz` & `tmp/mkdocs-simple-tags-plugin-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-simple-tags-plugin-0.3.tar", last modified: Tue May 23 07:52:28 2023, max compression
+gzip compressed data, was "mkdocs-simple-tags-plugin-0.4.tar", last modified: Tue May 23 08:43:34 2023, max compression
```

## Comparing `mkdocs-simple-tags-plugin-0.3.tar` & `mkdocs-simple-tags-plugin-0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-23 07:52:28.836894 mkdocs-simple-tags-plugin-0.3/
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)     1079 2023-05-23 06:24:49.000000 mkdocs-simple-tags-plugin-0.3/LICENSE.md
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)     4202 2023-05-23 07:52:28.836894 mkdocs-simple-tags-plugin-0.3/PKG-INFO
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)     3449 2023-05-23 07:51:57.000000 mkdocs-simple-tags-plugin-0.3/README.md
-drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-23 07:52:28.836894 mkdocs-simple-tags-plugin-0.3/mkdocs_simple_tags_plugin.egg-info/
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)     4202 2023-05-23 07:52:28.000000 mkdocs-simple-tags-plugin-0.3/mkdocs_simple_tags_plugin.egg-info/PKG-INFO
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)      399 2023-05-23 07:52:28.000000 mkdocs-simple-tags-plugin-0.3/mkdocs_simple_tags_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)        1 2023-05-23 07:52:28.000000 mkdocs-simple-tags-plugin-0.3/mkdocs_simple_tags_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)       54 2023-05-23 07:52:28.000000 mkdocs-simple-tags-plugin-0.3/mkdocs_simple_tags_plugin.egg-info/entry_points.txt
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)       14 2023-05-23 07:52:28.000000 mkdocs-simple-tags-plugin-0.3/mkdocs_simple_tags_plugin.egg-info/requires.txt
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)        5 2023-05-23 07:52:28.000000 mkdocs-simple-tags-plugin-0.3/mkdocs_simple_tags_plugin.egg-info/top_level.txt
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)      692 2023-05-23 07:52:28.837894 mkdocs-simple-tags-plugin-0.3/setup.cfg
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)      439 2023-05-23 07:50:51.000000 mkdocs-simple-tags-plugin-0.3/setup.py
-drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-23 07:52:28.836894 mkdocs-simple-tags-plugin-0.3/tags/
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)        1 2023-05-23 06:51:30.000000 mkdocs-simple-tags-plugin-0.3/tags/__init__.py
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)     4952 2023-05-23 07:49:59.000000 mkdocs-simple-tags-plugin-0.3/tags/plugin.py
-drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-23 07:52:28.836894 mkdocs-simple-tags-plugin-0.3/tags/templates/
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)      181 2023-05-23 06:29:22.000000 mkdocs-simple-tags-plugin-0.3/tags/templates/tags.md.template
+drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-23 08:43:34.831317 mkdocs-simple-tags-plugin-0.4/
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)     1079 2023-05-23 06:24:49.000000 mkdocs-simple-tags-plugin-0.4/LICENSE.md
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)     4182 2023-05-23 08:43:34.831317 mkdocs-simple-tags-plugin-0.4/PKG-INFO
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)     3429 2023-05-23 08:41:12.000000 mkdocs-simple-tags-plugin-0.4/README.md
+drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-23 08:43:34.831317 mkdocs-simple-tags-plugin-0.4/mkdocs_simple_tags_plugin.egg-info/
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)     4182 2023-05-23 08:43:34.000000 mkdocs-simple-tags-plugin-0.4/mkdocs_simple_tags_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)      399 2023-05-23 08:43:34.000000 mkdocs-simple-tags-plugin-0.4/mkdocs_simple_tags_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)        1 2023-05-23 08:43:34.000000 mkdocs-simple-tags-plugin-0.4/mkdocs_simple_tags_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)       54 2023-05-23 08:43:34.000000 mkdocs-simple-tags-plugin-0.4/mkdocs_simple_tags_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)       14 2023-05-23 08:43:34.000000 mkdocs-simple-tags-plugin-0.4/mkdocs_simple_tags_plugin.egg-info/requires.txt
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)        5 2023-05-23 08:43:34.000000 mkdocs-simple-tags-plugin-0.4/mkdocs_simple_tags_plugin.egg-info/top_level.txt
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)      692 2023-05-23 08:43:34.831317 mkdocs-simple-tags-plugin-0.4/setup.cfg
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)      439 2023-05-23 08:43:04.000000 mkdocs-simple-tags-plugin-0.4/setup.py
+drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-23 08:43:34.831317 mkdocs-simple-tags-plugin-0.4/tags/
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)        1 2023-05-23 06:51:30.000000 mkdocs-simple-tags-plugin-0.4/tags/__init__.py
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)     4950 2023-05-23 08:03:21.000000 mkdocs-simple-tags-plugin-0.4/tags/plugin.py
+drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-23 08:43:34.831317 mkdocs-simple-tags-plugin-0.4/tags/templates/
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)      181 2023-05-23 06:29:22.000000 mkdocs-simple-tags-plugin-0.4/tags/templates/tags.md.template
```

### Comparing `mkdocs-simple-tags-plugin-0.3/LICENSE.md` & `mkdocs-simple-tags-plugin-0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mkdocs-simple-tags-plugin-0.3/PKG-INFO` & `mkdocs-simple-tags-plugin-0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-simple-tags-plugin
-Version: 0.3
+Version: 0.4
 Summary: "Create tags in mkdocs"
 Home-page: https://github.com/BeyondIM/mkdocs-simple-tags-plugin
 Author: BeyondIM
 Author-email: lypdarling@gmail.com
 License: MIT
 Keywords: "mkdocs python markdown tags"
 Classifier: Intended Audience :: Developers
@@ -120,27 +120,27 @@
 different layout or metadata. The `page` object contains all the metadata
 in a mkdocs page, and in addition a `.filename` attribute, which contains
 the file name of the source of the page (relative to the docs folder),
 which can be used to link to that page.
 
 The full customizable options for the plugin are:
 
-* `tags_folder`: Folder in which the auxiliar tags markdown file will be written
+* `folder`: Folder in which the auxiliar tags markdown file will be written
   (`aux` by default, relative to the folder in which `mkdocs` is invoked).
   It can be set to an absolute path, such as `/tmp/mysite/aux`.
   The required folders are created.
-* `tags_template`: path to the file which contains the markdown-jinja template
+* `template`: path to the file which contains the markdown-jinja template
   for the tags page. It is `None` by default, which means that the
   package-provided template is used. It can be an absolute path,
   or relative to the folder in which `mkdocs` is run.
 * `css_name`: this allows you to pick what name styles the tag that appears on
   the top of the page that contains a tag. This way things won't be overloaded
 
 For example, this can be put at `mkdocs.yaml`:
 
 ```yaml
 plugins:
     - search
     - simple-tags:
-        tags_folder: /tmp/mysite/aux
-        tags_template: docs/theme/tags.md.template
+        folder: /tmp/mysite/aux
+        template: docs/theme/tags.md.template
 ```
```

### Comparing `mkdocs-simple-tags-plugin-0.3/README.md` & `mkdocs-simple-tags-plugin-0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -99,27 +99,27 @@
 different layout or metadata. The `page` object contains all the metadata
 in a mkdocs page, and in addition a `.filename` attribute, which contains
 the file name of the source of the page (relative to the docs folder),
 which can be used to link to that page.
 
 The full customizable options for the plugin are:
 
-* `tags_folder`: Folder in which the auxiliar tags markdown file will be written
+* `folder`: Folder in which the auxiliar tags markdown file will be written
   (`aux` by default, relative to the folder in which `mkdocs` is invoked).
   It can be set to an absolute path, such as `/tmp/mysite/aux`.
   The required folders are created.
-* `tags_template`: path to the file which contains the markdown-jinja template
+* `template`: path to the file which contains the markdown-jinja template
   for the tags page. It is `None` by default, which means that the
   package-provided template is used. It can be an absolute path,
   or relative to the folder in which `mkdocs` is run.
 * `css_name`: this allows you to pick what name styles the tag that appears on
   the top of the page that contains a tag. This way things won't be overloaded
 
 For example, this can be put at `mkdocs.yaml`:
 
 ```yaml
 plugins:
     - search
     - simple-tags:
-        tags_folder: /tmp/mysite/aux
-        tags_template: docs/theme/tags.md.template
+        folder: /tmp/mysite/aux
+        template: docs/theme/tags.md.template
 ```
```

### Comparing `mkdocs-simple-tags-plugin-0.3/mkdocs_simple_tags_plugin.egg-info/PKG-INFO` & `mkdocs-simple-tags-plugin-0.4/mkdocs_simple_tags_plugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-simple-tags-plugin
-Version: 0.3
+Version: 0.4
 Summary: "Create tags in mkdocs"
 Home-page: https://github.com/BeyondIM/mkdocs-simple-tags-plugin
 Author: BeyondIM
 Author-email: lypdarling@gmail.com
 License: MIT
 Keywords: "mkdocs python markdown tags"
 Classifier: Intended Audience :: Developers
@@ -120,27 +120,27 @@
 different layout or metadata. The `page` object contains all the metadata
 in a mkdocs page, and in addition a `.filename` attribute, which contains
 the file name of the source of the page (relative to the docs folder),
 which can be used to link to that page.
 
 The full customizable options for the plugin are:
 
-* `tags_folder`: Folder in which the auxiliar tags markdown file will be written
+* `folder`: Folder in which the auxiliar tags markdown file will be written
   (`aux` by default, relative to the folder in which `mkdocs` is invoked).
   It can be set to an absolute path, such as `/tmp/mysite/aux`.
   The required folders are created.
-* `tags_template`: path to the file which contains the markdown-jinja template
+* `template`: path to the file which contains the markdown-jinja template
   for the tags page. It is `None` by default, which means that the
   package-provided template is used. It can be an absolute path,
   or relative to the folder in which `mkdocs` is run.
 * `css_name`: this allows you to pick what name styles the tag that appears on
   the top of the page that contains a tag. This way things won't be overloaded
 
 For example, this can be put at `mkdocs.yaml`:
 
 ```yaml
 plugins:
     - search
     - simple-tags:
-        tags_folder: /tmp/mysite/aux
-        tags_template: docs/theme/tags.md.template
+        folder: /tmp/mysite/aux
+        template: docs/theme/tags.md.template
 ```
```

### Comparing `mkdocs-simple-tags-plugin-0.3/setup.cfg` & `mkdocs-simple-tags-plugin-0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `mkdocs-simple-tags-plugin-0.3/tags/plugin.py` & `mkdocs-simple-tags-plugin-0.4/tags/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         takes markdown, page, config, and files
         currently modifies the markdown to add a button to click to get related tag info
         tag is customizeable by adding css that keys off the `self.css_name`
         """
         if 'tags' in page.meta:
             swap_mark = [f"[{x}](/{str(self.filename).strip('.md')}.html#{x}){{{self.css_name}}}"
                          for x in page.meta['tags']]
-            # swap_mark.append('\n')
+            swap_mark.append('\n')
             return f'{" ".join(swap_mark)}{markdown}'
         return markdown
 
     def on_config(self, config):
         """Load config options"""
         self.filename = Path(self.config.get("filename") or self.filename)
         self.folder = Path(self.config.get("folder") or self.folder)
```

