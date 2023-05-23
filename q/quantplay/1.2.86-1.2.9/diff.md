# Comparing `tmp/quantplay-1.2.86.tar.gz` & `tmp/quantplay-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantplay-1.2.86.tar", last modified: Tue May 23 09:42:23 2023, max compression
+gzip compressed data, was "quantplay-1.2.9.tar", last modified: Tue Mar 14 05:33:14 2023, max compression
```

## Comparing `quantplay-1.2.86.tar` & `quantplay-1.2.9.tar`

### file list

```diff
@@ -1,139 +1,125 @@
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-23 09:42:23.791781 quantplay-1.2.86/
--rw-r--r--   0 ashok      (502) staff       (20)      663 2023-05-23 09:42:23.791846 quantplay-1.2.86/PKG-INFO
--rw-r--r--   0 ashok      (502) staff       (20)      494 2023-04-19 06:36:45.000000 quantplay-1.2.86/README.md
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-23 09:42:23.781638 quantplay-1.2.86/quantplay/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-23 09:42:23.782390 quantplay-1.2.86/quantplay/backtest/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/backtest/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    17605 2023-05-17 07:17:28.000000 quantplay-1.2.86/quantplay/backtest/backtest_trades.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-23 09:42:23.783957 quantplay-1.2.86/quantplay/broker/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/broker/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    10902 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/broker/angelone.py
--rw-r--r--   0 ashok      (502) staff       (20)     3738 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/broker/broker_client.py
--rw-r--r--   0 ashok      (502) staff       (20)       87 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/broker/client.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-23 09:42:23.784305 quantplay-1.2.86/quantplay/broker/finvasia_utils/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/broker/finvasia_utils/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     2576 2023-05-11 13:49:53.000000 quantplay-1.2.86/quantplay/broker/finvasia_utils/shoonya.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-23 09:42:23.784519 quantplay-1.2.86/quantplay/broker/generics/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/broker/generics/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    28749 2023-05-17 09:43:09.000000 quantplay-1.2.86/quantplay/broker/generics/broker.py
--rw-r--r--   0 ashok      (502) staff       (20)     3897 2023-05-17 07:17:28.000000 quantplay-1.2.86/quantplay/broker/iifl.py
--rw-r--r--   0 ashok      (502) staff       (20)      587 2023-05-10 06:43:57.000000 quantplay-1.2.86/quantplay/broker/iifl_xts.py
--rw-r--r--   0 ashok      (502) staff       (20)     2002 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/broker/kite_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)    31836 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/broker/motilal.py
--rw-r--r--   0 ashok      (502) staff       (20)    19618 2023-05-11 13:57:44.000000 quantplay-1.2.86/quantplay/broker/shoonya.py
--rw-r--r--   0 ashok      (502) staff       (20)      515 2023-04-19 06:37:00.000000 quantplay-1.2.86/quantplay/broker/symphony.py
--rw-r--r--   0 ashok      (502) staff       (20)    17880 2023-05-19 15:50:30.000000 quantplay-1.2.86/quantplay/broker/xts.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-23 09:42:23.785135 quantplay-1.2.86/quantplay/broker/xts_utils/
--rw-r--r--   0 ashok      (502) staff       (20)    33446 2023-04-24 08:10:10.000000 quantplay-1.2.86/quantplay/broker/xts_utils/Connect.py
--rw-r--r--   0 ashok      (502) staff       (20)     3046 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/broker/xts_utils/Exception.py
--rw-r--r--   0 ashok      (502) staff       (20)     6450 2023-05-19 15:50:30.000000 quantplay-1.2.86/quantplay/broker/xts_utils/InteractiveSocketClient.py
--rw-r--r--   0 ashok      (502) staff       (20)     9106 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/broker/xts_utils/MarketDataSocketClient.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/broker/xts_utils/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    17192 2023-05-23 09:41:25.000000 quantplay-1.2.86/quantplay/broker/zerodha.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-23 09:42:23.785228 quantplay-1.2.86/quantplay/brokerage/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/brokerage/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-23 09:42:23.785424 quantplay-1.2.86/quantplay/brokerage/angelone/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/brokerage/angelone/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    10989 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/brokerage/angelone/angel_broker.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-23 09:42:23.785617 quantplay-1.2.86/quantplay/brokerage/generics/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/brokerage/generics/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    28081 2023-04-26 18:39:03.000000 quantplay-1.2.86/quantplay/brokerage/generics/broker.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-23 09:42:23.785871 quantplay-1.2.86/quantplay/brokerage/zerodha/
--rw-r--r--   0 ashok      (502) staff       (20)    17690 2023-04-24 06:31:05.000000 quantplay-1.2.86/quantplay/brokerage/zerodha/ZBroker.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/brokerage/zerodha/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-23 09:42:23.786047 quantplay-1.2.86/quantplay/config/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/config/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     1461 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/config/qplay_config.py
--rw-r--r--   0 ashok      (502) staff       (20)     1127 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/create_sample_data.py
--rw-r--r--   0 ashok      (502) staff       (20)     1725 2023-04-19 06:37:00.000000 quantplay-1.2.86/quantplay/data_modify_script.py
--rw-r--r--   0 ashok      (502) staff       (20)     3481 2023-04-19 06:37:00.000000 quantplay-1.2.86/quantplay/date_fix.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-23 09:42:23.786255 quantplay-1.2.86/quantplay/exception/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/exception/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     2162 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/exception/exceptions.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-23 09:42:23.786474 quantplay-1.2.86/quantplay/executor/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/executor/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     6064 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/executor/strategy_executor.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-23 09:42:23.786796 quantplay-1.2.86/quantplay/indicators/
--rw-r--r--   0 ashok      (502) staff       (20)     1747 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/indicators/Indicator.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/indicators/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      455 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/indicators/atr.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-23 09:42:23.786903 quantplay-1.2.86/quantplay/model/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/model/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-23 09:42:23.787316 quantplay-1.2.86/quantplay/model/exchange/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/model/exchange/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     1472 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/model/exchange/instrument.py
--rw-r--r--   0 ashok      (502) staff       (20)     8794 2023-05-17 08:03:33.000000 quantplay-1.2.86/quantplay/model/exchange/order.py
--rw-r--r--   0 ashok      (502) staff       (20)     3238 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/model/exchange/tick.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-23 09:42:23.787525 quantplay-1.2.86/quantplay/model/strategy/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/model/strategy/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      206 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/model/strategy/strategy_response.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-23 09:42:23.787636 quantplay-1.2.86/quantplay/oms/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/oms/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-23 09:42:23.787929 quantplay-1.2.86/quantplay/order_execution/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/order_execution/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     2048 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/order_execution/execution_algorithm.py
--rw-r--r--   0 ashok      (502) staff       (20)     1281 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/order_execution/mean_price.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-23 09:42:23.788251 quantplay-1.2.86/quantplay/reporting/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/reporting/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    10780 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/reporting/strategy_report.py
--rw-r--r--   0 ashok      (502) staff       (20)     1521 2023-04-19 06:37:00.000000 quantplay-1.2.86/quantplay/reporting/visuals.py
--rw-r--r--   0 ashok      (502) staff       (20)      231 2023-04-24 06:31:05.000000 quantplay-1.2.86/quantplay/service.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-23 09:42:23.788566 quantplay-1.2.86/quantplay/services/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/services/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    18171 2023-04-19 18:27:29.000000 quantplay-1.2.86/quantplay/services/market.py
--rw-r--r--   0 ashok      (502) staff       (20)     8357 2023-05-07 17:22:15.000000 quantplay-1.2.86/quantplay/services/tradelens.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-23 09:42:23.788671 quantplay-1.2.86/quantplay/strategies/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:35:41.000000 quantplay-1.2.86/quantplay/strategies/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-23 09:42:23.788757 quantplay-1.2.86/quantplay/strategies/equities/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:48:09.000000 quantplay-1.2.86/quantplay/strategies/equities/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-23 09:42:23.788844 quantplay-1.2.86/quantplay/strategies/equities/intraday/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:48:26.000000 quantplay-1.2.86/quantplay/strategies/equities/intraday/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-23 09:42:23.788938 quantplay-1.2.86/quantplay/strategies/equities/overnight/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:49:47.000000 quantplay-1.2.86/quantplay/strategies/equities/overnight/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-23 09:42:23.789025 quantplay-1.2.86/quantplay/strategies/futures/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-24 08:54:42.000000 quantplay-1.2.86/quantplay/strategies/futures/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-23 09:42:23.789118 quantplay-1.2.86/quantplay/strategies/futures/overnight/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-24 08:54:48.000000 quantplay-1.2.86/quantplay/strategies/futures/overnight/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-23 09:42:23.789205 quantplay-1.2.86/quantplay/strategies/options/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:35:52.000000 quantplay-1.2.86/quantplay/strategies/options/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-23 09:42:23.789610 quantplay-1.2.86/quantplay/strategies/options/intraday/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:36:03.000000 quantplay-1.2.86/quantplay/strategies/options/intraday/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     1958 2022-09-14 18:05:01.000000 quantplay-1.2.86/quantplay/strategies/options/intraday/ladder.py
--rw-r--r--   0 ashok      (502) staff       (20)     2675 2022-06-25 11:41:44.000000 quantplay-1.2.86/quantplay/strategies/options/intraday/musk.py
--rw-r--r--   0 ashok      (502) staff       (20)      403 2022-09-17 07:36:48.000000 quantplay-1.2.86/quantplay/strategies/options/intraday/short_straddle.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-23 09:42:23.789806 quantplay-1.2.86/quantplay/strategy/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/strategy/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    12759 2023-05-17 07:17:28.000000 quantplay-1.2.86/quantplay/strategy/base.py
--rw-r--r--   0 ashok      (502) staff       (20)      214 2022-06-28 09:52:29.000000 quantplay-1.2.86/quantplay/strategy_run.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-23 09:42:23.790792 quantplay-1.2.86/quantplay/utils/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/utils/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      723 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/utils/config_util.py
--rw-r--r--   0 ashok      (502) staff       (20)    24181 2023-04-24 06:31:05.000000 quantplay-1.2.86/quantplay/utils/constant.py
--rw-r--r--   0 ashok      (502) staff       (20)     5433 2023-04-19 06:37:00.000000 quantplay-1.2.86/quantplay/utils/data_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)      711 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/utils/exchange.py
--rw-r--r--   0 ashok      (502) staff       (20)      517 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/utils/number_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)      458 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/utils/pickle_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)     1181 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/utils/selenium_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)     4094 2023-04-19 06:36:45.000000 quantplay-1.2.86/quantplay/utils/transaction_utils.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-23 09:42:23.782191 quantplay-1.2.86/quantplay.egg-info/
--rw-r--r--   0 ashok      (502) staff       (20)      663 2023-05-23 09:42:23.000000 quantplay-1.2.86/quantplay.egg-info/PKG-INFO
--rw-r--r--   0 ashok      (502) staff       (20)     3391 2023-05-23 09:42:23.000000 quantplay-1.2.86/quantplay.egg-info/SOURCES.txt
--rw-r--r--   0 ashok      (502) staff       (20)        1 2023-05-23 09:42:23.000000 quantplay-1.2.86/quantplay.egg-info/dependency_links.txt
--rw-r--r--   0 ashok      (502) staff       (20)      221 2023-05-23 09:42:23.000000 quantplay-1.2.86/quantplay.egg-info/requires.txt
--rw-r--r--   0 ashok      (502) staff       (20)       15 2023-05-23 09:42:23.000000 quantplay-1.2.86/quantplay.egg-info/top_level.txt
--rw-r--r--   0 ashok      (502) staff       (20)       49 2023-05-23 09:42:23.792067 quantplay-1.2.86/setup.cfg
--rw-r--r--   0 ashok      (502) staff       (20)      876 2023-05-23 09:41:51.000000 quantplay-1.2.86/setup.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-23 09:42:23.790983 quantplay-1.2.86/test/
--rw-------   0 ashok      (502) staff       (20)        0 2022-04-15 16:22:35.000000 quantplay-1.2.86/test/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-23 09:42:23.791181 quantplay-1.2.86/test/broker/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.86/test/broker/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      220 2023-04-19 06:36:45.000000 quantplay-1.2.86/test/broker/finvasia.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-23 09:42:23.791374 quantplay-1.2.86/test/executor/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.86/test/executor/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      304 2023-04-19 06:36:45.000000 quantplay-1.2.86/test/executor/strategy_executor.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-23 09:42:23.791678 quantplay-1.2.86/test/strategy/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.86/test/strategy/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      292 2023-04-19 06:36:45.000000 quantplay-1.2.86/test/strategy/base.py
--rw-r--r--   0 ashok      (502) staff       (20)     2194 2023-04-19 06:36:45.000000 quantplay-1.2.86/test/strategy/sample_strategy.py
--rw-r--r--   0 ashok      (502) staff       (20)     3302 2023-04-19 06:36:45.000000 quantplay-1.2.86/test/test_motilal.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-03-14 05:33:14.387924 quantplay-1.2.9/
+-rw-r--r--   0 ashok      (502) staff       (20)      662 2023-03-14 05:33:14.387984 quantplay-1.2.9/PKG-INFO
+-rw-r--r--   0 ashok      (502) staff       (20)      494 2022-04-17 10:54:24.000000 quantplay-1.2.9/README.md
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-03-14 05:33:14.376320 quantplay-1.2.9/quantplay/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-03-09 16:36:29.000000 quantplay-1.2.9/quantplay/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-03-14 05:33:14.377311 quantplay-1.2.9/quantplay/backtest/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-03-09 16:36:29.000000 quantplay-1.2.9/quantplay/backtest/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    17260 2023-01-19 02:56:14.000000 quantplay-1.2.9/quantplay/backtest/backtest_trades.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-03-14 05:33:14.378998 quantplay-1.2.9/quantplay/broker/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-09-14 14:42:56.000000 quantplay-1.2.9/quantplay/broker/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    10902 2023-02-18 12:07:06.000000 quantplay-1.2.9/quantplay/broker/angelone.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3738 2022-09-17 04:21:35.000000 quantplay-1.2.9/quantplay/broker/broker_client.py
+-rw-r--r--   0 ashok      (502) staff       (20)       87 2022-09-14 14:47:24.000000 quantplay-1.2.9/quantplay/broker/client.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-03-14 05:33:14.379281 quantplay-1.2.9/quantplay/broker/finvasia_utils/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-12-31 11:10:39.000000 quantplay-1.2.9/quantplay/broker/finvasia_utils/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2576 2023-02-11 04:10:25.000000 quantplay-1.2.9/quantplay/broker/finvasia_utils/shoonya.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-03-14 05:33:14.379531 quantplay-1.2.9/quantplay/broker/generics/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-09-16 14:05:50.000000 quantplay-1.2.9/quantplay/broker/generics/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    18638 2023-02-27 07:04:06.000000 quantplay-1.2.9/quantplay/broker/generics/broker.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2047 2023-01-22 16:18:04.000000 quantplay-1.2.9/quantplay/broker/kite_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)    31836 2023-02-27 07:02:13.000000 quantplay-1.2.9/quantplay/broker/motilal.py
+-rw-r--r--   0 ashok      (502) staff       (20)    16789 2023-03-14 05:32:26.000000 quantplay-1.2.9/quantplay/broker/shoonya.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2845 2023-01-30 13:09:52.000000 quantplay-1.2.9/quantplay/broker/symphony.py
+-rw-r--r--   0 ashok      (502) staff       (20)    18183 2023-02-27 07:32:47.000000 quantplay-1.2.9/quantplay/broker/zerodha.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-03-14 05:33:14.379708 quantplay-1.2.9/quantplay/brokerage/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-04-07 17:21:33.000000 quantplay-1.2.9/quantplay/brokerage/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-03-14 05:33:14.379908 quantplay-1.2.9/quantplay/brokerage/angelone/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 06:26:20.000000 quantplay-1.2.9/quantplay/brokerage/angelone/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    10989 2022-08-01 14:56:00.000000 quantplay-1.2.9/quantplay/brokerage/angelone/angel_broker.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-03-14 05:33:14.380158 quantplay-1.2.9/quantplay/brokerage/generics/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2022-03-09 16:36:29.000000 quantplay-1.2.9/quantplay/brokerage/generics/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    28033 2022-07-12 08:39:40.000000 quantplay-1.2.9/quantplay/brokerage/generics/broker.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-03-14 05:33:14.380536 quantplay-1.2.9/quantplay/brokerage/zerodha/
+-rw-r--r--   0 ashok      (502) staff       (20)    17401 2022-09-21 18:14:33.000000 quantplay-1.2.9/quantplay/brokerage/zerodha/ZBroker.py
+-rw-------   0 ashok      (502) staff       (20)        0 2022-04-07 17:21:33.000000 quantplay-1.2.9/quantplay/brokerage/zerodha/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-03-14 05:33:14.380730 quantplay-1.2.9/quantplay/config/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-04-07 17:21:33.000000 quantplay-1.2.9/quantplay/config/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1461 2022-06-22 08:09:40.000000 quantplay-1.2.9/quantplay/config/qplay_config.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1127 2022-06-15 08:16:17.000000 quantplay-1.2.9/quantplay/create_sample_data.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1724 2022-12-19 09:25:50.000000 quantplay-1.2.9/quantplay/data_modify_script.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-03-14 05:33:14.380965 quantplay-1.2.9/quantplay/exception/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-03-09 16:36:29.000000 quantplay-1.2.9/quantplay/exception/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2162 2022-10-03 07:10:49.000000 quantplay-1.2.9/quantplay/exception/exceptions.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-03-14 05:33:14.381199 quantplay-1.2.9/quantplay/executor/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2022-03-09 16:36:29.000000 quantplay-1.2.9/quantplay/executor/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     6064 2022-06-28 05:06:04.000000 quantplay-1.2.9/quantplay/executor/strategy_executor.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-03-14 05:33:14.381335 quantplay-1.2.9/quantplay/model/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-03-09 16:36:29.000000 quantplay-1.2.9/quantplay/model/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-03-14 05:33:14.381810 quantplay-1.2.9/quantplay/model/exchange/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-03-09 16:36:29.000000 quantplay-1.2.9/quantplay/model/exchange/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1472 2022-06-23 07:31:05.000000 quantplay-1.2.9/quantplay/model/exchange/instrument.py
+-rw-r--r--   0 ashok      (502) staff       (20)     8628 2023-01-09 04:21:22.000000 quantplay-1.2.9/quantplay/model/exchange/order.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3238 2022-07-12 07:44:24.000000 quantplay-1.2.9/quantplay/model/exchange/tick.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-03-14 05:33:14.382051 quantplay-1.2.9/quantplay/model/strategy/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-03-09 16:36:29.000000 quantplay-1.2.9/quantplay/model/strategy/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      206 2022-04-17 10:54:24.000000 quantplay-1.2.9/quantplay/model/strategy/strategy_response.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-03-14 05:33:14.382187 quantplay-1.2.9/quantplay/oms/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-27 04:43:46.000000 quantplay-1.2.9/quantplay/oms/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-03-14 05:33:14.382527 quantplay-1.2.9/quantplay/order_execution/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2022-03-09 16:36:29.000000 quantplay-1.2.9/quantplay/order_execution/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2048 2022-04-20 04:11:58.000000 quantplay-1.2.9/quantplay/order_execution/execution_algorithm.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1281 2022-04-19 06:42:52.000000 quantplay-1.2.9/quantplay/order_execution/mean_price.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-03-14 05:33:14.382897 quantplay-1.2.9/quantplay/reporting/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-03-09 16:36:29.000000 quantplay-1.2.9/quantplay/reporting/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    10780 2023-01-19 02:56:14.000000 quantplay-1.2.9/quantplay/reporting/strategy_report.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1510 2022-06-06 18:04:02.000000 quantplay-1.2.9/quantplay/reporting/visuals.py
+-rw-r--r--   0 ashok      (502) staff       (20)      231 2023-01-08 06:14:00.000000 quantplay-1.2.9/quantplay/service.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-03-14 05:33:14.383409 quantplay-1.2.9/quantplay/services/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-03-09 16:36:29.000000 quantplay-1.2.9/quantplay/services/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    17986 2023-01-23 02:26:35.000000 quantplay-1.2.9/quantplay/services/market.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2798 2023-01-08 06:12:37.000000 quantplay-1.2.9/quantplay/services/tradelens.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-03-14 05:33:14.383745 quantplay-1.2.9/quantplay/strategies/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:35:41.000000 quantplay-1.2.9/quantplay/strategies/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-03-14 05:33:14.383842 quantplay-1.2.9/quantplay/strategies/equities/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:48:09.000000 quantplay-1.2.9/quantplay/strategies/equities/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-03-14 05:33:14.383938 quantplay-1.2.9/quantplay/strategies/equities/intraday/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:48:26.000000 quantplay-1.2.9/quantplay/strategies/equities/intraday/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-03-14 05:33:14.384040 quantplay-1.2.9/quantplay/strategies/equities/overnight/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:49:47.000000 quantplay-1.2.9/quantplay/strategies/equities/overnight/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-03-14 05:33:14.384143 quantplay-1.2.9/quantplay/strategies/futures/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-24 08:54:42.000000 quantplay-1.2.9/quantplay/strategies/futures/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-03-14 05:33:14.384255 quantplay-1.2.9/quantplay/strategies/futures/overnight/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-24 08:54:48.000000 quantplay-1.2.9/quantplay/strategies/futures/overnight/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-03-14 05:33:14.384359 quantplay-1.2.9/quantplay/strategies/options/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:35:52.000000 quantplay-1.2.9/quantplay/strategies/options/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-03-14 05:33:14.384870 quantplay-1.2.9/quantplay/strategies/options/intraday/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:36:03.000000 quantplay-1.2.9/quantplay/strategies/options/intraday/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1958 2022-09-14 18:05:01.000000 quantplay-1.2.9/quantplay/strategies/options/intraday/ladder.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2675 2022-06-25 11:41:44.000000 quantplay-1.2.9/quantplay/strategies/options/intraday/musk.py
+-rw-r--r--   0 ashok      (502) staff       (20)      403 2022-09-17 07:36:48.000000 quantplay-1.2.9/quantplay/strategies/options/intraday/short_straddle.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-03-14 05:33:14.385114 quantplay-1.2.9/quantplay/strategy/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2022-03-09 16:36:29.000000 quantplay-1.2.9/quantplay/strategy/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    11810 2022-10-21 05:19:41.000000 quantplay-1.2.9/quantplay/strategy/base.py
+-rw-r--r--   0 ashok      (502) staff       (20)      214 2022-06-28 09:52:29.000000 quantplay-1.2.9/quantplay/strategy_run.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-03-14 05:33:14.386610 quantplay-1.2.9/quantplay/utils/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-03-09 16:36:29.000000 quantplay-1.2.9/quantplay/utils/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      723 2022-04-17 10:54:24.000000 quantplay-1.2.9/quantplay/utils/config_util.py
+-rw-r--r--   0 ashok      (502) staff       (20)    23741 2022-09-18 09:02:50.000000 quantplay-1.2.9/quantplay/utils/constant.py
+-rw-r--r--   0 ashok      (502) staff       (20)     5276 2022-08-22 16:31:03.000000 quantplay-1.2.9/quantplay/utils/data_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)      711 2022-04-17 10:54:24.000000 quantplay-1.2.9/quantplay/utils/exchange.py
+-rw-r--r--   0 ashok      (502) staff       (20)      517 2022-12-30 04:31:22.000000 quantplay-1.2.9/quantplay/utils/number_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)      458 2023-01-29 14:04:22.000000 quantplay-1.2.9/quantplay/utils/pickle_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1207 2023-01-16 02:41:32.000000 quantplay-1.2.9/quantplay/utils/selenium_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)     4094 2022-04-17 12:50:03.000000 quantplay-1.2.9/quantplay/utils/transaction_utils.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-03-14 05:33:14.377079 quantplay-1.2.9/quantplay.egg-info/
+-rw-r--r--   0 ashok      (502) staff       (20)      662 2023-03-14 05:33:14.000000 quantplay-1.2.9/quantplay.egg-info/PKG-INFO
+-rw-r--r--   0 ashok      (502) staff       (20)     2972 2023-03-14 05:33:14.000000 quantplay-1.2.9/quantplay.egg-info/SOURCES.txt
+-rw-r--r--   0 ashok      (502) staff       (20)        1 2023-03-14 05:33:14.000000 quantplay-1.2.9/quantplay.egg-info/dependency_links.txt
+-rw-r--r--   0 ashok      (502) staff       (20)      177 2023-03-14 05:33:14.000000 quantplay-1.2.9/quantplay.egg-info/requires.txt
+-rw-r--r--   0 ashok      (502) staff       (20)       15 2023-03-14 05:33:14.000000 quantplay-1.2.9/quantplay.egg-info/top_level.txt
+-rw-r--r--   0 ashok      (502) staff       (20)       49 2023-03-14 05:33:14.388194 quantplay-1.2.9/setup.cfg
+-rw-r--r--   0 ashok      (502) staff       (20)      875 2023-03-14 05:32:42.000000 quantplay-1.2.9/setup.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-03-14 05:33:14.386844 quantplay-1.2.9/test/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-04-15 16:22:35.000000 quantplay-1.2.9/test/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-03-14 05:33:14.387099 quantplay-1.2.9/test/broker/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2022-12-31 12:18:16.000000 quantplay-1.2.9/test/broker/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      220 2022-12-31 14:39:54.000000 quantplay-1.2.9/test/broker/finvasia.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-03-14 05:33:14.387368 quantplay-1.2.9/test/executor/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-04-17 06:24:33.000000 quantplay-1.2.9/test/executor/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      304 2022-04-17 10:58:40.000000 quantplay-1.2.9/test/executor/strategy_executor.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-03-14 05:33:14.387768 quantplay-1.2.9/test/strategy/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-04-15 16:23:22.000000 quantplay-1.2.9/test/strategy/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      292 2022-04-17 10:54:24.000000 quantplay-1.2.9/test/strategy/base.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2194 2022-04-20 14:52:19.000000 quantplay-1.2.9/test/strategy/sample_strategy.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3302 2022-11-15 06:12:07.000000 quantplay-1.2.9/test/test_motilal.py
```

### Comparing `quantplay-1.2.86/PKG-INFO` & `quantplay-1.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantplay
-Version: 1.2.86
+Version: 1.2.9
 Summary: This python package will be stored in AWS CodeArtifact
 Home-page: 
 Author: 
 Author-email: 
 License: MIT
 
 # Quantplay Alpha playground
