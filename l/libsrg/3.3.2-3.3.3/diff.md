# Comparing `tmp/libsrg-3.3.2-py3-none-any.whl.zip` & `tmp/libsrg-3.3.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,26 @@
-Zip file size: 31516 bytes, number of entries: 24
+Zip file size: 31527 bytes, number of entries: 24
 -rw-r--r--  2.0 unx     2103 b- defN 23-May-15 18:15 libsrg/Info.py
 -rw-r--r--  2.0 unx     3532 b- defN 23-Jan-31 15:26 libsrg/LevelBanner.py
 -rw-r--r--  2.0 unx     1492 b- defN 23-Jan-18 20:30 libsrg/LoggerGUIProxy.py
 -rw-r--r--  2.0 unx     5511 b- defN 23-Jan-31 15:26 libsrg/LoggingAppBase.py
 -rw-r--r--  2.0 unx     5733 b- defN 23-Jan-31 15:30 libsrg/LoggingCounter.py
 -rw-r--r--  2.0 unx      413 b- defN 23-Jan-31 15:26 libsrg/LoggingUtils.py
 -rw-r--r--  2.0 unx     1376 b- defN 23-Jan-08 15:03 libsrg/LoggingWatcher.py
 -rw-r--r--  2.0 unx     2680 b- defN 23-Jan-31 15:30 libsrg/NagiosBase.py
 -rw-r--r--  2.0 unx    14015 b- defN 23-May-01 17:29 libsrg/ReZFS.py
--rw-r--r--  2.0 unx     4193 b- defN 23-Feb-02 14:45 libsrg/Runner.py
+-rw-r--r--  2.0 unx     4214 b- defN 23-May-22 23:22 libsrg/Runner.py
 -rw-r--r--  2.0 unx     4015 b- defN 23-Jan-31 15:30 libsrg/Runner2.py
 -rw-r--r--  2.0 unx     6947 b- defN 23-Feb-09 18:22 libsrg/Stage0.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jan-31 16:52 libsrg/__init__.py
 -rw-r--r--  2.0 unx    17506 b- defN 23-Feb-06 00:12 libsrg/ztool.py
 -rw-r--r--  2.0 unx     2214 b- defN 23-Feb-05 15:02 libsrg/TKGUI/GuiBase.py
 -rw-r--r--  2.0 unx      447 b- defN 22-Mar-14 16:04 libsrg/TKGUI/GuiRequest.py
 -rw-r--r--  2.0 unx     3414 b- defN 23-Feb-05 15:22 libsrg/TKGUI/GuiRequestQueue.py
 -rw-r--r--  2.0 unx    10692 b- defN 23-May-15 18:18 libsrg/TKGUI/LoggerGUI.py
 -rw-r--r--  2.0 unx        1 b- defN 23-Jan-31 17:16 libsrg/TKGUI/__init__.py
--rw-rw-rw-  2.0 unx     1069 b- defN 23-May-15 18:18 libsrg-3.3.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     3357 b- defN 23-May-15 18:18 libsrg-3.3.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-15 18:18 libsrg-3.3.2.dist-info/WHEEL
--rw-rw-rw-  2.0 unx        7 b- defN 23-May-15 18:18 libsrg-3.3.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1861 b- defN 23-May-15 18:18 libsrg-3.3.2.dist-info/RECORD
-24 files, 92670 bytes uncompressed, 28556 bytes compressed:  69.2%
+-rw-rw-rw-  2.0 unx     1069 b- defN 23-May-22 23:24 libsrg-3.3.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     3357 b- defN 23-May-22 23:24 libsrg-3.3.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-22 23:24 libsrg-3.3.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx        7 b- defN 23-May-22 23:24 libsrg-3.3.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1861 b- defN 23-May-22 23:24 libsrg-3.3.3.dist-info/RECORD
+24 files, 92691 bytes uncompressed, 28567 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -51,23 +51,23 @@
 
 Filename: libsrg/TKGUI/LoggerGUI.py
 Comment: 
 
 Filename: libsrg/TKGUI/__init__.py
 Comment: 
 
-Filename: libsrg-3.3.2.dist-info/LICENSE.txt
+Filename: libsrg-3.3.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: libsrg-3.3.2.dist-info/METADATA
+Filename: libsrg-3.3.3.dist-info/METADATA
 Comment: 
 
-Filename: libsrg-3.3.2.dist-info/WHEEL
+Filename: libsrg-3.3.3.dist-info/WHEEL
 Comment: 
 
-Filename: libsrg-3.3.2.dist-info/top_level.txt
+Filename: libsrg-3.3.3.dist-info/top_level.txt
 Comment: 
 
-Filename: libsrg-3.3.2.dist-info/RECORD
+Filename: libsrg-3.3.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## libsrg/Runner.py

