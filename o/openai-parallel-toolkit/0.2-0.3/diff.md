# Comparing `tmp/openai_parallel_toolkit-0.2.tar.gz` & `tmp/openai_parallel_toolkit-0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_parallel_toolkit-0.2.tar", last modified: Thu May 18 11:48:41 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

