# Comparing `tmp/nonebot-plugin-puzzle-1.0.1.tar.gz` & `tmp/nonebot-plugin-puzzle-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-puzzle-1.0.1.tar", last modified: Tue May 23 20:05:39 2023, max compression
+gzip compressed data, was "nonebot-plugin-puzzle-1.0.2.tar", last modified: Tue May 23 20:38:46 2023, max compression
```

## Comparing `nonebot-plugin-puzzle-1.0.1.tar` & `nonebot-plugin-puzzle-1.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1073 2023-05-23 20:05:31.627085 nonebot-plugin-puzzle-1.0.1/LICENSE
--rw-r--r--   0        0        0      998 2023-05-23 20:05:31.627085 nonebot-plugin-puzzle-1.0.1/README.md
--rw-r--r--   0        0        0     5021 2023-05-23 20:05:31.627085 nonebot-plugin-puzzle-1.0.1/nonebot_plugin_puzzle/__init__.py
--rw-r--r--   0        0        0     4408 2023-05-23 20:05:31.627085 nonebot-plugin-puzzle-1.0.1/nonebot_plugin_puzzle/puzzle.py
--rw-r--r--   0        0        0     2214 2023-05-23 20:05:31.627085 nonebot-plugin-puzzle-1.0.1/nonebot_plugin_puzzle/rank.py
--rw-r--r--   0        0        0    41615 2023-05-23 20:05:31.627085 nonebot-plugin-puzzle-1.0.1/nonebot_plugin_puzzle/theme/33.png
--rw-r--r--   0        0        0    64289 2023-05-23 20:05:31.631085 nonebot-plugin-puzzle-1.0.1/nonebot_plugin_puzzle/theme/44.png
--rw-r--r--   0        0        0    97028 2023-05-23 20:05:31.631085 nonebot-plugin-puzzle-1.0.1/nonebot_plugin_puzzle/theme/55.png
--rw-r--r--   0        0        0      684 2023-05-23 20:05:31.631085 nonebot-plugin-puzzle-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1479 1970-01-01 00:00:00.000000 nonebot-plugin-puzzle-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-23 20:38:38.058282 nonebot-plugin-puzzle-1.0.2/LICENSE
+-rw-r--r--   0        0        0      998 2023-05-23 20:38:38.058282 nonebot-plugin-puzzle-1.0.2/README.md
+-rw-r--r--   0        0        0     5021 2023-05-23 20:38:38.058282 nonebot-plugin-puzzle-1.0.2/nonebot_plugin_puzzle/__init__.py
+-rw-r--r--   0        0        0     4457 2023-05-23 20:38:38.058282 nonebot-plugin-puzzle-1.0.2/nonebot_plugin_puzzle/puzzle.py
+-rw-r--r--   0        0        0     2214 2023-05-23 20:38:38.058282 nonebot-plugin-puzzle-1.0.2/nonebot_plugin_puzzle/rank.py
+-rw-r--r--   0        0        0    41615 2023-05-23 20:38:38.058282 nonebot-plugin-puzzle-1.0.2/nonebot_plugin_puzzle/theme/33.png
+-rw-r--r--   0        0        0    64289 2023-05-23 20:38:38.058282 nonebot-plugin-puzzle-1.0.2/nonebot_plugin_puzzle/theme/44.png
+-rw-r--r--   0        0        0    97028 2023-05-23 20:38:38.058282 nonebot-plugin-puzzle-1.0.2/nonebot_plugin_puzzle/theme/55.png
+-rw-r--r--   0        0        0      684 2023-05-23 20:38:38.058282 nonebot-plugin-puzzle-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1479 1970-01-01 00:00:00.000000 nonebot-plugin-puzzle-1.0.2/PKG-INFO
```

### Comparing `nonebot-plugin-puzzle-1.0.1/LICENSE` & `nonebot-plugin-puzzle-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-puzzle-1.0.1/README.md` & `nonebot-plugin-puzzle-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-puzzle-1.0.1/nonebot_plugin_puzzle/__init__.py` & `nonebot-plugin-puzzle-1.0.2/nonebot_plugin_puzzle/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-puzzle-1.0.1/nonebot_plugin_puzzle/puzzle.py` & `nonebot-plugin-puzzle-1.0.2/nonebot_plugin_puzzle/puzzle.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-from os.path import exists, abspath, join as os_join
+from os.path import exists, abspath,dirname, join as os_join
 from PIL import Image
 from random import randint
 from time import time,gmtime,strftime
 from io import BytesIO
 class Klotsk:
 
     def __init__(self, mode):
         self.cmd_strs = ''
         self.theme = []
         if exists(f'./src/plugins/klotsk/theme/{mode}{mode}.png'):
             img = Image.open(f'./src/plugins/klotsk/theme/{mode}{mode}.png')
         else:
             module_path = abspath(__file__)
-            img_path = os_join(module_path,f'theme/{mode}{mode}.png')
+            dir_path = dirname(module_path)
+            img_path = os_join(dir_path,f'theme/{mode}{mode}.png')
             img = Image.open(img_path)
         self.sl = 720 / mode
         for i in range(mode):                               # 剪切图片
             for j in range(mode):
                 self.theme.append(img.crop((j * self.sl, i * self.sl, (j + 1) * self.sl, (i + 1) * self.sl)))
         self.drctn_dist = {'U': [-1, 0], 'D': [1, 0], 'L': [0, -1], 'R': [0, 1]}
         self.drctn_list = ['U', 'D', 'L', 'R']
```

### Comparing `nonebot-plugin-puzzle-1.0.1/nonebot_plugin_puzzle/rank.py` & `nonebot-plugin-puzzle-1.0.2/nonebot_plugin_puzzle/rank.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-puzzle-1.0.1/nonebot_plugin_puzzle/theme/33.png` & `nonebot-plugin-puzzle-1.0.2/nonebot_plugin_puzzle/theme/33.png`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-puzzle-1.0.1/nonebot_plugin_puzzle/theme/44.png` & `nonebot-plugin-puzzle-1.0.2/nonebot_plugin_puzzle/theme/44.png`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-puzzle-1.0.1/nonebot_plugin_puzzle/theme/55.png` & `nonebot-plugin-puzzle-1.0.2/nonebot_plugin_puzzle/theme/55.png`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-puzzle-1.0.1/pyproject.toml` & `nonebot-plugin-puzzle-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-puzzle"
-version = "1.0.1"
+version = "1.0.2"
 description = "在QQ群玩数字华容道，基于nonebot框架的数字华容道插件，plugin of puzzle base on nonebot frame"
 authors = [
     { name = "initialencounter", email = "2911583893@qq.com" },
 ]
 license = "MIT"
 dependencies = [
     "nonebot2>=2.0.0b2",
```

### Comparing `nonebot-plugin-puzzle-1.0.1/PKG-INFO` & `nonebot-plugin-puzzle-1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-puzzle
-Version: 1.0.1
+Version: 1.0.2
 Summary: 在QQ群玩数字华容道，基于nonebot框架的数字华容道插件，plugin of puzzle base on nonebot frame
 License: MIT
 Author-email: initialencounter <2911583893@qq.com>
 Requires-Python: >=3.8
 Project-URL: Homepage, https://github.com/initialencounter/nonebot-plugin-puzzle
 Project-URL: Repository, https://github.com/initialencounter/nonebot-plugin-puzzle
 Description-Content-Type: text/markdown
```

