# Comparing `tmp/mfiles-0.5.2.tar.gz` & `tmp/mfiles-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mfiles-0.5.2.tar", last modified: Sat May  2 21:39:12 2020, max compression
+gzip compressed data, was "dist\mfiles-0.5.3.tar", last modified: Tue May 23 11:48:55 2023, max compression
```

## Comparing `mfiles-0.5.2.tar` & `mfiles-0.5.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2020-05-02 21:39:12.000000 mfiles-0.5.2/
--rw-rw-rw-   0        0        0     1032 2020-05-02 21:39:12.000000 mfiles-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     1174 2020-04-30 10:37:59.000000 mfiles-0.5.2/README.rst
-drwxrwxrwx   0        0        0        0 2020-05-02 21:39:12.000000 mfiles-0.5.2/mfiles/
--rw-rw-rw-   0        0        0      756 2020-04-29 13:37:13.000000 mfiles-0.5.2/mfiles/__init__.py
--rw-rw-rw-   0        0        0    21042 2020-05-02 21:36:44.000000 mfiles-0.5.2/mfiles/client.py
--rw-rw-rw-   0        0        0     1187 2020-04-29 13:37:13.000000 mfiles-0.5.2/mfiles/definitions.py
--rw-rw-rw-   0        0        0       98 2020-04-29 13:37:13.000000 mfiles-0.5.2/mfiles/errors.py
-drwxrwxrwx   0        0        0        0 2020-05-02 21:39:12.000000 mfiles-0.5.2/mfiles.egg-info/
--rw-rw-rw-   0        0        0     1032 2020-05-02 21:39:11.000000 mfiles-0.5.2/mfiles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2020-05-02 21:39:12.000000 mfiles-0.5.2/mfiles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-05-02 21:39:11.000000 mfiles-0.5.2/mfiles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2020-05-02 21:39:11.000000 mfiles-0.5.2/mfiles.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2020-05-02 21:39:11.000000 mfiles-0.5.2/mfiles.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       87 2020-05-02 21:39:12.000000 mfiles-0.5.2/setup.cfg
--rw-rw-rw-   0        0        0     1279 2020-05-02 21:39:01.000000 mfiles-0.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2020-05-02 21:39:12.000000 mfiles-0.5.2/test/
--rw-rw-rw-   0        0        0        0 2020-04-29 13:37:13.000000 mfiles-0.5.2/test/__init__.py
--rw-rw-rw-   0        0        0      249 2020-05-02 20:29:22.000000 mfiles-0.5.2/test/client_test.py
--rw-rw-rw-   0        0        0     1023 2020-05-02 21:14:13.000000 mfiles-0.5.2/test/local_test.py
+drwxrwxrwx   0        0        0        0 2023-05-23 11:48:55.000000 mfiles-0.5.3/
+-rw-rw-rw-   0        0        0     1032 2023-05-23 11:48:55.000000 mfiles-0.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1174 2020-04-30 10:37:59.000000 mfiles-0.5.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-23 11:48:55.000000 mfiles-0.5.3/mfiles/
+-rw-rw-rw-   0        0        0      756 2020-04-29 13:37:13.000000 mfiles-0.5.3/mfiles/__init__.py
+-rw-rw-rw-   0        0        0    21143 2023-05-23 11:40:35.000000 mfiles-0.5.3/mfiles/client.py
+-rw-rw-rw-   0        0        0     1187 2020-04-29 13:37:13.000000 mfiles-0.5.3/mfiles/definitions.py
+-rw-rw-rw-   0        0        0       98 2020-04-29 13:37:13.000000 mfiles-0.5.3/mfiles/errors.py
+drwxrwxrwx   0        0        0        0 2023-05-23 11:48:55.000000 mfiles-0.5.3/mfiles.egg-info/
+-rw-rw-rw-   0        0        0     1032 2023-05-23 11:48:55.000000 mfiles-0.5.3/mfiles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2023-05-23 11:48:55.000000 mfiles-0.5.3/mfiles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 11:48:55.000000 mfiles-0.5.3/mfiles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-23 11:48:55.000000 mfiles-0.5.3/mfiles.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-23 11:48:55.000000 mfiles-0.5.3/mfiles.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       87 2023-05-23 11:48:55.000000 mfiles-0.5.3/setup.cfg
+-rw-rw-rw-   0        0        0     1279 2023-05-23 11:44:19.000000 mfiles-0.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 11:48:55.000000 mfiles-0.5.3/test/
+-rw-rw-rw-   0        0        0        0 2020-04-29 13:37:13.000000 mfiles-0.5.3/test/__init__.py
+-rw-rw-rw-   0        0        0      249 2020-05-02 20:29:22.000000 mfiles-0.5.3/test/client_test.py
+-rw-rw-rw-   0        0        0     1023 2020-05-02 21:14:13.000000 mfiles-0.5.3/test/local_test.py
```

### Comparing `mfiles-0.5.2/PKG-INFO` & `mfiles-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: mfiles
-Version: 0.5.2
+Version: 0.5.3
 Summary: M-Files API wrapper
 Home-page: https://github.com/afcmrp/python-mfiles
 Author: Emil Hjelm
 Author-email: emil.hjelm@climeon.com
 License: MIT
 Description: 
         Python wrapper around the M-Files API.
