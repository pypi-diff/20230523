# Comparing `tmp/dcovlib-1.0.1.tar.gz` & `tmp/dcovlib-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcovlib-1.0.1.tar", last modified: Fri May 19 14:28:47 2023, max compression
+gzip compressed data, was "dcovlib-1.1.1.tar", last modified: Tue May 23 03:38:27 2023, max compression
```

## Comparing `dcovlib-1.0.1.tar` & `dcovlib-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 14:28:47.058950 dcovlib-1.0.1/
--rw-rw-rw-   0        0        0      424 2023-05-19 14:28:47.020244 dcovlib-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-19 14:28:46.492264 dcovlib-1.0.1/dcovlib/
--rw-rw-rw-   0        0        0       57 2023-05-19 14:25:57.000000 dcovlib-1.0.1/dcovlib/__init__.py
--rw-rw-rw-   0        0        0     2896 2023-05-18 02:59:29.000000 dcovlib-1.0.1/dcovlib/ird.py
-drwxrwxrwx   0        0        0        0 2023-05-19 14:28:46.936802 dcovlib-1.0.1/dcovlib.egg-info/
--rw-rw-rw-   0        0        0      424 2023-05-19 14:28:45.000000 dcovlib-1.0.1/dcovlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-05-19 14:28:46.000000 dcovlib-1.0.1/dcovlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 14:28:46.000000 dcovlib-1.0.1/dcovlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-19 14:28:45.000000 dcovlib-1.0.1/dcovlib.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-05-19 14:28:46.000000 dcovlib-1.0.1/dcovlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-19 14:28:46.000000 dcovlib-1.0.1/dcovlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-19 13:29:02.000000 dcovlib-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-19 14:28:47.058950 dcovlib-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      648 2023-05-19 14:27:57.000000 dcovlib-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 03:38:27.941252 dcovlib-1.1.1/
+-rw-rw-rw-   0        0        0      424 2023-05-23 03:38:27.902863 dcovlib-1.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-23 03:38:27.390379 dcovlib-1.1.1/dcovlib/
+-rw-rw-rw-   0        0        0       57 2023-05-19 14:25:57.000000 dcovlib-1.1.1/dcovlib/__init__.py
+-rw-rw-rw-   0        0        0     3809 2023-05-23 03:36:37.000000 dcovlib-1.1.1/dcovlib/ird.py
+drwxrwxrwx   0        0        0        0 2023-05-23 03:38:27.818692 dcovlib-1.1.1/dcovlib.egg-info/
+-rw-rw-rw-   0        0        0      424 2023-05-23 03:38:26.000000 dcovlib-1.1.1/dcovlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-05-23 03:38:27.000000 dcovlib-1.1.1/dcovlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 03:38:26.000000 dcovlib-1.1.1/dcovlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-23 03:38:26.000000 dcovlib-1.1.1/dcovlib.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-05-23 03:38:27.000000 dcovlib-1.1.1/dcovlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-23 03:38:27.000000 dcovlib-1.1.1/dcovlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-19 13:29:02.000000 dcovlib-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-23 03:38:27.942277 dcovlib-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      648 2023-05-23 03:28:03.000000 dcovlib-1.1.1/setup.py
```

### Comparing `dcovlib-1.0.1/dcovlib/ird.py` & `dcovlib-1.1.1/dcovlib/ird.py`

 * *Files 27% similar despite different names*

```diff
@@ -42,22 +42,46 @@
         return b'ird' + shapebyte + self._datatype + bytedata
     
     def savefile(self,path):
         #手动保存文件
         if self._data is None:
             print("You should set data first") 
             return ''
+        if path.split('.')[-1] != 'ird':
+            raise Exception("data type should be ird") 
         fi=open(path,'wb')
         fi.write(self.encode())
         fi.close()
-  
+    def savecsv(self,path):
+        if self._data is None:
+            print("You should set data first") 
+            return ''
+        if path.split('.')[-1] != 'csv':
+            raise Exception("data type should be csv") 
+        if len(self._data.shape)>2:
+            raise Exception('data shape should not exceed 2')
+        savedata = self._data.tolist()
+        if len(self._data.shape)==1:
+            txt = ','.join([str(c) for c in savedata])
+        if len(self._data.shape)==2:
+            txt = '\n'.join([','.join([str(c) for c in b]) for b in savedata])
+        fi=open(path,'wb')
+        fi.write(txt)
+        fi.close()
+        
     def savedata(self,data,path):
         #将np.array保存成ird文件
         self.setdata(data)
         self.savefile(path)
+       
+        
+    def savecsvdata(self,data,path):
+        #将np.array保存成ird文件
+        self.setdata(data)
+        self.savecsv(path)
         
     def _decodeshape(self):
         shape=[a for a in self._shape if a !=0]
         return shape
```

### Comparing `dcovlib-1.0.1/setup.py` & `dcovlib-1.1.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 REQUIRES = ["numpy"]
 
 setup(
     name='dcovlib',
-    version='1.0.1',
+    version='1.1.1',
     python_requires='>=3.6',
     description='convert numpy to ird file, or convert ird to numpy',
     platforms='Independant',
     author='Sun ling', # 作者
     author_email="ling.sun-01@qq.com",
     url="https://github.com/SheepBreedingLab-HZAU/dcovlib",
     zip_safe=False,
```

