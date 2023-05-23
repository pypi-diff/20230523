# Comparing `tmp/voliboli_pdf_scraper-1.6.tar.gz` & `tmp/voliboli_pdf_scraper-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voliboli_pdf_scraper-1.6.tar", last modified: Mon May 22 09:34:49 2023, max compression
+gzip compressed data, was "voliboli_pdf_scraper-1.7.tar", last modified: Tue May 23 10:51:27 2023, max compression
```

## Comparing `voliboli_pdf_scraper-1.6.tar` & `voliboli_pdf_scraper-1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 teodorpodobnik  (1000) teodorpodobnik  (1000)        0 2023-05-22 09:34:49.898289 voliboli_pdf_scraper-1.6/
--rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)     1065 2023-05-21 15:15:55.000000 voliboli_pdf_scraper-1.6/LICENSE.md
--rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)     1219 2023-05-22 09:34:49.898289 voliboli_pdf_scraper-1.6/PKG-INFO
--rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)      831 2023-05-21 15:15:55.000000 voliboli_pdf_scraper-1.6/README.md
--rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)       84 2023-05-21 15:15:55.000000 voliboli_pdf_scraper-1.6/pyproject.toml
--rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)      496 2023-05-22 09:34:49.898289 voliboli_pdf_scraper-1.6/setup.cfg
--rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)      340 2023-05-22 09:34:12.000000 voliboli_pdf_scraper-1.6/setup.py
-drwxrwxr-x   0 teodorpodobnik  (1000) teodorpodobnik  (1000)        0 2023-05-22 09:34:49.898289 voliboli_pdf_scraper-1.6/src/
-drwxrwxr-x   0 teodorpodobnik  (1000) teodorpodobnik  (1000)        0 2023-05-22 09:34:49.898289 voliboli_pdf_scraper-1.6/src/voliboli_pdf_scraper/
--rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)        0 2023-05-21 15:15:55.000000 voliboli_pdf_scraper-1.6/src/voliboli_pdf_scraper/__init__.py
--rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)     9885 2023-05-22 09:33:36.000000 voliboli_pdf_scraper-1.6/src/voliboli_pdf_scraper/constants.py
--rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)     4496 2023-05-21 15:15:55.000000 voliboli_pdf_scraper-1.6/src/voliboli_pdf_scraper/main.py
-drwxrwxr-x   0 teodorpodobnik  (1000) teodorpodobnik  (1000)        0 2023-05-22 09:34:49.898289 voliboli_pdf_scraper-1.6/src/voliboli_pdf_scraper.egg-info/
--rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)     1219 2023-05-22 09:34:49.000000 voliboli_pdf_scraper-1.6/src/voliboli_pdf_scraper.egg-info/PKG-INFO
--rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)      447 2023-05-22 09:34:49.000000 voliboli_pdf_scraper-1.6/src/voliboli_pdf_scraper.egg-info/SOURCES.txt
--rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)        1 2023-05-22 09:34:49.000000 voliboli_pdf_scraper-1.6/src/voliboli_pdf_scraper.egg-info/dependency_links.txt
--rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)       16 2023-05-22 09:34:49.000000 voliboli_pdf_scraper-1.6/src/voliboli_pdf_scraper.egg-info/requires.txt
--rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)       21 2023-05-22 09:34:49.000000 voliboli_pdf_scraper-1.6/src/voliboli_pdf_scraper.egg-info/top_level.txt
-drwxrwxr-x   0 teodorpodobnik  (1000) teodorpodobnik  (1000)        0 2023-05-22 09:34:49.898289 voliboli_pdf_scraper-1.6/tests/
--rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)      517 2023-05-21 15:15:55.000000 voliboli_pdf_scraper-1.6/tests/test_main.py
--rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)     2877 2023-05-21 15:15:55.000000 voliboli_pdf_scraper-1.6/tests/test_with_db_main.py
+drwxrwxr-x   0 teodorpodobnik  (1000) teodorpodobnik  (1000)        0 2023-05-23 10:51:27.740346 voliboli_pdf_scraper-1.7/
+-rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)     1065 2023-05-21 15:15:55.000000 voliboli_pdf_scraper-1.7/LICENSE.md
+-rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)     1219 2023-05-23 10:51:27.740346 voliboli_pdf_scraper-1.7/PKG-INFO
+-rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)      831 2023-05-21 15:15:55.000000 voliboli_pdf_scraper-1.7/README.md
+-rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)       84 2023-05-21 15:15:55.000000 voliboli_pdf_scraper-1.7/pyproject.toml
+-rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)      496 2023-05-23 10:51:27.740346 voliboli_pdf_scraper-1.7/setup.cfg
+-rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)      340 2023-05-23 10:51:11.000000 voliboli_pdf_scraper-1.7/setup.py
+drwxrwxr-x   0 teodorpodobnik  (1000) teodorpodobnik  (1000)        0 2023-05-23 10:51:27.736346 voliboli_pdf_scraper-1.7/src/
+drwxrwxr-x   0 teodorpodobnik  (1000) teodorpodobnik  (1000)        0 2023-05-23 10:51:27.736346 voliboli_pdf_scraper-1.7/src/voliboli_pdf_scraper/
+-rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)        0 2023-05-21 15:15:55.000000 voliboli_pdf_scraper-1.7/src/voliboli_pdf_scraper/__init__.py
+-rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)    10049 2023-05-23 10:49:03.000000 voliboli_pdf_scraper-1.7/src/voliboli_pdf_scraper/constants.py
+-rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)     4496 2023-05-21 15:15:55.000000 voliboli_pdf_scraper-1.7/src/voliboli_pdf_scraper/main.py
+drwxrwxr-x   0 teodorpodobnik  (1000) teodorpodobnik  (1000)        0 2023-05-23 10:51:27.740346 voliboli_pdf_scraper-1.7/src/voliboli_pdf_scraper.egg-info/
+-rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)     1219 2023-05-23 10:51:27.000000 voliboli_pdf_scraper-1.7/src/voliboli_pdf_scraper.egg-info/PKG-INFO
+-rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)      447 2023-05-23 10:51:27.000000 voliboli_pdf_scraper-1.7/src/voliboli_pdf_scraper.egg-info/SOURCES.txt
+-rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)        1 2023-05-23 10:51:27.000000 voliboli_pdf_scraper-1.7/src/voliboli_pdf_scraper.egg-info/dependency_links.txt
+-rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)       16 2023-05-23 10:51:27.000000 voliboli_pdf_scraper-1.7/src/voliboli_pdf_scraper.egg-info/requires.txt
+-rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)       21 2023-05-23 10:51:27.000000 voliboli_pdf_scraper-1.7/src/voliboli_pdf_scraper.egg-info/top_level.txt
+drwxrwxr-x   0 teodorpodobnik  (1000) teodorpodobnik  (1000)        0 2023-05-23 10:51:27.740346 voliboli_pdf_scraper-1.7/tests/
+-rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)      517 2023-05-21 15:15:55.000000 voliboli_pdf_scraper-1.7/tests/test_main.py
+-rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)     2877 2023-05-23 09:24:39.000000 voliboli_pdf_scraper-1.7/tests/test_with_db_main.py
```

### Comparing `voliboli_pdf_scraper-1.6/LICENSE.md` & `voliboli_pdf_scraper-1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `voliboli_pdf_scraper-1.6/PKG-INFO` & `voliboli_pdf_scraper-1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voliboli_pdf_scraper
-Version: 1.6
+Version: 1.7
 Summary: Voliboli PDF Scraper
 Author: Teodor Janez Podobnik
 Author-email: teo.podobnik1234@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `voliboli_pdf_scraper-1.6/README.md` & `voliboli_pdf_scraper-1.7/README.md`

 * *Files identical despite different names*

### Comparing `voliboli_pdf_scraper-1.6/src/voliboli_pdf_scraper/constants.py` & `voliboli_pdf_scraper-1.7/src/voliboli_pdf_scraper/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,37 +70,40 @@
                        "11": "Bojić Slobodan",
                        "12": "Okroglič Grega",
                        "13": "Kovačič Aleks",
                        "14": "Ikhbayri Mohamed",
                        "15": "Vrtovec Matic",
                        "17": "Maksimović Marko"},
     "ACH Volley Ljubljana": {"1": "Mejal Primož",
+                             "4": "Satler Rok",
                              "5": "Šket Alen",
                              "8": "Mašulović Nemanja",
                              "9": "Todorović Vuk",
                              "10": "Bošnjak Črtomir",
                              "11": "Koncilja Danijel",
                              "12": "Šestan Filip",
                              "13": "Kovačič Jani",
                              "14": "Gjorgiev Nikola",
                              "17": "Videčnik Matic",
                              "18": "Kök Matej",
                              "19": "Šen Klemen"},
     "Črnuče": {"1": "Kržič Jošt",
                "2": "Mihelčič Gregor",
+               "4": "Elikan Gaj",
                "5": "Prevorčnik Jaka",
                "6": "Karadža Pevc Matevž",
                "7": "Gornik Aljaž",
                "8": "Verdinek Jožef",
                "9": "Rojnik Matic",
                "10": "Oman Jurij",
                "11": "Sešek Jaka",
                "13": "Marovt Luka",
                "15": "Jančič Jan Karl",
                "16": "Valenčič Martin",
+               "17": "Vilar Blaž",
                "19": "Ramšak Vid",
                "33": "Česnovar Matic"},
     "Merkur Maribor": {"2": "Jevšnik Jaka",
                        "3": "Vodušek Timotej",
                        "4": "Pernuš Gregor",
                        "5": "Adžović Sani",
                        "6": "McConnell Connor",
@@ -108,14 +111,15 @@
                        "9": "Kumer Žiga",
                        "10": "Kržič Janž Janez",
                        "11": "Donik Žiga",
                        "12": "Leva Filip",
                        "13": "Fink Miha",
                        "14": "Najdič Nejc",
                        "16": "Iršič Jaka",
+                       "21": "Toplišek Maj",
                        "42": "Peruničić Nemanja"},
     "Panvita Pomgrad": {"1": "Rajnar Urban",
                         "5": "Šormaz Nenad",
                         "6": "Avšič Tine",
                         "7": "Drvarič Urban",
                         "8": "Vrabl Tin",
                         "9": "Suhadolnik Vid",
```

### Comparing `voliboli_pdf_scraper-1.6/src/voliboli_pdf_scraper/main.py` & `voliboli_pdf_scraper-1.7/src/voliboli_pdf_scraper/main.py`

 * *Files identical despite different names*

### Comparing `voliboli_pdf_scraper-1.6/src/voliboli_pdf_scraper.egg-info/PKG-INFO` & `voliboli_pdf_scraper-1.7/src/voliboli_pdf_scraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voliboli-pdf-scraper
-Version: 1.6
+Version: 1.7
 Summary: Voliboli PDF Scraper
 Author: Teodor Janez Podobnik
 Author-email: teo.podobnik1234@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `voliboli_pdf_scraper-1.6/tests/test_main.py` & `voliboli_pdf_scraper-1.7/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `voliboli_pdf_scraper-1.6/tests/test_with_db_main.py` & `voliboli_pdf_scraper-1.7/tests/test_with_db_main.py`

 * *Files identical despite different names*

