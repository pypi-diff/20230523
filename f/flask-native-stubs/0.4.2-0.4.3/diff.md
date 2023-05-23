# Comparing `tmp/flask-native-stubs-0.4.2.tar.gz` & `tmp/flask_native_stubs-0.4.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-native-stubs-0.4.2.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

