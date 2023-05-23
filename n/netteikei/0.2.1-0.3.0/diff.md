# Comparing `tmp/netteikei-0.2.1-py3-none-any.whl.zip` & `tmp/netteikei-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 6623 bytes, number of entries: 12
--rw-------  2.0 unx      131 b- defN 23-May-22 02:58 netteikei/__init__.py
--rw-------  2.0 unx     2679 b- defN 23-May-14 16:14 netteikei/core.py
+Zip file size: 6920 bytes, number of entries: 12
+-rw-------  2.0 unx      131 b- defN 23-May-23 11:17 netteikei/__init__.py
+-rw-------  2.0 unx     2755 b- defN 23-May-23 11:00 netteikei/core.py
 -rw-------  2.0 unx        0 b- defN 23-May-07 09:41 netteikei/py.typed
 -rw-------  2.0 unx     1297 b- defN 23-May-14 16:14 netteikei/typedefs.py
 -rw-------  2.0 unx        0 b- defN 23-May-07 13:53 netteikei/contrib/__init__.py
--rw-------  2.0 unx     2429 b- defN 23-May-20 16:10 netteikei/contrib/download.py
--rw-------  2.0 unx     1157 b- defN 23-May-20 16:09 netteikei/contrib/utils.py
--rw-------  2.0 unx     1068 b- defN 23-May-22 03:01 netteikei-0.2.1.dist-info/LICENSE
--rw-------  2.0 unx     1371 b- defN 23-May-22 03:01 netteikei-0.2.1.dist-info/METADATA
--rw-------  2.0 unx       92 b- defN 23-May-22 03:01 netteikei-0.2.1.dist-info/WHEEL
--rw-------  2.0 unx       10 b- defN 23-May-22 03:01 netteikei-0.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      949 b- defN 23-May-22 03:01 netteikei-0.2.1.dist-info/RECORD
-12 files, 11183 bytes uncompressed, 5029 bytes compressed:  55.0%
+-rw-------  2.0 unx     3072 b- defN 23-May-23 11:10 netteikei/contrib/download.py
+-rw-------  2.0 unx     1159 b- defN 23-May-23 10:16 netteikei/contrib/utils.py
+-rw-------  2.0 unx     1068 b- defN 23-May-23 11:18 netteikei-0.3.0.dist-info/LICENSE
+-rw-------  2.0 unx     1371 b- defN 23-May-23 11:18 netteikei-0.3.0.dist-info/METADATA
+-rw-------  2.0 unx       92 b- defN 23-May-23 11:18 netteikei-0.3.0.dist-info/WHEEL
+-rw-------  2.0 unx       10 b- defN 23-May-23 11:18 netteikei-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      949 b- defN 23-May-23 11:18 netteikei-0.3.0.dist-info/RECORD
+12 files, 11904 bytes uncompressed, 5326 bytes compressed:  55.3%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: netteikei/contrib/download.py
 Comment: 
 
 Filename: netteikei/contrib/utils.py
 Comment: 
 
-Filename: netteikei-0.2.1.dist-info/LICENSE
+Filename: netteikei-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: netteikei-0.2.1.dist-info/METADATA
+Filename: netteikei-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: netteikei-0.2.1.dist-info/WHEEL
+Filename: netteikei-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: netteikei-0.2.1.dist-info/top_level.txt
+Filename: netteikei-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: netteikei-0.2.1.dist-info/RECORD
+Filename: netteikei-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## netteikei/__init__.py

```diff
@@ -1,6 +1,6 @@
 from .core import Client, Handler
 from .typedefs import Request
 
 
-__version__ = "0.2.1"
+__version__ = "0.3.0"
 __all__ = ["Client", "Handler", "Request"]
```

## netteikei/core.py

```diff
@@ -1,9 +1,10 @@
 from abc import ABC, abstractmethod
 import asyncio
+from collections.abc import Iterable
 from contextvars import ContextVar
 from typing import Generic, TypeVar, final
 
 from aiohttp import ClientResponse, ClientSession
 
 from .typedefs import Request
 
@@ -20,18 +21,18 @@
     ctx
         Context variable possessing relevant data for making requests.
         The value is automatically set for each request.
 
     Methods
     -------
     create_request()
-        Returns the request URL and options to override the options set
-        in the underlying `aiohttp.ClientSession` instance. This method
-        is called before making each request.
-    process_response(resp)
+        Returns the request method, URL, and options to override the
+        options set in the underlying `aiohttp.ClientSession` instance.
+        This method is called before making each request.
+    process_response(res)
         Processes the `aiohttp.ClientResponse` instance received as its
         only argument into relevant data. This method is called after a
         request has been made.
     """
 
     ctx: ContextVar[_T] = ContextVar("ctx")
 
@@ -76,24 +77,24 @@
     async def _request(self, obj: _T) -> _R:
         async with self._sem:
             self._handler.ctx.set(obj)
             method, url, opts = await self._handler.create_request()
             async with self._session.request(method, url, **opts) as res:
                 return await self._handler.process_response(res)
 
-    async def gather(self, *objs: _T) -> list[_R]:
+    async def process(self, objs: Iterable[_T]) -> list[_R]:
         """Make multiple concurrent HTTP requests.
 
         Processes the given objects into relevant data using the provided
         `Handler` implementation.
 
         Parameters
         ----------
-        obj
-            Data required for making requests.
+        objs
+            Iterable containing data required for making requests.
 
         Returns
         -------
         list
             Results processed from the given data.
         """
         return await asyncio.gather(*(self._request(obj) for obj in objs))
```

## netteikei/contrib/download.py

