# Comparing `tmp/favorites_crawler-0.1.8.tar.gz` & `tmp/favorites_crawler-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "favorites_crawler-0.1.8.tar", last modified: Sat Feb  4 17:26:59 2023, max compression
+gzip compressed data, was "favorites_crawler-0.1.9.tar", last modified: Sun May 21 09:27:32 2023, max compression
```

## Comparing `favorites_crawler-0.1.8.tar` & `favorites_crawler-0.1.9.tar`

### file list

```diff
@@ -1,44 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 17:26:59.348341 favorites_crawler-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-02-04 17:26:46.000000 favorites_crawler-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-04 17:26:46.000000 favorites_crawler-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-02-04 17:26:59.348341 favorites_crawler-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-02-04 17:26:46.000000 favorites_crawler-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-04 17:26:46.000000 favorites_crawler-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-02-04 17:26:46.000000 favorites_crawler-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-02-04 17:26:59.352341 favorites_crawler-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-02-04 17:26:46.000000 favorites_crawler-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 17:26:59.344341 favorites_crawler-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 17:26:59.348341 favorites_crawler-0.1.8/src/favorites_crawler/
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-02-04 17:26:46.000000 favorites_crawler-0.1.8/src/favorites_crawler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 17:26:59.348341 favorites_crawler-0.1.8/src/favorites_crawler/constants/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-04 17:26:46.000000 favorites_crawler-0.1.8/src/favorites_crawler/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-02-04 17:26:46.000000 favorites_crawler-0.1.8/src/favorites_crawler/constants/domains.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-02-04 17:26:46.000000 favorites_crawler-0.1.8/src/favorites_crawler/constants/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-02-04 17:26:46.000000 favorites_crawler-0.1.8/src/favorites_crawler/constants/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-04 17:26:46.000000 favorites_crawler-0.1.8/src/favorites_crawler/constants/regexes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-02-04 17:26:46.000000 favorites_crawler-0.1.8/src/favorites_crawler/itemloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-02-04 17:26:46.000000 favorites_crawler-0.1.8/src/favorites_crawler/items.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-02-04 17:26:46.000000 favorites_crawler-0.1.8/src/favorites_crawler/middlewares.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-02-04 17:26:46.000000 favorites_crawler-0.1.8/src/favorites_crawler/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-02-04 17:26:46.000000 favorites_crawler-0.1.8/src/favorites_crawler/processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-02-04 17:26:46.000000 favorites_crawler-0.1.8/src/favorites_crawler/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 17:26:59.348341 favorites_crawler-0.1.8/src/favorites_crawler/spiders/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-02-04 17:26:46.000000 favorites_crawler-0.1.8/src/favorites_crawler/spiders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-02-04 17:26:46.000000 favorites_crawler-0.1.8/src/favorites_crawler/spiders/lemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-02-04 17:26:46.000000 favorites_crawler-0.1.8/src/favorites_crawler/spiders/nhentai.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-02-04 17:26:46.000000 favorites_crawler-0.1.8/src/favorites_crawler/spiders/pixiv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-02-04 17:26:46.000000 favorites_crawler-0.1.8/src/favorites_crawler/spiders/yandere.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 17:26:59.348341 favorites_crawler-0.1.8/src/favorites_crawler/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-04 17:26:46.000000 favorites_crawler-0.1.8/src/favorites_crawler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-02-04 17:26:46.000000 favorites_crawler-0.1.8/src/favorites_crawler/utils/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-02-04 17:26:46.000000 favorites_crawler-0.1.8/src/favorites_crawler/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-02-04 17:26:46.000000 favorites_crawler-0.1.8/src/favorites_crawler/utils/cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-02-04 17:26:46.000000 favorites_crawler-0.1.8/src/favorites_crawler/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-02-04 17:26:46.000000 favorites_crawler-0.1.8/src/favorites_crawler/utils/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 17:26:59.348341 favorites_crawler-0.1.8/src/favorites_crawler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-02-04 17:26:59.000000 favorites_crawler-0.1.8/src/favorites_crawler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-02-04 17:26:59.000000 favorites_crawler-0.1.8/src/favorites_crawler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-04 17:26:59.000000 favorites_crawler-0.1.8/src/favorites_crawler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-04 17:26:59.000000 favorites_crawler-0.1.8/src/favorites_crawler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-04 17:26:59.000000 favorites_crawler-0.1.8/src/favorites_crawler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-04 17:26:59.000000 favorites_crawler-0.1.8/src/favorites_crawler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 09:27:32.315065 favorites_crawler-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-21 09:27:21.000000 favorites_crawler-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-21 09:27:21.000000 favorites_crawler-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-05-21 09:27:32.315065 favorites_crawler-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-05-21 09:27:21.000000 favorites_crawler-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-21 09:27:21.000000 favorites_crawler-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-21 09:27:21.000000 favorites_crawler-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-21 09:27:32.319065 favorites_crawler-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-21 09:27:21.000000 favorites_crawler-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 09:27:32.311065 favorites_crawler-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 09:27:32.315065 favorites_crawler-0.1.9/src/favorites_crawler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-05-21 09:27:21.000000 favorites_crawler-0.1.9/src/favorites_crawler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 09:27:32.315065 favorites_crawler-0.1.9/src/favorites_crawler/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 09:27:21.000000 favorites_crawler-0.1.9/src/favorites_crawler/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-21 09:27:21.000000 favorites_crawler-0.1.9/src/favorites_crawler/constants/domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-21 09:27:21.000000 favorites_crawler-0.1.9/src/favorites_crawler/constants/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-21 09:27:21.000000 favorites_crawler-0.1.9/src/favorites_crawler/constants/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-21 09:27:21.000000 favorites_crawler-0.1.9/src/favorites_crawler/constants/regexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-21 09:27:21.000000 favorites_crawler-0.1.9/src/favorites_crawler/itemloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-21 09:27:21.000000 favorites_crawler-0.1.9/src/favorites_crawler/items.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-21 09:27:21.000000 favorites_crawler-0.1.9/src/favorites_crawler/middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-21 09:27:21.000000 favorites_crawler-0.1.9/src/favorites_crawler/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-21 09:27:21.000000 favorites_crawler-0.1.9/src/favorites_crawler/processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-21 09:27:21.000000 favorites_crawler-0.1.9/src/favorites_crawler/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 09:27:32.315065 favorites_crawler-0.1.9/src/favorites_crawler/spiders/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-21 09:27:21.000000 favorites_crawler-0.1.9/src/favorites_crawler/spiders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-21 09:27:21.000000 favorites_crawler-0.1.9/src/favorites_crawler/spiders/lemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-21 09:27:21.000000 favorites_crawler-0.1.9/src/favorites_crawler/spiders/nhentai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-21 09:27:21.000000 favorites_crawler-0.1.9/src/favorites_crawler/spiders/pixiv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-21 09:27:21.000000 favorites_crawler-0.1.9/src/favorites_crawler/spiders/yandere.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 09:27:32.315065 favorites_crawler-0.1.9/src/favorites_crawler/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 09:27:21.000000 favorites_crawler-0.1.9/src/favorites_crawler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-21 09:27:21.000000 favorites_crawler-0.1.9/src/favorites_crawler/utils/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-21 09:27:21.000000 favorites_crawler-0.1.9/src/favorites_crawler/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-21 09:27:21.000000 favorites_crawler-0.1.9/src/favorites_crawler/utils/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-21 09:27:21.000000 favorites_crawler-0.1.9/src/favorites_crawler/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-21 09:27:21.000000 favorites_crawler-0.1.9/src/favorites_crawler/utils/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 09:27:32.315065 favorites_crawler-0.1.9/src/favorites_crawler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-05-21 09:27:32.000000 favorites_crawler-0.1.9/src/favorites_crawler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-21 09:27:32.000000 favorites_crawler-0.1.9/src/favorites_crawler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 09:27:32.000000 favorites_crawler-0.1.9/src/favorites_crawler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-21 09:27:32.000000 favorites_crawler-0.1.9/src/favorites_crawler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-21 09:27:32.000000 favorites_crawler-0.1.9/src/favorites_crawler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-21 09:27:32.000000 favorites_crawler-0.1.9/src/favorites_crawler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 09:27:32.315065 favorites_crawler-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-21 09:27:21.000000 favorites_crawler-0.1.9/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-05-21 09:27:21.000000 favorites_crawler-0.1.9/tests/test_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-05-21 09:27:21.000000 favorites_crawler-0.1.9/tests/test_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-21 09:27:21.000000 favorites_crawler-0.1.9/tests/test_processors.py
```

### Comparing `favorites_crawler-0.1.8/LICENSE` & `favorites_crawler-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `favorites_crawler-0.1.8/PKG-INFO` & `favorites_crawler-0.1.9/src/favorites_crawler.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: favorites_crawler
-Version: 0.1.8
+Name: favorites-crawler
+Version: 0.1.9
 Summary: Crawl your personal favorite images, photo albums, comics from website. Support pixiv, yande.re for now.
 Home-page: https://github.com/RyouMon/FavoritesCrawler
 Author: RyouMon
 Author-email: wenslife@outlook.com
 Project-URL: Bug Tracker, https://github.com/RyouMon/FavoritesCrawler/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -126,18 +126,40 @@
   ACCESS_TOKEN: xxxxxxxxxxxxxxxxxxxxxxxxxxxx
   REFRESH_TOKEN: xxxxxxxxxxxxxxxxxxxxxxxxxxxx
   USER_ID: xxxx
 yandere:
   USERNAME: xxxx
 ```
 
