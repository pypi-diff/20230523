# Comparing `tmp/ghananews-scraper-1.0.8.tar.gz` & `tmp/ghananews-scraper-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ghananews-scraper-1.0.8.tar", last modified: Wed May  3 05:14:24 2023, max compression
+gzip compressed data, was "dist/ghananews-scraper-1.0.9.tar", last modified: Sat May 20 07:37:20 2023, max compression
```

## Comparing `ghananews-scraper-1.0.8.tar` & `ghananews-scraper-1.0.9.tar`

### file list

```diff
@@ -1,40 +1,45 @@
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 05:14:24.000000 ghananews-scraper-1.0.8/
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 05:14:24.000000 ghananews-scraper-1.0.8/3news/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-04-30 16:57:53.000000 ghananews-scraper-1.0.8/3news/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     2931 2023-04-30 16:59:02.000000 ghananews-scraper-1.0.8/3news/scraper.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghananews-scraper-1.0.8/3news/utils.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     9442 2023-05-03 05:14:24.000000 ghananews-scraper-1.0.8/PKG-INFO
--rw-r--r--   0 tsiameh    (501) staff       (20)     6642 2023-05-02 14:27:06.000000 ghananews-scraper-1.0.8/README.md
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 05:14:24.000000 ghananews-scraper-1.0.8/citionline/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-04-29 20:41:04.000000 ghananews-scraper-1.0.8/citionline/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     3478 2023-05-03 05:13:03.000000 ghananews-scraper-1.0.8/citionline/scraper.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghananews-scraper-1.0.8/citionline/utils.py
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 05:14:24.000000 ghananews-scraper-1.0.8/ghananews_scraper.egg-info/
--rw-r--r--   0 tsiameh    (501) staff       (20)     9442 2023-05-03 05:14:24.000000 ghananews-scraper-1.0.8/ghananews_scraper.egg-info/PKG-INFO
--rw-r--r--   0 tsiameh    (501) staff       (20)      667 2023-05-03 05:14:24.000000 ghananews-scraper-1.0.8/ghananews_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)        1 2023-05-03 05:14:24.000000 ghananews-scraper-1.0.8/ghananews_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)       13 2023-05-03 05:14:24.000000 ghananews-scraper-1.0.8/ghananews_scraper.egg-info/requires.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)       68 2023-05-03 05:14:24.000000 ghananews-scraper-1.0.8/ghananews_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 05:14:24.000000 ghananews-scraper-1.0.8/ghanaweb/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-03-13 15:04:12.000000 ghananews-scraper-1.0.8/ghanaweb/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     4317 2023-05-03 05:13:03.000000 ghananews-scraper-1.0.8/ghanaweb/scraper.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-16 02:31:26.000000 ghananews-scraper-1.0.8/ghanaweb/utils.py
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 05:14:24.000000 ghananews-scraper-1.0.8/graphiconline/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-04-30 14:50:37.000000 ghananews-scraper-1.0.8/graphiconline/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     3716 2023-05-03 05:13:03.000000 ghananews-scraper-1.0.8/graphiconline/scraper.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghananews-scraper-1.0.8/graphiconline/utils.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     1457 2023-04-30 16:53:26.000000 ghananews-scraper-1.0.8/graphiconline.py
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 05:14:24.000000 ghananews-scraper-1.0.8/modernghana/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-01 18:28:50.000000 ghananews-scraper-1.0.8/modernghana/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     3273 2023-05-01 18:29:39.000000 ghananews-scraper-1.0.8/modernghana/scraper.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghananews-scraper-1.0.8/modernghana/utils.py
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 05:14:24.000000 ghananews-scraper-1.0.8/myjoyonline/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-03-15 14:35:44.000000 ghananews-scraper-1.0.8/myjoyonline/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     6425 2023-05-03 05:13:03.000000 ghananews-scraper-1.0.8/myjoyonline/scraper.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      789 2023-05-03 05:13:03.000000 ghananews-scraper-1.0.8/myjoyonline/utils.py
--rw-r--r--   0 tsiameh    (501) staff       (20)       38 2023-05-03 05:14:24.000000 ghananews-scraper-1.0.8/setup.cfg
--rw-r--r--   0 tsiameh    (501) staff       (20)     1805 2023-05-03 05:14:21.000000 ghananews-scraper-1.0.8/setup.py
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 05:14:24.000000 ghananews-scraper-1.0.8/yen/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-04-30 18:14:26.000000 ghananews-scraper-1.0.8/yen/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     4372 2023-05-03 05:13:03.000000 ghananews-scraper-1.0.8/yen/scraper.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghananews-scraper-1.0.8/yen/utils.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-20 07:37:20.000000 ghananews-scraper-1.0.9/
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-20 07:37:20.000000 ghananews-scraper-1.0.9/3news/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-04-30 16:57:53.000000 ghananews-scraper-1.0.9/3news/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     8680 2023-05-20 07:36:58.000000 ghananews-scraper-1.0.9/3news/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghananews-scraper-1.0.9/3news/utils.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)    11741 2023-05-20 07:37:20.000000 ghananews-scraper-1.0.9/PKG-INFO
+-rw-r--r--   0 tsiameh    (501) staff       (20)     8354 2023-05-20 03:08:02.000000 ghananews-scraper-1.0.9/README.md
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-20 07:37:20.000000 ghananews-scraper-1.0.9/citionline/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-04-29 20:41:04.000000 ghananews-scraper-1.0.9/citionline/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     3478 2023-05-03 05:13:03.000000 ghananews-scraper-1.0.9/citionline/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghananews-scraper-1.0.9/citionline/utils.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-20 07:37:20.000000 ghananews-scraper-1.0.9/ghananews_scraper.egg-info/
+-rw-r--r--   0 tsiameh    (501) staff       (20)    11741 2023-05-20 07:37:19.000000 ghananews-scraper-1.0.9/ghananews_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 tsiameh    (501) staff       (20)      738 2023-05-20 07:37:20.000000 ghananews-scraper-1.0.9/ghananews_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)        1 2023-05-20 07:37:19.000000 ghananews-scraper-1.0.9/ghananews_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)       13 2023-05-20 07:37:19.000000 ghananews-scraper-1.0.9/ghananews_scraper.egg-info/requires.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)       77 2023-05-20 07:37:19.000000 ghananews-scraper-1.0.9/ghananews_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-20 07:37:20.000000 ghananews-scraper-1.0.9/ghanaweb/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-03-13 15:04:12.000000 ghananews-scraper-1.0.9/ghanaweb/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     4317 2023-05-03 05:13:03.000000 ghananews-scraper-1.0.9/ghanaweb/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-16 02:31:26.000000 ghananews-scraper-1.0.9/ghanaweb/utils.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-20 07:37:20.000000 ghananews-scraper-1.0.9/graphiconline/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-04-30 14:50:37.000000 ghananews-scraper-1.0.9/graphiconline/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     3716 2023-05-03 05:13:03.000000 ghananews-scraper-1.0.9/graphiconline/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghananews-scraper-1.0.9/graphiconline/utils.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     1457 2023-04-30 16:53:26.000000 ghananews-scraper-1.0.9/graphiconline.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-20 07:37:20.000000 ghananews-scraper-1.0.9/modernghana/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-01 18:28:50.000000 ghananews-scraper-1.0.9/modernghana/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     3273 2023-05-01 18:29:39.000000 ghananews-scraper-1.0.9/modernghana/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghananews-scraper-1.0.9/modernghana/utils.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-20 07:37:20.000000 ghananews-scraper-1.0.9/myjoyonline/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-03-15 14:35:44.000000 ghananews-scraper-1.0.9/myjoyonline/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     6425 2023-05-03 05:13:03.000000 ghananews-scraper-1.0.9/myjoyonline/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      789 2023-05-03 05:13:03.000000 ghananews-scraper-1.0.9/myjoyonline/utils.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-20 07:37:20.000000 ghananews-scraper-1.0.9/mynewsgh/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-18 09:08:24.000000 ghananews-scraper-1.0.9/mynewsgh/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     5875 2023-05-20 07:36:58.000000 ghananews-scraper-1.0.9/mynewsgh/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-05-18 09:19:40.000000 ghananews-scraper-1.0.9/mynewsgh/utils.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     1663 2023-05-18 09:00:25.000000 ghananews-scraper-1.0.9/mynewsgh.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)       38 2023-05-20 07:37:20.000000 ghananews-scraper-1.0.9/setup.cfg
+-rw-r--r--   0 tsiameh    (501) staff       (20)     1848 2023-05-20 07:36:58.000000 ghananews-scraper-1.0.9/setup.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-20 07:37:20.000000 ghananews-scraper-1.0.9/yen/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-04-30 18:14:26.000000 ghananews-scraper-1.0.9/yen/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     4372 2023-05-03 05:13:03.000000 ghananews-scraper-1.0.9/yen/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghananews-scraper-1.0.9/yen/utils.py
```

### Comparing `ghananews-scraper-1.0.8/3news/scraper.py` & `ghananews-scraper-1.0.9/modernghana/scraper.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import csv
 import os
