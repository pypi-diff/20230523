# Comparing `tmp/monkey.crawler.ldap-0.0.1.dev2.tar.gz` & `tmp/monkey.crawler.ldap-2.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monkey.crawler.ldap-0.0.1.dev2.tar", last modified: Mon Sep 20 08:55:03 2021, max compression
+gzip compressed data, was "monkey.crawler.ldap-2.0.0.dev1.tar", last modified: Tue May 23 11:53:53 2023, max compression
```

## Comparing `monkey.crawler.ldap-0.0.1.dev2.tar` & `monkey.crawler.ldap-2.0.0.dev1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2021-09-20 08:55:03.768997 monkey.crawler.ldap-0.0.1.dev2/
--rw-rw-rw-   0        0        0    11556 2021-08-12 08:39:34.000000 monkey.crawler.ldap-0.0.1.dev2/LICENSE.txt
--rw-rw-rw-   0        0        0       60 2021-08-12 08:39:34.000000 monkey.crawler.ldap-0.0.1.dev2/MANIFEST.in
--rw-rw-rw-   0        0        0      920 2021-09-20 08:55:03.768997 monkey.crawler.ldap-0.0.1.dev2/PKG-INFO
--rw-rw-rw-   0        0        0      266 2021-08-12 08:39:34.000000 monkey.crawler.ldap-0.0.1.dev2/README.rst
-drwxrwxrwx   0        0        0        0 2021-09-20 08:55:03.757028 monkey.crawler.ldap-0.0.1.dev2/monkey/
--rw-rw-rw-   0        0        0       84 2021-08-12 08:39:34.000000 monkey.crawler.ldap-0.0.1.dev2/monkey/__init__.py
-drwxrwxrwx   0        0        0        0 2021-09-20 08:55:03.765007 monkey.crawler.ldap-0.0.1.dev2/monkey/crawler/
--rw-rw-rw-   0        0        0       84 2021-08-12 08:39:34.000000 monkey.crawler.ldap-0.0.1.dev2/monkey/crawler/__init__.py
-drwxrwxrwx   0        0        0        0 2021-09-20 08:55:03.767002 monkey.crawler.ldap-0.0.1.dev2/monkey/crawler/ldap/
--rw-rw-rw-   0        0        0       55 2021-09-20 08:51:54.000000 monkey.crawler.ldap-0.0.1.dev2/monkey/crawler/ldap/__init__.py
-drwxrwxrwx   0        0        0        0 2021-09-20 08:55:03.768000 monkey.crawler.ldap-0.0.1.dev2/monkey/crawler/ldap/handlers/
--rw-rw-rw-   0        0        0       84 2021-08-12 08:39:34.000000 monkey.crawler.ldap-0.0.1.dev2/monkey/crawler/ldap/handlers/__init__.py
--rw-rw-rw-   0        0        0     6435 2021-08-12 08:39:34.000000 monkey.crawler.ldap-0.0.1.dev2/monkey/crawler/ldap/handlers/ad.py
--rw-rw-rw-   0        0        0     2216 2021-08-12 08:39:34.000000 monkey.crawler.ldap-0.0.1.dev2/monkey/crawler/ldap/ldap3.py
-drwxrwxrwx   0        0        0        0 2021-09-20 08:55:03.762016 monkey.crawler.ldap-0.0.1.dev2/monkey.crawler.ldap.egg-info/
--rw-rw-rw-   0        0        0      920 2021-09-20 08:55:03.000000 monkey.crawler.ldap-0.0.1.dev2/monkey.crawler.ldap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      457 2021-09-20 08:55:03.000000 monkey.crawler.ldap-0.0.1.dev2/monkey.crawler.ldap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-09-20 08:55:03.000000 monkey.crawler.ldap-0.0.1.dev2/monkey.crawler.ldap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2021-09-20 08:55:03.000000 monkey.crawler.ldap-0.0.1.dev2/monkey.crawler.ldap.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2021-09-20 08:55:03.000000 monkey.crawler.ldap-0.0.1.dev2/monkey.crawler.ldap.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       38 2021-08-12 08:39:34.000000 monkey.crawler.ldap-0.0.1.dev2/requirements.txt
--rw-rw-rw-   0        0        0       42 2021-09-20 08:55:03.768997 monkey.crawler.ldap-0.0.1.dev2/setup.cfg
--rw-rw-rw-   0        0        0     1294 2021-08-12 08:39:34.000000 monkey.crawler.ldap-0.0.1.dev2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 11:53:53.925373 monkey.crawler.ldap-2.0.0.dev1/
+-rw-rw-rw-   0        0        0    11556 2023-05-23 11:33:06.000000 monkey.crawler.ldap-2.0.0.dev1/LICENSE.txt
+-rw-rw-rw-   0        0        0       60 2023-05-23 11:33:06.000000 monkey.crawler.ldap-2.0.0.dev1/MANIFEST.in
+-rw-rw-rw-   0        0        0      920 2023-05-23 11:53:53.925373 monkey.crawler.ldap-2.0.0.dev1/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-05-23 11:33:06.000000 monkey.crawler.ldap-2.0.0.dev1/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-23 11:53:53.894239 monkey.crawler.ldap-2.0.0.dev1/monkey/
+-rw-rw-rw-   0        0        0       84 2023-05-23 11:33:06.000000 monkey.crawler.ldap-2.0.0.dev1/monkey/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 11:53:53.914333 monkey.crawler.ldap-2.0.0.dev1/monkey/crawler/
+-rw-rw-rw-   0        0        0       84 2023-05-23 11:33:06.000000 monkey.crawler.ldap-2.0.0.dev1/monkey/crawler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 11:53:53.919320 monkey.crawler.ldap-2.0.0.dev1/monkey/crawler/ldap/
+-rw-rw-rw-   0        0        0       55 2023-05-23 11:33:06.000000 monkey.crawler.ldap-2.0.0.dev1/monkey/crawler/ldap/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 11:53:53.923376 monkey.crawler.ldap-2.0.0.dev1/monkey/crawler/ldap/handlers/
+-rw-rw-rw-   0        0        0       84 2023-05-23 11:33:06.000000 monkey.crawler.ldap-2.0.0.dev1/monkey/crawler/ldap/handlers/__init__.py
+-rw-rw-rw-   0        0        0     6435 2023-05-23 11:33:06.000000 monkey.crawler.ldap-2.0.0.dev1/monkey/crawler/ldap/handlers/ad.py
+-rw-rw-rw-   0        0        0     2186 2023-05-23 11:33:06.000000 monkey.crawler.ldap-2.0.0.dev1/monkey/crawler/ldap/ldap3.py
+drwxrwxrwx   0        0        0        0 2023-05-23 11:53:53.912339 monkey.crawler.ldap-2.0.0.dev1/monkey.crawler.ldap.egg-info/
+-rw-rw-rw-   0        0        0      920 2023-05-23 11:53:53.000000 monkey.crawler.ldap-2.0.0.dev1/monkey.crawler.ldap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2023-05-23 11:53:53.000000 monkey.crawler.ldap-2.0.0.dev1/monkey.crawler.ldap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 11:53:53.000000 monkey.crawler.ldap-2.0.0.dev1/monkey.crawler.ldap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-05-23 11:53:53.000000 monkey.crawler.ldap-2.0.0.dev1/monkey.crawler.ldap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-23 11:53:53.000000 monkey.crawler.ldap-2.0.0.dev1/monkey.crawler.ldap.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       38 2023-05-23 11:33:06.000000 monkey.crawler.ldap-2.0.0.dev1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 11:53:53.926370 monkey.crawler.ldap-2.0.0.dev1/setup.cfg
+-rw-rw-rw-   0        0        0     1294 2023-05-23 11:53:44.000000 monkey.crawler.ldap-2.0.0.dev1/setup.py
```

### Comparing `monkey.crawler.ldap-0.0.1.dev2/LICENSE.txt` & `monkey.crawler.ldap-2.0.0.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `monkey.crawler.ldap-0.0.1.dev2/PKG-INFO` & `monkey.crawler.ldap-2.0.0.dev1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monkey.crawler.ldap
-Version: 0.0.1.dev2
+Version: 2.0.0.dev1
 Summary: Monkey crawler implementation for LDAP directory.
 Home-page: https://bitbucket.org/monkey-python/monkey-crawler-ldap/
 Author: Xavier ROY
 Author-email: xavier@regbuddy.eu
 License: Apache License, Version 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `monkey.crawler.ldap-0.0.1.dev2/monkey/crawler/ldap/handlers/ad.py` & `monkey.crawler.ldap-2.0.0.dev1/monkey/crawler/ldap/handlers/ad.py`

 * *Files identical despite different names*

### Comparing `monkey.crawler.ldap-0.0.1.dev2/monkey/crawler/ldap/ldap3.py` & `monkey.crawler.ldap-2.0.0.dev1/monkey/crawler/ldap/ldap3.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,32 +4,33 @@
 
 from monkey.crawler.crawler import Crawler
 from monkey.crawler.processor import Processor
 
 
 class LDAPCrawler(Crawler):
 
