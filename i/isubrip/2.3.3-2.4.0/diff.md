# Comparing `tmp/isubrip-2.3.3.tar.gz` & `tmp/isubrip-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isubrip-2.3.3.tar", last modified: Sun Oct  9 10:29:07 2022, max compression
+gzip compressed data, was "isubrip-2.4.0.tar", last modified: Tue May 23 20:01:56 2023, max compression
```

## Comparing `isubrip-2.3.3.tar` & `isubrip-2.4.0.tar`

### file list

```diff
@@ -1,29 +1,33 @@
-drwxrwxrwx   0        0        0        0 2022-10-09 10:29:07.584273 isubrip-2.3.3/
--rw-rw-rw-   0        0        0     1093 2022-01-28 09:13:22.000000 isubrip-2.3.3/LICENSE
--rw-rw-rw-   0        0        0     3480 2022-10-09 10:29:07.583272 isubrip-2.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     2505 2022-10-09 10:14:29.000000 isubrip-2.3.3/README.md
-drwxrwxrwx   0        0        0        0 2022-10-09 10:29:07.535783 isubrip-2.3.3/isubrip/
--rw-rw-rw-   0        0        0       23 2022-10-09 09:35:20.000000 isubrip-2.3.3/isubrip/__init__.py
--rw-rw-rw-   0        0        0     9196 2022-10-09 10:27:06.000000 isubrip-2.3.3/isubrip/__main__.py
--rw-rw-rw-   0        0        0     5613 2022-10-07 21:52:51.000000 isubrip-2.3.3/isubrip/config.py
--rw-rw-rw-   0        0        0     2842 2022-10-08 10:41:01.000000 isubrip-2.3.3/isubrip/constants.py
--rw-rw-rw-   0        0        0      463 2022-10-07 21:52:51.000000 isubrip-2.3.3/isubrip/enums.py
--rw-rw-rw-   0        0        0      642 2022-10-07 21:52:51.000000 isubrip-2.3.3/isubrip/exceptions.py
--rw-rw-rw-   0        0        0      800 2022-10-08 09:49:47.000000 isubrip-2.3.3/isubrip/namedtuples.py
--rw-rw-rw-   0        0        0     3910 2022-10-08 10:41:01.000000 isubrip-2.3.3/isubrip/playlist_downloader.py
-drwxrwxrwx   0        0        0        0 2022-10-09 10:29:07.581272 isubrip-2.3.3/isubrip/resources/
--rw-rw-rw-   0        0        0     3867 2022-08-18 19:10:44.000000 isubrip-2.3.3/isubrip/resources/atv_storefronts.json
--rw-rw-rw-   0        0        0      582 2022-10-07 21:52:51.000000 isubrip-2.3.3/isubrip/resources/default_config.toml
--rw-rw-rw-   0        0        0    14127 2022-10-08 09:49:47.000000 isubrip-2.3.3/isubrip/scraper.py
--rw-rw-rw-   0        0        0     7375 2022-06-23 19:52:39.000000 isubrip-2.3.3/isubrip/subtitles.py
--rw-rw-rw-   0        0        0     5835 2022-10-09 00:13:00.000000 isubrip-2.3.3/isubrip/utils.py
--rw-rw-rw-   0        0        0     4570 2022-06-23 19:52:39.000000 isubrip-2.3.3/isubrip/webvtt.py
-drwxrwxrwx   0        0        0        0 2022-10-09 10:29:07.549846 isubrip-2.3.3/isubrip.egg-info/
--rw-rw-rw-   0        0        0     3480 2022-10-09 10:29:07.000000 isubrip-2.3.3/isubrip.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      538 2022-10-09 10:29:07.000000 isubrip-2.3.3/isubrip.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-09 10:29:07.000000 isubrip-2.3.3/isubrip.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2022-10-09 10:29:07.000000 isubrip-2.3.3/isubrip.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       58 2022-10-09 10:29:07.000000 isubrip-2.3.3/isubrip.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-10-09 10:29:07.000000 isubrip-2.3.3/isubrip.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-10-09 10:29:07.584273 isubrip-2.3.3/setup.cfg
--rw-rw-rw-   0        0        0     2139 2022-08-06 19:15:15.000000 isubrip-2.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 20:01:56.316877 isubrip-2.4.0/
+-rw-rw-rw-   0        0        0     1093 2022-01-28 09:13:22.000000 isubrip-2.4.0/LICENSE
+-rw-rw-rw-   0        0        0     3536 2023-05-23 20:01:56.315875 isubrip-2.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2411 2023-05-23 20:01:27.000000 isubrip-2.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 20:01:56.303876 isubrip-2.4.0/isubrip/
+-rw-rw-rw-   0        0        0       23 2023-05-23 20:01:27.000000 isubrip-2.4.0/isubrip/__init__.py
+-rw-rw-rw-   0        0        0    12753 2023-05-23 20:01:27.000000 isubrip-2.4.0/isubrip/__main__.py
+-rw-rw-rw-   0        0        0    11798 2023-05-23 20:01:27.000000 isubrip-2.4.0/isubrip/config.py
+-rw-rw-rw-   0        0        0     2178 2023-05-23 20:01:27.000000 isubrip-2.4.0/isubrip/constants.py
+-rw-rw-rw-   0        0        0     6053 2023-05-23 20:01:27.000000 isubrip-2.4.0/isubrip/data_structures.py
+drwxrwxrwx   0        0        0        0 2023-05-23 20:01:56.309880 isubrip-2.4.0/isubrip/resources/
+-rw-rw-rw-   0        0        0      595 2023-05-23 20:01:27.000000 isubrip-2.4.0/isubrip/resources/default_config.toml
+drwxrwxrwx   0        0        0        0 2023-05-23 20:01:56.312875 isubrip-2.4.0/isubrip/scrapers/
+-rw-rw-rw-   0        0        0        0 2023-05-23 20:01:27.000000 isubrip-2.4.0/isubrip/scrapers/__init__.py
+-rw-rw-rw-   0        0        0    15845 2023-05-23 20:01:27.000000 isubrip-2.4.0/isubrip/scrapers/appletv_scraper.py
+-rw-rw-rw-   0        0        0     4375 2023-05-23 20:01:27.000000 isubrip-2.4.0/isubrip/scrapers/itunes_scraper.py
+-rw-rw-rw-   0        0        0    22230 2023-05-23 20:01:27.000000 isubrip-2.4.0/isubrip/scrapers/scraper.py
+drwxrwxrwx   0        0        0        0 2023-05-23 20:01:56.315875 isubrip-2.4.0/isubrip/subtitle_formats/
+-rw-rw-rw-   0        0        0        0 2023-05-23 20:01:27.000000 isubrip-2.4.0/isubrip/subtitle_formats/__init__.py
+-rw-rw-rw-   0        0        0     1383 2023-05-23 20:01:27.000000 isubrip-2.4.0/isubrip/subtitle_formats/subrip.py
+-rw-rw-rw-   0        0        0     7909 2023-05-23 20:01:27.000000 isubrip-2.4.0/isubrip/subtitle_formats/subtitles.py
+-rw-rw-rw-   0        0        0     9220 2023-05-23 20:01:27.000000 isubrip-2.4.0/isubrip/subtitle_formats/webvtt.py
+-rw-rw-rw-   0        0        0    13341 2023-05-23 20:01:27.000000 isubrip-2.4.0/isubrip/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-23 20:01:56.308879 isubrip-2.4.0/isubrip.egg-info/
+-rw-rw-rw-   0        0        0     3536 2023-05-23 20:01:56.000000 isubrip-2.4.0/isubrip.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      663 2023-05-23 20:01:56.000000 isubrip-2.4.0/isubrip.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 20:01:56.000000 isubrip-2.4.0/isubrip.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-23 20:01:56.000000 isubrip-2.4.0/isubrip.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       38 2023-05-23 20:01:56.000000 isubrip-2.4.0/isubrip.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-23 20:01:56.000000 isubrip-2.4.0/isubrip.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       83 2023-05-23 20:01:27.000000 isubrip-2.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-23 20:01:56.316877 isubrip-2.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     2815 2023-05-23 20:01:27.000000 isubrip-2.4.0/setup.py
```

### Comparing `isubrip-2.3.3/LICENSE` & `isubrip-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `isubrip-2.3.3/PKG-INFO` & `isubrip-2.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
 Name: isubrip
-Version: 2.3.3
+Version: 2.4.0
 Summary: A Python package for scraping and downloading subtitles from iTunes movie pages.
 Home-page: https://github.com/MichaelYochpaz/iSubRip
 Author: Michael Yochpaz
 License: MIT
 Project-URL: Bug Reports, https://github.com/MichaelYochpaz/iSubRip/issues
 Project-URL: Source, https://github.com/MichaelYochpaz/iSubRip
-Keywords: iTunes,movies,subtitles,scrape,scraper,download,m3u8
+Keywords: iTunes,AppleTV,movies,subtitles,scrape,scraper,download,m3u8
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # iSubRip
-A Python package for scraping and downloading subtitles from iTunes movie pages.  
-Latest version: 2.3.3 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))  
+A Python package for scraping and downloading subtitles from AppleTV / iTunes movie pages.  
+Latest version: 2.4.0 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))  
 
 <br/>
   
 [![PyPI - Version](https://img.shields.io/pypi/v/isubrip)](https://python.org/pypi/isubrip)
 [![PyPI - Monthly Downloads](https://pepy.tech/badge/isubrip/month)](https://python.org/pypi/isubrip)
 [![PyPI - Total Downloads](https://pepy.tech/badge/isubrip)](https://python.org/pypi/isubrip)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/isubrip)](https://python.org/pypi/isubrip)
@@ -37,15 +40,15 @@
 
 <p align="center">
   <a href="#"><img src="https://user-images.githubusercontent.com/8832013/194750946-8b4d4d4e-0230-4653-bede-3ec191df161b.gif" width="800"></a>
 </p>
 
 
 ##  Requirements
-* Python 3.7+
+* Python 3.8+
 
 ##  Installation
 ### PyPI (Recommended)
 ```
 python3 -m pip install isubrip
 ```
 
@@ -56,36 +59,33 @@
 
 ## Usage
 ```
 isubrip <iTunes movie URL> [iTunes movie URL...]
 ```  
 
 ## Configuration
-It's possible to configure different options and enable / disable different features using a [TOML](https://toml.io) config file.   
-A config file will be looked for in one of the following paths according to OS: 
+It's possible to configure different options and features by creating a [TOML](https://toml.io) config file.   
+A config file will be looked for in one of the following paths (according to OS): 
 
 **Windows**: `%USERPROFILE%\.isubrip\config.toml`  
 **Linux / macOS**: `$HOME/.isubrip/config.toml`  
 
 ### Examples:
 **Windows**: `C:\Users\Michael\.isubrip\config.toml`  
 **Linux**: `/home/Michael/.isubrip/config.toml`  
 **macOS**: `/Users/Michael/.isubrip/config.toml`  
 
 ---
 
 ### Example Config:
 ```toml
 [downloads]
