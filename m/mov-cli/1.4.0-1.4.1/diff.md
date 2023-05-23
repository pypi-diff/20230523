# Comparing `tmp/mov_cli-1.4.0.tar.gz` & `tmp/mov_cli-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov_cli-1.4.0.tar", max compression
+gzip compressed data, was "mov_cli-1.4.1.tar", max compression
```

## Comparing `mov_cli-1.4.0.tar` & `mov_cli-1.4.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0    35149 2023-05-19 23:35:55.147552 mov_cli-1.4.0/LICENSE
--rw-r--r--   0        0        0     7098 2023-05-19 23:35:55.147552 mov_cli-1.4.0/README.md
--rw-r--r--   0        0        0        0 2023-05-19 23:35:55.147552 mov_cli-1.4.0/mov_cli/__init__.py
--rw-r--r--   0        0        0     2701 2023-05-19 23:35:55.147552 mov_cli-1.4.0/mov_cli/__main__.py
--rw-r--r--   0        0        0        1 2023-05-19 23:35:55.147552 mov_cli-1.4.0/mov_cli/extractors/__init__.py
--rw-r--r--   0        0        0      823 2023-05-19 23:35:55.147552 mov_cli-1.4.0/mov_cli/extractors/doodstream.py
--rw-r--r--   0        0        0       71 2023-05-19 23:35:55.147552 mov_cli-1.4.0/mov_cli/extractors/scdn/NOTICE
--rw-r--r--   0        0        0        1 2023-05-19 23:35:55.147552 mov_cli-1.4.0/mov_cli/extractors/scdn/__init__.py
--rw-r--r--   0        0        0      169 2023-05-19 23:35:55.147552 mov_cli-1.4.0/mov_cli/extractors/scdn/allsportsdaily.py
--rw-r--r--   0        0        0      958 2023-05-19 23:35:55.147552 mov_cli-1.4.0/mov_cli/extractors/scdn/cr7sports.py
--rw-r--r--   0        0        0      256 2023-05-19 23:35:55.147552 mov_cli-1.4.0/mov_cli/extractors/scdn/enjoy4hd.py
--rw-r--r--   0        0        0      141 2023-05-19 23:35:55.147552 mov_cli-1.4.0/mov_cli/extractors/scdn/fabtech.py
--rw-r--r--   0        0        0      218 2023-05-19 23:35:55.147552 mov_cli-1.4.0/mov_cli/extractors/scdn/gameshdlive.py
--rw-r--r--   0        0        0      457 2023-05-19 23:35:55.147552 mov_cli-1.4.0/mov_cli/extractors/scdn/livestreames.py
--rw-r--r--   0        0        0      318 2023-05-19 23:35:55.147552 mov_cli-1.4.0/mov_cli/extractors/scdn/methstreams.py
--rw-r--r--   0        0        0      156 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/extractors/scdn/motornews.py
--rw-r--r--   0        0        0      873 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/extractors/scdn/onestream.py
--rw-r--r--   0        0        0      891 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/extractors/scdn/onionlive.py
--rw-r--r--   0        0        0      615 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/extractors/scdn/onionstream.py
--rw-r--r--   0        0        0      457 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/extractors/scdn/poscitech.py
--rw-r--r--   0        0        0      638 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/extractors/scdn/rainostreams.py
--rw-r--r--   0        0        0      358 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/extractors/scdn/ripple.py
--rw-r--r--   0        0        0      406 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/extractors/scdn/techclips.py
--rw-r--r--   0        0        0      417 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/extractors/scdn/techstips.py
--rw-r--r--   0        0        0     1333 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/extractors/scdn/weakstream.py
--rw-r--r--   0        0        0        0 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/players/__init__.py
--rw-r--r--   0        0        0     2238 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/players/player.py
--rw-r--r--   0        0        0        0 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/utils/__init__.py
--rw-r--r--   0        0        0     1483 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/utils/dbs.py
--rw-r--r--   0        0        0     2731 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/utils/httpclient.py
--rw-r--r--   0        0        0     6133 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/utils/jsunpack.py
--rw-r--r--   0        0        0     2269 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/utils/lang.py
--rw-r--r--   0        0        0     1592 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/utils/player.py
--rw-r--r--   0        0        0      941 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/utils/provider.py
--rw-r--r--   0        0        0     8714 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/utils/scraper.py
--rw-r--r--   0        0        0        0 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/__init__.py
--rw-r--r--   0        0        0    11020 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/actvid.py
--rw-r--r--   0        0        0     4177 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/animefox.py
--rw-r--r--   0        0        0     4112 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/dopebox.py
--rw-r--r--   0        0        0     1943 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/einthusan.py
--rw-r--r--   0        0        0     1724 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/eja.py
--rw-r--r--   0        0        0     3016 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/gogoanime.py
--rw-r--r--   0        0        0     7122 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/kinox.py
--rw-r--r--   0        0        0     3736 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/kisscartoon.py
--rw-r--r--   0        0        0     2509 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/openloadmov.py
--rw-r--r--   0        0        0     2563 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/redundant_kimcartoon.py
--rw-r--r--   0        0        0     4662 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/remotestream.py
--rw-r--r--   0        0        0     4422 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/scdn.py
--rw-r--r--   0        0        0     4121 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/sflix.py
--rw-r--r--   0        0        0     1622 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/solar.py
--rw-r--r--   0        0        0     2132 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/streamblasters.py
--rw-r--r--   0        0        0     1358 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/tamilyogi.py
--rw-r--r--   0        0        0     2895 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/turkish123.py
--rw-r--r--   0        0        0     4516 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/viewasian.py
--rw-r--r--   0        0        0     3395 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/watchasian.py
--rw-r--r--   0        0        0     3983 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/wlext.py
--rw-r--r--   0        0        0     3503 2023-05-19 23:35:55.155552 mov_cli-1.4.0/mov_cli/websites/yoturkish.py
--rw-r--r--   0        0        0      743 2023-05-19 23:35:55.155552 mov_cli-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     8093 1970-01-01 00:00:00.000000 mov_cli-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-23 10:46:55.139511 mov_cli-1.4.1/LICENSE
+-rw-r--r--   0        0        0     7098 2023-05-23 10:46:55.139511 mov_cli-1.4.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/__init__.py
+-rw-r--r--   0        0        0     2701 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/__main__.py
+-rw-r--r--   0        0        0        1 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/__init__.py
+-rw-r--r--   0        0        0      823 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/doodstream.py
+-rw-r--r--   0        0        0       71 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/NOTICE
+-rw-r--r--   0        0        0        1 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/__init__.py
+-rw-r--r--   0        0        0      169 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/allsportsdaily.py
+-rw-r--r--   0        0        0      958 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/cr7sports.py
+-rw-r--r--   0        0        0      256 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/enjoy4hd.py
+-rw-r--r--   0        0        0      141 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/fabtech.py
+-rw-r--r--   0        0        0      218 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/gameshdlive.py
+-rw-r--r--   0        0        0      457 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/livestreames.py
+-rw-r--r--   0        0        0      318 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/methstreams.py
+-rw-r--r--   0        0        0      156 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/motornews.py
+-rw-r--r--   0        0        0      873 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/onestream.py
+-rw-r--r--   0        0        0      891 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/onionlive.py
+-rw-r--r--   0        0        0      615 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/onionstream.py
+-rw-r--r--   0        0        0      457 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/poscitech.py
+-rw-r--r--   0        0        0      638 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/rainostreams.py
+-rw-r--r--   0        0        0      358 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/ripple.py
+-rw-r--r--   0        0        0      406 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/techclips.py
+-rw-r--r--   0        0        0      417 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/techstips.py
+-rw-r--r--   0        0        0     1333 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/weakstream.py
+-rw-r--r--   0        0        0        0 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/players/__init__.py
+-rw-r--r--   0        0        0     2238 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/players/player.py
+-rw-r--r--   0        0        0        0 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/utils/__init__.py
+-rw-r--r--   0        0        0     1483 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/utils/dbs.py
+-rw-r--r--   0        0        0     2731 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/utils/httpclient.py
+-rw-r--r--   0        0        0     6133 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/utils/jsunpack.py
+-rw-r--r--   0        0        0     2269 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/utils/lang.py
+-rw-r--r--   0        0        0     1592 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/utils/player.py
+-rw-r--r--   0        0        0      941 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/utils/provider.py
+-rw-r--r--   0        0        0     8714 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/utils/scraper.py
+-rw-r--r--   0        0        0        0 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/websites/__init__.py
+-rw-r--r--   0        0        0    11020 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/websites/actvid.py
+-rw-r--r--   0        0        0     4177 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/websites/animefox.py
+-rw-r--r--   0        0        0     4112 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/websites/dopebox.py
+-rw-r--r--   0        0        0     1943 2023-05-23 10:46:55.147511 mov_cli-1.4.1/mov_cli/websites/einthusan.py
+-rw-r--r--   0        0        0     1724 2023-05-23 10:46:55.147511 mov_cli-1.4.1/mov_cli/websites/eja.py
+-rw-r--r--   0        0        0     3210 2023-05-23 10:46:55.147511 mov_cli-1.4.1/mov_cli/websites/gogoanime.py
+-rw-r--r--   0        0        0     7122 2023-05-23 10:46:55.147511 mov_cli-1.4.1/mov_cli/websites/kinox.py
+-rw-r--r--   0        0        0     3736 2023-05-23 10:46:55.147511 mov_cli-1.4.1/mov_cli/websites/kisscartoon.py
+-rw-r--r--   0        0        0     2509 2023-05-23 10:46:55.147511 mov_cli-1.4.1/mov_cli/websites/openloadmov.py
+-rw-r--r--   0        0        0     2563 2023-05-23 10:46:55.147511 mov_cli-1.4.1/mov_cli/websites/redundant_kimcartoon.py
+-rw-r--r--   0        0        0     4662 2023-05-23 10:46:55.147511 mov_cli-1.4.1/mov_cli/websites/remotestream.py
+-rw-r--r--   0        0        0     4422 2023-05-23 10:46:55.147511 mov_cli-1.4.1/mov_cli/websites/scdn.py
+-rw-r--r--   0        0        0     4121 2023-05-23 10:46:55.147511 mov_cli-1.4.1/mov_cli/websites/sflix.py
+-rw-r--r--   0        0        0     1622 2023-05-23 10:46:55.147511 mov_cli-1.4.1/mov_cli/websites/solar.py
+-rw-r--r--   0        0        0     2132 2023-05-23 10:46:55.147511 mov_cli-1.4.1/mov_cli/websites/streamblasters.py
+-rw-r--r--   0        0        0     1358 2023-05-23 10:46:55.147511 mov_cli-1.4.1/mov_cli/websites/tamilyogi.py
+-rw-r--r--   0        0        0     2895 2023-05-23 10:46:55.147511 mov_cli-1.4.1/mov_cli/websites/turkish123.py
+-rw-r--r--   0        0        0     4516 2023-05-23 10:46:55.147511 mov_cli-1.4.1/mov_cli/websites/viewasian.py
+-rw-r--r--   0        0        0     3395 2023-05-23 10:46:55.147511 mov_cli-1.4.1/mov_cli/websites/watchasian.py
+-rw-r--r--   0        0        0     3983 2023-05-23 10:46:55.147511 mov_cli-1.4.1/mov_cli/websites/wlext.py
+-rw-r--r--   0        0        0     3503 2023-05-23 10:46:55.147511 mov_cli-1.4.1/mov_cli/websites/yoturkish.py
+-rw-r--r--   0        0        0      743 2023-05-23 10:46:55.147511 mov_cli-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     8093 1970-01-01 00:00:00.000000 mov_cli-1.4.1/PKG-INFO
```

### Comparing `mov_cli-1.4.0/LICENSE` & `mov_cli-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/README.md` & `mov_cli-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/mov_cli/__main__.py` & `mov_cli-1.4.1/mov_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/mov_cli/extractors/doodstream.py` & `mov_cli-1.4.1/mov_cli/extractors/doodstream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/mov_cli/extractors/scdn/cr7sports.py` & `mov_cli-1.4.1/mov_cli/extractors/scdn/cr7sports.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/mov_cli/extractors/scdn/onestream.py` & `mov_cli-1.4.1/mov_cli/extractors/scdn/onestream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/mov_cli/extractors/scdn/onionlive.py` & `mov_cli-1.4.1/mov_cli/extractors/scdn/onionlive.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/mov_cli/extractors/scdn/onionstream.py` & `mov_cli-1.4.1/mov_cli/extractors/scdn/onionstream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/mov_cli/extractors/scdn/rainostreams.py` & `mov_cli-1.4.1/mov_cli/extractors/scdn/rainostreams.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/mov_cli/extractors/scdn/weakstream.py` & `mov_cli-1.4.1/mov_cli/extractors/scdn/weakstream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/mov_cli/players/player.py` & `mov_cli-1.4.1/mov_cli/players/player.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/mov_cli/utils/dbs.py` & `mov_cli-1.4.1/mov_cli/utils/dbs.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/mov_cli/utils/httpclient.py` & `mov_cli-1.4.1/mov_cli/utils/httpclient.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/mov_cli/utils/jsunpack.py` & `mov_cli-1.4.1/mov_cli/utils/jsunpack.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/mov_cli/utils/lang.py` & `mov_cli-1.4.1/mov_cli/utils/lang.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/mov_cli/utils/player.py` & `mov_cli-1.4.1/mov_cli/utils/player.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/mov_cli/utils/provider.py` & `mov_cli-1.4.1/mov_cli/utils/provider.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/mov_cli/utils/scraper.py` & `mov_cli-1.4.1/mov_cli/utils/scraper.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/mov_cli/websites/actvid.py` & `mov_cli-1.4.1/mov_cli/websites/actvid.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/mov_cli/websites/animefox.py` & `mov_cli-1.4.1/mov_cli/websites/animefox.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/mov_cli/websites/dopebox.py` & `mov_cli-1.4.1/mov_cli/websites/dopebox.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/mov_cli/websites/einthusan.py` & `mov_cli-1.4.1/mov_cli/websites/einthusan.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/mov_cli/websites/eja.py` & `mov_cli-1.4.1/mov_cli/websites/eja.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/mov_cli/websites/gogoanime.py` & `mov_cli-1.4.1/mov_cli/websites/gogoanime.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,22 +9,28 @@
         self.base_url = base_url
 
     def search(self, q: str):
         q = input(f"[!] {self.translated[self.task]}") if q is None else q
         return q.replace(" ", "-")
 
     def results(self, data: str) -> list:
