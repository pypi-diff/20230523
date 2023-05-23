# Comparing `tmp/filmweb-0.6.tar.gz` & `tmp/filmweb-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filmweb-0.6.tar", last modified: Sat Jan 21 16:35:10 2023, max compression
+gzip compressed data, was "filmweb-0.7.tar", last modified: Tue May 23 16:27:03 2023, max compression
```

## Comparing `filmweb-0.6.tar` & `filmweb-0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-01-21 16:35:10.216042 filmweb-0.6/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1070 2020-08-04 13:32:10.000000 filmweb-0.6/LICENSE
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6258 2023-01-21 16:35:10.216042 filmweb-0.6/PKG-INFO
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5728 2023-01-21 16:28:36.000000 filmweb-0.6/README.md
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-01-21 16:35:10.212042 filmweb-0.6/filmweb/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-01-20 17:59:47.000000 filmweb-0.6/filmweb/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2842 2023-01-20 18:02:58.000000 filmweb-0.6/filmweb/getter.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2965 2023-01-20 18:21:47.000000 filmweb-0.6/filmweb/main.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2696 2023-01-21 16:08:00.000000 filmweb-0.6/filmweb/parser.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-01-21 16:35:10.216042 filmweb-0.6/filmweb.egg-info/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6258 2023-01-21 16:35:10.000000 filmweb-0.6/filmweb.egg-info/PKG-INFO
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      309 2023-01-21 16:35:10.000000 filmweb-0.6/filmweb.egg-info/SOURCES.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2023-01-21 16:35:10.000000 filmweb-0.6/filmweb.egg-info/dependency_links.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       46 2023-01-21 16:35:10.000000 filmweb-0.6/filmweb.egg-info/entry_points.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      162 2023-01-21 16:35:10.000000 filmweb-0.6/filmweb.egg-info/requires.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        8 2023-01-21 16:35:10.000000 filmweb-0.6/filmweb.egg-info/top_level.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      824 2023-01-20 09:39:36.000000 filmweb-0.6/pyproject.toml
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      162 2023-01-20 15:29:12.000000 filmweb-0.6/requirements.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       38 2023-01-21 16:35:10.216042 filmweb-0.6/setup.cfg
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-05-23 16:27:03.682055 filmweb-0.7/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1070 2020-08-04 13:32:10.000000 filmweb-0.7/LICENSE
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6072 2023-05-23 16:27:03.678055 filmweb-0.7/PKG-INFO
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5542 2023-05-23 16:14:25.000000 filmweb-0.7/README.md
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-05-23 16:27:03.674055 filmweb-0.7/filmweb/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-01-20 17:59:47.000000 filmweb-0.7/filmweb/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2842 2023-05-23 15:14:56.000000 filmweb-0.7/filmweb/getter.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2992 2023-05-23 15:53:42.000000 filmweb-0.7/filmweb/main.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3489 2023-05-23 15:57:56.000000 filmweb-0.7/filmweb/parser.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-05-23 16:27:03.678055 filmweb-0.7/filmweb.egg-info/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6072 2023-05-23 16:27:03.000000 filmweb-0.7/filmweb.egg-info/PKG-INFO
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      309 2023-05-23 16:27:03.000000 filmweb-0.7/filmweb.egg-info/SOURCES.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2023-05-23 16:27:03.000000 filmweb-0.7/filmweb.egg-info/dependency_links.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       46 2023-05-23 16:27:03.000000 filmweb-0.7/filmweb.egg-info/entry_points.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      153 2023-05-23 16:27:03.000000 filmweb-0.7/filmweb.egg-info/requires.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        8 2023-05-23 16:27:03.000000 filmweb-0.7/filmweb.egg-info/top_level.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      824 2023-05-23 08:48:38.000000 filmweb-0.7/pyproject.toml
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      153 2023-05-23 08:48:14.000000 filmweb-0.7/requirements.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       38 2023-05-23 16:27:03.682055 filmweb-0.7/setup.cfg
```

### Comparing `filmweb-0.6/LICENSE` & `filmweb-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `filmweb-0.6/PKG-INFO` & `filmweb-0.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filmweb
-Version: 0.6
+Version: 0.7
 Summary: Export movie ratings from filmweb.pl
 Author: Piotr Patrzyk
 License: MIT
 Project-URL: Source, https://github.com/ppatrzyk/filmweb
 Keywords: filmweb,movie,crawler,data
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -53,79 +53,78 @@
 4. Skopiuj wartość *Cookie* i podaj ją jako argument do skryptu.
 
 ![Browser Screenshot](browser_screen.jpg)
 
 ### Przykład
 
 ```
