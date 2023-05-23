# Comparing `tmp/docxreviews2txt-0.2.tar.gz` & `tmp/docxreviews2txt-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docxreviews2txt-0.2.tar", last modified: Mon Apr 25 17:20:35 2022, max compression
+gzip compressed data, was "docxreviews2txt-0.3.tar", last modified: Wed May 17 21:09:00 2023, max compression
```

## Comparing `docxreviews2txt-0.2.tar` & `docxreviews2txt-0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-04-25 17:20:35.436286 docxreviews2txt-0.2/
--rw-rw-rw-   0        0        0     1917 2022-04-25 17:20:35.435281 docxreviews2txt-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1220 2022-04-25 16:27:34.000000 docxreviews2txt-0.2/README.md
-drwxrwxrwx   0        0        0        0 2022-04-25 17:20:35.389482 docxreviews2txt-0.2/docxreviews2txt/
--rw-rw-rw-   0        0        0       34 2022-04-17 13:01:22.000000 docxreviews2txt-0.2/docxreviews2txt/__init__.py
--rw-rw-rw-   0        0        0     6134 2022-04-25 17:19:51.000000 docxreviews2txt-0.2/docxreviews2txt/docxreviews2txt.py
-drwxrwxrwx   0        0        0        0 2022-04-25 17:20:35.430287 docxreviews2txt-0.2/docxreviews2txt.egg-info/
--rw-rw-rw-   0        0        0     1917 2022-04-25 17:20:34.000000 docxreviews2txt-0.2/docxreviews2txt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2022-04-25 17:20:35.000000 docxreviews2txt-0.2/docxreviews2txt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-25 17:20:34.000000 docxreviews2txt-0.2/docxreviews2txt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2022-04-25 17:20:34.000000 docxreviews2txt-0.2/docxreviews2txt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2022-04-25 17:20:35.000000 docxreviews2txt-0.2/docxreviews2txt.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-04-25 17:20:35.432291 docxreviews2txt-0.2/scripts/
--rw-rw-rw-   0        0        0      133 2022-04-17 13:01:35.000000 docxreviews2txt-0.2/scripts/docxreviews2txt
--rw-rw-rw-   0        0        0       42 2022-04-25 17:20:35.436286 docxreviews2txt-0.2/setup.cfg
--rw-rw-rw-   0        0        0      997 2022-04-25 17:20:17.000000 docxreviews2txt-0.2/setup.py
+drwxr-xr-x   0 alan      (1000) alan      (1000)        0 2023-05-17 21:09:00.401589 docxreviews2txt-0.3/
+-rw-r--r--   0 alan      (1000) alan      (1000)     1853 2023-05-17 21:09:00.401589 docxreviews2txt-0.3/PKG-INFO
+-rw-r--r--   0 alan      (1000) alan      (1000)     1220 2023-05-17 21:08:18.000000 docxreviews2txt-0.3/README.md
+drwxr-xr-x   0 alan      (1000) alan      (1000)        0 2023-05-17 21:09:00.391589 docxreviews2txt-0.3/docxreviews2txt/
+-rw-r--r--   0 alan      (1000) alan      (1000)       75 2023-05-17 21:08:18.000000 docxreviews2txt-0.3/docxreviews2txt/__init__.py
+-rw-r--r--   0 alan      (1000) alan      (1000)     6272 2023-05-17 21:08:18.000000 docxreviews2txt-0.3/docxreviews2txt/docxreviews2txt.py
+drwxr-xr-x   0 alan      (1000) alan      (1000)        0 2023-05-17 21:09:00.401589 docxreviews2txt-0.3/docxreviews2txt.egg-info/
+-rw-r--r--   0 alan      (1000) alan      (1000)     1853 2023-05-17 21:09:00.000000 docxreviews2txt-0.3/docxreviews2txt.egg-info/PKG-INFO
+-rw-r--r--   0 alan      (1000) alan      (1000)      299 2023-05-17 21:09:00.000000 docxreviews2txt-0.3/docxreviews2txt.egg-info/SOURCES.txt
+-rw-r--r--   0 alan      (1000) alan      (1000)        1 2023-05-17 21:09:00.000000 docxreviews2txt-0.3/docxreviews2txt.egg-info/dependency_links.txt
+-rw-r--r--   0 alan      (1000) alan      (1000)       28 2023-05-17 21:09:00.000000 docxreviews2txt-0.3/docxreviews2txt.egg-info/requires.txt
+-rw-r--r--   0 alan      (1000) alan      (1000)        1 2023-05-17 21:09:00.000000 docxreviews2txt-0.3/docxreviews2txt.egg-info/top_level.txt
+drwxr-xr-x   0 alan      (1000) alan      (1000)        0 2023-05-17 21:09:00.401589 docxreviews2txt-0.3/scripts/
+-rw-r--r--   0 alan      (1000) alan      (1000)      133 2023-05-17 21:08:18.000000 docxreviews2txt-0.3/scripts/docxreviews2txt
+-rw-r--r--   0 alan      (1000) alan      (1000)       38 2023-05-17 21:09:00.401589 docxreviews2txt-0.3/setup.cfg
+-rw-r--r--   0 alan      (1000) alan      (1000)      997 2023-05-17 21:08:18.000000 docxreviews2txt-0.3/setup.py
```

### Comparing `docxreviews2txt-0.2/PKG-INFO` & `docxreviews2txt-0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-Metadata-Version: 2.1
-Name: docxreviews2txt
-Version: 0.2
-Summary: Extract reviews changes and commentaries from a docx file as plan text.
-Home-page: http://github.com/alanlivio/docxreviews2txt
-Author: Alan Guedes
-Author-email: alanlivio@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
-Classifier: Environment :: Console
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >= 3.6
-Description-Content-Type: text/markdown
-
-# docxreviews2txt
-
-Extract reviews changes and comments from a docx file as plan text.
-
-## How to install? 
-
-```bash
-pip install docxreviews2txt
-```
-
-## How to use?
-
-```txt
-$ docxreviews2txt -h
-usage: docxreviews2txt [-h] [--save_txt | --save_p_xml] docx
-
-positional arguments:
-  docx          input docx
-
-options:
-  -h, --help    show this help message and exit
-  --save_txt    save review as txt
-  --save_p_xml  save extracted paragraphs xml for debugging
-```
-  
-Example:
-
-```txt
-$ docxreviews2txt tests/lorem_ipsum.docx
-# comments
-- This is a comment from docx
-# Typos and rewriting suggestions
-- sit amet, consectetur  -> sit amet, consectetur Lorem ipsum
-- sit amet, consectetur adipiscing elit, sed do -> sit amet, consectetur elit, sed do
-- sit amet, consectetur adipiscing elit, sed -> sit amet, consectetur adipiscings elit, sed
-- enim ad minim veniam, quis nostrud -> enim ad minim do veniam, quis nostrud
-- enim ad minim veniam -> enim ad minim Lorem veniam
-- veniam, quis nostrud -> veniam ipsum, quis nostrud
-- sit amet, consectetur adipiscing elit, sed do -> sit amet, consectetur elit, sed do
-```
-
-## References
-
-- https://github.com/ankushshah89/python-docx2txt
-
+Metadata-Version: 2.1
+Name: docxreviews2txt
+Version: 0.3
+Summary: Extract reviews changes and commentaries from a docx file as plan text.
+Home-page: http://github.com/alanlivio/docxreviews2txt
+Author: Alan Guedes
+Author-email: alanlivio@gmail.com
+License: MIT
+Platform: UNKNOWN
+Classifier: Development Status :: 1 - Planning
+Classifier: Environment :: Console
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >= 3.6
+Description-Content-Type: text/markdown
+
+# docxreviews2txt
+
+Extract reviews changes and comments from a docx file as plan text.
+
+## How to install? 
+
+```bash
+pip install docxreviews2txt
+```
+
+## How to use?
+
+```txt
+$ docxreviews2txt -h
+usage: docxreviews2txt [-h] [--save_txt | --save_p_xml] docx
+
+positional arguments:
+  docx          input docx
+
+options:
+  -h, --help    show this help message and exit
+  --save_txt    save review as txt
+  --save_p_xml  save extracted paragraphs xml for debugging
+```
+  
+Example:
+
+```txt
+$ docxreviews2txt tests/lorem_ipsum.docx
+# comments
+- This is a comment from docx
+# Typos and rewriting suggestions
+- sit amet, consectetur  -> sit amet, consectetur Lorem ipsum
+- sit amet, consectetur adipiscing elit, sed do -> sit amet, consectetur elit, sed do
+- sit amet, consectetur adipiscing elit, sed -> sit amet, consectetur adipiscings elit, sed
+- enim ad minim veniam, quis nostrud -> enim ad minim do veniam, quis nostrud
+- enim ad minim veniam -> enim ad minim Lorem veniam
+- veniam, quis nostrud -> veniam ipsum, quis nostrud
+- sit amet, consectetur adipiscing elit, sed do -> sit amet, consectetur elit, sed do
+```
+
+## References
+
+- https://github.com/ankushshah89/python-docx2txt
+
```

### Comparing `docxreviews2txt-0.2/README.md` & `docxreviews2txt-0.3/README.md`

 * *Files identical despite different names*

### Comparing `docxreviews2txt-0.2/docxreviews2txt/docxreviews2txt.py` & `docxreviews2txt-0.3/docxreviews2txt/docxreviews2txt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from docx import Document
 import xml.etree.ElementTree as ET
 import argparse
 import os
