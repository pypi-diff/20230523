# Comparing `tmp/django_view_manager-1.0.2-py3-none-any.whl.zip` & `tmp/django_view_manager-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 11301 bytes, number of entries: 11
--rw-r--r--  2.0 unx        0 b- defN 23-May-19 22:12 django_view_manager/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-19 22:12 django_view_manager/utils/__init__.py
--rw-r--r--  2.0 unx      132 b- defN 23-May-19 22:12 django_view_manager/utils/apps.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-19 22:12 django_view_manager/utils/management/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-19 22:12 django_view_manager/utils/management/commands/__init__.py
--rw-r--r--  2.0 unx    20250 b- defN 23-May-19 22:12 django_view_manager/utils/management/commands/makeviewmigration.py
--rw-r--r--  2.0 unx     1504 b- defN 23-May-19 22:12 django_view_manager-1.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx    13963 b- defN 23-May-19 22:12 django_view_manager-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-19 22:12 django_view_manager-1.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-May-19 22:12 django_view_manager-1.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1049 b- defN 23-May-19 22:12 django_view_manager-1.0.2.dist-info/RECORD
-11 files, 37010 bytes uncompressed, 9461 bytes compressed:  74.4%
+Zip file size: 11297 bytes, number of entries: 11
+-rw-r--r--  2.0 unx        0 b- defN 23-May-23 16:39 django_view_manager/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-23 16:39 django_view_manager/utils/__init__.py
+-rw-r--r--  2.0 unx      132 b- defN 23-May-23 16:39 django_view_manager/utils/apps.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-23 16:39 django_view_manager/utils/management/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-23 16:39 django_view_manager/utils/management/commands/__init__.py
+-rw-r--r--  2.0 unx    20240 b- defN 23-May-23 16:39 django_view_manager/utils/management/commands/makeviewmigration.py
+-rw-r--r--  2.0 unx     1504 b- defN 23-May-23 16:39 django_view_manager-1.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx    13963 b- defN 23-May-23 16:39 django_view_manager-1.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-23 16:39 django_view_manager-1.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-May-23 16:39 django_view_manager-1.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1049 b- defN 23-May-23 16:39 django_view_manager-1.0.3.dist-info/RECORD
+11 files, 37000 bytes uncompressed, 9457 bytes compressed:  74.4%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: django_view_manager/utils/management/commands/__init__.py
 Comment: 
 
 Filename: django_view_manager/utils/management/commands/makeviewmigration.py
 Comment: 
 
-Filename: django_view_manager-1.0.2.dist-info/LICENSE
+Filename: django_view_manager-1.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: django_view_manager-1.0.2.dist-info/METADATA
+Filename: django_view_manager-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: django_view_manager-1.0.2.dist-info/WHEEL
+Filename: django_view_manager-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: django_view_manager-1.0.2.dist-info/top_level.txt
+Filename: django_view_manager-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: django_view_manager-1.0.2.dist-info/RECORD
+Filename: django_view_manager-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## django_view_manager/utils/management/commands/makeviewmigration.py

```diff
@@ -7,15 +7,15 @@
 from django.apps import apps
 from django.core.management import BaseCommand
 from django.core.management import call_command
 from django.db import migrations
 from django.db.transaction import atomic
 
 
-VERSION = "1.0.2"
+VERSION = "1.0.3"
 
 
 COPIED_SQL_VIEW_CONTENT = f"""/*
     This file was generated using django-view-manager {VERSION}.
     Modify the SQL for this view and then commit the changes.
     You can remove this comment before committing.
 
@@ -345,18 +345,18 @@
                 '''"SELECT 'replace_forwards';"''', "forwards_sql"
             )
             lines[class_line_no - 1 : class_line_no] = [
                 f'sql_path = "{os.path.relpath(sql_path)}"\n',
                 f'forward_sql_filename = "{forward_sql_filename}"\n',
                 f'reverse_sql_filename = "{reverse_sql_filename}"\n' if reverse_sql_filename else "",
                 "\n",
-                'with open(f"{os.path.join(sql_path, forward_sql_filename)}", mode="r") as f:\n',
+                'with open(os.path.join(sql_path, forward_sql_filename), mode="r") as f:\n',
                 "    forwards_sql = f.read()\n",
                 "\n",
-                'with open(f"{os.path.join(sql_path, reverse_sql_filename)}", mode="r") as f:\n'
+                'with open(os.path.join(sql_path, reverse_sql_filename), mode="r") as f:\n'
                 if reverse_sql_filename
                 else "",
                 "    reverse_sql = f.read()\n" if reverse_sql_filename else "",
                 "\n" if reverse_sql_filename else "",
             ]
             lines[imports_line_no - 1 : imports_line_no] = [
                 "import os\n",
```

## Comparing `django_view_manager-1.0.2.dist-info/LICENSE` & `django_view_manager-1.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `django_view_manager-1.0.2.dist-info/METADATA` & `django_view_manager-1.0.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-view-manager
-Version: 1.0.2
+Version: 1.0.3
 Summary: A management command for django that provides diffs of sql views.
 Author-email: Arrai Innovations <support@arrai.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Arrai Innovations
         
         Redistribution and use in source and binary forms, with or without
```

## Comparing `django_view_manager-1.0.2.dist-info/RECORD` & `django_view_manager-1.0.3.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 django_view_manager/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 django_view_manager/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 django_view_manager/utils/apps.py,sha256=fZoo89eHKqypCLKzeFxUNkGrHTBs4sWGm3ZcLDDGTi8,132
 django_view_manager/utils/management/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 django_view_manager/utils/management/commands/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-django_view_manager/utils/management/commands/makeviewmigration.py,sha256=48ZzxgcXiXrHWgUNmdXpSncGpOOVvW7maqhL5SwEK2E,20250
-django_view_manager-1.0.2.dist-info/LICENSE,sha256=C9Y-Cr2GS0AyKcVDN7Gwj4DjjYTUdCUrFDeASp8C8fA,1504
-django_view_manager-1.0.2.dist-info/METADATA,sha256=XFt6tQVLOwiEEvwHs5y9ztKjPBJCzfwmKASxS32mXjs,13963
-django_view_manager-1.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-django_view_manager-1.0.2.dist-info/top_level.txt,sha256=WaJvRmbbOJ7HI_7RuTxUSjULO_00vrBXScnfiFteTT8,20
-django_view_manager-1.0.2.dist-info/RECORD,,
+django_view_manager/utils/management/commands/makeviewmigration.py,sha256=6xvD_cFaUbV97K2KqIxls22SDvH28xIN3k5uh09iqPM,20240
+django_view_manager-1.0.3.dist-info/LICENSE,sha256=C9Y-Cr2GS0AyKcVDN7Gwj4DjjYTUdCUrFDeASp8C8fA,1504
+django_view_manager-1.0.3.dist-info/METADATA,sha256=8GvaUi9vDTwZ84cKrAB8Sg9jmbqMl0uG38YDdMATg5w,13963
+django_view_manager-1.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+django_view_manager-1.0.3.dist-info/top_level.txt,sha256=WaJvRmbbOJ7HI_7RuTxUSjULO_00vrBXScnfiFteTT8,20
+django_view_manager-1.0.3.dist-info/RECORD,,
```

