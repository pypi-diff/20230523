# Comparing `tmp/firebase_push-0.2.1.tar.gz` & `tmp/firebase_push-0.2.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firebase_push-0.2.1.tar", last modified: Thu Mar 23 16:44:41 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