```

### Comparing `quantplay-1.2.86/quantplay/backtest/backtest_trades.py` & `quantplay-1.2.9/quantplay/backtest/backtest_trades.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,18 @@
 
 
 class Backtesting:
     def __init__(self, market):
         self.market_data = []
         self.market = market
 
-    def load_data(self, symbols_by_security_type, interval, **kwargs):
+    def load_data(self, symbols_by_security_type, interval):
         self.market_data = self.market.data(
             interval=interval,
             symbols_by_security_type=symbols_by_security_type,
-            **kwargs
         )
 
         self.market_data.loc[:, "tradingsymbol"] = self.market_data.symbol
         self.market_data.loc[:, "date_only"] = self.market_data.date.dt.date
         self.market_data.loc[:, "date_only"] = pd.to_datetime(self.market_data.date_only)
 
         self.business_days_df = (
@@ -254,17 +253,14 @@
         else:
             trades.loc[:, "closing_timestamp"] = trades.exit_time
 
         interval_minutes = int(TickInterval.get_interval_seconds(interval) / 60)
         trades.loc[:, "order_timestamp"] = trades.entry_time + timedelta(
             minutes=interval_minutes
         )
-        trades.loc[:, "closing_timestamp"] = trades.closing_timestamp + timedelta(
-            minutes=interval_minutes
-        )
         trades.loc[:, "date"] = trades.original_date
         trades.loc[:, "exposure"] = trades.quantity * trades.entry_price
 
         fno_slippage = 0
         if 'fno_slippage' in args:
             fno_slippage = args['fno_slippage']
 
@@ -377,17 +373,14 @@
         return trades
 
     @staticmethod
     def apply_stoploss(trades):
 
         if "stoploss" not in trades.columns:
             return
-        minimum_stoploss = trades.stoploss.min()
-        if minimum_stoploss <= 0:
-            raise Exception(f"Invalid stoploss entry [{minimum_stoploss}] found in the trades data")
         print("Applying stoploss")
 
         trades.loc[:, "stoploss_price"] = np.where(
             trades.transaction_type == "SELL",
             Constants.round_to_tick((1 + trades.stoploss) * trades.entry_price),
             Constants.round_to_tick((1 - trades.stoploss) * trades.entry_price),
         )
```

### Comparing `quantplay-1.2.86/quantplay/broker/angelone.py` & `quantplay-1.2.9/quantplay/broker/angelone.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.86/quantplay/broker/broker_client.py` & `quantplay-1.2.9/quantplay/broker/broker_client.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.86/quantplay/broker/finvasia_utils/shoonya.py` & `quantplay-1.2.9/quantplay/broker/finvasia_utils/shoonya.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.86/quantplay/broker/generics/broker.py` & `quantplay-1.2.9/quantplay/broker/motilal.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,113 +1,166 @@
-import copy
-import math
-import random
+import hashlib
+import requests
+import json
 import time
-from collections import defaultdict
-from datetime import datetime
-from datetime import timedelta
-from threading import Lock
-
-import numpy as np
 import pandas as pd
-import io
-import os
-import zipfile
-import requests
 
-from quantplay.exception.exceptions import QuantplayOrderPlacementException
-from quantplay.utils.constant import Constants
-from quantplay.utils.exchange import Market as MarketConstants
+from quantplay.utils.constant import Constants, timeit, OrderType
+from quantplay.config.qplay_config import QplayConfig
+import getpass
+from quantplay.broker.generics.broker import Broker
+import traceback
+from quantplay.exception.exceptions import InvalidArgumentException
+import numpy as np
+import pyotp
+import math
 from quantplay.utils.number_utils import NumberUtils
+import random
+import websocket
+import _thread as thread
+import copy
+import threading
 from quantplay.utils.pickle_utils import PickleUtils
-from quantplay.utils.constant import Order, StrategyType, ExchangeName
 
-logger = Constants.logger
 
+class Motilal(Broker):
+    user_id = "motilal_user_id"
+    api_key = "motilal_api_key"
+    password = "motilal_password"
+    auth_token = "motilal_auth_token"
+    two_factor_authentication = "motilal_2FA"
+    secret_key = "motilal_secret_key"
+
+    headers = {
+        "Accept": "application/json",
+        "User-Agent": "MOSL/V.1.1.0",
+        "SourceId": "WEB",
+        "MacAddress": "00:50:56:BD:F4:0B",
+        "ClientLocalIp": "192.168.165.165",
+        "ClientPublicIp": "106.193.137.95",
+        "osname": "Ubuntu",
+        "osversion": "10.0.19041",
+        "devicemodel": "AHV",
+        "manufacturer": "DELL",
+        "productname": "Your Product Name",
+        "productversion": "Your Product Version",
+        "installedappid": "AppID",
+        "browsername": "Chrome",
+        "browserversion": "105.0"
+    }
+
+    @timeit(MetricName="Motilal:__init__")
+    def __init__(self, is_uat=False, headers=None, load_instruments=True, user_id=None, password=None, api_key=None,
+                 two_fa=None, totp=None):
+        super(Motilal, self).__init__()
+
+        self.instrument_data_by_exchange = {}
+
+        uat = ""
+        if is_uat:
+            uat = "uat"
+
+        self.url = "https://{}openapi.motilaloswal.com/rest/login/v3/authdirectapi".format(uat)
+        self.otp_url = "https://{}openapi.motilaloswal.com/rest/login/v3/resendotp".format(uat)
+        self.verify_otp_url = "https://{}openapi.motilaloswal.com/rest/login/v3/verifyotp".format(uat)
+        self.ltp_utl = "https://{}openapi.motilaloswal.com/rest/report/v1/getltpdata".format(uat)
+        self.place_order_url = "https://{}openapi.motilaloswal.com/rest/trans/v1/placeorder".format(uat)
+        self.get_profile_url = "https://{}openapi.motilaloswal.com/rest/login/v1/getprofile".format(uat)
+        self.margin_summary_url = "https://{}openapi.motilaloswal.com/rest/report/v1/getreportmarginsummary".format(uat)
+        self.modify_order_url = "https://{}openapi.motilaloswal.com/rest/trans/v2/modifyorder".format(uat)
+        self.order_book_url = "https://{}openapi.motilaloswal.com/rest/book/v1/getorderbook".format(uat)
+        self.cancel_order_url = "https://{}openapi.motilaloswal.com/rest/trans/v1/cancelorder".format(uat)
+        self.positions_url = "https://{}openapi.motilaloswal.com/rest/book/v1/getposition".format(uat)
 
-class Broker():
+        try:
+            if headers:
+                self.headers = headers
+            else:
+                self.generate_token(user_id, password, api_key, two_fa, totp)
+        except Exception as e:
+            raise e
 
-    def __init__(self):
-        self.instrument_id_to_symbol_map = dict()
-        self.instrument_id_to_exchange_map = dict()
-        self.instrument_id_to_security_type_map = dict()
-        self.exchange_symbol_to_instrument_id_map = defaultdict(dict)
-        self.order_type_sl = "SL"
-        self.nfo_exchange = "NFO"
-
-        self.orders_column_list = ['order_id', 'user_id', 'tradingsymbol', 'tag', 'average_price', 'transaction_type',
-                                   'status', 'ltp', 'exchange', 'product', 'quantity', 'filled_quantity',
-                                   'pending_quantity', 'order_timestamp']
-        self.positions_column_list = ['tradingsymbol', 'quantity', 'ltp', 'pnl', 'buy_quantity',
-                                      'sell_quantity', 'exchange', 'product', 'option_type']
-        self.trigger_pending_status = "TRIGGER PENDING"
-        self.lock = Lock()
+        try:
+            self.get_orders()
+        except Exception as e:
+            raise InvalidArgumentException("Motilal client generation failed due to invalid arguments")
 
-    def initialize_symbol_data(self, save_as=None):
-        instruments = self.instrument_data
-        instruments = instruments.to_dict('records')
-        self.symbol_data = {}
-        for instrument in instruments:
-            exchange = instrument['exchange']
-            tradingsymbol = instrument['broker_symbol']
+        if load_instruments:
+            self.load_instrument()
 
-            instrument_data = copy.deepcopy(instrument)
-            self.symbol_data["{}:{}".format(exchange, tradingsymbol)] = instrument_data
+        self.order_type_sl = "STOPLOSS"
+        self.nfo_exchange = "NSEFO"
+        self.exchange_code_map = {
+            "NFO": "NSEFO",
+            "CDS": "NSECD"
+        }
 
-        PickleUtils.save_data(self.symbol_data, save_as)
+    def update_headers(self):
+        Constants.logger.info("Updating headers")
+        quantplay_config = QplayConfig.get_config()
 
-    def initialize_broker_symbol_map(self):
-        self.broker_symbol_map = {}
-        for a in self.symbol_data:
-            self.broker_symbol_map[self.symbol_data[a]['broker_symbol']] = self.symbol_data[a]['tradingsymbol']
-        self.quantplay_symbol_map = {v: k for k, v in self.broker_symbol_map.items()}
+        auth_token = quantplay_config['DEFAULT'][Motilal.auth_token]
+        api_key = quantplay_config['DEFAULT'][Motilal.api_key]
+        user_id = quantplay_config['DEFAULT'][Motilal.user_id]
+
+        self.headers['vendorinfo'] = user_id
+        self.headers['Authorization'] = auth_token
+        self.headers['ApiKey'] = api_key
+
+        self.user_id = user_id
+
+    @timeit(MetricName="Motilal:initialize_expiry_fields")
+    def initialize_expiry_fields(self):
+        self.instrument_data.loc[:, 'tradingsymbol'] = self.instrument_data.scripshortname
+        self.instrument_data.loc[:, 'expiry'] = pd.to_datetime(self.instrument_data.expirydate + 315513000,
+                                                                  unit='s')
+
+        self.instrument_data.loc[:, "expiry_year"] = self.instrument_data["expiry"].dt.strftime("%y").astype(str)
+        self.instrument_data.loc[:, "month"] = self.instrument_data["expiry"].dt.strftime("%b").str.upper()
 
-    def round_to_tick(self, number):
-        return round(number * 20) / 20
+        self.instrument_data.loc[:, "month_number"] = self.instrument_data["expiry"].dt.strftime("%m").astype(
+            float).astype(str)
+        self.instrument_data.loc[:, 'month_number'] = np.where(self.instrument_data.month_number == 'nan',
+                                                                  np.nan,
+                                                                  self.instrument_data.month_number.str.split(
+                                                                      ".").str[0]
+                                                                  )
 
-    def populate_instruments(self, instruments):
-        """Fetches instruments for all exchanges from the broker
-        and stores them in the member attributes.
-        """
-        Constants.logger.info("populating instruments")
-        for instrument in instruments:
-            exchange, symbol, instrument_id = (
-                instrument.exchange,
-                instrument.symbol,
-                instrument.instrument_id,
-            )
-            self.instrument_id_to_symbol_map[instrument_id] = symbol
-            self.instrument_id_to_exchange_map[instrument_id] = exchange
-            self.instrument_id_to_security_type_map[
-                instrument_id
-            ] = instrument.security_type()
-            self.exchange_symbol_to_instrument_id_map[exchange][symbol] = instrument_id
+        self.instrument_data.loc[:, "week_option_prefix"] = np.where(
+            self.instrument_data.month_number.astype(float) >= 10,
+            self.instrument_data.month.str[0] + self.instrument_data["expiry"].dt.strftime("%d").astype(str),
+            self.instrument_data.month_number + self.instrument_data["expiry"].dt.strftime("%d").astype(str),
+        )
+
+        self.instrument_data.loc[:, "next_expiry"] = self.instrument_data.expiry + pd.DateOffset(days=7)
 
+    @timeit(MetricName="Motilal:add_quantplay_fut_tradingsymbol")
     def add_quantplay_fut_tradingsymbol(self):
         seg_condition = [
-            ((self.instrument_data["instrument"].str.contains("FUT")) & (
-                    self.instrument_data.instrument != "OPTFUT"))
+            ((self.instrument_data["instrumentname"].str.contains("FUT")) & (
+                        self.instrument_data.instrumentname != "OPTFUT"))
         ]
 
         tradingsymbol = [
             self.instrument_data.tradingsymbol + self.instrument_data.expiry_year + self.instrument_data.month + "FUT"
         ]
 
         self.instrument_data.loc[:, "tradingsymbol"] = np.select(
             seg_condition, tradingsymbol, default=self.instrument_data.tradingsymbol
         )
 
+    @timeit(MetricName="Motilal:add_quantplay_opt_tradingsymbol")
     def add_quantplay_opt_tradingsymbol(self):
-        seg_condition = (self.instrument_data["strike_price"] > 0)
+        seg_condition = (self.instrument_data["strikeprice"] > 0)
         weekly_option_condition = (
                 (self.instrument_data.expiry.dt.month == self.instrument_data.next_expiry.dt.month) & (
-                self.instrument_data.exchange == "NFO"))
+            self.instrument_data.exchangename.isin(["NFO", "NSEFO", "NSECD"])))
         month_option_condition = (
                 (self.instrument_data.expiry.dt.month != self.instrument_data.next_expiry.dt.month) | (
-                self.instrument_data.exchange == "MCX"))
+                    self.instrument_data.exchangename == "MCX"))
 
         self.instrument_data.loc[:, "tradingsymbol"] = np.where(
             seg_condition,
             self.instrument_data.tradingsymbol + self.instrument_data.expiry_year,
             self.instrument_data.tradingsymbol
         )
 
