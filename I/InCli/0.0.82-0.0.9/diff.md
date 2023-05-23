# Comparing `tmp/InCli-0.0.82.tar.gz` & `tmp/InCli-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "InCli-0.0.82.tar", last modified: Tue May 23 20:29:39 2023, max compression
+gzip compressed data, was "InCli-0.0.9.tar", last modified: Wed Dec  7 11:17:32 2022, max compression
```

## Comparing `InCli-0.0.82.tar` & `InCli-0.0.9.tar`

### file list

```diff
@@ -1,68 +1,35 @@
-drwxr-xr-x   0 uormaechea   (502) staff       (20)        0 2023-05-23 20:29:39.033076 InCli-0.0.82/
-drwxr-xr-x   0 uormaechea   (502) staff       (20)        0 2023-05-23 20:29:38.929041 InCli-0.0.82/InCli/
--rw-r--r--   0 uormaechea   (502) staff       (20)    33345 2023-05-18 19:37:38.000000 InCli-0.0.82/InCli/InCli.py
-drwxr-xr-x   0 uormaechea   (502) staff       (20)        0 2023-05-23 20:29:38.990646 InCli-0.0.82/InCli/SFAPI/
--rw-r--r--   0 uormaechea   (502) staff       (20)    27326 2023-05-19 07:10:31.000000 InCli-0.0.82/InCli/SFAPI/CPQ.py
--rw-r--r--   0 uormaechea   (502) staff       (20)     9597 2023-05-19 07:11:14.000000 InCli-0.0.82/InCli/SFAPI/CPQUtil.py
--rw-r--r--   0 uormaechea   (502) staff       (20)     5733 2023-02-27 20:30:06.000000 InCli-0.0.82/InCli/SFAPI/DR_IP.py
--rw-r--r--   0 uormaechea   (502) staff       (20)      917 2022-12-08 18:44:30.000000 InCli-0.0.82/InCli/SFAPI/DicPath.py
--rw-r--r--   0 uormaechea   (502) staff       (20)    12022 2023-03-21 09:14:53.000000 InCli-0.0.82/InCli/SFAPI/Sobjects.py
--rw-r--r--   0 uormaechea   (502) staff       (20)     7809 2023-04-11 19:38:12.000000 InCli-0.0.82/InCli/SFAPI/VlocityErrorLog.py
--rw-r--r--   0 uormaechea   (502) staff       (20)     7709 2023-04-19 12:07:47.000000 InCli-0.0.82/InCli/SFAPI/VlocityTrackingEntry.py
--rw-r--r--   0 uormaechea   (502) staff       (20)        0 2022-12-05 21:22:35.000000 InCli-0.0.82/InCli/SFAPI/__init__.py
--rw-r--r--   0 uormaechea   (502) staff       (20)     3505 2023-01-20 10:08:30.000000 InCli-0.0.82/InCli/SFAPI/account.py
--rw-r--r--   0 uormaechea   (502) staff       (20)    24873 2023-05-20 14:55:51.000000 InCli-0.0.82/InCli/SFAPI/debugLogs.py
--rw-r--r--   0 uormaechea   (502) staff       (20)    21579 2023-05-20 15:05:28.000000 InCli-0.0.82/InCli/SFAPI/debugLogsPrint.py
--rw-r--r--   0 uormaechea   (502) staff       (20)    13261 2023-03-29 12:05:45.000000 InCli-0.0.82/InCli/SFAPI/digitalCommerce.py
--rw-r--r--   0 uormaechea   (502) staff       (20)    12053 2023-03-17 09:22:54.000000 InCli-0.0.82/InCli/SFAPI/digitalCommerceUtil.py
--rw-r--r--   0 uormaechea   (502) staff       (20)    25495 2023-05-17 11:12:17.000000 InCli-0.0.82/InCli/SFAPI/elementParser.py
--rw-r--r--   0 uormaechea   (502) staff       (20)     2320 2023-04-12 14:44:43.000000 InCli-0.0.82/InCli/SFAPI/file.py
--rw-r--r--   0 uormaechea   (502) staff       (20)     2868 2023-04-27 15:52:46.000000 InCli-0.0.82/InCli/SFAPI/file_csv.py
--rw-r--r--   0 uormaechea   (502) staff       (20)    17609 2023-04-19 11:59:54.000000 InCli-0.0.82/InCli/SFAPI/ip_attachments.py
--rw-r--r--   0 uormaechea   (502) staff       (20)     2244 2022-12-05 21:42:40.000000 InCli-0.0.82/InCli/SFAPI/jsonFile.py
--rw-r--r--   0 uormaechea   (502) staff       (20)    12838 2023-05-19 07:11:37.000000 InCli-0.0.82/InCli/SFAPI/objectUtil.py
--rw-r--r--   0 uormaechea   (502) staff       (20)      648 2023-01-24 14:15:53.000000 InCli-0.0.82/InCli/SFAPI/priceBook.py
--rw-r--r--   0 uormaechea   (502) staff       (20)        0 2023-02-08 13:31:02.000000 InCli-0.0.82/InCli/SFAPI/product.py
--rw-r--r--   0 uormaechea   (502) staff       (20)     6828 2023-03-17 10:47:49.000000 InCli-0.0.82/InCli/SFAPI/query.py
--rw-r--r--   0 uormaechea   (502) staff       (20)    25056 2023-05-04 12:02:13.000000 InCli-0.0.82/InCli/SFAPI/restClient.py
--rw-r--r--   0 uormaechea   (502) staff       (20)     4314 2023-05-09 10:19:11.000000 InCli-0.0.82/InCli/SFAPI/thread.py
--rw-r--r--   0 uormaechea   (502) staff       (20)     2765 2023-05-19 07:12:06.000000 InCli-0.0.82/InCli/SFAPI/timeStats.py
--rw-r--r--   0 uormaechea   (502) staff       (20)     3697 2023-05-17 07:42:37.000000 InCli-0.0.82/InCli/SFAPI/tooling.py
--rw-r--r--   0 uormaechea   (502) staff       (20)     5940 2023-05-17 13:43:02.000000 InCli-0.0.82/InCli/SFAPI/traceFlag.py
--rw-r--r--   0 uormaechea   (502) staff       (20)    20099 2023-05-19 07:13:07.000000 InCli-0.0.82/InCli/SFAPI/utils.py
--rw-r--r--   0 uormaechea   (502) staff       (20)        0 2022-12-01 08:57:08.000000 InCli-0.0.82/InCli/__init__.py
-drwxr-xr-x   0 uormaechea   (502) staff       (20)        0 2023-05-23 20:29:38.935317 InCli-0.0.82/InCli.egg-info/
--rw-r--r--   0 uormaechea   (502) staff       (20)      210 2023-05-23 20:29:38.000000 InCli-0.0.82/InCli.egg-info/PKG-INFO
--rw-r--r--   0 uormaechea   (502) staff       (20)     1447 2023-05-23 20:29:38.000000 InCli-0.0.82/InCli.egg-info/SOURCES.txt
--rw-r--r--   0 uormaechea   (502) staff       (20)        1 2023-05-23 20:29:38.000000 InCli-0.0.82/InCli.egg-info/dependency_links.txt
--rw-r--r--   0 uormaechea   (502) staff       (20)       43 2023-05-23 20:29:38.000000 InCli-0.0.82/InCli.egg-info/entry_points.txt
--rw-r--r--   0 uormaechea   (502) staff       (20)       81 2023-05-23 20:29:38.000000 InCli-0.0.82/InCli.egg-info/requires.txt
--rw-r--r--   0 uormaechea   (502) staff       (20)        6 2023-05-23 20:29:38.000000 InCli-0.0.82/InCli.egg-info/top_level.txt
--rw-r--r--   0 uormaechea   (502) staff       (20)     1068 2022-12-01 10:54:37.000000 InCli-0.0.82/LICENSE.txt
--rw-r--r--   0 uormaechea   (502) staff       (20)      210 2023-05-23 20:29:39.032436 InCli-0.0.82/PKG-INFO
--rw-r--r--   0 uormaechea   (502) staff       (20)      117 2022-12-01 10:53:51.000000 InCli-0.0.82/README.md
--rw-r--r--   0 uormaechea   (502) staff       (20)      458 2023-05-23 20:29:22.000000 InCli-0.0.82/pyproject.toml
--rw-r--r--   0 uormaechea   (502) staff       (20)       38 2023-05-23 20:29:39.033256 InCli-0.0.82/setup.cfg
-drwxr-xr-x   0 uormaechea   (502) staff       (20)        0 2023-05-23 20:29:39.030911 InCli-0.0.82/test/
--rw-r--r--   0 uormaechea   (502) staff       (20)        0 2022-12-01 09:02:19.000000 InCli-0.0.82/test/__init__.py
--rw-r--r--   0 uormaechea   (502) staff       (20)    51603 2023-05-04 11:35:57.000000 InCli-0.0.82/test/test_CPQ.py
--rw-r--r--   0 uormaechea   (502) staff       (20)     8955 2023-04-03 08:24:27.000000 InCli-0.0.82/test/test_DC.py
--rw-r--r--   0 uormaechea   (502) staff       (20)      862 2023-04-28 22:09:55.000000 InCli-0.0.82/test/test_DicPath.py
--rw-r--r--   0 uormaechea   (502) staff       (20)    18651 2023-04-14 09:56:56.000000 InCli-0.0.82/test/test_GetCartItems.py
--rw-r--r--   0 uormaechea   (502) staff       (20)    27032 2023-05-18 13:21:28.000000 InCli-0.0.82/test/test_InCli.py
--rw-r--r--   0 uormaechea   (502) staff       (20)     1500 2023-01-20 10:08:30.000000 InCli-0.0.82/test/test_account.py
--rw-r--r--   0 uormaechea   (502) staff       (20)     2626 2023-02-13 19:27:20.000000 InCli-0.0.82/test/test_account_helper copy.py
--rw-r--r--   0 uormaechea   (502) staff       (20)     4100 2023-05-09 11:25:56.000000 InCli-0.0.82/test/test_attachment.py
--rw-r--r--   0 uormaechea   (502) staff       (20)    18146 2023-03-01 22:57:32.000000 InCli-0.0.82/test/test_dr_ip.py
--rw-r--r--   0 uormaechea   (502) staff       (20)      683 2022-12-05 21:56:14.000000 InCli-0.0.82/test/test_file.py
--rw-r--r--   0 uormaechea   (502) staff       (20)    14649 2023-02-17 16:43:33.000000 InCli-0.0.82/test/test_objects.py
--rw-r--r--   0 uormaechea   (502) staff       (20)    22296 2023-04-17 16:51:23.000000 InCli-0.0.82/test/test_order_stats.py
--rw-r--r--   0 uormaechea   (502) staff       (20)     1741 2023-01-30 08:24:22.000000 InCli-0.0.82/test/test_parse.py
--rw-r--r--   0 uormaechea   (502) staff       (20)      293 2022-12-16 14:39:30.000000 InCli-0.0.82/test/test_query.py
--rw-r--r--   0 uormaechea   (502) staff       (20)     6316 2023-03-17 09:15:34.000000 InCli-0.0.82/test/test_restClient.py
--rw-r--r--   0 uormaechea   (502) staff       (20)     3847 2023-05-21 21:18:15.000000 InCli-0.0.82/test/test_traceFlag.py
--rw-r--r--   0 uormaechea   (502) staff       (20)     3426 2023-05-18 12:58:54.000000 InCli-0.0.82/test/test_utilities.py
--rw-r--r--   0 uormaechea   (502) staff       (20)     1922 2023-03-16 10:31:43.000000 InCli-0.0.82/test/test_vlocityErrorEntry.py
--rw-r--r--   0 uormaechea   (502) staff       (20)    12720 2023-02-22 08:07:27.000000 InCli-0.0.82/test/test_z_compareOrgs.py
--rw-r--r--   0 uormaechea   (502) staff       (20)     2841 2023-03-17 09:22:54.000000 InCli-0.0.82/test/test_z_getCartItems.py
--rw-r--r--   0 uormaechea   (502) staff       (20)     1530 2023-04-12 12:16:32.000000 InCli-0.0.82/test/test_z_splunk.py
+drwxr-xr-x   0 uormaechea   (502) staff       (20)        0 2022-12-07 11:17:32.773822 InCli-0.0.9/
+drwxr-xr-x   0 uormaechea   (502) staff       (20)        0 2022-12-07 11:17:32.754355 InCli-0.0.9/InCli/
+-rw-r--r--   0 uormaechea   (502) staff       (20)    11566 2022-12-07 10:09:10.000000 InCli-0.0.9/InCli/InCli.py
+drwxr-xr-x   0 uormaechea   (502) staff       (20)        0 2022-12-07 11:17:32.768408 InCli-0.0.9/InCli/SFAPI/
+-rw-r--r--   0 uormaechea   (502) staff       (20)     8047 2022-12-06 00:07:38.000000 InCli-0.0.9/InCli/SFAPI/Sobjects.py
+-rw-r--r--   0 uormaechea   (502) staff       (20)        0 2022-12-05 21:22:35.000000 InCli-0.0.9/InCli/SFAPI/__init__.py
+-rw-r--r--   0 uormaechea   (502) staff       (20)    18625 2022-12-06 22:52:03.000000 InCli-0.0.9/InCli/SFAPI/debugLogs.py
+-rw-r--r--   0 uormaechea   (502) staff       (20)    10877 2022-12-06 00:26:30.000000 InCli-0.0.9/InCli/SFAPI/digitalCommerce.py
+-rw-r--r--   0 uormaechea   (502) staff       (20)     4818 2022-12-06 22:29:53.000000 InCli-0.0.9/InCli/SFAPI/digitalCommerceUtil.py
+-rw-r--r--   0 uormaechea   (502) staff       (20)     2142 2022-12-05 21:52:50.000000 InCli-0.0.9/InCli/SFAPI/file.py
+-rw-r--r--   0 uormaechea   (502) staff       (20)     2244 2022-12-05 21:42:40.000000 InCli-0.0.9/InCli/SFAPI/jsonFile.py
+-rw-r--r--   0 uormaechea   (502) staff       (20)     9921 2022-12-05 21:12:09.000000 InCli-0.0.9/InCli/SFAPI/objectUtil.py
+-rw-r--r--   0 uormaechea   (502) staff       (20)     4116 2022-12-06 00:07:38.000000 InCli-0.0.9/InCli/SFAPI/query.py
+-rw-r--r--   0 uormaechea   (502) staff       (20)    21128 2022-12-06 22:48:38.000000 InCli-0.0.9/InCli/SFAPI/restClient.py
+-rw-r--r--   0 uormaechea   (502) staff       (20)     2250 2022-12-05 21:22:33.000000 InCli-0.0.9/InCli/SFAPI/thread.py
+-rw-r--r--   0 uormaechea   (502) staff       (20)    11644 2022-12-06 22:30:56.000000 InCli-0.0.9/InCli/SFAPI/utils.py
+-rw-r--r--   0 uormaechea   (502) staff       (20)        0 2022-12-01 08:57:08.000000 InCli-0.0.9/InCli/__init__.py
+drwxr-xr-x   0 uormaechea   (502) staff       (20)        0 2022-12-07 11:17:32.758279 InCli-0.0.9/InCli.egg-info/
+-rw-r--r--   0 uormaechea   (502) staff       (20)      209 2022-12-07 11:17:32.000000 InCli-0.0.9/InCli.egg-info/PKG-INFO
+-rw-r--r--   0 uormaechea   (502) staff       (20)      641 2022-12-07 11:17:32.000000 InCli-0.0.9/InCli.egg-info/SOURCES.txt
+-rw-r--r--   0 uormaechea   (502) staff       (20)        1 2022-12-07 11:17:32.000000 InCli-0.0.9/InCli.egg-info/dependency_links.txt
+-rw-r--r--   0 uormaechea   (502) staff       (20)       43 2022-12-07 11:17:32.000000 InCli-0.0.9/InCli.egg-info/entry_points.txt
+-rw-r--r--   0 uormaechea   (502) staff       (20)       20 2022-12-07 11:17:32.000000 InCli-0.0.9/InCli.egg-info/requires.txt
+-rw-r--r--   0 uormaechea   (502) staff       (20)        6 2022-12-07 11:17:32.000000 InCli-0.0.9/InCli.egg-info/top_level.txt
+-rw-r--r--   0 uormaechea   (502) staff       (20)     1068 2022-12-01 10:54:37.000000 InCli-0.0.9/LICENSE.txt
+-rw-r--r--   0 uormaechea   (502) staff       (20)      209 2022-12-07 11:17:32.773342 InCli-0.0.9/PKG-INFO
+-rw-r--r--   0 uormaechea   (502) staff       (20)      117 2022-12-01 10:53:51.000000 InCli-0.0.9/README.md
+-rw-r--r--   0 uormaechea   (502) staff       (20)      384 2022-12-07 11:17:21.000000 InCli-0.0.9/pyproject.toml
+-rw-r--r--   0 uormaechea   (502) staff       (20)       38 2022-12-07 11:17:32.773936 InCli-0.0.9/setup.cfg
+drwxr-xr-x   0 uormaechea   (502) staff       (20)        0 2022-12-07 11:17:32.772301 InCli-0.0.9/test/
+-rw-r--r--   0 uormaechea   (502) staff       (20)        0 2022-12-01 09:02:19.000000 InCli-0.0.9/test/__init__.py
+-rw-r--r--   0 uormaechea   (502) staff       (20)     1553 2022-12-06 22:33:07.000000 InCli-0.0.9/test/test_InCli.py
+-rw-r--r--   0 uormaechea   (502) staff       (20)      683 2022-12-05 21:56:14.000000 InCli-0.0.9/test/test_file.py
+-rw-r--r--   0 uormaechea   (502) staff       (20)      291 2022-12-05 21:43:56.000000 InCli-0.0.9/test/test_query.py
+-rw-r--r--   0 uormaechea   (502) staff       (20)     6341 2022-12-06 22:11:24.000000 InCli-0.0.9/test/test_restClient.py
```

### Comparing `InCli-0.0.82/InCli/SFAPI/digitalCommerce.py` & `InCli-0.0.9/InCli/SFAPI/digitalCommerce.py`

 * *Files 27% similar despite different names*

```diff
@@ -20,53 +20,39 @@
     ret = ret + paramStr
     isFirst = False
 
   return ret
 
 #------------------------------------------------------------------------
 
