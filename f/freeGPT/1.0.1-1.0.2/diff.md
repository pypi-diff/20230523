# Comparing `tmp/freeGPT-1.0.0.1.tar.gz` & `tmp/freeGPT-1.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Ruu3f\Downloads\freeGPT\dist\.tmp-al3xau42\freeGPT-1.0.1.tar", last modified: Sat May 20 15:24:05 2023, max compression
+gzip compressed data, was "C:\Users\Ruu3f\Downloads\freeGPT\dist\.tmp-s8zeo95c\freeGPT-1.0.2.tar", last modified: Tue May 23 08:28:35 2023, max compression
```

## Comparing `freeGPT-1.0.0.1.tar` & `freeGPT-1.0.0.2.tar`

### file list

```diff
@@ -1,20 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 15:24:05.796605 freeGPT-1.0.1/
--rw-rw-rw-   0        0        0    35149 2023-05-20 15:22:24.000000 freeGPT-1.0.1/LICENSE
--rw-rw-rw-   0        0        0       98 2023-05-20 15:22:24.000000 freeGPT-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3036 2023-05-20 15:24:05.796605 freeGPT-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1952 2023-05-20 15:22:24.000000 freeGPT-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 15:24:05.780977 freeGPT-1.0.1/freeGPT/
--rw-rw-rw-   0        0        0     2449 2023-05-20 15:22:24.000000 freeGPT-1.0.1/freeGPT/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-20 15:24:05.780977 freeGPT-1.0.1/freeGPT/gpt3/
--rw-rw-rw-   0        0        0     2018 2023-05-20 15:22:24.000000 freeGPT-1.0.1/freeGPT/gpt3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-20 15:24:05.780977 freeGPT-1.0.1/freeGPT/gpt4/
--rw-rw-rw-   0        0        0     6228 2023-05-20 15:22:24.000000 freeGPT-1.0.1/freeGPT/gpt4/__init__.py
--rw-rw-rw-   0        0        0      410 2023-05-20 15:22:24.000000 freeGPT-1.0.1/freeGPT/gpt4/typing.py
-drwxrwxrwx   0        0        0        0 2023-05-20 15:24:05.780977 freeGPT-1.0.1/freeGPT.egg-info/
--rw-rw-rw-   0        0        0     3036 2023-05-20 15:24:05.000000 freeGPT-1.0.1/freeGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-05-20 15:24:05.000000 freeGPT-1.0.1/freeGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 15:24:05.000000 freeGPT-1.0.1/freeGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-20 15:24:05.000000 freeGPT-1.0.1/freeGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-20 15:24:05.000000 freeGPT-1.0.1/freeGPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 15:24:05.796605 freeGPT-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1486 2023-05-20 15:22:24.000000 freeGPT-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 08:28:35.747689 freeGPT-1.0.2/
+-rw-rw-rw-   0        0        0    35149 2023-05-23 08:00:03.000000 freeGPT-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0       98 2023-05-23 08:00:03.000000 freeGPT-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3349 2023-05-23 08:28:35.747689 freeGPT-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2258 2023-05-23 08:00:03.000000 freeGPT-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 08:28:35.736288 freeGPT-1.0.2/freeGPT/
+-rw-rw-rw-   0        0        0     2449 2023-05-23 08:28:09.000000 freeGPT-1.0.2/freeGPT/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 08:28:35.746353 freeGPT-1.0.2/freeGPT/gpt3/
+-rw-rw-rw-   0        0        0     2018 2023-05-23 08:00:03.000000 freeGPT-1.0.2/freeGPT/gpt3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 08:28:35.745331 freeGPT-1.0.2/freeGPT.egg-info/
+-rw-rw-rw-   0        0        0     3349 2023-05-23 08:28:35.000000 freeGPT-1.0.2/freeGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-05-23 08:28:35.000000 freeGPT-1.0.2/freeGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 08:28:35.000000 freeGPT-1.0.2/freeGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-23 08:28:35.000000 freeGPT-1.0.2/freeGPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-23 08:28:35.000000 freeGPT-1.0.2/freeGPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 08:28:35.747689 freeGPT-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1486 2023-05-23 08:28:20.000000 freeGPT-1.0.2/setup.py
```

### Comparing `freeGPT-1.0.1/LICENSE` & `freeGPT-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `freeGPT-1.0.1/PKG-INFO` & `freeGPT-1.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python package that provides free access to GPT3, GPT4, and more models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv3
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Issues, https://github.com/Ruu3f/freeGPT/issues
 Project-URL: Discussions, https://github.com/Ruu3f/freeGPT/discussions
@@ -17,24 +17,25 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+#### *Latest: 5 MORE STARS FOR INTERNET SEARCH GPT MODELS*
 [![PyPI version](https://badge.fury.io/py/freeGPT.svg)](https://badge.fury.io/py/freeGPT)
 [![Downloads](https://static.pepy.tech/personalized-badge/freeGPT?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/freeGPT)
 # freeGPT
 A Python package that gives access to GPT3 &amp; GPT4 models for free.
 <br>
 *Get started by doing: `pip install freeGPT`*
 
-## Examples
+## Examples:
 
-#### GPT-3
+#### GPT-3:
 
 ```python
 from freeGPT import gpt3
 
 def send_prompt():
     try:
         prompt = input("> ")
