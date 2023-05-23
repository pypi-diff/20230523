# Comparing `tmp/nonebot-plugin-cube-1.0.1.tar.gz` & `tmp/nonebot_plugin_cube-1.0.2-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-cube-1.0.1.tar", last modified: Tue May 23 13:12:48 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

