# Comparing `tmp/mlo-0.0.2.tar.gz` & `tmp/mlo-0.0.3-py3.9.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mlo-0.0.2.tar", last modified: Thu Apr 25 07:28:18 2019, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

