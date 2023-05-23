# Comparing `tmp/ud3tn-utils-0.12.0.tar.gz` & `tmp/ud3tn-utils-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ud3tn-utils-0.12.0.tar", last modified: Tue May 23 11:30:56 2023, max compression
+gzip compressed data, was "dist/ud3tn-utils-0.9.0.tar", last modified: Thu Nov 19 17:51:04 2020, max compression
```

## Comparing `ud3tn-utils-0.12.0.tar` & `ud3tn-utils-0.9.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 fw        (1000) users      (100)        0 2023-05-23 11:30:56.434011 ud3tn-utils-0.12.0/
--rw-r--r--   0 fw        (1000) users      (100)     1592 2022-01-22 13:20:17.000000 ud3tn-utils-0.12.0/LICENSE
--rw-r--r--   0 fw        (1000) users      (100)     1364 2023-05-23 11:30:56.434011 ud3tn-utils-0.12.0/PKG-INFO
--rw-r--r--   0 fw        (1000) users      (100)     1106 2022-01-22 13:20:17.000000 ud3tn-utils-0.12.0/README.md
--rw-r--r--   0 fw        (1000) users      (100)       38 2023-05-23 11:30:56.434011 ud3tn-utils-0.12.0/setup.cfg
--rw-r--r--   0 fw        (1000) users      (100)      541 2023-05-23 11:13:23.000000 ud3tn-utils-0.12.0/setup.py
-drwxr-xr-x   0 fw        (1000) users      (100)        0 2023-05-23 11:30:56.430678 ud3tn-utils-0.12.0/ud3tn_utils/
--rw-r--r--   0 fw        (1000) users      (100)      142 2022-12-21 15:21:24.000000 ud3tn-utils-0.12.0/ud3tn_utils/__init__.py
-drwxr-xr-x   0 fw        (1000) users      (100)        0 2023-05-23 11:30:56.434011 ud3tn-utils-0.12.0/ud3tn_utils/aap/
--rw-r--r--   0 fw        (1000) users      (100)      339 2022-12-21 15:21:24.000000 ud3tn-utils-0.12.0/ud3tn_utils/aap/__init__.py
--rw-r--r--   0 fw        (1000) users      (100)     7711 2023-05-16 09:34:14.000000 ud3tn-utils-0.12.0/ud3tn_utils/aap/aap_client.py
--rw-r--r--   0 fw        (1000) users      (100)     6906 2023-05-16 09:34:14.000000 ud3tn-utils-0.12.0/ud3tn_utils/aap/aap_message.py
--rw-r--r--   0 fw        (1000) users      (100)     4213 2023-05-16 09:34:14.000000 ud3tn-utils-0.12.0/ud3tn_utils/config.py
-drwxr-xr-x   0 fw        (1000) users      (100)        0 2023-05-23 11:30:56.434011 ud3tn-utils-0.12.0/ud3tn_utils.egg-info/
--rw-r--r--   0 fw        (1000) users      (100)     1364 2023-05-23 11:30:56.000000 ud3tn-utils-0.12.0/ud3tn_utils.egg-info/PKG-INFO
--rw-r--r--   0 fw        (1000) users      (100)      301 2023-05-23 11:30:56.000000 ud3tn-utils-0.12.0/ud3tn_utils.egg-info/SOURCES.txt
--rw-r--r--   0 fw        (1000) users      (100)        1 2023-05-23 11:30:56.000000 ud3tn-utils-0.12.0/ud3tn_utils.egg-info/dependency_links.txt
--rw-r--r--   0 fw        (1000) users      (100)       12 2023-05-23 11:30:56.000000 ud3tn-utils-0.12.0/ud3tn_utils.egg-info/top_level.txt
+drwxr-xr-x   0 fw        (1000) users      (100)        0 2020-11-19 17:51:04.156736 ud3tn-utils-0.9.0/
+-rw-r--r--   0 fw        (1000) users      (100)     1741 2020-11-19 17:51:04.156736 ud3tn-utils-0.9.0/PKG-INFO
+-rw-r--r--   0 fw        (1000) users      (100)     1106 2020-11-19 12:00:37.000000 ud3tn-utils-0.9.0/README.md
+-rw-r--r--   0 fw        (1000) users      (100)       38 2020-11-19 17:51:04.156736 ud3tn-utils-0.9.0/setup.cfg
+-rw-r--r--   0 fw        (1000) users      (100)      486 2020-11-19 17:39:47.000000 ud3tn-utils-0.9.0/setup.py
+drwxr-xr-x   0 fw        (1000) users      (100)        0 2020-11-19 17:51:04.156736 ud3tn-utils-0.9.0/ud3tn_utils/
+-rw-r--r--   0 fw        (1000) users      (100)       88 2020-11-19 12:00:37.000000 ud3tn-utils-0.9.0/ud3tn_utils/__init__.py
+drwxr-xr-x   0 fw        (1000) users      (100)        0 2020-11-19 17:51:04.156736 ud3tn-utils-0.9.0/ud3tn_utils/aap/
+-rw-r--r--   0 fw        (1000) users      (100)      285 2020-11-19 12:00:37.000000 ud3tn-utils-0.9.0/ud3tn_utils/aap/__init__.py
+-rw-r--r--   0 fw        (1000) users      (100)     5477 2020-11-19 12:00:37.000000 ud3tn-utils-0.9.0/ud3tn_utils/aap/aap_client.py
+-rw-r--r--   0 fw        (1000) users      (100)     4509 2020-11-19 12:00:37.000000 ud3tn-utils-0.9.0/ud3tn_utils/aap/aap_message.py
+-rw-r--r--   0 fw        (1000) users      (100)     4117 2020-11-19 12:00:37.000000 ud3tn-utils-0.9.0/ud3tn_utils/config.py
+drwxr-xr-x   0 fw        (1000) users      (100)        0 2020-11-19 17:51:04.156736 ud3tn-utils-0.9.0/ud3tn_utils.egg-info/
+-rw-r--r--   0 fw        (1000) users      (100)     1741 2020-11-19 17:51:04.000000 ud3tn-utils-0.9.0/ud3tn_utils.egg-info/PKG-INFO
+-rw-r--r--   0 fw        (1000) users      (100)      293 2020-11-19 17:51:04.000000 ud3tn-utils-0.9.0/ud3tn_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 fw        (1000) users      (100)        1 2020-11-19 17:51:04.000000 ud3tn-utils-0.9.0/ud3tn_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 fw        (1000) users      (100)       12 2020-11-19 17:51:04.000000 ud3tn-utils-0.9.0/ud3tn_utils.egg-info/top_level.txt
```

### Comparing `ud3tn-utils-0.12.0/PKG-INFO` & `ud3tn-utils-0.9.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: ud3tn-utils
-Version: 0.12.0
-Summary: μD3TN Utilities
-Home-page: https://gitlab.com/d3tn/ud3tn
-Author: D3TN GmbH
-Author-email: contact@d3tn.com
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # python-uD3TN-utils
 
 The Python package uD3TN-utils is a utility library to simplify the interaction
 with the uD3TN daemon within python applications.
 
 The included `AAPClient` enables user-friendly communication with the uD3TN
 daemon via local or remote sockets using the Application Agent Protocol (AAP).
