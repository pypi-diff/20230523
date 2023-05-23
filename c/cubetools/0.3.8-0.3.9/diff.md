# Comparing `tmp/cubetools-0.3.8.tar.gz` & `tmp/cubetools-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cubetools-0.3.8.tar", last modified: Tue May 23 11:33:52 2023, max compression
+gzip compressed data, was "dist/cubetools-0.3.9.tar", last modified: Tue May 23 11:40:25 2023, max compression
```

## Comparing `cubetools-0.3.8.tar` & `cubetools-0.3.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-23 11:33:52.000000 cubetools-0.3.8/
--rw-rw-r--   0 hls       (1000) hls       (1000)     2250 2023-05-23 11:33:52.000000 cubetools-0.3.8/PKG-INFO
--rw-rw-r--   0 hls       (1000) hls       (1000)     1150 2023-05-23 11:30:19.000000 cubetools-0.3.8/README.md
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-23 11:33:52.000000 cubetools-0.3.8/cubetools/
--rw-rw-r--   0 hls       (1000) hls       (1000)        0 2022-11-15 06:16:42.000000 cubetools-0.3.8/cubetools/__init__.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     9987 2023-05-15 01:24:04.000000 cubetools-0.3.8/cubetools/image_tools.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     1689 2023-04-03 13:20:28.000000 cubetools-0.3.8/cubetools/mindspore_lite_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)      607 2023-04-03 13:20:28.000000 cubetools-0.3.8/cubetools/onnx_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)      817 2023-04-06 07:12:09.000000 cubetools-0.3.8/cubetools/openvino_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3091 2023-04-03 13:20:28.000000 cubetools-0.3.8/cubetools/paddle_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     2430 2023-05-23 11:33:50.000000 cubetools-0.3.8/cubetools/python_chat_frontend.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     7658 2023-05-18 07:11:58.000000 cubetools-0.3.8/cubetools/python_video_frontend.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     2518 2023-03-08 07:16:48.000000 cubetools-0.3.8/cubetools/video_capture.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3726 2023-03-23 06:14:20.000000 cubetools-0.3.8/cubetools/video_predict.py
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-23 11:33:52.000000 cubetools-0.3.8/cubetools.egg-info/
--rw-rw-r--   0 hls       (1000) hls       (1000)     2250 2023-05-23 11:33:52.000000 cubetools-0.3.8/cubetools.egg-info/PKG-INFO
--rw-rw-r--   0 hls       (1000) hls       (1000)      508 2023-05-23 11:33:52.000000 cubetools-0.3.8/cubetools.egg-info/SOURCES.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)        1 2023-05-23 11:33:52.000000 cubetools-0.3.8/cubetools.egg-info/dependency_links.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)        5 2023-05-23 11:33:52.000000 cubetools-0.3.8/cubetools.egg-info/entry_points.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       27 2023-05-23 11:33:52.000000 cubetools-0.3.8/cubetools.egg-info/requires.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       10 2023-05-23 11:33:52.000000 cubetools-0.3.8/cubetools.egg-info/top_level.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       38 2023-05-23 11:33:52.000000 cubetools-0.3.8/setup.cfg
--rw-rw-r--   0 hls       (1000) hls       (1000)     2192 2023-05-23 11:33:50.000000 cubetools-0.3.8/setup.py
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-23 11:40:25.000000 cubetools-0.3.9/
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2250 2023-05-23 11:40:25.000000 cubetools-0.3.9/PKG-INFO
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1150 2023-05-23 11:40:23.000000 cubetools-0.3.9/README.md
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-23 11:40:25.000000 cubetools-0.3.9/cubetools/
+-rw-rw-r--   0 hls       (1000) hls       (1000)        0 2022-11-15 06:16:42.000000 cubetools-0.3.9/cubetools/__init__.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     9987 2023-05-15 01:24:04.000000 cubetools-0.3.9/cubetools/image_tools.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1689 2023-04-03 13:20:28.000000 cubetools-0.3.9/cubetools/mindspore_lite_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)      607 2023-04-03 13:20:28.000000 cubetools-0.3.9/cubetools/onnx_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)      817 2023-04-06 07:12:09.000000 cubetools-0.3.9/cubetools/openvino_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3091 2023-04-03 13:20:28.000000 cubetools-0.3.9/cubetools/paddle_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2394 2023-05-23 11:40:23.000000 cubetools-0.3.9/cubetools/python_chat_frontend.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     7658 2023-05-18 07:11:58.000000 cubetools-0.3.9/cubetools/python_video_frontend.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2518 2023-03-08 07:16:48.000000 cubetools-0.3.9/cubetools/video_capture.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3726 2023-03-23 06:14:20.000000 cubetools-0.3.9/cubetools/video_predict.py
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-23 11:40:25.000000 cubetools-0.3.9/cubetools.egg-info/
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2250 2023-05-23 11:40:25.000000 cubetools-0.3.9/cubetools.egg-info/PKG-INFO
+-rw-rw-r--   0 hls       (1000) hls       (1000)      508 2023-05-23 11:40:25.000000 cubetools-0.3.9/cubetools.egg-info/SOURCES.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)        1 2023-05-23 11:40:25.000000 cubetools-0.3.9/cubetools.egg-info/dependency_links.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)        5 2023-05-23 11:40:25.000000 cubetools-0.3.9/cubetools.egg-info/entry_points.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       27 2023-05-23 11:40:25.000000 cubetools-0.3.9/cubetools.egg-info/requires.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       10 2023-05-23 11:40:25.000000 cubetools-0.3.9/cubetools.egg-info/top_level.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       38 2023-05-23 11:40:25.000000 cubetools-0.3.9/setup.cfg
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2192 2023-05-23 11:40:23.000000 cubetools-0.3.9/setup.py
```

### Comparing `cubetools-0.3.8/PKG-INFO` & `cubetools-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: cubetools
-Version: 0.3.8
+Version: 0.3.9
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
-        - 基于Gradio的对话式聊天Python前端SDK组件。
+        - 基于Gradio的聊天对话式Python前端SDK组件。
         - 基于 [OpenVino Runtime](https://pypi.org/project/openvino/) 封装的通用OpenVino模型推理器。
         - 基于 [ONNX Runtime](https://pypi.org/project/onnxruntime-gpu/) 封装的通用ONNX模型推理器。
         - 基于 [Paddle Inference](https://www.paddlepaddle.org.cn/paddle/paddleinference) 推理引擎封装的通用PaddlePaddle模型推理器。
         - 基于 [MindSpore Lite](https://www.mindspore.cn/lite) 推理引擎封装的通用MindSporeLite推理器。
         
         
         ## 开源主页
```

### Comparing `cubetools-0.3.8/README.md` & `cubetools-0.3.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [CubeAI智立方](https://openi.pcl.ac.cn/OpenI/cubeai) 模型和应用开发常用工具集。
 
 目前主要包括：
 
 - 图像前处理、后处理常用函数封装。
 - 支持多路视频流媒体在线AI流式服务的通用SDK组件。
 - 基于Gradio的AI视频流媒体Python前端SDK组件。
-- 基于Gradio的对话式聊天Python前端SDK组件。
+- 基于Gradio的聊天对话式Python前端SDK组件。
 - 基于 [OpenVino Runtime](https://pypi.org/project/openvino/) 封装的通用OpenVino模型推理器。
 - 基于 [ONNX Runtime](https://pypi.org/project/onnxruntime-gpu/) 封装的通用ONNX模型推理器。
 - 基于 [Paddle Inference](https://www.paddlepaddle.org.cn/paddle/paddleinference) 推理引擎封装的通用PaddlePaddle模型推理器。
 - 基于 [MindSpore Lite](https://www.mindspore.cn/lite) 推理引擎封装的通用MindSporeLite推理器。
 
 
 ## 开源主页
```

### Comparing `cubetools-0.3.8/cubetools/image_tools.py` & `cubetools-0.3.9/cubetools/image_tools.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.8/cubetools/mindspore_lite_predict.py` & `cubetools-0.3.9/cubetools/mindspore_lite_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.8/cubetools/onnx_predict.py` & `cubetools-0.3.9/cubetools/onnx_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.8/cubetools/openvino_predict.py` & `cubetools-0.3.9/cubetools/openvino_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.8/cubetools/paddle_predict.py` & `cubetools-0.3.9/cubetools/paddle_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.8/cubetools/python_chat_frontend.py` & `cubetools-0.3.9/cubetools/python_chat_frontend.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,19 +34,19 @@
                 btn_show_api.update(visible=True), btn_hide_api.update(visible=False), api_docs.update(visible=False)),
                                    outputs=[btn_show_api, btn_hide_api, api_docs])
 
                 gr.Markdown('<br/>')
                 if readme:
                     gr.Markdown(open(readme).read())
 
-        # 在launch方法中启动Python前端服务，必须存在
-        def launch(self, **kwargs):
-            self.demo.launch(**kwargs)
+    # 在launch方法中启动Python前端服务，必须存在
+    def launch(self, **kwargs):
+        self.demo.launch(**kwargs)
 
-        def predict(self, text, history):
-            result = serviceboot_client('predict', text=text, history=history)
+    def predict(self, text, history):
+        result = serviceboot_client('predict', text=text, history=history)
 
-            if result['status'] == 'ok':
-                history.append((text, result['value']['response']))
-                return history, ''
+        if result['status'] == 'ok':
+            history.append((text, result['value']['response']))
+            return history, ''
 
-            raise gr.Error(result['value'])
+        raise gr.Error(result['value'])
```

### Comparing `cubetools-0.3.8/cubetools/python_video_frontend.py` & `cubetools-0.3.9/cubetools/python_video_frontend.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.8/cubetools/video_capture.py` & `cubetools-0.3.9/cubetools/video_capture.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.8/cubetools/video_predict.py` & `cubetools-0.3.9/cubetools/video_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.8/cubetools.egg-info/PKG-INFO` & `cubetools-0.3.9/cubetools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: cubetools
-Version: 0.3.8
+Version: 0.3.9
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
-        - 基于Gradio的对话式聊天Python前端SDK组件。
+        - 基于Gradio的聊天对话式Python前端SDK组件。
         - 基于 [OpenVino Runtime](https://pypi.org/project/openvino/) 封装的通用OpenVino模型推理器。
         - 基于 [ONNX Runtime](https://pypi.org/project/onnxruntime-gpu/) 封装的通用ONNX模型推理器。
         - 基于 [Paddle Inference](https://www.paddlepaddle.org.cn/paddle/paddleinference) 推理引擎封装的通用PaddlePaddle模型推理器。
         - 基于 [MindSpore Lite](https://www.mindspore.cn/lite) 推理引擎封装的通用MindSporeLite推理器。
         
         
         ## 开源主页
```

### Comparing `cubetools-0.3.8/setup.py` & `cubetools-0.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 with open("README.md", "r", encoding='utf-8') as file:
     long_description = file.read()
 
 
 setup(
     name='cubetools',
-    version='0.3.8',
+    version='0.3.9',
     author='cubeai',
     author_email='cubeai@163.com',
     description='CubeAI模型开发常用工具集',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     packages=find_packages(),
```