-    def __init__(self, source_name: str, processor: Processor, ds_hostname: str, user_name: str, password: str,
+    def __init__(self, source_name: str, ds_hostname: str, user_name: str, password: str,
                  search_base: str, search_filter: str, attributes=None,
-                 search_scope=SUBTREE, limit: int = 0, page_size=100, offset: int = 0, max_retry: int = 0):
-        super().__init__(source_name, processor, offset, max_retry)
+                 search_scope=SUBTREE, limit: int = 0, page_size=100, default_offset: int = 0):
+        super().__init__(source_name, default_offset)
         self.ds_hostname = ds_hostname
         self.user_name = user_name
         self.password = password
         self.base_dn = search_base
         self.search_filter = search_filter
         self.attributes = attributes
         self.limit = limit
         self.search_scope = search_scope
         self.page_size = page_size
 
-    def _get_records(self):
+    def _get_records(self, offset: int = 0):
         server = Server(self.ds_hostname)
         conn = Connection(server, user=self.user_name, password=self.password)
         conn.bind()
+        # TODO: Handle offset
         self._cursor = conn.extend.standard.paged_search(self.base_dn, self.search_filter,
                                                          search_scope=self.search_scope,
                                                          attributes=self.attributes,
                                                          paged_size=self.page_size,
                                                          size_limit=self.limit,
                                                          generator=True)
         return self