-If you want save pixiv files to `pictures/a`, and want save yandere files to `pictures/b`, you can modify config file like this:
+## Download location
+By default, pictures will download to working directory.  
+If you want to change download location, you can add FILES_STORE option to config.  
+For example, if you want save pixiv files to `pictures/a`, and want save yandere files to `pictures/b`, you can modify config file like this:
 ```yaml
 pixiv:
   ACCESS_TOKEN: xxxxxxxxxxxxxxxxxxxxxxxxxxxx
   REFRESH_TOKEN: xxxxxxxxxxxxxxxxxxxxxxxxxxxx
   USER_ID: xxxx
   FILES_STORE: pictures/a
 yandere:
   USERNAME: xxxx
   FILES_STORE: pictures/b
 ```
+
+## Organize file by artist
+if you want to organize pixiv illust by user, add this line to your config:
+```yaml
+...
+pixiv:
+  # FAVORS_PIXIV_ENABLE_ORGANIZE_BY_USER: true  # (Deprecation)
+  ENABLE_ORGANIZE_BY_ARTIST: true  # add this line to your yandere config
+  ...
+...
+```
+if you want to organize yandere post by artist, add this line to your config:
+```yaml
+...
+yandere:
+  ENABLE_ORGANIZE_BY_ARTIST: true  # add this line to your yandere config
+  ...
+...
+```
```

### Comparing `favorites_crawler-0.1.8/README.md` & `favorites_crawler-0.1.9/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -111,18 +111,40 @@
   ACCESS_TOKEN: xxxxxxxxxxxxxxxxxxxxxxxxxxxx
   REFRESH_TOKEN: xxxxxxxxxxxxxxxxxxxxxxxxxxxx
   USER_ID: xxxx
 yandere:
   USERNAME: xxxx
 ```
 
-If you want save pixiv files to `pictures/a`, and want save yandere files to `pictures/b`, you can modify config file like this:
+## Download location
+By default, pictures will download to working directory.  
+If you want to change download location, you can add FILES_STORE option to config.  
+For example, if you want save pixiv files to `pictures/a`, and want save yandere files to `pictures/b`, you can modify config file like this:
 ```yaml
 pixiv:
   ACCESS_TOKEN: xxxxxxxxxxxxxxxxxxxxxxxxxxxx
   REFRESH_TOKEN: xxxxxxxxxxxxxxxxxxxxxxxxxxxx
   USER_ID: xxxx
   FILES_STORE: pictures/a
 yandere:
   USERNAME: xxxx
   FILES_STORE: pictures/b
