# Comparing `tmp/RolexReserver-1.0.2.tar.gz` & `tmp/RolexReserver-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RolexReserver-1.0.2.tar", last modified: Sun May 14 03:26:04 2023, max compression
+gzip compressed data, was "RolexReserver-1.0.3.tar", last modified: Tue May 23 13:03:31 2023, max compression
```

## Comparing `RolexReserver-1.0.2.tar` & `RolexReserver-1.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 03:26:04.169183 RolexReserver-1.0.2/
--rw-rw-rw-   0        0        0      887 2023-05-14 03:26:04.168183 RolexReserver-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       17 2023-05-09 13:04:12.000000 RolexReserver-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 03:26:04.145187 RolexReserver-1.0.2/RolexReserver/
-drwxrwxrwx   0        0        0        0 2023-05-14 03:26:04.153183 RolexReserver-1.0.2/RolexReserver/Getter/
-drwxrwxrwx   0        0        0        0 2023-05-14 03:26:04.154183 RolexReserver-1.0.2/RolexReserver/Getter/Base/
--rw-rw-rw-   0        0        0     1417 2023-05-09 13:09:11.000000 RolexReserver-1.0.2/RolexReserver/Getter/Base/baseGetter.py
--rw-rw-rw-   0        0        0     5964 2023-05-14 03:20:49.000000 RolexReserver-1.0.2/RolexReserver/Getter/getter_rolexReserve.py
-drwxrwxrwx   0        0        0        0 2023-05-14 03:26:04.166189 RolexReserver-1.0.2/RolexReserver/Library/
--rw-rw-rw-   0        0        0     4614 2023-05-14 03:20:49.000000 RolexReserver-1.0.2/RolexReserver/Library/rolexReserverConfig.py
--rw-rw-rw-   0        0        0      704 2023-05-13 05:47:49.000000 RolexReserver-1.0.2/RolexReserver/Library/rolexReserverConfiger.py
--rw-rw-rw-   0        0        0     1538 2023-05-10 13:23:34.000000 RolexReserver-1.0.2/RolexReserver/Library/rolexReserverController.py
--rw-rw-rw-   0        0        0      164 2023-05-09 12:52:25.000000 RolexReserver-1.0.2/RolexReserver/Library/rolexReserverDeclare.py
--rw-rw-rw-   0        0        0     2092 2023-01-06 13:54:01.000000 RolexReserver-1.0.2/RolexReserver/Library/rolexReserverException.py
--rw-rw-rw-   0        0        0      573 2023-05-09 13:01:02.000000 RolexReserver-1.0.2/RolexReserver/Library/rolexReserverGlobals.py
--rw-rw-rw-   0        0        0     4731 2023-05-09 13:01:02.000000 RolexReserver-1.0.2/RolexReserver/Library/rolexReserverMailer.py
--rw-rw-rw-   0        0        0      261 2023-05-14 03:23:19.000000 RolexReserver-1.0.2/RolexReserver/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 03:26:04.152187 RolexReserver-1.0.2/RolexReserver.egg-info/
--rw-rw-rw-   0        0        0      887 2023-05-14 03:26:04.000000 RolexReserver-1.0.2/RolexReserver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      638 2023-05-14 03:26:04.000000 RolexReserver-1.0.2/RolexReserver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 03:26:04.000000 RolexReserver-1.0.2/RolexReserver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      709 2023-05-14 03:26:04.000000 RolexReserver-1.0.2/RolexReserver.egg-info/requires.txt
--rw-rw-rw-   0        0        0      105 2023-05-14 03:26:04.000000 RolexReserver-1.0.2/RolexReserver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 03:26:04.169183 RolexReserver-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2523 2023-05-09 12:42:27.000000 RolexReserver-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 13:03:31.751072 RolexReserver-1.0.3/
+-rw-rw-rw-   0        0        0      887 2023-05-23 13:03:31.750072 RolexReserver-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2023-05-09 13:04:12.000000 RolexReserver-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 13:03:31.734072 RolexReserver-1.0.3/RolexReserver/
+drwxrwxrwx   0        0        0        0 2023-05-23 13:03:31.740070 RolexReserver-1.0.3/RolexReserver/Getter/
+drwxrwxrwx   0        0        0        0 2023-05-23 13:03:31.741071 RolexReserver-1.0.3/RolexReserver/Getter/Base/
+-rw-rw-rw-   0        0        0     1417 2023-05-09 13:09:11.000000 RolexReserver-1.0.3/RolexReserver/Getter/Base/baseGetter.py
+-rw-rw-rw-   0        0        0     5828 2023-05-22 10:11:15.000000 RolexReserver-1.0.3/RolexReserver/Getter/getter_rolexReserve.py
+drwxrwxrwx   0        0        0        0 2023-05-23 13:03:31.749074 RolexReserver-1.0.3/RolexReserver/Library/
+-rw-rw-rw-   0        0        0     4820 2023-05-20 08:30:17.000000 RolexReserver-1.0.3/RolexReserver/Library/rolexReserverConfig.py
+-rw-rw-rw-   0        0        0      704 2023-05-13 05:47:49.000000 RolexReserver-1.0.3/RolexReserver/Library/rolexReserverConfiger.py
+-rw-rw-rw-   0        0        0     1538 2023-05-10 13:23:34.000000 RolexReserver-1.0.3/RolexReserver/Library/rolexReserverController.py
+-rw-rw-rw-   0        0        0      164 2023-05-09 12:52:25.000000 RolexReserver-1.0.3/RolexReserver/Library/rolexReserverDeclare.py
+-rw-rw-rw-   0        0        0     2092 2023-01-06 13:54:01.000000 RolexReserver-1.0.3/RolexReserver/Library/rolexReserverException.py
+-rw-rw-rw-   0        0        0      573 2023-05-09 13:01:02.000000 RolexReserver-1.0.3/RolexReserver/Library/rolexReserverGlobals.py
+-rw-rw-rw-   0        0        0     4731 2023-05-09 13:01:02.000000 RolexReserver-1.0.3/RolexReserver/Library/rolexReserverMailer.py
+-rw-rw-rw-   0        0        0      261 2023-05-22 10:12:16.000000 RolexReserver-1.0.3/RolexReserver/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 13:03:31.739072 RolexReserver-1.0.3/RolexReserver.egg-info/
+-rw-rw-rw-   0        0        0      887 2023-05-23 13:03:31.000000 RolexReserver-1.0.3/RolexReserver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      638 2023-05-23 13:03:31.000000 RolexReserver-1.0.3/RolexReserver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 13:03:31.000000 RolexReserver-1.0.3/RolexReserver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      784 2023-05-23 13:03:31.000000 RolexReserver-1.0.3/RolexReserver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      105 2023-05-23 13:03:31.000000 RolexReserver-1.0.3/RolexReserver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 13:03:31.751072 RolexReserver-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2523 2023-05-09 12:42:27.000000 RolexReserver-1.0.3/setup.py
```

### Comparing `RolexReserver-1.0.2/PKG-INFO` & `RolexReserver-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RolexReserver
-Version: 1.0.2
+Version: 1.0.3
 Summary: RolexReserver Package
 Home-page: https://github.com/kaioman/RolexReserver.git
 Author: unchainworks
 Author-email: kajin0318@gmail.com
 License: BSD-3-Clause
 Keywords: RolexReserver
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `RolexReserver-1.0.2/RolexReserver/Getter/Base/baseGetter.py` & `RolexReserver-1.0.3/RolexReserver/Getter/Base/baseGetter.py`

 * *Files identical despite different names*