```

### Comparing `ud3tn-utils-0.12.0/ud3tn_utils/config.py` & `ud3tn-utils-0.9.0/ud3tn_utils/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# SPDX-License-Identifier: BSD-3-Clause OR Apache-2.0
 import enum
 import time
 import struct
 
 from collections import namedtuple
 from datetime import datetime, timezone
 
@@ -35,25 +34,25 @@
 
 Contact = namedtuple('Contact', ['start', 'end', 'bitrate'])
 Contact.__doc__ = """named tuple holding uD3TN contact information
 
 Attrs:
     start (int): DTN timestamp when the contact starts
     end (int): DTN timestamp when the contact is over
-    bitrate (int): Bitrate of the contact, in bytes per second
+    bitrate (int): Bitrate of the contact
 """
 
 
 def make_contact(start_offset, duration, bitrate):
     """Create a :class:`Contact` tuple relative to the current time
 
     Args:
         start_offset (int): Start point of the contact from in seconds from now
         duration (int): Duration of the contact in seconds
-        bitrate (int): Bitrate of the contact, in bytes per second
+        bitrate (int): Bitrate of the contact
     Returns:
         Contact: contact tuple with DTN timestamps
     """
     cur_time = time.time()
     start = unix2dtn(cur_time + start_offset)
 
     return Contact(
```

### Comparing `ud3tn-utils-0.12.0/ud3tn_utils.egg-info/PKG-INFO` & `ud3tn-utils-0.9.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 Metadata-Version: 2.1
 Name: ud3tn-utils
-Version: 0.12.0
+Version: 0.9.0
 Summary: μD3TN Utilities
 Home-page: https://gitlab.com/d3tn/ud3tn
 Author: D3TN GmbH
 Author-email: contact@d3tn.com
+License: UNKNOWN
+Description: # python-uD3TN-utils
+        
+        The Python package uD3TN-utils is a utility library to simplify the interaction
+        with the uD3TN daemon within python applications.
+        
+        The included `AAPClient` enables user-friendly communication with the uD3TN
+        daemon via local or remote sockets using the Application Agent Protocol (AAP).
+        Besides sending and receiving bundles, it is also possible to change the
+        configuration of the uD3TN daemon via AAP messages.
+        
+        ## Installation
+        
+        From source:
+        
+        ```sh
+        git clone https://gitlab.com/d3tn/ud3tn
+        cd python-ud3tn-utils
+        python setup.py install
+        ```
+        
+        From [PyPi](https://pypi.org/project/ud3tn-utils) directly:
+        
+        ```sh
+        pip install ud3tn-utils
+        ```
+        
+        ## Examples
+        
+        ```python
+        from ud3tn_utils.aap import AAPUnixClient
+        
+        with AAPUnixClient() as aap_client:
+            aap_client.register()
+            aap_client.send_str(aap_client.eid(), "Hello World")
+            print(aap_client.receive())
+        ```
+        
+        ## Development
+        
+        pyD3TN is maintained as part of the µD3TN project and follows its development
+        processes. Please see the [µD3TN][ud3tn] repository for the code and further
+        information.
+        
+        [ud3tn]: https://gitlab.com/d3tn/ud3tn
+        
+Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# python-uD3TN-utils
-
-The Python package uD3TN-utils is a utility library to simplify the interaction
-with the uD3TN daemon within python applications.
-
-The included `AAPClient` enables user-friendly communication with the uD3TN
-daemon via local or remote sockets using the Application Agent Protocol (AAP).
-Besides sending and receiving bundles, it is also possible to change the
-configuration of the uD3TN daemon via AAP messages.
-
-## Installation
-
-From source:
-
-```sh
-git clone https://gitlab.com/d3tn/ud3tn
-cd python-ud3tn-utils
-python setup.py install
-```
-
-From [PyPi](https://pypi.org/project/ud3tn-utils) directly:
-
-```sh
-pip install ud3tn-utils
-```
-
-## Examples
-
-```python
-from ud3tn_utils.aap import AAPUnixClient
-
-with AAPUnixClient() as aap_client:
-    aap_client.register()
-    aap_client.send_str(aap_client.eid(), "Hello World")
-    print(aap_client.receive())
-```
-
-## Development
-
-pyD3TN is maintained as part of the µD3TN project and follows its development
-processes. Please see the [µD3TN][ud3tn] repository for the code and further
-information.
-
-[ud3tn]: https://gitlab.com/d3tn/ud3tn
```

