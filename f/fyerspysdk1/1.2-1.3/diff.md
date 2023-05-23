# Comparing `tmp/fyerspysdk1-1.2-py3-none-any.whl.zip` & `tmp/fyerspysdk1-1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 12097 bytes, number of entries: 9
+Zip file size: 12105 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx       20 b- defN 23-May-22 12:28 fyerstest/__init__.py
--rw-rw-r--  2.0 unx    16452 b- defN 23-May-22 12:49 fyerstest/fyersApi.py
+-rw-rw-r--  2.0 unx    16470 b- defN 23-May-23 04:02 fyerstest/fyersApi.py
 -rw-rw-r--  2.0 unx    15732 b- defN 23-May-22 11:31 fyerstest/hsmFyers.py
 -rw-rw-r--  2.0 unx     7894 b- defN 23-May-22 11:30 fyerstest/ws.py
--rwxrwxr-x  2.0 unx     1063 b- defN 23-May-22 13:00 fyerspysdk1-1.2.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx      622 b- defN 23-May-22 13:00 fyerspysdk1-1.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-22 13:00 fyerspysdk1-1.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-May-22 13:00 fyerspysdk1-1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      705 b- defN 23-May-22 13:00 fyerspysdk1-1.2.dist-info/RECORD
-9 files, 42590 bytes uncompressed, 10889 bytes compressed:  74.4%
+-rwxrwxr-x  2.0 unx     1063 b- defN 23-May-23 04:02 fyerspysdk1-1.3.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx      622 b- defN 23-May-23 04:02 fyerspysdk1-1.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-23 04:02 fyerspysdk1-1.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-May-23 04:02 fyerspysdk1-1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      705 b- defN 23-May-23 04:02 fyerspysdk1-1.3.dist-info/RECORD
+9 files, 42608 bytes uncompressed, 10897 bytes compressed:  74.4%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: fyerstest/hsmFyers.py
 Comment: 
 
 Filename: fyerstest/ws.py
 Comment: 
 
-Filename: fyerspysdk1-1.2.dist-info/LICENSE.txt
+Filename: fyerspysdk1-1.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: fyerspysdk1-1.2.dist-info/METADATA
+Filename: fyerspysdk1-1.3.dist-info/METADATA
 Comment: 
 
-Filename: fyerspysdk1-1.2.dist-info/WHEEL
+Filename: fyerspysdk1-1.3.dist-info/WHEEL
 Comment: 
 
-Filename: fyerspysdk1-1.2.dist-info/top_level.txt
+Filename: fyerspysdk1-1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: fyerspysdk1-1.2.dist-info/RECORD
+Filename: fyerspysdk1-1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fyerstest/fyersApi.py

```diff
@@ -98,15 +98,15 @@
         if data_flag:
             if api == '/history':
                 URL = Config.historyDataUrl + api
             else:
                 URL =  Config.data_Api +api
         else:
             URL = Config.Api + api
-        async with aiohttp.ClientSession(headers={'Authorization': header, 'Content-Type': self.content}) as session:
+        async with aiohttp.ClientSession(headers={'Authorization': header, 'Content-Type': self.content , 'version':'2.1'}) as session:
             async with session.get(URL, params=params) as response:
                 response_data = await response.json()
                 return response_data
 
 
     async def deleteAsyncCall(self, api, header, data):
         async with aiohttp.ClientSession(headers={'Authorization': header, 'Content-Type': self.content}) as session:
```

## Comparing `fyerspysdk1-1.2.dist-info/LICENSE.txt` & `fyerspysdk1-1.3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `fyerspysdk1-1.2.dist-info/METADATA` & `fyerspysdk1-1.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyerspysdk1
-Version: 1.2
+Version: 1.3
 Summary: XX trc APIs.
 Home-page: https://github.com
 Author: my-Tech
 Author-email: support@f.in
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