```

### Comparing `mfiles-0.5.2/README.rst` & `mfiles-0.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `mfiles-0.5.2/mfiles/__init__.py` & `mfiles-0.5.3/mfiles/__init__.py`

 * *Files identical despite different names*

### Comparing `mfiles-0.5.2/mfiles/client.py` & `mfiles-0.5.3/mfiles/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,16 @@
 
     def __init__(self, server=DEFAULT_URL, user=None, password=None, vault=None):
         self.user = user
         self.password = password
         self.vault = vault
         self.server = ""
         self.headers = {"X-Authentication": ""}
+        # need before set_server
+        self.session = requests.Session()
         self.set_server(server)
 
     def set_server(self, server):
         """Set the M-Files server API URL."""
         if server[-1] != "/":
             server += "/"
         self.server = server
@@ -95,15 +97,15 @@
         self.vault = vault or self.vault or env_vault
         if not all([self.server, self.user, self.password, self.vault]):
             return
         auth = json.dumps({"Username": self.user,
                            "Password": self.password,
                            "VaultGuid": self.vault})
         request_url = self.server + "server/authenticationtokens"
-        response = requests.post(request_url, data=auth)
+        response = self.session.post(request_url, data=auth)
         auth_token = json.loads(response.text)["Value"]
         self.headers = {"X-Authentication": auth_token}
 
     def get(self, endpoint):
         """General purpose GET method.
 
         Parameters:
@@ -114,15 +116,15 @@
 
         Returns:
             dict: Dictionary with request result.
         """
         if endpoint[0] == "/":
             endpoint = endpoint[1:]
         request_url = self.server + endpoint
-        response = requests.get(request_url, headers=self.headers)
+        response = self.session.get(request_url, headers=self.headers)
         if response.status_code != 200:
             raise MFilesException(response.text)
         return response.json()
 
     def put(self, endpoint, data=None):
         """General purpose PUT method.
 
@@ -135,15 +137,15 @@
 
         Returns:
             dict: Dictionary with request result.
         """
         if endpoint[0] == "/":
             endpoint = endpoint[1:]
         request_url = self.server + endpoint
-        response = requests.put(request_url, headers=self.headers, data=data)
+        response = self.session.put(request_url, headers=self.headers, data=data)
         if response.status_code != 200:
             raise MFilesException(response.text)
         return response.json()
 
     def post(self, endpoint, data=None):
         """General purpose POST method.
 
@@ -156,15 +158,15 @@
 
         Returns:
             dict: Dictionary with request result.
         """
         if endpoint[0] == "/":
             endpoint = endpoint[1:]
         request_url = self.server + endpoint
-        response = requests.post(request_url, headers=self.headers, data=data)
+        response = self.session.post(request_url, headers=self.headers, data=data)
         if response.status_code != 200:
             raise MFilesException(response.text)
         return response.json()
 
     def quick_search(self, query):
         """Perform a quick search in the M-Files vault.
 
@@ -473,15 +475,15 @@
 
         Returns:
             bool: True if file is found and downloaded successfully.
         """
         # pylint: disable=too-many-arguments
         request_url = "%sobjects/%s/%s/%s/files/%s/content" % \
             (self.server, object_type, object_id, object_version, file_id)
-        response = requests.get(request_url, headers=self.headers)
+        response = self.session.get(request_url, headers=self.headers)
         if response.status_code != 200:
             raise MFilesException(response.text)
         with open(local_path, mode="wb+") as file_stream:
             file_stream.write(response.content)
         return True
 
     def download_file_name(self, file_name, local_path=None):
@@ -534,11 +536,11 @@
 
         Caution:
             Destroying an object means unrecoverably deleting all
             versions of the object. Use with caution.
         """
         request_url = "%sobjects/%s/%s/latest?allVersions=true" % \
             (self.server, object_type, object_id)
-        response = requests.delete(request_url, headers=self.headers)
+        response = self.session.delete(request_url, headers=self.headers)
         if response.status_code != 200:
             raise MFilesException(response.text)
         return response
```

### Comparing `mfiles-0.5.2/mfiles/definitions.py` & `mfiles-0.5.3/mfiles/definitions.py`

 * *Files identical despite different names*

### Comparing `mfiles-0.5.2/mfiles.egg-info/PKG-INFO` & `mfiles-0.5.3/mfiles.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: mfiles
-Version: 0.5.2
+Version: 0.5.3
 Summary: M-Files API wrapper
 Home-page: https://github.com/afcmrp/python-mfiles
 Author: Emil Hjelm
 Author-email: emil.hjelm@climeon.com
 License: MIT
 Description: 
         Python wrapper around the M-Files API.
```

### Comparing `mfiles-0.5.2/setup.py` & `mfiles-0.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Documentation: https://mfiles.readthedocs.io/en/latest/
 """
 
 setup(
     name='mfiles',
     packages=find_packages(),
-    version='0.5.2',
+    version='0.5.3',
     license='MIT',
     description='M-Files API wrapper',
     long_description=PYPI_DESCRIPTION,
     author='Emil Hjelm',
     author_email='emil.hjelm@climeon.com',
     url='https://github.com/afcmrp/python-mfiles',
     keywords=['M-Files', 'mfiles', 'REST', 'API'],
```

### Comparing `mfiles-0.5.2/test/local_test.py` & `mfiles-0.5.3/test/local_test.py`

 * *Files identical despite different names*

