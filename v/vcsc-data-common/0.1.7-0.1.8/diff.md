# Comparing `tmp/vcsc_data_common-0.1.7.tar.gz` & `tmp/vcsc_data_common-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcsc_data_common-0.1.7.tar", last modified: Mon May 15 02:02:43 2023, max compression
+gzip compressed data, was "vcsc_data_common-0.1.8.tar", last modified: Mon May 15 03:19:38 2023, max compression
```

## Comparing `vcsc_data_common-0.1.7.tar` & `vcsc_data_common-0.1.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-15 02:02:43.808848 vcsc_data_common-0.1.7/
--rw-r--r--   0 pd         (501) staff       (20)      300 2023-05-15 02:02:43.808918 vcsc_data_common-0.1.7/PKG-INFO
--rw-r--r--   0 pd         (501) staff       (20)      143 2023-02-22 09:16:04.000000 vcsc_data_common-0.1.7/README.md
--rw-r--r--   0 pd         (501) staff       (20)      799 2023-03-23 03:54:32.000000 vcsc_data_common-0.1.7/pyproject.toml
--rw-r--r--   0 pd         (501) staff       (20)      339 2023-05-15 02:02:43.809193 vcsc_data_common-0.1.7/setup.cfg
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-15 02:02:43.806994 vcsc_data_common-0.1.7/vcsc_data_common/
--rw-r--r--   0 pd         (501) staff       (20)      108 2023-02-22 09:07:01.000000 vcsc_data_common-0.1.7/vcsc_data_common/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-15 02:02:43.808054 vcsc_data_common-0.1.7/vcsc_data_common/ai_framework/
--rw-r--r--   0 pd         (501) staff       (20)       48 2023-02-22 09:02:01.000000 vcsc_data_common-0.1.7/vcsc_data_common/ai_framework/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     4948 2023-03-31 09:44:29.000000 vcsc_data_common-0.1.7/vcsc_data_common/ai_framework/interval_fetching.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-15 02:02:43.808207 vcsc_data_common-0.1.7/vcsc_data_common/backtest/
--rw-r--r--   0 pd         (501) staff       (20)     2537 2023-05-12 03:24:29.000000 vcsc_data_common-0.1.7/vcsc_data_common/backtest/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-15 02:02:43.808335 vcsc_data_common-0.1.7/vcsc_data_common/live_price_data/
--rw-r--r--   0 pd         (501) staff       (20)     2341 2023-05-04 06:36:10.000000 vcsc_data_common-0.1.7/vcsc_data_common/live_price_data/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-15 02:02:43.808461 vcsc_data_common-0.1.7/vcsc_data_common/offline_price_data/
--rw-r--r--   0 pd         (501) staff       (20)      880 2023-03-14 02:58:59.000000 vcsc_data_common-0.1.7/vcsc_data_common/offline_price_data/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-15 02:02:43.808591 vcsc_data_common-0.1.7/vcsc_data_common/order/
--rw-r--r--   0 pd         (501) staff       (20)     3706 2023-05-11 08:39:33.000000 vcsc_data_common-0.1.7/vcsc_data_common/order/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-15 02:02:43.808736 vcsc_data_common-0.1.7/vcsc_data_common/portfolio_info/
--rw-r--r--   0 pd         (501) staff       (20)     3660 2023-05-11 09:51:24.000000 vcsc_data_common-0.1.7/vcsc_data_common/portfolio_info/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-15 02:02:43.807754 vcsc_data_common-0.1.7/vcsc_data_common.egg-info/
--rw-r--r--   0 pd         (501) staff       (20)      300 2023-05-15 02:02:43.000000 vcsc_data_common-0.1.7/vcsc_data_common.egg-info/PKG-INFO
--rw-r--r--   0 pd         (501) staff       (20)      565 2023-05-15 02:02:43.000000 vcsc_data_common-0.1.7/vcsc_data_common.egg-info/SOURCES.txt
--rw-r--r--   0 pd         (501) staff       (20)        1 2023-05-15 02:02:43.000000 vcsc_data_common-0.1.7/vcsc_data_common.egg-info/dependency_links.txt
--rw-r--r--   0 pd         (501) staff       (20)      140 2023-05-15 02:02:43.000000 vcsc_data_common-0.1.7/vcsc_data_common.egg-info/requires.txt
--rw-r--r--   0 pd         (501) staff       (20)       17 2023-05-15 02:02:43.000000 vcsc_data_common-0.1.7/vcsc_data_common.egg-info/top_level.txt
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-15 03:19:38.822515 vcsc_data_common-0.1.8/
+-rw-r--r--   0 pd         (501) staff       (20)      300 2023-05-15 03:19:38.822623 vcsc_data_common-0.1.8/PKG-INFO
+-rw-r--r--   0 pd         (501) staff       (20)      143 2023-02-22 09:16:04.000000 vcsc_data_common-0.1.8/README.md
+-rw-r--r--   0 pd         (501) staff       (20)      799 2023-03-23 03:54:32.000000 vcsc_data_common-0.1.8/pyproject.toml
+-rw-r--r--   0 pd         (501) staff       (20)      339 2023-05-15 03:19:38.822986 vcsc_data_common-0.1.8/setup.cfg
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-15 03:19:38.812908 vcsc_data_common-0.1.8/vcsc_data_common/
+-rw-r--r--   0 pd         (501) staff       (20)      108 2023-02-22 09:07:01.000000 vcsc_data_common-0.1.8/vcsc_data_common/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-15 03:19:38.814097 vcsc_data_common-0.1.8/vcsc_data_common/ai_framework/
+-rw-r--r--   0 pd         (501) staff       (20)       48 2023-02-22 09:02:01.000000 vcsc_data_common-0.1.8/vcsc_data_common/ai_framework/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     4948 2023-03-31 09:44:29.000000 vcsc_data_common-0.1.8/vcsc_data_common/ai_framework/interval_fetching.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-15 03:19:38.820332 vcsc_data_common-0.1.8/vcsc_data_common/backtest/
+-rw-r--r--   0 pd         (501) staff       (20)     2537 2023-05-12 03:24:29.000000 vcsc_data_common-0.1.8/vcsc_data_common/backtest/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-15 03:19:38.820831 vcsc_data_common-0.1.8/vcsc_data_common/live_price_data/
+-rw-r--r--   0 pd         (501) staff       (20)     2341 2023-05-04 06:36:10.000000 vcsc_data_common-0.1.8/vcsc_data_common/live_price_data/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-15 03:19:38.821129 vcsc_data_common-0.1.8/vcsc_data_common/offline_price_data/
+-rw-r--r--   0 pd         (501) staff       (20)      880 2023-03-14 02:58:59.000000 vcsc_data_common-0.1.8/vcsc_data_common/offline_price_data/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-15 03:19:38.821400 vcsc_data_common-0.1.8/vcsc_data_common/order/
+-rw-r--r--   0 pd         (501) staff       (20)     3777 2023-05-15 03:18:50.000000 vcsc_data_common-0.1.8/vcsc_data_common/order/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-15 03:19:38.821635 vcsc_data_common-0.1.8/vcsc_data_common/portfolio_info/
+-rw-r--r--   0 pd         (501) staff       (20)     3660 2023-05-11 09:51:24.000000 vcsc_data_common-0.1.8/vcsc_data_common/portfolio_info/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-05-15 03:19:38.813726 vcsc_data_common-0.1.8/vcsc_data_common.egg-info/
+-rw-r--r--   0 pd         (501) staff       (20)      300 2023-05-15 03:19:38.000000 vcsc_data_common-0.1.8/vcsc_data_common.egg-info/PKG-INFO
+-rw-r--r--   0 pd         (501) staff       (20)      565 2023-05-15 03:19:38.000000 vcsc_data_common-0.1.8/vcsc_data_common.egg-info/SOURCES.txt
+-rw-r--r--   0 pd         (501) staff       (20)        1 2023-05-15 03:19:38.000000 vcsc_data_common-0.1.8/vcsc_data_common.egg-info/dependency_links.txt
+-rw-r--r--   0 pd         (501) staff       (20)      140 2023-05-15 03:19:38.000000 vcsc_data_common-0.1.8/vcsc_data_common.egg-info/requires.txt
+-rw-r--r--   0 pd         (501) staff       (20)       17 2023-05-15 03:19:38.000000 vcsc_data_common-0.1.8/vcsc_data_common.egg-info/top_level.txt
```

### Comparing `vcsc_data_common-0.1.7/pyproject.toml` & `vcsc_data_common-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.1.7/vcsc_data_common/ai_framework/interval_fetching.py` & `vcsc_data_common-0.1.8/vcsc_data_common/ai_framework/interval_fetching.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.1.7/vcsc_data_common/backtest/__init__.py` & `vcsc_data_common-0.1.8/vcsc_data_common/backtest/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.1.7/vcsc_data_common/live_price_data/__init__.py` & `vcsc_data_common-0.1.8/vcsc_data_common/live_price_data/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.1.7/vcsc_data_common/offline_price_data/__init__.py` & `vcsc_data_common-0.1.8/vcsc_data_common/offline_price_data/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.1.7/vcsc_data_common/order/__init__.py` & `vcsc_data_common-0.1.8/vcsc_data_common/order/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     pass
 
 
 class Order:
     def __init__(self, paper_trading_api_end_point: str):
         self.paper_trading_api_end_point = paper_trading_api_end_point
 