@@ -42,15 +43,15 @@
         print("Response:", response.text)
     except Exception as e:
         print("Error:", str(e))
 
 while True:
     send_prompt()
 ```
-#### GPT-4
+#### GPT-4:
 
 ```python
 from freeGPT import gpt4
 
 token = gpt4.Account.create(logging=True)
 print("Token:", token) 
 
@@ -62,28 +63,34 @@
     except Exception as e:
         print("Error:", str(e))
 
 while True:
     send_prompt()
 ```
 
-## Source
-| Models        | Websites                                 |
-| ------------- | -----------------------------------------|
-| GPT-3         | [theb.ai](https://theb.ai)               |
-| GPT-4         | [forefront.ai](https://chat.forefront.ai)|
+## Source:
+*Models with .web have internet access on.*
+<br>
+| Models            | Websites                                 |
+| ----------------- | -----------------------------------------|
+| gpt3              | [theb.ai](https://theb.ai)               |
+| gpt3.web          | [you.com](https://you.com)               |
+| gpt4              | [useless.com](https://ai.useless.com)    |
+| gpt4.web          | [forefront.ai](https://chat.forefront.ai)|
 
 ### TODO-List:
 - [x] Add GPT-4.
 - [x] Make the library well-documented.
 - [x] Make the over-all library easier to use.
 - [x] Make the over-all library easier to understand.
 - [x] Replace you.com with theb.ai for less failed responses.
-- [ ] Add an internet search model
-- [ ] Add text to image generation
+- [ ] Add a internet search model for GPT-3 & GPT-4
 - [ ] Make a discord bot
+- [ ] Add text to image generation
 
-### Star History
+## Star History:
 [![Star History Chart](https://api.star-history.com/svg?repos=Ruu3f/freeGPT&type=Date)](https://github.com/Ruu3f/freeGPT/stargazers)
 
-#### Original by [xtekky](https://github.com/xtekky), package & improved code by Ruu3f.
+## Discord Server:
+#### Join my server to support me :D
+#### -> [discord.gg/NcQ26PrNDp](https://discord.gg/NcQ26PrNDp)
```

