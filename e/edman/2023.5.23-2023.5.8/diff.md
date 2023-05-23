# Comparing `tmp/edman-2023.5.23.tar.gz` & `tmp/edman-2023.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edman-2023.5.23.tar", last modified: Tue May 23 00:16:00 2023, max compression
+gzip compressed data, was "edman-2023.5.8.tar", last modified: Mon May  8 02:04:22 2023, max compression
```

## Comparing `edman-2023.5.23.tar` & `edman-2023.5.8.tar`

### file list

```diff
@@ -1,61 +1,30 @@
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-23 00:16:00.980164 edman-2023.5.23/
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-23 00:16:00.970164 edman-2023.5.23/.github/
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-23 00:16:00.970164 edman-2023.5.23/.github/workflows/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1379 2023-05-10 06:43:20.000000 edman-2023.5.23/.github/workflows/unittest.yml
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2266 2022-07-27 01:25:38.000000 edman-2023.5.23/.gitignore
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-23 00:16:00.970164 edman-2023.5.23/.idea/
--rw-r--r--   0 ohno      (1000) ohno      (1000)      238 2022-04-13 07:00:02.000000 edman-2023.5.23/.idea/.gitignore
--rw-r--r--   0 ohno      (1000) ohno      (1000)      557 2023-04-10 07:58:11.000000 edman-2023.5.23/.idea/edman.iml
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-23 00:16:00.970164 edman-2023.5.23/.idea/inspectionProfiles/
--rw-r--r--   0 ohno      (1000) ohno      (1000)      179 2022-04-13 07:00:02.000000 edman-2023.5.23/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 ohno      (1000) ohno      (1000)      254 2023-04-10 07:58:11.000000 edman-2023.5.23/.idea/misc.xml
--rw-r--r--   0 ohno      (1000) ohno      (1000)      269 2022-04-13 07:00:02.000000 edman-2023.5.23/.idea/modules.xml
--rw-r--r--   0 ohno      (1000) ohno      (1000)      185 2022-04-13 07:00:02.000000 edman-2023.5.23/.idea/vcs.xml
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1115 2023-02-17 05:03:50.000000 edman-2023.5.23/LICENSE.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)     7613 2023-05-23 00:16:00.980164 edman-2023.5.23/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)     6049 2023-01-20 03:28:32.000000 edman-2023.5.23/README.rst
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-23 00:16:00.980164 edman-2023.5.23/edman/
--rw-r--r--   0 ohno      (1000) ohno      (1000)      167 2023-05-09 07:38:50.000000 edman-2023.5.23/edman/__init__.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1446 2023-05-17 07:27:32.000000 edman-2023.5.23/edman/config.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    16569 2023-05-22 08:18:53.000000 edman-2023.5.23/edman/convert.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    47620 2023-05-22 08:18:53.000000 edman-2023.5.23/edman/db.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)      644 2022-04-13 07:00:02.000000 edman-2023.5.23/edman/exceptions.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    24845 2023-05-22 08:18:53.000000 edman-2023.5.23/edman/file.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1487 2023-05-22 08:18:53.000000 edman-2023.5.23/edman/json_manager.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)        0 2023-05-22 08:18:53.000000 edman-2023.5.23/edman/py.typed
--rw-r--r--   0 ohno      (1000) ohno      (1000)     9619 2023-05-22 08:18:53.000000 edman-2023.5.23/edman/search.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    10913 2023-05-22 08:18:53.000000 edman-2023.5.23/edman/utils.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-23 00:16:00.980164 edman-2023.5.23/edman.egg-info/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     7613 2023-05-23 00:16:00.000000 edman-2023.5.23/edman.egg-info/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)      986 2023-05-23 00:16:00.000000 edman-2023.5.23/edman.egg-info/SOURCES.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2023-05-23 00:16:00.000000 edman-2023.5.23/edman.egg-info/dependency_links.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       54 2023-05-23 00:16:00.000000 edman-2023.5.23/edman.egg-info/requires.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       34 2023-05-23 00:16:00.000000 edman-2023.5.23/edman.egg-info/top_level.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1124 2023-05-23 00:14:40.000000 edman-2023.5.23/pyproject.toml
--rw-r--r--   0 ohno      (1000) ohno      (1000)      861 2023-05-17 07:27:32.000000 edman-2023.5.23/requirements.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       38 2023-05-23 00:16:00.980164 edman-2023.5.23/setup.cfg
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-23 00:16:00.980164 edman-2023.5.23/tests/
--rw-r--r--   0 ohno      (1000) ohno      (1000)        0 2022-04-13 07:00:02.000000 edman-2023.5.23/tests/__init__.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-23 00:16:00.980164 edman-2023.5.23/tests/ini/
--rw-r--r--   0 ohno      (1000) ohno      (1000)      166 2022-11-15 02:42:20.000000 edman-2023.5.23/tests/ini/test_db.ini.sample
--rw-r--r--   0 ohno      (1000) ohno      (1000)    12303 2022-04-13 07:00:02.000000 edman-2023.5.23/tests/test_convert.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    86854 2023-04-20 03:03:49.000000 edman-2023.5.23/tests/test_db.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    40726 2023-05-18 02:16:03.000000 edman-2023.5.23/tests/test_file.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     5837 2023-03-09 05:51:32.000000 edman-2023.5.23/tests/test_multiuser.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    19062 2023-04-05 05:00:36.000000 edman-2023.5.23/tests/test_search.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     7898 2022-04-13 07:00:02.000000 edman-2023.5.23/tests/test_utils.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-23 00:16:00.970164 edman-2023.5.23/venv/
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-23 00:16:00.980164 edman-2023.5.23/venv/bin/
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1725 2023-04-07 00:37:51.000000 edman-2023.5.23/venv/bin/jp.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      632 2023-05-17 00:07:28.000000 edman-2023.5.23/venv/bin/rst2html.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      754 2023-05-17 00:07:28.000000 edman-2023.5.23/venv/bin/rst2html4.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1089 2023-05-17 00:07:28.000000 edman-2023.5.23/venv/bin/rst2html5.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      831 2023-05-17 00:07:28.000000 edman-2023.5.23/venv/bin/rst2latex.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      654 2023-05-17 00:07:28.000000 edman-2023.5.23/venv/bin/rst2man.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      820 2023-05-17 00:07:28.000000 edman-2023.5.23/venv/bin/rst2odt.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      626 2023-05-17 00:07:28.000000 edman-2023.5.23/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      639 2023-05-17 00:07:28.000000 edman-2023.5.23/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      675 2023-05-17 00:07:28.000000 edman-2023.5.23/venv/bin/rst2s5.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      911 2023-05-17 00:07:28.000000 edman-2023.5.23/venv/bin/rst2xetex.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      640 2023-05-17 00:07:28.000000 edman-2023.5.23/venv/bin/rst2xml.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      708 2023-05-17 00:07:28.000000 edman-2023.5.23/venv/bin/rstpep2html.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-08 02:04:22.028113 edman-2023.5.8/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1115 2023-02-17 05:03:50.000000 edman-2023.5.8/LICENSE.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       19 2022-04-13 07:00:02.000000 edman-2023.5.8/MANIFEST.in
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     6379 2023-05-08 02:04:22.028113 edman-2023.5.8/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     6049 2023-01-20 03:28:32.000000 edman-2023.5.8/README.rst
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-08 02:04:22.028113 edman-2023.5.8/edman/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      167 2022-04-13 07:00:02.000000 edman-2023.5.8/edman/__init__.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1373 2023-03-15 05:16:00.000000 edman-2023.5.8/edman/config.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    16457 2023-03-15 05:16:00.000000 edman-2023.5.8/edman/convert.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    47757 2023-04-05 05:00:36.000000 edman-2023.5.8/edman/db.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      644 2022-04-13 07:00:02.000000 edman-2023.5.8/edman/exceptions.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    21800 2023-05-08 02:02:11.000000 edman-2023.5.8/edman/file.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1520 2023-03-09 05:51:32.000000 edman-2023.5.8/edman/json_manager.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     9907 2023-04-10 07:58:11.000000 edman-2023.5.8/edman/search.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    10958 2023-03-09 05:51:32.000000 edman-2023.5.8/edman/utils.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-08 02:04:22.028113 edman-2023.5.8/edman.egg-info/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     6379 2023-05-08 02:04:21.000000 edman-2023.5.8/edman.egg-info/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      470 2023-05-08 02:04:21.000000 edman-2023.5.8/edman.egg-info/SOURCES.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2023-05-08 02:04:21.000000 edman-2023.5.8/edman.egg-info/dependency_links.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       54 2023-05-08 02:04:21.000000 edman-2023.5.8/edman.egg-info/requires.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        6 2023-05-08 02:04:21.000000 edman-2023.5.8/edman.egg-info/top_level.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      707 2023-05-08 02:04:22.028113 edman-2023.5.8/setup.cfg
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       41 2022-04-13 07:00:02.000000 edman-2023.5.8/setup.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-08 02:04:22.028113 edman-2023.5.8/tests/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    12303 2022-04-13 07:00:02.000000 edman-2023.5.8/tests/test_convert.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    86854 2023-04-20 03:03:49.000000 edman-2023.5.8/tests/test_db.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    36850 2023-05-08 02:02:11.000000 edman-2023.5.8/tests/test_file.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     5837 2023-03-09 05:51:32.000000 edman-2023.5.8/tests/test_multiuser.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    19062 2023-04-05 05:00:36.000000 edman-2023.5.8/tests/test_search.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     7898 2022-04-13 07:00:02.000000 edman-2023.5.8/tests/test_utils.py
```

### Comparing `edman-2023.5.23/LICENSE.txt` & `edman-2023.5.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edman-2023.5.23/PKG-INFO` & `edman-2023.5.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,19 @@
 Metadata-Version: 2.1
 Name: edman
