# Comparing `tmp/comathon-0.0.8-py3-none-any.whl.zip` & `tmp/comathon-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 23216 bytes, number of entries: 19
+Zip file size: 23223 bytes, number of entries: 19
 -rw-rw-rw-  2.0 fat       41 b- defN 22-Sep-17 12:20 comathon/__init__.py
 -rw-rw-rw-  2.0 fat    24333 b- defN 22-Sep-17 12:20 comathon/cmt_exchange.py
 -rw-rw-rw-  2.0 fat    15250 b- defN 22-Sep-17 12:20 comathon/cmt_quotation.py
--rw-rw-rw-  2.0 fat     2054 b- defN 22-Sep-25 12:21 comathon/cmt_test.py
+-rw-rw-rw-  2.0 fat     2053 b- defN 22-Sep-25 12:35 comathon/cmt_test.py
 -rw-rw-rw-  2.0 fat      283 b- defN 22-Sep-17 12:20 comathon/myfunctions.py
 -rw-rw-rw-  2.0 fat     5023 b- defN 22-Sep-17 12:20 comathon/pyupbit_errors.py
 -rw-rw-rw-  2.0 fat    24333 b- defN 22-Sep-17 12:20 comathon/pyupbit_exchange_api.py
 -rw-rw-rw-  2.0 fat    15250 b- defN 22-Sep-17 12:20 comathon/pyupbit_quotation_api.py
 -rw-rw-rw-  2.0 fat     4168 b- defN 22-Sep-17 12:20 comathon/pyupbit_request_api.py
 -rw-rw-rw-  2.0 fat     3622 b- defN 22-Sep-17 12:20 comathon/pyupbit_websocket_api.py
 -rw-rw-rw-  2.0 fat      411 b- defN 22-Sep-17 12:20 comathon/simple_addition.py
 -rw-rw-rw-  2.0 fat      479 b- defN 22-Sep-25 09:58 comathon/test_restAPI.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Sep-17 12:20 comathon_test/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Sep-17 12:20 comathon_test/test_myfunctions.py
--rw-rw-rw-  2.0 fat     1088 b- defN 22-Sep-25 12:25 comathon-0.0.8.dist-info/LICENSE.rst
--rw-rw-rw-  2.0 fat      268 b- defN 22-Sep-25 12:25 comathon-0.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Sep-25 12:25 comathon-0.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       23 b- defN 22-Sep-25 12:25 comathon-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1561 b- defN 22-Sep-25 12:25 comathon-0.0.8.dist-info/RECORD
-19 files, 98279 bytes uncompressed, 20662 bytes compressed:  79.0%
+-rw-rw-rw-  2.0 fat     1088 b- defN 22-Sep-25 12:37 comathon-0.0.9.dist-info/LICENSE.rst
+-rw-rw-rw-  2.0 fat      291 b- defN 22-Sep-25 12:37 comathon-0.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 22-Sep-25 12:37 comathon-0.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       23 b- defN 22-Sep-25 12:37 comathon-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1561 b- defN 22-Sep-25 12:37 comathon-0.0.9.dist-info/RECORD
+19 files, 98301 bytes uncompressed, 20669 bytes compressed:  79.0%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: comathon_test/__init__.py
 Comment: 
 
 Filename: comathon_test/test_myfunctions.py
 Comment: 
 
-Filename: comathon-0.0.8.dist-info/LICENSE.rst
+Filename: comathon-0.0.9.dist-info/LICENSE.rst
 Comment: 
 
-Filename: comathon-0.0.8.dist-info/METADATA
+Filename: comathon-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: comathon-0.0.8.dist-info/WHEEL
+Filename: comathon-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: comathon-0.0.8.dist-info/top_level.txt
+Filename: comathon-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: comathon-0.0.8.dist-info/RECORD
+Filename: comathon-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## comathon/cmt_test.py