-    def place_mp_buy_order_with_ratio(self, username: str, portfolio_cycle_id: int, symbol: str, ratio: float, tradingDate: None):
+    def place_mp_buy_order_with_ratio(self, username: str, portfolio_cycle_id: int, symbol: str, ratio: float, tradingDate: str = None):
         logging.info('start place_mp_buy_order_with_ratio')
         url = f"{self.paper_trading_api_end_point}/order/placeOrderWithRatio"
 
         payload = json.dumps({
             "username": username,
             "symbol": symbol,
             "orderType": "MP",
@@ -35,23 +35,24 @@
                 f'place_mp_buy_order_with_ratio: http code: {response.status_code} --> {response.text}')
 
             raise OrderException('place_mp_buy_order_with_ratio api error')
 
         logging.info(
             f'place_mp_buy_order_with_ratio {username} - {portfolio_cycle_id} - {symbol} - {ratio}: ')
 
-    def place_mp_sell_order_with_ratio(self, username: str, portfolio_cycle_id: int, symbol: str, ratio: float):
+    def place_mp_sell_order_with_ratio(self, username: str, portfolio_cycle_id: int, symbol: str, ratio: float, tradingDate: str = None):
         url = f"{self.paper_trading_api_end_point}/order/placeOrderWithRatio"
 
         payload = json.dumps({
             "username": username,
             "symbol": symbol,
             "orderType": "MP",
             "ratio": ratio,
-            "side": "S"
+            "side": "S",
+            'tradingDate': tradingDate
         })
         headers = {
             'Content-Type': 'application/json'
         }
 
         response = requests.request("POST", url, headers=headers, data=payload)
```

### Comparing `vcsc_data_common-0.1.7/vcsc_data_common/portfolio_info/__init__.py` & `vcsc_data_common-0.1.8/vcsc_data_common/portfolio_info/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.1.7/vcsc_data_common.egg-info/SOURCES.txt` & `vcsc_data_common-0.1.8/vcsc_data_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

