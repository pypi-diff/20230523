# Comparing `tmp/upconan-1.0.4.tar.gz` & `tmp/upconan-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upconan-1.0.4.tar", last modified: Mon May 22 07:34:02 2023, max compression
+gzip compressed data, was "upconan-1.0.5.tar", last modified: Tue May 23 06:34:53 2023, max compression
```

## Comparing `upconan-1.0.4.tar` & `upconan-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 07:34:02.214092 upconan-1.0.4/
--rw-rw-rw-   0        0        0     1062 2023-05-19 13:12:37.000000 upconan-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      490 2023-05-22 07:34:02.213088 upconan-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      124 2023-05-19 13:13:20.000000 upconan-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-22 07:34:02.214092 upconan-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      861 2023-05-22 07:34:00.000000 upconan-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 07:34:02.205094 upconan-1.0.4/src/
--rw-rw-rw-   0        0        0        0 2023-04-18 02:21:11.000000 upconan-1.0.4/src/__init__.py
--rw-rw-rw-   0        0        0     4913 2023-05-22 07:32:27.000000 upconan-1.0.4/src/upconan.py
-drwxrwxrwx   0        0        0        0 2023-05-22 07:34:02.213088 upconan-1.0.4/upconan.egg-info/
--rw-rw-rw-   0        0        0      490 2023-05-22 07:34:02.000000 upconan-1.0.4/upconan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-05-22 07:34:02.000000 upconan-1.0.4/upconan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 07:34:02.000000 upconan-1.0.4/upconan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-05-22 07:34:02.000000 upconan-1.0.4/upconan.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-22 07:32:48.000000 upconan-1.0.4/upconan.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       20 2023-05-22 07:34:02.000000 upconan-1.0.4/upconan.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-22 07:34:02.000000 upconan-1.0.4/upconan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 06:34:53.085477 upconan-1.0.5/
+-rw-rw-rw-   0        0        0     1062 2023-05-19 13:12:37.000000 upconan-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0      490 2023-05-23 06:34:53.084632 upconan-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2023-05-19 13:13:20.000000 upconan-1.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-23 06:34:53.085477 upconan-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      861 2023-05-23 06:34:30.000000 upconan-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 06:34:53.073632 upconan-1.0.5/src/
+-rw-rw-rw-   0        0        0        0 2023-04-18 02:21:11.000000 upconan-1.0.5/src/__init__.py
+-rw-rw-rw-   0        0        0     4799 2023-05-23 06:33:57.000000 upconan-1.0.5/src/upconan.py
+drwxrwxrwx   0        0        0        0 2023-05-23 06:34:53.084632 upconan-1.0.5/upconan.egg-info/
+-rw-rw-rw-   0        0        0      490 2023-05-23 06:34:53.000000 upconan-1.0.5/upconan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-05-23 06:34:53.000000 upconan-1.0.5/upconan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 06:34:53.000000 upconan-1.0.5/upconan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-05-23 06:34:53.000000 upconan-1.0.5/upconan.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-23 06:34:53.000000 upconan-1.0.5/upconan.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       20 2023-05-23 06:34:53.000000 upconan-1.0.5/upconan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-23 06:34:53.000000 upconan-1.0.5/upconan.egg-info/top_level.txt
```

### Comparing `upconan-1.0.4/LICENSE` & `upconan-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `upconan-1.0.4/setup.py` & `upconan-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 from setuptools import setup, find_packages
 
 setup(
     name='upconan',
-    version="1.0.4",
+    version="1.0.5",
     description="一个更新conanfile的便捷工具",
     long_description="""从剪贴板复制conan包信息，更新当前路径下的conanfile.py或conanfile.txt文件中对应的conan包版本""",
     long_description_content_type='text/x-rst',
     keywords='python conan',
     author='leytou',
     author_email='hi_litao@163.com',
     url='https://github.com/leytou/upconan',
```

### Comparing `upconan-1.0.4/src/upconan.py` & `upconan-1.0.5/src/upconan.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,19 +65,16 @@
         result_dict = result.groupdict()
         result_list.append(result_dict)
     return result_list
 
 
 def FindTargetPackageInfo(curent_package_info , target_package_infos):
     for target_package_info in  target_package_infos:
-        if curent_package_info['name'] == target_package_info['name'] and curent_package_info['version'] != target_package_info['version']:
-            if curent_package_info['owner'] == target_package_info['owner']:
-                return target_package_info
-            else:
-                print("waring: not same owner!")
+        if curent_package_info['name'] == target_package_info['name'] and curent_package_info['owner'] == target_package_info['owner']:
+            return target_package_info
     return None
 
 
 def UpdatePackageInfoLine(line,curent_package_info, target_package_info ):
     updated_line =  line.replace(curent_package_info['version'], target_package_info['version'])
     if curent_package_info['channel']:
         updated_line =  updated_line.replace(curent_package_info['channel'], target_package_info['channel'])
@@ -85,23 +82,20 @@
 
 is_changed = False
 def UpdatePackageInfoLines(lines, target_package_infos):
     global is_changed
     for idx, line in enumerate(lines):
         curent_package_info = ParsePackageInfoLine(line)
         if curent_package_info:
-            target_package_info =FindTargetPackageInfo(curent_package_info, target_package_infos)
-            if target_package_info:
+            target_package_info = FindTargetPackageInfo(curent_package_info, target_package_infos)
+            if target_package_info and curent_package_info != target_package_info:
                 lines[idx] = UpdatePackageInfoLine(line,curent_package_info, target_package_info)
                 is_changed=True
-       
-
     return lines
 
-
 test_target_text='''asio/1.25.0
 hello/2.3.4@world/stable
 good/1.0.1@boy/snapshot
 
 1.修复一些已知问题
 2.优化性能
 '''
@@ -177,9 +171,9 @@
    
 
 
 
 
 if __name__ == "__main__":
     EnvCheck()
-    Main()
+    main()
```

