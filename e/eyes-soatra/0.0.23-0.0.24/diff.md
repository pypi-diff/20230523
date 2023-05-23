# Comparing `tmp/eyes_soatra-0.0.23.tar.gz` & `tmp/eyes_soatra-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eyes_soatra-0.0.23.tar", last modified: Mon May 15 03:46:02 2023, max compression
+gzip compressed data, was "eyes_soatra-0.0.24.tar", last modified: Tue May 23 06:21:56 2023, max compression
```

## Comparing `eyes_soatra-0.0.23.tar` & `eyes_soatra-0.0.24.tar`

### file list

```diff
@@ -1,25 +1,46 @@
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-15 03:46:02.021640 eyes_soatra-0.0.23/
--rw-r--r--   0 soatra     (501) staff       (20)       13 2023-05-02 07:13:47.000000 eyes_soatra-0.0.23/LICENSE
--rw-r--r--   0 soatra     (501) staff       (20)      554 2023-05-15 03:46:02.021514 eyes_soatra-0.0.23/PKG-INFO
--rw-r--r--   0 soatra     (501) staff       (20)       49 2023-05-11 09:42:34.000000 eyes_soatra-0.0.23/README.md
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-15 03:46:02.016770 eyes_soatra-0.0.23/eyes_soatra/
--rw-r--r--   0 soatra     (501) staff       (20)       28 2023-05-02 07:14:02.000000 eyes_soatra-0.0.23/eyes_soatra/__init__.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-15 03:46:02.018021 eyes_soatra-0.0.23/eyes_soatra/depends/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-02 07:07:54.000000 eyes_soatra-0.0.23/eyes_soatra/depends/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)     7691 2023-05-11 01:49:20.000000 eyes_soatra-0.0.23/eyes_soatra/depends/depends_404.py
--rw-r--r--   0 soatra     (501) staff       (20)      276 2023-05-02 03:37:05.000000 eyes_soatra-0.0.23/eyes_soatra/depends/depends_no_data.py
--rw-r--r--   0 soatra     (501) staff       (20)    13126 2023-05-15 03:20:21.000000 eyes_soatra-0.0.23/eyes_soatra/eyes.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-15 03:46:02.018369 eyes_soatra-0.0.23/eyes_soatra/needs/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-11 07:51:47.000000 eyes_soatra-0.0.23/eyes_soatra/needs/__init__.py
--rw-rw-r--   0 soatra     (501) staff       (20)  1339531 2023-05-11 09:13:03.000000 eyes_soatra-0.0.23/eyes_soatra/needs/user_agents.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-15 03:46:02.017494 eyes_soatra-0.0.23/eyes_soatra.egg-info/
--rw-r--r--   0 soatra     (501) staff       (20)      554 2023-05-15 03:46:01.000000 eyes_soatra-0.0.23/eyes_soatra.egg-info/PKG-INFO
--rw-r--r--   0 soatra     (501) staff       (20)      440 2023-05-15 03:46:01.000000 eyes_soatra-0.0.23/eyes_soatra.egg-info/SOURCES.txt
--rw-r--r--   0 soatra     (501) staff       (20)        1 2023-05-15 03:46:01.000000 eyes_soatra-0.0.23/eyes_soatra.egg-info/dependency_links.txt
--rw-r--r--   0 soatra     (501) staff       (20)       43 2023-05-15 03:46:01.000000 eyes_soatra-0.0.23/eyes_soatra.egg-info/requires.txt
--rw-r--r--   0 soatra     (501) staff       (20)       12 2023-05-15 03:46:01.000000 eyes_soatra-0.0.23/eyes_soatra.egg-info/top_level.txt
--rw-r--r--   0 soatra     (501) staff       (20)       38 2023-05-15 03:46:02.021685 eyes_soatra-0.0.23/setup.cfg
--rw-r--r--   0 soatra     (501) staff       (20)     1131 2023-05-15 03:45:59.000000 eyes_soatra-0.0.23/setup.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-15 03:46:02.021035 eyes_soatra-0.0.23/test/
--rw-r--r--   0 soatra     (501) staff       (20)     2889 2023-05-15 02:48:58.000000 eyes_soatra-0.0.23/test/test.py
--rw-r--r--   0 soatra     (501) staff       (20)      332 2023-05-15 03:21:33.000000 eyes_soatra-0.0.23/test/test2.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-23 06:21:56.981136 eyes_soatra-0.0.24/
+-rw-r--r--   0 soatra     (501) staff       (20)       13 2023-05-02 07:13:47.000000 eyes_soatra-0.0.24/LICENSE
+-rw-r--r--   0 soatra     (501) staff       (20)      554 2023-05-23 06:21:56.980962 eyes_soatra-0.0.24/PKG-INFO
+-rw-r--r--   0 soatra     (501) staff       (20)       49 2023-05-11 09:42:34.000000 eyes_soatra-0.0.24/README.md
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-23 06:21:56.973509 eyes_soatra-0.0.24/eyes_soatra/
+-rw-r--r--   0 soatra     (501) staff       (20)       28 2023-05-02 07:14:02.000000 eyes_soatra-0.0.24/eyes_soatra/__init__.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-23 06:21:56.974510 eyes_soatra-0.0.24/eyes_soatra/constant/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:45:06.000000 eyes_soatra-0.0.24/eyes_soatra/constant/__init__.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-23 06:21:56.974739 eyes_soatra-0.0.24/eyes_soatra/constant/depends/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:46:17.000000 eyes_soatra-0.0.24/eyes_soatra/constant/depends/__init__.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-23 06:21:56.975449 eyes_soatra-0.0.24/eyes_soatra/constant/depends/app_date/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:54:07.000000 eyes_soatra-0.0.24/eyes_soatra/constant/depends/app_date/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)      395 2023-05-23 05:04:15.000000 eyes_soatra-0.0.24/eyes_soatra/constant/depends/app_date/end.py
+-rw-r--r--   0 soatra     (501) staff       (20)      260 2023-05-23 04:44:21.000000 eyes_soatra-0.0.24/eyes_soatra/constant/depends/app_date/period.py
+-rw-r--r--   0 soatra     (501) staff       (20)      261 2023-05-23 04:44:37.000000 eyes_soatra-0.0.24/eyes_soatra/constant/depends/app_date/start.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-23 06:21:56.976019 eyes_soatra-0.0.24/eyes_soatra/constant/depends/view/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:56:44.000000 eyes_soatra-0.0.24/eyes_soatra/constant/depends/view/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)      276 2023-05-02 03:37:05.000000 eyes_soatra-0.0.24/eyes_soatra/constant/depends/view/no_data.py
+-rw-r--r--   0 soatra     (501) staff       (20)     7691 2023-05-11 01:49:20.000000 eyes_soatra-0.0.24/eyes_soatra/constant/depends/view/not_found.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-23 06:21:56.976352 eyes_soatra-0.0.24/eyes_soatra/constant/libs/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:47:14.000000 eyes_soatra-0.0.24/eyes_soatra/constant/libs/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)      378 2023-05-23 01:48:11.000000 eyes_soatra-0.0.24/eyes_soatra/constant/libs/requests.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-23 06:21:56.976656 eyes_soatra-0.0.24/eyes_soatra/constant/user/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:46:27.000000 eyes_soatra-0.0.24/eyes_soatra/constant/user/__init__.py
+-rw-rw-r--   0 soatra     (501) staff       (20)  1339531 2023-05-11 09:13:03.000000 eyes_soatra-0.0.24/eyes_soatra/constant/user/user_agents.py
+-rw-r--r--   0 soatra     (501) staff       (20)      220 2023-05-23 02:00:10.000000 eyes_soatra-0.0.24/eyes_soatra/constant/vars.py
+-rw-r--r--   0 soatra     (501) staff       (20)      109 2023-05-23 06:21:34.000000 eyes_soatra-0.0.24/eyes_soatra/eyes.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-23 06:21:56.979417 eyes_soatra-0.0.24/eyes_soatra/funcs/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 01:41:01.000000 eyes_soatra-0.0.24/eyes_soatra/funcs/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)     6994 2023-05-23 06:20:17.000000 eyes_soatra-0.0.24/eyes_soatra/funcs/app_span.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-23 06:21:56.980047 eyes_soatra-0.0.24/eyes_soatra/funcs/utils/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-23 02:07:05.000000 eyes_soatra-0.0.24/eyes_soatra/funcs/utils/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)      168 2023-05-23 02:06:56.000000 eyes_soatra-0.0.24/eyes_soatra/funcs/utils/dict.py
+-rw-r--r--   0 soatra     (501) staff       (20)       82 2023-05-23 02:06:48.000000 eyes_soatra-0.0.24/eyes_soatra/funcs/utils/string.py
+-rw-r--r--   0 soatra     (501) staff       (20)    12655 2023-05-23 06:16:25.000000 eyes_soatra-0.0.24/eyes_soatra/funcs/view_page.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-23 06:21:56.974240 eyes_soatra-0.0.24/eyes_soatra.egg-info/
+-rw-r--r--   0 soatra     (501) staff       (20)      554 2023-05-23 06:21:56.000000 eyes_soatra-0.0.24/eyes_soatra.egg-info/PKG-INFO
+-rw-r--r--   0 soatra     (501) staff       (20)     1050 2023-05-23 06:21:56.000000 eyes_soatra-0.0.24/eyes_soatra.egg-info/SOURCES.txt
+-rw-r--r--   0 soatra     (501) staff       (20)        1 2023-05-23 06:21:56.000000 eyes_soatra-0.0.24/eyes_soatra.egg-info/dependency_links.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       43 2023-05-23 06:21:56.000000 eyes_soatra-0.0.24/eyes_soatra.egg-info/requires.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       12 2023-05-23 06:21:56.000000 eyes_soatra-0.0.24/eyes_soatra.egg-info/top_level.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       38 2023-05-23 06:21:56.981193 eyes_soatra-0.0.24/setup.cfg
+-rw-r--r--   0 soatra     (501) staff       (20)     1131 2023-05-23 02:47:19.000000 eyes_soatra-0.0.24/setup.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-23 06:21:56.980607 eyes_soatra-0.0.24/test/
+-rw-r--r--   0 soatra     (501) staff       (20)     4574 2023-05-23 05:08:45.000000 eyes_soatra-0.0.24/test/test.py
+-rw-r--r--   0 soatra     (501) staff       (20)      250 2023-05-23 06:16:40.000000 eyes_soatra-0.0.24/test/test2.py
```

### Comparing `eyes_soatra-0.0.23/PKG-INFO` & `eyes_soatra-0.0.24/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyes_soatra
-Version: 0.0.23
+Version: 0.0.24
 Summary: Eyes
 Author: Soatra
 Author-email: johnsoatra@gmail.com
 Keywords: python,crawler,scanner,requests
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eyes_soatra-0.0.23/eyes_soatra/depends/depends_404.py` & `eyes_soatra-0.0.24/eyes_soatra/constant/depends/view/not_found.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.23/eyes_soatra/eyes.py` & `eyes_soatra-0.0.24/eyes_soatra/funcs/view_page.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,81 +1,45 @@
 #!python3
