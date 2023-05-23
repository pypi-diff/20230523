# Comparing `tmp/Econ_linux-7.0.tar.gz` & `tmp/Econ_linux-8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Econ_linux-7.0.tar", last modified: Fri May 19 07:33:03 2023, max compression
+gzip compressed data, was "dist/Econ_linux-8.0.tar", last modified: Fri May 19 07:36:04 2023, max compression
```

## Comparing `Econ_linux-7.0.tar` & `Econ_linux-8.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 sulthan   (1001) sulthan   (1001)        0 2023-05-19 07:33:03.000000 Econ_linux-7.0/
-drwxrwxr-x   0 sulthan   (1001) sulthan   (1001)        0 2023-05-19 07:33:03.000000 Econ_linux-7.0/Econ_linux.egg-info/
--rw-rw-r--   0 sulthan   (1001) sulthan   (1001)        1 2023-05-19 07:33:03.000000 Econ_linux-7.0/Econ_linux.egg-info/dependency_links.txt
--rw-rw-r--   0 sulthan   (1001) sulthan   (1001)      225 2023-05-19 07:33:03.000000 Econ_linux-7.0/Econ_linux.egg-info/PKG-INFO
--rw-rw-r--   0 sulthan   (1001) sulthan   (1001)        1 2023-05-19 07:33:03.000000 Econ_linux-7.0/Econ_linux.egg-info/not-zip-safe
--rw-rw-r--   0 sulthan   (1001) sulthan   (1001)       11 2023-05-19 07:33:03.000000 Econ_linux-7.0/Econ_linux.egg-info/top_level.txt
--rw-rw-r--   0 sulthan   (1001) sulthan   (1001)      192 2023-05-19 07:33:03.000000 Econ_linux-7.0/Econ_linux.egg-info/SOURCES.txt
--rw-rw-r--   0 sulthan   (1001) sulthan   (1001)       38 2023-05-19 07:33:03.000000 Econ_linux-7.0/setup.cfg
--rw-rw-r--   0 sulthan   (1001) sulthan   (1001)    11917 2023-05-19 07:32:47.000000 Econ_linux-7.0/Econ_linux.cpp
--rw-rw-r--   0 sulthan   (1001) sulthan   (1001)      225 2023-05-19 07:33:03.000000 Econ_linux-7.0/PKG-INFO
--rw-rw-r--   0 sulthan   (1001) sulthan   (1001)     1628 2023-05-19 07:31:35.000000 Econ_linux-7.0/setup.py
+drwxrwxr-x   0 sulthan   (1001) sulthan   (1001)        0 2023-05-19 07:36:04.000000 Econ_linux-8.0/
+drwxrwxr-x   0 sulthan   (1001) sulthan   (1001)        0 2023-05-19 07:36:04.000000 Econ_linux-8.0/Econ_linux.egg-info/
+-rw-rw-r--   0 sulthan   (1001) sulthan   (1001)        1 2023-05-19 07:36:04.000000 Econ_linux-8.0/Econ_linux.egg-info/dependency_links.txt
+-rw-rw-r--   0 sulthan   (1001) sulthan   (1001)      225 2023-05-19 07:36:04.000000 Econ_linux-8.0/Econ_linux.egg-info/PKG-INFO
+-rw-rw-r--   0 sulthan   (1001) sulthan   (1001)        1 2023-05-19 07:36:04.000000 Econ_linux-8.0/Econ_linux.egg-info/not-zip-safe
+-rw-rw-r--   0 sulthan   (1001) sulthan   (1001)       11 2023-05-19 07:36:04.000000 Econ_linux-8.0/Econ_linux.egg-info/top_level.txt
+-rw-rw-r--   0 sulthan   (1001) sulthan   (1001)      192 2023-05-19 07:36:04.000000 Econ_linux-8.0/Econ_linux.egg-info/SOURCES.txt
+-rw-rw-r--   0 sulthan   (1001) sulthan   (1001)       38 2023-05-19 07:36:04.000000 Econ_linux-8.0/setup.cfg
+-rw-rw-r--   0 sulthan   (1001) sulthan   (1001)    11917 2023-05-19 07:32:47.000000 Econ_linux-8.0/Econ_linux.cpp
+-rw-rw-r--   0 sulthan   (1001) sulthan   (1001)      225 2023-05-19 07:36:04.000000 Econ_linux-8.0/PKG-INFO
+-rw-rw-r--   0 sulthan   (1001) sulthan   (1001)     1628 2023-05-19 07:35:46.000000 Econ_linux-8.0/setup.py
```

### Comparing `Econ_linux-7.0/Econ_linux.cpp` & `Econ_linux-8.0/Econ_linux.cpp`

 * *Files identical despite different names*

### Comparing `Econ_linux-7.0/setup.py` & `Econ_linux-8.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         for ext in self.extensions:
             ext.extra_compile_args = extra_compile_args
         build_ext.build_extensions(self)
 
 # Setup configuration
 setup(
     name='Econ_linux',
-    version='7.0',
+    version='8.0',
     description='Enumerator Linux Extension Module',
     author='Your Name',
     author_email='your_email@example.com',
     ext_modules=[ext_module],
     cmdclass={'build_ext': BuildExt},
     zip_safe=False
 )
```