-import sys
 import subprocess
 import pathlib
 from os.path import exists
 import zipfile
 import tempfile
 import shutil
 
+__version__ = '0.3'
 
 WORD_NS = 'http://schemas.openxmlformats.org/wordprocessingml/2006/main'
 NS_MAP = {"w": WORD_NS}
 ET_WORD_NS = '{' + WORD_NS + '}'
 ET_TEXT = ET_WORD_NS + 't'
 ET_DEL = ET_WORD_NS + 'del'
 ET_INS = ET_WORD_NS + 'ins'
@@ -101,69 +101,67 @@
         # changes
         self.reviews_append("# Typos and rewriting suggestions")
         for p in self.paragraphs:
             xml = p._p.xml
             root = ET.fromstring(xml)
             if len(root.findall('.//w:del', NS_MAP)) == 0 and len(root.findall('.//w:ins', NS_MAP)) == 0:
                 continue
-            for index in range(len(root)-1):
-                prev = root[index-1]
+            for index in range(len(root) - 1):
+                prev = root[index - 1]
                 cur = root[index]
-                next = root[index+1]
+                next = root[index + 1]
                 # DEL followed by INS
                 if (cur.tag == ET_DEL and next.tag == ET_INS):
                     del_text = str_deltext_elms(cur)
                     ins_text = str_t_elms(next)