-Version: 2023.5.23
+Version: 2023.5.8
 Summary: KEK IMSS SBRC/PF Experimental Data Management System
-Author-email: Masaki Ohno <masakio@post.kek.jp>
+Home-page: https://github.com/ryde/edman
+Author: Masaki Ohno
+Author-email: masakio@post.kek.jp
 License: MIT License
-        
-        Copyright (c) 2019-2023 KEK IMSS SBRC/PF, Yusuke Yamada, Masaki Ohno
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-        
-Project-URL: documentation, https://ryde.github.io/edman/
-Project-URL: repository, https://github.com/ryde/edman
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database :: Front-Ends
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 edman
 =====
```

### Comparing `edman-2023.5.23/README.rst` & `edman-2023.5.8/README.rst`

 * *Files identical despite different names*

### Comparing `edman-2023.5.23/edman/config.py` & `edman-2023.5.8/edman/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,13 @@
     child = '_ed_child'  # 子のリファレンス情報
     file = '_ed_file'  # Grid.fsのリファレンス情報
     date = '#date'  # 日付に変換する場合のタグ
 
     fs_files = 'fs.files' # Grid.fsのファイルコレクション名
     fs_chunks = 'fs.chunks' # Grid.fsのファイルチャンクコレクション名
 
-    file_attachment = '_ed_attachment'  # 添付ファイルのキー
-
     # Gzip 圧縮レベル (ファイル圧縮時に使用)
     gzip_compress_level = 6
 
     # 再帰で回数の上限に達した場合、下記を適切な値で設定
     # import sys
     # sys.setrecursionlimit(1000)  # pythonのデフォルトは1000
```

### Comparing `edman-2023.5.23/edman/convert.py` & `edman-2023.5.8/edman/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import copy
-import datetime
-from typing import Union, Any
+from typing import Union
 from collections import defaultdict
 from bson import ObjectId, DBRef
 from edman.utils import Utils
 from edman.exceptions import (EdmanInternalError, EdmanFormatError)
 from edman import Config
 
 
@@ -111,15 +110,15 @@
             collection = list(insert_unit.keys())[0]
             for doc in insert_unit[collection]:
                 result[collection].append(doc)
 
         return [dict(result)]
 
     def _list_intercept_hook(self, collection: str,
-                             doc_with_child: dict | list) -> dict:
+                             doc_with_child: Union[dict, list]) -> dict:
         """
         | 対象ドキュメントの子要素のみを削除し、
         | 出力の対象コレクション内のリストに対して要素の追加もしくは書き換えを行う
 
         :param str collection:
         :param dict doc_with_child:
         :return: output
@@ -147,15 +146,15 @@
 
             # outputのデータを入れ替える
             if collection in output:
                 output[collection].append(tmp)
             else:
                 output[collection] = [tmp]
 
-        output: dict[Any, Any] = {}
+        output = {}
         if isinstance(doc_with_child, list):
             for i in doc_with_child:
                 child_delete(i)
         else:
             child_delete(doc_with_child)
 
         return output
@@ -309,16 +308,15 @@
                     if key == pull_key:
                         output.update({key: value})
                         break
                     [recursive(i) for i in value]
                 else:
                     continue
 
-        output: dict[
-            str, Union[str, int, list, dict, float, datetime.datetime]] = {}
+        output = {}
         recursive(data)
         return output
 
     def exclusion_key(self, doc: dict, ex_keys: tuple) -> dict:
         """
         指定のキーの要素を除外する
```

### Comparing `edman-2023.5.23/edman/db.py` & `edman-2023.5.8/edman/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import copy
 import urllib.parse
-from typing import Generator, Any
+from typing import Union
 from jmespath import exceptions as jms_exceptions, search as jms_search
 from pymongo import MongoClient, errors
 from bson import ObjectId, DBRef
 from edman.utils import Utils
 from edman.exceptions import (EdmanDbConnectError, EdmanInternalError,
                               EdmanDbProcessError, EdmanFormatError)
 from edman import Config, Convert, File
@@ -81,15 +81,15 @@
         statement = ""
         if kwargs.get('options'):
             for option in kwargs['options']:
                 connector = '&' if len(statement) else '?'
                 statement += connector + option
 
         mongo_uri = f'mongodb://{user}:{password}@{host}:{port}/{statement}'
-        client: MongoClient = MongoClient(mongo_uri)
+        client = MongoClient(mongo_uri)
 
         try:  # サーバの接続確認
             client.admin.command('ping')
         except errors.OperationFailure:
             raise EdmanDbConnectError('Invalid account.')
         except errors.ConnectionFailure:
             raise EdmanDbConnectError('Server not available.')
@@ -281,38 +281,40 @@
         except errors.InvalidName:
             raise EdmanDbProcessError('ロール名が不正です')
         except errors.OperationFailure:
             raise EdmanDbProcessError('ロール削除処理でエラーが起きました')
         except:
             raise
 
-    def insert(self, insert_data: list) -> list[dict[str, list[ObjectId]]]:
+    def insert(self, insert_data: list) -> list:
         """
         インサート実行
 
         :param list insert_data: バルクインサート対応のリストデータ
         :return: results
         :rtype: list
         """
-        results: list[dict[str, list[ObjectId]]] = []
+        results = []
         for i in insert_data:
             for collection, bulk_list in i.items():
                 if isinstance(bulk_list, dict):
                     bulk_list = [bulk_list]
                 try:
                     result = self.db[collection].insert_many(bulk_list)
                 except errors.BulkWriteError as e:
                     raise EdmanDbProcessError(
                         f'インサートに失敗しました:{e.details}\nインサート結果:{results}')
                 results.append({collection: result.inserted_ids})
 
         return results
 
     def find_collection_from_objectid(self,
-                                      oid: str | ObjectId) -> str | None:
+                                      oid: Union[str,
+                                      ObjectId]) -> Union[str,
+    None]:
         """
         | DB内のコレクションから指定のObjectIDを探し、所属しているコレクションを返す
         | DBに負荷がかかるので使用は注意が必要
 
         :param oid:
         :type oid: ObjectId or str
         :return: collection
@@ -324,30 +326,32 @@
         for collection in self.db.list_collection_names(filter=coll_filter):
             find_oid = self.db[collection].find_one({'_id': oid})
             if find_oid is not None and '_id' in find_oid:
                 result = collection
                 break
         return result
 
-    def doc(self, collection: str, oid: ObjectId | str,
-            query: list | None, reference_delete=True) -> dict | None:
+    def doc(self, collection: str, oid: Union[ObjectId, str],
+            query: Union[list, None], reference_delete=True) -> dict:
         """
         | refもしくはembのドキュメントを取得する
         | オプションでedman特有のデータ含んで取得することもできる
 
         :param str collection:
         :param oid:
         :type oid: ObjectId or str
         :param query:
         :type query: list or None
         :param bool reference_delete: default True
         :return: result