-from eyes_soatra.depends.depends_no_data import depends as __depends_no_data
-from eyes_soatra.depends.depends_404 import depends as __depends_404
-from eyes_soatra.needs.user_agents import User_Agents as __User_Agents
+from eyes_soatra.constant.depends.view.no_data import depends as __depends_no_data
+from eyes_soatra.constant.depends.view.not_found import depends as __depends_404
+from eyes_soatra.constant.user.user_agents import User_Agents as __User_Agents
+from eyes_soatra.constant.libs.requests import requests as __requests
+from eyes_soatra.constant.vars import all_header_xpaths as __header_xpaths_all
+from eyes_soatra.funcs.utils.dict import sort_dict as __sort_dict
+from eyes_soatra.funcs.utils.string import strip as __strip
+
 from translate import Translator as __Translator
 from requests_html import HTML as __HTML
+
 import jellyfish as __jellyfish
-import requests as __requests
 import random as __random
 import time as __time
 import re as __re
 
-# Suppress only the single warning from urllib3 needed.
-__requests.packages.urllib3.disable_warnings()
-__requests.packages.urllib3.util.ssl_.DEFAULT_CIPHERS += ':HIGH:!DH:!aNULL'
-try:
-    __requests.packages.urllib3.contrib.pyopenssl.util.ssl_.DEFAULT_CIPHERS += ':HIGH:!DH:!aNULL'
-except AttributeError:
-    # no pyopenssl support used / needed / available
-    pass
 
 # private global variables
 __separator = '\||-|:'
 __header_min_length = 3
 __paragraph_min_length = 7
 __container = 'self::div or self::span or self::table'
 __header_xpaths = [
     '//title',
     '//h1[self::*//text() and last()=1]',
     '//h2[self::*//text() and last()=1]'
 ]
