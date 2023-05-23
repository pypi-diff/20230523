# Comparing `tmp/TradeGate-0.3.6.1.tar.gz` & `tmp/TradeGate-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TradeGate-0.3.6.1.tar", last modified: Thu Nov  3 08:32:01 2022, max compression
+gzip compressed data, was "TradeGate-0.3.7.tar", last modified: Tue May 23 11:10:15 2023, max compression
```

## Comparing `TradeGate-0.3.6.1.tar` & `TradeGate-0.3.7.tar`

### file list

```diff
@@ -1,169 +1,169 @@
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2022-11-03 08:32:01.136801 TradeGate-0.3.6.1/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1072 2022-02-23 07:14:51.000000 TradeGate-0.3.6.1/LICENSE
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     2608 2022-11-03 08:32:01.136892 TradeGate-0.3.6.1/PKG-INFO
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     2235 2022-06-20 05:37:13.000000 TradeGate-0.3.6.1/README.md
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2022-11-03 08:32:01.107224 TradeGate-0.3.6.1/TradeGates/
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2022-11-03 08:32:01.109718 TradeGate-0.3.6.1/TradeGates/Exchanges/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     3872 2022-08-25 13:29:43.000000 TradeGate-0.3.6.1/TradeGates/Exchanges/BaseExchange.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    29149 2022-11-03 08:31:41.000000 TradeGate-0.3.6.1/TradeGates/Exchanges/BinanceExchange.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    31008 2022-08-25 13:29:09.000000 TradeGate-0.3.6.1/TradeGates/Exchanges/BybitExchange.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    43853 2022-10-26 18:21:04.000000 TradeGate-0.3.6.1/TradeGates/Exchanges/KuCoinExchange.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)       83 2022-03-23 21:08:19.000000 TradeGate-0.3.6.1/TradeGates/Exchanges/__init__.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2022-11-03 08:32:01.110551 TradeGate-0.3.6.1/TradeGates/TradeGate.egg-info/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     2608 2022-11-03 08:32:01.000000 TradeGate-0.3.6.1/TradeGates/TradeGate.egg-info/PKG-INFO
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     5673 2022-11-03 08:32:01.000000 TradeGate-0.3.6.1/TradeGates/TradeGate.egg-info/SOURCES.txt
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        1 2022-11-03 08:32:01.000000 TradeGate-0.3.6.1/TradeGates/TradeGate.egg-info/dependency_links.txt
--rw-r--r--   0 rustinsoraki   (501) staff       (20)       89 2022-11-03 08:32:01.000000 TradeGate-0.3.6.1/TradeGates/TradeGate.egg-info/requires.txt
--rw-r--r--   0 rustinsoraki   (501) staff       (20)       67 2022-11-03 08:32:01.000000 TradeGate-0.3.6.1/TradeGates/TradeGate.egg-info/top_level.txt
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    58449 2022-09-12 11:40:50.000000 TradeGate-0.3.6.1/TradeGates/TradeGate.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2022-11-03 08:32:01.111517 TradeGate-0.3.6.1/TradeGates/Utils/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     4088 2022-06-27 15:23:02.000000 TradeGate-0.3.6.1/TradeGates/Utils/BinanceHelpers.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    13000 2022-06-27 15:23:02.000000 TradeGate-0.3.6.1/TradeGates/Utils/BybitHelpers.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     7822 2022-06-27 15:23:02.000000 TradeGate-0.3.6.1/TradeGates/Utils/DataHelpers.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    13251 2022-06-19 05:59:28.000000 TradeGate-0.3.6.1/TradeGates/Utils/KuCoinHelpers.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)       80 2022-10-02 08:05:21.000000 TradeGate-0.3.6.1/TradeGates/Utils/__init__.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2022-11-03 08:32:01.111780 TradeGate-0.3.6.1/TradeGates/Watchers/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-03-23 21:08:19.000000 TradeGate-0.3.6.1/TradeGates/Watchers/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     2561 2022-06-16 09:06:16.000000 TradeGate-0.3.6.1/TradeGates/Watchers/futureOrderWatchers.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2022-11-03 08:32:01.112309 TradeGate-0.3.6.1/TradeGates/binance_f/
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      112 2022-02-23 05:49:50.000000 TradeGate-0.3.6.1/TradeGates/binance_f/__init__.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2022-11-03 08:32:01.112948 TradeGate-0.3.6.1/TradeGates/binance_f/base/
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/base/__init__.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     5597 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/base/printobject.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      597 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/base/printtime.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2022-11-03 08:32:01.113364 TradeGate-0.3.6.1/TradeGates/binance_f/constant/
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/constant/__init__.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      399 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/constant/system.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      250 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/constant/test.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2022-11-03 08:32:01.113624 TradeGate-0.3.6.1/TradeGates/binance_f/exception/
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/exception/__init__.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      422 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/exception/binanceapiexception.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2022-11-03 08:32:01.114995 TradeGate-0.3.6.1/TradeGates/binance_f/impl/
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)       58 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/impl/__init__.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2680 2022-02-26 09:29:35.000000 TradeGate-0.3.6.1/TradeGates/binance_f/impl/restapiinvoker.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      310 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/impl/restapirequest.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)    36651 2022-06-16 09:06:16.000000 TradeGate-0.3.6.1/TradeGates/binance_f/impl/restapirequestimpl.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2022-11-03 08:32:01.116419 TradeGate-0.3.6.1/TradeGates/binance_f/impl/utils/
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      240 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/impl/utils/__init__.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1146 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/impl/utils/apisignature.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      156 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/impl/utils/channelparser.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     5407 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/impl/utils/channels.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     3139 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/impl/utils/inputchecker.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     3400 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/impl/utils/jsonwrapper.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      434 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/impl/utils/timeservice.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1030 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/impl/utils/urlparamsbuilder.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     7819 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/impl/websocketconnection.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      360 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/impl/websocketrequest.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)    15345 2022-03-03 18:09:37.000000 TradeGate-0.3.6.1/TradeGates/binance_f/impl/websocketrequestimpl.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2243 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/impl/websocketwatchdog.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2022-11-03 08:32:01.127079 TradeGate-0.3.6.1/TradeGates/binance_f/model/
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2976 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/__init__.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     4355 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/accountinformation.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     5309 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/accountinformationv2.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2355 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/accountupdate.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      343 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/adlquantile.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      690 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/aggregatetrade.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      971 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/aggregatetradeevent.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1102 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/apitradingstatus.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      999 2022-03-02 11:34:30.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/balance.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      854 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/balancev2.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      908 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/blvtinfoevent.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      706 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/blvtnavcandlestick.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1789 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/blvtnavcandlestickevent.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1607 2022-02-24 11:54:59.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/candlestick.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2230 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/candlestickevent.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      438 2022-03-04 10:50:30.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/codeandmsg.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1304 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/compositeindexevent.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2103 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/constant.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     2389 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/continuouscandelstickevent.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      352 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/countdowncancelall.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1634 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/diffdepthevent.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     3756 2022-06-16 09:06:16.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/exchangeinformation.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      433 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/fundingrate.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      791 2022-06-16 09:06:16.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/income.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1102 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/indexInfo.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      568 2022-03-23 21:08:19.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/leverage.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1271 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/leveragebracket.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      937 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/liquidationorder.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1410 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/liquidationorderevent.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      337 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/listenkeyexpired.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      775 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/longshortratio.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      620 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/markprice.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      661 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/markpriceevent.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      393 2022-03-23 21:08:19.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/message.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2369 2022-03-04 07:28:24.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/mytrade.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      349 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/openinterest.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      635 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/openintereststats.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     3160 2022-03-04 10:20:23.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/order.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1309 2022-06-17 14:41:44.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/orderbook.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1584 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/orderbookevent.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     3015 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/orderupdate.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1978 2022-03-23 21:08:19.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/position.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      461 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/positionmargin.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      558 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/positionmarginhistory.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      274 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/positionmode.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      765 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/symbolbooktickerevent.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      970 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/symbolminitickerevent.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      583 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/symbolorderbook.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      386 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/symbolprice.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1862 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/symboltickerevent.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      531 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/takerbuysellratio.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1691 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/tickerpricechangestatistics.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      896 2022-03-23 21:08:19.000000 TradeGate-0.3.6.1/TradeGates/binance_f/model/trade.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)    23283 2022-03-23 21:08:19.000000 TradeGate-0.3.6.1/TradeGates/binance_f/requestclient.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)    12780 2021-08-19 21:43:22.000000 TradeGate-0.3.6.1/TradeGates/binance_f/subscriptionclient.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2022-11-03 08:32:01.127676 TradeGate-0.3.6.1/TradeGates/kucoin/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.6.1/TradeGates/kucoin/__init__.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2022-11-03 08:32:01.128114 TradeGate-0.3.6.1/TradeGates/kucoin/base_request/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.6.1/TradeGates/kucoin/base_request/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     4269 2022-06-16 09:06:16.000000 TradeGate-0.3.6.1/TradeGates/kucoin/base_request/base_request.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      390 2022-06-16 09:06:16.000000 TradeGate-0.3.6.1/TradeGates/kucoin/client.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2022-11-03 08:32:01.128472 TradeGate-0.3.6.1/TradeGates/kucoin/margin/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.6.1/TradeGates/kucoin/margin/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    14243 2022-06-16 09:06:16.000000 TradeGate-0.3.6.1/TradeGates/kucoin/margin/margin.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2022-11-03 08:32:01.128873 TradeGate-0.3.6.1/TradeGates/kucoin/market/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.6.1/TradeGates/kucoin/market/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    16795 2022-06-16 09:06:16.000000 TradeGate-0.3.6.1/TradeGates/kucoin/market/market.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2022-11-03 08:32:01.129324 TradeGate-0.3.6.1/TradeGates/kucoin/trade/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.6.1/TradeGates/kucoin/trade/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    24825 2022-06-16 09:06:16.000000 TradeGate-0.3.6.1/TradeGates/kucoin/trade/trade.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2022-11-03 08:32:01.129926 TradeGate-0.3.6.1/TradeGates/kucoin/user/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.6.1/TradeGates/kucoin/user/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    23869 2022-06-27 12:34:05.000000 TradeGate-0.3.6.1/TradeGates/kucoin/user/user.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2022-11-03 08:32:01.130517 TradeGate-0.3.6.1/TradeGates/kucoin/websocket/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.6.1/TradeGates/kucoin/websocket/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     5633 2022-06-16 09:06:16.000000 TradeGate-0.3.6.1/TradeGates/kucoin/websocket/websocket.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1594 2022-06-16 09:06:16.000000 TradeGate-0.3.6.1/TradeGates/kucoin/ws_client.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2022-11-03 08:32:01.131143 TradeGate-0.3.6.1/TradeGates/kucoin/ws_token/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.6.1/TradeGates/kucoin/ws_token/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      451 2022-06-16 09:06:16.000000 TradeGate-0.3.6.1/TradeGates/kucoin/ws_token/token.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2022-11-03 08:32:01.132172 TradeGate-0.3.6.1/TradeGates/kucoin_futures/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.6.1/TradeGates/kucoin_futures/__init__.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2022-11-03 08:32:01.132835 TradeGate-0.3.6.1/TradeGates/kucoin_futures/base_request/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.6.1/TradeGates/kucoin_futures/base_request/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     4299 2022-06-16 09:06:16.000000 TradeGate-0.3.6.1/TradeGates/kucoin_futures/base_request/base_request.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      376 2022-06-16 09:06:16.000000 TradeGate-0.3.6.1/TradeGates/kucoin_futures/client.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2022-11-03 08:32:01.133444 TradeGate-0.3.6.1/TradeGates/kucoin_futures/marke_data/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.6.1/TradeGates/kucoin_futures/marke_data/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    22513 2022-06-16 09:06:16.000000 TradeGate-0.3.6.1/TradeGates/kucoin_futures/marke_data/market_data.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2022-11-03 08:32:01.134014 TradeGate-0.3.6.1/TradeGates/kucoin_futures/trade/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.6.1/TradeGates/kucoin_futures/trade/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    31092 2022-06-16 09:06:16.000000 TradeGate-0.3.6.1/TradeGates/kucoin_futures/trade/trade.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2022-11-03 08:32:01.134719 TradeGate-0.3.6.1/TradeGates/kucoin_futures/user/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.6.1/TradeGates/kucoin_futures/user/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     9818 2022-06-16 09:06:16.000000 TradeGate-0.3.6.1/TradeGates/kucoin_futures/user/user.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2022-11-03 08:32:01.135079 TradeGate-0.3.6.1/TradeGates/kucoin_futures/websocket/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.6.1/TradeGates/kucoin_futures/websocket/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     5633 2022-06-16 09:06:16.000000 TradeGate-0.3.6.1/TradeGates/kucoin_futures/websocket/websocket.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1620 2022-06-16 09:06:16.000000 TradeGate-0.3.6.1/TradeGates/kucoin_futures/ws_client.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2022-11-03 08:32:01.135371 TradeGate-0.3.6.1/TradeGates/kucoin_futures/ws_token/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.6.1/TradeGates/kucoin_futures/ws_token/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      480 2022-06-16 09:06:16.000000 TradeGate-0.3.6.1/TradeGates/kucoin_futures/ws_token/token.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      267 2022-06-17 08:03:32.000000 TradeGate-0.3.6.1/pyproject.toml
--rw-r--r--   0 rustinsoraki   (501) staff       (20)       79 2022-11-03 08:32:01.137172 TradeGate-0.3.6.1/setup.cfg
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1453 2022-11-03 08:31:51.000000 TradeGate-0.3.6.1/setup.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2022-11-03 08:32:01.136478 TradeGate-0.3.6.1/test/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     3400 2022-06-17 13:30:13.000000 TradeGate-0.3.6.1/test/testAccountInfo.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    16024 2022-06-27 15:23:02.000000 TradeGate-0.3.6.1/test/testFutures.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     5351 2022-06-16 09:06:16.000000 TradeGate-0.3.6.1/test/testMarketInfo.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     7291 2022-06-27 13:57:30.000000 TradeGate-0.3.6.1/test/testOrdering.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-23 11:10:15.614378 TradeGate-0.3.7/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1072 2022-02-23 07:14:51.000000 TradeGate-0.3.7/LICENSE
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     2606 2023-05-23 11:10:15.614500 TradeGate-0.3.7/PKG-INFO
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     2235 2022-06-20 05:37:13.000000 TradeGate-0.3.7/README.md
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-23 11:10:15.582758 TradeGate-0.3.7/TradeGates/
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-23 11:10:15.585041 TradeGate-0.3.7/TradeGates/Exchanges/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     4225 2023-05-23 06:35:44.000000 TradeGate-0.3.7/TradeGates/Exchanges/BaseExchange.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    29271 2023-05-23 06:39:51.000000 TradeGate-0.3.7/TradeGates/Exchanges/BinanceExchange.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    33903 2023-05-22 21:47:52.000000 TradeGate-0.3.7/TradeGates/Exchanges/BybitExchange.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    43853 2022-10-26 18:21:04.000000 TradeGate-0.3.7/TradeGates/Exchanges/KuCoinExchange.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)       83 2022-03-23 21:08:19.000000 TradeGate-0.3.7/TradeGates/Exchanges/__init__.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-23 11:10:15.585776 TradeGate-0.3.7/TradeGates/TradeGate.egg-info/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     2606 2023-05-23 11:10:15.000000 TradeGate-0.3.7/TradeGates/TradeGate.egg-info/PKG-INFO
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     5673 2023-05-23 11:10:15.000000 TradeGate-0.3.7/TradeGates/TradeGate.egg-info/SOURCES.txt
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        1 2023-05-23 11:10:15.000000 TradeGate-0.3.7/TradeGates/TradeGate.egg-info/dependency_links.txt
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)       89 2023-05-23 11:10:15.000000 TradeGate-0.3.7/TradeGates/TradeGate.egg-info/requires.txt
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)       67 2023-05-23 11:10:15.000000 TradeGate-0.3.7/TradeGates/TradeGate.egg-info/top_level.txt
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    58565 2023-05-23 11:03:39.000000 TradeGate-0.3.7/TradeGates/TradeGate.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-23 11:10:15.587204 TradeGate-0.3.7/TradeGates/Utils/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     4088 2022-06-27 15:23:02.000000 TradeGate-0.3.7/TradeGates/Utils/BinanceHelpers.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    13000 2022-06-27 15:23:02.000000 TradeGate-0.3.7/TradeGates/Utils/BybitHelpers.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     7822 2022-06-27 15:23:02.000000 TradeGate-0.3.7/TradeGates/Utils/DataHelpers.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    13251 2022-06-19 05:59:28.000000 TradeGate-0.3.7/TradeGates/Utils/KuCoinHelpers.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)       80 2022-10-02 08:05:21.000000 TradeGate-0.3.7/TradeGates/Utils/__init__.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-23 11:10:15.587648 TradeGate-0.3.7/TradeGates/Watchers/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-03-23 21:08:19.000000 TradeGate-0.3.7/TradeGates/Watchers/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     2561 2022-06-16 09:06:16.000000 TradeGate-0.3.7/TradeGates/Watchers/futureOrderWatchers.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-23 11:10:15.588608 TradeGate-0.3.7/TradeGates/binance_f/
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      112 2022-02-23 05:49:50.000000 TradeGate-0.3.7/TradeGates/binance_f/__init__.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-23 11:10:15.589258 TradeGate-0.3.7/TradeGates/binance_f/base/
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/base/__init__.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     5597 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/base/printobject.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      597 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/base/printtime.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-23 11:10:15.589646 TradeGate-0.3.7/TradeGates/binance_f/constant/
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/constant/__init__.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      399 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/constant/system.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      250 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/constant/test.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-23 11:10:15.589888 TradeGate-0.3.7/TradeGates/binance_f/exception/
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/exception/__init__.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      422 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/exception/binanceapiexception.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-23 11:10:15.591790 TradeGate-0.3.7/TradeGates/binance_f/impl/
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)       58 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/impl/__init__.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2680 2022-02-26 09:29:35.000000 TradeGate-0.3.7/TradeGates/binance_f/impl/restapiinvoker.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      310 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/impl/restapirequest.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)    36651 2022-06-16 09:06:16.000000 TradeGate-0.3.7/TradeGates/binance_f/impl/restapirequestimpl.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-23 11:10:15.593280 TradeGate-0.3.7/TradeGates/binance_f/impl/utils/
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      240 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/impl/utils/__init__.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1146 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/impl/utils/apisignature.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      156 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/impl/utils/channelparser.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     5407 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/impl/utils/channels.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     3139 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/impl/utils/inputchecker.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     3400 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/impl/utils/jsonwrapper.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      434 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/impl/utils/timeservice.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1030 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/impl/utils/urlparamsbuilder.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     7819 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/impl/websocketconnection.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      360 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/impl/websocketrequest.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)    15345 2022-03-03 18:09:37.000000 TradeGate-0.3.7/TradeGates/binance_f/impl/websocketrequestimpl.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2243 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/impl/websocketwatchdog.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-23 11:10:15.607000 TradeGate-0.3.7/TradeGates/binance_f/model/
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2976 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/__init__.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     4355 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/accountinformation.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     5309 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/accountinformationv2.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2355 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/accountupdate.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      343 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/adlquantile.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      690 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/aggregatetrade.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      971 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/aggregatetradeevent.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1102 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/apitradingstatus.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      999 2022-03-02 11:34:30.000000 TradeGate-0.3.7/TradeGates/binance_f/model/balance.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      854 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/balancev2.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      908 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/blvtinfoevent.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      706 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/blvtnavcandlestick.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1789 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/blvtnavcandlestickevent.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1607 2022-02-24 11:54:59.000000 TradeGate-0.3.7/TradeGates/binance_f/model/candlestick.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2230 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/candlestickevent.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      438 2022-03-04 10:50:30.000000 TradeGate-0.3.7/TradeGates/binance_f/model/codeandmsg.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1304 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/compositeindexevent.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2103 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/constant.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     2389 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/continuouscandelstickevent.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      352 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/countdowncancelall.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1634 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/diffdepthevent.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     3756 2022-06-16 09:06:16.000000 TradeGate-0.3.7/TradeGates/binance_f/model/exchangeinformation.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      433 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/fundingrate.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      791 2022-06-16 09:06:16.000000 TradeGate-0.3.7/TradeGates/binance_f/model/income.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1102 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/indexInfo.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      568 2022-03-23 21:08:19.000000 TradeGate-0.3.7/TradeGates/binance_f/model/leverage.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1271 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/leveragebracket.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      937 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/liquidationorder.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1410 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/liquidationorderevent.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      337 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/listenkeyexpired.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      775 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/longshortratio.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      620 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/markprice.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      661 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/markpriceevent.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      393 2022-03-23 21:08:19.000000 TradeGate-0.3.7/TradeGates/binance_f/model/message.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2369 2022-03-04 07:28:24.000000 TradeGate-0.3.7/TradeGates/binance_f/model/mytrade.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      349 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/openinterest.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      635 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/openintereststats.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     3160 2022-03-04 10:20:23.000000 TradeGate-0.3.7/TradeGates/binance_f/model/order.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1309 2022-06-17 14:41:44.000000 TradeGate-0.3.7/TradeGates/binance_f/model/orderbook.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1584 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/orderbookevent.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     3015 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/orderupdate.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1978 2022-03-23 21:08:19.000000 TradeGate-0.3.7/TradeGates/binance_f/model/position.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      461 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/positionmargin.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      558 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/positionmarginhistory.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      274 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/positionmode.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      765 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/symbolbooktickerevent.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      970 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/symbolminitickerevent.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      583 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/symbolorderbook.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      386 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/symbolprice.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1862 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/symboltickerevent.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      531 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/takerbuysellratio.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1691 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/model/tickerpricechangestatistics.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      896 2022-03-23 21:08:19.000000 TradeGate-0.3.7/TradeGates/binance_f/model/trade.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)    23283 2022-03-23 21:08:19.000000 TradeGate-0.3.7/TradeGates/binance_f/requestclient.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)    12780 2021-08-19 21:43:22.000000 TradeGate-0.3.7/TradeGates/binance_f/subscriptionclient.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-23 11:10:15.607573 TradeGate-0.3.7/TradeGates/kucoin/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.7/TradeGates/kucoin/__init__.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-23 11:10:15.607965 TradeGate-0.3.7/TradeGates/kucoin/base_request/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.7/TradeGates/kucoin/base_request/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     4269 2022-06-16 09:06:16.000000 TradeGate-0.3.7/TradeGates/kucoin/base_request/base_request.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      390 2022-06-16 09:06:16.000000 TradeGate-0.3.7/TradeGates/kucoin/client.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-23 11:10:15.608283 TradeGate-0.3.7/TradeGates/kucoin/margin/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.7/TradeGates/kucoin/margin/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    14243 2022-06-16 09:06:16.000000 TradeGate-0.3.7/TradeGates/kucoin/margin/margin.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-23 11:10:15.608670 TradeGate-0.3.7/TradeGates/kucoin/market/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.7/TradeGates/kucoin/market/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    16795 2022-06-16 09:06:16.000000 TradeGate-0.3.7/TradeGates/kucoin/market/market.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-23 11:10:15.609081 TradeGate-0.3.7/TradeGates/kucoin/trade/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.7/TradeGates/kucoin/trade/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    24825 2022-06-16 09:06:16.000000 TradeGate-0.3.7/TradeGates/kucoin/trade/trade.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-23 11:10:15.609585 TradeGate-0.3.7/TradeGates/kucoin/user/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.7/TradeGates/kucoin/user/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    23869 2022-06-27 12:34:05.000000 TradeGate-0.3.7/TradeGates/kucoin/user/user.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-23 11:10:15.610210 TradeGate-0.3.7/TradeGates/kucoin/websocket/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.7/TradeGates/kucoin/websocket/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     5633 2022-06-16 09:06:16.000000 TradeGate-0.3.7/TradeGates/kucoin/websocket/websocket.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1594 2022-06-16 09:06:16.000000 TradeGate-0.3.7/TradeGates/kucoin/ws_client.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-23 11:10:15.610544 TradeGate-0.3.7/TradeGates/kucoin/ws_token/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.7/TradeGates/kucoin/ws_token/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      451 2022-06-16 09:06:16.000000 TradeGate-0.3.7/TradeGates/kucoin/ws_token/token.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-23 11:10:15.611057 TradeGate-0.3.7/TradeGates/kucoin_futures/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.7/TradeGates/kucoin_futures/__init__.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-23 11:10:15.611343 TradeGate-0.3.7/TradeGates/kucoin_futures/base_request/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.7/TradeGates/kucoin_futures/base_request/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     4299 2022-06-16 09:06:16.000000 TradeGate-0.3.7/TradeGates/kucoin_futures/base_request/base_request.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      376 2022-06-16 09:06:16.000000 TradeGate-0.3.7/TradeGates/kucoin_futures/client.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-23 11:10:15.611631 TradeGate-0.3.7/TradeGates/kucoin_futures/marke_data/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.7/TradeGates/kucoin_futures/marke_data/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    22513 2022-06-16 09:06:16.000000 TradeGate-0.3.7/TradeGates/kucoin_futures/marke_data/market_data.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-23 11:10:15.611988 TradeGate-0.3.7/TradeGates/kucoin_futures/trade/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.7/TradeGates/kucoin_futures/trade/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    31092 2022-06-16 09:06:16.000000 TradeGate-0.3.7/TradeGates/kucoin_futures/trade/trade.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-23 11:10:15.612342 TradeGate-0.3.7/TradeGates/kucoin_futures/user/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.7/TradeGates/kucoin_futures/user/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     9818 2022-06-16 09:06:16.000000 TradeGate-0.3.7/TradeGates/kucoin_futures/user/user.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-23 11:10:15.612638 TradeGate-0.3.7/TradeGates/kucoin_futures/websocket/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.7/TradeGates/kucoin_futures/websocket/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     5633 2022-06-16 09:06:16.000000 TradeGate-0.3.7/TradeGates/kucoin_futures/websocket/websocket.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1620 2022-06-16 09:06:16.000000 TradeGate-0.3.7/TradeGates/kucoin_futures/ws_client.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-23 11:10:15.612904 TradeGate-0.3.7/TradeGates/kucoin_futures/ws_token/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.7/TradeGates/kucoin_futures/ws_token/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      480 2022-06-16 09:06:16.000000 TradeGate-0.3.7/TradeGates/kucoin_futures/ws_token/token.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      267 2022-06-17 08:03:32.000000 TradeGate-0.3.7/pyproject.toml
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)       79 2023-05-23 11:10:15.614871 TradeGate-0.3.7/setup.cfg
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1451 2023-05-23 11:10:10.000000 TradeGate-0.3.7/setup.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-23 11:10:15.614081 TradeGate-0.3.7/test/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     3400 2022-06-17 13:30:13.000000 TradeGate-0.3.7/test/testAccountInfo.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    16024 2022-06-27 15:23:02.000000 TradeGate-0.3.7/test/testFutures.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     5351 2022-06-16 09:06:16.000000 TradeGate-0.3.7/test/testMarketInfo.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     7291 2022-06-27 13:57:30.000000 TradeGate-0.3.7/test/testOrdering.py
```

### Comparing `TradeGate-0.3.6.1/LICENSE` & `TradeGate-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/PKG-INFO` & `TradeGate-0.3.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TradeGate
-Version: 0.3.6.1
+Version: 0.3.7
 Summary: A Trading Gateway
 Author: Rustin Soraki
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `TradeGate-0.3.6.1/README.md` & `TradeGate-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/Exchanges/BaseExchange.py` & `TradeGate-0.3.7/TradeGates/Exchanges/BaseExchange.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 class BaseExchange(ABC):
     @abstractmethod
     def __init__(self, credentials, sandbox=False, unifiedInOuts=True):
         pass
 
     @abstractmethod
-    def getBalance(self, asset='', futures=False):
+    def getBalance(self, asset="", futures=False):
         pass
 
     @abstractmethod
     def symbolAccountTradeHistory(self, symbol, futures=False, fromId=None, limit=None):
         pass
 
     @abstractmethod
@@ -19,21 +19,40 @@
         pass
 
     @abstractmethod
     def makeSpotOrder(self, orderData):
         pass
 
     @abstractmethod
-    def createAndTestSpotOrder(self, symbol, side, orderType, quantity=None, price=None, timeInForce=None,
-                               stopPrice=None, icebergQty=None, newOrderRespType=None,
-                               newClientOrderId=None, extraParams=None):
+    def createAndTestSpotOrder(
+        self,
+        symbol,
+        side,
+        orderType,
+        quantity=None,
+        price=None,
+        timeInForce=None,
+        stopPrice=None,
+        icebergQty=None,
+        newOrderRespType=None,
+        newClientOrderId=None,
+        extraParams=None,
+    ):
         pass
 
     @abstractmethod
-    def getSymbolOrders(self, symbol, futures=False, orderId=None, startTime=None, endTime=None, limit=None):
+    def getSymbolOrders(
+        self,
+        symbol,
+        futures=False,
+        orderId=None,
+        startTime=None,
+        endTime=None,
+        limit=None,
+    ):
         pass
 
     @abstractmethod
     def getOpenOrders(self, symbol, futures=False):
         pass
 
     @abstractmethod
@@ -53,16 +72,27 @@
         pass
 
     @abstractmethod
     def getSymbolTickerPrice(self, symbol, futures=False):
         pass
 
     @abstractmethod
-    def getSymbolKlines(self, symbol, interval, startTime=None, endTime=None, limit=None, futures=False, blvtnav=False,
-                        convertDateTime=False, doClean=False, toCleanDataframe=False):
+    def getSymbolKlines(
+        self,
+        symbol,
+        interval,
+        startTime=None,
+        endTime=None,
+        limit=None,
+        futures=False,
+        blvtnav=False,
+        convertDateTime=False,
+        doClean=False,
+        toCleanDataframe=False,
+    ):
         pass
 
     @abstractmethod
     def getExchangeTime(self, futures=False):
         pass
 
     @abstractmethod
@@ -74,19 +104,35 @@
         pass
 
     @abstractmethod
     def makeFuturesOrder(self, futuresOrderData):
         pass
 
     @abstractmethod
-    def createAndTestFuturesOrder(self, symbol, side, orderType, positionSide=None, timeInForce=None, quantity=None,
-                                  reduceOnly=None, price=None, newClientOrderId=None,
-                                  stopPrice=None, closePosition=None, activationPrice=None, callbackRate=None,
-                                  workingType=None, priceProtect=None, newOrderRespType=None,
-                                  recvWindow=None, extraParams=None):
+    def createAndTestFuturesOrder(
+        self,
+        symbol,
+        side,
+        orderType,
+        positionSide=None,
+        timeInForce=None,
+        quantity=None,
+        reduceOnly=None,
+        price=None,
+        newClientOrderId=None,
+        stopPrice=None,
+        closePosition=None,
+        activationPrice=None,
+        callbackRate=None,
+        workingType=None,
+        priceProtect=None,
+        newOrderRespType=None,
+        recvWindow=None,
+        extraParams=None,
+    ):
         pass
 
     @abstractmethod
     def makeBatchFuturesOrder(self, futuresOrderDatas):
         pass
 
     @abstractmethod
@@ -122,14 +168,30 @@
         pass
 
     @abstractmethod
     def getSymbolMinTrade(self, symbol, futures=False):
         pass
 
     @abstractmethod
-    def makeSlTpLimitFuturesOrder(self, symbol, orderSide, quantity=None, quoteQuantity=None, enterPrice=None,
-                                  takeProfit=None, stopLoss=None, leverage=None, marginType=None):
+    def makeSlTpLimitFuturesOrder(
+        self,
+        symbol,
+        orderSide,
+        quantity=None,
+        quoteQuantity=None,
+        enterPrice=None,
+        takeProfit=None,
+        stopLoss=None,
+        leverage=None,
+        marginType=None,
+    ):
         pass
 
     @abstractmethod
-    def getLongShortRatios(self, symbol, period, limit=None, startTime=None, endTime=None):
-        pass
+    def getLongShortRatios(
+        self, symbol, period, limit=None, startTime=None, endTime=None
+    ):
+        pass
+
+    @abstractmethod
+    def getDepositAddress(self, coin, network=None):
+        pass
```