-def checkBasketError():
-
-  lc = restClient.lastCall()
-  if lc['error'] is not None:
-      utils.raiseException(lc['errorCode'],lc['error'],lc['action'])
-  if 'error' in lc['response'] and lc['response']['error']!='OK':
-      utils.raiseException(lc['response']['errorCode'],lc['response']['error'],other=lc['action'])
-  if 'success' in lc['response'] and lc['response']['success'] == False:
-      utils.raiseException(lc['response']['errorCode'],f"{inspect.stack()[1].function}: success:{lc['response']['success']}  isBasketValid:{lc['response']['isBasketValid']}")
-  if 'result' in lc['response'] and 'offerDetails' in lc['response']['result']:
-      utils.raiseException(f"CreateBasket {lc['response']['result']['offerDetails']['StatusCode']}",lc['response']['result']['offerDetails']['messages'][0])
-  if 'STATUS' in lc['response'] and lc['response']['STATUS'] == 'ERROR':
-     utils.raiseException(lc['response']['errorCode'],lc['response']['STATUS'])
-  #if lc['response']['result']['error'] !='OK':
-  #  print()
-
 def checkOfferError():
+  #restClient.checkLastCallError('DigitalCommerce API')
+
 
   lc = restClient.lastCall()
   if lc['error'] is not None:
       utils.raiseException(lc['errorCode'],lc['error'],lc['action'])
   if lc['response']['error']!='OK':
       utils.raiseException(lc['response']['errorCode'],lc['response']['error'],other=lc['action'])
   if 'success' in lc['response'] and lc['response']['success'] == False:
       utils.raiseException(lc['response']['errorCode'],f"{inspect.stack()[1].function}: success:{lc['response']['success']}  isBasketValid:{lc['response']['isBasketValid']}")
 
+
 #------------------------------------------------------------------------
 
 def getResult(obj):
 
   if 'result' in obj:
     obj = obj['result']  
   return obj
 
 #------------------------------------------------------------------------
 
-def getCatalogs(catalogueCode=None):
-    where = f" where vlocity_cmt__CatalogCode__c = '{catalogueCode}' " if catalogueCode !=None else ''
-    call = query.query(f'select Fields(ALL) from vlocity_cmt__Catalog__c {where} limit 100')
+def getCatalogs():
+    call = query.query('select Fields(ALL) from vlocity_cmt__Catalog__c limit 100')
     return call['records']
 
 #------------------------------------------------------------------------
 
 def getCatalogProducts(catalogId):
     call = query.query(f"select Fields(ALL) from vlocity_cmt__CatalogProductRelationship__c where vlocity_cmt__CatalogId__c='{catalogId}' limit 100")  
     return call
@@ -88,18 +74,18 @@
   if 'offers' in call:
     return call['offers']
 
   return []
 
 #------------------------------------------------------------------------
 
-def getOfferDetails(catalogcode,offercode,contextkey=None,context=None,forceinvalidatecache=None,isloggedin=None,ts_name=None):
-  paramStr = stringify(locals(),exclude=['catalogcode','offercode',"ts_name"])
+def getOfferDetails(catalogcode,offercode,contextkey=None,context=None,forceinvalidatecache=None,isloggedin=None):
+  paramStr = stringify(locals(),exclude=['catalogcode','offercode'])
   action = f'/services/apexrest/{restClient.getNamespace()}/v3/catalogs/{catalogcode}/offers/{offercode}{paramStr}'
-  call = restClient.callAPI(action,ts_name=ts_name)
+  call = restClient.callAPI(action)
   checkOfferError()
 
 
   lc = restClient.lastCall()
   log = {
       'method':'getOfferDetails',
       'action':f"{lc['url']}{lc['action']}",
@@ -109,36 +95,27 @@
       'error':call['error'],
       'deltaTime':lc['deltaTime'],
       'elapsedTime':lc['elapsedTime']
   }
   lc['log'] = log
   return call
 #------------------------------------------------------------------------
-   
-def createBasket(catalogcode,offer,basketAction='AddWithNoConfig',productConfig=None,contextKey=None,context=None,forceinvalidatecache=None,isloggedin=None,includeAttachment=None,returnBasket=None,validatebasket=None,requestDateTime=None,rootAssetIds=None,canCreateBasket=False,ts_name=None):
-  paramStr = stringify(locals(),exclude=['catalogcode','offer','productConfig','requestDateTime','rootAssetIds','canCreateBasket'])
-  action = f'/services/apexrest/{restClient.getNamespace()}/v3/catalogs/{catalogcode}/basket{paramStr}'
-
-  if basketAction not in ['AddWithNoConfig','AddAfterConfig','AssetToBasket']:
-     utils.raiseException('Invalid_Option',f'bakset Action {basketAction} is not a valid option.')
 
+def createBasket(catalogcode,offer,contextKey=None,context=None,forceinvalidatecache=None,isloggedin=None,includeAttachment=None,returnBasket=None,validatebasket=None):
+  paramStr = stringify(locals(),exclude=['catalogcode','offer'])
+  action = f'/services/apexrest/{restClient.getNamespace()}/v3/catalogs/{catalogcode}/basket{paramStr}'
   restClient.glog().debug(action)
 
   body = {
-    "basketAction": basketAction,
+    "basketAction": "AddWithNoConfig",
+    "offer":offer
   }
-  if basketAction == 'AddWithNoConfig' :    body["offer"]=offer
-  if basketAction == 'AddAfterConfig' :    body["productConfig"]=productConfig
-  if basketAction == 'AssetToBasket' :    
-        body["rootAssetIds"]=rootAssetIds
-        body["requestDateTime"]=requestDateTime
-
-  response = restClient.callAPI(action, method="post", data=body,ts_name=ts_name)
-  filename = restClient.callSave('popopollll',logRequest=True,logReply=False)
-  checkBasketError()
+
+  response = restClient.callAPI(action, method="post", data=body)
+  checkOfferError()
 
   lc = restClient.lastCall()
   log = {
       'method':'AddWithNoConfig',
       'action':f"{lc['url']}{lc['action']}",
       'catalog':catalogcode,
       'offer':offer,
@@ -149,85 +126,63 @@
   }
   lc['log'] = log
 
   return response
 
 #------------------------------------------------------------------------
 
-def createBasketAfterConfig(catalogcode,offerDetails,contextKey=None,context=None,forceinvalidatecache=None,isloggedin=None,includeAttachment=None,returnBasket=None,validatebasket=None,ts_name=None):
-
-  res = createBasket(catalogcode,'',
-                    'AddAfterConfig',
-                    productConfig=getResult(offerDetails),
-                    context=contextKey,
-                    forceinvalidatecache=forceinvalidatecache,
-                    isloggedin=isloggedin,
-                    includeAttachment=includeAttachment,
-                    returnBasket=returnBasket,
-                    ts_name=ts_name)
-  
-  return res
+def createBasketAfterConfig(catalogcode,offerDetails,contextKey=None,context=None,forceinvalidatecache=None,isloggedin=None,includeAttachment=None,returnBasket=None,validatebasket=None):
   paramStr = stringify(locals(),exclude=['catalogcode','offerDetails'])
   action = f'/services/apexrest/{restClient.getNamespace()}/v3/catalogs/{catalogcode}/basket{paramStr}'
   restClient.glog().debug(action)
 
   body = {
     "basketAction": "AddAfterConfig",
     "productConfig": getResult(offerDetails)
   }
 
- # restClient.writeFile('body12xx',body)
+  restClient.writeFile('body12xx',body)
   response = restClient.callAPI(action, method="post", data=body)
-  checkBasketError()
+  checkOfferError()
 
 
   lc = restClient.lastCall()
   log = {
       'method':'AddAfterConfig',
       'action':f"{lc['url']}{lc['action']}",
       'catalog':catalogcode,
       'offer':getOfferCode( offerDetails['result']['offerDetails']['offer']),
       'contextKey':response['cartContextKey'] if 'cartContextKey' in response else "",
-      'error':response['error'] if 'error' in response else "",
+      'error':response['error'],
       'deltaTime':lc['deltaTime'],
       'elapsedTime':lc['elapsedTime']              
   }
   lc['log'] = log
 
   return response
 
 #------------------------------------------------------------------------
-def createBasket_AssetToBasket():
-   print()
-
-def getBasketDetails(catalogcode,basketkey,ts_name=None):
-  action = f'/services/apexrest/{restClient.getNamespace()}/v3/catalogs/{catalogcode}/basket/{basketkey}'
-  restClient.glog().debug(action)
-  response = restClient.callAPI(action, method="get",ts_name=ts_name)
-  checkBasketError()
 
-  return response
-   
-def executeActions(basketAction,ts_name=None):
+def executeActions(basketAction):
   action = basketAction['link']
   body = basketAction['params']
   method="post"
 
   if basketAction['method'] == 'updateBasketAction':
     method = 'put'
 
-  response = restClient.callAPI(action, method=method, data=body,ts_name=ts_name)
-  checkBasketError()
+  response = restClient.callAPI(action, method=method, data=body)
+  response = checkBasketError(response)
   return response
 
 #------------------------------------------------------------------------
 
-def addChildBasket(basket,path,ts_name=None):
+def addChildBasket(basket,path):
   basketAction = digitalCommerceUtil.getAction(basket,path,method='addChildBasketAction')
-  basket2 = executeActions(basketAction,ts_name=ts_name)
+  basket2 = executeActions(basketAction)
 
   return basket2
 
 #------------------------------------------------------------------------
 
 def deleteFromBasket(basket,path):
   basketAction = digitalCommerceUtil.getAction(basket,path,method='deleteFromBasketAction')
@@ -239,14 +194,28 @@
 
 def setError(error,errorCode):
     restClient.glog().error(f"Error {error}  {errorCode}")
     restClient.setLastCallError( error,errorCode)
 
 #------------------------------------------------------------------------
 
+def checkBasketError(basket):
+  response = basket
+  if 'success' in response:
+    if response['success'] == False:
+      setError(response['error'],response['errorCode'])
+      return None
+
+  if len(response['result']['messages'])>0:
+    setError(response['result']['messages'],'basket')
+    return None
+  return basket
+
+#------------------------------------------------------------------------
+
 def updateBasketQuantity(basket,path,value):
   basketAction = digitalCommerceUtil.getAction(basket,path,method='updateBasketAction')
   basketAction['params']['Quantity'] = str(value)
   basket2 = executeActions(basketAction)
   if len(basket2['result']['messages'])==0:
     print('ok')
   else:
@@ -259,14 +228,15 @@
 def updateBasketFields(basket,path,fieldsToBeUpdated):
   basketAction = digitalCommerceUtil.getAction(basket,path,method='updateBasketAction')
   basketAction['params']['fieldsToBeUpdated'] = fieldsToBeUpdated
   basket2 = executeActions(basketAction)
 
   return basket2
 
+
 #  updates = [
 #    {
 #      "Category":'ACAT_EQUIPMENT',
 #      "Attribute":'ATT_SERIAL_NUMBER',
 #      "value":""
 #    }
 #  ]
@@ -287,15 +257,15 @@
   basketAction['params']['attributeCategories'] = attributes
   basket2 = executeActions(basketAction)
 
   return basket2
 
 #------------------------------------------------------------------------
 
