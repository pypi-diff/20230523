# Comparing `tmp/ichika-0.0.6.tar.gz` & `tmp/ichika-0.0.7.tar.gz`

## Comparing `ichika-0.0.6.tar` & `ichika-0.0.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      253 1970-01-01 00:00:00.000000 ichika-0.0.6/local_dependencies/pyo3-repr/Cargo.toml
--rw-r--r--   0     1001      123     4379 2023-05-13 14:38:16.000000 ichika-0.0.6/local_dependencies/pyo3-repr/src/lib.rs
--rw-r--r--   0        0        0      177 1970-01-01 00:00:00.000000 ichika-0.0.6/local_dependencies/t544_enc/Cargo.toml
--rw-r--r--   0     1001      123       19 2023-05-13 14:38:24.000000 ichika-0.0.6/local_dependencies/t544_enc/src/lib.rs
--rw-r--r--   0     1001      123       86 2023-05-13 14:38:24.000000 ichika-0.0.6/local_dependencies/t544_enc/src/t544_sign.rs
--rw-r--r--   0        0        0     1471 1970-01-01 00:00:00.000000 ichika-0.0.6/Cargo.toml
--rw-r--r--   0     1001      123     2004 2023-05-13 14:38:16.000000 ichika-0.0.6/README.md
--rw-r--r--   0     1001      123     3028 2023-05-13 14:38:16.000000 ichika-0.0.6/pyproject.toml
--rw-r--r--   0     1001      123      231 2023-05-13 14:38:16.000000 ichika-0.0.6/python/ichika/__init__.py
--rw-r--r--   0     1001      123     1052 2023-05-13 14:38:16.000000 ichika-0.0.6/python/ichika/build_info.py
--rw-r--r--   0     1001      123     7580 2023-05-13 14:38:16.000000 ichika-0.0.6/python/ichika/client.py
--rw-r--r--   0     1001      123    19186 2023-05-13 14:38:16.000000 ichika-0.0.6/python/ichika/core.pyi
--rw-r--r--   0     1001      123     4138 2023-05-13 14:38:16.000000 ichika-0.0.6/python/ichika/event_defs.py
--rw-r--r--   0     1001      123      266 2023-05-13 14:38:16.000000 ichika-0.0.6/python/ichika/exceptions.py
--rw-r--r--   0     1001      123     6253 2023-05-13 14:38:16.000000 ichika-0.0.6/python/ichika/graia/__init__.py
--rw-r--r--   0     1001      123     7214 2023-05-13 14:38:16.000000 ichika-0.0.6/python/ichika/graia/event.py
--rw-r--r--   0     1001      123     4541 2023-05-13 14:38:16.000000 ichika-0.0.6/python/ichika/login/__init__.py
--rw-r--r--   0     1001      123     3864 2023-05-13 14:38:16.000000 ichika-0.0.6/python/ichika/login/password.py
--rw-r--r--   0     1001      123     4115 2023-05-13 14:38:16.000000 ichika-0.0.6/python/ichika/login/qrcode/__init__.py
--rw-r--r--   0     1001      123      249 2023-05-13 14:38:16.000000 ichika-0.0.6/python/ichika/login/qrcode/render/__init__.py
--rw-r--r--   0     1001      123      794 2023-05-13 14:38:16.000000 ichika-0.0.6/python/ichika/login/qrcode/render/dense1x2.py
--rw-r--r--   0     1001      123     1017 2023-05-13 14:38:16.000000 ichika-0.0.6/python/ichika/message/__init__.py
--rw-r--r--   0     1001      123      290 2023-05-13 14:38:16.000000 ichika-0.0.6/python/ichika/message/_sealed.py
--rw-r--r--   0     1001      123     1935 2023-05-13 14:38:16.000000 ichika-0.0.6/python/ichika/message/_serializer.py
--rw-r--r--   0     1001      123    13577 2023-05-13 14:38:16.000000 ichika-0.0.6/python/ichika/message/elements.py
--rw-r--r--   0     1001      123        0 2023-05-13 14:38:16.000000 ichika-0.0.6/python/ichika/scripts/__init__.py
--rw-r--r--   0     1001      123     1227 2023-05-13 14:38:16.000000 ichika-0.0.6/python/ichika/scripts/device/__init__.py
--rw-r--r--   0     1001      123     1903 2023-05-13 14:38:16.000000 ichika-0.0.6/python/ichika/scripts/device/converter.py
--rw-r--r--   0     1001      123     5163 2023-05-13 14:38:16.000000 ichika-0.0.6/python/ichika/scripts/device/data.json
--rw-r--r--   0     1001      123     2305 2023-05-13 14:38:16.000000 ichika-0.0.6/python/ichika/scripts/device/generator.py
--rw-r--r--   0     1001      123      741 2023-05-13 14:38:16.000000 ichika-0.0.6/python/ichika/structs.py
--rw-r--r--   0     1001      123     1934 2023-05-13 14:38:16.000000 ichika-0.0.6/python/ichika/utils.py
--rw-r--r--   0     1001      123     1036 2023-05-13 14:38:16.000000 ichika-0.0.6/src/build_info.rs
--rw-r--r--   0     1001      123     5602 2023-05-13 14:38:16.000000 ichika-0.0.6/src/client/cached.rs
--rw-r--r--   0     1001      123     1834 2023-05-13 14:38:16.000000 ichika-0.0.6/src/client/http.rs
--rw-r--r--   0     1001      123    26119 2023-05-13 14:38:16.000000 ichika-0.0.6/src/client/mod.rs
--rw-r--r--   0     1001      123     4489 2023-05-13 14:38:16.000000 ichika-0.0.6/src/client/params.rs
--rw-r--r--   0     1001      123    10304 2023-05-13 14:38:16.000000 ichika-0.0.6/src/client/structs.rs
--rw-r--r--   0     1001      123    12632 2023-05-13 14:38:16.000000 ichika-0.0.6/src/events/converter.rs
--rw-r--r--   0     1001      123     3897 2023-05-13 14:38:16.000000 ichika-0.0.6/src/events/mod.rs
--rw-r--r--   0     1001      123     2301 2023-05-13 14:38:16.000000 ichika-0.0.6/src/exc.rs
--rw-r--r--   0     1001      123     1895 2023-05-13 14:38:16.000000 ichika-0.0.6/src/lib.rs
--rw-r--r--   0     1001      123     1779 2023-05-13 14:38:16.000000 ichika-0.0.6/src/login/connector.rs
--rw-r--r--   0     1001      123    20578 2023-05-13 14:38:16.000000 ichika-0.0.6/src/login/mod.rs
--rw-r--r--   0     1001      123     6625 2023-05-13 14:38:16.000000 ichika-0.0.6/src/loguru.rs
--rw-r--r--   0     1001      123    10122 2023-05-13 14:38:16.000000 ichika-0.0.6/src/message/convert.rs
--rw-r--r--   0     1001      123     1667 2023-05-13 14:38:16.000000 ichika-0.0.6/src/message/elements.rs
--rw-r--r--   0     1001      123       35 2023-05-13 14:38:16.000000 ichika-0.0.6/src/message/mod.rs
--rw-r--r--   0     1001      123     5649 2023-05-13 14:38:16.000000 ichika-0.0.6/src/utils.rs
--rw-r--r--   0     1001      123    57725 2023-05-13 14:38:47.000000 ichika-0.0.6/Cargo.lock
--rw-r--r--   0        0        0     3388 1970-01-01 00:00:00.000000 ichika-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      253 1970-01-01 00:00:00.000000 ichika-0.0.7/local_dependencies/pyo3-repr/Cargo.toml
+-rw-r--r--   0     1001      123     4379 2023-05-23 10:09:26.000000 ichika-0.0.7/local_dependencies/pyo3-repr/src/lib.rs
+-rw-r--r--   0        0        0      177 1970-01-01 00:00:00.000000 ichika-0.0.7/local_dependencies/t544_enc/Cargo.toml
+-rw-r--r--   0     1001      123       19 2023-05-23 10:09:37.000000 ichika-0.0.7/local_dependencies/t544_enc/src/lib.rs
+-rw-r--r--   0     1001      123       86 2023-05-23 10:09:37.000000 ichika-0.0.7/local_dependencies/t544_enc/src/t544_sign.rs
+-rw-r--r--   0        0        0     1471 1970-01-01 00:00:00.000000 ichika-0.0.7/Cargo.toml
+-rw-r--r--   0     1001      123     2004 2023-05-23 10:09:26.000000 ichika-0.0.7/README.md
+-rw-r--r--   0     1001      123     3077 2023-05-23 10:09:26.000000 ichika-0.0.7/pyproject.toml
+-rw-r--r--   0     1001      123      231 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/__init__.py
+-rw-r--r--   0     1001      123     1052 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/build_info.py
+-rw-r--r--   0     1001      123     7580 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/client.py
+-rw-r--r--   0     1001      123    19186 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/core.pyi
+-rw-r--r--   0     1001      123     4138 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/event_defs.py
+-rw-r--r--   0     1001      123      266 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/exceptions.py
+-rw-r--r--   0     1001      123     6253 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/graia/__init__.py
+-rw-r--r--   0     1001      123     7214 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/graia/event.py
+-rw-r--r--   0     1001      123     4832 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/login/__init__.py
+-rw-r--r--   0     1001      123     3864 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/login/password.py
+-rw-r--r--   0     1001      123     4115 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/login/qrcode/__init__.py
+-rw-r--r--   0     1001      123      249 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/login/qrcode/render/__init__.py
+-rw-r--r--   0     1001      123      794 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/login/qrcode/render/dense1x2.py
+-rw-r--r--   0     1001      123     1017 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/message/__init__.py
+-rw-r--r--   0     1001      123      290 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/message/_sealed.py
+-rw-r--r--   0     1001      123     1935 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/message/_serializer.py
+-rw-r--r--   0     1001      123    13966 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/message/elements.py
+-rw-r--r--   0     1001      123        0 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/scripts/__init__.py
+-rw-r--r--   0     1001      123     1227 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/scripts/device/__init__.py
+-rw-r--r--   0     1001      123     1903 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/scripts/device/converter.py
+-rw-r--r--   0     1001      123     5163 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/scripts/device/data.json
+-rw-r--r--   0     1001      123     2305 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/scripts/device/generator.py
+-rw-r--r--   0     1001      123      741 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/structs.py
+-rw-r--r--   0     1001      123     1934 2023-05-23 10:09:26.000000 ichika-0.0.7/python/ichika/utils.py
+-rw-r--r--   0     1001      123     1036 2023-05-23 10:09:26.000000 ichika-0.0.7/src/build_info.rs
+-rw-r--r--   0     1001      123     5602 2023-05-23 10:09:26.000000 ichika-0.0.7/src/client/cached.rs
+-rw-r--r--   0     1001      123     1834 2023-05-23 10:09:26.000000 ichika-0.0.7/src/client/http.rs
+-rw-r--r--   0     1001      123    26119 2023-05-23 10:09:26.000000 ichika-0.0.7/src/client/mod.rs
+-rw-r--r--   0     1001      123     4489 2023-05-23 10:09:26.000000 ichika-0.0.7/src/client/params.rs
+-rw-r--r--   0     1001      123    10304 2023-05-23 10:09:26.000000 ichika-0.0.7/src/client/structs.rs
+-rw-r--r--   0     1001      123    12632 2023-05-23 10:09:26.000000 ichika-0.0.7/src/events/converter.rs
+-rw-r--r--   0     1001      123     4919 2023-05-23 10:09:26.000000 ichika-0.0.7/src/events/mod.rs
+-rw-r--r--   0     1001      123     2301 2023-05-23 10:09:26.000000 ichika-0.0.7/src/exc.rs
+-rw-r--r--   0     1001      123     1895 2023-05-23 10:09:26.000000 ichika-0.0.7/src/lib.rs
+-rw-r--r--   0     1001      123     1779 2023-05-23 10:09:26.000000 ichika-0.0.7/src/login/connector.rs
+-rw-r--r--   0     1001      123    21393 2023-05-23 10:09:26.000000 ichika-0.0.7/src/login/mod.rs
+-rw-r--r--   0     1001      123     6625 2023-05-23 10:09:26.000000 ichika-0.0.7/src/loguru.rs
+-rw-r--r--   0     1001      123    10122 2023-05-23 10:09:26.000000 ichika-0.0.7/src/message/convert.rs
+-rw-r--r--   0     1001      123     1667 2023-05-23 10:09:26.000000 ichika-0.0.7/src/message/elements.rs
+-rw-r--r--   0     1001      123       35 2023-05-23 10:09:26.000000 ichika-0.0.7/src/message/mod.rs
+-rw-r--r--   0     1001      123     5649 2023-05-23 10:09:26.000000 ichika-0.0.7/src/utils.rs
+-rw-r--r--   0     1001      123    57725 2023-05-23 10:10:05.000000 ichika-0.0.7/Cargo.lock
+-rw-r--r--   0        0        0     3388 1970-01-01 00:00:00.000000 ichika-0.0.7/PKG-INFO
```

### Comparing `ichika-0.0.6/local_dependencies/pyo3-repr/src/lib.rs` & `ichika-0.0.7/local_dependencies/pyo3-repr/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ichika-0.0.6/Cargo.toml` & `ichika-0.0.7/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "ichika"
 authors = ["BlueGlassBlock <blueglassblock@outlook.com>"]
