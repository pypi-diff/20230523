# Comparing `tmp/igdb-api-v4-0.1.0.tar.gz` & `tmp/igdb-api-v4-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "igdb-api-v4-0.1.0.tar", last modified: Tue Nov 22 15:28:51 2022, max compression
+gzip compressed data, was "igdb-api-v4-0.2.0.tar", last modified: Tue May 23 11:35:01 2023, max compression
```

## Comparing `igdb-api-v4-0.1.0.tar` & `igdb-api-v4-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 15:28:51.365659 igdb-api-v4-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-11-22 15:28:28.000000 igdb-api-v4-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5162 2022-11-22 15:28:51.365659 igdb-api-v4-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3827 2022-11-22 15:28:28.000000 igdb-api-v4-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 15:28:51.365659 igdb-api-v4-0.1.0/igdb_api_v4.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5162 2022-11-22 15:28:51.000000 igdb-api-v4-0.1.0/igdb_api_v4.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-11-22 15:28:51.000000 igdb-api-v4-0.1.0/igdb_api_v4.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-22 15:28:51.000000 igdb-api-v4-0.1.0/igdb_api_v4.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-22 15:28:51.000000 igdb-api-v4-0.1.0/igdb_api_v4.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-11-22 15:28:51.000000 igdb-api-v4-0.1.0/igdb_api_v4.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-22 15:28:51.365659 igdb-api-v4-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      673 2022-11-22 15:28:28.000000 igdb-api-v4-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 15:28:51.365659 igdb-api-v4-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 15:28:51.365659 igdb-api-v4-0.1.0/src/igdb/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-22 15:28:28.000000 igdb-api-v4-0.1.0/src/igdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   366292 2022-11-22 15:28:28.000000 igdb-api-v4-0.1.0/src/igdb/igdbapi_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     1474 2022-11-22 15:28:28.000000 igdb-api-v4-0.1.0/src/igdb/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:35:01.402211 igdb-api-v4-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-23 11:34:30.000000 igdb-api-v4-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-05-23 11:35:01.402211 igdb-api-v4-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-05-23 11:34:30.000000 igdb-api-v4-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:35:01.398211 igdb-api-v4-0.2.0/igdb_api_v4.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-05-23 11:35:01.000000 igdb-api-v4-0.2.0/igdb_api_v4.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-23 11:35:01.000000 igdb-api-v4-0.2.0/igdb_api_v4.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 11:35:01.000000 igdb-api-v4-0.2.0/igdb_api_v4.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 11:35:01.000000 igdb-api-v4-0.2.0/igdb_api_v4.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-23 11:35:01.000000 igdb-api-v4-0.2.0/igdb_api_v4.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 11:35:01.402211 igdb-api-v4-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-23 11:34:30.000000 igdb-api-v4-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:35:01.398211 igdb-api-v4-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:35:01.402211 igdb-api-v4-0.2.0/src/igdb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:34:30.000000 igdb-api-v4-0.2.0/src/igdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47788 2023-05-23 11:34:30.000000 igdb-api-v4-0.2.0/src/igdb/igdbapi_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-23 11:34:30.000000 igdb-api-v4-0.2.0/src/igdb/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:35:01.402211 igdb-api-v4-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-23 11:34:30.000000 igdb-api-v4-0.2.0/tests/test_wrapper.py
```

### Comparing `igdb-api-v4-0.1.0/LICENSE` & `igdb-api-v4-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `igdb-api-v4-0.1.0/PKG-INFO` & `igdb-api-v4-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,126 +1,125 @@
 Metadata-Version: 2.1
 Name: igdb-api-v4
-Version: 0.1.0
+Version: 0.2.0
 Summary: An API wrapper for IGDB API v4
 Home-page: https://github.com/twitchtv/igdb-api-python/
 Author: IGDB
 Author-email: dev@igdb.com
-License: UNKNOWN
-Description: # IGDB Python API V4
-        A Python wrapper for IGDB.com's Video Game Database API. 
-        
-        __IMPORTANT__
-        
-        This wrapper is ONLY compatible with the newest release (V4).
-        
-        ## About IGDB
-        One of the principles behind IGDB.com is accessibility of data. We wish to share the data with anyone who wants to build cool video game oriented websites, apps and services. This means that the information you contribute to IGDB.com can be used by other projects as well.
-        
-        Thus, you are not only contributing to the value of this site but to thousands of other projects as well. We are looking forward to see what exciting game related projects you come up with. Happy coding!
-        
-        More info here:
-        * [About the API](https://www.igdb.com/api)
-        * [API Documentation](https://api-docs.igdb.com/)
-        
-        Information about the Querying language APICalypse:
-        * [apicalypse.io](https://apicalypse.io/)
-        
-        ## About the Wrapper
-        
-        The Wrapper can handle both the IGDB generated classes and JSON (Strings), I have chosen to make the API's Generated classes ([Protocol Buffers](https://developers.google.com/protocol-buffers/)) the standard way because it will make it easier to use as you don't have to create your own classes to hold the information.
-        
-        The package contains two modules: the `wrapper` which holds the tools for querying the API, and `igdbapi_pb2` which contains all of the generated classes for the Protocol Buffers.
-        
-        # Installation and Setup
-        
-        ```py
-        pip install igdb-api-v4
-        ```
-        
-        # Usage
-        
-        ## Using your Twitch Credentials
-        
-        Create a new IGDBWrapper object and give it your Client-ID and App Access Token:
-        
-        ```py
-        from igdb.wrapper import IGDBWrapper
-        wrapper = IGDBWrapper("YOUR_CLIENT_ID", "YOUR_APP_ACCESS_TOKEN")
-        ```
-        
-        ## How to use the wrapper
-        
-        Right now, the wrapper is very barebone and only has one wrapping function `api_request`, which queries the API when given an endpoint and an `APICalypse`-like query and returns a byte array with the results.
-        
-        More utilities will be added in the future, such as endpoint helper functions, JSON conversion, and Protobuf message parsing.
-        
-        * `api_request`
-          This method handles IGDB generated proto classes which returns an `ByteArray` to be used to fill the appropriate class.
-        ```py
-        '''With a wrapper instance already created'''
-        # JSON API request
-        byte_array = wrapper.api_request(
-                    'games',
-                    'fields id, name; offset 0; where platforms=48;'
-                  )
-        # parse into JSON however you like...
-        
-        # Protobuf API request
-        from igdb.igdbapi_pb2 import GameResult
-        byte_array = wrapper.api_request(
-                    'games.pb', # Note the '.pb' suffix at the endpoint
-                    'fields id, name; offset 0; where platforms=48;'
-                  )
-        games_message = GameResult()
-        games_message.ParseFromString(byte_array) # Fills the protobuf message object with the response
-        ```
-        
-        ## Exceptions
-        
-        The wrapper throws a [`requests.HTTPError`](https://2.python-requests.org/en/master/api/#requests.HTTPError) when an exception occurs from the API.
-        
-        ## Code Examples
-        
-        # Contributing / Developers
-        
-        ## Setup
-        ### Python
-        This project uses Python 3.7+ and pipenv to manage dependencies.
-        ```
-        pip install --user pipenv
-        pipenv install --dev
-        ```
-        
-        ### Protocol Buffers
-        
-        If you want to update the library to use the latest Protobuf file from api.igdb.com you can run ./update-protobuf.sh
-        
-        #### Windows
-        This project uses [protoc](https://github.com/protocolbuffers/protobuf/releases) to generate the protocol buffer wrapper.
-        ```
-        set PB_REL="https://github.com/protocolbuffers/protobuf/releases"
-        set PB_VERSION=3.13.0
-        set PB_OS=win
-        set PB_ARCH=64
-        curl -LO %PB_REL%/download/v%PB_VERSION%/protoc-%PB_VERSION%-%PB_OS%%PB_ARCH%.zip
-        ```
-        
-        Unzip to a protoc folder.
-        ```
-        cd protoc-3.13.0-win64\bin
-        protoc.exe -I=../../src/igdb --python_out=../../src/igdb igdbapi.proto
-        ```
-        
-        
-        ### Mac
-        Then run protoc:
-        ```
-        protoc -I=. --python_out=. igdbapi.proto
-        ```
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# IGDB Python API V4
+A Python wrapper for IGDB.com's Video Game Database API. 
+
+__IMPORTANT__
+
+This wrapper is ONLY compatible with the newest release (V4).
+
+## About IGDB
+One of the principles behind IGDB.com is accessibility of data. We wish to share the data with anyone who wants to build cool video game oriented websites, apps and services. This means that the information you contribute to IGDB.com can be used by other projects as well.
+
+Thus, you are not only contributing to the value of this site but to thousands of other projects as well. We are looking forward to see what exciting game related projects you come up with. Happy coding!
+
+More info here:
+* [About the API](https://www.igdb.com/api)
+* [API Documentation](https://api-docs.igdb.com/)
+
+Information about the Querying language APICalypse:
+* [apicalypse.io](https://apicalypse.io/)
+
+## About the Wrapper
+
+The Wrapper can handle both the IGDB generated classes and JSON (Strings), I have chosen to make the API's Generated classes ([Protocol Buffers](https://developers.google.com/protocol-buffers/)) the standard way because it will make it easier to use as you don't have to create your own classes to hold the information.
+
+The package contains two modules: the `wrapper` which holds the tools for querying the API, and `igdbapi_pb2` which contains all of the generated classes for the Protocol Buffers.
+
+# Installation and Setup
+
+```py
+pip install igdb-api-v4
+```
+
+# Usage
+
+## Using your Twitch Credentials
+
+Create a new IGDBWrapper object and give it your Client-ID and App Access Token:
+
+```py
+from igdb.wrapper import IGDBWrapper
+wrapper = IGDBWrapper("YOUR_CLIENT_ID", "YOUR_APP_ACCESS_TOKEN")
+```
+
+## How to use the wrapper
+
+Right now, the wrapper is very barebone and only has one wrapping function `api_request`, which queries the API when given an endpoint and an `APICalypse`-like query and returns a byte array with the results.
+
+More utilities will be added in the future, such as endpoint helper functions, JSON conversion, and Protobuf message parsing.
+
+* `api_request`
+  This method handles IGDB generated proto classes which returns an `ByteArray` to be used to fill the appropriate class.
+```py
+'''With a wrapper instance already created'''
+# JSON API request
+byte_array = wrapper.api_request(
+            'games',
+            'fields id, name; offset 0; where platforms=48;'
+          )
+# parse into JSON however you like...
+
+# Protobuf API request
+from igdb.igdbapi_pb2 import GameResult
+byte_array = wrapper.api_request(
+            'games.pb', # Note the '.pb' suffix at the endpoint
+            'fields id, name; offset 0; where platforms=48;'
+          )
+games_message = GameResult()
+games_message.ParseFromString(byte_array) # Fills the protobuf message object with the response
+```
+
+## Exceptions
+
+The wrapper throws a [`requests.HTTPError`](https://2.python-requests.org/en/master/api/#requests.HTTPError) when an exception occurs from the API.
+
+## Code Examples
+
+# Contributing / Developers
+
+## Setup
+### Python
+This project uses Python 3.7+ and pipenv to manage dependencies.
+```
+pip install --user pipenv
+pipenv install --dev
+```
+
+### Protocol Buffers
+
+If you want to update the library to use the latest Protobuf file from api.igdb.com you can run ./update-protobuf.sh
+
+#### Windows
+This project uses [protoc](https://github.com/protocolbuffers/protobuf/releases) to generate the protocol buffer wrapper.
+```
+set PB_REL="https://github.com/protocolbuffers/protobuf/releases"
+set PB_VERSION=3.13.0
+set PB_OS=win
+set PB_ARCH=64
+curl -LO %PB_REL%/download/v%PB_VERSION%/protoc-%PB_VERSION%-%PB_OS%%PB_ARCH%.zip
+```
+
+Unzip to a protoc folder.
+```
+cd protoc-3.13.0-win64\bin
+protoc.exe -I=../../src/igdb --python_out=../../src/igdb igdbapi.proto
+```
+
+
+### Mac
+Then run protoc:
+```
+protoc -I=. --python_out=. igdbapi.proto
+```
```

