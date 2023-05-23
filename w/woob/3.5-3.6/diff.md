# Comparing `tmp/woob-3.5.tar.gz` & `tmp/woob-3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "woob-3.5.tar", last modified: Sat Apr  8 10:13:26 2023, max compression
+gzip compressed data, was "woob-3.6.tar", last modified: Tue May 23 13:50:43 2023, max compression
```

## Comparing `woob-3.5.tar` & `woob-3.6.tar`

### file list

```diff
@@ -1,299 +1,301 @@
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.326515 woob-3.5/
--rw-r--r--   0 rom1      (1000) rom1      (1000)    12426 2023-04-08 10:13:23.000000 woob-3.5/AUTHORS
--rw-r--r--   0 rom1      (1000) rom1      (1000)    35149 2023-04-08 10:13:23.000000 woob-3.5/COPYING
--rw-r--r--   0 rom1      (1000) rom1      (1000)     7652 2023-04-08 10:13:23.000000 woob-3.5/COPYING.LESSER
--rw-r--r--   0 rom1      (1000) rom1      (1000)     4526 2023-04-08 10:13:26.326515 woob-3.5/PKG-INFO
--rw-r--r--   0 rom1      (1000) rom1      (1000)     3164 2023-04-08 10:13:23.000000 woob-3.5/README.rst
--rw-r--r--   0 rom1      (1000) rom1      (1000)     2970 2023-04-08 10:13:23.000000 woob-3.5/pyproject.toml
--rw-r--r--   0 rom1      (1000) rom1      (1000)       38 2023-04-08 10:13:26.326515 woob-3.5/setup.cfg
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.302515 woob-3.5/weboob/
--rw-r--r--   0 rom1      (1000) rom1      (1000)     1898 2023-04-08 10:13:23.000000 woob-3.5/weboob/__init__.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.302515 woob-3.5/woob/
--rw-r--r--   0 rom1      (1000) rom1      (1000)      176 2023-04-08 10:13:23.000000 woob-3.5/woob/__init__.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.302515 woob-3.5/woob/applications/
--rw-r--r--   0 rom1      (1000) rom1      (1000)       66 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/__init__.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.302515 woob-3.5/woob/applications/bands/
--rw-r--r--   0 rom1      (1000) rom1      (1000)      757 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/bands/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     6527 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/bands/bands.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.302515 woob-3.5/woob/applications/bank/
--rw-r--r--   0 rom1      (1000) rom1      (1000)      754 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/bank/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    37071 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/bank/bank.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.302515 woob-3.5/woob/applications/bill/
--rw-r--r--   0 rom1      (1000) rom1      (1000)      753 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/bill/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    11124 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/bill/bill.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.302515 woob-3.5/woob/applications/books/
--rw-r--r--   0 rom1      (1000) rom1      (1000)      757 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/books/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     2777 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/books/books.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.302515 woob-3.5/woob/applications/bugtracker/
--rw-r--r--   0 rom1      (1000) rom1      (1000)      765 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/bugtracker/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    17645 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/bugtracker/bugtracker.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.302515 woob-3.5/woob/applications/calendar/
--rw-r--r--   0 rom1      (1000) rom1      (1000)      754 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/calendar/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    16284 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/calendar/calendar.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.302515 woob-3.5/woob/applications/cinema/
--rw-r--r--   0 rom1      (1000) rom1      (1000)      755 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/cinema/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    26526 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/cinema/cinema.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.302515 woob-3.5/woob/applications/cli/
--rw-r--r--   0 rom1      (1000) rom1      (1000)      749 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/cli/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     1699 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/cli/cli.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.302515 woob-3.5/woob/applications/config/
--rw-r--r--   0 rom1      (1000) rom1      (1000)      758 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/config/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    11169 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/config/config.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.302515 woob-3.5/woob/applications/contentedit/
--rw-r--r--   0 rom1      (1000) rom1      (1000)      773 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/contentedit/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     7670 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/contentedit/contentedit.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.302515 woob-3.5/woob/applications/dating/
--rw-r--r--   0 rom1      (1000) rom1      (1000)      758 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/dating/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    10199 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/dating/dating.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.306515 woob-3.5/woob/applications/debug/
--rw-r--r--   0 rom1      (1000) rom1      (1000)      756 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/debug/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     3429 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/debug/debug.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.306515 woob-3.5/woob/applications/gallery/
--rw-r--r--   0 rom1      (1000) rom1      (1000)      763 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/gallery/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     4703 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/gallery/gallery.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.306515 woob-3.5/woob/applications/gauge/
--rw-r--r--   0 rom1      (1000) rom1      (1000)      753 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/gauge/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     6967 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/gauge/gauge.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.306515 woob-3.5/woob/applications/geolocip/
--rw-r--r--   0 rom1      (1000) rom1      (1000)      764 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/geolocip/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     1556 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/geolocip/geolocip.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.306515 woob-3.5/woob/applications/housing/
--rw-r--r--   0 rom1      (1000) rom1      (1000)       58 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/housing/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    10239 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/housing/housing.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.306515 woob-3.5/woob/applications/job/
--rw-r--r--   0 rom1      (1000) rom1      (1000)      739 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/job/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     4875 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/job/job.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.306515 woob-3.5/woob/applications/lyrics/
--rw-r--r--   0 rom1      (1000) rom1      (1000)      755 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/lyrics/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     3526 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/lyrics/lyrics.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.306515 woob-3.5/woob/applications/main/
--rw-r--r--   0 rom1      (1000) rom1      (1000)      754 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/main/__init__.py
--rwxr-xr-x   0 rom1      (1000) rom1      (1000)     3136 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/main/main.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.306515 woob-3.5/woob/applications/money/
--rw-r--r--   0 rom1      (1000) rom1      (1000)      744 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/money/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    34529 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/money/money.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.306515 woob-3.5/woob/applications/msg/
--rw-r--r--   0 rom1      (1000) rom1      (1000)      751 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/msg/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    19113 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/msg/msg.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.306515 woob-3.5/woob/applications/parcel/
--rw-r--r--   0 rom1      (1000) rom1      (1000)      753 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/parcel/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     7265 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/parcel/parcel.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.306515 woob-3.5/woob/applications/paste/
--rw-r--r--   0 rom1      (1000) rom1      (1000)      755 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/paste/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     7499 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/paste/paste.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.306515 woob-3.5/woob/applications/pricecompare/
--rw-r--r--   0 rom1      (1000) rom1      (1000)       73 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/pricecompare/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     6102 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/pricecompare/pricecompare.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.306515 woob-3.5/woob/applications/radio/
--rw-r--r--   0 rom1      (1000) rom1      (1000)      755 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/radio/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    16009 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/radio/radio.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.306515 woob-3.5/woob/applications/recipes/
--rw-r--r--   0 rom1      (1000) rom1      (1000)      757 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/recipes/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     5429 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/recipes/recipes.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.306515 woob-3.5/woob/applications/repos/
--rw-r--r--   0 rom1      (1000) rom1      (1000)      763 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/repos/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     8762 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/repos/repos.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.306515 woob-3.5/woob/applications/rpg/
--rw-r--r--   0 rom1      (1000) rom1      (1000)      751 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/rpg/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     3921 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/rpg/rpg.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.306515 woob-3.5/woob/applications/shop/
--rw-r--r--   0 rom1      (1000) rom1      (1000)      753 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/shop/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     6585 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/shop/shop.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.306515 woob-3.5/woob/applications/smtp/
--rw-r--r--   0 rom1      (1000) rom1      (1000)      752 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/smtp/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    13512 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/smtp/smtp.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.310515 woob-3.5/woob/applications/subtitles/
--rw-r--r--   0 rom1      (1000) rom1      (1000)      763 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/subtitles/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     7660 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/subtitles/subtitles.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.310515 woob-3.5/woob/applications/torrent/
--rw-r--r--   0 rom1      (1000) rom1      (1000)      761 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/torrent/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     6572 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/torrent/torrent.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.310515 woob-3.5/woob/applications/translate/
--rw-r--r--   0 rom1      (1000) rom1      (1000)      763 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/translate/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     5117 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/translate/translate.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.310515 woob-3.5/woob/applications/travel/
--rw-r--r--   0 rom1      (1000) rom1      (1000)      758 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/travel/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     6717 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/travel/travel.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.310515 woob-3.5/woob/applications/video/
--rw-r--r--   0 rom1      (1000) rom1      (1000)      757 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/video/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     4890 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/video/image2xterm.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    12099 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/video/video.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.310515 woob-3.5/woob/applications/weather/
--rw-r--r--   0 rom1      (1000) rom1      (1000)      761 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/weather/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     5004 2023-04-08 10:13:23.000000 woob-3.5/woob/applications/weather/weather.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.310515 woob-3.5/woob/browser/
--rw-r--r--   0 rom1      (1000) rom1      (1000)     1120 2023-04-08 10:13:23.000000 woob-3.5/woob/browser/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     2369 2023-04-08 10:13:23.000000 woob-3.5/woob/browser/adapters.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    56044 2023-04-08 10:13:23.000000 woob-3.5/woob/browser/browsers.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     3397 2023-04-08 10:13:23.000000 woob-3.5/woob/browser/cache.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     1819 2023-04-08 10:13:23.000000 woob-3.5/woob/browser/cloudscraper.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     1873 2023-04-08 10:13:23.000000 woob-3.5/woob/browser/cookies.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    19314 2023-04-08 10:13:23.000000 woob-3.5/woob/browser/elements.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     2063 2023-04-08 10:13:23.000000 woob-3.5/woob/browser/exceptions.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.314515 woob-3.5/woob/browser/filters/
--rw-r--r--   0 rom1      (1000) rom1      (1000)      696 2023-04-08 10:13:23.000000 woob-3.5/woob/browser/filters/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     6156 2023-04-08 10:13:23.000000 woob-3.5/woob/browser/filters/base.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    10153 2023-04-08 10:13:23.000000 woob-3.5/woob/browser/filters/html.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     5984 2023-04-08 10:13:23.000000 woob-3.5/woob/browser/filters/javascript.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     2908 2023-04-08 10:13:23.000000 woob-3.5/woob/browser/filters/json.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    34453 2023-04-08 10:13:23.000000 woob-3.5/woob/browser/filters/standard.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     8589 2023-04-08 10:13:23.000000 woob-3.5/woob/browser/har.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     6751 2023-04-08 10:13:23.000000 woob-3.5/woob/browser/mfa.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    18247 2023-04-08 10:13:23.000000 woob-3.5/woob/browser/nss.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    32387 2023-04-08 10:13:23.000000 woob-3.5/woob/browser/pages.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     6009 2023-04-08 10:13:23.000000 woob-3.5/woob/browser/profiles.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     6661 2023-04-08 10:13:23.000000 woob-3.5/woob/browser/retry.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    28149 2023-04-08 10:13:23.000000 woob-3.5/woob/browser/selenium.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     5905 2023-04-08 10:13:23.000000 woob-3.5/woob/browser/sessions.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     4157 2023-04-08 10:13:23.000000 woob-3.5/woob/browser/switch.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    13824 2023-04-08 10:13:23.000000 woob-3.5/woob/browser/url.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.318515 woob-3.5/woob/capabilities/
--rw-r--r--   0 rom1      (1000) rom1      (1000)      159 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     4101 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/account.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     2122 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/address.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     4650 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/audio.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     1858 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/audiostream.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     4651 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/bands.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.318515 woob-3.5/woob/capabilities/bank/
--rw-r--r--   0 rom1      (1000) rom1      (1000)     3351 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/bank/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    22435 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/bank/base.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     3673 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/bank/pfm.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     2248 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/bank/rate.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    22863 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/bank/transfer.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     9467 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/bank/wealth.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    24507 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/base.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    14873 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/bill.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     9405 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/bugtracker.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     6468 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/calendar.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    10911 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/captcha.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     2306 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/chat.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     6302 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/cinema.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     5144 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/collection.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    10673 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/contact.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     2678 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/content.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     2204 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/date.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     3972 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/dating.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     3179 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/file.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     4252 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/gallery.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     3614 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/gauge.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     1883 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/geolocip.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     5341 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/housing.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     2962 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/image.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     3420 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/job.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     2178 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/library.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     1648 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/lyrics.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     6244 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/messages.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     2123 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/parcel.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     3648 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/paste.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     6402 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/picross.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     2620 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/pricecomparison.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     4189 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/profile.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     1690 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/radio.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     2724 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/recipe.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     8392 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/rpg.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     3898 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/shop.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     2277 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/subtitle.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     2453 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/torrent.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     2011 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/translate.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     4301 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/travel.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     1846 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/video.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     5403 2023-04-08 10:13:23.000000 woob-3.5/woob/capabilities/weather.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.318515 woob-3.5/woob/core/
--rw-r--r--   0 rom1      (1000) rom1      (1000)     1798 2023-04-08 10:13:23.000000 woob-3.5/woob/core/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     7196 2023-04-08 10:13:23.000000 woob-3.5/woob/core/backendscfg.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     6082 2023-04-08 10:13:23.000000 woob-3.5/woob/core/bcall.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    10821 2023-04-08 10:13:23.000000 woob-3.5/woob/core/modules.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     1068 2023-04-08 10:13:23.000000 woob-3.5/woob/core/ouiboube.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    35876 2023-04-08 10:13:23.000000 woob-3.5/woob/core/repositories.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     1371 2023-04-08 10:13:23.000000 woob-3.5/woob/core/requests.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     5105 2023-04-08 10:13:23.000000 woob-3.5/woob/core/scheduler.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    21819 2023-04-08 10:13:23.000000 woob-3.5/woob/core/woob.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    18192 2023-04-08 10:13:23.000000 woob-3.5/woob/exceptions.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.322515 woob-3.5/woob/tools/
--rw-r--r--   0 rom1      (1000) rom1      (1000)       66 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/__init__.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.322515 woob-3.5/woob/tools/application/
--rw-r--r--   0 rom1      (1000) rom1      (1000)       66 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/application/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    20142 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/application/base.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     1364 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/application/captcha.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    27072 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/application/console.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.322515 woob-3.5/woob/tools/application/formatters/
--rw-r--r--   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/application/formatters/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     1622 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/application/formatters/csv.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     9340 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/application/formatters/iformatter.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     1540 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/application/formatters/json.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     2572 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/application/formatters/load.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     1451 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/application/formatters/multiline.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     1240 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/application/formatters/simple.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     3437 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/application/formatters/table.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     1795 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/application/javascript.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     6678 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/application/media_player.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    53512 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/application/repl.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     5935 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/application/results.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    20076 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/backend.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.322515 woob-3.5/woob/tools/capabilities/
--rw-r--r--   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/capabilities/__init__.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.322515 woob-3.5/woob/tools/capabilities/audio/
--rw-r--r--   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/capabilities/audio/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     1323 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/capabilities/audio/audio.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.322515 woob-3.5/woob/tools/capabilities/bank/
--rw-r--r--   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/capabilities/bank/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)      938 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/capabilities/bank/bank_transfer.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     3770 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/capabilities/bank/data_matching.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     2939 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/capabilities/bank/iban.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     4378 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/capabilities/bank/investments.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     2485 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/capabilities/bank/sortcode.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     9839 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/capabilities/bank/test.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    12623 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/capabilities/bank/transactions.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.322515 woob-3.5/woob/tools/capabilities/bill/
--rw-r--r--   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/capabilities/bill/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     1531 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/capabilities/bill/documents.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.322515 woob-3.5/woob/tools/capabilities/housing/
--rw-r--r--   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/capabilities/housing/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     1255 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/capabilities/housing/housing.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     6252 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/capabilities/housing/housing_test.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.322515 woob-3.5/woob/tools/capabilities/messages/
--rw-r--r--   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/capabilities/messages/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     1774 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/capabilities/messages/threading.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     2865 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/capabilities/paste.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     4434 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/capabilities/recipe.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     1219 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/capabilities/streaminfo.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.326515 woob-3.5/woob/tools/capabilities/video/
--rw-r--r--   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/capabilities/video/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     2151 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/capabilities/video/ytdl.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.326515 woob-3.5/woob/tools/captcha/
--rw-r--r--   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/captcha/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    18694 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/captcha/virtkeyboard.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.326515 woob-3.5/woob/tools/config/
--rw-r--r--   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/config/__init__.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     2191 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/config/dbmconfig.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     4210 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/config/extra.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     1999 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/config/iconfig.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     4045 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/config/iniconfig.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     8576 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/config/sqliteconfig.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     2359 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/config/util.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     3663 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/config/yamlconfig.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    15496 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/date.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     1884 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/decorators.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     1085 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/html.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     3167 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/js.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     3644 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/json.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     2471 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/log.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     1450 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/lrudict.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     7204 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/misc.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     2661 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/newsfeed.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     1703 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/packaging.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     1910 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/path.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    18717 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/pdf.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    13828 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/regex_helper.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     2261 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/storage.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     3851 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/test.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     2602 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/tokenizer.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)     4149 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/url.py
--rw-r--r--   0 rom1      (1000) rom1      (1000)    10617 2023-04-08 10:13:23.000000 woob-3.5/woob/tools/value.py
-drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-04-08 10:13:26.302515 woob-3.5/woob.egg-info/
--rw-r--r--   0 rom1      (1000) rom1      (1000)     4526 2023-04-08 10:13:26.000000 woob-3.5/woob.egg-info/PKG-INFO
--rw-r--r--   0 rom1      (1000) rom1      (1000)     7469 2023-04-08 10:13:26.000000 woob-3.5/woob.egg-info/SOURCES.txt
--rw-r--r--   0 rom1      (1000) rom1      (1000)        1 2023-04-08 10:13:26.000000 woob-3.5/woob.egg-info/dependency_links.txt
--rw-r--r--   0 rom1      (1000) rom1      (1000)       61 2023-04-08 10:13:26.000000 woob-3.5/woob.egg-info/entry_points.txt
--rw-r--r--   0 rom1      (1000) rom1      (1000)      110 2023-04-08 10:13:26.000000 woob-3.5/woob.egg-info/requires.txt
--rw-r--r--   0 rom1      (1000) rom1      (1000)       12 2023-04-08 10:13:26.000000 woob-3.5/woob.egg-info/top_level.txt
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.233642 woob-3.6/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    12426 2023-05-23 13:50:40.000000 woob-3.6/AUTHORS
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    35149 2023-05-23 13:50:40.000000 woob-3.6/COPYING
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     7652 2023-05-23 13:50:40.000000 woob-3.6/COPYING.LESSER
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     4576 2023-05-23 13:50:43.233642 woob-3.6/PKG-INFO
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     3164 2023-05-23 13:50:40.000000 woob-3.6/README.rst
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     3023 2023-05-23 13:50:40.000000 woob-3.6/pyproject.toml
+-rw-r--r--   0 rom1      (1000) rom1      (1000)       38 2023-05-23 13:50:43.233642 woob-3.6/setup.cfg
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.213642 woob-3.6/weboob/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     1898 2023-05-23 13:50:40.000000 woob-3.6/weboob/__init__.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.213642 woob-3.6/woob/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      176 2023-05-23 13:50:40.000000 woob-3.6/woob/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)       49 2023-05-23 13:50:40.000000 woob-3.6/woob/__main__.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.213642 woob-3.6/woob/applications/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)       66 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/__init__.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.213642 woob-3.6/woob/applications/bands/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      757 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/bands/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     6527 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/bands/bands.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.213642 woob-3.6/woob/applications/bank/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      754 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/bank/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    37071 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/bank/bank.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.213642 woob-3.6/woob/applications/bill/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      753 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/bill/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    11124 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/bill/bill.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.213642 woob-3.6/woob/applications/books/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      757 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/books/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     2777 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/books/books.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.213642 woob-3.6/woob/applications/bugtracker/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      765 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/bugtracker/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    17645 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/bugtracker/bugtracker.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.213642 woob-3.6/woob/applications/calendar/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      754 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/calendar/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    16284 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/calendar/calendar.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.213642 woob-3.6/woob/applications/cinema/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      755 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/cinema/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    26526 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/cinema/cinema.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.213642 woob-3.6/woob/applications/cli/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      749 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/cli/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     1699 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/cli/cli.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.213642 woob-3.6/woob/applications/config/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      758 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/config/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    11169 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/config/config.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.213642 woob-3.6/woob/applications/contentedit/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      773 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/contentedit/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     7670 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/contentedit/contentedit.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.213642 woob-3.6/woob/applications/dating/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      758 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/dating/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    10199 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/dating/dating.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.217642 woob-3.6/woob/applications/debug/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      756 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/debug/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     3429 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/debug/debug.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.217642 woob-3.6/woob/applications/gallery/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      763 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/gallery/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     4703 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/gallery/gallery.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.217642 woob-3.6/woob/applications/gauge/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      753 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/gauge/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     6967 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/gauge/gauge.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.217642 woob-3.6/woob/applications/geolocip/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      764 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/geolocip/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     1557 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/geolocip/geolocip.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.217642 woob-3.6/woob/applications/housing/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)       58 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/housing/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    10239 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/housing/housing.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.217642 woob-3.6/woob/applications/job/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      739 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/job/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     4875 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/job/job.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.217642 woob-3.6/woob/applications/lyrics/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      755 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/lyrics/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     3526 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/lyrics/lyrics.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.217642 woob-3.6/woob/applications/main/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      854 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/main/__init__.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.217642 woob-3.6/woob/applications/money/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      744 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/money/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    34529 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/money/money.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.217642 woob-3.6/woob/applications/msg/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      751 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/msg/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    19113 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/msg/msg.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.217642 woob-3.6/woob/applications/parcel/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      753 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/parcel/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     7265 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/parcel/parcel.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.217642 woob-3.6/woob/applications/paste/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      755 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/paste/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     7499 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/paste/paste.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.217642 woob-3.6/woob/applications/pricecompare/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)       73 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/pricecompare/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     6102 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/pricecompare/pricecompare.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.217642 woob-3.6/woob/applications/radio/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      755 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/radio/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    16009 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/radio/radio.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.217642 woob-3.6/woob/applications/recipes/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      757 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/recipes/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     5429 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/recipes/recipes.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.217642 woob-3.6/woob/applications/repos/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      763 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/repos/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     8764 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/repos/repos.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.217642 woob-3.6/woob/applications/rpg/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      751 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/rpg/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     3921 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/rpg/rpg.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.217642 woob-3.6/woob/applications/shop/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      753 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/shop/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     6585 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/shop/shop.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.217642 woob-3.6/woob/applications/smtp/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      752 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/smtp/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    13512 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/smtp/smtp.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.217642 woob-3.6/woob/applications/subtitles/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      763 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/subtitles/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     7660 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/subtitles/subtitles.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.217642 woob-3.6/woob/applications/torrent/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      761 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/torrent/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     6572 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/torrent/torrent.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.221642 woob-3.6/woob/applications/translate/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      763 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/translate/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     5117 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/translate/translate.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.221642 woob-3.6/woob/applications/travel/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      758 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/travel/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     6717 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/travel/travel.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.221642 woob-3.6/woob/applications/video/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      757 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/video/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     4890 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/video/image2xterm.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    12099 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/video/video.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.221642 woob-3.6/woob/applications/weather/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      761 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/weather/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     5004 2023-05-23 13:50:40.000000 woob-3.6/woob/applications/weather/weather.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.221642 woob-3.6/woob/browser/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     1120 2023-05-23 13:50:40.000000 woob-3.6/woob/browser/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     2369 2023-05-23 13:50:40.000000 woob-3.6/woob/browser/adapters.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    60626 2023-05-23 13:50:40.000000 woob-3.6/woob/browser/browsers.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     3397 2023-05-23 13:50:40.000000 woob-3.6/woob/browser/cache.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     1819 2023-05-23 13:50:40.000000 woob-3.6/woob/browser/cloudscraper.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     1873 2023-05-23 13:50:40.000000 woob-3.6/woob/browser/cookies.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    21591 2023-05-23 13:50:40.000000 woob-3.6/woob/browser/elements.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     2063 2023-05-23 13:50:40.000000 woob-3.6/woob/browser/exceptions.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.221642 woob-3.6/woob/browser/filters/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      696 2023-05-23 13:50:40.000000 woob-3.6/woob/browser/filters/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     6156 2023-05-23 13:50:40.000000 woob-3.6/woob/browser/filters/base.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    10153 2023-05-23 13:50:40.000000 woob-3.6/woob/browser/filters/html.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     5985 2023-05-23 13:50:40.000000 woob-3.6/woob/browser/filters/javascript.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     3206 2023-05-23 13:50:40.000000 woob-3.6/woob/browser/filters/json.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    34455 2023-05-23 13:50:40.000000 woob-3.6/woob/browser/filters/standard.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     8589 2023-05-23 13:50:40.000000 woob-3.6/woob/browser/har.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     6751 2023-05-23 13:50:40.000000 woob-3.6/woob/browser/mfa.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    18247 2023-05-23 13:50:40.000000 woob-3.6/woob/browser/nss.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    32387 2023-05-23 13:50:40.000000 woob-3.6/woob/browser/pages.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     6009 2023-05-23 13:50:40.000000 woob-3.6/woob/browser/profiles.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     6661 2023-05-23 13:50:40.000000 woob-3.6/woob/browser/retry.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    28149 2023-05-23 13:50:40.000000 woob-3.6/woob/browser/selenium.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     5905 2023-05-23 13:50:40.000000 woob-3.6/woob/browser/sessions.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     4157 2023-05-23 13:50:40.000000 woob-3.6/woob/browser/switch.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    13829 2023-05-23 13:50:40.000000 woob-3.6/woob/browser/url.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.225642 woob-3.6/woob/capabilities/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      159 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     4101 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/account.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     2122 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/address.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     4650 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/audio.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     1858 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/audiostream.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     4651 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/bands.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.225642 woob-3.6/woob/capabilities/bank/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     3351 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/bank/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    22435 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/bank/base.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     3673 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/bank/pfm.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     2248 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/bank/rate.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    22863 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/bank/transfer.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     9467 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/bank/wealth.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    24516 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/base.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    14873 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/bill.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     9405 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/bugtracker.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     6472 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/calendar.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    10911 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/captcha.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     2306 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/chat.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     6302 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/cinema.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     5144 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/collection.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    10673 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/contact.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     2678 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/content.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     2204 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/date.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     3972 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/dating.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     3179 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/file.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     4252 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/gallery.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     3614 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/gauge.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     1883 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/geolocip.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     5341 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/housing.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     2962 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/image.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     3420 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/job.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     2178 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/library.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     1648 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/lyrics.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     6244 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/messages.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     2123 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/parcel.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     3648 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/paste.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     6402 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/picross.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     2620 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/pricecomparison.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     4189 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/profile.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     1690 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/radio.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     2724 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/recipe.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     8392 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/rpg.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     3898 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/shop.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     2277 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/subtitle.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     2453 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/torrent.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     2011 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/translate.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     4301 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/travel.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     1846 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/video.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     5403 2023-05-23 13:50:40.000000 woob-3.6/woob/capabilities/weather.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.229642 woob-3.6/woob/core/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     1798 2023-05-23 13:50:40.000000 woob-3.6/woob/core/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     7196 2023-05-23 13:50:40.000000 woob-3.6/woob/core/backendscfg.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     6082 2023-05-23 13:50:40.000000 woob-3.6/woob/core/bcall.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    10864 2023-05-23 13:50:40.000000 woob-3.6/woob/core/modules.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     1068 2023-05-23 13:50:40.000000 woob-3.6/woob/core/ouiboube.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    35876 2023-05-23 13:50:40.000000 woob-3.6/woob/core/repositories.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     1371 2023-05-23 13:50:40.000000 woob-3.6/woob/core/requests.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     5105 2023-05-23 13:50:40.000000 woob-3.6/woob/core/scheduler.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    21819 2023-05-23 13:50:40.000000 woob-3.6/woob/core/woob.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    18186 2023-05-23 13:50:40.000000 woob-3.6/woob/exceptions.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     3259 2023-05-23 13:50:40.000000 woob-3.6/woob/launcher.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.229642 woob-3.6/woob/tools/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)       66 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/__init__.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.229642 woob-3.6/woob/tools/application/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)       66 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/application/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    19930 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/application/base.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     1364 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/application/captcha.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    29102 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/application/console.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.233642 woob-3.6/woob/tools/application/formatters/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/application/formatters/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     1622 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/application/formatters/csv.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     9448 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/application/formatters/iformatter.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     1540 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/application/formatters/json.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     2572 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/application/formatters/load.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     1451 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/application/formatters/multiline.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     1240 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/application/formatters/simple.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     3437 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/application/formatters/table.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     1799 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/application/javascript.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     6678 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/application/media_player.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     1435 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/application/pretty.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    53924 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/application/repl.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     5935 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/application/results.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    20774 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/backend.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.233642 woob-3.6/woob/tools/capabilities/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/capabilities/__init__.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.233642 woob-3.6/woob/tools/capabilities/audio/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/capabilities/audio/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     1323 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/capabilities/audio/audio.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.233642 woob-3.6/woob/tools/capabilities/bank/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/capabilities/bank/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      938 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/capabilities/bank/bank_transfer.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     3770 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/capabilities/bank/data_matching.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     2939 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/capabilities/bank/iban.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     4601 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/capabilities/bank/investments.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     2485 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/capabilities/bank/sortcode.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     9839 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/capabilities/bank/test.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    12623 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/capabilities/bank/transactions.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.233642 woob-3.6/woob/tools/capabilities/bill/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/capabilities/bill/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     1531 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/capabilities/bill/documents.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.233642 woob-3.6/woob/tools/capabilities/housing/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/capabilities/housing/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     1255 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/capabilities/housing/housing.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     6252 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/capabilities/housing/housing_test.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.233642 woob-3.6/woob/tools/capabilities/messages/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/capabilities/messages/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     1774 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/capabilities/messages/threading.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     2865 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/capabilities/paste.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     4434 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/capabilities/recipe.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     1219 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/capabilities/streaminfo.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.233642 woob-3.6/woob/tools/capabilities/video/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/capabilities/video/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     2151 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/capabilities/video/ytdl.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.233642 woob-3.6/woob/tools/captcha/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/captcha/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    18305 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/captcha/virtkeyboard.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.233642 woob-3.6/woob/tools/config/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/config/__init__.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     2191 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/config/dbmconfig.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     4210 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/config/extra.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     1999 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/config/iconfig.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     4045 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/config/iniconfig.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     8576 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/config/sqliteconfig.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     2359 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/config/util.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     3663 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/config/yamlconfig.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    15496 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/date.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     1714 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/decorators.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     1085 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/html.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     3167 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/js.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     3645 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/json.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     2472 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/log.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     1450 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/lrudict.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     7204 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/misc.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     2661 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/newsfeed.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     1703 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/packaging.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     1910 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/path.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    18694 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/pdf.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    13828 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/regex_helper.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     2261 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/storage.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     3851 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/test.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     2602 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/tokenizer.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     4149 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/url.py
+-rw-r--r--   0 rom1      (1000) rom1      (1000)    12108 2023-05-23 13:50:40.000000 woob-3.6/woob/tools/value.py
+drwxr-xr-x   0 rom1      (1000) rom1      (1000)        0 2023-05-23 13:50:43.213642 woob-3.6/woob.egg-info/
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     4576 2023-05-23 13:50:43.000000 woob-3.6/woob.egg-info/PKG-INFO
+-rw-r--r--   0 rom1      (1000) rom1      (1000)     7505 2023-05-23 13:50:43.000000 woob-3.6/woob.egg-info/SOURCES.txt
+-rw-r--r--   0 rom1      (1000) rom1      (1000)        1 2023-05-23 13:50:43.000000 woob-3.6/woob.egg-info/dependency_links.txt
+-rw-r--r--   0 rom1      (1000) rom1      (1000)       52 2023-05-23 13:50:43.000000 woob-3.6/woob.egg-info/entry_points.txt
+-rw-r--r--   0 rom1      (1000) rom1      (1000)      121 2023-05-23 13:50:43.000000 woob-3.6/woob.egg-info/requires.txt
+-rw-r--r--   0 rom1      (1000) rom1      (1000)       12 2023-05-23 13:50:43.000000 woob-3.6/woob.egg-info/top_level.txt
```

### Comparing `woob-3.5/AUTHORS` & `woob-3.6/AUTHORS`

 * *Files identical despite different names*

### Comparing `woob-3.5/COPYING` & `woob-3.6/COPYING`

 * *Files identical despite different names*

### Comparing `woob-3.5/COPYING.LESSER` & `woob-3.6/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `woob-3.5/PKG-INFO` & `woob-3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: woob
-Version: 3.5
+Version: 3.6
 Summary: Woob, Web Outside Of Browsers
 Author-email: Romain Bignon <romain@woob.dev>
 License: LGPL-3.0-or-later
 Project-URL: Homepage, https://woob.tech
+Project-URL: Source, https://gitlab.com/woob/woob
 Project-URL: Release notes, https://gitlab.com/woob/woob/-/releases
 Project-URL: Documentation, https://woob.dev
 Project-URL: Bug Tracker, https://gitlab.com/woob/woob/-/issues
 Keywords: scraping,web,banking
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python
```

