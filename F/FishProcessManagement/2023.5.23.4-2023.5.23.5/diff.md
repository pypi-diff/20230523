# Comparing `tmp/FishProcessManagement-2023.5.23.4.tar.gz` & `tmp/FishProcessManagement-2023.5.23.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FishProcessManagement-2023.5.23.4.tar", last modified: Tue May 23 08:36:47 2023, max compression
+gzip compressed data, was "FishProcessManagement-2023.5.23.5.tar", last modified: Tue May 23 09:59:50 2023, max compression
```

## Comparing `FishProcessManagement-2023.5.23.4.tar` & `FishProcessManagement-2023.5.23.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 08:36:47.383651 FishProcessManagement-2023.5.23.4/
-drwxrwxrwx   0        0        0        0 2023-05-23 08:36:47.361095 FishProcessManagement-2023.5.23.4/FishProcessManagement/
--rw-rw-rw-   0        0        0     2336 2023-05-23 08:24:04.000000 FishProcessManagement-2023.5.23.4/FishProcessManagement/__init__.py
--rw-rw-rw-   0        0        0      676 2023-05-22 13:15:50.000000 FishProcessManagement-2023.5.23.4/FishProcessManagement/child.py
--rw-rw-rw-   0        0        0      160 2023-05-23 08:33:06.000000 FishProcessManagement-2023.5.23.4/FishProcessManagement/test.py
-drwxrwxrwx   0        0        0        0 2023-05-23 08:36:47.376669 FishProcessManagement-2023.5.23.4/FishProcessManagement.egg-info/
--rw-rw-rw-   0        0        0     1771 2023-05-23 08:36:47.000000 FishProcessManagement-2023.5.23.4/FishProcessManagement.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-05-23 08:36:47.000000 FishProcessManagement-2023.5.23.4/FishProcessManagement.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 08:36:47.000000 FishProcessManagement-2023.5.23.4/FishProcessManagement.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-05-23 08:36:47.000000 FishProcessManagement-2023.5.23.4/FishProcessManagement.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1771 2023-05-23 08:36:47.382654 FishProcessManagement-2023.5.23.4/PKG-INFO
--rw-rw-rw-   0        0        0     1358 2023-05-23 08:36:14.000000 FishProcessManagement-2023.5.23.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-23 08:36:47.384648 FishProcessManagement-2023.5.23.4/setup.cfg
--rw-rw-rw-   0        0        0     1002 2023-05-23 08:36:14.000000 FishProcessManagement-2023.5.23.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:59:50.039061 FishProcessManagement-2023.5.23.5/
+drwxrwxrwx   0        0        0        0 2023-05-23 09:59:50.024096 FishProcessManagement-2023.5.23.5/FishProcessManagement/
+-rw-rw-rw-   0        0        0     2645 2023-05-23 09:49:29.000000 FishProcessManagement-2023.5.23.5/FishProcessManagement/__init__.py
+-rw-rw-rw-   0        0        0      676 2023-05-22 13:15:50.000000 FishProcessManagement-2023.5.23.5/FishProcessManagement/child.py
+-rw-rw-rw-   0        0        0      214 2023-05-23 08:39:06.000000 FishProcessManagement-2023.5.23.5/FishProcessManagement/test.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:59:50.035066 FishProcessManagement-2023.5.23.5/FishProcessManagement.egg-info/
+-rw-rw-rw-   0        0        0     1734 2023-05-23 09:59:49.000000 FishProcessManagement-2023.5.23.5/FishProcessManagement.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-05-23 09:59:49.000000 FishProcessManagement-2023.5.23.5/FishProcessManagement.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 09:59:49.000000 FishProcessManagement-2023.5.23.5/FishProcessManagement.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-23 09:59:49.000000 FishProcessManagement-2023.5.23.5/FishProcessManagement.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1734 2023-05-23 09:59:50.037061 FishProcessManagement-2023.5.23.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1321 2023-05-23 09:59:04.000000 FishProcessManagement-2023.5.23.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-23 09:59:50.039061 FishProcessManagement-2023.5.23.5/setup.cfg
+-rw-rw-rw-   0        0        0     1002 2023-05-23 09:50:22.000000 FishProcessManagement-2023.5.23.5/setup.py
```

### Comparing `FishProcessManagement-2023.5.23.4/FishProcessManagement/__init__.py` & `FishProcessManagement-2023.5.23.5/FishProcessManagement/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 import os
 import subprocess
-import signal
 
 
 def 停止子进程(进程):
     if os.name == 'nt':
         subprocess.run(['taskkill', '/F', '/T', '/PID', str(进程.pid)], shell=True)
     else:
         def 杀死进程树(pid):
             # 查找进程及其子进程的PID列表
             子进程pid列表 = os.popen('pgrep -P {}'.format(pid)).read().splitlines()
