# Comparing `tmp/nonebot_plugin_cube-1.0.3-py3-none-any.whl.zip` & `tmp/nonebot_plugin_cube-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 8343 bytes, number of entries: 7
+Zip file size: 8341 bytes, number of entries: 7
 -rw-r--r--  2.0 fat     4636 b- defN 80-Jan-01 00:00 nonebot_plugin_cube/__init__.py
 -rw-r--r--  2.0 fat    17263 b- defN 80-Jan-01 00:00 nonebot_plugin_cube/mofang.py
 -rw-r--r--  2.0 fat     2232 b- defN 80-Jan-01 00:00 nonebot_plugin_cube/rank.py
--rw-r--r--  2.0 fat     1094 b- defN 80-Jan-01 00:00 nonebot_plugin_cube-1.0.3.dist-info/LICENSE
--rw-r--r--  2.0 fat     1639 b- defN 80-Jan-01 00:00 nonebot_plugin_cube-1.0.3.dist-info/METADATA
--rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 nonebot_plugin_cube-1.0.3.dist-info/WHEEL
-?rw-r--r--  2.0 fat      601 b- defN 16-Jan-01 00:00 nonebot_plugin_cube-1.0.3.dist-info/RECORD
-7 files, 27553 bytes uncompressed, 7275 bytes compressed:  73.6%
+-rw-r--r--  2.0 fat     1094 b- defN 80-Jan-01 00:00 nonebot_plugin_cube-1.0.4.dist-info/LICENSE
+-rw-r--r--  2.0 fat     1642 b- defN 80-Jan-01 00:00 nonebot_plugin_cube-1.0.4.dist-info/METADATA
+-rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 nonebot_plugin_cube-1.0.4.dist-info/WHEEL
+?rw-r--r--  2.0 fat      601 b- defN 16-Jan-01 00:00 nonebot_plugin_cube-1.0.4.dist-info/RECORD
+7 files, 27556 bytes uncompressed, 7273 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: nonebot_plugin_cube/mofang.py
 Comment: 
 
 Filename: nonebot_plugin_cube/rank.py
 Comment: 
 
-Filename: nonebot_plugin_cube-1.0.3.dist-info/LICENSE
+Filename: nonebot_plugin_cube-1.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: nonebot_plugin_cube-1.0.3.dist-info/METADATA
+Filename: nonebot_plugin_cube-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: nonebot_plugin_cube-1.0.3.dist-info/WHEEL
+Filename: nonebot_plugin_cube-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: nonebot_plugin_cube-1.0.3.dist-info/RECORD
+Filename: nonebot_plugin_cube-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `nonebot_plugin_cube-1.0.3.dist-info/LICENSE` & `nonebot_plugin_cube-1.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `nonebot_plugin_cube-1.0.3.dist-info/METADATA` & `nonebot_plugin_cube-1.0.4.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-cube
-Version: 1.0.3
+Version: 1.0.4
 Summary: "Rubik's Cube plugin based on nonebot framework,基于nonebot框架的魔方插件"
 License: MIT
 Author: initialencounter
 Author-email: 2911583893@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pillow (>=9.3.0,<10.0.0)
-Requires-Dist: cube (>=0.0.3,<0.0.4)
+Requires-Dist: nonebot (>=1.5.9,<2.0.0)
 Requires-Dist: nonebot2 (>=2.0.0rc2,<3.0.0)
 Requires-Dist: numpy (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # nonebot-plugin-cube
 Rubik's Cube plugin based on nonebot framework,基于nonebot框架的魔方插件
```

