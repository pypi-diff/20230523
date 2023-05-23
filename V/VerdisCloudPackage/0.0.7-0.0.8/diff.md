# Comparing `tmp/VerdisCloudPackage-0.0.7-py3-none-any.whl.zip` & `tmp/VerdisCloudPackage-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3007 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat      991 b- defN 23-May-22 10:22 VerdisCloudPackage/AWS.py
+Zip file size: 3035 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat      991 b- defN 23-May-22 10:42 VerdisCloudPackage/AWS.py
 -rw-rw-rw-  2.0 fat      250 b- defN 23-May-22 10:35 VerdisCloudPackage/__init__.py
--rw-rw-rw-  2.0 fat     1059 b- defN 23-May-22 10:36 VerdisCloudPackage-0.0.7.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      332 b- defN 23-May-22 10:36 VerdisCloudPackage-0.0.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-22 10:36 VerdisCloudPackage-0.0.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       19 b- defN 23-May-22 10:36 VerdisCloudPackage-0.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      611 b- defN 23-May-22 10:36 VerdisCloudPackage-0.0.7.dist-info/RECORD
-7 files, 3354 bytes uncompressed, 1907 bytes compressed:  43.1%
+-rw-rw-rw-  2.0 fat     1059 b- defN 23-May-22 10:43 VerdisCloudPackage-0.0.8.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      332 b- defN 23-May-22 10:43 VerdisCloudPackage-0.0.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-22 10:43 VerdisCloudPackage-0.0.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       19 b- defN 23-May-22 10:43 VerdisCloudPackage-0.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      611 b- defN 23-May-22 10:43 VerdisCloudPackage-0.0.8.dist-info/RECORD
+7 files, 3354 bytes uncompressed, 1935 bytes compressed:  42.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: VerdisCloudPackage/AWS.py
 Comment: 
 
 Filename: VerdisCloudPackage/__init__.py
 Comment: 
 
-Filename: VerdisCloudPackage-0.0.7.dist-info/LICENSE.txt
+Filename: VerdisCloudPackage-0.0.8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: VerdisCloudPackage-0.0.7.dist-info/METADATA
+Filename: VerdisCloudPackage-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: VerdisCloudPackage-0.0.7.dist-info/WHEEL
+Filename: VerdisCloudPackage-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: VerdisCloudPackage-0.0.7.dist-info/top_level.txt
+Filename: VerdisCloudPackage-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: VerdisCloudPackage-0.0.7.dist-info/RECORD
+Filename: VerdisCloudPackage-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## VerdisCloudPackage/AWS.py

```diff
@@ -1,15 +1,15 @@
 import boto3
 import json
 import os
 def getParameter(name):
     session = boto3.Session(
     region_name='ap-south-1',
-    aws_access_key_id=os.environ.get('aws_access_key_id', "ask shivam sir"),
-    aws_secret_access_key=os.environ.get('aws_secret_access_key', "ask shivam sir"))
+    aws_access_key_id=os.environ.get('AWS_ACCESS_KEY_ID', "ASK SHIVAM SIR"),
+    aws_secret_access_key=os.environ.get('AWS_SECRET_ACCESS_KEY', "ASK SHIVAM SIR"))
     ssm = session.client('ssm')
     return ssm.get_parameter(Name=name, WithDecryption=True)
 
 
 def recurse(d, keys=()):
     if type(d) == dict:
         for k in d:
```

## Comparing `VerdisCloudPackage-0.0.7.dist-info/LICENSE.txt` & `VerdisCloudPackage-0.0.8.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `VerdisCloudPackage-0.0.7.dist-info/RECORD` & `VerdisCloudPackage-0.0.8.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-VerdisCloudPackage/AWS.py,sha256=cH3N_BU5pmn39ZEwHoe2ARqVgWS-gh-3Ya9pky503kg,991
+VerdisCloudPackage/AWS.py,sha256=XqNTeLGCnH_VA4I_GHluJYGahKyy9PEuBxnuOO6qVmA,991
 VerdisCloudPackage/__init__.py,sha256=cRXXJPQqMWojkYNHAx1cyBWyMuKc7RWGRfzVPUwRGww,250
-VerdisCloudPackage-0.0.7.dist-info/LICENSE.txt,sha256=39GIK9SJIjsbLXA35-psr85XQHebE2eWN3prAXAMKkE,1059
-VerdisCloudPackage-0.0.7.dist-info/METADATA,sha256=uro_AAft5L2bUHw0aBjGZorLriNBM2bRszpCmQ1xkic,332
-VerdisCloudPackage-0.0.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-VerdisCloudPackage-0.0.7.dist-info/top_level.txt,sha256=QIsizpOeCOKcDD3EaH9WkH41Hh0toCM_EVBNZTLb-q8,19
-VerdisCloudPackage-0.0.7.dist-info/RECORD,,
+VerdisCloudPackage-0.0.8.dist-info/LICENSE.txt,sha256=39GIK9SJIjsbLXA35-psr85XQHebE2eWN3prAXAMKkE,1059
+VerdisCloudPackage-0.0.8.dist-info/METADATA,sha256=rl1VT_1JhZ4tsKWa7MLZLxyBcMvaqlXBdeNkHkwF9AE,332
+VerdisCloudPackage-0.0.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+VerdisCloudPackage-0.0.8.dist-info/top_level.txt,sha256=QIsizpOeCOKcDD3EaH9WkH41Hh0toCM_EVBNZTLb-q8,19
+VerdisCloudPackage-0.0.8.dist-info/RECORD,,
```