-
             # 递归终止进程及其子进程
             for 子进程pid in 子进程pid列表:
                 杀死进程树(子进程pid)
-
             # 终止给定PID的进程
             os.system('kill -9 {}'.format(pid))
 
         杀死进程树(进程.pid)
 
 
 def 启动子进程(命令):
@@ -26,48 +23,56 @@
         shell = True
     else:
         shell = False
     进程 = subprocess.Popen(命令, shell=shell)
     return 进程, 进程.pid
 
 
+def 显示进程池信息(进程池):
+    print("当前进程池状态:")
+    print("进程名\t\t进程ID\t\t已停止")
+    for 进程名, (进程, pid, 已停止) in 进程池.items():
+        print(f"{进程名}\t\t{pid}\t\t{已停止}")
+    print()
+
+
 def 进程管理器(进程列表):
     print("""
             Fishconsole 进程管理器 Versition(20230523)
 
                                             By 鱼鱼
     """)
-    进程池 = []
-    进程名池 = []
-    for 进程 in 进程列表:
-        进程名池.append(进程[0])
+    进程池 = {}
+
     while True:
         命令 = input("请输入命令：")
         命令列表 = 命令.split(" ")
         if 命令列表[0] == "关闭":
             进程名 = 命令列表[1]
-            try:
-                进程索引 = 进程名池.index(进程名)
-                进程, pid = 进程池[进程索引]
-                停止子进程(进程)
-                进程名池.remove(进程名)
-                进程池.remove([进程, pid])
-                print("进程已关闭")
-            except ValueError:
+            if 进程名 in 进程池:
+                进程, pid, 已停止 = 进程池[进程名]
+                if not 已停止:
+                    停止子进程(进程)
+                    进程池[进程名] = (进程, pid, True)
+                    print("进程已关闭")
+                else:
+                    print("进程已经处于关闭状态")
+                显示进程池信息(进程池)
+            else:
                 print("找不到对应的进程名字")
         elif 命令列表[0] == "启动":
             进程名 = 命令列表[1]
-            try:
-                进程索引 = 进程名池.index(进程名)
-                进程, pid = 启动子进程(进程列表[进程索引][1])
-                进程池.append((进程, pid))
-            except ValueError:
+            if 进程名 in 进程列表:
+                命令 = 进程列表[进程名]
+                进程, pid = 启动子进程(命令)
+                进程池[进程名] = (进程, pid, False)
+                print("进程已启动")
+                显示进程池信息(进程池)
+            else:
                 print("找不到对应的进程名字")
         else:
             print("无效的命令")
-
-
-# 进程列表 = [
-#         ['第一个进程', ['python', 'child.py']],
-#         # 其他进程信息
-#     ]
-# 进程管理器(进程列表)
+进程列表 = {
+    '第一个进程': ['python', 'child.py'],
+    # 其他进程信息
+    }
+进程管理器(进程列表)
```

### Comparing `FishProcessManagement-2023.5.23.4/FishProcessManagement/child.py` & `FishProcessManagement-2023.5.23.5/FishProcessManagement/child.py`

 * *Files identical despite different names*

### Comparing `FishProcessManagement-2023.5.23.4/FishProcessManagement.egg-info/PKG-INFO` & `FishProcessManagement-2023.5.23.5/FishProcessManagement.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 Metadata-Version: 2.1
 Name: FishProcessManagement
-Version: 2023.5.23.4
+Version: 2023.5.23.5
 Summary: 一个后台项目管理器，适用于启动或关闭多个毫不相关的项目，注意他不是函数，只允许启动时指定程序的位置
 Home-page: https://space.bilibili.com/698117971?spm_id_from=333.1007.0.0
 Author: FishProcessManagement
 Author-email: 2645602049@qq.com
 Description-Content-Type: text/markdown
 
->  我利用了几乎所有的业余时间设计了Fishconsole Project，虽然现在十分拉跨，但正努力前行
-
-- 它是一个启动python项目的工具
+>它是一个启动python项目的工具
 ----
 
 # 🦈FishProcessManagement 小鱼进程管理器功能一览
 ##### 
 - 启动 你的项目名
 - 关闭 你的项目名
 ------------
 
 
 
-- 主进程
+- 主进程(在进程管理器中使用的代码)
 
+```
 
 import FishProcessManagement
+
 进程列表 = [
 ['第一个进程', ['python', 'child.py']],
 ]
+
 FishProcessManagement.进程管理器(进程列表)
 
+```
 
 
 
 
 
 
 
