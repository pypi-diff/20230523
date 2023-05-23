# Comparing `tmp/dcovlib-1.1.1.tar.gz` & `tmp/dcovlib-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcovlib-1.1.1.tar", last modified: Tue May 23 03:38:27 2023, max compression
+gzip compressed data, was "dcovlib-1.1.2.tar", last modified: Tue May 23 07:32:51 2023, max compression
```

## Comparing `dcovlib-1.1.1.tar` & `dcovlib-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 03:38:27.941252 dcovlib-1.1.1/
--rw-rw-rw-   0        0        0      424 2023-05-23 03:38:27.902863 dcovlib-1.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-23 03:38:27.390379 dcovlib-1.1.1/dcovlib/
--rw-rw-rw-   0        0        0       57 2023-05-19 14:25:57.000000 dcovlib-1.1.1/dcovlib/__init__.py
--rw-rw-rw-   0        0        0     3809 2023-05-23 03:36:37.000000 dcovlib-1.1.1/dcovlib/ird.py
-drwxrwxrwx   0        0        0        0 2023-05-23 03:38:27.818692 dcovlib-1.1.1/dcovlib.egg-info/
--rw-rw-rw-   0        0        0      424 2023-05-23 03:38:26.000000 dcovlib-1.1.1/dcovlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-05-23 03:38:27.000000 dcovlib-1.1.1/dcovlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 03:38:26.000000 dcovlib-1.1.1/dcovlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-23 03:38:26.000000 dcovlib-1.1.1/dcovlib.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-05-23 03:38:27.000000 dcovlib-1.1.1/dcovlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-23 03:38:27.000000 dcovlib-1.1.1/dcovlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-19 13:29:02.000000 dcovlib-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-23 03:38:27.942277 dcovlib-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      648 2023-05-23 03:28:03.000000 dcovlib-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 07:32:51.831799 dcovlib-1.1.2/
+-rw-rw-rw-   0        0        0      424 2023-05-23 07:32:51.782785 dcovlib-1.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-23 07:32:51.298730 dcovlib-1.1.2/dcovlib/
+-rw-rw-rw-   0        0        0       57 2023-05-19 14:25:57.000000 dcovlib-1.1.2/dcovlib/__init__.py
+-rw-rw-rw-   0        0        0     3818 2023-05-23 07:32:03.000000 dcovlib-1.1.2/dcovlib/ird.py
+drwxrwxrwx   0        0        0        0 2023-05-23 07:32:51.709874 dcovlib-1.1.2/dcovlib.egg-info/
+-rw-rw-rw-   0        0        0      424 2023-05-23 07:32:50.000000 dcovlib-1.1.2/dcovlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-05-23 07:32:51.000000 dcovlib-1.1.2/dcovlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 07:32:50.000000 dcovlib-1.1.2/dcovlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-23 07:32:50.000000 dcovlib-1.1.2/dcovlib.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-05-23 07:32:50.000000 dcovlib-1.1.2/dcovlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-23 07:32:50.000000 dcovlib-1.1.2/dcovlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-19 13:29:02.000000 dcovlib-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-23 07:32:51.831799 dcovlib-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      648 2023-05-23 07:32:23.000000 dcovlib-1.1.2/setup.py
```

### Comparing `dcovlib-1.1.1/dcovlib/ird.py` & `dcovlib-1.1.2/dcovlib/ird.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,28 +47,29 @@
             print("You should set data first") 
             return ''
         if path.split('.')[-1] != 'ird':
             raise Exception("data type should be ird") 
         fi=open(path,'wb')
         fi.write(self.encode())
         fi.close()
+        
     def savecsv(self,path):
         if self._data is None:
             print("You should set data first") 
             return ''
         if path.split('.')[-1] != 'csv':
             raise Exception("data type should be csv") 
         if len(self._data.shape)>2:
             raise Exception('data shape should not exceed 2')
         savedata = self._data.tolist()
         if len(self._data.shape)==1:
             txt = ','.join([str(c) for c in savedata])
         if len(self._data.shape)==2:
             txt = '\n'.join([','.join([str(c) for c in b]) for b in savedata])
-        fi=open(path,'wb')
+        fi=open(path,'w')
         fi.write(txt)
         fi.close()
         
     def savedata(self,data,path):
         #将np.array保存成ird文件
         self.setdata(data)
         self.savefile(path)
```

### Comparing `dcovlib-1.1.1/setup.py` & `dcovlib-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 REQUIRES = ["numpy"]
 
 setup(
     name='dcovlib',
-    version='1.1.1',
+    version='1.1.2',
     python_requires='>=3.6',
     description='convert numpy to ird file, or convert ird to numpy',
     platforms='Independant',
     author='Sun ling', # 作者
     author_email="ling.sun-01@qq.com",
     url="https://github.com/SheepBreedingLab-HZAU/dcovlib",
     zip_safe=False,
```