@@ -122,539 +175,598 @@
             self.instrument_data.tradingsymbol + self.instrument_data.month,
             self.instrument_data.tradingsymbol
         )
 
         self.instrument_data.loc[:, "tradingsymbol"] = np.where(
             seg_condition,
             self.instrument_data.tradingsymbol +
-            self.instrument_data.strike_price.astype(float).astype(str).str.split(".").str[0],
+            self.instrument_data.strikeprice.astype(float).astype(str).str.split(".").str[0],
             self.instrument_data.tradingsymbol
         )
 
+        self.instrument_data.loc[:, 'after_point'] = (self.instrument_data.strikeprice * 100).astype(int)
+        self.instrument_data.loc[:, 'after_point'] = (self.instrument_data.after_point % 100).astype(str).apply(
+            lambda x: x.rstrip('0'))
+        self.instrument_data.loc[:, 'tradingsymbol'] = np.where(self.instrument_data.after_point.str.len() > 0,
+                                                                   self.instrument_data.tradingsymbol + "." + self.instrument_data.after_point,
+                                                                   self.instrument_data.tradingsymbol)
+
         self.instrument_data.loc[:, "tradingsymbol"] = np.where(
             seg_condition,
-            self.instrument_data.tradingsymbol + self.instrument_data.option_type,
+            self.instrument_data.tradingsymbol + self.instrument_data.optiontype,
             self.instrument_data.tradingsymbol
         )
 
-    def get_df_from_zip(self, url):
-        response = requests.get(url, timeout=10)
-        z = zipfile.ZipFile(io.BytesIO(response.content))
-
-        directory = '/tmp/'
-        z.extractall(path=directory)
-        file_name = url.split(".txt")[0].split("/")[-1]
-        os.system('cp /tmp/{}.txt /tmp/{}.csv'.format(file_name, file_name))
-        time.sleep(2)
-        return pd.read_csv('/tmp/{}.csv'.format(file_name))
+    @timeit(MetricName="Motilal:load_file_by_url")
+    def load_file_by_url(self, exchange):
+        data_url = "https://openapi.motilaloswal.com/getscripmastercsv?name={}".format(exchange)
+        df = pd.read_csv(data_url)
+        self.instrument_data_by_exchange[exchange] = df
 
-    def initialize_expiry_fields(self):
-        self.instrument_data.loc[:, 'tradingsymbol'] = self.instrument_data.instrument_symbol
-        self.instrument_data.loc[:, 'expiry'] = pd.to_datetime(self.instrument_data.instrument_expiry)
-
-        self.instrument_data.loc[:, "expiry_year"] = self.instrument_data["expiry"].dt.strftime("%y").astype(str)
-        self.instrument_data.loc[:, "month"] = self.instrument_data["expiry"].dt.strftime("%b").str.upper()
+    @timeit(MetricName="Motilal:load_instrument")
+    def load_instrument(self):
+        try:
+            self.symbol_data = PickleUtils.load_data("motilal_instruments")
+            Constants.logger.info("[LOADING_INSTRUMENTS] loading data from cache")
+        except Exception as e:
+            Constants.logger.info("[LOADING_INSTRUMENTS] loading data from server")
+            exchanges = ["NSEFO", "MCX", "NSECD", "NSE"]
+            threads = []
+            for exchange in exchanges:
+                th = threading.Thread(target=self.load_file_by_url, args=(exchange,))
+                th.start()
+                threads.append(th)
+            for thread in threads:
+                thread.join()
+
+            instrument_file_FO = self.instrument_data_by_exchange["NSEFO"]
+            instrument_file_MCX = self.instrument_data_by_exchange["MCX"]
+            instrument_file_CDS = self.instrument_data_by_exchange["NSECD"]
+            instrument_file_CDS = instrument_file_CDS[instrument_file_CDS.instrumentname.isin(["OPTCUR", "FUTCUR"])]
+            instrument_file_EQ = self.instrument_data_by_exchange["NSE"]
+            instrument_file_EQ = instrument_file_EQ[instrument_file_EQ['scripname'].str.contains(" EQ")]
+            instrument_file_EQ.loc[:, 'expiry'] = 0
+
+            self.instrument_data = pd.concat([instrument_file_CDS, instrument_file_MCX, instrument_file_FO,
+                                              instrument_file_EQ])
+
+            self.initialize_expiry_fields()
+            self.add_quantplay_opt_tradingsymbol()
+            self.add_quantplay_fut_tradingsymbol()
 
-        self.instrument_data.loc[:, "month_number"] = self.instrument_data["expiry"].dt.strftime("%m").astype(
-            float).astype(str)
-        self.instrument_data.loc[:, 'month_number'] = np.where(self.instrument_data.month_number == 'nan',
-                                                               np.nan,
-                                                               self.instrument_data.month_number.str.split(
-                                                                   ".").str[0]
-                                                               )
+            self.initialize_symbol_data()
 
-        self.instrument_data.loc[:, "week_option_prefix"] = np.where(
-            self.instrument_data.month_number.astype(float) >= 10,
-            self.instrument_data.month.str[0] + self.instrument_data["expiry"].dt.strftime("%d").astype(str),
-            self.instrument_data.month_number + self.instrument_data["expiry"].dt.strftime("%d").astype(str),
-        )
 
-        self.instrument_data.loc[:, "next_expiry"] = self.instrument_data.expiry + pd.DateOffset(days=7)
+        self.quantplay_symbol_map = {}
+        for a in self.symbol_data:
+            self.quantplay_symbol_map[self.symbol_data[a]['tradingsymbol']] = self.symbol_data[a]['scripname']
 
