# Comparing `tmp/bb_clients-0.1.36.tar.gz` & `tmp/bb_clients-0.1.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bb_clients-0.1.36.tar", last modified: Thu Mar 23 21:09:14 2023, max compression
+gzip compressed data, was "bb_clients-0.1.37.tar", last modified: Tue May 23 16:07:30 2023, max compression
```

## Comparing `bb_clients-0.1.36.tar` & `bb_clients-0.1.37.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      199 2023-03-23 21:09:13.636942 bb_clients-0.1.36/.bumpversion.cfg
--rw-r--r--   0        0        0     2057 2022-06-05 23:32:58.789493 bb_clients-0.1.36/.gitignore
--rw-r--r--   0        0        0       11 2022-06-05 23:32:58.789493 bb_clients-0.1.36/.python-version
--rw-r--r--   0        0        0     1078 2020-08-20 16:30:08.246633 bb_clients-0.1.36/LICENSE
--rw-r--r--   0        0        0       13 2020-08-20 17:03:12.984708 bb_clients-0.1.36/README.md
--rw-r--r--   0        0        0      151 2023-03-23 21:09:13.636942 bb_clients-0.1.36/bb_clients/__init__.py
--rw-r--r--   0        0        0     7819 2020-11-23 21:29:19.382816 bb_clients-0.1.36/bb_clients/fc/__init__.py
--rw-r--r--   0        0        0    11519 2023-03-23 21:08:11.629074 bb_clients-0.1.36/bb_clients/ims/__init__.py
--rw-r--r--   0        0        0      788 2020-11-23 21:29:19.382816 bb_clients-0.1.36/conftest.py
--rwxr-xr-x   0        0        0      384 2020-08-04 16:23:00.508000 bb_clients-0.1.36/patch.py
--rw-r--r--   0        0        0      561 2020-11-23 21:29:19.382816 bb_clients-0.1.36/pyproject.toml
--rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 bb_clients-0.1.36/PKG-INFO
+-rw-r--r--   0        0        0      199 2023-05-23 16:07:29.444836 bb_clients-0.1.37/.bumpversion.cfg
+-rw-r--r--   0        0        0     2057 2021-12-02 15:50:33.362838 bb_clients-0.1.37/.gitignore
+-rw-r--r--   0        0        0       11 2022-11-09 23:03:17.967780 bb_clients-0.1.37/.python-version
+-rw-r--r--   0        0        0     1078 2021-12-02 15:39:05.410072 bb_clients-0.1.37/LICENSE
+-rw-r--r--   0        0        0       13 2021-12-02 15:39:05.410072 bb_clients-0.1.37/README.md
+-rw-r--r--   0        0        0      151 2023-05-23 16:07:29.444836 bb_clients-0.1.37/bb_clients/__init__.py
+-rw-r--r--   0        0        0     7819 2021-12-02 15:39:05.410072 bb_clients-0.1.37/bb_clients/fc/__init__.py
+-rw-r--r--   0        0        0    12413 2023-05-23 15:45:41.587630 bb_clients-0.1.37/bb_clients/ims/__init__.py
+-rw-r--r--   0        0        0      788 2021-12-02 15:39:05.410072 bb_clients-0.1.37/conftest.py
+-rwxr-xr-x   0        0        0      384 2021-12-02 15:50:11.214687 bb_clients-0.1.37/patch.py
+-rw-r--r--   0        0        0      561 2021-12-02 15:39:05.410072 bb_clients-0.1.37/pyproject.toml
+-rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 bb_clients-0.1.37/PKG-INFO
```

### Comparing `bb_clients-0.1.36/.gitignore` & `bb_clients-0.1.37/.gitignore`

 * *Files identical despite different names*

### Comparing `bb_clients-0.1.36/LICENSE` & `bb_clients-0.1.37/LICENSE`

 * *Files identical despite different names*

### Comparing `bb_clients-0.1.36/bb_clients/fc/__init__.py` & `bb_clients-0.1.37/bb_clients/fc/__init__.py`

 * *Files identical despite different names*

### Comparing `bb_clients-0.1.36/bb_clients/ims/__init__.py` & `bb_clients-0.1.37/bb_clients/ims/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+import json
 from asyncio import sleep
 from datetime import datetime, timedelta
 from functools import lru_cache
 from http.client import HTTPException
 from json import JSONDecodeError
 from os import getenv
 from typing import Iterable, List, Union, Optional
 
 import httpx
 import pytz
 from dateutil.parser import parse
 from loguru import logger
 from pydantic import BaseModel
+from pydantic.json import pydantic_encoder
 from starlette.status import HTTP_200_OK
 from tenacity import retry, stop_after_attempt, wait_fixed
 
 
 class Tank(BaseModel):
     id: str
     monitor_type: str
@@ -25,21 +27,34 @@
     store_number: str
     tank_id: str
     temperature: Optional[float]
     updated: datetime
     volume: float
 
 
+class BaseStoreTank(BaseModel):
+    store: str
+    tank: str
+
+    @property
+    def identity(self):
+        return f"{self.store}:{self.tank}"
+
+    def store_tank_query(self):
+        return {"store_number": self.store, "tank_id": self.tank}
+
+
 class Reading(BaseModel):
-    read_time: datetime
-    run_time: datetime
     store_number: str
     tank_id: str
+    run_time: datetime  # UTC
+    read_time: datetime  # UTC
     volume: float
-    temperature: float
+    product: str = None
+    temperature: float = 0
 
 
 class RegisterTankMonitorRequest(BaseModel):
     store_number: str
     host: str
     port: int
     monitor_type: str
@@ -104,25 +119,37 @@
     ) -> list[NearestReading]:
         r = httpx.post(
             f"{self.base_url}/tank_inventory/nearest",
             json=store_numbers,
             params={"date": date.isoformat(), **self.params},
             timeout=self.timeout,
         )
-        print(r.json())
         data = r.json() if r.status_code == 200 else []
 
         def fix_store_to_site(row):
             row["site"] = row["store_number"]
             return row
 
         return [NearestReading.parse_obj(fix_store_to_site(row)) for row in data]
 
     @logger.catch(reraise=True)
     @retry(reraise=True, stop=stop_after_attempt(3), wait=wait_fixed(5))
+    def latest_readings(self, store_tanks: Iterable[BaseStoreTank]) -> list[Reading]:
+        encoded = json.dumps([d.dict() for d in store_tanks], default=pydantic_encoder)
+        r = httpx.post(
+            f"{self.base_url}/tank_inventory/latest/many",
+            data=encoded,
+            params=self.params,
+            timeout=self.timeout,
+        )
+        data = r.json() if r.status_code == 200 else []
+        return [Reading.parse_obj(row) for row in data]
+
+    @logger.catch(reraise=True)
+    @retry(reraise=True, stop=stop_after_attempt(3), wait=wait_fixed(5))
     def tank_connection_information(self, store, tank):
         params = {
             **self.params,
             "store_number": store,
             "tank_id": str(tank),
         }
```

### Comparing `bb_clients-0.1.36/conftest.py` & `bb_clients-0.1.37/conftest.py`

 * *Files identical despite different names*

### Comparing `bb_clients-0.1.36/pyproject.toml` & `bb_clients-0.1.37/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bb_clients-0.1.36/PKG-INFO` & `bb_clients-0.1.37/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bb_clients
-Version: 0.1.36
+Version: 0.1.37
 Summary: Simple python clients for the Gravitate BestBuy Services
 Author: James Vogel
 Author-email: jim.m.vogel@gmail.com
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: loguru
```