### Comparing `freeGPT-1.0.1/README.md` & `freeGPT-1.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+#### *Latest: 5 MORE STARS FOR INTERNET SEARCH GPT MODELS*
 [![PyPI version](https://badge.fury.io/py/freeGPT.svg)](https://badge.fury.io/py/freeGPT)
 [![Downloads](https://static.pepy.tech/personalized-badge/freeGPT?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/freeGPT)
 # freeGPT
 A Python package that gives access to GPT3 &amp; GPT4 models for free.
 <br>
 *Get started by doing: `pip install freeGPT`*
 
-## Examples
+## Examples:
 
-#### GPT-3
+#### GPT-3:
 
 ```python
 from freeGPT import gpt3
 
 def send_prompt():
     try:
         prompt = input("> ")
@@ -19,15 +20,15 @@
         print("Response:", response.text)
     except Exception as e:
         print("Error:", str(e))
 
 while True:
     send_prompt()
 ```
-#### GPT-4
+#### GPT-4:
 
 ```python
 from freeGPT import gpt4
 
 token = gpt4.Account.create(logging=True)
 print("Token:", token) 
 
@@ -39,28 +40,34 @@
     except Exception as e:
         print("Error:", str(e))
 
 while True:
     send_prompt()
 ```
 
-## Source
-| Models        | Websites                                 |
-| ------------- | -----------------------------------------|
-| GPT-3         | [theb.ai](https://theb.ai)               |
-| GPT-4         | [forefront.ai](https://chat.forefront.ai)|
+## Source:
+*Models with .web have internet access on.*
+<br>
+| Models            | Websites                                 |
+| ----------------- | -----------------------------------------|
+| gpt3              | [theb.ai](https://theb.ai)               |
+| gpt3.web          | [you.com](https://you.com)               |
+| gpt4              | [useless.com](https://ai.useless.com)    |
+| gpt4.web          | [forefront.ai](https://chat.forefront.ai)|
 
 ### TODO-List:
 - [x] Add GPT-4.
 - [x] Make the library well-documented.
 - [x] Make the over-all library easier to use.
 - [x] Make the over-all library easier to understand.
 - [x] Replace you.com with theb.ai for less failed responses.
-- [ ] Add an internet search model
-- [ ] Add text to image generation
+- [ ] Add a internet search model for GPT-3 & GPT-4
 - [ ] Make a discord bot
+- [ ] Add text to image generation
 
-### Star History
+## Star History:
 [![Star History Chart](https://api.star-history.com/svg?repos=Ruu3f/freeGPT&type=Date)](https://github.com/Ruu3f/freeGPT/stargazers)
 
-#### Original by [xtekky](https://github.com/xtekky), package & improved code by Ruu3f.
+## Discord Server:
+#### Join my server to support me :D
+#### -> [discord.gg/NcQ26PrNDp](https://discord.gg/NcQ26PrNDp)
```

### Comparing `freeGPT-1.0.1/freeGPT/__init__.py` & `freeGPT-1.0.2/freeGPT/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 the desired model and a `Completion` class for creating text completions.
 """
 
 from enum import Enum
 from .freeGPT import gpt3, gpt4
 
 __author__ = "Ruu3f"
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 
 __all__ = ["Provider", "Completion"]
 
 
 class Provider(Enum):
     """Enum class representing the available GPT providers."""
```

### Comparing `freeGPT-1.0.1/freeGPT/gpt3/__init__.py` & `freeGPT-1.0.2/freeGPT/gpt3/__init__.py`

 * *Files identical despite different names*

### Comparing `freeGPT-1.0.1/freeGPT.egg-info/PKG-INFO` & `freeGPT-1.0.2/freeGPT.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python package that provides free access to GPT3, GPT4, and more models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv3
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Issues, https://github.com/Ruu3f/freeGPT/issues
 Project-URL: Discussions, https://github.com/Ruu3f/freeGPT/discussions
@@ -17,24 +17,25 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+#### *Latest: 5 MORE STARS FOR INTERNET SEARCH GPT MODELS*
 [![PyPI version](https://badge.fury.io/py/freeGPT.svg)](https://badge.fury.io/py/freeGPT)
 [![Downloads](https://static.pepy.tech/personalized-badge/freeGPT?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/freeGPT)
 # freeGPT
 A Python package that gives access to GPT3 &amp; GPT4 models for free.
 <br>
 *Get started by doing: `pip install freeGPT`*
 
-## Examples
+## Examples:
 
-#### GPT-3
+#### GPT-3:
 
 ```python
 from freeGPT import gpt3
 
 def send_prompt():
     try:
         prompt = input("> ")
@@ -42,15 +43,15 @@
         print("Response:", response.text)
     except Exception as e:
         print("Error:", str(e))
 
 while True:
     send_prompt()
 ```
-#### GPT-4
+#### GPT-4:
 
 ```python
 from freeGPT import gpt4
 
 token = gpt4.Account.create(logging=True)
 print("Token:", token) 
 
@@ -62,28 +63,34 @@
     except Exception as e:
         print("Error:", str(e))
 
 while True:
     send_prompt()
 ```
 
-## Source
-| Models        | Websites                                 |
-| ------------- | -----------------------------------------|
-| GPT-3         | [theb.ai](https://theb.ai)               |
-| GPT-4         | [forefront.ai](https://chat.forefront.ai)|
+## Source:
+*Models with .web have internet access on.*
+<br>
+| Models            | Websites                                 |
+| ----------------- | -----------------------------------------|
+| gpt3              | [theb.ai](https://theb.ai)               |
+| gpt3.web          | [you.com](https://you.com)               |
+| gpt4              | [useless.com](https://ai.useless.com)    |
+| gpt4.web          | [forefront.ai](https://chat.forefront.ai)|
 
 ### TODO-List:
 - [x] Add GPT-4.
 - [x] Make the library well-documented.
 - [x] Make the over-all library easier to use.
 - [x] Make the over-all library easier to understand.
 - [x] Replace you.com with theb.ai for less failed responses.
-- [ ] Add an internet search model
-- [ ] Add text to image generation
+- [ ] Add a internet search model for GPT-3 & GPT-4
 - [ ] Make a discord bot
+- [ ] Add text to image generation
 
-### Star History
+## Star History:
 [![Star History Chart](https://api.star-history.com/svg?repos=Ruu3f/freeGPT&type=Date)](https://github.com/Ruu3f/freeGPT/stargazers)
 
-#### Original by [xtekky](https://github.com/xtekky), package & improved code by Ruu3f.
+## Discord Server:
+#### Join my server to support me :D
+#### -> [discord.gg/NcQ26PrNDp](https://discord.gg/NcQ26PrNDp)
```

### Comparing `freeGPT-1.0.1/setup.py` & `freeGPT-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="freeGPT",
-    version="1.0.1",
+    version="1.0.2",
     description="A Python package that provides free access to GPT3, GPT4, and more models.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Ruu3f/freeGPT",
     author="Ruu3f",
     license="GPLv3",
     keywords=[
```

