# Comparing `tmp/com.castsoftware.uc.python.common-1.0.4.tar.gz` & `tmp/com.castsoftware.uc.python.common-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "com.castsoftware.uc.python.common-1.0.4.tar", last modified: Thu May 18 17:41:39 2023, max compression
+gzip compressed data, was "com.castsoftware.uc.python.common-1.0.5.tar", last modified: Tue May 23 17:45:07 2023, max compression
```

## Comparing `com.castsoftware.uc.python.common-1.0.4.tar` & `com.castsoftware.uc.python.common-1.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 17:41:39.118391 com.castsoftware.uc.python.common-1.0.4/
--rw-rw-rw-   0        0        0    35823 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      714 2023-05-18 17:41:39.109952 com.castsoftware.uc.python.common-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      103 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 17:41:39.037442 com.castsoftware.uc.python.common-1.0.4/cast_common/
--rw-rw-rw-   0        0        0     2036 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.4/cast_common/abstractClass.py
--rw-rw-rw-   0        0        0    11811 2023-05-18 15:27:04.000000 com.castsoftware.uc.python.common-1.0.4/cast_common/aipRestCall.py
--rw-rw-rw-   0        0        0     4069 2023-05-18 15:21:32.000000 com.castsoftware.uc.python.common-1.0.4/cast_common/highlight.py
--rw-rw-rw-   0        0        0     5478 2023-05-18 15:25:57.000000 com.castsoftware.uc.python.common-1.0.4/cast_common/hlRestCall.py
--rw-rw-rw-   0        0        0     1688 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.4/cast_common/logger.py
--rw-rw-rw-   0        0        0     3823 2023-05-18 15:32:24.000000 com.castsoftware.uc.python.common-1.0.4/cast_common/restAPI.py
--rw-rw-rw-   0        0        0     6930 2023-05-18 15:27:50.000000 com.castsoftware.uc.python.common-1.0.4/cast_common/util.py
-drwxrwxrwx   0        0        0        0 2023-05-18 17:41:39.096689 com.castsoftware.uc.python.common-1.0.4/com.castsoftware.uc.python.common.egg-info/
--rw-rw-rw-   0        0        0      714 2023-05-18 17:41:38.000000 com.castsoftware.uc.python.common-1.0.4/com.castsoftware.uc.python.common.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      488 2023-05-18 17:41:38.000000 com.castsoftware.uc.python.common-1.0.4/com.castsoftware.uc.python.common.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 17:41:38.000000 com.castsoftware.uc.python.common-1.0.4/com.castsoftware.uc.python.common.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-18 17:41:38.000000 com.castsoftware.uc.python.common-1.0.4/com.castsoftware.uc.python.common.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-18 17:41:38.000000 com.castsoftware.uc.python.common-1.0.4/com.castsoftware.uc.python.common.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      630 2023-05-18 17:34:18.000000 com.castsoftware.uc.python.common-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-18 17:41:39.118391 com.castsoftware.uc.python.common-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-23 17:45:07.472983 com.castsoftware.uc.python.common-1.0.5/
+-rw-rw-rw-   0        0        0    35823 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0      714 2023-05-23 17:45:07.464557 com.castsoftware.uc.python.common-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      103 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 17:45:07.356525 com.castsoftware.uc.python.common-1.0.5/cast_common/
+-rw-rw-rw-   0        0        0     2036 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.5/cast_common/abstractClass.py
+-rw-rw-rw-   0        0        0    11918 2023-05-23 14:56:31.000000 com.castsoftware.uc.python.common-1.0.5/cast_common/aipRestCall.py
+-rw-rw-rw-   0        0        0     7524 2023-05-23 17:44:36.000000 com.castsoftware.uc.python.common-1.0.5/cast_common/highlight.py
+-rw-rw-rw-   0        0        0     5478 2023-05-18 15:25:57.000000 com.castsoftware.uc.python.common-1.0.5/cast_common/hlRestCall.py
+-rw-rw-rw-   0        0        0     1688 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.5/cast_common/logger.py
+-rw-rw-rw-   0        0        0     5264 2023-05-21 20:59:32.000000 com.castsoftware.uc.python.common-1.0.5/cast_common/restAPI.py
+-rw-rw-rw-   0        0        0     6930 2023-05-18 15:27:50.000000 com.castsoftware.uc.python.common-1.0.5/cast_common/util.py
+drwxrwxrwx   0        0        0        0 2023-05-23 17:45:07.449864 com.castsoftware.uc.python.common-1.0.5/com.castsoftware.uc.python.common.egg-info/
+-rw-rw-rw-   0        0        0      714 2023-05-23 17:45:07.000000 com.castsoftware.uc.python.common-1.0.5/com.castsoftware.uc.python.common.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      488 2023-05-23 17:45:07.000000 com.castsoftware.uc.python.common-1.0.5/com.castsoftware.uc.python.common.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 17:45:07.000000 com.castsoftware.uc.python.common-1.0.5/com.castsoftware.uc.python.common.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-05-23 17:45:07.000000 com.castsoftware.uc.python.common-1.0.5/com.castsoftware.uc.python.common.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-23 17:45:07.000000 com.castsoftware.uc.python.common-1.0.5/com.castsoftware.uc.python.common.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      643 2023-05-23 17:43:34.000000 com.castsoftware.uc.python.common-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-23 17:45:07.472983 com.castsoftware.uc.python.common-1.0.5/setup.cfg
```

### Comparing `com.castsoftware.uc.python.common-1.0.4/LICENSE` & `com.castsoftware.uc.python.common-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.0.4/PKG-INFO` & `com.castsoftware.uc.python.common-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.python.common
-Version: 1.0.4
+Version: 1.0.5
 Summary: A set of common classes and methods for use with python projects
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.python.common
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.python.common/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10.6
```

### Comparing `com.castsoftware.uc.python.common-1.0.4/cast_common/abstractClass.py` & `com.castsoftware.uc.python.common-1.0.5/cast_common/abstractClass.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.0.4/cast_common/aipRestCall.py` & `com.castsoftware.uc.python.common-1.0.5/cast_common/aipRestCall.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,16 @@
         if len(rule_arg) > 0:
             rule_arg = rule_arg + ','
         rule_arg=f'{rule_arg}{non_critical_arg}'
 
         url = f'{domain_id}/applications/3/snapshots/{snapshot_id}/violations?rule-pattern={rule_arg}&startRow={start_row}&nbRows={max_rows}'
         (status,json) = self.get(url)
         if status == codes.ok and len(json) > 0:
-            rslt_df = DataFrame(json)
+            rslt_df = json_normalize(json,meta=['component','diagnosis','remedialAction','rulePattern'])
+            #rslt_df = DataFrame(json)
         return rslt_df
 
 
     def get_action_plan(self,domain_id,snapshot_id):
         business_criteria = ['Robustness','Efficiency','Security','Transferability','Changeability']
     
         catagory = ''
```

### Comparing `com.castsoftware.uc.python.common-1.0.4/cast_common/hlRestCall.py` & `com.castsoftware.uc.python.common-1.0.5/cast_common/hlRestCall.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.0.4/cast_common/logger.py` & `com.castsoftware.uc.python.common-1.0.5/cast_common/logger.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.0.4/cast_common/restAPI.py` & `com.castsoftware.uc.python.common-1.0.5/cast_common/restAPI.py`

 * *Files 19% similar despite different names*

```diff
@@ -93,7 +93,41 @@
         except exceptions.HTTPError as e:
             self.error(e)
         except exceptions.RequestException as e:
             # catastrophic error. bail.
             self.error(f'General Request exception while performing api request using: {u}')
 
         return 0, "{}"
+    
+    def post(self, url = "",data = {}):
+
+        try:
+            if len(url) > 0 and url[0] != '/':
+                url=f'/{url}'
+            u = urllib.parse.quote(f'{self._base_url}{url}',safe='/:&?=')
+
+            resp = self._session.post(u,data=data,timeout = (5, 15),auth=self._auth,headers={'Accept': 'application/json'})
+            resp.raise_for_status()
+
+            if resp.status_code == codes.ok:
+                return resp.status_code, resp.json()
+            elif resp.status_code == codes.no_content:
+                return resp.status_code, {}
+            else:
+                return resp.status_code,""
+
+        except exceptions.ConnectionError:
+            self.error(f'Unable to connect to host {self._base_url}')
+        except exceptions.Timeout:
+            #TODO Maybe set up for a retry, or continue in a retry loop
+            self.error(f'Timeout while performing api request using: {url}')
+        except exceptions.TooManyRedirects:
+            #TODO Tell the user their URL was bad and try a different one
+            self.error(f'TooManyRedirects while performing api request using: {url}')
+        except exceptions.HTTPError as e:
+            self.error(e)
+        except exceptions.RequestException as e:
+            # catastrophic error. bail.
+            self.error(f'General Request exception while performing api request using: {u}')
+
+        return 0, "{}"
+
```

### Comparing `com.castsoftware.uc.python.common-1.0.4/cast_common/util.py` & `com.castsoftware.uc.python.common-1.0.5/cast_common/util.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.0.4/com.castsoftware.uc.python.common.egg-info/PKG-INFO` & `com.castsoftware.uc.python.common-1.0.5/com.castsoftware.uc.python.common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.python.common
-Version: 1.0.4
+Version: 1.0.5
 Summary: A set of common classes and methods for use with python projects
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.python.common
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.python.common/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10.6
```

### Comparing `com.castsoftware.uc.python.common-1.0.4/pyproject.toml` & `com.castsoftware.uc.python.common-1.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name='com.castsoftware.uc.python.common'
 description="A set of common classes and methods for use with python projects"
 
-version='1.0.4' #prod version
+version='1.0.5' #prod version
 
-dependencies = ['pandas','requests']
+dependencies = ['pandas','requests','XlsxWriter']
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 requires-python = ">=3.10.6"
```

