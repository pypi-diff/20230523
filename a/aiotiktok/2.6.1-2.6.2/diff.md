# Comparing `tmp/aiotiktok-2.6.1.tar.gz` & `tmp/aiotiktok-2.6.2.tar.gz`

## Comparing `aiotiktok-2.6.1.tar` & `aiotiktok-2.6.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 aiotiktok-2.6.1/aiotiktok/__init__.py
--rw-r--r--   0        0        0     6472 2020-02-02 00:00:00.000000 aiotiktok-2.6.1/aiotiktok/client.py
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 aiotiktok-2.6.1/aiotiktok/constants.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 aiotiktok-2.6.1/aiotiktok/exceptions.py
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 aiotiktok-2.6.1/aiotiktok/extractors.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 aiotiktok-2.6.1/aiotiktok/types.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 aiotiktok-2.6.1/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 aiotiktok-2.6.1/LICENSE
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 aiotiktok-2.6.1/README.md
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 aiotiktok-2.6.1/pyproject.toml
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 aiotiktok-2.6.1/PKG-INFO
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 aiotiktok-2.6.2/aiotiktok/__init__.py
+-rw-r--r--   0        0        0     6574 2020-02-02 00:00:00.000000 aiotiktok-2.6.2/aiotiktok/client.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 aiotiktok-2.6.2/aiotiktok/constants.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 aiotiktok-2.6.2/aiotiktok/exceptions.py
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 aiotiktok-2.6.2/aiotiktok/extractors.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 aiotiktok-2.6.2/aiotiktok/types.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 aiotiktok-2.6.2/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 aiotiktok-2.6.2/LICENSE
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 aiotiktok-2.6.2/README.rst
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 aiotiktok-2.6.2/pyproject.toml
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 aiotiktok-2.6.2/PKG-INFO
```

### Comparing `aiotiktok-2.6.1/aiotiktok/client.py` & `aiotiktok-2.6.2/aiotiktok/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import json
 import re
 from urllib.parse import urlencode, urljoin
 
 from httpx import AsyncClient
 
-from .constants import (default_user_videos_params,
-                        static_unsigned_user_videos, static_user_videos_url)
+from .constants import (
+    default_user_videos_params,
+    static_unsigned_user_videos,
+    static_user_videos_url,
+)
 from .exceptions import URLUnavailable, VideoUnavailable
