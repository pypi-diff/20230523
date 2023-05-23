# Comparing `tmp/xyz_util-0.7.8-py3-none-any.whl.zip` & `tmp/xyz_util-0.7.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,27 +1,27 @@
-Zip file size: 51087 bytes, number of entries: 25
+Zip file size: 51129 bytes, number of entries: 25
 -rw-r--r--  2.0 unx       88 b- defN 20-Jan-17 14:46 xyz_util/__init__.py
 -rw-r--r--  2.0 unx      732 b- defN 23-Apr-25 02:25 xyz_util/cmdutils.py
 -rw-r--r--  2.0 unx     9639 b- defN 23-Jan-12 06:48 xyz_util/crawlutils.py
 -rw-r--r--  2.0 unx      903 b- defN 18-Oct-15 06:43 xyz_util/cryptutils.py
 -rw-r--r--  2.0 unx    16035 b- defN 23-Apr-25 04:36 xyz_util/datautils.py
 -rw-r--r--  2.0 unx     6400 b- defN 21-Aug-09 10:21 xyz_util/dateutils.py
 -rw-r--r--  2.0 unx    13185 b- defN 21-Jul-04 23:24 xyz_util/dbutils.py
 -rw-r--r--  2.0 unx    17205 b- defN 21-Jul-26 09:02 xyz_util/excelutils.py
 -rw-r--r--  2.0 unx     2667 b- defN 21-Jul-04 23:24 xyz_util/formutils.py
 -rw-r--r--  2.0 unx     4613 b- defN 21-Dec-19 01:47 xyz_util/importutils.py
 -rw-r--r--  2.0 unx     2857 b- defN 23-Apr-27 07:24 xyz_util/mediautils.py
--rw-r--r--  2.0 unx    13998 b- defN 22-Aug-03 00:02 xyz_util/modelutils.py
+-rw-r--r--  2.0 unx    14127 b- defN 23-May-04 09:25 xyz_util/modelutils.py
 -rw-r--r--  2.0 unx    16893 b- defN 23-Mar-23 07:06 xyz_util/mongoutils.py
 -rw-r--r--  2.0 unx    14661 b- defN 21-Jul-13 11:57 xyz_util/pandasutils.py
 -rw-r--r--  2.0 unx      507 b- defN 21-Jun-01 00:29 xyz_util/pdfutils.py
--rw-r--r--  2.0 unx    15349 b- defN 22-Jul-04 08:21 xyz_util/statutils.py
+-rw-r--r--  2.0 unx    15457 b- defN 23-May-04 09:27 xyz_util/statutils.py
 -rw-r--r--  2.0 unx     1997 b- defN 23-Mar-06 16:57 xyz_util/textutils.py
 -rw-r--r--  2.0 unx     1675 b- defN 20-Aug-01 15:19 xyz_util/transferutils.py
 -rw-r--r--  2.0 unx     5316 b- defN 21-Jun-05 23:16 xyz_util/validators.py
 -rw-r--r--  2.0 unx     7815 b- defN 21-May-26 06:42 xyz_util/views.py
 -rw-r--r--  2.0 unx     3956 b- defN 21-Jul-04 23:24 xyz_util/widgetutils.py
--rw-r--r--  2.0 unx     1056 b- defN 23-Apr-27 08:41 xyz_util-0.7.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-27 08:41 xyz_util-0.7.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Apr-27 08:41 xyz_util-0.7.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1949 b- defN 23-Apr-27 08:41 xyz_util-0.7.8.dist-info/RECORD
-25 files, 159597 bytes uncompressed, 48003 bytes compressed:  69.9%
+-rw-r--r--  2.0 unx     1056 b- defN 23-May-04 10:47 xyz_util-0.7.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-04 10:47 xyz_util-0.7.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-May-04 10:47 xyz_util-0.7.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1949 b- defN 23-May-04 10:47 xyz_util-0.7.9.dist-info/RECORD
+25 files, 159834 bytes uncompressed, 48045 bytes compressed:  69.9%
```

## zipnote {}

```diff
@@ -57,20 +57,20 @@
 
 Filename: xyz_util/views.py
 Comment: 
 
 Filename: xyz_util/widgetutils.py
 Comment: 
 
-Filename: xyz_util-0.7.8.dist-info/METADATA
+Filename: xyz_util-0.7.9.dist-info/METADATA
 Comment: 
 
-Filename: xyz_util-0.7.8.dist-info/WHEEL
+Filename: xyz_util-0.7.9.dist-info/WHEEL
 Comment: 
 
-Filename: xyz_util-0.7.8.dist-info/top_level.txt
+Filename: xyz_util-0.7.9.dist-info/top_level.txt
 Comment: 
 
-Filename: xyz_util-0.7.8.dist-info/RECORD
+Filename: xyz_util-0.7.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xyz_util/modelutils.py

```diff
@@ -195,14 +195,16 @@
 
 def find_field(m, find_func):
     meta = m._meta if hasattr(m, '_meta') else m
     for f in meta.get_fields():
         if find_func(f):
             return f
 
+def get_datetime_field(meta):
+    return find_field(meta, lambda f: isinstance(f, (djfields.DateTimeField, djfields.DateField)))
 
 def get_generic_foreign_key(meta):
     return find_field(meta, lambda f: isinstance(f, GenericForeignKey))
 
 
 def get_related_fields(obj, field_name, start_position=0):
     meta = obj.model._meta if isinstance(obj, QuerySet) else obj._meta
```