+from datetime import datetime
 from urllib.parse import unquote
+
 import requests
 from bs4 import BeautifulSoup
-from .utils import SaveFile, HEADERS
 
+from .utils import HEADERS, SaveFile
+
+BASE_PAGE = 'https://www.graphic.com.gh'
 
-class ThreeNews:
+
+class ModernGhana:
     def __init__(self, url):
         if not url.startswith(("http://", "https://")):
             raise ValueError("Invalid URL: must start with 'http://' or 'https://'")
         self.url = url
         self.file_name = unquote(
             url.split("/")[-2] if url.endswith("/") else url.split("/")[-1]
         )
@@ -18,55 +23,59 @@
     def download(self, output_dir=None):
         """scrape data"""
         with requests.Session() as session:
             response = session.get(self.url, headers=HEADERS)
         soup = BeautifulSoup(response.text, "html.parser")
 
         lst_pages = [
-            page.a["href"] for page in soup.find_all("div", class_="jeg_thumb")
+            BASE_PAGE + page.a["href"] for page in soup.find_all('td', class_='list-title')
         ]
 
         try:
             print("saving results to csv...")
             if output_dir is None:
                 output_dir = os.getcwd()
                 SaveFile.mkdir(output_dir)
             if not os.path.isdir(output_dir):
                 raise ValueError(
                     f"Invalid output directory: {output_dir} is not a directory"
                 )
             print(f"File will be saved to: {output_dir}")
