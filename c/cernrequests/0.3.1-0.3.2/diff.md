# Comparing `tmp/cernrequests-0.3.1.tar.gz` & `tmp/cernrequests-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cernrequests-0.3.1.tar", last modified: Wed Aug 24 17:39:50 2022, max compression
+gzip compressed data, was "cernrequests-0.3.2.tar", last modified: Tue May 23 17:01:46 2023, max compression
```

## Comparing `cernrequests-0.3.1.tar` & `cernrequests-0.3.2.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxrwxr-x   0 mpliax    (1001) mpliax    (1001)        0 2022-08-24 17:39:50.002128 cernrequests-0.3.1/
--rw-rw-r--   0 mpliax    (1001) mpliax    (1001)     7651 2022-08-24 16:11:49.000000 cernrequests-0.3.1/LICENSE
--rw-rw-r--   0 mpliax    (1001) mpliax    (1001)     3778 2022-08-24 17:39:50.002128 cernrequests-0.3.1/PKG-INFO
--rw-rw-r--   0 mpliax    (1001) mpliax    (1001)     3471 2022-08-24 16:11:49.000000 cernrequests-0.3.1/README.md
-drwxrwxr-x   0 mpliax    (1001) mpliax    (1001)        0 2022-08-24 17:39:50.002128 cernrequests-0.3.1/cernrequests/
--rw-rw-r--   0 mpliax    (1001) mpliax    (1001)      487 2022-08-24 16:11:49.000000 cernrequests-0.3.1/cernrequests/__init__.py
--rw-rw-r--   0 mpliax    (1001) mpliax    (1001)     6858 2022-08-24 17:36:54.000000 cernrequests-0.3.1/cernrequests/cern-cacert.pem
--rw-rw-r--   0 mpliax    (1001) mpliax    (1001)     2718 2022-08-24 16:11:49.000000 cernrequests-0.3.1/cernrequests/certs.py
--rw-rw-r--   0 mpliax    (1001) mpliax    (1001)     2479 2022-08-24 16:11:49.000000 cernrequests-0.3.1/cernrequests/cookies.py
--rw-rw-r--   0 mpliax    (1001) mpliax    (1001)      760 2022-08-24 16:11:49.000000 cernrequests-0.3.1/cernrequests/core.py
-drwxrwxr-x   0 mpliax    (1001) mpliax    (1001)        0 2022-08-24 17:39:50.002128 cernrequests-0.3.1/cernrequests.egg-info/
--rw-rw-r--   0 mpliax    (1001) mpliax    (1001)     3778 2022-08-24 17:39:49.000000 cernrequests-0.3.1/cernrequests.egg-info/PKG-INFO
--rw-rw-r--   0 mpliax    (1001) mpliax    (1001)      326 2022-08-24 17:39:49.000000 cernrequests-0.3.1/cernrequests.egg-info/SOURCES.txt
--rw-rw-r--   0 mpliax    (1001) mpliax    (1001)        1 2022-08-24 17:39:49.000000 cernrequests-0.3.1/cernrequests.egg-info/dependency_links.txt
--rw-rw-r--   0 mpliax    (1001) mpliax    (1001)       16 2022-08-24 17:39:49.000000 cernrequests-0.3.1/cernrequests.egg-info/requires.txt
--rw-rw-r--   0 mpliax    (1001) mpliax    (1001)       13 2022-08-24 17:39:49.000000 cernrequests-0.3.1/cernrequests.egg-info/top_level.txt
--rw-rw-r--   0 mpliax    (1001) mpliax    (1001)       38 2022-08-24 17:39:50.002128 cernrequests-0.3.1/setup.cfg
--rw-rw-r--   0 mpliax    (1001) mpliax    (1001)     1222 2022-08-24 17:36:54.000000 cernrequests-0.3.1/setup.py
+drwxrwxr-x   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2023-05-23 17:01:46.006574 cernrequests-0.3.2/
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     7651 2023-05-23 15:59:26.000000 cernrequests-0.3.2/LICENSE
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     4495 2023-05-23 17:01:46.006574 cernrequests-0.3.2/PKG-INFO
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     4188 2023-05-23 16:53:33.000000 cernrequests-0.3.2/README.md
+drwxrwxr-x   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2023-05-23 17:01:46.002574 cernrequests-0.3.2/cernrequests/
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)      487 2023-05-23 15:59:26.000000 cernrequests-0.3.2/cernrequests/__init__.py
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)    14605 2023-05-23 16:47:13.000000 cernrequests-0.3.2/cernrequests/cern-cacert.pem
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     2718 2023-05-23 15:59:26.000000 cernrequests-0.3.2/cernrequests/certs.py
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     2479 2023-05-23 15:59:26.000000 cernrequests-0.3.2/cernrequests/cookies.py
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)      760 2023-05-23 15:59:26.000000 cernrequests-0.3.2/cernrequests/core.py
+drwxrwxr-x   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2023-05-23 17:01:46.006574 cernrequests-0.3.2/cernrequests.egg-info/
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     4495 2023-05-23 17:01:45.000000 cernrequests-0.3.2/cernrequests.egg-info/PKG-INFO
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)      377 2023-05-23 17:01:45.000000 cernrequests-0.3.2/cernrequests.egg-info/SOURCES.txt
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)        1 2023-05-23 17:01:45.000000 cernrequests-0.3.2/cernrequests.egg-info/dependency_links.txt
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)       16 2023-05-23 17:01:45.000000 cernrequests-0.3.2/cernrequests.egg-info/requires.txt
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)       13 2023-05-23 17:01:45.000000 cernrequests-0.3.2/cernrequests.egg-info/top_level.txt
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)       38 2023-05-23 17:01:46.006574 cernrequests-0.3.2/setup.cfg
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     1222 2023-05-23 16:47:13.000000 cernrequests-0.3.2/setup.py
+drwxrwxr-x   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2023-05-23 17:01:46.006574 cernrequests-0.3.2/tests/
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     1335 2023-05-23 15:59:26.000000 cernrequests-0.3.2/tests/test_cernrequests.py
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     1515 2023-05-23 16:18:02.000000 cernrequests-0.3.2/tests/test_real_data.py
```

### Comparing `cernrequests-0.3.1/LICENSE` & `cernrequests-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cernrequests-0.3.1/PKG-INFO` & `cernrequests-0.3.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: cernrequests
-Version: 0.3.1
-Home-page: https://github.com/CMSTrackerDPG/cernrequests
-Author: Peter Stein
-Author-email: peter.stein@cern.ch
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Build Status](https://travis-ci.com/CMSTrackerDPG/cernrequests.svg?branch=master)](https://travis-ci.com/CMSTrackerDPG/cernrequests)
 [![](https://img.shields.io/pypi/v/cernrequests.svg)](https://pypi.org/project/cernrequests/)
 
 
 # CERN Requests
 
 Enables using [requests]("https://github.com/requests/requests") without having to configure the CERN Root certificates.
@@ -104,14 +94,35 @@
 key = "my/custom/path/key.pem"      # Private key path
 
 cernrequests.get(url, cert=(cert,key))
 ```
 
 This way you can even use custom names such as ```cert.pem``` and ```key.pem```
 
+## Testing
+
+```bash
+python -m venv venv
+source venv/bin/activate
+pip install -r testing-requirements.txt
+pytest
+```
+
+## FAQ
+
+### I'm getting `certificate verify failed`! What should I do?
+
+The `cernrequests/cern-cacerts.pem` file has expired, and will need to be updated by the library maintainer. Download all the CA files from [here](https://ca.cern.ch/cafiles/certificates/Download.aspx?ca=cern) and convert them to `.pem` files, one-by-one by running:
+
+```bash
+ openssl x509 -in <CERN certification authority file.crt> -out temp.pem -outform PEM
+```
+
+Then, merge the contents of each `.pem` file into a single `cern-cacerts.pem` file and replace the existing one. Verify that the certs work by running `pytest`.
+
 ## References
 
 - http://docs.python-requests.org/en/master/
 - https://certifi.io/en/latest/
 - https://github.com/cerndb/cern-sso-python
 - https://linux.web.cern.ch/linux/docs/cernssocookie.shtml
 - http://linuxsoft.cern.ch/cern/centos/7/cern/x86_64/repoview/CERN-CA-certs.html
```

### Comparing `cernrequests-0.3.1/cernrequests/certs.py` & `cernrequests-0.3.2/cernrequests/certs.py`

 * *Files identical despite different names*

### Comparing `cernrequests-0.3.1/cernrequests/cookies.py` & `cernrequests-0.3.2/cernrequests/cookies.py`

 * *Files identical despite different names*

### Comparing `cernrequests-0.3.1/cernrequests/core.py` & `cernrequests-0.3.2/cernrequests/core.py`

 * *Files identical despite different names*

### Comparing `cernrequests-0.3.1/cernrequests.egg-info/PKG-INFO` & `cernrequests-0.3.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cernrequests
-Version: 0.3.1
+Version: 0.3.2
 Home-page: https://github.com/CMSTrackerDPG/cernrequests
 Author: Peter Stein
 Author-email: peter.stein@cern.ch
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -104,14 +104,35 @@
 key = "my/custom/path/key.pem"      # Private key path
 
 cernrequests.get(url, cert=(cert,key))
 ```
 
 This way you can even use custom names such as ```cert.pem``` and ```key.pem```
 
+## Testing
+
+```bash
+python -m venv venv
+source venv/bin/activate
+pip install -r testing-requirements.txt
+pytest
+```
+
+## FAQ
+
+### I'm getting `certificate verify failed`! What should I do?
+
+The `cernrequests/cern-cacerts.pem` file has expired, and will need to be updated by the library maintainer. Download all the CA files from [here](https://ca.cern.ch/cafiles/certificates/Download.aspx?ca=cern) and convert them to `.pem` files, one-by-one by running:
+
+```bash
+ openssl x509 -in <CERN certification authority file.crt> -out temp.pem -outform PEM
+```
+
+Then, merge the contents of each `.pem` file into a single `cern-cacerts.pem` file and replace the existing one. Verify that the certs work by running `pytest`.
+
 ## References
 
 - http://docs.python-requests.org/en/master/
 - https://certifi.io/en/latest/
 - https://github.com/cerndb/cern-sso-python
 - https://linux.web.cern.ch/linux/docs/cernssocookie.shtml
 - http://linuxsoft.cern.ch/cern/centos/7/cern/x86_64/repoview/CERN-CA-certs.html
```

### Comparing `cernrequests-0.3.1/setup.py` & `cernrequests-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 setup(
     name="cernrequests",
-    version="0.3.1",
+    version="0.3.2",
     desription="CERN wrapper around the requests package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/CMSTrackerDPG/cernrequests",
     author="Peter Stein",
     author_email="peter.stein@cern.ch",
     packages=["cernrequests"],
```

