# Comparing `tmp/forestadmin_agent_flask-0.1.0b8.tar.gz` & `tmp/forestadmin_agent_flask-0.1.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forestadmin_agent_flask-0.1.0b8.tar", max compression
+gzip compressed data, was "forestadmin_agent_flask-0.1.0b9.tar", max compression
```

## Comparing `forestadmin_agent_flask-0.1.0b8.tar` & `forestadmin_agent_flask-0.1.0b9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2022-12-07 16:06:56.008806 forestadmin_agent_flask-0.1.0b8/README.md
--rw-r--r--   0        0        0        0 2022-12-07 16:06:56.008806 forestadmin_agent_flask-0.1.0b8/forestadmin/flask_agent/__init__.py
--rw-r--r--   0        0        0     5711 2022-12-07 16:06:56.008806 forestadmin_agent_flask-0.1.0b8/forestadmin/flask_agent/agent.py
--rw-r--r--   0        0        0        0 2022-12-07 16:06:56.008806 forestadmin_agent_flask-0.1.0b8/forestadmin/flask_agent/utils/__init__.py
--rw-r--r--   0        0        0      582 2022-12-07 16:06:56.008806 forestadmin_agent_flask-0.1.0b8/forestadmin/flask_agent/utils/dispatcher.py
--rw-r--r--   0        0        0     1449 2022-12-07 16:06:56.008806 forestadmin_agent_flask-0.1.0b8/forestadmin/flask_agent/utils/requests.py
--rw-r--r--   0        0        0     1330 2022-12-07 16:07:16.956853 forestadmin_agent_flask-0.1.0b8/pyproject.toml
--rw-r--r--   0        0        0      975 1970-01-01 00:00:00.000000 forestadmin_agent_flask-0.1.0b8/setup.py
--rw-r--r--   0        0        0      856 1970-01-01 00:00:00.000000 forestadmin_agent_flask-0.1.0b8/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-12-07 16:22:25.605515 forestadmin_agent_flask-0.1.0b9/README.md
+-rw-r--r--   0        0        0        0 2022-12-07 16:22:25.605515 forestadmin_agent_flask-0.1.0b9/forestadmin/flask_agent/__init__.py
+-rw-r--r--   0        0        0     5711 2022-12-07 16:22:25.605515 forestadmin_agent_flask-0.1.0b9/forestadmin/flask_agent/agent.py
+-rw-r--r--   0        0        0        0 2022-12-07 16:22:25.609515 forestadmin_agent_flask-0.1.0b9/forestadmin/flask_agent/utils/__init__.py
+-rw-r--r--   0        0        0      582 2022-12-07 16:22:25.609515 forestadmin_agent_flask-0.1.0b9/forestadmin/flask_agent/utils/dispatcher.py
+-rw-r--r--   0        0        0     1449 2022-12-07 16:22:25.609515 forestadmin_agent_flask-0.1.0b9/forestadmin/flask_agent/utils/requests.py
+-rw-r--r--   0        0        0     1330 2022-12-07 16:22:42.049444 forestadmin_agent_flask-0.1.0b9/pyproject.toml
+-rw-r--r--   0        0        0      975 1970-01-01 00:00:00.000000 forestadmin_agent_flask-0.1.0b9/setup.py
+-rw-r--r--   0        0        0      856 1970-01-01 00:00:00.000000 forestadmin_agent_flask-0.1.0b9/PKG-INFO
```

### Comparing `forestadmin_agent_flask-0.1.0b8/forestadmin/flask_agent/agent.py` & `forestadmin_agent_flask-0.1.0b9/forestadmin/flask_agent/agent.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_flask-0.1.0b8/forestadmin/flask_agent/utils/dispatcher.py` & `forestadmin_agent_flask-0.1.0b9/forestadmin/flask_agent/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_flask-0.1.0b8/forestadmin/flask_agent/utils/requests.py` & `forestadmin_agent_flask-0.1.0b9/forestadmin/flask_agent/utils/requests.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_flask-0.1.0b8/pyproject.toml` & `forestadmin_agent_flask-0.1.0b9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "forestadmin-agent-flask"
-version = "0.1.0-beta.8"
+version = "0.1.0-beta.9"
 description = ""
 authors = [ "Valentin Monté <valentinm@forestadmin.com>",]
 readme = "README.md"
 [[tool.poetry.packages]]
 include = "forestadmin"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
 typing-extensions = "~=4.2"
 tzdata = "~=2022.6"
 flask = "~=2.2.0"
-forestadmin-datasource-toolkit = "^0.1.0-beta.8"
-forestadmin-agent-toolkit = "^0.1.0-beta.8"
+forestadmin-datasource-toolkit = "^0.1.0-beta.9"
+forestadmin-agent-toolkit = "^0.1.0-beta.9"
 
 [tool.poetry.dependencies."backports.zoneinfo"]
 version = "~=0.2.1"
 python = "<3.9"
 extras = [ "tzdata",]
 
 [tool.poetry.group.test]
```

### Comparing `forestadmin_agent_flask-0.1.0b8/setup.py` & `forestadmin_agent_flask-0.1.0b9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 ['forestadmin', 'forestadmin.flask_agent', 'forestadmin.flask_agent.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['flask>=2.2.0,<2.3.0',
- 'forestadmin-agent-toolkit>=0.1.0-beta.8,<0.2.0',
- 'forestadmin-datasource-toolkit>=0.1.0-beta.8,<0.2.0',
+ 'forestadmin-agent-toolkit>=0.1.0-beta.9,<0.2.0',
+ 'forestadmin-datasource-toolkit>=0.1.0-beta.9,<0.2.0',
  'typing-extensions>=4.2,<5.0',
  'tzdata>=2022.6,<2023.0']
 
 extras_require = \
 {':python_version < "3.9"': ['backports.zoneinfo[tzdata]>=0.2.1,<0.3.0']}
 
 setup_kwargs = {
     'name': 'forestadmin-agent-flask',
-    'version': '0.1.0b8',
+    'version': '0.1.0b9',
     'description': '',
     'long_description': '',
     'author': 'Valentin Monté',
     'author_email': 'valentinm@forestadmin.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `forestadmin_agent_flask-0.1.0b8/PKG-INFO` & `forestadmin_agent_flask-0.1.0b9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: forestadmin-agent-flask
-Version: 0.1.0b8
+Version: 0.1.0b9
 Summary: 
 Author: Valentin Monté
 Author-email: valentinm@forestadmin.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: backports.zoneinfo[tzdata] (>=0.2.1,<0.3.0); python_version < "3.9"
 Requires-Dist: flask (>=2.2.0,<2.3.0)
-Requires-Dist: forestadmin-agent-toolkit (>=0.1.0-beta.8,<0.2.0)
-Requires-Dist: forestadmin-datasource-toolkit (>=0.1.0-beta.8,<0.2.0)
+Requires-Dist: forestadmin-agent-toolkit (>=0.1.0-beta.9,<0.2.0)
+Requires-Dist: forestadmin-datasource-toolkit (>=0.1.0-beta.9,<0.2.0)
 Requires-Dist: typing-extensions (>=4.2,<5.0)
 Requires-Dist: tzdata (>=2022.6,<2023.0)
 Description-Content-Type: text/markdown
```