-        :rtype: dict or None
+        :rtype: dict
         """
-        doc = self.db[collection].find_one({'_id': Utils.conv_objectid(oid)})
+
+        oid = Utils.conv_objectid(oid)
+        doc = self.db[collection].find_one({'_id': oid})
 
         if doc is None:
             result = None
         else:
             # embの場合は指定階層のドキュメントを引き抜く
             # refの場合はdocの結果をそのまま入れる
             try:
@@ -380,16 +384,16 @@
         try:
             result = jms_search(s, doc)
         except jms_exceptions.ParseError:
             raise EdmanInternalError(f'クエリの変換が出来ませんでした: {s}')
 
         return result
 
-    def item_delete(self, collection: str, oid: ObjectId | str,
-                    delete_key: str, query: list | None) -> bool:
+    def item_delete(self, collection: str, oid: Union[ObjectId, str],
+                    delete_key: str, query: Union[list, None]) -> bool:
         """
         ドキュメントの項目を削除する
 
         :param str collection:
         :param oid:
         :type oid: str or ObjectId
         :param str delete_key:
@@ -452,15 +456,15 @@
                         buff = value
                     result.update({key: buff})
             except AttributeError:
                 raise EdmanInternalError(
                     f'日付変換に失敗しました.構造に問題があります. {amend}')
         return result
 
-    def update(self, collection: str, oid: str | ObjectId,
+    def update(self, collection: str, oid: Union[str, ObjectId],
                amend_data: dict, structure: str) -> bool:
         """
         修正データを用いてDBデータをアップデート
 
         :param str collection:
         :param oid:
         :type oid: str or ObjectId
@@ -537,15 +541,15 @@
                     result[item] = amend[item]
                 else:
                     result[item] = self._merge_list(orig[item], amend[item])
             else:
                 result[item] = amend[item]
         return result
 
-    def delete(self, oid: str | ObjectId, collection: str,
+    def delete(self, oid: Union[str, ObjectId], collection: str,
                structure: str) -> bool:
         """
         | ドキュメントを削除する
         | 指定のoidを含む下位のドキュメントを全削除
         | refで親が存在する時は親のchildリストから指定のoidを取り除く
 
         :param oid:
@@ -596,15 +600,15 @@
         """
         指定のドキュメント以下の子ドキュメントと関連ファイルを削除する
 
         :param dict db_result:
         :param str collection:
         :return:
         """
-        delete_doc_id_dict: dict[str, list[ObjectId]] = {}
+        delete_doc_id_dict = {}
         delete_file_ref_list = []
         for element in self._recursive_extract_elements_from_doc(db_result,
                                                                  collection):
             doc_collection = list(element.keys())[0]
             id_and_refs = list(element.values())[0]
 
             for oid, refs in id_and_refs.items():
@@ -645,26 +649,27 @@
 
         :param DBRef ref:
         :param ObjectId del_oid:
         :return:
         """
         parent_doc = self.db[ref.collection].find_one({'_id': ref.id})
         children = parent_doc[self.child]
+
         target = None
         for child in children:
             if child.id == del_oid:
                 target = child
                 break
         if target is None:
             raise ValueError(
                 f'親となる{parent_doc["id"]}に{str(del_oid)}が登録されていません')
         else:
             children.remove(target)
 
-            # 子要素が登録されていればself.childを更新
+            # 他に子要素が登録されていればself.childを更新
             if len(children) > 0:
                 result = self.db[ref.collection].update_one(
                     {'_id': ref.id},
                     {'$set': {self.child: children}})
             # 他に子要素がなければself.child自体を削除
             else:
                 del parent_doc[self.child]
@@ -679,50 +684,57 @@
         コレクション別の、oidとファイルリファレンスリストを取り出す
 
         :param dict doc:
         :param str collection:
         :return:
         :rtype: dict
         """
-        return {collection: {
-            doc['_id']: {self.file_ref: doc.get(self.file_ref, {})}}}
+        file_ref_buff = {}
+        if doc.get(self.file_ref) is not None:
+            file_ref_buff = {self.file_ref: doc[self.file_ref]}
+
+        return {collection: {doc['_id']: file_ref_buff}}
 
     def _recursive_extract_elements_from_doc(self, doc: dict,
-                                             collection: str) -> Generator:
+                                             collection: str) -> dict:
         """
         再帰処理で
         コレクション別の、oidとファイルリファレンスの辞書を取り出すジェネレータ
 
         :param dict doc:
         :param str collection:
         :return:
-        :rtype: Generator
+        :rtype: dict
         """
         yield self._extract_elements_from_doc(doc, collection)
+
         if doc.get(self.child):
             for child_ref in doc[self.child]:
                 yield from self._recursive_extract_elements_from_doc(
                     self.db.dereference(child_ref), child_ref.collection)
 
-    def _collect_emb_file_ref(self, doc: dict, request_key: str) -> Generator:
+    def _collect_emb_file_ref(self, doc: dict, request_key: str) -> list:
         """
         emb構造のデータからファイルリファレンスのリストだけを取り出すジェネレータ
 
         :param dict doc:
         :param str request_key:
         :return: value
-        :rtype: Generator
+        :rtype: list
         """
+
         for key, value in doc.items():
             if isinstance(value, dict):
                 yield from self._collect_emb_file_ref(value, request_key)
+
             elif isinstance(value, list) and Utils.item_literal_check(value):
                 if key == request_key:
                     yield value
                 continue
+
             elif isinstance(value, list):
                 if key == request_key:
                     yield value
                 else:
                     for i in value:
                         yield from self._collect_emb_file_ref(i, request_key)
             else:
@@ -745,25 +757,25 @@
 
     def get_structure(self, collection: str, oid: ObjectId) -> str:
         """
         対象のドキュメントの構造を取得する
 
         :param str collection:
         :param ObjectId oid:
-        :return: result
+        :return: ref or emb
         :rtype: str
         """
         doc = self.db[collection].find_one({'_id': Utils.conv_objectid(oid)})
         if doc is None:
             raise EdmanInternalError('該当するドキュメントは存在しません')
+
         if any(key in doc for key in (self.parent, self.child)):
-            result = 'ref'
+            return 'ref'
         else:
-            result = 'emb'
-        return result
+            return 'emb'
 
     def structure(self, collection: str, oid: ObjectId,
                   structure_mode: str, new_collection: str) -> list:
         """
         構造をrefからembへ、またはembからrefへ変更する
 
         :param str collection:
@@ -771,22 +783,22 @@
         :param str structure_mode:
         :param str new_collection:
         :return: structured_result
         :rtype: list
         """
         oid = Utils.conv_objectid(oid)
 
-        convert = Convert()
         # refデータをembに変換する
         if structure_mode == 'emb':
             # 自分データ取り出し
             ref_result = self.doc(collection, oid, query=None,
                                   reference_delete=False)
             if ref_result is None:
                 raise EdmanInternalError("ドキュメントが存在しません")
+
             reference_point_result = self.get_reference_point(
                 ref_result)
             if reference_point_result[self.child]:
                 # 子データを取り出し
                 children = self.get_child_all({collection: ref_result})
 
                 # 自分のリファレンスデータとidを削除
@@ -797,31 +809,34 @@
                 # 子のリファレンスデータ削除
                 non_ref_children = self.delete_reference(children,
                                                          ('_id', self.parent,
                                                           self.child))
                 # 自分と子要素をマージする
                 ref_result.update(non_ref_children)
 
+                convert = Convert()
                 converted_edman = convert.dict_to_edman(
                     {new_collection: ref_result}, mode='emb')
                 structured_result = self.insert(converted_edman)
             # 子が存在しないドキュメントの場合(新たなコレクションとして切り出す)
             else:
                 # 自分のリファレンスデータとidを削除
                 for del_key in (self.parent, '_id'):
                     if del_key in ref_result:
                         del ref_result[del_key]
+                convert = Convert()
                 converted_edman = convert.dict_to_edman(
                     {new_collection: ref_result}, mode='emb')
                 structured_result = self.insert(converted_edman)
 
         # embからrefに変換
         elif structure_mode == 'ref':
             emb_result = self.db[collection].find_one({'_id': oid})
             del emb_result['_id']
+            convert = Convert()
             converted_edman = convert.dict_to_edman(
                 {new_collection: emb_result}, mode='ref')
             structured_result = self.insert(converted_edman)
             structured_result.reverse()
 
         else:
             raise EdmanFormatError('structureはrefまたはembの指定が必要です')
@@ -842,15 +857,15 @@
             for doc in doc_list:
                 if tmp := self._child_storaged(doc):
                     result.append(tmp)
                 # 子データがある時は繰り返す
                 if tmp:
                     recursive(tmp)
 
-        result: list = []  # recによって書き換えられる
+        result = []  # recによって書き換えられる
         recursive([self_doc])  # 再帰関数をシンプルにするため、初期データをリストで囲む
         return self._build_to_doc_child(result)  # 親子構造に組み立て
 
     def get_child(self, self_doc: dict, depth: int) -> dict:
         """
         | 子のドキュメントを取得
         |
@@ -889,21 +904,22 @@
         |
         | 同じコレクションの場合は子データをリストで囲む
 
         :param dict doc:
         :return: children
         :rtype: list
         """
