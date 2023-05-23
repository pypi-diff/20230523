# Comparing `tmp/fyerspysdk1-1.4-py3-none-any.whl.zip` & `tmp/fyerspysdk1-1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 12099 bytes, number of entries: 9
+Zip file size: 12401 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx       20 b- defN 23-May-22 12:28 fyerstest/__init__.py
--rw-rw-r--  2.0 unx    16512 b- defN 23-May-23 04:45 fyerstest/fyersApi.py
--rw-rw-r--  2.0 unx    15732 b- defN 23-May-22 11:31 fyerstest/hsmFyers.py
--rw-rw-r--  2.0 unx     7894 b- defN 23-May-22 11:30 fyerstest/ws.py
--rwxrwxr-x  2.0 unx     1063 b- defN 23-May-23 05:00 fyerspysdk1-1.4.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx      622 b- defN 23-May-23 05:00 fyerspysdk1-1.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-23 05:00 fyerspysdk1-1.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-May-23 05:00 fyerspysdk1-1.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      705 b- defN 23-May-23 05:00 fyerspysdk1-1.4.dist-info/RECORD
-9 files, 42650 bytes uncompressed, 10891 bytes compressed:  74.5%
+-rw-rw-r--  2.0 unx    16456 b- defN 23-May-23 06:08 fyerstest/fyersApi.py
+-rw-rw-r--  2.0 unx    16544 b- defN 23-May-23 06:09 fyerstest/hsmFyers.py
+-rw-rw-r--  2.0 unx     8236 b- defN 23-May-23 06:09 fyerstest/ws.py
+-rwxrwxr-x  2.0 unx     1063 b- defN 23-May-23 06:09 fyerspysdk1-1.5.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx      622 b- defN 23-May-23 06:09 fyerspysdk1-1.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-23 06:09 fyerspysdk1-1.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-May-23 06:09 fyerspysdk1-1.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      705 b- defN 23-May-23 06:09 fyerspysdk1-1.5.dist-info/RECORD
+9 files, 43748 bytes uncompressed, 11193 bytes compressed:  74.4%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: fyerstest/hsmFyers.py
 Comment: 
 
 Filename: fyerstest/ws.py
 Comment: 
 
-Filename: fyerspysdk1-1.4.dist-info/LICENSE.txt
+Filename: fyerspysdk1-1.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: fyerspysdk1-1.4.dist-info/METADATA
+Filename: fyerspysdk1-1.5.dist-info/METADATA
 Comment: 
 
-Filename: fyerspysdk1-1.4.dist-info/WHEEL
+Filename: fyerspysdk1-1.5.dist-info/WHEEL
 Comment: 
 
-Filename: fyerspysdk1-1.4.dist-info/top_level.txt
+Filename: fyerspysdk1-1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: fyerspysdk1-1.4.dist-info/RECORD
+Filename: fyerspysdk1-1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fyerstest/fyersApi.py

```diff
@@ -391,27 +391,25 @@
         if self.is_async:
             
             response = asyncio.run(self.service.postAsyncCall(Config.gttorders, self.header, data))
         else:  
             response = self.service.postCall(Config.gttorders, self.header, data)
         return response
     
-    def get_gttorders(self, data):
+    def get_gttorders(self):
 
         '''
         Retrieves order details by Id
 
         '''
 
         if self.is_async:
-            
-            response = asyncio.run(self.service.getAsyncCall(Config.gttorders, self.header, params=data))
+            response = asyncio.run(self.service.getAsyncCall(Config.gttorders, self.header))
         else:
-            
-            response = self.service.getCall(Config.gttorders, self.header, data=data)
+            response = self.service.getCall(Config.gttorders, self.header)
         return response
     
     def modify_gttorder(self, data):
             '''
             Modify order
             
             '''
```

## fyerstest/hsmFyers.py