-        req = self.client.get(f"{self.base_url}/search.html?keyword={data}")
-        soup = BS(req, self.scraper)
-        items = soup.find("ul", {"class": "items"}).findAll("li")
-        urls = [items[i].find("a")["href"] for i in range(len(items))]
-        title = [items[i].find("a")["title"] for i in range(len(items))]
-        ids = [items[i].find("a")["title"] for i in range(len(items))]
-        mov_or_tv = ["TV" for i in range(len(items))]
-        return [list(sublist) for sublist in zip(title, urls, ids, mov_or_tv)]
+        results = []
+        page = 1
+        while True:
+            req = self.client.get(f"{self.base_url}/search.html?keyword={data}&page={page}")
+            soup = BS(req, self.scraper)
+            items = soup.find("ul", {"class": "items"}).findAll("li")
+            if len(items) == 0: break
+            urls = [items[i].find("a")["href"] for i in range(len(items))]
+            title = [items[i].find("a")["title"] for i in range(len(items))]
+            ids = [items[i].find("a")["title"] for i in range(len(items))]
+            mov_or_tv = ["TV" for i in range(len(items))]
+            results.extend([list(sublist) for sublist in zip(title, urls, ids, mov_or_tv)])
+            page += 1
+        return results
 
     def ask(self, url):
         req = self.client.get(f"{self.base_url}{url}")
         soup = BS(req, self.scraper)
         episodes = soup.find("ul", {"id": "episode_page"}).find_all("a")[-1]["ep_end"]
         episode = self.askepisode(int(episodes))
         url = url.split("/")[-1]