+        doc = list(doc.values())[0]
         children = []
         # 単純にリスト内に辞書データを入れたい場合
-        doc = list(doc.values())[0]
         if self.child in doc:
             children = [
                 {child_ref.collection: self.db.dereference(child_ref)}
                 for child_ref in doc[self.child]]
+
         return children
 
     def _build_to_doc_child(self, find_result: list) -> dict:
         """
         子の検索結果（リスト）を入れ子辞書に組み立てる
 
         :param list find_result:
@@ -1021,21 +1037,22 @@
         if self.db[collection].estimated_document_count() == 0:
             raise EdmanInternalError('該当するドキュメントは存在しません')
 
         id_list = [doc['_id'] for doc in self.db[collection].find() if
                    self.get_structure(collection, doc['_id']) == 'emb']
 
         result_list = []
-        convert = Convert()
         for oid in id_list:
             emb_result = self.db[collection].find_one({'_id': oid})
             del emb_result['_id']
+            convert = Convert()
             pull_result = convert.pullout_key(emb_result, key)
             if not pull_result:
                 raise EdmanInternalError(f'{key}は存在しません')
+
             if exclusion:
                 result = convert.exclusion_key(pull_result, exclusion)
                 if pull_result == result:
                     raise EdmanInternalError(f'{list(exclusion)}は存在しません')
             else:
                 result = pull_result
 
@@ -1058,14 +1075,15 @@
                        self.db.list_collection_names(filter=coll_filter)]
         if gf_filter:
             result = list(
                 set(collections) - {Config.fs_files, Config.fs_chunks})
         else:
             result = collections
         result.sort()
+
         return result
 
     @staticmethod
     def pack_list(types: list, target: list) -> list:
         """
         typesが少ない時に、最後の値で足りない分を埋める
         例
@@ -1118,15 +1136,15 @@
         |   型一覧:
         |   [int,float,bool,str,datetime]
 
         :param dict bson_data:
         :return: result
         :rtype: dict
         """
-        result: dict[str, Any] = {}
+        result = {}
 
         for collection, items in bson_data.items():
 
             # フィルタ、プロジェクション作成
             items_keys = list(items.keys())
             projection = {k: 1 for k in items_keys}
             reference = {'$or': [
@@ -1220,15 +1238,15 @@
             else:
                 # 親要素はツリーを遡っていくだけ
                 result = 1
                 result += self.get_ref_depth(
                     self.db.dereference(doc[reference_key]), reference_key)
         return result
 
-    def get_root_dbref(self, doc: dict) -> None | DBRef:
+    def get_root_dbref(self, doc: dict) -> Union[None, DBRef]:
         """
         ref形式のドキュメントのルートのDBRef要素を取得する
         ※root要素内にはparentのdbref要素は存在しないので、上から2階層目のparentのdbrefを取得する
         :param dict doc:
         :return: parent_ref
         :rtype: None or DBRef
         """
```

### Comparing `edman-2023.5.23/edman/exceptions.py` & `edman-2023.5.8/edman/exceptions.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.23/edman/file.py` & `edman-2023.5.8/edman/file.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import shutil
 import copy
-import json
-from tempfile import TemporaryDirectory
+import gzip
+from tempfile import TemporaryDirectory, NamedTemporaryFile
 import datetime
 import zipfile
-from typing import Tuple, Iterator, List, Any, IO
+from typing import Union, Tuple, Iterator, List, Any
 from pathlib import Path
 import gridfs
 from gridfs.errors import NoFile, GridFSError
 import jmespath
 from bson import ObjectId
 from edman.utils import Utils
 from edman.exceptions import (EdmanFormatError, EdmanDbProcessError,
@@ -25,15 +25,14 @@
     def __init__(self, db=None) -> None:
 
         if db is not None:
             self.db = db
             self.fs = gridfs.GridFS(self.db)
         self.file_ref = Config.file
         self.comp_level = Config.gzip_compress_level
-        self.file_attachment = Config.file_attachment
 
     @staticmethod
     def file_gen(files: Tuple[Path]) -> Iterator:
         """
         ファイルタプルからファイルを取り出すジェネレータ
 
         :param tuple files: 中身はPathオブジェクト
@@ -45,54 +44,60 @@
                 with file.open('rb') as f:
                     fp = f.read()
             except IOError:
                 raise
             yield file.name, fp
 
     def delete(self, delete_oid: ObjectId, collection: str,
-               oid: ObjectId | str, structure: str, query=None) -> bool:
+               oid: Union[ObjectId, str], structure: str, query=None) -> bool:
         """
         該当のoidをファイルリファレンスから削除し、GridFSからファイルを削除
 
         :param ObjectId delete_oid:
         :param str collection:
         :param str oid:
         :param str structure:
         :param query:
         :type query: list or None
         :return:
         :rtype: bool
         """
         oid = Utils.conv_objectid(oid)
-        if structure not in ['ref', 'emb']:
-            raise EdmanFormatError('structureはrefまたはembの指定が必要です')
 
         # ドキュメント存在確認&コレクション存在確認&対象ドキュメント取得
-        if (doc := self.db[collection].find_one({'_id': oid})) is None:
+        doc = self.db[collection].find_one({'_id': oid})
+        if doc is None:
             raise EdmanInternalError('対象のコレクション、またはドキュメントが存在しません')
 
         # ファイルリスト取得
         files_list = self.get_file_ref(doc, structure, query)
-        if len(files_list) == 0:
-            raise EdmanDbProcessError('ファイルが存在しません')
 
         # リファレンスデータを編集
-        # 何らかの原因で重複があった場合を避けるため一度setにする
-        files_list = list(set(files_list))
-        files_list.remove(delete_oid)
+        if len(files_list) > 0:
+            # 何らかの原因で重複があった場合を避けるため一度setにする
+            files_list = list(set(files_list))
+            files_list.remove(delete_oid)
+        else:
+            raise EdmanDbProcessError('ファイルが存在しません')
 
         # ドキュメントを新しいファイルリファレンスに置き換える
-        try:
-            if structure == 'ref':
+        if structure == 'ref':
+            try:
                 new_doc = self.file_list_replace(doc, files_list)
-            else:
+            except Exception:
+                raise
+        elif structure == 'emb':
+            try:
                 new_doc = Utils.doc_traverse(doc, files_list, query,
                                              self.file_list_replace)
-        except Exception:
-            raise
+            except Exception:
+                raise
+        else:
+            raise EdmanFormatError('structureはrefまたはembの指定が必要です')
+
         replace_result = self.db[collection].replace_one({'_id': oid}, new_doc)
         # fsから該当ファイルを削除
         if replace_result.modified_count:
             self.fs_delete([delete_oid])
 
         # ファイルが削除されればOK
         return False if self.fs.exists(delete_oid) else True
@@ -135,15 +140,15 @@
             try:
                 files_list = self._get_emb_files_list(doc, query_c)
             except Exception:
                 raise
 
         return files_list
 
