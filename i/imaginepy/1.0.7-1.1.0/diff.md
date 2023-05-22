# Comparing `tmp/imaginepy-1.0.7.tar.gz` & `tmp/imaginepy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imaginepy-1.0.7.tar", last modified: Wed May 17 20:39:56 2023, max compression
+gzip compressed data, was "imaginepy-1.1.0.tar", last modified: Mon May 22 22:10:40 2023, max compression
```

## Comparing `imaginepy-1.0.7.tar` & `imaginepy-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 20:39:56.353000 imaginepy-1.0.7/
--rw-rw-rw-   0        0        0    35823 2023-05-14 17:40:10.000000 imaginepy-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     4026 2023-05-17 20:39:56.352501 imaginepy-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3355 2023-05-14 18:30:19.000000 imaginepy-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 20:39:56.334000 imaginepy-1.0.7/imaginepy/
--rw-rw-rw-   0        0        0    25623 2023-05-17 20:37:40.000000 imaginepy-1.0.7/imaginepy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 20:39:56.351001 imaginepy-1.0.7/imaginepy.egg-info/
--rw-rw-rw-   0        0        0     4026 2023-05-17 20:39:56.000000 imaginepy-1.0.7/imaginepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-05-17 20:39:56.000000 imaginepy-1.0.7/imaginepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 20:39:56.000000 imaginepy-1.0.7/imaginepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-05-17 20:39:56.000000 imaginepy-1.0.7/imaginepy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-17 20:39:56.000000 imaginepy-1.0.7/imaginepy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 20:39:56.353000 imaginepy-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1017 2023-05-17 20:36:32.000000 imaginepy-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 22:10:40.261387 imaginepy-1.1.0/
+-rw-rw-rw-   0        0        0    35823 2023-05-14 17:40:10.000000 imaginepy-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     5009 2023-05-22 22:10:40.260381 imaginepy-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4338 2023-05-22 22:10:21.000000 imaginepy-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 22:10:40.238769 imaginepy-1.1.0/imaginepy/
+-rw-rw-rw-   0        0        0      127 2023-05-22 21:09:41.000000 imaginepy-1.1.0/imaginepy/__init__.py
+-rw-rw-rw-   0        0        0     6522 2023-05-22 21:09:25.000000 imaginepy-1.1.0/imaginepy/async_imagine.py
+-rw-rw-rw-   0        0        0    18638 2023-05-22 21:09:25.000000 imaginepy-1.1.0/imaginepy/constants.py
+-rw-rw-rw-   0        0        0     6988 2023-05-22 21:09:25.000000 imaginepy-1.1.0/imaginepy/sync_imagine.py
+drwxrwxrwx   0        0        0        0 2023-05-22 22:10:40.259881 imaginepy-1.1.0/imaginepy.egg-info/
+-rw-rw-rw-   0        0        0     5009 2023-05-22 22:10:40.000000 imaginepy-1.1.0/imaginepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2023-05-22 22:10:40.000000 imaginepy-1.1.0/imaginepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 22:10:40.000000 imaginepy-1.1.0/imaginepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-05-22 22:10:40.000000 imaginepy-1.1.0/imaginepy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-22 22:10:40.000000 imaginepy-1.1.0/imaginepy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 22:10:40.261387 imaginepy-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1017 2023-05-22 21:11:16.000000 imaginepy-1.1.0/setup.py
```

### Comparing `imaginepy-1.0.7/LICENSE` & `imaginepy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imaginepy-1.0.7/PKG-INFO` & `imaginepy-1.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,19 @@
-Metadata-Version: 2.1
-Name: imaginepy
-Version: 1.0.7
-Summary: Python library to create Art with AI.
-Home-page: https://github.com/ItsCEED/imaginepy
-Author: CEED
-Author-email: 
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Topic :: Utilities
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
 
 <img src="https://github.com/ItsCEED/ImaginePy-Midjourney-Free-Alternative/blob/main/docs/imagine_logo.gif" width="10%">
 
 **ImaginePy**
