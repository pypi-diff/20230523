# Comparing `tmp/segment_anything_utils-0.1.0.tar.gz` & `tmp/segment_anything_utils-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segment_anything_utils-0.1.0.tar", last modified: Mon May  8 09:04:21 2023, max compression
+gzip compressed data, was "segment_anything_utils-0.2.0.tar", last modified: Tue May 23 09:43:31 2023, max compression
```

## Comparing `segment_anything_utils-0.1.0.tar` & `segment_anything_utils-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 tomdyqin   (501) staff       (20)        0 2023-05-08 09:04:21.140631 segment_anything_utils-0.1.0/
--rw-r--r--   0 tomdyqin   (501) staff       (20)      864 2023-05-08 09:04:21.140384 segment_anything_utils-0.1.0/PKG-INFO
--rw-r--r--   0 tomdyqin   (501) staff       (20)      237 2023-05-08 08:07:22.000000 segment_anything_utils-0.1.0/README.md
-drwxr-xr-x   0 tomdyqin   (501) staff       (20)        0 2023-05-08 09:04:21.138333 segment_anything_utils-0.1.0/segment_anything_utils/
--rw-r--r--   0 tomdyqin   (501) staff       (20)       20 2023-05-08 03:07:00.000000 segment_anything_utils-0.1.0/segment_anything_utils/__init__.py
--rw-r--r--   0 tomdyqin   (501) staff       (20)     3687 2023-05-08 08:22:53.000000 segment_anything_utils-0.1.0/segment_anything_utils/load.py
-drwxr-xr-x   0 tomdyqin   (501) staff       (20)        0 2023-05-08 09:04:21.139990 segment_anything_utils-0.1.0/segment_anything_utils.egg-info/
--rw-r--r--   0 tomdyqin   (501) staff       (20)      864 2023-05-08 09:04:21.000000 segment_anything_utils-0.1.0/segment_anything_utils.egg-info/PKG-INFO
--rw-r--r--   0 tomdyqin   (501) staff       (20)      313 2023-05-08 09:04:21.000000 segment_anything_utils-0.1.0/segment_anything_utils.egg-info/SOURCES.txt
--rw-r--r--   0 tomdyqin   (501) staff       (20)        1 2023-05-08 09:04:21.000000 segment_anything_utils-0.1.0/segment_anything_utils.egg-info/dependency_links.txt
--rw-r--r--   0 tomdyqin   (501) staff       (20)       47 2023-05-08 09:04:21.000000 segment_anything_utils-0.1.0/segment_anything_utils.egg-info/requires.txt
--rw-r--r--   0 tomdyqin   (501) staff       (20)       23 2023-05-08 09:04:21.000000 segment_anything_utils-0.1.0/segment_anything_utils.egg-info/top_level.txt
--rw-r--r--   0 tomdyqin   (501) staff       (20)       38 2023-05-08 09:04:21.140706 segment_anything_utils-0.1.0/setup.cfg
--rw-r--r--   0 tomdyqin   (501) staff       (20)     3846 2023-05-08 09:03:31.000000 segment_anything_utils-0.1.0/setup.py
+drwxr-xr-x   0 tomdyqin   (501) staff       (20)        0 2023-05-23 09:43:31.355122 segment_anything_utils-0.2.0/
+-rw-r--r--   0 tomdyqin   (501) staff       (20)      839 2023-05-23 09:43:31.354678 segment_anything_utils-0.2.0/PKG-INFO
+-rw-r--r--   0 tomdyqin   (501) staff       (20)      212 2023-05-23 09:43:29.000000 segment_anything_utils-0.2.0/README.md
+drwxr-xr-x   0 tomdyqin   (501) staff       (20)        0 2023-05-23 09:43:31.351553 segment_anything_utils-0.2.0/segment_anything_utils/
+-rw-r--r--   0 tomdyqin   (501) staff       (20)       20 2023-05-08 03:07:00.000000 segment_anything_utils-0.2.0/segment_anything_utils/__init__.py
+-rw-r--r--   0 tomdyqin   (501) staff       (20)     3708 2023-05-19 08:11:52.000000 segment_anything_utils-0.2.0/segment_anything_utils/load.py
+drwxr-xr-x   0 tomdyqin   (501) staff       (20)        0 2023-05-23 09:43:31.354242 segment_anything_utils-0.2.0/segment_anything_utils.egg-info/
+-rw-r--r--   0 tomdyqin   (501) staff       (20)      839 2023-05-23 09:43:31.000000 segment_anything_utils-0.2.0/segment_anything_utils.egg-info/PKG-INFO
+-rw-r--r--   0 tomdyqin   (501) staff       (20)      313 2023-05-23 09:43:31.000000 segment_anything_utils-0.2.0/segment_anything_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 tomdyqin   (501) staff       (20)        1 2023-05-23 09:43:31.000000 segment_anything_utils-0.2.0/segment_anything_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 tomdyqin   (501) staff       (20)       47 2023-05-23 09:43:31.000000 segment_anything_utils-0.2.0/segment_anything_utils.egg-info/requires.txt
+-rw-r--r--   0 tomdyqin   (501) staff       (20)       23 2023-05-23 09:43:31.000000 segment_anything_utils-0.2.0/segment_anything_utils.egg-info/top_level.txt
+-rw-r--r--   0 tomdyqin   (501) staff       (20)       38 2023-05-23 09:43:31.355259 segment_anything_utils-0.2.0/setup.cfg
+-rw-r--r--   0 tomdyqin   (501) staff       (20)     3846 2023-05-23 09:42:15.000000 segment_anything_utils-0.2.0/setup.py
```

### Comparing `segment_anything_utils-0.1.0/PKG-INFO` & `segment_anything_utils-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment_anything_utils
-Version: 0.1.0
+Version: 0.2.0
 Summary: utils for segment_anything.
 Home-page: https://github.com/tomdyqin/segment-anything-utils
 Author: Tomdy Qin
 Author-email: tomdyqin@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -19,11 +19,11 @@
 ## 工具箱 for segment_anything
 
 ## 发布
 先确保已经安装了最新版本的 setuptools, twine
 ```bash
 pip install --user --upgrade setuptools twine
 ```