-    def get_file_names(self, collection: str, oid: ObjectId | str,
+    def get_file_names(self, collection: str, oid: Union[ObjectId, str],
                        structure: str, query=None) -> dict:
         """
         ファイル一覧を取得
         ファイルが存在しなければ空の辞書を返す
 
         :param str collection:
         :param str oid:
@@ -167,31 +172,34 @@
                 fs_out = self.fs.get(file_oid)
             except gridfs.errors.NoFile:
                 continue
             else:
                 result.update({file_oid: fs_out.filename})
         return result
 
-    def download(self, file_oid: list[ObjectId], path: str | Path) -> bool:
+    def download(self, file_oid: list[ObjectId],
+                 path: Union[str, Path]) -> bool:
         """
         Gridfsからデータをダウンロードし、ファイルに保存
+        metadataに圧縮指定があれば伸長する
 
         :param list file_oid:
         :param path:
         :type path: str or Path
         :return: result
         :rtype: bool
         """
         # 定型的な前処理があればここに追加する
         return self._grid_out(file_oid, path)
 
     def _grid_out(self, file_oid_list: List[ObjectId],
-                  path: str | Path) -> bool:
+                  path: Union[str, Path]) -> bool:
         """
         Gridfsからデータを取得し、ファイルに保存
+        metadataに圧縮指定があれば伸長する
         複数のファイルを指定すると、複数のファイルが作成される
 
         :param list file_oid_list:
         :param path:
         :type path: str or Path
         :return: result
         :rtype: bool
@@ -202,96 +210,105 @@
 
         # パスが正しいか検証
         if not p.exists():
             raise FileNotFoundError
         # ファイルが存在するか検証
         if False in map(self.fs.exists, file_oid_list):
             raise EdmanDbProcessError('指定のファイルはDBに存在しません')
-
-        # ダウンロード処理
-        results = []
-        for file_oid in file_oid_list:
-            fs_out = self.fs.get(file_oid)
-            save_path = p / fs_out.filename
-            try:
-                with save_path.open('wb') as f:
-                    tmp = fs_out.read()
-                    f.write(tmp)
-                    f.flush()
-                    os.fsync(f.fileno())
-            except IOError:
-                raise
-            results.append(save_path.exists())
-
+        else:
+            # ダウンロード処理
+            results = []
+            for file_oid in file_oid_list:
+                fs_out = self.fs.get(file_oid)
+                save_path = p / fs_out.filename
+                try:
+                    with save_path.open('wb') as f:
+                        tmp = fs_out.read()
+                        if hasattr(fs_out,
+                                   'compress') and fs_out.compress == 'gzip':
+                            tmp = gzip.decompress(tmp)
+                        f.write(tmp)
+                        f.flush()
+                        os.fsync(f.fileno())
+                except IOError:
+                    raise
+                results.append(save_path.exists())
         return all(results)
 
-    def upload(self, collection: str, oid: ObjectId | str,
+    def upload(self, collection: str, oid: Union[ObjectId, str],
                file_path: Tuple[Tuple[Any, bool]], structure: str,
                query=None) -> bool:
         """
         ドキュメントにファイルリファレンスを追加する
-        ファイルのインサート処理なども行う
+        ファイルのインサート処理、圧縮処理なども行う
         :param str collection:
         :param oid:
         :type oid: ObjectId or str
-        :param tuple file_path:ドキュメントに添付する単数or複数のファイルパス
+        :param tuple file_path:ドキュメントに添付する単数or複数のファイルパスと圧縮可否のタプル
         :param str structure:
         :param query:
         :type query: list or None
         :return:
         :rtype: bool
         """
+
         oid = Utils.conv_objectid(oid)
-        if structure not in ['ref', 'emb']:
-            raise EdmanFormatError('構造はrefかembが必要です')
 
         # ドキュメント存在確認&対象ドキュメント取得
         doc = self.db[collection].find_one({'_id': oid})
         if doc is None:
             raise EdmanInternalError('対象のドキュメントが存在しません')
         if structure == 'emb':
             # クエリーがドキュメントのキーとして存在するかチェック
             if not Utils.query_check(query, doc):
                 raise EdmanFormatError('対象のドキュメントに対してクエリーが一致しません.')
 
         # ファイルのインサート
         inserted_file_oids = self.grid_in(file_path)
         if structure == 'ref':
             new_doc = self.file_list_attachment(doc, inserted_file_oids)
-        else:
+        elif structure == 'emb':
             try:
                 new_doc = Utils.doc_traverse(doc, inserted_file_oids, query,
                                              self.file_list_attachment)
             except Exception:
                 raise
+        else:
+            raise EdmanFormatError('構造はrefかembが必要です')
 
         # ドキュメント差し替え
         replace_result = self.db[collection].replace_one({'_id': oid}, new_doc)
+
         if replace_result.modified_count == 1:
-            result = True
+            return True
         else:  # 差し替えができなかった時は添付ファイルは削除
             self.fs_delete(inserted_file_oids)
-            result = False
+            return False
 
-        return result
-
-    def grid_in(self, files: Tuple[Tuple[Path, bool], ...]) -> list[ObjectId]:
+    def grid_in(self, files: Tuple[Tuple[Any, bool]]) -> list[Any]:
         """
-        Gridfsへ複数のデータをアップロード
+        Gridfsへ複数のデータをアップロードし
+        compressに圧縮指定があればgzipで圧縮する
 
         :param tuple files:
         :return: inserted
         :rtype: list
         """
         inserted = []
         for file, compress in files:
             try:
                 with file.open('rb') as f:
                     fb = f.read()
-                    metadata = {'filename': os.path.basename(f.name)}
+                    if compress:
+                        fb = gzip.compress(fb, compresslevel=self.comp_level)
+                        compress = 'gzip'
+                    else:
+                        compress = None
+                    metadata = {'filename': os.path.basename(f.name),
+                                'compress': compress}
             except (IOError, OSError) as e:
                 raise EdmanDbProcessError(e)
             try:
                 inserted.append(self.fs.put(fb, **metadata))
             except GridFSError as e:
                 raise EdmanDbProcessError(e)
         return inserted
@@ -365,95 +382,110 @@
         now = datetime.datetime.now()
         name = now.strftime('%Y%m%d%H%M%S')
         if filename is not None:
             name = name + str(filename)
         return name + '.zip'
 
     def zipped_contents(self, downloads: dict, json_tree_file_name: str,
-                        encoded_json: bytes, p: Path) -> str:
+                        encoded_json: bytes) -> str:
         """
         jsonと添付ファイルを含むzipファイルを生成
         zipファイル内部にjson_tree_file_name.jsonのjsonファイルを含む
         添付ファイルがなく、jsonファイルだけ取得したい場合はzipped_jsonを利用
 
         :param dict downloads:
         :param str json_tree_file_name:
         :param bytes encoded_json:
-        :param Path p:
         :rtype: str
         :return:
         """
-        work = p
-        p = work / 'archives'
-        p.mkdir()
-        for file_refs, dir_path in zip([i for i in downloads.values()],
-                                       [p / str(doc_oid) for doc_oid in
-                                        downloads]):
-            os.mkdir(dir_path)
-            for file_ref in file_refs:
-                # 添付ファイルをダウンロード
-                try:
-                    content = self.fs.get(file_ref)
-                except NoFile:
-                    raise EdmanDbProcessError('指定の関連ファイルが存在しません')
-                except GridFSError:
-                    raise
 
-                # 添付ファイルを保存
-                filepath = dir_path / content.name
-                try:
-                    with open(filepath, 'wb') as f:
-                        f.write(content.read())
-                except (FileNotFoundError, IOError):
-                    EdmanInternalError('ファイルを保存することが出来ませんでした')
-
-            # jsonファイルを保存
-            json_file = json_tree_file_name + '.json'
-            json_path = p / json_file
+        zip_suffix = '.zip'
+        json_suffix = '.json'
+
+        with TemporaryDirectory() as tmpdir:
+            dir_path_list = [os.path.join(tmpdir, str(doc_oid)) for
+                             doc_oid in downloads]
+
+            for dir_path in dir_path_list:
+                os.mkdir(dir_path)
+
+            for file_refs, dir_path in zip([i for i in downloads.values()],
+                                           dir_path_list):
+                for file_ref in file_refs:
+                    try:
+                        content = self.fs.get(file_ref)
+                    except NoFile:
+                        raise EdmanDbProcessError('指定の関連ファイルが存在しません')
+                    except GridFSError:
+                        raise
+                    else:
+                        # 圧縮設定の場合はその拡張子を追加
+                        if content.compress is not None:
+                            filename = content.name + '.' + content.compress
+                        else:
+                            filename = content.name
+                        filepath = os.path.join(dir_path, filename)
+                    try:
+                        with open(filepath, 'wb') as f:
+                            f.write(content.read())
+                    except (FileNotFoundError, IOError):
+                        EdmanInternalError('ファイルを保存することが出来ませんでした')
+                    except GridFSError:
+                        raise
             try:
-                with json_path.open('wb') as f:
+                # jsonファイルとして一時ディレクトリに保存
+                with open(os.path.join(tmpdir,
+                                       json_tree_file_name + json_suffix),
+                          'wb') as f:
                     f.write(encoded_json)
             except (FileNotFoundError, IOError):
                 EdmanInternalError('ファイルを保存することが出来ませんでした')
-
-        # 最終的にDLするzipファイルを作成
-        base = work / 'dl'
-        try:
-            zip_filepath = shutil.make_archive(str(base), format='zip',
-                                               root_dir=str(p))
-        except Exception:
-            raise
+            try:
+                # 最終的にDLするzipファイルを作成
+                with NamedTemporaryFile() as fp:
+                    zip_filepath = shutil.make_archive(fp.name, zip_suffix[1:],
+                                                       tmpdir)
+            except Exception:
+                raise
         return zip_filepath
 
     @staticmethod
-    def zipped_json(encoded_json: bytes, json_tree_file_name: str,
-                    p: Path) -> Path:
+    def zipped_json(encoded_json: bytes, json_tree_file_name: str) -> str:
         """
+        jsonファイルとzipファイルを名前付きテンポラリとして生成し、パスを生成
         zipファイル内部にjson_tree_file_name.jsonのjsonファイルを含む
         添付ファイルがなく、jsonファイルだけ取得したい場合に使用する
+        # リファクタリング対象
 
         :param bytes encoded_json: json文字列としてダンプしたものを指定の文字コードでバイト列に変換したもの
         :param str json_tree_file_name: zipファイル内に配置するjsonファイルの名前
-        :param Path p: ファイルを保存するディレクトリのパス
-        :return:zip_filepath
-        :rtype:Path
-        """
-        zip_filename = json_tree_file_name + '.zip'
-        filename = json_tree_file_name + '.json'
-        jsonfile = p / filename
-        zip_filepath = p / zip_filename
+        :return:
+        :rtype:str
+        """
 
+        json_suffix = '.json'
+        zip_suffix = '.zip'
         try:
-            with jsonfile.open('wb') as f:
-                f.write(encoded_json)
+            # jsonファイルとして一時ファイルに保存
+            with NamedTemporaryFile(suffix=json_suffix,
+                                    delete=False) as fp:
+                filepath = fp.name
+                fp.write(encoded_json)
         except Exception:
             raise
         try:
-            with zipfile.ZipFile(zip_filepath, 'w', zipfile.ZIP_DEFLATED) as f:
-                f.write(jsonfile, arcname=filename)
+            # jsonファイルをzipで圧縮して一時ファイルに保存
+            with NamedTemporaryFile(suffix=zip_suffix,
+                                    delete=False) as fp:
+                with zipfile.ZipFile(fp.name, 'w',
+                                     zipfile.ZIP_DEFLATED) as archive:
+                    zip_filepath = fp.name
+                    archive.write(filepath,
+                                  arcname=json_tree_file_name + json_suffix)
         except Exception:
             raise
         return zip_filepath
 
     def get_fileref_and_generate_dl_list(self, docs: dict,
                                          attach_key: str) -> tuple[dict, dict]:
         """
@@ -506,124 +538,7 @@
                                data[key]]})
                 else:
                     c_docs.update({key: value})
             return c_docs
 
         new_docs = recursive(docs)
         return new_docs, dl_list