-from .extractors import (extract_data_from_html, extract_user_data,
-                         extract_video_data)
+from .extractors import extract_data_from_html, extract_user_data, extract_video_data
 from .types import Author, VideoData
 
 
 class Client:
     def __init__(self, signature_url: str = "http://127.0.0.1:8002/signature") -> None:
         self.signature_url = signature_url
         self.api_headers = {
             "user-agent": "com.ss.android.ugc.trill/2613 (Linux; U; Android 10; en_US; Pixel 4; "
-            "Build/QQ3A.200805.001; Cronet/58.0.2991.0)"
+                          "Build/QQ3A.200805.001; Cronet/58.0.2991.0)"
         }
         self.base_url = "https://www.tiktok.com/"
         self.api_url = (
             "https://api16-normal-c-useast1a.tiktokv.com/aweme/v1/feed/?aweme_id={}"
         )
         self.headers = {
             "Accept-Encoding": "gzip, deflate",
@@ -33,15 +35,15 @@
         self,
         url: str,
         method: str = "GET",
         params: dict | None = None,
         data: dict | str | None = None,
         headers: dict | None = None,
         allow_redirects: bool = True,
-    ):
+    ) -> dict:
         async with AsyncClient() as session:
             response = await session.request(
                 method=method,
                 url=url,
                 params=params,
                 data=data,
                 headers=headers,
@@ -50,26 +52,24 @@
             response_headers = response.headers
             try:
                 response = response.json()
             except json.decoder.JSONDecodeError:
                 response = response.read()
         return dict(response=response, headers=response_headers)
 
-    async def get_video_id(self, url: str):
-        if "@" in url:
-            pass
-        else:
+    async def get_video_id(self, url: str) -> str:
+        if "@" not in url:
             headers = (await self._request(url, allow_redirects=False)).get("headers")
             url = headers.get("Location").split("?")[0]
         if url == self.base_url or "video" not in url:
             raise URLUnavailable("URLUnavailable, check the link")
-        video_id = re.findall("/video/(\d+)?", url)[0]
+        video_id = re.findall("/video/(\d+)", url)[0]
         return video_id
 
-    async def get_data(
+    async def video_data(
         self, url: str | None = None, video_id: str | int | None = None
     ) -> VideoData:
         """
         Get TikTok data
         :param video_id: id of video:
         :param url: url to video
         :return: :class:`aiotiktok.types.VideoData`
@@ -84,46 +84,46 @@
         )
         if data and data.get("aweme_id") == str(video_id):
             return extract_video_data(data)
         raise VideoUnavailable("VideoUnavailable")
 
     async def user_feed(self, username: str, count: int = None) -> list[VideoData]:
         """
-        Get User Feed
+        Get user feed, only 30 videos.
         :param username:
         :param count:
         :return: list[:class:`aiotiktok.types.VideoData`]
         """
         url = urljoin(self.base_url, f"@{username}")
         response = await self._request(url, headers=self.headers)
         data = extract_data_from_html(response.get("response").decode())
         item_module = data.get("ItemModule")
         videos = []
         for video in list(item_module.values())[:count]:
-            videos.append(await self.get_data(video_id=video.get("id")))
+            videos.append(await self.video_data(video_id=video.get("id")))
         return videos
 
     async def user_info(self, username: str) -> Author:
         """
         Get UserInfo
         :param username:
-        :return:
+        :return :class:`aiotiktok.types.Author`:
         """
         url = urljoin(self.base_url, f"@{username}")
         response = await self._request(url, headers=self.headers)
         data = extract_data_from_html(response.get("response").decode())
         return extract_user_data(data)
 
-    async def sign_url(self, url: str):
+    async def sign_url(self, url: str) -> dict:
         request = await self._request(
             url=self.signature_url, method="POST", data={"url": url}
         )
         return request.get("response", {})
 
-    async def _get_user_feed_private(self, username: str, count: int | None = None):
+    async def _get_user_feed_private(self, username: str, count: int | None = None) -> list[dict]:
         sec_uid = (await self.user_info(username)).sec_uid
         params = default_user_videos_params
         params.update({"secUid": sec_uid})
         unsigned_url = f"{static_unsigned_user_videos}{urlencode(params)}"
         signature_data = await self.sign_url(unsigned_url)
         headers = {
             "x-tt-params": signature_data.get("x-tt-params"),
@@ -143,20 +143,20 @@
             api_response = (
                 await self._request(url=static_user_videos_url, headers=headers)
             ).get("response")
             user_videos.extend(api_response.get("itemList"))
             has_more = api_response.get("hasMore")
         return user_videos
 
-    async def user_feed_sig(self, username: str, count: int | None = None):
+    async def user_feed_sig(self, username: str, count: int | None = None) -> list[VideoData]:
         """
         Get user feed with private signature, for use that method you must up your application
         https://github.com/sheldygg/aiotiktok#signature
         :param username:
         :param count:
-        :return:
+        :return: list[:class:`aiotiktok.types.VideoData`]
         """
         videos = []
         user_videos = (await self._get_user_feed_private(username))[:count]
         for video in user_videos:
-            videos.append(await self.get_data(video_id=video.get("id")))
+            videos.append(await self.video_data(video_id=video.get("id")))
         return videos
```

### Comparing `aiotiktok-2.6.1/aiotiktok/constants.py` & `aiotiktok-2.6.2/aiotiktok/constants.py`

 * *Files identical despite different names*

### Comparing `aiotiktok-2.6.1/aiotiktok/extractors.py` & `aiotiktok-2.6.2/aiotiktok/extractors.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 import json
 import re
 
-from .types import Album, Author, Video, VideoData, VideoType, video_type_codes
+from .types import Album, Author, Music, Video, VideoData, VideoType, video_type_codes
 
 
 def extract_video_data(data: dict) -> VideoData:
     video_type = video_type_codes.get(data["aweme_type"], VideoType.VIDEO)
     if video_type == VideoType.ALBUM:
         images_list = []
         for images in data["image_post_info"]["images"]:
             images_list.append(images["display_image"]["url_list"][0])
         media = Album(urls=images_list)
     else:
         media = Video(url=data["video"]["play_addr"]["url_list"][0])
     author_data = data.get("author")
-    author = Author(
-        id=author_data.get("id"),
-        nickname=author_data.get("nickname"),
-        unique_id=author_data.get("unique_id"),
-        avatar=author_data.get("avatar_larger", {}).get("url_list")[0],
-    )
     return VideoData(
         video_type=video_type,
         media=media,
         cover=data["video"]["cover"]["url_list"][0],
         dynamic_cover=data["video"]["dynamic_cover"]["url_list"][0],
         description=data["desc"],
         play_count=data["statistics"]["comment_count"],
         comment_count=data["statistics"]["comment_count"],
         download_count=data["statistics"]["download_count"],
         share_count=data["statistics"]["share_count"],
         create_time=data["create_time"],
-        author=author,
-        music_title=data["music"]["title"],
-        music_author=data["music"]["author"],
-        music_url=data["music"]["play_url"]["uri"],
-        music_cover=data["music"]["cover_large"]["url_list"][0],
+        author=Author(
+            id=author_data.get("id"),
+            nickname=author_data.get("nickname"),
+            unique_id=author_data.get("unique_id"),
+            avatar=author_data.get("avatar_larger", {}).get("url_list")[0],
+        ),
+        music=Music(
+            title=data["music"]["title"],
+            author=data["music"]["author"],
+            url=data["music"]["play_url"]["uri"],
+            cover=data["music"]["cover_large"]["url_list"][0],
+        ),
     )
 
 
 def extract_data_from_html(data: str):
     pattern = r'<script id="SIGI_STATE" type="application\/json">(.*?)<\/script>'
     match = re.search(pattern, data, re.S)
     return json.loads(match.group(1))
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_o_syankm_/tmpn6auuqqu_TarContainer/0/4.py", line 57, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_o_syankm_/tmpn6auuqqu_TarContainer/0/4.py", line 57, column 0: CDATA terminal not found*

```diff
@@ -1,19 +1,19 @@
-import json import re from .types import Album, Author, Video, VideoData,
-VideoType, video_type_codes def extract_video_data(data: dict) -> VideoData:
-video_type = video_type_codes.get(data["aweme_type"], VideoType.VIDEO) if
-video_type == VideoType.ALBUM: images_list = [] for images in data
-["image_post_info"]["images"]: images_list.append(images["display_image"]
-["url_list"][0]) media = Album(urls=images_list) else: media = Video(url=data
-["video"]["play_addr"]["url_list"][0]) author_data = data.get("author") author
-= Author( id=author_data.get("id"), nickname=author_data.get("nickname"),
+import json import re from .types import Album, Author, Music, Video,
+VideoData, VideoType, video_type_codes def extract_video_data(data: dict) -
+> VideoData: video_type = video_type_codes.get(data["aweme_type"],
+VideoType.VIDEO) if video_type == VideoType.ALBUM: images_list = [] for images
+in data["image_post_info"]["images"]: images_list.append(images
+["display_image"]["url_list"][0]) media = Album(urls=images_list) else: media =
+Video(url=data["video"]["play_addr"]["url_list"][0]) author_data = data.get
+("author") return VideoData( video_type=video_type, media=media, cover=data
+["video"]["cover"]["url_list"][0], dynamic_cover=data["video"]["dynamic_cover"]
+["url_list"][0], description=data["desc"], play_count=data["statistics"]
+["comment_count"], comment_count=data["statistics"]["comment_count"],
+download_count=data["statistics"]["download_count"], share_count=data
+["statistics"]["share_count"], create_time=data["create_time"], author=Author
+( id=author_data.get("id"), nickname=author_data.get("nickname"),
 unique_id=author_data.get("unique_id"), avatar=author_data.get("avatar_larger",
-{}).get("url_list")[0], ) return VideoData( video_type=video_type, media=media,
-cover=data["video"]["cover"]["url_list"][0], dynamic_cover=data["video"]
-["dynamic_cover"]["url_list"][0], description=data["desc"], play_count=data
-["statistics"]["comment_count"], comment_count=data["statistics"]
-["comment_count"], download_count=data["statistics"]["download_count"],
-share_count=data["statistics"]["share_count"], create_time=data["create_time"],
-author=author, music_title=data["music"]["title"], music_author=data["music"]
-["author"], music_url=data["music"]["play_url"]["uri"], music_cover=data
-["music"]["cover_large"]["url_list"][0], ) def extract_data_from_html(data:
-str): pattern = r'
+{}).get("url_list")[0], ), music=Music( title=data["music"]["title"],
+author=data["music"]["author"], url=data["music"]["play_url"]["uri"],
+cover=data["music"]["cover_large"]["url_list"][0], ), ) def
+extract_data_from_html(data: str): pattern = r'
```

### Comparing `aiotiktok-2.6.1/aiotiktok/types.py` & `aiotiktok-2.6.2/aiotiktok/types.py`

 * *Files 17% similar despite different names*

```diff
@@ -31,26 +31,27 @@
     id: str
     unique_id: str
     nickname: str
     sec_uid: str | None = None
     avatar: str
 
 
+class Music(Struct):
+    title: str
+    author: str
+    url: str
+    cover: str
+
+
 class VideoData(Struct):
-    video_type: str
+    video_type: VideoType
     media: Video | Album
     cover: str
     dynamic_cover: str
     description: str
     play_count: int
     comment_count: int
     download_count: int
     share_count: int
     create_time: datetime
     author: Author
-    # author_name: str
-    # author_nick: str
-    # author_pic: str
-    music_title: str
-    music_author: str
-    music_url: str
-    music_cover: str
+    music: Music
```

### Comparing `aiotiktok-2.6.1/.gitignore` & `aiotiktok-2.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `aiotiktok-2.6.1/LICENSE` & `aiotiktok-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotiktok-2.6.1/pyproject.toml` & `aiotiktok-2.6.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -2,31 +2,38 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aiotiktok"
 dynamic = ["version"]
 description = "Tool for parse tiktok data"
-readme = "README.md"
+readme = "README.rst"
 license = "MIT"
 authors = [
     { name = "sheldy" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
     "httpx",
     "msgspec",
 ]
 
+[project.optional-dependencies]
+signature = [
+    "tiktok-signature"
+]
+
 [project.urls]
 Homepage = "https://github.com/sheldygg/aiotiktok"
 
 [tool.hatch.version]
 path = "aiotiktok/__init__.py"
 
 [tool.hatch.build.targets.sdist]
 include = [
     "/aiotiktok",
 ]
+[tool.isort]
+profile = "black"
```

### Comparing `aiotiktok-2.6.1/PKG-INFO` & `aiotiktok-2.6.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,76 @@
 Metadata-Version: 2.1
 Name: aiotiktok
-Version: 2.6.1
+Version: 2.6.2
 Summary: Tool for parse tiktok data
 Project-URL: Homepage, https://github.com/sheldygg/aiotiktok
 Author: sheldy
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: httpx
 Requires-Dist: msgspec
-Description-Content-Type: text/markdown
+Provides-Extra: signature
+Requires-Dist: tiktok-signature; extra == 'signature'
+Description-Content-Type: text/x-rst
 
-# aiotiktok
+####################
+aiotiktok
+####################
 
-[![PyPi Package Version](https://img.shields.io/pypi/v/aiotiktok?color=blue)](https://pypi.org/project/aiotiktok/)
-[![Downloads](https://img.shields.io/pypi/dm/aiotiktok?color=blue)](https://pypi.org/project/aiotiktok/)
+.. image:: https://img.shields.io/pypi/v/aiotiktok?color=blue
+    :target: https://pypi.python.org/pypi/aiotiktok
+    :alt: PyPi Package Version
 
-**aiotiktok** super simple and fast library to get all video data from TikTok
+.. image:: https://img.shields.io/pypi/dm/aiotiktok?color=blue
+    :target: https://pypi.python.org/pypi/aiotiktok
+    :alt: Downloads
 
+**aiotiktok** is super simple and fast library
+to get all video data from TikTok
 
-**One step before start.**
-- You must install a library with pip `pip install aiotiktok`
+Simple Request
+==============
 
-### Request
+.. code-block:: python
 
-```python
-import asyncio
-from aiotiktok import Client
+   import asyncio
+   from aiotiktok import Client
 
-tiktok = Client()
+   tiktok = Client()
 
-async def main():
-    data = await tiktok.get_data(url="some url")
-    print(data)
-    
-asyncio.run(main())
-```
 
-### Signature
+   async def main():
+       await tiktok.get_data(url="some url")
+
+
+   asyncio.run(main())
+
+Signature
+=========
 
 **For use method user_feed_sig you must up your application.**
 
 This must be done in order to be able to generate a signature for a request to the private TikTok api
 
 Follow this instruction https://github.com/sheldygg/tiktok-signature
 
 After you have run it, you must specify a reference when initializing the Client class
-```python
-from aiotiktok import Client
 
-tiktok = Client(signature_url="your url")
-```
-By default is http://127.0.0.1/signature
+.. code-block:: python
+
+    from aiotiktok import Client
+
+    tiktok = Client(signature_url="some url")
+
+By default is http://127.0.0.1:8002/signature
 
 Then you can get user feed
-```python
-from aiotiktok import Client
 
-tiktok = Client()
+.. code-block:: python
+
+    from aiotiktok import Client
+
+    tiktok = Client()
 
-await tiktok.user_feed_sig("playboicarti")
-```
+    await tiktok.user_feed_sig("playboicarti")
```