+```
+
+## Organize file by artist
+if you want to organize pixiv illust by user, add this line to your config:
+```yaml
+...
+pixiv:
+  # FAVORS_PIXIV_ENABLE_ORGANIZE_BY_USER: true  # (Deprecation)
+  ENABLE_ORGANIZE_BY_ARTIST: true  # add this line to your yandere config
+  ...
+...
+```
+if you want to organize yandere post by artist, add this line to your config:
+```yaml
+...
+yandere:
+  ENABLE_ORGANIZE_BY_ARTIST: true  # add this line to your yandere config
+  ...
+...
 ```
```

### Comparing `favorites_crawler-0.1.8/setup.cfg` & `favorites_crawler-0.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `favorites_crawler-0.1.8/src/favorites_crawler/__init__.py` & `favorites_crawler-0.1.9/src/favorites_crawler/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from scrapy.crawler import CrawlerProcess
 from scrapy.utils.project import get_project_settings
 from scrapy.spiderloader import SpiderLoader
 
 from favorites_crawler.utils import auth
 from favorites_crawler.utils.config import load_config, overwrite_settings
 
-__version__ = '0.1.8'
+__version__ = '0.1.9'
 
 logger = getLogger(__name__)
 
 os.environ.setdefault('SCRAPY_SETTINGS_MODULE', 'favorites_crawler.settings')
 scrapy_settings = get_project_settings()
 spider_loader = SpiderLoader(scrapy_settings)
 overwrite_settings(spider_loader, scrapy_settings, load_config())