-
-    def upload_zipped(self, zip_file: IO) -> dict | None:
-        """
-        zipファイルを解凍し、ファイルをgridfsに格納、結果のoidを含めたjsonを返す
-
-        :param IO zip_file: アップロードされたzipファイル
-        :return:
-        :rtype: dict
-        """
-        entry_json = None
-
-        with TemporaryDirectory() as td:
-            p = Path(td)
-            with zipfile.ZipFile(zip_file) as ex_zip:
-                ex_zip.extractall(td)
-
-            json_list = list(p.glob('*.json'))
-            if not json_list:
-                raise EdmanInternalError('jsonファイルが存在しません')
-            if len(json_list) > 1:
-                raise EdmanInternalError('jsonファイルは一つだけしか含めることはできません')
-            target_json = json_list[0]
-            # jsonデータ取り出し
-            with target_json.open() as f:
-                json_data = json.load(f)
-            try:
-                # 添付ファイルを取り出す
-                files_list = self.generate_upload_list(json_data)
-                # 解凍したデータ内に、実際にデータが存在するか照合する(ダウンロードするパスを接合する)
-                path_list = self.generate_file_path_dict(files_list, p)
-                # gridfsにファイルを格納するために専用のタプルを作成
-                paths = tuple([(v, False) for v in path_list.values()])
-                # grid.fsに入れる
-                grid_in_results = self.grid_in(paths)
-                # grid_inはinserted_idしか返さないため、jsonのファイルパスをキーとしてinserted_oidをバリューとする辞書を作成する
-                gf_inserted_dict = {i: j for i, j in
-                                    zip(path_list, grid_in_results)}
-            except Exception:
-                raise
-            else:
-                # jsonデータにoidを書き加え、添付ファイル用キーを削除
-                entry_json = self.json_rewrite(json_data, gf_inserted_dict)
-
-        return entry_json
-
-    def generate_upload_list(self, data: dict) -> list[str]:
-        """
-        json辞書からキーfiles_dir_keyの値であるリストを抽出し、新しいリストにする
-
-        :param dict data:
-        :return: result
-        :rtype: list
-        """
-        result = []
-        for key, value in data.items():
-            if isinstance(value, dict):
-                result.extend(self.generate_upload_list(value))
-            elif isinstance(value, list):
-                # ファイル添付のキーをフック
-                if key == self.file_attachment:
-                    result.extend(value)
-                else:
-                    for i in value:
-                        result.extend(self.generate_upload_list(i))
-            else:
-                continue
-        return result
-
-    def json_rewrite(self, data: dict, files_dict: dict) -> dict:
-        """
-        元のjsonのファイルパスをinsert済みのファイルのoidに書き換える
-
-        :param dict data:
-        :param dict files_dict:
-        :return:
-        :rtype: dict
-        """
-        result = {}
-        for key, value in data.items():
-            if isinstance(value, dict):
-                result.update(
-                    {key: self.json_rewrite(value, files_dict)})
-            elif isinstance(value, list):
-                if key == self.file_attachment:
-                    buff = []
-                    for filepath in value:
-                        if files_dict.get(filepath) is not None:
-                            buff.append(files_dict[filepath])
-                    result.update({self.file_ref: buff})
-                else:
-                    result.update({
-                        key: [self.json_rewrite(i, files_dict)
-                              for i in value]})
-            else:
-                result.update({key: value})
-        return result
-
-    @staticmethod
-    def generate_file_path_dict(files_list: list, p: Path) -> dict[str, Path]:
-        """
-        files_listから添付ファイルの存在確認をし、添付ファイルのファイルパスを値とする辞書を作成
-
-        :param list files_list:
-        :param Path p:
-        :return: result
-        :rtype: dict
-        """
-        result = {}
-        for json_file_path in files_list:
-            p1 = Path(json_file_path)
-            j = p / p1
-            if j.exists():
-                result.update({json_file_path: j})
-            else:
-                raise EdmanInternalError(
-                    'JSON内のパスとファイル配置に違いがありましたので中止します')
-        return result
```

### Comparing `edman-2023.5.23/edman/json_manager.py` & `edman-2023.5.8/edman/json_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import os
 from datetime import datetime
 from pathlib import Path
 from enum import Enum, auto
+from typing import Union
 from bson.json_util import dumps
 from edman.exceptions import EdmanFormatError
 
 
 class JsonManager:
     """
     JSONファイルの取扱いクラス
     """
 
     @staticmethod