-$ filmweb -f all pieca "didomi_token=(...)=="
+$ filmweb -f csv -f json pieca "didomi_token=(...)=="
 INFO:root:Checking args...
-INFO:root:Fetching list of movies...
-100%|██████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 38/38 [00:06<00:00,  6.26it/s]
-INFO:root:Parsing list of movies...
-100%|██████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 38/38 [00:02<00:00, 12.79it/s]
-INFO:root:User pieca has 926 movies...
-INFO:root:Fetching movie details...
-INFO:root:Fetching user ratings [1/3]...
-100%|████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 926/926 [00:39<00:00, 23.49it/s]
-INFO:root:Fetching info about movies [2/3]...
-100%|████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 926/926 [00:43<00:00, 21.22it/s]
-INFO:root:Fetching global rating for movies [3/3]...
-100%|████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 926/926 [00:43<00:00, 21.36it/s]
-INFO:root:Writing data...
-INFO:root:pieca_filmweb_20230121.json written!
-INFO:root:pieca_filmweb_20230121.csv written!
-$ cat pieca_filmweb_20230121.json | jq .[0]
+INFO:root:Fetching list of movies [1/6]...
+100%|██████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 38/38 [00:07<00:00,  4.98it/s]
+INFO:root:Parsing list of movies [2/6]...
+100%|██████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 38/38 [00:02<00:00, 15.47it/s]
+INFO:root:User pieca has 938 movies...
+INFO:root:Fetching user ratings [3/6]...
+100%|████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 938/938 [00:34<00:00, 27.34it/s]
+INFO:root:Fetching info about movies [4/6]...
+100%|████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 938/938 [00:33<00:00, 27.63it/s]
+INFO:root:Fetching global rating for movies [5/6]...
+100%|████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 938/938 [00:35<00:00, 26.57it/s]
+INFO:root:Writing data [6/6]...
+INFO:root:pieca_20230523.json written!
+INFO:root:pieca_20230523.csv written!
+$ cat pieca_20230523.json | jq .[0]
 {
-  "timestamp": 1657484863818,
-  "favorite": false,
-  "user_rating": 8,
-  "global_rating": 7.36859,
-  "global_rating_count": 1579,
-  "original_title": "Tehran Taboo",
-  "pl_title": "Teheran tabu",
-  "year": 2017,
-  "movie_id": "786978",
-  "url": "https://www.filmweb.pl/film/Teheran+tabu-2017-786978"
+  "timestamp": 1579354599456,
+  "favorite": null,
+  "user_rating": 5,
+  "global_rating": 6.03865,
+  "global_rating_count": 414,
+  "original_title": "Ejdeha Vared Mishavad!",
+  "pl_title": "Wejście smoka!",
+  "year": 2016,
+  "movie_id": "757318",
+  "url": "https://www.filmweb.pl/film/Wej%C5%9Bcie+smoka%21-2016-757318",
+  "date": "2020-01-18"
 }
