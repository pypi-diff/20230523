# Comparing `tmp/fling_start-0.1.8.tar.gz` & `tmp/fling_start-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fling_start-0.1.8.tar", max compression
+gzip compressed data, was "fling_start-0.1.9.tar", max compression
```

## Comparing `fling_start-0.1.8.tar` & `fling_start-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      156 2023-04-26 00:22:00.443542 fling_start-0.1.8/README.md
--rw-r--r--   0        0        0        6 2023-04-27 17:28:33.441460 fling_start-0.1.8/VERSION
--rw-r--r--   0        0        0        0 2023-04-19 21:06:07.644598 fling_start-0.1.8/fling/__init__.py
--rw-r--r--   0        0        0     1113 2023-04-27 05:22:45.984819 fling_start-0.1.8/fling/middleware.py
--rw-r--r--   0        0        0     4127 2023-04-27 16:49:54.982507 fling_start-0.1.8/fling/start.py
--rw-r--r--   0        0        0      778 2023-04-27 02:17:04.926768 fling_start-0.1.8/fling/static/start/styles.css
--rw-r--r--   0        0        0      487 2023-04-27 16:49:12.318822 fling_start-0.1.8/fling/templates/admin/index.html
--rw-r--r--   0        0        0     1716 2023-04-27 05:13:51.329779 fling_start-0.1.8/fling/templates/start/base.html
--rw-r--r--   0        0        0     8012 2023-04-27 05:17:42.026582 fling_start-0.1.8/fling/templates/start/index.html
--rw-r--r--   0        0        0      823 2023-04-20 00:30:35.165486 fling_start-0.1.8/fling/templates/start/x3d.html
--rw-r--r--   0        0        0      754 2023-04-27 17:28:37.944087 fling_start-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 fling_start-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      156 2023-04-26 00:22:00.443542 fling_start-0.1.9/README.md
+-rw-r--r--   0        0        0        6 2023-04-27 18:36:03.104192 fling_start-0.1.9/VERSION
+-rw-r--r--   0        0        0        0 2023-04-19 21:06:07.644598 fling_start-0.1.9/fling/__init__.py
+-rw-r--r--   0        0        0     1113 2023-04-27 05:22:45.984819 fling_start-0.1.9/fling/middleware.py
+-rw-r--r--   0        0        0     4127 2023-04-27 16:49:54.982507 fling_start-0.1.9/fling/start.py
+-rw-r--r--   0        0        0      889 2023-04-27 18:18:40.241320 fling_start-0.1.9/fling/static/start/styles.css
+-rw-r--r--   0        0        0      487 2023-04-27 16:49:12.318822 fling_start-0.1.9/fling/templates/admin/index.html
+-rw-r--r--   0        0        0     1716 2023-04-27 05:13:51.329779 fling_start-0.1.9/fling/templates/start/base.html
+-rw-r--r--   0        0        0     8173 2023-04-27 18:23:24.271880 fling_start-0.1.9/fling/templates/start/index.html
+-rw-r--r--   0        0        0      823 2023-04-20 00:30:35.165486 fling_start-0.1.9/fling/templates/start/x3d.html
+-rw-r--r--   0        0        0      754 2023-04-27 18:36:11.022184 fling_start-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 fling_start-0.1.9/PKG-INFO
```

### Comparing `fling_start-0.1.8/fling/middleware.py` & `fling_start-0.1.9/fling/middleware.py`

 * *Files identical despite different names*

### Comparing `fling_start-0.1.8/fling/start.py` & `fling_start-0.1.9/fling/start.py`

 * *Files identical despite different names*

### Comparing `fling_start-0.1.8/fling/templates/start/base.html` & `fling_start-0.1.9/fling/templates/start/base.html`

 * *Files identical despite different names*

### Comparing `fling_start-0.1.8/fling/templates/start/index.html` & `fling_start-0.1.9/fling/templates/start/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -125,17 +125,22 @@
 
   </div>
   
 {% endblock %}
   {% block scripts %}
 {{ super() }}
   <script async defer>
+  window.addEventListener("beforeunload", () => {
+     document.body.classList.remove("loaded");
+  });
+  window.addEventListener("pageshow", () => {
     fetch('/main', {redirect: 'error'}).then((response) => {
         response.text().then((html) => {
           document.getElementById('content').innerHTML =  html;
           document.body.classList.add("loaded");
         });
-  }).catch((response) => {
-      window.location.href = "/main";
+    }).catch((response) => {
+        window.location.href = "/main";
+    });
   });
   </script>
 {% endblock %}
```

### Comparing `fling_start-0.1.8/fling/templates/start/x3d.html` & `fling_start-0.1.9/fling/templates/start/x3d.html`

 * *Files identical despite different names*

### Comparing `fling_start-0.1.8/pyproject.toml` & `fling_start-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "fling-start"
-version = "0.1.8"
+version = "0.1.9"
 description = "Side Project Management from the command line"
 authors = [
     "Joshua McKenty <jmckenty@gmail.com>",
     "Anouk Ruhaak <anoukruhaak@gmail.com>",
 ]
 readme = "README.md"
 include = [{ path = "VERSION" }, { path = "README.md" },
```

### Comparing `fling_start-0.1.8/PKG-INFO` & `fling_start-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fling-start
-Version: 0.1.8
+Version: 0.1.9
 Summary: Side Project Management from the command line
 Author: Joshua McKenty
 Author-email: jmckenty@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