+
+            stamp = datetime.strftime(datetime.utcnow(), "%Y-%m-%d")
             with open(
-                os.path.join(output_dir, self.file_name + ".csv"),
-                mode="w",
-                newline="",
-                encoding="utf-8",
+                    os.path.join(output_dir, self.file_name + f"_{stamp}.csv"),
+                    mode="w",
+                    newline="",
+                    encoding="utf-8",
             ) as csv_file:
                 fieldnames = ["title", "content", "published_date", "page_url"]
                 writer = csv.DictWriter(csv_file, fieldnames=fieldnames)
                 writer.writeheader()
 
                 for page_url in lst_pages:
                     with requests.Session() as session:
                         response_page = session.get(page_url, headers=HEADERS)
                         soup_page = BeautifulSoup(response_page.text, "html.parser")
 
-                        title = soup_page.find("h1", class_="jeg_post_title")
+                        title = soup_page.find("div", class_="article-header")
                         title = title.text.strip() if title else ""
 
-                        content = soup_page.find("div", class_="content-inner")
-                        content = content.text.strip() if content else ""
+                        content_main = None
+                        content = soup_page.find("div", {"class": "article-details"}).select("div p")
+                        for tag in content:
+                            content_main = tag.get_text().strip() if tag else ""
 
-                        published_date = soup_page.find("div", class_="jeg_meta_date")
+                        published_date = soup_page.find("div", {"class": "article-info"}).find("span", class_="published")
                         published_date = published_date.text.strip() if published_date else ""
 
                         writer.writerow(
                             {
                                 "title": title,
-                                "content": content,
+                                "content": content_main,
                                 "published_date": published_date,
                                 "page_url": page_url,
                             }
                         )
                 print("Writing data to file...")
         except Exception as err:
             print(f"error: {err}")
