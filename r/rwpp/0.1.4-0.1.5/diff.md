# Comparing `tmp/rwpp-0.1.4.tar.gz` & `tmp/rwpp-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rwpp-0.1.4.tar", max compression
+gzip compressed data, was "rwpp-0.1.5.tar", max compression
```

## Comparing `rwpp-0.1.4.tar` & `rwpp-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1036 2023-05-18 09:28:32.742220 rwpp-0.1.4/LICENSE
--rw-r--r--   0        0        0     4481 2023-05-21 17:03:01.838556 rwpp-0.1.4/README.md
--rw-r--r--   0        0        0      458 2023-05-21 17:05:02.738834 rwpp-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-18 09:28:32.746220 rwpp-0.1.4/rwpp/__init__.py
--rw-r--r--   0        0        0     3312 2023-05-21 17:03:48.530664 rwpp-0.1.4/rwpp/main.py
--rw-r--r--   0        0        0     5101 1970-01-01 00:00:00.000000 rwpp-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1036 2023-05-18 09:28:32.742220 rwpp-0.1.5/LICENSE
+-rw-r--r--   0        0        0     4481 2023-05-21 17:03:01.838556 rwpp-0.1.5/README.md
+-rw-r--r--   0        0        0      458 2023-05-23 10:41:39.482510 rwpp-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-18 09:28:32.746220 rwpp-0.1.5/rwpp/__init__.py
+-rw-r--r--   0        0        0     3391 2023-05-23 10:40:06.974376 rwpp-0.1.5/rwpp/main.py
+-rw-r--r--   0        0        0     5101 1970-01-01 00:00:00.000000 rwpp-0.1.5/PKG-INFO
```

### Comparing `rwpp-0.1.4/LICENSE` & `rwpp-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rwpp-0.1.4/README.md` & `rwpp-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `rwpp-0.1.4/rwpp/main.py` & `rwpp-0.1.5/rwpp/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,36 +66,42 @@
 # @app.callback()
 def main(
     subreddit: str = typer.Argument(
         ..., help="The given subreddit(s) to pull images from"
     ),
     limit: int = typer.Option(
         10,
+        "--limit",
+        "-l",
         help="The amount of posts to pull from subreddit(s)",
         prompt="How many images would you like to download? ",
     ),
-    download_path: str = typer.Option(
+    path: str = typer.Option(
         "~/.wallpapers",
+        "--path",
+        "-p",
         help="The path where you would like to save images",
         prompt="Where would you like to save the images? ",
     ),
     sort_by: str = typer.Option(
         "hot",
+        "--sort",
+        "-s",
         help="The sort order to pull images by",
         prompt="Sort order for images?: [hot, new, top, rising] ",
     ),
 ):
     # Prompt for time option only if sort_by is top
     if sort_by == "top":
         time = typer.prompt(
             "Time period would you like to sort top by? [hour, day, week, month, year] "
         )
     else:
         time = None
-    download(subreddit, limit, download_path, time, sort_by)
+    download(subreddit, limit, path, time, sort_by)
 
 
 # Main function to be called from terminal
 @app.callback()
 def cli():
     typer.run(main)
```

### Comparing `rwpp-0.1.4/PKG-INFO` & `rwpp-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwpp
-Version: 0.1.4
+Version: 0.1.5
 Summary: Reddit Wallpaper Puller, a simple CLI to pull wallpapers from Reddit.
 Author: Ducky
 Author-email: duckbox007@pm.me
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

