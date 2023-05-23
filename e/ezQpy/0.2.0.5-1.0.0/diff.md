# Comparing `tmp/ezQpy-0.2.0.5.tar.gz` & `tmp/ezQpy-1.0.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezQpy-0.2.0.5.tar", last modified: Thu Apr 27 06:53:28 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

