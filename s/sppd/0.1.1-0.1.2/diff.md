# Comparing `tmp/sppd-0.1.1.tar.gz` & `tmp/sppd-0.1.2.tar.gz`

## Comparing `sppd-0.1.1.tar` & `sppd-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sppd-0.1.1/src/sppd/__init__.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 sppd-0.1.1/src/sppd/__main__.py
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 sppd-0.1.1/src/sppd/sppd.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sppd-0.1.1/LICENSE
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 sppd-0.1.1/README.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 sppd-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 sppd-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sppd-0.1.2/src/sppd/__init__.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 sppd-0.1.2/src/sppd/__main__.py
+-rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 sppd-0.1.2/src/sppd/sppd.py
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sppd-0.1.2/LICENSE
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 sppd-0.1.2/README.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 sppd-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 sppd-0.1.2/PKG-INFO
```

### Comparing `sppd-0.1.1/src/sppd/sppd.py` & `sppd-0.1.2/src/sppd/sppd.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from pytube import YouTube
 
 if os.name == 'posix':
     rawdownloadloc = os.environ.get('XDG_MUSIC_DIR', '~/Music/')
 elif os.name == 'nt':
     rawdownloadloc = '~\\Music'
 
-parser = argparse.ArgumentParser(description='Download Spotify playlist songs from YouTube', prog="sppd")
+parser = argparse.ArgumentParser(description='Download Spotify playlist songs from YouTube')
 parser.add_argument('-o', '--output', help='Specify download directory')
 parser.add_argument('PLAYLIST', type=str)
 args = parser.parse_args()
 
 playlist = args.PLAYLIST
 if args.output != None:
     rawdownloadloc = args.output
@@ -49,19 +49,18 @@
     print("Couldn't find album name, check playlist in browser or report bug")
     sys.exit(1)
 
 albumname = rawalbumname[0]['content']
 
 print("Finding song names")
 # Get song names
-for link in soup.find_all('button'):
-    if re.search("track", str(link.get('aria-label'))):
+for link in soup.find_all('div'):
+    if not re.search("None", str(link.get('aria-label'))):
         trackname = link.get('aria-label')
-        name = trackname.removeprefix('track ')
-        clean_name = re.sub('[^\w_.)( -]', '', name)
+        clean_name = re.sub('[^\w_.)( -]', '', trackname)
         namelist.append(clean_name)
 
 print("Searching YouTube, this will take a while")
 # Put 2 and 2 together and search youtube
 for ogname in namelist:
     s = Search(albumname + ' ' + ogname + ' explicit')
     ytlink = s.results[0]
```

### Comparing `sppd-0.1.1/LICENSE` & `sppd-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sppd-0.1.1/pyproject.toml` & `sppd-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sppd"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="emcy06236", email="emcy06236@proton.me" },
 ]
 description = "Spotify playlist downloader"
 readme = "README.md"
 license = "GPL-3.0"
 dependencies = [
```

### Comparing `sppd-0.1.1/PKG-INFO` & `sppd-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: sppd
-Version: 0.1.1
+Version: 0.1.2
 Summary: Spotify playlist downloader
 Project-URL: Homepage, https://github.com/emcy06236/sppd
 Project-URL: Bug Tracker, https://github.com/emcy06236/sppd/issues
 Author-email: emcy06236 <emcy06236@proton.me>
+License-Expression: GPL-3.0
+License-File: LICENSE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: beautifulsoup4
 Requires-Dist: pytube
 Description-Content-Type: text/markdown
 
 # sppd - spotify playlist downloader
 ## Windows
 ```
-py -m sppd [PLAYLIST]
+sppd [PLAYLIST]
 ```
 ## Anything else
 ```
 python3 -m sppd [PLAYLIST]
 ```
```