@@ -48,11 +49,9 @@
                     'dn': dn
                 }
                 record.update(rec['attributes'])
                 return record
         except StopIteration as e:
             raise e
 
-    def _echo_start(self):
-        self.logger.info(
-            f'Crawling {self.source_name} from LDAP server {self.ds_hostname}.'
-        )
+    def _get_start_message(self):
+        return f'Crawling {self.source_name} from LDAP server {self.ds_hostname}.'
```

### Comparing `monkey.crawler.ldap-0.0.1.dev2/monkey.crawler.ldap.egg-info/PKG-INFO` & `monkey.crawler.ldap-2.0.0.dev1/monkey.crawler.ldap.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monkey.crawler.ldap
-Version: 0.0.1.dev2
+Version: 2.0.0.dev1
 Summary: Monkey crawler implementation for LDAP directory.
 Home-page: https://bitbucket.org/monkey-python/monkey-crawler-ldap/
 Author: Xavier ROY
 Author-email: xavier@regbuddy.eu
 License: Apache License, Version 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `monkey.crawler.ldap-0.0.1.dev2/setup.py` & `monkey.crawler.ldap-2.0.0.dev1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import os
 from setuptools import setup, find_packages
 
 __name__ = 'monkey.crawler.ldap'
-__version__ = '0.0.1.dev2'
+__version__ = '2.0.0.dev1'
 __author__ = 'Xavier ROY'
 __author_email__ = 'xavier@regbuddy.eu'
 
 project_dir = os.path.dirname(os.path.realpath(__file__))
 requirement_file_path = project_dir + '/requirements.txt'
 requirements = []
 if os.path.isfile(requirement_file_path):
```

