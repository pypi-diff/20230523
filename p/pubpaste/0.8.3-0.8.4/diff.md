# Comparing `tmp/pubpaste-0.8.3-py3-none-any.whl.zip` & `tmp/pubpaste-0.8.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 24293 bytes, number of entries: 6
--rw-r--r--  2.0 unx    58606 b- defN 23-Mar-09 17:37 pubpaste.py
--rw-r--r--  2.0 unx    16332 b- defN 23-Mar-09 17:38 pubpaste-0.8.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-09 17:38 pubpaste-0.8.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       43 b- defN 23-Mar-09 17:38 pubpaste-0.8.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 23-Mar-09 17:38 pubpaste-0.8.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      467 b- defN 23-Mar-09 17:38 pubpaste-0.8.3.dist-info/RECORD
-6 files, 75549 bytes uncompressed, 23447 bytes compressed:  69.0%
+Zip file size: 24298 bytes, number of entries: 6
+-rw-r--r--  2.0 unx    58613 b- defN 23-May-23 17:24 pubpaste.py
+-rw-r--r--  2.0 unx    16332 b- defN 23-May-23 17:30 pubpaste-0.8.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-23 17:30 pubpaste-0.8.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       43 b- defN 23-May-23 17:30 pubpaste-0.8.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-May-23 17:30 pubpaste-0.8.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      467 b- defN 23-May-23 17:30 pubpaste-0.8.4.dist-info/RECORD
+6 files, 75556 bytes uncompressed, 23452 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: pubpaste.py
 Comment: 
 
-Filename: pubpaste-0.8.3.dist-info/METADATA
+Filename: pubpaste-0.8.4.dist-info/METADATA
 Comment: 
 
-Filename: pubpaste-0.8.3.dist-info/WHEEL
+Filename: pubpaste-0.8.4.dist-info/WHEEL
 Comment: 
 
-Filename: pubpaste-0.8.3.dist-info/entry_points.txt
+Filename: pubpaste-0.8.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: pubpaste-0.8.3.dist-info/top_level.txt
+Filename: pubpaste-0.8.4.dist-info/top_level.txt
 Comment: 
 
-Filename: pubpaste-0.8.3.dist-info/RECORD
+Filename: pubpaste-0.8.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pubpaste.py

```diff
@@ -1533,15 +1533,15 @@
             dump_content = [stdin_tmp_path]
             if uri_with_token:
                 uri = uri_with_token + quote(path)
 
         # dump file contents we know is terminal-safe
         if path in dump_content:
             with open(path, "rb") as fp:
-                print("uploading content: %r" % fp.read())
+                print("uploading content: %r" % bytes(fp.read()))
         assert args.output.endswith("/")
 
         # record history
         history.append_once(args.token, uri_with_token or None)
 
         if uri:
             logging.info("uploading %s to %s", path, uri)
```

## Comparing `pubpaste-0.8.3.dist-info/METADATA` & `pubpaste-0.8.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pubpaste
-Version: 0.8.3
+Version: 0.8.4
 Home-page: https://gitlab.com/anarcat/pubpaste/
 Author: The Anarcat
 Author-email: anarcat@debian.org
 Project-URL: Bug Reports, https://gitlab.com/anarcat/pubpaste/issues
 Project-URL: Say Thanks!, http://saythanks.io/to/anarcat
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: X11 Applications
```