-def createCart(accountId,catalogCode,cartContextKey,createAsset=False,assetReferenceKey=None,ts_name=None):
+def createCart(accountId,catalogCode,cartContextKey,createAsset=False,assetReferenceKey=None):
   if type(cartContextKey) is dict:
     cartContextKey = cartContextKey
 
   data = {
     "accountId": accountId,
     "catalogCode": catalogCode,
     "cartContextKey": cartContextKey
@@ -308,16 +278,15 @@
     action = f'/services/apexrest/{restClient.getNamespace()}/v3/carts?{context}&isloggedin=true&price=false&validate=false'
    # action = f'/services/apexrest/{client.getNamespace()}/v3/carts?{context}&isloggedin=true'
 
   if createAsset:
       action = f'{action}&createAsset=true'
 
   #print(data)
-  call = restClient.callAPI(action, method="post", data=data,ts_name=ts_name)
-  checkBasketError()
+  call = restClient.callAPI(action, method="post", data=data)
   return call
 
 #------------------------------------------------------------------------
 
 def printPricing(offerDetails):
   offer = offerDetails['result']['offerDetails']['offer']
   if 'priceResult' in offer:
```

### Comparing `InCli-0.0.82/InCli/SFAPI/file.py` & `InCli-0.0.9/InCli/SFAPI/file.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import os
 import errno
-from . import utils
-
 
 def abspath(filepath):
     return os.path.abspath(filepath)
 
 def addExtension(filename,extension):
     if '.' not in extension:
         extension = '.' + extension
@@ -19,45 +17,45 @@
         return True #local file
     if not os.path.exists(os.path.dirname(filename)):
         try:
             os.makedirs(os.path.dirname(filename))
             return True
         except OSError as exc: # Guard against race condition
             if exc.errno != errno.EEXIST:
-                utils.raiseException('OSError',f"Error creating directory {dirname}  {exc.errno}")
+                raise   
     return False
 
 #def getFilePath(folder,filename):
 
 def writeFileinFolder(folder,filename,data):
     return write(f"{folder}/{filename}",'.txt',data)
 
 def delete(filename):
     os.remove(filename)
 
 
 def write(filepath,data,mode="w"):
     _createDirectories(filepath)
-    f = open(filepath,mode,encoding="utf-8")
+    f = open(filepath,mode)
     f.write(data)
     f.close()
 
     return os.path.abspath(filepath)
 
 def exists(filepath):
     return os.path.exists(filepath)
 
 def read(filepath):
-    f = open(filepath,"r",encoding="utf-8",errors='ignore')
+    f = open(filepath,"r")
     data = f.read()
     f.close()
     return data
 
 def openFile(filepath,mode="w"):
-    f = open(filepath,mode,encoding="utf-8",errors='ignore')
+    f = open(filepath,mode)
     return f
 def write_line(f,line):
     f.write(line+ "\n")
     return f
 def closeFile(f):
     f.close()
```

### Comparing `InCli-0.0.82/InCli/SFAPI/jsonFile.py` & `InCli-0.0.9/InCli/SFAPI/jsonFile.py`

 * *Files identical despite different names*

### Comparing `InCli-0.0.82/InCli/SFAPI/objectUtil.py` & `InCli-0.0.9/InCli/SFAPI/objectUtil.py`

 * *Files 14% similar despite different names*

```diff
@@ -56,66 +56,30 @@
         return rets
     p = parse(obj, selectKey=selectKey, selectKeyValue=selectKeyValue,logValues=logValues)
     treeObjects = treeObjects[0:ident+1]
     keyPath = keyPath[0:ident+1]
 
     return p
 
-def getSibling_atPath(obj,path,field='ProductCode'):
-    for p in path.split(':'):
-        obj = getSibling(obj,field,p)  
-    return obj
-
-def getSiblingWhere_path(obj, selectKey,selectKeyValuePath, whereKey=None,whereValue=None,logValues=False):
-    paths = selectKeyValuePath.split(':')
+def getSiblingWhere(obj, selectKey,selectKeyValue=None, whereKey=None,whereValue=None,logValues=False):
 
     result = {
         'level':-1,
         'keys':[],
         'objects':[],
-        'object':None,
-        'object_list':[]
-    }
-    for path in paths:
-        index = 0
-        if '|' in path:
-            index = int(path.split('|')[1])
-            path = path.split('|')[0]
-
-        r = getSiblingWhere(obj, selectKey,path, whereKey,whereValue,logValues,onlyOne=False)
-
-        if len(r['object_list'])==0:
-            return None
-        
-        result['object'] = r['object_list'][index]
-        result['object_list'] = r['object_list']
-        result['objects'].extend(r['objects'])
-
-
-        obj = result['object']
-        
-    return result
-
-def getSiblingWhere(obj, selectKey,selectKeyValue=None, whereKey=None,whereValue=None,logValues=False,onlyOne=True):
-
-    result = {
-        'level':-1,
-        'keys':[],
-        'objects':[],
-        'object':None,
-        'object_list':[]
+        'object':None
     }
 
     if isinstance(obj,list)==True:
         for element in obj:
-            ret = parseWhere(element, selectKey=selectKey,selectKeyValue=selectKeyValue, whereKey=whereKey, whereValue=whereValue,logValues=logValues,result=result,onlyOne=onlyOne)
+            ret = parseWhere(element, selectKey=selectKey,selectKeyValue=selectKeyValue, whereKey=whereKey, whereValue=whereValue,logValues=logValues,result=result)
             if ret['object'] != None:
                 return ret
         return None
-    ret = parseWhere(obj, selectKey=selectKey, selectKeyValue=selectKeyValue,whereKey=whereKey, whereValue=whereValue,logValues=logValues,result=result,onlyOne=onlyOne)
+    ret = parseWhere(obj, selectKey=selectKey, selectKeyValue=selectKeyValue,whereKey=whereKey, whereValue=whereValue,logValues=logValues,result=result)
     if ret['level']<0:
         ret['level'] = 0
     ret['keys'] = ret['keys'][0:ret['level']]
     ret['objects'] = ret['objects'][0:ret['level']]
 
     return ret
 #------------------------
@@ -127,97 +91,57 @@
 
 def getValue(obj,name):
     value = obj[name]
     if 'value' in obj[name]:
         value = obj[name]['value']  
     return value
 
+#set selecte key where keyvalue is selectKeyValue and return jsonDic 
+# if set Key provided, will replace the setKeyValue
+def parseWhere(json,result,selectKey='', selectKeyValue=None,whereKey=None, whereValue=None,logValues=False):
+    def setret(result,json):
+        result['object'] = json
+        return result      
 
-def _match_obj(obj,key,selectKey,selectKeyValue,whereKey,whereValue):
-    if key == selectKey:
-        if selectKeyValue == None:
-            if whereKey == None:
-                return obj[key]
+    result['level']=result['level']+1
+    result['objects'].insert(result['level'], json)
 
-        else:
-            value = getValue(obj,selectKey) 
-            if value == selectKeyValue:
+    if isinstance(json,dict)==False and isinstance(json,list)==False:
+        return setret(result,None)
+
+    for key in json.keys():
+        result['keys'].insert(result['level'],key)
+
+        if key == selectKey:
+            if selectKeyValue == None:
                 if whereKey == None:
-                    return obj
-                elif whereKey in obj:
-                    if whereValue == None:
-                        return obj
-                    if obj[whereKey] == whereValue:
-                        return obj
-    return None
-             
-#set selecte key where keyvalue is selectKeyValue and return jsonDic 
-# if set Key provided, will replace the setKeyValue
-def parseWhere(obj,result,selectKey='', selectKeyValue=None,whereKey=None, whereValue=None,logValues=False,onlyOne=True,_level=-1,_objects=[]):
-    """
-    if selectKeyValue = None, if the obj contains the selectKey is a match. 
-    if whereValue = None, if the obj contains the whereKey is a match. 
-    """
-    #result['level']=result['level']+1
-    _level = _level+1
-    if len(_objects) > _level:
-        _objects[_level] = obj
-    else:
-        _objects.append(obj)
-    if len(_objects) > _level:
-        _objects = _objects[0:_level+1]
-  #  result['objects'].insert(result['level'], obj)
-  #  if len(result['objects']) > _level:
-  #      result['objects'] = result['objects'][0:_level+1]
-    _object_list = []
-
-
-    if isinstance(obj,dict)==False and isinstance(obj,list)==False:
-        result['object'] = None
-        return result
-
-    matchfields = ['records','lineItems','childProducts','productGroups','result']
-    if selectKey not in matchfields: matchfields.append(selectKey) 
-
-    _keys = list(obj.keys())
-    for key in obj.keys():
-        if key not in matchfields: continue
-        if 1==2:
-            if len(result['keys']) > _level:
-                result['keys'][_level] = key
+                    return setret(result,json[key])
+
             else:
-                result['keys'].append(key)
-            if len(result['keys']) > _level:
-                result['keys'] = result['keys'][0:_level+1]
-            print(result['keys'])
-        match_obj = _match_obj(obj,key,selectKey,selectKeyValue,whereKey,whereValue)
-        if match_obj!= None:
-            result['object'] = match_obj
-            result['level'] = _level
-            result['objects'] = _objects
-            return result         
-
-        if isinstance(obj[key],dict):
-            ret = parseWhere(obj[key],result,selectKey, selectKeyValue,whereKey,whereValue,logValues,onlyOne=onlyOne,_level=_level)
-            if ret['object'] != None:  
-                return ret
+                value = getValue(json,selectKey) 
+                if value == selectKeyValue:
+                    if whereKey == None:
+                        return setret(result,json)
+                    elif whereKey in json:
+                        if json[whereKey] == whereValue:
+                            return setret(result,json)
 
-        if isinstance(obj[key],list):
-            for x,l in enumerate(obj[key]):
-                ret = parseWhere(l,result,selectKey,selectKeyValue,whereKey,whereValue,logValues,onlyOne=onlyOne,_level=_level)
-                if ret['object'] != None :
-                    if onlyOne or len(ret['object_list'])>0:
-                        return ret
-                    else:
-                        _object_list.append(ret['object'])    
+        if isinstance(json[key],dict):
+            ret = parseWhere(json[key],result,selectKey, selectKeyValue,whereKey,whereValue,logValues)
 
-            if len(_object_list)>0:
-                result['object_list'] = _object_list
-                return result
-   # result['level'] = result['level']-1
+            if ret['object'] != None:
+                return ret
+
+        if isinstance(json[key],list):
+            for l in json[key]:
+                ret = parseWhere(l,result,selectKey,selectKeyValue,whereKey,whereValue,logValues)
+  
+                if ret['object'] != None:
+                    return ret
+    result['level'] = result['level']-1
 
     result['object'] = None
     return result
 
 def parse(json, selectKey='', selectKeyValue='',setKey='', setKeyValue='',logValues=False,rets=None):
     global ident,treeObjects
     ident=ident+1
@@ -326,19 +250,14 @@
 def addNode(path,node,level):
     if len(path) > level:
         path[level] = node
     else:
         path.append(node) 
 
 def getField(obj,path,separator=':'):
-    """
-    Get field in object for a path. 
-    - path: the path
-    - separator: for the path. a:b:c by default. 
-    """
     paths = path.split(separator)
     _obj = obj
     for p in paths:
         if p in _obj:
             _obj = _obj[p]
         else:
             return None
@@ -392,13 +311,8 @@
                 obj = obj[nodeName]
             else:
                 return "Error: " + nodeName + " not present in Object"
 
     return obj
 
 
-def replace_everywhere_in_obj(obj,find,replace):
-    strAll = simplejson.dumps(obj)
-    stItems2 = strAll.replace(find,replace)
-    return simplejson.loads(stItems2)
-
```

### Comparing `InCli-0.0.82/InCli/SFAPI/query.py` & `InCli-0.0.9/InCli/SFAPI/query.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,116 +1,42 @@
 import logging,json,simplejson
 #from posixpath import split
 from . import restClient as client
-from . import Sobjects,utils,thread
+from . import Sobjects,utils
 " select fields(all) from vlocity_cmt__EntityFilter__c where Id in ('a5W7Z0000009gEiUAI','a5W7Z0000009gdtUAA','a5W7Z0000009gFfUAI','a5W7Z0000009gEdUAI')"
 
-def _querry_api(q):
-    return client.callAPI(f'/services/data/v55.0/query?q={q}')
-
-def _query(q,raiseEx=True,logResponse = False,nextRecords=True,popAttributes=True):
+def _query(q,raiseEx=True,logResponse = False):
     logging.debug(q)
-    call = _querry_api(q)
-
-    call_next = call
-    if nextRecords:
-        while 'nextRecordsUrl' in call_next:
-            call_next = client.callAPI(call_next['nextRecordsUrl'])
-            call['records'].extend(call_next['records'])
+    call = client.callAPI(f'/services/data/v55.0/query?q={q}')
+    lc = client.lastThreadCall()
 
-    if checkError(q,raiseEx) == True:
+    lc['query']=q
+    if lc['error'] != None:
+        lc['query'] = q
+        if raiseEx==True:
+            utils.raiseException(lc['errorCode'],lc['error'],'query',f"{lc['errorOther']} . {q}")
+            raise ValueError(simplejson.dumps(call, indent=4))
         logging.warn(simplejson.dumps(call, indent=4))
+
         return None
-    
+
     if logResponse == True:
         utils.printJSON(call)
-    for r in call['records']: r.pop('attributes')
-
-    return call
-
-def _query_base64(q,raiseEx=True):
-    call = _querry_api(q)
-    checkError(q,raiseEx)
-    if call['totalSize'] > len(call['records']):
-        len_max_records = len(call['records'])
-        q_order = f"{q} order by Id asc"
-        call = _query(q_order,nextRecords=False)
-        len_records_last_call = len(call['records'])
-        call_next = call
-        while (len_records_last_call==len_max_records):
-            lastId = call_next['records'][len_max_records-1]['Id']
-            q_and= f"{q} and Id>'{lastId}' order by Id asc"
-            call_next = _query(q_and,nextRecords=False)
-            call['records'].extend(call_next['records'])
-            len_records_last_call = len(call_next['records'])
 
     return call
 
-def query_threaded(q,values,search="$$$",raiseEx=True):
-    result = []
-
-    def do_work(value):
-        q1 = q.replace(search,value)
-        res = _query(q1)
-        return res
-
-    def on_done(res,result):
-        result.append(res)
-
-    thread.execute_threaded(values,result,do_work,on_done,threads=1)
-
-def checkError(q,raiseEx=True):
-    lc = client.lastCall()
-
-    lc['query']=q
-    if lc['error'] != None:
-        lc['query'] = q
-        if raiseEx==True:
-            if 'serverResponse:' in lc['response']:
-                s = '{"a":' + lc['response'].split('serverResponse:')[-1] + "}"
-                obj = simplejson.loads(s)
-                utils.raiseException(obj['a'][0]['errorCode'],obj['a'][0]['message']).replace('\n', ' ')
-            errorOther = lc['errorOther'] if 'errorOther' in lc else ''
-            utils.raiseException(lc['errorCode'],lc['error'],'query',f"{errorOther} . {q}")
-        return True    
-    return False
-
 #--------------------------------------------------------------------------------------------------------------------------------------------------------
-def query(q,raiseEx=True,logResponse=False,base64=False,in_list=None,in_size=650):
+def query(q,raiseEx=True,X=['Id','Name'],logResponse=False):
     """
     Executes a query in Salesforce.
     - q: the query string. "select.... from... limit..."
         the where clause can specify a normal field or $X and $Z. 
     - X: by default it will query for Id and Name. 
     - logResponse: 
     """
-    def do_query(q,raiseEx,logResponse):
-        if base64:
-            return _query_base64(q,raiseEx)
-        else:
-            return _query(q,raiseEx,logResponse)
-        
-    if in_list == None:
-       return do_query(q,raiseEx,logResponse)
-
-    def divide_chunks(l, n):
-        for i in range(0, len(l), n):
-            yield l[i:i + n]
-    
-    ls_s= list(divide_chunks(in_list,in_size))
-    call = {
-        'records':[]
-    }
-    for ls in ls_s:
-        lsc = [f"'{l}'" for l in ls]
-        q1 = q.replace('$$$IN$$$',",".join(lsc))
-        res = do_query(q1,raiseEx,logResponse)
-        call['records'].extend(res['records'])
-
-    return call
     if '$X=' not in q and '$Z=' not in q:
         return _query(q,raiseEx,logResponse)
 
     if '$Z='  in q:
         X=['Id','ProductCode','Name']
         q = q.replace('$Z=','$X=')
 
@@ -131,67 +57,63 @@
         q1 = q.replace('$X',field)
         call = _query(q1,raiseEx=False)      
         if call['totalSize'] > 0:
             return call
 
     return None
 
-def queryRecords(q,raiseEx=True):
-    select = query(q,raiseEx)
+def queryRecords(q,raiseEx=True,X=['Id','Name']):
+    select = query(q,raiseEx,X)
     if select == None:
         return None
     return select['records']
 
 cache = {}
-def queryFieldList(q,field=None,raiseEx=False):
-    records = queryRecords(q,raiseEx)
+def queryFieldList(q,field=None,raiseEx=False,X=['Id','Name']):
+    if '$X=' in q or '$Z=' in q:
+        print(q)
+        if q in cache:
+            return cache[q]
+    records = queryRecords(q,raiseEx,X)
 
     if records == None:
         return None
 
     if field == None:
         field = q.strip().split()[1]
     
     fieldList = []
   
     for record in records:
         fieldList.append(record[field])
+        
+    if '$X=' in q or '$Z=' in q:
+        cache[q]=fieldList
 
     return fieldList
 
 #" select Id from vlocity_cmt__AttributeAssignment__c where vlocity_cmt__AttributeUniqueCode__c='ATT_MOBILE_CREDITS' and  vlocity_cmt__ObjectId__c='01t7Z00000AVpCLQA1' "
-def queryField(q,field=None,raiseEx=False):
-    fieldList = queryFieldList(q,field,raiseEx)
+def queryField(q,field=None,raiseEx=False,X=['Id','Name']):
+    fieldList = queryFieldList(q,field,raiseEx,X)
 
     if fieldList == None or len(fieldList) == 0:
         return None
 
     if len(fieldList) > 1:
         logging.warn(f"There is more than one record returned. total records {len(fieldList)}, query={q}")
 
     return fieldList[0]
 
-def queryIdF(objName,extendedF,init=None):
-    """Returns the Id for the especified extendedF.
-    - if extendedF is a string, returns the string
-    - if extendedF is a dictionary, return extendedF['Id]
-    - if extendedF is a fieldName:fieldValue, returns the query on object where fieldName=fieldValue
-    """
+def queryIdF(objName,extendedF):
     if extendedF == None:
         return None
-    if type(extendedF) is dict:
-        extendedF = extendedF['Id']
     ef = utils.extendedField(extendedF)
     if ef['field'] == 'Id':
-        if Sobjects.checkId(ef['value']):
-            return ef['value']
-        else:
-            utils.raiseException("No_Id",f"{extendedF} is not a valid Id")
+        return ef['value']
     return queryField(f" select Id from {objName} where {ef['field']} = '{ef['value']}' ")
-
 def logQuery(q,filename,raiseEx=False):
     if filename != None:
         client.logCall(filename)
     call = query(q,raiseEx)
 
     return call
 
@@ -204,12 +126,12 @@
     client.debugFile(fileName)
     client.setDebugReplyProcessing(postProcessing)
     query(q)
 
 def records(call):
     return call['records']
 
-def  IN_clause(list):
+def IN_clause(list):
     values = []
     for p in list:
         values.append(f"'{p}'")
     return ",".join(values)
```

### Comparing `InCli-0.0.82/InCli/SFAPI/restClient.py` & `InCli-0.0.9/InCli/SFAPI/restClient.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,142 +1,110 @@
 import os,sys,sys,gc
 from xmlrpc.client import Boolean
-from . import Sobjects, jsonFile,file, objectUtil,utils,timeStats
+from . import Sobjects, jsonFile,file, objectUtil,utils
 import requests,threading
 import logging,datetime,enum
 import simplejson as json
 
 _initializedConnections = []
 _allThreadsContext = {}
 _currentConnectionName = None
-
-def _create_thread_context(connection_name):
-    global _currentConnectionName
-    _currentConnectionName = connection_name if connection_name != None else _currentConnectionName
-    if _currentConnectionName == None:
-        utils.raiseException('ConnectionError',"Current Connection is no set.")
-    th = {
-            'connectionName': _currentConnectionName,
-            'calls':[]
-        }
-    _allThreadsContext[threading.get_native_id()] = th
-
-    return th
-
-def _get_thread_context(setConnectionName=None):
+def _threadContext(setConnectionName=None):
     """
     Threads can share a connection. However the call stack belongs to each thread.
     When a thread calls this function, it can set the connection for the thread (if especified) or get the connection previously set if setConnectionName=None
     If a connection has not been set fot the thread, the current one (the latest one set for any previous thread) is assigned to the thread   
     """
     global _allThreadsContext,_currentConnectionName
-    thread_id = threading.get_native_id()
-    if thread_id not in _allThreadsContext:
-    #    _currentConnectionName = setConnectionName if setConnectionName != None else _currentConnectionName
-    #    if _currentConnectionName == None:
-    #        utils.raiseException('ConnectionError',"Current Connection is no set.")
-        return _create_thread_context(setConnectionName)
-
-     #   _allThreadsContext[thread_id] = th
-     #   return th
+    id = threading.get_native_id()
+    if id not in _allThreadsContext:
+        _currentConnectionName = setConnectionName if setConnectionName != None else _currentConnectionName
+        if _currentConnectionName == None:
+            utils.raiseException('ConnectionError',"No default connection for thread")
+        th = {
+            'connectionName': _currentConnectionName,
+            'calls':[]
+        }
+        _allThreadsContext[id] = th
+        return th
     if setConnectionName != None:   #change the connection for the thread
-        _allThreadsContext[thread_id]['connectionName'] = setConnectionName
+        _allThreadsContext[id]['connectionName'] = setConnectionName
         _currentConnectionName = setConnectionName
-    return _allThreadsContext[thread_id]
+    return _allThreadsContext[id]
 
 ##################################################################
 def _pushThreadCall(call):
-    max_calls = 5
-    _calls = _get_thread_context()['calls']
-    if len(_calls) == max_calls:
+    _calls = _threadContext()['calls']
+    if len(_calls) == 5:
         _calls.pop(0)
     _calls.append(call)
 
 def _updateThreadCall(call):
-    _calls = _get_thread_context()['calls']
+    _calls = _threadContext()['calls']
     _calls[-1] = call
 
 def lastCall(field=None):
-    return _thread_lastCall(field)
-
-def thread_get_calls():
-    return _get_thread_context()['calls']
-
-def _thread_lastCall(field=None,index=-1):
+    return lastThreadCall(field)
+def lastThreadCall(field=None):
     """
     Returns the last rest call data (request, response, others).
     """
-    _calls = _get_thread_context()['calls']
+    _calls = _threadContext()['calls']
     if field == None:
-        return _calls[index]
-    return _calls[index][field]
+        return _calls[-1]
+    return _calls[-1][field]
 
-def checklastThreadCallError(caller,index=-1):
+def checklastThreadCallError(caller):
     """
     Raises and Exception if the last call has an error. """
-    lc = _thread_lastCall(index)
+    lc = lastThreadCall()
     if 'error' in lc and lc['error'] is not None:
         utils.raiseException(lc['errorCode'],lc['error'],caller)
 
-def _get_call_times(call):
-    et = call['elapsedTime']
-    delta = call['deltaTime']
-    times = {
-        'elapsed':(et.microseconds + et.seconds * 1000000 )/1000,
-        'delta':(delta.microseconds + delta.seconds * 1000000 )/1000,
-    }
-    return times 
-
-def _thread_lastCall_time(index=-1):
-    t = _thread_lastCall('elapsedTime',index=index)
+def getLastCallTime():
+    return getlastThreadCallTime()
+def getlastThreadCallTime():
+    t = lastThreadCall('elapsedTime')
     return (t.microseconds + t.seconds * 1000000 )/1000
 
-def getLastCallAllTimes(index=-1):
-    call = _thread_lastCall(index=index)
-    return _get_call_times(call)
-
-def getLastCallElapsedTime(index=-1):
-    return _thread_lastCall_time(index=index)
-
 def getConfigOrgsNames():
     """
     Get all names for the org in the config file."""
     return [configOrg['name'] for configOrg in loadConfigData()['orgs']]
 
 ##################################################################
 
-
+def glog():
+    return logging.getLogger('root')
 #/Users/uormaechea/Documents/Dev/python/Industries/input/ConnectionsParams.json
 _configData = None
 _configDataName = None
-#def setLoggingLevel(loggingLevel=logging.INFO):
-#    glog().level = loggingLevel
+def setLoggingLevel(loggingLevel=logging.INFO):
+    glog().level = loggingLevel
 
 def loadConfigData():
     global _configData,_configDataName
 
     if _configData is not None:
         return _configData
     
     incli = os.environ.get('INCLI')
     if incli is not None:
         setConfigFile(incli)
         return _configData
-    
-    root_folder = "incli"
 
-    _configDataName = os.path.abspath(f"{root_folder}/IncliConf.json")
+    _configDataName = os.path.abspath(".incli/IncliConf.json")
 
     if file.exists(_configDataName) == False:
         configData = {
             "folders": {
-                "input":os.path.abspath(f"{root_folder}/input"),
-                "debug":os.path.abspath(f"{root_folder}/debug"),
-                "output":os.path.abspath(f"{root_folder}/output"),
-                "log":os.path.abspath(f"{root_folder}/logs")
+                "input":os.path.abspath(".incli/input"),
+                "debug":os.path.abspath(".incli/debug"),
+                "output":os.path.abspath(".incli/output"),
+                "log":os.path.abspath(".incli/logs")
             },
             "orgs": []
         }
 
         jsonFile.write(_configDataName,configData)
 
     _configData = jsonFile.read(_configDataName)
@@ -193,22 +161,18 @@
 def deleteOrg_inConfigFile(orgName):
     cd = loadConfigData()
     cd2 = [i for i in cd['orgs'] if not (i['name'] == orgName)]
     cd['orgs'] = cd2
     jsonFile.write(_configDataName,cd)
     loadConfigData()
 
-loggerName = 'restClient'
-def glog():
-    return logging.getLogger(loggerName)
 def setLoggingLevel(level=logging.INFO):
-    log = logging.getLogger(loggerName)
+    log = logging.getLogger('root')
     logging.basicConfig()
     log.setLevel(level)
-    pass
 
 def setConfigFile(configFile):
     """
     Set the config file to use, and the log level"""
     global _configData,_configDataName
 
     if file.exists(configFile):
@@ -217,67 +181,55 @@
         utils.raiseException("NO_CONFIG",f"Cannot open the configuration file <{configFile}>, please provide a valid configuration file (path and name).")
 
     _configDataName = configFile
 
 sfdx_lock = threading.Lock()
 ####CONECTION
 def init(userName_or_orgAlias,connectionName=None):
-    if userName_or_orgAlias  != 'ConnectionLess' and userName_or_orgAlias != None:
-        print(f"Initializing connection for {userName_or_orgAlias}")
-    if userName_or_orgAlias == 'ConnectionLess':
-        _initMain(userName_or_orgAlias,None)
-        return
     with sfdx_lock:
         inConf = False
         if userName_or_orgAlias == None:
             userName_or_orgAlias = getConfigVar('u')
             if userName_or_orgAlias == None:
-                utils.raiseException('Configuration',f"No userName or Org Alias specified. Please specify a user name or org alias -> InCli -u orgAlias ...")
+                utils.raiseException('Configuration',"No userName or Org Alias specified. Please specify a user name or org alias.")
             inConf = True    
-            print(f"{utils.CFAINT}Using default connection,{utils.CEND}{utils.CGREEN} {userName_or_orgAlias}.{utils.CEND}")
 
         connectionName = connectionName if connectionName is not None else userName_or_orgAlias
         if _checkAndSetConnectionIfExists(connectionName):
             return
 
         try:
-            glog().debug(f"Calling sfdx")
-            success,obj,outputs = utils.execute_force_org_display(userName_or_orgAlias)
-            if success == False:
-                utils.raiseException('SFDXError',f"Connection failed. {outputs.stderr}")
-
-            if obj['Connected Status'] != 'Connected':
-                utils.raiseException('SFDXError',f"Connection failed. Connected Status:{obj['Connected Status']}")
+            success,outputs = utils.executeCommandParse(["sfdx","force:org:display","-u", userName_or_orgAlias])
 
-            glog().debug(f"post sfdx")
-
-        except utils.InCliError as e:
-                raise e
         except Exception as e:
-                if e.strerror == 'No such file or directory':
-                    utils.raiseException('SFDXError',"SFDX is not installed or it is not accesible.",other='https://developer.salesforce.com/docs/atlas.en-us.sfdx_setup.meta/sfdx_setup/sfdx_setup_install_cli.htm')
+            if e.strerror == 'No such file or directory':
+                utils.raiseException('SFDXError',"SFDX is not installed or it is not accesible.",other='https://developer.salesforce.com/docs/atlas.en-us.sfdx_setup.meta/sfdx_setup/sfdx_setup_install_cli.htm')
+            else:
                 utils.raiseException('SFDXError',e.strerror)
 
         if success is False:
             error = outputs.stderr.split('force:org:display')[1]
             if 'No AuthInfo found' in error:
                 addText = " set in the configuration " if inConf==True else ''
                 utils.raiseException('ConnectionError',f"{error}. Please authorize the org for the {userName_or_orgAlias}{addText}: sfdx auth:web:login",other="Check Connection status: sfdx force:org:list --verbose --all")
             else:
                 utils.raiseException('SFDX Error',error,other='')
 
+        obj  = {}
+        for output in outputs:
+            obj[output['KEY']] = output['VALUE']
+
         if obj['Connected Status'] != 'Connected':
             utils.raiseException("ConnectionStatus",f"Connected Status for client Id {userName_or_orgAlias} is {obj['Connected Status']}",other=f"Execute the following command to refresh the token.  -")
 
         assert(connectionName!=None)
         assert(obj['Instance Url']!=None)
         assert(obj['Access Token']!=None)
 
-        _initMain(connectionName,obj['Instance Url'],obj['Access Token'],username= obj['Username'])
-        return obj
+        _initMain(connectionName,obj['Instance Url'],obj['Access Token'])
 
 def initWithToken(name,url,token=None,input=None,output=None,debug=None):
     _initMain(name,url,token,input,output,debug)
 
 def initWithConfig(orgName,isGuest=False,connectionName=None)->Boolean:
     """
     Reads the ConnectionsParams.json configuration specified by environment. If isGuest=False it will authenticate with Salesforce and obtain the token and url. If isGuest=True, it will not authenticate and the url must be provided in the ConnectionsParams.
@@ -313,21 +265,20 @@
     _initMain(connectionName,url=url,token=token)
 
     return True
 
 def _checkAndSetConnectionIfExists(connectionName):
     for con in _initializedConnections:
         if con['connectionName'] == connectionName:
-            _get_thread_context(connectionName)
-            if connectionName != 'ConnectionLess':
-                glog().info(f"Connection {connectionName} set.")
+            _threadContext(connectionName)
+            glog().info(f"Connection {connectionName} set.")
             return True
     return False
 
-def _initMain(name,url,token=None,input=None,output=None,debug=None,username=None):
+def _initMain(name,url,token=None,input=None,output=None,debug=None):
     if _checkAndSetConnectionIfExists(name):
         return
 
     loadConfigData()
 
   #  currentDir = os.getcwd()
     connection = {
@@ -338,31 +289,25 @@
         'input':input if input is not None else _configData['folders']['input'],
         'output':output if input is not None else _configData['folders']['output'],
         'debug':debug if input is not None else _configData['folders']['debug'],
         'log':debug if input is not None else _configData['folders']['log'],
 
         'nameSpace':'vlocity_cmt'
     }
-    if username != None:
-        connection['username'] = username
     _initializedConnections.append(connection)
-    _get_thread_context(connection['connectionName'])
-    if name != 'ConnectionLess':
-        if connection['connectionName'] == username:
-             print(f"{utils.CYELLOW}Connection {connection['connectionName']} initialized.{utils.CEND}")
+    _threadContext(connection['connectionName'])
 
-        else:
-            print(f"Connection {connection['connectionName']} initialized for username {username}.")
+    glog().info(f"Connection {connection['connectionName']} initialized.")
 
 def getCurrentThreadConnection():
     """
     Retrieves the connectionParams for the current org. 
     """
     global _initializedConnections
-    connectionName = _get_thread_context()['connectionName']
+    connectionName = _threadContext()['connectionName']
     if connectionName == None:
         utils.raiseException('ConnectionError',"No connection has been established for current thread.",other="Make sure the connection is established.")
     connection = [con for con in _initializedConnections if con['connectionName']==connectionName][0]
     #connection = objectUtil.getSibling(_initializedConnections,"name",name)
     return connection
 
 def getNamespace():
@@ -373,75 +318,47 @@
 def outputFolder():
     return _gerFolder('output')
 def debugFolder():
     return _gerFolder('debug')
 def logFolder():
     return _gerFolder('log')
 def _gerFolder(name):
-    try:
-        folder =  getCurrentThreadConnection()[name]
-    except Exception as e:
-        if e.args[0]['error'] == 'No default connection for thread' or e.args[0]['error'] == 'Current Connection is no set.':
-            loadConfigData()
-            folder = _configData['folders'][name]
-        else:
-            raise
-
+    folder =  getCurrentThreadConnection()[name]
     if folder[-1] != '/':
         folder = folder + '/'
     if file.exists(folder) == False:
         os.makedirs(folder)
     return folder
 
+#################################################################################################################################
 def _authenticate(login,isSandbox):
     if 'isSandBox' == None:
         raise ValueError(f"Environment connection parameters missing isSandBox field.")
 
     headers = {
         'Content-type': 'application/x-www-form-urlencoded'
     }
     server = 'test' if isSandbox else 'login'
-    _get_thread_context('oauth2')
+    _threadContext('oauth2')
     call = requestRaw(url=f"https://{server}.salesforce.com/services/oauth2/token",method='post', parameters= login,headers=headers)
     
-    lc = _thread_lastCall()
+    lc = lastThreadCall()
     if lc['error'] is not None:
         utils.raiseException(lc['errorCode'],lc['error'],other=lc['errorOther'])
 
    # connection['access_token'] = call["access_token"]
    # connection['instance_url'] = call["instance_url"]
 
     glog().info('getting token')
     glog().info(f"Authenticated. Instance URL is {call['instance_url'] }")
     glog().info(f"Authenticated. Bearer token {call['access_token']}")
 
     return call["instance_url"],call["access_token"]
-#################################################################################################################################
-
-ts = timeStats.TimeStats()
-def new_time_record():
-    global ts
-    ts.new()
-
-def time_print():
-    global ts
-    ts.print()
-
-def checkError():
-    lc = lastCall()
-
-    if 'error' in lc and lc['error'] != None and len(lc['error'])>10:
-        if 'response' in lc:
-            if 'serverResponse:' in lc['response']:
-                s = '{"a":' + lc['response'].split('serverResponse:')[-1] + "}"
-                obj = json.loads(s)
-                utils.raiseException(obj['a'][0]['errorCode'],obj['a'][0]['message'])
-        utils.raiseException(lc['errorCode'],lc['error'])
 
-def requestRaw(url,action=None,method = 'get',parameters = {},data={},headers={},access_token=None,ts_name=None):
+def requestRaw(url,action=None,method = 'get',parameters = {},data={},headers={},access_token=None):
     """
     Basic request Call. 
     
     No need to perform init(), as it does not use the connectionParams and all information needs to be provided. 
     Method parameters are self explanatory. 
 
     """
@@ -468,21 +385,19 @@
         'action':action,
         'url':url,
         'parameters':parameters,
         'method':method,
         'data':data,
         'error':None,
         'errorCode':None,
-        'callTime':datetime.datetime.now(),
-        'errorOther' : ''
+        'callTime':datetime.datetime.now()
     }
 
-    if _currentConnectionName != 'ConnectionLess':
-        glog().debug(f"Current Connection {_currentConnectionName}")
-        _pushThreadCall(call)
+    glog().debug(f"Current Connection {_currentConnectionName}")
+    _pushThreadCall(call)
 
     r = None
 
     glog().debug(f"{call['url']}{call['action']}")
     try:
         if method in ['get','delete']:
             r = requests.request(method, completeUrl, headers=allheaders, params=parameters, timeout=300)
@@ -503,106 +418,97 @@
     except requests.exceptions.Timeout as errt:
         call['error'] = {'Timeout':f"{errt}"}
         call['errorCode'] = f"Timeout Error"    
     except requests.exceptions.RequestException as err:
         call['error'] = {'RequestException':f"{err}"}
         call['errorCode'] = f"RequestException"
 
-    call['responseTime'] = datetime.datetime.now()
-    call['deltaTime'] = call['responseTime'] - call['callTime']
-
     if r != None:
         glog().debug(f'Debug: API {method} call: {r.url}  status Code:{r.status_code}' ) 
         
+        call['responseTime'] = datetime.datetime.now()
         call['status_code'] = r.status_code
         call['elapsedTime'] = r.elapsed
         call['elapsedTimeCall'] = r.elapsed
-
-        if ts_name != None:
-            ts.time_inner(ts_name,r.elapsed)
+        call['deltaTime'] = call['responseTime'] - call['callTime']
 
         if r.status_code < 300 :
             if r.text == '':
                 call['response'] = ''
             else:
                 try:
                     call['response'] = r.json()
             
                 except Exception as e:
                     glog().debug(f"warn. Response is not json  --> {e}")
                     call['response'] = {}
                     call['response'] = r.text
                 
         else:
-          #  glog().warn('API error when calling %s : %s' % (r.url, r.content))
+            glog().warn('API error when calling %s : %s' % (r.url, r.content))
             call['response'] = call['error']
-    else:
-        call['elapsedTime'] = call['deltaTime']
-        call['elapsedTimeCall'] = call['deltaTime']
-        call['status_code'] = 600
-        call['response'] = 'No Response'
-        if ts_name != None:
-            ts.time_inner(ts_name,call['error'])
 
-    if _currentConnectionName != 'ConnectionLess':
-        _updateThreadCall(call)
+    _updateThreadCall(call)
 
     return call['response']
 
-def requestWithConnection(action,  parameters = {}, method = 'get', data = {},headers = {},ts_name=None):
+def requestWithConnection(action,  parameters = {}, method = 'get', data = {},headers = {}):
     """
     Performs a request using the current connection as configured in the file. 
     """
     connection = getCurrentThreadConnection()
 
     if connection == None:
         raise ValueError('restClient current org is not set. Have you init restClient?')
 
     return requestRaw(  url=connection['instance_url'],
                         action=action, 
                         parameters=parameters , 
                         method = method , 
                         data = data ,
                         headers  =headers,
-                        access_token=connection['access_token'] if 'access_token' in connection else None,
-                        ts_name=ts_name)
+                        access_token=connection['access_token'] if 'access_token' in connection else None
+                        )
 
-def callAPI_multi(action,params={} , method = 'get', data = {},headers={},ts_name=None):
+def callAPI_multi(action,params={} , method = 'get', data = {},headers={}):
     done = False
 
    # parameters = params
     totalElepsedTime = datetime.timedelta(microseconds=0)
     totalCalls = 0
 
     while done==False:
-        call = requestWithConnection(action,parameters = params,method=method, data=data, headers=headers,ts_name=ts_name)
+        call = requestWithConnection(action,parameters = params,method=method, data=data, headers=headers)
 
-        totalElepsedTime = _thread_lastCall('elapsedTime') + totalElepsedTime
+        totalElepsedTime = lastThreadCall('elapsedTime') + totalElepsedTime
         totalCalls = totalCalls + 1
 
-        if  call == None or _thread_lastCall('status_code')>=300:
+        if  call == None or lastThreadCall('status_code')>=300:
             break
         
-        glog().debug(f"callAPI_multi: <{action}>  ts:{_thread_lastCall('elapsedTime')}") 
+        glog().debug(f"callAPI_multi: <{action}>  ts:{lastThreadCall('elapsedTime')}") 
 
         #For chainable integration procedures
-        if type(call) is dict and 'IPResult' in call and 'vlcStatus' in call['IPResult'] and call['IPResult']['vlcStatus'] == 'InProgress':
+        if 'IPResult' in call and 'vlcStatus' in call['IPResult'] and call['IPResult']['vlcStatus'] == 'InProgress':
             data['input'] = "{}"
-            data['options'] = json.loads(data['options'])
-            data['options']['vlcIPData'] = call['IPResult']['vlcIPData']
-            data['options'] = json.dumps(data['options'])
-            print(call['IPResult']['vlcIPData'])
+            data['options'] = json.dumps({
+                'vlcMessage':None,
+                'vlcIPData':call['IPResult']['vlcIPData'],
+                'vlcStatus':'InProgress'
+            })
+
 
-        elif type(call) is dict and 'nexttransaction' in call :
+        #For digital commerce
+        elif 'nexttransaction' in call and type(call)==dict:
             multiTransactionKey = call['nexttransaction']['rest']['params']['multiTransactionKey']
             data['multiTransactionKey'] = multiTransactionKey  
         else:
             done = True
 
-    lc = _thread_lastCall()
+    lc = lastThreadCall()
     lc['elapsedTime'] = totalElepsedTime
     lc['totalCalls'] = totalCalls    
     _updateThreadCall(lc)
 
     return call
 
 #def callAPI(action, parameters = {}, method = 'get', data = {}, headers={}):    
@@ -612,49 +518,46 @@
 # stores the request input and the reply into files in the output directory
 # The file name is provided by the calling function tree "debugFile(filename)", or calculated if not provided
 # the request add _req to the file name, while the reply adds _rep to the file name
 # The reply can be processed -> change the json to take out data, or compute additional fields before storing it
 #def callAPI_debug(action, parameters = {}, method = 'get', data = {}, headers={}):    
     return callAPI(action,parameters,method,data,headers)
 
-def callAPI(action, parameters = {}, method = 'get', data = {}, headers={},ts_name=None):    
-    call = callAPI_multi(action,parameters,method,data,headers,ts_name=ts_name)
+def callAPI(action, parameters = {}, method = 'get', data = {}, headers={}):    
+    call = callAPI_multi(action,parameters,method,data,headers)
     return call
 
 def callSave(logFileName,logRequest=False,logReply=True,timeStamp=False,responseProcessing=None,requestProcessing=None):
     if logRequest == False and logReply == False:
         return  
 
     now =f"{utils.datetimeString_now('%H:%M:%S')}--"
     if  timeStamp == False:
         now = ''
     filename = f"{now}{logFileName}"
-    request_filename = None
-    response_filename = None
 
-    lc = _thread_lastCall()
+    lc = lastThreadCall()
 
     if logRequest == True:
         fn = f'{filename}_req'
-        request_filename = writeFile(fn,lc['data'])
-        lc['requestFilePath'] = request_filename
+        filepath = writeFile(fn,lc['data'])
+        lc['requestFilePath'] = filepath
 
     if logReply == True:
         if requestProcessing != None:
             requestProcessing(lc['data'])
         
         fn = f'{filename}_res'
         try:
-            response_filename = writeFile(fn,lc['response'])
+            filepath = writeFile(fn,lc['response'])
         except Exception as e:
-            response_filename = writeFile(fn,str(lc['response']))  
-        lc['responseFilePath'] = response_filename
+            filepath = writeFile(fn,str(lc['response']))  
+        lc['responseFilePath'] = filepath
 
     _updateThreadCall(lc)
-    return request_filename,response_filename
 
 def writeFile(filename,content):
     connection = getCurrentThreadConnection()
 
     try:
         cont = content
         if (type(content) is dict or type(content) is list ):
@@ -664,9 +567,7 @@
 
     except ValueError as e:
         return file.writeFileinFolder(outputFolder(),filename,str(content))        
         
 def initTest():
     init("DEVNOSCAT2",configFolder="../input")     
 
-
-
```

### Comparing `InCli-0.0.82/InCli/SFAPI/utils.py` & `InCli-0.0.9/InCli/SFAPI/debugLogs.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,666 +1,566 @@
-from datetime import datetime,timedelta
-from logging import log
-import logging
-from . import objectUtil
-import inspect,simplejson
-import os,sys
-from posixpath import dirname
-import time
-#import pytz
-import subprocess,traceback
-
-
-CBLACK = "\033[0;30m"
-CRED = "\033[0;31m"
-CGREEN = "\033[0;32m"
-CBROWN = "\033[0;33m"
-CBLUE = "\033[0;34m"
-CPURPLE = "\033[0;35m"
-CCYAN = "\033[0;36m"
-CLIGHT_GRAY = "\033[0;37m"
-CDARK_GRAY = "\033[1;30m"
-CLIGHT_RED = "\033[1;31m"
-CLIGHT_GREEN = "\033[1;32m"
-CYELLOW = "\033[1;33m"
-CLIGHT_BLUE = "\033[1;34m"
-CLIGHT_PURPLE = "\033[1;35m"
-CLIGHT_CYAN = "\033[1;36m"
-CLIGHT_WHITE = "\033[1;37m"
-CWHITE = '\33[37m'
-CBOLD = "\033[1m"
-CFAINT = "\033[2m"
-CITALIC = "\033[3m"
-CUNDERLINE = "\033[4m"
-CBLINK = "\033[5m"
-CNEGATIVE = "\033[7m"
-CCROSSED = "\033[9m"
-CEND = "\033[0m"
-
-CBGBLUE = "\033[104m"
-
-#https://stackoverflow.com/questions/287871/how-do-i-print-colored-text-to-the-terminal
-#----------------------------------------------------------------------------------------------------
-def stringifyUrlParameters(parameters,exclude,initSeparator='?'):
-  isFirst = True
-
-  ret = ''
-  for name in parameters:
-    if name in exclude:
-      continue
-    if(parameters[name] == None):
-      continue
-    separator = initSeparator if isFirst == True else '&'
-    value = parameters[name]
-    if isinstance(value, str) == False:
-      value = simplejson.dumps(value)
-    paramStr = f'{separator}{name}={value}'
-    ret = ret + paramStr
-    isFirst = False
-
-  return ret
-
-def executeCommand(command):
-    is_windows = sys.platform.startswith('win')
-    if is_windows == True:
-        list_files = subprocess.run(command,capture_output=True,text=True,shell=True)
-    else:
-        list_files = subprocess.run(command,capture_output=True,text=True)
+from . import restClient,query,digitalCommerceUtil,file,utils,objectUtil
+import simplejson,logging
+
+def queryLogRecords(logUserId=None,limit=50):
+    whereUSer = f" where logUserId='{logUserId}' " if logUserId is not None else ''
+
+    call = query.query(f"Select Id,LogUserId,LogLength,LastModifiedDate,Request,Operation,Application,Status,DurationMilliseconds,StartTime,Location,RequestIdentifier FROM ApexLog  {whereUSer} order by LastModifiedDate desc limit {limit}")
+    return call
+
+def queryLogData(logId):
+#    log = query.queryRecords(f"Select fields(all) FROM ApexLog where Id ='{logId}' limit 1")
+    log = query.queryRecords(f"Select Id,LogUserId,LogLength,LastModifiedDate,Request,Operation,Application,Status,DurationMilliseconds,StartTime,Location,RequestIdentifier FROM ApexLog where Id ='{logId}' limit 1")
+
+    if log == None or len(log)==0:
+        utils.raiseException(errorCode='NO_LOG',error=f'The requested log <{logId}> cannot be found in the Server.',other=f"No record in ApexLogwith Id {logId}")    
+    log = log[0]
+    logLine = f"""LOGDATA:    Id: {log['Id']}   LogUserId: {log['LogUserId']}    Request: {log['Request']}  Operation: {utils.CGREEN}{log['Operation']}{utils.CEND}    lenght: {log['LogLength']}    duration: {log['DurationMilliseconds']}    startTime: {log['StartTime']} 
+LOGDATA:    app: {log['Application']}      status: {log['Status']}     location: {log['Location']}     requestIdentifier: {log['RequestIdentifier']}
+    """    
+
+    action = f"/services/data/v56.0/sobjects/ApexLog/{logId}/Body/"
+    callbody = restClient.callAPI(action)
+    callbody = logLine + callbody
+    return log,callbody
+
+def parseLog(logId=None,printLimits=True,userDebug=True,lastN=1,logUserId=None):
+    body = None
+
+    if logId is not None:
+        filename = f"{restClient.logFolder()}{logId}.log"
+        if file.exists(filename) == True:
+            body = file.read(filename)
+       #     body = None
+
+    if body is None:
+        if logId is None:
+            whereUSer = f" where logUserId='{logUserId}' " if logUserId is not None else ''
+            logIds = query.queryFieldList(f"Select Id FROM ApexLog {whereUSer} order by LastModifiedDate desc limit {lastN}")
+            if logIds == None or len(logIds)==0:
+                utils.raiseException(errorCode='NO_LOG',error=f'No logs can be found. ')
+            for logId in logIds:
+                print()
+                print(f"Parsing log Id {logId}")
+                parseLog(logId)
+            #    input("Click for next")
+            return  
+        else:
+            logRecord,body = queryLogData(logId)
 
-    print(f"{CFAINT}{list_files.stderr}{CEND}")
-    if "ERROR" in list_files.stderr:
-        error = list_files.stderr.split('ERROR')[1]
-        raiseException("SFDXError",f"ERROR{error}")
-    return list_files
-
-def execute_force_org_display(userName_or_orgAlias):
-    def getValue(field):
-        if field in line:
-            chunks = line.split(field)
-            val = chunks[1].strip()
-            obj[field]=val
-    output = executeCommand(["sfdx","force:org:display","-u", userName_or_orgAlias])
-    if output.stdout == '':
-        return False,None,output
-
-    lines = output.stdout.splitlines()
-
-    obj = {}
-    for line in lines:
-        getValue('Access Token')
-        getValue('Connected Status')
-        getValue('Instance Url')
-        getValue('Username')
-
-
-    return True,obj,output
-
-def executeCommandParse(command):
-    output = executeCommand(command)
-
-    if output.stdout == '':
-        return False,output
-
-    obj = {}
-
-    sl = output.stdout.splitlines()
-    namesline = sl[1]
-    lenLine = sl[2]
-    lenLines = lenLine.split(' ')
-    ll =[0]
-    ll = ll+[len(lenline)+2 for lenline in lenLines if lenline!='']
-    ll[-1] = ll[-1]-2
-
-    pos = []
-    position = 0
-    for l in ll:
-        position = position + l
-        pos.append(position)
-
-
-    names = []
-    for x in range(len(pos)-1):
-        name = namesline[pos[x]:pos[x+1]].strip()
-      #  print(namesline[pos[x]:pos[x+1]])
-        if name == '':
-            name = f"{x}"
-        names.append(name)
-
-    objs =[]
-    for y in range(3,len(sl)-1):
-        obj = {}
-        objs.append(obj)
-        for x in range(len(pos)-1):
-            value = sl[y][pos[x]:pos[x+1]].strip()
-            obj[names[x]] = value
-
-    return True,objs
-#----------------------------------------------------------------------------------------------------
-def extendedField(field):
-    """
-    An extended field is a field defined as "field:value"
-    returns a json containing {'field':field,'value':value}
-    If the parameter is just a value, the field is set to Id  'value' --> 'Id:value'
-    """
-    if field is None:
-        return None
-
-    sp = field.split(':')
-    if len(sp) == 1:
-        return {
-            'field':'Id',
-            'value':sp[0]
+    if body == None or len(body)==0:
+        utils.raiseException(errorCode='NO_LOG',error=f'The requested log <{logId}> cannot be found. ')
+    filename = f"{restClient.logFolder()}{logId}.log"
+
+    file.write(filename,body)
+    parse(body,printLimits=printLimits,userDebug=userDebug)
+
+def printLogs(logUserId=None,limit=50):
+    logs = queryLogRecords(logUserId,limit=limit)
+    logs = utils.deleteNulls(logs,delSystemFields=False)
+    utils.printFormated(logs)
+
+def delta(obj,field):
+    return obj[field][1] - obj[field][0] if len(obj[field]) > 1 else 0
+
+def setTimes(line,obj=None,field=None,value=None,chunkNum=None,type=None):
+    def addList(obj,field,val):
+        if field in obj:
+            obj[field].append(val)
+        else:
+            obj[field] = [val]
+
+    chunks = line.split('|')
+
+    if obj == None:
+        obj = {
+            'type' : type,
+            'ident' : _context['ident'],
+            'exception' :False
         }
-    return {
-        'field':sp[0],
-        'value':sp[1]
-    }
-#----------------------------------------------------------------------------------------------------
-class InCliError(Exception):
-    pass
-
-def exception_2_InCliException(exception):
-  #  aa = inspect.stack()[2]
-
-    error = {
-        'errorCode':'CODE',
-        'error':exception.args[0]
-    }   
-    error['json'] = message = simplejson.dumps(error, indent=2, ensure_ascii=False)
-#    print(traceback.format_exc())
-    return InCliError(error)
-
-def raiseException(errorCode,error,module=None,other=None):
-    aa = inspect.stack()[1]
-    error = {
-        'errorCode':errorCode,
-        'error':error,
-        'module':f"{aa[1].split('/')[-1]}  {aa[3]}  {aa[2]}",
+       
+        if len(chunks)>3:
+            obj['Id'] = chunks[3]
+
+    addList(obj,'lines',line)
+    addList(obj,'CPUTime',_context['DEF:CPU time'])
+    addList(obj,'SOQLQueries',_context['DEF:SOQL queries'])
+    addList(obj,'cmtCPUTime',_context['CMT:CPU time'])
+    addList(obj,'cmtSOQLQueries',_context['CMT:SOQL queries'])
+    addList(obj,'totalQueries',_context['totalQueries'])
+    addList(obj,'time',chunks[0].split(' ')[0])
+    addList(obj,'timeStamp',int ((chunks[0].split('(')[1]).split(')')[0]))
+
+    if _context['exception'] == True and obj['exception'] == False:
+        obj['exception'] = True
+        _context['exception'] = False
+
+    if obj['type'] is None:
+        print()
+
+    if field is not None:
+        obj[field] = chunks[chunkNum] if value is None else value
+
+    if _context['timeZero'] == 0:
+        _context['timeZero'] = obj['timeStamp'][0]
+
+    obj['elapsedTime'] = obj[f'timeStamp'][0] - _context['timeZero']
+
+    return obj
+
+_context = {
+    'totalQueries' : 0,
+    'timeZero':0,
+    'ident':0,
+    'DEF:SOQL queries' : 0,
+    'DEF:CPU time' : 0,
+    'CMT:SOQL queries' : 0,
+    'CMT:CPU time' : 0,
+    "exception":False
+}
+
+#######################################################################
+def resetContext():
+    _context['totalQueries'] = 0
+    _context['timeZero'] = 0
+    _context['ident'] = 0
+    _context['DEF:SOQL queries'] = 0
+    _context['DEF:CPU time']=0
+    _context['CMT:SOQL queries'] = 0
+    _context['CMT:CPU time']=0
+    _context['exception'] = False
+    _context['previousElapsedTime'] = 0
+    _context['previousCPUTime'] = 0
+    _context['previousIsLimit'] = False
+    _context['prevTimes'] = {
+        "0":[0,0]
     }
-    if other is not None:
-        error['other'] = other
+    _context['firstLineIn'] = True
+    _context['firstLineOut'] = True
+
     
-    error['json'] = message = simplejson.dumps(error, indent=2, ensure_ascii=False)
 
-    raise InCliError(error)
+def parse(log,printLimits=True,userDebug=True):
+   # log = file.read(filepath=filepath)
+    _context['printLimits'] = printLimits
+    _context['userDebug'] = userDebug
 
-def to_CliError(e):
-    if type(e) == InCliError: return e
-    er = {
-        'errorCode':'',
-        'error':'',
-        'module':''
-    }
-    er['error'] = e.args[0]['error'] if 'error' in e.args[0] else e.args[0]
-    er['errorCode'] = e.args[0]['errorCode'] if 'errorCode' in e.args[0] else ''
+    lines = log.splitlines()
 
-    return InCliError(er)
+    ident = 0
 
-def printException(exception):
-    print()
-    print(type(exception).__name__)
-    if type(exception) == InCliError:
-        _str = exception.args[0]['json']
-    else:
-        error = {
-            "errorCode":type(exception).__name__,
-            "error":str(exception)
-        }
-        _str = simplejson.dumps(error, indent=2, ensure_ascii=False)
-    logging.error(_str)
+    SOQL = {}
+
+    #totalQueries = 0
+
+    methodsList = []
+    constructorList = []
+    codeUnitsList = []
+    constructorList = []
+    dmlList=[]
+    limits = None
+
+    exceptionDict = None
+
+    limitsDict = {}
+
+    #workflow = {}
+
+    debugList = []
+    multiLine = None #for multiline commands
+
+    resetContext()
 
-def print_json(obj,filename=None):
-   # input_data = simplejson.loads(obj)
-    json_formatted_str = simplejson.dumps(obj, indent=2, ensure_ascii=False)
-
-    if filename != None:
-        original_stdout = sys.stdout
-        _filename = f"{filename}.json"
-        with open(_filename, 'w') as f:
-            sys.stdout = f 
-            print(json_formatted_str)
-            sys.stdout = original_stdout 
-            print()
-            print(f"   File {_filename} created.")
-    else:  
-        print(json_formatted_str)
-#----------------------------------------------------------------------------------------------------
-
-def throwOrLog(message,raiseEx=True,dumps=False):
-    """
-    if raiseEx is True, it raises an error. IF not logs the error. 
-    - message: the error messages. Can be a dictionary
-    - raiseEx: boolean
-    """
-    if dumps == True:
-        message = simplejson.dumps(message, indent=2)
-
-    if raiseEx == True:
-        logging.error(message)
-        raise ValueError(message)
-    else:
-        logging.info(message)
-        return None
-#----------------------------------------------------------------------------------------------------
-def printJSON(obj,delNull=False):
-    if delNull == True:
-        obj = deleteNulls(obj)
-    d = simplejson.dumps(obj, indent=2)
-    logging.debug(d)
     print()
 
-def deleteNulls(obj,systemFields=True,nulls=True,delAttributes=True):
-    systemFields= ['OwnerId','IsDeleted','CreatedDate','CreatedById','LastModifiedDate','LastModifiedById','LastViewedDate','LastReferencedDate','SystemModstamp','attributes']
-  #  if systemFields == False:
-  #      systemFields = True
-  #      systemFields = ['attributes']
-
-    if systemFields == True and nulls == True:
-        return obj
-    if 'records' in obj:
-        obj = obj['records']
-    if type(obj) is list:
-        res = []
-        for ob in obj:
-            res.append(deleteNulls(ob,systemFields,nulls))
-        return res
-
-    res = {}
-    for key in obj.keys():
-        if systemFields == False:
-            if key in systemFields:
+    for num,line in enumerate(lines):
+        chunks = line.split('|')
+
+        if _context['firstLineIn'] == True:
+            if 'LOGDATA:' in line:
+                print(line)
                 continue
-        if delAttributes == True:
-            if key in ['attributes']:
+            else:
+                _context['firstLineIn'] = False
+                levels = line.strip().split(' ')[1].replace(',','=').replace(';','  ')
+                print(levels)
+                print()
                 continue
-        if type(obj[key]) is dict:
-            res[key] = deleteNulls(obj[key],systemFields,nulls)
-        else:
-            if obj[key] is None and nulls is False:
+
+        if len(chunks)>1 and chunks[1] in ['HEAP_ALLOCATE','STATEMENT_EXECUTE','USER_INFO','VARIABLE_SCOPE_BEGIN']:
+            continue
+
+        if '|SYSTEM_MODE_EXIT|' in line:
+            nop=1
+
+        if '|USER_INFO|' in line:
+            setTimes(line)
+
+        if '|' in line:   #This is a new line always. 
+            multiLine = None
+        
+        if exceptionDict is not None:
+            if multiLine != 'EXCEPTION':   #This is a new line without the exeption
+                debugList.append(exceptionDict.copy())
+                exceptionDict = None
+                multiLine = None
+            else:
+                if line != '':
+                    exceptionDict['line'] = exceptionDict['line'] + line
+        if '|EXCEPTION_THROWN|' in line or 'FATAL_ERROR' in line:
+            exceptionDict = {
+                'line': line,
+                'type': 'EXCEPTION'
+            }
+            _context['exception'] = True
+            multiLine = 'EXCEPTION'
+
+        if '|VARIABLE_ASSIGNMENT|' in line:
+            if len(chunks) >= 5:
+                if 'ExecutionException' in chunks[4]:
+                    obj = setTimes(line,type='VAR_ASSIGN')
+                    obj['type'] = 'VAR_ASSIGN'
+                    obj['subType'] = 'EXCEPTION'
+                    obj['string'] = chunks[4]
+                    obj['apexline'] = chunks[2][1:-1] if chunks[2]!='[EXTERNAL]' else 'EX'
+
+                    debugList.append(obj)
+ 
+        if '|LIMIT_USAGE|' in line:
+            if '|SOQL|' in line:
+                _context[f'DEF:SOQL queries'] = chunks[4]
+
+        if '|LIMIT_USAGE_FOR_NS|' in line:
+            limits = chunks[2]
+            if limits == '(default)':
+                limits = 'DEF:'
+            elif limits == 'vlocity_cmt':
+                limits = 'CMT:'
+            else:
+                limits = f"{limits}:"
+
+            limitsDict = setTimes(line,type='LIMITS')
+            limitsDict['limitType'] = limits
+
+        if limits is not None and line == ' ':
+            limits = None
+        
+        if limits is not None:
+            chunks = line.split(' ')
+            if 'SOQL queries' in line:
+                _context[f'{limits}SOQL queries'] = chunks[6]
+            if 'CPU time' in line:
+                _context[f'{limits}CPU time'] = chunks[5]
+
+        if limits is not None and line =='':
+            setTimes(limitsDict['lines'][0],limitsDict)
+            s = f"limits-{limits.lower()} {limitsDict['time'][0]}"
+            if _context['printLimits'] == True:
+                debugList.append(limitsDict)
+            limits = None   
+
+
+        if '*** getCpuTime() ***' in line:
+            chs = chunks[4].split(' ')
+            _context[f'DEF:CPU time'] = chs[4]
+        if '*** getQueries() ***' in line:
+            chs = chunks[4].split(' ')
+            _context[f'DEF:SOQL queries'] = chs[4]
+
+        if '|USER_DEBUG|' in line:
+            multiLine = 'DEBUG'
+        if multiLine == 'DEBUG':
+            if '|' in line:
+                obj = setTimes(line,type='DEBUG')
+                obj['type'] = 'DEBUG'
+                obj['subType'] = chunks[3]
+                obj['string'] = chunks[4]
+                obj['apexline'] = chunks[2][1:-1]
+
+            else:
+                obj = debugList[-1].copy()
+                obj['string'] = line
+        #    if _context['userDebug'] == True:
+            debugList.append(obj)
+
+    
+        if '|WF_RULE_EVAL' in line:
+            if 'BEGIN' in chunks[1]:
+                workflow = setTimes(line,field='method',value=chunks[2])
+
+            if 'END' in chunks[1]:
+                setTimes(line,workflow)
+        if '|WF_ACTION|' in line:
+            workflow['action'] = chunks[2]
+
+        if '|CONSTRUCTOR_' in line:
+            if 'ENTRY' in chunks[1]:      
+                obj = setTimes(line,field='method',value=chunks[5],type='CONSTRUCTOR')
+                constructorList.append(obj)
+                increaseIdent()    
+                debugList.append(obj)
+
+
+            if 'EXIT' in chunks[1]:    
+                decreaseIdent()
+                obj = delFromList(constructorList,'method',chunks[5])
+                setTimes(line,obj)   
+         
+        if '|CODE_UNIT_' in line:
+            if 'STARTED' in chunks[1]:
+                obj = setTimes(line,type='CODE_UNIT')
+                obj['trigger'] = chunks[3]  if len(chunks)>4 else ''
+                obj['method'] = chunks[4] if len(chunks)>4 else chunks[3]
+                codeUnitsList.append(obj)
+                increaseIdent()
+                debugList.append(obj)
+
+            if 'FINISHED' in chunks[1]:
+                decreaseIdent()
+                obj = delFromList(codeUnitsList,'method',chunks[2])
+                setTimes(line,obj)
+
+        if '|DML_' in line:
+            if 'BEGIN' in chunks[1]:
+                obj = setTimes(line,type="DML")
+                obj['OP'] = chunks[3]
+                obj['Type'] = chunks[4]
+                obj['Id'] = chunks[2]
+                obj['apexline'] = chunks[2][1:-1]
+                dmlList.append(obj)
+                increaseIdent()
+                debugList.append(obj)
+
+            if 'END' in chunks[1]:
+                obj = delFromList(dmlList,'Id',chunks[2])
+                setTimes(line,obj)
+                decreaseIdent()
+
+        if 'SOQL_EXECUTE_' in line:
+            if 'BEGIN' in chunks[1]:
+                SOQL = setTimes(line,field='query',value=chunks[4],type="SOQL")
+                SOQL['object'] = chunks[4].lower().split(' from ')[1].strip().split(' ')[0]
+                SOQL['apexline'] = chunks[2][1:-1]
+
+                a= 1
+                debugList.append(SOQL)
+
+            if 'END' in chunks[1]:
+                _context['totalQueries'] = _context['totalQueries'] + 1
+                setTimes(line,SOQL)
+                SOQL['rows'] = chunks[3].split(':')[1]
+                if len(SOQL['query']) > 180:
+                    if 'from' in SOQL['query'].lower():
+                        SOQL['query'] = SOQL['query'].replace('from',"FROM")
+                        SOQL['query'] = SOQL['query'].replace('From',"FROM")
+
+                    SOQL['query'] = f"{SOQL['query'].split(' ')[0]} ... FROM {SOQL['query'].split('FROM')[1]}"
+
+        if '|METHOD_' in line:
+            if len(chunks)<4:
+                print(line)
                 continue
-            res[key] = obj[key]
-    return res
 
-def printFormated(records,fieldsString=None,rename=None,exclude=None,checkNumber=False,separator=':',print_renames=True):
-    """
-    - fieldsString: format field%name:field2%name2:field3
-        field is the field in the obj. Name is how it will be printed (the short version). 
-        name3 is equivalent to field3-field3
-    - rename : field%name:field2%name2
-    """
-    if records is None or len(records) == 0:
-        print('No records to print')
-        return
+            operation = chunks[1]
+            method = getMethod(line)
+
+            if 'ENTRY' in operation:
+                obj = setTimes(line,type='METHOD')
+                obj['method'] = method
+                obj['apexline'] = chunks[2][1:-1] if chunks[2]!='[EXTERNAL]' else 'EX'
+                debugList.append(obj)
+
+                if '.getInstance' in method:
+                    pass
+                else:
+                    methodsList.append(obj)
+                    increaseIdent()
+            else:
+                obj = delFromList(methodsList,'method',method)
+
+                if obj is not None:
+                    decreaseIdent()
+                    setTimes(line,obj)
+
+                else:
+                    obj = setTimes(line,type='NO_ENTRY')
 
-    if type(records) is dict:
-        records = [records]
+    for d in debugList:
+        printParsedLog(d)
     print()
-    if 'records' in records:
-        records = records['records']
 
-    if fieldsString == None:
-        fieldsString = separator.join(records[0].keys())
-    fields = fieldsString.split(separator)
-    if exclude != None:
-        fields2 = [field for field in fields if field not in exclude.split(separator)]
-        fields = fields2
-
-    _renames = {}
-    if rename != None:
-        renames = rename.split(':')
-        for ren in renames:
-            chunks = ren.split('%')
-            _renames[chunks[0]] = chunks[1]
-            if print_renames: print( CFAINT +  f"Column {chunks[0]} as {chunks[1]}" +CEND)
+
+ #  utils.printFormated(logsList)
+def getMethod(line):
+    chunks = line.split('|')
+    if len(chunks) == 4:
+        method = chunks[3]
+    else:
+        method = chunks[4]
+    if '(' in method:
+        method = method.split('(')[0]
+    return method
+
+def getTime(line):
+    chunks = line.split('|')
+    return chunks[0].split(' ')[0]
+
+def getTimeStamp(line):
+    chunks = line.split('|')
+    return int ((chunks[0].split('(')[1]).split(')')[0])
+
+def increaseIdent():
+    _context['ident'] = _context['ident'] + 1
+
+def decreaseIdent():
+    _context['ident'] = _context['ident'] - 1
+
+def emptyString(size,char=' ',ident=None):
+    str = ''
+    if ident is None:
+        ident = _context['ident']
+    length = ident * size
+    for x in range(length):
+        str = str + char  
+    return str     
+
+def rootString():
+    str = ''
+    length = _context['ident'] 
+    if length == 0:
+        return ''
+    for x in range(length-1):
+        str = str + '⎮'
+    str = str + '⌈' 
+
+    return str     
+
+bufVal=''
+buffer=''
+previousEnd = False
+
+prevTS = 0
+
+
+def printParsedLog(d):
+
+    CEND    = '\33[0m'
+    CRED    = '\33[31m'
+    CWHITE  = '\33[37m'
+    CBLUE   = '\33[34m'
+    CGREEN  = '\33[32m'
+    CYELLOW = '\33[33m'
+
+    Cinit = CWHITE
+
+    _plimit=' '
+    if d['type'] == 'EXCEPTION':
+        print(CRED + d['line'] + CEND)
+        return
+
+    if d['type'] == 'LIMITS':
+        _context['previousIsLimit'] = True
+        return
+    if _context['previousIsLimit'] == True:
+        _plimit = '*' 
+        _context['previousIsLimit'] = False
+
+    level = d['ident']
+
+    _type = d['type']
+    if _type == 'DEBUG':
+        _type = f"{d['type']}-{d['subType']}"
+        Cinit = CRED if d['subType'] == 'ERROR' else CGREEN
+
+    if _type == 'VAR_ASSIGN':
+        if d['subType'] == 'EXCEPTION':
+            Cinit = CRED
+        else:
+            return
+
+    if d['type'] == 'SOQL':
+        Cinit = CBLUE
+    if d['type'] == 'DML':
+        Cinit =  CYELLOW
+
+    i = f"{emptyString(1,' ',level)}."
+    i= level
+    identation = f"{emptyString(3,' ',level)}"
+
+    val = d['query'] if d['type'] == 'SOQL' else ''
+    val = d['method'] if d['type'] == 'METHOD' else val
+    val = d['method'] if d['type'] == 'CONSTRUCTOR' else val
+    val = d['method'] if d['type'] == 'CODE_UNIT' else val
+    val = f"{d['OP']} {d['Type']}" if d['type'] == 'DML' else val
+    val = f"{d['limitType']} " if d['type'] == 'LIMITS' else val
+    val = d['string'] if d['type'] == 'DEBUG' else val
+    val = d['string'] if d['type'] == 'VAR_ASSIGN' else val
+
+    if val == '':
         print()
     
-    _fields = {}
-    for field in fields:
-        v = {}
-        v['obj_name'] = field
-        v['print_name'] = _renames[field] if field in _renames else field
-        v['size'] = len(v['print_name'])
-        _fields[field] = v
-
-    #calculate _fileds size based in value.
-    for record in records:
-        for key in _fields.keys():
-            size = 0
-            value = objectUtil.getField(record,key,'.')
-            if value is not None:
-                size = len(str(value))
-                if size > _fields[key]['size']:
-                    _fields[key]['size'] = size
-
-    #print header
-    spacing = 2    
-    line = ''
-    for key in _fields.keys():
-        if key == "__color__":
-            continue
-        field = _fields[key]        
-        value = field['print_name']
+    val = Cinit +f"{identation}{val}"
 
-        line =  f"{line}{value:{int(field['size']+spacing)}}" 
-    print(CUNDERLINE+line+CEND)
+    _apexline = d['apexline'] if 'apexline' in d else ''
 
-    for record in records:
-        line = ''
-        for key in _fields.keys():
-            field = _fields[key]    
+    _totalQueriesTrace = delta(d,'totalQueries') 
+    spacer = '_' if d['type'] == 'SOQL' else '.'
+    _totalQueriesTrace = f"{level:2}:{emptyString(1,spacer,level)}{_totalQueriesTrace}" if _totalQueriesTrace >0 else ' '
 
-            if key == "__color__":
-                continue
+    _cpuTime0 = int(d['CPUTime'][0])
+    _cpuTime1 = int(d['CPUTime'][1]) if len(d['CPUTime']) >1 else ''
+    _timeStamp1 = d['timeStamp'][1] if len(d['timeStamp'])>1 else d['timeStamp'][0]
 
-            val = objectUtil.getField(record,key,'.')
-            val = '' if val is None else str(val) 
-            padding = int(field['size']+spacing)
- #           print(f"{padding}  {field['size']}")
-            if checkNumber and _isInt(val):
-                line = f"{line}{int(val):>{padding-1}} "
-            elif checkNumber and _isFloat(val):
-                line = f"{line}{float(val):>{padding-1}.2f} "
-            else:
-                line = f"{line}{val:{padding}}"
-        if '__color__' in record:
-            if record['__color__'] != '':
-                line = record['__color__'] + line + CEND
-
-        print(line)
-
-def _isInt(s):
-    try:
-        int(s)
-        return True
-    except ValueError:
-        return False
-
-def _isFloat(s):
-    try:
-        float(s)
-        return True
-    except ValueError:
-        return False
-
-def datetimeString_now(format = '%Y-%m-%dT%H:%M:%S'):
-    ts = time.time()
-    dt = datetime.fromtimestamp(ts).strftime(format)
-    return dt
-
-def datetimeString_to_timestamp(str,format=None):
-    if str == None: 
-        return None
-    if format == None:
-        format = '%Y-%m-%dT%H:%M:%S.%f%z'
-    #str = '2021-08-31T22:23:24.000+0000'   '%Y-%m-%dT%H:%M:%S.%f%z'
-    dt = datetime.strptime(str,format)
-    ts = datetime.timestamp(dt) * 1000
-    
-    return int(ts)
+    _totalQueries0 = d['totalQueries'][0]
+    _totalQueries1 = d['totalQueries'][1] if len(d['SOQLQueries']) >1 else _totalQueries0
+    _totalQueriesD = _totalQueries1-_totalQueries0
 
-def today_date(format="%Y-%m-%d"):
-    today = datetime.today()
-    return today.strftime(format)  
-
-def datetimestr_around(str,minutes,format = '%Y-%m-%dT%H:%M:%S'):
-    dt = datetime.strptime(str,format)
-    dt_before = dt - timedelta(minutes=minutes) 
-    dt_after = dt + timedelta(minutes=minutes) 
-    return dt_before.strftime(format),dt_after.strftime(format)
-
-def future_date(years=None,days=None,minutes=None,format="%Y-%m-%d"):
-    today = datetime.today()
-    if years!=None:  future = today.replace(year=today.year + years)
-    if days!=None:    future = today.replace(day=today.day + days)
-    return future.strftime(format)  
-
-def callerPythonFileFolder():
-    caller_filepath = inspect.currentframe().f_back.f_code.co_filename
-    caller_filefolder = os.path.dirname(caller_filepath)
-    if caller_filefolder.endswith('SFAPI'):
-        caller_filefolder = dirname(caller_filefolder)
-    return caller_filefolder
-
-def getEntryDirectory():
-    return sys.path[0]
-
-def currentFilePath():
-    frame = inspect.stack()[1]
-    filename = frame[0].f_code.co_filename
-    dirname = os.path.dirname(filename)
-    return dirname
-
-def getFieldc(var,field,onlyOne=True):
-    return Id(var,field=field,onlyOne=True)
-
-def getRecord(obj):
-
-    if 'records' in obj:
-        return getRecord(obj['records'])
-    if 'result' in obj:
-        return getRecord(obj['result'])
-    if 'fields' in obj:
-        return getRecord(obj['fields'])
-    return obj
+    _cpuPrevD = _cpuTime0 - int(_context['previousCPUTime'])
 
-def Id(var):
-    return selectField(var,field='Id',onlyOne=True)
+    _l = f"{level}"
+    prev = _context['prevTimes'][_l][1] if _l in _context['prevTimes'] else _context['prevTimes'][f"{level-1}"][0]
+    _elapsedPrevD = d['timeStamp'][0] - prev
+    _context['prevTimes'][_l] = [d['timeStamp'][0],_timeStamp1]
+    _elapsedPrevD = ms(_elapsedPrevD)
 
-def selectField(var,field='Id',onlyOne=True):
-    if type(var) is str:
-        return var
-    if (type(var) is dict):
-        if field in var:
-            if 'value' in var[field]:
-                return var[field]['value']
-            return var[field]
-
-        if 'records' in var:
-            return selectField(var['records'],field,onlyOne)
-        if 'result' in var:
-            return selectField(var['result'],field,onlyOne)
-        if 'fields' in var:
-            return selectField(var['fields'],field,onlyOne)
-    if type(var) == list:
-        if onlyOne == True:
-            if len(var)>1:
-                logging.warn(f"There is more than 1 element in the list {len(var)}, returning Id from first one")
-            return selectField(var[0],field,onlyOne)
-        else:
-            _ids = []
-            i=0
-            while i<len(var):
-                _ids.append(selectField(var[i],field,onlyOne))
-                i = i + 1
-            return _ids
-
-def Obj(var,onlyOne=True):
-    if (type(var) is dict):
-        if 'records' in var:
-            return Obj(var['records'],onlyOne)
-        else :
-            return var
-
-    if type(var) == list:
-        if onlyOne == True:
-            if len(var)>1:
-                logging.warn(f"There is more than 1 element in the list {len(var)}, returning Id from first one")
-            return Obj(var[0],onlyOne)
-        else:
-            _objs = []
-            i=0
-            while i<len(var):
-                _objs.append(Obj(var[i],onlyOne))
-                i = i + 1
-            return _objs
-
-def computeTimes(call,name,times,_type=None):
-    global _counter
-
-    debugTimes = {}
-
-    time = call['elapsedTime']
-    sec = time.microseconds + time.seconds * 1000000 
-    times[name]=sec
-
-    debugTimes['ElapsedCall'] = sec
-
-    if 'debugIP' == _type and 'IPResult' in call:
-
-        if 'debugLog' in call['IPResult']:
-            for key in call['IPResult']:
-                if key.endswith('Debug'):
-                    debugTimes[f'{key}_ElapsedTime'] = call['IPResult'][key]['deltaTime'] * 1000
-                    debugTimes[f'{key}_ElapsedTimeCPU'] = call['IPResult'][key]['ElapsedTimeCPU'] * 1000
-
-        if 'elapsedTimeActual' in call['IPResult']:
-            debugTimes['elapsedTimeActual'] = call['IPResult']['elapsedTimeActual'] * 1000
-        if 'elapsedTimeCPU' in call['IPResult']:
-            debugTimes['elapsedTimeCPU'] = call['IPResult']['elapsedTimeCPU'] * 1000
-            #print(f" {_counter} , {sec}  , {elapsedTimeActual}  , {sec-timeActual} ,{apigeeTime}")
-            #_counter = _counter + 1
-            #return
-        print(debugTimes)
-
-    print (sec)
-    return debugTimes
-
-def _is_match(objs,x,y,field):
-    ox = objs[x]
-    oy = objs[y]
-
-    if 'ident' not in ox: return False
-    if 'ident' not in oy: return False
-
-    if ox['ident'] != oy['ident'] : return False
-
-    if ox[field] != oy[field]:  return False
-    return True
-def _is_next_link(objs,field,chain_start,link_lenght,posible_link_start):
-    for z in range(0,link_lenght):
-        if posible_link_start+z >= len(objs): return False
-        if _is_match(objs,chain_start+z,posible_link_start+z,field) == False: return False
-
-    return True
-
-def get_all_loops(objs,field):
-
-    all_loops = []
-    _all_loops = []
-
-    lastX = 0
-
-    for x,val in enumerate(objs):
-        if x < lastX:    continue
-        if objs[x]['type'] == 'SOQL':continue
-        loop_lenght = None
-        lastDelta = 0
-        loop = []
+    _exp = "!" if d['exception'] == True else ''
 
-        max = 30
-        is_loop = False
-        
-        ox = objs[x]
-        if 'timeStamp' in ox and ox['timeStamp'][0] == 10189843723:
-            a=1
-        for y in range(x+1,len(objs)):
-            if is_loop == False and y-x>=max:
-                break
-            oy = objs[y]
-            if 'ident' in ox and ox['ident'] > oy['ident']:
-                break        
-            #    print(f"{x}:{ox['output']} {y}:{oy['output']}")
-  
-            
-            if _is_match(objs,x,y,field):
-                chain_start = x
-                next_link_start = y
-                link_lenght = y-x
-                loop = []
-
-                while True:
-                    if _is_next_link(objs,field,chain_start,link_lenght,next_link_start):
-                        if len(loop) == 0: loop.append(x)
-                        loop.append(next_link_start)
-                        next_link_start = next_link_start + link_lenght
-                        lastX = next_link_start
-                    else:
-                        break
-                if len(loop) > 0:  
-                    all_loops.append(loop)
-                    break
-
-
-    return all_loops
-    print(all_loops)
-def get_all_loops1(objs,field):
-
-    all_loops = []
-    lastX = 0
-  #  if objs==None:
-  #      a=1
- #   lenObj = len(objs)
-    for x,val in enumerate(objs):
-        if x <= lastX:    continue
-        loop_lenght = None
-        lastDelta = 0
-        loop = []
-   #     if 'output' not in objs[x]:
-   #         oo = objs[x]
-   #     objx = objs[x]['output']
-
-        max = 30
-        is_loop = False
-
-        for y in range(x+1,len(objs)):
-            if is_loop == False and y-x>=max:
-                break
-     #       if 'output' not in objs[y]:
-     #           oo = objs[y]
-     #       objy=objs[y]['output']
-
-     #       if field not in objs[y]:
-     #           _o = objs[y]
-            ox = objs[x]
-            oy = objs[y]
-            if _is_match(objs,x,y,field):
-          #  if 'ident' in objs[y] and 'ident' in objs[x] and objs[y]['ident'] == objs[x]['ident'] and objs[y][field] == objs[x][field]:
-      #          line = objs[y][field]
-                posible_link_start = x
-                posible_link_end = y
-                if y == 1445:
-                    a=1
-                if y == 1575:
-                    a=1
-                if loop_lenght == None:
-                    loop_lenght = y-x
-                    lastDelta = loop_lenght
-                else:   lastDelta = y - lastX
-                
-                is_loop = True
-                if lastDelta == loop_lenght:
-                    for z in range(0,loop_lenght):
-                        if y+z >= len(objs): is_loop=False
-                        elif objs[y+z][field] != objs[x+z][field]: is_loop = False
-
-                    if is_loop == False:   break
-                    if is_loop == True:
-                        if len(loop) == 0:   loop.append(y-loop_lenght)
-                        loop.append(y)
-                else:  break
-                if is_loop == True:     lastX = y 
-         #   else:
-         #       if is_loop:
-         #           is_loop = False
-         #           break
-        if len(loop) > 0:  all_loops.append(loop)
-
-    return all_loops
-def datetime_now_string(format = '%Y-%m-%dT%H:%M:%S%z',addMinutes=0,addDays=0):
-    tz2 = datetime.now().astimezone()
-    if addMinutes != 0:
-        tz2 = tz2 + timedelta(minutes = addMinutes)
-    if addDays != 0:
-        tz2 = tz2 + timedelta(days= addDays)
-    st = tz2.strftime(format)
+    _sql2 = d['SOQLQueries'][1] if len(d['SOQLQueries'])>1 else d['SOQLQueries'][0]
+    _sqlcmt2 = d['cmtSOQLQueries'][1] if len(d['cmtSOQLQueries'])>1 else d['cmtSOQLQueries'][0]
+
+    _context['previousCPUTime'] = _cpuTime0
+    _context['previousElapsedTime']  = d['elapsedTime']
+
+    if _context['firstLineOut'] == True:
+        print(f"{' ':15}|{'time(ms)':10}|{'elapsed':10}|{'time1(ns)':12}|{'time2(ns)':12}|{'ExecTime':10}|{'QueriesStack':15}|{'Qd':4}|{'Qt':4}|{'L':1}|{'cpuD':6}|{'CPUin':6}|{'CPUout':6}|{'Q':3}|{'Qcm':3}|{'type':12}|{'E':1}|{'al':4}{'':50}")
+        _context['firstLineOut'] = False
+
+    print(f"{i:15} {ms(d['elapsedTime']):10}|{_elapsedPrevD:8}|{d['timeStamp'][0]:12}|{_timeStamp1:12}|{ms(delta(d,'timeStamp')):10}|{_totalQueriesTrace:15}|{_totalQueriesD:4}|{_totalQueries1:4}|{_plimit:1}|{_cpuPrevD:6}|{_cpuTime0:6}|{_cpuTime1:6}|{_sql2:3}|{_sqlcmt2:3}|{_type:12}|{_exp:1}|{_apexline:>4}|{val[:150]:50}"+CEND)
+
+
+logsList = []
+def ms(val):
+    return f"{val/1000000:10.2f}"
+def printIdent(string,ident):
+    str = ''
+    for x in range(_context['ident'] * 3):
+        str = str + ' '
+    print(str + string)
+
+
+def delFromList(theList,field,value):
+    for i in range(len(theList)):
+        obj = theList[len(theList)-i-1]
+
+        if obj[field] == value:
+            theList.pop(len(theList)-i-1)
+            return obj
+
+    for i in range(len(theList)):
+        obj = theList[len(theList)-i-1]
+
+        if value in obj[field]:
+            theList.pop(len(theList)-i-1)
+            return obj
+
+    return None    
 
-    return st
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `InCli-0.0.82/LICENSE.txt` & `InCli-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `InCli-0.0.82/test/test_file.py` & `InCli-0.0.9/test/test_file.py`

 * *Files identical despite different names*

### Comparing `InCli-0.0.82/test/test_restClient.py` & `InCli-0.0.9/test/test_restClient.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         restClient.init("DEVNOSCAT2")   
         action = '/services/data'
 
         #Test  callAPI_debug 
         call = restClient.callAPI(action)
         self.assertTrue(len(call)>0)    
         restClient.callSave("testFile")
-        lc = restClient.lastCall()
+        lc = restClient.lastThreadCall()
 
         self.assertTrue('responseFilePath' in lc)
         fileContent = jsonFile.read(lc['responseFilePath'])
 
         self.assertEqual(call,fileContent)
 
         q = query.query(" select fields(all) from Account limit 1")
@@ -101,15 +101,15 @@
         a = [1]*100
 
         allTimes = []
         def doWork(a):
             action = '/services/data'
             call = restClient.callAPI(action)
             times= {
-                "elapsed":restClient.lastCall()
+                "elapsed":restClient.getlastThreadCallTime()
             } 
             allTimes.append(times)
 
         thread.processList(doWork,a,10)
 
         utils.printFormated(allTimes)
 
@@ -126,15 +126,15 @@
         except Exception as e:
             self.assertTrue(e.args[0]['errorCode'] ==  'ConnectionError')
             utils.printException(e)
 
         try:            
             restClient.init("uormaechea.devnoscat2@nos.pt")
             q = query.query(" select fields(all) from Order limit 1")
-            lc = restClient.lastCall()
+            lc = restClient.lastThreadCall()
             self.assertEqual(lc['status_code'],200)
             print(q)
 
         except Exception as e:
             self.assertEqual('This','Should not happen')
 
     def test_congifData(self):
```

