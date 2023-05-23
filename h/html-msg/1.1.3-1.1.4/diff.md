# Comparing `tmp/html_msg-1.1.3.tar.gz` & `tmp/html_msg-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html_msg-1.1.3.tar", last modified: Fri May 12 13:35:31 2023, max compression
+gzip compressed data, was "html_msg-1.1.4.tar", last modified: Tue May 23 19:04:39 2023, max compression
```

## Comparing `html_msg-1.1.3.tar` & `html_msg-1.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 13:35:31.937904 html_msg-1.1.3/
--rw-rw-rw-   0        0        0     1095 2023-05-06 11:32:57.000000 html_msg-1.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0     3965 2023-05-12 13:35:31.936906 html_msg-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     3383 2023-05-09 19:29:44.000000 html_msg-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 13:35:31.925935 html_msg-1.1.3/html_msg/
--rw-rw-rw-   0        0        0      115 2023-05-12 13:35:08.000000 html_msg-1.1.3/html_msg/__init__.py
--rw-rw-rw-   0        0        0    12112 2023-05-12 12:59:50.000000 html_msg-1.1.3/html_msg/html_message.py
--rw-rw-rw-   0        0        0    14937 2023-05-12 13:34:56.000000 html_msg-1.1.3/html_msg/html_table.py
-drwxrwxrwx   0        0        0        0 2023-05-12 13:35:31.936906 html_msg-1.1.3/html_msg.egg-info/
--rw-rw-rw-   0        0        0     3965 2023-05-12 13:35:31.000000 html_msg-1.1.3/html_msg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-05-12 13:35:31.000000 html_msg-1.1.3/html_msg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 13:35:31.000000 html_msg-1.1.3/html_msg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-12 13:35:31.000000 html_msg-1.1.3/html_msg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-12 13:35:31.000000 html_msg-1.1.3/html_msg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-12 13:35:31.937904 html_msg-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      823 2023-05-12 13:35:20.000000 html_msg-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 19:04:39.577057 html_msg-1.1.4/
+-rw-rw-rw-   0        0        0     1095 2023-05-06 11:32:57.000000 html_msg-1.1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     3988 2023-05-23 19:04:39.577057 html_msg-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3383 2023-05-09 19:29:44.000000 html_msg-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 19:04:39.573061 html_msg-1.1.4/html_msg/
+-rw-rw-rw-   0        0        0      115 2023-05-23 19:04:28.000000 html_msg-1.1.4/html_msg/__init__.py
+-rw-rw-rw-   0        0        0    12112 2023-05-12 12:59:50.000000 html_msg-1.1.4/html_msg/html_message.py
+-rw-rw-rw-   0        0        0    14824 2023-05-23 19:00:41.000000 html_msg-1.1.4/html_msg/html_table.py
+drwxrwxrwx   0        0        0        0 2023-05-23 19:04:39.577057 html_msg-1.1.4/html_msg.egg-info/
+-rw-rw-rw-   0        0        0     3988 2023-05-23 19:04:39.000000 html_msg-1.1.4/html_msg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-05-23 19:04:39.000000 html_msg-1.1.4/html_msg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 19:04:39.000000 html_msg-1.1.4/html_msg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-23 19:04:39.000000 html_msg-1.1.4/html_msg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-23 19:04:39.000000 html_msg-1.1.4/html_msg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 19:04:39.578055 html_msg-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      823 2023-05-23 19:03:41.000000 html_msg-1.1.4/setup.py
```

### Comparing `html_msg-1.1.3/LICENSE.txt` & `html_msg-1.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `html_msg-1.1.3/PKG-INFO` & `html_msg-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: html_msg
-Version: 1.1.3
+Version: 1.1.4
 Summary: This tool allows you to create HTML messages using simple methods, without the need to write HTML code manually.
 Home-page: https://github.com/Sirakan-B/html_msg/
-Download-URL: https://pypi.org/project/html-msg/
 Author: Sirakan Bagdasarian
 Author-email: bsirak@bk.ru
 License: MIT
+Download-URL: https://pypi.org/project/html-msg/
 Keywords: HTML,Message
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # What is it?
 
 **html_msg** is a Python package that provides functionality to build up HTML messages via simple methods, without the need to write HTML code manually.
 
@@ -143,7 +144,9 @@
 ```
 # the method 'to_string' returns HTML code in string formart. 
 # One can pass it to abstract email sender, which will send it to the recepient.
 html_code = message.to_string()
 ```
 
 
+
+
```

### Comparing `html_msg-1.1.3/README.md` & `html_msg-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `html_msg-1.1.3/html_msg/html_message.py` & `html_msg-1.1.4/html_msg/html_message.py`

 * *Files identical despite different names*

### Comparing `html_msg-1.1.3/html_msg/html_table.py` & `html_msg-1.1.4/html_msg/html_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
         "Modern":
         {
             "table_style": "border-top: solid #E0E0E0 1.0pt; border-left: none; border-bottom: solid #E0E0E0 1.0pt; border-right: none; padding: 3.75pt 3.75pt 3.75pt; color: #1B5198; text-align: left;",
             "header_style": "border-top: none; border-left: none; border-bottom: solid #E0E0E0 1.0pt; border-right: none; padding: 3.75pt 3.75pt 3.75pt; text-align: center; color: #6C8999"
         },
         
         "Grey":{
-            "table_style": "border: 1.5px solid #000000;text-align: center;border-collapse: collapse; padding: 5pt 5pt 5pt;color: black;",
-            "header_style": "border: 1.5px solid #000000;text-align: center;border-collapse: collapse;background: linear-gradient(to bottom, #dbdbdb 0%, #d3d3d3 66%, #CFCFCF 100%);border-bottom: 1.5px solid #000000;color: black;padding: 10pt 10pt 10pt;margin-left: auto;margin-right: auto;"
+            "table_style": "border: 1.5px solid; text-align: center;border-collapse: collapse; padding: 5pt 5pt 5pt; color: black;",
+            "header_style": "border: 1.5px solid;text-align: center;border-collapse: collapse; background: #D3D3D3; border-bottom: 1.5px solid; color: black; padding: 10pt 10pt 10pt;"
         },
         
     }
     
     def __init__(self, rows=None, headers=None):
         
         if rows is None:
```

### Comparing `html_msg-1.1.3/html_msg.egg-info/PKG-INFO` & `html_msg-1.1.4/html_msg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: html-msg
-Version: 1.1.3
+Version: 1.1.4
 Summary: This tool allows you to create HTML messages using simple methods, without the need to write HTML code manually.
 Home-page: https://github.com/Sirakan-B/html_msg/
-Download-URL: https://pypi.org/project/html-msg/
 Author: Sirakan Bagdasarian
 Author-email: bsirak@bk.ru
 License: MIT
+Download-URL: https://pypi.org/project/html-msg/
 Keywords: HTML,Message
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # What is it?
 
 **html_msg** is a Python package that provides functionality to build up HTML messages via simple methods, without the need to write HTML code manually.
 
@@ -143,7 +144,9 @@
 ```
 # the method 'to_string' returns HTML code in string formart. 
 # One can pass it to abstract email sender, which will send it to the recepient.
 html_code = message.to_string()
 ```
 
 
+
+
```

### Comparing `html_msg-1.1.3/setup.py` & `html_msg-1.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 
 
 setup_args = dict(
     name='html_msg',
-    version='1.1.3',
+    version='1.1.4',
     description='This tool allows you to create HTML messages using simple methods, without the need to write HTML code manually.',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n',
     license='MIT',
     packages=find_packages(),
     author='Sirakan Bagdasarian',
     author_email='bsirak@bk.ru',
```

