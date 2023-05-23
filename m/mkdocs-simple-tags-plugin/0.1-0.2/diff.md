# Comparing `tmp/mkdocs-simple-tags-plugin-0.1.tar.gz` & `tmp/mkdocs-simple-tags-plugin-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-simple-tags-plugin-0.1.tar", last modified: Tue May 23 06:56:55 2023, max compression
+gzip compressed data, was "mkdocs-simple-tags-plugin-0.2.tar", last modified: Tue May 23 07:28:40 2023, max compression
```

## Comparing `mkdocs-simple-tags-plugin-0.1.tar` & `mkdocs-simple-tags-plugin-0.2.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-23 06:56:55.912777 mkdocs-simple-tags-plugin-0.1/
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)     1079 2023-05-23 06:24:49.000000 mkdocs-simple-tags-plugin-0.1/LICENSE.md
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)       47 2023-05-23 06:24:49.000000 mkdocs-simple-tags-plugin-0.1/MANIFEST.in
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)     4153 2023-05-23 06:56:55.912777 mkdocs-simple-tags-plugin-0.1/PKG-INFO
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)     3400 2023-05-23 06:24:49.000000 mkdocs-simple-tags-plugin-0.1/README.md
-drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-23 06:56:55.911777 mkdocs-simple-tags-plugin-0.1/mkdocs_simple_tags_plugin.egg-info/
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)     4153 2023-05-23 06:56:55.000000 mkdocs-simple-tags-plugin-0.1/mkdocs_simple_tags_plugin.egg-info/PKG-INFO
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)      411 2023-05-23 06:56:55.000000 mkdocs-simple-tags-plugin-0.1/mkdocs_simple_tags_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)        1 2023-05-23 06:56:55.000000 mkdocs-simple-tags-plugin-0.1/mkdocs_simple_tags_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)       47 2023-05-23 06:56:55.000000 mkdocs-simple-tags-plugin-0.1/mkdocs_simple_tags_plugin.egg-info/entry_points.txt
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)       14 2023-05-23 06:56:55.000000 mkdocs-simple-tags-plugin-0.1/mkdocs_simple_tags_plugin.egg-info/requires.txt
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)        5 2023-05-23 06:56:55.000000 mkdocs-simple-tags-plugin-0.1/mkdocs_simple_tags_plugin.egg-info/top_level.txt
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)      692 2023-05-23 06:56:55.912777 mkdocs-simple-tags-plugin-0.1/setup.cfg
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)      432 2023-05-23 06:53:24.000000 mkdocs-simple-tags-plugin-0.1/setup.py
-drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-23 06:56:55.911777 mkdocs-simple-tags-plugin-0.1/tags/
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)        1 2023-05-23 06:51:30.000000 mkdocs-simple-tags-plugin-0.1/tags/__init__.py
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)     4950 2023-05-23 06:24:49.000000 mkdocs-simple-tags-plugin-0.1/tags/plugin.py
-drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-23 06:56:55.912777 mkdocs-simple-tags-plugin-0.1/tags/templates/
--rw-r--r--   0 beyondim  (8076) beyondim  (8076)      181 2023-05-23 06:29:22.000000 mkdocs-simple-tags-plugin-0.1/tags/templates/tags.md.template
+drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-23 07:28:40.948657 mkdocs-simple-tags-plugin-0.2/
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)     1079 2023-05-23 06:24:49.000000 mkdocs-simple-tags-plugin-0.2/LICENSE.md
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)     4175 2023-05-23 07:28:40.948657 mkdocs-simple-tags-plugin-0.2/PKG-INFO
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)     3422 2023-05-23 07:26:49.000000 mkdocs-simple-tags-plugin-0.2/README.md
+drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-23 07:28:40.948657 mkdocs-simple-tags-plugin-0.2/mkdocs_simple_tags_plugin.egg-info/
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)     4175 2023-05-23 07:28:40.000000 mkdocs-simple-tags-plugin-0.2/mkdocs_simple_tags_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)      399 2023-05-23 07:28:40.000000 mkdocs-simple-tags-plugin-0.2/mkdocs_simple_tags_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)        1 2023-05-23 07:28:40.000000 mkdocs-simple-tags-plugin-0.2/mkdocs_simple_tags_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)       54 2023-05-23 07:28:40.000000 mkdocs-simple-tags-plugin-0.2/mkdocs_simple_tags_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)       14 2023-05-23 07:28:40.000000 mkdocs-simple-tags-plugin-0.2/mkdocs_simple_tags_plugin.egg-info/requires.txt
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)        5 2023-05-23 07:28:40.000000 mkdocs-simple-tags-plugin-0.2/mkdocs_simple_tags_plugin.egg-info/top_level.txt
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)      692 2023-05-23 07:28:40.948657 mkdocs-simple-tags-plugin-0.2/setup.cfg
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)      439 2023-05-23 07:28:36.000000 mkdocs-simple-tags-plugin-0.2/setup.py
+drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-23 07:28:40.948657 mkdocs-simple-tags-plugin-0.2/tags/
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)        1 2023-05-23 06:51:30.000000 mkdocs-simple-tags-plugin-0.2/tags/__init__.py
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)     4950 2023-05-23 06:24:49.000000 mkdocs-simple-tags-plugin-0.2/tags/plugin.py
+drwxr-xr-x   0 beyondim  (8076) beyondim  (8076)        0 2023-05-23 07:28:40.948657 mkdocs-simple-tags-plugin-0.2/tags/templates/
+-rw-r--r--   0 beyondim  (8076) beyondim  (8076)      181 2023-05-23 06:29:22.000000 mkdocs-simple-tags-plugin-0.2/tags/templates/tags.md.template
```

### Comparing `mkdocs-simple-tags-plugin-0.1/LICENSE.md` & `mkdocs-simple-tags-plugin-0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mkdocs-simple-tags-plugin-0.1/PKG-INFO` & `mkdocs-simple-tags-plugin-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-simple-tags-plugin
-Version: 0.1
+Version: 0.2
 Summary: "Create tags in mkdocs"
 Home-page: https://github.com/BeyondIM/mkdocs-simple-tags-plugin
 Author: BeyondIM
 Author-email: lypdarling@gmail.com
 License: MIT
 Keywords: "mkdocs python markdown tags"
 Classifier: Intended Audience :: Developers