### Comparing `RolexReserver-1.0.2/RolexReserver/Getter/getter_rolexReserve.py` & `RolexReserver-1.0.3/RolexReserver/Getter/getter_rolexReserve.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,14 @@
-#import datetime
-#import pandas as pd
-#import numpy as np
 import LibHanger.Library.uwLogger as Logger
 from bs4 import BeautifulSoup
 from pandas.core.frame import DataFrame
-#from enum import Enum
-#from decimal import Decimal
-#from LibHanger.Models.recset import recset
 from Scrapinger.Library.browserContainer import browserContainer
 from RolexReserver.Library.rolexReserverConfig import rolexReserverConfig
 from RolexReserver.Library.rolexReserverGlobals import *
 from RolexReserver.Library.rolexReserverException import getterError
-#from RolexReserver.Library.rolexReserverException import gettingValueError
 from RolexReserver.Getter.Base.baseGetter import baseGetter
 
 class getter_rolexReserve(baseGetter):
     
     """
     予約サイト巡回
     """
@@ -49,27 +42,26 @@
         
         Parameters
         ----------
         None
         
         """
         
-        result = None
         try:
             kwargs['getter'] = self
             
             # 予約状況取得
-            self.getRolexReserveDataToDataFrame(**kwargs)
+            for times in range(int(gv.rolexReserverConfig.gettingCount)):
+                Logger.logging.info('times = {}'.format(str(times + 1)))
+                self.getRolexReserveDataToDataFrame(**kwargs)
             
         except Exception as e: # その他例外
             Logger.logging.error(str(e))
             raise getterError
         
-        return result
-    
     def cbCheckMem():
         pass
     
     @Logger.loggerDecorator("getStockDataToDataFrame")
     def getRolexReserveDataToDataFrame(self, *args, **kwargs):
 
         """