### Comparing `TradeGate-0.3.6.1/TradeGates/Exchanges/BinanceExchange.py` & `TradeGate-0.3.7/TradeGates/Exchanges/BinanceExchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,15 +274,14 @@
         timeInForce=None,
         stopPrice=None,
         icebergQty=None,
         newOrderRespType=None,
         newClientOrderId=None,
         extraParams=None,
     ):
-
         currOrder = DataHelpers.setSpotOrderData(
             icebergQty,
             newClientOrderId,
             newOrderRespType,
             orderType,
             price,
             quantity,
@@ -702,15 +701,14 @@
         quoteQuantity=None,
         enterPrice=None,
         takeProfit=None,
         stopLoss=None,
         leverage=None,
         marginType=None,
     ):
-
         symbolInfo = self.getSymbolMinTrade(symbol=symbol, futures=True)
 
         quantity = DataHelpers.getQuantity(
             enterPrice, quantity, quoteQuantity, symbolInfo["precisionStep"]
         )
         self._setLeverage(leverage, symbol)
         self.changeMarginType(symbol, marginType)
@@ -762,15 +760,14 @@
         quantity=None,
         quoteQuantity=None,
         takeProfit=None,
         stopLoss=None,
         leverage=None,
         marginType=None,
     ):
-
         symbolInfo = self.getSymbolMinTrade(symbol=symbol, futures=True)
         marketPrice = self.getSymbolTickerPrice(symbol=symbol, futures=True)
 
         quantity = DataHelpers.getQuantity(
             marketPrice, quantity, quoteQuantity, symbolInfo["precisionStep"]
         )
         self._setLeverage(leverage, symbol)
