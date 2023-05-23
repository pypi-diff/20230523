# Comparing `tmp/cubetools-0.3.7.tar.gz` & `tmp/cubetools-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cubetools-0.3.7.tar", last modified: Tue May 23 11:30:22 2023, max compression
+gzip compressed data, was "dist/cubetools-0.3.8.tar", last modified: Tue May 23 11:33:52 2023, max compression
```

## Comparing `cubetools-0.3.7.tar` & `cubetools-0.3.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-23 11:30:22.000000 cubetools-0.3.7/
--rw-rw-r--   0 hls       (1000) hls       (1000)     2250 2023-05-23 11:30:22.000000 cubetools-0.3.7/PKG-INFO
--rw-rw-r--   0 hls       (1000) hls       (1000)     1150 2023-05-23 11:30:19.000000 cubetools-0.3.7/README.md
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-23 11:30:22.000000 cubetools-0.3.7/cubetools/
--rw-rw-r--   0 hls       (1000) hls       (1000)        0 2022-11-15 06:16:42.000000 cubetools-0.3.7/cubetools/__init__.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     9987 2023-05-15 01:24:04.000000 cubetools-0.3.7/cubetools/image_tools.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     1689 2023-04-03 13:20:28.000000 cubetools-0.3.7/cubetools/mindspore_lite_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)      607 2023-04-03 13:20:28.000000 cubetools-0.3.7/cubetools/onnx_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)      817 2023-04-06 07:12:09.000000 cubetools-0.3.7/cubetools/openvino_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3091 2023-04-03 13:20:28.000000 cubetools-0.3.7/cubetools/paddle_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     2431 2023-05-23 11:30:19.000000 cubetools-0.3.7/cubetools/python_chat_frontend.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     7658 2023-05-18 07:11:58.000000 cubetools-0.3.7/cubetools/python_video_frontend.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     2518 2023-03-08 07:16:48.000000 cubetools-0.3.7/cubetools/video_capture.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3726 2023-03-23 06:14:20.000000 cubetools-0.3.7/cubetools/video_predict.py
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-23 11:30:22.000000 cubetools-0.3.7/cubetools.egg-info/
--rw-rw-r--   0 hls       (1000) hls       (1000)     2250 2023-05-23 11:30:22.000000 cubetools-0.3.7/cubetools.egg-info/PKG-INFO
--rw-rw-r--   0 hls       (1000) hls       (1000)      508 2023-05-23 11:30:22.000000 cubetools-0.3.7/cubetools.egg-info/SOURCES.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)        1 2023-05-23 11:30:22.000000 cubetools-0.3.7/cubetools.egg-info/dependency_links.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)        5 2023-05-23 11:30:22.000000 cubetools-0.3.7/cubetools.egg-info/entry_points.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       27 2023-05-23 11:30:22.000000 cubetools-0.3.7/cubetools.egg-info/requires.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       10 2023-05-23 11:30:22.000000 cubetools-0.3.7/cubetools.egg-info/top_level.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       38 2023-05-23 11:30:22.000000 cubetools-0.3.7/setup.cfg
--rw-rw-r--   0 hls       (1000) hls       (1000)     2192 2023-05-23 11:30:19.000000 cubetools-0.3.7/setup.py
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-23 11:33:52.000000 cubetools-0.3.8/
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2250 2023-05-23 11:33:52.000000 cubetools-0.3.8/PKG-INFO
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1150 2023-05-23 11:30:19.000000 cubetools-0.3.8/README.md
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-23 11:33:52.000000 cubetools-0.3.8/cubetools/
+-rw-rw-r--   0 hls       (1000) hls       (1000)        0 2022-11-15 06:16:42.000000 cubetools-0.3.8/cubetools/__init__.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     9987 2023-05-15 01:24:04.000000 cubetools-0.3.8/cubetools/image_tools.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1689 2023-04-03 13:20:28.000000 cubetools-0.3.8/cubetools/mindspore_lite_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)      607 2023-04-03 13:20:28.000000 cubetools-0.3.8/cubetools/onnx_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)      817 2023-04-06 07:12:09.000000 cubetools-0.3.8/cubetools/openvino_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3091 2023-04-03 13:20:28.000000 cubetools-0.3.8/cubetools/paddle_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2430 2023-05-23 11:33:50.000000 cubetools-0.3.8/cubetools/python_chat_frontend.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     7658 2023-05-18 07:11:58.000000 cubetools-0.3.8/cubetools/python_video_frontend.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2518 2023-03-08 07:16:48.000000 cubetools-0.3.8/cubetools/video_capture.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3726 2023-03-23 06:14:20.000000 cubetools-0.3.8/cubetools/video_predict.py
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-23 11:33:52.000000 cubetools-0.3.8/cubetools.egg-info/
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2250 2023-05-23 11:33:52.000000 cubetools-0.3.8/cubetools.egg-info/PKG-INFO
+-rw-rw-r--   0 hls       (1000) hls       (1000)      508 2023-05-23 11:33:52.000000 cubetools-0.3.8/cubetools.egg-info/SOURCES.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)        1 2023-05-23 11:33:52.000000 cubetools-0.3.8/cubetools.egg-info/dependency_links.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)        5 2023-05-23 11:33:52.000000 cubetools-0.3.8/cubetools.egg-info/entry_points.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       27 2023-05-23 11:33:52.000000 cubetools-0.3.8/cubetools.egg-info/requires.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       10 2023-05-23 11:33:52.000000 cubetools-0.3.8/cubetools.egg-info/top_level.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       38 2023-05-23 11:33:52.000000 cubetools-0.3.8/setup.cfg
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2192 2023-05-23 11:33:50.000000 cubetools-0.3.8/setup.py
```

### Comparing `cubetools-0.3.7/PKG-INFO` & `cubetools-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubetools
-Version: 0.3.7
+Version: 0.3.8
 Summary: CubeAI模型开发常用工具集
 Home-page: https://openi.pcl.ac.cn/cubeai/cubetools
 Author: cubeai
 Author-email: cubeai@163.com
 License: Apache License 2.0
 Description: # CubeTools
