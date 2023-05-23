# Comparing `tmp/InsightIDR4Py-0.2.tar.gz` & `tmp/InsightIDR4Py-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "InsightIDR4Py-0.2.tar", last modified: Mon May 22 18:25:03 2023, max compression
+gzip compressed data, was "InsightIDR4Py-0.3.tar", last modified: Tue May 23 21:28:50 2023, max compression
```

## Comparing `InsightIDR4Py-0.2.tar` & `InsightIDR4Py-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 18:25:03.122037 InsightIDR4Py-0.2/
-drwxrwxrwx   0        0        0        0 2023-05-22 18:25:03.122037 InsightIDR4Py-0.2/InsightIDR4Py.egg-info/
--rw-rw-rw-   0        0        0     5973 2023-05-22 18:25:03.000000 InsightIDR4Py-0.2/InsightIDR4Py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-05-22 18:25:03.000000 InsightIDR4Py-0.2/InsightIDR4Py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 18:25:03.000000 InsightIDR4Py-0.2/InsightIDR4Py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-22 18:25:03.000000 InsightIDR4Py-0.2/InsightIDR4Py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-22 18:25:03.000000 InsightIDR4Py-0.2/InsightIDR4Py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    23729 2023-05-22 18:17:07.000000 InsightIDR4Py-0.2/InsightIDR4Py.py
--rw-rw-rw-   0        0        0     1092 2023-05-22 16:57:04.000000 InsightIDR4Py-0.2/LICENSE
--rw-rw-rw-   0        0        0     5973 2023-05-22 18:25:03.122037 InsightIDR4Py-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5555 2023-05-22 17:35:51.000000 InsightIDR4Py-0.2/README.md
--rw-rw-rw-   0        0        0       99 2023-05-22 16:55:58.000000 InsightIDR4Py-0.2/pyproject.toml
--rw-rw-rw-   0        0        0      111 2023-05-22 18:25:03.123037 InsightIDR4Py-0.2/setup.cfg
--rw-rw-rw-   0        0        0      692 2023-05-22 18:22:40.000000 InsightIDR4Py-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 21:28:50.198984 InsightIDR4Py-0.3/
+drwxrwxrwx   0        0        0        0 2023-05-23 21:28:50.198984 InsightIDR4Py-0.3/InsightIDR4Py.egg-info/
+-rw-rw-rw-   0        0        0     6046 2023-05-23 21:28:49.000000 InsightIDR4Py-0.3/InsightIDR4Py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-05-23 21:28:50.000000 InsightIDR4Py-0.3/InsightIDR4Py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 21:28:49.000000 InsightIDR4Py-0.3/InsightIDR4Py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-23 21:28:49.000000 InsightIDR4Py-0.3/InsightIDR4Py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-23 21:28:49.000000 InsightIDR4Py-0.3/InsightIDR4Py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    25652 2023-05-23 21:22:05.000000 InsightIDR4Py-0.3/InsightIDR4Py.py
+-rw-rw-rw-   0        0        0     1092 2023-05-22 16:57:04.000000 InsightIDR4Py-0.3/LICENSE
+-rw-rw-rw-   0        0        0     6046 2023-05-23 21:28:50.207170 InsightIDR4Py-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5628 2023-05-23 21:27:27.000000 InsightIDR4Py-0.3/README.md
+-rw-rw-rw-   0        0        0       99 2023-05-22 16:55:58.000000 InsightIDR4Py-0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      111 2023-05-23 21:28:50.207170 InsightIDR4Py-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      692 2023-05-23 21:27:49.000000 InsightIDR4Py-0.3/setup.py
```

### Comparing `InsightIDR4Py-0.2/InsightIDR4Py.egg-info/PKG-INFO` & `InsightIDR4Py-0.3/InsightIDR4Py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InsightIDR4Py
-Version: 0.2
+Version: 0.3
 Summary: A Python client allowing simplified interaction with Rapid7's InsightIDR REST API.
 Home-page: https://github.com/mbabinski/InsightIDR4Py
 Author: Micah Babinski
 Author-email: m.babinski.88@gmail.com
 License: MIT
 Keywords: Rapid7,InsightIDR,SIEM,Logsearch,Investigations,Threats
 Description-Content-Type: text/markdown
@@ -20,14 +20,17 @@
 * List Investigations
 * Get an Investigation
 * Create Investigation
 * Close Investigations in Bulk
 * List Alerts by Investigation
 * List Rapid7 Product Alerts by Investigation
 * Update Investigation
+* List Comments on an Investigation
+* Create Comment
+* Delete Comment
 ## Threats
 * Create Threat
 * Add Indicators to Threat
 * Replace Threat Indicators
 * Delete Threat
 ## Saved Queries
 * List Saved Queries