@@ -908,7 +905,10 @@
         )
 
         return {
             "topLongShortAccounts": topLongShortAccounts,
             "topLongShortPositions": topLongShortPositions,
             "longShortRatio": longShortRatio,
         }
+
+    def getDepositAddress(self, coin, network=None):
+        return self.client.deposit_address(coin=coin, network=network)
```

### Comparing `TradeGate-0.3.6.1/TradeGates/Exchanges/KuCoinExchange.py` & `TradeGate-0.3.7/TradeGates/Exchanges/KuCoinExchange.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/TradeGate.egg-info/PKG-INFO` & `TradeGate-0.3.7/TradeGates/TradeGate.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TradeGate
-Version: 0.3.6.1
+Version: 0.3.7
 Summary: A Trading Gateway
 Author: Rustin Soraki
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `TradeGate-0.3.6.1/TradeGates/TradeGate.egg-info/SOURCES.txt` & `TradeGate-0.3.7/TradeGates/TradeGate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/TradeGate.py` & `TradeGate-0.3.7/TradeGates/TradeGate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1519,7 +1519,10 @@
     def getLongShortRatios(
         self, symbol, period, limit=None, startTime=None, endTime=None
     ):
         print(self.exchange)
         return self.exchange.getLongShortRatios(
             symbol, period, limit, startTime, endTime
         )
+
+    def getDepositAddress(self, coin, network=None):
+        return self.exchange.getDepositAddress(coin, network)
```