```

### Comparing `favorites_crawler-0.1.8/src/favorites_crawler/itemloaders.py` & `favorites_crawler-0.1.9/src/favorites_crawler/itemloaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 class YanderePostItemLoader(ItemLoader):
     """Yandere Post Loader"""
     default_item_class = items.YanderePostItem
     default_output_processor = take_first
 
     file_urls_out = identity
+    artist_out = Compose(take_first, lambda s: s.strip())
 
 
 class NHentaiGalleryItemLoader(ItemLoader):
     default_item_class = items.NHentaiGalleryItem
     default_output_processor = take_first
 
     id_out = Compose(take_first, get_nhentai_id)
```

### Comparing `favorites_crawler-0.1.8/src/favorites_crawler/items.py` & `favorites_crawler-0.1.9/src/favorites_crawler/items.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,24 +70,29 @@
 
 @dataclass
 class PixivIllustItem(BaseItem):
 
     user_id: str = field(default=None)
 
     def get_folder_name(self, spider):
-        if not spider.crawler.settings.getbool('FAVORS_PIXIV_ENABLE_ORGANIZE_BY_USER'):
+        if not (spider.crawler.settings.getbool('FAVORS_PIXIV_ENABLE_ORGANIZE_BY_USER')
+                or spider.crawler.settings.getbool('ENABLE_ORGANIZE_BY_ARTIST')):
             return ''
         return self.user_id or 'unknown'
 
 
 @dataclass
 class YanderePostItem(BaseItem):
 
-    def get_folder_name(self, _):
-        return ''
+    artist: str = field(default=None)
+
+    def get_folder_name(self, spider):
+        if not spider.crawler.settings.getbool('ENABLE_ORGANIZE_BY_ARTIST'):
+            return ''
+        return self.artist or 'unknown'
 
 
 @dataclass
 class LemonPicPostItem(BaseItem, ComicBookInfoItem):
     title: str = field(default=None, metadata={'is_comic_info': True})
     tags: list = field(default=None, metadata={'is_comic_info': True})