```

### Comparing `InsightIDR4Py-0.2/InsightIDR4Py.py` & `InsightIDR4Py-0.3/InsightIDR4Py.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
             self.region = self._get_region()
         else:
             self.region = region
         self.logs_url = "https://{}.rest.logs.insight.rapid7.com/query/logs/".format(self.region)
         self.query_url = "https://{}.rest.logs.insight.rapid7.com/query/".format(self.region)
         self.log_mgmt_url = "https://{}.api.insight.rapid7.com/log_search/management/logs/".format(self.region)
         self.investigations_url = "https://{}.api.insight.rapid7.com/idr/v2/investigations/".format(self.region)
+        self.comments_url = "https://{}.api.insight.rapid7.com/idr/v1/comments/".format(self.region)
         self.threat_url = "https://{}.api.insight.rapid7.com/idr/v1/customthreats/".format(self.region)
 
     def _get_region(self):
         """
         This method cycles through available API regions, making a call to the log management URL with each
         region until a successful call indicates the correct region. If you already know your region, simply
         pass that in when creating the InsightIDR object.
@@ -382,14 +383,68 @@
         url = self.investigations_url + investigation_id
         self.session.headers["Accept-version"] = "investigations-preview"
         response = self.session.patch(url, json=data, params=params)
         result = response.json()
 
         return result
 
+    def ListCommentsByInvestigation(self, investigation_rrn):
+        """
+        Returns a list of comments filtered by a specific investigation with a given rrn.
+        """
+        comments = []
+        url = self.comments_url
+        params = {
+            "index": 0,
+            "size": 100,
+            "target": investigation_rrn
+        }
+        
+        # make initial request
+        self.session.headers["Accept-version"] = "comments-preview"
+        response = self.session.get(url, params=params)
+        result = response.json()
+        # get the total
+        total = result["metadata"]["total_data"]
+        # add the results to the output list
+        comments.extend(result["data"])
+        # iterate through remaining alerts and add them to the output list
+        while len(comments) < total:
+            params["index"] += 100
+            response = self.session.get(url, params)
+            result = response.json()
+            comments.extend(result["data"])
+
+        return comments
+
+    def CreateComment(self, investigation_rrn, comment_text):
+        """
+        Creates a comment on an investigation.
+        """
+        data = {
+            "attachments": [], # attachments not yet supported
+            "body": comment_text,
+            "target": investigation_rrn
+        }
+        url = self.comments_url
+        self.session.headers["Accept-version"] = "comments-preview"
+        response = self.session.post(url, json=data)
+        result = response.json()
+
+        return result
+
+    def DeleteComment(self, comment_rrn):
+        """
+        Deletes a comment identified by its rrn value.
+        """
+        url = self.comments_url + "{}".format(comment_rrn)
+        response = self.session.delete(url)
+
+        return response
+
     def CreateThreat(self, threat_name, threat_description, indicators={}):
         """
         CreateS a private InsightIDR Community Threat and optionally adds indicators to this Community Threat.
         Indicator types can include IP addresses, hashes, domain names, or URLs.
         """
         data = {
             "threat": threat_name,
```

### Comparing `InsightIDR4Py-0.2/LICENSE` & `InsightIDR4Py-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `InsightIDR4Py-0.2/PKG-INFO` & `InsightIDR4Py-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InsightIDR4Py
-Version: 0.2
+Version: 0.3
 Summary: A Python client allowing simplified interaction with Rapid7's InsightIDR REST API.
 Home-page: https://github.com/mbabinski/InsightIDR4Py
 Author: Micah Babinski
 Author-email: m.babinski.88@gmail.com
 License: MIT
 Keywords: Rapid7,InsightIDR,SIEM,Logsearch,Investigations,Threats
 Description-Content-Type: text/markdown
@@ -20,14 +20,17 @@
 * List Investigations
 * Get an Investigation
 * Create Investigation
 * Close Investigations in Bulk
 * List Alerts by Investigation
 * List Rapid7 Product Alerts by Investigation
 * Update Investigation
+* List Comments on an Investigation
+* Create Comment
+* Delete Comment
 ## Threats
 * Create Threat
 * Add Indicators to Threat
 * Replace Threat Indicators
 * Delete Threat
 ## Saved Queries
 * List Saved Queries
```

### Comparing `InsightIDR4Py-0.2/README.md` & `InsightIDR4Py-0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 * List Investigations
 * Get an Investigation
 * Create Investigation
 * Close Investigations in Bulk
 * List Alerts by Investigation
 * List Rapid7 Product Alerts by Investigation
 * Update Investigation
+* List Comments on an Investigation
+* Create Comment
+* Delete Comment
 ## Threats
 * Create Threat
 * Add Indicators to Threat
 * Replace Threat Indicators
 * Delete Threat
 ## Saved Queries
 * List Saved Queries
```

### Comparing `InsightIDR4Py-0.2/setup.py` & `InsightIDR4Py-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="InsightIDR4Py",
-    version="0.2",
+    version="0.3",
     description="A Python client allowing simplified interaction with Rapid7's InsightIDR REST API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     author="Micah Babinski",
     author_email="m.babinski.88@gmail.com",
     py_modules=["InsightIDR4Py"],
```

