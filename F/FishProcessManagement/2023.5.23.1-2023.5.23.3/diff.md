# Comparing `tmp/FishProcessManagement-2023.5.23.1.tar.gz` & `tmp/FishProcessManagement-2023.5.23.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FishProcessManagement-2023.5.23.1.tar", last modified: Tue May 23 08:17:25 2023, max compression
+gzip compressed data, was "FishProcessManagement-2023.5.23.3.tar", last modified: Tue May 23 08:28:53 2023, max compression
```

## Comparing `FishProcessManagement-2023.5.23.1.tar` & `FishProcessManagement-2023.5.23.3.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 08:17:25.813351 FishProcessManagement-2023.5.23.1/
-drwxrwxrwx   0        0        0        0 2023-05-23 08:17:25.794926 FishProcessManagement-2023.5.23.1/FishProcessManagement/
--rw-rw-rw-   0        0        0       28 2023-05-23 07:52:21.000000 FishProcessManagement-2023.5.23.1/FishProcessManagement/__init__.py
--rw-rw-rw-   0        0        0      676 2023-05-22 13:15:50.000000 FishProcessManagement-2023.5.23.1/FishProcessManagement/child.py
--rw-rw-rw-   0        0        0     2264 2023-05-23 08:13:12.000000 FishProcessManagement-2023.5.23.1/FishProcessManagement/main.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:17:25.810352 FishProcessManagement-2023.5.23.1/FishProcessManagement.egg-info/
--rw-rw-rw-   0        0        0     1765 2023-05-23 08:17:25.000000 FishProcessManagement-2023.5.23.1/FishProcessManagement.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-05-23 08:17:25.000000 FishProcessManagement-2023.5.23.1/FishProcessManagement.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 08:17:25.000000 FishProcessManagement-2023.5.23.1/FishProcessManagement.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-05-23 08:17:25.000000 FishProcessManagement-2023.5.23.1/FishProcessManagement.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1765 2023-05-23 08:17:25.812350 FishProcessManagement-2023.5.23.1/PKG-INFO
--rw-rw-rw-   0        0        0     1352 2023-05-23 07:58:30.000000 FishProcessManagement-2023.5.23.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-23 08:17:25.813351 FishProcessManagement-2023.5.23.1/setup.cfg
--rw-rw-rw-   0        0        0      901 2023-05-23 08:15:50.000000 FishProcessManagement-2023.5.23.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 08:28:53.848570 FishProcessManagement-2023.5.23.3/
+drwxrwxrwx   0        0        0        0 2023-05-23 08:28:53.830969 FishProcessManagement-2023.5.23.3/FishProcessManagement/
+-rw-rw-rw-   0        0        0     2336 2023-05-23 08:24:04.000000 FishProcessManagement-2023.5.23.3/FishProcessManagement/__init__.py
+-rw-rw-rw-   0        0        0      676 2023-05-22 13:15:50.000000 FishProcessManagement-2023.5.23.3/FishProcessManagement/child.py
+drwxrwxrwx   0        0        0        0 2023-05-23 08:28:53.844608 FishProcessManagement-2023.5.23.3/FishProcessManagement.egg-info/
+-rw-rw-rw-   0        0        0     1765 2023-05-23 08:28:53.000000 FishProcessManagement-2023.5.23.3/FishProcessManagement.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-05-23 08:28:53.000000 FishProcessManagement-2023.5.23.3/FishProcessManagement.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 08:28:53.000000 FishProcessManagement-2023.5.23.3/FishProcessManagement.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-23 08:28:53.000000 FishProcessManagement-2023.5.23.3/FishProcessManagement.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1765 2023-05-23 08:28:53.847572 FishProcessManagement-2023.5.23.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1352 2023-05-23 07:58:30.000000 FishProcessManagement-2023.5.23.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-23 08:28:53.848570 FishProcessManagement-2023.5.23.3/setup.cfg
+-rw-rw-rw-   0        0        0     1002 2023-05-23 08:28:35.000000 FishProcessManagement-2023.5.23.3/setup.py
```

### Comparing `FishProcessManagement-2023.5.23.1/FishProcessManagement/child.py` & `FishProcessManagement-2023.5.23.3/FishProcessManagement/child.py`

 * *Files identical despite different names*

### Comparing `FishProcessManagement-2023.5.23.1/FishProcessManagement/main.py` & `FishProcessManagement-2023.5.23.3/FishProcessManagement/__init__.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-import os
-import subprocess
-import signal
-
-
-def 停止子进程(进程):
-    if os.name == 'nt':
-        subprocess.run(['taskkill', '/F', '/T', '/PID', str(进程.pid)], shell=True)
-    else:
-        def 杀死进程树(pid):
-            # 查找进程及其子进程的PID列表
-            子进程pid列表 = os.popen('pgrep -P {}'.format(pid)).read().splitlines()
-
-            # 递归终止进程及其子进程
-            for 子进程pid in 子进程pid列表:
-                杀死进程树(子进程pid)
-
-            # 终止给定PID的进程
-            os.system('kill -9 {}'.format(pid))
-
-        杀死进程树(进程.pid)
-
-
-def 启动子进程(命令):
-    if os.name == 'nt':
-        shell = True
-    else:
-        shell = False
-    进程 = subprocess.Popen(命令, shell=shell)
-    return 进程, 进程.pid
-
-
-def 进程管理器(进程列表):
-    print("""
-            Fishconsole 进程管理器 Versition(20230523)
-
-                                            By 鱼鱼
-    """)
-    进程池 = []
-    进程名池 = []
-    for 进程 in 进程列表:
-        进程名池.append(进程[0])
-    while True:
-        命令 = input("请输入命令：")
-        命令列表 = 命令.split(" ")
-        if 命令列表[0] == "关闭":
-            进程名 = 命令列表[1]
-            try:
-                进程索引 = 进程名池.index(进程名)
-                进程, pid = 进程池[进程索引]
-                停止子进程(进程)
-                进程名池.remove(进程名)
-                进程池.remove([进程, pid])
-                print("进程已关闭")
-            except ValueError:
-                print("找不到对应的进程名字")
-        elif 命令列表[0] == "启动":
-            进程名 = 命令列表[1]
-            try:
-                进程索引 = 进程名池.index(进程名)
-                进程, pid = 启动子进程(进程列表[进程索引][1])
-                进程池.append((进程, pid))
-            except ValueError:
-                print("找不到对应的进程名字")
-        else:
-            print("无效的命令")
-
-
-# 进程列表 = [
-#         ['第一个进程', ['python', 'child.py']],
-#         # 其他进程信息
-#     ]
+import os
+import subprocess
+import signal
+
+
+def 停止子进程(进程):
+    if os.name == 'nt':
+        subprocess.run(['taskkill', '/F', '/T', '/PID', str(进程.pid)], shell=True)
+    else:
+        def 杀死进程树(pid):
+            # 查找进程及其子进程的PID列表
+            子进程pid列表 = os.popen('pgrep -P {}'.format(pid)).read().splitlines()
+
+            # 递归终止进程及其子进程
+            for 子进程pid in 子进程pid列表:
+                杀死进程树(子进程pid)
+
+            # 终止给定PID的进程
+            os.system('kill -9 {}'.format(pid))
+
+        杀死进程树(进程.pid)
+
+
+def 启动子进程(命令):
+    if os.name == 'nt':
+        shell = True
+    else:
+        shell = False
+    进程 = subprocess.Popen(命令, shell=shell)
+    return 进程, 进程.pid
+
+
+def 进程管理器(进程列表):
+    print("""
+            Fishconsole 进程管理器 Versition(20230523)
+
+                                            By 鱼鱼
+    """)
+    进程池 = []
+    进程名池 = []
+    for 进程 in 进程列表:
+        进程名池.append(进程[0])
+    while True:
+        命令 = input("请输入命令：")
+        命令列表 = 命令.split(" ")
+        if 命令列表[0] == "关闭":
+            进程名 = 命令列表[1]
+            try:
+                进程索引 = 进程名池.index(进程名)
+                进程, pid = 进程池[进程索引]
+                停止子进程(进程)
+                进程名池.remove(进程名)
+                进程池.remove([进程, pid])
+                print("进程已关闭")
+            except ValueError:
+                print("找不到对应的进程名字")
+        elif 命令列表[0] == "启动":
+            进程名 = 命令列表[1]
+            try:
+                进程索引 = 进程名池.index(进程名)
+                进程, pid = 启动子进程(进程列表[进程索引][1])
+                进程池.append((进程, pid))
+            except ValueError:
+                print("找不到对应的进程名字")
+        else:
+            print("无效的命令")
+
+
+# 进程列表 = [
+#         ['第一个进程', ['python', 'child.py']],
+#         # 其他进程信息
+#     ]
 # 进程管理器(进程列表)