```diff
@@ -8,76 +8,97 @@
 import tqdm
 
 from .. import Client, Handler, Request
 from ..typedefs import SessionOpts, StrOrURL
 from .utils import isfile, parse_name, parse_length, get_start_byte
 
 
-_DIR: ContextVar[Path] = ContextVar("dir")
+__all__ = ["download"]
+
+DOWNLOAD_DIR: ContextVar[Path] = ContextVar("dir")
 
 
 class DownloadAlreadyExists(Exception):
     
     def __init__(self, path: Path) -> None:
         self.path = path
 
     def __str__(self) -> str:
-        return f"'{self.path}' alredy exists"
+        return f"Download has already been saved in {self.path}."
 
 
 class DownloadInfo(NamedTuple):
     url: StrOrURL
     path: Path
     length: int | None
     start: int
 
     @classmethod
     async def find(cls, session: ClientSession, url: StrOrURL, /) -> Self:
         async with session.head(url, allow_redirects=True) as resp:
             name = parse_name(resp, "untitled")
             length = parse_length(resp.headers)
-            path = _DIR.get() / name
+            path = DOWNLOAD_DIR.get() / name
             start = await get_start_byte(resp.headers, path)
-            if await isfile(path) and start == length:
+
+            # Throw an error if the file already exists and isn't empty.
+            if await isfile(path) and 0 < start == length:
                 raise DownloadAlreadyExists(path)
+
             return cls(url, path, length, start)
 
 
 class DownloadHandler(Handler[DownloadInfo, None]):
 
     async def create_request(self) -> Request:
         info = self.ctx.get()
-        return Request.new(
-            url=info.url,
-            headers={"Range": f"bytes={info.start}-"}
-        )
+        # Don't send extra headers when starting a download from the beginning
+        # of a file.
+        headers = {} if info.start == 0 else {"Range": f"bytes={info.start}-"} 
+        return Request.new(url=info.url, headers=headers)
 
-    async def process_response(self, resp: ClientResponse) -> None:
+    async def process_response(self, res: ClientResponse) -> None:
         info = self.ctx.get()
-        async with resp, aiofiles.open(info.path, "ab") as fp:
+        async with res, aiofiles.open(info.path, "ab") as fp:
             with tqdm.tqdm(
                 total=info.length,
                 initial=info.start,
                 unit="B",
                 unit_scale=True,
                 unit_divisor=1024
             ) as bar:
-                async for chunk in resp.content.iter_any():
+                async for chunk in res.content.iter_any():
                     progress = await fp.write(chunk)
                     bar.update(progress)
 
 
 async def download(
     dir: Path,
     /,
     *urls: StrOrURL,
     limit: int = 3,
     **kwargs: Unpack[SessionOpts]
 ) -> None:
-    token = _DIR.set(dir)
+    """Asynchronously download files.
+
+    Parameters
+    ----------
+    dir
+        Directory where downloads will be stored.
+    *urls
+        URLs to download from.
+    **kwargs
+        initialization options for the underlying `aiohttp.ClientSession`.
+
+    Raises
+    ------
+    DownloadAlreadyExists
+        Raised when the file has already been downloaded.
+    """
+    token = DOWNLOAD_DIR.set(dir)
     async with ClientSession(**kwargs) as session:
         info = await asyncio.gather(
             *(DownloadInfo.find(session, url) for url in urls)
         )
         client = Client(session, DownloadHandler(), max_workers=limit)
-        await client.gather(*info)
-    _DIR.reset(token)
+        await client.process(info)
+    DOWNLOAD_DIR.reset(token)
```

## netteikei/contrib/utils.py

```diff
@@ -13,33 +13,34 @@
 
 _P = ParamSpec("_P")
 _R = TypeVar("_R")
 
 
 def wrap(fn: Callable[_P, _R]) -> Callable[_P, Awaitable[_R]]:
     @functools.wraps(fn)
-    async def inner(*args: _P.args, **kwargs: _P.kwargs) -> _R:
+    async def wrapper(*args: _P.args, **kwargs: _P.kwargs) -> _R:
         return await asyncio.to_thread(fn, *args, **kwargs)
-    return inner
+    return wrapper
 
 
 getsize = wrap(os.path.getsize)
 isfile = wrap(os.path.isfile)
 
 
-def parse_name(resp: ClientResponse, default: str) -> str:
-    if (s := resp.headers.get("Content-Disposition")) is None:
-        return resp.url.name
+def parse_name(res: ClientResponse, default: str) -> str:
+    if (s := res.headers.get("Content-Disposition")) is None:
+        return res.url.name
     else:
         if (name := pyrfc6266.parse_filename(s)) is None:
             return default
         return name
 
 
 def parse_length(headers: Headers) -> int | None:
     if (s := headers.get("Content-Length")) is not None:
         return int(s)
 
+
 async def get_start_byte(headers: Headers, file: Path) -> int:
     if headers.get("Accept-Ranges") == "bytes" and await isfile(file):
         return await getsize(file)
     return 0
```

## Comparing `netteikei-0.2.1.dist-info/LICENSE` & `netteikei-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `netteikei-0.2.1.dist-info/METADATA` & `netteikei-0.3.0.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netteikei
-Version: 0.2.1
+Version: 0.3.0
 Summary: Utility for making concurrent HTTP requests with aiohttp
 Home-page: https://github.com/fernofsigma/netteikei
 Author: FernOfSigma
 Author-email: fernofsigma@tuta.io
 License: MIT
 Project-URL: GitHub: issues, https://github.com/fernofsigma/netteikei/issues
 Project-URL: GitHub: repo, https://github.com/fernofsigma/netteikei
```

