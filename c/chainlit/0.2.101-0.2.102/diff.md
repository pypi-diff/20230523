# Comparing `tmp/chainlit-0.2.101.tar.gz` & `tmp/chainlit-0.2.102.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainlit-0.2.101.tar", max compression
+gzip compressed data, was "chainlit-0.2.102.tar", max compression
```

## Comparing `chainlit-0.2.101.tar` & `chainlit-0.2.102.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     2505 2023-05-23 12:39:55.931848 chainlit-0.2.101/README.md
--rw-r--r--   0        0        0    12914 2023-05-23 12:39:19.308237 chainlit-0.2.101/chainlit/__init__.py
--rw-r--r--   0        0        0       87 2023-05-23 12:39:19.308237 chainlit-0.2.101/chainlit/__main__.py
--rw-r--r--   0        0        0      765 2023-05-23 12:39:19.308237 chainlit-0.2.101/chainlit/action.py
--rw-r--r--   0        0        0     3527 2023-05-23 12:39:19.308237 chainlit-0.2.101/chainlit/cli/__init__.py
--rw-r--r--   0        0        0     4093 2023-05-23 12:39:19.308237 chainlit-0.2.101/chainlit/cli/auth.py
--rw-r--r--   0        0        0     2594 2023-05-23 12:39:19.308237 chainlit-0.2.101/chainlit/cli/deploy.py
--rw-r--r--   0        0        0      716 2023-05-23 12:39:19.312237 chainlit-0.2.101/chainlit/cli/utils.py
--rw-r--r--   0        0        0     5278 2023-05-23 12:39:19.312237 chainlit-0.2.101/chainlit/client.py
--rw-r--r--   0        0        0     6273 2023-05-23 12:39:19.312237 chainlit-0.2.101/chainlit/config.py
--rw-r--r--   0        0        0     3293 2023-05-23 12:39:19.312237 chainlit-0.2.101/chainlit/element.py
--rw-r--r--   0        0        0  2071267 2023-05-23 12:40:20.771521 chainlit-0.2.101/chainlit/frontend/dist/assets/index-86181eb5.js
--rw-r--r--   0        0        0     4317 2023-05-23 12:40:20.771521 chainlit-0.2.101/chainlit/frontend/dist/assets/index-bdffdaa0.css
--rw-r--r--   0        0        0     8889 2023-05-23 12:40:20.767521 chainlit-0.2.101/chainlit/frontend/dist/assets/logo_dark-bc7401f6.svg
--rw-r--r--   0        0        0     8891 2023-05-23 12:40:20.771521 chainlit-0.2.101/chainlit/frontend/dist/assets/logo_light-f19fc2ea.svg
--rw-r--r--   0        0        0     6455 2023-05-23 12:40:19.563536 chainlit-0.2.101/chainlit/frontend/dist/favicon.svg
--rw-r--r--   0        0        0      772 2023-05-23 12:40:20.771521 chainlit-0.2.101/chainlit/frontend/dist/index.html
--rw-r--r--   0        0        0      344 2023-05-23 12:39:19.316237 chainlit-0.2.101/chainlit/hello.py
--rw-r--r--   0        0        0        0 2023-05-23 12:39:19.316237 chainlit-0.2.101/chainlit/lc/__init__.py
--rw-r--r--   0        0        0     8077 2023-05-23 12:39:19.316237 chainlit-0.2.101/chainlit/lc/chainlit_handler.py
--rw-r--r--   0        0        0      863 2023-05-23 12:39:19.316237 chainlit-0.2.101/chainlit/lc/monkey.py
--rw-r--r--   0        0        0     5388 2023-05-23 12:39:19.316237 chainlit-0.2.101/chainlit/lc/new_monkey.py
--rw-r--r--   0        0        0     4129 2023-05-23 12:39:19.316237 chainlit-0.2.101/chainlit/lc/old_monkey.py
--rw-r--r--   0        0        0     1068 2023-05-23 12:39:19.316237 chainlit-0.2.101/chainlit/lc/utils.py
--rw-r--r--   0        0        0      398 2023-05-23 12:39:19.316237 chainlit-0.2.101/chainlit/logger.py
--rw-r--r--   0        0        0     1618 2023-05-23 12:39:19.316237 chainlit-0.2.101/chainlit/markdown.py
--rw-r--r--   0        0        0     6747 2023-05-23 12:39:19.316237 chainlit-0.2.101/chainlit/sdk.py
--rw-r--r--   0        0        0    10159 2023-05-23 12:39:19.316237 chainlit-0.2.101/chainlit/server.py
--rw-r--r--   0        0        0      813 2023-05-23 12:39:19.316237 chainlit-0.2.101/chainlit/session.py
--rw-r--r--   0        0        0     2161 2023-05-23 12:39:19.316237 chainlit-0.2.101/chainlit/telemetry.py
--rw-r--r--   0        0        0      965 2023-05-23 12:39:19.316237 chainlit-0.2.101/chainlit/types.py
--rw-r--r--   0        0        0     1145 2023-05-23 12:39:19.316237 chainlit-0.2.101/chainlit/user_session.py
--rw-r--r--   0        0        0      196 2023-05-23 12:39:19.316237 chainlit-0.2.101/chainlit/version.py
--rw-r--r--   0        0        0     1551 2023-05-23 12:39:19.316237 chainlit-0.2.101/chainlit/watch.py
--rw-r--r--   0        0        0     1073 2023-05-23 12:39:19.316237 chainlit-0.2.101/pyproject.toml
--rw-r--r--   0        0        0     4018 1970-01-01 00:00:00.000000 chainlit-0.2.101/PKG-INFO
+-rw-r--r--   0        0        0     2505 2023-05-23 17:13:05.807116 chainlit-0.2.102/README.md
+-rw-r--r--   0        0        0    12914 2023-05-23 17:12:31.886880 chainlit-0.2.102/chainlit/__init__.py
+-rw-r--r--   0        0        0       87 2023-05-23 17:12:31.886880 chainlit-0.2.102/chainlit/__main__.py
+-rw-r--r--   0        0        0      765 2023-05-23 17:12:31.886880 chainlit-0.2.102/chainlit/action.py
+-rw-r--r--   0        0        0     3527 2023-05-23 17:12:31.886880 chainlit-0.2.102/chainlit/cli/__init__.py
+-rw-r--r--   0        0        0     4093 2023-05-23 17:12:31.886880 chainlit-0.2.102/chainlit/cli/auth.py
+-rw-r--r--   0        0        0     2594 2023-05-23 17:12:31.886880 chainlit-0.2.102/chainlit/cli/deploy.py
+-rw-r--r--   0        0        0      716 2023-05-23 17:12:31.886880 chainlit-0.2.102/chainlit/cli/utils.py
+-rw-r--r--   0        0        0     5278 2023-05-23 17:12:31.886880 chainlit-0.2.102/chainlit/client.py
+-rw-r--r--   0        0        0     6273 2023-05-23 17:12:31.886880 chainlit-0.2.102/chainlit/config.py
+-rw-r--r--   0        0        0     3293 2023-05-23 17:12:31.886880 chainlit-0.2.102/chainlit/element.py
+-rw-r--r--   0        0        0  2071267 2023-05-23 17:13:31.995299 chainlit-0.2.102/chainlit/frontend/dist/assets/index-86181eb5.js
+-rw-r--r--   0        0        0     4317 2023-05-23 17:13:31.995299 chainlit-0.2.102/chainlit/frontend/dist/assets/index-bdffdaa0.css
+-rw-r--r--   0        0        0     8889 2023-05-23 17:13:31.987299 chainlit-0.2.102/chainlit/frontend/dist/assets/logo_dark-bc7401f6.svg
+-rw-r--r--   0        0        0     8891 2023-05-23 17:13:31.995299 chainlit-0.2.102/chainlit/frontend/dist/assets/logo_light-f19fc2ea.svg
+-rw-r--r--   0        0        0     6455 2023-05-23 17:13:30.747291 chainlit-0.2.102/chainlit/frontend/dist/favicon.svg
+-rw-r--r--   0        0        0      772 2023-05-23 17:13:31.995299 chainlit-0.2.102/chainlit/frontend/dist/index.html
+-rw-r--r--   0        0        0      344 2023-05-23 17:12:31.890880 chainlit-0.2.102/chainlit/hello.py
+-rw-r--r--   0        0        0        0 2023-05-23 17:12:31.890880 chainlit-0.2.102/chainlit/lc/__init__.py
+-rw-r--r--   0        0        0     8077 2023-05-23 17:12:31.890880 chainlit-0.2.102/chainlit/lc/chainlit_handler.py
+-rw-r--r--   0        0        0      863 2023-05-23 17:12:31.890880 chainlit-0.2.102/chainlit/lc/monkey.py
+-rw-r--r--   0        0        0     5388 2023-05-23 17:12:31.890880 chainlit-0.2.102/chainlit/lc/new_monkey.py
+-rw-r--r--   0        0        0     4129 2023-05-23 17:12:31.890880 chainlit-0.2.102/chainlit/lc/old_monkey.py
+-rw-r--r--   0        0        0     1068 2023-05-23 17:12:31.890880 chainlit-0.2.102/chainlit/lc/utils.py
+-rw-r--r--   0        0        0      398 2023-05-23 17:12:31.890880 chainlit-0.2.102/chainlit/logger.py
+-rw-r--r--   0        0        0     1618 2023-05-23 17:12:31.890880 chainlit-0.2.102/chainlit/markdown.py
+-rw-r--r--   0        0        0     6747 2023-05-23 17:12:31.890880 chainlit-0.2.102/chainlit/sdk.py
+-rw-r--r--   0        0        0    10159 2023-05-23 17:12:31.890880 chainlit-0.2.102/chainlit/server.py
+-rw-r--r--   0        0        0      813 2023-05-23 17:12:31.890880 chainlit-0.2.102/chainlit/session.py
+-rw-r--r--   0        0        0     2161 2023-05-23 17:12:31.890880 chainlit-0.2.102/chainlit/telemetry.py
+-rw-r--r--   0        0        0      965 2023-05-23 17:12:31.890880 chainlit-0.2.102/chainlit/types.py
+-rw-r--r--   0        0        0     1145 2023-05-23 17:12:31.890880 chainlit-0.2.102/chainlit/user_session.py
+-rw-r--r--   0        0        0      196 2023-05-23 17:12:31.890880 chainlit-0.2.102/chainlit/version.py
+-rw-r--r--   0        0        0     1551 2023-05-23 17:12:31.890880 chainlit-0.2.102/chainlit/watch.py
+-rw-r--r--   0        0        0     1074 2023-05-23 17:12:31.890880 chainlit-0.2.102/pyproject.toml
+-rw-r--r--   0        0        0     4013 1970-01-01 00:00:00.000000 chainlit-0.2.102/PKG-INFO
```

### Comparing `chainlit-0.2.101/README.md` & `chainlit-0.2.102/README.md`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.101/chainlit/__init__.py` & `chainlit-0.2.102/chainlit/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.101/chainlit/action.py` & `chainlit-0.2.102/chainlit/action.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.101/chainlit/cli/__init__.py` & `chainlit-0.2.102/chainlit/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.101/chainlit/cli/auth.py` & `chainlit-0.2.102/chainlit/cli/auth.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.101/chainlit/cli/deploy.py` & `chainlit-0.2.102/chainlit/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.101/chainlit/cli/utils.py` & `chainlit-0.2.102/chainlit/cli/utils.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.101/chainlit/client.py` & `chainlit-0.2.102/chainlit/client.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.101/chainlit/config.py` & `chainlit-0.2.102/chainlit/config.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.101/chainlit/element.py` & `chainlit-0.2.102/chainlit/element.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.101/chainlit/frontend/dist/assets/index-86181eb5.js` & `chainlit-0.2.102/chainlit/frontend/dist/assets/index-86181eb5.js`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.101/chainlit/frontend/dist/assets/index-bdffdaa0.css` & `chainlit-0.2.102/chainlit/frontend/dist/assets/index-bdffdaa0.css`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.101/chainlit/frontend/dist/assets/logo_dark-bc7401f6.svg` & `chainlit-0.2.102/chainlit/frontend/dist/assets/logo_dark-bc7401f6.svg`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.101/chainlit/frontend/dist/assets/logo_light-f19fc2ea.svg` & `chainlit-0.2.102/chainlit/frontend/dist/assets/logo_light-f19fc2ea.svg`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.101/chainlit/frontend/dist/favicon.svg` & `chainlit-0.2.102/chainlit/frontend/dist/favicon.svg`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.101/chainlit/frontend/dist/index.html` & `chainlit-0.2.102/chainlit/frontend/dist/index.html`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.101/chainlit/lc/chainlit_handler.py` & `chainlit-0.2.102/chainlit/lc/chainlit_handler.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.101/chainlit/lc/monkey.py` & `chainlit-0.2.102/chainlit/lc/monkey.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.101/chainlit/lc/new_monkey.py` & `chainlit-0.2.102/chainlit/lc/new_monkey.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.101/chainlit/lc/old_monkey.py` & `chainlit-0.2.102/chainlit/lc/old_monkey.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.101/chainlit/lc/utils.py` & `chainlit-0.2.102/chainlit/lc/utils.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.101/chainlit/markdown.py` & `chainlit-0.2.102/chainlit/markdown.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.101/chainlit/sdk.py` & `chainlit-0.2.102/chainlit/sdk.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.101/chainlit/server.py` & `chainlit-0.2.102/chainlit/server.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.101/chainlit/session.py` & `chainlit-0.2.102/chainlit/session.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.101/chainlit/telemetry.py` & `chainlit-0.2.102/chainlit/telemetry.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.101/chainlit/types.py` & `chainlit-0.2.102/chainlit/types.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.101/chainlit/user_session.py` & `chainlit-0.2.102/chainlit/user_session.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.101/chainlit/watch.py` & `chainlit-0.2.102/chainlit/watch.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.2.101/PKG-INFO` & `chainlit-0.2.102/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainlit
-Version: 0.2.101
+Version: 0.2.102
 Summary: A faster way to build chatbot UIs.
 Home-page: https://github.com/Chainlit/chainlit
 License: Apache-2.0 license
 Keywords: LLM,Agents,gen ai,chat ui,chatbot ui,langchain
 Author: Chainlit
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
@@ -12,28 +12,28 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: auth0-python (>=4.1.1,<5.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: dataclasses_json (>=0.5.7,<0.6.0)
-Requires-Dist: flask (>=2.2.3,<3.0.0)
 Requires-Dist: flask-limiter (>=3.3.0,<4.0.0)
 Requires-Dist: flask_cors (>=3.0.10,<4.0.0)
 Requires-Dist: flask_socketio (>=5.3.3,<6.0.0)
 Requires-Dist: gevent (>=22.10.2,<23.0.0)
 Requires-Dist: gevent_websocket (>=0.10.1,<0.11.0)
+Requires-Dist: grpcio (==1.54.2)
 Requires-Dist: openai (>=0.27.2,<0.28.0)
 Requires-Dist: pydantic (>=1.10.6,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: python-graphql-client (>=0.4.3,<0.5.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: typing-inspect (==0.8.0)
 Requires-Dist: typing_extensions (==4.5.0)
-Requires-Dist: uptrace (>=1.17.0,<2.0.0)
+Requires-Dist: uptrace (>=1.18.0,<2.0.0)
 Requires-Dist: watchdog (>=3.0.0,<4.0.0)
 Requires-Dist: watchdog_gevent (>=0.1.1,<0.2.0)
 Project-URL: Repository, https://github.com/Chainlit/chainlit
 Description-Content-Type: text/markdown
 
 # Welcome to Chainlit 👋
```