```

### Comparing `mov_cli-1.4.0/mov_cli/websites/kinox.py` & `mov_cli-1.4.1/mov_cli/websites/kinox.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/mov_cli/websites/kisscartoon.py` & `mov_cli-1.4.1/mov_cli/websites/kisscartoon.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/mov_cli/websites/openloadmov.py` & `mov_cli-1.4.1/mov_cli/websites/openloadmov.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/mov_cli/websites/redundant_kimcartoon.py` & `mov_cli-1.4.1/mov_cli/websites/redundant_kimcartoon.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/mov_cli/websites/remotestream.py` & `mov_cli-1.4.1/mov_cli/websites/remotestream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/mov_cli/websites/scdn.py` & `mov_cli-1.4.1/mov_cli/websites/scdn.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/mov_cli/websites/sflix.py` & `mov_cli-1.4.1/mov_cli/websites/sflix.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/mov_cli/websites/solar.py` & `mov_cli-1.4.1/mov_cli/websites/solar.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/mov_cli/websites/streamblasters.py` & `mov_cli-1.4.1/mov_cli/websites/streamblasters.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/mov_cli/websites/tamilyogi.py` & `mov_cli-1.4.1/mov_cli/websites/tamilyogi.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/mov_cli/websites/turkish123.py` & `mov_cli-1.4.1/mov_cli/websites/turkish123.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/mov_cli/websites/viewasian.py` & `mov_cli-1.4.1/mov_cli/websites/viewasian.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/mov_cli/websites/watchasian.py` & `mov_cli-1.4.1/mov_cli/websites/watchasian.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/mov_cli/websites/wlext.py` & `mov_cli-1.4.1/mov_cli/websites/wlext.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/mov_cli/websites/yoturkish.py` & `mov_cli-1.4.1/mov_cli/websites/yoturkish.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.0/pyproject.toml` & `mov_cli-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mov-cli"
-version = "1.4.0"
+version = "1.4.1"
 description = "A cli tool to browse and watch Movies/Shows/TV/Sports."
 authors = ["Pain <painedposeidon444@gmail.com>"]
 maintainers = ["Ananas <ananas@historylifeonline.xyz>"]
 license = "GPLv3"
 readme = "README.md"
 packages = [{include = "mov_cli"}]
 repository = "https://github.com/mov-cli/mov-cli"
```

### Comparing `mov_cli-1.4.0/PKG-INFO` & `mov_cli-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli
-Version: 1.4.0
+Version: 1.4.1
 Summary: A cli tool to browse and watch Movies/Shows/TV/Sports.
 Home-page: https://github.com/mov-cli/mov-cli
 License: GPLv3
 Author: Pain
 Author-email: painedposeidon444@gmail.com
 Maintainer: Ananas
 Maintainer-email: ananas@historylifeonline.xyz
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mov-cli Version: 1.4.0 Summary: A cli tool to
+Metadata-Version: 2.1 Name: mov-cli Version: 1.4.1 Summary: A cli tool to
 browse and watch Movies/Shows/TV/Sports. Home-page: https://github.com/mov-cli/
 mov-cli License: GPLv3 Author: Pain Author-email: painedposeidon444@gmail.com
 Maintainer: Ananas Maintainer-email: ananas@historylifeonline.xyz Requires-
 Python: >=3.9,<4.0 Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: beautifulsoup4
```