### Comparing `TradeGate-0.3.6.1/TradeGates/Utils/BinanceHelpers.py` & `TradeGate-0.3.7/TradeGates/Utils/BinanceHelpers.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/Utils/BybitHelpers.py` & `TradeGate-0.3.7/TradeGates/Utils/BybitHelpers.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/Utils/DataHelpers.py` & `TradeGate-0.3.7/TradeGates/Utils/DataHelpers.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/Utils/KuCoinHelpers.py` & `TradeGate-0.3.7/TradeGates/Utils/KuCoinHelpers.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/Watchers/futureOrderWatchers.py` & `TradeGate-0.3.7/TradeGates/Watchers/futureOrderWatchers.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/base/printobject.py` & `TradeGate-0.3.7/TradeGates/binance_f/base/printobject.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/base/printtime.py` & `TradeGate-0.3.7/TradeGates/binance_f/base/printtime.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/impl/restapiinvoker.py` & `TradeGate-0.3.7/TradeGates/binance_f/impl/restapiinvoker.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/impl/restapirequestimpl.py` & `TradeGate-0.3.7/TradeGates/binance_f/impl/restapirequestimpl.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/impl/utils/apisignature.py` & `TradeGate-0.3.7/TradeGates/binance_f/impl/utils/apisignature.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/impl/utils/channels.py` & `TradeGate-0.3.7/TradeGates/binance_f/impl/utils/channels.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/impl/utils/inputchecker.py` & `TradeGate-0.3.7/TradeGates/binance_f/impl/utils/inputchecker.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/impl/utils/jsonwrapper.py` & `TradeGate-0.3.7/TradeGates/binance_f/impl/utils/jsonwrapper.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/impl/utils/urlparamsbuilder.py` & `TradeGate-0.3.7/TradeGates/binance_f/impl/utils/urlparamsbuilder.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/impl/websocketconnection.py` & `TradeGate-0.3.7/TradeGates/binance_f/impl/websocketconnection.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/impl/websocketrequestimpl.py` & `TradeGate-0.3.7/TradeGates/binance_f/impl/websocketrequestimpl.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/impl/websocketwatchdog.py` & `TradeGate-0.3.7/TradeGates/binance_f/impl/websocketwatchdog.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/__init__.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/__init__.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/accountinformation.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/accountinformation.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/accountinformationv2.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/accountinformationv2.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/accountupdate.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/accountupdate.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/aggregatetrade.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/aggregatetrade.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/aggregatetradeevent.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/aggregatetradeevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/apitradingstatus.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/apitradingstatus.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/balance.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/balance.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/balancev2.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/balancev2.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/blvtinfoevent.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/blvtinfoevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/blvtnavcandlestick.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/blvtnavcandlestick.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/blvtnavcandlestickevent.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/blvtnavcandlestickevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/candlestick.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/candlestick.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/candlestickevent.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/candlestickevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/compositeindexevent.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/compositeindexevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/constant.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/constant.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/continuouscandelstickevent.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/continuouscandelstickevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/diffdepthevent.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/diffdepthevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/exchangeinformation.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/exchangeinformation.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/income.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/income.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/indexInfo.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/indexInfo.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/leverage.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/leverage.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/leveragebracket.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/leveragebracket.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/liquidationorder.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/liquidationorder.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/liquidationorderevent.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/liquidationorderevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/longshortratio.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/longshortratio.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/markprice.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/markprice.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/markpriceevent.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/markpriceevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/mytrade.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/mytrade.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/openintereststats.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/openintereststats.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/order.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/order.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/orderbook.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/orderbook.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/orderbookevent.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/orderbookevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/orderupdate.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/orderupdate.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/position.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/position.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/positionmarginhistory.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/positionmarginhistory.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/symbolbooktickerevent.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/symbolbooktickerevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/symbolminitickerevent.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/symbolminitickerevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/symbolorderbook.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/symbolorderbook.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/symboltickerevent.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/symboltickerevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/takerbuysellratio.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/takerbuysellratio.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/tickerpricechangestatistics.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/tickerpricechangestatistics.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/model/trade.py` & `TradeGate-0.3.7/TradeGates/binance_f/model/trade.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/requestclient.py` & `TradeGate-0.3.7/TradeGates/binance_f/requestclient.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/binance_f/subscriptionclient.py` & `TradeGate-0.3.7/TradeGates/binance_f/subscriptionclient.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/kucoin/base_request/base_request.py` & `TradeGate-0.3.7/TradeGates/kucoin/base_request/base_request.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/kucoin/margin/margin.py` & `TradeGate-0.3.7/TradeGates/kucoin/margin/margin.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/kucoin/market/market.py` & `TradeGate-0.3.7/TradeGates/kucoin/market/market.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/kucoin/trade/trade.py` & `TradeGate-0.3.7/TradeGates/kucoin/trade/trade.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/kucoin/user/user.py` & `TradeGate-0.3.7/TradeGates/kucoin/user/user.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/kucoin/websocket/websocket.py` & `TradeGate-0.3.7/TradeGates/kucoin/websocket/websocket.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/kucoin/ws_client.py` & `TradeGate-0.3.7/TradeGates/kucoin/ws_client.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/kucoin_futures/base_request/base_request.py` & `TradeGate-0.3.7/TradeGates/kucoin_futures/base_request/base_request.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/kucoin_futures/marke_data/market_data.py` & `TradeGate-0.3.7/TradeGates/kucoin_futures/marke_data/market_data.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/kucoin_futures/trade/trade.py` & `TradeGate-0.3.7/TradeGates/kucoin_futures/trade/trade.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/kucoin_futures/user/user.py` & `TradeGate-0.3.7/TradeGates/kucoin_futures/user/user.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/kucoin_futures/websocket/websocket.py` & `TradeGate-0.3.7/TradeGates/kucoin_futures/websocket/websocket.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/TradeGates/kucoin_futures/ws_client.py` & `TradeGate-0.3.7/TradeGates/kucoin_futures/ws_client.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/setup.py` & `TradeGate-0.3.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     shutil.rmtree("./build")
     shutil.rmtree("./dist")
 except OSError as e:
     print("Error: %s - %s." % (e.filename, e.strerror))
 
 setuptools.setup(
     name="TradeGate",  # This is the name of the package
-    version="0.3.6.1",
+    version="0.3.7",
     author="Rustin Soraki",  # Full name of the author
     description="A Trading Gateway",
     long_description=long_description,  # Long description read from the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(
         where="TradeGates"
     ),  # List of all python modules to be installed
```

### Comparing `TradeGate-0.3.6.1/test/testAccountInfo.py` & `TradeGate-0.3.7/test/testAccountInfo.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/test/testFutures.py` & `TradeGate-0.3.7/test/testFutures.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/test/testMarketInfo.py` & `TradeGate-0.3.7/test/testMarketInfo.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.6.1/test/testOrdering.py` & `TradeGate-0.3.7/test/testOrdering.py`

 * *Files identical despite different names*

