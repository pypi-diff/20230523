# Comparing `tmp/emark-1.0rc5.tar.gz` & `tmp/emark-1.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emark-1.0rc5.tar", last modified: Wed Mar 29 18:46:46 2023, max compression
+gzip compressed data, was "emark-1.0rc6.tar", last modified: Tue Apr 25 15:25:13 2023, max compression
```

## Comparing `emark-1.0rc5.tar` & `emark-1.0rc6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1518 2023-03-29 18:46:20.094896 emark-1.0rc5/LICENSE
--rw-r--r--   0        0        0     4038 2023-03-29 18:46:20.094896 emark-1.0rc5/README.md
--rw-r--r--   0        0        0      152 2023-03-29 18:46:20.094896 emark-1.0rc5/emark/__init__.py
--rw-r--r--   0        0        0      158 2023-03-29 18:46:46.822988 emark-1.0rc5/emark/_version.py
--rw-r--r--   0        0        0      281 2023-03-29 18:46:20.094896 emark-1.0rc5/emark/conf.py
--rw-r--r--   0        0        0     6550 2023-03-29 18:46:20.094896 emark-1.0rc5/emark/message.py
--rw-r--r--   0        0        0     2204 2023-03-29 18:46:20.094896 emark-1.0rc5/emark/templates/emark/base.html
--rw-r--r--   0        0        0     1081 2023-03-29 18:46:20.094896 emark-1.0rc5/emark/templates/emark/license.txt
--rw-r--r--   0        0        0     5822 2023-03-29 18:46:20.094896 emark-1.0rc5/emark/templates/emark/styles.css
--rw-r--r--   0        0        0     3780 2023-03-29 18:46:20.094896 emark-1.0rc5/emark/utils.py
--rw-r--r--   0        0        0     2257 2023-03-29 18:46:20.094896 emark-1.0rc5/pyproject.toml
--rw-r--r--   0        0        0     5728 1970-01-01 00:00:00.000000 emark-1.0rc5/PKG-INFO
+-rw-r--r--   0        0        0     1518 2023-04-25 15:24:45.038876 emark-1.0rc6/LICENSE
+-rw-r--r--   0        0        0     4038 2023-04-25 15:24:45.038876 emark-1.0rc6/README.md
+-rw-r--r--   0        0        0      152 2023-04-25 15:24:45.038876 emark-1.0rc6/emark/__init__.py
+-rw-r--r--   0        0        0      158 2023-04-25 15:25:13.895214 emark-1.0rc6/emark/_version.py
+-rw-r--r--   0        0        0      281 2023-04-25 15:24:45.038876 emark-1.0rc6/emark/conf.py
+-rw-r--r--   0        0        0     6550 2023-04-25 15:24:45.038876 emark-1.0rc6/emark/message.py
+-rw-r--r--   0        0        0     2414 2023-04-25 15:24:45.038876 emark-1.0rc6/emark/templates/emark/base.html
+-rw-r--r--   0        0        0     1081 2023-04-25 15:24:45.038876 emark-1.0rc6/emark/templates/emark/license.txt
+-rw-r--r--   0        0        0     5822 2023-04-25 15:24:45.038876 emark-1.0rc6/emark/templates/emark/styles.css
+-rw-r--r--   0        0        0     3780 2023-04-25 15:24:45.038876 emark-1.0rc6/emark/utils.py
+-rw-r--r--   0        0        0     2257 2023-04-25 15:24:45.038876 emark-1.0rc6/pyproject.toml
+-rw-r--r--   0        0        0     5728 1970-01-01 00:00:00.000000 emark-1.0rc6/PKG-INFO
```

### Comparing `emark-1.0rc5/LICENSE` & `emark-1.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `emark-1.0rc5/README.md` & `emark-1.0rc6/README.md`

 * *Files identical despite different names*

### Comparing `emark-1.0rc5/emark/message.py` & `emark-1.0rc6/emark/message.py`

 * *Files identical despite different names*

### Comparing `emark-1.0rc5/emark/templates/emark/base.html` & `emark-1.0rc6/emark/templates/emark/base.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {% load i18n %}
-<!doctype html>
+<!DOCTYPE html>
 <html>
   <head>
