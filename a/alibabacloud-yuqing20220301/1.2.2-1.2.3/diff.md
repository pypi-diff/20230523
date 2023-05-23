# Comparing `tmp/alibabacloud_yuqing20220301-1.2.2.tar.gz` & `tmp/alibabacloud_yuqing20220301-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_yuqing20220301-1.2.2.tar", last modified: Mon May 22 02:31:18 2023, max compression
+gzip compressed data, was "dist/alibabacloud_yuqing20220301-1.2.3.tar", last modified: Tue May 23 02:07:25 2023, max compression
```

## Comparing `alibabacloud_yuqing20220301-1.2.2.tar` & `alibabacloud_yuqing20220301-1.2.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 02:31:18.000000 alibabacloud_yuqing20220301-1.2.2/
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-22 02:31:17.000000 alibabacloud_yuqing20220301-1.2.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-22 02:31:17.000000 alibabacloud_yuqing20220301-1.2.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2346 2023-05-22 02:31:18.000000 alibabacloud_yuqing20220301-1.2.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1031 2023-05-22 02:31:17.000000 alibabacloud_yuqing20220301-1.2.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2023-05-22 02:31:17.000000 alibabacloud_yuqing20220301-1.2.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 02:31:18.000000 alibabacloud_yuqing20220301-1.2.2/alibabacloud_yuqing20220301/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-22 02:31:17.000000 alibabacloud_yuqing20220301-1.2.2/alibabacloud_yuqing20220301/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29628 2023-05-22 02:31:17.000000 alibabacloud_yuqing20220301-1.2.2/alibabacloud_yuqing20220301/client.py
--rw-r--r--   0 root         (0) root         (0)    81156 2023-05-22 02:31:17.000000 alibabacloud_yuqing20220301-1.2.2/alibabacloud_yuqing20220301/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 02:31:18.000000 alibabacloud_yuqing20220301-1.2.2/alibabacloud_yuqing20220301.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2346 2023-05-22 02:31:18.000000 alibabacloud_yuqing20220301-1.2.2/alibabacloud_yuqing20220301.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      431 2023-05-22 02:31:18.000000 alibabacloud_yuqing20220301-1.2.2/alibabacloud_yuqing20220301.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 02:31:18.000000 alibabacloud_yuqing20220301-1.2.2/alibabacloud_yuqing20220301.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-05-22 02:31:18.000000 alibabacloud_yuqing20220301-1.2.2/alibabacloud_yuqing20220301.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2023-05-22 02:31:18.000000 alibabacloud_yuqing20220301-1.2.2/alibabacloud_yuqing20220301.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-22 02:31:18.000000 alibabacloud_yuqing20220301-1.2.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2625 2023-05-22 02:31:17.000000 alibabacloud_yuqing20220301-1.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:07:25.000000 alibabacloud_yuqing20220301-1.2.3/
+-rw-r--r--   0 root         (0) root         (0)       52 2023-05-23 02:07:24.000000 alibabacloud_yuqing20220301-1.2.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-23 02:07:24.000000 alibabacloud_yuqing20220301-1.2.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-23 02:07:24.000000 alibabacloud_yuqing20220301-1.2.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2346 2023-05-23 02:07:25.000000 alibabacloud_yuqing20220301-1.2.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-05-23 02:07:24.000000 alibabacloud_yuqing20220301-1.2.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-05-23 02:07:24.000000 alibabacloud_yuqing20220301-1.2.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:07:25.000000 alibabacloud_yuqing20220301-1.2.3/alibabacloud_yuqing20220301/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-23 02:07:24.000000 alibabacloud_yuqing20220301-1.2.3/alibabacloud_yuqing20220301/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29628 2023-05-23 02:07:24.000000 alibabacloud_yuqing20220301-1.2.3/alibabacloud_yuqing20220301/client.py
+-rw-r--r--   0 root         (0) root         (0)    81384 2023-05-23 02:07:24.000000 alibabacloud_yuqing20220301-1.2.3/alibabacloud_yuqing20220301/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:07:25.000000 alibabacloud_yuqing20220301-1.2.3/alibabacloud_yuqing20220301.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2346 2023-05-23 02:07:24.000000 alibabacloud_yuqing20220301-1.2.3/alibabacloud_yuqing20220301.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      444 2023-05-23 02:07:25.000000 alibabacloud_yuqing20220301-1.2.3/alibabacloud_yuqing20220301.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 02:07:24.000000 alibabacloud_yuqing20220301-1.2.3/alibabacloud_yuqing20220301.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-05-23 02:07:24.000000 alibabacloud_yuqing20220301-1.2.3/alibabacloud_yuqing20220301.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-05-23 02:07:24.000000 alibabacloud_yuqing20220301-1.2.3/alibabacloud_yuqing20220301.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-23 02:07:25.000000 alibabacloud_yuqing20220301-1.2.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2625 2023-05-23 02:07:24.000000 alibabacloud_yuqing20220301-1.2.3/setup.py
```

### Comparing `alibabacloud_yuqing20220301-1.2.2/LICENSE` & `alibabacloud_yuqing20220301-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_yuqing20220301-1.2.2/PKG-INFO` & `alibabacloud_yuqing20220301-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_yuqing20220301
-Version: 1.2.2
+Version: 1.2.3
 Summary: Alibaba Cloud Yuqing (20220301) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_yuqing20220301-1.2.2/README-CN.md` & `alibabacloud_yuqing20220301-1.2.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_yuqing20220301-1.2.2/README.md` & `alibabacloud_yuqing20220301-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_yuqing20220301-1.2.2/alibabacloud_yuqing20220301/client.py` & `alibabacloud_yuqing20220301-1.2.3/alibabacloud_yuqing20220301/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_yuqing20220301-1.2.2/alibabacloud_yuqing20220301/models.py` & `alibabacloud_yuqing20220301-1.2.3/alibabacloud_yuqing20220301/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -756,15 +756,15 @@
         doc_self_content_sign: str = None,
         doc_title: str = None,
         doc_url: str = None,
         emotion_score: float = None,
         emotion_type: int = None,
         ext_info: Dict[str, str] = None,
         fin_event_count: int = None,