-                    left_text = str_left_t_elms(root, index-1)
-                    right_text = str_right_t_elms(root, index+2)
+                    left_text = str_left_t_elms(root, index - 1)
+                    right_text = str_right_t_elms(root, index + 2)
                     self.reviews_append("- " + left_text + del_text + right_text +
                                         " -> " + left_text + ins_text + right_text)
                 # INS alone
                 elif (cur.tag == ET_INS and prev.tag != ET_DEL):
                     ins_text = str_t_elms(cur)
-                    left_text = str_left_t_elms(root, index-1)
+                    left_text = str_left_t_elms(root, index - 1)
                     right_text = str_right_t_elms(root, index)
                     self.reviews_append("- " + left_text + right_text +
                                         " -> " + left_text + ins_text + right_text)
                 # DEL alone
                 elif (cur.tag == ET_DEL and next.tag != ET_INS):
                     del_text = str_deltext_elms(cur)
-                    left_text = str_left_t_elms(root, index-1)
-                    right_text = str_right_t_elms(root, index+1)
+                    left_text = str_left_t_elms(root, index - 1)
+                    right_text = str_right_t_elms(root, index + 1)
                     self.reviews_append("- " + left_text + del_text + right_text +
                                         " -> " + left_text + right_text)
 
     def save_reviews_to_file(self):
-        file_txt_name = str(os.path.splitext(self.file_docx)[0])+'_review.txt'
+        file_txt_name = str(os.path.splitext(self.file_docx)[0]) + '_review.txt'
         with open(file_txt_name, "w") as file:
             for change in self.reviews:
                 file.write(f"{change}\n")
 
     def save_xml_p_elems(self):
-        file_txt_name = str(os.path.splitext(self.file_docx)[0])+'.xml'
+        file_txt_name = str(os.path.splitext(self.file_docx)[0]) + '.xml'
         with open(file_txt_name, "w") as file:
             for p in self.paragraphs:
                 xml = p._p.xml
                 file.write(f"{xml}\n")
 
 
 def main(argv):
     parser = argparse.ArgumentParser()
-
-
-
     parser.add_argument("docx", help="input docx", type=pathlib.Path)
     group = parser.add_mutually_exclusive_group()
     group.add_argument('--save_txt', help='save review as txt', action="store_true")
     group.add_argument('--save_p_xml', help='save extracted paragraphs xml for debugging', action="store_true")
+    parser.add_argument('--version', help='show version', action='version', version='%(prog)s ' + __version__)
     args = parser.parse_args(argv)
     verbose = not args.save_p_xml and not args.save_txt
     if not exists(args.docx):
         print(f'{args.docx} does not exist')
         return 1
     docx_reviews = DocxReviews(args.docx, verbose)
     docx_reviews.parse()
     if args.save_p_xml:
         docx_reviews.save_xml_p_elems()
     if args.save_txt:
         docx_reviews.save_reviews_to_file()
