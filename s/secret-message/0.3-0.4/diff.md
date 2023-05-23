# Comparing `tmp/secret_message-0.3.tar.gz` & `tmp/secret_message-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secret_message-0.3.tar", last modified: Mon May 22 14:18:39 2023, max compression
+gzip compressed data, was "secret_message-0.4.tar", last modified: Mon May 22 19:09:13 2023, max compression
```

## Comparing `secret_message-0.3.tar` & `secret_message-0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-22 14:18:39.395295 secret_message-0.3/
--rw-rw----   0 root         (0) everybody  (9997)     1065 2023-05-22 13:17:48.000000 secret_message-0.3/LICENSE.txt
--rw-rw----   0 root         (0) everybody  (9997)     2523 2023-05-22 14:18:39.385295 secret_message-0.3/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     2140 2023-05-12 19:51:42.000000 secret_message-0.3/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-22 14:18:39.325296 secret_message-0.3/secret_message/
--rw-rw----   0 root         (0) everybody  (9997)     1762 2023-05-12 17:57:05.000000 secret_message-0.3/secret_message/__init__.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-22 14:18:39.375295 secret_message-0.3/secret_message.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     2523 2023-05-22 14:18:39.000000 secret_message-0.3/secret_message.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      209 2023-05-22 14:18:39.000000 secret_message-0.3/secret_message.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-22 14:18:39.000000 secret_message-0.3/secret_message.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       15 2023-05-22 14:18:39.000000 secret_message-0.3/secret_message.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-22 14:18:39.395295 secret_message-0.3/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     2691 2023-05-22 14:16:00.000000 secret_message-0.3/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-22 19:09:13.569997 secret_message-0.4/
+-rw-rw----   0 root         (0) everybody  (9997)     1065 2023-05-22 13:17:48.000000 secret_message-0.4/LICENSE.txt
+-rw-rw----   0 root         (0) everybody  (9997)     2523 2023-05-22 19:09:13.569997 secret_message-0.4/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     2140 2023-05-12 19:51:42.000000 secret_message-0.4/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-22 19:09:13.469997 secret_message-0.4/secret_message/
+-rw-rw----   0 root         (0) everybody  (9997)     1762 2023-05-22 19:05:19.000000 secret_message-0.4/secret_message/__init__.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-22 19:09:13.539997 secret_message-0.4/secret_message.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     2523 2023-05-22 19:09:13.000000 secret_message-0.4/secret_message.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      209 2023-05-22 19:09:13.000000 secret_message-0.4/secret_message.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-22 19:09:13.000000 secret_message-0.4/secret_message.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       15 2023-05-22 19:09:13.000000 secret_message-0.4/secret_message.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-22 19:09:13.569997 secret_message-0.4/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     2691 2023-05-22 19:05:32.000000 secret_message-0.4/setup.py
```

### Comparing `secret_message-0.3/LICENSE.txt` & `secret_message-0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `secret_message-0.3/PKG-INFO` & `secret_message-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secret_message
-Version: 0.3
+Version: 0.4
 Summary: Create and share a Message Secretly.
 Author: E Lusifa Taehyung
 Author-email: purplebird7613@gmail.com
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `secret_message-0.3/README.md` & `secret_message-0.4/README.md`

 * *Files identical despite different names*

### Comparing `secret_message-0.3/secret_message/__init__.py` & `secret_message-0.4/secret_message/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 import json
 import os
 
-host = "https://secret-message-5uxb.onrender.com"
+host = "https://secretmessage.pythonanywhere.com"
 
 # ====== Getting Token as User ======
 def user(username):
 	url = f"{host}/api/create-user/"
 	
 	data = {
 			"name" : username
```

### Comparing `secret_message-0.3/secret_message.egg-info/PKG-INFO` & `secret_message-0.4/secret_message.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secret-message
-Version: 0.3
+Version: 0.4
 Summary: Create and share a Message Secretly.
 Author: E Lusifa Taehyung
 Author-email: purplebird7613@gmail.com
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `secret_message-0.3/setup.py` & `secret_message-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 
 """          
 
 setuptools.setup(
 
 	name = 'secret_message', 
 
-	version = '0.3',
+	version = '0.4',
 
 	author = "E Lusifa Taehyung",
 
 	author_email = "purplebird7613@gmail.com",
 
 	description = "Create and share a Message Secretly.",
```