### Comparing `woob-3.5/README.rst` & `woob-3.6/README.rst`

 * *Files identical despite different names*

### Comparing `woob-3.5/pyproject.toml` & `woob-3.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 include = ["woob", "woob.*", "weboob"]
 
 [project]
 name = "woob"
-version = "3.5"
+version = "3.6"
 description = "Woob, Web Outside Of Browsers"
 authors = [
     { name="Romain Bignon", email="romain@woob.dev" }
 ]
 readme = "README.rst"
 license = { text="LGPL-3.0-or-later" }
 keywords = ["scraping", "web", "banking"]
@@ -39,30 +39,32 @@
     "PyYAML",
     "html2text >= 3.200",
     "unidecode",
     "Pillow",
     "Babel",
     "packaging ~= 23.0",
     "pycountry",
+    "rich ~= 13.0",
 ]
 
 [project.urls]
 "Homepage" = "https://woob.tech"
+"Source" = "https://gitlab.com/woob/woob"
 "Release notes" = "https://gitlab.com/woob/woob/-/releases"
 "Documentation" = "https://woob.dev"
 "Bug Tracker" = "https://gitlab.com/woob/woob/-/issues"
 
 [project.scripts]
-woob = "woob.applications.main:WoobMain.run"
+woob = "woob.launcher:Launcher.run"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
 tag_format = "$version"
 update_changelog_on_bump = true
-version = "3.5"
+version = "3.6"
 version_files = [
     "pyproject.toml:version",
 ]
 
 [tool.isort]
 lines_after_imports = 2
 include_trailing_comma = true
```

### Comparing `woob-3.5/weboob/__init__.py` & `woob-3.6/weboob/__init__.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/applications/bands/__init__.py` & `woob-3.6/woob/applications/bands/__init__.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/applications/bands/bands.py` & `woob-3.6/woob/applications/bands/bands.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         result+='---------------------------------------------------------------------------'
         return result.strip()
 
 
 
 class Appbands(ReplApplication):
     APPNAME = 'bands'
-    VERSION = '3.5'
+    VERSION = '3.6'
     COPYRIGHT = 'Copyright(C) 2018-YEAR Quentin Defenouillere'
     DESCRIPTION = "Console application allowing to display music bands and offer music suggestions."
     SHORT_DESCRIPTION = "display bands and suggestions"
     CAPS = CapBands
     DEFAULT_FORMATTER = 'table'
     EXTRA_FORMATTERS = {
         'band_search': BandListFormatter,
```

### Comparing `woob-3.5/woob/applications/bank/__init__.py` & `woob-3.6/woob/applications/bank/__init__.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/applications/bank/bank.py` & `woob-3.6/woob/applications/bank/bank.py`

 * *Files 0% similar despite different names*

```diff
@@ -518,15 +518,15 @@
             )
         )
 
 
 class Appbank(CaptchaMixin, ReplApplication):
     APPNAME = 'bank'
     OLD_APPNAME = 'boobank'