-
+<br>
+<img src="https://discordapp.com/api/guilds/1110314971012808774/widget.png?style=banner4" alt="Discord Banner 4"/>
+<br>
 <img src="https://img.shields.io/badge/python-3.7+-informational?style=plastic" alt="Python version">
 <img src="https://img.shields.io/github/release-date/ItsCEED/ImaginePy-Midjourney-Free-Alternative?style=plastic" alt="Release">
 <img src="https://img.shields.io/github/release/ItsCEED/ImaginePy-Midjourney-Free-Alternative?style=plastic" alt="Version">
+
 </div>
 
 ## Features
 
 - 🎨 Turn words into art
 - 👓 Choose from an array of art styles
 - 🔧 Adjust your masterpiece with creative controls!
@@ -60,16 +44,16 @@
 [hyugogirubato]: https://github.com/hyugogirubato/pyImagine
 
 ### From Source Code
 
 The following steps are instructions on download, preparing, and running the code under a Venv environment.
 You can skip steps 3-5 with a simple `python setup.py install` call instead, but you miss out on a wide array of benefits.
 
-1. `git clone https://github.com/ItsCEED/ImaginePy-Midjourney-Free-Alternative`
-2. `cd ImaginePy-Midjourney-Free-Alternative`
+1. `git clone https://github.com/ItsCEED/Imaginepy`
+2. `cd Imaginepy`
 3. `python -m venv env`
 4. `source env/bin/activate`
 5. `python setup.py install`
 
 As seen in Step 5, running the `imaginepy` executable is somewhat different to a normal PIP installation.
 See [Venv's Docs] on various ways of making calls under the virtual-environment.
 
@@ -111,14 +95,52 @@
     except Exception as e:
         print(f"An error occurred while writing the image to file: {e}")
 
 if __name__ == "__main__":
     main()
 ```
 
+Async version
+
+```python
+import asyncio
+from imaginepy import AsyncImagine, Style, Ratio
+
+
+async def main():
+    imagine = AsyncImagine()
+
+    img_data = await imagine.sdprem(
+        prompt="Woman sitting on a table, looking at the sky, seen from behind",
+        style=Style.ANIME_V2,
+        ratio=Ratio.RATIO_16X9
+    )
+
+    if img_data is None:
+        print("An error occurred while generating the image.")
+        return
+
+    img_data = await imagine.upscale(image=img_data)
+
+    if img_data is None:
+        print("An error occurred while upscaling the image.")
+        return
+
+    await imagine.close()
+    try:
+        with open("example.png", mode="wb") as img_file:
+            img_file.write(img_data)
+    except Exception as e:
+        print(f"An error occurred while writing the image to file: {e}")
+
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
+
 ## Credit
 
 - Imagine Icon &copy; Vyro AI & API
 - Original reverse and version by: [hyugogirubato]
 
 ## License
```

### Comparing `imaginepy-1.0.7/README.md` & `imaginepy-1.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,38 @@
+Metadata-Version: 2.1
+Name: imaginepy
+Version: 1.1.0
+Summary: Python library to create Art with AI.
+Home-page: https://github.com/ItsCEED/imaginepy
+Author: CEED
+Author-email: 
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Utilities
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="center">
 
 <img src="https://github.com/ItsCEED/ImaginePy-Midjourney-Free-Alternative/blob/main/docs/imagine_logo.gif" width="10%">
 
 **ImaginePy**
-
+<br>
+<img src="https://discordapp.com/api/guilds/1110314971012808774/widget.png?style=banner4" alt="Discord Banner 4"/>
+<br>
 <img src="https://img.shields.io/badge/python-3.7+-informational?style=plastic" alt="Python version">
 <img src="https://img.shields.io/github/release-date/ItsCEED/ImaginePy-Midjourney-Free-Alternative?style=plastic" alt="Release">
 <img src="https://img.shields.io/github/release/ItsCEED/ImaginePy-Midjourney-Free-Alternative?style=plastic" alt="Version">
+
 </div>
 
 ## Features
 
 - 🎨 Turn words into art
 - 👓 Choose from an array of art styles
 - 🔧 Adjust your masterpiece with creative controls!
@@ -41,16 +63,16 @@
 [hyugogirubato]: https://github.com/hyugogirubato/pyImagine
 
 ### From Source Code
 
 The following steps are instructions on download, preparing, and running the code under a Venv environment.
 You can skip steps 3-5 with a simple `python setup.py install` call instead, but you miss out on a wide array of benefits.
 
-1. `git clone https://github.com/ItsCEED/ImaginePy-Midjourney-Free-Alternative`
-2. `cd ImaginePy-Midjourney-Free-Alternative`
+1. `git clone https://github.com/ItsCEED/Imaginepy`
+2. `cd Imaginepy`
 3. `python -m venv env`
 4. `source env/bin/activate`
 5. `python setup.py install`
 
 As seen in Step 5, running the `imaginepy` executable is somewhat different to a normal PIP installation.
 See [Venv's Docs] on various ways of making calls under the virtual-environment.
 
@@ -92,14 +114,52 @@
     except Exception as e:
         print(f"An error occurred while writing the image to file: {e}")
 
 if __name__ == "__main__":
     main()
 ```
 
+Async version
+
+```python
+import asyncio
+from imaginepy import AsyncImagine, Style, Ratio
+
+
+async def main():
+    imagine = AsyncImagine()
+
+    img_data = await imagine.sdprem(
+        prompt="Woman sitting on a table, looking at the sky, seen from behind",
+        style=Style.ANIME_V2,
+        ratio=Ratio.RATIO_16X9
+    )
+
+    if img_data is None:
+        print("An error occurred while generating the image.")
+        return
+
+    img_data = await imagine.upscale(image=img_data)
+
+    if img_data is None:
+        print("An error occurred while upscaling the image.")
+        return
+
+    await imagine.close()
+    try:
+        with open("example.png", mode="wb") as img_file:
+            img_file.write(img_data)
+    except Exception as e:
+        print(f"An error occurred while writing the image to file: {e}")
+
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
+
 ## Credit
 
 - Imagine Icon &copy; Vyro AI & API
 - Original reverse and version by: [hyugogirubato]
 
 ## License
```

### Comparing `imaginepy-1.0.7/imaginepy/__init__.py` & `imaginepy-1.1.0/imaginepy/constants.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,8 @@
 from enum import Enum
-from typing import Any, Optional, Tuple
-from requests import Session, Response
-from requests_toolbelt.multipart.encoder import MultipartEncoder
-from langdetect import detect
 
 
 class Style(Enum):
     """
     Enumeration class for different styles. Each style has three attributes:
     - styles_id: Identifier for the style.
     - asset: Reference to the asset associated with the style.
@@ -168,197 +164,7 @@
     DEPTH = "depth"
 
 
 class DeviantArt(Enum):
     """Enum for the DeviantArt API credentials."""
     ID = 23185
     SECRET = "fae0145a0736611056a5196a122c0d36"
-
-
-def validate_cfg(cfg: float) -> str:
-    """Validates the cfg parameter."""
-    if cfg < 0.0 or cfg > 16.0:
-        raise ValueError(f"Invalid CFG, must be in range (0; 16), {cfg}")
-    return str(cfg)
-
-
-class Imagine:
-    """Class for handling API requests to the Imagine service."""
-
-    HEADERS = {
-        "accept": "*/*",
-        "user-agent": "okhttp/4.10.0"
-    }
-
-    def __init__(self):
-        self.asset = "https://1966211409.rsc.cdn77.org"
-        self.api = "https://inferenceengine.vyro.ai"
-        self.session = Session()
-        self.version = "1"
-
-    def _request(self, **kwargs) -> Response:
-        """Sends a request to the server and returns the response."""
-        headers = Imagine.HEADERS.copy()
-        headers.update(kwargs.get("headers", {}))
-
-        response = self.session.request(
-            method=kwargs.get("method", "GET").upper(),
-            url=kwargs.get("url"),
-            params=kwargs.get("params"),
-            data=kwargs.get("data"),
-            headers=headers
-        )
-
-        response.raise_for_status()
-        return response
-
-    def _build_multipart_data(self, fields: dict) -> Tuple[MultipartEncoder, dict]:
-        """Helper function to build multipart form data."""
-        multi = MultipartEncoder(fields=fields)
-        headers = {"content-type": multi.content_type}
-        return multi, headers
-
-    def assets(self, style: Style = Style.IMAGINE_V1) -> bytes:
-        """Gets the assets."""
-        return self._request(
-            url=f"{self.asset}/appStuff/imagine-fncisndcubnsduigfuds//assets/{style.value[2]}/{style.value[1]}.webp"
-        ).content
-
-    def variate(self, image: bytes, prompt: str, style: Style = Style.IMAGINE_V1) -> bytes:
-        """Variates the character."""
-        multi, headers = self._build_multipart_data({
-            "model_version": self.version,
-            "prompt": prompt + (style.value[3] or ""),
-            "strength": "0",
-            "style_id": str(style.value[0]),
-            "image": ("image.png", image, "image/png")
-        })
-
-        return self._request(
-            method="POST",
-            url=f"{self.api}/variate",
-            data=multi,
-            headers=headers
-        ).content
-
-    def sdprem(self, prompt: str, negative: str = None, priority: str = None, steps: str = None, high_res_results: str = None, style: Style = Style.IMAGINE_V1, seed: str = None, ratio: Ratio = Ratio.RATIO_1X1, cfg: float = 9.5) -> bytes:
-        """Generates AI Art."""
-        try:
-            validated_cfg = validate_cfg(cfg)
-        except Exception as e:
-            print(f"An error occurred while validating cfg: {e}")
-            return None
-
-        try:
-            return self._request(
-                method="POST",
-                url=f"{self.api}/sdprem",
-                data={
-                    "model_version": self.version,
-                    "prompt": prompt + (style.value[3] or ""),
-                    "negative_prompt": negative or "",
-                    "style_id": style.value[0],
-                    "width": ratio.value[0],
-                    "height": ratio.value[1],
-                    "seed": seed or "",
-                    "steps": steps or "30",
-                    "cfg": validated_cfg,
-                    "priority": priority or "0",
-                    "high_res_results": high_res_results or "0"
-                }
-            ).content
-        except Exception as e:
-            print(f"An error occurred while making the request: {e}")
-            return None
-
-    def upscale(self, image: bytes) -> bytes:
-        """Upscales the image."""
-        try:
-            multi, headers = self._build_multipart_data({
-                "model_version": self.version,
-                "image": ("test.png", image, "image/png")
-            })
-        except Exception as e:
-            print(f"An error occurred while building the multipart data: {e}")
-            return None
-
-        try:
-            return self._request(
-                method="POST",
-                url=f"{self.api}/upscale",
-                data=multi,
-                headers=headers
-            ).content
-        except Exception as e:
-            print(f"An error occurred while making the request: {e}")
-            return None
-
-    def translate(self, prompt: str) -> str:
-        """Translates the prompt."""
-        multi, headers = self._build_multipart_data({
-            "q": prompt,
-            "source": detect(prompt),
-            "target": "en"
-        })
-
-        return self._request(
-            method="POST",
-            url=f"{self.api}/translate",
-            data=multi,
-            headers=headers
-        ).json()["translatedText"]
-
-    def interrogator(self, image: bytes) -> str:
-        """Generates a prompt."""
-        multi, headers = self._build_multipart_data({
-            "model_version": str(self.version),
-            "image": ("prompt_generator_temp.png", image, "application/zip")
-        })
-
-        return self._request(
-            method="POST",
-            url=f"{self.api}/interrogator",
-            data=multi,
-            headers=headers
-        ).text
-
-    def sdimg(self, image: bytes, prompt: str, negative: str = None, seed: str = None, cfg: float = 9.5) -> bytes:
-        """Performs inpainting."""
-        multi, headers = self._build_multipart_data({
-            "model_version": self.version,
-            "prompt": prompt,
-            "negative_prompt": negative or "",
-            "seed": seed or "",
-            "cfg": validate_cfg(cfg),
-            "image": ("image.png", image, "image/png")
-        })
-
-        return self._request(
-            method="POST",
-            url=f"{self.api}/sdimg",
-            data=multi,
-            headers=headers
-        ).content
-
-    def controlnet(self, image: bytes, prompt: str, negative: str = None, cfg: float = 9.5, control: Control = Control.SCRIBBLE, style: Style = Style.IMAGINE_V1, seed: str = None) -> bytes:
-        """Performs image remix."""
-        multi, headers = self._build_multipart_data({
-            "model_version": self.version,
-            "prompt": prompt + (style.value[3] or ""),
-            "negative_prompt": negative or "",
-            "strength": "0",
-            "cfg": validate_cfg(cfg),
-            "control": control.value,
-            "style_id": str(style.value[0]),
-            "seed": seed or "",
-            "image": ("image.png", image, "image/png")
-        })
-
-        return self._request(
-            method="POST",
-            url=f"{self.api}/controlnet",
-            data=multi,
-            headers=headers
-        ).content
-
-
-__version__ = "1.0.7"
```

### Comparing `imaginepy-1.0.7/imaginepy.egg-info/PKG-INFO` & `imaginepy-1.1.0/imaginepy.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imaginepy
-Version: 1.0.7
+Version: 1.1.0
 Summary: Python library to create Art with AI.
 Home-page: https://github.com/ItsCEED/imaginepy
 Author: CEED
 Author-email: 
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -18,18 +18,21 @@
 License-File: LICENSE
 
 <div align="center">
 
 <img src="https://github.com/ItsCEED/ImaginePy-Midjourney-Free-Alternative/blob/main/docs/imagine_logo.gif" width="10%">
 
 **ImaginePy**
-
+<br>
+<img src="https://discordapp.com/api/guilds/1110314971012808774/widget.png?style=banner4" alt="Discord Banner 4"/>
+<br>
 <img src="https://img.shields.io/badge/python-3.7+-informational?style=plastic" alt="Python version">
 <img src="https://img.shields.io/github/release-date/ItsCEED/ImaginePy-Midjourney-Free-Alternative?style=plastic" alt="Release">
 <img src="https://img.shields.io/github/release/ItsCEED/ImaginePy-Midjourney-Free-Alternative?style=plastic" alt="Version">
+
 </div>
 
 ## Features
 
 - 🎨 Turn words into art
 - 👓 Choose from an array of art styles
 - 🔧 Adjust your masterpiece with creative controls!
@@ -60,16 +63,16 @@
 [hyugogirubato]: https://github.com/hyugogirubato/pyImagine
 
 ### From Source Code
 
 The following steps are instructions on download, preparing, and running the code under a Venv environment.
 You can skip steps 3-5 with a simple `python setup.py install` call instead, but you miss out on a wide array of benefits.
 
-1. `git clone https://github.com/ItsCEED/ImaginePy-Midjourney-Free-Alternative`
-2. `cd ImaginePy-Midjourney-Free-Alternative`
+1. `git clone https://github.com/ItsCEED/Imaginepy`
+2. `cd Imaginepy`
 3. `python -m venv env`
 4. `source env/bin/activate`
 5. `python setup.py install`
 
 As seen in Step 5, running the `imaginepy` executable is somewhat different to a normal PIP installation.
 See [Venv's Docs] on various ways of making calls under the virtual-environment.
 
@@ -111,14 +114,52 @@
     except Exception as e:
         print(f"An error occurred while writing the image to file: {e}")
 
 if __name__ == "__main__":
     main()
 ```
 
+Async version
+
+```python
+import asyncio
+from imaginepy import AsyncImagine, Style, Ratio
+
+
+async def main():
+    imagine = AsyncImagine()
+
+    img_data = await imagine.sdprem(
+        prompt="Woman sitting on a table, looking at the sky, seen from behind",
+        style=Style.ANIME_V2,
+        ratio=Ratio.RATIO_16X9
+    )
+
+    if img_data is None:
+        print("An error occurred while generating the image.")
+        return
+
+    img_data = await imagine.upscale(image=img_data)
+
+    if img_data is None:
+        print("An error occurred while upscaling the image.")
+        return
+
+    await imagine.close()
+    try:
+        with open("example.png", mode="wb") as img_file:
+            img_file.write(img_data)
+    except Exception as e:
+        print(f"An error occurred while writing the image to file: {e}")
+
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
+
 ## Credit
 
 - Imagine Icon &copy; Vyro AI & API
 - Original reverse and version by: [hyugogirubato]
 
 ## License
```

### Comparing `imaginepy-1.0.7/setup.py` & `imaginepy-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='imaginepy',
-    version='1.0.7',
+    version='1.1.0',
     author='CEED',
     author_email='',
     description='Python library to create Art with AI.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/ItsCEED/imaginepy',
     packages=find_packages(),
```