-    return 0
+    return 0
```

### Comparing `docxreviews2txt-0.2/docxreviews2txt.egg-info/PKG-INFO` & `docxreviews2txt-0.3/docxreviews2txt.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-Metadata-Version: 2.1
-Name: docxreviews2txt
-Version: 0.2
-Summary: Extract reviews changes and commentaries from a docx file as plan text.
-Home-page: http://github.com/alanlivio/docxreviews2txt
-Author: Alan Guedes
-Author-email: alanlivio@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
-Classifier: Environment :: Console
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >= 3.6
-Description-Content-Type: text/markdown
-
-# docxreviews2txt
-
-Extract reviews changes and comments from a docx file as plan text.
-
-## How to install? 
-
-```bash
-pip install docxreviews2txt
-```
-
-## How to use?
-
-```txt
-$ docxreviews2txt -h
-usage: docxreviews2txt [-h] [--save_txt | --save_p_xml] docx
-
-positional arguments:
-  docx          input docx
-
-options:
-  -h, --help    show this help message and exit
-  --save_txt    save review as txt
-  --save_p_xml  save extracted paragraphs xml for debugging
-```
-  
-Example:
-
-```txt
-$ docxreviews2txt tests/lorem_ipsum.docx
-# comments
-- This is a comment from docx
-# Typos and rewriting suggestions
-- sit amet, consectetur  -> sit amet, consectetur Lorem ipsum
-- sit amet, consectetur adipiscing elit, sed do -> sit amet, consectetur elit, sed do
-- sit amet, consectetur adipiscing elit, sed -> sit amet, consectetur adipiscings elit, sed
-- enim ad minim veniam, quis nostrud -> enim ad minim do veniam, quis nostrud
-- enim ad minim veniam -> enim ad minim Lorem veniam
-- veniam, quis nostrud -> veniam ipsum, quis nostrud
-- sit amet, consectetur adipiscing elit, sed do -> sit amet, consectetur elit, sed do
-```
-
-## References
-
-- https://github.com/ankushshah89/python-docx2txt
-
+Metadata-Version: 2.1
+Name: docxreviews2txt
+Version: 0.3
+Summary: Extract reviews changes and commentaries from a docx file as plan text.
+Home-page: http://github.com/alanlivio/docxreviews2txt
+Author: Alan Guedes
+Author-email: alanlivio@gmail.com
+License: MIT
+Platform: UNKNOWN
+Classifier: Development Status :: 1 - Planning
+Classifier: Environment :: Console
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >= 3.6
+Description-Content-Type: text/markdown
+
+# docxreviews2txt
+
+Extract reviews changes and comments from a docx file as plan text.
+
+## How to install? 
+
+```bash
+pip install docxreviews2txt
+```
+
+## How to use?
+
+```txt
+$ docxreviews2txt -h
+usage: docxreviews2txt [-h] [--save_txt | --save_p_xml] docx
+
+positional arguments:
+  docx          input docx
+
+options:
+  -h, --help    show this help message and exit
+  --save_txt    save review as txt
+  --save_p_xml  save extracted paragraphs xml for debugging
+```
+  
+Example:
+
+```txt
+$ docxreviews2txt tests/lorem_ipsum.docx
+# comments
+- This is a comment from docx
+# Typos and rewriting suggestions
+- sit amet, consectetur  -> sit amet, consectetur Lorem ipsum
+- sit amet, consectetur adipiscing elit, sed do -> sit amet, consectetur elit, sed do
+- sit amet, consectetur adipiscing elit, sed -> sit amet, consectetur adipiscings elit, sed
+- enim ad minim veniam, quis nostrud -> enim ad minim do veniam, quis nostrud
+- enim ad minim veniam -> enim ad minim Lorem veniam
+- veniam, quis nostrud -> veniam ipsum, quis nostrud
+- sit amet, consectetur adipiscing elit, sed do -> sit amet, consectetur elit, sed do
+```
+
+## References
+
+- https://github.com/ankushshah89/python-docx2txt
+
```

### Comparing `docxreviews2txt-0.2/setup.py` & `docxreviews2txt-0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     required = f.read().splitlines()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="docxreviews2txt",
-    version="0.2",
+    version="0.3",
     author="Alan Guedes",
     license='MIT',
     url="http://github.com/alanlivio/docxreviews2txt",
     python_requires='>= 3.6',
     install_requires=required,
     long_description=long_description,
     long_description_content_type="text/markdown",
```