-$ cat pieca_filmweb_20230121.csv | xsv sample 5 | xsv table
-timestamp      favorite  user_rating  global_rating  global_rating_count  original_title  pl_title       year  movie_id  url
-1464302814850  False     4            6.91279        1743                 Pupendo         Pupendo        2003  103930    https://www.filmweb.pl/film/Pupendo-2003-103930
-1581177494926  False     7            6.51905        210                  Dukhtar         Dukhtar        2014  727743    https://www.filmweb.pl/film/Dukhtar-2014-727743
-1601716769499  False     8            7.59777        179                  Shah-re ziba    Piękne miasto  2004  155344    https://www.filmweb.pl/film/Pi%C4%99kne+miasto-2004-155344
-1548505975360  False     8            7.12276        1784                 Geu-mul         W sieci        2016  766555    https://www.filmweb.pl/film/W+sieci-2016-766555
-1638616845248  False     5            6.59127        115166               Ida             Ida            2013  546529    https://www.filmweb.pl/film/Ida-2013-546529
+$ cat pieca_20230523.csv | xsv sample 3 | xsv table
+timestamp      favorite  user_rating  global_rating  global_rating_count  original_title          pl_title                 year  movie_id  url                                                                  date
+1588407481213            9            7.91448        3777                 Werckmeister harmóniák  Harmonie Werckmeistera   2000  117108    https://www.filmweb.pl/film/Harmonie+Werckmeistera-2000-117108       2020-05-02
+1425511804375            4            6.69102        87448                Czas surferów           Czas surferów            2005  137466    https://www.filmweb.pl/film/Czas+surfer%C3%B3w-2005-137466           2015-03-05
+1496177689168            6            7.16478        619                  Kukačka v temném lese   Kukułka w ciemnym lesie  1984  35947     https://www.filmweb.pl/film/Kuku%C5%82ka+w+ciemnym+lesie-1984-35947  2017-05-30             2015-03-05
 ```
 
 ### Wszystkie opcje
 
 ```
 $ filmweb -h
 filmweb
 
 Usage:
-    filmweb [--format=<fileformat>] [--debug] <username> <cookie>
+    filmweb [--format=<fileformat>]... [--debug] <username> <cookie>
 
 Options:
     -h --help                     Show this screen
-    -f --format=<fileformat>      Output file format: json (default), csv, all (writes both)
-    -d --debug                    Debug prints                 Debug prints
+    -f --format=<fileformat>      Output file format: json (default), csv, letterboxd
+    -d --debug                    Debug prints
 ```
 
 ## Dostępne dane:
 
 Kolumna | Opis
 --- | ---
 year | _premiera_
 global\_rating\_count | _ilość ocen filmu_
 global\_rating | _ocena filmweb_
 timestamp | _[czas oceny (unix)](https://pl.wikipedia.org/wiki/Czas_uniksowy)_
+date | _data oceny_ (yyyy-mm-dd)
 user\_rating | _ocena użytkownika_
 favorite | _dodany do ulubionych_
 original\_title | _tytuł oryginalny_
 pl\_title | _tytuł polski_
-movie\_id | _id filmu_
+movie\_id | _id filmu_ (filmweb)
 url | _strona filmu_
 
 ## Znane problemy:
 
 - Eksport tylko ocen filmów, inne (np. seriale) niedostępne,
```