-__header_xpaths_all = [
-    '//title',
-    '//h1',
-    '//h2',
-    '//h3',
-    '//h4',
-    '//h5',
-    '//h6',
-    '//p',
-    '//a',
-    '//button',
-    
-    '//span',
-    '//div',
-    
-    '//li',
-    '//dt',
-    '//dd'
-]
 __paragraph_xpaths = [
     '//p[@class="no_data"]',
     '//h1[self::*//text()]/following-sibling::p[1]',
     '//h1[self::*//text()]/following-sibling::*//p[1]',
     f'//*[({__container}) and self::*//h1[self::*//text()] and self::*/*[last()=1]]/following-sibling::*[1][{__container}]//p[1]'
 ]
 __content_xpaths = [
     '//h1[self::*//text()]/following-sibling::*|//h1[self::*//text()]/following-sibling::*//*|//*[self::*//h1[self::*//text()] and self::*/*[last()=1]]/following-sibling::*[1]//*'
 ]
 
-# private functions
-def __sort_dict(dict):
-    keys = list(dict.keys())
-    keys.sort()
-    new_dict = {}
-    
-    for key in keys:
-        new_dict[key] = dict[key]
-    
-    return new_dict
-
-def __strip(text):
-    return __re.sub(r'\s+', ' ', text).strip()
-
 def __get_highlight(
     html,
     header_xpath,
     paragraph_xpath,
     content_xpath,
     allow_all_tags,
 ):