```diff
@@ -1,23 +1,24 @@
 import asyncio
 import struct
 import websockets
 
 
 class FyersHsmSocket():
 
-    def __init__(self,access_token,scrips):
+    def __init__(self,access_token,scrips, litemode = False):
         self.url = ""
         self.access_token = access_token
         self.Source = "PythonSDK-1.0.0"
         self.channelNum = 1
         self.scrips = scrips
         self.channels = [1,2,3,4,5]
         self.ackCount = None
         self.updateCount = 0
+        self.lite = litemode
         self.output = {}
         self.resp = {}
         self.symDict = {}
 
     def TokenByteMsg(self):
         buffer_size = 18 + len(self.access_token) + len(self.Source)
         byte_buffer = bytearray(buffer_size)
@@ -304,44 +305,62 @@
             message = self.TokenByteMsg()
             await websocket.send(message)
             print(f"Sent message: {message}")
             response = await websocket.recv()
             # print(response)
             self.ByteToJson(response)
             # message = b'\x00\x11\x0c\x02\x01\x00\x08\x00\x00\x00\x00\x00\x00\x12&\x02\x00\x01F'
-            message = self.SetToFullMode()
-            await websocket.send(message)
-            response = await websocket.recv()
-            self.ByteToJson(response)
-            
+            if not self.lite:
+                message = self.SetToFullMode()
+                await websocket.send(message)
+                response = await websocket.recv()
+                self.ByteToJson(response)
+                
             # message = bytearray(b'\x00\xaf\x04\x02\x01\x00V\x00\x06\x0fsf|nse_cm|11536\x0fdp|nse_cm|11536\x0csf|nse_cm|25\x0cdp|nse_cm|25\x0csf|nse_cm|22\x0cdp|nse_cm|22\x02\x00\x01\x01')
             # message =bytearray(b'\x00{\x04\x02\x01\x00"\x00\x02\x0fsf|nse_cm|11536\x0fdp|nse_cm|11536\x02\x00\x01\x01')
             message = self.SubscribeMsgByte()
             await websocket.send(message)
             print(f"Sent message: {message}")
             asyncio.ensure_future(self.send_ping(websocket))
             x = 0
             while True:
                 response = await websocket.recv()
                 self.ByteToJson(response)
-                x += 1
-                print("-------------------------------",x)
-                if x == 10:
-                    scrips = ["sf|nse_cm|25","dp|nse_cm|25", "sf|nse_cm|22", "dp|nse_cm|22"]
-                    msh = self.UnSubscribeByte(scrips)
-
-
-
-    async def main(self):
-        ws_task = asyncio.create_task(self.connectWS())
-
-        await ws_task
-
+                # x += 1
+                # print("-------------------------------",x)
+                # if x == 10:
+                #     scrips = ["sf|nse_cm|25","dp|nse_cm|25", "sf|nse_cm|22", "dp|nse_cm|22"]
+                #     msg = self.UnSubscribeByte(scrips)
+                #     await websocket.send(msg)
+                #     response = await websocket.recv()
+                #     self.ByteToJson(response)
+
+
+    # async def main(self):
+    #     ws_task = asyncio.create_task(self.connectWS())
+
+    #     await ws_task
+    def subscribe(self):
+        loop = asyncio.get_event_loop()
+        websocket_task = loop.create_task(self.connectWS())
+        try:
+            loop.run_until_complete(websocket_task)
+        except KeyboardInterrupt:
+            websocket_task.cancel()
+            try:
+                loop.run_until_complete(websocket_task)
+            except asyncio.CancelledError:
+                pass
+            finally:
+                loop.run_until_complete(self.close(websocket_task))
+        finally:
+            loop.close()
 # access_token ="3fd5caefeb662931c6560cf5991b55e327f33ddf8ca0b2a1b0ed7165"
 # access_token = "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJodHRwczovL2xvZ2luLmZ5ZXJzLmluIiwiaWF0IjoxNjg0NzMwNDA2LCJleHAiOjE2ODQ4MDE4MDYsIm5iZiI6MTY4NDczMDQwNiwiYXVkIjpbIng6MCJdLCJzdWIiOiJhY2Nlc3NfdG9rZW4iLCJhdF9oYXNoIjoiZ0FBQUFBQmthdkltdGMtQUFueTVnR2liMGRtVHdXeko5TmFuTUtEVlBzYTVHRnRFaUdCczN1OTh2ZE01UFlZanNOc3Bfd2szbEpYcUU5cXJTQVQ2eXJDZTh0R0pBcnlFcFJtaWhaSVMtSVBPZmY1VkVlX3M3U0U9IiwiZGlzcGxheV9uYW1lIjoiVklOQVkgS1VNQVIgTUFVUllBIiwiZnlfaWQiOiJYVjIwOTg2IiwiYXBwVHlwZSI6IiIsIm9tcyI6IksxIiwicG9hX2ZsYWciOiJOIiwiaHNtX2tleSI6IjNmZDVjYWVmZWI2NjI5MzFjNjU2MGNmNTk5MWI1NWUzMjdmMzNkZGY4Y2EwYjJhMWIwZWQ3MTY1In0.8I11EvKNf-Z4dHn8nd6gSM0AhN0D4zf0-e59GWaEP_8"
 # access_token = "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJhcGkuZnllcnMuaW4iLCJpYXQiOjE2ODQ3MzgzMjUsImV4cCI6MTY4NDgwMTgwNSwibmJmIjoxNjg0NzM4MzI1LCJhdWQiOlsieDowIiwieDoxIiwieDoyIiwiZDoxIiwiZDoyIiwieDoxIiwieDowIl0sInN1YiI6ImFjY2Vzc190b2tlbiIsImF0X2hhc2giOiJnQUFBQUFCa2F4RVZLSWZPVGVUNkZtYmw4b29wLW9sTU1JaG0waU1IOGIzZmNESlVxNjI1andudnM1LXdTTnA0RTR0TmY1aGxDWWNFUm56QXlnNWVmWFFTUVFiR0M2Y0NaMVVKN3hkc2ptZ3FMZkxOejhsa3FWZz0iLCJkaXNwbGF5X25hbWUiOiJWSU5BWSBLVU1BUiBNQVVSWUEiLCJvbXMiOiJLMSIsImZ5X2lkIjoiWFYyMDk4NiIsImFwcFR5cGUiOjEwMCwicG9hX2ZsYWciOiJOIn0.8GfqzLmubDCX-FCcjIppkzurYhz4wakgaeeD5Ryk30s"
 access_token = "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJhcGkuZnllcnMuaW4iLCJpYXQiOjE2ODMwMDE4OTgsImV4cCI6MTY4MzA3MzgzOCwibmJmIjoxNjgzMDAxODk4LCJhdWQiOlsieDowIiwieDoxIiwieDoyIiwiZDoxIiwiZDoyIiwieDoxIiwieDowIl0sInN1YiI6ImFjY2Vzc190b2tlbiIsImF0X2hhc2giOiJnQUFBQUFCa1VKSXFKLTNQMl9BSXFWWFNWUlg5UXlIVW5QWlpGRnFnNG5xRkNWRzYwQU5qX0F6T2hVWmxPZmtCNUV4ak03MXBMWVlqSEpjWXBsaVpVNWpFREQ1R3JFVkt4Rmx0SzR4RDh2SERVdkZndWgwUEVGRT0iLCJkaXNwbGF5X25hbWUiOiJWSU5BWSBLVU1BUiBNQVVSWUEiLCJvbXMiOiJLMSIsImZ5X2lkIjoiWFYyMDk4NiIsImFwcFR5cGUiOjEwMCwicG9hX2ZsYWciOiJOIn0.MghUuBXEV3INDwH-buwTUvJDvBQ0HS37d69nwRCE7nE"
 scrips =  ["sf|nse_cm|11536","sf|nse_cm|25","dp|nse_cm|25", "sf|nse_cm|22", "dp|nse_cm|22"]
 client = FyersHsmSocket(access_token,scrips)
 
-result = asyncio.run(client.main())
+# result = asyncio.run(client.main())
+client.subscribe()
```