-folder = "C:\\iTunes-Subtitles"
-format = "srt"
-languages = ["en-US"]
+folder = "C:\\Subtitles\\iTunes"
+languages = ["en-US", "fr-FR", "he"]
 zip = false
 
 [subtitles]
+convert-to-srt = true
 fix-rtl = true
 ```
 
 A complete config with all the available options and explanations for each configuration can be found [here](https://github.com/MichaelYochpaz/iSubRip/blob/main/config.toml)
-
-### Notes
-* All settings are optional. Not specifying a setting will result in using the default value.
```

#### html2text {}

```diff
@@ -1,46 +1,46 @@
-Metadata-Version: 2.1 Name: isubrip Version: 2.3.3 Summary: A Python package
+Metadata-Version: 2.1 Name: isubrip Version: 2.4.0 Summary: A Python package
 for scraping and downloading subtitles from iTunes movie pages. Home-page:
 https://github.com/MichaelYochpaz/iSubRip Author: Michael Yochpaz License: MIT
 Project-URL: Bug Reports, https://github.com/MichaelYochpaz/iSubRip/issues
 Project-URL: Source, https://github.com/MichaelYochpaz/iSubRip Keywords:
-iTunes,movies,subtitles,scrape,scraper,download,m3u8 Classifier: Development
-Status :: 5 - Production/Stable Classifier: Intended Audience :: End Users/
-Desktop Classifier: Intended Audience :: Developers Classifier: Topic ::
-Utilities Classifier: License :: OSI Approved :: MIT License Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Requires-Python: >=3.7 Description-
-Content-Type: text/markdown License-File: LICENSE # iSubRip A Python package
-for scraping and downloading subtitles from iTunes movie pages. Latest version:
-2.3.3 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/
-CHANGELOG.md))
+iTunes,AppleTV,movies,subtitles,scrape,scraper,download,m3u8 Classifier:
+Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
+End Users/Desktop Classifier: Intended Audience :: Developers Classifier:
+Operating System :: Microsoft :: Windows Classifier: Operating System :: MacOS
+Classifier: Operating System :: POSIX :: Linux Classifier: Topic :: Utilities
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Requires-Python: >=3.8 Description-Content-Type:
+text/markdown License-File: LICENSE # iSubRip A Python package for scraping and
+downloading subtitles from AppleTV / iTunes movie pages. Latest version: 2.4.0
+([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))
+
 [![PyPI - Version](https://img.shields.io/pypi/v/isubrip)](https://python.org/
 pypi/isubrip) [![PyPI - Monthly Downloads](https://pepy.tech/badge/isubrip/
 month)](https://python.org/pypi/isubrip) [![PyPI - Total Downloads](https://
 pepy.tech/badge/isubrip)](https://python.org/pypi/isubrip) [![PyPI - Python
 Version](https://img.shields.io/pypi/pyversions/isubrip)](https://python.org/
 pypi/isubrip) [![GitHub - License](https://img.shields.io/github/license/
 MichaelYochpaz/iSubRip)](https://github.com/MichaelYochpaz/iSubRip/blob/main/
 LICENSE) [![GitHub - issues](https://img.shields.io/github/issues/
 MichaelYochpaz/iSubRip)](https://github.com/MichaelYochpaz/iSubRip/issues) [!
 [GitHub - Repo stars](https://img.shields.io/github/stars/MichaelYochpaz/
 iSubRip.svg?color=yellow)](https://github.com/MichaelYochpaz/iSubRip)
   [https://user-images.githubusercontent.com/8832013/194750946-8b4d4d4e-0230-
                           4653-bede-3ec191df161b.gif]
-## Requirements * Python 3.7+ ## Installation ### PyPI (Recommended) ```
+## Requirements * Python 3.8+ ## Installation ### PyPI (Recommended) ```
 python3 -m pip install isubrip ``` ### Git Source Code ``` python3 -m pip
 install -e git+https://github.com/MichaelYochpaz/iSubRip.git#egg=isubrip ``` ##
 Usage ``` isubrip  [iTunes movie URL...] ``` ## Configuration It's possible to