### Comparing `igdb-api-v4-0.1.0/README.md` & `igdb-api-v4-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `igdb-api-v4-0.1.0/igdb_api_v4.egg-info/PKG-INFO` & `igdb-api-v4-0.2.0/igdb_api_v4.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,126 +1,125 @@
 Metadata-Version: 2.1
 Name: igdb-api-v4
-Version: 0.1.0
+Version: 0.2.0
 Summary: An API wrapper for IGDB API v4
 Home-page: https://github.com/twitchtv/igdb-api-python/
 Author: IGDB
 Author-email: dev@igdb.com
-License: UNKNOWN
-Description: # IGDB Python API V4
-        A Python wrapper for IGDB.com's Video Game Database API. 
-        
-        __IMPORTANT__
-        
-        This wrapper is ONLY compatible with the newest release (V4).
-        
-        ## About IGDB
-        One of the principles behind IGDB.com is accessibility of data. We wish to share the data with anyone who wants to build cool video game oriented websites, apps and services. This means that the information you contribute to IGDB.com can be used by other projects as well.
-        
-        Thus, you are not only contributing to the value of this site but to thousands of other projects as well. We are looking forward to see what exciting game related projects you come up with. Happy coding!
-        
-        More info here:
-        * [About the API](https://www.igdb.com/api)
-        * [API Documentation](https://api-docs.igdb.com/)
-        
-        Information about the Querying language APICalypse:
-        * [apicalypse.io](https://apicalypse.io/)
-        
-        ## About the Wrapper
-        
-        The Wrapper can handle both the IGDB generated classes and JSON (Strings), I have chosen to make the API's Generated classes ([Protocol Buffers](https://developers.google.com/protocol-buffers/)) the standard way because it will make it easier to use as you don't have to create your own classes to hold the information.
-        
-        The package contains two modules: the `wrapper` which holds the tools for querying the API, and `igdbapi_pb2` which contains all of the generated classes for the Protocol Buffers.
-        
-        # Installation and Setup
-        
-        ```py
-        pip install igdb-api-v4
-        ```
-        
-        # Usage
-        
-        ## Using your Twitch Credentials
-        
-        Create a new IGDBWrapper object and give it your Client-ID and App Access Token:
-        
-        ```py
-        from igdb.wrapper import IGDBWrapper
-        wrapper = IGDBWrapper("YOUR_CLIENT_ID", "YOUR_APP_ACCESS_TOKEN")
-        ```
-        
-        ## How to use the wrapper
-        
-        Right now, the wrapper is very barebone and only has one wrapping function `api_request`, which queries the API when given an endpoint and an `APICalypse`-like query and returns a byte array with the results.
-        
-        More utilities will be added in the future, such as endpoint helper functions, JSON conversion, and Protobuf message parsing.
-        
-        * `api_request`
-          This method handles IGDB generated proto classes which returns an `ByteArray` to be used to fill the appropriate class.
-        ```py
-        '''With a wrapper instance already created'''
-        # JSON API request
-        byte_array = wrapper.api_request(
-                    'games',
-                    'fields id, name; offset 0; where platforms=48;'
-                  )
-        # parse into JSON however you like...
-        
-        # Protobuf API request
-        from igdb.igdbapi_pb2 import GameResult
-        byte_array = wrapper.api_request(
-                    'games.pb', # Note the '.pb' suffix at the endpoint
-                    'fields id, name; offset 0; where platforms=48;'
-                  )
-        games_message = GameResult()
-        games_message.ParseFromString(byte_array) # Fills the protobuf message object with the response
-        ```
-        
-        ## Exceptions
-        
-        The wrapper throws a [`requests.HTTPError`](https://2.python-requests.org/en/master/api/#requests.HTTPError) when an exception occurs from the API.
-        
-        ## Code Examples
-        
-        # Contributing / Developers
-        
-        ## Setup
-        ### Python
-        This project uses Python 3.7+ and pipenv to manage dependencies.
-        ```
-        pip install --user pipenv
-        pipenv install --dev
-        ```
-        
-        ### Protocol Buffers
-        
-        If you want to update the library to use the latest Protobuf file from api.igdb.com you can run ./update-protobuf.sh
-        
-        #### Windows
-        This project uses [protoc](https://github.com/protocolbuffers/protobuf/releases) to generate the protocol buffer wrapper.
-        ```
-        set PB_REL="https://github.com/protocolbuffers/protobuf/releases"
-        set PB_VERSION=3.13.0
-        set PB_OS=win
-        set PB_ARCH=64
-        curl -LO %PB_REL%/download/v%PB_VERSION%/protoc-%PB_VERSION%-%PB_OS%%PB_ARCH%.zip
-        ```
-        
-        Unzip to a protoc folder.
-        ```
-        cd protoc-3.13.0-win64\bin
-        protoc.exe -I=../../src/igdb --python_out=../../src/igdb igdbapi.proto
-        ```
-        
-        
-        ### Mac
-        Then run protoc:
-        ```
-        protoc -I=. --python_out=. igdbapi.proto
-        ```
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# IGDB Python API V4
+A Python wrapper for IGDB.com's Video Game Database API. 
+
+__IMPORTANT__
+
+This wrapper is ONLY compatible with the newest release (V4).
+
+## About IGDB
+One of the principles behind IGDB.com is accessibility of data. We wish to share the data with anyone who wants to build cool video game oriented websites, apps and services. This means that the information you contribute to IGDB.com can be used by other projects as well.
+
+Thus, you are not only contributing to the value of this site but to thousands of other projects as well. We are looking forward to see what exciting game related projects you come up with. Happy coding!
+
+More info here:
+* [About the API](https://www.igdb.com/api)
+* [API Documentation](https://api-docs.igdb.com/)
+
+Information about the Querying language APICalypse:
+* [apicalypse.io](https://apicalypse.io/)
+
+## About the Wrapper
+
+The Wrapper can handle both the IGDB generated classes and JSON (Strings), I have chosen to make the API's Generated classes ([Protocol Buffers](https://developers.google.com/protocol-buffers/)) the standard way because it will make it easier to use as you don't have to create your own classes to hold the information.
+
+The package contains two modules: the `wrapper` which holds the tools for querying the API, and `igdbapi_pb2` which contains all of the generated classes for the Protocol Buffers.
+
+# Installation and Setup
+
+```py
+pip install igdb-api-v4
+```
+
+# Usage
+
+## Using your Twitch Credentials
+
+Create a new IGDBWrapper object and give it your Client-ID and App Access Token:
+
+```py
+from igdb.wrapper import IGDBWrapper
+wrapper = IGDBWrapper("YOUR_CLIENT_ID", "YOUR_APP_ACCESS_TOKEN")
+```
+
+## How to use the wrapper
+
+Right now, the wrapper is very barebone and only has one wrapping function `api_request`, which queries the API when given an endpoint and an `APICalypse`-like query and returns a byte array with the results.
+
+More utilities will be added in the future, such as endpoint helper functions, JSON conversion, and Protobuf message parsing.
+
+* `api_request`
+  This method handles IGDB generated proto classes which returns an `ByteArray` to be used to fill the appropriate class.
+```py
+'''With a wrapper instance already created'''
+# JSON API request
+byte_array = wrapper.api_request(
+            'games',
+            'fields id, name; offset 0; where platforms=48;'
+          )
+# parse into JSON however you like...
+
+# Protobuf API request
+from igdb.igdbapi_pb2 import GameResult
+byte_array = wrapper.api_request(
+            'games.pb', # Note the '.pb' suffix at the endpoint
+            'fields id, name; offset 0; where platforms=48;'
+          )
+games_message = GameResult()
+games_message.ParseFromString(byte_array) # Fills the protobuf message object with the response
+```
+
+## Exceptions
+
+The wrapper throws a [`requests.HTTPError`](https://2.python-requests.org/en/master/api/#requests.HTTPError) when an exception occurs from the API.
+
+## Code Examples
+
+# Contributing / Developers
+
+## Setup
+### Python
+This project uses Python 3.7+ and pipenv to manage dependencies.
+```
+pip install --user pipenv
+pipenv install --dev
+```
+
+### Protocol Buffers
+
+If you want to update the library to use the latest Protobuf file from api.igdb.com you can run ./update-protobuf.sh
+
+#### Windows
+This project uses [protoc](https://github.com/protocolbuffers/protobuf/releases) to generate the protocol buffer wrapper.
+```
+set PB_REL="https://github.com/protocolbuffers/protobuf/releases"
+set PB_VERSION=3.13.0
+set PB_OS=win
+set PB_ARCH=64
+curl -LO %PB_REL%/download/v%PB_VERSION%/protoc-%PB_VERSION%-%PB_OS%%PB_ARCH%.zip
+```
+
+Unzip to a protoc folder.
+```
+cd protoc-3.13.0-win64\bin
+protoc.exe -I=../../src/igdb --python_out=../../src/igdb igdbapi.proto
+```
+
+
+### Mac
+Then run protoc:
+```
+protoc -I=. --python_out=. igdbapi.proto
+```
```

### Comparing `igdb-api-v4-0.1.0/setup.py` & `igdb-api-v4-0.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setup(
   name="igdb-api-v4",
-  version="0.1.0",
+  version="0.2.0",
   author="IGDB",
   author_email="dev@igdb.com",
   description="An API wrapper for IGDB API v4",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/twitchtv/igdb-api-python/",
   classifiers=[
```

### Comparing `igdb-api-v4-0.1.0/src/igdb/wrapper.py` & `igdb-api-v4-0.2.0/src/igdb/wrapper.py`

 * *Files identical despite different names*