```diff
@@ -1,11 +1,11 @@
 import logging
 import subprocess
 from pathlib import Path
-from typing import List, Optional
+from typing import List, Optional,Union
 
 
 class Runner:
     """
     Runner is a utility class to run a command as a subprocess and return results
     * command is passed as a list of program followed by zero or more arguments
       * if provided as a single string, call split to make it a list
@@ -20,16 +20,16 @@
     * any exception raised is caught
       * returned in caught field
       * logged as an error
       * optionally rethrown if rethrow is set True
     * success field is true if no exceptions caught and return code is zero
     """
 
-    def __init__(self, cmd: List[str] | str, timeout=None, rethrow=False, verbose=False,
-                 cwd: Optional[str | Path] = None,
+    def __init__(self, cmd: Union[ List[str] , str], timeout=None, rethrow=False, verbose=False,
+                 cwd: Optional[Union[str , Path]] = None,
                  userat: Optional[str] = None):
         """
         Run the given command and return results
 
         :param cmd: A list of strings, or a single string which Runner will str.split()
         :param timeout: If positive, number of seconds before a timeout exception is raised
         :param rethrow: If true, rethrow any exceptions caught, else success set False
```

## Comparing `libsrg-3.3.2.dist-info/LICENSE.txt` & `libsrg-3.3.3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `libsrg-3.3.2.dist-info/METADATA` & `libsrg-3.3.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libsrg
-Version: 3.3.2
+Version: 3.3.3
 Summary: Base class for logging apps, Nagios, utilities
 Home-page: https://gitlab.com/SRG_gitlab/libsrg
 Author: Steven Goncalo
 Author-email: srg_pypi@ice9mail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `libsrg-3.3.2.dist-info/RECORD` & `libsrg-3.3.3.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 libsrg/LoggerGUIProxy.py,sha256=qrgLnB0Gtmu5IXP9EzBpIpKWYphcVVQOmIpqWOH9Y6k,1492
 libsrg/LoggingAppBase.py,sha256=JCeaLFPTwQjVS2YnIHOh5ciK54u1lLXt_dwGP7hv-r0,5511
 libsrg/LoggingCounter.py,sha256=fL3E_lErmjSQDy9TPDn-m0_PASoOM7wlf3VQs2R4AEM,5733
 libsrg/LoggingUtils.py,sha256=brhP-2YaCd69vI0CKWTFUZtiTRhj1ud4i-tApP4FWg0,413
 libsrg/LoggingWatcher.py,sha256=tZ803wbw_qvW8tSRDwAbBRQSCrMzhz-FIJsf_hCNIFo,1376
 libsrg/NagiosBase.py,sha256=5FniCUJ8ywFX8oM2q0gKQX2Wvz6J6yt0HT_WYfPniik,2680
 libsrg/ReZFS.py,sha256=8SInGf72nnju_MRpYqNPtf6VHAqesuZr50_wy7iPE_c,14015
-libsrg/Runner.py,sha256=CeZLOhBiIUZ60MgBxktQnaWB5NsLhJE8wNJISd23TtM,4193
+libsrg/Runner.py,sha256=ujgpms51fz5H43y_YXjhMorjrFfneVEd79Aajq3gMIA,4214
 libsrg/Runner2.py,sha256=bZqvmyw9O-2XQconsWQTvtUHy7QYzQrNfoSBKMc3XXA,4015
 libsrg/Stage0.py,sha256=gMPTzSn7ZE0RaO85zmvwZbik4zPUsuwnNITUsD1iXWE,6947
 libsrg/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 libsrg/ztool.py,sha256=PCGHW1WghwegWXyR8rhYocsJ2HyDfjGSd5-gcvjIhJY,17506
 libsrg/TKGUI/GuiBase.py,sha256=MG4D10voRxszQvglABmHG8GHqRNXNo6gWZmY77fpkGU,2214
 libsrg/TKGUI/GuiRequest.py,sha256=ZrUBxrpkAV8ITqbcr7br0-sX9iK69bx1_Fu7COKB5uc,447
 libsrg/TKGUI/GuiRequestQueue.py,sha256=SLoT-PdXgK4JgU-WcESlRwehZIEPBwRgPORn0Tm8Mws,3414
 libsrg/TKGUI/LoggerGUI.py,sha256=A2XBTtlvtNwnxFlw8xTkHkuCITxvgZlQfWjWeaAmejQ,10692
 libsrg/TKGUI/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-libsrg-3.3.2.dist-info/LICENSE.txt,sha256=ACwmltkrXIz5VsEQcrqljq-fat6ZXAMepjXGoe40KtE,1069
-libsrg-3.3.2.dist-info/METADATA,sha256=LV4NY71c-HaRMKLZuSKBgFNqLMqNhp_yoMVtI_cE4LU,3357
-libsrg-3.3.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-libsrg-3.3.2.dist-info/top_level.txt,sha256=NYEOHhvqWFavgb_q4ADmjraMpsan8oFEQPXmMMHGvZ0,7
-libsrg-3.3.2.dist-info/RECORD,,
+libsrg-3.3.3.dist-info/LICENSE.txt,sha256=ACwmltkrXIz5VsEQcrqljq-fat6ZXAMepjXGoe40KtE,1069
+libsrg-3.3.3.dist-info/METADATA,sha256=BSZVgO6eXgohxTAhJmG869N7gw70nDDB9dzmpoO9Lxs,3357
+libsrg-3.3.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+libsrg-3.3.3.dist-info/top_level.txt,sha256=NYEOHhvqWFavgb_q4ADmjraMpsan8oFEQPXmMMHGvZ0,7
+libsrg-3.3.3.dist-info/RECORD,,
```

