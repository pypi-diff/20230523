# Comparing `tmp/copius_api-1.4.tar.gz` & `tmp/copius_api-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copius_api-1.4.tar", last modified: Wed Nov 17 20:16:35 2021, max compression
+gzip compressed data, was "copius_api-1.4.1.tar", last modified: Tue May 23 16:06:59 2023, max compression
```

## Comparing `copius_api-1.4.tar` & `copius_api-1.4.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2021-11-17 20:16:35.334945 copius_api-1.4/
--rw-rw-rw-   0        0        0     1088 2021-11-17 18:15:40.000000 copius_api-1.4/LICENSE.txt
--rw-rw-rw-   0        0        0        0 2021-11-17 18:52:48.000000 copius_api-1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2524 2021-11-17 20:16:35.335941 copius_api-1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1656 2021-11-17 20:16:15.000000 copius_api-1.4/README.md
-drwxrwxrwx   0        0        0        0 2021-11-17 20:16:35.281089 copius_api-1.4/copius_api/
--rw-rw-rw-   0        0        0        0 2021-11-16 19:00:39.000000 copius_api-1.4/copius_api/__init__.py
--rw-rw-rw-   0        0        0     1470 2021-11-16 19:02:04.000000 copius_api-1.4/copius_api/api.py
-drwxrwxrwx   0        0        0        0 2021-11-17 20:16:35.332950 copius_api-1.4/copius_api.egg-info/
--rw-rw-rw-   0        0        0     2524 2021-11-17 20:16:34.000000 copius_api-1.4/copius_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2021-11-17 20:16:34.000000 copius_api-1.4/copius_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-11-17 20:16:34.000000 copius_api-1.4/copius_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2021-11-17 20:16:34.000000 copius_api-1.4/copius_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2021-11-17 20:16:34.000000 copius_api-1.4/copius_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2021-11-17 20:16:35.338105 copius_api-1.4/setup.cfg
--rw-rw-rw-   0        0        0     1945 2021-11-17 20:16:19.000000 copius_api-1.4/setup.py
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2023-05-23 16:06:59.075521 copius_api-1.4.1/
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     3676 2023-05-23 16:06:59.075521 copius_api-1.4.1/PKG-INFO
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     2003 2023-05-23 15:59:18.000000 copius_api-1.4.1/README.rst
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2023-05-23 16:06:59.075521 copius_api-1.4.1/copius_api/
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)        0 2023-05-23 15:39:49.000000 copius_api-1.4.1/copius_api/__init__.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     1485 2023-05-23 15:41:40.000000 copius_api-1.4.1/copius_api/api.py
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2023-05-23 16:06:59.075521 copius_api-1.4.1/copius_api.egg-info/
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     3676 2023-05-23 16:06:59.000000 copius_api-1.4.1/copius_api.egg-info/PKG-INFO
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)      265 2023-05-23 16:06:59.000000 copius_api-1.4.1/copius_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)        1 2023-05-23 16:06:59.000000 copius_api-1.4.1/copius_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)       48 2023-05-23 16:06:59.000000 copius_api-1.4.1/copius_api.egg-info/requires.txt
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)       17 2023-05-23 16:06:59.000000 copius_api-1.4.1/copius_api.egg-info/top_level.txt
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)       38 2023-05-23 16:06:59.075521 copius_api-1.4.1/setup.cfg
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     1372 2023-05-23 16:06:32.000000 copius_api-1.4.1/setup.py
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2023-05-23 16:06:59.075521 copius_api-1.4.1/tests/
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)        0 2023-05-23 15:39:49.000000 copius_api-1.4.1/tests/__init__.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)      425 2023-05-23 15:39:49.000000 copius_api-1.4.1/tests/test_api.py
```

### Comparing `copius_api-1.4/copius_api/api.py` & `copius_api-1.4.1/copius_api/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,44 @@
-"""a simple API to transcribe some Finno-Ugric, Turkic and the Russian language"""
-
-import requests
-from bs4 import BeautifulSoup
-
-lang_dict = {
-    "Mari (Hill Mari)": "mhr", "Udmurt": "udm", "Komi": "kom",
-    "Erzya": "myv", "Moksha": "mdf", "Mansi": "mns", "Tatar": "tat",
-    "Bashkir": "bak", "Chuvash": "chv", "Russian": "rus"
-}
-
-orth = {"Cyrillic": "c", "Latin": "l", "IPA": "i", "ISO9":"9", "<1917": "3"}
-
-orth_dict = {f"{osrc} to {otgt}" : f"{orth[osrc]}{orth[otgt]}"
-             for osrc in orth for otgt in list(orth)[:-1]
-             if orth[osrc]+orth[otgt] not in ["ii", "99"]}
-
-def transcribe(text, language='udm', which_orth='li'): 
-    """
-    This is an api for https://copius.eu/trtr.php (© 2021 COPIUS)
-    
-    :param text: The text you want to transcribe
-    :type text: str
-    
-    :param language: Abbreviation of the language you want to transcribe from. \ 
-Call lang_dict for a comprehensive list of abbreviations
-    :type language: str
-    
-    :param which_orth: Abbreviation of source and target orthography. \
-Call orth_dict for a comprehensive list of abbreviations
-    :tpye which_orth: str
-    
-    """
-
-    
-    r = requests.post(f'https://copius.eu/trtr.php?lang={language}', data = {'inField':text, 'dir': which_orth})
-    soup = BeautifulSoup(r.text, 'html.parser')
-    for t in soup.find_all("td"):
-        res = t.find("div", class_="trans")
-        if res:
-            return res.text
+"""a simple API to transcribe some Finno-Ugric, Turkic and the Russian language"""
+
+import requests
+from bs4 import BeautifulSoup
+
+lang_dict = {
+    "Mari (Hill Mari)": "mhr", "Udmurt": "udm", "Komi": "kom",
+    "Erzya": "myv", "Moksha": "mdf", "Mansi": "mns", "Tatar": "tat",
+    "Bashkir": "bak", "Chuvash": "chv", "Russian": "rus"
+}
+
+orth = {"Cyrillic": "c", "Latin": "l", "IPA": "i", "ISO9":"9", "<1917": "3"}
+
+orth_dict = {f"{osrc} to {otgt}" : f"{orth[osrc]}{orth[otgt]}"
+             for osrc in orth for otgt in list(orth)[:-1]
+             if orth[osrc]+orth[otgt] not in ["ii", "99"]}
+
+def transcribe(text, language='udm', which_orth='li'):
+    """
+    This is an api for https://copius.eu/trtr.php (© 2021 COPIUS)
+
+    :param text: The text you want to transcribe
+    :type text: str
+
+    :param language: Abbreviation of the language you want to transcribe from.
+                     Call lang_dict for a comprehensive list of abbreviations
+    :type language: str
+
+    :param which_orth: Abbreviation of source and target orthography.
+                       Call orth_dict for a comprehensive list of abbreviations
+    :tpye which_orth: str
+
+    """
+
+
+    r = requests.post(
+            f'https://copius.eu/trtr.php?lang={language}',
+            data={'inField':text, 'dir': which_orth}
+            )
+    soup = BeautifulSoup(r.text, 'html.parser')
+    for t in soup.find_all("td"):
+        res = t.find("div", class_="trans")
+        if res:
+            return res.text
```

### Comparing `copius_api-1.4/copius_api.egg-info/PKG-INFO` & `copius_api-1.4.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,66 +1,94 @@
-Metadata-Version: 2.1
-Name: copius-api
-Version: 1.4
-Summary: Transcription & orthography toolset
-Home-page: https://copius.eu/ortho.php
-Author: Viktor Martinović
-Author-email: viktormartin95@hotmail.com
-License: MIT
-Download-URL: https://github.com/martino-vic/copius_api/archive/refs/tags/v1.1.tar.gz
-Keywords: api,ipa,transcription,copius,Volga-Kama
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Natural Language :: English
-Classifier: Natural Language :: Russian
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# copius_api
-This is a Python-api to the transcription and orthography toolset at https://copius.eu/ortho.php:  
-  
-"This toolset is a loose conglomeration of applications aiming to help you handle various character encodings, orthographies, transcriptions and transliterations you might encounter when working with Uralic languages and other languages of Europe and Northern Asia that use variants of the Latin or Cyrillic alphabet." (Copyright © 2021 COPIUS) 
-  
-How to use:
-
-```
->>> from copius_api import api
->>> api.transcribe("ke̮")
-"kɘ"
-```
-```
->>> from copius_api import api
->>> api.transcribe("lol","kom","lc")
-"лол"
-```
-```
->>> from copius_api import api
->>> api.transcribe("kiki","mns","9c")
-"кики"
-```
-```
->>> from copius_api import api
->>> api.transcribe("буба","mns","c9")
-"buba"
-```
-
-To see the language abbreviations:
-
-```
->>> from copius_api import api
->>> api.lang_dict
-{'Mari (Hill Mari)': 'mhr', 'Udmurt': 'udm', 'Komi': 'kom', 'Erzya': 'myv', 'Moksha': 'mdf', 'Mansi': 'mns', 'Tatar': 'tat', 'Bashkir': 'bak', 'Chuvash': 'chv', 'Russian': 'rus'}
-```
-
-To see the script abbrevations:
-
-```
->>> from copius_api import api
->>> api.orth_dict
-{'Cyrillic to Cyrillic': 'cc', 'Cyrillic to Latin': 'cl', 'Cyrillic to IPA': 'ci', 'Cyrillic to ISO9': 'c9', 'Latin to Cyrillic': 'lc', 'Latin to Latin': 'll', 'Latin to IPA': 'li', 'Latin to ISO9': 'l9', 'IPA to Cyrillic': 'ic', 'IPA to Latin': 'il', 'IPA to ISO9': 'i9', 'ISO9 to Cyrillic': '9c', 'ISO9 to Latin': '9l', 'ISO9 to IPA': '9i', '<1917 to Cyrillic': '3c', '<1917 to Latin': '3l', '<1917 to IPA': '3i', '<1917 to ISO9': '39'}
-```
-
+Metadata-Version: 2.1
+Name: copius_api
+Version: 1.4.1
+Summary: Transcription & orthography toolset
+Home-page: https://github.com/martino-vic/copius_api
+Author: Viktor Martinović
+Author-email: viktoringermany@gmail.com
+License: MIT
+Download-URL: https://github.com/martino-vic/copius_api/archive/refs/tags/v1.4.1.tar.gz
+Project-URL: continuous integration, https://app.circleci.com/pipelines/github/martino-vic/copius_api?branch=master
+Description: |DOI| |CircleCI|
+        
+        copius_api
+        ==========
+        
+        This is a Python-api to the transcription and orthography toolset at
+        https://copius.eu/ortho.php:
+        
+        “This toolset is a loose conglomeration of applications aiming to help
+        you handle various character encodings, orthographies, transcriptions
+        and transliterations you might encounter when working with Uralic
+        languages and other languages of Europe and Northern Asia that use
+        variants of the Latin or Cyrillic alphabet.” (Copyright © 2021 COPIUS)
+        
+        How to install:
+        
+        ::
+        
+           $ pip install copius_api
+        
+        How to use:
+        
+        ::
+        
+           >>> from copius_api import api
+           >>> api.transcribe("ke̮")
+           "kɘ"
+        
+        ::
+        
+           >>> from copius_api import api
+           >>> api.transcribe("lol","kom","lc")
+           "лол"
+        
+        ::
+        
+           >>> from copius_api import api
+           >>> api.transcribe("kiki","mns","9c")
+           "кики"
+        
+        ::
+        
+           >>> from copius_api import api
+           >>> api.transcribe("буба","mns","c9")
+           "buba"
+        
+        To see the language abbreviations:
+        
+        ::
+        
+           >>> from copius_api import api
+           >>> api.lang_dict
+           {'Mari (Hill Mari)': 'mhr', 'Udmurt': 'udm', 'Komi': 'kom', 'Erzya': 'myv', 'Moksha': 'mdf', 'Mansi': 'mns', 'Tatar': 'tat', 'Bashkir': 'bak', 'Chuvash': 'chv', 'Russian': 'rus'}
+        
+        To see the script abbrevations:
+        
+        ::
+        
+           >>> from copius_api import api
+           >>> api.orth_dict
+           {'Cyrillic to Cyrillic': 'cc', 'Cyrillic to Latin': 'cl', 'Cyrillic to IPA': 'ci', 'Cyrillic to ISO9': 'c9', 'Latin to Cyrillic': 'lc', 'Latin to Latin': 'll', 'Latin to IPA': 'li', 'Latin to ISO9': 'l9', 'IPA to Cyrillic': 'ic', 'IPA to Latin': 'il', 'IPA to ISO9': 'i9', 'ISO9 to Cyrillic': '9c', 'ISO9 to Latin': '9l', 'ISO9 to IPA': '9i', '<1917 to Cyrillic': '3c', '<1917 to Latin': '3l', '<1917 to IPA': '3i', '<1917 to ISO9': '39'}
+        
+        .. |DOI| image:: https://zenodo.org/badge/428920599.svg
+           :target: https://zenodo.org/badge/latestdoi/428920599
+        .. |CircleCI| image:: https://circleci.com/gh/martino-vic/copius_api/tree/master.svg?style=svg
+           :target: https://circleci.com/gh/martino-vic/copius_api/tree/master
+        
+Keywords: linguistics,transcription
+Platform: Linux
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Text Processing :: Linguistic
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
+Provides-Extra: dev
+Provides-Extra: test
```