-        finance_event_list: YuqingFinanceEvent = None,
+        finance_event_list: List[YuqingFinanceEvent] = None,
         highlight_keywords: List[str] = None,
         image_count: int = None,
         influence_score: float = None,
         media_hosts: List[str] = None,
         media_influence_level: int = None,
         media_name: str = None,
         media_propagation_level: int = None,
@@ -848,15 +848,17 @@
         self.topics = topics
         self.video_count = video_count
         self.weibo_comment_id = weibo_comment_id
         self.weibo_mid = weibo_mid
 
     def validate(self):
         if self.finance_event_list:
-            self.finance_event_list.validate()
+            for k in self.finance_event_list:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -948,16 +950,18 @@
             result['emotionScore'] = self.emotion_score
         if self.emotion_type is not None:
             result['emotionType'] = self.emotion_type
         if self.ext_info is not None:
             result['extInfo'] = self.ext_info
         if self.fin_event_count is not None:
             result['finEventCount'] = self.fin_event_count
+        result['financeEventList'] = []
         if self.finance_event_list is not None:
-            result['financeEventList'] = self.finance_event_list.to_map()
+            for k in self.finance_event_list:
+                result['financeEventList'].append(k.to_map() if k else None)
         if self.highlight_keywords is not None:
             result['highlightKeywords'] = self.highlight_keywords
         if self.image_count is not None:
             result['imageCount'] = self.image_count
         if self.influence_score is not None:
             result['influenceScore'] = self.influence_score
         if self.media_hosts is not None:
@@ -1086,17 +1090,19 @@
             self.emotion_score = m.get('emotionScore')
         if m.get('emotionType') is not None:
             self.emotion_type = m.get('emotionType')
         if m.get('extInfo') is not None:
             self.ext_info = m.get('extInfo')
         if m.get('finEventCount') is not None:
             self.fin_event_count = m.get('finEventCount')
+        self.finance_event_list = []
         if m.get('financeEventList') is not None:
-            temp_model = YuqingFinanceEvent()
-            self.finance_event_list = temp_model.from_map(m['financeEventList'])
+            for k in m.get('financeEventList'):
+                temp_model = YuqingFinanceEvent()
+                self.finance_event_list.append(temp_model.from_map(k))
         if m.get('highlightKeywords') is not None:
             self.highlight_keywords = m.get('highlightKeywords')
         if m.get('imageCount') is not None:
             self.image_count = m.get('imageCount')
         if m.get('influenceScore') is not None:
             self.influence_score = m.get('influenceScore')
         if m.get('mediaHosts') is not None:
```

### Comparing `alibabacloud_yuqing20220301-1.2.2/alibabacloud_yuqing20220301.egg-info/PKG-INFO` & `alibabacloud_yuqing20220301-1.2.3/alibabacloud_yuqing20220301.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-yuqing20220301
-Version: 1.2.2
+Version: 1.2.3
 Summary: Alibaba Cloud Yuqing (20220301) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_yuqing20220301-1.2.2/setup.py` & `alibabacloud_yuqing20220301-1.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_yuqing20220301.
 
-Created on 22/05/2023
+Created on 23/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_yuqing20220301"
 NAME = "alibabacloud_yuqing20220301" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Yuqing (20220301) SDK Library for Python"
```