### Comparing `filmweb-0.6/README.md` & `filmweb-0.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -36,79 +36,78 @@
 4. Skopiuj wartość *Cookie* i podaj ją jako argument do skryptu.
 
 ![Browser Screenshot](browser_screen.jpg)
 
 ### Przykład
 
 ```
-$ filmweb -f all pieca "didomi_token=(...)=="
+$ filmweb -f csv -f json pieca "didomi_token=(...)=="
 INFO:root:Checking args...
-INFO:root:Fetching list of movies...
-100%|██████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 38/38 [00:06<00:00,  6.26it/s]
-INFO:root:Parsing list of movies...
-100%|██████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 38/38 [00:02<00:00, 12.79it/s]
-INFO:root:User pieca has 926 movies...
-INFO:root:Fetching movie details...
-INFO:root:Fetching user ratings [1/3]...
-100%|████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 926/926 [00:39<00:00, 23.49it/s]
-INFO:root:Fetching info about movies [2/3]...
-100%|████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 926/926 [00:43<00:00, 21.22it/s]
-INFO:root:Fetching global rating for movies [3/3]...
-100%|████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 926/926 [00:43<00:00, 21.36it/s]
-INFO:root:Writing data...
-INFO:root:pieca_filmweb_20230121.json written!
-INFO:root:pieca_filmweb_20230121.csv written!
-$ cat pieca_filmweb_20230121.json | jq .[0]
+INFO:root:Fetching list of movies [1/6]...
+100%|██████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 38/38 [00:07<00:00,  4.98it/s]
+INFO:root:Parsing list of movies [2/6]...
+100%|██████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 38/38 [00:02<00:00, 15.47it/s]
+INFO:root:User pieca has 938 movies...
+INFO:root:Fetching user ratings [3/6]...
+100%|████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 938/938 [00:34<00:00, 27.34it/s]
+INFO:root:Fetching info about movies [4/6]...
+100%|████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 938/938 [00:33<00:00, 27.63it/s]
+INFO:root:Fetching global rating for movies [5/6]...
+100%|████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 938/938 [00:35<00:00, 26.57it/s]
+INFO:root:Writing data [6/6]...
+INFO:root:pieca_20230523.json written!
+INFO:root:pieca_20230523.csv written!
+$ cat pieca_20230523.json | jq .[0]
 {
-  "timestamp": 1657484863818,
-  "favorite": false,
-  "user_rating": 8,
-  "global_rating": 7.36859,
-  "global_rating_count": 1579,
-  "original_title": "Tehran Taboo",
-  "pl_title": "Teheran tabu",
-  "year": 2017,
-  "movie_id": "786978",
-  "url": "https://www.filmweb.pl/film/Teheran+tabu-2017-786978"
+  "timestamp": 1579354599456,
+  "favorite": null,
+  "user_rating": 5,
+  "global_rating": 6.03865,
+  "global_rating_count": 414,
+  "original_title": "Ejdeha Vared Mishavad!",
+  "pl_title": "Wejście smoka!",
+  "year": 2016,
+  "movie_id": "757318",
+  "url": "https://www.filmweb.pl/film/Wej%C5%9Bcie+smoka%21-2016-757318",
+  "date": "2020-01-18"
 }
-$ cat pieca_filmweb_20230121.csv | xsv sample 5 | xsv table
-timestamp      favorite  user_rating  global_rating  global_rating_count  original_title  pl_title       year  movie_id  url
-1464302814850  False     4            6.91279        1743                 Pupendo         Pupendo        2003  103930    https://www.filmweb.pl/film/Pupendo-2003-103930
-1581177494926  False     7            6.51905        210                  Dukhtar         Dukhtar        2014  727743    https://www.filmweb.pl/film/Dukhtar-2014-727743
-1601716769499  False     8            7.59777        179                  Shah-re ziba    Piękne miasto  2004  155344    https://www.filmweb.pl/film/Pi%C4%99kne+miasto-2004-155344
-1548505975360  False     8            7.12276        1784                 Geu-mul         W sieci        2016  766555    https://www.filmweb.pl/film/W+sieci-2016-766555
-1638616845248  False     5            6.59127        115166               Ida             Ida            2013  546529    https://www.filmweb.pl/film/Ida-2013-546529
+$ cat pieca_20230523.csv | xsv sample 3 | xsv table
+timestamp      favorite  user_rating  global_rating  global_rating_count  original_title          pl_title                 year  movie_id  url                                                                  date
+1588407481213            9            7.91448        3777                 Werckmeister harmóniák  Harmonie Werckmeistera   2000  117108    https://www.filmweb.pl/film/Harmonie+Werckmeistera-2000-117108       2020-05-02
+1425511804375            4            6.69102        87448                Czas surferów           Czas surferów            2005  137466    https://www.filmweb.pl/film/Czas+surfer%C3%B3w-2005-137466           2015-03-05
+1496177689168            6            7.16478        619                  Kukačka v temném lese   Kukułka w ciemnym lesie  1984  35947     https://www.filmweb.pl/film/Kuku%C5%82ka+w+ciemnym+lesie-1984-35947  2017-05-30             2015-03-05
 ```
 
 ### Wszystkie opcje
 
 ```
 $ filmweb -h
 filmweb
 
 Usage:
-    filmweb [--format=<fileformat>] [--debug] <username> <cookie>
+    filmweb [--format=<fileformat>]... [--debug] <username> <cookie>
 
 Options:
     -h --help                     Show this screen
-    -f --format=<fileformat>      Output file format: json (default), csv, all (writes both)
-    -d --debug                    Debug prints                 Debug prints
+    -f --format=<fileformat>      Output file format: json (default), csv, letterboxd
+    -d --debug                    Debug prints
 ```
 
 ## Dostępne dane:
 
 Kolumna | Opis
 --- | ---
 year | _premiera_
 global\_rating\_count | _ilość ocen filmu_
 global\_rating | _ocena filmweb_
 timestamp | _[czas oceny (unix)](https://pl.wikipedia.org/wiki/Czas_uniksowy)_
+date | _data oceny_ (yyyy-mm-dd)
 user\_rating | _ocena użytkownika_
 favorite | _dodany do ulubionych_
 original\_title | _tytuł oryginalny_
 pl\_title | _tytuł polski_
-movie\_id | _id filmu_
+movie\_id | _id filmu_ (filmweb)
 url | _strona filmu_
 
 ## Znane problemy:
 
 - Eksport tylko ocen filmów, inne (np. seriale) niedostępne,
```

### Comparing `filmweb-0.6/filmweb/getter.py` & `filmweb-0.7/filmweb/getter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import json
 import requests
 
 HEADERS = {
     # https://www.whatismybrowser.com/guides/the-latest-user-agent/firefox
-    'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 13.1; rv:109.0) Gecko/20100101 Firefox/109.0',
-    'x-locale': 'pl_PL',
-    'Host': 'www.filmweb.pl',
-    'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8',
-    'Accept-Language': 'en-US,en;q=0.5',
-    'Accept-Encoding': 'gzip, deflate, br',
-    'Origin': 'https://www.filmweb.pl',
-    'DNT': '1',
-    'Connection': 'keep-alive',
-    'Upgrade-Insecure-Requests': '1',
+    "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 13.4; rv:109.0) Gecko/20100101 Firefox/113.0",
+    "x-locale": "pl_PL",
+    "Host": "www.filmweb.pl",
+    "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8",
+    "Accept-Language": "en-US,en;q=0.5",
+    "Accept-Encoding": "gzip, deflate, br",
+    "Origin": "https://www.filmweb.pl",
+    "DNT": "1",
+    "Connection": "keep-alive",
+    "Upgrade-Insecure-Requests": "1",
 }
 
 def get_films_page(args):
     """
     request films page
     """
     # this workaround is necessary because multiprocessing imap takes one arg only
     (cookie, user, n) = args
-    url = f'https://www.filmweb.pl/user/{user}/films'
-    params = {'page': n}
-    response = requests.get(url, params=params, headers={'Cookie': cookie, **HEADERS})
+    url = f"https://www.filmweb.pl/user/{user}/films"
+    params = {"page": n}
+    response = requests.get(url, params=params, headers={"Cookie": cookie, **HEADERS})
     response.raise_for_status()
     return response.text
 
 def auth_check(cookie):
     """
     Check if auth is OK (valid cookie after login)
     """
@@ -38,15 +38,15 @@
 
 def get_votes_count(user):
     """
     Get total count of votes
     Args:
         user: user to get ratings for
     """
-    url = f'https://www.filmweb.pl/api/v1/user/{user}/votes/film/count'
+    url = f"https://www.filmweb.pl/api/v1/user/{user}/votes/film/count"
     return _get_json(url, "", "get_votes_count")
 
 def get_user_rating(args):
     """
     Gets user rating
     """
     (cookie, movie_id, user, friend_query) = args
@@ -78,14 +78,14 @@
     return json.dumps(data)
 
 def _get_json(url, cookie, func_name):
     """
     Wrapper for request and unified error
     """
     try:
-        response = requests.get(url, headers={'Cookie': cookie, **HEADERS})
+        response = requests.get(url, headers={"Cookie": cookie, **HEADERS})
         response.raise_for_status()
         content = response.json()
     except Exception as e:
-        raise ValueError(f'Failure in {func_name}: {str(e)}')
+        raise ValueError(f"Failure in {func_name}: {str(e)}")
     else:
         return content
```

### Comparing `filmweb-0.6/filmweb/parser.py` & `filmweb-0.7/filmweb/parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,80 +2,104 @@
 import logging
 import json
 from datetime import datetime
 from bs4 import BeautifulSoup
 from urllib.parse import quote_plus
 
 KEY_MAPPING = {
-    'timestamp': 'timestamp',
-    'favorite': 'favorite',
-    'rate': 'user_rating',
-    'global_rate': 'global_rating',
-    'count': 'global_rating_count',
-    'originalTitle': 'original_title',
-    'title': 'pl_title',
-    'year': 'year',
-    'movie_id': 'movie_id',
-    'url': 'url',
+    "timestamp": "timestamp",
+    "favorite": "favorite",
+    "rate": "user_rating",
+    "global_rate": "global_rating",
+    "count": "global_rating_count",
+    "originalTitle": "original_title",
+    "title": "pl_title",
+    "year": "year",
+    "movie_id": "movie_id",
+    "url": "url",
+    "date": "date",
 }
+# TODO? country/genre info not visible in api, would need to parse htmls
 
 def extract_movie_ids(content):
     """
     Extract movie ids from films page
     Args:
         content: raw html
     """
-    soup = BeautifulSoup(content, 'html.parser')
-    id_containers = soup.find_all('div', attrs={'data-film-id': True})
-    ids = set(el['data-film-id'] for el in id_containers)
+    soup = BeautifulSoup(content, "html.parser")
+    id_containers = soup.find_all("div", attrs={"data-film-id": True})
+    ids = set(el["data-film-id"] for el in id_containers)
     # necessary for multiprocessing pickle to work
     return json.dumps(list(ids))
 
 def merge_data(ids, user_ratings, global_info, global_rating):
     """
     Merge all data into one
     """
     all_data = tuple(_movie_id_key(el) for el in (user_ratings, global_info, global_rating))
     merged = ({**all_data[0][id], **all_data[1][id], **all_data[2][id]} for id in ids)
-    return tuple(_rewrite_keys(entry) for entry in merged)
+    return tuple(_fix_keys(entry) for entry in merged)
 
 def _movie_id_key(data):
     """
-    Reformat data into dict with movie_id as key
+    Parse and reformat data into dict with movie_id as key
     """
     data = (json.loads(el) for el in data)
     return {entry["movie_id"]: entry for entry in data}
 
-def _rewrite_keys(entry):
+def _fix_keys(entry):
     """
     Fix keys names for data
     """
     fixed = {new_key: entry.get(old_key) for old_key, new_key in KEY_MAPPING.items()}
     if fixed.get("original_title") is None:
         fixed["original_title"] = fixed["pl_title"]
-    path = quote_plus(f"{fixed['pl_title'].strip()}-{fixed['year']}-{fixed['movie_id']}")
+    path = quote_plus(f"""{fixed["pl_title"].strip()}-{fixed["year"]}-{fixed["movie_id"]}""")
     fixed["url"] = f"https://www.filmweb.pl/film/{path}"
+    fixed["date"] = datetime.fromtimestamp(fixed["timestamp"]/1000).strftime("%Y-%m-%d")
     return fixed
 
-def write_data(movies, user, data_format='json'):
+def _write_csv(file_name, field_names, movies):
     """
+    Helper for writing csv
     """
-    assert movies, 'no data to write'
-    date = datetime.now().strftime('%Y%m%d')
-    if data_format == 'all':
-        file_formats = ('csv', 'json')
-    else:
-        file_formats = (data_format, )
-    if 'json' in file_formats:
-        file_name = f'{user}_filmweb_{date}.json'
-        with open(file_name, 'w', encoding='utf-8') as out_file:
+    with open(file_name, "w", encoding="utf-8") as out_file:
+        writer = csv.DictWriter(out_file, fieldnames=field_names, dialect="unix")
+        writer.writeheader()
+        for movie in movies:
+            writer.writerow(movie)
+    return True
+
+def _letterbox_entry(entry):
+    """
+    Format letterboxd column names
+    https://letterboxd.com/about/importing-data/
+    """
+    fixed = {
+        "Title": entry.get("original_title"),
+        "Year": entry.get("year"),
+        "Rating10": entry.get("user_rating"),
+        "WatchedDate": entry.get("date"),
+    }
+    return fixed
+
+def write_data(movies, user, formats):
+    """
+    """
+    assert movies, "no data to write"
+    date = datetime.now().strftime("%Y%m%d")
+    if "json" in formats:
+        file_name = f"{user}_{date}.json"
+        with open(file_name, "w", encoding="utf-8") as out_file:
             out_file.write(json.dumps(movies))
-        logging.info(f'{file_name} written!')
-    if 'csv' in file_formats:
-        file_name = f'{user}_filmweb_{date}.csv'
-        with open(file_name, 'w', encoding='utf-8') as out_file:
-            writer = csv.DictWriter(out_file, fieldnames=KEY_MAPPING.values(), dialect='unix')
-            writer.writeheader()
-            for movie in movies:
-                writer.writerow(movie)
-        logging.info(f'{file_name} written!')
+        logging.info(f"{file_name} written!")
+    if "csv" in formats:
+        file_name = f"{user}_{date}.csv"
+        _write_csv(file_name, KEY_MAPPING.values(), movies)
+        logging.info(f"{file_name} written!")
+    if "letterboxd" in formats:
+        file_name = f"{user}_{date}_letterboxd.csv"
+        movies_letterbox = tuple(_letterbox_entry(entry) for entry in movies)
+        _write_csv(file_name, movies_letterbox[0].keys(), movies_letterbox)
+        logging.info(f"{file_name} written!")
     return file_name
```

### Comparing `filmweb-0.6/filmweb.egg-info/PKG-INFO` & `filmweb-0.7/filmweb.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filmweb
-Version: 0.6
+Version: 0.7
 Summary: Export movie ratings from filmweb.pl
 Author: Piotr Patrzyk
 License: MIT
 Project-URL: Source, https://github.com/ppatrzyk/filmweb
 Keywords: filmweb,movie,crawler,data
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -53,79 +53,78 @@
 4. Skopiuj wartość *Cookie* i podaj ją jako argument do skryptu.
 
 ![Browser Screenshot](browser_screen.jpg)
 
 ### Przykład
 
 ```
-$ filmweb -f all pieca "didomi_token=(...)=="
+$ filmweb -f csv -f json pieca "didomi_token=(...)=="
 INFO:root:Checking args...
-INFO:root:Fetching list of movies...
-100%|██████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 38/38 [00:06<00:00,  6.26it/s]
-INFO:root:Parsing list of movies...
-100%|██████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 38/38 [00:02<00:00, 12.79it/s]
-INFO:root:User pieca has 926 movies...
-INFO:root:Fetching movie details...
-INFO:root:Fetching user ratings [1/3]...
-100%|████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 926/926 [00:39<00:00, 23.49it/s]
-INFO:root:Fetching info about movies [2/3]...
-100%|████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 926/926 [00:43<00:00, 21.22it/s]
-INFO:root:Fetching global rating for movies [3/3]...
-100%|████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 926/926 [00:43<00:00, 21.36it/s]
-INFO:root:Writing data...
-INFO:root:pieca_filmweb_20230121.json written!
-INFO:root:pieca_filmweb_20230121.csv written!
-$ cat pieca_filmweb_20230121.json | jq .[0]
+INFO:root:Fetching list of movies [1/6]...
+100%|██████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 38/38 [00:07<00:00,  4.98it/s]
+INFO:root:Parsing list of movies [2/6]...
+100%|██████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 38/38 [00:02<00:00, 15.47it/s]
+INFO:root:User pieca has 938 movies...
+INFO:root:Fetching user ratings [3/6]...
+100%|████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 938/938 [00:34<00:00, 27.34it/s]
+INFO:root:Fetching info about movies [4/6]...
+100%|████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 938/938 [00:33<00:00, 27.63it/s]
+INFO:root:Fetching global rating for movies [5/6]...
+100%|████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 938/938 [00:35<00:00, 26.57it/s]
+INFO:root:Writing data [6/6]...
+INFO:root:pieca_20230523.json written!
+INFO:root:pieca_20230523.csv written!
+$ cat pieca_20230523.json | jq .[0]
 {
-  "timestamp": 1657484863818,
-  "favorite": false,
-  "user_rating": 8,
-  "global_rating": 7.36859,
-  "global_rating_count": 1579,
-  "original_title": "Tehran Taboo",
-  "pl_title": "Teheran tabu",
-  "year": 2017,
-  "movie_id": "786978",
-  "url": "https://www.filmweb.pl/film/Teheran+tabu-2017-786978"
+  "timestamp": 1579354599456,
+  "favorite": null,
+  "user_rating": 5,
+  "global_rating": 6.03865,
+  "global_rating_count": 414,
+  "original_title": "Ejdeha Vared Mishavad!",
+  "pl_title": "Wejście smoka!",
+  "year": 2016,
+  "movie_id": "757318",
+  "url": "https://www.filmweb.pl/film/Wej%C5%9Bcie+smoka%21-2016-757318",
+  "date": "2020-01-18"
 }
-$ cat pieca_filmweb_20230121.csv | xsv sample 5 | xsv table
-timestamp      favorite  user_rating  global_rating  global_rating_count  original_title  pl_title       year  movie_id  url
-1464302814850  False     4            6.91279        1743                 Pupendo         Pupendo        2003  103930    https://www.filmweb.pl/film/Pupendo-2003-103930
-1581177494926  False     7            6.51905        210                  Dukhtar         Dukhtar        2014  727743    https://www.filmweb.pl/film/Dukhtar-2014-727743
-1601716769499  False     8            7.59777        179                  Shah-re ziba    Piękne miasto  2004  155344    https://www.filmweb.pl/film/Pi%C4%99kne+miasto-2004-155344
-1548505975360  False     8            7.12276        1784                 Geu-mul         W sieci        2016  766555    https://www.filmweb.pl/film/W+sieci-2016-766555
-1638616845248  False     5            6.59127        115166               Ida             Ida            2013  546529    https://www.filmweb.pl/film/Ida-2013-546529
+$ cat pieca_20230523.csv | xsv sample 3 | xsv table
+timestamp      favorite  user_rating  global_rating  global_rating_count  original_title          pl_title                 year  movie_id  url                                                                  date
+1588407481213            9            7.91448        3777                 Werckmeister harmóniák  Harmonie Werckmeistera   2000  117108    https://www.filmweb.pl/film/Harmonie+Werckmeistera-2000-117108       2020-05-02
+1425511804375            4            6.69102        87448                Czas surferów           Czas surferów            2005  137466    https://www.filmweb.pl/film/Czas+surfer%C3%B3w-2005-137466           2015-03-05
+1496177689168            6            7.16478        619                  Kukačka v temném lese   Kukułka w ciemnym lesie  1984  35947     https://www.filmweb.pl/film/Kuku%C5%82ka+w+ciemnym+lesie-1984-35947  2017-05-30             2015-03-05
 ```
 
 ### Wszystkie opcje
 
 ```
 $ filmweb -h
 filmweb
 
 Usage:
-    filmweb [--format=<fileformat>] [--debug] <username> <cookie>
+    filmweb [--format=<fileformat>]... [--debug] <username> <cookie>
 
 Options:
     -h --help                     Show this screen
-    -f --format=<fileformat>      Output file format: json (default), csv, all (writes both)
-    -d --debug                    Debug prints                 Debug prints
+    -f --format=<fileformat>      Output file format: json (default), csv, letterboxd
+    -d --debug                    Debug prints
 ```
 
 ## Dostępne dane:
 
 Kolumna | Opis
 --- | ---
 year | _premiera_
 global\_rating\_count | _ilość ocen filmu_
 global\_rating | _ocena filmweb_
 timestamp | _[czas oceny (unix)](https://pl.wikipedia.org/wiki/Czas_uniksowy)_
+date | _data oceny_ (yyyy-mm-dd)
 user\_rating | _ocena użytkownika_
 favorite | _dodany do ulubionych_
 original\_title | _tytuł oryginalny_
 pl\_title | _tytuł polski_
-movie\_id | _id filmu_
+movie\_id | _id filmu_ (filmweb)
 url | _strona filmu_
 
 ## Znane problemy:
 
 - Eksport tylko ocen filmów, inne (np. seriale) niedostępne,
```

### Comparing `filmweb-0.6/pyproject.toml` & `filmweb-0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "filmweb"
-version = "0.6"
+version = "0.7"
 description = "Export movie ratings from filmweb.pl"
 authors = [ {name = "Piotr Patrzyk"}, ]
 license = {text = "MIT"}
 readme = "README.md"
 requires-python = ">=3.10"
 dynamic = ["dependencies", ]
 keywords = ["filmweb", "movie", "crawler", "data"]
```