```diff
@@ -56,11 +56,11 @@
         secret_key = i['securitykey']
 
         upbit = pyupbit.Upbit(access_key, secret_key)  # API 로그인 함수 호출
         upbit #upbit 라는 instance가 생성됨
         KRW_balance = upbit.get_balance()
         print(i['userid'], "Balance : ", KRW_balance)
                 
-        coin_balance = upbit.get_balance(ticker=)
+        coin_balance = upbit.get_balance(ticker)
         sell_coin = upbit.sell_market_order(ticker, coin_balance) ## Sell all balance
 
     return None
```

## Comparing `comathon-0.0.8.dist-info/LICENSE.rst` & `comathon-0.0.9.dist-info/LICENSE.rst`

 * *Files identical despite different names*

## Comparing `comathon-0.0.8.dist-info/RECORD` & `comathon-0.0.9.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 comathon/__init__.py,sha256=p2Hja89bx5ViKNUTE0PRDFWCvyvK0qh8IcxSrRaAm54,41
 comathon/cmt_exchange.py,sha256=rH98jboDeGY01XIOmEPT0lDiP8CJ_y32kEmgLL5VM2Q,24333
 comathon/cmt_quotation.py,sha256=T-OUOJeqzoCqMQIAtuzSmw7on8UcIgXAppMxcApTOf4,15250
-comathon/cmt_test.py,sha256=c8_xfPfPHkTjsGTAiqJV_O9oWlD39bsWzUFOJ6EY40Q,2054
+comathon/cmt_test.py,sha256=0jG7c8LCAlHqlCoWPzDLiJojw9nye17dfCZBHkJcLcY,2053
 comathon/myfunctions.py,sha256=hhE6iPf4OGWedsEQZjDyUbcvSTYdl71mGZUshYkHRa4,283
 comathon/pyupbit_errors.py,sha256=LpPJ7tpm1gBx8H2GR_r6n6TcDOTOWQlp62qY8TBibw8,5023
 comathon/pyupbit_exchange_api.py,sha256=rH98jboDeGY01XIOmEPT0lDiP8CJ_y32kEmgLL5VM2Q,24333
 comathon/pyupbit_quotation_api.py,sha256=T-OUOJeqzoCqMQIAtuzSmw7on8UcIgXAppMxcApTOf4,15250
 comathon/pyupbit_request_api.py,sha256=CTdhHw3H-FR1r48UjOQR4t2-uAi9PpodTwGMaT2Bum8,4168
 comathon/pyupbit_websocket_api.py,sha256=eQwrpoEJ-7AIeHyKinUqydbRms4ruB09pK9ezTZyWXk,3622
 comathon/simple_addition.py,sha256=pqP-vMDlKQEL-eK18bIzUwvd01LJI_tUljusxTnluHE,411
 comathon/test_restAPI.py,sha256=mgHL5C7usqMhLe8aOE2Ee-cwBfaCdlop9AiOgUHy3mQ,479
 comathon_test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 comathon_test/test_myfunctions.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-comathon-0.0.8.dist-info/LICENSE.rst,sha256=ogqZImH5e0QPxVcwonCtLUGKEFUxFIifb3aK9JHysE8,1088
-comathon-0.0.8.dist-info/METADATA,sha256=vxVF52I8zLY8WV2Dldk5d2fN-9U2Vee5-ZqMOySY7iU,268
-comathon-0.0.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-comathon-0.0.8.dist-info/top_level.txt,sha256=yoNhE8mDf5F4aOmVsKykTN51Rj-zX6PCF_m2DmHe7EE,23
-comathon-0.0.8.dist-info/RECORD,,
+comathon-0.0.9.dist-info/LICENSE.rst,sha256=ogqZImH5e0QPxVcwonCtLUGKEFUxFIifb3aK9JHysE8,1088
+comathon-0.0.9.dist-info/METADATA,sha256=uZG9lGuxh-ekxH65wVU_jbk730wyypQ8gb4AAmWSEKQ,291
+comathon-0.0.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+comathon-0.0.9.dist-info/top_level.txt,sha256=yoNhE8mDf5F4aOmVsKykTN51Rj-zX6PCF_m2DmHe7EE,23
+comathon-0.0.9.dist-info/RECORD,,
```