@@ -27,15 +27,15 @@
 and all pages for each tag.
 
 ## Quick Demo
 
 Install this plugin (it will also install mkdocs if required)
 
 ```bash
-pip install mkdocs-plugin-tags
+pip install mkdocs-simple-tags-plugin
 ```
 
 Create a new documentation folder:
 
 ```bash
 mkdocs new demo
 ```
@@ -61,15 +61,15 @@
 ^D
 ```
 
 Edit `mkdocs.yml` to include this plugin:
 
 ```yaml
 plugins:
-  - tags:
+  - simple-tags:
 ```
 
 Run the server:
 
 ```bash
 mkdocs serve --livereload
 ```
@@ -102,14 +102,15 @@
 title: Tags
 ---
 # Contents grouped by tag
 
 {% for tag, pages in tags %}
 
 ## <span class="tag">{{tag}}</span>
+
 {%  for page in pages %}
   * [{{page.title}}]({{page.filename}})
 {% endfor %}
 
 {% endfor %}
 ```
 
@@ -135,11 +136,11 @@
   the top of the page that contains a tag. This way things won't be overloaded
 
 For example, this can be put at `mkdocs.yaml`:
 
 ```yaml
 plugins:
     - search
-    - tags:
+    - simple-tags:
         tags_folder: /tmp/mysite/aux
         tags_template: docs/theme/tags.md.template
 ```
```

### Comparing `mkdocs-simple-tags-plugin-0.1/README.md` & `mkdocs-simple-tags-plugin-0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 and all pages for each tag.
 
 ## Quick Demo
 
 Install this plugin (it will also install mkdocs if required)
 
 ```bash
-pip install mkdocs-plugin-tags
+pip install mkdocs-simple-tags-plugin
 ```
 
 Create a new documentation folder:
 
 ```bash
 mkdocs new demo
 ```
@@ -40,15 +40,15 @@
 ^D
 ```
 
 Edit `mkdocs.yml` to include this plugin:
 
 ```yaml
 plugins:
-  - tags:
+  - simple-tags:
 ```
 
 Run the server:
 
 ```bash
 mkdocs serve --livereload
 ```
@@ -81,14 +81,15 @@
 title: Tags
 ---
 # Contents grouped by tag
 
 {% for tag, pages in tags %}
 
 ## <span class="tag">{{tag}}</span>
+
 {%  for page in pages %}
   * [{{page.title}}]({{page.filename}})
 {% endfor %}
 
 {% endfor %}
 ```
 
@@ -114,11 +115,11 @@
   the top of the page that contains a tag. This way things won't be overloaded
 
 For example, this can be put at `mkdocs.yaml`:
 
 ```yaml
 plugins:
     - search
-    - tags:
+    - simple-tags:
         tags_folder: /tmp/mysite/aux
         tags_template: docs/theme/tags.md.template
 ```
```

### Comparing `mkdocs-simple-tags-plugin-0.1/mkdocs_simple_tags_plugin.egg-info/PKG-INFO` & `mkdocs-simple-tags-plugin-0.2/mkdocs_simple_tags_plugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-simple-tags-plugin
-Version: 0.1
+Version: 0.2
 Summary: "Create tags in mkdocs"
 Home-page: https://github.com/BeyondIM/mkdocs-simple-tags-plugin
 Author: BeyondIM
 Author-email: lypdarling@gmail.com
 License: MIT
 Keywords: "mkdocs python markdown tags"
 Classifier: Intended Audience :: Developers
@@ -27,15 +27,15 @@
 and all pages for each tag.
 
 ## Quick Demo
 
 Install this plugin (it will also install mkdocs if required)
 
 ```bash
-pip install mkdocs-plugin-tags
+pip install mkdocs-simple-tags-plugin
 ```
 
 Create a new documentation folder:
 
 ```bash
 mkdocs new demo
 ```
@@ -61,15 +61,15 @@
 ^D
 ```
 
 Edit `mkdocs.yml` to include this plugin:
 
 ```yaml
 plugins:
-  - tags:
+  - simple-tags:
 ```
 
 Run the server:
 
 ```bash
 mkdocs serve --livereload
 ```
@@ -102,14 +102,15 @@
 title: Tags
 ---
 # Contents grouped by tag
 
 {% for tag, pages in tags %}
 
 ## <span class="tag">{{tag}}</span>
+
 {%  for page in pages %}
   * [{{page.title}}]({{page.filename}})
 {% endfor %}
 
 {% endfor %}
 ```
 
@@ -135,11 +136,11 @@
   the top of the page that contains a tag. This way things won't be overloaded
 
 For example, this can be put at `mkdocs.yaml`:
 
 ```yaml
 plugins:
     - search
-    - tags:
+    - simple-tags:
         tags_folder: /tmp/mysite/aux
         tags_template: docs/theme/tags.md.template
 ```
```

### Comparing `mkdocs-simple-tags-plugin-0.1/setup.cfg` & `mkdocs-simple-tags-plugin-0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `mkdocs-simple-tags-plugin-0.1/tags/plugin.py` & `mkdocs-simple-tags-plugin-0.2/tags/plugin.py`

 * *Files identical despite different names*

