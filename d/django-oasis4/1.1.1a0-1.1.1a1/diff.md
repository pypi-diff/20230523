# Comparing `tmp/django-oasis4-1.1.1a0.tar.gz` & `tmp/django_oasis4-1.1.1a1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-oasis4-1.1.1a0.tar", last modified: Fri May 19 22:12:01 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