-    def execute_order_v2(self, order):
-        start_time = datetime.now()
-        tradingsymbol = order['tradingsymbol']
-        exchange = order['exchange']
-        trigger_price = order['trigger_price']
-        transaction_type = order['transaction_type']
-        if order['validity'] is not None and order['trigger_price'] is not None:
-            while True:
-                self.lock.acquire()
-                try:
-                    ltp = self.get_ltp(exchange, tradingsymbol)
-                except Exception as e:
-                    Constants.logger.error("[GET_LTP_FAILED] with exception {}".format(e))
-                time.sleep(.5)
-                self.lock.release()
-                if (transaction_type == "SELL" and trigger_price > ltp) or (
-                        transaction_type == "BUY" and trigger_price < ltp):
-                    logger.info(
-                        "[EXECUTING_ORDER] ltp {} crossed trigger price {} for {}".format(ltp, trigger_price, order))
-                    self.execute_order(tradingsymbol=order['tradingsymbol'],
-                                       exchange=order['exchange'],
-                                       quantity=order['quantity'],
-                                       product=order['product'],
-                                       tag=order['tag'],
-                                       stoploss=order['stoploss'],
-                                       transaction_type=order['transaction_type'],
-                                       order_type=order['order_type'])
-                    return
-                current_time = datetime.now()
-                if (current_time - start_time).seconds > order['validity']:
-                    Constants.logger.info("[ORDER_VALIDITY_EXPIRED] order [{}]".format(order))
-                    return
-
-    def execute_order(self, tradingsymbol=None, exchange=None, quantity=None, order_type=None, transaction_type=None,
-                      stoploss=None, tag=None, product=None, price=None):
-        upper_circuit = None
-        if price is None:
-            live_data = self.live_data(exchange=exchange, tradingsymbol=tradingsymbol)
-            price = live_data['ltp']
-            upper_circuit = live_data['upper_circuit']
-            trade_price = copy.deepcopy(price)
-        try:
-            if stoploss != None:
-                if transaction_type == "SELL":
-                    sl_transaction_type = "BUY"
-                    sl_trigger_price = self.round_to_tick(price * (1 + stoploss))
-
-                    if exchange == self.nfo_exchange:
-                        price = sl_trigger_price * 1.05
-                    elif exchange == "NSE":
-                        price = sl_trigger_price * 1.01
-                    else:
-                        raise Exception("{} not supported for trading".format(exchange))
-
-                    sl_price = self.round_to_tick(price)
-                elif transaction_type == "BUY":
-                    sl_transaction_type = "SELL"
-                    sl_trigger_price = self.round_to_tick(price * (1 - stoploss))
-
-                    if exchange == self.nfo_exchange:
-                        price = sl_trigger_price * .95
-                    elif exchange == "NSE":
-                        price = sl_trigger_price * .99
-                    else:
-                        raise Exception("{} not supported for trading".format(exchange))
+    @timeit(MetricName="Motilal:initialize_symbol_data")
+    def initialize_symbol_data(self):
+        instruments = self.instrument_data
+        instruments = instruments.to_dict('records')
+        self.symbol_data = {}
+        for instrument_data in instruments:
+            exchange = instrument_data['exchangename']
+            tradingsymbol = instrument_data['scripname']
 
-                    sl_price = self.round_to_tick(price)
-                else:
-                    raise Exception("Invalid transaction_type {}".format(transaction_type))
+            instrument_data['lot_size'] = instrument_data['marketlot']
+            self.symbol_data["{}:{}".format(exchange, tradingsymbol)] = instrument_data
 
-                if upper_circuit != None and sl_price > upper_circuit:
-                    raise Exception(f"[PRICE_BREACHED] {sl_price} is above upper circuit price [{upper_circuit}]")
+        PickleUtils.save_data(self.symbol_data, "motilal_instruments")
 
-                stoploss_order_id = self.place_order(tradingsymbol=tradingsymbol,
-                                                     exchange=exchange,
-                                                     quantity=quantity,
-                                                     order_type=self.order_type_sl,
-                                                     transaction_type=sl_transaction_type,
-                                                     tag=tag, product=product, price=sl_price,
-                                                     trigger_price=sl_trigger_price)
-
-                if stoploss_order_id is None:
-                    Constants.logger.error(
-                        "[ORDER_REJECTED] tradingsymbol {}".format(tradingsymbol))
-                    raise QuantplayOrderPlacementException("Order reject for {}".format(tradingsymbol))
-
-            if order_type == "MARKET":
-                trade_price = 0
-
-            response = self.place_order(tradingsymbol=tradingsymbol, exchange=exchange, quantity=quantity,
-                                        order_type=order_type, transaction_type=transaction_type, tag=tag,
-                                        product=product, price=trade_price)
-            return response
-        except Exception as e:
-            raise e
 
-    """
-            Input  : quantplay symbol
-            Output : broker symbol
-        """
 
     def get_symbol(self, symbol):
-        return symbol
-
-    """
-        Input  : quantplay exchange
-        Output : broker exchange
-    """
+        if symbol not in self.quantplay_symbol_map:
+            return symbol
+        return self.quantplay_symbol_map[symbol]
 
     def get_order_type(self, order_type):
+        if order_type == OrderType.sl:
+            return "STOPLOSS"
         return order_type
 
     def get_exchange(self, exchange):
+        if exchange in self.exchange_code_map:
+            return self.exchange_code_map[exchange]
+
         return exchange
 
-    def live_data(self, exchange, tradingsymbol):
-        return {
-            'ltp': self.get_ltp(exchange, tradingsymbol),
-            'upper_circuit': None,
-            'lower_circuit': None
-        }
+    def get_product(self, product):
+        return "NORMAL"
 
     def place_order_quantity(self, quantity, tradingsymbol, exchange):
         lot_size = self.get_lot_size(exchange, tradingsymbol)
         quantity_in_lots = int(quantity / lot_size)
 
-        return quantity_in_lots * lot_size
-
-    def get_product(self, product):
-        return product
-
-    def get_lot_size(self, exchange, tradingsymbol):
-        try:
-            return int(self.symbol_data["{}:{}".format(exchange, tradingsymbol)]['lot_size'])
-        except Exception as e:
-            logger.error("[GET_LOT_SIZE] unable to get lot size for {} {}".format(exchange, tradingsymbol))
-            raise e
-
-    def filter_orders(self, orders, tag=None, status=None):
-        if tag:
-            orders = orders[orders.tag == tag]
-
-        if status:
-            orders = orders[orders.status == status]
-
-        return orders
-
-    def option_symbol(self, underlying_symbol, expiry_date, strike_price, type):
-        option_symbol = MarketConstants.INDEX_SYMBOL_TO_DERIVATIVE_SYMBOL_MAP[underlying_symbol]
-        option_symbol += expiry_date.strftime('%y')
-
-        month_number = str(int(expiry_date.strftime("%m")))
-        monthly_option_prefix = expiry_date.strftime("%b").upper()
-
-        if int(month_number) >= 10:
-            week_option_prefix = monthly_option_prefix[0]
-        else:
-            week_option_prefix = month_number
-        week_option_prefix += expiry_date.strftime("%d")
-
-        next_expiry = expiry_date + timedelta(days=7)
-
-        if next_expiry.month != expiry_date.month:
-            option_symbol += monthly_option_prefix
-        else:
-            option_symbol += week_option_prefix
-
-        option_symbol += str(int(strike_price))
-        option_symbol += type
-
-        return option_symbol
-
-    def exit_all_trigger_orders(self, tag="ALL", symbol_contains=None, order_timestamp=None):
-        stoploss_orders = self.orders()
-        stoploss_orders = stoploss_orders[stoploss_orders.status == "TRIGGER PENDING"]
-
-        if len(stoploss_orders) == 0:
-            Constants.logger.info("All stoploss orders have been already closed")
-            return
-
-        if tag != "ALL":
-            stoploss_orders = stoploss_orders[stoploss_orders.tag == tag]
+        return quantity_in_lots
 
-        if symbol_contains is not None:
-            stoploss_orders = stoploss_orders[stoploss_orders['tradingsymbol'].str.contains(symbol_contains)]
+    def generate_token(self, user_id, password, api_key, two_fa, totp):
+        current_totp = pyotp.TOTP(totp).now()
+        Constants.logger.info("TOTP is {}".format(current_totp))
+        # initializing string
+        str = "{}{}".format(password, api_key)
+        result = hashlib.sha256(str.encode())
+
+        data = {
+            "userid": user_id,
+            "password": result.hexdigest(),
+            "2FA": two_fa,
+            "totp": current_totp
+        }
 
-        if order_timestamp is not None:
-            stoploss_orders.loc[:, 'order_timestamp'] = stoploss_orders.order_timestamp.apply(lambda x: x.replace(second=0))
-            stoploss_orders = stoploss_orders[stoploss_orders.order_timestamp == order_timestamp]
+        self.headers['ApiKey'] = api_key
+        self.headers['vendorinfo'] = user_id
+        response = requests.post(self.url, headers=self.headers, data=json.dumps(data))
+
+        resp_json = response.json()
+        Constants.logger.info("login response {}".format(resp_json))
+        self.headers['Authorization'] = resp_json['AuthToken']
+        self.user_id = user_id
+
+    def send_otp(self):
+        response = requests.post(self.otp_url, headers=self.headers).json()
+        Constants.logger.info(response)
+        return response
 
-        if len(stoploss_orders) == 0:
-            Constants.logger.info("All stoploss orders have been already closed")
-            return
+    def verify_otp(self, otp):
+        data = {
+            "otp": otp
+        }
+        response = requests.post(self.verify_otp_url, headers=self.headers, data=json.dumps(data)).json()
+        Constants.logger.info(response)
+        return response
 
-        orders_to_close = list(stoploss_orders.order_id.unique())
+    def get_ltp(self, exchange=None, tradingsymbol=None):
+        tradingsymbol = self.get_symbol(tradingsymbol)
+        data = {
+            "userid": self.user_id,
+            "exchange": exchange,
+            "scripcode": self.symbol_data["{}:{}".format(exchange, tradingsymbol)]['scripcode']
+        }
 
-        stoploss_orders = stoploss_orders.to_dict('records')
-        for stoploss_order in stoploss_orders:
-            exchange = stoploss_order['exchange']
-            tradingsymbol = stoploss_order['tradingsymbol']
+        response = requests.post(self.ltp_utl, headers=self.headers, data=json.dumps(data))
+        Constants.logger.info("[GET_LTP_RESPONSE] response {}".format(response.json()))
+        return response.json()["data"]["ltp"] / 100.0
+
+    def get_orders(self, order_status=None, order_type=None):
+        response = (requests.post(self.order_book_url, headers=self.headers)).json()
+        if response["status"] == "ERROR":
+            Constants.logger.info("Error while fetching order book [{}]".format(response["message"]))
+            raise Exception(response["message"])
+        orders = response["data"]
 
-            if exchange == "NFO":
-                stoploss_order['order_type'] = "MARKET"
-                stoploss_order['price'] = 0
-            else:
-                ltp = self.get_ltp(exchange, tradingsymbol)
-                stoploss_order['order_type'] = "LIMIT"
-                stoploss_order['price'] = self.round_to_tick(ltp)
+        if order_status:
+            orders = [a for a in orders if a['orderstatus'] == order_status]
 
-            self.modify_order(stoploss_order)
-            time.sleep(.1)
+        if order_type:
+            orders = [a for a in orders if a['ordertype'] == order_type]
 
-        self.modify_orders_till_complete(orders_to_close)
-        Constants.logger.info("All order have been closed successfully")
+        return orders
 
-    def square_off_all(self, dry_run=True, contains=None, sleep_time=0.1):
-        positions = self.positions()
-        if len(positions) == 0:
+    def get_positions(self):
+        response = (requests.post(self.positions_url, headers=self.headers)).json()
+        if response["status"] == "ERROR":
+            Constants.logger.info("Error while fetching order book [{}]".format(response["message"]))
+            raise Exception(response["message"])
+
+        positions = response["data"]
+
+        return positions
+
+    def square_off_all(self, dry_run=True, strike=None, sleep_time=0.1, tag=None):
+        positions = self.get_positions()
+        if positions == None:
             print("Positions are already squared off")
             return
 
-        if contains:
-            positions = positions[positions.tradingsymbol.str.contains(contains)]
+        positions = pd.DataFrame(positions)
+        if strike:
+            positions = positions[positions.symbol.str.contains(strike)]
 
-        positions.loc[:, 'net_quantity'] = positions.buy_quantity - positions.sell_quantity
-        positions = positions[positions.net_quantity != 0]
-        positions.loc[:, 'transaction_type'] = np.where(positions.quantity < 0,
-                                                        "BUY",
-                                                        "SELL")
-        positions.loc[:, 'lot_size'] = positions.apply(lambda x: self.get_lot_size(x.exchange, x.tradingsymbol), axis=1)
-        positions.loc[:, 'price'] = positions.apply(lambda x: self.get_ltp(x['exchange'], x['tradingsymbol']), axis=1)
+        positions.loc[:, 'net_quantity'] = positions.buyquantity - positions.sellquantity
+        positions = positions[['exchange', 'symbol', 'net_quantity']].sort_values("net_quantity")
 
         positions = positions.to_dict('records')
         orders_to_close = []
         for position in positions:
-            quantity = abs(position['net_quantity'])
             exchange = position['exchange']
-            tradingsymbol = position['tradingsymbol']
-            transaction_type = position['transaction_type']
+            symbol = position['symbol']
+            quantity = position['net_quantity']
 
-            quantity_in_lots = int(quantity / self.get_lot_size(exchange, tradingsymbol))
+            transaction_type = "SELL"
+            if quantity == 0 or exchange != "NSEFO":
+                continue
+            elif quantity < 0:
+                transaction_type = "BUY"
+
+            quantity = abs(quantity)
+            quantity_in_lots = int(quantity / self.get_lot_size(exchange, symbol))
 
             split_into = int(math.ceil(quantity_in_lots / 25))
             split_array = NumberUtils.split(abs(quantity_in_lots), abs(split_into))
 
             for q in split_array:
                 orders_to_close.append(
                     {
-                        'symbol': tradingsymbol,
+                        'symbol': symbol,
                         'exchange': exchange,
                         'transaction_type': transaction_type,
-                        'quantity_in_lots': q,
-                        'product': position['product'],
-                        'price': position['price']
+                        'quantity_in_lots': q
                     })
 
         random.shuffle(orders_to_close)
         orders_to_close = sorted(orders_to_close, key=lambda d: d['transaction_type'])
-        orders_placed = []
         for order in orders_to_close:
-            quantity = int(order['quantity_in_lots'] * self.get_lot_size(order['exchange'], order['symbol']))
-            print(order['symbol'], order['exchange'], order['transaction_type'], quantity, order['product'],
-                  order['price'])
+            print(order['symbol'], order['exchange'], order['transaction_type'], order['quantity_in_lots'])
             if dry_run == False:
-                order_id = self.place_order(tradingsymbol=order['symbol'],
-                                            exchange=order['exchange'],
-                                            quantity=quantity,
-                                            order_type="LIMIT",
-                                            transaction_type=order['transaction_type'],
-                                            tag="killall",
-                                            product=order['product'],
-                                            price=order['price'])
-                orders_placed.append(str(order_id))
+                self.place_order(tradingsymbol=order['symbol'],
+                                 exchange=order['exchange'],
+                                 quantity=order['quantity_in_lots'],
+                                 order_type="MARKET",
+                                 transaction_type=order['transaction_type'],
+                                 tag="square-off",
+                                 product="NORMAL",
+                                 price=0)
                 time.sleep(sleep_time)
-        if dry_run == False:
-            self.modify_orders_till_complete(orders_placed)
 
