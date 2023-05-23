# Comparing `tmp/cubetools-0.3.6.tar.gz` & `tmp/cubetools-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cubetools-0.3.6.tar", last modified: Thu May 18 07:08:58 2023, max compression
+gzip compressed data, was "dist/cubetools-0.3.7.tar", last modified: Tue May 23 11:30:22 2023, max compression
```

## Comparing `cubetools-0.3.6.tar` & `cubetools-0.3.7.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-18 07:08:58.000000 cubetools-0.3.6/
--rw-rw-r--   0 hls       (1000) hls       (1000)     2185 2023-05-18 07:08:58.000000 cubetools-0.3.6/PKG-INFO
--rw-rw-r--   0 hls       (1000) hls       (1000)     1093 2023-05-18 06:45:24.000000 cubetools-0.3.6/README.md
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-18 07:08:58.000000 cubetools-0.3.6/cubetools/
--rw-rw-r--   0 hls       (1000) hls       (1000)        0 2022-11-15 06:16:42.000000 cubetools-0.3.6/cubetools/__init__.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     9987 2023-05-15 01:24:04.000000 cubetools-0.3.6/cubetools/image_tools.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     1689 2023-04-03 13:20:28.000000 cubetools-0.3.6/cubetools/mindspore_lite_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)      607 2023-04-03 13:20:28.000000 cubetools-0.3.6/cubetools/onnx_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)      817 2023-04-06 07:12:09.000000 cubetools-0.3.6/cubetools/openvino_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3091 2023-04-03 13:20:28.000000 cubetools-0.3.6/cubetools/paddle_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     7658 2023-05-18 07:07:26.000000 cubetools-0.3.6/cubetools/python_video_frontend.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     2518 2023-03-08 07:16:48.000000 cubetools-0.3.6/cubetools/video_capture.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3726 2023-03-23 06:14:20.000000 cubetools-0.3.6/cubetools/video_predict.py
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-18 07:08:58.000000 cubetools-0.3.6/cubetools.egg-info/
--rw-rw-r--   0 hls       (1000) hls       (1000)     2185 2023-05-18 07:08:58.000000 cubetools-0.3.6/cubetools.egg-info/PKG-INFO
--rw-rw-r--   0 hls       (1000) hls       (1000)      474 2023-05-18 07:08:58.000000 cubetools-0.3.6/cubetools.egg-info/SOURCES.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)        1 2023-05-18 07:08:58.000000 cubetools-0.3.6/cubetools.egg-info/dependency_links.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)        5 2023-05-18 07:08:58.000000 cubetools-0.3.6/cubetools.egg-info/entry_points.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       27 2023-05-18 07:08:58.000000 cubetools-0.3.6/cubetools.egg-info/requires.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       10 2023-05-18 07:08:58.000000 cubetools-0.3.6/cubetools.egg-info/top_level.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       38 2023-05-18 07:08:58.000000 cubetools-0.3.6/setup.cfg
--rw-rw-r--   0 hls       (1000) hls       (1000)     2192 2023-05-18 07:07:27.000000 cubetools-0.3.6/setup.py
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-23 11:30:22.000000 cubetools-0.3.7/
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2250 2023-05-23 11:30:22.000000 cubetools-0.3.7/PKG-INFO
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1150 2023-05-23 11:30:19.000000 cubetools-0.3.7/README.md
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-23 11:30:22.000000 cubetools-0.3.7/cubetools/
+-rw-rw-r--   0 hls       (1000) hls       (1000)        0 2022-11-15 06:16:42.000000 cubetools-0.3.7/cubetools/__init__.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     9987 2023-05-15 01:24:04.000000 cubetools-0.3.7/cubetools/image_tools.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1689 2023-04-03 13:20:28.000000 cubetools-0.3.7/cubetools/mindspore_lite_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)      607 2023-04-03 13:20:28.000000 cubetools-0.3.7/cubetools/onnx_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)      817 2023-04-06 07:12:09.000000 cubetools-0.3.7/cubetools/openvino_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3091 2023-04-03 13:20:28.000000 cubetools-0.3.7/cubetools/paddle_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2431 2023-05-23 11:30:19.000000 cubetools-0.3.7/cubetools/python_chat_frontend.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     7658 2023-05-18 07:11:58.000000 cubetools-0.3.7/cubetools/python_video_frontend.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2518 2023-03-08 07:16:48.000000 cubetools-0.3.7/cubetools/video_capture.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3726 2023-03-23 06:14:20.000000 cubetools-0.3.7/cubetools/video_predict.py
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-23 11:30:22.000000 cubetools-0.3.7/cubetools.egg-info/
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2250 2023-05-23 11:30:22.000000 cubetools-0.3.7/cubetools.egg-info/PKG-INFO
+-rw-rw-r--   0 hls       (1000) hls       (1000)      508 2023-05-23 11:30:22.000000 cubetools-0.3.7/cubetools.egg-info/SOURCES.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)        1 2023-05-23 11:30:22.000000 cubetools-0.3.7/cubetools.egg-info/dependency_links.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)        5 2023-05-23 11:30:22.000000 cubetools-0.3.7/cubetools.egg-info/entry_points.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       27 2023-05-23 11:30:22.000000 cubetools-0.3.7/cubetools.egg-info/requires.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       10 2023-05-23 11:30:22.000000 cubetools-0.3.7/cubetools.egg-info/top_level.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       38 2023-05-23 11:30:22.000000 cubetools-0.3.7/setup.cfg
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2192 2023-05-23 11:30:19.000000 cubetools-0.3.7/setup.py
```

### Comparing `cubetools-0.3.6/PKG-INFO` & `cubetools-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: cubetools
-Version: 0.3.6
+Version: 0.3.7
 Summary: CubeAI模型开发常用工具集
 Home-page: https://openi.pcl.ac.cn/cubeai/cubetools
 Author: cubeai
 Author-email: cubeai@163.com
 License: Apache License 2.0
 Description: # CubeTools
         
         [CubeAI智立方](https://openi.pcl.ac.cn/OpenI/cubeai) 模型和应用开发常用工具集。
         
         目前主要包括：
         
         - 图像前处理、后处理常用函数封装。
         - 支持多路视频流媒体在线AI流式服务的通用SDK组件。
         - 基于Gradio的AI视频流媒体Python前端SDK组件。
+        - 基于Gradio的对话式聊天Python前端SDK组件。
         - 基于 [OpenVino Runtime](https://pypi.org/project/openvino/) 封装的通用OpenVino模型推理器。
         - 基于 [ONNX Runtime](https://pypi.org/project/onnxruntime-gpu/) 封装的通用ONNX模型推理器。
         - 基于 [Paddle Inference](https://www.paddlepaddle.org.cn/paddle/paddleinference) 推理引擎封装的通用PaddlePaddle模型推理器。
         - 基于 [MindSpore Lite](https://www.mindspore.cn/lite) 推理引擎封装的通用MindSporeLite推理器。
         
         
         ## 开源主页
```

### Comparing `cubetools-0.3.6/README.md` & `cubetools-0.3.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 [CubeAI智立方](https://openi.pcl.ac.cn/OpenI/cubeai) 模型和应用开发常用工具集。
 
 目前主要包括：
 
 - 图像前处理、后处理常用函数封装。
 - 支持多路视频流媒体在线AI流式服务的通用SDK组件。
 - 基于Gradio的AI视频流媒体Python前端SDK组件。
+- 基于Gradio的对话式聊天Python前端SDK组件。
 - 基于 [OpenVino Runtime](https://pypi.org/project/openvino/) 封装的通用OpenVino模型推理器。
 - 基于 [ONNX Runtime](https://pypi.org/project/onnxruntime-gpu/) 封装的通用ONNX模型推理器。
 - 基于 [Paddle Inference](https://www.paddlepaddle.org.cn/paddle/paddleinference) 推理引擎封装的通用PaddlePaddle模型推理器。
 - 基于 [MindSpore Lite](https://www.mindspore.cn/lite) 推理引擎封装的通用MindSporeLite推理器。
 
 
 ## 开源主页
```

### Comparing `cubetools-0.3.6/cubetools/image_tools.py` & `cubetools-0.3.7/cubetools/image_tools.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.6/cubetools/mindspore_lite_predict.py` & `cubetools-0.3.7/cubetools/mindspore_lite_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.6/cubetools/onnx_predict.py` & `cubetools-0.3.7/cubetools/onnx_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.6/cubetools/openvino_predict.py` & `cubetools-0.3.7/cubetools/openvino_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.6/cubetools/paddle_predict.py` & `cubetools-0.3.7/cubetools/paddle_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.6/cubetools/python_video_frontend.py` & `cubetools-0.3.7/cubetools/python_video_frontend.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.6/cubetools/video_capture.py` & `cubetools-0.3.7/cubetools/video_capture.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.6/cubetools/video_predict.py` & `cubetools-0.3.7/cubetools/video_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.6/cubetools.egg-info/PKG-INFO` & `cubetools-0.3.7/cubetools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: cubetools
-Version: 0.3.6
+Version: 0.3.7
 Summary: CubeAI模型开发常用工具集
 Home-page: https://openi.pcl.ac.cn/cubeai/cubetools
 Author: cubeai
 Author-email: cubeai@163.com
 License: Apache License 2.0
 Description: # CubeTools
         
         [CubeAI智立方](https://openi.pcl.ac.cn/OpenI/cubeai) 模型和应用开发常用工具集。
         
         目前主要包括：
         
         - 图像前处理、后处理常用函数封装。
         - 支持多路视频流媒体在线AI流式服务的通用SDK组件。
         - 基于Gradio的AI视频流媒体Python前端SDK组件。
+        - 基于Gradio的对话式聊天Python前端SDK组件。
         - 基于 [OpenVino Runtime](https://pypi.org/project/openvino/) 封装的通用OpenVino模型推理器。
         - 基于 [ONNX Runtime](https://pypi.org/project/onnxruntime-gpu/) 封装的通用ONNX模型推理器。
         - 基于 [Paddle Inference](https://www.paddlepaddle.org.cn/paddle/paddleinference) 推理引擎封装的通用PaddlePaddle模型推理器。
         - 基于 [MindSpore Lite](https://www.mindspore.cn/lite) 推理引擎封装的通用MindSporeLite推理器。
         
         
         ## 开源主页
```

### Comparing `cubetools-0.3.6/setup.py` & `cubetools-0.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 with open("README.md", "r", encoding='utf-8') as file:
     long_description = file.read()
 
 
 setup(
     name='cubetools',
-    version='0.3.6',
+    version='0.3.7',
     author='cubeai',
     author_email='cubeai@163.com',
     description='CubeAI模型开发常用工具集',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     packages=find_packages(),
```