-    def save(report_data: dict, path: str| Path, name: str,
+    def save(report_data: dict, path: Union[str, Path], name: str,
              date=False) -> None:
         """
         JSONファイルに書き出し
 
         :param dict report_data: 対象の辞書データ
         :param path: ファイルパス
         :type path: str or Path
```

### Comparing `edman-2023.5.23/edman/search.py` & `edman-2023.5.8/edman/search.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from datetime import datetime
+from typing import Union
 from pymongo import errors
-from bson import errors as bson_errors, ObjectId
+from bson import errors, ObjectId
 from edman.utils import Utils
 from edman.exceptions import EdmanDbProcessError
 from edman import Config
 
 
 class Search:
     """
@@ -113,19 +114,19 @@
         :param dict query:
         :return: query
         :rtype: dict
         """
         if '_id' in query:
             try:
                 query['_id'] = ObjectId(query['_id'])
-            except bson_errors.InvalidId:
+            except errors.InvalidId:
                 raise
         return query
 
-    def _get_self(self, query: dict, collection: str) -> dict | None:
+    def _get_self(self, query: dict, collection: str) -> Union[dict, None]:
         """
         自分自身のドキュメント取得
 
         :param dict query:
         :param str collection:
         :return:
         :rtype: dict or None
@@ -136,15 +137,15 @@
         except errors.OperationFailure:
             raise EdmanDbProcessError('ドキュメントが取得できませんでした')
         else:
             if len(docs):
                 result = {collection: docs[0]}
         return result
 
-    def _get_parent(self, self_doc: dict, depth: int) -> dict | None:
+    def _get_parent(self, self_doc: dict, depth: int) -> Union[dict, None]:
         """
         | 親となるドキュメントを取得
         | depthで深度を設定し、階層分取得する
 
         :param dict self_doc:
         :param int depth:
         :return: result
@@ -155,39 +156,39 @@
             """
             再帰でドキュメントを取得
             DBReferenceを利用し、設定されている深度を減らしながら再帰
             """
             if self.parent in doc:
                 parent = self.connected_db.dereference(doc[self.parent])
                 parent_collection = doc[self.parent].collection
-                data.append({parent_collection: parent})
+                result.append({parent_collection: parent})
                 nonlocal depth
                 depth -= 1
                 if depth > 0:
                     recursive(parent)
 
         if depth > 0:
-            data: list = []  # recによって書き換えられる
+            result = []  # recによって書き換えられる
             recursive(list(self_doc.values())[0])
-            result = self._build_to_doc_parent(data)
+            result = self._build_to_doc_parent(result)
         else:
             result = None
         return result
 
     @staticmethod
-    def _build_to_doc_parent(parent_data_list: list) -> dict | None:
+    def _build_to_doc_parent(parent_data_list: list) -> dict:
         """
         | 親の検索結果（リスト）を入れ子辞書に組み立てる
         |
         | 入力値であるparent_data_listについて、
         | parentに近い方から順番に並んでいる(一番最後がrootまたはrootに近い方)
 
         :param list parent_data_list:
         :return: result
-        :rtype: dict or None
+        :rtype: dict
         """
         result = None
         for read_data in parent_data_list:
             if result is not None:
                 buff = read_data
                 collection = list(buff.keys())[0]
                 doc = list(buff.values())[0]
@@ -229,33 +230,36 @@
             # idとrefの削除
             for key, val in data.items():
                 if isinstance(data[key], dict):
                     recursive(Utils.item_delete(data[key], refs))
                 # リストデータは中身を型変換する
                 elif isinstance(data[key], list) and Utils.item_literal_check(
                         data[key]):
-                    data[key] = [self._format_datetime(j)
-                                 if isinstance(j, datetime) else j
-                                 for j in data[key]]
+                    data[key] = [self._format_datetime(j) for j in data[key]]
                 elif isinstance(data[key], list):
                     for item in data[key]:
                         recursive(Utils.item_delete(item, refs))
                 else:
                     try:  # 型変換
-                        if isinstance(data[key], datetime):
-                            data[key] = self._format_datetime(data[key])
+                        data[key] = self._format_datetime(data[key])
                     except Exception:
                         raise
 
         recursive(result_dict)
         return result_dict
 
-    def _format_datetime(self, item: datetime) -> dict[str, str]:
+    def _format_datetime(self, item: Union[str, int, float, bool, datetime]
+                         ) -> Union[dict, str, int, float, bool, datetime]:
         """
         datetime型なら書式変更して辞書に入れる
+        その場合は辞書を返し、それ以外の時は入ってきた値をそのまま返す
 
         :param item:
-        :type item: datetime
+        :type item: str or int or float or bool or datetime
         :return: result
-        :rtype: dict
+        :rtype: dict or str or int or float or bool or datetime
         """
-        return {self.date: item.strftime("%Y-%m-%d %H:%M:%S")}
+        # datetimeそのままだと%Y-%m-%dと%H:%M:%Sの間に"T"が入るため書式変更
+        result = item
+        if isinstance(item, datetime):
+            result = {self.date: item.strftime("%Y-%m-%d %H:%M:%S")}
+        return result
```

### Comparing `edman-2023.5.23/edman/utils.py` & `edman-2023.5.8/edman/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 from collections import defaultdict
-from typing import Union, Callable, Generator
+from typing import Union, Callable
 from datetime import datetime
 import dateutil.parser
 from bson import ObjectId, errors
 
 
 class Utils:
     """
@@ -12,15 +12,15 @@
     | インスタンス化禁止
     """
 
     def __init__(self):
         raise NotImplementedError('not allowed')
 
     @staticmethod
-    def item_literal_check(list_child: dict | list) -> bool:
+    def item_literal_check(list_child: Union[dict, list]) -> bool:
         """
         | リストデータ内にリテラルやオブジェクトのデータだけあればTrue
         | それ以外はFalse
         |
         | OKパターン
         | list_child = [1,2,3]
         | list_child = [1,2,objectId()]
@@ -127,15 +127,15 @@
             raise e
         if len(query) != 0:
             raise ValueError(f'クエリが実行されませんでした. 実行されなかったクエリ:{query}')
 
         return doc
 
     @staticmethod
-    def conv_objectid(oid: str | ObjectId) -> ObjectId:
+    def conv_objectid(oid: Union[str, ObjectId]) -> ObjectId:
         """
         | 文字列だった場合ObjectIdを変換する
         | 元々ObjectIdならそのまま
 
         :param oid:
         :type oid: ObjectId or str
         :return: result
@@ -148,15 +148,15 @@
             except errors.InvalidId:
                 raise
         else:
             result = oid
         return result
 
     @staticmethod
-    def to_datetime(s: str) -> datetime | str:
+    def to_datetime(s: str) -> Union[datetime, str]:
         """
         | 日付もしくは日付時間をdatetimeオブジェクトに変換
         | 日付や日付時間にならないものは文字列に変換
 
         :param str s:
         :return:
         :rtype: datetime or str
@@ -204,24 +204,24 @@
         :rtype: dict
         """
         for key in (i for i in del_keys if i in doc):
             del doc[key]
         return doc
 
     @staticmethod
-    def child_combine(rec_result: list) -> Generator:
+    def child_combine(rec_result: list) -> dict:
         """
         | 同じコレクションのデータをリストでまとめるジェネレータ
         |
         | コレクション:ドキュメントのリストを作成
         | {collection:[{key:value},{key:value}...]}
 
         :param list rec_result:
         :return:
-        :rtype: Generator
+        :rtype: dict
         """
         for bros in rec_result:
             tmp_bros = defaultdict(list)
 
             for docs in bros:
                 for collection, doc in docs.items():
                     tmp_bros[collection].append(doc)
@@ -293,31 +293,31 @@
         # 先頭に記号があるとマッチする
         if re.match(r'(\W)', collection_name) is not None:
             return False
 
         return True
 
     @staticmethod
-    def type_cast_conv(datatype: str) -> object | Callable:
+    def type_cast_conv(datatype: str) -> Union[bool, int, float, str,
+    dateutil.parser.parse]:
         """
         データタイプに合わせて型を選択する
 
-        :param str datatype:
+        :param int datatype:
         :return:
-        :rtype: object or callable
+        :rtype: bool or int or float or str or dateutil.parser.parse
         """
         type_table = {
             'bool': bool,
             'int': int,
             'float': float,
             'str': str,
             'datetime': dateutil.parser.parse
         }
-        result = type_table.get(datatype, str)
-        return result
+        return type_table.get(datatype, str)
 
     @staticmethod
     def generate_jms_query(query):
         s = ''
         for idx, i in enumerate(query):
             if i.isdecimal():
                 s += '[' + i + ']'
```

### Comparing `edman-2023.5.23/edman.egg-info/PKG-INFO` & `edman-2023.5.8/edman.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,19 @@
 Metadata-Version: 2.1
 Name: edman
-Version: 2023.5.23
+Version: 2023.5.8
 Summary: KEK IMSS SBRC/PF Experimental Data Management System
-Author-email: Masaki Ohno <masakio@post.kek.jp>
+Home-page: https://github.com/ryde/edman
+Author: Masaki Ohno
+Author-email: masakio@post.kek.jp
 License: MIT License
-        
-        Copyright (c) 2019-2023 KEK IMSS SBRC/PF, Yusuke Yamada, Masaki Ohno
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-        
-Project-URL: documentation, https://ryde.github.io/edman/
-Project-URL: repository, https://github.com/ryde/edman
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database :: Front-Ends
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 edman
 =====
```

### Comparing `edman-2023.5.23/tests/test_convert.py` & `edman-2023.5.8/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.23/tests/test_db.py` & `edman-2023.5.8/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.23/tests/test_file.py` & `edman-2023.5.8/tests/test_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -438,34 +438,29 @@
     def test_zipped_json(self):
 
         # # 正常系
         s = {"document": [{"test1": "ABC"}, {"test2": 12345}]}
         raw_json = dumps(s, ensure_ascii=False, indent=4)
         encoded_json = raw_json.encode('utf-8')
         filename = 'jsonfile'
+        ac_z_path = self.file.zipped_json(encoded_json, filename)
 
+        # ac_z_pathを解凍して中身のファイル名がzipped_filepathと同じか調べる
         with tempfile.TemporaryDirectory() as tmpdir:
-            p = Path(tmpdir)
-            ac_z_path = self.file.zipped_json(encoded_json, filename, p)
-
-            # 圧縮前のjsonファイルを削除する
-            first_file = filename + '.json'
-            first = p / first_file
-            first.unlink()
-
-            # ac_z_pathを解凍して中身のファイル名がzipped_filepathと同じか調べる
             with zipfile.ZipFile(ac_z_path, 'r') as inputFile:
                 inputFile.extractall(tmpdir)
-
+            p = Path(tmpdir)
             # 解凍されたディレクトリ名を取得する
+            # print(list(p.glob('**/*.json')))
             ps = list(p.glob('**/*.json'))[0]
             actual = ps.stem
 
         expected = filename
         self.assertEqual(expected, actual)
+        os.unlink(ac_z_path)
 
     def test_zipped_contents(self):
         if not self.db_server_connect:
             return
 
         with tempfile.TemporaryDirectory() as tmp_dl_dir:
             # 添付ファイル用テキストファイル作成
@@ -533,39 +528,38 @@
             res = search.process_data_derived_from_mongodb(
                 result_with_filepath)
 
         # 実行
         raw_json = dumps(res, ensure_ascii=False, indent=4)
         encoded_json = raw_json.encode('utf-8')
         json_tree_file_name = 'json_tree'
-
+        zip_filepath = self.file.zipped_contents(downloads,
+                                                 json_tree_file_name,
+                                                 encoded_json)
         with tempfile.TemporaryDirectory() as tmp:
-            p = Path(tmp)
-            zip_filepath = self.file.zipped_contents(downloads,
-                                                     json_tree_file_name,
-                                                     encoded_json, p)
             # 解凍
-            # print('unpack before',list(p.iterdir()))
             shutil.unpack_archive(zip_filepath, tmp)
-            # print('unpack after', list(p.iterdir()))
-
             # 添付ファイルを読み込んでテキストの中身を抽出
             path_lists = [tmp, str(list(downloads.keys())[0]), name]
             with open(os.path.join(*path_lists)) as f:
                 attached_s = f.read()
             path_lists = [tmp, json_tree_file_name + '.json']
             json_file_path = os.path.join(*path_lists)
             with open(json_file_path) as jf:
                 j_data = json.load(jf)
             # 外に出すデータを組み立て(zip内部のjsonデータ、上記の添付ファイルデータ)
             actual_data = {'json_data': j_data, 'attached_data': attached_s}
         # テスト
         self.assertDictEqual(res, actual_data['json_data'])
         self.assertEqual(test_var, actual_data['attached_data'])
 
+        # テスト用zipファイル削除
+        if os.path.exists(zip_filepath):
+            os.remove(zip_filepath)
+
     def test_get_fileref_and_generate_dl_list(self):
 
         if not self.db_server_connect:
             return
 
         # DBにdocsと添付ファイルを挿入する
         with tempfile.TemporaryDirectory() as tmp_dl_dir:
@@ -643,20 +637,18 @@
             # ファイル読み込み、ファイルをgridfsに入れる
             files_oid = []
             self.fs = gridfs.GridFS(self.testdb)
             test_vars = {}
             for filename in files:
                 with filename.open('rb') as f:
                     content = f.read()
-                    # file_obj = gzip.compress(content, compresslevel=6)
-                    # files_oid.append(
-                    #     self.fs.put(file_obj, filename=filename.name,
-                    #                 compress='gzip'))
+                    file_obj = gzip.compress(content, compresslevel=6)
                     files_oid.append(
-                        self.fs.put(content, filename=filename.name))
+                        self.fs.put(file_obj, filename=filename.name,
+                                    compress='gzip'))
                     test_vars.update({filename.name: content.decode()})
 
         with tempfile.TemporaryDirectory() as tmp_dl_dir:
             path = Path(tmp_dl_dir)
 
             grid_out_result = self.file._grid_out(files_oid, tmp_dl_dir)
             # 実行結果
@@ -893,132 +885,29 @@
         if not self.db_server_connect:
             return
 
         # 正常系
         with tempfile.TemporaryDirectory() as tmp_dir:
             sample_files = self.make_txt_files(tmp_dir, name='grid_in_test',
                                                qty=2)
-            compress_settings = [False, False]
+            compress_settings = [True, False]
             td = tuple(
                 [(p, b) for (p, b) in zip(sample_files, compress_settings)])
 
             self.fs = gridfs.GridFS(self.testdb)
             actual = []
             for oid in self.file.grid_in(td):
                 data = self.fs.get(oid)
-                f_data = data.read().decode()
-                b_data = False
+                if data.compress == 'gzip':
+                    f_data = gzip.decompress(data.read()).decode()
+                    b_data = True
+                else:
+                    f_data = data.read().decode()
+                    b_data = False
                 actual.append([data.filename, f_data, b_data])
 
             expected = []
             for file_path, compress in zip(sample_files, compress_settings):
                 with file_path.open() as f:
                     expected.append([file_path.name, f.read(), compress])
 
             self.assertListEqual(sorted(actual), sorted(expected))
-
-    def test_generate_file_path_dict(self):
-        with tempfile.TemporaryDirectory() as tmp:
-            tmp_p = Path(tmp)
-            p = tmp_p / 'sub'
-            p.mkdir()
-            sample_files = self.make_txt_files(p,
-                                               name='generate_file_path_dict_test',
-                                               qty=2)
-            file_list = list(map(str, sample_files))
-            expected = {k: v for k, v in zip(file_list, sample_files)}
-            actual = self.file.generate_file_path_dict(file_list, p)
-
-            # paths = [(v, False) for k, v in actual.items()]
-            # data = tuple(paths)
-            # print('data', data)
-            # grid_in_results = self.file.grid_in(data)
-            # gf_inserted_dict = {}
-            # for i, j in zip(actual, grid_in_results):
-            #     gf_inserted_dict.update({i: j})
-            # print('gf_inserted_dict', gf_inserted_dict)
-
-            self.assertDictEqual(actual, expected)
-
-    def test_generate_upload_list(self):
-        json_dict = {
-            "position": "top",
-            "structure_2": [
-                {
-                    "maker": "Ferrari",
-                    "carname": "F355",
-                    "power": 380,
-                    "_ed_attachment": ['aaa/01.jpg']
-                },
-                {
-                    "maker": "Ferrari",
-                    "carname": "458 Italia",
-                    "_ed_attachment": ['bbb/01.jpg', 'bbb/02.jpg'],
-
-                }],
-            "structure_3": {
-                "structure_4": {
-                    "data1": 45,
-                    "_ed_attachment": ['ccc/01.jpg']}
-            }
-        }
-        expected = ['aaa/01.jpg', 'bbb/01.jpg', 'bbb/02.jpg', 'ccc/01.jpg']
-        actual = self.file.generate_upload_list(json_dict)
-        # print(actual)
-        self.assertListEqual(actual, expected)
-
-    def test_json_rewrite(self):
-        if not self.db_server_connect:
-            return
-
-        json_dict = {
-            "position": "top",
-            "structure_2": [
-                {
-                    "maker": "Ferrari",
-                    "carname": "F355",
-                    "power": 380,
-                    "_ed_attachment": ['aaa/01.jpg']
-                },
-                {
-                    "maker": "Ferrari",
-                    "carname": "458 Italia",
-                    "_ed_attachment": ['bbb/01.jpg', 'bbb/02.jpg'],
-
-                }],
-            "structure_3": {
-                "structure_4": {
-                    "data1": 45,
-                    "_ed_attachment": ['ccc/01.jpg']}
-            }
-        }
-        a01_file = ObjectId()
-        b01_file = ObjectId()
-        b02_file = ObjectId()
-        c01_file = ObjectId()
-        files_dict = {'aaa/01.jpg': a01_file,
-                      'bbb/01.jpg': b01_file,
-                      'bbb/02.jpg': b02_file,
-                      'ccc/01.jpg': c01_file}
-        expected = {
-            "position": "top",
-            "structure_2": [
-                {
-                    "maker": "Ferrari",
-                    "carname": "F355",
-                    "power": 380,
-                    "_ed_file": [a01_file]
-                },
-                {
-                    "maker": "Ferrari",
-                    "carname": "458 Italia",
-                    "_ed_file": [b01_file, b02_file]
-                }],
-            "structure_3": {
-                "structure_4": {
-                    "data1": 45,
-                    "_ed_file": [c01_file]}
-            }
-        }
-        actual = self.file.json_rewrite(json_dict, files_dict)
-        # print(actual)
-        self.assertDictEqual(actual, expected)
```

### Comparing `edman-2023.5.23/tests/test_multiuser.py` & `edman-2023.5.8/tests/test_multiuser.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.23/tests/test_search.py` & `edman-2023.5.8/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `edman-2023.5.23/tests/test_utils.py` & `edman-2023.5.8/tests/test_utils.py`

 * *Files identical despite different names*

