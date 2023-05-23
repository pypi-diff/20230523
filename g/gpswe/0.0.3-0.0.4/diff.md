# Comparing `tmp/gpswe-0.0.3.tar.gz` & `tmp/gpswe-0.0.4-py3.10.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpswe-0.0.3.tar", last modified: Mon May 22 01:13:25 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

