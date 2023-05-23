# Comparing `tmp/mlbi_at_dku_lib-0.1.0.tar.gz` & `tmp/mlbi_at_dku_lib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlbi_at_dku_lib-0.1.0.tar", last modified: Tue May 23 01:46:41 2023, max compression
+gzip compressed data, was "mlbi_at_dku_lib-0.1.1.tar", last modified: Tue May 23 01:54:36 2023, max compression
```

## Comparing `mlbi_at_dku_lib-0.1.0.tar` & `mlbi_at_dku_lib-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-05-23 01:46:41.314121 mlbi_at_dku_lib-0.1.0/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.0/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       60 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.0/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      732 2023-05-23 01:46:41.314121 mlbi_at_dku_lib-0.1.0/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.0/README.md
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-05-23 01:46:41.314121 mlbi_at_dku_lib-0.1.0/mlbi_at_dku_lib/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.1.0/mlbi_at_dku_lib/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     9379 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.0/mlbi_at_dku_lib/cpdb.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.0/mlbi_at_dku_lib/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    30883 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.0/mlbi_at_dku_lib/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    32541 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.0/mlbi_at_dku_lib/misc.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-05-23 01:46:41.314121 mlbi_at_dku_lib-0.1.0/mlbi_at_dku_lib.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      732 2023-05-23 01:46:40.000000 mlbi_at_dku_lib-0.1.0/mlbi_at_dku_lib.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      422 2023-05-23 01:46:41.000000 mlbi_at_dku_lib-0.1.0/mlbi_at_dku_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-05-23 01:46:40.000000 mlbi_at_dku_lib-0.1.0/mlbi_at_dku_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-05-23 01:46:40.000000 mlbi_at_dku_lib-0.1.0/mlbi_at_dku_lib.egg-info/not-zip-safe
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       64 2023-05-23 01:46:40.000000 mlbi_at_dku_lib-0.1.0/mlbi_at_dku_lib.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       22 2023-05-23 01:46:40.000000 mlbi_at_dku_lib-0.1.0/mlbi_at_dku_lib.egg-info/top_level.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       79 2023-05-23 01:46:41.314121 mlbi_at_dku_lib-0.1.0/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     2774 2023-05-23 01:46:36.000000 mlbi_at_dku_lib-0.1.0/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-05-23 01:46:41.314121 mlbi_at_dku_lib-0.1.0/tests/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      124 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.1.0/tests/__init__.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-05-23 01:54:36.913584 mlbi_at_dku_lib-0.1.1/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.1/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       60 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.1/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      732 2023-05-23 01:54:36.913584 mlbi_at_dku_lib-0.1.1/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.1/README.md
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-05-23 01:54:36.913584 mlbi_at_dku_lib-0.1.1/mlbi_at_dku_lib/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.1.1/mlbi_at_dku_lib/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     9379 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.1/mlbi_at_dku_lib/cpdb.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.1/mlbi_at_dku_lib/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    30883 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.1/mlbi_at_dku_lib/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    32541 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.1/mlbi_at_dku_lib/misc.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-05-23 01:54:36.913584 mlbi_at_dku_lib-0.1.1/mlbi_at_dku_lib.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      732 2023-05-23 01:54:36.000000 mlbi_at_dku_lib-0.1.1/mlbi_at_dku_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      422 2023-05-23 01:54:36.000000 mlbi_at_dku_lib-0.1.1/mlbi_at_dku_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-05-23 01:54:36.000000 mlbi_at_dku_lib-0.1.1/mlbi_at_dku_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-05-23 01:46:40.000000 mlbi_at_dku_lib-0.1.1/mlbi_at_dku_lib.egg-info/not-zip-safe
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       27 2023-05-23 01:54:36.000000 mlbi_at_dku_lib-0.1.1/mlbi_at_dku_lib.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       22 2023-05-23 01:54:36.000000 mlbi_at_dku_lib-0.1.1/mlbi_at_dku_lib.egg-info/top_level.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       79 2023-05-23 01:54:36.913584 mlbi_at_dku_lib-0.1.1/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     2725 2023-05-23 01:49:57.000000 mlbi_at_dku_lib-0.1.1/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-05-23 01:54:36.913584 mlbi_at_dku_lib-0.1.1/tests/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      124 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.1.1/tests/__init__.py
```

### Comparing `mlbi_at_dku_lib-0.1.0/LICENSE` & `mlbi_at_dku_lib-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.0/PKG-INFO` & `mlbi_at_dku_lib-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlbi_at_dku_lib
-Version: 0.1.0
+Version: 0.1.1
 Summary: Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Home-page: https://github.com/combio-dku
 Download-URL: https://github.com/combio-dku
 Author: Seokhyun Yoon
 Author-email: syoon@dku.edu
 Keywords: pypi mlbi_at_dku_lib
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mlbi_at_dku_lib-0.1.0/mlbi_at_dku_lib/cpdb.py` & `mlbi_at_dku_lib-0.1.1/mlbi_at_dku_lib/cpdb.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.0/mlbi_at_dku_lib/gsea.py` & `mlbi_at_dku_lib-0.1.1/mlbi_at_dku_lib/gsea.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.0/mlbi_at_dku_lib/icnv.py` & `mlbi_at_dku_lib-0.1.1/mlbi_at_dku_lib/icnv.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.0/mlbi_at_dku_lib/misc.py` & `mlbi_at_dku_lib-0.1.1/mlbi_at_dku_lib/misc.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.0/mlbi_at_dku_lib.egg-info/PKG-INFO` & `mlbi_at_dku_lib-0.1.1/mlbi_at_dku_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlbi-at-dku-lib
-Version: 0.1.0
+Version: 0.1.1
 Summary: Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Home-page: https://github.com/combio-dku
 Download-URL: https://github.com/combio-dku
 Author: Seokhyun Yoon
 Author-email: syoon@dku.edu
 Keywords: pypi mlbi_at_dku_lib
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mlbi_at_dku_lib-0.1.0/setup.py` & `mlbi_at_dku_lib-0.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 
 setup(
     # 배포할 패키지의 이름을 적어줍니다. setup.py파일을 가지는 폴더 이름과 동일하게 합니다.
     name                = 'mlbi_at_dku_lib',
     # 배포할 패키지의 버전을 적어줍니다. 첫 등록이므로 0.1 또는 0.0.1을 사용합니다.
-    version             = '0.1.0',
+    version             = '0.1.1',
     # 배포할 패키지에 대한 설명을 작성합니다.
     description         = 'Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)',
     # 배포하는 사람의 이름을 작성합니다.
     author              = 'Seokhyun Yoon',
     # 배포하는 사람의 메일주소를 작성합니다.
     author_email        = 'syoon@dku.edu',
     # 배포하는 패키지의 url을 적어줍니다. 보통 github 링크를 적습니다.
     url                 = 'https://github.com/combio-dku',
     # 배포하는 패키지의 다운로드 url을 적어줍니다.
     download_url        = 'https://github.com/combio-dku',
     # 해당 패키지를 사용하기 위해 필요한 패키지를 적어줍니다. ex. install_requires= ['numpy', 'django']
     # 여기에 적어준 패키지는 현재 패키지를 install할때 함께 install됩니다.
-    install_requires    =  ['numpy', 'scipy', 'pandas', 'sklearn', 'cellphonedb', 'gseapy', 'infercnvpy', 'plotly'],
+    install_requires    =  ['numpy', 'scipy', 'pandas', 'sklearn'],
     # 등록하고자 하는 패키지를 적는 곳입니다.
     # 우리는 find_packages 라이브러리를 이용하기 때문에 아래와 같이 적어줍니다.
     # 만약 제외하고자 하는 파일이 있다면 exclude에 적어줍니다.
     packages            = find_packages(exclude = []),
     # 패키지의 키워드를 적습니다.
     keywords            = ['pypi mlbi_at_dku_lib'],
     # 해당 패키지를 사용하기 위해 필요한 파이썬 버전을 적습니다.
```

