# Comparing `tmp/subsonic_connector-0.1.8.tar.gz` & `tmp/subsonic_connector-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subsonic_connector-0.1.8.tar", max compression
+gzip compressed data, was "subsonic_connector-0.1.9.tar", max compression
```

## Comparing `subsonic_connector-0.1.8.tar` & `subsonic_connector-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1071 2023-02-09 22:19:58.092756 subsonic_connector-0.1.8/LICENSE
--rw-r--r--   0        0        0     1015 2023-02-09 22:19:58.092852 subsonic_connector-0.1.8/README.md
--rw-r--r--   0        0        0      869 2023-02-14 13:51:20.264220 subsonic_connector-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-09 22:19:58.093122 subsonic_connector-0.1.8/subsonic_connector/__init__.py
--rw-r--r--   0        0        0     1560 2023-02-09 22:19:58.093223 subsonic_connector-0.1.8/subsonic_connector/album.py
--rw-r--r--   0        0        0      296 2023-02-09 22:19:58.093317 subsonic_connector-0.1.8/subsonic_connector/album_list.py
--rw-r--r--   0        0        0     1127 2023-02-09 22:19:58.093407 subsonic_connector-0.1.8/subsonic_connector/artist.py
--rw-r--r--   0        0        0      272 2023-02-09 22:19:58.093494 subsonic_connector-0.1.8/subsonic_connector/artist_cover.py
--rw-r--r--   0        0        0      476 2023-02-09 22:19:58.093597 subsonic_connector-0.1.8/subsonic_connector/artist_list_item.py
--rw-r--r--   0        0        0      346 2023-02-09 22:19:58.093694 subsonic_connector-0.1.8/subsonic_connector/artists.py
--rw-r--r--   0        0        0      424 2023-02-09 22:19:58.093794 subsonic_connector-0.1.8/subsonic_connector/artists_initial.py
--rw-r--r--   0        0        0     1106 2023-02-14 11:07:22.523640 subsonic_connector-0.1.8/subsonic_connector/configuration.py
--rw-r--r--   0        0        0     7690 2023-02-14 13:49:35.241430 subsonic_connector-0.1.8/subsonic_connector/connector.py
--rw-r--r--   0        0        0      868 2023-02-14 11:07:17.593581 subsonic_connector-0.1.8/subsonic_connector/default_config.py
--rw-r--r--   0        0        0      386 2023-02-09 22:19:58.094167 subsonic_connector-0.1.8/subsonic_connector/genre.py
--rw-r--r--   0        0        0      295 2023-02-09 22:19:58.094252 subsonic_connector-0.1.8/subsonic_connector/genres.py
--rw-r--r--   0        0        0     1494 2023-02-09 22:19:58.094343 subsonic_connector-0.1.8/subsonic_connector/item.py
--rw-r--r--   0        0        0      521 2023-02-09 22:19:58.094427 subsonic_connector-0.1.8/subsonic_connector/list_type.py
--rw-r--r--   0        0        0      299 2023-02-09 22:19:58.094517 subsonic_connector-0.1.8/subsonic_connector/random_songs.py
--rw-r--r--   0        0        0      556 2023-02-10 14:10:19.231432 subsonic_connector-0.1.8/subsonic_connector/response.py
--rw-r--r--   0        0        0      761 2023-02-09 22:19:58.094728 subsonic_connector-0.1.8/subsonic_connector/search_result.py
--rw-r--r--   0        0        0     2288 2023-02-09 22:19:58.094894 subsonic_connector-0.1.8/subsonic_connector/song.py
--rw-r--r--   0        0        0     1452 1970-01-01 00:00:00.000000 subsonic_connector-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-01-09 22:52:18.513324 subsonic_connector-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1015 2023-02-18 08:28:51.534469 subsonic_connector-0.1.9/README.md
+-rw-r--r--   0        0        0      869 2023-02-18 08:50:14.785480 subsonic_connector-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-09 17:27:17.948469 subsonic_connector-0.1.9/subsonic_connector/__init__.py
+-rw-r--r--   0        0        0     1650 2023-02-18 08:48:29.322930 subsonic_connector-0.1.9/subsonic_connector/album.py
+-rw-r--r--   0        0        0      296 2023-02-18 08:28:51.534469 subsonic_connector-0.1.9/subsonic_connector/album_list.py
+-rw-r--r--   0        0        0     1127 2023-02-18 08:28:51.534469 subsonic_connector-0.1.9/subsonic_connector/artist.py
+-rw-r--r--   0        0        0      272 2023-01-13 17:20:38.897139 subsonic_connector-0.1.9/subsonic_connector/artist_cover.py
+-rw-r--r--   0        0        0      476 2023-02-18 08:28:51.534469 subsonic_connector-0.1.9/subsonic_connector/artist_list_item.py
+-rw-r--r--   0        0        0      346 2023-02-18 08:28:51.534469 subsonic_connector-0.1.9/subsonic_connector/artists.py
+-rw-r--r--   0        0        0      424 2023-02-18 08:28:51.534469 subsonic_connector-0.1.9/subsonic_connector/artists_initial.py
+-rw-r--r--   0        0        0     1106 2023-02-18 08:28:51.534469 subsonic_connector-0.1.9/subsonic_connector/configuration.py
+-rw-r--r--   0        0        0     7690 2023-02-18 08:28:51.534469 subsonic_connector-0.1.9/subsonic_connector/connector.py
+-rw-r--r--   0        0        0      868 2023-02-18 08:28:51.534469 subsonic_connector-0.1.9/subsonic_connector/default_config.py
+-rw-r--r--   0        0        0      386 2023-02-18 08:28:51.534469 subsonic_connector-0.1.9/subsonic_connector/genre.py
+-rw-r--r--   0        0        0      295 2023-02-18 08:28:51.534469 subsonic_connector-0.1.9/subsonic_connector/genres.py
+-rw-r--r--   0        0        0     1494 2023-02-18 08:28:51.534469 subsonic_connector-0.1.9/subsonic_connector/item.py
+-rw-r--r--   0        0        0      521 2023-02-18 08:28:51.534469 subsonic_connector-0.1.9/subsonic_connector/list_type.py
+-rw-r--r--   0        0        0      299 2023-02-18 08:28:51.534469 subsonic_connector-0.1.9/subsonic_connector/random_songs.py
+-rw-r--r--   0        0        0      556 2023-02-18 08:28:51.537802 subsonic_connector-0.1.9/subsonic_connector/response.py
+-rw-r--r--   0        0        0      761 2023-02-18 08:28:51.537802 subsonic_connector-0.1.9/subsonic_connector/search_result.py
+-rw-r--r--   0        0        0     2288 2023-02-18 08:28:51.537802 subsonic_connector-0.1.9/subsonic_connector/song.py
+-rw-r--r--   0        0        0     1452 1970-01-01 00:00:00.000000 subsonic_connector-0.1.9/PKG-INFO
```

### Comparing `subsonic_connector-0.1.8/LICENSE` & `subsonic_connector-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `subsonic_connector-0.1.8/README.md` & `subsonic_connector-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `subsonic_connector-0.1.8/pyproject.toml` & `subsonic_connector-0.1.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "subsonic_connector_GioF71"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="GioF71", email="giovanni.fulco@gmail.com" },
 ]
 description = "SubSonic Connector based on LibSonic"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -15,15 +15,15 @@
 
 [project.urls]
 "Homepage" = "https://github.com/GioF71/subsonic-connector"
 "Bug Tracker" = "https://github.com/GioF71/subsonic-connector/issues"
 
 [tool.poetry]
 name = "subsonic-connector"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["GioF71 <giovanni.fulco@gmail.com>"]
 readme = "README.md"
 packages = [{include = "subsonic_connector"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `subsonic_connector-0.1.8/subsonic_connector/album.py` & `subsonic_connector-0.1.9/subsonic_connector/album.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,17 @@
 
     def getTitle(self) -> str | None:
         return self.__select_item.getByName(self.__key_title)
 
     def getGenre(self) -> str | None:
         return self.__select_item.getByName("genre")
 
+    def getYear(self) -> str | None:
+        return self.__select_item.getByName("year")
+
     def getDuration(self) -> str:
         return self.__select_item.getByName("duration")
 
     def getSongCount(self) -> str:
         return self.__select_item.getByName("songCount")
 
     def getSongs(self) -> list[Song]:
```

### Comparing `subsonic_connector-0.1.8/subsonic_connector/artist.py` & `subsonic_connector-0.1.9/subsonic_connector/artist.py`

 * *Files identical despite different names*

### Comparing `subsonic_connector-0.1.8/subsonic_connector/configuration.py` & `subsonic_connector-0.1.9/subsonic_connector/configuration.py`

 * *Files identical despite different names*

### Comparing `subsonic_connector-0.1.8/subsonic_connector/connector.py` & `subsonic_connector-0.1.9/subsonic_connector/connector.py`

 * *Files identical despite different names*

### Comparing `subsonic_connector-0.1.8/subsonic_connector/default_config.py` & `subsonic_connector-0.1.9/subsonic_connector/default_config.py`

 * *Files identical despite different names*

### Comparing `subsonic_connector-0.1.8/subsonic_connector/item.py` & `subsonic_connector-0.1.9/subsonic_connector/item.py`

 * *Files identical despite different names*

### Comparing `subsonic_connector-0.1.8/subsonic_connector/list_type.py` & `subsonic_connector-0.1.9/subsonic_connector/list_type.py`

 * *Files identical despite different names*

### Comparing `subsonic_connector-0.1.8/subsonic_connector/response.py` & `subsonic_connector-0.1.9/subsonic_connector/response.py`

 * *Files identical despite different names*

### Comparing `subsonic_connector-0.1.8/subsonic_connector/search_result.py` & `subsonic_connector-0.1.9/subsonic_connector/search_result.py`

 * *Files identical despite different names*

### Comparing `subsonic_connector-0.1.8/subsonic_connector/song.py` & `subsonic_connector-0.1.9/subsonic_connector/song.py`

 * *Files identical despite different names*

### Comparing `subsonic_connector-0.1.8/PKG-INFO` & `subsonic_connector-0.1.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subsonic-connector
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: GioF71
 Author-email: giovanni.fulco@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