-    <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
-    <meta http-equiv="Content-Type" content="text/html; charset=UTF-8"/>
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
+    <meta http-equiv="Content-Type" content="text/html; charset=UTF-8" />
     <title>{{ subject }}</title>
     {% block styles %}
       <style>{% include "emark/styles.css" %}</style>
     {% endblock styles %}
   </head>
   <body>
     {% block preheader %}
@@ -21,33 +21,37 @@
            cellspacing="0"
            class="body">
       <tr>
         <td class="container-padding">&#xfeff;</td>
         <td class="container">
           <div class="content">
             <!-- START CENTERED WHITE CONTAINER -->
-            <table role="presentation" class="main">
-              <!-- START MAIN CONTENT AREA -->
-              <tr>
-                <td class="wrapper">
-                  <table role="presentation" border="0" cellpadding="0" cellspacing="0">
-                    <tr>
-                      <td>
-                        <!-- START ACTUAL CONTENT -->
-                        {% spaceless %}
-                          {% block content %}{{ markdown_string }}{% endblock %}
-                        {% endspaceless %}
-                        <!-- END ACTUAL CONTENT -->
-                      </td>
-                    </tr>
-                  </table>
-                </td>
-              </tr>
-              <!-- END MAIN CONTENT AREA -->
-            </table>
+            {% block container %}
+              <table role="presentation" class="main">
+                <!-- START MAIN CONTENT AREA -->
+                {% block main %}
+                  <tr>
+                    <td class="wrapper">
+                      <table role="presentation" border="0" cellpadding="0" cellspacing="0">
+                        <tr>
+                          <td>
+                            <!-- START ACTUAL CONTENT -->
+                            {% spaceless %}
+                              {% block content %}{{ markdown_string }}{% endblock %}
+                            {% endspaceless %}
+                            <!-- END ACTUAL CONTENT -->
+                          </td>
+                        </tr>
+                      </table>
+                    </td>
+                  </tr>
+                {% endblock main %}
+                <!-- END MAIN CONTENT AREA -->
+              </table>
+            {% endblock container %}
             <!-- END CENTERED WHITE CONTAINER -->
             <!-- START FOOTER -->
             <div class="footer">
               <table role="presentation" border="0" cellpadding="0" cellspacing="0">
                 <tr>
                   <td class="content-block">
                     {% spaceless %}
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
 {% load i18n %}
 
 {% block styles %}
  {% endblock styles %}
 {% block preheader %} {% spaceless %}  {% endspaceless %} {% endblock preheader
 %}
+          {% block container %}
           {% spaceless %} {% block content %}{{ markdown_string }}{%
-         endblock %} {% endspaceless %}
-&#xfeff;                                                             &#xfeff;
+&#xfeff; endblock %} {% endspaceless %}                              &#xfeff;
+         {% endblock container %}
          {% spaceless %} {% block footer %}{% endblock %} {%
          endspaceless %}
```

### Comparing `emark-1.0rc5/emark/templates/emark/license.txt` & `emark-1.0rc6/emark/templates/emark/license.txt`

 * *Files identical despite different names*

### Comparing `emark-1.0rc5/emark/templates/emark/styles.css` & `emark-1.0rc6/emark/templates/emark/styles.css`

 * *Files identical despite different names*

### Comparing `emark-1.0rc5/emark/utils.py` & `emark-1.0rc6/emark/utils.py`

 * *Files identical despite different names*

### Comparing `emark-1.0rc5/pyproject.toml` & `emark-1.0rc6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `emark-1.0rc5/PKG-INFO` & `emark-1.0rc6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emark
-Version: 1.0rc5
+Version: 1.0rc6
 Summary: Markdown template based HTML and text emails for Django.
 Keywords: Markdown,Django,email,templates,HTML
 Author-email: Rust Saiargaliev <fly.amureki@gmail.com>, Johannes Maron <johannes@maron.family>, Mostafa Mohamed <mostafa.anm91@gmail.com>, Jacqueline Kraus <jacquelinekraus1992@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