-复制代码生成项目包：
+生成发布包
 ```bash
-python setup.py sdist bdist_wheel
+python ./setup.py sdist
 ```
```

### Comparing `segment_anything_utils-0.1.0/segment_anything_utils/load.py` & `segment_anything_utils-0.2.0/segment_anything_utils/load.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,11 +82,12 @@
 
 def load_generator(sam = None, options: Dict[str, Any] = {}):
     sam = sam if sam is not None else load_model()
     print('sam', sam)
     output_mode = "coco_rle" if options.get('convert_to_rle', None) else "binary_mask"
     amg_kwargs = get_amg_kwargs(options)
     generator = SamAutomaticMaskGenerator(sam, output_mode=output_mode, **amg_kwargs)
+    return generator
 
 
 if __name__ == "__main__":
     load_model(download_root= Path.cwd())
```

### Comparing `segment_anything_utils-0.1.0/segment_anything_utils.egg-info/PKG-INFO` & `segment_anything_utils-0.2.0/segment_anything_utils.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-anything-utils
-Version: 0.1.0
+Version: 0.2.0
 Summary: utils for segment_anything.
 Home-page: https://github.com/tomdyqin/segment-anything-utils
 Author: Tomdy Qin
 Author-email: tomdyqin@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -19,11 +19,11 @@
 ## 工具箱 for segment_anything
 
 ## 发布
 先确保已经安装了最新版本的 setuptools, twine
 ```bash
 pip install --user --upgrade setuptools twine
 ```
-复制代码生成项目包：
+生成发布包
 ```bash
-python setup.py sdist bdist_wheel
+python ./setup.py sdist
 ```
```

### Comparing `segment_anything_utils-0.1.0/setup.py` & `segment_anything_utils-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'segment_anything_utils'
 DESCRIPTION = 'utils for segment_anything.'
 URL = 'https://github.com/tomdyqin/segment-anything-utils'
 EMAIL = 'tomdyqin@qq.com'
 AUTHOR = 'Tomdy Qin'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.0'
+VERSION = '0.2.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests',
     'importlib',
     'tqdm',
     'torch',
```

