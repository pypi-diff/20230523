# Comparing `tmp/aliyun-python-sdk-computenestsupplier-1.0.4.tar.gz` & `tmp/aliyun-python-sdk-computenestsupplier-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-computenestsupplier-1.0.4.tar", last modified: Tue May 16 10:07:10 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-computenestsupplier-1.0.5.tar", last modified: Tue May 23 05:32:19 2023, max compression
```

## Comparing `aliyun-python-sdk-computenestsupplier-1.0.4.tar` & `aliyun-python-sdk-computenestsupplier-1.0.5.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:07:10.000000 aliyun-python-sdk-computenestsupplier-1.0.4/
--rw-r--r--   0 root         (0) root         (0)      575 2023-05-16 10:07:09.000000 aliyun-python-sdk-computenestsupplier-1.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-16 10:07:09.000000 aliyun-python-sdk-computenestsupplier-1.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1617 2023-05-16 10:07:10.000000 aliyun-python-sdk-computenestsupplier-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      559 2023-05-16 10:07:09.000000 aliyun-python-sdk-computenestsupplier-1.0.4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:07:10.000000 aliyun-python-sdk-computenestsupplier-1.0.4/aliyun_python_sdk_computenestsupplier.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1617 2023-05-16 10:07:09.000000 aliyun-python-sdk-computenestsupplier-1.0.4/aliyun_python_sdk_computenestsupplier.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1800 2023-05-16 10:07:09.000000 aliyun-python-sdk-computenestsupplier-1.0.4/aliyun_python_sdk_computenestsupplier.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 10:07:09.000000 aliyun-python-sdk-computenestsupplier-1.0.4/aliyun_python_sdk_computenestsupplier.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-05-16 10:07:09.000000 aliyun-python-sdk-computenestsupplier-1.0.4/aliyun_python_sdk_computenestsupplier.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-16 10:07:09.000000 aliyun-python-sdk-computenestsupplier-1.0.4/aliyun_python_sdk_computenestsupplier.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:07:10.000000 aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-16 10:07:09.000000 aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1088 2023-05-16 10:07:09.000000 aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:07:10.000000 aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 10:07:09.000000 aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:07:10.000000 aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/v20210521/
--rw-r--r--   0 root         (0) root         (0)     2778 2023-05-16 10:07:09.000000 aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/v20210521/CreateArtifactRequest.py
--rw-r--r--   0 root         (0) root         (0)     6253 2023-05-16 10:07:09.000000 aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/v20210521/CreateServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1708 2023-05-16 10:07:09.000000 aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/v20210521/DeleteArtifactRequest.py
--rw-r--r--   0 root         (0) root         (0)     1891 2023-05-16 10:07:09.000000 aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/v20210521/DeleteServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1750 2023-05-16 10:07:09.000000 aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRepositoryCredentialsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1702 2023-05-16 10:07:09.000000 aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRequest.py
--rw-r--r--   0 root         (0) root         (0)     2536 2023-05-16 10:07:09.000000 aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/v20210521/GetServiceEstimateCostRequest.py
--rw-r--r--   0 root         (0) root         (0)     1537 2023-05-16 10:07:09.000000 aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/v20210521/GetServiceInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1688 2023-05-16 10:07:09.000000 aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/v20210521/GetServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1869 2023-05-16 10:07:09.000000 aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/v20210521/ListArtifactVersionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2217 2023-05-16 10:07:09.000000 aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/v20210521/ListArtifactsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2845 2023-05-16 10:07:09.000000 aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/v20210521/ListServiceInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2223 2023-05-16 10:07:09.000000 aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/v20210521/ListServiceUsagesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3050 2023-05-16 10:07:09.000000 aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/v20210521/ListServicesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1489 2023-05-16 10:07:09.000000 aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/v20210521/ReleaseArtifactRequest.py
--rw-r--r--   0 root         (0) root         (0)     2420 2023-05-16 10:07:09.000000 aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/v20210521/UpdateArtifactRequest.py
--rw-r--r--   0 root         (0) root         (0)     5446 2023-05-16 10:07:09.000000 aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/v20210521/UpdateServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 10:07:09.000000 aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/v20210521/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-05-16 10:07:10.000000 aliyun-python-sdk-computenestsupplier-1.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2532 2023-05-16 10:07:09.000000 aliyun-python-sdk-computenestsupplier-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:32:19.000000 aliyun-python-sdk-computenestsupplier-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1617 2023-05-23 05:32:19.000000 aliyun-python-sdk-computenestsupplier-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      559 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:32:19.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyun_python_sdk_computenestsupplier.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1617 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyun_python_sdk_computenestsupplier.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1878 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyun_python_sdk_computenestsupplier.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyun_python_sdk_computenestsupplier.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyun_python_sdk_computenestsupplier.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyun_python_sdk_computenestsupplier.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:32:19.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:32:19.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:32:19.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/
+-rw-r--r--   0 root         (0) root         (0)     2778 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/CreateArtifactRequest.py
+-rw-r--r--   0 root         (0) root         (0)     6253 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/CreateServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1708 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/DeleteArtifactRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1891 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/DeleteServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1750 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRepositoryCredentialsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1905 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2536 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/GetServiceEstimateCostRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/GetServiceInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1688 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/GetServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/GetUploadCredentialsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1869 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/ListArtifactVersionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2217 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/ListArtifactsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2845 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/ListServiceInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2223 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/ListServiceUsagesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3050 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/ListServicesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/ReleaseArtifactRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2420 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/UpdateArtifactRequest.py
+-rw-r--r--   0 root         (0) root         (0)     5446 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/UpdateServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-05-23 05:32:19.000000 aliyun-python-sdk-computenestsupplier-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2532 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/setup.py
```

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.4/LICENSE` & `aliyun-python-sdk-computenestsupplier-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.4/PKG-INFO` & `aliyun-python-sdk-computenestsupplier-1.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-computenestsupplier
-Version: 1.0.4
+Version: 1.0.5
 Summary: The computenestsupplier module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-computenestsupplier
```

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.4/README.rst` & `aliyun-python-sdk-computenestsupplier-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.4/aliyun_python_sdk_computenestsupplier.egg-info/PKG-INFO` & `aliyun-python-sdk-computenestsupplier-1.0.5/aliyun_python_sdk_computenestsupplier.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-computenestsupplier
-Version: 1.0.4
+Version: 1.0.5
 Summary: The computenestsupplier module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-computenestsupplier