```

### Comparing `ghananews-scraper-1.0.8/3news/utils.py` & `ghananews-scraper-1.0.9/3news/utils.py`

 * *Files identical despite different names*

### Comparing `ghananews-scraper-1.0.8/PKG-INFO` & `ghananews-scraper-1.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghananews-scraper
-Version: 1.0.8
+Version: 1.0.9
 Summary: A python package to scrape data from Ghana News Portals
 Home-page: https://github.com/donwany/ghananews-scraper
 Author: Theophilus Siameh
 Author-email: theodondre@gmail.com
 License: MIT License
 Description: ![Python 3.7, 3.8, 3.9](https://img.shields.io/badge/Python-3.7%2C%203.8%2C%203.9-3776ab.svg?maxAge=2592000)
         [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
@@ -12,15 +12,16 @@
         ### GhanaNews Scraper
           A simple unofficial python package to scrape data from 
           [GhanaWeb](https://www.ghanaweb.com),
           [MyJoyOnline](https://www.myjoyonline.com),
           [DailyGraphic](https://www.graphic.com.gh),
           [CitiBusinessNews](https://citibusinessnews.com),
           [YenGH](https://www.yen.com.gh),
-          Affiliated to [bank-of-ghana-fx-rates](https://pypi.org/project/bank-of-ghana-fx-rates/)
+          Affiliated to [bank of ghana fx rates](https://pypi.org/project/bank-of-ghana-fx-rates/) and 
+          [GhanaShops-Scraper](https://pypi.org/project/ghanashops-scraper/)
         
         ### How to install
         ```shell
         pip install ghananews-scraper
         ```
         
         ### Example Google Colab Notebook
@@ -182,26 +183,96 @@
         
         for url in urls:
             print(f"Downloading data from: {url}")
             yen = Yen(url=url)
             yen.download()
         ```
         
+        ### Scrape data from [MyNewsGh](https://mynewsgh.com)
+        ```python
+        from mynewsgh.scraper import MyNewsGh
+        
+        # scrape from multiple URLs
+        urls = [
+          "https://www.mynewsgh.com/category/politics/",
+          "https://www.mynewsgh.com/category/news/",
+          "https://www.mynewsgh.com/category/entertainment/",
+          "https://www.mynewsgh.com/category/business/",
+          "https://www.mynewsgh.com/category/lifestyle/",
+          "https://www.mynewsgh.com/tag/feature/",
+          "https://www.mynewsgh.com/category/world/",
+          "https://www.mynewsgh.com/category/sports/"
+        ]
+        
+        for url in urls:
+            print(f"Downloading data from: {url}")
+            my_news = MyNewsGh(url=url, limit_pages=50)
+            my_news.download()
+        
+        # scrape from a single URL
+        from mynewsgh.scraper import MyNewsGh
+        
+        url = "https://www.mynewsgh.com/category/politics/"
+        my_news = MyNewsGh(url=url, limit_pages=None)
+        my_news.download()
+        ```
+        ### Scrape data from [3News](https://3news.com)
+        ```python
+        from 3news.scraper import ThreeNews
+        
+        # DO NOT RUN ALL AUTHORS: select ONLY few
+        # DO NOT CHANGE THE AUTHOR NAMES
+        authors = [
+          "laud-nartey",
+          "3xtra",
+          "essel-issac",
+          "arabaincoom",
+          "bbc",
+          "betty-kankam-boadu",
+          "kwameamoh",
+          "fiifi_forson",
+          "fdoku",
+          "frankappiah",
+          "godwin-asediba",
+          "afua-somuah",
+          "irene",
+          "joyce-sesi",
+          "3news_user",
+          "ntollo",
+          "pwaberi-denis",
+          "sonia-amade",
+          "effah-steven",
+          "michael-tetteh"
+        ]
+        
+        for author in authors:
+            print(f"Downloading data from author: {author}")
+            three_news = ThreeNews(author=author, limit_pages=50)
+            three_news.download()
+            
+        # OR
+        from 3news.scraper import ThreeNews
+        
+        three = ThreeNews(author="laud-nartey", limit_pages=None)
+        three.download()
+        
+        ```
+        
         
         BuyMeCoffee
         -----------
         [![Build](https://www.buymeacoffee.com/assets/img/custom_images/yellow_img.png)](https://www.buymeacoffee.com/theodondrew)
         
         Credits
         -------
         -  `Theophilus Siameh`
         <div>
             <a href="https://twitter.com/tsiameh"><img src="https://img.shields.io/twitter/follow/tsiameh?color=blue&logo=twitter&style=flat" alt="tsiameh twitter"></a>
         </div>
-Keywords: Scraper,Data,GhanaNews,GhanaWeb,JoyNews,MyJoyOnline,News,Web Scraper,Ghana Scraper
+Keywords: Scraper,Data,GhanaNews,GhanaWeb,JoyNews,MyJoyOnline,News,Yen,MyNewsGh,3news,Web Scraper,Ghana Scraper
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `ghananews-scraper-1.0.8/citionline/scraper.py` & `ghananews-scraper-1.0.9/citionline/scraper.py`

 * *Files identical despite different names*

### Comparing `ghananews-scraper-1.0.8/citionline/utils.py` & `ghananews-scraper-1.0.9/citionline/utils.py`

 * *Files identical despite different names*

### Comparing `ghananews-scraper-1.0.8/ghananews_scraper.egg-info/PKG-INFO` & `ghananews-scraper-1.0.9/ghananews_scraper.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghananews-scraper
-Version: 1.0.8
+Version: 1.0.9
 Summary: A python package to scrape data from Ghana News Portals
 Home-page: https://github.com/donwany/ghananews-scraper
 Author: Theophilus Siameh
 Author-email: theodondre@gmail.com
 License: MIT License
 Description: ![Python 3.7, 3.8, 3.9](https://img.shields.io/badge/Python-3.7%2C%203.8%2C%203.9-3776ab.svg?maxAge=2592000)
         [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
@@ -12,15 +12,16 @@
         ### GhanaNews Scraper
           A simple unofficial python package to scrape data from 
           [GhanaWeb](https://www.ghanaweb.com),
           [MyJoyOnline](https://www.myjoyonline.com),
           [DailyGraphic](https://www.graphic.com.gh),
           [CitiBusinessNews](https://citibusinessnews.com),
           [YenGH](https://www.yen.com.gh),
-          Affiliated to [bank-of-ghana-fx-rates](https://pypi.org/project/bank-of-ghana-fx-rates/)
+          Affiliated to [bank of ghana fx rates](https://pypi.org/project/bank-of-ghana-fx-rates/) and 
+          [GhanaShops-Scraper](https://pypi.org/project/ghanashops-scraper/)
         
         ### How to install
         ```shell
         pip install ghananews-scraper
         ```
         
         ### Example Google Colab Notebook
@@ -182,26 +183,96 @@
         
         for url in urls:
             print(f"Downloading data from: {url}")
             yen = Yen(url=url)
             yen.download()
         ```
         
+        ### Scrape data from [MyNewsGh](https://mynewsgh.com)
+        ```python
+        from mynewsgh.scraper import MyNewsGh
+        
+        # scrape from multiple URLs
+        urls = [
+          "https://www.mynewsgh.com/category/politics/",
+          "https://www.mynewsgh.com/category/news/",
+          "https://www.mynewsgh.com/category/entertainment/",
+          "https://www.mynewsgh.com/category/business/",
+          "https://www.mynewsgh.com/category/lifestyle/",
+          "https://www.mynewsgh.com/tag/feature/",
+          "https://www.mynewsgh.com/category/world/",
+          "https://www.mynewsgh.com/category/sports/"
+        ]
+        
+        for url in urls:
+            print(f"Downloading data from: {url}")
+            my_news = MyNewsGh(url=url, limit_pages=50)
+            my_news.download()
+        
+        # scrape from a single URL
+        from mynewsgh.scraper import MyNewsGh
+        
+        url = "https://www.mynewsgh.com/category/politics/"
+        my_news = MyNewsGh(url=url, limit_pages=None)
+        my_news.download()
+        ```
+        ### Scrape data from [3News](https://3news.com)
+        ```python
+        from 3news.scraper import ThreeNews
+        
+        # DO NOT RUN ALL AUTHORS: select ONLY few
+        # DO NOT CHANGE THE AUTHOR NAMES
+        authors = [
+          "laud-nartey",
+          "3xtra",
+          "essel-issac",
+          "arabaincoom",
+          "bbc",
+          "betty-kankam-boadu",
+          "kwameamoh",
+          "fiifi_forson",
+          "fdoku",
+          "frankappiah",
+          "godwin-asediba",
+          "afua-somuah",
+          "irene",
+          "joyce-sesi",
+          "3news_user",
+          "ntollo",
+          "pwaberi-denis",
+          "sonia-amade",
+          "effah-steven",
+          "michael-tetteh"
+        ]
+        
+        for author in authors:
+            print(f"Downloading data from author: {author}")
+            three_news = ThreeNews(author=author, limit_pages=50)
+            three_news.download()
+            
+        # OR
+        from 3news.scraper import ThreeNews
+        
+        three = ThreeNews(author="laud-nartey", limit_pages=None)
+        three.download()
+        
+        ```
+        
         
         BuyMeCoffee
         -----------
         [![Build](https://www.buymeacoffee.com/assets/img/custom_images/yellow_img.png)](https://www.buymeacoffee.com/theodondrew)
         
         Credits
         -------
         -  `Theophilus Siameh`
         <div>
             <a href="https://twitter.com/tsiameh"><img src="https://img.shields.io/twitter/follow/tsiameh?color=blue&logo=twitter&style=flat" alt="tsiameh twitter"></a>
         </div>
-Keywords: Scraper,Data,GhanaNews,GhanaWeb,JoyNews,MyJoyOnline,News,Web Scraper,Ghana Scraper
+Keywords: Scraper,Data,GhanaNews,GhanaWeb,JoyNews,MyJoyOnline,News,Yen,MyNewsGh,3news,Web Scraper,Ghana Scraper
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `ghananews-scraper-1.0.8/ghanaweb/scraper.py` & `ghananews-scraper-1.0.9/ghanaweb/scraper.py`

 * *Files identical despite different names*

### Comparing `ghananews-scraper-1.0.8/ghanaweb/utils.py` & `ghananews-scraper-1.0.9/ghanaweb/utils.py`

 * *Files identical despite different names*

### Comparing `ghananews-scraper-1.0.8/graphiconline/scraper.py` & `ghananews-scraper-1.0.9/graphiconline/scraper.py`

 * *Files identical despite different names*

### Comparing `ghananews-scraper-1.0.8/graphiconline/utils.py` & `ghananews-scraper-1.0.9/graphiconline/utils.py`

 * *Files identical despite different names*

### Comparing `ghananews-scraper-1.0.8/graphiconline.py` & `ghananews-scraper-1.0.9/graphiconline.py`

 * *Files identical despite different names*

### Comparing `ghananews-scraper-1.0.8/modernghana/utils.py` & `ghananews-scraper-1.0.9/modernghana/utils.py`

 * *Files identical despite different names*

### Comparing `ghananews-scraper-1.0.8/myjoyonline/scraper.py` & `ghananews-scraper-1.0.9/myjoyonline/scraper.py`

 * *Files identical despite different names*

### Comparing `ghananews-scraper-1.0.8/myjoyonline/utils.py` & `ghananews-scraper-1.0.9/myjoyonline/utils.py`

 * *Files identical despite different names*

### Comparing `ghananews-scraper-1.0.8/setup.py` & `ghananews-scraper-1.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
     README = f.read()
 
 with open("requirements.txt", "r") as f:
     install_requires = f.read().splitlines()
 
 setup(
     name='ghananews-scraper',
-    py_modules=['ghanaweb', 'myjoyonline', 'graphiconline', 'yen', 'citionline'],
-    version='1.0.8',
+    py_modules=['ghanaweb', 'myjoyonline', 'graphiconline', 'yen', 'citionline', "mynewsgh", "3news"],
+    version='1.0.9',
     packages=find_packages(exclude=["docs", "tests", "tests.*"]),
     long_description=README,
     long_description_content_type="text/markdown",
     url='https://github.com/donwany/ghananews-scraper',
     license="MIT License",
     author='Theophilus Siameh',
     author_email='theodondre@gmail.com',
@@ -34,11 +34,11 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Software Development :: Testing",
         "Topic :: Utilities",
     ],
-    keywords="Scraper, Data, GhanaNews, GhanaWeb, JoyNews, MyJoyOnline, News, Web Scraper, Ghana Scraper",
+    keywords="Scraper, Data, GhanaNews, GhanaWeb, JoyNews, MyJoyOnline, News, Yen, MyNewsGh, 3news, Web Scraper, Ghana Scraper",
     platforms=["any"],
     python_requires=">=3.7",
 )
```

### Comparing `ghananews-scraper-1.0.8/yen/scraper.py` & `ghananews-scraper-1.0.9/yen/scraper.py`

 * *Files identical despite different names*

### Comparing `ghananews-scraper-1.0.8/yen/utils.py` & `ghananews-scraper-1.0.9/mynewsgh/utils.py`

 * *Files identical despite different names*