```

### Comparing `RolexReserver-1.0.2/RolexReserver/Library/rolexReserverConfig.py` & `RolexReserver-1.0.3/RolexReserver/Library/rolexReserverConfig.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,17 @@
 
         self.menuExistsCheckLogNoData = "NO DATA"
         """ 予約可能メニュー存在チェックログ(データ無し) """
 
         self.menuExistsCheckLogExistsData = "EXISTS DATA"
         """ 予約可能メニュー存在チェックログ(データ有り) """
         
+        self.gettingCount = 5
+        """ 予約状況を確認する回数 """
+        
         # 設定ファイル名追加
         self.setConfigFileName('RolexReserver.ini')
         
     def getConfig(self, _scriptFilePath: str, configFileDir: str = ''):
         
         """ 
         設定ファイルを読み込む 
@@ -124,7 +127,10 @@
         self.setConfigValue('menuExistsCheckLogFormat',self.config_ini,'SITE','MENU_EXISTS_CHECK_LOG_FORMAT',str)
 
         # menuExistsCheckLogNoData
         self.setConfigValue('menuExistsCheckLogNoData',self.config_ini,'SITE','MENU_EXISTS_CHECK_LOG_NODATA',str)
 
         # menuExistsCheckLogExistsData
         self.setConfigValue('menuExistsCheckLogExistsData',self.config_ini,'SITE','MENU_EXISTS_CHECK_LOG_EXISTSDATA',str)
+
+        # gettingCount
+        self.setConfigValue('gettingCount',self.config_ini,'SITE','GETTING_COUNT',str)
```

### Comparing `RolexReserver-1.0.2/RolexReserver/Library/rolexReserverConfiger.py` & `RolexReserver-1.0.3/RolexReserver/Library/rolexReserverConfiger.py`

 * *Files identical despite different names*

### Comparing `RolexReserver-1.0.2/RolexReserver/Library/rolexReserverController.py` & `RolexReserver-1.0.3/RolexReserver/Library/rolexReserverController.py`

 * *Files identical despite different names*

### Comparing `RolexReserver-1.0.2/RolexReserver/Library/rolexReserverException.py` & `RolexReserver-1.0.3/RolexReserver/Library/rolexReserverException.py`

 * *Files identical despite different names*

### Comparing `RolexReserver-1.0.2/RolexReserver/Library/rolexReserverGlobals.py` & `RolexReserver-1.0.3/RolexReserver/Library/rolexReserverGlobals.py`

 * *Files identical despite different names*

### Comparing `RolexReserver-1.0.2/RolexReserver/Library/rolexReserverMailer.py` & `RolexReserver-1.0.3/RolexReserver/Library/rolexReserverMailer.py`

 * *Files identical despite different names*

### Comparing `RolexReserver-1.0.2/RolexReserver.egg-info/PKG-INFO` & `RolexReserver-1.0.3/RolexReserver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RolexReserver
-Version: 1.0.2
+Version: 1.0.3
 Summary: RolexReserver Package
 Home-page: https://github.com/kaioman/RolexReserver.git
 Author: unchainworks
 Author-email: kajin0318@gmail.com
 License: BSD-3-Clause
 Keywords: RolexReserver
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `RolexReserver-1.0.2/RolexReserver.egg-info/SOURCES.txt` & `RolexReserver-1.0.3/RolexReserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RolexReserver-1.0.2/RolexReserver.egg-info/requires.txt` & `RolexReserver-1.0.3/RolexReserver.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 greenlet==2.0.1
 idna==3.4
 importlib-metadata==6.0.0
 jaraco.classes==3.2.3
 keyring==23.13.1
 LibHanger
 lxml==4.9.1
+markdown-it-py==2.2.0
+mdurl==0.1.2
 more-itertools==9.0.0
 numpy==1.23.4
 openpyxl==3.0.10
 pandas==1.5.1
 Pillow==9.3.0
 pkginfo==1.9.5
 psutil==5.9.4
@@ -32,11 +34,13 @@
 rich==13.0.1
 Scrapinger
 selenium==3.141.0
 six==1.16.0
 soupsieve==2.3.2.post1
 SQLAlchemy==1.4.44
 twine==4.0.2
+typing_extensions==4.5.0
+tzdata==2023.3
 urllib3==1.26.12
 webencodings==0.5.1
 xlrd==2.0.1
 zipp==3.11.0
```

### Comparing `RolexReserver-1.0.2/setup.py` & `RolexReserver-1.0.3/setup.py`

 * *Files identical despite different names*