-        return orders_to_close
+    def modify_price(self, order_id, price, trigger_price=None, order_type=None):
+        orders = pd.DataFrame(self.get_orders())
+        orders = orders.to_dict('records')
+        order_found = False
+
+        for order in orders:
+            if order['uniqueorderid'] == order_id:
+                order_found = True
+                break
 
-    def square_off_by_tag(self, tag, dry_run=True, sleep_time=0.05):
-        self.exit_all_trigger_orders(tag=tag)
-        orders = self.orders(tag=tag)
-
-        if len(orders) == 0:
-            logger.info(f"All positions with tag {tag} are already squared-off for {self.profile()}")
-        orders.loc[:, 'exit_quantity'] = np.where(orders.transaction_type == "BUY",
-                                                  -orders.filled_quantity,
-                                                  orders.filled_quantity)
-        exit_orders = orders.groupby('tradingsymbol').agg({'exit_quantity': 'sum',
-                                                           'exchange': 'first',
-                                                           'product': 'first'
-                                                           }).reset_index()
+        if order_found == False:
+            Constants.logger.error("[ORDER_NOT_FOUND] invalid modify request for {}".format(order_id))
+            return
 
-        orders_to_close = []
-        exit_orders = exit_orders[exit_orders.exit_quantity != 0]
-        positions = exit_orders.to_dict('records')
-        for position in positions:
-            exchange = position['exchange']
-            tradingsymbol = position['tradingsymbol']
-            quantity = position['exit_quantity']
+        order['price'] = price
+        if trigger_price != None:
+            order['triggerprice'] = trigger_price
 
-            transaction_type = "SELL"
-            if quantity == 0:
-                continue
-            elif quantity > 0:
-                transaction_type = "BUY"
+        if order["ordertype"] == "Stop Loss":
+            order["ordertype"] = "STOPLOSS"
 
-            quantity = abs(quantity)
-            quantity_in_lots = int(quantity / self.get_lot_size(exchange, tradingsymbol))
+        self.modify_order(order)
 
-            split_into = int(math.ceil(quantity_in_lots / 25))
-            split_array = NumberUtils.split(abs(quantity_in_lots), abs(split_into))
+    def modify_orders_till_complete(self, orders_placed):
+        modification_count = {}
+        while 1:
+            time.sleep(10)
+            orders = pd.DataFrame(self.get_orders())
+            orders = orders[orders.uniqueorderid.isin(orders_placed)]
 
-            for q in split_array:
-                orders_to_close.append(
-                    {
-                        'tradingsymbol': tradingsymbol,
-                        'exchange': exchange,
-                        'transaction_type': transaction_type,
-                        'quantity_in_lots': q,
-                        'product': position['product']
-                    })
+            orders = orders[~orders.orderstatus.isin(["Error", "Traded", "Cancel", "Rejected"])]
 
-        random.shuffle(orders_to_close)
-        orders_to_close = sorted(orders_to_close, key=lambda d: d['transaction_type'])
-        for order in orders_to_close:
-            tradingsymbol = order['tradingsymbol']
-            exchange = order['exchange']
-            transaction_type = order['transaction_type']
-            product = order['product']
-            quantity = order['quantity_in_lots'] * self.get_lot_size(exchange, tradingsymbol)
-            quantity = self.place_order_quantity(quantity, tradingsymbol, exchange)
+            if len(orders) == 0:
+                Constants.logger.info("ALL orders have be completed")
+                break
 
-            print(tradingsymbol, exchange, transaction_type, quantity)
-            if dry_run == False:
-                self.place_order(tradingsymbol=tradingsymbol,
-                                 exchange=exchange,
-                                 quantity=quantity,
-                                 order_type="MARKET",
-                                 transaction_type=transaction_type,
-                                 tag=tag,
-                                 product=product,
-                                 price=0)
-                time.sleep(sleep_time)
+            orders = orders.to_dict('records')
+            for order in orders:
+                order_id = order['uniqueorderid']
 
-        return orders_to_close
+                ltp = self.get_ltp(order['exchange'], order['symbol'])
+                order['price'] = ltp
+                self.modify_order(order)
 
-    def add_ltp(self, orders):
-        orders.loc[:, 'exchange_symbol'] = orders.exchange + ":" + orders.tradingsymbol
+                if order_id not in modification_count:
+                    modification_count[order_id] = 1
+                else:
+                    modification_count[order_id] += 1
 
-        all_symbols = list(orders.exchange_symbol.unique())
-        symbol_ltp = {}
-        for exchange_symbol in all_symbols:
-            ltp = self.get_ltp(exchange_symbol.split(":")[0], exchange_symbol.split(":")[1])
-            symbol_ltp[exchange_symbol] = ltp
-        orders.loc[:, 'ltp'] = orders['exchange_symbol'].map(symbol_ltp)
+                time.sleep(.1)
 
-    def risk_analysis(self):
-        positions = self.positions()
-        positions.loc[:, 'net_quantity'] = positions.buy_quantity - positions.sell_quantity
-        positions.loc[:, 'premium'] = positions.net_quantity * positions.ltp
+                if modification_count[order_id] > 5:
+                    order['ordertype'] = "MARKET"
+                    order['price'] = 0
+                    Constants.logger.info("Placing MARKET order [{}]".format(order))
+                    self.modify_order(order)
 
