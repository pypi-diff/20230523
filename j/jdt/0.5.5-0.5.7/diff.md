# Comparing `tmp/jdt-0.5.5.tar.gz` & `tmp/jdt-0.5.7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jdt-0.5.5.tar", last modified: Thu Jan 28 18:16:33 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