-- 子进程
+- 子进程（示例的子进程代码）
+```
 
 import multiprocessing
 import time
 
 def worker(num):
     """子进程"""
     print('子进程 %d 开始执行' % num)
@@ -51,28 +54,28 @@
        print('子进程正在运行')
 
 def sub_worker(num):
     """子子进程"""
     while True:
        time.sleep(1)
        print('子子进程 %d 开始执行' % num)
-    
+
    
 
 def main():
     # 主进程
     print('主进程开始执行')
     process1 = multiprocessing.Process(target=worker, args=(1,))
     process1.start()
     process1.join()
     print('主进程执行完毕')
 
 if __name__ == '__main__':
     main()
-
+```
 
 
 
 -----------
```

### Comparing `FishProcessManagement-2023.5.23.4/PKG-INFO` & `FishProcessManagement-2023.5.23.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 Metadata-Version: 2.1
 Name: FishProcessManagement
-Version: 2023.5.23.4
+Version: 2023.5.23.5
 Summary: 一个后台项目管理器，适用于启动或关闭多个毫不相关的项目，注意他不是函数，只允许启动时指定程序的位置
 Home-page: https://space.bilibili.com/698117971?spm_id_from=333.1007.0.0
 Author: FishProcessManagement
 Author-email: 2645602049@qq.com
 Description-Content-Type: text/markdown
 
->  我利用了几乎所有的业余时间设计了Fishconsole Project，虽然现在十分拉跨，但正努力前行
-
-- 它是一个启动python项目的工具
+>它是一个启动python项目的工具
 ----
 
 # 🦈FishProcessManagement 小鱼进程管理器功能一览
 ##### 
 - 启动 你的项目名
 - 关闭 你的项目名
 ------------
 
 
 
-- 主进程
+- 主进程(在进程管理器中使用的代码)
 
+```
 
 import FishProcessManagement
+
 进程列表 = [
 ['第一个进程', ['python', 'child.py']],
 ]
+
 FishProcessManagement.进程管理器(进程列表)
 
+```
 
 
 
 
 
 
 
-- 子进程
+- 子进程（示例的子进程代码）
+```
 
 import multiprocessing
 import time
 
 def worker(num):
     """子进程"""
     print('子进程 %d 开始执行' % num)
@@ -51,28 +54,28 @@
        print('子进程正在运行')
 
 def sub_worker(num):
     """子子进程"""
     while True:
        time.sleep(1)
        print('子子进程 %d 开始执行' % num)
-    
+
    
 
 def main():
     # 主进程
     print('主进程开始执行')
     process1 = multiprocessing.Process(target=worker, args=(1,))
     process1.start()
     process1.join()
     print('主进程执行完毕')
 
 if __name__ == '__main__':
     main()
-
+```
 
 
 
 -----------
```

### Comparing `FishProcessManagement-2023.5.23.4/README.md` & `FishProcessManagement-2023.5.23.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,40 @@
->  我利用了几乎所有的业余时间设计了Fishconsole Project，虽然现在十分拉跨，但正努力前行
-
-- 它是一个启动python项目的工具
+>它是一个启动python项目的工具
 ----
 
 # 🦈FishProcessManagement 小鱼进程管理器功能一览
 ##### 
 - 启动 你的项目名
 - 关闭 你的项目名
 ------------
 
 
 
-- 主进程
+- 主进程(在进程管理器中使用的代码)
 
+```
 
 import FishProcessManagement
+
 进程列表 = [
 ['第一个进程', ['python', 'child.py']],
 ]
+
 FishProcessManagement.进程管理器(进程列表)
 
+```
 
 
 
 
 
 
 
-- 子进程
+- 子进程（示例的子进程代码）
+```
 
 import multiprocessing
 import time
 
 def worker(num):
     """子进程"""
     print('子进程 %d 开始执行' % num)
@@ -42,28 +45,28 @@
        print('子进程正在运行')
 
 def sub_worker(num):
     """子子进程"""
     while True:
        time.sleep(1)
        print('子子进程 %d 开始执行' % num)
-    
+
    
 
 def main():
     # 主进程
     print('主进程开始执行')
     process1 = multiprocessing.Process(target=worker, args=(1,))
     process1.start()
     process1.join()
     print('主进程执行完毕')
 
 if __name__ == '__main__':
     main()
-
+```
 
 
 
 -----------
```

### Comparing `FishProcessManagement-2023.5.23.4/setup.py` & `FishProcessManagement-2023.5.23.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 filepath = 'README.md'
 
 # python setup.py bdist_wheel # 打包为whl文件
 # python setup.py sdist # 打包为tar.gz文件
 
 setup(
     name="FishProcessManagement",
-    version="2023.5.23.4",
+    version="2023.5.23.5",
     author="FishProcessManagement",
     author_email="2645602049@qq.com",
     description="一个后台项目管理器，适用于启动或关闭多个毫不相关的项目，注意他不是函数，只允许启动时指定程序的位置",
 
     # 项目主页
     url="https://space.bilibili.com/698117971?spm_id_from=333.1007.0.0",
     # 长描述
```