-        bank_nifty = positions[positions.tradingsymbol.str.contains("BANKNIFTY")]
-        t_df = bank_nifty.groupby('option_type').premium.sum().reset_index()
-        t_df.loc[:, 'segment'] = t_df.option_type
-        t_df = t_df[['segment', 'premium']]
-        response = {
-            "banknifty_premium": t_df
+    def exit_all_trigger_orders(self, tag="ALL",
+                                symbol_contains=None):
+
+        stoploss_orders = self.get_orders(order_status="Confirm", order_type="Stop Loss")
+
+        if len(stoploss_orders) == 0:
+            print("All stoploss orders have been already closed")
+            return
+
+        stoploss_orders = pd.DataFrame(stoploss_orders)
+        if tag != "ALL":
+            stoploss_orders = stoploss_orders[stoploss_orders.tag == tag]
+
+        if symbol_contains is not None:
+            stoploss_orders = stoploss_orders[stoploss_orders['symbol'].str.contains(symbol_contains)]
+
+        if len(stoploss_orders) == 0:
+            print("All stoploss orders have been already closed")
+            return
+
+        orders_to_close = list(stoploss_orders.uniqueorderid.unique())
+
+        stoploss_orders = stoploss_orders.to_dict('records')
+        for stoploss_order in stoploss_orders:
+            exchange = stoploss_order['exchange']
+            tradingsymbol = stoploss_order['symbol']
+
+            if exchange == "NFO":
+                stoploss_order['ordertype'] = "MARKET"
+                stoploss_order['price'] = 0
+            else:
+                ltp = self.get_ltp(exchange, tradingsymbol)
+                stoploss_order['ordertype'] = "LIMIT"
+                stoploss_order['price'] = self.round_to_tick(ltp)
+
+            self.modify_order(stoploss_order)
+            time.sleep(.1)
+
+        self.modify_orders_till_complete(orders_to_close)
+        print("All order have been closed successfully")
+
+    def modify_order(self, order):
+        data = {
+            "uniqueorderid": order['uniqueorderid'],
+            "newordertype": order['ordertype'].upper(),
+            "neworderduration": order['orderduration'].upper(),
+            "newquantityinlot": int(order['totalqtyremaining'] / order['lotsize']),
+            # "newdisclosedquantity": 0,
+            "newprice": order['price'],
+            "newtriggerprice": order['triggerprice'],
+            "qtytradedtoday": order['qtytradedtoday'],
+            "lastmodifiedtime": order['lastmodifiedtime']
         }
 
-        fin_nifty = positions[positions.tradingsymbol.str.contains("FINNIFTY")]
-        t_df = fin_nifty.groupby('option_type').premium.sum().reset_index()
-        t_df.loc[:, 'segment'] = t_df.option_type
-        t_df = t_df[['segment', 'premium']]
-        response["finnifty_premium"] = t_df
+        if 'exchange' in order and order['exchange'] == "MCX":
+            data['newquantityinlot'] = int(order['totalqtyremaining'])
 
-        return response
+        try:
+            Constants.logger.info("[MODIFYING_ORDER] order [{}]".format(data))
+            response = requests.post(self.modify_order_url, headers=self.headers, data=json.dumps(data)).json()
+            Constants.logger.info("[MODIFY_ORDER_RESPONSE] {}".format(response))
+        except Exception as e:
+            exception_message = "[ORDER_MODIFICATION_FAILED] for {} failed with exception {}".format(
+                order['uniqueorderid'],
+                e)
+            Constants.logger.error("{}".format(exception_message))
+
+    def cancel_order(self, unique_order_id):
+        data = {
+            "uniqueorderid": unique_order_id
+        }
 
-    def add_transaction_charges(self, orders, cm_charges=0.0003, fo_charges=20):
-        orders.loc[:, 'sell_value'] = np.where(orders.transaction_type == "SELL",
-                                               orders.average_price * orders.quantity,
-                                               0)
-        orders.loc[:, 'buy_value'] = np.where(orders.transaction_type == "BUY",
-                                              orders.average_price * orders.quantity,
-                                              0)
-
-        orders.loc[:, 'product'] = np.where(orders.exchange == ExchangeName.nse, "MIS", "NRML")
-        orders.loc[:, 'security_type'] = np.where(orders.exchange == ExchangeName.nse, "EQ", "OPT")
-
-        charges_condition = [
-            (orders["product"] == "MIS")
-            & (orders["exchange"] == ExchangeName.nse),
-            (orders["product"] == "CNC")
-            & (orders["exchange"] == ExchangeName.nse),
-            (orders["exchange"] == ExchangeName.nfo)
-            & (orders["security_type"] == "FUT"),
-            (orders["exchange"] == ExchangeName.nfo)
-            & (orders["security_type"] == "OPT"),
-        ]
+        try:
+            Constants.logger.info("Cancelling order [{}]".format(unique_order_id))
+            response = requests.post(self.cancel_order_url, headers=self.headers, data=json.dumps(data)).json()
+            Constants.logger.info("Cancel order response [{}]".format(response))
+        except Exception as e:
+            exception_message = "[ORDER_CANCELLATION_FAILED] unique_order_id {} exception {}".format(unique_order_id,
+                                                                                                     e)
+            Constants.logger.error(exception_message)
+
+    def get_profile(self):
+        response = requests.post(self.get_profile_url, headers=self.headers,
+                                 data=json.dumps({'Clientcode': self.headers['vendorinfo']})).json()
+        if response['status'] == "ERROR":
+            raise Exception(response['message'])
+
+        return response['data']
+
+    def margin_summary(self):
+        response = requests.post(self.margin_summary_url, headers=self.headers,
+                                 data=json.dumps({'Clientcode': self.headers['vendorinfo']})).json()
+        if response['status'] == "ERROR":
+            raise Exception(response['message'])
+
+        return response['data']
+
+    def place_order(self, tradingsymbol=None, exchange=None, quantity=None, order_type=None, transaction_type=None,
+                    tag=None, product=None, price=None, trigger_price=None):
+        data = {
+            "exchange": exchange,
+            "symboltoken": self.symbol_data["{}:{}".format(exchange, tradingsymbol)]['scripcode'],
+            "buyorsell": transaction_type,
+            "ordertype": order_type,
+            "producttype": product,
+            "orderduration": "DAY",
+            "price": price,
+            "triggerprice": trigger_price,
+            "quantityinlot": quantity,
+            "disclosedquantity": 0,
+            "amoorder": "N",
+            "algoid": "",
+            "tag": tag
+        }
+        try:
+            Constants.logger.info("[PLACING_ORDER] {}".format(json.dumps(data)))
+            response = requests.post(self.place_order_url, headers=self.headers, data=json.dumps(data)).json()
+            Constants.logger.info("[PLACE_ORDER_RESPONSE] {} input {}".format(response, json.dumps(data)))
+            if response['status'] == "ERROR":
+                raise Exception(response['message'])
+            return response['uniqueorderid']
+        except Exception as e:
+            exception_message = "Order placement failed with error [{}]".format(str(e))
+            print(exception_message)
 
-        brokerage_charges_choices = [
-            cm_charges * orders.quantity * orders.average_price,
-            0,
-            fo_charges,
-            fo_charges,
-        ]
+    def on_message(self, ws, order):
+        try:
+            order = json.loads(order)
+            print(order)
 
-        orders.loc[:, Order.brokerage_charges] = np.select(
-            charges_condition, brokerage_charges_choices, default=0
-        )
+            order['placed_by'] = self.user_id
+            order['tag'] = self.user_id
+            order['order_id'] = order['orderid']
+            order['exchange_order_id'] = order['order_id']
+            order['transaction_type'] = order['transactiontype']
+            order['quantity'] = int(order['quantity'])
+            order['order_type'] = order['ordertype']
 
-        stt_charges_choices = [
-            0.00025 * (orders.sell_value),
-            0.001 * (orders.quantity * orders.average_price),
-            0.000125 * (orders.sell_value),
-            0.000625 * (orders.sell_value),
-        ]
+            if order['exchange'] == "NFO":
+                order["tradingsymbol"] = self.symbol_map[order["tradingsymbol"]]
 
-        orders.loc[:, Order.stt_charges] = np.select(
-            charges_condition, stt_charges_choices, default=0
-        )
+            if order['order_type'] == "STOPLOSS_LIMIT":
+                order['order_type'] = "SL"
 
-        exchange_charges_choices = [
-            0.0000325 * (orders.quantity * orders.average_price),
-            0.0000325 * (orders.quantity * orders.average_price),
-            0.000019 * (orders.quantity * orders.average_price),
-            0.00053 * (orders.quantity * orders.average_price),
-        ]
+            if 'triggerprice' in order and order['triggerprice'] != 0:
+                order['trigger_price'] = float(order['triggerprice'])
+            else:
+                order['trigger_price'] = None
 
-        orders.loc[:, Order.exchange_transaction_charges] = np.select(
-            charges_condition, exchange_charges_choices, default=0
-        )
+            if order["status"] == "trigger pending":
+                order["status"] = "TRIGGER PENDING"
+            elif order["status"] == "cancelled":
+                order["status"] = "CANCELLED"
+            elif order["status"] == "open":
+                order["status"] = "OPEN"
+            elif order["status"] == "complete":
+                order["status"] = "COMPLETE"
 
-        stamp_charges_choices = [
-            0.00003 * (orders.buy_value),
-            0.00015 * (orders.buy_value),
-            0.00002 * (orders.buy_value),
-            0.00003 * (orders.buy_value),
-        ]
+            # self.order_updates.put(order)
+            print("Final order {}".format(order))
+        except Exception as e:
+            Constants.logger.error("[ORDER_UPDATE_PROCESSING_FAILED] {}".format(e))
+        print(json.dumps(order))
 
-        orders.loc[:, Order.stamp_charges] = np.select(
-            charges_condition, stamp_charges_choices, default=0
-        )
+    def on_error(self, ws, error):
+        print(error)
 
-        orders.loc[:, Order.gst_charges] = (
-                0.18 * (orders[Order.exchange_transaction_charges] + orders[Order.brokerage_charges])
-        )
+    def on_close(self, ws):
+        print("### closed ###")
 
-        orders.loc[:, Order.total_charges] = (
-                orders[Order.stt_charges]
-                + orders[Order.exchange_transaction_charges]
-                + orders[Order.stamp_charges]
-                + orders[Order.gst_charges]
-                + orders[Order.brokerage_charges]
-        )
+    def on_open(self, ws):
+        def run(*args):
+            for i in range(300000):
+                time.sleep(1)
+                print({
+                    "actiontype": "TradeSubscribe",
+                    "clientid": self.headers['vendorinfo']
+                })
+                ws.send(json.dumps({
+                    "actiontype": "TradeSubscribe",
+                    "clientid": self.headers['vendorinfo']
+                }))
+            time.sleep(1)
+            ws.close()
+            print("thread terminating...")
+
+        thread.start_new_thread(run, ())
+
+    def stream_order_data(self):
+        api_key = self.headers['ApiKey']
+        auth_token = self.headers['Authorization']
+        client_id = self.headers['vendorinfo']
+
+        root_url = "wss://openapi.motilaloswal.com/ws"
+        ws_url = "{}?clientid={}&authtoken={}&apikey={}".format(root_url, client_id, auth_token, api_key)
+
+        websocket.enableTrace(False)
+        print(ws_url)
+        ws = websocket.WebSocketApp(ws_url,
+                                    on_message=self.on_message,
+                                    on_error=self.on_error)
+        ws.on_open = self.on_open
+        ws.run_forever()
 
-        return orders
+    def account_summary(self):
+        response = {
+            'margin_used': 0
+        }
 
-    def modify_orders_till_complete(self, orders_placed, sleep_time=10, max_modification_count=5):
-        modification_count = {}
-        while 1:
-            time.sleep(sleep_time)
-            orders = self.orders()
+        margin_summary = self.margin_summary()
+        for margin_particular in margin_summary:
+            if margin_particular['srno'] == 103:
+                response['margin_available'] = margin_particular['amount']
+            if margin_particular['srno'] in [301, 321, 340, 360]:
+                response['margin_used'] += margin_particular['amount']
 
-            orders = orders[orders.order_id.isin(orders_placed)]
-            orders = orders[~orders.status.isin(["REJECTED", "CANCELLED", "COMPLETE"])]
+        response['pnl'] = self.positions().pnl.sum()
+        return response
 
-            if len(orders) == 0:
-                Constants.logger.info("ALL orders have been completed")
-                break
+    def profile(self):
+        api_response = requests.post(self.get_profile_url, headers=self.headers,
+                                     data=json.dumps({'Clientcode': self.headers['vendorinfo']})).json()
+        if api_response['status'] == "ERROR":
+            raise Exception(api_response['message'])
 
-            orders = orders.to_dict('records')
-            for order in orders:
-                order_id = order['order_id']
+        api_response = api_response['data']
+        response = {
+            'user_id': api_response['clientcode'],
+            'full_name': api_response['name'],
+            'segments': api_response['exchanges']
+        }
 
-                ltp = self.get_ltp(order['exchange'], order['tradingsymbol'])
-                self.modify_order(order_id=order["order_id"], price=ltp)
+        return response
 
-                if order_id not in modification_count:
-                    modification_count[order_id] = 1
-                else:
-                    modification_count[order_id] += 1
+    def positions(self):
+        response = (requests.post(self.positions_url, headers=self.headers)).json()
+        if response["status"] == "ERROR":
+            Constants.logger.info("Error while fetching order book [{}]".format(response["message"]))
+            raise Exception(response["message"])
+
+        positions = response["data"]
+
+        if positions is None or len(positions) == 0:
+            return pd.DataFrame(columns=self.positions_column_list)
+
+        positions = pd.DataFrame(positions)
+        positions.loc[:, 'tradingsymbol'] = positions.symbol
+
+        positions.loc[:, 'ltp'] = positions.LTP
+        positions.loc[:, 'pnl'] = positions.sellamount - positions.buyamount
+        positions.loc[:, 'pnl'] += (positions.buyquantity - positions.sellquantity)*positions.ltp
+        positions.loc[:, 'quantity'] = positions.buyquantity - positions.sellquantity
+        positions.rename(
+            columns={
+                "productname": "product",
+                "sellquantity": "sell_quantity",
+                "buyquantity": "buy_quantity",
+                "optiontype": "option_type"
+            }, inplace=True)
+        return positions[self.positions_column_list]
+
+    def orders(self, tag=None):
+        response = (requests.post(self.order_book_url, headers=self.headers)).json()
+        if response["status"] == "ERROR":
+            Constants.logger.info("Error while fetching order book [{}]".format(response["message"]))
+            raise Exception(response["message"])
+        orders = response["data"]
+        orders = pd.DataFrame(orders)
 
-                time.sleep(.1)
+        positions = self.positions()
+        if len(positions) == 0 or len(orders) == 0:
+            return pd.DataFrame(columns=self.orders_column_list)
+
+        orders.loc[:, 'tradingsymbol'] = orders.symbol
+        orders = pd.merge(orders, positions[['tradingsymbol', 'ltp']],
+                          how="left",
+                          left_on=['tradingsymbol'],
+                          right_on=['tradingsymbol'])
+
+        orders.rename(
+            columns={
+                'clientid': 'user_id',
+                "LTP": 'ltp',
+                'buyorsell': 'transaction_type',
+                "averageprice": "average_price",
+                "orderid" : "order_id",
+                "orderstatus" : "status",
+                "entrydatetime" : "order_timestamp",
+                "orderqty" : "quantity",
+                "totalqtytraded" : "filled_quantity",
+                "totalqtyremaining" : "pending_quantity"
+            }, inplace=True)
+        orders.loc[:, 'product'] = orders.ordercategory
+
+        orders = orders[self.orders_column_list]
+        orders.loc[:, 'pnl'] = orders.ltp * orders.filled_quantity - orders.average_price * orders.filled_quantity
+        orders.loc[:, 'pnl'] = np.where(orders.transaction_type == "SELL", -orders.pnl, orders.pnl)
+
+        if tag:
+            orders = orders[orders.tag == tag]
+
+        return orders
 
-                if modification_count[order_id] > max_modification_count:
-                    Constants.logger.info("Placing MARKET order [{}]".format(order))
-                    self.modify_order(order_id=order["order_id"], price=0, order_type="MARKET")
```

### Comparing `quantplay-1.2.86/quantplay/broker/kite_utils.py` & `quantplay-1.2.9/quantplay/broker/kite_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 import time
 import traceback
 
 from retrying import retry
+import getpass
 from quantplay.utils.selenium_utils import Selenium
+from quantplay.config.qplay_config import QplayConfig
 import pyotp
 
 class KiteUtils():
     zerodha_username = "zerodha_username"
     zerodha_password = "zerodha_password"
     zeordha_totp_unique_id = "zerodha_totp_unique_id"
 
     @staticmethod
     @retry(wait_exponential_multiplier=1000, wait_exponential_max=10000, stop_max_attempt_number=3)
     def get_request_token(api_key=None, user_id=None, password=None, totp=None):
-    
         try:
             browser = Selenium.get_browser()
 
             # TODO api should be fetched from configuration
 
             kite_url = "https://kite.trade/connect/login?api_key={}&v=3".format(api_key)
             print("Kite Url {}".format(kite_url))
             browser.get(kite_url)
             time.sleep(5)
 
-
             user_id_element = browser.find_element("xpath", '//*[@id="container"]/div/div/div[2]/form/div[1]/input')
             password_element = browser.find_element("xpath", '//*[@id="container"]/div/div/div[2]/form/div[2]/input')
 
             user_id_element.send_keys(user_id)
             password_element.send_keys(password)
 
             login_attempt = browser.find_element("xpath", '//*[@id="container"]/div/div/div[2]/form/div[4]/button')
             login_attempt.submit()
             time.sleep(5)
 
-            kite_pin = browser.find_element("xpath", '/html/body/div[1]/div/div[2]/div[1]/div[2]/div/div[2]/form/div[1]/input')
+            kite_pin = browser.find_element("xpath", '//*[@id="container"]/div/div/div[2]/form/div[2]/input')
             kite_pin.send_keys(pyotp.TOTP(totp).now())
             time.sleep(3)
             # login_attempt = browser.find_element("xpath", '//*[@id="container"]/div/div/div[2]/form/div[3]/button')
             # login_attempt.submit()
             # time.sleep(1)
 
             url = browser.current_url
```

### Comparing `quantplay-1.2.86/quantplay/broker/shoonya.py` & `quantplay-1.2.9/quantplay/broker/shoonya.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 
         self.set_attributes(response)
 
         if load_instruments:
             self.load_instrument()
 
         self.order_type_sl = "SL-LMT"
-        self.trigger_pending_status = "TRIGGER_PENDING"
 
     def set_attributes(self, response):
         self.email = response['email']
         self.user_id = response['actid']
         self.full_name = response['uname']
 
     def load_instrument(self):
@@ -231,38 +230,16 @@
         return self.api.get_order_book()
 
     def get_ltp(self, exchange, tradingsymbol):
         tradingsymbol = self.get_symbol(tradingsymbol)
         token = self.symbol_data["{}:{}".format(exchange, tradingsymbol)]['Token']
         return float(self.api.get_quotes(exchange, str(token))['lp'])
 
-    def live_data(self, exchange, tradingsymbol):
-        tradingsymbol = self.get_symbol(tradingsymbol)
-        token = self.symbol_data["{}:{}".format(exchange, tradingsymbol)]['Token']
-        data = self.api.get_quotes(exchange, str(token))
-        return {
-            'ltp' : float(data['lp']),
-            'upper_circuit' : float(data['uc']),
-            'lower_circuit' : float(data['lc'])
-        }
-
     @retry(wait_exponential_multiplier=3000, wait_exponential_max=10000, stop_max_attempt_number=3)
     def modify_order(self, data):
-        if 'order_id' in data:
-            data['norenordno'] = data['order_id']
-        if 'exchange' in data:
-            data['exch'] = data['exchange']
-        if 'tradingsymbol' in data:
-            data['tsym'] = data['tradingsymbol']
-        if 'order_type' in data:
-            data['prctyp'] = data['order_type']
-        if 'quantity' in data:
-            data['qty'] = data['quantity']
-        if 'price' in data:
-            data['prc'] = data['price']
         try:
             logger.info("Modifying order [{}] new price [{}]".format(data['norenordno'], data['prc']))
             response = self.api.modify_order(orderno=data['norenordno'],
                                              exchange=data['exch'],
                                              tradingsymbol=data['tsym'],
                                              newprice_type=data['prctyp'],
                                              newquantity=data['qty'],
@@ -304,17 +281,17 @@
 
             if len(orders) == 0:
                 Constants.logger.info("ALL orders have been completed")
                 break
 
             orders = orders.to_dict('records')
             for order in orders:
-                order_id = order['norenordno']
+                order_id = order['order_id']
 
-                ltp = self.get_ltp(order['exch'], order['tsym'])
+                ltp = self.get_ltp(order['exchange'], order['tradingsymbol'])
                 order['prc'] = ltp
                 self.modify_order(order)
 
                 if order_id not in modification_count:
                     modification_count[order_id] = 1
                 else:
                     modification_count[order_id] += 1
@@ -371,17 +348,15 @@
 
         positions.loc[:, 'buy_quantity'] = positions.buy_quantity.astype(int)
         positions.loc[:, 'sell_quantity'] = positions.sell_quantity.astype(int)
         positions.loc[:, 'quantity'] = positions.buy_quantity - positions.sell_quantity
 
         return positions[self.positions_column_list]
 
-    def add_transaction_charges(self, orders):
-        return super(FinvAsia, self).add_transaction_charges(orders, cm_charges=0, fo_charges=0)
-    def orders(self, tag=None, status=None):
+    def orders(self, tag=None):
         orders = pd.DataFrame(self.api.get_order_book())
         positions = self.positions()
         if len(orders) == 0:
             return pd.DataFrame(columns=self.orders_column_list)
 
         orders.loc[:, 'tradingsymbol'] = orders.tsym
         orders = pd.merge(orders, positions[['tradingsymbol', 'ltp']],
@@ -406,21 +381,18 @@
             }, inplace=True)
 
         orders = orders[self.orders_column_list]
         orders.loc[:, 'filled_quantity'] = orders.filled_quantity.astype(float)
         orders.loc[:, 'average_price'] = orders.average_price.astype(float)
         orders.loc[:, 'pnl'] = orders.ltp * orders.filled_quantity - orders.average_price * orders.filled_quantity
         orders.loc[:, 'pnl'] = np.where(orders.transaction_type == "S", -orders.pnl, orders.pnl)
-        orders.loc[:, 'order_timestamp'] = pd.to_datetime(orders.order_timestamp, format='%H:%M:%S %d-%m-%Y')
-
-        orders = self.filter_orders(orders, status=status, tag=tag)
+        orders.loc[:, 'order_timestamp'] = pd.to_datetime(orders.order_timestamp)
 
-        orders.transaction_type = orders.transaction_type.replace(
-            ["S", "B"], ["SELL", "BUY"]
-        )
+        if tag:
+            orders = orders[orders.tag == tag]
 
         return orders
 
     def account_summary(self):
         margins = self.api.get_limits()
 
         pnl = 0
@@ -435,48 +407,8 @@
         margin_available = float(margins['cash']) + float(margins['payin']) - float(margins['marginused'])
         response = {
             'margin_used': float(margins['marginused']),
             'total_balance' : float(margins['cash']),
             'margin_available': margin_available,
             'pnl': pnl
         }
-        return response
-
-    def exit_all_trigger_orders(self, tag="ALL", symbol_contains=None):
-        stoploss_orders = self.orders(status=self.trigger_pending_status)
-
-        if len(stoploss_orders) == 0:
-            Constants.logger.info("All stoploss orders have been already closed")
-            return
-
-        stoploss_orders = pd.DataFrame(stoploss_orders)
-
-        if tag != "ALL":
-            stoploss_orders = stoploss_orders[stoploss_orders.tag == tag]
-
-        if symbol_contains is not None:
-            stoploss_orders = stoploss_orders[stoploss_orders['tradingsymbol'].str.contains(symbol_contains)]
-
-        if len(stoploss_orders) == 0:
-            Constants.logger.info("All stoploss orders have been already closed")
-            return
-
-        orders_to_close = list(stoploss_orders.order_id.unique())
-
-        stoploss_orders = stoploss_orders.to_dict('records')
-        for stoploss_order in stoploss_orders:
-            exchange = stoploss_order['exchange']
-            tradingsymbol = stoploss_order['tradingsymbol']
-
-            if exchange == "NFO":
-                stoploss_order['order_type'] = self.get_order_type("MARKET")
-                stoploss_order['price'] = 0
-            else:
-                ltp = self.get_ltp(exchange, tradingsymbol)
-                stoploss_order['order_type'] = self.get_order_type("LIMIT")
-                stoploss_order['price'] = self.round_to_tick(ltp)
-
-            self.modify_order(stoploss_order)
-            time.sleep(.1)
-
-        self.modify_orders_till_complete(orders_to_close)
-        Constants.logger.info("All order have been closed successfully")
+        return response
```

### Comparing `quantplay-1.2.86/quantplay/broker/zerodha.py` & `quantplay-1.2.9/quantplay/broker/zerodha.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,22 +14,21 @@
 import math
 from quantplay.utils.number_utils import NumberUtils
 import random
 from kiteconnect import KiteTicker
 from quantplay.exception.exceptions import InvalidArgumentException
 from quantplay.utils.pickle_utils import PickleUtils
 
-
 class Zerodha(Broker):
     stoploss = 'stoploss'
     zerodha_api_key = "zerodha_api_key"
     zerodha_api_secret = "zerodha_api_secret"
     zerodha_wrapper = "zerodha_wrapper"
 
-    @timeit(MetricName="Zerodha:__init__")
+    @timeit(MetricName="Motilal:__init__")
     def __init__(self, wrapper=None, user_id=None, api_key=None, api_secret=None, password=None, totp=None):
         try:
             if wrapper:
                 self.set_wrapper(wrapper)
             else:
                 self.generate_token(user_id, api_key, api_secret, password, totp)
         except Exception as e:
@@ -59,14 +58,15 @@
                 exchange = instrument['exchange']
                 tradingsymbol = instrument['tradingsymbol']
                 self.symbol_data["{}:{}".format(exchange, tradingsymbol)] = instrument
 
             PickleUtils.save_data(self.symbol_data, "zerodha_instruments")
             Constants.logger.info("[LOADING_INSTRUMENTS] loading data from server")
 
+
     def set_username(self, username):
         self.username = username
 
     def get_username(self):
         return self.username
 
     def on_ticks(self, kws, ticks):
@@ -116,20 +116,56 @@
     @retry(wait_exponential_multiplier=3000, wait_exponential_max=10000, stop_max_attempt_number=3)
     def get_orders(self, status=None):
         orders = self.wrapper.orders()
         if status:
             orders = [a for a in orders if a['status'] == status]
         return orders
 
+    def exit_all_trigger_orders(self, tag="ALL", symbol_contains=None):
+        stoploss_orders = self.get_orders("TRIGGER PENDING")
+
+        if len(stoploss_orders) == 0:
+            Constants.logger.info("All stoploss orders have been already closed")
+            return
+
+        stoploss_orders = pd.DataFrame(stoploss_orders)
+        if tag != "ALL":
+            stoploss_orders = stoploss_orders[stoploss_orders.tag == tag]
+
+        if symbol_contains is not None:
+            stoploss_orders = stoploss_orders[stoploss_orders['tradingsymbol'].str.contains(symbol_contains)]
+
+        if len(stoploss_orders) == 0:
+            Constants.logger.info("All stoploss orders have been already closed")
+            return
+
+        orders_to_close = list(stoploss_orders.order_id.unique())
+
+        stoploss_orders = stoploss_orders.to_dict('records')
+        for stoploss_order in stoploss_orders:
+            exchange = stoploss_order['exchange']
+            tradingsymbol = stoploss_order['tradingsymbol']
+
+            if exchange == "NFO":
+                stoploss_order['order_type'] = "MARKET"
+                stoploss_order['price'] = 0
+            else:
+                ltp = self.get_ltp(exchange, tradingsymbol)
+                stoploss_order['order_type'] = "LIMIT"
+                stoploss_order['price'] = self.round_to_tick(ltp)
+
+            self.modify_order(stoploss_order)
+            time.sleep(.1)
+
+        self.modify_orders_till_complete(orders_to_close)
+        Constants.logger.info("All order have been closed successfully")
+
     @retry(wait_exponential_multiplier=3000, wait_exponential_max=10000, stop_max_attempt_number=3)
     def modify_order(self, data):
         try:
-            data['variety'] = 'regular'
-            if "trigger_price" not in data:
-                data["trigger_price"] = None
             Constants.logger.info("Modifying order [{}] new price [{}]".format(data['order_id'], data['price']))
             response = self.wrapper.modify_order(order_id=data['order_id'],
                                                  variety=data['variety'],
                                                  price=data['price'],
                                                  trigger_price=data['trigger_price'],
                                                  order_type=data['order_type'])
             return response
@@ -359,22 +395,15 @@
 
     def positions(self):
         positions = pd.DataFrame(self.wrapper.positions()['net'])
 
         if len(positions) == 0:
             return pd.DataFrame(columns=self.positions_column_list)
 
-        positions.loc[:, 'exchange_symbol'] = positions.exchange + ":" + positions.tradingsymbol
-        symbols = positions.exchange_symbol.unique().tolist()
-        symbol_ltps = self.get_ltps(symbols)
-
-        positions.loc[:, 'ltp'] = positions.exchange_symbol.apply(lambda x: symbol_ltps[x]['last_price'])
-        positions.loc[:, 'pnl'] = positions.sell_value - positions.buy_value
-        positions.loc[:, 'pnl'] += (positions.quantity) * positions.ltp
-
+        positions.loc[:, 'ltp'] = positions.last_price
         positions.loc[:, 'option_type'] = np.where("PE" == positions.tradingsymbol.str[-2:], "PE", "CE")
         positions.loc[:, 'option_type'] = np.where(positions.exchange != "NFO", None, positions.option_type)
         return positions[self.positions_column_list]
 
     def orders(self, tag=None):
         orders = pd.DataFrame(self.wrapper.orders())
 
@@ -401,12 +430,12 @@
             orders = orders[orders.tag == tag]
 
         return orders
 
     def account_summary(self):
         margins = self.wrapper.margins()
         response = {
-            'margin_used': float(margins['equity']['utilised']['debits']),
-            'margin_available': float(margins['equity']['available']['live_balance']),
-            'pnl': float(self.positions().pnl.sum())
+            'margin_used': margins['equity']['utilised']['debits'],
+            'margin_available': margins['equity']['available']['live_balance'],
+            'pnl': self.positions().pnl.sum()
         }
         return response
```

### Comparing `quantplay-1.2.86/quantplay/brokerage/angelone/angel_broker.py` & `quantplay-1.2.9/quantplay/brokerage/angelone/angel_broker.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.86/quantplay/brokerage/generics/broker.py` & `quantplay-1.2.9/quantplay/brokerage/generics/broker.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,29 +70,29 @@
 
         for tick_interval in self.tick_intervals:
             self.ongoing_tick_updates[tick_interval] = {}
             self.ongoing_tick_interval_time[tick_interval] = None
             self.last_updated_interval_tick[tick_interval] = None
             self.prev_tick_volume[tick_interval] = {}
 
-    def load_historical_market_feed(self, interval_max_days):
+    def load_historical_market_feed(self, days):
         instrument_data_by_interval = defaultdict(list)
 
         for instrument_id in self.strategy_instruments:
             symbol = self.instrument_id_to_symbol_map[instrument_id]
             security_type = self.instrument_id_to_security_type_map[instrument_id]
 
             end_date = datetime.now()
             end_date = end_date.replace(second=0, microsecond=0)
 
-            start_date = end_date - timedelta(days=20)
+            start_date = end_date - timedelta(days=days)
             start_date = start_date.replace(minute=0, hour=0)
 
             response = self.get_historical_data(
-                instrument_id, start_date=start_date, end_date=end_date, interval_max_days=interval_max_days
+                instrument_id, start_date=start_date, end_date=end_date
             )
             for interval, data in response.items():
                 if len(data) > 0:
                     data = self.add_today_candles(data, symbol)
                     data.loc[:, "security_type"] = security_type
                     instrument_data_by_interval[interval].append(data)
                 else:
@@ -105,15 +105,15 @@
         for interval, df_list in instrument_data_by_interval.items():
             self.live_market_df_by_interval[interval] = pd.concat(df_list).reset_index(
                 drop=True
             )
 
         self.reset_market_df_index()
         for interval in self.live_market_df_by_interval:
-            self.live_market_df_by_interval[interval].to_csv(
+            self.live_market_df_by_interval["minute"].to_csv(
                 f"/tmp/live_feed_{interval}.csv"
             )
 
     def add_today_candles(self, data, symbol):
         """Adds todays empty candles for the given interval to the data"""
         current_time = datetime.now()
         unique_times = data.date.dt.time.sort_values().unique()
```

### Comparing `quantplay-1.2.86/quantplay/brokerage/zerodha/ZBroker.py` & `quantplay-1.2.9/quantplay/brokerage/zerodha/ZBroker.py`

 * *Files 3% similar despite different names*

```diff
@@ -382,28 +382,22 @@
     def get_historical_data_from_kite(
         self, instrument, start_date, end_date, interval, continuous=False
     ):
         return self.kite.historical_data(
             instrument, start_date, end_date, interval, continuous=continuous
         )
 
-    def get_historical_data(self, instrument, start_date, end_date, interval_max_days=None):
+    def get_historical_data(self, instrument, start_date, end_date):
         data_by_interval = dict()
 
         for interval in self.tick_intervals:
-            if interval_max_days != None:
-                start_date = end_date - timedelta(days=interval_max_days[interval])
-                start_date = start_date.replace(minute=0, hour=0)
-
             if interval == "5minute":
                 days_diff = 100
             elif interval == "minute":
                 days_diff = 60
-            elif interval == "15minute":
-                days_diff = 60
             elif interval == "day":
                 days_diff = 2000
             else:
                 raise Exception("interval {} not whitelisted".format(interval))
 
             time_diff = timedelta(days=days_diff)
```

### Comparing `quantplay-1.2.86/quantplay/config/qplay_config.py` & `quantplay-1.2.9/quantplay/config/qplay_config.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.86/quantplay/create_sample_data.py` & `quantplay-1.2.9/quantplay/create_sample_data.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.86/quantplay/data_modify_script.py` & `quantplay-1.2.9/quantplay/data_modify_script.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,30 +33,30 @@
     df = df[["date", "open", "high", "low", "close", "volume", "symbol"]]
 
     print("saving file {}".format(file_name))
     df.sort_values(["date"]).reset_index(drop=True).to_csv(
         "~/.quantplay/NSE_OPT/minute/{}".format(file_name), index=False
     )
 
-dir_name = "/Users/ashok/Documents/stock_option_data"
+dir_name = "/Users/ashok/Downloads/stock-options-data/2022"
 file_paths = {}
 for path, currentDirectory, files in os.walk(dir_name):
     for file in files:
         if "csv" in os.path.join(path, file):
             file_location = os.path.join(path, file)
 
             if file not in file_paths:
                 file_paths[file] = [file_location]
             else:
                 file_paths[file].append(file_location)
 
 
 threads = []
 for file_name in file_paths:
-    if 'NIFTY201' not in file_name:
+    if 'NIFTY' in file_name:
         continue
 
     th = threading.Thread(target=convert_file, args=(file_paths, file_name, ))
     th.start()
 
     threads.append(th)
     if len(threads) > 100:
```

### Comparing `quantplay-1.2.86/quantplay/exception/exceptions.py` & `quantplay-1.2.9/quantplay/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.86/quantplay/executor/strategy_executor.py` & `quantplay-1.2.9/quantplay/executor/strategy_executor.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.86/quantplay/model/exchange/instrument.py` & `quantplay-1.2.9/quantplay/model/exchange/instrument.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.86/quantplay/model/exchange/order.py` & `quantplay-1.2.9/quantplay/model/exchange/order.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,15 +132,14 @@
         self.transaction_type = trade["transaction_type"]
 
         # TODO CRITICAL
         self.price = None
         self.trigger_price = None
         self.validity = None
         self.order_timestamp = None
-        self.exit_time = None
 
         if "stoploss" in trade:
             self.stoploss = float(trade["stoploss"])
         else:
             self.stoploss = None
 
         if "price" in trade:
@@ -155,16 +154,14 @@
             self.squareoff = None
 
         if "trigger_price" in trade:
             self.trigger_price = Constants.round_to_tick(float(trade["trigger_price"]))
 
         if "order_timestamp" in trade:
             self.order_timestamp = trade["order_timestamp"]
-        if "exit_time" in trade:
-            self.exit_time = trade["exit_time"]
 
         if "lot_size" in trade and not pd.isna(trade["lot_size"]):
             self.lot_size = trade["lot_size"]
 
     def get_child_order(self):
         """Returns the child order for this QuantplayExchangeOrder"""
         if self.is_child_order:
@@ -198,15 +195,14 @@
         data = {}
         data["variety"] = OrderVariety.regular
         data["tradingsymbol"] = self.tradingsymbol
         data["exchange"] = self.exchange
         data["transaction_type"] = self.transaction_type
         data["quantity"] = self.quantity
         data["order_type"] = self.order_type
-        data["order_timestamp"] = self.order_timestamp
         data["disclosed_quantity"] = None
         data["price"] = self.price
         data["trigger_price"] = self.trigger_price
         data["validity"] = self.validity
 
         if self.exchange == ExchangeName.nfo:
             data["product"] = Product.nrml
```

### Comparing `quantplay-1.2.86/quantplay/model/exchange/tick.py` & `quantplay-1.2.9/quantplay/model/exchange/tick.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.86/quantplay/order_execution/execution_algorithm.py` & `quantplay-1.2.9/quantplay/order_execution/execution_algorithm.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.86/quantplay/order_execution/mean_price.py` & `quantplay-1.2.9/quantplay/order_execution/mean_price.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.86/quantplay/reporting/strategy_report.py` & `quantplay-1.2.9/quantplay/reporting/strategy_report.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.86/quantplay/reporting/visuals.py` & `quantplay-1.2.9/quantplay/reporting/visuals.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,11 +32,11 @@
         plt.savefig(file_path)
         plt.show()
 
     @staticmethod
     def display_balance_report(trades, file_prefix):
         file_path = "/tmp/{}balance.png".format(file_prefix)
         trades.loc[:, "balance"] = trades.sort_values(["order_timestamp"]).profit.cumsum()
-        trades.plot(kind="line", x="order_timestamp", y="balance", color="blue")
+        trades.plot(kind="line", x="date", y="balance", color="blue")
         plt.title("Balance Progression")
         plt.savefig(file_path)
         plt.show()
```

### Comparing `quantplay-1.2.86/quantplay/services/market.py` & `quantplay-1.2.9/quantplay/services/market.py`

 * *Files 1% similar despite different names*

```diff
@@ -360,36 +360,33 @@
     def equity_data(self, interval=None, symbols=None):
         df = DataUtils.load_data_using_pandas(
             stocks=symbols, interval=interval, path=self.nse_equity_path
         )
         df.loc[:, "security_type"] = "EQ"
         return df
 
-    def data_by_path(self, interval=None, symbols=None, path=None):
+    def day_by_path(self, interval=None, symbols=None, path=None):
         df = DataUtils.load_data_using_pandas(
             stocks=symbols, interval=interval, path=path
         )
 
         return df
+
     def mcx_data(self, interval=None, symbols=None):
         df = DataUtils.load_data_using_pandas(
             stocks=symbols, interval=interval, path=self.mcx_path
         )
         return df
 
     def data(self, interval=None, symbols_by_security_type=None, **kwargs):
         security_type_data_path = {
             "EQ": self.nse_equity_path,
             "FUT": self.nse_fut_path,
             "OPT": self.nse_opt_path,
         }
-        if "path_suffix" in kwargs:
-            for key in security_type_data_path:
-                security_type_data_path[key] = security_type_data_path[key] + kwargs["path_suffix"]
-
         dfs = []
         for security_type, symbols in symbols_by_security_type.items():
 
             print(
                 f"Loading {security_type} data for {len(set(symbols))} symbols, interval {interval}"
             )
             df = DataUtils.load_data_using_pandas(
```

### Comparing `quantplay-1.2.86/quantplay/strategies/options/intraday/ladder.py` & `quantplay-1.2.9/quantplay/strategies/options/intraday/ladder.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.86/quantplay/strategies/options/intraday/musk.py` & `quantplay-1.2.9/quantplay/strategies/options/intraday/musk.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.86/quantplay/strategy/base.py` & `quantplay-1.2.9/quantplay/strategy/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import re
 import numpy as np
 import uuid
-from quantplay.utils.constant import Constants, OrderType, IntervalAttribute
+from quantplay.utils.constant import Constants, OrderType
 from quantplay.service import market, backtesting
 from quantplay.utils.exchange import Market as MarketConstants
 from quantplay.model.exchange.order import QuantplayExchangeOrder
 from quantplay.exception.exceptions import StrategyInvocationException
 import datetime
 import pandas as pd
-from datetime import timedelta
 
 pd.options.mode.chained_assignment = None  # default='warn'
 
 
 class QuantplayAlgorithm:
     MAX_LEN_FOR_STRATEGY_TAG = 15
 
@@ -119,64 +118,45 @@
         trades["uuid"] = uuids[g.ngroup()]
 
     def filter_uuids_not_matching_count(self, trades):
         """Filters out trades with uuids not matching the self.exact_number_of_order_per_uuid count"""
         self.add_orders_uuid(trades, self.columns_for_uuid)
 
         trades.loc[
-        :, "exact_number_of_orders_per_uuid"
+            :, "exact_number_of_orders_per_uuid"
         ] = self.exact_number_of_orders_per_uuid
 
         return trades[
             trades["uuid"].map(trades["uuid"].value_counts())
             == trades["exact_number_of_orders_per_uuid"]
-            ]
+        ]
 
     def live_orders(self, market_data, tick_time):
         """Returns list of QuantplayExchangeOrder tuples
         which are to be executed immediately.
         """
         try:
             trades = self.get_trades(market_data)
 
             if len(trades) == 0:
-                return {
-                    "entry_orders": trades
-                }
-
-            interval_minutes = int(Constants.interval_attributes[self.interval][IntervalAttribute.seconds] / 60)
+                return trades
 
             trades.loc[:, "tag"] = self.strategy_tag
             trades.loc[:, "strategy_type"] = self.strategy_type
-            trades.loc[:, 'order_timestamp'] = trades.date.apply(lambda x: x + timedelta(minutes=interval_minutes))
-
-            exit_orders = []
-            if "exit_time" in trades.columns:
-                exit_trades = trades[trades.exit_time == tick_time]
-                exit_trades = exit_trades.to_dict("records")
-                exit_orders = QuantplayExchangeOrder.get_exchange_orders(
-                        exit_trades,
-                        order_type=self.order_type,
-                        exchange=self.exchange_to_trade_on,
-                        execution_algo=self.execution_algo,
-                    )
 
-            entry_trades = trades[trades.date == tick_time]
-            entry_trades = entry_trades.to_dict("records")
-            entry_orders = QuantplayExchangeOrder.get_exchange_orders(
-                entry_trades,
+            trades = trades[trades.date == tick_time]
+            trades = trades.to_dict("records")
+            orders = QuantplayExchangeOrder.get_exchange_orders(
+                trades,
                 order_type=self.order_type,
                 exchange=self.exchange_to_trade_on,
                 execution_algo=self.execution_algo,
             )
 
-            return {
-                "entry_orders": entry_orders,
-                "exit_orders": exit_orders
-            }
+            return orders
         except Exception as e:
             raise StrategyInvocationException(
                 f"Failed to invoke strategy {self.strategy_tag}"
             ) from e
 
     def add_derivative_symbols(self, mode='backtest'):
         opt_derivative_symbols, fut_derivative_symbols = set(), set()
@@ -231,14 +211,15 @@
                     symbol + formatted_expiry_date + str(strike) + "PE"
                     for strike in range(lowest_strike, highest_strike, strike_gap)
                 ]
                 opt_derivative_symbols.update(ce_symbols + pe_symbols)
 
             self.stream_symbols_by_security_type["OPT"] = list(opt_derivative_symbols)
 
+
         if hasattr(self, "future_nearest_expiry_offset"):
             self.fut_expiry_data = market.get_nearest_expiry_data(
                 symbols=equity_symbols,
                 days_offset=self.future_nearest_expiry_offset,
                 security_type="FUT",
             )
 
@@ -249,28 +230,29 @@
                 formatted_expiry_date = market.format_expiry_date(
                     expiry_date, security_type="FUT"
                 )
                 fut_derivative_symbols.add(symbol + formatted_expiry_date + "FUT")
 
             self.stream_symbols_by_security_type["FUT"] = list(fut_derivative_symbols)
 
+
     def add_expiry(self, trades, security_type=None):
         if security_type == "OPT":
             return market.add_expiry(
-                trades,
-                security_type=security_type,
-                days_offset=self.option_nearest_expiry_offset,
-            )
+                    trades,
+                    security_type=security_type,
+                    days_offset=self.option_nearest_expiry_offset,
+                )
 
         if security_type == "FUT":
             return market.add_expiry(
-                trades,
-                security_type=security_type,
-                days_offset=self.future_nearest_expiry_offset,
-            )
+                    trades,
+                    security_type=security_type,
+                    days_offset=self.future_nearest_expiry_offset,
+                )
 
     def backtest(self, **kwargs):
         if hasattr(self, "backtest_after_date"):
             kwargs["after"] = self.backtest_after_date
         if hasattr(self, "backtest_before_date"):
             kwargs["before"] = self.backtest_before_date
         market_data = market.data(
@@ -297,21 +279,22 @@
         for security_type in security_types:
             symbols_by_security_type[security_type] = list(
                 trades[trades.security_type == security_type].tradingsymbol.unique()
             )
 
         trades.loc[:, "date_only"] = pd.to_datetime(trades.date.dt.date)
 
-        backtesting.load_data(symbols_by_security_type, self.interval, **kwargs)
+        backtesting.load_data(symbols_by_security_type, self.interval)
         if hasattr(self, "exit_time"):
             trades = backtesting.add_time(
                 trades,
                 column_time_tuple=("exit_time", self.exit_time),
                 holding_days=holding_days,
             )
         backtesting.validate_trades(trades, columns_to_validate=["exit_time"])
 
+
         results, trades_res = backtesting.evaluate_performance(
             trades, self.interval, tag=self.strategy_tag, args=kwargs
         )
 
         return results, trades_res
```

### Comparing `quantplay-1.2.86/quantplay/utils/config_util.py` & `quantplay-1.2.9/quantplay/utils/config_util.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.86/quantplay/utils/constant.py` & `quantplay-1.2.9/quantplay/utils/constant.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,14 @@
 
     five_minute = "5minute"
     day = "day"
     thirty_minute = "30minute"
     three_minute = "3minute"
     minute = "minute"
     fifteen_minute = "15minute"
-    hour = "60minute"
 
     @staticmethod
     def get_interval_seconds(interval: str) -> int:
         if interval == TickInterval.minute:
             return 60
         elif interval == TickInterval.five_minute:
             return 300
@@ -105,34 +104,23 @@
 
 class Constants:
     interval_attributes = {
         TickInterval.minute: {
             IntervalAttribute.seconds: 60,
             IntervalAttribute.mod_value: 1,
         },
-        TickInterval.fifteen_minute: {
-            IntervalAttribute.seconds: 60*15,
-            IntervalAttribute.mod_value: 15,
-        },
-        TickInterval.thirty_minute: {
-            IntervalAttribute.seconds: 60 * 30,
-            IntervalAttribute.mod_value: 30,
-        },
-        TickInterval.hour: {
-            IntervalAttribute.seconds: 60 * 60,
-            IntervalAttribute.mod_value: 60,
-        },
         TickInterval.five_minute: {
             IntervalAttribute.seconds: 300,
             IntervalAttribute.mod_value: 5,
         },
         TickInterval.day: {
             IntervalAttribute.seconds: 375 * 60,
             IntervalAttribute.mod_value: 1,
         },
+        TickInterval.thirty_minute: {IntervalAttribute.seconds: 30 * 60},
         TickInterval.three_minute: {
             IntervalAttribute.seconds: 180,
             IntervalAttribute.mod_value: 3,
         },
     }
 
     security_wise_delivery_position = "security_wise_delivery_position"
@@ -224,15 +212,14 @@
 
     home = expanduser("~")
 
     stock_data_path = "{}/stock_data/".format(home)
     stock_temp_data = "{}/stock_temp_data/".format(home)
 
     logger = LoggerUtils.setup_logger("main_logger", "trading")
-    latency_logger = LoggerUtils.setup_logger('latency', 'latency')
     order_execution_logger = LoggerUtils.setup_logger(
         "order_execution", "order_execution"
     )
     historical_data_logger = LoggerUtils.setup_logger(
         "hist_data_looger", "historical_data"
     )
     tick_logger = LoggerUtils.setup_logger("tick_logger", "tick")
@@ -898,15 +885,15 @@
                         {"Name": "Region", "Value": Constants.region},
                         {
                             "Name": "InstanceType",
                             "Value": Constants.instance_type,
                         },
                     ],
                 }
