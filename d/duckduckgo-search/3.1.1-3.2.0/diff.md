# Comparing `tmp/duckduckgo_search-3.1.1.tar.gz` & `tmp/duckduckgo_search-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckduckgo_search-3.1.1.tar", last modified: Sun May 21 20:18:22 2023, max compression
+gzip compressed data, was "duckduckgo_search-3.2.0.tar", last modified: Tue May 23 12:18:40 2023, max compression
```

## Comparing `duckduckgo_search-3.1.1.tar` & `duckduckgo_search-3.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:18:22.064579 duckduckgo_search-3.1.1/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-05-21 20:18:02.000000 duckduckgo_search-3.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    14528 2023-05-21 20:18:22.064579 duckduckgo_search-3.1.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    13413 2023-05-21 20:18:02.000000 duckduckgo_search-3.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:18:22.060578 duckduckgo_search-3.1.1/duckduckgo_search/
--rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-05-21 20:18:02.000000 duckduckgo_search-3.1.1/duckduckgo_search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-05-21 20:18:02.000000 duckduckgo_search-3.1.1/duckduckgo_search/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15809 2023-05-21 20:18:02.000000 duckduckgo_search-3.1.1/duckduckgo_search/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-05-21 20:18:02.000000 duckduckgo_search-3.1.1/duckduckgo_search/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    24680 2023-05-21 20:18:02.000000 duckduckgo_search-3.1.1/duckduckgo_search/duckduckgo_search.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-05-21 20:18:02.000000 duckduckgo_search-3.1.1/duckduckgo_search/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:18:22.064579 duckduckgo_search-3.1.1/duckduckgo_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14528 2023-05-21 20:18:22.000000 duckduckgo_search-3.1.1/duckduckgo_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-21 20:18:22.000000 duckduckgo_search-3.1.1/duckduckgo_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 20:18:22.000000 duckduckgo_search-3.1.1/duckduckgo_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-21 20:18:22.000000 duckduckgo_search-3.1.1/duckduckgo_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-21 20:18:22.000000 duckduckgo_search-3.1.1/duckduckgo_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-21 20:18:22.000000 duckduckgo_search-3.1.1/duckduckgo_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-21 20:18:02.000000 duckduckgo_search-3.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 20:18:22.064579 duckduckgo_search-3.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:18:22.064579 duckduckgo_search-3.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-21 20:18:02.000000 duckduckgo_search-3.1.1/tests/test_duckduckgo_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:18:40.041953 duckduckgo_search-3.2.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-05-23 12:18:23.000000 duckduckgo_search-3.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14676 2023-05-23 12:18:40.041953 duckduckgo_search-3.2.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13561 2023-05-23 12:18:23.000000 duckduckgo_search-3.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:18:40.041953 duckduckgo_search-3.2.0/duckduckgo_search/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-05-23 12:18:23.000000 duckduckgo_search-3.2.0/duckduckgo_search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-05-23 12:18:23.000000 duckduckgo_search-3.2.0/duckduckgo_search/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15809 2023-05-23 12:18:23.000000 duckduckgo_search-3.2.0/duckduckgo_search/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-05-23 12:18:23.000000 duckduckgo_search-3.2.0/duckduckgo_search/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25007 2023-05-23 12:18:23.000000 duckduckgo_search-3.2.0/duckduckgo_search/duckduckgo_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-05-23 12:18:23.000000 duckduckgo_search-3.2.0/duckduckgo_search/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:18:40.041953 duckduckgo_search-3.2.0/duckduckgo_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14676 2023-05-23 12:18:40.000000 duckduckgo_search-3.2.0/duckduckgo_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-23 12:18:40.000000 duckduckgo_search-3.2.0/duckduckgo_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 12:18:40.000000 duckduckgo_search-3.2.0/duckduckgo_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-23 12:18:40.000000 duckduckgo_search-3.2.0/duckduckgo_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-23 12:18:40.000000 duckduckgo_search-3.2.0/duckduckgo_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 12:18:40.000000 duckduckgo_search-3.2.0/duckduckgo_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-23 12:18:23.000000 duckduckgo_search-3.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 12:18:40.041953 duckduckgo_search-3.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:18:40.041953 duckduckgo_search-3.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-23 12:18:23.000000 duckduckgo_search-3.2.0/tests/test_duckduckgo_search.py
```

### Comparing `duckduckgo_search-3.1.1/LICENSE.md` & `duckduckgo_search-3.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.1.1/PKG-INFO` & `duckduckgo_search-3.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo_search
-Version: 3.1.1
+Version: 3.2.0
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -160,16 +160,18 @@
     wt-wt for No region
 ___
 </details>
 
 [Go To TOP](#TOP)
 
 ## Using proxy
-The site blocks ip for a few minutes if you send too many requests. In this case, you need to use a proxy.
-Also you can set a timeout if the proxy takes a long time to respond (default timeout=10).
+If you send too many requests the site blocks ip for up to one minute and DDGS will raise an exception 
+`requests.exceptions.HTTPError: 418 Client Error:  for url: https://duckduckgo.com/`.
+In this case, you need repeat again after a while or to use a proxy. 
+You can set a timeout if the proxy takes a long time to respond (default timeout=10).
 
 *1. The easiest way. Launch the Tor Browser*
 ```python3
 from duckduckgo_search import DDGS
 
 proxies = {
     "http": "socks5h://localhost:9150",
```

### Comparing `duckduckgo_search-3.1.1/README.md` & `duckduckgo_search-3.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -135,16 +135,18 @@
     wt-wt for No region
 ___
 </details>
 
 [Go To TOP](#TOP)
 
 ## Using proxy
-The site blocks ip for a few minutes if you send too many requests. In this case, you need to use a proxy.
-Also you can set a timeout if the proxy takes a long time to respond (default timeout=10).
+If you send too many requests the site blocks ip for up to one minute and DDGS will raise an exception 
+`requests.exceptions.HTTPError: 418 Client Error:  for url: https://duckduckgo.com/`.
+In this case, you need repeat again after a while or to use a proxy. 
+You can set a timeout if the proxy takes a long time to respond (default timeout=10).
 
 *1. The easiest way. Launch the Tor Browser*
 ```python3
 from duckduckgo_search import DDGS
 
 proxies = {
     "http": "socks5h://localhost:9150",
```

### Comparing `duckduckgo_search-3.1.1/duckduckgo_search/__init__.py` & `duckduckgo_search-3.2.0/duckduckgo_search/__init__.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.1.1/duckduckgo_search/cli.py` & `duckduckgo_search-3.2.0/duckduckgo_search/cli.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.1.1/duckduckgo_search/compat.py` & `duckduckgo_search-3.2.0/duckduckgo_search/compat.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.1.1/duckduckgo_search/duckduckgo_search.py` & `duckduckgo_search-3.2.0/duckduckgo_search/duckduckgo_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 
     def __init__(
         self,
         headers: Optional[Dict[str, str]] = None,
         proxies: Optional[Dict[str, str]] = None,
         timeout: int = 10,
     ) -> None:
-        self.headers = headers if headers else HEADERS
         self._session = requests.Session()
         self._session.headers.update(headers if headers else HEADERS)
         self._session.proxies.update(proxies if proxies else {})
         self._timeout = timeout
 
     def _get_url(self, method: str, url: str, **kwargs) -> Optional[Response]:
         for i in range(3):
@@ -60,18 +59,19 @@
                 resp = self._session.request(
                     method, url, timeout=self._timeout, **kwargs
                 )
                 if self._is_500_in_url(resp.url):
                     raise requests.HTTPError
                 resp.raise_for_status()
                 return resp
-            except (HTTPError, Timeout) as ex:
+            except Exception as ex:
                 logger.warning(f"_get_url() {url} {type(ex).__name__} {ex}")
-                if i < 2:
-                    sleep(2**i)
+                if i >= 2 or "418" in str(ex):
+                    raise ex
+                sleep(2**i)
         return None
 
     def _get_vqd(self, keywords: str) -> Optional[str]:
         """Get vqd value for a search query."""
         resp = self._get_url("POST", "https://duckduckgo.com", data={"q": keywords})
         if resp:
             for c1, c2 in (
@@ -115,16 +115,15 @@
         Yields:
             dict with search results.
 
         """
         assert keywords, "keywords is mandatory"
 
         vqd = self._get_vqd(keywords)
-        if not vqd:
-            return None
+        assert vqd, "error in getting vqd"
 
         safesearch_base = {"on": 1, "moderate": -1, "off": -2}
         payload = {
             "q": keywords,
             "l": region,
             "p": safesearch_base[safesearch.lower()],
             "s": 0,
@@ -141,37 +140,38 @@
             if resp is None:
                 break
             try:
                 page_data = resp.json().get("results", None)
             except (AttributeError, JSONDecodeError):
                 break
 
-            result_exists = False
-            for row in page_data:
-                if "n" in row:
-                    payload["s"] = row["n"].split("s=")[-1].split("&")[0]  # next page
-                href = row.get("u", None)
-                if (
-                    href
-                    and href not in cache
-                    and href != f"http://www.google.com/search?q={keywords}"
-                ):
-                    cache.add(href)
-                    body = self._normalize(row["a"])
-                    if body:
-                        result_exists = True
-                        yield {
-                            "title": self._normalize(row["t"]),
-                            "href": href,
-                            "body": body,
-                        }
-                elif result_exists is False:
+            if page_data:
+                result_exists = False
+                for row in page_data:
+                    if "n" in row:
+                        payload["s"] = row["n"].split("s=")[-1].split("&")[0]
+                    href = row.get("u", None)
+                    if (
+                        href
+                        and href not in cache
+                        and href != f"http://www.google.com/search?q={keywords}"
+                    ):
+                        cache.add(href)
+                        body = self._normalize(row["a"])
+                        if body:
+                            result_exists = True
+                            yield {
+                                "title": self._normalize(row["t"]),
+                                "href": href,
+                                "body": body,
+                            }
+                    elif result_exists is False:
+                        break
+                if result_exists is False:
                     break
-            if result_exists is False:
-                break
 
     def images(
         self,
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
@@ -202,16 +202,15 @@
         Yields:
             dict with image search results.
 
         """
         assert keywords, "keywords is mandatory"
 
         vqd = self._get_vqd(keywords)
-        if not vqd:
-            return None
+        assert vqd, "error in getting vqd"
 
         safesearch_base = {"on": 1, "moderate": 1, "off": -1}
         timelimit = f"time:{timelimit}" if timelimit else ""
         size = f"size:{size}" if size else ""
         color = f"color:{color}" if color else ""
         type_image = f"type:{type_image}" if type_image else ""
         layout = f"layout:{layout}" if layout else ""
@@ -233,34 +232,35 @@
                 break
             try:
                 resp_json = resp.json()
             except (AttributeError, JSONDecodeError):
                 break
 
             page_data = resp_json.get("results", None)
-            result_exists = False
-            for row in page_data:
-                image_url = row.get("image", None)
-                if image_url and image_url not in cache:
-                    cache.add(image_url)
-                    result_exists = True
-                    yield {
-                        "title": row["title"],
-                        "image": image_url,
-                        "thumbnail": row["thumbnail"],
-                        "url": row["url"],
-                        "height": row["height"],
-                        "width": row["width"],
-                        "source": row["source"],
-                    }
-            next = resp_json.get("next", None)
-            if next:
-                payload["s"] = next.split("s=")[-1].split("&")[0]
-            if next is None or result_exists is False:
-                break
+            if page_data:
+                result_exists = False
+                for row in page_data:
+                    image_url = row.get("image", None)
+                    if image_url and image_url not in cache:
+                        cache.add(image_url)
+                        result_exists = True
+                        yield {
+                            "title": row["title"],
+                            "image": image_url,
+                            "thumbnail": row["thumbnail"],
+                            "url": row["url"],
+                            "height": row["height"],
+                            "width": row["width"],
+                            "source": row["source"],
+                        }
+                next = resp_json.get("next", None)
+                if next:
+                    payload["s"] = next.split("s=")[-1].split("&")[0]
+                if next is None or result_exists is False:
+                    break
 
     def videos(
         self,
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
@@ -282,16 +282,15 @@
         Yields:
             dict with videos search results
 
         """
         assert keywords, "keywords is mandatory"
 
         vqd = self._get_vqd(keywords)
-        if not vqd:
-            return None
+        assert vqd, "error in getting vqd"
 
         safesearch_base = {"on": 1, "moderate": -1, "off": -2}
         timelimit = f"publishedAfter:{timelimit}" if timelimit else ""
         resolution = f"videoDefinition:{resolution}" if resolution else ""
         duration = f"videoDuration:{duration}" if duration else ""
         license_videos = f"videoLicense:{license_videos}" if license_videos else ""
         payload = {
@@ -346,16 +345,15 @@
         Yields:
             dict with news search results.
 
         """
         assert keywords, "keywords is mandatory"
 
         vqd = self._get_vqd(keywords)
-        if not vqd:
-            return None
+        assert vqd, "error in getting vqd"
 
         safesearch_base = {"on": 1, "moderate": -1, "off": -2}
         payload = {
             "l": region,
             "o": "json",
             "noamp": "1",
             "q": keywords,
@@ -535,16 +533,15 @@
         Yields:
             dict with maps search results
         """
 
         assert keywords, "keywords is mandatory"
 
         vqd = self._get_vqd(keywords)
-        if not vqd:
-            return None
+        assert vqd, "error in getting vqd"
 
         # if longitude and latitude are specified, skip the request about bbox to the nominatim api
         if latitude and longitude:
             lat_t = Decimal(latitude.replace(",", "."))
             lat_b = Decimal(latitude.replace(",", "."))
             lon_l = Decimal(longitude.replace(",", "."))
             lon_r = Decimal(longitude.replace(",", "."))
@@ -619,44 +616,45 @@
             if resp is None:
                 break
             try:
                 page_data = resp.json().get("results", [])
             except (AttributeError, JSONDecodeError):
                 break
 
-            for res in page_data:
-                result = MapsResult()
-                result.title = res["name"]
-                result.address = res["address"]
-                if f"{result.title} {result.address}" in cache:
-                    continue
-                else:
-                    cache.add(f"{result.title} {result.address}")
-                    result.country_code = res["country_code"]
-                    result.url = res["website"]
-                    result.phone = res["phone"]
-                    result.latitude = res["coordinates"]["latitude"]
-                    result.longitude = res["coordinates"]["longitude"]
-                    result.source = unquote(res["url"])
-                    if res["embed"]:
-                        result.image = res["embed"].get("image", "")
-                        result.links = res["embed"].get("third_party_links", "")
-                        result.desc = res["embed"].get("description", "")
-                    result.hours = res["hours"]
-                    yield result.__dict__
-
-            # divide the square into 4 parts and add to the queue
-            if len(page_data) >= 15:
-                lat_middle = (lat_t + lat_b) / 2
-                lon_middle = (lon_l + lon_r) / 2
-                bbox1 = (lat_t, lon_l, lat_middle, lon_middle)
-                bbox2 = (lat_t, lon_middle, lat_middle, lon_r)
-                bbox3 = (lat_middle, lon_l, lat_b, lon_middle)
-                bbox4 = (lat_middle, lon_middle, lat_b, lon_r)
-                work_bboxes.extendleft([bbox1, bbox2, bbox3, bbox4])
+            if page_data:
+                for res in page_data:
+                    result = MapsResult()
+                    result.title = res["name"]
+                    result.address = res["address"]
+                    if f"{result.title} {result.address}" in cache:
+                        continue
+                    else:
+                        cache.add(f"{result.title} {result.address}")
+                        result.country_code = res["country_code"]
+                        result.url = res["website"]
+                        result.phone = res["phone"]
+                        result.latitude = res["coordinates"]["latitude"]
+                        result.longitude = res["coordinates"]["longitude"]
+                        result.source = unquote(res["url"])
+                        if res["embed"]:
+                            result.image = res["embed"].get("image", "")
+                            result.links = res["embed"].get("third_party_links", "")
+                            result.desc = res["embed"].get("description", "")
+                        result.hours = res["hours"]
+                        yield result.__dict__
+
+                # divide the square into 4 parts and add to the queue
+                if len(page_data) >= 15:
+                    lat_middle = (lat_t + lat_b) / 2
+                    lon_middle = (lon_l + lon_r) / 2
+                    bbox1 = (lat_t, lon_l, lat_middle, lon_middle)
+                    bbox2 = (lat_t, lon_middle, lat_middle, lon_r)
+                    bbox3 = (lat_middle, lon_l, lat_b, lon_middle)
+                    bbox4 = (lat_middle, lon_middle, lat_b, lon_r)
+                    work_bboxes.extendleft([bbox1, bbox2, bbox3, bbox4])
 
     def translate(
         self,
         keywords: str,
         from_: Optional[str] = None,
         to: str = "en",
     ) -> Optional[dict]:
@@ -670,16 +668,15 @@
         Returns:
             dict with translated keywords.
         """
 
         assert keywords, "keywords is mandatory"
 
         vqd = self._get_vqd("translate")
-        if not vqd:
-            return None
+        assert vqd, "error in getting vqd"
 
         payload = {
             "vqd": vqd,
             "query": "translate",
             "from": from_,
             "to": to,
         }
```

### Comparing `duckduckgo_search-3.1.1/duckduckgo_search.egg-info/PKG-INFO` & `duckduckgo_search-3.2.0/duckduckgo_search.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo-search
-Version: 3.1.1
+Version: 3.2.0
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -160,16 +160,18 @@
     wt-wt for No region
 ___
 </details>
 
 [Go To TOP](#TOP)
 
 ## Using proxy
-The site blocks ip for a few minutes if you send too many requests. In this case, you need to use a proxy.
-Also you can set a timeout if the proxy takes a long time to respond (default timeout=10).
+If you send too many requests the site blocks ip for up to one minute and DDGS will raise an exception 
+`requests.exceptions.HTTPError: 418 Client Error:  for url: https://duckduckgo.com/`.
+In this case, you need repeat again after a while or to use a proxy. 
+You can set a timeout if the proxy takes a long time to respond (default timeout=10).
 
 *1. The easiest way. Launch the Tor Browser*
 ```python3
 from duckduckgo_search import DDGS
 
 proxies = {
     "http": "socks5h://localhost:9150",
```

### Comparing `duckduckgo_search-3.1.1/pyproject.toml` & `duckduckgo_search-3.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Internet :: WWW/HTTP :: Indexing/Search",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
     "click>=8.1.3",
-    "requests>=2.30.0",
+    "requests>=2.31.0",
 ]
 dynamic = ["version"]
 
 [project.urls]  # Optional
 "Homepage" = "https://github.com/deedy5/duckduckgo_search"
 
 [project.scripts]
```

### Comparing `duckduckgo_search-3.1.1/tests/test_duckduckgo_search.py` & `duckduckgo_search-3.2.0/tests/test_duckduckgo_search.py`

 * *Files identical despite different names*