## xyz_util/statutils.py

```diff
@@ -218,14 +218,16 @@
         rs = nrs
     return rs
 
 
 class DateStat(object):
     def __init__(self, query_set, time_field):
         self.query_set = query_set
+        if time_field is None:
+            time_field = modelutils.get_datetime_field(query_set.model).name
         self.time_field = time_field
         self.model = self.query_set.model
 
     def get_period_query_set(self, period):
         qset = self.query_set
         if period and period != 'all':
             begin_time, end_time = dateutils.get_period_by_name(period)
```

## Comparing `xyz_util-0.7.8.dist-info/METADATA` & `xyz_util-0.7.9.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xyz-util
-Version: 0.7.8
+Version: 0.7.9
 Summary: common utils
 Home-page: https://github.com/szuprefix/py-xyz-util
 Author: szuprefix
 Author-email: szuprefix@126.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

## Comparing `xyz_util-0.7.8.dist-info/RECORD` & `xyz_util-0.7.9.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 xyz_util/datautils.py,sha256=XeXSclf9hedQ8uJzF8C9X_iSy-kj-o7rj4DxgTNSAvY,16035
 xyz_util/dateutils.py,sha256=doPQh86iJNIWhA1EsZy1ar3Vgw3RSFAxUkTgPX_RU3s,6400
 xyz_util/dbutils.py,sha256=Wj4Bf7tJg2UzwTP5-p4rCACXTaIvH5J6milAOpAGHUk,13185
 xyz_util/excelutils.py,sha256=FuK1RnGPG1XFRNDyYbKPK7urc9tvgNXFtR9-NLlamkE,17205
 xyz_util/formutils.py,sha256=bM5pEShw-gmUm5RMVyQ9xPO7RAHZ4TNTwaFXlzebvmU,2667
 xyz_util/importutils.py,sha256=9EQaTCRYVzWAo9SHpffFV1XqFND9MU0e63KMJPmx1bI,4613
 xyz_util/mediautils.py,sha256=X9_YVpfNLU852hxsn11d5VQjjM6PadMAZcwHtRcVsxI,2857
-xyz_util/modelutils.py,sha256=wuwMbTCL3RIjPOlbpuxC55dqfET5SsitV_gu0tRHwHk,13998
+xyz_util/modelutils.py,sha256=bz5_KnuM7XxfUO5MOslwZf6tdAFFpCOaxPlF-bJtQkw,14127
 xyz_util/mongoutils.py,sha256=vilihwLZ7g6n89a02nOhXvcIxu8UTTzdf4t3qywZWDM,16893
 xyz_util/pandasutils.py,sha256=gOuey7Vf6E62WFYVM4T2EwER9WQ_4Tmk4Ays0h6bCTQ,14661
 xyz_util/pdfutils.py,sha256=EFWIB4j74NHaCmGuVTZGSRbvoB-spl0Vj1_BKFjZl2I,507
-xyz_util/statutils.py,sha256=pl1Dn4rIPYfaZnSEkmPbfY5Z_tItKpeqor01tfPkE6Y,15349
+xyz_util/statutils.py,sha256=qkJ1icvRkoq2lQPzS5IZ4sShiKTxLUFxEN-EZrMDHqA,15457
 xyz_util/textutils.py,sha256=AYJm8SQrq-CxyLA4G9bzJyiFFcNW57NckRU0X2CItLI,1997
 xyz_util/transferutils.py,sha256=76VLi9Fjt3whO42oDvBJ0R2_CFzCkxeVxcfIB7VWtrc,1675
 xyz_util/validators.py,sha256=8qulZP-yPyal_GJWzmQzkm8yCHiMuGJ_hVPmK8bW-Ww,5316
 xyz_util/views.py,sha256=X2_JtrTLmg_nzaAHRKuh4umUtgmFsnVvcFFNRtlUfOo,7815
 xyz_util/widgetutils.py,sha256=uTZenfxd0zXpRx40lgS86kU0BKccYyg_Sh3XdmUVg7Q,3956
-xyz_util-0.7.8.dist-info/METADATA,sha256=29kuOEbBfUewtV-_jmazyTuARnW9k3ERnupB8i3XKNs,1056
-xyz_util-0.7.8.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-xyz_util-0.7.8.dist-info/top_level.txt,sha256=0uGpvx0NID3M2oMuWv7LYVDnUpUIIOwIWp8Br1tItgM,9
-xyz_util-0.7.8.dist-info/RECORD,,
+xyz_util-0.7.9.dist-info/METADATA,sha256=-O-9ZHbeajcoFmKDentYFl67Znw6WAbgK6jEjf4PP9A,1056
+xyz_util-0.7.9.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+xyz_util-0.7.9.dist-info/top_level.txt,sha256=0uGpvx0NID3M2oMuWv7LYVDnUpUIIOwIWp8Br1tItgM,9
+xyz_util-0.7.9.dist-info/RECORD,,
```