## fyerstest/ws.py

```diff
@@ -140,17 +140,25 @@
 
     async def close(self, websocket_task):
         if not websocket_task.done():
             websocket = websocket_task.result()
             if not websocket.closed:
                 await websocket.close()
 
+    def get_or_create_eventloop(self):
+        try:
+            return asyncio.get_event_loop()
+        except RuntimeError as ex:
+            if "There is no current event loop in thread" in str(ex):
+                loop = asyncio.new_event_loop()
+                asyncio.set_event_loop(loop)
+                return asyncio.get_event_loop()
     def subscribe(self,data_type):
         self.data_type = [self.socket_type[(type)] for type in data_type.split(",")]
-        loop = asyncio.get_event_loop()
+        loop = self.get_or_create_eventloop()
         websocket_task = loop.create_task(self.ScoketConnect())
         try:
             loop.run_until_complete(websocket_task)
         except KeyboardInterrupt:
             websocket_task.cancel()
             try:
                 loop.run_until_complete(websocket_task)
@@ -196,11 +204,11 @@
 			},
 		}
         dictConfig(LOGGING)
         self.logger = logging.getLogger('fyers_socket')
 
 
 # client_id = "XC4EOD67IM-100"
-# access_token=  "XC4EOD67IM-100:eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJhcGkuZnllcnMuaW4iLCJpYXQiOjE2ODQ3MzgzMjUsImV4cCI6MTY4NDgwMTgwNSwibmJmIjoxNjg0NzM4MzI1LCJhdWQiOlsieDowIiwieDoxIiwieDoyIiwiZDoxIiwiZDoyIiwieDoxIiwieDowIl0sInN1YiI6ImFjY2Vzc190b2tlbiIsImF0X2hhc2giOiJnQUFBQUFCa2F4RVZLSWZPVGVUNkZtYmw4b29wLW9sTU1JaG0waU1IOGIzZmNESlVxNjI1andudnM1LXdTTnA0RTR0TmY1aGxDWWNFUm56QXlnNWVmWFFTUVFiR0M2Y0NaMVVKN3hkc2ptZ3FMZkxOejhsa3FWZz0iLCJkaXNwbGF5X25hbWUiOiJWSU5BWSBLVU1BUiBNQVVSWUEiLCJvbXMiOiJLMSIsImZ5X2lkIjoiWFYyMDk4NiIsImFwcFR5cGUiOjEwMCwicG9hX2ZsYWciOiJOIn0.8GfqzLmubDCX-FCcjIppkzurYhz4wakgaeeD5Ryk30s"
+access_token=  "XC4EOD67IM-100:eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJhcGkuZnllcnMuaW4iLCJpYXQiOjE2ODQ4MTM5NTgsImV4cCI6MTY4NDg4ODIzOCwibmJmIjoxNjg0ODEzOTU4LCJhdWQiOlsieDowIiwieDoxIiwieDoyIiwiZDoxIiwiZDoyIiwieDoxIiwieDowIl0sInN1YiI6ImFjY2Vzc190b2tlbiIsImF0X2hhc2giOiJnQUFBQUFCa2JEaUd1Q1BGek1uUFlXTVFxRjNvUGt0T3lsRDhpNzMyOTJfS0VVZUl6RU1oc2lKMTNLV2dfc2ZWU1BBWTFNdmxGblQtQzh0dG1VX1hqM1NYSklLLTNkaVFHMTZJVE5kTDlvVTJKSmxVbjBwNlI1UT0iLCJkaXNwbGF5X25hbWUiOiJWSU5BWSBLVU1BUiBNQVVSWUEiLCJvbXMiOiJLMSIsImZ5X2lkIjoiWFYyMDk4NiIsImFwcFR5cGUiOjEwMCwicG9hX2ZsYWciOiJOIn0.s4CJCOZCnUohVaMttSwA_Iz0p9t-HHSHNwqED5NemhQ"
 
-# fyers= FyersSocket(access_token,False , None)
-# fyers.subscribe("OnOrders,OnTrades,OnPositions")
+fyers= FyersSocket(access_token,False , None)
+fyers.subscribe("OnOrders,OnTrades,OnPositions")
```

## Comparing `fyerspysdk1-1.4.dist-info/LICENSE.txt` & `fyerspysdk1-1.5.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `fyerspysdk1-1.4.dist-info/METADATA` & `fyerspysdk1-1.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyerspysdk1
-Version: 1.4
+Version: 1.5
 Summary: XX trc APIs.
 Home-page: https://github.com
 Author: my-Tech
 Author-email: support@f.in
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

