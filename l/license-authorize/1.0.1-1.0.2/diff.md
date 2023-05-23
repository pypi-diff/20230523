# Comparing `tmp/license_authorize-1.0.1.tar.gz` & `tmp/license_authorize-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\license_authorize-1.0.1.tar", last modified: Fri May 19 11:19:01 2023, max compression
+gzip compressed data, was "dist\license_authorize-1.0.2.tar", last modified: Tue May 23 09:51:19 2023, max compression
```

## Comparing `license_authorize-1.0.1.tar` & `license_authorize-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 11:19:01.665431 license_authorize-1.0.1/
--rw-rw-rw-   0        0        0     1394 2023-05-19 11:19:01.663432 license_authorize-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      389 2023-05-19 09:47:18.000000 license_authorize-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 11:19:01.656432 license_authorize-1.0.1/license_authorize/
--rw-rw-rw-   0        0        0      226 2023-05-19 06:53:07.000000 license_authorize-1.0.1/license_authorize/__init__.py
--rw-rw-rw-   0        0        0     3103 2023-05-19 10:27:37.000000 license_authorize-1.0.1/license_authorize/_core.py
--rw-rw-rw-   0        0        0      877 2023-05-19 10:12:48.000000 license_authorize-1.0.1/license_authorize/decode.py
-drwxrwxrwx   0        0        0        0 2023-05-19 11:19:01.662432 license_authorize-1.0.1/license_authorize.egg-info/
--rw-rw-rw-   0        0        0     1394 2023-05-19 11:19:01.000000 license_authorize-1.0.1/license_authorize.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-05-19 11:19:01.000000 license_authorize-1.0.1/license_authorize.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 11:19:01.000000 license_authorize-1.0.1/license_authorize.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-19 11:19:01.000000 license_authorize-1.0.1/license_authorize.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-19 11:19:01.000000 license_authorize-1.0.1/license_authorize.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 11:19:01.665431 license_authorize-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2175 2023-05-19 11:18:58.000000 license_authorize-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:51:19.355155 license_authorize-1.0.2/
+-rw-rw-rw-   0        0        0     1405 2023-05-23 09:51:19.355155 license_authorize-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      389 2023-05-19 09:47:18.000000 license_authorize-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 09:51:19.345156 license_authorize-1.0.2/license_authorize/
+-rw-rw-rw-   0        0        0      202 2023-05-23 09:22:29.000000 license_authorize-1.0.2/license_authorize/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:51:19.353156 license_authorize-1.0.2/license_authorize.egg-info/
+-rw-rw-rw-   0        0        0     1405 2023-05-23 09:51:19.000000 license_authorize-1.0.2/license_authorize.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-05-23 09:51:19.000000 license_authorize-1.0.2/license_authorize.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 09:51:19.000000 license_authorize-1.0.2/license_authorize.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-23 09:51:19.000000 license_authorize-1.0.2/license_authorize.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-23 09:51:19.000000 license_authorize-1.0.2/license_authorize.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 09:51:19.356155 license_authorize-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2236 2023-05-23 09:24:13.000000 license_authorize-1.0.2/setup.py
```

### Comparing `license_authorize-1.0.1/PKG-INFO` & `license_authorize-1.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: license_authorize
-Version: 1.0.1
-Summary: A tools for license authorize
+Version: 1.0.2
+Summary: A tools for license authorize in windows
 Home-page: https://github.com/gisfanmachel/licenseAuthorize
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Description: ## this program is for lincense authorize
         
         ### it use cpuid and servertime and clienttime to verify the request with the premaked lic file
```

### Comparing `license_authorize-1.0.1/license_authorize.egg-info/PKG-INFO` & `license_authorize-1.0.2/license_authorize.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: license-authorize
-Version: 1.0.1
-Summary: A tools for license authorize
+Version: 1.0.2
+Summary: A tools for license authorize in windows
 Home-page: https://github.com/gisfanmachel/licenseAuthorize
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Description: ## this program is for lincense authorize
         
         ### it use cpuid and servertime and clienttime to verify the request with the premaked lic file
```

### Comparing `license_authorize-1.0.1/setup.py` & `license_authorize-1.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,17 +18,18 @@
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
 
+    # name="license_authorize",  # Required 项目名称
     name="license_authorize",  # Required 项目名称
-    version="1.0.1",  # Required 发布版本号
-    description="A tools for license authorize",  # Optional 项目简单描述
+    version="1.0.2",  # Required 发布版本号
+    description="A tools for license authorize in windows",  # Optional 项目简单描述
     long_description=long_description,  # Optional 详细描述
     long_description_content_type="text/markdown",  # 内容类型
     url="https://github.com/gisfanmachel/licenseAuthorize",  # Optional github项目地址
     author="gisfanmachel",  # Optional 作者
     author_email="gisfanmachel@gmail.com",  # Optional 作者邮箱
     classifiers=[  # Optional 分类器通过对项目进行分类来帮助用户找到项目, 以下除了python版本其他的 不需要改动
 
@@ -44,18 +45,14 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3 :: Only",
     ],
 
     keywords="license,authorize, setuptools, development",  # Optional 搜索关键字
 
-
     packages=find_packages(),  # Required
 
     python_requires=">=3.7, <4",  # python 版本要求
 
     install_requires=["pycryptodome"],  # Optional 第三方依赖库
 
-
-
-
 )
```