-    VERSION = '3.5'
+    VERSION = '3.6'
     COPYRIGHT = 'Copyright(C) 2010-YEAR Romain Bignon, Christophe Benz'
     CAPS = CapBank
     DESCRIPTION = "Console application allowing to list your bank accounts and get their balance, " \
                   "display accounts history and coming bank operations, and transfer money from an account to " \
                   "another (if available)."
     SHORT_DESCRIPTION = "manage bank accounts"
     EXTRA_FORMATTERS = {
```

### Comparing `woob-3.5/woob/applications/bill/__init__.py` & `woob-3.6/woob/applications/bill/__init__.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/applications/bill/bill.py` & `woob-3.6/woob/applications/bill/bill.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             return "%s - %s" % (obj.label, obj.renewdate.strftime('%d/%m/%y'))
         return obj.label
 
 
 class AppBill(CaptchaMixin, ReplApplication):
     APPNAME = 'bill'
     OLD_APPNAME = 'boobill'
-    VERSION = '3.5'
+    VERSION = '3.6'
     COPYRIGHT = 'Copyright(C) 2012-YEAR Florent Fourcot'
     DESCRIPTION = 'Console application allowing to get/download documents and bills.'
     SHORT_DESCRIPTION = "get/download documents and bills"
     CAPS = CapDocument
     COLLECTION_OBJECTS = (Subscription, )
     EXTRA_FORMATTERS = {'subscriptions':   SubscriptionsFormatter,
                         }
```

### Comparing `woob-3.5/woob/applications/books/__init__.py` & `woob-3.6/woob/applications/books/__init__.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/applications/books/books.py` & `woob-3.6/woob/applications/books/books.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         if obj.late:
             s += ' %sLATE!%s' % (self.RED, self.NC)
         return s
 
 
 class AppBooks(ReplApplication):
     APPNAME = 'books'
-    VERSION = '3.5'
+    VERSION = '3.6'
     COPYRIGHT = 'Copyright(C) 2012-YEAR Jeremy Monnet'
     CAPS = CapBook
     DESCRIPTION = "Console application allowing to list your books rented or booked at the library, " \
                   "book and search new ones, get your booking history (if available)."
     SHORT_DESCRIPTION = "manage rented books"
     EXTRA_FORMATTERS = {'rented_list':   RentedListFormatter,
                         }
```

### Comparing `woob-3.5/woob/applications/bugtracker/__init__.py` & `woob-3.6/woob/applications/bugtracker/__init__.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/applications/bugtracker/bugtracker.py` & `woob-3.6/woob/applications/bugtracker/bugtracker.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
     def get_description(self, obj):
         return obj.category
 
 
 class AppBugTracker(ReplApplication):
     APPNAME = 'bugtracker'
-    VERSION = '3.5'
+    VERSION = '3.6'
     COPYRIGHT = 'Copyright(C) 2011-YEAR Romain Bignon'
     DESCRIPTION = "Console application allowing to create, edit, view bug tracking issues."
     SHORT_DESCRIPTION = "manage bug tracking issues"
     CAPS = CapBugTracker
     EXTRA_FORMATTERS = {'issue_info': IssueFormatter,
                         'issues_list': IssuesListFormatter,
                        }
```

### Comparing `woob-3.5/woob/applications/calendar/__init__.py` & `woob-3.6/woob/applications/calendar/__init__.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/applications/calendar/calendar.py` & `woob-3.6/woob/applications/calendar/calendar.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
             result += 'Status: %s\n' % obj.status
 
         return result
 
 
 class AppCalendar(ReplApplication):
     APPNAME = 'calendar'
-    VERSION = '3.5'
+    VERSION = '3.6'
     COPYRIGHT = 'Copyright(C) 2012-YEAR Bezleputh'
     DESCRIPTION = "Console application to see upcoming events."
     SHORT_DESCRIPTION = "see upcoming events"
     CAPS = CapCalendarEvent
     EXTRA_FORMATTERS = {'upcoming_list': UpcomingListFormatter,
                         'upcoming': UpcomingFormatter,
                         'simple_upcoming': UpcomingSimpleFormatter,
```

### Comparing `woob-3.5/woob/applications/cinema/__init__.py` & `woob-3.6/woob/applications/cinema/__init__.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/applications/cinema/cinema.py` & `woob-3.6/woob/applications/cinema/cinema.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
     def get_description(self, obj):
         result = '\n%s' % obj.biography
         return result
 
 
 class AppCinema(ReplApplication):
     APPNAME = 'cinema'
-    VERSION = '3.5'
+    VERSION = '3.6'
     COPYRIGHT = 'Copyright(C) 2013-YEAR Julien Veyssier'
     DESCRIPTION = "Console application allowing to search for movies and persons on various cinema databases " \
                   ", list persons related to a movie, list movies related to a person and list common movies " \
                   "of two persons."
     SHORT_DESCRIPTION = "search movies and persons around cinema"
     CAPS = (CapCinema, CapTorrent, CapSubtitle)
     EXTRA_FORMATTERS = {'movie_list': MovieListFormatter,
```

### Comparing `woob-3.5/woob/applications/cli/__init__.py` & `woob-3.6/woob/applications/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/applications/cli/cli.py` & `woob-3.6/woob/applications/cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 __all__ = ['AppCli']
 
 
 class AppCli(ReplApplication):
     APPNAME = 'cli'
-    VERSION = '3.5'
+    VERSION = '3.6'
     COPYRIGHT = 'Copyright(C) 2010-YEAR Romain Bignon'
     SYNOPSIS =  'Usage: %prog [-dqv] [-b backends] [-cnfs] capability method [arguments..]\n'
     SYNOPSIS += '       %prog [--help] [--version]'
     DESCRIPTION = "Console application to call a specific method on backends " \
                   "which implement the given capability."
     SHORT_DESCRIPTION = "call a method on backends"
     DISABLE_REPL = True
```

### Comparing `woob-3.5/woob/applications/config/__init__.py` & `woob-3.6/woob/applications/config/__init__.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/applications/config/config.py` & `woob-3.6/woob/applications/config/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
                     result += '|                 | %s: %s\n' % (key, label)
         result += "'-----------------'\n"
         return result
 
 
 class AppConfig(ReplApplication):
     APPNAME = 'config'
-    VERSION = '3.5'
+    VERSION = '3.6'
     COPYRIGHT = 'Copyright(C) 2010-YEAR Christophe Benz, Romain Bignon'
     DESCRIPTION = "Console application to add/edit/remove backends, " \
                   "and to register new website accounts."
     SHORT_DESCRIPTION = "manage backends or register new accounts"
     EXTRA_FORMATTERS = {'info_formatter': ModuleInfoFormatter}
     COMMANDS_FORMATTERS = {'modules':     'table',
                            'list':        'table',
```

### Comparing `woob-3.5/woob/applications/contentedit/__init__.py` & `woob-3.6/woob/applications/contentedit/__init__.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/applications/contentedit/contentedit.py` & `woob-3.6/woob/applications/contentedit/contentedit.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 
 __all__ = ['AppContentEdit']
 
 
 class AppContentEdit(ReplApplication):
     APPNAME = 'contentedit'
-    VERSION = '3.5'
+    VERSION = '3.6'
     COPYRIGHT = 'Copyright(C) 2010-YEAR Romain Bignon'
     DESCRIPTION = "Console application allowing to display and edit contents on various websites."
     SHORT_DESCRIPTION = "manage websites content"
     CAPS = CapContent
 
     def do_edit(self, line):
         """
```

### Comparing `woob-3.5/woob/applications/dating/__init__.py` & `woob-3.6/woob/applications/dating/__init__.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/applications/dating/dating.py` & `woob-3.6/woob/applications/dating/dating.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     def get_description(self, event):
         if hasattr(event, 'message'):
             return event.message
 
 
 class AppDating(AppMsg):
     APPNAME = 'dating'
-    VERSION = '3.5'
+    VERSION = '3.6'
     COPYRIGHT = 'Copyright(C) 2010-YEAR Romain Bignon'
     DESCRIPTION = "Console application allowing to interact with various dating websites " \
                   "and to optimize seduction algorithmically."
     SHORT_DESCRIPTION = "interact with dating websites"
     STORAGE_FILENAME = 'dating.storage'
     STORAGE = {'optims': {}}
     CAPS = CapDating
```

### Comparing `woob-3.5/woob/applications/debug/__init__.py` & `woob-3.6/woob/applications/debug/__init__.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/applications/debug/debug.py` & `woob-3.6/woob/applications/debug/debug.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from optparse import OptionGroup
 
 from woob.tools.application.base import Application
 
 
 class AppDebug(Application):
     APPNAME = 'debug'
-    VERSION = '3.5'
+    VERSION = '3.6'
     COPYRIGHT = 'Copyright(C) 2010-YEAR Christophe Benz'
     DESCRIPTION = "Console application to debug backends."
     SHORT_DESCRIPTION = "debug backends"
 
     def __init__(self, option_parser=None):
         super(AppDebug, self).__init__(option_parser)
         options = OptionGroup(self._parser, 'Debug options')
```

### Comparing `woob-3.5/woob/applications/gallery/__init__.py` & `woob-3.6/woob/applications/gallery/__init__.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/applications/gallery/gallery.py` & `woob-3.6/woob/applications/gallery/gallery.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     def get_description(self, obj):
         if hasattr(obj, 'description') and obj.description:
             return obj.description
 
 
 class AppGallery(ReplApplication):
     APPNAME = 'gallery'
-    VERSION = '3.5'
+    VERSION = '3.6'
     COPYRIGHT = 'Copyright(C) 2011-YEAR Noé Rubinstein'
     DESCRIPTION = 'gallery browses and downloads web image galleries'
     SHORT_DESCRIPTION = 'browse and download web image galleries'
     CAPS = CapGallery
     EXTRA_FORMATTERS = {'gallery_list': GalleryListFormatter}
     COMMANDS_FORMATTERS = {'search': 'gallery_list', 'ls': 'gallery_list'}
     COLLECTION_OBJECTS = (BaseGallery, BaseImage, )
```

### Comparing `woob-3.5/woob/applications/gauge/__init__.py` & `woob-3.6/woob/applications/gauge/__init__.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/applications/gauge/gauge.py` & `woob-3.6/woob/applications/gauge/gauge.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
                                   self.colored('%-33s' % sensor.address[:33], 'yellow')
 
         return result
 
 
 class AppGauge(ReplApplication):
     APPNAME = 'gauge'
-    VERSION = '3.5'
+    VERSION = '3.6'
     COPYRIGHT = 'Copyright(C) 2013-YEAR Florent Fourcot'
     DESCRIPTION = "Console application allowing to display various sensors and gauges values."
     SHORT_DESCRIPTION = "display sensors and gauges values"
     CAPS = (CapGauge)
     DEFAULT_FORMATTER = 'table'
     EXTRA_FORMATTERS = {'gauge_list':   GaugeFormatter, }
     COMMANDS_FORMATTERS = {'search':    'gauge_list',
```

### Comparing `woob-3.5/woob/applications/geolocip/__init__.py` & `woob-3.6/woob/applications/geolocip/__init__.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/applications/geolocip/geolocip.py` & `woob-3.6/woob/applications/geolocip/geolocip.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,22 +20,22 @@
 
 
 __all__ = ['AppGeolocIP']
 
 
 class AppGeolocIP(ReplApplication):
     APPNAME = 'geolocip'
-    VERSION = '3.5'
+    VERSION = '3.6'
     COPYRIGHT = 'Copyright(C) 2010-YEAR Romain Bignon'
     DESCRIPTION = "Console application allowing to geolocalize IP addresses."
     SHORT_DESCRIPTION = "geolocalize IP addresses"
     CAPS = CapGeolocIp
 
     def main(self, argv):
         if len(argv) < 2:
             print('Syntax: %s ipaddr' % argv[0], file=self.stderr)
             return 2
 
         for location in self.do('get_location', argv[1]):
             if location.lt and location.lg:
-                location.osmlink = 'http://www.openstreetmap.org/?mlat=%s&mlon=%s#map=13/%s/%s' % (location.lt, location.lg, location.lt, location.lg)
+                location.osmlink = 'https://www.openstreetmap.org/?mlat=%s&mlon=%s#map=13/%s/%s' % (location.lt, location.lg, location.lt, location.lg)
             self.format(location)
```

### Comparing `woob-3.5/woob/applications/housing/housing.py` & `woob-3.6/woob/applications/housing/housing.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
             result += '%s - ' % obj.date.strftime('%Y-%m-%d')
         result += obj.text
         return result
 
 
 class AppHousing(ReplApplication):
     APPNAME = 'housing'
-    VERSION = '3.5'
+    VERSION = '3.6'
     COPYRIGHT = 'Copyright(C) 2012-YEAR Romain Bignon'
     DESCRIPTION = "Console application to search for housing."
     SHORT_DESCRIPTION = "search for housing"
     CAPS = CapHousing
     CONFIG = {'queries': {}}
     EXTRA_FORMATTERS = {'housing_list': HousingListFormatter,
                         'housing':      HousingFormatter,
```

### Comparing `woob-3.5/woob/applications/job/__init__.py` & `woob-3.6/woob/applications/job/__init__.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/applications/job/job.py` & `woob-3.6/woob/applications/job/job.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         if hasattr(obj, 'contract_type') and obj.contract_type:
             result += '\tContract : %s\n' % obj.contract_type
         return result.strip('\n\t')
 
 
 class AppJob(ReplApplication):
     APPNAME = 'job'
-    VERSION = '3.5'
+    VERSION = '3.6'
     COPYRIGHT = 'Copyright(C) 2012-YEAR Bezleputh'
     DESCRIPTION = "Console application to search for a job."
     SHORT_DESCRIPTION = "search for a job"
     CAPS = CapJob
     EXTRA_FORMATTERS = {'job_advert_list': JobAdvertListFormatter,
                         'job_advert': JobAdvertFormatter,
                         }
```

### Comparing `woob-3.5/woob/applications/lyrics/__init__.py` & `woob-3.6/woob/applications/lyrics/__init__.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/applications/lyrics/lyrics.py` & `woob-3.6/woob/applications/lyrics/lyrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         if not empty(obj.artist):
             artist = obj.artist
         return '%s' % artist
 
 
 class AppLyrics(ReplApplication):
     APPNAME = 'lyrics'
-    VERSION = '3.5'
+    VERSION = '3.6'
     COPYRIGHT = 'Copyright(C) 2013-YEAR Julien Veyssier'
     DESCRIPTION = "Console application allowing to search for song lyrics on various websites."
     SHORT_DESCRIPTION = "search and display song lyrics"
     CAPS = CapLyrics
     EXTRA_FORMATTERS = {'lyrics_list': LyricsListFormatter,
                         'lyrics_get': LyricsGetFormatter,
                         }
```

### Comparing `woob-3.5/woob/applications/main/__init__.py` & `woob-3.6/woob/applications/radio/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with woob. If not, see <http://www.gnu.org/licenses/>.
 
 
-from .main import WoobMain
+from .radio import AppRadio
 
-__all__ = ['WoobMain']
+__all__ = ['AppRadio']
```

### Comparing `woob-3.5/woob/applications/main/main.py` & `woob-3.6/woob/launcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 # Copyright(C) 2009-2021  Romain Bignon
 #
 # This file is part of woob.
 #
 # woob is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
@@ -26,18 +25,18 @@
 
 try:
     import woob_applications
 except ImportError:
     woob_applications = None
 
 
-__all__ = ['WoobMain']
+__all__ = ['Launcher']
 
 
-class WoobMain:
+class Launcher:
     @classmethod
     def list_apps(cls):
         apps = set()
         for module in pkgutil.iter_modules(woob.applications.__path__):
             apps.add(module.name)
 
         if woob_applications:
@@ -63,16 +62,20 @@
 
     @classmethod
     def print_list(cls, app_list):
         print('usage: woob [--version] <command> [<args>]')
         print()
         print('Use one of this commands:')
         for app in app_list:
-            app_class = cls.load_app(app)
-            print('   %-15s %s' % (app_class.APPNAME, app_class.SHORT_DESCRIPTION))
+            try:
+                app_class = cls.load_app(app)
+            except ImportError as e:
+                print('   %-15s (unable to load: %s)' % (app, e))
+            else:
+                print('   %-15s %s' % (app_class.APPNAME, app_class.SHORT_DESCRIPTION))
         print()
         print('For more information about a command, use:')
         print('   $ man woob-<command>')
         print('or')
         print('   $ woob <command> --help')
 
     @classmethod
```

### Comparing `woob-3.5/woob/applications/money/__init__.py` & `woob-3.6/woob/applications/money/__init__.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/applications/money/money.py` & `woob-3.6/woob/applications/money/money.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,15 +288,15 @@
         if self.stdouterr != "":
             self.money.print(" ".join(self.cmd) + "\n" + self.stdouterr)
 
 
 class AppMoney(Appbank):
     APPNAME = 'money'
     OLD_APPNAME = 'boomoney'
-    VERSION = '3.5'
+    VERSION = '3.6'
     COPYRIGHT = 'Copyright(C) 2018-YEAR Bruno Chabrier'
     DESCRIPTION = "Console application that imports bank accounts into Microsoft Money"
     SHORT_DESCRIPTION = "import bank accounts into Microsoft Money"
 
     EXTRA_FORMATTERS = {'list': ListFormatter, 'ops_list': MoneyOfxFormatter}
     COMMANDS_FORMATTERS = {'list': 'list', 'history': 'ops_list', 'coming': 'ops_list'}
```

### Comparing `woob-3.5/woob/applications/msg/__init__.py` & `woob-3.6/woob/applications/msg/__init__.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/applications/msg/msg.py` & `woob-3.6/woob/applications/msg/msg.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,15 +228,15 @@
     def format_obj(self, obj, alias=None):
         return obj.get_text()
 
 
 class AppMsg(ReplApplication):
     APPNAME = 'msg'
     OLD_APPNAME = 'boobmsg'
-    VERSION = '3.5'
+    VERSION = '3.6'
     COPYRIGHT = 'Copyright(C) 2010-YEAR Christophe Benz'
     DESCRIPTION = "Console application allowing to send messages on various websites and " \
                   "to display message threads and contents."
     SHORT_DESCRIPTION = "send and receive message threads"
     CAPS = CapMessages
     EXTRA_FORMATTERS = {'msglist':  MessagesListFormatter,
                         'msg':      MessageFormatter,
```

### Comparing `woob-3.5/woob/applications/parcel/__init__.py` & `woob-3.6/woob/applications/parcel/__init__.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/applications/parcel/parcel.py` & `woob-3.6/woob/applications/parcel/parcel.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
         return result
 
 
 class AppParcel(ReplApplication):
     APPNAME = 'parcel'
     OLD_APPNAME = 'parceloob'
-    VERSION = '3.5'
+    VERSION = '3.6'
     COPYRIGHT = 'Copyright(C) 2013-YEAR Romain Bignon'
     CAPS = CapParcel
     DESCRIPTION = "Console application to track your parcels."
     SHORT_DESCRIPTION = "manage your parcels"
     EXTRA_FORMATTERS = {'status':   StatusFormatter,
                         'history':  HistoryFormatter,
                        }
```

### Comparing `woob-3.5/woob/applications/paste/__init__.py` & `woob-3.6/woob/applications/paste/__init__.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/applications/paste/paste.py` & `woob-3.6/woob/applications/paste/paste.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 
 __all__ = ['AppPaste']
 
 
 class AppPaste(ReplApplication):
     APPNAME = 'paste'
-    VERSION = '3.5'
+    VERSION = '3.6'
     COPYRIGHT = 'Copyright(C) 2011-YEAR Romain Bignon'
     DESCRIPTION = "Console application allowing to post and get pastes from pastebins."
     SHORT_DESCRIPTION = "post and get pastes from pastebins"
     CAPS = CapPaste
 
     def main(self, argv):
         self.load_config()
```

### Comparing `woob-3.5/woob/applications/pricecompare/pricecompare.py` & `woob-3.6/woob/applications/pricecompare/pricecompare.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     def get_description(self, obj):
         if obj.date:
             return obj.date.strftime('%Y-%m-%d')
 
 
 class AppPriceCompare(ReplApplication):
     APPNAME = 'pricecompare'
-    VERSION = '3.5'
+    VERSION = '3.6'
     COPYRIGHT = 'Copyright(C) 2012-YEAR Romain Bignon'
     DESCRIPTION = "Console application to compare products."
     SHORT_DESCRIPTION = "compare products"
     DEFAULT_FORMATTER = 'table'
     EXTRA_FORMATTERS = {'prices':       PricesFormatter,
                         'price':        PriceFormatter,
                        }
```

### Comparing `woob-3.5/woob/applications/radio/__init__.py` & `woob-3.6/woob/applications/smtp/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with woob. If not, see <http://www.gnu.org/licenses/>.
 
 
-from .radio import AppRadio
+from .smtp import AppSmtp
 
-__all__ = ['AppRadio']
+__all__ = ['AppSmtp']
```

### Comparing `woob-3.5/woob/applications/radio/radio.py` & `woob-3.6/woob/applications/radio/radio.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
             result += '(%s)\r\n\t' % (song.id)
 
         return result
 
 
 class AppRadio(ReplApplication):
     APPNAME = 'radio'
-    VERSION = '3.5'
+    VERSION = '3.6'
     COPYRIGHT = 'Copyright(C) 2010-YEAR Romain Bignon\nCopyright(C) YEAR Pierre Maziere'
     DESCRIPTION = "Console application allowing to search for web radio stations, listen to them and get information " \
                   "like the current song."
     SHORT_DESCRIPTION = "search, show or listen to radio stations"
     CAPS = (CapRadio, CapAudio)
     EXTRA_FORMATTERS = {'radio_list': RadioListFormatter,
                         'song_list': SongListFormatter,
```

### Comparing `woob-3.5/woob/applications/recipes/__init__.py` & `woob-3.6/woob/applications/recipes/__init__.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/applications/recipes/recipes.py` & `woob-3.6/woob/applications/recipes/recipes.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         if not empty(obj.short_description):
             result += 'description: %s\n' % obj.short_description
         return result.strip()
 
 
 class AppRecipes(ReplApplication):
     APPNAME = 'recipes'
-    VERSION = '3.5'
+    VERSION = '3.6'
     COPYRIGHT = 'Copyright(C) 2013-YEAR Julien Veyssier'
     DESCRIPTION = "Console application allowing to search for recipes on various websites."
     SHORT_DESCRIPTION = "search and consult recipes"
     CAPS = CapRecipe
     EXTRA_FORMATTERS = {'recipe_list': RecipeListFormatter,
                         'recipe_info': RecipeInfoFormatter
                         }
```

### Comparing `woob-3.5/woob/applications/repos/__init__.py` & `woob-3.6/woob/applications/repos/__init__.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/applications/repos/repos.py` & `woob-3.6/woob/applications/repos/repos.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 
 __all__ = ['AppWoobRepos']
 
 
 class AppWoobRepos(ReplApplication):
     APPNAME = 'repos'
-    VERSION = '3.5'
+    VERSION = '3.6'
     COPYRIGHT = 'Copyright(C) 2012-YEAR Romain Bignon'
     DESCRIPTION = "Console application to manage a Woob Repository."
     SHORT_DESCRIPTION = "manage a woob repository"
     COMMANDS_FORMATTERS = {'backends':    'table',
                            'list':        'table',
                            }
     DISABLE_REPL = True
@@ -65,15 +65,15 @@
 
         if not os.path.exists(path):
             os.mkdir(path)
         elif not os.path.isdir(path):
             print('"%s" is not a directory' % path)
             return 1
 
-        r = Repository('http://')
+        r = Repository('https://')
         r.name = name
         r.maintainer = self.ask('Enter maintainer of the repository')
         r.save(os.path.join(path, r.INDEX))
         print('Repository "%s" created.' % path)
 
     def do_build(self, line):
         """
@@ -83,15 +83,15 @@
 
         Example:
         $ woob repos build $HOME/src/woob/modules /var/www/updates.woob.tech/0.a/
         """
         source_path, repo_path = self.parse_command_args(line, 2, 2)
         index_file = os.path.join(repo_path, Repository.INDEX)
 
-        r = Repository('http://')
+        r = Repository('https://')
         try:
             with open(index_file, 'r') as fp:
                 r.parse_index(fp)
         except IOError as e:
             print('Unable to open repository: %s' % e, file=self.stderr)
             print('Use the "create" command before.', file=self.stderr)
             return 1
```

### Comparing `woob-3.5/woob/applications/rpg/__init__.py` & `woob-3.6/woob/applications/rpg/__init__.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/applications/rpg/rpg.py` & `woob-3.6/woob/applications/rpg/rpg.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from woob.capabilities.rpg import CapRPG, Character, Skill, CharacterClass, CollectableItem
 from woob.tools.application.repl import ReplApplication, defaultcount
 
 
 class AppRPG(ReplApplication):
     APPNAME = 'rpg'
-    VERSION = '3.5'
+    VERSION = '3.6'
     COPYRIGHT = 'Copyright(C) 2019-YEAR Célande Adrien'
     CAPS = CapRPG
     DESCRIPTION = 'Console application allowing to list informations from a RPG.'
     SHORT_DESCRIPTION = 'manage RPG data'
     DEFAULT_FORMATTER = 'table'
     COLLECTION_OBJECTS = (Character, Skill, CharacterClass, CollectableItem, )
```

### Comparing `woob-3.5/woob/applications/shop/__init__.py` & `woob-3.6/woob/applications/shop/__init__.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/applications/shop/shop.py` & `woob-3.6/woob/applications/shop/shop.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
     def flush(self):
         self.output('-----------+-----------------+----------')
 
 
 class AppShop(ReplApplication):
     APPNAME = 'shop'
-    VERSION = '3.5'
+    VERSION = '3.6'
     COPYRIGHT = 'Copyright(C) 2015 Christophe Lampin'
     DESCRIPTION = 'Console application to obtain details and status of e-commerce orders.'
     SHORT_DESCRIPTION = "obtain details and status of e-commerce orders"
     CAPS = CapShop
     COLLECTION_OBJECTS = (Order, )
     EXTRA_FORMATTERS = {'orders':   OrdersFormatter,
                         'items':   ItemsFormatter,
```

### Comparing `woob-3.5/woob/applications/smtp/__init__.py` & `woob-3.6/woob/applications/travel/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with woob. If not, see <http://www.gnu.org/licenses/>.
 
 
-from .smtp import AppSmtp
+from .travel import AppTravel
 
-__all__ = ['AppSmtp']
+__all__ = ['AppTravel']
```

### Comparing `woob-3.5/woob/applications/smtp/smtp.py` & `woob-3.6/woob/applications/smtp/smtp.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             self._wait_to_stop()
         return True
 
 
 class AppSmtp(ReplApplication):
     APPNAME = 'smtp'
     OLD_APPNAME = 'monboob'
-    VERSION = '3.5'
+    VERSION = '3.6'
     COPYRIGHT = 'Copyright(C) 2010-YEAR Romain Bignon'
     DESCRIPTION = 'Daemon allowing to regularly check for new messages on various websites, ' \
                   'and send an email for each message, and post a reply to a message on a website.'
     SHORT_DESCRIPTION = "daemon to send and check messages"
     CONFIG = {'interval':  300,
               'domain':    'woob.example.org',
               'recipient': 'woob@example.org',
```

### Comparing `woob-3.5/woob/applications/subtitles/__init__.py` & `woob-3.6/woob/applications/subtitles/__init__.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/applications/subtitles/subtitles.py` & `woob-3.6/woob/applications/subtitles/subtitles.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         if not empty(obj.url):
             result += ' ; url : %s' % obj.url
         return result
 
 
 class AppSubtitles(ReplApplication):
     APPNAME = 'subtitles'
-    VERSION = '3.5'
+    VERSION = '3.6'
     COPYRIGHT = 'Copyright(C) 2013-YEAR Julien Veyssier'
     DESCRIPTION = "Console application allowing to search for subtitles on various services " \
                   "and download them."
     SHORT_DESCRIPTION = "search and download subtitles"
     CAPS = CapSubtitle
     EXTRA_FORMATTERS = {'subtitle_list': SubtitleListFormatter,
                         'subtitle_info': SubtitleInfoFormatter
```

### Comparing `woob-3.5/woob/applications/torrent/__init__.py` & `woob-3.6/woob/applications/torrent/__init__.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/applications/torrent/torrent.py` & `woob-3.6/woob/applications/torrent/torrent.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         return '%s   (Seed: %s / Leech: %s)' % (size,
                                                 self._get_color(obj.seeders),
                                                 self._get_color(obj.leechers))
 
 
 class AppTorrent(ReplApplication):
     APPNAME = 'torrent'
-    VERSION = '3.5'
+    VERSION = '3.6'
     COPYRIGHT = 'Copyright(C) 2010-YEAR Romain Bignon'
     DESCRIPTION = "Console application allowing to search for torrents on various trackers " \
                   "and download .torrent files."
     SHORT_DESCRIPTION = "search and download torrents"
     CAPS = CapTorrent
     EXTRA_FORMATTERS = {'torrent_list': TorrentListFormatter,
                         'torrent_info': TorrentInfoFormatter,
```

### Comparing `woob-3.5/woob/applications/translate/__init__.py` & `woob-3.6/woob/applications/translate/__init__.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/applications/translate/translate.py` & `woob-3.6/woob/applications/translate/translate.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
     def format_obj(self, obj, alias):
         return '<translation %s>\n%s\n</translation>' % (obj.backend, obj.text)
 
 
 class AppTranslate(ReplApplication):
     APPNAME = 'translate'
-    VERSION = '3.5'
+    VERSION = '3.6'
     COPYRIGHT = 'Copyright(C) 2012-YEAR Lucien Loiseau'
     DESCRIPTION = "Console application to translate text from one language to another"
     SHORT_DESCRIPTION = "translate text from one language to another"
     CAPS = CapTranslate
     EXTRA_FORMATTERS = {'translation': TranslationFormatter,
                         'xmltrans':    XmlTranslationFormatter}
     COMMANDS_FORMATTERS = {'translate': 'translation'}
```

### Comparing `woob-3.5/woob/applications/travel/__init__.py` & `woob-3.6/woob/browser/filters/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright(C) 2010-2011 Romain Bignon
+# Copyright(C) 2014 Romain Bignon
 #
 # This file is part of woob.
 #
 # woob is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -10,12 +10,7 @@
 # woob is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with woob. If not, see <http://www.gnu.org/licenses/>.
-
-
-from .travel import AppTravel
-
-__all__ = ['AppTravel']
```

### Comparing `woob-3.5/woob/applications/travel/travel.py` & `woob-3.6/woob/applications/travel/travel.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
     def get_title(self, obj):
         return obj.name
 
 
 class AppTravel(ReplApplication):
     APPNAME = 'travel'
-    VERSION = '3.5'
+    VERSION = '3.6'
     COPYRIGHT = 'Copyright(C) 2010-YEAR Romain Bignon'
     DESCRIPTION = "Console application allowing to search for train stations and get departure times."
     SHORT_DESCRIPTION = "search for train stations and departures"
     CAPS = CapTravel
     DEFAULT_FORMATTER = 'table'
     EXTRA_FORMATTERS = {'stations': StationsFormatter,
                         'departures': DeparturesFormatter,
```

### Comparing `woob-3.5/woob/applications/video/__init__.py` & `woob-3.6/woob/applications/video/__init__.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/applications/video/image2xterm.py` & `woob-3.6/woob/applications/video/image2xterm.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/applications/video/video.py` & `woob-3.6/woob/applications/video/video.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             result += image2xterm(BytesIO(obj.thumbnail.data), newsize=get_term_size())
 
         return result
 
 
 class AppVideo(ReplApplication):
     APPNAME = 'video'
-    VERSION = '3.5'
+    VERSION = '3.6'
     COPYRIGHT = 'Copyright(C) 2010-YEAR Christophe Benz, Romain Bignon, John Obbele'
     DESCRIPTION = "Console application allowing to search for videos on various websites, " \
                   "play and download them and get information."
     SHORT_DESCRIPTION = "search and play videos"
     CAPS = CapVideo
     EXTRA_FORMATTERS = {'video_list': VideoListFormatter}
     COMMANDS_FORMATTERS = {'search': 'video_list',
```

### Comparing `woob-3.5/woob/applications/weather/__init__.py` & `woob-3.6/woob/applications/weather/__init__.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/applications/weather/weather.py` & `woob-3.6/woob/applications/weather/weather.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
     def get_title(self, obj):
         return obj.name
 
 
 class AppWeather(ReplApplication):
     APPNAME = 'weather'
-    VERSION = '3.5'
+    VERSION = '3.6'
     COPYRIGHT = 'Copyright(C) 2010-YEAR Romain Bignon'
     DESCRIPTION = "Console application allowing to display weather and forecasts in your city."
     SHORT_DESCRIPTION = "display weather and forecasts"
     CAPS = CapWeather
     DEFAULT_FORMATTER = 'table'
     EXTRA_FORMATTERS = {'cities':    CitiesFormatter,
                         'current':   CurrentFormatter,
```

### Comparing `woob-3.5/woob/browser/__init__.py` & `woob-3.6/woob/browser/__init__.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/browser/adapters.py` & `woob-3.6/woob/browser/adapters.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/browser/browsers.py` & `woob-3.6/woob/browser/browsers.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 from logging import Logger
 from typing import Callable, Tuple, Type, Dict, Any, List, ClassVar
 
 import os
 from copy import copy, deepcopy
 import inspect
 from datetime import datetime, timedelta
-from requests import PreparedRequest
 from threading import Lock
 from urllib.parse import urlparse, urljoin, urlencode, parse_qsl
 import http
 from uuid import uuid4
 import warnings
 import tempfile
 import mimetypes
@@ -61,24 +60,33 @@
 from .pages import NextPage
 from .url import URL, normalize_url
 
 
 class Browser:
     """
     Simple browser class.
-    Act like a browser, and don't try to do too much.
+    Acts like a browser, and doesn't try to do too much.
+
+    >>> with Browser() as browser:
+    ...     browser.open('https://example.org')
+    ...
+    <Response [200]>
 
     :param logger: parent logger (optional)
     :type logger: :py:class:`logging.Logger`
     :param proxy: use a proxy (dictionary with http/https as key and URI as value) (optional)
     :type proxy: dict
     :param responses_dirname: save responses to this directory (optional)
     :type responses_dirname: str
     :param proxy_headers: headers to supply to proxy (optional)
     :type proxy_headers: dict
+    :param verify: either a boolean, in which case it controls whether we verify the server’s
+        TLS certificate, or a string, in which case it must be a path to a CA bundle to use.
+        Defaults will use the :attr:`Browser.VERIFY` attribute.
+    :type verify: `None`, `bool` or `str`
     """
 
     PROFILE: ClassVar[Profile] = Firefox()
     """
     Default profile used by browser to navigate on websites.
     """
 
@@ -93,15 +101,18 @@
     time in lesser than this value.
     """
 
     VERIFY: ClassVar[bool | str] = True
     """
     Check SSL certificates.
 
-    If this is a string, path to the certificate.
+    If this is a string, path to the certificate or the CA bundle.
+
+    Note that this value may be overriden by the ``verify`` argument on the
+    constructor.
     """
 
     MAX_RETRIES: ClassVar[int] = 2
     """
     Maximum retries on failed requests.
     """
 
@@ -123,15 +134,15 @@
     Adapter class to use.
     """
 
     COOKIE_POLICY: ClassVar[http.cookiejar.CookiePolicy | None] = None
     """
     Default CookieJar policy.
 
-    Example: :class:`woob.browser.cookies.BlockAllCookies()`
+    Example: :class:`~woob.browser.cookies.BlockAllCookies()`
     """
 
     @classmethod
     def asset(cls, localfile: str) -> str:
         """
         Absolute file path for a module local file.
         """
@@ -152,15 +163,17 @@
     def __init__(
         self,
         logger: Logger | None = None,
         proxy: Dict[str, str] | None = None,
         responses_dirname: str | None = None,
         proxy_headers: Dict[str, str] | None = None,
         woob: None = None,
-        weboob: None = None
+        weboob: None = None,
+        *,
+        verify: bool | str | None = None,
     ):
 
         if woob is not None or weboob is not None:
             warnings.warn(
                 "Don't use the 'woob' and 'weboob' parameters, they will be removed in woob 4.0",
                 DeprecationWarning,
                 stacklevel=2,
@@ -171,15 +184,21 @@
         else:
             self.logger = getLogger("woob.browser")
 
         self.responses_dirname = responses_dirname
         self.responses_count = 0
         self.responses_lock = Lock()
 
-        self.verify = self.VERIFY
+        if self.logger.settings['ssl_insecure']:
+            self.verify = False
+        elif verify is not None:
+            self.verify = verify
+        else:
+            self.verify = self.VERIFY
+
         if isinstance(self.verify, str):
             self.verify = self.asset(self.verify)
 
         self.PROXIES = proxy or {}
         self.proxy_headers = proxy_headers or {}
         self._setup_session(self.PROFILE)
         self.url: str | None = None
@@ -189,21 +208,28 @@
         if self.responses_dirname is not None:
             self.har_manager = HARManager(self.responses_dirname, self.logger)
 
     def deinit(self):
         """
         Deinitialisation of the browser.
 
-        Call it when you stop to use the browser.
+        Call it when you stop to use the browser and you don't use it in a
+        context manager.
 
         Can be overrided by any subclass which wants to cleanup after browser
         usage.
         """
         self.session.close()
 
+    def __enter__(self):
+        return self
+
+    def __exit__(self, *args):
+        self.deinit()
+
     def set_normalized_url(self, response: requests.Response, **kwargs):
         """
         Set the normalized URL on the response.
 
         :param response: the response to change
         :type response: :class:`requests.Response`
         """
@@ -246,20 +272,17 @@
             self.responses_count += 1
 
         response_filepath = slug
 
         if os.environ.get('WOOB_USE_OBSOLETE_RESPONSES_DIR') == '1':
             # get the content-type, remove optionnal charset part
             mimetype = response.headers.get('Content-Type', '').split(';')[0]
-            # due to http://bugs.python.org/issue1043134
-            if mimetype == 'text/plain':
-                ext = '.txt'
-            else:
-                # try to get an extension (and avoid adding 'None')
-                ext = mimetypes.guess_extension(mimetype, False) or ''
+
+            # try to get an extension (and avoid adding 'None')
+            ext = mimetypes.guess_extension(mimetype, False) or ''
 
             filename = '%02d-%d-%s%s' % \
                 (counter, response.status_code, slug, ext)
 
             response_filepath = os.path.join(self.responses_dirname, filename)
 
             request = response.request
@@ -317,15 +340,16 @@
         """
         Set up a python3-requests session for our usage.
         """
         session = self._create_session()
 
         session.proxies = self.PROXIES
 
-        session.verify = not self.logger.settings['ssl_insecure'] and self.verify
+        session.verify = self.verify
+
         if not session.verify:
             try:
                 urllib3.disable_warnings()
             except AttributeError:
                 # urllib3 is too old, warnings won't be disable
                 pass
 
@@ -357,22 +381,25 @@
         self.session = session
 
         session.cookies = WoobCookieJar()
         if self.COOKIE_POLICY:
             session.cookies.set_policy(self.COOKIE_POLICY)
 
     def set_profile(self, profile: Profile):
+        """
+        Update the profile of the session.
+        """
         profile.setup_session(self.session)
 
     def location(self, url: str | requests.Request, **kwargs) -> requests.Response:
         """
-        Like :meth:`open` but also changes the current URL and response.
+        Like :meth:`open()` but also changes the current URL and response.
         This is the most common method to request web pages.
 
-        Other than that, has the exact same behavior of open().
+        Other than that, has the exact same behavior of :meth:`open()`.
         """
         assert not kwargs.get('is_async'), "Please use open() instead of location() to make asynchronous requests."
         response = self.open(url, **kwargs)
         self.response = response
         self.url = self.response.url
         return response
 
@@ -385,60 +412,84 @@
         stream: bool | None = None,
         timeout: float | None = None,
         verify: str | bool | None = None,
         cert: str | Tuple[str, str] | None = None,
         proxies: Dict | None = None,
         data_encoding: str | None = None,
         is_async: bool = False,
-        callback: Callable[[requests.Response], requests.Response] = lambda response: response,
+        callback: Callable[[requests.Response], requests.Response] | None = None,
         **kwargs
     ) -> requests.Response:
         """
         Make an HTTP request like a browser does:
          * follow redirects (unless disabled)
          * provide referrers (unless disabled)
 
-        Unless a `method` is explicitly provided, it makes a GET request,
+        Unless a ``method`` is explicitly provided, it makes a GET request,
         or a POST if data is not None,
-        An empty `data` (not None, like '' or {}) *will* make a POST.
+        An empty ``data`` (like ``''`` or ``{}``, not ``None``) *will* make a POST.
 
         It is a wrapper around session.request().
-        All session.request() options are available.
-        You should use location() or open() and not session.request(),
-        since it has some interesting additions, which are easily
-        individually disabled through the arguments.
+        All ``session.request()`` options are available.
+        You should use :meth:`location()` or :meth:`open()` and not ``session.request()``,
+        since it has some interesting additions, which are easily individually
+        disabled through the arguments.
 
-        Call this instead of location() if you do not want to "visit" the URL
+        Call this instead of :meth:`location()` if you do not want to "visit" the URL
         (for instance, you are downloading a file).
 
-        When `is_async` is True, open() returns a Future object (see
-        concurrent.futures for more details), which can be evaluated with its
-        result() method. If any exception is raised while processing request,
-        it is caught and re-raised when calling result().
+        When ``is_async`` is ``True``, :meth:`open()` returns a :py:class:`~concurrent.futures.Future` object (see
+        :py:mod:`concurrent.futures` for more details), which can be evaluated with its
+        :py:meth:`~concurrent.futures.Future.result()` method. If any exception is raised while processing request,
+        it is caught and re-raised when calling :py:meth:`~concurrent.futures.Future.result()`.
 
         For example:
 
-        >>> Browser().open('http://google.com', is_async=True).result().text # doctest: +SKIP
+        >>> Browser().open('https://google.com', is_async=True).result().text # doctest: +SKIP
 
         :param url: URL
-        :type url: str
-
-        :param data: POST data
-        :type url: str or dict or None
+        :param params: (optional) Dictionary, list of tuples or bytes to send
+            in the query string
+        :param data: (optional) Dictionary, list of tuples, bytes, or file-like
+            object to send in the body
+        :param json: (optional) A JSON serializable Python object to send in the body
+        :param headers: (optional) Dictionary of HTTP Headers to send
+        :param cookies: (optional) Dict or CookieJar object to send
+        :param files: (optional) Dictionary of ``'name': file-like-objects`` (or ``{'name': file-tuple}``) for multipart encoding upload.
+            ``file-tuple`` can be a 2-tuple ``('filename', fileobj)``, 3-tuple ``('filename', fileobj, 'content_type')``
+            or a 4-tuple ``('filename', fileobj, 'content_type', custom_headers)``, where ``'content-type'`` is a string
+            defining the content type of the given file and ``custom_headers`` a dict-like object containing additional headers
+            to add for the file.
+        :param auth: (optional) Auth tuple to enable Basic/Digest/Custom HTTP Auth.
 
-        :param referrer: Force referrer. False to disable sending it, None for guessing
+        :param referrer: (optional) Force referrer. False to disable sending it, None for guessing
         :type referrer: str or False or None
 
-        :param is_async: Process request in a non-blocking way
+        :param allow_redirects: (optional) if ``True``, follow HTTP redirects (default: ``True``)
+        :type allow_redirects: bool
+
+        :param stream: (optional) if ``False``, the response content will be immediately downloaded.
+        :param timeout: (optional) How many seconds to wait for the server to send data
+                        before giving up, as a float, or a tuple.
+        :type timeout: float or tuple
+        :param verify: (optional) Either a boolean, in which case it controls whether we verify
+                the server's TLS certificate, or a string, in which case it must be a path
+                to a CA bundle to use. If not provided, uses the :attr:`Browser.VERIFY` class attribute value, the
+                :attr:`Browser.verify` attribute one, or ``True``.
+        :param cert: (optional) if String, path to ssl client cert file (.pem). If Tuple, ('cert', 'key') pair.
+        :param proxies: (optional) Dictionary mapping protocol to the URL of the proxy.
+
+        :param is_async: (optional) Process request in a non-blocking way (default: ``False``)
         :type is_async: bool
 
-        :param callback: Callback to be called when request has finished,
+        :param callback: (optional) Callback to be called when request has finished,
                          with response as its first and only argument
-        :type callback: function
+        :type callback: callable
 
+        :return: :class:`requests.Response <Response>` object
         :rtype: :class:`requests.Response`
         """
 
         if isinstance(url, str):
             url = normalize_url(url)
         elif isinstance(url, requests.Request):
             url.url = normalize_url(url.url)
@@ -454,18 +505,20 @@
             if self.COOKIE_POLICY:
                 preq._cookies.set_policy(self.COOKIE_POLICY)
 
         if proxies is None:
             proxies = self.PROXIES
 
         if verify is None:
-            verify = not self.logger.settings['ssl_insecure'] and self.verify
+            verify = self.verify
 
         if timeout is None:
             timeout = self.TIMEOUT
+        if callback is None:
+            callback = lambda response: response
 
         # We define an inner_callback here in order to execute the same code
         # regardless of is_async param.
         def inner_callback(future, response):
             if allow_redirects:
                 response = self.handle_refresh(response)
 
@@ -519,15 +572,20 @@
             del kwargs['async']
         if 'is_async' in kwargs:
             del kwargs['is_async']
         return self.open(url, is_async=True, **kwargs)
 
     def raise_for_status(self, response: requests.Response):
         """
-        Like Response.raise_for_status but will use other classes if needed.
+        Like :meth:`requests.Response.raise_for_status()` but will use other
+        exception specific classes:
+
+        * :class:`~woob.browser.exceptions.HTTPNotFound` for 404
+        * :class:`~woob.browser.exceptions.ClientError` for 4xx errors
+        * :class:`~woob.browser.exceptions.ServerError` for 5xx errors
         """
         if 400 <= response.status_code < 500:
             http_error_msg = '%s Client Error: %s' % (response.status_code, response.reason)
             if response.status_code == 404:
                 raise HTTPNotFound(http_error_msg, response=response)
             raise ClientError(http_error_msg, response=response)
         elif 500 <= response.status_code < 600:
@@ -542,17 +600,17 @@
         url: str | requests.Request,
         *,
         referrer: str | None = None,
         data_encoding: str | None = None,
         **kwargs
     ) -> requests.Request:
         """
-        Does the same job as open(), but returns a Request without
+        Does the same job as :meth:`open()`, but returns a :class:`~requests.Request` without
         submitting it.
-        This allows further customization to the Request.
+        This allows further customization to the :class:`~requests.Request`.
         """
 
         url_string: str
         if isinstance(url, requests.Request):
             req = url
             url_string = req.url
         elif isinstance(url, str):
@@ -599,28 +657,28 @@
             # Yes, it is a misspelling.
             req.headers.setdefault('Referer', referrer)
 
         return req
 
     def prepare_request(self, req: requests.Request) -> requests.PreparedRequest:
         """
-        Get a prepared request from a Request object.
+        Get a prepared request from a :class:`~requests.Request` object.
 
         This method aims to be overloaded by children classes.
         """
         return self.session.prepare_request(req)
 
     REFRESH_RE = re.compile(r"^(?P<sleep>[\d\.]+)(;\s*url=[\"']?(?P<url>.*?)[\"']?)?$", re.IGNORECASE)
 
     def handle_refresh(self, response: requests.Response) -> requests.Response:
         """
         Called by open, to handle Refresh HTTP header.
 
         It only redirect to the refresh URL if the sleep time is inferior to
-        REFRESH_MAX.
+        :attr:`REFRESH_MAX`.
         """
         if 'Refresh' not in response.headers:
             return response
 
         m = self.REFRESH_RE.match(response.headers['Refresh'])
         if m:
             # XXX perhaps we should not redirect if the refresh url is equal to the current url.
@@ -704,40 +762,49 @@
             'url': self.url,
             'cookies': [make_cookie(c) for c in self.session.cookies],
         }
 
 
 class UrlNotAllowed(Exception):
     """
-    Raises by :class:`DomainBrowser` when `RESTRICT_URL` is set and trying to go
-    on an url not matching `BASEURL`.
+    Raises by :class:`DomainBrowser` when :attr:`~DomainBrowser.RESTRICT_URL` is set and trying to go
+    on an url not matching :attr:`~DomainBrowser.BASEURL`.
     """
 
 
 class DomainBrowser(Browser):
     """
     A browser that handles relative URLs and can have a base URL (usually a domain).
 
-    For instance self.location('/hello') will get http://woob.tech/hello
-    if BASEURL is 'http://woob.tech/'.
+    For instance ``self.location('/hello')`` will get https://woob.tech/hello
+    if :attr:`BASEURL` is ``'https://woob.tech/'``.
+
+    >>> class ExampleBrowser(DomainBrowser):
+    ...     BASEURL = 'https://example.org'
+    ...
+    >>> with ExampleBrowser() as browser:
+    ...     browser.open('/')
+    ...
+    <Response [200]>
     """
 
     BASEURL: str | None = None
     """
-    Base URL, e.g. 'http://woob.tech/' or 'https://woob.tech/'
-    See absurl().
+    Base URL, e.g. ``'https://woob.tech/'``.
+
+    See :meth:`absurl()`.
     """
 
     RESTRICT_URL: ClassVar[bool | List[str]] = False
     """
     URLs allowed to load.
-    This can be used to force SSL (if the BASEURL is SSL) or any other leakage.
-    Set to True to allow only URLs starting by the BASEURL.
+    This can be used to force SSL (if the :attr:`BASEURL` is SSL) or any other leakage.
+    Set to ``True`` to allow only URLs starting by the :attr:`BASEURL`.
     Set it to a list of allowed URLs if you have multiple allowed URLs.
-    More complex behavior is possible by overloading url_allowed()
+    More complex behavior is possible by overloading :meth:`url_allowed()`.
     """
 
     def __init__(
         self,
         baseurl: str | None = None,
         *args,
         **kwargs
@@ -763,19 +830,19 @@
             if url.startswith(restrict_url):
                 return True
         return False
 
     def absurl(self, uri: str, base: str | bool | None = None) -> str:
         """
         Get the absolute URL, relative to a base URL.
-        If base is None, it will try to use the current URL.
-        If there is no current URL, it will try to use BASEURL.
+        If base is ``None``, it will try to use the current URL.
+        If there is no current URL, it will try to use :attr:`BASEURL`.
 
-        If base is False, it will always try to use the current URL.
-        If base is True, it will always try to use BASEURL.
+        If base is ``False``, it will always try to use the current URL.
+        If base is ``True``, it will always try to use BASEURL.
 
         :param uri: URI to make absolute. It can be already absolute.
         :type uri: str
 
         :param base: Base absolute URL.
         :type base: str or None or False or True
 
@@ -818,43 +885,50 @@
         return self.location(self.BASEURL or self.absurl('/'))
 
 
 class PagesBrowser(DomainBrowser):
     r"""
     A browser which works pages and keep state of navigation.
 
-    To use it, you have to derive it and to create URL objects as class
-    attributes. When open() or location() are called, if the url matches
-    one of URL objects, it returns a Page object. In case of location(), it
-    stores it in self.page.
+    To use it, you have to derive it and to create :class:`~woob.browser.url.URL` objects as class attributes. When
+    :meth:`open()` or :meth:`location()` are called, if the url matches one of :class:`~woob.browser.url.URL` objects, it returns a
+    :class:`~woob.browser.pages.Page` object. In case of :meth:`location()`, it stores it in ``self.page``.
 
     Example:
 
-    >>> from .pages import HTMLPage
-    >>> class ListPage(HTMLPage):
-    ...     def get_items():
-    ...         return [el.attrib['id'] for el in self.doc.xpath('//div[@id="items"]/div')]
-    ...
-    >>> class ItemPage(HTMLPage):
-    ...     pass
-    ...
-    >>> class MyBrowser(PagesBrowser):
-    ...     BASEURL = 'http://example.org/'
-    ...     list = URL('list-items', ListPage)
-    ...     item = URL('item/view/(?P<id>\d+)', ItemPage)
-    ...
-    >>> MyBrowser().list.stay_or_go().get_items() # doctest: +SKIP
-    >>> bool(MyBrowser().list.match('http://example.org/list-items'))
-    True
-    >>> bool(MyBrowser().list.match('http://example.org/'))
-    False
-    >>> str(MyBrowser().item.build(id=42))
-    'http://example.org/item/view/42'
-
-    You can then use URL instances to go on pages.
+        >>> import re
+        >>> from .pages import HTMLPage
+        >>> class ListPage(HTMLPage):
+        ...     def get_items(self):
+        ...         for link in self.doc.xpath('//a[matches(@href, "list-\d+.html")]/@href'):
+        ...             yield re.match('list-(\d+).html', link).group(1)
+        ...
+        >>> class ItemPage(HTMLPage):
+        ...     def iter_values(self):
+        ...         for el in self.doc.xpath('//li'):
+        ...             yield el.text
+        ...
+        >>> class MyBrowser(PagesBrowser):
+        ...     BASEURL = 'https://woob.tech/tests/'
+        ...     list = URL(r'$', ListPage)
+        ...     item = URL(r'list-(?P<id>\d+)\.html', ItemPage)
+        ...
+        >>> b = MyBrowser()
+        >>> b.list.go()
+        <woob.browser.browsers.ListPage object at 0x...>
+        >>> b.page.url
+        'https://woob.tech/tests/'
+        >>> list(b.page.get_items())
+        ['1', '2']
+        >>> b.item.build(id=42)
+        'https://woob.tech/tests/list-42.html'
+        >>> b.item.go(id=1)
+        <woob.browser.browsers.ItemPage object at 0x...>
+        >>> list(b.page.iter_values())
+        ['One', 'Two']
     """
 
     _urls = None
 
     def __init__(self, *args, **kwargs):
         self._urls = OrderedDict()
         self.highlight_el = kwargs.pop('highlight_el', False)
@@ -902,17 +976,17 @@
                 del self._urls[key]
 
         super().__delattr__(key)
 
     def open(self, *args, **kwargs) -> requests.Response:
         """
         Same method than
-        :meth:`woob.browser.browsers.DomainBrowser.open`, but the
-        response contains an attribute `page` if the url matches any
-        :class:`URL` object.
+        :meth:`~woob.browser.browsers.DomainBrowser.open`, but the
+        response contains an attribute ``page`` if the url matches any
+        :class:`~woob.browser.url.URL` object.
         """
 
         callback = kwargs.pop('callback', lambda response: response)
         page_class = kwargs.pop('page', None)
 
         # Have to define a callback to seamlessly process synchronous and
         # asynchronous requests, see :meth:`Browser.open` and its `is_async`
@@ -945,18 +1019,18 @@
 
             return callback(response)
 
         return super(PagesBrowser, self).open(callback=internal_callback, *args, **kwargs)
 
     def location(self, *args, **kwargs) -> requests.Response:
         """
-        Same method than
-        :meth:`woob.browser.browsers.Browser.location`, but if the
-        url matches any :class:`URL` object, an attribute `page` is added to
-        response, and the attribute :attr:`PagesBrowser.page` is set.
+        Same method than :meth:`~woob.browser.browsers.Browser.location`, but
+        if the url matches any :class:`~woob.browser.url.URL` object, an
+        attribute ``page`` is added to response, and the attribute :attr:`page`
+        is set on the browser.
         """
         if self.page is not None:
             # Call leave hook.
             self.page.on_leave()
 
         response = self.open(*args, **kwargs)
 
@@ -971,18 +1045,18 @@
         # Returns self.response in case on_load recalls location()
         return self.response
 
     def pagination(self, func: Callable, *args, **kwargs):
         r"""
         This helper function can be used to handle pagination pages easily.
 
-        When the called function raises an exception :class:`NextPage`, it goes
+        When the called function raises an exception :class:`~woob.browser.pages.NextPage`, it goes
         on the wanted page and recall the function.
 
-        :class:`NextPage` constructor can take an url or a Request object.
+        :class:`~woob.browser.pages.NextPage` constructor can take an url or a Request object.
 
         >>> from .pages import HTMLPage
         >>> class Page(HTMLPage):
         ...     def iter_values(self):
         ...         for el in self.doc.xpath('//li'):
         ...             yield el.text
         ...         for next in self.doc.xpath('//a'):
@@ -993,14 +1067,16 @@
         ...     list = URL('/tests/list-(?P<pagenum>\d+).html', Page)
         ...
         >>> b = Browser()
         >>> b.list.go(pagenum=1) # doctest: +ELLIPSIS
         <woob.browser.browsers.Page object at 0x...>
         >>> list(b.pagination(lambda: b.page.iter_values()))
         ['One', 'Two', 'Three', 'Four']
+
+        .. note: consider using :func:`~woob.browser.pages.pagination` decorator instead.
         """
         while True:
             try:
                 for r in func(*args, **kwargs):
                     yield r
             except NextPage as e:
                 self.location(e.request)
@@ -1010,20 +1086,20 @@
 
 def need_login(func):
     """
     Decorator used to require to be logged to access to this function.
 
     This decorator can be used on any method whose first argument is a
     browser (typically a :class:`LoginBrowser`). It checks for the
-    `logged` attribute in the current browser's page: when this
+    ``logged`` attribute in the current browser's page: when this
     attribute is set to ``True`` (e.g., when the page inherits
-    :class:`LoggedPage`), then nothing special happens.
+    :class:`~woob.browser.pages.LoggedPage`), then nothing special happens.
 
     In all other cases (when the browser isn't on any defined page or
-    when the page's `logged` attribute is ``False``), the
+    when the page's ``logged`` attribute is ``False``), the
     :meth:`LoginBrowser.do_login` method of the browser is called before
     calling :`func`.
     """
 
     @wraps(func)
     def inner(browser: LoginBrowser, *args, **kwargs):
         if (
@@ -1198,36 +1274,42 @@
     def open(self, *args, **kwargs) -> requests.Response:
         """
         Do a JSON request.
 
         The "Content-Type" header is always set to "application/json".
 
         :param data: if specified, format as JSON and send as request body
-        :type data: :class:`dict`
+        :type data: dict
         :param headers: if specified, add these headers to the request
-        :type headers: :class:`dict`
+        :type headers: dict
         """
         return super().open(*args, **kwargs)
 
     def request(self, *args, **kwargs) -> requests.Response:
         """
         Do a JSON request and parse the response.
 
         :returns: a dict containing the parsed JSON server response
-        :rtype: :class:`dict`
+        :rtype: dict
         """
         return self.open(*args, **kwargs).json()
 
 
 class AbstractBrowserMissingParentError(Exception):
-    pass
+    """
+    .. deprecated:: 3.4
+       Don't use this class, import woob_modules.other_module.etc instead
+    """
 
 
 class MetaBrowser(type):
-    # we can remove this class as soon as we get rid of Abstract*
+    """
+    .. deprecated:: 3.4
+       Don't use this class, import woob_modules.other_module.etc instead
+    """
 
     _parent_attr_re = re.compile(r'^[^.]+\.(.*)\.([^.]+)$')
 
     def __new__(mcs, name, bases, dct):
         from woob.tools.backend import Module  # Here to avoid file wide circular dependency
 
         if name != 'AbstractBrowser' and AbstractBrowser in bases:
@@ -1488,57 +1570,57 @@
             'redirect_uri': self.redirect_uri,
             'client_id': self.client_id,
             'client_secret': self.client_secret,
         }
 
 
 class DigestMixin:
-    """Browser mixin to add a 'Digest' header compliant with RFC 3230 section 4.3.2."""
+    """Browser mixin to add a ``Digest`` header compliant with RFC 3230 section 4.3.2."""
 
     HTTP_DIGEST_ALGORITHM: str = 'SHA-256'
     """Digest algorithm used to obtain a hash of the request content.
 
     The only supported digest algorithm for now is 'SHA-256'.
     """
 
     HTTP_DIGEST_METHODS: tuple[str, ...] | None = ('GET', 'POST', 'PUT', 'DELETE')
-    """The list of HTTP methods on which to add a 'Digest' header.
+    """The list of HTTP methods on which to add a ``Digest`` header.
 
-    To add the 'Digest' header to all methods, set this constant to None.
+    To add the ``Digest`` header to all methods, set this constant to None.
     """
 
     HTTP_DIGEST_COMPACT_JSON: bool = False
     """If the content type of the request payload is JSON, compact it first."""
 
     def compute_digest_header(self, body: bytes) -> str:
-        """Compute the value of the 'Digest' header.
+        """Compute the value of the ``Digest`` header.
 
         :param body: The body to compute with.
-        :return: The computed 'Digest' header value.
+        :return: The computed ``Digest`` header value.
         """
         if self.HTTP_DIGEST_ALGORITHM == 'SHA-256':
             return 'SHA-256=' + base64.b64encode(sha256(body).digest()).decode()
 
         raise ValueError(f'Unhandled digest algorithm {self.HTTP_DIGEST_ALGORITHM!r}')
 
-    def add_digest_header(self, preq: PreparedRequest) -> None:
-        """Add the 'Digest' header to the prepared request.
+    def add_digest_header(self, preq: requests.PreparedRequest) -> None:
+        """Add the ``Digest`` header to the prepared request.
 
-        The 'Digest' header presence depends on the request:
+        The ``Digest`` header presence depends on the request:
 
-        - If the request has a 'HTTP_DIGEST_INCLUDE' header, the 'Digest' header is added.
-        - Otherwise, if the request has a 'HTTP_DIGEST_EXCLUDE' header, the 'Digest' header is not added.
-        - Otherwise, if HTTP_DIGEST_METHOD is an HTTP method list and the request method is not in said list,
-          the 'Digest' header is not added.
-        - Otherwise, the 'Digest' header is added.
+        - If the request has a ``HTTP_DIGEST_INCLUDE`` header, the ``Digest`` header is added.
+        - Otherwise, if the request has a ``HTTP_DIGEST_EXCLUDE`` header, the ``Digest`` header is not added.
+        - Otherwise, if :attr:`HTTP_DIGEST_METHOD` is an HTTP method list and the request method is not in said list,
+          the ``Digest`` header is not added.
+        - Otherwise, the ``Digest`` header is added.
 
-        Note that the 'HTTP_DIGEST_INCLUDE' and 'HTTP_DIGEST_EXCLUDE' headers are removed from the request before
+        Note that the ``HTTP_DIGEST_INCLUDE`` and ``HTTP_DIGEST_EXCLUDE`` headers are removed from the request before
         sending it.
 
-        :param preq: The prepared request on which the 'Digest' header is added.
+        :param preq: The prepared request on which the ``Digest`` header is added.
 
         .. code-block:: python
 
             class MyBrowser(DigestMixin, Browser):
                 HTTP_DIGEST_METHODS = ('POST', 'PUT', 'DELETE')
 
             my_browser = MyBrowser()
@@ -1561,11 +1643,14 @@
 
         if self.HTTP_DIGEST_COMPACT_JSON:
             if 'application/json' in preq.headers.get('Content-Type', ''):
                 body = json.dumps(json.loads(body), separators=(',', ':')).encode('utf-8')
 
         preq.headers['Digest'] = self.compute_digest_header(body)
 
-    def prepare_request(self, *args, **kwargs) -> PreparedRequest:
+    def prepare_request(self, *args, **kwargs) -> requests.PreparedRequest:
+        """
+        Get the prepared request with a ``Digest`` header.
+        """
         preq = super().prepare_request(*args, **kwargs)
         self.add_digest_header(preq)
         return preq
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `woob-3.5/woob/browser/cache.py` & `woob-3.6/woob/browser/cache.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/browser/cloudscraper.py` & `woob-3.6/woob/browser/cloudscraper.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/browser/cookies.py` & `woob-3.6/woob/browser/cookies.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/browser/elements.py` & `woob-3.6/woob/browser/elements.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,29 +21,40 @@
 import importlib
 import os
 import re
 import sys
 from collections import OrderedDict
 from copy import deepcopy
 import traceback
+import warnings
 
 import lxml.html
 
 from woob.tools.log import getLogger, DEBUG_FILTERS
 from woob.browser.pages import NextPage
 from woob.capabilities.base import FetchError
 
 from .filters.standard import _Filter, CleanText
 from .filters.html import AttributeNotFound, XPathNotFound
 from .filters.json import Dict
 
 
 __all__ = [
-    'DataError', 'AbstractElement', 'ListElement', 'ItemElement', 'TableElement', 'SkipItem',
+    'AbstractElement',
+    'DataError',
+    'DictElement',
+    'ItemElement',
     'ItemElementFromAbstractPage',
+    'ListElement',
+    'MetaAbstractItemElement',
+    'SkipItem',
+    'TableElement',
+    'generate_table_element',
+    'magic_highlight',
+    'method',
 ]
 
 
 def generate_table_element(doc, head_xpath, cleaner=CleanText):
     """
     Prints generated base code for TableElement/TableCell usage.
     It is intended for development purposes, typically in woob-debug.
@@ -332,37 +343,28 @@
 
         attrs['_class_file'], attrs['_class_line'] = traceback.extract_stack()[-2][:2]
         new_class = super().__new__(mcs, name, bases, attrs)
         new_class._attrs = _attrs + [f[0] for f in filters]
         return new_class
 
 
-class ItemElementRerootMixin:
-    """
-    Mixin used to reroot an ItemElement by defining a reroot_xpath.
-    """
-
-    reroot_xpath = None
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-        if self.reroot_xpath:
-            if hasattr(self.el, 'xpath'):
-                self.el = self.el.xpath(self.reroot_xpath)
-            elif isinstance(self.el, (dict, list)):
-                self.el = Dict.select(self.reroot_xpath.split('/'), self)
-
-
 class ItemElement(AbstractElement, metaclass=_ItemElementMeta):
     _attrs = None
     klass: Type | None = None
     validate: Callable[[Any], bool] | None = None
     skip_optional_fields_errors: bool = False
 
+    item_xpath: str | None = None
+    """The xpath to reroot the element in.
+
+    This will be evaluated only once the object and environment are set,
+    so it can be defined as a property using ``self.obj`` and ``self.env``,
+    i.e. call parameters.
+    """
+
     class Index:
         pass
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.obj: Any | None = None
         self.saved_attrib = {}  # safer way would be to clone lxml tree
@@ -386,14 +388,48 @@
             if not self.el.getroottree():
                 return False
         except AttributeError:
             return False
         else:
             return True
 
+    def reroot_element(self, el: Any) -> Any:
+        """Reroot a given element for parsing a given object.
+
+        This will be called once the object and environment is set.
+        """
+        item_xpath = self.item_xpath
+        if item_xpath is None:
+            # TODO: Remove 'reroot_xpath' references in Woob 4.x, as it has
+            # been renamed to 'item_xpath' when merging ItemElementRerootMixin
+            # back into ItemElement in 3.6.
+            try:
+                item_xpath = self.reroot_xpath
+            except AttributeError:
+                pass
+            else:
+                # Whether or not it has returned None, it is defined, and is
+                # such, should be warned as deprecated.
+                warnings.warn(
+                    "'reroot_xpath' has been placed into ItemElement "
+                    + "and renamed 'item_xpath', please rename the attribute "
+                    + "on your side as such; reading this attribute will be "
+                    + "removed in Woob 4.0",
+                    DeprecationWarning,
+                )
+
+        if item_xpath is None:
+            return el
+
+        if hasattr(el, 'xpath'):
+            return el.xpath(item_xpath)
+        elif isinstance(el, (dict, list)):
+            return Dict.select(item_xpath.split('/'), self)
+        return el
+
     def _write_highlighted(self):
         if not self.should_highlight():
             return
 
         responses_dirname = self.page.browser.responses_dirname
         html = lxml.html.tostring(self.el.getroottree().getroot())
 
@@ -409,41 +445,46 @@
         for key, value in kwargs.items():
             self.env[key] = value
 
         for obj in self:
             return obj
 
     def __iter__(self):
-        if not self.check_condition():
-            return
-
-        highlight = False
+        original_element = self.el
+        self.el = self.reroot_element(original_element)
         try:
-            if self.should_highlight():
-                self.saved_attrib[self.el] = dict(self.el.attrib)
-                self.el.attrib['style'] = 'color: white !important; background: orange !important;'
+            if not self.check_condition():
+                return
 
+            highlight = False
             try:
-                if self.obj is None:
-                    self.obj = self.build_object()
-                self.parse(self.el)
-                self.handle_loaders()
-                for attr in self._attrs:
-                    self.handle_attr(attr, getattr(self, 'obj_%s' % attr))
-            except SkipItem:
-                return
+                if self.should_highlight():
+                    self.saved_attrib[self.el] = dict(self.el.attrib)
+                    self.el.attrib['style'] = 'color: white !important; background: orange !important;'
+
+                try:
+                    if self.obj is None:
+                        self.obj = self.build_object()
+                    self.parse(self.el)
+                    self.handle_loaders()
+                    for attr in self._attrs:
+                        self.handle_attr(attr, getattr(self, 'obj_%s' % attr))
+                except SkipItem:
+                    return
 
-            if self.validate is not None and not self.validate(self.obj):
-                return
+                if self.validate is not None and not self.validate(self.obj):
+                    return
 
-            highlight = True
+                highlight = True
+            finally:
+                if highlight:
+                    self._write_highlighted()
+                self._restore_attrib()
         finally:
-            if highlight:
-                self._write_highlighted()
-            self._restore_attrib()
+            self.el = original_element
 
         yield self.obj
 
     def handle_attr(self, key: str, func):
         try:
             value = self.use_selector(func, key=key)
         except SkipItem as e:
@@ -589,7 +630,32 @@
     _, fn = tempfile.mkstemp(prefix='woob-highlight', suffix='.html')
     with open(fn, 'w') as fd:
         fd.write(html)
 
     print('Saved to %r' % fn)
     if open_browser:
         webbrowser.open('file://%s' % fn)
+
+
+def __getattr__(name: str) -> Any:
+    if name == 'ItemElementRerootMixin':
+        warnings.warn(
+            'ItemElementRerootMixin is deprecated: rerooting is now '
+            + 'allowed with ItemElement directly.',
+            DeprecationWarning,
+            stacklevel=2,
+        )
+
+        class ItemElementRerootMixin:
+            """No-op class kept for compatibility.
+
+            This existed because rerooting was only an option with this mixin.
+            Since Woob 3.5, rerooting is present in base ItemElement.
+            """
+
+        return ItemElementRerootMixin
+
+    raise AttributeError(f"module '{__name__}' has no attribute '{name}'")
+
+
+def __dir__() -> list[str]:
+    return sorted(list(__all__) + ['ItemElementRerootMixin'])
```

### Comparing `woob-3.5/woob/browser/exceptions.py` & `woob-3.6/woob/browser/exceptions.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/browser/filters/__init__.py` & `woob-3.6/woob/core/ouiboube.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright(C) 2014 Romain Bignon
+# Copyright(C) 2010-2021 Romain Bignon
 #
 # This file is part of woob.
 #
 # woob is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -10,7 +10,26 @@
 # woob is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with woob. If not, see <http://www.gnu.org/licenses/>.
+
+"""
+.. deprecated:: 3.0
+   Please use :mod:`woob.core.woob` instead.
+"""
+
+import warnings
+from .woob import WoobBase, Woob, VersionsMismatchError  # noqa
+
+__all__ = ["WoobBase", "Woob", "VersionsMismatchError", "Weboob", "WebNip"]
+
+warnings.warn(
+    'Please use woob.core.woob instead.',
+    DeprecationWarning,
+    stacklevel=2,
+)
+
+WebNip = WoobBase
+Weboob = Woob
```

### Comparing `woob-3.5/woob/browser/filters/base.py` & `woob-3.6/woob/browser/filters/base.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/browser/filters/html.py` & `woob-3.6/woob/browser/filters/html.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/browser/filters/javascript.py` & `woob-3.6/woob/browser/filters/javascript.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 class JSPayload(Filter):
     r"""
     Get Javascript code from tag's text, cleaned from all comments.
 
     It filters code in a such a way that corner cases are handled, such as
     comments in string literals and comments in comments.
 
-    The following snippet is borrowed from <http://ostermiller.org/findcomment.html>:
+    The following snippet is borrowed from <https://ostermiller.org/findcomment.html>:
 
     >>> JSPayload.filter('''someString = "An example comment: /* example */";
     ...
     ... // The comment around this code has been commented out.
     ... // /*
     ... some_code();
     ... // */''')
```

### Comparing `woob-3.5/woob/browser/filters/json.py` & `woob-3.6/woob/browser/filters/json.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,21 +29,28 @@
     def __repr__(self):
         return 'NOT_FOUND'
 
 _NOT_FOUND = NotFound()
 
 
 class Dict(Filter):
-    """
-    Filter to find elements in a dictionary
+    """Filter to find elements in a dictionary or list.
+
+    Note that a selector defined as None or an empty string will be equivalent
+    to selecting the root of the provided document, as for None.
 
-    :param selector: input selector to use on the object
-    :param default: default value is the element is not found, or if the type mismatch
+    :param selector: Input selector to use on the object.
+    :param default: Default value is an element of the chain is not found, or
+        if a type mismatch occurs.
 
     >>> d = {'a': {'b': 'c', 'd': None}}
+    >>> Dict('')(d)
+    {'a': {'b': 'c', 'd': None}}
+    >>> Dict()(d)
+    {'a': {'b': 'c', 'd': None}}
     >>> Dict('a/b')(d)
     'c'
     >>> Dict('a')(d)
     {'b': 'c', 'd': None}
     >>> Dict('notfound')(d)
     Traceback (most recent call last):
         ...
@@ -51,15 +58,15 @@
     >>> Dict('notfound', default=None)(d)
     >>>
     """
     def __init__(self,
                  selector: str | _Filter | Callable | Any | None = None,
                  default: Any = _NO_DEFAULT):
         super().__init__(default=default)
-        if selector is None:
+        if selector is None or selector == '':
             self.selector = []
         elif isinstance(selector, str):
             self.selector = selector.split('/')
         elif callable(selector):
             self.selector = [selector]
         else:
             self.selector = selector
```

### Comparing `woob-3.5/woob/browser/filters/standard.py` & `woob-3.6/woob/browser/filters/standard.py`

 * *Files 0% similar despite different names*

```diff
@@ -392,15 +392,15 @@
 
     If `replace_dots` is set to True, we remove all the dots. The ',' is used as decimal
     separator (often useful for French values)
 
     If `replace_dots` is a tuple, the first element will be used as the thousands separator,
     and the second as the decimal separator.
 
-    See http://en.wikipedia.org/wiki/Thousands_separator#Examples_of_use
+    See https://en.wikipedia.org/wiki/Thousands_separator#Examples_of_use
 
     For example, for the UK style (as in 1,234,567.89):
 
     >>> CleanDecimal('./td[1]', replace_dots=(',', '.'))  # doctest: +SKIP
     """
 
     def __init__(self, selector=None, replace_dots=False, sign=None, legacy=True, default=_NO_DEFAULT):
@@ -1043,15 +1043,15 @@
 class QueryValue(Filter):
     """
     Extract the value of a parameter from an URL with a query string.
 
     >>> from lxml.html import etree
     >>> from .html import Link
     >>> f = QueryValue(Link('//a'), 'id')
-    >>> f(etree.fromstring('<html><body><a href="http://example.org/view?id=1234"></a></body></html>')) == u'1234'
+    >>> f(etree.fromstring('<html><body><a href="https://example.org/view?id=1234"></a></body></html>')) == u'1234'
     True
     """
     def __init__(self, selector, key, default=_NO_DEFAULT):
         super(QueryValue, self).__init__(selector, default=default)
         self.querykey = key
 
     @debug()
```

### Comparing `woob-3.5/woob/browser/har.py` & `woob-3.6/woob/browser/har.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/browser/mfa.py` & `woob-3.6/woob/browser/mfa.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/browser/nss.py` & `woob-3.6/woob/browser/nss.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/browser/pages.py` & `woob-3.6/woob/browser/pages.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/browser/profiles.py` & `woob-3.6/woob/browser/profiles.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/browser/retry.py` & `woob-3.6/woob/browser/retry.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/browser/selenium.py` & `woob-3.6/woob/browser/selenium.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/browser/sessions.py` & `woob-3.6/woob/browser/sessions.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/browser/switch.py` & `woob-3.6/woob/browser/switch.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/browser/url.py` & `woob-3.6/woob/browser/url.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         **kwargs
     ) -> requests.Response | Page:
         """
         Request to go on this url only if we aren't already here.
 
         Arguments are optional parameters for url.
 
-        >>> url = URL('http://exawple.org/(?P<pagename>).html')
+        >>> url = URL('https://exawple.org/(?P<pagename>).html')
         >>> url.stay_or_go(pagename='index')
         """
         assert self.browser is not None
 
         if self.is_here(**kwargs):
             return self.browser.page
 
@@ -127,15 +127,15 @@
         **kwargs
     ) -> requests.Response | Page:
         """
         Request to go on this url.
 
         Arguments are optional parameters for url.
 
-        >>> url = URL('http://exawple.org/(?P<pagename>).html')
+        >>> url = URL('https://exawple.org/(?P<pagename>).html')
         >>> url.stay_or_go(pagename='index')
         """
         assert self.browser is not None
 
         r = self.browser.location(self.build(**kwargs), params=params, data=data, json=json, method=method,
                                   headers=headers or {})
         return r.page or r
@@ -153,15 +153,15 @@
         **kwargs
     ) -> requests.Response | Page:
         """
         Request to open on this url.
 
         Arguments are optional parameters for url.
 
-        >>> url = URL('http://exawple.org/(?P<pagename>).html')
+        >>> url = URL('https://exawple.org/(?P<pagename>).html')
         >>> url.open(pagename='index')
         """
         assert self.browser is not None
 
         r = self.browser.open(self.build(**kwargs), params=params, data=data, json=json, method=method, headers=headers or {}, is_async=is_async, callback=callback)
 
         if hasattr(r, 'page') and r.page:
@@ -387,16 +387,16 @@
 
 
 def normalize_url(url: str) -> str:
     """Normalize URL by lower-casing the domain and other fixes.
 
     Lower-cases the domain, removes the default port and a trailing dot.
 
-    >>> normalize_url('http://EXAMPLE:80')
-    'http://example'
+    >>> normalize_url('https://EXAMPLE:80')
+    'https://example'
     """
 
     def norm_domain(m):
         # don't use urlparse/urlunparse because it might do too much normalization
 
         auth, authsep, hostport = m.group(2).rpartition('@')
         host, portsep, port = hostport.partition(':')
```

### Comparing `woob-3.5/woob/capabilities/account.py` & `woob-3.6/woob/capabilities/account.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/address.py` & `woob-3.6/woob/capabilities/address.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/audio.py` & `woob-3.6/woob/capabilities/audio.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/audiostream.py` & `woob-3.6/woob/capabilities/audiostream.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/bands.py` & `woob-3.6/woob/capabilities/bands.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/bank/__init__.py` & `woob-3.6/woob/capabilities/bank/__init__.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/bank/base.py` & `woob-3.6/woob/capabilities/bank/base.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/bank/pfm.py` & `woob-3.6/woob/capabilities/bank/pfm.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/bank/rate.py` & `woob-3.6/woob/capabilities/bank/rate.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/bank/transfer.py` & `woob-3.6/woob/capabilities/bank/transfer.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/bank/wealth.py` & `woob-3.6/woob/capabilities/bank/wealth.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/base.py` & `woob-3.6/woob/capabilities/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -539,15 +539,15 @@
             date =      Field('Date of transfer', str, date, datetime)
             origin =    Field('Origin of transfer', int, str)
             recipient = Field('Recipient', int, str)
 
     The docstring is mandatory.
     """
 
-    id: str = ''
+    id: str | None = None
     backend: str | None = None
     _fields: Dict[str, Field] = {}
 
     # XXX remove it?
     url = StringField('url')
 
     def __init__(
```

### Comparing `woob-3.5/woob/capabilities/bill.py` & `woob-3.6/woob/capabilities/bill.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/bugtracker.py` & `woob-3.6/woob/capabilities/bugtracker.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/calendar.py` & `woob-3.6/woob/capabilities/calendar.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     EXPO = 'Exposition'
     SPECTACLE = 'Spectacle'
     FEST = 'Festival'
     SPORT = 'Sport'
 
 
 #the following elements deal with ICalendar stantdards
-#see http://fr.wikipedia.org/wiki/ICalendar#Ev.C3.A9nements_.28VEVENT.29
+#see https://fr.wikipedia.org/wiki/ICalendar#%C3%89v%C3%A9nements_(VEVENT)
 class TRANSP(Enum):
     OPAQUE = 'OPAQUE'
     TRANSPARENT = 'TRANSPARENT'
 
 
 class STATUS(Enum):
     TENTATIVE = 'TENTATIVE'
@@ -78,15 +78,15 @@
     max_entries = IntField('Max entry number')
     event_planner = StringField('Name of the event planner')
 
     city = compat_field('address', 'city')
     location = compat_field('address', 'street')
 
     #the following elements deal with ICalendar stantdards
-    #see http://fr.wikipedia.org/wiki/ICalendar#Ev.C3.A9nements_.28VEVENT.29
+    #see https://fr.wikipedia.org/wiki/ICalendar#%C3%89v%C3%A9nements_(VEVENT)
     sequence = IntField('Number of updates, the first is number 1')
 
     # (TENTATIVE, CONFIRMED, CANCELLED)
     status = EnumField('Status of the event', STATUS)
     # (OPAQUE, TRANSPARENT)
     transp = EnumField('Describes if event is available', TRANSP)
     # (AVAILABLE, NOTAVAILABLE, CLOSED)
```

### Comparing `woob-3.5/woob/capabilities/captcha.py` & `woob-3.6/woob/capabilities/captcha.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/chat.py` & `woob-3.6/woob/capabilities/chat.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/cinema.py` & `woob-3.6/woob/capabilities/cinema.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/collection.py` & `woob-3.6/woob/capabilities/collection.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/contact.py` & `woob-3.6/woob/capabilities/contact.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/content.py` & `woob-3.6/woob/capabilities/content.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/date.py` & `woob-3.6/woob/capabilities/date.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/dating.py` & `woob-3.6/woob/capabilities/dating.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/file.py` & `woob-3.6/woob/capabilities/file.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/gallery.py` & `woob-3.6/woob/capabilities/gallery.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/gauge.py` & `woob-3.6/woob/capabilities/gauge.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/geolocip.py` & `woob-3.6/woob/capabilities/geolocip.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/housing.py` & `woob-3.6/woob/capabilities/housing.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/image.py` & `woob-3.6/woob/capabilities/image.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/job.py` & `woob-3.6/woob/capabilities/job.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/library.py` & `woob-3.6/woob/capabilities/library.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/lyrics.py` & `woob-3.6/woob/capabilities/lyrics.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/messages.py` & `woob-3.6/woob/capabilities/messages.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/parcel.py` & `woob-3.6/woob/capabilities/parcel.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/paste.py` & `woob-3.6/woob/capabilities/paste.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/picross.py` & `woob-3.6/woob/capabilities/picross.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/pricecomparison.py` & `woob-3.6/woob/capabilities/pricecomparison.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/profile.py` & `woob-3.6/woob/capabilities/profile.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/radio.py` & `woob-3.6/woob/capabilities/radio.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/recipe.py` & `woob-3.6/woob/capabilities/recipe.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/rpg.py` & `woob-3.6/woob/capabilities/rpg.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/shop.py` & `woob-3.6/woob/capabilities/shop.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/subtitle.py` & `woob-3.6/woob/capabilities/subtitle.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/torrent.py` & `woob-3.6/woob/capabilities/torrent.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/translate.py` & `woob-3.6/woob/capabilities/translate.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/travel.py` & `woob-3.6/woob/capabilities/travel.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/video.py` & `woob-3.6/woob/capabilities/video.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/capabilities/weather.py` & `woob-3.6/woob/capabilities/weather.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/core/__init__.py` & `woob-3.6/woob/core/__init__.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/core/backendscfg.py` & `woob-3.6/woob/core/backendscfg.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/core/bcall.py` & `woob-3.6/woob/core/bcall.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/core/modules.py` & `woob-3.6/woob/core/modules.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,27 +252,27 @@
             module.path,
         ))
 
     def get_module_path(self, module_name):
         return self.path
 
     def check_version(self, module_name, module_spec):
-        woob_version = Version(self.version)
+        woob_version = Version(self.version) if self.version else None
 
         # For a directory module, module_spec.origin is
         # 'woob_modules/bnp/__init__.py' so get 'woob_modules/bnp'.
         # For a single-file module, module_spec.origin is
         # 'woob_modules/bnp.py' so get 'woob_modules/'.
         # In that case, that's not a problem, we can assume the parent
         # requirements.txt file applies on all single-file modules.
         requirements_path = Path(module_spec.origin).parent / 'requirements.txt'
 
         for name, spec in parse_requirements(requirements_path).items():
             if name == 'woob':
-                if woob_version not in spec:
+                if woob_version and woob_version not in spec:
                     # specific user friendly error message
                     raise ModuleLoadError(
                         module_name,
                         f"Module requires woob {spec}, but you use woob {self.version}'.\n"
                         "Hint: use 'woob update' or install a newer version of woob"
                     )
                 continue
@@ -284,15 +284,15 @@
                     module_name,
                     f'Module requires python package "{name}" but not installed.'
                 ) from exc
 
             if Version(pkg.version) not in spec:
                 raise ModuleLoadError(
                     module_name,
-                    f'Modure requires python package "{name}" {spec} but version {pkg.version} is installed'
+                    f'Module requires python package "{name}" {spec} but version {pkg.version} is installed'
                 )
 
 
 class RepositoryModulesLoader(ModulesLoader):
     """
     Load modules from repositories.
     """
```

### Comparing `woob-3.5/woob/core/ouiboube.py` & `woob-3.6/woob/tools/html.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright(C) 2010-2021 Romain Bignon
+# Copyright(C) 2010-2014 Romain Bignon
 #
 # This file is part of woob.
 #
 # woob is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -11,25 +11,26 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with woob. If not, see <http://www.gnu.org/licenses/>.
 
-"""
-.. deprecated:: 3.0
-   Please use :mod:`woob.core.woob` instead.
-"""
-
-import warnings
-from .woob import WoobBase, Woob, VersionsMismatchError  # noqa
-
-__all__ = ["WoobBase", "Woob", "VersionsMismatchError", "Weboob", "WebNip"]
-
-warnings.warn(
-    'Please use woob.core.woob instead.',
-    DeprecationWarning,
-    stacklevel=2,
-)
 
-WebNip = WoobBase
-Weboob = Woob
+__all__ = ['html2text']
+
+
+from html2text import HTML2Text
+
+
+def html2text(html, **options):
+    h = HTML2Text()
+    defaults = dict(
+        unicode_snob=True,
+        skip_internal_links=True,
+        inline_links=False,
+        links_each_paragraph=True,
+    )
+    defaults.update(options)
+    for k, v in defaults.items():
+        setattr(h, k, v)
+    return str(h.handle(html))
```

### Comparing `woob-3.5/woob/core/repositories.py` & `woob-3.6/woob/core/repositories.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/core/requests.py` & `woob-3.6/woob/core/requests.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/core/scheduler.py` & `woob-3.6/woob/core/scheduler.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/core/woob.py` & `woob-3.6/woob/core/woob.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/exceptions.py` & `woob-3.6/woob/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -544,15 +544,15 @@
     """
     def __init__(self, *args, **kwargs):
         warnings.warn(
             'Do not use this exception.',
             DeprecationWarning,
             stacklevel=2
         )
-        super().__init__(self, *args, **kwargs)
+        super().__init__(*args, **kwargs)
 
 
 __deprecated__ = {
     'ImageCaptchaQuestion': 'woob.capabilities.captcha.ImageCaptchaQuestion',
     'RecaptchaV2Question': 'woob.capabilities.captcha.RecaptchaV2Question',
     'RecaptchaQuestion': 'woob.capabilities.captcha.RecaptchaQuestion',
     'GeetestV4Question': 'woob.capabilities.captcha.GeetestV4Question',
```

### Comparing `woob-3.5/woob/tools/application/base.py` & `woob-3.6/woob/tools/application/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,15 +272,16 @@
         elif os.path.sep not in path:
             path = os.path.join(self.CONFDIR, path)
 
         self.config = klass(path)
         self.config.load(self.CONFIG)
 
         if int(self.config.get('use_nss', default=0)):
-            self.setup_nss()
+            # TODO Deprecated
+            print('Key "use_nss" is deprecated and will be ignored', file=sys.stderr)
 
         if int(self.config.get('export_session', default=0)):
             log_settings['export_session'] = True
 
     def main(self, argv):
         """
         Main method
@@ -424,15 +425,15 @@
         elif self.options.quiet:
             level = logging.ERROR
         else:
             level = logging.WARNING
         if self.options.insecure:
             log_settings['ssl_insecure'] = True
         if self.options.nss:
-            self.setup_nss()
+            print('--nss is deprecated and will be removed', file=sys.stderr)
         if self.options.ipversion:
             self.setup_ipversion()
 
         # this only matters to developers
         if not self.options.debug and not self.options.save_responses:
             warnings.simplefilter('ignore', category=ConversionWarning)
             warnings.simplefilter('ignore', category=FormFieldConversionWarning)
@@ -478,25 +479,14 @@
     def setup_logging(cls, level, handlers):
         logging.root.handlers = []
 
         logging.root.setLevel(level)
         for handler in handlers:
             logging.root.addHandler(handler)
 
-    def setup_nss(self):
-        from woob.browser.nss import (
-            init_nss, inject_in_urllib3, create_cert_db, certificate_db_filename,
-        )
-
-        path = self.CONFDIR
-        if not os.path.exists(os.path.join(path, certificate_db_filename())):
-            create_cert_db(path)
-        init_nss(path)
-        inject_in_urllib3()
-
     def setup_ipversion(self):
         import socket
         import requests.packages.urllib3.util.connection
         import urllib3.util.connection
 
         for module in (requests.packages.urllib3.util.connection, urllib3.util.connection):
             family = socket.AF_INET
```

### Comparing `woob-3.5/woob/tools/application/captcha.py` & `woob-3.6/woob/tools/application/captcha.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/application/console.py` & `woob-3.6/woob/tools/application/console.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,90 +23,139 @@
 import logging
 import shlex
 import subprocess
 from subprocess import check_output
 import sys
 import os
 from tempfile import NamedTemporaryFile
+import warnings
+
+from rich.progress import Progress, TaskProgressColumn, BarColumn, TextColumn
 
 from woob.capabilities import UserError
 from woob.capabilities.account import CapAccount, Account, AccountRegisterError
 from woob.core.backendscfg import BackendAlreadyExists
 from woob.core.repositories import IProgress
 from woob.exceptions import (
     BrowserUnavailable, BrowserIncorrectPassword, BrowserForbidden,
     BrowserSSLError, BrowserQuestion, BrowserHTTPSDowngrade,
     ModuleInstallError, ModuleLoadError, ActionNeeded, CaptchaQuestion,
     NeedInteractiveFor2FA,
 )
+from woob.tools.application.pretty import colored, NC, BOLD
 from woob.tools.value import Value, ValueBool, ValueFloat, ValueInt, ValueBackendPassword
-from woob.tools.misc import to_unicode
+from woob.tools.misc import to_unicode, classproperty
 
 from .base import Application, MoreResultsAvailable
 
 
 __all__ = ['ConsoleApplication', 'BackendNotGiven']
 
 
 class BackendNotGiven(Exception):
     def __init__(self, id, backends):
         self.id = id
         self.backends = sorted(backends)
-        super().__init__('Please specify a backend to use for this argument (%s@backend_name). '
-                'Availables: %s.' % (id, ', '.join(name for name, backend in backends)))
+        super().__init__(
+            'Please specify a backend to use for this argument (%s@backend_name). '
+            'Availables: %s.' % (id, ', '.join(name for name, backend in backends))
+        )
 
 
 class BackendNotFound(Exception):
     pass
 
 
 class ConsoleProgress(IProgress):
     def __init__(self, app):
         self.app = app
+        self._progress = None
+        self._progress_task = None
 
     def progress(self, percent, message):
-        try:
-            quiet = self.app.options.quiet
-        except AttributeError:
-            quiet = False
-        if not quiet:
-            self.app.stdout.write('=== [%3.0f%%] %s\n' % (percent*100, message))
+        if not self._progress:
+            self._progress = Progress(
+                TaskProgressColumn(),
+                BarColumn(),
+                TextColumn("[progress.description]{task.description}")
+            )
+            self._progress_task = self._progress.add_task(message, total=1)
+            self._progress.start()
+
+        self._progress.update(self._progress_task, advance=percent, description=message)
+
+        if percent == 1:
+            self._progress.stop()
+            self._progress = None
 
     def error(self, message):
-        self.app.stderr.write('ERROR: %s\n' % message)
+        if self._progress:
+            self._progress.stop()
 
-    def prompt(self, message):
-        return self.app.ask(message, default=True)
+        print(colored(f'ERROR: {message}', 'red'), file=self.app.stderr)
+
+        if self._progress:
+            self._progress.start()
+
+    def prompt(self, message: str, default: bool = True) -> bool:
+        try:
+            if self._progress:
+                self._progress.stop()
+            return self.app.ask(message, default=default)
+        finally:
+            if self._progress:
+                self._progress.start()
 
 
 class ConsoleApplication(Application):
     """
     Base application class for CLI applications.
     """
 
     CAPS = None
 
-    # shell escape strings
-    if sys.platform == 'win32' \
-            or not sys.stdout.isatty() \
-            or os.getenv('NO_COLOR') is not None \
-            or os.getenv('ANSI_COLORS_DISABLED') is not None:
-        #workaround to disable bold
-        BOLD   = ''
-        NC     = ''          # no color
-    else:
-        BOLD   = '[1m'
-        NC     = '[0m'    # no color
+    @classproperty
+    def BOLD(self):
+        """
+        .. deprecated:: 3.6
+            This attribute is deprecated, use :attr:`woob.tools.application.pretty.BOLD` instead.
+            That's also better to use :func:`woob.tools.application.pretty.colored`.
+        """
+        warnings.warn(
+            'Use woob.tools.application.pretty.BOLD instead.\n'
+            'That\'s also better to use woob.tools.application.pretty.colored.',
+            DeprecationWarning,
+            stacklevel=2
+        )
+        return BOLD
+
+    @classproperty
+    def NC(self):
+        """
+        .. deprecated:: 3.6
+            This attribute is deprecated, use :attr:`woob.tools.application.pretty.NC` instead.
+            That's also better to use :func:`woob.tools.application.pretty.colored`.
+        """
+        warnings.warn(
+            'Use woob.tools.application.pretty.NC instead.\n'
+            'That\'s also better to use woob.tools.application.pretty.colored.',
+            DeprecationWarning,
+            stacklevel=2
+        )
+        return NC
 
     def __init__(self, option_parser=None):
         super().__init__(option_parser)
         self.woob.requests.register('login', self.login_cb)
         self.enabled_backends = set()
-        self._parser.add_option('--auto-update', action='store_true',
-                                help='Automatically check for updates when a bug in a module is encountered')
+        self._parser.add_option(
+            '--auto-update',
+            action='store_true',
+            help='Automatically check for updates when a bug in a module is encountered'
+        )
 
     def login_cb(self, backend_name, value):
         return self.ask('[%s] %s' % (backend_name,
                         value.label),
                         masked=True,
                         default='',
                         regexp=value.regexp)
@@ -140,26 +189,23 @@
             self.enabled_backends.add(backend)
 
         self.check_loaded_backends()
 
         return ret
 
     def check_loaded_backends(self, default_config=None):
-        while len(self.enabled_backends) == 0:
-            print('Warning: there is currently no configured backend for %s' % self.APPNAME)
-            if not self.stdout.isatty() or not self.ask('Do you want to configure backends?', default=True):
-                return False
-
+        if len(self.enabled_backends) == 0:
+            print('There is currently no configured backend for %s' % self.APPNAME)
             self.prompt_create_backends(default_config)
 
         return True
 
     def prompt_create_backends(self, default_config=None):
         r = ''
-        while r != 'q':
+        while True:
             modules = []
             print('\nAvailable modules:')
             for name, info in sorted(self.woob.repositories.get_all_modules_info().items()):
                 if not self.is_module_loadable(info):
                     continue
                 modules.append(name)
                 loaded = ' '
@@ -167,47 +213,72 @@
                     if bi.NAME == name:
                         if loaded == ' ':
                             loaded = 'X'
                         elif loaded == 'X':
                             loaded = 2
                         else:
                             loaded += 1
-                print('%s%d)%s [%s] %s%-15s%s   %s' % (self.BOLD, len(modules), self.NC, loaded,
-                                                       self.BOLD, name, self.NC,
-                                                       info.description))
-            print('%sa) --all--%s               install all backends' % (self.BOLD, self.NC))
-            print('%sq)%s --stop--\n' % (self.BOLD, self.NC))
-            r = self.ask('Select a backend to create (q to stop)', regexp=r'^(\d+|q|a)$')
+                print(
+                    '%s) [%s] %s%s' % (
+                        colored('%2d' % len(modules), 'white', attrs=['bold']),
+                        colored(str(loaded), attrs=['bold']),
+                        colored('%-20s' % name, 'magenta', attrs=['bold']),
+                        colored(info.description, 'green')
+                    )
+                )
+
+            print(
+                ' %s) %s                 %s' % (
+                    colored('a', 'white', attrs=['bold']),
+                    colored('--all--', attrs=['bold']),
+                    colored('install all backends', 'green')
+                )
+            )
+            print(
+                ' %s) %s\n' % (
+                    colored('q', 'white', attrs=['bold']),
+                    colored('--stop--', attrs=['bold'])
+                )
+            )
+            r = self.ask('Select a backend to create', default='')
 
-            if str(r).isdigit():
-                i = int(r) - 1
-                if i < 0 or i >= len(modules):
-                    print('Error: %s is not a valid choice' % r, file=self.stderr)
-                    continue
-                name = modules[i]
-                try:
-                    inst = self.add_backend(name, name, default_config)
-                    if inst:
-                        self.load_backends(names=[inst])
-                except (KeyboardInterrupt, EOFError):
-                    print('\nAborted.')
-            elif r == 'a':
+            if r in ('q', ''):
+                break
+            if r == 'a':
                 try:
                     for name in modules:
                         if name in [b.NAME for b in self.woob.iter_backends()]:
                             continue
                         inst = self.add_backend(name, name, default_config)
                         if inst:
                             self.load_backends(names=[inst])
                 except (KeyboardInterrupt, EOFError):
                     print('\nAborted.')
                 else:
                     break
+                continue
 
-        print('Right right!')
+            if r.isdigit():
+                i = int(r) - 1
+                if i < 0 or i >= len(modules):
+                    print(f'Error: {r} is not a valid choice', file=self.stderr)
+                    continue
+                name = modules[i]
+            elif r in modules:
+                name = r
+            else:
+                print(f'Error: {r} is not a valid choice', file=self.stderr)
+                continue
+
+            try:
+                inst = self.add_backend(name, name, default_config)
+                if inst:
+                    self.load_backends(names=[inst])
+            except (KeyboardInterrupt, EOFError):
+                print('\nAborted.')
 
     def _handle_options(self):
         self.load_default_backends()
 
     def load_default_backends(self):
         """
         By default loads all backends.
@@ -216,19 +287,19 @@
         """
         if len(self.STORAGE) > 0:
             self.load_backends(self.CAPS, storage=self.create_storage())
         else:
             self.load_backends(self.CAPS)
 
     @classmethod
-    def run(klass, args=None):
+    def run(cls, args=None):
         try:
             super().run(args)
         except BackendNotFound as e:
-            print('Error: Backend "%s" not found.' % e)
+            print(f'Error: Backend "{e}" not found.')
             sys.exit(1)
 
     def do(self, function, *args, **kwargs):
         if 'backends' not in kwargs:
             kwargs['backends'] = self.enabled_backends
         return self.woob.do(function, *args, **kwargs)
 
@@ -316,15 +387,14 @@
     def install_module(self, minfo):
         try:
             self.woob.repositories.install(minfo, ConsoleProgress(self))
         except ModuleInstallError as e:
             print('Unable to install module "%s": %s' % (minfo.name, e), file=self.stderr)
             return False
 
-        print('')
         return True
 
     def edit_backend(self, name, params=None):
         return self.add_backend(name, name, params, True)
 
     def add_backend(self, module_name, backend_name, params=None, edit=False, ask_register=True):
         if params is None:
```

### Comparing `woob-3.5/woob/tools/application/formatters/csv.py` & `woob-3.6/woob/tools/application/formatters/csv.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/application/formatters/iformatter.py` & `woob-3.6/woob/tools/application/formatters/iformatter.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,30 +12,19 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with woob. If not, see <http://www.gnu.org/licenses/>.
 
 
-from codecs import open
 from collections import OrderedDict
 import os
 import sys
 import subprocess
-
-try:
-    from termcolor import colored
-except ImportError:
-    def colored(s, color=None, on_color=None, attrs=None):
-        if os.getenv('ANSI_COLORS_DISABLED') is None \
-                and os.getenv('NO_COLOR') is None \
-                and attrs is not None and 'bold' in attrs:
-            return '%s%s%s' % (IFormatter.BOLD, s, IFormatter.NC)
-        else:
-            return s
+import warnings
 
 try:
     import tty
     import termios
 except ImportError:
     PROMPT = '--Press return to continue--'
 
@@ -55,34 +44,52 @@
             if c == '\x03':
                 raise KeyboardInterrupt()
             return c
         finally:
             termios.tcsetattr(fd, termios.TCSADRAIN, old_settings)
 
 from woob.capabilities.base import BaseObject
-from woob.tools.application.console import ConsoleApplication
-from woob.tools.misc import guess_encoding
+from woob.tools.application.pretty import colored, NC, BOLD
+from woob.tools.misc import guess_encoding, classproperty
+
 
 __all__ = ['IFormatter', 'MandatoryFieldsNotFound']
 
 
 class MandatoryFieldsNotFound(Exception):
     def __init__(self, missing_fields):
-        super(MandatoryFieldsNotFound, self).__init__('Mandatory fields not found: %s.' % ', '.join(missing_fields))
+        super().__init__('Mandatory fields not found: %s.' % ', '.join(missing_fields))
 
 
 class IFormatter:
     # Tuple of fields mandatory to not crash
     MANDATORY_FIELDS = None
     # Tuple of displayed field. Set to None if all available fields are
     # displayed
     DISPLAYED_FIELDS = None
 
-    BOLD = ConsoleApplication.BOLD
-    NC = ConsoleApplication.NC
+    @classproperty
+    def BOLD(self):
+        warnings.warn(
+            'Use woob.tools.application.pretty.BOLD instead.\n'
+            'That\'s also better to use woob.tools.application.pretty.colored.',
+            DeprecationWarning,
+            stacklevel=2
+        )
+        return BOLD
+
+    @classproperty
+    def NC(self):
+        warnings.warn(
+            'Use woob.tools.application.pretty.NC instead.\n'
+            'That\'s also better to use woob.tools.application.pretty.colored.',
+            DeprecationWarning,
+            stacklevel=2
+        )
+        return NC
 
     def colored(self, string, color, attrs=None, on_color=None):
         if (
             self.outfile != sys.stdout
             or not self.outfile.isatty()
             or os.getenv("NO_COLOR") is not None
         ):
```

### Comparing `woob-3.5/woob/tools/application/formatters/json.py` & `woob-3.6/woob/tools/application/formatters/json.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/application/formatters/load.py` & `woob-3.6/woob/tools/application/formatters/load.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/application/formatters/multiline.py` & `woob-3.6/woob/tools/application/formatters/multiline.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/application/formatters/simple.py` & `woob-3.6/woob/tools/application/formatters/simple.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/application/formatters/table.py` & `woob-3.6/woob/tools/application/formatters/table.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/application/media_player.py` & `woob-3.6/woob/tools/application/media_player.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/application/repl.py` & `woob-3.6/woob/tools/application/repl.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 from woob.exceptions import BrowserQuestion, BrowserRedirect, DecoupledValidation
 from woob.tools.application.formatters.iformatter import MandatoryFieldsNotFound
 from woob.tools.path import WorkingPath
 
 from .console import BackendNotGiven, ConsoleApplication
 from .formatters.load import FormatterLoadError, FormattersLoader
 from .results import ResultsCondition, ResultsConditionError
+from .pretty import colored
+
 
 __all__ = [
     'NotEnoughArguments', 'TooManyArguments', 'ArgSyntaxError',
     'ReplApplication'
 ]
 
 
@@ -120,15 +122,15 @@
     woob_commands = {'backends', 'condition', 'count', 'formatter', 'logging', 'select', 'quit', 'ls', 'cd', 'storage'}
     hidden_commands = {'EOF'}
 
     def __init__(self):
         super().__init__(ReplOptionParser(self.SYNOPSIS, version=self._get_optparse_version()))
 
         copyright = self.COPYRIGHT.replace('YEAR', '%d' % datetime.today().year)
-        self.intro = '\n'.join(('Welcome to %s%s%s v%s' % (self.BOLD, self.APPNAME, self.NC, self.VERSION),
+        self.intro = '\n'.join(('Welcome to %s v%s' % (colored(self.APPNAME, attrs=['bold']), self.VERSION),
                                 '',
                                 copyright,
                                 'This program is free software: you can redistribute it and/or modify',
                                 'it under the terms of the GNU Lesser General Public License as published by',
                                 'the Free Software Foundation, either version 3 of the License, or',
                                 '(at your option) any later version.',
                                 '',
@@ -210,16 +212,23 @@
         try:
             return super().parse_id(id, unique_backend)
         except BackendNotGiven as e:
             backend_name = None
             while not backend_name:
                 print('This command works with an unique backend. Availables:')
                 for index, (name, backend) in enumerate(e.backends):
-                    print('%s%d)%s %s%-15s%s   %s' % (self.BOLD, index + 1, self.NC, self.BOLD, name, self.NC,
-                          backend.DESCRIPTION))
+                    print(
+                        '%s) %s%s' % (
+                            colored('%2d' % (index + 1), 'white', attrs=['bold']),
+                            colored('%-20s' % name, 'magenta', attrs=['bold']),
+                            colored(backend.DESCRIPTION, 'green')
+                        )
+                    )
+
+
                 i = self.ask('Select a backend to proceed with "%s"' % id)
                 if not i.isdigit():
                     if i not in dict(e.backends):
                         print('Error: %s is not a valid backend' % i, file=self.stderr)
                         continue
                     backend_name = i
                 else:
@@ -905,15 +914,21 @@
                     if bi.NAME == name:
                         if loaded == ' ':
                             loaded = 'X'
                         elif loaded == 'X':
                             loaded = 2
                         else:
                             loaded += 1
-                print('[%s] %s%-15s%s   %s' % (loaded, self.BOLD, name, self.NC, info.description))
+                print(
+                    '[%s] %s%s' % (
+                        colored(str(loaded), attrs=['bold']),
+                        colored('%-20s' % name, 'magenta', attrs=['bold']),
+                        colored(info.description, 'green')
+                    )
+                )
 
         else:
             print('Unknown action: "%s"' % action, file=self.stderr)
             return 1
 
         if len(self.enabled_backends) == 0:
             print('Warning: no more backends are loaded. %s is probably unusable.' % self.APPNAME.capitalize(), file=self.stderr)
```

### Comparing `woob-3.5/woob/tools/application/results.py` & `woob-3.6/woob/tools/application/results.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/backend.py` & `woob-3.6/woob/tools/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 from woob import __version__
 from woob.capabilities.base import BaseObject, Capability, FieldNotFound, NotAvailable, NotLoaded
 from woob.tools.json import json
 from woob.tools.log import getLogger
 from woob.tools.misc import iter_fields
 from woob.tools.storage import IStorage
-from woob.tools.value import ValuesDict
+from woob.tools.value import ValuesDict, ValueBool
 
 if TYPE_CHECKING:
     from woob.core import WoobBase
     from woob.browser import Browser
 
 
 __all__ = ['BackendStorage', 'BackendConfig', 'Module']
@@ -443,23 +443,42 @@
 
         kwargs['proxy'] = self.get_proxy()
         if '_proxy_headers' in self._private_config:
             kwargs['proxy_headers'] = self._private_config['_proxy_headers']
             if isinstance(kwargs['proxy_headers'], str):
                 kwargs['proxy_headers'] = json.loads(kwargs['proxy_headers'])
 
+        if '_ssl_verify' in self._private_config:
+            # value can be either a boolean or a string (path)
+            value = ValueBool()
+            try:
+                value.set(self._private_config['_ssl_verify'])
+            except ValueError:
+                kwargs.setdefault('verify', self._private_config['_ssl_verify'])
+            else:
+                kwargs.setdefault('verify', value.get())
+
         kwargs['logger'] = self.logger
 
         if self.logger.settings['responses_dirname']:
             kwargs.setdefault('responses_dirname', os.path.join(self.logger.settings['responses_dirname'],
                                                                 self._private_config.get('_debug_dir', self.name)))
         elif os.path.isabs(self._private_config.get('_debug_dir', '')):
             kwargs.setdefault('responses_dirname', self._private_config['_debug_dir'])
-        if self._private_config.get('_highlight_el', ''):
-            kwargs.setdefault('highlight_el', bool(int(self._private_config['_highlight_el'])))
+
+        if '_highlight_el' in self._private_config:
+            value = ValueBool()
+            try:
+                value.set(self._private_config['_highlight_el'])
+            except ValueError as e:
+                raise Module.ConfigError(
+                    f'Backend({self.name}): Configuration error: _highlight_el must be a boolean'
+                ) from e
+
+            kwargs.setdefault('highlight_el', value.get())
 
         browser = klass(*args, **kwargs)
 
         if hasattr(browser, 'load_state'):
             browser.load_state(self.storage.get('browser_state', default={}))
 
         return browser
```

### Comparing `woob-3.5/woob/tools/capabilities/audio/audio.py` & `woob-3.6/woob/tools/capabilities/audio/audio.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/capabilities/bank/bank_transfer.py` & `woob-3.6/woob/tools/capabilities/bank/bank_transfer.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/capabilities/bank/data_matching.py` & `woob-3.6/woob/tools/capabilities/bank/data_matching.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/capabilities/bank/iban.py` & `woob-3.6/woob/tools/capabilities/bank/iban.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/capabilities/bank/investments.py` & `woob-3.6/woob/tools/capabilities/bank/investments.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,19 +11,21 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with woob. If not, see <http://www.gnu.org/licenses/>.
 
+from decimal import Decimal
 import re
 
 from woob.capabilities.base import NotAvailable
 from woob.capabilities.bank.wealth import Investment
 from woob.browser.filters.base import Filter, FilterError, debug
+from woob.tools.log import getLogger
 
 def is_isin_valid(isin):
     """
     Méthode générale
     Table de conversion des lettres en chiffres
     A=10    B=11    C=12    D=13    E=14    F=15    G=16    H=17    I=18
     J=19    K=20    L=21    M=22    N=23    O=24    P=25    Q=26    R=27
@@ -69,14 +71,16 @@
     return str(sum(int(x) for x in result) + int(key))[-1] == '0'
 
 
 def create_french_liquidity(valuation):
     """
     Automatically fills a liquidity investment with label, code and code_type.
     """
+    if isinstance(valuation, Decimal) and valuation < 0:
+        getLogger('%s.create_French_liquidity' % __name__).warning("Liquidity has a negative value")
     liquidity = Investment()
     liquidity.label = "Liquidités"
     liquidity.code = "XX-liquidity"
     liquidity.code_type = NotAvailable
     liquidity.valuation = valuation
     return liquidity
```

### Comparing `woob-3.5/woob/tools/capabilities/bank/sortcode.py` & `woob-3.6/woob/tools/capabilities/bank/sortcode.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/capabilities/bank/test.py` & `woob-3.6/woob/tools/capabilities/bank/test.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/capabilities/bank/transactions.py` & `woob-3.6/woob/tools/capabilities/bank/transactions.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/capabilities/bill/documents.py` & `woob-3.6/woob/tools/capabilities/bill/documents.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/capabilities/housing/housing.py` & `woob-3.6/woob/tools/capabilities/housing/housing.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/capabilities/housing/housing_test.py` & `woob-3.6/woob/tools/capabilities/housing/housing_test.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/capabilities/messages/threading.py` & `woob-3.6/woob/tools/capabilities/messages/threading.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/capabilities/paste.py` & `woob-3.6/woob/tools/capabilities/paste.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/capabilities/recipe.py` & `woob-3.6/woob/tools/capabilities/recipe.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/capabilities/streaminfo.py` & `woob-3.6/woob/tools/capabilities/streaminfo.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/capabilities/video/ytdl.py` & `woob-3.6/woob/tools/capabilities/video/ytdl.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/captcha/virtkeyboard.py` & `woob-3.6/woob/tools/captcha/virtkeyboard.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,41 +11,50 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with woob. If not, see <http://www.gnu.org/licenses/>.
 
+from __future__ import annotations
+
 import hashlib
 import tempfile
+from typing import IO, ClassVar, TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from woob.browser import Browser
+
 
 try:
     from PIL import Image
 except ImportError:
     raise ImportError('Please install python-imaging')
 
 
 class VirtKeyboardError(Exception):
     pass
 
 
 class VirtKeyboard:
     """
     Handle a virtual keyboard.
-
-    :attribute margin: Margin used by :meth:`get_symbol_coords` to reduce size
-        of each "key" of the virtual keyboard. This attribute is always
-        converted to a 4-tuple, and has the same semantic as the CSS
-        ``margin`` property (top, right, bottom, right), in pixels.
-    :type margin: int or float or (2|3|4)-tuple
     """
+
     margin = None
+    """
+    Margin used by :meth:`get_symbol_coords` to reduce size
+    of each "key" of the virtual keyboard. This attribute is always
+    converted to a 4-tuple, and has the same semantic as the CSS
+    ``margin`` property (top, right, bottom, right), in pixels.
+    """
 
     codesep = ''
-    """Output separator between code strings.
+    """
+    Output separator between code strings.
 
     See :func:`get_string_code`.
     """
 
     def __init__(self, file=None, coords=None, color=None, convert=None):
         # file: virtual keyboard image
         # coords: dictionary <value to return>:<tuple(x1,y1,x2,y2)>
@@ -205,34 +214,30 @@
 
 
 class GridVirtKeyboard(VirtKeyboard):
     """
     Make a virtual keyboard where "keys" are distributed on a grid.
     Example here: https://www.e-sgbl.com/portalserver/sgbl-web/login
 
-    Parameters:
-        :param symbols: Sequence of symbols, ordered in the grid from left to
-            right and up to down
-        :type symbols: iterable
-        :param cols: Column count of the grid
-        :type cols: int
-        :param rows: Row count of the grid
-        :type rows: int
-        :param image: File-like object to be used as data source
-        :type image: file
-        :param color: Color of the meaningful pixels
-        :type color: 3-tuple
-        :param convert: Mode to which convert color of pixels, see
-            :meth:`Image.Image.convert` for more information
-
-    Attributes:
-        :attribute symbols: Association table between symbols and md5s
-        :type symbols: dict
+    :param symbols: Sequence of symbols, ordered in the grid from left to
+        right and up to down
+    :type symbols: iterable
+    :param cols: Column count of the grid
+    :type cols: int
+    :param rows: Row count of the grid
+    :type rows: int
+    :param image: File-like object to be used as data source
+    :type image: file
+    :param color: Color of the meaningful pixels
+    :type color: 3-tuple
+    :param convert: Mode to which convert color of pixels, see
+        :meth:`Image.Image.convert` for more information
     """
     symbols = {}
+    """Assocation table between symbols and md5s"""
 
     def __init__(self, symbols, cols, rows, image, color, convert=None):
         self.load_image(image, color, convert)
 
         tileW = self.width / cols
         tileH = self.height / rows
         positions = ((s, i * tileW % self.width, i // cols * tileH)
@@ -245,19 +250,17 @@
         self.load_symbols(coords)
 
 
 class SplitKeyboard:
     """Virtual keyboard for when the chars are in individual images, not a single grid"""
 
     char_to_hash = None
-
     """dict mapping password characters to image hashes"""
 
     codesep = ''
-
     """Output separator between symbols"""
 
     def __init__(self, code_to_filedata):
         """Create a SplitKeyboard
 
         :param code_to_filedata: dict mapping site codes to images data
         :type code_to_filedata: dict[str, str]
@@ -315,60 +318,67 @@
         self.image = image
         self.md5 = md5
 
 
 class SimpleVirtualKeyboard:
     """Handle a virtual keyboard where "keys" are distributed on a simple grid.
 
-    Parameters:
-        :param cols: Column count of the grid
-        :type cols: int
-        :param rows: Row count of the grid
-        :type rows: int
-        :param image: File-like object to be used as data source
-        :type image: file
-        :param convert: Mode to which convert color of pixels, see
-            :meth:`Image.Image.convert` for more information
-        :param matching_symbols: symbol that match all case of image grid from left to right and top
-                                 to down, European reading way.
-        :type matching_symbols: iterable
-        :param matching_symbols_coords: dict mapping matching website symbols to their image coords
-                                        (x0, y0, x1, y1) on grid image from left to right and top to
-                                        down, European reading way. It's not symbols in the image.
-        :type matching_symbols_coords: dict[str:4-tuple(int)]
-        :param browser: Browser of woob session.
-                        Allow to dump tiles files in same directory than session folder
-        :type browser: obj(Browser)
-
-    Attributes:
-        :attribute codesep: Output separator between matching symbols
-        :type codesep: str
-        :param margin: Useless image pixel to cut.
-                       See :func:`cut_margin`.
-        :type margin: 4-tuple(int), same as HTML margin: (top, right, bottom, left).
-                      or 2-tuple(int), (top = bottom, right = left),
-                      or int, top = right = bottom = left
-        :attribute tile_margin: Useless tile pixel to cut.
-                                See :func:`cut_margin`.
-        :attribute symbols: Association table between image symbols and md5s
-        :type symbols: dict[str:str] or dict[str:n-tuple(str)]
-        :attribute convert: Mode to which convert color of pixels, see
-            :meth:`Image.Image.convert` for more information
-        :attribute alter: Allow custom main image alteration. Then overwrite :func:`alter_image`.
-        :type alter: boolean
+    :param cols: Column count of the grid
+    :param rows: Row count of the grid
+    :param file: File-like object to be used as data source
+    :param convert: Mode to which convert color of pixels, see
+        :meth:`Image.Image.convert` for more information
+    :param matching_symbols: symbol that match all case of image grid from left to right and top
+        to down, European reading way.
+    :param matching_symbols_coords: dict mapping matching website symbols to their image coords
+        (x0, y0, x1, y1) on grid image from left to right and top to
+        down, European reading way. It's not symbols in the image.
+    :param browser: Browser of woob session.
+        Allow to dump tiles files in same directory than session folder
+    """
+
+    codesep: ClassVar[str] = ''
+    """Output separator between matching symbols"""
+
+    margin: ClassVar[tuple[int, int, int, int] | tuple[int, int] | int | None] = None
+    """
+    4-tuple(int), same as HTML margin: (top, right, bottom, left).
+    or 2-tuple(int), (top = bottom, right = left),
+    or int, top = right = bottom = left
+    """
+
+    tile_margin: ClassVar[tuple[int, int, int, int] | tuple[int, int] | int | None] = None
+    """
+    4-tuple(int), same as HTML margin: (top, right, bottom, left).
+    or 2-tuple(int), (top = bottom, right = left),
+    or int, top = right = bottom = left
+    """
+
+    symbols: ClassVar[dict[str, str | tuple[str, ...]]] = None
+    """
+    Association table between image symbols and md5s
+    """
+
+    convert: ClassVar[str | None] = None
+    """
+    Mode to which convert color of pixels, see
+    :meth:`Image.Image.convert` for more information
     """
 
-    codesep = ''
-    margin = None
-    tile_margin = None
-    symbols = None
-    convert = None
     tile_klass = Tile
 
-    def __init__(self, file, cols, rows, matching_symbols=None, matching_symbols_coords=None, browser=None):
+    def __init__(
+        self,
+        file: IO,
+        cols: int,
+        rows: int,
+        matching_symbols: list[str] | None = None,
+        matching_symbols_coords: dict[str, tuple[int, int, int, int]] | None = None,
+        browser: Browser | None = None
+    ):
         self.cols = cols
         self.rows = rows
 
         # Needed even if init is overwrite
         self.path = self.build_path(browser)
 
         # Get self.image
```

### Comparing `woob-3.5/woob/tools/config/dbmconfig.py` & `woob-3.6/woob/tools/config/dbmconfig.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/config/extra.py` & `woob-3.6/woob/tools/config/extra.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/config/iconfig.py` & `woob-3.6/woob/tools/config/iconfig.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/config/iniconfig.py` & `woob-3.6/woob/tools/config/iniconfig.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/config/sqliteconfig.py` & `woob-3.6/woob/tools/config/sqliteconfig.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/config/util.py` & `woob-3.6/woob/tools/config/util.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/config/yamlconfig.py` & `woob-3.6/woob/tools/config/yamlconfig.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/date.py` & `woob-3.6/woob/tools/date.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/decorators.py` & `woob-3.6/woob/tools/decorators.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,37 +14,34 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with woob. If not, see <http://www.gnu.org/licenses/>.
 
 import logging
 import time
 
+
 __all__ = ['retry']
 
 
 def retry(exceptions_to_check, exc_handler=None, tries=3, delay=2, backoff=2):
     """
     Retry decorator
-    from http://www.saltycrane.com/blog/2009/11/trying-out-retry-decorator-python/
-    original from http://wiki.python.org/moin/PythonDecoratorLibrary#Retry
+    from https://www.saltycrane.com/blog/2009/11/trying-out-retry-decorator-python/
+    original from https://wiki.python.org/moin/PythonDecoratorLibrary#Retry
     """
     def deco_retry(f):
         def f_retry(*args, **kwargs):
             mtries = kwargs.pop('_tries', tries)
             mdelay = kwargs.pop('_delay', delay)
             while mtries > 1:
                 try:
                     return f(*args, **kwargs)
                 except exceptions_to_check as exc:
                     if exc_handler:
                         exc_handler(exc, **kwargs)
-                    try:
-                        logging.debug('%s, Retrying in %d seconds...' % (exc, mdelay))
-                    except UnicodeDecodeError:
-                        logging.debug('%s, Retrying in %d seconds...' % (repr(exc), mdelay))
+                    logging.debug('%s, Retrying in %d seconds...', exc, mdelay)
                     time.sleep(mdelay)
                     mtries -= 1
                     mdelay *= backoff
             return f(*args, **kwargs)
         return f_retry  # true decorator
     return deco_retry
-
```

### Comparing `woob-3.5/woob/tools/js.py` & `woob-3.6/woob/tools/js.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/json.py` & `woob-3.6/woob/tools/json.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 
 def mini_jsonpath(node, path):
     """
     Evaluates a dot separated path against JSON data. Path can contains
     star wilcards. Always returns a generator.
 
-    Relates to http://goessner.net/articles/JsonPath/ but in a really basic
+    Relates to https://goessner.net/articles/JsonPath/ but in a really basic
     and simpler form.
 
     >>> list(mini_jsonpath({"x": 95, "y": 77, "z": 68}, 'y'))
     [77]
     >>> list(mini_jsonpath({"x": {"y": {"z": "nested"}}}, 'x.y.z'))
     ['nested']
     >>> list(mini_jsonpath('{"data": [{"x": "foo", "y": 13}, {"x": "bar", "y": 42}, {"x": "baz", "y": 128}]}', 'data.*.y'))
```

### Comparing `woob-3.5/woob/tools/log.py` & `woob-3.6/woob/tools/log.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         logger.settings = settings
     return logger
 
 
 class ColoredFormatter(Formatter):
     """
     Class written by airmind:
-    http://stackoverflow.com/questions/384076/how-can-i-make-the-python-logging-output-to-be-colored
+    https://stackoverflow.com/questions/384076/how-can-i-make-the-python-logging-output-to-be-colored
     """
 
     def format(self, record):
         levelname = record.levelname
 
         msg = super().format(record)
         if levelname in COLORS:
```

### Comparing `woob-3.5/woob/tools/lrudict.py` & `woob-3.6/woob/tools/lrudict.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/misc.py` & `woob-3.6/woob/tools/misc.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/newsfeed.py` & `woob-3.6/woob/tools/newsfeed.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/packaging.py` & `woob-3.6/woob/tools/packaging.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/path.py` & `woob-3.6/woob/tools/path.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/pdf.py` & `woob-3.6/woob/tools/pdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 def decompress_pdf(inpdf: bytes) -> bytes:
     """
     Takes PDF file contents as a string and returns decompressed version
     of the file contents, suitable for text parsing.
 
     External dependencies:
-    MuPDF (http://www.mupdf.com).
+    MuPDF (https://www.mupdf.com).
     """
 
     inh, inname = mkstemp(suffix='.pdf')
     outh, outname = mkstemp(suffix='.pdf')
     os.write(inh, inpdf)
     os.close(inh)
     os.close(outh)
@@ -292,15 +292,15 @@
     Note that the rows may belong to different tables.
 
     There are no logic tables in PDF format, so this parses PDF drawing instructions
     and tries to find rectangles and arrange them in rows, then arrange text in
     the rectangles.
 
     External dependencies:
-    PDFMiner (http://www.unixuser.org/~euske/python/pdfminer/index.html).
+    PDFMiner (https://github.com/euske/pdfminer).
     """
 
     try:
         from pdfminer.pdfparser import PDFParser, PDFSyntaxError
     except ImportError:
         raise ImportError('Please install python3-pdfminer')
```

### Comparing `woob-3.5/woob/tools/regex_helper.py` & `woob-3.6/woob/tools/regex_helper.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/storage.py` & `woob-3.6/woob/tools/storage.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/test.py` & `woob-3.6/woob/tools/test.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/tokenizer.py` & `woob-3.6/woob/tools/tokenizer.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/url.py` & `woob-3.6/woob/tools/url.py`

 * *Files identical despite different names*

### Comparing `woob-3.5/woob/tools/value.py` & `woob-3.6/woob/tools/value.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,37 +11,76 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with woob. If not, see <http://www.gnu.org/licenses/>.
 
+from __future__ import annotations
 
 import re
 import datetime
 from collections import OrderedDict
+from typing import TypeVar
 
 from .misc import to_unicode
 
 
 __all__ = ['ValuesDict', 'Value', 'ValueBackendPassword', 'ValueInt', 'ValueFloat', 'ValueBool']
 
+ValuesDictType = TypeVar('ValuesDictType', bound='ValuesDict')
+
 
 class ValuesDict(OrderedDict):
-    """
-    Ordered dictionarry which can take values in constructor.
+    """Ordered dictionary which can take values in constructor.
 
     >>> ValuesDict(Value('a', label='Test'), ValueInt('b', label='Test2'))
     """
 
     def __init__(self, *values):
         super(ValuesDict, self).__init__()
         for v in values:
             self[v.id] = v
 
+    def with_values(self: ValuesDictType, *values: Value) -> ValuesDictType:
+        """Get a copy of the object, with new values.
+
+        :param values: The values to set.
+        :return: The new values dictionary.
+        """
+        existing_values = {key: value for key, value in self.items()}
+        existing_values.update({value.id: value for value in values})
+        return self.__class__(*existing_values.values())
+
+    def with_values_from(self: ValuesDictType, other: ValuesDict) -> ValuesDictType:
+        """Get a copy of the object, with overrides from another values dictionary.
+
+        Values from the other dictionary will override values from the
+        current dictionary.
+
+        :param other: the other dictionary to take values from.
+        :return: The new values dictionary.
+        """
+        return self.with_values(*other.values())
+
+    def without_values(self: ValuesDictType, *value_names: str) -> ValuesDictType:
+        """Get a copy of the object, without values with the given names.
+
+        This method will ignore value names that aren't present in the
+        original dictionary.
+
+        :param value_names: The name of the values to remove.
+        :return: The new values dictionary.
+        """
+        existing_values = {key: value for key, value in self.items()}
+        for value_name in value_names:
+            existing_values.pop(value_name, None)
+
+        return self.__class__(*existing_values.values())
+
 
 class Value:
     """
     Value.
 
     :param label: human readable description of a value
     :type label: str
@@ -111,19 +150,22 @@
         if self.required and v is None:
             raise ValueError('Value is required and thus must be set')
         if v == self.default:
             return
         if v == '' and self.default != '' and (self.choices is None or v not in self.choices):
             raise ValueError('Value can\'t be empty')
         if self.regexp is not None and not re.match(self.regexp, str(v) if v is not None else ''):
-            raise ValueError('Value "%s" does not match regexp "%s"' % (self.show_value(v), self.regexp))
+            raise ValueError('Value does not match regexp "%s"' % self.regexp)
         if self.choices is not None and v not in self.choices:
             if not self.aliases or v not in self.aliases:
-                raise ValueError('Value "%s" is not in list: %s' % (
-                    self.show_value(v), ', '.join(str(s) for s in self.choices)))
+                raise ValueError(
+                    'Value is not in list: %s' % (
+                        ', '.join(str(s) for s in self.choices)
+                    )
+                )
 
     def load(self, domain, v, requests):
         """
         Load value.
 
         :param domain: what is the domain of this value
         :type domain: str
@@ -246,15 +288,15 @@
         super(ValueFloat, self).__init__(*args, **kwargs)
         self.default = kwargs.get('default', 0.0)
 
     def check_valid(self, v):
         try:
             float(v)
         except ValueError:
-            raise ValueError('Value "%s" is not a float value' % self.show_value(v))
+            raise ValueError('Value is not a float value')
 
     def get(self):
         return float(self._value)
 
 
 class ValueBool(Value):
     def __init__(self, *args, **kwargs):
@@ -265,15 +307,15 @@
     def check_valid(self, v):
         if not isinstance(v, bool) and \
             str(v).lower() not in {
                 'y', 'yes', '1', 'true',  'on',
                 'n', 'no',  '0', 'false', 'off',
             }:
 
-            raise ValueError('Value "%s" is not a boolean (y/n)' % self.show_value(v))
+            raise ValueError('Value is not a boolean (y/n)')
 
     def get(self):
         return (isinstance(self._value, bool) and self._value) or \
                 str(self._value).lower() in {'y', 'yes', '1', 'true', 'on'}
 
 
 class ValueDate(Value):
@@ -293,15 +335,15 @@
         for format in self.accepted_formats:
             try:
                 dateval = datetime.datetime.strptime(v, format).date()
             except ValueError:
                 continue
             return dateval
 
-        raise ValueError('Value "%s" does not match format in %s' % (self.show_value(v), self.accepted_formats))
+        raise ValueError('Value does not match format in %s' % self.accepted_formats)
 
     def check_valid(self, v):
         if self.required and not v:
             raise ValueError('Value is required and thus must be set')
 
     def load(self, domain, v, requests):
         self.check_valid(v)
@@ -309,15 +351,15 @@
             self._value = None
             return
         if isinstance(v, str):
             v = self._parse(v)
         if isinstance(v, datetime.date):
             self._value = v
         else:
-            raise ValueError('Value %r is not of the proper type' % self.show_value(v))
+            raise ValueError('Value is not of the proper type')
 
     def dump(self):
         if self._value:
             return self._value.strftime(self.DEFAULT_FORMAT)
 
     def set(self, v):
         self.load(None, v, None)
```

### Comparing `woob-3.5/woob.egg-info/PKG-INFO` & `woob-3.6/woob.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: woob
-Version: 3.5
+Version: 3.6
 Summary: Woob, Web Outside Of Browsers
 Author-email: Romain Bignon <romain@woob.dev>
 License: LGPL-3.0-or-later
 Project-URL: Homepage, https://woob.tech
+Project-URL: Source, https://gitlab.com/woob/woob
 Project-URL: Release notes, https://gitlab.com/woob/woob/-/releases
 Project-URL: Documentation, https://woob.dev
 Project-URL: Bug Tracker, https://gitlab.com/woob/woob/-/issues
 Keywords: scraping,web,banking
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python
```

### Comparing `woob-3.5/woob.egg-info/SOURCES.txt` & `woob-3.6/woob.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 AUTHORS
 COPYING
 COPYING.LESSER
 README.rst
 pyproject.toml
 weboob/__init__.py
 woob/__init__.py
+woob/__main__.py
 woob/exceptions.py
+woob/launcher.py
 woob.egg-info/PKG-INFO
 woob.egg-info/SOURCES.txt
 woob.egg-info/dependency_links.txt
 woob.egg-info/entry_points.txt
 woob.egg-info/requires.txt
 woob.egg-info/top_level.txt
 woob/applications/__init__.py
@@ -46,15 +48,14 @@
 woob/applications/housing/__init__.py
 woob/applications/housing/housing.py
 woob/applications/job/__init__.py
 woob/applications/job/job.py
 woob/applications/lyrics/__init__.py
 woob/applications/lyrics/lyrics.py
 woob/applications/main/__init__.py
-woob/applications/main/main.py
 woob/applications/money/__init__.py
 woob/applications/money/money.py
 woob/applications/msg/__init__.py
 woob/applications/msg/msg.py
 woob/applications/parcel/__init__.py
 woob/applications/parcel/parcel.py
 woob/applications/paste/__init__.py
@@ -190,14 +191,15 @@
 woob/tools/value.py
 woob/tools/application/__init__.py
 woob/tools/application/base.py
 woob/tools/application/captcha.py
 woob/tools/application/console.py
 woob/tools/application/javascript.py
 woob/tools/application/media_player.py
+woob/tools/application/pretty.py
 woob/tools/application/repl.py
 woob/tools/application/results.py
 woob/tools/application/formatters/__init__.py
 woob/tools/application/formatters/csv.py
 woob/tools/application/formatters/iformatter.py
 woob/tools/application/formatters/json.py
 woob/tools/application/formatters/load.py
```