```

### Comparing `favorites_crawler-0.1.8/src/favorites_crawler/pipelines.py` & `favorites_crawler-0.1.9/src/favorites_crawler/pipelines.py`

 * *Files identical despite different names*

### Comparing `favorites_crawler-0.1.8/src/favorites_crawler/processors.py` & `favorites_crawler-0.1.9/src/favorites_crawler/processors.py`

 * *Files identical despite different names*

### Comparing `favorites_crawler-0.1.8/src/favorites_crawler/settings.py` & `favorites_crawler-0.1.9/src/favorites_crawler/settings.py`

 * *Files identical despite different names*

### Comparing `favorites_crawler-0.1.8/src/favorites_crawler/spiders/lemon.py` & `favorites_crawler-0.1.9/src/favorites_crawler/spiders/lemon.py`

 * *Files identical despite different names*

### Comparing `favorites_crawler-0.1.8/src/favorites_crawler/spiders/nhentai.py` & `favorites_crawler-0.1.9/src/favorites_crawler/spiders/nhentai.py`

 * *Files identical despite different names*

### Comparing `favorites_crawler-0.1.8/src/favorites_crawler/spiders/pixiv.py` & `favorites_crawler-0.1.9/src/favorites_crawler/spiders/pixiv.py`

 * *Files identical despite different names*

### Comparing `favorites_crawler-0.1.8/src/favorites_crawler/spiders/yandere.py` & `favorites_crawler-0.1.9/src/favorites_crawler/spiders/yandere.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from scrapy import Request
 from scrapy.exceptions import CloseSpider
 
 from favorites_crawler.spiders import BaseSpider
 from favorites_crawler.constants.domains import YANDERE_DOMAIN
 from favorites_crawler.itemloaders import YanderePostItemLoader