```

### Comparing `cubetools-0.3.7/README.md` & `cubetools-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.7/cubetools/image_tools.py` & `cubetools-0.3.8/cubetools/image_tools.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.7/cubetools/mindspore_lite_predict.py` & `cubetools-0.3.8/cubetools/mindspore_lite_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.7/cubetools/onnx_predict.py` & `cubetools-0.3.8/cubetools/onnx_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.7/cubetools/openvino_predict.py` & `cubetools-0.3.8/cubetools/openvino_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.7/cubetools/paddle_predict.py` & `cubetools-0.3.8/cubetools/paddle_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.7/cubetools/python_chat_frontend.py` & `cubetools-0.3.8/cubetools/python_chat_frontend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import gradio as gr
 from serviceboot.serviceboot import serviceboot_client, gen_api_docs
 
 
-class PythonVideoFrontend(object):
+class PythonChatFrontend(object):
 
     # 在__init__中定义Python前端界面
     def __init__(self, model_name_cn, model_name_en=None, readme='README.md'):
         title = f'CubeAI应用示范——{model_name_cn}'
         if model_name_en:
             url_model_zoo = 'https://openi.pcl.ac.cn/cubeai-model-zoo/cubeai-model-zoo'
             url_model = f'https://openi.pcl.ac.cn/cubeai-model-zoo/{model_name_en}'
```

### Comparing `cubetools-0.3.7/cubetools/python_video_frontend.py` & `cubetools-0.3.8/cubetools/python_video_frontend.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.7/cubetools/video_capture.py` & `cubetools-0.3.8/cubetools/video_capture.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.7/cubetools/video_predict.py` & `cubetools-0.3.8/cubetools/video_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.7/cubetools.egg-info/PKG-INFO` & `cubetools-0.3.8/cubetools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubetools
-Version: 0.3.7
+Version: 0.3.8
 Summary: CubeAI模型开发常用工具集
 Home-page: https://openi.pcl.ac.cn/cubeai/cubetools
 Author: cubeai
 Author-email: cubeai@163.com
 License: Apache License 2.0
 Description: # CubeTools
```

### Comparing `cubetools-0.3.7/setup.py` & `cubetools-0.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 with open("README.md", "r", encoding='utf-8') as file:
     long_description = file.read()
 
 
 setup(
     name='cubetools',
-    version='0.3.7',
+    version='0.3.8',
     author='cubeai',
     author_email='cubeai@163.com',
     description='CubeAI模型开发常用工具集',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     packages=find_packages(),
```

