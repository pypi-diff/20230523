# Comparing `tmp/django_bootstrap_colors-5.2.0-py3-none-any.whl.zip` & `tmp/django_bootstrap_colors-5.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3729 bytes, number of entries: 8
+Zip file size: 3745 bytes, number of entries: 8
 -rw-r--r--  2.0 unx        0 b- defN 23-May-09 09:26 bootstrap_colors/__init__.py
--rw-r--r--  2.0 unx      390 b- defN 23-May-09 09:41 bootstrap_colors/views.py
+-rw-r--r--  2.0 unx      430 b- defN 23-May-23 07:28 bootstrap_colors/views.py
 -rw-r--r--  2.0 unx     1722 b- defN 23-May-09 09:13 bootstrap_colors/templates/bootstrap_colors.css
--rw-r--r--  2.0 unx     1065 b- defN 23-May-16 11:14 django_bootstrap_colors-5.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1208 b- defN 23-May-16 11:14 django_bootstrap_colors-5.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-16 11:14 django_bootstrap_colors-5.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-May-16 11:14 django_bootstrap_colors-5.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      733 b- defN 23-May-16 11:14 django_bootstrap_colors-5.2.0.dist-info/RECORD
-8 files, 5227 bytes uncompressed, 2421 bytes compressed:  53.7%
+-rw-r--r--  2.0 unx     1065 b- defN 23-May-23 07:31 django_bootstrap_colors-5.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1206 b- defN 23-May-23 07:31 django_bootstrap_colors-5.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-23 07:31 django_bootstrap_colors-5.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-May-23 07:31 django_bootstrap_colors-5.2.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      733 b- defN 23-May-23 07:31 django_bootstrap_colors-5.2.1.dist-info/RECORD
+8 files, 5265 bytes uncompressed, 2437 bytes compressed:  53.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: bootstrap_colors/views.py
 Comment: 
 
 Filename: bootstrap_colors/templates/bootstrap_colors.css
 Comment: 
 
-Filename: django_bootstrap_colors-5.2.0.dist-info/LICENSE
+Filename: django_bootstrap_colors-5.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: django_bootstrap_colors-5.2.0.dist-info/METADATA
+Filename: django_bootstrap_colors-5.2.1.dist-info/METADATA
 Comment: 
 
-Filename: django_bootstrap_colors-5.2.0.dist-info/WHEEL
+Filename: django_bootstrap_colors-5.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: django_bootstrap_colors-5.2.0.dist-info/top_level.txt
+Filename: django_bootstrap_colors-5.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: django_bootstrap_colors-5.2.0.dist-info/RECORD
+Filename: django_bootstrap_colors-5.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bootstrap_colors/views.py

```diff
@@ -4,9 +4,11 @@
 
 class BootstrapColorsView(TemplateView):
     template_name = 'bootstrap_colors.css'
     content_type = 'text/css'
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
-        context['BOOTSTRAP_THEME_COLORS'] = settings.BOOTSTRAP_THEME_COLORS
+        context['BOOTSTRAP_THEME_COLORS'] = getattr(
+            settings, 'BOOTSTRAP_THEME_COLORS', None
+        )
         return context
```

## Comparing `django_bootstrap_colors-5.2.0.dist-info/LICENSE` & `django_bootstrap_colors-5.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `django_bootstrap_colors-5.2.0.dist-info/METADATA` & `django_bootstrap_colors-5.2.1.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: django-bootstrap-colors
-Version: 5.2.0
+Version: 5.2.1
 Summary: UNKNOWN
 Home-page: https://git.mpib-berlin.mpg.de/castellum/django-bootstrap-colors
 Author: Max-Planck-Gesellschaft
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This django app allows to override the primary color and its variants in
 bootstrap.
 
 # Usage
 
 -   Add `bootstrap_colors` to `INSTALLED_APPS`
--   Add `path('colors.css', BootstrapColorsView().as_view(), name='colors')` to
+-   Add `path('colors.css', BootstrapColorsView.as_view(), name='colors')` to
     `urls.py`
 -   Add `<link rel="stylesheet" type="text/css" href="{% url 'colors' %}">` to
     your template
 -   Set `BOOTSTRAP_THEME_COLORS` (Default: `['#0d6efd', '#0b5ed7', '#0a58ca']`)
 
 # Alternatives
```

## Comparing `django_bootstrap_colors-5.2.0.dist-info/RECORD` & `django_bootstrap_colors-5.2.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 bootstrap_colors/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-bootstrap_colors/views.py,sha256=FYN2jPlF9d6X3YxXXRp_i9vWzd8xpqodTxRoLEGamGc,390
+bootstrap_colors/views.py,sha256=AxcQBX5qz3pLpSZrFxaJTsOeHegVqLfjH4-BpYb4uCU,430
 bootstrap_colors/templates/bootstrap_colors.css,sha256=HBRqKst05pET74i66wpBvek3KmdoZosERxA99BIqwqY,1722
-django_bootstrap_colors-5.2.0.dist-info/LICENSE,sha256=2PyjqrEsgnfGJ45bh-MInPp6o71wQ6QxjCODf4ufXAM,1065
-django_bootstrap_colors-5.2.0.dist-info/METADATA,sha256=e5dBRcbe2oE1SFQDYqLBv0UUC3gFpcwceRjC-fwKdWY,1208
-django_bootstrap_colors-5.2.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-django_bootstrap_colors-5.2.0.dist-info/top_level.txt,sha256=EVK2cCc-6-m3DIbl6jIVv0O2p-ZH7DZUwK2ZkFK0tHA,17
-django_bootstrap_colors-5.2.0.dist-info/RECORD,,
+django_bootstrap_colors-5.2.1.dist-info/LICENSE,sha256=2PyjqrEsgnfGJ45bh-MInPp6o71wQ6QxjCODf4ufXAM,1065
+django_bootstrap_colors-5.2.1.dist-info/METADATA,sha256=SwF1Q8Di9lndzAqEa5HvO6jBlBGl4AgsDTtjoMaPCCQ,1206
+django_bootstrap_colors-5.2.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+django_bootstrap_colors-5.2.1.dist-info/top_level.txt,sha256=EVK2cCc-6-m3DIbl6jIVv0O2p-ZH7DZUwK2ZkFK0tHA,17
+django_bootstrap_colors-5.2.1.dist-info/RECORD,,
```

