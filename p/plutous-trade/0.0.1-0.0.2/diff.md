# Comparing `tmp/plutous_trade-0.0.1.tar.gz` & `tmp/plutous_trade-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plutous_trade-0.0.1.tar", max compression
+gzip compressed data, was "plutous_trade-0.0.2.tar", max compression
```

## Comparing `plutous_trade-0.0.1.tar` & `plutous_trade-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,30 @@
--rw-r--r--   0        0        0     1064 2023-05-16 06:32:04.597270 plutous_trade-0.0.1/LICENSE
--rw-r--r--   0        0        0       40 2023-05-16 06:32:04.597270 plutous_trade-0.0.1/README.md
--rw-r--r--   0        0        0       65 2023-05-16 06:36:17.270223 plutous_trade-0.0.1/plutous/__init__.py
--rw-r--r--   0        0        0       83 2023-05-16 06:37:00.077773 plutous_trade-0.0.1/plutous/trade/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 06:44:14.005733 plutous_trade-0.0.1/plutous/trade/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 06:44:07.605202 plutous_trade-0.0.1/plutous/trade/models/__init__.py
--rw-r--r--   0        0        0      557 2023-05-16 06:53:01.873488 plutous_trade-0.0.1/plutous/trade/models/base.py
--rw-r--r--   0        0        0      132 2023-05-16 07:14:45.401501 plutous_trade-0.0.1/plutous/trade/models/strategy.py
--rw-r--r--   0        0        0      560 2023-05-16 06:43:53.184007 plutous_trade-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 plutous_trade-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-16 06:32:04.597270 plutous_trade-0.0.2/LICENSE
+-rw-r--r--   0        0        0       40 2023-05-16 06:32:04.597270 plutous_trade-0.0.2/README.md
+-rw-r--r--   0        0        0       65 2023-05-16 06:36:17.270223 plutous_trade-0.0.2/plutous/__init__.py
+-rw-r--r--   0        0        0       83 2023-05-22 19:29:47.425201 plutous_trade-0.0.2/plutous/trade/__init__.py
+-rw-r--r--   0        0        0     3382 2023-05-16 07:55:03.221919 plutous_trade-0.0.2/plutous/trade/alembic.ini
+-rw-r--r--   0        0        0        0 2023-05-16 06:44:14.005733 plutous_trade-0.0.2/plutous/trade/app/__init__.py
+-rw-r--r--   0        0        0     1199 2023-05-22 13:52:41.032088 plutous_trade-0.0.2/plutous/trade/app/main.py
+-rw-r--r--   0        0        0      590 2023-05-22 16:03:14.229359 plutous_trade-0.0.2/plutous/trade/app/models.py
+-rw-r--r--   0        0        0        0 2023-05-16 09:19:41.262810 plutous_trade-0.0.2/plutous/trade/cli/__init__.py
+-rw-r--r--   0        0        0      565 2023-05-21 14:49:47.617177 plutous_trade-0.0.2/plutous/trade/cli/database.py
+-rw-r--r--   0        0        0      253 2023-05-16 09:53:06.465010 plutous_trade-0.0.2/plutous/trade/cli/main.py
+-rw-r--r--   0        0        0      221 2023-05-22 15:46:21.868004 plutous_trade-0.0.2/plutous/trade/enums/__init__.py
+-rw-r--r--   0        0        0       78 2023-05-21 16:59:31.441696 plutous_trade-0.0.2/plutous/trade/enums/action.py
+-rw-r--r--   0        0        0      575 2023-05-16 18:35:53.699585 plutous_trade-0.0.2/plutous/trade/enums/asset_type.py
+-rw-r--r--   0        0        0       90 2023-05-22 03:47:08.998276 plutous_trade-0.0.2/plutous/trade/enums/bot_type.py
+-rw-r--r--   0        0        0       87 2023-05-16 18:50:39.068724 plutous_trade-0.0.2/plutous/trade/enums/position_side.py
+-rw-r--r--   0        0        0      111 2023-05-21 18:52:25.169077 plutous_trade-0.0.2/plutous/trade/enums/strategy_direction.py
+-rw-r--r--   0        0        0      244 2023-05-21 15:33:24.216798 plutous_trade-0.0.2/plutous/trade/enums/strategy_type.py
+-rw-r--r--   0        0        0       38 2023-05-16 07:55:03.225919 plutous_trade-0.0.2/plutous/trade/migrations/README
+-rw-r--r--   0        0        0     2275 2023-05-22 13:26:57.883694 plutous_trade-0.0.2/plutous/trade/migrations/env.py
+-rw-r--r--   0        0        0      510 2023-05-16 07:55:03.225919 plutous_trade-0.0.2/plutous/trade/migrations/script.py.mako
+-rw-r--r--   0        0        0      159 2023-05-22 03:55:30.430494 plutous_trade-0.0.2/plutous/trade/models/__init__.py
+-rw-r--r--   0        0        0     1089 2023-05-22 15:48:07.454158 plutous_trade-0.0.2/plutous/trade/models/api_key.py
+-rw-r--r--   0        0        0      401 2023-05-22 13:39:10.362131 plutous_trade-0.0.2/plutous/trade/models/base.py
+-rw-r--r--   0        0        0      977 2023-05-22 13:31:52.932067 plutous_trade-0.0.2/plutous/trade/models/bot.py
+-rw-r--r--   0        0        0      941 2023-05-22 19:13:23.674596 plutous_trade-0.0.2/plutous/trade/models/position.py
+-rw-r--r--   0        0        0      647 2023-05-22 13:38:30.726320 plutous_trade-0.0.2/plutous/trade/models/strategy.py
+-rw-r--r--   0        0        0      968 2023-05-22 18:41:14.933111 plutous_trade-0.0.2/plutous/trade/models/trade.py
+-rw-r--r--   0        0        0      560 2023-05-22 19:29:55.381966 plutous_trade-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 plutous_trade-0.0.2/PKG-INFO
```

### Comparing `plutous_trade-0.0.1/LICENSE` & `plutous_trade-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `plutous_trade-0.0.1/pyproject.toml` & `plutous_trade-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "plutous-trade"
-version = "0.0.1"
+version = "0.0.2"
 description = "Plutous Trading Library"
 packages = [{include = "plutous"}]
 authors = ["Cheun Hong <cheunhong@plutous.io>"]
 readme = "README.md"
 license="MIT"
 classifiers = [
     "Programming Language :: Python :: 3.10",
```

### Comparing `plutous_trade-0.0.1/PKG-INFO` & `plutous_trade-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: plutous-trade
-Version: 0.0.1
+Version: 0.0.2
 Summary: Plutous Trading Library
 License: MIT
 Author: Cheun Hong
 Author-email: cheunhong@plutous.io
 Requires-Python: >=3.10,<3.11
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: plutous (>=0.0.1)
 Description-Content-Type: text/markdown
 
 # plutous-trade
 Plutous Trading Library
```