-configure different options and enable / disable different features using a
-[TOML](https://toml.io) config file. A config file will be looked for in one of
-the following paths according to OS: **Windows**:
-`%USERPROFILE%\.isubrip\config.toml` **Linux / macOS**: `$HOME/.isubrip/
-config.toml` ### Examples: **Windows**: `C:\Users\Michael\.isubrip\config.toml`
-**Linux**: `/home/Michael/.isubrip/config.toml` **macOS**: `/Users/
-Michael/.isubrip/config.toml` --- ### Example Config: ```toml [downloads]
-folder = "C:\\iTunes-Subtitles" format = "srt" languages = ["en-US"] zip =
-false [subtitles] fix-rtl = true ``` A complete config with all the available
-options and explanations for each configuration can be found [here](https://
-github.com/MichaelYochpaz/iSubRip/blob/main/config.toml) ### Notes * All
-settings are optional. Not specifying a setting will result in using the
-default value.
+configure different options and features by creating a [TOML](https://toml.io)
+config file. A config file will be looked for in one of the following paths
+(according to OS): **Windows**: `%USERPROFILE%\.isubrip\config.toml` **Linux /
+macOS**: `$HOME/.isubrip/config.toml` ### Examples: **Windows**: `C:
+\Users\Michael\.isubrip\config.toml` **Linux**: `/home/Michael/.isubrip/
+config.toml` **macOS**: `/Users/Michael/.isubrip/config.toml` --- ### Example
+Config: ```toml [downloads] folder = "C:\\Subtitles\\iTunes" languages = ["en-
+US", "fr-FR", "he"] zip = false [subtitles] convert-to-srt = true fix-rtl =
+true ``` A complete config with all the available options and explanations for
+each configuration can be found [here](https://github.com/MichaelYochpaz/
+iSubRip/blob/main/config.toml)
```

### Comparing `isubrip-2.3.3/README.md` & `isubrip-2.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # iSubRip
-A Python package for scraping and downloading subtitles from iTunes movie pages.  
-Latest version: 2.3.3 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))  
+A Python package for scraping and downloading subtitles from AppleTV / iTunes movie pages.  
+Latest version: 2.4.0 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))  
 
 <br/>
   
 [![PyPI - Version](https://img.shields.io/pypi/v/isubrip)](https://python.org/pypi/isubrip)
 [![PyPI - Monthly Downloads](https://pepy.tech/badge/isubrip/month)](https://python.org/pypi/isubrip)
 [![PyPI - Total Downloads](https://pepy.tech/badge/isubrip)](https://python.org/pypi/isubrip)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/isubrip)](https://python.org/pypi/isubrip)
@@ -14,15 +14,15 @@
 
 <p align="center">
   <a href="#"><img src="https://user-images.githubusercontent.com/8832013/194750946-8b4d4d4e-0230-4653-bede-3ec191df161b.gif" width="800"></a>
 </p>
 
 
 ##  Requirements
-* Python 3.7+
+* Python 3.8+
 
 ##  Installation
 ### PyPI (Recommended)
 ```
 python3 -m pip install isubrip
 ```
 
@@ -33,36 +33,33 @@
 
 ## Usage
 ```
 isubrip <iTunes movie URL> [iTunes movie URL...]
 ```  
 
 ## Configuration
-It's possible to configure different options and enable / disable different features using a [TOML](https://toml.io) config file.   
-A config file will be looked for in one of the following paths according to OS: 
+It's possible to configure different options and features by creating a [TOML](https://toml.io) config file.   
+A config file will be looked for in one of the following paths (according to OS): 
 
 **Windows**: `%USERPROFILE%\.isubrip\config.toml`  
 **Linux / macOS**: `$HOME/.isubrip/config.toml`  
 
 ### Examples:
 **Windows**: `C:\Users\Michael\.isubrip\config.toml`  
 **Linux**: `/home/Michael/.isubrip/config.toml`  
 **macOS**: `/Users/Michael/.isubrip/config.toml`  
 
 ---
 
 ### Example Config:
 ```toml
 [downloads]
-folder = "C:\\iTunes-Subtitles"
-format = "srt"
-languages = ["en-US"]
+folder = "C:\\Subtitles\\iTunes"
+languages = ["en-US", "fr-FR", "he"]
 zip = false
 
 [subtitles]
+convert-to-srt = true
 fix-rtl = true
 ```
 
 A complete config with all the available options and explanations for each configuration can be found [here](https://github.com/MichaelYochpaz/iSubRip/blob/main/config.toml)
-
-### Notes
-* All settings are optional. Not specifying a setting will result in using the default value.
```

#### html2text {}

```diff
@@ -1,33 +1,31 @@
-# iSubRip A Python package for scraping and downloading subtitles from iTunes
-movie pages. Latest version: 2.3.3 ([changelog](https://github.com/
+# iSubRip A Python package for scraping and downloading subtitles from AppleTV
+/ iTunes movie pages. Latest version: 2.4.0 ([changelog](https://github.com/
 MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))
 [![PyPI - Version](https://img.shields.io/pypi/v/isubrip)](https://python.org/
 pypi/isubrip) [![PyPI - Monthly Downloads](https://pepy.tech/badge/isubrip/
 month)](https://python.org/pypi/isubrip) [![PyPI - Total Downloads](https://
 pepy.tech/badge/isubrip)](https://python.org/pypi/isubrip) [![PyPI - Python
 Version](https://img.shields.io/pypi/pyversions/isubrip)](https://python.org/
 pypi/isubrip) [![GitHub - License](https://img.shields.io/github/license/
 MichaelYochpaz/iSubRip)](https://github.com/MichaelYochpaz/iSubRip/blob/main/
 LICENSE) [![GitHub - issues](https://img.shields.io/github/issues/
 MichaelYochpaz/iSubRip)](https://github.com/MichaelYochpaz/iSubRip/issues) [!
 [GitHub - Repo stars](https://img.shields.io/github/stars/MichaelYochpaz/
 iSubRip.svg?color=yellow)](https://github.com/MichaelYochpaz/iSubRip)
   [https://user-images.githubusercontent.com/8832013/194750946-8b4d4d4e-0230-
                           4653-bede-3ec191df161b.gif]
-## Requirements * Python 3.7+ ## Installation ### PyPI (Recommended) ```
+## Requirements * Python 3.8+ ## Installation ### PyPI (Recommended) ```
 python3 -m pip install isubrip ``` ### Git Source Code ``` python3 -m pip
 install -e git+https://github.com/MichaelYochpaz/iSubRip.git#egg=isubrip ``` ##
 Usage ``` isubrip  [iTunes movie URL...] ``` ## Configuration It's possible to
-configure different options and enable / disable different features using a
-[TOML](https://toml.io) config file. A config file will be looked for in one of
-the following paths according to OS: **Windows**:
-`%USERPROFILE%\.isubrip\config.toml` **Linux / macOS**: `$HOME/.isubrip/
-config.toml` ### Examples: **Windows**: `C:\Users\Michael\.isubrip\config.toml`
-**Linux**: `/home/Michael/.isubrip/config.toml` **macOS**: `/Users/
-Michael/.isubrip/config.toml` --- ### Example Config: ```toml [downloads]
-folder = "C:\\iTunes-Subtitles" format = "srt" languages = ["en-US"] zip =
-false [subtitles] fix-rtl = true ``` A complete config with all the available
-options and explanations for each configuration can be found [here](https://
-github.com/MichaelYochpaz/iSubRip/blob/main/config.toml) ### Notes * All
-settings are optional. Not specifying a setting will result in using the
-default value.
+configure different options and features by creating a [TOML](https://toml.io)
+config file. A config file will be looked for in one of the following paths
+(according to OS): **Windows**: `%USERPROFILE%\.isubrip\config.toml` **Linux /
+macOS**: `$HOME/.isubrip/config.toml` ### Examples: **Windows**: `C:
+\Users\Michael\.isubrip\config.toml` **Linux**: `/home/Michael/.isubrip/
+config.toml` **macOS**: `/Users/Michael/.isubrip/config.toml` --- ### Example
+Config: ```toml [downloads] folder = "C:\\Subtitles\\iTunes" languages = ["en-
+US", "fr-FR", "he"] zip = false [subtitles] convert-to-srt = true fix-rtl =
+true ``` A complete config with all the available options and explanations for
+each configuration can be found [here](https://github.com/MichaelYochpaz/
+iSubRip/blob/main/config.toml)
```

### Comparing `isubrip-2.3.3/isubrip/subtitles.py` & `isubrip-2.4.0/isubrip/subtitle_formats/subtitles.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,205 +1,230 @@
 from __future__ import annotations
 
-import re
-
+from abc import ABC, abstractmethod
 from datetime import time
+from typing import ClassVar, Generic, TYPE_CHECKING, TypeVar
 
-from isubrip.constants import WEBVTT_CAPTION_BLOCK_REGEX, WEBVTT_COMMENT_HEADER_REGEX
-from isubrip.enums import SubtitlesFormat
-from isubrip.webvtt import WebVTTBlock, Caption, Comment, Region, Style
-
-
-class Subtitles:
-    """An object representing subtitles, made out of WebVTTBlocks."""
-    remove_duplicates = False
-    fix_rtl = False
-    rtl_languages = []
-
-    def __init__(self, language_code: str = None):
-        """Initalize a new Subtitles object."""
-        self.language_code: str = language_code
-        self.blocks: list[WebVTTBlock] = []
+from isubrip.data_structures import SubtitlesFormat, SubtitlesType
 
-    def __add__(self, block: WebVTTBlock) -> Subtitles:
-        self.add_block(block)
-        return self
+if TYPE_CHECKING:
+    from isubrip.subtitle_formats.subrip import SubRipCaptionBlock, SubRipSubtitles
 
-    def _dumps_vtt(self) -> str:
-        """
-        Dump subtitles to a string in VTT format.
+RTL_CONTROL_CHARS = ('\u200e', '\u200f', '\u202a', '\u202b', '\u202c', '\u202d', '\u202e')
+RTL_CHAR = '\u202b'
+RTL_LANGUAGES = ["ar", "he"]
 
-        Returns:
-            str: The subtitles formatted as a string in VTT format.
-        """
-        subtitles_str = "WEBVTT\n\n"
+SubtitlesT = TypeVar('SubtitlesT', bound='Subtitles')
+SubtitlesBlockT = TypeVar('SubtitlesBlockT', bound='SubtitlesBlock')
 
-        for block in self.blocks:
-            subtitles_str += str(block) + "\n\n"
 
-        return subtitles_str.rstrip('\n')
+class SubtitlesBlock(ABC):
+    """Abstract base class for subtitles blocks."""
+    @abstractmethod
+    def __str__(self):
+        pass
 
-    def _dumps_srt(self) -> str:
-        """
-        Dump subtitles to a string in SRT format.
+    @abstractmethod
+    def __eq__(self, other):
+        pass
 
-        Returns:
-            str: The subtitles formatted as a string in SRT format.
-        """
-        subtitles_str = ""
-        count = 0
-
-        for block in self.blocks:
-            if isinstance(block, Caption):
-                subtitles_str += f"{(count + 1)}\n{block.to_string(SubtitlesFormat.SRT)}\n\n"
-                count += 1
 
-        return subtitles_str.rstrip('\n')
+class SubtitlesCaptionBlock(SubtitlesBlock, ABC):
+    """A base class for subtitles caption blocks."""
 
-    @staticmethod
-    def _split_timestamp(timestamp: str) -> tuple[time, time]:
+    def __init__(self, start_time: time, end_time: time, payload: str):
         """
-        Splits a timestamp into start and end.
+        Initialize a new SubtitlesCaptionBlock object.
 
         Args:
-            timestamp (str): A subtitles timestamp. For example: "00:00:00.000 --> 00:00:00.000"
+            start_time: Start timestamp of the caption block.
+            end_time: End timestamp of the caption block.
+            payload: Caption block's payload (text).
+        """
+        self.start_time = start_time
+        self.end_time = end_time
+        self.payload = payload
+
+    def fix_rtl(self) -> None:
+        """Fix text direction to RTL."""
+        # Remove previous RTL-related formatting
+        for char in RTL_CONTROL_CHARS:
+            self.payload = self.payload.replace(char, '')
+
+        # Add RLM char at the start of every line
+        self.payload = RTL_CHAR + self.payload.replace("\n", f"\n{RTL_CHAR}")
+
+    def to_srt(self) -> SubRipCaptionBlock:
+        """
+        Convert WebVTT caption block to SRT caption block.
 
         Returns:
-            tuple(time, time): A tuple containing start and end times as a datetime object.
+            SubRipCaptionBlock: The caption block in SRT format.
         """
-        # Support ',' character in timestamp's milliseconds (used in srt format).
-        timestamp = timestamp.replace(',', '.')
+        from isubrip.subtitle_formats.subrip import SubRipCaptionBlock
 
-        start_time, end_time = timestamp.split(" --> ")
-        return time.fromisoformat(start_time), time.fromisoformat(end_time)
+        return SubRipCaptionBlock(self.start_time, self.end_time, self.payload)
 
-    def add_block(self, block: WebVTTBlock) -> None:
-        """
-        Add a new WebVTT block to current subtitles.
 
-        Args:
-            block (WebVTTBlock): A block object to append.
-        """
-        # Don't append if `remove-duplicates` is set to true and block is same as previous one
-        if not (Subtitles.remove_duplicates and len(self.blocks) > 0 and self.blocks[-1] == block):
-            # Fix RTL before appending if `fix-rtl` is set to true and language is an RTL language
-            if isinstance(block, Caption) and Subtitles.fix_rtl and self.language_code in Subtitles.rtl_languages:
-                block.fix_rtl()
+class Subtitles(Generic[SubtitlesBlockT], ABC):
+    """
+    An object representing subtitles, made out of blocks.
 
-            self.blocks.append(block)
+    Attributes:
+        format (SubtitlesFormat): [Class Attribute] Format of the subtitles (contains name and file extension).
+        blocks (list[SubtitlesBlock]): A list of subtitles blocks that make up the subtitles.
+        language_code (str | None): Language code of the subtitles.
+        special_type (SubtitlesType | None): Special type of the subtitles (if any).
+    """
+    format: ClassVar[SubtitlesFormat]
 
-    def append_subtitles(self, subtitles: Subtitles) -> None:
+    def __init__(self, blocks: list[SubtitlesBlockT] | None = None,
+                 language_code: str | None = None, special_type: SubtitlesType | None = None):
         """
-        Append an existing subtitles object.
+        Initialize a new Subtitles object.
 
         Args:
-            subtitles (Subtitles): Subtitles object to append to current subtitels.
+            blocks (list[SubtitlesBlock] | None, optional): A list of subtitles to initialize the object with.
+                Defaults to None.
+            language_code (str | None, optional): Language code of the subtitles. Defaults to None.
+            special_type (SubtitlesType | None, optional): Special type of the subtitles (if any). Defaults to None.
         """
-        for block in subtitles.blocks:
-            self.add_block(block)
+        self.language_code = language_code
+        self.special_type = special_type
 
-    @staticmethod
-    def loads(subtitles_data: str) -> Subtitles:
+        if blocks is None:
+            self.blocks = []
+
+        else:
+            self.blocks = blocks
+
+    def __add__(self: SubtitlesT, obj: SubtitlesBlockT | SubtitlesT) -> SubtitlesT:
         """
-        Load subtitles from a string.
+        Add a new subtitles block, or append blocks from another subtitles object.
 
         Args:
-            subtitles_data (str): Subtitles data to load.
+            obj (SubtitlesBlock | Subtitles): A subtitles block or another subtitles object.
 
         Returns:
-            Subtitles: A Subtitles object loaded from the string.
+            Subtitles: The current subtitles object.
         """
-        subtitles_obj = Subtitles()
-        prev_line: str = ""
+        if isinstance(obj, SubtitlesBlock):
+            self.add_block(obj)
+
+        elif isinstance(obj, self.__class__):
+            self.append_subtitles(obj)
+
+        return self
 
-        line_split_generator = iter(subtitles_data.splitlines())
-        for line in line_split_generator:
-            # TODO: Change 're' functinos to Walrus operator inside if statemetns once minimum Python version is 3.8
-            caption_block_regex = re.match(WEBVTT_CAPTION_BLOCK_REGEX, line)
-            comment_block_regex = re.match(WEBVTT_COMMENT_HEADER_REGEX, line)
+    def __eq__(self, other) -> bool:
+        return isinstance(other, type(self)) and self.blocks == other.blocks
 
-            # If the line is a timestamp
-            if caption_block_regex:
-                # If previous line wasn't empty, add it as an identifier
-                if prev_line:
-                    caption_identifier = prev_line
+    def __str__(self) -> str:
+        return self.dumps()
 
-                else:
-                    caption_identifier = ""
+    @abstractmethod
+    def dumps(self) -> str:
+        """Dump subtitles object to a string representing the subtitles."""
+        pass
 
-                caption_timestamps = Subtitles._split_timestamp(caption_block_regex.group(1))
-                caption_settings = caption_block_regex.group(2)
-                caption_payload = ""
+    @staticmethod
+    @abstractmethod
+    def loads(subtitles_data: str) -> Subtitles:
+        pass
 
-                for additional_line in line_split_generator:
-                    if not additional_line:
-                        line = additional_line
-                        break
+    def add_block(self: SubtitlesT, block: SubtitlesBlockT | list[SubtitlesBlockT]) -> SubtitlesT:
+        """
+        Add a new subtitles block to current subtitles.
 
-                    caption_payload += additional_line + "\n"
+        Args:
+            block (SubtitlesBlock | list[SubtitlesBlock]):
+                A block object or a list of block objects to append.
 
-                caption_payload = caption_payload.rstrip("\n")
-                subtitles_obj.add_block(Caption(identifier=caption_identifier,
-                                                start_time=caption_timestamps[0],
-                                                end_time=caption_timestamps[1],
-                                                settings=caption_settings,
-                                                payload=caption_payload))
+        Returns:
+            Subtitles: The current subtitles object.
+        """
+        if isinstance(block, list):
+            self.blocks.extend(block)
 
-            elif comment_block_regex:
-                comment_payload = ""
-                inline = False
+        else:
+            self.blocks.append(block)
 
-                if comment_block_regex.group(1) is not None:
-                    comment_payload += comment_block_regex.group(1) + "\n"
-                    inline = True
+        return self
 
-                for additional_line in line_split_generator:
-                    if not additional_line:
-                        line = additional_line
-                        break
+    def append_subtitles(self: SubtitlesT, subtitles: SubtitlesT) -> SubtitlesT:
+        """
+        Append an existing subtitles object.
 
-                    comment_payload += additional_line + "\n"
+        Args:
+            subtitles (Subtitles): Subtitles object to append to current subtitles.
 
-                subtitles_obj.add_block(Comment(comment_payload.rstrip("\n"), inline=inline))
+        Returns:
+            Subtitles: The current subtitles object.
+        """
+        for block in subtitles.blocks:
+            self.add_block(block)
 
-            elif line.rstrip(' \t') == Region.header:
-                region_payload = ""
+        return self
 
-                for additional_line in line_split_generator:
-                    if not additional_line:
-                        line = additional_line
-                        break
+    def dump(self) -> bytes:
+        return self.dumps().encode(encoding="UTF-8")
 
-                    region_payload += additional_line + "\n"
+    def polish(self: SubtitlesT, fix_rtl: bool = False,
+               rtl_languages: list[str] | None = None, remove_duplicates: bool = False) -> SubtitlesT:
+        """
+        Apply various fixes to subtitles.
 
-                subtitles_obj.add_block(Region(region_payload.rstrip("\n")))
+        Args:
+            fix_rtl (bool, optional): Whether to fix text direction of RTL languages. Defaults to False.
+            rtl_languages (list[str] | None, optional): Language code of the RTL language.
+                If not set, a default list of RTL languages will be used. Defaults to None.
+            remove_duplicates (bool, optional): Whether to remove duplicate captions. Defaults to False.
 
-            elif line.rstrip(' \t') == Style.header:
-                style_payload = ""
+        Returns:
+            Subtitles: The current subtitles object.
+        """
+        rtl_language = rtl_languages or RTL_LANGUAGES
+        previous_block: SubtitlesBlockT | None = None
 
-                for additional_line in line_split_generator:
-                    if not additional_line:
-                        line = additional_line
-                        break
+        for block in self.blocks:
+            if fix_rtl and isinstance(block, SubtitlesCaptionBlock) and \
+                    self.language_code in rtl_language:
+                block.fix_rtl()
 
-                    style_payload += additional_line + "\n"
+            if remove_duplicates and previous_block is not None and block == previous_block:
+                self.blocks.remove(previous_block)
 
-                subtitles_obj.add_block(Region(style_payload.rstrip("\n")))
+            previous_block = block
 
-            prev_line = line
-        return subtitles_obj
+        return self
 
-    def dumps(self, subtitles_format: SubtitlesFormat = SubtitlesFormat.VTT) -> str:
+    def to_srt(self) -> SubRipSubtitles:
         """
-        Dump subtitles to a string.
-
-        Args:
-            subtitles_format (SubtitlesFormat): Subtitles format specification to use.
+        Convert subtitles to SRT format.
 
         Returns:
-            str: The subtitles formatted as a string matching the specified subtitles format.
+            SubRipSubtitles: The subtitles in SRT format.
         """
-        if subtitles_format == SubtitlesFormat.VTT:
-            return self._dumps_vtt()
+        from isubrip.subtitle_formats.subrip import SubRipSubtitles
+
+        return SubRipSubtitles(
+            blocks=[block.to_srt() for block in self.blocks if isinstance(block, SubtitlesCaptionBlock)],
+            language_code=self.language_code,
+            special_type=self.special_type
+        )
+
+
+def split_timestamp(timestamp: str) -> tuple[time, time]:
+    """
+    Split a subtitles timestamp into start and end.
+
+    Args:
+        timestamp (str): A subtitles timestamp. For example: "00:00:00.000 --> 00:00:00.000"
+
+    Returns:
+        tuple(time, time): A tuple containing start and end times as a datetime object.
+    """
+    # Support ',' character in timestamp's milliseconds (used in SubRip format).
+    timestamp = timestamp.replace(',', '.')
 
-        elif subtitles_format == SubtitlesFormat.SRT:
-            return self._dumps_srt()
+    start_time, end_time = timestamp.split(" --> ")
+    return time.fromisoformat(start_time), time.fromisoformat(end_time)
```

### Comparing `isubrip-2.3.3/isubrip.egg-info/PKG-INFO` & `isubrip-2.4.0/isubrip.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
 Name: isubrip
-Version: 2.3.3
+Version: 2.4.0
 Summary: A Python package for scraping and downloading subtitles from iTunes movie pages.
 Home-page: https://github.com/MichaelYochpaz/iSubRip
 Author: Michael Yochpaz
 License: MIT
 Project-URL: Bug Reports, https://github.com/MichaelYochpaz/iSubRip/issues
 Project-URL: Source, https://github.com/MichaelYochpaz/iSubRip
-Keywords: iTunes,movies,subtitles,scrape,scraper,download,m3u8
+Keywords: iTunes,AppleTV,movies,subtitles,scrape,scraper,download,m3u8
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # iSubRip
-A Python package for scraping and downloading subtitles from iTunes movie pages.  
-Latest version: 2.3.3 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))  
+A Python package for scraping and downloading subtitles from AppleTV / iTunes movie pages.  
+Latest version: 2.4.0 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))  
 
 <br/>
   
 [![PyPI - Version](https://img.shields.io/pypi/v/isubrip)](https://python.org/pypi/isubrip)
 [![PyPI - Monthly Downloads](https://pepy.tech/badge/isubrip/month)](https://python.org/pypi/isubrip)
 [![PyPI - Total Downloads](https://pepy.tech/badge/isubrip)](https://python.org/pypi/isubrip)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/isubrip)](https://python.org/pypi/isubrip)
@@ -37,15 +40,15 @@
 
 <p align="center">
   <a href="#"><img src="https://user-images.githubusercontent.com/8832013/194750946-8b4d4d4e-0230-4653-bede-3ec191df161b.gif" width="800"></a>
 </p>
 
 
 ##  Requirements
-* Python 3.7+
+* Python 3.8+
 
 ##  Installation
 ### PyPI (Recommended)
 ```
 python3 -m pip install isubrip
 ```
 
@@ -56,36 +59,33 @@
 
 ## Usage
 ```
 isubrip <iTunes movie URL> [iTunes movie URL...]
 ```  
 
 ## Configuration
-It's possible to configure different options and enable / disable different features using a [TOML](https://toml.io) config file.   
-A config file will be looked for in one of the following paths according to OS: 
+It's possible to configure different options and features by creating a [TOML](https://toml.io) config file.   
+A config file will be looked for in one of the following paths (according to OS): 
 
 **Windows**: `%USERPROFILE%\.isubrip\config.toml`  
 **Linux / macOS**: `$HOME/.isubrip/config.toml`  
 
 ### Examples:
 **Windows**: `C:\Users\Michael\.isubrip\config.toml`  
 **Linux**: `/home/Michael/.isubrip/config.toml`  
 **macOS**: `/Users/Michael/.isubrip/config.toml`  
 
 ---
 
 ### Example Config:
 ```toml
 [downloads]
-folder = "C:\\iTunes-Subtitles"
-format = "srt"
-languages = ["en-US"]
+folder = "C:\\Subtitles\\iTunes"
+languages = ["en-US", "fr-FR", "he"]
 zip = false
 
 [subtitles]
+convert-to-srt = true
 fix-rtl = true
 ```
 
 A complete config with all the available options and explanations for each configuration can be found [here](https://github.com/MichaelYochpaz/iSubRip/blob/main/config.toml)
-
-### Notes
-* All settings are optional. Not specifying a setting will result in using the default value.
```

#### html2text {}

```diff
@@ -1,46 +1,46 @@
-Metadata-Version: 2.1 Name: isubrip Version: 2.3.3 Summary: A Python package
+Metadata-Version: 2.1 Name: isubrip Version: 2.4.0 Summary: A Python package
 for scraping and downloading subtitles from iTunes movie pages. Home-page:
 https://github.com/MichaelYochpaz/iSubRip Author: Michael Yochpaz License: MIT
 Project-URL: Bug Reports, https://github.com/MichaelYochpaz/iSubRip/issues
 Project-URL: Source, https://github.com/MichaelYochpaz/iSubRip Keywords:
-iTunes,movies,subtitles,scrape,scraper,download,m3u8 Classifier: Development
-Status :: 5 - Production/Stable Classifier: Intended Audience :: End Users/
-Desktop Classifier: Intended Audience :: Developers Classifier: Topic ::
-Utilities Classifier: License :: OSI Approved :: MIT License Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Requires-Python: >=3.7 Description-
-Content-Type: text/markdown License-File: LICENSE # iSubRip A Python package
-for scraping and downloading subtitles from iTunes movie pages. Latest version:
-2.3.3 ([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/
-CHANGELOG.md))
+iTunes,AppleTV,movies,subtitles,scrape,scraper,download,m3u8 Classifier:
+Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
+End Users/Desktop Classifier: Intended Audience :: Developers Classifier:
+Operating System :: Microsoft :: Windows Classifier: Operating System :: MacOS
+Classifier: Operating System :: POSIX :: Linux Classifier: Topic :: Utilities
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Requires-Python: >=3.8 Description-Content-Type:
+text/markdown License-File: LICENSE # iSubRip A Python package for scraping and
+downloading subtitles from AppleTV / iTunes movie pages. Latest version: 2.4.0
+([changelog](https://github.com/MichaelYochpaz/iSubRip/blob/main/CHANGELOG.md))
+
 [![PyPI - Version](https://img.shields.io/pypi/v/isubrip)](https://python.org/
 pypi/isubrip) [![PyPI - Monthly Downloads](https://pepy.tech/badge/isubrip/
 month)](https://python.org/pypi/isubrip) [![PyPI - Total Downloads](https://
 pepy.tech/badge/isubrip)](https://python.org/pypi/isubrip) [![PyPI - Python
 Version](https://img.shields.io/pypi/pyversions/isubrip)](https://python.org/
 pypi/isubrip) [![GitHub - License](https://img.shields.io/github/license/
 MichaelYochpaz/iSubRip)](https://github.com/MichaelYochpaz/iSubRip/blob/main/
 LICENSE) [![GitHub - issues](https://img.shields.io/github/issues/
 MichaelYochpaz/iSubRip)](https://github.com/MichaelYochpaz/iSubRip/issues) [!
 [GitHub - Repo stars](https://img.shields.io/github/stars/MichaelYochpaz/
 iSubRip.svg?color=yellow)](https://github.com/MichaelYochpaz/iSubRip)
   [https://user-images.githubusercontent.com/8832013/194750946-8b4d4d4e-0230-
                           4653-bede-3ec191df161b.gif]
-## Requirements * Python 3.7+ ## Installation ### PyPI (Recommended) ```
+## Requirements * Python 3.8+ ## Installation ### PyPI (Recommended) ```
 python3 -m pip install isubrip ``` ### Git Source Code ``` python3 -m pip
 install -e git+https://github.com/MichaelYochpaz/iSubRip.git#egg=isubrip ``` ##
 Usage ``` isubrip  [iTunes movie URL...] ``` ## Configuration It's possible to
-configure different options and enable / disable different features using a
-[TOML](https://toml.io) config file. A config file will be looked for in one of
-the following paths according to OS: **Windows**:
-`%USERPROFILE%\.isubrip\config.toml` **Linux / macOS**: `$HOME/.isubrip/
-config.toml` ### Examples: **Windows**: `C:\Users\Michael\.isubrip\config.toml`
-**Linux**: `/home/Michael/.isubrip/config.toml` **macOS**: `/Users/
-Michael/.isubrip/config.toml` --- ### Example Config: ```toml [downloads]
-folder = "C:\\iTunes-Subtitles" format = "srt" languages = ["en-US"] zip =
-false [subtitles] fix-rtl = true ``` A complete config with all the available
-options and explanations for each configuration can be found [here](https://
-github.com/MichaelYochpaz/iSubRip/blob/main/config.toml) ### Notes * All
-settings are optional. Not specifying a setting will result in using the
-default value.
+configure different options and features by creating a [TOML](https://toml.io)
+config file. A config file will be looked for in one of the following paths
+(according to OS): **Windows**: `%USERPROFILE%\.isubrip\config.toml` **Linux /
+macOS**: `$HOME/.isubrip/config.toml` ### Examples: **Windows**: `C:
+\Users\Michael\.isubrip\config.toml` **Linux**: `/home/Michael/.isubrip/
+config.toml` **macOS**: `/Users/Michael/.isubrip/config.toml` --- ### Example
+Config: ```toml [downloads] folder = "C:\\Subtitles\\iTunes" languages = ["en-
+US", "fr-FR", "he"] zip = false [subtitles] convert-to-srt = true fix-rtl =
+true ``` A complete config with all the available options and explanations for
+each configuration can be found [here](https://github.com/MichaelYochpaz/
+iSubRip/blob/main/config.toml)
```

### Comparing `isubrip-2.3.3/setup.py` & `isubrip-2.4.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,80 @@
-from os import PathLike
+from __future__ import annotations
+
+import re
 from pathlib import Path
-from typing import Union
+from setuptools import find_packages, setup
+
+CURRENT_PATH = Path(__file__).parent.absolute()
+PACKAGE_NAME = "isubrip"
+README_PATH = CURRENT_PATH / "README.md"
 
-from setuptools import setup
 
+def get_version() -> str:
+    init_file_path = CURRENT_PATH / PACKAGE_NAME / "__init__.py"
+    version_regex = r"^__version__ = ['\"](\d+(?:\.\d+){2,3})['\"]"
 
-def get_version(relative_path: Union[str, PathLike]) -> str:
-    current_path = Path(__file__).parent.absolute()
+    if not init_file_path.exists():
+        raise FileNotFoundError(f"{init_file_path} file is missing.")
 
-    with open(current_path / relative_path, 'r') as fp:
-        file_data: str = fp.read()
+    with open(init_file_path, 'r') as fp:
+        file_data = fp.read()
 
     for line in file_data.splitlines():
-        if line.startswith('__version__'):
-            delim = '"' if '"' in line else "'"
-            return line.split(delim)[1]
+        if line.startswith("__version__"):
+            if result := re.match(version_regex, line).group(1):
+                return result
+
+            else:
+                raise RuntimeError('__version__ assignment does not match expected regex.')
+
+    raise RuntimeError('Unable to find version string.')
 
-    raise RuntimeError("Unable to find version string.")
 
+def get_long_description() -> str:
+    readme_path = CURRENT_PATH / "README.md"
 
-PACKAGE_NAME: str = "isubrip"
+    if not readme_path.exists():
+        raise FileNotFoundError(f"{readme_path} file is missing.")
 
-with open("README.md", "r") as file:
-    long_description = file.read()
+    with open(readme_path, "r") as file:
+        return file.read()
 
 
 setup(
     name=PACKAGE_NAME,
-    version=get_version(Path(PACKAGE_NAME) / "__init__.py"),
+    version=get_version(),
     author="Michael Yochpaz",
     license="MIT",
     license_files=('LICENSE',),
     description="A Python package for scraping and downloading subtitles from iTunes movie pages.",
-    long_description=long_description,
+    long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/MichaelYochpaz/iSubRip",
-
     project_urls={
         "Bug Reports": "https://github.com/MichaelYochpaz/iSubRip/issues",
         "Source": "https://github.com/MichaelYochpaz/iSubRip"
     },
-
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: End Users/Desktop",
         "Intended Audience :: Developers",
+        "Operating System :: Microsoft :: Windows",
+        "Operating System :: MacOS",
+        "Operating System :: POSIX :: Linux",
         "Topic :: Utilities",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10"
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
-
-    keywords=["iTunes", "movies", "subtitles", "scrape", "scraper", "download", "m3u8"],
-    packages=["isubrip"],
-    install_requires=["aiohttp", "beautifulsoup4", "lxml", "m3u8", "mergedeep", "requests", "tomli"],
-    package_data={"isubrip": ["resources/*"]},
-    python_requires=">=3.7",
+    keywords=["iTunes", "AppleTV", "movies", "subtitles", "scrape", "scraper", "download", "m3u8"],
+    packages=find_packages(where=str(CURRENT_PATH)),
+    package_data={PACKAGE_NAME: ["resources/*"]},
+    python_requires=">=3.8",
+    install_requires=["aiohttp", "m3u8", "mergedeep", "requests", "tomli"],
     entry_points={
         "console_scripts":
-            ["isubrip = isubrip.__main__:main"]
+            [f"{PACKAGE_NAME} = {PACKAGE_NAME}.__main__:main"]
     },
 )
```