```

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.4/aliyun_python_sdk_computenestsupplier.egg-info/SOURCES.txt` & `aliyun-python-sdk-computenestsupplier-1.0.5/aliyun_python_sdk_computenestsupplier.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 aliyunsdkcomputenestsupplier/request/v20210521/DeleteArtifactRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/DeleteServiceRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRepositoryCredentialsRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/GetServiceEstimateCostRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/GetServiceInstanceRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/GetServiceRequest.py
+aliyunsdkcomputenestsupplier/request/v20210521/GetUploadCredentialsRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/ListArtifactVersionsRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/ListArtifactsRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/ListServiceInstancesRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/ListServiceUsagesRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/ListServicesRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/ReleaseArtifactRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/UpdateArtifactRequest.py
```

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/endpoint.py` & `aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/v20210521/CreateArtifactRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/CreateArtifactRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/v20210521/CreateServiceRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/CreateServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/v20210521/DeleteArtifactRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/DeleteArtifactRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/v20210521/DeleteServiceRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/DeleteServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRepositoryCredentialsRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRepositoryCredentialsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,12 +32,17 @@
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ArtifactVersion(self): # String
 		return self.get_query_params().get('ArtifactVersion')
 
 	def set_ArtifactVersion(self, ArtifactVersion):  # String
 		self.add_query_param('ArtifactVersion', ArtifactVersion)
+	def get_ArtifactName(self): # String
+		return self.get_query_params().get('ArtifactName')
+
+	def set_ArtifactName(self, ArtifactName):  # String
+		self.add_query_param('ArtifactName', ArtifactName)
 	def get_ArtifactId(self): # String
 		return self.get_query_params().get('ArtifactId')
 
 	def set_ArtifactId(self, ArtifactId):  # String
 		self.add_query_param('ArtifactId', ArtifactId)
```

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/v20210521/GetServiceEstimateCostRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/GetServiceEstimateCostRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/v20210521/GetServiceInstanceRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/GetServiceInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/v20210521/GetServiceRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/GetServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/v20210521/ListArtifactVersionsRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/ListArtifactVersionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/v20210521/ListArtifactsRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/ListArtifactsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/v20210521/ListServiceInstancesRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/ListServiceInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/v20210521/ListServiceUsagesRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/ListServiceUsagesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/v20210521/ListServicesRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/ListServicesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/v20210521/ReleaseArtifactRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/ReleaseArtifactRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/v20210521/UpdateArtifactRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/UpdateArtifactRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.4/aliyunsdkcomputenestsupplier/request/v20210521/UpdateServiceRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/UpdateServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.4/setup.py` & `aliyun-python-sdk-computenestsupplier-1.0.5/setup.py`

 * *Files identical despite different names*