-                Constants.latency_logger.info("{}".format(json.dumps(data)))
+                Constants.logger.info("{}".format(json.dumps(data)))
             else:
                 Constants.logger.error("No metric found in {}".format(function.__name__))
             return result
 
         return wrapper
 
     return inner_function
```

### Comparing `quantplay-1.2.86/quantplay/utils/data_utils.py` & `quantplay-1.2.9/quantplay/utils/data_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,17 +33,14 @@
         try:
             df = pd.read_csv(path, usecols=columns)
 
             if "after" in kwargs:
                 df = df[df.date >= kwargs["after"]]
             if "before" in kwargs:
                 df = df[df.date <= kwargs["before"]]
-            if "hours" in kwargs:
-                df.loc[:, 'date'] = pd.to_datetime(df.date)
-                df = df[df.date.dt.hour.isin(kwargs["hours"])]
 
             Constants.logger.info("loaded {}".format(path))
             df = df.reset_index(drop=True)
             return df
             # x = pd.read_csv(path)
         except Exception as e:
             Constants.logger.error(
```

### Comparing `quantplay-1.2.86/quantplay/utils/exchange.py` & `quantplay-1.2.9/quantplay/utils/exchange.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.86/quantplay/utils/number_utils.py` & `quantplay-1.2.9/quantplay/utils/number_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.86/quantplay/utils/selenium_utils.py` & `quantplay-1.2.9/quantplay/utils/selenium_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from retrying import retry
 from selenium import webdriver
 
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.common.by import By
 from selenium.common.exceptions import TimeoutException
 from selenium.webdriver.support.ui import WebDriverWait
-from selenium.webdriver.chrome.options import Options
 
 class Selenium():
     def __init__(self):
         self.x = False
 
     @staticmethod
     @retry(wait_exponential_multiplier=1000, wait_exponential_max=10000, stop_max_attempt_number=3)
     def get_browser(headless=True):
-        options = Options()
+        opts = webdriver.ChromeOptions()
+
         if headless == True:
-            options.add_argument("--headless")
+            opts.add_argument('headless')
+
+        opts.add_argument('no-sandbox')
+        browser = webdriver.Chrome(chrome_options=opts)
 
-        return webdriver.Chrome(options=options)
+        return browser
 
     @staticmethod
     def get_element(browser, element_xpath, delay=10):
         if delay == None:
             return browser.find_element("xpath", element_xpath)
         try:
             element = WebDriverWait(browser, delay).until(
```

### Comparing `quantplay-1.2.86/quantplay/utils/transaction_utils.py` & `quantplay-1.2.9/quantplay/utils/transaction_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.86/quantplay.egg-info/PKG-INFO` & `quantplay-1.2.9/quantplay.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantplay
-Version: 1.2.86
+Version: 1.2.9
 Summary: This python package will be stored in AWS CodeArtifact
 Home-page: 
 Author: 
 Author-email: 
 License: MIT
 
 # Quantplay Alpha playground
```

### Comparing `quantplay-1.2.86/quantplay.egg-info/SOURCES.txt` & `quantplay-1.2.9/quantplay.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,60 +1,48 @@
 README.md
 setup.cfg
 setup.py
 quantplay/__init__.py
 quantplay/create_sample_data.py
 quantplay/data_modify_script.py
-quantplay/date_fix.py
 quantplay/service.py
 quantplay/strategy_run.py
 quantplay.egg-info/PKG-INFO
 quantplay.egg-info/SOURCES.txt
 quantplay.egg-info/dependency_links.txt
 quantplay.egg-info/requires.txt
 quantplay.egg-info/top_level.txt
 quantplay/backtest/__init__.py
 quantplay/backtest/backtest_trades.py
 quantplay/broker/__init__.py
 quantplay/broker/angelone.py
 quantplay/broker/broker_client.py
 quantplay/broker/client.py
-quantplay/broker/iifl.py
-quantplay/broker/iifl_xts.py
 quantplay/broker/kite_utils.py
 quantplay/broker/motilal.py
 quantplay/broker/shoonya.py
 quantplay/broker/symphony.py
-quantplay/broker/xts.py
 quantplay/broker/zerodha.py
 quantplay/broker/finvasia_utils/__init__.py
 quantplay/broker/finvasia_utils/shoonya.py
 quantplay/broker/generics/__init__.py
 quantplay/broker/generics/broker.py
-quantplay/broker/xts_utils/Connect.py
-quantplay/broker/xts_utils/Exception.py
-quantplay/broker/xts_utils/InteractiveSocketClient.py
-quantplay/broker/xts_utils/MarketDataSocketClient.py
-quantplay/broker/xts_utils/__init__.py
 quantplay/brokerage/__init__.py
 quantplay/brokerage/angelone/__init__.py
 quantplay/brokerage/angelone/angel_broker.py
 quantplay/brokerage/generics/__init__.py
 quantplay/brokerage/generics/broker.py
 quantplay/brokerage/zerodha/ZBroker.py
 quantplay/brokerage/zerodha/__init__.py
 quantplay/config/__init__.py
 quantplay/config/qplay_config.py
 quantplay/exception/__init__.py
 quantplay/exception/exceptions.py
 quantplay/executor/__init__.py
 quantplay/executor/strategy_executor.py
-quantplay/indicators/Indicator.py
-quantplay/indicators/__init__.py
-quantplay/indicators/atr.py
 quantplay/model/__init__.py
 quantplay/model/exchange/__init__.py
 quantplay/model/exchange/instrument.py
 quantplay/model/exchange/order.py
 quantplay/model/exchange/tick.py
 quantplay/model/strategy/__init__.py
 quantplay/model/strategy/strategy_response.py
```

### Comparing `quantplay-1.2.86/setup.py` & `quantplay-1.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     for line in Path("requirements.txt").read_text().splitlines()
     if is_requirement(line)
 ]
 
 setup(
     name="quantplay",
     long_description=Path("README.md").read_text(),
-    version="1.2.86",
+    version="1.2.9",
     setup_requires=["pytest-runner"],
     install_requires=requirements,
     tests_require=[],
     packages=find_packages(),
     url="",
     license="MIT",
     author="",
```

### Comparing `quantplay-1.2.86/test/strategy/sample_strategy.py` & `quantplay-1.2.9/test/strategy/sample_strategy.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.86/test/test_motilal.py` & `quantplay-1.2.9/test/test_motilal.py`

 * *Files identical despite different names*