-from favorites_crawler.constants.endpoints import YANDERE_POST_URL
+from favorites_crawler.constants.endpoints import YANDERE_LIST_POST_URL, YANDERE_SHOW_POST_URL
 
 
 class YandereSpider(BaseSpider):
     """Crawl voted post from yandere"""
     name = 'yandere'
     allowed_domains = (YANDERE_DOMAIN, )
     custom_settings = {
@@ -24,30 +24,39 @@
 
     def start_requests(self):
         username = self.custom_settings.get('USERNAME')
         if not username:
             raise CloseSpider('Did you run "favors login yandere"?')
 
         self.params['tags'] = f'vote:>=1:{username}'
-        yield Request(f'{YANDERE_POST_URL}?{urlencode(self.params)}')
+        yield Request(f'{YANDERE_LIST_POST_URL}?{urlencode(self.params)}')
 
     def parse_start_url(self, response, **kwargs):
-        for request_or_item in self.parse(response, **kwargs):
-            yield request_or_item
-
-    def parse(self, response, **kwargs):
-        """Spider Contracts:
+        """Parse list post url
         @url https://yande.re/post.json?limit=100&page=1
-        @returns item 100
-        @returns requests 1
-        @scrapes file_urls
+        @returns requests 101
         """
         posts = response.json()
 
         if len(posts) == self.limit:
             self.params['page'] += 1
-            yield Request(f'{YANDERE_POST_URL}?{urlencode(self.params)}')
+            yield Request(f'{YANDERE_LIST_POST_URL}?{urlencode(self.params)}', callback=self.parse_start_url)
 
         for post in posts:
             loader = YanderePostItemLoader()
             loader.add_value('file_urls', post['file_url'])
-            yield loader.load_item()
+            if self.settings.getbool('ENABLE_ORGANIZE_BY_ARTIST'):
+                yield Request(YANDERE_SHOW_POST_URL.format(id=post['id']),
+                              callback=self.parse, cb_kwargs={'loader': loader})
+            else:
+                yield loader.load_item()
+
+    def parse(self, response, **kwargs):
+        """Parse show post url
+        @url https://yande.re/post/show/1056911
+        @returns item 1
+        @scrapes artist
+        """
+        loader = kwargs.get('loader', YanderePostItemLoader())
+        loader.selector = response
+        loader.add_xpath('artist', '//li[@class="tag-type-artist"]/a[last()]/text()')
+        yield loader.load_item()
```

### Comparing `favorites_crawler-0.1.8/src/favorites_crawler/utils/auth.py` & `favorites_crawler-0.1.9/src/favorites_crawler/utils/auth.py`

 * *Files identical despite different names*

### Comparing `favorites_crawler-0.1.8/src/favorites_crawler/utils/config.py` & `favorites_crawler-0.1.9/src/favorites_crawler/utils/config.py`

 * *Files identical despite different names*

### Comparing `favorites_crawler-0.1.8/src/favorites_crawler.egg-info/PKG-INFO` & `favorites_crawler-0.1.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: favorites-crawler
-Version: 0.1.8
+Name: favorites_crawler
+Version: 0.1.9
 Summary: Crawl your personal favorite images, photo albums, comics from website. Support pixiv, yande.re for now.
 Home-page: https://github.com/RyouMon/FavoritesCrawler
 Author: RyouMon
 Author-email: wenslife@outlook.com
 Project-URL: Bug Tracker, https://github.com/RyouMon/FavoritesCrawler/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -126,18 +126,40 @@
   ACCESS_TOKEN: xxxxxxxxxxxxxxxxxxxxxxxxxxxx
   REFRESH_TOKEN: xxxxxxxxxxxxxxxxxxxxxxxxxxxx
   USER_ID: xxxx
 yandere:
   USERNAME: xxxx
 ```
 
-If you want save pixiv files to `pictures/a`, and want save yandere files to `pictures/b`, you can modify config file like this:
+## Download location
+By default, pictures will download to working directory.  
+If you want to change download location, you can add FILES_STORE option to config.  
+For example, if you want save pixiv files to `pictures/a`, and want save yandere files to `pictures/b`, you can modify config file like this:
 ```yaml
 pixiv:
   ACCESS_TOKEN: xxxxxxxxxxxxxxxxxxxxxxxxxxxx
   REFRESH_TOKEN: xxxxxxxxxxxxxxxxxxxxxxxxxxxx
   USER_ID: xxxx
   FILES_STORE: pictures/a
 yandere:
   USERNAME: xxxx
   FILES_STORE: pictures/b
 ```
+
+## Organize file by artist
+if you want to organize pixiv illust by user, add this line to your config:
+```yaml
+...
+pixiv:
+  # FAVORS_PIXIV_ENABLE_ORGANIZE_BY_USER: true  # (Deprecation)
+  ENABLE_ORGANIZE_BY_ARTIST: true  # add this line to your yandere config
+  ...
+...
+```
+if you want to organize yandere post by artist, add this line to your config:
+```yaml
+...
+yandere:
+  ENABLE_ORGANIZE_BY_ARTIST: true  # add this line to your yandere config
+  ...
+...
+```
```

### Comparing `favorites_crawler-0.1.8/src/favorites_crawler.egg-info/SOURCES.txt` & `favorites_crawler-0.1.9/src/favorites_crawler.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -29,8 +29,12 @@
 src/favorites_crawler/spiders/pixiv.py
 src/favorites_crawler/spiders/yandere.py
 src/favorites_crawler/utils/__init__.py
 src/favorites_crawler/utils/auth.py
 src/favorites_crawler/utils/config.py
 src/favorites_crawler/utils/cookies.py
 src/favorites_crawler/utils/files.py
-src/favorites_crawler/utils/text.py
+src/favorites_crawler/utils/text.py
+tests/test_init.py
+tests/test_items.py
+tests/test_pipelines.py
+tests/test_processors.py
```