@@ -99,42 +63,47 @@
 ):
     header_texts = []
     paragraph_texts = []
     content_texts = []
     
     for xpath in (__header_xpaths_all if allow_all_tags else __header_xpaths) + (header_xpath if type(header_xpath) == list else []):
         header_list = html.xpath(f'({xpath})//text()')
-        header = ' '.join(header_list)
-        header = __strip(header)
         
-        if len(header) >= __header_min_length:
-            header_texts.append(header)
+        for header in header_list:
+            header = __strip(header)
+            
+            if len(header) >= __header_min_length:
+                header_texts.append(header)
     
     for xpath in __paragraph_xpaths + (paragraph_xpath if type(paragraph_xpath) == list else []):
         paragraph_list = html.xpath(f'({xpath})//text()')
-        paragraph = ' '.join(paragraph_list)
-        paragraph = __strip(paragraph)
         
-        if len(paragraph) >= __paragraph_min_length:
-            paragraph_texts.append(paragraph)
+        for paragraph in paragraph_list:
+            paragraph = __strip(paragraph)
+            
+            if len(paragraph) >= __paragraph_min_length:
+                paragraph_texts.append(paragraph)
 
-        if len(paragraph_texts):
-            break
+            if len(paragraph_texts):
+                break
+            
         # for paragraph in paragraph_list:
     
     for xpath in __content_xpaths + (content_xpath if type(content_xpath) == list else []):
         content_list = html.xpath(f'({xpath})//text()')
-        content = ' '.join(content_list)
-        content = __strip(content)
         
-        if len(content) > 0:
-            content_texts.append(content)
+        for content in content_list:
+            content = __strip(content)
+            
+            if len(content) > 0:
+                content_texts.append(content)
 
-        if len(content_texts):
-            break
+            if len(content_texts):
+                break
+            
         # for content in content_list:
             
     return {
         'headers': header_texts,
         'paragraphs': paragraph_texts,
         'contents': content_texts,
     }
```

### Comparing `eyes_soatra-0.0.23/eyes_soatra/needs/user_agents.py` & `eyes_soatra-0.0.24/eyes_soatra/constant/user/user_agents.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.23/eyes_soatra.egg-info/PKG-INFO` & `eyes_soatra-0.0.24/eyes_soatra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyes-soatra
-Version: 0.0.23
+Version: 0.0.24
 Summary: Eyes
 Author: Soatra
 Author-email: johnsoatra@gmail.com
 Keywords: python,crawler,scanner,requests
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eyes_soatra-0.0.23/setup.py` & `eyes_soatra-0.0.24/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 NAME = 'eyes_soatra'
-VERSION = '0.0.23'
+VERSION = '0.0.24'
 DESCRIPTION = 'Eyes'
 
 AUTHOR_NAME = 'Soatra'
 AUTHOR_EMAIL = 'johnsoatra@gmail.com'
 
 # Setting up
 setup(
```

