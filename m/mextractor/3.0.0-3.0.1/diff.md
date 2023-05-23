# Comparing `tmp/mextractor-3.0.0.tar.gz` & `tmp/mextractor-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mextractor-3.0.0.tar", max compression
+gzip compressed data, was "mextractor-3.0.1.tar", max compression
```

## Comparing `mextractor-3.0.0.tar` & `mextractor-3.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1620 2023-04-23 14:38:11.432613 mextractor-3.0.0/README.md
--rw-r--r--   0        0        0        0 2023-04-23 14:47:49.396153 mextractor-3.0.0/mextractor/__init__.py
--rw-r--r--   0        0        0     2461 2023-04-23 14:47:43.177188 mextractor-3.0.0/mextractor/base.py
--rw-r--r--   0        0        0      788 2023-04-23 14:48:01.751085 mextractor-3.0.0/mextractor/cli.py
--rw-r--r--   0        0        0       67 2023-04-23 14:38:11.432613 mextractor-3.0.0/mextractor/constants.py
--rw-r--r--   0        0        0     2545 2023-04-23 14:47:29.104265 mextractor-3.0.0/mextractor/extractors.py
--rw-r--r--   0        0        0      518 2023-04-23 14:38:11.432613 mextractor-3.0.0/mextractor/utils.py
--rw-r--r--   0        0        0     2351 2023-04-23 14:47:43.185188 mextractor-3.0.0/mextractor/workflow.py
--rw-r--r--   0        0        0     1247 2023-04-23 14:47:40.535202 mextractor-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     2787 1970-01-01 00:00:00.000000 mextractor-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1620 2022-10-17 12:17:16.047116 mextractor-3.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 07:57:13.655731 mextractor-3.0.1/mextractor/__init__.py
+-rw-r--r--   0        0        0     2461 2023-05-23 07:57:13.655731 mextractor-3.0.1/mextractor/base.py
+-rw-r--r--   0        0        0      788 2023-05-23 07:57:13.655731 mextractor-3.0.1/mextractor/cli.py
+-rw-r--r--   0        0        0       67 2022-10-17 12:21:33.238089 mextractor-3.0.1/mextractor/constants.py
+-rw-r--r--   0        0        0     2545 2023-05-23 07:57:13.655731 mextractor-3.0.1/mextractor/extractors.py
+-rw-r--r--   0        0        0      518 2023-05-23 07:57:13.655731 mextractor-3.0.1/mextractor/utils.py
+-rw-r--r--   0        0        0     2638 2023-05-23 08:53:53.635112 mextractor-3.0.1/mextractor/workflow.py
+-rw-r--r--   0        0        0     1273 2023-05-23 08:53:56.848112 mextractor-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2829 1970-01-01 00:00:00.000000 mextractor-3.0.1/PKG-INFO
```

### Comparing `mextractor-3.0.0/README.md` & `mextractor-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mextractor-3.0.0/mextractor/base.py` & `mextractor-3.0.1/mextractor/base.py`

 * *Files identical despite different names*

### Comparing `mextractor-3.0.0/mextractor/cli.py` & `mextractor-3.0.1/mextractor/cli.py`

 * *Files identical despite different names*

### Comparing `mextractor-3.0.0/mextractor/extractors.py` & `mextractor-3.0.1/mextractor/extractors.py`

 * *Files identical despite different names*

### Comparing `mextractor-3.0.0/mextractor/utils.py` & `mextractor-3.0.1/mextractor/utils.py`

 * *Files identical despite different names*

### Comparing `mextractor-3.0.0/pyproject.toml` & `mextractor-3.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mextractor"
-version = "3.0.0"
+version = "3.0.1"
 description = "mextractor can extract media metadata to YAML and read them"
 readme = "README.md"
 repository = "https://github.com/caniko/media-metadata-extractor"
 homepage = "https://pypi.org/project/mextractor/"
 authors = ["Can H. Tartanoglu <canhtart@gmail.com>"]
 license = "Apache-2.0"
 keywords = ["pydantic", "metadata", "video", "image", "bigdata"]
@@ -29,14 +29,15 @@
 click = "^8.1.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 
 [tool.poetry.extras]
 video-extract = ["ffmpeg-python"]
+video = ["ffmpeg-python"]
 
 [tool.poetry.scripts]
 mextractor = "mextractor.cli:mextractor_cli"
 
 [tool.mypy]
 python_version = "3.10"
 plugins = "numpy.typing.mypy_plugin"
```

### Comparing `mextractor-3.0.0/PKG-INFO` & `mextractor-3.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: mextractor
-Version: 3.0.0
+Version: 3.0.1
 Summary: mextractor can extract media metadata to YAML and read them
 Home-page: https://pypi.org/project/mextractor/
 License: Apache-2.0
 Keywords: pydantic,metadata,video,image,bigdata
 Author: Can H. Tartanoglu
 Author-email: canhtart@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: video
 Provides-Extra: video-extract
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0) ; extra == "video-extract"
+Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0) ; extra == "video-extract" or extra == "video"
 Requires-Dist: numpy
 Requires-Dist: opencv-python (>=4.6.0,<5.0.0)
 Requires-Dist: pydantic (>=1.9.2,<2.0.0)
 Requires-Dist: pydantic-numpy (>=2.2.1,<3.0.0)
 Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
 Project-URL: Repository, https://github.com/caniko/media-metadata-extractor
 Description-Content-Type: text/markdown
```