```

### Comparing `FishProcessManagement-2023.5.23.1/FishProcessManagement.egg-info/PKG-INFO` & `FishProcessManagement-2023.5.23.3/FishProcessManagement.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FishProcessManagement
-Version: 2023.5.23.1
+Version: 2023.5.23.3
 Summary: 一个后台项目管理器，适用于启动或关闭多个毫不相关的项目，注意他不是函数，只允许启动时指定程序的位置
 Home-page: https://space.bilibili.com/698117971?spm_id_from=333.1007.0.0
 Author: FishProcessManagement
 Author-email: 2645602049@qq.com
 Description-Content-Type: text/markdown
 
 >  我利用了几乎所有的业余时间设计了Fishconsole Project，虽然现在十分拉跨，但正努力前行
```

### Comparing `FishProcessManagement-2023.5.23.1/PKG-INFO` & `FishProcessManagement-2023.5.23.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FishProcessManagement
-Version: 2023.5.23.1
+Version: 2023.5.23.3
 Summary: 一个后台项目管理器，适用于启动或关闭多个毫不相关的项目，注意他不是函数，只允许启动时指定程序的位置
 Home-page: https://space.bilibili.com/698117971?spm_id_from=333.1007.0.0
 Author: FishProcessManagement
 Author-email: 2645602049@qq.com
 Description-Content-Type: text/markdown
 
 >  我利用了几乎所有的业余时间设计了Fishconsole Project，虽然现在十分拉跨，但正努力前行
```

### Comparing `FishProcessManagement-2023.5.23.1/README.md` & `FishProcessManagement-2023.5.23.3/README.md`

 * *Files identical despite different names*

### Comparing `FishProcessManagement-2023.5.23.1/setup.py` & `FishProcessManagement-2023.5.23.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from setuptools import setup, find_packages
 
 
 filepath = 'README.md'
 
+# python setup.py bdist_wheel # 打包为whl文件
+# python setup.py sdist # 打包为tar.gz文件
 
 setup(
     name="FishProcessManagement",
-    version="2023.5.23.1",
+    version="2023.5.23.3",
     author="FishProcessManagement",
     author_email="2645602049@qq.com",
     description="一个后台项目管理器，适用于启动或关闭多个毫不相关的项目，注意他不是函数，只允许启动时指定程序的位置",
 
     # 项目主页
     url="https://space.bilibili.com/698117971?spm_id_from=333.1007.0.0",
     # 长描述
```