-version = "0.0.6"
+version = "0.0.7"
 license = "AGPL-3.0"
 edition = "2021"
 include = [
     "/python",
     "/src",
     "Cargo.lock",
     "pyproject.toml",
```

### Comparing `ichika-0.0.6/README.md` & `ichika-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ichika-0.0.6/pyproject.toml` & `ichika-0.0.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -121,10 +121,10 @@
 dev = [
     "maturin>=0.14.16",
     "pip>=23.0.1",
     "graia-saya>=0.0.17",
     "graiax-shortcut>=0.2.1",
 ]
 [tool.pdm.scripts]
-develop.cmd = "maturin develop"
+develop= {cmd = "pdm install -v", env = {MATURIN_PEP517_ARGS = "--profile dev"}}
 build-docs.cmd = "mkdocs build"
 view-docs.cmd = "mkdocs serve"
```

### Comparing `ichika-0.0.6/python/ichika/build_info.py` & `ichika-0.0.7/python/ichika/build_info.py`

 * *Files identical despite different names*

### Comparing `ichika-0.0.6/python/ichika/client.py` & `ichika-0.0.7/python/ichika/client.py`

 * *Files identical despite different names*

### Comparing `ichika-0.0.6/python/ichika/core.pyi` & `ichika-0.0.7/python/ichika/core.pyi`

 * *Files identical despite different names*

### Comparing `ichika-0.0.6/python/ichika/event_defs.py` & `ichika-0.0.7/python/ichika/event_defs.py`

 * *Files identical despite different names*

### Comparing `ichika-0.0.6/python/ichika/graia/__init__.py` & `ichika-0.0.7/python/ichika/graia/__init__.py`

 * *Files identical despite different names*

### Comparing `ichika-0.0.6/python/ichika/graia/event.py` & `ichika-0.0.7/python/ichika/graia/event.py`

 * *Files identical despite different names*

### Comparing `ichika-0.0.6/python/ichika/login/__init__.py` & `ichika-0.0.7/python/ichika/login/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,25 +31,31 @@
 
         return asdict(generate(Random(hash(protocol) ^ uin)))
 
 
 class PathCredentialStore(BaseLoginCredentialStore):
     """可以给所有账号共享的，基于路径的凭据存储器"""
 
-    def __init__(self, path: Union[str, os.PathLike[str]]) -> None:
+    def __init__(self, path: Union[str, os.PathLike[str]], device_name: str = "ricq_device.json") -> None:
+        """初始化
+
+        :param path: 存储路径
+        :param device_name: 设备信息文件名，可以使用 `{protocol}` 占位符，注意其为 PascalCase 格式
+        """
+        self.device_name = device_name
         self.path = Path(path)
         self.path.mkdir(parents=True, exist_ok=True)
 
     def uin_path(self, uin: int) -> Path:
         path = self.path / str(uin)
         path.mkdir(parents=True, exist_ok=True)
         return path
 
     def get_device(self, uin: int, protocol: str) -> dict:
-        ricq_device = self.uin_path(uin) / "ricq_device.json"
+        ricq_device = self.uin_path(uin) / self.device_name.format(protocol=protocol)
         if ricq_device.exists():
             log.info("发现 `ricq_device.json`, 读取")
             return json.loads(ricq_device.read_text("utf-8"))
 
         other_device = self.uin_path(uin) / "device.json"
         if other_device.exists():
             from dataclasses import asdict
```

### Comparing `ichika-0.0.6/python/ichika/login/password.py` & `ichika-0.0.7/python/ichika/login/password.py`

 * *Files identical despite different names*

### Comparing `ichika-0.0.6/python/ichika/login/qrcode/__init__.py` & `ichika-0.0.7/python/ichika/login/qrcode/__init__.py`

 * *Files identical despite different names*

### Comparing `ichika-0.0.6/python/ichika/login/qrcode/render/dense1x2.py` & `ichika-0.0.7/python/ichika/login/qrcode/render/dense1x2.py`

 * *Files identical despite different names*

### Comparing `ichika-0.0.6/python/ichika/message/__init__.py` & `ichika-0.0.7/python/ichika/message/__init__.py`

 * *Files identical despite different names*

### Comparing `ichika-0.0.6/python/ichika/message/_serializer.py` & `ichika-0.0.7/python/ichika/message/_serializer.py`

 * *Files identical despite different names*

### Comparing `ichika-0.0.6/python/ichika/message/elements.py` & `ichika-0.0.7/python/ichika/message/elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,15 +196,15 @@
     """未下载的合并转发消息，本质为 XML 卡片"""
 
     res_id: str
     """转发卡片的资源 ID"""
     file_name: str
     """转发卡片的子文件名"""
     content: str
-    """转发卡片的内容"""
+    """转发卡片的原始内容，可以为 XML 或 JSON 格式 (Android 8.9.50+?)"""
 
     def __str__(self) -> str:
         return "[合并转发]"
 
     async def download(self, client: __Client) -> list[ForwardMessage]:
         """使用 aiohttp 下载本转发卡片对应的转发消息
 
@@ -478,27 +478,33 @@
 
 
 def _light_app_deserializer(**data) -> Element:
     import json
     from contextlib import suppress
 
     with suppress(ValueError, KeyError):
+        app_data = json.loads(data["content"])
+        if app_data["app"] == "com.tencent.multimsg":
+            res_id = app_data["meta"]["resid"]
+            extra = json.loads(app_data["extra"])
+            return ForwardCard(res_id=res_id, file_name=extra["filename"], content=data["content"])
+
         # MusicShare resolver
         # https://github.com/mamoe/mirai/blob/893fb3e9f653623056f9c4bff73b4dac957cd2a2/mirai-core/src/commonMain/kotlin/message/data/lightApp.kt
-        app_data = json.loads(data["content"])
-        music_info = app_data["meta"]["music"]
-        return MusicShare(
-            kind=__MUSIC_SHARE_APPID_MAP[app_data["extra"]["appid"]],
-            title=music_info["title"],
-            summary=music_info["desc"],
-            jump_url=music_info["jumpUrl"],
-            picture_url=music_info["preview"],
-            music_url=music_info["musicUrl"],
-            brief=data["prompt"],
-        )
+        if "music" in app_data["meta"]:
+            music_info = app_data["meta"]["music"]
+            return MusicShare(
+                kind=__MUSIC_SHARE_APPID_MAP[app_data["extra"]["appid"]],
+                title=music_info["title"],
+                summary=music_info["desc"],
+                jump_url=music_info["jumpUrl"],
+                picture_url=music_info["preview"],
+                music_url=music_info["musicUrl"],
+                brief=data["prompt"],
+            )
 
     return LightApp(content=data["content"])
 
 
 __RES_ID_PAT = re.compile(r"m_resid=\"(.*?)\"")
 __FILE_NAME_PAT = re.compile(r"m_fileName=\"(.*?)\"")
```

### Comparing `ichika-0.0.6/python/ichika/scripts/device/__init__.py` & `ichika-0.0.7/python/ichika/scripts/device/__init__.py`

 * *Files identical despite different names*

### Comparing `ichika-0.0.6/python/ichika/scripts/device/converter.py` & `ichika-0.0.7/python/ichika/scripts/device/converter.py`

 * *Files identical despite different names*

### Comparing `ichika-0.0.6/python/ichika/scripts/device/data.json` & `ichika-0.0.7/python/ichika/scripts/device/data.json`

 * *Files identical despite different names*

### Comparing `ichika-0.0.6/python/ichika/scripts/device/generator.py` & `ichika-0.0.7/python/ichika/scripts/device/generator.py`

 * *Files identical despite different names*

### Comparing `ichika-0.0.6/python/ichika/structs.py` & `ichika-0.0.7/python/ichika/structs.py`

 * *Files identical despite different names*

### Comparing `ichika-0.0.6/python/ichika/utils.py` & `ichika-0.0.7/python/ichika/utils.py`

 * *Files identical despite different names*

### Comparing `ichika-0.0.6/src/build_info.rs` & `ichika-0.0.7/src/build_info.rs`

 * *Files identical despite different names*

### Comparing `ichika-0.0.6/src/client/cached.rs` & `ichika-0.0.7/src/client/cached.rs`

 * *Files identical despite different names*

### Comparing `ichika-0.0.6/src/client/http.rs` & `ichika-0.0.7/src/client/http.rs`

 * *Files identical despite different names*

### Comparing `ichika-0.0.6/src/client/mod.rs` & `ichika-0.0.7/src/client/mod.rs`

 * *Files identical despite different names*

### Comparing `ichika-0.0.6/src/client/params.rs` & `ichika-0.0.7/src/client/params.rs`

 * *Files identical despite different names*

### Comparing `ichika-0.0.6/src/client/structs.rs` & `ichika-0.0.7/src/client/structs.rs`

 * *Files identical despite different names*

### Comparing `ichika-0.0.6/src/events/converter.rs` & `ichika-0.0.7/src/events/converter.rs`

 * *Files identical despite different names*

### Comparing `ichika-0.0.6/src/events/mod.rs` & `ichika-0.0.7/src/events/mod.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 use async_trait::async_trait;
 use pyo3::exceptions::PyIndexError;
 use pyo3::prelude::*;
 use pyo3::types::*;
 use pyo3_asyncio::{into_future_with_locals, TaskLocals};
 use pyo3_repr::PyRepr;
+use ricq::client::event::DisconnectReason;
+use ricq::client::NetworkStatus;
 use ricq::handler::{Handler, QEvent};
 
 pub mod converter;
 
 use crate::utils::{datetime_from_ts, py_client_refs, py_try, py_use};
 
 #[pyclass(get_all, module = "ichika.core")]
@@ -54,14 +56,37 @@
     }
 }
 
 #[async_trait]
 impl Handler for PyHandler {
     async fn handle(&self, event: QEvent) {
         let event_repr = format!("{event:?}");
+        if let QEvent::ClientDisconnect(e) = event {
+            match e.inner {
+                DisconnectReason::Network => {
+                    tracing::error!("网络错误, 尝试重连");
+                }
+                DisconnectReason::Actively(net) => match net {
+                    NetworkStatus::Drop => {
+                        tracing::error!("意料之外的内存释放");
+                    }
+                    NetworkStatus::NetworkOffline => {
+                        tracing::error!("网络离线, 尝试重连");
+                    }
+                    NetworkStatus::KickedOffline => {
+                        tracing::error!("其他设备登录, 被踢下线");
+                    }
+                    NetworkStatus::MsfOffline => {
+                        tracing::error!("服务器强制下线");
+                    }
+                    _ => {}
+                },
+            }
+            return;
+        }
         let py_event = match self::converter::convert(event).await {
             Ok(obj) => obj,
             Err(e) => {
                 tracing::error!("转换事件失败: {}", event_repr);
                 py_use(|py| e.print_and_set_sys_last_vars(py));
                 return;
             }
```

### Comparing `ichika-0.0.6/src/exc.rs` & `ichika-0.0.7/src/exc.rs`

 * *Files identical despite different names*

### Comparing `ichika-0.0.6/src/lib.rs` & `ichika-0.0.7/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ichika-0.0.6/src/login/connector.rs` & `ichika-0.0.7/src/login/connector.rs`

 * *Files identical despite different names*

### Comparing `ichika-0.0.6/src/login/mod.rs` & `ichika-0.0.7/src/login/mod.rs`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     LoginSuccess,
     LoginUnknownStatus,
     QRCodeState,
 };
 use tokio::task::JoinHandle;
 
 use crate::events::PyHandler;
-use crate::exc::MapPyErr;
+use crate::exc::{MapPyErr, RICQError};
 use crate::utils::{partial, py_bytes, py_client_refs, py_future, py_try, py_use};
 use crate::{exc, import_call, PyRet};
 
 #[cfg(feature = "t544")]
 pub(crate) mod t544 {
     use bytes::{BufMut, Bytes, BytesMut};
     use ricq::Client;
@@ -40,15 +40,15 @@
         guid: Bytes,
         version: Bytes,
     }
 
     impl NativeT544Provider {
         async fn new(client: &Client) -> Self {
             let uin = client.uin().await;
-            let guid = client.device().await.guid();
+            let guid = client.engine.read().await.transport.sig.guid.clone();
             let version = client.version().await.sdk_version;
 
             Self {
                 uin,
                 guid,
                 version: Bytes::copy_from_slice(version.as_bytes()),
             }
@@ -578,18 +578,35 @@
                 ref sig,
                 ref image_data,
             }) => {
                 image_sig = sig.clone();
                 let qrcode_data = parse_qrcode(image_data)?;
                 invoke_cb(locals, &handle_getter, "DisplayQRCode", (qrcode_data,)).await?;
             }
-            QRCodeState::Confirmed(ricq::QRCodeConfirmed { uin, .. }) => {
+            QRCodeState::Confirmed(ricq::QRCodeConfirmed {
+                uin,
+                ref tmp_pwd,
+                ref tmp_no_pic_sig,
+                ref tgt_qr,
+                ..
+            }) => {
                 if uin == decl_uin {
-                    invoke_cb(locals, &handle_getter, "Success", (uin,)).await?;
-                    break;
+                    let mut login_resp = client
+                        .qrcode_login(tmp_pwd, tmp_no_pic_sig, tgt_qr)
+                        .await
+                        .py_res()?;
+                    if matches!(login_resp, LoginResponse::DeviceLockLogin(_)) {
+                        tracing::info!("账号 {} 尝试设备锁登录", uin);
+                        login_resp = client.device_lock_login().await.py_res()?;
+                    }
+                    if matches!(login_resp, LoginResponse::Success(_)) {
+                        invoke_cb(locals, &handle_getter, "Success", (uin,)).await?;
+                        break;
+                    }
+                    Err(RICQError::new_err(format!("登录失败: {login_resp:?}")))?;
                 }
                 invoke_cb(locals, &handle_getter, "UINMismatch", (decl_uin, uin)).await?;
                 resp = client.fetch_qrcode().await.py_res()?;
                 continue;
             }
         }
         sleep_until(st_time + Duration::from_secs_f64(interval)).await;
```

### Comparing `ichika-0.0.6/src/loguru.rs` & `ichika-0.0.7/src/loguru.rs`

 * *Files identical despite different names*

### Comparing `ichika-0.0.6/src/message/convert.rs` & `ichika-0.0.7/src/message/convert.rs`

 * *Files identical despite different names*

### Comparing `ichika-0.0.6/src/message/elements.rs` & `ichika-0.0.7/src/message/elements.rs`

 * *Files identical despite different names*

### Comparing `ichika-0.0.6/src/utils.rs` & `ichika-0.0.7/src/utils.rs`

 * *Files identical despite different names*

### Comparing `ichika-0.0.6/Cargo.lock` & `ichika-0.0.7/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -762,15 +762,15 @@
 dependencies = [
  "cxx",
  "cxx-build",
 ]
 
 [[package]]
 name = "ichika"
-version = "0.0.6"
+version = "0.0.7"
 dependencies = [
  "async-trait",
  "backon",
  "built",
  "bytes",
  "futures-util",
  "hex",
@@ -1526,15 +1526,15 @@
 version = "0.6.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
 
 [[package]]
 name = "ricq"
 version = "0.1.20"
-source = "git+https://github.com/BlueGlassBlock/ricq.git?branch=ichika-snapshot#ef8f04b90abe22c612ad5ecf3ee7f2d3c998400d"
+source = "git+https://github.com/BlueGlassBlock/ricq.git?branch=ichika-snapshot#c74e58e659095e2d2bc53d6be58f7bb6e899da50"
 dependencies = [
  "async-trait",
  "bytes",
  "cached",
  "derivative",
  "flate2",
  "futures-util",
@@ -1549,15 +1549,15 @@
  "tokio-util",
  "tracing",
 ]
 
 [[package]]
 name = "ricq-core"
 version = "0.1.20"
-source = "git+https://github.com/BlueGlassBlock/ricq.git?branch=ichika-snapshot#ef8f04b90abe22c612ad5ecf3ee7f2d3c998400d"
+source = "git+https://github.com/BlueGlassBlock/ricq.git?branch=ichika-snapshot#c74e58e659095e2d2bc53d6be58f7bb6e899da50"
 dependencies = [
  "byteorder",
  "bytes",
  "derivative",
  "flate2",
  "generic-array",
  "jcers",
```

### Comparing `ichika-0.0.6/PKG-INFO` & `ichika-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ichika
-Version: 0.0.6
+Version: 0.0.7
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Communications
 Classifier: Programming Language :: Python :: 3
```

